# Comparing `tmp/emcee-3.1.5.tar.gz` & `tmp/emcee-3.1.5rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emcee-3.1.5.tar", last modified: Tue Apr 16 14:19:18 2024, max compression
+gzip compressed data, was "emcee-3.1.5rc1.tar", last modified: Wed Apr 10 20:13:49 2024, max compression
```

## Comparing `emcee-3.1.5.tar` & `emcee-3.1.5rc1.tar`

### file list

```diff
@@ -1,133 +1,133 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:19:18.932112 emcee-3.1.5/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-16 14:19:11.000000 emcee-3.1.5/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:19:18.908111 emcee-3.1.5/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-16 14:19:11.000000 emcee-3.1.5/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-16 14:19:11.000000 emcee-3.1.5/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:19:18.908111 emcee-3.1.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3573 2024-04-16 14:19:11.000000 emcee-3.1.5/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-16 14:19:11.000000 emcee-3.1.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-16 14:19:11.000000 emcee-3.1.5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-16 14:19:11.000000 emcee-3.1.5/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-16 14:19:11.000000 emcee-3.1.5/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3221 2024-04-16 14:19:11.000000 emcee-3.1.5/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-04-16 14:19:11.000000 emcee-3.1.5/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     3860 2024-04-16 14:19:11.000000 emcee-3.1.5/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-16 14:19:11.000000 emcee-3.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-16 14:19:11.000000 emcee-3.1.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3012 2024-04-16 14:19:18.932112 emcee-3.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-04-16 14:19:11.000000 emcee-3.1.5/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-16 14:19:11.000000 emcee-3.1.5/VISION.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:19:18.908111 emcee-3.1.5/binder/
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-16 14:19:11.000000 emcee-3.1.5/binder/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:19:18.912111 emcee-3.1.5/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-16 14:19:11.000000 emcee-3.1.5/docs/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     5591 2024-04-16 14:19:11.000000 emcee-3.1.5/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:19:18.912111 emcee-3.1.5/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-04-16 14:19:11.000000 emcee-3.1.5/docs/_static/favicon.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:19:18.912111 emcee-3.1.5/docs/_static/line/
--rw-r--r--   0 runner    (1001) docker     (127)    19384 2024-04-16 14:19:11.000000 emcee-3.1.5/docs/_static/line/line-data.png
--rw-r--r--   0 runner    (1001) docker     (127)    26456 2024-04-16 14:19:11.000000 emcee-3.1.5/docs/_static/line/line-least-squares.png
--rw-r--r--   0 runner    (1001) docker     (127)    34934 2024-04-16 14:19:11.000000 emcee-3.1.5/docs/_static/line/line-max-likelihood.png
--rw-r--r--   0 runner    (1001) docker     (127)    67232 2024-04-16 14:19:11.000000 emcee-3.1.5/docs/_static/line/line-mcmc.png
--rw-r--r--   0 runner    (1001) docker     (127)   404073 2024-04-16 14:19:11.000000 emcee-3.1.5/docs/_static/line/line-time.png
--rw-r--r--   0 runner    (1001) docker     (127)   126982 2024-04-16 14:19:11.000000 emcee-3.1.5/docs/_static/line/line-triangle.png
--rw-r--r--   0 runner    (1001) docker     (127)    13320 2024-04-16 14:19:11.000000 emcee-3.1.5/docs/_static/logo-sidebar.png
--rw-r--r--   0 runner    (1001) docker     (127)   150797 2024-04-16 14:19:11.000000 emcee-3.1.5/docs/_static/logo.pxm
--rw-r--r--   0 runner    (1001) docker     (127)    13411 2024-04-16 14:19:11.000000 emcee-3.1.5/docs/_static/logo2.png
--rw-r--r--   0 runner    (1001) docker     (127)   240605 2024-04-16 14:19:11.000000 emcee-3.1.5/docs/_static/logo2.pxm
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-16 14:19:11.000000 emcee-3.1.5/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-16 14:19:11.000000 emcee-3.1.5/docs/fix_internal_links.py
--rw-r--r--   0 runner    (1001) docker     (127)     3699 2024-04-16 14:19:11.000000 emcee-3.1.5/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-16 14:19:11.000000 emcee-3.1.5/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:19:18.916111 emcee-3.1.5/docs/tutorials/
--rw-r--r--   0 runner    (1001) docker     (127)   515948 2024-04-16 14:19:11.000000 emcee-3.1.5/docs/tutorials/autocorr.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   865248 2024-04-16 14:19:11.000000 emcee-3.1.5/docs/tutorials/line.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)  1100525 2024-04-16 14:19:11.000000 emcee-3.1.5/docs/tutorials/monitor.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   245392 2024-04-16 14:19:11.000000 emcee-3.1.5/docs/tutorials/moves.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    14605 2024-04-16 14:19:11.000000 emcee-3.1.5/docs/tutorials/parallel.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    18991 2024-04-16 14:19:11.000000 emcee-3.1.5/docs/tutorials/quickstart.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-04-16 14:19:11.000000 emcee-3.1.5/docs/tutorials/tutorial_rst.tpl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:19:18.920111 emcee-3.1.5/docs/user/
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-16 14:19:11.000000 emcee-3.1.5/docs/user/autocorr.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-16 14:19:11.000000 emcee-3.1.5/docs/user/backends.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5237 2024-04-16 14:19:11.000000 emcee-3.1.5/docs/user/blobs.rst
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-16 14:19:11.000000 emcee-3.1.5/docs/user/faq.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-04-16 14:19:11.000000 emcee-3.1.5/docs/user/install.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-04-16 14:19:11.000000 emcee-3.1.5/docs/user/moves.rst
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-16 14:19:11.000000 emcee-3.1.5/docs/user/sampler.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-04-16 14:19:11.000000 emcee-3.1.5/docs/user/upgrade.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:19:18.920111 emcee-3.1.5/document/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-16 14:19:11.000000 emcee-3.1.5/document/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-16 14:19:11.000000 emcee-3.1.5/document/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)    66184 2024-04-16 14:19:11.000000 emcee-3.1.5/document/aastex.cls
--rw-r--r--   0 runner    (1001) docker     (127)    41540 2024-04-16 14:19:11.000000 emcee-3.1.5/document/ms.tex
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:19:18.920111 emcee-3.1.5/document/plots/
--rw-r--r--   0 runner    (1001) docker     (127)     2131 2024-04-16 14:19:11.000000 emcee-3.1.5/document/plots/oned.py
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-16 14:19:11.000000 emcee-3.1.5/document/plots/plot_acor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:19:18.920111 emcee-3.1.5/joss/
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-16 14:19:11.000000 emcee-3.1.5/joss/.gitignore
--rwxr-xr-x   0 runner    (1001) docker     (127)     1234 2024-04-16 14:19:11.000000 emcee-3.1.5/joss/make_latex.sh
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-16 14:19:11.000000 emcee-3.1.5/joss/metadata.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-04-16 14:19:11.000000 emcee-3.1.5/joss/paper.bib
--rw-r--r--   0 runner    (1001) docker     (127)     5349 2024-04-16 14:19:11.000000 emcee-3.1.5/joss/paper.md
--rw-r--r--   0 runner    (1001) docker     (127)    16848 2024-04-16 14:19:11.000000 emcee-3.1.5/joss/paper.tex
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-16 14:19:11.000000 emcee-3.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 14:19:18.932112 emcee-3.1.5/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     2376 2024-04-16 14:19:11.000000 emcee-3.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:19:18.904111 emcee-3.1.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:19:18.924111 emcee-3.1.5/src/emcee/
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-04-16 14:19:11.000000 emcee-3.1.5/src/emcee/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4422 2024-04-16 14:19:11.000000 emcee-3.1.5/src/emcee/autocorr.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:19:18.924111 emcee-3.1.5/src/emcee/backends/
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-16 14:19:11.000000 emcee-3.1.5/src/emcee/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8376 2024-04-16 14:19:11.000000 emcee-3.1.5/src/emcee/backends/backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     9191 2024-04-16 14:19:11.000000 emcee-3.1.5/src/emcee/backends/hdf.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-16 14:19:18.000000 emcee-3.1.5/src/emcee/emcee_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    25923 2024-04-16 14:19:11.000000 emcee-3.1.5/src/emcee/ensemble.py
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-16 14:19:11.000000 emcee-3.1.5/src/emcee/interruptible_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-16 14:19:11.000000 emcee-3.1.5/src/emcee/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:19:18.928111 emcee-3.1.5/src/emcee/moves/
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-16 14:19:11.000000 emcee-3.1.5/src/emcee/moves/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-04-16 14:19:11.000000 emcee-3.1.5/src/emcee/moves/de.py
--rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-04-16 14:19:11.000000 emcee-3.1.5/src/emcee/moves/de_snooker.py
--rw-r--r--   0 runner    (1001) docker     (127)     4006 2024-04-16 14:19:11.000000 emcee-3.1.5/src/emcee/moves/gaussian.py
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-16 14:19:11.000000 emcee-3.1.5/src/emcee/moves/kde.py
--rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-04-16 14:19:11.000000 emcee-3.1.5/src/emcee/moves/mh.py
--rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-04-16 14:19:11.000000 emcee-3.1.5/src/emcee/moves/move.py
--rw-r--r--   0 runner    (1001) docker     (127)     4008 2024-04-16 14:19:11.000000 emcee-3.1.5/src/emcee/moves/red_blue.py
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-16 14:19:11.000000 emcee-3.1.5/src/emcee/moves/stretch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-16 14:19:11.000000 emcee-3.1.5/src/emcee/moves/walk.py
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-16 14:19:11.000000 emcee-3.1.5/src/emcee/mpi_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-04-16 14:19:11.000000 emcee-3.1.5/src/emcee/pbar.py
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-16 14:19:11.000000 emcee-3.1.5/src/emcee/ptsampler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-04-16 14:19:11.000000 emcee-3.1.5/src/emcee/state.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:19:18.928111 emcee-3.1.5/src/emcee/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 14:19:11.000000 emcee-3.1.5/src/emcee/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:19:18.928111 emcee-3.1.5/src/emcee/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 14:19:11.000000 emcee-3.1.5/src/emcee/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-16 14:19:11.000000 emcee-3.1.5/src/emcee/tests/integration/test_de.py
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-16 14:19:11.000000 emcee-3.1.5/src/emcee/tests/integration/test_de_snooker.py
--rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-04-16 14:19:11.000000 emcee-3.1.5/src/emcee/tests/integration/test_gaussian.py
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-16 14:19:11.000000 emcee-3.1.5/src/emcee/tests/integration/test_kde.py
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-16 14:19:11.000000 emcee-3.1.5/src/emcee/tests/integration/test_longdouble.py
--rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-04-16 14:19:11.000000 emcee-3.1.5/src/emcee/tests/integration/test_proposal.py
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-04-16 14:19:11.000000 emcee-3.1.5/src/emcee/tests/integration/test_stretch.py
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-16 14:19:11.000000 emcee-3.1.5/src/emcee/tests/integration/test_walk.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:19:18.928111 emcee-3.1.5/src/emcee/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 14:19:11.000000 emcee-3.1.5/src/emcee/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-04-16 14:19:11.000000 emcee-3.1.5/src/emcee/tests/unit/test_autocorr.py
--rw-r--r--   0 runner    (1001) docker     (127)     8487 2024-04-16 14:19:11.000000 emcee-3.1.5/src/emcee/tests/unit/test_backends.py
--rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-04-16 14:19:11.000000 emcee-3.1.5/src/emcee/tests/unit/test_blobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     6918 2024-04-16 14:19:11.000000 emcee-3.1.5/src/emcee/tests/unit/test_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (127)    11018 2024-04-16 14:19:11.000000 emcee-3.1.5/src/emcee/tests/unit/test_sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-04-16 14:19:11.000000 emcee-3.1.5/src/emcee/tests/unit/test_state.py
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-16 14:19:11.000000 emcee-3.1.5/src/emcee/tests/unit/test_stretch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-04-16 14:19:11.000000 emcee-3.1.5/src/emcee/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:19:18.928111 emcee-3.1.5/src/emcee.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3012 2024-04-16 14:19:18.000000 emcee-3.1.5/src/emcee.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-04-16 14:19:18.000000 emcee-3.1.5/src/emcee.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 14:19:18.000000 emcee-3.1.5/src/emcee.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 14:19:18.000000 emcee-3.1.5/src/emcee.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-16 14:19:18.000000 emcee-3.1.5/src/emcee.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-16 14:19:18.000000 emcee-3.1.5/src/emcee.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-16 14:19:11.000000 emcee-3.1.5/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:13:49.306466 emcee-3.1.5rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:13:49.282467 emcee-3.1.5rc1/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:13:49.282467 emcee-3.1.5rc1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3573 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3221 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3860 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-04-10 20:13:49.306466 emcee-3.1.5rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/VISION.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:13:49.282467 emcee-3.1.5rc1/binder/
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/binder/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:13:49.286466 emcee-3.1.5rc1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/docs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     5591 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:13:49.286466 emcee-3.1.5rc1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/docs/_static/favicon.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:13:49.286466 emcee-3.1.5rc1/docs/_static/line/
+-rw-r--r--   0 runner    (1001) docker     (127)    19384 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/docs/_static/line/line-data.png
+-rw-r--r--   0 runner    (1001) docker     (127)    26456 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/docs/_static/line/line-least-squares.png
+-rw-r--r--   0 runner    (1001) docker     (127)    34934 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/docs/_static/line/line-max-likelihood.png
+-rw-r--r--   0 runner    (1001) docker     (127)    67232 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/docs/_static/line/line-mcmc.png
+-rw-r--r--   0 runner    (1001) docker     (127)   404073 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/docs/_static/line/line-time.png
+-rw-r--r--   0 runner    (1001) docker     (127)   126982 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/docs/_static/line/line-triangle.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13320 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/docs/_static/logo-sidebar.png
+-rw-r--r--   0 runner    (1001) docker     (127)   150797 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/docs/_static/logo.pxm
+-rw-r--r--   0 runner    (1001) docker     (127)    13411 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/docs/_static/logo2.png
+-rw-r--r--   0 runner    (1001) docker     (127)   240605 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/docs/_static/logo2.pxm
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/docs/fix_internal_links.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3699 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:13:49.290466 emcee-3.1.5rc1/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (127)   515948 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/docs/tutorials/autocorr.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   865248 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/docs/tutorials/line.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)  1100525 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/docs/tutorials/monitor.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   245392 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/docs/tutorials/moves.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    14605 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/docs/tutorials/parallel.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    18991 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/docs/tutorials/quickstart.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/docs/tutorials/tutorial_rst.tpl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:13:49.294466 emcee-3.1.5rc1/docs/user/
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/docs/user/autocorr.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/docs/user/backends.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5237 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/docs/user/blobs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/docs/user/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/docs/user/install.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/docs/user/moves.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/docs/user/sampler.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/docs/user/upgrade.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:13:49.294466 emcee-3.1.5rc1/document/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/document/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/document/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    66184 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/document/aastex.cls
+-rw-r--r--   0 runner    (1001) docker     (127)    41540 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/document/ms.tex
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:13:49.294466 emcee-3.1.5rc1/document/plots/
+-rw-r--r--   0 runner    (1001) docker     (127)     2131 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/document/plots/oned.py
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/document/plots/plot_acor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:13:49.294466 emcee-3.1.5rc1/joss/
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/joss/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1234 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/joss/make_latex.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/joss/metadata.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/joss/paper.bib
+-rw-r--r--   0 runner    (1001) docker     (127)     5349 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/joss/paper.md
+-rw-r--r--   0 runner    (1001) docker     (127)    16848 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/joss/paper.tex
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 20:13:49.306466 emcee-3.1.5rc1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2376 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:13:49.278466 emcee-3.1.5rc1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:13:49.298467 emcee-3.1.5rc1/src/emcee/
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/src/emcee/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4422 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/src/emcee/autocorr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:13:49.298467 emcee-3.1.5rc1/src/emcee/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/src/emcee/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8376 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/src/emcee/backends/backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9191 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/src/emcee/backends/hdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-10 20:13:49.000000 emcee-3.1.5rc1/src/emcee/emcee_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25923 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/src/emcee/ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/src/emcee/interruptible_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/src/emcee/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:13:49.302466 emcee-3.1.5rc1/src/emcee/moves/
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/src/emcee/moves/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/src/emcee/moves/de.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/src/emcee/moves/de_snooker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4006 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/src/emcee/moves/gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/src/emcee/moves/kde.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/src/emcee/moves/mh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/src/emcee/moves/move.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4008 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/src/emcee/moves/red_blue.py
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/src/emcee/moves/stretch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/src/emcee/moves/walk.py
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/src/emcee/mpi_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/src/emcee/pbar.py
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/src/emcee/ptsampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/src/emcee/state.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:13:49.302466 emcee-3.1.5rc1/src/emcee/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/src/emcee/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:13:49.302466 emcee-3.1.5rc1/src/emcee/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/src/emcee/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/src/emcee/tests/integration/test_de.py
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/src/emcee/tests/integration/test_de_snooker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/src/emcee/tests/integration/test_gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/src/emcee/tests/integration/test_kde.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/src/emcee/tests/integration/test_longdouble.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/src/emcee/tests/integration/test_proposal.py
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/src/emcee/tests/integration/test_stretch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/src/emcee/tests/integration/test_walk.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:13:49.302466 emcee-3.1.5rc1/src/emcee/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/src/emcee/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/src/emcee/tests/unit/test_autocorr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8487 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/src/emcee/tests/unit/test_backends.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/src/emcee/tests/unit/test_blobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6918 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/src/emcee/tests/unit/test_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11018 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/src/emcee/tests/unit/test_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/src/emcee/tests/unit/test_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/src/emcee/tests/unit/test_stretch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/src/emcee/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:13:49.302466 emcee-3.1.5rc1/src/emcee.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-04-10 20:13:49.000000 emcee-3.1.5rc1/src/emcee.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-04-10 20:13:49.000000 emcee-3.1.5rc1/src/emcee.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 20:13:49.000000 emcee-3.1.5rc1/src/emcee.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 20:13:49.000000 emcee-3.1.5rc1/src/emcee.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-10 20:13:49.000000 emcee-3.1.5rc1/src/emcee.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-10 20:13:49.000000 emcee-3.1.5rc1/src/emcee.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-10 20:13:42.000000 emcee-3.1.5rc1/tox.ini
```

### Comparing `emcee-3.1.5/.github/ISSUE_TEMPLATE.md` & `emcee-3.1.5rc1/.github/ISSUE_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5/.github/workflows/tests.yml` & `emcee-3.1.5rc1/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5/CODE_OF_CONDUCT.md` & `emcee-3.1.5rc1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5/CONTRIBUTING.md` & `emcee-3.1.5rc1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5/HISTORY.rst` & `emcee-3.1.5rc1/HISTORY.rst`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5/LICENSE` & `emcee-3.1.5rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5/PKG-INFO` & `emcee-3.1.5rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emcee
-Version: 3.1.5
+Version: 3.1.5rc1
 Summary: The Python ensemble sampling toolkit for MCMC
 Home-page: https://emcee.readthedocs.io
 Author: Daniel Foreman-Mackey
 Author-email: foreman.mackey@gmail.com
 Maintainer: Daniel Foreman-Mackey
 Maintainer-email: foreman.mackey@gmail.com
 License: MIT
```

### Comparing `emcee-3.1.5/README.rst` & `emcee-3.1.5rc1/README.rst`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5/docs/Makefile` & `emcee-3.1.5rc1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5/docs/_static/favicon.png` & `emcee-3.1.5rc1/docs/_static/favicon.png`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5/docs/_static/line/line-data.png` & `emcee-3.1.5rc1/docs/_static/line/line-data.png`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5/docs/_static/line/line-least-squares.png` & `emcee-3.1.5rc1/docs/_static/line/line-least-squares.png`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5/docs/_static/line/line-max-likelihood.png` & `emcee-3.1.5rc1/docs/_static/line/line-max-likelihood.png`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5/docs/_static/line/line-mcmc.png` & `emcee-3.1.5rc1/docs/_static/line/line-mcmc.png`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5/docs/_static/line/line-time.png` & `emcee-3.1.5rc1/docs/_static/line/line-time.png`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5/docs/_static/line/line-triangle.png` & `emcee-3.1.5rc1/docs/_static/line/line-triangle.png`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5/docs/_static/logo-sidebar.png` & `emcee-3.1.5rc1/docs/_static/logo-sidebar.png`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5/docs/_static/logo.pxm` & `emcee-3.1.5rc1/docs/_static/logo.pxm`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5/docs/_static/logo2.png` & `emcee-3.1.5rc1/docs/_static/logo2.png`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5/docs/_static/logo2.pxm` & `emcee-3.1.5rc1/docs/_static/logo2.pxm`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5/docs/conf.py` & `emcee-3.1.5rc1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5/docs/index.rst` & `emcee-3.1.5rc1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5/docs/tutorials/autocorr.ipynb` & `emcee-3.1.5rc1/docs/tutorials/autocorr.ipynb`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5/docs/tutorials/line.ipynb` & `emcee-3.1.5rc1/docs/tutorials/line.ipynb`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5/docs/tutorials/monitor.ipynb` & `emcee-3.1.5rc1/docs/tutorials/monitor.ipynb`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5/docs/tutorials/moves.ipynb` & `emcee-3.1.5rc1/docs/tutorials/moves.ipynb`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5/docs/tutorials/parallel.ipynb` & `emcee-3.1.5rc1/docs/tutorials/parallel.ipynb`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5/docs/tutorials/quickstart.ipynb` & `emcee-3.1.5rc1/docs/tutorials/quickstart.ipynb`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5/docs/tutorials/tutorial_rst.tpl` & `emcee-3.1.5rc1/docs/tutorials/tutorial_rst.tpl`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5/docs/user/backends.rst` & `emcee-3.1.5rc1/docs/user/backends.rst`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5/docs/user/blobs.rst` & `emcee-3.1.5rc1/docs/user/blobs.rst`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5/docs/user/faq.rst` & `emcee-3.1.5rc1/docs/user/faq.rst`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5/docs/user/install.rst` & `emcee-3.1.5rc1/docs/user/install.rst`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5/docs/user/moves.rst` & `emcee-3.1.5rc1/docs/user/moves.rst`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5/docs/user/upgrade.rst` & `emcee-3.1.5rc1/docs/user/upgrade.rst`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5/document/aastex.cls` & `emcee-3.1.5rc1/document/aastex.cls`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5/document/ms.tex` & `emcee-3.1.5rc1/document/ms.tex`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5/document/plots/oned.py` & `emcee-3.1.5rc1/document/plots/oned.py`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5/joss/make_latex.sh` & `emcee-3.1.5rc1/joss/make_latex.sh`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5/joss/metadata.yaml` & `emcee-3.1.5rc1/joss/metadata.yaml`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5/joss/paper.bib` & `emcee-3.1.5rc1/joss/paper.bib`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5/joss/paper.md` & `emcee-3.1.5rc1/joss/paper.md`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5/joss/paper.tex` & `emcee-3.1.5rc1/joss/paper.tex`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5/pyproject.toml` & `emcee-3.1.5rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5/setup.py` & `emcee-3.1.5rc1/setup.py`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5/src/emcee/__init__.py` & `emcee-3.1.5rc1/src/emcee/__init__.py`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5/src/emcee/autocorr.py` & `emcee-3.1.5rc1/src/emcee/autocorr.py`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5/src/emcee/backends/backend.py` & `emcee-3.1.5rc1/src/emcee/backends/backend.py`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5/src/emcee/backends/hdf.py` & `emcee-3.1.5rc1/src/emcee/backends/hdf.py`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5/src/emcee/ensemble.py` & `emcee-3.1.5rc1/src/emcee/ensemble.py`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5/src/emcee/moves/de.py` & `emcee-3.1.5rc1/src/emcee/moves/de.py`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5/src/emcee/moves/de_snooker.py` & `emcee-3.1.5rc1/src/emcee/moves/de_snooker.py`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5/src/emcee/moves/gaussian.py` & `emcee-3.1.5rc1/src/emcee/moves/gaussian.py`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5/src/emcee/moves/kde.py` & `emcee-3.1.5rc1/src/emcee/moves/kde.py`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5/src/emcee/moves/mh.py` & `emcee-3.1.5rc1/src/emcee/moves/mh.py`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5/src/emcee/moves/move.py` & `emcee-3.1.5rc1/src/emcee/moves/move.py`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5/src/emcee/moves/red_blue.py` & `emcee-3.1.5rc1/src/emcee/moves/red_blue.py`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5/src/emcee/moves/stretch.py` & `emcee-3.1.5rc1/src/emcee/moves/stretch.py`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5/src/emcee/moves/walk.py` & `emcee-3.1.5rc1/src/emcee/moves/walk.py`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5/src/emcee/pbar.py` & `emcee-3.1.5rc1/src/emcee/pbar.py`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5/src/emcee/state.py` & `emcee-3.1.5rc1/src/emcee/state.py`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5/src/emcee/tests/integration/test_gaussian.py` & `emcee-3.1.5rc1/src/emcee/tests/integration/test_gaussian.py`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5/src/emcee/tests/integration/test_kde.py` & `emcee-3.1.5rc1/src/emcee/tests/integration/test_kde.py`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5/src/emcee/tests/integration/test_longdouble.py` & `emcee-3.1.5rc1/src/emcee/tests/integration/test_longdouble.py`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5/src/emcee/tests/integration/test_proposal.py` & `emcee-3.1.5rc1/src/emcee/tests/integration/test_proposal.py`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5/src/emcee/tests/integration/test_stretch.py` & `emcee-3.1.5rc1/src/emcee/tests/integration/test_stretch.py`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5/src/emcee/tests/unit/test_autocorr.py` & `emcee-3.1.5rc1/src/emcee/tests/unit/test_autocorr.py`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5/src/emcee/tests/unit/test_backends.py` & `emcee-3.1.5rc1/src/emcee/tests/unit/test_backends.py`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5/src/emcee/tests/unit/test_blobs.py` & `emcee-3.1.5rc1/src/emcee/tests/unit/test_blobs.py`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5/src/emcee/tests/unit/test_ensemble.py` & `emcee-3.1.5rc1/src/emcee/tests/unit/test_ensemble.py`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5/src/emcee/tests/unit/test_sampler.py` & `emcee-3.1.5rc1/src/emcee/tests/unit/test_sampler.py`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5/src/emcee/tests/unit/test_state.py` & `emcee-3.1.5rc1/src/emcee/tests/unit/test_state.py`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5/src/emcee/tests/unit/test_stretch.py` & `emcee-3.1.5rc1/src/emcee/tests/unit/test_stretch.py`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5/src/emcee/utils.py` & `emcee-3.1.5rc1/src/emcee/utils.py`

 * *Files identical despite different names*

### Comparing `emcee-3.1.5/src/emcee.egg-info/PKG-INFO` & `emcee-3.1.5rc1/src/emcee.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emcee
-Version: 3.1.5
+Version: 3.1.5rc1
 Summary: The Python ensemble sampling toolkit for MCMC
 Home-page: https://emcee.readthedocs.io
 Author: Daniel Foreman-Mackey
 Author-email: foreman.mackey@gmail.com
 Maintainer: Daniel Foreman-Mackey
 Maintainer-email: foreman.mackey@gmail.com
 License: MIT
```

### Comparing `emcee-3.1.5/src/emcee.egg-info/SOURCES.txt` & `emcee-3.1.5rc1/src/emcee.egg-info/SOURCES.txt`

 * *Files identical despite different names*

