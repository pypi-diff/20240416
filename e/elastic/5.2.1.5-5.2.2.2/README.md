# Comparing `tmp/elastic-5.2.1.5.tar.gz` & `tmp/elastic-5.2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elastic-5.2.1.5.tar", last modified: Mon Apr 15 21:51:16 2024, max compression
+gzip compressed data, was "elastic-5.2.2.2.tar", last modified: Mon Apr 15 23:43:47 2024, max compression
```

## Comparing `elastic-5.2.1.5.tar` & `elastic-5.2.2.2.tar`

### file list

```diff
@@ -1,155 +1,155 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:51:16.554148 elastic-5.2.1.5/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-15 21:51:11.000000 elastic-5.2.1.5/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:51:16.530148 elastic-5.2.1.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:51:16.538148 elastic-5.2.1.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-04-15 21:51:11.000000 elastic-5.2.1.5/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-15 21:51:11.000000 elastic-5.2.1.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-15 21:51:11.000000 elastic-5.2.1.5/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-15 21:51:11.000000 elastic-5.2.1.5/Contributors
--rw-r--r--   0 runner    (1001) docker     (127)    35121 2024-04-15 21:51:11.000000 elastic-5.2.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-15 21:51:11.000000 elastic-5.2.1.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3448 2024-04-15 21:51:16.554148 elastic-5.2.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-04-15 21:51:11.000000 elastic-5.2.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:51:16.538148 elastic-5.2.1.5/conda/
--rwxr-xr-x   0 runner    (1001) docker     (127)      282 2024-04-15 21:51:11.000000 elastic-5.2.1.5/conda/anaconda_deploy.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-04-15 21:51:11.000000 elastic-5.2.1.5/conda/meta.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:51:16.538148 elastic-5.2.1.5/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     4598 2024-04-15 21:51:11.000000 elastic-5.2.1.5/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-15 21:51:11.000000 elastic-5.2.1.5/docs/_config.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2956 2024-04-15 21:51:11.000000 elastic-5.2.1.5/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:51:16.538148 elastic-5.2.1.5/docs/notebook/
--rw-r--r--   0 runner    (1001) docker     (127)    60989 2024-04-15 21:51:11.000000 elastic-5.2.1.5/docs/notebook/lib-usage.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:51:16.538148 elastic-5.2.1.5/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:51:16.538148 elastic-5.2.1.5/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-04-15 21:51:11.000000 elastic-5.2.1.5/docs/source/_static/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:51:16.538148 elastic-5.2.1.5/docs/source/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-04-15 21:51:11.000000 elastic-5.2.1.5/docs/source/_templates/layout.html
--rw-r--r--   0 runner    (1001) docker     (127)     6086 2024-04-15 21:51:11.000000 elastic-5.2.1.5/docs/source/cli-usage.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8465 2024-04-15 21:51:11.000000 elastic-5.2.1.5/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     8304 2024-04-15 21:51:11.000000 elastic-5.2.1.5/docs/source/conf.py.tmpl
--rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-04-15 21:51:11.000000 elastic-5.2.1.5/docs/source/endmatter.rst
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 21:51:11.000000 elastic-5.2.1.5/docs/source/examples.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:51:16.542147 elastic-5.2.1.5/docs/source/fig/
--rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-04-15 21:51:11.000000 elastic-5.2.1.5/docs/source/fig/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-04-15 21:51:11.000000 elastic-5.2.1.5/docs/source/fig/favicon.png
--rw-r--r--   0 runner    (1001) docker     (127)     5145 2024-04-15 21:51:11.000000 elastic-5.2.1.5/docs/source/fig/favicon.svg
--rw-r--r--   0 runner    (1001) docker     (127)     7319 2024-04-15 21:51:11.000000 elastic-5.2.1.5/docs/source/fig/plot1.pdf
--rw-r--r--   0 runner    (1001) docker     (127)    17836 2024-04-15 21:51:11.000000 elastic-5.2.1.5/docs/source/fig/plot1.png
--rw-r--r--   0 runner    (1001) docker     (127)    24292 2024-04-15 21:51:11.000000 elastic-5.2.1.5/docs/source/fig/plot1.svg
--rw-r--r--   0 runner    (1001) docker     (127)     5703 2024-04-15 21:51:11.000000 elastic-5.2.1.5/docs/source/fig/plot2.pdf
--rw-r--r--   0 runner    (1001) docker     (127)    24303 2024-04-15 21:51:11.000000 elastic-5.2.1.5/docs/source/fig/plot2.png
--rw-r--r--   0 runner    (1001) docker     (127)    18497 2024-04-15 21:51:11.000000 elastic-5.2.1.5/docs/source/fig/plot2.svg
--rw-r--r--   0 runner    (1001) docker     (127)     7407 2024-04-15 21:51:11.000000 elastic-5.2.1.5/docs/source/fig/plot3.pdf
--rw-r--r--   0 runner    (1001) docker     (127)    28926 2024-04-15 21:51:11.000000 elastic-5.2.1.5/docs/source/fig/plot3.png
--rw-r--r--   0 runner    (1001) docker     (127)    27181 2024-04-15 21:51:11.000000 elastic-5.2.1.5/docs/source/fig/plot3.svg
--rw-r--r--   0 runner    (1001) docker     (127)     7757 2024-04-15 21:51:11.000000 elastic-5.2.1.5/docs/source/fig/plot3a.pdf
--rw-r--r--   0 runner    (1001) docker     (127)    34509 2024-04-15 21:51:11.000000 elastic-5.2.1.5/docs/source/fig/plot3a.png
--rw-r--r--   0 runner    (1001) docker     (127)    36285 2024-04-15 21:51:11.000000 elastic-5.2.1.5/docs/source/fig/plot3a.svg
--rw-r--r--   0 runner    (1001) docker     (127)     7419 2024-04-15 21:51:11.000000 elastic-5.2.1.5/docs/source/fig/plot3b.pdf
--rw-r--r--   0 runner    (1001) docker     (127)    27897 2024-04-15 21:51:11.000000 elastic-5.2.1.5/docs/source/fig/plot3b.png
--rw-r--r--   0 runner    (1001) docker     (127)    30417 2024-04-15 21:51:11.000000 elastic-5.2.1.5/docs/source/fig/plot3b.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-04-15 21:51:11.000000 elastic-5.2.1.5/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)    15113 2024-04-15 21:51:11.000000 elastic-5.2.1.5/docs/source/intro.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9637 2024-04-15 21:51:11.000000 elastic-5.2.1.5/docs/source/lib-usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:51:16.542147 elastic-5.2.1.5/docs/source/lib-usage_files/
--rw-r--r--   0 runner    (1001) docker     (127)    11186 2024-04-15 21:51:11.000000 elastic-5.2.1.5/docs/source/lib-usage_files/lib-usage_12_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    18112 2024-04-15 21:51:11.000000 elastic-5.2.1.5/docs/source/lib-usage_files/lib-usage_18_1.png
--rw-r--r--   0 runner    (1001) docker     (127)     4947 2024-04-15 21:51:11.000000 elastic-5.2.1.5/docs/source/lib-usage_files/lib-usage_9_1.png
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-15 21:51:11.000000 elastic-5.2.1.5/docs/source/modules.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:51:16.542147 elastic-5.2.1.5/elastic/
--rw-r--r--   0 runner    (1001) docker     (127)     2639 2024-04-15 21:51:11.000000 elastic-5.2.1.5/elastic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-15 21:51:16.000000 elastic-5.2.1.5/elastic/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:51:16.546148 elastic-5.2.1.5/elastic/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 21:51:11.000000 elastic-5.2.1.5/elastic/cli/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5857 2024-04-15 21:51:11.000000 elastic-5.2.1.5/elastic/cli/elastic.py
--rw-r--r--   0 runner    (1001) docker     (127)    26585 2024-04-15 21:51:11.000000 elastic-5.2.1.5/elastic/elastic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:51:16.554148 elastic-5.2.1.5/elastic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3448 2024-04-15 21:51:16.000000 elastic-5.2.1.5/elastic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2958 2024-04-15 21:51:16.000000 elastic-5.2.1.5/elastic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 21:51:16.000000 elastic-5.2.1.5/elastic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-15 21:51:16.000000 elastic-5.2.1.5/elastic.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-15 21:51:16.000000 elastic-5.2.1.5/elastic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-15 21:51:16.000000 elastic-5.2.1.5/elastic.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:51:16.546148 elastic-5.2.1.5/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-04-15 21:51:11.000000 elastic-5.2.1.5/examples/example1.py
--rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-04-15 21:51:11.000000 elastic-5.2.1.5/examples/example2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-04-15 21:51:11.000000 elastic-5.2.1.5/examples/example3.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:51:16.546148 elastic-5.2.1.5/examples/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)      486 2024-04-15 21:51:11.000000 elastic-5.2.1.5/examples/scripts/check-job
--rwxr-xr-x   0 runner    (1001) docker     (127)       48 2024-04-15 21:51:11.000000 elastic-5.2.1.5/examples/scripts/run-on-tsi
--rwxr-xr-x   0 runner    (1001) docker     (127)     2106 2024-04-15 21:51:11.000000 elastic-5.2.1.5/examples/scripts/run-vasp5-lock
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-15 21:51:11.000000 elastic-5.2.1.5/examples/scripts/run_vasp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-04-15 21:51:11.000000 elastic-5.2.1.5/paper.bib
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-15 21:51:11.000000 elastic-5.2.1.5/paper.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:51:16.546148 elastic-5.2.1.5/parcalc/
--rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-04-15 21:51:11.000000 elastic-5.2.1.5/parcalc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24638 2024-04-15 21:51:11.000000 elastic-5.2.1.5/parcalc/parcalc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-04-15 21:51:11.000000 elastic-5.2.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 21:51:11.000000 elastic-5.2.1.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 21:51:16.554148 elastic-5.2.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-15 21:51:11.000000 elastic-5.2.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:51:16.546148 elastic-5.2.1.5/test/
--rw-r--r--   0 runner    (1001) docker     (127)     3526 2024-04-15 21:51:11.000000 elastic-5.2.1.5/test/test_elastic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:51:16.546148 elastic-5.2.1.5/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:51:16.550148 elastic-5.2.1.5/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-15 21:51:11.000000 elastic-5.2.1.5/tests/data/INCAR
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-15 21:51:11.000000 elastic-5.2.1.5/tests/data/KPOINTS
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-15 21:51:11.000000 elastic-5.2.1.5/tests/data/POSCAR
--rw-r--r--   0 runner    (1001) docker     (127)   438201 2024-04-15 21:51:11.000000 elastic-5.2.1.5/tests/data/POTCAR
--rw-r--r--   0 runner    (1001) docker     (127)      925 2024-04-15 21:51:11.000000 elastic-5.2.1.5/tests/data/abinit
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:51:16.550148 elastic-5.2.1.5/tests/data/calc-cij_000/
--rw-r--r--   0 runner    (1001) docker     (127)    44183 2024-04-15 21:51:11.000000 elastic-5.2.1.5/tests/data/calc-cij_000/vasprun.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:51:16.550148 elastic-5.2.1.5/tests/data/calc-cij_001/
--rw-r--r--   0 runner    (1001) docker     (127)    46925 2024-04-15 21:51:11.000000 elastic-5.2.1.5/tests/data/calc-cij_001/vasprun.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:51:16.550148 elastic-5.2.1.5/tests/data/calc-cij_002/
--rw-r--r--   0 runner    (1001) docker     (127)    46183 2024-04-15 21:51:11.000000 elastic-5.2.1.5/tests/data/calc-cij_002/vasprun.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:51:16.550148 elastic-5.2.1.5/tests/data/calc-cij_003/
--rw-r--r--   0 runner    (1001) docker     (127)    44183 2024-04-15 21:51:11.000000 elastic-5.2.1.5/tests/data/calc-cij_003/vasprun.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:51:16.550148 elastic-5.2.1.5/tests/data/calc-cij_004/
--rw-r--r--   0 runner    (1001) docker     (127)    46183 2024-04-15 21:51:11.000000 elastic-5.2.1.5/tests/data/calc-cij_004/vasprun.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:51:16.550148 elastic-5.2.1.5/tests/data/calc-cij_005/
--rw-r--r--   0 runner    (1001) docker     (127)    46183 2024-04-15 21:51:11.000000 elastic-5.2.1.5/tests/data/calc-cij_005/vasprun.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:51:16.550148 elastic-5.2.1.5/tests/data/calc-cij_006/
--rw-r--r--   0 runner    (1001) docker     (127)    48183 2024-04-15 21:51:11.000000 elastic-5.2.1.5/tests/data/calc-cij_006/vasprun.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:51:16.550148 elastic-5.2.1.5/tests/data/calc-cij_007/
--rw-r--r--   0 runner    (1001) docker     (127)    50184 2024-04-15 21:51:11.000000 elastic-5.2.1.5/tests/data/calc-cij_007/vasprun.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:51:16.554148 elastic-5.2.1.5/tests/data/calc-cij_008/
--rw-r--r--   0 runner    (1001) docker     (127)    50926 2024-04-15 21:51:11.000000 elastic-5.2.1.5/tests/data/calc-cij_008/vasprun.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:51:16.554148 elastic-5.2.1.5/tests/data/calc-cij_009/
--rw-r--r--   0 runner    (1001) docker     (127)    50926 2024-04-15 21:51:11.000000 elastic-5.2.1.5/tests/data/calc-cij_009/vasprun.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:51:16.554148 elastic-5.2.1.5/tests/data/calc-cij_010/
--rw-r--r--   0 runner    (1001) docker     (127)    50926 2024-04-15 21:51:11.000000 elastic-5.2.1.5/tests/data/calc-cij_010/vasprun.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:51:16.554148 elastic-5.2.1.5/tests/data/calc-eos_000/
--rw-r--r--   0 runner    (1001) docker     (127)    44183 2024-04-15 21:51:11.000000 elastic-5.2.1.5/tests/data/calc-eos_000/vasprun.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:51:16.554148 elastic-5.2.1.5/tests/data/calc-eos_001/
--rw-r--r--   0 runner    (1001) docker     (127)    44183 2024-04-15 21:51:11.000000 elastic-5.2.1.5/tests/data/calc-eos_001/vasprun.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:51:16.554148 elastic-5.2.1.5/tests/data/calc-eos_002/
--rw-r--r--   0 runner    (1001) docker     (127)    44183 2024-04-15 21:51:11.000000 elastic-5.2.1.5/tests/data/calc-eos_002/vasprun.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:51:16.554148 elastic-5.2.1.5/tests/data/calc-eos_003/
--rw-r--r--   0 runner    (1001) docker     (127)    44183 2024-04-15 21:51:11.000000 elastic-5.2.1.5/tests/data/calc-eos_003/vasprun.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:51:16.554148 elastic-5.2.1.5/tests/data/calc-eos_004/
--rw-r--r--   0 runner    (1001) docker     (127)    44183 2024-04-15 21:51:11.000000 elastic-5.2.1.5/tests/data/calc-eos_004/vasprun.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:51:16.554148 elastic-5.2.1.5/tests/data/calc-eos_005/
--rw-r--r--   0 runner    (1001) docker     (127)    44183 2024-04-15 21:51:11.000000 elastic-5.2.1.5/tests/data/calc-eos_005/vasprun.xml
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-15 21:51:11.000000 elastic-5.2.1.5/tests/data/cij_000.POSCAR
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-15 21:51:11.000000 elastic-5.2.1.5/tests/data/cij_001.POSCAR
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-15 21:51:11.000000 elastic-5.2.1.5/tests/data/cij_002.POSCAR
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-15 21:51:11.000000 elastic-5.2.1.5/tests/data/cij_003.POSCAR
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-15 21:51:11.000000 elastic-5.2.1.5/tests/data/cij_004.POSCAR
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-15 21:51:11.000000 elastic-5.2.1.5/tests/data/cij_005.POSCAR
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-15 21:51:11.000000 elastic-5.2.1.5/tests/data/cij_006.POSCAR
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-15 21:51:11.000000 elastic-5.2.1.5/tests/data/cij_007.POSCAR
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-15 21:51:11.000000 elastic-5.2.1.5/tests/data/cij_008.POSCAR
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-15 21:51:11.000000 elastic-5.2.1.5/tests/data/cij_009.POSCAR
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-15 21:51:11.000000 elastic-5.2.1.5/tests/data/cij_010.POSCAR
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-15 21:51:11.000000 elastic-5.2.1.5/tests/data/eos_000.POSCAR
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-15 21:51:11.000000 elastic-5.2.1.5/tests/data/eos_001.POSCAR
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-15 21:51:11.000000 elastic-5.2.1.5/tests/data/eos_002.POSCAR
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-15 21:51:11.000000 elastic-5.2.1.5/tests/data/eos_003.POSCAR
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-15 21:51:11.000000 elastic-5.2.1.5/tests/data/eos_004.POSCAR
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-15 21:51:11.000000 elastic-5.2.1.5/tests/data/eos_005.POSCAR
--rwxr-xr-x   0 runner    (1001) docker     (127)      319 2024-04-15 21:51:11.000000 elastic-5.2.1.5/tests/data/run-calcs
--rwxr-xr-x   0 runner    (1001) docker     (127)      190 2024-04-15 21:51:11.000000 elastic-5.2.1.5/tests/runtest.sh
--rw-r--r--   0 runner    (1001) docker     (127)     7656 2024-04-15 21:51:11.000000 elastic-5.2.1.5/tests/test_01.py
--rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-04-15 21:51:11.000000 elastic-5.2.1.5/tests/test_02.py
--rw-r--r--   0 runner    (1001) docker     (127)     6441 2024-04-15 21:51:11.000000 elastic-5.2.1.5/tests/test_elastic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 23:43:47.467111 elastic-5.2.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-15 23:43:43.000000 elastic-5.2.2.2/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 23:43:47.443111 elastic-5.2.2.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 23:43:47.447111 elastic-5.2.2.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-04-15 23:43:43.000000 elastic-5.2.2.2/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-15 23:43:43.000000 elastic-5.2.2.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-15 23:43:43.000000 elastic-5.2.2.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-15 23:43:43.000000 elastic-5.2.2.2/Contributors
+-rw-r--r--   0 runner    (1001) docker     (127)    35121 2024-04-15 23:43:43.000000 elastic-5.2.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-15 23:43:43.000000 elastic-5.2.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3448 2024-04-15 23:43:47.467111 elastic-5.2.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-04-15 23:43:43.000000 elastic-5.2.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 23:43:47.447111 elastic-5.2.2.2/conda/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      282 2024-04-15 23:43:43.000000 elastic-5.2.2.2/conda/anaconda_deploy.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-04-15 23:43:43.000000 elastic-5.2.2.2/conda/meta.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 23:43:47.447111 elastic-5.2.2.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     4598 2024-04-15 23:43:43.000000 elastic-5.2.2.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-15 23:43:43.000000 elastic-5.2.2.2/docs/_config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2956 2024-04-15 23:43:43.000000 elastic-5.2.2.2/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 23:43:47.447111 elastic-5.2.2.2/docs/notebook/
+-rw-r--r--   0 runner    (1001) docker     (127)    60989 2024-04-15 23:43:43.000000 elastic-5.2.2.2/docs/notebook/lib-usage.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 23:43:47.451111 elastic-5.2.2.2/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 23:43:47.451111 elastic-5.2.2.2/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-04-15 23:43:43.000000 elastic-5.2.2.2/docs/source/_static/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 23:43:47.451111 elastic-5.2.2.2/docs/source/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-04-15 23:43:43.000000 elastic-5.2.2.2/docs/source/_templates/layout.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6086 2024-04-15 23:43:43.000000 elastic-5.2.2.2/docs/source/cli-usage.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8465 2024-04-15 23:43:43.000000 elastic-5.2.2.2/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8304 2024-04-15 23:43:43.000000 elastic-5.2.2.2/docs/source/conf.py.tmpl
+-rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-04-15 23:43:43.000000 elastic-5.2.2.2/docs/source/endmatter.rst
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 23:43:43.000000 elastic-5.2.2.2/docs/source/examples.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 23:43:47.451111 elastic-5.2.2.2/docs/source/fig/
+-rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-04-15 23:43:43.000000 elastic-5.2.2.2/docs/source/fig/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-04-15 23:43:43.000000 elastic-5.2.2.2/docs/source/fig/favicon.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5145 2024-04-15 23:43:43.000000 elastic-5.2.2.2/docs/source/fig/favicon.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     7319 2024-04-15 23:43:43.000000 elastic-5.2.2.2/docs/source/fig/plot1.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)    17836 2024-04-15 23:43:43.000000 elastic-5.2.2.2/docs/source/fig/plot1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    24292 2024-04-15 23:43:43.000000 elastic-5.2.2.2/docs/source/fig/plot1.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     5703 2024-04-15 23:43:43.000000 elastic-5.2.2.2/docs/source/fig/plot2.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)    24303 2024-04-15 23:43:43.000000 elastic-5.2.2.2/docs/source/fig/plot2.png
+-rw-r--r--   0 runner    (1001) docker     (127)    18497 2024-04-15 23:43:43.000000 elastic-5.2.2.2/docs/source/fig/plot2.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     7407 2024-04-15 23:43:43.000000 elastic-5.2.2.2/docs/source/fig/plot3.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)    28926 2024-04-15 23:43:43.000000 elastic-5.2.2.2/docs/source/fig/plot3.png
+-rw-r--r--   0 runner    (1001) docker     (127)    27181 2024-04-15 23:43:43.000000 elastic-5.2.2.2/docs/source/fig/plot3.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     7757 2024-04-15 23:43:43.000000 elastic-5.2.2.2/docs/source/fig/plot3a.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)    34509 2024-04-15 23:43:43.000000 elastic-5.2.2.2/docs/source/fig/plot3a.png
+-rw-r--r--   0 runner    (1001) docker     (127)    36285 2024-04-15 23:43:43.000000 elastic-5.2.2.2/docs/source/fig/plot3a.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     7419 2024-04-15 23:43:43.000000 elastic-5.2.2.2/docs/source/fig/plot3b.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)    27897 2024-04-15 23:43:43.000000 elastic-5.2.2.2/docs/source/fig/plot3b.png
+-rw-r--r--   0 runner    (1001) docker     (127)    30417 2024-04-15 23:43:43.000000 elastic-5.2.2.2/docs/source/fig/plot3b.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-04-15 23:43:43.000000 elastic-5.2.2.2/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    15113 2024-04-15 23:43:43.000000 elastic-5.2.2.2/docs/source/intro.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9637 2024-04-15 23:43:43.000000 elastic-5.2.2.2/docs/source/lib-usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 23:43:47.455111 elastic-5.2.2.2/docs/source/lib-usage_files/
+-rw-r--r--   0 runner    (1001) docker     (127)    11186 2024-04-15 23:43:43.000000 elastic-5.2.2.2/docs/source/lib-usage_files/lib-usage_12_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    18112 2024-04-15 23:43:43.000000 elastic-5.2.2.2/docs/source/lib-usage_files/lib-usage_18_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4947 2024-04-15 23:43:43.000000 elastic-5.2.2.2/docs/source/lib-usage_files/lib-usage_9_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-15 23:43:43.000000 elastic-5.2.2.2/docs/source/modules.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 23:43:47.455111 elastic-5.2.2.2/elastic/
+-rw-r--r--   0 runner    (1001) docker     (127)     2639 2024-04-15 23:43:43.000000 elastic-5.2.2.2/elastic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-15 23:43:47.000000 elastic-5.2.2.2/elastic/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 23:43:47.455111 elastic-5.2.2.2/elastic/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 23:43:43.000000 elastic-5.2.2.2/elastic/cli/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5857 2024-04-15 23:43:43.000000 elastic-5.2.2.2/elastic/cli/elastic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26585 2024-04-15 23:43:43.000000 elastic-5.2.2.2/elastic/elastic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 23:43:47.467111 elastic-5.2.2.2/elastic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3448 2024-04-15 23:43:47.000000 elastic-5.2.2.2/elastic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2958 2024-04-15 23:43:47.000000 elastic-5.2.2.2/elastic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 23:43:47.000000 elastic-5.2.2.2/elastic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-15 23:43:47.000000 elastic-5.2.2.2/elastic.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-15 23:43:47.000000 elastic-5.2.2.2/elastic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-15 23:43:47.000000 elastic-5.2.2.2/elastic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 23:43:47.455111 elastic-5.2.2.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-04-15 23:43:43.000000 elastic-5.2.2.2/examples/example1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-04-15 23:43:43.000000 elastic-5.2.2.2/examples/example2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-04-15 23:43:43.000000 elastic-5.2.2.2/examples/example3.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 23:43:47.455111 elastic-5.2.2.2/examples/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      486 2024-04-15 23:43:43.000000 elastic-5.2.2.2/examples/scripts/check-job
+-rwxr-xr-x   0 runner    (1001) docker     (127)       48 2024-04-15 23:43:43.000000 elastic-5.2.2.2/examples/scripts/run-on-tsi
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2106 2024-04-15 23:43:43.000000 elastic-5.2.2.2/examples/scripts/run-vasp5-lock
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-15 23:43:43.000000 elastic-5.2.2.2/examples/scripts/run_vasp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-04-15 23:43:43.000000 elastic-5.2.2.2/paper.bib
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-15 23:43:43.000000 elastic-5.2.2.2/paper.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 23:43:47.455111 elastic-5.2.2.2/parcalc/
+-rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-04-15 23:43:43.000000 elastic-5.2.2.2/parcalc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25059 2024-04-15 23:43:43.000000 elastic-5.2.2.2/parcalc/parcalc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-04-15 23:43:43.000000 elastic-5.2.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 23:43:43.000000 elastic-5.2.2.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 23:43:47.467111 elastic-5.2.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-04-15 23:43:43.000000 elastic-5.2.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 23:43:47.455111 elastic-5.2.2.2/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     3526 2024-04-15 23:43:43.000000 elastic-5.2.2.2/test/test_elastic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 23:43:47.459111 elastic-5.2.2.2/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 23:43:47.463111 elastic-5.2.2.2/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-15 23:43:43.000000 elastic-5.2.2.2/tests/data/INCAR
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-15 23:43:43.000000 elastic-5.2.2.2/tests/data/KPOINTS
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-15 23:43:43.000000 elastic-5.2.2.2/tests/data/POSCAR
+-rw-r--r--   0 runner    (1001) docker     (127)   438201 2024-04-15 23:43:43.000000 elastic-5.2.2.2/tests/data/POTCAR
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-04-15 23:43:43.000000 elastic-5.2.2.2/tests/data/abinit
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 23:43:47.463111 elastic-5.2.2.2/tests/data/calc-cij_000/
+-rw-r--r--   0 runner    (1001) docker     (127)    44183 2024-04-15 23:43:43.000000 elastic-5.2.2.2/tests/data/calc-cij_000/vasprun.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 23:43:47.463111 elastic-5.2.2.2/tests/data/calc-cij_001/
+-rw-r--r--   0 runner    (1001) docker     (127)    46925 2024-04-15 23:43:43.000000 elastic-5.2.2.2/tests/data/calc-cij_001/vasprun.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 23:43:47.463111 elastic-5.2.2.2/tests/data/calc-cij_002/
+-rw-r--r--   0 runner    (1001) docker     (127)    46183 2024-04-15 23:43:43.000000 elastic-5.2.2.2/tests/data/calc-cij_002/vasprun.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 23:43:47.463111 elastic-5.2.2.2/tests/data/calc-cij_003/
+-rw-r--r--   0 runner    (1001) docker     (127)    44183 2024-04-15 23:43:43.000000 elastic-5.2.2.2/tests/data/calc-cij_003/vasprun.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 23:43:47.463111 elastic-5.2.2.2/tests/data/calc-cij_004/
+-rw-r--r--   0 runner    (1001) docker     (127)    46183 2024-04-15 23:43:43.000000 elastic-5.2.2.2/tests/data/calc-cij_004/vasprun.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 23:43:47.463111 elastic-5.2.2.2/tests/data/calc-cij_005/
+-rw-r--r--   0 runner    (1001) docker     (127)    46183 2024-04-15 23:43:43.000000 elastic-5.2.2.2/tests/data/calc-cij_005/vasprun.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 23:43:47.463111 elastic-5.2.2.2/tests/data/calc-cij_006/
+-rw-r--r--   0 runner    (1001) docker     (127)    48183 2024-04-15 23:43:43.000000 elastic-5.2.2.2/tests/data/calc-cij_006/vasprun.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 23:43:47.463111 elastic-5.2.2.2/tests/data/calc-cij_007/
+-rw-r--r--   0 runner    (1001) docker     (127)    50184 2024-04-15 23:43:43.000000 elastic-5.2.2.2/tests/data/calc-cij_007/vasprun.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 23:43:47.463111 elastic-5.2.2.2/tests/data/calc-cij_008/
+-rw-r--r--   0 runner    (1001) docker     (127)    50926 2024-04-15 23:43:43.000000 elastic-5.2.2.2/tests/data/calc-cij_008/vasprun.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 23:43:47.463111 elastic-5.2.2.2/tests/data/calc-cij_009/
+-rw-r--r--   0 runner    (1001) docker     (127)    50926 2024-04-15 23:43:43.000000 elastic-5.2.2.2/tests/data/calc-cij_009/vasprun.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 23:43:47.463111 elastic-5.2.2.2/tests/data/calc-cij_010/
+-rw-r--r--   0 runner    (1001) docker     (127)    50926 2024-04-15 23:43:43.000000 elastic-5.2.2.2/tests/data/calc-cij_010/vasprun.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 23:43:47.463111 elastic-5.2.2.2/tests/data/calc-eos_000/
+-rw-r--r--   0 runner    (1001) docker     (127)    44183 2024-04-15 23:43:43.000000 elastic-5.2.2.2/tests/data/calc-eos_000/vasprun.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 23:43:47.463111 elastic-5.2.2.2/tests/data/calc-eos_001/
+-rw-r--r--   0 runner    (1001) docker     (127)    44183 2024-04-15 23:43:43.000000 elastic-5.2.2.2/tests/data/calc-eos_001/vasprun.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 23:43:47.463111 elastic-5.2.2.2/tests/data/calc-eos_002/
+-rw-r--r--   0 runner    (1001) docker     (127)    44183 2024-04-15 23:43:43.000000 elastic-5.2.2.2/tests/data/calc-eos_002/vasprun.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 23:43:47.467111 elastic-5.2.2.2/tests/data/calc-eos_003/
+-rw-r--r--   0 runner    (1001) docker     (127)    44183 2024-04-15 23:43:43.000000 elastic-5.2.2.2/tests/data/calc-eos_003/vasprun.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 23:43:47.467111 elastic-5.2.2.2/tests/data/calc-eos_004/
+-rw-r--r--   0 runner    (1001) docker     (127)    44183 2024-04-15 23:43:43.000000 elastic-5.2.2.2/tests/data/calc-eos_004/vasprun.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 23:43:47.467111 elastic-5.2.2.2/tests/data/calc-eos_005/
+-rw-r--r--   0 runner    (1001) docker     (127)    44183 2024-04-15 23:43:43.000000 elastic-5.2.2.2/tests/data/calc-eos_005/vasprun.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-15 23:43:43.000000 elastic-5.2.2.2/tests/data/cij_000.POSCAR
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-15 23:43:43.000000 elastic-5.2.2.2/tests/data/cij_001.POSCAR
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-15 23:43:43.000000 elastic-5.2.2.2/tests/data/cij_002.POSCAR
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-15 23:43:43.000000 elastic-5.2.2.2/tests/data/cij_003.POSCAR
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-15 23:43:43.000000 elastic-5.2.2.2/tests/data/cij_004.POSCAR
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-15 23:43:43.000000 elastic-5.2.2.2/tests/data/cij_005.POSCAR
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-15 23:43:43.000000 elastic-5.2.2.2/tests/data/cij_006.POSCAR
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-15 23:43:43.000000 elastic-5.2.2.2/tests/data/cij_007.POSCAR
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-15 23:43:43.000000 elastic-5.2.2.2/tests/data/cij_008.POSCAR
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-15 23:43:43.000000 elastic-5.2.2.2/tests/data/cij_009.POSCAR
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-15 23:43:43.000000 elastic-5.2.2.2/tests/data/cij_010.POSCAR
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-15 23:43:43.000000 elastic-5.2.2.2/tests/data/eos_000.POSCAR
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-15 23:43:43.000000 elastic-5.2.2.2/tests/data/eos_001.POSCAR
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-15 23:43:43.000000 elastic-5.2.2.2/tests/data/eos_002.POSCAR
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-15 23:43:43.000000 elastic-5.2.2.2/tests/data/eos_003.POSCAR
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-15 23:43:43.000000 elastic-5.2.2.2/tests/data/eos_004.POSCAR
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-15 23:43:43.000000 elastic-5.2.2.2/tests/data/eos_005.POSCAR
+-rwxr-xr-x   0 runner    (1001) docker     (127)      319 2024-04-15 23:43:43.000000 elastic-5.2.2.2/tests/data/run-calcs
+-rwxr-xr-x   0 runner    (1001) docker     (127)      190 2024-04-15 23:43:43.000000 elastic-5.2.2.2/tests/runtest.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     7656 2024-04-15 23:43:43.000000 elastic-5.2.2.2/tests/test_01.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-04-15 23:43:43.000000 elastic-5.2.2.2/tests/test_02.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6441 2024-04-15 23:43:43.000000 elastic-5.2.2.2/tests/test_elastic.py
```

### Comparing `elastic-5.2.1.5/.github/workflows/pypi.yml` & `elastic-5.2.2.2/.github/workflows/pypi.yml`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 name: Build, test and publish to (test)PyPI
-on: [ push, pull_request ]
+on: [push, pull_request, release]
 
 jobs:
   build:
     name: Build distribution
     runs-on: ubuntu-latest
 
     steps:
```

### Comparing `elastic-5.2.1.5/LICENSE` & `elastic-5.2.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `elastic-5.2.1.5/PKG-INFO` & `elastic-5.2.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elastic
-Version: 5.2.1.5
+Version: 5.2.2.2
 Summary: Extension for ASE to calculate elastic constants
 Author-email: "Paweł T. Jochym" <Pawel.Jochym@ifj.edu.pl>, Georgios Tritsaris <gtritsaris@seas.harvard.edu>
 Maintainer-email: "Paweł T. Jochym" <Pawel.Jochym@ifj.edu.pl>
 License: GPLv3
 Project-URL: Homepage, https://wolf.ifj.edu.pl/elastic
 Project-URL: Documentation, http://elastic.rtfd.org/
 Project-URL: Repository, https://github.com/jochym/Elastic
```

### Comparing `elastic-5.2.1.5/README.md` & `elastic-5.2.2.2/README.md`

 * *Files identical despite different names*

### Comparing `elastic-5.2.1.5/conda/meta.yaml` & `elastic-5.2.2.2/conda/meta.yaml`

 * *Files identical despite different names*

### Comparing `elastic-5.2.1.5/docs/Makefile` & `elastic-5.2.2.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `elastic-5.2.1.5/docs/index.md` & `elastic-5.2.2.2/docs/index.md`

 * *Files identical despite different names*

### Comparing `elastic-5.2.1.5/docs/notebook/lib-usage.ipynb` & `elastic-5.2.2.2/docs/notebook/lib-usage.ipynb`

 * *Files identical despite different names*

### Comparing `elastic-5.2.1.5/docs/source/_static/favicon.ico` & `elastic-5.2.2.2/docs/source/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `elastic-5.2.1.5/docs/source/_templates/layout.html` & `elastic-5.2.2.2/docs/source/_templates/layout.html`

 * *Files identical despite different names*

### Comparing `elastic-5.2.1.5/docs/source/cli-usage.rst` & `elastic-5.2.2.2/docs/source/cli-usage.rst`

 * *Files identical despite different names*

### Comparing `elastic-5.2.1.5/docs/source/conf.py` & `elastic-5.2.2.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `elastic-5.2.1.5/docs/source/conf.py.tmpl` & `elastic-5.2.2.2/docs/source/conf.py.tmpl`

 * *Files identical despite different names*

### Comparing `elastic-5.2.1.5/docs/source/endmatter.rst` & `elastic-5.2.2.2/docs/source/endmatter.rst`

 * *Files identical despite different names*

### Comparing `elastic-5.2.1.5/docs/source/fig/favicon.ico` & `elastic-5.2.2.2/docs/source/fig/favicon.ico`

 * *Files identical despite different names*

### Comparing `elastic-5.2.1.5/docs/source/fig/favicon.png` & `elastic-5.2.2.2/docs/source/fig/favicon.png`

 * *Files identical despite different names*

### Comparing `elastic-5.2.1.5/docs/source/fig/favicon.svg` & `elastic-5.2.2.2/docs/source/fig/favicon.svg`

 * *Files identical despite different names*

### Comparing `elastic-5.2.1.5/docs/source/fig/plot1.pdf` & `elastic-5.2.2.2/docs/source/fig/plot1.pdf`

 * *Files identical despite different names*

### Comparing `elastic-5.2.1.5/docs/source/fig/plot1.png` & `elastic-5.2.2.2/docs/source/fig/plot1.png`

 * *Files identical despite different names*

### Comparing `elastic-5.2.1.5/docs/source/fig/plot1.svg` & `elastic-5.2.2.2/docs/source/fig/plot1.svg`

 * *Files identical despite different names*

### Comparing `elastic-5.2.1.5/docs/source/fig/plot2.pdf` & `elastic-5.2.2.2/docs/source/fig/plot2.pdf`

 * *Files identical despite different names*

### Comparing `elastic-5.2.1.5/docs/source/fig/plot2.png` & `elastic-5.2.2.2/docs/source/fig/plot2.png`

 * *Files identical despite different names*

### Comparing `elastic-5.2.1.5/docs/source/fig/plot2.svg` & `elastic-5.2.2.2/docs/source/fig/plot2.svg`

 * *Files identical despite different names*

### Comparing `elastic-5.2.1.5/docs/source/fig/plot3.pdf` & `elastic-5.2.2.2/docs/source/fig/plot3.pdf`

 * *Files identical despite different names*

### Comparing `elastic-5.2.1.5/docs/source/fig/plot3.png` & `elastic-5.2.2.2/docs/source/fig/plot3.png`

 * *Files identical despite different names*

### Comparing `elastic-5.2.1.5/docs/source/fig/plot3.svg` & `elastic-5.2.2.2/docs/source/fig/plot3.svg`

 * *Files identical despite different names*

### Comparing `elastic-5.2.1.5/docs/source/fig/plot3a.pdf` & `elastic-5.2.2.2/docs/source/fig/plot3a.pdf`

 * *Files identical despite different names*

### Comparing `elastic-5.2.1.5/docs/source/fig/plot3a.png` & `elastic-5.2.2.2/docs/source/fig/plot3a.png`

 * *Files identical despite different names*

### Comparing `elastic-5.2.1.5/docs/source/fig/plot3a.svg` & `elastic-5.2.2.2/docs/source/fig/plot3a.svg`

 * *Files identical despite different names*

### Comparing `elastic-5.2.1.5/docs/source/fig/plot3b.pdf` & `elastic-5.2.2.2/docs/source/fig/plot3b.pdf`

 * *Files identical despite different names*

### Comparing `elastic-5.2.1.5/docs/source/fig/plot3b.png` & `elastic-5.2.2.2/docs/source/fig/plot3b.png`

 * *Files identical despite different names*

### Comparing `elastic-5.2.1.5/docs/source/fig/plot3b.svg` & `elastic-5.2.2.2/docs/source/fig/plot3b.svg`

 * *Files identical despite different names*

### Comparing `elastic-5.2.1.5/docs/source/index.rst` & `elastic-5.2.2.2/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `elastic-5.2.1.5/docs/source/intro.rst` & `elastic-5.2.2.2/docs/source/intro.rst`

 * *Files identical despite different names*

### Comparing `elastic-5.2.1.5/docs/source/lib-usage.rst` & `elastic-5.2.2.2/docs/source/lib-usage.rst`

 * *Files identical despite different names*

### Comparing `elastic-5.2.1.5/docs/source/lib-usage_files/lib-usage_12_1.png` & `elastic-5.2.2.2/docs/source/lib-usage_files/lib-usage_12_1.png`

 * *Files identical despite different names*

### Comparing `elastic-5.2.1.5/docs/source/lib-usage_files/lib-usage_18_1.png` & `elastic-5.2.2.2/docs/source/lib-usage_files/lib-usage_18_1.png`

 * *Files identical despite different names*

### Comparing `elastic-5.2.1.5/docs/source/lib-usage_files/lib-usage_9_1.png` & `elastic-5.2.2.2/docs/source/lib-usage_files/lib-usage_9_1.png`

 * *Files identical despite different names*

### Comparing `elastic-5.2.1.5/docs/source/modules.rst` & `elastic-5.2.2.2/docs/source/modules.rst`

 * *Files identical despite different names*

### Comparing `elastic-5.2.1.5/elastic/__init__.py` & `elastic-5.2.2.2/elastic/__init__.py`

 * *Files identical despite different names*

### Comparing `elastic-5.2.1.5/elastic/cli/elastic.py` & `elastic-5.2.2.2/elastic/cli/elastic.py`

 * *Files identical despite different names*

### Comparing `elastic-5.2.1.5/elastic/elastic.py` & `elastic-5.2.2.2/elastic/elastic.py`

 * *Files identical despite different names*

### Comparing `elastic-5.2.1.5/elastic.egg-info/PKG-INFO` & `elastic-5.2.2.2/elastic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elastic
-Version: 5.2.1.5
+Version: 5.2.2.2
 Summary: Extension for ASE to calculate elastic constants
 Author-email: "Paweł T. Jochym" <Pawel.Jochym@ifj.edu.pl>, Georgios Tritsaris <gtritsaris@seas.harvard.edu>
 Maintainer-email: "Paweł T. Jochym" <Pawel.Jochym@ifj.edu.pl>
 License: GPLv3
 Project-URL: Homepage, https://wolf.ifj.edu.pl/elastic
 Project-URL: Documentation, http://elastic.rtfd.org/
 Project-URL: Repository, https://github.com/jochym/Elastic
```

### Comparing `elastic-5.2.1.5/elastic.egg-info/SOURCES.txt` & `elastic-5.2.2.2/elastic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `elastic-5.2.1.5/examples/example1.py` & `elastic-5.2.2.2/examples/example1.py`

 * *Files identical despite different names*

### Comparing `elastic-5.2.1.5/examples/example2.py` & `elastic-5.2.2.2/examples/example2.py`

 * *Files identical despite different names*

### Comparing `elastic-5.2.1.5/examples/example3.py` & `elastic-5.2.2.2/examples/example3.py`

 * *Files identical despite different names*

### Comparing `elastic-5.2.1.5/examples/scripts/run-vasp5-lock` & `elastic-5.2.2.2/examples/scripts/run-vasp5-lock`

 * *Files identical despite different names*

### Comparing `elastic-5.2.1.5/paper.bib` & `elastic-5.2.2.2/paper.bib`

 * *Files identical despite different names*

### Comparing `elastic-5.2.1.5/paper.md` & `elastic-5.2.2.2/paper.md`

 * *Files identical despite different names*

### Comparing `elastic-5.2.1.5/parcalc/__init__.py` & `elastic-5.2.2.2/parcalc/__init__.py`

 * *Files identical despite different names*

### Comparing `elastic-5.2.1.5/parcalc/parcalc.py` & `elastic-5.2.2.2/parcalc/parcalc.py`

 * *Files 3% similar despite different names*

```diff
@@ -202,16 +202,16 @@
             Vasp.set_results(self, atoms)
 
     def run(self):
         '''
         Blocking/Non-blocing run method.
         In blocking mode it just runs parent run method.
         In non-blocking mode it raises the __NonBlockingRunException
-        to bail out of the processing of standard calculate method 
-        (or any other method in fact) and signal that the data is not 
+        to bail out of the processing of standard calculate method
+        (or any other method in fact) and signal that the data is not
         ready to be collected.
         '''
         # This is only called from self.calculate - thus
         # we do not need to change to working_dir
         # since calculate already did
         Vasp.run(self)
         if not self.block :
@@ -298,28 +298,28 @@
         Aims.run(self)
 
 
 class RemoteCalculator(Calculator):
     '''
     Remote calculator based on ASE calculator class.
     This class is only involved with the machanics of remotly executing
-    the software and transporting the data. The calculation is 
+    the software and transporting the data. The calculation is
     delegated to the actual calculator class.
     '''
     
     # Queue system submit command
     qsub_tool='qsub'
     qstat_tool='qstat'
     
     qsub_cmd='cd %(rdir)s ; %(qsub_tool)s -N %(title)s -l procs=%(procs)d ./run-pw.pbs'
 
     # Remote execution command
     remote_exec_cmd='ssh %(user)s@%(host)s "%(command)s"'
 
-    # If you cannot mount the data directory into your system it is best 
+    # If you cannot mount the data directory into your system it is best
     # to use the rsync command to transfer the results back into the system.
 
     # Command for copying the data out to the computing system
     copy_out_cmd='rsync -a "%(ldir)s" "%(user)s@%(host)s:%(rdir)s"'
     # Command for copying the data in after the calculation
     copy_in_cmd='rsync -a "%(user)s@%(host)s:%(rdir)s" "%(ldir)s"'
 
@@ -354,15 +354,15 @@
         label: str
             Name used for all files.  May contain a directory.
         atoms: Atoms object
             Optional Atoms object to which the calculator will be
             attached.  When restarting, atoms will get its positions and
             unit-cell updated from file.
 
-        Create a remote execution calculator based on actual ASE calculator 
+        Create a remote execution calculator based on actual ASE calculator
         calc.
         '''
         logging.debug("Calc: %s Label: %s" % (calc, label))
         Calculator.__init__(self, restart, ignore_bad_restart_file, label, atoms, **kwargs)
         logging.debug("Dir: %s Ext: %s" % (self.directory, self.ext))
         self.calc=calc
         self.jobid=None
@@ -370,33 +370,43 @@
 
     def write_pbs_in(self,properties):
         with work_dir(self.directory):
             with open(os.path.join(self.directory,'run-ase-calc.pbs'),'w') as fh:
                 fh.write(self.pbs_template % {
                     'command': self.build_command(self,prop=properties,
                                                     params=self.parameters)
-                    })        
+                    })
 
-    def build_command(self,prop=['energy'],params={}):
+    def build_command(self, prop=None, params=None):
+        '''
+        Build command strings for local or remote execution
+        '''
+        if prop is None :
+            prop = ['energy']
+        if params is None :
+            params = {}
         cmd=self.qsub_cmd % {
-            'qsub_tool': self.qsub_tool,
-            'qstat_tool': self.qstat_tool,
-            'title': self.label,
-            'procs': self.parameters['procs'],
-            'rdir': os.path.join(self.parameters['rdir'],os.path.split(self.directory)[-1])
-        }
+                'qsub_tool': self.qsub_tool,
+                'qstat_tool': self.qstat_tool,
+                'title': self.label,
+                'procs': self.parameters['procs'],
+                'rdir': os.path.join(self.parameters['rdir'],
+                                     os.path.split(self.directory)[-1])
+            }
         cmd=self.remote_exec_cmd % {
                 'command': cmd,
                 'user': self.parameters['user'],
                 'host': self.parameters['host']
-         }
+            }
         return cmd
 
-    def write_input(self, atoms=None, properties=['energy'], system_changes=all_changes):
+    def write_input(self, atoms=None, properties=None, system_changes=all_changes):
         '''Write input file(s).'''
+        if properties is None :
+            properties = ['energy']
         with work_dir(self.directory):
             self.calc.write_input(self, atoms, properties, system_changes)
             self.write_pbs_in(properties)
             subprocess.call(self.copy_out_cmd % {
                                 'ldir': self.directory,
                                 'rdir': self.parameters['rdir'],
                                 'user': self.parameters['user'],
@@ -418,25 +428,27 @@
         except (subprocess.CalledProcessError, IndexError) :
             # Unknown state. We assume it has finished and continue
             state='N'
 
         return not (state in ['Q','R'])
 
 
-    def run_calculation(self, atoms=None, properties=['energy'],
+    def run_calculation(self, atoms=None, properties=None,
                             system_changes=all_changes):
         '''
         Internal calculation executor. We cannot use FileIOCalculator
         directly since we need to support remote execution.
         
-        This calculator is different from others. 
+        This calculator is different from others.
         It prepares the directory, launches the remote process and
         raises the exception to signal that we need to come back for results
         when the job is finished.
         '''
+        if properties is None :
+            properties = ['energy']
         self.calc.calculate(self, atoms, properties, system_changes)
         self.write_input(self.atoms, properties, system_changes)
         if self.command is None:
             raise RuntimeError('Please configure Remote calculator!')
         olddir = os.getcwd()
         errorcode=0
         try:
@@ -477,40 +489,42 @@
                 'user': self.parameters['user'],
                 'host': self.parameters['host']
             }, shell=True)
                 
         
         fn=os.path.join(self.directory,'pw.out')
         # Read the pan-ultimate line of the output file
-        try: 
+        try:
             ln=open(fn).readlines()[-2]
             if ln.find('JOB DONE.')>-1 :
                 # Job is done we can read the output
                 r=read_quantumespresso_textoutput(fn)
                 self.submited=False
                 self.jobid=None
             else :
                 # Job not ready.
                 raise CalcNotReadyError
         except (IOError, IndexError) :
             # Job not ready.
             raise CalcNotReadyError
-        
+
         # All is fine - really read the results
         self.calc.read_results(self)
 
     @classmethod
-    def ParallelCalculate(cls,syslst,properties=['energy'],system_changes=all_changes):
+    def ParallelCalculate(cls,syslst,properties=None,system_changes=all_changes):
         '''
-        Run a series of calculations in parallel using (implicitely) some 
+        Run a series of calculations in parallel using (implicitely) some
         remote machine/cluster. The function returns the list of systems ready
         for the extraction of calculated properties.
         '''
         print('Launching:',end=' ')
         sys.stdout.flush()
+        if properties is None :
+            properties = ['energy']
         for n,s in enumerate(syslst):
             try :
                 s.calc.block=False
                 s.calc.calculate(atoms=s,properties=properties,system_changes=system_changes)
             except CalcNotReadyError:
                 s.calc.block=True
             print(n+1, end=' ')
@@ -578,18 +592,18 @@
 def ParCalculate(systems,calc,cleanup=True,block=True,prefix="Calc_"):
     '''
     Run calculators in parallel for all systems.
     Calculators are executed in isolated processes and directories.
     The resulting objects are returned in the list (one per input system).
     '''
 
-    if type(systems) != type([]) :
-        sysl=[systems]
+    if isinstance(systems, list) :
+        sysl = systems
     else :
-        sysl=systems
+        sysl = [systems]
 
     if block :
         iq=Queue(len(sysl)+1)
         oq=Queue(len(sysl)+1)
 
         # Create workers
         for s in sysl:
```

### Comparing `elastic-5.2.1.5/pyproject.toml` & `elastic-5.2.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `elastic-5.2.1.5/test/test_elastic.py` & `elastic-5.2.2.2/test/test_elastic.py`

 * *Files identical despite different names*

### Comparing `elastic-5.2.1.5/tests/data/POSCAR` & `elastic-5.2.2.2/tests/data/POSCAR`

 * *Files identical despite different names*

### Comparing `elastic-5.2.1.5/tests/data/POTCAR` & `elastic-5.2.2.2/tests/data/POTCAR`

 * *Files identical despite different names*

### Comparing `elastic-5.2.1.5/tests/data/abinit` & `elastic-5.2.2.2/tests/data/abinit`

 * *Files identical despite different names*

### Comparing `elastic-5.2.1.5/tests/data/calc-cij_000/vasprun.xml` & `elastic-5.2.2.2/tests/data/calc-cij_000/vasprun.xml`

 * *Files identical despite different names*

### Comparing `elastic-5.2.1.5/tests/data/calc-cij_001/vasprun.xml` & `elastic-5.2.2.2/tests/data/calc-cij_001/vasprun.xml`

 * *Files identical despite different names*

### Comparing `elastic-5.2.1.5/tests/data/calc-cij_002/vasprun.xml` & `elastic-5.2.2.2/tests/data/calc-cij_002/vasprun.xml`

 * *Files identical despite different names*

### Comparing `elastic-5.2.1.5/tests/data/calc-cij_003/vasprun.xml` & `elastic-5.2.2.2/tests/data/calc-cij_003/vasprun.xml`

 * *Files identical despite different names*

### Comparing `elastic-5.2.1.5/tests/data/calc-cij_004/vasprun.xml` & `elastic-5.2.2.2/tests/data/calc-cij_004/vasprun.xml`

 * *Files identical despite different names*

### Comparing `elastic-5.2.1.5/tests/data/calc-cij_005/vasprun.xml` & `elastic-5.2.2.2/tests/data/calc-cij_005/vasprun.xml`

 * *Files identical despite different names*

### Comparing `elastic-5.2.1.5/tests/data/calc-cij_006/vasprun.xml` & `elastic-5.2.2.2/tests/data/calc-cij_006/vasprun.xml`

 * *Files identical despite different names*

### Comparing `elastic-5.2.1.5/tests/data/calc-cij_007/vasprun.xml` & `elastic-5.2.2.2/tests/data/calc-cij_007/vasprun.xml`

 * *Files identical despite different names*

### Comparing `elastic-5.2.1.5/tests/data/calc-cij_008/vasprun.xml` & `elastic-5.2.2.2/tests/data/calc-cij_008/vasprun.xml`

 * *Files identical despite different names*

### Comparing `elastic-5.2.1.5/tests/data/calc-cij_009/vasprun.xml` & `elastic-5.2.2.2/tests/data/calc-cij_009/vasprun.xml`

 * *Files identical despite different names*

### Comparing `elastic-5.2.1.5/tests/data/calc-cij_010/vasprun.xml` & `elastic-5.2.2.2/tests/data/calc-cij_010/vasprun.xml`

 * *Files identical despite different names*

### Comparing `elastic-5.2.1.5/tests/data/calc-eos_000/vasprun.xml` & `elastic-5.2.2.2/tests/data/calc-eos_000/vasprun.xml`

 * *Files identical despite different names*

### Comparing `elastic-5.2.1.5/tests/data/calc-eos_001/vasprun.xml` & `elastic-5.2.2.2/tests/data/calc-eos_001/vasprun.xml`

 * *Files identical despite different names*

### Comparing `elastic-5.2.1.5/tests/data/calc-eos_002/vasprun.xml` & `elastic-5.2.2.2/tests/data/calc-eos_002/vasprun.xml`

 * *Files identical despite different names*

### Comparing `elastic-5.2.1.5/tests/data/calc-eos_003/vasprun.xml` & `elastic-5.2.2.2/tests/data/calc-eos_003/vasprun.xml`

 * *Files identical despite different names*

### Comparing `elastic-5.2.1.5/tests/data/calc-eos_004/vasprun.xml` & `elastic-5.2.2.2/tests/data/calc-eos_004/vasprun.xml`

 * *Files identical despite different names*

### Comparing `elastic-5.2.1.5/tests/data/calc-eos_005/vasprun.xml` & `elastic-5.2.2.2/tests/data/calc-eos_005/vasprun.xml`

 * *Files identical despite different names*

### Comparing `elastic-5.2.1.5/tests/data/cij_000.POSCAR` & `elastic-5.2.2.2/tests/data/cij_000.POSCAR`

 * *Files identical despite different names*

### Comparing `elastic-5.2.1.5/tests/data/cij_001.POSCAR` & `elastic-5.2.2.2/tests/data/cij_001.POSCAR`

 * *Files identical despite different names*

### Comparing `elastic-5.2.1.5/tests/data/cij_002.POSCAR` & `elastic-5.2.2.2/tests/data/cij_002.POSCAR`

 * *Files identical despite different names*

### Comparing `elastic-5.2.1.5/tests/data/cij_003.POSCAR` & `elastic-5.2.2.2/tests/data/cij_003.POSCAR`

 * *Files identical despite different names*

### Comparing `elastic-5.2.1.5/tests/data/cij_004.POSCAR` & `elastic-5.2.2.2/tests/data/cij_004.POSCAR`

 * *Files identical despite different names*

### Comparing `elastic-5.2.1.5/tests/data/cij_005.POSCAR` & `elastic-5.2.2.2/tests/data/cij_005.POSCAR`

 * *Files identical despite different names*

### Comparing `elastic-5.2.1.5/tests/data/cij_006.POSCAR` & `elastic-5.2.2.2/tests/data/cij_006.POSCAR`

 * *Files identical despite different names*

### Comparing `elastic-5.2.1.5/tests/data/cij_007.POSCAR` & `elastic-5.2.2.2/tests/data/cij_007.POSCAR`

 * *Files identical despite different names*

### Comparing `elastic-5.2.1.5/tests/data/cij_008.POSCAR` & `elastic-5.2.2.2/tests/data/cij_008.POSCAR`

 * *Files identical despite different names*

### Comparing `elastic-5.2.1.5/tests/data/cij_009.POSCAR` & `elastic-5.2.2.2/tests/data/cij_009.POSCAR`

 * *Files identical despite different names*

### Comparing `elastic-5.2.1.5/tests/data/cij_010.POSCAR` & `elastic-5.2.2.2/tests/data/cij_010.POSCAR`

 * *Files identical despite different names*

### Comparing `elastic-5.2.1.5/tests/data/eos_000.POSCAR` & `elastic-5.2.2.2/tests/data/eos_000.POSCAR`

 * *Files identical despite different names*

### Comparing `elastic-5.2.1.5/tests/data/eos_001.POSCAR` & `elastic-5.2.2.2/tests/data/eos_001.POSCAR`

 * *Files identical despite different names*

### Comparing `elastic-5.2.1.5/tests/data/eos_002.POSCAR` & `elastic-5.2.2.2/tests/data/eos_002.POSCAR`

 * *Files identical despite different names*

### Comparing `elastic-5.2.1.5/tests/data/eos_003.POSCAR` & `elastic-5.2.2.2/tests/data/eos_003.POSCAR`

 * *Files identical despite different names*

### Comparing `elastic-5.2.1.5/tests/data/eos_004.POSCAR` & `elastic-5.2.2.2/tests/data/eos_004.POSCAR`

 * *Files identical despite different names*

### Comparing `elastic-5.2.1.5/tests/data/eos_005.POSCAR` & `elastic-5.2.2.2/tests/data/eos_005.POSCAR`

 * *Files identical despite different names*

### Comparing `elastic-5.2.1.5/tests/test_01.py` & `elastic-5.2.2.2/tests/test_01.py`

 * *Files identical despite different names*

### Comparing `elastic-5.2.1.5/tests/test_02.py` & `elastic-5.2.2.2/tests/test_02.py`

 * *Files identical despite different names*

### Comparing `elastic-5.2.1.5/tests/test_elastic.py` & `elastic-5.2.2.2/tests/test_elastic.py`

 * *Files identical despite different names*

