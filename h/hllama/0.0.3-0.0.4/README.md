# Comparing `tmp/hllama-0.0.3-py3-none-any.whl.zip` & `tmp/hllama-0.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 6414 bytes, number of entries: 7
--rw-rw-r--  2.0 unx       52 b- defN 24-Apr-16 01:36 hllama/__init__.py
--rw-rw-r--  2.0 unx     2094 b- defN 24-Apr-16 01:30 hllama/json_utils.py
--rw-rw-r--  2.0 unx    11357 b- defN 24-Apr-16 01:37 hllama-0.0.3.dist-info/LICENSE
--rw-rw-r--  2.0 unx      639 b- defN 24-Apr-16 01:37 hllama-0.0.3.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-Apr-16 01:37 hllama-0.0.3.dist-info/WHEEL
--rw-rw-r--  2.0 unx        7 b- defN 24-Apr-16 01:37 hllama-0.0.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      530 b- defN 24-Apr-16 01:37 hllama-0.0.3.dist-info/RECORD
-7 files, 14771 bytes uncompressed, 5476 bytes compressed:  62.9%
+Zip file size: 6812 bytes, number of entries: 7
+-rw-rw-r--  2.0 unx       48 b- defN 24-Apr-16 03:55 hllama/__init__.py
+-rw-rw-r--  2.0 unx     2304 b- defN 24-Apr-16 02:11 hllama/json_utils.py
+-rw-rw-r--  2.0 unx    11357 b- defN 24-Apr-16 03:56 hllama-0.0.4.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     1402 b- defN 24-Apr-16 03:56 hllama-0.0.4.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-Apr-16 03:56 hllama-0.0.4.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        7 b- defN 24-Apr-16 03:56 hllama-0.0.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      531 b- defN 24-Apr-16 03:56 hllama-0.0.4.dist-info/RECORD
+7 files, 15741 bytes uncompressed, 5874 bytes compressed:  62.7%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: hllama/__init__.py
 Comment: 
 
 Filename: hllama/json_utils.py
 Comment: 
 
-Filename: hllama-0.0.3.dist-info/LICENSE
+Filename: hllama-0.0.4.dist-info/LICENSE
 Comment: 
 
-Filename: hllama-0.0.3.dist-info/METADATA
+Filename: hllama-0.0.4.dist-info/METADATA
 Comment: 
 
-Filename: hllama-0.0.3.dist-info/WHEEL
+Filename: hllama-0.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: hllama-0.0.3.dist-info/top_level.txt
+Filename: hllama-0.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: hllama-0.0.3.dist-info/RECORD
+Filename: hllama-0.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## hllama/__init__.py

```diff
@@ -1,3 +1,3 @@
-__version__ = '0.0.3'
+__version__ = "0.0.4"
 
-from hllama import json_utils
+__all__ = ["json_utils"]
```

## hllama/json_utils.py

```diff
@@ -1,10 +1,11 @@
 import json
 from typing import Dict, Any
 
+
 def match_structure(schema: Dict[str, Any], data: Dict[str, Any]) -> bool:
     for key, expected_type in schema.items():
         if key not in data:
             print(f"Missing key: {key}")
             return False
 
         if isinstance(expected_type, dict):
@@ -21,47 +22,49 @@
                 return False
         else:
             print(f"Unsupported type specification: {expected_type}")
             return False
 
     return True
 
+
 def _find_json_snippet(raw_snippet):
-	"""
-	_find_json_snippet tries to find JSON snippets in a given raw_snippet string
-	"""
-	json_parsed_string = None
-
-	json_start_index = raw_snippet.find('{')
-	json_end_index = raw_snippet.rfind('}')
-
-	if json_start_index >= 0 and json_end_index >= 0:
-		json_snippet = raw_snippet[json_start_index:json_end_index+1]
-		try:
-			json_parsed_string = json.loads(json_snippet, strict=False)
-		except:
-			raise ValueError('failed to parse string into JSON format')
-	else:
-		raise ValueError('no JSON code snippet found in string.')
+    """
+    _find_json_snippet tries to find JSON snippets in a given raw_snippet string
+    """
+    json_parsed_string = None
+
+    json_start_index = raw_snippet.find("{")
+    json_end_index = raw_snippet.rfind("}")
+
+    if json_start_index >= 0 and json_end_index >= 0:
+        json_snippet = raw_snippet[json_start_index : json_end_index + 1]
+        try:
+            json_parsed_string = json.loads(json_snippet, strict=False)
+        except ValueError:
+            raise ValueError("failed to parse string into JSON format")
+    else:
+        raise ValueError("no JSON code snippet found in string.")
+
+    return json_parsed_string
 
-	return json_parsed_string
 
 def parse_first_json_snippet(snippet):
-	"""
-	parse_first_json_snippet tries to find JSON snippet and parse into json object
-	"""
-	json_parsed_string = None
-
-	if isinstance(snippet, list):
-		for snippet_piece in snippet:
-			try:
-				json_parsed_string = _find_json_snippet(snippet_piece)
-				return json_parsed_string
-			except:
-				pass
-	else:
-		try:
-			json_parsed_string = _find_json_snippet(snippet)
-		except Exception as e:
-			raise ValueError(str(e))
+    """
+    parse_first_json_snippet tries to find JSON snippet and parse into json object
+    """
+    json_parsed_string = None
+
+    if isinstance(snippet, list):
+        for snippet_piece in snippet:
+            try:
+                json_parsed_string = _find_json_snippet(snippet_piece)
+                return json_parsed_string
+            except ValueError:
+                pass
+    else:
+        try:
+            json_parsed_string = _find_json_snippet(snippet)
+        except Exception as e:
+            raise ValueError(str(e))
 
-	return json_parsed_string
+    return json_parsed_string
```

## Comparing `hllama-0.0.3.dist-info/LICENSE` & `hllama-0.0.4.dist-info/LICENSE`

 * *Files identical despite different names*

