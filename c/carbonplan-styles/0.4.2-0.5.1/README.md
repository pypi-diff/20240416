# Comparing `tmp/carbonplan-styles-0.4.2.tar.gz` & `tmp/carbonplan_styles-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "carbonplan-styles-0.4.2.tar", last modified: Thu Sep 16 02:30:07 2021, max compression
+gzip compressed data, was "carbonplan_styles-0.5.1.tar", last modified: Tue Apr 16 21:25:32 2024, max compression
```

## Comparing `carbonplan-styles-0.4.2.tar` & `carbonplan_styles-0.5.1.tar`

### file list

```diff
@@ -1,35 +1,34 @@
-drwxr-xr-x   0 jhamman    (501) staff       (20)        0 2021-09-16 02:30:07.757848 carbonplan-styles-0.4.2/
-drwxr-xr-x   0 jhamman    (501) staff       (20)        0 2021-09-16 02:30:07.749858 carbonplan-styles-0.4.2/.github/
--rw-r--r--   0 jhamman    (501) staff       (20)      259 2021-01-08 19:53:32.000000 carbonplan-styles-0.4.2/.github/dependabot.yml
-drwxr-xr-x   0 jhamman    (501) staff       (20)        0 2021-09-16 02:30:07.750171 carbonplan-styles-0.4.2/.github/workflows/
--rw-r--r--   0 jhamman    (501) staff       (20)     1228 2021-09-15 20:16:53.000000 carbonplan-styles-0.4.2/.github/workflows/main.yaml
--rw-r--r--   0 jhamman    (501) staff       (20)       95 2021-09-15 20:16:53.000000 carbonplan-styles-0.4.2/.isort.cfg
--rw-r--r--   0 jhamman    (501) staff       (20)      851 2021-09-15 20:16:53.000000 carbonplan-styles-0.4.2/.pre-commit-config.yaml
--rw-r--r--   0 jhamman    (501) staff       (20)     1067 2020-05-03 04:09:43.000000 carbonplan-styles-0.4.2/LICENSE
--rw-r--r--   0 jhamman    (501) staff       (20)     3301 2021-09-16 02:30:07.757959 carbonplan-styles-0.4.2/PKG-INFO
--rw-r--r--   0 jhamman    (501) staff       (20)     2033 2021-04-28 23:51:43.000000 carbonplan-styles-0.4.2/README.md
-drwxr-xr-x   0 jhamman    (501) staff       (20)        0 2021-09-16 02:30:07.750923 carbonplan-styles-0.4.2/carbonplan_styles/
--rw-r--r--   0 jhamman    (501) staff       (20)      764 2021-09-09 02:48:32.000000 carbonplan-styles-0.4.2/carbonplan_styles/__init__.py
--rw-r--r--   0 jhamman    (501) staff       (20)     3185 2020-10-19 16:30:00.000000 carbonplan-styles-0.4.2/carbonplan_styles/altair.py
--rw-r--r--   0 jhamman    (501) staff       (20)     1884 2021-09-09 02:50:39.000000 carbonplan-styles-0.4.2/carbonplan_styles/colors.py
-drwxr-xr-x   0 jhamman    (501) staff       (20)        0 2021-09-16 02:30:07.751852 carbonplan-styles-0.4.2/carbonplan_styles/data/
--rw-r--r--   0 jhamman    (501) staff       (20)   540217 2021-09-16 02:29:27.000000 carbonplan-styles-0.4.2/carbonplan_styles/data/colormaps.json
-drwxr-xr-x   0 jhamman    (501) staff       (20)        0 2021-09-16 02:30:07.756163 carbonplan-styles-0.4.2/carbonplan_styles/mpl/
--rw-r--r--   0 jhamman    (501) staff       (20)     4881 2021-09-15 20:16:53.000000 carbonplan-styles-0.4.2/carbonplan_styles/mpl/__init__.py
--rw-r--r--   0 jhamman    (501) staff       (20)      795 2021-09-15 23:57:46.000000 carbonplan-styles-0.4.2/carbonplan_styles/mpl/colormaps.py
-drwxr-xr-x   0 jhamman    (501) staff       (20)        0 2021-09-16 02:30:07.756741 carbonplan-styles-0.4.2/carbonplan_styles/tests/
--rw-r--r--   0 jhamman    (501) staff       (20)      217 2021-09-15 20:16:53.000000 carbonplan-styles-0.4.2/carbonplan_styles/tests/test_altair.py
--rw-r--r--   0 jhamman    (501) staff       (20)     1552 2021-09-15 20:16:53.000000 carbonplan-styles-0.4.2/carbonplan_styles/tests/test_mpl.py
-drwxr-xr-x   0 jhamman    (501) staff       (20)        0 2021-09-16 02:30:07.751730 carbonplan-styles-0.4.2/carbonplan_styles.egg-info/
--rw-r--r--   0 jhamman    (501) staff       (20)     3301 2021-09-16 02:30:07.000000 carbonplan-styles-0.4.2/carbonplan_styles.egg-info/PKG-INFO
--rw-r--r--   0 jhamman    (501) staff       (20)      698 2021-09-16 02:30:07.000000 carbonplan-styles-0.4.2/carbonplan_styles.egg-info/SOURCES.txt
--rw-r--r--   0 jhamman    (501) staff       (20)        1 2021-09-16 02:30:07.000000 carbonplan-styles-0.4.2/carbonplan_styles.egg-info/dependency_links.txt
--rw-r--r--   0 jhamman    (501) staff       (20)      126 2021-09-16 02:30:07.000000 carbonplan-styles-0.4.2/carbonplan_styles.egg-info/entry_points.txt
--rw-r--r--   0 jhamman    (501) staff       (20)       37 2021-09-16 02:30:07.000000 carbonplan-styles-0.4.2/carbonplan_styles.egg-info/requires.txt
--rw-r--r--   0 jhamman    (501) staff       (20)       18 2021-09-16 02:30:07.000000 carbonplan-styles-0.4.2/carbonplan_styles.egg-info/top_level.txt
-drwxr-xr-x   0 jhamman    (501) staff       (20)        0 2021-09-16 02:30:07.757003 carbonplan-styles-0.4.2/demo/
--rw-r--r--   0 jhamman    (501) staff       (20)   185140 2021-09-15 20:16:53.000000 carbonplan-styles-0.4.2/demo/theme_demo.ipynb
--rw-r--r--   0 jhamman    (501) staff       (20)       51 2020-05-03 04:18:11.000000 carbonplan-styles-0.4.2/dev-requirements.txt
--rw-r--r--   0 jhamman    (501) staff       (20)       37 2021-09-09 04:11:18.000000 carbonplan-styles-0.4.2/requirements.txt
--rw-r--r--   0 jhamman    (501) staff       (20)      539 2021-09-16 02:30:07.758244 carbonplan-styles-0.4.2/setup.cfg
--rw-r--r--   0 jhamman    (501) staff       (20)     1556 2021-09-09 04:04:10.000000 carbonplan-styles-0.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:25:32.966579 carbonplan_styles-0.5.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:25:32.962579 carbonplan_styles-0.5.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-16 21:25:23.000000 carbonplan_styles-0.5.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:25:32.962579 carbonplan_styles-0.5.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-04-16 21:25:23.000000 carbonplan_styles-0.5.1/.github/workflows/main.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-04-16 21:25:23.000000 carbonplan_styles-0.5.1/.github/workflows/pypi-release.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-04-16 21:25:23.000000 carbonplan_styles-0.5.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-04-16 21:25:23.000000 carbonplan_styles-0.5.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-16 21:25:23.000000 carbonplan_styles-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3186 2024-04-16 21:25:32.966579 carbonplan_styles-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-04-16 21:25:23.000000 carbonplan_styles-0.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:25:32.962579 carbonplan_styles-0.5.1/carbonplan_styles/
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-16 21:25:23.000000 carbonplan_styles-0.5.1/carbonplan_styles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3327 2024-04-16 21:25:23.000000 carbonplan_styles-0.5.1/carbonplan_styles/altair.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-04-16 21:25:23.000000 carbonplan_styles-0.5.1/carbonplan_styles/colors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:25:32.966579 carbonplan_styles-0.5.1/carbonplan_styles/data/
+-rw-r--r--   0 runner    (1001) docker     (127)   540217 2024-04-16 21:25:23.000000 carbonplan_styles-0.5.1/carbonplan_styles/data/colormaps.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:25:32.966579 carbonplan_styles-0.5.1/carbonplan_styles/mpl/
+-rw-r--r--   0 runner    (1001) docker     (127)     4935 2024-04-16 21:25:23.000000 carbonplan_styles-0.5.1/carbonplan_styles/mpl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-16 21:25:23.000000 carbonplan_styles-0.5.1/carbonplan_styles/mpl/colormaps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:25:32.966579 carbonplan_styles-0.5.1/carbonplan_styles/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-16 21:25:23.000000 carbonplan_styles-0.5.1/carbonplan_styles/tests/test_altair.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-04-16 21:25:23.000000 carbonplan_styles-0.5.1/carbonplan_styles/tests/test_mpl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:25:32.966579 carbonplan_styles-0.5.1/carbonplan_styles.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3186 2024-04-16 21:25:32.000000 carbonplan_styles-0.5.1/carbonplan_styles.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-16 21:25:32.000000 carbonplan_styles-0.5.1/carbonplan_styles.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 21:25:32.000000 carbonplan_styles-0.5.1/carbonplan_styles.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-16 21:25:32.000000 carbonplan_styles-0.5.1/carbonplan_styles.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-16 21:25:32.000000 carbonplan_styles-0.5.1/carbonplan_styles.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-16 21:25:32.000000 carbonplan_styles-0.5.1/carbonplan_styles.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 21:25:32.966579 carbonplan_styles-0.5.1/demo/
+-rw-r--r--   0 runner    (1001) docker     (127)   185128 2024-04-16 21:25:23.000000 carbonplan_styles-0.5.1/demo/theme_demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-04-16 21:25:23.000000 carbonplan_styles-0.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 21:25:32.966579 carbonplan_styles-0.5.1/setup.cfg
```

### Comparing `carbonplan-styles-0.4.2/.pre-commit-config.yaml` & `carbonplan_styles-0.5.1/.pre-commit-config.yaml`

 * *Files 22% similar despite different names*

```diff
@@ -1,35 +1,54 @@
+ci:
+  autoupdate_schedule: quarterly
+
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.0.1
+    rev: v4.6.0
     hooks:
       - id: trailing-whitespace
       - id: end-of-file-fixer
       - id: check-docstring-first
       - id: check-json
       - id: check-yaml
-      - id: double-quote-string-fixer
+      - id: debug-statements
+      - id: mixed-line-ending
+
+  - repo: https://github.com/asottile/pyupgrade
+    rev: v3.15.2
+    hooks:
+      - id: pyupgrade
+        args:
+          - "--py38-plus"
 
   - repo: https://github.com/psf/black
-    rev: 21.8b0
+    rev: 24.3.0
     hooks:
       - id: black
-        args: ["--line-length", "100", "--skip-string-normalization"]
+      - id: black-jupyter
 
-  - repo: https://github.com/PyCQA/flake8
-    rev: 3.9.2
+  - repo: https://github.com/keewis/blackdoc
+    rev: v0.3.9
     hooks:
-      - id: flake8
-  - repo: https://github.com/asottile/seed-isort-config
-    rev: v2.2.0
+      - id: blackdoc
+
+  - repo: https://github.com/astral-sh/ruff-pre-commit
+    rev: "v0.3.5"
     hooks:
-      - id: seed-isort-config
-  - repo: https://github.com/PyCQA/isort
-    rev: 5.9.3
+      - id: ruff
+        args: ["--fix"]
+
+  - repo: https://github.com/pre-commit/mirrors-prettier
+    rev: v4.0.0-alpha.8
     hooks:
-      - id: isort
+      - id: prettier
 
   - repo: https://github.com/pre-commit/mirrors-prettier
-    rev: v2.4.0
+    rev: "v4.0.0-alpha.8"
     hooks:
       - id: prettier
-        language_version: system
+        name: prettier-markdown
+        entry: prettier --write --parser mdx
+        files: "\\.(\
+          |md|markdown|mdown|mkdn\
+          |mdx\
+          )$"
```

### Comparing `carbonplan-styles-0.4.2/LICENSE` & `carbonplan_styles-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `carbonplan-styles-0.4.2/README.md` & `carbonplan_styles-0.5.1/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,128 +1,133 @@
-00000000: 3c69 6d67 0a20 2073 7263 3d27 6874 7470  <img.  src='http
-00000010: 733a 2f2f 6361 7262 6f6e 706c 616e 2d61  s://carbonplan-a
-00000020: 7373 6574 732e 7333 2e61 6d61 7a6f 6e61  ssets.s3.amazona
-00000030: 7773 2e63 6f6d 2f6d 6f6e 6f67 7261 6d2f  ws.com/monogram/
-00000040: 6461 726b 2d73 6d61 6c6c 2e70 6e67 270a  dark-small.png'.
-00000050: 2020 6865 6967 6874 3d27 3438 270a 2f3e    height='48'./>
-00000060: 0a0a 2320 6361 7262 6f6e 706c 616e 202f  ..# carbonplan /
-00000070: 2073 7479 6c65 730a 0a2a 2a70 6c6f 7420   styles..**plot 
-00000080: 7374 796c 6573 2066 6f72 206d 6174 706c  styles for matpl
-00000090: 6f74 6c69 6220 616e 6420 616c 7461 6972  otlib and altair
-000000a0: 2a2a 0a0a 5b21 5b47 6974 4875 625d 5b67  **..[![GitHub][g
-000000b0: 6974 6875 622d 6261 6467 655d 5d5b 6769  ithub-badge]][gi
-000000c0: 7468 7562 5d0a 5b21 5b42 7569 6c64 2053  thub].[![Build S
-000000d0: 7461 7475 735d 5d5b 6163 7469 6f6e 735d  tatus]][actions]
-000000e0: 0a21 5b4d 4954 204c 6963 656e 7365 5d5b  .![MIT License][
-000000f0: 5d0a 0a5b 6769 7468 7562 5d3a 2068 7474  ]..[github]: htt
-00000100: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000110: 6361 7262 6f6e 706c 616e 2f73 7479 6c65  carbonplan/style
-00000120: 730a 5b67 6974 6875 622d 6261 6467 655d  s.[github-badge]
-00000130: 3a20 6874 7470 733a 2f2f 6261 6467 656e  : https://badgen
-00000140: 2e6e 6574 2f62 6164 6765 2f2d 2f67 6974  .net/badge/-/git
-00000150: 6875 623f 6963 6f6e 3d67 6974 6875 6226  hub?icon=github&
-00000160: 6c61 6265 6c0a 5b62 7569 6c64 2073 7461  label.[build sta
-00000170: 7475 735d 3a20 6874 7470 733a 2f2f 6769  tus]: https://gi
-00000180: 7468 7562 2e63 6f6d 2f63 6172 626f 6e70  thub.com/carbonp
-00000190: 6c61 6e2f 7374 796c 6573 2f61 6374 696f  lan/styles/actio
-000001a0: 6e73 2f77 6f72 6b66 6c6f 7773 2f6d 6169  ns/workflows/mai
-000001b0: 6e2e 7961 6d6c 2f62 6164 6765 2e73 7667  n.yaml/badge.svg
-000001c0: 0a5b 6163 7469 6f6e 735d 3a20 6874 7470  .[actions]: http
-000001d0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f63  s://github.com/c
-000001e0: 6172 626f 6e70 6c61 6e2f 7374 796c 6573  arbonplan/styles
-000001f0: 2f61 6374 696f 6e73 2f77 6f72 6b66 6c6f  /actions/workflo
-00000200: 7773 2f6d 6169 6e2e 7961 6d6c 0a5b 6d69  ws/main.yaml.[mi
-00000210: 7420 6c69 6365 6e73 655d 3a20 6874 7470  t license]: http
-00000220: 733a 2f2f 6261 6467 656e 2e6e 6574 2f62  s://badgen.net/b
-00000230: 6164 6765 2f6c 6963 656e 7365 2f4d 4954  adge/license/MIT
-00000240: 2f62 6c75 650a 0a41 2063 6f6c 6c65 6374  /blue..A collect
-00000250: 696f 6e20 6f66 2070 6c6f 7474 696e 6720  ion of plotting 
-00000260: 7374 796c 6573 2066 6f72 205b 4d61 7470  styles for [Matp
-00000270: 6c6f 746c 6962 5d28 6874 7470 733a 2f2f  lotlib](https://
-00000280: 6d61 7470 6c6f 746c 6962 2e6f 7267 2f29  matplotlib.org/)
-00000290: 2061 6e64 205b 416c 7461 6972 5d28 6874   and [Altair](ht
-000002a0: 7470 733a 2f2f 616c 7461 6972 2d76 697a  tps://altair-viz
-000002b0: 2e67 6974 6875 622e 696f 2f29 2e0a 0a54  .github.io/)...T
-000002c0: 7279 2069 7420 6f75 7420 6f6e 2042 696e  ry it out on Bin
-000002d0: 6465 723a 0a5b 215b 4269 6e64 6572 5d28  der:.[![Binder](
-000002e0: 6874 7470 733a 2f2f 6d79 6269 6e64 6572  https://mybinder
-000002f0: 2e6f 7267 2f62 6164 6765 5f6c 6f67 6f2e  .org/badge_logo.
-00000300: 7376 6729 5d28 6874 7470 733a 2f2f 6d79  svg)](https://my
-00000310: 6269 6e64 6572 2e6f 7267 2f76 322f 6768  binder.org/v2/gh
-00000320: 2f6a 6861 6d6d 616e 2f63 6172 626f 6e70  /jhamman/carbonp
-00000330: 6c61 6e2d 7374 796c 6573 2f6d 6173 7465  lan-styles/maste
-00000340: 723f 7572 6c70 6174 683d 6c61 6229 0a0a  r?urlpath=lab)..
-00000350: 2323 2069 6e73 7461 6c6c 0a0a 6060 6073  ## install..```s
-00000360: 6865 6c6c 0a70 6970 2069 6e73 7461 6c6c  hell.pip install
-00000370: 2063 6172 626f 6e70 6c61 6e5b 7374 796c   carbonplan[styl
-00000380: 6573 5d0a 6060 600a 0a23 2320 7573 6167  es].```..## usag
-00000390: 650a 0a54 6865 7265 2061 7265 2063 7572  e..There are cur
-000003a0: 7265 6e74 6c79 2074 776f 2073 6570 6172  rently two separ
-000003b0: 6174 6520 7374 796c 6573 2f74 6865 6d65  ate styles/theme
-000003c0: 7320 6176 6169 6c61 626c 6520 696e 2074  s available in t
-000003d0: 6869 7320 7061 636b 6167 653a 0a0a 312e  his package:..1.
-000003e0: 2060 6361 7262 6f6e 706c 616e 5f64 6172   `carbonplan_dar
-000003f0: 6b60 3a20 626c 6163 6b20 6261 636b 6772  k`: black backgr
-00000400: 6f75 6e64 2c20 6c69 6768 7465 7220 636f  ound, lighter co
-00000410: 6c6f 7273 0a32 2e20 6063 6172 626f 6e70  lors.2. `carbonp
-00000420: 6c61 6e5f 6c69 6768 7460 3a20 7768 6974  lan_light`: whit
-00000430: 6520 6261 636b 6772 6f75 6e64 2c20 6461  e background, da
-00000440: 726b 6572 2063 6f6c 6f72 730a 0a42 6f74  rker colors..Bot
-00000450: 6820 7374 7965 6c73 2f74 6865 6d65 7320  h styels/themes 
-00000460: 6172 6520 6175 746f 6d61 7469 6361 6c6c  are automaticall
-00000470: 7920 6d61 6465 2061 7661 696c 6162 6c65  y made available
-00000480: 2069 6e20 4d61 7470 6c6f 746c 6962 2061   in Matplotlib a
-00000490: 6e64 2041 6c74 6169 722e 0a0a 2323 2320  nd Altair...### 
-000004a0: 6d61 7470 6c6f 746c 6962 0a0a 6060 6070  matplotlib..```p
-000004b0: 7974 686f 6e0a 6672 6f6d 2063 6172 626f  ython.from carbo
-000004c0: 6e70 6c61 6e20 696d 706f 7274 2073 7479  nplan import sty
-000004d0: 6c65 730a 0a73 7479 6c65 732e 6d70 6c2e  les..styles.mpl.
-000004e0: 7365 745f 7468 656d 6528 7374 796c 653d  set_theme(style=
-000004f0: 2763 6172 626f 6e70 6c61 6e5f 6461 726b  'carbonplan_dark
-00000500: 2729 0a60 6060 0a0a 2323 2320 616c 7461  ').```..### alta
-00000510: 6972 0a0a 6060 6070 7974 686f 6e0a 696d  ir..```python.im
-00000520: 706f 7274 2061 6c74 6169 7220 6173 2061  port altair as a
-00000530: 6c74 0a0a 616c 742e 7468 656d 6573 2e65  lt..alt.themes.e
-00000540: 6e61 626c 6528 2763 6172 626f 6e70 6c61  nable('carbonpla
-00000550: 6e5f 6461 726b 2729 0a60 6060 0a0a 2323  n_dark').```..##
-00000560: 206c 6963 656e 7365 0a0a 416c 6c20 7468   license..All th
-00000570: 6520 636f 6465 2069 6e20 7468 6973 2072  e code in this r
-00000580: 6570 6f73 6974 6f72 7920 6973 205b 4d49  epository is [MI
-00000590: 545d 2868 7474 7073 3a2f 2f63 686f 6f73  T](https://choos
-000005a0: 6561 6c69 6365 6e73 652e 636f 6d2f 6c69  ealicense.com/li
-000005b0: 6365 6e73 6573 2f6d 6974 2f29 206c 6963  censes/mit/) lic
-000005c0: 656e 7365 642e 2057 6520 696e 636c 7564  ensed. We includ
-000005d0: 6520 6174 7472 6962 7574 696f 6e20 666f  e attribution fo
-000005e0: 7220 7468 6973 2063 6f6e 7465 6e74 2c20  r this content, 
-000005f0: 616e 6420 7765 2070 6c65 6173 6520 7265  and we please re
-00000600: 7175 6573 7420 7468 6174 2079 6f75 2061  quest that you a
-00000610: 6c73 6f20 6d61 696e 7461 696e 2074 6861  lso maintain tha
-00000620: 7420 6174 7472 6962 7574 696f 6e20 6966  t attribution if
-00000630: 2075 7369 6e67 2074 6869 7320 6461 7461   using this data
-00000640: 2e0a 0a23 2320 6162 6f75 7420 7573 0a0a  ...## about us..
-00000650: 4361 7262 6f6e 506c 616e 2069 7320 6120  CarbonPlan is a 
-00000660: 6e6f 6e2d 7072 6f66 6974 206f 7267 616e  non-profit organ
-00000670: 697a 6174 696f 6e20 7468 6174 2075 7365  ization that use
-00000680: 7320 6461 7461 2061 6e64 2073 6369 656e  s data and scien
-00000690: 6365 2066 6f72 2063 6c69 6d61 7465 2061  ce for climate a
-000006a0: 6374 696f 6e2e 2057 6520 6169 6d20 746f  ction. We aim to
-000006b0: 2069 6d70 726f 7665 2074 6865 2074 7261   improve the tra
-000006c0: 6e73 7061 7265 6e63 7920 616e 6420 7363  nsparency and sc
-000006d0: 6965 6e74 6966 6963 2069 6e74 6567 7269  ientific integri
-000006e0: 7479 206f 6620 6361 7262 6f6e 2072 656d  ty of carbon rem
-000006f0: 6f76 616c 2061 6e64 2063 6c69 6d61 7465  oval and climate
-00000700: 2073 6f6c 7574 696f 6e73 2074 6872 6f75   solutions throu
-00000710: 6768 206f 7065 6e20 6461 7461 2061 6e64  gh open data and
-00000720: 2074 6f6f 6c73 2e20 4669 6e64 206f 7574   tools. Find out
-00000730: 206d 6f72 6520 6174 205b 6361 7262 6f6e   more at [carbon
-00000740: 706c 616e 2e6f 7267 5d28 6874 7470 733a  plan.org](https:
-00000750: 2f2f 6361 7262 6f6e 706c 616e 2e6f 7267  //carbonplan.org
-00000760: 2f29 206f 7220 6765 7420 696e 2074 6f75  /) or get in tou
-00000770: 6368 2062 7920 5b6f 7065 6e69 6e67 2061  ch by [opening a
-00000780: 6e20 6973 7375 655d 2868 7474 7073 3a2f  n issue](https:/
-00000790: 2f67 6974 6875 622e 636f 6d2f 6361 7262  /github.com/carb
-000007a0: 6f6e 706c 616e 2f73 7479 6c65 732f 6973  onplan/styles/is
-000007b0: 7375 6573 2f6e 6577 2920 6f72 205b 7365  sues/new) or [se
-000007c0: 6e64 696e 6720 7573 2061 6e20 656d 6169  nding us an emai
-000007d0: 6c5d 286d 6169 6c74 6f3a 6865 6c6c 6f40  l](mailto:hello@
-000007e0: 6361 7262 6f6e 706c 616e 2e6f 7267 292e  carbonplan.org).
-000007f0: 0a                                       .
+00000000: 3c70 2061 6c69 676e 3d22 6c65 6674 2220  <p align="left" 
+00000010: 3e0a 3c61 2068 7265 663d 2768 7474 7073  >.<a href='https
+00000020: 3a2f 2f63 6172 626f 6e70 6c61 6e2e 6f72  ://carbonplan.or
+00000030: 6727 3e0a 3c70 6963 7475 7265 3e0a 2020  g'>.<picture>.  
+00000040: 3c73 6f75 7263 6520 6d65 6469 613d 2228  <source media="(
+00000050: 7072 6566 6572 732d 636f 6c6f 722d 7363  prefers-color-sc
+00000060: 6865 6d65 3a20 6461 726b 2922 2073 7263  heme: dark)" src
+00000070: 7365 743d 2268 7474 7073 3a2f 2f63 6172  set="https://car
+00000080: 626f 6e70 6c61 6e2d 6173 7365 7473 2e73  bonplan-assets.s
+00000090: 332e 616d 617a 6f6e 6177 732e 636f 6d2f  3.amazonaws.com/
+000000a0: 6d6f 6e6f 6772 616d 2f6c 6967 6874 2d73  monogram/light-s
+000000b0: 6d61 6c6c 2e70 6e67 223e 0a20 203c 696d  mall.png">.  <im
+000000c0: 6720 616c 743d 2243 6172 626f 6e50 6c61  g alt="CarbonPla
+000000d0: 6e20 6d6f 6e6f 6772 616d 2e22 2068 6569  n monogram." hei
+000000e0: 6768 743d 2234 3822 2073 7263 3d22 6874  ght="48" src="ht
+000000f0: 7470 733a 2f2f 6361 7262 6f6e 706c 616e  tps://carbonplan
+00000100: 2d61 7373 6574 732e 7333 2e61 6d61 7a6f  -assets.s3.amazo
+00000110: 6e61 7773 2e63 6f6d 2f6d 6f6e 6f67 7261  naws.com/monogra
+00000120: 6d2f 6461 726b 2d73 6d61 6c6c 2e70 6e67  m/dark-small.png
+00000130: 223e 0a3c 2f70 6963 7475 7265 3e0a 3c2f  ">.</picture>.</
+00000140: 613e 0a3c 2f70 3e0a 0a23 2063 6172 626f  a>.</p>..# carbo
+00000150: 6e70 6c61 6e20 2f20 7374 796c 6573 0a0a  nplan / styles..
+00000160: 2a2a 706c 6f74 2073 7479 6c65 7320 666f  **plot styles fo
+00000170: 7220 6d61 7470 6c6f 746c 6962 2061 6e64  r matplotlib and
+00000180: 2061 6c74 6169 722a 2a0a 0a5b 215b 4349   altair**..[![CI
+00000190: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+000001a0: 2e63 6f6d 2f63 6172 626f 6e70 6c61 6e2f  .com/carbonplan/
+000001b0: 7374 796c 6573 2f61 6374 696f 6e73 2f77  styles/actions/w
+000001c0: 6f72 6b66 6c6f 7773 2f6d 6169 6e2e 7961  orkflows/main.ya
+000001d0: 6d6c 2f62 6164 6765 2e73 7667 295d 2868  ml/badge.svg)](h
+000001e0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000001f0: 6d2f 6361 7262 6f6e 706c 616e 2f73 7479  m/carbonplan/sty
+00000200: 6c65 732f 6163 7469 6f6e 732f 776f 726b  les/actions/work
+00000210: 666c 6f77 732f 6d61 696e 2e79 616d 6c29  flows/main.yaml)
+00000220: 0a21 5b50 7950 495d 2868 7474 7073 3a2f  .![PyPI](https:/
+00000230: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
+00000240: 7079 7069 2f76 2f63 6172 626f 6e70 6c61  pypi/v/carbonpla
+00000250: 6e5f 7374 796c 6573 290a 5b21 5b4c 6963  n_styles).[![Lic
+00000260: 656e 7365 3a20 4d49 545d 2868 7474 7073  ense: MIT](https
+00000270: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
+00000280: 6f2f 6261 6467 652f 4c69 6365 6e73 652d  o/badge/License-
+00000290: 4d49 542d 626c 7565 2e73 7667 295d 2868  MIT-blue.svg)](h
+000002a0: 7474 7073 3a2f 2f6f 7065 6e73 6f75 7263  ttps://opensourc
+000002b0: 652e 6f72 672f 6c69 6365 6e73 6573 2f4d  e.org/licenses/M
+000002c0: 4954 290a 0a41 2063 6f6c 6c65 6374 696f  IT)..A collectio
+000002d0: 6e20 6f66 2070 6c6f 7474 696e 6720 7374  n of plotting st
+000002e0: 796c 6573 2066 6f72 205b 4d61 7470 6c6f  yles for [Matplo
+000002f0: 746c 6962 5d28 6874 7470 733a 2f2f 6d61  tlib](https://ma
+00000300: 7470 6c6f 746c 6962 2e6f 7267 2f29 2061  tplotlib.org/) a
+00000310: 6e64 205b 416c 7461 6972 5d28 6874 7470  nd [Altair](http
+00000320: 733a 2f2f 616c 7461 6972 2d76 697a 2e67  s://altair-viz.g
+00000330: 6974 6875 622e 696f 2f29 2e0a 0a54 7279  ithub.io/)...Try
+00000340: 2069 7420 6f75 7420 6f6e 2042 696e 6465   it out on Binde
+00000350: 723a 0a5b 215b 4269 6e64 6572 5d28 6874  r:.[![Binder](ht
+00000360: 7470 733a 2f2f 6d79 6269 6e64 6572 2e6f  tps://mybinder.o
+00000370: 7267 2f62 6164 6765 5f6c 6f67 6f2e 7376  rg/badge_logo.sv
+00000380: 6729 5d28 6874 7470 733a 2f2f 6d79 6269  g)](https://mybi
+00000390: 6e64 6572 2e6f 7267 2f76 322f 6768 2f63  nder.org/v2/gh/c
+000003a0: 6172 626f 6e70 6c61 6e2f 7374 796c 6573  arbonplan/styles
+000003b0: 2f6d 6169 6e3f 7572 6c70 6174 683d 6c61  /main?urlpath=la
+000003c0: 6229 0a0a 2323 2069 6e73 7461 6c6c 0a0a  b)..## install..
+000003d0: 6060 6073 6865 6c6c 0a70 6970 2069 6e73  ```shell.pip ins
+000003e0: 7461 6c6c 2022 6361 7262 6f6e 706c 616e  tall "carbonplan
+000003f0: 5b73 7479 6c65 735d 220a 6060 600a 0a23  [styles]".```..#
+00000400: 2320 7573 6167 650a 0a54 6865 7265 2061  # usage..There a
+00000410: 7265 2063 7572 7265 6e74 6c79 2074 776f  re currently two
+00000420: 2073 6570 6172 6174 6520 7374 796c 6573   separate styles
+00000430: 2f74 6865 6d65 7320 6176 6169 6c61 626c  /themes availabl
+00000440: 6520 696e 2074 6869 7320 7061 636b 6167  e in this packag
+00000450: 653a 0a0a 312e 2060 6361 7262 6f6e 706c  e:..1. `carbonpl
+00000460: 616e 5f64 6172 6b60 3a20 626c 6163 6b20  an_dark`: black 
+00000470: 6261 636b 6772 6f75 6e64 2c20 6c69 6768  background, ligh
+00000480: 7465 7220 636f 6c6f 7273 0a32 2e20 6063  ter colors.2. `c
+00000490: 6172 626f 6e70 6c61 6e5f 6c69 6768 7460  arbonplan_light`
+000004a0: 3a20 7768 6974 6520 6261 636b 6772 6f75  : white backgrou
+000004b0: 6e64 2c20 6461 726b 6572 2063 6f6c 6f72  nd, darker color
+000004c0: 730a 0a42 6f74 6820 7374 7965 6c73 2f74  s..Both styels/t
+000004d0: 6865 6d65 7320 6172 6520 6175 746f 6d61  hemes are automa
+000004e0: 7469 6361 6c6c 7920 6d61 6465 2061 7661  tically made ava
+000004f0: 696c 6162 6c65 2069 6e20 4d61 7470 6c6f  ilable in Matplo
+00000500: 746c 6962 2061 6e64 2041 6c74 6169 722e  tlib and Altair.
+00000510: 0a0a 2323 2320 6d61 7470 6c6f 746c 6962  ..### matplotlib
+00000520: 0a0a 6060 6070 7974 686f 6e0a 6672 6f6d  ..```python.from
+00000530: 2063 6172 626f 6e70 6c61 6e20 696d 706f   carbonplan impo
+00000540: 7274 2073 7479 6c65 730a 0a73 7479 6c65  rt styles..style
+00000550: 732e 6d70 6c2e 7365 745f 7468 656d 6528  s.mpl.set_theme(
+00000560: 7374 796c 653d 2763 6172 626f 6e70 6c61  style='carbonpla
+00000570: 6e5f 6461 726b 2729 0a60 6060 0a0a 2323  n_dark').```..##
+00000580: 2320 616c 7461 6972 0a0a 6060 6070 7974  # altair..```pyt
+00000590: 686f 6e0a 696d 706f 7274 2061 6c74 6169  hon.import altai
+000005a0: 7220 6173 2061 6c74 0a0a 616c 742e 7468  r as alt..alt.th
+000005b0: 656d 6573 2e65 6e61 626c 6528 2763 6172  emes.enable('car
+000005c0: 626f 6e70 6c61 6e5f 6461 726b 2729 0a60  bonplan_dark').`
+000005d0: 6060 0a0a 2323 206c 6963 656e 7365 0a0a  ``..## license..
+000005e0: 416c 6c20 7468 6520 636f 6465 2069 6e20  All the code in 
+000005f0: 7468 6973 2072 6570 6f73 6974 6f72 7920  this repository 
+00000600: 6973 205b 4d49 545d 2868 7474 7073 3a2f  is [MIT](https:/
+00000610: 2f63 686f 6f73 6561 6c69 6365 6e73 652e  /choosealicense.
+00000620: 636f 6d2f 6c69 6365 6e73 6573 2f6d 6974  com/licenses/mit
+00000630: 2f29 2d6c 6963 656e 7365 642e 2057 6520  /)-licensed. We 
+00000640: 696e 636c 7564 6520 6174 7472 6962 7574  include attribut
+00000650: 696f 6e20 666f 7220 7468 6973 2063 6f6e  ion for this con
+00000660: 7465 6e74 2c20 616e 6420 7765 2070 6c65  tent, and we ple
+00000670: 6173 6520 7265 7175 6573 7420 7468 6174  ase request that
+00000680: 2079 6f75 2061 6c73 6f20 6d61 696e 7461   you also mainta
+00000690: 696e 2074 6861 7420 6174 7472 6962 7574  in that attribut
+000006a0: 696f 6e20 6966 2075 7369 6e67 2074 6869  ion if using thi
+000006b0: 7320 6461 7461 2e0a 0a23 2320 6162 6f75  s data...## abou
+000006c0: 7420 7573 0a0a 4361 7262 6f6e 506c 616e  t us..CarbonPlan
+000006d0: 2069 7320 6120 6e6f 6e70 726f 6669 7420   is a nonprofit 
+000006e0: 6f72 6761 6e69 7a61 7469 6f6e 2074 6861  organization tha
+000006f0: 7420 7573 6573 2064 6174 6120 616e 6420  t uses data and 
+00000700: 7363 6965 6e63 6520 666f 7220 636c 696d  science for clim
+00000710: 6174 6520 6163 7469 6f6e 2e20 5765 2061  ate action. We a
+00000720: 696d 2074 6f20 696d 7072 6f76 6520 7468  im to improve th
+00000730: 6520 7472 616e 7370 6172 656e 6379 2061  e transparency a
+00000740: 6e64 2073 6369 656e 7469 6669 6320 696e  nd scientific in
+00000750: 7465 6772 6974 7920 6f66 2063 6c69 6d61  tegrity of clima
+00000760: 7465 2073 6f6c 7574 696f 6e73 2077 6974  te solutions wit
+00000770: 6820 6f70 656e 2064 6174 6120 616e 6420  h open data and 
+00000780: 746f 6f6c 732e 2046 696e 6420 6f75 7420  tools. Find out 
+00000790: 6d6f 7265 2061 7420 5b63 6172 626f 6e70  more at [carbonp
+000007a0: 6c61 6e2e 6f72 675d 2868 7474 7073 3a2f  lan.org](https:/
+000007b0: 2f63 6172 626f 6e70 6c61 6e2e 6f72 672f  /carbonplan.org/
+000007c0: 2920 6f72 2067 6574 2069 6e20 746f 7563  ) or get in touc
+000007d0: 6820 6279 205b 6f70 656e 696e 6720 616e  h by [opening an
+000007e0: 2069 7373 7565 5d28 6874 7470 733a 2f2f   issue](https://
+000007f0: 6769 7468 7562 2e63 6f6d 2f63 6172 626f  github.com/carbo
+00000800: 6e70 6c61 6e2f 7374 796c 6573 2f69 7373  nplan/styles/iss
+00000810: 7565 732f 6e65 7729 206f 7220 5b73 656e  ues/new) or [sen
+00000820: 6469 6e67 2075 7320 616e 2065 6d61 696c  ding us an email
+00000830: 5d28 6d61 696c 746f 3a68 656c 6c6f 4063  ](mailto:hello@c
+00000840: 6172 626f 6e70 6c61 6e2e 6f72 6729 2e0a  arbonplan.org)..
```

### Comparing `carbonplan-styles-0.4.2/carbonplan_styles/data/colormaps.json` & `carbonplan_styles-0.5.1/carbonplan_styles/data/colormaps.json`

 * *Files identical despite different names*

### Comparing `carbonplan-styles-0.4.2/carbonplan_styles/mpl/__init__.py` & `carbonplan_styles-0.5.1/carbonplan_styles/mpl/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,74 +4,87 @@
 import matplotlib.colors as mcolors
 import numpy as np
 import seaborn as sns
 
 from ..colors import colors, hex_to_rgb, rgb_to_dec
 from . import colormaps  # noqa
 
-palette_colors = ['blue', 'orange', 'green', 'red', 'purple', 'pink', 'grey', 'yellow', 'teal']
+palette_colors = [
+    "blue",
+    "orange",
+    "green",
+    "red",
+    "purple",
+    "pink",
+    "grey",
+    "yellow",
+    "teal",
+]
 
 
 def get_style_config(mode):
-
     c = colors(mode=mode)
 
-    if mode == 'light':
-        background = 'white'  # instead of c['background']
+    if mode == "light":
+        background = "white"  # instead of c['background']
     else:
-        background = c['background']
+        background = c["background"]
 
     style = {
-        'axes.facecolor': background,
-        'axes.edgecolor': c['secondary'],
-        'axes.grid': False,
-        'axes.axisbelow': True,
-        'axes.labelcolor': c['text'],
-        'figure.facecolor': background,
-        'grid.color': c['secondary'],
-        'grid.linestyle': '-',
-        'text.color': c['text'],
-        'xtick.color': c['secondary'],
-        'ytick.color': c['secondary'],
-        'xtick.labelcolor': c['blue'],
-        'ytick.labelcolor': c['blue'],
-        'xtick.direction': 'out',
-        'ytick.direction': 'out',
-        'lines.markeredgewidth': 0.0,
-        'lines.solid_capstyle': 'round',
-        'patch.edgecolor': c['secondary'],
-        'patch.force_edgecolor': True,
-        'image.cmap': 'cool_light',
-        'font.weight': '400',
-        'font.family': 'monospace',
-        'font.monospace': ['relative-mono-11-pitch-pro', 'Menlo', 'monospace'],
-        'font.sans-serif': [
-            'relative-book-pro',
-            'Roboto',
-            'system-ui',
-            '-apple-system',
-            'BlinkMacSystemFont',
+        "axes.facecolor": background,
+        "axes.edgecolor": c["secondary"],
+        "axes.grid": False,
+        "axes.axisbelow": True,
+        "axes.labelcolor": c["text"],
+        "figure.facecolor": background,
+        "grid.color": c["secondary"],
+        "grid.linestyle": "-",
+        "text.color": c["text"],
+        "xtick.color": c["secondary"],
+        "ytick.color": c["secondary"],
+        "xtick.labelcolor": c["blue"],
+        "ytick.labelcolor": c["blue"],
+        "xtick.direction": "out",
+        "ytick.direction": "out",
+        "lines.markeredgewidth": 0.0,
+        "lines.solid_capstyle": "round",
+        "patch.edgecolor": c["secondary"],
+        "patch.force_edgecolor": True,
+        "image.cmap": "cool_light",
+        "font.weight": "400",
+        "font.family": "monospace",
+        "font.monospace": ["relative-mono-11-pitch-pro", "Menlo", "monospace"],
+        "font.sans-serif": [
+            "relative-book-pro",
+            "Roboto",
+            "system-ui",
+            "-apple-system",
+            "BlinkMacSystemFont",
         ],
-        'xtick.bottom': True,
-        'xtick.top': False,
-        'ytick.left': True,
-        'ytick.right': False,
-        'axes.spines.left': True,
-        'axes.spines.bottom': True,
-        'axes.spines.right': False,
-        'axes.spines.top': False,
-        'scatter.marker': 'o',
-        'scatter.edgecolors': None,
+        "xtick.bottom": True,
+        "xtick.top": False,
+        "ytick.left": True,
+        "ytick.right": False,
+        "axes.spines.left": True,
+        "axes.spines.bottom": True,
+        "axes.spines.right": False,
+        "axes.spines.top": False,
+        "scatter.marker": "o",
+        "scatter.edgecolors": None,
     }
 
     return style, c
 
 
 def set_theme(
-    context='notebook', style='carbonplan_light', font='monospace', font_scale=1, rc=None
+    context="notebook",
+    style="carbonplan_light",
+    font="monospace",
+    font_scale=1,
+    rc=None,
 ):
     """Set multiple theme parameters in one step.
 
     Each set of parameters can be set directly or temporarily, see the
     referenced functions below for more information.
 
     Parameters
@@ -90,15 +103,15 @@
     seaborn.set_theme
     """
     # set context
     sns.set_context(context, font_scale)
 
     # set style
     style_dict, colors_dict = get_style_config(style)
-    sns.set_style(style_dict, rc={'font.family': font})
+    sns.set_style(style_dict, rc={"font.family": font})
 
     # set color palette
     c = [colors_dict[k] for k in palette_colors]
     palette = sns.color_palette(c)
     sns.set_palette(palette)
 
     if rc is not None:
@@ -124,44 +137,43 @@
 
     References
     ----------
     https://towardsdatascience.com/beautiful-custom-colormaps-with-matplotlib-5bab3d1f0e72
     """
 
     warnings.warn(
-        'get_continuous_cmap is deprecated, use carbonplan_styles.mpl.colormaps instead',
+        "get_continuous_cmap is deprecated, use carbonplan_styles.mpl.colormaps instead",
         DeprecationWarning,
     )
 
     if name is None:
-        name = '-'.join(hex_list)
+        name = "-".join(hex_list)
 
     rgb_list = [rgb_to_dec(hex_to_rgb(i)) for i in hex_list]
 
     if float_list:
         pass
     else:
         float_list = list(np.linspace(0, 1, len(rgb_list)))
 
     cdict = dict()
-    for num, col in enumerate(['red', 'green', 'blue']):
+    for num, col in enumerate(["red", "green", "blue"]):
         cdict[col] = [
             [float_list[i], rgb_list[i][num], rgb_list[i][num]] for i in range(len(float_list))
         ]
     cmap = mcolors.LinearSegmentedColormap(name, segmentdata=cdict, N=256)
 
     return cmap
 
 
 def get_colormap(name):
-
     warnings.warn(
-        'get_colormap is deprecated, use carbonplan_styles.mpl.colormaps instead',
+        "get_colormap is deprecated, use carbonplan_styles.mpl.colormaps instead",
         DeprecationWarning,
     )
 
-    if name == 'blues':
-        return get_continuous_cmap(['#CFE0F9', '#588EF9', '#0432A5'])
-    elif name == 'pinks':
-        return get_continuous_cmap(['#F9C7ED', '#E563BA', '#770361'])
-    elif name == 'reds':
-        return get_continuous_cmap(['#F9D3BD', '#E87A3D', '#752003'])
+    if name == "blues":
+        return get_continuous_cmap(["#CFE0F9", "#588EF9", "#0432A5"])
+    elif name == "pinks":
+        return get_continuous_cmap(["#F9C7ED", "#E563BA", "#770361"])
+    elif name == "reds":
+        return get_continuous_cmap(["#F9D3BD", "#E87A3D", "#752003"])
```

### Comparing `carbonplan-styles-0.4.2/carbonplan_styles/tests/test_mpl.py` & `carbonplan_styles-0.5.1/carbonplan_styles/tests/test_mpl.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,57 +3,57 @@
 import pytest
 from matplotlib import cm
 from matplotlib.colors import ListedColormap
 
 from carbonplan_styles.mpl import colormaps, set_theme
 
 
-@pytest.mark.parametrize('style', ['carbonplan_dark', 'carbonplan_light'])
+@pytest.mark.parametrize("style", ["carbonplan_dark", "carbonplan_light"])
 def test_set_style(style):
     set_theme(style=style)
 
 
 def test_colormaps():
     base_names = [
-        'reds',
-        'oranges',
-        'yellows',
-        'greens',
-        'teals',
-        'blues',
-        'purples',
-        'pinks',
-        'greys',
-        'fire',
-        'earth',
-        'water',
-        'heart',
-        'wind',
-        'warm',
-        'cool',
-        'pinkgreen',
-        'redteal',
-        'orangeblue',
-        'yellowpurple',
-        'redgrey',
-        'orangegrey',
-        'yellowgrey',
-        'greengrey',
-        'tealgrey',
-        'bluegrey',
-        'purplegrey',
-        'pinkgrey',
-        'rainbow',
-        'sinebow',
+        "reds",
+        "oranges",
+        "yellows",
+        "greens",
+        "teals",
+        "blues",
+        "purples",
+        "pinks",
+        "greys",
+        "fire",
+        "earth",
+        "water",
+        "heart",
+        "wind",
+        "warm",
+        "cool",
+        "pinkgreen",
+        "redteal",
+        "orangeblue",
+        "yellowpurple",
+        "redgrey",
+        "orangegrey",
+        "yellowgrey",
+        "greengrey",
+        "tealgrey",
+        "bluegrey",
+        "purplegrey",
+        "pinkgrey",
+        "rainbow",
+        "sinebow",
     ]
 
     explicit_cmaps = colormaps.colormaps()
 
-    for pieces in itertools.product(base_names, ['_light', '_dark'], '', '_r'):
-        cmap_name = ''.join(pieces)
+    for pieces in itertools.product(base_names, ["_light", "_dark"], "", "_r"):
+        cmap_name = "".join(pieces)
 
         exp_cmap = explicit_cmaps[cmap_name]
         assert isinstance(exp_cmap, ListedColormap)
 
         imp_cmap = getattr(colormaps, cmap_name)
         assert isinstance(imp_cmap, ListedColormap)
```

### Comparing `carbonplan-styles-0.4.2/carbonplan_styles.egg-info/SOURCES.txt` & `carbonplan_styles-0.5.1/carbonplan_styles.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,15 @@
-.isort.cfg
+.gitignore
 .pre-commit-config.yaml
 LICENSE
 README.md
-dev-requirements.txt
-requirements.txt
-setup.cfg
-setup.py
+pyproject.toml
 .github/dependabot.yml
 .github/workflows/main.yaml
+.github/workflows/pypi-release.yaml
 carbonplan_styles/__init__.py
 carbonplan_styles/altair.py
 carbonplan_styles/colors.py
 carbonplan_styles.egg-info/PKG-INFO
 carbonplan_styles.egg-info/SOURCES.txt
 carbonplan_styles.egg-info/dependency_links.txt
 carbonplan_styles.egg-info/entry_points.txt
```

### Comparing `carbonplan-styles-0.4.2/demo/theme_demo.ipynb` & `carbonplan_styles-0.5.1/demo/theme_demo.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9966859567901234%*

 * *Differences: {"'cells'": '{3: {\'source\': {insert: [(2, \'c = colors(mode="light")\\n\')], delete: [2]}}, 5: '*

 * *            "{'source': {insert: [(3, 'print(list(colormaps()))')], delete: [3]}}, 6: {'source': "*

 * *            '{insert: [(1, \'plt.pcolor(np.random.random((10, 10)), cmap="redteal_light")\\n\')], '*

 * *            "delete: [1]}}, 8: {'source': {insert: [(1, 'df = pd.read_csv(\\n'), (2, '    "*

 * *            '"https://raw.githubusercontent.com/vega/vega-datasets/master/data/co2-concentration.csv"\\n\'), '*

 * *            […]*

```diff
@@ -57,15 +57,15 @@
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "from carbonplan_styles.colors import colors\n",
                 "\n",
-                "c = colors(mode='light')\n",
+                "c = colors(mode=\"light\")\n",
                 "c"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -85,15 +85,15 @@
                     ]
                 }
             ],
             "source": [
                 "from carbonplan_styles.mpl.colormaps import colormaps\n",
                 "\n",
                 "# print all CarbonPlan colormaps\n",
-                "print(list(colormaps()))\n"
+                "print(list(colormaps()))"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 5,
             "metadata": {},
             "outputs": [
@@ -118,15 +118,15 @@
                         "needs_background": "light"
                     },
                     "output_type": "display_data"
                 }
             ],
             "source": [
                 "# after importing `carbonplan_styles.mpl`, any of the CarbonPlan colormaps can be used in matplotlib\n",
-                "plt.pcolor(np.random.random((10, 10)), cmap='redteal_light')\n",
+                "plt.pcolor(np.random.random((10, 10)), cmap=\"redteal_light\")\n",
                 "plt.colorbar()"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -213,15 +213,17 @@
                     "execution_count": 6,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "# Load some sample data\n",
-                "df = pd.read_csv('https://raw.githubusercontent.com/vega/vega-datasets/master/data/co2-concentration.csv')\n",
+                "df = pd.read_csv(\n",
+                "    \"https://raw.githubusercontent.com/vega/vega-datasets/master/data/co2-concentration.csv\"\n",
+                ")\n",
                 "df.head()"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -251,15 +253,15 @@
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 }
             ],
             "source": [
-                "set_theme(style='carbonplan_dark')\n",
+                "set_theme(style=\"carbonplan_dark\")\n",
                 "\n",
                 "df.plot()"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
@@ -290,15 +292,15 @@
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 }
             ],
             "source": [
-                "set_theme(style='carbonplan_light')\n",
+                "set_theme(style=\"carbonplan_light\")\n",
                 "df.plot()"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -370,19 +372,17 @@
                     },
                     "execution_count": 9,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "alt.themes.enable('carbonplan_dark')\n",
+                "alt.themes.enable(\"carbonplan_dark\")\n",
                 "alt.Chart(df).mark_line().encode(\n",
-                "    x='Date:T',\n",
-                "    y=alt.Y('CO2:Q', scale=alt.Scale(domain=(310, 420))\n",
-                "    )\n",
+                "    x=\"Date:T\", y=alt.Y(\"CO2:Q\", scale=alt.Scale(domain=(310, 420)))\n",
                 ").properties(width=350, height=250)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -454,20 +454,18 @@
                     },
                     "execution_count": 10,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "alt.themes.enable('carbonplan_light')\n",
+                "alt.themes.enable(\"carbonplan_light\")\n",
                 "alt.Chart(df).mark_line().encode(\n",
-                "    x='Date:T',\n",
-                "    y=alt.Y('CO2:Q', scale=alt.Scale(domain=(310, 420))\n",
-                "    )\n",
-                ").properties(width=350, height=250)\n"
+                "    x=\"Date:T\", y=alt.Y(\"CO2:Q\", scale=alt.Scale(domain=(310, 420)))\n",
+                ").properties(width=350, height=250)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
```

