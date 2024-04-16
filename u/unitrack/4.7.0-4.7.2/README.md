# Comparing `tmp/unitrack-4.7.0.tar.gz` & `tmp/unitrack-4.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unitrack-4.7.0.tar", last modified: Fri Jan 26 13:30:00 2024, max compression
+gzip compressed data, was "unitrack-4.7.2.tar", last modified: Tue Apr 16 11:56:53 2024, max compression
```

## Comparing `unitrack-4.7.0.tar` & `unitrack-4.7.2.tar`

### file list

```diff
@@ -1,35 +1,40 @@
-drwxrwxr-x   0 kurt      (1003) kurt      (1003)        0 2024-01-26 13:30:00.271302 unitrack-4.7.0/
--rw-rw-r--   0 kurt      (1003) kurt      (1003)     1068 2023-12-11 16:48:07.000000 unitrack-4.7.0/LICENSE
--rw-r--r--   0 kurt      (1003) kurt      (1003)     6059 2024-01-26 13:30:00.271302 unitrack-4.7.0/PKG-INFO
--rw-rw-r--   0 kurt      (1003) kurt      (1003)     4294 2023-12-11 16:48:07.000000 unitrack-4.7.0/README.md
--rw-rw-r--   0 kurt      (1003) kurt      (1003)     6373 2023-12-11 16:48:07.000000 unitrack-4.7.0/pyproject.toml
--rw-rw-r--   0 kurt      (1003) kurt      (1003)       38 2024-01-26 13:30:00.271302 unitrack-4.7.0/setup.cfg
-drwxrwxr-x   0 kurt      (1003) kurt      (1003)        0 2024-01-26 13:30:00.267302 unitrack-4.7.0/sources/
-drwxrwxr-x   0 kurt      (1003) kurt      (1003)        0 2024-01-26 13:30:00.267302 unitrack-4.7.0/sources/unitrack/
--rw-rw-r--   0 kurt      (1003) kurt      (1003)      860 2024-01-26 13:29:43.000000 unitrack-4.7.0/sources/unitrack/__init__.py
-drwxrwxr-x   0 kurt      (1003) kurt      (1003)        0 2024-01-26 13:30:00.267302 unitrack-4.7.0/sources/unitrack/assignment/
--rw-rw-r--   0 kurt      (1003) kurt      (1003)      275 2023-12-11 16:48:07.000000 unitrack-4.7.0/sources/unitrack/assignment/__init__.py
--rw-rw-r--   0 kurt      (1003) kurt      (1003)     3512 2023-12-11 16:48:07.000000 unitrack-4.7.0/sources/unitrack/assignment/auction.py
--rw-rw-r--   0 kurt      (1003) kurt      (1003)     1470 2023-12-11 16:48:07.000000 unitrack-4.7.0/sources/unitrack/assignment/base_assignment.py
--rw-rw-r--   0 kurt      (1003) kurt      (1003)     2357 2023-12-11 16:48:07.000000 unitrack-4.7.0/sources/unitrack/assignment/greedy.py
--rw-rw-r--   0 kurt      (1003) kurt      (1003)     2254 2023-12-11 16:48:07.000000 unitrack-4.7.0/sources/unitrack/assignment/hungarian.py
--rw-rw-r--   0 kurt      (1003) kurt      (1003)     1349 2023-12-11 16:48:07.000000 unitrack-4.7.0/sources/unitrack/assignment/jonker.py
--rw-rw-r--   0 kurt      (1003) kurt      (1003)      190 2023-12-11 16:48:07.000000 unitrack-4.7.0/sources/unitrack/constants.py
--rw-rw-r--   0 kurt      (1003) kurt      (1003)    10436 2024-01-04 12:44:35.000000 unitrack-4.7.0/sources/unitrack/costs.py
--rw-rw-r--   0 kurt      (1003) kurt      (1003)     6271 2023-12-11 16:48:07.000000 unitrack-4.7.0/sources/unitrack/memory.py
-drwxrwxr-x   0 kurt      (1003) kurt      (1003)        0 2024-01-26 13:30:00.267302 unitrack-4.7.0/sources/unitrack/stages/
--rw-rw-r--   0 kurt      (1003) kurt      (1003)      128 2023-12-11 16:48:07.000000 unitrack-4.7.0/sources/unitrack/stages/__init__.py
--rw-rw-r--   0 kurt      (1003) kurt      (1003)     1966 2023-12-11 16:48:07.000000 unitrack-4.7.0/sources/unitrack/stages/association.py
--rw-rw-r--   0 kurt      (1003) kurt      (1003)      845 2023-12-11 16:48:07.000000 unitrack-4.7.0/sources/unitrack/stages/base_stage.py
--rw-rw-r--   0 kurt      (1003) kurt      (1003)     1318 2023-12-11 16:48:07.000000 unitrack-4.7.0/sources/unitrack/stages/lost.py
-drwxrwxr-x   0 kurt      (1003) kurt      (1003)        0 2024-01-26 13:30:00.267302 unitrack-4.7.0/sources/unitrack/states/
--rw-rw-r--   0 kurt      (1003) kurt      (1003)      127 2023-12-11 16:48:07.000000 unitrack-4.7.0/sources/unitrack/states/__init__.py
--rw-rw-r--   0 kurt      (1003) kurt      (1003)     1666 2023-12-11 16:48:07.000000 unitrack-4.7.0/sources/unitrack/states/base_state.py
--rw-rw-r--   0 kurt      (1003) kurt      (1003)     2157 2023-12-11 16:48:07.000000 unitrack-4.7.0/sources/unitrack/states/value.py
--rw-rw-r--   0 kurt      (1003) kurt      (1003)     2356 2023-12-11 16:48:07.000000 unitrack-4.7.0/sources/unitrack/tracker.py
-drwxrwxr-x   0 kurt      (1003) kurt      (1003)        0 2024-01-26 13:30:00.267302 unitrack-4.7.0/sources/unitrack.egg-info/
--rw-r--r--   0 kurt      (1003) kurt      (1003)     6059 2024-01-26 13:30:00.000000 unitrack-4.7.0/sources/unitrack.egg-info/PKG-INFO
--rw-rw-r--   0 kurt      (1003) kurt      (1003)      866 2024-01-26 13:30:00.000000 unitrack-4.7.0/sources/unitrack.egg-info/SOURCES.txt
--rw-rw-r--   0 kurt      (1003) kurt      (1003)        1 2024-01-26 13:30:00.000000 unitrack-4.7.0/sources/unitrack.egg-info/dependency_links.txt
--rw-rw-r--   0 kurt      (1003) kurt      (1003)      425 2024-01-26 13:30:00.000000 unitrack-4.7.0/sources/unitrack.egg-info/requires.txt
--rw-rw-r--   0 kurt      (1003) kurt      (1003)        9 2024-01-26 13:30:00.000000 unitrack-4.7.0/sources/unitrack.egg-info/top_level.txt
+drwxrwxr-x   0 kurt      (1003) kurt      (1003)        0 2024-04-16 11:56:53.297855 unitrack-4.7.2/
+-rw-rw-r--   0 kurt      (1003) kurt      (1003)     1068 2023-12-11 16:48:07.000000 unitrack-4.7.2/LICENSE
+-rw-r--r--   0 kurt      (1003) kurt      (1003)     7643 2024-04-16 11:56:53.297855 unitrack-4.7.2/PKG-INFO
+-rw-rw-r--   0 kurt      (1003) kurt      (1003)     4294 2023-12-11 16:48:07.000000 unitrack-4.7.2/README.md
+-rw-rw-r--   0 kurt      (1003) kurt      (1003)     9170 2024-04-14 20:03:23.000000 unitrack-4.7.2/pyproject.toml
+-rw-rw-r--   0 kurt      (1003) kurt      (1003)       38 2024-04-16 11:56:53.297855 unitrack-4.7.2/setup.cfg
+drwxrwxr-x   0 kurt      (1003) kurt      (1003)        0 2024-04-16 11:56:53.289854 unitrack-4.7.2/sources/
+drwxrwxr-x   0 kurt      (1003) kurt      (1003)        0 2024-04-16 11:56:53.289854 unitrack-4.7.2/sources/unitrack/
+-rw-rw-r--   0 kurt      (1003) kurt      (1003)      857 2024-04-16 11:56:25.000000 unitrack-4.7.2/sources/unitrack/__init__.py
+-rw-rw-r--   0 kurt      (1003) kurt      (1003)    13643 2024-04-11 08:12:11.000000 unitrack-4.7.2/sources/unitrack/_memory.py
+-rw-rw-r--   0 kurt      (1003) kurt      (1003)     4925 2024-04-09 10:30:16.000000 unitrack-4.7.2/sources/unitrack/_stateful.py
+-rw-rw-r--   0 kurt      (1003) kurt      (1003)     3422 2024-04-11 08:12:09.000000 unitrack-4.7.2/sources/unitrack/_tracker.py
+drwxrwxr-x   0 kurt      (1003) kurt      (1003)        0 2024-04-16 11:56:53.293855 unitrack-4.7.2/sources/unitrack/assignment/
+-rw-rw-r--   0 kurt      (1003) kurt      (1003)      323 2024-04-11 08:12:11.000000 unitrack-4.7.2/sources/unitrack/assignment/__init__.py
+-rw-rw-r--   0 kurt      (1003) kurt      (1003)     4150 2024-04-11 08:12:11.000000 unitrack-4.7.2/sources/unitrack/assignment/_auction.py
+-rw-rw-r--   0 kurt      (1003) kurt      (1003)     1549 2024-04-11 06:46:56.000000 unitrack-4.7.2/sources/unitrack/assignment/_base.py
+-rw-rw-r--   0 kurt      (1003) kurt      (1003)     2413 2024-04-11 08:01:22.000000 unitrack-4.7.2/sources/unitrack/assignment/_greedy.py
+-rw-rw-r--   0 kurt      (1003) kurt      (1003)     3482 2024-04-11 08:12:11.000000 unitrack-4.7.2/sources/unitrack/assignment/_hungarian.py
+-rw-rw-r--   0 kurt      (1003) kurt      (1003)     2519 2024-04-11 08:12:11.000000 unitrack-4.7.2/sources/unitrack/assignment/_jonker.py
+-rw-rw-r--   0 kurt      (1003) kurt      (1003)      689 2024-04-11 08:12:11.000000 unitrack-4.7.2/sources/unitrack/assignment/_utils.py
+-rw-rw-r--   0 kurt      (1003) kurt      (1003)      226 2024-04-09 07:33:16.000000 unitrack-4.7.2/sources/unitrack/consts.py
+-rw-rw-r--   0 kurt      (1003) kurt      (1003)    11371 2024-04-11 08:12:10.000000 unitrack-4.7.2/sources/unitrack/costs.py
+-rw-rw-r--   0 kurt      (1003) kurt      (1003)      427 2024-04-09 10:30:16.000000 unitrack-4.7.2/sources/unitrack/debug.py
+-rw-rw-r--   0 kurt      (1003) kurt      (1003)        0 2024-02-20 07:37:48.000000 unitrack-4.7.2/sources/unitrack/py.typed
+drwxrwxr-x   0 kurt      (1003) kurt      (1003)        0 2024-04-16 11:56:53.293855 unitrack-4.7.2/sources/unitrack/stages/
+-rw-rw-r--   0 kurt      (1003) kurt      (1003)      184 2024-02-28 12:39:53.000000 unitrack-4.7.2/sources/unitrack/stages/__init__.py
+-rw-rw-r--   0 kurt      (1003) kurt      (1003)     1733 2024-04-11 08:12:11.000000 unitrack-4.7.2/sources/unitrack/stages/association.py
+-rw-rw-r--   0 kurt      (1003) kurt      (1003)     2051 2024-04-11 08:12:11.000000 unitrack-4.7.2/sources/unitrack/stages/base_stage.py
+-rw-rw-r--   0 kurt      (1003) kurt      (1003)     1990 2024-04-10 18:23:39.000000 unitrack-4.7.2/sources/unitrack/stages/gate.py
+-rw-rw-r--   0 kurt      (1003) kurt      (1003)     1478 2024-04-10 18:23:39.000000 unitrack-4.7.2/sources/unitrack/stages/lost.py
+drwxrwxr-x   0 kurt      (1003) kurt      (1003)        0 2024-04-16 11:56:53.293855 unitrack-4.7.2/sources/unitrack/states/
+-rw-rw-r--   0 kurt      (1003) kurt      (1003)      163 2024-02-20 07:37:48.000000 unitrack-4.7.2/sources/unitrack/states/__init__.py
+-rw-rw-r--   0 kurt      (1003) kurt      (1003)     1702 2024-02-20 07:37:48.000000 unitrack-4.7.2/sources/unitrack/states/base_state.py
+-rw-rw-r--   0 kurt      (1003) kurt      (1003)     2475 2024-02-28 13:25:59.000000 unitrack-4.7.2/sources/unitrack/states/value.py
+drwxrwxr-x   0 kurt      (1003) kurt      (1003)        0 2024-04-16 11:56:53.293855 unitrack-4.7.2/sources/unitrack.egg-info/
+-rw-r--r--   0 kurt      (1003) kurt      (1003)     7643 2024-04-16 11:56:53.000000 unitrack-4.7.2/sources/unitrack.egg-info/PKG-INFO
+-rw-rw-r--   0 kurt      (1003) kurt      (1003)     1011 2024-04-16 11:56:53.000000 unitrack-4.7.2/sources/unitrack.egg-info/SOURCES.txt
+-rw-rw-r--   0 kurt      (1003) kurt      (1003)        1 2024-04-16 11:56:53.000000 unitrack-4.7.2/sources/unitrack.egg-info/dependency_links.txt
+-rw-rw-r--   0 kurt      (1003) kurt      (1003)      901 2024-04-16 11:56:53.000000 unitrack-4.7.2/sources/unitrack.egg-info/requires.txt
+-rw-rw-r--   0 kurt      (1003) kurt      (1003)        9 2024-04-16 11:56:53.000000 unitrack-4.7.2/sources/unitrack.egg-info/top_level.txt
```

### Comparing `unitrack-4.7.0/LICENSE` & `unitrack-4.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `unitrack-4.7.0/README.md` & `unitrack-4.7.2/README.md`

 * *Files identical despite different names*

### Comparing `unitrack-4.7.0/pyproject.toml` & `unitrack-4.7.2/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [build-system]
-requires = ["setuptools>=61.0"]
+requires = ["setuptools>=68.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "unitrack"
 description = 'A multi-stage object tracking framework'
 readme = "README.md"
 requires-python = ">=3.10"
@@ -15,112 +15,241 @@
     "instance segmentation",
     "semantic segmentation",
 ]
 authors = [{ name = "Kurt Stolle", email = "k.h.w.stolle@gmail.com" }]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Programming Language :: Python",
-    "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: Implementation :: CPython",
 ]
 dependencies = [
-    "torch >= 2.0.0",
+    "torch >= 2.2.2",
     "scikit-learn >= 1.2.2",
-    "tensordict >= 0.1.2",
+    "tensordict >= 0.3.2",
+    "unipercept",
 ]
 
 dynamic = ["version"]
 
 [tool.setuptools.dynamic]
 version = { attr = "unitrack.__version__" }
 
 [tool.setuptools.packages.find]
 where = ["sources"]
-include = ["*"]
-exclude = []
+include = ["uni*"]
+exclude = ["tests"]
+namespaces = true
 
 [project.optional-dependencies]
-docs = ["sphinx", "sphinx-rtd-theme"]
-tests = [
-    "hypothesis",
-    "bandit[toml]==1.7.5",
-    "black==23.1.0",
-    "check-manifest==0.49",
-    "flake8-bugbear==23.3.12",
+qa = [
+    "black>=24.3.0",
+    "bandit[toml]",
+    "check-manifest",
+    "flake8 >= 7.0.0",
+    "flake8-bugbear",
     "flake8-docstrings",
     "flake8-formatter_junit_xml",
-    "flake8",
+    "flake8-import-conventions",
+    "flake8-unused-arguments",
+    "flake8-comprehensions",
+    "flake8-errmsg",
+    "flake8-logging-format",
+    "flake8-pie",
+    "flake8-pyi",
+    "flake8-pytest-style",
+    "flake8-return",
+    "flake8-2020",
+    "flake8-executable",
+    "flake8-simplify",
+    "flake8-black",
     "flake8-pyproject",
-    "pre-commit==3.1.1",
-    "pylint==2.17.0",
-    "pylint_junit",
-    "pytest-cov==4.0.0",
-    "pytest-mock<3.10.1",
+    "pre-commit",
+    "pygrep",
+    "isort >= 5.13.2",
+    "refurb",
+    "pylint >= 3.0.3",
+    "pylint_junit", 
+    "shellcheck-py",
+    "pylint",
+    "mypy >= 1.9.0",
+    "autoflake",
+    "pydocstyle",
+    "pyre-check",
+    "pydocstringformatter",
+    "pyrefact",
+    "pyflakes",
+    "mccabe",
+]
+tests = [
+    "hypothesis >= 6.100.1",
+    "pytest >= 8.1.1",
+    "pytest-sugar",
+    "pytest-xdist",
+    "pytest-benchmark",
+    "pytest-cov",
+    "pytest-mock",
     "pytest-runner",
-    "pytest==7.2.2",
     "pytest-github-actions-annotate-failures",
-    "shellcheck-py==0.9.0.2",
 ]
+notebooks = [
+    "jupyterlab",
+    "ipywidgets",
+    "ipykernel",
+    "ipython-autotime",
+    "matplotlib >= 3.8.4",
+    "seaborn >= 0.13.2",
+]
+docs = ["sphinx", "sphinx-rtd-theme", "numpydoc"]
+
+[tool.pydocstringformatter]
+write = true
+strip-whitespaces = true
+split-summary-body = false
+numpydoc-section-hyphen-length = false
 
 [tool.bandit]
-exclude_dirs = ["build", "dist", "tests", "scripts"]
+exclude_dirs = [
+    "build",
+    "dist",
+    "tests",
+    "scripts",
+    "configs",
+    "docs",
+    "output",
+    "datasets",
+    "dependencies",
+    "benchmarks",
+]
 number = 4
 recursive = true
 targets = "sources"
 
 [tool.black]
-line-length = 120
+line-length = 88
 fast = true
-target-version = ['py310']
+target-version = ['py311']
 
 [tool.coverage.run]
 branch = true
 
 [tool.coverage.report]
 fail_under = 100
 
 [tool.flake8]
-max-line-length = 120
-select = "F,E,W,B,B901,B902,B903"
+docstring-convention = "numpy"
+max-complexity = 50
+max-line-length = 80
+extend-select = [
+    "F",    # flake8
+    "B",    # flake8-bugbear
+    "B901", # 
+    "B902", # 
+    "B903", #
+    "BLK",  # flake8-black
+    "C",    # mccabe
+    "I",    # isort
+    "ARG",  # flake8-unused-arguments
+    "C4",   # flake8-comprehensions
+    "EM",   # flake8-errmsg
+    "ICN",  # flake8-import-conventions
+    "G",    # flake8-logging-format
+    "PGH",  # pygrep-hooks
+    "PIE",  # flake8-pie
+    "PL",   # pylint
+    "PT",   # flake8-pytest-style
+    "PTH",  # flake8-use-pathlib
+    "RET",  # flake8-return
+    "SIM",  # flake8-simplify
+    "T20",  # flake8-print
+    "UP",   # pyupgrade
+    "YTT",  # flake8-2020
+    "EXE",  # flake8-executable
+    "NPY",  # NumPy specific rules
+    "FURB", # refurb
+    "PYI",  # flake8-pyi
+]
+per-file-ignores = """
+    __init__.py: F401, F403
+    __init__.pyi: F401, F403
+    tests/**: T20
+    tests/**/conftest.py: F401, F403, E402
+"""
+extend-ignore = [
+    # "E203", # whitespace before ':'
+    "E501", # line too long
+    # "E722", # do not use bare 'except'
+    # "W503", # line break before binary operator
+    "B001", # assert used
+    "D200", # One-line docstring should fit on one line with quotes
+]
 exclude = [
     ".eggs",
     ".git",
     ".tox",
     "nssm",
     "obj",
     "out",
     "packages",
     "pywin32",
     "tests",
     "swagger_client",
+    # "*.pyi",
 ]
-ignore = ["E722", "B001", "W503", "E203"]
+
 
 [tool.pyright]
 include = ["sources"]
-exclude = ["**/node_modules", "**/__pycache__"]
-venv = "env310"
 reportPrivateImportUsage = false
 reportMissingImports = true
 reportMissingTypeStubs = false
-pythonVersion = "3.10"
+strictListInference = true
+strictSetInference = true
+reportImportCycles = true
+reportMatchNotExhaustive = true
+reportShadowedImports = true
+reportImplicitOverride = "warning"
+pythonVersion = "3.11"
 pythonPlatform = "Linux"
+exclude = ["datasets", "dependencies", "output", "**/prototypes"]
 executionEnvironments = [{ root = "sources" }]
 
+[tool.autoflake]
+check = false
+exclude = [
+    "__init__.py",
+    "tests/**/*",
+    "docs/**.*",
+]
+imports = [
+    "requests",
+    "torch",
+    "transformers",
+    "torchvision",
+    "tensordict",
+    "unitrack",
+    "tensordict",
+    "einops",
+    "timm",
+]
+recursive = true
+ignore_init_module_imports = true
+expand_star_imports = true
+
 [tool.pytest.ini_options]
-addopts = "--cov-report xml:coverage.xml --cov sources --cov-fail-under 0 --cov-append -m 'not integration'"
+addopts = "--doctest-modules -m 'not integration' -m 'not gpu' --benchmark-disable"
 pythonpath = ["sources"]
 testpaths = "tests"
 junit_family = "xunit2"
+junit_suite_name = "tests"
 markers = [
     "integration: marks as integration test",
     "notebooks: marks as notebook test",
     "gpu: marks as gpu test",
-    "spark: marks tests which need Spark",
     "slow: marks tests as slow",
     "unit: fast offline tests",
 ]
 
 [tool.pylint]
 extension-pkg-whitelist = [
     "numpy",
@@ -130,20 +259,21 @@
     "pydantic",
     "ciso8601",
     "netcdf4",
     "scipy",
 ]
 ignore = "CVS"
 ignore-patterns = "test.*?py,conftest.py"
-init-hook = 'import sys; sys.setrecursionlimit(8 * sys.getrecursionlimit())'
+init-hook = 'import sys; sys.setrecursionlimit(4 * sys.getrecursionlimit())'
 jobs = 0
 limit-inference-results = 100
 persistent = "yes"
 suggestion-mode = "yes"
 unsafe-load-any-extension = "no"
+include = ["sources"]
 
 [tool.pylint.'MESSAGES CONTROL']
 enable = "c-extension-no-member"
 
 [tool.pylint.'REPORTS']
 evaluation = "10.0 - ((float(5 * error + warning + refactor + convention) / statement) * 10)"
 output-format = "text"
@@ -172,15 +302,15 @@
 property-classes = "abc.abstractproperty"
 variable-naming-style = "snake_case"
 
 [tool.pylint.'FORMAT']
 ignore-long-lines = "^\\s*(# )?.*['\"]?<?https?://\\S+>?"
 indent-after-paren = 4
 indent-string = '    '
-max-line-length = 120
+max-line-length = 88
 max-module-lines = 1000
 single-line-class-stmt = "no"
 single-line-if-stmt = "no"
 
 [tool.pylint.'LOGGING']
 logging-format-style = "old"
 logging-modules = "logging"
@@ -245,12 +375,17 @@
 analyse-fallback-blocks = "no"
 deprecated-modules = "optparse,tkinter.tix"
 
 [tool.pylint.'EXCEPTIONS']
 overgeneral-exceptions = ["BaseException", "Exception"]
 
 [tool.isort]
-multi_line_output = 5
-include_trailing_comma = true
-force_grid_wrap = 0
-line_length = 80
 profile = "black"
+add_imports = ["from __future__ import annotations"]
+
+[tool.mypy]
+python_version = "3.11"
+strict = true
+disallow_untyped_defs = false
+warn_unused_ignores = true
+check_untyped_defs = false
+no_implicit_optional = true
```

### Comparing `unitrack-4.7.0/sources/unitrack/__init__.py` & `unitrack-4.7.2/sources/unitrack/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 """
-Modules that peform tracking tasks.
+UniTrack
+========
 
-A tracker implements an algorithm to find a mapping from detections to
-tracklets, i.e.:
+This module implements a tracker algorithm that maps detections to tracklets.
 
-    Tracker: Detections --> Tracklets
+.. math::
+
+    Tracker: Detections \rightarrow Tracklets
 
 Each detection has fields that can be used to assign IDs from Tracklets in the
 previous frame to Tracklets in the current frame.
 
 Terminology
 -----------
-Detections
-    All detected structures at the current frame.
-Tracklets
-    All detections from previous frames, having an unique track ID.
-Assignment
-    Process that assigns each Detection to a Tracklet.
-Lost
-    State of a Tracklet that has not been assigned to a detection at the current
-    or a previous frame.
 
+- **Detections**: All detected structures at the current frame.
+
+- **Tracklets**: All detections from previous frames, each having a unique track ID.
+
+- **Assignment**: The process that assigns each Detection to a Tracklet.
+
+- **Lost**: The state of a Tracklet that has not been assigned to a detection at the current
+    or a previous frame.
 """
 
-__version__ = "4.7.0"
+from __future__ import annotations
+
+__version__ = "4.7.2"
 
-from . import assignment, costs, stages, states  # noqa: F401
-from .constants import *  # noqa: F401, F403
-from .memory import *  # noqa: F401, F403
-from .tracker import *  # noqa: F401, F403
+from . import assignment, consts, costs, debug, stages, states
+from ._memory import *
+from ._stateful import *
+from ._tracker import *
```

### Comparing `unitrack-4.7.0/sources/unitrack/assignment/auction.py` & `unitrack-4.7.2/sources/unitrack/assignment/_auction.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,43 +1,62 @@
-from typing import Tuple
+r"""
+Implements the Auction algorithm for solving a linear assignment problem.
+
+The Auction algorithm is an iterative algorithm that solves the linear assignment
+problem by simulating an auction process.
+"""
+
+from __future__ import annotations
+
+import typing as T
 
 import torch
+import torch.fx
+import typing_extensions as TX
 
-from .base_assignment import Assignment
+from ._base import Assignment
 
 __all__ = ["Auction", "auction_assignment"]
 
 
 class Auction(Assignment):
     """
     Solves the linear assignment over a cost matrix using an auction algorithm.
     """
 
-    bid_size: torch.jit.Final[float]
+    bid_size: T.Final[float]
 
     def __init__(self, bid_size=0.05, *args, **kwargs):
         """
         Parameters
         ----------
         bid_size, optional
-            Step size of auction bids, by default None
+            Step size of auction bids, which should be tuned according to the expected
+            domain of the cost matrix.
         """
         super().__init__(*args, **kwargs)
 
         self.bid_size = bid_size
 
-    def _assign(self, cost_matrix: torch.Tensor) -> Tuple[torch.Tensor, torch.Tensor, torch.Tensor]:
+    @TX.override
+    def _assign(
+        self, cost_matrix: torch.Tensor
+    ) -> T.Tuple[torch.Tensor, torch.Tensor, torch.Tensor]:
         return auction_assignment(cost_matrix, self.bid_size)
 
 
-@torch.jit.script_if_tracing
 @torch.no_grad()
-def auction_assignment(cost_matrix: torch.Tensor, bid_size: float) -> Tuple[torch.Tensor, torch.Tensor, torch.Tensor]:
+def auction_assignment(
+    cost_matrix: torch.Tensor, bid_size: float
+) -> T.Tuple[torch.Tensor, torch.Tensor, torch.Tensor]:
+    cost_matrix = cost_matrix * -1  # Convert cost matrix to profit matrix
+    cost_matrix = cost_matrix - cost_matrix.min()  # Normalize cost matrix
+
     # Compute epsilon based on bid_size and the smaller dimension of the cost matrix
-    eps = bid_size / min(cost_matrix.shape)
+    eps = min(bid_size / min(cost_matrix.shape), 1e-3)
 
     device = cost_matrix.device
 
     # Initialize cost, assignments, and bids tensors
     cost = torch.zeros((1, cost_matrix.shape[1]), device=device)
     ass = torch.full((cost_matrix.shape[0],), -1, device=device, dtype=torch.long)
     bids = torch.zeros_like(cost_matrix)
@@ -59,38 +78,50 @@
 
         bid_increments = first_value - second_value + eps
 
         # Reset bids for unassigned rows
         bids.index_fill_(0, unassigned, 0)
         # bids.zero_()
         # Update bids for the highest values
-        bids[unassigned] = bids[unassigned].scatter_(dim=1, index=first_idx.view(-1, 1), src=bid_increments.view(-1, 1))
+        bids[unassigned] = bids[unassigned].scatter_(
+            dim=1, index=first_idx.view(-1, 1), src=bid_increments.view(-1, 1)
+        )
 
         # Get columns with bidders
         have_bidder = (bids > 0).int().sum(dim=0).nonzero().squeeze()
 
         # Get maximum bids and their row indices
         high_bids, high_bidders = bids[:, have_bidder].max(dim=0)
         # high_bidders = unassigned[high_bidders.squeeze()]
         high_bidders = high_bidders.squeeze()
 
         # Update cost matrix with the high bids
         cost[:, have_bidder] += high_bids
 
         # Temporarily unassign rows that were previously assigned to the current winning columns
-        ass[(ass.view(-1, 1) == have_bidder.view(1, -1)).sum(dim=1).nonzero().squeeze()] = -1
+        ass[
+            (ass.view(-1, 1) == have_bidder.view(1, -1)).sum(dim=1).nonzero().squeeze()
+        ] = -1
 
         # Assign high bidders to the winning columns
         ass[high_bidders] = have_bidder.squeeze()
 
         # Set matched rows in the cost matrix to infinity
         # cost_matrix[high_bidders, :] = torch.inf
         # cost_matrix[:, have_bidder] = torch.inf
 
     # Get matches, unmatched_rows, and unmatched_cols
     idx = torch.arange(ass.numel())
     matches = torch.stack([idx, ass], dim=1)
     matches = matches[ass >= 0]
     unmatched_rows = ass[ass < 0]
-    unmatched_cols = (torch.arange(cost_matrix.shape[1])[None, :] != ass[:, None]).all(dim=0).nonzero().squeeze()
+    unmatched_cols = (
+        (torch.arange(cost_matrix.shape[1])[None, :] != ass[:, None])
+        .all(dim=0)
+        .nonzero()
+        .squeeze()
+    )
 
     return matches, unmatched_rows, unmatched_cols
+
+
+torch.fx.wrap("auction_assignment")
```

### Comparing `unitrack-4.7.0/sources/unitrack/assignment/base_assignment.py` & `unitrack-4.7.2/sources/unitrack/assignment/_base.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from abc import abstractmethod
 from typing import Tuple
 
 import torch
 
 __all__ = ["Assignment"]
 
@@ -15,15 +17,17 @@
 
     def __init__(self, threshold: float = torch.inf):
         super().__init__()
 
         self.threshold = threshold
 
     @torch.jit.script_if_tracing
-    def forward(self, cost_matrix: torch.Tensor) -> Tuple[torch.Tensor, torch.Tensor, torch.Tensor]:
+    def forward(
+        self, cost_matrix: torch.Tensor
+    ) -> Tuple[torch.Tensor, torch.Tensor, torch.Tensor]:
         """
         Solve the cost matrix
 
         Parameters
         ----------
         cost_matrix
             Cost matrix (NxM) to solve
@@ -33,23 +37,27 @@
             Tuple of matches (N_match x M_match), unmatched columns and
             unmatched rows
         """
 
         if min(cost_matrix.shape) == 0:
             return self._no_match(cost_matrix)
 
-        cost_matrix = cost_matrix * (cost_matrix < self.threshold).type_as(cost_matrix)
+        cost_matrix = torch.where(cost_matrix < self.threshold, cost_matrix, torch.inf)
 
         return self._assign(cost_matrix)
 
     @staticmethod
-    def _no_match(cost_matrix: torch.Tensor) -> Tuple[torch.Tensor, torch.Tensor, torch.Tensor]:
+    def _no_match(
+        cost_matrix: torch.Tensor,
+    ) -> Tuple[torch.Tensor, torch.Tensor, torch.Tensor]:
         cs_num, ds_num = cost_matrix.shape
         return (
             torch.empty((0, 2), dtype=torch.long),
             torch.arange(cs_num, dtype=torch.long),
             torch.arange(ds_num, dtype=torch.long),
         )
 
     @abstractmethod
-    def _assign(self, cost_matrix: torch.Tensor) -> Tuple[torch.Tensor, torch.Tensor, torch.Tensor]:
+    def _assign(
+        self, cost_matrix: torch.Tensor
+    ) -> Tuple[torch.Tensor, torch.Tensor, torch.Tensor]:
         raise NotImplementedError
```

### Comparing `unitrack-4.7.0/sources/unitrack/assignment/greedy.py` & `unitrack-4.7.2/sources/unitrack/assignment/_greedy.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,41 @@
 """
 Greedy assignment is a simple assignment algorithm that greedily assigns 
 detections to tracklets, by selecting the best match at each step. This
 algorithm is not guaranteed to find the optimal solution, but it is fast
 and simple to implement.
 """
 
+from __future__ import annotations
+
 from typing import Tuple
 
 import torch
+import torch.fx
 
-from .base_assignment import Assignment
+from ._base import Assignment
 
 __all__ = ["Greedy", "greedy_assignment"]
 
 
 class Greedy(Assignment):
     """
     See :func:`.greedy_assignment` for details.
     """
 
-    def _assign(self, cost_matrix: torch.Tensor) -> Tuple[torch.Tensor, torch.Tensor, torch.Tensor]:
+    def _assign(
+        self, cost_matrix: torch.Tensor
+    ) -> Tuple[torch.Tensor, torch.Tensor, torch.Tensor]:
         return greedy_assignment(cost_matrix)
 
 
-@torch.jit.script_if_tracing
 @torch.no_grad()
-def greedy_assignment(cost_matrix: torch.Tensor) -> Tuple[torch.Tensor, torch.Tensor, torch.Tensor]:
+def greedy_assignment(
+    cost_matrix: torch.Tensor,
+) -> Tuple[torch.Tensor, torch.Tensor, torch.Tensor]:
     """
     Performs a greedy assignment algorithm on a cost matrix, assigning pairs of elements (rows and columns) based on
     the minimum cost, with a threshold as the stopping condition.
 
     Parameters
     ----------
     cost_matrix : torch.Tensor
@@ -43,30 +49,34 @@
         A tensor containing the indices of matched row-column pairs.
     unmatched_rows : torch.Tensor
         A tensor containing the indices of unmatched rows.
     unmatched_cols : torch.Tensor
         A tensor containing the indices of unmatched columns.
 
     """
-    N, M = cost_matrix.shape
-    matches = torch.full((min(N, M), 2), -1, dtype=torch.long, device=cost_matrix.device)
-    unmatched_rows = torch.arange(N, dtype=torch.long, device=cost_matrix.device)
-    unmatched_cols = torch.arange(M, dtype=torch.long, device=cost_matrix.device)
-
-    match_count = 0
-    while True:
-        min_val, idx = torch.min(cost_matrix.flatten(), dim=0)
-        row, col = idx // M, idx % M
-
-        if not torch.isfinite(min_val):
-            break
+    with cost_matrix.device:
+        N, M = cost_matrix.shape
+        matches = torch.full((min(N, M), 2), -1, dtype=torch.long)
+        unmatched_rows = torch.arange(N, dtype=torch.long)
+        unmatched_cols = torch.arange(M, dtype=torch.long)
+
+        match_count = 0
+        while True:
+            min_val, idx = torch.min(cost_matrix.flatten(), dim=0)
+            row, col = idx // M, idx % M
+
+            if not torch.isfinite(min_val):
+                break
 
-        matches[match_count] = torch.tensor([row, col], dtype=torch.long, device=cost_matrix.device)
-        match_count += 1
+            matches[match_count] = torch.tensor([row, col], dtype=torch.long)
+            match_count += 1
 
-        cost_matrix[row, :] = torch.inf
-        cost_matrix[:, col] = torch.inf
+            cost_matrix[row, :] = torch.inf
+            cost_matrix[:, col] = torch.inf
 
-    unmatched_rows = unmatched_rows[torch.isfinite(cost_matrix[:, 0])]
-    unmatched_cols = unmatched_cols[torch.isfinite(cost_matrix[0, :])]
+        unmatched_rows = unmatched_rows[torch.isfinite(cost_matrix[:, 0])]
+        unmatched_cols = unmatched_cols[torch.isfinite(cost_matrix[0, :])]
 
     return matches[:match_count], unmatched_rows, unmatched_cols
+
+
+torch.fx.wrap("greedy_assignment")
```

### Comparing `unitrack-4.7.0/sources/unitrack/assignment/hungarian.py` & `unitrack-4.7.2/sources/unitrack/assignment/_jonker.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,69 +1,80 @@
-"""
-PyTorch implementation of the Hungarian algorithm for solving the assignment problem.
-"""
+from __future__ import annotations
 
 from typing import Tuple
 
+import numpy as np
 import torch
-from torch import Tensor
+import torch.fx
 
-from .base_assignment import Assignment
+from ._base import Assignment
 
-__all__ = ["Hungarian", "hungarian_assignment"]
+__all__ = ["Jonker", "jonker_volgenant_assignment"]
 
 
-class Hungarian(Assignment):
-    def _assign(self, cost_matrix: Tensor) -> Tuple[Tensor, Tensor, Tensor]:
-        """
-        Solves the assignment problem using the Hungarian algorithm.
+class Jonker(Assignment):
+    """
+    Uses the Jonker-Volgenant algorithm to solve the linear assignment problem.
+    """
 
-        Parameters
-        ----------
-        cost_matrix
-            Cost matrix
+    def _assign(
+        self, cost_matrix: torch.Tensor
+    ) -> Tuple[torch.Tensor, torch.Tensor, torch.Tensor]:
+        return jonker_volgenant_assignment(cost_matrix, self.threshold)
 
-        Returns
-        -------
-            Tuple of the optimal assignment and the total assignment cost.
-        """
-        return hungarian_assignment(cost_matrix)
 
+def jonker_volgenant_assignment(
+    cost_matrix: torch.Tensor, threshold: float
+) -> Tuple[torch.Tensor, torch.Tensor, torch.Tensor]:
+    """
+    Perform linear assignment. If possible, an assignment on the diagonal of the
+    matrix is preferred if this assignment has equal cost to the algorithm
+    result.
 
-@torch.jit.script_if_tracing
-@torch.no_grad()
-def hungarian_assignment(cost_matrix: Tensor) -> Tuple[Tensor, Tensor, Tensor]:
-    N, M = cost_matrix.shape
+    TODO: PyTorch implementation
+    """
 
-    # Step 1: Subtract the minimum value from each row
-    cost_matrix -= cost_matrix.min(dim=1, keepdim=True).values
+    from lap import lapjv
 
-    # Step 2: Subtract the minimum value from each column
-    cost_matrix -= cost_matrix.min(dim=0, keepdim=True).values
+    device = cost_matrix.device
+    cost_matrix = cost_matrix.detach().cpu().contiguous()
+    cost_matrix = np.ascontiguousarray(cost_matrix).astype(np.float64)
+    cost_matrix = np.where(np.isfinite(cost_matrix), cost_matrix, np.inf)
+    matches, unmatched_a, unmatched_b = [], [], []
 
-    mask = torch.zeros_like(cost_matrix, dtype=torch.bool)
-    row_mask = torch.ones(N, dtype=torch.bool)
-    col_mask = torch.ones(M, dtype=torch.bool)
+    # Jonker algorithm, i.e. linear sum assignment (rows) -> (cols)
+    cost, x, y = lapjv(cost_matrix, extend_cost=True, cost_limit=threshold)
 
-    while True:
-        # Step 3: Find zeros that have no other zeros in the same row or column
-        mask[row_mask] = cost_matrix[row_mask] == 0
-        mask[:, col_mask] = mask[:, col_mask] * (cost_matrix[:, col_mask] == 0)
+    # Create match and unassigned lists
+    for ix in range(x.shape[0]):
+        mx = x[ix]
+        if mx < 0:
+            continue
+        c = cost_matrix[ix, mx]
+        if not np.isfinite(c):
+            continue
+        matches.append([ix, mx])
 
-        # Step 4: If there are enough zeros, terminate
-        if mask.sum() >= min(N, M):
-            break
+    unmatched_a = torch.from_numpy(np.where(x < 0)[0]).clone().long()
+    unmatched_b = torch.from_numpy(np.where(y < 0)[0]).clone().long()
+    matches = torch.from_numpy(np.asarray(matches)).clone().long()
 
-        # Step 5: Otherwise, update cost matrix by adding the minimum uncovered value
-        min_val = cost_matrix[row_mask][:, col_mask].min()
-        cost_matrix[row_mask] -= min_val
-        cost_matrix[:, ~col_mask] += min_val
+    # NOTE: Too verbose. Needs revision
+    # if check_debug_enabled():
+    #     print(f"Jonker-Volgenant Assignment completed with total cost: {cost}")
+    #     for i, j in matches:
+    #         print(f"- match: C {i} -> D {j} (cost: {cost_matrix[i,j]})")
 
-    # Extract matched row and column indices
-    rows, cols = torch.where(mask)
-    matches = torch.stack((rows, cols), dim=1)
+    #     unmatch_min_cost = [
+    #         f"{i} (min. cost: {cost_matrix[i, :].min()})" for i in unmatched_a
+    #     ]
+    #     print(f"Unmatched C: {unmatch_min_cost}")
 
-    # Identify unmatched rows and columns
-    unmatched_rows = torch.tensor([i for i in range(N) if not (rows == i).any()], device=cost_matrix.device)
-    unmatched_cols = torch.tensor([j for j in range(M) if not (cols == j).any()], device=cost_matrix.device)
+    #     unmatch_min_cost = [
+    #         f"{i} (min. cost: {cost_matrix[:, i].min()})" for i in unmatched_b
+    #     ]
+    #     print(f"Unmatched D: {unmatch_min_cost}")
 
-    return matches, unmatched_rows, unmatched_cols
+    return matches.to(device), unmatched_a.to(device), unmatched_b.to(device)
+
+
+torch.fx.wrap("jonker_volgenant_assignment")
```

### Comparing `unitrack-4.7.0/sources/unitrack/costs.py` & `unitrack-4.7.2/sources/unitrack/costs.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,32 @@
 """
 This package implements the cost functions that are used to compute the assignment costs between tracklets and
 detections.
 """
 
-from abc import abstractmethod
+from __future__ import annotations
 
-import typing as T
 import enum as E
 import itertools
+import typing as T
+from abc import abstractmethod
+from re import I
+
 import torch
 import torch.nn as nn
+import typing_extensions as TX
 from tensordict import TensorDictBase
-
+from torchvision.ops import box_iou
 
 __all__ = []
 
+# ---------------- #
+# Abstract classes #
+# ---------------- #
+
 
 class Cost(torch.nn.Module):
     """
     A cost module computes an assignment cost matrix between detections and
     tracklets.
     """
 
@@ -26,14 +34,15 @@
 
     def __init__(self, required_fields: T.Iterable[str]):
         super().__init__()
 
         self.required_fields = list(set(required_fields))
 
     @abstractmethod
+    @TX.override
     def forward(self, cs: TensorDictBase, ds: TensorDictBase) -> torch.Tensor:
         """
         Computes the assignment costs between previous tracklets and current
         detections.
 
         This is an abstract method that should be overwritten.
 
@@ -47,23 +56,46 @@
         -------
             Cost matrix (N x M).
         """
         raise NotImplementedError
 
 
 class FieldCost(Cost):
-    field: torch.jit.Final[str]
+    field: T.Final[str]
+    select: T.Final[T.List[int]]
 
-    def __init__(self, field: str):
+    def __init__(self, field: str, select: T.Iterable[int] | None = None):
         super().__init__(required_fields=[field])
 
         self.field = field
+        if select is None:
+            select = []
+        else:
+            select = list(select)
+        self.select = select
+
+    def get_field(
+        self, cs: TensorDictBase, ds: TensorDictBase
+    ) -> T.Tuple[torch.Tensor, torch.Tensor]:
+        ts_field = cs.get(self.field)
+        ds_field = ds.get(self.field)
 
-    def forward(self, cs: TensorDictBase, ds: TensorDictBase) -> torch.Tensor:
-        return self.compute(cs.get(self.field), ds.get(self.field))
+        if len(self.select) > 0:
+            assert ts_field.shape[1] >= max(self.select)
+            assert ds_field.shape[1] >= max(self.select)
+
+            ts_field = ts_field[:, self.select]
+            ds_field = ds_field[:, self.select]
+
+        return ts_field, ds_field
+
+    @TX.override
+    def forward(self, cs: TensorDictBase, ds: TensorDictBase):
+        ts_field, ds_field = self.get_field(cs, ds)
+        return self.compute(ts_field, ds_field)
 
     @abstractmethod
     def compute(self, cs: torch.Tensor, ds: torch.Tensor) -> torch.Tensor:
         """
         Computes the assignment costs between previous tracklets and current
         detections.
 
@@ -76,57 +108,85 @@
         ds
             Detections (M) values for a single field.
 
         Returns
         -------
             Cost matrix (N x M).
         """
-        raise NotImplementedError
+        ...
+
+
+# ------------------- #
+# Category gate macro #
+# ------------------- #
 
 
-class CategoryGate(FieldCost):
+class GateCost(FieldCost):
     """
     Returns a matrix where each tracklet/detection pair that have equal
-    categories are set to `True` and  that have different categories are set to
+    field values are set to `True` and  that have different field values are set to
     `False`.
     """
 
-    def __init__(self, field="categories"):
-        super().__init__(field=field)
-
+    @TX.override
     def compute(self, cs_cats: torch.Tensor, ds_cats: torch.Tensor) -> torch.Tensor:
         gate_matrix = ds_cats[None, :] - cs_cats[:, None]
 
-        return gate_matrix == 0
+        return torch.where(gate_matrix == 0, 0.0, torch.inf)
 
+    def wrap(self, cost: Cost) -> Reduce:
+        """
+        Wraps another cost function with a gated cost function, using a sum
+        reduction to merge the two costs.
 
-DEFAULT_EPS: T.Final = 1e-8
+        Parameters
+        ----------
+        cost: Cost
+            The cost function to wrap.
+
+        Returns
+        -------
+        Reduction
+            The wrapped cost function.
+        """
+        return Reduce([cost, self], Reduction.SUM)
+
+
+DEFAULT_EPS: T.Final = torch.finfo(torch.float32).eps
+
+# ------------- #
+# Overlap costs #
+# ------------- #
 
 
 class MaskIoU(FieldCost):
     """
     Computes IoU cost matrix between two sets of bitmasks.
     """
 
     eps: torch.jit.Final[float]
 
-    def __init__(self, eps: float = DEFAULT_EPS, **kwargs):
-        super().__init__(**kwargs)
+    def __init__(self, *args, eps: float = DEFAULT_EPS, **kwargs):
+        super().__init__(*args, **kwargs)
         self.eps = eps
 
+    @TX.override
     def compute(self, cs: torch.Tensor, ds: torch.Tensor) -> torch.Tensor:
         return _naive_mask_iou(cs, ds, self.eps)
 
 
 class BoxIoU(MaskIoU):
+    @TX.override
     def compute(self, cs: torch.Tensor, ds: torch.Tensor) -> torch.Tensor:
         cs_field = _pad_degenerate_boxes(cs)
         ds_field = _pad_degenerate_boxes(ds)
 
-        return 1.0 - _complete_box_iou(cs_field, ds_field, self.eps)
+        iou = _complete_box_iou(cs_field, ds_field, self.eps)
+
+        return 1.0 - iou
 
 
 def _naive_mask_iou(cs: torch.Tensor, ds: torch.Tensor, eps: float) -> torch.Tensor:
     cs_m = cs.reshape(len(cs), -1).int()
     ds_m = ds.reshape(len(ds), -1).int()
 
     isec = torch.mm(cs_m, ds_m.T)
@@ -145,15 +205,17 @@
     boxes = boxes.clone()
     boxes[:, 2] += 1
     boxes[:, 3] += 1
 
     return boxes
 
 
-def _box_diou_iou(boxes1: torch.Tensor, boxes2: torch.Tensor, eps: float) -> T.Tuple[torch.Tensor, torch.Tensor]:
+def _box_diou_iou(
+    boxes1: torch.Tensor, boxes2: torch.Tensor, eps: float
+) -> T.Tuple[torch.Tensor, torch.Tensor]:
     """
     IoU with penalized center-distance
     """
 
     iou = box_iou(boxes1, boxes2)
     lti = torch.min(boxes1[:, None, :2], boxes2[:, :2])
     rbi = torch.max(boxes1[:, None, 2:], boxes2[:, 2:])
@@ -169,37 +231,47 @@
     # The distance between boxes' centers squared.
     centers_distance_squared = (((x_p[:, None] - x_g[None, :])).float() ** 2) + (
         ((y_p[:, None] - y_g[None, :])).float() ** 2
     )
 
     # The distance IoU is the IoU penalized by a normalized
     # distance between boxes' centers squared.
-    return iou - ((centers_distance_squared) / diagonal_distance_squared.clamp(eps)), iou
+    return (
+        iou - ((centers_distance_squared) / diagonal_distance_squared.clamp(eps)),
+        iou,
+    )
 
 
 def _complete_box_iou(boxes1: torch.Tensor, boxes2: torch.Tensor, eps) -> torch.Tensor:
     boxes1 = boxes1.float()
     boxes2 = boxes2.float()
 
     diou, iou = _box_diou_iou(boxes1, boxes2, eps)
 
     w_pred = boxes1[:, None, 2] - boxes1[:, None, 0]
     h_pred = boxes1[:, None, 3] - boxes1[:, None, 1]
 
     w_gt = boxes2[:, 2] - boxes2[:, 0]
     h_gt = boxes2[:, 3] - boxes2[:, 1]
 
-    v = (4 / (torch.pi**2)) * torch.pow(torch.atan(w_pred / h_pred) - torch.atan(w_gt / h_gt), 2)
+    v = (4 / (torch.pi**2)) * torch.pow(
+        torch.atan(w_pred / h_pred) - torch.atan(w_gt / h_gt), 2
+    )
 
     with torch.no_grad():
         alpha = v / (1 - iou + v).clamp(eps)
 
     return diou - alpha * v
 
 
+# ------------------- #
+# Combinational costs #
+# ------------------- #
+
+
 class Weighted(Cost):
     """
     A weighted cost module.
     """
 
     def __init__(self, cost: Cost, weight: float):
         super().__init__(required_fields=cost.required_fields)
@@ -207,168 +279,153 @@
         self.cost = cost
         self.weight = weight
 
     def forward(self, cs: TensorDictBase, ds: TensorDictBase) -> torch.Tensor:
         return self.weight * self.cost(cs, ds)
 
 
-class Reduction(E.Enum):
+class Reduction(E.StrEnum):
     """
     Reduction method for :class:`.Reduce` cost module.
     """
 
-    SUM = "sum"
-    MEAN = "mean"
-    MIN = "min"
-    MAX = "max"
-    PRODUCT = "product"
+    SUM = E.auto()
+    MEAN = E.auto()
+    MIN = E.auto()
+    MAX = E.auto()
+    PRODUCT = E.auto()
 
 
 class Reduce(Cost):
     """
     A cost reduction module.
     """
 
-    weights: torch.Tensor
-    method: torch.jit.Final[Reduction]
+    weights: T.Final[T.List[float]]
+    method: T.Final[method]
 
     def __init__(
         self,
         costs: T.Sequence[Cost],
-        method: Reduction,
+        method: Reduction | str,
         weights: T.Optional[T.Sequence[float]] = None,
     ):
-        super().__init__(required_fields=itertools.chain(*(c.required_fields for c in costs)))
-
-        if isinstance(method, str):
-            method = Reduction(method)
-
-        self.method = method
+        super().__init__(
+            required_fields=itertools.chain(*(c.required_fields for c in costs))
+        )
+        self.method = Reduction(method)
         self.costs = nn.ModuleList(costs)
         if weights is None:
             weights = [1.0] * len(costs)
+        self.weights = list(weights)
 
-        self.register_buffer("weights", torch.tensor(weights, dtype=torch.float32).unsqueeze_(-1).unsqueeze_(-1))
-
+    @TX.override
     def forward(self, cs: TensorDictBase, ds: TensorDictBase) -> torch.Tensor:
-        costs = torch.stack([cost(cs, ds) for cost in self.costs])
-        costs = costs * self.weights
-        costs = _reduce_stack(costs, self.method)
+        res = torch.stack(
+            [fn(cs, ds) * wt for fn, wt in zip(self.costs, self.weights, strict=True)]
+        )
 
-        return costs
+        match self.method:
+            case Reduction.SUM:
+                return res.sum(dim=0)
+            case Reduction.MEAN:
+                return res.mean(dim=0)
+            case Reduction.MIN:
+                return res.min(dim=0).values
+            case Reduction.MAX:
+                return res.max(dim=0).values
+            case Reduction.PRODUCT:
+                return res.prod(dim=0)
+            case _:
+                pass
+        msg = f"Reduction method '{method}' not implemented!"
+        raise NotImplementedError(msg)
 
 
-@torch.jit.script_if_tracing
-def _reduce_stack(costs: torch.Tensor, method: Reduction) -> torch.Tensor:
-    if method == Reduction.SUM:
-        return costs.sum(dim=0)
-    if method == Reduction.MEAN:
-        return costs.mean(dim=0)
-    if method == Reduction.MIN:
-        return costs.min(dim=0).values
-    if method == Reduction.MAX:
-        return costs.max(dim=0).values
-    raise NotImplementedError(f"Reduction method '{method}' not implemented!")
+# -------------------------- #
+# Various distance functions #
+# -------------------------- #
 
 
-class Distance(Cost):
+class CDist(FieldCost):
     """
-    Cost function that wraps a distance module.
+    Computes a distance between two fields using ``torch.cdist``.
     """
 
-    select: torch.jit.Final[T.List[int]]
-    p: torch.jit.Final[float]
-    field: torch.jit.Final[str]
+    p: T.Final[float]
 
-    def __init__(
-        self,
-        field: str,
-        select: T.Optional[T.List[int]] = None,
-        p_norm: float = 2.0,
-    ):
-        """
-        Parameters
-        ----------
-        critereon
-            Module that computes distance between two fields
-        field_name
-            Name if the field to read tensors from that are passed to the
-            ``torch.cdist`` function.
-        select
-            List of indices to select from the field.
-        p_norm
-            Value of p-norm.
-        """
-        super().__init__(required_fields=(field,))
-
-        self.field = field
-
-        if select is None:
-            select = []
-
-        self.select = select  # type: ignore
+    def __init__(self, *args, p_norm: float = 2.0, **kwargs):
+        super().__init__(*args, **kwargs)
         self.p = p_norm
 
-    def get_field(self, cs: TensorDictBase, ds: TensorDictBase) -> T.Tuple[torch.Tensor, torch.Tensor]:
-        ts_field = cs.get(self.field)
-        ds_field = ds.get(self.field)
-
-        if len(self.select) > 0:
-            assert ts_field.shape[1] >= max(self.select)
-            assert ds_field.shape[1] >= max(self.select)
-
-            ts_field = ts_field[:, self.select]
-            ds_field = ds_field[:, self.select]
-
-        return ts_field, ds_field
-
-    def forward(self, cs: TensorDictBase, ds: TensorDictBase):
-        ts_field, ds_field = self.get_field(cs, ds)
-        return torch.cdist(ts_field, ds_field, self.p, "donot_use_mm_for_euclid_dist")
+    @TX.override
+    def compute(self, cs: torch.Tensor, ds: torch.Tensor) -> torch.Tensor:
+        return torch.cdist(cs, ds, self.p, "donot_use_mm_for_euclid_dist")
 
 
-class Cosine(Distance):
+class Cosine(FieldCost):
     r"""
     Computes the distance between two fields based on a similarity measure with
     range $[0,1]$ by computing $1 - \mathrm{CosineSimilarity}(x,y)$.
     """
 
     def __init__(self, *args, eps: float = DEFAULT_EPS, **kwargs):
         super().__init__(*args, **kwargs)
         self.eps = eps
 
-    def compute(self, cs: TensorDictBase, ds: TensorDictBase):
+    @TX.override
+    def forward(self, cs: TensorDictBase, ds: TensorDictBase):
         ts_field, ds_field = self.get_field(cs, ds)
-        return 1.0 - _cosine_similarity(ts_field, ds_field, self.eps)
+        return cosine_distance(ts_field, ds_field, self.eps)
+
 
+def cosine_distance(a: torch.Tensor, b: torch.Tensor, eps) -> torch.Tensor:
+    a_norm = _stable_norm(a, eps)
+    b_norm = _stable_norm(b, eps)
 
-class Softmax(Distance):
+    return 1.0 - a_norm @ b_norm.mT
+
+
+class Softmax(FieldCost):
     r"""
     Computes the distance between two fields based on a similarity measure with
     range $[0,1]$ by computing $1 - \mathrm{ReciprocalSoftmax}(x,y)$.
     """
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
-    def compute(self, cs: TensorDictBase, ds: TensorDictBase):
+    @TX.override
+    def forward(self, cs: TensorDictBase, ds: TensorDictBase):
         ts_field, ds_field = self.get_field(cs, ds)
-        return 1.0 - _softmax_similarity(ts_field, ds_field)
+        return softmax_distance(ts_field, ds_field)
 
 
-def _cosine_similarity(a: torch.Tensor, b: torch.Tensor, eps) -> torch.Tensor:
-    a_norm = _stable_norm(a, eps)
-    b_norm = _stable_norm(b, eps)
+def softmax_distance(a: torch.Tensor, b: torch.Tensor) -> torch.Tensor:
+    mul = torch.mm(a, b.T)
+    a2b = mul.softmax(dim=0)
+    b2a = mul.softmax(dim=1)
+    return 1.0 - (a2b + b2a) / 2.0
 
-    return a_norm @ b_norm.mT
+
+class RadialBasis(FieldCost):
+    r"""
+    Computes the radial basis function (RBF) between two fields.
+    """
+
+    @TX.override
+    def compute(self, x: torch.Tensor, y: torch.Tensor) -> torch.Tensor:
+        return radial_basis_distance(x, y)
+
+
+def radial_basis_distance(a: torch.Tensor, b: torch.Tensor) -> torch.Tensor:
+    return torch.exp(-torch.cdist(a, b, p=2))
+
+
+# --------- #
+# Utilities #
+# --------- #
 
 
 def _stable_norm(t: torch.Tensor, eps):
     norm = torch.linalg.vector_norm(t, dim=-1, keepdim=True)
     return t / norm.clamp_min(eps)
-
-
-def _softmax_similarity(a: torch.Tensor, b: torch.Tensor) -> torch.Tensor:
-    mul = torch.mm(a, b.T)
-    a2b = mul.softmax(dim=0)
-    b2a = mul.softmax(dim=1)
-    return (a2b + b2a) / 2.0
```

### Comparing `unitrack-4.7.0/sources/unitrack/stages/association.py` & `unitrack-4.7.2/sources/unitrack/stages/association.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,20 @@
-from typing import Tuple
+from __future__ import annotations
 
+import typing as T
+
+import typing_extensions as TX
 from tensordict import TensorDictBase
 
-from ..assignment import Assignment
-from ..constants import KEY_FRAME, KEY_ID, KEY_INDEX
-from ..costs import Cost
+if T.TYPE_CHECKING:
+    from unitrack.assignment import Assignment
+    from unitrack.costs import Cost
+
+from unitrack.debug import check_debug_enabled
+
 from .base_stage import Stage
 
 __all__ = ["Association"]
 
 
 class Association(Stage):
     """
@@ -28,47 +34,34 @@
 
         self._extend_required_fields(self.cost)
 
     def _extend_required_fields(self, *costs: Cost) -> None:
         for cost in costs:
             self.required_fields += cost.required_fields
 
+    @TX.override
     def forward(
         self, ctx: TensorDictBase, cs: TensorDictBase, ds: TensorDictBase
-    ) -> Tuple[TensorDictBase, TensorDictBase]:
+    ) -> T.Tuple[TensorDictBase, TensorDictBase]:
+        if check_debug_enabled():
+            print(
+                f"Associating {cs.batch_size[0]} candidates / "
+                f"{ds.batch_size[0]} detections"
+            )
+
         if len(cs) == 0 or len(ds) == 0:
             return cs, ds
 
         cost_matrix = self.cost(cs, ds)
 
         matches, cs_fail_idx, ds_fail_idx = self.assignment(cost_matrix)
 
         if len(matches) > 0:
-            cs_match = cs.get_sub_tensordict(matches[:, 0])
-            ds_match = ds.get_sub_tensordict(matches[:, 1])
+            cs_match = cs._get_sub_tensordict(matches[:, 0])
+            ds_match = ds._get_sub_tensordict(matches[:, 1])
 
             self.match(cs_match, ds_match)
 
-        cs_fail = cs.get_sub_tensordict(cs_fail_idx)
-        ds_fail = ds.get_sub_tensordict(ds_fail_idx)
+        cs_fail = cs._get_sub_tensordict(cs_fail_idx)
+        ds_fail = ds._get_sub_tensordict(ds_fail_idx)
 
         return cs_fail, ds_fail
-
-    def match(self, cs: TensorDictBase, ds: TensorDictBase) -> None:
-        """
-        Match candidates to detections. Propagates data and IDs from detections to candidates.
-
-        Parameters
-        ----------
-        cs
-            Candidates
-        ds
-            Detections
-        """
-        for key, value in ds.items():
-            if key.startswith("_"):
-                continue
-            if key not in cs.keys():
-                continue
-            cs.set_(key, value)
-
-        cs.set_(KEY_INDEX, ds.get(KEY_INDEX))
```

### Comparing `unitrack-4.7.0/sources/unitrack/stages/lost.py` & `unitrack-4.7.2/sources/unitrack/stages/lost.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,20 @@
-from typing import Tuple
+r"""
+Implements the `Lost` stage, which filters out candidates that have been lost for more
+than a configurable maximum amount of time.
+"""
+
+from __future__ import annotations
+
+import typing as T
 
 import torch
 from tensordict import TensorDictBase
 
-from ..constants import KEY_DELTA, KEY_FRAME
+from ..consts import KEY_DELTA, KEY_FRAME
 from .base_stage import Stage
 
 __all__ = ["Lost"]
 
 
 class Lost(Stage):
     """
@@ -18,15 +25,15 @@
     The time lost is computed via $$ T_l = t - T_c - dt $$ where $t$ is the
     current time (i.e. frame) and $T_c$ are the candidate time states.
     The value is corrected with time-step $dt$ to account for candidates not yet
     being updated to the current time, as the state update is performed
     *after* all stages have been ran.
     """
 
-    max_lost: torch.jit.Final[int]
+    max_lost: T.Final[int]
 
     def __init__(self, max_lost: int):
         """
         Parameters
         ----------
         max_lost
             Maximum amount of time a candidate may remain lost.
```

### Comparing `unitrack-4.7.0/sources/unitrack/states/base_state.py` & `unitrack-4.7.2/sources/unitrack/states/base_state.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from abc import abstractmethod
 from typing import Iterable, TypeAlias, cast
 
 import torch
 from torch import Tensor
 
 __all__ = ["State"]
```

### Comparing `unitrack-4.7.0/sources/unitrack/tracker.py` & `unitrack-4.7.2/sources/unitrack/_tracker.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,76 +1,104 @@
-from typing import Dict, List, Mapping, Sequence, Tuple, cast
+from __future__ import annotations
+
+import typing as T
 
 import torch
 import torch.nn as nn
 from tensordict import TensorDict, TensorDictBase
-from tensordict.nn import (
-    TensorDictModule,
-    TensorDictModuleBase,
-    TensorDictSequential,
-)
+from tensordict.nn import TensorDictModule, TensorDictModuleBase, TensorDictSequential
 
-from .constants import KEY_ACTIVE, KEY_FRAME, KEY_ID, KEY_INDEX, KEY_START
+from .consts import KEY_ACTIVE, KEY_FRAME, KEY_ID, KEY_INDEX, KEY_START
+from .debug import check_debug_enabled
 from .stages import Stage
 
 
 class MultiStageTracker(nn.Module):
     """
     Multi-stage tracker that applies a cascade of stages to a set of detections.
     """
 
-    def __init__(self, fields: Sequence[TensorDictModule], stages: Sequence[Stage]):
+    def __init__(self, fields: T.Sequence[TensorDictModule], stages: T.Sequence[Stage]):
         super().__init__()
 
         assert len(stages) > 0
 
         self.fields = nn.ModuleList(fields)
-        self.stages = cast(List[Stage], nn.ModuleList(stages))
+        self.stages = nn.ModuleList(stages)
 
     def forward(
         self,
         ctx: TensorDictBase,
         obs: TensorDictBase,
         inp: TensorDictBase,
-    ) -> tuple[TensorDictBase, TensorDictBase]:
+        num: int,
+    ) -> T.Tuple[TensorDictBase, TensorDictBase]:
         """
         Perform tracking, returns a tuple of updated observations and the field-values of new tracklets.
 
 
+        Parameters
+        ----------
+        ctx: TensorDictBase
+            The current state's context
+        obs: TensorDictBase
+            The current state's observations (i.e. when ``.observe()`` is called on
+            each field in memory)
+        inp: TensorDictBase
+            The state of the next frame, from which new detections are gathered at
+            every field.
+        num: int
+            The amount of detections made. Fields must allocate within a TensorDict
+            that enforces ``batch_size=[num]``.
+
+
         Returns
         -------
         Tuple[TensorDict, TensorDict]
             Updated observations and field-values of new tracklets.
         """
 
-        # Fields target (newly detected objects)
+        if inp.device is None:
+            msg = (
+                "Inputs TensorDict device is None. Check that the tensors are on the "
+                "same device and that the container TensorDict instance has the device "
+                "property set."
+            )
+            raise ValueError(msg)
+
+        # Create a dict of new tracklet candidates by passing the input state to
+        # each field
+        new_index = torch.arange(num, device=inp.device, dtype=torch.int64)
         new = TensorDict(
-            {},
-            batch_size=[],
+            {KEY_INDEX: new_index},
+            batch_size=new_index.shape,
             device=inp.device,
+            _run_checks=False,
         )
 
+        obs = obs.to(device=inp.device)
+
         for field in self.fields:
             field(inp, tensordict_out=new)
 
-        # Infer the number of detections from the batch size of some element in the new detections
-        num_det = int(next(iter(new.values())).shape[0])
-        new.batch_size = torch.Size((num_det,))
-        if num_det == 0:
-            return obs, new
-
-        # Add the index of the detections to association
-        new[KEY_INDEX] = torch.arange(num_det, device=inp.device)
+        assert obs.device is not None
+        assert new.device is not None
 
         # Candidates for matching are all active observed tracklets
-        obs_active = obs.get(KEY_ACTIVE)
-        if obs_active.any():
-            obs_candidates = obs.get_sub_tensordict(obs_active)
-            for stage in self.stages:
-                obs_candidates, new = stage(ctx, obs_candidates, new)
-                if len(obs_candidates) == 0 or len(new) == 0:
-                    break
-
-            if len(obs_candidates) > 0 and obs_candidates.batch_size[0] > 0:
-                obs_candidates.fill_(KEY_ACTIVE, False)
+        active_mask = obs.get(KEY_ACTIVE)
+        obs_candidates = obs._get_sub_tensordict(active_mask)
+        for stage in self.stages:
+            if obs_candidates.batch_size[0] == 0 or new.batch_size[0] == 0:
+                break
+            obs_candidates, new = stage(ctx, obs_candidates, new)
+
+        obs_unmatched_mask = obs.get(KEY_INDEX) < 0
+
+        if check_debug_enabled():
+            print(
+                f"TRACKER COMPLETE: remaining {obs_unmatched_mask.int().sum().item()}/{len(obs)} unmatched observations"
+            )
+        obs[KEY_ACTIVE] = torch.where(obs_unmatched_mask, False, True)
+        # obs.set_at_(KEY_ACTIVE, False, obs_unmatched_mask)
+        # obs.set_at_(KEY_ACTIVE, True, ~obs_unmatched_mask)
 
         return obs, new
```

### Comparing `unitrack-4.7.0/sources/unitrack.egg-info/SOURCES.txt` & `unitrack-4.7.2/sources/unitrack.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 LICENSE
 README.md
 pyproject.toml
 sources/unitrack/__init__.py
-sources/unitrack/constants.py
+sources/unitrack/_memory.py
+sources/unitrack/_stateful.py
+sources/unitrack/_tracker.py
+sources/unitrack/consts.py
 sources/unitrack/costs.py
-sources/unitrack/memory.py
-sources/unitrack/tracker.py
+sources/unitrack/debug.py
+sources/unitrack/py.typed
 sources/unitrack.egg-info/PKG-INFO
 sources/unitrack.egg-info/SOURCES.txt
 sources/unitrack.egg-info/dependency_links.txt
 sources/unitrack.egg-info/requires.txt
 sources/unitrack.egg-info/top_level.txt
 sources/unitrack/assignment/__init__.py
-sources/unitrack/assignment/auction.py
-sources/unitrack/assignment/base_assignment.py
-sources/unitrack/assignment/greedy.py
-sources/unitrack/assignment/hungarian.py
-sources/unitrack/assignment/jonker.py
+sources/unitrack/assignment/_auction.py
+sources/unitrack/assignment/_base.py
+sources/unitrack/assignment/_greedy.py
+sources/unitrack/assignment/_hungarian.py
+sources/unitrack/assignment/_jonker.py
+sources/unitrack/assignment/_utils.py
 sources/unitrack/stages/__init__.py
 sources/unitrack/stages/association.py
 sources/unitrack/stages/base_stage.py
+sources/unitrack/stages/gate.py
 sources/unitrack/stages/lost.py
 sources/unitrack/states/__init__.py
 sources/unitrack/states/base_state.py
 sources/unitrack/states/value.py
```

