# Comparing `tmp/ipyniivue-1.1.0.tar.gz` & `tmp/ipyniivue-2.0.0.tar.gz`

## Comparing `ipyniivue-1.1.0.tar` & `ipyniivue-2.0.0.tar`

### file list

```diff
@@ -1,92 +1,11 @@
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 ipyniivue-1.1.0/.coveragerc
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 ipyniivue-1.1.0/.eslintignore
--rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 ipyniivue-1.1.0/.eslintrc.js
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 ipyniivue-1.1.0/.npmignore
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 ipyniivue-1.1.0/.prettierignore
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 ipyniivue-1.1.0/.prettierrc
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 ipyniivue-1.1.0/.readthedocs.yaml
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 ipyniivue-1.1.0/.yarnrc.yml
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 ipyniivue-1.1.0/MANIFEST.in
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 ipyniivue-1.1.0/babel.config.js
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 ipyniivue-1.1.0/codecov.yml
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 ipyniivue-1.1.0/dev-environment.yml
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 ipyniivue-1.1.0/environment.yml
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 ipyniivue-1.1.0/fileMock.js
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 ipyniivue-1.1.0/install.json
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 ipyniivue-1.1.0/ipyniivue.json
--rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 ipyniivue-1.1.0/jest.config.js
--rw-r--r--   0        0        0     3004 2020-02-02 00:00:00.000000 ipyniivue-1.1.0/package.json
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 ipyniivue-1.1.0/pytest.ini
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 ipyniivue-1.1.0/setup.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 ipyniivue-1.1.0/tsconfig.eslint.json
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 ipyniivue-1.1.0/tsconfig.json
--rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 ipyniivue-1.1.0/webpack.config.js
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 ipyniivue-1.1.0/docs/Makefile
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 ipyniivue-1.1.0/docs/README.md
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 ipyniivue-1.1.0/docs/environment.yml
--rw-r--r--   0        0        0   856986 2020-02-02 00:00:00.000000 ipyniivue-1.1.0/docs/example.png
--rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 ipyniivue-1.1.0/docs/make.bat
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 ipyniivue-1.1.0/docs/source/api.rst
--rw-r--r--   0        0        0     6185 2020-02-02 00:00:00.000000 ipyniivue-1.1.0/docs/source/conf.py
--rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 ipyniivue-1.1.0/docs/source/develop-install.rst
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 ipyniivue-1.1.0/docs/source/development-notes.rst
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 ipyniivue-1.1.0/docs/source/index.rst
--rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 ipyniivue-1.1.0/docs/source/installing.rst
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 ipyniivue-1.1.0/docs/source/introduction.rst
--rw-r--r--   0        0        0     1781 2020-02-02 00:00:00.000000 ipyniivue-1.1.0/docs/source/_static/embed-bundle.js.LICENSE.txt
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 ipyniivue-1.1.0/docs/source/_static/helper.js
--rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 ipyniivue-1.1.0/docs/source/development-notes/attribute-docstrings.rst
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 ipyniivue-1.1.0/docs/source/development-notes/cell-syncing.rst
--rw-r--r--   0        0        0     4528 2020-02-02 00:00:00.000000 ipyniivue-1.1.0/docs/source/development-notes/py-ts-messaging.rst
--rw-r--r--   0        0        0   243278 2020-02-02 00:00:00.000000 ipyniivue-1.1.0/docs/source/development-notes/traceback.png
--rw-r--r--   0        0        0   150323 2020-02-02 00:00:00.000000 ipyniivue-1.1.0/docs/source/development-notes/ws.png
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 ipyniivue-1.1.0/docs/source/examples/index.rst
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 ipyniivue-1.1.0/docs/source/examples/introduction.nblink
--rw-r--r--   0        0        0     7767 2020-02-02 00:00:00.000000 ipyniivue-1.1.0/examples/custom_code.ipynb
--rw-r--r--   0        0        0     4837 2020-02-02 00:00:00.000000 ipyniivue-1.1.0/examples/draw.ipynb
--rw-r--r--   0        0        0     5257 2020-02-02 00:00:00.000000 ipyniivue-1.1.0/examples/introduction.ipynb
--rw-r--r--   0        0        0     6646 2020-02-02 00:00:00.000000 ipyniivue-1.1.0/examples/tractography.ipynb
--rw-r--r--   0        0        0   707836 2020-02-02 00:00:00.000000 ipyniivue-1.1.0/examples/demo_images/CT_pitch.nii.gz
--rw-r--r--   0        0        0  4336029 2020-02-02 00:00:00.000000 ipyniivue-1.1.0/examples/demo_images/mni152.nii.gz
--rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 ipyniivue-1.1.0/ipyniivue/__init__.py
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 ipyniivue-1.1.0/ipyniivue/_frontend.py
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 ipyniivue-1.1.0/ipyniivue/_version.py
--rw-r--r--   0        0        0    46657 2020-02-02 00:00:00.000000 ipyniivue-1.1.0/ipyniivue/niivue.py
--rw-r--r--   0        0        0     2612 2020-02-02 00:00:00.000000 ipyniivue-1.1.0/ipyniivue/nvimage.py
--rw-r--r--   0        0        0     1273 2020-02-02 00:00:00.000000 ipyniivue-1.1.0/ipyniivue/nvmesh.py
--rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 ipyniivue-1.1.0/ipyniivue/traits.py
--rw-r--r--   0        0        0    21555 2020-02-02 00:00:00.000000 ipyniivue-1.1.0/ipyniivue/labextension/build_log.json
--rw-r--r--   0        0        0     3120 2020-02-02 00:00:00.000000 ipyniivue-1.1.0/ipyniivue/labextension/package.json
--rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 ipyniivue-1.1.0/ipyniivue/labextension/static/lib_index_js.6ffc91ccc740d1bae4db.js
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 ipyniivue-1.1.0/ipyniivue/labextension/static/lib_index_js.6ffc91ccc740d1bae4db.js.map
--rw-r--r--   0        0        0     2334 2020-02-02 00:00:00.000000 ipyniivue-1.1.0/ipyniivue/labextension/static/lib_plugin_js.fc0d5f43be1407591887.js
--rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 ipyniivue-1.1.0/ipyniivue/labextension/static/lib_plugin_js.fc0d5f43be1407591887.js.map
--rw-r--r--   0        0        0    21390 2020-02-02 00:00:00.000000 ipyniivue-1.1.0/ipyniivue/labextension/static/lib_widget_js.760766bd94c741330a5e.js
--rw-r--r--   0        0        0    27648 2020-02-02 00:00:00.000000 ipyniivue-1.1.0/ipyniivue/labextension/static/lib_widget_js.760766bd94c741330a5e.js.map
--rw-r--r--   0        0        0    27672 2020-02-02 00:00:00.000000 ipyniivue-1.1.0/ipyniivue/labextension/static/remoteEntry.8e28055fbc696747f07b.js
--rw-r--r--   0        0        0    26383 2020-02-02 00:00:00.000000 ipyniivue-1.1.0/ipyniivue/labextension/static/remoteEntry.8e28055fbc696747f07b.js.map
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 ipyniivue-1.1.0/ipyniivue/labextension/static/style.js
--rw-r--r--   0        0        0  3071880 2020-02-02 00:00:00.000000 ipyniivue-1.1.0/ipyniivue/labextension/static/vendors-node_modules_niivue_niivue_dist_niivue_es_js.45f525f821c155e098b9.js
--rw-r--r--   0        0        0  3527680 2020-02-02 00:00:00.000000 ipyniivue-1.1.0/ipyniivue/labextension/static/vendors-node_modules_niivue_niivue_dist_niivue_es_js.45f525f821c155e098b9.js.map
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 ipyniivue-1.1.0/ipyniivue/nbextension/extension.js
--rw-r--r--   0        0        0  1793025 2020-02-02 00:00:00.000000 ipyniivue-1.1.0/ipyniivue/nbextension/index.js
--rw-r--r--   0        0        0     1781 2020-02-02 00:00:00.000000 ipyniivue-1.1.0/ipyniivue/nbextension/index.js.LICENSE.txt
--rw-r--r--   0        0        0  4548084 2020-02-02 00:00:00.000000 ipyniivue-1.1.0/ipyniivue/nbextension/index.js.map
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ipyniivue-1.1.0/ipyniivue/tests/__init__.py
--rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 ipyniivue-1.1.0/ipyniivue/tests/conftest.py
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 ipyniivue-1.1.0/ipyniivue/tests/test_example.py
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 ipyniivue-1.1.0/ipyniivue/tests/test_nbextension_path.py
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 ipyniivue-1.1.0/src/extension.ts
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 ipyniivue-1.1.0/src/index.ts
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 ipyniivue-1.1.0/src/niivue.d.ts
--rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 ipyniivue-1.1.0/src/plugin.ts
--rw-r--r--   0        0        0     2745 2020-02-02 00:00:00.000000 ipyniivue-1.1.0/src/utils.ts
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 ipyniivue-1.1.0/src/version.ts
--rw-r--r--   0        0        0    11439 2020-02-02 00:00:00.000000 ipyniivue-1.1.0/src/widget.ts
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 ipyniivue-1.1.0/src/__tests__/index.spec.ts
--rw-r--r--   0        0        0     2909 2020-02-02 00:00:00.000000 ipyniivue-1.1.0/src/__tests__/utils.ts
--rw-r--r--   0        0        0     2061 2020-02-02 00:00:00.000000 ipyniivue-1.1.0/.gitignore
--rw-r--r--   0        0        0     1491 2020-02-02 00:00:00.000000 ipyniivue-1.1.0/LICENSE.txt
--rw-r--r--   0        0        0     1376 2020-02-02 00:00:00.000000 ipyniivue-1.1.0/README.md
--rw-r--r--   0        0        0     2760 2020-02-02 00:00:00.000000 ipyniivue-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     4513 2020-02-02 00:00:00.000000 ipyniivue-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 ipyniivue-2.0.0/src/ipyniivue/__init__.py
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 ipyniivue-2.0.0/src/ipyniivue/_constants.py
+-rw-r--r--   0        0        0    14423 2020-02-02 00:00:00.000000 ipyniivue-2.0.0/src/ipyniivue/_options_mixin.py
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 ipyniivue-2.0.0/src/ipyniivue/_utils.py
+-rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 ipyniivue-2.0.0/src/ipyniivue/_widget.py
+-rw-r--r--   0        0        0  2045073 2020-02-02 00:00:00.000000 ipyniivue-2.0.0/src/ipyniivue/static/widget.js
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 ipyniivue-2.0.0/.gitignore
+-rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 ipyniivue-2.0.0/LICENSE
+-rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 ipyniivue-2.0.0/README.md
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 ipyniivue-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 ipyniivue-2.0.0/PKG-INFO
```

### Comparing `ipyniivue-1.1.0/docs/source/_static/embed-bundle.js.LICENSE.txt` & `ipyniivue-2.0.0/LICENSE`

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,25 @@
-/*!
-  		 Copyright (c) 2007-2010, Jan de Vaan
-  		 All rights reserved.
+BSD 2-Clause License
 
-  		 Redistribution and use in source and binary forms, with or without
-  		 modification, are permitted provided that the following conditions are met:
+Copyright (c) 2024, Niivue
+All rights reserved.
 
-  		 * Redistributions of source code must retain the above copyright notice, this
-  		 list of conditions and the following disclaimer.
+Redistribution and use in source and binary forms, with or without
+modification, are permitted provided that the following conditions are met:
 
-  		 * Redistributions in binary form must reproduce the above copyright notice,
-  		 this list of conditions and the following disclaimer in the documentation
-  		 and/or other materials provided with the distribution.
-
-  		 * Neither the name of my employer, nor the names of its contributors may be
-  		 used to endorse or promote products derived from this software without
-  		 specific prior written permission.
-
-  		 THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
-  		 AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
-  		 IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-  		 DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT OWNER OR CONTRIBUTORS BE LIABLE FOR
-  		 ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
-  		 (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
-  		 LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON
-  		 ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
-  		 (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
-  		 SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
-  		 */
-
-/*! CharLS.js - v2.0.1 - 2016-06-08 | (c) 2016 Chris Hafey | https://github.com/chafey/charls */
-
-/*! image-JPEG2000 - v0.3.1 - 2015-08-26 | https://github.com/OHIF/image-JPEG2000 */
+1. Redistributions of source code must retain the above copyright notice, this
+   list of conditions and the following disclaimer.
+
+2. Redistributions in binary form must reproduce the above copyright notice,
+   this list of conditions and the following disclaimer in the documentation
+   and/or other materials provided with the distribution.
+
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
+FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
+DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
+SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
+CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
+OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

