# Comparing `tmp/chemparse-0.1.3.tar.gz` & `tmp/chemparse-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chemparse-0.1.3.tar", last modified: Wed Nov 29 22:35:32 2023, max compression
+gzip compressed data, was "chemparse-0.2.0.tar", last modified: Tue Apr 16 21:43:21 2024, max compression
```

## Comparing `chemparse-0.1.3.tar` & `chemparse-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,22 @@
-drwxr-xr-x   0 jupyter-gmboyer-singleuser (64940) jupyter-gmboyer-singleuser (64940)        0 2023-11-29 22:35:32.034015 chemparse-0.1.3/
--rw-r--r--   0 jupyter-gmboyer-singleuser (64940) jupyter-gmboyer-singleuser (64940)     1056 2023-11-29 22:30:38.000000 chemparse-0.1.3/LICENSE.txt
--rw-r--r--   0 jupyter-gmboyer-singleuser (64940) jupyter-gmboyer-singleuser (64940)     1225 2023-11-29 22:35:32.030015 chemparse-0.1.3/PKG-INFO
--rw-r--r--   0 jupyter-gmboyer-singleuser (64940) jupyter-gmboyer-singleuser (64940)      850 2023-11-29 22:29:43.000000 chemparse-0.1.3/README.md
-drwxr-xr-x   0 jupyter-gmboyer-singleuser (64940) jupyter-gmboyer-singleuser (64940)        0 2023-11-29 22:35:32.014013 chemparse-0.1.3/chemparse/
--rw-r--r--   0 jupyter-gmboyer-singleuser (64940) jupyter-gmboyer-singleuser (64940)       30 2023-11-29 22:29:43.000000 chemparse-0.1.3/chemparse/__init__.py
--rw-r--r--   0 jupyter-gmboyer-singleuser (64940) jupyter-gmboyer-singleuser (64940)     4459 2023-11-29 22:30:14.000000 chemparse-0.1.3/chemparse/fun.py
-drwxr-xr-x   0 jupyter-gmboyer-singleuser (64940) jupyter-gmboyer-singleuser (64940)        0 2023-11-29 22:35:32.030015 chemparse-0.1.3/chemparse.egg-info/
--rw-r--r--   0 jupyter-gmboyer-singleuser (64940) jupyter-gmboyer-singleuser (64940)     1225 2023-11-29 22:35:31.000000 chemparse-0.1.3/chemparse.egg-info/PKG-INFO
--rw-r--r--   0 jupyter-gmboyer-singleuser (64940) jupyter-gmboyer-singleuser (64940)      233 2023-11-29 22:35:31.000000 chemparse-0.1.3/chemparse.egg-info/SOURCES.txt
--rw-r--r--   0 jupyter-gmboyer-singleuser (64940) jupyter-gmboyer-singleuser (64940)        1 2023-11-29 22:35:31.000000 chemparse-0.1.3/chemparse.egg-info/dependency_links.txt
--rw-r--r--   0 jupyter-gmboyer-singleuser (64940) jupyter-gmboyer-singleuser (64940)        1 2023-11-29 22:35:31.000000 chemparse-0.1.3/chemparse.egg-info/not-zip-safe
--rw-r--r--   0 jupyter-gmboyer-singleuser (64940) jupyter-gmboyer-singleuser (64940)       10 2023-11-29 22:35:31.000000 chemparse-0.1.3/chemparse.egg-info/top_level.txt
--rw-r--r--   0 jupyter-gmboyer-singleuser (64940) jupyter-gmboyer-singleuser (64940)       38 2023-11-29 22:35:32.034015 chemparse-0.1.3/setup.cfg
--rw-r--r--   0 jupyter-gmboyer-singleuser (64940) jupyter-gmboyer-singleuser (64940)      668 2023-11-29 22:30:46.000000 chemparse-0.1.3/setup.py
+drwxr-xr-x   0 jupyter-gmboyer-singleuser (64940) jupyter-gmboyer-singleuser (64940)        0 2024-04-16 21:43:21.400973 chemparse-0.2.0/
+-rw-r--r--   0 jupyter-gmboyer-singleuser (64940) jupyter-gmboyer-singleuser (64940)     1077 2024-04-15 22:12:43.000000 chemparse-0.2.0/LICENSE.txt
+-rw-r--r--   0 jupyter-gmboyer-singleuser (64940) jupyter-gmboyer-singleuser (64940)     1534 2024-04-16 21:43:21.400973 chemparse-0.2.0/PKG-INFO
+-rw-r--r--   0 jupyter-gmboyer-singleuser (64940) jupyter-gmboyer-singleuser (64940)     1171 2024-04-15 22:18:03.000000 chemparse-0.2.0/README.md
+drwxr-xr-x   0 jupyter-gmboyer-singleuser (64940) jupyter-gmboyer-singleuser (64940)        0 2024-04-16 21:43:21.400973 chemparse-0.2.0/chemparse/
+-rw-r--r--   0 jupyter-gmboyer-singleuser (64940) jupyter-gmboyer-singleuser (64940)       30 2024-04-12 21:02:23.000000 chemparse-0.2.0/chemparse/__init__.py
+-rw-r--r--   0 jupyter-gmboyer-singleuser (64940) jupyter-gmboyer-singleuser (64940)       48 2024-04-12 21:02:23.000000 chemparse-0.2.0/chemparse/__init__.pyi
+-rw-r--r--   0 jupyter-gmboyer-singleuser (64940) jupyter-gmboyer-singleuser (64940)      679 2024-04-12 21:02:23.000000 chemparse-0.2.0/chemparse/exceptions.py
+-rw-r--r--   0 jupyter-gmboyer-singleuser (64940) jupyter-gmboyer-singleuser (64940)      387 2024-04-12 21:02:23.000000 chemparse-0.2.0/chemparse/exceptions.pyi
+-rw-r--r--   0 jupyter-gmboyer-singleuser (64940) jupyter-gmboyer-singleuser (64940)     5897 2024-04-12 21:02:23.000000 chemparse-0.2.0/chemparse/fun.py
+-rw-r--r--   0 jupyter-gmboyer-singleuser (64940) jupyter-gmboyer-singleuser (64940)      584 2024-04-12 21:02:23.000000 chemparse-0.2.0/chemparse/fun.pyi
+drwxr-xr-x   0 jupyter-gmboyer-singleuser (64940) jupyter-gmboyer-singleuser (64940)        0 2024-04-16 21:43:21.400973 chemparse-0.2.0/chemparse.egg-info/
+-rw-r--r--   0 jupyter-gmboyer-singleuser (64940) jupyter-gmboyer-singleuser (64940)     1534 2024-04-16 21:43:21.000000 chemparse-0.2.0/chemparse.egg-info/PKG-INFO
+-rw-r--r--   0 jupyter-gmboyer-singleuser (64940) jupyter-gmboyer-singleuser (64940)      369 2024-04-16 21:43:21.000000 chemparse-0.2.0/chemparse.egg-info/SOURCES.txt
+-rw-r--r--   0 jupyter-gmboyer-singleuser (64940) jupyter-gmboyer-singleuser (64940)        1 2024-04-16 21:43:21.000000 chemparse-0.2.0/chemparse.egg-info/dependency_links.txt
+-rw-r--r--   0 jupyter-gmboyer-singleuser (64940) jupyter-gmboyer-singleuser (64940)        1 2024-04-16 21:43:21.000000 chemparse-0.2.0/chemparse.egg-info/not-zip-safe
+-rw-r--r--   0 jupyter-gmboyer-singleuser (64940) jupyter-gmboyer-singleuser (64940)       10 2024-04-16 21:43:21.000000 chemparse-0.2.0/chemparse.egg-info/top_level.txt
+-rw-r--r--   0 jupyter-gmboyer-singleuser (64940) jupyter-gmboyer-singleuser (64940)       38 2024-04-16 21:43:21.400973 chemparse-0.2.0/setup.cfg
+-rw-r--r--   0 jupyter-gmboyer-singleuser (64940) jupyter-gmboyer-singleuser (64940)      705 2024-04-15 22:10:03.000000 chemparse-0.2.0/setup.py
+drwxr-xr-x   0 jupyter-gmboyer-singleuser (64940) jupyter-gmboyer-singleuser (64940)        0 2024-04-16 21:43:21.400973 chemparse-0.2.0/test/
+-rw-r--r--   0 jupyter-gmboyer-singleuser (64940) jupyter-gmboyer-singleuser (64940)     1189 2024-04-12 21:02:23.000000 chemparse-0.2.0/test/test_chemparse.py
+-rw-r--r--   0 jupyter-gmboyer-singleuser (64940) jupyter-gmboyer-singleuser (64940)     1063 2024-04-12 21:02:23.000000 chemparse-0.2.0/test/test_exeptions.py
```

### Comparing `chemparse-0.1.3/LICENSE.txt` & `chemparse-0.2.0/LICENSE.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2023 Grayson Boyer
+Copyright (c) 2024 Grayson Boyer and Victor Ignatenko
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `chemparse-0.1.3/PKG-INFO` & `chemparse-0.2.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 Metadata-Version: 2.1
 Name: chemparse
-Version: 0.1.3
+Version: 0.2.0
 Summary: Chemical formula parser
-Author: Grayson Boyer
-Author-email: gmboyer@asu.edu
+Author: Grayson Boyer, Victor Ignatenko
+Author-email: gmboyer@asu.edu, vityaig@yandex.ru
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # chemparse
 
+**Authors:** Grayson Boyer and Victor Ignatenko
+
 A lightweight package for parsing chemical formula strings into python dictionaries. 
 
 ## Features
 
 * Convert a chemical formula string into a python dictionary.
     - example: `"CH4"` returns `{"C":1.0, "H":4.0}`
 * Handles fractional stoichiometry.
     - example: `"C1.5O3"` returns `{"C":1.5, "O":3.0}`
     - example: `"H2e-1O1e-1"` returns `{"H":0.2, "O":0.1}`
 * Handles groups with parentheses.
     - example: `"(CH3)2(CH2)4"` returns `{"C":6.0, "H":14.0}`
-    - Note: chemparse currently only handles non-nested paretheses. A formula with nested parentheses like `"CH3(C2(CH3)2)3CH3"` will not work properly.
+* **New in 2024** Chemparse now handles nested paretheses!
+    - example: `"((CH3)2)3"` returns `{'C': 6, 'H': 18}`
 
 ## Installation
 
 Install `chemparse` with pip:
 
 ```
 $ pip install chemparse
@@ -39,7 +42,22 @@
 Import chemparse in python and use the parse_formula function:
 
 ```
 import chemparse
 
 print(chemparse.parse_formula("C6H12O6"))
 ```
+
+## Contribute
+
+Install python
+
+Clone `chemparse` using git: \
+`git clone https://github.com/gmboyer/chemparse.git`
+
+Go to the `chemparse` directory: \
+`cd chemparse`
+
+Install requirements: \
+`pip install -r requirements.txt`
+
+Now you are ready to contribute!
```

### Comparing `chemparse-0.1.3/chemparse/fun.py` & `chemparse-0.2.0/chemparse/fun.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,110 +1,151 @@
 import re
+from typing import Generator
+from typing import Any
+# from .exceptions import NestedParenthesesError, ParenthesesMismatchError, ClosedParenthesesBeforeOpenError
+from .exceptions import ParenthesesMismatchError, ClosedParenthesesBeforeOpenError
+
+RE_SIGNED_NUMBER:str = r"(^(?=.)([+-]?([0-9]*)(\.([0-9]+))?)([eE][+-]?\d+)?)"
+RE_NUMBER:str        =      r"(^(?=.)(([0-9]*)(\.([0-9]+))?)([eE][+-]?\d+)?)"
+RE_LETTERS:str = r"^[a-zA-Z-+]+"
 
 # function to return index of all instances of a substring in a string
-def find_all(sub, a_str):
-    start = 0
+def find_all(sub:str, a_str:str) -> Generator[int , Any , None]:
+    start:int = 0
     while True:
         start = a_str.find(sub, start)
         if start == -1: return
         yield start
         start += len(sub) # use start += 1 to find overlapping matches
 
 # functions to parse elemental formulas (handles both floats and ints)
-def get_first_elem(formula):
-    needed_split = False
+def get_first_elem(formula:str) -> tuple[str, bool]:
+    needed_split:bool = False
     for char in formula:
         if formula.find(char) != 0 and (char.isupper() or char == "+" or char == "-"):
             formula = formula.split(char)[0]
             needed_split = True
             return formula, needed_split
         
         char_ind = list(find_all(char, formula))
         if len(char_ind) > 1 and (char.isupper() or char == "+" or char == "-") and (formula[1] == char or formula[1].islower()) and sum(1 for c in formula[0:char_ind[1]] if c.isupper())==1:
             formula = formula[0:char_ind[1]]
             needed_split = True
             return formula, needed_split
 
     return formula, needed_split
 
-def inner_parse_formula(text):
-    formula_dict = {}
-    for i in range(0, len(text)):
-        element = re.findall("^[a-zA-Z-+]+", text)
-        if element == []:
+def inner_parse_formula(text:str) -> dict[str, float]:
+    formula_dict:dict[str,float] = {}
+    for _ in range(0, len(text)):
+        element = re.findall(RE_LETTERS, text)
+        if len(element) == 0:
             break
         else:
             element, needed_split = get_first_elem(element[0])
             text = text.replace(element, '', 1)
             if needed_split:
                 number = 1.0
             else:
                 try:
-                    number = float(re.findall(r"(^(?=.)([+-]?([0-9]*)(\.([0-9]+))?)([eE][+-]?\d+)?)", text)[0][0])
+                    number = float(re.findall(RE_SIGNED_NUMBER, text)[0][0])
                 except:
                     number = 1.0
-                text = re.sub(r"(^(?=.)([+-]?([0-9]*)(\.([0-9]+))?)([eE][+-]?\d+)?)", "", text)
+                text = re.sub(RE_SIGNED_NUMBER, "", text)
             if element not in list(formula_dict.keys()):
                 formula_dict[element] = number
             else:
                 formula_dict[element] += number
     return formula_dict
 
-def find_occurrences(s, ch):
+def find_occurrences(s:str, ch:str) -> list[int]:
     return [i for i, letter in enumerate(s) if letter == ch]
+def get_first_parenth_match(text:str) -> int:
+    position:int = -1
+    ch_number:int = 0
+    closed_parenth_count: int = 0
+    opened_parenth_count: int = 0
+    for ch in text:
+        if ch == '(':
+            opened_parenth_count += 1
+        elif ch == ')':
+            closed_parenth_count += 1
+            if opened_parenth_count == closed_parenth_count:
+                position = closed_parenth_count - 1
+                break
+        ch_number += 1
 
+    return position
 
-def parse_formula(text):
+def parse_formula(text:str) -> dict[str, float]:
     
     text = str(text)
     
     # get indices of starting parentheses "(" and ending ")"
     open_parenth_idx_list = find_occurrences(text, "(")
     closed_parenth_idx_list = find_occurrences(text, ")")
     
     if len(open_parenth_idx_list) != len(closed_parenth_idx_list):
-        raise Exception("Open and closed parentheses mismatch in formula '"+text+"'")
+        raise ParenthesesMismatchError(text)
     
     for i in range(0, len(open_parenth_idx_list)-1):
-        if open_parenth_idx_list[i+1] < closed_parenth_idx_list[i]:
-            msg = ("Cannot parse nested parentheses in formula '"+text+"'")
-            raise Exception(msg)
+        # if open_parenth_idx_list[i+1] < closed_parenth_idx_list[i]:
+        #     raise NestedParenthesesError(text)
         if closed_parenth_idx_list[i] < open_parenth_idx_list[i]:
-            raise Exception("Closed parentheses detected before open parentheses in formula '"+text+"'")
+            raise ClosedParenthesesBeforeOpenError(text)
         if i == len(open_parenth_idx_list)-1:
             if closed_parenth_idx_list[i+1] < open_parenth_idx_list[i+1]:
-                raise Exception("Closed parentheses detected before open parentheses in formula '"+text+"'")
+                raise ClosedParenthesesBeforeOpenError(text)
     
-    seg_dict_list = []
-    for seg_i in range(0, len(open_parenth_idx_list)):
+    seg_dict_list:list[dict[str,float]] = []
+    parenth_pairs_count = len(open_parenth_idx_list)
+    for _ in range(parenth_pairs_count):
         text = str(text)
+        if len(text) <= 0:
+            break
+        if not '(' in text and not ')' in text:
+            break
         
         # get indices of starting parentheses "(" and ending ")"
         open_parenth_idx_list = find_occurrences(text, "(")
         closed_parenth_idx_list = find_occurrences(text, ")")
 
-        seg = text[open_parenth_idx_list[0]:closed_parenth_idx_list[0]+1]
+        first_parenth_match:int = get_first_parenth_match(text)
+        if first_parenth_match < 0:
+            raise ParenthesesMismatchError(text)
+        seg = text[open_parenth_idx_list[0]:closed_parenth_idx_list[first_parenth_match]+1]
         
         try:
-            number = float(re.findall(r"(^(?=.)([+-]?([0-9]*)(\.([0-9]+))?)([eE][+-]?\d+)?)", text[closed_parenth_idx_list[0]+1:])[0][0])
+            number = float(re.findall(RE_SIGNED_NUMBER, text[closed_parenth_idx_list[first_parenth_match]+1:])[0][0])
         except:
             number = 1
         
         seg_no_parenth = seg[1:-1]
-        seg_formula_dict = inner_parse_formula(seg_no_parenth)
+        # nested_parenth:bool = False
+        if '(' in seg_no_parenth or ')' in seg_no_parenth:
+            seg_formula_dict = parse_formula(seg_no_parenth)
+            # nested_parenth = True
+
+        else:
+            seg_formula_dict = inner_parse_formula(seg_no_parenth)
         seg_formula_dict_mult = {k:v*number for (k,v) in seg_formula_dict.items()}
 
-        endseg = re.sub(r"(^(?=.)(([0-9]*)(\.([0-9]+))?)([eE][+-]?\d+)?)", "", text[closed_parenth_idx_list[0]+1:])
+        endseg = re.sub(RE_NUMBER, "", text[closed_parenth_idx_list[first_parenth_match]+1:])
+        # if not nested_parenth:
         text = text[:open_parenth_idx_list[0]]+endseg
         seg_dict_list.append(seg_formula_dict_mult)
 
-    seg_dict_list.append(inner_parse_formula(text))
+    if '(' in text in text:
+        seg_dict_list.append(parse_formula(text))
+    else:
+        seg_dict_list.append(inner_parse_formula(text))
 
     # merge and sum all segments
     if len(seg_dict_list) > 1:
         start_dict = seg_dict_list[0]
         for i in range(1, len(seg_dict_list)):
             next_dict = seg_dict_list[i]
             start_dict = { k: start_dict.get(k, 0) + next_dict.get(k, 0) for k in set(start_dict) | set(next_dict) }
         return start_dict
     else:
-        return seg_dict_list[0]
+        return seg_dict_list[0]
+
```

### Comparing `chemparse-0.1.3/chemparse.egg-info/PKG-INFO` & `chemparse-0.2.0/chemparse.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 Metadata-Version: 2.1
 Name: chemparse
-Version: 0.1.3
+Version: 0.2.0
 Summary: Chemical formula parser
-Author: Grayson Boyer
-Author-email: gmboyer@asu.edu
+Author: Grayson Boyer, Victor Ignatenko
+Author-email: gmboyer@asu.edu, vityaig@yandex.ru
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # chemparse
 
+**Authors:** Grayson Boyer and Victor Ignatenko
+
 A lightweight package for parsing chemical formula strings into python dictionaries. 
 
 ## Features
 
 * Convert a chemical formula string into a python dictionary.
     - example: `"CH4"` returns `{"C":1.0, "H":4.0}`
 * Handles fractional stoichiometry.
     - example: `"C1.5O3"` returns `{"C":1.5, "O":3.0}`
     - example: `"H2e-1O1e-1"` returns `{"H":0.2, "O":0.1}`
 * Handles groups with parentheses.
     - example: `"(CH3)2(CH2)4"` returns `{"C":6.0, "H":14.0}`
-    - Note: chemparse currently only handles non-nested paretheses. A formula with nested parentheses like `"CH3(C2(CH3)2)3CH3"` will not work properly.
+* **New in 2024** Chemparse now handles nested paretheses!
+    - example: `"((CH3)2)3"` returns `{'C': 6, 'H': 18}`
 
 ## Installation
 
 Install `chemparse` with pip:
 
 ```
 $ pip install chemparse
@@ -39,7 +42,22 @@
 Import chemparse in python and use the parse_formula function:
 
 ```
 import chemparse
 
 print(chemparse.parse_formula("C6H12O6"))
 ```
+
+## Contribute
+
+Install python
+
+Clone `chemparse` using git: \
+`git clone https://github.com/gmboyer/chemparse.git`
+
+Go to the `chemparse` directory: \
+`cd chemparse`
+
+Install requirements: \
+`pip install -r requirements.txt`
+
+Now you are ready to contribute!
```

### Comparing `chemparse-0.1.3/setup.py` & `chemparse-0.2.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="chemparse",
-    version="0.1.3",
-    author="Grayson Boyer",
-    author_email="gmboyer@asu.edu",
+    version="0.2.0",
+    author="Grayson Boyer, Victor Ignatenko",
+    author_email="gmboyer@asu.edu, vityaig@yandex.ru",
     description="Chemical formula parser",
     long_description=long_description,
     long_description_content_type="text/markdown",
     entry_points={},
     packages=['chemparse'],
     classifiers=[
         "Programming Language :: Python :: 3",
```

