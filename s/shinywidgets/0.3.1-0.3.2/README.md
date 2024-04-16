# Comparing `tmp/shinywidgets-0.3.1.tar.gz` & `tmp/shinywidgets-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shinywidgets-0.3.1.tar", last modified: Fri Mar  1 16:55:29 2024, max compression
+gzip compressed data, was "shinywidgets-0.3.2.tar", last modified: Tue Apr 16 15:18:42 2024, max compression
```

## Comparing `shinywidgets-0.3.1.tar` & `shinywidgets-0.3.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 16:55:29.404805 shinywidgets-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-03-01 16:55:02.000000 shinywidgets-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-03-01 16:55:02.000000 shinywidgets-0.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-03-01 16:55:29.404805 shinywidgets-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-03-01 16:55:02.000000 shinywidgets-0.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-03-01 16:55:29.404805 shinywidgets-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-01 16:55:02.000000 shinywidgets-0.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 16:55:29.392805 shinywidgets-0.3.1/shinywidgets/
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-03-01 16:55:02.000000 shinywidgets-0.3.1/shinywidgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2994 2024-03-01 16:55:02.000000 shinywidgets-0.3.1/shinywidgets/_as_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-03-01 16:55:02.000000 shinywidgets-0.3.1/shinywidgets/_cdn.py
--rw-r--r--   0 runner    (1001) docker     (127)     7092 2024-03-01 16:55:02.000000 shinywidgets-0.3.1/shinywidgets/_comm.py
--rw-r--r--   0 runner    (1001) docker     (127)     8319 2024-03-01 16:55:02.000000 shinywidgets-0.3.1/shinywidgets/_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-03-01 16:55:02.000000 shinywidgets-0.3.1/shinywidgets/_output_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-03-01 16:55:02.000000 shinywidgets-0.3.1/shinywidgets/_render_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)     7480 2024-03-01 16:55:02.000000 shinywidgets-0.3.1/shinywidgets/_render_widget_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-03-01 16:55:02.000000 shinywidgets-0.3.1/shinywidgets/_serialization.py
--rw-r--r--   0 runner    (1001) docker     (127)     9285 2024-03-01 16:55:02.000000 shinywidgets-0.3.1/shinywidgets/_shinywidgets.py
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-03-01 16:55:02.000000 shinywidgets-0.3.1/shinywidgets/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 16:55:29.400805 shinywidgets-0.3.1/shinywidgets/static/
--rw-r--r--   0 runner    (1001) docker     (127)   165548 2024-03-01 16:55:02.000000 shinywidgets-0.3.1/shinywidgets/static/1e59d2330b4c6deb84b340635ed36249.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    77160 2024-03-01 16:55:02.000000 shinywidgets-0.3.1/shinywidgets/static/20fd1704ea223900efa9fd4e869efb08.woff2
--rw-r--r--   0 runner    (1001) docker     (127)   165742 2024-03-01 16:55:02.000000 shinywidgets-0.3.1/shinywidgets/static/8b43027f47b20503057dfbbaa9401fef.eot
--rw-r--r--   0 runner    (1001) docker     (127)   444379 2024-03-01 16:55:02.000000 shinywidgets-0.3.1/shinywidgets/static/c1e38fd9e0e74ba58f7a2b77ef29fdd3.svg
--rw-r--r--   0 runner    (1001) docker     (127)    98024 2024-03-01 16:55:02.000000 shinywidgets-0.3.1/shinywidgets/static/f691f37e57f04c152e2315ab7dbad881.woff
--rw-r--r--   0 runner    (1001) docker     (127)  3866031 2024-03-01 16:55:02.000000 shinywidgets-0.3.1/shinywidgets/static/libembed-amd.js
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-01 16:55:02.000000 shinywidgets-0.3.1/shinywidgets/static/node_modules_codemirror_mode_sync_recursive_js_.output.js
--rw-r--r--   0 runner    (1001) docker     (127)    23805 2024-03-01 16:55:02.000000 shinywidgets-0.3.1/shinywidgets/static/output.js
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-03-01 16:55:02.000000 shinywidgets-0.3.1/shinywidgets/static/shinywidgets.css
--rw-r--r--   0 runner    (1001) docker     (127)  1006878 2024-03-01 16:55:02.000000 shinywidgets-0.3.1/shinywidgets/static/vendors-node_modules_codemirror_mode_apl_apl_js-node_modules_codemirror_mode_asciiarmor_ascii-26282f.output.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 16:55:29.396805 shinywidgets-0.3.1/shinywidgets.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-03-01 16:55:28.000000 shinywidgets-0.3.1/shinywidgets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-03-01 16:55:29.000000 shinywidgets-0.3.1/shinywidgets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-01 16:55:28.000000 shinywidgets-0.3.1/shinywidgets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-01 16:55:28.000000 shinywidgets-0.3.1/shinywidgets.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-03-01 16:55:28.000000 shinywidgets-0.3.1/shinywidgets.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-01 16:55:28.000000 shinywidgets-0.3.1/shinywidgets.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:18:42.480912 shinywidgets-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-16 15:18:18.000000 shinywidgets-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-16 15:18:18.000000 shinywidgets-0.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-04-16 15:18:42.484912 shinywidgets-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-16 15:18:18.000000 shinywidgets-0.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-04-16 15:18:42.484912 shinywidgets-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 15:18:18.000000 shinywidgets-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:18:42.472911 shinywidgets-0.3.2/shinywidgets/
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-16 15:18:18.000000 shinywidgets-0.3.2/shinywidgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2994 2024-04-16 15:18:18.000000 shinywidgets-0.3.2/shinywidgets/_as_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-04-16 15:18:18.000000 shinywidgets-0.3.2/shinywidgets/_cdn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7092 2024-04-16 15:18:18.000000 shinywidgets-0.3.2/shinywidgets/_comm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8319 2024-04-16 15:18:18.000000 shinywidgets-0.3.2/shinywidgets/_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-04-16 15:18:18.000000 shinywidgets-0.3.2/shinywidgets/_output_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-04-16 15:18:18.000000 shinywidgets-0.3.2/shinywidgets/_render_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7537 2024-04-16 15:18:18.000000 shinywidgets-0.3.2/shinywidgets/_render_widget_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-04-16 15:18:18.000000 shinywidgets-0.3.2/shinywidgets/_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9285 2024-04-16 15:18:18.000000 shinywidgets-0.3.2/shinywidgets/_shinywidgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-16 15:18:18.000000 shinywidgets-0.3.2/shinywidgets/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:18:42.480912 shinywidgets-0.3.2/shinywidgets/static/
+-rw-r--r--   0 runner    (1001) docker     (127)   165548 2024-04-16 15:18:18.000000 shinywidgets-0.3.2/shinywidgets/static/1e59d2330b4c6deb84b340635ed36249.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    77160 2024-04-16 15:18:18.000000 shinywidgets-0.3.2/shinywidgets/static/20fd1704ea223900efa9fd4e869efb08.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)   165742 2024-04-16 15:18:18.000000 shinywidgets-0.3.2/shinywidgets/static/8b43027f47b20503057dfbbaa9401fef.eot
+-rw-r--r--   0 runner    (1001) docker     (127)   444379 2024-04-16 15:18:18.000000 shinywidgets-0.3.2/shinywidgets/static/c1e38fd9e0e74ba58f7a2b77ef29fdd3.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    98024 2024-04-16 15:18:18.000000 shinywidgets-0.3.2/shinywidgets/static/f691f37e57f04c152e2315ab7dbad881.woff
+-rw-r--r--   0 runner    (1001) docker     (127)  3866031 2024-04-16 15:18:18.000000 shinywidgets-0.3.2/shinywidgets/static/libembed-amd.js
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-16 15:18:18.000000 shinywidgets-0.3.2/shinywidgets/static/node_modules_codemirror_mode_sync_recursive_js_.output.js
+-rw-r--r--   0 runner    (1001) docker     (127)    23908 2024-04-16 15:18:18.000000 shinywidgets-0.3.2/shinywidgets/static/output.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-04-16 15:18:18.000000 shinywidgets-0.3.2/shinywidgets/static/shinywidgets.css
+-rw-r--r--   0 runner    (1001) docker     (127)  1006878 2024-04-16 15:18:18.000000 shinywidgets-0.3.2/shinywidgets/static/vendors-node_modules_codemirror_mode_apl_apl_js-node_modules_codemirror_mode_asciiarmor_ascii-26282f.output.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:18:42.472911 shinywidgets-0.3.2/shinywidgets.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-04-16 15:18:42.000000 shinywidgets-0.3.2/shinywidgets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-04-16 15:18:42.000000 shinywidgets-0.3.2/shinywidgets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 15:18:42.000000 shinywidgets-0.3.2/shinywidgets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 15:18:42.000000 shinywidgets-0.3.2/shinywidgets.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-16 15:18:42.000000 shinywidgets-0.3.2/shinywidgets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-16 15:18:42.000000 shinywidgets-0.3.2/shinywidgets.egg-info/top_level.txt
```

### Comparing `shinywidgets-0.3.1/LICENSE` & `shinywidgets-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `shinywidgets-0.3.1/PKG-INFO` & `shinywidgets-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shinywidgets
-Version: 0.3.1
+Version: 0.3.2
 Summary: Render ipywidgets in Shiny applications
 Home-page: https://github.com/rstudio/py-shinywidgets
 Author: Carson Sievert
 Author-email: carson@rstudio.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/rstudio/py-shinywidgets/issues
 Project-URL: Documentation, https://github.com/rstudio/py-shinywidgets/
```

### Comparing `shinywidgets-0.3.1/setup.cfg` & `shinywidgets-0.3.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `shinywidgets-0.3.1/shinywidgets/__init__.py` & `shinywidgets-0.3.2/shinywidgets/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Top-level package for shinywidgets."""
 
 __author__ = """Carson Sievert"""
 __email__ = "carson@posit.co"
-__version__ = "0.3.1"
+__version__ = "0.3.2"
 
 from ._as_widget import as_widget
 from ._dependencies import bokeh_dependency
 from ._output_widget import output_widget
 from ._render_widget import (
     render_altair,
     render_bokeh,
```

### Comparing `shinywidgets-0.3.1/shinywidgets/_as_widget.py` & `shinywidgets-0.3.2/shinywidgets/_as_widget.py`

 * *Files identical despite different names*

### Comparing `shinywidgets-0.3.1/shinywidgets/_cdn.py` & `shinywidgets-0.3.2/shinywidgets/_cdn.py`

 * *Files identical despite different names*

### Comparing `shinywidgets-0.3.1/shinywidgets/_comm.py` & `shinywidgets-0.3.2/shinywidgets/_comm.py`

 * *Files identical despite different names*

### Comparing `shinywidgets-0.3.1/shinywidgets/_dependencies.py` & `shinywidgets-0.3.2/shinywidgets/_dependencies.py`

 * *Files identical despite different names*

### Comparing `shinywidgets-0.3.1/shinywidgets/_output_widget.py` & `shinywidgets-0.3.2/shinywidgets/_output_widget.py`

 * *Files identical despite different names*

### Comparing `shinywidgets-0.3.1/shinywidgets/_render_widget.py` & `shinywidgets-0.3.2/shinywidgets/_render_widget.py`

 * *Files identical despite different names*

### Comparing `shinywidgets-0.3.1/shinywidgets/_render_widget_base.py` & `shinywidgets-0.3.2/shinywidgets/_render_widget_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -206,14 +206,14 @@
                 warnings.warn(
                     "Consider using shiny.ui.layout_column_wrap() instead of alt.concat() "
                     "for multi-column layout (the latter doesn't support filling layout).",
                     stacklevel=2,
                 )
             else:
                 UndefinedType = alt.utils.schemapi.UndefinedType  # type: ignore
-                if isinstance(chart.width, UndefinedType):  # type: ignore[reportMissingTypeStubs]
+                if hasattr(chart, "width") and isinstance(chart.width, UndefinedType):  # type: ignore[reportMissingTypeStubs]
                     chart = chart.properties(width="container")  # type: ignore
-                if isinstance(chart.height, UndefinedType):  # type: ignore[reportMissingTypeStubs]
+                if hasattr(chart, "height") and isinstance(chart.height, UndefinedType):  # type: ignore[reportMissingTypeStubs]
                     chart = chart.properties(height="container")  # type: ignore
             widget.chart = chart
 
     return (widget, fill)
```

### Comparing `shinywidgets-0.3.1/shinywidgets/_serialization.py` & `shinywidgets-0.3.2/shinywidgets/_serialization.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import decimal
 import json
 import numbers
 import warnings
 from binascii import b2a_base64
 from datetime import datetime
 from typing import Iterable
 
@@ -40,14 +41,17 @@
 
     if isinstance(obj, numbers.Integral):
         return int(obj)
 
     if isinstance(obj, numbers.Real):
         return float(obj)
 
+    if isinstance(obj, decimal.Decimal):
+        return float(obj)
+
     raise TypeError("%r is not JSON serializable" % obj)
 
 
 def _ensure_tzinfo(dt: datetime) -> datetime:
     """Ensure a datetime object has tzinfo (if none is present, add it)"""
     if not dt.tzinfo:
         # No more naïve datetime objects!
```

### Comparing `shinywidgets-0.3.1/shinywidgets/_shinywidgets.py` & `shinywidgets-0.3.2/shinywidgets/_shinywidgets.py`

 * *Files identical despite different names*

### Comparing `shinywidgets-0.3.1/shinywidgets/_utils.py` & `shinywidgets-0.3.2/shinywidgets/_utils.py`

 * *Files identical despite different names*

### Comparing `shinywidgets-0.3.1/shinywidgets/static/1e59d2330b4c6deb84b340635ed36249.ttf` & `shinywidgets-0.3.2/shinywidgets/static/1e59d2330b4c6deb84b340635ed36249.ttf`

 * *Files identical despite different names*

### Comparing `shinywidgets-0.3.1/shinywidgets/static/20fd1704ea223900efa9fd4e869efb08.woff2` & `shinywidgets-0.3.2/shinywidgets/static/20fd1704ea223900efa9fd4e869efb08.woff2`

 * *Files identical despite different names*

### Comparing `shinywidgets-0.3.1/shinywidgets/static/8b43027f47b20503057dfbbaa9401fef.eot` & `shinywidgets-0.3.2/shinywidgets/static/8b43027f47b20503057dfbbaa9401fef.eot`

 * *Files identical despite different names*

### Comparing `shinywidgets-0.3.1/shinywidgets/static/c1e38fd9e0e74ba58f7a2b77ef29fdd3.svg` & `shinywidgets-0.3.2/shinywidgets/static/c1e38fd9e0e74ba58f7a2b77ef29fdd3.svg`

 * *Files identical despite different names*

### Comparing `shinywidgets-0.3.1/shinywidgets/static/f691f37e57f04c152e2315ab7dbad881.woff` & `shinywidgets-0.3.2/shinywidgets/static/f691f37e57f04c152e2315ab7dbad881.woff`

 * *Files identical despite different names*

### Comparing `shinywidgets-0.3.1/shinywidgets/static/libembed-amd.js` & `shinywidgets-0.3.2/shinywidgets/static/libembed-amd.js`

 * *Files identical despite different names*

### Comparing `shinywidgets-0.3.1/shinywidgets/static/node_modules_codemirror_mode_sync_recursive_js_.output.js` & `shinywidgets-0.3.2/shinywidgets/static/node_modules_codemirror_mode_sync_recursive_js_.output.js`

 * *Files identical despite different names*

### Comparing `shinywidgets-0.3.1/shinywidgets/static/output.js` & `shinywidgets-0.3.2/shinywidgets/static/output.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -43,15 +43,15 @@
             "./src/output.ts":
                 /*!***********************!*\
                   !*** ./src/output.ts ***!
                   \***********************/
                 /***/
                 ((__unused_webpack_module, __webpack_exports__, __webpack_require__) => {
 
-                    eval("__webpack_require__.r(__webpack_exports__);\n/* harmony import */ var _jupyter_widgets_html_manager__WEBPACK_IMPORTED_MODULE_0__ = __webpack_require__(/*! @jupyter-widgets/html-manager */ \"@jupyter-widgets/html-manager\");\n/* harmony import */ var _jupyter_widgets_html_manager__WEBPACK_IMPORTED_MODULE_0___default = /*#__PURE__*/__webpack_require__.n(_jupyter_widgets_html_manager__WEBPACK_IMPORTED_MODULE_0__);\n/* harmony import */ var _comm__WEBPACK_IMPORTED_MODULE_1__ = __webpack_require__(/*! ./comm */ \"./src/comm.ts\");\n/* harmony import */ var _utils__WEBPACK_IMPORTED_MODULE_2__ = __webpack_require__(/*! ./utils */ \"./src/utils.ts\");\nvar _a;\n\n\n\n/******************************************************************************\n * Define a custom HTMLManager for use with Shiny\n ******************************************************************************/\nclass OutputManager extends _jupyter_widgets_html_manager__WEBPACK_IMPORTED_MODULE_0__.HTMLManager {\n    // In a soon-to-be-released version of @jupyter-widgets/html-manager,\n    // display_view()'s first \"dummy\" argument will be removed... this shim simply\n    // makes it so that our manager can work with either version\n    // https://github.com/jupyter-widgets/ipywidgets/commit/159bbe4#diff-45c126b24c3c43d2cee5313364805c025e911c4721d45ff8a68356a215bfb6c8R42-R43\n    async display_view(view, options) {\n        const n_args = super.display_view.length;\n        if (n_args === 3) {\n            return super.display_view({}, view, options);\n        }\n        else {\n            // @ts-ignore\n            return super.display_view(view, options);\n        }\n    }\n}\n// Define our own custom module loader for Shiny\nconst shinyRequireLoader = async function (moduleName, moduleVersion) {\n    // shiny provides require.js and also sets `define.amd=false` to prevent <script>s\n    // with UMD loaders from triggering anonymous define() errors. shinywidgets should\n    // generally be able to avoid anonymous define errors though since there should only\n    // be one 'main' anonymous define() for the widget's module (located in a JS file that\n    // we've already require.config({paths: {...}})ed; and in that case, requirejs adds a\n    // data-requiremodule attribute to the <script> tag that shiny's custom define will\n    // recognize and use as the name).)\n    const oldAmd = window.define.amd;\n    // The is the original value for define.amd that require.js sets\n    window.define.amd = { jQuery: true };\n    // Store jQuery global since loading we load a module, it may overwrite it\n    // (qgrid is one good example)\n    const old$ = window.$;\n    const oldJQ = window.jQuery;\n    if (moduleName === 'qgrid') {\n        // qgrid wants to use base/js/dialog (if it's available) for full-screen tables\n        // https://github.com/quantopian/qgrid/blob/877b420/js/src/qgrid.widget.js#L11-L16\n        // Maybe that's worth supporting someday, but for now, we define it to be nothing\n        // to avoid require('qgrid') from producing an error\n        window.define(\"base/js/dialog\", [], function () { return null; });\n    }\n    return (0,_jupyter_widgets_html_manager__WEBPACK_IMPORTED_MODULE_0__.requireLoader)(moduleName, moduleVersion).finally(() => {\n        window.define.amd = oldAmd;\n        window.$ = old$;\n        window.jQuery = oldJQ;\n    });\n};\nconst manager = new OutputManager({ loader: shinyRequireLoader });\n/******************************************************************************\n* Define the Shiny binding\n******************************************************************************/\n// Ideally we'd extend Shiny's HTMLOutputBinding, but the implementation isn't exported\nclass IPyWidgetOutput extends Shiny.OutputBinding {\n    find(scope) {\n        return $(scope).find(\".shiny-ipywidget-output\");\n    }\n    onValueError(el, err) {\n        Shiny.unbindAll(el);\n        this.renderError(el, err);\n    }\n    async renderValue(el, data) {\n        // Allow for a None/null value to hide the widget (css inspired by htmlwidgets)\n        if (!data) {\n            el.style.visibility = \"hidden\";\n            return;\n        }\n        else {\n            el.style.visibility = \"inherit\";\n        }\n        // Only forward the potential to fill if `output_widget(fillable=True)`\n        // _and_ the widget instance wants to fill\n        const fill = data.fill && el.classList.contains(\"html-fill-container\");\n        if (fill)\n            el.classList.add(\"forward-fill-potential\");\n        // At this time point, we should've already handled an 'open' message, and so\n        // the model should be ready to use\n        const model = await manager.get_model(data.model_id);\n        if (!model) {\n            throw new Error(`No model found for id ${data.model_id}`);\n        }\n        const view = await manager.create_view(model, {});\n        await manager.display_view(view, { el: el });\n        // Don't allow more than one .lmWidget container, which can happen\n        // when the view is displayed more than once\n        // TODO: It's probably better to get view(s) from m.views and .remove() them\n        while (el.childNodes.length > 1) {\n            el.removeChild(el.childNodes[0]);\n        }\n        // The ipywidgets container (.lmWidget)\n        const lmWidget = el.children[0];\n        this._maybeResize(lmWidget);\n    }\n    _maybeResize(lmWidget) {\n        const impl = lmWidget.children[0];\n        if (impl.children.length > 0) {\n            return this._doResize(impl);\n        }\n        // Some widget implementation (e.g., ipyleaflet, pydeck) won't actually\n        // have rendered to the DOM at this point, so wait until they do\n        const mo = new MutationObserver((mutations) => {\n            if (impl.children.length > 0) {\n                mo.disconnect();\n                this._doResize(impl);\n            }\n        });\n        mo.observe(impl, { childList: true });\n    }\n    _doResize(impl) {\n        // Trigger resize event to force layout (setTimeout() is needed for altair)\n        // TODO: debounce this call?\n        setTimeout(() => {\n            window.dispatchEvent(new Event('resize'));\n        }, 0);\n    }\n}\nShiny.outputBindings.register(new IPyWidgetOutput(), \"shiny.IPyWidgetOutput\");\n// Due to the way HTMLManager (and widget implementations) get loaded (via\n// require.js), the binding registration above can happen _after_ Shiny has\n// already bound the DOM, especially in the dynamic UI case (i.e., output_binding()'s\n// dependencies don't come in until after initial page load). And, in the dynamic UI\n// case, UI is rendered asychronously via Shiny.shinyapp.taskQueue, so if it exists,\n// we probably need to re-bind the DOM after the taskQueue is done.\nconst taskQueue = (_a = Shiny === null || Shiny === void 0 ? void 0 : Shiny.shinyapp) === null || _a === void 0 ? void 0 : _a.taskQueue;\nif (taskQueue) {\n    taskQueue.enqueue(() => Shiny.bindAll(document.body));\n}\n/******************************************************************************\n* Handle messages from the server-side Widget\n******************************************************************************/\n// Initialize the comm and model when a new widget is created\n// This is basically our version of https://github.com/jupyterlab/jupyterlab/blob/d33de15/packages/services/src/kernel/default.ts#L1144-L1176\nShiny.addCustomMessageHandler(\"shinywidgets_comm_open\", (msg_txt) => {\n    setBaseURL();\n    const msg = (0,_utils__WEBPACK_IMPORTED_MODULE_2__.jsonParse)(msg_txt);\n    Shiny.renderDependencies(msg.content.html_deps);\n    const comm = new _comm__WEBPACK_IMPORTED_MODULE_1__.ShinyComm(msg.content.comm_id);\n    manager.handle_comm_open(comm, msg);\n});\n// Handle any mutation of the model (e.g., add a marker to a map, without a full redraw)\n// Basically out version of https://github.com/jupyterlab/jupyterlab/blob/d33de15/packages/services/src/kernel/default.ts#L1200-L1215\nShiny.addCustomMessageHandler(\"shinywidgets_comm_msg\", (msg_txt) => {\n    const msg = (0,_utils__WEBPACK_IMPORTED_MODULE_2__.jsonParse)(msg_txt);\n    manager.get_model(msg.content.comm_id).then(m => {\n        // @ts-ignore for some reason IClassicComm doesn't have this method, but we do\n        m.comm.handle_msg(msg);\n    });\n});\n// TODO: test that this actually works\nShiny.addCustomMessageHandler(\"shinywidgets_comm_close\", (msg_txt) => {\n    const msg = (0,_utils__WEBPACK_IMPORTED_MODULE_2__.jsonParse)(msg_txt);\n    manager.get_model(msg.content.comm_id).then(m => {\n        // @ts-ignore for some reason IClassicComm doesn't have this method, but we do\n        m.comm.handle_close(msg);\n    });\n});\n// Our version of https://github.com/jupyter-widgets/widget-cookiecutter/blob/9694718/%7B%7Bcookiecutter.github_project_name%7D%7D/js/lib/extension.js#L8\nfunction setBaseURL(x = '') {\n    const base_url = document.querySelector('body').getAttribute('data-base-url');\n    if (!base_url) {\n        document.querySelector('body').setAttribute('data-base-url', x);\n    }\n}\n\n\n//# sourceURL=webpack://@jupyter-widgets/shiny-embed-manager/./src/output.ts?");
+                    eval("__webpack_require__.r(__webpack_exports__);\n/* harmony import */ var _jupyter_widgets_html_manager__WEBPACK_IMPORTED_MODULE_0__ = __webpack_require__(/*! @jupyter-widgets/html-manager */ \"@jupyter-widgets/html-manager\");\n/* harmony import */ var _jupyter_widgets_html_manager__WEBPACK_IMPORTED_MODULE_0___default = /*#__PURE__*/__webpack_require__.n(_jupyter_widgets_html_manager__WEBPACK_IMPORTED_MODULE_0__);\n/* harmony import */ var _comm__WEBPACK_IMPORTED_MODULE_1__ = __webpack_require__(/*! ./comm */ \"./src/comm.ts\");\n/* harmony import */ var _utils__WEBPACK_IMPORTED_MODULE_2__ = __webpack_require__(/*! ./utils */ \"./src/utils.ts\");\nvar _a;\n\n\n\n/******************************************************************************\n * Define a custom HTMLManager for use with Shiny\n ******************************************************************************/\nclass OutputManager extends _jupyter_widgets_html_manager__WEBPACK_IMPORTED_MODULE_0__.HTMLManager {\n    // In a soon-to-be-released version of @jupyter-widgets/html-manager,\n    // display_view()'s first \"dummy\" argument will be removed... this shim simply\n    // makes it so that our manager can work with either version\n    // https://github.com/jupyter-widgets/ipywidgets/commit/159bbe4#diff-45c126b24c3c43d2cee5313364805c025e911c4721d45ff8a68356a215bfb6c8R42-R43\n    async display_view(view, options) {\n        const n_args = super.display_view.length;\n        if (n_args === 3) {\n            return super.display_view({}, view, options);\n        }\n        else {\n            // @ts-ignore\n            return super.display_view(view, options);\n        }\n    }\n}\n// Define our own custom module loader for Shiny\nconst shinyRequireLoader = async function (moduleName, moduleVersion) {\n    // shiny provides require.js and also sets `define.amd=false` to prevent <script>s\n    // with UMD loaders from triggering anonymous define() errors. shinywidgets should\n    // generally be able to avoid anonymous define errors though since there should only\n    // be one 'main' anonymous define() for the widget's module (located in a JS file that\n    // we've already require.config({paths: {...}})ed; and in that case, requirejs adds a\n    // data-requiremodule attribute to the <script> tag that shiny's custom define will\n    // recognize and use as the name).)\n    const oldAmd = window.define.amd;\n    // The is the original value for define.amd that require.js sets\n    window.define.amd = { jQuery: true };\n    // Store jQuery global since loading we load a module, it may overwrite it\n    // (qgrid is one good example)\n    const old$ = window.$;\n    const oldJQ = window.jQuery;\n    if (moduleName === 'qgrid') {\n        // qgrid wants to use base/js/dialog (if it's available) for full-screen tables\n        // https://github.com/quantopian/qgrid/blob/877b420/js/src/qgrid.widget.js#L11-L16\n        // Maybe that's worth supporting someday, but for now, we define it to be nothing\n        // to avoid require('qgrid') from producing an error\n        window.define(\"base/js/dialog\", [], function () { return null; });\n    }\n    return (0,_jupyter_widgets_html_manager__WEBPACK_IMPORTED_MODULE_0__.requireLoader)(moduleName, moduleVersion).finally(() => {\n        window.define.amd = oldAmd;\n        window.$ = old$;\n        window.jQuery = oldJQ;\n    });\n};\nconst manager = new OutputManager({ loader: shinyRequireLoader });\n/******************************************************************************\n* Define the Shiny binding\n******************************************************************************/\n// Ideally we'd extend Shiny's HTMLOutputBinding, but the implementation isn't exported\nclass IPyWidgetOutput extends Shiny.OutputBinding {\n    find(scope) {\n        return $(scope).find(\".shiny-ipywidget-output\");\n    }\n    onValueError(el, err) {\n        Shiny.unbindAll(el);\n        this.renderError(el, err);\n    }\n    async renderValue(el, data) {\n        // Allow for a None/null value to hide the widget (css inspired by htmlwidgets)\n        if (!data) {\n            el.style.visibility = \"hidden\";\n            return;\n        }\n        else {\n            el.style.visibility = \"inherit\";\n        }\n        // Only forward the potential to fill if `output_widget(fillable=True)`\n        // _and_ the widget instance wants to fill\n        const fill = data.fill && el.classList.contains(\"html-fill-container\");\n        if (fill)\n            el.classList.add(\"forward-fill-potential\");\n        // At this time point, we should've already handled an 'open' message, and so\n        // the model should be ready to use\n        const model = await manager.get_model(data.model_id);\n        if (!model) {\n            throw new Error(`No model found for id ${data.model_id}`);\n        }\n        const view = await manager.create_view(model, {});\n        await manager.display_view(view, { el: el });\n        // Don't allow more than one .lmWidget container, which can happen\n        // when the view is displayed more than once\n        // TODO: It's probably better to get view(s) from m.views and .remove() them\n        while (el.childNodes.length > 1) {\n            el.removeChild(el.childNodes[0]);\n        }\n        // The ipywidgets container (.lmWidget)\n        const lmWidget = el.children[0];\n        this._maybeResize(lmWidget);\n    }\n    _maybeResize(lmWidget) {\n        if (this._hasImplementation(lmWidget)) {\n            return this._doResize();\n        }\n        // Some widget implementation (e.g., ipyleaflet, pydeck) won't actually\n        // have rendered to the DOM at this point, so wait until they do\n        const mo = new MutationObserver((mutations) => {\n            if (this._hasImplementation(lmWidget)) {\n                mo.disconnect();\n                this._doResize();\n            }\n        });\n        mo.observe(lmWidget, { childList: true });\n    }\n    _doResize() {\n        // Trigger resize event to force layout (setTimeout() is needed for altair)\n        // TODO: debounce this call?\n        setTimeout(() => {\n            window.dispatchEvent(new Event('resize'));\n        }, 0);\n    }\n    _hasImplementation(lmWidget) {\n        const impl = lmWidget.children[0];\n        return impl && impl.children.length > 0;\n    }\n}\nShiny.outputBindings.register(new IPyWidgetOutput(), \"shiny.IPyWidgetOutput\");\n// Due to the way HTMLManager (and widget implementations) get loaded (via\n// require.js), the binding registration above can happen _after_ Shiny has\n// already bound the DOM, especially in the dynamic UI case (i.e., output_binding()'s\n// dependencies don't come in until after initial page load). And, in the dynamic UI\n// case, UI is rendered asychronously via Shiny.shinyapp.taskQueue, so if it exists,\n// we probably need to re-bind the DOM after the taskQueue is done.\nconst taskQueue = (_a = Shiny === null || Shiny === void 0 ? void 0 : Shiny.shinyapp) === null || _a === void 0 ? void 0 : _a.taskQueue;\nif (taskQueue) {\n    taskQueue.enqueue(() => Shiny.bindAll(document.body));\n}\n/******************************************************************************\n* Handle messages from the server-side Widget\n******************************************************************************/\n// Initialize the comm and model when a new widget is created\n// This is basically our version of https://github.com/jupyterlab/jupyterlab/blob/d33de15/packages/services/src/kernel/default.ts#L1144-L1176\nShiny.addCustomMessageHandler(\"shinywidgets_comm_open\", (msg_txt) => {\n    setBaseURL();\n    const msg = (0,_utils__WEBPACK_IMPORTED_MODULE_2__.jsonParse)(msg_txt);\n    Shiny.renderDependencies(msg.content.html_deps);\n    const comm = new _comm__WEBPACK_IMPORTED_MODULE_1__.ShinyComm(msg.content.comm_id);\n    manager.handle_comm_open(comm, msg);\n});\n// Handle any mutation of the model (e.g., add a marker to a map, without a full redraw)\n// Basically out version of https://github.com/jupyterlab/jupyterlab/blob/d33de15/packages/services/src/kernel/default.ts#L1200-L1215\nShiny.addCustomMessageHandler(\"shinywidgets_comm_msg\", (msg_txt) => {\n    const msg = (0,_utils__WEBPACK_IMPORTED_MODULE_2__.jsonParse)(msg_txt);\n    manager.get_model(msg.content.comm_id).then(m => {\n        // @ts-ignore for some reason IClassicComm doesn't have this method, but we do\n        m.comm.handle_msg(msg);\n    });\n});\n// TODO: test that this actually works\nShiny.addCustomMessageHandler(\"shinywidgets_comm_close\", (msg_txt) => {\n    const msg = (0,_utils__WEBPACK_IMPORTED_MODULE_2__.jsonParse)(msg_txt);\n    manager.get_model(msg.content.comm_id).then(m => {\n        // @ts-ignore for some reason IClassicComm doesn't have this method, but we do\n        m.comm.handle_close(msg);\n    });\n});\n// Our version of https://github.com/jupyter-widgets/widget-cookiecutter/blob/9694718/%7B%7Bcookiecutter.github_project_name%7D%7D/js/lib/extension.js#L8\nfunction setBaseURL(x = '') {\n    const base_url = document.querySelector('body').getAttribute('data-base-url');\n    if (!base_url) {\n        document.querySelector('body').setAttribute('data-base-url', x);\n    }\n}\n\n\n//# sourceURL=webpack://@jupyter-widgets/shiny-embed-manager/./src/output.ts?");
 
                     /***/
                 }),
 
             /***/
             "./src/utils.ts":
                 /*!**********************!*\
```

### Comparing `shinywidgets-0.3.1/shinywidgets/static/vendors-node_modules_codemirror_mode_apl_apl_js-node_modules_codemirror_mode_asciiarmor_ascii-26282f.output.js` & `shinywidgets-0.3.2/shinywidgets/static/vendors-node_modules_codemirror_mode_apl_apl_js-node_modules_codemirror_mode_asciiarmor_ascii-26282f.output.js`

 * *Files identical despite different names*

### Comparing `shinywidgets-0.3.1/shinywidgets.egg-info/PKG-INFO` & `shinywidgets-0.3.2/shinywidgets.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shinywidgets
-Version: 0.3.1
+Version: 0.3.2
 Summary: Render ipywidgets in Shiny applications
 Home-page: https://github.com/rstudio/py-shinywidgets
 Author: Carson Sievert
 Author-email: carson@rstudio.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/rstudio/py-shinywidgets/issues
 Project-URL: Documentation, https://github.com/rstudio/py-shinywidgets/
```

### Comparing `shinywidgets-0.3.1/shinywidgets.egg-info/SOURCES.txt` & `shinywidgets-0.3.2/shinywidgets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

