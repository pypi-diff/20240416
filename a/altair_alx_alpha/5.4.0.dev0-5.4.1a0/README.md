# Comparing `tmp/altair_alx_alpha-5.4.0.dev0.tar.gz` & `tmp/altair_alx_alpha-5.4.1a0.tar.gz`

## Comparing `altair_alx_alpha-5.4.0.dev0.tar` & `altair_alx_alpha-5.4.1a0.tar`

### file list

```diff
@@ -1,53 +1,52 @@
--rw-r--r--   0        0        0    14641 2020-02-02 00:00:00.000000 altair_alx_alpha-5.4.0.dev0/altair/__init__.py
--rw-r--r--   0        0        0     2996 2020-02-02 00:00:00.000000 altair_alx_alpha-5.4.0.dev0/altair/_magics.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 altair_alx_alpha-5.4.0.dev0/altair/py.typed
--rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 altair_alx_alpha-5.4.0.dev0/altair/expr/__init__.py
--rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 altair_alx_alpha-5.4.0.dev0/altair/expr/consts.py
--rw-r--r--   0        0        0     6848 2020-02-02 00:00:00.000000 altair_alx_alpha-5.4.0.dev0/altair/expr/core.py
--rw-r--r--   0        0        0    34418 2020-02-02 00:00:00.000000 altair_alx_alpha-5.4.0.dev0/altair/expr/funcs.py
--rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 altair_alx_alpha-5.4.0.dev0/altair/jupyter/__init__.py
--rw-r--r--   0        0        0    15289 2020-02-02 00:00:00.000000 altair_alx_alpha-5.4.0.dev0/altair/jupyter/jupyter_chart.py
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 altair_alx_alpha-5.4.0.dev0/altair/jupyter/js/README.md
--rw-r--r--   0        0        0     7936 2020-02-02 00:00:00.000000 altair_alx_alpha-5.4.0.dev0/altair/jupyter/js/index.js
--rw-r--r--   0        0        0    11356 2020-02-02 00:00:00.000000 altair_alx_alpha-5.4.0.dev0/altair/sphinxext/altairplot.py
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 altair_alx_alpha-5.4.0.dev0/altair/utils/__init__.py
--rw-r--r--   0        0        0     6503 2020-02-02 00:00:00.000000 altair_alx_alpha-5.4.0.dev0/altair/utils/_dfi_types.py
--rw-r--r--   0        0        0     3690 2020-02-02 00:00:00.000000 altair_alx_alpha-5.4.0.dev0/altair/utils/_importers.py
--rw-r--r--   0        0        0     2261 2020-02-02 00:00:00.000000 altair_alx_alpha-5.4.0.dev0/altair/utils/_show.py
--rw-r--r--   0        0        0    18128 2020-02-02 00:00:00.000000 altair_alx_alpha-5.4.0.dev0/altair/utils/_transformed_data.py
--rw-r--r--   0        0        0     8205 2020-02-02 00:00:00.000000 altair_alx_alpha-5.4.0.dev0/altair/utils/_vegafusion_data.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 altair_alx_alpha-5.4.0.dev0/altair/utils/compiler.py
--rw-r--r--   0        0        0    27776 2020-02-02 00:00:00.000000 altair_alx_alpha-5.4.0.dev0/altair/utils/core.py
--rw-r--r--   0        0        0    13030 2020-02-02 00:00:00.000000 altair_alx_alpha-5.4.0.dev0/altair/utils/data.py
--rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 altair_alx_alpha-5.4.0.dev0/altair/utils/deprecation.py
--rw-r--r--   0        0        0     8852 2020-02-02 00:00:00.000000 altair_alx_alpha-5.4.0.dev0/altair/utils/display.py
--rw-r--r--   0        0        0     1423 2020-02-02 00:00:00.000000 altair_alx_alpha-5.4.0.dev0/altair/utils/execeval.py
--rw-r--r--   0        0        0    10044 2020-02-02 00:00:00.000000 altair_alx_alpha-5.4.0.dev0/altair/utils/html.py
--rw-r--r--   0        0        0    12178 2020-02-02 00:00:00.000000 altair_alx_alpha-5.4.0.dev0/altair/utils/mimebundle.py
--rw-r--r--   0        0        0     7936 2020-02-02 00:00:00.000000 altair_alx_alpha-5.4.0.dev0/altair/utils/plugin_registry.py
--rw-r--r--   0        0        0     8004 2020-02-02 00:00:00.000000 altair_alx_alpha-5.4.0.dev0/altair/utils/save.py
--rw-r--r--   0        0        0    52252 2020-02-02 00:00:00.000000 altair_alx_alpha-5.4.0.dev0/altair/utils/schemapi.py
--rw-r--r--   0        0        0     4175 2020-02-02 00:00:00.000000 altair_alx_alpha-5.4.0.dev0/altair/utils/selection.py
--rw-r--r--   0        0        0     4076 2020-02-02 00:00:00.000000 altair_alx_alpha-5.4.0.dev0/altair/utils/server.py
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 altair_alx_alpha-5.4.0.dev0/altair/utils/theme.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 altair_alx_alpha-5.4.0.dev0/altair/vegalite/__init__.py
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 altair_alx_alpha-5.4.0.dev0/altair/vegalite/api.py
--rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 altair_alx_alpha-5.4.0.dev0/altair/vegalite/data.py
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 altair_alx_alpha-5.4.0.dev0/altair/vegalite/display.py
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 altair_alx_alpha-5.4.0.dev0/altair/vegalite/schema.py
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 altair_alx_alpha-5.4.0.dev0/altair/vegalite/v5/__init__.py
--rw-r--r--   0        0        0   156055 2020-02-02 00:00:00.000000 altair_alx_alpha-5.4.0.dev0/altair/vegalite/v5/api.py
--rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 altair_alx_alpha-5.4.0.dev0/altair/vegalite/v5/compiler.py
--rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 altair_alx_alpha-5.4.0.dev0/altair/vegalite/v5/data.py
--rw-r--r--   0        0        0     5659 2020-02-02 00:00:00.000000 altair_alx_alpha-5.4.0.dev0/altair/vegalite/v5/display.py
--rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 altair_alx_alpha-5.4.0.dev0/altair/vegalite/v5/theme.py
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 altair_alx_alpha-5.4.0.dev0/altair/vegalite/v5/schema/__init__.py
--rw-r--r--   0        0        0  2784087 2020-02-02 00:00:00.000000 altair_alx_alpha-5.4.0.dev0/altair/vegalite/v5/schema/channels.py
--rw-r--r--   0        0        0  2157102 2020-02-02 00:00:00.000000 altair_alx_alpha-5.4.0.dev0/altair/vegalite/v5/schema/core.py
--rw-r--r--   0        0        0   443354 2020-02-02 00:00:00.000000 altair_alx_alpha-5.4.0.dev0/altair/vegalite/v5/schema/mixins.py
--rw-r--r--   0        0        0  1817604 2020-02-02 00:00:00.000000 altair_alx_alpha-5.4.0.dev0/altair/vegalite/v5/schema/vega-lite-schema.json
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 altair_alx_alpha-5.4.0.dev0/.gitignore
--rw-r--r--   0        0        0     1497 2020-02-02 00:00:00.000000 altair_alx_alpha-5.4.0.dev0/LICENSE
--rw-r--r--   0        0        0     6696 2020-02-02 00:00:00.000000 altair_alx_alpha-5.4.0.dev0/README.md
--rw-r--r--   0        0        0     5664 2020-02-02 00:00:00.000000 altair_alx_alpha-5.4.0.dev0/pyproject.toml
--rw-r--r--   0        0        0     9176 2020-02-02 00:00:00.000000 altair_alx_alpha-5.4.0.dev0/PKG-INFO
+-rw-r--r--   0        0        0    14643 2020-02-02 00:00:00.000000 altair_alx_alpha-5.4.1a0/altair/__init__.py
+-rw-r--r--   0        0        0     2996 2020-02-02 00:00:00.000000 altair_alx_alpha-5.4.1a0/altair/_magics.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 altair_alx_alpha-5.4.1a0/altair/py.typed
+-rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 altair_alx_alpha-5.4.1a0/altair/expr/__init__.py
+-rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 altair_alx_alpha-5.4.1a0/altair/expr/consts.py
+-rw-r--r--   0        0        0     6848 2020-02-02 00:00:00.000000 altair_alx_alpha-5.4.1a0/altair/expr/core.py
+-rw-r--r--   0        0        0    34418 2020-02-02 00:00:00.000000 altair_alx_alpha-5.4.1a0/altair/expr/funcs.py
+-rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 altair_alx_alpha-5.4.1a0/altair/jupyter/__init__.py
+-rw-r--r--   0        0        0    15289 2020-02-02 00:00:00.000000 altair_alx_alpha-5.4.1a0/altair/jupyter/jupyter_chart.py
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 altair_alx_alpha-5.4.1a0/altair/jupyter/js/README.md
+-rw-r--r--   0        0        0     7936 2020-02-02 00:00:00.000000 altair_alx_alpha-5.4.1a0/altair/jupyter/js/index.js
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 altair_alx_alpha-5.4.1a0/altair/utils/__init__.py
+-rw-r--r--   0        0        0     6503 2020-02-02 00:00:00.000000 altair_alx_alpha-5.4.1a0/altair/utils/_dfi_types.py
+-rw-r--r--   0        0        0     3690 2020-02-02 00:00:00.000000 altair_alx_alpha-5.4.1a0/altair/utils/_importers.py
+-rw-r--r--   0        0        0     2261 2020-02-02 00:00:00.000000 altair_alx_alpha-5.4.1a0/altair/utils/_show.py
+-rw-r--r--   0        0        0    18128 2020-02-02 00:00:00.000000 altair_alx_alpha-5.4.1a0/altair/utils/_transformed_data.py
+-rw-r--r--   0        0        0     8205 2020-02-02 00:00:00.000000 altair_alx_alpha-5.4.1a0/altair/utils/_vegafusion_data.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 altair_alx_alpha-5.4.1a0/altair/utils/compiler.py
+-rw-r--r--   0        0        0    27770 2020-02-02 00:00:00.000000 altair_alx_alpha-5.4.1a0/altair/utils/core.py
+-rw-r--r--   0        0        0    13030 2020-02-02 00:00:00.000000 altair_alx_alpha-5.4.1a0/altair/utils/data.py
+-rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 altair_alx_alpha-5.4.1a0/altair/utils/deprecation.py
+-rw-r--r--   0        0        0     8852 2020-02-02 00:00:00.000000 altair_alx_alpha-5.4.1a0/altair/utils/display.py
+-rw-r--r--   0        0        0     1423 2020-02-02 00:00:00.000000 altair_alx_alpha-5.4.1a0/altair/utils/execeval.py
+-rw-r--r--   0        0        0    10083 2020-02-02 00:00:00.000000 altair_alx_alpha-5.4.1a0/altair/utils/html.py
+-rw-r--r--   0        0        0    12178 2020-02-02 00:00:00.000000 altair_alx_alpha-5.4.1a0/altair/utils/mimebundle.py
+-rw-r--r--   0        0        0     7936 2020-02-02 00:00:00.000000 altair_alx_alpha-5.4.1a0/altair/utils/plugin_registry.py
+-rw-r--r--   0        0        0     8004 2020-02-02 00:00:00.000000 altair_alx_alpha-5.4.1a0/altair/utils/save.py
+-rw-r--r--   0        0        0    52246 2020-02-02 00:00:00.000000 altair_alx_alpha-5.4.1a0/altair/utils/schemapi.py
+-rw-r--r--   0        0        0     4175 2020-02-02 00:00:00.000000 altair_alx_alpha-5.4.1a0/altair/utils/selection.py
+-rw-r--r--   0        0        0     4076 2020-02-02 00:00:00.000000 altair_alx_alpha-5.4.1a0/altair/utils/server.py
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 altair_alx_alpha-5.4.1a0/altair/utils/theme.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 altair_alx_alpha-5.4.1a0/altair/vegalite/__init__.py
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 altair_alx_alpha-5.4.1a0/altair/vegalite/api.py
+-rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 altair_alx_alpha-5.4.1a0/altair/vegalite/data.py
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 altair_alx_alpha-5.4.1a0/altair/vegalite/display.py
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 altair_alx_alpha-5.4.1a0/altair/vegalite/schema.py
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 altair_alx_alpha-5.4.1a0/altair/vegalite/v5/__init__.py
+-rw-r--r--   0        0        0   156055 2020-02-02 00:00:00.000000 altair_alx_alpha-5.4.1a0/altair/vegalite/v5/api.py
+-rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 altair_alx_alpha-5.4.1a0/altair/vegalite/v5/compiler.py
+-rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 altair_alx_alpha-5.4.1a0/altair/vegalite/v5/data.py
+-rw-r--r--   0        0        0     5659 2020-02-02 00:00:00.000000 altair_alx_alpha-5.4.1a0/altair/vegalite/v5/display.py
+-rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 altair_alx_alpha-5.4.1a0/altair/vegalite/v5/theme.py
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 altair_alx_alpha-5.4.1a0/altair/vegalite/v5/schema/__init__.py
+-rw-r--r--   0        0        0  2784087 2020-02-02 00:00:00.000000 altair_alx_alpha-5.4.1a0/altair/vegalite/v5/schema/channels.py
+-rw-r--r--   0        0        0  2157102 2020-02-02 00:00:00.000000 altair_alx_alpha-5.4.1a0/altair/vegalite/v5/schema/core.py
+-rw-r--r--   0        0        0   443354 2020-02-02 00:00:00.000000 altair_alx_alpha-5.4.1a0/altair/vegalite/v5/schema/mixins.py
+-rw-r--r--   0        0        0  1817604 2020-02-02 00:00:00.000000 altair_alx_alpha-5.4.1a0/altair/vegalite/v5/schema/vega-lite-schema.json
+-rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 altair_alx_alpha-5.4.1a0/.gitignore
+-rw-r--r--   0        0        0     1497 2020-02-02 00:00:00.000000 altair_alx_alpha-5.4.1a0/LICENSE
+-rw-r--r--   0        0        0     6672 2020-02-02 00:00:00.000000 altair_alx_alpha-5.4.1a0/README.md
+-rw-r--r--   0        0        0     5658 2020-02-02 00:00:00.000000 altair_alx_alpha-5.4.1a0/pyproject.toml
+-rw-r--r--   0        0        0     9143 2020-02-02 00:00:00.000000 altair_alx_alpha-5.4.1a0/PKG-INFO
```

### Comparing `altair_alx_alpha-5.4.0.dev0/altair/__init__.py` & `altair_alx_alpha-5.4.1a0/altair/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ruff: noqa
-__version__ = "5.4.0dev"
+__version__ = "5.4.1alpha"
 
 from typing import Any
 
 # Necessary as mypy would see expr as the module alt.expr although due to how
 # the imports are set up it is expr in the alt.expr module
 expr: Any
```

### Comparing `altair_alx_alpha-5.4.0.dev0/altair/_magics.py` & `altair_alx_alpha-5.4.1a0/altair/_magics.py`

 * *Files identical despite different names*

### Comparing `altair_alx_alpha-5.4.0.dev0/altair/expr/consts.py` & `altair_alx_alpha-5.4.1a0/altair/expr/consts.py`

 * *Files identical despite different names*

### Comparing `altair_alx_alpha-5.4.0.dev0/altair/expr/core.py` & `altair_alx_alpha-5.4.1a0/altair/expr/core.py`

 * *Files identical despite different names*

### Comparing `altair_alx_alpha-5.4.0.dev0/altair/expr/funcs.py` & `altair_alx_alpha-5.4.1a0/altair/expr/funcs.py`

 * *Files identical despite different names*

### Comparing `altair_alx_alpha-5.4.0.dev0/altair/jupyter/__init__.py` & `altair_alx_alpha-5.4.1a0/altair/jupyter/__init__.py`

 * *Files identical despite different names*

### Comparing `altair_alx_alpha-5.4.0.dev0/altair/jupyter/jupyter_chart.py` & `altair_alx_alpha-5.4.1a0/altair/jupyter/jupyter_chart.py`

 * *Files identical despite different names*

### Comparing `altair_alx_alpha-5.4.0.dev0/altair/jupyter/js/index.js` & `altair_alx_alpha-5.4.1a0/altair/jupyter/js/index.js`

 * *Files identical despite different names*

### Comparing `altair_alx_alpha-5.4.0.dev0/altair/utils/__init__.py` & `altair_alx_alpha-5.4.1a0/altair/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `altair_alx_alpha-5.4.0.dev0/altair/utils/_dfi_types.py` & `altair_alx_alpha-5.4.1a0/altair/utils/_dfi_types.py`

 * *Files identical despite different names*

### Comparing `altair_alx_alpha-5.4.0.dev0/altair/utils/_importers.py` & `altair_alx_alpha-5.4.1a0/altair/utils/_importers.py`

 * *Files identical despite different names*

### Comparing `altair_alx_alpha-5.4.0.dev0/altair/utils/_show.py` & `altair_alx_alpha-5.4.1a0/altair/utils/_show.py`

 * *Files identical despite different names*

### Comparing `altair_alx_alpha-5.4.0.dev0/altair/utils/_transformed_data.py` & `altair_alx_alpha-5.4.1a0/altair/utils/_transformed_data.py`

 * *Files identical despite different names*

### Comparing `altair_alx_alpha-5.4.0.dev0/altair/utils/_vegafusion_data.py` & `altair_alx_alpha-5.4.1a0/altair/utils/_vegafusion_data.py`

 * *Files identical despite different names*

### Comparing `altair_alx_alpha-5.4.0.dev0/altair/utils/core.py` & `altair_alx_alpha-5.4.1a0/altair/utils/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -367,15 +367,15 @@
             df[col_name] = col.where(col.notnull(), None)
         elif dtype_name.startswith("datetime") or dtype_name.startswith("timestamp"):
             # Convert datetimes to strings. This needs to be a full ISO string
             # with time, which is why we cannot use ``col.astype(str)``.
             # This is because Javascript parses date-only times in UTC, but
             # parses full ISO-8601 dates as local time, and dates in Vega and
             # Vega-Lite are displayed in local time by default.
-            # (see https://github.com/altair-viz/altair/issues/1027)
+            # (see https://github.com/vega/altair/issues/1027)
             df[col_name] = (
                 df[col_name].apply(lambda x: x.isoformat()).replace("NaT", "")
             )
         elif dtype_name.startswith("timedelta"):
             raise ValueError(
                 'Field "{col_name}" has type "{dtype}" which is '
                 "not supported by Altair. Please convert to "
```

### Comparing `altair_alx_alpha-5.4.0.dev0/altair/utils/data.py` & `altair_alx_alpha-5.4.1a0/altair/utils/data.py`

 * *Files identical despite different names*

### Comparing `altair_alx_alpha-5.4.0.dev0/altair/utils/deprecation.py` & `altair_alx_alpha-5.4.1a0/altair/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `altair_alx_alpha-5.4.0.dev0/altair/utils/display.py` & `altair_alx_alpha-5.4.1a0/altair/utils/display.py`

 * *Files identical despite different names*

### Comparing `altair_alx_alpha-5.4.0.dev0/altair/utils/execeval.py` & `altair_alx_alpha-5.4.1a0/altair/utils/execeval.py`

 * *Files identical despite different names*

### Comparing `altair_alx_alpha-5.4.0.dev0/altair/utils/html.py` & `altair_alx_alpha-5.4.1a0/altair/utils/html.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,15 @@
   <script>
     {%- if requirejs and not fullhtml %}
     requirejs.config({
         "paths": {
             "vega": "{{ base_url }}/vega@{{ vega_version }}?noext",
             "vega-lib": "{{ base_url }}/vega-lib?noext",
             "vega-lite": "{{ base_url }}/vega-lite@{{ vegalite_version }}?noext",
-            "vega-embed": "https://cdn.jsdelivr.net/gh/dwootton/vega-embed/build/vega-embed.min.js?noext",
+            "vega-embed": "https://cdn.jsdelivr.net/gh/dwootton/vega-embed@altair-express/build/vega-embed.min.js?noext",
         }
     });
     {% endif %}
     {% if requirejs -%}
     require(['vega-embed'],
     {%- else -%}
     (
@@ -112,15 +112,15 @@
     if (outputDiv.id !== "{{ output_div }}") {
       outputDiv = document.getElementById("{{ output_div }}");
     }
     const paths = {
       "vega": "{{ base_url }}/vega@{{ vega_version }}?noext",
       "vega-lib": "{{ base_url }}/vega-lib?noext",
       "vega-lite": "{{ base_url }}/vega-lite@{{ vegalite_version }}?noext",
-      "vega-embed": "https://raw.githack.com/dwootton/vega-embed/next/build/vega-embed.js",
+      "vega-embed": "https://cdn.jsdelivr.net/gh/dwootton/vega-embed@altair-express/build/vega-embed.min.js?noext",
     };
     console.log('new paths updated',paths);
     function maybeLoadScript(lib, version)
      
       
         {
       var key = `${lib.replace("-", "")}_version`;
```

### Comparing `altair_alx_alpha-5.4.0.dev0/altair/utils/mimebundle.py` & `altair_alx_alpha-5.4.1a0/altair/utils/mimebundle.py`

 * *Files identical despite different names*

### Comparing `altair_alx_alpha-5.4.0.dev0/altair/utils/plugin_registry.py` & `altair_alx_alpha-5.4.1a0/altair/utils/plugin_registry.py`

 * *Files identical despite different names*

### Comparing `altair_alx_alpha-5.4.0.dev0/altair/utils/save.py` & `altair_alx_alpha-5.4.1a0/altair/utils/save.py`

 * *Files identical despite different names*

### Comparing `altair_alx_alpha-5.4.0.dev0/altair/utils/schemapi.py` & `altair_alx_alpha-5.4.1a0/altair/utils/schemapi.py`

 * *Files 0% similar despite different names*

```diff
@@ -265,15 +265,15 @@
     )
 
 
 def _json_path(err: jsonschema.exceptions.ValidationError) -> str:
     """Drop in replacement for the .json_path property of the jsonschema
     ValidationError class, which is not available as property for
     ValidationError with jsonschema<4.0.1.
-    More info, see https://github.com/altair-viz/altair/issues/3038
+    More info, see https://github.com/vega/altair/issues/3038
     """
     path = "$"
     for elem in err.absolute_path:
         if isinstance(elem, int):
             path += "[" + str(elem) + "]"
         else:
             path += "." + elem
```

### Comparing `altair_alx_alpha-5.4.0.dev0/altair/utils/selection.py` & `altair_alx_alpha-5.4.1a0/altair/utils/selection.py`

 * *Files identical despite different names*

### Comparing `altair_alx_alpha-5.4.0.dev0/altair/utils/server.py` & `altair_alx_alpha-5.4.1a0/altair/utils/server.py`

 * *Files identical despite different names*

### Comparing `altair_alx_alpha-5.4.0.dev0/altair/vegalite/data.py` & `altair_alx_alpha-5.4.1a0/altair/vegalite/data.py`

 * *Files identical despite different names*

### Comparing `altair_alx_alpha-5.4.0.dev0/altair/vegalite/v5/api.py` & `altair_alx_alpha-5.4.1a0/altair/vegalite/v5/api.py`

 * *Files identical despite different names*

### Comparing `altair_alx_alpha-5.4.0.dev0/altair/vegalite/v5/compiler.py` & `altair_alx_alpha-5.4.1a0/altair/vegalite/v5/compiler.py`

 * *Files identical despite different names*

### Comparing `altair_alx_alpha-5.4.0.dev0/altair/vegalite/v5/data.py` & `altair_alx_alpha-5.4.1a0/altair/vegalite/v5/data.py`

 * *Files identical despite different names*

### Comparing `altair_alx_alpha-5.4.0.dev0/altair/vegalite/v5/display.py` & `altair_alx_alpha-5.4.1a0/altair/vegalite/v5/display.py`

 * *Files identical despite different names*

### Comparing `altair_alx_alpha-5.4.0.dev0/altair/vegalite/v5/theme.py` & `altair_alx_alpha-5.4.1a0/altair/vegalite/v5/theme.py`

 * *Files identical despite different names*

### Comparing `altair_alx_alpha-5.4.0.dev0/altair/vegalite/v5/schema/channels.py` & `altair_alx_alpha-5.4.1a0/altair/vegalite/v5/schema/channels.py`

 * *Files identical despite different names*

### Comparing `altair_alx_alpha-5.4.0.dev0/altair/vegalite/v5/schema/core.py` & `altair_alx_alpha-5.4.1a0/altair/vegalite/v5/schema/core.py`

 * *Files identical despite different names*

### Comparing `altair_alx_alpha-5.4.0.dev0/altair/vegalite/v5/schema/mixins.py` & `altair_alx_alpha-5.4.1a0/altair/vegalite/v5/schema/mixins.py`

 * *Files identical despite different names*

### Comparing `altair_alx_alpha-5.4.0.dev0/altair/vegalite/v5/schema/vega-lite-schema.json` & `altair_alx_alpha-5.4.1a0/altair/vegalite/v5/schema/vega-lite-schema.json`

 * *Files identical despite different names*

### Comparing `altair_alx_alpha-5.4.0.dev0/.gitignore` & `altair_alx_alpha-5.4.1a0/.gitignore`

 * *Files 3% similar despite different names*

```diff
@@ -8,20 +8,22 @@
 # Distribution / packaging
 .Python
 env/
 venv
 .venv
 build/
 develop-eggs/
+dist/
 downloads/
 eggs/
 .eggs/
 lib/
 lib64/
 parts/
+sdist/
 var/
 *.egg-info/
 .installed.cfg
 *.egg
 
 # PyInstaller
 #  Usually these files are written by a python script from a template
```

### Comparing `altair_alx_alpha-5.4.0.dev0/LICENSE` & `altair_alx_alpha-5.4.1a0/LICENSE`

 * *Files identical despite different names*

### Comparing `altair_alx_alpha-5.4.0.dev0/README.md` & `altair_alx_alpha-5.4.1a0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Vega-Altair <a href="https://altair-viz.github.io/"><img align="right" src="https://altair-viz.github.io/_static/altair-logo-light.png" height="50"></img></a>
 
-[![github actions](https://github.com/altair-viz/altair/workflows/build/badge.svg)](https://github.com/altair-viz/altair/actions?query=workflow%3Abuild)
+[![github actions](https://github.com/vega/altair/workflows/build/badge.svg)](https://github.com/vega/altair/actions?query=workflow%3Abuild)
 [![typedlib_mypy](https://www.mypy-lang.org/static/mypy_badge.svg)](https://www.mypy-lang.org)
 [![JOSS Paper](https://joss.theoj.org/papers/10.21105/joss.01057/status.svg)](https://joss.theoj.org/papers/10.21105/joss.01057)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/altair)](https://pypi.org/project/altair)
 
 **Vega-Altair** is a declarative statistical visualization library for Python. With Vega-Altair, you can spend more time understanding your data and its meaning. Vega-Altair's
 API is simple, friendly and consistent and built on top of the powerful
 [Vega-Lite](https://github.com/vega/vega-lite) JSON specification. This elegant
@@ -101,15 +101,15 @@
 
 For full installation instructions, please see [the documentation](https://altair-viz.github.io/getting_started/installation.html).
 
 ## Getting Help
 
 If you have a question that is not addressed in the documentation, 
 you can post it on [StackOverflow](https://stackoverflow.com/questions/tagged/altair) using the `altair` tag.
-For bugs and feature requests, please open a [Github Issue](https://github.com/altair-viz/altair/issues).
+For bugs and feature requests, please open a [Github Issue](https://github.com/vega/altair/issues).
 
 ## Development
 
 [![Hatch project](https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg)](https://github.com/pypa/hatch)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 [![pytest](https://img.shields.io/badge/logo-pytest-blue?logo=pytest&labelColor=5c5c5c&label=%20)](https://github.com/pytest-dev/pytest)
 
@@ -118,15 +118,15 @@
 To run the tests and linters, use
 
 ```
 hatch run test
 ```
 
 For information on how to contribute your developments back to the Vega-Altair repository, see
-[`CONTRIBUTING.md`](https://github.com/altair-viz/altair/blob/main/CONTRIBUTING.md)
+[`CONTRIBUTING.md`](https://github.com/vega/altair/blob/main/CONTRIBUTING.md)
 
 ## Citing Vega-Altair
 
 [![JOSS Paper](https://joss.theoj.org/papers/10.21105/joss.01057/status.svg)](https://joss.theoj.org/papers/10.21105/joss.01057)
 
 If you use Vega-Altair in academic work, please consider citing https://joss.theoj.org/papers/10.21105/joss.01057 as
```

#### html2text {}

```diff
@@ -1,38 +1,38 @@
 # Vega-Altair _[_h_t_t_p_s_:_/_/_a_l_t_a_i_r_-_v_i_z_._g_i_t_h_u_b_._i_o_/___s_t_a_t_i_c_/_a_l_t_a_i_r_-_l_o_g_o_-_l_i_g_h_t_._p_n_g_][!
-[github actions](https://github.com/altair-viz/altair/workflows/build/
-badge.svg)](https://github.com/altair-viz/altair/
-actions?query=workflow%3Abuild) [![typedlib_mypy](https://www.mypy-lang.org/
-static/mypy_badge.svg)](https://www.mypy-lang.org) [![JOSS Paper](https://
-joss.theoj.org/papers/10.21105/joss.01057/status.svg)](https://joss.theoj.org/
-papers/10.21105/joss.01057) [![PyPI - Downloads](https://img.shields.io/pypi/
-dm/altair)](https://pypi.org/project/altair) **Vega-Altair** is a declarative
-statistical visualization library for Python. With Vega-Altair, you can spend
-more time understanding your data and its meaning. Vega-Altair's API is simple,
-friendly and consistent and built on top of the powerful [Vega-Lite](https://
-github.com/vega/vega-lite) JSON specification. This elegant simplicity produces
-beautiful and effective visualizations with a minimal amount of code. *Vega-
-Altair was originally developed by [Jake Vanderplas](https://github.com/
-jakevdp) and [Brian Granger](https://github.com/ellisonbg) in close
-collaboration with the [UW Interactive Data Lab](https://idl.cs.washington.edu/
-).* *The Vega-Altair open source project is not affiliated with Altair
-Engineering, Inc.* ## Documentation See [Vega-Altair's Documentation Site]
-(https://altair-viz.github.io) as well as the [Tutorial Notebooks](https://
-github.com/altair-viz/altair_notebooks). You can run the notebooks directly in
-your browser by clicking on one of the following badges: [![Binder](https://
-beta.mybinder.org/badge.svg)](https://beta.mybinder.org/v2/gh/altair-viz/
-altair_notebooks/master) [![Colab](https://colab.research.google.com/assets/
-colab-badge.svg)](https://colab.research.google.com/github/altair-viz/
-altair_notebooks/blob/master/notebooks/Index.ipynb) ## Example Here is an
-example using Vega-Altair to quickly visualize and display a dataset with the
-native Vega-Lite renderer in the JupyterLab: ```python import altair as alt #
-load a simple dataset as a pandas DataFrame from vega_datasets import data cars
-= data.cars() alt.Chart(cars).mark_point().encode( x='Horsepower',
-y='Miles_per_Gallon', color='Origin', ) ``` ![Vega-Altair Visualization](https:
-//raw.githubusercontent.com/altair-viz/altair/main/images/cars.png) One of the
+[github actions](https://github.com/vega/altair/workflows/build/badge.svg)]
+(https://github.com/vega/altair/actions?query=workflow%3Abuild) [!
+[typedlib_mypy](https://www.mypy-lang.org/static/mypy_badge.svg)](https://
+www.mypy-lang.org) [![JOSS Paper](https://joss.theoj.org/papers/10.21105/
+joss.01057/status.svg)](https://joss.theoj.org/papers/10.21105/joss.01057) [!
+[PyPI - Downloads](https://img.shields.io/pypi/dm/altair)](https://pypi.org/
+project/altair) **Vega-Altair** is a declarative statistical visualization
+library for Python. With Vega-Altair, you can spend more time understanding
+your data and its meaning. Vega-Altair's API is simple, friendly and consistent
+and built on top of the powerful [Vega-Lite](https://github.com/vega/vega-lite)
+JSON specification. This elegant simplicity produces beautiful and effective
+visualizations with a minimal amount of code. *Vega-Altair was originally
+developed by [Jake Vanderplas](https://github.com/jakevdp) and [Brian Granger]
+(https://github.com/ellisonbg) in close collaboration with the [UW Interactive
+Data Lab](https://idl.cs.washington.edu/).* *The Vega-Altair open source
+project is not affiliated with Altair Engineering, Inc.* ## Documentation See
+[Vega-Altair's Documentation Site](https://altair-viz.github.io) as well as the
+[Tutorial Notebooks](https://github.com/altair-viz/altair_notebooks). You can
+run the notebooks directly in your browser by clicking on one of the following
+badges: [![Binder](https://beta.mybinder.org/badge.svg)](https://
+beta.mybinder.org/v2/gh/altair-viz/altair_notebooks/master) [![Colab](https://
+colab.research.google.com/assets/colab-badge.svg)](https://
+colab.research.google.com/github/altair-viz/altair_notebooks/blob/master/
+notebooks/Index.ipynb) ## Example Here is an example using Vega-Altair to
+quickly visualize and display a dataset with the native Vega-Lite renderer in
+the JupyterLab: ```python import altair as alt # load a simple dataset as a
+pandas DataFrame from vega_datasets import data cars = data.cars() alt.Chart
+(cars).mark_point().encode( x='Horsepower', y='Miles_per_Gallon',
+color='Origin', ) ``` ![Vega-Altair Visualization](https://
+raw.githubusercontent.com/altair-viz/altair/main/images/cars.png) One of the
 unique features of Vega-Altair, inherited from Vega-Lite, is a declarative
 grammar of not just visualization, but _interaction_. With a few modifications
 to the example above we can create a linked histogram that is filtered based on
 a selection of the scatter plot. ```python import altair as alt from
 vega_datasets import data source = data.cars() brush = alt.selection_interval()
 points = alt.Chart(source).mark_point().encode( x='Horsepower',
 y='Miles_per_Gallon', color=alt.condition(brush, 'Origin', alt.value
@@ -51,27 +51,27 @@
 Altair can be installed with: ```bash pip install altair ``` If you are using
 the conda package manager, the equivalent is: ```bash conda install altair -
 c conda-forge ``` For full installation instructions, please see [the
 documentation](https://altair-viz.github.io/getting_started/installation.html).
 ## Getting Help If you have a question that is not addressed in the
 documentation, you can post it on [StackOverflow](https://stackoverflow.com/
 questions/tagged/altair) using the `altair` tag. For bugs and feature requests,
-please open a [Github Issue](https://github.com/altair-viz/altair/issues). ##
+please open a [Github Issue](https://github.com/vega/altair/issues). ##
 Development [![Hatch project](https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-
 4051b5.svg)](https://github.com/pypa/hatch) [![Ruff](https://img.shields.io/
 endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/
 badge/v2.json)](https://github.com/astral-sh/ruff) [![pytest](https://
 img.shields.io/badge/logo-pytest-blue?logo=pytest&labelColor=5c5c5c&label=%20)]
 (https://github.com/pytest-dev/pytest) You can find the instructions on how to
 install the package for development in [the documentation](https://altair-
 viz.github.io/getting_started/installation.html). To run the tests and linters,
 use ``` hatch run test ``` For information on how to contribute your
 developments back to the Vega-Altair repository, see [`CONTRIBUTING.md`](https:
-//github.com/altair-viz/altair/blob/main/CONTRIBUTING.md) ## Citing Vega-Altair
-[![JOSS Paper](https://joss.theoj.org/papers/10.21105/joss.01057/status.svg)]
+//github.com/vega/altair/blob/main/CONTRIBUTING.md) ## Citing Vega-Altair [!
+[JOSS Paper](https://joss.theoj.org/papers/10.21105/joss.01057/status.svg)]
 (https://joss.theoj.org/papers/10.21105/joss.01057) If you use Vega-Altair in
 academic work, please consider citing https://joss.theoj.org/papers/10.21105/
 joss.01057 as ```bib @article{VanderPlas2018, doi = {10.21105/joss.01057}, url
 = {https://doi.org/10.21105/joss.01057}, year = {2018}, publisher = {The Open
 Journal}, volume = {3}, number = {32}, pages = {1057}, author = {Jacob
 VanderPlas and Brian Granger and Jeffrey Heer and Dominik Moritz and Kanit
 Wongsuphasawat and Arvind Satyanarayan and Eitan Lees and Ilia Timofeev and Ben
```

### Comparing `altair_alx_alpha-5.4.0.dev0/pyproject.toml` & `altair_alx_alpha-5.4.1a0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Typing :: Typed",
 ]
 
 [project.urls]
 Documentation = "https://altair-viz.github.io"
-Source = "https://github.com/altair-viz/altair"
+Source = "https://github.com/vega/altair"
 
 [project.optional-dependencies]
 all = [
     "vega_datasets>=0.9.0",
     "vl-convert-python>=1.3.0",
     "pyarrow>=11",
     "vegafusion[embed]>=1.6.6",
```

### Comparing `altair_alx_alpha-5.4.0.dev0/PKG-INFO` & `altair_alx_alpha-5.4.1a0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.3
 Name: altair_alx_alpha
-Version: 5.4.0.dev0
+Version: 5.4.1a0
 Summary: Vega-Altair: A declarative statistical visualization library for Python.
 Project-URL: Documentation, https://altair-viz.github.io
-Project-URL: Source, https://github.com/altair-viz/altair
+Project-URL: Source, https://github.com/vega/altair
 Author: Vega-Altair Contributors
 License-File: LICENSE
 Keywords: declarative,interactive,json,statistics,vega-lite,visualization
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
@@ -57,15 +57,15 @@
 Requires-Dist: sphinx-copybutton; extra == 'doc'
 Requires-Dist: sphinx-design; extra == 'doc'
 Requires-Dist: sphinxext-altair; extra == 'doc'
 Description-Content-Type: text/markdown
 
 # Vega-Altair <a href="https://altair-viz.github.io/"><img align="right" src="https://altair-viz.github.io/_static/altair-logo-light.png" height="50"></img></a>
 
-[![github actions](https://github.com/altair-viz/altair/workflows/build/badge.svg)](https://github.com/altair-viz/altair/actions?query=workflow%3Abuild)
+[![github actions](https://github.com/vega/altair/workflows/build/badge.svg)](https://github.com/vega/altair/actions?query=workflow%3Abuild)
 [![typedlib_mypy](https://www.mypy-lang.org/static/mypy_badge.svg)](https://www.mypy-lang.org)
 [![JOSS Paper](https://joss.theoj.org/papers/10.21105/joss.01057/status.svg)](https://joss.theoj.org/papers/10.21105/joss.01057)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/altair)](https://pypi.org/project/altair)
 
 **Vega-Altair** is a declarative statistical visualization library for Python. With Vega-Altair, you can spend more time understanding your data and its meaning. Vega-Altair's
 API is simple, friendly and consistent and built on top of the powerful
 [Vega-Lite](https://github.com/vega/vega-lite) JSON specification. This elegant
@@ -162,15 +162,15 @@
 
 For full installation instructions, please see [the documentation](https://altair-viz.github.io/getting_started/installation.html).
 
 ## Getting Help
 
 If you have a question that is not addressed in the documentation, 
 you can post it on [StackOverflow](https://stackoverflow.com/questions/tagged/altair) using the `altair` tag.
-For bugs and feature requests, please open a [Github Issue](https://github.com/altair-viz/altair/issues).
+For bugs and feature requests, please open a [Github Issue](https://github.com/vega/altair/issues).
 
 ## Development
 
 [![Hatch project](https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg)](https://github.com/pypa/hatch)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 [![pytest](https://img.shields.io/badge/logo-pytest-blue?logo=pytest&labelColor=5c5c5c&label=%20)](https://github.com/pytest-dev/pytest)
 
@@ -179,15 +179,15 @@
 To run the tests and linters, use
 
 ```
 hatch run test
 ```
 
 For information on how to contribute your developments back to the Vega-Altair repository, see
-[`CONTRIBUTING.md`](https://github.com/altair-viz/altair/blob/main/CONTRIBUTING.md)
+[`CONTRIBUTING.md`](https://github.com/vega/altair/blob/main/CONTRIBUTING.md)
 
 ## Citing Vega-Altair
 
 [![JOSS Paper](https://joss.theoj.org/papers/10.21105/joss.01057/status.svg)](https://joss.theoj.org/papers/10.21105/joss.01057)
 
 If you use Vega-Altair in academic work, please consider citing https://joss.theoj.org/papers/10.21105/joss.01057 as
```

#### html2text {}

```diff
@@ -1,45 +1,45 @@
-Metadata-Version: 2.3 Name: altair_alx_alpha Version: 5.4.0.dev0 Summary: Vega-
+Metadata-Version: 2.3 Name: altair_alx_alpha Version: 5.4.1a0 Summary: Vega-
 Altair: A declarative statistical visualization library for Python. Project-
 URL: Documentation, https://altair-viz.github.io Project-URL: Source, https://
-github.com/altair-viz/altair Author: Vega-Altair Contributors License-File:
-LICENSE Keywords: declarative,interactive,json,statistics,vega-
-lite,visualization Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Console Classifier: Intended Audience :: Science/
-Research Classifier: License :: OSI Approved :: BSD License Classifier: Natural
-Language :: English Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
-Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12 Classifier: Typing :: Typed
-Requires-Python: >=3.8 Requires-Dist: jinja2 Requires-Dist: jsonschema>=3.0
-Requires-Dist: numpy Requires-Dist: packaging Requires-Dist: pandas>=0.25
-Requires-Dist: toolz Requires-Dist: typing-extensions>=4.0.1; python_version <
-'3.11' Provides-Extra: all Requires-Dist: altair-tiles>=0.3.0; extra == 'all'
-Requires-Dist: anywidget>=0.9.0; extra == 'all' Requires-Dist: pyarrow>=11;
-extra == 'all' Requires-Dist: vega-datasets>=0.9.0; extra == 'all' Requires-
-Dist: vegafusion[embed]>=1.6.6; extra == 'all' Requires-Dist: vl-convert-
-python>=1.3.0; extra == 'all' Provides-Extra: dev Requires-Dist: geopandas;
-extra == 'dev' Requires-Dist: hatch; extra == 'dev' Requires-Dist: ipython;
-extra == 'dev' Requires-Dist: m2r; extra == 'dev' Requires-Dist: mypy; extra ==
-'dev' Requires-Dist: pandas-stubs; extra == 'dev' Requires-Dist: pytest; extra
-== 'dev' Requires-Dist: pytest-cov; extra == 'dev' Requires-Dist: ruff>=0.3.0;
-extra == 'dev' Requires-Dist: types-jsonschema; extra == 'dev' Requires-Dist:
-types-setuptools; extra == 'dev' Provides-Extra: doc Requires-Dist: docutils;
-extra == 'doc' Requires-Dist: jinja2; extra == 'doc' Requires-Dist: myst-
-parser; extra == 'doc' Requires-Dist: numpydoc; extra == 'doc' Requires-Dist:
+github.com/vega/altair Author: Vega-Altair Contributors License-File: LICENSE
+Keywords: declarative,interactive,json,statistics,vega-lite,visualization
+Classifier: Development Status :: 5 - Production/Stable Classifier: Environment
+:: Console Classifier: Intended Audience :: Science/Research Classifier:
+License :: OSI Approved :: BSD License Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
+Language :: Python :: 3.12 Classifier: Typing :: Typed Requires-Python: >=3.8
+Requires-Dist: jinja2 Requires-Dist: jsonschema>=3.0 Requires-Dist: numpy
+Requires-Dist: packaging Requires-Dist: pandas>=0.25 Requires-Dist: toolz
+Requires-Dist: typing-extensions>=4.0.1; python_version < '3.11' Provides-
+Extra: all Requires-Dist: altair-tiles>=0.3.0; extra == 'all' Requires-Dist:
+anywidget>=0.9.0; extra == 'all' Requires-Dist: pyarrow>=11; extra == 'all'
+Requires-Dist: vega-datasets>=0.9.0; extra == 'all' Requires-Dist: vegafusion
+[embed]>=1.6.6; extra == 'all' Requires-Dist: vl-convert-python>=1.3.0; extra
+== 'all' Provides-Extra: dev Requires-Dist: geopandas; extra == 'dev' Requires-
+Dist: hatch; extra == 'dev' Requires-Dist: ipython; extra == 'dev' Requires-
+Dist: m2r; extra == 'dev' Requires-Dist: mypy; extra == 'dev' Requires-Dist:
+pandas-stubs; extra == 'dev' Requires-Dist: pytest; extra == 'dev' Requires-
+Dist: pytest-cov; extra == 'dev' Requires-Dist: ruff>=0.3.0; extra == 'dev'
+Requires-Dist: types-jsonschema; extra == 'dev' Requires-Dist: types-
+setuptools; extra == 'dev' Provides-Extra: doc Requires-Dist: docutils; extra
+== 'doc' Requires-Dist: jinja2; extra == 'doc' Requires-Dist: myst-parser;
+extra == 'doc' Requires-Dist: numpydoc; extra == 'doc' Requires-Dist:
 pillow<10,>=9; extra == 'doc' Requires-Dist: pydata-sphinx-theme>=0.14.1; extra
 == 'doc' Requires-Dist: scipy; extra == 'doc' Requires-Dist: sphinx; extra ==
 'doc' Requires-Dist: sphinx-copybutton; extra == 'doc' Requires-Dist: sphinx-
 design; extra == 'doc' Requires-Dist: sphinxext-altair; extra == 'doc'
 Description-Content-Type: text/markdown # Vega-Altair _[_h_t_t_p_s_:_/_/_a_l_t_a_i_r_-
 _v_i_z_._g_i_t_h_u_b_._i_o_/___s_t_a_t_i_c_/_a_l_t_a_i_r_-_l_o_g_o_-_l_i_g_h_t_._p_n_g_][![github actions](https://
-github.com/altair-viz/altair/workflows/build/badge.svg)](https://github.com/
-altair-viz/altair/actions?query=workflow%3Abuild) [![typedlib_mypy](https://
-www.mypy-lang.org/static/mypy_badge.svg)](https://www.mypy-lang.org) [![JOSS
-Paper](https://joss.theoj.org/papers/10.21105/joss.01057/status.svg)](https://
+github.com/vega/altair/workflows/build/badge.svg)](https://github.com/vega/
+altair/actions?query=workflow%3Abuild) [![typedlib_mypy](https://www.mypy-
+lang.org/static/mypy_badge.svg)](https://www.mypy-lang.org) [![JOSS Paper]
+(https://joss.theoj.org/papers/10.21105/joss.01057/status.svg)](https://
 joss.theoj.org/papers/10.21105/joss.01057) [![PyPI - Downloads](https://
 img.shields.io/pypi/dm/altair)](https://pypi.org/project/altair) **Vega-
 Altair** is a declarative statistical visualization library for Python. With
 Vega-Altair, you can spend more time understanding your data and its meaning.
 Vega-Altair's API is simple, friendly and consistent and built on top of the
 powerful [Vega-Lite](https://github.com/vega/vega-lite) JSON specification.
 This elegant simplicity produces beautiful and effective visualizations with a
@@ -84,27 +84,27 @@
 Altair can be installed with: ```bash pip install altair ``` If you are using
 the conda package manager, the equivalent is: ```bash conda install altair -
 c conda-forge ``` For full installation instructions, please see [the
 documentation](https://altair-viz.github.io/getting_started/installation.html).
 ## Getting Help If you have a question that is not addressed in the
 documentation, you can post it on [StackOverflow](https://stackoverflow.com/
 questions/tagged/altair) using the `altair` tag. For bugs and feature requests,
-please open a [Github Issue](https://github.com/altair-viz/altair/issues). ##
+please open a [Github Issue](https://github.com/vega/altair/issues). ##
 Development [![Hatch project](https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-
 4051b5.svg)](https://github.com/pypa/hatch) [![Ruff](https://img.shields.io/
 endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/
 badge/v2.json)](https://github.com/astral-sh/ruff) [![pytest](https://
 img.shields.io/badge/logo-pytest-blue?logo=pytest&labelColor=5c5c5c&label=%20)]
 (https://github.com/pytest-dev/pytest) You can find the instructions on how to
 install the package for development in [the documentation](https://altair-
 viz.github.io/getting_started/installation.html). To run the tests and linters,
 use ``` hatch run test ``` For information on how to contribute your
 developments back to the Vega-Altair repository, see [`CONTRIBUTING.md`](https:
-//github.com/altair-viz/altair/blob/main/CONTRIBUTING.md) ## Citing Vega-Altair
-[![JOSS Paper](https://joss.theoj.org/papers/10.21105/joss.01057/status.svg)]
+//github.com/vega/altair/blob/main/CONTRIBUTING.md) ## Citing Vega-Altair [!
+[JOSS Paper](https://joss.theoj.org/papers/10.21105/joss.01057/status.svg)]
 (https://joss.theoj.org/papers/10.21105/joss.01057) If you use Vega-Altair in
 academic work, please consider citing https://joss.theoj.org/papers/10.21105/
 joss.01057 as ```bib @article{VanderPlas2018, doi = {10.21105/joss.01057}, url
 = {https://doi.org/10.21105/joss.01057}, year = {2018}, publisher = {The Open
 Journal}, volume = {3}, number = {32}, pages = {1057}, author = {Jacob
 VanderPlas and Brian Granger and Jeffrey Heer and Dominik Moritz and Kanit
 Wongsuphasawat and Arvind Satyanarayan and Eitan Lees and Ilia Timofeev and Ben
```

