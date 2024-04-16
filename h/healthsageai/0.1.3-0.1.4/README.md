# Comparing `tmp/healthsageai-0.1.3.tar.gz` & `tmp/healthsageai-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "healthsageai-0.1.3.tar", last modified: Thu Apr  4 11:01:03 2024, max compression
+gzip compressed data, was "healthsageai-0.1.4.tar", last modified: Tue Apr 16 08:31:47 2024, max compression
```

## Comparing `healthsageai-0.1.3.tar` & `healthsageai-0.1.4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 a.groen    (501) staff       (20)        0 2024-04-04 11:01:03.142219 healthsageai-0.1.3/
--rw-r--r--   0 a.groen    (501) staff       (20)    34523 2023-12-01 10:10:21.000000 healthsageai-0.1.3/LICENSE
--rw-r--r--   0 a.groen    (501) staff       (20)    47022 2024-04-04 11:01:03.141871 healthsageai-0.1.3/PKG-INFO
--rw-r--r--   0 a.groen    (501) staff       (20)     5699 2024-04-04 09:53:35.000000 healthsageai-0.1.3/README.md
--rw-r--r--   0 a.groen    (501) staff       (20)     1505 2024-04-04 09:53:35.000000 healthsageai-0.1.3/pyproject.toml
--rw-r--r--   0 a.groen    (501) staff       (20)       38 2024-04-04 11:01:03.142280 healthsageai-0.1.3/setup.cfg
-drwxr-xr-x   0 a.groen    (501) staff       (20)        0 2024-04-04 11:01:03.137376 healthsageai-0.1.3/src/
--rw-r--r--   0 a.groen    (501) staff       (20)        0 2024-01-17 13:46:31.000000 healthsageai-0.1.3/src/__init__.py
-drwxr-xr-x   0 a.groen    (501) staff       (20)        0 2024-04-04 11:01:03.136272 healthsageai-0.1.3/src/healthsageai/
-drwxr-xr-x   0 a.groen    (501) staff       (20)        0 2024-04-04 11:01:03.138609 healthsageai-0.1.3/src/healthsageai/note_to_fhir/
--rw-r--r--   0 a.groen    (501) staff       (20)        0 2024-02-14 08:50:05.000000 healthsageai-0.1.3/src/healthsageai/note_to_fhir/__init__.py
--rw-r--r--   0 a.groen    (501) staff       (20)     2950 2024-04-04 09:53:35.000000 healthsageai-0.1.3/src/healthsageai/note_to_fhir/data_utils.py
-drwxr-xr-x   0 a.groen    (501) staff       (20)        0 2024-04-04 11:01:03.139954 healthsageai-0.1.3/src/healthsageai/note_to_fhir/evaluation/
--rw-r--r--   0 a.groen    (501) staff       (20)        0 2024-02-14 08:50:05.000000 healthsageai-0.1.3/src/healthsageai/note_to_fhir/evaluation/__init__.py
--rw-r--r--   0 a.groen    (501) staff       (20)     4644 2024-04-04 09:53:35.000000 healthsageai-0.1.3/src/healthsageai/note_to_fhir/evaluation/datamodels.py
--rw-r--r--   0 a.groen    (501) staff       (20)     3592 2024-04-04 09:53:35.000000 healthsageai-0.1.3/src/healthsageai/note_to_fhir/evaluation/fhirmodels.py
--rw-r--r--   0 a.groen    (501) staff       (20)    19893 2024-04-04 09:53:35.000000 healthsageai-0.1.3/src/healthsageai/note_to_fhir/evaluation/utils.py
--rw-r--r--   0 a.groen    (501) staff       (20)     3660 2024-02-14 08:50:05.000000 healthsageai-0.1.3/src/healthsageai/note_to_fhir/evaluation/visuals.py
-drwxr-xr-x   0 a.groen    (501) staff       (20)        0 2024-04-04 11:01:03.140696 healthsageai-0.1.3/src/healthsageai/note_to_fhir/inference/
--rw-r--r--   0 a.groen    (501) staff       (20)      104 2024-02-14 08:50:05.000000 healthsageai-0.1.3/src/healthsageai/note_to_fhir/inference/__init__.py
--rw-r--r--   0 a.groen    (501) staff       (20)     3315 2024-02-14 08:50:05.000000 healthsageai-0.1.3/src/healthsageai/note_to_fhir/inference/note_to_fhir.py
--rw-r--r--   0 a.groen    (501) staff       (20)     2039 2024-02-14 08:50:05.000000 healthsageai-0.1.3/src/healthsageai/note_to_fhir/parsers.py
-drwxr-xr-x   0 a.groen    (501) staff       (20)        0 2024-04-04 11:01:03.140916 healthsageai-0.1.3/src/healthsageai/note_to_fhir/templates/
--rw-r--r--   0 a.groen    (501) staff       (20)     2480 2024-02-14 08:50:05.000000 healthsageai-0.1.3/src/healthsageai/note_to_fhir/templates/simple.py
-drwxr-xr-x   0 a.groen    (501) staff       (20)        0 2024-04-04 11:01:03.141260 healthsageai-0.1.3/src/healthsageai.egg-info/
--rw-r--r--   0 a.groen    (501) staff       (20)    47022 2024-04-04 11:01:03.000000 healthsageai-0.1.3/src/healthsageai.egg-info/PKG-INFO
--rw-r--r--   0 a.groen    (501) staff       (20)      797 2024-04-04 11:01:03.000000 healthsageai-0.1.3/src/healthsageai.egg-info/SOURCES.txt
--rw-r--r--   0 a.groen    (501) staff       (20)        1 2024-04-04 11:01:03.000000 healthsageai-0.1.3/src/healthsageai.egg-info/dependency_links.txt
--rw-r--r--   0 a.groen    (501) staff       (20)      157 2024-04-04 11:01:03.000000 healthsageai-0.1.3/src/healthsageai.egg-info/requires.txt
--rw-r--r--   0 a.groen    (501) staff       (20)       35 2024-04-04 11:01:03.000000 healthsageai-0.1.3/src/healthsageai.egg-info/top_level.txt
+drwxr-xr-x   0 a.groen    (501) staff       (20)        0 2024-04-16 08:31:47.253445 healthsageai-0.1.4/
+-rw-r--r--   0 a.groen    (501) staff       (20)    34523 2023-12-01 10:10:21.000000 healthsageai-0.1.4/LICENSE
+-rw-r--r--   0 a.groen    (501) staff       (20)    47022 2024-04-16 08:31:47.253016 healthsageai-0.1.4/PKG-INFO
+-rw-r--r--   0 a.groen    (501) staff       (20)     5699 2024-04-04 09:53:35.000000 healthsageai-0.1.4/README.md
+-rw-r--r--   0 a.groen    (501) staff       (20)     1505 2024-04-16 08:31:28.000000 healthsageai-0.1.4/pyproject.toml
+-rw-r--r--   0 a.groen    (501) staff       (20)       38 2024-04-16 08:31:47.253519 healthsageai-0.1.4/setup.cfg
+drwxr-xr-x   0 a.groen    (501) staff       (20)        0 2024-04-16 08:31:47.247290 healthsageai-0.1.4/src/
+-rw-r--r--   0 a.groen    (501) staff       (20)        0 2024-01-17 13:46:31.000000 healthsageai-0.1.4/src/__init__.py
+drwxr-xr-x   0 a.groen    (501) staff       (20)        0 2024-04-16 08:31:47.246518 healthsageai-0.1.4/src/healthsageai/
+drwxr-xr-x   0 a.groen    (501) staff       (20)        0 2024-04-16 08:31:47.248938 healthsageai-0.1.4/src/healthsageai/note_to_fhir/
+-rw-r--r--   0 a.groen    (501) staff       (20)        0 2024-02-14 08:50:05.000000 healthsageai-0.1.4/src/healthsageai/note_to_fhir/__init__.py
+-rw-r--r--   0 a.groen    (501) staff       (20)     2950 2024-04-04 09:53:35.000000 healthsageai-0.1.4/src/healthsageai/note_to_fhir/data_utils.py
+drwxr-xr-x   0 a.groen    (501) staff       (20)        0 2024-04-16 08:31:47.250753 healthsageai-0.1.4/src/healthsageai/note_to_fhir/evaluation/
+-rw-r--r--   0 a.groen    (501) staff       (20)        0 2024-02-14 08:50:05.000000 healthsageai-0.1.4/src/healthsageai/note_to_fhir/evaluation/__init__.py
+-rw-r--r--   0 a.groen    (501) staff       (20)     4644 2024-04-04 09:53:35.000000 healthsageai-0.1.4/src/healthsageai/note_to_fhir/evaluation/datamodels.py
+-rw-r--r--   0 a.groen    (501) staff       (20)     3592 2024-04-04 09:53:35.000000 healthsageai-0.1.4/src/healthsageai/note_to_fhir/evaluation/fhirmodels.py
+-rw-r--r--   0 a.groen    (501) staff       (20)    23029 2024-04-16 08:30:15.000000 healthsageai-0.1.4/src/healthsageai/note_to_fhir/evaluation/utils.py
+-rw-r--r--   0 a.groen    (501) staff       (20)     3660 2024-02-14 08:50:05.000000 healthsageai-0.1.4/src/healthsageai/note_to_fhir/evaluation/visuals.py
+drwxr-xr-x   0 a.groen    (501) staff       (20)        0 2024-04-16 08:31:47.251639 healthsageai-0.1.4/src/healthsageai/note_to_fhir/inference/
+-rw-r--r--   0 a.groen    (501) staff       (20)      104 2024-02-14 08:50:05.000000 healthsageai-0.1.4/src/healthsageai/note_to_fhir/inference/__init__.py
+-rw-r--r--   0 a.groen    (501) staff       (20)     3315 2024-02-14 08:50:05.000000 healthsageai-0.1.4/src/healthsageai/note_to_fhir/inference/note_to_fhir.py
+-rw-r--r--   0 a.groen    (501) staff       (20)     2039 2024-02-14 08:50:05.000000 healthsageai-0.1.4/src/healthsageai/note_to_fhir/parsers.py
+drwxr-xr-x   0 a.groen    (501) staff       (20)        0 2024-04-16 08:31:47.251956 healthsageai-0.1.4/src/healthsageai/note_to_fhir/templates/
+-rw-r--r--   0 a.groen    (501) staff       (20)     2480 2024-02-14 08:50:05.000000 healthsageai-0.1.4/src/healthsageai/note_to_fhir/templates/simple.py
+drwxr-xr-x   0 a.groen    (501) staff       (20)        0 2024-04-16 08:31:47.252304 healthsageai-0.1.4/src/healthsageai.egg-info/
+-rw-r--r--   0 a.groen    (501) staff       (20)    47022 2024-04-16 08:31:47.000000 healthsageai-0.1.4/src/healthsageai.egg-info/PKG-INFO
+-rw-r--r--   0 a.groen    (501) staff       (20)      797 2024-04-16 08:31:47.000000 healthsageai-0.1.4/src/healthsageai.egg-info/SOURCES.txt
+-rw-r--r--   0 a.groen    (501) staff       (20)        1 2024-04-16 08:31:47.000000 healthsageai-0.1.4/src/healthsageai.egg-info/dependency_links.txt
+-rw-r--r--   0 a.groen    (501) staff       (20)      157 2024-04-16 08:31:47.000000 healthsageai-0.1.4/src/healthsageai.egg-info/requires.txt
+-rw-r--r--   0 a.groen    (501) staff       (20)       35 2024-04-16 08:31:47.000000 healthsageai-0.1.4/src/healthsageai.egg-info/top_level.txt
```

### Comparing `healthsageai-0.1.3/LICENSE` & `healthsageai-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `healthsageai-0.1.3/PKG-INFO` & `healthsageai-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: healthsageai
-Version: 0.1.3
+Version: 0.1.4
 Summary: HealthSage AI LLMs, Healthcare genAI platform
 Author-email: HealthSage AI <hello@healthsage.ai>
 Maintainer-email: HealthSage AI <hello@healthsage.ai>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `healthsageai-0.1.3/README.md` & `healthsageai-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `healthsageai-0.1.3/pyproject.toml` & `healthsageai-0.1.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=40.6.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "healthsageai"
-version = "0.1.3"
+version = "0.1.4"
 description = "HealthSage AI LLMs, Healthcare genAI platform"
 readme = "README.md"
 
 requires-python = ">=3.9"
 
 license = {file = "LICENSE"}
```

### Comparing `healthsageai-0.1.3/src/healthsageai/note_to_fhir/data_utils.py` & `healthsageai-0.1.4/src/healthsageai/note_to_fhir/data_utils.py`

 * *Files identical despite different names*

### Comparing `healthsageai-0.1.3/src/healthsageai/note_to_fhir/evaluation/datamodels.py` & `healthsageai-0.1.4/src/healthsageai/note_to_fhir/evaluation/datamodels.py`

 * *Files identical despite different names*

### Comparing `healthsageai-0.1.3/src/healthsageai/note_to_fhir/evaluation/fhirmodels.py` & `healthsageai-0.1.4/src/healthsageai/note_to_fhir/evaluation/fhirmodels.py`

 * *Files identical despite different names*

### Comparing `healthsageai-0.1.3/src/healthsageai/note_to_fhir/evaluation/utils.py` & `healthsageai-0.1.4/src/healthsageai/note_to_fhir/evaluation/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,25 +10,30 @@
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Affero General Public License for more details.
 #
 #  You should have received a copy of the GNU Affero General Public License
 #  along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 import json
-from healthsageai.note_to_fhir.evaluation.datamodels import FhirScore, ElementDetails, FhirDiff
+from healthsageai.note_to_fhir.evaluation.datamodels import (
+    FhirScore,
+    ElementDetails,
+    FhirDiff,
+)
 from healthsageai.note_to_fhir.evaluation.fhirmodels import object_mapping
 from typing import List
 import warnings
 from collections import defaultdict
 from pydantic.v1.main import ModelMetaclass
 import pandas as pd
 import itertools
 import numpy as np
 
-MAX_PERMUTATIONS_ARRAY_SIZE = 5  # When all permutations have to be calculated
+
+MAX_PERMUTATIONS_ARRAY_SIZE = 7  # When all permutations have to be calculated
 
 
 def get_resource_details(Resource) -> List[ElementDetails]:
     """Get the details of a certain fhir resource that are relevant to evaluation in a friendly format.
 
     Args:
         Resource (fhir.resources): Resource Metadata
@@ -47,18 +52,18 @@
         if "type" not in spec.keys():
             continue
 
         required = (
             False if "element_required" not in spec.keys() else spec["element_required"]
         )
 
-        fhirtype = spec["type"]
+        fhirtype = spec.get("format", spec.get("type"))
         array_item_type = None
         if fhirtype == "array":
-            array_item_type = spec["items"]["type"]
+            array_item_type = spec["items"].get("format", spec["items"].get("type"))
 
         element_details = ElementDetails(
             key=name,
             fhirtype=fhirtype,
             required=required,
             is_leaf=fhirtype_is_leaf(fhirtype),
             is_struct=fhirtype_is_struct(fhirtype),
@@ -78,14 +83,18 @@
         list_2 (list): A list of items
 
     Returns:
         tuple: The respective lists but of equal length, imputed with None.
     """
     list_1 = list_1 if list_1 else []
     list_2 = list_2 if list_2 else []
+
+    list_1 = [i for i in list_1 if i is not None]  # Clear None
+    list_2 = [i for i in list_2 if i is not None]  # Clear None
+
     len_1 = len(list_1)
     len_2 = len(list_2)
     max_len = max(len_1, len_2)
     for i in range(max_len):
         if i >= len_1:
             list_1.append(None)
         elif i >= len_2:
@@ -143,15 +152,23 @@
 
     Args:
         fhirtype (str): fhirtype as specified by fhir.resources
 
     Returns:
         bool: True if fhirtype is leaf, False otherwise
     """
-    return fhirtype in ["boolean", "integer", "string", "decimal", "number"]
+    return fhirtype in [
+        "boolean",
+        "integer",
+        "string",
+        "decimal",
+        "number",
+        "date-time",
+        "date",
+    ]
 
 
 def map_align_arrays(arr1, arr2):
     """Maps two arrays to each other and aligns them in corresponding order.
 
     Args:
         arr1 (list): list of fhir elements
@@ -159,91 +176,177 @@
 
     Returns:
         arr1, arr2: Where arr1[i] corresponds to arr2[i]
     """
     warnings.warn("NotImplemented; arrays are assumed to be in identical order.")
     return match_list_len(arr1, arr2)
 
-def optimize_array_order(fhir_true_array: list, fhir_pred_array: list, element_details: ElementDetails) -> tuple:
+
+def optimize_array_order(
+    fhir_true_array: list, fhir_pred_array: list, element_details: ElementDetails
+) -> tuple:
     if len(fhir_true_array) <= MAX_PERMUTATIONS_ARRAY_SIZE:
-        return optimize_array_order_exact(fhir_true_array, fhir_pred_array, element_details)  # scales n!
+        return optimize_array_order_exact(
+            fhir_true_array, fhir_pred_array, element_details
+        )  # scales n!
     else:
-        return optimize_array_order_approx(fhir_true_array, fhir_pred_array, element_details)  # scales n**2
+        return optimize_array_order_approx(
+            fhir_true_array, fhir_pred_array, element_details
+        )  # scales n**2
 
-def optimize_array_order_exact(fhir_true_array: list, fhir_pred_array: list, element_details: ElementDetails) -> tuple:
-    """Finds the list order for fhir_pred the results in the highest accuracy by calculating all permutations
+
+def optimize_array_order_exact(
+    fhir_true_array: list, fhir_pred_array: list, element_details: ElementDetails
+) -> tuple:
+    """Finds the list order for fhir_pred the results in the highest accuracy by calculating all possible permutations.
 
     Args:
         fhir_true_array (list): list of Fhir resources
         fhir_pred_array (list): list of Fhir resources to optimize
         element_details (ElementDetails): metadata
     """
-    assert isinstance(fhir_true_array, list) and isinstance(fhir_pred_array, list), (fhir_true_array, fhir_pred_array)
-    fhir_pred_child_permutations = [list(permutation) for permutation in itertools.permutations(fhir_pred_array)]
+    assert isinstance(fhir_true_array, list) and isinstance(fhir_pred_array, list), (
+        fhir_true_array,
+        fhir_pred_array,
+    )
+    fhir_pred_child_permutations = [
+        list(permutation) for permutation in itertools.permutations(fhir_pred_array)
+    ]
     max_idx = -1
-    max_accuracy = 0.
+    max_accuracy = 0.0
     for i, permutation in enumerate(fhir_pred_child_permutations):
         score = _get_array_score(fhir_true_array, permutation, element_details)
         if score.accuracy > max_accuracy:
             max_idx = i
             max_accuracy = score.accuracy
     fhir_pred_child_max = fhir_pred_child_permutations[max_idx]
     return fhir_true_array, fhir_pred_child_max
 
-def optimize_array_order_approx(fhir_true_array: list, fhir_pred_array: list, element_details: ElementDetails) -> tuple:
-    """Finds the list order for fhir_pred the results in the highest accuracy using argmax with penalties
+
+def are_same_types(a, b) -> bool:
+    """Checks if two resource types are the same by checking the resourceType attribute or whether python types match.
+
+    Returns True if:
+    a and b are both dictionaries without resourceType attribute
+    a and b are both dictionaries with the same resourceType
+    a and b are both lists
+    a and b are both strings
+    a and b are both numeric (float or int)
 
     Args:
-        fhir_true_array (list): _description_
-        fhir_pred_array (list): _description_
-        element_details (ElementDetails): _description_
+        a (Any): Fhir value
+        b (Any): Fhir value
+
+    Returns:
+        bool: True if resource are considered of the same type
+    """
+    if isinstance(a, dict) and isinstance(b, dict):
+        type_a, type_b = a.get("resourceType", ""), b.get("resourceType", "")
+        # For Bundle-Entries, take the resourcetype of the entry.
+        if (
+            type_a == ""
+            and type_b == ""
+            and "entry" in a.keys()
+            and "entry" in b.keys()
+        ):
+            type_a, type_b = (
+                a["entry"].get("resourceType", ""),
+                b["entry"].get("resourceType", ""),
+            )
+        same_type = type_a == type_b
+        return same_type
+    elif isinstance(a, list) and isinstance(b, list):
+        return True
+    elif isinstance(a, str) and isinstance(b, str):
+        return True
+    elif (isinstance(a, float) or isinstance(a, int)) and (
+        isinstance(b, float) or isinstance(b, int)
+    ):
+        return True
+    else:
+        return False
+
+
+def optimize_array_order_approx(
+    fhir_true_array: list, fhir_pred_array: list, element_details: ElementDetails
+) -> tuple:
+    """Finds the list order for fhir_pred the results in the highest accuracy calculating the match score (accuracy) between each
+    list item.
+
+    Args:
+        fhir_true_array (list): The array/list in the ground truth FHIR resource
+        fhir_pred_array (list): The array/list to be re-ordered
+        element_details (ElementDetails): Metadata
 
     Returns:
-        tuple: _description_
+        tuple: fhir_true_array and fhir_pred_array_max, where fhir_pred_array_max is a re-ordered version of the fhir_pred_array
     """
-    accuracy_matrix = pd.DataFrame(0., index=np.arange(len(fhir_true_array)), columns=np.arange(len(fhir_pred_array)))
+    accuracy_matrix = pd.DataFrame(
+        0.0,
+        index=np.arange(len(fhir_true_array)),
+        columns=np.arange(len(fhir_pred_array)),
+    )
     for i_true, fhir_true in enumerate(fhir_true_array):
         for i_pred, fhir_pred in enumerate(fhir_pred_array):
-            diff = FhirDiff(
-            fhir_true=fhir_true,
-            fhir_pred=fhir_pred,
-            resource_name=element_details.array_item_type,
-            parent=None,
-            key=element_details.key,
-            )
-            diff = _expand_diff_tree(diff)
-            accuracy_matrix.iloc[i_true, i_pred] = diff.score.accuracy
+            if not are_same_types(fhir_true, fhir_pred):
+                accuracy_matrix.iloc[i_true, i_pred] = -1.0
+            else:
+                diff = FhirDiff(
+                    fhir_true=fhir_true,
+                    fhir_pred=fhir_pred,
+                    resource_name=element_details.array_item_type,
+                    parent=None,
+                    key=element_details.key,
+                )
+                diff = _expand_diff_tree(diff)
+                accuracy_matrix.iloc[i_true, i_pred] = diff.score.accuracy
 
     optimal_order = get_optimal_order(accuracy_matrix)
-    fhir_pred_array_max = []
-    for target_idx in optimal_order:
-        fhir_pred_array_max.append(fhir_pred_array[target_idx])
+
+    # Initialize
+    fhir_pred_array_max = [x for x in range(len(optimal_order))]
+
+    # Align each item with its best matching ground truth item
+    for pred_idx, true_idx in optimal_order.items():
+        fhir_pred_array_max[true_idx] = fhir_pred_array[pred_idx]
 
     return fhir_true_array, fhir_pred_array_max
 
 
-def get_optimal_order(accuracy_matrix):
+def get_optimal_order(accuracy_matrix) -> dict:
     """
 
     Args:
         matrix (_type_): _description_
     """
-    epsilon = 0.01
-    marginal_distribution_pred = accuracy_matrix.mean(axis=0) + epsilon
-    marginal_distribution_true = accuracy_matrix.mean(axis=1) + epsilon
-    joint_distribution = np.dot(np.expand_dims(marginal_distribution_true, axis=1), np.expand_dims(marginal_distribution_pred, axis=0))
+    optimal_order = {}  # pred idx : true idx
+    while accuracy_matrix.shape[0] > 0:
+        max_col, max_idx = _get_max_loc(accuracy_matrix)
+        optimal_order[max_col] = max_idx
+        del accuracy_matrix[max_col]
+        accuracy_matrix.drop(max_idx, inplace=True)
 
-    accuracy_ratio_matrix = accuracy_matrix / joint_distribution
+    return optimal_order
 
-    optimal_order = accuracy_ratio_matrix.idxmax(axis=1)
 
-    return optimal_order
+def _get_max_loc(df: pd.DataFrame) -> tuple:
+    """Returns the column and index of the highest value in a DataFrame
 
+    Args:
+        df (pd.DataFrame): Numeric dataframe
+
+    Returns:
+        tuple: column, index
+    """
+    return df.unstack().idxmax()
 
-def _get_array_score(fhir_true_array: list, fhir_pred_array: list, element_details: ElementDetails) -> FhirScore:
+
+def _get_array_score(
+    fhir_true_array: list, fhir_pred_array: list, element_details: ElementDetails
+) -> FhirScore:
     """Calculate FhirScore of fhir_pred_array in that particular order
 
     Args:
         fhir_true_array (list): list of Fhir resources
         fhir_pred_array (list): list of Fhir resources to optimize
         element_details (ElementDetails): metadata
 
@@ -265,15 +368,14 @@
         )
         childdiff_item = _expand_diff_tree(childdiff_item)
         childscore = childscore + childdiff_item.score
         i += 1
     return childscore
 
 
-
 def convert_to_defaultdict(obj) -> any:
     """Convert dict to default dict, if it's a dict
 
     Args:
         obj (any): _description_
 
     Returns:
@@ -347,30 +449,29 @@
     else:
         resource_type = get_resource_type(diff.fhir_pred, diff.resource_name)
 
     if fhirtype_is_leaf(resource_type):
         diff.score = compare_leaf(diff)
         return diff
 
-    Resource = get_resource_class(
-        resource_type
-    )
+    Resource = get_resource_class(resource_type)
     resource_details = get_resource_details(Resource)  # list of ElementDetails
 
-
+    if not (isinstance(diff.fhir_pred, dict) or diff.fhir_pred is None):
+        diff.fhir_pred = {"illegal fhirtype": diff.fhir_pred}
 
     for element_details in resource_details:
         # Skip if the element is absent in both fhir_true and fhir_pred.
         if (
             element_details.key not in diff.fhir_pred.keys()
             and element_details.key not in diff.fhir_true.keys()
         ):
             continue
-        if (
-            element_is_absent(diff.fhir_true[element_details.key]) and element_is_absent(diff.fhir_pred[element_details.key])
+        if element_is_absent(diff.fhir_true[element_details.key]) and element_is_absent(
+            diff.fhir_pred[element_details.key]
         ):
             continue
 
         # If the element is a struct (dictionary) with arbitrary depth, handle recursively
         if element_details.is_struct:
             _expand_diff_tree_struct(diff, element_details)
             childscore = diff.children[element_details.key].score
@@ -385,15 +486,17 @@
         # If the element is a leaf, calculate the score directly
         elif element_details.is_leaf:
             _expand_diff_tree_leaf(diff, element_details)
             childscore = diff.children[element_details.key].score
 
         else:
             childscore = FhirScore()
-            warnings.warn(f"Details of element {element_details} could not be determined. \n fhir true: {diff.fhir_true} \n fhir pred: {diff.fhir_pred}")
+            warnings.warn(
+                f"Details of element {element_details} could not be determined. \n fhir true: {diff.fhir_true} \n fhir pred: {diff.fhir_pred}"
+            )
 
         # Add the child node score to the current score
         diff.score = diff.score + childscore
 
     # diff.score.is_valid = validate_resource(diff.fhir_pred, diff.resource_type)
 
     return diff
@@ -422,15 +525,15 @@
     """Expand FhirDiff with struct/dict-like node
 
     Args:
         diff (FhirDiff): _description_
         element_details (ElementDetails): _description_
     """
     if not isinstance(diff.fhir_pred[element_details.key], dict):
-        diff.fhir_pred[element_details.key]= {}
+        diff.fhir_pred[element_details.key] = {}
     childdiff = FhirDiff(
         fhir_true=diff.fhir_true[element_details.key],
         fhir_pred=diff.fhir_pred[element_details.key],
         resource_name=element_details.fhirtype,
         parent=diff,
         key=element_details.key,
     )
@@ -441,21 +544,26 @@
 def _expand_diff_tree_array(diff: FhirDiff, element_details: ElementDetails):
     """Expand FhirDiff with array node
 
     Args:
         diff (FhirDiff): _description_
         element_details (ElementDetails): _description_
     """
-    if not isinstance(diff.fhir_pred[element_details.key], list):
+    if not isinstance(diff.fhir_pred.get(element_details.key, None), list):
         diff.fhir_pred[element_details.key] = []
     diff.children[element_details.key] = []
-    fhir_true_child, fhir_pred_child = diff.fhir_true[element_details.key], diff.fhir_pred[element_details.key]
+    fhir_true_child, fhir_pred_child = (
+        diff.fhir_true[element_details.key],
+        diff.fhir_pred[element_details.key],
+    )
     fhir_true_child, fhir_pred_child = match_list_len(fhir_true_child, fhir_pred_child)
     if len(fhir_true_child) > 1 or len(fhir_pred_child) > 1:
-        fhir_true_child, fhir_pred_child = optimize_array_order(fhir_true_child, fhir_pred_child, element_details)
+        fhir_true_child, fhir_pred_child = optimize_array_order(
+            fhir_true_child, fhir_pred_child, element_details
+        )
 
     i = 0
     childscore = FhirScore()
     for fhir_true_child_item, fhir_pred_child_item in zip(
         fhir_true_child, fhir_pred_child
     ):
         childdiff_item = FhirDiff(
@@ -467,28 +575,30 @@
             key=element_details.key,
         )
         childdiff_item = _expand_diff_tree(childdiff_item)
         diff.children[element_details.key].append(childdiff_item)
         childscore = childscore + childdiff_item.score
         i += 1
 
+
 def remove_id_from_reference(reference: str):
-    """Remove id from reference for evaluation. 
-    
+    """Remove id from reference for evaluation.
+
     Args:
         reference (str): Reference to another FHIR resource, e.g. "Patient/1", "Encounter/2" etc.
 
     Returns:
         str: Reference without the id, e.g. "Patient", "Encounter"
     """
     if "/" in reference:
         return reference.split("/")[0]
     else:
         return reference
-    
+
+
 def element_is_absent(leaf: any) -> bool:
     """Check if an element is semantically null/None, taking into account different types.
 
     Args:
         leaf (any): The value of a Fhir Element
 
     Returns:
@@ -516,15 +626,27 @@
     Returns:
         FhirScore: object containing score for the leaf node.
     """
     element_true, element_pred = diff.fhir_true, diff.fhir_pred
     if diff.key == "id":
         return FhirScore()
     if diff.key == "reference":
-        element_true, element_pred = remove_id_from_reference(element_true), remove_id_from_reference(element_pred)
+        element_true, element_pred = (
+            remove_id_from_reference(element_true),
+            remove_id_from_reference(element_pred),
+        )
+    if (
+        diff.resource_type == "date-time"
+        and isinstance(element_true, str)
+        and isinstance(element_pred, str)
+    ):
+        element_true, element_pred = (
+            element_true[:16],
+            element_pred[:16],
+        )  # Datetimes are evaluated on minute level
     if element_is_absent(element_pred) and element_is_absent(element_true):
         fhirscore = FhirScore()
     elif element_is_absent(element_pred):
         fhirscore = FhirScore(n_deletions=1, n_leaves=1)  # miss
     elif element_is_absent(element_true):
         fhirscore = FhirScore(n_additions=1, n_leaves=1)  # hallucination
     elif element_true != element_pred:
@@ -552,23 +674,19 @@
 
     if not diff.children:
         return diffs
 
     for child_comparison in diff.children.values():
         if isinstance(child_comparison, list):
             for child_comparison_item in child_comparison:
-                new_diffs = diff_to_list(
-                    child_comparison_item
-                )
+                new_diffs = diff_to_list(child_comparison_item)
                 diffs = diffs + new_diffs
 
         else:
-            new_diffs = diff_to_list(
-                child_comparison
-            )
+            new_diffs = diff_to_list(child_comparison)
             diffs = diffs + new_diffs
     return diffs
 
 
 def diff_to_dataframe(diff: FhirDiff) -> pd.DataFrame:
     """Flattens a Diff Tree object to a pandas dataframe
 
@@ -582,10 +700,25 @@
     diff_dicts = []
     scores = [diff.score for diff in diffs]
     for diff in diffs:
         diff_dict_out = diff.model_dump()
         score = diff.score.model_dump()
         diff_dict_out.update(score)
         diff_dicts.append(diff_dict_out)
-    df = pd.DataFrame(diff_dicts)[['resource_type', 'entry_nr', 'key', 'label', 'n_leaves', 'n_matches','n_additions','n_deletions','n_modifications','accuracy','precision','recall']]
-    df['score'] = scores
+    df = pd.DataFrame(diff_dicts)[
+        [
+            "resource_type",
+            "entry_nr",
+            "key",
+            "label",
+            "n_leaves",
+            "n_matches",
+            "n_additions",
+            "n_deletions",
+            "n_modifications",
+            "accuracy",
+            "precision",
+            "recall",
+        ]
+    ]
+    df["score"] = scores
     return df
```

### Comparing `healthsageai-0.1.3/src/healthsageai/note_to_fhir/evaluation/visuals.py` & `healthsageai-0.1.4/src/healthsageai/note_to_fhir/evaluation/visuals.py`

 * *Files identical despite different names*

### Comparing `healthsageai-0.1.3/src/healthsageai/note_to_fhir/inference/note_to_fhir.py` & `healthsageai-0.1.4/src/healthsageai/note_to_fhir/inference/note_to_fhir.py`

 * *Files identical despite different names*

### Comparing `healthsageai-0.1.3/src/healthsageai/note_to_fhir/parsers.py` & `healthsageai-0.1.4/src/healthsageai/note_to_fhir/parsers.py`

 * *Files identical despite different names*

### Comparing `healthsageai-0.1.3/src/healthsageai/note_to_fhir/templates/simple.py` & `healthsageai-0.1.4/src/healthsageai/note_to_fhir/templates/simple.py`

 * *Files identical despite different names*

### Comparing `healthsageai-0.1.3/src/healthsageai.egg-info/PKG-INFO` & `healthsageai-0.1.4/src/healthsageai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: healthsageai
-Version: 0.1.3
+Version: 0.1.4
 Summary: HealthSage AI LLMs, Healthcare genAI platform
 Author-email: HealthSage AI <hello@healthsage.ai>
 Maintainer-email: HealthSage AI <hello@healthsage.ai>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `healthsageai-0.1.3/src/healthsageai.egg-info/SOURCES.txt` & `healthsageai-0.1.4/src/healthsageai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

