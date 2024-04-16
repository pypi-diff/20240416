# Comparing `tmp/ansys-mechanical-env-0.1.5.tar.gz` & `tmp/ansys_mechanical_env-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansys-mechanical-env-0.1.5.tar", last modified: Fri Mar 22 14:11:17 2024, max compression
+gzip compressed data, was "ansys_mechanical_env-0.1.6.tar", last modified: Tue Apr 16 15:56:15 2024, max compression
```

## Comparing `ansys-mechanical-env-0.1.5.tar` & `ansys_mechanical_env-0.1.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 14:11:17.051988 ansys-mechanical-env-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-03-22 14:11:03.000000 ansys-mechanical-env-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     9135 2024-03-22 14:11:17.047988 ansys-mechanical-env-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8390 2024-03-22 14:11:03.000000 ansys-mechanical-env-0.1.5/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-03-22 14:11:03.000000 ansys-mechanical-env-0.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-22 14:11:17.051988 ansys-mechanical-env-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-03-22 14:11:03.000000 ansys-mechanical-env-0.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 14:11:17.047988 ansys-mechanical-env-0.1.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 14:11:17.047988 ansys-mechanical-env-0.1.5/src/ansys/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 14:11:17.047988 ansys-mechanical-env-0.1.5/src/ansys/mechanical/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 14:11:17.047988 ansys-mechanical-env-0.1.5/src/ansys/mechanical/env/
--rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-03-22 14:11:03.000000 ansys-mechanical-env-0.1.5/src/ansys/mechanical/env/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5967 2024-03-22 14:11:03.000000 ansys-mechanical-env-0.1.5/src/ansys/mechanical/env/mechanical-env
--rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-03-22 14:11:03.000000 ansys-mechanical-env-0.1.5/src/ansys/mechanical/env/run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 14:11:17.047988 ansys-mechanical-env-0.1.5/src/ansys_mechanical_env.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9135 2024-03-22 14:11:17.000000 ansys-mechanical-env-0.1.5/src/ansys_mechanical_env.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-03-22 14:11:17.000000 ansys-mechanical-env-0.1.5/src/ansys_mechanical_env.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 14:11:17.000000 ansys-mechanical-env-0.1.5/src/ansys_mechanical_env.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-03-22 14:11:17.000000 ansys-mechanical-env-0.1.5/src/ansys_mechanical_env.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-03-22 14:11:17.000000 ansys-mechanical-env-0.1.5/src/ansys_mechanical_env.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-22 14:11:17.000000 ansys-mechanical-env-0.1.5/src/ansys_mechanical_env.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 14:11:17.047988 ansys-mechanical-env-0.1.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-03-22 14:11:03.000000 ansys-mechanical-env-0.1.5/tests/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     4436 2024-03-22 14:11:03.000000 ansys-mechanical-env-0.1.5/tests/test_script.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:56:15.384674 ansys_mechanical_env-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-16 15:56:05.000000 ansys_mechanical_env-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9135 2024-04-16 15:56:15.384674 ansys_mechanical_env-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8390 2024-04-16 15:56:05.000000 ansys_mechanical_env-0.1.6/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-16 15:56:05.000000 ansys_mechanical_env-0.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 15:56:15.384674 ansys_mechanical_env-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-04-16 15:56:05.000000 ansys_mechanical_env-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:56:15.380674 ansys_mechanical_env-0.1.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:56:15.380674 ansys_mechanical_env-0.1.6/src/ansys/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:56:15.380674 ansys_mechanical_env-0.1.6/src/ansys/mechanical/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:56:15.384674 ansys_mechanical_env-0.1.6/src/ansys/mechanical/env/
+-rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-04-16 15:56:05.000000 ansys_mechanical_env-0.1.6/src/ansys/mechanical/env/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6140 2024-04-16 15:56:05.000000 ansys_mechanical_env-0.1.6/src/ansys/mechanical/env/mechanical-env
+-rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-04-16 15:56:05.000000 ansys_mechanical_env-0.1.6/src/ansys/mechanical/env/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:56:15.384674 ansys_mechanical_env-0.1.6/src/ansys_mechanical_env.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9135 2024-04-16 15:56:15.000000 ansys_mechanical_env-0.1.6/src/ansys_mechanical_env.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-16 15:56:15.000000 ansys_mechanical_env-0.1.6/src/ansys_mechanical_env.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 15:56:15.000000 ansys_mechanical_env-0.1.6/src/ansys_mechanical_env.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-16 15:56:15.000000 ansys_mechanical_env-0.1.6/src/ansys_mechanical_env.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-16 15:56:15.000000 ansys_mechanical_env-0.1.6/src/ansys_mechanical_env.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-16 15:56:15.000000 ansys_mechanical_env-0.1.6/src/ansys_mechanical_env.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:56:15.384674 ansys_mechanical_env-0.1.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-04-16 15:56:05.000000 ansys_mechanical_env-0.1.6/tests/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4621 2024-04-16 15:56:05.000000 ansys_mechanical_env-0.1.6/tests/test_script.py
```

### Comparing `ansys-mechanical-env-0.1.5/LICENSE` & `ansys_mechanical_env-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ansys-mechanical-env-0.1.5/PKG-INFO` & `ansys_mechanical_env-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansys-mechanical-env
-Version: 0.1.5
+Version: 0.1.6
 Summary: A python wrapper for loading environment variables when using PyMechanical embedded instances in Linux.
 Home-page: https://github.com/ansys/pymechanical-env
 Author: ANSYS, Inc.
 Author-email: pyansys.core@ansys.com
 Maintainer: ANSYS, Inc.
 Maintainer-email: pyansys.core@ansys.com
 License: MIT
```

### Comparing `ansys-mechanical-env-0.1.5/README.rst` & `ansys_mechanical_env-0.1.6/README.rst`

 * *Files identical despite different names*

### Comparing `ansys-mechanical-env-0.1.5/setup.py` & `ansys_mechanical_env-0.1.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Project installation script."""
 
 from setuptools import find_namespace_packages, setup
 
 setup(
     name="ansys-mechanical-env",
-    version="0.1.5",
+    version="0.1.6",
     url="https://github.com/ansys/pymechanical-env",
     author="ANSYS, Inc.",
     author_email="pyansys.core@ansys.com",
     maintainer="ANSYS, Inc.",
     maintainer_email="pyansys.core@ansys.com",
     classifiers=[
         "Development Status :: 4 - Beta",
```

### Comparing `ansys-mechanical-env-0.1.5/src/ansys/mechanical/env/__init__.py` & `ansys_mechanical_env-0.1.6/src/ansys/mechanical/env/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys-mechanical-env-0.1.5/src/ansys/mechanical/env/mechanical-env` & `ansys_mechanical_env-0.1.6/src/ansys/mechanical/env/mechanical-env`

 * *Files 2% similar despite different names*

```diff
@@ -174,11 +174,16 @@
 PATH=${MWHOME}/bin-amd64_linux_optimized\
 :${DS_INSTALL_DIR}/CommonFiles/linx64\
 :${DS_INSTALL_DIR}/CADIntegration/linx64\
 :${!awp_root}/Tools/mono/Linux64/bin\
 :${PATH}
 export PATH
 
+# Adding dummy variable to check if mechanical-env is used
+# when performing embedding with pymechanical in linux
+PYMECHANICAL_EMBEDDING=TRUE
+export PYMECHANICAL_EMBEDDING
+
 # Evaluate the command and get the return code of the process
 eval $@
 returnCode=$?
 exit $returnCode
```

### Comparing `ansys-mechanical-env-0.1.5/src/ansys/mechanical/env/run.py` & `ansys_mechanical_env-0.1.6/src/ansys/mechanical/env/run.py`

 * *Files 8% similar despite different names*

```diff
@@ -49,23 +49,15 @@
 
     Example
     -------
     Get the version and location of the installation directory.
 
     >>> find-mechanical -r 232
     """
-    # Get the version number
-    if not version:
-        exe = atp.get_mechanical_path()  # check for saved mechanical path
-        if exe:
-            version = atp.version_from_path("mechanical", exe)  # version is already int here
-        else:
-            exe, _version = atp.find_mechanical()
-            version = int(_version * 10)
-    else:
-        exe, _version = atp.find_mechanical(version=version)
-        version = int(_version * 10)
+    # checks for saved mechanical path else try to find installation path
+    _exe = atp.get_mechanical_path(allow_input=False, version=version)
+    _version = atp.version_from_path("mechanical", _exe)
 
-    aisol_path = os.path.dirname(exe)
-    print(version, aisol_path)
+    _aisol_path = os.path.dirname(_exe)
+    print(_version, _aisol_path)
 
-    return version, aisol_path
+    return _version, _aisol_path
```

### Comparing `ansys-mechanical-env-0.1.5/src/ansys_mechanical_env.egg-info/PKG-INFO` & `ansys_mechanical_env-0.1.6/src/ansys_mechanical_env.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansys-mechanical-env
-Version: 0.1.5
+Version: 0.1.6
 Summary: A python wrapper for loading environment variables when using PyMechanical embedded instances in Linux.
 Home-page: https://github.com/ansys/pymechanical-env
 Author: ANSYS, Inc.
 Author-email: pyansys.core@ansys.com
 Maintainer: ANSYS, Inc.
 Maintainer-email: pyansys.core@ansys.com
 License: MIT
```

### Comparing `ansys-mechanical-env-0.1.5/tests/test_metadata.py` & `ansys_mechanical_env-0.1.6/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `ansys-mechanical-env-0.1.5/tests/test_script.py` & `ansys_mechanical_env-0.1.6/tests/test_script.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,74 +19,75 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 import os
 import subprocess
 
-import ansys.tools.path as atp
+from click.testing import CliRunner
 import pytest
 
+from ansys.mechanical.env.run import cli_find_mechanical
+
 
 def find_installed_versions():
     """Finds all the installed version of Mechanical."""
     supported_versions = [232, 241, 242]
     versions_found = []
+    runner = CliRunner()
     for supported_version in supported_versions:
-        try:
-            exe, version = atp.find_mechanical(version=supported_version)
-        except:
-            version = None
-        if version:
-            versions_found.append(supported_version)
+        result = runner.invoke(cli_find_mechanical, ["-r", int(supported_version)])
+        _version = None
+        if result.exit_code == 0:
+            _version = result.output.split()[0]  # exe is not needed for this test
+        if _version is not None:
+            versions_found.append(_version)
     return versions_found
 
 
 @pytest.mark.parametrize("version_number", find_installed_versions())
 def test_version_argument(version_number):
     """Ensure script takes version and find if it present"""
     cmd = f"mechanical-env -r {version_number} env"
     process = subprocess.Popen(
         cmd,
         shell=True,
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
     )
-    stdout, stderr = process.communicate()
+    _, stderr = process.communicate()
 
     # Assert no error after running script
     assert stderr is None or stderr == b""
 
 
 def test_unsupported_version():
     """Ensure script gives error for unsupported version."""
     cmd = "mechanical-env -r 230 env"
     process = subprocess.Popen(
         cmd,
         shell=True,
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
     )
-    stdout, stderr = process.communicate()
-    assert "ValueError" in stderr.decode()
+    _, stderr = process.communicate()
+    assert stderr is not None
 
 
 def test_env_variable():
     """Ensure the system environment does not change when running ``mechanical-env``."""
     start_env = os.environ
     cmd = "mechanical-env python"
     process = subprocess.Popen(
         cmd,
         shell=True,
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
     )
     process.wait()
-    stdout = process.stdout.read().decode()
-    stderr = process.stderr.read().decode()
 
     # Get environment after running mechanical-env
     end_env = os.environ
 
     # Assert the environment did not change
     assert start_env == end_env
 
@@ -97,20 +98,22 @@
     cmd = "mechanical-env env 2>&1"
     process = subprocess.Popen(
         cmd,
         shell=True,
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
     )
-    stdout, stderr = process.communicate()
+    stdout, _ = process.communicate()
     return_code = process.returncode
 
-    # Assert for AWP_ROOT variable which created by script
-    assert f"AWP_ROOT{version_number}=/install/ansys_inc/v{version_number}/aisol/.." in str(stdout)
-
+    # Assert for some common variables sets by script
+    assert f"AWP_ROOT{version_number}=" in str(stdout)
+    assert f"AWP_LOCALE{version_number}=en-us" in str(stdout)
+    # Assert dummy env PYMECHANICAL_EMBEDDING
+    assert f"PYMECHANICAL_EMBEDDING=TRUE" in str(stdout)
     # Assert variable specific to version 232
     if version_number == 232:
         print(version_number)
         assert "/tp/IntelCompiler/2019.3.199/linx64/lib/intel64" in str(stdout)
 
     # Assert variable specific to version 241
     if version_number == 241:
```

