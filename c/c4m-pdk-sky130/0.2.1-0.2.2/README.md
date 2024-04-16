# Comparing `tmp/c4m_pdk_sky130-0.2.1.tar.gz` & `tmp/c4m_pdk_sky130-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "c4m_pdk_sky130-0.2.1.tar", last modified: Fri Mar 29 10:24:55 2024, max compression
+gzip compressed data, was "c4m_pdk_sky130-0.2.2.tar", last modified: Tue Apr 16 16:58:36 2024, max compression
```

## Comparing `c4m_pdk_sky130-0.2.1.tar` & `c4m_pdk_sky130-0.2.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      526 2021-04-23 08:32:56.158279 c4m_pdk_sky130-0.2.1/LICENSE.md
--rw-r--r--   0        0        0    34523 2021-04-23 08:25:39.341778 c4m_pdk_sky130-0.2.1/LICENSES/agpl-3.0.txt
--rw-r--r--   0        0        0    10172 2021-04-23 08:25:39.357779 c4m_pdk_sky130-0.2.1/LICENSES/apache-2.0.txt
--rw-r--r--   0        0        0    13419 2021-04-23 08:25:39.349778 c4m_pdk_sky130-0.2.1/LICENSES/cern_ohl_s_v2.txt
--rw-r--r--   0        0        0    18009 2021-04-23 08:25:39.353778 c4m_pdk_sky130-0.2.1/LICENSES/gpl-2.0.txt
--rw-r--r--   0        0        0     1937 2024-03-29 10:20:05.547904 c4m_pdk_sky130-0.2.1/README.md
--rw-r--r--   0        0        0       85 2022-09-05 08:53:58.956782 c4m_pdk_sky130-0.2.1/doitlib/__init__.py
--rw-r--r--   0        0        0      139 2024-03-29 09:37:44.962191 c4m_pdk_sky130-0.2.1/doitlib/libs.py
--rw-r--r--   0        0        0     1315 2024-03-29 10:24:55.735539 c4m_pdk_sky130-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     2365 1970-01-01 00:00:00.000000 c4m_pdk_sky130-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      526 2024-04-16 12:02:53.748097 c4m_pdk_sky130-0.2.2/LICENSE.md
+-rw-r--r--   0        0        0    34523 2024-04-16 12:02:53.748097 c4m_pdk_sky130-0.2.2/LICENSES/agpl-3.0.txt
+-rw-r--r--   0        0        0    10172 2024-04-16 12:02:53.748097 c4m_pdk_sky130-0.2.2/LICENSES/apache-2.0.txt
+-rw-r--r--   0        0        0    13419 2024-04-16 12:02:53.748097 c4m_pdk_sky130-0.2.2/LICENSES/cern_ohl_s_v2.txt
+-rw-r--r--   0        0        0    18009 2024-04-16 12:02:53.748097 c4m_pdk_sky130-0.2.2/LICENSES/gpl-2.0.txt
+-rw-r--r--   0        0        0     2119 2024-04-16 16:55:29.047553 c4m_pdk_sky130-0.2.2/README.md
+-rw-r--r--   0        0        0       85 2024-04-16 12:02:53.752097 c4m_pdk_sky130-0.2.2/doitlib/__init__.py
+-rw-r--r--   0        0        0      139 2024-04-16 12:02:53.752097 c4m_pdk_sky130-0.2.2/doitlib/libs.py
+-rw-r--r--   0        0        0     1369 2024-04-16 16:58:36.316875 c4m_pdk_sky130-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     2547 1970-01-01 00:00:00.000000 c4m_pdk_sky130-0.2.2/PKG-INFO
```

### Comparing `c4m_pdk_sky130-0.2.1/LICENSE.md` & `c4m_pdk_sky130-0.2.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `c4m_pdk_sky130-0.2.1/LICENSES/agpl-3.0.txt` & `c4m_pdk_sky130-0.2.2/LICENSES/agpl-3.0.txt`

 * *Files identical despite different names*

### Comparing `c4m_pdk_sky130-0.2.1/LICENSES/apache-2.0.txt` & `c4m_pdk_sky130-0.2.2/LICENSES/apache-2.0.txt`

 * *Files identical despite different names*

### Comparing `c4m_pdk_sky130-0.2.1/LICENSES/cern_ohl_s_v2.txt` & `c4m_pdk_sky130-0.2.2/LICENSES/cern_ohl_s_v2.txt`

 * *Files identical despite different names*

### Comparing `c4m_pdk_sky130-0.2.1/LICENSES/gpl-2.0.txt` & `c4m_pdk_sky130-0.2.2/LICENSES/gpl-2.0.txt`

 * *Files identical despite different names*

### Comparing `c4m_pdk_sky130-0.2.1/README.md` & `c4m_pdk_sky130-0.2.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 This is the PDK for Sky130 based on the [PDKMaster](https://gitlab.com/Chips4Makers/PDKMaster) framework. It currently is basically undocumented. Development is driven by sky130 MPW shuttle development.
 A little more information on what is possible can be found in the `.gitlab-ci.yml` file.
 
 In the [`v0.1`](https://gitlab.com/Chips4Makers/c4m-pdk-sky130/-/tree/v0.1) branch a SRAM block and some analog circuits were present. These blocks did not work anymore with updated [PDKMaster](https://gitlab.com/Chips4Makers/PDKMaster) and [c4m-flexcell](https://gitlab.com/Chips4Makers/c4m-flexcell) modules. These blocks have therefor been removed from the main branch. Furhter development is not done in the [`sram`](https://gitlab.com/Chips4Makers/c4m-pdk-sky130/-/tree/sram) and the [`analog`](https://gitlab.com/Chips4Makers/c4m-pdk-sky130/-/tree/analog) branch.
 
 ## Release history
 
+* [v0.2.2](https://gitlab.com/Chips4Makers/c4m-pdk-sky130/-/commits/v0.2.2): build infrastructure and dependencies update; no major code changes but KLayout PCell lib support added.
 * v0.2.1: Switch to latest version of PDKMaster and c4m-flexcell. As these updates break the SRAM and analog circuits they have been removed from this stable branch. `v0.1` branch is available using old version of these modules and with the SRAM block and the analog circuits.
 Development of SRAM and analog blocks is done in separate branches `sram` and `analog`. Development in these branches will be merged again in upstream as they are fixed.  
 Intermediate development was done on a `v0.2.0` dev branch.
 * v0.1.5: Update bandgap model support, update analog python notebooks.
 * v0.1.4: No code changes; update dependencies for latest bug fixes
 * v0.1.3: No code change; use PDKMaster 0.9.2 to get Coriolis export compatible with namespace of
   latest Coriolis release.
```

### Comparing `c4m_pdk_sky130-0.2.1/pyproject.toml` & `c4m_pdk_sky130-0.2.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -3,29 +3,28 @@
 dynamic = []
 description = "PDKMaster based PDK for open source GF180MCU process"
 authors = [
     { name = "Chips4Makers contributors" },
 ]
 dependencies = [
     "PDKMaster~=0.11.0",
-    "pdkmaster-io-klayout~=0.1.0",
+    "pdkmaster-io-klayout~=0.1.1",
     "c4m-flexcell~=0.4.2",
     "c4m-flexio~=0.4.2",
 ]
 requires-python = "~=3.8"
 readme = "README.md"
-version = "0.2.1"
+version = "0.2.2"
 
 [project.license]
 text = "GPL-2.0-or-later OR AGPL-3.0-or-later OR CERN-OHL-S-2.0+"
 
 [build-system]
 requires = [
     "pdm-backend",
-    "dunamai",
 ]
 build-backend = "pdm.backend"
 
 [tool.pdm]
 ignore_package_warnings = [
     "*",
 ]
@@ -39,20 +38,27 @@
     "-e file:///${PROJECT_ROOT}/deps/PySpice#egg=PySpice",
     "-e file:///${PROJECT_ROOT}/deps/PDKMaster#egg=PDKMaster",
     "-e file:///${PROJECT_ROOT}/deps/pdkmaster-io-klayout#egg=pdkmaster-io-klayout",
     "-e file:///${PROJECT_ROOT}/deps/c4m-flexcell#egg=c4m-flexcell",
     "-e file:///${PROJECT_ROOT}/deps/c4m-flexio#egg=c4m-flexio",
     "doit",
     "tomlkit",
-    "jupyter",
-    "nbconvert",
+]
+vscode = [
     "pip",
     "docutils",
     "esbonio",
 ]
+notebook = [
+    "jupyter",
+    "nbconvert",
+]
+fixed_deps = [
+    "klayout==0.27.13",
+]
 
 [tool.pdm.scripts]
 post_install = "doit spice_models_python"
 pre_build = "doit spice_models_python"
 cell_list = "./scripts/regen_celllist.sh"
 doit = "doit"
 clean = "doit clean"
```

### Comparing `c4m_pdk_sky130-0.2.1/PKG-INFO` & `c4m_pdk_sky130-0.2.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 Metadata-Version: 2.1
 Name: c4m-pdk-sky130
-Version: 0.2.1
+Version: 0.2.2
 Summary: PDKMaster based PDK for open source GF180MCU process
 Author: Chips4Makers contributors
 License: GPL-2.0-or-later OR AGPL-3.0-or-later OR CERN-OHL-S-2.0+
 Requires-Python: ~=3.8
 Requires-Dist: PDKMaster~=0.11.0
-Requires-Dist: pdkmaster-io-klayout~=0.1.0
+Requires-Dist: pdkmaster-io-klayout~=0.1.1
 Requires-Dist: c4m-flexcell~=0.4.2
 Requires-Dist: c4m-flexio~=0.4.2
 Description-Content-Type: text/markdown
 
 # PDKMaster based Sky130 PDK
 
 This is the PDK for Sky130 based on the [PDKMaster](https://gitlab.com/Chips4Makers/PDKMaster) framework. It currently is basically undocumented. Development is driven by sky130 MPW shuttle development.
 A little more information on what is possible can be found in the `.gitlab-ci.yml` file.
 
 In the [`v0.1`](https://gitlab.com/Chips4Makers/c4m-pdk-sky130/-/tree/v0.1) branch a SRAM block and some analog circuits were present. These blocks did not work anymore with updated [PDKMaster](https://gitlab.com/Chips4Makers/PDKMaster) and [c4m-flexcell](https://gitlab.com/Chips4Makers/c4m-flexcell) modules. These blocks have therefor been removed from the main branch. Furhter development is not done in the [`sram`](https://gitlab.com/Chips4Makers/c4m-pdk-sky130/-/tree/sram) and the [`analog`](https://gitlab.com/Chips4Makers/c4m-pdk-sky130/-/tree/analog) branch.
 
 ## Release history
 
+* [v0.2.2](https://gitlab.com/Chips4Makers/c4m-pdk-sky130/-/commits/v0.2.2): build infrastructure and dependencies update; no major code changes but KLayout PCell lib support added.
 * v0.2.1: Switch to latest version of PDKMaster and c4m-flexcell. As these updates break the SRAM and analog circuits they have been removed from this stable branch. `v0.1` branch is available using old version of these modules and with the SRAM block and the analog circuits.
 Development of SRAM and analog blocks is done in separate branches `sram` and `analog`. Development in these branches will be merged again in upstream as they are fixed.  
 Intermediate development was done on a `v0.2.0` dev branch.
 * v0.1.5: Update bandgap model support, update analog python notebooks.
 * v0.1.4: No code changes; update dependencies for latest bug fixes
 * v0.1.3: No code change; use PDKMaster 0.9.2 to get Coriolis export compatible with namespace of
   latest Coriolis release.
```

