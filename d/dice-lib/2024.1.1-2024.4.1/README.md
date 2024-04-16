# Comparing `tmp/dice_lib-2024.1.1.tar.gz` & `tmp/dice_lib-2024.4.1.tar.gz`

## Comparing `dice_lib-2024.1.1.tar` & `dice_lib-2024.4.1.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 dice_lib-2024.1.1/.flake8
--rw-r--r--   0        0        0     2373 2020-02-02 00:00:00.000000 dice_lib-2024.1.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 dice_lib-2024.1.1/.readthedocs.yml
--rw-r--r--   0        0        0     2744 2020-02-02 00:00:00.000000 dice_lib-2024.1.1/noxfile.py
--rw-r--r--   0        0        0     2357 2020-02-02 00:00:00.000000 dice_lib-2024.1.1/.github/CONTRIBUTING.md
--rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 dice_lib-2024.1.1/.github/dependabot.yml
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 dice_lib-2024.1.1/.github/matchers/pylint.json
--rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 dice_lib-2024.1.1/.github/workflows/cd.yml
--rw-r--r--   0        0        0     1488 2020-02-02 00:00:00.000000 dice_lib-2024.1.1/.github/workflows/ci.yml
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 dice_lib-2024.1.1/docs/Makefile
--rw-r--r--   0        0        0     2647 2020-02-02 00:00:00.000000 dice_lib-2024.1.1/docs/conf.py
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 dice_lib-2024.1.1/docs/index.rst
--rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 dice_lib-2024.1.1/docs/make.bat
--rw-r--r--   0        0        0   259300 2020-02-02 00:00:00.000000 dice_lib-2024.1.1/docs/_static/dice_logo_dark.png
--rw-r--r--   0        0        0   258511 2020-02-02 00:00:00.000000 dice_lib-2024.1.1/docs/_static/dice_logo_light.png
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 dice_lib-2024.1.1/docs/_static/css/custom.css
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 dice_lib-2024.1.1/src/dice_lib/__init__.py
--rw-r--r--   0        0        0     2206 2020-02-02 00:00:00.000000 dice_lib-2024.1.1/src/dice_lib/_config.py
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 dice_lib-2024.1.1/src/dice_lib/_version.py
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 dice_lib-2024.1.1/src/dice_lib/_version.pyi
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 dice_lib-2024.1.1/src/dice_lib/date.py
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 dice_lib-2024.1.1/src/dice_lib/glossary.py
--rw-r--r--   0        0        0     6476 2020-02-02 00:00:00.000000 dice_lib-2024.1.1/src/dice_lib/host.py
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 dice_lib-2024.1.1/src/dice_lib/logger.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dice_lib-2024.1.1/src/dice_lib/py.typed
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 dice_lib-2024.1.1/src/dice_lib/ranges.py
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 dice_lib-2024.1.1/src/dice_lib/units.py
--rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 dice_lib-2024.1.1/src/dice_lib/user.py
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 dice_lib-2024.1.1/src/dice_lib/distributed/__init__.py
--rw-r--r--   0        0        0     3609 2020-02-02 00:00:00.000000 dice_lib-2024.1.1/src/dice_lib/fs/__init__.py
--rw-r--r--   0        0        0     3023 2020-02-02 00:00:00.000000 dice_lib-2024.1.1/src/dice_lib/fs/_base.py
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 dice_lib-2024.1.1/src/dice_lib/fs/_davix.py
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 dice_lib-2024.1.1/src/dice_lib/fs/_gridftp.py
--rw-r--r--   0        0        0     3601 2020-02-02 00:00:00.000000 dice_lib-2024.1.1/src/dice_lib/fs/_hdfs.py
--rw-r--r--   0        0        0     4026 2020-02-02 00:00:00.000000 dice_lib-2024.1.1/src/dice_lib/fs/_posix.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 dice_lib-2024.1.1/src/dice_lib/fs/_s3.py
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 dice_lib-2024.1.1/src/dice_lib/fs/_xrootd.py
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 dice_lib-2024.1.1/src/dice_lib/health/__init__.py
--rw-r--r--   0        0        0     2736 2020-02-02 00:00:00.000000 dice_lib-2024.1.1/src/dice_lib/health/apel_accounting.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dice_lib-2024.1.1/src/dice_lib/network/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dice_lib-2024.1.1/tests/__init__.py
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 dice_lib-2024.1.1/tests/conftest.py
--rw-r--r--   0        0        0     5682 2020-02-02 00:00:00.000000 dice_lib-2024.1.1/tests/test_config.py
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 dice_lib-2024.1.1/tests/test_package.py
--rw-r--r--   0        0        0     4475 2020-02-02 00:00:00.000000 dice_lib-2024.1.1/tests/data/config.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dice_lib-2024.1.1/tests/fs/__init__.py
--rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 dice_lib-2024.1.1/tests/fs/test_generic.py
--rw-r--r--   0        0        0     2071 2020-02-02 00:00:00.000000 dice_lib-2024.1.1/.gitignore
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 dice_lib-2024.1.1/LICENSE
--rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 dice_lib-2024.1.1/README.md
--rw-r--r--   0        0        0     4264 2020-02-02 00:00:00.000000 dice_lib-2024.1.1/pyproject.toml
--rw-r--r--   0        0        0     4717 2020-02-02 00:00:00.000000 dice_lib-2024.1.1/PKG-INFO
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 dice_lib-2024.4.1/.flake8
+-rw-r--r--   0        0        0     2373 2020-02-02 00:00:00.000000 dice_lib-2024.4.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 dice_lib-2024.4.1/.readthedocs.yml
+-rw-r--r--   0        0        0     2744 2020-02-02 00:00:00.000000 dice_lib-2024.4.1/noxfile.py
+-rw-r--r--   0        0        0     2357 2020-02-02 00:00:00.000000 dice_lib-2024.4.1/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 dice_lib-2024.4.1/.github/dependabot.yml
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 dice_lib-2024.4.1/.github/matchers/pylint.json
+-rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 dice_lib-2024.4.1/.github/workflows/cd.yml
+-rw-r--r--   0        0        0     1488 2020-02-02 00:00:00.000000 dice_lib-2024.4.1/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 dice_lib-2024.4.1/docs/Makefile
+-rw-r--r--   0        0        0     2647 2020-02-02 00:00:00.000000 dice_lib-2024.4.1/docs/conf.py
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 dice_lib-2024.4.1/docs/index.rst
+-rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 dice_lib-2024.4.1/docs/make.bat
+-rw-r--r--   0        0        0   259300 2020-02-02 00:00:00.000000 dice_lib-2024.4.1/docs/_static/dice_logo_dark.png
+-rw-r--r--   0        0        0   258511 2020-02-02 00:00:00.000000 dice_lib-2024.4.1/docs/_static/dice_logo_light.png
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 dice_lib-2024.4.1/docs/_static/css/custom.css
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 dice_lib-2024.4.1/src/dice_lib/__init__.py
+-rw-r--r--   0        0        0     2206 2020-02-02 00:00:00.000000 dice_lib-2024.4.1/src/dice_lib/_config.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 dice_lib-2024.4.1/src/dice_lib/_version.py
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 dice_lib-2024.4.1/src/dice_lib/_version.pyi
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 dice_lib-2024.4.1/src/dice_lib/date.py
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 dice_lib-2024.4.1/src/dice_lib/glossary.py
+-rw-r--r--   0        0        0     6887 2020-02-02 00:00:00.000000 dice_lib-2024.4.1/src/dice_lib/host.py
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 dice_lib-2024.4.1/src/dice_lib/logger.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dice_lib-2024.4.1/src/dice_lib/py.typed
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 dice_lib-2024.4.1/src/dice_lib/ranges.py
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 dice_lib-2024.4.1/src/dice_lib/units.py
+-rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 dice_lib-2024.4.1/src/dice_lib/user.py
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 dice_lib-2024.4.1/src/dice_lib/distributed/__init__.py
+-rw-r--r--   0        0        0     3609 2020-02-02 00:00:00.000000 dice_lib-2024.4.1/src/dice_lib/fs/__init__.py
+-rw-r--r--   0        0        0     3023 2020-02-02 00:00:00.000000 dice_lib-2024.4.1/src/dice_lib/fs/_base.py
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 dice_lib-2024.4.1/src/dice_lib/fs/_davix.py
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 dice_lib-2024.4.1/src/dice_lib/fs/_gridftp.py
+-rw-r--r--   0        0        0     3601 2020-02-02 00:00:00.000000 dice_lib-2024.4.1/src/dice_lib/fs/_hdfs.py
+-rw-r--r--   0        0        0     4026 2020-02-02 00:00:00.000000 dice_lib-2024.4.1/src/dice_lib/fs/_posix.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 dice_lib-2024.4.1/src/dice_lib/fs/_s3.py
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 dice_lib-2024.4.1/src/dice_lib/fs/_xrootd.py
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 dice_lib-2024.4.1/src/dice_lib/health/__init__.py
+-rw-r--r--   0        0        0     2736 2020-02-02 00:00:00.000000 dice_lib-2024.4.1/src/dice_lib/health/apel_accounting.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dice_lib-2024.4.1/src/dice_lib/network/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dice_lib-2024.4.1/tests/__init__.py
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 dice_lib-2024.4.1/tests/conftest.py
+-rw-r--r--   0        0        0     5682 2020-02-02 00:00:00.000000 dice_lib-2024.4.1/tests/test_config.py
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 dice_lib-2024.4.1/tests/test_package.py
+-rw-r--r--   0        0        0     4475 2020-02-02 00:00:00.000000 dice_lib-2024.4.1/tests/data/config.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dice_lib-2024.4.1/tests/fs/__init__.py
+-rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 dice_lib-2024.4.1/tests/fs/test_generic.py
+-rw-r--r--   0        0        0     2071 2020-02-02 00:00:00.000000 dice_lib-2024.4.1/.gitignore
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 dice_lib-2024.4.1/LICENSE
+-rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 dice_lib-2024.4.1/README.md
+-rw-r--r--   0        0        0     4182 2020-02-02 00:00:00.000000 dice_lib-2024.4.1/pyproject.toml
+-rw-r--r--   0        0        0     4629 2020-02-02 00:00:00.000000 dice_lib-2024.4.1/PKG-INFO
```

### Comparing `dice_lib-2024.1.1/.pre-commit-config.yaml` & `dice_lib-2024.4.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dice_lib-2024.1.1/noxfile.py` & `dice_lib-2024.4.1/noxfile.py`

 * *Files identical despite different names*

### Comparing `dice_lib-2024.1.1/.github/CONTRIBUTING.md` & `dice_lib-2024.4.1/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `dice_lib-2024.1.1/.github/matchers/pylint.json` & `dice_lib-2024.4.1/.github/matchers/pylint.json`

 * *Files identical despite different names*

### Comparing `dice_lib-2024.1.1/.github/workflows/cd.yml` & `dice_lib-2024.4.1/.github/workflows/cd.yml`

 * *Files identical despite different names*

### Comparing `dice_lib-2024.1.1/.github/workflows/ci.yml` & `dice_lib-2024.4.1/.github/workflows/ci.yml`

 * *Files 2% similar despite different names*

```diff
@@ -58,8 +58,8 @@
 
       - name: Test package
         run: >-
           python -m pytest -ra --cov --cov-report=xml --cov-report=term
           --durations=20
 
       - name: Upload coverage report
-        uses: codecov/codecov-action@v3.1.4
+        uses: codecov/codecov-action@v4.3.0
```

### Comparing `dice_lib-2024.1.1/docs/Makefile` & `dice_lib-2024.4.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dice_lib-2024.1.1/docs/conf.py` & `dice_lib-2024.4.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dice_lib-2024.1.1/docs/make.bat` & `dice_lib-2024.4.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dice_lib-2024.1.1/docs/_static/dice_logo_dark.png` & `dice_lib-2024.4.1/docs/_static/dice_logo_dark.png`

 * *Files identical despite different names*

### Comparing `dice_lib-2024.1.1/docs/_static/dice_logo_light.png` & `dice_lib-2024.4.1/docs/_static/dice_logo_light.png`

 * *Files identical despite different names*

### Comparing `dice_lib-2024.1.1/src/dice_lib/_config.py` & `dice_lib-2024.4.1/src/dice_lib/_config.py`

 * *Files identical despite different names*

### Comparing `dice_lib-2024.1.1/src/dice_lib/glossary.py` & `dice_lib-2024.4.1/src/dice_lib/glossary.py`

 * *Files identical despite different names*

### Comparing `dice_lib-2024.1.1/src/dice_lib/host.py` & `dice_lib-2024.4.1/src/dice_lib/host.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 import socket
 from dataclasses import dataclass, field
 from typing import Callable
 
-from plumbum import local
+from plumbum import CommandNotFound, local
 from plumbum.machines.paramiko_machine import ParamikoMachine
 
 OUTPUT_PROCESSING_FUNCTIONS = {
     "noop": lambda x: x,
     "to_lower": lambda x: x.lower(),
     "to_upper": lambda x: x.upper(),
     "split_unique_join": lambda x: ",".join(set(x.split(","))),
@@ -170,18 +170,29 @@
            "hostname": HostCommand(command="hostname", args=["-s"]),
            "fqdn": HostCommand(command="hostname", args=["-f"]),
        }
     will return:
        {  "hostname": "<result of 'hostname -s' command>",
           "fqdn": "<result of 'hostname -f' command>",
        }
+
+    If a command does not exist, the output will be:
+         {"<command>": "Command not found: <command>"}
     """
 
     results = {}
     for name, command in commands.items():
+        # test if command exists
+        try:
+            local.which(
+                command.command
+            )  # throws plumbum.commands.CommandNotFound if not found
+        except CommandNotFound as e:
+            results[name] = f"Command not found: {e}"
+            continue
         results[name] = local[command.command](*command.parameters)
         results[name] = command.default_processing_function(results[name])
         if command.output_processing:
             for func in command.output_processing:
                 results[name] = func(results[name])
 
     return results
```

### Comparing `dice_lib-2024.1.1/src/dice_lib/ranges.py` & `dice_lib-2024.4.1/src/dice_lib/ranges.py`

 * *Files identical despite different names*

### Comparing `dice_lib-2024.1.1/src/dice_lib/units.py` & `dice_lib-2024.4.1/src/dice_lib/units.py`

 * *Files identical despite different names*

### Comparing `dice_lib-2024.1.1/src/dice_lib/user.py` & `dice_lib-2024.4.1/src/dice_lib/user.py`

 * *Files identical despite different names*

### Comparing `dice_lib-2024.1.1/src/dice_lib/fs/__init__.py` & `dice_lib-2024.4.1/src/dice_lib/fs/__init__.py`

 * *Files identical despite different names*

### Comparing `dice_lib-2024.1.1/src/dice_lib/fs/_base.py` & `dice_lib-2024.4.1/src/dice_lib/fs/_base.py`

 * *Files identical despite different names*

### Comparing `dice_lib-2024.1.1/src/dice_lib/fs/_hdfs.py` & `dice_lib-2024.4.1/src/dice_lib/fs/_hdfs.py`

 * *Files identical despite different names*

### Comparing `dice_lib-2024.1.1/src/dice_lib/fs/_posix.py` & `dice_lib-2024.4.1/src/dice_lib/fs/_posix.py`

 * *Files identical despite different names*

### Comparing `dice_lib-2024.1.1/src/dice_lib/health/apel_accounting.py` & `dice_lib-2024.4.1/src/dice_lib/health/apel_accounting.py`

 * *Files identical despite different names*

### Comparing `dice_lib-2024.1.1/tests/test_config.py` & `dice_lib-2024.4.1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `dice_lib-2024.1.1/tests/data/config.yaml` & `dice_lib-2024.4.1/tests/data/config.yaml`

 * *Files identical despite different names*

### Comparing `dice_lib-2024.1.1/tests/fs/test_generic.py` & `dice_lib-2024.4.1/tests/fs/test_generic.py`

 * *Files identical despite different names*

### Comparing `dice_lib-2024.1.1/.gitignore` & `dice_lib-2024.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `dice_lib-2024.1.1/LICENSE` & `dice_lib-2024.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dice_lib-2024.1.1/README.md` & `dice_lib-2024.4.1/README.md`

 * *Files identical despite different names*

### Comparing `dice_lib-2024.1.1/pyproject.toml` & `dice_lib-2024.4.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -23,35 +23,34 @@
     "Topic :: Scientific/Engineering",
     "Intended Audience :: Science/Research",
     "Intended Audience :: Developers",
     "Operating System :: OS Independent",
     "License :: OSI Approved :: BSD License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.7",
-    "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Development Status :: 4 - Beta",
 ]
 
 
 dynamic = ["version"]
 dependencies = [
     "beautifulsoup4 < 5",
     "dnspython>=2.2.0",
     "fasthep-logging",
     "htcondor>=23",
     "omegaconf>=2.1.2",
     "pandas",
     "paramiko",
     "plumbum",
+    "pyarrow",
     "pydantic",
     "pyhdfs",
-    "typing_extensions >=3.7; python_version<'3.8'",
 ]
 
 [project.optional-dependencies]
 test = [
     "pytest >=6",
     "pytest-cov >=3",
 ]
```

### Comparing `dice_lib-2024.1.1/PKG-INFO` & `dice_lib-2024.4.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: dice_lib
-Version: 2024.1.1
+Version: 2024.4.1
 Summary: Python Library for DICE
 Project-URL: homepage, https://github.com/uobdic/dice-lib
 Project-URL: Bug Tracker, https://github.com/uobdic/dice-lib/issues
 Project-URL: Discussions, https://github.com/uobdic/dice-lib/discussions
 Project-URL: Changelog, https://github.com/uobdic/dice-lib/releases
 Author-email: UoB DICE team <lcg-admin@bristol.ac.uk>
 Maintainer-email: The UoB DICE Team <lcg-admin@bristol.ac.uk>
@@ -41,31 +41,30 @@
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.6
 Requires-Dist: beautifulsoup4<5
 Requires-Dist: dnspython>=2.2.0
 Requires-Dist: fasthep-logging
 Requires-Dist: htcondor>=23
 Requires-Dist: omegaconf>=2.1.2
 Requires-Dist: pandas
 Requires-Dist: paramiko
 Requires-Dist: plumbum
+Requires-Dist: pyarrow
 Requires-Dist: pydantic
 Requires-Dist: pyhdfs
-Requires-Dist: typing-extensions>=3.7; python_version < '3.8'
 Provides-Extra: dev
 Requires-Dist: pytest-cov>=3; extra == 'dev'
 Requires-Dist: pytest>=6; extra == 'dev'
 Provides-Extra: docs
 Requires-Dist: furo>=2023.08.17; extra == 'docs'
 Requires-Dist: myst-parser>=0.13; extra == 'docs'
 Requires-Dist: sphinx-autodoc-typehints; extra == 'docs'
```

