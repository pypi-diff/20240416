# Comparing `tmp/paracelsus-0.5.0.tar.gz` & `tmp/paracelsus-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paracelsus-0.5.0.tar", last modified: Mon Mar 25 01:39:39 2024, max compression
+gzip compressed data, was "paracelsus-0.5.1.tar", last modified: Tue Apr 16 02:53:12 2024, max compression
```

## Comparing `paracelsus-0.5.0.tar` & `paracelsus-0.5.1.tar`

### file list

```diff
@@ -1,63 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 01:39:39.618389 paracelsus-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-03-25 01:39:15.000000 paracelsus-0.5.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 01:39:39.610388 paracelsus-0.5.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-03-25 01:39:15.000000 paracelsus-0.5.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 01:39:39.610388 paracelsus-0.5.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-03-25 01:39:15.000000 paracelsus-0.5.0/.github/workflows/black.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-03-25 01:39:15.000000 paracelsus-0.5.0/.github/workflows/dapperdata.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-03-25 01:39:15.000000 paracelsus-0.5.0/.github/workflows/mypy.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-03-25 01:39:15.000000 paracelsus-0.5.0/.github/workflows/pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-03-25 01:39:15.000000 paracelsus-0.5.0/.github/workflows/pytest.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-03-25 01:39:15.000000 paracelsus-0.5.0/.github/workflows/ruff.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-03-25 01:39:15.000000 paracelsus-0.5.0/.github/workflows/tomlsort.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-03-25 01:39:15.000000 paracelsus-0.5.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-03-25 01:39:15.000000 paracelsus-0.5.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-25 01:39:15.000000 paracelsus-0.5.0/.python-version
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-03-25 01:39:15.000000 paracelsus-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7617 2024-03-25 01:39:39.618389 paracelsus-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5704 2024-03-25 01:39:15.000000 paracelsus-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 01:39:39.610388 paracelsus-0.5.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 01:39:39.610388 paracelsus-0.5.0/docs/dev/
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-03-25 01:39:15.000000 paracelsus-0.5.0/docs/dev/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-03-25 01:39:15.000000 paracelsus-0.5.0/docs/dev/cli.md
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-25 01:39:15.000000 paracelsus-0.5.0/docs/dev/github.md
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-25 01:39:15.000000 paracelsus-0.5.0/docs/dev/pypi.md
--rw-r--r--   0 runner    (1001) docker     (127)    64875 2024-03-25 01:39:15.000000 paracelsus-0.5.0/docs/example.png
--rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-03-25 01:39:15.000000 paracelsus-0.5.0/makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 01:39:39.610388 paracelsus-0.5.0/paracelsus/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-03-25 01:39:15.000000 paracelsus-0.5.0/paracelsus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-25 01:39:39.000000 paracelsus-0.5.0/paracelsus/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     5127 2024-03-25 01:39:15.000000 paracelsus-0.5.0/paracelsus/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-03-25 01:39:15.000000 paracelsus-0.5.0/paracelsus/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-03-25 01:39:15.000000 paracelsus-0.5.0/paracelsus/pyproject.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 01:39:39.614388 paracelsus-0.5.0/paracelsus/transformers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 01:39:15.000000 paracelsus-0.5.0/paracelsus/transformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-03-25 01:39:15.000000 paracelsus-0.5.0/paracelsus/transformers/dot.py
--rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-03-25 01:39:15.000000 paracelsus-0.5.0/paracelsus/transformers/mermaid.py
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-03-25 01:39:15.000000 paracelsus-0.5.0/paracelsus/transformers/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 01:39:39.614388 paracelsus-0.5.0/paracelsus.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7617 2024-03-25 01:39:39.000000 paracelsus-0.5.0/paracelsus.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-03-25 01:39:39.000000 paracelsus-0.5.0/paracelsus.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 01:39:39.000000 paracelsus-0.5.0/paracelsus.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-03-25 01:39:39.000000 paracelsus-0.5.0/paracelsus.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-03-25 01:39:39.000000 paracelsus-0.5.0/paracelsus.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-03-25 01:39:39.000000 paracelsus-0.5.0/paracelsus.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      944 2024-03-25 01:39:15.000000 paracelsus-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-25 01:39:39.618389 paracelsus-0.5.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 01:39:39.614388 paracelsus-0.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 01:39:15.000000 paracelsus-0.5.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 01:39:39.614388 paracelsus-0.5.0/tests/assets/
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-03-25 01:39:15.000000 paracelsus-0.5.0/tests/assets/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 01:39:39.614388 paracelsus-0.5.0/tests/assets/example/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 01:39:15.000000 paracelsus-0.5.0/tests/assets/example/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-03-25 01:39:15.000000 paracelsus-0.5.0/tests/assets/example/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-03-25 01:39:15.000000 paracelsus-0.5.0/tests/assets/example/models.py
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-03-25 01:39:15.000000 paracelsus-0.5.0/tests/assets/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-03-25 01:39:15.000000 paracelsus-0.5.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-03-25 01:39:15.000000 paracelsus-0.5.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-03-25 01:39:15.000000 paracelsus-0.5.0/tests/test_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-03-25 01:39:15.000000 paracelsus-0.5.0/tests/test_pyproject.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 01:39:39.614388 paracelsus-0.5.0/tests/transformers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 01:39:15.000000 paracelsus-0.5.0/tests/transformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-03-25 01:39:15.000000 paracelsus-0.5.0/tests/transformers/test_dot.py
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-03-25 01:39:15.000000 paracelsus-0.5.0/tests/transformers/test_mermaid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:53:12.187562 paracelsus-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-16 02:52:47.000000 paracelsus-0.5.1/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:53:12.179562 paracelsus-0.5.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-16 02:52:47.000000 paracelsus-0.5.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:53:12.179562 paracelsus-0.5.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-16 02:52:47.000000 paracelsus-0.5.1/.github/workflows/black.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-16 02:52:47.000000 paracelsus-0.5.1/.github/workflows/dapperdata.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-16 02:52:47.000000 paracelsus-0.5.1/.github/workflows/mypy.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-16 02:52:47.000000 paracelsus-0.5.1/.github/workflows/pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-16 02:52:47.000000 paracelsus-0.5.1/.github/workflows/pytest.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-16 02:52:47.000000 paracelsus-0.5.1/.github/workflows/ruff.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-16 02:52:47.000000 paracelsus-0.5.1/.github/workflows/tomlsort.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-04-16 02:52:47.000000 paracelsus-0.5.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-16 02:52:47.000000 paracelsus-0.5.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-16 02:52:47.000000 paracelsus-0.5.1/.python-version
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-16 02:52:47.000000 paracelsus-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7662 2024-04-16 02:53:12.187562 paracelsus-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5704 2024-04-16 02:52:47.000000 paracelsus-0.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:53:12.179562 paracelsus-0.5.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:53:12.179562 paracelsus-0.5.1/docs/dev/
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-16 02:52:47.000000 paracelsus-0.5.1/docs/dev/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-16 02:52:47.000000 paracelsus-0.5.1/docs/dev/cli.md
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-16 02:52:47.000000 paracelsus-0.5.1/docs/dev/github.md
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-16 02:52:47.000000 paracelsus-0.5.1/docs/dev/pypi.md
+-rw-r--r--   0 runner    (1001) docker     (127)    64875 2024-04-16 02:52:47.000000 paracelsus-0.5.1/docs/example.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-04-16 02:52:47.000000 paracelsus-0.5.1/makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:53:12.183562 paracelsus-0.5.1/paracelsus/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-16 02:52:47.000000 paracelsus-0.5.1/paracelsus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-16 02:53:12.000000 paracelsus-0.5.1/paracelsus/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5127 2024-04-16 02:52:47.000000 paracelsus-0.5.1/paracelsus/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-16 02:52:47.000000 paracelsus-0.5.1/paracelsus/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-16 02:52:47.000000 paracelsus-0.5.1/paracelsus/pyproject.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:53:12.183562 paracelsus-0.5.1/paracelsus/transformers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 02:52:47.000000 paracelsus-0.5.1/paracelsus/transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-04-16 02:52:47.000000 paracelsus-0.5.1/paracelsus/transformers/dot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-04-16 02:52:47.000000 paracelsus-0.5.1/paracelsus/transformers/mermaid.py
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-16 02:52:47.000000 paracelsus-0.5.1/paracelsus/transformers/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:53:12.187562 paracelsus-0.5.1/paracelsus.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7662 2024-04-16 02:53:12.000000 paracelsus-0.5.1/paracelsus.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-04-16 02:53:12.000000 paracelsus-0.5.1/paracelsus.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 02:53:12.000000 paracelsus-0.5.1/paracelsus.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-16 02:53:12.000000 paracelsus-0.5.1/paracelsus.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-16 02:53:12.000000 paracelsus-0.5.1/paracelsus.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-16 02:53:12.000000 paracelsus-0.5.1/paracelsus.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-04-16 02:52:47.000000 paracelsus-0.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 02:53:12.187562 paracelsus-0.5.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:53:12.183562 paracelsus-0.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 02:52:47.000000 paracelsus-0.5.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:53:12.183562 paracelsus-0.5.1/tests/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-16 02:52:47.000000 paracelsus-0.5.1/tests/assets/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:53:12.183562 paracelsus-0.5.1/tests/assets/example/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 02:52:47.000000 paracelsus-0.5.1/tests/assets/example/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-16 02:52:47.000000 paracelsus-0.5.1/tests/assets/example/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-04-16 02:52:47.000000 paracelsus-0.5.1/tests/assets/example/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-16 02:52:47.000000 paracelsus-0.5.1/tests/assets/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-04-16 02:52:47.000000 paracelsus-0.5.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-04-16 02:52:47.000000 paracelsus-0.5.1/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-16 02:52:47.000000 paracelsus-0.5.1/tests/test_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-16 02:52:47.000000 paracelsus-0.5.1/tests/test_pyproject.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:53:12.187562 paracelsus-0.5.1/tests/transformers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 02:52:47.000000 paracelsus-0.5.1/tests/transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-16 02:52:47.000000 paracelsus-0.5.1/tests/transformers/test_dot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-16 02:52:47.000000 paracelsus-0.5.1/tests/transformers/test_mermaid.py
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-16 02:52:47.000000 paracelsus-0.5.1/tests/utils.py
```

### Comparing `paracelsus-0.5.0/.github/workflows/pypi.yaml` & `paracelsus-0.5.1/.github/workflows/pypi.yaml`

 * *Files identical despite different names*

### Comparing `paracelsus-0.5.0/.gitignore` & `paracelsus-0.5.1/.gitignore`

 * *Files identical despite different names*

### Comparing `paracelsus-0.5.0/.pre-commit-config.yaml` & `paracelsus-0.5.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `paracelsus-0.5.0/LICENSE` & `paracelsus-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `paracelsus-0.5.0/PKG-INFO` & `paracelsus-0.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paracelsus
-Version: 0.5.0
+Version: 0.5.1
 Author: Robert Hafner
 License: MIT License
         
         Copyright (c) 2023, Robert Hafner
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -25,14 +25,15 @@
         SOFTWARE.
         
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pydot
 Requires-Dist: sqlalchemy
 Requires-Dist: typer
+Requires-Dist: toml; python_version < "3.11"
 Provides-Extra: dev
 Requires-Dist: build; extra == "dev"
 Requires-Dist: dapperdata; extra == "dev"
 Requires-Dist: glom; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: pip-tools; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
```

### Comparing `paracelsus-0.5.0/README.md` & `paracelsus-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `paracelsus-0.5.0/docs/example.png` & `paracelsus-0.5.1/docs/example.png`

 * *Files identical despite different names*

### Comparing `paracelsus-0.5.0/makefile` & `paracelsus-0.5.1/makefile`

 * *Files identical despite different names*

### Comparing `paracelsus-0.5.0/paracelsus/cli.py` & `paracelsus-0.5.1/paracelsus/cli.py`

 * *Files identical despite different names*

### Comparing `paracelsus-0.5.0/paracelsus/graph.py` & `paracelsus-0.5.1/paracelsus/graph.py`

 * *Files identical despite different names*

### Comparing `paracelsus-0.5.0/paracelsus/transformers/dot.py` & `paracelsus-0.5.1/paracelsus/transformers/dot.py`

 * *Files identical despite different names*

### Comparing `paracelsus-0.5.0/paracelsus/transformers/mermaid.py` & `paracelsus-0.5.1/paracelsus/transformers/mermaid.py`

 * *Files identical despite different names*

### Comparing `paracelsus-0.5.0/paracelsus.egg-info/PKG-INFO` & `paracelsus-0.5.1/paracelsus.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paracelsus
-Version: 0.5.0
+Version: 0.5.1
 Author: Robert Hafner
 License: MIT License
         
         Copyright (c) 2023, Robert Hafner
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -25,14 +25,15 @@
         SOFTWARE.
         
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pydot
 Requires-Dist: sqlalchemy
 Requires-Dist: typer
+Requires-Dist: toml; python_version < "3.11"
 Provides-Extra: dev
 Requires-Dist: build; extra == "dev"
 Requires-Dist: dapperdata; extra == "dev"
 Requires-Dist: glom; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: pip-tools; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
```

### Comparing `paracelsus-0.5.0/paracelsus.egg-info/SOURCES.txt` & `paracelsus-0.5.1/paracelsus.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 paracelsus/transformers/mermaid.py
 paracelsus/transformers/utils.py
 tests/__init__.py
 tests/conftest.py
 tests/test_cli.py
 tests/test_graph.py
 tests/test_pyproject.py
+tests/utils.py
 tests/assets/README.md
 tests/assets/pyproject.toml
 tests/assets/example/__init__.py
 tests/assets/example/base.py
 tests/assets/example/models.py
 tests/transformers/__init__.py
 tests/transformers/test_dot.py
```

### Comparing `paracelsus-0.5.0/pyproject.toml` & `paracelsus-0.5.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 requires = ["setuptools>=67.0", "setuptools_scm[toml]>=7.1"]
 
 [project]
 authors = [{"name" = "Robert Hafner"}]
 dependencies = [
   "pydot",
   "sqlalchemy",
-  "typer"
+  "typer",
+  "toml; python_version < '3.11'"
 ]
 description = ""
 dynamic = ["version"]
 license = {"file" = "LICENSE"}
 name = "paracelsus"
 readme = {file = "README.md", content-type = "text/markdown"}
```

### Comparing `paracelsus-0.5.0/tests/assets/example/models.py` & `paracelsus-0.5.1/tests/assets/example/models.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,17 @@
-from datetime import UTC, datetime
+from datetime import datetime, timezone
 from uuid import uuid4
 
 from sqlalchemy import Boolean, DateTime, ForeignKey, String, Text, Uuid
 from sqlalchemy.orm import mapped_column
 
 from .base import Base
 
+UTC = timezone.utc
+
 
 class User(Base):
     __tablename__ = "users"
 
     id = mapped_column(Uuid, primary_key=True, default=uuid4())
     display_name = mapped_column(String(100))
     created = mapped_column(DateTime, nullable=False, default=datetime.now(UTC))
@@ -17,15 +19,15 @@
 
 class Post(Base):
     __tablename__ = "posts"
 
     id = mapped_column(Uuid, primary_key=True, default=uuid4())
     author = mapped_column(ForeignKey(User.id), nullable=False)
     created = mapped_column(DateTime, nullable=False, default=datetime.now(UTC))
-    live = mapped_column(Boolean, default=False)
+    live = mapped_column(Boolean, default=False, comment="True if post is published")
     content = mapped_column(Text, default="")
 
 
 class Comment(Base):
     __tablename__ = "comments"
 
     id = mapped_column(Uuid, primary_key=True, default=uuid4())
```

### Comparing `paracelsus-0.5.0/tests/conftest.py` & `paracelsus-0.5.1/tests/conftest.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 import os
-from datetime import UTC, datetime
+import shutil
+import tempfile
+from datetime import datetime, timezone
 from pathlib import Path
 from uuid import uuid4
 
 import pytest
 from sqlalchemy import Boolean, DateTime, ForeignKey, String, Text, Uuid
 from sqlalchemy.orm import declarative_base, mapped_column
 
+UTC = timezone.utc
+
 
 @pytest.fixture
 def metaclass():
     Base = declarative_base()
 
     class User(Base):
         __tablename__ = "users"
@@ -39,8 +43,11 @@
         content = mapped_column(Text, default="")
 
     return Base.metadata
 
 
 @pytest.fixture
 def package_path():
-    return Path(os.path.dirname(os.path.realpath(__file__))) / "assets"
+    template_path = Path(os.path.dirname(os.path.realpath(__file__))) / "assets"
+    with tempfile.TemporaryDirectory() as package_path:
+        shutil.copytree(template_path, package_path, dirs_exist_ok=True)
+        yield Path(package_path)
```

### Comparing `paracelsus-0.5.0/tests/transformers/test_dot.py` & `paracelsus-0.5.1/tests/transformers/test_dot.py`

 * *Files identical despite different names*

