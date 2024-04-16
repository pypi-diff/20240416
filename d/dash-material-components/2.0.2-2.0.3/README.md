# Comparing `tmp/dash_material_components-2.0.2.tar.gz` & `tmp/dash_material_components-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dash_material_components-2.0.2.tar", max compression
+gzip compressed data, was "dash_material_components-2.0.3.tar", max compression
```

## Comparing `dash_material_components-2.0.2.tar` & `dash_material_components-2.0.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0     1077 2024-03-26 11:08:03.805259 dash_material_components-2.0.2/LICENSE
--rw-r--r--   0        0        0     5627 2024-03-26 11:08:03.805259 dash_material_components-2.0.2/README.md
--rw-r--r--   0        0        0     1506 2024-03-26 11:07:32.000000 dash_material_components-2.0.2/dash_material_components/Alert.py
--rw-r--r--   0        0        0     3496 2024-03-26 11:07:32.000000 dash_material_components-2.0.2/dash_material_components/Autocomplete.py
--rw-r--r--   0        0        0     1350 2024-03-26 11:07:32.000000 dash_material_components-2.0.2/dash_material_components/Box.py
--rw-r--r--   0        0        0     3120 2024-03-26 11:07:32.000000 dash_material_components-2.0.2/dash_material_components/Button.py
--rw-r--r--   0        0        0     2772 2024-03-26 11:07:32.000000 dash_material_components-2.0.2/dash_material_components/Calendar.py
--rw-r--r--   0        0        0     1457 2024-03-26 11:07:32.000000 dash_material_components-2.0.2/dash_material_components/Dashboard.py
--rw-r--r--   0        0        0     2345 2024-03-26 11:07:32.000000 dash_material_components-2.0.2/dash_material_components/Dropdown.py
--rw-r--r--   0        0        0     3643 2024-03-26 11:07:32.000000 dash_material_components-2.0.2/dash_material_components/InputText.py
--rw-r--r--   0        0        0     1289 2024-03-26 11:07:32.000000 dash_material_components-2.0.2/dash_material_components/NavBar.py
--rw-r--r--   0        0        0     1591 2024-03-26 11:07:32.000000 dash_material_components-2.0.2/dash_material_components/Page.py
--rw-r--r--   0        0        0     2102 2024-03-26 11:07:32.000000 dash_material_components-2.0.2/dash_material_components/Section.py
--rw-r--r--   0        0        0     1383 2024-03-26 11:07:32.000000 dash_material_components-2.0.2/dash_material_components/SideBar.py
--rw-r--r--   0        0        0     2980 2024-03-26 11:07:32.000000 dash_material_components-2.0.2/dash_material_components/Slider.py
--rw-r--r--   0        0        0     1614 2024-03-26 11:07:32.000000 dash_material_components-2.0.2/dash_material_components/Tab.py
--rw-r--r--   0        0        0     1894 2024-03-26 11:07:32.000000 dash_material_components-2.0.2/dash_material_components/Table.py
--rw-r--r--   0        0        0     1972 2024-03-26 11:07:32.000000 dash_material_components-2.0.2/dash_material_components/Toggle.py
--rw-r--r--   0        0        0     1675 2024-03-26 11:07:32.000000 dash_material_components-2.0.2/dash_material_components/Typography.py
--rw-r--r--   0        0        0     1077 2024-03-26 11:05:35.000000 dash_material_components-2.0.2/dash_material_components/__init__.py
--rw-r--r--   0        0        0      746 2024-03-26 11:07:32.000000 dash_material_components-2.0.2/dash_material_components/_imports_.py
--rw-r--r--   0        0        0  4863311 2024-03-26 11:07:22.000000 dash_material_components-2.0.2/dash_material_components/dash_material_components.js
--rw-r--r--   0        0        0    49596 2024-03-26 11:07:32.000000 dash_material_components-2.0.2/dash_material_components/metadata.json
--rw-r--r--   0        0        0     2806 2024-03-26 11:07:25.000000 dash_material_components-2.0.2/dash_material_components/package-info.json
--rw-r--r--   0        0        0       56 2024-03-26 11:05:35.000000 dash_material_components-2.0.2/dash_material_components/themes/__init__.py
--rw-r--r--   0        0        0     1624 2024-03-26 11:05:35.000000 dash_material_components-2.0.2/dash_material_components/themes/base.py
--rw-r--r--   0        0        0     3104 2024-03-26 11:05:35.000000 dash_material_components-2.0.2/dash_material_components/themes/plotly.py
--rw-r--r--   0        0        0    44261 2024-03-26 11:05:35.000000 dash_material_components-2.0.2/dash_material_components/themes/static/logo.png
--rw-r--r--   0        0        0      562 2024-03-26 11:05:35.000000 dash_material_components-2.0.2/dash_material_components/themes/utils.py
--rw-r--r--   0        0        0     2806 2024-03-26 11:08:03.805259 dash_material_components-2.0.2/package.json
--rw-r--r--   0        0        0     2305 2024-03-26 11:08:03.805259 dash_material_components-2.0.2/pyproject.toml
--rw-r--r--   0        0        0     6310 1970-01-01 00:00:00.000000 dash_material_components-2.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1077 2024-04-16 17:21:31.390977 dash_material_components-2.0.3/LICENSE
+-rw-r--r--   0        0        0     5627 2024-04-16 17:21:31.390977 dash_material_components-2.0.3/README.md
+-rw-r--r--   0        0        0     1506 2024-04-16 17:20:43.000000 dash_material_components-2.0.3/dash_material_components/Alert.py
+-rw-r--r--   0        0        0     3496 2024-04-16 17:20:43.000000 dash_material_components-2.0.3/dash_material_components/Autocomplete.py
+-rw-r--r--   0        0        0     1350 2024-04-16 17:20:43.000000 dash_material_components-2.0.3/dash_material_components/Box.py
+-rw-r--r--   0        0        0     3120 2024-04-16 17:20:43.000000 dash_material_components-2.0.3/dash_material_components/Button.py
+-rw-r--r--   0        0        0     2772 2024-04-16 17:20:43.000000 dash_material_components-2.0.3/dash_material_components/Calendar.py
+-rw-r--r--   0        0        0     1457 2024-04-16 17:20:43.000000 dash_material_components-2.0.3/dash_material_components/Dashboard.py
+-rw-r--r--   0        0        0     2345 2024-04-16 17:20:43.000000 dash_material_components-2.0.3/dash_material_components/Dropdown.py
+-rw-r--r--   0        0        0     3934 2024-04-16 17:20:43.000000 dash_material_components-2.0.3/dash_material_components/InputText.py
+-rw-r--r--   0        0        0     1289 2024-04-16 17:20:43.000000 dash_material_components-2.0.3/dash_material_components/NavBar.py
+-rw-r--r--   0        0        0     1591 2024-04-16 17:20:43.000000 dash_material_components-2.0.3/dash_material_components/Page.py
+-rw-r--r--   0        0        0     2102 2024-04-16 17:20:43.000000 dash_material_components-2.0.3/dash_material_components/Section.py
+-rw-r--r--   0        0        0     1383 2024-04-16 17:20:43.000000 dash_material_components-2.0.3/dash_material_components/SideBar.py
+-rw-r--r--   0        0        0     2980 2024-04-16 17:20:43.000000 dash_material_components-2.0.3/dash_material_components/Slider.py
+-rw-r--r--   0        0        0     1614 2024-04-16 17:20:43.000000 dash_material_components-2.0.3/dash_material_components/Tab.py
+-rw-r--r--   0        0        0     1894 2024-04-16 17:20:43.000000 dash_material_components-2.0.3/dash_material_components/Table.py
+-rw-r--r--   0        0        0     1972 2024-04-16 17:20:43.000000 dash_material_components-2.0.3/dash_material_components/Toggle.py
+-rw-r--r--   0        0        0     1675 2024-04-16 17:20:43.000000 dash_material_components-2.0.3/dash_material_components/Typography.py
+-rw-r--r--   0        0        0     1077 2024-04-16 17:18:33.000000 dash_material_components-2.0.3/dash_material_components/__init__.py
+-rw-r--r--   0        0        0      746 2024-04-16 17:20:43.000000 dash_material_components-2.0.3/dash_material_components/_imports_.py
+-rw-r--r--   0        0        0  4863579 2024-04-16 17:20:34.000000 dash_material_components-2.0.3/dash_material_components/dash_material_components.js
+-rw-r--r--   0        0        0    50010 2024-04-16 17:20:43.000000 dash_material_components-2.0.3/dash_material_components/metadata.json
+-rw-r--r--   0        0        0     2806 2024-04-16 17:20:36.000000 dash_material_components-2.0.3/dash_material_components/package-info.json
+-rw-r--r--   0        0        0       56 2024-04-16 17:18:33.000000 dash_material_components-2.0.3/dash_material_components/themes/__init__.py
+-rw-r--r--   0        0        0     1624 2024-04-16 17:18:33.000000 dash_material_components-2.0.3/dash_material_components/themes/base.py
+-rw-r--r--   0        0        0     3104 2024-04-16 17:18:33.000000 dash_material_components-2.0.3/dash_material_components/themes/plotly.py
+-rw-r--r--   0        0        0    44261 2024-04-16 17:18:33.000000 dash_material_components-2.0.3/dash_material_components/themes/static/logo.png
+-rw-r--r--   0        0        0      562 2024-04-16 17:18:33.000000 dash_material_components-2.0.3/dash_material_components/themes/utils.py
+-rw-r--r--   0        0        0     2806 2024-04-16 17:21:31.394977 dash_material_components-2.0.3/package.json
+-rw-r--r--   0        0        0     2305 2024-04-16 17:21:31.394977 dash_material_components-2.0.3/pyproject.toml
+-rw-r--r--   0        0        0     6310 1970-01-01 00:00:00.000000 dash_material_components-2.0.3/PKG-INFO
```

### Comparing `dash_material_components-2.0.2/LICENSE` & `dash_material_components-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dash_material_components-2.0.2/README.md` & `dash_material_components-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `dash_material_components-2.0.2/dash_material_components/Alert.py` & `dash_material_components-2.0.3/dash_material_components/Alert.py`

 * *Files identical despite different names*

### Comparing `dash_material_components-2.0.2/dash_material_components/Autocomplete.py` & `dash_material_components-2.0.3/dash_material_components/Autocomplete.py`

 * *Files identical despite different names*

### Comparing `dash_material_components-2.0.2/dash_material_components/Box.py` & `dash_material_components-2.0.3/dash_material_components/Box.py`

 * *Files identical despite different names*

### Comparing `dash_material_components-2.0.2/dash_material_components/Button.py` & `dash_material_components-2.0.3/dash_material_components/Button.py`

 * *Files identical despite different names*

### Comparing `dash_material_components-2.0.2/dash_material_components/Calendar.py` & `dash_material_components-2.0.3/dash_material_components/Calendar.py`

 * *Files identical despite different names*

### Comparing `dash_material_components-2.0.2/dash_material_components/Dashboard.py` & `dash_material_components-2.0.3/dash_material_components/Dashboard.py`

 * *Files identical despite different names*

### Comparing `dash_material_components-2.0.2/dash_material_components/Dropdown.py` & `dash_material_components-2.0.3/dash_material_components/Dropdown.py`

 * *Files identical despite different names*

### Comparing `dash_material_components-2.0.2/dash_material_components/InputText.py` & `dash_material_components-2.0.3/dash_material_components/InputText.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,14 +20,20 @@
 
 - adornmentRight (string; optional):
     An adornment to be displayed at the end of the input.
 
 - autoFocus (boolean; optional):
     If True, the input will be focused automatically.
 
+- debounce (boolean; optional):
+    Delay dash update.
+
+- debounceSeconds (number; optional):
+    Dash update delay in seconds, must pass debounce=True as well.
+
 - disabled (boolean; optional):
     If True, the input field will be disabled.
 
 - error (boolean; optional):
     If True, the input field will indicate an error.
 
 - inputType (a value equal to: 'text', 'integer', 'float'; optional):
@@ -66,18 +72,18 @@
 - width (string; optional):
     The width of the input field (CSS value as string)."""
     _children_props = []
     _base_nodes = ['children']
     _namespace = 'dash_material_components'
     _type = 'InputText'
     @_explicitize_args
-    def __init__(self, children=None, labelText=Component.UNDEFINED, value=Component.UNDEFINED, maxValue=Component.UNDEFINED, minValue=Component.UNDEFINED, precision=Component.UNDEFINED, inputType=Component.UNDEFINED, multiline=Component.UNDEFINED, variant=Component.UNDEFINED, maxLength=Component.UNDEFINED, autoFocus=Component.UNDEFINED, size=Component.UNDEFINED, width=Component.UNDEFINED, margin=Component.UNDEFINED, adornmentLeft=Component.UNDEFINED, adornmentRight=Component.UNDEFINED, disabled=Component.UNDEFINED, error=Component.UNDEFINED, id=Component.UNDEFINED, **kwargs):
-        self._prop_names = ['children', 'id', 'adornmentLeft', 'adornmentRight', 'autoFocus', 'disabled', 'error', 'inputType', 'labelText', 'margin', 'maxLength', 'maxValue', 'minValue', 'multiline', 'precision', 'size', 'value', 'variant', 'width']
+    def __init__(self, children=None, labelText=Component.UNDEFINED, value=Component.UNDEFINED, maxValue=Component.UNDEFINED, minValue=Component.UNDEFINED, precision=Component.UNDEFINED, inputType=Component.UNDEFINED, multiline=Component.UNDEFINED, variant=Component.UNDEFINED, maxLength=Component.UNDEFINED, autoFocus=Component.UNDEFINED, size=Component.UNDEFINED, width=Component.UNDEFINED, margin=Component.UNDEFINED, adornmentLeft=Component.UNDEFINED, adornmentRight=Component.UNDEFINED, disabled=Component.UNDEFINED, error=Component.UNDEFINED, debounce=Component.UNDEFINED, debounceSeconds=Component.UNDEFINED, id=Component.UNDEFINED, **kwargs):
+        self._prop_names = ['children', 'id', 'adornmentLeft', 'adornmentRight', 'autoFocus', 'debounce', 'debounceSeconds', 'disabled', 'error', 'inputType', 'labelText', 'margin', 'maxLength', 'maxValue', 'minValue', 'multiline', 'precision', 'size', 'value', 'variant', 'width']
         self._valid_wildcard_attributes =            []
-        self.available_properties = ['children', 'id', 'adornmentLeft', 'adornmentRight', 'autoFocus', 'disabled', 'error', 'inputType', 'labelText', 'margin', 'maxLength', 'maxValue', 'minValue', 'multiline', 'precision', 'size', 'value', 'variant', 'width']
+        self.available_properties = ['children', 'id', 'adornmentLeft', 'adornmentRight', 'autoFocus', 'debounce', 'debounceSeconds', 'disabled', 'error', 'inputType', 'labelText', 'margin', 'maxLength', 'maxValue', 'minValue', 'multiline', 'precision', 'size', 'value', 'variant', 'width']
         self.available_wildcard_properties =            []
         _explicit_args = kwargs.pop('_explicit_args')
         _locals = locals()
         _locals.update(kwargs)  # For wildcard attrs and excess named props
         args = {k: _locals[k] for k in _explicit_args if k != 'children'}
 
         super(InputText, self).__init__(children=children, **args)
```

### Comparing `dash_material_components-2.0.2/dash_material_components/NavBar.py` & `dash_material_components-2.0.3/dash_material_components/NavBar.py`

 * *Files identical despite different names*

### Comparing `dash_material_components-2.0.2/dash_material_components/Page.py` & `dash_material_components-2.0.3/dash_material_components/Page.py`

 * *Files identical despite different names*

### Comparing `dash_material_components-2.0.2/dash_material_components/Section.py` & `dash_material_components-2.0.3/dash_material_components/Section.py`

 * *Files identical despite different names*

### Comparing `dash_material_components-2.0.2/dash_material_components/SideBar.py` & `dash_material_components-2.0.3/dash_material_components/SideBar.py`

 * *Files identical despite different names*

### Comparing `dash_material_components-2.0.2/dash_material_components/Slider.py` & `dash_material_components-2.0.3/dash_material_components/Slider.py`

 * *Files identical despite different names*

### Comparing `dash_material_components-2.0.2/dash_material_components/Tab.py` & `dash_material_components-2.0.3/dash_material_components/Tab.py`

 * *Files identical despite different names*

### Comparing `dash_material_components-2.0.2/dash_material_components/Table.py` & `dash_material_components-2.0.3/dash_material_components/Table.py`

 * *Files identical despite different names*

### Comparing `dash_material_components-2.0.2/dash_material_components/Toggle.py` & `dash_material_components-2.0.3/dash_material_components/Toggle.py`

 * *Files identical despite different names*

### Comparing `dash_material_components-2.0.2/dash_material_components/Typography.py` & `dash_material_components-2.0.3/dash_material_components/Typography.py`

 * *Files identical despite different names*

### Comparing `dash_material_components-2.0.2/dash_material_components/__init__.py` & `dash_material_components-2.0.3/dash_material_components/__init__.py`

 * *Files identical despite different names*

### Comparing `dash_material_components-2.0.2/dash_material_components/_imports_.py` & `dash_material_components-2.0.3/dash_material_components/_imports_.py`

 * *Files identical despite different names*

### Comparing `dash_material_components-2.0.2/dash_material_components/dash_material_components.js` & `dash_material_components-2.0.3/dash_material_components/dash_material_components.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -95302,25 +95302,32 @@
                         R = void 0 === b ? null : b,
                         O = e.adornmentRight,
                         k = void 0 === O ? null : O,
                         P = e.disabled,
                         D = void 0 !== P && P,
                         B = e.error,
                         F = void 0 !== B && B,
-                        N = e.setProps,
-                        E = (0, o.useState)(g),
-                        I = E[0],
-                        W = E[1];
+                        N = e.debounce,
+                        E = void 0 !== N && N,
+                        I = e.debounceSeconds,
+                        W = void 0 === I ? 1 : I,
+                        $ = e.setProps,
+                        U = (0, o.useState)(g),
+                        G = U[0],
+                        K = U[1],
+                        _ = (0, o.useState)(0),
+                        Y = _[0],
+                        q = _[1];
                     return (0, a.jsx)(l.Box, h({
                         id: t,
                         m: T,
                         width: C
                     }, {
                         children: (0, a.jsx)(l.TextField, {
-                            value: I,
+                            value: G,
                             type: p,
                             size: j,
                             label: d,
                             InputLabelProps: {
                                 shrink: !0
                             },
                             multiline: u,
@@ -95337,17 +95344,25 @@
                                         }
                                         if ("integer" === c || "float" === c) {
                                             if (e.split("-").length > 2) return !1;
                                             if (e = Number(e), null != t && e < t || null != h && e > h) return !1
                                         } else if (o && e.length > o) return !1;
                                         return !0
                                     }(c, p, n, i, w, H);
-                                t ? (W(c), N({
+                                t ? (K(c), E ? function(e, c) {
+                                    window.clearTimeout(Y);
+                                    var t = window.setTimeout((function() {
+                                        $({
+                                            value: c
+                                        })
+                                    }), 1e3 * e);
+                                    q(t)
+                                }(W, c) : $({
                                     value: c
-                                })) : "" != c && "-" != c || W(c)
+                                })) : "" != c && "-" != c || K(c)
                             },
                             autoFocus: x,
                             InputProps: {
                                 startAdornment: R ? (0, a.jsx)(l.InputAdornment, h({
                                     position: "start"
                                 }, {
                                     children: R
@@ -95356,15 +95371,20 @@
                                     position: "end"
                                 }, {
                                     children: k
                                 })) : null
                             },
                             fullWidth: null !== C,
                             disabled: D,
-                            error: F
+                            error: F,
+                            onBlur: function() {
+                                E && (window.clearTimeout(Y), $({
+                                    value: G
+                                }))
+                            }
                         })
                     }))
                 }
             },
             2442: function(e, c, t) {
                 "use strict";
                 var h = this && this.__makeTemplateObject || function(e, c) {
```

### Comparing `dash_material_components-2.0.2/dash_material_components/metadata.json` & `dash_material_components-2.0.3/dash_material_components/metadata.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9996657754010694%*

 * *Differences: {"'src/components/inputs/InputText.tsx'": "{'props': {'debounce': OrderedDict([('description', "*

 * *                                          "'Delay dash update'), ('required', False), ('type', "*

 * *                                          "OrderedDict([('name', 'bool'), ('raw', 'boolean')]))]), "*

 * *                                          "'debounceSeconds': OrderedDict([('description', 'Dash "*

 * *                                          'update delay in seconds, must pass debounce=True as '*

 * *                      […]*

```diff
@@ -1127,14 +1127,30 @@
                 "description": "Component children",
                 "required": false,
                 "type": {
                     "name": "node",
                     "raw": "ReactNode"
                 }
             },
+            "debounce": {
+                "description": "Delay dash update",
+                "required": false,
+                "type": {
+                    "name": "bool",
+                    "raw": "boolean"
+                }
+            },
+            "debounceSeconds": {
+                "description": "Dash update delay in seconds, must pass debounce=True as well",
+                "required": false,
+                "type": {
+                    "name": "number",
+                    "raw": "number"
+                }
+            },
             "disabled": {
                 "description": "If true, the input field will be disabled",
                 "required": false,
                 "type": {
                     "name": "bool",
                     "raw": "boolean"
                 }
```

### Comparing `dash_material_components-2.0.2/dash_material_components/package-info.json` & `dash_material_components-2.0.3/dash_material_components/package-info.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9583333333333334%*

 * *Differences: {"'version'": "'2.0.3'"}*

```diff
@@ -73,9 +73,9 @@
         "lint": "yarn run lint:prettier && yarn run lint:eslint",
         "lint:eslint": "eslint ./src",
         "lint:prettier": "prettier ./src --config .prettierrc --list-different",
         "postbuild": "es-check es7 dash_material_components/*.js",
         "test": "jest ./src",
         "watch": "yarn run build:js::dev -- --watch"
     },
-    "version": "2.0.2"
+    "version": "2.0.3"
 }
```

### Comparing `dash_material_components-2.0.2/dash_material_components/themes/base.py` & `dash_material_components-2.0.3/dash_material_components/themes/base.py`

 * *Files identical despite different names*

### Comparing `dash_material_components-2.0.2/dash_material_components/themes/plotly.py` & `dash_material_components-2.0.3/dash_material_components/themes/plotly.py`

 * *Files identical despite different names*

### Comparing `dash_material_components-2.0.2/dash_material_components/themes/static/logo.png` & `dash_material_components-2.0.3/dash_material_components/themes/static/logo.png`

 * *Files identical despite different names*

### Comparing `dash_material_components-2.0.2/dash_material_components/themes/utils.py` & `dash_material_components-2.0.3/dash_material_components/themes/utils.py`

 * *Files identical despite different names*

### Comparing `dash_material_components-2.0.2/package.json` & `dash_material_components-2.0.3/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9583333333333334%*

 * *Differences: {"'version'": "'2.0.3'"}*

```diff
@@ -73,9 +73,9 @@
         "lint": "yarn run lint:prettier && yarn run lint:eslint",
         "lint:eslint": "eslint ./src",
         "lint:prettier": "prettier ./src --config .prettierrc --list-different",
         "postbuild": "es-check es7 dash_material_components/*.js",
         "test": "jest ./src",
         "watch": "yarn run build:js::dev -- --watch"
     },
-    "version": "2.0.2"
+    "version": "2.0.3"
 }
```

### Comparing `dash_material_components-2.0.2/pyproject.toml` & `dash_material_components-2.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry>=1.0.0"]
 build-backend = "poetry.masonry.api"
 
 [tool.poetry]
 # Description
 name = "dash-material-components"
-version = "2.0.2"
+version = "2.0.3"
 description = "Dash Material Design components for the Noos platform."
 # Credentials
 license = "MIT"
 authors = ["Noos Energy <contact@noos.energy>"]
 homepage = "https://github.com/noosenergy/dash-material-components"
 # Package data
 readme = "README.md"
```

### Comparing `dash_material_components-2.0.2/PKG-INFO` & `dash_material_components-2.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dash-material-components
-Version: 2.0.2
+Version: 2.0.3
 Summary: Dash Material Design components for the Noos platform.
 Home-page: https://github.com/noosenergy/dash-material-components
 License: MIT
 Author: Noos Energy
 Author-email: contact@noos.energy
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 3 - Alpha
```

