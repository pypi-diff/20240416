# Comparing `tmp/hllama-0.0.4-py3-none-any.whl.zip` & `tmp/hllama-0.0.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 6812 bytes, number of entries: 7
--rw-rw-r--  2.0 unx       48 b- defN 24-Apr-16 03:55 hllama/__init__.py
--rw-rw-r--  2.0 unx     2304 b- defN 24-Apr-16 02:11 hllama/json_utils.py
--rw-rw-r--  2.0 unx    11357 b- defN 24-Apr-16 03:56 hllama-0.0.4.dist-info/LICENSE
--rw-rw-r--  2.0 unx     1402 b- defN 24-Apr-16 03:56 hllama-0.0.4.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-Apr-16 03:56 hllama-0.0.4.dist-info/WHEEL
--rw-rw-r--  2.0 unx        7 b- defN 24-Apr-16 03:56 hllama-0.0.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      531 b- defN 24-Apr-16 03:56 hllama-0.0.4.dist-info/RECORD
-7 files, 15741 bytes uncompressed, 5874 bytes compressed:  62.7%
+Zip file size: 7008 bytes, number of entries: 7
+-rw-rw-r--  2.0 unx       22 b- defN 24-Apr-16 04:23 hllama/__init__.py
+-rw-rw-r--  2.0 unx     3301 b- defN 24-Apr-16 04:22 hllama/json_utils.py
+-rw-rw-r--  2.0 unx    11357 b- defN 24-Apr-16 04:23 hllama-0.0.6.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     1402 b- defN 24-Apr-16 04:23 hllama-0.0.6.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-Apr-16 04:23 hllama-0.0.6.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        7 b- defN 24-Apr-16 04:23 hllama-0.0.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      531 b- defN 24-Apr-16 04:23 hllama-0.0.6.dist-info/RECORD
+7 files, 16712 bytes uncompressed, 6070 bytes compressed:  63.7%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: hllama/__init__.py
 Comment: 
 
 Filename: hllama/json_utils.py
 Comment: 
 
-Filename: hllama-0.0.4.dist-info/LICENSE
+Filename: hllama-0.0.6.dist-info/LICENSE
 Comment: 
 
-Filename: hllama-0.0.4.dist-info/METADATA
+Filename: hllama-0.0.6.dist-info/METADATA
 Comment: 
 
-Filename: hllama-0.0.4.dist-info/WHEEL
+Filename: hllama-0.0.6.dist-info/WHEEL
 Comment: 
 
-Filename: hllama-0.0.4.dist-info/top_level.txt
+Filename: hllama-0.0.6.dist-info/top_level.txt
 Comment: 
 
-Filename: hllama-0.0.4.dist-info/RECORD
+Filename: hllama-0.0.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## hllama/__init__.py

```diff
@@ -1,3 +1 @@
-__version__ = "0.0.4"
-
-__all__ = ["json_utils"]
+__version__ = "0.0.6"
```

## hllama/json_utils.py

```diff
@@ -4,28 +4,47 @@
 
 def match_structure(schema: Dict[str, Any], data: Dict[str, Any]) -> bool:
     for key, expected_type in schema.items():
         if key not in data:
             print(f"Missing key: {key}")
             return False
 
-        if isinstance(expected_type, dict):
+        # Check if the expected_type is explicitly a list of dictionaries
+        if isinstance(expected_type, list):
+            # Ensure the data is a list
+            if not isinstance(data[key], list):
+                print(f"Expected a list for key: {key}, got {type(data[key])}")
+                return False
+            # Check each item in the list if it conforms to the expected dictionary schema
+            for item in data[key]:
+                if not isinstance(item, dict):
+                    print(
+                        f"Expected a dictionary in the list for key: {key}, got {type(item)}"
+                    )
+                    return False
+                # Recursively check the structure of each dictionary in the list
+                if not match_structure(expected_type[0], item):
+                    return False
+        elif isinstance(expected_type, dict):
             # If the expected type is a dictionary, recursively check the structure
             if not isinstance(data[key], dict):
                 print(f"Expected a dictionary for key: {key}, got {type(data[key])}")
                 return False
             if not match_structure(expected_type, data[key]):
                 return False
         elif isinstance(expected_type, type):
             # Direct type checking
             if not isinstance(data[key], expected_type):
-                print(f"Key '{key}' expected {expected_type}, got {type(data[key])}")
+                print(
+                    f"Key '{key}' expected {expected_type.__name__}, got {type(data[key]).__name__}"
+                )
                 return False
         else:
-            print(f"Unsupported type specification: {expected_type}")
+            # This block now handles cases where expected_type is not recognized
+            print(f"Unsupported type specification for key '{key}': {expected_type}")
             return False
 
     return True
 
 
 def _find_json_snippet(raw_snippet):
     """
```

## Comparing `hllama-0.0.4.dist-info/LICENSE` & `hllama-0.0.6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `hllama-0.0.4.dist-info/METADATA` & `hllama-0.0.6.dist-info/METADATA`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hllama
-Version: 0.0.4
+Version: 0.0.6
 Summary: hllama provides some useful utility functions for LLM.
 Home-page: https://github.com/deep-diver/hllama
 Author: chansung park
 Author-email: deep.diver.csp@gmail.com
 Keywords: LLM,Large Language Model,Verification,Utility
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

## Comparing `hllama-0.0.4.dist-info/RECORD` & `hllama-0.0.6.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-hllama/__init__.py,sha256=jSg6X7xjfhk3oWuEIkZHjPqY0R3IyjvCzvVUR4h54jM,48
-hllama/json_utils.py,sha256=bDCwgJr7jMjk-xSGf7a7BS9YkBg-zHZF2NUs29N66nE,2304
-hllama-0.0.4.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-hllama-0.0.4.dist-info/METADATA,sha256=gdWx84-GG68unGKL8vaKnd_Jaab968m4Bc5sbxhuE7o,1402
-hllama-0.0.4.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-hllama-0.0.4.dist-info/top_level.txt,sha256=ARnLMMR8NzM9RnQhrEQXQJgFVcD9qc6CYJVram6SS9Y,7
-hllama-0.0.4.dist-info/RECORD,,
+hllama/__init__.py,sha256=QiiYsv0kcJaB8wCWyT-FnI2b6be87HA-CrrIUn8LQhg,22
+hllama/json_utils.py,sha256=tVSl8mnzyOFyf11odEjvshJATi40j8x1MPmPHqGg19c,3301
+hllama-0.0.6.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+hllama-0.0.6.dist-info/METADATA,sha256=hx9Bg4bRZ1NGIH8kbPMT8MO9Wt9Z59uEI6_jHuvMKhk,1402
+hllama-0.0.6.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+hllama-0.0.6.dist-info/top_level.txt,sha256=ARnLMMR8NzM9RnQhrEQXQJgFVcD9qc6CYJVram6SS9Y,7
+hllama-0.0.6.dist-info/RECORD,,
```

