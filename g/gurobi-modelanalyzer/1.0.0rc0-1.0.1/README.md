# Comparing `tmp/gurobi_modelanalyzer-1.0.0rc0.tar.gz` & `tmp/gurobi_modelanalyzer-1.0.1.tar.gz`

## Comparing `gurobi_modelanalyzer-1.0.0rc0.tar` & `gurobi_modelanalyzer-1.0.1.tar`

### file list

```diff
@@ -1,71 +1,71 @@
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.0rc0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.0rc0/.readthedocs.yaml
--rw-r--r--   0        0        0     5762 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.0rc0/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     3130 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.0rc0/CONTRIBUTING.md
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.0rc0/copyright.txt
--rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.0rc0/.github/workflows/build-wheel.yml
--rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.0rc0/.github/workflows/doc-build.yml
--rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.0rc0/.github/workflows/publish-pypi.yml
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.0rc0/.github/workflows/release.yml
--rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.0rc0/.github/workflows/test-wheels.yml
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.0rc0/.github/workflows/test.yml
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.0rc0/.github/workflows/unit-tests.yml
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.0rc0/docs/Makefile
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.0rc0/docs/README.md
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.0rc0/docs/make.bat
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.0rc0/docs/requirements.txt
--rw-r--r--   0        0        0    32836 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.0rc0/docs/source/advanced_usage_illcond.rst
--rw-r--r--   0        0        0     5268 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.0rc0/docs/source/apiref_illcond.rst
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.0rc0/docs/source/bib_illcond.bib
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.0rc0/docs/source/bib_illcond.rst
--rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.0rc0/docs/source/conf.py
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.0rc0/docs/source/contactus.rst
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.0rc0/docs/source/illcond.rst
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.0rc0/docs/source/index.rst
--rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.0rc0/docs/source/installation.rst
--rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.0rc0/docs/source/license.rst
--rw-r--r--   0        0        0     9461 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.0rc0/docs/source/quickstart_illcond.rst
--rw-r--r--   0        0        0   136593 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.0rc0/docs/source/_static/1603965_agg.png
--rw-r--r--   0        0        0   170358 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.0rc0/docs/source/_static/1603965_bitmap1.png
--rw-r--r--   0        0        0   108564 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.0rc0/docs/source/_static/1603965_bitmap2.png
--rw-r--r--   0        0        0    15517 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.0rc0/docs/source/_static/Basis.png
--rw-r--r--   0        0        0    19799 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.0rc0/docs/source/_static/BasisInv.png
--rw-r--r--   0        0        0    26296 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.0rc0/docs/source/_static/Binet.png
--rw-r--r--   0        0        0     7417 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.0rc0/docs/source/_static/gurobi-logo-title.png
--rw-r--r--   0        0        0    10344 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.0rc0/docs/source/_static/gurobi.png
--rw-r--r--   0        0        0    14546 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.0rc0/docs/source/_static/image8.png
--rw-r--r--   0        0        0   232669 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.0rc0/docs/source/_static/irish_bitmap.png
--rw-r--r--   0        0        0   397035 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.0rc0/docs/source/_static/irish_dualvals.png
--rw-r--r--   0        0        0    94865 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.0rc0/docs/source/_static/irish_fibonacci.png
--rw-r--r--   0        0        0   145061 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.0rc0/docs/source/_static/irish_pivots.png
--rw-r--r--   0        0        0   293841 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.0rc0/docs/source/_static/irish_reordered.png
--rwxr-xr-x   0        0        0      509 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.0rc0/examples/afiroill.lp.bz2
--rw-r--r--   0        0        0    16399 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.0rc0/examples/cantilever_sublp.bas.bz2
--rw-r--r--   0        0        0   643077 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.0rc0/examples/cantilever_sublp.mps.bz2
--rw-r--r--   0        0        0    20141 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.0rc0/examples/cantilever_sublp_kappaexplain.lp.bz2
--rw-r--r--   0        0        0  1650055 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.0rc0/examples/irish-electricity.mps.bz2
--rw-r--r--   0        0        0    78193 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.0rc0/examples/irish-electricity.mps_kappaexplain.lp.bz2
--rw-r--r--   0        0        0   322461 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.0rc0/examples/neos-1603965rel.mps.bz2
--rw-r--r--   0        0        0    17074 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.0rc0/examples/neos-1603965rel_kappaexplain.lp.bz2
--rw-r--r--   0        0        0   360205 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.0rc0/examples/ns2122603rel.mps.bz2
--rw-r--r--   0        0        0    25558 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.0rc0/examples/ns2122603rel_kappaexplain.lp.bz2
--rw-r--r--   0        0        0    34987 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.0rc0/examples/ns2122603rel_kappaexplain.mps.bz2
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.0rc0/src/gurobi_modelanalyzer/__init__.py
--rw-r--r--   0        0        0     4635 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.0rc0/src/gurobi_modelanalyzer/analyzer.py
--rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.0rc0/src/gurobi_modelanalyzer/basic_analyzer.py
--rw-r--r--   0        0        0    15488 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.0rc0/src/gurobi_modelanalyzer/common.py
--rw-r--r--   0        0        0    20842 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.0rc0/src/gurobi_modelanalyzer/constraint_analyzer.py
--rw-r--r--   0        0        0     6865 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.0rc0/src/gurobi_modelanalyzer/file_analyzer.py
--rw-r--r--   0        0        0     3184 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.0rc0/src/gurobi_modelanalyzer/objective_function_analyzer.py
--rw-r--r--   0        0        0    78748 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.0rc0/src/gurobi_modelanalyzer/results_analyzer.py
--rw-r--r--   0        0        0     2008 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.0rc0/src/gurobi_modelanalyzer/variable_analyzer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.0rc0/tests/__init__.py
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.0rc0/tests/test_analyzer.py
--rw-r--r--   0        0        0     2907 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.0rc0/tests/test_explainer.py
--rwxr-xr-x   0        0        0    84882 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.0rc0/tests/dataset/glass4.mps
--rwxr-xr-x   0        0        0     2213 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.0rc0/tests/dataset/p0033.lp
--rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.0rc0/.gitignore
--rw-r--r--   0        0        0    10976 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.0rc0/LICENSE
--rw-r--r--   0        0        0     3946 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.0rc0/README.md
--rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.0rc0/pyproject.toml
--rw-r--r--   0        0        0     4923 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.0rc0/PKG-INFO
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.1/.readthedocs.yaml
+-rw-r--r--   0        0        0     5762 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     3130 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.1/CONTRIBUTING.md
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.1/copyright.txt
+-rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.1/.github/workflows/build-wheel.yml
+-rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.1/.github/workflows/doc-build.yml
+-rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.1/.github/workflows/publish-pypi.yml
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.1/.github/workflows/release.yml
+-rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.1/.github/workflows/test-wheels.yml
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.1/.github/workflows/test.yml
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.1/.github/workflows/unit-tests.yml
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.1/docs/Makefile
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.1/docs/README.md
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.1/docs/make.bat
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.1/docs/requirements.txt
+-rw-r--r--   0        0        0    32836 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.1/docs/source/advanced_usage_illcond.rst
+-rw-r--r--   0        0        0     5268 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.1/docs/source/apiref_illcond.rst
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.1/docs/source/bib_illcond.bib
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.1/docs/source/bib_illcond.rst
+-rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.1/docs/source/conf.py
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.1/docs/source/contactus.rst
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.1/docs/source/illcond.rst
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.1/docs/source/index.rst
+-rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.1/docs/source/installation.rst
+-rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.1/docs/source/license.rst
+-rw-r--r--   0        0        0     9461 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.1/docs/source/quickstart_illcond.rst
+-rw-r--r--   0        0        0   136593 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.1/docs/source/_static/1603965_agg.png
+-rw-r--r--   0        0        0   170358 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.1/docs/source/_static/1603965_bitmap1.png
+-rw-r--r--   0        0        0   108564 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.1/docs/source/_static/1603965_bitmap2.png
+-rw-r--r--   0        0        0    15517 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.1/docs/source/_static/Basis.png
+-rw-r--r--   0        0        0    19799 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.1/docs/source/_static/BasisInv.png
+-rw-r--r--   0        0        0    26296 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.1/docs/source/_static/Binet.png
+-rw-r--r--   0        0        0     7417 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.1/docs/source/_static/gurobi-logo-title.png
+-rw-r--r--   0        0        0    10344 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.1/docs/source/_static/gurobi.png
+-rw-r--r--   0        0        0    14546 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.1/docs/source/_static/image8.png
+-rw-r--r--   0        0        0   232669 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.1/docs/source/_static/irish_bitmap.png
+-rw-r--r--   0        0        0   397035 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.1/docs/source/_static/irish_dualvals.png
+-rw-r--r--   0        0        0    94865 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.1/docs/source/_static/irish_fibonacci.png
+-rw-r--r--   0        0        0   145061 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.1/docs/source/_static/irish_pivots.png
+-rw-r--r--   0        0        0   293841 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.1/docs/source/_static/irish_reordered.png
+-rwxr-xr-x   0        0        0      509 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.1/examples/afiroill.lp.bz2
+-rw-r--r--   0        0        0    16399 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.1/examples/cantilever_sublp.bas.bz2
+-rw-r--r--   0        0        0   643077 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.1/examples/cantilever_sublp.mps.bz2
+-rw-r--r--   0        0        0    20141 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.1/examples/cantilever_sublp_kappaexplain.lp.bz2
+-rw-r--r--   0        0        0  1650055 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.1/examples/irish-electricity.mps.bz2
+-rw-r--r--   0        0        0    78193 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.1/examples/irish-electricity.mps_kappaexplain.lp.bz2
+-rw-r--r--   0        0        0   322461 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.1/examples/neos-1603965rel.mps.bz2
+-rw-r--r--   0        0        0    17074 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.1/examples/neos-1603965rel_kappaexplain.lp.bz2
+-rw-r--r--   0        0        0   360205 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.1/examples/ns2122603rel.mps.bz2
+-rw-r--r--   0        0        0    25558 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.1/examples/ns2122603rel_kappaexplain.lp.bz2
+-rw-r--r--   0        0        0    34987 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.1/examples/ns2122603rel_kappaexplain.mps.bz2
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.1/src/gurobi_modelanalyzer/__init__.py
+-rw-r--r--   0        0        0     4635 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.1/src/gurobi_modelanalyzer/analyzer.py
+-rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.1/src/gurobi_modelanalyzer/basic_analyzer.py
+-rw-r--r--   0        0        0    15488 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.1/src/gurobi_modelanalyzer/common.py
+-rw-r--r--   0        0        0    20842 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.1/src/gurobi_modelanalyzer/constraint_analyzer.py
+-rw-r--r--   0        0        0     6865 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.1/src/gurobi_modelanalyzer/file_analyzer.py
+-rw-r--r--   0        0        0     3184 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.1/src/gurobi_modelanalyzer/objective_function_analyzer.py
+-rw-r--r--   0        0        0    78754 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.1/src/gurobi_modelanalyzer/results_analyzer.py
+-rw-r--r--   0        0        0     2008 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.1/src/gurobi_modelanalyzer/variable_analyzer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.1/tests/__init__.py
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.1/tests/test_analyzer.py
+-rw-r--r--   0        0        0     2907 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.1/tests/test_explainer.py
+-rwxr-xr-x   0        0        0    84882 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.1/tests/dataset/glass4.mps
+-rwxr-xr-x   0        0        0     2213 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.1/tests/dataset/p0033.lp
+-rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.1/.gitignore
+-rw-r--r--   0        0        0    10976 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.1/LICENSE
+-rw-r--r--   0        0        0     3946 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.1/README.md
+-rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     4920 2020-02-02 00:00:00.000000 gurobi_modelanalyzer-1.0.1/PKG-INFO
```

### Comparing `gurobi_modelanalyzer-1.0.0rc0/.pre-commit-config.yaml` & `gurobi_modelanalyzer-1.0.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `gurobi_modelanalyzer-1.0.0rc0/CODE_OF_CONDUCT.md` & `gurobi_modelanalyzer-1.0.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `gurobi_modelanalyzer-1.0.0rc0/CONTRIBUTING.md` & `gurobi_modelanalyzer-1.0.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `gurobi_modelanalyzer-1.0.0rc0/copyright.txt` & `gurobi_modelanalyzer-1.0.1/copyright.txt`

 * *Files identical despite different names*

### Comparing `gurobi_modelanalyzer-1.0.0rc0/.github/workflows/build-wheel.yml` & `gurobi_modelanalyzer-1.0.1/.github/workflows/build-wheel.yml`

 * *Files identical despite different names*

### Comparing `gurobi_modelanalyzer-1.0.0rc0/.github/workflows/doc-build.yml` & `gurobi_modelanalyzer-1.0.1/.github/workflows/doc-build.yml`

 * *Files identical despite different names*

### Comparing `gurobi_modelanalyzer-1.0.0rc0/.github/workflows/publish-pypi.yml` & `gurobi_modelanalyzer-1.0.1/.github/workflows/publish-pypi.yml`

 * *Files identical despite different names*

### Comparing `gurobi_modelanalyzer-1.0.0rc0/.github/workflows/test-wheels.yml` & `gurobi_modelanalyzer-1.0.1/.github/workflows/test-wheels.yml`

 * *Files identical despite different names*

### Comparing `gurobi_modelanalyzer-1.0.0rc0/.github/workflows/unit-tests.yml` & `gurobi_modelanalyzer-1.0.1/.github/workflows/unit-tests.yml`

 * *Files identical despite different names*

### Comparing `gurobi_modelanalyzer-1.0.0rc0/docs/Makefile` & `gurobi_modelanalyzer-1.0.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `gurobi_modelanalyzer-1.0.0rc0/docs/README.md` & `gurobi_modelanalyzer-1.0.1/docs/README.md`

 * *Files identical despite different names*

### Comparing `gurobi_modelanalyzer-1.0.0rc0/docs/make.bat` & `gurobi_modelanalyzer-1.0.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `gurobi_modelanalyzer-1.0.0rc0/docs/source/advanced_usage_illcond.rst` & `gurobi_modelanalyzer-1.0.1/docs/source/advanced_usage_illcond.rst`

 * *Files identical despite different names*

### Comparing `gurobi_modelanalyzer-1.0.0rc0/docs/source/apiref_illcond.rst` & `gurobi_modelanalyzer-1.0.1/docs/source/apiref_illcond.rst`

 * *Files identical despite different names*

### Comparing `gurobi_modelanalyzer-1.0.0rc0/docs/source/bib_illcond.bib` & `gurobi_modelanalyzer-1.0.1/docs/source/bib_illcond.bib`

 * *Files identical despite different names*

### Comparing `gurobi_modelanalyzer-1.0.0rc0/docs/source/conf.py` & `gurobi_modelanalyzer-1.0.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `gurobi_modelanalyzer-1.0.0rc0/docs/source/index.rst` & `gurobi_modelanalyzer-1.0.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `gurobi_modelanalyzer-1.0.0rc0/docs/source/installation.rst` & `gurobi_modelanalyzer-1.0.1/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `gurobi_modelanalyzer-1.0.0rc0/docs/source/license.rst` & `gurobi_modelanalyzer-1.0.1/docs/source/license.rst`

 * *Files identical despite different names*

### Comparing `gurobi_modelanalyzer-1.0.0rc0/docs/source/quickstart_illcond.rst` & `gurobi_modelanalyzer-1.0.1/docs/source/quickstart_illcond.rst`

 * *Files identical despite different names*

### Comparing `gurobi_modelanalyzer-1.0.0rc0/docs/source/_static/1603965_agg.png` & `gurobi_modelanalyzer-1.0.1/docs/source/_static/1603965_agg.png`

 * *Files identical despite different names*

### Comparing `gurobi_modelanalyzer-1.0.0rc0/docs/source/_static/1603965_bitmap1.png` & `gurobi_modelanalyzer-1.0.1/docs/source/_static/1603965_bitmap1.png`

 * *Files identical despite different names*

### Comparing `gurobi_modelanalyzer-1.0.0rc0/docs/source/_static/1603965_bitmap2.png` & `gurobi_modelanalyzer-1.0.1/docs/source/_static/1603965_bitmap2.png`

 * *Files identical despite different names*

### Comparing `gurobi_modelanalyzer-1.0.0rc0/docs/source/_static/Basis.png` & `gurobi_modelanalyzer-1.0.1/docs/source/_static/Basis.png`

 * *Files identical despite different names*

### Comparing `gurobi_modelanalyzer-1.0.0rc0/docs/source/_static/BasisInv.png` & `gurobi_modelanalyzer-1.0.1/docs/source/_static/BasisInv.png`

 * *Files identical despite different names*

### Comparing `gurobi_modelanalyzer-1.0.0rc0/docs/source/_static/Binet.png` & `gurobi_modelanalyzer-1.0.1/docs/source/_static/Binet.png`

 * *Files identical despite different names*

### Comparing `gurobi_modelanalyzer-1.0.0rc0/docs/source/_static/gurobi-logo-title.png` & `gurobi_modelanalyzer-1.0.1/docs/source/_static/gurobi-logo-title.png`

 * *Files identical despite different names*

### Comparing `gurobi_modelanalyzer-1.0.0rc0/docs/source/_static/gurobi.png` & `gurobi_modelanalyzer-1.0.1/docs/source/_static/gurobi.png`

 * *Files identical despite different names*

### Comparing `gurobi_modelanalyzer-1.0.0rc0/docs/source/_static/image8.png` & `gurobi_modelanalyzer-1.0.1/docs/source/_static/image8.png`

 * *Files identical despite different names*

### Comparing `gurobi_modelanalyzer-1.0.0rc0/docs/source/_static/irish_bitmap.png` & `gurobi_modelanalyzer-1.0.1/docs/source/_static/irish_bitmap.png`

 * *Files identical despite different names*

### Comparing `gurobi_modelanalyzer-1.0.0rc0/docs/source/_static/irish_dualvals.png` & `gurobi_modelanalyzer-1.0.1/docs/source/_static/irish_dualvals.png`

 * *Files identical despite different names*

### Comparing `gurobi_modelanalyzer-1.0.0rc0/docs/source/_static/irish_fibonacci.png` & `gurobi_modelanalyzer-1.0.1/docs/source/_static/irish_fibonacci.png`

 * *Files identical despite different names*

### Comparing `gurobi_modelanalyzer-1.0.0rc0/docs/source/_static/irish_pivots.png` & `gurobi_modelanalyzer-1.0.1/docs/source/_static/irish_pivots.png`

 * *Files identical despite different names*

### Comparing `gurobi_modelanalyzer-1.0.0rc0/docs/source/_static/irish_reordered.png` & `gurobi_modelanalyzer-1.0.1/docs/source/_static/irish_reordered.png`

 * *Files identical despite different names*

### Comparing `gurobi_modelanalyzer-1.0.0rc0/examples/cantilever_sublp.bas.bz2` & `gurobi_modelanalyzer-1.0.1/examples/cantilever_sublp.bas.bz2`

 * *Files identical despite different names*

### Comparing `gurobi_modelanalyzer-1.0.0rc0/examples/cantilever_sublp.mps.bz2` & `gurobi_modelanalyzer-1.0.1/examples/cantilever_sublp.mps.bz2`

 * *Files identical despite different names*

### Comparing `gurobi_modelanalyzer-1.0.0rc0/examples/cantilever_sublp_kappaexplain.lp.bz2` & `gurobi_modelanalyzer-1.0.1/examples/cantilever_sublp_kappaexplain.lp.bz2`

 * *Files identical despite different names*

### Comparing `gurobi_modelanalyzer-1.0.0rc0/examples/irish-electricity.mps.bz2` & `gurobi_modelanalyzer-1.0.1/examples/irish-electricity.mps.bz2`

 * *Files identical despite different names*

### Comparing `gurobi_modelanalyzer-1.0.0rc0/examples/irish-electricity.mps_kappaexplain.lp.bz2` & `gurobi_modelanalyzer-1.0.1/examples/irish-electricity.mps_kappaexplain.lp.bz2`

 * *Files identical despite different names*

### Comparing `gurobi_modelanalyzer-1.0.0rc0/examples/neos-1603965rel.mps.bz2` & `gurobi_modelanalyzer-1.0.1/examples/neos-1603965rel.mps.bz2`

 * *Files identical despite different names*

### Comparing `gurobi_modelanalyzer-1.0.0rc0/examples/neos-1603965rel_kappaexplain.lp.bz2` & `gurobi_modelanalyzer-1.0.1/examples/neos-1603965rel_kappaexplain.lp.bz2`

 * *Files identical despite different names*

### Comparing `gurobi_modelanalyzer-1.0.0rc0/examples/ns2122603rel.mps.bz2` & `gurobi_modelanalyzer-1.0.1/examples/ns2122603rel.mps.bz2`

 * *Files identical despite different names*

### Comparing `gurobi_modelanalyzer-1.0.0rc0/examples/ns2122603rel_kappaexplain.lp.bz2` & `gurobi_modelanalyzer-1.0.1/examples/ns2122603rel_kappaexplain.lp.bz2`

 * *Files identical despite different names*

### Comparing `gurobi_modelanalyzer-1.0.0rc0/examples/ns2122603rel_kappaexplain.mps.bz2` & `gurobi_modelanalyzer-1.0.1/examples/ns2122603rel_kappaexplain.mps.bz2`

 * *Files identical despite different names*

### Comparing `gurobi_modelanalyzer-1.0.0rc0/src/gurobi_modelanalyzer/analyzer.py` & `gurobi_modelanalyzer-1.0.1/src/gurobi_modelanalyzer/analyzer.py`

 * *Files identical despite different names*

### Comparing `gurobi_modelanalyzer-1.0.0rc0/src/gurobi_modelanalyzer/basic_analyzer.py` & `gurobi_modelanalyzer-1.0.1/src/gurobi_modelanalyzer/basic_analyzer.py`

 * *Files identical despite different names*

### Comparing `gurobi_modelanalyzer-1.0.0rc0/src/gurobi_modelanalyzer/common.py` & `gurobi_modelanalyzer-1.0.1/src/gurobi_modelanalyzer/common.py`

 * *Files identical despite different names*

### Comparing `gurobi_modelanalyzer-1.0.0rc0/src/gurobi_modelanalyzer/constraint_analyzer.py` & `gurobi_modelanalyzer-1.0.1/src/gurobi_modelanalyzer/constraint_analyzer.py`

 * *Files identical despite different names*

### Comparing `gurobi_modelanalyzer-1.0.0rc0/src/gurobi_modelanalyzer/file_analyzer.py` & `gurobi_modelanalyzer-1.0.1/src/gurobi_modelanalyzer/file_analyzer.py`

 * *Files identical despite different names*

### Comparing `gurobi_modelanalyzer-1.0.0rc0/src/gurobi_modelanalyzer/objective_function_analyzer.py` & `gurobi_modelanalyzer-1.0.1/src/gurobi_modelanalyzer/objective_function_analyzer.py`

 * *Files identical despite different names*

### Comparing `gurobi_modelanalyzer-1.0.0rc0/src/gurobi_modelanalyzer/results_analyzer.py` & `gurobi_modelanalyzer-1.0.1/src/gurobi_modelanalyzer/results_analyzer.py`

 * *Files 1% similar despite different names*

```diff
@@ -571,15 +571,15 @@
             tmp = 0  # No statuses or factorization; solve from scratch
 
         model.optimize()
         try:  # Confirm basis available after solve.
             tmp2 = modvars[0].VBasis
             tmp1 = modvars[0].X
         except AttributeError as e:  # no basis; no explanation to return
-            return None, None, None, None
+            return None, None, None, None, None
 
     m = model.numConstrs
     n = model.numVars
     #
     #   Extract the basic structural variables from the model into the model
     #   containing the basis matrix of interest.  When explaining by rows,
     #   each column of the basis matrix corresponds to a constraint in the
```

### Comparing `gurobi_modelanalyzer-1.0.0rc0/src/gurobi_modelanalyzer/variable_analyzer.py` & `gurobi_modelanalyzer-1.0.1/src/gurobi_modelanalyzer/variable_analyzer.py`

 * *Files identical despite different names*

### Comparing `gurobi_modelanalyzer-1.0.0rc0/tests/test_explainer.py` & `gurobi_modelanalyzer-1.0.1/tests/test_explainer.py`

 * *Files identical despite different names*

### Comparing `gurobi_modelanalyzer-1.0.0rc0/tests/dataset/glass4.mps` & `gurobi_modelanalyzer-1.0.1/tests/dataset/glass4.mps`

 * *Files identical despite different names*

### Comparing `gurobi_modelanalyzer-1.0.0rc0/tests/dataset/p0033.lp` & `gurobi_modelanalyzer-1.0.1/tests/dataset/p0033.lp`

 * *Files identical despite different names*

### Comparing `gurobi_modelanalyzer-1.0.0rc0/.gitignore` & `gurobi_modelanalyzer-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `gurobi_modelanalyzer-1.0.0rc0/LICENSE` & `gurobi_modelanalyzer-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gurobi_modelanalyzer-1.0.0rc0/README.md` & `gurobi_modelanalyzer-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `gurobi_modelanalyzer-1.0.0rc0/pyproject.toml` & `gurobi_modelanalyzer-1.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gurobi_modelanalyzer-1.0.0rc0/PKG-INFO` & `gurobi_modelanalyzer-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: gurobi-modelanalyzer
-Version: 1.0.0rc0
+Version: 1.0.1
 Summary: Model analysis tools; v1.0 is an ill conditioning explainer.
 Project-URL: Documentation, https://gurobi-optimization-gurobi-modelanalyzer.readthedocs-hosted.com/en/latest
 Project-URL: Issues, https://github.com/Gurobi/gurobi-modelanalyzer/issues
 Project-URL: Source, https://github.com/Gurobi/gurobi-modelanalyzer
 Author-email: Ed Klotz <klotz@gurobi.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
```

