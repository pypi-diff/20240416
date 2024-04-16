# Comparing `tmp/manamodeller-0.1.1.tar.gz` & `tmp/manamodeller-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "manamodeller-0.1.1.tar", max compression
+gzip compressed data, was "manamodeller-0.1.2.tar", max compression
```

## Comparing `manamodeller-0.1.1.tar` & `manamodeller-0.1.2.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0     4525 2024-04-01 15:24:21.067290 manamodeller-0.1.1/README.md
--rw-r--r--   0        0        0        0 2024-04-01 14:34:25.718289 manamodeller-0.1.1/manamodeller/__init__.py
--rw-r--r--   0        0        0     7295 2024-04-01 14:34:25.722289 manamodeller-0.1.1/manamodeller/batchs.py
--rw-r--r--   0        0        0     9291 2024-04-01 14:34:25.722289 manamodeller-0.1.1/manamodeller/dars.py
--rw-r--r--   0        0        0     8786 2024-04-01 14:34:25.722289 manamodeller-0.1.1/manamodeller/modelling.py
--rw-r--r--   0        0        0     9545 2024-04-01 14:34:25.722289 manamodeller-0.1.1/manamodeller/results_analysis.py
--rw-r--r--   0        0        0     8975 2024-04-01 14:34:25.722289 manamodeller-0.1.1/manamodeller/results_processing.py
--rw-r--r--   0        0        0     2441 2024-04-01 14:34:25.722289 manamodeller-0.1.1/manamodeller/utils.py
--rw-r--r--   0        0        0      491 2024-04-01 15:26:06.415440 manamodeller-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     5408 2024-04-01 15:26:12.894845 manamodeller-0.1.1/setup.py
--rw-r--r--   0        0        0     5281 2024-04-01 15:26:12.895108 manamodeller-0.1.1/PKG-INFO
+-rwxr-xr-x   0        0        0     4525 2024-04-16 12:39:15.562814 manamodeller-0.1.2/README.md
+-rwxr-xr-x   0        0        0        0 2024-04-16 12:39:16.060932 manamodeller-0.1.2/manamodeller/__init__.py
+-rwxr-xr-x   0        0        0     7295 2024-04-16 12:39:16.060932 manamodeller-0.1.2/manamodeller/batchs.py
+-rwxr-xr-x   0        0        0     9291 2024-04-16 12:39:16.060932 manamodeller-0.1.2/manamodeller/dars.py
+-rwxr-xr-x   0        0        0     8786 2024-04-16 12:39:16.074976 manamodeller-0.1.2/manamodeller/modelling.py
+-rwxr-xr-x   0        0        0     9545 2024-04-16 12:39:16.076007 manamodeller-0.1.2/manamodeller/results_analysis.py
+-rwxr-xr-x   0        0        0     8975 2024-04-16 12:39:16.121300 manamodeller-0.1.2/manamodeller/results_processing.py
+-rwxr-xr-x   0        0        0     2441 2024-04-16 12:39:16.141931 manamodeller-0.1.2/manamodeller/utils.py
+-rwxr-xr-x   0        0        0      491 2024-04-16 12:39:16.724995 manamodeller-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     5281 1970-01-01 00:00:00.000000 manamodeller-0.1.2/PKG-INFO
```

### Comparing `manamodeller-0.1.1/README.md` & `manamodeller-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `manamodeller-0.1.1/manamodeller/batchs.py` & `manamodeller-0.1.2/manamodeller/batchs.py`

 * *Files identical despite different names*

### Comparing `manamodeller-0.1.1/manamodeller/dars.py` & `manamodeller-0.1.2/manamodeller/dars.py`

 * *Files identical despite different names*

### Comparing `manamodeller-0.1.1/manamodeller/modelling.py` & `manamodeller-0.1.2/manamodeller/modelling.py`

 * *Files identical despite different names*

### Comparing `manamodeller-0.1.1/manamodeller/results_analysis.py` & `manamodeller-0.1.2/manamodeller/results_analysis.py`

 * *Files identical despite different names*

### Comparing `manamodeller-0.1.1/manamodeller/results_processing.py` & `manamodeller-0.1.2/manamodeller/results_processing.py`

 * *Files identical despite different names*

### Comparing `manamodeller-0.1.1/manamodeller/utils.py` & `manamodeller-0.1.2/manamodeller/utils.py`

 * *Files identical despite different names*

### Comparing `manamodeller-0.1.1/setup.py` & `manamodeller-0.1.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,112 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: manamodeller
+Version: 0.1.2
+Summary: 
+Author: Louison Fresnais
+Author-email: fresnaislouison@gmail.com
+Requires-Python: >=3.7,<3.10
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Requires-Dist: dexom-python (>=1.0)
+Requires-Dist: jproperties (>=2.1.1)
+Requires-Dist: jupyterlab (>=4.0)
+Requires-Dist: networkx (>=2.8.4)
+Requires-Dist: numpy (>=1.2.0,<2.0.0)
+Requires-Dist: pandas (<=1.5.0)
+Requires-Dist: progressbar (>=2.5,<3.0)
+Requires-Dist: pyvis (>=0.3.2)
+Requires-Dist: tqdm (>=4.65.0,<5.0.0)
+Requires-Dist: xlsxwriter (>=3.1.0)
+Description-Content-Type: text/markdown
 
-packages = \
-['manamodeller']
+# MANA
+MANA: mMoA identification Assisted by modelling and Network Analysis.
+[![Documentation Status](https://readthedocs.org/projects/manamodeller/badge/?version=latest)](https://manamodeller.readthedocs.io/en/latest/?badge=latest)
+[![PyPI version](https://badge.fury.io/py/manamodeller.svg)](https://badge.fury.io/py/manamodeller)
 
-package_data = \
-{'': ['*']}
+This repository contains code and a test case associated with the article named : 
 
-install_requires = \
-['dexom-python>=1.0',
- 'jproperties>=2.1.1',
- 'jupyterlab>=4.0',
- 'networkx>=2.8.4',
- 'numpy>=1.2.0,<2.0.0',
- 'pandas<=1.5.0',
- 'progressbar>=2.5,<3.0',
- 'pyvis>=0.3.2',
- 'tqdm>=4.65.0,<5.0.0',
- 'xlsxwriter>=3.1.0']
-
-setup_kwargs = {
-    'name': 'manamodeller',
-    'version': '0.1.1',
-    'description': '',
-    'long_description': '# MANA\nMANA: mMoA identification Assisted by modelling and Network Analysis.\n[![Documentation Status](https://readthedocs.org/projects/manamodeller/badge/?version=latest)](https://manamodeller.readthedocs.io/en/latest/?badge=latest)\n[![PyPI version](https://badge.fury.io/py/manamodeller.svg)](https://badge.fury.io/py/manamodeller)\n\nThis repository contains code and a test case associated with the article named : \n\n    A strategy to detect metabolic changes induced by exposure to chemicals from large sets of condition-specific metabolic models computed with enumeration techniques\n\nAPI documentation is available here: https://manamodeller.readthedocs.io/en/latest/\n\nThe workflow presented in this article aims at improving our understanding of the metabolic Mechanism of Action and can be divided in three steps:\n1. Condition-specific metabolic network modelling with partial enumeration from gene expression data\n2. Identify Differentially Activated Reactions (DAR) from the modelised sets of condition-specific metabolic networks\n3. Network anaylsis to extract minimal subnetworks représentative of the chemical\'s mMoA\n\nEach step of the workflow is performed by a jupyter notebook:\n* **partial_enumeration.ipynb**\n* **dars_calculation.ipynb**\n* **analysis.ipynb**\n\nProperties and parameters for the workflow are stored in a unique file to update in order to change parameters such as compound, dose, time, etc:\n* **props.properties**\n\nThe package source code is contained in the mana folder and can be installed as a python module.\n## Installation:\n### Requirements:\n\n* Python3.9X\n* Java 11\n* Met4j 1.2.2 jar (stored in this repository)\n* CPLEX 12.10 or newer (not required for the test case)\n\n### Installing the package\n\nIf needed, install poetry (package and dependances management):\n\n<code>pip install poetry</code>\n\nThen, from the root directory of the MANA repository, enter the following command:\n\n<code>pip install -e .</code>\n\n### Launching the main jupyter notebook (test case)\n\nFrom the root directory of the MANA repository, enter the following command:\n\n<code>python3 -m jupyterlab master_notebook.ipynb</code>\n\nOnce JupyterLab opened in your navigator, you can click on "Run", then click on "Run All Cells" as illustrated below.\n\n![Alt text](readme_figures/jupyterlab_interface_example.png)\n\nIt will perform the complete workflow on the test case (PHH exposed to amiodarone during 24h and associated controls).\nThe notebook will pause near the end of the workflow waiting for you to provide the desired number of clusters during the hierarchical clustering step.\n\n## Localisation of the main results files:\n\n[Annotated cluster 1](tests/analysis/clusters_annotation_tables/amiodarone_24_hr_extracellexclude_cluster1_table.xlsx)\n\n[Annotated cluster 2](tests/analysis/clusters_annotation_tables/amiodarone_24_hr_extracellexclude_cluster2_table.xlsx)\n\n[Subnetwork 1 reactions list](tests/analysis/subnetwork_reactions/amiodarone_24_hr_extracellexclude_cluster1_undirected_r2_noisecond_extracell.txt)\n\n[Subnetwork 2 reactions list](tests/analysis/subnetwork_reactions/amiodarone_24_hr_extracellexclude_cluster2_undirected_r2_noisecond_extracell.txt)\n\n## Visualisation with MetExploreViz:\n\nTo visualise cluster\'s subnetworks in MetExploreViz, follow these steps:\n* go to https://metexplore.toulouse.inrae.fr/metexplore2/, then click on "Start MetExplore"\n* In the BioSources tab, find and left click on "Homo Sapiens", then double click on "Swainston2016 - Reconstruction of human metabolic network (Recon 2.2)"\n* Once loading is finished, left click on "OMICS", then on "Mapping -> From omics", load the desired subnetwork reactions .txt file\n* Change Object from "Metabolites" to "Reaction" and left click on "Map"\n* Once the mapping is finished, click on the "Network Data" tab then on the "Reactions" tab.\n* Filter reactions to keep only mapped reactions:\n    ![Alt text](readme_figures/filter_reactions.png)\n* Right click and left click on "Copy all to cart"\n* Create the network from the cart as shown below:\n    ![Alt text](readme_figures/graph_from_cart.png)\n\nNext, you will be able to remove side compounds, move nodes and map new information on the visualisation.\nMore information available in MetExplore documentation (https://metexplore.toulouse.inrae.fr/metexplore-doc/index.php) and MetExploreViz documentation (https://metexplore.toulouse.inrae.fr/metexploreViz/doc/index.php)\n\n\n## Contact:\nLouison Fresnais: fresnaislouison@gmail.com\n\nMetExplore/MetExploreViz team: contact-metexplore@inra.fr\n',
-    'author': 'Louison Fresnais',
-    'author_email': 'fresnaislouison@gmail.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': None,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.7,<3.10',
-}
+    A strategy to detect metabolic changes induced by exposure to chemicals from large sets of condition-specific metabolic models computed with enumeration techniques
 
+API documentation is available here: https://manamodeller.readthedocs.io/en/latest/
+
+The workflow presented in this article aims at improving our understanding of the metabolic Mechanism of Action and can be divided in three steps:
+1. Condition-specific metabolic network modelling with partial enumeration from gene expression data
+2. Identify Differentially Activated Reactions (DAR) from the modelised sets of condition-specific metabolic networks
+3. Network anaylsis to extract minimal subnetworks représentative of the chemical's mMoA
+
+Each step of the workflow is performed by a jupyter notebook:
+* **partial_enumeration.ipynb**
+* **dars_calculation.ipynb**
+* **analysis.ipynb**
+
+Properties and parameters for the workflow are stored in a unique file to update in order to change parameters such as compound, dose, time, etc:
+* **props.properties**
+
+The package source code is contained in the mana folder and can be installed as a python module.
+## Installation:
+### Requirements:
+
+* Python3.9X
+* Java 11
+* Met4j 1.2.2 jar (stored in this repository)
+* CPLEX 12.10 or newer (not required for the test case)
+
+### Installing the package
+
+If needed, install poetry (package and dependances management):
+
+<code>pip install poetry</code>
+
+Then, from the root directory of the MANA repository, enter the following command:
+
+<code>pip install -e .</code>
+
+### Launching the main jupyter notebook (test case)
+
+From the root directory of the MANA repository, enter the following command:
+
+<code>python3 -m jupyterlab master_notebook.ipynb</code>
+
+Once JupyterLab opened in your navigator, you can click on "Run", then click on "Run All Cells" as illustrated below.
+
+![Alt text](readme_figures/jupyterlab_interface_example.png)
+
+It will perform the complete workflow on the test case (PHH exposed to amiodarone during 24h and associated controls).
+The notebook will pause near the end of the workflow waiting for you to provide the desired number of clusters during the hierarchical clustering step.
+
+## Localisation of the main results files:
+
+[Annotated cluster 1](tests/analysis/clusters_annotation_tables/amiodarone_24_hr_extracellexclude_cluster1_table.xlsx)
+
+[Annotated cluster 2](tests/analysis/clusters_annotation_tables/amiodarone_24_hr_extracellexclude_cluster2_table.xlsx)
+
+[Subnetwork 1 reactions list](tests/analysis/subnetwork_reactions/amiodarone_24_hr_extracellexclude_cluster1_undirected_r2_noisecond_extracell.txt)
+
+[Subnetwork 2 reactions list](tests/analysis/subnetwork_reactions/amiodarone_24_hr_extracellexclude_cluster2_undirected_r2_noisecond_extracell.txt)
+
+## Visualisation with MetExploreViz:
+
+To visualise cluster's subnetworks in MetExploreViz, follow these steps:
+* go to https://metexplore.toulouse.inrae.fr/metexplore2/, then click on "Start MetExplore"
+* In the BioSources tab, find and left click on "Homo Sapiens", then double click on "Swainston2016 - Reconstruction of human metabolic network (Recon 2.2)"
+* Once loading is finished, left click on "OMICS", then on "Mapping -> From omics", load the desired subnetwork reactions .txt file
+* Change Object from "Metabolites" to "Reaction" and left click on "Map"
+* Once the mapping is finished, click on the "Network Data" tab then on the "Reactions" tab.
+* Filter reactions to keep only mapped reactions:
+    ![Alt text](readme_figures/filter_reactions.png)
+* Right click and left click on "Copy all to cart"
+* Create the network from the cart as shown below:
+    ![Alt text](readme_figures/graph_from_cart.png)
+
+Next, you will be able to remove side compounds, move nodes and map new information on the visualisation.
+More information available in MetExplore documentation (https://metexplore.toulouse.inrae.fr/metexplore-doc/index.php) and MetExploreViz documentation (https://metexplore.toulouse.inrae.fr/metexploreViz/doc/index.php)
+
+
+## Contact:
+Louison Fresnais: fresnaislouison@gmail.com
+
+MetExplore/MetExploreViz team: contact-metexplore@inra.fr
 
-setup(**setup_kwargs)
```

