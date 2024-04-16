# Comparing `tmp/xplt-0.7.0.tar.gz` & `tmp/xplt-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xplt-0.7.0.tar", last modified: Tue Feb  6 11:18:15 2024, max compression
+gzip compressed data, was "xplt-0.7.2.tar", last modified: Tue Apr 16 07:16:06 2024, max compression
```

## Comparing `xplt-0.7.0.tar` & `xplt-0.7.2.tar`

### file list

```diff
@@ -1,61 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 11:18:15.969893 xplt-0.7.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 11:18:15.953893 xplt-0.7.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)   306475 2024-02-06 11:18:08.000000 xplt-0.7.0/.github/sampleplot.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 11:18:15.953893 xplt-0.7.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-02-06 11:18:08.000000 xplt-0.7.0/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-02-06 11:18:08.000000 xplt-0.7.0/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-02-06 11:18:08.000000 xplt-0.7.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-02-06 11:18:08.000000 xplt-0.7.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-02-06 11:18:08.000000 xplt-0.7.0/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-02-06 11:18:15.969893 xplt-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-02-06 11:18:08.000000 xplt-0.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 11:18:15.953893 xplt-0.7.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-02-06 11:18:08.000000 xplt-0.7.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-02-06 11:18:08.000000 xplt-0.7.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4046 2024-02-06 11:18:08.000000 xplt-0.7.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 11:18:15.957893 xplt-0.7.0/docs/gallery/
--rw-r--r--   0 runner    (1001) docker     (127)   198024 2024-02-06 11:18:08.000000 xplt-0.7.0/docs/gallery/bpm.png
--rw-r--r--   0 runner    (1001) docker     (127)   220074 2024-02-06 11:18:08.000000 xplt-0.7.0/docs/gallery/floorplot.png
--rw-r--r--   0 runner    (1001) docker     (127)   322259 2024-02-06 11:18:08.000000 xplt-0.7.0/docs/gallery/phasespaceplot.png
--rw-r--r--   0 runner    (1001) docker     (127)   106520 2024-02-06 11:18:08.000000 xplt-0.7.0/docs/gallery/spill.png
--rw-r--r--   0 runner    (1001) docker     (127)   206605 2024-02-06 11:18:08.000000 xplt-0.7.0/docs/gallery/spillquality.png
--rw-r--r--   0 runner    (1001) docker     (127)   186129 2024-02-06 11:18:08.000000 xplt-0.7.0/docs/gallery/twissplot.png
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-02-06 11:18:08.000000 xplt-0.7.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-02-06 11:18:08.000000 xplt-0.7.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-02-06 11:18:08.000000 xplt-0.7.0/docs/quickstart.md
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-02-06 11:18:08.000000 xplt-0.7.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-02-06 11:18:08.000000 xplt-0.7.0/docs/usage.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 11:18:15.965893 xplt-0.7.0/examples/
--rw-r--r--   0 runner    (1001) docker     (127)  2664892 2024-02-06 11:18:08.000000 xplt-0.7.0/examples/animations.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   162997 2024-02-06 11:18:08.000000 xplt-0.7.0/examples/colors.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   190624 2024-02-06 11:18:08.000000 xplt-0.7.0/examples/hamiltonians.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   236063 2024-02-06 11:18:08.000000 xplt-0.7.0/examples/line.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)  1714757 2024-02-06 11:18:08.000000 xplt-0.7.0/examples/phasespace.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   378560 2024-02-06 11:18:08.000000 xplt-0.7.0/examples/properties.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-02-06 11:18:08.000000 xplt-0.7.0/examples/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)   646711 2024-02-06 11:18:08.000000 xplt-0.7.0/examples/timestructure.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   166129 2024-02-06 11:18:08.000000 xplt-0.7.0/examples/twiss.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-02-06 11:18:08.000000 xplt-0.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-06 11:18:15.969893 xplt-0.7.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 11:18:15.965893 xplt-0.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-02-06 11:18:08.000000 xplt-0.7.0/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-02-06 11:18:08.000000 xplt-0.7.0/tests/test_examples.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 11:18:15.969893 xplt-0.7.0/xplt/
--rw-r--r--   0 runner    (1001) docker     (127)      938 2024-02-06 11:18:08.000000 xplt-0.7.0/xplt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    33632 2024-02-06 11:18:08.000000 xplt-0.7.0/xplt/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-02-06 11:18:08.000000 xplt-0.7.0/xplt/colors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-02-06 11:18:08.000000 xplt-0.7.0/xplt/hooks.py
--rw-r--r--   0 runner    (1001) docker     (127)    21811 2024-02-06 11:18:08.000000 xplt-0.7.0/xplt/line.py
--rw-r--r--   0 runner    (1001) docker     (127)    12585 2024-02-06 11:18:08.000000 xplt-0.7.0/xplt/particles.py
--rw-r--r--   0 runner    (1001) docker     (127)    28161 2024-02-06 11:18:08.000000 xplt-0.7.0/xplt/phasespace.py
--rw-r--r--   0 runner    (1001) docker     (127)    13108 2024-02-06 11:18:08.000000 xplt-0.7.0/xplt/properties.py
--rw-r--r--   0 runner    (1001) docker     (127)    60304 2024-02-06 11:18:08.000000 xplt-0.7.0/xplt/timestructure.py
--rw-r--r--   0 runner    (1001) docker     (127)     6099 2024-02-06 11:18:08.000000 xplt-0.7.0/xplt/twiss.py
--rw-r--r--   0 runner    (1001) docker     (127)    15100 2024-02-06 11:18:08.000000 xplt-0.7.0/xplt/util.py
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-02-06 11:18:08.000000 xplt-0.7.0/xplt/xplt.mplstyle
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 11:18:15.969893 xplt-0.7.0/xplt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-02-06 11:18:15.000000 xplt-0.7.0/xplt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-02-06 11:18:15.000000 xplt-0.7.0/xplt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-06 11:18:15.000000 xplt-0.7.0/xplt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-02-06 11:18:15.000000 xplt-0.7.0/xplt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-06 11:18:15.000000 xplt-0.7.0/xplt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:16:06.061430 xplt-0.7.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:16:06.045430 xplt-0.7.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)   306475 2024-04-16 07:16:01.000000 xplt-0.7.2/.github/sampleplot.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:16:06.045430 xplt-0.7.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-04-16 07:16:01.000000 xplt-0.7.2/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-16 07:16:01.000000 xplt-0.7.2/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-04-16 07:16:01.000000 xplt-0.7.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-16 07:16:01.000000 xplt-0.7.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-16 07:16:01.000000 xplt-0.7.2/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-16 07:16:01.000000 xplt-0.7.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14610 2024-04-16 07:16:06.061430 xplt-0.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-16 07:16:01.000000 xplt-0.7.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:16:06.045430 xplt-0.7.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-16 07:16:01.000000 xplt-0.7.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-16 07:16:01.000000 xplt-0.7.2/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4046 2024-04-16 07:16:01.000000 xplt-0.7.2/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:16:06.049430 xplt-0.7.2/docs/gallery/
+-rw-r--r--   0 runner    (1001) docker     (127)   198024 2024-04-16 07:16:01.000000 xplt-0.7.2/docs/gallery/bpm.png
+-rw-r--r--   0 runner    (1001) docker     (127)   220074 2024-04-16 07:16:01.000000 xplt-0.7.2/docs/gallery/floorplot.png
+-rw-r--r--   0 runner    (1001) docker     (127)   322259 2024-04-16 07:16:01.000000 xplt-0.7.2/docs/gallery/phasespaceplot.png
+-rw-r--r--   0 runner    (1001) docker     (127)   106520 2024-04-16 07:16:01.000000 xplt-0.7.2/docs/gallery/spill.png
+-rw-r--r--   0 runner    (1001) docker     (127)   206605 2024-04-16 07:16:01.000000 xplt-0.7.2/docs/gallery/spillquality.png
+-rw-r--r--   0 runner    (1001) docker     (127)   186129 2024-04-16 07:16:01.000000 xplt-0.7.2/docs/gallery/twissplot.png
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-16 07:16:01.000000 xplt-0.7.2/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-04-16 07:16:01.000000 xplt-0.7.2/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-16 07:16:01.000000 xplt-0.7.2/docs/quickstart.md
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-16 07:16:01.000000 xplt-0.7.2/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-16 07:16:01.000000 xplt-0.7.2/docs/usage.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:16:06.057430 xplt-0.7.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)  2664892 2024-04-16 07:16:01.000000 xplt-0.7.2/examples/animations.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   162997 2024-04-16 07:16:01.000000 xplt-0.7.2/examples/colors.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   190624 2024-04-16 07:16:01.000000 xplt-0.7.2/examples/hamiltonians.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   237021 2024-04-16 07:16:01.000000 xplt-0.7.2/examples/line.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)  1714757 2024-04-16 07:16:01.000000 xplt-0.7.2/examples/phasespace.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   378560 2024-04-16 07:16:01.000000 xplt-0.7.2/examples/properties.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-16 07:16:01.000000 xplt-0.7.2/examples/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   646711 2024-04-16 07:16:01.000000 xplt-0.7.2/examples/timestructure.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   166129 2024-04-16 07:16:01.000000 xplt-0.7.2/examples/twiss.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-04-16 07:16:01.000000 xplt-0.7.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 07:16:06.061430 xplt-0.7.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:16:06.057430 xplt-0.7.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-16 07:16:01.000000 xplt-0.7.2/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-16 07:16:01.000000 xplt-0.7.2/tests/test_examples.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:16:06.061430 xplt-0.7.2/xplt/
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-04-16 07:16:01.000000 xplt-0.7.2/xplt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33673 2024-04-16 07:16:01.000000 xplt-0.7.2/xplt/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-04-16 07:16:01.000000 xplt-0.7.2/xplt/colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-04-16 07:16:01.000000 xplt-0.7.2/xplt/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21493 2024-04-16 07:16:01.000000 xplt-0.7.2/xplt/line.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12585 2024-04-16 07:16:01.000000 xplt-0.7.2/xplt/particles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28161 2024-04-16 07:16:01.000000 xplt-0.7.2/xplt/phasespace.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13108 2024-04-16 07:16:01.000000 xplt-0.7.2/xplt/properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60500 2024-04-16 07:16:01.000000 xplt-0.7.2/xplt/timestructure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6099 2024-04-16 07:16:01.000000 xplt-0.7.2/xplt/twiss.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15100 2024-04-16 07:16:01.000000 xplt-0.7.2/xplt/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-16 07:16:01.000000 xplt-0.7.2/xplt/xplt.mplstyle
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:16:06.061430 xplt-0.7.2/xplt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14610 2024-04-16 07:16:05.000000 xplt-0.7.2/xplt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-04-16 07:16:06.000000 xplt-0.7.2/xplt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 07:16:05.000000 xplt-0.7.2/xplt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-16 07:16:05.000000 xplt-0.7.2/xplt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-16 07:16:05.000000 xplt-0.7.2/xplt.egg-info/top_level.txt
```

### Comparing `xplt-0.7.0/.github/sampleplot.png` & `xplt-0.7.2/.github/sampleplot.png`

 * *Files identical despite different names*

### Comparing `xplt-0.7.0/.github/workflows/release.yaml` & `xplt-0.7.2/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `xplt-0.7.0/.github/workflows/test.yaml` & `xplt-0.7.2/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `xplt-0.7.0/.gitignore` & `xplt-0.7.2/.gitignore`

 * *Files identical despite different names*

### Comparing `xplt-0.7.0/docs/Makefile` & `xplt-0.7.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `xplt-0.7.0/docs/conf.py` & `xplt-0.7.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `xplt-0.7.0/docs/gallery/bpm.png` & `xplt-0.7.2/docs/gallery/bpm.png`

 * *Files identical despite different names*

### Comparing `xplt-0.7.0/docs/gallery/floorplot.png` & `xplt-0.7.2/docs/gallery/floorplot.png`

 * *Files identical despite different names*

### Comparing `xplt-0.7.0/docs/gallery/phasespaceplot.png` & `xplt-0.7.2/docs/gallery/phasespaceplot.png`

 * *Files identical despite different names*

### Comparing `xplt-0.7.0/docs/gallery/spill.png` & `xplt-0.7.2/docs/gallery/spill.png`

 * *Files identical despite different names*

### Comparing `xplt-0.7.0/docs/gallery/spillquality.png` & `xplt-0.7.2/docs/gallery/spillquality.png`

 * *Files identical despite different names*

### Comparing `xplt-0.7.0/docs/gallery/twissplot.png` & `xplt-0.7.2/docs/gallery/twissplot.png`

 * *Files identical despite different names*

### Comparing `xplt-0.7.0/docs/make.bat` & `xplt-0.7.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `xplt-0.7.0/docs/quickstart.md` & `xplt-0.7.2/docs/quickstart.md`

 * *Files identical despite different names*

### Comparing `xplt-0.7.0/docs/usage.md` & `xplt-0.7.2/docs/usage.md`

 * *Files 9% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 examples/timestructure
 examples/animations
 examples/colors
 examples/properties
 ```
 
 :::{tip}
-Xsuite is not an explicit dependency, rather an API assumption on available attributes, indices and units. You can use data from any source, and also custom attributes. See {doc}`examples/units` on how to specify units of custom attributes.
+Xsuite is not an explicit dependency, rather an API assumption on available attributes, indices and units. You can use data from any source, and also custom attributes. See {doc}`examples/properties` on how to specify units of custom attributes.
 
 ```python
 import xplt
 xplt.apply_style()  # use our matplotlib style sheet
 import numpy as np
 import pandas as pd
```

### Comparing `xplt-0.7.0/examples/animations.ipynb` & `xplt-0.7.2/examples/animations.ipynb`

 * *Files identical despite different names*

### Comparing `xplt-0.7.0/examples/colors.ipynb` & `xplt-0.7.2/examples/colors.ipynb`

 * *Files identical despite different names*

### Comparing `xplt-0.7.0/examples/hamiltonians.ipynb` & `xplt-0.7.2/examples/hamiltonians.ipynb`

 * *Files identical despite different names*

### Comparing `xplt-0.7.0/examples/phasespace.ipynb` & `xplt-0.7.2/examples/phasespace.ipynb`

 * *Files identical despite different names*

### Comparing `xplt-0.7.0/examples/properties.ipynb` & `xplt-0.7.2/examples/properties.ipynb`

 * *Files identical despite different names*

### Comparing `xplt-0.7.0/examples/timestructure.ipynb` & `xplt-0.7.2/examples/timestructure.ipynb`

 * *Files identical despite different names*

### Comparing `xplt-0.7.0/examples/twiss.ipynb` & `xplt-0.7.2/examples/twiss.ipynb`

 * *Files identical despite different names*

### Comparing `xplt-0.7.0/pyproject.toml` & `xplt-0.7.2/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -4,22 +4,24 @@
 # Project information
 
 [project]
 name = "xplt"
 description = "Plotting for Xsuite"
 readme = "README.md"
 keywords = ["python"]
-#license = {text = ""}
+license = {file = "LICENSE"}
 authors = [
   { name = "Philipp Niedermayer (github.com/eltos)", email = "eltos@outlook.de" },
 ]
 classifiers = [
     "Development Status :: 4 - Beta",
-#    "License :: ",
+    "License :: OSI Approved :: Apache Software License",
     "Topic :: Scientific/Engineering :: Physics",
+    "Topic :: Scientific/Engineering :: Visualization",
+    "Framework :: Matplotlib",
     "Programming Language :: Python :: 3",
 ]
 
 requires-python = ">=3.8"
 dependencies = [
     "matplotlib>=3.6",
     "numpy",
```

### Comparing `xplt-0.7.0/tests/test_examples.py` & `xplt-0.7.2/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `xplt-0.7.0/xplt/__init__.py` & `xplt-0.7.2/xplt/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 __author__ = "Philipp Niedermayer"
 __contact__ = "eltos@outlook.de"
 
 
-__version__ = "0.7.0"
+__version__ = "0.7.2"
 
 # allow usage of xplt.mpl.* without importing matplotlib
 import matplotlib as mpl
 
 from .properties import register_data_property, register_derived_property
 from .colors import *
 from .line import KnlPlot, FloorPlot
```

### Comparing `xplt-0.7.0/xplt/base.py` & `xplt-0.7.2/xplt/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -761,15 +761,16 @@
                 for h in handles:
                     if main_handle := getattr(h, "_join_legend_entry_with", None):
                         handle_map[main_handle].append(h)
                 handles = [tuple(hs) for hs in handle_map.values()]
                 labels = [h.get_label() for h in handle_map]
 
                 # show legend
-                ax.legend(handles=handles, labels=labels, **kwargs)
+                if len(handles) > 0:
+                    ax.legend(handles=handles, labels=labels, **kwargs)
 
     def autoscale(self, subplot="all", *, reset=False, freeze=True, tight=None):
         """Autoscale the axes of a subplot
 
         Args:
             subplot (int | iterable | str): Subplot axis index, indices or "all"
             reset (bool): Whether to ignore any data limits already registered.
```

### Comparing `xplt-0.7.0/xplt/colors.py` & `xplt-0.7.2/xplt/colors.py`

 * *Files identical despite different names*

### Comparing `xplt-0.7.0/xplt/hooks.py` & `xplt-0.7.2/xplt/hooks.py`

 * *Files identical despite different names*

### Comparing `xplt-0.7.0/xplt/line.py` & `xplt-0.7.2/xplt/line.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,19 @@
 
 
 def order(knl):
     """Get order of knl string as int"""
     return int(re.match(r"k(\d+)l", knl).group(1))
 
 
+def tanc(x):
+    """Tangens cardinalis, i.e. tan(x)/x with limit tanc(0)=1"""
+    return np.sinc(x) / np.cos(x)
+
+
 class KnlPlot(XManifoldPlot):
     """A plot for knl values along line"""
 
     def __init__(
         self, line=None, *, knl=None, filled=True, resolution=1000, line_length=None, **kwargs
     ):
         """
@@ -390,27 +395,19 @@
                     length = box_style.pop("length", 0)
                     if box_style.get("label") in legend_entries:
                         box_style.pop("label")  # prevent duplicate legend entries
                     else:
                         legend_entries.append(box_style.get("label"))
 
                     # Handle thick elements
-                    if is_thick and i + 1 < len(X):
-                        # Find the center of the arc
-                        x_mid = 0.5 * (x + X[i + 1])
-                        y_mid = 0.5 * (y + Y[i + 1])
-                        dr = np.array([X[i + 1] - x, Y[i + 1] - y, 0])
-                        dn = np.cross(dr, [0, 0, 1])
-                        dn /= np.linalg.norm(dn)
-                        d = np.linalg.norm(dr) / 2
-                        sin_theta = np.abs(d * arc / length)
-                        dh = d * sin_theta
-                        p_center = np.array([x_mid, y_mid, 0]) - helicity * dh * dn
-                        x = p_center[0]
-                        y = p_center[1]
+                    if is_thick:
+                        # Find the center of single kick for equivalent thin element
+                        d = length * tanc(arc / 2) / 2
+                        x += d * np.cos(ang(rt))
+                        y += d * np.sin(ang(rt))
 
                     if length > 0 and arc:
                         # bending elements as wedge
                         rho = length / arc
                         box = mpl.patches.Wedge(
                             **defaults_for(
                                 mpl.patches.Wedge,
```

### Comparing `xplt-0.7.0/xplt/particles.py` & `xplt-0.7.2/xplt/particles.py`

 * *Files identical despite different names*

### Comparing `xplt-0.7.0/xplt/phasespace.py` & `xplt-0.7.2/xplt/phasespace.py`

 * *Files identical despite different names*

### Comparing `xplt-0.7.0/xplt/properties.py` & `xplt-0.7.2/xplt/properties.py`

 * *Files identical despite different names*

### Comparing `xplt-0.7.0/xplt/timestructure.py` & `xplt-0.7.2/xplt/timestructure.py`

 * *Files 0% similar despite different names*

```diff
@@ -717,15 +717,15 @@
                     # calculate histogram
                     counts, edges = np.histogram(
                         delay,
                         bins=self.bin_count,
                         range=(0, self.bin_count * self.bin_time),
                         weights=weights,
                     )
-                    counts = counts.astype(np.float)
+                    counts = counts.astype(float)
                     if p in ("rate", "current"):
                         counts /= self.bin_time
                     if self.relative:
                         counts /= len(delay)
                     counts *= self.factor_for(p)
 
                     # update plot
@@ -837,14 +837,18 @@
             twin_is_duty (bool): True if cv data is on `ax` and duty data is on `at`. False if that is swapped.
             orientation (str): "x" if data is on x-axis, "y" otherwise
             factor_cv (float): Optional factor associated with cv axis
             factor_duty (float): Optional factor associated with duty axis
         """
         xy = "x" if orientation[0].lower() in "xh" else "y"
         ax_cv, ax_duty = (ax, at) if twin_is_duty else (at, ax)
+        if getattr(ax, f"get_{xy}scale")() != "linear":
+            raise NotImplementedError(
+                "Linked cv and duty axes are only supported for linear scaling!"
+            )
 
         cv2duty = lambda cv: factor_duty / (1 + (cv / factor_cv) ** 2)
         duty2cv = lambda du: factor_cv * (factor_duty / du - 1) ** 0.5
 
         # cv axis
         axis_cv = getattr(ax_cv, f"{xy}axis")
         prop_cv = MetricesMixin._metric_properties.get("cv")
@@ -1304,17 +1308,17 @@
             # calculate metric on sliding window
             stride = min(self.counting_bins_per_evaluation or N.size, N.size)
             N = np.lib.stride_tricks.sliding_window_view(N, stride)
 
             for metric in F.keys():
                 # calculate metrics
                 v, lim = self._calculate_metric(N, metric, axis=1)
-                F[metric][i] = np.mean(v)
-                F_std[metric][i] = np.std(v) or np.nan
-                F_poisson[metric][i] = np.mean(lim)
+                F[metric][i] = np.nanmean(v)
+                F_std[metric][i] = np.nanstd(v) or np.nan
+                F_poisson[metric][i] = np.nanmean(lim)
 
         DT = DT * self.factor_for(self.on_x)
 
         # update plots
         changed = []
         for i, ppp in enumerate(self.on_y):
             for j, pp in enumerate(ppp):
```

### Comparing `xplt-0.7.0/xplt/twiss.py` & `xplt-0.7.2/xplt/twiss.py`

 * *Files identical despite different names*

### Comparing `xplt-0.7.0/xplt/util.py` & `xplt-0.7.2/xplt/util.py`

 * *Files identical despite different names*

### Comparing `xplt-0.7.0/xplt.egg-info/SOURCES.txt` & `xplt-0.7.2/xplt.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 .gitignore
 .pre-commit-config.yaml
 CITATION.cff
+LICENSE
 README.md
 pyproject.toml
 .github/sampleplot.png
 .github/workflows/release.yaml
 .github/workflows/test.yaml
 docs/Makefile
 docs/api.rst
```

