# Comparing `tmp/depends-on-0.15.0.tar.gz` & `tmp/depends-on-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "depends-on-0.15.0.tar", last modified: Tue Apr 16 09:38:34 2024, max compression
+gzip compressed data, was "depends-on-0.9.0.tar", last modified: Mon Nov 13 11:06:48 2023, max compression
```

## Comparing `depends-on-0.15.0.tar` & `depends-on-0.9.0.tar`

### file list

```diff
@@ -1,23 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:38:34.244754 depends-on-0.15.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-16 09:38:33.000000 depends-on-0.15.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-16 09:38:33.000000 depends-on-0.15.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9269 2024-04-16 09:38:34.244754 depends-on-0.15.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8636 2024-04-16 09:38:33.000000 depends-on-0.15.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:38:34.244754 depends-on-0.15.0/depends_on/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 09:38:33.000000 depends-on-0.15.0/depends_on/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-04-16 09:38:33.000000 depends-on-0.15.0/depends_on/ansible.py
--rw-r--r--   0 runner    (1001) docker     (127)    13116 2024-04-16 09:38:33.000000 depends-on-0.15.0/depends_on/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-04-16 09:38:33.000000 depends-on-0.15.0/depends_on/golang.py
--rw-r--r--   0 runner    (1001) docker     (127)     4362 2024-04-16 09:38:33.000000 depends-on-0.15.0/depends_on/javascript.py
--rw-r--r--   0 runner    (1001) docker     (127)     5164 2024-04-16 09:38:33.000000 depends-on-0.15.0/depends_on/python.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:38:34.244754 depends-on-0.15.0/depends_on.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9269 2024-04-16 09:38:34.000000 depends-on-0.15.0/depends_on.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-16 09:38:34.000000 depends-on-0.15.0/depends_on.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 09:38:34.000000 depends-on-0.15.0/depends_on.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-16 09:38:34.000000 depends-on-0.15.0/depends_on.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1160 2024-04-16 09:38:33.000000 depends-on-0.15.0/depends_on_stage1
--rwxr-xr-x   0 runner    (1001) docker     (127)     4904 2024-04-16 09:38:33.000000 depends-on-0.15.0/depends_on_stage2
--rwxr-xr-x   0 runner    (1001) docker     (127)     3064 2024-04-16 09:38:33.000000 depends-on-0.15.0/depends_on_stage3
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-16 09:38:33.000000 depends-on-0.15.0/package.json
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 09:38:34.244754 depends-on-0.15.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-16 09:38:33.000000 depends-on-0.15.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 11:06:48.875347 depends-on-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2023-11-13 11:06:48.000000 depends-on-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2023-11-13 11:06:48.000000 depends-on-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6048 2023-11-13 11:06:48.875347 depends-on-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5416 2023-11-13 11:06:48.000000 depends-on-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 11:06:48.875347 depends-on-0.9.0/depends_on/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-13 11:06:48.000000 depends-on-0.9.0/depends_on/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1939 2023-11-13 11:06:48.000000 depends-on-0.9.0/depends_on/golang.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4743 2023-11-13 11:06:48.000000 depends-on-0.9.0/depends_on/javascript.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5535 2023-11-13 11:06:48.000000 depends-on-0.9.0/depends_on/python.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 11:06:48.875347 depends-on-0.9.0/depends_on.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6048 2023-11-13 11:06:48.000000 depends-on-0.9.0/depends_on.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2023-11-13 11:06:48.000000 depends-on-0.9.0/depends_on.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-13 11:06:48.000000 depends-on-0.9.0/depends_on.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2023-11-13 11:06:48.000000 depends-on-0.9.0/depends_on.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5781 2023-11-13 11:06:48.000000 depends-on-0.9.0/depends_on_stage2
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2816 2023-11-13 11:06:48.000000 depends-on-0.9.0/depends_on_stage3
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2023-11-13 11:06:48.000000 depends-on-0.9.0/package.json
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-13 11:06:48.875347 depends-on-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2023-11-13 11:06:48.000000 depends-on-0.9.0/setup.py
```

### Comparing `depends-on-0.15.0/LICENSE` & `depends-on-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `depends-on-0.15.0/depends_on/golang.py` & `depends-on-0.9.0/depends_on/golang.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 "golang specific code for stage 3."
 
 import os
 import re
-
-from depends_on.common import log
+import sys
 
 
 def process_golang(main_dir, dirs, container_mode):
     "Add replace directives in go.mod for the local dependencies."
     go_mod = os.path.join(main_dir, "go.mod")
     if not os.path.exists(go_mod):
         return False
-    log(f"processing {go_mod}")
     # get the list of github.com/... dependencies that are in the local dependencies
     github_mods = []
     with open(go_mod, "r", encoding="UTF-8") as in_stream:
         for line in in_stream.readlines():
             match = re.match(r"^(require)?\s*(github.com/.*?)\s", line)
             if match and match.group(2) in dirs:
                 github_mods.append(match.group(2))
@@ -26,23 +24,25 @@
             if container_mode:
                 # remove https:// at the beginning of the url and .git at the end
                 fork_url = (
                     dirs[mod]["fork_url"]
                     .replace("https://", "", 1)
                     .replace(".git", "", 1)
                 )
-                log(
-                    f'Adding replace directive in go.mod for {mod} => {fork_url} {dirs[mod]["branch"]}'
+                print(
+                    f'Adding replace directive in go.mod for {mod} => {fork_url} {dirs[mod]["branch"]}',
+                    file=sys.stderr,
                 )
                 os.system(
                     f"set -x; go mod edit -replace {mod}={fork_url}@{dirs[mod]['branch']}"
                 )
             else:
-                log(
-                    f'Adding replace directive in go.mod for {mod} => {dirs[mod]["path"]}'
+                print(
+                    f'Adding replace directive in go.mod for {mod} => {dirs[mod]["path"]}',
+                    file=sys.stderr,
                 )
                 os.system(f"set -x; go mod edit -replace {mod}={dirs[mod]['path']}")
             nb_replace += 1
     # if there is any change to go.mod, `go mod tidy` needs to be called to have a correct go.sums
     if nb_replace > 0:
         os.system("set -x; go mod tidy")
     return nb_replace > 0
```

### Comparing `depends-on-0.15.0/depends_on/javascript.py` & `depends-on-0.9.0/depends_on/javascript.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 "javascript specific code for stage 3."
 
 import glob
 import json
 import os
-
-from depends_on.common import log
+import sys
 
 
 def load_package_json(package_json_path):
     """Load package.json file."""
     with open(package_json_path, "r", encoding="UTF-8") as package_json:
         return json.load(package_json)
 
@@ -25,69 +24,79 @@
         else:
             local_path = dirs[local_dir]["path"]
         package_json_path = os.path.join(local_path, "package.json")
         if os.path.exists(package_json_path):
             package = load_package_json(package_json_path)
             deps[package["name"]] = dirs[local_dir]
             if "workspaces" in package and "packages" in package["workspaces"]:
-                log("detected workspaces")
+                print("detected workspaces", file=sys.stderr)
                 for workspace_glob in package["workspaces"]["packages"]:
-                    log(f"processing {workspace_glob}")
+                    print(f"processing {workspace_glob}", file=sys.stderr)
                     for workspace_dir in glob.glob(
                         os.path.join(local_path, workspace_glob)
                     ):
-                        log(f"found subdir={workspace_dir}")
+                        print(f"found subdir={workspace_dir}", file=sys.stderr)
                         workspace_path = os.path.join(local_path, workspace_dir)
-                        log(f"checking workspace {workspace_path} for package.json")
+                        print(
+                            f"checking workspace {workspace_path} for package.json",
+                            file=sys.stderr,
+                        )
                         workspace_package_json_path = os.path.join(
                             workspace_path, "package.json"
                         )
                         if os.path.exists(workspace_package_json_path):
                             workspace_package = load_package_json(
                                 workspace_package_json_path
                             )
-                            log(f"found package {workspace_package['name']}")
+                            print(
+                                f"found package {workspace_package['name']}",
+                                file=sys.stderr,
+                            )
                             deps[workspace_package["name"]] = {
                                 "path": workspace_path,
                                 "subdir": workspace_dir[len(local_path) + 1 :],
                                 "fork_url": dirs[local_dir]["fork_url"],
                                 "branch": dirs[local_dir]["branch"],
                             }
     return deps
 
 
 def process_dependencies(dependencies, dirs, container_mode, package_json_path):
     """Process dependencies in package.json and replace local dependencies"""
     local_deps = local_dependencies(dirs)
-    log(f"Found {len(local_deps)} local dependencies: {local_deps=}")
+    print(f"Found {len(local_deps)} local dependencies: {local_deps=}", file=sys.stderr)
     count = 0
     for dependency in dependencies:
         if dependency in local_deps:
             if container_mode:
                 info = local_deps[dependency]
                 repo = "git+" + info["fork_url"] + "#" + info["branch"]
-                log(
-                    f"Replacing {dependency} with remote version from {repo} in package.json"
+                print(
+                    f"Replacing {dependency} with remote version from {repo} in package.json",
+                    file=sys.stderr,
                 )
                 dependencies[dependency] = repo
             else:
-                log(
-                    f"Replacing {dependency} with local version from {local_deps[dependency]['path']} in package.json"
+                print(
+                    f"Replacing {dependency} with local version from {local_deps[dependency]['path']} in package.json",
+                    file=sys.stderr,
                 )
                 dependencies[dependency] = "file:" + local_deps[dependency]["path"]
             count += 1
     return count
 
 
 def process_javascript(main_dir, dirs, container_mode):
     """Use changes from PR in package.json if present"""
     package_json_path = os.path.join(main_dir, "package.json")
     if not os.path.exists(package_json_path):
         return False
-    log("Detected package.json file, checking for local dependencies")
+    print(
+        "Detected package.json file, checking for local dependencies", file=sys.stderr
+    )
     package = load_package_json(package_json_path)
     if "dependencies" not in package:
         return False
     dependencies = package["dependencies"]
     count = process_dependencies(dependencies, dirs, container_mode, package_json_path)
     if "devDependencies" in package:
         dependencies = package["devDependencies"]
```

### Comparing `depends-on-0.15.0/depends_on/python.py` & `depends-on-0.9.0/depends_on/python.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 "Python specific code for stage 3."
 
 import os
 import re
-
-from depends_on.common import log
+import sys
 
 
 def lookup_name(fname):
     "Lookup the name of a module"
     if os.path.exists(fname):
-        log(f"Looking up name in {fname}")
+        print(f"Looking up name in {fname}", file=sys.stderr)
         with open(fname, "r", encoding="UTF-8") as in_stream:
             for line in in_stream.readlines():
                 match = re.match(r"^\s*name\s*=\s*['\"](.*?)['\"]\s*,", line)
                 if match:
                     return match.group(1)
     return None
 
@@ -32,17 +31,17 @@
 
 def process_python_requirements(main_dir, dirs, container_mode):
     "Replace modules in requirements.txt for the local dependencies."
     requirements_txt = os.path.join(main_dir, "requirements.txt")
     requirements_txt_new = requirements_txt + ".new"
     if not os.path.exists(requirements_txt):
         return False
-    log("requirements.txt detected")
+    print("requirements.txt detected", file=sys.stderr)
     module_dirs = get_modules(dirs)
-    log(f"{module_dirs=}")
+    print(f"{module_dirs=}", file=sys.stderr)
     # replace the modules in requirements.txt
     nb_replace = 0
     with open(requirements_txt, "r", encoding="UTF-8") as in_stream:
         with open(requirements_txt_new, "w", encoding="UTF-8") as out_stream:
             for line in in_stream.readlines():
                 match = re.match(r"^\s*(\w+)", line)
                 if match and match.group(1) in module_dirs:
@@ -50,19 +49,23 @@
                     if container_mode:
                         # doc at https://pip.pypa.io/en/stable/cli/pip_install/#git
                         pkg = f"{mod} @ git+{module_dirs[mod]['fork_url']}@{module_dirs[mod]['branch']}"
                         if "subdir" in module_dirs[mod]:
                             pkg += (
                                 f"#egg=subdir&subdirectory={module_dirs[mod]['subdir']}"
                             )
-                        log(f"Replacing {mod} in requirements.txt with {pkg}")
+                        print(
+                            f"Replacing {mod} in requirements.txt with {pkg}",
+                            file=sys.stderr,
+                        )
                         out_stream.write(f"{pkg}\n")
                     else:
-                        log(
-                            f"Replacing {mod} in requirements.txt with {module_dirs[mod]['path']}"
+                        print(
+                            f"Replacing {mod} in requirements.txt with {module_dirs[mod]['path']}",
+                            file=sys.stderr,
                         )
                         out_stream.write(f"-e {module_dirs[mod]['path']}\n")
                     nb_replace += 1
                 else:
                     out_stream.write(line)
     os.rename(requirements_txt_new, requirements_txt)
     return nb_replace > 0
@@ -70,18 +73,18 @@
 
 def process_python_pyproject(main_dir, dirs, container_mode):
     "Replace modules in pyproject.toml for the local dependencies."
     pyproject_toml = os.path.join(main_dir, "pyproject.toml")
     pyproject_toml_new = pyproject_toml + ".new"
     if not os.path.exists(pyproject_toml):
         return False
-    log("pyproject.toml detected")
+    print("pyproject.toml detected", file=sys.stderr)
     # get the list of python packages from local dependencies
     module_dirs = get_modules(dirs)
-    log(f"{module_dirs=}")
+    print(f"{module_dirs=}", file=sys.stderr)
     # replace the modules in pyproject.toml
     nb_replace = 0
     with open(pyproject_toml, "r", encoding="UTF-8") as in_stream:
         with open(pyproject_toml_new, "w", encoding="UTF-8") as out_stream:
             for line in in_stream.readlines():
                 match = re.match(r"^\s*(\w+)\s*=", line)
                 if match and match.group(1) in module_dirs:
@@ -91,19 +94,23 @@
                         pkg = f"{mod} = {{ git = \"{module_dirs[mod]['fork_url']}\", branch = \"{module_dirs[mod]['branch']}\""
                         if "subdir" in module_dirs[mod]:
                             pkg += (
                                 f", subdirectory = \"{module_dirs[mod]['subdir']}\" }}"
                             )
                         else:
                             pkg += " }"
-                        log(f"Replacing {mod} in pyproject.toml with {pkg}")
+                        print(
+                            f"Replacing {mod} in pyproject.toml with {pkg}",
+                            file=sys.stderr,
+                        )
                         out_stream.write(f"{pkg}\n")
                     else:
-                        log(
-                            f"Replacing {mod} in pyproject.toml with {module_dirs[mod]['path']}"
+                        print(
+                            f"Replacing {mod} in pyproject.toml with {module_dirs[mod]['path']}",
+                            file=sys.stderr,
                         )
                         out_stream.write(
                             f'{mod} = {{ path = "{module_dirs[mod]["path"]}" }}\n'
                         )
                     nb_replace += 1
                 else:
                     out_stream.write(line)
```

### Comparing `depends-on-0.15.0/depends_on_stage3` & `depends-on-0.9.0/depends_on_stage3`

 * *Files 6% similar despite different names*

```diff
@@ -3,16 +3,14 @@
 """Stage3: inject the local dependencies into the main changeset.
 """
 
 import json
 import os
 import sys
 
-from depends_on.ansible import process_ansible
-from depends_on.common import init_sensitive_strings, log
 from depends_on.golang import process_golang
 from depends_on.javascript import process_javascript
 from depends_on.python import process_python
 
 
 def extract_repo_name(url):
     "Return the repository name from a git URL in the form github.com/<org>/<repo>."
@@ -33,27 +31,27 @@
     return origin_url
 
 
 def directories(top_dir, main_dir):
     """Return a dict of {repo_name: <dict info>} for all git repositories in top_dir.
 
     dict info:
-    - top_dir: the top directory of the repository
+    - topdir: the top directory of the repository
     - path: the path to the module in the repository
     - subdir: the subdirectory of the module in the repository (optional)
     """
     ret = {}
     for d in os.listdir(top_dir):
         key_dir = os.path.join(top_dir, d)
         if (
             os.path.isdir(key_dir)
             and key_dir != main_dir
             and os.path.isdir(os.path.join(key_dir, ".git"))
         ):
-            info = {"top_dir": top_dir, "path": top_dir}
+            info = {"topdir": top_dir, "path": top_dir}
             json_fname = os.path.join(key_dir, "depends-on.json")
             if os.path.exists(json_fname):
                 with open(json_fname, "r") as json_stream:
                     data = json.load(json_stream)
                     info.update(data)
                     if "subdir" in data:
                         info["path"] = os.path.join(key_dir, data["subdir"])
@@ -64,36 +62,29 @@
 def detect_container_mode(main_dir):
     "Return True if main_dir contains a Dockerfile or a Containerfile."
     return os.path.exists(os.path.join(main_dir, "Dockerfile")) or os.path.exists(
         os.path.join(main_dir, "Containerfile")
     )
 
 
-def main(args):
+def main():
     "Main function."
-
-    if len(args) != 2:
-        print(f"Usage: {args[0]} <top dir>", file=sys.stderr)
-        return 1
-
-    init_sensitive_strings()
-
     main_dir = os.getcwd()
-    top_dir = args[1]
+    top_dir = os.path.dirname(main_dir)
 
     dirs = directories(top_dir, main_dir)
-    log(f"{main_dir=} {top_dir=} {dirs=} called from {__file__}!")
+    print(
+        f"{main_dir=} {top_dir=} {dirs=} called from {__file__}!",
+        file=sys.stderr,
+    )
 
     container_mode = detect_container_mode(main_dir)
-    log(f"{container_mode=}")
+    print(f"{container_mode=}", file=sys.stderr)
     process_golang(main_dir, dirs, container_mode)
     process_python(main_dir, dirs, container_mode)
     process_javascript(main_dir, dirs, container_mode)
-    process_ansible(main_dir, dirs, container_mode)
-
-    return 0
 
 
 if __name__ == "__main__":
-    sys.exit(main(sys.argv))
+    sys.exit(main())
 
-# depends_on_stage3 ends here
+# stage3.py ends here
```

### Comparing `depends-on-0.15.0/package.json` & `depends-on-0.9.0/package.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8977272727272727%*

 * *Differences: {"'dependencies'": "{delete: ['npm']}", "'license'": "'GPL-3.0-or-later'", "'version'": "'0.9.0'"}*

```diff
@@ -1,25 +1,24 @@
 {
     "author": "",
     "dependencies": {
         "@actions/core": "^1.10.0",
         "@actions/exec": "^1.1.1",
-        "@actions/github": "^5.1.1",
-        "npm": "^10.5.2"
+        "@actions/github": "^5.1.1"
     },
     "description": "GitHub Action to install dependent Pull Requests",
     "devDependencies": {
         "@vercel/ncc": "^0.36.1"
     },
     "keywords": [],
-    "license": "GPL-3.0",
+    "license": "GPL-3.0-or-later",
     "main": "index.js",
     "name": "depends-on",
     "repository": {
         "type": "git",
         "url": "https://github.com/depends-on/depends-on-action.git"
     },
     "scripts": {
         "build": "ncc build index.js -o dist"
     },
-    "version": "0.15.0"
+    "version": "0.9.0"
 }
```

### Comparing `depends-on-0.15.0/setup.py` & `depends-on-0.9.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,9 +14,9 @@
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Topic :: Software Development :: Version Control :: Git",
         "Topic :: Software Development :: Testing",
         "Topic :: Software Development :: Quality Assurance",
     ],
     version=json.load(open("package.json"))["version"],
     packages=["depends_on"],
-    scripts=["depends_on_stage1", "depends_on_stage2", "depends_on_stage3"],
+    scripts=["depends_on_stage2", "depends_on_stage3"],
 )
```

