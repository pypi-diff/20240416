# Comparing `tmp/wwpdb.apps.editormodule-0.18.tar.gz` & `tmp/wwpdb_apps_editormodule-0.18.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wwpdb.apps.editormodule-0.18.tar", last modified: Sat Apr 13 10:13:23 2024, max compression
+gzip compressed data, was "wwpdb_apps_editormodule-0.18.1.tar", last modified: Mon Apr 15 23:53:40 2024, max compression
```

## Comparing `wwpdb.apps.editormodule-0.18.tar` & `wwpdb_apps_editormodule-0.18.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-13 10:13:23.210903 wwpdb.apps.editormodule-0.18/
--rw-r--r--   0 vsts      (1001) docker     (127)      552 2024-04-13 10:12:23.000000 wwpdb.apps.editormodule-0.18/LICENSE
--rwxr-xr-x   0 vsts      (1001) docker     (127)      110 2024-04-13 10:12:23.000000 wwpdb.apps.editormodule-0.18/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (127)     1087 2024-04-13 10:13:23.210903 wwpdb.apps.editormodule-0.18/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)       51 2024-04-13 10:12:23.000000 wwpdb.apps.editormodule-0.18/README.md
--rw-r--r--   0 vsts      (1001) docker     (127)      108 2024-04-13 10:13:23.210903 wwpdb.apps.editormodule-0.18/setup.cfg
--rwxr-xr-x   0 vsts      (1001) docker     (127)     2209 2024-04-13 10:12:23.000000 wwpdb.apps.editormodule-0.18/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-13 10:13:23.206903 wwpdb.apps.editormodule-0.18/wwpdb/
--rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-04-13 10:12:23.000000 wwpdb.apps.editormodule-0.18/wwpdb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-13 10:13:23.206903 wwpdb.apps.editormodule-0.18/wwpdb/apps/
--rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-04-13 10:12:23.000000 wwpdb.apps.editormodule-0.18/wwpdb/apps/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-13 10:13:23.206903 wwpdb.apps.editormodule-0.18/wwpdb/apps/editormodule/
--rw-r--r--   0 vsts      (1001) docker     (127)      150 2024-04-13 10:12:23.000000 wwpdb.apps.editormodule-0.18/wwpdb/apps/editormodule/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-13 10:13:23.206903 wwpdb.apps.editormodule-0.18/wwpdb/apps/editormodule/config/
--rw-r--r--   0 vsts      (1001) docker     (127)      290 2024-04-13 10:12:23.000000 wwpdb.apps.editormodule-0.18/wwpdb/apps/editormodule/config/AccessConfigCifFiles.py
--rw-r--r--   0 vsts      (1001) docker     (127)      170 2024-04-13 10:12:23.000000 wwpdb.apps.editormodule-0.18/wwpdb/apps/editormodule/config/AccessTemplateFiles.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7864 2024-04-13 10:12:23.000000 wwpdb.apps.editormodule-0.18/wwpdb/apps/editormodule/config/EditorConfig.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-13 10:12:23.000000 wwpdb.apps.editormodule-0.18/wwpdb/apps/editormodule/config/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)   144958 2024-04-13 10:12:23.000000 wwpdb.apps.editormodule-0.18/wwpdb/apps/editormodule/config/pdbx_display_view_info.cif
--rw-r--r--   0 vsts      (1001) docker     (127)   216512 2024-04-13 10:12:23.000000 wwpdb.apps.editormodule-0.18/wwpdb/apps/editormodule/config/pdbx_display_view_info_master.cif
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-13 10:13:23.210903 wwpdb.apps.editormodule-0.18/wwpdb/apps/editormodule/depict/
--rwxr-xr-x   0 vsts      (1001) docker     (127)    52449 2024-04-13 10:12:23.000000 wwpdb.apps.editormodule-0.18/wwpdb/apps/editormodule/depict/EditorDepict.py
--rwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-13 10:12:23.000000 wwpdb.apps.editormodule-0.18/wwpdb/apps/editormodule/depict/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-13 10:13:23.210903 wwpdb.apps.editormodule-0.18/wwpdb/apps/editormodule/io/
--rw-r--r--   0 vsts      (1001) docker     (127)     4873 2024-04-13 10:12:23.000000 wwpdb.apps.editormodule-0.18/wwpdb/apps/editormodule/io/EditorDataImport.py
--rw-r--r--   0 vsts      (1001) docker     (127)   163711 2024-04-13 10:12:23.000000 wwpdb.apps.editormodule-0.18/wwpdb/apps/editormodule/io/PdbxDataIo.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8061 2024-04-13 10:12:23.000000 wwpdb.apps.editormodule-0.18/wwpdb/apps/editormodule/io/PdbxMasterViewDictionary.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1616 2024-04-13 10:12:23.000000 wwpdb.apps.editormodule-0.18/wwpdb/apps/editormodule/io/PdbxMasterViewDictionaryExec.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-13 10:12:23.000000 wwpdb.apps.editormodule-0.18/wwpdb/apps/editormodule/io/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-13 10:13:23.210903 wwpdb.apps.editormodule-0.18/wwpdb/apps/editormodule/templates/
--rw-r--r--   0 vsts      (1001) docker     (127)     6211 2024-04-13 10:12:23.000000 wwpdb.apps.editormodule-0.18/wwpdb/apps/editormodule/templates/common_tool_beta_testing_feedback.html
--rw-r--r--   0 vsts      (1001) docker     (127)      641 2024-04-13 10:12:23.000000 wwpdb.apps.editormodule-0.18/wwpdb/apps/editormodule/templates/editor_jmol_tmplt.html
--rw-r--r--   0 vsts      (1001) docker     (127)    13947 2024-04-13 10:12:23.000000 wwpdb.apps.editormodule-0.18/wwpdb/apps/editormodule/templates/editor_launch_tmplt.html
--rw-r--r--   0 vsts      (1001) docker     (127)    17945 2024-04-13 10:12:23.000000 wwpdb.apps.editormodule-0.18/wwpdb/apps/editormodule/templates/editor_launch_tmplt_config.html
--rw-r--r--   0 vsts      (1001) docker     (127)    15904 2024-04-13 10:12:23.000000 wwpdb.apps.editormodule-0.18/wwpdb/apps/editormodule/templates/editor_launch_tmplt_scrollnav.html
--rw-r--r--   0 vsts      (1001) docker     (127)     3502 2024-04-13 10:12:23.000000 wwpdb.apps.editormodule-0.18/wwpdb/apps/editormodule/templates/editor_prototyping.html
--rw-r--r--   0 vsts      (1001) docker     (127)     2470 2024-04-13 10:12:23.000000 wwpdb.apps.editormodule-0.18/wwpdb/apps/editormodule/templates/editor_ui_config_admin.html
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-13 10:13:23.210903 wwpdb.apps.editormodule-0.18/wwpdb/apps/editormodule/webapp/
--rw-r--r--   0 vsts      (1001) docker     (127)    79034 2024-04-13 10:12:23.000000 wwpdb.apps.editormodule-0.18/wwpdb/apps/editormodule/webapp/EditorWebApp.py
--rwxr-xr-x   0 vsts      (1001) docker     (127)    10750 2024-04-13 10:12:23.000000 wwpdb.apps.editormodule-0.18/wwpdb/apps/editormodule/webapp/WebRequest.py
--rwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-13 10:12:23.000000 wwpdb.apps.editormodule-0.18/wwpdb/apps/editormodule/webapp/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-13 10:13:23.210903 wwpdb.apps.editormodule-0.18/wwpdb.apps.editormodule.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)     1087 2024-04-13 10:13:23.000000 wwpdb.apps.editormodule-0.18/wwpdb.apps.editormodule.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     1637 2024-04-13 10:13:23.000000 wwpdb.apps.editormodule-0.18/wwpdb.apps.editormodule.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-13 10:13:23.000000 wwpdb.apps.editormodule-0.18/wwpdb.apps.editormodule.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-13 10:13:11.000000 wwpdb.apps.editormodule-0.18/wwpdb.apps.editormodule.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (127)      162 2024-04-13 10:13:23.000000 wwpdb.apps.editormodule-0.18/wwpdb.apps.editormodule.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        6 2024-04-13 10:13:23.000000 wwpdb.apps.editormodule-0.18/wwpdb.apps.editormodule.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-15 23:53:40.225452 wwpdb_apps_editormodule-0.18.1/
+-rw-r--r--   0 vsts      (1001) docker     (127)      552 2024-04-15 23:52:28.000000 wwpdb_apps_editormodule-0.18.1/LICENSE
+-rwxr-xr-x   0 vsts      (1001) docker     (127)      110 2024-04-15 23:52:28.000000 wwpdb_apps_editormodule-0.18.1/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (127)     1089 2024-04-15 23:53:40.225452 wwpdb_apps_editormodule-0.18.1/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)       51 2024-04-15 23:52:28.000000 wwpdb_apps_editormodule-0.18.1/README.md
+-rw-r--r--   0 vsts      (1001) docker     (127)      108 2024-04-15 23:53:40.225452 wwpdb_apps_editormodule-0.18.1/setup.cfg
+-rwxr-xr-x   0 vsts      (1001) docker     (127)     2209 2024-04-15 23:52:28.000000 wwpdb_apps_editormodule-0.18.1/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-15 23:53:40.217451 wwpdb_apps_editormodule-0.18.1/wwpdb/
+-rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-04-15 23:52:28.000000 wwpdb_apps_editormodule-0.18.1/wwpdb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-15 23:53:40.217451 wwpdb_apps_editormodule-0.18.1/wwpdb/apps/
+-rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-04-15 23:52:28.000000 wwpdb_apps_editormodule-0.18.1/wwpdb/apps/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-15 23:53:40.217451 wwpdb_apps_editormodule-0.18.1/wwpdb/apps/editormodule/
+-rw-r--r--   0 vsts      (1001) docker     (127)      152 2024-04-15 23:52:28.000000 wwpdb_apps_editormodule-0.18.1/wwpdb/apps/editormodule/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-15 23:53:40.217451 wwpdb_apps_editormodule-0.18.1/wwpdb/apps/editormodule/config/
+-rw-r--r--   0 vsts      (1001) docker     (127)      290 2024-04-15 23:52:28.000000 wwpdb_apps_editormodule-0.18.1/wwpdb/apps/editormodule/config/AccessConfigCifFiles.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      170 2024-04-15 23:52:28.000000 wwpdb_apps_editormodule-0.18.1/wwpdb/apps/editormodule/config/AccessTemplateFiles.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7864 2024-04-15 23:52:28.000000 wwpdb_apps_editormodule-0.18.1/wwpdb/apps/editormodule/config/EditorConfig.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-15 23:52:28.000000 wwpdb_apps_editormodule-0.18.1/wwpdb/apps/editormodule/config/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   144958 2024-04-15 23:52:28.000000 wwpdb_apps_editormodule-0.18.1/wwpdb/apps/editormodule/config/pdbx_display_view_info.cif
+-rw-r--r--   0 vsts      (1001) docker     (127)   216804 2024-04-15 23:52:28.000000 wwpdb_apps_editormodule-0.18.1/wwpdb/apps/editormodule/config/pdbx_display_view_info_master.cif
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-15 23:53:40.221451 wwpdb_apps_editormodule-0.18.1/wwpdb/apps/editormodule/depict/
+-rwxr-xr-x   0 vsts      (1001) docker     (127)    52449 2024-04-15 23:52:28.000000 wwpdb_apps_editormodule-0.18.1/wwpdb/apps/editormodule/depict/EditorDepict.py
+-rwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-15 23:52:28.000000 wwpdb_apps_editormodule-0.18.1/wwpdb/apps/editormodule/depict/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-15 23:53:40.221451 wwpdb_apps_editormodule-0.18.1/wwpdb/apps/editormodule/io/
+-rw-r--r--   0 vsts      (1001) docker     (127)     4873 2024-04-15 23:52:28.000000 wwpdb_apps_editormodule-0.18.1/wwpdb/apps/editormodule/io/EditorDataImport.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   163711 2024-04-15 23:52:28.000000 wwpdb_apps_editormodule-0.18.1/wwpdb/apps/editormodule/io/PdbxDataIo.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8061 2024-04-15 23:52:28.000000 wwpdb_apps_editormodule-0.18.1/wwpdb/apps/editormodule/io/PdbxMasterViewDictionary.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1616 2024-04-15 23:52:28.000000 wwpdb_apps_editormodule-0.18.1/wwpdb/apps/editormodule/io/PdbxMasterViewDictionaryExec.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-15 23:52:28.000000 wwpdb_apps_editormodule-0.18.1/wwpdb/apps/editormodule/io/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-15 23:53:40.221451 wwpdb_apps_editormodule-0.18.1/wwpdb/apps/editormodule/templates/
+-rw-r--r--   0 vsts      (1001) docker     (127)     6211 2024-04-15 23:52:28.000000 wwpdb_apps_editormodule-0.18.1/wwpdb/apps/editormodule/templates/common_tool_beta_testing_feedback.html
+-rw-r--r--   0 vsts      (1001) docker     (127)      641 2024-04-15 23:52:28.000000 wwpdb_apps_editormodule-0.18.1/wwpdb/apps/editormodule/templates/editor_jmol_tmplt.html
+-rw-r--r--   0 vsts      (1001) docker     (127)    13947 2024-04-15 23:52:28.000000 wwpdb_apps_editormodule-0.18.1/wwpdb/apps/editormodule/templates/editor_launch_tmplt.html
+-rw-r--r--   0 vsts      (1001) docker     (127)    17945 2024-04-15 23:52:28.000000 wwpdb_apps_editormodule-0.18.1/wwpdb/apps/editormodule/templates/editor_launch_tmplt_config.html
+-rw-r--r--   0 vsts      (1001) docker     (127)    15904 2024-04-15 23:52:28.000000 wwpdb_apps_editormodule-0.18.1/wwpdb/apps/editormodule/templates/editor_launch_tmplt_scrollnav.html
+-rw-r--r--   0 vsts      (1001) docker     (127)     3502 2024-04-15 23:52:28.000000 wwpdb_apps_editormodule-0.18.1/wwpdb/apps/editormodule/templates/editor_prototyping.html
+-rw-r--r--   0 vsts      (1001) docker     (127)     2470 2024-04-15 23:52:28.000000 wwpdb_apps_editormodule-0.18.1/wwpdb/apps/editormodule/templates/editor_ui_config_admin.html
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-15 23:53:40.221451 wwpdb_apps_editormodule-0.18.1/wwpdb/apps/editormodule/webapp/
+-rw-r--r--   0 vsts      (1001) docker     (127)    79034 2024-04-15 23:52:28.000000 wwpdb_apps_editormodule-0.18.1/wwpdb/apps/editormodule/webapp/EditorWebApp.py
+-rwxr-xr-x   0 vsts      (1001) docker     (127)    10750 2024-04-15 23:52:28.000000 wwpdb_apps_editormodule-0.18.1/wwpdb/apps/editormodule/webapp/WebRequest.py
+-rwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-15 23:52:28.000000 wwpdb_apps_editormodule-0.18.1/wwpdb/apps/editormodule/webapp/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-15 23:53:40.221451 wwpdb_apps_editormodule-0.18.1/wwpdb.apps.editormodule.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1089 2024-04-15 23:53:40.000000 wwpdb_apps_editormodule-0.18.1/wwpdb.apps.editormodule.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     1637 2024-04-15 23:53:40.000000 wwpdb_apps_editormodule-0.18.1/wwpdb.apps.editormodule.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-15 23:53:40.000000 wwpdb_apps_editormodule-0.18.1/wwpdb.apps.editormodule.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-15 23:53:25.000000 wwpdb_apps_editormodule-0.18.1/wwpdb.apps.editormodule.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (127)      162 2024-04-15 23:53:40.000000 wwpdb_apps_editormodule-0.18.1/wwpdb.apps.editormodule.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        6 2024-04-15 23:53:40.000000 wwpdb_apps_editormodule-0.18.1/wwpdb.apps.editormodule.egg-info/top_level.txt
```

### Comparing `wwpdb.apps.editormodule-0.18/LICENSE` & `wwpdb_apps_editormodule-0.18.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.editormodule-0.18/PKG-INFO` & `wwpdb_apps_editormodule-0.18.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwpdb.apps.editormodule
-Version: 0.18
+Version: 0.18.1
 Summary: wwPDB mmCIF form editor module
 Home-page: https://github.com/rcsb/py-wwpdb_apps_editormodule
 Author: Ezra Peisach
 Author-email: ezra.peisach@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `wwpdb.apps.editormodule-0.18/setup.py` & `wwpdb_apps_editormodule-0.18.1/setup.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.editormodule-0.18/wwpdb/apps/editormodule/config/EditorConfig.py` & `wwpdb_apps_editormodule-0.18.1/wwpdb/apps/editormodule/config/EditorConfig.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.editormodule-0.18/wwpdb/apps/editormodule/config/pdbx_display_view_info.cif` & `wwpdb_apps_editormodule-0.18.1/wwpdb/apps/editormodule/config/pdbx_display_view_info.cif`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.editormodule-0.18/wwpdb/apps/editormodule/config/pdbx_display_view_info_master.cif` & `wwpdb_apps_editormodule-0.18.1/wwpdb/apps/editormodule/config/pdbx_display_view_info_master.cif`

 * *Files 1% similar despite different names*

```diff
@@ -927,20 +927,22 @@
 struct_ncs_dom                        '_struct_ncs_dom.id'                                          id                                          N
 struct_ncs_dom                        '_struct_ncs_dom.details'                                     details                                     N
 struct_ncs_dom                        '_struct_ncs_dom.pdbx_ens_id'                                 pdbx_ens_id                                 N
 
 struct_ncs_dom_lim                    '_struct_ncs_dom_lim.dom_id'                                  dom_id                                      N
 struct_ncs_dom_lim                    '_struct_ncs_dom_lim.beg_auth_asym_id'                        beg_auth_asym_id                            N
 struct_ncs_dom_lim                    '_struct_ncs_dom_lim.beg_auth_seq_id'                         beg_auth_seq_id                             N
+struct_ncs_dom_lim                    '_struct_ncs_dom_lim.beg_auth_comp_id'                        beg_auth_comp_id                            N
 struct_ncs_dom_lim                    '_struct_ncs_dom_lim.beg_label_alt_id'                        beg_label_alt_id                            N
 struct_ncs_dom_lim                    '_struct_ncs_dom_lim.beg_label_asym_id'                       beg_label_asym_id                           N
 struct_ncs_dom_lim                    '_struct_ncs_dom_lim.beg_label_comp_id'                       beg_label_comp_id                           N
 struct_ncs_dom_lim                    '_struct_ncs_dom_lim.beg_label_seq_id'                        beg_label_seq_id                            N
 struct_ncs_dom_lim                    '_struct_ncs_dom_lim.end_auth_asym_id'                        end_auth_asym_id                            N
 struct_ncs_dom_lim                    '_struct_ncs_dom_lim.end_auth_seq_id'                         end_auth_seq_id                             N
+struct_ncs_dom_lim                    '_struct_ncs_dom_lim.end_auth_comp_id'                        end_auth_comp_id                            N
 struct_ncs_dom_lim                    '_struct_ncs_dom_lim.end_label_alt_id'                        end_label_alt_id                            N
 struct_ncs_dom_lim                    '_struct_ncs_dom_lim.end_label_asym_id'                       end_label_asym_id                           N
 struct_ncs_dom_lim                    '_struct_ncs_dom_lim.end_label_comp_id'                       end_label_comp_id                           N
 struct_ncs_dom_lim                    '_struct_ncs_dom_lim.end_label_seq_id'                        end_label_seq_id                            N
 struct_ncs_dom_lim                    '_struct_ncs_dom_lim.pdbx_component_id'                       pdbx_component_id                           N
 struct_ncs_dom_lim                    '_struct_ncs_dom_lim.pdbx_refine_code'                        pdbx_refine_code                            N
 struct_ncs_dom_lim                    '_struct_ncs_dom_lim.pdbx_ens_id'                             pdbx_ens_id                                 N
```

### Comparing `wwpdb.apps.editormodule-0.18/wwpdb/apps/editormodule/depict/EditorDepict.py` & `wwpdb_apps_editormodule-0.18.1/wwpdb/apps/editormodule/depict/EditorDepict.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.editormodule-0.18/wwpdb/apps/editormodule/io/EditorDataImport.py` & `wwpdb_apps_editormodule-0.18.1/wwpdb/apps/editormodule/io/EditorDataImport.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.editormodule-0.18/wwpdb/apps/editormodule/io/PdbxDataIo.py` & `wwpdb_apps_editormodule-0.18.1/wwpdb/apps/editormodule/io/PdbxDataIo.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.editormodule-0.18/wwpdb/apps/editormodule/io/PdbxMasterViewDictionary.py` & `wwpdb_apps_editormodule-0.18.1/wwpdb/apps/editormodule/io/PdbxMasterViewDictionary.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.editormodule-0.18/wwpdb/apps/editormodule/io/PdbxMasterViewDictionaryExec.py` & `wwpdb_apps_editormodule-0.18.1/wwpdb/apps/editormodule/io/PdbxMasterViewDictionaryExec.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.editormodule-0.18/wwpdb/apps/editormodule/templates/common_tool_beta_testing_feedback.html` & `wwpdb_apps_editormodule-0.18.1/wwpdb/apps/editormodule/templates/common_tool_beta_testing_feedback.html`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.editormodule-0.18/wwpdb/apps/editormodule/templates/editor_jmol_tmplt.html` & `wwpdb_apps_editormodule-0.18.1/wwpdb/apps/editormodule/templates/editor_jmol_tmplt.html`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.editormodule-0.18/wwpdb/apps/editormodule/templates/editor_launch_tmplt.html` & `wwpdb_apps_editormodule-0.18.1/wwpdb/apps/editormodule/templates/editor_launch_tmplt.html`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.editormodule-0.18/wwpdb/apps/editormodule/templates/editor_launch_tmplt_config.html` & `wwpdb_apps_editormodule-0.18.1/wwpdb/apps/editormodule/templates/editor_launch_tmplt_config.html`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.editormodule-0.18/wwpdb/apps/editormodule/templates/editor_launch_tmplt_scrollnav.html` & `wwpdb_apps_editormodule-0.18.1/wwpdb/apps/editormodule/templates/editor_launch_tmplt_scrollnav.html`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.editormodule-0.18/wwpdb/apps/editormodule/templates/editor_prototyping.html` & `wwpdb_apps_editormodule-0.18.1/wwpdb/apps/editormodule/templates/editor_prototyping.html`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.editormodule-0.18/wwpdb/apps/editormodule/templates/editor_ui_config_admin.html` & `wwpdb_apps_editormodule-0.18.1/wwpdb/apps/editormodule/templates/editor_ui_config_admin.html`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.editormodule-0.18/wwpdb/apps/editormodule/webapp/EditorWebApp.py` & `wwpdb_apps_editormodule-0.18.1/wwpdb/apps/editormodule/webapp/EditorWebApp.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.editormodule-0.18/wwpdb/apps/editormodule/webapp/WebRequest.py` & `wwpdb_apps_editormodule-0.18.1/wwpdb/apps/editormodule/webapp/WebRequest.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.editormodule-0.18/wwpdb.apps.editormodule.egg-info/PKG-INFO` & `wwpdb_apps_editormodule-0.18.1/wwpdb.apps.editormodule.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwpdb.apps.editormodule
-Version: 0.18
+Version: 0.18.1
 Summary: wwPDB mmCIF form editor module
 Home-page: https://github.com/rcsb/py-wwpdb_apps_editormodule
 Author: Ezra Peisach
 Author-email: ezra.peisach@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `wwpdb.apps.editormodule-0.18/wwpdb.apps.editormodule.egg-info/SOURCES.txt` & `wwpdb_apps_editormodule-0.18.1/wwpdb.apps.editormodule.egg-info/SOURCES.txt`

 * *Files identical despite different names*

