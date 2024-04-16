# Comparing `tmp/gradio_demotest-0.0.3.tar.gz` & `tmp/gradio_demotest-0.0.4.tar.gz`

## Comparing `gradio_demotest-0.0.3.tar` & `gradio_demotest-0.0.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 gradio_demotest-0.0.3/backend/gradio_demotest/__init__.py
--rw-r--r--   0        0        0     4233 2020-02-02 00:00:00.000000 gradio_demotest-0.0.3/backend/gradio_demotest/demotest.py
--rw-r--r--   0        0        0    19533 2020-02-02 00:00:00.000000 gradio_demotest-0.0.3/backend/gradio_demotest/demotest.pyi
--rw-r--r--   0        0        0    55374 2020-02-02 00:00:00.000000 gradio_demotest-0.0.3/backend/gradio_demotest/templates/component/index.js
--rw-r--r--   0        0        0    13450 2020-02-02 00:00:00.000000 gradio_demotest-0.0.3/backend/gradio_demotest/templates/component/style.css
--rw-r--r--   0        0        0     2315 2020-02-02 00:00:00.000000 gradio_demotest-0.0.3/backend/gradio_demotest/templates/example/index.js
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 gradio_demotest-0.0.3/backend/gradio_demotest/templates/example/style.css
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gradio_demotest-0.0.3/demo/__init__.py
--rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 gradio_demotest-0.0.3/demo/app.py
--rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 gradio_demotest-0.0.3/demo/css.css
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 gradio_demotest-0.0.3/demo/requirements.txt
--rw-r--r--   0        0        0     7296 2020-02-02 00:00:00.000000 gradio_demotest-0.0.3/demo/space.py
--rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 gradio_demotest-0.0.3/frontend/Example.svelte
--rw-r--r--   0        0        0     2946 2020-02-02 00:00:00.000000 gradio_demotest-0.0.3/frontend/Index.svelte
--rw-r--r--   0        0        0    33857 2020-02-02 00:00:00.000000 gradio_demotest-0.0.3/frontend/package-lock.json
--rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 gradio_demotest-0.0.3/frontend/package.json
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 gradio_demotest-0.0.3/.gitignore
--rw-r--r--   0        0        0     6610 2020-02-02 00:00:00.000000 gradio_demotest-0.0.3/README.md
--rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 gradio_demotest-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     7620 2020-02-02 00:00:00.000000 gradio_demotest-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 gradio_demotest-0.0.4/backend/gradio_demotest/__init__.py
+-rw-r--r--   0        0        0     4233 2020-02-02 00:00:00.000000 gradio_demotest-0.0.4/backend/gradio_demotest/demotest.py
+-rw-r--r--   0        0        0    19533 2020-02-02 00:00:00.000000 gradio_demotest-0.0.4/backend/gradio_demotest/demotest.pyi
+-rw-r--r--   0        0        0    55374 2020-02-02 00:00:00.000000 gradio_demotest-0.0.4/backend/gradio_demotest/templates/component/index.js
+-rw-r--r--   0        0        0    13450 2020-02-02 00:00:00.000000 gradio_demotest-0.0.4/backend/gradio_demotest/templates/component/style.css
+-rw-r--r--   0        0        0     2315 2020-02-02 00:00:00.000000 gradio_demotest-0.0.4/backend/gradio_demotest/templates/example/index.js
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 gradio_demotest-0.0.4/backend/gradio_demotest/templates/example/style.css
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gradio_demotest-0.0.4/demo/__init__.py
+-rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 gradio_demotest-0.0.4/demo/app.py
+-rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 gradio_demotest-0.0.4/demo/css.css
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 gradio_demotest-0.0.4/demo/requirements.txt
+-rw-r--r--   0        0        0     7296 2020-02-02 00:00:00.000000 gradio_demotest-0.0.4/demo/space.py
+-rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 gradio_demotest-0.0.4/frontend/Example.svelte
+-rw-r--r--   0        0        0     2946 2020-02-02 00:00:00.000000 gradio_demotest-0.0.4/frontend/Index.svelte
+-rw-r--r--   0        0        0    33857 2020-02-02 00:00:00.000000 gradio_demotest-0.0.4/frontend/package-lock.json
+-rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 gradio_demotest-0.0.4/frontend/package.json
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 gradio_demotest-0.0.4/.gitignore
+-rw-r--r--   0        0        0     6610 2020-02-02 00:00:00.000000 gradio_demotest-0.0.4/README.md
+-rw-r--r--   0        0        0     1921 2020-02-02 00:00:00.000000 gradio_demotest-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     7620 2020-02-02 00:00:00.000000 gradio_demotest-0.0.4/PKG-INFO
```

### Comparing `gradio_demotest-0.0.3/backend/gradio_demotest/demotest.py` & `gradio_demotest-0.0.4/backend/gradio_demotest/demotest.py`

 * *Files identical despite different names*

### Comparing `gradio_demotest-0.0.3/backend/gradio_demotest/demotest.pyi` & `gradio_demotest-0.0.4/backend/gradio_demotest/demotest.pyi`

 * *Files identical despite different names*

### Comparing `gradio_demotest-0.0.3/backend/gradio_demotest/templates/component/index.js` & `gradio_demotest-0.0.4/backend/gradio_demotest/templates/component/index.js`

 * *Files identical despite different names*

### Comparing `gradio_demotest-0.0.3/backend/gradio_demotest/templates/component/style.css` & `gradio_demotest-0.0.4/backend/gradio_demotest/templates/component/style.css`

 * *Files identical despite different names*

### Comparing `gradio_demotest-0.0.3/backend/gradio_demotest/templates/example/index.js` & `gradio_demotest-0.0.4/backend/gradio_demotest/templates/example/index.js`

 * *Files identical despite different names*

### Comparing `gradio_demotest-0.0.3/demo/css.css` & `gradio_demotest-0.0.4/demo/css.css`

 * *Files identical despite different names*

### Comparing `gradio_demotest-0.0.3/demo/space.py` & `gradio_demotest-0.0.4/demo/space.py`

 * *Files identical despite different names*

### Comparing `gradio_demotest-0.0.3/frontend/Example.svelte` & `gradio_demotest-0.0.4/frontend/Example.svelte`

 * *Files identical despite different names*

### Comparing `gradio_demotest-0.0.3/frontend/Index.svelte` & `gradio_demotest-0.0.4/frontend/Index.svelte`

 * *Files identical despite different names*

### Comparing `gradio_demotest-0.0.3/frontend/package-lock.json` & `gradio_demotest-0.0.4/frontend/package-lock.json`

 * *Files identical despite different names*

### Comparing `gradio_demotest-0.0.3/README.md` & `gradio_demotest-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `gradio_demotest-0.0.3/pyproject.toml` & `gradio_demotest-0.0.4/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   "hatch-requirements-txt",
   "hatch-fancy-pypi-readme>=22.5.0",
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "gradio_demotest"
-version = "0.0.3"
+version = "0.0.4"
 description = "foo component"
 readme = "README.md"
 license = "apache-2.0"
 requires-python = ">=3.8"
 authors = [{ name = "YOUR NAME", email = "YOUREMAIL@domain.com" }]
 keywords = ["gradio-custom-component", "gradio-template-SimpleTextbox", "key", "word", "nyc", "cool", "test"]
 # Add dependencies here
@@ -41,11 +41,11 @@
 # repository = "your github repository"
 # space = "your space url"
 
 [project.optional-dependencies]
 dev = ["build", "twine"]
 
 [tool.hatch.build]
-artifacts = ["/backend/gradio_demotest/templates", "*.pyi", "backend/gradio_demotest/templates", "backend/gradio_demotest/templates", "backend/gradio_demotest/templates", "backend/gradio_demotest/templates"]
+artifacts = ["/backend/gradio_demotest/templates", "*.pyi", "backend/gradio_demotest/templates", "backend/gradio_demotest/templates", "backend/gradio_demotest/templates", "backend/gradio_demotest/templates", "backend/gradio_demotest/templates"]
 
 [tool.hatch.build.targets.wheel]
 packages = ["/backend/gradio_demotest"]
```

### Comparing `gradio_demotest-0.0.3/PKG-INFO` & `gradio_demotest-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: gradio_demotest
-Version: 0.0.3
+Version: 0.0.4
 Summary: foo component
 Author-email: YOUR NAME <YOUREMAIL@domain.com>
 License-Expression: Apache-2.0
 Keywords: cool,gradio-custom-component,gradio-template-SimpleTextbox,key,nyc,test,word
 Classifier: Development Status :: 3 - Alpha
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

