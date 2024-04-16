# Comparing `tmp/trame-components-2.2.1.tar.gz` & `tmp/trame-components-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trame-components-2.2.1.tar", last modified: Tue Sep 19 20:44:35 2023, max compression
+gzip compressed data, was "trame-components-2.3.0.tar", last modified: Tue Apr 16 00:01:04 2024, max compression
```

## Comparing `trame-components-2.2.1.tar` & `trame-components-2.3.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 20:44:35.532225 trame-components-2.2.1/
--rw-r--r--   0 root         (0) root         (0)      552 2023-09-19 20:44:15.000000 trame-components-2.2.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       69 2023-09-19 20:44:15.000000 trame-components-2.2.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3379 2023-09-19 20:44:35.532225 trame-components-2.2.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2606 2023-09-19 20:44:15.000000 trame-components-2.2.1/README.rst
--rw-r--r--   0 root         (0) root         (0)      916 2023-09-19 20:44:35.532225 trame-components-2.2.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       38 2023-09-19 20:44:15.000000 trame-components-2.2.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 20:44:35.528225 trame-components-2.2.1/trame/
--rw-r--r--   0 root         (0) root         (0)       65 2023-09-19 20:44:15.000000 trame-components-2.2.1/trame/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 20:44:35.528225 trame-components-2.2.1/trame/modules/
--rw-r--r--   0 root         (0) root         (0)       65 2023-09-19 20:44:15.000000 trame-components-2.2.1/trame/modules/__init__.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-09-19 20:44:15.000000 trame-components-2.2.1/trame/modules/trame.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 20:44:35.528225 trame-components-2.2.1/trame/widgets/
--rw-r--r--   0 root         (0) root         (0)       65 2023-09-19 20:44:15.000000 trame-components-2.2.1/trame/widgets/__init__.py
--rw-r--r--   0 root         (0) root         (0)      145 2023-09-19 20:44:15.000000 trame-components-2.2.1/trame/widgets/trame.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 20:44:35.532225 trame-components-2.2.1/trame_components/
--rw-r--r--   0 root         (0) root         (0)      552 2023-09-19 20:44:15.000000 trame-components-2.2.1/trame_components/LICENSE
--rw-r--r--   0 root         (0) root         (0)       98 2023-09-19 20:44:15.000000 trame-components-2.2.1/trame_components/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 20:44:35.532225 trame-components-2.2.1/trame_components/module/
--rw-r--r--   0 root         (0) root         (0)      388 2023-09-19 20:44:15.000000 trame-components-2.2.1/trame_components/module/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 20:44:35.532225 trame-components-2.2.1/trame_components/module/serve/
--rw-r--r--   0 root         (0) root         (0)   222603 2023-09-19 20:44:30.000000 trame-components-2.2.1/trame_components/module/serve/trame-components.umd.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 20:44:35.532225 trame-components-2.2.1/trame_components/widgets/
--rw-r--r--   0 root         (0) root         (0)        0 2023-09-19 20:44:15.000000 trame-components-2.2.1/trame_components/widgets/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15306 2023-09-19 20:44:15.000000 trame-components-2.2.1/trame_components/widgets/trame.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-19 20:44:35.532225 trame-components-2.2.1/trame_components.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3379 2023-09-19 20:44:35.000000 trame-components-2.2.1/trame_components.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      579 2023-09-19 20:44:35.000000 trame-components-2.2.1/trame_components.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-09-19 20:44:35.000000 trame-components-2.2.1/trame_components.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-09-19 20:44:35.000000 trame-components-2.2.1/trame_components.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       23 2023-09-19 20:44:35.000000 trame-components-2.2.1/trame_components.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 00:01:04.958520 trame-components-2.3.0/
+-rw-r--r--   0 root         (0) root         (0)      552 2024-04-16 00:00:48.000000 trame-components-2.3.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       69 2024-04-16 00:00:48.000000 trame-components-2.3.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3379 2024-04-16 00:01:04.958520 trame-components-2.3.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2606 2024-04-16 00:00:48.000000 trame-components-2.3.0/README.rst
+-rw-r--r--   0 root         (0) root         (0)      916 2024-04-16 00:01:04.958520 trame-components-2.3.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-16 00:00:48.000000 trame-components-2.3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 00:01:04.954520 trame-components-2.3.0/trame/
+-rw-r--r--   0 root         (0) root         (0)       65 2024-04-16 00:00:48.000000 trame-components-2.3.0/trame/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 00:01:04.954520 trame-components-2.3.0/trame/modules/
+-rw-r--r--   0 root         (0) root         (0)       65 2024-04-16 00:00:48.000000 trame-components-2.3.0/trame/modules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-16 00:00:48.000000 trame-components-2.3.0/trame/modules/trame.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 00:01:04.958520 trame-components-2.3.0/trame/widgets/
+-rw-r--r--   0 root         (0) root         (0)       65 2024-04-16 00:00:48.000000 trame-components-2.3.0/trame/widgets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      145 2024-04-16 00:00:48.000000 trame-components-2.3.0/trame/widgets/trame.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 00:01:04.958520 trame-components-2.3.0/trame_components/
+-rw-r--r--   0 root         (0) root         (0)      552 2024-04-16 00:00:48.000000 trame-components-2.3.0/trame_components/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       98 2024-04-16 00:00:48.000000 trame-components-2.3.0/trame_components/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 00:01:04.958520 trame-components-2.3.0/trame_components/module/
+-rw-r--r--   0 root         (0) root         (0)      388 2024-04-16 00:00:48.000000 trame-components-2.3.0/trame_components/module/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 00:01:04.958520 trame-components-2.3.0/trame_components/module/serve/
+-rw-r--r--   0 root         (0) root         (0)   227244 2024-04-16 00:01:01.000000 trame-components-2.3.0/trame_components/module/serve/trame-components.umd.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 00:01:04.958520 trame-components-2.3.0/trame_components/widgets/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-16 00:00:48.000000 trame-components-2.3.0/trame_components/widgets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15929 2024-04-16 00:00:48.000000 trame-components-2.3.0/trame_components/widgets/trame.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 00:01:04.958520 trame-components-2.3.0/trame_components.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3379 2024-04-16 00:01:04.000000 trame-components-2.3.0/trame_components.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      579 2024-04-16 00:01:04.000000 trame-components-2.3.0/trame_components.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-16 00:01:04.000000 trame-components-2.3.0/trame_components.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2024-04-16 00:01:04.000000 trame-components-2.3.0/trame_components.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2024-04-16 00:01:04.000000 trame-components-2.3.0/trame_components.egg-info/top_level.txt
```

### Comparing `trame-components-2.2.1/LICENSE` & `trame-components-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trame-components-2.2.1/PKG-INFO` & `trame-components-2.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trame-components
-Version: 2.2.1
+Version: 2.3.0
 Summary: Core components for trame widgets
 Author: Kitware Inc.
 License: Apache License 2.0
 Keywords: Python,Interactive,Web,Application,Framework
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `trame-components-2.2.1/README.rst` & `trame-components-2.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `trame-components-2.2.1/setup.cfg` & `trame-components-2.3.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = trame-components
-version = 2.2.1
+version = 2.3.0
 description = Core components for trame widgets
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 author = Kitware Inc.
 license = Apache License 2.0
 classifiers = 
 	Development Status :: 5 - Production/Stable
```

### Comparing `trame-components-2.2.1/trame_components/LICENSE` & `trame-components-2.3.0/trame_components/LICENSE`

 * *Files identical despite different names*

### Comparing `trame-components-2.2.1/trame_components/module/serve/trame-components.umd.js` & `trame-components-2.3.0/trame_components/module/serve/trame-components.umd.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -1,15 +1,15 @@
-(function(C0, G0) {
-    typeof exports == "object" && typeof module < "u" ? G0(exports) : typeof define == "function" && define.amd ? define(["exports"], G0) : (C0 = typeof globalThis < "u" ? globalThis : C0 || self, G0(C0.trame_components = {}))
-})(this, function(C0) {
+(function(b0, k0) {
+    typeof exports == "object" && typeof module < "u" ? k0(exports) : typeof define == "function" && define.amd ? define(["exports"], k0) : (b0 = typeof globalThis < "u" ? globalThis : b0 || self, k0(b0.trame_components = {}))
+})(this, function(b0) {
     "use strict";
     const {
-        watch: G0,
-        nextTick: a9
-    } = window.Vue, o9 = {
+        watch: k0,
+        nextTick: s9
+    } = window.Vue, c9 = {
         props: {
             value: {
                 type: String
             },
             immediate: {
                 type: Boolean,
                 default: !1
@@ -19,82 +19,82 @@
                 default: !1
             }
         },
         emits: ["change"],
         setup(e, {
             emit: t
         }) {
-            G0(() => e.value, r => {
-                e.immediate ? t("change", r) : a9(() => {
+            k0(() => e.value, r => {
+                e.immediate ? t("change", r) : s9(() => {
                     t("change", r)
                 })
             }), e.triggerChangeOnCreate && t("change", e.value)
         }
     }, {
-        onMounted: i9,
-        onBeforeUnmount: u9
-    } = window.Vue, s9 = {
+        onMounted: l9,
+        onBeforeUnmount: f9
+    } = window.Vue, g9 = {
         emits: ["mounted", "created", "beforeDestroy", "beforeUnmount"],
         setup(e, {
             emit: t,
             expose: r
         }) {
             function n(a, o) {
                 t(a, o)
             }
-            return i9(() => t("mounted")), u9(() => {
+            return l9(() => t("mounted")), f9(() => {
                 t("beforeDestroy"), t("beforeUnmount")
             }), r({
                 emit: n
             }), t("created"), {
                 emit: n
             }
         }
     }, {
-        ref: c9,
-        computed: f9,
-        watch: l9,
-        onMounted: p9,
-        onBeforeUnmount: g9
-    } = window.Vue, v9 = {
+        ref: p9,
+        computed: v9,
+        watch: y9,
+        onMounted: d9,
+        onBeforeUnmount: h9
+    } = window.Vue, m9 = {
         props: {
             active: {
                 type: Number,
                 default: 0
             },
             cursors: {
                 type: Array,
                 default: () => ["default", "wait"]
             }
         },
         setup(e) {
-            const t = c9(null);
+            const t = p9(null);
 
             function r(a) {
                 var o;
                 (o = t.value) != null && o.parentElement && (t.value.parentElement.style.cursor = a)
             }
-            const n = f9(() => e.cursors[e.active] || "default");
-            return l9(() => n.value, r), p9(() => r(n.value)), g9(() => r("default")), {
+            const n = v9(() => e.cursors[e.active] || "default");
+            return y9(() => n.value, r), d9(() => r(n.value)), h9(() => r("default")), {
                 elem: t,
                 activeCursor: n,
                 updateCursor: r
             }
         },
         template: '<div ref="elem" style="display: none"></div>'
     }, {
-        ref: D1,
-        watch: y9,
-        computed: L1
-    } = window.Vue, d9 = {
+        ref: $1,
+        watch: C9,
+        computed: j1
+    } = window.Vue, S9 = {
         top: "horizontal",
         bottom: "horizontal",
         left: "vertical",
         right: "vertical"
-    }, h9 = {
+    }, w9 = {
         props: {
             handleColor: {
                 type: String,
                 default: "#aaa"
             },
             handlePosition: {
                 type: String,
@@ -177,58 +177,58 @@
                 default: !1
             },
             width: {
                 type: [Number, String]
             }
         },
         setup(e) {
-            const t = D1(e.location[0]),
-                r = D1(e.location[1]);
+            const t = $1(e.location[0]),
+                r = $1(e.location[1]);
             let n = null,
                 a = 0,
                 o = 0,
                 c = !1;
 
             function s() {
-                c = !1, document.removeEventListener("mouseup", s), document.removeEventListener("mousemove", i)
+                c = !1, document.removeEventListener("mouseup", s), document.removeEventListener("mousemove", u)
             }
 
-            function i(f) {
-                c && (f.preventDefault(), r.value = f.clientY + o, t.value = f.clientX + a)
+            function u(l) {
+                c && (l.preventDefault(), r.value = l.clientY + o, t.value = l.clientX + a)
             }
 
-            function u(f) {
-                a = t.value - f.clientX, o = r.value - f.clientY, c = !0, document.addEventListener("mouseup", s), document.addEventListener("mousemove", i)
+            function i(l) {
+                a = t.value - l.clientX, o = r.value - l.clientY, c = !0, document.addEventListener("mouseup", s), document.addEventListener("mousemove", u)
             }
-            y9(() => e.location, f => {
-                n !== JSON.stringify(f) && ([t.value, r.value] = f, n = JSON.stringify(f))
+            C9(() => e.location, l => {
+                n !== JSON.stringify(l) && ([t.value, r.value] = l, n = JSON.stringify(l))
             });
-            const l = L1(() => ({
+            const f = j1(() => ({
                     zIndex: 100,
                     position: "fixed",
                     top: `${r.value}px`,
                     left: `${t.value}px`
                 })),
-                p = L1(() => {
-                    const f = {
+                g = j1(() => {
+                    const l = {
                         position: "absolute",
                         cursor: "grab",
                         backgroundImage: `radial-gradient(${e.handleColor} 25%, transparent 20%), radial-gradient(${e.handleColor} 25%, transparent 20%)`,
                         backgroundPosition: `-${e.handleSize/12}px 0, ${e.handleSize/6}px ${e.handleSize/4}px`,
                         backgroundSize: `${e.handleSize/2}px ${e.handleSize/2}px`,
                         backgroundRepeat: `repeat, repeat-${e.handlePosition in["top","bottom"]?"x":"y"}`
                     };
-                    return d9[e.handlePosition] === "horizontal" ? (f.backgroundRepeat = "repeat, repeat-x", f.left = 0, f.width = `calc(100% - ${e.handleSize/3}px)`, f.height = `${e.handleSize}px`, f.margin = `0 ${e.handleSize/6}px`) : (f.backgroundRepeat = "repeat, repeat-y", f.top = 0, f.height = `calc(100% - ${e.handleSize/3}px)`, f.width = `${e.handleSize}px`, f.margin = `${e.handleSize/6}px 0`), e.handlePosition == "top" && (f.top = 0), e.handlePosition == "bottom" && (f.bottom = 0), e.handlePosition == "left" && (f.left = 0), e.handlePosition == "right" && (f.right = 0), f
+                    return S9[e.handlePosition] === "horizontal" ? (l.backgroundRepeat = "repeat, repeat-x", l.left = 0, l.width = `calc(100% - ${e.handleSize/3}px)`, l.height = `${e.handleSize}px`, l.margin = `0 ${e.handleSize/6}px`) : (l.backgroundRepeat = "repeat, repeat-y", l.top = 0, l.height = `calc(100% - ${e.handleSize/3}px)`, l.width = `${e.handleSize}px`, l.margin = `${e.handleSize/6}px 0`), e.handlePosition == "top" && (l.top = 0), e.handlePosition == "bottom" && (l.bottom = 0), e.handlePosition == "left" && (l.left = 0), e.handlePosition == "right" && (l.right = 0), l
                 });
             return {
                 left: t,
                 top: r,
-                positionStyle: l,
-                handleStyle: p,
-                onMouseDown: u
+                positionStyle: f,
+                handleStyle: g,
+                onMouseDown: i
             }
         },
         template: `
     <v-card
       :style="positionStyle"
       :color="color"
       :dark="dark"
@@ -252,26 +252,26 @@
       :width="width"
     >
       <div @mousedown="onMouseDown" :style="handleStyle" />
       <slot></slot>
     </v-card>
     `
     }, {
-        ref: E0,
-        toRefs: m9,
-        watch: P1,
-        computed: Q0,
-        onMounted: C9
+        ref: D0,
+        toRefs: b9,
+        watch: U1,
+        computed: t1,
+        onMounted: N9
     } = window.Vue;
 
-    function _1(e, t) {
+    function F1(e, t) {
         return Number(e.id) - Number(t.id)
     }
 
-    function S9(e, t) {
+    function B9(e, t) {
         const r = {
             tree: {
                 [t]: []
             },
             map: {},
             leaves: [],
             rootId: t,
@@ -280,91 +280,91 @@
             forks: [],
             branches: [],
             actives: []
         };
         return e.forEach(n => {
             const a = Object.assign({}, n);
             ({}).hasOwnProperty.call(r.tree, a.parent) ? r.tree[a.parent].push(a) : r.tree[a.parent] = [a], r.map[a.id] = a
-        }), r.tree[t].sort(_1), r
+        }), r.tree[t].sort(F1), r
     }
 
-    function $1(e, t, r) {
+    function V1(e, t, r) {
         const n = e.tree[t.id];
-        t.x = r, t.y = e.y, e.y += 1, e.nodes.push(t), !n || n.length === 0 ? e.leaves.push(t) : (n.sort(_1), n.forEach((a, o) => {
-            $1(e, a, r + n.length - (o + 1))
+        t.x = r, t.y = e.y, e.y += 1, e.nodes.push(t), !n || n.length === 0 ? e.leaves.push(t) : (n.sort(F1), n.forEach((a, o) => {
+            V1(e, a, r + n.length - (o + 1))
         }))
     }
 
-    function w9(e, t) {
+    function x9(e, t) {
         const {
             x: r,
             y: n
         } = t, {
             rootId: a,
             map: o,
             branches: c,
             forks: s
-        } = e, i = {
+        } = e, u = {
             x: r,
             y: n
         };
-        let u = t;
-        for (; u.parent !== a && o[u.parent].x === i.x;) i.color || (i.color = u.color), u = o[u.parent], i.to = u.y;
-        typeof i.to < "u" && i.to !== i.y && c.push(i), u.parent !== a && s.push({
-            x: o[u.parent].x,
-            y: o[u.parent].y,
-            toX: u.x,
-            toY: u.y,
-            color: u.color
+        let i = t;
+        for (; i.parent !== a && o[i.parent].x === u.x;) u.color || (u.color = i.color), i = o[i.parent], u.to = i.y;
+        typeof u.to < "u" && u.to !== u.y && c.push(u), i.parent !== a && s.push({
+            x: o[i.parent].x,
+            y: o[i.parent].y,
+            toX: i.x,
+            toY: i.y,
+            color: i.color
         })
     }
 
-    function b9(e, t = []) {
+    function R9(e, t = []) {
         const {
             nodes: r,
             actives: n
         } = e;
         r.forEach(a => {
             t.indexOf(a.id) !== -1 && n.push(a.y)
         })
     }
 
-    function N9(e, t = [], r = "0") {
-        const n = S9(e, r),
+    function O9(e, t = [], r = "0") {
+        const n = B9(e, r),
             {
                 tree: a,
                 leaves: o,
                 rootId: c
             } = n,
             {
                 nodes: s,
-                branches: i,
-                forks: u,
-                actives: l
+                branches: u,
+                forks: i,
+                actives: f
             } = n;
-        return a[c].forEach(p => $1(n, p, 0)), b9(n, t), o.forEach(p => w9(n, p)), u.sort((p, f) => p.toX > f.toX), {
+        return a[c].forEach(g => V1(n, g, 0)), R9(n, t), o.forEach(g => x9(n, g)), i.sort((g, l) => g.toX > l.toX), {
             nodes: s,
-            branches: i,
-            forks: u,
-            actives: l,
+            branches: u,
+            forks: i,
+            actives: f,
             leaves: o
         }
     }
 
-    function B9(e, t, r, n, a) {
+    function T9(e, t, r, n, a) {
         const o = .5 * (Number(r) - Number(n));
         return (c, s) => ({
             name: c,
             x: t - 1.1 * n * (s + 1),
             y: Number(e) + o,
             size: n,
             href: a[c]
         })
     }
-    const R9 = {
+    const M9 = {
             props: {
                 sources: {
                     type: Array,
                     default: () => []
                 },
                 actives: {
                     type: Array,
@@ -443,141 +443,141 @@
                 }
             },
             emits: ["activesChange", "visibilityChange", "action"],
             setup(e, {
                 emit: t,
                 expose: r
             }) {
-                const n = E0(null),
-                    a = E0([]),
-                    o = E0([]),
-                    c = E0([]),
-                    s = E0([]);
+                const n = D0(null),
+                    a = D0([]),
+                    o = D0([]),
+                    c = D0([]),
+                    s = D0([]);
 
-                function i() {
+                function u() {
                     const {
                         nodes: h,
                         branches: C,
                         forks: N,
-                        actives: R
-                    } = N9(e.sources, e.actives, e.rootId);
-                    a.value = h, o.value = C, c.value = N, s.value = R
+                        actives: x
+                    } = O9(e.sources, e.actives, e.rootId);
+                    a.value = h, o.value = C, c.value = N, s.value = x
                 }
 
-                function u(h) {
+                function i(h) {
                     const {
                         actives: C,
                         deltaY: N,
-                        multiselect: R
+                        multiselect: x
                     } = e, B = C.slice();
                     if (h.target.nodeName !== "circle") {
-                        const w = n.value.getClientRects()[0],
-                            S = w.y || w.top,
-                            b = Math.floor((h.clientY - S) / N),
-                            v = C.indexOf(b);
-                        R && (h.metaKey || h.ctrlKey) ? (v === -1 ? B.push(b) : B.splice(v, 1), s.value = B, t("activesChange", s.value.map(d => a.value[d].id))) : (B[0] = b, s.value = B, t("activesChange", s.value.map(d => a.value[d].id)))
+                        const b = n.value.getClientRects()[0],
+                            S = b.y || b.top,
+                            w = Math.floor((h.clientY - S) / N),
+                            v = C.indexOf(w);
+                        x && (h.metaKey || h.ctrlKey) ? (v === -1 ? B.push(w) : B.splice(v, 1), s.value = B, t("activesChange", s.value.map(d => a.value[d].id))) : (B[0] = w, s.value = B, t("activesChange", s.value.map(d => a.value[d].id)))
                     }
                 }
 
-                function l(h) {
+                function f(h) {
                     const C = parseInt(h.currentTarget.dataset.id, 10),
                         N = Object.assign({}, a.value[C]);
-                    N.visible = !N.visible, a.value = a.value.map((R, B) => B === C ? N : R), t("visibilityChange", {
+                    N.visible = !N.visible, a.value = a.value.map((x, B) => B === C ? N : x), t("visibilityChange", {
                         id: N.id,
                         visible: N.visible
                     })
                 }
 
-                function p(h) {
+                function g(h) {
                     const C = parseInt(h.currentTarget.dataset.id, 10),
                         N = h.currentTarget.dataset.name,
                         {
-                            id: R
+                            id: x
                         } = a.value[C];
                     t("action", {
-                        id: R,
+                        id: x,
                         action: N
                     })
                 }
-                P1(() => e.sources, i), P1(() => e.actives, i);
-                const f = Q0(() => o.value.map((h, C) => {
+                U1(() => e.sources, u), U1(() => e.actives, u);
+                const l = t1(() => o.value.map((h, C) => {
                         const N = e.deltaX * h.x + e.offset,
-                            R = e.deltaY * h.y + e.deltaY / 2,
+                            x = e.deltaY * h.y + e.deltaY / 2,
                             B = e.deltaY * h.to + e.deltaY / 2,
-                            w = h.color || e.palette[h.x % e.palette.length];
+                            b = h.color || e.palette[h.x % e.palette.length];
                         return {
                             key: `branch-${C}`,
-                            d: `M${N},${R} L${N},${B}`,
-                            stroke: w
+                            d: `M${N},${x} L${N},${B}`,
+                            stroke: b
                         }
                     })),
-                    g = Q0(() => c.value.map((h, C) => {
+                    p = t1(() => c.value.map((h, C) => {
                         const N = e.deltaX * h.x + e.offset,
-                            R = e.deltaY * h.y + e.deltaY / 2 + e.radius,
+                            x = e.deltaY * h.y + e.deltaY / 2 + e.radius,
                             B = e.deltaX * h.toX + e.offset,
-                            w = e.deltaY * h.toY + e.deltaY / 2 + e.radius,
+                            b = e.deltaY * h.toY + e.deltaY / 2 + e.radius,
                             S = h.color || e.palette[h.toX % e.palette.length],
-                            b = `M${N},${R} Q${N},${R+e.deltaY/3},${(N+B)/2},${R+e.deltaY/3} T${B},${R+e.deltaY} L${B},${w}`;
+                            w = `M${N},${x} Q${N},${x+e.deltaY/3},${(N+B)/2},${x+e.deltaY/3} T${B},${x+e.deltaY} L${B},${b}`;
                         return {
                             key: `fork-${C}`,
-                            d: b,
+                            d: w,
                             stroke: S
                         }
                     })),
-                    y = Q0(() => a.value.map((h, C) => {
+                    y = t1(() => a.value.map((h, C) => {
                         const N = s.value.includes(C),
-                            R = !!h.visible,
+                            x = !!h.visible,
                             B = h.color || e.palette[h.x % e.palette.length],
-                            w = e.textColor[N ? 1 : 0],
+                            b = e.textColor[N ? 1 : 0],
                             S = e.textWeight[N ? 1 : 0],
-                            b = N ? e.activeCircleStrokeColor : B || B,
-                            v = R ? B : e.notVisibleCircleFillColor || B,
+                            w = N ? e.activeCircleStrokeColor : B || B,
+                            v = x ? B : e.notVisibleCircleFillColor || B,
                             d = e.deltaX * h.x + e.offset,
                             m = e.deltaY * h.y + e.deltaY / 2,
-                            x = d + e.radius * 2,
+                            O = d + e.radius * 2,
                             D = m + (e.radius - 1),
-                            P = (h.actions || []).map(B9(e.deltaY * h.y, e.width, e.deltaY, e.actionSize, e.actionMap));
+                            _ = (h.actions || []).map(T9(e.deltaY * h.y, e.width, e.deltaY, e.actionSize, e.actionMap));
                         return {
                             key: `node-${C}`,
                             id: h.y,
                             circle: {
                                 cx: d,
                                 cy: m,
                                 radius: e.radius,
-                                stroke: b,
+                                stroke: w,
                                 fill: v
                             },
                             text: {
-                                x,
+                                x: O,
                                 y: D,
-                                fill: w,
+                                fill: b,
                                 fontWeight: S,
                                 fontSize: e.fontSize,
                                 content: h.name
                             },
-                            actions: P
+                            actions: _
                         }
                     }));
-                return C9(i), r({
-                    toggleActive: u,
-                    toggleVisibility: l,
-                    triggerAction: p
+                return N9(u), r({
+                    toggleActive: i,
+                    toggleVisibility: f,
+                    triggerAction: g
                 }), {
                     elem: n,
-                    ...m9(e),
+                    ...b9(e),
                     nodes: a,
                     branches: o,
                     forks: c,
                     activesToRender: s,
-                    branchesToRender: f,
-                    forksToRender: g,
+                    branchesToRender: l,
+                    forksToRender: p,
                     nodesToRender: y,
-                    toggleActive: u,
-                    toggleVisibility: l,
-                    triggerAction: p
+                    toggleActive: i,
+                    toggleVisibility: f,
+                    triggerAction: g
                 }
             },
             template: `
     <svg
     :width="width"
     :height="deltaY * nodes.length"
     v-on:click="toggleActive"
@@ -661,28 +661,28 @@
         @click="triggerAction"
       />
     </g>
   </svg>  
     `
         },
         {
-            onMounted: x9,
-            onBeforeUnmount: O9
+            onMounted: G9,
+            onBeforeUnmount: E9
         } = window.Vue,
-        k0 = () => {},
-        j1 = {
-            created: k0,
-            beforeMount: k0,
-            mounted: x9,
-            beforeUpdate: k0,
-            updated: k0,
-            beforeDestroy: O9,
-            destroyed: k0
+        L0 = () => {},
+        z1 = {
+            created: L0,
+            beforeMount: L0,
+            mounted: G9,
+            beforeUpdate: L0,
+            updated: L0,
+            beforeDestroy: E9,
+            destroyed: L0
         },
-        T9 = {
+        k9 = {
             props: {
                 name: {
                     type: String,
                     default: "TrameLifeCycleMonitor"
                 },
                 type: {
                     type: String,
@@ -693,37 +693,37 @@
                     default: "value"
                 },
                 events: {
                     type: Array,
                     default: () => ["created", "beforeMount", "mounted", "beforeUpdate", "updated", "beforeDestroy", "destroyed"]
                 }
             },
-            emits: Object.keys(j1),
+            emits: Object.keys(z1),
             setup(e, {
                 emit: t
             }) {
                 for (let r = 0; r < e.events.length; r++) {
                     const n = e.events[r],
-                        a = j1[n];
+                        a = z1[n];
                     a(() => {
                         e.type === "emit" ? t(n, {
                             name: e.name,
                             value: e.value
                         }) : console[e.type](e.name, n, e.value)
                     })
                 }
             }
         },
         {
-            ref: U1,
-            computed: F1,
-            version: Z0
+            ref: H1,
+            computed: I1,
+            version: r1
         } = window.Vue,
-        M9 = Z0[0] === "2" ? "v-text" : ":icon",
-        G9 = Z0[0] === "2" ? `
+        D9 = r1[0] === "2" ? "v-text" : ":icon",
+        L9 = r1[0] === "2" ? `
   <v-list-item-icon v-if="item.prependIcon">
       <v-icon v-text="item.prependIcon"/>
   </v-list-item-icon>
   <v-list-item-content>
       <v-list-item-title v-text="item.text" />
   </v-list-item-content>
   <v-list-item-icon v-if="item.appendIcon">
@@ -734,15 +734,15 @@
     <v-icon :icon="item.prependIcon"></v-icon>
   </template>
   <v-list-item-title v-text="item.text"></v-list-item-title>
   <template v-slot:append v-if="item.appendIcon">
     <v-icon :icon="item.appendIcon"></v-icon>
   </template>
 `,
-        E9 = Z0[0] === "2" ? `<v-text-field
+        A9 = r1[0] === "2" ? `<v-text-field
         name="filter-algo"
         v-model="filterText"
         label="Filter"
         clearable
         class="mx-3"
         :prepend-inner-icon="filterIcon"
         dense
@@ -760,15 +760,15 @@
           :prepend-inner-icon="filterIcon"
           dense="compact"
           filled
           single-line
           variant="outlined"
           hide-details
       />`,
-        k9 = {
+        P9 = {
             props: {
                 pathIcon: {
                     type: String,
                     default: "mdi-folder-outline"
                 },
                 pathSelectedIcon: {
                     type: String,
@@ -792,43 +792,43 @@
                     type: String
                 }
             },
             emits: ["click"],
             setup(e, {
                 emit: t
             }) {
-                const r = U1(""),
-                    n = U1(-1),
-                    a = F1(() => e.filterQuery ? e.filterQuery.toLowerCase().split(" ") : r.value ? r.value.toLowerCase().split(" ") : []),
-                    o = F1(() => e.path.slice(n.value)[0]);
+                const r = H1(""),
+                    n = H1(-1),
+                    a = I1(() => e.filterQuery ? e.filterQuery.toLowerCase().split(" ") : r.value ? r.value.toLowerCase().split(" ") : []),
+                    o = I1(() => e.path.slice(n.value)[0]);
                 return {
                     filterText: r,
                     activeFolderIndex: n,
                     filterValues: a,
                     activeFolderName: o,
                     ...{
                         show(s) {
                             if (!a.value.length) return !0;
-                            const i = [s.text.toLowerCase(), s.type.toLowerCase()].join("  "),
-                                u = a.value;
-                            for (let l = 0; l < u.length; l++)
-                                if (!i.includes(u[l])) return !1;
+                            const u = [s.text.toLowerCase(), s.type.toLowerCase()].join("  "),
+                                i = a.value;
+                            for (let f = 0; f < i.length; f++)
+                                if (!u.includes(i[f])) return !1;
                             return !0
                         },
                         goToPath(s) {
                             t("click", {
                                 type: "path",
                                 value: e.path.slice(0, s + 1).join("/")
                             })
                         },
                         selectItem(s) {
-                            const i = e.list[s];
+                            const u = e.list[s];
                             t("click", {
-                                type: i.type || "item",
-                                value: i.value || s
+                                type: u.type || "item",
+                                value: u.value || s
                             })
                         },
                         activatePath(s) {
                             n.value = s
                         },
                         deactivatePath() {
                             n.value = -1
@@ -840,42 +840,42 @@
     <v-col class="pa-0">
         <v-divider v-if="path" class="mb-3" />
         <v-row v-if="path" class="mx-2 py-2 rounded-0 align-center">
             <div v-for="item, idx in path" :key="idx" class="d-flex">
                 <span v-if="idx">></span>
                 <v-icon
                     class="mx-1"
-                    ${M9}="activeFolderIndex === idx ? pathSelectedIcon : pathIcon"
+                    ${D9}="activeFolderIndex === idx ? pathSelectedIcon : pathIcon"
                     @click="goToPath(idx)"
                     @mouseenter="activatePath(idx)"
                     @mouseleave="deactivatePath"
                 />
             </div>
             <div class="text-truncate text-body-2 pl-1">{{ activeFolderName }}</div>
         </v-row>
         <v-divider v-if="path" class="mt-3" />
         <v-row v-if="filter" class="px-2 py-0 ma-0" :class="{ 'mt-3': path }">
-            ${E9}
+            ${A9}
         </v-row>
         <v-list dense v-if="list" class="overflow-y-auto" fill-height>
             <v-list-item
                 v-for="(item, i) in list"
                 :key="i"
                 @click="selectItem(i)"
                 v-show="show(item)"
             >
-              ${G9}
+              ${L9}
             </v-list-item>
         </v-list>
     </v-col>
     `
         };
-    var q = typeof globalThis < "u" ? globalThis : typeof window < "u" ? window : typeof global < "u" ? global : typeof self < "u" ? self : {};
+    var e0 = typeof globalThis < "u" ? globalThis : typeof window < "u" ? window : typeof global < "u" ? global : typeof self < "u" ? self : {};
 
-    function A9(e) {
+    function _9(e) {
         if (e.__esModule) return e;
         var t = e.default;
         if (typeof t == "function") {
             var r = function n() {
                 if (this instanceof n) {
                     var a = [null];
                     a.push.apply(a, arguments);
@@ -894,21 +894,21 @@
                 enumerable: !0,
                 get: function() {
                     return e[n]
                 }
             })
         }), r
     }
-    var e1 = {},
-        D9 = {
+    var n1 = {},
+        $9 = {
             get exports() {
-                return e1
+                return n1
             },
             set exports(e) {
-                e1 = e
+                n1 = e
             }
         };
     (function(e) {
         (function(t, r, n) {
             if (!t) return;
             for (var a = {
                     8: "backspace",
@@ -973,38 +973,38 @@
                 }, s = {
                     option: "alt",
                     command: "meta",
                     return: "enter",
                     escape: "esc",
                     plus: "+",
                     mod: /Mac|iPod|iPhone|iPad/.test(navigator.platform) ? "meta" : "ctrl"
-                }, i, u = 1; u < 20; ++u) a[111 + u] = "f" + u;
-            for (u = 0; u <= 9; ++u) a[u + 96] = u.toString();
+                }, u, i = 1; i < 20; ++i) a[111 + i] = "f" + i;
+            for (i = 0; i <= 9; ++i) a[i + 96] = i.toString();
 
-            function l(v, d, m) {
+            function f(v, d, m) {
                 if (v.addEventListener) {
                     v.addEventListener(d, m, !1);
                     return
                 }
                 v.attachEvent("on" + d, m)
             }
 
-            function p(v) {
+            function g(v) {
                 if (v.type == "keypress") {
                     var d = String.fromCharCode(v.which);
                     return v.shiftKey || (d = d.toLowerCase()), d
                 }
                 return a[v.which] ? a[v.which] : o[v.which] ? o[v.which] : String.fromCharCode(v.which).toLowerCase()
             }
 
-            function f(v, d) {
+            function l(v, d) {
                 return v.sort().join(",") === d.sort().join(",")
             }
 
-            function g(v) {
+            function p(v) {
                 var d = [];
                 return v.shiftKey && d.push("shift"), v.altKey && d.push("alt"), v.ctrlKey && d.push("ctrl"), v.metaKey && d.push("meta"), d
             }
 
             function y(v) {
                 if (v.preventDefault) {
                     v.preventDefault();
@@ -1022,423 +1022,423 @@
             }
 
             function C(v) {
                 return v == "shift" || v == "ctrl" || v == "alt" || v == "meta"
             }
 
             function N() {
-                if (!i) {
-                    i = {};
-                    for (var v in a) v > 95 && v < 112 || a.hasOwnProperty(v) && (i[a[v]] = v)
+                if (!u) {
+                    u = {};
+                    for (var v in a) v > 95 && v < 112 || a.hasOwnProperty(v) && (u[a[v]] = v)
                 }
-                return i
+                return u
             }
 
-            function R(v, d, m) {
+            function x(v, d, m) {
                 return m || (m = N()[v] ? "keydown" : "keypress"), m == "keypress" && d.length && (m = "keydown"), m
             }
 
             function B(v) {
                 return v === "+" ? ["+"] : (v = v.replace(/\+{2}/g, "+plus"), v.split("+"))
             }
 
-            function w(v, d) {
-                var m, x, D, P = [];
-                for (m = B(v), D = 0; D < m.length; ++D) x = m[D], s[x] && (x = s[x]), d && d != "keypress" && c[x] && (x = c[x], P.push("shift")), C(x) && P.push(x);
-                return d = R(x, P, d), {
-                    key: x,
-                    modifiers: P,
+            function b(v, d) {
+                var m, O, D, _ = [];
+                for (m = B(v), D = 0; D < m.length; ++D) O = m[D], s[O] && (O = s[O]), d && d != "keypress" && c[O] && (O = c[O], _.push("shift")), C(O) && _.push(O);
+                return d = x(O, _, d), {
+                    key: O,
+                    modifiers: _,
                     action: d
                 }
             }
 
             function S(v, d) {
                 return v === null || v === r ? !1 : v === d ? !0 : S(v.parentNode, d)
             }
 
-            function b(v) {
+            function w(v) {
                 var d = this;
-                if (v = v || r, !(d instanceof b)) return new b(v);
+                if (v = v || r, !(d instanceof w)) return new w(v);
                 d.target = v, d._callbacks = {}, d._directMap = {};
                 var m = {},
-                    x, D = !1,
-                    P = !1,
+                    O, D = !1,
+                    _ = !1,
                     U = !1;
 
-                function H(T) {
-                    T = T || {};
-                    var G = !1,
-                        k;
-                    for (k in m) {
-                        if (T[k]) {
-                            G = !0;
+                function F(M) {
+                    M = M || {};
+                    var E = !1,
+                        A;
+                    for (A in m) {
+                        if (M[A]) {
+                            E = !0;
                             continue
                         }
-                        m[k] = 0
+                        m[A] = 0
                     }
-                    G || (U = !1)
+                    E || (U = !1)
                 }
 
-                function O(T, G, k, E, L, X) {
-                    var A, _, I = [],
-                        W = k.type;
-                    if (!d._callbacks[T]) return [];
-                    for (W == "keyup" && C(T) && (G = [T]), A = 0; A < d._callbacks[T].length; ++A)
-                        if (_ = d._callbacks[T][A], !(!E && _.seq && m[_.seq] != _.level) && W == _.action && (W == "keypress" && !k.metaKey && !k.ctrlKey || f(G, _.modifiers))) {
-                            var o0 = !E && _.combo == L,
-                                i0 = E && _.seq == E && _.level == X;
-                            (o0 || i0) && d._callbacks[T].splice(A, 1), I.push(_)
-                        } return I
-                }
-
-                function F(T, G, k, E) {
-                    d.stopCallback(G, G.target || G.srcElement, k, E) || T(G, k) === !1 && (y(G), h(G))
-                }
-                d._handleKey = function(T, G, k) {
-                    var E = O(T, G, k),
-                        L, X = {},
-                        A = 0,
-                        _ = !1;
-                    for (L = 0; L < E.length; ++L) E[L].seq && (A = Math.max(A, E[L].level));
-                    for (L = 0; L < E.length; ++L) {
-                        if (E[L].seq) {
-                            if (E[L].level != A) continue;
-                            _ = !0, X[E[L].seq] = 1, F(E[L].callback, k, E[L].combo, E[L].seq);
+                function T(M, E, A, k, $, Z) {
+                    var P, j, Y = [],
+                        X = A.type;
+                    if (!d._callbacks[M]) return [];
+                    for (X == "keyup" && C(M) && (E = [M]), P = 0; P < d._callbacks[M].length; ++P)
+                        if (j = d._callbacks[M][P], !(!k && j.seq && m[j.seq] != j.level) && X == j.action && (X == "keypress" && !A.metaKey && !A.ctrlKey || l(E, j.modifiers))) {
+                            var l0 = !k && j.combo == $,
+                                f0 = k && j.seq == k && j.level == Z;
+                            (l0 || f0) && d._callbacks[M].splice(P, 1), Y.push(j)
+                        } return Y
+                }
+
+                function L(M, E, A, k) {
+                    d.stopCallback(E, E.target || E.srcElement, A, k) || M(E, A) === !1 && (y(E), h(E))
+                }
+                d._handleKey = function(M, E, A) {
+                    var k = T(M, E, A),
+                        $, Z = {},
+                        P = 0,
+                        j = !1;
+                    for ($ = 0; $ < k.length; ++$) k[$].seq && (P = Math.max(P, k[$].level));
+                    for ($ = 0; $ < k.length; ++$) {
+                        if (k[$].seq) {
+                            if (k[$].level != P) continue;
+                            j = !0, Z[k[$].seq] = 1, L(k[$].callback, A, k[$].combo, k[$].seq);
                             continue
                         }
-                        _ || F(E[L].callback, k, E[L].combo)
+                        j || L(k[$].callback, A, k[$].combo)
                     }
-                    var I = k.type == "keypress" && P;
-                    k.type == U && !C(T) && !I && H(X), P = _ && k.type == "keydown"
+                    var Y = A.type == "keypress" && _;
+                    A.type == U && !C(M) && !Y && F(Z), _ = j && A.type == "keydown"
                 };
 
-                function J(T) {
-                    typeof T.which != "number" && (T.which = T.keyCode);
-                    var G = p(T);
-                    if (G) {
-                        if (T.type == "keyup" && D === G) {
+                function V(M) {
+                    typeof M.which != "number" && (M.which = M.keyCode);
+                    var E = g(M);
+                    if (E) {
+                        if (M.type == "keyup" && D === E) {
                             D = !1;
                             return
                         }
-                        d.handleKey(G, g(T), T)
+                        d.handleKey(E, p(M), M)
                     }
                 }
 
-                function u0() {
-                    clearTimeout(x), x = setTimeout(H, 1e3)
+                function Q() {
+                    clearTimeout(O), O = setTimeout(F, 1e3)
                 }
 
-                function M0(T, G, k, E) {
-                    m[T] = 0;
+                function K(M, E, A, k) {
+                    m[M] = 0;
 
-                    function L(W) {
+                    function $(X) {
                         return function() {
-                            U = W, ++m[T], u0()
+                            U = X, ++m[M], Q()
                         }
                     }
 
-                    function X(W) {
-                        F(k, W, T), E !== "keyup" && (D = p(W)), setTimeout(H, 10)
+                    function Z(X) {
+                        L(A, X, M), k !== "keyup" && (D = g(X)), setTimeout(F, 10)
                     }
-                    for (var A = 0; A < G.length; ++A) {
-                        var _ = A + 1 === G.length,
-                            I = _ ? X : L(E || w(G[A + 1]).action);
-                        h0(G[A], I, E, T, A)
+                    for (var P = 0; P < E.length; ++P) {
+                        var j = P + 1 === E.length,
+                            Y = j ? Z : $(k || b(E[P + 1]).action);
+                        a0(E[P], Y, k, M, P)
                     }
                 }
 
-                function h0(T, G, k, E, L) {
-                    d._directMap[T + ":" + k] = G, T = T.replace(/\s+/g, " ");
-                    var X = T.split(" "),
-                        A;
-                    if (X.length > 1) {
-                        M0(T, X, G, k);
+                function a0(M, E, A, k, $) {
+                    d._directMap[M + ":" + A] = E, M = M.replace(/\s+/g, " ");
+                    var Z = M.split(" "),
+                        P;
+                    if (Z.length > 1) {
+                        K(M, Z, E, A);
                         return
                     }
-                    A = w(T, k), d._callbacks[A.key] = d._callbacks[A.key] || [], O(A.key, A.modifiers, {
-                        type: A.action
-                    }, E, T, L), d._callbacks[A.key][E ? "unshift" : "push"]({
-                        callback: G,
-                        modifiers: A.modifiers,
-                        action: A.action,
-                        seq: E,
-                        level: L,
-                        combo: T
+                    P = b(M, A), d._callbacks[P.key] = d._callbacks[P.key] || [], T(P.key, P.modifiers, {
+                        type: P.action
+                    }, k, M, $), d._callbacks[P.key][k ? "unshift" : "push"]({
+                        callback: E,
+                        modifiers: P.modifiers,
+                        action: P.action,
+                        seq: k,
+                        level: $,
+                        combo: M
                     })
                 }
-                d._bindMultiple = function(T, G, k) {
-                    for (var E = 0; E < T.length; ++E) h0(T[E], G, k)
-                }, l(v, "keypress", J), l(v, "keydown", J), l(v, "keyup", J)
-            }
-            b.prototype.bind = function(v, d, m) {
-                var x = this;
-                return v = v instanceof Array ? v : [v], x._bindMultiple.call(x, v, d, m), x
-            }, b.prototype.unbind = function(v, d) {
+                d._bindMultiple = function(M, E, A) {
+                    for (var k = 0; k < M.length; ++k) a0(M[k], E, A)
+                }, f(v, "keypress", V), f(v, "keydown", V), f(v, "keyup", V)
+            }
+            w.prototype.bind = function(v, d, m) {
+                var O = this;
+                return v = v instanceof Array ? v : [v], O._bindMultiple.call(O, v, d, m), O
+            }, w.prototype.unbind = function(v, d) {
                 var m = this;
                 return m.bind.call(m, v, function() {}, d)
-            }, b.prototype.trigger = function(v, d) {
+            }, w.prototype.trigger = function(v, d) {
                 var m = this;
                 return m._directMap[v + ":" + d] && m._directMap[v + ":" + d]({}, v), m
-            }, b.prototype.reset = function() {
+            }, w.prototype.reset = function() {
                 var v = this;
                 return v._callbacks = {}, v._directMap = {}, v
-            }, b.prototype.stopCallback = function(v, d) {
+            }, w.prototype.stopCallback = function(v, d) {
                 var m = this;
                 if ((" " + d.className + " ").indexOf(" mousetrap ") > -1 || S(d, m.target)) return !1;
                 if ("composedPath" in v && typeof v.composedPath == "function") {
-                    var x = v.composedPath()[0];
-                    x !== v.target && (d = x)
+                    var O = v.composedPath()[0];
+                    O !== v.target && (d = O)
                 }
                 return d.tagName == "INPUT" || d.tagName == "SELECT" || d.tagName == "TEXTAREA" || d.isContentEditable
-            }, b.prototype.handleKey = function() {
+            }, w.prototype.handleKey = function() {
                 var v = this;
                 return v._handleKey.apply(v, arguments)
-            }, b.addKeycodes = function(v) {
+            }, w.addKeycodes = function(v) {
                 for (var d in v) v.hasOwnProperty(d) && (a[d] = v[d]);
-                i = null
-            }, b.init = function() {
-                var v = b(r);
-                for (var d in v) d.charAt(0) !== "_" && (b[d] = function(m) {
+                u = null
+            }, w.init = function() {
+                var v = w(r);
+                for (var d in v) d.charAt(0) !== "_" && (w[d] = function(m) {
                     return function() {
                         return v[m].apply(v, arguments)
                     }
                 }(d))
-            }, b.init(), t.Mousetrap = b, e.exports && (e.exports = b), typeof n == "function" && n.amd && n(function() {
-                return b
+            }, w.init(), t.Mousetrap = w, e.exports && (e.exports = w), typeof n == "function" && n.amd && n(function() {
+                return w
             })
         })(typeof window < "u" ? window : null, typeof window < "u" ? document : null)
-    })(D9);
-    const c0 = e1,
+    })($9);
+    const p0 = n1,
         {
-            watch: L9,
-            onBeforeUnmount: P9
+            watch: j9,
+            onBeforeUnmount: U9
         } = window.Vue,
-        _9 = {
+        F9 = {
             inject: ["trame"],
             props: {
                 mapping: {
                     type: Array
                 }
             },
             emits: [],
             setup(e, {
                 emit: t,
                 expose: r
             }) {
                 const n = {
                     bind(...o) {
-                        c0.bind(...o)
+                        p0.bind(...o)
                     },
                     unbind(o) {
-                        c0.unbind(o)
+                        p0.unbind(o)
                     },
                     trigger(o) {
-                        c0.trigger(o)
+                        p0.trigger(o)
                     },
                     addKeycodes(...o) {
-                        c0.trigger(...o)
+                        p0.trigger(...o)
                     }
                 };
 
                 function a() {
-                    e.mapping && (c0.reset(), e.mapping.forEach(({
+                    e.mapping && (p0.reset(), e.mapping.forEach(({
                         keys: o,
                         event: c,
                         stop: s,
-                        listen: i
+                        listen: u
                     }) => {
-                        c0.bind(o, u => {
-                            if (t(c, u), s) return !1
-                        }, i)
+                        p0.bind(o, i => {
+                            if (t(c, i), s) return !1
+                        }, u)
                     }))
                 }
-                return a(), L9(e.mapping, a), P9(() => {
-                    c0.reset()
+                return a(), j9(e.mapping, a), U9(() => {
+                    p0.reset()
                 }), r(n), n
             }
         },
         {
-            inject: $9,
-            ref: j9,
-            onMounted: U9,
-            onBeforeUnmount: F9
+            inject: V9,
+            ref: z9,
+            onMounted: H9,
+            onBeforeUnmount: I9
         } = window.Vue,
-        V9 = {
+        W9 = {
             props: {
                 name: {
                     type: String
                 }
             },
             emits: ["change"],
             setup(e, {
                 emit: t
             }) {
-                const r = $9("trame"),
-                    n = j9(null);
+                const r = V9("trame"),
+                    n = z9(null);
 
                 function a() {
                     const c = n.value.getBoundingClientRect(),
                         s = window.devicePixelRatio,
-                        i = 96 * s,
-                        u = {
+                        u = 96 * s,
+                        i = {
                             size: c,
                             pixelRatio: s,
-                            dpi: i
+                            dpi: u
                         };
-                    e.name && (u.name = e.name), r && r.state.set(e.name, u), t("change", u)
+                    e.name && (i.name = e.name), r && r.state.set(e.name, i), t("change", i)
                 }
                 const o = new ResizeObserver(a);
-                return U9(() => {
+                return H9(() => {
                     o.observe(n.value)
-                }), F9(() => {
+                }), I9(() => {
                     o.unobserve(n.value)
                 }), {
                     elem: n,
                     resize: a
                 }
             },
             template: '<div ref="elem" style="overflow: hidden; position: relative; width: 100%; height: 100%; margin: 0; padding: 0;"><slot></slot></div>'
         };
 
-    function f0(e, t, r) {
+    function v0(e, t, r) {
         return t in e ? Object.defineProperty(e, t, {
             value: r,
             enumerable: !0,
             configurable: !0,
             writable: !0
         }) : e[t] = r, e
     }
 
-    function z9(e) {
+    function Y9(e) {
         if (Array.isArray(e)) return e
     }
 
-    function H9(e, t) {
+    function X9(e, t) {
         var r = e == null ? null : typeof Symbol < "u" && e[Symbol.iterator] || e["@@iterator"];
         if (r != null) {
             var n = [],
                 a = !0,
                 o = !1,
                 c, s;
             try {
                 for (r = r.call(e); !(a = (c = r.next()).done) && (n.push(c.value), !(t && n.length === t)); a = !0);
-            } catch (i) {
-                o = !0, s = i
+            } catch (u) {
+                o = !0, s = u
             } finally {
                 try {
                     !a && r.return != null && r.return()
                 } finally {
                     if (o) throw s
                 }
             }
             return n
         }
     }
 
-    function t1(e, t) {
+    function a1(e, t) {
         (t == null || t > e.length) && (t = e.length);
         for (var r = 0, n = new Array(t); r < t; r++) n[r] = e[r];
         return n
     }
 
-    function V1(e, t) {
+    function W1(e, t) {
         if (e) {
-            if (typeof e == "string") return t1(e, t);
+            if (typeof e == "string") return a1(e, t);
             var r = Object.prototype.toString.call(e).slice(8, -1);
             if (r === "Object" && e.constructor && (r = e.constructor.name), r === "Map" || r === "Set") return Array.from(e);
-            if (r === "Arguments" || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(r)) return t1(e, t)
+            if (r === "Arguments" || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(r)) return a1(e, t)
         }
     }
 
-    function I9() {
+    function q9() {
         throw new TypeError(`Invalid attempt to destructure non-iterable instance.
 In order to be iterable, non-array objects must have a [Symbol.iterator]() method.`)
     }
 
-    function r0(e, t) {
-        return z9(e) || H9(e, t) || V1(e, t) || I9()
+    function u0(e, t) {
+        return Y9(e) || X9(e, t) || W1(e, t) || q9()
     }
 
-    function l0(e) {
-        return l0 = typeof Symbol == "function" && typeof Symbol.iterator == "symbol" ? function(t) {
+    function y0(e) {
+        return y0 = typeof Symbol == "function" && typeof Symbol.iterator == "symbol" ? function(t) {
             return typeof t
         } : function(t) {
             return t && typeof Symbol == "function" && t.constructor === Symbol && t !== Symbol.prototype ? "symbol" : typeof t
-        }, l0(e)
+        }, y0(e)
     }
 
-    function W9(e) {
-        if (Array.isArray(e)) return t1(e)
+    function K9(e) {
+        if (Array.isArray(e)) return a1(e)
     }
 
-    function Y9(e) {
+    function J9(e) {
         if (typeof Symbol < "u" && e[Symbol.iterator] != null || e["@@iterator"] != null) return Array.from(e)
     }
 
-    function X9() {
+    function Q9() {
         throw new TypeError(`Invalid attempt to spread non-iterable instance.
 In order to be iterable, non-array objects must have a [Symbol.iterator]() method.`)
     }
 
-    function r1(e) {
-        return W9(e) || Y9(e) || V1(e) || X9()
+    function o1(e) {
+        return K9(e) || J9(e) || W1(e) || Q9()
     }
 
     function A0(e, t) {
         return A0 = Object.setPrototypeOf || function(n, a) {
             return n.__proto__ = a, n
         }, A0(e, t)
     }
 
-    function q9() {
+    function Z9() {
         if (typeof Reflect > "u" || !Reflect.construct || Reflect.construct.sham) return !1;
         if (typeof Proxy == "function") return !0;
         try {
             return Boolean.prototype.valueOf.call(Reflect.construct(Boolean, [], function() {})), !0
         } catch {
             return !1
         }
     }
 
-    function D0(e, t, r) {
-        return q9() ? D0 = Reflect.construct : D0 = function(a, o, c) {
+    function P0(e, t, r) {
+        return Z9() ? P0 = Reflect.construct : P0 = function(a, o, c) {
             var s = [null];
             s.push.apply(s, o);
-            var i = Function.bind.apply(a, s),
-                u = new i;
-            return c && A0(u, c.prototype), u
-        }, D0.apply(null, arguments)
-    }
-    var z1 = Object.prototype.toString,
-        H1 = function(t) {
-            var r = z1.call(t),
+            var u = Function.bind.apply(a, s),
+                i = new u;
+            return c && A0(i, c.prototype), i
+        }, P0.apply(null, arguments)
+    }
+    var Y1 = Object.prototype.toString,
+        X1 = function(t) {
+            var r = Y1.call(t),
                 n = r === "[object Arguments]";
-            return n || (n = r !== "[object Array]" && t !== null && typeof t == "object" && typeof t.length == "number" && t.length >= 0 && z1.call(t.callee) === "[object Function]"), n
+            return n || (n = r !== "[object Array]" && t !== null && typeof t == "object" && typeof t.length == "number" && t.length >= 0 && Y1.call(t.callee) === "[object Function]"), n
         },
-        n1, I1;
+        i1, q1;
 
-    function K9() {
-        if (I1) return n1;
-        I1 = 1;
+    function e5() {
+        if (q1) return i1;
+        q1 = 1;
         var e;
         if (!Object.keys) {
             var t = Object.prototype.hasOwnProperty,
                 r = Object.prototype.toString,
-                n = H1,
+                n = X1,
                 a = Object.prototype.propertyIsEnumerable,
                 o = !a.call({
                     toString: null
                 }, "toString"),
                 c = a.call(function() {}, "prototype"),
                 s = ["toString", "toLocaleString", "valueOf", "hasOwnProperty", "isPrototypeOf", "propertyIsEnumerable", "constructor"],
-                i = function(f) {
-                    var g = f.constructor;
-                    return g && g.prototype === f
+                u = function(l) {
+                    var p = l.constructor;
+                    return p && p.prototype === l
                 },
-                u = {
+                i = {
                     $applicationCache: !0,
                     $console: !0,
                     $external: !0,
                     $frame: !0,
                     $frameElement: !0,
                     $frames: !0,
                     $innerHeight: !0,
@@ -1455,77 +1455,77 @@
                     $scrollX: !0,
                     $scrollY: !0,
                     $self: !0,
                     $webkitIndexedDB: !0,
                     $webkitStorageInfo: !0,
                     $window: !0
                 },
-                l = function() {
+                f = function() {
                     if (typeof window > "u") return !1;
-                    for (var f in window) try {
-                        if (!u["$" + f] && t.call(window, f) && window[f] !== null && typeof window[f] == "object") try {
-                            i(window[f])
+                    for (var l in window) try {
+                        if (!i["$" + l] && t.call(window, l) && window[l] !== null && typeof window[l] == "object") try {
+                            u(window[l])
                         } catch {
                             return !0
                         }
                     } catch {
                         return !0
                     }
                     return !1
                 }(),
-                p = function(f) {
-                    if (typeof window > "u" || !l) return i(f);
+                g = function(l) {
+                    if (typeof window > "u" || !f) return u(l);
                     try {
-                        return i(f)
+                        return u(l)
                     } catch {
                         return !1
                     }
                 };
-            e = function(g) {
-                var y = g !== null && typeof g == "object",
-                    h = r.call(g) === "[object Function]",
-                    C = n(g),
-                    N = y && r.call(g) === "[object String]",
-                    R = [];
+            e = function(p) {
+                var y = p !== null && typeof p == "object",
+                    h = r.call(p) === "[object Function]",
+                    C = n(p),
+                    N = y && r.call(p) === "[object String]",
+                    x = [];
                 if (!y && !h && !C) throw new TypeError("Object.keys called on a non-object");
                 var B = c && h;
-                if (N && g.length > 0 && !t.call(g, 0))
-                    for (var w = 0; w < g.length; ++w) R.push(String(w));
-                if (C && g.length > 0)
-                    for (var S = 0; S < g.length; ++S) R.push(String(S));
+                if (N && p.length > 0 && !t.call(p, 0))
+                    for (var b = 0; b < p.length; ++b) x.push(String(b));
+                if (C && p.length > 0)
+                    for (var S = 0; S < p.length; ++S) x.push(String(S));
                 else
-                    for (var b in g) !(B && b === "prototype") && t.call(g, b) && R.push(String(b));
+                    for (var w in p) !(B && w === "prototype") && t.call(p, w) && x.push(String(w));
                 if (o)
-                    for (var v = p(g), d = 0; d < s.length; ++d) !(v && s[d] === "constructor") && t.call(g, s[d]) && R.push(s[d]);
-                return R
+                    for (var v = g(p), d = 0; d < s.length; ++d) !(v && s[d] === "constructor") && t.call(p, s[d]) && x.push(s[d]);
+                return x
             }
         }
-        return n1 = e, n1
+        return i1 = e, i1
     }
-    var J9 = Array.prototype.slice,
-        Q9 = H1,
-        W1 = Object.keys,
-        $0 = W1 ? function(t) {
-            return W1(t)
-        } : K9(),
-        Y1 = Object.keys;
-    $0.shim = function() {
+    var t5 = Array.prototype.slice,
+        r5 = X1,
+        K1 = Object.keys,
+        U0 = K1 ? function(t) {
+            return K1(t)
+        } : e5(),
+        J1 = Object.keys;
+    U0.shim = function() {
         if (Object.keys) {
             var t = function() {
                 var r = Object.keys(arguments);
                 return r && r.length === arguments.length
             }(1, 2);
             t || (Object.keys = function(n) {
-                return Q9(n) ? Y1(J9.call(n)) : Y1(n)
+                return r5(n) ? J1(t5.call(n)) : J1(n)
             })
-        } else Object.keys = $0;
-        return Object.keys || $0
+        } else Object.keys = U0;
+        return Object.keys || U0
     };
-    var Z9 = $0,
-        e5 = function() {
+    var n5 = U0,
+        a5 = function() {
             if (typeof Symbol != "function" || typeof Object.getOwnPropertySymbols != "function") return !1;
             if (typeof Symbol.iterator == "symbol") return !0;
             var t = {},
                 r = Symbol("test"),
                 n = Object(r);
             if (typeof r == "string" || Object.prototype.toString.call(r) !== "[object Symbol]" || Object.prototype.toString.call(n) !== "[object Symbol]") return !1;
             var a = 42;
@@ -1536,178 +1536,178 @@
             if (o.length !== 1 || o[0] !== r || !Object.prototype.propertyIsEnumerable.call(t, r)) return !1;
             if (typeof Object.getOwnPropertyDescriptor == "function") {
                 var c = Object.getOwnPropertyDescriptor(t, r);
                 if (c.value !== a || c.enumerable !== !0) return !1
             }
             return !0
         },
-        X1 = typeof Symbol < "u" && Symbol,
-        t5 = e5,
-        r5 = function() {
-            return typeof X1 != "function" || typeof Symbol != "function" || typeof X1("foo") != "symbol" || typeof Symbol("bar") != "symbol" ? !1 : t5()
+        Q1 = typeof Symbol < "u" && Symbol,
+        o5 = a5,
+        i5 = function() {
+            return typeof Q1 != "function" || typeof Symbol != "function" || typeof Q1("foo") != "symbol" || typeof Symbol("bar") != "symbol" ? !1 : o5()
         },
-        q1 = {
+        Z1 = {
             foo: {}
         },
-        n5 = Object,
-        a5 = function() {
+        u5 = Object,
+        s5 = function() {
             return {
-                __proto__: q1
-            }.foo === q1.foo && !({
+                __proto__: Z1
+            }.foo === Z1.foo && !({
                     __proto__: null
                 }
-                instanceof n5)
+                instanceof u5)
         },
-        o5 = "Function.prototype.bind called on incompatible ",
-        a1 = Array.prototype.slice,
-        i5 = Object.prototype.toString,
-        u5 = "[object Function]",
-        s5 = function(t) {
+        c5 = "Function.prototype.bind called on incompatible ",
+        u1 = Array.prototype.slice,
+        l5 = Object.prototype.toString,
+        f5 = "[object Function]",
+        g5 = function(t) {
             var r = this;
-            if (typeof r != "function" || i5.call(r) !== u5) throw new TypeError(o5 + r);
-            for (var n = a1.call(arguments, 1), a, o = function() {
+            if (typeof r != "function" || l5.call(r) !== f5) throw new TypeError(c5 + r);
+            for (var n = u1.call(arguments, 1), a, o = function() {
                     if (this instanceof a) {
-                        var l = r.apply(this, n.concat(a1.call(arguments)));
-                        return Object(l) === l ? l : this
-                    } else return r.apply(t, n.concat(a1.call(arguments)))
-                }, c = Math.max(0, r.length - n.length), s = [], i = 0; i < c; i++) s.push("$" + i);
+                        var f = r.apply(this, n.concat(u1.call(arguments)));
+                        return Object(f) === f ? f : this
+                    } else return r.apply(t, n.concat(u1.call(arguments)))
+                }, c = Math.max(0, r.length - n.length), s = [], u = 0; u < c; u++) s.push("$" + u);
             if (a = Function("binder", "return function (" + s.join(",") + "){ return binder.apply(this,arguments); }")(o), r.prototype) {
-                var u = function() {};
-                u.prototype = r.prototype, a.prototype = new u, u.prototype = null
+                var i = function() {};
+                i.prototype = r.prototype, a.prototype = new i, i.prototype = null
             }
             return a
         },
-        c5 = s5,
-        K1 = Function.prototype.bind || c5,
-        f5 = K1,
-        l5 = f5.call(Function.call, Object.prototype.hasOwnProperty),
-        M, S0 = SyntaxError,
-        J1 = Function,
-        w0 = TypeError,
-        o1 = function(e) {
+        p5 = g5,
+        e2 = Function.prototype.bind || p5,
+        v5 = e2,
+        y5 = v5.call(Function.call, Object.prototype.hasOwnProperty),
+        G, N0 = SyntaxError,
+        t2 = Function,
+        B0 = TypeError,
+        s1 = function(e) {
             try {
-                return J1('"use strict"; return (' + e + ").constructor;")()
+                return t2('"use strict"; return (' + e + ").constructor;")()
             } catch {}
         },
-        p0 = Object.getOwnPropertyDescriptor;
-    if (p0) try {
-        p0({}, "")
+        d0 = Object.getOwnPropertyDescriptor;
+    if (d0) try {
+        d0({}, "")
     } catch {
-        p0 = null
+        d0 = null
     }
-    var i1 = function() {
-            throw new w0
+    var c1 = function() {
+            throw new B0
         },
-        p5 = p0 ? function() {
+        d5 = d0 ? function() {
             try {
-                return arguments.callee, i1
+                return arguments.callee, c1
             } catch {
                 try {
-                    return p0(arguments, "callee").get
+                    return d0(arguments, "callee").get
                 } catch {
-                    return i1
+                    return c1
                 }
             }
-        }() : i1,
-        b0 = r5(),
-        g5 = a5(),
-        $ = Object.getPrototypeOf || (g5 ? function(e) {
+        }() : c1,
+        x0 = i5(),
+        h5 = s5(),
+        z = Object.getPrototypeOf || (h5 ? function(e) {
             return e.__proto__
         } : null),
-        N0 = {},
-        v5 = typeof Uint8Array > "u" || !$ ? M : $(Uint8Array),
-        g0 = {
-            "%AggregateError%": typeof AggregateError > "u" ? M : AggregateError,
+        R0 = {},
+        m5 = typeof Uint8Array > "u" || !z ? G : z(Uint8Array),
+        h0 = {
+            "%AggregateError%": typeof AggregateError > "u" ? G : AggregateError,
             "%Array%": Array,
-            "%ArrayBuffer%": typeof ArrayBuffer > "u" ? M : ArrayBuffer,
-            "%ArrayIteratorPrototype%": b0 && $ ? $([][Symbol.iterator]()) : M,
-            "%AsyncFromSyncIteratorPrototype%": M,
-            "%AsyncFunction%": N0,
-            "%AsyncGenerator%": N0,
-            "%AsyncGeneratorFunction%": N0,
-            "%AsyncIteratorPrototype%": N0,
-            "%Atomics%": typeof Atomics > "u" ? M : Atomics,
-            "%BigInt%": typeof BigInt > "u" ? M : BigInt,
-            "%BigInt64Array%": typeof BigInt64Array > "u" ? M : BigInt64Array,
-            "%BigUint64Array%": typeof BigUint64Array > "u" ? M : BigUint64Array,
+            "%ArrayBuffer%": typeof ArrayBuffer > "u" ? G : ArrayBuffer,
+            "%ArrayIteratorPrototype%": x0 && z ? z([][Symbol.iterator]()) : G,
+            "%AsyncFromSyncIteratorPrototype%": G,
+            "%AsyncFunction%": R0,
+            "%AsyncGenerator%": R0,
+            "%AsyncGeneratorFunction%": R0,
+            "%AsyncIteratorPrototype%": R0,
+            "%Atomics%": typeof Atomics > "u" ? G : Atomics,
+            "%BigInt%": typeof BigInt > "u" ? G : BigInt,
+            "%BigInt64Array%": typeof BigInt64Array > "u" ? G : BigInt64Array,
+            "%BigUint64Array%": typeof BigUint64Array > "u" ? G : BigUint64Array,
             "%Boolean%": Boolean,
-            "%DataView%": typeof DataView > "u" ? M : DataView,
+            "%DataView%": typeof DataView > "u" ? G : DataView,
             "%Date%": Date,
             "%decodeURI%": decodeURI,
             "%decodeURIComponent%": decodeURIComponent,
             "%encodeURI%": encodeURI,
             "%encodeURIComponent%": encodeURIComponent,
             "%Error%": Error,
             "%eval%": eval,
             "%EvalError%": EvalError,
-            "%Float32Array%": typeof Float32Array > "u" ? M : Float32Array,
-            "%Float64Array%": typeof Float64Array > "u" ? M : Float64Array,
-            "%FinalizationRegistry%": typeof FinalizationRegistry > "u" ? M : FinalizationRegistry,
-            "%Function%": J1,
-            "%GeneratorFunction%": N0,
-            "%Int8Array%": typeof Int8Array > "u" ? M : Int8Array,
-            "%Int16Array%": typeof Int16Array > "u" ? M : Int16Array,
-            "%Int32Array%": typeof Int32Array > "u" ? M : Int32Array,
+            "%Float32Array%": typeof Float32Array > "u" ? G : Float32Array,
+            "%Float64Array%": typeof Float64Array > "u" ? G : Float64Array,
+            "%FinalizationRegistry%": typeof FinalizationRegistry > "u" ? G : FinalizationRegistry,
+            "%Function%": t2,
+            "%GeneratorFunction%": R0,
+            "%Int8Array%": typeof Int8Array > "u" ? G : Int8Array,
+            "%Int16Array%": typeof Int16Array > "u" ? G : Int16Array,
+            "%Int32Array%": typeof Int32Array > "u" ? G : Int32Array,
             "%isFinite%": isFinite,
             "%isNaN%": isNaN,
-            "%IteratorPrototype%": b0 && $ ? $($([][Symbol.iterator]())) : M,
-            "%JSON%": typeof JSON == "object" ? JSON : M,
-            "%Map%": typeof Map > "u" ? M : Map,
-            "%MapIteratorPrototype%": typeof Map > "u" || !b0 || !$ ? M : $(new Map()[Symbol.iterator]()),
+            "%IteratorPrototype%": x0 && z ? z(z([][Symbol.iterator]())) : G,
+            "%JSON%": typeof JSON == "object" ? JSON : G,
+            "%Map%": typeof Map > "u" ? G : Map,
+            "%MapIteratorPrototype%": typeof Map > "u" || !x0 || !z ? G : z(new Map()[Symbol.iterator]()),
             "%Math%": Math,
             "%Number%": Number,
             "%Object%": Object,
             "%parseFloat%": parseFloat,
             "%parseInt%": parseInt,
-            "%Promise%": typeof Promise > "u" ? M : Promise,
-            "%Proxy%": typeof Proxy > "u" ? M : Proxy,
+            "%Promise%": typeof Promise > "u" ? G : Promise,
+            "%Proxy%": typeof Proxy > "u" ? G : Proxy,
             "%RangeError%": RangeError,
             "%ReferenceError%": ReferenceError,
-            "%Reflect%": typeof Reflect > "u" ? M : Reflect,
+            "%Reflect%": typeof Reflect > "u" ? G : Reflect,
             "%RegExp%": RegExp,
-            "%Set%": typeof Set > "u" ? M : Set,
-            "%SetIteratorPrototype%": typeof Set > "u" || !b0 || !$ ? M : $(new Set()[Symbol.iterator]()),
-            "%SharedArrayBuffer%": typeof SharedArrayBuffer > "u" ? M : SharedArrayBuffer,
+            "%Set%": typeof Set > "u" ? G : Set,
+            "%SetIteratorPrototype%": typeof Set > "u" || !x0 || !z ? G : z(new Set()[Symbol.iterator]()),
+            "%SharedArrayBuffer%": typeof SharedArrayBuffer > "u" ? G : SharedArrayBuffer,
             "%String%": String,
-            "%StringIteratorPrototype%": b0 && $ ? $("" [Symbol.iterator]()) : M,
-            "%Symbol%": b0 ? Symbol : M,
-            "%SyntaxError%": S0,
-            "%ThrowTypeError%": p5,
-            "%TypedArray%": v5,
-            "%TypeError%": w0,
-            "%Uint8Array%": typeof Uint8Array > "u" ? M : Uint8Array,
-            "%Uint8ClampedArray%": typeof Uint8ClampedArray > "u" ? M : Uint8ClampedArray,
-            "%Uint16Array%": typeof Uint16Array > "u" ? M : Uint16Array,
-            "%Uint32Array%": typeof Uint32Array > "u" ? M : Uint32Array,
+            "%StringIteratorPrototype%": x0 && z ? z("" [Symbol.iterator]()) : G,
+            "%Symbol%": x0 ? Symbol : G,
+            "%SyntaxError%": N0,
+            "%ThrowTypeError%": d5,
+            "%TypedArray%": m5,
+            "%TypeError%": B0,
+            "%Uint8Array%": typeof Uint8Array > "u" ? G : Uint8Array,
+            "%Uint8ClampedArray%": typeof Uint8ClampedArray > "u" ? G : Uint8ClampedArray,
+            "%Uint16Array%": typeof Uint16Array > "u" ? G : Uint16Array,
+            "%Uint32Array%": typeof Uint32Array > "u" ? G : Uint32Array,
             "%URIError%": URIError,
-            "%WeakMap%": typeof WeakMap > "u" ? M : WeakMap,
-            "%WeakRef%": typeof WeakRef > "u" ? M : WeakRef,
-            "%WeakSet%": typeof WeakSet > "u" ? M : WeakSet
+            "%WeakMap%": typeof WeakMap > "u" ? G : WeakMap,
+            "%WeakRef%": typeof WeakRef > "u" ? G : WeakRef,
+            "%WeakSet%": typeof WeakSet > "u" ? G : WeakSet
         };
-    if ($) try {
+    if (z) try {
         null.error
     } catch (e) {
-        var y5 = $($(e));
-        g0["%Error.prototype%"] = y5
+        var C5 = z(z(e));
+        h0["%Error.prototype%"] = C5
     }
-    var d5 = function e(t) {
+    var S5 = function e(t) {
             var r;
-            if (t === "%AsyncFunction%") r = o1("async function () {}");
-            else if (t === "%GeneratorFunction%") r = o1("function* () {}");
-            else if (t === "%AsyncGeneratorFunction%") r = o1("async function* () {}");
+            if (t === "%AsyncFunction%") r = s1("async function () {}");
+            else if (t === "%GeneratorFunction%") r = s1("function* () {}");
+            else if (t === "%AsyncGeneratorFunction%") r = s1("async function* () {}");
             else if (t === "%AsyncGenerator%") {
                 var n = e("%AsyncGeneratorFunction%");
                 n && (r = n.prototype)
             } else if (t === "%AsyncIteratorPrototype%") {
                 var a = e("%AsyncGenerator%");
-                a && $ && (r = $(a.prototype))
+                a && z && (r = z(a.prototype))
             }
-            return g0[t] = r, r
+            return h0[t] = r, r
         },
-        Q1 = {
+        r2 = {
             "%ArrayBufferPrototype%": ["ArrayBuffer", "prototype"],
             "%ArrayPrototype%": ["Array", "prototype"],
             "%ArrayProto_entries%": ["Array", "prototype", "entries"],
             "%ArrayProto_forEach%": ["Array", "prototype", "forEach"],
             "%ArrayProto_keys%": ["Array", "prototype", "keys"],
             "%ArrayProto_values%": ["Array", "prototype", "values"],
             "%AsyncFunctionPrototype%": ["AsyncFunction", "prototype"],
@@ -1752,506 +1752,506 @@
             "%Uint8ClampedArrayPrototype%": ["Uint8ClampedArray", "prototype"],
             "%Uint16ArrayPrototype%": ["Uint16Array", "prototype"],
             "%Uint32ArrayPrototype%": ["Uint32Array", "prototype"],
             "%URIErrorPrototype%": ["URIError", "prototype"],
             "%WeakMapPrototype%": ["WeakMap", "prototype"],
             "%WeakSetPrototype%": ["WeakSet", "prototype"]
         },
-        L0 = K1,
-        j0 = l5,
-        h5 = L0.call(Function.call, Array.prototype.concat),
-        m5 = L0.call(Function.apply, Array.prototype.splice),
-        Z1 = L0.call(Function.call, String.prototype.replace),
-        U0 = L0.call(Function.call, String.prototype.slice),
-        C5 = L0.call(Function.call, RegExp.prototype.exec),
-        S5 = /[^%.[\]]+|\[(?:(-?\d+(?:\.\d+)?)|(["'])((?:(?!\2)[^\\]|\\.)*?)\2)\]|(?=(?:\.|\[\])(?:\.|\[\]|%$))/g,
-        w5 = /\\(\\)?/g,
-        b5 = function(t) {
-            var r = U0(t, 0, 1),
-                n = U0(t, -1);
-            if (r === "%" && n !== "%") throw new S0("invalid intrinsic syntax, expected closing `%`");
-            if (n === "%" && r !== "%") throw new S0("invalid intrinsic syntax, expected opening `%`");
+        _0 = e2,
+        F0 = y5,
+        w5 = _0.call(Function.call, Array.prototype.concat),
+        b5 = _0.call(Function.apply, Array.prototype.splice),
+        n2 = _0.call(Function.call, String.prototype.replace),
+        V0 = _0.call(Function.call, String.prototype.slice),
+        N5 = _0.call(Function.call, RegExp.prototype.exec),
+        B5 = /[^%.[\]]+|\[(?:(-?\d+(?:\.\d+)?)|(["'])((?:(?!\2)[^\\]|\\.)*?)\2)\]|(?=(?:\.|\[\])(?:\.|\[\]|%$))/g,
+        x5 = /\\(\\)?/g,
+        R5 = function(t) {
+            var r = V0(t, 0, 1),
+                n = V0(t, -1);
+            if (r === "%" && n !== "%") throw new N0("invalid intrinsic syntax, expected closing `%`");
+            if (n === "%" && r !== "%") throw new N0("invalid intrinsic syntax, expected opening `%`");
             var a = [];
-            return Z1(t, S5, function(o, c, s, i) {
-                a[a.length] = s ? Z1(i, w5, "$1") : c || o
+            return n2(t, B5, function(o, c, s, u) {
+                a[a.length] = s ? n2(u, x5, "$1") : c || o
             }), a
         },
-        N5 = function(t, r) {
+        O5 = function(t, r) {
             var n = t,
                 a;
-            if (j0(Q1, n) && (a = Q1[n], n = "%" + a[0] + "%"), j0(g0, n)) {
-                var o = g0[n];
-                if (o === N0 && (o = d5(n)), typeof o > "u" && !r) throw new w0("intrinsic " + t + " exists, but is not available. Please file an issue!");
+            if (F0(r2, n) && (a = r2[n], n = "%" + a[0] + "%"), F0(h0, n)) {
+                var o = h0[n];
+                if (o === R0 && (o = S5(n)), typeof o > "u" && !r) throw new B0("intrinsic " + t + " exists, but is not available. Please file an issue!");
                 return {
                     alias: a,
                     name: n,
                     value: o
                 }
             }
-            throw new S0("intrinsic " + t + " does not exist!")
+            throw new N0("intrinsic " + t + " does not exist!")
         },
-        B5 = function(t, r) {
-            if (typeof t != "string" || t.length === 0) throw new w0("intrinsic name must be a non-empty string");
-            if (arguments.length > 1 && typeof r != "boolean") throw new w0('"allowMissing" argument must be a boolean');
-            if (C5(/^%?[^%]*%?$/, t) === null) throw new S0("`%` may not be present anywhere but at the beginning and end of the intrinsic name");
-            var n = b5(t),
+        T5 = function(t, r) {
+            if (typeof t != "string" || t.length === 0) throw new B0("intrinsic name must be a non-empty string");
+            if (arguments.length > 1 && typeof r != "boolean") throw new B0('"allowMissing" argument must be a boolean');
+            if (N5(/^%?[^%]*%?$/, t) === null) throw new N0("`%` may not be present anywhere but at the beginning and end of the intrinsic name");
+            var n = R5(t),
                 a = n.length > 0 ? n[0] : "",
-                o = N5("%" + a + "%", r),
+                o = O5("%" + a + "%", r),
                 c = o.name,
                 s = o.value,
-                i = !1,
-                u = o.alias;
-            u && (a = u[0], m5(n, h5([0, 1], u)));
-            for (var l = 1, p = !0; l < n.length; l += 1) {
-                var f = n[l],
-                    g = U0(f, 0, 1),
-                    y = U0(f, -1);
-                if ((g === '"' || g === "'" || g === "`" || y === '"' || y === "'" || y === "`") && g !== y) throw new S0("property names with quotes must have matching quotes");
-                if ((f === "constructor" || !p) && (i = !0), a += "." + f, c = "%" + a + "%", j0(g0, c)) s = g0[c];
+                u = !1,
+                i = o.alias;
+            i && (a = i[0], b5(n, w5([0, 1], i)));
+            for (var f = 1, g = !0; f < n.length; f += 1) {
+                var l = n[f],
+                    p = V0(l, 0, 1),
+                    y = V0(l, -1);
+                if ((p === '"' || p === "'" || p === "`" || y === '"' || y === "'" || y === "`") && p !== y) throw new N0("property names with quotes must have matching quotes");
+                if ((l === "constructor" || !g) && (u = !0), a += "." + l, c = "%" + a + "%", F0(h0, c)) s = h0[c];
                 else if (s != null) {
-                    if (!(f in s)) {
-                        if (!r) throw new w0("base intrinsic for " + t + " exists, but the property is not available.");
+                    if (!(l in s)) {
+                        if (!r) throw new B0("base intrinsic for " + t + " exists, but the property is not available.");
                         return
                     }
-                    if (p0 && l + 1 >= n.length) {
-                        var h = p0(s, f);
-                        p = !!h, p && "get" in h && !("originalValue" in h.get) ? s = h.get : s = s[f]
-                    } else p = j0(s, f), s = s[f];
-                    p && !i && (g0[c] = s)
+                    if (d0 && f + 1 >= n.length) {
+                        var h = d0(s, l);
+                        g = !!h, g && "get" in h && !("originalValue" in h.get) ? s = h.get : s = s[l]
+                    } else g = F0(s, l), s = s[l];
+                    g && !u && (h0[c] = s)
                 }
             }
             return s
         },
-        R5 = B5,
-        u1 = R5("%Object.defineProperty%", !0),
-        s1 = function() {
-            if (u1) try {
-                return u1({}, "a", {
+        M5 = T5,
+        l1 = M5("%Object.defineProperty%", !0),
+        f1 = function() {
+            if (l1) try {
+                return l1({}, "a", {
                     value: 1
                 }), !0
             } catch {
                 return !1
             }
             return !1
         };
-    s1.hasArrayLengthDefineBug = function() {
-        if (!s1()) return null;
+    f1.hasArrayLengthDefineBug = function() {
+        if (!f1()) return null;
         try {
-            return u1([], "length", {
+            return l1([], "length", {
                 value: 1
             }).length !== 1
         } catch {
             return !0
         }
     };
-    var x5 = s1,
-        O5 = Z9,
-        T5 = typeof Symbol == "function" && typeof Symbol("foo") == "symbol",
-        M5 = Object.prototype.toString,
-        G5 = Array.prototype.concat,
-        e2 = Object.defineProperty,
-        E5 = function(e) {
-            return typeof e == "function" && M5.call(e) === "[object Function]"
-        },
-        k5 = x5(),
-        t2 = e2 && k5,
-        A5 = function(e, t, r, n) {
+    var G5 = f1,
+        E5 = n5,
+        k5 = typeof Symbol == "function" && typeof Symbol("foo") == "symbol",
+        D5 = Object.prototype.toString,
+        L5 = Array.prototype.concat,
+        a2 = Object.defineProperty,
+        A5 = function(e) {
+            return typeof e == "function" && D5.call(e) === "[object Function]"
+        },
+        P5 = G5(),
+        o2 = a2 && P5,
+        _5 = function(e, t, r, n) {
             if (t in e) {
                 if (n === !0) {
                     if (e[t] === r) return
-                } else if (!E5(n) || !n()) return
+                } else if (!A5(n) || !n()) return
             }
-            t2 ? e2(e, t, {
+            o2 ? a2(e, t, {
                 configurable: !0,
                 enumerable: !1,
                 value: r,
                 writable: !0
             }) : e[t] = r
         },
-        r2 = function(e, t) {
+        i2 = function(e, t) {
             var r = arguments.length > 2 ? arguments[2] : {},
-                n = O5(t);
-            T5 && (n = G5.call(n, Object.getOwnPropertySymbols(t)));
-            for (var a = 0; a < n.length; a += 1) A5(e, n[a], t[n[a]], r[n[a]])
+                n = E5(t);
+            k5 && (n = L5.call(n, Object.getOwnPropertySymbols(t)));
+            for (var a = 0; a < n.length; a += 1) _5(e, n[a], t[n[a]], r[n[a]])
         };
-    r2.supportsDescriptors = !!t2;
-    var n2 = r2,
-        F0 = {},
-        c1 = {
+    i2.supportsDescriptors = !!o2;
+    var u2 = i2,
+        z0 = {},
+        g1 = {
             get exports() {
-                return F0
+                return z0
             },
             set exports(e) {
-                F0 = e
+                z0 = e
             }
         };
-    typeof self < "u" ? c1.exports = self : typeof window < "u" ? c1.exports = window : c1.exports = Function("return this")();
-    var D5 = F0,
-        a2 = function() {
-            return typeof q != "object" || !q || q.Math !== Math || q.Array !== Array ? D5 : q
-        },
-        L5 = n2,
-        P5 = a2,
-        _5 = function() {
-            var t = P5();
-            if (L5.supportsDescriptors) {
+    typeof self < "u" ? g1.exports = self : typeof window < "u" ? g1.exports = window : g1.exports = Function("return this")();
+    var $5 = z0,
+        s2 = function() {
+            return typeof e0 != "object" || !e0 || e0.Math !== Math || e0.Array !== Array ? $5 : e0
+        },
+        j5 = u2,
+        U5 = s2,
+        F5 = function() {
+            var t = U5();
+            if (j5.supportsDescriptors) {
                 var r = Object.getOwnPropertyDescriptor(t, "globalThis");
                 (!r || r.configurable && (r.enumerable || r.writable || globalThis !== t)) && Object.defineProperty(t, "globalThis", {
                     configurable: !0,
                     enumerable: !1,
                     value: t,
                     writable: !1
                 })
             } else(typeof globalThis != "object" || globalThis !== t) && (t.globalThis = t);
             return t
         },
-        $5 = n2,
-        j5 = F0,
-        o2 = a2,
-        U5 = _5,
-        F5 = o2(),
-        i2 = function() {
-            return F5
+        V5 = u2,
+        z5 = z0,
+        c2 = s2,
+        H5 = F5,
+        I5 = c2(),
+        l2 = function() {
+            return I5
         };
-    $5(i2, {
-        getPolyfill: o2,
-        implementation: j5,
-        shim: U5
+    V5(l2, {
+        getPolyfill: c2,
+        implementation: z5,
+        shim: H5
     });
-    var V5 = i2;
+    var W5 = l2;
 
-    function u2(e, t) {
+    function f2(e, t) {
         var r = Object.keys(e);
         if (Object.getOwnPropertySymbols) {
             var n = Object.getOwnPropertySymbols(e);
             t && (n = n.filter(function(a) {
                 return Object.getOwnPropertyDescriptor(e, a).enumerable
             })), r.push.apply(r, n)
         }
         return r
     }
 
-    function z5(e) {
+    function Y5(e) {
         for (var t = 1; t < arguments.length; t++) {
             var r = arguments[t] != null ? arguments[t] : {};
-            t % 2 ? u2(Object(r), !0).forEach(function(n) {
-                f0(e, n, r[n])
-            }) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(r)) : u2(Object(r)).forEach(function(n) {
+            t % 2 ? f2(Object(r), !0).forEach(function(n) {
+                v0(e, n, r[n])
+            }) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(r)) : f2(Object(r)).forEach(function(n) {
                 Object.defineProperty(e, n, Object.getOwnPropertyDescriptor(r, n))
             })
         }
         return e
     }
-    var Q = V5(),
-        s2 = {
+    var r0 = W5(),
+        g2 = {
             vtkObject: function() {
                 return null
             }
         };
 
-    function v0(e) {
+    function m0(e) {
         if (e == null || e.isA) return e;
-        if (!e.vtkClass) return Q.console && Q.console.error && Q.console.error("Invalid VTK object"), null;
-        var t = s2[e.vtkClass];
-        if (!t) return Q.console && Q.console.error && Q.console.error("No vtk class found for Object of type ".concat(e.vtkClass)), null;
-        var r = z5({}, e);
+        if (!e.vtkClass) return r0.console && r0.console.error && r0.console.error("Invalid VTK object"), null;
+        var t = g2[e.vtkClass];
+        if (!t) return r0.console && r0.console.error && r0.console.error("No vtk class found for Object of type ".concat(e.vtkClass)), null;
+        var r = Y5({}, e);
         Object.keys(r).forEach(function(a) {
-            r[a] && l0(r[a]) === "object" && r[a].vtkClass && (r[a] = v0(r[a]))
+            r[a] && y0(r[a]) === "object" && r[a].vtkClass && (r[a] = m0(r[a]))
         });
         var n = t(r);
         return n && n.modified && n.modified(), n
     }
 
-    function H5(e, t) {
-        s2[e] = t
+    function X5(e, t) {
+        g2[e] = t
     }
-    v0.register = H5;
+    m0.register = X5;
 
-    function I5(e, t) {
+    function q5(e, t) {
         if (!(e instanceof t)) throw new TypeError("Cannot call a class as a function")
     }
 
-    function c2(e, t) {
+    function p2(e, t) {
         for (var r = 0; r < t.length; r++) {
             var n = t[r];
             n.enumerable = n.enumerable || !1, n.configurable = !0, "value" in n && (n.writable = !0), Object.defineProperty(e, n.key, n)
         }
     }
 
-    function W5(e, t, r) {
-        return t && c2(e.prototype, t), r && c2(e, r), Object.defineProperty(e, "prototype", {
+    function K5(e, t, r) {
+        return t && p2(e.prototype, t), r && p2(e, r), Object.defineProperty(e, "prototype", {
             writable: !1
         }), e
     }
 
-    function y0(e) {
-        return y0 = Object.setPrototypeOf ? Object.getPrototypeOf : function(r) {
+    function C0(e) {
+        return C0 = Object.setPrototypeOf ? Object.getPrototypeOf : function(r) {
             return r.__proto__ || Object.getPrototypeOf(r)
-        }, y0(e)
+        }, C0(e)
     }
 
-    function Y5(e, t) {
-        for (; !Object.prototype.hasOwnProperty.call(e, t) && (e = y0(e), e !== null););
+    function J5(e, t) {
+        for (; !Object.prototype.hasOwnProperty.call(e, t) && (e = C0(e), e !== null););
         return e
     }
 
-    function V0() {
-        return typeof Reflect < "u" && Reflect.get ? V0 = Reflect.get : V0 = function(t, r, n) {
-            var a = Y5(t, r);
+    function H0() {
+        return typeof Reflect < "u" && Reflect.get ? H0 = Reflect.get : H0 = function(t, r, n) {
+            var a = J5(t, r);
             if (a) {
                 var o = Object.getOwnPropertyDescriptor(a, r);
                 return o.get ? o.get.call(arguments.length < 3 ? t : n) : o.value
             }
-        }, V0.apply(this, arguments)
+        }, H0.apply(this, arguments)
     }
 
-    function X5(e, t) {
+    function Q5(e, t) {
         if (typeof t != "function" && t !== null) throw new TypeError("Super expression must either be null or a function");
         e.prototype = Object.create(t && t.prototype, {
             constructor: {
                 value: e,
                 writable: !0,
                 configurable: !0
             }
         }), Object.defineProperty(e, "prototype", {
             writable: !1
         }), t && A0(e, t)
     }
 
-    function q5(e) {
+    function Z5(e) {
         if (e === void 0) throw new ReferenceError("this hasn't been initialised - super() hasn't been called");
         return e
     }
 
-    function K5(e, t) {
-        if (t && (l0(t) === "object" || typeof t == "function")) return t;
+    function e3(e, t) {
+        if (t && (y0(t) === "object" || typeof t == "function")) return t;
         if (t !== void 0) throw new TypeError("Derived constructors may only return object or undefined");
-        return q5(e)
+        return Z5(e)
     }
 
-    function J5(e) {
+    function t3(e) {
         return Function.toString.call(e).indexOf("[native code]") !== -1
     }
 
-    function f1(e) {
+    function p1(e) {
         var t = typeof Map == "function" ? new Map : void 0;
-        return f1 = function(n) {
-            if (n === null || !J5(n)) return n;
+        return p1 = function(n) {
+            if (n === null || !t3(n)) return n;
             if (typeof n != "function") throw new TypeError("Super expression must either be null or a function");
             if (typeof t < "u") {
                 if (t.has(n)) return t.get(n);
                 t.set(n, a)
             }
 
             function a() {
-                return D0(n, arguments, y0(this).constructor)
+                return P0(n, arguments, C0(this).constructor)
             }
             return a.prototype = Object.create(n.prototype, {
                 constructor: {
                     value: a,
                     enumerable: !1,
                     writable: !0,
                     configurable: !0
                 }
             }), A0(a, n)
-        }, f1(e)
+        }, p1(e)
     }
 
-    function Q5(e) {
-        var t = Z5();
+    function r3(e) {
+        var t = n3();
         return function() {
-            var n = y0(e),
+            var n = C0(e),
                 a;
             if (t) {
-                var o = y0(this).constructor;
+                var o = C0(this).constructor;
                 a = Reflect.construct(n, arguments, o)
             } else a = n.apply(this, arguments);
-            return K5(this, a)
+            return e3(this, a)
         }
     }
 
-    function Z5() {
+    function n3() {
         if (typeof Reflect > "u" || !Reflect.construct || Reflect.construct.sham) return !1;
         if (typeof Proxy == "function") return !0;
         try {
             return Boolean.prototype.valueOf.call(Reflect.construct(Boolean, [], function() {})), !0
         } catch {
             return !1
         }
     }
-    var l1 = function(e) {
-        X5(r, e);
-        var t = Q5(r);
+    var v1 = function(e) {
+        Q5(r, e);
+        var t = r3(r);
 
         function r() {
-            return I5(this, r), t.apply(this, arguments)
+            return q5(this, r), t.apply(this, arguments)
         }
-        return W5(r, [{
+        return K5(r, [{
             key: "push",
             value: function() {
-                for (var a = this, o, c = arguments.length, s = new Array(c), i = 0; i < c; i++) s[i] = arguments[i];
-                var u = s.filter(function(l) {
-                    return !a.includes(l)
+                for (var a = this, o, c = arguments.length, s = new Array(c), u = 0; u < c; u++) s[u] = arguments[u];
+                var i = s.filter(function(f) {
+                    return !a.includes(f)
                 });
-                return (o = V0(y0(r.prototype), "push", this)).call.apply(o, [this].concat(r1(u)))
+                return (o = H0(C0(r.prototype), "push", this)).call.apply(o, [this].concat(o1(i)))
             }
         }]), r
-    }(f1(Array));
+    }(p1(Array));
 
-    function f2(e, t) {
+    function v2(e, t) {
         var r = Object.keys(e);
         if (Object.getOwnPropertySymbols) {
             var n = Object.getOwnPropertySymbols(e);
             t && (n = n.filter(function(a) {
                 return Object.getOwnPropertyDescriptor(e, a).enumerable
             })), r.push.apply(r, n)
         }
         return r
     }
 
-    function p1(e) {
+    function y1(e) {
         for (var t = 1; t < arguments.length; t++) {
             var r = arguments[t] != null ? arguments[t] : {};
-            t % 2 ? f2(Object(r), !0).forEach(function(n) {
-                f0(e, n, r[n])
-            }) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(r)) : f2(Object(r)).forEach(function(n) {
+            t % 2 ? v2(Object(r), !0).forEach(function(n) {
+                v0(e, n, r[n])
+            }) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(r)) : v2(Object(r)).forEach(function(n) {
                 Object.defineProperty(e, n, Object.getOwnPropertyDescriptor(r, n))
             })
         }
         return e
     }
-    var g1 = 0,
-        e3 = Symbol("void");
+    var d1 = 0,
+        a3 = Symbol("void");
 
-    function t3() {
-        return g1
+    function o3() {
+        return d1
     }
-    var l2 = {};
+    var y2 = {};
 
-    function d0() {}
-    var r3 = ["log", "debug", "info", "warn", "error", "time", "timeEnd", "group", "groupEnd"];
-    r3.forEach(function(e) {
-        l2[e] = d0
-    }), Q.console = console.hasOwnProperty("log") ? console : l2;
-    var Y = {
-        debug: d0,
-        error: Q.console.error || d0,
-        info: Q.console.info || d0,
-        log: Q.console.log || d0,
-        warn: Q.console.warn || d0
+    function S0() {}
+    var i3 = ["log", "debug", "info", "warn", "error", "time", "timeEnd", "group", "groupEnd"];
+    i3.forEach(function(e) {
+        y2[e] = S0
+    }), r0.console = console.hasOwnProperty("log") ? console : y2;
+    var J = {
+        debug: S0,
+        error: r0.console.error || S0,
+        info: r0.console.info || S0,
+        log: r0.console.log || S0,
+        warn: r0.console.warn || S0
     };
 
-    function n3(e, t) {
-        Y[e] && (Y[e] = t || d0)
+    function u3(e, t) {
+        J[e] && (J[e] = t || S0)
     }
 
-    function a3() {
-        Y.log.apply(Y, arguments)
+    function s3() {
+        J.log.apply(J, arguments)
     }
 
-    function o3() {
-        Y.info.apply(Y, arguments)
+    function c3() {
+        J.info.apply(J, arguments)
     }
 
-    function v1() {
-        Y.debug.apply(Y, arguments)
+    function h1() {
+        J.debug.apply(J, arguments)
     }
 
-    function j() {
-        Y.error.apply(Y, arguments)
+    function H() {
+        J.error.apply(J, arguments)
     }
 
-    function p2() {
-        Y.warn.apply(Y, arguments)
+    function d2() {
+        J.warn.apply(J, arguments)
     }
-    var g2 = {};
+    var h2 = {};
 
-    function i3(e) {
-        g2[e] || (Y.error(e), g2[e] = !0)
+    function l3(e) {
+        h2[e] || (J.error(e), h2[e] = !0)
     }
-    var K = Object.create(null);
-    K.Float32Array = Float32Array, K.Float64Array = Float64Array, K.Uint8Array = Uint8Array, K.Int8Array = Int8Array, K.Uint16Array = Uint16Array, K.Int16Array = Int16Array, K.Uint32Array = Uint32Array, K.Int32Array = Int32Array, K.Uint8ClampedArray = Uint8ClampedArray;
+    var t0 = Object.create(null);
+    t0.Float32Array = Float32Array, t0.Float64Array = Float64Array, t0.Uint8Array = Uint8Array, t0.Int8Array = Int8Array, t0.Uint16Array = Uint16Array, t0.Int16Array = Int16Array, t0.Uint32Array = Uint32Array, t0.Int32Array = Int32Array, t0.Uint8ClampedArray = Uint8ClampedArray;
 
-    function v2(e) {
+    function m2(e) {
         for (var t = arguments.length, r = new Array(t > 1 ? t - 1 : 0), n = 1; n < t; n++) r[n - 1] = arguments[n];
-        return D0(K[e] || Float64Array, r)
+        return P0(t0[e] || Float64Array, r)
     }
 
-    function y2(e) {
+    function C2(e) {
         for (var t, r = arguments.length, n = new Array(r > 1 ? r - 1 : 0), a = 1; a < r; a++) n[a - 1] = arguments[a];
-        return (t = K[e] || Float64Array).from.apply(t, n)
+        return (t = t0[e] || Float64Array).from.apply(t, n)
     }
 
-    function y1(e) {
+    function m1(e) {
         return e.charAt(0).toUpperCase() + e.slice(1)
     }
 
-    function V(e) {
-        return y1(e[0] === "_" ? e.slice(1) : e)
+    function I(e) {
+        return m1(e[0] === "_" ? e.slice(1) : e)
     }
 
-    function u3(e) {
+    function f3(e) {
         return e.charAt(0).toLowerCase() + e.slice(1)
     }
 
-    function s3(e) {
+    function g3(e) {
         for (var t = arguments.length > 1 && arguments[1] !== void 0 ? arguments[1] : 2, r = arguments.length > 2 && arguments[2] !== void 0 ? arguments[2] : 1e3, n = ["TB", "GB", "MB", "KB"], a = Number(e), o = "B"; a > r;) a /= r, o = n.pop();
         return "".concat(a.toFixed(t), " ").concat(o)
     }
 
-    function c3(e) {
+    function p3(e) {
         for (var t = arguments.length > 1 && arguments[1] !== void 0 ? arguments[1] : " ", r = [], n = e; n > 1e3;) r.push("000".concat(n % 1e3).slice(-3)), n = Math.floor(n / 1e3);
         return n > 0 && r.push(n), r.reverse(), r.join(t)
     }
 
-    function d2(e) {
+    function S2(e) {
         Object.keys(e).forEach(function(t) {
             Array.isArray(e[t]) && (e[t] = [].concat(e[t]))
         })
     }
 
-    function f3(e, t) {
+    function v3(e, t) {
         if (e === t) return !0;
         if (Array.isArray(e) && Array.isArray(t)) {
             if (e.length !== t.length) return !1;
             for (var r = 0; r < e.length; r++)
                 if (e[r] !== t[r]) return !1;
             return !0
         }
         return !1
     }
 
-    function l3(e, t) {
+    function y3(e, t) {
         return Object.keys(e).find(function(r) {
             return e[r] === t
         })
     }
 
-    function h2(e) {
+    function w2(e) {
         return e && e.isA ? e.getState() : e
     }
 
-    function m2(e) {
+    function b2(e) {
         setTimeout(e, 0)
     }
 
-    function p3(e, t) {
+    function d3(e, t) {
         var r = performance.now();
         e.finally(function() {
             var n = performance.now() - r;
             t(n)
         })
     }
 
-    function C2() {
+    function N2() {
         var e = arguments.length > 0 && arguments[0] !== void 0 ? arguments[0] : {},
             t = arguments.length > 1 && arguments[1] !== void 0 ? arguments[1] : {};
-        d2(t);
+        S2(t);
         var r = [];
-        Number.isInteger(t.mtime) || (t.mtime = ++g1), "classHierarchy" in t ? t.classHierarchy instanceof l1 || (t.classHierarchy = l1.from(t.classHierarchy)) : t.classHierarchy = new l1("vtkObject");
+        Number.isInteger(t.mtime) || (t.mtime = ++d1), "classHierarchy" in t ? t.classHierarchy instanceof v1 || (t.classHierarchy = v1.from(t.classHierarchy)) : t.classHierarchy = new v1("vtkObject");
 
         function n(o) {
             r[o] = null
         }
 
         function a(o) {
             function c() {
@@ -2261,22 +2261,22 @@
                 unsubscribe: c
             })
         }
         return e.isDeleted = function() {
             return !!t.deleted
         }, e.modified = function(o) {
             if (t.deleted) {
-                j("instance deleted - cannot call any method");
+                H("instance deleted - cannot call any method");
                 return
             }
-            o && o < e.getMTime() || (t.mtime = ++g1, r.forEach(function(c) {
+            o && o < e.getMTime() || (t.mtime = ++d1, r.forEach(function(c) {
                 return c && c(e)
             }))
         }, e.onModified = function(o) {
-            if (t.deleted) return j("instance deleted - cannot call any method"), null;
+            if (t.deleted) return H("instance deleted - cannot call any method"), null;
             var c = r.length;
             return r.push(o), a(c)
         }, e.getMTime = function() {
             return t.mtime
         }, e.isA = function(o) {
             for (var c = t.classHierarchy.length; c--;)
                 if (t.classHierarchy[c] === o) return !0;
@@ -2284,257 +2284,257 @@
         }, e.getClassName = function() {
             var o = arguments.length > 0 && arguments[0] !== void 0 ? arguments[0] : 0;
             return t.classHierarchy[t.classHierarchy.length - 1 - o]
         }, e.set = function() {
             var o = arguments.length > 0 && arguments[0] !== void 0 ? arguments[0] : {},
                 c = arguments.length > 1 && arguments[1] !== void 0 ? arguments[1] : !1,
                 s = arguments.length > 2 && arguments[2] !== void 0 ? arguments[2] : !1,
-                i = !1;
-            return Object.keys(o).forEach(function(u) {
-                var l = s ? null : e["set".concat(y1(u))];
-                l && Array.isArray(o[u]) && l.length > 1 ? i = l.apply(void 0, r1(o[u])) || i : l ? i = l(o[u]) || i : (["mtime"].indexOf(u) === -1 && !c && p2("Warning: Set value to model directly ".concat(u, ", ").concat(o[u])), i = t[u] !== o[u] || i, t[u] = o[u])
-            }), i
+                u = !1;
+            return Object.keys(o).forEach(function(i) {
+                var f = s ? null : e["set".concat(m1(i))];
+                f && Array.isArray(o[i]) && f.length > 1 ? u = f.apply(void 0, o1(o[i])) || u : f ? u = f(o[i]) || u : (["mtime"].indexOf(i) === -1 && !c && d2("Warning: Set value to model directly ".concat(i, ", ").concat(o[i])), u = t[i] !== o[i] || u, t[i] = o[i])
+            }), u
         }, e.get = function() {
             for (var o = arguments.length, c = new Array(o), s = 0; s < o; s++) c[s] = arguments[s];
             if (!c.length) return t;
-            var i = {};
-            return c.forEach(function(u) {
-                i[u] = t[u]
-            }), i
+            var u = {};
+            return c.forEach(function(i) {
+                u[i] = t[i]
+            }), u
         }, e.getReferenceByName = function(o) {
             return t[o]
         }, e.delete = function() {
             Object.keys(t).forEach(function(o) {
                 return delete t[o]
             }), r.forEach(function(o, c) {
                 return n(c)
             }), t.deleted = !0
         }, e.getState = function() {
             if (t.deleted) return null;
-            var o = p1(p1({}, t), {}, {
+            var o = y1(y1({}, t), {}, {
                 vtkClass: e.getClassName()
             });
             Object.keys(o).forEach(function(s) {
-                o[s] === null || o[s] === void 0 || s[0] === "_" ? delete o[s] : o[s].isA ? o[s] = o[s].getState() : Array.isArray(o[s]) && (o[s] = o[s].map(h2))
+                o[s] === null || o[s] === void 0 || s[0] === "_" ? delete o[s] : o[s].isA ? o[s] = o[s].getState() : Array.isArray(o[s]) && (o[s] = o[s].map(w2))
             });
             var c = {};
             return Object.keys(o).sort().forEach(function(s) {
                 c[s] = o[s]
             }), c.mtime && delete c.mtime, c
         }, e.shallowCopy = function(o) {
             var c = arguments.length > 1 && arguments[1] !== void 0 ? arguments[1] : !1;
             if (o.getClassName() !== e.getClassName()) throw new Error("Cannot ShallowCopy ".concat(o.getClassName(), " into ").concat(e.getClassName()));
             var s = o.get(),
-                i = Object.keys(t).sort(),
-                u = Object.keys(s).sort();
-            u.forEach(function(l) {
-                var p = i.indexOf(l);
-                p === -1 ? c && v1("add ".concat(l, " in shallowCopy")) : i.splice(p, 1), t[l] = s[l]
-            }), i.length && c && v1("Untouched keys: ".concat(i.join(", "))), e.modified()
+                u = Object.keys(t).sort(),
+                i = Object.keys(s).sort();
+            i.forEach(function(f) {
+                var g = u.indexOf(f);
+                g === -1 ? c && h1("add ".concat(f, " in shallowCopy")) : u.splice(g, 1), t[f] = s[f]
+            }), u.length && c && h1("Untouched keys: ".concat(u.join(", "))), e.modified()
         }, e.toJSON = function() {
             return e.getState()
         }, e
     }
 
-    function z0(e, t, r) {
+    function I0(e, t, r) {
         r.forEach(function(n) {
-            l0(n) === "object" ? e["get".concat(V(n.name))] = function() {
+            y0(n) === "object" ? e["get".concat(I(n.name))] = function() {
                 return t[n.name]
-            } : e["get".concat(V(n))] = function() {
+            } : e["get".concat(I(n))] = function() {
                 return t[n]
             }
         })
     }
-    var g3 = {
+    var h3 = {
         enum: function(t, r, n) {
             return function(a) {
                 if (typeof a == "string") {
                     if (n.enum[a] !== void 0) return r[n.name] !== n.enum[a] ? (r[n.name] = n.enum[a], t.modified(), !0) : !1;
-                    throw j("Set Enum with invalid argument ".concat(n, ", ").concat(a)), new RangeError("Set Enum with invalid string argument")
+                    throw H("Set Enum with invalid argument ".concat(n, ", ").concat(a)), new RangeError("Set Enum with invalid string argument")
                 }
                 if (typeof a == "number") {
                     if (r[n.name] !== a) {
                         if (Object.keys(n.enum).map(function(o) {
                                 return n.enum[o]
                             }).indexOf(a) !== -1) return r[n.name] = a, t.modified(), !0;
-                        throw j("Set Enum outside numeric range ".concat(n, ", ").concat(a)), new RangeError("Set Enum outside numeric range")
+                        throw H("Set Enum outside numeric range ".concat(n, ", ").concat(a)), new RangeError("Set Enum outside numeric range")
                     }
                     return !1
                 }
-                throw j("Set Enum with invalid argument (String/Number) ".concat(n, ", ").concat(a)), new TypeError("Set Enum with invalid argument (String/Number)")
+                throw H("Set Enum with invalid argument (String/Number) ".concat(n, ", ").concat(a)), new TypeError("Set Enum with invalid argument (String/Number)")
             }
         }
     };
 
-    function S2(e) {
-        if (l0(e) === "object") {
-            var t = g3[e.type];
+    function B2(e) {
+        if (y0(e) === "object") {
+            var t = h3[e.type];
             if (t) return function(r, n) {
                 return t(r, n, e)
             };
-            throw j("No setter for field ".concat(e)), new TypeError("No setter for field")
+            throw H("No setter for field ".concat(e)), new TypeError("No setter for field")
         }
         return function(n, a) {
             return function(c) {
-                return a.deleted ? (j("instance deleted - cannot call any method"), !1) : a[e] !== c ? (a[e] = c, n.modified(), !0) : !1
+                return a.deleted ? (H("instance deleted - cannot call any method"), !1) : a[e] !== c ? (a[e] = c, n.modified(), !0) : !1
             }
         }
     }
 
-    function d1(e, t, r) {
+    function C1(e, t, r) {
         r.forEach(function(n) {
-            l0(n) === "object" ? e["set".concat(V(n.name))] = S2(n)(e, t) : e["set".concat(V(n))] = S2(n)(e, t)
+            y0(n) === "object" ? e["set".concat(I(n.name))] = B2(n)(e, t) : e["set".concat(I(n))] = B2(n)(e, t)
         })
     }
 
-    function w2(e, t, r) {
-        z0(e, t, r), d1(e, t, r)
+    function x2(e, t, r) {
+        I0(e, t, r), C1(e, t, r)
     }
 
-    function b2(e, t, r) {
+    function R2(e, t, r) {
         r.forEach(function(n) {
-            e["get".concat(V(n))] = function() {
+            e["get".concat(I(n))] = function() {
                 return t[n] ? [].concat(t[n]) : t[n]
-            }, e["get".concat(V(n), "ByReference")] = function() {
+            }, e["get".concat(I(n), "ByReference")] = function() {
                 return t[n]
             }
         })
     }
 
-    function N2(e, t, r, n) {
+    function O2(e, t, r, n) {
         var a = arguments.length > 4 && arguments[4] !== void 0 ? arguments[4] : void 0;
         r.forEach(function(o) {
             if (t[o] && n && t[o].length !== n) throw new RangeError("Invalid initial number of values for array (".concat(o, ")"));
-            e["set".concat(V(o))] = function() {
-                if (t.deleted) return j("instance deleted - cannot call any method"), !1;
-                for (var c = arguments.length, s = new Array(c), i = 0; i < c; i++) s[i] = arguments[i];
-                var u = s,
-                    l, p = !1;
-                if (u.length === 1 && (u[0] == null || u[0].length >= 0) && (u = u[0], p = !0), u == null) l = t[o] !== u;
+            e["set".concat(I(o))] = function() {
+                if (t.deleted) return H("instance deleted - cannot call any method"), !1;
+                for (var c = arguments.length, s = new Array(c), u = 0; u < c; u++) s[u] = arguments[u];
+                var i = s,
+                    f, g = !1;
+                if (i.length === 1 && (i[0] == null || i[0].length >= 0) && (i = i[0], g = !0), i == null) f = t[o] !== i;
                 else {
-                    if (n && u.length !== n)
-                        if (u.length < n && a !== void 0)
-                            for (u = Array.from(u), p = !1; u.length < n;) u.push(a);
+                    if (n && i.length !== n)
+                        if (i.length < n && a !== void 0)
+                            for (i = Array.from(i), g = !1; i.length < n;) i.push(a);
                         else throw new RangeError("Invalid number of values for array setter (".concat(o, ")"));
-                    l = t[o] == null || t[o].some(function(f, g) {
-                        return f !== u[g]
-                    }) || t[o].length !== u.length, l && p && (u = Array.from(u))
+                    f = t[o] == null || t[o].some(function(l, p) {
+                        return l !== i[p]
+                    }) || t[o].length !== i.length, f && g && (i = Array.from(i))
                 }
-                return l && (t[o] = u, e.modified()), l
-            }, e["set".concat(V(o), "From")] = function(c) {
+                return f && (t[o] = i, e.modified()), f
+            }, e["set".concat(I(o), "From")] = function(c) {
                 var s = t[o];
-                c.forEach(function(i, u) {
-                    s[u] = i
+                c.forEach(function(u, i) {
+                    s[i] = u
                 })
             }
         })
     }
 
-    function v3(e, t, r, n) {
+    function m3(e, t, r, n) {
         var a = arguments.length > 4 && arguments[4] !== void 0 ? arguments[4] : void 0;
-        b2(e, t, r), N2(e, t, r, n, a)
+        R2(e, t, r), O2(e, t, r, n, a)
     }
 
-    function y3(e, t, r) {
+    function C3(e, t, r) {
         for (var n = 0; n < r.length; n++) {
             var a = r[n];
             t[a] !== void 0 && (t["_".concat(a)] = t[a], delete t[a])
         }
     }
 
-    function d3(e, t, r, n) {
-        t.inputData ? t.inputData = t.inputData.map(v0) : t.inputData = [], t.inputConnection ? t.inputConnection = t.inputConnection.map(v0) : t.inputConnection = [], t.output ? t.output = t.output.map(v0) : t.output = [], t.inputArrayToProcess ? t.inputArrayToProcess = t.inputArrayToProcess.map(v0) : t.inputArrayToProcess = [], t.numberOfInputs = r;
+    function S3(e, t, r, n) {
+        t.inputData ? t.inputData = t.inputData.map(m0) : t.inputData = [], t.inputConnection ? t.inputConnection = t.inputConnection.map(m0) : t.inputConnection = [], t.output ? t.output = t.output.map(m0) : t.output = [], t.inputArrayToProcess ? t.inputArrayToProcess = t.inputArrayToProcess.map(m0) : t.inputArrayToProcess = [], t.numberOfInputs = r;
 
         function a(y) {
             var h = arguments.length > 1 && arguments[1] !== void 0 ? arguments[1] : 0;
             if (t.deleted) {
-                j("instance deleted - cannot call any method");
+                H("instance deleted - cannot call any method");
                 return
             }
             if (h >= t.numberOfInputs) {
-                j("algorithm ".concat(e.getClassName(), " only has ").concat(t.numberOfInputs, " input ports. To add more input ports, use addInputData()"));
+                H("algorithm ".concat(e.getClassName(), " only has ").concat(t.numberOfInputs, " input ports. To add more input ports, use addInputData()"));
                 return
             }(t.inputData[h] !== y || t.inputConnection[h]) && (t.inputData[h] = y, t.inputConnection[h] = null, e.modified && e.modified())
         }
 
         function o() {
             var y = arguments.length > 0 && arguments[0] !== void 0 ? arguments[0] : 0;
             return t.inputConnection[y] && (t.inputData[y] = t.inputConnection[y]()), t.inputData[y]
         }
 
         function c(y) {
             var h = arguments.length > 1 && arguments[1] !== void 0 ? arguments[1] : 0;
             if (t.deleted) {
-                j("instance deleted - cannot call any method");
+                H("instance deleted - cannot call any method");
                 return
             }
             if (h >= t.numberOfInputs) {
                 var C = "algorithm ".concat(e.getClassName(), " only has ");
-                C += "".concat(t.numberOfInputs), C += " input ports. To add more input ports, use addInputConnection()", j(C);
+                C += "".concat(t.numberOfInputs), C += " input ports. To add more input ports, use addInputConnection()", H(C);
                 return
             }
             t.inputData[h] = null, t.inputConnection[h] = y
         }
 
         function s() {
             var y = arguments.length > 0 && arguments[0] !== void 0 ? arguments[0] : 0;
             return t.inputConnection[y]
         }
 
-        function i() {
+        function u() {
             for (var y = t.numberOfInputs; y && !t.inputData[y - 1] && !t.inputConnection[y - 1];) y--;
             return y === t.numberOfInputs && t.numberOfInputs++, y
         }
 
-        function u(y) {
+        function i(y) {
             if (t.deleted) {
-                j("instance deleted - cannot call any method");
+                H("instance deleted - cannot call any method");
                 return
             }
-            c(y, i())
+            c(y, u())
         }
 
-        function l(y) {
+        function f(y) {
             if (t.deleted) {
-                j("instance deleted - cannot call any method");
+                H("instance deleted - cannot call any method");
                 return
             }
-            a(y, i())
+            a(y, u())
         }
 
-        function p() {
+        function g() {
             var y = arguments.length > 0 && arguments[0] !== void 0 ? arguments[0] : 0;
-            return t.deleted ? (j("instance deleted - cannot call any method"), null) : (e.shouldUpdate() && e.update(), t.output[y])
+            return t.deleted ? (H("instance deleted - cannot call any method"), null) : (e.shouldUpdate() && e.update(), t.output[y])
         }
         e.shouldUpdate = function() {
             for (var y = e.getMTime(), h = 1 / 0, C = n; C--;) {
                 if (!t.output[C] || t.output[C].isDeleted()) return !0;
                 var N = t.output[C].getMTime();
                 if (N < y) return !0;
                 N < h && (h = N)
             }
             for (C = t.numberOfInputs; C--;) {
-                var R, B;
-                if ((R = t.inputConnection[C]) !== null && R !== void 0 && R.filter.shouldUpdate() || ((B = e.getInputData(C)) === null || B === void 0 ? void 0 : B.getMTime()) > h) return !0
+                var x, B;
+                if ((x = t.inputConnection[C]) !== null && x !== void 0 && x.filter.shouldUpdate() || ((B = e.getInputData(C)) === null || B === void 0 ? void 0 : B.getMTime()) > h) return !0
             }
             return !1
         };
 
-        function f() {
+        function l() {
             var y = arguments.length > 0 && arguments[0] !== void 0 ? arguments[0] : 0,
                 h = function() {
-                    return p(y)
+                    return g(y)
                 };
             return h.filter = e, h
         }
         if (t.numberOfInputs) {
-            for (var g = t.numberOfInputs; g--;) t.inputData.push(null), t.inputConnection.push(null);
-            e.setInputData = a, e.setInputConnection = c, e.addInputData = l, e.addInputConnection = u, e.getInputData = o, e.getInputConnection = s
+            for (var p = t.numberOfInputs; p--;) t.inputData.push(null), t.inputConnection.push(null);
+            e.setInputData = a, e.setInputConnection = c, e.addInputData = f, e.addInputConnection = i, e.getInputData = o, e.getInputConnection = s
         }
-        n && (e.getOutputData = p, e.getOutputPort = f), e.update = function() {
+        n && (e.getOutputData = g, e.getOutputPort = l), e.update = function() {
             var y = [];
             if (t.numberOfInputs)
                 for (var h = 0; h < t.numberOfInputs;) y[h] = e.getInputData(h), h++;
             e.shouldUpdate() && e.requestData && e.requestData(y, t.output)
         }, e.getNumberOfInputPorts = function() {
             return t.numberOfInputs
         }, e.getNumberOfOutputPorts = function() {
@@ -2548,162 +2548,162 @@
             t.inputArrayToProcess[y] = {
                 arrayName: h,
                 fieldAssociation: C,
                 attributeType: N
             }
         }
     }
-    var B2 = Symbol("Event abort");
+    var T2 = Symbol("Event abort");
 
-    function h3(e, t, r) {
+    function w3(e, t, r) {
         var n = [],
             a = e.delete,
             o = 1;
 
-        function c(u) {
-            for (var l = 0; l < n.length; ++l) {
-                var p = r0(n[l], 1),
-                    f = p[0];
-                if (f === u) {
-                    n.splice(l, 1);
+        function c(i) {
+            for (var f = 0; f < n.length; ++f) {
+                var g = u0(n[f], 1),
+                    l = g[0];
+                if (l === i) {
+                    n.splice(f, 1);
                     return
                 }
             }
         }
 
-        function s(u) {
-            function l() {
-                c(u)
+        function s(i) {
+            function f() {
+                c(i)
             }
             return Object.freeze({
-                unsubscribe: l
+                unsubscribe: f
             })
         }
 
-        function i() {
-            var u = arguments;
+        function u() {
+            var i = arguments;
             if (t.deleted) {
-                j("instance deleted - cannot call any method");
+                H("instance deleted - cannot call any method");
                 return
             }
-            for (var l = n.slice(), p = function(h) {
-                    var C = r0(l[h], 3),
+            for (var f = n.slice(), g = function(h) {
+                    var C = u0(f[h], 3),
                         N = C[1],
-                        R = C[2];
+                        x = C[2];
                     if (!N) return "continue";
-                    if (R < 0) setTimeout(function() {
-                        return N.apply(e, u)
-                    }, 1 - R);
+                    if (x < 0) setTimeout(function() {
+                        return N.apply(e, i)
+                    }, 1 - x);
                     else {
-                        var B = N.apply(e, u);
-                        if (B === B2) return "break"
+                        var B = N.apply(e, i);
+                        if (B === T2) return "break"
                     }
-                }, f = 0; f < l.length; ++f) {
-                var g = p(f);
-                if (g !== "continue" && g === "break") break
+                }, l = 0; l < f.length; ++l) {
+                var p = g(l);
+                if (p !== "continue" && p === "break") break
             }
         }
-        e["invoke".concat(V(r))] = i, e["on".concat(V(r))] = function(u) {
-            var l = arguments.length > 1 && arguments[1] !== void 0 ? arguments[1] : 0;
-            if (!u.apply) return console.error("Invalid callback for event ".concat(r)), null;
-            if (t.deleted) return j("instance deleted - cannot call any method"), null;
-            var p = o++;
-            return n.push([p, u, l]), n.sort(function(f, g) {
-                return g[2] - f[2]
-            }), s(p)
+        e["invoke".concat(I(r))] = u, e["on".concat(I(r))] = function(i) {
+            var f = arguments.length > 1 && arguments[1] !== void 0 ? arguments[1] : 0;
+            if (!i.apply) return console.error("Invalid callback for event ".concat(r)), null;
+            if (t.deleted) return H("instance deleted - cannot call any method"), null;
+            var g = o++;
+            return n.push([g, i, f]), n.sort(function(l, p) {
+                return p[2] - l[2]
+            }), s(g)
         }, e.delete = function() {
-            a(), n.forEach(function(u) {
-                var l = r0(u, 1),
-                    p = l[0];
-                return c(p)
+            a(), n.forEach(function(i) {
+                var f = u0(i, 1),
+                    g = f[0];
+                return c(g)
             })
         }
     }
 
-    function R2(e, t) {
+    function M2(e, t) {
         var r = function() {
             var a = arguments.length > 0 && arguments[0] !== void 0 ? arguments[0] : {},
                 o = {},
                 c = {};
             return e(c, o, a), Object.freeze(c)
         };
-        return t && v0.register(t, r), r
+        return t && m0.register(t, r), r
     }
 
-    function m3() {
+    function b3() {
         for (var e = arguments.length, t = new Array(e), r = 0; r < e; r++) t[r] = arguments[r];
         return function() {
             for (var n = arguments.length, a = new Array(n), o = 0; o < n; o++) a[o] = arguments[o];
             return t.filter(function(c) {
                 return !!c
             }).map(function(c) {
                 return c.apply(void 0, a)
             })
         }
     }
 
-    function x2(e) {
+    function G2(e) {
         return e && e.isA && e.isA("vtkObject")
     }
 
-    function h1(e, t) {
+    function S1(e, t) {
         var r = arguments.length > 2 && arguments[2] !== void 0 ? arguments[2] : [],
             n = arguments.length > 3 && arguments[3] !== void 0 ? arguments[3] : [];
-        if (x2(e)) {
+        if (G2(e)) {
             if (n.indexOf(e) >= 0) return r;
             n.push(e);
             var a = t(e);
             a !== void 0 && r.push(a);
             var o = e.get();
             Object.keys(o).forEach(function(c) {
                 var s = o[c];
-                Array.isArray(s) ? s.forEach(function(i) {
-                    h1(i, t, r, n)
-                }) : h1(s, t, r, n)
+                Array.isArray(s) ? s.forEach(function(u) {
+                    S1(u, t, r, n)
+                }) : S1(s, t, r, n)
             })
         }
         return r
     }
 
-    function C3(e, t, r) {
+    function N3(e, t, r) {
         var n = this,
             a, o = function() {
-                for (var s = arguments.length, i = new Array(s), u = 0; u < s; u++) i[u] = arguments[u];
-                var l = n,
-                    p = function() {
-                        a = null, r || e.apply(l, i)
+                for (var s = arguments.length, u = new Array(s), i = 0; i < s; i++) u[i] = arguments[i];
+                var f = n,
+                    g = function() {
+                        a = null, r || e.apply(f, u)
                     },
-                    f = r && !a;
-                clearTimeout(a), a = setTimeout(p, t), f && e.apply(l, i)
+                    l = r && !a;
+                clearTimeout(a), a = setTimeout(g, t), l && e.apply(f, u)
             };
         return o.cancel = function() {
             return clearTimeout(a)
         }, o
     }
 
-    function S3(e, t) {
+    function B3(e, t) {
         var r = !1,
             n = null;
 
         function a() {
-            r = !1, n !== null && (o.apply(void 0, r1(n)), n = null)
+            r = !1, n !== null && (o.apply(void 0, o1(n)), n = null)
         }
 
         function o() {
-            for (var c = arguments.length, s = new Array(c), i = 0; i < c; i++) s[i] = arguments[i];
+            for (var c = arguments.length, s = new Array(c), u = 0; u < c; u++) s[u] = arguments[u];
             if (r) {
                 n = s;
                 return
             }
             r = !0, e.apply(void 0, s), setTimeout(a, t)
         }
         return o
     }
 
-    function O2(e, t) {
+    function E2(e, t) {
         var r = arguments.length > 2 && arguments[2] !== void 0 ? arguments[2] : {};
         t.keystore = Object.assign(t.keystore || {}, r), e.setKey = function(n, a) {
             t.keystore[n] = a
         }, e.getKey = function(n) {
             return t.keystore[n]
         }, e.getAllKeys = function() {
             return Object.keys(t.keystore)
@@ -2711,701 +2711,701 @@
             return delete t.keystore[n]
         }, e.clearKeystore = function() {
             return e.getAllKeys().forEach(function(n) {
                 return delete t.keystore[n]
             })
         }
     }
-    var w3 = 1,
-        H0 = "__root__";
+    var x3 = 1,
+        W0 = "__root__";
 
-    function b3(e, t) {
-        O2(e, t);
+    function R3(e, t) {
+        E2(e, t);
         var r = e.delete;
-        t.proxyId = "".concat(w3++), t.ui = JSON.parse(JSON.stringify(t.ui || [])), z0(e, t, ["proxyId", "proxyGroup", "proxyName"]), w2(e, t, ["proxyManager"]);
+        t.proxyId = "".concat(x3++), t.ui = JSON.parse(JSON.stringify(t.ui || [])), I0(e, t, ["proxyId", "proxyGroup", "proxyName"]), x2(e, t, ["proxyManager"]);
         var n = {},
             a = {};
 
-        function o(u, l) {
-            a[l] || (a[l] = []);
-            for (var p = a[l], f = 0; f < u.length; f++) p.push(u[f].name), n[u[f].name] = u[f], u[f].children && u[f].children.length && o(u[f].children, u[f].name)
-        }
-        o(t.ui, H0), e.updateUI = function(u) {
-            t.ui = JSON.parse(JSON.stringify(u || [])), Object.keys(n).forEach(function(l) {
-                return delete n[l]
-            }), Object.keys(a).forEach(function(l) {
-                return delete a[l]
-            }), o(t.ui, H0), e.modified()
+        function o(i, f) {
+            a[f] || (a[f] = []);
+            for (var g = a[f], l = 0; l < i.length; l++) g.push(i[l].name), n[i[l].name] = i[l], i[l].children && i[l].children.length && o(i[l].children, i[l].name)
+        }
+        o(t.ui, W0), e.updateUI = function(i) {
+            t.ui = JSON.parse(JSON.stringify(i || [])), Object.keys(n).forEach(function(f) {
+                return delete n[f]
+            }), Object.keys(a).forEach(function(f) {
+                return delete a[f]
+            }), o(t.ui, W0), e.modified()
         };
 
         function c() {
-            var u = arguments.length > 0 && arguments[0] !== void 0 ? arguments[0] : H0;
-            return a[u]
+            var i = arguments.length > 0 && arguments[0] !== void 0 ? arguments[0] : W0;
+            return a[i]
         }
-        e.updateProxyProperty = function(u, l) {
-            var p = n[u];
-            p ? Object.assign(p, l) : n[u] = p1({}, l)
+        e.updateProxyProperty = function(i, f) {
+            var g = n[i];
+            g ? Object.assign(g, f) : n[i] = y1({}, f)
         }, e.activate = function() {
             if (t.proxyManager) {
-                var u = "setActive".concat(V(e.getProxyGroup().slice(0, -1)));
-                t.proxyManager[u] && t.proxyManager[u](e)
+                var i = "setActive".concat(I(e.getProxyGroup().slice(0, -1)));
+                t.proxyManager[i] && t.proxyManager[i](e)
             }
-        }, t.propertyLinkSubscribers = {}, e.registerPropertyLinkForGC = function(u, l) {
-            l in t.propertyLinkSubscribers || (t.propertyLinkSubscribers[l] = []), t.propertyLinkSubscribers[l].push(u)
-        }, e.gcPropertyLinks = function(u) {
-            for (var l = t.propertyLinkSubscribers[u] || []; l.length;) l.pop().unbind(e)
-        }, t.propertyLinkMap = {}, e.getPropertyLink = function(u) {
-            var l = arguments.length > 1 && arguments[1] !== void 0 ? arguments[1] : !1;
-            if (t.propertyLinkMap[u]) return t.propertyLinkMap[u];
-            var p = null,
-                f = [],
-                g = 0,
+        }, t.propertyLinkSubscribers = {}, e.registerPropertyLinkForGC = function(i, f) {
+            f in t.propertyLinkSubscribers || (t.propertyLinkSubscribers[f] = []), t.propertyLinkSubscribers[f].push(i)
+        }, e.gcPropertyLinks = function(i) {
+            for (var f = t.propertyLinkSubscribers[i] || []; f.length;) f.pop().unbind(e)
+        }, t.propertyLinkMap = {}, e.getPropertyLink = function(i) {
+            var f = arguments.length > 1 && arguments[1] !== void 0 ? arguments[1] : !1;
+            if (t.propertyLinkMap[i]) return t.propertyLinkMap[i];
+            var g = null,
+                l = [],
+                p = 0,
                 y = !1;
 
-            function h(w) {
+            function h(b) {
                 var S = arguments.length > 1 && arguments[1] !== void 0 ? arguments[1] : !1;
                 if (y) return null;
-                var b = [],
+                var w = [],
                     v = null;
-                for (g = f.length; g--;) {
-                    var d = f[g];
-                    d.instance === w ? v = d : b.push(d)
+                for (p = l.length; p--;) {
+                    var d = l[p];
+                    d.instance === b ? v = d : w.push(d)
                 }
                 if (!v) return null;
-                var m = v.instance["get".concat(V(v.propertyName))]();
-                if (!f3(m, p) || S) {
-                    for (p = m, y = !0; b.length;) {
-                        var x = b.pop();
-                        x.instance.set(f0({}, x.propertyName, p))
+                var m = v.instance["get".concat(I(v.propertyName))]();
+                if (!v3(m, g) || S) {
+                    for (g = m, y = !0; w.length;) {
+                        var O = w.pop();
+                        O.instance.set(v0({}, O.propertyName, g))
                     }
                     y = !1
                 }
-                return t.propertyLinkMap[u].persistent && (t.propertyLinkMap[u].value = m), m
+                return t.propertyLinkMap[i].persistent && (t.propertyLinkMap[i].value = m), m
             }
 
-            function C(w, S) {
-                var b = [];
-                for (g = f.length; g--;) {
-                    var v = f[g];
-                    v.instance === w && (v.propertyName === S || S === void 0) && (v.subscription.unsubscribe(), b.push(g))
+            function C(b, S) {
+                var w = [];
+                for (p = l.length; p--;) {
+                    var v = l[p];
+                    v.instance === b && (v.propertyName === S || S === void 0) && (v.subscription.unsubscribe(), w.push(p))
                 }
-                for (; b.length;) f.splice(b.pop(), 1)
+                for (; w.length;) l.splice(w.pop(), 1)
             }
 
-            function N(w, S) {
-                var b = arguments.length > 2 && arguments[2] !== void 0 ? arguments[2] : !1,
-                    v = w.onModified(h),
-                    d = f[0];
-                return f.push({
-                    instance: w,
+            function N(b, S) {
+                var w = arguments.length > 2 && arguments[2] !== void 0 ? arguments[2] : !1,
+                    v = b.onModified(h),
+                    d = l[0];
+                return l.push({
+                    instance: b,
                     propertyName: S,
                     subscription: v
-                }), b && (t.propertyLinkMap[u].persistent && t.propertyLinkMap[u].value !== void 0 ? w.set(f0({}, S, t.propertyLinkMap[u].value)) : d && h(d.instance, !0)), {
+                }), w && (t.propertyLinkMap[i].persistent && t.propertyLinkMap[i].value !== void 0 ? b.set(v0({}, S, t.propertyLinkMap[i].value)) : d && h(d.instance, !0)), {
                     unsubscribe: function() {
-                        return C(w, S)
+                        return C(b, S)
                     }
                 }
             }
 
-            function R() {
-                for (; f.length;) f.pop().subscription.unsubscribe()
+            function x() {
+                for (; l.length;) l.pop().subscription.unsubscribe()
             }
             var B = {
                 bind: N,
                 unbind: C,
-                unsubscribe: R,
-                persistent: l
+                unsubscribe: x,
+                persistent: f
             };
-            return t.propertyLinkMap[u] = B, B
+            return t.propertyLinkMap[i] = B, B
         };
 
         function s() {
-            for (var u = arguments.length > 0 && arguments[0] !== void 0 ? arguments[0] : H0, l = [], p = t.proxyId, f = c(u) || [], g = 0; g < f.length; g++) {
-                var y = f[g],
-                    h = e["get".concat(V(y))],
+            for (var i = arguments.length > 0 && arguments[0] !== void 0 ? arguments[0] : W0, f = [], g = t.proxyId, l = c(i) || [], p = 0; p < l.length; p++) {
+                var y = l[p],
+                    h = e["get".concat(I(y))],
                     C = h ? h() : void 0,
                     N = {
-                        id: p,
+                        id: g,
                         name: y,
                         value: C
                     },
-                    R = s(y);
-                R.length && (N.children = R), l.push(N)
+                    x = s(y);
+                x.length && (N.children = x), f.push(N)
             }
-            return l
+            return f
         }
         e.listPropertyNames = function() {
-            return s().map(function(u) {
-                return u.name
+            return s().map(function(i) {
+                return i.name
             })
-        }, e.getPropertyByName = function(u) {
-            return s().find(function(l) {
-                return l.name === u
+        }, e.getPropertyByName = function(i) {
+            return s().find(function(f) {
+                return f.name === i
             })
-        }, e.getPropertyDomainByName = function(u) {
-            return (n[u] || {}).domain
+        }, e.getPropertyDomainByName = function(i) {
+            return (n[i] || {}).domain
         }, e.getProxySection = function() {
             return {
                 id: t.proxyId,
                 name: t.proxyGroup,
                 ui: t.ui,
                 properties: s()
             }
         }, e.delete = function() {
-            for (var u = Object.keys(t.propertyLinkMap), l = u.length; l--;) t.propertyLinkMap[u[l]].unsubscribe();
+            for (var i = Object.keys(t.propertyLinkMap), f = i.length; f--;) t.propertyLinkMap[i[f]].unsubscribe();
             Object.keys(t.propertyLinkSubscribers).forEach(e.gcPropertyLinks), r()
         }, e.getState = function() {
             return null
         };
 
-        function i() {
+        function u() {
             if (t.links)
-                for (var u = 0; u < t.links.length; u++) {
-                    var l = t.links[u],
-                        p = l.link,
-                        f = l.property,
-                        g = l.persistent,
-                        y = l.updateOnBind,
-                        h = l.type;
+                for (var i = 0; i < t.links.length; i++) {
+                    var f = t.links[i],
+                        g = f.link,
+                        l = f.property,
+                        p = f.persistent,
+                        y = f.updateOnBind,
+                        h = f.type;
                     if (h === "application") {
-                        var C = t.proxyManager.getPropertyLink(p, g);
-                        e.registerPropertyLinkForGC(C, "application"), C.bind(e, f, y)
+                        var C = t.proxyManager.getPropertyLink(g, p);
+                        e.registerPropertyLinkForGC(C, "application"), C.bind(e, l, y)
                     }
                 }
         }
-        m2(i)
+        b2(u)
     }
 
-    function N3(e, t, r) {
+    function O3(e, t, r) {
         for (var n = e.delete, a = [], o = Object.keys(r), c = o.length; c--;) {
             var s = o[c],
-                i = r[s],
-                u = i.modelKey,
-                l = i.property,
-                p = i.modified,
-                f = p === void 0 ? !0 : p,
-                g = V(l),
-                y = V(s);
-            e["get".concat(y)] = t[u]["get".concat(g)], e["set".concat(y)] = t[u]["set".concat(g)], f && a.push(t[u].onModified(e.modified))
+                u = r[s],
+                i = u.modelKey,
+                f = u.property,
+                g = u.modified,
+                l = g === void 0 ? !0 : g,
+                p = I(f),
+                y = I(s);
+            e["get".concat(y)] = t[i]["get".concat(p)], e["set".concat(y)] = t[i]["set".concat(p)], l && a.push(t[i].onModified(e.modified))
         }
         e.delete = function() {
             for (; a.length;) a.pop().unsubscribe();
             n()
         }
     }
 
-    function B3(e, t) {
+    function T3(e, t) {
         var r = arguments.length > 2 && arguments[2] !== void 0 ? arguments[2] : {},
             n = arguments.length > 3 && arguments[3] !== void 0 ? arguments[3] : {};
         t.this = e;
 
-        function a(i) {
-            for (var u = Object.keys(i), l = u.length; l--;) {
-                var p = u[l];
-                t[p].set(i[p])
+        function a(u) {
+            for (var i = Object.keys(u), f = i.length; f--;) {
+                var g = i[f];
+                t[g].set(u[g])
             }
         }
         for (var o = Object.keys(n), c = o.length, s = function() {
-                var u = o[c];
-                t[u] = n[u];
-                var l = r[u];
-                e["set".concat(V(u))] = function(p) {
-                    if (p !== t[u]) {
-                        t[u] = p;
-                        var f = l[p];
-                        a(f), e.modified()
+                var i = o[c];
+                t[i] = n[i];
+                var f = r[i];
+                e["set".concat(I(i))] = function(g) {
+                    if (g !== t[i]) {
+                        t[i] = g;
+                        var l = f[g];
+                        a(l), e.modified()
                     }
                 }
             }; c--;) s();
-        o.length && z0(e, t, o)
+        o.length && I0(e, t, o)
     }
-    var T2 = 10,
-        M2 = 40,
-        G2 = 800;
+    var k2 = 10,
+        D2 = 40,
+        L2 = 800;
 
-    function R3(e) {
+    function M3(e) {
         var t = 0,
             r = 0,
             n = 0,
             a = 0;
-        return "detail" in e && (r = e.detail), "wheelDelta" in e && (r = -e.wheelDelta / 120), "wheelDeltaY" in e && (r = -e.wheelDeltaY / 120), "wheelDeltaX" in e && (t = -e.wheelDeltaX / 120), "axis" in e && e.axis === e.HORIZONTAL_AXIS && (t = r, r = 0), n = t * T2, a = r * T2, "deltaY" in e && (a = e.deltaY), "deltaX" in e && (n = e.deltaX), (n || a) && e.deltaMode && (e.deltaMode === 1 ? (n *= M2, a *= M2) : (n *= G2, a *= G2)), n && !t && (t = n < 1 ? -1 : 1), a && !r && (r = a < 1 ? -1 : 1), {
+        return "detail" in e && (r = e.detail), "wheelDelta" in e && (r = -e.wheelDelta / 120), "wheelDeltaY" in e && (r = -e.wheelDeltaY / 120), "wheelDeltaX" in e && (t = -e.wheelDeltaX / 120), "axis" in e && e.axis === e.HORIZONTAL_AXIS && (t = r, r = 0), n = t * k2, a = r * k2, "deltaY" in e && (a = e.deltaY), "deltaX" in e && (n = e.deltaX), (n || a) && e.deltaMode && (e.deltaMode === 1 ? (n *= D2, a *= D2) : (n *= L2, a *= L2)), n && !t && (t = n < 1 ? -1 : 1), a && !r && (r = a < 1 ? -1 : 1), {
             spinX: t,
             spinY: r,
             pixelX: n,
             pixelY: a
         }
     }
-    var z = {
-            algo: d3,
-            capitalize: y1,
-            chain: m3,
-            debounce: C3,
-            enumToString: l3,
-            event: h3,
-            EVENT_ABORT: B2,
-            formatBytesToProperUnit: s3,
-            formatNumbersWithThousandSeparator: c3,
-            get: z0,
-            getArray: b2,
-            getCurrentGlobalMTime: t3,
-            getStateArrayMapFunc: h2,
-            isVtkObject: x2,
-            keystore: O2,
-            measurePromiseExecution: p3,
-            moveToProtected: y3,
-            newInstance: R2,
-            newTypedArray: v2,
-            newTypedArrayFrom: y2,
-            normalizeWheel: R3,
-            obj: C2,
-            proxy: b3,
-            proxyPropertyMapping: N3,
-            proxyPropertyState: B3,
-            safeArrays: d2,
-            set: d1,
-            setArray: N2,
-            setGet: w2,
-            setGetArray: v3,
-            setImmediate: m2,
-            setLoggerFunction: n3,
-            throttle: S3,
-            traverseInstanceTree: h1,
-            TYPED_ARRAYS: K,
-            uncapitalize: u3,
-            VOID: e3,
-            vtkDebugMacro: v1,
-            vtkErrorMacro: j,
-            vtkInfoMacro: o3,
-            vtkLogMacro: a3,
-            vtkOnceErrorMacro: i3,
-            vtkWarningMacro: p2
+    var W = {
+            algo: S3,
+            capitalize: m1,
+            chain: b3,
+            debounce: N3,
+            enumToString: y3,
+            event: w3,
+            EVENT_ABORT: T2,
+            formatBytesToProperUnit: g3,
+            formatNumbersWithThousandSeparator: p3,
+            get: I0,
+            getArray: R2,
+            getCurrentGlobalMTime: o3,
+            getStateArrayMapFunc: w2,
+            isVtkObject: G2,
+            keystore: E2,
+            measurePromiseExecution: d3,
+            moveToProtected: C3,
+            newInstance: M2,
+            newTypedArray: m2,
+            newTypedArrayFrom: C2,
+            normalizeWheel: M3,
+            obj: N2,
+            proxy: R3,
+            proxyPropertyMapping: O3,
+            proxyPropertyState: T3,
+            safeArrays: S2,
+            set: C1,
+            setArray: O2,
+            setGet: x2,
+            setGetArray: m3,
+            setImmediate: b2,
+            setLoggerFunction: u3,
+            throttle: B3,
+            traverseInstanceTree: S1,
+            TYPED_ARRAYS: t0,
+            uncapitalize: f3,
+            VOID: a3,
+            vtkDebugMacro: h1,
+            vtkErrorMacro: H,
+            vtkInfoMacro: c3,
+            vtkLogMacro: s3,
+            vtkOnceErrorMacro: l3,
+            vtkWarningMacro: d2
         },
-        m1 = {},
-        x3 = {
+        w1 = {},
+        G3 = {
             get exports() {
-                return m1
+                return w1
             },
             set exports(e) {
-                m1 = e
+                w1 = e
             }
         };
     (function(e) {
         (function(t, r, n) {
-            function a(i) {
-                var u = this,
-                    l = s();
-                u.next = function() {
-                    var p = 2091639 * u.s0 + u.c * 23283064365386963e-26;
-                    return u.s0 = u.s1, u.s1 = u.s2, u.s2 = p - (u.c = p | 0)
-                }, u.c = 1, u.s0 = l(" "), u.s1 = l(" "), u.s2 = l(" "), u.s0 -= l(i), u.s0 < 0 && (u.s0 += 1), u.s1 -= l(i), u.s1 < 0 && (u.s1 += 1), u.s2 -= l(i), u.s2 < 0 && (u.s2 += 1), l = null
-            }
-
-            function o(i, u) {
-                return u.c = i.c, u.s0 = i.s0, u.s1 = i.s1, u.s2 = i.s2, u
-            }
-
-            function c(i, u) {
-                var l = new a(i),
-                    p = u && u.state,
-                    f = l.next;
-                return f.int32 = function() {
-                    return l.next() * 4294967296 | 0
-                }, f.double = function() {
-                    return f() + (f() * 2097152 | 0) * 11102230246251565e-32
-                }, f.quick = f, p && (typeof p == "object" && o(p, l), f.state = function() {
-                    return o(l, {})
-                }), f
+            function a(u) {
+                var i = this,
+                    f = s();
+                i.next = function() {
+                    var g = 2091639 * i.s0 + i.c * 23283064365386963e-26;
+                    return i.s0 = i.s1, i.s1 = i.s2, i.s2 = g - (i.c = g | 0)
+                }, i.c = 1, i.s0 = f(" "), i.s1 = f(" "), i.s2 = f(" "), i.s0 -= f(u), i.s0 < 0 && (i.s0 += 1), i.s1 -= f(u), i.s1 < 0 && (i.s1 += 1), i.s2 -= f(u), i.s2 < 0 && (i.s2 += 1), f = null
+            }
+
+            function o(u, i) {
+                return i.c = u.c, i.s0 = u.s0, i.s1 = u.s1, i.s2 = u.s2, i
+            }
+
+            function c(u, i) {
+                var f = new a(u),
+                    g = i && i.state,
+                    l = f.next;
+                return l.int32 = function() {
+                    return f.next() * 4294967296 | 0
+                }, l.double = function() {
+                    return l() + (l() * 2097152 | 0) * 11102230246251565e-32
+                }, l.quick = l, g && (typeof g == "object" && o(g, f), l.state = function() {
+                    return o(f, {})
+                }), l
             }
 
             function s() {
-                var i = 4022871197,
-                    u = function(l) {
-                        l = String(l);
-                        for (var p = 0; p < l.length; p++) {
-                            i += l.charCodeAt(p);
-                            var f = .02519603282416938 * i;
-                            i = f >>> 0, f -= i, f *= i, i = f >>> 0, f -= i, i += f * 4294967296
+                var u = 4022871197,
+                    i = function(f) {
+                        f = String(f);
+                        for (var g = 0; g < f.length; g++) {
+                            u += f.charCodeAt(g);
+                            var l = .02519603282416938 * u;
+                            u = l >>> 0, l -= u, l *= u, u = l >>> 0, l -= u, u += l * 4294967296
                         }
-                        return (i >>> 0) * 23283064365386963e-26
+                        return (u >>> 0) * 23283064365386963e-26
                     };
-                return u
+                return i
             }
             r && r.exports ? r.exports = c : n && n.amd ? n(function() {
                 return c
             }) : this.alea = c
-        })(q, e, !1)
-    })(x3);
-    var C1 = {},
-        O3 = {
+        })(e0, e, !1)
+    })(G3);
+    var b1 = {},
+        E3 = {
             get exports() {
-                return C1
+                return b1
             },
             set exports(e) {
-                C1 = e
+                b1 = e
             }
         };
     (function(e) {
         (function(t, r, n) {
             function a(s) {
-                var i = this,
-                    u = "";
-                i.x = 0, i.y = 0, i.z = 0, i.w = 0, i.next = function() {
-                    var p = i.x ^ i.x << 11;
-                    return i.x = i.y, i.y = i.z, i.z = i.w, i.w ^= i.w >>> 19 ^ p ^ p >>> 8
-                }, s === (s | 0) ? i.x = s : u += s;
-                for (var l = 0; l < u.length + 64; l++) i.x ^= u.charCodeAt(l) | 0, i.next()
-            }
-
-            function o(s, i) {
-                return i.x = s.x, i.y = s.y, i.z = s.z, i.w = s.w, i
-            }
-
-            function c(s, i) {
-                var u = new a(s),
-                    l = i && i.state,
-                    p = function() {
-                        return (u.next() >>> 0) / 4294967296
+                var u = this,
+                    i = "";
+                u.x = 0, u.y = 0, u.z = 0, u.w = 0, u.next = function() {
+                    var g = u.x ^ u.x << 11;
+                    return u.x = u.y, u.y = u.z, u.z = u.w, u.w ^= u.w >>> 19 ^ g ^ g >>> 8
+                }, s === (s | 0) ? u.x = s : i += s;
+                for (var f = 0; f < i.length + 64; f++) u.x ^= i.charCodeAt(f) | 0, u.next()
+            }
+
+            function o(s, u) {
+                return u.x = s.x, u.y = s.y, u.z = s.z, u.w = s.w, u
+            }
+
+            function c(s, u) {
+                var i = new a(s),
+                    f = u && u.state,
+                    g = function() {
+                        return (i.next() >>> 0) / 4294967296
                     };
-                return p.double = function() {
-                    do var f = u.next() >>> 11,
-                        g = (u.next() >>> 0) / 4294967296,
-                        y = (f + g) / (1 << 21); while (y === 0);
+                return g.double = function() {
+                    do var l = i.next() >>> 11,
+                        p = (i.next() >>> 0) / 4294967296,
+                        y = (l + p) / (1 << 21); while (y === 0);
                     return y
-                }, p.int32 = u.next, p.quick = p, l && (typeof l == "object" && o(l, u), p.state = function() {
-                    return o(u, {})
-                }), p
+                }, g.int32 = i.next, g.quick = g, f && (typeof f == "object" && o(f, i), g.state = function() {
+                    return o(i, {})
+                }), g
             }
             r && r.exports ? r.exports = c : n && n.amd ? n(function() {
                 return c
             }) : this.xor128 = c
-        })(q, e, !1)
-    })(O3);
-    var S1 = {},
-        T3 = {
+        })(e0, e, !1)
+    })(E3);
+    var N1 = {},
+        k3 = {
             get exports() {
-                return S1
+                return N1
             },
             set exports(e) {
-                S1 = e
+                N1 = e
             }
         };
     (function(e) {
         (function(t, r, n) {
             function a(s) {
-                var i = this,
-                    u = "";
-                i.next = function() {
-                    var p = i.x ^ i.x >>> 2;
-                    return i.x = i.y, i.y = i.z, i.z = i.w, i.w = i.v, (i.d = i.d + 362437 | 0) + (i.v = i.v ^ i.v << 4 ^ (p ^ p << 1)) | 0
-                }, i.x = 0, i.y = 0, i.z = 0, i.w = 0, i.v = 0, s === (s | 0) ? i.x = s : u += s;
-                for (var l = 0; l < u.length + 64; l++) i.x ^= u.charCodeAt(l) | 0, l == u.length && (i.d = i.x << 10 ^ i.x >>> 4), i.next()
+                var u = this,
+                    i = "";
+                u.next = function() {
+                    var g = u.x ^ u.x >>> 2;
+                    return u.x = u.y, u.y = u.z, u.z = u.w, u.w = u.v, (u.d = u.d + 362437 | 0) + (u.v = u.v ^ u.v << 4 ^ (g ^ g << 1)) | 0
+                }, u.x = 0, u.y = 0, u.z = 0, u.w = 0, u.v = 0, s === (s | 0) ? u.x = s : i += s;
+                for (var f = 0; f < i.length + 64; f++) u.x ^= i.charCodeAt(f) | 0, f == i.length && (u.d = u.x << 10 ^ u.x >>> 4), u.next()
             }
 
-            function o(s, i) {
-                return i.x = s.x, i.y = s.y, i.z = s.z, i.w = s.w, i.v = s.v, i.d = s.d, i
+            function o(s, u) {
+                return u.x = s.x, u.y = s.y, u.z = s.z, u.w = s.w, u.v = s.v, u.d = s.d, u
             }
 
-            function c(s, i) {
-                var u = new a(s),
-                    l = i && i.state,
-                    p = function() {
-                        return (u.next() >>> 0) / 4294967296
+            function c(s, u) {
+                var i = new a(s),
+                    f = u && u.state,
+                    g = function() {
+                        return (i.next() >>> 0) / 4294967296
                     };
-                return p.double = function() {
-                    do var f = u.next() >>> 11,
-                        g = (u.next() >>> 0) / 4294967296,
-                        y = (f + g) / (1 << 21); while (y === 0);
+                return g.double = function() {
+                    do var l = i.next() >>> 11,
+                        p = (i.next() >>> 0) / 4294967296,
+                        y = (l + p) / (1 << 21); while (y === 0);
                     return y
-                }, p.int32 = u.next, p.quick = p, l && (typeof l == "object" && o(l, u), p.state = function() {
-                    return o(u, {})
-                }), p
+                }, g.int32 = i.next, g.quick = g, f && (typeof f == "object" && o(f, i), g.state = function() {
+                    return o(i, {})
+                }), g
             }
             r && r.exports ? r.exports = c : n && n.amd ? n(function() {
                 return c
             }) : this.xorwow = c
-        })(q, e, !1)
-    })(T3);
-    var w1 = {},
-        M3 = {
+        })(e0, e, !1)
+    })(k3);
+    var B1 = {},
+        D3 = {
             get exports() {
-                return w1
+                return B1
             },
             set exports(e) {
-                w1 = e
+                B1 = e
             }
         };
     (function(e) {
         (function(t, r, n) {
             function a(s) {
-                var i = this;
-                i.next = function() {
-                    var l = i.x,
-                        p = i.i,
-                        f, g;
-                    return f = l[p], f ^= f >>> 7, g = f ^ f << 24, f = l[p + 1 & 7], g ^= f ^ f >>> 10, f = l[p + 3 & 7], g ^= f ^ f >>> 3, f = l[p + 4 & 7], g ^= f ^ f << 7, f = l[p + 7 & 7], f = f ^ f << 13, g ^= f ^ f << 9, l[p] = g, i.i = p + 1 & 7, g
+                var u = this;
+                u.next = function() {
+                    var f = u.x,
+                        g = u.i,
+                        l, p;
+                    return l = f[g], l ^= l >>> 7, p = l ^ l << 24, l = f[g + 1 & 7], p ^= l ^ l >>> 10, l = f[g + 3 & 7], p ^= l ^ l >>> 3, l = f[g + 4 & 7], p ^= l ^ l << 7, l = f[g + 7 & 7], l = l ^ l << 13, p ^= l ^ l << 9, f[g] = p, u.i = g + 1 & 7, p
                 };
 
-                function u(l, p) {
-                    var f, g = [];
-                    if (p === (p | 0)) g[0] = p;
+                function i(f, g) {
+                    var l, p = [];
+                    if (g === (g | 0)) p[0] = g;
                     else
-                        for (p = "" + p, f = 0; f < p.length; ++f) g[f & 7] = g[f & 7] << 15 ^ p.charCodeAt(f) + g[f + 1 & 7] << 13;
-                    for (; g.length < 8;) g.push(0);
-                    for (f = 0; f < 8 && g[f] === 0; ++f);
-                    for (f == 8 ? g[7] = -1 : g[f], l.x = g, l.i = 0, f = 256; f > 0; --f) l.next()
+                        for (g = "" + g, l = 0; l < g.length; ++l) p[l & 7] = p[l & 7] << 15 ^ g.charCodeAt(l) + p[l + 1 & 7] << 13;
+                    for (; p.length < 8;) p.push(0);
+                    for (l = 0; l < 8 && p[l] === 0; ++l);
+                    for (l == 8 ? p[7] = -1 : p[l], f.x = p, f.i = 0, l = 256; l > 0; --l) f.next()
                 }
-                u(i, s)
+                i(u, s)
             }
 
-            function o(s, i) {
-                return i.x = s.x.slice(), i.i = s.i, i
+            function o(s, u) {
+                return u.x = s.x.slice(), u.i = s.i, u
             }
 
-            function c(s, i) {
+            function c(s, u) {
                 s == null && (s = +new Date);
-                var u = new a(s),
-                    l = i && i.state,
-                    p = function() {
-                        return (u.next() >>> 0) / 4294967296
+                var i = new a(s),
+                    f = u && u.state,
+                    g = function() {
+                        return (i.next() >>> 0) / 4294967296
                     };
-                return p.double = function() {
-                    do var f = u.next() >>> 11,
-                        g = (u.next() >>> 0) / 4294967296,
-                        y = (f + g) / (1 << 21); while (y === 0);
+                return g.double = function() {
+                    do var l = i.next() >>> 11,
+                        p = (i.next() >>> 0) / 4294967296,
+                        y = (l + p) / (1 << 21); while (y === 0);
                     return y
-                }, p.int32 = u.next, p.quick = p, l && (l.x && o(l, u), p.state = function() {
-                    return o(u, {})
-                }), p
+                }, g.int32 = i.next, g.quick = g, f && (f.x && o(f, i), g.state = function() {
+                    return o(i, {})
+                }), g
             }
             r && r.exports ? r.exports = c : n && n.amd ? n(function() {
                 return c
             }) : this.xorshift7 = c
-        })(q, e, !1)
-    })(M3);
-    var b1 = {},
-        G3 = {
+        })(e0, e, !1)
+    })(D3);
+    var x1 = {},
+        L3 = {
             get exports() {
-                return b1
+                return x1
             },
             set exports(e) {
-                b1 = e
+                x1 = e
             }
         };
     (function(e) {
         (function(t, r, n) {
             function a(s) {
-                var i = this;
-                i.next = function() {
-                    var l = i.w,
-                        p = i.X,
-                        f = i.i,
-                        g, y;
-                    return i.w = l = l + 1640531527 | 0, y = p[f + 34 & 127], g = p[f = f + 1 & 127], y ^= y << 13, g ^= g << 17, y ^= y >>> 15, g ^= g >>> 12, y = p[f] = y ^ g, i.i = f, y + (l ^ l >>> 16) | 0
+                var u = this;
+                u.next = function() {
+                    var f = u.w,
+                        g = u.X,
+                        l = u.i,
+                        p, y;
+                    return u.w = f = f + 1640531527 | 0, y = g[l + 34 & 127], p = g[l = l + 1 & 127], y ^= y << 13, p ^= p << 17, y ^= y >>> 15, p ^= p >>> 12, y = g[l] = y ^ p, u.i = l, y + (f ^ f >>> 16) | 0
                 };
 
-                function u(l, p) {
-                    var f, g, y, h, C, N = [],
-                        R = 128;
-                    for (p === (p | 0) ? (g = p, p = null) : (p = p + "\0", g = 0, R = Math.max(R, p.length)), y = 0, h = -32; h < R; ++h) p && (g ^= p.charCodeAt((h + 32) % p.length)), h === 0 && (C = g), g ^= g << 10, g ^= g >>> 15, g ^= g << 4, g ^= g >>> 13, h >= 0 && (C = C + 1640531527 | 0, f = N[h & 127] ^= g + C, y = f == 0 ? y + 1 : 0);
-                    for (y >= 128 && (N[(p && p.length || 0) & 127] = -1), y = 127, h = 4 * 128; h > 0; --h) g = N[y + 34 & 127], f = N[y = y + 1 & 127], g ^= g << 13, f ^= f << 17, g ^= g >>> 15, f ^= f >>> 12, N[y] = g ^ f;
-                    l.w = C, l.X = N, l.i = y
+                function i(f, g) {
+                    var l, p, y, h, C, N = [],
+                        x = 128;
+                    for (g === (g | 0) ? (p = g, g = null) : (g = g + "\0", p = 0, x = Math.max(x, g.length)), y = 0, h = -32; h < x; ++h) g && (p ^= g.charCodeAt((h + 32) % g.length)), h === 0 && (C = p), p ^= p << 10, p ^= p >>> 15, p ^= p << 4, p ^= p >>> 13, h >= 0 && (C = C + 1640531527 | 0, l = N[h & 127] ^= p + C, y = l == 0 ? y + 1 : 0);
+                    for (y >= 128 && (N[(g && g.length || 0) & 127] = -1), y = 127, h = 4 * 128; h > 0; --h) p = N[y + 34 & 127], l = N[y = y + 1 & 127], p ^= p << 13, l ^= l << 17, p ^= p >>> 15, l ^= l >>> 12, N[y] = p ^ l;
+                    f.w = C, f.X = N, f.i = y
                 }
-                u(i, s)
+                i(u, s)
             }
 
-            function o(s, i) {
-                return i.i = s.i, i.w = s.w, i.X = s.X.slice(), i
+            function o(s, u) {
+                return u.i = s.i, u.w = s.w, u.X = s.X.slice(), u
             }
 
-            function c(s, i) {
+            function c(s, u) {
                 s == null && (s = +new Date);
-                var u = new a(s),
-                    l = i && i.state,
-                    p = function() {
-                        return (u.next() >>> 0) / 4294967296
+                var i = new a(s),
+                    f = u && u.state,
+                    g = function() {
+                        return (i.next() >>> 0) / 4294967296
                     };
-                return p.double = function() {
-                    do var f = u.next() >>> 11,
-                        g = (u.next() >>> 0) / 4294967296,
-                        y = (f + g) / (1 << 21); while (y === 0);
+                return g.double = function() {
+                    do var l = i.next() >>> 11,
+                        p = (i.next() >>> 0) / 4294967296,
+                        y = (l + p) / (1 << 21); while (y === 0);
                     return y
-                }, p.int32 = u.next, p.quick = p, l && (l.X && o(l, u), p.state = function() {
-                    return o(u, {})
-                }), p
+                }, g.int32 = i.next, g.quick = g, f && (f.X && o(f, i), g.state = function() {
+                    return o(i, {})
+                }), g
             }
             r && r.exports ? r.exports = c : n && n.amd ? n(function() {
                 return c
             }) : this.xor4096 = c
-        })(q, e, !1)
-    })(G3);
-    var N1 = {},
-        E3 = {
+        })(e0, e, !1)
+    })(L3);
+    var R1 = {},
+        A3 = {
             get exports() {
-                return N1
+                return R1
             },
             set exports(e) {
-                N1 = e
+                R1 = e
             }
         };
     (function(e) {
         (function(t, r, n) {
             function a(s) {
-                var i = this,
-                    u = "";
-                i.next = function() {
-                    var p = i.b,
-                        f = i.c,
-                        g = i.d,
-                        y = i.a;
-                    return p = p << 25 ^ p >>> 7 ^ f, f = f - g | 0, g = g << 24 ^ g >>> 8 ^ y, y = y - p | 0, i.b = p = p << 20 ^ p >>> 12 ^ f, i.c = f = f - g | 0, i.d = g << 16 ^ f >>> 16 ^ y, i.a = y - p | 0
-                }, i.a = 0, i.b = 0, i.c = -1640531527, i.d = 1367130551, s === Math.floor(s) ? (i.a = s / 4294967296 | 0, i.b = s | 0) : u += s;
-                for (var l = 0; l < u.length + 20; l++) i.b ^= u.charCodeAt(l) | 0, i.next()
-            }
-
-            function o(s, i) {
-                return i.a = s.a, i.b = s.b, i.c = s.c, i.d = s.d, i
-            }
-
-            function c(s, i) {
-                var u = new a(s),
-                    l = i && i.state,
-                    p = function() {
-                        return (u.next() >>> 0) / 4294967296
+                var u = this,
+                    i = "";
+                u.next = function() {
+                    var g = u.b,
+                        l = u.c,
+                        p = u.d,
+                        y = u.a;
+                    return g = g << 25 ^ g >>> 7 ^ l, l = l - p | 0, p = p << 24 ^ p >>> 8 ^ y, y = y - g | 0, u.b = g = g << 20 ^ g >>> 12 ^ l, u.c = l = l - p | 0, u.d = p << 16 ^ l >>> 16 ^ y, u.a = y - g | 0
+                }, u.a = 0, u.b = 0, u.c = -1640531527, u.d = 1367130551, s === Math.floor(s) ? (u.a = s / 4294967296 | 0, u.b = s | 0) : i += s;
+                for (var f = 0; f < i.length + 20; f++) u.b ^= i.charCodeAt(f) | 0, u.next()
+            }
+
+            function o(s, u) {
+                return u.a = s.a, u.b = s.b, u.c = s.c, u.d = s.d, u
+            }
+
+            function c(s, u) {
+                var i = new a(s),
+                    f = u && u.state,
+                    g = function() {
+                        return (i.next() >>> 0) / 4294967296
                     };
-                return p.double = function() {
-                    do var f = u.next() >>> 11,
-                        g = (u.next() >>> 0) / 4294967296,
-                        y = (f + g) / (1 << 21); while (y === 0);
+                return g.double = function() {
+                    do var l = i.next() >>> 11,
+                        p = (i.next() >>> 0) / 4294967296,
+                        y = (l + p) / (1 << 21); while (y === 0);
                     return y
-                }, p.int32 = u.next, p.quick = p, l && (typeof l == "object" && o(l, u), p.state = function() {
-                    return o(u, {})
-                }), p
+                }, g.int32 = i.next, g.quick = g, f && (typeof f == "object" && o(f, i), g.state = function() {
+                    return o(i, {})
+                }), g
             }
             r && r.exports ? r.exports = c : n && n.amd ? n(function() {
                 return c
             }) : this.tychei = c
-        })(q, e, !1)
-    })(E3);
-    var B1 = {},
-        k3 = {
+        })(e0, e, !1)
+    })(A3);
+    var O1 = {},
+        P3 = {
             get exports() {
-                return B1
+                return O1
             },
             set exports(e) {
-                B1 = e
+                O1 = e
             }
         };
-    const A3 = A9(Object.freeze(Object.defineProperty({
+    const _3 = _9(Object.freeze(Object.defineProperty({
         __proto__: null,
         default: {}
     }, Symbol.toStringTag, {
         value: "Module"
     })));
     (function(e) {
         (function(t, r, n) {
             var a = 256,
                 o = 6,
                 c = 52,
                 s = "random",
-                i = n.pow(a, o),
-                u = n.pow(2, c),
-                l = u * 2,
-                p = a - 1,
-                f;
+                u = n.pow(a, o),
+                i = n.pow(2, c),
+                f = i * 2,
+                g = a - 1,
+                l;
 
-            function g(w, S, b) {
+            function p(b, S, w) {
                 var v = [];
                 S = S == !0 ? {
                     entropy: !0
                 } : S || {};
-                var d = N(C(S.entropy ? [w, B(r)] : w ?? R(), 3), v),
+                var d = N(C(S.entropy ? [b, B(r)] : b ?? x(), 3), v),
                     m = new y(v),
-                    x = function() {
-                        for (var D = m.g(o), P = i, U = 0; D < u;) D = (D + U) * a, P *= a, U = m.g(1);
-                        for (; D >= l;) D /= 2, P /= 2, U >>>= 1;
-                        return (D + U) / P
+                    O = function() {
+                        for (var D = m.g(o), _ = u, U = 0; D < i;) D = (D + U) * a, _ *= a, U = m.g(1);
+                        for (; D >= f;) D /= 2, _ /= 2, U >>>= 1;
+                        return (D + U) / _
                     };
-                return x.int32 = function() {
+                return O.int32 = function() {
                     return m.g(4) | 0
-                }, x.quick = function() {
+                }, O.quick = function() {
                     return m.g(4) / 4294967296
-                }, x.double = x, N(B(m.S), r), (S.pass || b || function(D, P, U, H) {
-                    return H && (H.S && h(H, m), D.state = function() {
+                }, O.double = O, N(B(m.S), r), (S.pass || w || function(D, _, U, F) {
+                    return F && (F.S && h(F, m), D.state = function() {
                         return h(m, {})
-                    }), U ? (n[s] = D, P) : D
-                })(x, d, "global" in S ? S.global : this == n, S.state)
+                    }), U ? (n[s] = D, _) : D
+                })(O, d, "global" in S ? S.global : this == n, S.state)
             }
 
-            function y(w) {
-                var S, b = w.length,
+            function y(b) {
+                var S, w = b.length,
                     v = this,
                     d = 0,
                     m = v.i = v.j = 0,
-                    x = v.S = [];
-                for (b || (w = [b++]); d < a;) x[d] = d++;
-                for (d = 0; d < a; d++) x[d] = x[m = p & m + w[d % b] + (S = x[d])], x[m] = S;
+                    O = v.S = [];
+                for (w || (b = [w++]); d < a;) O[d] = d++;
+                for (d = 0; d < a; d++) O[d] = O[m = g & m + b[d % w] + (S = O[d])], O[m] = S;
                 (v.g = function(D) {
-                    for (var P, U = 0, H = v.i, O = v.j, F = v.S; D--;) P = F[H = p & H + 1], U = U * a + F[p & (F[H] = F[O = p & O + P]) + (F[O] = P)];
-                    return v.i = H, v.j = O, U
+                    for (var _, U = 0, F = v.i, T = v.j, L = v.S; D--;) _ = L[F = g & F + 1], U = U * a + L[g & (L[F] = L[T = g & T + _]) + (L[T] = _)];
+                    return v.i = F, v.j = T, U
                 })(a)
             }
 
-            function h(w, S) {
-                return S.i = w.i, S.j = w.j, S.S = w.S.slice(), S
+            function h(b, S) {
+                return S.i = b.i, S.j = b.j, S.S = b.S.slice(), S
             }
 
-            function C(w, S) {
-                var b = [],
-                    v = typeof w,
+            function C(b, S) {
+                var w = [],
+                    v = typeof b,
                     d;
                 if (S && v == "object")
-                    for (d in w) try {
-                        b.push(C(w[d], S - 1))
+                    for (d in b) try {
+                        w.push(C(b[d], S - 1))
                     } catch {}
-                return b.length ? b : v == "string" ? w : w + "\0"
+                return w.length ? w : v == "string" ? b : b + "\0"
             }
 
-            function N(w, S) {
-                for (var b = w + "", v, d = 0; d < b.length;) S[p & d] = p & (v ^= S[p & d] * 19) + b.charCodeAt(d++);
+            function N(b, S) {
+                for (var w = b + "", v, d = 0; d < w.length;) S[g & d] = g & (v ^= S[g & d] * 19) + w.charCodeAt(d++);
                 return B(S)
             }
 
-            function R() {
+            function x() {
                 try {
-                    var w;
-                    return f && (w = f.randomBytes) ? w = w(a) : (w = new Uint8Array(a), (t.crypto || t.msCrypto).getRandomValues(w)), B(w)
+                    var b;
+                    return l && (b = l.randomBytes) ? b = b(a) : (b = new Uint8Array(a), (t.crypto || t.msCrypto).getRandomValues(b)), B(b)
                 } catch {
                     var S = t.navigator,
-                        b = S && S.plugins;
-                    return [+new Date, t, b, t.screen, B(r)]
+                        w = S && S.plugins;
+                    return [+new Date, t, w, t.screen, B(r)]
                 }
             }
 
-            function B(w) {
-                return String.fromCharCode.apply(0, w)
+            function B(b) {
+                return String.fromCharCode.apply(0, b)
             }
             if (N(n.random(), r), e.exports) {
-                e.exports = g;
+                e.exports = p;
                 try {
-                    f = A3
+                    l = _3
                 } catch {}
-            } else n["seed" + s] = g
-        })(typeof self < "u" ? self : q, [], Math)
-    })(k3);
-    var D3 = m1,
-        L3 = C1,
-        P3 = S1,
-        _3 = w1,
-        $3 = b1,
-        j3 = N1,
-        B0 = B1;
-    B0.alea = D3, B0.xor128 = L3, B0.xorwow = P3, B0.xorshift7 = _3, B0.xor4096 = $3, B0.tychei = j3;
-    var U3 = Math.floor;
+            } else n["seed" + s] = p
+        })(typeof self < "u" ? self : e0, [], Math)
+    })(P3);
+    var $3 = w1,
+        j3 = b1,
+        U3 = N1,
+        F3 = B1,
+        V3 = x1,
+        z3 = R1,
+        O0 = O1;
+    O0.alea = $3, O0.xor128 = j3, O0.xorwow = U3, O0.xorshift7 = F3, O0.xor4096 = V3, O0.tychei = z3;
+    var H3 = Math.floor;
 
-    function F3(e) {
+    function I3(e) {
         var t = arguments.length > 1 && arguments[1] !== void 0 ? arguments[1] : 3;
         switch (t) {
             case 1:
                 return Math.abs(e);
             case 2:
                 return Math.sqrt(e[0] * e[0] + e[1] * e[1]);
             case 3:
@@ -3413,176 +3413,176 @@
             default: {
                 for (var r = 0, n = 0; n < t; n++) r += e[n] * e[n];
                 return Math.sqrt(r)
             }
         }
     }
 
-    function I0(e, t) {
-        var r, n, a = r0(e, 3),
+    function Y0(e, t) {
+        var r, n, a = u0(e, 3),
             o = a[0],
             c = a[1],
             s = a[2],
-            i = 1 / 3,
-            u = 1 / 6,
-            l = 2 / 3,
-            p = o,
-            f = o;
-        c > p ? p = c : c < f && (f = c), s > p ? p = s : s < f && (f = s);
-        var g = p;
-        g > 0 ? n = (p - f) / p : n = 0, n > 0 ? (o === p ? r = u * (c - s) / (p - f) : c === p ? r = i + u * (s - o) / (p - f) : r = l + u * (o - c) / (p - f), r < 0 && (r += 1)) : r = 0, t[0] = r, t[1] = n, t[2] = g
+            u = 1 / 3,
+            i = 1 / 6,
+            f = 2 / 3,
+            g = o,
+            l = o;
+        c > g ? g = c : c < l && (l = c), s > g ? g = s : s < l && (l = s);
+        var p = g;
+        p > 0 ? n = (g - l) / g : n = 0, n > 0 ? (o === g ? r = i * (c - s) / (g - l) : c === g ? r = u + i * (s - o) / (g - l) : r = f + i * (o - c) / (g - l), r < 0 && (r += 1)) : r = 0, t[0] = r, t[1] = n, t[2] = p
     }
 
-    function P0(e, t) {
-        var r = r0(e, 3),
+    function $0(e, t) {
+        var r = u0(e, 3),
             n = r[0],
             a = r[1],
             o = r[2],
             c = 1 / 3,
             s = 1 / 6,
-            i = 2 / 3,
-            u = 5 / 6,
-            l, p, f;
-        n > s && n <= c ? (p = 1, l = (c - n) / s, f = 0) : n > c && n <= .5 ? (p = 1, f = (n - c) / s, l = 0) : n > .5 && n <= i ? (f = 1, p = (i - n) / s, l = 0) : n > i && n <= u ? (f = 1, l = (n - i) / s, p = 0) : n > u && n <= 1 ? (l = 1, f = (1 - n) / s, p = 0) : (l = 1, p = n / s, f = 0), l = a * l + (1 - a), p = a * p + (1 - a), f = a * f + (1 - a), l *= o, p *= o, f *= o, t[0] = l, t[1] = p, t[2] = f
+            u = 2 / 3,
+            i = 5 / 6,
+            f, g, l;
+        n > s && n <= c ? (g = 1, f = (c - n) / s, l = 0) : n > c && n <= .5 ? (g = 1, l = (n - c) / s, f = 0) : n > .5 && n <= u ? (l = 1, g = (u - n) / s, f = 0) : n > u && n <= i ? (l = 1, f = (n - u) / s, g = 0) : n > i && n <= 1 ? (f = 1, l = (1 - n) / s, g = 0) : (f = 1, g = n / s, l = 0), f = a * f + (1 - a), g = a * g + (1 - a), l = a * l + (1 - a), f *= o, g *= o, l *= o, t[0] = f, t[1] = g, t[2] = l
     }
 
-    function V3(e, t) {
-        var r = r0(e, 3),
+    function W3(e, t) {
+        var r = u0(e, 3),
             n = r[0],
             a = r[1],
             o = r[2],
             c = (n + 16) / 116,
             s = a / 500 + c,
-            i = c - o / 200;
-        Math.pow(c, 3) > .008856 ? c = Math.pow(c, 3) : c = (c - 16 / 116) / 7.787, Math.pow(s, 3) > .008856 ? s = Math.pow(s, 3) : s = (s - 16 / 116) / 7.787, Math.pow(i, 3) > .008856 ? i = Math.pow(i, 3) : i = (i - 16 / 116) / 7.787;
-        var u = .9505,
-            l = 1,
-            p = 1.089;
-        t[0] = u * s, t[1] = l * c, t[2] = p * i
+            u = c - o / 200;
+        Math.pow(c, 3) > .008856 ? c = Math.pow(c, 3) : c = (c - 16 / 116) / 7.787, Math.pow(s, 3) > .008856 ? s = Math.pow(s, 3) : s = (s - 16 / 116) / 7.787, Math.pow(u, 3) > .008856 ? u = Math.pow(u, 3) : u = (u - 16 / 116) / 7.787;
+        var i = .9505,
+            f = 1,
+            g = 1.089;
+        t[0] = i * s, t[1] = f * c, t[2] = g * u
     }
 
-    function z3(e, t) {
-        var r = r0(e, 3),
+    function Y3(e, t) {
+        var r = u0(e, 3),
             n = r[0],
             a = r[1],
             o = r[2],
             c = .9505,
             s = 1,
-            i = 1.089,
-            u = n / c,
-            l = a / s,
-            p = o / i;
-        u > .008856 ? u = Math.pow(u, 1 / 3) : u = 7.787 * u + 16 / 116, l > .008856 ? l = Math.pow(l, 1 / 3) : l = 7.787 * l + 16 / 116, p > .008856 ? p = Math.pow(p, 1 / 3) : p = 7.787 * p + 16 / 116, t[0] = 116 * l - 16, t[1] = 500 * (u - l), t[2] = 200 * (l - p)
+            u = 1.089,
+            i = n / c,
+            f = a / s,
+            g = o / u;
+        i > .008856 ? i = Math.pow(i, 1 / 3) : i = 7.787 * i + 16 / 116, f > .008856 ? f = Math.pow(f, 1 / 3) : f = 7.787 * f + 16 / 116, g > .008856 ? g = Math.pow(g, 1 / 3) : g = 7.787 * g + 16 / 116, t[0] = 116 * f - 16, t[1] = 500 * (i - f), t[2] = 200 * (f - g)
     }
 
-    function H3(e, t) {
-        var r = r0(e, 3),
+    function X3(e, t) {
+        var r = u0(e, 3),
             n = r[0],
             a = r[1],
             o = r[2],
             c = n * 3.2406 + a * -1.5372 + o * -.4986,
             s = n * -.9689 + a * 1.8758 + o * .0415,
-            i = n * .0557 + a * -.204 + o * 1.057;
-        c > .0031308 ? c = 1.055 * Math.pow(c, 1 / 2.4) - .055 : c *= 12.92, s > .0031308 ? s = 1.055 * Math.pow(s, 1 / 2.4) - .055 : s *= 12.92, i > .0031308 ? i = 1.055 * Math.pow(i, 1 / 2.4) - .055 : i *= 12.92;
-        var u = c;
-        u < s && (u = s), u < i && (u = i), u > 1 && (c /= u, s /= u, i /= u), c < 0 && (c = 0), s < 0 && (s = 0), i < 0 && (i = 0), t[0] = c, t[1] = s, t[2] = i
+            u = n * .0557 + a * -.204 + o * 1.057;
+        c > .0031308 ? c = 1.055 * Math.pow(c, 1 / 2.4) - .055 : c *= 12.92, s > .0031308 ? s = 1.055 * Math.pow(s, 1 / 2.4) - .055 : s *= 12.92, u > .0031308 ? u = 1.055 * Math.pow(u, 1 / 2.4) - .055 : u *= 12.92;
+        var i = c;
+        i < s && (i = s), i < u && (i = u), i > 1 && (c /= i, s /= i, u /= i), c < 0 && (c = 0), s < 0 && (s = 0), u < 0 && (u = 0), t[0] = c, t[1] = s, t[2] = u
     }
 
-    function I3(e, t) {
-        var r = r0(e, 3),
+    function q3(e, t) {
+        var r = u0(e, 3),
             n = r[0],
             a = r[1],
             o = r[2];
         n > .04045 ? n = Math.pow((n + .055) / 1.055, 2.4) : n /= 12.92, a > .04045 ? a = Math.pow((a + .055) / 1.055, 2.4) : a /= 12.92, o > .04045 ? o = Math.pow((o + .055) / 1.055, 2.4) : o /= 12.92, t[0] = n * .4124 + a * .3576 + o * .1805, t[1] = n * .2126 + a * .7152 + o * .0722, t[2] = n * .0193 + a * .1192 + o * .9505
     }
 
-    function R0(e, t) {
+    function T0(e, t) {
         var r = [0, 0, 0];
-        I3(e, r), z3(r, t)
+        q3(e, r), Y3(r, t)
     }
 
-    function R1(e, t) {
+    function T1(e, t) {
         var r = [0, 0, 0];
-        V3(e, r), H3(r, t)
+        W3(e, r), X3(r, t)
     }
-    var W3 = function(t) {
+    var K3 = function(t) {
             return !Number.isFinite(t)
         },
-        Y3 = Number.isNaN,
-        E2 = Y3,
-        X3 = {
+        J3 = Number.isNaN,
+        A2 = J3,
+        Q3 = {
             Int8Array: 1,
             Uint8Array: 1,
             Uint8ClampedArray: 1,
             Int16Array: 2,
             Uint16Array: 2,
             Int32Array: 4,
             Uint32Array: 4,
             Float32Array: 4,
             Float64Array: 8
         },
-        k2 = {
+        P2 = {
             VOID: "",
             CHAR: "Int8Array",
             SIGNED_CHAR: "Int8Array",
             UNSIGNED_CHAR: "Uint8Array",
             SHORT: "Int16Array",
             UNSIGNED_SHORT: "Uint16Array",
             INT: "Int32Array",
             UNSIGNED_INT: "Uint32Array",
             FLOAT: "Float32Array",
             DOUBLE: "Float64Array"
         },
-        q3 = k2.FLOAT,
-        A2 = {
-            DefaultDataType: q3,
-            DataTypeByteSize: X3,
-            VtkDataTypes: k2
+        Z3 = P2.FLOAT,
+        _2 = {
+            DefaultDataType: Z3,
+            DataTypeByteSize: Q3,
+            VtkDataTypes: P2
         };
 
-    function D2(e, t) {
+    function $2(e, t) {
         var r = Object.keys(e);
         if (Object.getOwnPropertySymbols) {
             var n = Object.getOwnPropertySymbols(e);
             t && (n = n.filter(function(a) {
                 return Object.getOwnPropertyDescriptor(e, a).enumerable
             })), r.push.apply(r, n)
         }
         return r
     }
 
-    function W0(e) {
+    function X0(e) {
         for (var t = 1; t < arguments.length; t++) {
             var r = arguments[t] != null ? arguments[t] : {};
-            t % 2 ? D2(Object(r), !0).forEach(function(n) {
-                f0(e, n, r[n])
-            }) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(r)) : D2(Object(r)).forEach(function(n) {
+            t % 2 ? $2(Object(r), !0).forEach(function(n) {
+                v0(e, n, r[n])
+            }) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(r)) : $2(Object(r)).forEach(function(n) {
                 Object.defineProperty(e, n, Object.getOwnPropertyDescriptor(r, n))
             })
         }
         return e
     }
-    var K3 = A2.DefaultDataType,
-        J3 = [];
+    var e8 = _2.DefaultDataType,
+        t8 = [];
 
-    function x1(e, t, r) {
+    function M1(e, t, r) {
         var n = e.length,
             a, o, c, s;
         if (n === 0) return {
             min: Number.MAX_VALUE,
             max: -Number.MAX_VALUE
         };
         for (a = e[t], o = a, s = t; s < n; s += r) c = e[s], c < a ? a = c : c > o && (o = c);
         return {
             min: a,
             max: o
         }
     }
 
-    function Q3() {
+    function r8() {
         var e = Number.MAX_VALUE,
             t = -Number.MAX_VALUE,
             r = 0,
             n = 0;
         return {
             add: function(o) {
                 e > o && (e = o), t < o && (t = o), r++, n += o
@@ -3601,52 +3601,52 @@
                     min: e,
                     max: t
                 }
             }
         }
     }
 
-    function L2(e) {
+    function j2(e) {
         var t = arguments.length > 1 && arguments[1] !== void 0 ? arguments[1] : 0,
             r = arguments.length > 2 && arguments[2] !== void 0 ? arguments[2] : 1;
         if (t < 0 && r > 1) {
             for (var n = e.length, a = n / r, o = new Float64Array(a), c = 0, s = 0; c < a; ++c) {
-                for (var i, u = s + r; s < u; ++s) o[c] += e[s] * e[s];
-                i = c, o[i] = Math.pow(o[i], .5)
+                for (var u, i = s + r; s < i; ++s) o[c] += e[s] * e[s];
+                u = c, o[u] = Math.pow(o[u], .5)
             }
-            return x1(o, 0, 1)
+            return M1(o, 0, 1)
         }
-        return x1(e, t < 0 ? 0 : t, r)
+        return M1(e, t < 0 ? 0 : t, r)
     }
 
-    function P2(e) {
+    function U2(e) {
         for (var t = arguments.length > 1 && arguments[1] !== void 0 ? arguments[1] : 0, r = e || []; r.length <= t;) r.push(null);
         return r
     }
 
-    function O1(e) {
+    function G1(e) {
         return Object.prototype.toString.call(e).slice(8, -1)
     }
 
-    function Z3(e) {
+    function n8(e) {
         for (var t = e.getNumberOfComponents(), r = 0, n = 0; n < e.getNumberOfTuples(); ++n) {
-            var a = F3(e.getTuple(n), t);
+            var a = I3(e.getTuple(n), t);
             a > r && (r = a)
         }
         return r
     }
-    var e8 = {
-        computeRange: L2,
-        createRangeHelper: Q3,
-        fastComputeRange: x1,
-        getDataType: O1,
-        getMaxNorm: Z3
+    var a8 = {
+        computeRange: j2,
+        createRangeHelper: r8,
+        fastComputeRange: M1,
+        getDataType: G1,
+        getMaxNorm: n8
     };
 
-    function t8(e, t) {
+    function o8(e, t) {
         t.classHierarchy.push("vtkDataArray");
 
         function r() {
             t.ranges = null, e.modified()
         }
         e.getElementComponentSize = function() {
             return t.values.BYTES_PER_ELEMENT
@@ -3657,26 +3657,26 @@
             o !== t.values[n * t.numberOfComponents + a] && (t.values[n * t.numberOfComponents + a] = o, r())
         }, e.getData = function() {
             return t.values
         }, e.getRange = function() {
             var n = arguments.length > 0 && arguments[0] !== void 0 ? arguments[0] : -1,
                 a = n < 0 ? t.numberOfComponents : n,
                 o = null;
-            return t.ranges || (t.ranges = P2(t.ranges, t.numberOfComponents)), o = t.ranges[a], o ? (t.rangeTuple[0] = o.min, t.rangeTuple[1] = o.max, t.rangeTuple) : (o = L2(t.values, n, t.numberOfComponents), t.ranges[a] = o, t.rangeTuple[0] = o.min, t.rangeTuple[1] = o.max, t.rangeTuple)
+            return t.ranges || (t.ranges = U2(t.ranges, t.numberOfComponents)), o = t.ranges[a], o ? (t.rangeTuple[0] = o.min, t.rangeTuple[1] = o.max, t.rangeTuple) : (o = j2(t.values, n, t.numberOfComponents), t.ranges[a] = o, t.rangeTuple[0] = o.min, t.rangeTuple[1] = o.max, t.rangeTuple)
         }, e.setRange = function(n, a) {
-            t.ranges || (t.ranges = P2(t.ranges, t.numberOfComponents));
+            t.ranges || (t.ranges = U2(t.ranges, t.numberOfComponents));
             var o = {
                 min: n.min,
                 max: n.max
             };
             return t.ranges[a] = o, t.rangeTuple[0] = o.min, t.rangeTuple[1] = o.max, t.rangeTuple
         }, e.setTuple = function(n, a) {
             for (var o = n * t.numberOfComponents, c = 0; c < t.numberOfComponents; c++) t.values[o + c] = a[c]
         }, e.getTuple = function(n) {
-            var a = arguments.length > 1 && arguments[1] !== void 0 ? arguments[1] : J3,
+            var a = arguments.length > 1 && arguments[1] !== void 0 ? arguments[1] : t8,
                 o = t.numberOfComponents || 1;
             a.length !== o && (a.length = o);
             var c = n * o;
             if (o === 1) a[0] = t.values[c];
             else if (o === 2) a[0] = t.values[c], a[1] = t.values[c + 1];
             else if (o === 3) a[0] = t.values[c], a[1] = t.values[c + 1], a[2] = t.values[c + 2];
             else if (o === 4) a[0] = t.values[c], a[1] = t.values[c + 1], a[2] = t.values[c + 2], a[3] = t.values[c + 3];
@@ -3691,143 +3691,143 @@
         }, e.getNumberOfValues = function() {
             return t.values.length
         }, e.getNumberOfTuples = function() {
             return t.values.length / t.numberOfComponents
         }, e.getDataType = function() {
             return t.dataType
         }, e.newClone = function() {
-            return $2({
+            return V2({
                 empty: !0,
                 name: t.name,
                 dataType: t.dataType,
                 numberOfComponents: t.numberOfComponents
             })
         }, e.getName = function() {
             return t.name || (e.modified(), t.name = "vtkDataArray".concat(e.getMTime())), t.name
         }, e.setData = function(n, a) {
-            t.values = n, t.size = n.length, t.dataType = O1(n), a && (t.numberOfComponents = a), t.size % t.numberOfComponents !== 0 && (t.numberOfComponents = 1), r()
+            t.values = n, t.size = n.length, t.dataType = G1(n), a && (t.numberOfComponents = a), t.size % t.numberOfComponents !== 0 && (t.numberOfComponents = 1), r()
         }, e.getState = function() {
             if (t.deleted) return null;
-            var n = W0(W0({}, t), {}, {
+            var n = X0(X0({}, t), {}, {
                 vtkClass: e.getClassName()
             });
             n.values = Array.from(n.values), delete n.buffer, Object.keys(n).forEach(function(o) {
                 n[o] || delete n[o]
             });
             var a = {};
             return Object.keys(n).sort().forEach(function(o) {
                 a[o] = n[o]
             }), a.mtime && delete a.mtime, a
         }
     }
-    var r8 = {
+    var i8 = {
         name: "",
         numberOfComponents: 1,
         size: 0,
-        dataType: K3,
+        dataType: e8,
         rangeTuple: [0, 0]
     };
 
-    function _2(e, t) {
+    function F2(e, t) {
         var r = arguments.length > 2 && arguments[2] !== void 0 ? arguments[2] : {};
-        if (Object.assign(t, r8, r), !t.empty && !t.values && !t.size) throw new TypeError("Cannot create vtkDataArray object without: size > 0, values");
-        t.values ? Array.isArray(t.values) && (t.values = y2(t.dataType, t.values)) : t.values = v2(t.dataType, t.size), t.values && (t.size = t.values.length, t.dataType = O1(t.values)), C2(e, t), d1(e, t, ["name", "numberOfComponents"]), t8(e, t)
+        if (Object.assign(t, i8, r), !t.empty && !t.values && !t.size) throw new TypeError("Cannot create vtkDataArray object without: size > 0, values");
+        t.values ? Array.isArray(t.values) && (t.values = C2(t.dataType, t.values)) : t.values = m2(t.dataType, t.size), t.values && (t.size = t.values.length, t.dataType = G1(t.values)), N2(e, t), C1(e, t, ["name", "numberOfComponents"]), o8(e, t)
     }
-    var $2 = R2(_2, "vtkDataArray"),
-        Y0 = W0(W0({
-            newInstance: $2,
-            extend: _2
-        }, e8), A2),
-        n8 = {
+    var V2 = M2(F2, "vtkDataArray"),
+        q0 = X0(X0({
+            newInstance: V2,
+            extend: F2
+        }, a8), _2),
+        u8 = {
             MAGNITUDE: 0,
             COMPONENT: 1,
             RGBCOLORS: 2
         },
-        a8 = {
+        s8 = {
             LUMINANCE: 1,
             LUMINANCE_ALPHA: 2,
             RGB: 3,
             RGBA: 4
         },
-        T1 = {
-            VectorMode: n8,
-            ScalarMappingTarget: a8
+        E1 = {
+            VectorMode: u8,
+            ScalarMappingTarget: s8
         },
-        o8 = {
+        c8 = {
             DEFAULT: 0,
             MAP_SCALARS: 1,
             DIRECT_SCALARS: 2
         },
-        i8 = {
+        l8 = {
             DEFAULT: 0,
             USE_POINT_DATA: 1,
             USE_CELL_DATA: 2,
             USE_POINT_FIELD_DATA: 3,
             USE_CELL_FIELD_DATA: 4,
             USE_FIELD_DATA: 5
         },
-        u8 = {
+        f8 = {
             BY_ID: 0,
             BY_NAME: 1
         },
-        s8 = {
-            ColorMode: o8,
-            GetArray: u8,
-            ScalarMode: i8
+        g8 = {
+            ColorMode: c8,
+            GetArray: f8,
+            ScalarMode: l8
         };
 
-    function j2(e, t) {
+    function z2(e, t) {
         var r = Object.keys(e);
         if (Object.getOwnPropertySymbols) {
             var n = Object.getOwnPropertySymbols(e);
             t && (n = n.filter(function(a) {
                 return Object.getOwnPropertyDescriptor(e, a).enumerable
             })), r.push.apply(r, n)
         }
         return r
     }
 
-    function c8(e) {
+    function p8(e) {
         for (var t = 1; t < arguments.length; t++) {
             var r = arguments[t] != null ? arguments[t] : {};
-            t % 2 ? j2(Object(r), !0).forEach(function(n) {
-                f0(e, n, r[n])
-            }) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(r)) : j2(Object(r)).forEach(function(n) {
+            t % 2 ? z2(Object(r), !0).forEach(function(n) {
+                v0(e, n, r[n])
+            }) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(r)) : z2(Object(r)).forEach(function(n) {
                 Object.defineProperty(e, n, Object.getOwnPropertyDescriptor(r, n))
             })
         }
         return e
     }
-    var U2 = T1.ScalarMappingTarget,
-        e0 = T1.VectorMode,
-        x0 = Y0.VtkDataTypes,
-        F2 = s8.ColorMode,
-        V2 = z.vtkErrorMacro;
+    var H2 = E1.ScalarMappingTarget,
+        o0 = E1.VectorMode,
+        M0 = q0.VtkDataTypes,
+        I2 = g8.ColorMode,
+        W2 = W.vtkErrorMacro;
 
-    function f8(e) {
+    function v8(e) {
         return e
     }
 
-    function z2(e) {
+    function Y2(e) {
         return Math.floor(e * 255 + .5)
     }
 
-    function l8(e, t) {
+    function y8(e, t) {
         t.classHierarchy.push("vtkScalarsToColors"), e.setVectorModeToMagnitude = function() {
-            return e.setVectorMode(e0.MAGNITUDE)
+            return e.setVectorMode(o0.MAGNITUDE)
         }, e.setVectorModeToComponent = function() {
-            return e.setVectorMode(e0.COMPONENT)
+            return e.setVectorMode(o0.COMPONENT)
         }, e.setVectorModeToRGBColors = function() {
-            return e.setVectorMode(e0.RGBCOLORS)
+            return e.setVectorMode(o0.RGBCOLORS)
         }, e.build = function() {}, e.isOpaque = function() {
             return !0
         }, e.setAnnotations = function(r, n) {
             if (!(r && !n || !r && n)) {
                 if (r && n && r.length !== n.length) {
-                    V2("Values and annotations do not have the same number of tuples so ignoring");
+                    W2("Values and annotations do not have the same number of tuples so ignoring");
                     return
                 }
                 if (t.annotationArray = [], n && r)
                     for (var a = n.length, o = 0; o < a; o++) t.annotationArray.push({
                         value: r[o],
                         annotation: String(n[o])
                     });
@@ -3871,252 +3871,252 @@
             n[0] = 0, n[1] = 0, n[2] = 0, n[3] = 0
         }, e.updateAnnotatedValueMap = function() {
             t.annotatedValueMap = [];
             for (var r = t.annotationArray.length, n = 0; n < r; n++) t.annotatedValueMap[t.annotationArray[n].value] = n
         }, e.mapScalars = function(r, n, a) {
             var o = r.getNumberOfComponents(),
                 c = null;
-            if (n === F2.DEFAULT && r.getDataType() === x0.UNSIGNED_CHAR || n === F2.DIRECT_SCALARS && r) c = e.convertToRGBA(r, o, r.getNumberOfTuples());
+            if (n === I2.DEFAULT && r.getDataType() === M0.UNSIGNED_CHAR || n === I2.DIRECT_SCALARS && r) c = e.convertToRGBA(r, o, r.getNumberOfTuples());
             else {
                 var s = {
                         type: "vtkDataArray",
                         name: "temp",
                         numberOfComponents: 4,
-                        dataType: x0.UNSIGNED_CHAR
+                        dataType: M0.UNSIGNED_CHAR
                     },
-                    i = z.newTypedArray(s.dataType, 4 * r.getNumberOfTuples());
-                s.values = i, s.size = i.length, c = Y0.newInstance(s);
-                var u = a;
-                u < 0 && o > 1 ? e.mapVectorsThroughTable(r, c, U2.RGBA, -1, -1) : (u < 0 && (u = 0), u >= o && (u = o - 1), e.mapScalarsThroughTable(r, c, U2.RGBA, u))
+                    u = W.newTypedArray(s.dataType, 4 * r.getNumberOfTuples());
+                s.values = u, s.size = u.length, c = q0.newInstance(s);
+                var i = a;
+                i < 0 && o > 1 ? e.mapVectorsThroughTable(r, c, H2.RGBA, -1, -1) : (i < 0 && (i = 0), i >= o && (i = o - 1), e.mapScalarsThroughTable(r, c, H2.RGBA, i))
             }
             return c
         }, e.mapVectorsToMagnitude = function(r, n, a) {
-            for (var o = r.getNumberOfTuples(), c = r.getNumberOfComponents(), s = n.getData(), i = r.getData(), u = 0; u < o; u++) {
-                for (var l = 0, p = 0; p < a; p++) l += i[u * c + p] * i[u * c + p];
-                s[u] = Math.sqrt(l)
+            for (var o = r.getNumberOfTuples(), c = r.getNumberOfComponents(), s = n.getData(), u = r.getData(), i = 0; i < o; i++) {
+                for (var f = 0, g = 0; g < a; g++) f += u[i * c + g] * u[i * c + g];
+                s[i] = Math.sqrt(f)
             }
         }, e.mapVectorsThroughTable = function(r, n, a, o, c) {
             var s = e.getVectorMode(),
-                i = c,
-                u = o,
-                l = r.getNumberOfComponents();
-            s === e0.COMPONENT ? (u === -1 && (u = e.getVectorComponent()), u < 0 && (u = 0), u >= l && (u = l - 1)) : (i === -1 && (i = e.getVectorSize()), i <= 0 ? (u = 0, i = l) : (u < 0 && (u = 0), u >= l && (u = l - 1), u + i > l && (i = l - u)), s === e0.MAGNITUDE && (l === 1 || i === 1) && (s = e0.COMPONENT));
-            var p = 0;
-            switch (u > 0 && (p = u), s) {
-                case e0.COMPONENT: {
-                    e.mapScalarsThroughTable(r, n, a, p);
+                u = c,
+                i = o,
+                f = r.getNumberOfComponents();
+            s === o0.COMPONENT ? (i === -1 && (i = e.getVectorComponent()), i < 0 && (i = 0), i >= f && (i = f - 1)) : (u === -1 && (u = e.getVectorSize()), u <= 0 ? (i = 0, u = f) : (i < 0 && (i = 0), i >= f && (i = f - 1), i + u > f && (u = f - i)), s === o0.MAGNITUDE && (f === 1 || u === 1) && (s = o0.COMPONENT));
+            var g = 0;
+            switch (i > 0 && (g = i), s) {
+                case o0.COMPONENT: {
+                    e.mapScalarsThroughTable(r, n, a, g);
                     break
                 }
-                case e0.RGBCOLORS:
+                case o0.RGBCOLORS:
                     break;
-                case e0.MAGNITUDE:
+                case o0.MAGNITUDE:
                 default: {
-                    var f = Y0.newInstance({
+                    var l = q0.newInstance({
                         numberOfComponents: 1,
                         values: new Float32Array(r.getNumberOfTuples())
                     });
-                    e.mapVectorsToMagnitude(r, f, i), e.mapScalarsThroughTable(f, n, a, 0);
+                    e.mapVectorsToMagnitude(r, l, u), e.mapScalarsThroughTable(l, n, a, 0);
                     break
                 }
             }
         }, e.luminanceToRGBA = function(r, n, a, o) {
-            for (var c = o(a), s = n.getData(), i = r.getData(), u = s.length, l = 0, p = 1, f = 0, g = l; g < u; g += p) {
-                var y = o(s[g]);
-                i[f * 4] = y, i[f * 4 + 1] = y, i[f * 4 + 2] = y, i[f * 4 + 3] = c, f++
+            for (var c = o(a), s = n.getData(), u = r.getData(), i = s.length, f = 0, g = 1, l = 0, p = f; p < i; p += g) {
+                var y = o(s[p]);
+                u[l * 4] = y, u[l * 4 + 1] = y, u[l * 4 + 2] = y, u[l * 4 + 3] = c, l++
             }
         }, e.luminanceAlphaToRGBA = function(r, n, a, o) {
-            for (var c = n.getData(), s = r.getData(), i = c.length, u = 0, l = 2, p = 0, f = u; f < i; f += l) {
-                var g = o(c[f]);
-                s[p] = g, s[p + 1] = g, s[p + 2] = g, s[p + 3] = o(c[f + 1]) * a, p += 4
+            for (var c = n.getData(), s = r.getData(), u = c.length, i = 0, f = 2, g = 0, l = i; l < u; l += f) {
+                var p = o(c[l]);
+                s[g] = p, s[g + 1] = p, s[g + 2] = p, s[g + 3] = o(c[l + 1]) * a, g += 4
             }
         }, e.rGBToRGBA = function(r, n, a, o) {
-            for (var c = z2(a), s = n.getData(), i = r.getData(), u = s.length, l = 0, p = 3, f = 0, g = l; g < u; g += p) i[f * 4] = o(s[g]), i[f * 4 + 1] = o(s[g + 1]), i[f * 4 + 2] = o(s[g + 2]), i[f * 4 + 3] = c, f++
+            for (var c = Y2(a), s = n.getData(), u = r.getData(), i = s.length, f = 0, g = 3, l = 0, p = f; p < i; p += g) u[l * 4] = o(s[p]), u[l * 4 + 1] = o(s[p + 1]), u[l * 4 + 2] = o(s[p + 2]), u[l * 4 + 3] = c, l++
         }, e.rGBAToRGBA = function(r, n, a, o) {
-            for (var c = n.getData(), s = r.getData(), i = c.length, u = 0, l = 4, p = 0, f = u; f < i; f += l) s[p * 4] = o(c[f]), s[p * 4 + 1] = o(c[f + 1]), s[p * 4 + 2] = o(c[f + 2]), s[p * 4 + 3] = o(c[f + 3]) * a, p++
+            for (var c = n.getData(), s = r.getData(), u = c.length, i = 0, f = 4, g = 0, l = i; l < u; l += f) s[g * 4] = o(c[l]), s[g * 4 + 1] = o(c[l + 1]), s[g * 4 + 2] = o(c[l + 2]), s[g * 4 + 3] = o(c[l + 3]) * a, g++
         }, e.convertToRGBA = function(r, n, a) {
             var o = t.alpha;
-            if (n === 4 && o >= 1 && r.getDataType() === x0.UNSIGNED_CHAR) return r;
-            var c = Y0.newInstance({
+            if (n === 4 && o >= 1 && r.getDataType() === M0.UNSIGNED_CHAR) return r;
+            var c = q0.newInstance({
                 numberOfComponents: 4,
                 empty: !0,
                 size: 4 * a,
-                dataType: x0.UNSIGNED_CHAR
+                dataType: M0.UNSIGNED_CHAR
             });
             if (a <= 0) return c;
             o = o > 0 ? o : 0, o = o < 1 ? o : 1;
-            var s = f8;
-            switch ((r.getDataType() === x0.FLOAT || r.getDataType() === x0.DOUBLE) && (s = z2), n) {
+            var s = v8;
+            switch ((r.getDataType() === M0.FLOAT || r.getDataType() === M0.DOUBLE) && (s = Y2), n) {
                 case 1:
                     e.luminanceToRGBA(c, r, o, s);
                     break;
                 case 2:
                     e.luminanceAlphaToRGBA(c, r, s);
                     break;
                 case 3:
                     e.rGBToRGBA(c, r, o, s);
                     break;
                 case 4:
                     e.rGBAToRGBA(c, r, o, s);
                     break;
                 default:
-                    return V2("Cannot convert colors"), null
+                    return W2("Cannot convert colors"), null
             }
             return c
         }, e.usingLogScale = function() {
             return !1
         }, e.getNumberOfAvailableColors = function() {
             return 256 * 256 * 256
         }, e.setRange = function(r, n) {
             return e.setMappingRange(r, n)
         }, e.getRange = function(r, n) {
             return e.getMappingRange()
         }
     }
-    var p8 = {
+    var d8 = {
         alpha: 1,
         vectorComponent: 0,
         vectorSize: -1,
-        vectorMode: e0.COMPONENT,
+        vectorMode: o0.COMPONENT,
         mappingRange: null,
         annotationArray: null,
         annotatedValueMap: null,
         indexedLookup: !1
     };
 
-    function H2(e, t) {
+    function X2(e, t) {
         var r = arguments.length > 2 && arguments[2] !== void 0 ? arguments[2] : {};
-        Object.assign(t, p8, r), z.obj(e, t), t.mappingRange = [0, 255], t.annotationArray = [], t.annotatedValueMap = [], z.setGet(e, t, ["vectorSize", "vectorComponent", "vectorMode", "alpha", "indexedLookup"]), z.setArray(e, t, ["mappingRange"], 2), z.getArray(e, t, ["mappingRange"]), l8(e, t)
+        Object.assign(t, d8, r), W.obj(e, t), t.mappingRange = [0, 255], t.annotationArray = [], t.annotatedValueMap = [], W.setGet(e, t, ["vectorSize", "vectorComponent", "vectorMode", "alpha", "indexedLookup"]), W.setArray(e, t, ["mappingRange"], 2), W.getArray(e, t, ["mappingRange"]), y8(e, t)
     }
-    var g8 = z.newInstance(H2, "vtkScalarsToColors"),
-        I2 = c8({
-            newInstance: g8,
-            extend: H2
-        }, T1),
-        v8 = {
+    var h8 = W.newInstance(X2, "vtkScalarsToColors"),
+        q2 = p8({
+            newInstance: h8,
+            extend: X2
+        }, E1),
+        m8 = {
             RGB: 0,
             HSV: 1,
             LAB: 2,
             DIVERGING: 3
         },
-        y8 = {
+        C8 = {
             LINEAR: 0,
             LOG10: 1
         },
-        M1 = {
-            ColorSpace: v8,
-            Scale: y8
+        k1 = {
+            ColorSpace: m8,
+            Scale: C8
         };
 
-    function W2(e, t) {
+    function K2(e, t) {
         var r = Object.keys(e);
         if (Object.getOwnPropertySymbols) {
             var n = Object.getOwnPropertySymbols(e);
             t && (n = n.filter(function(a) {
                 return Object.getOwnPropertyDescriptor(e, a).enumerable
             })), r.push.apply(r, n)
         }
         return r
     }
 
-    function d8(e) {
+    function S8(e) {
         for (var t = 1; t < arguments.length; t++) {
             var r = arguments[t] != null ? arguments[t] : {};
-            t % 2 ? W2(Object(r), !0).forEach(function(n) {
-                f0(e, n, r[n])
-            }) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(r)) : W2(Object(r)).forEach(function(n) {
+            t % 2 ? K2(Object(r), !0).forEach(function(n) {
+                v0(e, n, r[n])
+            }) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(r)) : K2(Object(r)).forEach(function(n) {
                 Object.defineProperty(e, n, Object.getOwnPropertyDescriptor(r, n))
             })
         }
         return e
     }
-    var Z = M1.ColorSpace,
-        Y2 = M1.Scale,
-        X0 = I2.ScalarMappingTarget,
-        h8 = z.vtkDebugMacro,
-        n0 = z.vtkErrorMacro,
-        m8 = z.vtkWarningMacro;
+    var n0 = k1.ColorSpace,
+        J2 = k1.Scale,
+        K0 = q2.ScalarMappingTarget,
+        w8 = W.vtkDebugMacro,
+        s0 = W.vtkErrorMacro,
+        b8 = W.vtkWarningMacro;
 
-    function X2(e, t) {
+    function Q2(e, t) {
         var r = e[0],
             n = e[1],
             a = e[2],
             o = Math.sqrt(r * r + n * n + a * a),
             c = o > .001 ? Math.acos(r / o) : 0,
             s = c > .001 ? Math.atan2(a, n) : 0;
         t[0] = o, t[1] = c, t[2] = s
     }
 
-    function C8(e, t) {
+    function N8(e, t) {
         var r = e[0],
             n = e[1],
             a = e[2];
         t[0] = r * Math.cos(n), t[1] = r * Math.sin(n) * Math.cos(a), t[2] = r * Math.sin(n) * Math.sin(a)
     }
 
-    function q2(e, t) {
+    function Z2(e, t) {
         if (e[0] >= t - .1) return e[2];
         var r = e[1] * Math.sqrt(t * t - e[0] * e[0]) / (e[0] * Math.sin(e[1]));
         return e[2] > -.3 * Math.PI ? e[2] + r : e[2] - r
     }
 
-    function S8(e, t) {
+    function B8(e, t) {
         var r = e - t;
         for (r < 0 && (r = -r); r >= 2 * Math.PI;) r -= 2 * Math.PI;
         return r > Math.PI && (r = 2 * Math.PI - r), r
     }
 
-    function K2(e, t, r, n) {
+    function e9(e, t, r, n) {
         var a = [],
             o = [];
-        R0(t, a), R0(r, o);
+        T0(t, a), T0(r, o);
         var c = [],
             s = [];
-        X2(a, c), X2(o, s);
-        var i = e;
-        if (c[1] > .05 && s[1] > .05 && S8(c[2], s[2]) > .33 * Math.PI) {
-            var u = Math.max(c[0], s[0]);
-            u = Math.max(88, u), e < .5 ? (s[0] = u, s[1] = 0, s[2] = 0, i *= 2) : (c[0] = u, c[1] = 0, c[2] = 0, i = 2 * i - 1)
-        }
-        c[1] < .05 && s[1] > .05 ? c[2] = q2(s, c[0]) : s[1] < .05 && c[1] > .05 && (s[2] = q2(c, s[0]));
-        var l = [];
-        l[0] = (1 - i) * c[0] + i * s[0], l[1] = (1 - i) * c[1] + i * s[1], l[2] = (1 - i) * c[2] + i * s[2];
-        var p = [];
-        C8(l, p), R1(p, n)
+        Q2(a, c), Q2(o, s);
+        var u = e;
+        if (c[1] > .05 && s[1] > .05 && B8(c[2], s[2]) > .33 * Math.PI) {
+            var i = Math.max(c[0], s[0]);
+            i = Math.max(88, i), e < .5 ? (s[0] = i, s[1] = 0, s[2] = 0, u *= 2) : (c[0] = i, c[1] = 0, c[2] = 0, u = 2 * u - 1)
+        }
+        c[1] < .05 && s[1] > .05 ? c[2] = Z2(s, c[0]) : s[1] < .05 && c[1] > .05 && (s[2] = Z2(c, s[0]));
+        var f = [];
+        f[0] = (1 - u) * c[0] + u * s[0], f[1] = (1 - u) * c[1] + u * s[1], f[2] = (1 - u) * c[2] + u * s[2];
+        var g = [];
+        N8(f, g), T1(g, n)
     }
 
-    function w8(e, t) {
+    function x8(e, t) {
         t.classHierarchy.push("vtkColorTransferFunction"), e.getSize = function() {
             return t.nodes.length
         }, e.addRGBPoint = function(r, n, a, o) {
             return e.addRGBPointLong(r, n, a, o, .5, 0)
         }, e.addRGBPointLong = function(r, n, a, o) {
             var c = arguments.length > 4 && arguments[4] !== void 0 ? arguments[4] : .5,
                 s = arguments.length > 5 && arguments[5] !== void 0 ? arguments[5] : 0;
-            if (c < 0 || c > 1) return n0("Midpoint outside range [0.0, 1.0]"), -1;
-            if (s < 0 || s > 1) return n0("Sharpness outside range [0.0, 1.0]"), -1;
+            if (c < 0 || c > 1) return s0("Midpoint outside range [0.0, 1.0]"), -1;
+            if (s < 0 || s > 1) return s0("Sharpness outside range [0.0, 1.0]"), -1;
             t.allowDuplicateScalars || e.removePoint(r);
-            var i = {
+            var u = {
                 x: r,
                 r: n,
                 g: a,
                 b: o,
                 midpoint: c,
                 sharpness: s
             };
-            t.nodes.push(i), e.sortAndUpdateRange();
-            for (var u = 0; u < t.nodes.length && t.nodes[u].x !== r; u++);
-            return u < t.nodes.length ? u : -1
+            t.nodes.push(u), e.sortAndUpdateRange();
+            for (var i = 0; i < t.nodes.length && t.nodes[i].x !== r; i++);
+            return i < t.nodes.length ? i : -1
         }, e.addHSVPoint = function(r, n, a, o) {
             return e.addHSVPointLong(r, n, a, o, .5, 0)
         }, e.addHSVPointLong = function(r, n, a, o) {
             var c = arguments.length > 4 && arguments[4] !== void 0 ? arguments[4] : .5,
                 s = arguments.length > 5 && arguments[5] !== void 0 ? arguments[5] : 0,
-                i = [],
-                u = [n, a, o];
-            return P0(u, i), e.addRGBPoint(r, i[0], i[1], i[2], c, s)
+                u = [],
+                i = [n, a, o];
+            return $0(i, u), e.addRGBPoint(r, u[0], u[1], u[2], c, s)
         }, e.setNodes = function(r) {
             if (t.nodes !== r) {
                 var n = JSON.stringify(t.nodes);
                 t.nodes = r;
                 var a = JSON.stringify(t.nodes);
                 if (e.sortAndUpdateRange() || n !== a) return e.modified(), !0
             }
@@ -4147,24 +4147,24 @@
                     if (t.nodes[a].x === r) {
                         t.nodes[a].x = n, e.sortAndUpdateRange();
                         break
                     }
             }
         }, e.removeAllPoints = function() {
             t.nodes = [], e.sortAndUpdateRange()
-        }, e.addRGBSegment = function(r, n, a, o, c, s, i, u) {
+        }, e.addRGBSegment = function(r, n, a, o, c, s, u, i) {
             e.sortAndUpdateRange();
-            for (var l = 0; l < t.nodes.length;) t.nodes[l].x >= r && t.nodes[l].x <= c ? t.nodes.splice(l, 1) : l++;
-            e.addRGBPointLong(r, n, a, o, .5, 0), e.addRGBPointLong(c, s, i, u, .5, 0), e.modified()
-        }, e.addHSVSegment = function(r, n, a, o, c, s, i, u) {
-            var l = [n, a, o],
-                p = [s, i, u],
-                f = [],
-                g = [];
-            P0(l, f), P0(p, g), e.addRGBSegment(r, f[0], f[1], f[2], c, g[0], g[1], g[2])
+            for (var f = 0; f < t.nodes.length;) t.nodes[f].x >= r && t.nodes[f].x <= c ? t.nodes.splice(f, 1) : f++;
+            e.addRGBPointLong(r, n, a, o, .5, 0), e.addRGBPointLong(c, s, u, i, .5, 0), e.modified()
+        }, e.addHSVSegment = function(r, n, a, o, c, s, u, i) {
+            var f = [n, a, o],
+                g = [s, u, i],
+                l = [],
+                p = [];
+            $0(f, l), $0(g, p), e.addRGBSegment(r, l[0], l[1], l[2], c, p[0], p[1], p[2])
         }, e.mapValue = function(r) {
             var n = [];
             return e.getColor(r, n), [Math.floor(255 * n[0] + .5), Math.floor(255 * n[1] + .5), Math.floor(255 * n[2] + .5), 255]
         }, e.getColor = function(r, n) {
             if (t.indexedLookup) {
                 var a = e.getSize(),
                     o = e.getAnnotatedValueIndexInternal(r);
@@ -4182,139 +4182,139 @@
         }, e.getGreenValue = function(r) {
             var n = [];
             return e.getColor(r, n), n[1]
         }, e.getBlueValue = function(r) {
             var n = [];
             return e.getColor(r, n), n[2]
         }, e.getTable = function(r, n, a, o) {
-            if (E2(r) || E2(n)) {
+            if (A2(r) || A2(n)) {
                 for (var c = 0; c < a; c++) o[c * 3 + 0] = t.nanColor[0], o[c * 3 + 1] = t.nanColor[1], o[c * 3 + 2] = t.nanColor[2];
                 return
             }
             var s = 0,
-                i = t.nodes.length,
-                u = 0,
-                l = 0,
-                p = 0;
-            i !== 0 && (u = t.nodes[i - 1].r, l = t.nodes[i - 1].g, p = t.nodes[i - 1].b);
-            var f = 0,
-                g = 0,
+                u = t.nodes.length,
+                i = 0,
+                f = 0,
+                g = 0;
+            u !== 0 && (i = t.nodes[u - 1].r, f = t.nodes[u - 1].g, g = t.nodes[u - 1].b);
+            var l = 0,
+                p = 0,
                 y = 0,
                 h = [0, 0, 0],
                 C = [0, 0, 0],
                 N = 0,
-                R = 0,
+                x = 0,
                 B = [],
-                w = t.scale === Y2.LOG10;
-            w && (w = t.mappingRange[0] > 0);
+                b = t.scale === J2.LOG10;
+            b && (b = t.mappingRange[0] > 0);
             var S = 0,
-                b = 0,
+                w = 0,
                 v = 0;
-            w && (S = Math.log10(r), b = Math.log10(n));
+            b && (S = Math.log10(r), w = Math.log10(n));
             for (var d = 0; d < a; d++) {
                 var m = 3 * d;
-                if (a > 1 ? w ? (v = S + d / (a - 1) * (b - S), f = Math.pow(10, v)) : f = r + d / (a - 1) * (n - r) : w ? (v = .5 * (S + b), f = Math.pow(10, v)) : f = .5 * (r + n), t.discretize) {
-                    var x = t.mappingRange;
-                    if (f >= x[0] && f <= x[1]) {
+                if (a > 1 ? b ? (v = S + d / (a - 1) * (w - S), l = Math.pow(10, v)) : l = r + d / (a - 1) * (n - r) : b ? (v = .5 * (S + w), l = Math.pow(10, v)) : l = .5 * (r + n), t.discretize) {
+                    var O = t.mappingRange;
+                    if (l >= O[0] && l <= O[1]) {
                         var D = t.numberOfValues,
-                            P = x[1] - x[0];
-                        if (D <= 1) f = x[0] + P / 2;
+                            _ = O[1] - O[0];
+                        if (D <= 1) l = O[0] + _ / 2;
                         else {
-                            var U = (f - x[0]) / P,
-                                H = U3(D * U);
-                            f = x[0] + H / (D - 1) * P
+                            var U = (l - O[0]) / _,
+                                F = H3(D * U);
+                            l = O[0] + F / (D - 1) * _
                         }
                     }
                 }
-                for (; s < i && f > t.nodes[s].x;) s++, s < i && (g = t.nodes[s - 1].x, y = t.nodes[s].x, w && (g = Math.log10(g), y = Math.log10(y)), h[0] = t.nodes[s - 1].r, C[0] = t.nodes[s].r, h[1] = t.nodes[s - 1].g, C[1] = t.nodes[s].g, h[2] = t.nodes[s - 1].b, C[2] = t.nodes[s].b, N = t.nodes[s - 1].midpoint, R = t.nodes[s - 1].sharpness, N < 1e-5 && (N = 1e-5), N > .99999 && (N = .99999));
-                if (f > t.mappingRange[1]) o[m] = 0, o[m + 1] = 0, o[m + 2] = 0, t.clamping && (e.getUseAboveRangeColor() ? (o[m] = t.aboveRangeColor[0], o[m + 1] = t.aboveRangeColor[1], o[m + 2] = t.aboveRangeColor[2]) : (o[m] = u, o[m + 1] = l, o[m + 2] = p));
-                else if (f < t.mappingRange[0] || W3(f) && f < 0) o[m] = 0, o[m + 1] = 0, o[m + 2] = 0, t.clamping && (e.getUseBelowRangeColor() ? (o[m] = t.belowRangeColor[0], o[m + 1] = t.belowRangeColor[1], o[m + 2] = t.belowRangeColor[2]) : i > 0 && (o[m] = t.nodes[0].r, o[m + 1] = t.nodes[0].g, o[m + 2] = t.nodes[0].b));
-                else if (s === 0 && (Math.abs(f - r) < 1e-6 || t.discretize)) i > 0 ? (o[m] = t.nodes[0].r, o[m + 1] = t.nodes[0].g, o[m + 2] = t.nodes[0].b) : (o[m] = 0, o[m + 1] = 0, o[m + 2] = 0);
+                for (; s < u && l > t.nodes[s].x;) s++, s < u && (p = t.nodes[s - 1].x, y = t.nodes[s].x, b && (p = Math.log10(p), y = Math.log10(y)), h[0] = t.nodes[s - 1].r, C[0] = t.nodes[s].r, h[1] = t.nodes[s - 1].g, C[1] = t.nodes[s].g, h[2] = t.nodes[s - 1].b, C[2] = t.nodes[s].b, N = t.nodes[s - 1].midpoint, x = t.nodes[s - 1].sharpness, N < 1e-5 && (N = 1e-5), N > .99999 && (N = .99999));
+                if (l > t.mappingRange[1]) o[m] = 0, o[m + 1] = 0, o[m + 2] = 0, t.clamping && (e.getUseAboveRangeColor() ? (o[m] = t.aboveRangeColor[0], o[m + 1] = t.aboveRangeColor[1], o[m + 2] = t.aboveRangeColor[2]) : (o[m] = i, o[m + 1] = f, o[m + 2] = g));
+                else if (l < t.mappingRange[0] || K3(l) && l < 0) o[m] = 0, o[m + 1] = 0, o[m + 2] = 0, t.clamping && (e.getUseBelowRangeColor() ? (o[m] = t.belowRangeColor[0], o[m + 1] = t.belowRangeColor[1], o[m + 2] = t.belowRangeColor[2]) : u > 0 && (o[m] = t.nodes[0].r, o[m + 1] = t.nodes[0].g, o[m + 2] = t.nodes[0].b));
+                else if (s === 0 && (Math.abs(l - r) < 1e-6 || t.discretize)) u > 0 ? (o[m] = t.nodes[0].r, o[m + 1] = t.nodes[0].g, o[m + 2] = t.nodes[0].b) : (o[m] = 0, o[m + 1] = 0, o[m + 2] = 0);
                 else {
-                    var O = 0;
-                    if (w ? O = (v - g) / (y - g) : O = (f - g) / (y - g), O < N ? O = .5 * O / N : O = .5 + .5 * (O - N) / (1 - N), R > .99)
-                        if (O < .5) {
+                    var T = 0;
+                    if (b ? T = (v - p) / (y - p) : T = (l - p) / (y - p), T < N ? T = .5 * T / N : T = .5 + .5 * (T - N) / (1 - N), x > .99)
+                        if (T < .5) {
                             o[m] = h[0], o[m + 1] = h[1], o[m + 2] = h[2];
                             continue
                         } else {
                             o[m] = C[0], o[m + 1] = C[1], o[m + 2] = C[2];
                             continue
-                        } if (R < .01) {
-                        if (t.colorSpace === Z.RGB) o[m] = (1 - O) * h[0] + O * C[0], o[m + 1] = (1 - O) * h[1] + O * C[1], o[m + 2] = (1 - O) * h[2] + O * C[2];
-                        else if (t.colorSpace === Z.HSV) {
-                            var F = [],
-                                J = [];
-                            I0(h, F), I0(C, J), t.hSVWrap && (F[0] - J[0] > .5 || J[0] - F[0] > .5) && (F[0] > J[0] ? F[0] -= 1 : J[0] -= 1);
-                            var u0 = [];
-                            u0[0] = (1 - O) * F[0] + O * J[0], u0[0] < 0 && (u0[0] += 1), u0[1] = (1 - O) * F[1] + O * J[1], u0[2] = (1 - O) * F[2] + O * J[2], P0(u0, B), o[m] = B[0], o[m + 1] = B[1], o[m + 2] = B[2]
-                        } else if (t.colorSpace === Z.LAB) {
-                            var M0 = [],
-                                h0 = [];
-                            R0(h, M0), R0(C, h0);
-                            var T = [];
-                            T[0] = (1 - O) * M0[0] + O * h0[0], T[1] = (1 - O) * M0[1] + O * h0[1], T[2] = (1 - O) * M0[2] + O * h0[2], R1(T, B), o[m] = B[0], o[m + 1] = B[1], o[m + 2] = B[2]
-                        } else t.colorSpace === Z.DIVERGING ? (K2(O, h, C, B), o[m] = B[0], o[m + 1] = B[1], o[m + 2] = B[2]) : n0("ColorSpace set to invalid value.", t.colorSpace);
+                        } if (x < .01) {
+                        if (t.colorSpace === n0.RGB) o[m] = (1 - T) * h[0] + T * C[0], o[m + 1] = (1 - T) * h[1] + T * C[1], o[m + 2] = (1 - T) * h[2] + T * C[2];
+                        else if (t.colorSpace === n0.HSV) {
+                            var L = [],
+                                V = [];
+                            Y0(h, L), Y0(C, V), t.hSVWrap && (L[0] - V[0] > .5 || V[0] - L[0] > .5) && (L[0] > V[0] ? L[0] -= 1 : V[0] -= 1);
+                            var Q = [];
+                            Q[0] = (1 - T) * L[0] + T * V[0], Q[0] < 0 && (Q[0] += 1), Q[1] = (1 - T) * L[1] + T * V[1], Q[2] = (1 - T) * L[2] + T * V[2], $0(Q, B), o[m] = B[0], o[m + 1] = B[1], o[m + 2] = B[2]
+                        } else if (t.colorSpace === n0.LAB) {
+                            var K = [],
+                                a0 = [];
+                            T0(h, K), T0(C, a0);
+                            var M = [];
+                            M[0] = (1 - T) * K[0] + T * a0[0], M[1] = (1 - T) * K[1] + T * a0[1], M[2] = (1 - T) * K[2] + T * a0[2], T1(M, B), o[m] = B[0], o[m + 1] = B[1], o[m + 2] = B[2]
+                        } else t.colorSpace === n0.DIVERGING ? (e9(T, h, C, B), o[m] = B[0], o[m + 1] = B[1], o[m + 2] = B[2]) : s0("ColorSpace set to invalid value.", t.colorSpace);
                         continue
                     }
-                    O < .5 ? O = .5 * Math.pow(O * 2, 1 + 10 * R) : O > .5 && (O = 1 - .5 * Math.pow((1 - O) * 2, 1 + 10 * R));
-                    var G = O * O,
-                        k = G * O,
-                        E = 2 * k - 3 * G + 1,
-                        L = -2 * k + 3 * G,
-                        X = k - 2 * G + O,
-                        A = k - G,
-                        _ = void 0,
-                        I = void 0;
-                    if (t.colorSpace === Z.RGB)
-                        for (var W = 0; W < 3; W++) _ = C[W] - h[W], I = (1 - R) * _, o[m + W] = E * h[W] + L * C[W] + X * I + A * I;
-                    else if (t.colorSpace === Z.HSV) {
-                        var o0 = [],
-                            i0 = [];
-                        I0(h, o0), I0(C, i0), t.hSVWrap && (o0[0] - i0[0] > .5 || i0[0] - o0[0] > .5) && (o0[0] > i0[0] ? o0[0] -= 1 : i0[0] -= 1);
-                        for (var J0 = [], t0 = 0; t0 < 3; t0++) _ = i0[t0] - o0[t0], I = (1 - R) * _, J0[t0] = E * o0[t0] + L * i0[t0] + X * I + A * I, t0 === 0 && J0[t0] < 0 && (J0[t0] += 1);
-                        P0(J0, B), o[m] = B[0], o[m + 1] = B[1], o[m + 2] = B[2]
-                    } else if (t.colorSpace === Z.LAB) {
-                        var k1 = [],
-                            A1 = [];
-                        R0(h, k1), R0(C, A1);
-                        for (var n9 = [], m0 = 0; m0 < 3; m0++) _ = A1[m0] - k1[m0], I = (1 - R) * _, n9[m0] = E * k1[m0] + L * A1[m0] + X * I + A * I;
-                        R1(n9, B), o[m] = B[0], o[m + 1] = B[1], o[m + 2] = B[2]
-                    } else t.colorSpace === Z.DIVERGING ? (K2(O, h, C, B), o[m] = B[0], o[m + 1] = B[1], o[m + 2] = B[2]) : n0("ColorSpace set to invalid value.");
-                    for (var s0 = 0; s0 < 3; s0++) o[m + s0] = o[m + s0] < 0 ? 0 : o[m + s0], o[m + s0] = o[m + s0] > 1 ? 1 : o[m + s0]
+                    T < .5 ? T = .5 * Math.pow(T * 2, 1 + 10 * x) : T > .5 && (T = 1 - .5 * Math.pow((1 - T) * 2, 1 + 10 * x));
+                    var E = T * T,
+                        A = E * T,
+                        k = 2 * A - 3 * E + 1,
+                        $ = -2 * A + 3 * E,
+                        Z = A - 2 * E + T,
+                        P = A - E,
+                        j = void 0,
+                        Y = void 0;
+                    if (t.colorSpace === n0.RGB)
+                        for (var X = 0; X < 3; X++) j = C[X] - h[X], Y = (1 - x) * j, o[m + X] = k * h[X] + $ * C[X] + Z * Y + P * Y;
+                    else if (t.colorSpace === n0.HSV) {
+                        var l0 = [],
+                            f0 = [];
+                        Y0(h, l0), Y0(C, f0), t.hSVWrap && (l0[0] - f0[0] > .5 || f0[0] - l0[0] > .5) && (l0[0] > f0[0] ? l0[0] -= 1 : f0[0] -= 1);
+                        for (var e1 = [], i0 = 0; i0 < 3; i0++) j = f0[i0] - l0[i0], Y = (1 - x) * j, e1[i0] = k * l0[i0] + $ * f0[i0] + Z * Y + P * Y, i0 === 0 && e1[i0] < 0 && (e1[i0] += 1);
+                        $0(e1, B), o[m] = B[0], o[m + 1] = B[1], o[m + 2] = B[2]
+                    } else if (t.colorSpace === n0.LAB) {
+                        var P1 = [],
+                            _1 = [];
+                        T0(h, P1), T0(C, _1);
+                        for (var u9 = [], w0 = 0; w0 < 3; w0++) j = _1[w0] - P1[w0], Y = (1 - x) * j, u9[w0] = k * P1[w0] + $ * _1[w0] + Z * Y + P * Y;
+                        T1(u9, B), o[m] = B[0], o[m + 1] = B[1], o[m + 2] = B[2]
+                    } else t.colorSpace === n0.DIVERGING ? (e9(T, h, C, B), o[m] = B[0], o[m + 1] = B[1], o[m + 2] = B[2]) : s0("ColorSpace set to invalid value.");
+                    for (var g0 = 0; g0 < 3; g0++) o[m + g0] = o[m + g0] < 0 ? 0 : o[m + g0], o[m + g0] = o[m + g0] > 1 ? 1 : o[m + g0]
                 }
             }
         }, e.getUint8Table = function(r, n, a) {
             var o = arguments.length > 3 && arguments[3] !== void 0 ? arguments[3] : !1;
             if (e.getMTime() <= t.buildTime && t.tableSize === a && t.tableWithAlpha !== o) return t.table;
-            if (t.nodes.length === 0) return n0("Attempting to lookup a value with no points in the function"), t.table;
+            if (t.nodes.length === 0) return s0("Attempting to lookup a value with no points in the function"), t.table;
             var c = o ? 4 : 3;
             (t.tableSize !== a || t.tableWithAlpha !== o) && (t.table = new Uint8Array(a * c), t.tableSize = a, t.tableWithAlpha = o);
             var s = [];
             e.getTable(r, n, a, s);
-            for (var i = 0; i < a; i++) t.table[i * c + 0] = Math.floor(s[i * 3 + 0] * 255 + .5), t.table[i * c + 1] = Math.floor(s[i * 3 + 1] * 255 + .5), t.table[i * c + 2] = Math.floor(s[i * 3 + 2] * 255 + .5), o && (t.table[i * c + 3] = 255);
+            for (var u = 0; u < a; u++) t.table[u * c + 0] = Math.floor(s[u * 3 + 0] * 255 + .5), t.table[u * c + 1] = Math.floor(s[u * 3 + 1] * 255 + .5), t.table[u * c + 2] = Math.floor(s[u * 3 + 2] * 255 + .5), o && (t.table[u * c + 3] = 255);
             return t.buildTime.modified(), t.table
         }, e.buildFunctionFromTable = function(r, n, a, o) {
             var c = 0;
             e.removeAllPoints(), a > 1 && (c = (n - r) / (a - 1));
             for (var s = 0; s < a; s++) {
-                var i = {
+                var u = {
                     x: r + c * s,
                     r: o[s * 3],
                     g: o[s * 3 + 1],
                     b: o[s * 3 + 2],
                     sharpness: 0,
                     midpoint: .5
                 };
-                t.nodes.push(i)
+                t.nodes.push(u)
             }
             e.sortAndUpdateRange()
         }, e.getNodeValue = function(r, n) {
-            return r < 0 || r >= t.nodes.length ? (n0("Index out of range!"), -1) : (n[0] = t.nodes[r].x, n[1] = t.nodes[r].r, n[2] = t.nodes[r].g, n[3] = t.nodes[r].b, n[4] = t.nodes[r].midpoint, n[5] = t.nodes[r].sharpness, 1)
+            return r < 0 || r >= t.nodes.length ? (s0("Index out of range!"), -1) : (n[0] = t.nodes[r].x, n[1] = t.nodes[r].r, n[2] = t.nodes[r].g, n[3] = t.nodes[r].b, n[4] = t.nodes[r].midpoint, n[5] = t.nodes[r].sharpness, 1)
         }, e.setNodeValue = function(r, n) {
-            if (r < 0 || r >= t.nodes.length) return n0("Index out of range!"), -1;
+            if (r < 0 || r >= t.nodes.length) return s0("Index out of range!"), -1;
             var a = t.nodes[r].x;
             return t.nodes[r].x = n[0], t.nodes[r].r = n[1], t.nodes[r].g = n[2], t.nodes[r].b = n[3], t.nodes[r].midpoint = n[4], t.nodes[r].sharpness = n[5], a !== n[0] ? e.sortAndUpdateRange() : e.modified(), 1
         }, e.getNumberOfAvailableColors = function() {
             return t.indexedLookup && e.getSize() ? e.getSize() : t.tableSize ? t.tableSize : 16777216
         }, e.getIndexedColor = function(r, n) {
             var a = e.getSize();
             if (a > 0 && r >= 0) {
@@ -4331,18 +4331,18 @@
                 for (var a = 0; a < r; a++) e.addRGBPoint(n[a * 4], n[a * 4 + 1], n[a * 4 + 2], n[a * 4 + 3])
             }
         }, e.setMappingRange = function(r, n) {
             var a = [r, n],
                 o = e.getRange();
             if (!(o[1] === a[1] && o[0] === a[0])) {
                 if (a[1] === a[0]) {
-                    n0("attempt to set zero width color range");
+                    s0("attempt to set zero width color range");
                     return
                 }
-                for (var c = (a[1] - a[0]) / (o[1] - o[0]), s = a[0] - o[0] * c, i = 0; i < t.nodes.length; ++i) t.nodes[i].x = t.nodes[i].x * c + s;
+                for (var c = (a[1] - a[0]) / (o[1] - o[0]), s = a[0] - o[0] * c, u = 0; u < t.nodes.length; ++u) t.nodes[u].x = t.nodes[u].x * c + s;
                 t.mappingRange[0] = a[0], t.mappingRange[1] = a[1], e.modified()
             }
         }, e.adjustRange = function(r) {
             var n = e.getRange(),
                 a = [];
             n[0] < r[0] ? (e.getColor(r[0], a), e.addRGBPoint(r[0], a[0], a[1], a[2])) : (e.getColor(n[0], a), e.addRGBPoint(r[0], a[0], a[1], a[2])), n[1] > r[1] ? (e.getColor(r[1], a), e.addRGBPoint(r[1], a[0], a[1], a[2])) : (e.getColor(n[1], a), e.addRGBPoint(r[1], a[0], a[1], a[2])), e.sortAndUpdateRange();
             for (var o = 0; o < t.nodes.length;) t.nodes[o].x >= r[0] && t.nodes[o].x <= r[1] ? t.nodes.splice(o, 1) : ++o;
@@ -4355,51 +4355,51 @@
             for (var r = Number.MAX_VALUE, n = 0; n < t.nodes.length - 1; n++) {
                 var a = t.nodes[n + 1].x - t.nodes[n].x;
                 a < r && (r = a)
             }
             return r
         }, e.mapScalarsThroughTable = function(r, n, a, o) {
             if (e.getSize() === 0) {
-                h8("Transfer Function Has No Points!");
+                w8("Transfer Function Has No Points!");
                 return
             }
             t.indexedLookup ? e.mapDataIndexed(r, n, a, o) : e.mapData(r, n, a, o)
         }, e.mapData = function(r, n, a, o) {
             if (e.getSize() === 0) {
-                m8("Transfer Function Has No Points!");
+                b8("Transfer Function Has No Points!");
                 return
             }
             var c = Math.floor(e.getAlpha() * 255 + .5),
                 s = r.getNumberOfTuples(),
-                i = r.getNumberOfComponents(),
-                u = n.getData(),
-                l = r.getData(),
-                p = [];
-            if (a === X0.RGBA)
-                for (var f = 0; f < s; f++) {
-                    var g = l[f * i + o];
-                    e.getColor(g, p), u[f * 4] = Math.floor(p[0] * 255 + .5), u[f * 4 + 1] = Math.floor(p[1] * 255 + .5), u[f * 4 + 2] = Math.floor(p[2] * 255 + .5), u[f * 4 + 3] = c
+                u = r.getNumberOfComponents(),
+                i = n.getData(),
+                f = r.getData(),
+                g = [];
+            if (a === K0.RGBA)
+                for (var l = 0; l < s; l++) {
+                    var p = f[l * u + o];
+                    e.getColor(p, g), i[l * 4] = Math.floor(g[0] * 255 + .5), i[l * 4 + 1] = Math.floor(g[1] * 255 + .5), i[l * 4 + 2] = Math.floor(g[2] * 255 + .5), i[l * 4 + 3] = c
                 }
-            if (a === X0.RGB)
+            if (a === K0.RGB)
                 for (var y = 0; y < s; y++) {
-                    var h = l[y * i + o];
-                    e.getColor(h, p), u[y * 3] = Math.floor(p[0] * 255 + .5), u[y * 3 + 1] = Math.floor(p[1] * 255 + .5), u[y * 3 + 2] = Math.floor(p[2] * 255 + .5)
+                    var h = f[y * u + o];
+                    e.getColor(h, g), i[y * 3] = Math.floor(g[0] * 255 + .5), i[y * 3 + 1] = Math.floor(g[1] * 255 + .5), i[y * 3 + 2] = Math.floor(g[2] * 255 + .5)
                 }
-            if (a === X0.LUMINANCE)
+            if (a === K0.LUMINANCE)
                 for (var C = 0; C < s; C++) {
-                    var N = l[C * i + o];
-                    e.getColor(N, p), u[C] = Math.floor(p[0] * 76.5 + p[1] * 150.45 + p[2] * 28.05 + .5)
+                    var N = f[C * u + o];
+                    e.getColor(N, g), i[C] = Math.floor(g[0] * 76.5 + g[1] * 150.45 + g[2] * 28.05 + .5)
                 }
-            if (a === X0.LUMINANCE_ALPHA)
-                for (var R = 0; R < s; R++) {
-                    var B = l[R * i + o];
-                    e.getColor(B, p), u[R * 2] = Math.floor(p[0] * 76.5 + p[1] * 150.45 + p[2] * 28.05 + .5), u[R * 2 + 1] = c
+            if (a === K0.LUMINANCE_ALPHA)
+                for (var x = 0; x < s; x++) {
+                    var B = f[x * u + o];
+                    e.getColor(B, g), i[x * 2] = Math.floor(g[0] * 76.5 + g[1] * 150.45 + g[2] * 28.05 + .5), i[x * 2 + 1] = c
                 }
         }, e.applyColorMap = function(r) {
-            if (r.ColorSpace && (t.colorSpace = Z[r.ColorSpace.toUpperCase()], t.colorSpace === void 0 && (n0("ColorSpace ".concat(r.ColorSpace, " not supported, using RGB instead")), t.colorSpace = Z.RGB)), r.NanColor)
+            if (r.ColorSpace && (t.colorSpace = n0[r.ColorSpace.toUpperCase()], t.colorSpace === void 0 && (s0("ColorSpace ".concat(r.ColorSpace, " not supported, using RGB instead")), t.colorSpace = n0.RGB)), r.NanColor)
                 for (t.nanColor = [].concat(r.NanColor); t.nanColor.length < 4;) t.nanColor.push(1);
             if (r.RGBPoints) {
                 var n = r.RGBPoints.length;
                 t.nodes = [];
                 for (var a = .5, o = 0, c = 0; c < n; c += 4) t.nodes.push({
                     x: r.RGBPoints[c],
                     r: r.RGBPoints[c + 1],
@@ -4408,43 +4408,43 @@
                     midpoint: a,
                     sharpness: o
                 })
             }
             e.sortAndUpdateRange()
         }
     }
-    var b8 = {
+    var R8 = {
         clamping: !0,
-        colorSpace: Z.RGB,
+        colorSpace: n0.RGB,
         hSVWrap: !0,
-        scale: Y2.LINEAR,
+        scale: J2.LINEAR,
         nanColor: null,
         belowRangeColor: null,
         aboveRangeColor: null,
         useAboveRangeColor: !1,
         useBelowRangeColor: !1,
         allowDuplicateScalars: !1,
         table: null,
         tableSize: 0,
         buildTime: null,
         nodes: null,
         discretize: !1,
         numberOfValues: 256
     };
 
-    function J2(e, t) {
+    function t9(e, t) {
         var r = arguments.length > 2 && arguments[2] !== void 0 ? arguments[2] : {};
-        Object.assign(t, b8, r), I2.extend(e, t, r), t.table = [], t.nodes = [], t.nanColor = [.5, 0, 0, 1], t.belowRangeColor = [0, 0, 0, 1], t.aboveRangeColor = [1, 1, 1, 1], t.buildTime = {}, z.obj(t.buildTime), z.get(e, t, ["buildTime", "mappingRange"]), z.setGet(e, t, ["useAboveRangeColor", "useBelowRangeColor", "colorSpace", "discretize", "numberOfValues"]), z.setArray(e, t, ["nanColor", "belowRangeColor", "aboveRangeColor"], 4), z.getArray(e, t, ["nanColor", "belowRangeColor", "aboveRangeColor"]), w8(e, t)
+        Object.assign(t, R8, r), q2.extend(e, t, r), t.table = [], t.nodes = [], t.nanColor = [.5, 0, 0, 1], t.belowRangeColor = [0, 0, 0, 1], t.aboveRangeColor = [1, 1, 1, 1], t.buildTime = {}, W.obj(t.buildTime), W.get(e, t, ["buildTime", "mappingRange"]), W.setGet(e, t, ["useAboveRangeColor", "useBelowRangeColor", "colorSpace", "discretize", "numberOfValues"]), W.setArray(e, t, ["nanColor", "belowRangeColor", "aboveRangeColor"], 4), W.getArray(e, t, ["nanColor", "belowRangeColor", "aboveRangeColor"]), x8(e, t)
     }
-    var N8 = z.newInstance(J2, "vtkColorTransferFunction"),
-        B8 = d8({
-            newInstance: N8,
-            extend: J2
-        }, M1),
-        R8 = [{
+    var O8 = W.newInstance(t9, "vtkColorTransferFunction"),
+        T8 = S8({
+            newInstance: O8,
+            extend: t9
+        }, k1),
+        M8 = [{
             Name: "KAAMS",
             IndexedColors: [1, 1, 1, 1, 0, 0, 0, 1, 0, 0, 0, 1, 1, 1, 0, 1, 0, 1, 0, 1, 1, .63, .63, 1, .67, .5, .33, 1, .5, .75, .53, .35, .7, 1, .75, .5],
             Annotations: [0, 0, 1, 1, 2, 2, 3, 3, 4, 4, 5, 5, 6, 6, 7, 7, 8, 8, 9, 9, 10, 10, 11, 11]
         }, {
             ColorSpace: "Diverging",
             Name: "Cool to Warm",
             NanColor: [1, 1, 0],
@@ -5245,63 +5245,63 @@
             RGBPoints: [0, .267004, .004874, .329415, .003922, .26851, .009605, .335427, .007843, .269944, .014625, .341379, .011765, .271305, .019942, .347269, .015686, .272594, .025563, .353093, .019608, .273809, .031497, .358853, .023529, .274952, .037752, .364543, .027451, .276022, .044167, .370164, .031373, .277018, .050344, .375715, .035294, .277941, .056324, .381191, .039216, .278791, .062145, .386592, .043137, .279566, .067836, .391917, .047059, .280267, .073417, .397163, .05098, .280894, .078907, .402329, .054902, .281446, .08432, .407414, .058824, .281924, .089666, .412415, .062745, .282327, .094955, .417331, .066667, .282656, .100196, .42216, .070588, .28291, .105393, .426902, .07451, .283091, .110553, .431554, .078431, .283197, .11568, .436115, .082353, .283229, .120777, .440584, .086275, .283187, .125848, .44496, .090196, .283072, .130895, .449241, .094118, .282884, .13592, .453427, .098039, .282623, .140926, .457517, .101961, .28229, .145912, .46151, .105882, .281887, .150881, .465405, .109804, .281412, .155834, .469201, .113725, .280868, .160771, .472899, .117647, .280255, .165693, .476498, .121569, .279574, .170599, .479997, .12549, .278826, .17549, .483397, .129412, .278012, .180367, .486697, .133333, .277134, .185228, .489898, .137255, .276194, .190074, .493001, .141176, .275191, .194905, .496005, .145098, .274128, .199721, .498911, .14902, .273006, .20452, .501721, .152941, .271828, .209303, .504434, .156863, .270595, .214069, .507052, .160784, .269308, .218818, .509577, .164706, .267968, .223549, .512008, .168627, .26658, .228262, .514349, .172549, .265145, .232956, .516599, .176471, .263663, .237631, .518762, .180392, .262138, .242286, .520837, .184314, .260571, .246922, .522828, .188235, .258965, .251537, .524736, .192157, .257322, .25613, .526563, .196078, .255645, .260703, .528312, .2, .253935, .265254, .529983, .203922, .252194, .269783, .531579, .207843, .250425, .27429, .533103, .211765, .248629, .278775, .534556, .215686, .246811, .283237, .535941, .219608, .244972, .287675, .53726, .223529, .243113, .292092, .538516, .227451, .241237, .296485, .539709, .231373, .239346, .300855, .540844, .235294, .237441, .305202, .541921, .239216, .235526, .309527, .542944, .243137, .233603, .313828, .543914, .247059, .231674, .318106, .544834, .25098, .229739, .322361, .545706, .254902, .227802, .326594, .546532, .258824, .225863, .330805, .547314, .262745, .223925, .334994, .548053, .266667, .221989, .339161, .548752, .270588, .220057, .343307, .549413, .27451, .21813, .347432, .550038, .278431, .21621, .351535, .550627, .282353, .214298, .355619, .551184, .286275, .212395, .359683, .55171, .290196, .210503, .363727, .552206, .294118, .208623, .367752, .552675, .298039, .206756, .371758, .553117, .301961, .204903, .375746, .553533, .305882, .203063, .379716, .553925, .309804, .201239, .38367, .554294, .313725, .19943, .387607, .554642, .317647, .197636, .391528, .554969, .321569, .19586, .395433, .555276, .32549, .1941, .399323, .555565, .329412, .192357, .403199, .555836, .333333, .190631, .407061, .556089, .337255, .188923, .41091, .556326, .341176, .187231, .414746, .556547, .345098, .185556, .41857, .556753, .34902, .183898, .422383, .556944, .352941, .182256, .426184, .55712, .356863, .180629, .429975, .557282, .360784, .179019, .433756, .55743, .364706, .177423, .437527, .557565, .368627, .175841, .44129, .557685, .372549, .174274, .445044, .557792, .376471, .172719, .448791, .557885, .380392, .171176, .45253, .557965, .384314, .169646, .456262, .55803, .388235, .168126, .459988, .558082, .392157, .166617, .463708, .558119, .396078, .165117, .467423, .558141, .4, .163625, .471133, .558148, .403922, .162142, .474838, .55814, .407843, .160665, .47854, .558115, .411765, .159194, .482237, .558073, .415686, .157729, .485932, .558013, .419608, .15627, .489624, .557936, .423529, .154815, .493313, .55784, .427451, .153364, .497, .557724, .431373, .151918, .500685, .557587, .435294, .150476, .504369, .55743, .439216, .149039, .508051, .55725, .443137, .147607, .511733, .557049, .447059, .14618, .515413, .556823, .45098, .144759, .519093, .556572, .454902, .143343, .522773, .556295, .458824, .141935, .526453, .555991, .462745, .140536, .530132, .555659, .466667, .139147, .533812, .555298, .470588, .13777, .537492, .554906, .47451, .136408, .541173, .554483, .478431, .135066, .544853, .554029, .482353, .133743, .548535, .553541, .486275, .132444, .552216, .553018, .490196, .131172, .555899, .552459, .494118, .129933, .559582, .551864, .498039, .128729, .563265, .551229, .501961, .127568, .566949, .550556, .505882, .126453, .570633, .549841, .509804, .125394, .574318, .549086, .513725, .124395, .578002, .548287, .517647, .123463, .581687, .547445, .521569, .122606, .585371, .546557, .52549, .121831, .589055, .545623, .529412, .121148, .592739, .544641, .533333, .120565, .596422, .543611, .537255, .120092, .600104, .54253, .541176, .119738, .603785, .5414, .545098, .119512, .607464, .540218, .54902, .119423, .611141, .538982, .552941, .119483, .614817, .537692, .556863, .119699, .61849, .536347, .560784, .120081, .622161, .534946, .564706, .120638, .625828, .533488, .568627, .12138, .629492, .531973, .572549, .122312, .633153, .530398, .576471, .123444, .636809, .528763, .580392, .12478, .640461, .527068, .584314, .126326, .644107, .525311, .588235, .128087, .647749, .523491, .592157, .130067, .651384, .521608, .596078, .132268, .655014, .519661, .6, .134692, .658636, .517649, .603922, .137339, .662252, .515571, .607843, .14021, .665859, .513427, .611765, .143303, .669459, .511215, .615686, .146616, .67305, .508936, .619608, .150148, .676631, .506589, .623529, .153894, .680203, .504172, .627451, .157851, .683765, .501686, .631373, .162016, .687316, .499129, .635294, .166383, .690856, .496502, .639216, .170948, .694384, .493803, .643137, .175707, .6979, .491033, .647059, .180653, .701402, .488189, .65098, .185783, .704891, .485273, .654902, .19109, .708366, .482284, .658824, .196571, .711827, .479221, .662745, .202219, .715272, .476084, .666667, .20803, .718701, .472873, .670588, .214, .722114, .469588, .67451, .220124, .725509, .466226, .678431, .226397, .728888, .462789, .682353, .232815, .732247, .459277, .686275, .239374, .735588, .455688, .690196, .24607, .73891, .452024, .694118, .252899, .742211, .448284, .698039, .259857, .745492, .444467, .701961, .266941, .748751, .440573, .705882, .274149, .751988, .436601, .709804, .281477, .755203, .432552, .713725, .288921, .758394, .428426, .717647, .296479, .761561, .424223, .721569, .304148, .764704, .419943, .72549, .311925, .767822, .415586, .729412, .319809, .770914, .411152, .733333, .327796, .77398, .40664, .737255, .335885, .777018, .402049, .741176, .344074, .780029, .397381, .745098, .35236, .783011, .392636, .74902, .360741, .785964, .387814, .752941, .369214, .788888, .382914, .756863, .377779, .791781, .377939, .760784, .386433, .794644, .372886, .764706, .395174, .797475, .367757, .768627, .404001, .800275, .362552, .772549, .412913, .803041, .357269, .776471, .421908, .805774, .35191, .780392, .430983, .808473, .346476, .784314, .440137, .811138, .340967, .788235, .449368, .813768, .335384, .792157, .458674, .816363, .329727, .796078, .468053, .818921, .323998, .8, .477504, .821444, .318195, .803922, .487026, .823929, .312321, .807843, .496615, .826376, .306377, .811765, .506271, .828786, .300362, .815686, .515992, .831158, .294279, .819608, .525776, .833491, .288127, .823529, .535621, .835785, .281908, .827451, .545524, .838039, .275626, .831373, .555484, .840254, .269281, .835294, .565498, .84243, .262877, .839216, .575563, .844566, .256415, .843137, .585678, .846661, .249897, .847059, .595839, .848717, .243329, .85098, .606045, .850733, .236712, .854902, .616293, .852709, .230052, .858824, .626579, .854645, .223353, .862745, .636902, .856542, .21662, .866667, .647257, .8584, .209861, .870588, .657642, .860219, .203082, .87451, .668054, .861999, .196293, .878431, .678489, .863742, .189503, .882353, .688944, .865448, .182725, .886275, .699415, .867117, .175971, .890196, .709898, .868751, .169257, .894118, .720391, .87035, .162603, .898039, .730889, .871916, .156029, .901961, .741388, .873449, .149561, .905882, .751884, .874951, .143228, .909804, .762373, .876424, .137064, .913725, .772852, .877868, .131109, .917647, .783315, .879285, .125405, .921569, .79376, .880678, .120005, .92549, .804182, .882046, .114965, .929412, .814576, .883393, .110347, .933333, .82494, .88472, .106217, .937255, .83527, .886029, .102646, .941176, .845561, .887322, .099702, .945098, .85581, .888601, .097452, .94902, .866013, .889868, .095953, .952941, .876168, .891125, .09525, .956863, .886271, .892374, .095374, .960784, .89632, .893616, .096335, .964706, .906311, .894855, .098125, .968627, .916242, .896091, .100717, .972549, .926106, .89733, .104071, .976471, .935904, .89857, .108131, .980392, .945636, .899815, .112838, .984314, .9553, .901065, .118128, .988235, .964894, .902323, .123941, .992157, .974417, .90359, .130215, .996078, .983868, .904867, .136897, 1, .993248, .906157, .143936]
         }, {
             ShowIndexedColorActiveValues: 1,
             IndexedColors: [.07, .5, .7, 1, 1, 1, .85, 1, 1, .8, .5, 1, .76, 1, 0, 1, .71, .71, .5, .5, .5, .05, .05, 1, 1, .05, .05, .7, 1, 1, .7, .89, .96, .67, .36, .95, .54, 1, 0, .75, .65, .65, .5, .6, .6, 1, .5, 0, 1, 1, .19, .12, .94, .12, .5, .82, .89, .56, .25, .83, .24, 1, 0, .9, .9, .9, .75, .76, .78, .65, .65, .67, .54, .6, .78, .61, .48, .78, .5, .48, .78, .44, .48, .78, .36, .48, .76, 1, .48, .38, .49, .5, .69, .76, .56, .56, .4, .56, .56, .74, .5, .89, 1, .63, 0, .65, .16, .16, .36, .72, .82, .44, .18, .69, 0, 1, 0, .58, 1, 1, .58, .88, .88, .45, .76, .79, .33, .71, .71, .23, .62, .62, .14, .56, .56, .04, .49, .55, 0, .41, .52, .88, .88, 1, 1, .85, .56, .65, .46, .45, .4, .5, .5, .62, .39, .71, .83, .48, 0, .58, 0, .58, .26, .62, .69, .34, .09, .56, 0, .79, 0, .44, .83, 1, 1, 1, .78, .85, 1, .78, .78, 1, .78, .64, 1, .78, .56, 1, .78, .38, 1, .78, .27, 1, .78, .19, 1, .78, .12, 1, .78, 0, 1, .61, 0, .9, .46, 0, .83, .32, 0, .75, .22, 0, .67, .14, .3, .76, 1, .3, .65, 1, .13, .58, .84, .15, .49, .67, .15, .4, .59, .09, .33, .53, .96, .93, .82, .8, .82, .12, .71, .71, .76, .65, .33, .3, .34, .35, .38, .62, .31, .71, .67, .36, 0, .46, .31, .27, .26, .51, .59, .26, 0, .4, 0, .49, 0, .44, .67, .98, 0, .73, 1, 0, .63, 1, 0, .56, 1, 0, .5, 1, 0, .42, 1, .33, .36, .95, .47, .36, .89, .54, .31, .89, .63, .21, .83, .7, .12, .83, .7, .12, .73, .7, .05, .65, .74, .05, .53, .78, 0, .4, .8, 0, .35, .82, 0, .31, .85, 0, .27, .88, 0, .22, .9, 0, .18, .91, 0, .15, .92, 0, .14, .93, 0, .13, .94, 0, .12, .95, 0, .11, .96, 0, .1, .97, 0, .09, .98, 0, .08, .99, 0, .07, 1, 0, .06],
             Annotations: [0, "Xx", 1, "H", 2, "He", 3, "Li", 4, "Be", 5, "B", 6, "C", 7, "N", 8, "O", 9, "F", 10, "Ne", 11, "Na", 12, "Mg", 13, "Al", 14, "Si", 15, "P", 16, "S", 17, "Cl", 18, "Ar", 19, "K", 20, "Ca", 21, "Sc", 22, "Ti", 23, "V", 24, "Cr", 25, "Mn", 26, "Fe", 27, "Co", 28, "Ni", 29, "Cu", 30, "Zn", 31, "Ga", 32, "Ge", 33, "As", 34, "Se", 35, "Br", 36, "Kr", 37, "Rb", 38, "Sr", 39, "Y", 40, "Zr", 41, "Nb", 42, "Mo", 43, "Tc", 44, "Ru", 45, "Rh", 46, "Pd", 47, "Ag", 48, "Cd", 49, "In", 50, "Sn", 51, "Sb", 52, "Te", 53, "I", 54, "Xe", 55, "Cs", 56, "Ba", 57, "La", 58, "Ce", 59, "Pr", 60, "Nd", 61, "Pm", 62, "Sm", 63, "Eu", 64, "Gd", 65, "Tb", 66, "Dy", 67, "Ho", 68, "Er", 69, "Tm", 70, "Yb", 71, "Lu", 72, "Hf", 73, "Ta", 74, "W", 75, "Re", 76, "Os", 77, "Ir", 78, "Pt", 79, "Au", 80, "Hg", 81, "Tl", 82, "Pb", 83, "Bi", 84, "Po", 85, "At", 86, "Rn", 87, "Fr", 88, "Ra", 89, "Ac", 90, "Th", 91, "Pa", 92, "U", 93, "Np", 94, "Pu", 95, "Am", 96, "Cm", 97, "Bk", 98, "Cf", 99, "Es", 100, "Fm", 101, "Md", 102, "No", 103, "Lr", 104, "Rf", 105, "Db", 106, "Sg", 107, "Bh", 108, "Hs", 109, "Mt", 110, "Ds", 111, "Rg", 112, "Cn", 113, "Uut", 114, "Uuq", 115, "Uup", 116, "Uuh", 117, "Uus", 118, "Uuo"],
             Name: "BlueObeliskElements"
         }],
-        O0 = Object.create(null);
-    R8.filter(function(e) {
+        G0 = Object.create(null);
+    M8.filter(function(e) {
         return e.RGBPoints
     }).filter(function(e) {
         return e.ColorSpace !== "CIELAB"
     }).forEach(function(e) {
-        O0[e.Name] = e
+        G0[e.Name] = e
     });
-    var T0 = Object.keys(O0);
-    T0.sort();
+    var E0 = Object.keys(G0);
+    E0.sort();
 
-    function x8(e) {
-        return O0[e]
+    function G8(e) {
+        return G0[e]
     }
 
-    function O8(e) {
-        !e.RGBPoints || e.ColorSpace === "CIELAB" || (O0[e.Name] || (T0.push(e.Name), T0.sort()), O0[e.Name] = e)
+    function E8(e) {
+        !e.RGBPoints || e.ColorSpace === "CIELAB" || (G0[e.Name] || (E0.push(e.Name), E0.sort()), G0[e.Name] = e)
     }
 
-    function T8(e) {
-        var t = T0.indexOf(e);
-        t > -1 && T0.splice(t, 1), delete O0[e]
+    function k8(e) {
+        var t = E0.indexOf(e);
+        t > -1 && E0.splice(t, 1), delete G0[e]
     }
-    var Q2 = {
-        addPreset: O8,
-        removePresetByName: T8,
-        getPresetByName: x8,
-        rgbPresetNames: T0
+    var r9 = {
+        addPreset: E8,
+        removePresetByName: k8,
+        getPresetByName: G8,
+        rgbPresetNames: E0
     };
-    const G1 = document.createElement("canvas");
-    G1.width = 100, G1.height = 100;
+    const D1 = document.createElement("canvas");
+    D1.width = 100, D1.height = 100;
 
-    function M8(e, t, r, n) {
-        const o = G1.getContext("2d").createImageData(e, t);
+    function D8(e, t, r, n) {
+        const o = D1.getContext("2d").createImageData(e, t);
         for (let c = 0; c < t; c++)
             for (let s = 0; s < e; s++) {
-                const i = s + c * e,
-                    u = n(r[i]);
-                o.data[i * 4 + 0] = u[0], o.data[i * 4 + 1] = u[1], o.data[i * 4 + 2] = u[2], o.data[i * 4 + 3] = 255
+                const u = s + c * e,
+                    i = n(r[u]);
+                o.data[u * 4 + 0] = i[0], o.data[u * 4 + 1] = i[1], o.data[u * 4 + 2] = i[2], o.data[u * 4 + 3] = 255
             }
         return o
     }
     const {
-        ref: Z2,
-        computed: a0,
-        onMounted: G8,
-        nextTick: E8,
-        watch: q0
-    } = window.Vue, e9 = {
+        ref: n9,
+        computed: c0,
+        onMounted: L8,
+        nextTick: A8,
+        watch: J0
+    } = window.Vue, a9 = {
         props: {
             heatmap: {
                 type: [Array, Float32Array, Float64Array, Uint8Array, Uint16Array, Uint32Array, Int8Array, Int16Array, Int32Array],
                 default: () => []
             },
             shape: {
                 type: Array,
@@ -5321,297 +5321,286 @@
             }
         },
         emits: ["fullRange", "colorRange", "hover", "enter", "exit"],
         setup(e, {
             emit: t,
             expose: r
         }) {
-            const n = Z2(null),
-                a = Z2(null),
-                o = B8.newInstance();
-            o.applyColorMap(Q2.getPresetByName(e.colorPreset));
+            const n = n9(null),
+                a = n9(null),
+                o = T8.newInstance();
+            o.applyColorMap(r9.getPresetByName(e.colorPreset));
             const c = [0, 0, 0, 255];
 
             function s(S) {
                 return o.getColor(S, c), c[0] *= 255, c[1] *= 255, c[2] *= 255, c
             }
-            const i = a0(() => e.shape[0]),
-                u = a0(() => e.shape[1]),
-                l = a0(() => {
+            const u = c0(() => e.shape[0]),
+                i = c0(() => e.shape[1]),
+                f = c0(() => {
                     let S = e.heatmap[0],
-                        b = e.heatmap[0];
+                        w = e.heatmap[0];
                     for (let v = 0; v < e.heatmap.length; v++) {
                         const d = e.heatmap[v];
-                        S > d && (S = d), b < d && (b = d)
+                        S > d && (S = d), w < d && (w = d)
                     }
-                    return t("fullRange", [S, b]), [S, b]
+                    return t("fullRange", [S, w]), [S, w]
                 }),
-                p = a0(() => {
-                    const [S, b] = l.value, v = Math.max(-S, b);
+                g = c0(() => {
+                    const [S, w] = f.value, v = Math.max(-S, w);
                     return [-v, v]
                 }),
-                f = a0(() => {
-                    const [S, b] = l.value, v = Math.min(-S, b);
+                l = c0(() => {
+                    const [S, w] = f.value, v = Math.min(-S, w);
                     return [-v, v]
                 }),
-                g = a0(() => {
-                    const [, S] = l.value;
+                p = c0(() => {
+                    const [, S] = f.value;
                     return S < 0 ? [S, 0] : [0, S]
                 }),
-                y = a0(() => {
-                    const [S] = l.value;
+                y = c0(() => {
+                    const [S] = f.value;
                     return S > 0 ? [0, S] : [S, 0]
                 }),
-                h = a0(() => ({
-                    full: l.value,
-                    maxSym: p.value,
-                    minSym: f.value,
-                    positive: g.value,
+                h = c0(() => ({
+                    full: f.value,
+                    maxSym: g.value,
+                    minSym: l.value,
+                    positive: p.value,
                     negative: y.value,
                     custom: e.colorRange.map(Number)
                 })),
-                C = a0(() => h.value[e.colorMode] || l.value);
+                C = c0(() => h.value[e.colorMode] || f.value);
 
             function N() {
-                const [S, b] = C.value;
-                if (!i.value || !u.value || !(b - S) || !e.heatmap || (t("colorRange", [S, b]), o.setMappingRange(S, b), o.updateRange(), !i.value || !u.value)) return;
-                const v = M8(i.value, u.value, e.heatmap, s),
+                const [S, w] = C.value;
+                if (!u.value || !i.value || !(w - S) || !e.heatmap || (t("colorRange", [S, w]), o.setMappingRange(S, w), o.updateRange(), !u.value || !i.value)) return;
+                const v = D8(u.value, i.value, e.heatmap, s),
                     d = n.value.getContext("2d");
-                d.imageSmoothingEnabled = !1, d.clearRect(0, 0, i.value, u.value), d.putImageData(v, 0, 0)
+                d.imageSmoothingEnabled = !1, d.clearRect(0, 0, u.value, i.value), d.putImageData(v, 0, 0)
             }
 
-            function R() {
-                E8(N)
+            function x() {
+                A8(N)
             }
 
             function B(S) {
                 const {
-                    clientX: b,
+                    clientX: w,
                     clientY: v
                 } = S, {
                     top: d,
                     left: m,
-                    width: x,
+                    width: O,
                     height: D
-                } = a.value, P = (b - m) / x, U = 1 - (v - d) / D, H = Math.round(P * (i.value - 1)), O = Math.round(U * (u.value - 1));
+                } = a.value, _ = (w - m) / O, U = 1 - (v - d) / D, F = Math.round(_ * (u.value - 1)), T = Math.round(U * (i.value - 1));
                 t("hover", {
-                    i: H,
-                    j: O
+                    i: F,
+                    j: T
                 })
             }
 
-            function w() {
+            function b() {
                 t("enter"), a.value = n.value.getBoundingClientRect()
             }
-            return q0(() => C.value, R), q0(() => e.shape, R), q0(() => e.heatmap, R), q0(() => e.colorPreset, S => {
-                o.applyColorMap(Q2.getPresetByName(S)), R()
-            }), G8(R), r({
+            return J0(() => C.value, x), J0(() => e.shape, x), J0(() => e.heatmap, x), J0(() => e.colorPreset, S => {
+                o.applyColorMap(r9.getPresetByName(S)), x()
+            }), L8(x), r({
                 render: N
             }), {
                 canvasElem: n,
-                width: i,
-                height: u,
-                fullRange: l,
-                maxSymRange: p,
-                minSymRange: f,
-                positiveRange: g,
+                width: u,
+                height: i,
+                fullRange: f,
+                maxSymRange: g,
+                minSymRange: l,
+                positiveRange: p,
                 negativeRange: y,
                 colorRanges: h,
                 colorRangeToUse: C,
                 onMouseMove: B,
-                onMouseEnter: w,
+                onMouseEnter: b,
                 emit: t
             }
         },
         template: `
     <canvas 
         ref="canvasElem" 
         :width="width" 
         :height="height"
         @mousemove="onMouseMove" 
         @mouseenter="onMouseEnter" 
         @mouseleave="emit('exit')"
     >
     </canvas>`
     }, {
-        ref: _0,
-        toRefs: k8,
-        reactive: E1,
-        computed: K0,
-        onBeforeUnmount: A8,
-        watch: t9,
-        watchEffect: D8
-    } = window.Vue, r9 = {
-        TrameClientStateChange: o9,
-        TrameClientTriggers: s9,
-        TrameCursor: v9,
-        TrameFloatCard: h9,
-        TrameGitTree: R9,
-        TrameLifeCycleMonitor: T9,
-        TrameListBrowser: k9,
-        TrameMouseTrap: _9,
-        TrameSizeObserver: V9,
-        TrameXaiHeatMap: e9,
-        TrameXaiImage: {
-            components: {
-                XaiHeatMap: e9
+        ref: j0,
+        toRefs: P8,
+        reactive: L1,
+        computed: Q0,
+        onBeforeUnmount: _8,
+        watch: o9,
+        watchEffect: $8
+    } = window.Vue, j8 = {
+        components: {
+            XaiHeatMap: a9
+        },
+        emits: ["areaSelectionChange", "fullRange", "colorRange", "hover", "enter", "exit"],
+        props: {
+            src: {
+                type: String
             },
-            emits: ["areaSelectionChange", "fullRange", "colorRange", "hover", "enter", "exit"],
-            props: {
-                src: {
-                    type: String
-                },
-                maxHeight: {
-                    type: [String, Number]
-                },
-                maxWidth: {
-                    type: [String, Number]
-                },
-                width: {
-                    type: String
-                },
-                colors: {
-                    type: Array,
-                    default () {
-                        return ["#e1002a", "#417dc0", "#1d9a57", "#e9bc2f", "#9b3880"]
-                    }
-                },
-                areas: {
-                    type: Array
-                },
-                areaKey: {
-                    type: String,
-                    default: "name"
-                },
-                areaStyle: {
-                    type: Object,
-                    default () {
-                        return {
-                            "stroke-width": 3,
-                            rx: 10
-                        }
-                    }
-                },
-                areaSelected: {
-                    type: Array
-                },
-                areaSelectedOpacity: {
-                    type: [Number, String]
-                },
-                areaOpacity: {
-                    type: [Number, String]
-                },
-                heatmaps: {
-                    type: Object
-                },
-                heatmapOpacity: {
-                    type: [String, Number]
-                },
-                heatmapColorPreset: {
-                    type: [String, Object],
-                    default: "rainbow"
-                },
-                heatmapColorRange: {
-                    type: Array
-                },
-                heatmapActive: {
-                    type: String
-                },
-                heatmapColorMode: {
-                    type: String,
-                    default: "full"
-                }
+            maxHeight: {
+                type: [String, Number]
             },
-            setup(e, {
-                emit: t,
-                expose: r
-            }) {
-                const n = new Image,
-                    a = _0(0),
-                    o = _0(0),
-                    c = _0(1),
-                    s = _0(1),
-                    i = E1({}),
-                    u = E1({
-                        position: "relative"
-                    }),
-                    l = E1({
-                        position: "relative"
-                    }),
-                    p = _0({
-                        position: "absolute",
-                        top: 0,
-                        left: 0
-                    }),
-                    f = K0(() => {
-                        e.areaSelected;
-                        const w = e.areaSelectedOpacity ?? c.value,
-                            S = e.areaOpacity ?? s.value;
-                        return e.areas.map((b, v) => ({
-                            ...b,
-                            opacity: N(v) ? w : S,
-                            color: e.colors[v % e.colors.length]
-                        }))
-                    }),
-                    g = K0(() => e.heatmaps && e.heatmaps[e.heatmapActive]),
-                    y = K0(() => ({
-                        ...p.value,
-                        opacity: e.heatmapOpacity
-                    })),
-                    h = K0(() => [a.value, o.value]);
-
-                function C() {
-                    l.height = "auto", l.width = "auto";
-                    const w = {
-                        ...p.value
-                    };
-                    e.maxHeight ? (l.maxHeight = `min(${e.maxHeight}px, ${o.value||e.maxHeight}px)`, w.maxHeight = `min(${e.maxHeight}px, ${o.value||e.maxHeight}px)`) : (delete l.maxHeight, delete w.maxHeight), e.maxWidth ? (l.maxWidth = `min(${e.maxWidth}px, ${a.value||e.maxWidth}px)`, w.maxWidth = `min(${e.maxWidth}px, ${a.value||e.maxWidth}px)`) : (l.maxWidth = "100%", w.maxWidth = "100%"), e.width ? (u.width = e.width, l.width = e.width, w.width = e.width) : (delete u.width, delete w.width), p.value = w
-                }
-
-                function N(w) {
-                    const S = e.areas[w][e.areaKey];
-                    return e.areaSelected ? !!e.areaSelected.find(b => S == b) : !1
+            maxWidth: {
+                type: [String, Number]
+            },
+            width: {
+                type: String
+            },
+            colors: {
+                type: Array,
+                default () {
+                    return ["#e1002a", "#417dc0", "#1d9a57", "#e9bc2f", "#9b3880"]
                 }
-
-                function R(w, S) {
-                    const b = e.areas[w];
-                    i[b[e.areaKey]] = S;
-                    const v = [];
-                    for (let d = 0; d < e.areas.length; d++) {
-                        const m = e.areas[d][this.areaKey];
-                        i[m] && v.push(m)
+            },
+            areas: {
+                type: Array
+            },
+            areaKey: {
+                type: String,
+                default: "name"
+            },
+            areaStyle: {
+                type: Object,
+                default () {
+                    return {
+                        "stroke-width": 3,
+                        rx: 10
                     }
-                    t("areaSelectionChange", v)
-                }
-
-                function B() {
-                    a.value = this.width, o.value = this.height
-                }
-                return n.addEventListener("load", B), A8(() => {
-                    n.removeEventListener("load", B)
-                }), D8(() => n.src = e.src), t9(() => e.maxWidth, C), t9(() => e.maxHeight, C), r({
-                    updateAreaSelection: R
-                }), C(), {
-                    ...k8(e),
-                    imageWidth: a,
-                    imageHeight: o,
-                    areaSelectedOpacityValue: c,
-                    areaOpacityValue: s,
-                    containerStyle: u,
-                    imageStyle: l,
-                    annotationStyle: p,
-                    selectedAreas: i,
-                    decoratedAreas: f,
-                    activeHeatmap: g,
-                    heatMapStyle: y,
-                    shape: h,
-                    emit: t
                 }
             },
-            template: `
+            areaSelected: {
+                type: Array
+            },
+            areaSelectedOpacity: {
+                type: [Number, String]
+            },
+            areaOpacity: {
+                type: [Number, String]
+            },
+            heatmaps: {
+                type: Object
+            },
+            heatmapOpacity: {
+                type: [String, Number]
+            },
+            heatmapColorPreset: {
+                type: [String, Object],
+                default: "rainbow"
+            },
+            heatmapColorRange: {
+                type: Array
+            },
+            heatmapActive: {
+                type: String
+            },
+            heatmapColorMode: {
+                type: String,
+                default: "full"
+            }
+        },
+        setup(e, {
+            emit: t,
+            expose: r
+        }) {
+            const n = new Image,
+                a = j0(0),
+                o = j0(0),
+                c = j0(1),
+                s = j0(1),
+                u = L1({}),
+                i = L1({
+                    position: "relative"
+                }),
+                f = L1({
+                    position: "relative"
+                }),
+                g = j0({
+                    position: "absolute",
+                    top: 0,
+                    left: 0
+                }),
+                l = Q0(() => {
+                    e.areaSelected;
+                    const b = e.areaSelectedOpacity ?? c.value,
+                        S = e.areaOpacity ?? s.value;
+                    return e.areas.map((w, v) => ({
+                        ...w,
+                        opacity: N(v) ? b : S,
+                        color: e.colors[v % e.colors.length]
+                    }))
+                }),
+                p = Q0(() => e.heatmaps && e.heatmaps[e.heatmapActive]),
+                y = Q0(() => ({
+                    ...g.value,
+                    opacity: e.heatmapOpacity
+                })),
+                h = Q0(() => [a.value, o.value]);
+
+            function C() {
+                f.height = "auto", f.width = "auto";
+                const b = {
+                    ...g.value
+                };
+                e.maxHeight ? (f.maxHeight = `min(${e.maxHeight}px, ${o.value||e.maxHeight}px)`, b.maxHeight = `min(${e.maxHeight}px, ${o.value||e.maxHeight}px)`) : (delete f.maxHeight, delete b.maxHeight), e.maxWidth ? (f.maxWidth = `min(${e.maxWidth}px, ${a.value||e.maxWidth}px)`, b.maxWidth = `min(${e.maxWidth}px, ${a.value||e.maxWidth}px)`) : (f.maxWidth = "100%", b.maxWidth = "100%"), e.width ? (i.width = e.width, f.width = e.width, b.width = e.width) : (delete i.width, delete b.width), g.value = b
+            }
+
+            function N(b) {
+                const S = e.areas[b][e.areaKey];
+                return e.areaSelected ? !!e.areaSelected.find(w => S == w) : !1
+            }
+
+            function x(b, S) {
+                const w = e.areas[b];
+                u[w[e.areaKey]] = S;
+                const v = [];
+                for (let d = 0; d < e.areas.length; d++) {
+                    const m = e.areas[d][this.areaKey];
+                    u[m] && v.push(m)
+                }
+                t("areaSelectionChange", v)
+            }
+
+            function B() {
+                a.value = this.width, o.value = this.height
+            }
+            return n.addEventListener("load", B), _8(() => {
+                n.removeEventListener("load", B)
+            }), $8(() => n.src = e.src), o9(() => e.maxWidth, C), o9(() => e.maxHeight, C), r({
+                updateAreaSelection: x
+            }), C(), {
+                ...P8(e),
+                imageWidth: a,
+                imageHeight: o,
+                areaSelectedOpacityValue: c,
+                areaOpacityValue: s,
+                containerStyle: i,
+                imageStyle: f,
+                annotationStyle: g,
+                selectedAreas: u,
+                decoratedAreas: l,
+                activeHeatmap: p,
+                heatMapStyle: y,
+                shape: h,
+                emit: t
+            }
+        },
+        template: `
     <div :style="containerStyle">
       <img :src="src" :style="imageStyle" />
       <xai-heat-map
         :style="heatMapStyle"
         :heatmap="activeHeatmap"
         :shape="shape"
         :colorMode="heatmapColorMode"
@@ -5634,19 +5623,276 @@
           :stroke="item.color"
           :opacity="item.opacity"
           fill="none"
           v-bind="areaStyle"
         />
       </svg>
     </div>`
+    }, {
+        ref: q,
+        computed: Z0,
+        watch: A1,
+        unref: R,
+        toRefs: U8,
+        onMounted: F8,
+        onBeforeUnmount: V8
+    } = window.Vue, i9 = {
+        TrameClientStateChange: c9,
+        TrameClientTriggers: g9,
+        TrameCursor: m9,
+        TrameFloatCard: w9,
+        TrameGitTree: M9,
+        TrameLifeCycleMonitor: k9,
+        TrameListBrowser: P9,
+        TrameMouseTrap: F9,
+        TrameSizeObserver: W9,
+        TrameXaiHeatMap: a9,
+        TrameXaiImage: j8,
+        TrameLineSeed: {
+            props: {
+                point1: {
+                    type: Array,
+                    default () {
+                        return [0, 0, 0]
+                    }
+                },
+                point2: {
+                    type: Array,
+                    default () {
+                        return [0, 0, 0]
+                    }
+                },
+                numberOfSteps: {
+                    type: Number,
+                    default: 255
+                },
+                bounds: {
+                    type: Array,
+                    default () {
+                        return [-1, 1, -1, 1, -1, 1]
+                    }
+                },
+                image: {
+                    default: null
+                }
+            },
+            emit: ["update-seed"],
+            setup(e, {
+                emit: t
+            }) {
+                let r = 0,
+                    n = null,
+                    a = null;
+                const o = q(null),
+                    c = q([0, 0]),
+                    s = q(1),
+                    u = q(10),
+                    i = q([0, 0]),
+                    f = q([0, 0]),
+                    g = q(!1),
+                    l = q(e.point1[0]),
+                    p = q(e.point1[1]),
+                    y = q(e.point1[2]),
+                    h = q(e.point2[0]),
+                    C = q(e.point2[1]),
+                    N = q(e.point2[2]),
+                    x = q(!0),
+                    B = q(50),
+                    b = Z0(() => R(x) ? "#2196F3" : "#4CAF50"),
+                    S = Z0(() => (e.bounds[5] - e.bounds[4]) / e.numberOfSteps),
+                    w = Z0(() => (e.bounds[3] - e.bounds[2]) / 500),
+                    v = Z0(() => (e.bounds[5] - e.bounds[4]) / 500);
+
+                function d() {
+                    i.value = [500 - (R(p) - e.bounds[2]) / R(w), 500 - (R(y) - e.bounds[4]) / R(v)], f.value = [500 - (R(C) - e.bounds[2]) / R(w), 500 - (R(N) - e.bounds[4]) / R(v)]
+                }
+
+                function m() {
+                    if (!R(g)) return;
+                    const L = R(x) ? l : h;
+                    t("update-seed", {
+                        p1: [R(l), R(p), R(y)],
+                        p2: [R(L), R(C), R(N)]
+                    })
+                }
+
+                function O(L) {
+                    if (R(g) || (g.value = !0), r) {
+                        const V = n.clientX - L.clientX,
+                            Q = n.clientY - L.clientY;
+                        switch (r) {
+                            case 1:
+                                i.value = [a[0] - R(s) * V, a[1] - R(s) * Q], p.value = (500 - R(i)[0]) * R(w) + e.bounds[2], y.value = (500 - R(i)[1]) * R(v) + e.bounds[4];
+                                break;
+                            case 2:
+                                f.value = [a[0] - R(s) * V, a[1] - R(s) * Q], C.value = (500 - R(f)[0]) * R(w) + e.bounds[2], N.value = (500 - R(f)[1]) * R(v) + e.bounds[4];
+                                break;
+                            case 3:
+                                i.value = [a[0][0] - R(s) * V, a[0][1] - R(s) * Q], p.value = (500 - R(i)[0]) * R(w) + e.bounds[2], y.value = (500 - R(i)[1]) * R(v) + e.bounds[4], f.value = [a[1][0] - R(s) * V, a[1][1] - R(s) * Q], C.value = (500 - R(f)[0]) * R(w) + e.bounds[2], N.value = (500 - R(f)[1]) * R(v) + e.bounds[4];
+                                break
+                        }
+                        const K = [R(i)[0] - R(f)[0], R(i)[1] - R(f)[1]],
+                            a0 = Math.sqrt(K[0] * K[0] + K[1] * K[1]);
+                        a0 > 1e-4 && (K[0] /= a0, K[1] /= a0), c.value = K, m()
+                    }
+                }
+
+                function D(L, V) {
+                    switch (r = L, n = V, L) {
+                        case 1:
+                            a = R(i).slice();
+                            break;
+                        case 2:
+                            a = R(f).slice();
+                            break;
+                        case 3:
+                            a = [R(i).slice(), R(f).slice()];
+                            break
+                    }
+                }
+
+                function _() {
+                    r = 0
+                }
+
+                function U() {
+                    s.value = 500 / R(o).getBoundingClientRect().width
+                }
+                const F = new ResizeObserver(U);
+                F8(() => {
+                    console.log("svgContainer", R(o)), F.observe(R(o))
+                }), V8(() => F.disconnect()), A1(() => e.point1, L => {
+                    [l.value, p.value, y.value] = L, d()
+                }), A1(() => e.point2, L => {
+                    [h.value, C.value, N.value] = L, d()
+                }), A1(x, m), d();
+                const {
+                    image: T
+                } = U8(e);
+                return {
+                    svgContainer: o,
+                    onMouseMove: O,
+                    onMousePress: D,
+                    onMouseRelease: _,
+                    normalDelta: c,
+                    radius: u,
+                    p1: i,
+                    p2: f,
+                    nbSeeds: B,
+                    sharedDepth: x,
+                    x1: l,
+                    x2: h,
+                    step: S,
+                    pointColor2: b,
+                    pushLineSeed: m,
+                    image: T
+                }
+            },
+            template: `<v-col class="mt-2">
+  <svg viewBox="0 0 500 500"
+    ref="svgContainer"
+    width="100%"
+    @mousemove="onMouseMove"
+    @mouseup="onMouseRelease"
+  >
+    <image
+      :href="image"
+      x="0"
+      y="0"
+      width="500"
+      height="500"
+    />
+    <line
+      :x1="p1[0] - normalDelta[0] * radius"
+      :y1="p1[1] - normalDelta[1] * radius"
+      :x2="p2[0] + normalDelta[0] * radius"
+      :y2="p2[1] + normalDelta[1] * radius"
+      style="cursor: grab;stroke: rgba(0,0,0,0.25);stroke-width:8"
+      @mousedown="onMousePress(3, $event)"
+    />
+    <circle
+      :cx="p2[0]"
+      :cy="p2[1]"
+      :r="radius"
+      :stroke="pointColor2"
+      stroke-width="8"
+      fill="rgba(0,0,0,0)"
+      @mousedown="onMousePress(2, $event)"
+      style="cursor: pointer;"
+    />
+    <circle
+      :cx="p1[0]"
+      :cy="p1[1]"
+      r="10"
+      stroke="#2196F3"
+      stroke-width="8"
+      fill="rgba(0,0,0,0)"
+      @mousedown="onMousePress(1, $event)"
+      style="cursor: pointer;"
+    />
+  </svg>
+  <v-col class="pt-0">
+    <v-row class="align-center">
+      <v-col cols="12" md="11">
+      <v-text-field
+        density="compact"
+        hide-details
+        type="number"
+        min="5"
+        max="1000"
+        step="1"
+        label="Seeds count"
+        v-model="nbSeeds"
+      />
+      </v-col>
+      <v-col cols="12" md="1">
+      <v-switch
+        style="width: 80px" 
+        class="mt-0"
+        density="compact"
+        v-model="sharedDepth"
+        hide-details
+      />
+      </v-col>
+    </v-row>
+    <v-row>
+        <v-slider 
+            v-show="!sharedDepth" 
+            v-model="x2" 
+            track-color="green" 
+            color="green" 
+            density="compact" 
+            hide-details 
+            @update:modelValue="pushLineSeed" 
+            :min="bounds[0]" 
+            :max="bounds[1]" 
+            :step="step" 
+        />
+    </v-row>
+    <v-row>
+        <v-slider 
+            v-model="x1" 
+            track-color="blue" 
+            color="blue" 
+            density="compact"  
+            hide-details 
+            @update:modelValue="pushLineSeed"
+            :min="bounds[0]" 
+            :max="bounds[1]" 
+            :step="step" 
+        />
+    </v-row>
+  </v-col>
+</v-col>
+`
         }
     };
 
-    function L8(e) {
-        Object.keys(r9).forEach(t => {
-            e.component(t, r9[t])
+    function z8(e) {
+        Object.keys(i9).forEach(t => {
+            e.component(t, i9[t])
         })
     }
-    C0.install = L8, Object.defineProperty(C0, Symbol.toStringTag, {
+    b0.install = z8, Object.defineProperty(b0, Symbol.toStringTag, {
         value: "Module"
     })
 });
```

### Comparing `trame-components-2.2.1/trame_components/widgets/trame.py` & `trame-components-2.3.0/trame_components/widgets/trame.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     "MouseTrap",
     "SizeObserver",
     "FloatCard",
     "ListBrowser",
     "GitTree",
     "XaiHeatMap",
     "XaiImage",
+    "LineSeed",
 ]
 
 
 class HtmlElement(AbstractElement):
     def __init__(self, _elem_name, children=None, **kwargs):
         super().__init__(_elem_name, children, **kwargs)
         if self.server:
@@ -474,7 +475,27 @@
             ("area_selection_change", "areaSelectionChange"),
             "hover",
             "enter",
             "exit",
             ("color_range_change", "colorRange"),
             ("full_range_change", "fullRange"),
         ]
+
+
+# -----------------------------------------------------------------------------
+# TrameLineSeed
+# -----------------------------------------------------------------------------
+
+
+class LineSeed(HtmlElement):
+    def __init__(self, children=None, **kwargs):
+        super().__init__("trame-line-seed", children, **kwargs)
+        self._attr_names += [
+            ("point_1", "point1"),
+            ("point_2", "point2"),
+            ("number_steps", "numberOfSteps"),
+            "bounds",
+            "image",
+        ]
+        self._event_names += [
+            ("update_seed", "update-seed"),
+        ]
```

### Comparing `trame-components-2.2.1/trame_components.egg-info/PKG-INFO` & `trame-components-2.3.0/trame_components.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trame-components
-Version: 2.2.1
+Version: 2.3.0
 Summary: Core components for trame widgets
 Author: Kitware Inc.
 License: Apache License 2.0
 Keywords: Python,Interactive,Web,Application,Framework
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `trame-components-2.2.1/trame_components.egg-info/SOURCES.txt` & `trame-components-2.3.0/trame_components.egg-info/SOURCES.txt`

 * *Files identical despite different names*

