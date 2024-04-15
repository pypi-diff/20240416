# Comparing `tmp/qstress-0.3.2.tar.gz` & `tmp/qstress-0.3.3.tar.gz`

## Comparing `qstress-0.3.2.tar` & `qstress-0.3.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 qstress-0.3.2/src/qstress/__about__.py
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 qstress-0.3.2/src/qstress/cache.py
--rw-r--r--   0        0        0     6790 2020-02-02 00:00:00.000000 qstress-0.3.2/src/qstress/cli.py
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 qstress-0.3.2/src/qstress/config.py
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 qstress-0.3.2/src/qstress/globals.py
--rw-r--r--   0        0        0     1335 2020-02-02 00:00:00.000000 qstress-0.3.2/src/qstress/util.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 qstress-0.3.2/.gitignore
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 qstress-0.3.2/LICENSE.txt
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 qstress-0.3.2/README.md
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 qstress-0.3.2/pyproject.toml
--rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 qstress-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 qstress-0.3.3/src/qstress/__about__.py
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 qstress-0.3.3/src/qstress/cache.py
+-rw-r--r--   0        0        0     6790 2020-02-02 00:00:00.000000 qstress-0.3.3/src/qstress/cli.py
+-rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 qstress-0.3.3/src/qstress/config.py
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 qstress-0.3.3/src/qstress/globals.py
+-rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 qstress-0.3.3/src/qstress/util.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 qstress-0.3.3/.gitignore
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 qstress-0.3.3/LICENSE.txt
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 qstress-0.3.3/README.md
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 qstress-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 qstress-0.3.3/PKG-INFO
```

### Comparing `qstress-0.3.2/src/qstress/cache.py` & `qstress-0.3.3/src/qstress/cache.py`

 * *Files identical despite different names*

### Comparing `qstress-0.3.2/src/qstress/cli.py` & `qstress-0.3.3/src/qstress/cli.py`

 * *Files identical despite different names*

### Comparing `qstress-0.3.2/src/qstress/config.py` & `qstress-0.3.3/src/qstress/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 import typing
 
 from .globals import qstress_path
 
 default_config = {
-    "compilerBin": "g++", "compileFlags": ["-O2", "-std=c++17"], "tests": 200, "find": 1,
+    "compilerBin": "g++", "compileArgs": ["-O2", "-std=c++17"], "tests": 200, "find": 1,
     "folder": "test_cases"
 }
 
 def get_config() -> dict[str, typing.Any]:
 
     config_path = qstress_path / "config.json"
```

### Comparing `qstress-0.3.2/src/qstress/globals.py` & `qstress-0.3.3/src/qstress/globals.py`

 * *Files identical despite different names*

### Comparing `qstress-0.3.2/src/qstress/util.py` & `qstress-0.3.3/src/qstress/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     cur_hash = hash_file(source_path)
 
     if cur_hash == global_cache[target]:
         console.print(f"Used cached [bold]{source_file}[/]")
         return True
 
     process = subprocess.run(
-        [shutil.which(global_config["compilerBin"])] + global_config["compileFlags"] +
+        [shutil.which(global_config["compilerBin"])] + global_config["compileArgs"] +
         [str(source_path), "-o", str(get_path("bin", target))]
     )
 
     if process.returncode:
         console.print()
         console.print(f"[red]Failed to compile [bold]{source_file}[/][/]")
         return False
```

### Comparing `qstress-0.3.2/LICENSE.txt` & `qstress-0.3.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qstress-0.3.2/pyproject.toml` & `qstress-0.3.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `qstress-0.3.2/PKG-INFO` & `qstress-0.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: qstress
-Version: 0.3.2
+Version: 0.3.3
 Summary: A simple tool for stress testing.
 Project-URL: Documentation, https://github.com/GMbrianlaw/qstress#readme
 Project-URL: Issues, https://github.com/GMbrianlaw/qstress/issues
 Project-URL: Source, https://github.com/GMbrianlaw/qstress
 Author-email: Brian Law <gmbrianlaw@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
```

