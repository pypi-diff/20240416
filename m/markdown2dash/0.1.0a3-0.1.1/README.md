# Comparing `tmp/markdown2dash-0.1.0a3.tar.gz` & `tmp/markdown2dash-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "markdown2dash-0.1.0a3.tar", max compression
+gzip compressed data, was "markdown2dash-0.1.1.tar", max compression
```

## Comparing `markdown2dash-0.1.0a3.tar` & `markdown2dash-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,18 @@
--rw-r--r--   0        0        0     1069 2023-08-09 17:04:50.363457 markdown2dash-0.1.0a3/LICENSE
--rw-r--r--   0        0        0     5850 2023-08-16 14:21:51.549569 markdown2dash-0.1.0a3/README.md
--rw-r--r--   0        0        0      434 2023-08-18 02:24:44.861413 markdown2dash-0.1.0a3/markdown2dash/__init__.py
--rw-r--r--   0        0        0      367 2023-08-16 10:00:21.280058 markdown2dash-0.1.0a3/markdown2dash/src/decorators.py
--rw-r--r--   0        0        0      410 2023-08-16 10:01:43.165098 markdown2dash-0.1.0a3/markdown2dash/src/directives/admonition.py
--rw-r--r--   0        0        0     1101 2023-08-16 10:00:42.384225 markdown2dash-0.1.0a3/markdown2dash/src/directives/base.py
--rw-r--r--   0        0        0      834 2023-08-16 10:01:53.791751 markdown2dash-0.1.0a3/markdown2dash/src/directives/exec.py
--rw-r--r--   0        0        0      304 2023-08-16 10:01:57.695655 markdown2dash-0.1.0a3/markdown2dash/src/directives/image.py
--rw-r--r--   0        0        0     1444 2023-08-16 10:31:38.867216 markdown2dash-0.1.0a3/markdown2dash/src/directives/kwargs.py
--rw-r--r--   0        0        0     1880 2023-08-17 18:09:34.062119 markdown2dash-0.1.0a3/markdown2dash/src/directives/toc.py
--rw-r--r--   0        0        0      808 2023-08-16 06:35:05.068396 markdown2dash-0.1.0a3/markdown2dash/src/parser.py
--rw-r--r--   0        0        0     3197 2023-08-18 02:24:37.705572 markdown2dash-0.1.0a3/markdown2dash/src/renderer.py
--rw-r--r--   0        0        0      729 2023-08-16 09:53:13.580520 markdown2dash-0.1.0a3/markdown2dash/src/utils.py
--rw-r--r--   0        0        0     1735 2023-09-10 11:52:53.669136 markdown2dash-0.1.0a3/pyproject.toml
--rw-r--r--   0        0        0     6949 2023-09-10 11:55:53.383152 markdown2dash-0.1.0a3/setup.py
--rw-r--r--   0        0        0     7652 2023-09-10 11:55:53.383736 markdown2dash-0.1.0a3/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-08-09 17:04:50.363457 markdown2dash-0.1.1/LICENSE
+-rw-r--r--   0        0        0    11403 2024-04-16 12:06:37.805500 markdown2dash-0.1.1/README.md
+-rw-r--r--   0        0        0      639 2024-04-16 12:07:05.092745 markdown2dash-0.1.1/markdown2dash/__init__.py
+-rw-r--r--   0        0        0      399 2024-04-16 11:20:15.525425 markdown2dash-0.1.1/markdown2dash/src/decorators.py
+-rw-r--r--   0        0        0      410 2024-04-13 12:27:40.899415 markdown2dash-0.1.1/markdown2dash/src/directives/admonition.py
+-rw-r--r--   0        0        0     1101 2023-08-16 10:00:42.384225 markdown2dash-0.1.1/markdown2dash/src/directives/base.py
+-rw-r--r--   0        0        0      312 2024-04-13 11:17:44.362364 markdown2dash-0.1.1/markdown2dash/src/directives/divider.py
+-rw-r--r--   0        0        0      842 2024-04-13 11:43:55.583632 markdown2dash-0.1.1/markdown2dash/src/directives/exec.py
+-rw-r--r--   0        0        0      304 2024-04-13 11:11:26.268821 markdown2dash-0.1.1/markdown2dash/src/directives/image.py
+-rw-r--r--   0        0        0     1564 2024-04-16 12:07:05.145583 markdown2dash-0.1.1/markdown2dash/src/directives/kwargs.py
+-rw-r--r--   0        0        0      442 2024-04-13 11:48:35.568796 markdown2dash-0.1.1/markdown2dash/src/directives/source.py
+-rw-r--r--   0        0        0     1863 2024-04-13 07:25:15.024723 markdown2dash-0.1.1/markdown2dash/src/directives/toc.py
+-rw-r--r--   0        0        0      988 2024-04-15 18:45:00.927682 markdown2dash-0.1.1/markdown2dash/src/parser.py
+-rw-r--r--   0        0        0     3799 2024-04-16 05:12:21.364237 markdown2dash-0.1.1/markdown2dash/src/renderer.py
+-rw-r--r--   0        0        0      729 2023-08-16 09:53:13.580520 markdown2dash-0.1.1/markdown2dash/src/utils.py
+-rw-r--r--   0        0        0     1746 2024-04-15 18:45:25.562689 markdown2dash-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0    12705 2024-04-16 12:09:47.309582 markdown2dash-0.1.1/setup.py
+-rw-r--r--   0        0        0    13239 2024-04-16 12:09:47.310649 markdown2dash-0.1.1/PKG-INFO
```

### Comparing `markdown2dash-0.1.0a3/LICENSE` & `markdown2dash-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `markdown2dash-0.1.0a3/markdown2dash/src/directives/base.py` & `markdown2dash-0.1.1/markdown2dash/src/directives/base.py`

 * *Files identical despite different names*

### Comparing `markdown2dash-0.1.0a3/markdown2dash/src/directives/kwargs.py` & `markdown2dash-0.1.1/markdown2dash/src/directives/kwargs.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import importlib
 import inspect
 
 import dash_mantine_components as dmc
-from dash import html
 from dash.development.base_component import Component
 
 from .base import BaseDirective
 from ..utils import convert_docstring_to_dict
 
 
 class Kwargs(BaseDirective):
@@ -27,18 +26,23 @@
             imported = importlib.import_module(package)
             component = getattr(imported, component_name)
             docstring = inspect.getdoc(component).split("Keyword arguments:")[-1]
             attrs["kwargs"] = convert_docstring_to_dict(docstring)
 
     def render(self, renderer, title: str, content: str, **options) -> Component:
         data = options.pop("kwargs")
-        head = renderer.table_head(
-            [renderer.table_cell(col.title(), head=True) for col in data[0]]
-        )
-        body = renderer.table_body(
-            [
-                renderer.table_row([renderer.table_cell(col) for col in row.values()])
-                for row in data
-            ]
-        )
-        table = dmc.Table([head, body], **options)
+        if data:
+            head = renderer.table_head(
+                [renderer.table_cell(col.title(), head=True) for col in data[0]]
+            )
+            body = renderer.table_body(
+                [
+                    renderer.table_row(
+                        [renderer.table_cell(col) for col in row.values()]
+                    )
+                    for row in data
+                ]
+            )
+            table = dmc.Table([head, body], **options)
+        else:
+            table = None
         return table
```

### Comparing `markdown2dash-0.1.0a3/markdown2dash/src/directives/toc.py` & `markdown2dash-0.1.1/markdown2dash/src/directives/toc.py`

 * *Files 9% similar despite different names*

```diff
@@ -31,24 +31,24 @@
 
             attrs["table_of_contents"] = table_of_contents
             attrs["title"] = attrs["title"] or "Table of Contents"
 
     def render(self, renderer, title: str, content: str, **options) -> Component:
         table_of_contents = options.pop("table_of_contents")
         min_level = int(options.pop("min_level", "3"))
-        paddings = {3: 0, 5: 40}
+        paddings = {3: 0, 4: 30, 5: 60}
         links = [
             html.A(
-                dmc.Text(text, color="indigo", size="sm"),
+                dmc.Text(text, c="indigo"),
                 href="#" + hid,
                 style={
                     "textTransform": "capitalize",
                     "textDecoration": "none",
                     "paddingLeft": paddings[level],
                     "width": "fit-content",
                 },
             )
             for level, text, hid in table_of_contents
             if level >= min_level
         ]
-        heading = dmc.Text(title, mb=10, weight=500) if links else None
-        return dmc.Stack([heading, *links], spacing=4, mt=20, mb=30, **options)
+        heading = dmc.Text(title, mb=10, w=500) if links else None
+        return dmc.Stack([heading, *links], gap=4, mt=20, mb=30, **options)
```

### Comparing `markdown2dash-0.1.0a3/markdown2dash/src/renderer.py` & `markdown2dash-0.1.1/markdown2dash/src/renderer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,27 @@
-from typing import List
 from urllib.parse import urlparse
 
 import dash_mantine_components as dmc
-from dash import html
 from dash.development.base_component import Component
 from mistune import safe_entity, HTMLRenderer
 
 from .decorators import class_name
 from .utils import create_heading_id
 
 
+def flatten(xs):
+    result = []
+    if isinstance(xs, (list, tuple)):
+        for x in xs:
+            result.extend(flatten(x))
+    else:
+        result.append(xs)
+    return result
+
+
 # noinspection PyMethodMayBeStatic
 class DashRenderer(HTMLRenderer):
     NAME = "dash"
 
     def text(self, text: str) -> str:
         return text
 
@@ -28,19 +36,19 @@
 
     @class_name
     def paragraph(self, text: str) -> Component:
         return dmc.Text(text)
 
     @class_name
     def emphasis(self, text: str) -> Component:
-        return dmc.Text(text, fs="italic")
+        return dmc.Text(text, fs="italic", display="inline")
 
     @class_name
     def strong(self, text: str) -> Component:
-        return dmc.Text(text, weight="bold")
+        return dmc.Text(text, fw="bold", display="inline")
 
     @class_name
     def codespan(self, text: str) -> Component:
         return dmc.Code(text)
 
     @class_name
     def heading(self, text: str, level: int, **attrs) -> Component:
@@ -55,34 +63,31 @@
 
     @class_name
     def block_code(self, code: str, info=None) -> Component:
         if info is not None:
             info = safe_entity(info.strip())
         if info:
             lang = info.split(None, 1)[0]
-            return dmc.Prism(code, language=lang)
+            return dmc.CodeHighlight(code, language=lang)
         else:
             return dmc.Code(code)
 
     @class_name
     def block_quote(self, text: str) -> Component:
         return dmc.Blockquote(text)
 
     @class_name
-    def list_item(self, text: str) -> Component:
-        if isinstance(text[0], list):
-            text = text[0]
+    def list_item(self, text: list) -> Component:
+        text = flatten(text)
         return dmc.ListItem(text)
 
     @class_name
-    def list(self, text: List[dmc.ListItem], ordered: bool, **attrs) -> Component:
+    def list(self, text, ordered: bool, **attrs) -> Component:
         return dmc.List(
-            text,
-            type="ordered" if ordered else "unordered",
-            withPadding=True,
+            text, type="ordered" if ordered else "unordered", withPadding=True
         )
 
     @class_name
     def strikethrough(self, text: str) -> Component:
         return dmc.Text(text, td="line-through")
 
     @class_name
@@ -91,27 +96,40 @@
 
     @class_name
     def table(self, text: Component) -> Component:
         return dmc.Table(text)
 
     @class_name
     def table_head(self, text: str) -> Component:
-        return html.Thead(html.Tr(text))
+        return dmc.TableThead(self.table_row(text))
 
     @class_name
     def table_body(self, text: Component) -> Component:
-        return html.Tbody(text)
+        return dmc.TableTbody(text)
 
     @class_name
     def table_row(self, text: str) -> Component:
-        return html.Tr(text)
+        return dmc.TableTr(text)
 
     @class_name
-    def table_cell(self, text: str, align=None, head=False):
-        return html.Th(text) if head else html.Td(text)
+    def table_cell(self, text: str, align=None, head=False) -> Component:
+        return dmc.TableTh(text) if head else dmc.TableTd(text)
 
     def blank_line(self) -> None:
         return
 
+    @class_name
+    def block_spoiler(self, children: Component) -> Component:
+        return dmc.Spoiler(children, hideLabel="Show less", showLabel="Show more")
+
+    @class_name
+    def task_list_item(self, text: list, checked: bool, **attrs):
+        text = flatten(text)
+        return dmc.ListItem(
+            dmc.Checkbox(dmc.Text(text), checked=checked),
+            style={"listStyleType": "none"},
+        )
+
     def render_tokens(self, tokens, state):
         components = list(self.iter_tokens(tokens, state))
-        return [comp for comp in components if comp]
+        components = [comp for comp in components if comp is not None]
+        return components
```

### Comparing `markdown2dash-0.1.0a3/markdown2dash/src/utils.py` & `markdown2dash-0.1.1/markdown2dash/src/utils.py`

 * *Files identical despite different names*

### Comparing `markdown2dash-0.1.0a3/pyproject.toml` & `markdown2dash-0.1.1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "markdown2dash"
-version = "0.1.0a3"
+version = "0.1.1"
 description = "Render markdown into a dash layout using dash-mantine-components"
 authors = ["Snehil Vijay <snehilvj@outlook.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/snehilvj/markdown2dash"
 repository = "https://github.com/snehilvj/markdown2dash"
 documentation = "https://github.com/snehilvj/markdown2dash"
@@ -30,19 +30,20 @@
     "Topic :: Scientific/Engineering :: Visualization",
     "Topic :: Software Development :: Libraries :: Application Frameworks",
     "Topic :: Software Development :: Widget Sets",
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.7"
-dash = "^2.11.1"
-dash-mantine-components = "0.13.0a3"
+dash = "^2"
+dash-mantine-components = "^0.14"
 mistune = "^3.0.1"
 jsonpath = "^0.82"
 dash-iconify = "^0.1.2"
+gunicorn = "^21.2.0"
 
 [tool.poetry.dev-dependencies]
 black = "^22.1.0"
 twine = "^4.0.2"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

