# Comparing `tmp/gradio_demotest-0.0.1.tar.gz` & `tmp/gradio_demotest-0.0.2.tar.gz`

## Comparing `gradio_demotest-0.0.1.tar` & `gradio_demotest-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 gradio_demotest-0.0.1/backend/gradio_demotest/__init__.py
--rw-r--r--   0        0        0     4233 2020-02-02 00:00:00.000000 gradio_demotest-0.0.1/backend/gradio_demotest/demotest.py
--rw-r--r--   0        0        0    19533 2020-02-02 00:00:00.000000 gradio_demotest-0.0.1/backend/gradio_demotest/demotest.pyi
--rw-r--r--   0        0        0    55374 2020-02-02 00:00:00.000000 gradio_demotest-0.0.1/backend/gradio_demotest/templates/component/index.js
--rw-r--r--   0        0        0    13450 2020-02-02 00:00:00.000000 gradio_demotest-0.0.1/backend/gradio_demotest/templates/component/style.css
--rw-r--r--   0        0        0     2315 2020-02-02 00:00:00.000000 gradio_demotest-0.0.1/backend/gradio_demotest/templates/example/index.js
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 gradio_demotest-0.0.1/backend/gradio_demotest/templates/example/style.css
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gradio_demotest-0.0.1/demo/__init__.py
--rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 gradio_demotest-0.0.1/demo/app.py
--rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 gradio_demotest-0.0.1/demo/css.css
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gradio_demotest-0.0.1/demo/requirements.txt
--rw-r--r--   0        0        0     7252 2020-02-02 00:00:00.000000 gradio_demotest-0.0.1/demo/space.py
--rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 gradio_demotest-0.0.1/frontend/Example.svelte
--rw-r--r--   0        0        0     2946 2020-02-02 00:00:00.000000 gradio_demotest-0.0.1/frontend/Index.svelte
--rw-r--r--   0        0        0    33857 2020-02-02 00:00:00.000000 gradio_demotest-0.0.1/frontend/package-lock.json
--rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 gradio_demotest-0.0.1/frontend/package.json
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 gradio_demotest-0.0.1/.gitignore
--rw-r--r--   0        0        0     6593 2020-02-02 00:00:00.000000 gradio_demotest-0.0.1/README.md
--rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 gradio_demotest-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     7617 2020-02-02 00:00:00.000000 gradio_demotest-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 gradio_demotest-0.0.2/backend/gradio_demotest/__init__.py
+-rw-r--r--   0        0        0     4233 2020-02-02 00:00:00.000000 gradio_demotest-0.0.2/backend/gradio_demotest/demotest.py
+-rw-r--r--   0        0        0    19533 2020-02-02 00:00:00.000000 gradio_demotest-0.0.2/backend/gradio_demotest/demotest.pyi
+-rw-r--r--   0        0        0    55374 2020-02-02 00:00:00.000000 gradio_demotest-0.0.2/backend/gradio_demotest/templates/component/index.js
+-rw-r--r--   0        0        0    13450 2020-02-02 00:00:00.000000 gradio_demotest-0.0.2/backend/gradio_demotest/templates/component/style.css
+-rw-r--r--   0        0        0     2315 2020-02-02 00:00:00.000000 gradio_demotest-0.0.2/backend/gradio_demotest/templates/example/index.js
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 gradio_demotest-0.0.2/backend/gradio_demotest/templates/example/style.css
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gradio_demotest-0.0.2/demo/__init__.py
+-rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 gradio_demotest-0.0.2/demo/app.py
+-rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 gradio_demotest-0.0.2/demo/css.css
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 gradio_demotest-0.0.2/demo/requirements.txt
+-rw-r--r--   0        0        0     7296 2020-02-02 00:00:00.000000 gradio_demotest-0.0.2/demo/space.py
+-rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 gradio_demotest-0.0.2/frontend/Example.svelte
+-rw-r--r--   0        0        0     2946 2020-02-02 00:00:00.000000 gradio_demotest-0.0.2/frontend/Index.svelte
+-rw-r--r--   0        0        0    33857 2020-02-02 00:00:00.000000 gradio_demotest-0.0.2/frontend/package-lock.json
+-rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 gradio_demotest-0.0.2/frontend/package.json
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 gradio_demotest-0.0.2/.gitignore
+-rw-r--r--   0        0        0     6610 2020-02-02 00:00:00.000000 gradio_demotest-0.0.2/README.md
+-rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 gradio_demotest-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     7620 2020-02-02 00:00:00.000000 gradio_demotest-0.0.2/PKG-INFO
```

### Comparing `gradio_demotest-0.0.1/backend/gradio_demotest/demotest.py` & `gradio_demotest-0.0.2/backend/gradio_demotest/demotest.py`

 * *Files identical despite different names*

### Comparing `gradio_demotest-0.0.1/backend/gradio_demotest/demotest.pyi` & `gradio_demotest-0.0.2/backend/gradio_demotest/demotest.pyi`

 * *Files identical despite different names*

### Comparing `gradio_demotest-0.0.1/backend/gradio_demotest/templates/component/index.js` & `gradio_demotest-0.0.2/backend/gradio_demotest/templates/component/index.js`

 * *Files identical despite different names*

### Comparing `gradio_demotest-0.0.1/backend/gradio_demotest/templates/component/style.css` & `gradio_demotest-0.0.2/backend/gradio_demotest/templates/component/style.css`

 * *Files identical despite different names*

### Comparing `gradio_demotest-0.0.1/backend/gradio_demotest/templates/example/index.js` & `gradio_demotest-0.0.2/backend/gradio_demotest/templates/example/index.js`

 * *Files identical despite different names*

### Comparing `gradio_demotest-0.0.1/demo/css.css` & `gradio_demotest-0.0.2/demo/css.css`

 * *Files identical despite different names*

### Comparing `gradio_demotest-0.0.1/demo/space.py` & `gradio_demotest-0.0.2/demo/space.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,18 +17,18 @@
     ),
 ) as demo:
     gr.Markdown(
 """
 # `gradio_demotest`
 
 <div style="display: flex; gap: 7px;">
-<img alt="Static Badge" src="https://img.shields.io/badge/version%20-%200.0.1%20-%20orange">  
+<a href="https://pypi.org/project/gradio_demotest/" target="_blank"><img alt="PyPI - Version" src="https://img.shields.io/pypi/v/gradio_demotest"></a>  
 </div>
 
-test component for new flow
+foo component
 """, elem_classes=["md-custom"], header_links=True)
     app.render()
     gr.Markdown(
 """
 ## Installation
 
 ```bash
```

### Comparing `gradio_demotest-0.0.1/frontend/Example.svelte` & `gradio_demotest-0.0.2/frontend/Example.svelte`

 * *Files identical despite different names*

### Comparing `gradio_demotest-0.0.1/frontend/Index.svelte` & `gradio_demotest-0.0.2/frontend/Index.svelte`

 * *Files identical despite different names*

### Comparing `gradio_demotest-0.0.1/frontend/package-lock.json` & `gradio_demotest-0.0.2/frontend/package-lock.json`

 * *Files identical despite different names*

### Comparing `gradio_demotest-0.0.1/README.md` & `gradio_demotest-0.0.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 ---
-tags: [gradio-custom-component, SimpleTextbox, key, word, cool, flow, nyc]
+tags: [gradio-custom-component, SimpleTextbox, key, word, nyc, cool, test]
 title: gradio_demotest
-short_description: test component for new flow
+short_description: foo component
 colorFrom: blue
 colorTo: yellow
-sdk: docker
+sdk: gradio
 pinned: false
-header: mini
 app_file: space.py
 ---
 
 # `gradio_demotest`
-<img alt="Static Badge" src="https://img.shields.io/badge/version%20-%200.0.1%20-%20orange">  
+<a href="https://pypi.org/project/gradio_demotest/" target="_blank"><img alt="PyPI - Version" src="https://img.shields.io/pypi/v/gradio_demotest"></a>  
 
-test component for new flow
+foo component
 
 ## Installation
 
 ```bash
 pip install gradio_demotest
 ```
```

### Comparing `gradio_demotest-0.0.1/pyproject.toml` & `gradio_demotest-0.0.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -4,21 +4,21 @@
   "hatch-requirements-txt",
   "hatch-fancy-pypi-readme>=22.5.0",
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "gradio_demotest"
-version = "0.0.1"
-description = "test component for new flow"
+version = "0.0.2"
+description = "foo component"
 readme = "README.md"
 license = "apache-2.0"
 requires-python = ">=3.8"
 authors = [{ name = "YOUR NAME", email = "YOUREMAIL@domain.com" }]
-keywords = ["gradio-custom-component", "gradio-template-SimpleTextbox", "key", "word", "cool", "flow", "nyc"]
+keywords = ["gradio-custom-component", "gradio-template-SimpleTextbox", "key", "word", "nyc", "cool", "test"]
 # Add dependencies here
 dependencies = ["gradio>=4.0,<5.0"]
 classifiers = [
   'Development Status :: 3 - Alpha',
   'Operating System :: OS Independent',
   'Programming Language :: Python :: 3',
   'Programming Language :: Python :: 3 :: Only',
@@ -41,11 +41,11 @@
 # repository = "your github repository"
 # space = "your space url"
 
 [project.optional-dependencies]
 dev = ["build", "twine"]
 
 [tool.hatch.build]
-artifacts = ["/backend/gradio_demotest/templates", "*.pyi", "backend/gradio_demotest/templates"]
+artifacts = ["/backend/gradio_demotest/templates", "*.pyi", "backend/gradio_demotest/templates", "backend/gradio_demotest/templates"]
 
 [tool.hatch.build.targets.wheel]
 packages = ["/backend/gradio_demotest"]
```

### Comparing `gradio_demotest-0.0.1/PKG-INFO` & `gradio_demotest-0.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.3
 Name: gradio_demotest
-Version: 0.0.1
-Summary: test component for new flow
+Version: 0.0.2
+Summary: foo component
 Author-email: YOUR NAME <YOUREMAIL@domain.com>
 License-Expression: Apache-2.0
-Keywords: cool,flow,gradio-custom-component,gradio-template-SimpleTextbox,key,nyc,word
+Keywords: cool,gradio-custom-component,gradio-template-SimpleTextbox,key,nyc,test,word
 Classifier: Development Status :: 3 - Alpha
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -20,29 +20,28 @@
 Requires-Dist: gradio<5.0,>=4.0
 Provides-Extra: dev
 Requires-Dist: build; extra == 'dev'
 Requires-Dist: twine; extra == 'dev'
 Description-Content-Type: text/markdown
 
 ---
-tags: [gradio-custom-component, SimpleTextbox, key, word, cool, flow, nyc]
+tags: [gradio-custom-component, SimpleTextbox, key, word, nyc, cool, test]
 title: gradio_demotest
-short_description: test component for new flow
+short_description: foo component
 colorFrom: blue
 colorTo: yellow
-sdk: docker
+sdk: gradio
 pinned: false
-header: mini
 app_file: space.py
 ---
 
 # `gradio_demotest`
-<img alt="Static Badge" src="https://img.shields.io/badge/version%20-%200.0.1%20-%20orange">  
+<a href="https://pypi.org/project/gradio_demotest/" target="_blank"><img alt="PyPI - Version" src="https://img.shields.io/pypi/v/gradio_demotest"></a>  
 
-test component for new flow
+foo component
 
 ## Installation
 
 ```bash
 pip install gradio_demotest
 ```
```

