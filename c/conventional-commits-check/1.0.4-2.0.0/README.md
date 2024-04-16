# Comparing `tmp/conventional-commits-check-1.0.4.tar.gz` & `tmp/conventional_commits_check-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "conventional-commits-check-1.0.4.tar", last modified: Thu Jun 15 11:04:43 2023, max compression
+gzip compressed data, was "conventional_commits_check-2.0.0.tar", last modified: Tue Apr 16 21:36:16 2024, max compression
```

## Comparing `conventional-commits-check-1.0.4.tar` & `conventional_commits_check-2.0.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 aliyaman   (501) staff       (20)        0 2023-06-15 11:04:43.724404 conventional-commits-check-1.0.4/
--rw-r--r--   0 aliyaman   (501) staff       (20)     1066 2023-03-26 21:03:56.000000 conventional-commits-check-1.0.4/LICENSE
--rw-r--r--   0 aliyaman   (501) staff       (20)     4064 2023-06-15 11:04:43.724263 conventional-commits-check-1.0.4/PKG-INFO
--rw-r--r--   0 aliyaman   (501) staff       (20)     2880 2023-06-15 11:03:59.000000 conventional-commits-check-1.0.4/README.md
-drwxr-xr-x   0 aliyaman   (501) staff       (20)        0 2023-06-15 11:04:43.723145 conventional-commits-check-1.0.4/conventional_commits_check/
--rw-r--r--   0 aliyaman   (501) staff       (20)        0 2023-03-27 22:33:22.000000 conventional-commits-check-1.0.4/conventional_commits_check/__init__.py
--rw-r--r--   0 aliyaman   (501) staff       (20)     2352 2023-06-15 11:01:14.000000 conventional-commits-check-1.0.4/conventional_commits_check/main.py
-drwxr-xr-x   0 aliyaman   (501) staff       (20)        0 2023-06-15 11:04:43.724083 conventional-commits-check-1.0.4/conventional_commits_check.egg-info/
--rw-r--r--   0 aliyaman   (501) staff       (20)     4064 2023-06-15 11:04:43.000000 conventional-commits-check-1.0.4/conventional_commits_check.egg-info/PKG-INFO
--rw-r--r--   0 aliyaman   (501) staff       (20)      402 2023-06-15 11:04:43.000000 conventional-commits-check-1.0.4/conventional_commits_check.egg-info/SOURCES.txt
--rw-r--r--   0 aliyaman   (501) staff       (20)        1 2023-06-15 11:04:43.000000 conventional-commits-check-1.0.4/conventional_commits_check.egg-info/dependency_links.txt
--rw-r--r--   0 aliyaman   (501) staff       (20)       84 2023-06-15 11:04:43.000000 conventional-commits-check-1.0.4/conventional_commits_check.egg-info/entry_points.txt
--rw-r--r--   0 aliyaman   (501) staff       (20)       11 2023-06-15 11:04:43.000000 conventional-commits-check-1.0.4/conventional_commits_check.egg-info/requires.txt
--rw-r--r--   0 aliyaman   (501) staff       (20)       27 2023-06-15 11:04:43.000000 conventional-commits-check-1.0.4/conventional_commits_check.egg-info/top_level.txt
--rw-r--r--   0 aliyaman   (501) staff       (20)       38 2023-06-15 11:04:43.724447 conventional-commits-check-1.0.4/setup.cfg
--rw-r--r--   0 aliyaman   (501) staff       (20)     1640 2023-06-15 11:04:08.000000 conventional-commits-check-1.0.4/setup.py
+drwxr-xr-x   0 aliymn     (501) staff       (20)        0 2024-04-16 21:36:16.788059 conventional_commits_check-2.0.0/
+-rw-r--r--   0 aliymn     (501) staff       (20)     1066 2024-04-13 19:29:03.000000 conventional_commits_check-2.0.0/LICENSE
+-rw-r--r--   0 aliymn     (501) staff       (20)     4134 2024-04-16 21:36:16.787813 conventional_commits_check-2.0.0/PKG-INFO
+-rw-r--r--   0 aliymn     (501) staff       (20)     2925 2024-04-16 21:31:09.000000 conventional_commits_check-2.0.0/README.md
+drwxr-xr-x   0 aliymn     (501) staff       (20)        0 2024-04-16 21:36:16.786659 conventional_commits_check-2.0.0/conventional_commits_check/
+-rw-r--r--   0 aliymn     (501) staff       (20)        0 2024-04-13 19:29:03.000000 conventional_commits_check-2.0.0/conventional_commits_check/__init__.py
+-rw-r--r--   0 aliymn     (501) staff       (20)     2523 2024-04-16 21:33:18.000000 conventional_commits_check-2.0.0/conventional_commits_check/main.py
+drwxr-xr-x   0 aliymn     (501) staff       (20)        0 2024-04-16 21:36:16.787598 conventional_commits_check-2.0.0/conventional_commits_check.egg-info/
+-rw-r--r--   0 aliymn     (501) staff       (20)     4134 2024-04-16 21:36:16.000000 conventional_commits_check-2.0.0/conventional_commits_check.egg-info/PKG-INFO
+-rw-r--r--   0 aliymn     (501) staff       (20)      402 2024-04-16 21:36:16.000000 conventional_commits_check-2.0.0/conventional_commits_check.egg-info/SOURCES.txt
+-rw-r--r--   0 aliymn     (501) staff       (20)        1 2024-04-16 21:36:16.000000 conventional_commits_check-2.0.0/conventional_commits_check.egg-info/dependency_links.txt
+-rw-r--r--   0 aliymn     (501) staff       (20)       84 2024-04-16 21:36:16.000000 conventional_commits_check-2.0.0/conventional_commits_check.egg-info/entry_points.txt
+-rw-r--r--   0 aliymn     (501) staff       (20)       11 2024-04-16 21:36:16.000000 conventional_commits_check-2.0.0/conventional_commits_check.egg-info/requires.txt
+-rw-r--r--   0 aliymn     (501) staff       (20)       27 2024-04-16 21:36:16.000000 conventional_commits_check-2.0.0/conventional_commits_check.egg-info/top_level.txt
+-rw-r--r--   0 aliymn     (501) staff       (20)       38 2024-04-16 21:36:16.788107 conventional_commits_check-2.0.0/setup.cfg
+-rw-r--r--   0 aliymn     (501) staff       (20)     1640 2024-04-16 21:28:44.000000 conventional_commits_check-2.0.0/setup.py
```

### Comparing `conventional-commits-check-1.0.4/LICENSE` & `conventional_commits_check-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `conventional-commits-check-1.0.4/PKG-INFO` & `conventional_commits_check-2.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conventional-commits-check
-Version: 1.0.4
+Version: 2.0.0
 Summary: A pre-commit hook to check Conventional Commits and add emojis.
 Home-page: https://github.com/AliYmn/conventional-commits-check
 Author: Ali Yaman
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
@@ -21,14 +21,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pre-commit
 
 # Conventional Commits Check
 
 <img src="https://raw.githubusercontent.com/AliYmn/conventional-commits-check/master/images/result.png">
 
 `conventional-commits-check` is a Python pre-commit hook that enforces Conventional Commits rules on your commit messages and automatically adds relevant emojis based on the commit type.
 
@@ -53,20 +54,20 @@
     "revert": "⏪",
 }
 ```
 
 # Customization
 
 ```bash
-touch conventional_commits_check_config.yaml
+touch commits_check_config.yaml.yaml
 ````
 
 `NOTE` : Please do not leave it blank if you create it.
 
-To add custom commit types and emojis, update your `conventional_commits_check_config.yaml` file with the additional_commands and additional_emojis fields. Here's an example:
+To add custom commit types and emojis, update your `commits_check_config.yaml` file with the additional_commands and additional_emojis fields. Here's an example:
 
 ```yaml
 additional_commands:
   database: "^database(\\(.+\\))?:"
   design: "^design(\\(.+\\))?:"
 
 additional_emojis:
@@ -103,14 +104,15 @@
 ```yaml
 repos:
   - repo: https://github.com/AliYmn/conventional-commits-check
     rev: v0.3.0  # Use the latest release version
     hooks:
       - id: conventional-commits-check
         stages: [commit-msg]
+    args: ["--emoji-disabled"] # Add this argument to disable emojis
 ```
 
 2. Update the pre-commit hooks in your project:
 
 
 ```bash
 pre-commit install --hook-type commit-msg -f
@@ -127,8 +129,8 @@
 
 ```bash
 pre-commit autoupdate
 ```
 
 # Usage
 
-Once the hook is added to your project, it will automatically run every time you create a commit. The hook will check the commit messages according to the Conventional Commits rules and add the corresponding emojis. If a commit message does not follow the rules, the commit will be blocked.
+Once the hook is added to your project, it will automatically run every time you create a commit. The hook will check the commit messages according to the Conventional Commits rules and add corresponding emojis. If a commit message does not follow the rules, the commit will be blocked.
```

### Comparing `conventional-commits-check-1.0.4/README.md` & `conventional_commits_check-2.0.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -25,20 +25,20 @@
     "revert": "⏪",
 }
 ```
 
 # Customization
 
 ```bash
-touch conventional_commits_check_config.yaml
+touch commits_check_config.yaml.yaml
 ````
 
 `NOTE` : Please do not leave it blank if you create it.
 
-To add custom commit types and emojis, update your `conventional_commits_check_config.yaml` file with the additional_commands and additional_emojis fields. Here's an example:
+To add custom commit types and emojis, update your `commits_check_config.yaml` file with the additional_commands and additional_emojis fields. Here's an example:
 
 ```yaml
 additional_commands:
   database: "^database(\\(.+\\))?:"
   design: "^design(\\(.+\\))?:"
 
 additional_emojis:
@@ -75,14 +75,15 @@
 ```yaml
 repos:
   - repo: https://github.com/AliYmn/conventional-commits-check
     rev: v0.3.0  # Use the latest release version
     hooks:
       - id: conventional-commits-check
         stages: [commit-msg]
+    args: ["--emoji-disabled"] # Add this argument to disable emojis
 ```
 
 2. Update the pre-commit hooks in your project:
 
 
 ```bash
 pre-commit install --hook-type commit-msg -f
@@ -99,8 +100,8 @@
 
 ```bash
 pre-commit autoupdate
 ```
 
 # Usage
 
-Once the hook is added to your project, it will automatically run every time you create a commit. The hook will check the commit messages according to the Conventional Commits rules and add the corresponding emojis. If a commit message does not follow the rules, the commit will be blocked.
+Once the hook is added to your project, it will automatically run every time you create a commit. The hook will check the commit messages according to the Conventional Commits rules and add corresponding emojis. If a commit message does not follow the rules, the commit will be blocked.
```

### Comparing `conventional-commits-check-1.0.4/conventional_commits_check/main.py` & `conventional_commits_check-2.0.0/conventional_commits_check/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 #!/usr/bin/env python3
 import argparse
 import re
 import sys
-from typing import Dict
 import yaml
 import os
 
 COMMIT_TYPES = {
     "feat": "^feat(\(.+\))?:",
     "fix": "^fix(\(.+\))?:",
     "docs": "^docs(\(.+\))?:",
@@ -39,52 +38,58 @@
 def load_custom_rules(config_file="commits_check_config.yaml"):
     config_path = os.path.join(os.getcwd(), config_file)
 
     try:
         with open(config_path, "r") as file:
             config_data = yaml.safe_load(file)
 
-        return config_data.get("additional_commands", {}), config_data.get("additional_emojis", {})
+        return config_data.get("additional_commands", {}), config_data.get(
+            "additional_emojis", {}
+        )
 
     except FileNotFoundError:
         print(
-            f"No such file or directory: '{config_path}'. Please make sure the config file is in the correct directory.")
+            f"💥 No such file or directory: '{config_path}'. Please make sure the config file is in the correct directory."
+        )
         sys.exit(1)
 
 
 def main():
     additional_commands, additional_emojis = load_custom_rules()
 
     # Merge additional commands and emojis with the existing ones
     COMMIT_TYPES.update(additional_commands)
     EMOJIS.update(additional_emojis)
 
     parser = argparse.ArgumentParser()
     parser.add_argument("commit_message_file")
+    parser.add_argument("--emoji-disabled", action="store_true", help="Disable emojis in commit messages")
     args = parser.parse_args()
 
     with open(args.commit_message_file, "r") as file:
         commit_message = file.read()
 
     commit_type = None
     for commit, pattern in COMMIT_TYPES.items():
         if re.match(pattern, commit_message.strip()):
             commit_type = commit
             break
 
     if not commit_type:
-        print("Commit message does not follow Conventional Commits rules.")
+        print("💥 Commit message does not follow Conventional Commits rules.")
         sys.exit(1)
 
     emoji = EMOJIS.get(commit_type)
 
-    if emoji:
+    if emoji and not args.emoji_disabled:
         new_commit_message = f"{emoji} {commit_message}"
         with open(args.commit_message_file, "w") as file:
             file.write(new_commit_message)
 
-    print("Commit message follows Conventional Commits rules and has been updated with an emoji.")
+    print(
+        "🎉 Commit message follows Conventional Commits rules and has been updated with an emoji."
+    )
     sys.exit(0)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `conventional-commits-check-1.0.4/conventional_commits_check.egg-info/PKG-INFO` & `conventional_commits_check-2.0.0/conventional_commits_check.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conventional-commits-check
-Version: 1.0.4
+Version: 2.0.0
 Summary: A pre-commit hook to check Conventional Commits and add emojis.
 Home-page: https://github.com/AliYmn/conventional-commits-check
 Author: Ali Yaman
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
@@ -21,14 +21,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pre-commit
 
 # Conventional Commits Check
 
 <img src="https://raw.githubusercontent.com/AliYmn/conventional-commits-check/master/images/result.png">
 
 `conventional-commits-check` is a Python pre-commit hook that enforces Conventional Commits rules on your commit messages and automatically adds relevant emojis based on the commit type.
 
@@ -53,20 +54,20 @@
     "revert": "⏪",
 }
 ```
 
 # Customization
 
 ```bash
-touch conventional_commits_check_config.yaml
+touch commits_check_config.yaml.yaml
 ````
 
 `NOTE` : Please do not leave it blank if you create it.
 
-To add custom commit types and emojis, update your `conventional_commits_check_config.yaml` file with the additional_commands and additional_emojis fields. Here's an example:
+To add custom commit types and emojis, update your `commits_check_config.yaml` file with the additional_commands and additional_emojis fields. Here's an example:
 
 ```yaml
 additional_commands:
   database: "^database(\\(.+\\))?:"
   design: "^design(\\(.+\\))?:"
 
 additional_emojis:
@@ -103,14 +104,15 @@
 ```yaml
 repos:
   - repo: https://github.com/AliYmn/conventional-commits-check
     rev: v0.3.0  # Use the latest release version
     hooks:
       - id: conventional-commits-check
         stages: [commit-msg]
+    args: ["--emoji-disabled"] # Add this argument to disable emojis
 ```
 
 2. Update the pre-commit hooks in your project:
 
 
 ```bash
 pre-commit install --hook-type commit-msg -f
@@ -127,8 +129,8 @@
 
 ```bash
 pre-commit autoupdate
 ```
 
 # Usage
 
-Once the hook is added to your project, it will automatically run every time you create a commit. The hook will check the commit messages according to the Conventional Commits rules and add the corresponding emojis. If a commit message does not follow the rules, the commit will be blocked.
+Once the hook is added to your project, it will automatically run every time you create a commit. The hook will check the commit messages according to the Conventional Commits rules and add corresponding emojis. If a commit message does not follow the rules, the commit will be blocked.
```

### Comparing `conventional-commits-check-1.0.4/setup.py` & `conventional_commits_check-2.0.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
         README = f.read()
 else:
     with open('README.md', encoding='utf-8') as f:
         README = f.read()
 
 setup(
     name="conventional-commits-check",
-    version="1.0.4",
+    version="2.0.0",
     description="A pre-commit hook to check Conventional Commits and add emojis.",
     author="Ali Yaman",
     packages=find_packages(),
     license="MIT",
     long_description_content_type="text/markdown",
     long_description=README,
     url="https://github.com/AliYmn/conventional-commits-check",
```

