# Comparing `tmp/catppuccin_jupyterlab-0.2.0.tar.gz` & `tmp/catppuccin_jupyterlab-0.2.1.tar.gz`

## Comparing `catppuccin_jupyterlab-0.2.0.tar` & `catppuccin_jupyterlab-0.2.1.tar`

### file list

```diff
@@ -1,43 +1,46 @@
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 catppuccin_jupyterlab-0.2.0/.copier-answers.yml
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 catppuccin_jupyterlab-0.2.0/.editorconfig
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 catppuccin_jupyterlab-0.2.0/.prettierignore
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 catppuccin_jupyterlab-0.2.0/.yarnrc.yml
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 catppuccin_jupyterlab-0.2.0/CHANGELOG.md
--rw-r--r--   0        0        0     3930 2020-02-02 00:00:00.000000 catppuccin_jupyterlab-0.2.0/RELEASE.md
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 catppuccin_jupyterlab-0.2.0/install.json
--rw-r--r--   0        0        0     6433 2020-02-02 00:00:00.000000 catppuccin_jupyterlab-0.2.0/package.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 catppuccin_jupyterlab-0.2.0/setup.py
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 catppuccin_jupyterlab-0.2.0/tsconfig.json
--rw-r--r--   0        0        0   199166 2020-02-02 00:00:00.000000 catppuccin_jupyterlab-0.2.0/yarn.lock
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 catppuccin_jupyterlab-0.2.0/assets/.gitkeep
--rw-r--r--   0        0        0    91456 2020-02-02 00:00:00.000000 catppuccin_jupyterlab-0.2.0/assets/frappe.webp
--rw-r--r--   0        0        0    92726 2020-02-02 00:00:00.000000 catppuccin_jupyterlab-0.2.0/assets/latte.webp
--rw-r--r--   0        0        0    93536 2020-02-02 00:00:00.000000 catppuccin_jupyterlab-0.2.0/assets/macchiato.webp
--rw-r--r--   0        0        0    95586 2020-02-02 00:00:00.000000 catppuccin_jupyterlab-0.2.0/assets/mocha-brand.webp
--rw-r--r--   0        0        0    95400 2020-02-02 00:00:00.000000 catppuccin_jupyterlab-0.2.0/assets/mocha.webp
--rw-r--r--   0        0        0   205072 2020-02-02 00:00:00.000000 catppuccin_jupyterlab-0.2.0/assets/preview.webp
--rw-r--r--   0        0        0    15260 2020-02-02 00:00:00.000000 catppuccin_jupyterlab-0.2.0/assets/settings.webp
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 catppuccin_jupyterlab-0.2.0/catppuccin_jupyterlab/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 catppuccin_jupyterlab-0.2.0/catppuccin_jupyterlab/_version.py
--rw-r--r--   0        0        0     5673 2020-02-02 00:00:00.000000 catppuccin_jupyterlab-0.2.0/catppuccin_jupyterlab/labextension/package.json
--rw-r--r--   0        0        0     6433 2020-02-02 00:00:00.000000 catppuccin_jupyterlab-0.2.0/catppuccin_jupyterlab/labextension/schemas/catppuccin_jupyterlab/package.json.orig
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 catppuccin_jupyterlab-0.2.0/catppuccin_jupyterlab/labextension/schemas/catppuccin_jupyterlab/plugin.json
--rw-r--r--   0        0        0     9253 2020-02-02 00:00:00.000000 catppuccin_jupyterlab-0.2.0/catppuccin_jupyterlab/labextension/static/649.5fbedda80fda1f1c26e7.js
--rw-r--r--   0        0        0     6260 2020-02-02 00:00:00.000000 catppuccin_jupyterlab-0.2.0/catppuccin_jupyterlab/labextension/static/remoteEntry.dafa4d2843fffc35a6db.js
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 catppuccin_jupyterlab-0.2.0/catppuccin_jupyterlab/labextension/static/style.js
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 catppuccin_jupyterlab-0.2.0/catppuccin_jupyterlab/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0    19543 2020-02-02 00:00:00.000000 catppuccin_jupyterlab-0.2.0/catppuccin_jupyterlab/labextension/themes/catppuccin_jupyterlab/index.css
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 catppuccin_jupyterlab-0.2.0/catppuccin_jupyterlab/labextension/themes/catppuccin_jupyterlab/index.js
--rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 catppuccin_jupyterlab-0.2.0/examples/markdown.md
--rw-r--r--   0        0        0    35405 2020-02-02 00:00:00.000000 catppuccin_jupyterlab-0.2.0/examples/python.ipynb
--rw-r--r--   0        0        0    30282 2020-02-02 00:00:00.000000 catppuccin_jupyterlab-0.2.0/examples/r.ipynb
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 catppuccin_jupyterlab-0.2.0/schema/plugin.json
--rw-r--r--   0        0        0     2787 2020-02-02 00:00:00.000000 catppuccin_jupyterlab-0.2.0/src/index.ts
--rw-r--r--   0        0        0     8766 2020-02-02 00:00:00.000000 catppuccin_jupyterlab-0.2.0/src/palettes.ts
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 catppuccin_jupyterlab-0.2.0/style/index.css
--rw-r--r--   0        0        0    19331 2020-02-02 00:00:00.000000 catppuccin_jupyterlab-0.2.0/style/variables.css
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 catppuccin_jupyterlab-0.2.0/.gitignore
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 catppuccin_jupyterlab-0.2.0/LICENSE
--rw-r--r--   0        0        0     3656 2020-02-02 00:00:00.000000 catppuccin_jupyterlab-0.2.0/README.md
--rw-r--r--   0        0        0     2292 2020-02-02 00:00:00.000000 catppuccin_jupyterlab-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     5967 2020-02-02 00:00:00.000000 catppuccin_jupyterlab-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 catppuccin_jupyterlab-0.2.1/.copier-answers.yml
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 catppuccin_jupyterlab-0.2.1/.editorconfig
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 catppuccin_jupyterlab-0.2.1/.prettierignore
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 catppuccin_jupyterlab-0.2.1/.yarnrc.yml
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 catppuccin_jupyterlab-0.2.1/CHANGELOG.md
+-rw-r--r--   0        0        0     3930 2020-02-02 00:00:00.000000 catppuccin_jupyterlab-0.2.1/RELEASE.md
+-rw-r--r--   0        0        0     2043 2020-02-02 00:00:00.000000 catppuccin_jupyterlab-0.2.1/index.tera
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 catppuccin_jupyterlab-0.2.1/install.json
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 catppuccin_jupyterlab-0.2.1/jupyterlab.tera
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 catppuccin_jupyterlab-0.2.1/justfile
+-rw-r--r--   0        0        0     6433 2020-02-02 00:00:00.000000 catppuccin_jupyterlab-0.2.1/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 catppuccin_jupyterlab-0.2.1/setup.py
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 catppuccin_jupyterlab-0.2.1/tsconfig.json
+-rw-r--r--   0        0        0   199166 2020-02-02 00:00:00.000000 catppuccin_jupyterlab-0.2.1/yarn.lock
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 catppuccin_jupyterlab-0.2.1/assets/.gitkeep
+-rw-r--r--   0        0        0    91456 2020-02-02 00:00:00.000000 catppuccin_jupyterlab-0.2.1/assets/frappe.webp
+-rw-r--r--   0        0        0    92726 2020-02-02 00:00:00.000000 catppuccin_jupyterlab-0.2.1/assets/latte.webp
+-rw-r--r--   0        0        0    93536 2020-02-02 00:00:00.000000 catppuccin_jupyterlab-0.2.1/assets/macchiato.webp
+-rw-r--r--   0        0        0    95586 2020-02-02 00:00:00.000000 catppuccin_jupyterlab-0.2.1/assets/mocha-brand.webp
+-rw-r--r--   0        0        0    95400 2020-02-02 00:00:00.000000 catppuccin_jupyterlab-0.2.1/assets/mocha.webp
+-rw-r--r--   0        0        0   205072 2020-02-02 00:00:00.000000 catppuccin_jupyterlab-0.2.1/assets/preview.webp
+-rw-r--r--   0        0        0    15260 2020-02-02 00:00:00.000000 catppuccin_jupyterlab-0.2.1/assets/settings.webp
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 catppuccin_jupyterlab-0.2.1/catppuccin_jupyterlab/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 catppuccin_jupyterlab-0.2.1/catppuccin_jupyterlab/_version.py
+-rw-r--r--   0        0        0     5673 2020-02-02 00:00:00.000000 catppuccin_jupyterlab-0.2.1/catppuccin_jupyterlab/labextension/package.json
+-rw-r--r--   0        0        0     6433 2020-02-02 00:00:00.000000 catppuccin_jupyterlab-0.2.1/catppuccin_jupyterlab/labextension/schemas/catppuccin_jupyterlab/package.json.orig
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 catppuccin_jupyterlab-0.2.1/catppuccin_jupyterlab/labextension/schemas/catppuccin_jupyterlab/plugin.json
+-rw-r--r--   0        0        0     9252 2020-02-02 00:00:00.000000 catppuccin_jupyterlab-0.2.1/catppuccin_jupyterlab/labextension/static/649.d990bd40ed4bd0441591.js
+-rw-r--r--   0        0        0     6258 2020-02-02 00:00:00.000000 catppuccin_jupyterlab-0.2.1/catppuccin_jupyterlab/labextension/static/remoteEntry.b3a8b3a1d29fe76e2c73.js
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 catppuccin_jupyterlab-0.2.1/catppuccin_jupyterlab/labextension/static/style.js
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 catppuccin_jupyterlab-0.2.1/catppuccin_jupyterlab/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0    19543 2020-02-02 00:00:00.000000 catppuccin_jupyterlab-0.2.1/catppuccin_jupyterlab/labextension/themes/catppuccin_jupyterlab/index.css
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 catppuccin_jupyterlab-0.2.1/catppuccin_jupyterlab/labextension/themes/catppuccin_jupyterlab/index.js
+-rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 catppuccin_jupyterlab-0.2.1/examples/markdown.md
+-rw-r--r--   0        0        0    35405 2020-02-02 00:00:00.000000 catppuccin_jupyterlab-0.2.1/examples/python.ipynb
+-rw-r--r--   0        0        0    30282 2020-02-02 00:00:00.000000 catppuccin_jupyterlab-0.2.1/examples/r.ipynb
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 catppuccin_jupyterlab-0.2.1/schema/plugin.json
+-rw-r--r--   0        0        0     2787 2020-02-02 00:00:00.000000 catppuccin_jupyterlab-0.2.1/src/index.ts
+-rw-r--r--   0        0        0     8766 2020-02-02 00:00:00.000000 catppuccin_jupyterlab-0.2.1/src/palettes.ts
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 catppuccin_jupyterlab-0.2.1/style/index.css
+-rw-r--r--   0        0        0    19331 2020-02-02 00:00:00.000000 catppuccin_jupyterlab-0.2.1/style/variables.css
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 catppuccin_jupyterlab-0.2.1/.gitignore
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 catppuccin_jupyterlab-0.2.1/LICENSE
+-rw-r--r--   0        0        0     3656 2020-02-02 00:00:00.000000 catppuccin_jupyterlab-0.2.1/README.md
+-rw-r--r--   0        0        0     2292 2020-02-02 00:00:00.000000 catppuccin_jupyterlab-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     5985 2020-02-02 00:00:00.000000 catppuccin_jupyterlab-0.2.1/PKG-INFO
```

### Comparing `catppuccin_jupyterlab-0.2.0/.copier-answers.yml` & `catppuccin_jupyterlab-0.2.1/.copier-answers.yml`

 * *Files identical despite different names*

### Comparing `catppuccin_jupyterlab-0.2.0/.editorconfig` & `catppuccin_jupyterlab-0.2.1/.editorconfig`

 * *Files identical despite different names*

### Comparing `catppuccin_jupyterlab-0.2.0/RELEASE.md` & `catppuccin_jupyterlab-0.2.1/RELEASE.md`

 * *Files identical despite different names*

### Comparing `catppuccin_jupyterlab-0.2.0/package.json` & `catppuccin_jupyterlab-0.2.1/catppuccin_jupyterlab/labextension/schemas/catppuccin_jupyterlab/package.json.orig`

 * *Files identical despite different names*

### Comparing `catppuccin_jupyterlab-0.2.0/tsconfig.json` & `catppuccin_jupyterlab-0.2.1/tsconfig.json`

 * *Files identical despite different names*

### Comparing `catppuccin_jupyterlab-0.2.0/yarn.lock` & `catppuccin_jupyterlab-0.2.1/yarn.lock`

 * *Files identical despite different names*

### Comparing `catppuccin_jupyterlab-0.2.0/assets/frappe.webp` & `catppuccin_jupyterlab-0.2.1/assets/frappe.webp`

 * *Files identical despite different names*

### Comparing `catppuccin_jupyterlab-0.2.0/assets/latte.webp` & `catppuccin_jupyterlab-0.2.1/assets/latte.webp`

 * *Files identical despite different names*

### Comparing `catppuccin_jupyterlab-0.2.0/assets/macchiato.webp` & `catppuccin_jupyterlab-0.2.1/assets/macchiato.webp`

 * *Files identical despite different names*

### Comparing `catppuccin_jupyterlab-0.2.0/assets/mocha-brand.webp` & `catppuccin_jupyterlab-0.2.1/assets/mocha-brand.webp`

 * *Files identical despite different names*

### Comparing `catppuccin_jupyterlab-0.2.0/assets/mocha.webp` & `catppuccin_jupyterlab-0.2.1/assets/mocha.webp`

 * *Files identical despite different names*

### Comparing `catppuccin_jupyterlab-0.2.0/assets/preview.webp` & `catppuccin_jupyterlab-0.2.1/assets/preview.webp`

 * *Files identical despite different names*

### Comparing `catppuccin_jupyterlab-0.2.0/assets/settings.webp` & `catppuccin_jupyterlab-0.2.1/assets/settings.webp`

 * *Files identical despite different names*

### Comparing `catppuccin_jupyterlab-0.2.0/catppuccin_jupyterlab/__init__.py` & `catppuccin_jupyterlab-0.2.1/catppuccin_jupyterlab/__init__.py`

 * *Files identical despite different names*

### Comparing `catppuccin_jupyterlab-0.2.0/catppuccin_jupyterlab/labextension/package.json` & `catppuccin_jupyterlab-0.2.1/catppuccin_jupyterlab/labextension/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9994318181818183%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.b3a8b3a1d29fe76e2c73.js'}}"}*

```diff
@@ -101,15 +101,15 @@
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "schema/*.json"
     ],
     "homepage": "https://github.com/catppuccin/jupyterlab",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.dafa4d2843fffc35a6db.js"
+            "load": "static/remoteEntry.b3a8b3a1d29fe76e2c73.js"
         },
         "extension": true,
         "outputDir": "catppuccin_jupyterlab/labextension",
         "schemaDir": "schema",
         "themePath": "style/index.css"
     },
     "keywords": [
```

### Comparing `catppuccin_jupyterlab-0.2.0/catppuccin_jupyterlab/labextension/schemas/catppuccin_jupyterlab/package.json.orig` & `catppuccin_jupyterlab-0.2.1/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9772727272727273%*

 * *Differences: {"'version'": "'0.2.1'"}*

```diff
@@ -181,9 +181,9 @@
             "csstree/validator": true,
             "property-no-vendor-prefix": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.2.0"
+    "version": "0.2.1"
 }
```

### Comparing `catppuccin_jupyterlab-0.2.0/catppuccin_jupyterlab/labextension/schemas/catppuccin_jupyterlab/plugin.json` & `catppuccin_jupyterlab-0.2.1/catppuccin_jupyterlab/labextension/schemas/catppuccin_jupyterlab/plugin.json`

 * *Files identical despite different names*

### Comparing `catppuccin_jupyterlab-0.2.0/catppuccin_jupyterlab/labextension/static/649.5fbedda80fda1f1c26e7.js` & `catppuccin_jupyterlab-0.2.1/catppuccin_jupyterlab/labextension/static/649.d990bd40ed4bd0441591.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,16 +1,16 @@
 "use strict";
 (self.webpackChunkcatppuccin_jupyterlab = self.webpackChunkcatppuccin_jupyterlab || []).push([
     [649], {
         649: (e, t, c) => {
             c.r(t), c.d(t, {
                 default: () => m
             });
-            var o = c(609),
-                l = c(426);
+            var o = c(464),
+                l = c(99);
             class n {
                 setConfigColors(e, t) {
                     document.documentElement.style.setProperty("--ctp-cfg-brand-color", `var(--ctp-plt-${e})`), document.documentElement.style.setProperty("--ctp-cfg-accent-color", `var(--ctp-plt-${t})`)
                 }
                 setColorsLatte() {
                     document.documentElement.style.setProperty("--ctp-plt-rosewater", "#dc8a78"), document.documentElement.style.setProperty("--ctp-plt-flamingo", "#dd7878"), document.documentElement.style.setProperty("--ctp-plt-pink", "#ea76cb"), document.documentElement.style.setProperty("--ctp-plt-mauve", "#8839ef"), document.documentElement.style.setProperty("--ctp-plt-red", "#d20f39"), document.documentElement.style.setProperty("--ctp-plt-maroon", "#e64553"), document.documentElement.style.setProperty("--ctp-plt-peach", "#fe640b"), document.documentElement.style.setProperty("--ctp-plt-yellow", "#df8e1d"), document.documentElement.style.setProperty("--ctp-plt-green", "#40a02b"), document.documentElement.style.setProperty("--ctp-plt-teal", "#179299"), document.documentElement.style.setProperty("--ctp-plt-sky", "#04a5e5"), document.documentElement.style.setProperty("--ctp-plt-sapphire", "#209fb5"), document.documentElement.style.setProperty("--ctp-plt-blue", "#1e66f5"), document.documentElement.style.setProperty("--ctp-plt-lavender", "#7287fd"), document.documentElement.style.setProperty("--ctp-plt-text", "#4c4f69"), document.documentElement.style.setProperty("--ctp-plt-subtext1", "#5c5f77"), document.documentElement.style.setProperty("--ctp-plt-subtext0", "#6c6f85"), document.documentElement.style.setProperty("--ctp-plt-overlay2", "#7c7f93"), document.documentElement.style.setProperty("--ctp-plt-overlay1", "#8c8fa1"), document.documentElement.style.setProperty("--ctp-plt-overlay0", "#9ca0b0"), document.documentElement.style.setProperty("--ctp-plt-surface2", "#acb0be"), document.documentElement.style.setProperty("--ctp-plt-surface1", "#bcc0cc"), document.documentElement.style.setProperty("--ctp-plt-surface0", "#ccd0da"), document.documentElement.style.setProperty("--ctp-plt-base", "#eff1f5"), document.documentElement.style.setProperty("--ctp-plt-mantle", "#e6e9ef"), document.documentElement.style.setProperty("--ctp-plt-crust", "#dce0e8")
                 }
```

### Comparing `catppuccin_jupyterlab-0.2.0/catppuccin_jupyterlab/labextension/static/remoteEntry.dafa4d2843fffc35a6db.js` & `catppuccin_jupyterlab-0.2.1/catppuccin_jupyterlab/labextension/static/remoteEntry.b3a8b3a1d29fe76e2c73.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -1,12 +1,12 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
     var e, r, t, n, o, a, i, u, l, p, f, s, c, d, h, v, g = {
-            900: (e, r, t) => {
+            144: (e, r, t) => {
                 var n = {
                         "./index": () => t.e(649).then((() => () => t(649))),
                         "./extension": () => t.e(649).then((() => () => t(649)))
                     },
                     o = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
@@ -35,15 +35,15 @@
         return g[e](t, t.exports, m), t.exports
     }
     m.m = g, m.c = b, m.d = (e, r) => {
         for (var t in r) m.o(r, t) && !m.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
-    }, m.f = {}, m.e = e => Promise.all(Object.keys(m.f).reduce(((r, t) => (m.f[t](e, r), r)), [])), m.u = e => e + ".5fbedda80fda1f1c26e7.js?v=5fbedda80fda1f1c26e7", m.g = function() {
+    }, m.f = {}, m.e = e => Promise.all(Object.keys(m.f).reduce(((r, t) => (m.f[t](e, r), r)), [])), m.u = e => e + ".d990bd40ed4bd0441591.js?v=d990bd40ed4bd0441591", m.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
     }(), m.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "catppuccin_jupyterlab:", m.l = (t, n, o, a) => {
@@ -195,18 +195,18 @@
         return a(n, o) || f(l(e, t, o, n)), s(e[t][o])
     }, f = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
     }, s = e => (e.loaded = 1, e.get()), c = (e => function(r, t, n, o) {
         var a = m.I(r);
         return a && a.then ? a.then(e.bind(e, r, m.S[r], t, n, o)) : e(r, m.S[r], t, n)
     })(((e, r, t, n) => (i(e, t), p(r, 0, t, n)))), d = {}, h = {
-        609: () => c("default", "@jupyterlab/apputils", [1, 4, 1, 5]),
-        426: () => c("default", "@jupyterlab/settingregistry", [1, 4, 0, 5])
+        464: () => c("default", "@jupyterlab/apputils", [1, 4, 2, 6]),
+        99: () => c("default", "@jupyterlab/settingregistry", [1, 4, 1, 6])
     }, v = {
-        649: [609, 426]
+        649: [464, 99]
     }, m.f.consumes = (e, r) => {
         m.o(v, e) && v[e].forEach((e => {
             if (m.o(d, e)) return r.push(d[e]);
             var t = r => {
                     d[e] = 0, m.m[e] = t => {
                         delete m.c[e], t.exports = r()
                     }
@@ -253,10 +253,10 @@
                     u && u(m)
                 }
                 for (r && r(t); l < a.length; l++) o = a[l], m.o(e, o) && e[o] && e[o][0](), e[o] = 0
             },
             t = self.webpackChunkcatppuccin_jupyterlab = self.webpackChunkcatppuccin_jupyterlab || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
     })();
-    var y = m(900);
+    var y = m(144);
     (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB).catppuccin_jupyterlab = y
 })();
```

### Comparing `catppuccin_jupyterlab-0.2.0/catppuccin_jupyterlab/labextension/themes/catppuccin_jupyterlab/index.css` & `catppuccin_jupyterlab-0.2.1/catppuccin_jupyterlab/labextension/themes/catppuccin_jupyterlab/index.css`

 * *Files identical despite different names*

### Comparing `catppuccin_jupyterlab-0.2.0/examples/markdown.md` & `catppuccin_jupyterlab-0.2.1/examples/markdown.md`

 * *Files identical despite different names*

### Comparing `catppuccin_jupyterlab-0.2.0/examples/python.ipynb` & `catppuccin_jupyterlab-0.2.1/examples/python.ipynb`

 * *Files identical despite different names*

### Comparing `catppuccin_jupyterlab-0.2.0/examples/r.ipynb` & `catppuccin_jupyterlab-0.2.1/examples/r.ipynb`

 * *Files identical despite different names*

### Comparing `catppuccin_jupyterlab-0.2.0/schema/plugin.json` & `catppuccin_jupyterlab-0.2.1/schema/plugin.json`

 * *Files identical despite different names*

### Comparing `catppuccin_jupyterlab-0.2.0/src/index.ts` & `catppuccin_jupyterlab-0.2.1/src/index.ts`

 * *Files identical despite different names*

### Comparing `catppuccin_jupyterlab-0.2.0/src/palettes.ts` & `catppuccin_jupyterlab-0.2.1/src/palettes.ts`

 * *Files identical despite different names*

### Comparing `catppuccin_jupyterlab-0.2.0/style/variables.css` & `catppuccin_jupyterlab-0.2.1/style/variables.css`

 * *Files identical despite different names*

### Comparing `catppuccin_jupyterlab-0.2.0/.gitignore` & `catppuccin_jupyterlab-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `catppuccin_jupyterlab-0.2.0/LICENSE` & `catppuccin_jupyterlab-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `catppuccin_jupyterlab-0.2.0/README.md` & `catppuccin_jupyterlab-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `catppuccin_jupyterlab-0.2.0/pyproject.toml` & `catppuccin_jupyterlab-0.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `catppuccin_jupyterlab-0.2.0/PKG-INFO` & `catppuccin_jupyterlab-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: catppuccin-jupyterlab
-Version: 0.2.0
+Version: 0.2.1
+Dynamic: Keywords
 Summary: 📊 Soothing pastel theme for JupyterLab.
 Project-URL: Homepage, https://github.com/catppuccin/jupyterlab
 Project-URL: Bug Tracker, https://github.com/catppuccin/jupyterlab/issues
 Project-URL: Repository, https://github.com/catppuccin/jupyterlab.git
 Author-email: Gabriel Magno <gabrielmagno1@gmail.com>
 License: MIT License
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
-Metadata-Version: 2.1 Name: catppuccin-jupyterlab Version: 0.2.0 Summary: ð
-Soothing pastel theme for JupyterLab. Project-URL: Homepage, https://
-github.com/catppuccin/jupyterlab Project-URL: Bug Tracker, https://github.com/
-catppuccin/jupyterlab/issues Project-URL: Repository, https://github.com/
-catppuccin/jupyterlab.git Author-email: Gabriel Magno
+Metadata-Version: 2.3 Name: catppuccin-jupyterlab Version: 0.2.1 Dynamic:
+Keywords Summary: ð Soothing pastel theme for JupyterLab. Project-URL:
+Homepage, https://github.com/catppuccin/jupyterlab Project-URL: Bug Tracker,
+https://github.com/catppuccin/jupyterlab/issues Project-URL: Repository, https:
+//github.com/catppuccin/jupyterlab.git Author-email: Gabriel Magno
 gmail.com> License: MIT License Copyright (c) 2021 Catppuccin Permission is
 hereby granted, free of charge, to any person obtaining a copy of this software
 and associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
 modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
 subject to the following conditions: The above copyright notice and this
```

