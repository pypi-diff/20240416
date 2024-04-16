# Comparing `tmp/haruka_parser-0.4.9.tar.gz` & `tmp/haruka_parser-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "haruka_parser-0.4.9.tar", last modified: Fri Apr  5 19:51:21 2024, max compression
+gzip compressed data, was "haruka_parser-0.5.0.tar", last modified: Tue Apr 16 10:07:11 2024, max compression
```

## Comparing `haruka_parser-0.4.9.tar` & `haruka_parser-0.5.0.tar`

### file list

```diff
@@ -1,35 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:51:21.953289 haruka_parser-0.4.9/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-05 19:51:15.000000 haruka_parser-0.4.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-04-05 19:51:21.953289 haruka_parser-0.4.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-04-05 19:51:15.000000 haruka_parser-0.4.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:51:21.949289 haruka_parser-0.4.9/haruka_parser/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 19:51:15.000000 haruka_parser-0.4.9/haruka_parser/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:51:21.949289 haruka_parser-0.4.9/haruka_parser/dictionary/
--rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-04-05 19:51:15.000000 haruka_parser-0.4.9/haruka_parser/dictionary/banned_selectors.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-04-05 19:51:15.000000 haruka_parser-0.4.9/haruka_parser/dictionary/boilerplate_words.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2582 2024-04-05 19:51:15.000000 haruka_parser-0.4.9/haruka_parser/dictionary/latex_words.txt
--rw-r--r--   0 runner    (1001) docker     (127)    15907 2024-04-05 19:51:15.000000 haruka_parser-0.4.9/haruka_parser/extract.py
--rw-r--r--   0 runner    (1001) docker     (127)    33581 2024-04-05 19:51:15.000000 haruka_parser-0.4.9/haruka_parser/latex_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)     4338 2024-04-05 19:51:15.000000 haruka_parser-0.4.9/haruka_parser/line_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)    23265 2024-04-05 19:51:15.000000 haruka_parser-0.4.9/haruka_parser/meta_processing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:51:21.953289 haruka_parser-0.4.9/haruka_parser/mmltex/
--rw-r--r--   0 runner    (1001) docker     (127)    36723 2024-04-05 19:51:15.000000 haruka_parser-0.4.9/haruka_parser/mmltex/cmarkup.xsl
--rw-r--r--   0 runner    (1001) docker     (127)    71528 2024-04-05 19:51:15.000000 haruka_parser-0.4.9/haruka_parser/mmltex/entities.xsl
--rw-r--r--   0 runner    (1001) docker     (127)     6333 2024-04-05 19:51:15.000000 haruka_parser-0.4.9/haruka_parser/mmltex/glayout.xsl
--rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-04-05 19:51:15.000000 haruka_parser-0.4.9/haruka_parser/mmltex/mmltex.xsl
--rw-r--r--   0 runner    (1001) docker     (127)     9901 2024-04-05 19:51:15.000000 haruka_parser-0.4.9/haruka_parser/mmltex/scripts.xsl
--rw-r--r--   0 runner    (1001) docker     (127)     4327 2024-04-05 19:51:15.000000 haruka_parser-0.4.9/haruka_parser/mmltex/tables.xsl
--rw-r--r--   0 runner    (1001) docker     (127)    10654 2024-04-05 19:51:15.000000 haruka_parser-0.4.9/haruka_parser/mmltex/tokens.xsl
--rw-r--r--   0 runner    (1001) docker     (127)    35530 2024-04-05 19:51:15.000000 haruka_parser-0.4.9/haruka_parser/readablity_lxml.py
--rw-r--r--   0 runner    (1001) docker     (127)    14291 2024-04-05 19:51:15.000000 haruka_parser-0.4.9/haruka_parser/time_formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)    15057 2024-04-05 19:51:15.000000 haruka_parser-0.4.9/haruka_parser/tree_cleaning.py
--rw-r--r--   0 runner    (1001) docker     (127)    27457 2024-04-05 19:51:15.000000 haruka_parser-0.4.9/haruka_parser/tree_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)     9574 2024-04-05 19:51:15.000000 haruka_parser-0.4.9/haruka_parser/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:51:21.953289 haruka_parser-0.4.9/haruka_parser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-04-05 19:51:21.000000 haruka_parser-0.4.9/haruka_parser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-05 19:51:21.000000 haruka_parser-0.4.9/haruka_parser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 19:51:21.000000 haruka_parser-0.4.9/haruka_parser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-05 19:51:21.000000 haruka_parser-0.4.9/haruka_parser.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-05 19:51:21.000000 haruka_parser-0.4.9/haruka_parser.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 19:51:21.953289 haruka_parser-0.4.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-04-05 19:51:15.000000 haruka_parser-0.4.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:07:11.477351 haruka_parser-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-16 10:07:04.000000 haruka_parser-0.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-04-16 10:07:11.477351 haruka_parser-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-04-16 10:07:04.000000 haruka_parser-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:07:11.457351 haruka_parser-0.5.0/haruka_parser/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 10:07:04.000000 haruka_parser-0.5.0/haruka_parser/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:07:11.461351 haruka_parser-0.5.0/haruka_parser/dictionary/
+-rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-04-16 10:07:04.000000 haruka_parser-0.5.0/haruka_parser/dictionary/banned_selectors.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-04-16 10:07:04.000000 haruka_parser-0.5.0/haruka_parser/dictionary/boilerplate_words.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2582 2024-04-16 10:07:04.000000 haruka_parser-0.5.0/haruka_parser/dictionary/latex_words.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    16827 2024-04-16 10:07:04.000000 haruka_parser-0.5.0/haruka_parser/extract.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33581 2024-04-16 10:07:04.000000 haruka_parser-0.5.0/haruka_parser/latex_processing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:07:11.465351 haruka_parser-0.5.0/haruka_parser/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)  4970706 2024-04-16 10:07:04.000000 haruka_parser-0.5.0/haruka_parser/lib/libparser-arm64.dylib
+-rw-r--r--   0 runner    (1001) docker     (127)  6978584 2024-04-16 10:07:04.000000 haruka_parser-0.5.0/haruka_parser/lib/libparser-x86.so
+-rw-r--r--   0 runner    (1001) docker     (127)     4338 2024-04-16 10:07:04.000000 haruka_parser-0.5.0/haruka_parser/line_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23265 2024-04-16 10:07:04.000000 haruka_parser-0.5.0/haruka_parser/meta_processing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:07:11.477351 haruka_parser-0.5.0/haruka_parser/mmltex/
+-rw-r--r--   0 runner    (1001) docker     (127)    36723 2024-04-16 10:07:04.000000 haruka_parser-0.5.0/haruka_parser/mmltex/cmarkup.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)    71528 2024-04-16 10:07:04.000000 haruka_parser-0.5.0/haruka_parser/mmltex/entities.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)     6333 2024-04-16 10:07:04.000000 haruka_parser-0.5.0/haruka_parser/mmltex/glayout.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-04-16 10:07:04.000000 haruka_parser-0.5.0/haruka_parser/mmltex/mmltex.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)     9901 2024-04-16 10:07:04.000000 haruka_parser-0.5.0/haruka_parser/mmltex/scripts.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)     4327 2024-04-16 10:07:04.000000 haruka_parser-0.5.0/haruka_parser/mmltex/tables.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)    10654 2024-04-16 10:07:04.000000 haruka_parser-0.5.0/haruka_parser/mmltex/tokens.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-16 10:07:04.000000 haruka_parser-0.5.0/haruka_parser/readablity_go.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35597 2024-04-16 10:07:04.000000 haruka_parser-0.5.0/haruka_parser/readablity_lxml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14291 2024-04-16 10:07:04.000000 haruka_parser-0.5.0/haruka_parser/time_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15057 2024-04-16 10:07:04.000000 haruka_parser-0.5.0/haruka_parser/tree_cleaning.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27590 2024-04-16 10:07:04.000000 haruka_parser-0.5.0/haruka_parser/tree_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9574 2024-04-16 10:07:04.000000 haruka_parser-0.5.0/haruka_parser/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:07:11.477351 haruka_parser-0.5.0/haruka_parser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-04-16 10:07:11.000000 haruka_parser-0.5.0/haruka_parser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-04-16 10:07:11.000000 haruka_parser-0.5.0/haruka_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 10:07:11.000000 haruka_parser-0.5.0/haruka_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-16 10:07:11.000000 haruka_parser-0.5.0/haruka_parser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-16 10:07:11.000000 haruka_parser-0.5.0/haruka_parser.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 10:07:11.477351 haruka_parser-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-04-16 10:07:04.000000 haruka_parser-0.5.0/setup.py
```

### Comparing `haruka_parser-0.4.9/PKG-INFO` & `haruka_parser-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: haruka_parser
-Version: 0.4.9
+Version: 0.5.0
 Summary: A simple HTML Parser
 Home-page: https://github.com/prnake/haruka-parser
 Author: papersnake
 Author-email: prnake@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: haruka_parser Version: 0.4.9 Summary: A simple HTML
+Metadata-Version: 2.1 Name: haruka_parser Version: 0.5.0 Summary: A simple HTML
 Parser Home-page: https://github.com/prnake/haruka-parser Author: papersnake
 Author-email: prnake@gmail.com Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Classifier: Topic :: Text Processing Classifier: Topic ::
 Text Processing :: Markup :: HTML Classifier: Topic :: Utilities Description-
 Content-Type: text/markdown Requires-Dist: py_asciimath Requires-Dist:
 inscriptis Requires-Dist: tabulate Requires-Dist: numpy Requires-Dist:
```

### Comparing `haruka_parser-0.4.9/README.md` & `haruka_parser-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.9/haruka_parser/dictionary/banned_selectors.txt` & `haruka_parser-0.5.0/haruka_parser/dictionary/banned_selectors.txt`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.9/haruka_parser/dictionary/boilerplate_words.txt` & `haruka_parser-0.5.0/haruka_parser/dictionary/boilerplate_words.txt`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.9/haruka_parser/dictionary/latex_words.txt` & `haruka_parser-0.5.0/haruka_parser/dictionary/latex_words.txt`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.9/haruka_parser/extract.py` & `haruka_parser-0.5.0/haruka_parser/extract.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
 import re
+import traceback
 import unicodedata
 from collections import defaultdict
 from typing import Dict
 from haruka_parser.readablity_lxml import Document, get_html
 from resiliparse.parse.html import HTMLTree
 from resiliparse.extract.html2text import extract_plain_text
 from inscriptis import ParserConfig
@@ -64,14 +65,15 @@
     remove_chinese_characters,
     remove_boilerplate,
     restore_replacements,
 )
 from haruka_parser.utils import IMG_SRC_ATTR, ReplacementManager, fast_html2text
 from haruka_parser.meta_processing import extract_metadata
 from haruka_parser.tree_cleaning import OVERALL_DISCARD_XPATH, PAYWALL_DISCARD_XPATH, TEASER_DISCARD_XPATH, prune_unwanted_nodes, tree_cleaning, delete_by_link_density
+from haruka_parser.readablity_go import readablity_go_parse
 
 DEFAULT_CONFIG = defaultdict(
     bool,
     {
         "add_title": True,
         "readability": False,
         "skip_large_links": False,
@@ -262,27 +264,64 @@
     
     info["text_list"] = processed_text
     info["images"] = images
     info['images_meta'] = new_image_list
     # 返回处理后的文本和图片URL列表
     return info
 
+def readability_parse(full_html, pre_process_tree, info, website_url="https://example.com"):
+    try:
+        res_html = None
+
+        full_content = fast_html2text(full_html, filter_length = 20)
+
+        # readability go
+        try:
+            data = readablity_go_parse(full_html, website_url)
+            res_html = data["html"]
+            info["meta"].update(data["metadata"])
+        except:
+            # dev monitoring
+            traceback.print_exc()
+
+        if res_html:
+            clean_content = fast_html2text(res_html, filter_length = 20)
+
+            if (len(clean_content) + 200) / (len(full_content) + 200) > 0.67:
+                info["use_readability"] = True
+                info["use_readability_go"] = True
+                return res_html
+
+        # readability lxml
+        res_html, clean_tree = Document(pre_process_tree).summary()
 
-def extract_text(html, config=DEFAULT_CONFIG, encoding="utf-8"):
+        clean_content = fast_html2text(res_html, filter_length = 20)
+
+        if (len(clean_content) + 200) / (len(full_content) + 200) > 0.67:
+            info["use_readability"] = True
+            info["use_readability_go"] = False
+            return res_html
+    except:
+        pass
+    
+    return full_html
+
+def extract_text(html, config=DEFAULT_CONFIG, encoding="utf-8", website_url="https://example.com"):
     """Extracts plain text from an HTML string."""
     
     def _start_li(state: HtmlDocumentState, _: Dict) -> None:
         """Handle the <li> tag."""
         pass
 
     info = {
         "found_math": False,
         "found_latex_text": False,
         "found_latex_script": False,
         "use_readability": False,
+        "use_readability_go": False,
         "script_math_tex": 0,
         "script_math_asciimath": 0,
         "math_annotations": 0,
         "math_alttext": 0,
         "mathml": 0,
         "mathjax_tag": 0,
         "mathjax_inline_tex": 0,
@@ -336,15 +375,15 @@
 
     filter_tree(pre_process_resiliparse_tree, config, info)
 
     pre_process_tree = get_lxml_tree(str(pre_process_resiliparse_tree))
 
     # try: info["time"] = extract_time(html, pre_process_tree)
     # except: pass
-    try: info['meta'] = extract_metadata(pre_process_tree)
+    try: info["meta"].update(extract_metadata(pre_process_tree))
     except: pass
 
     # jobs done by trafilatura
     try:
         pre_process_tree = tree_cleaning(pre_process_tree)
         pre_process_tree = prune_unwanted_nodes(pre_process_tree, OVERALL_DISCARD_XPATH, with_backup=True)
         pre_process_tree = prune_unwanted_nodes(pre_process_tree, PAYWALL_DISCARD_XPATH)
@@ -355,28 +394,15 @@
         pre_process_tree = delete_by_link_density(pre_process_tree, 'p', backtracking=False, favor_precision=False)
     except:
         pass
     
     full_html = get_html(pre_process_tree)
         
     if config["readability"]:
-        try:
-            
-            full_content = fast_html2text(full_html, filter_length = 20)
-            # origin readability
-            html, clean_tree = Document(pre_process_tree).summary()
-
-            clean_content = fast_html2text(html, filter_length = 20)
-
-            if (len(clean_content) + 200) / (len(full_content) + 200) < 0.67:
-                html = full_html
-            else:
-                info["use_readability"] = True
-        except:
-            html = full_html
+        html = readability_parse(full_html, pre_process_tree, info, website_url)
     else:
         html = full_html
 
     html = html_preprocessing(html, config)
     tree = HTMLTree.parse(html)
     replacement_manager = ReplacementManager()
```

### Comparing `haruka_parser-0.4.9/haruka_parser/latex_processing.py` & `haruka_parser-0.5.0/haruka_parser/latex_processing.py`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.9/haruka_parser/line_processing.py` & `haruka_parser-0.5.0/haruka_parser/line_processing.py`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.9/haruka_parser/meta_processing.py` & `haruka_parser-0.5.0/haruka_parser/meta_processing.py`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.9/haruka_parser/mmltex/cmarkup.xsl` & `haruka_parser-0.5.0/haruka_parser/mmltex/cmarkup.xsl`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.9/haruka_parser/mmltex/entities.xsl` & `haruka_parser-0.5.0/haruka_parser/mmltex/entities.xsl`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.9/haruka_parser/mmltex/glayout.xsl` & `haruka_parser-0.5.0/haruka_parser/mmltex/glayout.xsl`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.9/haruka_parser/mmltex/mmltex.xsl` & `haruka_parser-0.5.0/haruka_parser/mmltex/mmltex.xsl`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.9/haruka_parser/mmltex/scripts.xsl` & `haruka_parser-0.5.0/haruka_parser/mmltex/scripts.xsl`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.9/haruka_parser/mmltex/tables.xsl` & `haruka_parser-0.5.0/haruka_parser/mmltex/tables.xsl`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.9/haruka_parser/mmltex/tokens.xsl` & `haruka_parser-0.5.0/haruka_parser/mmltex/tokens.xsl`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.9/haruka_parser/readablity_lxml.py` & `haruka_parser-0.5.0/haruka_parser/readablity_lxml.py`

 * *Files 1% similar despite different names*

```diff
@@ -280,15 +280,17 @@
 
     if not 15 < len(title) < 150:
         return orig
 
     return title
 
 def get_html(doc):
-    return clean_attributes(tounicode(doc, method="html"))
+    return tounicode(doc, method="html")
+    # do not clean here
+    # return clean_attributes(tounicode(doc, method="html"))
 
 # is it necessary? Cleaner from LXML is initialized correctly in cleaners.py
 def get_body(doc):
     for elem in doc.xpath(".//script | .//link | .//style"):
         elem.drop_tree()
     # tostring() always return utf-8 encoded string
     # FIXME: isn't better to use tounicode?
```

### Comparing `haruka_parser-0.4.9/haruka_parser/time_formatter.py` & `haruka_parser-0.5.0/haruka_parser/time_formatter.py`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.9/haruka_parser/tree_cleaning.py` & `haruka_parser-0.5.0/haruka_parser/tree_cleaning.py`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.9/haruka_parser/tree_processing.py` & `haruka_parser-0.5.0/haruka_parser/tree_processing.py`

 * *Files 2% similar despite different names*

```diff
@@ -427,14 +427,15 @@
         if edit_button.parent:
             edit_button.parent.remove_child(edit_button)
 
 
 def remove_display_none(tree):
     # Remove all elements with display none
     elements = tree.document.query_selector_all('[style*="display:none"]')
+    # elements = tree.document.query_selector_all('[style*="display:none"], [style*="display: none"]')
     for element in elements:
         element.parent.remove_child(element)
 
 def remove_svg(tree):
     # Remove all elements with display none
     elements = tree.document.query_selector_all('svg')
     for element in elements:
@@ -693,44 +694,44 @@
     '//span[contains(@class, "pub_time")]/text()',
     '//span[contains(@class, "item-time")]/text()',
     '//span[contains(@class, "publishtime")]/text()',
     '//div[contains(@class, "news_time_source")]/text()',
 ]
 
 REGEX_TIME = [
-    "(\d{1,2}月\d{1,2}日)",
-    "(\d{2}年\d{1,2}月\d{1,2}日)",
-    "(\d{4}年\d{1,2}月\d{1,2}日)",
-    "(\d{2}[-|/|.]\d{1,2}[-|/|.]\d{1,2})",
-    "(\d{4}[-|/|.]\d{1,2}[-|/|.]\d{1,2})",
-    "(\d{1,2}月\d{1,2}日\s*?[2][0-3]:[0-5]?[0-9])",
-    "(\d{1,2}月\d{1,2}日\s*?[0-1]?[0-9]:[0-5]?[0-9])",
-    "(\d{2}年\d{1,2}月\d{1,2}日\s*?[2][0-3]:[0-5]?[0-9])",
-    "(\d{4}年\d{1,2}月\d{1,2}日\s*?[2][0-3]:[0-5]?[0-9])",
-    "(\d{2}年\d{1,2}月\d{1,2}日\s*?[0-1]?[0-9]:[0-5]?[0-9])",
-    "(\d{4}年\d{1,2}月\d{1,2}日\s*?[0-1]?[0-9]:[0-5]?[0-9])",
-    "(\d{1,2}月\d{1,2}日\s*?[1-24]\d时[0-60]\d分)([1-24]\d时)",
-    "(\d{1,2}月\d{1,2}日\s*?[2][0-3]:[0-5]?[0-9]:[0-5]?[0-9])",
-    "(\d{4}[-|/|.]\d{1,2}[-|/|.]\d{1,2}\s*?[2][0-3]:[0-5]?[0-9])",
-    "(\d{1,2}月\d{1,2}日\s*?[0-1]?[0-9]:[0-5]?[0-9]:[0-5]?[0-9])",
-    "(\d{2}[-|/|.]\d{1,2}[-|/|.]\d{1,2}\s*?[2][0-3]:[0-5]?[0-9])",
-    "(\d{4}[-|/|.]\d{1,2}[-|/|.]\d{1,2}\s*?[0-1]?[0-9]:[0-5]?[0-9])",
-    "(\d{2}[-|/|.]\d{1,2}[-|/|.]\d{1,2}\s*?[0-1]?[0-9]:[0-5]?[0-9])",
-    "(\d{2}年\d{1,2}月\d{1,2}日\s*?[1-24]\d时[0-60]\d分)([1-24]\d时)",
-    "(\d{4}年\d{1,2}月\d{1,2}日\s*?[1-24]\d时[0-60]\d分)([1-24]\d时)",
-    "(\d{2}年\d{1,2}月\d{1,2}日\s*?[2][0-3]:[0-5]?[0-9]:[0-5]?[0-9])",
-    "(\d{4}年\d{1,2}月\d{1,2}日\s*?[2][0-3]:[0-5]?[0-9]:[0-5]?[0-9])",
-    "(\d{2}年\d{1,2}月\d{1,2}日\s*?[0-1]?[0-9]:[0-5]?[0-9]:[0-5]?[0-9])",
-    "(\d{4}年\d{1,2}月\d{1,2}日\s*?[0-1]?[0-9]:[0-5]?[0-9]:[0-5]?[0-9])",
-    "(\d{4}[-|/|.]\d{1,2}[-|/|.]\d{1,2}\s*?[1-24]\d时[0-60]\d分)([1-24]\d时)",
-    "(\d{2}[-|/|.]\d{1,2}[-|/|.]\d{1,2}\s*?[1-24]\d时[0-60]\d分)([1-24]\d时)",
-    "(\d{2}[-|/|.]\d{1,2}[-|/|.]\d{1,2}\s*?[2][0-3]:[0-5]?[0-9]:[0-5]?[0-9])",
-    "(\d{4}[-|/|.]\d{1,2}[-|/|.]\d{1,2}\s*?[2][0-3]:[0-5]?[0-9]:[0-5]?[0-9])",
-    "(\d{4}[-|/|.]\d{1,2}[-|/|.]\d{1,2}\s*?[0-1]?[0-9]:[0-5]?[0-9]:[0-5]?[0-9])",
-    "(\d{2}[-|/|.]\d{1,2}[-|/|.]\d{1,2}\s*?[0-1]?[0-9]:[0-5]?[0-9]:[0-5]?[0-9])",
+    r"(\d{1,2}月\d{1,2}日)",
+    r"(\d{2}年\d{1,2}月\d{1,2}日)",
+    r"(\d{4}年\d{1,2}月\d{1,2}日)",
+    r"(\d{2}[-|/|.]\d{1,2}[-|/|.]\d{1,2})",
+    r"(\d{4}[-|/|.]\d{1,2}[-|/|.]\d{1,2})",
+    r"(\d{1,2}月\d{1,2}日\s*?[2][0-3]:[0-5]?[0-9])",
+    r"(\d{1,2}月\d{1,2}日\s*?[0-1]?[0-9]:[0-5]?[0-9])",
+    r"(\d{2}年\d{1,2}月\d{1,2}日\s*?[2][0-3]:[0-5]?[0-9])",
+    r"(\d{4}年\d{1,2}月\d{1,2}日\s*?[2][0-3]:[0-5]?[0-9])",
+    r"(\d{2}年\d{1,2}月\d{1,2}日\s*?[0-1]?[0-9]:[0-5]?[0-9])",
+    r"(\d{4}年\d{1,2}月\d{1,2}日\s*?[0-1]?[0-9]:[0-5]?[0-9])",
+    r"(\d{1,2}月\d{1,2}日\s*?[1-24]\d时[0-60]\d分)([1-24]\d时)",
+    r"(\d{1,2}月\d{1,2}日\s*?[2][0-3]:[0-5]?[0-9]:[0-5]?[0-9])",
+    r"(\d{4}[-|/|.]\d{1,2}[-|/|.]\d{1,2}\s*?[2][0-3]:[0-5]?[0-9])",
+    r"(\d{1,2}月\d{1,2}日\s*?[0-1]?[0-9]:[0-5]?[0-9]:[0-5]?[0-9])",
+    r"(\d{2}[-|/|.]\d{1,2}[-|/|.]\d{1,2}\s*?[2][0-3]:[0-5]?[0-9])",
+    r"(\d{4}[-|/|.]\d{1,2}[-|/|.]\d{1,2}\s*?[0-1]?[0-9]:[0-5]?[0-9])",
+    r"(\d{2}[-|/|.]\d{1,2}[-|/|.]\d{1,2}\s*?[0-1]?[0-9]:[0-5]?[0-9])",
+    r"(\d{2}年\d{1,2}月\d{1,2}日\s*?[1-24]\d时[0-60]\d分)([1-24]\d时)",
+    r"(\d{4}年\d{1,2}月\d{1,2}日\s*?[1-24]\d时[0-60]\d分)([1-24]\d时)",
+    r"(\d{2}年\d{1,2}月\d{1,2}日\s*?[2][0-3]:[0-5]?[0-9]:[0-5]?[0-9])",
+    r"(\d{4}年\d{1,2}月\d{1,2}日\s*?[2][0-3]:[0-5]?[0-9]:[0-5]?[0-9])",
+    r"(\d{2}年\d{1,2}月\d{1,2}日\s*?[0-1]?[0-9]:[0-5]?[0-9]:[0-5]?[0-9])",
+    r"(\d{4}年\d{1,2}月\d{1,2}日\s*?[0-1]?[0-9]:[0-5]?[0-9]:[0-5]?[0-9])",
+    r"(\d{4}[-|/|.]\d{1,2}[-|/|.]\d{1,2}\s*?[1-24]\d时[0-60]\d分)([1-24]\d时)",
+    r"(\d{2}[-|/|.]\d{1,2}[-|/|.]\d{1,2}\s*?[1-24]\d时[0-60]\d分)([1-24]\d时)",
+    r"(\d{2}[-|/|.]\d{1,2}[-|/|.]\d{1,2}\s*?[2][0-3]:[0-5]?[0-9]:[0-5]?[0-9])",
+    r"(\d{4}[-|/|.]\d{1,2}[-|/|.]\d{1,2}\s*?[2][0-3]:[0-5]?[0-9]:[0-5]?[0-9])",
+    r"(\d{4}[-|/|.]\d{1,2}[-|/|.]\d{1,2}\s*?[0-1]?[0-9]:[0-5]?[0-9]:[0-5]?[0-9])",
+    r"(\d{2}[-|/|.]\d{1,2}[-|/|.]\d{1,2}\s*?[0-1]?[0-9]:[0-5]?[0-9]:[0-5]?[0-9])",
 ]
 
 
 def get_valid_length_time(publish_time_list):
     if len(publish_time_list) > 0:
         length_valid_publish_time = [y for y in publish_time_list if len(y) >= 9]
         publish_time = (
```

### Comparing `haruka_parser-0.4.9/haruka_parser/utils.py` & `haruka_parser-0.5.0/haruka_parser/utils.py`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.9/haruka_parser.egg-info/PKG-INFO` & `haruka_parser-0.5.0/haruka_parser.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: haruka_parser
-Version: 0.4.9
+Version: 0.5.0
 Summary: A simple HTML Parser
 Home-page: https://github.com/prnake/haruka-parser
 Author: papersnake
 Author-email: prnake@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: haruka_parser Version: 0.4.9 Summary: A simple HTML
+Metadata-Version: 2.1 Name: haruka_parser Version: 0.5.0 Summary: A simple HTML
 Parser Home-page: https://github.com/prnake/haruka-parser Author: papersnake
 Author-email: prnake@gmail.com Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Classifier: Topic :: Text Processing Classifier: Topic ::
 Text Processing :: Markup :: HTML Classifier: Topic :: Utilities Description-
 Content-Type: text/markdown Requires-Dist: py_asciimath Requires-Dist:
 inscriptis Requires-Dist: tabulate Requires-Dist: numpy Requires-Dist:
```

### Comparing `haruka_parser-0.4.9/haruka_parser.egg-info/SOURCES.txt` & `haruka_parser-0.5.0/haruka_parser.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -2,27 +2,30 @@
 README.md
 setup.py
 haruka_parser/__init__.py
 haruka_parser/extract.py
 haruka_parser/latex_processing.py
 haruka_parser/line_processing.py
 haruka_parser/meta_processing.py
+haruka_parser/readablity_go.py
 haruka_parser/readablity_lxml.py
 haruka_parser/time_formatter.py
 haruka_parser/tree_cleaning.py
 haruka_parser/tree_processing.py
 haruka_parser/utils.py
 haruka_parser.egg-info/PKG-INFO
 haruka_parser.egg-info/SOURCES.txt
 haruka_parser.egg-info/dependency_links.txt
 haruka_parser.egg-info/requires.txt
 haruka_parser.egg-info/top_level.txt
 haruka_parser/dictionary/banned_selectors.txt
 haruka_parser/dictionary/boilerplate_words.txt
 haruka_parser/dictionary/latex_words.txt
+haruka_parser/lib/libparser-arm64.dylib
+haruka_parser/lib/libparser-x86.so
 haruka_parser/mmltex/cmarkup.xsl
 haruka_parser/mmltex/entities.xsl
 haruka_parser/mmltex/glayout.xsl
 haruka_parser/mmltex/mmltex.xsl
 haruka_parser/mmltex/scripts.xsl
 haruka_parser/mmltex/tables.xsl
 haruka_parser/mmltex/tokens.xsl
```

### Comparing `haruka_parser-0.4.9/setup.py` & `haruka_parser-0.5.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 # 0.1 version from OpenWebMath: https://github.com/keirp/OpenWebMath
 # OpenWebMath is made available under an ODC-By 1.0 license; users should also abide by the CommonCrawl ToU: https://commoncrawl.org/terms-of-use/. We do not alter the license of any of the underlying data.
 setup(
     name="haruka_parser",
-    version="0.4.9",
+    version="0.5.0",
     description="A simple HTML Parser",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="papersnake",
     author_email="prnake@gmail.com",
     url="https://github.com/prnake/haruka-parser",
     packages=["haruka_parser"],
```

