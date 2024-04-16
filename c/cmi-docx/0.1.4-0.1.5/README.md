# Comparing `tmp/cmi_docx-0.1.4.tar.gz` & `tmp/cmi_docx-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmi_docx-0.1.4.tar", max compression
+gzip compressed data, was "cmi_docx-0.1.5.tar", max compression
```

## Comparing `cmi_docx-0.1.4.tar` & `cmi_docx-0.1.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    26526 2024-04-05 13:44:46.392508 cmi_docx-0.1.4/LICENSE
--rw-r--r--   0        0        0     2762 2024-04-05 13:44:46.392508 cmi_docx-0.1.4/README.md
--rw-r--r--   0        0        0     1557 2024-04-05 13:44:46.392508 cmi_docx-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      295 2024-04-05 13:44:46.392508 cmi_docx-0.1.4/src/cmi_docx/__init__.py
--rw-r--r--   0        0        0     4839 2024-04-05 13:44:46.392508 cmi_docx-0.1.4/src/cmi_docx/document.py
--rw-r--r--   0        0        0     4983 2024-04-05 13:44:46.392508 cmi_docx-0.1.4/src/cmi_docx/paragraph.py
--rw-r--r--   0        0        0     4747 2024-04-05 13:44:46.392508 cmi_docx-0.1.4/src/cmi_docx/run.py
--rw-r--r--   0        0        0     2684 2024-04-05 13:44:46.392508 cmi_docx-0.1.4/src/cmi_docx/table.py
--rw-r--r--   0        0        0     3278 1970-01-01 00:00:00.000000 cmi_docx-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0    26526 2024-04-16 20:57:19.130206 cmi_docx-0.1.5/LICENSE
+-rw-r--r--   0        0        0     2762 2024-04-16 20:57:19.130206 cmi_docx-0.1.5/README.md
+-rw-r--r--   0        0        0     1557 2024-04-16 20:57:19.130206 cmi_docx-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      295 2024-04-16 20:57:19.130206 cmi_docx-0.1.5/src/cmi_docx/__init__.py
+-rw-r--r--   0        0        0     4839 2024-04-16 20:57:19.130206 cmi_docx-0.1.5/src/cmi_docx/document.py
+-rw-r--r--   0        0        0     6029 2024-04-16 20:57:19.130206 cmi_docx-0.1.5/src/cmi_docx/paragraph.py
+-rw-r--r--   0        0        0     6833 2024-04-16 20:57:19.130206 cmi_docx-0.1.5/src/cmi_docx/run.py
+-rw-r--r--   0        0        0     2684 2024-04-16 20:57:19.130206 cmi_docx-0.1.5/src/cmi_docx/table.py
+-rw-r--r--   0        0        0     3278 1970-01-01 00:00:00.000000 cmi_docx-0.1.5/PKG-INFO
```

### Comparing `cmi_docx-0.1.4/LICENSE` & `cmi_docx-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cmi_docx-0.1.4/README.md` & `cmi_docx-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `cmi_docx-0.1.4/pyproject.toml` & `cmi_docx-0.1.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cmi_docx"
-version = "0.1.4"
+version = "0.1.5"
 description = ".docx utilities"
 authors = ["Reinder Vos de Wael <reinder.vosdewael@childmind.org>"]
 license = "LGPL-2.1"
 readme = "README.md"
 packages = [{include = "cmi_docx", from = "src"}]
 
 [tool.poetry.dependencies]
```

### Comparing `cmi_docx-0.1.4/src/cmi_docx/document.py` & `cmi_docx-0.1.5/src/cmi_docx/document.py`

 * *Files identical despite different names*

### Comparing `cmi_docx-0.1.4/src/cmi_docx/paragraph.py` & `cmi_docx-0.1.5/src/cmi_docx/paragraph.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 """Module for extending python-docx Paragraph objects."""
 
 import bisect
 import dataclasses
 import itertools
 import re
+from typing import Any
 
 from docx.enum import text
 from docx.text import paragraph as docx_paragraph
+from docx.text import run as docx_run
 
 from cmi_docx import run
 
 
 @dataclasses.dataclass
 class FindParagraph:
     """Data class for maintaing find results in paragraphs.
@@ -92,28 +94,55 @@
                     paragraph=self.paragraph,
                     run_indices=(start_run, end_run),
                     character_indices=(start_index, end_index),
                 )
             )
         return run_finds
 
-    def replace(self, needle: str, replace: str) -> None:
+    def replace(
+        self, needle: str, replace: str, style: dict[str, Any] | None = None
+    ) -> None:
         """Finds and replaces text in a Word paragraph.
 
         Args:
             needle: The text to find.
             replace: The text to replace.
+            style: The style to apply to the replacement text.
         """
         run_finder = self.find_in_runs(needle)
         run_finder.sort(
             key=lambda x: (x.run_indices[0], x.character_indices[0]), reverse=True
         )
 
         for run_find in run_finder:
-            run_find.replace(replace)
+            run_find.replace(replace, style)
+
+    def insert_run(self, index: int, text: str, style: dict[str, Any]) -> docx_run.Run:
+        """Inserts a run into a paragraph.
+
+        Args:
+            index: The index to insert the run at.
+            text: The text of the run.
+            style: The style of the run, see run.ExtendRun.format for more details.
+
+        Returns:
+            The inserted run.
+        """
+        if index == len(self.paragraph.runs):
+            self.paragraph.add_run(text)
+        else:
+            new_run = self.paragraph._element._new_r()
+            new_run.text = text
+            if index < 0:
+                self.paragraph.runs[index]._element.addnext(new_run)
+            else:
+                self.paragraph.runs[index]._element.addprevious(new_run)
+
+        run.ExtendRun(self.paragraph.runs[index]).format(**style)
+        return self.paragraph.runs[index]
 
     def format(
         self,
         *,
         bold: bool | None = None,
         italics: bool | None = None,
         font_size: int | None = None,
```

### Comparing `cmi_docx-0.1.4/src/cmi_docx/table.py` & `cmi_docx-0.1.5/src/cmi_docx/table.py`

 * *Files identical despite different names*

### Comparing `cmi_docx-0.1.4/PKG-INFO` & `cmi_docx-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmi_docx
-Version: 0.1.4
+Version: 0.1.5
 Summary: .docx utilities
 License: LGPL-2.1
 Author: Reinder Vos de Wael
 Author-email: reinder.vosdewael@childmind.org
 Requires-Python: >=3.10
 Classifier: License :: OSI Approved
 Classifier: Programming Language :: Python :: 3
```

