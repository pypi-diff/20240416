# Comparing `tmp/linearmodels-5.3.tar.gz` & `tmp/linearmodels-5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linearmodels-5.3.tar", last modified: Tue Sep 26 14:53:47 2023, max compression
+gzip compressed data, was "linearmodels-5.4.tar", last modified: Fri Jan  5 08:39:12 2024, max compression
```

## Comparing `linearmodels-5.3.tar` & `linearmodels-5.4.tar`

### file list

```diff
@@ -1,319 +1,319 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-26 14:53:47.835877 linearmodels-5.3/
--rw-r--r--   0 root         (0) root         (0)       46 2023-05-26 11:28:32.000000 linearmodels-5.3/.codacy.yml
--rw-r--r--   0 root         (0) root         (0)       24 2023-05-26 11:28:32.000000 linearmodels-5.3/.codebeatignore
--rw-r--r--   0 root         (0) root         (0)      805 2023-05-26 11:28:32.000000 linearmodels-5.3/.coveragerc
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-26 11:28:32.000000 linearmodels-5.3/.gitattributes
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-26 14:53:47.795877 linearmodels-5.3/.github/
--rw-r--r--   0 root         (0) root         (0)       41 2023-05-26 11:28:32.000000 linearmodels-5.3/.github/codeql.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-26 14:53:47.795877 linearmodels-5.3/.github/workflows/
--rw-r--r--   0 root         (0) root         (0)      971 2023-09-26 14:53:34.000000 linearmodels-5.3/.github/workflows/codeql.yml
--rw-r--r--   0 root         (0) root         (0)     1384 2023-09-26 14:53:34.000000 linearmodels-5.3/.github/workflows/cron-test.yml
--rw-r--r--   0 root         (0) root         (0)     1225 2023-09-26 14:53:34.000000 linearmodels-5.3/.github/workflows/generate-documentation.yml
--rw-r--r--   0 root         (0) root         (0)     1577 2023-05-26 11:28:32.000000 linearmodels-5.3/.gitignore
--rw-r--r--   0 root         (0) root         (0)       84 2023-05-26 11:28:32.000000 linearmodels-5.3/.lgtm.yml
--rw-r--r--   0 root         (0) root         (0)     1725 2023-05-26 11:28:32.000000 linearmodels-5.3/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)      445 2023-05-26 11:28:32.000000 linearmodels-5.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     8190 2023-09-26 14:53:47.835877 linearmodels-5.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6600 2023-05-26 11:28:32.000000 linearmodels-5.3/README.md
--rw-r--r--   0 root         (0) root         (0)     1210 2023-05-26 11:28:32.000000 linearmodels-5.3/appveyor.yml
--rw-r--r--   0 root         (0) root         (0)      628 2023-05-26 11:28:32.000000 linearmodels-5.3/azure-pipelines.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-26 14:53:47.795877 linearmodels-5.3/ci/
--rw-r--r--   0 root         (0) root         (0)     4489 2023-09-26 14:53:34.000000 linearmodels-5.3/ci/azure_template_posix.yml
--rw-r--r--   0 root         (0) root         (0)     1735 2023-05-26 11:28:32.000000 linearmodels-5.3/ci/azure_template_windows.yml
--rw-r--r--   0 root         (0) root         (0)      577 2023-05-26 11:28:32.000000 linearmodels-5.3/ci/install-posix.sh
--rw-r--r--   0 root         (0) root         (0)     1312 2023-05-26 11:28:32.000000 linearmodels-5.3/ci/push-docs-gh-pages.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-26 14:53:47.805877 linearmodels-5.3/doc/
--rw-r--r--   0 root         (0) root         (0)      614 2023-05-26 11:28:32.000000 linearmodels-5.3/doc/Makefile
--rw-r--r--   0 root         (0) root         (0)      837 2023-05-26 11:28:32.000000 linearmodels-5.3/doc/make.bat
--rw-r--r--   0 root         (0) root         (0)      178 2023-05-26 11:28:32.000000 linearmodels-5.3/doc/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-26 14:53:47.805877 linearmodels-5.3/doc/source/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-26 14:53:47.735877 linearmodels-5.3/doc/source/_static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-26 14:53:47.805877 linearmodels-5.3/doc/source/_static/css/
--rw-r--r--   0 root         (0) root         (0)      575 2023-05-26 11:28:32.000000 linearmodels-5.3/doc/source/_static/css/small_fixes.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-26 14:53:47.805877 linearmodels-5.3/doc/source/_static/icons/
--rw-r--r--   0 root         (0) root         (0)     9111 2023-05-26 11:28:32.000000 linearmodels-5.3/doc/source/_static/icons/android-chrome-192x192.png
--rw-r--r--   0 root         (0) root         (0)    27372 2023-05-26 11:28:32.000000 linearmodels-5.3/doc/source/_static/icons/android-chrome-512x512.png
--rw-r--r--   0 root         (0) root         (0)     8509 2023-05-26 11:28:32.000000 linearmodels-5.3/doc/source/_static/icons/apple-touch-icon.png
--rw-r--r--   0 root         (0) root         (0)      273 2023-05-26 11:28:32.000000 linearmodels-5.3/doc/source/_static/icons/browserconfig.xml
--rw-r--r--   0 root         (0) root         (0)     1204 2023-05-26 11:28:32.000000 linearmodels-5.3/doc/source/_static/icons/favicon-16x16.png
--rw-r--r--   0 root         (0) root         (0)     2041 2023-05-26 11:28:32.000000 linearmodels-5.3/doc/source/_static/icons/favicon-32x32.png
--rw-r--r--   0 root         (0) root         (0)    15086 2023-05-26 11:28:32.000000 linearmodels-5.3/doc/source/_static/icons/favicon.ico
--rw-r--r--   0 root         (0) root         (0)     7693 2023-05-26 11:28:32.000000 linearmodels-5.3/doc/source/_static/icons/mstile-144x144.png
--rw-r--r--   0 root         (0) root         (0)     7593 2023-05-26 11:28:32.000000 linearmodels-5.3/doc/source/_static/icons/mstile-150x150.png
--rw-r--r--   0 root         (0) root         (0)     8319 2023-05-26 11:28:32.000000 linearmodels-5.3/doc/source/_static/icons/mstile-310x150.png
--rw-r--r--   0 root         (0) root         (0)    16992 2023-05-26 11:28:32.000000 linearmodels-5.3/doc/source/_static/icons/mstile-310x310.png
--rw-r--r--   0 root         (0) root         (0)     5416 2023-05-26 11:28:32.000000 linearmodels-5.3/doc/source/_static/icons/mstile-70x70.png
--rw-r--r--   0 root         (0) root         (0)     4910 2023-05-26 11:28:32.000000 linearmodels-5.3/doc/source/_static/icons/safari-pinned-tab.svg
--rw-r--r--   0 root         (0) root         (0)      504 2023-05-26 11:28:32.000000 linearmodels-5.3/doc/source/_static/icons/site.webmanifest
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-26 14:53:47.805877 linearmodels-5.3/doc/source/_templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-26 14:53:47.815877 linearmodels-5.3/doc/source/_templates/autosummary/
--rw-r--r--   0 root         (0) root         (0)      117 2023-05-26 11:28:32.000000 linearmodels-5.3/doc/source/_templates/autosummary/attribute.rst
--rw-r--r--   0 root         (0) root         (0)      821 2023-05-26 11:28:32.000000 linearmodels-5.3/doc/source/_templates/autosummary/class.rst
--rw-r--r--   0 root         (0) root         (0)      118 2023-05-26 11:28:32.000000 linearmodels-5.3/doc/source/_templates/autosummary/member.rst
--rw-r--r--   0 root         (0) root         (0)      117 2023-05-26 11:28:32.000000 linearmodels-5.3/doc/source/_templates/autosummary/method.rst
--rw-r--r--   0 root         (0) root         (0)      113 2023-05-26 11:28:32.000000 linearmodels-5.3/doc/source/_templates/autosummary/minimal_module.rst
--rw-r--r--   0 root         (0) root         (0)      872 2023-05-26 11:28:32.000000 linearmodels-5.3/doc/source/_templates/layout.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-26 14:53:47.815877 linearmodels-5.3/doc/source/asset-pricing/
--rw-r--r--   0 root         (0) root         (0)      422 2023-05-26 11:28:32.000000 linearmodels-5.3/doc/source/asset-pricing/convert-lyx.cmd
--rw-r--r--   0 root         (0) root         (0)     2689 2023-05-26 11:28:32.000000 linearmodels-5.3/doc/source/asset-pricing/index.rst
--rw-r--r--   0 root         (0) root         (0)     3610 2023-05-26 11:28:32.000000 linearmodels-5.3/doc/source/asset-pricing/introduction.rst
--rw-r--r--   0 root         (0) root         (0)    23708 2023-05-26 11:28:32.000000 linearmodels-5.3/doc/source/asset-pricing/mathematical-detail.lyx
--rw-r--r--   0 root         (0) root         (0)     9122 2023-05-26 11:28:32.000000 linearmodels-5.3/doc/source/asset-pricing/mathematical-detail.txt
--rw-r--r--   0 root         (0) root         (0)      173 2023-05-26 11:28:32.000000 linearmodels-5.3/doc/source/asset-pricing/mathematical-formula.rst
--rw-r--r--   0 root         (0) root         (0)     1187 2023-05-26 11:28:32.000000 linearmodels-5.3/doc/source/asset-pricing/reference.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-26 14:53:47.815877 linearmodels-5.3/doc/source/changes/
--rw-r--r--   0 root         (0) root         (0)      577 2023-05-26 11:28:32.000000 linearmodels-5.3/doc/source/changes/3.0-2.0-1.0.rst
--rw-r--r--   0 root         (0) root         (0)    10957 2023-05-26 11:28:32.000000 linearmodels-5.3/doc/source/changes/4.0.rst
--rw-r--r--   0 root         (0) root         (0)      847 2023-09-26 14:53:34.000000 linearmodels-5.3/doc/source/changes/5.0.rst
--rw-r--r--   0 root         (0) root         (0)      164 2023-05-26 11:28:32.000000 linearmodels-5.3/doc/source/changes.rst
--rw-r--r--   0 root         (0) root         (0)      269 2023-05-26 11:28:32.000000 linearmodels-5.3/doc/source/compatibility.rst
--rw-r--r--   0 root         (0) root         (0)    15897 2023-09-26 14:53:34.000000 linearmodels-5.3/doc/source/conf.py
--rw-r--r--   0 root         (0) root         (0)      768 2023-05-26 11:28:32.000000 linearmodels-5.3/doc/source/contributing.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-26 14:53:47.815877 linearmodels-5.3/doc/source/images/
--rw-r--r--   0 root         (0) root         (0)     6817 2023-05-26 11:28:32.000000 linearmodels-5.3/doc/source/images/bw-logo.svg
--rw-r--r--   0 root         (0) root         (0)    15086 2023-05-26 11:28:32.000000 linearmodels-5.3/doc/source/images/favicon.ico
--rw-r--r--   0 root         (0) root         (0)    21193 2023-05-26 11:28:32.000000 linearmodels-5.3/doc/source/images/logo-text.svg
--rw-r--r--   0 root         (0) root         (0)     6392 2023-05-26 11:28:32.000000 linearmodels-5.3/doc/source/images/logo.svg
--rw-r--r--   0 root         (0) root         (0)     2543 2023-05-26 11:28:32.000000 linearmodels-5.3/doc/source/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-26 14:53:47.815877 linearmodels-5.3/doc/source/iv/
--rw-r--r--   0 root         (0) root         (0)      291 2023-05-26 11:28:32.000000 linearmodels-5.3/doc/source/iv/convert-lyx.cmd
--rw-r--r--   0 root         (0) root         (0)    34612 2023-05-26 11:28:32.000000 linearmodels-5.3/doc/source/iv/estimators.lyx
--rw-r--r--   0 root         (0) root         (0)    21743 2023-05-26 11:28:32.000000 linearmodels-5.3/doc/source/iv/estimators.txt
--rw-r--r--   0 root         (0) root         (0)     1255 2023-05-26 11:28:32.000000 linearmodels-5.3/doc/source/iv/index.rst
--rw-r--r--   0 root         (0) root         (0)     8663 2023-05-26 11:28:32.000000 linearmodels-5.3/doc/source/iv/introduction.rst
--rw-r--r--   0 root         (0) root         (0)      252 2023-05-26 11:28:32.000000 linearmodels-5.3/doc/source/iv/mathematical-formula.rst
--rw-r--r--   0 root         (0) root         (0)     2340 2023-05-26 11:28:32.000000 linearmodels-5.3/doc/source/iv/reference.rst
--rw-r--r--   0 root         (0) root         (0)      359 2023-05-26 11:28:32.000000 linearmodels-5.3/doc/source/names_wordlist.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-26 14:53:47.825877 linearmodels-5.3/doc/source/panel/
--rw-r--r--   0 root         (0) root         (0)      393 2023-05-26 11:28:32.000000 linearmodels-5.3/doc/source/panel/convert-lyx.cmd
--rw-r--r--   0 root         (0) root         (0)     1436 2023-05-26 11:28:32.000000 linearmodels-5.3/doc/source/panel/faq.rst
--rw-r--r--   0 root         (0) root         (0)     1656 2023-05-26 11:28:32.000000 linearmodels-5.3/doc/source/panel/index.rst
--rw-r--r--   0 root         (0) root         (0)     5724 2023-05-26 11:28:32.000000 linearmodels-5.3/doc/source/panel/introduction.rst
--rw-r--r--   0 root         (0) root         (0)    21824 2023-05-26 11:28:32.000000 linearmodels-5.3/doc/source/panel/mathematical-detail.lyx
--rw-r--r--   0 root         (0) root         (0)    12588 2023-05-26 11:28:32.000000 linearmodels-5.3/doc/source/panel/mathematical-detail.txt
--rw-r--r--   0 root         (0) root         (0)       71 2023-05-26 11:28:32.000000 linearmodels-5.3/doc/source/panel/mathematical-formula.rst
--rw-r--r--   0 root         (0) root         (0)     7697 2023-05-26 11:28:32.000000 linearmodels-5.3/doc/source/panel/pandas.rst
--rw-r--r--   0 root         (0) root         (0)     1676 2023-05-26 11:28:32.000000 linearmodels-5.3/doc/source/panel/reference.rst
--rw-r--r--   0 root         (0) root         (0)     2197 2023-05-26 11:28:32.000000 linearmodels-5.3/doc/source/plan.rst
--rw-r--r--   0 root         (0) root         (0)     2063 2023-05-26 11:28:32.000000 linearmodels-5.3/doc/source/references.rst
--rw-r--r--   0 root         (0) root         (0)     2170 2023-05-26 11:28:32.000000 linearmodels-5.3/doc/source/spelling_wordlist.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-26 14:53:47.825877 linearmodels-5.3/doc/source/system/
--rw-r--r--   0 root         (0) root         (0)      425 2023-05-26 11:28:32.000000 linearmodels-5.3/doc/source/system/convert-lyx.cmd
--rw-r--r--   0 root         (0) root         (0)     3911 2023-05-26 11:28:32.000000 linearmodels-5.3/doc/source/system/index.rst
--rw-r--r--   0 root         (0) root         (0)    27063 2023-05-26 11:28:32.000000 linearmodels-5.3/doc/source/system/mathematical-detail.lyx
--rw-r--r--   0 root         (0) root         (0)    17361 2023-05-26 11:28:32.000000 linearmodels-5.3/doc/source/system/mathematical-detail.txt
--rw-r--r--   0 root         (0) root         (0)      161 2023-05-26 11:28:32.000000 linearmodels-5.3/doc/source/system/mathematical-formula.rst
--rw-r--r--   0 root         (0) root         (0)     1781 2023-05-26 11:28:32.000000 linearmodels-5.3/doc/source/system/reference.rst
--rw-r--r--   0 root         (0) root         (0)      648 2023-05-26 11:28:32.000000 linearmodels-5.3/doc/source/utility.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-26 14:53:47.825877 linearmodels-5.3/examples/
--rw-r--r--   0 root         (0) root         (0)    13198 2023-05-26 11:28:32.000000 linearmodels-5.3/examples/asset-pricing_examples.ipynb
--rw-r--r--   0 root         (0) root         (0)     5352 2023-05-26 11:28:32.000000 linearmodels-5.3/examples/asset-pricing_formulas.ipynb
--rw-r--r--   0 root         (0) root         (0)     5051 2023-05-26 11:28:32.000000 linearmodels-5.3/examples/iv_absorbing-regression.ipynb
--rw-r--r--   0 root         (0) root         (0)    18612 2023-05-26 11:28:32.000000 linearmodels-5.3/examples/iv_advanced-examples.ipynb
--rw-r--r--   0 root         (0) root         (0)    23744 2023-05-26 11:28:32.000000 linearmodels-5.3/examples/iv_basic-examples.ipynb
--rw-r--r--   0 root         (0) root         (0)     7218 2023-05-26 11:28:32.000000 linearmodels-5.3/examples/iv_using-formulas.ipynb
--rw-r--r--   0 root         (0) root         (0)     7181 2023-05-26 11:28:32.000000 linearmodels-5.3/examples/panel_data-formats.ipynb
--rw-r--r--   0 root         (0) root         (0)    16882 2023-05-26 11:28:32.000000 linearmodels-5.3/examples/panel_examples.ipynb
--rw-r--r--   0 root         (0) root         (0)     6201 2023-05-26 11:28:32.000000 linearmodels-5.3/examples/panel_using-formulas.ipynb
--rw-r--r--   0 root         (0) root         (0)    35002 2023-05-26 11:28:32.000000 linearmodels-5.3/examples/system_correct-greene-table-10-1.png
--rw-r--r--   0 root         (0) root         (0)    17212 2023-05-26 11:28:32.000000 linearmodels-5.3/examples/system_correct-greene-table-10-2.png
--rw-r--r--   0 root         (0) root         (0)    31657 2023-05-26 11:28:32.000000 linearmodels-5.3/examples/system_correct-greene-table-10-3.png
--rw-r--r--   0 root         (0) root         (0)    27604 2023-05-26 11:28:32.000000 linearmodels-5.3/examples/system_examples.ipynb
--rw-r--r--   0 root         (0) root         (0)     6305 2023-05-26 11:28:32.000000 linearmodels-5.3/examples/system_formulas.ipynb
--rw-r--r--   0 root         (0) root         (0)    11652 2023-05-26 11:28:32.000000 linearmodels-5.3/examples/system_three-stage-ls.ipynb
--rw-r--r--   0 root         (0) root         (0)     4408 2023-05-26 11:28:32.000000 linearmodels-5.3/github_deploy_key.enc
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-26 14:53:47.735877 linearmodels-5.3/linearmodels/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-26 14:53:47.735877 linearmodels-5.3/linearmodels/__future__/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/__future__/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/__future__/ordering.py
--rw-r--r--   0 root         (0) root         (0)     3142 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/__init__.py
--rw-r--r--   0 root         (0) root         (0)      155 2023-09-26 14:53:47.000000 linearmodels-5.3/linearmodels/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-26 14:53:47.745877 linearmodels-5.3/linearmodels/asset_pricing/
--rw-r--r--   0 root         (0) root         (0)      156 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/asset_pricing/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10526 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/asset_pricing/covariance.py
--rw-r--r--   0 root         (0) root         (0)    41062 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/asset_pricing/model.py
--rw-r--r--   0 root         (0) root         (0)    10771 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/asset_pricing/results.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-26 14:53:47.745877 linearmodels-5.3/linearmodels/compat/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/compat/__init__.py
--rw-r--r--   0 root         (0) root         (0)      502 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/compat/statsmodels.py
--rw-r--r--   0 root         (0) root         (0)     1958 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-26 14:53:47.745877 linearmodels-5.3/linearmodels/datasets/
--rw-r--r--   0 root         (0) root         (0)      272 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/datasets/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-26 14:53:47.745877 linearmodels-5.3/linearmodels/datasets/birthweight/
--rw-r--r--   0 root         (0) root         (0)     1042 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/datasets/birthweight/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11243 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/datasets/birthweight/birthweight.csv.bz2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-26 14:53:47.745877 linearmodels-5.3/linearmodels/datasets/card/
--rw-r--r--   0 root         (0) root         (0)     2071 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/datasets/card/__init__.py
--rw-r--r--   0 root         (0) root         (0)    44790 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/datasets/card/card.csv.bz2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-26 14:53:47.745877 linearmodels-5.3/linearmodels/datasets/fertility/
--rw-r--r--   0 root         (0) root         (0)     1105 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/datasets/fertility/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7162 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/datasets/fertility/fertility.csv.bz2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-26 14:53:47.745877 linearmodels-5.3/linearmodels/datasets/french/
--rw-r--r--   0 root         (0) root         (0)     1422 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/datasets/french/__init__.py
--rw-r--r--   0 root         (0) root         (0)    48052 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/datasets/french/french.csv.bz2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-26 14:53:47.745877 linearmodels-5.3/linearmodels/datasets/fringe/
--rw-r--r--   0 root         (0) root         (0)     2122 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/datasets/fringe/__init__.py
--rw-r--r--   0 root         (0) root         (0)    26658 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/datasets/fringe/fringe.csv.bz2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-26 14:53:47.745877 linearmodels-5.3/linearmodels/datasets/jobtraining/
--rw-r--r--   0 root         (0) root         (0)     1715 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/datasets/jobtraining/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17898 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/datasets/jobtraining/jobtraining.csv.bz2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-26 14:53:47.745877 linearmodels-5.3/linearmodels/datasets/meps/
--rw-r--r--   0 root         (0) root         (0)     1122 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/datasets/meps/__init__.py
--rw-r--r--   0 root         (0) root         (0)   304022 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/datasets/meps/meps.csv.bz2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-26 14:53:47.745877 linearmodels-5.3/linearmodels/datasets/mroz/
--rw-r--r--   0 root         (0) root         (0)     1112 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/datasets/mroz/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19474 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/datasets/mroz/mroz.csv.bz2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-26 14:53:47.745877 linearmodels-5.3/linearmodels/datasets/munnell/
--rw-r--r--   0 root         (0) root         (0)      597 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/datasets/munnell/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21577 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/datasets/munnell/munnell.csv.bz2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-26 14:53:47.755877 linearmodels-5.3/linearmodels/datasets/wage/
--rw-r--r--   0 root         (0) root         (0)     1102 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/datasets/wage/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12142 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/datasets/wage/wage.csv.bz2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-26 14:53:47.755877 linearmodels-5.3/linearmodels/datasets/wage_panel/
--rw-r--r--   0 root         (0) root         (0)      869 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/datasets/wage_panel/__init__.py
--rw-r--r--   0 root         (0) root         (0)    42109 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/datasets/wage_panel/wage_panel.csv.bz2
--rw-r--r--   0 root         (0) root         (0)     1356 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/formula.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-26 14:53:47.755877 linearmodels-5.3/linearmodels/iv/
--rw-r--r--   0 root         (0) root         (0)      301 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/iv/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6444 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/iv/_utility.py
--rw-r--r--   0 root         (0) root         (0)    41525 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/iv/absorbing.py
--rw-r--r--   0 root         (0) root         (0)     2056 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/iv/common.py
--rw-r--r--   0 root         (0) root         (0)    18865 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/iv/covariance.py
--rw-r--r--   0 root         (0) root         (0)     7187 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/iv/data.py
--rw-r--r--   0 root         (0) root         (0)    14290 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/iv/gmm.py
--rw-r--r--   0 root         (0) root         (0)    54577 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/iv/model.py
--rw-r--r--   0 root         (0) root         (0)    58665 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/iv/results.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-26 14:53:47.835877 linearmodels-5.3/linearmodels/panel/
--rw-r--r--   0 root         (0) root         (0)      391 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/panel/__init__.py
--rw-r--r--   0 root         (0) root         (0)  1303816 2023-09-26 14:53:47.000000 linearmodels-5.3/linearmodels/panel/_utility.c
--rw-r--r--   0 root         (0) root         (0)      114 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/panel/_utility.pxi
--rw-r--r--   0 root         (0) root         (0)     2698 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/panel/_utility.pyx
--rw-r--r--   0 root         (0) root         (0)    24104 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/panel/covariance.py
--rw-r--r--   0 root         (0) root         (0)    24729 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/panel/data.py
--rw-r--r--   0 root         (0) root         (0)   114027 2023-09-08 09:53:46.000000 linearmodels-5.3/linearmodels/panel/model.py
--rw-r--r--   0 root         (0) root         (0)    37469 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/panel/results.py
--rw-r--r--   0 root         (0) root         (0)    20026 2023-09-08 09:53:46.000000 linearmodels-5.3/linearmodels/panel/utility.py
--rw-r--r--   0 root         (0) root         (0)       72 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-26 14:53:47.765877 linearmodels-5.3/linearmodels/shared/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/shared/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3945 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/shared/base.py
--rw-r--r--   0 root         (0) root         (0)     2873 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/shared/covariance.py
--rw-r--r--   0 root         (0) root         (0)     1020 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/shared/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     6922 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/shared/hypotheses.py
--rw-r--r--   0 root         (0) root         (0)     3127 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/shared/io.py
--rw-r--r--   0 root         (0) root         (0)     1693 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/shared/linalg.py
--rw-r--r--   0 root         (0) root         (0)     4441 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/shared/typed_getters.py
--rw-r--r--   0 root         (0) root         (0)     7736 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/shared/utility.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-26 14:53:47.765877 linearmodels-5.3/linearmodels/system/
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/system/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9568 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/system/_utility.py
--rw-r--r--   0 root         (0) root         (0)    24392 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/system/covariance.py
--rw-r--r--   0 root         (0) root         (0)    11324 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/system/gmm.py
--rw-r--r--   0 root         (0) root         (0)    76106 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/system/model.py
--rw-r--r--   0 root         (0) root         (0)    27787 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/system/results.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-26 14:53:47.765877 linearmodels-5.3/linearmodels/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-26 14:53:47.765877 linearmodels-5.3/linearmodels/tests/asset_pricing/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/tests/asset_pricing/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1394 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/tests/asset_pricing/_utility.py
--rw-r--r--   0 root         (0) root         (0)     1892 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/tests/asset_pricing/test_covariance.py
--rw-r--r--   0 root         (0) root         (0)     5064 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/tests/asset_pricing/test_formulas.py
--rw-r--r--   0 root         (0) root         (0)     3356 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/tests/asset_pricing/test_linear_factor_gmm.py
--rw-r--r--   0 root         (0) root         (0)    12283 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/tests/asset_pricing/test_linear_factor_model.py
--rw-r--r--   0 root         (0) root         (0)     7358 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/tests/asset_pricing/test_model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-26 14:53:47.765877 linearmodels-5.3/linearmodels/tests/datasets/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/tests/datasets/__init__.py
--rw-r--r--   0 root         (0) root         (0)      636 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/tests/datasets/test_datasets.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-26 14:53:47.775877 linearmodels-5.3/linearmodels/tests/iv/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/tests/iv/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1442 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/tests/iv/_utility.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-26 14:53:47.775877 linearmodels-5.3/linearmodels/tests/iv/results/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/tests/iv/results/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4154 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/tests/iv/results/execute-stata-simulated-data.py
--rw-r--r--   0 root         (0) root         (0)     2583 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/tests/iv/results/execute-stata.py
--rw-r--r--   0 root         (0) root         (0)     5777 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/tests/iv/results/housing.csv
--rw-r--r--   0 root         (0) root         (0)     3465 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/tests/iv/results/read_stata_results.py
--rw-r--r--   0 root         (0) root         (0)    97696 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/tests/iv/results/simulated-data.dta
--rw-r--r--   0 root         (0) root         (0)     2332 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/tests/iv/results/simulated-test-data.py
--rw-r--r--   0 root         (0) root         (0)    13232 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/tests/iv/results/stata-iv-housing-results.txt
--rw-r--r--   0 root         (0) root         (0)   547258 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/tests/iv/results/stata-iv-simulated-results.txt
--rw-r--r--   0 root         (0) root         (0)    24433 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/tests/iv/test_absorbing.py
--rw-r--r--   0 root         (0) root         (0)     7460 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/tests/iv/test_against_stata.py
--rw-r--r--   0 root         (0) root         (0)    10791 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/tests/iv/test_covariance.py
--rw-r--r--   0 root         (0) root         (0)     8041 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/tests/iv/test_data.py
--rw-r--r--   0 root         (0) root         (0)    11585 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/tests/iv/test_formulas.py
--rw-r--r--   0 root         (0) root         (0)     9641 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/tests/iv/test_gmm.py
--rw-r--r--   0 root         (0) root         (0)     2797 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/tests/iv/test_missing_data.py
--rw-r--r--   0 root         (0) root         (0)    15202 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/tests/iv/test_model.py
--rw-r--r--   0 root         (0) root         (0)     5577 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/tests/iv/test_postestimation.py
--rw-r--r--   0 root         (0) root         (0)     3293 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/tests/iv/test_results.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-26 14:53:47.785877 linearmodels-5.3/linearmodels/tests/panel/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/tests/panel/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8029 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/tests/panel/_utility.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-26 14:53:47.785877 linearmodels-5.3/linearmodels/tests/panel/results/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/tests/panel/results/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3374 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/tests/panel/results/execute-stata-simulated-data.py
--rw-r--r--   0 root         (0) root         (0)     1923 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/tests/panel/results/generate-panel-data.py
--rw-r--r--   0 root         (0) root         (0)     1994 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/tests/panel/results/parse_stata_results.py
--rw-r--r--   0 root         (0) root         (0)   578091 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/tests/panel/results/simulated-panel.dta
--rw-r--r--   0 root         (0) root         (0)    65624 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/tests/panel/results/stata-panel-simulated-results.txt
--rw-r--r--   0 root         (0) root         (0)    11968 2023-09-08 09:53:46.000000 linearmodels-5.3/linearmodels/tests/panel/test_between_ols.py
--rw-r--r--   0 root         (0) root         (0)     4972 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/tests/panel/test_cluster_input_formats.py
--rw-r--r--   0 root         (0) root         (0)    27934 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/tests/panel/test_data.py
--rw-r--r--   0 root         (0) root         (0)     5941 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/tests/panel/test_fama_macbeth.py
--rw-r--r--   0 root         (0) root         (0)     7010 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/tests/panel/test_firstdifference_ols.py
--rw-r--r--   0 root         (0) root         (0)    10720 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/tests/panel/test_formula.py
--rw-r--r--   0 root         (0) root         (0)     7966 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/tests/panel/test_model.py
--rw-r--r--   0 root         (0) root         (0)     7696 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/tests/panel/test_panel_covariance.py
--rw-r--r--   0 root         (0) root         (0)    51469 2023-09-08 09:53:46.000000 linearmodels-5.3/linearmodels/tests/panel/test_panel_ols.py
--rw-r--r--   0 root         (0) root         (0)     7953 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/tests/panel/test_pooled_ols.py
--rw-r--r--   0 root         (0) root         (0)     2738 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/tests/panel/test_random_effects.py
--rw-r--r--   0 root         (0) root         (0)     8478 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/tests/panel/test_results.py
--rw-r--r--   0 root         (0) root         (0)     4978 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/tests/panel/test_simulated_against_stata.py
--rw-r--r--   0 root         (0) root         (0)     9039 2023-09-08 09:53:46.000000 linearmodels-5.3/linearmodels/tests/panel/test_utility.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-26 14:53:47.785877 linearmodels-5.3/linearmodels/tests/shared/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/tests/shared/__init__.py
--rw-r--r--   0 root         (0) root         (0)      193 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/tests/shared/test_base.py
--rw-r--r--   0 root         (0) root         (0)     2561 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/tests/shared/test_typed_getters.py
--rw-r--r--   0 root         (0) root         (0)     7068 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/tests/shared/test_utility.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-26 14:53:47.795877 linearmodels-5.3/linearmodels/tests/system/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/tests/system/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12361 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/tests/system/_utility.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-26 14:53:47.795877 linearmodels-5.3/linearmodels/tests/system/results/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/tests/system/results/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2679 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/tests/system/results/execute-stata-3sls.py
--rw-r--r--   0 root         (0) root         (0)     3587 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/tests/system/results/execute-stata.py
--rw-r--r--   0 root         (0) root         (0)     1565 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/tests/system/results/generate_data.py
--rw-r--r--   0 root         (0) root         (0)     2682 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/tests/system/results/parse_stata_3sls_results.py
--rw-r--r--   0 root         (0) root         (0)     3357 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/tests/system/results/parse_stata_results.py
--rw-r--r--   0 root         (0) root         (0)    50504 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/tests/system/results/simulated-3sls.dta
--rw-r--r--   0 root         (0) root         (0)    55085 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/tests/system/results/simulated-sur.dta
--rw-r--r--   0 root         (0) root         (0)    85208 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/tests/system/results/stata-3sls-results.txt
--rw-r--r--   0 root         (0) root         (0)    32162 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/tests/system/results/stata-sur-results.txt
--rw-r--r--   0 root         (0) root         (0)    12026 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/tests/system/test_3sls.py
--rw-r--r--   0 root         (0) root         (0)     2518 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/tests/system/test_3sls_against_stata.py
--rw-r--r--   0 root         (0) root         (0)    12405 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/tests/system/test_covariance.py
--rw-r--r--   0 root         (0) root         (0)     1619 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/tests/system/test_equivalence.py
--rw-r--r--   0 root         (0) root         (0)     6999 2023-09-26 14:53:34.000000 linearmodels-5.3/linearmodels/tests/system/test_formulas.py
--rw-r--r--   0 root         (0) root         (0)    13455 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/tests/system/test_gmm.py
--rw-r--r--   0 root         (0) root         (0)    28960 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/tests/system/test_sur.py
--rw-r--r--   0 root         (0) root         (0)     5194 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/tests/system/test_sur_against_stata.py
--rw-r--r--   0 root         (0) root         (0)     6165 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/tests/system/test_utility.py
--rw-r--r--   0 root         (0) root         (0)     2091 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/tests/test_examples.py
--rw-r--r--   0 root         (0) root         (0)      710 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/tests/test_tester.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-26 14:53:47.795877 linearmodels-5.3/linearmodels/typing/
--rw-r--r--   0 root         (0) root         (0)     1617 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/typing/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1344 2023-05-26 11:28:32.000000 linearmodels-5.3/linearmodels/typing/data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-26 14:53:47.825877 linearmodels-5.3/linearmodels.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8190 2023-09-26 14:53:47.000000 linearmodels-5.3/linearmodels.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    16269 2023-09-26 14:53:47.000000 linearmodels-5.3/linearmodels.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-09-26 14:53:47.000000 linearmodels-5.3/linearmodels.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-09-26 14:53:46.000000 linearmodels-5.3/linearmodels.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      162 2023-09-26 14:53:47.000000 linearmodels-5.3/linearmodels.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       34 2023-09-26 14:53:47.000000 linearmodels-5.3/linearmodels.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      583 2023-09-08 09:53:46.000000 linearmodels-5.3/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      260 2023-09-08 09:53:46.000000 linearmodels-5.3/requirements-dev.txt
--rw-r--r--   0 root         (0) root         (0)      121 2023-09-08 09:53:46.000000 linearmodels-5.3/requirements-test.txt
--rw-r--r--   0 root         (0) root         (0)      176 2023-09-26 14:53:34.000000 linearmodels-5.3/requirements.txt
--rw-r--r--   0 root         (0) root         (0)     2143 2023-09-26 14:53:47.835877 linearmodels-5.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     5213 2023-09-26 14:53:34.000000 linearmodels-5.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-05 08:39:12.137550 linearmodels-5.4/
+-rw-r--r--   0 root         (0) root         (0)       46 2023-05-26 11:28:32.000000 linearmodels-5.4/.codacy.yml
+-rw-r--r--   0 root         (0) root         (0)       24 2023-05-26 11:28:32.000000 linearmodels-5.4/.codebeatignore
+-rw-r--r--   0 root         (0) root         (0)      805 2023-05-26 11:28:32.000000 linearmodels-5.4/.coveragerc
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-26 11:28:32.000000 linearmodels-5.4/.gitattributes
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-05 08:39:12.077550 linearmodels-5.4/.github/
+-rw-r--r--   0 root         (0) root         (0)       41 2023-05-26 11:28:32.000000 linearmodels-5.4/.github/codeql.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-05 08:39:12.077550 linearmodels-5.4/.github/workflows/
+-rw-r--r--   0 root         (0) root         (0)      971 2024-01-02 12:10:00.000000 linearmodels-5.4/.github/workflows/codeql.yml
+-rw-r--r--   0 root         (0) root         (0)     1462 2024-01-02 12:10:00.000000 linearmodels-5.4/.github/workflows/cron-test.yml
+-rw-r--r--   0 root         (0) root         (0)     1225 2024-01-02 12:10:00.000000 linearmodels-5.4/.github/workflows/generate-documentation.yml
+-rw-r--r--   0 root         (0) root         (0)     1577 2023-05-26 11:28:32.000000 linearmodels-5.4/.gitignore
+-rw-r--r--   0 root         (0) root         (0)       84 2023-05-26 11:28:32.000000 linearmodels-5.4/.lgtm.yml
+-rw-r--r--   0 root         (0) root         (0)     1725 2023-05-26 11:28:32.000000 linearmodels-5.4/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)      445 2023-05-26 11:28:32.000000 linearmodels-5.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     7932 2024-01-05 08:39:12.137550 linearmodels-5.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6342 2024-01-05 08:38:51.000000 linearmodels-5.4/README.md
+-rw-r--r--   0 root         (0) root         (0)      630 2024-01-05 08:38:51.000000 linearmodels-5.4/azure-pipelines.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-05 08:39:12.077550 linearmodels-5.4/ci/
+-rw-r--r--   0 root         (0) root         (0)     5348 2024-01-05 08:38:51.000000 linearmodels-5.4/ci/azure_template_posix.yml
+-rw-r--r--   0 root         (0) root         (0)     1735 2023-05-26 11:28:32.000000 linearmodels-5.4/ci/azure_template_windows.yml
+-rw-r--r--   0 root         (0) root         (0)      959 2024-01-04 11:19:21.000000 linearmodels-5.4/ci/install-posix.sh
+-rw-r--r--   0 root         (0) root         (0)     1312 2023-05-26 11:28:32.000000 linearmodels-5.4/ci/push-docs-gh-pages.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-05 08:39:12.077550 linearmodels-5.4/doc/
+-rw-r--r--   0 root         (0) root         (0)      614 2023-05-26 11:28:32.000000 linearmodels-5.4/doc/Makefile
+-rw-r--r--   0 root         (0) root         (0)      988 2024-01-05 08:38:51.000000 linearmodels-5.4/doc/make.bat
+-rw-r--r--   0 root         (0) root         (0)      180 2024-01-05 08:38:51.000000 linearmodels-5.4/doc/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-05 08:39:12.077550 linearmodels-5.4/doc/source/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-05 08:39:12.007550 linearmodels-5.4/doc/source/_static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-05 08:39:12.077550 linearmodels-5.4/doc/source/_static/css/
+-rw-r--r--   0 root         (0) root         (0)      575 2023-05-26 11:28:32.000000 linearmodels-5.4/doc/source/_static/css/small_fixes.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-05 08:39:12.087550 linearmodels-5.4/doc/source/_static/icons/
+-rw-r--r--   0 root         (0) root         (0)     9111 2023-05-26 11:28:32.000000 linearmodels-5.4/doc/source/_static/icons/android-chrome-192x192.png
+-rw-r--r--   0 root         (0) root         (0)    27372 2023-05-26 11:28:32.000000 linearmodels-5.4/doc/source/_static/icons/android-chrome-512x512.png
+-rw-r--r--   0 root         (0) root         (0)     8509 2023-05-26 11:28:32.000000 linearmodels-5.4/doc/source/_static/icons/apple-touch-icon.png
+-rw-r--r--   0 root         (0) root         (0)      273 2023-05-26 11:28:32.000000 linearmodels-5.4/doc/source/_static/icons/browserconfig.xml
+-rw-r--r--   0 root         (0) root         (0)     1204 2023-05-26 11:28:32.000000 linearmodels-5.4/doc/source/_static/icons/favicon-16x16.png
+-rw-r--r--   0 root         (0) root         (0)     2041 2023-05-26 11:28:32.000000 linearmodels-5.4/doc/source/_static/icons/favicon-32x32.png
+-rw-r--r--   0 root         (0) root         (0)    15086 2023-05-26 11:28:32.000000 linearmodels-5.4/doc/source/_static/icons/favicon.ico
+-rw-r--r--   0 root         (0) root         (0)     7693 2023-05-26 11:28:32.000000 linearmodels-5.4/doc/source/_static/icons/mstile-144x144.png
+-rw-r--r--   0 root         (0) root         (0)     7593 2023-05-26 11:28:32.000000 linearmodels-5.4/doc/source/_static/icons/mstile-150x150.png
+-rw-r--r--   0 root         (0) root         (0)     8319 2023-05-26 11:28:32.000000 linearmodels-5.4/doc/source/_static/icons/mstile-310x150.png
+-rw-r--r--   0 root         (0) root         (0)    16992 2023-05-26 11:28:32.000000 linearmodels-5.4/doc/source/_static/icons/mstile-310x310.png
+-rw-r--r--   0 root         (0) root         (0)     5416 2023-05-26 11:28:32.000000 linearmodels-5.4/doc/source/_static/icons/mstile-70x70.png
+-rw-r--r--   0 root         (0) root         (0)     4910 2023-05-26 11:28:32.000000 linearmodels-5.4/doc/source/_static/icons/safari-pinned-tab.svg
+-rw-r--r--   0 root         (0) root         (0)      504 2023-05-26 11:28:32.000000 linearmodels-5.4/doc/source/_static/icons/site.webmanifest
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-05 08:39:12.087550 linearmodels-5.4/doc/source/_templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-05 08:39:12.087550 linearmodels-5.4/doc/source/_templates/autosummary/
+-rw-r--r--   0 root         (0) root         (0)      117 2023-05-26 11:28:32.000000 linearmodels-5.4/doc/source/_templates/autosummary/attribute.rst
+-rw-r--r--   0 root         (0) root         (0)      821 2023-05-26 11:28:32.000000 linearmodels-5.4/doc/source/_templates/autosummary/class.rst
+-rw-r--r--   0 root         (0) root         (0)      118 2023-05-26 11:28:32.000000 linearmodels-5.4/doc/source/_templates/autosummary/member.rst
+-rw-r--r--   0 root         (0) root         (0)      117 2023-05-26 11:28:32.000000 linearmodels-5.4/doc/source/_templates/autosummary/method.rst
+-rw-r--r--   0 root         (0) root         (0)      113 2023-05-26 11:28:32.000000 linearmodels-5.4/doc/source/_templates/autosummary/minimal_module.rst
+-rw-r--r--   0 root         (0) root         (0)      872 2023-05-26 11:28:32.000000 linearmodels-5.4/doc/source/_templates/layout.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-05 08:39:12.087550 linearmodels-5.4/doc/source/asset-pricing/
+-rw-r--r--   0 root         (0) root         (0)      422 2023-05-26 11:28:32.000000 linearmodels-5.4/doc/source/asset-pricing/convert-lyx.cmd
+-rw-r--r--   0 root         (0) root         (0)     2689 2023-05-26 11:28:32.000000 linearmodels-5.4/doc/source/asset-pricing/index.rst
+-rw-r--r--   0 root         (0) root         (0)     3610 2023-05-26 11:28:32.000000 linearmodels-5.4/doc/source/asset-pricing/introduction.rst
+-rw-r--r--   0 root         (0) root         (0)    23708 2023-05-26 11:28:32.000000 linearmodels-5.4/doc/source/asset-pricing/mathematical-detail.lyx
+-rw-r--r--   0 root         (0) root         (0)     9122 2023-05-26 11:28:32.000000 linearmodels-5.4/doc/source/asset-pricing/mathematical-detail.txt
+-rw-r--r--   0 root         (0) root         (0)      173 2023-05-26 11:28:32.000000 linearmodels-5.4/doc/source/asset-pricing/mathematical-formula.rst
+-rw-r--r--   0 root         (0) root         (0)     1187 2023-05-26 11:28:32.000000 linearmodels-5.4/doc/source/asset-pricing/reference.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-05 08:39:12.087550 linearmodels-5.4/doc/source/changes/
+-rw-r--r--   0 root         (0) root         (0)      577 2023-05-26 11:28:32.000000 linearmodels-5.4/doc/source/changes/3.0-2.0-1.0.rst
+-rw-r--r--   0 root         (0) root         (0)    10957 2023-05-26 11:28:32.000000 linearmodels-5.4/doc/source/changes/4.0.rst
+-rw-r--r--   0 root         (0) root         (0)      944 2024-01-05 08:38:51.000000 linearmodels-5.4/doc/source/changes/5.0.rst
+-rw-r--r--   0 root         (0) root         (0)      164 2023-05-26 11:28:32.000000 linearmodels-5.4/doc/source/changes.rst
+-rw-r--r--   0 root         (0) root         (0)      269 2023-05-26 11:28:32.000000 linearmodels-5.4/doc/source/compatibility.rst
+-rw-r--r--   0 root         (0) root         (0)    15895 2024-01-02 12:10:00.000000 linearmodels-5.4/doc/source/conf.py
+-rw-r--r--   0 root         (0) root         (0)      768 2023-05-26 11:28:32.000000 linearmodels-5.4/doc/source/contributing.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-05 08:39:12.087550 linearmodels-5.4/doc/source/images/
+-rw-r--r--   0 root         (0) root         (0)     6817 2023-05-26 11:28:32.000000 linearmodels-5.4/doc/source/images/bw-logo.svg
+-rw-r--r--   0 root         (0) root         (0)    15086 2023-05-26 11:28:32.000000 linearmodels-5.4/doc/source/images/favicon.ico
+-rw-r--r--   0 root         (0) root         (0)    21193 2023-05-26 11:28:32.000000 linearmodels-5.4/doc/source/images/logo-text.svg
+-rw-r--r--   0 root         (0) root         (0)     6392 2023-05-26 11:28:32.000000 linearmodels-5.4/doc/source/images/logo.svg
+-rw-r--r--   0 root         (0) root         (0)     2543 2023-05-26 11:28:32.000000 linearmodels-5.4/doc/source/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-05 08:39:12.097550 linearmodels-5.4/doc/source/iv/
+-rw-r--r--   0 root         (0) root         (0)      291 2023-05-26 11:28:32.000000 linearmodels-5.4/doc/source/iv/convert-lyx.cmd
+-rw-r--r--   0 root         (0) root         (0)    34612 2023-05-26 11:28:32.000000 linearmodels-5.4/doc/source/iv/estimators.lyx
+-rw-r--r--   0 root         (0) root         (0)    21743 2023-05-26 11:28:32.000000 linearmodels-5.4/doc/source/iv/estimators.txt
+-rw-r--r--   0 root         (0) root         (0)     1255 2023-05-26 11:28:32.000000 linearmodels-5.4/doc/source/iv/index.rst
+-rw-r--r--   0 root         (0) root         (0)     8663 2023-05-26 11:28:32.000000 linearmodels-5.4/doc/source/iv/introduction.rst
+-rw-r--r--   0 root         (0) root         (0)      252 2023-05-26 11:28:32.000000 linearmodels-5.4/doc/source/iv/mathematical-formula.rst
+-rw-r--r--   0 root         (0) root         (0)     2340 2023-05-26 11:28:32.000000 linearmodels-5.4/doc/source/iv/reference.rst
+-rw-r--r--   0 root         (0) root         (0)      359 2023-05-26 11:28:32.000000 linearmodels-5.4/doc/source/names_wordlist.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-05 08:39:12.097550 linearmodels-5.4/doc/source/panel/
+-rw-r--r--   0 root         (0) root         (0)      393 2023-05-26 11:28:32.000000 linearmodels-5.4/doc/source/panel/convert-lyx.cmd
+-rw-r--r--   0 root         (0) root         (0)     1436 2023-05-26 11:28:32.000000 linearmodels-5.4/doc/source/panel/faq.rst
+-rw-r--r--   0 root         (0) root         (0)     1656 2023-05-26 11:28:32.000000 linearmodels-5.4/doc/source/panel/index.rst
+-rw-r--r--   0 root         (0) root         (0)     5724 2023-05-26 11:28:32.000000 linearmodels-5.4/doc/source/panel/introduction.rst
+-rw-r--r--   0 root         (0) root         (0)    21824 2023-05-26 11:28:32.000000 linearmodels-5.4/doc/source/panel/mathematical-detail.lyx
+-rw-r--r--   0 root         (0) root         (0)    12588 2023-05-26 11:28:32.000000 linearmodels-5.4/doc/source/panel/mathematical-detail.txt
+-rw-r--r--   0 root         (0) root         (0)       71 2023-05-26 11:28:32.000000 linearmodels-5.4/doc/source/panel/mathematical-formula.rst
+-rw-r--r--   0 root         (0) root         (0)     7697 2023-05-26 11:28:32.000000 linearmodels-5.4/doc/source/panel/pandas.rst
+-rw-r--r--   0 root         (0) root         (0)     1676 2023-05-26 11:28:32.000000 linearmodels-5.4/doc/source/panel/reference.rst
+-rw-r--r--   0 root         (0) root         (0)     2197 2023-05-26 11:28:32.000000 linearmodels-5.4/doc/source/plan.rst
+-rw-r--r--   0 root         (0) root         (0)     2063 2023-05-26 11:28:32.000000 linearmodels-5.4/doc/source/references.rst
+-rw-r--r--   0 root         (0) root         (0)     2170 2023-05-26 11:28:32.000000 linearmodels-5.4/doc/source/spelling_wordlist.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-05 08:39:12.097550 linearmodels-5.4/doc/source/system/
+-rw-r--r--   0 root         (0) root         (0)      425 2023-05-26 11:28:32.000000 linearmodels-5.4/doc/source/system/convert-lyx.cmd
+-rw-r--r--   0 root         (0) root         (0)     3911 2023-05-26 11:28:32.000000 linearmodels-5.4/doc/source/system/index.rst
+-rw-r--r--   0 root         (0) root         (0)    27063 2023-05-26 11:28:32.000000 linearmodels-5.4/doc/source/system/mathematical-detail.lyx
+-rw-r--r--   0 root         (0) root         (0)    17361 2023-05-26 11:28:32.000000 linearmodels-5.4/doc/source/system/mathematical-detail.txt
+-rw-r--r--   0 root         (0) root         (0)      161 2023-05-26 11:28:32.000000 linearmodels-5.4/doc/source/system/mathematical-formula.rst
+-rw-r--r--   0 root         (0) root         (0)     1781 2023-05-26 11:28:32.000000 linearmodels-5.4/doc/source/system/reference.rst
+-rw-r--r--   0 root         (0) root         (0)      648 2023-05-26 11:28:32.000000 linearmodels-5.4/doc/source/utility.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-05 08:39:12.107550 linearmodels-5.4/examples/
+-rw-r--r--   0 root         (0) root         (0)    13119 2024-01-02 12:10:00.000000 linearmodels-5.4/examples/asset-pricing_examples.ipynb
+-rw-r--r--   0 root         (0) root         (0)     5351 2024-01-02 12:10:00.000000 linearmodels-5.4/examples/asset-pricing_formulas.ipynb
+-rw-r--r--   0 root         (0) root         (0)     5050 2024-01-02 12:10:00.000000 linearmodels-5.4/examples/iv_absorbing-regression.ipynb
+-rw-r--r--   0 root         (0) root         (0)    18611 2024-01-02 12:10:00.000000 linearmodels-5.4/examples/iv_advanced-examples.ipynb
+-rw-r--r--   0 root         (0) root         (0)    23743 2024-01-02 12:10:00.000000 linearmodels-5.4/examples/iv_basic-examples.ipynb
+-rw-r--r--   0 root         (0) root         (0)     6749 2024-01-02 12:10:00.000000 linearmodels-5.4/examples/iv_using-formulas.ipynb
+-rw-r--r--   0 root         (0) root         (0)     7180 2024-01-02 12:10:00.000000 linearmodels-5.4/examples/panel_data-formats.ipynb
+-rw-r--r--   0 root         (0) root         (0)    16881 2024-01-02 12:10:00.000000 linearmodels-5.4/examples/panel_examples.ipynb
+-rw-r--r--   0 root         (0) root         (0)     6200 2024-01-02 12:10:00.000000 linearmodels-5.4/examples/panel_using-formulas.ipynb
+-rw-r--r--   0 root         (0) root         (0)    35002 2023-05-26 11:28:32.000000 linearmodels-5.4/examples/system_correct-greene-table-10-1.png
+-rw-r--r--   0 root         (0) root         (0)    17212 2023-05-26 11:28:32.000000 linearmodels-5.4/examples/system_correct-greene-table-10-2.png
+-rw-r--r--   0 root         (0) root         (0)    31657 2023-05-26 11:28:32.000000 linearmodels-5.4/examples/system_correct-greene-table-10-3.png
+-rw-r--r--   0 root         (0) root         (0)    27603 2024-01-02 12:10:00.000000 linearmodels-5.4/examples/system_examples.ipynb
+-rw-r--r--   0 root         (0) root         (0)     6148 2024-01-02 12:10:00.000000 linearmodels-5.4/examples/system_formulas.ipynb
+-rw-r--r--   0 root         (0) root         (0)    11651 2024-01-02 12:10:00.000000 linearmodels-5.4/examples/system_three-stage-ls.ipynb
+-rw-r--r--   0 root         (0) root         (0)     4408 2023-05-26 11:28:32.000000 linearmodels-5.4/github_deploy_key.enc
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-05 08:39:12.107550 linearmodels-5.4/linearmodels/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-05 08:39:12.107550 linearmodels-5.4/linearmodels/__future__/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/__future__/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/__future__/ordering.py
+-rw-r--r--   0 root         (0) root         (0)     3142 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      155 2024-01-05 08:39:11.000000 linearmodels-5.4/linearmodels/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-05 08:39:12.107550 linearmodels-5.4/linearmodels/asset_pricing/
+-rw-r--r--   0 root         (0) root         (0)      156 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/asset_pricing/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10526 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/asset_pricing/covariance.py
+-rw-r--r--   0 root         (0) root         (0)    41062 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/asset_pricing/model.py
+-rw-r--r--   0 root         (0) root         (0)    10771 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/asset_pricing/results.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-05 08:39:12.107550 linearmodels-5.4/linearmodels/compat/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/compat/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      302 2024-01-04 11:19:21.000000 linearmodels-5.4/linearmodels/compat/pandas.py
+-rw-r--r--   0 root         (0) root         (0)      502 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/compat/statsmodels.py
+-rw-r--r--   0 root         (0) root         (0)     1958 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-05 08:39:12.107550 linearmodels-5.4/linearmodels/datasets/
+-rw-r--r--   0 root         (0) root         (0)      272 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/datasets/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-05 08:39:12.107550 linearmodels-5.4/linearmodels/datasets/birthweight/
+-rw-r--r--   0 root         (0) root         (0)     1042 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/datasets/birthweight/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11243 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/datasets/birthweight/birthweight.csv.bz2
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-05 08:39:12.107550 linearmodels-5.4/linearmodels/datasets/card/
+-rw-r--r--   0 root         (0) root         (0)     2071 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/datasets/card/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    44790 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/datasets/card/card.csv.bz2
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-05 08:39:12.107550 linearmodels-5.4/linearmodels/datasets/fertility/
+-rw-r--r--   0 root         (0) root         (0)     1105 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/datasets/fertility/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7162 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/datasets/fertility/fertility.csv.bz2
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-05 08:39:12.107550 linearmodels-5.4/linearmodels/datasets/french/
+-rw-r--r--   0 root         (0) root         (0)     1422 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/datasets/french/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    48052 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/datasets/french/french.csv.bz2
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-05 08:39:12.107550 linearmodels-5.4/linearmodels/datasets/fringe/
+-rw-r--r--   0 root         (0) root         (0)     2122 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/datasets/fringe/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    26658 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/datasets/fringe/fringe.csv.bz2
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-05 08:39:12.107550 linearmodels-5.4/linearmodels/datasets/jobtraining/
+-rw-r--r--   0 root         (0) root         (0)     1715 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/datasets/jobtraining/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17898 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/datasets/jobtraining/jobtraining.csv.bz2
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-05 08:39:12.107550 linearmodels-5.4/linearmodels/datasets/meps/
+-rw-r--r--   0 root         (0) root         (0)     1122 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/datasets/meps/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   304022 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/datasets/meps/meps.csv.bz2
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-05 08:39:12.117550 linearmodels-5.4/linearmodels/datasets/mroz/
+-rw-r--r--   0 root         (0) root         (0)     1112 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/datasets/mroz/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19474 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/datasets/mroz/mroz.csv.bz2
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-05 08:39:12.117550 linearmodels-5.4/linearmodels/datasets/munnell/
+-rw-r--r--   0 root         (0) root         (0)      597 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/datasets/munnell/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21577 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/datasets/munnell/munnell.csv.bz2
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-05 08:39:12.117550 linearmodels-5.4/linearmodels/datasets/wage/
+-rw-r--r--   0 root         (0) root         (0)     1102 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/datasets/wage/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12142 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/datasets/wage/wage.csv.bz2
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-05 08:39:12.117550 linearmodels-5.4/linearmodels/datasets/wage_panel/
+-rw-r--r--   0 root         (0) root         (0)      869 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/datasets/wage_panel/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    42109 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/datasets/wage_panel/wage_panel.csv.bz2
+-rw-r--r--   0 root         (0) root         (0)     1356 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/formula.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-05 08:39:12.117550 linearmodels-5.4/linearmodels/iv/
+-rw-r--r--   0 root         (0) root         (0)      301 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/iv/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6444 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/iv/_utility.py
+-rw-r--r--   0 root         (0) root         (0)    41525 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/iv/absorbing.py
+-rw-r--r--   0 root         (0) root         (0)     2056 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/iv/common.py
+-rw-r--r--   0 root         (0) root         (0)    18865 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/iv/covariance.py
+-rw-r--r--   0 root         (0) root         (0)     7187 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/iv/data.py
+-rw-r--r--   0 root         (0) root         (0)    14290 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/iv/gmm.py
+-rw-r--r--   0 root         (0) root         (0)    54577 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/iv/model.py
+-rw-r--r--   0 root         (0) root         (0)    58789 2024-01-04 11:19:21.000000 linearmodels-5.4/linearmodels/iv/results.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-05 08:39:12.117550 linearmodels-5.4/linearmodels/panel/
+-rw-r--r--   0 root         (0) root         (0)      391 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/panel/__init__.py
+-rw-r--r--   0 root         (0) root         (0)  1314932 2024-01-05 08:39:11.000000 linearmodels-5.4/linearmodels/panel/_utility.c
+-rw-r--r--   0 root         (0) root         (0)      114 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/panel/_utility.pxi
+-rw-r--r--   0 root         (0) root         (0)     2698 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/panel/_utility.pyx
+-rw-r--r--   0 root         (0) root         (0)    24104 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/panel/covariance.py
+-rw-r--r--   0 root         (0) root         (0)    24934 2024-01-04 11:19:21.000000 linearmodels-5.4/linearmodels/panel/data.py
+-rw-r--r--   0 root         (0) root         (0)   114101 2024-01-05 08:38:51.000000 linearmodels-5.4/linearmodels/panel/model.py
+-rw-r--r--   0 root         (0) root         (0)    37469 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/panel/results.py
+-rw-r--r--   0 root         (0) root         (0)    20082 2024-01-04 11:19:21.000000 linearmodels-5.4/linearmodels/panel/utility.py
+-rw-r--r--   0 root         (0) root         (0)       72 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-05 08:39:12.117550 linearmodels-5.4/linearmodels/shared/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/shared/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3945 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/shared/base.py
+-rw-r--r--   0 root         (0) root         (0)     2873 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/shared/covariance.py
+-rw-r--r--   0 root         (0) root         (0)     1020 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/shared/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     6922 2024-01-04 11:19:21.000000 linearmodels-5.4/linearmodels/shared/hypotheses.py
+-rw-r--r--   0 root         (0) root         (0)     3127 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/shared/io.py
+-rw-r--r--   0 root         (0) root         (0)     1693 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/shared/linalg.py
+-rw-r--r--   0 root         (0) root         (0)     4441 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/shared/typed_getters.py
+-rw-r--r--   0 root         (0) root         (0)     7736 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/shared/utility.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-05 08:39:12.117550 linearmodels-5.4/linearmodels/system/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/system/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9568 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/system/_utility.py
+-rw-r--r--   0 root         (0) root         (0)    24392 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/system/covariance.py
+-rw-r--r--   0 root         (0) root         (0)    11324 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/system/gmm.py
+-rw-r--r--   0 root         (0) root         (0)    76106 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/system/model.py
+-rw-r--r--   0 root         (0) root         (0)    27787 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/system/results.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-05 08:39:12.117550 linearmodels-5.4/linearmodels/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-05 08:39:12.117550 linearmodels-5.4/linearmodels/tests/asset_pricing/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/tests/asset_pricing/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1394 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/tests/asset_pricing/_utility.py
+-rw-r--r--   0 root         (0) root         (0)     1892 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/tests/asset_pricing/test_covariance.py
+-rw-r--r--   0 root         (0) root         (0)     5065 2024-01-02 12:10:00.000000 linearmodels-5.4/linearmodels/tests/asset_pricing/test_formulas.py
+-rw-r--r--   0 root         (0) root         (0)     3356 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/tests/asset_pricing/test_linear_factor_gmm.py
+-rw-r--r--   0 root         (0) root         (0)    12283 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/tests/asset_pricing/test_linear_factor_model.py
+-rw-r--r--   0 root         (0) root         (0)     7358 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/tests/asset_pricing/test_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-05 08:39:12.117550 linearmodels-5.4/linearmodels/tests/datasets/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/tests/datasets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      636 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/tests/datasets/test_datasets.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-05 08:39:12.127550 linearmodels-5.4/linearmodels/tests/iv/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/tests/iv/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1442 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/tests/iv/_utility.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-05 08:39:12.127550 linearmodels-5.4/linearmodels/tests/iv/results/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/tests/iv/results/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4154 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/tests/iv/results/execute-stata-simulated-data.py
+-rw-r--r--   0 root         (0) root         (0)     2583 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/tests/iv/results/execute-stata.py
+-rw-r--r--   0 root         (0) root         (0)     5777 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/tests/iv/results/housing.csv
+-rw-r--r--   0 root         (0) root         (0)     3465 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/tests/iv/results/read_stata_results.py
+-rw-r--r--   0 root         (0) root         (0)    97696 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/tests/iv/results/simulated-data.dta
+-rw-r--r--   0 root         (0) root         (0)     2332 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/tests/iv/results/simulated-test-data.py
+-rw-r--r--   0 root         (0) root         (0)    13232 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/tests/iv/results/stata-iv-housing-results.txt
+-rw-r--r--   0 root         (0) root         (0)   547258 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/tests/iv/results/stata-iv-simulated-results.txt
+-rw-r--r--   0 root         (0) root         (0)    24433 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/tests/iv/test_absorbing.py
+-rw-r--r--   0 root         (0) root         (0)     7460 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/tests/iv/test_against_stata.py
+-rw-r--r--   0 root         (0) root         (0)    10791 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/tests/iv/test_covariance.py
+-rw-r--r--   0 root         (0) root         (0)     8041 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/tests/iv/test_data.py
+-rw-r--r--   0 root         (0) root         (0)    11585 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/tests/iv/test_formulas.py
+-rw-r--r--   0 root         (0) root         (0)     9641 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/tests/iv/test_gmm.py
+-rw-r--r--   0 root         (0) root         (0)     2797 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/tests/iv/test_missing_data.py
+-rw-r--r--   0 root         (0) root         (0)    15202 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/tests/iv/test_model.py
+-rw-r--r--   0 root         (0) root         (0)     5577 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/tests/iv/test_postestimation.py
+-rw-r--r--   0 root         (0) root         (0)     3293 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/tests/iv/test_results.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-05 08:39:12.127550 linearmodels-5.4/linearmodels/tests/panel/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/tests/panel/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8085 2024-01-04 11:19:21.000000 linearmodels-5.4/linearmodels/tests/panel/_utility.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-05 08:39:12.127550 linearmodels-5.4/linearmodels/tests/panel/results/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/tests/panel/results/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3374 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/tests/panel/results/execute-stata-simulated-data.py
+-rw-r--r--   0 root         (0) root         (0)     1923 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/tests/panel/results/generate-panel-data.py
+-rw-r--r--   0 root         (0) root         (0)     1994 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/tests/panel/results/parse_stata_results.py
+-rw-r--r--   0 root         (0) root         (0)   578091 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/tests/panel/results/simulated-panel.dta
+-rw-r--r--   0 root         (0) root         (0)    65624 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/tests/panel/results/stata-panel-simulated-results.txt
+-rw-r--r--   0 root         (0) root         (0)    11968 2023-09-08 09:53:46.000000 linearmodels-5.4/linearmodels/tests/panel/test_between_ols.py
+-rw-r--r--   0 root         (0) root         (0)     4972 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/tests/panel/test_cluster_input_formats.py
+-rw-r--r--   0 root         (0) root         (0)    27934 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/tests/panel/test_data.py
+-rw-r--r--   0 root         (0) root         (0)     5941 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/tests/panel/test_fama_macbeth.py
+-rw-r--r--   0 root         (0) root         (0)     7010 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/tests/panel/test_firstdifference_ols.py
+-rw-r--r--   0 root         (0) root         (0)    10720 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/tests/panel/test_formula.py
+-rw-r--r--   0 root         (0) root         (0)     7966 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/tests/panel/test_model.py
+-rw-r--r--   0 root         (0) root         (0)     7696 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/tests/panel/test_panel_covariance.py
+-rw-r--r--   0 root         (0) root         (0)    51469 2023-09-08 09:53:46.000000 linearmodels-5.4/linearmodels/tests/panel/test_panel_ols.py
+-rw-r--r--   0 root         (0) root         (0)     7953 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/tests/panel/test_pooled_ols.py
+-rw-r--r--   0 root         (0) root         (0)     2738 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/tests/panel/test_random_effects.py
+-rw-r--r--   0 root         (0) root         (0)     8478 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/tests/panel/test_results.py
+-rw-r--r--   0 root         (0) root         (0)     4978 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/tests/panel/test_simulated_against_stata.py
+-rw-r--r--   0 root         (0) root         (0)     9039 2023-09-08 09:53:46.000000 linearmodels-5.4/linearmodels/tests/panel/test_utility.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-05 08:39:12.127550 linearmodels-5.4/linearmodels/tests/shared/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/tests/shared/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      193 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/tests/shared/test_base.py
+-rw-r--r--   0 root         (0) root         (0)     2561 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/tests/shared/test_typed_getters.py
+-rw-r--r--   0 root         (0) root         (0)     7124 2024-01-04 11:19:21.000000 linearmodels-5.4/linearmodels/tests/shared/test_utility.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-05 08:39:12.127550 linearmodels-5.4/linearmodels/tests/system/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/tests/system/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12361 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/tests/system/_utility.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-05 08:39:12.127550 linearmodels-5.4/linearmodels/tests/system/results/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/tests/system/results/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2679 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/tests/system/results/execute-stata-3sls.py
+-rw-r--r--   0 root         (0) root         (0)     3587 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/tests/system/results/execute-stata.py
+-rw-r--r--   0 root         (0) root         (0)     1565 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/tests/system/results/generate_data.py
+-rw-r--r--   0 root         (0) root         (0)     2682 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/tests/system/results/parse_stata_3sls_results.py
+-rw-r--r--   0 root         (0) root         (0)     3357 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/tests/system/results/parse_stata_results.py
+-rw-r--r--   0 root         (0) root         (0)    50504 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/tests/system/results/simulated-3sls.dta
+-rw-r--r--   0 root         (0) root         (0)    55085 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/tests/system/results/simulated-sur.dta
+-rw-r--r--   0 root         (0) root         (0)    85208 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/tests/system/results/stata-3sls-results.txt
+-rw-r--r--   0 root         (0) root         (0)    32162 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/tests/system/results/stata-sur-results.txt
+-rw-r--r--   0 root         (0) root         (0)    12026 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/tests/system/test_3sls.py
+-rw-r--r--   0 root         (0) root         (0)     2518 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/tests/system/test_3sls_against_stata.py
+-rw-r--r--   0 root         (0) root         (0)    12405 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/tests/system/test_covariance.py
+-rw-r--r--   0 root         (0) root         (0)     1619 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/tests/system/test_equivalence.py
+-rw-r--r--   0 root         (0) root         (0)     6999 2024-01-02 12:10:00.000000 linearmodels-5.4/linearmodels/tests/system/test_formulas.py
+-rw-r--r--   0 root         (0) root         (0)    13455 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/tests/system/test_gmm.py
+-rw-r--r--   0 root         (0) root         (0)    28960 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/tests/system/test_sur.py
+-rw-r--r--   0 root         (0) root         (0)     5194 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/tests/system/test_sur_against_stata.py
+-rw-r--r--   0 root         (0) root         (0)     6165 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/tests/system/test_utility.py
+-rw-r--r--   0 root         (0) root         (0)     2091 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/tests/test_examples.py
+-rw-r--r--   0 root         (0) root         (0)      710 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/tests/test_tester.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-05 08:39:12.127550 linearmodels-5.4/linearmodels/typing/
+-rw-r--r--   0 root         (0) root         (0)     1617 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/typing/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1344 2023-05-26 11:28:32.000000 linearmodels-5.4/linearmodels/typing/data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-05 08:39:12.127550 linearmodels-5.4/linearmodels.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7932 2024-01-05 08:39:11.000000 linearmodels-5.4/linearmodels.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    16318 2024-01-05 08:39:11.000000 linearmodels-5.4/linearmodels.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-01-05 08:39:11.000000 linearmodels-5.4/linearmodels.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-01-05 08:39:10.000000 linearmodels-5.4/linearmodels.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      162 2024-01-05 08:39:11.000000 linearmodels-5.4/linearmodels.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2024-01-05 08:39:11.000000 linearmodels-5.4/linearmodels.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      583 2024-01-04 11:19:21.000000 linearmodels-5.4/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      261 2024-01-02 12:10:00.000000 linearmodels-5.4/requirements-dev.txt
+-rw-r--r--   0 root         (0) root         (0)      131 2024-01-04 11:19:21.000000 linearmodels-5.4/requirements-test.txt
+-rw-r--r--   0 root         (0) root         (0)      176 2024-01-05 08:38:51.000000 linearmodels-5.4/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)     2143 2024-01-05 08:39:12.137550 linearmodels-5.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     5285 2024-01-02 12:10:00.000000 linearmodels-5.4/setup.py
```

### Comparing `linearmodels-5.3/.coveragerc` & `linearmodels-5.4/.coveragerc`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/.github/workflows/codeql.yml` & `linearmodels-5.4/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/.github/workflows/cron-test.yml` & `linearmodels-5.4/.github/workflows/cron-test.yml`

 * *Files 9% similar despite different names*

```diff
@@ -14,22 +14,23 @@
     runs-on: ${{ matrix.os }}
     defaults:
       run:
         shell: bash
     strategy:
       fail-fast: false
       matrix:
-        python: [cp310]
-        os: [ubuntu-20.04, windows-2019]
+        python: [cp311]
+        os: [ubuntu-latest, windows-latest]
     env:
       BUILD_COMMIT: "main"
       CIBW_BUILD: ${{ matrix.python }}-*
       CIBW_ARCHS_LINUX: "x86_64"
       CIBW_ARCHS_MACOS: "x86_64"
       CIBW_SKIP: "pp* *-musllinux_* *-win32"
+      CIBW_BEFORE_BUILD: python -m pip install wheel>=0.41.0 pip --upgrade
       CIBW_TEST_REQUIRES: pytest pytest-xdist xarray matplotlib
       CIBW_TEST_COMMAND: python -c "import linearmodels; linearmodels.test(['--skip-examples','--skip-slow','-n','2'])"
       # Avoid testing on emulated architectures
       CIBW_REPAIR_WHEEL_COMMAND_LINUX: 'auditwheel repair --strip -w {dest_dir} {wheel}'
       MKL_NUM_THREADS: 1
       OMP_NUM_THREADS: 1
       OPENLAS_NUM_THREADS: 1
@@ -41,11 +42,11 @@
           fetch-depth: 0
 
       - uses: actions/setup-python@v4
         with:
           python-version: '3.x'
 
       - name: Install cibuildwheel
-        run: python -m pip install cibuildwheel==2.12.2
+        run: python -m pip install cibuildwheel==2.16.2
 
       - name: Build wheels
         run: python -m cibuildwheel --output-dir wheelhouse .
```

### Comparing `linearmodels-5.3/.github/workflows/generate-documentation.yml` & `linearmodels-5.4/.github/workflows/generate-documentation.yml`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/.gitignore` & `linearmodels-5.4/.gitignore`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/LICENSE.md` & `linearmodels-5.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/PKG-INFO` & `linearmodels-5.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linearmodels
-Version: 5.3
+Version: 5.4
 Summary: Linear Panel, Instrumental Variable, Asset Pricing, and System Regression models for Python
 Home-page: http://github.com/bashtage/linearmodels
 Author: Kevin Sheppard
 Author-email: kevin.k.sheppard@gmail.com
 License: NCSA
 Keywords: linear models,regression,instrumental variables,IV,panel,fixed effects,clustered,heteroskedasticity,endogeneity,instruments,statistics,statistical inference,econometrics
 Classifier: Development Status :: 5 - Production/Stable
@@ -20,31 +20,30 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
-Requires-Dist: numpy>=1.19.0
-Requires-Dist: pandas>=1.1.0
+Requires-Dist: numpy>=1.22.0
+Requires-Dist: pandas>=1.3.0
 Requires-Dist: scipy>=1.5.0
 Requires-Dist: statsmodels>=0.12.0
 Requires-Dist: mypy_extensions>=0.4
-Requires-Dist: Cython>=0.29.34
+Requires-Dist: Cython>=0.29.37
 Requires-Dist: pyhdfe>=0.1
 Requires-Dist: formulaic>=0.6.5
-Requires-Dist: setuptools_scm[toml]<8.0.0,>=7.0.0
+Requires-Dist: setuptools_scm[toml]<9.0.0,>=8.0.0
 
 # Linear Models
 
 | Metric                     |                                                                                                                                                                                                                                                          |
 | :------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
 | **Latest Release**         | [![PyPI version](https://badge.fury.io/py/linearmodels.svg)](https://badge.fury.io/py/linearmodels)                                                                                                                                                      |
 | **Continuous Integration** | [![Build Status](https://dev.azure.com/kevinksheppard/kevinksheppard/_apis/build/status/bashtage.linearmodels?branchName=main)](https://dev.azure.com/kevinksheppard/kevinksheppard/_build/latest?definitionId=2&branchName=main)                        |
-|                            | [![Build status](https://ci.appveyor.com/api/projects/status/7768doy6wrdunmdt/branch/main?svg=true)](https://ci.appveyor.com/project/bashtage/linearmodels/branch/main)                                                                                  |
 | **Coverage**               | [![codecov](https://codecov.io/gh/bashtage/linearmodels/branch/main/graph/badge.svg)](https://codecov.io/gh/bashtage/linearmodels)                                                                                                                       |
 | **Code Quality**           | [![Codacy Badge](https://api.codacy.com/project/badge/Grade/745a24a69cb2466b95df6a53c83892de)](https://www.codacy.com/manual/bashtage/linearmodels?utm_source=github.com&utm_medium=referral&utm_content=bashtage/linearmodels&utm_campaign=Badge_Grade) |
 |                            | [![codebeat badge](https://codebeat.co/badges/aaae2fb4-72b5-4a66-97cd-77b93488f243)](https://codebeat.co/projects/github-com-bashtage-linearmodels-main)                                                                                                 |
 | **Citation**               | [![DOI](https://zenodo.org/badge/82291672.svg)](https://zenodo.org/badge/latestdoi/82291672)                                                                                                                                                             |
 
 Linear (regression) models for Python. Extends
 [statsmodels](http://www.statsmodels.org) with Panel regression,
@@ -165,20 +164,22 @@
 -   Dynamic Panel model estimation - _not started_
 
 ## Requirements
 
 ### Running
 
 -   Python 3.9+
--   NumPy (1.19+)
+-   NumPy (1.22+)
 -   SciPy (1.5+)
--   pandas (1.1+)
+-   pandas (1.3+)
 -   statsmodels (0.12+)
+-   formulaic (0.6.5+)
 -   xarray (0.16+, optional)
--   Cython (0.29.34+, optional)
+-   Cython (0.29.37+, optional)
+
 
 ### Testing
 
 -   py.test
 
 ### Documentation
```

### Comparing `linearmodels-5.3/README.md` & `linearmodels-5.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Linear Models
 
 | Metric                     |                                                                                                                                                                                                                                                          |
 | :------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
 | **Latest Release**         | [![PyPI version](https://badge.fury.io/py/linearmodels.svg)](https://badge.fury.io/py/linearmodels)                                                                                                                                                      |
 | **Continuous Integration** | [![Build Status](https://dev.azure.com/kevinksheppard/kevinksheppard/_apis/build/status/bashtage.linearmodels?branchName=main)](https://dev.azure.com/kevinksheppard/kevinksheppard/_build/latest?definitionId=2&branchName=main)                        |
-|                            | [![Build status](https://ci.appveyor.com/api/projects/status/7768doy6wrdunmdt/branch/main?svg=true)](https://ci.appveyor.com/project/bashtage/linearmodels/branch/main)                                                                                  |
 | **Coverage**               | [![codecov](https://codecov.io/gh/bashtage/linearmodels/branch/main/graph/badge.svg)](https://codecov.io/gh/bashtage/linearmodels)                                                                                                                       |
 | **Code Quality**           | [![Codacy Badge](https://api.codacy.com/project/badge/Grade/745a24a69cb2466b95df6a53c83892de)](https://www.codacy.com/manual/bashtage/linearmodels?utm_source=github.com&utm_medium=referral&utm_content=bashtage/linearmodels&utm_campaign=Badge_Grade) |
 |                            | [![codebeat badge](https://codebeat.co/badges/aaae2fb4-72b5-4a66-97cd-77b93488f243)](https://codebeat.co/projects/github-com-bashtage-linearmodels-main)                                                                                                 |
 | **Citation**               | [![DOI](https://zenodo.org/badge/82291672.svg)](https://zenodo.org/badge/latestdoi/82291672)                                                                                                                                                             |
 
 Linear (regression) models for Python. Extends
 [statsmodels](http://www.statsmodels.org) with Panel regression,
@@ -129,20 +128,22 @@
 -   Dynamic Panel model estimation - _not started_
 
 ## Requirements
 
 ### Running
 
 -   Python 3.9+
--   NumPy (1.19+)
+-   NumPy (1.22+)
 -   SciPy (1.5+)
--   pandas (1.1+)
+-   pandas (1.3+)
 -   statsmodels (0.12+)
+-   formulaic (0.6.5+)
 -   xarray (0.16+, optional)
--   Cython (0.29.34+, optional)
+-   Cython (0.29.37+, optional)
+
 
 ### Testing
 
 -   py.test
 
 ### Documentation
```

### Comparing `linearmodels-5.3/azure-pipelines.yml` & `linearmodels-5.4/azure-pipelines.yml`

 * *Files 6% similar despite different names*

```diff
@@ -6,18 +6,19 @@
 variables:
   MKL_NUM_THREADS: 1
   NUMEXPR_NUM_THREADS: 1
   OMP_NUM_THREADS: 1
   VML_NUM_THREADS: 1
   OPENBLAS_NUM_THREADS: 1
   PYTHONHASHSEED: 12345678 # Ensure tests are correctly gathered by xdist
-  SETUPTOOLS_USE_DISTUTILS: "stdlib"
   TEST_INSTALL: false
   MPLBACKEND: agg
   coverage: true
+  test.install: false
+  pip.pre: false
 
 jobs:
 - template: ci/azure_template_posix.yml
   parameters:
     name: Linux
     vmImage: ubuntu-20.04
```

### Comparing `linearmodels-5.3/ci/azure_template_posix.yml` & `linearmodels-5.4/ci/azure_template_posix.yml`

 * *Files 12% similar despite different names*

```diff
@@ -12,62 +12,69 @@
 jobs:
 
 - job: ${{ parameters.name }}Test
   pool:
     vmImage: ${{ parameters.vmImage }}
   strategy:
     matrix:
-      python39_legacy:
+      python39_minimums:
         python.version: '3.9'
-        NUMPY: 1.19.0
+        NUMPY: 1.22.0
         SCIPY: 1.5.0
-        PANDAS: 1.1.0
+        PANDAS: 1.3.0
         STATSMODELS: 0.12.0
-        XARRAY: 0.16.0
+        XARRAY: 0.21.0
         FORMULAIC: 0.6.5
         test.install: true
       python39_mid:
         python.version: '3.9'
-        NUMPY: 1.20.0
+        NUMPY: 1.23.0
         SCIPY: 1.6.0
-        PANDAS: 1.2.0
-        STATSMODELS: 0.12.0
-        XARRAY: 0.18.0
+        PANDAS: 1.4.0
+        STATSMODELS: 0.13.0
+        XARRAY: 2022.6.0
         XXHASH: true
         FORMULAIC: 0.6.5
         test.install: true
       python39_recent:
         python.version: '3.9'
-        NUMPY: 1.21.0
+        NUMPY: 1.24.0
         SCIPY: 1.7.0
-        PANDAS: 1.3.0
+        PANDAS: 1.5.0
         STATSMODELS: 0.13.0
-        XARRAY: 0.20.0
+        XARRAY: 2022.12.0
         FORMULAIC: 0.6.5
         test.install: true
       python310_no_cython:
         python.version: '3.10'
         LM_NO_BINARY: 1
       python310_recent:
         python.version: '3.10'
-        NUMPY: 1.22.0
-        SCIPY: 1.8.0
-        PANDAS: 1.5.0
-        STATSMODELS: 0.13.0
-        XARRAY: 22.0
+        NUMPY: 1.24.0
+        SCIPY: 1.9.0
+        PANDAS: 2.0.0
+        STATSMODELS: 0.14.0
+        XARRAY: 2023.4.0
       python310_latest:
         python.version: '3.10'
+        FORMULAIC: 1.0.1
         XXHASH: true
       python311_latest:
         python.version: '3.11'
         XXHASH: true
-      python311_copy_on_write:
-        python.version: '3.11'
+      python312_latest:
+        python.version: '3.12'
+        XXHASH: true
+      python312_copy_on_write:
+        python.version: '3.12'
         XXHASH: true
         LM_TEST_COPY_ON_WRITE: 1
+      python312_pre:
+        python.version: '3.12'
+        pip.pre: true
     maxParallel: 10
 
   steps:
   - task: UsePythonVersion@0
     inputs:
       versionSpec: '$(python.version)'
       architecture: 'x64'
@@ -109,25 +116,36 @@
   - script: |
       echo "Testing site packages"
       mkdir test_run_dir
       pushd test_run_dir
       python -c "import linearmodels; linearmodels.test(['-n', 'auto', '--junitxml=../junit/test-results.xml'])"
       popd
     displayName: 'Run tests (site-packages)'
-    condition: eq(variables['test.install'], 'true')
+    condition: and(eq(variables['test.install'], 'true'), ne(variables['pip.pre'], 'true'))
 
   - script: |
       echo "Testing editable install"
       if [[ ${COVERAGE} == "true" ]]; then
         export COVERAGE_OPTS="--cov-config .coveragerc --cov=linearmodels --cov-report xml:coverage.xml --cov-report term"
       fi
       echo pytest -m "${PYTEST_PATTERN}" --junitxml=junit/test-results.xml -n auto --durations=25 ${COVERAGE_OPTS} linearmodels/tests
       pytest -m "${PYTEST_PATTERN}" --junitxml=junit/test-results.xml -n auto --durations=25 ${COVERAGE_OPTS} linearmodels/tests
     displayName: 'Run tests (editable)'
-    condition: ne(variables['test.install'], 'true')
+    condition: and(ne(variables['test.install'], 'true'), ne(variables['pip.pre'], 'true'))
+
+  - script: |
+      echo "Testing pip-pre"
+      if [[ ${COVERAGE} == "true" ]]; then
+        export COVERAGE_OPTS="--cov-config .coveragerc --cov=linearmodels --cov-report xml:coverage.xml --cov-report term"
+      fi
+      echo pytest -m "${PYTEST_PATTERN}" --junitxml=junit/test-results.xml -n auto --durations=25 ${COVERAGE_OPTS} linearmodels/tests
+      pytest -m "${PYTEST_PATTERN}" --junitxml=junit/test-results.xml -n auto --durations=25 ${COVERAGE_OPTS} linearmodels/tests
+    displayName: 'Run tests (pip pre)'
+    condition: eq(variables['pip.pre'], 'true')
+    continueOnError: true
 
   - task: PublishTestResults@2
     inputs:
       testResultsFiles: '**/test-results.xml'
       testRunTitle: 'Python $(python.version)'
     condition: succeededOrFailed()
```

### Comparing `linearmodels-5.3/ci/azure_template_windows.yml` & `linearmodels-5.4/ci/azure_template_windows.yml`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/ci/install-posix.sh` & `linearmodels-5.4/ci/install-posix.sh`

 * *Files 22% similar despite different names*

```diff
@@ -9,7 +9,13 @@
 CMD="$CMD statsmodels"
 if [[ -n ${STATSMODELS} ]]; then CMD="$CMD~=${STATSMODELS}"; fi
 if [[ -n ${XARRAY} ]]; then CMD="$CMD xarray~=${XARRAY}"; fi
 if [[ -n ${FORMULAIC} ]]; then CMD="$CMD formulaic~=${FORMULAIC}"; fi
 if [[ -n ${XXHASH} ]]; then CMD="$CMD xxhash"; fi
 echo "$CMD"
 eval "$CMD"
+
+if [ "${PIP_PRE}" = true ]; then
+  python -m pip uninstall -y numpy pandas scipy matplotlib statsmodels
+  python -m pip install -i https://pypi.anaconda.org/scientific-python-nightly-wheels/simple numpy pandas scipy matplotlib --upgrade --use-deprecated=legacy-resolver
+  python -m pip install git+https://github.com/statsmodels/statsmodels.git --upgrade --no-build-isolation -v
+fi
```

### Comparing `linearmodels-5.3/ci/push-docs-gh-pages.sh` & `linearmodels-5.4/ci/push-docs-gh-pages.sh`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/doc/Makefile` & `linearmodels-5.4/doc/Makefile`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/doc/make.bat` & `linearmodels-5.4/doc/make.bat`

 * *Files 14% similar despite different names*

```diff
@@ -7,31 +7,35 @@
 if "%SPHINXBUILD%" == "" (
 	set SPHINXBUILD=sphinx-build
 )
 set SOURCEDIR=source
 set BUILDDIR=build
 set SPHINXPROJ=linearmodels
 set SPHINXOPTS=
+set PYDEVD_DISABLE_FILE_VALIDATION=1
 
 if "%1" == "" goto help
 
 %SPHINXBUILD% >NUL 2>NUL
 if errorlevel 9009 (
 	echo.
 	echo.The 'sphinx-build' command was not found. Make sure you have Sphinx
 	echo.installed, then set the SPHINXBUILD environment variable to point
 	echo.to the full path of the 'sphinx-build' executable. Alternatively you
 	echo.may add the Sphinx directory to PATH.
 	echo.
 	echo.If you don't have Sphinx installed, grab it from
-	echo.http://sphinx-doc.org/
+	echo.https://sphinx-doc.org/
+	set PYDEVD_DISABLE_FILE_VALIDATION=
 	exit /b 1
 )
 
 %SPHINXBUILD% -M %1 %SOURCEDIR% %BUILDDIR% %SPHINXOPTS%
+set PYDEVD_DISABLE_FILE_VALIDATION=
 goto end
 
 :help
 %SPHINXBUILD% -M help %SOURCEDIR% %BUILDDIR% %SPHINXOPTS%
+set PYDEVD_DISABLE_FILE_VALIDATION=
 
 :end
 popd
```

### Comparing `linearmodels-5.3/doc/source/_static/css/small_fixes.css` & `linearmodels-5.4/doc/source/_static/css/small_fixes.css`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/doc/source/_static/icons/android-chrome-192x192.png` & `linearmodels-5.4/doc/source/_static/icons/android-chrome-192x192.png`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/doc/source/_static/icons/android-chrome-512x512.png` & `linearmodels-5.4/doc/source/_static/icons/android-chrome-512x512.png`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/doc/source/_static/icons/apple-touch-icon.png` & `linearmodels-5.4/doc/source/_static/icons/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/doc/source/_static/icons/favicon-16x16.png` & `linearmodels-5.4/doc/source/_static/icons/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/doc/source/_static/icons/favicon-32x32.png` & `linearmodels-5.4/doc/source/_static/icons/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/doc/source/_static/icons/favicon.ico` & `linearmodels-5.4/doc/source/_static/icons/favicon.ico`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/doc/source/_static/icons/mstile-144x144.png` & `linearmodels-5.4/doc/source/_static/icons/mstile-144x144.png`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/doc/source/_static/icons/mstile-150x150.png` & `linearmodels-5.4/doc/source/_static/icons/mstile-150x150.png`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/doc/source/_static/icons/mstile-310x150.png` & `linearmodels-5.4/doc/source/_static/icons/mstile-310x150.png`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/doc/source/_static/icons/mstile-310x310.png` & `linearmodels-5.4/doc/source/_static/icons/mstile-310x310.png`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/doc/source/_static/icons/mstile-70x70.png` & `linearmodels-5.4/doc/source/_static/icons/mstile-70x70.png`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/doc/source/_static/icons/safari-pinned-tab.svg` & `linearmodels-5.4/doc/source/_static/icons/safari-pinned-tab.svg`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/doc/source/_templates/autosummary/class.rst` & `linearmodels-5.4/doc/source/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/doc/source/_templates/layout.html` & `linearmodels-5.4/doc/source/_templates/layout.html`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/doc/source/asset-pricing/index.rst` & `linearmodels-5.4/doc/source/asset-pricing/index.rst`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/doc/source/asset-pricing/introduction.rst` & `linearmodels-5.4/doc/source/asset-pricing/introduction.rst`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/doc/source/asset-pricing/mathematical-detail.lyx` & `linearmodels-5.4/doc/source/asset-pricing/mathematical-detail.lyx`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/doc/source/asset-pricing/mathematical-detail.txt` & `linearmodels-5.4/doc/source/asset-pricing/mathematical-detail.txt`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/doc/source/asset-pricing/reference.rst` & `linearmodels-5.4/doc/source/asset-pricing/reference.rst`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/doc/source/changes/3.0-2.0-1.0.rst` & `linearmodels-5.4/doc/source/changes/3.0-2.0-1.0.rst`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/doc/source/changes/4.0.rst` & `linearmodels-5.4/doc/source/changes/4.0.rst`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/doc/source/changes/5.0.rst` & `linearmodels-5.4/doc/source/changes/5.0.rst`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+Verison 5.4
+----------
+- Compatibility with NumPy 2
+- Compatibility with recent pandas releases
+
 Version 5.3
 -----------
 - Bumped the minimum formulaic to 0.6.5.
 - Released wheels for Python 3.12.
 
 Version 5.2
 -----------
```

### Comparing `linearmodels-5.3/doc/source/conf.py` & `linearmodels-5.4/doc/source/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,15 +117,15 @@
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
 language = "en"
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This pattern also affects html_static_path and html_extra_path.
-# exclude_patterns: list[str] = []
+exclude_patterns: list[str] = []
 
 # The name of the Pygments (syntax highlighting) style to use.
 pygments_style = "colorful"
 
 # If true, `todo` and `todoList` produce output, else they produce nothing.
 todo_include_todos = True
```

### Comparing `linearmodels-5.3/doc/source/contributing.rst` & `linearmodels-5.4/doc/source/contributing.rst`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/doc/source/images/bw-logo.svg` & `linearmodels-5.4/doc/source/images/bw-logo.svg`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/doc/source/images/favicon.ico` & `linearmodels-5.4/doc/source/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/doc/source/images/logo-text.svg` & `linearmodels-5.4/doc/source/images/logo-text.svg`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/doc/source/images/logo.svg` & `linearmodels-5.4/doc/source/images/logo.svg`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/doc/source/index.rst` & `linearmodels-5.4/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/doc/source/iv/estimators.lyx` & `linearmodels-5.4/doc/source/iv/estimators.lyx`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/doc/source/iv/estimators.txt` & `linearmodels-5.4/doc/source/iv/estimators.txt`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/doc/source/iv/index.rst` & `linearmodels-5.4/doc/source/iv/index.rst`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/doc/source/iv/introduction.rst` & `linearmodels-5.4/doc/source/iv/introduction.rst`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/doc/source/iv/reference.rst` & `linearmodels-5.4/doc/source/iv/reference.rst`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/doc/source/panel/faq.rst` & `linearmodels-5.4/doc/source/panel/faq.rst`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/doc/source/panel/index.rst` & `linearmodels-5.4/doc/source/panel/index.rst`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/doc/source/panel/introduction.rst` & `linearmodels-5.4/doc/source/panel/introduction.rst`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/doc/source/panel/mathematical-detail.lyx` & `linearmodels-5.4/doc/source/panel/mathematical-detail.lyx`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/doc/source/panel/mathematical-detail.txt` & `linearmodels-5.4/doc/source/panel/mathematical-detail.txt`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/doc/source/panel/pandas.rst` & `linearmodels-5.4/doc/source/panel/pandas.rst`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/doc/source/panel/reference.rst` & `linearmodels-5.4/doc/source/panel/reference.rst`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/doc/source/plan.rst` & `linearmodels-5.4/doc/source/plan.rst`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/doc/source/references.rst` & `linearmodels-5.4/doc/source/references.rst`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/doc/source/spelling_wordlist.txt` & `linearmodels-5.4/doc/source/spelling_wordlist.txt`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/doc/source/system/index.rst` & `linearmodels-5.4/doc/source/system/index.rst`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/doc/source/system/mathematical-detail.lyx` & `linearmodels-5.4/doc/source/system/mathematical-detail.lyx`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/doc/source/system/mathematical-detail.txt` & `linearmodels-5.4/doc/source/system/mathematical-detail.txt`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/doc/source/system/reference.rst` & `linearmodels-5.4/doc/source/system/reference.rst`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/doc/source/utility.rst` & `linearmodels-5.4/doc/source/utility.rst`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/examples/asset-pricing_examples.ipynb` & `linearmodels-5.4/examples/asset-pricing_examples.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9981740669240668%*

 * *Differences: {"'cells'": "{5: {'metadata': {replace: OrderedDict()}}}",*

 * * "'metadata'": "{'language_info': {'version': '3.12.0'}}"}*

```diff
@@ -47,20 +47,15 @@
                 "\n",
                 "Subtract the risk-free rate from the test portfolios since these are not zero-investment."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "metadata": {
-                "collapsed": true,
-                "jupyter": {
-                    "outputs_hidden": true
-                }
-            },
+            "metadata": {},
             "outputs": [],
             "source": [
                 "data.iloc[:, 6:] = data.iloc[:, 6:].values - data[[\"RF\"]].values"
             ]
         },
         {
             "cell_type": "markdown",
@@ -413,15 +408,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.11"
+            "version": "3.12.0"
         },
         "pycharm": {
             "stem_cell": {
                 "cell_type": "raw",
                 "metadata": {
                     "collapsed": false
                 },
```

### Comparing `linearmodels-5.3/examples/asset-pricing_formulas.ipynb` & `linearmodels-5.4/examples/asset-pricing_formulas.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9985119047619048%*

 * *Differences: {"'metadata'": "{'language_info': {'version': '3.12.0'}}"}*

```diff
@@ -135,15 +135,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.11"
+            "version": "3.12.0"
         },
         "pycharm": {
             "stem_cell": {
                 "cell_type": "raw",
                 "metadata": {
                     "collapsed": false
                 },
```

### Comparing `linearmodels-5.3/examples/iv_absorbing-regression.ipynb` & `linearmodels-5.4/examples/iv_absorbing-regression.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9985119047619048%*

 * *Differences: {"'metadata'": "{'language_info': {'version': '3.12.0'}}"}*

```diff
@@ -147,15 +147,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.11"
+            "version": "3.12.0"
         },
         "pycharm": {
             "stem_cell": {
                 "cell_type": "raw",
                 "metadata": {
                     "collapsed": false
                 },
```

### Comparing `linearmodels-5.3/examples/iv_advanced-examples.ipynb` & `linearmodels-5.4/examples/iv_advanced-examples.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9988839285714286%*

 * *Differences: {"'metadata'": "{'language_info': {'version': '3.12.0'}}"}*

```diff
@@ -568,15 +568,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.11"
+            "version": "3.12.0"
         },
         "nbsphinx": {
             "allow_errors": true
         },
         "pycharm": {
             "stem_cell": {
                 "cell_type": "raw",
```

### Comparing `linearmodels-5.3/examples/iv_basic-examples.ipynb` & `linearmodels-5.4/examples/iv_basic-examples.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9985119047619048%*

 * *Differences: {"'metadata'": "{'language_info': {'version': '3.12.0'}}"}*

```diff
@@ -798,15 +798,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.11"
+            "version": "3.12.0"
         },
         "pycharm": {
             "stem_cell": {
                 "cell_type": "raw",
                 "metadata": {
                     "collapsed": false
                 },
```

### Comparing `linearmodels-5.3/examples/iv_using-formulas.ipynb` & `linearmodels-5.4/examples/iv_using-formulas.ipynb`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.992742673992674%*

 * *Differences: {"'cells'": "{3: {'metadata': {replace: OrderedDict()}}, 5: {'metadata': {replace: "*

 * *            "OrderedDict()}}, 6: {'metadata': {replace: OrderedDict()}}, 8: {'metadata': {replace: "*

 * *            "OrderedDict()}}, 10: {'metadata': {replace: OrderedDict()}}, 12: {'metadata': "*

 * *            '{replace: OrderedDict()}}}',*

 * * "'metadata'": "{'language_info': {'version': '3.12.0'}}"}*

```diff
@@ -65,20 +65,15 @@
                 "\n",
                 "This first block imports the data and numpy."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "metadata": {
-                "collapsed": true,
-                "jupyter": {
-                    "outputs_hidden": true
-                }
-            },
+            "metadata": {},
             "outputs": [],
             "source": [
                 "import numpy as np\n",
                 "from linearmodels.datasets import meps\n",
                 "from linearmodels.iv import IV2SLS\n",
                 "\n",
                 "data = meps.load()\n",
@@ -94,37 +89,27 @@
                 "\n",
                 "This model uses a formula which is input using the `from_formula` interface. Unlike direct initialization, this interface takes the formula and a DataFrame containing the data necessary to evaluate the formula."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "metadata": {
-                "collapsed": true,
-                "jupyter": {
-                    "outputs_hidden": true
-                }
-            },
+            "metadata": {},
             "outputs": [],
             "source": [
                 "formula = (\n",
                 "    \"ldrugexp ~ 1 + totchr + female + age + linc + blhisp + [hi_empunion ~ ssiratio]\"\n",
                 ")\n",
                 "mod = IV2SLS.from_formula(formula, data)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "metadata": {
-                "collapsed": true,
-                "jupyter": {
-                    "outputs_hidden": true
-                }
-            },
+            "metadata": {},
             "outputs": [],
             "source": [
                 "iv_res = mod.fit(cov_type=\"robust\")\n",
                 "print(iv_res)"
             ]
         },
         {
@@ -135,20 +120,15 @@
                 "\n",
                 "Standard formulaic syntax, such as using mathematical expressions, can be readily used."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "metadata": {
-                "collapsed": true,
-                "jupyter": {
-                    "outputs_hidden": true
-                }
-            },
+            "metadata": {},
             "outputs": [],
             "source": [
                 "formula = (\n",
                 "    \"np.log(drugexp) ~ 1 + totchr + age + linc + blhisp + [hi_empunion ~ ssiratio]\"\n",
                 ")\n",
                 "mod = IV2SLS.from_formula(formula, data)\n",
                 "iv_res2 = mod.fit(cov_type=\"robust\")"
@@ -162,20 +142,15 @@
                 "\n",
                 "Omitting the block that marks a variable as endogenous will produce OLS -- just like using `None` for both `endog` and `instruments`."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "metadata": {
-                "collapsed": true,
-                "jupyter": {
-                    "outputs_hidden": true
-                }
-            },
+            "metadata": {},
             "outputs": [],
             "source": [
                 "formula = \"ldrugexp ~ 1 + totchr + female + age + linc + blhisp + hi_empunion\"\n",
                 "ols = IV2SLS.from_formula(formula, data)\n",
                 "ols_res = ols.fit(cov_type=\"robust\")\n",
                 "print(ols_res)"
             ]
@@ -188,20 +163,15 @@
                 "\n",
                 "The function `compare` can be used to compare the result of multiple models.  Here dropping `female` from the IV regression improves the $R^2$."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "metadata": {
-                "collapsed": true,
-                "jupyter": {
-                    "outputs_hidden": true
-                }
-            },
+            "metadata": {},
             "outputs": [],
             "source": [
                 "from linearmodels.iv import compare\n",
                 "\n",
                 "print(compare({\"IV\": iv_res, \"OLS\": ols_res, \"IV-formula\": iv_res2}))"
             ]
         }
@@ -218,15 +188,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.11"
+            "version": "3.12.0"
         },
         "pycharm": {
             "stem_cell": {
                 "cell_type": "raw",
                 "metadata": {
                     "collapsed": false
                 },
```

### Comparing `linearmodels-5.3/examples/panel_data-formats.ipynb` & `linearmodels-5.4/examples/panel_data-formats.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9985119047619048%*

 * *Differences: {"'metadata'": "{'language_info': {'version': '3.12.0'}}"}*

```diff
@@ -220,15 +220,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.11"
+            "version": "3.12.0"
         },
         "pycharm": {
             "stem_cell": {
                 "cell_type": "raw",
                 "metadata": {
                     "collapsed": false
                 },
```

### Comparing `linearmodels-5.3/examples/panel_examples.ipynb` & `linearmodels-5.4/examples/panel_examples.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9985119047619048%*

 * *Differences: {"'metadata'": "{'language_info': {'version': '3.12.0'}}"}*

```diff
@@ -423,15 +423,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.11"
+            "version": "3.12.0"
         },
         "pycharm": {
             "stem_cell": {
                 "cell_type": "raw",
                 "metadata": {
                     "collapsed": false
                 },
```

### Comparing `linearmodels-5.3/examples/panel_using-formulas.ipynb` & `linearmodels-5.4/examples/panel_using-formulas.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9985119047619048%*

 * *Differences: {"'metadata'": "{'language_info': {'version': '3.12.0'}}"}*

```diff
@@ -178,15 +178,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.11"
+            "version": "3.12.0"
         },
         "pycharm": {
             "stem_cell": {
                 "cell_type": "raw",
                 "metadata": {
                     "collapsed": false
                 },
```

### Comparing `linearmodels-5.3/examples/system_correct-greene-table-10-1.png` & `linearmodels-5.4/examples/system_correct-greene-table-10-1.png`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/examples/system_correct-greene-table-10-2.png` & `linearmodels-5.4/examples/system_correct-greene-table-10-2.png`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/examples/system_correct-greene-table-10-3.png` & `linearmodels-5.4/examples/system_correct-greene-table-10-3.png`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/examples/system_examples.ipynb` & `linearmodels-5.4/examples/system_examples.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9985119047619048%*

 * *Differences: {"'metadata'": "{'language_info': {'version': '3.12.0'}}"}*

```diff
@@ -776,15 +776,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.11"
+            "version": "3.12.0"
         },
         "pycharm": {
             "stem_cell": {
                 "cell_type": "raw",
                 "metadata": {
                     "collapsed": false
                 },
```

### Comparing `linearmodels-5.3/examples/system_formulas.ipynb` & `linearmodels-5.4/examples/system_formulas.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9965888278388279%*

 * *Differences: {"'cells'": "{1: {'metadata': {replace: OrderedDict()}}, 3: {'metadata': {replace: "*

 * *            'OrderedDict()}}}',*

 * * "'metadata'": "{'language_info': {'version': '3.12.0'}}"}*

```diff
@@ -14,20 +14,15 @@
                 "These examples use data on fringe benefits from F. Vella (1993), \"A Simple Estimator for Simultaneous Models with Censored\n",
                 "Endogenous Regressors\" which appears in Wooldridge (2002).  The model consists of two equations, one for hourly wage and the other for hourly benefits.  The initial model uses the same regressors in both equations. "
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "metadata": {
-                "collapsed": true,
-                "jupyter": {
-                    "outputs_hidden": true
-                }
-            },
+            "metadata": {},
             "outputs": [],
             "source": [
                 "import numpy as np\n",
                 "import pandas as pd\n",
                 "from linearmodels.datasets import fringe\n",
                 "\n",
                 "data = fringe.load()"
@@ -41,20 +36,15 @@
                 "\n",
                 "The dictionary syntax is virtually identical to standard [formulaic syntax](https://matthewwardrop.github.io/formulaic/) where each equation is specified in a key-value pair where the key is the equation label and the value is the formula. It is recommended to use an OrderedDict which will preserve equation order in results. Keys **must** be strings."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "metadata": {
-                "collapsed": true,
-                "jupyter": {
-                    "outputs_hidden": true
-                }
-            },
+            "metadata": {},
             "outputs": [],
             "source": [
                 "from collections import OrderedDict\n",
                 "\n",
                 "formula = OrderedDict()\n",
                 "formula[\n",
                 "    \"benefits\"\n",
@@ -185,15 +175,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.11"
+            "version": "3.12.0"
         },
         "pycharm": {
             "stem_cell": {
                 "cell_type": "raw",
                 "metadata": {
                     "collapsed": false
                 },
```

### Comparing `linearmodels-5.3/examples/system_three-stage-ls.ipynb` & `linearmodels-5.4/examples/system_three-stage-ls.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9985119047619048%*

 * *Differences: {"'metadata'": "{'language_info': {'version': '3.12.0'}}"}*

```diff
@@ -349,15 +349,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.11"
+            "version": "3.12.0"
         },
         "pycharm": {
             "stem_cell": {
                 "cell_type": "raw",
                 "metadata": {
                     "collapsed": false
                 },
```

### Comparing `linearmodels-5.3/github_deploy_key.enc` & `linearmodels-5.4/github_deploy_key.enc`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/linearmodels/__init__.py` & `linearmodels-5.4/linearmodels/__init__.py`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/linearmodels/asset_pricing/covariance.py` & `linearmodels-5.4/linearmodels/asset_pricing/covariance.py`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/linearmodels/asset_pricing/model.py` & `linearmodels-5.4/linearmodels/asset_pricing/model.py`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/linearmodels/asset_pricing/results.py` & `linearmodels-5.4/linearmodels/asset_pricing/results.py`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/linearmodels/conftest.py` & `linearmodels-5.4/linearmodels/conftest.py`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/linearmodels/datasets/birthweight/__init__.py` & `linearmodels-5.4/linearmodels/datasets/birthweight/__init__.py`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/linearmodels/datasets/birthweight/birthweight.csv.bz2` & `linearmodels-5.4/linearmodels/datasets/birthweight/birthweight.csv.bz2`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/linearmodels/datasets/card/__init__.py` & `linearmodels-5.4/linearmodels/datasets/card/__init__.py`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/linearmodels/datasets/card/card.csv.bz2` & `linearmodels-5.4/linearmodels/datasets/card/card.csv.bz2`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/linearmodels/datasets/fertility/__init__.py` & `linearmodels-5.4/linearmodels/datasets/fertility/__init__.py`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/linearmodels/datasets/fertility/fertility.csv.bz2` & `linearmodels-5.4/linearmodels/datasets/fertility/fertility.csv.bz2`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/linearmodels/datasets/french/__init__.py` & `linearmodels-5.4/linearmodels/datasets/french/__init__.py`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/linearmodels/datasets/french/french.csv.bz2` & `linearmodels-5.4/linearmodels/datasets/french/french.csv.bz2`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/linearmodels/datasets/fringe/__init__.py` & `linearmodels-5.4/linearmodels/datasets/fringe/__init__.py`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/linearmodels/datasets/fringe/fringe.csv.bz2` & `linearmodels-5.4/linearmodels/datasets/fringe/fringe.csv.bz2`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/linearmodels/datasets/jobtraining/__init__.py` & `linearmodels-5.4/linearmodels/datasets/jobtraining/__init__.py`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/linearmodels/datasets/jobtraining/jobtraining.csv.bz2` & `linearmodels-5.4/linearmodels/datasets/jobtraining/jobtraining.csv.bz2`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/linearmodels/datasets/meps/__init__.py` & `linearmodels-5.4/linearmodels/datasets/meps/__init__.py`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/linearmodels/datasets/meps/meps.csv.bz2` & `linearmodels-5.4/linearmodels/datasets/meps/meps.csv.bz2`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/linearmodels/datasets/mroz/__init__.py` & `linearmodels-5.4/linearmodels/datasets/mroz/__init__.py`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/linearmodels/datasets/mroz/mroz.csv.bz2` & `linearmodels-5.4/linearmodels/datasets/mroz/mroz.csv.bz2`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/linearmodels/datasets/munnell/__init__.py` & `linearmodels-5.4/linearmodels/datasets/munnell/__init__.py`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/linearmodels/datasets/munnell/munnell.csv.bz2` & `linearmodels-5.4/linearmodels/datasets/munnell/munnell.csv.bz2`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/linearmodels/datasets/wage/__init__.py` & `linearmodels-5.4/linearmodels/datasets/wage/__init__.py`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/linearmodels/datasets/wage/wage.csv.bz2` & `linearmodels-5.4/linearmodels/datasets/wage/wage.csv.bz2`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/linearmodels/datasets/wage_panel/__init__.py` & `linearmodels-5.4/linearmodels/datasets/wage_panel/__init__.py`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/linearmodels/datasets/wage_panel/wage_panel.csv.bz2` & `linearmodels-5.4/linearmodels/datasets/wage_panel/wage_panel.csv.bz2`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/linearmodels/formula.py` & `linearmodels-5.4/linearmodels/formula.py`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/linearmodels/iv/_utility.py` & `linearmodels-5.4/linearmodels/iv/_utility.py`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/linearmodels/iv/absorbing.py` & `linearmodels-5.4/linearmodels/iv/absorbing.py`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/linearmodels/iv/common.py` & `linearmodels-5.4/linearmodels/iv/common.py`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/linearmodels/iv/covariance.py` & `linearmodels-5.4/linearmodels/iv/covariance.py`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/linearmodels/iv/data.py` & `linearmodels-5.4/linearmodels/iv/data.py`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/linearmodels/iv/gmm.py` & `linearmodels-5.4/linearmodels/iv/gmm.py`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/linearmodels/iv/model.py` & `linearmodels-5.4/linearmodels/iv/model.py`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/linearmodels/iv/results.py` & `linearmodels-5.4/linearmodels/iv/results.py`

 * *Files 1% similar despite different names*

```diff
@@ -626,15 +626,15 @@
         return [
             ("R-squared:", _str(self.rsquared)),
             ("Adj. R-squared:", _str(self.rsquared_adj)),
             ("F-statistic:", f_stat),
             ("P-value (F-stat):", pval_format(self.f_statistic.pval)),
             ("Distribution:", str(self.f_statistic.dist_name)),
             ("R-squared (No Effects):", _str(round(self.absorbed_rsquared, 5))),
-            ("Varaibles Absorbed:", _str(self.df_absorbed)),
+            ("Variables Absorbed:", _str(self.df_absorbed)),
         ]
 
     @property
     def absorbed_rsquared(self) -> float:
         """Coefficient of determination (R**2), ignoring absorbed variables"""
         return self._absorbed_rsquared
 
@@ -760,15 +760,19 @@
             "shea.rsquared",
             "f.stat",
             "f.pval",
             "f.dist",
         ]
         out_df = out_df[cols]
         for col in out_df:
-            out_df[col] = to_numeric(out_df[col], errors="ignore")
+            try:
+                out_df[col] = to_numeric(out_df[col])
+            except ValueError:
+                # If an error is raised, ignore and keep the column
+                pass
 
         return out_df
 
     @cached_property
     def individual(self) -> dict[str, OLSResults]:
         """
         Individual model results from first-stage regressions
```

### Comparing `linearmodels-5.3/linearmodels/panel/_utility.c` & `linearmodels-5.4/linearmodels/panel/_utility.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-/* Generated by Cython 3.0.2 */
+/* Generated by Cython 3.0.7 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "define_macros": [
             [
                 "NPY_NO_DEPRECATED_API",
                 "1"
             ]
         ],
         "depends": [
-            "/tmp/build-env-b2_49hlm/lib/python3.10/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/tmp/build-env-b2_49hlm/lib/python3.10/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "/tmp/build-env-b2_49hlm/lib/python3.10/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "/tmp/build-env-b2_49hlm/lib/python3.10/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "/tmp/build-env-b2_49hlm/lib/python3.10/site-packages/numpy/core/include/numpy/ufuncobject.h"
+            "/tmp/build-env-wicvywyh/lib/python3.10/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/tmp/build-env-wicvywyh/lib/python3.10/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/tmp/build-env-wicvywyh/lib/python3.10/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/tmp/build-env-wicvywyh/lib/python3.10/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/tmp/build-env-wicvywyh/lib/python3.10/site-packages/numpy/core/include/numpy/ufuncobject.h"
         ],
         "include_dirs": [
-            "/tmp/build-env-b2_49hlm/lib/python3.10/site-packages/numpy/core/include"
+            "/tmp/build-env-wicvywyh/lib/python3.10/site-packages/numpy/core/include"
         ],
         "name": "linearmodels.panel._utility",
         "sources": [
             "linearmodels/panel/_utility.pyx"
         ]
     },
     "module_name": "linearmodels.panel._utility"
@@ -43,23 +43,23 @@
 
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02070000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.7+ or Python 3.3+.
 #else
-#if CYTHON_LIMITED_API
+#if defined(CYTHON_LIMITED_API) && CYTHON_LIMITED_API
 #define __PYX_EXTRA_ABI_MODULE_NAME "limited"
 #else
 #define __PYX_EXTRA_ABI_MODULE_NAME ""
 #endif
-#define CYTHON_ABI "3_0_2" __PYX_EXTRA_ABI_MODULE_NAME
+#define CYTHON_ABI "3_0_7" __PYX_EXTRA_ABI_MODULE_NAME
 #define __PYX_ABI_MODULE_NAME "_cython_" CYTHON_ABI
 #define __PYX_TYPE_MODULE_PREFIX __PYX_ABI_MODULE_NAME "."
-#define CYTHON_HEX_VERSION 0x030002F0
+#define CYTHON_HEX_VERSION 0x030007F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(_WIN32) && !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -265,15 +265,15 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
-#elif defined(PY_NOGIL)
+#elif defined(Py_GIL_DISABLED) || defined(Py_NOGIL)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 1
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
@@ -592,25 +592,28 @@
 #if CYTHON_COMPILING_IN_LIMITED_API
     static CYTHON_INLINE PyObject* __Pyx_PyCode_New(int a, int p, int k, int l, int s, int f,
                                                     PyObject *code, PyObject *c, PyObject* n, PyObject *v,
                                                     PyObject *fv, PyObject *cell, PyObject* fn,
                                                     PyObject *name, int fline, PyObject *lnos) {
         PyObject *exception_table = NULL;
         PyObject *types_module=NULL, *code_type=NULL, *result=NULL;
+        #if __PYX_LIMITED_VERSION_HEX < 0x030B0000
         PyObject *version_info; // borrowed
         PyObject *py_minor_version = NULL;
+        #endif
         long minor_version = 0;
         PyObject *type, *value, *traceback;
         PyErr_Fetch(&type, &value, &traceback);
         #if __PYX_LIMITED_VERSION_HEX >= 0x030B0000
         minor_version = 11; // we don't yet need to distinguish between versions > 11
         #else
         if (!(version_info = PySys_GetObject("version_info"))) goto end;
         if (!(py_minor_version = PySequence_GetItem(version_info, 1))) goto end;
         minor_version = PyLong_AsLong(py_minor_version);
+        Py_DECREF(py_minor_version);
         if (minor_version == -1 && PyErr_Occurred()) goto end;
         #endif
         if (!(types_module = PyImport_ImportModule("types"))) goto end;
         if (!(code_type = PyObject_GetAttrString(types_module, "CodeType"))) goto end;
         if (minor_version <= 7) {
             (void)p;
             result = PyObject_CallFunction(code_type, "iiiiiOOOOOOiOO", a, k, l, s, f, code,
@@ -623,15 +626,14 @@
             result = PyObject_CallFunction(code_type, "iiiiiiOOOOOOOiOO", a,p, k, l, s, f, code,
                           c, n, v, fn, name, name, fline, lnos, exception_table, fv, cell);
         }
     end:
         Py_XDECREF(code_type);
         Py_XDECREF(exception_table);
         Py_XDECREF(types_module);
-        Py_XDECREF(py_minor_version);
         if (type) {
             PyErr_Restore(type, value, traceback);
         }
         return result;
     }
     #ifndef CO_OPTIMIZED
     #define CO_OPTIMIZED 0x0001
@@ -767,14 +769,39 @@
                                             size_t nargsf, PyObject *kwnames);
   #define __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET  ((size_t)1 << (8 * sizeof(size_t) - 1))
   #define __Pyx_PyVectorcall_NARGS(n)  ((Py_ssize_t)(((size_t)(n)) & ~__Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET))
 #else
   #define __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET  0
   #define __Pyx_PyVectorcall_NARGS(n)  ((Py_ssize_t)(n))
 #endif
+#if PY_MAJOR_VERSION >= 0x030900B1
+#define __Pyx_PyCFunction_CheckExact(func)  PyCFunction_CheckExact(func)
+#else
+#define __Pyx_PyCFunction_CheckExact(func)  PyCFunction_Check(func)
+#endif
+#define __Pyx_CyOrPyCFunction_Check(func)  PyCFunction_Check(func)
+#if CYTHON_COMPILING_IN_CPYTHON
+#define __Pyx_CyOrPyCFunction_GET_FUNCTION(func)  (((PyCFunctionObject*)(func))->m_ml->ml_meth)
+#elif !CYTHON_COMPILING_IN_LIMITED_API
+#define __Pyx_CyOrPyCFunction_GET_FUNCTION(func)  PyCFunction_GET_FUNCTION(func)
+#endif
+#if CYTHON_COMPILING_IN_CPYTHON
+#define __Pyx_CyOrPyCFunction_GET_FLAGS(func)  (((PyCFunctionObject*)(func))->m_ml->ml_flags)
+static CYTHON_INLINE PyObject* __Pyx_CyOrPyCFunction_GET_SELF(PyObject *func) {
+    return (__Pyx_CyOrPyCFunction_GET_FLAGS(func) & METH_STATIC) ? NULL : ((PyCFunctionObject*)func)->m_self;
+}
+#endif
+static CYTHON_INLINE int __Pyx__IsSameCFunction(PyObject *func, void *cfunc) {
+#if CYTHON_COMPILING_IN_LIMITED_API
+    return PyCFunction_Check(func) && PyCFunction_GetFunction(func) == (PyCFunction) cfunc;
+#else
+    return PyCFunction_Check(func) && PyCFunction_GET_FUNCTION(func) == (PyCFunction) cfunc;
+#endif
+}
+#define __Pyx_IsSameCFunction(func, cfunc)   __Pyx__IsSameCFunction(func, cfunc)
 #if __PYX_LIMITED_VERSION_HEX < 0x030900B1
   #define __Pyx_PyType_FromModuleAndSpec(m, s, b)  ((void)m, PyType_FromSpecWithBases(s, b))
   typedef PyObject *(*__Pyx_PyCMethod)(PyObject *, PyTypeObject *, PyObject *const *, size_t, PyObject *);
 #else
   #define __Pyx_PyType_FromModuleAndSpec(m, s, b)  PyType_FromModuleAndSpec(m, s, b)
   #define __Pyx_PyCMethod  PyCMethod
 #endif
@@ -793,14 +820,16 @@
   #define __Pyx_PyCode_HasFreeVars(co)  (PyCode_GetNumFree(co) > 0)
   #define __Pyx_PyFrame_SetLineNumber(frame, lineno)  (frame)->f_lineno = (lineno)
 #endif
 #if CYTHON_COMPILING_IN_LIMITED_API
   #define __Pyx_PyThreadState_Current PyThreadState_Get()
 #elif !CYTHON_FAST_THREAD_STATE
   #define __Pyx_PyThreadState_Current PyThreadState_GET()
+#elif PY_VERSION_HEX >= 0x030d00A1
+  #define __Pyx_PyThreadState_Current PyThreadState_GetUnchecked()
 #elif PY_VERSION_HEX >= 0x03060000
   #define __Pyx_PyThreadState_Current _PyThreadState_UncheckedGet()
 #elif PY_VERSION_HEX >= 0x03000000
   #define __Pyx_PyThreadState_Current PyThreadState_GET()
 #else
   #define __Pyx_PyThreadState_Current _PyThreadState_Current
 #endif
@@ -868,27 +897,27 @@
     #else
         static CYTHON_INLINE int PyGILState_Check(void) {
             PyThreadState * tstate = _PyThreadState_Current;
             return tstate && (tstate == PyGILState_GetThisThreadState());
         }
     #endif
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON || defined(_PyDict_NewPresized)
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030d0000 || defined(_PyDict_NewPresized)
 #define __Pyx_PyDict_NewPresized(n)  ((n <= 8) ? PyDict_New() : _PyDict_NewPresized(n))
 #else
 #define __Pyx_PyDict_NewPresized(n)  PyDict_New()
 #endif
 #if PY_MAJOR_VERSION >= 3 || CYTHON_FUTURE_DIVISION
   #define __Pyx_PyNumber_Divide(x,y)         PyNumber_TrueDivide(x,y)
   #define __Pyx_PyNumber_InPlaceDivide(x,y)  PyNumber_InPlaceTrueDivide(x,y)
 #else
   #define __Pyx_PyNumber_Divide(x,y)         PyNumber_Divide(x,y)
   #define __Pyx_PyNumber_InPlaceDivide(x,y)  PyNumber_InPlaceDivide(x,y)
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX > 0x030600B4 && CYTHON_USE_UNICODE_INTERNALS
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX > 0x030600B4 && PY_VERSION_HEX < 0x030d0000 && CYTHON_USE_UNICODE_INTERNALS
 #define __Pyx_PyDict_GetItemStrWithError(dict, name)  _PyDict_GetItem_KnownHash(dict, name, ((PyASCIIObject *) name)->hash)
 static CYTHON_INLINE PyObject * __Pyx_PyDict_GetItemStr(PyObject *dict, PyObject *name) {
     PyObject *res = __Pyx_PyDict_GetItemStrWithError(dict, name);
     if (res == NULL) PyErr_Clear();
     return res;
 }
 #elif PY_MAJOR_VERSION >= 3 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07020000)
@@ -924,15 +953,15 @@
 #if CYTHON_COMPILING_IN_LIMITED_API
   #define __Pyx_SetItemOnTypeDict(tp, k, v) PyObject_GenericSetAttr((PyObject*)tp, k, v)
 #else
   #define __Pyx_SetItemOnTypeDict(tp, k, v) PyDict_SetItem(tp->tp_dict, k, v)
 #endif
 #if CYTHON_USE_TYPE_SPECS && PY_VERSION_HEX >= 0x03080000
 #define __Pyx_PyHeapTypeObject_GC_Del(obj)  {\
-    PyTypeObject *type = Py_TYPE(obj);\
+    PyTypeObject *type = Py_TYPE((PyObject*)obj);\
     assert(__Pyx_PyType_HasFeature(type, Py_TPFLAGS_HEAPTYPE));\
     PyObject_GC_Del(obj);\
     Py_DECREF(type);\
 }
 #else
 #define __Pyx_PyHeapTypeObject_GC_Del(obj)  PyObject_GC_Del(obj)
 #endif
@@ -1068,14 +1097,23 @@
   #define __Pyx_PyList_SET_ITEM(o, i, v) PyList_SetItem(o, i, v)
   #define __Pyx_PyTuple_GET_SIZE(o) PyTuple_Size(o)
   #define __Pyx_PyList_GET_SIZE(o) PyList_Size(o)
   #define __Pyx_PySet_GET_SIZE(o) PySet_Size(o)
   #define __Pyx_PyBytes_GET_SIZE(o) PyBytes_Size(o)
   #define __Pyx_PyByteArray_GET_SIZE(o) PyByteArray_Size(o)
 #endif
+#if PY_VERSION_HEX >= 0x030d00A1
+  #define __Pyx_PyImport_AddModuleRef(name) PyImport_AddModuleRef(name)
+#else
+  static CYTHON_INLINE PyObject *__Pyx_PyImport_AddModuleRef(const char *name) {
+      PyObject *module = PyImport_AddModule(name);
+      Py_XINCREF(module);
+      return module;
+  }
+#endif
 #if PY_MAJOR_VERSION >= 3
   #define PyIntObject                  PyLongObject
   #define PyInt_Type                   PyLong_Type
   #define PyInt_Check(op)              PyLong_Check(op)
   #define PyInt_CheckExact(op)         PyLong_CheckExact(op)
   #define __Pyx_Py3Int_Check(op)       PyLong_Check(op)
   #define __Pyx_Py3Int_CheckExact(op)  PyLong_CheckExact(op)
@@ -1230,17 +1268,18 @@
 #elif defined (__STDC_VERSION__) && __STDC_VERSION__ >= 199901L
     #define __Pyx_sst_abs(value) llabs(value)
 #elif defined (__GNUC__)
     #define __Pyx_sst_abs(value) __builtin_llabs(value)
 #else
     #define __Pyx_sst_abs(value) ((value<0) ? -value : value)
 #endif
+static CYTHON_INLINE Py_ssize_t __Pyx_ssize_strlen(const char *s);
 static CYTHON_INLINE const char* __Pyx_PyObject_AsString(PyObject*);
 static CYTHON_INLINE const char* __Pyx_PyObject_AsStringAndSize(PyObject*, Py_ssize_t* length);
-#define __Pyx_PyByteArray_FromString(s) PyByteArray_FromStringAndSize((const char*)s, strlen((const char*)s))
+static CYTHON_INLINE PyObject* __Pyx_PyByteArray_FromString(const char*);
 #define __Pyx_PyByteArray_FromStringAndSize(s, l) PyByteArray_FromStringAndSize((const char*)s, l)
 #define __Pyx_PyBytes_FromString        PyBytes_FromString
 #define __Pyx_PyBytes_FromStringAndSize PyBytes_FromStringAndSize
 static CYTHON_INLINE PyObject* __Pyx_PyUnicode_FromString(const char*);
 #if PY_MAJOR_VERSION < 3
     #define __Pyx_PyStr_FromString        __Pyx_PyBytes_FromString
     #define __Pyx_PyStr_FromStringAndSize __Pyx_PyBytes_FromStringAndSize
@@ -1348,14 +1387,15 @@
   #if PY_VERSION_HEX >= 0x030C00A5
   #define __Pyx_PyLong_Digits(x)  (((PyLongObject*)x)->long_value.ob_digit)
   #else
   #define __Pyx_PyLong_Digits(x)  (((PyLongObject*)x)->ob_digit)
   #endif
 #endif
 #if PY_MAJOR_VERSION < 3 && __PYX_DEFAULT_STRING_ENCODING_IS_ASCII
+#include <string.h>
 static int __Pyx_sys_getdefaultencoding_not_ascii;
 static int __Pyx_init_sys_getdefaultencoding_params(void) {
     PyObject* sys;
     PyObject* default_encoding = NULL;
     PyObject* ascii_chars_u = NULL;
     PyObject* ascii_chars_b = NULL;
     const char* default_encoding_c;
@@ -1398,14 +1438,15 @@
 }
 #endif
 #if __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT && PY_MAJOR_VERSION >= 3
 #define __Pyx_PyUnicode_FromStringAndSize(c_str, size) PyUnicode_DecodeUTF8(c_str, size, NULL)
 #else
 #define __Pyx_PyUnicode_FromStringAndSize(c_str, size) PyUnicode_Decode(c_str, size, __PYX_DEFAULT_STRING_ENCODING, NULL)
 #if __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT
+#include <string.h>
 static char* __PYX_DEFAULT_STRING_ENCODING;
 static int __Pyx_init_sys_getdefaultencoding_params(void) {
     PyObject* sys;
     PyObject* default_encoding = NULL;
     char* default_encoding_c;
     sys = PyImport_ImportModule("sys");
     if (!sys) goto bad;
@@ -1445,15 +1486,15 @@
 static const char * __pyx_cfilenm = __FILE__;
 static const char *__pyx_filename;
 
 /* Header.proto */
 #if !defined(CYTHON_CCOMPLEX)
   #if defined(__cplusplus)
     #define CYTHON_CCOMPLEX 1
-  #elif (defined(_Complex_I) && !defined(_MSC_VER)) || ((defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L) && !defined(__STDC_NO_COMPLEX__))
+  #elif (defined(_Complex_I) && !defined(_MSC_VER)) || ((defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L) && !defined(__STDC_NO_COMPLEX__) && !defined(_MSC_VER))
     #define CYTHON_CCOMPLEX 1
   #else
     #define CYTHON_CCOMPLEX 0
   #endif
 #endif
 #if CYTHON_CCOMPLEX
   #ifdef __cplusplus
@@ -1575,14 +1616,15 @@
     #ifdef __PYX_DEBUG_ATOMICS
         #warning "Using GNU atomics"
     #endif
 #elif CYTHON_ATOMICS && defined(_MSC_VER)
     #include <intrin.h>
     #undef __pyx_atomic_int_type
     #define __pyx_atomic_int_type long
+    #undef __pyx_nonatomic_int_type
     #define __pyx_nonatomic_int_type long
     #pragma intrinsic (_InterlockedExchangeAdd)
     #define __pyx_atomic_incr_aligned(value) _InterlockedExchangeAdd(value, 1)
     #define __pyx_atomic_decr_aligned(value) _InterlockedExchangeAdd(value, -1)
     #ifdef __PYX_DEBUG_ATOMICS
         #pragma message ("Using MSVC atomics")
     #endif
@@ -1614,195 +1656,195 @@
   Py_ssize_t strides[8];
   Py_ssize_t suboffsets[8];
 } __Pyx_memviewslice;
 #define __Pyx_MemoryView_Len(m)  (m.shape[0])
 
 /* #### Code section: numeric_typedefs ### */
 
-/* "../../../tmp/build-env-b2_49hlm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":732
+/* "../../../tmp/build-env-wicvywyh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":732
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../tmp/build-env-b2_49hlm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":733
+/* "../../../tmp/build-env-wicvywyh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":733
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../tmp/build-env-b2_49hlm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":734
+/* "../../../tmp/build-env-wicvywyh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":734
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../tmp/build-env-b2_49hlm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":735
+/* "../../../tmp/build-env-wicvywyh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":735
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../tmp/build-env-b2_49hlm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":739
+/* "../../../tmp/build-env-wicvywyh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":739
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../tmp/build-env-b2_49hlm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":740
+/* "../../../tmp/build-env-wicvywyh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":740
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../tmp/build-env-b2_49hlm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":741
+/* "../../../tmp/build-env-wicvywyh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":741
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../tmp/build-env-b2_49hlm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":742
+/* "../../../tmp/build-env-wicvywyh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":742
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../tmp/build-env-b2_49hlm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":746
+/* "../../../tmp/build-env-wicvywyh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":746
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../tmp/build-env-b2_49hlm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":747
+/* "../../../tmp/build-env-wicvywyh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":747
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../tmp/build-env-b2_49hlm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":756
+/* "../../../tmp/build-env-wicvywyh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":756
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../tmp/build-env-b2_49hlm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":757
+/* "../../../tmp/build-env-wicvywyh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":757
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "../../../tmp/build-env-b2_49hlm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":758
+/* "../../../tmp/build-env-wicvywyh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":758
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../tmp/build-env-b2_49hlm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":760
+/* "../../../tmp/build-env-wicvywyh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":760
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../tmp/build-env-b2_49hlm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":761
+/* "../../../tmp/build-env-wicvywyh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":761
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "../../../tmp/build-env-b2_49hlm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":762
+/* "../../../tmp/build-env-wicvywyh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":762
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../tmp/build-env-b2_49hlm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":764
+/* "../../../tmp/build-env-wicvywyh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":764
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../tmp/build-env-b2_49hlm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":765
+/* "../../../tmp/build-env-wicvywyh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":765
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../tmp/build-env-b2_49hlm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":767
+/* "../../../tmp/build-env-wicvywyh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":767
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../tmp/build-env-b2_49hlm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":768
+/* "../../../tmp/build-env-wicvywyh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":768
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../tmp/build-env-b2_49hlm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":769
+/* "../../../tmp/build-env-wicvywyh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":769
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1835,42 +1877,42 @@
 
 /*--- Type declarations ---*/
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "../../../tmp/build-env-b2_49hlm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":771
+/* "../../../tmp/build-env-wicvywyh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":771
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../tmp/build-env-b2_49hlm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":772
+/* "../../../tmp/build-env-wicvywyh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":772
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../tmp/build-env-b2_49hlm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":773
+/* "../../../tmp/build-env-wicvywyh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../tmp/build-env-b2_49hlm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":775
+/* "../../../tmp/build-env-wicvywyh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":775
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -2185,15 +2227,19 @@
 #define __Pyx_GetKwValue_VARARGS(kw, kwvalues, s) __Pyx_PyDict_GetItemStrWithError(kw, s)
 #define __Pyx_KwargsAsDict_VARARGS(kw, kwvalues) PyDict_Copy(kw)
 #if CYTHON_METH_FASTCALL
     #define __Pyx_Arg_FASTCALL(args, i) args[i]
     #define __Pyx_NumKwargs_FASTCALL(kwds) PyTuple_GET_SIZE(kwds)
     #define __Pyx_KwValues_FASTCALL(args, nargs) ((args) + (nargs))
     static CYTHON_INLINE PyObject * __Pyx_GetKwValue_FASTCALL(PyObject *kwnames, PyObject *const *kwvalues, PyObject *s);
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030d0000
+    CYTHON_UNUSED static PyObject *__Pyx_KwargsAsDict_FASTCALL(PyObject *kwnames, PyObject *const *kwvalues);
+  #else
     #define __Pyx_KwargsAsDict_FASTCALL(kw, kwvalues) _PyStack_AsDict(kwvalues, kw)
+  #endif
     #define __Pyx_Arg_NewRef_FASTCALL(arg) arg // no-op, __Pyx_Arg_FASTCALL is direct and this needs
     #define __Pyx_Arg_XDECREF_FASTCALL(arg)  // no-op - arg was returned from array
 #else
     #define __Pyx_Arg_FASTCALL __Pyx_Arg_VARARGS
     #define __Pyx_NumKwargs_FASTCALL __Pyx_NumKwargs_VARARGS
     #define __Pyx_KwValues_FASTCALL __Pyx_KwValues_VARARGS
     #define __Pyx_GetKwValue_FASTCALL __Pyx_GetKwValue_VARARGS
@@ -2510,17 +2556,14 @@
 
 /* ImportDottedModule.proto */
 static PyObject *__Pyx_ImportDottedModule(PyObject *name, PyObject *parts_tuple);
 #if PY_MAJOR_VERSION >= 3
 static PyObject *__Pyx_ImportDottedModule_WalkParts(PyObject *module, PyObject *name, PyObject *parts_tuple);
 #endif
 
-/* ssize_strlen.proto */
-static CYTHON_INLINE Py_ssize_t __Pyx_ssize_strlen(const char *s);
-
 /* FastTypeChecks.proto */
 #if CYTHON_COMPILING_IN_CPYTHON
 #define __Pyx_TypeCheck(obj, type) __Pyx_IsSubtype(Py_TYPE(obj), (PyTypeObject *)type)
 #define __Pyx_TypeCheck2(obj, type1, type2) __Pyx_IsAnySubtype2(Py_TYPE(obj), (PyTypeObject *)type1, (PyTypeObject *)type2)
 static CYTHON_INLINE int __Pyx_IsSubtype(PyTypeObject *a, PyTypeObject *b);
 static CYTHON_INLINE int __Pyx_IsAnySubtype2(PyTypeObject *cls, PyTypeObject *a, PyTypeObject *b);
 static CYTHON_INLINE int __Pyx_PyErr_GivenExceptionMatches(PyObject *err, PyObject *type);
@@ -2538,15 +2581,19 @@
 /* ListCompAppend.proto */
 #if CYTHON_USE_PYLIST_INTERNALS && CYTHON_ASSUME_SAFE_MACROS
 static CYTHON_INLINE int __Pyx_ListComp_Append(PyObject* list, PyObject* x) {
     PyListObject* L = (PyListObject*) list;
     Py_ssize_t len = Py_SIZE(list);
     if (likely(L->allocated > len)) {
         Py_INCREF(x);
+        #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030d0000
+        L->ob_item[len] = x;
+        #else
         PyList_SET_ITEM(list, len, x);
+        #endif
         __Pyx_SET_SIZE(list, len + 1);
         return 0;
     }
     return PyList_Append(list, x);
 }
 #else
 #define __Pyx_ListComp_Append(L,x) PyList_Append(L,x)
@@ -2578,15 +2625,19 @@
     return unlikely(result < 0) ? result : (result == (eq == Py_EQ));
 }
 
 /* ImportFrom.proto */
 static PyObject* __Pyx_ImportFrom(PyObject* module, PyObject* name);
 
 /* HasAttr.proto */
+#if __PYX_LIMITED_VERSION_HEX >= 0x030d00A1
+#define __Pyx_HasAttr(o, n)  PyObject_HasAttrWithError(o, n)
+#else
 static CYTHON_INLINE int __Pyx_HasAttr(PyObject *, PyObject *);
+#endif
 
 /* PyDictContains.proto */
 static CYTHON_INLINE int __Pyx_PyDict_ContainsTF(PyObject* item, PyObject* dict, int eq) {
     int result = PyDict_Contains(dict, item);
     return unlikely(result < 0) ? result : (result == (eq == Py_EQ));
 }
 
@@ -2663,15 +2714,15 @@
 static CYTHON_INLINE PyObject* __Pyx_dict_iterator(PyObject* dict, int is_dict, PyObject* method_name,
                                                    Py_ssize_t* p_orig_length, int* p_is_dict);
 static CYTHON_INLINE int __Pyx_dict_iter_next(PyObject* dict_or_iter, Py_ssize_t orig_length, Py_ssize_t* ppos,
                                               PyObject** pkey, PyObject** pvalue, PyObject** pitem, int is_dict);
 
 /* ListExtend.proto */
 static CYTHON_INLINE int __Pyx_PyList_Extend(PyObject* L, PyObject* v) {
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030d0000
     PyObject* none = _PyList_Extend((PyListObject*)L, v);
     if (unlikely(!none))
         return -1;
     Py_DECREF(none);
     return 0;
 #else
     return PyList_SetSlice(L, PY_SSIZE_T_MAX, PY_SSIZE_T_MAX, v);
@@ -2706,22 +2757,45 @@
                ((cfunc)->flag == METH_VARARGS ?  (*((cfunc)->func))(self, __pyx_empty_tuple) :\
                __Pyx__CallUnboundCMethod0(cfunc, self)))))) :\
         __Pyx__CallUnboundCMethod0(cfunc, self))
 #else
 #define __Pyx_CallUnboundCMethod0(cfunc, self)  __Pyx__CallUnboundCMethod0(cfunc, self)
 #endif
 
+/* dict_getitem_default.proto */
+static PyObject* __Pyx_PyDict_GetItemDefault(PyObject* d, PyObject* key, PyObject* default_value);
+
+/* CallUnboundCMethod1.proto */
+static PyObject* __Pyx__CallUnboundCMethod1(__Pyx_CachedCFunction* cfunc, PyObject* self, PyObject* arg);
+#if CYTHON_COMPILING_IN_CPYTHON
+static CYTHON_INLINE PyObject* __Pyx_CallUnboundCMethod1(__Pyx_CachedCFunction* cfunc, PyObject* self, PyObject* arg);
+#else
+#define __Pyx_CallUnboundCMethod1(cfunc, self, arg)  __Pyx__CallUnboundCMethod1(cfunc, self, arg)
+#endif
+
+/* CallUnboundCMethod2.proto */
+static PyObject* __Pyx__CallUnboundCMethod2(__Pyx_CachedCFunction* cfunc, PyObject* self, PyObject* arg1, PyObject* arg2);
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030600B1
+static CYTHON_INLINE PyObject *__Pyx_CallUnboundCMethod2(__Pyx_CachedCFunction *cfunc, PyObject *self, PyObject *arg1, PyObject *arg2);
+#else
+#define __Pyx_CallUnboundCMethod2(cfunc, self, arg1, arg2)  __Pyx__CallUnboundCMethod2(cfunc, self, arg1, arg2)
+#endif
+
 /* ListAppend.proto */
 #if CYTHON_USE_PYLIST_INTERNALS && CYTHON_ASSUME_SAFE_MACROS
 static CYTHON_INLINE int __Pyx_PyList_Append(PyObject* list, PyObject* x) {
     PyListObject* L = (PyListObject*) list;
     Py_ssize_t len = Py_SIZE(list);
     if (likely(L->allocated > len) & likely(len > (L->allocated >> 1))) {
         Py_INCREF(x);
+        #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030d0000
+        L->ob_item[len] = x;
+        #else
         PyList_SET_ITEM(list, len, x);
+        #endif
         __Pyx_SET_SIZE(list, len + 1);
         return 0;
     }
     return PyList_Append(list, x);
 }
 #else
 #define __Pyx_PyList_Append(L,x) PyList_Append(L,x)
@@ -2770,30 +2844,30 @@
 
 /* SetupReduce.proto */
 #if !CYTHON_COMPILING_IN_LIMITED_API
 static int __Pyx_setup_reduce(PyObject* type_obj);
 #endif
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto_3_0_2
-#define __PYX_HAVE_RT_ImportType_proto_3_0_2
+#ifndef __PYX_HAVE_RT_ImportType_proto_3_0_7
+#define __PYX_HAVE_RT_ImportType_proto_3_0_7
 #if defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L
 #include <stdalign.h>
 #endif
 #if (defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L) || __cplusplus >= 201103L
-#define __PYX_GET_STRUCT_ALIGNMENT_3_0_2(s) alignof(s)
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_7(s) alignof(s)
 #else
-#define __PYX_GET_STRUCT_ALIGNMENT_3_0_2(s) sizeof(void*)
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_7(s) sizeof(void*)
 #endif
-enum __Pyx_ImportType_CheckSize_3_0_2 {
-   __Pyx_ImportType_CheckSize_Error_3_0_2 = 0,
-   __Pyx_ImportType_CheckSize_Warn_3_0_2 = 1,
-   __Pyx_ImportType_CheckSize_Ignore_3_0_2 = 2
+enum __Pyx_ImportType_CheckSize_3_0_7 {
+   __Pyx_ImportType_CheckSize_Error_3_0_7 = 0,
+   __Pyx_ImportType_CheckSize_Warn_3_0_7 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_3_0_7 = 2
 };
-static PyTypeObject *__Pyx_ImportType_3_0_2(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_2 check_size);
+static PyTypeObject *__Pyx_ImportType_3_0_7(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_7 check_size);
 #endif
 
 /* FetchSharedCythonModule.proto */
 static PyObject *__Pyx_FetchSharedCythonABIModule(void);
 
 /* FetchCommonType.proto */
 #if !CYTHON_USE_TYPE_SPECS
@@ -2886,17 +2960,21 @@
     int flags;
     PyObject *defaults_tuple;
     PyObject *defaults_kwdict;
     PyObject *(*defaults_getter)(PyObject *);
     PyObject *func_annotations;
     PyObject *func_is_coroutine;
 } __pyx_CyFunctionObject;
+#undef __Pyx_CyOrPyCFunction_Check
 #define __Pyx_CyFunction_Check(obj)  __Pyx_TypeCheck(obj, __pyx_CyFunctionType)
-#define __Pyx_IsCyOrPyCFunction(obj)  __Pyx_TypeCheck2(obj, __pyx_CyFunctionType, &PyCFunction_Type)
+#define __Pyx_CyOrPyCFunction_Check(obj)  __Pyx_TypeCheck2(obj, __pyx_CyFunctionType, &PyCFunction_Type)
 #define __Pyx_CyFunction_CheckExact(obj)  __Pyx_IS_TYPE(obj, __pyx_CyFunctionType)
+static CYTHON_INLINE int __Pyx__IsSameCyOrCFunction(PyObject *func, void *cfunc);
+#undef __Pyx_IsSameCFunction
+#define __Pyx_IsSameCFunction(func, cfunc)   __Pyx__IsSameCyOrCFunction(func, cfunc)
 static PyObject *__Pyx_CyFunction_Init(__pyx_CyFunctionObject* op, PyMethodDef *ml,
                                       int flags, PyObject* qualname,
                                       PyObject *closure,
                                       PyObject *module, PyObject *globals,
                                       PyObject* code);
 static CYTHON_INLINE void __Pyx__CyFunction_SetClassObj(__pyx_CyFunctionObject* f, PyObject* classobj);
 static CYTHON_INLINE void *__Pyx_CyFunction_InitDefaults(PyObject *m,
@@ -3025,14 +3103,17 @@
 
 /* ObjectToMemviewSlice.proto */
 static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_d_dc_nn___pyx_t_5numpy_int32_t(PyObject *, int writable_flag);
 
 /* ObjectToMemviewSlice.proto */
 static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_d_dc_nn___pyx_t_5numpy_int64_t(PyObject *, int writable_flag);
 
+/* PyUCS4InUnicode.proto */
+static CYTHON_INLINE int __Pyx_UnicodeContainsUCS4(PyObject* unicode, Py_UCS4 character);
+
 /* RealImag.proto */
 #if CYTHON_CCOMPLEX
   #ifdef __cplusplus
     #define __Pyx_CREAL(z) ((z).real())
     #define __Pyx_CIMAG(z) ((z).imag())
   #else
     #define __Pyx_CREAL(z) (__real__(z))
@@ -3158,17 +3239,14 @@
 #define __PYX_XCLEAR_MEMVIEW(slice, have_gil) __Pyx_XCLEAR_MEMVIEW(slice, have_gil, __LINE__)
 static CYTHON_INLINE void __Pyx_INC_MEMVIEW(__Pyx_memviewslice *, int, int);
 static CYTHON_INLINE void __Pyx_XCLEAR_MEMVIEW(__Pyx_memviewslice *, int, int);
 
 /* CIntToPy.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value);
 
-/* BytesContains.proto */
-static CYTHON_INLINE int __Pyx_BytesContains(PyObject* bytes, char character);
-
 /* CIntFromPy.proto */
 static CYTHON_INLINE npy_int8 __Pyx_PyInt_As_npy_int8(PyObject *);
 
 /* CIntFromPy.proto */
 static CYTHON_INLINE npy_int16 __Pyx_PyInt_As_npy_int16(PyObject *);
 
 /* CIntFromPy.proto */
@@ -3203,15 +3281,16 @@
 typedef const char *__Pyx_TypeName;
 #define __Pyx_FMT_TYPENAME "%.200s"
 #define __Pyx_PyType_GetName(tp) ((tp)->tp_name)
 #define __Pyx_DECREF_TypeName(obj)
 #endif
 
 /* CheckBinaryVersion.proto */
-static int __Pyx_check_binary_version(void);
+static unsigned long __Pyx_get_runtime_version(void);
+static int __Pyx_check_binary_version(unsigned long ct_version, unsigned long rt_version, int allow_newer);
 
 /* InitStrings.proto */
 static int __Pyx_InitStrings(__Pyx_StringTabEntry *t);
 
 /* #### Code section: module_declarations ### */
 static PyObject *__pyx_array_get_memview(struct __pyx_array_obj *__pyx_v_self); /* proto*/
 static char *__pyx_memoryview_get_item_pointer(struct __pyx_memoryview_obj *__pyx_v_self, PyObject *__pyx_v_index); /* proto*/
@@ -3334,14 +3413,15 @@
 static const char __pyx_k_gc[] = "gc";
 static const char __pyx_k_id[] = "id";
 static const char __pyx_k__11[] = "()";
 static const char __pyx_k__12[] = "|";
 static const char __pyx_k__28[] = "?";
 static const char __pyx_k_abc[] = "abc";
 static const char __pyx_k_and[] = " and ";
+static const char __pyx_k_get[] = "get";
 static const char __pyx_k_got[] = " (got ";
 static const char __pyx_k_new[] = "__new__";
 static const char __pyx_k_obj[] = "obj";
 static const char __pyx_k_sys[] = "sys";
 static const char __pyx_k_args[] = "args";
 static const char __pyx_k_base[] = "base";
 static const char __pyx_k_dict[] = "__dict__";
@@ -3516,14 +3596,15 @@
 static PyObject *__pyx_pf_12linearmodels_5panel_8_utility_4_drop_singletons(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_meta, __Pyx_memviewslice __pyx_v_orig_dest); /* proto */
 static PyObject *__pyx_pf_12linearmodels_5panel_8_utility_6_drop_singletons(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_meta, __Pyx_memviewslice __pyx_v_orig_dest); /* proto */
 static PyObject *__pyx_pf_12linearmodels_5panel_8_utility_8_drop_singletons(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_meta, __Pyx_memviewslice __pyx_v_orig_dest); /* proto */
 static PyObject *__pyx_tp_new_array(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_Enum(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_memoryview(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new__memoryviewslice(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
+static __Pyx_CachedCFunction __pyx_umethod_PyDict_Type_get = {0, 0, 0, 0, 0};
 static __Pyx_CachedCFunction __pyx_umethod_PyDict_Type_values = {0, 0, 0, 0, 0};
 /* #### Code section: late_includes ### */
 /* #### Code section: module_state ### */
 typedef struct {
   PyObject *__pyx_d;
   PyObject *__pyx_b;
   PyObject *__pyx_cython_runtime;
@@ -3663,14 +3744,15 @@
   PyObject *__pyx_n_s_error;
   PyObject *__pyx_n_s_flags;
   PyObject *__pyx_n_s_format;
   PyObject *__pyx_n_s_fortran;
   PyObject *__pyx_n_u_fortran;
   PyObject *__pyx_n_s_fused_sigindex;
   PyObject *__pyx_kp_u_gc;
+  PyObject *__pyx_n_s_get;
   PyObject *__pyx_n_s_getstate;
   PyObject *__pyx_kp_u_got;
   PyObject *__pyx_kp_u_got_differing_extents_in_dimensi;
   PyObject *__pyx_n_s_i;
   PyObject *__pyx_n_s_id;
   PyObject *__pyx_n_s_import;
   PyObject *__pyx_n_s_index;
@@ -3907,14 +3989,15 @@
   Py_CLEAR(clear_module_state->__pyx_n_s_error);
   Py_CLEAR(clear_module_state->__pyx_n_s_flags);
   Py_CLEAR(clear_module_state->__pyx_n_s_format);
   Py_CLEAR(clear_module_state->__pyx_n_s_fortran);
   Py_CLEAR(clear_module_state->__pyx_n_u_fortran);
   Py_CLEAR(clear_module_state->__pyx_n_s_fused_sigindex);
   Py_CLEAR(clear_module_state->__pyx_kp_u_gc);
+  Py_CLEAR(clear_module_state->__pyx_n_s_get);
   Py_CLEAR(clear_module_state->__pyx_n_s_getstate);
   Py_CLEAR(clear_module_state->__pyx_kp_u_got);
   Py_CLEAR(clear_module_state->__pyx_kp_u_got_differing_extents_in_dimensi);
   Py_CLEAR(clear_module_state->__pyx_n_s_i);
   Py_CLEAR(clear_module_state->__pyx_n_s_id);
   Py_CLEAR(clear_module_state->__pyx_n_s_import);
   Py_CLEAR(clear_module_state->__pyx_n_s_index);
@@ -4129,14 +4212,15 @@
   Py_VISIT(traverse_module_state->__pyx_n_s_error);
   Py_VISIT(traverse_module_state->__pyx_n_s_flags);
   Py_VISIT(traverse_module_state->__pyx_n_s_format);
   Py_VISIT(traverse_module_state->__pyx_n_s_fortran);
   Py_VISIT(traverse_module_state->__pyx_n_u_fortran);
   Py_VISIT(traverse_module_state->__pyx_n_s_fused_sigindex);
   Py_VISIT(traverse_module_state->__pyx_kp_u_gc);
+  Py_VISIT(traverse_module_state->__pyx_n_s_get);
   Py_VISIT(traverse_module_state->__pyx_n_s_getstate);
   Py_VISIT(traverse_module_state->__pyx_kp_u_got);
   Py_VISIT(traverse_module_state->__pyx_kp_u_got_differing_extents_in_dimensi);
   Py_VISIT(traverse_module_state->__pyx_n_s_i);
   Py_VISIT(traverse_module_state->__pyx_n_s_id);
   Py_VISIT(traverse_module_state->__pyx_n_s_import);
   Py_VISIT(traverse_module_state->__pyx_n_s_index);
@@ -4379,14 +4463,15 @@
 #define __pyx_n_s_error __pyx_mstate_global->__pyx_n_s_error
 #define __pyx_n_s_flags __pyx_mstate_global->__pyx_n_s_flags
 #define __pyx_n_s_format __pyx_mstate_global->__pyx_n_s_format
 #define __pyx_n_s_fortran __pyx_mstate_global->__pyx_n_s_fortran
 #define __pyx_n_u_fortran __pyx_mstate_global->__pyx_n_u_fortran
 #define __pyx_n_s_fused_sigindex __pyx_mstate_global->__pyx_n_s_fused_sigindex
 #define __pyx_kp_u_gc __pyx_mstate_global->__pyx_kp_u_gc
+#define __pyx_n_s_get __pyx_mstate_global->__pyx_n_s_get
 #define __pyx_n_s_getstate __pyx_mstate_global->__pyx_n_s_getstate
 #define __pyx_kp_u_got __pyx_mstate_global->__pyx_kp_u_got
 #define __pyx_kp_u_got_differing_extents_in_dimensi __pyx_mstate_global->__pyx_kp_u_got_differing_extents_in_dimensi
 #define __pyx_n_s_i __pyx_mstate_global->__pyx_n_s_i
 #define __pyx_n_s_id __pyx_mstate_global->__pyx_n_s_id
 #define __pyx_n_s_import __pyx_mstate_global->__pyx_n_s_import
 #define __pyx_n_s_index __pyx_mstate_global->__pyx_n_s_index
@@ -4512,16 +4597,15 @@
   int __pyx_clineno = 0;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__cinit__ (wrapper)", 0);
   #if CYTHON_ASSUME_SAFE_MACROS
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
-  __pyx_nargs = PyTuple_Size(__pyx_args);
-  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(1, 131, __pyx_L3_error)
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return -1;
   #endif
   __pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
   {
     PyObject **__pyx_pyargnames[] = {&__pyx_n_s_shape,&__pyx_n_s_itemsize,&__pyx_n_s_format,&__pyx_n_s_mode,&__pyx_n_s_allocate_buffer,0};
     values[3] = __Pyx_Arg_NewRef_VARARGS(((PyObject *)__pyx_n_s_c));
     if (__pyx_kwds) {
       Py_ssize_t kw_args;
@@ -4614,18 +4698,19 @@
  *                   mode="c", bint allocate_buffer=True):             # <<<<<<<<<<<<<<
  * 
  *         cdef int idx
  */
       __pyx_v_allocate_buffer = ((int)1);
     }
   }
-  goto __pyx_L4_argument_unpacking_done;
+  goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 3, 5, __pyx_nargs); __PYX_ERR(1, 131, __pyx_L3_error)
-  goto __pyx_L3_error;
+  __pyx_L6_skip:;
+  goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_VARARGS(values[__pyx_temp]);
     }
   }
@@ -4900,21 +4985,28 @@
  * 
  * 
  *         for idx, dim in enumerate(shape):             # <<<<<<<<<<<<<<
  *             if dim <= 0:
  *                 raise ValueError, f"Invalid shape in axis {idx}: {dim}."
  */
   __pyx_t_7 = 0;
-  __pyx_t_4 = __pyx_v_shape; __Pyx_INCREF(__pyx_t_4); __pyx_t_1 = 0;
+  __pyx_t_4 = __pyx_v_shape; __Pyx_INCREF(__pyx_t_4);
+  __pyx_t_1 = 0;
   for (;;) {
-    if (__pyx_t_1 >= PyTuple_GET_SIZE(__pyx_t_4)) break;
+    {
+      Py_ssize_t __pyx_temp = __Pyx_PyTuple_GET_SIZE(__pyx_t_4);
+      #if !CYTHON_ASSUME_SAFE_MACROS
+      if (unlikely((__pyx_temp < 0))) __PYX_ERR(1, 159, __pyx_L1_error)
+      #endif
+      if (__pyx_t_1 >= __pyx_temp) break;
+    }
     #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
     __pyx_t_5 = PyTuple_GET_ITEM(__pyx_t_4, __pyx_t_1); __Pyx_INCREF(__pyx_t_5); __pyx_t_1++; if (unlikely((0 < 0))) __PYX_ERR(1, 159, __pyx_L1_error)
     #else
-    __pyx_t_5 = PySequence_ITEM(__pyx_t_4, __pyx_t_1); __pyx_t_1++; if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 159, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PySequence_ITEM(__pyx_t_4, __pyx_t_1); __pyx_t_1++; if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 159, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     #endif
     __pyx_t_9 = __Pyx_PyIndex_AsSsize_t(__pyx_t_5); if (unlikely((__pyx_t_9 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(1, 159, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __pyx_v_dim = __pyx_t_9;
     __pyx_v_idx = __pyx_t_7;
     __pyx_t_7 = (__pyx_t_7 + 1);
@@ -5549,18 +5641,16 @@
   __pyx_array___pyx_pf_15View_dot_MemoryView_5array_4__dealloc__(((struct __pyx_array_obj *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
 static void __pyx_array___pyx_pf_15View_dot_MemoryView_5array_4__dealloc__(struct __pyx_array_obj *__pyx_v_self) {
-  __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_t_2;
-  __Pyx_RefNannySetupContext("__dealloc__", 0);
 
   /* "View.MemoryView":211
  * 
  *     def __dealloc__(array self):
  *         if self.callback_free_data != NULL:             # <<<<<<<<<<<<<<
  *             self.callback_free_data(self.data)
  *         elif self.free_data and self.data is not NULL:
@@ -5664,15 +5754,14 @@
  * 
  *     def __dealloc__(array self):             # <<<<<<<<<<<<<<
  *         if self.callback_free_data != NULL:
  *             self.callback_free_data(self.data)
  */
 
   /* function exit code */
-  __Pyx_RefNannyFinishContext();
 }
 
 /* "View.MemoryView":219
  *         PyObject_Free(self._shape)
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def memview(self):
@@ -5697,15 +5786,15 @@
 static PyObject *__pyx_pf_15View_dot_MemoryView_5array_7memview___get__(struct __pyx_array_obj *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__get__", 0);
+  __Pyx_RefNannySetupContext("__get__", 1);
 
   /* "View.MemoryView":221
  *     @property
  *     def memview(self):
  *         return self.get_memview()             # <<<<<<<<<<<<<<
  * 
  *     @cname('get_memview')
@@ -5750,15 +5839,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("get_memview", 0);
+  __Pyx_RefNannySetupContext("get_memview", 1);
 
   /* "View.MemoryView":225
  *     @cname('get_memview')
  *     cdef get_memview(self):
  *         flags =  PyBUF_ANY_CONTIGUOUS|PyBUF_FORMAT|PyBUF_WRITABLE             # <<<<<<<<<<<<<<
  *         return  memoryview(self, flags, self.dtype_is_object)
  * 
@@ -5837,16 +5926,14 @@
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static Py_ssize_t __pyx_array___pyx_pf_15View_dot_MemoryView_5array_6__len__(struct __pyx_array_obj *__pyx_v_self) {
   Py_ssize_t __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__len__", 0);
 
   /* "View.MemoryView":229
  * 
  *     def __len__(self):
  *         return self._shape[0]             # <<<<<<<<<<<<<<
  * 
  *     def __getattr__(self, attr):
@@ -5860,15 +5947,14 @@
  *     def __len__(self):             # <<<<<<<<<<<<<<
  *         return self._shape[0]
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "View.MemoryView":231
  *         return self._shape[0]
  * 
  *     def __getattr__(self, attr):             # <<<<<<<<<<<<<<
@@ -5895,15 +5981,15 @@
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__getattr__", 0);
+  __Pyx_RefNannySetupContext("__getattr__", 1);
 
   /* "View.MemoryView":232
  * 
  *     def __getattr__(self, attr):
  *         return getattr(self.memview, attr)             # <<<<<<<<<<<<<<
  * 
  *     def __getitem__(self, item):
@@ -5965,15 +6051,15 @@
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__getitem__", 0);
+  __Pyx_RefNannySetupContext("__getitem__", 1);
 
   /* "View.MemoryView":235
  * 
  *     def __getitem__(self, item):
  *         return self.memview[item]             # <<<<<<<<<<<<<<
  * 
  *     def __setitem__(self, item, value):
@@ -6034,15 +6120,15 @@
 static int __pyx_array___pyx_pf_15View_dot_MemoryView_5array_12__setitem__(struct __pyx_array_obj *__pyx_v_self, PyObject *__pyx_v_item, PyObject *__pyx_v_value) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__setitem__", 0);
+  __Pyx_RefNannySetupContext("__setitem__", 1);
 
   /* "View.MemoryView":238
  * 
  *     def __setitem__(self, item, value):
  *         self.memview[item] = value             # <<<<<<<<<<<<<<
  * 
  * 
@@ -6093,53 +6179,42 @@
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   #if !CYTHON_METH_FASTCALL
   CYTHON_UNUSED Py_ssize_t __pyx_nargs;
   #endif
   CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__reduce_cython__ (wrapper)", 0);
   #if !CYTHON_METH_FASTCALL
   #if CYTHON_ASSUME_SAFE_MACROS
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
-  __pyx_nargs = PyTuple_Size(__pyx_args);
-  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(1, 1, __pyx_L3_error)
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   #endif
   __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   if (unlikely(__pyx_nargs > 0)) {
     __Pyx_RaiseArgtupleInvalid("__reduce_cython__", 1, 0, 0, __pyx_nargs); return NULL;}
   if (unlikely(__pyx_kwds) && __Pyx_NumKwargs_FASTCALL(__pyx_kwds) && unlikely(!__Pyx_CheckKeywordStrings(__pyx_kwds, "__reduce_cython__", 0))) return NULL;
-  goto __pyx_L4_argument_unpacking_done;
-  goto __pyx_L3_error;
-  __pyx_L3_error:;
-  __Pyx_AddTraceback("View.MemoryView.array.__reduce_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __Pyx_RefNannyFinishContext();
-  return NULL;
-  __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf___pyx_array___reduce_cython__(((struct __pyx_array_obj *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf___pyx_array___reduce_cython__(CYTHON_UNUSED struct __pyx_array_obj *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__reduce_cython__", 0);
+  __Pyx_RefNannySetupContext("__reduce_cython__", 1);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  */
@@ -6195,16 +6270,15 @@
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__setstate_cython__ (wrapper)", 0);
   #if !CYTHON_METH_FASTCALL
   #if CYTHON_ASSUME_SAFE_MACROS
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
-  __pyx_nargs = PyTuple_Size(__pyx_args);
-  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(1, 3, __pyx_L3_error)
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   #endif
   __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   {
     PyObject **__pyx_pyargnames[] = {&__pyx_n_s_pyx_state,0};
     if (__pyx_kwds) {
       Py_ssize_t kw_args;
@@ -6231,18 +6305,19 @@
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v___pyx_state = values[0];
   }
-  goto __pyx_L4_argument_unpacking_done;
+  goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("__setstate_cython__", 1, 1, 1, __pyx_nargs); __PYX_ERR(1, 3, __pyx_L3_error)
-  goto __pyx_L3_error;
+  __pyx_L6_skip:;
+  goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
@@ -6265,15 +6340,15 @@
 
 static PyObject *__pyx_pf___pyx_array_2__setstate_cython__(CYTHON_UNUSED struct __pyx_array_obj *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__setstate_cython__", 0);
+  __Pyx_RefNannySetupContext("__setstate_cython__", 1);
 
   /* "(tree fragment)":4
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"             # <<<<<<<<<<<<<<
  */
   __Pyx_Raise(__pyx_builtin_TypeError, __pyx_kp_s_no_default___reduce___due_to_non, 0, 0);
@@ -6303,23 +6378,21 @@
  * 
  */
 
 static int __pyx_array_allocate_buffer(struct __pyx_array_obj *__pyx_v_self) {
   Py_ssize_t __pyx_v_i;
   PyObject **__pyx_v_p;
   int __pyx_r;
-  __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   Py_ssize_t __pyx_t_2;
   Py_ssize_t __pyx_t_3;
   Py_ssize_t __pyx_t_4;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("_allocate_buffer", 0);
 
   /* "View.MemoryView":254
  *     cdef PyObject **p
  * 
  *     self.free_data = True             # <<<<<<<<<<<<<<
  *     self.data = <char *>malloc(self.len)
  *     if not self.data:
@@ -6449,15 +6522,14 @@
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_AddTraceback("View.MemoryView._allocate_buffer", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "View.MemoryView":268
  * 
  * @cname("__pyx_array_new")
  * cdef array array_cwrapper(tuple shape, Py_ssize_t itemsize, char *format, char *c_mode, char *buf):             # <<<<<<<<<<<<<<
@@ -6473,15 +6545,15 @@
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("array_cwrapper", 0);
+  __Pyx_RefNannySetupContext("array_cwrapper", 1);
 
   /* "View.MemoryView":270
  * cdef array array_cwrapper(tuple shape, Py_ssize_t itemsize, char *format, char *c_mode, char *buf):
  *     cdef array result
  *     cdef str mode = "fortran" if c_mode[0] == b'f' else "c"  # this often comes from a constant C string.             # <<<<<<<<<<<<<<
  * 
  *     if buf is NULL:
@@ -6650,16 +6722,15 @@
   int __pyx_clineno = 0;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__init__ (wrapper)", 0);
   #if CYTHON_ASSUME_SAFE_MACROS
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
-  __pyx_nargs = PyTuple_Size(__pyx_args);
-  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(1, 304, __pyx_L3_error)
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return -1;
   #endif
   __pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
   {
     PyObject **__pyx_pyargnames[] = {&__pyx_n_s_name,0};
     if (__pyx_kwds) {
       Py_ssize_t kw_args;
       switch (__pyx_nargs) {
@@ -6685,18 +6756,19 @@
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_VARARGS(__pyx_args, 0);
     }
     __pyx_v_name = values[0];
   }
-  goto __pyx_L4_argument_unpacking_done;
+  goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("__init__", 1, 1, 1, __pyx_nargs); __PYX_ERR(1, 304, __pyx_L3_error)
-  goto __pyx_L3_error;
+  __pyx_L6_skip:;
+  goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_VARARGS(values[__pyx_temp]);
     }
   }
@@ -6716,15 +6788,15 @@
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static int __pyx_MemviewEnum___pyx_pf_15View_dot_MemoryView_4Enum___init__(struct __pyx_MemviewEnum_obj *__pyx_v_self, PyObject *__pyx_v_name) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__init__", 0);
+  __Pyx_RefNannySetupContext("__init__", 1);
 
   /* "View.MemoryView":305
  *     cdef object name
  *     def __init__(self, name):
  *         self.name = name             # <<<<<<<<<<<<<<
  *     def __repr__(self):
  *         return self.name
@@ -6771,15 +6843,15 @@
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_MemviewEnum___pyx_pf_15View_dot_MemoryView_4Enum_2__repr__(struct __pyx_MemviewEnum_obj *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__repr__", 0);
+  __Pyx_RefNannySetupContext("__repr__", 1);
 
   /* "View.MemoryView":307
  *         self.name = name
  *     def __repr__(self):
  *         return self.name             # <<<<<<<<<<<<<<
  * 
  * cdef generic = Enum("<strided and direct or indirect>")
@@ -6825,39 +6897,28 @@
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   #if !CYTHON_METH_FASTCALL
   CYTHON_UNUSED Py_ssize_t __pyx_nargs;
   #endif
   CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__reduce_cython__ (wrapper)", 0);
   #if !CYTHON_METH_FASTCALL
   #if CYTHON_ASSUME_SAFE_MACROS
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
-  __pyx_nargs = PyTuple_Size(__pyx_args);
-  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(1, 1, __pyx_L3_error)
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   #endif
   __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   if (unlikely(__pyx_nargs > 0)) {
     __Pyx_RaiseArgtupleInvalid("__reduce_cython__", 1, 0, 0, __pyx_nargs); return NULL;}
   if (unlikely(__pyx_kwds) && __Pyx_NumKwargs_FASTCALL(__pyx_kwds) && unlikely(!__Pyx_CheckKeywordStrings(__pyx_kwds, "__reduce_cython__", 0))) return NULL;
-  goto __pyx_L4_argument_unpacking_done;
-  goto __pyx_L3_error;
-  __pyx_L3_error:;
-  __Pyx_AddTraceback("View.MemoryView.Enum.__reduce_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __Pyx_RefNannyFinishContext();
-  return NULL;
-  __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf___pyx_MemviewEnum___reduce_cython__(((struct __pyx_MemviewEnum_obj *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
@@ -6870,15 +6931,15 @@
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__reduce_cython__", 0);
+  __Pyx_RefNannySetupContext("__reduce_cython__", 1);
 
   /* "(tree fragment)":5
  *     cdef object _dict
  *     cdef bint use_setstate
  *     state = (self.name,)             # <<<<<<<<<<<<<<
  *     _dict = getattr(self, '__dict__', None)
  *     if _dict is not None:
@@ -7107,16 +7168,15 @@
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__setstate_cython__ (wrapper)", 0);
   #if !CYTHON_METH_FASTCALL
   #if CYTHON_ASSUME_SAFE_MACROS
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
-  __pyx_nargs = PyTuple_Size(__pyx_args);
-  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(1, 16, __pyx_L3_error)
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   #endif
   __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   {
     PyObject **__pyx_pyargnames[] = {&__pyx_n_s_pyx_state,0};
     if (__pyx_kwds) {
       Py_ssize_t kw_args;
@@ -7143,18 +7203,19 @@
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v___pyx_state = values[0];
   }
-  goto __pyx_L4_argument_unpacking_done;
+  goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("__setstate_cython__", 1, 1, 1, __pyx_nargs); __PYX_ERR(1, 16, __pyx_L3_error)
-  goto __pyx_L3_error;
+  __pyx_L6_skip:;
+  goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
@@ -7178,15 +7239,15 @@
 static PyObject *__pyx_pf___pyx_MemviewEnum_2__setstate_cython__(struct __pyx_MemviewEnum_obj *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__setstate_cython__", 0);
+  __Pyx_RefNannySetupContext("__setstate_cython__", 1);
 
   /* "(tree fragment)":17
  *         return __pyx_unpickle_Enum, (type(self), 0x82a3537, state)
  * def __setstate_cython__(self, __pyx_state):
  *     __pyx_unpickle_Enum__set_state(self, __pyx_state)             # <<<<<<<<<<<<<<
  */
   if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None) || __Pyx_RaiseUnexpectedTypeError("tuple", __pyx_v___pyx_state))) __PYX_ERR(1, 17, __pyx_L1_error)
@@ -7236,16 +7297,15 @@
   int __pyx_clineno = 0;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__cinit__ (wrapper)", 0);
   #if CYTHON_ASSUME_SAFE_MACROS
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
-  __pyx_nargs = PyTuple_Size(__pyx_args);
-  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(1, 349, __pyx_L3_error)
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return -1;
   #endif
   __pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
   {
     PyObject **__pyx_pyargnames[] = {&__pyx_n_s_obj,&__pyx_n_s_flags,&__pyx_n_s_dtype_is_object,0};
     if (__pyx_kwds) {
       Py_ssize_t kw_args;
       switch (__pyx_nargs) {
@@ -7303,18 +7363,19 @@
     __pyx_v_flags = __Pyx_PyInt_As_int(values[1]); if (unlikely((__pyx_v_flags == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 349, __pyx_L3_error)
     if (values[2]) {
       __pyx_v_dtype_is_object = __Pyx_PyObject_IsTrue(values[2]); if (unlikely((__pyx_v_dtype_is_object == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 349, __pyx_L3_error)
     } else {
       __pyx_v_dtype_is_object = ((int)0);
     }
   }
-  goto __pyx_L4_argument_unpacking_done;
+  goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 2, 3, __pyx_nargs); __PYX_ERR(1, 349, __pyx_L3_error)
-  goto __pyx_L3_error;
+  __pyx_L6_skip:;
+  goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_VARARGS(values[__pyx_temp]);
     }
   }
@@ -7342,15 +7403,15 @@
   int __pyx_t_2;
   int __pyx_t_3;
   Py_intptr_t __pyx_t_4;
   size_t __pyx_t_5;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__cinit__", 0);
+  __Pyx_RefNannySetupContext("__cinit__", 1);
 
   /* "View.MemoryView":350
  * 
  *     def __cinit__(memoryview self, object obj, int flags, bint dtype_is_object=False):
  *         self.obj = obj             # <<<<<<<<<<<<<<
  *         self.flags = flags
  *         if type(self) is memoryview or obj is not None:
@@ -7677,22 +7738,20 @@
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
 static void __pyx_memoryview___pyx_pf_15View_dot_MemoryView_10memoryview_2__dealloc__(struct __pyx_memoryview_obj *__pyx_v_self) {
   int __pyx_v_i;
-  __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_t_2;
   int __pyx_t_3;
   int __pyx_t_4;
   PyThread_type_lock __pyx_t_5;
   PyThread_type_lock __pyx_t_6;
-  __Pyx_RefNannySetupContext("__dealloc__", 0);
 
   /* "View.MemoryView":377
  * 
  *     def __dealloc__(memoryview self):
  *         if self.obj is not None:             # <<<<<<<<<<<<<<
  *             __Pyx_ReleaseBuffer(&self.view)
  *         elif (<__pyx_buffer *> &self.view).obj == Py_None:
@@ -7882,15 +7941,14 @@
  * 
  *     def __dealloc__(memoryview self):             # <<<<<<<<<<<<<<
  *         if self.obj is not None:
  *             __Pyx_ReleaseBuffer(&self.view)
  */
 
   /* function exit code */
-  __Pyx_RefNannyFinishContext();
 }
 
 /* "View.MemoryView":397
  *                 PyThread_free_lock(self.lock)
  * 
  *     cdef char *get_item_pointer(memoryview self, object index) except NULL:             # <<<<<<<<<<<<<<
  *         cdef Py_ssize_t dim
@@ -7909,15 +7967,15 @@
   PyObject *(*__pyx_t_4)(PyObject *);
   PyObject *__pyx_t_5 = NULL;
   Py_ssize_t __pyx_t_6;
   char *__pyx_t_7;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("get_item_pointer", 0);
+  __Pyx_RefNannySetupContext("get_item_pointer", 1);
 
   /* "View.MemoryView":399
  *     cdef char *get_item_pointer(memoryview self, object index) except NULL:
  *         cdef Py_ssize_t dim
  *         cdef char *itemp = <char *> self.view.buf             # <<<<<<<<<<<<<<
  * 
  *         for dim, idx in enumerate(index):
@@ -7929,37 +7987,50 @@
  * 
  *         for dim, idx in enumerate(index):             # <<<<<<<<<<<<<<
  *             itemp = pybuffer_index(&self.view, itemp, idx, dim)
  * 
  */
   __pyx_t_1 = 0;
   if (likely(PyList_CheckExact(__pyx_v_index)) || PyTuple_CheckExact(__pyx_v_index)) {
-    __pyx_t_2 = __pyx_v_index; __Pyx_INCREF(__pyx_t_2); __pyx_t_3 = 0;
+    __pyx_t_2 = __pyx_v_index; __Pyx_INCREF(__pyx_t_2);
+    __pyx_t_3 = 0;
     __pyx_t_4 = NULL;
   } else {
     __pyx_t_3 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_v_index); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 401, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_4 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 401, __pyx_L1_error)
   }
   for (;;) {
     if (likely(!__pyx_t_4)) {
       if (likely(PyList_CheckExact(__pyx_t_2))) {
-        if (__pyx_t_3 >= PyList_GET_SIZE(__pyx_t_2)) break;
+        {
+          Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_2);
+          #if !CYTHON_ASSUME_SAFE_MACROS
+          if (unlikely((__pyx_temp < 0))) __PYX_ERR(1, 401, __pyx_L1_error)
+          #endif
+          if (__pyx_t_3 >= __pyx_temp) break;
+        }
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
         __pyx_t_5 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_5); __pyx_t_3++; if (unlikely((0 < 0))) __PYX_ERR(1, 401, __pyx_L1_error)
         #else
-        __pyx_t_5 = PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 401, __pyx_L1_error)
+        __pyx_t_5 = __Pyx_PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 401, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_5);
         #endif
       } else {
-        if (__pyx_t_3 >= PyTuple_GET_SIZE(__pyx_t_2)) break;
+        {
+          Py_ssize_t __pyx_temp = __Pyx_PyTuple_GET_SIZE(__pyx_t_2);
+          #if !CYTHON_ASSUME_SAFE_MACROS
+          if (unlikely((__pyx_temp < 0))) __PYX_ERR(1, 401, __pyx_L1_error)
+          #endif
+          if (__pyx_t_3 >= __pyx_temp) break;
+        }
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
         __pyx_t_5 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_5); __pyx_t_3++; if (unlikely((0 < 0))) __PYX_ERR(1, 401, __pyx_L1_error)
         #else
-        __pyx_t_5 = PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 401, __pyx_L1_error)
+        __pyx_t_5 = __Pyx_PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 401, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_5);
         #endif
       }
     } else {
       __pyx_t_5 = __pyx_t_4(__pyx_t_2);
       if (unlikely(!__pyx_t_5)) {
         PyObject* exc_type = PyErr_Occurred();
@@ -8060,15 +8131,15 @@
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   char *__pyx_t_5;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__getitem__", 0);
+  __Pyx_RefNannySetupContext("__getitem__", 1);
 
   /* "View.MemoryView":408
  * 
  *     def __getitem__(memoryview self, object index):
  *         if index is Ellipsis:             # <<<<<<<<<<<<<<
  *             return self
  * 
@@ -8671,15 +8742,15 @@
   PyObject *__pyx_t_2 = NULL;
   int __pyx_t_3;
   int __pyx_t_4;
   int __pyx_t_5;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("setitem_slice_assignment", 0);
+  __Pyx_RefNannySetupContext("setitem_slice_assignment", 1);
 
   /* "View.MemoryView":448
  *         cdef __Pyx_memviewslice dst_slice
  *         cdef __Pyx_memviewslice src_slice
  *         cdef __Pyx_memviewslice msrc = get_slice_from_memview(src, &src_slice)[0]             # <<<<<<<<<<<<<<
  *         cdef __Pyx_memviewslice mdst = get_slice_from_memview(dst, &dst_slice)[0]
  * 
@@ -8764,15 +8835,15 @@
   PyObject *__pyx_t_9 = NULL;
   PyObject *__pyx_t_10 = NULL;
   PyObject *__pyx_t_11 = NULL;
   PyObject *__pyx_t_12 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("setitem_slice_assign_scalar", 0);
+  __Pyx_RefNannySetupContext("setitem_slice_assign_scalar", 1);
 
   /* "View.MemoryView":455
  *     cdef setitem_slice_assign_scalar(self, memoryview dst, value):
  *         cdef int array[128]
  *         cdef void *tmp = NULL             # <<<<<<<<<<<<<<
  *         cdef void *item
  * 
@@ -9037,15 +9108,15 @@
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   char *__pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("setitem_indexed", 0);
+  __Pyx_RefNannySetupContext("setitem_indexed", 1);
 
   /* "View.MemoryView":486
  * 
  *     cdef setitem_indexed(self, index, value):
  *         cdef char *itemp = self.get_item_pointer(index)             # <<<<<<<<<<<<<<
  *         self.assign_item_from_object(itemp, value)
  * 
@@ -9108,15 +9179,15 @@
   PyObject *__pyx_t_7 = NULL;
   int __pyx_t_8;
   Py_ssize_t __pyx_t_9;
   int __pyx_t_10;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("convert_item_to_object", 0);
+  __Pyx_RefNannySetupContext("convert_item_to_object", 1);
 
   /* "View.MemoryView":492
  *         """Only used if instantiated manually by the user, or if Cython doesn't
  *         know how to convert the type"""
  *         import struct             # <<<<<<<<<<<<<<
  *         cdef bytes bytesitem
  * 
@@ -9358,15 +9429,15 @@
   char *__pyx_t_9;
   char *__pyx_t_10;
   char *__pyx_t_11;
   char *__pyx_t_12;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("assign_item_from_object", 0);
+  __Pyx_RefNannySetupContext("assign_item_from_object", 1);
 
   /* "View.MemoryView":508
  *         """Only used if instantiated manually by the user, or if Cython doesn't
  *         know how to convert the type"""
  *         import struct             # <<<<<<<<<<<<<<
  *         cdef char c
  *         cdef bytes bytesvalue
@@ -9911,15 +9982,15 @@
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__get__", 0);
+  __Pyx_RefNannySetupContext("__get__", 1);
 
   /* "View.MemoryView":556
  *     @property
  *     def T(self):
  *         cdef _memoryviewslice result = memoryview_copy(self)             # <<<<<<<<<<<<<<
  *         transpose_memslice(&result.from_slice)
  *         return result
@@ -9997,15 +10068,15 @@
 static PyObject *__pyx_pf_15View_dot_MemoryView_10memoryview_4base___get__(struct __pyx_memoryview_obj *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__get__", 0);
+  __Pyx_RefNannySetupContext("__get__", 1);
 
   /* "View.MemoryView":562
  *     @property
  *     def base(self):
  *         return self._get_base()             # <<<<<<<<<<<<<<
  * 
  *     cdef _get_base(self):
@@ -10043,15 +10114,15 @@
  *         return self.obj
  * 
  */
 
 static PyObject *__pyx_memoryview__get_base(struct __pyx_memoryview_obj *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("_get_base", 0);
+  __Pyx_RefNannySetupContext("_get_base", 1);
 
   /* "View.MemoryView":565
  * 
  *     cdef _get_base(self):
  *         return self.obj             # <<<<<<<<<<<<<<
  * 
  *     @property
@@ -10107,15 +10178,15 @@
   Py_ssize_t *__pyx_t_2;
   Py_ssize_t *__pyx_t_3;
   Py_ssize_t *__pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__get__", 0);
+  __Pyx_RefNannySetupContext("__get__", 1);
 
   /* "View.MemoryView":569
  *     @property
  *     def shape(self):
  *         return tuple([length for length in self.view.shape[:self.view.ndim]])             # <<<<<<<<<<<<<<
  * 
  *     @property
@@ -10193,15 +10264,15 @@
   Py_ssize_t *__pyx_t_3;
   Py_ssize_t *__pyx_t_4;
   Py_ssize_t *__pyx_t_5;
   PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__get__", 0);
+  __Pyx_RefNannySetupContext("__get__", 1);
 
   /* "View.MemoryView":573
  *     @property
  *     def strides(self):
  *         if self.view.strides == NULL:             # <<<<<<<<<<<<<<
  * 
  *             raise ValueError, "Buffer view does not expose strides"
@@ -10308,15 +10379,15 @@
   Py_ssize_t *__pyx_t_3;
   Py_ssize_t *__pyx_t_4;
   Py_ssize_t *__pyx_t_5;
   PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__get__", 0);
+  __Pyx_RefNannySetupContext("__get__", 1);
 
   /* "View.MemoryView":581
  *     @property
  *     def suboffsets(self):
  *         if self.view.suboffsets == NULL:             # <<<<<<<<<<<<<<
  *             return (-1,) * self.view.ndim
  * 
@@ -10421,15 +10492,15 @@
 static PyObject *__pyx_pf_15View_dot_MemoryView_10memoryview_4ndim___get__(struct __pyx_memoryview_obj *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__get__", 0);
+  __Pyx_RefNannySetupContext("__get__", 1);
 
   /* "View.MemoryView":588
  *     @property
  *     def ndim(self):
  *         return self.view.ndim             # <<<<<<<<<<<<<<
  * 
  *     @property
@@ -10486,15 +10557,15 @@
 static PyObject *__pyx_pf_15View_dot_MemoryView_10memoryview_8itemsize___get__(struct __pyx_memoryview_obj *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__get__", 0);
+  __Pyx_RefNannySetupContext("__get__", 1);
 
   /* "View.MemoryView":592
  *     @property
  *     def itemsize(self):
  *         return self.view.itemsize             # <<<<<<<<<<<<<<
  * 
  *     @property
@@ -10553,15 +10624,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__get__", 0);
+  __Pyx_RefNannySetupContext("__get__", 1);
 
   /* "View.MemoryView":596
  *     @property
  *     def nbytes(self):
  *         return self.size * self.view.itemsize             # <<<<<<<<<<<<<<
  * 
  *     @property
@@ -10632,15 +10703,15 @@
   Py_ssize_t *__pyx_t_2;
   Py_ssize_t *__pyx_t_3;
   Py_ssize_t *__pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__get__", 0);
+  __Pyx_RefNannySetupContext("__get__", 1);
 
   /* "View.MemoryView":600
  *     @property
  *     def size(self):
  *         if self._size is None:             # <<<<<<<<<<<<<<
  *             result = 1
  * 
@@ -10762,17 +10833,15 @@
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static Py_ssize_t __pyx_memoryview___pyx_pf_15View_dot_MemoryView_10memoryview_10__len__(struct __pyx_memoryview_obj *__pyx_v_self) {
   Py_ssize_t __pyx_r;
-  __Pyx_RefNannyDeclarations
   int __pyx_t_1;
-  __Pyx_RefNannySetupContext("__len__", 0);
 
   /* "View.MemoryView":611
  * 
  *     def __len__(self):
  *         if self.view.ndim >= 1:             # <<<<<<<<<<<<<<
  *             return self.view.shape[0]
  * 
@@ -10815,15 +10884,14 @@
  *     def __len__(self):             # <<<<<<<<<<<<<<
  *         if self.view.ndim >= 1:
  *             return self.view.shape[0]
  */
 
   /* function exit code */
   __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "View.MemoryView":616
  *         return 0
  * 
  *     def __repr__(self):             # <<<<<<<<<<<<<<
@@ -10851,15 +10919,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__repr__", 0);
+  __Pyx_RefNannySetupContext("__repr__", 1);
 
   /* "View.MemoryView":617
  * 
  *     def __repr__(self):
  *         return "<MemoryView of %r at 0x%x>" % (self.base.__class__.__name__,             # <<<<<<<<<<<<<<
  *                                                id(self))
  * 
@@ -10954,15 +11022,15 @@
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__str__", 0);
+  __Pyx_RefNannySetupContext("__str__", 1);
 
   /* "View.MemoryView":621
  * 
  *     def __str__(self):
  *         return "<MemoryView of %r object>" % (self.base.__class__.__name__,)             # <<<<<<<<<<<<<<
  * 
  * 
@@ -11031,39 +11099,28 @@
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   #if !CYTHON_METH_FASTCALL
   CYTHON_UNUSED Py_ssize_t __pyx_nargs;
   #endif
   CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_c_contig (wrapper)", 0);
   #if !CYTHON_METH_FASTCALL
   #if CYTHON_ASSUME_SAFE_MACROS
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
-  __pyx_nargs = PyTuple_Size(__pyx_args);
-  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(1, 624, __pyx_L3_error)
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   #endif
   __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   if (unlikely(__pyx_nargs > 0)) {
     __Pyx_RaiseArgtupleInvalid("is_c_contig", 1, 0, 0, __pyx_nargs); return NULL;}
   if (unlikely(__pyx_kwds) && __Pyx_NumKwargs_FASTCALL(__pyx_kwds) && unlikely(!__Pyx_CheckKeywordStrings(__pyx_kwds, "is_c_contig", 0))) return NULL;
-  goto __pyx_L4_argument_unpacking_done;
-  goto __pyx_L3_error;
-  __pyx_L3_error:;
-  __Pyx_AddTraceback("View.MemoryView.memoryview.is_c_contig", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __Pyx_RefNannyFinishContext();
-  return NULL;
-  __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_memoryview___pyx_pf_15View_dot_MemoryView_10memoryview_16is_c_contig(((struct __pyx_memoryview_obj *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
@@ -11073,15 +11130,15 @@
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_memviewslice *__pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("is_c_contig", 0);
+  __Pyx_RefNannySetupContext("is_c_contig", 1);
 
   /* "View.MemoryView":627
  *         cdef __Pyx_memviewslice *mslice
  *         cdef __Pyx_memviewslice tmp
  *         mslice = get_slice_from_memview(self, &tmp)             # <<<<<<<<<<<<<<
  *         return slice_is_contig(mslice[0], 'C', self.view.ndim)
  * 
@@ -11145,39 +11202,28 @@
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   #if !CYTHON_METH_FASTCALL
   CYTHON_UNUSED Py_ssize_t __pyx_nargs;
   #endif
   CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_f_contig (wrapper)", 0);
   #if !CYTHON_METH_FASTCALL
   #if CYTHON_ASSUME_SAFE_MACROS
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
-  __pyx_nargs = PyTuple_Size(__pyx_args);
-  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(1, 630, __pyx_L3_error)
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   #endif
   __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   if (unlikely(__pyx_nargs > 0)) {
     __Pyx_RaiseArgtupleInvalid("is_f_contig", 1, 0, 0, __pyx_nargs); return NULL;}
   if (unlikely(__pyx_kwds) && __Pyx_NumKwargs_FASTCALL(__pyx_kwds) && unlikely(!__Pyx_CheckKeywordStrings(__pyx_kwds, "is_f_contig", 0))) return NULL;
-  goto __pyx_L4_argument_unpacking_done;
-  goto __pyx_L3_error;
-  __pyx_L3_error:;
-  __Pyx_AddTraceback("View.MemoryView.memoryview.is_f_contig", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __Pyx_RefNannyFinishContext();
-  return NULL;
-  __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_memoryview___pyx_pf_15View_dot_MemoryView_10memoryview_18is_f_contig(((struct __pyx_memoryview_obj *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
@@ -11187,15 +11233,15 @@
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_memviewslice *__pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("is_f_contig", 0);
+  __Pyx_RefNannySetupContext("is_f_contig", 1);
 
   /* "View.MemoryView":633
  *         cdef __Pyx_memviewslice *mslice
  *         cdef __Pyx_memviewslice tmp
  *         mslice = get_slice_from_memview(self, &tmp)             # <<<<<<<<<<<<<<
  *         return slice_is_contig(mslice[0], 'F', self.view.ndim)
  * 
@@ -11259,39 +11305,28 @@
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   #if !CYTHON_METH_FASTCALL
   CYTHON_UNUSED Py_ssize_t __pyx_nargs;
   #endif
   CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("copy (wrapper)", 0);
   #if !CYTHON_METH_FASTCALL
   #if CYTHON_ASSUME_SAFE_MACROS
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
-  __pyx_nargs = PyTuple_Size(__pyx_args);
-  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(1, 636, __pyx_L3_error)
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   #endif
   __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   if (unlikely(__pyx_nargs > 0)) {
     __Pyx_RaiseArgtupleInvalid("copy", 1, 0, 0, __pyx_nargs); return NULL;}
   if (unlikely(__pyx_kwds) && __Pyx_NumKwargs_FASTCALL(__pyx_kwds) && unlikely(!__Pyx_CheckKeywordStrings(__pyx_kwds, "copy", 0))) return NULL;
-  goto __pyx_L4_argument_unpacking_done;
-  goto __pyx_L3_error;
-  __pyx_L3_error:;
-  __Pyx_AddTraceback("View.MemoryView.memoryview.copy", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __Pyx_RefNannyFinishContext();
-  return NULL;
-  __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_memoryview___pyx_pf_15View_dot_MemoryView_10memoryview_20copy(((struct __pyx_memoryview_obj *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
@@ -11301,15 +11336,15 @@
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_memviewslice __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("copy", 0);
+  __Pyx_RefNannySetupContext("copy", 1);
 
   /* "View.MemoryView":638
  *     def copy(self):
  *         cdef __Pyx_memviewslice mslice
  *         cdef int flags = self.flags & ~PyBUF_F_CONTIGUOUS             # <<<<<<<<<<<<<<
  * 
  *         slice_copy(self, &mslice)
@@ -11391,39 +11426,28 @@
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   #if !CYTHON_METH_FASTCALL
   CYTHON_UNUSED Py_ssize_t __pyx_nargs;
   #endif
   CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("copy_fortran (wrapper)", 0);
   #if !CYTHON_METH_FASTCALL
   #if CYTHON_ASSUME_SAFE_MACROS
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
-  __pyx_nargs = PyTuple_Size(__pyx_args);
-  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(1, 648, __pyx_L3_error)
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   #endif
   __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   if (unlikely(__pyx_nargs > 0)) {
     __Pyx_RaiseArgtupleInvalid("copy_fortran", 1, 0, 0, __pyx_nargs); return NULL;}
   if (unlikely(__pyx_kwds) && __Pyx_NumKwargs_FASTCALL(__pyx_kwds) && unlikely(!__Pyx_CheckKeywordStrings(__pyx_kwds, "copy_fortran", 0))) return NULL;
-  goto __pyx_L4_argument_unpacking_done;
-  goto __pyx_L3_error;
-  __pyx_L3_error:;
-  __Pyx_AddTraceback("View.MemoryView.memoryview.copy_fortran", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __Pyx_RefNannyFinishContext();
-  return NULL;
-  __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_memoryview___pyx_pf_15View_dot_MemoryView_10memoryview_22copy_fortran(((struct __pyx_memoryview_obj *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
@@ -11434,15 +11458,15 @@
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_memviewslice __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("copy_fortran", 0);
+  __Pyx_RefNannySetupContext("copy_fortran", 1);
 
   /* "View.MemoryView":650
  *     def copy_fortran(self):
  *         cdef __Pyx_memviewslice src, dst
  *         cdef int flags = self.flags & ~PyBUF_C_CONTIGUOUS             # <<<<<<<<<<<<<<
  * 
  *         slice_copy(self, &src)
@@ -11522,53 +11546,42 @@
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   #if !CYTHON_METH_FASTCALL
   CYTHON_UNUSED Py_ssize_t __pyx_nargs;
   #endif
   CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__reduce_cython__ (wrapper)", 0);
   #if !CYTHON_METH_FASTCALL
   #if CYTHON_ASSUME_SAFE_MACROS
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
-  __pyx_nargs = PyTuple_Size(__pyx_args);
-  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(1, 1, __pyx_L3_error)
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   #endif
   __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   if (unlikely(__pyx_nargs > 0)) {
     __Pyx_RaiseArgtupleInvalid("__reduce_cython__", 1, 0, 0, __pyx_nargs); return NULL;}
   if (unlikely(__pyx_kwds) && __Pyx_NumKwargs_FASTCALL(__pyx_kwds) && unlikely(!__Pyx_CheckKeywordStrings(__pyx_kwds, "__reduce_cython__", 0))) return NULL;
-  goto __pyx_L4_argument_unpacking_done;
-  goto __pyx_L3_error;
-  __pyx_L3_error:;
-  __Pyx_AddTraceback("View.MemoryView.memoryview.__reduce_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __Pyx_RefNannyFinishContext();
-  return NULL;
-  __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf___pyx_memoryview___reduce_cython__(((struct __pyx_memoryview_obj *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf___pyx_memoryview___reduce_cython__(CYTHON_UNUSED struct __pyx_memoryview_obj *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__reduce_cython__", 0);
+  __Pyx_RefNannySetupContext("__reduce_cython__", 1);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  */
@@ -11624,16 +11637,15 @@
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__setstate_cython__ (wrapper)", 0);
   #if !CYTHON_METH_FASTCALL
   #if CYTHON_ASSUME_SAFE_MACROS
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
-  __pyx_nargs = PyTuple_Size(__pyx_args);
-  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(1, 3, __pyx_L3_error)
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   #endif
   __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   {
     PyObject **__pyx_pyargnames[] = {&__pyx_n_s_pyx_state,0};
     if (__pyx_kwds) {
       Py_ssize_t kw_args;
@@ -11660,18 +11672,19 @@
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v___pyx_state = values[0];
   }
-  goto __pyx_L4_argument_unpacking_done;
+  goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("__setstate_cython__", 1, 1, 1, __pyx_nargs); __PYX_ERR(1, 3, __pyx_L3_error)
-  goto __pyx_L3_error;
+  __pyx_L6_skip:;
+  goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
@@ -11694,15 +11707,15 @@
 
 static PyObject *__pyx_pf___pyx_memoryview_2__setstate_cython__(CYTHON_UNUSED struct __pyx_memoryview_obj *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__setstate_cython__", 0);
+  __Pyx_RefNannySetupContext("__setstate_cython__", 1);
 
   /* "(tree fragment)":4
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"             # <<<<<<<<<<<<<<
  */
   __Pyx_Raise(__pyx_builtin_TypeError, __pyx_kp_s_no_default___reduce___due_to_non, 0, 0);
@@ -11738,15 +11751,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("memoryview_cwrapper", 0);
+  __Pyx_RefNannySetupContext("memoryview_cwrapper", 1);
 
   /* "View.MemoryView":663
  * @cname('__pyx_memoryview_new')
  * cdef memoryview_cwrapper(object o, int flags, bint dtype_is_object, __Pyx_TypeInfo *typeinfo):
  *     cdef memoryview result = memoryview(o, flags, dtype_is_object)             # <<<<<<<<<<<<<<
  *     result.typeinfo = typeinfo
  *     return result
@@ -11821,17 +11834,15 @@
  * cdef inline bint memoryview_check(object o) noexcept:             # <<<<<<<<<<<<<<
  *     return isinstance(o, memoryview)
  * 
  */
 
 static CYTHON_INLINE int __pyx_memoryview_check(PyObject *__pyx_v_o) {
   int __pyx_r;
-  __Pyx_RefNannyDeclarations
   int __pyx_t_1;
-  __Pyx_RefNannySetupContext("memoryview_check", 0);
 
   /* "View.MemoryView":669
  * @cname('__pyx_memoryview_check')
  * cdef inline bint memoryview_check(object o) noexcept:
  *     return isinstance(o, memoryview)             # <<<<<<<<<<<<<<
  * 
  * cdef tuple _unellipsify(object index, int ndim):
@@ -11846,15 +11857,14 @@
  * cdef inline bint memoryview_check(object o) noexcept:             # <<<<<<<<<<<<<<
  *     return isinstance(o, memoryview)
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "View.MemoryView":671
  *     return isinstance(o, memoryview)
  * 
  * cdef tuple _unellipsify(object index, int ndim):             # <<<<<<<<<<<<<<
@@ -11878,15 +11888,15 @@
   Py_ssize_t __pyx_t_4;
   Py_ssize_t __pyx_t_5;
   Py_UCS4 __pyx_t_6;
   PyObject *__pyx_t_7 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("_unellipsify", 0);
+  __Pyx_RefNannySetupContext("_unellipsify", 1);
 
   /* "View.MemoryView":677
  *     """
  *     cdef Py_ssize_t idx
  *     tup = <tuple>index if isinstance(index, tuple) else (index,)             # <<<<<<<<<<<<<<
  * 
  *     result = [slice(None)] * ndim
@@ -11960,21 +11970,28 @@
  *         if item is Ellipsis:
  *             if not seen_ellipsis:
  */
   if (unlikely(__pyx_v_tup == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not iterable");
     __PYX_ERR(1, 683, __pyx_L1_error)
   }
-  __pyx_t_1 = __pyx_v_tup; __Pyx_INCREF(__pyx_t_1); __pyx_t_4 = 0;
+  __pyx_t_1 = __pyx_v_tup; __Pyx_INCREF(__pyx_t_1);
+  __pyx_t_4 = 0;
   for (;;) {
-    if (__pyx_t_4 >= PyTuple_GET_SIZE(__pyx_t_1)) break;
+    {
+      Py_ssize_t __pyx_temp = __Pyx_PyTuple_GET_SIZE(__pyx_t_1);
+      #if !CYTHON_ASSUME_SAFE_MACROS
+      if (unlikely((__pyx_temp < 0))) __PYX_ERR(1, 683, __pyx_L1_error)
+      #endif
+      if (__pyx_t_4 >= __pyx_temp) break;
+    }
     #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
     __pyx_t_3 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_4); __Pyx_INCREF(__pyx_t_3); __pyx_t_4++; if (unlikely((0 < 0))) __PYX_ERR(1, 683, __pyx_L1_error)
     #else
-    __pyx_t_3 = PySequence_ITEM(__pyx_t_1, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 683, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PySequence_ITEM(__pyx_t_1, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 683, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     #endif
     __Pyx_XDECREF_SET(__pyx_v_item, __pyx_t_3);
     __pyx_t_3 = 0;
 
     /* "View.MemoryView":684
  *     idx = 0
@@ -12235,23 +12252,21 @@
  *     for suboffset in suboffsets[:ndim]:
  *         if suboffset >= 0:
  */
 
 static int assert_direct_dimensions(Py_ssize_t *__pyx_v_suboffsets, int __pyx_v_ndim) {
   Py_ssize_t __pyx_v_suboffset;
   int __pyx_r;
-  __Pyx_RefNannyDeclarations
   Py_ssize_t *__pyx_t_1;
   Py_ssize_t *__pyx_t_2;
   Py_ssize_t *__pyx_t_3;
   int __pyx_t_4;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("assert_direct_dimensions", 0);
 
   /* "View.MemoryView":701
  * 
  * cdef int assert_direct_dimensions(Py_ssize_t *suboffsets, int ndim) except -1:
  *     for suboffset in suboffsets[:ndim]:             # <<<<<<<<<<<<<<
  *         if suboffset >= 0:
  *             raise ValueError, "Indirect dimensions not supported"
@@ -12310,15 +12325,14 @@
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_AddTraceback("View.MemoryView.assert_direct_dimensions", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "View.MemoryView":711
  * 
  * @cname('__pyx_memview_slice')
  * cdef memoryview memview_slice(memoryview memview, object indices):             # <<<<<<<<<<<<<<
@@ -12356,15 +12370,15 @@
   PyObject *__pyx_t_8 = NULL;
   Py_ssize_t __pyx_t_9;
   int __pyx_t_10;
   Py_ssize_t __pyx_t_11;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("memview_slice", 0);
+  __Pyx_RefNannySetupContext("memview_slice", 1);
 
   /* "View.MemoryView":712
  * @cname('__pyx_memview_slice')
  * cdef memoryview memview_slice(memoryview memview, object indices):
  *     cdef int new_ndim = 0, suboffset_dim = -1, dim             # <<<<<<<<<<<<<<
  *     cdef bint negative_step
  *     cdef __Pyx_memviewslice src, dst
@@ -12506,37 +12520,50 @@
  * 
  *     for dim, index in enumerate(indices):             # <<<<<<<<<<<<<<
  *         if PyIndex_Check(index):
  *             cindex = index
  */
   __pyx_t_5 = 0;
   if (likely(PyList_CheckExact(__pyx_v_indices)) || PyTuple_CheckExact(__pyx_v_indices)) {
-    __pyx_t_2 = __pyx_v_indices; __Pyx_INCREF(__pyx_t_2); __pyx_t_6 = 0;
+    __pyx_t_2 = __pyx_v_indices; __Pyx_INCREF(__pyx_t_2);
+    __pyx_t_6 = 0;
     __pyx_t_7 = NULL;
   } else {
     __pyx_t_6 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_v_indices); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 747, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_7 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_2); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 747, __pyx_L1_error)
   }
   for (;;) {
     if (likely(!__pyx_t_7)) {
       if (likely(PyList_CheckExact(__pyx_t_2))) {
-        if (__pyx_t_6 >= PyList_GET_SIZE(__pyx_t_2)) break;
+        {
+          Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_2);
+          #if !CYTHON_ASSUME_SAFE_MACROS
+          if (unlikely((__pyx_temp < 0))) __PYX_ERR(1, 747, __pyx_L1_error)
+          #endif
+          if (__pyx_t_6 >= __pyx_temp) break;
+        }
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
         __pyx_t_8 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_6); __Pyx_INCREF(__pyx_t_8); __pyx_t_6++; if (unlikely((0 < 0))) __PYX_ERR(1, 747, __pyx_L1_error)
         #else
-        __pyx_t_8 = PySequence_ITEM(__pyx_t_2, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 747, __pyx_L1_error)
+        __pyx_t_8 = __Pyx_PySequence_ITEM(__pyx_t_2, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 747, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_8);
         #endif
       } else {
-        if (__pyx_t_6 >= PyTuple_GET_SIZE(__pyx_t_2)) break;
+        {
+          Py_ssize_t __pyx_temp = __Pyx_PyTuple_GET_SIZE(__pyx_t_2);
+          #if !CYTHON_ASSUME_SAFE_MACROS
+          if (unlikely((__pyx_temp < 0))) __PYX_ERR(1, 747, __pyx_L1_error)
+          #endif
+          if (__pyx_t_6 >= __pyx_temp) break;
+        }
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
         __pyx_t_8 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_6); __Pyx_INCREF(__pyx_t_8); __pyx_t_6++; if (unlikely((0 < 0))) __PYX_ERR(1, 747, __pyx_L1_error)
         #else
-        __pyx_t_8 = PySequence_ITEM(__pyx_t_2, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 747, __pyx_L1_error)
+        __pyx_t_8 = __Pyx_PySequence_ITEM(__pyx_t_2, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 747, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_8);
         #endif
       }
     } else {
       __pyx_t_8 = __pyx_t_7(__pyx_t_2);
       if (unlikely(!__pyx_t_8)) {
         PyObject* exc_type = PyErr_Occurred();
@@ -12907,25 +12934,23 @@
  *         Py_ssize_t shape, Py_ssize_t stride, Py_ssize_t suboffset,
  */
 
 static int __pyx_memoryview_slice_memviewslice(__Pyx_memviewslice *__pyx_v_dst, Py_ssize_t __pyx_v_shape, Py_ssize_t __pyx_v_stride, Py_ssize_t __pyx_v_suboffset, int __pyx_v_dim, int __pyx_v_new_ndim, int *__pyx_v_suboffset_dim, Py_ssize_t __pyx_v_start, Py_ssize_t __pyx_v_stop, Py_ssize_t __pyx_v_step, int __pyx_v_have_start, int __pyx_v_have_stop, int __pyx_v_have_step, int __pyx_v_is_slice) {
   Py_ssize_t __pyx_v_new_shape;
   int __pyx_v_negative_step;
   int __pyx_r;
-  __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_t_2;
   int __pyx_t_3;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   #ifdef WITH_THREAD
   PyGILState_STATE __pyx_gilstate_save;
   #endif
-  __Pyx_RefNannySetupContext("slice_memviewslice", 1);
 
   /* "View.MemoryView":813
  *     cdef bint negative_step
  * 
  *     if not is_slice:             # <<<<<<<<<<<<<<
  * 
  *         if start < 0:
@@ -13672,15 +13697,14 @@
   #endif
   __Pyx_AddTraceback("View.MemoryView.slice_memviewslice", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   #ifdef WITH_THREAD
   __Pyx_PyGILState_Release(__pyx_gilstate_save);
   #endif
   __pyx_L0:;
-  __Pyx_RefNannyFinishContextNogil()
   return __pyx_r;
 }
 
 /* "View.MemoryView":896
  * 
  * @cname('__pyx_pybuffer_index')
  * cdef char *pybuffer_index(Py_buffer *view, char *bufp, Py_ssize_t index,             # <<<<<<<<<<<<<<
@@ -13700,15 +13724,15 @@
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   Py_UCS4 __pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("pybuffer_index", 0);
+  __Pyx_RefNannySetupContext("pybuffer_index", 1);
 
   /* "View.MemoryView":898
  * cdef char *pybuffer_index(Py_buffer *view, char *bufp, Py_ssize_t index,
  *                           Py_ssize_t dim) except NULL:
  *     cdef Py_ssize_t shape, stride, suboffset = -1             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t itemsize = view.itemsize
  *     cdef char *resultp
@@ -14027,15 +14051,14 @@
 static int __pyx_memslice_transpose(__Pyx_memviewslice *__pyx_v_memslice) {
   int __pyx_v_ndim;
   Py_ssize_t *__pyx_v_shape;
   Py_ssize_t *__pyx_v_strides;
   int __pyx_v_i;
   int __pyx_v_j;
   int __pyx_r;
-  __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   Py_ssize_t *__pyx_t_2;
   long __pyx_t_3;
   long __pyx_t_4;
   Py_ssize_t __pyx_t_5;
   Py_ssize_t __pyx_t_6;
   int __pyx_t_7;
@@ -14043,15 +14066,14 @@
   int __pyx_t_9;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   #ifdef WITH_THREAD
   PyGILState_STATE __pyx_gilstate_save;
   #endif
-  __Pyx_RefNannySetupContext("transpose_memslice", 1);
 
   /* "View.MemoryView":930
  * @cname('__pyx_memslice_transpose')
  * cdef int transpose_memslice(__Pyx_memviewslice *memslice) except -1 nogil:
  *     cdef int ndim = memslice.memview.view.ndim             # <<<<<<<<<<<<<<
  * 
  *     cdef Py_ssize_t *shape = memslice.shape
@@ -14186,15 +14208,14 @@
   #endif
   __Pyx_AddTraceback("View.MemoryView.transpose_memslice", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   #ifdef WITH_THREAD
   __Pyx_PyGILState_Release(__pyx_gilstate_save);
   #endif
   __pyx_L0:;
-  __Pyx_RefNannyFinishContextNogil()
   return __pyx_r;
 }
 
 /* "View.MemoryView":963
  *     cdef int (*to_dtype_func)(char *, object) except 0
  * 
  *     def __dealloc__(self):             # <<<<<<<<<<<<<<
@@ -14212,16 +14233,14 @@
   __pyx_memoryviewslice___pyx_pf_15View_dot_MemoryView_16_memoryviewslice___dealloc__(((struct __pyx_memoryviewslice_obj *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
 static void __pyx_memoryviewslice___pyx_pf_15View_dot_MemoryView_16_memoryviewslice___dealloc__(struct __pyx_memoryviewslice_obj *__pyx_v_self) {
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__dealloc__", 0);
 
   /* "View.MemoryView":964
  * 
  *     def __dealloc__(self):
  *         __PYX_XCLEAR_MEMVIEW(&self.from_slice, 1)             # <<<<<<<<<<<<<<
  * 
  *     cdef convert_item_to_object(self, char *itemp):
@@ -14233,15 +14252,14 @@
  * 
  *     def __dealloc__(self):             # <<<<<<<<<<<<<<
  *         __PYX_XCLEAR_MEMVIEW(&self.from_slice, 1)
  * 
  */
 
   /* function exit code */
-  __Pyx_RefNannyFinishContext();
 }
 
 /* "View.MemoryView":966
  *         __PYX_XCLEAR_MEMVIEW(&self.from_slice, 1)
  * 
  *     cdef convert_item_to_object(self, char *itemp):             # <<<<<<<<<<<<<<
  *         if self.to_object_func != NULL:
@@ -14252,15 +14270,15 @@
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("convert_item_to_object", 0);
+  __Pyx_RefNannySetupContext("convert_item_to_object", 1);
 
   /* "View.MemoryView":967
  * 
  *     cdef convert_item_to_object(self, char *itemp):
  *         if self.to_object_func != NULL:             # <<<<<<<<<<<<<<
  *             return self.to_object_func(itemp)
  *         else:
@@ -14339,15 +14357,15 @@
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("assign_item_from_object", 0);
+  __Pyx_RefNannySetupContext("assign_item_from_object", 1);
 
   /* "View.MemoryView":973
  * 
  *     cdef assign_item_from_object(self, char *itemp, object value):
  *         if self.to_dtype_func != NULL:             # <<<<<<<<<<<<<<
  *             self.to_dtype_func(itemp, value)
  *         else:
@@ -14416,15 +14434,15 @@
  *         return self.from_object
  * 
  */
 
 static PyObject *__pyx_memoryviewslice__get_base(struct __pyx_memoryviewslice_obj *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("_get_base", 0);
+  __Pyx_RefNannySetupContext("_get_base", 1);
 
   /* "View.MemoryView":979
  * 
  *     cdef _get_base(self):
  *         return self.from_object             # <<<<<<<<<<<<<<
  * 
  * 
@@ -14470,53 +14488,42 @@
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   #if !CYTHON_METH_FASTCALL
   CYTHON_UNUSED Py_ssize_t __pyx_nargs;
   #endif
   CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__reduce_cython__ (wrapper)", 0);
   #if !CYTHON_METH_FASTCALL
   #if CYTHON_ASSUME_SAFE_MACROS
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
-  __pyx_nargs = PyTuple_Size(__pyx_args);
-  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(1, 1, __pyx_L3_error)
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   #endif
   __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   if (unlikely(__pyx_nargs > 0)) {
     __Pyx_RaiseArgtupleInvalid("__reduce_cython__", 1, 0, 0, __pyx_nargs); return NULL;}
   if (unlikely(__pyx_kwds) && __Pyx_NumKwargs_FASTCALL(__pyx_kwds) && unlikely(!__Pyx_CheckKeywordStrings(__pyx_kwds, "__reduce_cython__", 0))) return NULL;
-  goto __pyx_L4_argument_unpacking_done;
-  goto __pyx_L3_error;
-  __pyx_L3_error:;
-  __Pyx_AddTraceback("View.MemoryView._memoryviewslice.__reduce_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __Pyx_RefNannyFinishContext();
-  return NULL;
-  __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf___pyx_memoryviewslice___reduce_cython__(((struct __pyx_memoryviewslice_obj *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf___pyx_memoryviewslice___reduce_cython__(CYTHON_UNUSED struct __pyx_memoryviewslice_obj *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__reduce_cython__", 0);
+  __Pyx_RefNannySetupContext("__reduce_cython__", 1);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  */
@@ -14572,16 +14579,15 @@
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__setstate_cython__ (wrapper)", 0);
   #if !CYTHON_METH_FASTCALL
   #if CYTHON_ASSUME_SAFE_MACROS
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
-  __pyx_nargs = PyTuple_Size(__pyx_args);
-  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(1, 3, __pyx_L3_error)
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   #endif
   __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   {
     PyObject **__pyx_pyargnames[] = {&__pyx_n_s_pyx_state,0};
     if (__pyx_kwds) {
       Py_ssize_t kw_args;
@@ -14608,18 +14614,19 @@
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v___pyx_state = values[0];
   }
-  goto __pyx_L4_argument_unpacking_done;
+  goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("__setstate_cython__", 1, 1, 1, __pyx_nargs); __PYX_ERR(1, 3, __pyx_L3_error)
-  goto __pyx_L3_error;
+  __pyx_L6_skip:;
+  goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
@@ -14642,15 +14649,15 @@
 
 static PyObject *__pyx_pf___pyx_memoryviewslice_2__setstate_cython__(CYTHON_UNUSED struct __pyx_memoryviewslice_obj *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__setstate_cython__", 0);
+  __Pyx_RefNannySetupContext("__setstate_cython__", 1);
 
   /* "(tree fragment)":4
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"             # <<<<<<<<<<<<<<
  */
   __Pyx_Raise(__pyx_builtin_TypeError, __pyx_kp_s_no_default___reduce___due_to_non, 0, 0);
@@ -14694,15 +14701,15 @@
   Py_ssize_t *__pyx_t_6;
   Py_ssize_t *__pyx_t_7;
   Py_ssize_t *__pyx_t_8;
   Py_ssize_t __pyx_t_9;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("memoryview_fromslice", 0);
+  __Pyx_RefNannySetupContext("memoryview_fromslice", 1);
 
   /* "View.MemoryView":1007
  *     cdef _memoryviewslice result
  * 
  *     if <PyObject *> memviewslice.memview == Py_None:             # <<<<<<<<<<<<<<
  *         return None
  * 
@@ -15071,15 +15078,15 @@
   __Pyx_memviewslice *__pyx_r;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("get_slice_from_memview", 0);
+  __Pyx_RefNannySetupContext("get_slice_from_memview", 1);
 
   /* "View.MemoryView":1055
  *                                                    __Pyx_memviewslice *mslice) except NULL:
  *     cdef _memoryviewslice obj
  *     if isinstance(memview, _memoryviewslice):             # <<<<<<<<<<<<<<
  *         obj = memview
  *         return &obj.from_slice
@@ -15168,22 +15175,20 @@
  */
 
 static void __pyx_memoryview_slice_copy(struct __pyx_memoryview_obj *__pyx_v_memview, __Pyx_memviewslice *__pyx_v_dst) {
   int __pyx_v_dim;
   Py_ssize_t *__pyx_v_shape;
   Py_ssize_t *__pyx_v_strides;
   Py_ssize_t *__pyx_v_suboffsets;
-  __Pyx_RefNannyDeclarations
   Py_ssize_t *__pyx_t_1;
   int __pyx_t_2;
   int __pyx_t_3;
   int __pyx_t_4;
   Py_ssize_t __pyx_t_5;
   int __pyx_t_6;
-  __Pyx_RefNannySetupContext("slice_copy", 0);
 
   /* "View.MemoryView":1067
  *     cdef (Py_ssize_t*) shape, strides, suboffsets
  * 
  *     shape = memview.view.shape             # <<<<<<<<<<<<<<
  *     strides = memview.view.strides
  *     suboffsets = memview.view.suboffsets
@@ -15280,15 +15285,14 @@
  * @cname('__pyx_memoryview_slice_copy')
  * cdef void slice_copy(memoryview memview, __Pyx_memviewslice *dst) noexcept:             # <<<<<<<<<<<<<<
  *     cdef int dim
  *     cdef (Py_ssize_t*) shape, strides, suboffsets
  */
 
   /* function exit code */
-  __Pyx_RefNannyFinishContext();
 }
 
 /* "View.MemoryView":1080
  * 
  * @cname('__pyx_memoryview_copy_object')
  * cdef memoryview_copy(memoryview memview):             # <<<<<<<<<<<<<<
  *     "Create a new memoryview object"
@@ -15299,15 +15303,15 @@
   __Pyx_memviewslice __pyx_v_memviewslice;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("memoryview_copy", 0);
+  __Pyx_RefNannySetupContext("memoryview_copy", 1);
 
   /* "View.MemoryView":1083
  *     "Create a new memoryview object"
  *     cdef __Pyx_memviewslice memviewslice
  *     slice_copy(memview, &memviewslice)             # <<<<<<<<<<<<<<
  *     return memoryview_copy_from_slice(memview, &memviewslice)
  * 
@@ -15363,15 +15367,15 @@
   int __pyx_t_1;
   PyObject *(*__pyx_t_2)(char *);
   int (*__pyx_t_3)(char *, PyObject *);
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("memoryview_copy_from_slice", 0);
+  __Pyx_RefNannySetupContext("memoryview_copy_from_slice", 1);
 
   /* "View.MemoryView":1094
  *     cdef int (*to_dtype_func)(char *, object) except 0
  * 
  *     if isinstance(memview, _memoryviewslice):             # <<<<<<<<<<<<<<
  *         to_object_func = (<_memoryviewslice> memview).to_object_func
  *         to_dtype_func = (<_memoryviewslice> memview).to_dtype_func
@@ -16172,28 +16176,26 @@
 
 static void *__pyx_memoryview_copy_data_to_temp(__Pyx_memviewslice *__pyx_v_src, __Pyx_memviewslice *__pyx_v_tmpslice, char __pyx_v_order, int __pyx_v_ndim) {
   int __pyx_v_i;
   void *__pyx_v_result;
   size_t __pyx_v_itemsize;
   size_t __pyx_v_size;
   void *__pyx_r;
-  __Pyx_RefNannyDeclarations
   Py_ssize_t __pyx_t_1;
   int __pyx_t_2;
   int __pyx_t_3;
   struct __pyx_memoryview_obj *__pyx_t_4;
   int __pyx_t_5;
   int __pyx_t_6;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   #ifdef WITH_THREAD
   PyGILState_STATE __pyx_gilstate_save;
   #endif
-  __Pyx_RefNannySetupContext("copy_data_to_temp", 1);
 
   /* "View.MemoryView":1216
  *     cdef void *result
  * 
  *     cdef size_t itemsize = src.memview.view.itemsize             # <<<<<<<<<<<<<<
  *     cdef size_t size = slice_get_size(src, ndim)
  * 
@@ -16413,15 +16415,14 @@
   #endif
   __Pyx_AddTraceback("View.MemoryView.copy_data_to_temp", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   #ifdef WITH_THREAD
   __Pyx_PyGILState_Release(__pyx_gilstate_save);
   #endif
   __pyx_L0:;
-  __Pyx_RefNannyFinishContextNogil()
   return __pyx_r;
 }
 
 /* "View.MemoryView":1247
  * 
  * @cname('__pyx_memoryview_err_extents')
  * cdef int _err_extents(int i, Py_ssize_t extent1,             # <<<<<<<<<<<<<<
@@ -16633,22 +16634,20 @@
  * cdef int _err_no_memory() except -1 with gil:             # <<<<<<<<<<<<<<
  *     raise MemoryError
  * 
  */
 
 static int __pyx_memoryview_err_no_memory(void) {
   int __pyx_r;
-  __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   #ifdef WITH_THREAD
   PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
   #endif
-  __Pyx_RefNannySetupContext("_err_no_memory", 0);
 
   /* "View.MemoryView":1261
  * @cname('__pyx_memoryview_err_no_memory')
  * cdef int _err_no_memory() except -1 with gil:
  *     raise MemoryError             # <<<<<<<<<<<<<<
  * 
  * 
@@ -16663,15 +16662,14 @@
  * 
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_AddTraceback("View.MemoryView._err_no_memory", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
-  __Pyx_RefNannyFinishContext();
   #ifdef WITH_THREAD
   __Pyx_PyGILState_Release(__pyx_gilstate_save);
   #endif
   return __pyx_r;
 }
 
 /* "View.MemoryView":1265
@@ -16688,29 +16686,27 @@
   int __pyx_v_i;
   char __pyx_v_order;
   int __pyx_v_broadcasting;
   int __pyx_v_direct_copy;
   __Pyx_memviewslice __pyx_v_tmp;
   int __pyx_v_ndim;
   int __pyx_r;
-  __Pyx_RefNannyDeclarations
   Py_ssize_t __pyx_t_1;
   int __pyx_t_2;
   int __pyx_t_3;
   int __pyx_t_4;
   int __pyx_t_5;
   int __pyx_t_6;
   void *__pyx_t_7;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   #ifdef WITH_THREAD
   PyGILState_STATE __pyx_gilstate_save;
   #endif
-  __Pyx_RefNannySetupContext("memoryview_copy_contents", 1);
 
   /* "View.MemoryView":1273
  *     Check for overlapping memory and verify the shapes.
  *     """
  *     cdef void *tmpdata = NULL             # <<<<<<<<<<<<<<
  *     cdef size_t itemsize = src.memview.view.itemsize
  *     cdef int i
@@ -17247,15 +17243,14 @@
   #endif
   __Pyx_AddTraceback("View.MemoryView.memoryview_copy_contents", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   #ifdef WITH_THREAD
   __Pyx_PyGILState_Release(__pyx_gilstate_save);
   #endif
   __pyx_L0:;
-  __Pyx_RefNannyFinishContextNogil()
   return __pyx_r;
 }
 
 /* "View.MemoryView":1337
  * 
  * @cname('__pyx_memoryview_broadcast_leading')
  * cdef void broadcast_leading(__Pyx_memviewslice *mslice,             # <<<<<<<<<<<<<<
@@ -17421,19 +17416,17 @@
  * @cname('__pyx_memoryview_refcount_objects_in_slice_with_gil')
  * cdef void refcount_objects_in_slice_with_gil(char *data, Py_ssize_t *shape,             # <<<<<<<<<<<<<<
  *                                              Py_ssize_t *strides, int ndim,
  *                                              bint inc) noexcept with gil:
  */
 
 static void __pyx_memoryview_refcount_objects_in_slice_with_gil(char *__pyx_v_data, Py_ssize_t *__pyx_v_shape, Py_ssize_t *__pyx_v_strides, int __pyx_v_ndim, int __pyx_v_inc) {
-  __Pyx_RefNannyDeclarations
   #ifdef WITH_THREAD
   PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
   #endif
-  __Pyx_RefNannySetupContext("refcount_objects_in_slice_with_gil", 0);
 
   /* "View.MemoryView":1368
  *                                              Py_ssize_t *strides, int ndim,
  *                                              bint inc) noexcept with gil:
  *     refcount_objects_in_slice(data, shape, strides, ndim, inc)             # <<<<<<<<<<<<<<
  * 
  * @cname('__pyx_memoryview_refcount_objects_in_slice')
@@ -17445,15 +17438,14 @@
  * @cname('__pyx_memoryview_refcount_objects_in_slice_with_gil')
  * cdef void refcount_objects_in_slice_with_gil(char *data, Py_ssize_t *shape,             # <<<<<<<<<<<<<<
  *                                              Py_ssize_t *strides, int ndim,
  *                                              bint inc) noexcept with gil:
  */
 
   /* function exit code */
-  __Pyx_RefNannyFinishContext();
   #ifdef WITH_THREAD
   __Pyx_PyGILState_Release(__pyx_gilstate_save);
   #endif
 }
 
 /* "View.MemoryView":1371
  * 
@@ -17462,20 +17454,18 @@
  *                                     Py_ssize_t *strides, int ndim, bint inc) noexcept:
  *     cdef Py_ssize_t i
  */
 
 static void __pyx_memoryview_refcount_objects_in_slice(char *__pyx_v_data, Py_ssize_t *__pyx_v_shape, Py_ssize_t *__pyx_v_strides, int __pyx_v_ndim, int __pyx_v_inc) {
   CYTHON_UNUSED Py_ssize_t __pyx_v_i;
   Py_ssize_t __pyx_v_stride;
-  __Pyx_RefNannyDeclarations
   Py_ssize_t __pyx_t_1;
   Py_ssize_t __pyx_t_2;
   Py_ssize_t __pyx_t_3;
   int __pyx_t_4;
-  __Pyx_RefNannySetupContext("refcount_objects_in_slice", 0);
 
   /* "View.MemoryView":1374
  *                                     Py_ssize_t *strides, int ndim, bint inc) noexcept:
  *     cdef Py_ssize_t i
  *     cdef Py_ssize_t stride = strides[0]             # <<<<<<<<<<<<<<
  * 
  *     for i in range(shape[0]):
@@ -17581,15 +17571,14 @@
  * @cname('__pyx_memoryview_refcount_objects_in_slice')
  * cdef void refcount_objects_in_slice(char *data, Py_ssize_t *shape,             # <<<<<<<<<<<<<<
  *                                     Py_ssize_t *strides, int ndim, bint inc) noexcept:
  *     cdef Py_ssize_t i
  */
 
   /* function exit code */
-  __Pyx_RefNannyFinishContext();
 }
 
 /* "View.MemoryView":1391
  * 
  * @cname('__pyx_memoryview_slice_assign_scalar')
  * cdef void slice_assign_scalar(__Pyx_memviewslice *dst, int ndim,             # <<<<<<<<<<<<<<
  *                               size_t itemsize, void *item,
@@ -17803,16 +17792,15 @@
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__pyx_unpickle_Enum (wrapper)", 0);
   #if !CYTHON_METH_FASTCALL
   #if CYTHON_ASSUME_SAFE_MACROS
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
-  __pyx_nargs = PyTuple_Size(__pyx_args);
-  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(1, 1, __pyx_L3_error)
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   #endif
   __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   {
     PyObject **__pyx_pyargnames[] = {&__pyx_n_s_pyx_type,&__pyx_n_s_pyx_checksum,&__pyx_n_s_pyx_state,0};
     if (__pyx_kwds) {
       Py_ssize_t kw_args;
@@ -17867,18 +17855,19 @@
       values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
       values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
     }
     __pyx_v___pyx_type = values[0];
     __pyx_v___pyx_checksum = __Pyx_PyInt_As_long(values[1]); if (unlikely((__pyx_v___pyx_checksum == (long)-1) && PyErr_Occurred())) __PYX_ERR(1, 1, __pyx_L3_error)
     __pyx_v___pyx_state = values[2];
   }
-  goto __pyx_L4_argument_unpacking_done;
+  goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("__pyx_unpickle_Enum", 1, 3, 3, __pyx_nargs); __PYX_ERR(1, 1, __pyx_L3_error)
-  goto __pyx_L3_error;
+  __pyx_L6_skip:;
+  goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
@@ -17908,15 +17897,15 @@
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_t_5;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__pyx_unpickle_Enum", 0);
+  __Pyx_RefNannySetupContext("__pyx_unpickle_Enum", 1);
 
   /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  *     if __pyx_checksum not in (0x82a3537, 0x6ae9995, 0xb068931):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError, "Incompatible checksums (0x%x vs (0x82a3537, 0x6ae9995, 0xb068931) = (name))" % __pyx_checksum
@@ -18090,15 +18079,15 @@
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   int __pyx_t_8;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__pyx_unpickle_Enum__set_state", 0);
+  __Pyx_RefNannySetupContext("__pyx_unpickle_Enum__set_state", 1);
 
   /* "(tree fragment)":12
  *     return __pyx_result
  * cdef __pyx_unpickle_Enum__set_state(Enum __pyx_result, tuple __pyx_state):
  *     __pyx_result.name = __pyx_state[0]             # <<<<<<<<<<<<<<
  *     if len(__pyx_state) > 1 and hasattr(__pyx_result, '__dict__'):
  *         __pyx_result.__dict__.update(__pyx_state[1])
@@ -18206,292 +18195,292 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-b2_49hlm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":246
+/* "../../../tmp/build-env-wicvywyh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":246
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_7ndarray_4base_base(PyArrayObject *__pyx_v_self) {
   PyObject *__pyx_r;
 
-  /* "../../../tmp/build-env-b2_49hlm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":249
+  /* "../../../tmp/build-env-wicvywyh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":249
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  *             return PyArray_BASE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_BASE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-b2_49hlm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":246
+  /* "../../../tmp/build-env-wicvywyh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":246
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-b2_49hlm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":252
+/* "../../../tmp/build-env-wicvywyh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":252
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
 static CYTHON_INLINE PyArray_Descr *__pyx_f_5numpy_7ndarray_5descr_descr(PyArrayObject *__pyx_v_self) {
   PyArray_Descr *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyArray_Descr *__pyx_t_1;
-  __Pyx_RefNannySetupContext("descr", 0);
+  __Pyx_RefNannySetupContext("descr", 1);
 
-  /* "../../../tmp/build-env-b2_49hlm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":255
+  /* "../../../tmp/build-env-wicvywyh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":255
  *             """Returns an owned reference to the dtype of the array.
  *             """
  *             return <dtype>PyArray_DESCR(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __Pyx_XDECREF((PyObject *)__pyx_r);
   __pyx_t_1 = PyArray_DESCR(__pyx_v_self);
   __Pyx_INCREF((PyObject *)((PyArray_Descr *)__pyx_t_1));
   __pyx_r = ((PyArray_Descr *)__pyx_t_1);
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-b2_49hlm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":252
+  /* "../../../tmp/build-env-wicvywyh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":252
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-b2_49hlm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":258
+/* "../../../tmp/build-env-wicvywyh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":258
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_7ndarray_4ndim_ndim(PyArrayObject *__pyx_v_self) {
   int __pyx_r;
 
-  /* "../../../tmp/build-env-b2_49hlm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":261
+  /* "../../../tmp/build-env-wicvywyh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":261
  *             """Returns the number of dimensions in the array.
  *             """
  *             return PyArray_NDIM(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_NDIM(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-b2_49hlm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":258
+  /* "../../../tmp/build-env-wicvywyh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":258
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-b2_49hlm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":264
+/* "../../../tmp/build-env-wicvywyh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":264
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_5shape_shape(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../tmp/build-env-b2_49hlm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":269
+  /* "../../../tmp/build-env-wicvywyh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":269
  *             Can return NULL for 0-dimensional arrays.
  *             """
  *             return PyArray_DIMS(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_DIMS(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-b2_49hlm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":264
+  /* "../../../tmp/build-env-wicvywyh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":264
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-b2_49hlm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":272
+/* "../../../tmp/build-env-wicvywyh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":272
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_7strides_strides(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../tmp/build-env-b2_49hlm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":276
+  /* "../../../tmp/build-env-wicvywyh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":276
  *             The number of elements matches the number of dimensions of the array (ndim).
  *             """
  *             return PyArray_STRIDES(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_STRIDES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-b2_49hlm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":272
+  /* "../../../tmp/build-env-wicvywyh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":272
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-b2_49hlm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":279
+/* "../../../tmp/build-env-wicvywyh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":279
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
 static CYTHON_INLINE npy_intp __pyx_f_5numpy_7ndarray_4size_size(PyArrayObject *__pyx_v_self) {
   npy_intp __pyx_r;
 
-  /* "../../../tmp/build-env-b2_49hlm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":282
+  /* "../../../tmp/build-env-wicvywyh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":282
  *             """Returns the total size (in number of elements) of the array.
  *             """
  *             return PyArray_SIZE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_SIZE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-b2_49hlm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":279
+  /* "../../../tmp/build-env-wicvywyh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":279
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-b2_49hlm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":285
+/* "../../../tmp/build-env-wicvywyh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":285
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
 static CYTHON_INLINE char *__pyx_f_5numpy_7ndarray_4data_data(PyArrayObject *__pyx_v_self) {
   char *__pyx_r;
 
-  /* "../../../tmp/build-env-b2_49hlm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":291
+  /* "../../../tmp/build-env-wicvywyh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":291
  *             of `PyArray_DATA()` instead, which returns a 'void*'.
  *             """
  *             return PyArray_BYTES(self)             # <<<<<<<<<<<<<<
  * 
  *     ctypedef unsigned char      npy_bool
  */
   __pyx_r = PyArray_BYTES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-b2_49hlm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":285
+  /* "../../../tmp/build-env-wicvywyh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":285
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-b2_49hlm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":777
+/* "../../../tmp/build-env-wicvywyh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":777
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyArray_MultiIterNew1(PyObject *__pyx_v_a) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
+  __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 1);
 
-  /* "../../../tmp/build-env-b2_49hlm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":778
+  /* "../../../tmp/build-env-wicvywyh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":778
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 778, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-b2_49hlm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":777
+  /* "../../../tmp/build-env-wicvywyh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":777
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -18502,46 +18491,46 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-b2_49hlm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":780
+/* "../../../tmp/build-env-wicvywyh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":780
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyArray_MultiIterNew2(PyObject *__pyx_v_a, PyObject *__pyx_v_b) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
+  __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 1);
 
-  /* "../../../tmp/build-env-b2_49hlm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":781
+  /* "../../../tmp/build-env-wicvywyh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":781
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 781, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-b2_49hlm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":780
+  /* "../../../tmp/build-env-wicvywyh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":780
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -18552,46 +18541,46 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-b2_49hlm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":783
+/* "../../../tmp/build-env-wicvywyh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":783
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyArray_MultiIterNew3(PyObject *__pyx_v_a, PyObject *__pyx_v_b, PyObject *__pyx_v_c) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
+  __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 1);
 
-  /* "../../../tmp/build-env-b2_49hlm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":784
+  /* "../../../tmp/build-env-wicvywyh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":784
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 784, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-b2_49hlm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":783
+  /* "../../../tmp/build-env-wicvywyh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":783
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -18602,46 +18591,46 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-b2_49hlm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":786
+/* "../../../tmp/build-env-wicvywyh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":786
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyArray_MultiIterNew4(PyObject *__pyx_v_a, PyObject *__pyx_v_b, PyObject *__pyx_v_c, PyObject *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
+  __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 1);
 
-  /* "../../../tmp/build-env-b2_49hlm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":787
+  /* "../../../tmp/build-env-wicvywyh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":787
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 787, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-b2_49hlm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":786
+  /* "../../../tmp/build-env-wicvywyh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":786
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -18652,46 +18641,46 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-b2_49hlm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":789
+/* "../../../tmp/build-env-wicvywyh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":789
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyArray_MultiIterNew5(PyObject *__pyx_v_a, PyObject *__pyx_v_b, PyObject *__pyx_v_c, PyObject *__pyx_v_d, PyObject *__pyx_v_e) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
+  __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 1);
 
-  /* "../../../tmp/build-env-b2_49hlm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":790
+  /* "../../../tmp/build-env-wicvywyh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":790
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 790, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-b2_49hlm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":789
+  /* "../../../tmp/build-env-wicvywyh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":789
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -18702,212 +18691,209 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-b2_49hlm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":792
+/* "../../../tmp/build-env-wicvywyh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":792
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
-  __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
+  __Pyx_RefNannySetupContext("PyDataType_SHAPE", 1);
 
-  /* "../../../tmp/build-env-b2_49hlm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":793
+  /* "../../../tmp/build-env-wicvywyh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":793
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = PyDataType_HASSUBARRAY(__pyx_v_d);
   if (__pyx_t_1) {
 
-    /* "../../../tmp/build-env-b2_49hlm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":794
+    /* "../../../tmp/build-env-wicvywyh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":794
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../tmp/build-env-b2_49hlm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":793
+    /* "../../../tmp/build-env-wicvywyh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":793
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../tmp/build-env-b2_49hlm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":796
+  /* "../../../tmp/build-env-wicvywyh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":796
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../tmp/build-env-b2_49hlm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":792
+  /* "../../../tmp/build-env-wicvywyh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":792
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-b2_49hlm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":971
+/* "../../../tmp/build-env-wicvywyh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":971
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../../tmp/build-env-b2_49hlm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":972
+  /* "../../../tmp/build-env-wicvywyh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":972
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../tmp/build-env-b2_49hlm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":973
+  /* "../../../tmp/build-env-wicvywyh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":973
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
 
-  /* "../../../tmp/build-env-b2_49hlm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":971
+  /* "../../../tmp/build-env-wicvywyh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":971
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
-  __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../tmp/build-env-b2_49hlm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":975
+/* "../../../tmp/build-env-wicvywyh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":975
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
-  __Pyx_RefNannySetupContext("get_array_base", 0);
+  __Pyx_RefNannySetupContext("get_array_base", 1);
 
-  /* "../../../tmp/build-env-b2_49hlm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":976
+  /* "../../../tmp/build-env-wicvywyh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":976
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../tmp/build-env-b2_49hlm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":977
+  /* "../../../tmp/build-env-wicvywyh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":977
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = (__pyx_v_base == NULL);
   if (__pyx_t_1) {
 
-    /* "../../../tmp/build-env-b2_49hlm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":978
+    /* "../../../tmp/build-env-wicvywyh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":978
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../tmp/build-env-b2_49hlm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":977
+    /* "../../../tmp/build-env-wicvywyh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":977
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../tmp/build-env-b2_49hlm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":979
+  /* "../../../tmp/build-env-wicvywyh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":979
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-b2_49hlm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":975
+  /* "../../../tmp/build-env-wicvywyh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":975
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-b2_49hlm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":983
+/* "../../../tmp/build-env-wicvywyh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":983
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -18921,17 +18907,17 @@
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("import_array", 0);
+  __Pyx_RefNannySetupContext("import_array", 1);
 
-  /* "../../../tmp/build-env-b2_49hlm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":984
+  /* "../../../tmp/build-env-wicvywyh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":984
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -18939,68 +18925,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../tmp/build-env-b2_49hlm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":985
+      /* "../../../tmp/build-env-wicvywyh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":985
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 985, __pyx_L3_error)
 
-      /* "../../../tmp/build-env-b2_49hlm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":984
+      /* "../../../tmp/build-env-wicvywyh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":984
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../tmp/build-env-b2_49hlm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":986
+    /* "../../../tmp/build-env-wicvywyh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":986
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 986, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../tmp/build-env-b2_49hlm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":987
+      /* "../../../tmp/build-env-wicvywyh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":987
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 987, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 987, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../tmp/build-env-b2_49hlm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":984
+    /* "../../../tmp/build-env-wicvywyh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":984
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -19008,15 +18994,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../tmp/build-env-b2_49hlm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":983
+  /* "../../../tmp/build-env-wicvywyh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":983
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -19031,15 +19017,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-b2_49hlm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":989
+/* "../../../tmp/build-env-wicvywyh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":989
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -19053,17 +19039,17 @@
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("import_umath", 0);
+  __Pyx_RefNannySetupContext("import_umath", 1);
 
-  /* "../../../tmp/build-env-b2_49hlm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":990
+  /* "../../../tmp/build-env-wicvywyh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":990
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -19071,68 +19057,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../tmp/build-env-b2_49hlm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":991
+      /* "../../../tmp/build-env-wicvywyh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":991
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 991, __pyx_L3_error)
 
-      /* "../../../tmp/build-env-b2_49hlm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":990
+      /* "../../../tmp/build-env-wicvywyh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":990
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../tmp/build-env-b2_49hlm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":992
+    /* "../../../tmp/build-env-wicvywyh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":992
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 992, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../tmp/build-env-b2_49hlm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":993
+      /* "../../../tmp/build-env-wicvywyh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":993
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 993, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 993, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../tmp/build-env-b2_49hlm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":990
+    /* "../../../tmp/build-env-wicvywyh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":990
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -19140,15 +19126,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../tmp/build-env-b2_49hlm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":989
+  /* "../../../tmp/build-env-wicvywyh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":989
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -19163,15 +19149,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-b2_49hlm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":995
+/* "../../../tmp/build-env-wicvywyh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":995
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -19185,17 +19171,17 @@
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("import_ufunc", 0);
+  __Pyx_RefNannySetupContext("import_ufunc", 1);
 
-  /* "../../../tmp/build-env-b2_49hlm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":996
+  /* "../../../tmp/build-env-wicvywyh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":996
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -19203,68 +19189,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../tmp/build-env-b2_49hlm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":997
+      /* "../../../tmp/build-env-wicvywyh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":997
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 997, __pyx_L3_error)
 
-      /* "../../../tmp/build-env-b2_49hlm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":996
+      /* "../../../tmp/build-env-wicvywyh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":996
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../tmp/build-env-b2_49hlm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":998
+    /* "../../../tmp/build-env-wicvywyh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":998
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 998, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../tmp/build-env-b2_49hlm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":999
+      /* "../../../tmp/build-env-wicvywyh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":999
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * 
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 999, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 999, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../tmp/build-env-b2_49hlm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":996
+    /* "../../../tmp/build-env-wicvywyh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":996
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -19272,15 +19258,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../tmp/build-env-b2_49hlm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":995
+  /* "../../../tmp/build-env-wicvywyh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":995
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -19295,176 +19281,170 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-b2_49hlm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1002
+/* "../../../tmp/build-env-wicvywyh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1002
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../../tmp/build-env-b2_49hlm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1014
+  /* "../../../tmp/build-env-wicvywyh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1014
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-b2_49hlm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1002
+  /* "../../../tmp/build-env-wicvywyh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1002
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-b2_49hlm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1017
+/* "../../../tmp/build-env-wicvywyh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1017
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../../tmp/build-env-b2_49hlm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1029
+  /* "../../../tmp/build-env-wicvywyh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1029
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-b2_49hlm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1017
+  /* "../../../tmp/build-env-wicvywyh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1017
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-b2_49hlm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1032
+/* "../../../tmp/build-env-wicvywyh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1032
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../tmp/build-env-b2_49hlm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1039
+  /* "../../../tmp/build-env-wicvywyh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1039
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-b2_49hlm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1032
+  /* "../../../tmp/build-env-wicvywyh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1032
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-b2_49hlm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1042
+/* "../../../tmp/build-env-wicvywyh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1042
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../tmp/build-env-b2_49hlm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1046
+  /* "../../../tmp/build-env-wicvywyh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1046
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-b2_49hlm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1042
+  /* "../../../tmp/build-env-wicvywyh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1042
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../tmp/build-env-b2_49hlm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1049
+/* "../../../tmp/build-env-wicvywyh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1049
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../tmp/build-env-b2_49hlm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1053
+  /* "../../../tmp/build-env-wicvywyh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1053
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../tmp/build-env-b2_49hlm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1049
+  /* "../../../tmp/build-env-wicvywyh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1049
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -19483,19 +19463,17 @@
 
 static void __pyx_fuse_0__pyx_f_12linearmodels_5panel_8_utility__remove_node(__pyx_t_5numpy_int8_t __pyx_v_node, __Pyx_memviewslice __pyx_v_meta, __Pyx_memviewslice __pyx_v_orig_dest, __pyx_t_5numpy_int8_t *__pyx_v_next_node, __pyx_t_5numpy_int8_t *__pyx_v_next_count) {
   __pyx_t_5numpy_int8_t __pyx_v_next_offset;
   __pyx_t_5numpy_int8_t __pyx_v_orig;
   __pyx_t_5numpy_int8_t __pyx_v_reverse_offset;
   __pyx_t_5numpy_int8_t __pyx_v_reverse_node;
   CYTHON_UNUSED __pyx_t_5numpy_int8_t __pyx_v__next_orig;
-  __Pyx_RefNannyDeclarations
   Py_ssize_t __pyx_t_1;
   Py_ssize_t __pyx_t_2;
   int __pyx_t_3;
-  __Pyx_RefNannySetupContext("__pyx_fuse_0_remove_node", 0);
 
   /* "linearmodels/panel/_utility.pyx":47
  *     cdef any_int next_offset, orig, reverse_offset, reverse_node, _next_orig
  *     # 3. Decrement
  *     meta[node, 1] -= 1             # <<<<<<<<<<<<<<
  *     # 1. Remove forewrd link
  *     next_offset = meta[node, 2]
@@ -19683,28 +19661,25 @@
  * 
  * cdef void _remove_node(             # <<<<<<<<<<<<<<
  *         any_int node,
  *         any_int[:, ::1] meta,
  */
 
   /* function exit code */
-  __Pyx_RefNannyFinishContext();
 }
 
 static void __pyx_fuse_1__pyx_f_12linearmodels_5panel_8_utility__remove_node(__pyx_t_5numpy_int16_t __pyx_v_node, __Pyx_memviewslice __pyx_v_meta, __Pyx_memviewslice __pyx_v_orig_dest, __pyx_t_5numpy_int16_t *__pyx_v_next_node, __pyx_t_5numpy_int16_t *__pyx_v_next_count) {
   __pyx_t_5numpy_int16_t __pyx_v_next_offset;
   __pyx_t_5numpy_int16_t __pyx_v_orig;
   __pyx_t_5numpy_int16_t __pyx_v_reverse_offset;
   __pyx_t_5numpy_int16_t __pyx_v_reverse_node;
   CYTHON_UNUSED __pyx_t_5numpy_int16_t __pyx_v__next_orig;
-  __Pyx_RefNannyDeclarations
   Py_ssize_t __pyx_t_1;
   Py_ssize_t __pyx_t_2;
   int __pyx_t_3;
-  __Pyx_RefNannySetupContext("__pyx_fuse_1_remove_node", 0);
 
   /* "linearmodels/panel/_utility.pyx":47
  *     cdef any_int next_offset, orig, reverse_offset, reverse_node, _next_orig
  *     # 3. Decrement
  *     meta[node, 1] -= 1             # <<<<<<<<<<<<<<
  *     # 1. Remove forewrd link
  *     next_offset = meta[node, 2]
@@ -19892,28 +19867,25 @@
  * 
  * cdef void _remove_node(             # <<<<<<<<<<<<<<
  *         any_int node,
  *         any_int[:, ::1] meta,
  */
 
   /* function exit code */
-  __Pyx_RefNannyFinishContext();
 }
 
 static void __pyx_fuse_2__pyx_f_12linearmodels_5panel_8_utility__remove_node(__pyx_t_5numpy_int32_t __pyx_v_node, __Pyx_memviewslice __pyx_v_meta, __Pyx_memviewslice __pyx_v_orig_dest, __pyx_t_5numpy_int32_t *__pyx_v_next_node, __pyx_t_5numpy_int32_t *__pyx_v_next_count) {
   __pyx_t_5numpy_int32_t __pyx_v_next_offset;
   __pyx_t_5numpy_int32_t __pyx_v_orig;
   __pyx_t_5numpy_int32_t __pyx_v_reverse_offset;
   __pyx_t_5numpy_int32_t __pyx_v_reverse_node;
   CYTHON_UNUSED __pyx_t_5numpy_int32_t __pyx_v__next_orig;
-  __Pyx_RefNannyDeclarations
   Py_ssize_t __pyx_t_1;
   Py_ssize_t __pyx_t_2;
   int __pyx_t_3;
-  __Pyx_RefNannySetupContext("__pyx_fuse_2_remove_node", 0);
 
   /* "linearmodels/panel/_utility.pyx":47
  *     cdef any_int next_offset, orig, reverse_offset, reverse_node, _next_orig
  *     # 3. Decrement
  *     meta[node, 1] -= 1             # <<<<<<<<<<<<<<
  *     # 1. Remove forewrd link
  *     next_offset = meta[node, 2]
@@ -20101,28 +20073,25 @@
  * 
  * cdef void _remove_node(             # <<<<<<<<<<<<<<
  *         any_int node,
  *         any_int[:, ::1] meta,
  */
 
   /* function exit code */
-  __Pyx_RefNannyFinishContext();
 }
 
 static void __pyx_fuse_3__pyx_f_12linearmodels_5panel_8_utility__remove_node(__pyx_t_5numpy_int64_t __pyx_v_node, __Pyx_memviewslice __pyx_v_meta, __Pyx_memviewslice __pyx_v_orig_dest, __pyx_t_5numpy_int64_t *__pyx_v_next_node, __pyx_t_5numpy_int64_t *__pyx_v_next_count) {
   __pyx_t_5numpy_int64_t __pyx_v_next_offset;
   __pyx_t_5numpy_int64_t __pyx_v_orig;
   __pyx_t_5numpy_int64_t __pyx_v_reverse_offset;
   __pyx_t_5numpy_int64_t __pyx_v_reverse_node;
   CYTHON_UNUSED __pyx_t_5numpy_int64_t __pyx_v__next_orig;
-  __Pyx_RefNannyDeclarations
   __pyx_t_5numpy_int64_t __pyx_t_1;
   Py_ssize_t __pyx_t_2;
   int __pyx_t_3;
-  __Pyx_RefNannySetupContext("__pyx_fuse_3_remove_node", 0);
 
   /* "linearmodels/panel/_utility.pyx":47
  *     cdef any_int next_offset, orig, reverse_offset, reverse_node, _next_orig
  *     # 3. Decrement
  *     meta[node, 1] -= 1             # <<<<<<<<<<<<<<
  *     # 1. Remove forewrd link
  *     next_offset = meta[node, 2]
@@ -20310,15 +20279,14 @@
  * 
  * cdef void _remove_node(             # <<<<<<<<<<<<<<
  *         any_int node,
  *         any_int[:, ::1] meta,
  */
 
   /* function exit code */
-  __Pyx_RefNannyFinishContext();
 }
 
 /* "linearmodels/panel/_utility.pyx":74
  * 
  * 
  * def _drop_singletons(any_int[:, ::1] meta, any_int[:, ::1] orig_dest):             # <<<<<<<<<<<<<<
  *     """
@@ -20343,16 +20311,15 @@
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__pyx_fused_cpdef (wrapper)", 0);
   #if CYTHON_ASSUME_SAFE_MACROS
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
-  __pyx_nargs = PyTuple_Size(__pyx_args);
-  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(0, 74, __pyx_L3_error)
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   __pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
   {
     PyObject **__pyx_pyargnames[] = {&__pyx_n_s_signatures,&__pyx_n_s_args,&__pyx_n_s_kwargs,&__pyx_n_s_defaults,&__pyx_n_s_fused_sigindex,0};
     __pyx_defaults *__pyx_dynamic_args = __Pyx_CyFunction_Defaults(__pyx_defaults, __pyx_self);
     values[4] = __Pyx_Arg_NewRef_VARARGS(__pyx_dynamic_args->__pyx_arg__fused_sigindex);
     if (__pyx_kwds) {
@@ -20436,18 +20403,19 @@
     }
     __pyx_v_signatures = values[0];
     __pyx_v_args = values[1];
     __pyx_v_kwargs = values[2];
     __pyx_v_defaults = values[3];
     __pyx_v__fused_sigindex = values[4];
   }
-  goto __pyx_L4_argument_unpacking_done;
+  goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("__pyx_fused_cpdef", 0, 4, 5, __pyx_nargs); __PYX_ERR(0, 74, __pyx_L3_error)
-  goto __pyx_L3_error;
+  __pyx_L6_skip:;
+  goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_VARARGS(values[__pyx_temp]);
     }
   }
@@ -20466,23 +20434,22 @@
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_12linearmodels_5panel_8_utility__drop_singletons(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_signatures, PyObject *__pyx_v_args, PyObject *__pyx_v_kwargs, CYTHON_UNUSED PyObject *__pyx_v_defaults, PyObject *__pyx_v__fused_sigindex) {
   PyObject *__pyx_v_search_list = 0;
-  PyObject *__pyx_v_sn = 0;
   PyObject *__pyx_v_sigindex_node = 0;
   PyObject *__pyx_v_dest_sig = NULL;
   PyTypeObject *__pyx_v_ndarray = 0;
   PyObject *__pyx_v_arg_as_memoryview = 0;
   __Pyx_memviewslice __pyx_v_memslice;
   Py_ssize_t __pyx_v_itemsize;
   int __pyx_v_dtype_signed;
-  char __pyx_v_kind;
+  Py_UCS4 __pyx_v_kind;
   int __pyx_v____pyx_int8_t_is_signed;
   int __pyx_v____pyx_int16_t_is_signed;
   int __pyx_v____pyx_int32_t_is_signed;
   int __pyx_v____pyx_int64_t_is_signed;
   PyObject *__pyx_v_arg = NULL;
   PyObject *__pyx_v_dtype = NULL;
   PyObject *__pyx_v_arg_base = NULL;
@@ -20491,14 +20458,16 @@
   PyObject *__pyx_v_last_type = NULL;
   PyObject *__pyx_v_sig_type = NULL;
   PyObject *__pyx_v_sigindex_matches = NULL;
   PyObject *__pyx_v_sigindex_candidates = NULL;
   PyObject *__pyx_v_dst_type = NULL;
   PyObject *__pyx_v_found_matches = NULL;
   PyObject *__pyx_v_found_candidates = NULL;
+  PyObject *__pyx_v_sn = NULL;
+  PyObject *__pyx_v_type_match = NULL;
   PyObject *__pyx_v_candidates = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
   int __pyx_t_3;
   int __pyx_t_4;
@@ -20669,18 +20638,18 @@
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
         __pyx_v_itemsize = __pyx_t_5;
         __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_dtype, __pyx_n_s_kind); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 74, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_6);
         __pyx_t_7 = __Pyx_PyObject_Ord(__pyx_t_6); if (unlikely(__pyx_t_7 == ((long)(long)(Py_UCS4)-1))) __PYX_ERR(0, 74, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
         __pyx_v_kind = __pyx_t_7;
-        __pyx_v_dtype_signed = (__pyx_v_kind == 'i');
+        __pyx_v_dtype_signed = (__pyx_v_kind == 0x69);
         switch (__pyx_v_kind) {
-          case 'i':
-          case 'u':
+          case 0x69:
+          case 0x75:
           __pyx_t_4 = ((sizeof(__pyx_t_5numpy_int8_t)) == __pyx_v_itemsize);
           if (__pyx_t_4) {
           } else {
             __pyx_t_2 = __pyx_t_4;
             goto __pyx_L16_bool_binop_done;
           }
           __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_arg, __pyx_n_s_ndim); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 74, __pyx_L1_error)
@@ -20766,19 +20735,19 @@
           __pyx_t_2 = __pyx_t_4;
           __pyx_L28_bool_binop_done:;
           if (__pyx_t_2) {
             if (unlikely((__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_int64_t, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0))) __PYX_ERR(0, 74, __pyx_L1_error)
             goto __pyx_L10_break;
           }
           break;
-          case 'f':
+          case 0x66:
           break;
-          case 'c':
+          case 99:
           break;
-          case 'O':
+          case 79:
           break;
           default: break;
         }
       }
     }
     __pyx_t_2 = (__pyx_v_arg == Py_None);
     if (__pyx_t_2) {
@@ -21003,15 +20972,14 @@
     while (1) {
       __pyx_t_15 = __Pyx_dict_iter_next(__pyx_t_13, __pyx_t_14, &__pyx_t_5, &__pyx_t_1, NULL, NULL, __pyx_t_11);
       if (unlikely(__pyx_t_15 == 0)) break;
       if (unlikely(__pyx_t_15 == -1)) __PYX_ERR(0, 74, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_XDECREF_SET(__pyx_v_sig, __pyx_t_1);
       __pyx_t_1 = 0;
-      if (!(likely(PyDict_CheckExact(__pyx_v__fused_sigindex))||((__pyx_v__fused_sigindex) == Py_None) || __Pyx_RaiseUnexpectedTypeError("dict", __pyx_v__fused_sigindex))) __PYX_ERR(0, 74, __pyx_L1_error)
       __pyx_t_1 = __pyx_v__fused_sigindex;
       __Pyx_INCREF(__pyx_t_1);
       __Pyx_XDECREF_SET(__pyx_v_sigindex_node, ((PyObject*)__pyx_t_1));
       __pyx_t_1 = 0;
       __pyx_t_16 = __Pyx_PyObject_GetAttrStr(__pyx_v_sig, __pyx_n_s_strip); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 74, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_16);
       __pyx_t_17 = NULL;
@@ -21083,21 +21051,28 @@
       #else
       CYTHON_UNUSED_VAR(__pyx_t_17);
       #endif
       __Pyx_XDECREF_SET(__pyx_v_sig_series, ((PyObject*)__pyx_t_16));
       __pyx_t_16 = 0;
       __Pyx_XDECREF_SET(__pyx_v_last_type, __pyx_t_6);
       __pyx_t_6 = 0;
-      __pyx_t_1 = __pyx_v_sig_series; __Pyx_INCREF(__pyx_t_1); __pyx_t_18 = 0;
+      __pyx_t_1 = __pyx_v_sig_series; __Pyx_INCREF(__pyx_t_1);
+      __pyx_t_18 = 0;
       for (;;) {
-        if (__pyx_t_18 >= PyList_GET_SIZE(__pyx_t_1)) break;
+        {
+          Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_1);
+          #if !CYTHON_ASSUME_SAFE_MACROS
+          if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 74, __pyx_L1_error)
+          #endif
+          if (__pyx_t_18 >= __pyx_temp) break;
+        }
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
         __pyx_t_6 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_18); __Pyx_INCREF(__pyx_t_6); __pyx_t_18++; if (unlikely((0 < 0))) __PYX_ERR(0, 74, __pyx_L1_error)
         #else
-        __pyx_t_6 = PySequence_ITEM(__pyx_t_1, __pyx_t_18); __pyx_t_18++; if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 74, __pyx_L1_error)
+        __pyx_t_6 = __Pyx_PySequence_ITEM(__pyx_t_1, __pyx_t_18); __pyx_t_18++; if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 74, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_6);
         #endif
         __Pyx_XDECREF_SET(__pyx_v_sig_type, __pyx_t_6);
         __pyx_t_6 = 0;
         if (unlikely(__pyx_v_sigindex_node == Py_None)) {
           PyErr_SetString(PyExc_TypeError, "'NoneType' object is not iterable");
           __PYX_ERR(0, 74, __pyx_L1_error)
@@ -21119,17 +21094,19 @@
         /*else*/ {
           if (unlikely(__pyx_v_sigindex_node == Py_None)) {
             PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
             __PYX_ERR(0, 74, __pyx_L1_error)
           }
           __pyx_t_6 = __Pyx_PyDict_GetItem(__pyx_v_sigindex_node, __pyx_v_sig_type); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 74, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_6);
-          if (!(likely(PyDict_CheckExact(__pyx_t_6))||((__pyx_t_6) == Py_None) || __Pyx_RaiseUnexpectedTypeError("dict", __pyx_t_6))) __PYX_ERR(0, 74, __pyx_L1_error)
-          __Pyx_DECREF_SET(__pyx_v_sigindex_node, ((PyObject*)__pyx_t_6));
-          __pyx_t_6 = 0;
+          __pyx_t_16 = __pyx_t_6;
+          __Pyx_INCREF(__pyx_t_16);
+          __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+          __Pyx_DECREF_SET(__pyx_v_sigindex_node, ((PyObject*)__pyx_t_16));
+          __pyx_t_16 = 0;
         }
         __pyx_L71:;
       }
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       if (unlikely(__pyx_v_sigindex_node == Py_None)) {
         PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
         __PYX_ERR(0, 74, __pyx_L1_error)
@@ -21145,137 +21122,160 @@
   __pyx_t_13 = PyList_New(1); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 74, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_13);
   __Pyx_INCREF(__pyx_v__fused_sigindex);
   __Pyx_GIVEREF(__pyx_v__fused_sigindex);
   if (__Pyx_PyList_SET_ITEM(__pyx_t_13, 0, __pyx_v__fused_sigindex)) __PYX_ERR(0, 74, __pyx_L1_error);
   __pyx_v_sigindex_candidates = ((PyObject*)__pyx_t_13);
   __pyx_t_13 = 0;
-  __pyx_t_13 = __pyx_v_dest_sig; __Pyx_INCREF(__pyx_t_13); __pyx_t_14 = 0;
+  __pyx_t_13 = __pyx_v_dest_sig; __Pyx_INCREF(__pyx_t_13);
+  __pyx_t_14 = 0;
   for (;;) {
-    if (__pyx_t_14 >= PyList_GET_SIZE(__pyx_t_13)) break;
+    {
+      Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_13);
+      #if !CYTHON_ASSUME_SAFE_MACROS
+      if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 74, __pyx_L1_error)
+      #endif
+      if (__pyx_t_14 >= __pyx_temp) break;
+    }
     #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
     __pyx_t_1 = PyList_GET_ITEM(__pyx_t_13, __pyx_t_14); __Pyx_INCREF(__pyx_t_1); __pyx_t_14++; if (unlikely((0 < 0))) __PYX_ERR(0, 74, __pyx_L1_error)
     #else
-    __pyx_t_1 = PySequence_ITEM(__pyx_t_13, __pyx_t_14); __pyx_t_14++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 74, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PySequence_ITEM(__pyx_t_13, __pyx_t_14); __pyx_t_14++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 74, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     #endif
     __Pyx_XDECREF_SET(__pyx_v_dst_type, __pyx_t_1);
     __pyx_t_1 = 0;
     __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 74, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_XDECREF_SET(__pyx_v_found_matches, ((PyObject*)__pyx_t_1));
     __pyx_t_1 = 0;
     __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 74, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_XDECREF_SET(__pyx_v_found_candidates, ((PyObject*)__pyx_t_1));
     __pyx_t_1 = 0;
     __pyx_t_4 = (__pyx_v_dst_type == Py_None);
     if (__pyx_t_4) {
-      __pyx_t_1 = __pyx_v_sigindex_matches; __Pyx_INCREF(__pyx_t_1); __pyx_t_5 = 0;
+      __pyx_t_1 = __pyx_v_sigindex_matches; __Pyx_INCREF(__pyx_t_1);
+      __pyx_t_5 = 0;
       for (;;) {
-        if (__pyx_t_5 >= PyList_GET_SIZE(__pyx_t_1)) break;
+        {
+          Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_1);
+          #if !CYTHON_ASSUME_SAFE_MACROS
+          if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 74, __pyx_L1_error)
+          #endif
+          if (__pyx_t_5 >= __pyx_temp) break;
+        }
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_6 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_5); __Pyx_INCREF(__pyx_t_6); __pyx_t_5++; if (unlikely((0 < 0))) __PYX_ERR(0, 74, __pyx_L1_error)
+        __pyx_t_16 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_5); __Pyx_INCREF(__pyx_t_16); __pyx_t_5++; if (unlikely((0 < 0))) __PYX_ERR(0, 74, __pyx_L1_error)
         #else
-        __pyx_t_6 = PySequence_ITEM(__pyx_t_1, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 74, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_6);
+        __pyx_t_16 = __Pyx_PySequence_ITEM(__pyx_t_1, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 74, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_16);
         #endif
-        if (!(likely(PyDict_CheckExact(__pyx_t_6))||((__pyx_t_6) == Py_None) || __Pyx_RaiseUnexpectedTypeError("dict", __pyx_t_6))) __PYX_ERR(0, 74, __pyx_L1_error)
-        __Pyx_XDECREF_SET(__pyx_v_sn, ((PyObject*)__pyx_t_6));
-        __pyx_t_6 = 0;
+        __Pyx_XDECREF_SET(__pyx_v_sn, __pyx_t_16);
+        __pyx_t_16 = 0;
         if (unlikely(__pyx_v_sn == Py_None)) {
           PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "values");
           __PYX_ERR(0, 74, __pyx_L1_error)
         }
-        __pyx_t_6 = __Pyx_PyDict_Values(__pyx_v_sn); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 74, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_6);
-        __pyx_t_19 = __Pyx_PyList_Extend(__pyx_v_found_matches, __pyx_t_6); if (unlikely(__pyx_t_19 == ((int)-1))) __PYX_ERR(0, 74, __pyx_L1_error)
-        __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+        __pyx_t_16 = __Pyx_PyDict_Values(((PyObject*)__pyx_v_sn)); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 74, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_16);
+        __pyx_t_19 = __Pyx_PyList_Extend(__pyx_v_found_matches, __pyx_t_16); if (unlikely(__pyx_t_19 == ((int)-1))) __PYX_ERR(0, 74, __pyx_L1_error)
+        __Pyx_DECREF(__pyx_t_16); __pyx_t_16 = 0;
       }
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-      __pyx_t_1 = __pyx_v_sigindex_candidates; __Pyx_INCREF(__pyx_t_1); __pyx_t_5 = 0;
+      __pyx_t_1 = __pyx_v_sigindex_candidates; __Pyx_INCREF(__pyx_t_1);
+      __pyx_t_5 = 0;
       for (;;) {
-        if (__pyx_t_5 >= PyList_GET_SIZE(__pyx_t_1)) break;
+        {
+          Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_1);
+          #if !CYTHON_ASSUME_SAFE_MACROS
+          if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 74, __pyx_L1_error)
+          #endif
+          if (__pyx_t_5 >= __pyx_temp) break;
+        }
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_6 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_5); __Pyx_INCREF(__pyx_t_6); __pyx_t_5++; if (unlikely((0 < 0))) __PYX_ERR(0, 74, __pyx_L1_error)
+        __pyx_t_16 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_5); __Pyx_INCREF(__pyx_t_16); __pyx_t_5++; if (unlikely((0 < 0))) __PYX_ERR(0, 74, __pyx_L1_error)
         #else
-        __pyx_t_6 = PySequence_ITEM(__pyx_t_1, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 74, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_6);
+        __pyx_t_16 = __Pyx_PySequence_ITEM(__pyx_t_1, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 74, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_16);
         #endif
-        if (!(likely(PyDict_CheckExact(__pyx_t_6))||((__pyx_t_6) == Py_None) || __Pyx_RaiseUnexpectedTypeError("dict", __pyx_t_6))) __PYX_ERR(0, 74, __pyx_L1_error)
-        __Pyx_XDECREF_SET(__pyx_v_sn, ((PyObject*)__pyx_t_6));
-        __pyx_t_6 = 0;
+        __Pyx_XDECREF_SET(__pyx_v_sn, __pyx_t_16);
+        __pyx_t_16 = 0;
         if (unlikely(__pyx_v_sn == Py_None)) {
           PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "values");
           __PYX_ERR(0, 74, __pyx_L1_error)
         }
-        __pyx_t_6 = __Pyx_PyDict_Values(__pyx_v_sn); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 74, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_6);
-        __pyx_t_19 = __Pyx_PyList_Extend(__pyx_v_found_candidates, __pyx_t_6); if (unlikely(__pyx_t_19 == ((int)-1))) __PYX_ERR(0, 74, __pyx_L1_error)
-        __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+        __pyx_t_16 = __Pyx_PyDict_Values(((PyObject*)__pyx_v_sn)); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 74, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_16);
+        __pyx_t_19 = __Pyx_PyList_Extend(__pyx_v_found_candidates, __pyx_t_16); if (unlikely(__pyx_t_19 == ((int)-1))) __PYX_ERR(0, 74, __pyx_L1_error)
+        __Pyx_DECREF(__pyx_t_16); __pyx_t_16 = 0;
       }
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       goto __pyx_L75;
     }
     /*else*/ {
       __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 74, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_INCREF(__pyx_v_sigindex_matches);
       __Pyx_GIVEREF(__pyx_v_sigindex_matches);
       if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_sigindex_matches)) __PYX_ERR(0, 74, __pyx_L1_error);
       __Pyx_INCREF(__pyx_v_sigindex_candidates);
       __Pyx_GIVEREF(__pyx_v_sigindex_candidates);
       if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_v_sigindex_candidates)) __PYX_ERR(0, 74, __pyx_L1_error);
-      __pyx_t_6 = __pyx_t_1; __Pyx_INCREF(__pyx_t_6); __pyx_t_5 = 0;
+      __pyx_t_16 = __pyx_t_1; __Pyx_INCREF(__pyx_t_16);
+      __pyx_t_5 = 0;
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       for (;;) {
         if (__pyx_t_5 >= 2) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_1 = PyTuple_GET_ITEM(__pyx_t_6, __pyx_t_5); __Pyx_INCREF(__pyx_t_1); __pyx_t_5++; if (unlikely((0 < 0))) __PYX_ERR(0, 74, __pyx_L1_error)
+        __pyx_t_1 = PyTuple_GET_ITEM(__pyx_t_16, __pyx_t_5); __Pyx_INCREF(__pyx_t_1); __pyx_t_5++; if (unlikely((0 < 0))) __PYX_ERR(0, 74, __pyx_L1_error)
         #else
-        __pyx_t_1 = PySequence_ITEM(__pyx_t_6, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 74, __pyx_L1_error)
+        __pyx_t_1 = __Pyx_PySequence_ITEM(__pyx_t_16, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 74, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         #endif
         __Pyx_XDECREF_SET(__pyx_v_search_list, ((PyObject*)__pyx_t_1));
         __pyx_t_1 = 0;
         if (unlikely(__pyx_v_search_list == Py_None)) {
           PyErr_SetString(PyExc_TypeError, "'NoneType' object is not iterable");
           __PYX_ERR(0, 74, __pyx_L1_error)
         }
-        __pyx_t_1 = __pyx_v_search_list; __Pyx_INCREF(__pyx_t_1); __pyx_t_18 = 0;
+        __pyx_t_1 = __pyx_v_search_list; __Pyx_INCREF(__pyx_t_1);
+        __pyx_t_18 = 0;
         for (;;) {
-          if (__pyx_t_18 >= PyList_GET_SIZE(__pyx_t_1)) break;
+          {
+            Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_1);
+            #if !CYTHON_ASSUME_SAFE_MACROS
+            if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 74, __pyx_L1_error)
+            #endif
+            if (__pyx_t_18 >= __pyx_temp) break;
+          }
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_16 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_18); __Pyx_INCREF(__pyx_t_16); __pyx_t_18++; if (unlikely((0 < 0))) __PYX_ERR(0, 74, __pyx_L1_error)
+          __pyx_t_6 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_18); __Pyx_INCREF(__pyx_t_6); __pyx_t_18++; if (unlikely((0 < 0))) __PYX_ERR(0, 74, __pyx_L1_error)
           #else
-          __pyx_t_16 = PySequence_ITEM(__pyx_t_1, __pyx_t_18); __pyx_t_18++; if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 74, __pyx_L1_error)
-          __Pyx_GOTREF(__pyx_t_16);
+          __pyx_t_6 = __Pyx_PySequence_ITEM(__pyx_t_1, __pyx_t_18); __pyx_t_18++; if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 74, __pyx_L1_error)
+          __Pyx_GOTREF(__pyx_t_6);
           #endif
-          if (!(likely(PyDict_CheckExact(__pyx_t_16))||((__pyx_t_16) == Py_None) || __Pyx_RaiseUnexpectedTypeError("dict", __pyx_t_16))) __PYX_ERR(0, 74, __pyx_L1_error)
-          __Pyx_XDECREF_SET(__pyx_v_sn, ((PyObject*)__pyx_t_16));
-          __pyx_t_16 = 0;
+          __Pyx_XDECREF_SET(__pyx_v_sn, __pyx_t_6);
+          __pyx_t_6 = 0;
           if (unlikely(__pyx_v_sn == Py_None)) {
-            PyErr_SetString(PyExc_TypeError, "'NoneType' object is not iterable");
+            PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "get");
             __PYX_ERR(0, 74, __pyx_L1_error)
           }
-          __pyx_t_4 = (__Pyx_PyDict_ContainsTF(__pyx_v_dst_type, __pyx_v_sn, Py_EQ)); if (unlikely((__pyx_t_4 < 0))) __PYX_ERR(0, 74, __pyx_L1_error)
+          __pyx_t_6 = __Pyx_PyDict_GetItemDefault(((PyObject*)__pyx_v_sn), __pyx_v_dst_type, Py_None); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 74, __pyx_L1_error)
+          __Pyx_GOTREF(__pyx_t_6);
+          __Pyx_XDECREF_SET(__pyx_v_type_match, __pyx_t_6);
+          __pyx_t_6 = 0;
+          __pyx_t_4 = (__pyx_v_type_match != Py_None);
           if (__pyx_t_4) {
-            if (unlikely(__pyx_v_sn == Py_None)) {
-              PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-              __PYX_ERR(0, 74, __pyx_L1_error)
-            }
-            __pyx_t_16 = __Pyx_PyDict_GetItem(__pyx_v_sn, __pyx_v_dst_type); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 74, __pyx_L1_error)
-            __Pyx_GOTREF(__pyx_t_16);
-            __pyx_t_19 = __Pyx_PyList_Append(__pyx_v_found_matches, __pyx_t_16); if (unlikely(__pyx_t_19 == ((int)-1))) __PYX_ERR(0, 74, __pyx_L1_error)
-            __Pyx_DECREF(__pyx_t_16); __pyx_t_16 = 0;
+            __pyx_t_19 = __Pyx_PyList_Append(__pyx_v_found_matches, __pyx_v_type_match); if (unlikely(__pyx_t_19 == ((int)-1))) __PYX_ERR(0, 74, __pyx_L1_error)
           }
         }
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       }
-      __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+      __Pyx_DECREF(__pyx_t_16); __pyx_t_16 = 0;
     }
     __pyx_L75:;
     __Pyx_INCREF(__pyx_v_found_matches);
     __Pyx_DECREF_SET(__pyx_v_sigindex_matches, __pyx_v_found_matches);
     __Pyx_INCREF(__pyx_v_found_candidates);
     __Pyx_DECREF_SET(__pyx_v_sigindex_candidates, __pyx_v_found_candidates);
     __pyx_t_2 = (PyList_GET_SIZE(__pyx_v_found_matches) != 0);
@@ -21338,15 +21338,14 @@
   __Pyx_XDECREF(__pyx_t_13);
   __Pyx_XDECREF(__pyx_t_16);
   __Pyx_XDECREF(__pyx_t_17);
   __Pyx_AddTraceback("linearmodels.panel._utility.__pyx_fused_cpdef", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_search_list);
-  __Pyx_XDECREF(__pyx_v_sn);
   __Pyx_XDECREF(__pyx_v_sigindex_node);
   __Pyx_XDECREF(__pyx_v_dest_sig);
   __Pyx_XDECREF((PyObject *)__pyx_v_ndarray);
   __Pyx_XDECREF(__pyx_v_arg_as_memoryview);
   __Pyx_XDECREF(__pyx_v_arg);
   __Pyx_XDECREF(__pyx_v_dtype);
   __Pyx_XDECREF(__pyx_v_arg_base);
@@ -21355,14 +21354,16 @@
   __Pyx_XDECREF(__pyx_v_last_type);
   __Pyx_XDECREF(__pyx_v_sig_type);
   __Pyx_XDECREF(__pyx_v_sigindex_matches);
   __Pyx_XDECREF(__pyx_v_sigindex_candidates);
   __Pyx_XDECREF(__pyx_v_dst_type);
   __Pyx_XDECREF(__pyx_v_found_matches);
   __Pyx_XDECREF(__pyx_v_found_candidates);
+  __Pyx_XDECREF(__pyx_v_sn);
+  __Pyx_XDECREF(__pyx_v_type_match);
   __Pyx_XDECREF(__pyx_v_candidates);
   __Pyx_XDECREF(__pyx_v_kwargs);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
@@ -21380,16 +21381,15 @@
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("_drop_singletons (wrapper)", 0);
   #if CYTHON_ASSUME_SAFE_MACROS
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
-  __pyx_nargs = PyTuple_Size(__pyx_args);
-  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(0, 74, __pyx_L3_error)
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   __pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
   {
     PyObject **__pyx_pyargnames[] = {&__pyx_n_s_meta,&__pyx_n_s_orig_dest,0};
     if (__pyx_kwds) {
       Py_ssize_t kw_args;
       switch (__pyx_nargs) {
@@ -21429,18 +21429,19 @@
     } else {
       values[0] = __Pyx_Arg_VARARGS(__pyx_args, 0);
       values[1] = __Pyx_Arg_VARARGS(__pyx_args, 1);
     }
     __pyx_v_meta = __Pyx_PyObject_to_MemoryviewSlice_d_dc_nn___pyx_t_5numpy_int8_t(values[0], PyBUF_WRITABLE); if (unlikely(!__pyx_v_meta.memview)) __PYX_ERR(0, 74, __pyx_L3_error)
     __pyx_v_orig_dest = __Pyx_PyObject_to_MemoryviewSlice_d_dc_nn___pyx_t_5numpy_int8_t(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_orig_dest.memview)) __PYX_ERR(0, 74, __pyx_L3_error)
   }
-  goto __pyx_L4_argument_unpacking_done;
+  goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("_drop_singletons", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 74, __pyx_L3_error)
-  goto __pyx_L3_error;
+  __pyx_L6_skip:;
+  goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_VARARGS(values[__pyx_temp]);
     }
   }
@@ -21476,15 +21477,15 @@
   __pyx_t_5numpy_int8_t __pyx_t_3;
   Py_ssize_t __pyx_t_4;
   Py_ssize_t __pyx_t_5;
   int __pyx_t_6;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__pyx_fuse_0_drop_singletons", 0);
+  __Pyx_RefNannySetupContext("__pyx_fuse_0_drop_singletons", 1);
 
   /* "linearmodels/panel/_utility.pyx":87
  *     """
  *     cdef any_int next_node, next_count, i
  *     for i in range(meta.shape[0]):             # <<<<<<<<<<<<<<
  *         if meta[i, 1] == 1:
  *             next_node = i
@@ -21587,16 +21588,15 @@
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("_drop_singletons (wrapper)", 0);
   #if CYTHON_ASSUME_SAFE_MACROS
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
-  __pyx_nargs = PyTuple_Size(__pyx_args);
-  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(0, 74, __pyx_L3_error)
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   __pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
   {
     PyObject **__pyx_pyargnames[] = {&__pyx_n_s_meta,&__pyx_n_s_orig_dest,0};
     if (__pyx_kwds) {
       Py_ssize_t kw_args;
       switch (__pyx_nargs) {
@@ -21636,18 +21636,19 @@
     } else {
       values[0] = __Pyx_Arg_VARARGS(__pyx_args, 0);
       values[1] = __Pyx_Arg_VARARGS(__pyx_args, 1);
     }
     __pyx_v_meta = __Pyx_PyObject_to_MemoryviewSlice_d_dc_nn___pyx_t_5numpy_int16_t(values[0], PyBUF_WRITABLE); if (unlikely(!__pyx_v_meta.memview)) __PYX_ERR(0, 74, __pyx_L3_error)
     __pyx_v_orig_dest = __Pyx_PyObject_to_MemoryviewSlice_d_dc_nn___pyx_t_5numpy_int16_t(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_orig_dest.memview)) __PYX_ERR(0, 74, __pyx_L3_error)
   }
-  goto __pyx_L4_argument_unpacking_done;
+  goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("_drop_singletons", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 74, __pyx_L3_error)
-  goto __pyx_L3_error;
+  __pyx_L6_skip:;
+  goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_VARARGS(values[__pyx_temp]);
     }
   }
@@ -21683,15 +21684,15 @@
   __pyx_t_5numpy_int16_t __pyx_t_3;
   Py_ssize_t __pyx_t_4;
   Py_ssize_t __pyx_t_5;
   int __pyx_t_6;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__pyx_fuse_1_drop_singletons", 0);
+  __Pyx_RefNannySetupContext("__pyx_fuse_1_drop_singletons", 1);
 
   /* "linearmodels/panel/_utility.pyx":87
  *     """
  *     cdef any_int next_node, next_count, i
  *     for i in range(meta.shape[0]):             # <<<<<<<<<<<<<<
  *         if meta[i, 1] == 1:
  *             next_node = i
@@ -21794,16 +21795,15 @@
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("_drop_singletons (wrapper)", 0);
   #if CYTHON_ASSUME_SAFE_MACROS
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
-  __pyx_nargs = PyTuple_Size(__pyx_args);
-  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(0, 74, __pyx_L3_error)
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   __pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
   {
     PyObject **__pyx_pyargnames[] = {&__pyx_n_s_meta,&__pyx_n_s_orig_dest,0};
     if (__pyx_kwds) {
       Py_ssize_t kw_args;
       switch (__pyx_nargs) {
@@ -21843,18 +21843,19 @@
     } else {
       values[0] = __Pyx_Arg_VARARGS(__pyx_args, 0);
       values[1] = __Pyx_Arg_VARARGS(__pyx_args, 1);
     }
     __pyx_v_meta = __Pyx_PyObject_to_MemoryviewSlice_d_dc_nn___pyx_t_5numpy_int32_t(values[0], PyBUF_WRITABLE); if (unlikely(!__pyx_v_meta.memview)) __PYX_ERR(0, 74, __pyx_L3_error)
     __pyx_v_orig_dest = __Pyx_PyObject_to_MemoryviewSlice_d_dc_nn___pyx_t_5numpy_int32_t(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_orig_dest.memview)) __PYX_ERR(0, 74, __pyx_L3_error)
   }
-  goto __pyx_L4_argument_unpacking_done;
+  goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("_drop_singletons", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 74, __pyx_L3_error)
-  goto __pyx_L3_error;
+  __pyx_L6_skip:;
+  goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_VARARGS(values[__pyx_temp]);
     }
   }
@@ -21890,15 +21891,15 @@
   __pyx_t_5numpy_int32_t __pyx_t_3;
   Py_ssize_t __pyx_t_4;
   Py_ssize_t __pyx_t_5;
   int __pyx_t_6;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__pyx_fuse_2_drop_singletons", 0);
+  __Pyx_RefNannySetupContext("__pyx_fuse_2_drop_singletons", 1);
 
   /* "linearmodels/panel/_utility.pyx":87
  *     """
  *     cdef any_int next_node, next_count, i
  *     for i in range(meta.shape[0]):             # <<<<<<<<<<<<<<
  *         if meta[i, 1] == 1:
  *             next_node = i
@@ -22001,16 +22002,15 @@
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("_drop_singletons (wrapper)", 0);
   #if CYTHON_ASSUME_SAFE_MACROS
   __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #else
-  __pyx_nargs = PyTuple_Size(__pyx_args);
-  if (unlikely((__pyx_nargs < 0))) __PYX_ERR(0, 74, __pyx_L3_error)
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   __pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
   {
     PyObject **__pyx_pyargnames[] = {&__pyx_n_s_meta,&__pyx_n_s_orig_dest,0};
     if (__pyx_kwds) {
       Py_ssize_t kw_args;
       switch (__pyx_nargs) {
@@ -22050,18 +22050,19 @@
     } else {
       values[0] = __Pyx_Arg_VARARGS(__pyx_args, 0);
       values[1] = __Pyx_Arg_VARARGS(__pyx_args, 1);
     }
     __pyx_v_meta = __Pyx_PyObject_to_MemoryviewSlice_d_dc_nn___pyx_t_5numpy_int64_t(values[0], PyBUF_WRITABLE); if (unlikely(!__pyx_v_meta.memview)) __PYX_ERR(0, 74, __pyx_L3_error)
     __pyx_v_orig_dest = __Pyx_PyObject_to_MemoryviewSlice_d_dc_nn___pyx_t_5numpy_int64_t(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_orig_dest.memview)) __PYX_ERR(0, 74, __pyx_L3_error)
   }
-  goto __pyx_L4_argument_unpacking_done;
+  goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("_drop_singletons", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 74, __pyx_L3_error)
-  goto __pyx_L3_error;
+  __pyx_L6_skip:;
+  goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_VARARGS(values[__pyx_temp]);
     }
   }
@@ -22097,15 +22098,15 @@
   __pyx_t_5numpy_int64_t __pyx_t_3;
   __pyx_t_5numpy_int64_t __pyx_t_4;
   Py_ssize_t __pyx_t_5;
   int __pyx_t_6;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__pyx_fuse_3_drop_singletons", 0);
+  __Pyx_RefNannySetupContext("__pyx_fuse_3_drop_singletons", 1);
 
   /* "linearmodels/panel/_utility.pyx":87
  *     """
  *     cdef any_int next_node, next_count, i
  *     for i in range(meta.shape[0]):             # <<<<<<<<<<<<<<
  *         if meta[i, 1] == 1:
  *             next_node = i
@@ -23227,14 +23228,15 @@
     {&__pyx_n_s_error, __pyx_k_error, sizeof(__pyx_k_error), 0, 0, 1, 1},
     {&__pyx_n_s_flags, __pyx_k_flags, sizeof(__pyx_k_flags), 0, 0, 1, 1},
     {&__pyx_n_s_format, __pyx_k_format, sizeof(__pyx_k_format), 0, 0, 1, 1},
     {&__pyx_n_s_fortran, __pyx_k_fortran, sizeof(__pyx_k_fortran), 0, 0, 1, 1},
     {&__pyx_n_u_fortran, __pyx_k_fortran, sizeof(__pyx_k_fortran), 0, 1, 0, 1},
     {&__pyx_n_s_fused_sigindex, __pyx_k_fused_sigindex, sizeof(__pyx_k_fused_sigindex), 0, 0, 1, 1},
     {&__pyx_kp_u_gc, __pyx_k_gc, sizeof(__pyx_k_gc), 0, 1, 0, 0},
+    {&__pyx_n_s_get, __pyx_k_get, sizeof(__pyx_k_get), 0, 0, 1, 1},
     {&__pyx_n_s_getstate, __pyx_k_getstate, sizeof(__pyx_k_getstate), 0, 0, 1, 1},
     {&__pyx_kp_u_got, __pyx_k_got, sizeof(__pyx_k_got), 0, 1, 0, 0},
     {&__pyx_kp_u_got_differing_extents_in_dimensi, __pyx_k_got_differing_extents_in_dimensi, sizeof(__pyx_k_got_differing_extents_in_dimensi), 0, 1, 0, 0},
     {&__pyx_n_s_i, __pyx_k_i, sizeof(__pyx_k_i), 0, 0, 1, 1},
     {&__pyx_n_s_id, __pyx_k_id, sizeof(__pyx_k_id), 0, 0, 1, 1},
     {&__pyx_n_s_import, __pyx_k_import, sizeof(__pyx_k_import), 0, 0, 1, 1},
     {&__pyx_n_s_index, __pyx_k_index, sizeof(__pyx_k_index), 0, 0, 1, 1},
@@ -23365,26 +23367,26 @@
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError, "Incompatible checksums (0x%x vs (0x82a3537, 0x6ae9995, 0xb068931) = (name))" % __pyx_checksum
  */
   __pyx_tuple__8 = PyTuple_Pack(3, __pyx_int_136983863, __pyx_int_112105877, __pyx_int_184977713); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__8);
   __Pyx_GIVEREF(__pyx_tuple__8);
 
-  /* "../../../tmp/build-env-b2_49hlm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":987
+  /* "../../../tmp/build-env-wicvywyh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":987
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(2, 987, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__9);
   __Pyx_GIVEREF(__pyx_tuple__9);
 
-  /* "../../../tmp/build-env-b2_49hlm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":993
+  /* "../../../tmp/build-env-wicvywyh/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":993
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__10 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(2, 993, __pyx_L1_error)
@@ -23522,14 +23524,16 @@
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 /* #### Code section: init_constants ### */
 
 static CYTHON_SMALL_CODE int __Pyx_InitConstants(void) {
+  __pyx_umethod_PyDict_Type_get.type = (PyObject*)&PyDict_Type;
+  __pyx_umethod_PyDict_Type_get.method_name = &__pyx_n_s_get;
   __pyx_umethod_PyDict_Type_values.type = (PyObject*)&PyDict_Type;
   __pyx_umethod_PyDict_Type_values.method_name = &__pyx_n_s_values;
   if (__Pyx_CreateStringTabAndInitStrings() < 0) __PYX_ERR(0, 1, __pyx_L1_error);
   __pyx_int_0 = PyInt_FromLong(0); if (unlikely(!__pyx_int_0)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_1 = PyInt_FromLong(1); if (unlikely(!__pyx_int_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_2 = PyInt_FromLong(2); if (unlikely(!__pyx_int_2)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_3 = PyInt_FromLong(3); if (unlikely(!__pyx_int_3)) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -23774,41 +23778,41 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_3_0_2(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_3_0_7(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_2(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_7(PyTypeObject),
   #elif CYTHON_COMPILING_IN_LIMITED_API
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_2(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_7(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_2(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_7(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn_3_0_2); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_3_0_7); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 203, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5numpy_dtype = __Pyx_ImportType_3_0_2(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT_3_0_2(PyArray_Descr),__Pyx_ImportType_CheckSize_Ignore_3_0_2); if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(2, 203, __pyx_L1_error)
-  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType_3_0_2(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_2(PyArrayIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_2); if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(2, 226, __pyx_L1_error)
-  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType_3_0_2(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_2(PyArrayMultiIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_2); if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(2, 230, __pyx_L1_error)
-  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType_3_0_2(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_2(PyArrayObject),__Pyx_ImportType_CheckSize_Ignore_3_0_2); if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(2, 239, __pyx_L1_error)
-  __pyx_ptype_5numpy_generic = __Pyx_ImportType_3_0_2(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_2(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_2); if (!__pyx_ptype_5numpy_generic) __PYX_ERR(2, 813, __pyx_L1_error)
-  __pyx_ptype_5numpy_number = __Pyx_ImportType_3_0_2(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_2(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_2); if (!__pyx_ptype_5numpy_number) __PYX_ERR(2, 815, __pyx_L1_error)
-  __pyx_ptype_5numpy_integer = __Pyx_ImportType_3_0_2(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_2(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_2); if (!__pyx_ptype_5numpy_integer) __PYX_ERR(2, 817, __pyx_L1_error)
-  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType_3_0_2(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_2(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_2); if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(2, 819, __pyx_L1_error)
-  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType_3_0_2(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_2(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_2); if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(2, 821, __pyx_L1_error)
-  __pyx_ptype_5numpy_inexact = __Pyx_ImportType_3_0_2(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_2(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_2); if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(2, 823, __pyx_L1_error)
-  __pyx_ptype_5numpy_floating = __Pyx_ImportType_3_0_2(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_2(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_2); if (!__pyx_ptype_5numpy_floating) __PYX_ERR(2, 825, __pyx_L1_error)
-  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType_3_0_2(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_2(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_2); if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(2, 827, __pyx_L1_error)
-  __pyx_ptype_5numpy_flexible = __Pyx_ImportType_3_0_2(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_2(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_2); if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(2, 829, __pyx_L1_error)
-  __pyx_ptype_5numpy_character = __Pyx_ImportType_3_0_2(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_2(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_2); if (!__pyx_ptype_5numpy_character) __PYX_ERR(2, 831, __pyx_L1_error)
-  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType_3_0_2(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_2(PyUFuncObject),__Pyx_ImportType_CheckSize_Ignore_3_0_2); if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(2, 869, __pyx_L1_error)
+  __pyx_ptype_5numpy_dtype = __Pyx_ImportType_3_0_7(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT_3_0_7(PyArray_Descr),__Pyx_ImportType_CheckSize_Ignore_3_0_7); if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(2, 203, __pyx_L1_error)
+  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType_3_0_7(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_7(PyArrayIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_7); if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(2, 226, __pyx_L1_error)
+  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType_3_0_7(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_7(PyArrayMultiIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_7); if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(2, 230, __pyx_L1_error)
+  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType_3_0_7(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_7(PyArrayObject),__Pyx_ImportType_CheckSize_Ignore_3_0_7); if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(2, 239, __pyx_L1_error)
+  __pyx_ptype_5numpy_generic = __Pyx_ImportType_3_0_7(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_7(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_7); if (!__pyx_ptype_5numpy_generic) __PYX_ERR(2, 813, __pyx_L1_error)
+  __pyx_ptype_5numpy_number = __Pyx_ImportType_3_0_7(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_7(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_7); if (!__pyx_ptype_5numpy_number) __PYX_ERR(2, 815, __pyx_L1_error)
+  __pyx_ptype_5numpy_integer = __Pyx_ImportType_3_0_7(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_7(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_7); if (!__pyx_ptype_5numpy_integer) __PYX_ERR(2, 817, __pyx_L1_error)
+  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType_3_0_7(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_7(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_7); if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(2, 819, __pyx_L1_error)
+  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType_3_0_7(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_7(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_7); if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(2, 821, __pyx_L1_error)
+  __pyx_ptype_5numpy_inexact = __Pyx_ImportType_3_0_7(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_7(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_7); if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(2, 823, __pyx_L1_error)
+  __pyx_ptype_5numpy_floating = __Pyx_ImportType_3_0_7(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_7(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_7); if (!__pyx_ptype_5numpy_floating) __PYX_ERR(2, 825, __pyx_L1_error)
+  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType_3_0_7(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_7(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_7); if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(2, 827, __pyx_L1_error)
+  __pyx_ptype_5numpy_flexible = __Pyx_ImportType_3_0_7(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_7(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_7); if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(2, 829, __pyx_L1_error)
+  __pyx_ptype_5numpy_character = __Pyx_ImportType_3_0_7(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_7(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_7); if (!__pyx_ptype_5numpy_character) __PYX_ERR(2, 831, __pyx_L1_error)
+  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType_3_0_7(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_7(PyUFuncObject),__Pyx_ImportType_CheckSize_Ignore_3_0_7); if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(2, 869, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -24020,42 +24024,40 @@
   #if PY_MAJOR_VERSION < 3
   __pyx_m = Py_InitModule4("_utility", __pyx_methods, 0, 0, PYTHON_API_VERSION); Py_XINCREF(__pyx_m);
   if (unlikely(!__pyx_m)) __PYX_ERR(0, 1, __pyx_L1_error)
   #elif CYTHON_USE_MODULE_STATE
   __pyx_t_1 = PyModule_Create(&__pyx_moduledef); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   {
     int add_module_result = PyState_AddModule(__pyx_t_1, &__pyx_moduledef);
-    __pyx_t_1 = 0; /* transfer ownership from __pyx_t_1 to _utility pseudovariable */
+    __pyx_t_1 = 0; /* transfer ownership from __pyx_t_1 to "_utility" pseudovariable */
     if (unlikely((add_module_result < 0))) __PYX_ERR(0, 1, __pyx_L1_error)
     pystate_addmodule_run = 1;
   }
   #else
   __pyx_m = PyModule_Create(&__pyx_moduledef);
   if (unlikely(!__pyx_m)) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   #endif
   CYTHON_UNUSED_VAR(__pyx_t_1);
   __pyx_d = PyModule_GetDict(__pyx_m); if (unlikely(!__pyx_d)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_d);
-  __pyx_b = PyImport_AddModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_b)) __PYX_ERR(0, 1, __pyx_L1_error)
-  Py_INCREF(__pyx_b);
-  __pyx_cython_runtime = PyImport_AddModule((char *) "cython_runtime"); if (unlikely(!__pyx_cython_runtime)) __PYX_ERR(0, 1, __pyx_L1_error)
-  Py_INCREF(__pyx_cython_runtime);
+  __pyx_b = __Pyx_PyImport_AddModuleRef(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_b)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_cython_runtime = __Pyx_PyImport_AddModuleRef((const char *) "cython_runtime"); if (unlikely(!__pyx_cython_runtime)) __PYX_ERR(0, 1, __pyx_L1_error)
   if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #if CYTHON_REFNANNY
 __Pyx_RefNanny = __Pyx_RefNannyImportAPI("refnanny");
 if (!__Pyx_RefNanny) {
   PyErr_Clear();
   __Pyx_RefNanny = __Pyx_RefNannyImportAPI("Cython.Runtime.refnanny");
   if (!__Pyx_RefNanny)
       Py_FatalError("failed to import 'refnanny' module");
 }
 #endif
   __Pyx_RefNannySetupContext("__Pyx_PyMODINIT_FUNC PyInit__utility(void)", 0);
-  if (__Pyx_check_binary_version() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_check_binary_version(__PYX_LIMITED_VERSION_HEX, __Pyx_get_runtime_version(), CYTHON_COMPILING_IN_LIMITED_API) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #ifdef __Pxy_PyFrame_Initialize_Offsets
   __Pxy_PyFrame_Initialize_Offsets();
   #endif
   __pyx_empty_tuple = PyTuple_New(0); if (unlikely(!__pyx_empty_tuple)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_empty_bytes = PyBytes_FromStringAndSize("", 0); if (unlikely(!__pyx_empty_bytes)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_empty_unicode = PyUnicode_FromStringAndSize("", 0); if (unlikely(!__pyx_empty_unicode)) __PYX_ERR(0, 1, __pyx_L1_error)
   #ifdef __Pyx_CyFunction_USED
@@ -24807,14 +24809,16 @@
         if (unlikely(((PyBaseExceptionObject*) value)->traceback != tb))
         #endif
             PyException_SetTraceback(value, tb);
     }
     tmp_value = tstate->current_exception;
     tstate->current_exception = value;
     Py_XDECREF(tmp_value);
+    Py_XDECREF(type);
+    Py_XDECREF(tb);
 #else
     PyObject *tmp_type, *tmp_value, *tmp_tb;
     tmp_type = tstate->curexc_type;
     tmp_value = tstate->curexc_value;
     tmp_tb = tstate->curexc_traceback;
     tstate->curexc_type = type;
     tstate->curexc_value = value;
@@ -24864,33 +24868,40 @@
         return tp->tp_getattr(obj, PyString_AS_STRING(attr_name));
 #endif
     return PyObject_GetAttr(obj, attr_name);
 }
 #endif
 
 /* PyObjectGetAttrStrNoError */
+#if __PYX_LIMITED_VERSION_HEX < 0x030d00A1
 static void __Pyx_PyObject_GetAttrStr_ClearAttributeError(void) {
     __Pyx_PyThreadState_declare
     __Pyx_PyThreadState_assign
     if (likely(__Pyx_PyErr_ExceptionMatches(PyExc_AttributeError)))
         __Pyx_PyErr_Clear();
 }
+#endif
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStrNoError(PyObject* obj, PyObject* attr_name) {
     PyObject *result;
+#if __PYX_LIMITED_VERSION_HEX >= 0x030d00A1
+    (void) PyObject_GetOptionalAttr(obj, attr_name, &result);
+    return result;
+#else
 #if CYTHON_COMPILING_IN_CPYTHON && CYTHON_USE_TYPE_SLOTS && PY_VERSION_HEX >= 0x030700B1
     PyTypeObject* tp = Py_TYPE(obj);
     if (likely(tp->tp_getattro == PyObject_GenericGetAttr)) {
         return _PyObject_GenericGetAttrWithDict(obj, attr_name, NULL, 1);
     }
 #endif
     result = __Pyx_PyObject_GetAttrStr(obj, attr_name);
     if (unlikely(!result)) {
         __Pyx_PyObject_GetAttrStr_ClearAttributeError();
     }
     return result;
+#endif
 }
 
 /* GetBuiltinName */
 static PyObject *__Pyx_GetBuiltinName(PyObject *name) {
     PyObject* result = __Pyx_PyObject_GetAttrStrNoError(__pyx_b, name);
     if (unlikely(!result) && !PyErr_Occurred()) {
         PyErr_Format(PyExc_NameError,
@@ -25104,14 +25115,32 @@
         if (unlikely(eq != 0)) {
             if (unlikely(eq < 0)) return NULL;  // error
             return kwvalues[i];
         }
     }
     return NULL;  // not found (no exception set)
 }
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030d0000
+CYTHON_UNUSED static PyObject *__Pyx_KwargsAsDict_FASTCALL(PyObject *kwnames, PyObject *const *kwvalues) {
+    Py_ssize_t i, nkwargs = PyTuple_GET_SIZE(kwnames);
+    PyObject *dict;
+    dict = PyDict_New();
+    if (unlikely(!dict))
+        return NULL;
+    for (i=0; i<nkwargs; i++) {
+        PyObject *key = PyTuple_GET_ITEM(kwnames, i);
+        if (unlikely(PyDict_SetItem(dict, key, kwvalues[i]) < 0))
+            goto bad;
+    }
+    return dict;
+bad:
+    Py_DECREF(dict);
+    return NULL;
+}
+#endif
 #endif
 
 /* RaiseArgTupleInvalid */
 static void __Pyx_RaiseArgtupleInvalid(
     const char* func_name,
     int exact,
     Py_ssize_t num_min,
@@ -25535,17 +25564,23 @@
     PyObject *kwtuple, **k;
     PyObject **d;
     Py_ssize_t nd;
     Py_ssize_t nk;
     PyObject *result;
     assert(kwargs == NULL || PyDict_Check(kwargs));
     nk = kwargs ? PyDict_Size(kwargs) : 0;
+    #if PY_MAJOR_VERSION < 3
     if (unlikely(Py_EnterRecursiveCall((char*)" while calling a Python object"))) {
         return NULL;
     }
+    #else
+    if (unlikely(Py_EnterRecursiveCall(" while calling a Python object"))) {
+        return NULL;
+    }
+    #endif
     if (
 #if PY_MAJOR_VERSION >= 3
             co->co_kwonlyargcount == 0 &&
 #endif
             likely(kwargs == NULL || nk == 0) &&
             co->co_flags == (CO_OPTIMIZED | CO_NEWLOCALS | CO_NOFREE)) {
         if (argdefs == NULL && co->co_argcount == nargs) {
@@ -25614,16 +25649,21 @@
 /* PyObjectCall */
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_Call(PyObject *func, PyObject *arg, PyObject *kw) {
     PyObject *result;
     ternaryfunc call = Py_TYPE(func)->tp_call;
     if (unlikely(!call))
         return PyObject_Call(func, arg, kw);
+    #if PY_MAJOR_VERSION < 3
     if (unlikely(Py_EnterRecursiveCall((char*)" while calling a Python object")))
         return NULL;
+    #else
+    if (unlikely(Py_EnterRecursiveCall(" while calling a Python object")))
+        return NULL;
+    #endif
     result = (*call)(func, arg, kw);
     Py_LeaveRecursiveCall();
     if (unlikely(!result) && unlikely(!PyErr_Occurred())) {
         PyErr_SetString(
             PyExc_SystemError,
             "NULL result without error in PyObject_Call");
     }
@@ -25632,30 +25672,36 @@
 #endif
 
 /* PyObjectCallMethO */
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallMethO(PyObject *func, PyObject *arg) {
     PyObject *self, *result;
     PyCFunction cfunc;
-    cfunc = PyCFunction_GET_FUNCTION(func);
-    self = PyCFunction_GET_SELF(func);
+    cfunc = __Pyx_CyOrPyCFunction_GET_FUNCTION(func);
+    self = __Pyx_CyOrPyCFunction_GET_SELF(func);
+    #if PY_MAJOR_VERSION < 3
     if (unlikely(Py_EnterRecursiveCall((char*)" while calling a Python object")))
         return NULL;
+    #else
+    if (unlikely(Py_EnterRecursiveCall(" while calling a Python object")))
+        return NULL;
+    #endif
     result = cfunc(self, arg);
     Py_LeaveRecursiveCall();
     if (unlikely(!result) && unlikely(!PyErr_Occurred())) {
         PyErr_SetString(
             PyExc_SystemError,
             "NULL result without error in PyObject_Call");
     }
     return result;
 }
 #endif
 
 /* PyObjectFastCall */
+#if PY_VERSION_HEX < 0x03090000 || CYTHON_COMPILING_IN_LIMITED_API
 static PyObject* __Pyx_PyObject_FastCall_fallback(PyObject *func, PyObject **args, size_t nargs, PyObject *kwargs) {
     PyObject *argstuple;
     PyObject *result = 0;
     size_t i;
     argstuple = PyTuple_New((Py_ssize_t)nargs);
     if (unlikely(!argstuple)) return NULL;
     for (i = 0; i < nargs; i++) {
@@ -25663,36 +25709,25 @@
         if (__Pyx_PyTuple_SET_ITEM(argstuple, (Py_ssize_t)i, args[i]) < 0) goto bad;
     }
     result = __Pyx_PyObject_Call(func, argstuple, kwargs);
   bad:
     Py_DECREF(argstuple);
     return result;
 }
+#endif
 static CYTHON_INLINE PyObject* __Pyx_PyObject_FastCallDict(PyObject *func, PyObject **args, size_t _nargs, PyObject *kwargs) {
     Py_ssize_t nargs = __Pyx_PyVectorcall_NARGS(_nargs);
 #if CYTHON_COMPILING_IN_CPYTHON
     if (nargs == 0 && kwargs == NULL) {
-#if defined(__Pyx_CyFunction_USED) && defined(NDEBUG)
-        if (__Pyx_IsCyOrPyCFunction(func))
-#else
-        if (PyCFunction_Check(func))
-#endif
-        {
-            if (likely(PyCFunction_GET_FLAGS(func) & METH_NOARGS)) {
-                return __Pyx_PyObject_CallMethO(func, NULL);
-            }
-        }
+        if (__Pyx_CyOrPyCFunction_Check(func) && likely( __Pyx_CyOrPyCFunction_GET_FLAGS(func) & METH_NOARGS))
+            return __Pyx_PyObject_CallMethO(func, NULL);
     }
     else if (nargs == 1 && kwargs == NULL) {
-        if (PyCFunction_Check(func))
-        {
-            if (likely(PyCFunction_GET_FLAGS(func) & METH_O)) {
-                return __Pyx_PyObject_CallMethO(func, args[0]);
-            }
-        }
+        if (__Pyx_CyOrPyCFunction_Check(func) && likely( __Pyx_CyOrPyCFunction_GET_FLAGS(func) & METH_O))
+            return __Pyx_PyObject_CallMethO(func, args[0]);
     }
 #endif
     #if PY_VERSION_HEX < 0x030800B1
     #if CYTHON_FAST_PYCCALL
     if (PyCFunction_Check(func)) {
         if (kwargs) {
             return _PyCFunction_FastCallDict(func, args, nargs, kwargs);
@@ -25708,33 +25743,39 @@
     #endif
     #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(func)) {
         return __Pyx_PyFunction_FastCallDict(func, args, nargs, kwargs);
     }
     #endif
     #endif
-    #if CYTHON_VECTORCALL
-    #if Py_VERSION_HEX < 0x03090000
-    vectorcallfunc f = _PyVectorcall_Function(func);
-    #else
-    vectorcallfunc f = PyVectorcall_Function(func);
-    #endif
-    if (f) {
-        return f(func, args, (size_t)nargs, kwargs);
-    }
-    #elif defined(__Pyx_CyFunction_USED) && CYTHON_BACKPORT_VECTORCALL
-    if (__Pyx_CyFunction_CheckExact(func)) {
-        __pyx_vectorcallfunc f = __Pyx_CyFunction_func_vectorcall(func);
-        if (f) return f(func, args, (size_t)nargs, kwargs);
+    if (kwargs == NULL) {
+        #if CYTHON_VECTORCALL
+        #if PY_VERSION_HEX < 0x03090000
+        vectorcallfunc f = _PyVectorcall_Function(func);
+        #else
+        vectorcallfunc f = PyVectorcall_Function(func);
+        #endif
+        if (f) {
+            return f(func, args, (size_t)nargs, NULL);
+        }
+        #elif defined(__Pyx_CyFunction_USED) && CYTHON_BACKPORT_VECTORCALL
+        if (__Pyx_CyFunction_CheckExact(func)) {
+            __pyx_vectorcallfunc f = __Pyx_CyFunction_func_vectorcall(func);
+            if (f) return f(func, args, (size_t)nargs, NULL);
+        }
+        #endif
     }
-    #endif
     if (nargs == 0) {
         return __Pyx_PyObject_Call(func, __pyx_empty_tuple, kwargs);
     }
+    #if PY_VERSION_HEX >= 0x03090000 && !CYTHON_COMPILING_IN_LIMITED_API
+    return PyObject_VectorcallDict(func, args, (size_t)nargs, kwargs);
+    #else
     return __Pyx_PyObject_FastCall_fallback(func, args, (size_t)nargs, kwargs);
+    #endif
 }
 
 /* RaiseUnexpectedTypeError */
 static int
 __Pyx_RaiseUnexpectedTypeError(const char *expected, PyObject *obj)
 {
     __Pyx_TypeName obj_type_name = __Pyx_PyType_GetName(Py_TYPE(obj));
@@ -26029,15 +26070,15 @@
         if (unlikely((PY_SSIZE_T_MAX >> kind_shift) - ulength < char_pos))
             goto overflow;
         ukind = __Pyx_PyUnicode_KIND(uval);
         udata = __Pyx_PyUnicode_DATA(uval);
         if (!CYTHON_PEP393_ENABLED || ukind == result_ukind) {
             memcpy((char *)result_udata + (char_pos << kind_shift), udata, (size_t) (ulength << kind_shift));
         } else {
-            #if PY_VERSION_HEX >= 0x030D0000
+            #if PY_VERSION_HEX >= 0x030d0000
             if (unlikely(PyUnicode_CopyCharacters(result_uval, char_pos, uval, 0, ulength) < 0)) goto bad;
             #elif CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030300F0 || defined(_PyUnicode_FastCopyCharacters)
             _PyUnicode_FastCopyCharacters(result_uval, char_pos, uval, 0, ulength);
             #else
             Py_ssize_t j;
             for (j=0; j < ulength; j++) {
                 Py_UCS4 uchar = __Pyx_PyUnicode_READ(ukind, udata, j);
@@ -26158,15 +26199,15 @@
                     PyErr_Clear();
                 }
             }
             return sm->sq_item(o, i);
         }
     }
 #else
-    if (is_list || PySequence_Check(o)) {
+    if (is_list || !PyMapping_Check(o)) {
         return PySequence_GetItem(o, i);
     }
 #endif
     return __Pyx_GetItemInt_Generic(o, PyInt_FromSsize_t(i));
 }
 
 /* PyObjectCallOneArg */
@@ -26193,15 +26234,17 @@
     }
     return NULL;
 }
 static PyObject *__Pyx_PyObject_GetItem_Slow(PyObject *obj, PyObject *key) {
     __Pyx_TypeName obj_type_name;
     if (likely(PyType_Check(obj))) {
         PyObject *meth = __Pyx_PyObject_GetAttrStrNoError(obj, __pyx_n_s_class_getitem);
-        if (meth) {
+        if (!meth) {
+            PyErr_Clear();
+        } else {
             PyObject *result = __Pyx_PyObject_CallOneArg(meth, key);
             Py_DECREF(meth);
             return result;
         }
     }
     obj_type_name = __Pyx_PyType_GetName(Py_TYPE(obj));
     PyErr_Format(PyExc_TypeError,
@@ -26302,36 +26345,43 @@
     Py_ssize_t q = a / b;
     Py_ssize_t r = a - q*b;
     q -= ((r != 0) & ((r ^ b) < 0));
     return q;
 }
 
 /* GetAttr3 */
+#if __PYX_LIMITED_VERSION_HEX < 0x030d00A1
 static PyObject *__Pyx_GetAttr3Default(PyObject *d) {
     __Pyx_PyThreadState_declare
     __Pyx_PyThreadState_assign
     if (unlikely(!__Pyx_PyErr_ExceptionMatches(PyExc_AttributeError)))
         return NULL;
     __Pyx_PyErr_Clear();
     Py_INCREF(d);
     return d;
 }
+#endif
 static CYTHON_INLINE PyObject *__Pyx_GetAttr3(PyObject *o, PyObject *n, PyObject *d) {
     PyObject *r;
-#if CYTHON_USE_TYPE_SLOTS
+#if __PYX_LIMITED_VERSION_HEX >= 0x030d00A1
+    int res = PyObject_GetOptionalAttr(o, n, &r);
+    return (res != 0) ? r : __Pyx_NewRef(d);
+#else
+  #if CYTHON_USE_TYPE_SLOTS
     if (likely(PyString_Check(n))) {
         r = __Pyx_PyObject_GetAttrStrNoError(o, n);
         if (unlikely(!r) && likely(!PyErr_Occurred())) {
             r = __Pyx_NewRef(d);
         }
         return r;
     }
-#endif
+  #endif
     r = PyObject_GetAttr(o, n);
     return (likely(r)) ? r : __Pyx_GetAttr3Default(d);
+#endif
 }
 
 /* PyDictVersioning */
 #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_TYPE_SLOTS
 static CYTHON_INLINE PY_UINT64_T __Pyx_get_tp_dict_version(PyObject *obj) {
     PyObject *dict = Py_TYPE(obj)->tp_dict;
     return likely(dict) ? __PYX_GET_DICT_VERSION(dict) : 0;
@@ -26361,15 +26411,15 @@
 static PyObject *__Pyx__GetModuleGlobalName(PyObject *name, PY_UINT64_T *dict_version, PyObject **dict_cached_value)
 #else
 static CYTHON_INLINE PyObject *__Pyx__GetModuleGlobalName(PyObject *name)
 #endif
 {
     PyObject *result;
 #if !CYTHON_AVOID_BORROWED_REFS
-#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1 && PY_VERSION_HEX < 0x030d0000
     result = _PyDict_GetItem_KnownHash(__pyx_d, name, ((PyASCIIObject *) name)->hash);
     __PYX_UPDATE_DICT_CACHE(__pyx_d, result, *dict_cached_value, *dict_version)
     if (likely(result)) {
         return __Pyx_NewRef(result);
     } else if (unlikely(PyErr_Occurred())) {
         return NULL;
     }
@@ -26687,15 +26737,15 @@
     #endif
     empty_dict = PyDict_New();
     if (unlikely(!empty_dict))
         goto bad;
     {
         #if PY_MAJOR_VERSION >= 3
         if (level == -1) {
-            if ((1) && (strchr(__Pyx_MODULE_NAME, '.'))) {
+            if (strchr(__Pyx_MODULE_NAME, '.') != NULL) {
                 module = PyImport_ImportModuleLevelObject(
                     name, __pyx_d, empty_dict, from_list, 1);
                 if (unlikely(!module)) {
                     if (unlikely(!PyErr_ExceptionMatches(PyExc_ImportError)))
                         goto bad;
                     PyErr_Clear();
                 }
@@ -26850,24 +26900,14 @@
     } else if (PyErr_Occurred()) {
         PyErr_Clear();
     }
 #endif
     return __Pyx__ImportDottedModule(name, parts_tuple);
 }
 
-/* ssize_strlen */
-static CYTHON_INLINE Py_ssize_t __Pyx_ssize_strlen(const char *s) {
-    size_t len = strlen(s);
-    if (unlikely(len > PY_SSIZE_T_MAX)) {
-        PyErr_SetString(PyExc_OverflowError, "byte string is too long");
-        return -1;
-    }
-    return (Py_ssize_t) len;
-}
-
 /* FastTypeChecks */
 #if CYTHON_COMPILING_IN_CPYTHON
 static int __Pyx_InBases(PyTypeObject *a, PyTypeObject *b) {
     while (a) {
         a = __Pyx_PyType_GetSlot(a, tp_base, PyTypeObject*);
         if (a == b)
             return 1;
@@ -27043,19 +27083,15 @@
                     PyErr_Clear();
                 }
             }
             return sm->sq_ass_item(o, i, v);
         }
     }
 #else
-#if CYTHON_COMPILING_IN_PYPY
-    if (is_list || (PySequence_Check(o) && !PyDict_Check(o)))
-#else
-    if (is_list || PySequence_Check(o))
-#endif
+    if (is_list || !PyMapping_Check(o))
     {
         return PySequence_SetItem(o, i, v);
     }
 #endif
     return __Pyx_SetItemInt_Generic(o, PyInt_FromSsize_t(i), v);
 }
 
@@ -27112,14 +27148,15 @@
             "cannot import name %S", name);
         #endif
     }
     return value;
 }
 
 /* HasAttr */
+#if __PYX_LIMITED_VERSION_HEX < 0x030d00A1
 static CYTHON_INLINE int __Pyx_HasAttr(PyObject *o, PyObject *n) {
     PyObject *r;
     if (unlikely(!__Pyx_PyBaseString_Check(n))) {
         PyErr_SetString(PyExc_TypeError,
                         "hasattr(): attribute name must be string");
         return -1;
     }
@@ -27128,14 +27165,15 @@
         PyErr_Clear();
         return 0;
     } else {
         Py_DECREF(r);
         return 1;
     }
 }
+#endif
 
 /* DictGetItem */
 #if PY_MAJOR_VERSION >= 3 && !CYTHON_COMPILING_IN_PYPY
 static PyObject *__Pyx_PyDict_GetItem(PyObject *d, PyObject* key) {
     PyObject *value;
     value = PyDict_GetItemWithError(d, key);
     if (unlikely(!value)) {
@@ -27268,16 +27306,16 @@
         return 0;
     }
     return 0;
 }
 
 /* PyObjectCallNoArg */
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallNoArg(PyObject *func) {
-    PyObject *arg = NULL;
-    return __Pyx_PyObject_FastCall(func, (&arg)+1, 0 | __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET);
+    PyObject *arg[2] = {NULL, NULL};
+    return __Pyx_PyObject_FastCall(func, arg + 1, 0 | __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET);
 }
 
 /* PyObjectGetMethod */
 static int __Pyx_PyObject_GetMethod(PyObject *obj, PyObject *name, PyObject **method) {
     PyObject *attr;
 #if CYTHON_UNPACK_METHODS && CYTHON_COMPILING_IN_CPYTHON && CYTHON_USE_PYTYPE_LOOKUP
     __Pyx_TypeName type_name;
@@ -27463,14 +27501,17 @@
     Py_XDECREF(value1);
     Py_XDECREF(value2);
     if (decref_tuple) { Py_XDECREF(tuple); }
     return -1;
 }
 
 /* dict_iter */
+#if CYTHON_COMPILING_IN_PYPY && PY_MAJOR_VERSION >= 3
+#include <string.h>
+#endif
 static CYTHON_INLINE PyObject* __Pyx_dict_iterator(PyObject* iterable, int is_dict, PyObject* method_name,
                                                    Py_ssize_t* p_orig_length, int* p_source_is_dict) {
     is_dict = is_dict || likely(PyDict_CheckExact(iterable));
     *p_source_is_dict = is_dict;
     if (is_dict) {
 #if !CYTHON_COMPILING_IN_PYPY
         *p_orig_length = PyDict_Size(iterable);
@@ -27599,25 +27640,23 @@
     if (unlikely(!method))
         return -1;
     target->method = method;
 #if CYTHON_COMPILING_IN_CPYTHON
     #if PY_MAJOR_VERSION >= 3
     if (likely(__Pyx_TypeCheck(method, &PyMethodDescr_Type)))
     #else
-    if (likely(!PyCFunction_Check(method)))
+    if (likely(!__Pyx_CyOrPyCFunction_Check(method)))
     #endif
     {
         PyMethodDescrObject *descr = (PyMethodDescrObject*) method;
         target->func = descr->d_method->ml_meth;
         target->flag = descr->d_method->ml_flags & ~(METH_CLASS | METH_STATIC | METH_COEXIST | METH_STACKLESS);
     } else
 #endif
-#if defined(CYTHON_COMPILING_IN_PYPY)
-#elif PY_VERSION_HEX >= 0x03090000
-    if (PyCFunction_CheckExact(method))
+#if CYTHON_COMPILING_IN_PYPY
 #else
     if (PyCFunction_Check(method))
 #endif
     {
         PyObject *self;
         int self_found;
 #if CYTHON_COMPILING_IN_LIMITED_API || CYTHON_COMPILING_IN_PYPY
@@ -27665,14 +27704,152 @@
 static CYTHON_INLINE PyObject* __Pyx_PyDict_Values(PyObject* d) {
     if (PY_MAJOR_VERSION >= 3)
         return __Pyx_CallUnboundCMethod0(&__pyx_umethod_PyDict_Type_values, d);
     else
         return PyDict_Values(d);
 }
 
+/* CallUnboundCMethod1 */
+#if CYTHON_COMPILING_IN_CPYTHON
+static CYTHON_INLINE PyObject* __Pyx_CallUnboundCMethod1(__Pyx_CachedCFunction* cfunc, PyObject* self, PyObject* arg) {
+    if (likely(cfunc->func)) {
+        int flag = cfunc->flag;
+        if (flag == METH_O) {
+            return (*(cfunc->func))(self, arg);
+        } else if ((PY_VERSION_HEX >= 0x030600B1) && flag == METH_FASTCALL) {
+            #if PY_VERSION_HEX >= 0x030700A0
+                return (*(__Pyx_PyCFunctionFast)(void*)(PyCFunction)cfunc->func)(self, &arg, 1);
+            #else
+                return (*(__Pyx_PyCFunctionFastWithKeywords)(void*)(PyCFunction)cfunc->func)(self, &arg, 1, NULL);
+            #endif
+        } else if ((PY_VERSION_HEX >= 0x030700A0) && flag == (METH_FASTCALL | METH_KEYWORDS)) {
+            return (*(__Pyx_PyCFunctionFastWithKeywords)(void*)(PyCFunction)cfunc->func)(self, &arg, 1, NULL);
+        }
+    }
+    return __Pyx__CallUnboundCMethod1(cfunc, self, arg);
+}
+#endif
+static PyObject* __Pyx__CallUnboundCMethod1(__Pyx_CachedCFunction* cfunc, PyObject* self, PyObject* arg){
+    PyObject *args, *result = NULL;
+    if (unlikely(!cfunc->func && !cfunc->method) && unlikely(__Pyx_TryUnpackUnboundCMethod(cfunc) < 0)) return NULL;
+#if CYTHON_COMPILING_IN_CPYTHON
+    if (cfunc->func && (cfunc->flag & METH_VARARGS)) {
+        args = PyTuple_New(1);
+        if (unlikely(!args)) goto bad;
+        Py_INCREF(arg);
+        PyTuple_SET_ITEM(args, 0, arg);
+        if (cfunc->flag & METH_KEYWORDS)
+            result = (*(PyCFunctionWithKeywords)(void*)(PyCFunction)cfunc->func)(self, args, NULL);
+        else
+            result = (*cfunc->func)(self, args);
+    } else {
+        args = PyTuple_New(2);
+        if (unlikely(!args)) goto bad;
+        Py_INCREF(self);
+        PyTuple_SET_ITEM(args, 0, self);
+        Py_INCREF(arg);
+        PyTuple_SET_ITEM(args, 1, arg);
+        result = __Pyx_PyObject_Call(cfunc->method, args, NULL);
+    }
+#else
+    args = PyTuple_Pack(2, self, arg);
+    if (unlikely(!args)) goto bad;
+    result = __Pyx_PyObject_Call(cfunc->method, args, NULL);
+#endif
+bad:
+    Py_XDECREF(args);
+    return result;
+}
+
+/* CallUnboundCMethod2 */
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030600B1
+static CYTHON_INLINE PyObject *__Pyx_CallUnboundCMethod2(__Pyx_CachedCFunction *cfunc, PyObject *self, PyObject *arg1, PyObject *arg2) {
+    if (likely(cfunc->func)) {
+        PyObject *args[2] = {arg1, arg2};
+        if (cfunc->flag == METH_FASTCALL) {
+            #if PY_VERSION_HEX >= 0x030700A0
+            return (*(__Pyx_PyCFunctionFast)(void*)(PyCFunction)cfunc->func)(self, args, 2);
+            #else
+            return (*(__Pyx_PyCFunctionFastWithKeywords)(void*)(PyCFunction)cfunc->func)(self, args, 2, NULL);
+            #endif
+        }
+        #if PY_VERSION_HEX >= 0x030700A0
+        if (cfunc->flag == (METH_FASTCALL | METH_KEYWORDS))
+            return (*(__Pyx_PyCFunctionFastWithKeywords)(void*)(PyCFunction)cfunc->func)(self, args, 2, NULL);
+        #endif
+    }
+    return __Pyx__CallUnboundCMethod2(cfunc, self, arg1, arg2);
+}
+#endif
+static PyObject* __Pyx__CallUnboundCMethod2(__Pyx_CachedCFunction* cfunc, PyObject* self, PyObject* arg1, PyObject* arg2){
+    PyObject *args, *result = NULL;
+    if (unlikely(!cfunc->func && !cfunc->method) && unlikely(__Pyx_TryUnpackUnboundCMethod(cfunc) < 0)) return NULL;
+#if CYTHON_COMPILING_IN_CPYTHON
+    if (cfunc->func && (cfunc->flag & METH_VARARGS)) {
+        args = PyTuple_New(2);
+        if (unlikely(!args)) goto bad;
+        Py_INCREF(arg1);
+        PyTuple_SET_ITEM(args, 0, arg1);
+        Py_INCREF(arg2);
+        PyTuple_SET_ITEM(args, 1, arg2);
+        if (cfunc->flag & METH_KEYWORDS)
+            result = (*(PyCFunctionWithKeywords)(void*)(PyCFunction)cfunc->func)(self, args, NULL);
+        else
+            result = (*cfunc->func)(self, args);
+    } else {
+        args = PyTuple_New(3);
+        if (unlikely(!args)) goto bad;
+        Py_INCREF(self);
+        PyTuple_SET_ITEM(args, 0, self);
+        Py_INCREF(arg1);
+        PyTuple_SET_ITEM(args, 1, arg1);
+        Py_INCREF(arg2);
+        PyTuple_SET_ITEM(args, 2, arg2);
+        result = __Pyx_PyObject_Call(cfunc->method, args, NULL);
+    }
+#else
+    args = PyTuple_Pack(3, self, arg1, arg2);
+    if (unlikely(!args)) goto bad;
+    result = __Pyx_PyObject_Call(cfunc->method, args, NULL);
+#endif
+bad:
+    Py_XDECREF(args);
+    return result;
+}
+
+/* dict_getitem_default */
+static PyObject* __Pyx_PyDict_GetItemDefault(PyObject* d, PyObject* key, PyObject* default_value) {
+    PyObject* value;
+#if PY_MAJOR_VERSION >= 3 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07020000)
+    value = PyDict_GetItemWithError(d, key);
+    if (unlikely(!value)) {
+        if (unlikely(PyErr_Occurred()))
+            return NULL;
+        value = default_value;
+    }
+    Py_INCREF(value);
+    if ((1));
+#else
+    if (PyString_CheckExact(key) || PyUnicode_CheckExact(key) || PyInt_CheckExact(key)) {
+        value = PyDict_GetItem(d, key);
+        if (unlikely(!value)) {
+            value = default_value;
+        }
+        Py_INCREF(value);
+    }
+#endif
+    else {
+        if (default_value == Py_None)
+            value = __Pyx_CallUnboundCMethod1(&__pyx_umethod_PyDict_Type_get, d, key);
+        else
+            value = __Pyx_CallUnboundCMethod2(&__pyx_umethod_PyDict_Type_get, d, key, default_value);
+    }
+    return value;
+}
+
 /* PyObject_GenericGetAttrNoDict */
 #if CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP && PY_VERSION_HEX < 0x03070000
 static PyObject *__Pyx_RaiseGenericGetAttributeError(PyTypeObject *tp, PyObject *attr_name) {
     __Pyx_TypeName type_name = __Pyx_PyType_GetName(tp);
     PyErr_Format(PyExc_AttributeError,
 #if PY_MAJOR_VERSION >= 3
                  "'" __Pyx_FMT_TYPENAME "' object has no attribute '%U'",
@@ -27835,46 +28012,46 @@
                 "base class '" __Pyx_FMT_TYPENAME "' is not a heap type", b_name);
             __Pyx_DECREF_TypeName(b_name);
 #if CYTHON_AVOID_BORROWED_REFS
             Py_DECREF(b0);
 #endif
             return -1;
         }
-#if !CYTHON_USE_TYPE_SLOTS
-        if (dictoffset == 0) {
-            PyErr_Format(PyExc_TypeError,
-                "extension type '%s.200s': "
-                "unable to validate whether bases have a __dict__ "
-                "when CYTHON_USE_TYPE_SLOTS is off "
-                "(likely because you are building in the limited API). "
-                "Therefore, all extension types with multiple bases "
-                "must add 'cdef dict __dict__' in this compilation mode",
-                type_name);
-#if CYTHON_AVOID_BORROWED_REFS
-            Py_DECREF(b0);
-#endif
-            return -1;
-        }
-#else
-        if (dictoffset == 0 && b->tp_dictoffset)
+        if (dictoffset == 0)
         {
-            __Pyx_TypeName b_name = __Pyx_PyType_GetName(b);
-            PyErr_Format(PyExc_TypeError,
-                "extension type '%.200s' has no __dict__ slot, "
-                "but base type '" __Pyx_FMT_TYPENAME "' has: "
-                "either add 'cdef dict __dict__' to the extension type "
-                "or add '__slots__ = [...]' to the base type",
-                type_name, b_name);
-            __Pyx_DECREF_TypeName(b_name);
+            Py_ssize_t b_dictoffset = 0;
+#if CYTHON_USE_TYPE_SLOTS || CYTHON_COMPILING_IN_PYPY
+            b_dictoffset = b->tp_dictoffset;
+#else
+            PyObject *py_b_dictoffset = PyObject_GetAttrString((PyObject*)b, "__dictoffset__");
+            if (!py_b_dictoffset) goto dictoffset_return;
+            b_dictoffset = PyLong_AsSsize_t(py_b_dictoffset);
+            Py_DECREF(py_b_dictoffset);
+            if (b_dictoffset == -1 && PyErr_Occurred()) goto dictoffset_return;
+#endif
+            if (b_dictoffset) {
+                {
+                    __Pyx_TypeName b_name = __Pyx_PyType_GetName(b);
+                    PyErr_Format(PyExc_TypeError,
+                        "extension type '%.200s' has no __dict__ slot, "
+                        "but base type '" __Pyx_FMT_TYPENAME "' has: "
+                        "either add 'cdef dict __dict__' to the extension type "
+                        "or add '__slots__ = [...]' to the base type",
+                        type_name, b_name);
+                    __Pyx_DECREF_TypeName(b_name);
+                }
+#if !(CYTHON_USE_TYPE_SLOTS || CYTHON_COMPILING_IN_PYPY)
+              dictoffset_return:
+#endif
 #if CYTHON_AVOID_BORROWED_REFS
-            Py_DECREF(b0);
+                Py_DECREF(b0);
 #endif
-            return -1;
+                return -1;
+            }
         }
-#endif
 #if CYTHON_AVOID_BORROWED_REFS
         Py_DECREF(b0);
 #endif
     }
     return 0;
 }
 #endif
@@ -28160,18 +28337,18 @@
     Py_XDECREF(setstate);
     Py_XDECREF(setstate_cython);
     return ret;
 }
 #endif
 
 /* TypeImport */
-#ifndef __PYX_HAVE_RT_ImportType_3_0_2
-#define __PYX_HAVE_RT_ImportType_3_0_2
-static PyTypeObject *__Pyx_ImportType_3_0_2(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_2 check_size)
+#ifndef __PYX_HAVE_RT_ImportType_3_0_7
+#define __PYX_HAVE_RT_ImportType_3_0_7
+static PyTypeObject *__Pyx_ImportType_3_0_7(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_7 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
     Py_ssize_t itemsize;
 #if CYTHON_COMPILING_IN_LIMITED_API
     PyObject *py_basicsize;
@@ -28217,23 +28394,23 @@
     if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize+itemsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error_3_0_2 &&
+    if (check_size == __Pyx_ImportType_CheckSize_Error_3_0_7 &&
             ((size_t)basicsize > size || (size_t)(basicsize + itemsize) < size)) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd-%zd from PyObject",
             module_name, class_name, size, basicsize, basicsize+itemsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn_3_0_2 && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_3_0_7 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
@@ -28241,18 +28418,15 @@
     Py_XDECREF(result);
     return NULL;
 }
 #endif
 
 /* FetchSharedCythonModule */
 static PyObject *__Pyx_FetchSharedCythonABIModule(void) {
-    PyObject *abi_module = PyImport_AddModule((char*) __PYX_ABI_MODULE_NAME);
-    if (unlikely(!abi_module)) return NULL;
-    Py_INCREF(abi_module);
-    return abi_module;
+    return __Pyx_PyImport_AddModuleRef((char*) __PYX_ABI_MODULE_NAME);
 }
 
 /* FetchCommonType */
 static int __Pyx_VerifyCachedType(PyObject *cached_type,
                                const char *name,
                                Py_ssize_t basicsize,
                                Py_ssize_t expected_basicsize) {
@@ -28405,14 +28579,28 @@
         return vc(func, args, nargs, NULL);
     }
     return __Pyx_PyVectorcall_FastCallDict_kw(func, vc, args, nargs, kw);
 }
 #endif
 
 /* CythonFunctionShared */
+#if CYTHON_COMPILING_IN_LIMITED_API
+static CYTHON_INLINE int __Pyx__IsSameCyOrCFunction(PyObject *func, void *cfunc) {
+    if (__Pyx_CyFunction_Check(func)) {
+        return PyCFunction_GetFunction(((__pyx_CyFunctionObject*)func)->func) == (PyCFunction) cfunc;
+    } else if (PyCFunction_Check(func)) {
+        return PyCFunction_GetFunction(func) == (PyCFunction) cfunc;
+    }
+    return 0;
+}
+#else
+static CYTHON_INLINE int __Pyx__IsSameCyOrCFunction(PyObject *func, void *cfunc) {
+    return __Pyx_CyOrPyCFunction_Check(func) && __Pyx_CyOrPyCFunction_GET_FUNCTION(func) == (PyCFunction) cfunc;
+}
+#endif
 static CYTHON_INLINE void __Pyx__CyFunction_SetClassObj(__pyx_CyFunctionObject* f, PyObject* classobj) {
 #if PY_VERSION_HEX < 0x030900B1 || CYTHON_COMPILING_IN_LIMITED_API
     __Pyx_Py_XDECREF_SET(
         __Pyx_CyFunction_GetClassObj(f),
             ((classobj) ? __Pyx_NewRef(classobj) : NULL));
 #else
     __Pyx_Py_XDECREF_SET(
@@ -29898,16 +30086,16 @@
     replace = PyObject_GetAttrString(code, "replace");
     if (likely(replace)) {
         PyObject *result;
         result = PyObject_Call(replace, __pyx_empty_tuple, scratch_dict);
         Py_DECREF(replace);
         return result;
     }
-    #if __PYX_LIMITED_VERSION_HEX < 0x030780000
     PyErr_Clear();
+    #if __PYX_LIMITED_VERSION_HEX < 0x030780000
     {
         PyObject *compiled = NULL, *result = NULL;
         if (unlikely(PyDict_SetItemString(scratch_dict, "code", code))) return NULL;
         if (unlikely(PyDict_SetItemString(scratch_dict, "type", (PyObject*)(&PyType_Type)))) return NULL;
         compiled = Py_CompileString(
             "out = type(code)(\n"
             "  code.co_argcount, code.co_kwonlyargcount, code.co_nlocals, code.co_stacksize,\n"
@@ -29919,14 +30107,16 @@
         Py_DECREF(compiled);
         if (!result) PyErr_Print();
         Py_DECREF(result);
         result = PyDict_GetItemString(scratch_dict, "out");
         if (result) Py_INCREF(result);
         return result;
     }
+    #else
+    return NULL;
     #endif
 }
 static void __Pyx_AddTraceback(const char *funcname, int c_line,
                                int py_line, const char *filename) {
     PyObject *code_object = NULL, *py_py_line = NULL, *py_funcname = NULL, *dict = NULL;
     PyObject *replace = NULL, *getframe = NULL, *frame = NULL;
     PyObject *exc_type, *exc_value, *exc_traceback;
@@ -30986,14 +31176,83 @@
     return result;
 __pyx_fail:
     result.memview = NULL;
     result.data = NULL;
     return result;
 }
 
+/* PyUCS4InUnicode */
+  #if PY_VERSION_HEX < 0x03090000 || (defined(PyUnicode_WCHAR_KIND) && defined(PyUnicode_AS_UNICODE))
+#if PY_VERSION_HEX < 0x03090000
+#define __Pyx_PyUnicode_AS_UNICODE(op) PyUnicode_AS_UNICODE(op)
+#define __Pyx_PyUnicode_GET_SIZE(op) PyUnicode_GET_SIZE(op)
+#else
+#define __Pyx_PyUnicode_AS_UNICODE(op) (((PyASCIIObject *)(op))->wstr)
+#define __Pyx_PyUnicode_GET_SIZE(op) ((PyCompactUnicodeObject *)(op))->wstr_length
+#endif
+#if !defined(Py_UNICODE_SIZE) || Py_UNICODE_SIZE == 2
+static int __Pyx_PyUnicodeBufferContainsUCS4_SP(Py_UNICODE* buffer, Py_ssize_t length, Py_UCS4 character) {
+    Py_UNICODE high_val, low_val;
+    Py_UNICODE* pos;
+    high_val = (Py_UNICODE) (0xD800 | (((character - 0x10000) >> 10) & ((1<<10)-1)));
+    low_val  = (Py_UNICODE) (0xDC00 | ( (character - 0x10000)        & ((1<<10)-1)));
+    for (pos=buffer; pos < buffer+length-1; pos++) {
+        if (unlikely((high_val == pos[0]) & (low_val == pos[1]))) return 1;
+    }
+    return 0;
+}
+#endif
+static int __Pyx_PyUnicodeBufferContainsUCS4_BMP(Py_UNICODE* buffer, Py_ssize_t length, Py_UCS4 character) {
+    Py_UNICODE uchar;
+    Py_UNICODE* pos;
+    uchar = (Py_UNICODE) character;
+    for (pos=buffer; pos < buffer+length; pos++) {
+        if (unlikely(uchar == pos[0])) return 1;
+    }
+    return 0;
+}
+#endif
+static CYTHON_INLINE int __Pyx_UnicodeContainsUCS4(PyObject* unicode, Py_UCS4 character) {
+#if CYTHON_PEP393_ENABLED
+    const int kind = PyUnicode_KIND(unicode);
+    #ifdef PyUnicode_WCHAR_KIND
+    if (likely(kind != PyUnicode_WCHAR_KIND))
+    #endif
+    {
+        Py_ssize_t i;
+        const void* udata = PyUnicode_DATA(unicode);
+        const Py_ssize_t length = PyUnicode_GET_LENGTH(unicode);
+        for (i=0; i < length; i++) {
+            if (unlikely(character == PyUnicode_READ(kind, udata, i))) return 1;
+        }
+        return 0;
+    }
+#elif PY_VERSION_HEX >= 0x03090000
+    #error Cannot use "UChar in Unicode" in Python 3.9 without PEP-393 unicode strings.
+#elif !defined(PyUnicode_AS_UNICODE)
+    #error Cannot use "UChar in Unicode" in Python < 3.9 without Py_UNICODE support.
+#endif
+#if PY_VERSION_HEX < 0x03090000 || (defined(PyUnicode_WCHAR_KIND) && defined(PyUnicode_AS_UNICODE))
+#if !defined(Py_UNICODE_SIZE) || Py_UNICODE_SIZE == 2
+    if ((sizeof(Py_UNICODE) == 2) && unlikely(character > 65535)) {
+        return __Pyx_PyUnicodeBufferContainsUCS4_SP(
+            __Pyx_PyUnicode_AS_UNICODE(unicode),
+            __Pyx_PyUnicode_GET_SIZE(unicode),
+            character);
+    } else
+#endif
+    {
+        return __Pyx_PyUnicodeBufferContainsUCS4_BMP(
+            __Pyx_PyUnicode_AS_UNICODE(unicode),
+            __Pyx_PyUnicode_GET_SIZE(unicode),
+            character);
+    }
+#endif
+}
+
 /* CIntFromPyVerify */
   #define __PYX_VERIFY_RETURN_INT(target_type, func_type, func_value)\
     __PYX__VERIFY_RETURN_INT(target_type, func_type, func_value, 0)
 #define __PYX_VERIFY_RETURN_INT_EXC(target_type, func_type, func_value)\
     __PYX__VERIFY_RETURN_INT(target_type, func_type, func_value, 1)
 #define __PYX__VERIFY_RETURN_INT(target_type, func_type, func_value, exc)\
     {\
@@ -31551,50 +31810,45 @@
             return PyLong_FromLongLong((PY_LONG_LONG) value);
 #endif
         }
     }
     {
         int one = 1; int little = (int)*(unsigned char *)&one;
         unsigned char *bytes = (unsigned char *)&value;
-#if !CYTHON_COMPILING_IN_LIMITED_API
+#if !CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030d0000
         return _PyLong_FromByteArray(bytes, sizeof(long),
                                      little, !is_unsigned);
 #else
         PyObject *from_bytes, *result = NULL;
         PyObject *py_bytes = NULL, *arg_tuple = NULL, *kwds = NULL, *order_str = NULL;
-        from_bytes = PyObject_GetAttrString((PyObject*)&PyInt_Type, "from_bytes");
+        from_bytes = PyObject_GetAttrString((PyObject*)&PyLong_Type, "from_bytes");
         if (!from_bytes) return NULL;
         py_bytes = PyBytes_FromStringAndSize((char*)bytes, sizeof(long));
         if (!py_bytes) goto limited_bad;
         order_str = PyUnicode_FromString(little ? "little" : "big");
         if (!order_str) goto limited_bad;
         arg_tuple = PyTuple_Pack(2, py_bytes, order_str);
         if (!arg_tuple) goto limited_bad;
-        kwds = PyDict_New();
-        if (!kwds) goto limited_bad;
-        if (PyDict_SetItemString(kwds, "signed", __Pyx_NewRef(!is_unsigned ? Py_True : Py_False))) goto limited_bad;
+        if (!is_unsigned) {
+            kwds = PyDict_New();
+            if (!kwds) goto limited_bad;
+            if (PyDict_SetItemString(kwds, "signed", __Pyx_NewRef(Py_True))) goto limited_bad;
+        }
         result = PyObject_Call(from_bytes, arg_tuple, kwds);
         limited_bad:
-        Py_XDECREF(from_bytes);
-        Py_XDECREF(py_bytes);
-        Py_XDECREF(order_str);
-        Py_XDECREF(arg_tuple);
         Py_XDECREF(kwds);
+        Py_XDECREF(arg_tuple);
+        Py_XDECREF(order_str);
+        Py_XDECREF(py_bytes);
+        Py_XDECREF(from_bytes);
         return result;
 #endif
     }
 }
 
-/* BytesContains */
-  static CYTHON_INLINE int __Pyx_BytesContains(PyObject* bytes, char character) {
-    const Py_ssize_t length = PyBytes_GET_SIZE(bytes);
-    char* char_start = PyBytes_AS_STRING(bytes);
-    return memchr(char_start, (unsigned char)character, (size_t)length) != NULL;
-}
-
 /* CIntFromPy */
   static CYTHON_INLINE npy_int8 __Pyx_PyInt_As_npy_int8(PyObject *x) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const npy_int8 neg_one = (npy_int8) -1, const_zero = (npy_int8) 0;
@@ -31757,15 +32011,15 @@
                 PyObject *tmp = v;
                 v = PyNumber_Long(tmp);
                 Py_DECREF(tmp);
             }
 #endif
             if (likely(v)) {
                 int ret = -1;
-#if !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
+#if PY_VERSION_HEX < 0x030d0000 && !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
                 int one = 1; int is_little = (int)*(unsigned char *)&one;
                 unsigned char *bytes = (unsigned char *)&val;
                 ret = _PyLong_AsByteArray((PyLongObject *)v,
                                            bytes, sizeof(val),
                                            is_little, !is_unsigned);
 #else
                 PyObject *stepval = NULL, *mask = NULL, *shift = NULL;
@@ -32030,15 +32284,15 @@
                 PyObject *tmp = v;
                 v = PyNumber_Long(tmp);
                 Py_DECREF(tmp);
             }
 #endif
             if (likely(v)) {
                 int ret = -1;
-#if !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
+#if PY_VERSION_HEX < 0x030d0000 && !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
                 int one = 1; int is_little = (int)*(unsigned char *)&one;
                 unsigned char *bytes = (unsigned char *)&val;
                 ret = _PyLong_AsByteArray((PyLongObject *)v,
                                            bytes, sizeof(val),
                                            is_little, !is_unsigned);
 #else
                 PyObject *stepval = NULL, *mask = NULL, *shift = NULL;
@@ -32303,15 +32557,15 @@
                 PyObject *tmp = v;
                 v = PyNumber_Long(tmp);
                 Py_DECREF(tmp);
             }
 #endif
             if (likely(v)) {
                 int ret = -1;
-#if !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
+#if PY_VERSION_HEX < 0x030d0000 && !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
                 int one = 1; int is_little = (int)*(unsigned char *)&one;
                 unsigned char *bytes = (unsigned char *)&val;
                 ret = _PyLong_AsByteArray((PyLongObject *)v,
                                            bytes, sizeof(val),
                                            is_little, !is_unsigned);
 #else
                 PyObject *stepval = NULL, *mask = NULL, *shift = NULL;
@@ -32576,15 +32830,15 @@
                 PyObject *tmp = v;
                 v = PyNumber_Long(tmp);
                 Py_DECREF(tmp);
             }
 #endif
             if (likely(v)) {
                 int ret = -1;
-#if !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
+#if PY_VERSION_HEX < 0x030d0000 && !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
                 int one = 1; int is_little = (int)*(unsigned char *)&one;
                 unsigned char *bytes = (unsigned char *)&val;
                 ret = _PyLong_AsByteArray((PyLongObject *)v,
                                            bytes, sizeof(val),
                                            is_little, !is_unsigned);
 #else
                 PyObject *stepval = NULL, *mask = NULL, *shift = NULL;
@@ -32875,15 +33129,15 @@
                 PyObject *tmp = v;
                 v = PyNumber_Long(tmp);
                 Py_DECREF(tmp);
             }
 #endif
             if (likely(v)) {
                 int ret = -1;
-#if !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
+#if PY_VERSION_HEX < 0x030d0000 && !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
                 int one = 1; int is_little = (int)*(unsigned char *)&one;
                 unsigned char *bytes = (unsigned char *)&val;
                 ret = _PyLong_AsByteArray((PyLongObject *)v,
                                            bytes, sizeof(val),
                                            is_little, !is_unsigned);
 #else
                 PyObject *stepval = NULL, *mask = NULL, *shift = NULL;
@@ -33148,15 +33402,15 @@
                 PyObject *tmp = v;
                 v = PyNumber_Long(tmp);
                 Py_DECREF(tmp);
             }
 #endif
             if (likely(v)) {
                 int ret = -1;
-#if !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
+#if PY_VERSION_HEX < 0x030d0000 && !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
                 int one = 1; int is_little = (int)*(unsigned char *)&one;
                 unsigned char *bytes = (unsigned char *)&val;
                 ret = _PyLong_AsByteArray((PyLongObject *)v,
                                            bytes, sizeof(val),
                                            is_little, !is_unsigned);
 #else
                 PyObject *stepval = NULL, *mask = NULL, *shift = NULL;
@@ -33284,38 +33538,40 @@
             return PyLong_FromLongLong((PY_LONG_LONG) value);
 #endif
         }
     }
     {
         int one = 1; int little = (int)*(unsigned char *)&one;
         unsigned char *bytes = (unsigned char *)&value;
-#if !CYTHON_COMPILING_IN_LIMITED_API
+#if !CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030d0000
         return _PyLong_FromByteArray(bytes, sizeof(int),
                                      little, !is_unsigned);
 #else
         PyObject *from_bytes, *result = NULL;
         PyObject *py_bytes = NULL, *arg_tuple = NULL, *kwds = NULL, *order_str = NULL;
-        from_bytes = PyObject_GetAttrString((PyObject*)&PyInt_Type, "from_bytes");
+        from_bytes = PyObject_GetAttrString((PyObject*)&PyLong_Type, "from_bytes");
         if (!from_bytes) return NULL;
         py_bytes = PyBytes_FromStringAndSize((char*)bytes, sizeof(int));
         if (!py_bytes) goto limited_bad;
         order_str = PyUnicode_FromString(little ? "little" : "big");
         if (!order_str) goto limited_bad;
         arg_tuple = PyTuple_Pack(2, py_bytes, order_str);
         if (!arg_tuple) goto limited_bad;
-        kwds = PyDict_New();
-        if (!kwds) goto limited_bad;
-        if (PyDict_SetItemString(kwds, "signed", __Pyx_NewRef(!is_unsigned ? Py_True : Py_False))) goto limited_bad;
+        if (!is_unsigned) {
+            kwds = PyDict_New();
+            if (!kwds) goto limited_bad;
+            if (PyDict_SetItemString(kwds, "signed", __Pyx_NewRef(Py_True))) goto limited_bad;
+        }
         result = PyObject_Call(from_bytes, arg_tuple, kwds);
         limited_bad:
-        Py_XDECREF(from_bytes);
-        Py_XDECREF(py_bytes);
-        Py_XDECREF(order_str);
-        Py_XDECREF(arg_tuple);
         Py_XDECREF(kwds);
+        Py_XDECREF(arg_tuple);
+        Py_XDECREF(order_str);
+        Py_XDECREF(py_bytes);
+        Py_XDECREF(from_bytes);
         return result;
 #endif
     }
 }
 
 /* CIntFromPy */
   static CYTHON_INLINE char __Pyx_PyInt_As_char(PyObject *x) {
@@ -33483,15 +33739,15 @@
                 PyObject *tmp = v;
                 v = PyNumber_Long(tmp);
                 Py_DECREF(tmp);
             }
 #endif
             if (likely(v)) {
                 int ret = -1;
-#if !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
+#if PY_VERSION_HEX < 0x030d0000 && !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
                 int one = 1; int is_little = (int)*(unsigned char *)&one;
                 unsigned char *bytes = (unsigned char *)&val;
                 ret = _PyLong_AsByteArray((PyLongObject *)v,
                                            bytes, sizeof(val),
                                            is_little, !is_unsigned);
 #else
                 PyObject *stepval = NULL, *mask = NULL, *shift = NULL;
@@ -33603,49 +33859,58 @@
         name = __Pyx_NewRef(__pyx_n_s__28);
     }
     return name;
 }
 #endif
 
 /* CheckBinaryVersion */
-  static int __Pyx_check_binary_version(void) {
-    char ctversion[5];
-    int same=1, i, found_dot;
-    const char* rt_from_call = Py_GetVersion();
-    PyOS_snprintf(ctversion, 5, "%d.%d", PY_MAJOR_VERSION, PY_MINOR_VERSION);
-    found_dot = 0;
-    for (i = 0; i < 4; i++) {
-        if (!ctversion[i]) {
-            same = (rt_from_call[i] < '0' || rt_from_call[i] > '9');
-            break;
+  static unsigned long __Pyx_get_runtime_version(void) {
+#if __PYX_LIMITED_VERSION_HEX >= 0x030B00A4
+    return Py_Version & ~0xFFUL;
+#else
+    const char* rt_version = Py_GetVersion();
+    unsigned long version = 0;
+    unsigned long factor = 0x01000000UL;
+    unsigned int digit = 0;
+    int i = 0;
+    while (factor) {
+        while ('0' <= rt_version[i] && rt_version[i] <= '9') {
+            digit = digit * 10 + (unsigned int) (rt_version[i] - '0');
+            ++i;
         }
-        if (rt_from_call[i] != ctversion[i]) {
-            same = 0;
+        version += factor * digit;
+        if (rt_version[i] != '.')
             break;
-        }
+        digit = 0;
+        factor >>= 8;
+        ++i;
     }
-    if (!same) {
-        char rtversion[5] = {'\0'};
+    return version;
+#endif
+}
+static int __Pyx_check_binary_version(unsigned long ct_version, unsigned long rt_version, int allow_newer) {
+    const unsigned long MAJOR_MINOR = 0xFFFF0000UL;
+    if ((rt_version & MAJOR_MINOR) == (ct_version & MAJOR_MINOR))
+        return 0;
+    if (likely(allow_newer && (rt_version & MAJOR_MINOR) > (ct_version & MAJOR_MINOR)))
+        return 1;
+    {
         char message[200];
-        for (i=0; i<4; ++i) {
-            if (rt_from_call[i] == '.') {
-                if (found_dot) break;
-                found_dot = 1;
-            } else if (rt_from_call[i] < '0' || rt_from_call[i] > '9') {
-                break;
-            }
-            rtversion[i] = rt_from_call[i];
-        }
         PyOS_snprintf(message, sizeof(message),
-                      "compile time version %s of module '%.100s' "
-                      "does not match runtime version %s",
-                      ctversion, __Pyx_MODULE_NAME, rtversion);
+                      "compile time Python version %d.%d "
+                      "of module '%.100s' "
+                      "%s "
+                      "runtime version %d.%d",
+                       (int) (ct_version >> 24), (int) ((ct_version >> 16) & 0xFF),
+                       __Pyx_MODULE_NAME,
+                       (allow_newer) ? "was newer than" : "does not match",
+                       (int) (rt_version >> 24), (int) ((rt_version >> 16) & 0xFF)
+       );
         return PyErr_WarnEx(NULL, message, 1);
     }
-    return 0;
 }
 
 /* InitStrings */
   #if PY_MAJOR_VERSION >= 3
 static int __Pyx_InitString(__Pyx_StringTabEntry t, PyObject **str) {
     if (t.is_unicode | t.is_str) {
         if (t.intern) {
@@ -33683,16 +33948,32 @@
             return -1;
         #endif
         ++t;
     }
     return 0;
 }
 
+#include <string.h>
+static CYTHON_INLINE Py_ssize_t __Pyx_ssize_strlen(const char *s) {
+    size_t len = strlen(s);
+    if (unlikely(len > (size_t) PY_SSIZE_T_MAX)) {
+        PyErr_SetString(PyExc_OverflowError, "byte string is too long");
+        return -1;
+    }
+    return (Py_ssize_t) len;
+}
 static CYTHON_INLINE PyObject* __Pyx_PyUnicode_FromString(const char* c_str) {
-    return __Pyx_PyUnicode_FromStringAndSize(c_str, (Py_ssize_t)strlen(c_str));
+    Py_ssize_t len = __Pyx_ssize_strlen(c_str);
+    if (unlikely(len < 0)) return NULL;
+    return __Pyx_PyUnicode_FromStringAndSize(c_str, len);
+}
+static CYTHON_INLINE PyObject* __Pyx_PyByteArray_FromString(const char* c_str) {
+    Py_ssize_t len = __Pyx_ssize_strlen(c_str);
+    if (unlikely(len < 0)) return NULL;
+    return PyByteArray_FromStringAndSize(c_str, len);
 }
 static CYTHON_INLINE const char* __Pyx_PyObject_AsString(PyObject* o) {
     Py_ssize_t ignore;
     return __Pyx_PyObject_AsStringAndSize(o, &ignore);
 }
 #if __PYX_DEFAULT_STRING_ENCODING_IS_ASCII || __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT
 #if !CYTHON_PEP393_ENABLED
```

### Comparing `linearmodels-5.3/linearmodels/panel/_utility.pyx` & `linearmodels-5.4/linearmodels/panel/_utility.pyx`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/linearmodels/panel/covariance.py` & `linearmodels-5.4/linearmodels/panel/covariance.py`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/linearmodels/panel/data.py` & `linearmodels-5.4/linearmodels/panel/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from __future__ import annotations
 
+from linearmodels.compat.pandas import PD_GTE_21
+
 from collections.abc import Hashable, Sequence
 from itertools import product
 from typing import Literal, Union, cast, overload
 
 import numpy as np
 from numpy.linalg import lstsq
 import pandas as pd
@@ -223,15 +225,16 @@
                 if isinstance(self._original, (DataFrame, PanelData, Series)):
                     for i in range(2):
                         index_names[i] = x.index.levels[i].name or index_names[i]
                 self._frame = x
                 if copy:
                     self._frame = self._frame.copy()
             else:
-                self._frame = DataFrame({var_name: x.T.stack(dropna=False)})
+                options = {"future_stack": True} if PD_GTE_21 else {"dropna": False}
+                self._frame = DataFrame({var_name: x.T.stack(**options)})
         elif isinstance(x, np.ndarray):
             if x.ndim not in (2, 3):
                 raise ValueError("2 or 3-d array required for numpy input")
             if x.ndim == 2:
                 x = x[None, :, :]
 
             k, t, n = x.shape
@@ -294,14 +297,16 @@
 
         Parameters
         ----------
         locs : ndarray
             Boolean array indicating observations to drop with reference to
             the dataframe view of the data
         """
+        if isinstance(locs, Series):
+            locs = np.asarray(locs)
         self._frame = self._frame.loc[~locs.ravel()]
         self._frame = self._minimize_multiindex(self._frame)
         # Reset panel and shape after a drop
         self._panel = self._shape = None
         self._k, self._t, self._n = self.shape
 
     @property
```

### Comparing `linearmodels-5.3/linearmodels/panel/model.py` & `linearmodels-5.4/linearmodels/panel/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1874,15 +1874,17 @@
                         stacklevel=2,
                     )
                     x = x[:, retain]
                     # Update constant index loc
                     if self._constant:
                         assert isinstance(self._constant_index, int)
                         self._constant_index = int(
-                            np.argwhere(np.array(retain) == self._constant_index)
+                            np.squeeze(
+                                np.argwhere(np.array(retain) == self._constant_index)
+                            )
                         )
 
                     # Adjust exog
                     self.exog = PanelData(self.exog.dataframe.iloc[:, retain])
                     x_effects = x_effects[:, retain]
 
         params = _lstsq(x, y, rcond=None)[0]
```

### Comparing `linearmodels-5.3/linearmodels/panel/results.py` & `linearmodels-5.4/linearmodels/panel/results.py`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/linearmodels/panel/utility.py` & `linearmodels-5.4/linearmodels/panel/utility.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from __future__ import annotations
 
+from linearmodels.compat.pandas import ANNUAL_FREQ
+
 from collections import defaultdict
 from typing import NamedTuple, TypeVar, cast
 
 import numpy as np
 from pandas import DataFrame, concat, date_range
 import scipy.sparse as sp
 
@@ -609,15 +611,15 @@
     if missing > 0:
         locs = rng.choice(n * t, int(n * t * missing))
         y.flat[locs] = np.nan
         locs = rng.choice(n * t * k, int(n * t * k * missing))
         x.flat[locs] = np.nan
 
     entities = [f"firm{i}" for i in range(n)]
-    time = [dt for dt in date_range("1-1-1900", periods=t, freq="A-DEC")]
+    time = [dt for dt in date_range("1-1-1900", periods=t, freq=ANNUAL_FREQ)]
     var_names = [f"x{i}" for i in range(k)]
     if const:
         var_names[1:] = var_names[:-1]
         var_names[0] = "const"
     # y = DataFrame(y, index=time, columns=entities)
     y_df = panel_to_frame(
         y[None], items=["y"], major_axis=time, minor_axis=entities, swap=True
```

### Comparing `linearmodels-5.3/linearmodels/shared/base.py` & `linearmodels-5.4/linearmodels/shared/base.py`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/linearmodels/shared/covariance.py` & `linearmodels-5.4/linearmodels/shared/covariance.py`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/linearmodels/shared/exceptions.py` & `linearmodels-5.4/linearmodels/shared/exceptions.py`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/linearmodels/shared/hypotheses.py` & `linearmodels-5.4/linearmodels/shared/hypotheses.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,21 +113,21 @@
     See Also
     --------
     WaldTestStatistic
     """
 
     def __init__(self, reason: str, *, name: str | None = None) -> None:
         self._reason = reason
-        super().__init__(np.NaN, "", df=1, df_denom=1, name=name)
+        super().__init__(np.nan, "", df=1, df_denom=1, name=name)
         self.dist_name = "None"
 
     @property
     def pval(self) -> float:
-        """Always returns np.NaN"""
-        return np.NaN
+        """Always returns np.nan"""
+        return np.nan
 
     @property
     def critical_values(self) -> None:
         """Always returns None"""
         return None
 
     def __str__(self) -> str:
@@ -154,21 +154,21 @@
     """
 
     def __init__(self, *, reason: str | None = None, name: str | None = None):
         self._reason = reason
         if reason is None:
             self._reason = "Test is not applicable to model specification"
 
-        super().__init__(np.NaN, "", df=1, df_denom=1, name=name)
+        super().__init__(np.nan, "", df=1, df_denom=1, name=name)
         self.dist_name = "None"
 
     @property
     def pval(self) -> float:
-        """Always returns np.NaN"""
-        return np.NaN
+        """Always returns np.nan"""
+        return np.nan
 
     @property
     def critical_values(self) -> None:
         """Always returns None"""
         return None
 
     def __str__(self) -> str:
```

### Comparing `linearmodels-5.3/linearmodels/shared/io.py` & `linearmodels-5.4/linearmodels/shared/io.py`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/linearmodels/shared/linalg.py` & `linearmodels-5.4/linearmodels/shared/linalg.py`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/linearmodels/shared/typed_getters.py` & `linearmodels-5.4/linearmodels/shared/typed_getters.py`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/linearmodels/shared/utility.py` & `linearmodels-5.4/linearmodels/shared/utility.py`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/linearmodels/system/_utility.py` & `linearmodels-5.4/linearmodels/system/_utility.py`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/linearmodels/system/covariance.py` & `linearmodels-5.4/linearmodels/system/covariance.py`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/linearmodels/system/gmm.py` & `linearmodels-5.4/linearmodels/system/gmm.py`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/linearmodels/system/model.py` & `linearmodels-5.4/linearmodels/system/model.py`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/linearmodels/system/results.py` & `linearmodels-5.4/linearmodels/system/results.py`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/linearmodels/tests/asset_pricing/_utility.py` & `linearmodels-5.4/linearmodels/tests/asset_pricing/_utility.py`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/linearmodels/tests/asset_pricing/test_covariance.py` & `linearmodels-5.4/linearmodels/tests/asset_pricing/test_covariance.py`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/linearmodels/tests/asset_pricing/test_formulas.py` & `linearmodels-5.4/linearmodels/tests/asset_pricing/test_formulas.py`

 * *Files 0% similar despite different names*

```diff
@@ -113,15 +113,15 @@
 
     with pytest.raises(ValueError, match="tarting values"):
         mod2.fit(starting=sv[:-3], opt_options=oo, disp=0)
 
 
 def test_escaped_formula(data, model):
     def transform(fmla):
-        names = [f"`{factor.strip().replace('_',' ')}`" for factor in fmla.split("+")]
+        names = [f"`{factor.strip().replace('_', ' ')}`" for factor in fmla.split("+")]
         return " + ".join(names)
 
     formula_factors = transform(FORMULA_FACTORS)
     formula_port = transform(FORMULA_PORT)
     formula = " ~ ".join((formula_port, formula_factors))
     data_rename = data.joined.copy()
     data_rename.columns = [col.replace("_", " ") for col in data_rename]
```

### Comparing `linearmodels-5.3/linearmodels/tests/asset_pricing/test_linear_factor_gmm.py` & `linearmodels-5.4/linearmodels/tests/asset_pricing/test_linear_factor_gmm.py`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/linearmodels/tests/asset_pricing/test_linear_factor_model.py` & `linearmodels-5.4/linearmodels/tests/asset_pricing/test_linear_factor_model.py`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/linearmodels/tests/asset_pricing/test_model.py` & `linearmodels-5.4/linearmodels/tests/asset_pricing/test_model.py`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/linearmodels/tests/datasets/test_datasets.py` & `linearmodels-5.4/linearmodels/tests/datasets/test_datasets.py`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/linearmodels/tests/iv/_utility.py` & `linearmodels-5.4/linearmodels/tests/iv/_utility.py`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/linearmodels/tests/iv/results/execute-stata-simulated-data.py` & `linearmodels-5.4/linearmodels/tests/iv/results/execute-stata-simulated-data.py`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/linearmodels/tests/iv/results/execute-stata.py` & `linearmodels-5.4/linearmodels/tests/iv/results/execute-stata.py`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/linearmodels/tests/iv/results/housing.csv` & `linearmodels-5.4/linearmodels/tests/iv/results/housing.csv`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/linearmodels/tests/iv/results/read_stata_results.py` & `linearmodels-5.4/linearmodels/tests/iv/results/read_stata_results.py`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/linearmodels/tests/iv/results/simulated-data.dta` & `linearmodels-5.4/linearmodels/tests/iv/results/simulated-data.dta`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/linearmodels/tests/iv/results/simulated-test-data.py` & `linearmodels-5.4/linearmodels/tests/iv/results/simulated-test-data.py`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/linearmodels/tests/iv/results/stata-iv-housing-results.txt` & `linearmodels-5.4/linearmodels/tests/iv/results/stata-iv-housing-results.txt`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/linearmodels/tests/iv/results/stata-iv-simulated-results.txt` & `linearmodels-5.4/linearmodels/tests/iv/results/stata-iv-simulated-results.txt`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/linearmodels/tests/iv/test_absorbing.py` & `linearmodels-5.4/linearmodels/tests/iv/test_absorbing.py`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/linearmodels/tests/iv/test_against_stata.py` & `linearmodels-5.4/linearmodels/tests/iv/test_against_stata.py`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/linearmodels/tests/iv/test_covariance.py` & `linearmodels-5.4/linearmodels/tests/iv/test_covariance.py`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/linearmodels/tests/iv/test_data.py` & `linearmodels-5.4/linearmodels/tests/iv/test_data.py`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/linearmodels/tests/iv/test_formulas.py` & `linearmodels-5.4/linearmodels/tests/iv/test_formulas.py`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/linearmodels/tests/iv/test_gmm.py` & `linearmodels-5.4/linearmodels/tests/iv/test_gmm.py`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/linearmodels/tests/iv/test_missing_data.py` & `linearmodels-5.4/linearmodels/tests/iv/test_missing_data.py`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/linearmodels/tests/iv/test_model.py` & `linearmodels-5.4/linearmodels/tests/iv/test_model.py`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/linearmodels/tests/iv/test_postestimation.py` & `linearmodels-5.4/linearmodels/tests/iv/test_postestimation.py`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/linearmodels/tests/iv/test_results.py` & `linearmodels-5.4/linearmodels/tests/iv/test_results.py`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/linearmodels/tests/panel/_utility.py` & `linearmodels-5.4/linearmodels/tests/panel/_utility.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from __future__ import annotations
 
+from linearmodels.compat.pandas import ANNUAL_FREQ
+
 from typing import Literal
 
 import numpy as np
 from numpy.linalg import lstsq
 from numpy.random import RandomState, standard_normal
 from numpy.testing import assert_allclose
 from pandas import Categorical, DataFrame, Series, date_range, get_dummies
@@ -117,15 +119,15 @@
         x.flat[locs] = float(np.nan)
     if rng is not None:
         rng.set_state(np.random.get_state())
     if datatype == "numpy":
         return AttrDict(y=y, x=x, w=w, c=c, vc1=vc1, vc2=vc2)
 
     entities = ["firm" + str(i) for i in range(n)]
-    time = date_range("1-1-1900", periods=t, freq="A-DEC")
+    time = date_range("1-1-1900", periods=t, freq=ANNUAL_FREQ)
     var_names = ["x" + str(i) for i in range(k)]
     # y = DataFrame(y, index=time, columns=entities)
     y_df = panel_to_frame(
         y[None], items=["y"], major_axis=time, minor_axis=entities, swap=True
     )
     w_df = panel_to_frame(
         w[None], items=["w"], major_axis=time, minor_axis=entities, swap=True
```

### Comparing `linearmodels-5.3/linearmodels/tests/panel/results/execute-stata-simulated-data.py` & `linearmodels-5.4/linearmodels/tests/panel/results/execute-stata-simulated-data.py`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/linearmodels/tests/panel/results/generate-panel-data.py` & `linearmodels-5.4/linearmodels/tests/panel/results/generate-panel-data.py`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/linearmodels/tests/panel/results/parse_stata_results.py` & `linearmodels-5.4/linearmodels/tests/panel/results/parse_stata_results.py`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/linearmodels/tests/panel/results/simulated-panel.dta` & `linearmodels-5.4/linearmodels/tests/panel/results/simulated-panel.dta`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/linearmodels/tests/panel/results/stata-panel-simulated-results.txt` & `linearmodels-5.4/linearmodels/tests/panel/results/stata-panel-simulated-results.txt`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/linearmodels/tests/panel/test_between_ols.py` & `linearmodels-5.4/linearmodels/tests/panel/test_between_ols.py`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/linearmodels/tests/panel/test_cluster_input_formats.py` & `linearmodels-5.4/linearmodels/tests/panel/test_cluster_input_formats.py`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/linearmodels/tests/panel/test_data.py` & `linearmodels-5.4/linearmodels/tests/panel/test_data.py`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/linearmodels/tests/panel/test_fama_macbeth.py` & `linearmodels-5.4/linearmodels/tests/panel/test_fama_macbeth.py`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/linearmodels/tests/panel/test_firstdifference_ols.py` & `linearmodels-5.4/linearmodels/tests/panel/test_firstdifference_ols.py`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/linearmodels/tests/panel/test_formula.py` & `linearmodels-5.4/linearmodels/tests/panel/test_formula.py`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/linearmodels/tests/panel/test_model.py` & `linearmodels-5.4/linearmodels/tests/panel/test_model.py`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/linearmodels/tests/panel/test_panel_covariance.py` & `linearmodels-5.4/linearmodels/tests/panel/test_panel_covariance.py`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/linearmodels/tests/panel/test_panel_ols.py` & `linearmodels-5.4/linearmodels/tests/panel/test_panel_ols.py`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/linearmodels/tests/panel/test_pooled_ols.py` & `linearmodels-5.4/linearmodels/tests/panel/test_pooled_ols.py`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/linearmodels/tests/panel/test_random_effects.py` & `linearmodels-5.4/linearmodels/tests/panel/test_random_effects.py`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/linearmodels/tests/panel/test_results.py` & `linearmodels-5.4/linearmodels/tests/panel/test_results.py`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/linearmodels/tests/panel/test_simulated_against_stata.py` & `linearmodels-5.4/linearmodels/tests/panel/test_simulated_against_stata.py`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/linearmodels/tests/panel/test_utility.py` & `linearmodels-5.4/linearmodels/tests/panel/test_utility.py`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/linearmodels/tests/shared/test_typed_getters.py` & `linearmodels-5.4/linearmodels/tests/shared/test_typed_getters.py`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/linearmodels/tests/shared/test_utility.py` & `linearmodels-5.4/linearmodels/tests/shared/test_utility.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from linearmodels.compat.pandas import ANNUAL_FREQ
+
 import pickle
 import random
 import string
 import warnings
 
 import numpy as np
 from numpy.testing import assert_allclose
@@ -220,15 +222,15 @@
             "".join,
             [
                 [random.choice(string.ascii_lowercase) for __ in range(10)]
                 for _ in range(100)
             ],
         )
     )
-    times = pd.date_range("1999-12-31", freq="A-DEC", periods=7)
+    times = pd.date_range("1999-12-31", freq=ANNUAL_FREQ, periods=7)
     var_names = [f"x.{i}" for i in range(1, 4)]
     df3 = panel_to_frame(x, var_names, times, entities, True)
     mi = pd.MultiIndex.from_product([times, entities])
     expected3 = pd.DataFrame(index=mi, columns=var_names)
     for i in range(1, 4):
         expected3[f"x.{i}"] = x[i - 1].ravel()
     expected3.index = expected3.index.swaplevel(0, 1)
```

### Comparing `linearmodels-5.3/linearmodels/tests/system/_utility.py` & `linearmodels-5.4/linearmodels/tests/system/_utility.py`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/linearmodels/tests/system/results/execute-stata-3sls.py` & `linearmodels-5.4/linearmodels/tests/system/results/execute-stata-3sls.py`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/linearmodels/tests/system/results/execute-stata.py` & `linearmodels-5.4/linearmodels/tests/system/results/execute-stata.py`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/linearmodels/tests/system/results/generate_data.py` & `linearmodels-5.4/linearmodels/tests/system/results/generate_data.py`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/linearmodels/tests/system/results/parse_stata_3sls_results.py` & `linearmodels-5.4/linearmodels/tests/system/results/parse_stata_3sls_results.py`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/linearmodels/tests/system/results/parse_stata_results.py` & `linearmodels-5.4/linearmodels/tests/system/results/parse_stata_results.py`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/linearmodels/tests/system/results/simulated-3sls.dta` & `linearmodels-5.4/linearmodels/tests/system/results/simulated-3sls.dta`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/linearmodels/tests/system/results/simulated-sur.dta` & `linearmodels-5.4/linearmodels/tests/system/results/simulated-sur.dta`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/linearmodels/tests/system/results/stata-3sls-results.txt` & `linearmodels-5.4/linearmodels/tests/system/results/stata-3sls-results.txt`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/linearmodels/tests/system/results/stata-sur-results.txt` & `linearmodels-5.4/linearmodels/tests/system/results/stata-sur-results.txt`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/linearmodels/tests/system/test_3sls.py` & `linearmodels-5.4/linearmodels/tests/system/test_3sls.py`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/linearmodels/tests/system/test_3sls_against_stata.py` & `linearmodels-5.4/linearmodels/tests/system/test_3sls_against_stata.py`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/linearmodels/tests/system/test_covariance.py` & `linearmodels-5.4/linearmodels/tests/system/test_covariance.py`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/linearmodels/tests/system/test_equivalence.py` & `linearmodels-5.4/linearmodels/tests/system/test_equivalence.py`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/linearmodels/tests/system/test_formulas.py` & `linearmodels-5.4/linearmodels/tests/system/test_formulas.py`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/linearmodels/tests/system/test_gmm.py` & `linearmodels-5.4/linearmodels/tests/system/test_gmm.py`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/linearmodels/tests/system/test_sur.py` & `linearmodels-5.4/linearmodels/tests/system/test_sur.py`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/linearmodels/tests/system/test_sur_against_stata.py` & `linearmodels-5.4/linearmodels/tests/system/test_sur_against_stata.py`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/linearmodels/tests/system/test_utility.py` & `linearmodels-5.4/linearmodels/tests/system/test_utility.py`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/linearmodels/tests/test_examples.py` & `linearmodels-5.4/linearmodels/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/linearmodels/tests/test_tester.py` & `linearmodels-5.4/linearmodels/tests/test_tester.py`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/linearmodels/typing/__init__.py` & `linearmodels-5.4/linearmodels/typing/__init__.py`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/linearmodels/typing/data.py` & `linearmodels-5.4/linearmodels/typing/data.py`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/linearmodels.egg-info/PKG-INFO` & `linearmodels-5.4/linearmodels.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linearmodels
-Version: 5.3
+Version: 5.4
 Summary: Linear Panel, Instrumental Variable, Asset Pricing, and System Regression models for Python
 Home-page: http://github.com/bashtage/linearmodels
 Author: Kevin Sheppard
 Author-email: kevin.k.sheppard@gmail.com
 License: NCSA
 Keywords: linear models,regression,instrumental variables,IV,panel,fixed effects,clustered,heteroskedasticity,endogeneity,instruments,statistics,statistical inference,econometrics
 Classifier: Development Status :: 5 - Production/Stable
@@ -20,31 +20,30 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
-Requires-Dist: numpy>=1.19.0
-Requires-Dist: pandas>=1.1.0
+Requires-Dist: numpy>=1.22.0
+Requires-Dist: pandas>=1.3.0
 Requires-Dist: scipy>=1.5.0
 Requires-Dist: statsmodels>=0.12.0
 Requires-Dist: mypy_extensions>=0.4
-Requires-Dist: Cython>=0.29.34
+Requires-Dist: Cython>=0.29.37
 Requires-Dist: pyhdfe>=0.1
 Requires-Dist: formulaic>=0.6.5
-Requires-Dist: setuptools_scm[toml]<8.0.0,>=7.0.0
+Requires-Dist: setuptools_scm[toml]<9.0.0,>=8.0.0
 
 # Linear Models
 
 | Metric                     |                                                                                                                                                                                                                                                          |
 | :------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
 | **Latest Release**         | [![PyPI version](https://badge.fury.io/py/linearmodels.svg)](https://badge.fury.io/py/linearmodels)                                                                                                                                                      |
 | **Continuous Integration** | [![Build Status](https://dev.azure.com/kevinksheppard/kevinksheppard/_apis/build/status/bashtage.linearmodels?branchName=main)](https://dev.azure.com/kevinksheppard/kevinksheppard/_build/latest?definitionId=2&branchName=main)                        |
-|                            | [![Build status](https://ci.appveyor.com/api/projects/status/7768doy6wrdunmdt/branch/main?svg=true)](https://ci.appveyor.com/project/bashtage/linearmodels/branch/main)                                                                                  |
 | **Coverage**               | [![codecov](https://codecov.io/gh/bashtage/linearmodels/branch/main/graph/badge.svg)](https://codecov.io/gh/bashtage/linearmodels)                                                                                                                       |
 | **Code Quality**           | [![Codacy Badge](https://api.codacy.com/project/badge/Grade/745a24a69cb2466b95df6a53c83892de)](https://www.codacy.com/manual/bashtage/linearmodels?utm_source=github.com&utm_medium=referral&utm_content=bashtage/linearmodels&utm_campaign=Badge_Grade) |
 |                            | [![codebeat badge](https://codebeat.co/badges/aaae2fb4-72b5-4a66-97cd-77b93488f243)](https://codebeat.co/projects/github-com-bashtage-linearmodels-main)                                                                                                 |
 | **Citation**               | [![DOI](https://zenodo.org/badge/82291672.svg)](https://zenodo.org/badge/latestdoi/82291672)                                                                                                                                                             |
 
 Linear (regression) models for Python. Extends
 [statsmodels](http://www.statsmodels.org) with Panel regression,
@@ -165,20 +164,22 @@
 -   Dynamic Panel model estimation - _not started_
 
 ## Requirements
 
 ### Running
 
 -   Python 3.9+
--   NumPy (1.19+)
+-   NumPy (1.22+)
 -   SciPy (1.5+)
--   pandas (1.1+)
+-   pandas (1.3+)
 -   statsmodels (0.12+)
+-   formulaic (0.6.5+)
 -   xarray (0.16+, optional)
--   Cython (0.29.34+, optional)
+-   Cython (0.29.37+, optional)
+
 
 ### Testing
 
 -   py.test
 
 ### Documentation
```

### Comparing `linearmodels-5.3/linearmodels.egg-info/SOURCES.txt` & `linearmodels-5.4/linearmodels.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 .coveragerc
 .gitattributes
 .gitignore
 .lgtm.yml
 LICENSE.md
 MANIFEST.in
 README.md
-appveyor.yml
 azure-pipelines.yml
 github_deploy_key.enc
 pyproject.toml
 requirements-dev.txt
 requirements-test.txt
 requirements.txt
 setup.cfg
@@ -24,14 +23,15 @@
 ./linearmodels/__future__/__init__.py
 ./linearmodels/__future__/ordering.py
 ./linearmodels/asset_pricing/__init__.py
 ./linearmodels/asset_pricing/covariance.py
 ./linearmodels/asset_pricing/model.py
 ./linearmodels/asset_pricing/results.py
 ./linearmodels/compat/__init__.py
+./linearmodels/compat/pandas.py
 ./linearmodels/compat/statsmodels.py
 ./linearmodels/datasets/__init__.py
 ./linearmodels/datasets/birthweight/__init__.py
 ./linearmodels/datasets/birthweight/birthweight.csv.bz2
 ./linearmodels/datasets/card/__init__.py
 ./linearmodels/datasets/card/card.csv.bz2
 ./linearmodels/datasets/fertility/__init__.py
@@ -271,14 +271,15 @@
 linearmodels/__future__/__init__.py
 linearmodels/__future__/ordering.py
 linearmodels/asset_pricing/__init__.py
 linearmodels/asset_pricing/covariance.py
 linearmodels/asset_pricing/model.py
 linearmodels/asset_pricing/results.py
 linearmodels/compat/__init__.py
+linearmodels/compat/pandas.py
 linearmodels/compat/statsmodels.py
 linearmodels/datasets/__init__.py
 linearmodels/datasets/birthweight/__init__.py
 linearmodels/datasets/birthweight/birthweight.csv.bz2
 linearmodels/datasets/card/__init__.py
 linearmodels/datasets/card/card.csv.bz2
 linearmodels/datasets/fertility/__init__.py
```

### Comparing `linearmodels-5.3/pyproject.toml` & `linearmodels-5.4/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [
   "setuptools>=61",
   "wheel",
   "setuptools_scm[toml]>=7,<8",
   "oldest-supported-numpy",
-  "numpy; python_version>='3.12'",
+  "numpy; python_version>='3.13'",
   "cython>=0.29.34"
 ]
 build-backend = "setuptools.build_meta"
 
 [tool.black]
 target-version = ['py39', 'py310', 'py311']
 exclude = '''
```

### Comparing `linearmodels-5.3/setup.cfg` & `linearmodels-5.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `linearmodels-5.3/setup.py` & `linearmodels-5.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,15 +77,16 @@
         logging.warning("Building without binary support")
 
     setup(
         name="linearmodels",
         license="NCSA",
         description="Linear Panel, Instrumental Variable, Asset Pricing, and System "
         "Regression models for Python",
-        packages=find_namespace_packages(),
+        packages=["linearmodels"]
+        + [f"linearmodels.{v}" for v in find_namespace_packages("linearmodels")],
         package_dir={"linearmodels": "./linearmodels"},
         author="Kevin Sheppard",
         author_email="kevin.k.sheppard@gmail.com",
         url="http://github.com/bashtage/linearmodels",
         long_description=long_description,
         long_description_content_type="text/markdown",
         install_requires=open("requirements.txt").read().split("\n"),
```

