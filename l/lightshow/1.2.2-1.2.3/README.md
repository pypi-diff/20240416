# Comparing `tmp/lightshow-1.2.2.tar.gz` & `tmp/lightshow-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightshow-1.2.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "lightshow-1.2.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `lightshow-1.2.2.tar` & `lightshow-1.2.3.tar`

### file list

```diff
@@ -1,95 +1,98 @@
--rw-r--r--   0        0        0      135 2024-03-02 03:08:16.307608 lightshow-1.2.2/.coveragerc
--rw-r--r--   0        0        0      221 2024-03-02 03:08:16.307608 lightshow-1.2.2/.flake8
--rw-r--r--   0        0        0       58 2024-03-02 03:08:16.307608 lightshow-1.2.2/.gitattributes
--rw-r--r--   0        0        0      198 2024-03-02 03:08:16.307608 lightshow-1.2.2/.github/dependabot.yml
--rw-r--r--   0        0        0     5118 2024-03-02 03:08:16.307608 lightshow-1.2.2/.github/workflows/ci.yml
--rw-r--r--   0        0        0     2128 2024-03-02 03:08:16.307608 lightshow-1.2.2/.gitignore
--rw-r--r--   0        0        0      336 2024-03-02 03:08:16.307608 lightshow-1.2.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1099 2024-03-02 03:08:16.307608 lightshow-1.2.2/AUTHORS.rst
--rw-r--r--   0        0        0     1065 2024-03-02 03:08:16.307608 lightshow-1.2.2/CHANGES.md
--rw-r--r--   0        0        0     1118 2024-03-02 03:08:16.307608 lightshow-1.2.2/CONTRIBUTING.md
--rw-r--r--   0        0        0     1574 2024-03-02 03:08:16.307608 lightshow-1.2.2/LICENSE
--rw-r--r--   0        0        0     7392 2024-03-02 03:08:16.307608 lightshow-1.2.2/README.md
--rw-r--r--   0        0        0      673 2024-03-02 03:08:16.307608 lightshow-1.2.2/docs/Makefile
--rw-r--r--   0        0        0    60563 2024-03-02 03:08:16.307608 lightshow-1.2.2/docs/_static/images/lightshow.jpg
--rw-r--r--   0        0        0   118686 2024-03-02 03:08:16.307608 lightshow-1.2.2/docs/_static/images/lightshow_old.jpg
--rw-r--r--   0        0        0      797 2024-03-02 03:08:16.307608 lightshow-1.2.2/docs/make.bat
--rw-r--r--   0        0        0        0 2024-03-02 03:08:16.307608 lightshow-1.2.2/docs/source/_static/.placeholder
--rw-r--r--   0        0        0     6725 2024-03-02 03:08:16.307608 lightshow-1.2.2/docs/source/conf.py
--rw-r--r--   0        0        0     2023 2024-03-02 03:08:16.307608 lightshow-1.2.2/docs/source/index.rst
--rw-r--r--   0        0        0     1181 2024-03-02 03:08:16.307608 lightshow-1.2.2/docs/source/installation.rst
--rw-r--r--   0        0        0     1053 2024-03-02 03:08:16.307608 lightshow-1.2.2/docs/source/lightshow.parameters.rst
--rw-r--r--   0        0        0      559 2024-03-02 03:08:16.307608 lightshow-1.2.2/docs/source/lightshow.rst
--rw-r--r--   0        0        0       86 2024-03-02 03:08:16.307608 lightshow-1.2.2/docs/source/modules.rst
--rw-r--r--   0        0        0      337 2024-03-02 03:08:16.307608 lightshow-1.2.2/docs/source/project.rst
--rw-r--r--   0        0        0       34 2024-03-02 03:08:16.307608 lightshow-1.2.2/docs/source/project/authors.rst
--rw-r--r--   0        0        0     1720 2024-03-02 03:08:16.307608 lightshow-1.2.2/docs/source/project/funding.rst
--rw-r--r--   0        0        0       47 2024-03-02 03:08:16.307608 lightshow-1.2.2/docs/source/project/license.rst
--rw-r--r--   0        0        0    20734 2024-03-02 03:08:16.307608 lightshow-1.2.2/docs/source/quickstart.rst
--rw-r--r--   0        0        0    92531 2024-03-02 03:08:16.311608 lightshow-1.2.2/figures/Lightshow_Workflow_Diagram.jpg
--rw-r--r--   0        0        0    25190 2024-03-02 03:08:16.311608 lightshow-1.2.2/figures/Lightshow_Workflow_Diagram.pdf
--rw-r--r--   0        0        0     1941 2024-03-02 03:08:19.611597 lightshow-1.2.2/lightshow/__init__.py
--rw-r--r--   0        0        0        0 2024-03-02 03:08:16.311608 lightshow-1.2.2/lightshow/_tests/__init__.py
--rw-r--r--   0        0        0     2821 2024-03-02 03:08:16.311608 lightshow-1.2.2/lightshow/_tests/conftest.py
--rw-r--r--   0        0        0       40 2024-03-02 03:08:16.311608 lightshow-1.2.2/lightshow/_tests/dummy_chpsp_files/Core_O.wfc
--rw-r--r--   0        0        0       42 2024-03-02 03:08:16.311608 lightshow-1.2.2/lightshow/_tests/dummy_chpsp_files/Core_Ti.wfc
--rw-r--r--   0        0        0       34 2024-03-02 03:08:16.311608 lightshow-1.2.2/lightshow/_tests/dummy_chpsp_files/O.fch.upf
--rw-r--r--   0        0        0       35 2024-03-02 03:08:16.311608 lightshow-1.2.2/lightshow/_tests/dummy_chpsp_files/Ti.fch.upf
--rw-r--r--   0        0        0      476 2024-03-02 03:08:16.311608 lightshow-1.2.2/lightshow/_tests/dummy_potcar_files/O_GW/POTCAR
--rw-r--r--   0        0        0      480 2024-03-02 03:08:16.311608 lightshow-1.2.2/lightshow/_tests/dummy_potcar_files/Ti_sv_GW/POTCAR
--rw-r--r--   0        0        0       24 2024-03-02 03:08:16.311608 lightshow-1.2.2/lightshow/_tests/dummy_psp_files/O.mock.upf
--rw-r--r--   0        0        0       25 2024-03-02 03:08:16.311608 lightshow-1.2.2/lightshow/_tests/dummy_psp_files/Ti.mock.upf
--rw-r--r--   0        0        0      152 2024-03-02 03:08:16.311608 lightshow-1.2.2/lightshow/_tests/dummy_psp_files/mock_cutoff_table.json
--rw-r--r--   0        0        0        0 2024-03-02 03:08:16.311608 lightshow-1.2.2/lightshow/_tests/helpers/__init__.py
--rw-r--r--   0        0        0    13328 2024-03-02 03:08:16.311608 lightshow-1.2.2/lightshow/_tests/helpers/geometry.py
--rw-r--r--   0        0        0       82 2024-03-02 03:08:16.311608 lightshow-1.2.2/lightshow/_tests/sample_files/README.rst
--rw-r--r--   0        0        0    42630 2024-03-02 03:08:16.311608 lightshow-1.2.2/lightshow/_tests/sample_files/ene_dep_broad.txt
--rw-r--r--   0        0        0    43441 2024-03-02 03:08:16.311608 lightshow-1.2.2/lightshow/_tests/sample_files/gauss_broad.txt
--rw-r--r--   0        0        0    43519 2024-03-02 03:08:16.311608 lightshow-1.2.2/lightshow/_tests/sample_files/lorentz_broad.txt
--rw-r--r--   0        0        0    43398 2024-03-02 03:08:16.311608 lightshow-1.2.2/lightshow/_tests/sample_files/voigt_broad.txt
--rw-r--r--   0        0        0      376 2024-03-02 03:08:16.311608 lightshow-1.2.2/lightshow/_tests/structure_files/mp-10734/POSCAR
--rw-r--r--   0        0        0      198 2024-03-02 03:08:16.311608 lightshow-1.2.2/lightshow/_tests/structure_files/mp-1215/POSCAR
--rw-r--r--   0        0        0      814 2024-03-02 03:08:16.311608 lightshow-1.2.2/lightshow/_tests/structure_files/mp-1840/POSCAR
--rw-r--r--   0        0        0      284 2024-03-02 03:08:16.311608 lightshow-1.2.2/lightshow/_tests/structure_files/mp-2657/POSCAR
--rw-r--r--   0        0        0      167 2024-03-02 03:08:16.311608 lightshow-1.2.2/lightshow/_tests/structure_files/mp-2664/POSCAR
--rw-r--r--   0        0        0      287 2024-03-02 03:08:16.311608 lightshow-1.2.2/lightshow/_tests/structure_files/mp-390/POSCAR
--rw-r--r--   0        0        0      460 2024-03-02 03:08:16.311608 lightshow-1.2.2/lightshow/_tests/structure_files/mp-430/POSCAR
--rw-r--r--   0        0        0      403 2024-03-02 03:08:16.311608 lightshow-1.2.2/lightshow/_tests/structure_files/mp-458/POSCAR
--rw-r--r--   0        0        0     1702 2024-03-02 03:08:16.311608 lightshow-1.2.2/lightshow/_tests/test_broaden.py
--rw-r--r--   0        0        0     3798 2024-03-02 03:08:16.311608 lightshow-1.2.2/lightshow/_tests/test_database.py
--rw-r--r--   0        0        0    12398 2024-03-02 03:08:16.311608 lightshow-1.2.2/lightshow/_tests/test_exciting.py
--rw-r--r--   0        0        0     1352 2024-03-02 03:08:16.311608 lightshow-1.2.2/lightshow/_tests/test_metadata.py
--rw-r--r--   0        0        0        0 2024-03-02 03:08:16.311608 lightshow-1.2.2/lightshow/common/__init__.py
--rw-r--r--   0        0        0     2580 2024-03-02 03:08:16.311608 lightshow-1.2.2/lightshow/common/kpoints.py
--rw-r--r--   0        0        0     3322 2024-03-02 03:08:16.311608 lightshow-1.2.2/lightshow/common/nbands.py
--rw-r--r--   0        0        0    18842 2024-03-02 03:08:16.311608 lightshow-1.2.2/lightshow/database.py
--rw-r--r--   0        0        0      602 2024-03-02 03:08:16.311608 lightshow-1.2.2/lightshow/defaults.py
--rw-r--r--   0        0        0        0 2024-03-02 03:08:16.311608 lightshow-1.2.2/lightshow/parameters/__init__.py
--rw-r--r--   0        0        0      206 2024-03-02 03:08:16.311608 lightshow-1.2.2/lightshow/parameters/_base.py
--rw-r--r--   0        0        0     9115 2024-03-02 03:08:16.311608 lightshow-1.2.2/lightshow/parameters/exciting.py
--rw-r--r--   0        0        0     8143 2024-03-02 03:08:16.311608 lightshow-1.2.2/lightshow/parameters/feff.py
--rw-r--r--   0        0        0    14284 2024-03-02 03:08:16.311608 lightshow-1.2.2/lightshow/parameters/ocean.py
--rw-r--r--   0        0        0    29454 2024-03-02 03:08:16.311608 lightshow-1.2.2/lightshow/parameters/vasp.py
--rw-r--r--   0        0        0    19946 2024-03-02 03:08:16.311608 lightshow-1.2.2/lightshow/parameters/xspectra.py
--rw-r--r--   0        0        0        0 2024-03-02 03:08:16.311608 lightshow-1.2.2/lightshow/postprocess/__init__.py
--rw-r--r--   0        0        0     9023 2024-03-02 03:08:16.311608 lightshow-1.2.2/lightshow/postprocess/broaden.py
--rw-r--r--   0        0        0     7584 2024-03-02 03:08:16.311608 lightshow-1.2.2/lightshow/postprocess/compare_utils.py
--rw-r--r--   0        0        0    12888 2024-03-02 03:08:16.311608 lightshow-1.2.2/lightshow/postprocess/parse.py
--rw-r--r--   0        0        0     4935 2024-03-02 03:08:16.311608 lightshow-1.2.2/lightshow/pymatgen_utils.py
--rw-r--r--   0        0        0    32826 2024-03-02 03:08:16.315608 lightshow-1.2.2/notebooks/00_basic_usage.ipynb
--rw-r--r--   0        0        0    10037 2024-03-02 03:08:16.315608 lightshow-1.2.2/notebooks/01_Ti_K_anatase_broaden.ipynb
--rw-r--r--   0        0        0     5829 2024-03-02 03:08:16.315608 lightshow-1.2.2/notebooks/compare_spectra.ipynb
--rw-r--r--   0        0        0     7248 2024-03-02 03:08:16.315608 lightshow-1.2.2/notebooks/parse_spectra.ipynb
--rwxr-xr-x   0        0        0    41029 2024-03-02 03:08:16.315608 lightshow-1.2.2/notebooks/spectra_files/anatase_exciting.txt
--rw-r--r--   0        0        0     3816 2024-03-02 03:08:16.315608 lightshow-1.2.2/notebooks/spectra_files/anatase_exp.txt
--rw-r--r--   0        0        0    54210 2024-03-02 03:08:16.315608 lightshow-1.2.2/notebooks/spectra_files/anatase_ocean.txt
--rw-r--r--   0        0        0     5000 2024-03-02 03:08:16.315608 lightshow-1.2.2/notebooks/spectra_files/anatase_theory_FEFF.txt
--rw-r--r--   0        0        0  2000000 2024-03-02 03:08:16.319608 lightshow-1.2.2/notebooks/spectra_files/anatase_theory_VASP.txt
--rwxr-xr-x   0        0        0    11578 2024-03-02 03:08:16.319608 lightshow-1.2.2/notebooks/spectra_files/anatase_xspectra.txt
--rw-r--r--   0        0        0     1972 2024-03-02 03:08:16.319608 lightshow-1.2.2/pyproject.toml
--rw-r--r--   0        0        0     1204 2024-03-02 03:08:16.319608 lightshow-1.2.2/scripts/README.rst
--rw-r--r--   0        0        0      575 2024-03-02 03:08:16.319608 lightshow-1.2.2/scripts/build_docs.sh
--rw-r--r--   0        0        0      118 2024-03-02 03:08:16.323608 lightshow-1.2.2/scripts/build_project.sh
--rw-r--r--   0        0        0      943 2024-03-02 03:08:16.323608 lightshow-1.2.2/scripts/install.sh
--rw-r--r--   0        0        0     1076 2024-03-02 03:08:16.323608 lightshow-1.2.2/scripts/update_version.sh
--rw-r--r--   0        0        0     9008 1970-01-01 00:00:00.000000 lightshow-1.2.2/PKG-INFO
+-rw-r--r--   0        0        0      135 2024-04-16 14:43:45.136438 lightshow-1.2.3/.coveragerc
+-rw-r--r--   0        0        0      248 2024-04-16 14:43:45.136438 lightshow-1.2.3/.flake8
+-rw-r--r--   0        0        0       58 2024-04-16 14:43:45.136438 lightshow-1.2.3/.gitattributes
+-rw-r--r--   0        0        0      198 2024-04-16 14:43:45.136438 lightshow-1.2.3/.github/dependabot.yml
+-rw-r--r--   0        0        0     4662 2024-04-16 14:43:45.136438 lightshow-1.2.3/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     2147 2024-04-16 14:43:45.136438 lightshow-1.2.3/.gitignore
+-rw-r--r--   0        0        0      484 2024-04-16 14:43:45.136438 lightshow-1.2.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      885 2024-04-16 14:43:45.136438 lightshow-1.2.3/AUTHORS.md
+-rw-r--r--   0        0        0     1239 2024-04-16 14:43:45.136438 lightshow-1.2.3/CHANGES.md
+-rw-r--r--   0        0        0     1118 2024-04-16 14:43:45.136438 lightshow-1.2.3/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1574 2024-04-16 14:43:45.136438 lightshow-1.2.3/LICENSE
+-rw-r--r--   0        0        0     7436 2024-04-16 14:43:45.136438 lightshow-1.2.3/README.md
+-rw-r--r--   0        0        0      673 2024-04-16 14:43:45.136438 lightshow-1.2.3/docs/Makefile
+-rw-r--r--   0        0        0    60563 2024-04-16 14:43:45.136438 lightshow-1.2.3/docs/_static/images/lightshow.jpg
+-rw-r--r--   0        0        0   118686 2024-04-16 14:43:45.136438 lightshow-1.2.3/docs/_static/images/lightshow_old.jpg
+-rw-r--r--   0        0        0      797 2024-04-16 14:43:45.136438 lightshow-1.2.3/docs/make.bat
+-rw-r--r--   0        0        0        0 2024-04-16 14:43:45.136438 lightshow-1.2.3/docs/source/_static/.placeholder
+-rw-r--r--   0        0        0     6725 2024-04-16 14:43:45.136438 lightshow-1.2.3/docs/source/conf.py
+-rw-r--r--   0        0        0     2023 2024-04-16 14:43:45.136438 lightshow-1.2.3/docs/source/index.rst
+-rw-r--r--   0        0        0     1181 2024-04-16 14:43:45.136438 lightshow-1.2.3/docs/source/installation.rst
+-rw-r--r--   0        0        0     1053 2024-04-16 14:43:45.136438 lightshow-1.2.3/docs/source/lightshow.parameters.rst
+-rw-r--r--   0        0        0      559 2024-04-16 14:43:45.136438 lightshow-1.2.3/docs/source/lightshow.rst
+-rw-r--r--   0        0        0       86 2024-04-16 14:43:45.136438 lightshow-1.2.3/docs/source/modules.rst
+-rw-r--r--   0        0        0      337 2024-04-16 14:43:45.136438 lightshow-1.2.3/docs/source/project.rst
+-rw-r--r--   0        0        0       35 2024-04-16 14:43:45.136438 lightshow-1.2.3/docs/source/project/authors.rst
+-rw-r--r--   0        0        0     1720 2024-04-16 14:43:45.136438 lightshow-1.2.3/docs/source/project/funding.rst
+-rw-r--r--   0        0        0       47 2024-04-16 14:43:45.136438 lightshow-1.2.3/docs/source/project/license.rst
+-rw-r--r--   0        0        0    20734 2024-04-16 14:43:45.136438 lightshow-1.2.3/docs/source/quickstart.rst
+-rw-r--r--   0        0        0    92531 2024-04-16 14:43:45.136438 lightshow-1.2.3/figures/Lightshow_Workflow_Diagram.jpg
+-rw-r--r--   0        0        0    25190 2024-04-16 14:43:45.136438 lightshow-1.2.3/figures/Lightshow_Workflow_Diagram.pdf
+-rw-r--r--   0        0        0      535 2024-04-16 14:43:45.136438 lightshow-1.2.3/lightshow/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:43:45.136438 lightshow-1.2.3/lightshow/_tests/__init__.py
+-rw-r--r--   0        0        0     2820 2024-04-16 14:43:45.136438 lightshow-1.2.3/lightshow/_tests/conftest.py
+-rw-r--r--   0        0        0       40 2024-04-16 14:43:45.136438 lightshow-1.2.3/lightshow/_tests/dummy_chpsp_files/Core_O.wfc
+-rw-r--r--   0        0        0       42 2024-04-16 14:43:45.136438 lightshow-1.2.3/lightshow/_tests/dummy_chpsp_files/Core_Ti.wfc
+-rw-r--r--   0        0        0       34 2024-04-16 14:43:45.136438 lightshow-1.2.3/lightshow/_tests/dummy_chpsp_files/O.fch.upf
+-rw-r--r--   0        0        0       35 2024-04-16 14:43:45.136438 lightshow-1.2.3/lightshow/_tests/dummy_chpsp_files/Ti.fch.upf
+-rw-r--r--   0        0        0      476 2024-04-16 14:43:45.136438 lightshow-1.2.3/lightshow/_tests/dummy_potcar_files/O_GW/POTCAR
+-rw-r--r--   0        0        0      480 2024-04-16 14:43:45.140438 lightshow-1.2.3/lightshow/_tests/dummy_potcar_files/Ti_sv_GW/POTCAR
+-rw-r--r--   0        0        0       24 2024-04-16 14:43:45.140438 lightshow-1.2.3/lightshow/_tests/dummy_psp_files/O.mock.upf
+-rw-r--r--   0        0        0       25 2024-04-16 14:43:45.140438 lightshow-1.2.3/lightshow/_tests/dummy_psp_files/Ti.mock.upf
+-rw-r--r--   0        0        0      152 2024-04-16 14:43:45.140438 lightshow-1.2.3/lightshow/_tests/dummy_psp_files/mock_cutoff_table.json
+-rw-r--r--   0        0        0        0 2024-04-16 14:43:45.140438 lightshow-1.2.3/lightshow/_tests/helpers/__init__.py
+-rw-r--r--   0        0        0    13328 2024-04-16 14:43:45.140438 lightshow-1.2.3/lightshow/_tests/helpers/geometry.py
+-rw-r--r--   0        0        0       82 2024-04-16 14:43:45.140438 lightshow-1.2.3/lightshow/_tests/sample_files/README.rst
+-rw-r--r--   0        0        0    42630 2024-04-16 14:43:45.140438 lightshow-1.2.3/lightshow/_tests/sample_files/ene_dep_broad.txt
+-rw-r--r--   0        0        0    43441 2024-04-16 14:43:45.140438 lightshow-1.2.3/lightshow/_tests/sample_files/gauss_broad.txt
+-rw-r--r--   0        0        0    43519 2024-04-16 14:43:45.140438 lightshow-1.2.3/lightshow/_tests/sample_files/lorentz_broad.txt
+-rw-r--r--   0        0        0    43398 2024-04-16 14:43:45.140438 lightshow-1.2.3/lightshow/_tests/sample_files/voigt_broad.txt
+-rw-r--r--   0        0        0      376 2024-04-16 14:43:45.140438 lightshow-1.2.3/lightshow/_tests/structure_files/mp-10734/POSCAR
+-rw-r--r--   0        0        0      198 2024-04-16 14:43:45.140438 lightshow-1.2.3/lightshow/_tests/structure_files/mp-1215/POSCAR
+-rw-r--r--   0        0        0      814 2024-04-16 14:43:45.140438 lightshow-1.2.3/lightshow/_tests/structure_files/mp-1840/POSCAR
+-rw-r--r--   0        0        0      284 2024-04-16 14:43:45.140438 lightshow-1.2.3/lightshow/_tests/structure_files/mp-2657/POSCAR
+-rw-r--r--   0        0        0      167 2024-04-16 14:43:45.140438 lightshow-1.2.3/lightshow/_tests/structure_files/mp-2664/POSCAR
+-rw-r--r--   0        0        0      287 2024-04-16 14:43:45.140438 lightshow-1.2.3/lightshow/_tests/structure_files/mp-390/POSCAR
+-rw-r--r--   0        0        0      460 2024-04-16 14:43:45.140438 lightshow-1.2.3/lightshow/_tests/structure_files/mp-430/POSCAR
+-rw-r--r--   0        0        0      403 2024-04-16 14:43:45.140438 lightshow-1.2.3/lightshow/_tests/structure_files/mp-458/POSCAR
+-rw-r--r--   0        0        0     1702 2024-04-16 14:43:45.140438 lightshow-1.2.3/lightshow/_tests/test_broaden.py
+-rw-r--r--   0        0        0     3798 2024-04-16 14:43:45.140438 lightshow-1.2.3/lightshow/_tests/test_database.py
+-rw-r--r--   0        0        0    12398 2024-04-16 14:43:45.140438 lightshow-1.2.3/lightshow/_tests/test_exciting.py
+-rw-r--r--   0        0        0     1225 2024-04-16 14:43:45.140438 lightshow-1.2.3/lightshow/_tests/test_metadata.py
+-rw-r--r--   0        0        0       22 2024-04-16 14:43:50.216423 lightshow-1.2.3/lightshow/_version.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:43:45.140438 lightshow-1.2.3/lightshow/common/__init__.py
+-rw-r--r--   0        0        0     2580 2024-04-16 14:43:45.140438 lightshow-1.2.3/lightshow/common/kpoints.py
+-rw-r--r--   0        0        0     3322 2024-04-16 14:43:45.140438 lightshow-1.2.3/lightshow/common/nbands.py
+-rw-r--r--   0        0        0    19997 2024-04-16 14:43:45.140438 lightshow-1.2.3/lightshow/database.py
+-rw-r--r--   0        0        0      766 2024-04-16 14:43:45.140438 lightshow-1.2.3/lightshow/defaults.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:43:45.140438 lightshow-1.2.3/lightshow/parameters/__init__.py
+-rw-r--r--   0        0        0      206 2024-04-16 14:43:45.140438 lightshow-1.2.3/lightshow/parameters/_base.py
+-rw-r--r--   0        0        0     9135 2024-04-16 14:43:45.140438 lightshow-1.2.3/lightshow/parameters/exciting.py
+-rw-r--r--   0        0        0     8143 2024-04-16 14:43:45.140438 lightshow-1.2.3/lightshow/parameters/feff.py
+-rw-r--r--   0        0        0    14263 2024-04-16 14:43:45.140438 lightshow-1.2.3/lightshow/parameters/ocean.py
+-rw-r--r--   0        0        0    29716 2024-04-16 14:43:45.140438 lightshow-1.2.3/lightshow/parameters/vasp.py
+-rw-r--r--   0        0        0    19869 2024-04-16 14:43:45.140438 lightshow-1.2.3/lightshow/parameters/xspectra.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:43:45.140438 lightshow-1.2.3/lightshow/postprocess/__init__.py
+-rw-r--r--   0        0        0     9023 2024-04-16 14:43:45.140438 lightshow-1.2.3/lightshow/postprocess/broaden.py
+-rw-r--r--   0        0        0     7584 2024-04-16 14:43:45.140438 lightshow-1.2.3/lightshow/postprocess/compare_utils.py
+-rw-r--r--   0        0        0    12888 2024-04-16 14:43:45.140438 lightshow-1.2.3/lightshow/postprocess/parse.py
+-rw-r--r--   0        0        0     4935 2024-04-16 14:43:45.140438 lightshow-1.2.3/lightshow/pymatgen_utils.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:43:45.140438 lightshow-1.2.3/lightshow/utils/__init__.py
+-rw-r--r--   0        0        0     1227 2024-04-16 14:43:45.140438 lightshow-1.2.3/lightshow/utils/environ_utils.py
+-rw-r--r--   0        0        0    32847 2024-04-16 14:43:45.140438 lightshow-1.2.3/notebooks/00_basic_usage.ipynb
+-rw-r--r--   0        0        0    10037 2024-04-16 14:43:45.140438 lightshow-1.2.3/notebooks/01_Ti_K_anatase_broaden.ipynb
+-rw-r--r--   0        0        0     5829 2024-04-16 14:43:45.140438 lightshow-1.2.3/notebooks/compare_spectra.ipynb
+-rw-r--r--   0        0        0     6741 2024-04-16 14:43:45.140438 lightshow-1.2.3/notebooks/parse_spectra.ipynb
+-rwxr-xr-x   0        0        0    41029 2024-04-16 14:43:45.140438 lightshow-1.2.3/notebooks/spectra_files/anatase_exciting.txt
+-rw-r--r--   0        0        0     3816 2024-04-16 14:43:45.140438 lightshow-1.2.3/notebooks/spectra_files/anatase_exp.txt
+-rw-r--r--   0        0        0    54210 2024-04-16 14:43:45.144438 lightshow-1.2.3/notebooks/spectra_files/anatase_ocean.txt
+-rw-r--r--   0        0        0     5000 2024-04-16 14:43:45.144438 lightshow-1.2.3/notebooks/spectra_files/anatase_theory_FEFF.txt
+-rw-r--r--   0        0        0  2000000 2024-04-16 14:43:45.148438 lightshow-1.2.3/notebooks/spectra_files/anatase_theory_VASP.txt
+-rwxr-xr-x   0        0        0    11578 2024-04-16 14:43:45.148438 lightshow-1.2.3/notebooks/spectra_files/anatase_xspectra.txt
+-rw-r--r--   0        0        0     1980 2024-04-16 14:43:45.148438 lightshow-1.2.3/pyproject.toml
+-rw-r--r--   0        0        0     1204 2024-04-16 14:43:45.148438 lightshow-1.2.3/scripts/README.rst
+-rw-r--r--   0        0        0      575 2024-04-16 14:43:45.148438 lightshow-1.2.3/scripts/build_docs.sh
+-rw-r--r--   0        0        0      184 2024-04-16 14:43:45.148438 lightshow-1.2.3/scripts/build_project.sh
+-rw-r--r--   0        0        0      418 2024-04-16 14:43:45.148438 lightshow-1.2.3/scripts/install.sh
+-rw-r--r--   0        0        0     1076 2024-04-16 14:43:45.148438 lightshow-1.2.3/scripts/update_version.sh
+-rw-r--r--   0        0        0     9166 1970-01-01 00:00:00.000000 lightshow-1.2.3/PKG-INFO
```

### Comparing `lightshow-1.2.2/.github/workflows/ci.yml` & `lightshow-1.2.3/.github/workflows/ci.yml`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 name: CI
 
 # Run on all PR's and on pushes/merges to deploy and master
 on:
   pull_request:
-    branches: ['master', '!paper.md']
+    branches: ['master', 'dev/*', '!paper.md']
   push:
-    branches: ['master', '!paper.md']
+    branches: ['master', 'dev/*', '!paper.md']
     tags: ["v*"]
 
 jobs:
 
   tests:
-    name: Run unit testing suite
+    name: Tests
 
     env:
         MP_API_KEY: ${{ secrets.MP_API_KEY }}
 
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
         os: [ubuntu-latest, macOS-latest]
         python-version: [3.9, '3.10', 3.11]
 
     steps:
 
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
 
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v2
       with:
         python-version: ${{ matrix.python-version }}
 
     - name: Install testing dependencies
@@ -43,72 +43,50 @@
     - name: Upload code coverage
       uses: codecov/codecov-action@v2
       timeout-minutes: 10
       with:
         token: ${{ secrets.CODECOV_TOKEN }}
         fail_ci_if_error: false
 
-  black:
-    name: Run Black code quality check
-
+  ruff:
+    name: Run Ruff code quality check
     runs-on: ubuntu-latest
-
     steps:
-      - uses: actions/checkout@v3
-      - uses: rickstaa/action-black@v1
+      - uses: actions/checkout@v4
+      - uses: chartboost/ruff-action@v1
         with:
-          black_args: "lightshow/ --check"
-          fail_on_error: "true"
+          src: './lightshow'
 
   flake8_py3:
     name: Run flake8 code quality check
-
     runs-on: ubuntu-latest
-
     steps:
-
-      - uses: actions/checkout@v3
-
+      - uses: actions/checkout@v4
       - name: Setup Python
         uses: actions/setup-python@v2
         with:
           python-version: 3.9
-
       - name: Install flake8
         run: pip install flake8
-
       - name: Run flake8
         uses: suo/flake8-github-action@releases/v1
         with:
           checkName: 'flake8_py3'   # NOTE: this needs to be the same as the job name
         env:
           GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
 
-  check_semantic_version_placeholder:
-    name: Check semantic version placeholder exists in the __init__
-
-    runs-on: ubuntu-latest
-
-    steps:
-
-    - uses: actions/checkout@v3
-
-    - name: Check lines exist
-      run: |
-        grep -x "__version__ = ...  # semantic-version-placeholder" lightshow/__init__.py
-
   docs:
     name: Build documentation test
 
     runs-on: ubuntu-latest
 
     steps:
 
     - name: Checkout
-      uses: actions/checkout@v3
+      uses: actions/checkout@v4
 
     ###########################################################################
     # Getting the tags like this is REQUIRED for the dynamic versioning
     # system to work properly
     - name: Get tags
       if: "! startsWith(github.ref, 'refs/tags')"
       run: git fetch --unshallow --tags
@@ -134,23 +112,22 @@
       name: pypi
       url: https://pypi.org/project/lightshow/
     permissions:
       id-token: write
 
     needs:
       - tests
-      - black
+      - ruff
       - flake8_py3
-      - check_semantic_version_placeholder
       - docs
 
     steps:
 
     - name: Checkout
-      uses: actions/checkout@v3
+      uses: actions/checkout@v4
 
     - name: Set up Python 3.9
       uses: actions/setup-python@v2
       with:
         python-version: 3.9
 
     - name: Build and apply version
@@ -169,17 +146,16 @@
       url: ${{ steps.deployment.outputs.page_url }}
     
     # Only allow tagged commits
     if: github.event_name == 'push' && startsWith(github.ref, 'refs/tags')
 
     needs:
       - tests
-      - black
+      - ruff
       - flake8_py3
-      - check_semantic_version_placeholder
       - docs
       - build_and_publish
 
     # Sets permissions of the GITHUB_TOKEN to allow deployment to GitHub Pages
     permissions:
       contents: read
       pages: write
@@ -191,15 +167,15 @@
       cancel-in-progress: true
 
     runs-on: ubuntu-latest
 
     steps:
 
     - name: Checkout
-      uses: actions/checkout@v3
+      uses: actions/checkout@v4
 
     - name: Set up Python 3.9
       uses: actions/setup-python@v2
       with:
         python-version: 3.9
 
     - name: Build and apply version
```

### Comparing `lightshow-1.2.2/.gitignore` & `lightshow-1.2.3/.gitignore`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 .DS_Store
+pyrightconfig.json
 
 *.pyc
 !build_sphinx.sh
 *.png
 .ipynb_checkpoints/
 .coverage
```

### Comparing `lightshow-1.2.2/CHANGES.md` & `lightshow-1.2.3/CHANGES.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 # Changelog
 
+## v1.2.3
+
+- Fix the "ghost atom" problem in VASP. See [#256](https://github.com/AI-multimodal/Lightshow/issues/254).
+- Cleanup the testing suite, replace Black with Ruff.
+
+
 ## v1.2.2
 
 - Add multiple utilities into the `lightshow.postprocess`.
 - Add functionality to output a `metadata.json` file when writing to disk. This saves information about site multiplicity, and allows for other information to be saved in the future.
 
 ## v1.2.1
```

### Comparing `lightshow-1.2.2/CONTRIBUTING.md` & `lightshow-1.2.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `lightshow-1.2.2/LICENSE` & `lightshow-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lightshow-1.2.2/README.md` & `lightshow-1.2.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
     
 ![sysfs line plot](https://raw.githubusercontent.com/AI-multimodal/Lightshow/master/docs/_static/images/lightshow.jpg)
 
 [![image](https://joss.theoj.org/papers/a9cabcd7f4b85a926a797997c6622b43/status.svg)](https://joss.theoj.org/papers/a9cabcd7f4b85a926a797997c6622b43)
 [![image](https://github.com/AI-multimodal/Lightshow/actions/workflows/ci.yml/badge.svg)](https://github.com/AI-multimodal/Lightshow/actions/workflows/ci.yml)
 [![image](https://codecov.io/gh/AI-multimodal/Lightshow/branch/master/graph/badge.svg?token=CW7BMFA5O7)](https://codecov.io/gh/AI-multimodal/Lightshow)
 [![image](https://app.codacy.com/project/badge/Grade/d31a4e18672c4d71bbaafa719181c140)](https://www.codacy.com/gh/AI-multimodal/Lightshow/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=AI-multimodal/Lightshow&amp;utm_campaign=Badge_Grade) <br>
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 [![python](https://img.shields.io/badge/-Python_3.9+-blue?logo=python&logoColor=white)](https://github.com/pre-commit/pre-commit)
 [![Downloads](https://static.pepy.tech/badge/lightshow)](https://pepy.tech/project/lightshow)
 </div>
     
 ------------------------------------------------------------------------
 
 **Lightshow** is a Python library for easily generating computational
```

### Comparing `lightshow-1.2.2/docs/Makefile` & `lightshow-1.2.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `lightshow-1.2.2/docs/_static/images/lightshow.jpg` & `lightshow-1.2.3/docs/_static/images/lightshow.jpg`

 * *Files identical despite different names*

### Comparing `lightshow-1.2.2/docs/_static/images/lightshow_old.jpg` & `lightshow-1.2.3/docs/_static/images/lightshow_old.jpg`

 * *Files identical despite different names*

### Comparing `lightshow-1.2.2/docs/make.bat` & `lightshow-1.2.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `lightshow-1.2.2/docs/source/conf.py` & `lightshow-1.2.3/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `lightshow-1.2.2/docs/source/index.rst` & `lightshow-1.2.3/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `lightshow-1.2.2/docs/source/installation.rst` & `lightshow-1.2.3/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `lightshow-1.2.2/docs/source/lightshow.parameters.rst` & `lightshow-1.2.3/docs/source/lightshow.parameters.rst`

 * *Files identical despite different names*

### Comparing `lightshow-1.2.2/docs/source/lightshow.rst` & `lightshow-1.2.3/docs/source/lightshow.rst`

 * *Files identical despite different names*

### Comparing `lightshow-1.2.2/docs/source/project/funding.rst` & `lightshow-1.2.3/docs/source/project/funding.rst`

 * *Files identical despite different names*

### Comparing `lightshow-1.2.2/docs/source/quickstart.rst` & `lightshow-1.2.3/docs/source/quickstart.rst`

 * *Files identical despite different names*

### Comparing `lightshow-1.2.2/figures/Lightshow_Workflow_Diagram.jpg` & `lightshow-1.2.3/figures/Lightshow_Workflow_Diagram.jpg`

 * *Files identical despite different names*

### Comparing `lightshow-1.2.2/figures/Lightshow_Workflow_Diagram.pdf` & `lightshow-1.2.3/figures/Lightshow_Workflow_Diagram.pdf`

 * *Files identical despite different names*

### Comparing `lightshow-1.2.2/lightshow/_tests/conftest.py` & `lightshow-1.2.3/lightshow/_tests/conftest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
+import random
 from copy import deepcopy
 from functools import cache
 from pathlib import Path
-import pytest
-import random
 
+import pytest
 from pymatgen.core.structure import Structure
 
 from lightshow import Database
 
 STRUCTURE_FILES_PATH = Path(__file__).parent / Path("structure_files")
 
 SPECTRA_FILES_PATH = Path.cwd() / Path("notebooks") / Path("spectra_files")
@@ -61,15 +61,15 @@
     # "mp-1208324", "mp-10734"]
     # return Database.from_materials_project(material_ids=trouble)
     # return Database.from_materials_project(material_ids=["mp-980945"])
     db = Database.from_materials_project(chemsys=["Ti-*", "Mn-O-*"])
     # db = Database.from_materials_project(material_ids=["mp-390"])
     keys = sorted(list(db._structures.keys()))
     random.seed(123)
-    keys = random.sample(keys, 1000)
+    keys = random.sample(keys, 100)
     db._structures = {key: db._structures[key] for key in keys}
     db._metadata = {key: db._metadata[key] for key in keys}
     return db
 
 
 @pytest.fixture
 def database_for_stress_test():
```

### Comparing `lightshow-1.2.2/lightshow/_tests/helpers/geometry.py` & `lightshow-1.2.3/lightshow/_tests/helpers/geometry.py`

 * *Files identical despite different names*

### Comparing `lightshow-1.2.2/lightshow/_tests/sample_files/ene_dep_broad.txt` & `lightshow-1.2.3/lightshow/_tests/sample_files/ene_dep_broad.txt`

 * *Files identical despite different names*

### Comparing `lightshow-1.2.2/lightshow/_tests/sample_files/gauss_broad.txt` & `lightshow-1.2.3/lightshow/_tests/sample_files/gauss_broad.txt`

 * *Files identical despite different names*

### Comparing `lightshow-1.2.2/lightshow/_tests/sample_files/lorentz_broad.txt` & `lightshow-1.2.3/lightshow/_tests/sample_files/lorentz_broad.txt`

 * *Files identical despite different names*

### Comparing `lightshow-1.2.2/lightshow/_tests/sample_files/voigt_broad.txt` & `lightshow-1.2.3/lightshow/_tests/sample_files/voigt_broad.txt`

 * *Files identical despite different names*

### Comparing `lightshow-1.2.2/lightshow/_tests/structure_files/mp-1840/POSCAR` & `lightshow-1.2.3/lightshow/_tests/structure_files/mp-1840/POSCAR`

 * *Files identical despite different names*

### Comparing `lightshow-1.2.2/lightshow/_tests/test_broaden.py` & `lightshow-1.2.3/lightshow/_tests/test_broaden.py`

 * *Files identical despite different names*

### Comparing `lightshow-1.2.2/lightshow/_tests/test_database.py` & `lightshow-1.2.3/lightshow/_tests/test_database.py`

 * *Files identical despite different names*

### Comparing `lightshow-1.2.2/lightshow/_tests/test_exciting.py` & `lightshow-1.2.3/lightshow/_tests/test_exciting.py`

 * *Files identical despite different names*

### Comparing `lightshow-1.2.2/lightshow/_tests/test_metadata.py` & `lightshow-1.2.3/lightshow/_tests/test_metadata.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 from pathlib import Path
 
 from lightshow.parameters.feff import FEFFParameters
 
 
-def test_multiplicipty_writing(database_from_file, tmp_path):
-    target = Path(tmp_path) / Path("multi") / Path("destination")
+def test_multiplicity_writing(database_from_file, tmp_path):
+    target = Path(tmp_path) / "t"
     target.mkdir(exist_ok=True, parents=True)
     R = 10.0
     feff_parameters = FEFFParameters(
         cards={
             "S02": "0",
             "COREHOLE": "RPA",
             "CONTROL": "1 1 1 1 1 1",
@@ -28,17 +28,16 @@
         target,
         absorbing_atoms="all",
         options=[feff_parameters],
         write_unit_cells=True,
         pbar=False,
     )
     for k, v in database_from_file.metadata.items():
-        metadata_fn = target / Path(k) / Path("metadata.json")
-        with open(metadata_fn) as f:
-            d_metadata = json.load(f)
+        fname = target / k / Path("multiplicity.json")
+        with open(fname) as f:
+            mult = json.load(f)
         prim_meta = v["primitive"]
         for i_site, n_multi in zip(
             prim_meta["sites"], prim_meta["multiplicities"]
         ):
             i_site = str(i_site)
-            assert "multiplicities" in d_metadata
-            assert d_metadata["multiplicities"][i_site] == n_multi
+            assert mult[i_site] == n_multi
```

### Comparing `lightshow-1.2.2/lightshow/common/kpoints.py` & `lightshow-1.2.3/lightshow/common/kpoints.py`

 * *Files identical despite different names*

### Comparing `lightshow-1.2.2/lightshow/common/nbands.py` & `lightshow-1.2.3/lightshow/common/nbands.py`

 * *Files identical despite different names*

### Comparing `lightshow-1.2.2/lightshow/database.py` & `lightshow-1.2.3/lightshow/database.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,57 @@
 """Contains all relevant classes and functions for constructing databases of
 various materials and clusters. This includes pulling and processing data from
 the `Materials Project Database <https://materialsproject.org/>`_, as well as
 utilizing existing data the user may have on their hard drive."""
 
-from datetime import datetime
 import json
+from datetime import datetime
 from pathlib import Path
 from shutil import copy2
 from warnings import warn
 
 from monty.json import MSONable
 from mp_api.client import MPRester
-from pymatgen.core.structure import Structure, Molecule
+from pymatgen.core.structure import Molecule, Structure
 from tqdm import tqdm
 
-from lightshow import _get_API_key_from_environ
 from lightshow import pymatgen_utils
+from lightshow.utils.environ_utils import get_API_key_from_environ
 
 
 def _get_api_key(api_key):
     if api_key is None:
-        api_key = _get_API_key_from_environ()
+        api_key = get_API_key_from_environ()
     if api_key is None:
         raise ValueError(f"Invalid API key {api_key}")
     return api_key
 
 
+def _get_method(method, mpr):
+    """Get all the available search methods; if the given method is not
+    present, the search will be performed using mpr.materials.search"""
+
+    methods = [
+        methods
+        for methods in dir(mpr.materials)
+        if methods is not callable and not methods.startswith("_")
+    ]
+
+    if method is None:
+        print("Searching Materials Project with default method")
+    elif method not in methods:
+        warn(
+            f"Provided method={method} not in available methods {methods}",
+            "falling back on default search method.",
+        )
+        method = None
+
+    return method
+
+
 class Database(MSONable):
     """Contains all materials and metadata for some database."""
 
     @classmethod
     def from_files_molecule(
         cls,
         root,
@@ -45,15 +67,16 @@
         ----------
         root : str
             The directory in which to begin the search.
         filename : str, optional
             The files to search for. Uses ``rglob`` to recursively find any
             files matching ``filename`` within the provided directory.
         lattice : list of floats, optional
-            Lattice parameter used to construct the crystal lattice.
+            Lattice parameter used to construct the crystal lattice. If not
+            provided, defaults to [20.0, 20.0, 20.0] Angstroms.
         pbar : bool, optional
             If True, will show a tqdm progress bar.
 
         Returns
         -------
         Database
         """
@@ -110,53 +133,55 @@
             key = f"{key:08}"
             struct = Structure.from_file(path)
             structures[key] = struct.get_primitive_structure()
             metadata[key] = {"origin": str(path)}
         return cls(structures=structures, metadata=metadata, supercells=dict())
 
     @classmethod
-    def from_materials_project(cls, **kwargs):
+    def from_materials_project(cls, api_key=None, method=None, **kwargs):
         """Constructs the :class:`.Database` object by pulling structures and
         metadata directly from the Materials Project. This is a simple
         passthrough method which utilizes the MPRester.materials.search
         API of the Materials Project v2 API.
 
         Parameters
         ----------
-        **kwargs
-            Description
-
-        Examples
-        --------
-
-        Deleted Parameters
-        ------------------
-        mpr_query_kwargs : dict
-            Direct passthrough to MPRester.materials.search. See
-            examples below.
         api_key : None, optional
             API key which can either be provided directly or is read from
             the MP_API_KEY environment variable.
+        method : None, optional, str
+            Keyword to get different information about materials'
+            for e.g. 'thermo', 'xas', 'summary' etc. fetch information on
+            thermodynamic properties, computed XAS data, large amount of
+            amalgated data about the material, respectively.
+            See https://api.materialsproject.org/docs for more details.
+        **kwargs
+            Description
 
         Returns
         -------
         Database
         """
 
-        api_key = _get_api_key(kwargs.get("api_key"))
-
-        try:
-            kwargs.pop("api_key")
-        except KeyError:
-            pass
+        api_key = _get_api_key(api_key)
+        method = kwargs.get("method")
 
         with MPRester(api_key) as mpr:
-            searched = mpr.materials.search(**kwargs)
-
-        structures = {s.material_id.string: s.structure for s in searched}
+            method = _get_method(method, mpr=mpr)
+            if method is not None:
+                searched = getattr(mpr.materials, method).search(**kwargs)
+            else:
+                searched = mpr.materials.search(**kwargs)
+
+        structures = {
+            s.material_id.string: s.structure
+            if hasattr(s, "structure")
+            else None
+            for s in searched
+        }
         metadata = {s.material_id.string: s.dict() for s in searched}
 
         return cls(structures=structures, metadata=metadata, supercells=dict())
 
     def initialize_supercells(self, supercell_cutoff=9.0):
         """Initializes the supercells from the structures pulled from the
         Materials project.
@@ -254,26 +279,32 @@
             for key, value in self.as_dict().items()
             if key not in ["structures", "metadata", "supercells"]
         }
 
     def __init__(
         self,
         structures,
-        metadata=dict(),
-        supercells=dict(),
+        metadata=None,
+        supercells=None,
         supercell_cutoff=None,
         inequivalent_sites_initialized=False,
         supercells_initialized=False,
     ):
         """Initializer for the Database class. Note it is recommended to use
         the classmethods to initialize this object."""
 
         self._structures = structures
-        self._metadata = metadata
-        self._supercells = supercells
+        if metadata is None:
+            self._metadata = {}
+        else:
+            self._metadata = metadata
+        if supercells is None:
+            self._supercells = {}
+        else:
+            self._supercells = supercells
         self._supercell_cutoff = supercell_cutoff
         self._inequivalent_sites_initialized = inequivalent_sites_initialized
         self._supercells_initialized = supercells_initialized
 
     def _setup_preliminary_attributes(self):
         """Initializes supercells and inequivalent site info in the metadata
         if they're not already."""
@@ -331,49 +362,39 @@
         pbar : bool, optional
         """
 
         for key, structure in tqdm(self._structures.items(), disable=not pbar):
             fname = Path(root) / key / "POSCAR"
             structure.to(fmt="POSCAR", filename=str(fname))
 
-    def _write_origin_paths(self, root, pbar=False):
-        """A helper method for writing important metadata for each of the
-        structures if the data was loaded from disk.
-
-        Parameters
-        ----------
-        root : os.PathLike
-        pbar : bool, optional
-        """
+    def _write_multiplicity(self, root, pbar=False):
+        """Helper method for writing the site multiplicity information of
+        the structure."""
 
         for key, metadata in tqdm(self._metadata.items(), disable=not pbar):
-            if "origin" not in metadata.keys():
-                continue
-            fname = Path(root) / key / "metadata.json"
-            origin = str(Path(metadata["origin"]).resolve())
-            new_metadata = {"origin": origin}
+            fname = Path(root) / key / "multiplicity.json"
             multiplicities = {
                 i_site: n_multi
                 for i_site, n_multi in zip(
                     metadata["primitive"]["sites"],
                     metadata["primitive"]["multiplicities"],
                 )
             }
-            new_metadata["multiplicities"] = multiplicities
             with open(fname, "w") as outfile:
-                json.dump(new_metadata, outfile, indent=4, sort_keys=True)
+                json.dump(multiplicities, outfile, indent=4, sort_keys=True)
 
     def write(
         self,
         root,
         absorbing_atoms=None,
         options=[],
         pbar=True,
         copy_script=None,
         write_unit_cells=True,
+        write_multiplicity=True,
     ):
         """The core method of the :class:`.Database` class. This method will
         write all input files specified in the ``options`` parameter to disk.
         Of particular note is the directory structure, which is always
         consistent regardless of the type of calculation: At the first level is
         the ``key`` (usually an mpid) indexing the material of interest. At the
         next level is the user-specified "name" of the calculation, which are
@@ -423,14 +444,17 @@
             If True, enables the :class:`tqdm` progress bar.
         copy_script : os.PathLike
             If not ``None``, will copy the script in the provided path to each
             of the input file locations.
         write_unit_cells : bool, optional
             If True, writes the unit cells in the materials directory in
             POSCAR format. Very useful!
+        write_multiplicity : bool, optional
+            If True, writes the multiplicities of each atom in the unit cell
+            to a multiplicities.json file.
         """
 
         self._setup_preliminary_attributes()
 
         root = str(Path(root).resolve())  # Get absolute path
 
         _write_all_atoms = False
@@ -507,14 +531,14 @@
                         warn(f"error: {key}+{option.name}: {d}")
                     if copy_script is not None and "paths" in status.keys():
                         for p in status["paths"]:
                             copy2(copy_script, p)
 
         if write_unit_cells:
             self._write_unit_cells(root, pbar=pbar)
-
-        self._write_origin_paths(root, pbar=pbar)
+        if write_multiplicity:
+            self._write_multiplicity(root, pbar=pbar)
 
         # Save a metadata file (not a serialized version of this class) to
         # disk along with the input files
         with open(writer_metadata_path, "w") as outfile:
             json.dump(writer_metadata, outfile, indent=4, sort_keys=True)
```

### Comparing `lightshow-1.2.2/lightshow/parameters/exciting.py` & `lightshow-1.2.3/lightshow/parameters/exciting.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-from pathlib import Path
 import xml.etree.ElementTree as ET
+from pathlib import Path
 from warnings import warn
 
 from monty.json import MSONable
 from pymatgen.io.exciting import ExcitingInput
 
-from lightshow.parameters._base import _BaseParameters
 from lightshow.common.kpoints import GenericEstimatorKpoints
 from lightshow.common.nbands import UnitCellVolumeEstimate
-from lightshow import _get_SPECIES_DIRECTORY_from_environ
+from lightshow.parameters._base import _BaseParameters
+from lightshow.utils.environ_utils import get_SPECIES_DIRECTORY_from_environ
 
 EXCITING_DEFAULT_GQMAX = 4.0
 
 EXCITING_DEFAULT_CARDS = {
     "structure": {"speciespath": "./", "autormt": "true"},
     "groundstate": {
         "xctype": "GGA_PBE",
@@ -142,15 +142,15 @@
         name="EXCITING",
     ):
         # Default cards
         self._cards = cards
 
         # species directory
         if species_directory is None:
-            species_directory = _get_SPECIES_DIRECTORY_from_environ()
+            species_directory = get_SPECIES_DIRECTORY_from_environ()
         if species_directory is None:
             warn(
                 "species_directory not set, and SPECIES_DIRECTORY not in "
                 "the current environment variables. The current/working "
                 "folder will be used as default. Please make sure you copy "
                 "all the corresponding species file into the working folder, "
                 "e.g. where the input.xml file is generated."
@@ -206,17 +206,17 @@
 
         excitinginput = ExcitingInput(structure)
         # Estimate number of band
         nbands = self._nbands(structure)
         self._cards["xs"]["BSE"]["nstlxas"] = f"1 {nbands}"
         # Estimate number of kpoints
         kmesh = self._kpoints(structure)
-        self._cards["groundstate"][
-            "ngridk"
-        ] = f"{kmesh[0]} {kmesh[1]} {kmesh[2]}"
+        self._cards["groundstate"]["ngridk"] = (
+            f"{kmesh[0]} {kmesh[1]} {kmesh[2]}"
+        )
         self._cards["xs"]["ngridk"] = f"{kmesh[0]} {kmesh[1]} {kmesh[2]}"
         self._cards["xs"]["ngridq"] = f"{kmesh[0]} {kmesh[1]} {kmesh[2]}"
         # Determine XAS species
         species = [structure[site].specie.symbol for site in sites]
 
         for i, specie in enumerate(
             sorted(structure.types_of_species, key=lambda el: el.X)
```

### Comparing `lightshow-1.2.2/lightshow/parameters/feff.py` & `lightshow-1.2.3/lightshow/parameters/feff.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 from copy import copy
 from pathlib import Path
 from warnings import warn
 
 from monty.json import MSONable
-from pymatgen.io.feff.sets import MPXANESSet, MPEXAFSSet, FEFFDictSet
+from pymatgen.io.feff.sets import FEFFDictSet, MPEXAFSSet, MPXANESSet
 
 from lightshow.parameters._base import _BaseParameters
 
-
 FEFF_DEFAULT_CARDS = {
     "S02": "0",
     "COREHOLE": "RPA",
     "CONTROL": "1 1 1 1 1 1",
     "XANES": "4 0.04 0.1",
     "SCF": "7.0 0 100 0.2 3",
     "FMS": "9.0 0",
@@ -50,15 +49,15 @@
                 "S02": "0",
                 "COREHOLE": "RPA",
                 "CONTROL": "1 1 1 1 1 1",
                 "XANES": "4 0.04 0.1",
                 "SCF": "7.0 0 100 0.2 3",
                 "FMS": "9.0 0",
                 "EXCHANGE": "0 0.0 0.0 2",
-                "RPATH": "-1"
+                "RPATH": "-1",
             }
 
         And for EXAFS,
 
         .. code-block:: python
 
             cards = {
```

### Comparing `lightshow-1.2.2/lightshow/parameters/ocean.py` & `lightshow-1.2.3/lightshow/parameters/ocean.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 from copy import copy
 from pathlib import Path
-import numpy as np
 
+import numpy as np
 from monty.json import MSONable
 from pymatgen.core import Element
 
-from lightshow.parameters._base import _BaseParameters
 from lightshow.common.kpoints import GenericEstimatorKpoints
 from lightshow.common.nbands import UnitCellVolumeEstimate
-
+from lightshow.parameters._base import _BaseParameters
 
 OCEAN_DEFAULT_CARDS = {
     "dft": "qe",
     "ecut": "-1",
     "opf.program": "hamann",
     "para_prefix": "mpirun -np 24",
 }
@@ -32,18 +31,18 @@
         parameters in OCEAN; the values are the correspongding values.
         In LightShow, minimum parameters to run ocean is provided in
         ``OCEAN_DEFAULT_CARDS``, which looks something like
 
         .. code-block:: python
 
             cards = {
-                    "dft" : "qe",
-                    "ecut" : "-1",
-                    "opf.program" : "hamann",
-                    "para_prefix" : "mpirun -np 24",
+                "dft": "qe",
+                "ecut": "-1",
+                "opf.program": "hamann",
+                "para_prefix": "mpirun -np 24",
             }
 
         The detailed description of the OCEAN parameters can be find at
         its official website. If the user wants to change some parameters,
         they can just add a key-value pair to the cards.
     kpoints : lightshow.common.kpoints._BaseKpointsMethod
         The method for constructing he kpoints file from the structure. Should
```

### Comparing `lightshow-1.2.2/lightshow/parameters/vasp.py` & `lightshow-1.2.3/lightshow/parameters/vasp.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,23 @@
+import warnings
 from copy import copy, deepcopy
 from functools import lru_cache
 from pathlib import Path
-import warnings
 
-from monty.json import MSONable
 import numpy as np
-from pymatgen.io.vasp.sets import DictSet
+from monty.json import MSONable
 from pymatgen.io.vasp.inputs import Incar as pmgIncar
 from pymatgen.io.vasp.inputs import Kpoints as pmgKpoints
 from pymatgen.io.vasp.inputs import Poscar as pmgPoscar
+from pymatgen.io.vasp.sets import DictSet
 
-from lightshow import _get_POTCAR_DIRECTORY_from_environ
-from lightshow.parameters._base import _BaseParameters
 from lightshow.common.kpoints import GenericEstimatorKpoints
 from lightshow.common.nbands import UnitCellVolumeEstimate
-
+from lightshow.parameters._base import _BaseParameters
+from lightshow.utils.environ_utils import get_POTCAR_DIRECTORY_from_environ
 
 VASP_INCAR_DEFAULT_NEUTRAL_POTENTIAL = {
     "ALGO": "Normal",
     "EDIFF": 1e-05,
     "IBRION": 2,
     "ISIF": 2,
     "ISMEAR": 0,
@@ -687,15 +686,21 @@
         atom_type_loc = np.where(np.array(self.site_symbols) == atom_type)[
             0
         ].item()
         new_line_5 = [atom_type, *self.site_symbols]
         line_6_asint = [int(xx) for xx in self.natoms]
         line_6_asint[atom_type_loc] -= 1
         new_line_6_asint = [1, *line_6_asint]
-        new_line_6 = [str(xx) for xx in new_line_6_asint]
+
+        # Account for the fact that sometimes we only have a single atom
+        # of the absorbing type in the unit cell
+        new_line_5 = [
+            el for ii, el in enumerate(new_line_5) if new_line_6_asint[ii] > 0
+        ]
+        new_line_6 = [str(xx) for xx in new_line_6_asint if xx > 0]
 
         # Use the new lines 5 and 6
         lines[5] = " ".join(new_line_5)
         lines[6] = " ".join(new_line_6)
 
         # Execute the swap. First, get the line of interest
         move_to_front = lines[site_index]
@@ -806,15 +811,15 @@
             )
 
         # Method for generating the KPOINTS file
         self._kpoints = kpoints
 
         # POTCAR information
         if potcar_directory is None:
-            potcar_directory = _get_POTCAR_DIRECTORY_from_environ()
+            potcar_directory = get_POTCAR_DIRECTORY_from_environ()
         if potcar_directory is None:
             warnings.warn(
                 "potcar_directory not provided, and VASP_POTCAR_DIRECTORY "
                 "not in the current environment variables. POTCAR files will "
                 "not be written."
             )
```

### Comparing `lightshow-1.2.2/lightshow/parameters/xspectra.py` & `lightshow-1.2.3/lightshow/parameters/xspectra.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-from pathlib import Path
-import json
-import bz2
 import base64
+import bz2
+import json
 import shutil
+from pathlib import Path
 from warnings import warn
 
 from monty.json import MSONable
 from pymatgen.io.pwscf import PWInput
 
-from lightshow.parameters._base import _BaseParameters
 from lightshow.common.kpoints import GenericEstimatorKpoints
-from lightshow import (
-    _get_CHPSP_DIRECTORY_from_environ,
-    _get_PSP_DIRECTORY_from_environ,
+from lightshow.parameters._base import _BaseParameters
+from lightshow.utils.environ_utils import (
+    get_CHPSP_DIRECTORY_from_environ,
+    get_PSP_DIRECTORY_from_environ,
 )
 
 XSPECTRA_DEFAULT_CARDS = {
     "QE": {
         "control": {"restart_mode": "from_scratch"},
         "electrons": {"conv_thr": 1e-08, "mixing_beta": 0.4},
         "system": {
@@ -59,48 +59,51 @@
     cards : dict
         A dictionary of of the cards to be control the parameters in the
         OCEAN calculations. For example, one might wish to use something like
 
         .. code-block:: python
 
            cards = {
-                    "QE": {
-                        "control": {
-                            "restart_mode": "from_scratch",
-                        },
-                        "electrons": {"conv_thr": 1e-08, "mixing_beta": 0.4},
-                        "system": {
-                            "degauss": 0.002,
-                            "ecutrho": 320,
-                            "ecutwfc": 40,
-                            "nspin": 1,
-                            "occupations": "smearing",
-                            "smearing": "gauss",
-                        },
-                    },
-                    "XS": {
-                        "cut_occ": {"cut_desmooth": 0.3},
-                        "input_xspectra": {
-                            "outdir": "../",
-                            "prefix": "pwscf",
-                            "xcheck_conv": 200,
-                            "xerror": 0.01,  #
-                            "xniter": 5000,
-                            "xcoordcrys": ".false.",
-                       },
-                        "kpts": {"kpts": "2 2 2", "shift": "0 0 0"},
-                        "plot": {
-                            "cut_occ_states": ".true.",
-                            "terminator": ".true.",
-                            "xemax": 70,
-                            "xemin": -15.0,
-                            "xnepoint": 400,
-                        },
-                    },
-            }
+               "QE": {
+                   "control": {
+                       "restart_mode": "from_scratch",
+                   },
+                   "electrons": {
+                       "conv_thr": 1e-08,
+                       "mixing_beta": 0.4,
+                   },
+                   "system": {
+                       "degauss": 0.002,
+                       "ecutrho": 320,
+                       "ecutwfc": 40,
+                       "nspin": 1,
+                       "occupations": "smearing",
+                       "smearing": "gauss",
+                   },
+               },
+               "XS": {
+                   "cut_occ": {"cut_desmooth": 0.3},
+                   "input_xspectra": {
+                       "outdir": "../",
+                       "prefix": "pwscf",
+                       "xcheck_conv": 200,
+                       "xerror": 0.01,  #
+                       "xniter": 5000,
+                       "xcoordcrys": ".false.",
+                   },
+                   "kpts": {"kpts": "2 2 2", "shift": "0 0 0"},
+                   "plot": {
+                       "cut_occ_states": ".true.",
+                       "terminator": ".true.",
+                       "xemax": 70,
+                       "xemin": -15.0,
+                       "xnepoint": 400,
+                   },
+               },
+           }
 
     kpoints : lightshow.common.kpoints._BaseKpointsMethod
         The method for constructing he kpoints file from the structure. Should
         be a class with a ``__call__`` method defined. This method should take
         the structure as input and return a tuple corresponding to the kpoints
         density along each axis.
     psp_directory : os.PathLike, optional
@@ -149,28 +152,28 @@
         name="XSpectra",
     ):
         # Default cards
         self._cards = cards
 
         # chpsp information
         if chpsp_directory is None:
-            chpsp_directory = _get_CHPSP_DIRECTORY_from_environ()
+            chpsp_directory = get_CHPSP_DIRECTORY_from_environ()
         if chpsp_directory is None:
             warn(
                 "chpsp_directory not provided, and XS_CHPSP_DIRECTORY not in "
                 "the current environment variables. core-hole pseudo "
                 "potential files will not be written."
             )
         self._chpsp_directory = chpsp_directory
         # psp information
         self._psp_cutoff_table = psp_cutoff_table
         self._psp_json = psp_json
 
         if psp_directory is None:
-            psp_directory = _get_PSP_DIRECTORY_from_environ()
+            psp_directory = get_PSP_DIRECTORY_from_environ()
 
         self._psp_directory = psp_directory
 
         if psp_directory is None or self._psp_cutoff_table is None:
             warn(
                 "psp_directory not provided XS_PSP_DIRECTORY not in the "
                 "current environment variables OR psp_cutoff_table not "
@@ -385,21 +388,21 @@
             # use Gamma point for ground state calculations (es.in and gs.in)
             kpoints_scf = [1, 1, 1]
         else:
             kpoints_scf = self._kpoints(structure)
 
         kpoints_xas = self._kpoints(structure)
 
-        self._cards["XS"]["kpts"][
-            "kpts"
-        ] = f"{kpoints_xas[0]} {kpoints_xas[1]} {kpoints_xas[2]}"
+        self._cards["XS"]["kpts"]["kpts"] = (
+            f"{kpoints_xas[0]} {kpoints_xas[1]} {kpoints_xas[2]}"
+        )
         # Determine the SCF? convergence threshold
-        self._cards["QE"]["electrons"][
-            "conv_thr"
-        ] = self._defaultConvPerAtom * len(structure)
+        self._cards["QE"]["electrons"]["conv_thr"] = (
+            self._defaultConvPerAtom * len(structure)
+        )
         # Get the psp data ready for the GS calculations; similar to SCF
         # (neutral) calculations in VASP
         # need to treat three different cases here
 
         ecutwfc = self._cards["QE"]["system"]["ecutwfc"]
         ecutrho = self._cards["QE"]["system"]["ecutrho"]
```

### Comparing `lightshow-1.2.2/lightshow/postprocess/broaden.py` & `lightshow-1.2.3/lightshow/postprocess/broaden.py`

 * *Files identical despite different names*

### Comparing `lightshow-1.2.2/lightshow/postprocess/compare_utils.py` & `lightshow-1.2.3/lightshow/postprocess/compare_utils.py`

 * *Files identical despite different names*

### Comparing `lightshow-1.2.2/lightshow/postprocess/parse.py` & `lightshow-1.2.3/lightshow/postprocess/parse.py`

 * *Files identical despite different names*

### Comparing `lightshow-1.2.2/lightshow/pymatgen_utils.py` & `lightshow-1.2.3/lightshow/pymatgen_utils.py`

 * *Files identical despite different names*

### Comparing `lightshow-1.2.2/notebooks/00_basic_usage.ipynb` & `lightshow-1.2.3/notebooks/00_basic_usage.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9982592617270789%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(4, '📝 **Note:** You can find our JOSS manuscript here: "*

 * *            "https://doi.org/10.21105/joss.05182\\n')], delete: [4]}}, 15: {'metadata': {replace: "*

 * *            "OrderedDict([('tags', [])])}}, 35: {'source': {insert: [(3, '    "*

 * *            "force_spin_unpolarized=True,\\n')], delete: [3]}}}",*

 * * "'metadata'": "{'language_info': {'version': '3.11.6'}}"}*

```diff
@@ -13,15 +13,15 @@
             "id": "07834dfe-a6e2-498f-99d7-744aee18474b",
             "metadata": {},
             "source": [
                 "The [Lightshow](https://github.com/AI-multimodal/Lightshow) software package is a one-stop-shop for writing computational spectroscopy input files. In this tutorial, we'll show you how to initialize a `Database` object from the Materials Project, and use that database to write input files for the FEFF, VASP, EXCITING, Xspectra and OCEAN codes.\n",
                 "\n",
                 "\ud83d\udcdd **Note:** This notebook is a tutorial designed to be run via online hosting services, but you can of course run it locally, it just might require a few modifications.\n",
                 "\n",
-                "\ud83d\udcdd **Note:** You can find our arXiv Preprint here: https://arxiv.org/abs/2211.04452.\n",
+                "\ud83d\udcdd **Note:** You can find our JOSS manuscript here: https://doi.org/10.21105/joss.05182\n",
                 "\n",
                 "\u26a0\ufe0f **Important Note:** In order to pull data from the Materials Project, you will have to setup an API key. Lightshow currently uses the v2 API of the Materials Project, and you can find the instructions on how to get an API key here: https://materialsproject.org/api."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
@@ -172,15 +172,17 @@
                 "sys.path.append(\"..\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "1e52ffc5-4209-47af-964b-e9d3401480f2",
-            "metadata": {},
+            "metadata": {
+                "tags": []
+            },
             "outputs": [],
             "source": [
                 "import lightshow\n",
                 "from lightshow import Database\n",
                 "print(lightshow.__version__)"
             ]
         },
@@ -447,15 +449,15 @@
             "id": "becea3c2-6098-4a3a-9baa-18c4a7ae5bda",
             "metadata": {},
             "outputs": [],
             "source": [
                 "vasp_params_corehole = VASPParameters(\n",
                 "    incar=VASP_INCAR_DEFAULT_COREHOLE_POTENTIAL,\n",
                 "    potcar_directory=None,\n",
-                "    force_spin_unpolarized=False,\n",
+                "    force_spin_unpolarized=True,\n",
                 "    kpoints=lightshow.common.kpoints.GenericEstimatorKpoints(cutoff=43),\n",
                 "    nbands=lightshow.common.nbands.UnitCellVolumeEstimate(e_range=40)\n",
                 ")"
             ]
         },
         {
             "cell_type": "markdown",
@@ -865,14 +867,14 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.16"
+            "version": "3.11.6"
         },
         "toc-autonumbering": true
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `lightshow-1.2.2/notebooks/01_Ti_K_anatase_broaden.ipynb` & `lightshow-1.2.3/notebooks/01_Ti_K_anatase_broaden.ipynb`

 * *Files identical despite different names*

### Comparing `lightshow-1.2.2/notebooks/compare_spectra.ipynb` & `lightshow-1.2.3/notebooks/compare_spectra.ipynb`

 * *Files identical despite different names*

### Comparing `lightshow-1.2.2/notebooks/parse_spectra.ipynb` & `lightshow-1.2.3/notebooks/parse_spectra.ipynb`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9589947089947091%*

 * *Differences: {"'cells'": "{0: {'cell_type': 'markdown', 'id': 'f604d3ea-13ed-4cba-a633-03604abf7897', 'source': "*

 * *            "['# Parse spectral results'], delete: ['execution_count', 'outputs']}, 1: {'id': "*

 * *            "'6eac0404-521b-43a0-b0b7-ce61b4f2cf33', 'source': ['import numpy as np\\n', 'import "*

 * *            "sys\\n', 'import matplotlib.pyplot as plt']}, 2: {'id': "*

 * *            "'ee479958-90c2-4467-8e15-5aaf17eaa098', 'source': ['!pip install lightshow']}, 4: "*

 * *            "{'source': ['from lightshow.postpro […]*

```diff
@@ -1,65 +1,55 @@
 {
     "cells": [
         {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "6eac0404-521b-43a0-b0b7-ce61b4f2cf33",
+            "cell_type": "markdown",
+            "id": "f604d3ea-13ed-4cba-a633-03604abf7897",
             "metadata": {},
-            "outputs": [],
             "source": [
-                "import numpy as np "
+                "# Parse spectral results"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "8e382f34-7957-4efc-8f41-a2fe6e473e09",
+            "id": "6eac0404-521b-43a0-b0b7-ce61b4f2cf33",
             "metadata": {},
             "outputs": [],
             "source": [
-                "import sys"
+                "import numpy as np\n",
+                "import sys\n",
+                "import matplotlib.pyplot as plt"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "3adc5640-4a1a-4c1e-989f-f36b3b78ed29",
+            "id": "ee479958-90c2-4467-8e15-5aaf17eaa098",
             "metadata": {},
             "outputs": [],
             "source": [
-                "import matplotlib.pyplot as plt"
+                "!pip install lightshow"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "a2c1b545-ab9b-4c68-a580-fd7d250e7dba",
             "metadata": {},
             "source": [
                 "###### Please change directory"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "58919792-0445-4008-90f1-0ae07b26ea97",
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "sys.path.append('/sdcc/u/ccao/scripts/Lightshow-master/lightshow')"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
             "id": "c68156ee-66b5-4576-abb7-1e2ca97e72f0",
             "metadata": {},
             "outputs": [],
             "source": [
-                "from postprocess.parse import *"
+                "from lightshow.postprocess import parse"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "01b19c95-d2e1-44bb-82ab-ac11ea12c6c1",
             "metadata": {},
@@ -75,19 +65,19 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "c9f254cf-46f9-4cbc-865a-3be8dcaf0ee8",
             "metadata": {},
             "outputs": [],
             "source": [
-                "dict_feff = extract_FEFF(path_feff)\n",
-                "dict_vasp = extract_VASP(path_vasp)\n",
-                "dict_xs = extract_XSpectra(path_xs, es_out_file='./data_parse_spectra/mp-1203/XSPECTRA/es_0.out')\n",
-                "dict_ocean = extract_OCEAN(path_ocean, scf_out_file='./data_parse_spectra/mp-1203/OCEAN/scf.out')\n",
-                "dict_exciting = extract_exciting(path_exciting, INFO_out_file='./data_parse_spectra/mp-1203/EXCITING/INFO.OUT')"
+                "dict_feff = parse.extract_FEFF(path_feff)\n",
+                "dict_vasp = parse.extract_VASP(path_vasp)\n",
+                "dict_xs = parse.extract_XSpectra(path_xs, es_out_file='./data_parse_spectra/mp-1203/XSPECTRA/es_0.out')\n",
+                "dict_ocean = parse.extract_OCEAN(path_ocean, scf_out_file='./data_parse_spectra/mp-1203/OCEAN/scf.out')\n",
+                "dict_exciting = parse.extract_exciting(path_exciting, INFO_out_file='./data_parse_spectra/mp-1203/EXCITING/INFO.OUT')"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "5e86a6b0-925d-48d3-bd0c-07a81ac3c621",
             "metadata": {},
@@ -195,47 +185,31 @@
                 "plt.plot(dict_exciting['energy'],dict_exciting['spectrum'], label='spectrum')\n",
                 "plt.plot(dict_exciting['energy'],dict_exciting['11']-1e-6, label='11')\n",
                 "plt.plot(dict_exciting['energy'],dict_exciting['22']-2e-6, label='22')\n",
                 "plt.plot(dict_exciting['energy'],dict_exciting['33']-3e-6, label='33')\n",
                 "plt.title('exciting')\n",
                 "plt.legend()"
             ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "303680c6-afa7-492f-8ce4-fb89f8942c64",
-            "metadata": {},
-            "outputs": [],
-            "source": []
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "4aeb9531-4efa-44b0-87bf-1c57cff3ad56",
-            "metadata": {},
-            "outputs": [],
-            "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "kernel_chuntian",
+            "display_name": "Python 3 (ipykernel)",
             "language": "python",
-            "name": "kernel_chuntian"
+            "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.8.5"
+            "version": "3.9.16"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `lightshow-1.2.2/notebooks/spectra_files/anatase_exciting.txt` & `lightshow-1.2.3/notebooks/spectra_files/anatase_exciting.txt`

 * *Files identical despite different names*

### Comparing `lightshow-1.2.2/notebooks/spectra_files/anatase_exp.txt` & `lightshow-1.2.3/notebooks/spectra_files/anatase_exp.txt`

 * *Files identical despite different names*

### Comparing `lightshow-1.2.2/notebooks/spectra_files/anatase_ocean.txt` & `lightshow-1.2.3/notebooks/spectra_files/anatase_ocean.txt`

 * *Files identical despite different names*

### Comparing `lightshow-1.2.2/notebooks/spectra_files/anatase_theory_FEFF.txt` & `lightshow-1.2.3/notebooks/spectra_files/anatase_theory_FEFF.txt`

 * *Files identical despite different names*

### Comparing `lightshow-1.2.2/notebooks/spectra_files/anatase_theory_VASP.txt` & `lightshow-1.2.3/notebooks/spectra_files/anatase_theory_VASP.txt`

 * *Files identical despite different names*

### Comparing `lightshow-1.2.2/notebooks/spectra_files/anatase_xspectra.txt` & `lightshow-1.2.3/notebooks/spectra_files/anatase_xspectra.txt`

 * *Files identical despite different names*

### Comparing `lightshow-1.2.2/pyproject.toml` & `lightshow-1.2.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -31,16 +31,16 @@
     "Topic :: Scientific/Engineering",
     "Intended Audience :: Developers",
     "Intended Audience :: Education",
     "Intended Audience :: Science/Research",
 ]
 dependencies = [
     "numpy==1.26.4",
-    "pymatgen==2024.2.23",
-    "mp-api==0.41.1",
+    "pymatgen==2024.3.1",
+    "mp-api==0.41.2",
     "ase",
     "tqdm",
     "monty"
 ]
 
 # Dynamic version reads __version__ directly from my_package.__init__
 dynamic = ["version"]
@@ -51,42 +51,37 @@
 #     "docs"
 # ]
 
 [project.optional-dependencies]
 test = [
     "coverage",
     "flake8",
+    "ruff",
     "pytest",
     "pytest-cov",
-    "black",
     "nbstripout",
     "pre-commit",
 ]
 doc = [
     "sphinx",
     "numpydoc",
     "sphinx-copybutton",
     "sphinx_rtd_theme",
     "ipython",
     "matplotlib"
 ]
+build = [
+    "flit~=3.7",
+    "dunamai==1.19.2",
+]
 
 [tool.setuptools]
 packages = ["lightshow"]
 
-[tool.black]
+[tool.ruff]
 line-length = 80
-include = '\.pyi?$'
-exclude = '''
-/(
-  | \.git
-  | \.hg
-  | \.mypy_cache
-  | \.tox
-  | \.venv
-  | _build
-  | buck-out
-  | build
-  | dist
-  | docs/source/conf.py
-)/
-'''
+
+[tool.ruff.format]
+quote-style = "double"
+indent-style = "space"
+docstring-code-format = true
+docstring-code-line-length = 60
```

### Comparing `lightshow-1.2.2/scripts/README.rst` & `lightshow-1.2.3/scripts/README.rst`

 * *Files identical despite different names*

### Comparing `lightshow-1.2.2/scripts/build_docs.sh` & `lightshow-1.2.3/scripts/build_docs.sh`

 * *Files identical despite different names*

### Comparing `lightshow-1.2.2/scripts/update_version.sh` & `lightshow-1.2.3/scripts/update_version.sh`

 * *Files identical despite different names*

### Comparing `lightshow-1.2.2/PKG-INFO` & `lightshow-1.2.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightshow
-Version: 1.2.2
+Version: 1.2.3
 Summary: A one-stop-shop for writing computational spectroscopy input files
 Author: Benedikt Maurer, Fabien Peschel, Eli Stavitski, Xiaohui Qu, John T. Vinson, Christian Vorwerk
 Author-email: "Matthew R. Carbone" <mcarbone@bnl.gov>, Fanchen Meng <fmeng1@bnl.gov>, Deyu Lu <dlu@bnl.gov>
 Maintainer-email: "Matthew R. Carbone" <mcarbone@bnl.gov>, Fanchen Meng <fmeng1@bnl.gov>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -12,44 +12,47 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Requires-Dist: numpy==1.26.4
-Requires-Dist: pymatgen==2024.2.23
-Requires-Dist: mp-api==0.41.1
+Requires-Dist: pymatgen==2024.3.1
+Requires-Dist: mp-api==0.41.2
 Requires-Dist: ase
 Requires-Dist: tqdm
 Requires-Dist: monty
+Requires-Dist: flit~=3.7 ; extra == "build"
+Requires-Dist: dunamai==1.19.2 ; extra == "build"
 Requires-Dist: sphinx ; extra == "doc"
 Requires-Dist: numpydoc ; extra == "doc"
 Requires-Dist: sphinx-copybutton ; extra == "doc"
 Requires-Dist: sphinx_rtd_theme ; extra == "doc"
 Requires-Dist: ipython ; extra == "doc"
 Requires-Dist: matplotlib ; extra == "doc"
 Requires-Dist: coverage ; extra == "test"
 Requires-Dist: flake8 ; extra == "test"
+Requires-Dist: ruff ; extra == "test"
 Requires-Dist: pytest ; extra == "test"
 Requires-Dist: pytest-cov ; extra == "test"
-Requires-Dist: black ; extra == "test"
 Requires-Dist: nbstripout ; extra == "test"
 Requires-Dist: pre-commit ; extra == "test"
+Provides-Extra: build
 Provides-Extra: doc
 Provides-Extra: test
 
 <div align="center">
     
 ![sysfs line plot](https://raw.githubusercontent.com/AI-multimodal/Lightshow/master/docs/_static/images/lightshow.jpg)
 
 [![image](https://joss.theoj.org/papers/a9cabcd7f4b85a926a797997c6622b43/status.svg)](https://joss.theoj.org/papers/a9cabcd7f4b85a926a797997c6622b43)
 [![image](https://github.com/AI-multimodal/Lightshow/actions/workflows/ci.yml/badge.svg)](https://github.com/AI-multimodal/Lightshow/actions/workflows/ci.yml)
 [![image](https://codecov.io/gh/AI-multimodal/Lightshow/branch/master/graph/badge.svg?token=CW7BMFA5O7)](https://codecov.io/gh/AI-multimodal/Lightshow)
 [![image](https://app.codacy.com/project/badge/Grade/d31a4e18672c4d71bbaafa719181c140)](https://www.codacy.com/gh/AI-multimodal/Lightshow/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=AI-multimodal/Lightshow&amp;utm_campaign=Badge_Grade) <br>
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 [![python](https://img.shields.io/badge/-Python_3.9+-blue?logo=python&logoColor=white)](https://github.com/pre-commit/pre-commit)
 [![Downloads](https://static.pepy.tech/badge/lightshow)](https://pepy.tech/project/lightshow)
 </div>
     
 ------------------------------------------------------------------------
 
 **Lightshow** is a Python library for easily generating computational
```

