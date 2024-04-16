# Comparing `tmp/cmind-2.0.4.tar.gz` & `tmp/cmind-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmind-2.0.4.tar", last modified: Wed Apr 10 13:41:29 2024, max compression
+gzip compressed data, was "cmind-2.1.0.tar", last modified: Tue Apr 16 14:54:06 2024, max compression
```

## Comparing `cmind-2.0.4.tar` & `cmind-2.1.0.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2024-04-10 13:41:29.702234 cmind-2.0.4/
--rw-r--r--   0 fursin    (1000) fursin    (1000)    10174 2024-04-10 13:40:53.000000 cmind-2.0.4/LICENSE.CK.md
--rw-r--r--   0 fursin    (1000) fursin    (1000)    10174 2024-04-10 13:40:53.000000 cmind-2.0.4/LICENSE.md
--rw-r--r--   0 fursin    (1000) fursin    (1000)    10383 2024-04-10 13:41:29.702234 cmind-2.0.4/PKG-INFO
--rw-r--r--   0 fursin    (1000) fursin    (1000)     9948 2024-04-10 13:40:53.000000 cmind-2.0.4/README.md
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2024-04-10 13:41:29.692234 cmind-2.0.4/cmind/
--rw-r--r--   0 fursin    (1000) fursin    (1000)      136 2024-04-10 13:40:53.000000 cmind-2.0.4/cmind/__init__.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)       35 2024-04-10 13:40:53.000000 cmind-2.0.4/cmind/__main__.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)     4888 2024-04-10 13:40:53.000000 cmind-2.0.4/cmind/artifact.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)    47918 2024-04-10 13:40:53.000000 cmind-2.0.4/cmind/automation.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)     6437 2024-04-10 13:40:53.000000 cmind-2.0.4/cmind/cli.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)     3285 2024-04-10 13:40:53.000000 cmind-2.0.4/cmind/config.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)    28106 2024-04-10 13:40:53.000000 cmind-2.0.4/cmind/core.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)     9511 2024-04-10 13:40:53.000000 cmind-2.0.4/cmind/index.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)     2046 2024-04-10 13:40:53.000000 cmind-2.0.4/cmind/net.py
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2024-04-10 13:41:29.692234 cmind-2.0.4/cmind/repo/
--rw-r--r--   0 fursin    (1000) fursin    (1000)      491 2024-04-10 13:40:53.000000 cmind-2.0.4/cmind/repo/README.md
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2024-04-10 13:41:29.692234 cmind-2.0.4/cmind/repo/automation/
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2024-04-10 13:41:29.692234 cmind-2.0.4/cmind/repo/automation/automation/
--rw-r--r--   0 fursin    (1000) fursin    (1000)     2647 2024-04-10 13:40:53.000000 cmind-2.0.4/cmind/repo/automation/automation/README.md
--rw-r--r--   0 fursin    (1000) fursin    (1000)      289 2024-04-10 13:40:53.000000 cmind-2.0.4/cmind/repo/automation/automation/_cm.json
--rw-r--r--   0 fursin    (1000) fursin    (1000)     3799 2024-04-10 13:40:53.000000 cmind-2.0.4/cmind/repo/automation/automation/module.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)     1518 2024-04-10 13:40:53.000000 cmind-2.0.4/cmind/repo/automation/automation/module_dummy.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)     8772 2024-04-10 13:40:53.000000 cmind-2.0.4/cmind/repo/automation/automation/module_misc.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)      310 2024-04-10 13:40:53.000000 cmind-2.0.4/cmind/repo/automation/automation/template_list_of_automations.md
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2024-04-10 13:41:29.692234 cmind-2.0.4/cmind/repo/automation/ck/
--rw-r--r--   0 fursin    (1000) fursin    (1000)      984 2024-04-10 13:40:53.000000 cmind-2.0.4/cmind/repo/automation/ck/README.md
--rw-r--r--   0 fursin    (1000) fursin    (1000)      325 2024-04-10 13:40:53.000000 cmind-2.0.4/cmind/repo/automation/ck/_cm.json
--rw-r--r--   0 fursin    (1000) fursin    (1000)     1015 2024-04-10 13:40:53.000000 cmind-2.0.4/cmind/repo/automation/ck/module.py
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2024-04-10 13:41:29.692234 cmind-2.0.4/cmind/repo/automation/core/
--rw-r--r--   0 fursin    (1000) fursin    (1000)      996 2024-04-10 13:40:53.000000 cmind-2.0.4/cmind/repo/automation/core/README.md
--rw-r--r--   0 fursin    (1000) fursin    (1000)      302 2024-04-10 13:40:53.000000 cmind-2.0.4/cmind/repo/automation/core/_cm.json
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2024-04-10 13:41:29.692234 cmind-2.0.4/cmind/repo/automation/core/cm_60cb625a46b38610/
--rw-r--r--   0 fursin    (1000) fursin    (1000)        0 2024-04-10 13:40:53.000000 cmind-2.0.4/cmind/repo/automation/core/cm_60cb625a46b38610/__init__.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)      220 2024-04-10 13:40:53.000000 cmind-2.0.4/cmind/repo/automation/core/cm_60cb625a46b38610/misc.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)     1008 2024-04-10 13:40:53.000000 cmind-2.0.4/cmind/repo/automation/core/module.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)      220 2024-04-10 13:40:53.000000 cmind-2.0.4/cmind/repo/automation/core/module_misc.py
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2024-04-10 13:41:29.702234 cmind-2.0.4/cmind/repo/automation/repo/
--rw-r--r--   0 fursin    (1000) fursin    (1000)      388 2024-04-10 13:40:53.000000 cmind-2.0.4/cmind/repo/automation/repo/README-extra.md
--rw-r--r--   0 fursin    (1000) fursin    (1000)    10273 2024-04-10 13:40:53.000000 cmind-2.0.4/cmind/repo/automation/repo/README.md
--rw-r--r--   0 fursin    (1000) fursin    (1000)      433 2024-04-10 13:40:53.000000 cmind-2.0.4/cmind/repo/automation/repo/_cm.json
--rw-r--r--   0 fursin    (1000) fursin    (1000)    37831 2024-04-10 13:40:53.000000 cmind-2.0.4/cmind/repo/automation/repo/module.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)       71 2024-04-10 13:40:53.000000 cmind-2.0.4/cmind/repo/cmr.yaml
--rw-r--r--   0 fursin    (1000) fursin    (1000)     2008 2024-04-10 13:40:53.000000 cmind-2.0.4/cmind/repo.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)    22835 2024-04-10 13:40:53.000000 cmind-2.0.4/cmind/repos.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)    42753 2024-04-10 13:40:53.000000 cmind-2.0.4/cmind/utils.py
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2024-04-10 13:41:29.692234 cmind-2.0.4/cmind.egg-info/
--rw-r--r--   0 fursin    (1000) fursin    (1000)    10383 2024-04-10 13:41:29.000000 cmind-2.0.4/cmind.egg-info/PKG-INFO
--rw-r--r--   0 fursin    (1000) fursin    (1000)     1290 2024-04-10 13:41:29.000000 cmind-2.0.4/cmind.egg-info/SOURCES.txt
--rw-r--r--   0 fursin    (1000) fursin    (1000)        1 2024-04-10 13:41:29.000000 cmind-2.0.4/cmind.egg-info/dependency_links.txt
--rw-r--r--   0 fursin    (1000) fursin    (1000)      176 2024-04-10 13:41:29.000000 cmind-2.0.4/cmind.egg-info/entry_points.txt
--rw-r--r--   0 fursin    (1000) fursin    (1000)        1 2024-04-10 13:41:29.000000 cmind-2.0.4/cmind.egg-info/not-zip-safe
--rw-r--r--   0 fursin    (1000) fursin    (1000)       16 2024-04-10 13:41:29.000000 cmind-2.0.4/cmind.egg-info/requires.txt
--rw-r--r--   0 fursin    (1000) fursin    (1000)        6 2024-04-10 13:41:29.000000 cmind-2.0.4/cmind.egg-info/top_level.txt
--rw-r--r--   0 fursin    (1000) fursin    (1000)       38 2024-04-10 13:41:29.702234 cmind-2.0.4/setup.cfg
--rw-r--r--   0 fursin    (1000) fursin    (1000)     2898 2024-04-10 13:40:53.000000 cmind-2.0.4/setup.py
+drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2024-04-16 14:54:06.513303 cmind-2.1.0/
+-rw-r--r--   0 fursin    (1000) fursin    (1000)    10174 2024-04-16 14:53:52.000000 cmind-2.1.0/LICENSE.CK.md
+-rw-r--r--   0 fursin    (1000) fursin    (1000)    10174 2024-04-16 14:53:52.000000 cmind-2.1.0/LICENSE.md
+-rw-r--r--   0 fursin    (1000) fursin    (1000)    10413 2024-04-16 14:54:06.513303 cmind-2.1.0/PKG-INFO
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     9978 2024-04-16 14:53:52.000000 cmind-2.1.0/README.md
+drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2024-04-16 14:54:06.513303 cmind-2.1.0/cmind/
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      136 2024-04-16 14:53:52.000000 cmind-2.1.0/cmind/__init__.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)       35 2024-04-16 14:53:52.000000 cmind-2.1.0/cmind/__main__.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     4888 2024-04-16 14:53:52.000000 cmind-2.1.0/cmind/artifact.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)    47918 2024-04-16 14:53:52.000000 cmind-2.1.0/cmind/automation.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     6437 2024-04-16 14:53:52.000000 cmind-2.1.0/cmind/cli.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     3285 2024-04-16 14:53:52.000000 cmind-2.1.0/cmind/config.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)    28106 2024-04-16 14:53:52.000000 cmind-2.1.0/cmind/core.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     9511 2024-04-16 14:53:52.000000 cmind-2.1.0/cmind/index.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     2046 2024-04-16 14:53:52.000000 cmind-2.1.0/cmind/net.py
+drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2024-04-16 14:54:06.513303 cmind-2.1.0/cmind/repo/
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      491 2024-04-16 14:53:52.000000 cmind-2.1.0/cmind/repo/README.md
+drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2024-04-16 14:54:06.513303 cmind-2.1.0/cmind/repo/automation/
+drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2024-04-16 14:54:06.513303 cmind-2.1.0/cmind/repo/automation/automation/
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     2647 2024-04-16 14:53:52.000000 cmind-2.1.0/cmind/repo/automation/automation/README.md
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      289 2024-04-16 14:53:52.000000 cmind-2.1.0/cmind/repo/automation/automation/_cm.json
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     3958 2024-04-16 14:53:52.000000 cmind-2.1.0/cmind/repo/automation/automation/module.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     1518 2024-04-16 14:53:52.000000 cmind-2.1.0/cmind/repo/automation/automation/module_dummy.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     8772 2024-04-16 14:53:52.000000 cmind-2.1.0/cmind/repo/automation/automation/module_misc.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      310 2024-04-16 14:53:52.000000 cmind-2.1.0/cmind/repo/automation/automation/template_list_of_automations.md
+drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2024-04-16 14:54:06.513303 cmind-2.1.0/cmind/repo/automation/ckx/
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      984 2024-04-16 14:53:52.000000 cmind-2.1.0/cmind/repo/automation/ckx/README.md
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      327 2024-04-16 14:53:52.000000 cmind-2.1.0/cmind/repo/automation/ckx/_cm.json
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     1015 2024-04-16 14:53:52.000000 cmind-2.1.0/cmind/repo/automation/ckx/module.py
+drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2024-04-16 14:54:06.513303 cmind-2.1.0/cmind/repo/automation/core/
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      996 2024-04-16 14:53:52.000000 cmind-2.1.0/cmind/repo/automation/core/README.md
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      302 2024-04-16 14:53:52.000000 cmind-2.1.0/cmind/repo/automation/core/_cm.json
+drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2024-04-16 14:54:06.513303 cmind-2.1.0/cmind/repo/automation/core/cm_60cb625a46b38610/
+-rw-r--r--   0 fursin    (1000) fursin    (1000)        0 2024-04-16 14:53:52.000000 cmind-2.1.0/cmind/repo/automation/core/cm_60cb625a46b38610/__init__.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      220 2024-04-16 14:53:52.000000 cmind-2.1.0/cmind/repo/automation/core/cm_60cb625a46b38610/misc.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     1008 2024-04-16 14:53:52.000000 cmind-2.1.0/cmind/repo/automation/core/module.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      220 2024-04-16 14:53:52.000000 cmind-2.1.0/cmind/repo/automation/core/module_misc.py
+drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2024-04-16 14:54:06.513303 cmind-2.1.0/cmind/repo/automation/repo/
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      388 2024-04-16 14:53:52.000000 cmind-2.1.0/cmind/repo/automation/repo/README-extra.md
+-rw-r--r--   0 fursin    (1000) fursin    (1000)    10273 2024-04-16 14:53:52.000000 cmind-2.1.0/cmind/repo/automation/repo/README.md
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      433 2024-04-16 14:53:52.000000 cmind-2.1.0/cmind/repo/automation/repo/_cm.json
+-rw-r--r--   0 fursin    (1000) fursin    (1000)    37831 2024-04-16 14:53:52.000000 cmind-2.1.0/cmind/repo/automation/repo/module.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)       71 2024-04-16 14:53:52.000000 cmind-2.1.0/cmind/repo/cmr.yaml
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     2008 2024-04-16 14:53:52.000000 cmind-2.1.0/cmind/repo.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)    22835 2024-04-16 14:53:52.000000 cmind-2.1.0/cmind/repos.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)    42753 2024-04-16 14:53:52.000000 cmind-2.1.0/cmind/utils.py
+drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2024-04-16 14:54:06.513303 cmind-2.1.0/cmind.egg-info/
+-rw-r--r--   0 fursin    (1000) fursin    (1000)    10413 2024-04-16 14:54:06.000000 cmind-2.1.0/cmind.egg-info/PKG-INFO
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     1293 2024-04-16 14:54:06.000000 cmind-2.1.0/cmind.egg-info/SOURCES.txt
+-rw-r--r--   0 fursin    (1000) fursin    (1000)        1 2024-04-16 14:54:06.000000 cmind-2.1.0/cmind.egg-info/dependency_links.txt
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      176 2024-04-16 14:54:06.000000 cmind-2.1.0/cmind.egg-info/entry_points.txt
+-rw-r--r--   0 fursin    (1000) fursin    (1000)        1 2024-04-16 14:54:06.000000 cmind-2.1.0/cmind.egg-info/not-zip-safe
+-rw-r--r--   0 fursin    (1000) fursin    (1000)       16 2024-04-16 14:54:06.000000 cmind-2.1.0/cmind.egg-info/requires.txt
+-rw-r--r--   0 fursin    (1000) fursin    (1000)        6 2024-04-16 14:54:06.000000 cmind-2.1.0/cmind.egg-info/top_level.txt
+-rw-r--r--   0 fursin    (1000) fursin    (1000)       38 2024-04-16 14:54:06.513303 cmind-2.1.0/setup.cfg
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     2898 2024-04-16 14:53:52.000000 cmind-2.1.0/setup.py
```

### Comparing `cmind-2.0.4/LICENSE.CK.md` & `cmind-2.1.0/LICENSE.CK.md`

 * *Files identical despite different names*

### Comparing `cmind-2.0.4/LICENSE.md` & `cmind-2.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `cmind-2.0.4/PKG-INFO` & `cmind-2.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmind
-Version: 2.0.4
+Version: 2.1.0
 Summary: cmind
 Home-page: https://github.com/mlcommons/ck
 Author: Grigori Fursin
 Author-email: Grigori.Fursin@cTuning.org
 License: Apache 2.0
 Keywords: collective mind,cmind,ck3,cdatabase,cmeta,automation,portability,reusability,productivity,meta,JSON,YAML,python,api,cli
 Platform: UNKNOWN
@@ -60,18 +60,18 @@
 For example, you should be able to run the MLPerf inference benchmark on Linux, Windows and MacOS
 using a few CM commands:
 
 ```bash
 
 pip install cmind -U
 
-cm pull repo mlcommons@ck
+cm pull repo mlcommons@cm4mlops
 
-cm checkout repo mlcommons@ck --branch=dev
-cm checkout repo mlcommons@ck --branch=master
+cm checkout repo mlcommons@cm4mlops --branch=dev
+cm checkout repo mlcommons@cm4mlops --branch=master
 
 cm rm cache -f
 
 cm run script "get mlcommons inference src"
 
 cm run script "get generic-python-lib _onnxruntime" --version=1.17.1
 
@@ -145,15 +145,15 @@
 
 See more examples of CM scripts and workflows to download Stable Diffusion, GPT-J and LLAMA2 models, process datasets, install tools and compose AI applications:
 
 
 ```bash
 pip install cmind -U
 
-cm pull repo mlcommons@ck
+cm pull repo mlcommons@cm4mlops
 
 cm run script "python app image-classification onnx"
 cmr "python app image-classification onnx"
 
 cmr "download file _wget" --url=https://cKnowledge.org/ai/data/computer_mouse.jpg --verify=no --env.CM_DOWNLOAD_CHECKSUM=45ae5c940233892c2f860efdf0b66e7e
 cmr "python app image-classification onnx" --input=computer_mouse.jpg
 cmr "python app image-classification onnx" --input=computer_mouse.jpg --debug
@@ -193,15 +193,15 @@
 cm find script "run common mlperf inference"
 
 cmr "get generic-python-lib _package.torch" --version=2.1.2
 cmr "get generic-python-lib _package.torchvision" --version=0.16.2
 cmr "python app image-classification torch" --input=computer_mouse.jpg
 
 
-cm rm repo mlcommons@ck
+cm rm repo mlcommons@cm4mlops
 cm pull repo --url=https://zenodo.org/records/10787459/files/cm-mlops-repo-20240306.zip
 
 cmr "install llvm prebuilt" --version=17.0.6
 cmr "app image corner-detection"
 
 cm run experiment --tags=tuning,experiment,batch_size -- echo --batch_size={{VAR1{range(1,8)}}}
 cm replay experiment --tags=tuning,experiment,batch_size
```

### Comparing `cmind-2.0.4/README.md` & `cmind-2.1.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -46,18 +46,18 @@
 For example, you should be able to run the MLPerf inference benchmark on Linux, Windows and MacOS
 using a few CM commands:
 
 ```bash
 
 pip install cmind -U
 
-cm pull repo mlcommons@ck
+cm pull repo mlcommons@cm4mlops
 
-cm checkout repo mlcommons@ck --branch=dev
-cm checkout repo mlcommons@ck --branch=master
+cm checkout repo mlcommons@cm4mlops --branch=dev
+cm checkout repo mlcommons@cm4mlops --branch=master
 
 cm rm cache -f
 
 cm run script "get mlcommons inference src"
 
 cm run script "get generic-python-lib _onnxruntime" --version=1.17.1
 
@@ -131,15 +131,15 @@
 
 See more examples of CM scripts and workflows to download Stable Diffusion, GPT-J and LLAMA2 models, process datasets, install tools and compose AI applications:
 
 
 ```bash
 pip install cmind -U
 
-cm pull repo mlcommons@ck
+cm pull repo mlcommons@cm4mlops
 
 cm run script "python app image-classification onnx"
 cmr "python app image-classification onnx"
 
 cmr "download file _wget" --url=https://cKnowledge.org/ai/data/computer_mouse.jpg --verify=no --env.CM_DOWNLOAD_CHECKSUM=45ae5c940233892c2f860efdf0b66e7e
 cmr "python app image-classification onnx" --input=computer_mouse.jpg
 cmr "python app image-classification onnx" --input=computer_mouse.jpg --debug
@@ -179,15 +179,15 @@
 cm find script "run common mlperf inference"
 
 cmr "get generic-python-lib _package.torch" --version=2.1.2
 cmr "get generic-python-lib _package.torchvision" --version=0.16.2
 cmr "python app image-classification torch" --input=computer_mouse.jpg
 
 
-cm rm repo mlcommons@ck
+cm rm repo mlcommons@cm4mlops
 cm pull repo --url=https://zenodo.org/records/10787459/files/cm-mlops-repo-20240306.zip
 
 cmr "install llvm prebuilt" --version=17.0.6
 cmr "app image corner-detection"
 
 cm run experiment --tags=tuning,experiment,batch_size -- echo --batch_size={{VAR1{range(1,8)}}}
 cm replay experiment --tags=tuning,experiment,batch_size
```

### Comparing `cmind-2.0.4/cmind/artifact.py` & `cmind-2.1.0/cmind/artifact.py`

 * *Files identical despite different names*

### Comparing `cmind-2.0.4/cmind/automation.py` & `cmind-2.1.0/cmind/automation.py`

 * *Files identical despite different names*

### Comparing `cmind-2.0.4/cmind/cli.py` & `cmind-2.1.0/cmind/cli.py`

 * *Files identical despite different names*

### Comparing `cmind-2.0.4/cmind/config.py` & `cmind-2.1.0/cmind/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -56,15 +56,15 @@
                        "rm":"delete",
                        "mv":"move",
                        "ren":"move",
                        "rename":"move",
                        "cp":"copy"
                      },
 
-                     "new_repo_requirements": "cmind >= 0.7.5\n",
+                     "new_repo_requirements": "cmind >= 2.0.4\n",
 
                      "cmind_automation":"automation",
 
                      "file_cmeta":"_cm",
 
                      "local_repo_name": "local",
                      "local_repo_meta": {
```

### Comparing `cmind-2.0.4/cmind/core.py` & `cmind-2.1.0/cmind/core.py`

 * *Files identical despite different names*

### Comparing `cmind-2.0.4/cmind/index.py` & `cmind-2.1.0/cmind/index.py`

 * *Files identical despite different names*

### Comparing `cmind-2.0.4/cmind/net.py` & `cmind-2.1.0/cmind/net.py`

 * *Files identical despite different names*

### Comparing `cmind-2.0.4/cmind/repo/automation/automation/README.md` & `cmind-2.1.0/cmind/repo/automation/automation/README.md`

 * *Files identical despite different names*

### Comparing `cmind-2.0.4/cmind/repo/automation/automation/module.py` & `cmind-2.1.0/cmind/repo/automation/automation/module.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,14 +77,18 @@
 
         i['meta']={'automation_alias':self.meta['alias'],
                    'automation_uid':self.meta['uid'],
                    'tags':tags_list}
 
         if 'tags' in i: del(i['tags'])
 
+        automation = i['automation']
+        if automation!='.' and ',' not in automation: 
+            i['automation'] = automation + ',' + self.meta['uid']
+
         r_obj=self.cmind.access(i)
         if r_obj['return']>0: return r_obj
 
         new_automation_path = r_obj['path']
 
         if console:
             print ('Created automation in {}'.format(new_automation_path))
```

### Comparing `cmind-2.0.4/cmind/repo/automation/automation/module_dummy.py` & `cmind-2.1.0/cmind/repo/automation/automation/module_dummy.py`

 * *Files identical despite different names*

### Comparing `cmind-2.0.4/cmind/repo/automation/automation/module_misc.py` & `cmind-2.1.0/cmind/repo/automation/automation/module_misc.py`

 * *Files identical despite different names*

### Comparing `cmind-2.0.4/cmind/repo/automation/ck/README.md` & `cmind-2.1.0/cmind/repo/automation/ckx/README.md`

 * *Files identical despite different names*

### Comparing `cmind-2.0.4/cmind/repo/automation/ck/module.py` & `cmind-2.1.0/cmind/repo/automation/ckx/module.py`

 * *Files identical despite different names*

### Comparing `cmind-2.0.4/cmind/repo/automation/core/README.md` & `cmind-2.1.0/cmind/repo/automation/core/README.md`

 * *Files identical despite different names*

### Comparing `cmind-2.0.4/cmind/repo/automation/core/module.py` & `cmind-2.1.0/cmind/repo/automation/core/module.py`

 * *Files identical despite different names*

### Comparing `cmind-2.0.4/cmind/repo/automation/repo/README.md` & `cmind-2.1.0/cmind/repo/automation/repo/README.md`

 * *Files identical despite different names*

### Comparing `cmind-2.0.4/cmind/repo/automation/repo/module.py` & `cmind-2.1.0/cmind/repo/automation/repo/module.py`

 * *Files identical despite different names*

### Comparing `cmind-2.0.4/cmind/repo.py` & `cmind-2.1.0/cmind/repo.py`

 * *Files identical despite different names*

### Comparing `cmind-2.0.4/cmind/repos.py` & `cmind-2.1.0/cmind/repos.py`

 * *Files identical despite different names*

### Comparing `cmind-2.0.4/cmind/utils.py` & `cmind-2.1.0/cmind/utils.py`

 * *Files identical despite different names*

### Comparing `cmind-2.0.4/cmind.egg-info/PKG-INFO` & `cmind-2.1.0/cmind.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmind
-Version: 2.0.4
+Version: 2.1.0
 Summary: cmind
 Home-page: https://github.com/mlcommons/ck
 Author: Grigori Fursin
 Author-email: Grigori.Fursin@cTuning.org
 License: Apache 2.0
 Keywords: collective mind,cmind,ck3,cdatabase,cmeta,automation,portability,reusability,productivity,meta,JSON,YAML,python,api,cli
 Platform: UNKNOWN
@@ -60,18 +60,18 @@
 For example, you should be able to run the MLPerf inference benchmark on Linux, Windows and MacOS
 using a few CM commands:
 
 ```bash
 
 pip install cmind -U
 
-cm pull repo mlcommons@ck
+cm pull repo mlcommons@cm4mlops
 
-cm checkout repo mlcommons@ck --branch=dev
-cm checkout repo mlcommons@ck --branch=master
+cm checkout repo mlcommons@cm4mlops --branch=dev
+cm checkout repo mlcommons@cm4mlops --branch=master
 
 cm rm cache -f
 
 cm run script "get mlcommons inference src"
 
 cm run script "get generic-python-lib _onnxruntime" --version=1.17.1
 
@@ -145,15 +145,15 @@
 
 See more examples of CM scripts and workflows to download Stable Diffusion, GPT-J and LLAMA2 models, process datasets, install tools and compose AI applications:
 
 
 ```bash
 pip install cmind -U
 
-cm pull repo mlcommons@ck
+cm pull repo mlcommons@cm4mlops
 
 cm run script "python app image-classification onnx"
 cmr "python app image-classification onnx"
 
 cmr "download file _wget" --url=https://cKnowledge.org/ai/data/computer_mouse.jpg --verify=no --env.CM_DOWNLOAD_CHECKSUM=45ae5c940233892c2f860efdf0b66e7e
 cmr "python app image-classification onnx" --input=computer_mouse.jpg
 cmr "python app image-classification onnx" --input=computer_mouse.jpg --debug
@@ -193,15 +193,15 @@
 cm find script "run common mlperf inference"
 
 cmr "get generic-python-lib _package.torch" --version=2.1.2
 cmr "get generic-python-lib _package.torchvision" --version=0.16.2
 cmr "python app image-classification torch" --input=computer_mouse.jpg
 
 
-cm rm repo mlcommons@ck
+cm rm repo mlcommons@cm4mlops
 cm pull repo --url=https://zenodo.org/records/10787459/files/cm-mlops-repo-20240306.zip
 
 cmr "install llvm prebuilt" --version=17.0.6
 cmr "app image corner-detection"
 
 cm run experiment --tags=tuning,experiment,batch_size -- echo --batch_size={{VAR1{range(1,8)}}}
 cm replay experiment --tags=tuning,experiment,batch_size
```

### Comparing `cmind-2.0.4/cmind.egg-info/SOURCES.txt` & `cmind-2.1.0/cmind.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -25,17 +25,17 @@
 cmind/repo/cmr.yaml
 cmind/repo/automation/automation/README.md
 cmind/repo/automation/automation/_cm.json
 cmind/repo/automation/automation/module.py
 cmind/repo/automation/automation/module_dummy.py
 cmind/repo/automation/automation/module_misc.py
 cmind/repo/automation/automation/template_list_of_automations.md
-cmind/repo/automation/ck/README.md
-cmind/repo/automation/ck/_cm.json
-cmind/repo/automation/ck/module.py
+cmind/repo/automation/ckx/README.md
+cmind/repo/automation/ckx/_cm.json
+cmind/repo/automation/ckx/module.py
 cmind/repo/automation/core/README.md
 cmind/repo/automation/core/_cm.json
 cmind/repo/automation/core/module.py
 cmind/repo/automation/core/module_misc.py
 cmind/repo/automation/core/cm_60cb625a46b38610/__init__.py
 cmind/repo/automation/core/cm_60cb625a46b38610/misc.py
 cmind/repo/automation/repo/README-extra.md
```

### Comparing `cmind-2.0.4/setup.py` & `cmind-2.1.0/setup.py`

 * *Files identical despite different names*

