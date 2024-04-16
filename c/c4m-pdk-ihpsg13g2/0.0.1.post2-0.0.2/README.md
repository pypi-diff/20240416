# Comparing `tmp/c4m_pdk_ihpsg13g2-0.0.1.post2.tar.gz` & `tmp/c4m_pdk_ihpsg13g2-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "c4m_pdk_ihpsg13g2-0.0.1.post2.tar", last modified: Fri Feb 16 11:43:45 2024, max compression
+gzip compressed data, was "c4m_pdk_ihpsg13g2-0.0.2.tar", last modified: Tue Apr 16 15:59:57 2024, max compression
```

## Comparing `c4m_pdk_ihpsg13g2-0.0.1.post2.tar` & `c4m_pdk_ihpsg13g2-0.0.2.tar`

### file list

```diff
@@ -1,31 +1,10 @@
--rw-r--r--   0        0        0      566 2023-07-14 12:42:38.032196 c4m_pdk_ihpsg13g2-0.0.1.post2/LICENSE.md
--rw-r--r--   0        0        0    34523 2023-07-14 12:42:38.032196 c4m_pdk_ihpsg13g2-0.0.1.post2/LICENSES/agpl-3.0.txt
--rw-r--r--   0        0        0    11358 2023-07-14 12:42:38.032196 c4m_pdk_ihpsg13g2-0.0.1.post2/LICENSES/apache-2.0.txt
--rw-r--r--   0        0        0    13419 2023-07-14 12:42:38.032196 c4m_pdk_ihpsg13g2-0.0.1.post2/LICENSES/cern_ohl_s_v2.txt
--rw-r--r--   0        0        0    18009 2023-07-14 12:42:38.036196 c4m_pdk_ihpsg13g2-0.0.1.post2/LICENSES/gpl-2.0.txt
--rw-r--r--   0        0        0     7223 2024-02-16 11:38:55.160660 c4m_pdk_ihpsg13g2-0.0.1.post2/README.md
--rw-r--r--   0        0        0      149 2024-02-14 16:37:29.438141 c4m_pdk_ihpsg13g2-0.0.1.post2/c4m/__init__.py
--rw-r--r--   0        0        0      149 2024-02-14 16:37:29.438141 c4m_pdk_ihpsg13g2-0.0.1.post2/c4m/pdk/__init__.py
--rw-r--r--   0        0        0      386 2024-02-14 16:48:41.349717 c4m_pdk_ihpsg13g2-0.0.1.post2/c4m/pdk/ihpsg13g2/__init__.py
--rw-r--r--   0        0        0     4558 2024-02-14 17:14:31.962434 c4m_pdk_ihpsg13g2-0.0.1.post2/c4m/pdk/ihpsg13g2/_io_compliance.py
--rw-r--r--   0        0        0     6904 2024-02-14 17:14:31.978434 c4m_pdk_ihpsg13g2-0.0.1.post2/c4m/pdk/ihpsg13g2/io.py
--rw-r--r--   0        0        0       23 2024-01-07 16:49:21.036072 c4m_pdk_ihpsg13g2-0.0.1.post2/c4m/pdk/ihpsg13g2/models/__init__.py
--rw-r--r--   0        0        0      775 2024-01-07 16:49:21.100072 c4m_pdk_ihpsg13g2-0.0.1.post2/c4m/pdk/ihpsg13g2/models/all.spice
--rw-r--r--   0        0        0    24555 2024-01-07 16:49:21.076072 c4m_pdk_ihpsg13g2-0.0.1.post2/c4m/pdk/ihpsg13g2/models/cornerMOShv.lib
--rw-r--r--   0        0        0    22926 2024-01-07 16:49:21.056072 c4m_pdk_ihpsg13g2-0.0.1.post2/c4m/pdk/ihpsg13g2/models/cornerMOSlv.lib
--rw-r--r--   0        0        0     2460 2024-01-07 16:49:21.092072 c4m_pdk_ihpsg13g2-0.0.1.post2/c4m/pdk/ihpsg13g2/models/cornerRES.lib
--rw-r--r--   0        0        0     3704 2024-01-07 16:49:21.096072 c4m_pdk_ihpsg13g2-0.0.1.post2/c4m/pdk/ihpsg13g2/models/diodes.lib
--rw-r--r--   0        0        0     1900 2024-01-07 16:49:21.080072 c4m_pdk_ihpsg13g2-0.0.1.post2/c4m/pdk/ihpsg13g2/models/resistors_mod.lib
--rw-r--r--   0        0        0     1039 2024-01-07 16:49:21.084072 c4m_pdk_ihpsg13g2-0.0.1.post2/c4m/pdk/ihpsg13g2/models/resistors_parm.lib
--rw-r--r--   0        0        0     1045 2024-01-07 16:49:21.088072 c4m_pdk_ihpsg13g2-0.0.1.post2/c4m/pdk/ihpsg13g2/models/resistors_stat.lib
--rw-r--r--   0        0        0     8466 2024-01-07 16:49:21.060072 c4m_pdk_ihpsg13g2-0.0.1.post2/c4m/pdk/ihpsg13g2/models/sg13g2_moshv_mod.lib
--rw-r--r--   0        0        0    40830 2024-01-07 16:49:21.064072 c4m_pdk_ihpsg13g2-0.0.1.post2/c4m/pdk/ihpsg13g2/models/sg13g2_moshv_parm.lib
--rw-r--r--   0        0        0     4027 2024-01-07 16:49:21.068072 c4m_pdk_ihpsg13g2-0.0.1.post2/c4m/pdk/ihpsg13g2/models/sg13g2_moshv_stat.lib
--rw-r--r--   0        0        0     8422 2024-01-07 16:49:21.040072 c4m_pdk_ihpsg13g2-0.0.1.post2/c4m/pdk/ihpsg13g2/models/sg13g2_moslv_mod.lib
--rw-r--r--   0        0        0    41163 2024-01-07 16:49:21.044072 c4m_pdk_ihpsg13g2-0.0.1.post2/c4m/pdk/ihpsg13g2/models/sg13g2_moslv_parm.lib
--rw-r--r--   0        0        0     4890 2024-01-07 16:49:21.048072 c4m_pdk_ihpsg13g2-0.0.1.post2/c4m/pdk/ihpsg13g2/models/sg13g2_moslv_stat.lib
--rw-r--r--   0        0        0    18343 2024-02-14 17:18:42.851496 c4m_pdk_ihpsg13g2-0.0.1.post2/c4m/pdk/ihpsg13g2/pdkmaster.py
--rw-r--r--   0        0        0     2617 2024-02-14 16:48:41.345718 c4m_pdk_ihpsg13g2-0.0.1.post2/c4m/pdk/ihpsg13g2/pyspice.py
--rw-r--r--   0        0        0     4300 2024-02-14 17:18:42.851496 c4m_pdk_ihpsg13g2-0.0.1.post2/c4m/pdk/ihpsg13g2/stdcell.py
--rw-r--r--   0        0        0     1224 2024-02-16 11:43:45.650147 c4m_pdk_ihpsg13g2-0.0.1.post2/pyproject.toml
--rw-r--r--   0        0        0     7619 1970-01-01 00:00:00.000000 c4m_pdk_ihpsg13g2-0.0.1.post2/PKG-INFO
+-rw-r--r--   0        0        0      566 2024-04-16 12:07:28.460124 c4m_pdk_ihpsg13g2-0.0.2/LICENSE.md
+-rw-r--r--   0        0        0    34523 2024-04-16 12:07:28.460124 c4m_pdk_ihpsg13g2-0.0.2/LICENSES/agpl-3.0.txt
+-rw-r--r--   0        0        0    11358 2024-04-16 12:07:28.460124 c4m_pdk_ihpsg13g2-0.0.2/LICENSES/apache-2.0.txt
+-rw-r--r--   0        0        0    13419 2024-04-16 12:07:28.460124 c4m_pdk_ihpsg13g2-0.0.2/LICENSES/cern_ohl_s_v2.txt
+-rw-r--r--   0        0        0    18009 2024-04-16 12:07:28.460124 c4m_pdk_ihpsg13g2-0.0.2/LICENSES/gpl-2.0.txt
+-rw-r--r--   0        0        0     7408 2024-04-16 15:44:57.688258 c4m_pdk_ihpsg13g2-0.0.2/README.md
+-rw-r--r--   0        0        0    24621 2024-04-16 12:07:28.460124 c4m_pdk_ihpsg13g2-0.0.2/dodo.py
+-rw-r--r--   0        0        0     1488 2024-04-16 15:59:57.490877 c4m_pdk_ihpsg13g2-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0        6 2024-04-16 15:59:57.490877 c4m_pdk_ihpsg13g2-0.0.2/version.txt
+-rw-r--r--   0        0        0     7841 1970-01-01 00:00:00.000000 c4m_pdk_ihpsg13g2-0.0.2/PKG-INFO
```

### Comparing `c4m_pdk_ihpsg13g2-0.0.1.post2/LICENSE.md` & `c4m_pdk_ihpsg13g2-0.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `c4m_pdk_ihpsg13g2-0.0.1.post2/LICENSES/agpl-3.0.txt` & `c4m_pdk_ihpsg13g2-0.0.2/LICENSES/agpl-3.0.txt`

 * *Files identical despite different names*

### Comparing `c4m_pdk_ihpsg13g2-0.0.1.post2/LICENSES/apache-2.0.txt` & `c4m_pdk_ihpsg13g2-0.0.2/LICENSES/apache-2.0.txt`

 * *Files identical despite different names*

### Comparing `c4m_pdk_ihpsg13g2-0.0.1.post2/LICENSES/cern_ohl_s_v2.txt` & `c4m_pdk_ihpsg13g2-0.0.2/LICENSES/cern_ohl_s_v2.txt`

 * *Files identical despite different names*

### Comparing `c4m_pdk_ihpsg13g2-0.0.1.post2/LICENSES/gpl-2.0.txt` & `c4m_pdk_ihpsg13g2-0.0.2/LICENSES/gpl-2.0.txt`

 * *Files identical despite different names*

### Comparing `c4m_pdk_ihpsg13g2-0.0.1.post2/README.md` & `c4m_pdk_ihpsg13g2-0.0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 This is the Chips4Makers' PDK for the SG13G2 open source PDK.
 
 # Versions
 
+* [v0.0.2](https://gitlab.com/Chips4Makers/c4m-pdk-ihpsg13g2/-/commits/v0.0.1): build infrastructure and dependencies update; no major code changes but KLayout PCell lib support added.
 * [v0.0.1](https://gitlab.com/Chips4Makers/c4m-pdk-ihpsg13g2/-/commits/v0.0.1): First public release; main achievement is that code can generate a version of the IO library ready for upstreaming to [IHP-Open-PDK](https://github.com/IHP-GmbH/IHP-Open-PDK/).  
   It can also generate standard cells but these have not been used yet in P&R.
 
 ## Alpha Version of Code
 
 This is an alpha version of the IHP SG13G2 PDK, if it breaks you need to keep the pieces. E.g. hiccups are still expected when using this code base. For further discussion you can use the [Chips4Makers matrix channel](https://matrix.to/#/#Chips4Makers_community:gitter.im). Certainly interested to be made aware about usage of this project.
```

### Comparing `c4m_pdk_ihpsg13g2-0.0.1.post2/pyproject.toml` & `c4m_pdk_ihpsg13g2-0.0.2/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -2,54 +2,68 @@
 name = "c4m-pdk-ihpsg13g2"
 dynamic = []
 description = "PDKMaster based PDK for open source IHP SG13G2 process"
 authors = [
     { name = "Chips4Makers contributors" },
 ]
 dependencies = [
-    "PDKMaster~=0.10.2",
+    "PDKMaster~=0.11.0",
+    "pdkmaster-io-klayout~=0.1.1",
     "c4m-flexcell~=0.4.2",
     "c4m-flexio~=0.4.2",
 ]
-requires-python = "~=3.7"
+requires-python = "~=3.8"
 readme = "README.md"
-version = "0.0.1.post2"
+version = "0.0.2"
 
 [project.license]
 text = "GPL-2.0-or-later OR AGPL-3.0-or-later OR CERN-OHL-S-2.0+"
 
 [build-system]
 requires = [
     "pdm-backend",
-    "dunamai",
 ]
 build-backend = "pdm.backend"
 
 [tool.pdm]
-package-type = "library"
+distribution = true
 ignore_package_warnings = [
     "*",
 ]
 
 [tool.pdm.version]
-source = "call"
-getter = "scripts.version:get_version"
+source = "scm"
+write_to = "version.txt"
 
 [tool.pdm.dev-dependencies]
 dev = [
-    "dunamai",
     "-e file:///${PROJECT_ROOT}/deps/PySpice#egg=PySpice",
     "-e file:///${PROJECT_ROOT}/deps/PDKMaster#egg=PDKMaster",
+    "-e file:///${PROJECT_ROOT}/deps/pdkmaster-io-klayout#egg=pdkmaster-io-klayout",
     "-e file:///${PROJECT_ROOT}/deps/c4m-flexcell#egg=c4m-flexcell",
     "-e file:///${PROJECT_ROOT}/deps/c4m-flexio#egg=c4m-flexio",
     "doit",
     "tomlkit",
+]
+notebook = [
     "jupyter",
     "nbconvert",
 ]
+vscode = [
+    "pip",
+    "docutils",
+    "esbonio",
+]
+fixed_deps = [
+    "klayout==0.27.13",
+    "nbconvert==6.5.3",
+    "Jinja2==3.1.2",
+    "markupsafe==2.1.2",
+    "lxml==4.9.2",
+]
 
 [tool.pdm.scripts]
 post_install = "doit spice_models_python"
 pre_build = "doit spice_models_python"
 cell_list = "./scripts/regen_celllist.sh"
 doit = "doit"
 clean = "doit clean"
```

### Comparing `c4m_pdk_ihpsg13g2-0.0.1.post2/PKG-INFO` & `c4m_pdk_ihpsg13g2-0.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: c4m-pdk-ihpsg13g2
-Version: 0.0.1.post2
+Version: 0.0.2
 Summary: PDKMaster based PDK for open source IHP SG13G2 process
 Author: Chips4Makers contributors
 License: GPL-2.0-or-later OR AGPL-3.0-or-later OR CERN-OHL-S-2.0+
-Requires-Python: ~=3.7
-Requires-Dist: PDKMaster~=0.10.2
+Requires-Python: ~=3.8
+Requires-Dist: PDKMaster~=0.11.0
+Requires-Dist: pdkmaster-io-klayout~=0.1.1
 Requires-Dist: c4m-flexcell~=0.4.2
 Requires-Dist: c4m-flexio~=0.4.2
 Description-Content-Type: text/markdown
 
 This is the Chips4Makers' PDK for the SG13G2 open source PDK.
 
 # Versions
 
+* [v0.0.2](https://gitlab.com/Chips4Makers/c4m-pdk-ihpsg13g2/-/commits/v0.0.1): build infrastructure and dependencies update; no major code changes but KLayout PCell lib support added.
 * [v0.0.1](https://gitlab.com/Chips4Makers/c4m-pdk-ihpsg13g2/-/commits/v0.0.1): First public release; main achievement is that code can generate a version of the IO library ready for upstreaming to [IHP-Open-PDK](https://github.com/IHP-GmbH/IHP-Open-PDK/).  
   It can also generate standard cells but these have not been used yet in P&R.
 
 ## Alpha Version of Code
 
 This is an alpha version of the IHP SG13G2 PDK, if it breaks you need to keep the pieces. E.g. hiccups are still expected when using this code base. For further discussion you can use the [Chips4Makers matrix channel](https://matrix.to/#/#Chips4Makers_community:gitter.im). Certainly interested to be made aware about usage of this project.
```

