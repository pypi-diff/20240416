# Comparing `tmp/pylemur-0.1.0.tar.gz` & `tmp/pylemur-0.2.0.tar.gz`

## Comparing `pylemur-0.1.0.tar` & `pylemur-0.2.0.tar`

### file list

```diff
@@ -1,53 +1,51 @@
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 pylemur-0.1.0/.codecov.yaml
--rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 pylemur-0.1.0/.cruft.json
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 pylemur-0.1.0/.editorconfig
--rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 pylemur-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 pylemur-0.1.0/.readthedocs.yaml
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 pylemur-0.1.0/CHANGELOG.md
--rw-r--r--   0        0        0     3080 2020-02-02 00:00:00.000000 pylemur-0.1.0/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 pylemur-0.1.0/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 pylemur-0.1.0/.github/ISSUE_TEMPLATE/feature_request.yml
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 pylemur-0.1.0/.github/workflows/build.yaml
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 pylemur-0.1.0/.github/workflows/release.yaml
--rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 pylemur-0.1.0/.github/workflows/test.yaml
--rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 pylemur-0.1.0/docs/Makefile
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 pylemur-0.1.0/docs/api.md
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 pylemur-0.1.0/docs/changelog.md
--rw-r--r--   0        0        0     4276 2020-02-02 00:00:00.000000 pylemur-0.1.0/docs/conf.py
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 pylemur-0.1.0/docs/index.md
--rw-r--r--   0        0        0     2014 2020-02-02 00:00:00.000000 pylemur-0.1.0/docs/references.bib
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 pylemur-0.1.0/docs/references.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pylemur-0.1.0/docs/_static/.gitkeep
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 pylemur-0.1.0/docs/_static/css/custom.css
--rw-r--r--   0        0        0    69769 2020-02-02 00:00:00.000000 pylemur-0.1.0/docs/_static/images/equation_schematic.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pylemur-0.1.0/docs/_templates/.gitkeep
--rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 pylemur-0.1.0/docs/_templates/autosummary/class.rst
--rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 pylemur-0.1.0/docs/extensions/typed_returns.py
--rw-r--r--   0        0        0  1110593 2020-02-02 00:00:00.000000 pylemur-0.1.0/docs/notebooks/Tutorial.ipynb
--rw-r--r--   0        0        0     7844 2020-02-02 00:00:00.000000 pylemur-0.1.0/docs/notebooks/Tutorial.qmd
--rw-r--r--   0        0        0     1970 2020-02-02 00:00:00.000000 pylemur-0.1.0/notebooks/check_implementation.qmd
--rw-r--r--   0        0        0     2437 2020-02-02 00:00:00.000000 pylemur-0.1.0/notebooks/devel_experiments.qmd
--rw-r--r--   0        0        0     1790 2020-02-02 00:00:00.000000 pylemur-0.1.0/notebooks/kang_analysis_in_R.qmd
--rw-r--r--   0        0        0     2815 2020-02-02 00:00:00.000000 pylemur-0.1.0/notebooks/lemur_model_experiments.qmd
--rw-r--r--   0        0        0     4593 2020-02-02 00:00:00.000000 pylemur-0.1.0/notebooks/scanpy_experiments.qmd
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 pylemur-0.1.0/src/pylemur/__init__.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 pylemur-0.1.0/src/pylemur/pl/__init__.py
--rw-r--r--   0        0        0     1212 2020-02-02 00:00:00.000000 pylemur-0.1.0/src/pylemur/pl/basic.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pylemur-0.1.0/src/pylemur/pp/__init__.py
--rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 pylemur-0.1.0/src/pylemur/pp/basic.py
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 pylemur-0.1.0/src/pylemur/tl/__init__.py
--rw-r--r--   0        0        0     2704 2020-02-02 00:00:00.000000 pylemur-0.1.0/src/pylemur/tl/_design_matrix_utils.py
--rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 pylemur-0.1.0/src/pylemur/tl/_grassmann.py
--rw-r--r--   0        0        0     3906 2020-02-02 00:00:00.000000 pylemur-0.1.0/src/pylemur/tl/_grassmann_lm.py
--rw-r--r--   0        0        0     2796 2020-02-02 00:00:00.000000 pylemur-0.1.0/src/pylemur/tl/_lin_alg_wrappers.py
--rw-r--r--   0        0        0     9553 2020-02-02 00:00:00.000000 pylemur-0.1.0/src/pylemur/tl/alignment.py
--rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 pylemur-0.1.0/src/pylemur/tl/lemur.py
--rw-r--r--   0        0        0     5648 2020-02-02 00:00:00.000000 pylemur-0.1.0/src/pylemur/tl/predict.py
--rw-r--r--   0        0        0     3504 2020-02-02 00:00:00.000000 pylemur-0.1.0/tests/test_grasmann_lm.py
--rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 pylemur-0.1.0/tests/test_grassmann.py
--rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 pylemur-0.1.0/tests/test_lin_alg_utils.py
--rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 pylemur-0.1.0/.gitignore
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 pylemur-0.1.0/LICENSE
--rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 pylemur-0.1.0/README.md
--rw-r--r--   0        0        0     3447 2020-02-02 00:00:00.000000 pylemur-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     4845 2020-02-02 00:00:00.000000 pylemur-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 pylemur-0.2.0/.codecov.yaml
+-rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 pylemur-0.2.0/.cruft.json
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 pylemur-0.2.0/.editorconfig
+-rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 pylemur-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 pylemur-0.2.0/.readthedocs.yaml
+-rw-r--r--   0        0        0     1007 2020-02-02 00:00:00.000000 pylemur-0.2.0/CHANGELOG.md
+-rw-r--r--   0        0        0     3080 2020-02-02 00:00:00.000000 pylemur-0.2.0/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 pylemur-0.2.0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 pylemur-0.2.0/.github/ISSUE_TEMPLATE/feature_request.yml
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 pylemur-0.2.0/.github/workflows/build.yaml
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 pylemur-0.2.0/.github/workflows/release.yaml
+-rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 pylemur-0.2.0/.github/workflows/test.yaml
+-rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 pylemur-0.2.0/docs/Makefile
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 pylemur-0.2.0/docs/api.md
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 pylemur-0.2.0/docs/changelog.md
+-rw-r--r--   0        0        0     4392 2020-02-02 00:00:00.000000 pylemur-0.2.0/docs/conf.py
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 pylemur-0.2.0/docs/index.md
+-rw-r--r--   0        0        0     2014 2020-02-02 00:00:00.000000 pylemur-0.2.0/docs/references.bib
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 pylemur-0.2.0/docs/references.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pylemur-0.2.0/docs/_static/.gitkeep
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 pylemur-0.2.0/docs/_static/css/custom.css
+-rw-r--r--   0        0        0    69769 2020-02-02 00:00:00.000000 pylemur-0.2.0/docs/_static/images/equation_schematic.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pylemur-0.2.0/docs/_templates/.gitkeep
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 pylemur-0.2.0/docs/_templates/autosummary/class.rst
+-rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 pylemur-0.2.0/docs/extensions/typed_returns.py
+-rw-r--r--   0        0        0     8445 2020-02-02 00:00:00.000000 pylemur-0.2.0/docs/notebooks/Tutorial.myst
+-rw-r--r--   0        0        0     1940 2020-02-02 00:00:00.000000 pylemur-0.2.0/notebooks/check_implementation.qmd
+-rw-r--r--   0        0        0     2437 2020-02-02 00:00:00.000000 pylemur-0.2.0/notebooks/devel_experiments.qmd
+-rw-r--r--   0        0        0     1790 2020-02-02 00:00:00.000000 pylemur-0.2.0/notebooks/kang_analysis_in_R.qmd
+-rw-r--r--   0        0        0     2815 2020-02-02 00:00:00.000000 pylemur-0.2.0/notebooks/lemur_model_experiments.qmd
+-rw-r--r--   0        0        0     4593 2020-02-02 00:00:00.000000 pylemur-0.2.0/notebooks/scanpy_experiments.qmd
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 pylemur-0.2.0/src/pylemur/__init__.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 pylemur-0.2.0/src/pylemur/pl/__init__.py
+-rw-r--r--   0        0        0     1212 2020-02-02 00:00:00.000000 pylemur-0.2.0/src/pylemur/pl/basic.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pylemur-0.2.0/src/pylemur/pp/__init__.py
+-rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 pylemur-0.2.0/src/pylemur/pp/basic.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 pylemur-0.2.0/src/pylemur/tl/__init__.py
+-rw-r--r--   0        0        0     2806 2020-02-02 00:00:00.000000 pylemur-0.2.0/src/pylemur/tl/_design_matrix_utils.py
+-rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 pylemur-0.2.0/src/pylemur/tl/_grassmann.py
+-rw-r--r--   0        0        0     3939 2020-02-02 00:00:00.000000 pylemur-0.2.0/src/pylemur/tl/_grassmann_lm.py
+-rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 pylemur-0.2.0/src/pylemur/tl/_lin_alg_wrappers.py
+-rw-r--r--   0        0        0     5635 2020-02-02 00:00:00.000000 pylemur-0.2.0/src/pylemur/tl/alignment.py
+-rw-r--r--   0        0        0    19188 2020-02-02 00:00:00.000000 pylemur-0.2.0/src/pylemur/tl/lemur.py
+-rw-r--r--   0        0        0     3561 2020-02-02 00:00:00.000000 pylemur-0.2.0/tests/test_grasmann_lm.py
+-rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 pylemur-0.2.0/tests/test_grassmann.py
+-rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 pylemur-0.2.0/tests/test_lin_alg_utils.py
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 pylemur-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 pylemur-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 pylemur-0.2.0/README.md
+-rw-r--r--   0        0        0     3447 2020-02-02 00:00:00.000000 pylemur-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4845 2020-02-02 00:00:00.000000 pylemur-0.2.0/PKG-INFO
```

### Comparing `pylemur-0.1.0/.cruft.json` & `pylemur-0.2.0/.cruft.json`

 * *Files identical despite different names*

### Comparing `pylemur-0.1.0/.pre-commit-config.yaml` & `pylemur-0.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pylemur-0.1.0/.github/ISSUE_TEMPLATE/bug_report.yml` & `pylemur-0.2.0/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `pylemur-0.1.0/.github/workflows/build.yaml` & `pylemur-0.2.0/.github/workflows/build.yaml`

 * *Files identical despite different names*

### Comparing `pylemur-0.1.0/.github/workflows/release.yaml` & `pylemur-0.2.0/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `pylemur-0.1.0/.github/workflows/test.yaml` & `pylemur-0.2.0/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `pylemur-0.1.0/docs/Makefile` & `pylemur-0.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pylemur-0.1.0/docs/conf.py` & `pylemur-0.2.0/docs/conf.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 urls = dict(pu.split(", ") for pu in info.get_all("Project-URL"))
 repository_url = urls["Source"]
 
 # The full version, including alpha/beta/rc tags
 release = info["Version"]
 
 bibtex_bibfiles = ["references.bib"]
-bibtex_default_style = 'unsrt'
+bibtex_default_style = "unsrt"
 
 templates_path = ["_templates"]
 nitpicky = True  # Warn about broken links
 needs_sphinx = "4.0"
 
 html_context = {
     "display_github": True,  # Integrate GitHub
@@ -69,27 +69,29 @@
 autodoc_member_order = "groupwise"
 default_role = "literal"
 napoleon_google_docstring = False
 napoleon_numpy_docstring = True
 napoleon_include_init_with_doc = False
 napoleon_use_rtype = True  # having a separate entry generally helps readability
 napoleon_use_param = True
+napoleon_use_ivar = True
+
 
 myst_heading_anchors = 6  # create anchors for h1-h6
 myst_enable_extensions = [
     "amsmath",
     "colon_fence",
     "deflist",
     "dollarmath",
     "html_image",
     "html_admonition",
 ]
 myst_url_schemes = ("http", "https", "mailto")
 nb_output_stderr = "remove"
-nb_execution_mode = "off"
+nb_execution_mode = "auto"
 nb_merge_streams = True
 typehints_defaults = "braces"
 
 source_suffix = {
     ".rst": "restructuredtext",
     ".ipynb": "myst-nb",
     ".myst": "myst-nb",
@@ -98,14 +100,15 @@
 intersphinx_mapping = {
     "python": ("https://docs.python.org/3", None),
     "anndata": ("https://anndata.readthedocs.io/en/stable/", None),
     "numpy": ("https://numpy.org/doc/stable/", None),
     "pandas": ("https://pandas.pydata.org/pandas-docs/stable/", None),
     "scipy": ("https://docs.scipy.org/doc/scipy/", None),
     "sklearn": ("https://scikit-learn.org/stable/", None),
+    # "formulaic": ("https://matthewwardrop.github.io/formulaic/", None) # Doesn't work.
 }
 
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This pattern also affects html_static_path and html_extra_path.
 exclude_patterns = ["_build", "Thumbs.db", ".DS_Store", "**.ipynb_checkpoints"]
```

### Comparing `pylemur-0.1.0/docs/references.bib` & `pylemur-0.2.0/docs/references.bib`

 * *Files identical despite different names*

### Comparing `pylemur-0.1.0/docs/_static/images/equation_schematic.png` & `pylemur-0.2.0/docs/_static/images/equation_schematic.png`

 * *Files identical despite different names*

### Comparing `pylemur-0.1.0/docs/_templates/autosummary/class.rst` & `pylemur-0.2.0/docs/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `pylemur-0.1.0/docs/extensions/typed_returns.py` & `pylemur-0.2.0/docs/extensions/typed_returns.py`

 * *Files identical despite different names*

### Comparing `pylemur-0.1.0/docs/notebooks/Tutorial.qmd` & `pylemur-0.2.0/docs/notebooks/Tutorial.myst`

 * *Files 11% similar despite different names*

```diff
@@ -1,193 +1,190 @@
 ---
-title: pyLemur Walkthrough
-date: today
-authors: Constantin Ahlmann-Eltze
-bibliography: ../references.bib
-format: 
-    ipynb:
-        toc: true
-        fig-format: retina
-        df-print: default
-        standalone: false
-execute: 
-  enabled: true
-jupyter: python3
+file_format: mystnb
+mystnb:
+    execution_timeout: 600
+kernelspec:
+  name: python3
 ---
 
+# pyLemur Walkthrough
+
 
 The goal of `pyLemur` is to simplify analysis of multi-condition single-cell data. If you have collected a single-cell RNA-seq dataset with more than one condition, lemur predicts for each cell and gene how much the expression would change if the cell had been in the other condition.
 
 `pyLemur` is a Python implementation of the LEMUR model; there is also an `R` package called [lemur](https://bioconductor.org/packages/lemur/) which provides additional functionality: identifying neighborhoods of cells that show consistent differential expression values and a pseudo-bulk test to validate the findings.
 
-`pyLemur` implements a novel framework to disentangle the effects of known covariates, latent cell states, and their interactions. At the core, is a combination of matrix factorization and regression analysis implemented as geodesic regression on Grassmann manifolds. We call this latent embedding multivariate regression. For more details see our [preprint](https://www.biorxiv.org/content/10.1101/2023.03.06.531268) [@Ahlmann-Eltze2024].
+`pyLemur` implements a novel framework to disentangle the effects of known covariates, latent cell states, and their interactions. At the core, is a combination of matrix factorization and regression analysis implemented as geodesic regression on Grassmann manifolds. We call this latent embedding multivariate regression. For more details see our [preprint](https://www.biorxiv.org/content/10.1101/2023.03.06.531268) {cite:p}`Ahlmann-Eltze2024`.
 
 <img src="../_static/images/equation_schematic.png" alt="Schematic of the matrix decomposition atthe core of LEMUR" />
 
 
 ## Data
 
-For demonstration, I will use the a dataset of interferon-$\beta$ stimuted blood cells from @kang2018.
+For demonstration, I will use the a dataset of interferon-$\beta$ stimuted blood cells from {cite:t}`kang2018`.
 
-```{python}
-#| label: import-data
-#| warning: false
+```{code-cell} ipython3
+---
+output_stderr: remove
+---
 # Standard imports
 import numpy as np
 import scanpy as sc
 # pertpy is need to download the kang data
 import pertpy 
 
 # This will download the data to ./data/kang_2018.h5ad
 adata = pertpy.data.kang_2018()
 # Store counts separately in the layers
 adata.layers["counts"] = adata.X.copy()
 ```
 
 The data consist of $24\,673$ cells and $15\,706$ genes. The cells were measured in two conditions (`label="ctrl"` and `label="stim"`). The authors have annotated the cell type for each cell. This will be useful to analyze LEMUR's results, but the cell type labels are not actually used to the LEMUR model.
 
-```{python}
-#| label: pandas-print-settings
-#| echo: false
+```{code-cell} ipython3
+:tags: ["remove-cell"]
 import pandas as pd
 pd.options.display.width = 200
 pd.options.display.max_colwidth = 20
 ```
 
-```{python}
-#| label: data-overview
+```{code-cell} ipython3
 print(adata)
 print(adata.obs)
 ```
 
 ## Preprocessing
 
 LEMUR expects that the input has been variance-stabilized. Here, I will use the log-transformation as a simple, yet effective approach.
 In addition, I will select the $1\,000$ most variable genes, to make the results easier to manage.
-```{python}
-#| label: standard-preprocessing
+```{code-cell} ipython3
 # This follows the standard recommendation from scanpy 
 sc.pp.normalize_total(adata, target_sum = 1e4, inplace=True)
 sc.pp.log1p(adata)
 adata.layers["logcounts"] = adata.X.copy()
 sc.pp.highly_variable_genes(adata, n_top_genes=1000, flavor="cell_ranger")
 adata = adata[:, adata.var.highly_variable]
 adata
 ```
 
 If we make a dimensional-embedding of the data using UMAP, we see that the cell types split-up by treatment status.
-```{python}
+```{code-cell} ipython3
 #| label: fig-raw-umap
 sc.tl.pca(adata)
 sc.pp.neighbors(adata)
 sc.tl.umap(adata)
 sc.pl.umap(adata, color=["label", "cell_type"])
 ```
 
 
 ## LEMUR
 
 First, we import `pyLemur`; then, we fit the LEMUR model by providing the `AnnData` object, a specification of the experimental design, and the number of latent dimensions.
 
-```{python}
-#| label: fit-lemur
+```{code-cell} ipython3
 import pylemur
-fit = pylemur.tl.lemur(adata, design = "~ label", n_embedding=15)
-fit = pylemur.tl.align_with_harmony(fit, verbose=False)
+model = pylemur.tl.LEMUR(adata, design = "~ label", n_embedding=15)
+model.fit()
+model.align_with_harmony()
+print(model)
 ```
 
 To assess the success of the LEMUR model fit, we plot a UMAP representation of the embedding calculated by LEMUR. Here, the two conditions are mixed and the different cell types and cell states drive the visible variation.
-```{python}
-#| label: fig-plot-lemur
+```{code-cell} ipython3
 # Recalculate the UMAP embedding on calculated by LEMUR
-sc.pp.neighbors(fit, use_rep="embedding")
-sc.tl.umap(fit)
-sc.pl.umap(fit, color=["label", "cell_type"])
+adata.obsm["embedding"] = model.embedding
+sc.pp.neighbors(adata, use_rep="embedding")
+sc.tl.umap(adata)
+sc.pl.umap(adata, color=["label", "cell_type"])
 ```
 
 The LEMUR model is fully parametric, which means that we can predict for each cell what it's expression would have been in any condition (i.e., for a cell observed in the control condition, we can predict its expression under treatment), as a function of its low-dimensional embedding.
 
-```{python}
-#| label: predict-expression
-ctrl_pred = pylemur.tl.predict(fit, new_condition=pylemur.tl.cond(fit, label="ctrl"))
-stim_pred = pylemur.tl.predict(fit, new_condition=pylemur.tl.cond(fit, label="stim"))
+```{code-cell} ipython3
+ctrl_pred = model.predict(new_condition=model.cond(label="ctrl"))
+stim_pred = model.predict(new_condition=model.cond(label="stim"))
 ```
 
 We can now check the predicted differential expression against the underlying observed expression patterns for individual genes.
-```{python}
-#| label: fig-example-gene-expr
+```{code-cell} ipython3
 import matplotlib.pyplot as plt
-fit.layers["diff"] = stim_pred - ctrl_pred
+adata.layers["diff"] = stim_pred - ctrl_pred
 sel_gene = "TNFRSF18"
 
 _,axs = plt.subplots(nrows = 1, ncols = 3)
-sc.pl.umap(fit, layer="diff", color=[sel_gene], cmap = plt.get_cmap("seismic"), vcenter=0,
+sc.pl.umap(adata, layer="diff", color=[sel_gene], cmap = plt.get_cmap("seismic"), vcenter=0,
     vmin = -0.5, vmax =0.5, title="Pred diff (ctrl - stim)", ax=axs[0], show=False)
-sc.pl.umap(fit[fit.obs["label"]=="ctrl"], layer="logcounts", color=[sel_gene], vmin = 0, vmax =4,
+sc.pl.umap(adata[adata.obs["label"]=="ctrl"], layer="logcounts", color=[sel_gene], vmin = 0, vmax =4,
     title="Ctrl expr", ax=axs[1], show=False)
-sc.pl.umap(fit[fit.obs["label"]=="stim"], layer="logcounts", color=[sel_gene], vmin = 0, vmax =4,
+sc.pl.umap(adata[adata.obs["label"]=="stim"], layer="logcounts", color=[sel_gene], vmin = 0, vmax =4,
     title="Stim expr", ax=axs[2])
 ```
 
 To assess the overall accuracy of LEMUR's predictions, I compare the average prediction per cell type across conditions. Genes on the diagonal don't change expression much between conditions, whereas all genes off-diagonal show differential expression within a cell type:
-```{python}
-#| label: fig-pred-raw
+```{code-cell} ipython3
 def rowMeans_per_group(X, group):
     uniq = np.unique(group)
     res = np.zeros((len(uniq), X.shape[1]))
     for i, e in enumerate(uniq):
         res[i,:] = X[group == e,:].sum(axis=0) / sum(group == e)
     return res
 
-fit_ctrl = fit[fit.obs["label"] == "ctrl",:]
-fit_stim = fit[fit.obs["label"] == "stim",:]
-ctrl_expr_per_cell_type = rowMeans_per_group(fit_ctrl.layers["logcounts"], fit_ctrl.obs["cell_type"])
-stim_expr_per_cell_type = rowMeans_per_group(fit_stim.layers["logcounts"], fit_stim.obs["cell_type"])
+adata_ctrl = adata[adata.obs["label"] == "ctrl",:]
+adata_stim = adata[adata.obs["label"] == "stim",:]
+ctrl_expr_per_cell_type = rowMeans_per_group(adata_ctrl.layers["logcounts"], adata_ctrl.obs["cell_type"])
+stim_expr_per_cell_type = rowMeans_per_group(adata_stim.layers["logcounts"], adata_stim.obs["cell_type"])
 obs_diff = stim_expr_per_cell_type - ctrl_expr_per_cell_type
 plt.scatter(ctrl_expr_per_cell_type, stim_expr_per_cell_type, c = obs_diff,
     cmap = plt.get_cmap("seismic"), vmin=-5, vmax=5, marker="o",edgecolors= "black")
 plt.colorbar()
 plt.title( "Inf-b stim. increases gene expression for many genes")
 plt.axline((0, 0), (1, 1), linewidth=1, color='black')
 ```
 
 Too check how well LEMUR learned the underlying expression relations, I predict the expression of cells from the control condition under stimulation, against the observed expression in the stimulated condition.
-```{python}
-#| label: fig-pred-accuracy
-stim_pred_per_cell_type = rowMeans_per_group(stim_pred[fit.obs["label"]=="ctrl"], fit_ctrl.obs["cell_type"])
+```{code-cell} ipython3
+stim_pred_per_cell_type = rowMeans_per_group(stim_pred[adata.obs["label"]=="ctrl"], adata_ctrl.obs["cell_type"])
 
 plt.scatter(stim_expr_per_cell_type, stim_pred_per_cell_type, c = obs_diff,
     cmap = plt.get_cmap("seismic"), vmin=-5, vmax=5, marker="o",edgecolors= "black")
 plt.colorbar()
 plt.title( "LEMUR's expression predictions are accurate")
 plt.axline((0, 0), (1, 1), linewidth=1, color='black')
 ```
 
 Lastly, I diretly, compare the predicted differential expression against the observed differential expression per cell type.
 
-```{python}
-#| label: fig-de-accuracy
-pred_diff = rowMeans_per_group(fit.layers["diff"], fit.obs["cell_type"])
+```{code-cell} ipython3
+pred_diff = rowMeans_per_group(adata.layers["diff"], adata.obs["cell_type"])
 
 plt.scatter(obs_diff, pred_diff, c = obs_diff,
     cmap = plt.get_cmap("seismic"), vmin=-5, vmax=5, marker="o",edgecolors= "black")
 plt.colorbar()
 plt.title( "LEMUR's DE predictions are accurate")
 plt.axline((0, 0), (1, 1), linewidth=1, color='black')
 ```
 
+Another advantage of LEMUR's parametricity is that you could also train the model on a subset of the data and then apply it to the full data. I train the same LEMUR model on 5% of the original data, `transform` the full data, and compare the first three dimensions of the embedding against the embedding from the model trained on the full model.
+```{code-cell} ipython3
+adata_subset = adata[np.random.choice(np.arange(adata.shape[0]), size = round(adata.shape[0] * 0.05)),]
+model_small = pylemur.tl.LEMUR(adata_subset, design = "~ label", n_embedding=15)
+model_small.fit().align_with_harmony()
+emb_proj = model_small.transform(adata)
+plt.scatter(emb_proj[:,0:3], model.embedding[:,0:3], s = 0.1)
+plt.axline((0, 0), (1, 1), linewidth=1, color='black')
+plt.axline((0, 0), (-1, 1), linewidth=1, color='black')
+```
 
 ### Session Info
 
-```{python}
-#| label: session-info
-#| code-fold: true
+```{code-cell} ipython3
 import session_info
 session_info.show()
 ```
 
 
-### References
-
-::: {#refs}
-:::
+### Referenes
 
+```{bibliography}
+:style: plain
+:filter: docname in docnames
+```
```

### Comparing `pylemur-0.1.0/notebooks/check_implementation.qmd` & `pylemur-0.2.0/notebooks/check_implementation.qmd`

 * *Files 12% similar despite different names*

```diff
@@ -42,21 +42,23 @@
 import pylemur.pp.basic
 adata.layers["logcounts"] = pylemur.pp.basic.shifted_log_transform(adata.X)
 adata = adata[:, pylemur.pp.basic.get_top_hvgs(adata, layer="logcounts", n=1000)]
 ```
 
 ```{python}
 import pylemur
-fit = pylemur.tl.lemur(adata, design = "~ label", n_embedding=15, layer = "logcounts")
-# fit = pylemur.tl.align_with_harmony(fit)
+model = pylemur.tl.LEMUR(adata, design = "~ label", n_embedding=15, layer = "logcounts")
+model.fit()
+model.align_with_harmony()
+print(model)
 ```
 
 ```{python}
-fit.obsm["embedding"][0:3, 0:3].T
-fit.obsm["embedding"][24600:24603,0:3].T
+model.embedding.shape
+model.adata
 ```
 
 ```{python}
 # groups = np.array([np.nan] * fit.shape[0])
 # groups[fit.obs["cell_type"] == "CD4 T cells"] = 1
 # groups[fit.obs["cell_type"] == "NK cells"] = 2
 # groups[fit.obs["cell_type"] == "Dendritic cells"] = 3
```

### Comparing `pylemur-0.1.0/notebooks/devel_experiments.qmd` & `pylemur-0.2.0/notebooks/devel_experiments.qmd`

 * *Files identical despite different names*

### Comparing `pylemur-0.1.0/notebooks/kang_analysis_in_R.qmd` & `pylemur-0.2.0/notebooks/kang_analysis_in_R.qmd`

 * *Files identical despite different names*

### Comparing `pylemur-0.1.0/notebooks/lemur_model_experiments.qmd` & `pylemur-0.2.0/notebooks/lemur_model_experiments.qmd`

 * *Files identical despite different names*

### Comparing `pylemur-0.1.0/notebooks/scanpy_experiments.qmd` & `pylemur-0.2.0/notebooks/scanpy_experiments.qmd`

 * *Files identical despite different names*

### Comparing `pylemur-0.1.0/src/pylemur/pl/basic.py` & `pylemur-0.2.0/src/pylemur/pl/basic.py`

 * *Files identical despite different names*

### Comparing `pylemur-0.1.0/src/pylemur/pp/basic.py` & `pylemur-0.2.0/src/pylemur/pp/basic.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 import numpy as np
 import scanpy.preprocessing._simple
 import scipy
 
-def shifted_log_transform(counts, overdispersion = 0.05, pseudo_count = None, minimum_overdispersion = 0.001):
+
+def shifted_log_transform(counts, overdispersion=0.05, pseudo_count=None, minimum_overdispersion=0.001):
     if pseudo_count is None:
-        pseudo_count = 1/(4 * overdispersion)
+        pseudo_count = 1 / (4 * overdispersion)
 
     n_cells = counts.shape[0]
     size_factors = counts.sum(axis=1)
     size_factors = size_factors / np.exp(np.mean(np.log(size_factors)))
     norm_mat = counts / size_factors.reshape((n_cells, 1))
-    overdispersion = 1/(4 * pseudo_count)
-    res = 1/np.sqrt(overdispersion) * np.log1p(4 * overdispersion * norm_mat)
+    overdispersion = 1 / (4 * pseudo_count)
+    res = 1 / np.sqrt(overdispersion) * np.log1p(4 * overdispersion * norm_mat)
     if scipy.sparse.issparse(counts):
         res = scipy.sparse.csr_matrix(res)
     return res
 
-def get_top_hvgs(adata, n = 1000, layer = None):
+
+def get_top_hvgs(adata, n=1000, layer=None):
     if layer is None:
         mat = adata.X
     else:
         mat = adata.layers[layer]
     var = scanpy.preprocessing._simple._get_mean_var(mat)[1]
-    return var.argsort()[:-(n+1):-1]
+    return var.argsort()[: -(n + 1) : -1]
```

### Comparing `pylemur-0.1.0/src/pylemur/tl/_design_matrix_utils.py` & `pylemur-0.2.0/src/pylemur/tl/_design_matrix_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 from collections.abc import Mapping
+
 import numpy as np
+from numpy.lib import NumpyVersion
 import pandas as pd
+
 # import patsy
 from formulaic import model_matrix
 
 
 def handle_data(data, layer):
     Y = data.X if layer is None else data.layers[layer]
     if not isinstance(Y, np.ndarray):
         Y = Y.toarray()
     return Y
 
+
 def handle_design_parameter(design, obs_data):
     if isinstance(design, np.ndarray):
         if design.ndim == 1:
             # Throw error
             raise ValueError("design specified as a 1d array is not supported yet")
         elif design.ndim == 2:
             design_matrix = design
@@ -26,55 +30,59 @@
     elif isinstance(design, str):
         # Check if design starts with a ~
         if design[0] != "~":
             design = "~" + design + " - 1"
         design_matrix, design_formula = convert_formula_to_design_matrix(design, obs_data)
     else:
         raise ValueError("design must be a 2d array or string")
-    
+
     return design_matrix, design_formula
 
+
 def handle_obs_data(adata, obs_data):
     a = make_data_frame(adata.obs)
-    b = make_data_frame(obs_data, preferred_index = a.index if a is not None else None)
+    b = make_data_frame(obs_data, preferred_index=a.index if a is not None else None)
     if a is None and b is None:
-        return pd.DataFrame(index = pd.RangeIndex(0, adata.shape[0]))
+        return pd.DataFrame(index=pd.RangeIndex(0, adata.shape[0]))
     elif a is None:
         return b
     elif b is None:
         return a
     else:
         return pd.concat([a, b], axis=1)
 
-def make_data_frame(data, preferred_index = None):
+
+def make_data_frame(data, preferred_index=None):
     if data is None:
         return None
     if isinstance(data, pd.DataFrame):
         return data
     elif isinstance(data, Mapping):
-        return pd.DataFrame(data, index = preferred_index)
-    else: 
+        return pd.DataFrame(data, index=preferred_index)
+    else:
         raise ValueError("data must be None, a pandas DataFrame or a Mapping object")
 
 
 def convert_formula_to_design_matrix(formula, obs_data):
     # Check if formula is string
     if isinstance(formula, str):
         # Convert formula to design matrix
         # design_matrix = patsy.dmatrix(formula, obs_data)
         design_matrix = model_matrix(formula, obs_data)
         return design_matrix, formula
     else:
         raise ValueError("formula must be a string")
 
 
-def row_groups(matrix, return_reduced_matrix = False, return_group_ids = False):
-    reduced_matrix, inv = np.unique(matrix, axis = 0, return_inverse=True)
+def row_groups(matrix, return_reduced_matrix=False, return_group_ids=False):
+    reduced_matrix, inv = np.unique(matrix, axis=0, return_inverse=True)
+    if NumpyVersion(np.__version__) >= '2.0.0rc':
+        inv = np.squeeze(inv)
     group_ids = np.unique(inv)
     if return_reduced_matrix and return_group_ids:
         return inv, reduced_matrix, group_ids
     elif return_reduced_matrix:
         return inv, reduced_matrix
     elif return_group_ids:
         return inv, group_ids
     else:
-        return inv
+        return inv
```

### Comparing `pylemur-0.1.0/src/pylemur/tl/_grassmann.py` & `pylemur-0.2.0/src/pylemur/tl/_grassmann.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,21 @@
-import numpy as np 
+import numpy as np
 
 
 def grassmann_map(x, base_point):
     if base_point.shape[0] == 0 or base_point.shape[1] == 0:
         return base_point
     elif np.isnan(x).any():
         # Return an object with the same shape as x filled with nan
         return np.full(x.shape, np.nan)
     else:
-        u, s, vt = np.linalg.svd(x, full_matrices = False)
+        u, s, vt = np.linalg.svd(x, full_matrices=False)
         return (base_point @ vt.T) @ np.diag(np.cos(s)) @ vt + u @ np.diag(np.sin(s)) @ vt
 
+
 def grassmann_log(p, q):
     n = p.shape[0]
     k = p.shape[1]
 
     if n == 0 or k == 0:
         return p
     else:
@@ -22,32 +23,38 @@
         At = q.T - z @ p.T
         # Translate `lm.fit(z, At)$coefficients` to python
         Bt = np.linalg.lstsq(z, At, rcond=None)[0]
         u, s, vt = np.linalg.svd(Bt.T, full_matrices=True)
         u = u[:, :k]
         s = s[:k]
         vt = vt[:k, :]
-        return u @ np.diag(np.arctan(s)) @ vt     
+        return u @ np.diag(np.arctan(s)) @ vt
+
 
 def grassmann_project(x):
     return np.linalg.qr(x)[0]
 
+
 def grassmann_project_tangent(x, base_point):
     return x - base_point @ base_point.T @ x
 
+
 def grassmann_random_point(n, k):
     x = np.random.randn(n, k)
     return grassmann_project(x)
 
+
 def grassmann_random_tangent(base_point):
     x = np.random.randn(*base_point.shape)
     return grassmann_project_tangent(x, base_point)
 
-def grassmann_angle_from_tangent(x, normalized = True):
-    thetas = np.linalg.svd(x, full_matrices = True, compute_uv=False) / np.pi * 180
+
+def grassmann_angle_from_tangent(x, normalized=True):
+    thetas = np.linalg.svd(x, full_matrices=True, compute_uv=False) / np.pi * 180
     if normalized:
-            return np.minimum(thetas, 180 - thetas).max()
+        return np.minimum(thetas, 180 - thetas).max()
     else:
         return thetas[0]
-    
+
+
 def grassmann_angle_from_point(x, y):
-    return grassmann_angle_from_tangent(grassmann_log(y, x))
+    return grassmann_angle_from_tangent(grassmann_log(y, x))
```

### Comparing `pylemur-0.1.0/src/pylemur/tl/_grassmann_lm.py` & `pylemur-0.2.0/src/pylemur/tl/_grassmann_lm.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,98 +1,105 @@
-
-
 import numpy as np
+
 from pylemur.tl._design_matrix_utils import row_groups
 from pylemur.tl._grassmann import grassmann_log, grassmann_map
 from pylemur.tl._lin_alg_wrappers import fit_pca, ridge_regression
 
 
-def grassmann_geodesic_regression(coord_systems, design, base_point, weights = None):
+def grassmann_geodesic_regression(coord_systems, design, base_point, weights=None):
     """
-    Solve Sum_j d(U_j, Exp_p(Sum_k V_k:: * X_jk)) for V, where 
+    Solve Sum_j d(U_j, Exp_p(Sum_k V_k:: * X_jk)) for V, where
     d(U, V) = ||Log(U, V)|| is the inverse of the exponential map on the Grassmann manifold.
 
     Parameters
     ----------
     coord_systems : a list of orthonormal 2D matrices (length n_groups)
     design : design matrix, shape (n_groups, n_coef)
     base_point : array-like, shape (n_emb, n_features)
         The base point.
     weights : array-like, shape (n_groups,)
-    
+
     Returns
-    ----------
+    -------
     beta: array-like, shape (n_emb, n_features, n_coef)
     """
     n_obs = design.shape[0]
     n_coef = design.shape[1]
     n_emb = base_point.shape[0]
     n_features = base_point.shape[1]
 
     assert len(coord_systems) == n_obs
     for i in range(n_obs):
         assert coord_systems[i].shape == (n_emb, n_features)
     if weights is None:
         weights = np.ones(n_obs)
-    
-    tangent_vecs = [grassmann_log(base_point.T, coord_systems[i].T).T.reshape((n_emb * n_features)) for i in range(n_obs)]
+
+    tangent_vecs = [
+        grassmann_log(base_point.T, coord_systems[i].T).T.reshape(n_emb * n_features) for i in range(n_obs)
+    ]
     tangent_vecs = np.vstack(tangent_vecs)
     if tangent_vecs.shape[0] == 0:
         tangent_fit = np.zeros((0, n_coef))
     else:
-        tangent_fit = ridge_regression(tangent_vecs, design, weights = weights)
+        tangent_fit = ridge_regression(tangent_vecs, design, weights=weights)
 
-    tangent_fit = tangent_fit.reshape((n_coef, n_emb, n_features)).transpose((1,2,0))
+    tangent_fit = tangent_fit.reshape((n_coef, n_emb, n_features)).transpose((1, 2, 0))
     return tangent_fit
 
 
 def grassmann_lm(Y, design_matrix, base_point):
     """
     Solve Sum_i||Y_i: - Y_i: Proj(Exp_p(Sum_k V_k:: * X_ik))||^2 for V.
+
     Parameters
     ----------
     Y : array-like, shape (n_samples, n_features)
         The input data matrix.
     design_matrix : array-like, shape (n_samples, n_coef)
         The design matrix.
     base_point : array-like, shape (n_emb, n_features)
         The base point.
+
     Returns
     -------
     beta: array-like, shape (n_emb, n_features, n_coef)
     """
     n_emb = base_point.shape[0]
 
-    des_row_groups, reduced_design_matrix, des_row_group_ids = row_groups(design_matrix, return_reduced_matrix=True,return_group_ids=True)
+    des_row_groups, reduced_design_matrix, des_row_group_ids = row_groups(
+        design_matrix, return_reduced_matrix=True, return_group_ids=True
+    )
     if np.min(np.unique(des_row_groups, return_counts=True)[1]) < n_emb:
         raise ValueError("Too few dataset points in some design matrix group.")
-    group_planes = [fit_pca(Y[des_row_groups == i, :], n_emb, center = False).coord_system for i in des_row_group_ids]
+    group_planes = [fit_pca(Y[des_row_groups == i, :], n_emb, center=False).coord_system for i in des_row_group_ids]
     group_sizes = [np.sum(des_row_groups == i) for i in des_row_group_ids]
 
-    coef = grassmann_geodesic_regression(group_planes, reduced_design_matrix, base_point, weights = group_sizes)
+    coef = grassmann_geodesic_regression(group_planes, reduced_design_matrix, base_point, weights=group_sizes)
     return coef
 
 
 def project_diffemb_into_data_space(embedding, design_matrix, coefficients, base_point):
     n_features = base_point.shape[1]
     res = np.zeros((design_matrix.shape[0], n_features))
-    des_row_groups, reduced_design_matrix, des_row_group_ids = row_groups(design_matrix, return_reduced_matrix=True,return_group_ids=True)
+    des_row_groups, reduced_design_matrix, des_row_group_ids = row_groups(
+        design_matrix, return_reduced_matrix=True, return_group_ids=True
+    )
     for id in des_row_group_ids:
-        covar = reduced_design_matrix[id,:]
+        covar = reduced_design_matrix[id, :]
         subspace = grassmann_map(np.dot(coefficients, covar).T, base_point.T)
         res[des_row_groups == id, :] = embedding[des_row_groups == id, :] @ subspace.T
     return res
-    
+
 
 def project_data_on_diffemb(Y, design_matrix, coefficients, base_point):
     n_emb = base_point.shape[0]
     n_obs = Y.shape[0]
     res = np.zeros((n_obs, n_emb))
-    des_row_groups, reduced_design_matrix, des_row_group_ids = row_groups(design_matrix, return_reduced_matrix=True,return_group_ids=True)
+    des_row_groups, reduced_design_matrix, des_row_group_ids = row_groups(
+        design_matrix, return_reduced_matrix=True, return_group_ids=True
+    )
     for id in des_row_group_ids:
-        Y_subset = Y[des_row_groups == id,:]
-        covar = reduced_design_matrix[id,:]
+        Y_subset = Y[des_row_groups == id, :]
+        covar = reduced_design_matrix[id, :]
         subspace = grassmann_map(np.dot(coefficients, covar).T, base_point.T)
         res[des_row_groups == id, :] = Y_subset @ subspace
     return res
-
-
```

### Comparing `pylemur-0.1.0/src/pylemur/tl/_lin_alg_wrappers.py` & `pylemur-0.2.0/src/pylemur/tl/_lin_alg_wrappers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,58 +1,65 @@
-import sklearn.decomposition as skd
 from typing import NamedTuple
+
 import numpy as np
+import sklearn.decomposition as skd
+
 
 class PCA(NamedTuple):
     embedding: np.ndarray
     coord_system: np.ndarray
     offset: np.ndarray
 
+
 def fit_pca(Y, n, center=True):
     """
     Calculate the PCA of a given data matrix Y.
+
     Parameters
     ----------
     Y : array-like, shape (n_samples, n_features)
         The input data matrix.
     n : int
         The number of principal components to return.
     center : bool, default=True
         If True, the data will be centered before computing the covariance matrix.
+
     Returns
     -------
     pca : sklearn.decomposition.PCA
         The PCA object.
     """
     if center:
         pca = skd.PCA(n_components=n)
         emb = pca.fit_transform(Y)
         coord_system = pca.components_
         mean = pca.mean_
     else:
-        svd = skd.TruncatedSVD(n_components=n, algorithm='arpack')
+        svd = skd.TruncatedSVD(n_components=n, algorithm="arpack")
         emb = svd.fit_transform(Y)
-        coord_system =  svd.components_
+        coord_system = svd.components_
         mean = np.zeros(Y.shape[1])
     return PCA(emb, coord_system, mean)
 
 
-def ridge_regression(Y, X, ridge_penalty = 0, weights = None):
+def ridge_regression(Y, X, ridge_penalty=0, weights=None):
     """
     Calculate the ridge regression of a given data matrix Y.
+
     Parameters
     ----------
     Y : array-like, shape (n_samples, n_features)
         The input data matrix.
     X : array-like, shape (n_samples, n_coef)
         The input data matrix.
     ridge_penalty : float, default=0
         The ridge penalty.
     weights : array-like, shape (n_features,)
         The weights to apply to each feature.
+
     Returns
     -------
     ridge: array-like, shape (n_coef, n_features)
     """
     n_coef = X.shape[1]
     n_samples = X.shape[0]
     n_feat = Y.shape[1]
@@ -67,19 +74,20 @@
         assert len(ridge_penalty) == n_coef
         ridge_penalty = np.diag(ridge_penalty)
     elif np.ndim(ridge_penalty) == 1:
         assert ridge_penalty.shape == (n_coef, n_coef)
         pass
     else:
         raise ValueError("ridge_penalty must be a scalar, 1d array, or 2d array")
-        
+
     ridge_penalty_sq = np.sqrt(np.sum(weights)) * (ridge_penalty.T @ ridge_penalty)
     weights_sqrt = np.sqrt(weights)
     X_ext = np.vstack([multiply_along_axis(X, weights_sqrt, 0), ridge_penalty_sq])
     Y_ext = np.vstack([multiply_along_axis(Y, weights_sqrt, 0), np.zeros((n_coef, n_feat))])
 
     ridge = np.linalg.lstsq(X_ext, Y_ext, rcond=None)[0]
     return ridge
 
+
 def multiply_along_axis(A, B, axis):
     # Copied from https://stackoverflow.com/a/71750176/604854
-    return np.swapaxes(np.swapaxes(A, axis, -1) * B, -1, axis)
+    return np.swapaxes(np.swapaxes(A, axis, -1) * B, -1, axis)
```

### Comparing `pylemur-0.1.0/tests/test_grasmann_lm.py` & `pylemur-0.2.0/tests/test_grasmann_lm.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,81 +1,88 @@
-
 import numpy as np
 
 from pylemur.tl._grassmann import grassmann_angle_from_point, grassmann_map, grassmann_project
-from pylemur.tl._grassmann_lm import grassmann_geodesic_regression, grassmann_lm, project_data_on_diffemb, project_diffemb_into_data_space
+from pylemur.tl._grassmann_lm import (
+    grassmann_geodesic_regression,
+    grassmann_lm,
+    project_data_on_diffemb,
+    project_diffemb_into_data_space,
+)
 from pylemur.tl._lin_alg_wrappers import fit_pca
 
 
 def test_geodesic_regression():
     n_feat = 17
     base_point = grassmann_project(np.random.randn(n_feat, 3)).T
     assert np.allclose(base_point @ base_point.T, np.eye(3))
     coord_systems = [grassmann_project(np.random.randn(n_feat, 3)).T for _ in range(10)]
     x = np.arange(10)
     design = np.vstack([np.ones(10), x]).T
 
     fit = grassmann_geodesic_regression(coord_systems, design, base_point)
     assert fit.shape == (3, n_feat, 2)
-    proj = grassmann_map(fit[:,:,0].T, base_point.T)
+    proj = grassmann_map(fit[:, :, 0].T, base_point.T)
     assert np.allclose(proj.T @ proj, np.eye(3))
-    proj = grassmann_map(fit[:,:,1].T, base_point.T)
+    proj = grassmann_map(fit[:, :, 1].T, base_point.T)
     assert np.allclose(proj.T @ proj, np.eye(3))
 
 
 def test_grassmann_lm():
     n_obs = 100
     base_point = grassmann_project(np.random.randn(5, 2)).T
     data = np.random.randn(n_obs, 5)
-    plane_all = fit_pca(data, 2, center = False).coord_system
+    plane_all = fit_pca(data, 2, center=False).coord_system
     des = np.ones((n_obs, 1))
     fit = grassmann_lm(data, des, base_point)
-    assert np.allclose(grassmann_angle_from_point(grassmann_map(fit[:,:,0].T, base_point.T), plane_all.T), 0)
-    
+    assert np.allclose(grassmann_angle_from_point(grassmann_map(fit[:, :, 0].T, base_point.T), plane_all.T), 0)
+
     # Make a design matrix of three groups (with an intercept)
     x = np.random.randint(3, size=n_obs)
-    des = np.eye(3)[x,:]
-    des = np.hstack([np.ones((n_obs, 1)), des[:,1:3]])
+    des = np.eye(3)[x, :]
+    des = np.hstack([np.ones((n_obs, 1)), des[:, 1:3]])
     fit = grassmann_lm(data, des, base_point)
 
-    plane_a = fit_pca(data[x == 0], 2, center = False).coord_system
-    plane_b = fit_pca(data[x == 1], 2, center = False).coord_system
-    plane_c = fit_pca(data[x == 2], 2, center = False).coord_system
-
-    assert np.allclose(grassmann_angle_from_point(grassmann_map(fit[:,:,0].T, base_point.T), plane_a.T), 0)
-    assert np.allclose(grassmann_angle_from_point(grassmann_map((fit[:,:,0] + fit[:,:,1]).T, base_point.T), plane_b.T), 0)
-    assert np.allclose(grassmann_angle_from_point(grassmann_map((fit[:,:,0] + fit[:,:,2]).T, base_point.T), plane_c.T), 0)
+    plane_a = fit_pca(data[x == 0], 2, center=False).coord_system
+    plane_b = fit_pca(data[x == 1], 2, center=False).coord_system
+    plane_c = fit_pca(data[x == 2], 2, center=False).coord_system
+
+    assert np.allclose(grassmann_angle_from_point(grassmann_map(fit[:, :, 0].T, base_point.T), plane_a.T), 0)
+    assert np.allclose(
+        grassmann_angle_from_point(grassmann_map((fit[:, :, 0] + fit[:, :, 1]).T, base_point.T), plane_b.T), 0
+    )
+    assert np.allclose(
+        grassmann_angle_from_point(grassmann_map((fit[:, :, 0] + fit[:, :, 2]).T, base_point.T), plane_c.T), 0
+    )
 
 
 def test_project_data_on_diffemb():
     n_obs = 100
     base_point = grassmann_project(np.random.randn(5, 2)).T
     data = np.random.randn(n_obs, 5)
     des = np.ones((n_obs, 1))
     fit = grassmann_lm(data, des, base_point)
-    pca = fit_pca(data, 2, center = False)
-    angle = grassmann_angle_from_point(grassmann_map(fit[:,:,0].T, base_point.T), pca.coord_system.T)
+    pca = fit_pca(data, 2, center=False)
+    angle = grassmann_angle_from_point(grassmann_map(fit[:, :, 0].T, base_point.T), pca.coord_system.T)
     assert np.allclose(angle, 0)
 
     proj = project_data_on_diffemb(data, des, fit, base_point)
     # The projection and the embedding are rotated to each other
     # Remove rotation effect using orthogonal procrustes
-    U,_,Vt=np.linalg.svd(proj.T @ pca.embedding, full_matrices=False)
+    U, _, Vt = np.linalg.svd(proj.T @ pca.embedding, full_matrices=False)
     rot = U @ Vt
     assert np.allclose(proj @ rot, pca.embedding)
 
 
 def test_project_data_on_diffemb():
     n_obs = 100
     base_point = grassmann_project(np.random.randn(5, 2)).T
     data = np.random.randn(n_obs, 5)
     des = np.ones((n_obs, 1))
     fit = grassmann_lm(data, des, base_point)
-    pca = fit_pca(data, 2, center = False)
-    angle = grassmann_angle_from_point(grassmann_map(fit[:,:,0].T, base_point.T), pca.coord_system.T)
+    pca = fit_pca(data, 2, center=False)
+    angle = grassmann_angle_from_point(grassmann_map(fit[:, :, 0].T, base_point.T), pca.coord_system.T)
     assert np.allclose(angle, 0)
 
     proj = project_data_on_diffemb(data, des, fit, base_point)
     data_hat1 = pca.embedding @ pca.coord_system
     data_hat2 = project_diffemb_into_data_space(proj, des, fit, base_point)
     assert np.allclose(data_hat1, data_hat2)
-
```

### Comparing `pylemur-0.1.0/tests/test_grassmann.py` & `pylemur-0.2.0/tests/test_grassmann.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import numpy as np
+
 from pylemur.tl._grassmann import *
 
+
 def test_grassmann_map():
     # Test case 1: empty base point
     x = np.array([[1, 2], [3, 4], [5, 6]])
     p = np.array([])
     assert np.array_equal(grassmann_map(x, p), p)
 
-
     # Test case 2: x contains NaN values
     x = np.array([[1, 2], [3, np.nan], [5, 6]])
     p = np.array([[1, 0], [0, 1], [0, 0]])
     assert np.isnan(grassmann_map(x, p)).all()
 
     p = grassmann_random_point(5, 2)
     assert np.allclose(p.T @ p, np.eye(2))
```

### Comparing `pylemur-0.1.0/tests/test_lin_alg_utils.py` & `pylemur-0.2.0/tests/test_lin_alg_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 import numpy as np
 from sklearn.linear_model import LinearRegression, Ridge
+
 from pylemur.tl._lin_alg_wrappers import *
 
+
 def test_fit_pca():
     # Make example data
     Y = np.random.randn(30, 400)
-    pca = fit_pca(Y, 3, center = True)
-    assert np.allclose(pca.offset, Y.mean(axis = 0))
+    pca = fit_pca(Y, 3, center=True)
+    assert np.allclose(pca.offset, Y.mean(axis=0))
     assert np.allclose(pca.coord_system @ pca.coord_system.T, np.eye(3))
     assert np.allclose(pca.embedding, (Y - pca.offset) @ pca.coord_system.T)
 
-    pca2 = fit_pca(Y, 3, center = False)
+    pca2 = fit_pca(Y, 3, center=False)
     assert np.allclose(pca2.offset, np.zeros(Y.shape[1]))
     assert np.allclose(pca2.coord_system @ pca2.coord_system.T, np.eye(3))
     assert np.allclose(pca2.embedding, (Y - pca2.offset) @ pca2.coord_system.T)
     assert np.allclose(Y @ pca2.coord_system.T, pca2.embedding)
 
 
 def test_ridge_regression():
@@ -26,19 +28,19 @@
     assert np.allclose(beta, np.linalg.inv(X.T @ X) @ X.T @ Y)
     reg = LinearRegression(fit_intercept=False).fit(X, Y)
     assert np.allclose(beta, reg.coef_.T)
 
     # Check with weights
     weights = np.random.rand(400)
     beta = ridge_regression(Y, X, weights=weights)
-    reg = LinearRegression(fit_intercept=False).fit(X, Y, sample_weight = weights)
+    reg = LinearRegression(fit_intercept=False).fit(X, Y, sample_weight=weights)
     assert np.allclose(beta, reg.coef_.T)
 
     # Check with ridge penalty
     pen = 0.3
     beta = ridge_regression(Y, X, ridge_penalty=pen)
     gamma = np.sqrt(400) * pen**2 * np.eye(3)
     beta2 = np.linalg.inv(X.T @ X + gamma.T @ gamma) @ X.T @ Y
     assert np.allclose(beta, beta2)
 
     reg = Ridge(alpha=pen**4 * 400, fit_intercept=False).fit(X, Y)
-    assert np.allclose(beta, reg.coef_.T)
+    assert np.allclose(beta, reg.coef_.T)
```

### Comparing `pylemur-0.1.0/.gitignore` & `pylemur-0.2.0/.gitignore`

 * *Files 11% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 # Temp files
 .DS_Store
 *~
 buck-out/
 
 # Compiled files
 .venv/
+.venv_pre_release/
 __pycache__/
 .mypy_cache/
 .ruff_cache/
 
 # Distribution / packaging
 /build/
 /dist/
@@ -58,7 +59,12 @@
 # docs
 /docs/generated/
 /docs/_build/
 
 # IDEs
 /.idea/
 /.vscode/
+
+# Data files from tutorial
+docs/notebooks/data/*
+
+
```

### Comparing `pylemur-0.1.0/LICENSE` & `pylemur-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pylemur-0.1.0/README.md` & `pylemur-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pylemur-0.1.0/pyproject.toml` & `pylemur-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 build-backend = "hatchling.build"
 requires = ["hatchling"]
 
 [project]
 name = "pyLemur"
-version = "0.1.0"
+version = "0.2.0"
 description = "A Python implementation of the LEMUR algorithm for analyzing multi-condition single-cell RNA-seq data."
 readme = "README.md"
 requires-python = ">=3.9"
 license = {file = "LICENSE"}
 authors = [
     {name = "Constantin Ahlmann-Eltze"},
 ]
```

### Comparing `pylemur-0.1.0/PKG-INFO` & `pylemur-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pyLemur
-Version: 0.1.0
+Version: 0.2.0
 Summary: A Python implementation of the LEMUR algorithm for analyzing multi-condition single-cell RNA-seq data.
 Project-URL: Documentation, https://pyLemur.readthedocs.io/
 Project-URL: Source, https://github.com/const-ae/pyLemur
 Project-URL: Home-page, https://github.com/const-ae/pyLemur
 Author: Constantin Ahlmann-Eltze
 Maintainer-email: Constantin Ahlmann-Eltze <artjom31415@googlemail.com>
 License: MIT License
```

