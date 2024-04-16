# Comparing `tmp/pulpo-dev-0.0.2.tar.gz` & `tmp/pulpo-dev-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulpo-dev-0.0.2.tar", last modified: Wed Oct 11 09:11:04 2023, max compression
+gzip compressed data, was "pulpo-dev-0.0.3.tar", last modified: Fri Dec 15 10:08:14 2023, max compression
```

## Comparing `pulpo-dev-0.0.2.tar` & `pulpo-dev-0.0.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-10-11 09:11:04.358548 pulpo-dev-0.0.2/
--rw-rw-rw-   0        0        0     1553 2023-10-05 10:57:10.000000 pulpo-dev-0.0.2/LICENSE
--rw-rw-rw-   0        0        0       39 2023-10-11 09:03:16.000000 pulpo-dev-0.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     4541 2023-10-11 09:11:04.357551 pulpo-dev-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0    11321 2023-10-11 07:55:10.000000 pulpo-dev-0.0.2/README.md
--rw-rw-rw-   0        0        0     3884 2023-10-11 07:52:23.000000 pulpo-dev-0.0.2/README_pypi.md
-drwxrwxrwx   0        0        0        0 2023-10-11 09:11:04.341090 pulpo-dev-0.0.2/pulpo/
--rw-rw-rw-   0        0        0        0 2023-07-03 13:40:34.000000 pulpo-dev-0.0.2/pulpo/__init__.py
--rw-rw-rw-   0        0        0     3168 2023-10-11 08:11:44.000000 pulpo-dev-0.0.2/pulpo/pulpo.py
-drwxrwxrwx   0        0        0        0 2023-10-11 09:11:04.345197 pulpo-dev-0.0.2/pulpo/utils/
--rw-rw-rw-   0        0        0        0 2023-07-03 15:12:57.000000 pulpo-dev-0.0.2/pulpo/utils/__init__.py
--rw-rw-rw-   0        0        0     4192 2023-10-05 10:57:10.000000 pulpo-dev-0.0.2/pulpo/utils/bw_parser.py
--rw-rw-rw-   0        0        0     5305 2023-10-05 10:57:10.000000 pulpo-dev-0.0.2/pulpo/utils/converter.py
--rw-rw-rw-   0        0        0     8401 2023-10-05 10:57:10.000000 pulpo-dev-0.0.2/pulpo/utils/optimizer.py
--rw-rw-rw-   0        0        0     5231 2023-10-05 10:56:55.000000 pulpo-dev-0.0.2/pulpo/utils/saver.py
--rw-rw-rw-   0        0        0     9628 2023-10-11 07:42:04.000000 pulpo-dev-0.0.2/pulpo/utils/tests.py
-drwxrwxrwx   0        0        0        0 2023-10-11 09:11:04.355556 pulpo-dev-0.0.2/pulpo_dev.egg-info/
--rw-rw-rw-   0        0        0     4541 2023-10-11 09:11:04.000000 pulpo-dev-0.0.2/pulpo_dev.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      458 2023-10-11 09:11:04.000000 pulpo-dev-0.0.2/pulpo_dev.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-10-11 09:11:04.000000 pulpo-dev-0.0.2/pulpo_dev.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       78 2023-10-11 09:11:04.000000 pulpo-dev-0.0.2/pulpo_dev.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-10-11 09:11:04.000000 pulpo-dev-0.0.2/pulpo_dev.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-10-11 09:11:04.358548 pulpo-dev-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1023 2023-10-11 08:59:41.000000 pulpo-dev-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-10-11 09:11:04.356554 pulpo-dev-0.0.2/tests/
--rw-rw-rw-   0        0        0        0 2023-07-03 15:12:14.000000 pulpo-dev-0.0.2/tests/__init__.py
--rw-rw-rw-   0        0        0     6046 2023-10-05 10:56:55.000000 pulpo-dev-0.0.2/tests/sample_database.py
--rw-rw-rw-   0        0        0     4012 2023-10-10 18:13:23.000000 pulpo-dev-0.0.2/tests/test_functions.py
+drwxrwxrwx   0        0        0        0 2023-12-15 10:08:14.415817 pulpo-dev-0.0.3/
+-rw-rw-rw-   0        0        0     1553 2023-12-11 14:40:49.000000 pulpo-dev-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0       39 2023-12-13 18:18:53.000000 pulpo-dev-0.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     4541 2023-12-15 10:08:14.415817 pulpo-dev-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0    11321 2023-12-13 18:18:53.000000 pulpo-dev-0.0.3/README.md
+-rw-rw-rw-   0        0        0     3884 2023-12-13 18:18:53.000000 pulpo-dev-0.0.3/README_pypi.md
+drwxrwxrwx   0        0        0        0 2023-12-15 10:08:14.402904 pulpo-dev-0.0.3/pulpo/
+-rw-rw-rw-   0        0        0        0 2023-07-03 13:40:34.000000 pulpo-dev-0.0.3/pulpo/__init__.py
+-rw-rw-rw-   0        0        0     3520 2023-12-15 09:58:33.000000 pulpo-dev-0.0.3/pulpo/pulpo.py
+drwxrwxrwx   0        0        0        0 2023-12-15 10:08:14.406847 pulpo-dev-0.0.3/pulpo/utils/
+-rw-rw-rw-   0        0        0        0 2023-07-03 15:12:57.000000 pulpo-dev-0.0.3/pulpo/utils/__init__.py
+-rw-rw-rw-   0        0        0     4419 2023-12-15 09:58:33.000000 pulpo-dev-0.0.3/pulpo/utils/bw_parser.py
+-rw-rw-rw-   0        0        0     6372 2023-12-15 09:58:33.000000 pulpo-dev-0.0.3/pulpo/utils/converter.py
+-rw-rw-rw-   0        0        0     9852 2023-12-15 09:58:33.000000 pulpo-dev-0.0.3/pulpo/utils/optimizer.py
+-rw-rw-rw-   0        0        0     5566 2023-12-15 09:58:33.000000 pulpo-dev-0.0.3/pulpo/utils/saver.py
+-rw-rw-rw-   0        0        0     9628 2023-12-13 18:18:53.000000 pulpo-dev-0.0.3/pulpo/utils/tests.py
+drwxrwxrwx   0        0        0        0 2023-12-15 10:08:14.414820 pulpo-dev-0.0.3/pulpo_dev.egg-info/
+-rw-rw-rw-   0        0        0     4541 2023-12-15 10:08:14.000000 pulpo-dev-0.0.3/pulpo_dev.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      458 2023-12-15 10:08:14.000000 pulpo-dev-0.0.3/pulpo_dev.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-12-15 10:08:14.000000 pulpo-dev-0.0.3/pulpo_dev.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       78 2023-12-15 10:08:14.000000 pulpo-dev-0.0.3/pulpo_dev.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-12-15 10:08:14.000000 pulpo-dev-0.0.3/pulpo_dev.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-12-15 10:08:14.416813 pulpo-dev-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1023 2023-12-15 10:03:45.000000 pulpo-dev-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-12-15 10:08:14.414820 pulpo-dev-0.0.3/tests/
+-rw-rw-rw-   0        0        0        0 2023-07-03 15:12:14.000000 pulpo-dev-0.0.3/tests/__init__.py
+-rw-rw-rw-   0        0        0     6046 2023-10-05 10:56:55.000000 pulpo-dev-0.0.3/tests/sample_database.py
+-rw-rw-rw-   0        0        0     4756 2023-12-15 09:58:33.000000 pulpo-dev-0.0.3/tests/test_functions.py
```

### Comparing `pulpo-dev-0.0.2/LICENSE` & `pulpo-dev-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pulpo-dev-0.0.2/PKG-INFO` & `pulpo-dev-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulpo-dev
-Version: 0.0.2
+Version: 0.0.3
 Summary: pulpo package for optimization in LCI databases
 Home-page: https://github.com/flechtenberg/pulpo
 Author: Fabian Lechtenberg
 Author-email: fabian.lechtenberg@upc.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `pulpo-dev-0.0.2/README.md` & `pulpo-dev-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pulpo-dev-0.0.2/README_pypi.md` & `pulpo-dev-0.0.3/README_pypi.md`

 * *Files identical despite different names*

### Comparing `pulpo-dev-0.0.2/pulpo/pulpo.py` & `pulpo-dev-0.0.3/pulpo/pulpo.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,53 +2,55 @@
 from typing import List, Union
 import webbrowser
 
 class PulpoOptimizer:
     def __init__(self, project: str, database: str, method: Union[str, List[str], dict], directory: str):
         self.project = project
         self.database = database
+        self.intervention_matrix = 'biosphere3'
         self.method = converter.convert_to_dict(method)
         self.directory = directory
         self.lci_data = None
         self.instance = None
 
     def get_lci_data(self):
-        self.lci_data = bw_parser.import_data(self.project, self.database, self.method)
+        self.lci_data = bw_parser.import_data(self.project, self.database, self.method, self.intervention_matrix)
 
-    def instantiate(self, choices={}, demand={}, upper_limit={},lower_limit={}):
+    def instantiate(self, choices={}, demand={}, upper_limit={},lower_limit={}, upper_elem_limit={}):
         # Instantiate only for those methods that are part of the objecitve
         methods = {h: self.method[h] for h in self.method if self.method[h] !=0}
-        data = converter.combine_inputs(self.lci_data, demand, choices, upper_limit, lower_limit, methods)
+        data = converter.combine_inputs(self.lci_data, demand, choices, upper_limit, lower_limit, upper_elem_limit, methods)
         self.instance = optimizer.instantiate(data)
 
-    def solve(self, GAMS_PATH=False):
-        results, self.instance = optimizer.solve_model(self.instance, GAMS_PATH)
+    def solve(self, GAMS_PATH=False, options=None):
+        results, self.instance = optimizer.solve_model(self.instance, GAMS_PATH, options=options)
         # Post calculate additional methods, in case several methods have been specified and one of them is 0
         if not isinstance(self.method, str):
             if len(self.method) > 1 and 0 in [self.method[x] for x in self.method]:
                 self.instance = optimizer.calculate_methods(self.instance, self.lci_data, self.method)
+        self.instance = optimizer.calculate_inv_flows(self.instance, self.lci_data)
         return results
 
     def retrieve_activities(self, keys=None, activities=None, reference_products=None, locations=None):
-        activities = bw_parser.retrieve_activities(self.project, self.database, keys, activities, reference_products, locations)
+        activities = bw_parser.retrieve_processes(self.project, self.database, keys, activities, reference_products, locations)
         return activities
 
     def retrieve_envflows(self, keys=None, activities=None, categories=None):
-        activities = bw_parser.retrieve_envflows(self.project, keys, activities, categories)
+        activities = bw_parser.retrieve_env_interventions(project=self.project, intervention_matrix=self.intervention_matrix, keys=keys, activities=activities, categories=categories)
         return activities
 
     def retrieve_methods(self, string=""):
         methods = bw_parser.retrieve_methods(self.project, string)
         return methods
 
     def save_results(self, choices={}, constraints={}, demand={}, name='results.xlxs'):
-        saver.save_results(self.instance, self.project, self.database, choices, constraints, demand, self.lci_data['activity_map'], self.directory, name)
+        saver.save_results(self.instance, self.project, self.database, choices, constraints, demand, self.lci_data['process_map'], self.lci_data['intervention_map'], self.directory, name)
 
     def summarize_results(self, choices={}, constraints={}, demand={}, zeroes=False):
-            saver.summarize_results(self.instance, self.project, self.database, choices, constraints, demand, self.lci_data['activity_map'], zeroes)
+            saver.summarize_results(self.instance, self.project, self.database, choices, constraints, demand, self.lci_data['process_map'], zeroes)
 
 def electricity_showcase():
     github_url = 'https://github.com/flechtenberg/pulpo/blob/develop/notebooks/electricity_showcase.ipynb'  # Replace with your GitHub URL
     nbviewer_url = 'https://nbviewer.jupyter.org/github/' + github_url.split('github.com/')[1]
     webbrowser.open(nbviewer_url)
 
 def hydrogen_showcase():
```

### Comparing `pulpo-dev-0.0.2/pulpo/utils/bw_parser.py` & `pulpo-dev-0.0.3/pulpo/utils/bw_parser.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,93 +1,98 @@
 from typing import List, Union, Dict, Any
 from pathlib import Path
 import pickle
 import brightway2 as bw
 from scipy import sparse
 
-def import_data(project: str, database: str, method: Union[str, List[str], dict[str, int]]) -> Dict[str, Union[dict, Any]]:
-    """ TODO can we find a faster way to import the data without having to save it locally? """
+def import_data(project: str, database: str, method: Union[str, List[str], dict[str, int]], intervention_matrix_name: str) -> Dict[str, Union[dict, Any]]:
     """
     Main function to import LCI data for a project from a database.
-
-    :param project: The name of the Ecoinvent project.
-    :param database: The name of the Ecoinvent database.
-    :param method: The method(s) to evaluate. Can be a single method name or a list of method names.
-    :return: A dictionary with the relevant LCI data.
-
-    :rtype: dict[str, Union[dict, Any]]
     """
+
     # Set project and get database
     bw.projects.set_current(project)
     eidb = bw.Database(database)
     # Prepare methods
     if isinstance(method, str):
         method = [method]  # Convert single string to list of strings
     method = sorted(method)
     methods = retrieve_methods(project, method)
     # Get data
-    matrices = {}
+    characterization_matrices = {}
     rand_act = eidb.random()
     for method in methods:
         lca = bw.LCA({rand_act: 1}, method)
         lca.load_lci_data()
         lca.load_lcia_data()
-        matrices[str(method)] = lca.characterization_matrix
-    technosphere = lca.technosphere_matrix
-    biosphere = lca.biosphere_matrix
+        characterization_matrices[str(method)] = lca.characterization_matrix
+    technology_matrix = lca.technosphere_matrix
+    intervention_matrix = lca.biosphere_matrix
     # Create activity map key --> ID | ID --> description
-    activity_map = lca.product_dict
+    process_map = lca.product_dict
+
     for act in eidb:
-        activity_map[activity_map[act.key]] = str(act['name']) + ' | ' + str(act['reference product']) + ' | ' + str(
+        process_map[process_map[act.key]] = str(act['name']) + ' | ' + str(act['reference product']) + ' | ' + str(
             act['location'])
 
+    if intervention_matrix_name in bw.databases:
+        eidb_bio = bw.Database(intervention_matrix_name)
+        intervention_map = lca.biosphere_dict
+        for act in eidb_bio:
+            if act.key in intervention_map:
+                intervention_map[intervention_map[act.key]] = act['name'] + ' | ' + str(act['categories'])
+    else:
+        print("The name of the biosphere is not '" + intervention_matrix_name + "'. Please specify the correct biosphere.")
+        return {}
+
     lci_data = {
-        'matrices': matrices,
-        'biosphere': biosphere,
-        'technosphere': technosphere,
-        'activity_map': activity_map
+        'matrices': characterization_matrices,
+        'intervention_matrix': intervention_matrix,
+        'technology_matrix': technology_matrix,
+        'process_map': process_map,
+        'intervention_map': intervention_map,
     }
 
     return lci_data
 
 
-def retrieve_activities(project, database, keys=None, activities=None, reference_products=None, locations=None):
+def retrieve_processes(project, database, keys=None, activities=None, reference_products=None, locations=None):
     """
     Retrieve activities from a database based on specified keys, activities, reference products, and locations.
     """
 
     bw.projects.set_current(project)
     eidb = bw.Database(database)
 
     if keys is not None:
         if isinstance(keys, str):
             keys = [keys]
         keys = [eval(key) for key in keys]
-        return [act for act in eidb if act.key in keys]
+        return [proc for proc in eidb if proc.key in keys]
 
-    matching_activities = []
+    matching_processes = []
 
-    for act in eidb:
-        if (activities is None or act['name'] in activities) and \
-                (reference_products is None or act['reference product'] in reference_products) and \
-                (locations is None or act['location'] in locations):
-            matching_activities.append(act)
+    for proc in eidb:
+        if (activities is None or proc['name'] in activities) and \
+                (reference_products is None or proc['reference product'] in reference_products) and \
+                (locations is None or proc['location'] in locations):
+            matching_processes.append(proc)
 
-    if not matching_activities:
+    if not matching_processes:
         print("No activities match the given specifications or the input format is incorrect.")
     else:
-        return matching_activities
+        return matching_processes
 
-def retrieve_envflows(project, biosphere='biosphere3', keys=None, activities=None, categories=None):
+def retrieve_env_interventions(project='', intervention_matrix='biosphere3', keys=None, activities=None, categories=None):
     """
     Retrieve environmental flows from the biosphere database based on specified keys, activities, and categories.
     """
 
     bw.projects.set_current(project)
-    eidb = bw.Database(biosphere)
+    eidb = bw.Database(intervention_matrix)
 
     if keys is not None:
         if isinstance(keys, str):
             keys = [keys]
         keys = [eval(key) for key in keys]
         return [flow for flow in eidb if flow.key in keys]
 
@@ -104,13 +109,7 @@
         return matching_flows
 
 
 def retrieve_methods(project: str, sub_string: List[str]):
     ''' This function retrieves all the methods that contain the specified list of substrings'''
     bw.projects.set_current(project)
     return [method for method in bw.methods if any([x.lower() in str(method).lower() for x in sub_string])]
-
-def main():
-    1+1
-
-if __name__ == "__main__":
-    main()
```

### Comparing `pulpo-dev-0.0.2/pulpo/utils/optimizer.py` & `pulpo-dev-0.0.3/pulpo/utils/optimizer.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,148 +2,167 @@
 
 def create_model():
     """Builds an abstract model on top of the ecoinvent database."""
     model = pyo.AbstractModel()
 
     # Sets
     model.PRODUCT = pyo.Set(doc='Set of intermediate products (or technosphere exchanges), indexed by i')
-    model.PROCESS = pyo.Set(doc='Set of processes (or activities), indexed by p')
-    model.ELEMENTARY = pyo.Set(doc='Set of elementary flows, indexed by e')
+    model.PROCESS = pyo.Set(doc='Set of processes (or activities), indexed by j')
+    model.ENV_COST = pyo.Set(doc='Set of environmental cost flows, indexed by e')
     model.INDICATOR = pyo.Set(doc='Set of impact assessment indicators, indexed by h')
-    model.ELEMENTARY_PROCESS = pyo.Set(within=model.ELEMENTARY * model.PROCESS * model.INDICATOR, doc='Relation set between elementary flows and processes')
-    model.ELEMENTARY_IN = pyo.Set(model.INDICATOR, within=model.ELEMENTARY)
-    model.ELEMENTARY_OUT = pyo.Set(model.ELEMENTARY * model.INDICATOR, within=model.PROCESS)
-    model.PROCESS_IN = pyo.Set(model.PROCESS, within=model.PRODUCT, doc='Subset of intermediate products i produced/absorbed by process p')
-    model.PROCESS_OUT = pyo.Set(model.PRODUCT, within=model.PROCESS, doc='Subset of processes p that produce/absorb intermediate product i')
+    model.INV = pyo.Set(doc='Set of intervention flows, indexed by g')
+    model.ENV_COST_PROCESS = pyo.Set(within=model.ENV_COST * model.PROCESS * model.INDICATOR, doc='Relation set between environmental cost flows and processes')
+    model.ENV_COST_IN = pyo.Set(model.INDICATOR, within=model.ENV_COST)
+    model.ENV_COST_OUT = pyo.Set(model.ENV_COST * model.INDICATOR, within=model.PROCESS)
+    model.PROCESS_IN = pyo.Set(model.PROCESS, within=model.PRODUCT)
+    model.PROCESS_OUT = pyo.Set(model.PRODUCT, within=model.PROCESS)
     model.PRODUCT_PROCESS = pyo.Set(within=model.PRODUCT * model.PROCESS, doc='Relation set between intermediate products and processes')
+    model.INV_PROCESS = pyo.Set(within=model.INV * model.PROCESS, doc='Relation set between environmental flows and processes')
+    model.INV_OUT = pyo.Set(model.INV, within=model.PROCESS)
 
     # Parameters
-    model.UPPER_LIMIT = pyo.Param(model.PROCESS, mutable=True, within=pyo.Reals, doc='Maximum production capacity of process p')
-    model.LOWER_LIMIT = pyo.Param(model.PROCESS, mutable=True, within=pyo.Reals, doc='Minimum production capacity of process p')
-    model.ELEMENTARY_MATRIX = pyo.Param(model.ELEMENTARY_PROCESS, mutable=True, doc='Biosphere Impact matrix Q*B describing the elementary flow e entering/leaving process p')
-    model.FINAL_DEMAND = pyo.Param(model.PRODUCT, mutable=True, within=pyo.Reals, doc='Final demand of intermediate flows (i.e., functional unit)')
+    model.UPPER_LIMIT = pyo.Param(model.PROCESS, mutable=True, within=pyo.Reals, doc='Maximum production capacity of process j')
+    model.LOWER_LIMIT = pyo.Param(model.PROCESS, mutable=True, within=pyo.Reals, doc='Minimum production capacity of process j')
+    model.UPPER_INV_LIMIT = pyo.Param(model.INV, mutable=True, within=pyo.Reals, doc='Maximum intervention flow flow g')
+    model.ENV_COST_MATRIX = pyo.Param(model.ENV_COST_PROCESS, mutable=True, doc='Enviornmental cost matrix Q*B describing the environmental cost flows e associated to process j')
+    model.INV_MATRIX = pyo.Param(model.INV_PROCESS, mutable=True, doc='Intervention matrix B describing the intervention flow g entering/leaving process j')
+    model.FINAL_DEMAND = pyo.Param(model.PRODUCT, mutable=True, within=pyo.Reals, doc='Final demand of intermediate product flows (i.e., functional unit)')
     model.SUPPLY = pyo.Param(model.PRODUCT, mutable=True, within=pyo.Binary, doc='Binary parameter which specifies whether or not a supply has been specified instead of a demand')
-    model.TECH_MATRIX = pyo.Param(model.PRODUCT_PROCESS, mutable=True, doc='Technology matrix A describing the intermediate product i produced/absorbed by process p')
+    model.TECH_MATRIX = pyo.Param(model.PRODUCT_PROCESS, mutable=True, doc='Technology matrix A describing the intermediate product i produced/absorbed by process j')
     model.WEIGHTS = pyo.Param(model.INDICATOR, mutable=True, within=pyo.NonNegativeReals, doc='Weighting factors for the impact assessment indicators in the objective function')
 
     # Variables
     model.impacts = pyo.Var(model.INDICATOR, bounds=(-1e24, 1e24), doc='Environmental impact on indicator h evaluated with the established LCIA method')
     model.scaling_vector = pyo.Var(model.PROCESS, bounds=(-1e24, 1e24), doc='Activity level of each process to meet the final demand')
+    model.inv_vector = pyo.Var(model.INV, bounds=(-1e24, 1e24), doc='Intervention flows')
     model.slack = pyo.Var(model.PRODUCT, bounds=(0, 1e24), doc='Supply slack variables')
 
     # Building rules for sets
-    model.Env = pyo.BuildAction(rule=populate_env)
-    model.In_n_Out = pyo.BuildAction(rule=populate_in_and_out)
+    model.Env_in_out = pyo.BuildAction(rule=populate_env)
+    model.Process_in_out = pyo.BuildAction(rule=populate_in_and_out)
+    model.Inv_in_out = pyo.BuildAction(rule=populate_inv)
 
     # Constraints
     model.FINAL_DEMAND_CNSTR = pyo.Constraint(model.PRODUCT, rule=demand_constraint)
     model.IMPACTS_CNSTR = pyo.Constraint(model.INDICATOR, rule=impact_constraint)
+    model.INVENTORY_CNSTR = pyo.Constraint(model.INV, rule=inventory_constraint)
     model.UPPER_CNSTR = pyo.Constraint(model.PROCESS, rule=upper_constraint)
     model.LOWER_CNSTR = pyo.Constraint(model.PROCESS, rule=lower_constraint)
     model.SLACK_CNSTR = pyo.Constraint(model.PRODUCT, rule=slack_constraint)
+    model.INV_CNSTR = pyo.Constraint(model.INV, rule=upper_env_constraint)
 
     # Objective function
     model.OBJ = pyo.Objective(sense=pyo.minimize, rule=objective_function)
 
     return model
 
 
 # Rule functions
 def populate_env(model):
     """Relates the environmental flows to the processes."""
-    for i, j, h in model.ELEMENTARY_PROCESS:
-        if i not in model.ELEMENTARY_IN[h]:
-            model.ELEMENTARY_IN[h].add(i)
-        model.ELEMENTARY_OUT[i, h].add(j)
+    for i, j, h in model.ENV_COST_PROCESS:
+        if i not in model.ENV_COST_IN[h]:
+            model.ENV_COST_IN[h].add(i)
+        model.ENV_COST_OUT[i, h].add(j)
 
 
 def populate_in_and_out(model):
     """Relates the inputs of an activity to its outputs."""
     for i, j in model.PRODUCT_PROCESS:
         model.PROCESS_OUT[i].add(j)
         model.PROCESS_IN[j].add(i)
 
+def populate_inv(model):
+    """Relates the impacts to the environmental flows"""
+    for a, j in model.INV_PROCESS:
+        model.INV_OUT[a].add(j)
 
 def demand_constraint(model, i):
     """Fixes a value in the demand vector"""
-    return sum(model.TECH_MATRIX[i, p] * model.scaling_vector[p] for p in model.PROCESS_OUT[i]) == model.FINAL_DEMAND[i] + model.slack[i]
+    return sum(model.TECH_MATRIX[i, j] * model.scaling_vector[j] for j in model.PROCESS_OUT[i]) == model.FINAL_DEMAND[i] + model.slack[i]
 
 
 def impact_constraint(model, h):
     """Calculates all the impact categories"""
-    return model.impacts[h] == sum(sum(model.ELEMENTARY_MATRIX[i, j, h] * model.scaling_vector[j] for j in model.ELEMENTARY_OUT[i, h]) for i in model.ELEMENTARY_IN[h])
+    return model.impacts[h] == sum(sum(model.ENV_COST_MATRIX[i, j, h] * model.scaling_vector[j] for j in model.ENV_COST_OUT[i, h]) for i in model.ENV_COST_IN[h])
 
+def inventory_constraint(model, g):
+    """Calculates the environmental flows"""
+    return model.inv_vector[g] == sum(model.INV_MATRIX[g, j] * model.scaling_vector[j] for j in model.INV_OUT[g])
 
-def upper_constraint(model, p):
+
+def upper_constraint(model, j):
     """Ensures that variables are within capacities (Maximum production constraint) """
-    return model.scaling_vector[p] <= model.UPPER_LIMIT[p]
+    return model.scaling_vector[j] <= model.UPPER_LIMIT[j]
 
 
-def lower_constraint(model, p):
+def lower_constraint(model, j):
     """ Minimum production constraint """
-    return model.scaling_vector[p] >= model.LOWER_LIMIT[p]
+    return model.scaling_vector[j] >= model.LOWER_LIMIT[j]
+
+def upper_env_constraint(model, g):
+    """Ensures that variables are within capacities (Maximum production constraint) """
+    return model.inv_vector[g] <= model.UPPER_INV_LIMIT[g]
 
-def slack_constraint(model, p):
+def slack_constraint(model, j):
     """ Slack variable upper limit for activities where supply is specified instead of demand """
-    return model.slack[p] <= 1e20 * model.SUPPLY[p]
+    return model.slack[j] <= 1e20 * model.SUPPLY[j]
 
 
 def objective_function(model):
     """Objective is a sum over all indicators with weights. Typically, the indicator of study has weight 1, the rest 0"""
     return sum(model.impacts[h] * model.WEIGHTS[h] for h in model.INDICATOR)
 
 def calculate_methods(instance, lci_data, methods):
     '''
     This function calculates the impacts if a method with weight 0 has been specified
     '''
     import scipy.sparse as sparse
     import numpy as np
     matrices = lci_data['matrices']
-    biosphere = lci_data['biosphere']
+    intervention_matrix = lci_data['intervention_matrix']
     matrices = {h: matrices[h] for h in matrices if str(h) in methods}
-    env_cost = {h: sparse.csr_matrix.dot(matrices[h], biosphere) for h in matrices}
+    env_cost = {h: sparse.csr_matrix.dot(matrices[h], intervention_matrix) for h in matrices}
     try:
         scaling_vector = np.array([instance.scaling_vector[x].value for x in instance.scaling_vector])
     except:
         scaling_vector = np.array([instance.scaling_vector[x] for x in instance.scaling_vector])
     impacts = {}
     for h in matrices:
         impacts[h] = sum(env_cost[h].dot(scaling_vector))
     instance.impacts_calculated = pyo.Var([h for h in impacts], initialize=impacts)
     return instance
 
+def calculate_inv_flows(instance, lci_data):
+    '''
+    This function calculates elementary flows post-optimization
+    '''
+    import numpy as np
+    intervention_matrix = lci_data['intervention_matrix']
+    try:
+        scaling_vector = np.array([instance.scaling_vector[x].value for x in instance.scaling_vector])
+    except:
+        scaling_vector = np.array([instance.scaling_vector[x] for x in instance.scaling_vector])
+    flows = intervention_matrix.dot(scaling_vector)
+    instance.inv_flows = pyo.Var(range(0, intervention_matrix.shape[0]), initialize=flows)
+    return instance
+
 
 
 def instantiate(model_data):
     """ This function builds an instance of the optimization model with specific data and objective function"""
     print('Creating Instance')
     model = create_model()
     problem = model.create_instance(model_data, report_timing=False)
     print('Instance created')
     return problem
 
 
 def solve_model(model_instance, gams_path, options=None):
-    """ TODO enable ipopt or other free solver application! """
-    """Solves the instance of the optimization model.
-
-    Parameters:
-    ------------
-    model_instance: pyomo.ConcreteModel
-        The instance of the Pyomo model to solve.
-    gams_path: str
-        The directory path of GAMS.
-    options: list of str, optional
-        Additional solver options.
-
-    Returns:
-    ------------
-    pyomo.SolverResults, pyomo.ConcreteModel
-        The solver results and the updated instance of the Pyomo model.
-    """
+    """Solves the instance of the optimization model. """
     if gams_path is not False:
         pyo.pyomo.common.Executable('gams').set_path(gams_path)
         solver = pyo.SolverFactory('gams')
         print('GAMS solvers library availability:', solver.available())
         print('Solver path:', solver.executable())
 
         io_options = {
@@ -164,23 +183,22 @@
                 #'eprhs=1E-9',
                 '$offecho',
             ]
 
         results = solver.solve(
             model_instance,
             keepfiles=True,
+            symbolic_solver_labels=True,
             tee=True,
             report_timing=True,
             io_options=io_options,
             add_options=options
         )
 
         model_instance.solutions.load_from(results)
 
     else:
         from pyomo.contrib import appsi
         opt = appsi.solvers.Highs()
         results = opt.solve(model_instance)
 
-    return results, model_instance
-
-
+    return results, model_instance
```

### Comparing `pulpo-dev-0.0.2/pulpo/utils/saver.py` & `pulpo-dev-0.0.3/pulpo/utils/saver.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import pyomo.environ as pyo
 from pyomo.repn.plugins.baron_writer import *
 import pandas as pd
 from pathlib import Path
 from IPython.display import display
 
-def save_results(instance, project, database, choices, constraints, demand, map, directory, name):
+def save_results(instance, project, database, choices, constraints, demand, process_map, itervention_map, directory, name):
     """ TODO Imporve readability and structure ...
     There must be a better way to save the outputs of a pyomo model than this code I developed in 2020 """
     # Check if data/results folder exists, if not create it
     Path(directory + '/results').mkdir(parents=True, exist_ok=True)
 
     # Recover dictionary values
     list_of_vars = []
@@ -19,103 +19,106 @@
 
     # Open xlsx writer
     writer = pd.ExcelWriter(directory + '/results/' + name, engine='xlsxwriter')
 
     # Raw results
     for v in list_of_vars:
         try:
-            data = [(k, map[k], v) for k, v in v._data.items()]
+            if str(v) == 'inv_flows' or str(v) == 'inv_vector':
+                data = [(k, itervention_map[k], v) for k, v in v._data.items()]
+            else:
+                data = [(k, process_map[k], v) for k, v in v._data.items()]
             df = pd.DataFrame(data, columns=['ID', 'Activity', 'Value'])
         except:
             data = [(k, v) for k, v in v._data.items()]
             df = pd.DataFrame(data, columns=['Key', 'Value'])
         df.sort_values(by=['Value'], inplace=True, ascending=False)
         df.to_excel(writer, sheet_name=v.name, index=False)
 
-    # Store the metadata of the TCM
+    # Store the metadata
     pd.DataFrame([project + '__' + database]).to_excel(writer, sheet_name='project and db')
 
     metadata = {}
     for choice in choices:
         i = 0
         temp_dict = []
         for alt in choices[choice]:
-            temp_dict.append((alt, i, instance.scaling_vector[map[alt.key]]))
+            temp_dict.append((alt, i, instance.scaling_vector[process_map[alt.key]]))
             i+=1
-        metadata[(choice, 'Activity')] = {'Activity ' + str(i): map[map[alt.key]] for alt, i, val in temp_dict}
+        metadata[(choice, 'Activity')] = {'Activity ' + str(i): process_map[process_map[alt.key]] for alt, i, val in temp_dict}
         metadata[(choice, 'Capacity')] = {'Activity ' + str(i): choices[choice][alt] for alt, i, val in temp_dict}
         metadata[(choice, 'Value')] = {'Activity ' + str(i): x for alt, i, x in temp_dict}
 
     pd.DataFrame(metadata).to_excel(writer, sheet_name='choices')
 
     metadata = {}
-    metadata['Demand'] = {map[map[key]]: demand[key] for key in demand}
+    metadata['Demand'] = {process_map[process_map[key]]: demand[key] for key in demand}
     pd.DataFrame(metadata).to_excel(writer, sheet_name='demand')
 
     metadata = {}
-    metadata['Demand'] = {map[map[key]]: constraints[key] for key in constraints}
+    metadata['Demand'] = {process_map[process_map[key]]: constraints[key] for key in constraints}
     pd.DataFrame(metadata).to_excel(writer, sheet_name='constraints')
 
     # Save xlsx file
     writer.close()
     return
 
-def summarize_results(instance, project, database, choices, constraints, demand, map, zeroes):
+def summarize_results(instance, project, database, choices, constraints, demand, process_map, zeroes):
     metadata = {}
-    metadata['Demand'] = {map[map[key]]: demand[key] for key in demand}
+    metadata['Demand'] = {process_map[process_map[key]]: demand[key] for key in demand}
     print('The following demand / functional unit has been specified: ')
     display(pd.DataFrame(metadata))
 
     # Recover dictionary values
     list_of_vars = []
     for v in instance.component_objects(ctype=pyo.Var, active=True, descend_into=True):
         for e in v._data:
             v._data[e] = value(v[e])
         list_of_vars.append(v)
 
     # Raw results
     for v in list_of_vars:
         if v.name == 'impacts':
             try:
-                data = [(k, map[k], v) for k, v in v._data.items()]
+                data = [(k, process_map[k], v) for k, v in v._data.items()]
                 df = pd.DataFrame(data, columns=['ID', 'Activity', 'Value'])
             except:
                 data = [(k, v) for k, v in v._data.items()]
                 df = pd.DataFrame(data, columns=['Key', 'Value'])
             df.sort_values(by=['Value'], inplace=True, ascending=False)
             print('\nThese are the impacts contained in the objective:')
             display(df)
 
         if v.name == 'impacts_calculated':
             try:
-                data = [(k, map[k], v) for k, v in v._data.items()]
+                data = [(k, process_map[k], v) for k, v in v._data.items()]
                 df = pd.DataFrame(data, columns=['ID', 'Activity', 'Value'])
             except:
                 data = [(k, v) for k, v in v._data.items()]
                 df = pd.DataFrame(data, columns=['Key', 'Value'])
             df.sort_values(by=['Value'], inplace=True, ascending=False)
             print('\nThe following impacts were calculated: ')
             display(df)
 
     print('\nThe following choices were made: ')
     for choice in choices:
         metadata = {}
         i = 0
         temp_dict = []
         for alt in choices[choice]:
-            if zeroes == False or instance.scaling_vector[map[alt.key]] != 0:
-                temp_dict.append((alt, i, instance.scaling_vector[map[alt.key]]))
+            if zeroes == False or instance.scaling_vector[process_map[alt.key]] != 0:
+                temp_dict.append((alt, i, instance.scaling_vector[process_map[alt.key]]))
                 i += 1
-        metadata[(choice, 'Activity')] = {'Activity ' + str(i): map[map[alt.key]] for alt, i, val in temp_dict}
+        metadata[(choice, 'Activity')] = {'Activity ' + str(i): process_map[process_map[alt.key]] for alt, i, val in temp_dict}
         metadata[(choice, 'Capacity')] = {'Activity ' + str(i): choices[choice][alt] for alt, i, val in temp_dict}
         metadata[(choice, 'Value')] = {'Activity ' + str(i): x for alt, i, x in temp_dict}
         print(choice)
         display(pd.DataFrame(metadata))
 
     if constraints == {}:
         print('No additional constraints have been passed.')
     else:
         metadata = {}
-        metadata['Constraints'] = {map[map[key]]: constraints[key] for key in constraints}
+        metadata['Constraints'] = {process_map[process_map[key]]: constraints[key] for key in constraints}
         print('\nThe following constraints were implemented and oblieged: ')
         display(pd.DataFrame(metadata))
```

### Comparing `pulpo-dev-0.0.2/pulpo/utils/tests.py` & `pulpo-dev-0.0.3/pulpo/utils/tests.py`

 * *Files identical despite different names*

### Comparing `pulpo-dev-0.0.2/pulpo_dev.egg-info/PKG-INFO` & `pulpo-dev-0.0.3/pulpo_dev.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulpo-dev
-Version: 0.0.2
+Version: 0.0.3
 Summary: pulpo package for optimization in LCI databases
 Home-page: https://github.com/flechtenberg/pulpo
 Author: Fabian Lechtenberg
 Author-email: fabian.lechtenberg@upc.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `pulpo-dev-0.0.2/setup.py` & `pulpo-dev-0.0.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Open and read the contents of the README file
 with open('README_pypi.md', 'r', encoding='utf-8') as readme_file:
     long_description = readme_file.read()
 
 setup(
     name="pulpo-dev",
-    version="0.0.2",
+    version="0.0.3",
     description="pulpo package for optimization in LCI databases",
     author="Fabian Lechtenberg",
     author_email="fabian.lechtenberg@upc.edu",
     url="https://github.com/flechtenberg/pulpo",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: BSD License",
```

### Comparing `pulpo-dev-0.0.2/tests/sample_database.py` & `pulpo-dev-0.0.3/tests/sample_database.py`

 * *Files identical despite different names*

### Comparing `pulpo-dev-0.0.2/tests/test_functions.py` & `pulpo-dev-0.0.3/tests/test_functions.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import pulpo as pulpo
 import unittest
 from tests.sample_database import sample_lcia, setup_test_db
-from pulpo.utils.bw_parser import import_data, retrieve_methods, retrieve_envflows, retrieve_activities
+from pulpo.utils.bw_parser import import_data, retrieve_methods, retrieve_env_interventions, retrieve_processes
 from pulpo import pulpo
 
 setup_test_db()
 
 class TestParser(unittest.TestCase):
     def test_database_import(self):
         result = sample_lcia()
@@ -15,65 +15,76 @@
         # Test if the import works and has the expected structure
         methods = {
             "('my project', 'climate change')": 1,
             "('my project', 'air quality')": 1,
             "('my project', 'resources')": 1,
         }
 
-        result = import_data('sample_project', 'technosphere', methods)
+        result = import_data('sample_project', 'technosphere', methods, 'biosphere')
 
-        self.assertEqual([idx for idx in result], ['matrices', 'biosphere', 'technosphere', 'activity_map'])
-        self.assertEqual(result['technosphere'].shape, (5, 5))
-        self.assertEqual(result['biosphere'].shape, (4, 5))
-        self.assertEqual(result['activity_map'], {('technosphere', 'oil extraction'): 0, ('technosphere', 'lignite extraction'): 1, ('technosphere', 'steam cycle'): 2, ('technosphere', 'wind turbine'): 3, ('technosphere', 'e-Car'): 4, 2: 'steam cycle | electricity | GLO', 1: 'lignite extraction | lignite | GLO', 0: 'oil extraction | oil | GLO', 3: 'wind turbine | electricity | GLO', 4: 'e-Car | transport | GLO'})
+        self.assertEqual([idx for idx in result], ['matrices', 'intervention_matrix', 'technology_matrix', 'process_map', 'intervention_map'])
+        self.assertEqual(result['technology_matrix'].shape, (5, 5))
+        self.assertEqual(result['intervention_matrix'].shape, (4, 5))
+        self.assertEqual(result['process_map'], {('technosphere', 'oil extraction'): 0, ('technosphere', 'lignite extraction'): 1, ('technosphere', 'steam cycle'): 2, ('technosphere', 'wind turbine'): 3, ('technosphere', 'e-Car'): 4, 2: 'steam cycle | electricity | GLO', 1: 'lignite extraction | lignite | GLO', 0: 'oil extraction | oil | GLO', 3: 'wind turbine | electricity | GLO', 4: 'e-Car | transport | GLO'})
 
     def test_retrieve_activities(self):
-        key = retrieve_activities('sample_project', 'technosphere', keys=["('technosphere', 'wind turbine')"])
-        name = retrieve_activities('sample_project', 'technosphere', activities=['e-Car'])
-        location = retrieve_activities('sample_project', 'technosphere', locations=['GLO'])
+        key = retrieve_processes('sample_project', 'technosphere', keys=["('technosphere', 'wind turbine')"])
+        name = retrieve_processes('sample_project', 'technosphere', activities=['e-Car'])
+        location = retrieve_processes('sample_project', 'technosphere', locations=['GLO'])
         self.assertEqual(key[0]['name'], "wind turbine")
         self.assertEqual(name[0]['name'], "e-Car")
         self.assertEqual(len(location), 5)
 
     def test_retrieve_methods(self):
         single_result = retrieve_methods('sample_project', ['climate'])
         multi_result = retrieve_methods('sample_project', ['project'])
         self.assertEqual(single_result, [('my project', 'climate change')])
         self.assertEqual(multi_result, [('my project', 'climate change'), ('my project', 'air quality'), ('my project', 'resources')])
 
     def test_retrieve_envflows(self):
-        result = retrieve_envflows('sample_project', biosphere='biosphere', keys="('biosphere', 'PM')")
+        result = retrieve_env_interventions('sample_project', intervention_matrix='biosphere', keys="('biosphere', 'PM')")
         self.assertEqual(result[0]['name'], 'Particulate matter, industrial')
 
 class TestPULPO(unittest.TestCase):
 
     def test_pulpo(self):
         project = 'sample_project'
         database = 'technosphere'
         methods = {"('my project', 'climate change')": 1,
                    "('my project', 'air quality')": 1,
                    "('my project', 'resources')": 0}
-
+        # Test basic PULPO:
         worker = pulpo.PulpoOptimizer(project, database, methods, '')
+        worker.intervention_matrix = 'biosphere'
         worker.get_lci_data()
         eCar = worker.retrieve_activities(reference_products='transport')
         demand = {eCar[0]: 1}
         elec = worker.retrieve_activities(reference_products='electricity')
         choices = {'electricity': {elec[0]: 100, elec[1]: 100}}
         worker.instantiate(choices=choices, demand=demand)
         worker.solve()
         result_obj = round(worker.instance.OBJ(), 6)
         result_aux = round(worker.instance.impacts_calculated["('my project', 'resources')"].value, 5)
         self.assertEqual(result_obj, 0.103093)
         self.assertEqual(result_aux, 5.25773)
-
+        # Test supply specification:
         upper_limit = {eCar[0]: 1}
         lower_limit = {eCar[0]: 1}
         worker.instantiate(choices=choices, upper_limit=upper_limit, lower_limit=lower_limit)
         worker.solve()
         result_obj = round(worker.instance.OBJ(), 6)
         result_aux = round(worker.instance.impacts_calculated["('my project', 'resources')"].value, 5)
         self.assertEqual(result_obj, 0.1)
         self.assertEqual(result_aux, 5.1)
+        # Test elementary / intervention flow constraint:
+        water = worker.retrieve_envflows(activities="Water, irrigation")
+        upper_elem_limit = {water[0]: 5.2}
+        worker.instantiate(choices=choices, demand=demand, upper_elem_limit=upper_elem_limit)
+        worker.solve()
+        result_obj = round(worker.instance.OBJ(), 6)
+        result_aux = round(worker.instance.impacts_calculated["('my project', 'resources')"].value, 5)
+        self.assertEqual(result_obj, 0.14237)
+        self.assertEqual(result_aux, 5.2)
+
```

