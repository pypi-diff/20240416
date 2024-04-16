# Comparing `tmp/kometautils-0.1.0.tar.gz` & `tmp/kometautils-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kometautils-0.1.0.tar", last modified: Tue Apr 16 17:39:13 2024, max compression
+gzip compressed data, was "kometautils-0.2.0.tar", last modified: Tue Apr 16 18:48:44 2024, max compression
```

## Comparing `kometautils-0.1.0.tar` & `kometautils-0.2.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-04-16 17:39:13.707182 kometautils-0.1.0/
--rw-rw-rw-   0        0        0     1088 2024-04-15 18:34:56.000000 kometautils-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     2436 2024-04-16 17:39:13.706178 kometautils-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1283 2024-04-16 17:37:37.000000 kometautils-0.1.0/README.rst
-drwxrwxrwx   0        0        0        0 2024-04-16 17:39:13.691992 kometautils-0.1.0/kometautils/
--rw-rw-rw-   0        0        0      950 2024-04-16 15:15:53.000000 kometautils-0.1.0/kometautils/__init__.py
--rw-rw-rw-   0        0        0     9280 2024-04-15 19:46:42.000000 kometautils-0.1.0/kometautils/args.py
--rw-rw-rw-   0        0        0      387 2023-08-14 18:16:56.000000 kometautils-0.1.0/kometautils/exceptions.py
--rw-rw-rw-   0        0        0    22617 2024-04-15 20:15:21.000000 kometautils-0.1.0/kometautils/logging.py
--rw-rw-rw-   0        0        0    32467 2023-08-14 18:16:56.000000 kometautils-0.1.0/kometautils/schedule.py
--rw-rw-rw-   0        0        0     3798 2024-04-16 15:43:06.000000 kometautils-0.1.0/kometautils/util.py
--rw-rw-rw-   0        0        0     2974 2024-04-15 19:48:17.000000 kometautils-0.1.0/kometautils/yaml.py
-drwxrwxrwx   0        0        0        0 2024-04-16 17:39:13.704126 kometautils-0.1.0/kometautils.egg-info/
--rw-rw-rw-   0        0        0     2436 2024-04-16 17:39:13.000000 kometautils-0.1.0/kometautils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      358 2024-04-16 17:39:13.000000 kometautils-0.1.0/kometautils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-16 17:39:13.000000 kometautils-0.1.0/kometautils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      142 2024-04-16 17:39:13.000000 kometautils-0.1.0/kometautils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-16 17:39:13.000000 kometautils-0.1.0/kometautils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-16 17:39:13.708178 kometautils-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1560 2024-04-15 19:26:19.000000 kometautils-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:48:44.003018 kometautils-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-16 18:48:31.000000 kometautils-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-04-16 18:48:44.003018 kometautils-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-04-16 18:48:31.000000 kometautils-0.2.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:48:44.003018 kometautils-0.2.0/kometautils/
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-04-16 18:48:31.000000 kometautils-0.2.0/kometautils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9019 2024-04-16 18:48:31.000000 kometautils-0.2.0/kometautils/args.py
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-16 18:48:31.000000 kometautils-0.2.0/kometautils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22117 2024-04-16 18:48:31.000000 kometautils-0.2.0/kometautils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31561 2024-04-16 18:48:31.000000 kometautils-0.2.0/kometautils/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3705 2024-04-16 18:48:31.000000 kometautils-0.2.0/kometautils/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2874 2024-04-16 18:48:31.000000 kometautils-0.2.0/kometautils/yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:48:44.003018 kometautils-0.2.0/kometautils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-04-16 18:48:43.000000 kometautils-0.2.0/kometautils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-16 18:48:43.000000 kometautils-0.2.0/kometautils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 18:48:43.000000 kometautils-0.2.0/kometautils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-16 18:48:43.000000 kometautils-0.2.0/kometautils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-16 18:48:43.000000 kometautils-0.2.0/kometautils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 18:48:44.003018 kometautils-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-04-16 18:48:31.000000 kometautils-0.2.0/setup.py
```

### Comparing `kometautils-0.1.0/LICENSE` & `kometautils-0.2.0/LICENSE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2024 meisnate12
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2024 meisnate12
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `kometautils-0.1.0/README.rst` & `kometautils-0.2.0/README.rst`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-Kometa Utils
-==========================================================
-
-.. image:: https://img.shields.io/github/v/release/Kometa-Team/Kometa-Utils?style=plastic
-    :target: https://github.com/Kometa-Team/Kometa-Utils/releases
-    :alt: GitHub release (latest by date)
-
-.. image:: https://img.shields.io/pypi/v/kometa-utils?style=plastic
-    :target: https://pypi.org/project/kometa-utils/
-    :alt: PyPI
-
-.. image:: https://img.shields.io/pypi/dm/kometa-utils.svg?style=plastic
-    :target: https://pypi.org/project/kometa-utils/
-    :alt: Downloads
-
-.. image:: https://img.shields.io/github/commits-since/Kometa-Team/Kometa-Utils/latest?style=plastic
-    :target: https://github.com/Kometa-Team/Kometa-Utils/commits/master
-    :alt: GitHub commits since latest release (by date) for a branch
-
-.. image:: https://img.shields.io/badge/-Sponsor_or_Donate-blueviolet?style=plastic
-    :target: https://github.com/sponsors/meisnate12
-    :alt: GitHub Sponsor
-
-Overview
-----------------------------------------------------------
-
-Common Utility Methods and Modules used by Kometa and Kometa Partner Scripts
-
-
-Installation & Documentation
-----------------------------------------------------------
-
-.. code-block:: python
-
-    pip install kometautils
+Kometa Utils
+==========================================================
+
+.. image:: https://img.shields.io/github/v/release/Kometa-Team/Kometa-Utils?style=plastic
+    :target: https://github.com/Kometa-Team/Kometa-Utils/releases
+    :alt: GitHub release (latest by date)
+
+.. image:: https://img.shields.io/pypi/v/kometa-utils?style=plastic
+    :target: https://pypi.org/project/kometa-utils/
+    :alt: PyPI
+
+.. image:: https://img.shields.io/pypi/dm/kometa-utils.svg?style=plastic
+    :target: https://pypi.org/project/kometa-utils/
+    :alt: Downloads
+
+.. image:: https://img.shields.io/github/commits-since/Kometa-Team/Kometa-Utils/latest?style=plastic
+    :target: https://github.com/Kometa-Team/Kometa-Utils/commits/master
+    :alt: GitHub commits since latest release (by date) for a branch
+
+.. image:: https://img.shields.io/badge/-Sponsor_or_Donate-blueviolet?style=plastic
+    :target: https://github.com/sponsors/meisnate12
+    :alt: GitHub Sponsor
+
+Overview
+----------------------------------------------------------
+
+Common Utility Methods and Modules used by Kometa and Kometa Partner Scripts
+
+
+Installation & Documentation
+----------------------------------------------------------
+
+.. code-block:: python
+
+    pip install kometautils
```

### Comparing `kometautils-0.1.0/kometautils/__init__.py` & `kometautils-0.2.0/kometautils/__init__.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-from importlib.metadata import version, PackageNotFoundError
-from . import util
-from .logging import KometaLogger
-from .args import KometaArgs, Version
-from .exceptions import Continue, Deleted, Failed, FilterFailed, LimitReached, NonExisting, NotScheduled, NotScheduledRange, TimeoutExpired
-
-
-try:
-    __version__ = version("kometautils")
-except PackageNotFoundError:
-    __version__ = ""
-
-__author__ = "Nathan Taggart"
-__credits__ = "meisnate12"
-__package_name__ = "kometautils"
-__project_name__ = "Kometa-Utils"
-__description__ = "Util Methods for Kometa"
-__url__ = "https://github.com/Kometa-Team/Kometa-Utils"
-__email__ = 'meisnate12@gmail.com'
-__license__ = 'MIT License'
-__all__ = [
-    "KometaLogger",
-    "KometaArgs",
-    "Version",
-    "Continue",
-    "Deleted",
-    "Failed",
-    "FilterFailed",
-    "LimitReached",
-    "NonExisting",
-    "NotScheduled",
-    "NotScheduledRange",
-    "TimeoutExpired",
-]
+from importlib.metadata import version, PackageNotFoundError
+from . import util
+from .logging import KometaLogger
+from .args import KometaArgs, Version
+from .exceptions import Continue, Deleted, Failed, FilterFailed, LimitReached, NonExisting, NotScheduled, NotScheduledRange, TimeoutExpired
+
+
+try:
+    __version__ = version("kometautils")
+except PackageNotFoundError:
+    __version__ = ""
+
+__author__ = "Nathan Taggart"
+__credits__ = "meisnate12"
+__package_name__ = "kometautils"
+__project_name__ = "Kometa-Utils"
+__description__ = "Util Methods for Kometa"
+__url__ = "https://github.com/Kometa-Team/Kometa-Utils"
+__email__ = 'meisnate12@gmail.com'
+__license__ = 'MIT License'
+__all__ = [
+    "KometaLogger",
+    "KometaArgs",
+    "Version",
+    "Continue",
+    "Deleted",
+    "Failed",
+    "FilterFailed",
+    "LimitReached",
+    "NonExisting",
+    "NotScheduled",
+    "NotScheduledRange",
+    "TimeoutExpired",
+]
```

### Comparing `kometautils-0.1.0/kometautils/args.py` & `kometautils-0.2.0/kometautils/args.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,261 +1,261 @@
-import argparse, os, platform, re, requests, uuid
-from dotenv import load_dotenv
-from functools import cached_property
-from pathlib import Path
-from .exceptions import Failed
-
-def parse_choice(env_str, default, arg_bool=False, arg_int=False):
-    env_value = os.environ.get(env_str)
-    if env_value is None:
-        return default
-    elif arg_bool:
-        return parse_bool(env_value, default)
-    elif arg_int:
-        try:
-            return int(env_value)
-        except ValueError:
-            return default
-    else:
-        return str(env_value)
-
-def parse_bool(value, default=None):
-    if value is True or value is False:
-        return value
-    elif value.lower() in ["t", "true", "1", "y", "yes"]:
-        return True
-    elif value.lower() in ["f", "false", "0", "n", "no"]:
-        return False
-    else:
-        return default
-
-class Version:
-    def __init__(self, original="Unknown", text="develop"):
-        self.original = original
-        self.text = text
-        self.version = self.original.replace("develop", self.text)
-        split_version = self.version.split(f"-{self.text}")
-        self.master = split_version[0]
-        self.patch = int(split_version[1]) if len(split_version) > 1 else 0
-        sp = self.master.split(".")
-        sep = (0, 0, 0) if self.original == "Unknown" or len(sp) < 3 else sp
-        self.compare = (sep[0], sep[1], sep[2], self.patch)
-        self._has_patch = None
-
-    def same_master(self, other):
-        return self.master == other.master
-
-    def has_patch(self):
-        return self.patch > 0
-
-    def __str__(self):
-        return self.version
-
-    def __bool__(self):
-        return self.original != "Unknown"
-
-    def __eq__(self, other):
-        return self.compare == other.compare
-
-    def __ne__(self, other):
-        return self.compare != other.compare
-
-    def __lt__(self, other):
-        return self.compare < other.compare
-
-    def __le__(self, other):
-        return self.compare <= other.compare
-
-    def __gt__(self, other):
-        return self.compare > other.compare
-
-    def __ge__(self, other):
-        return self.compare >= other.compare
-
-class KometaArgs:
-    def __init__(self, repo_name, base_dir, options, config_folder="config", use_nightly=True, running_nightly=False):
-        self.repo = repo_name
-        self.base_dir = Path(base_dir)
-        self.options = options
-        self.use_nightly = use_nightly
-        self.running_nightly = running_nightly
-        self.original_choices = {}
-        self.choices = {}
-        parser = argparse.ArgumentParser()
-        if not isinstance(options, list):
-            raise ValueError("options must be a list")
-        for o in self.options:
-            for atr in ["type", "arg", "env", "key", "help", "default"]:
-                if atr not in o:
-                    raise AttributeError(f"{o} attribute must be in every option")
-            if o["type"] == "int":
-                parser.add_argument(f"-{o['arg']}", f"--{o['key']}", dest=o["key"], help=o["help"], type=int, default=o["default"])
-            elif o["type"] == "bool":
-                parser.add_argument(f"-{o['arg']}", f"--{o['key']}", dest=o["key"], help=o["help"], action="store_true", default=o["default"])
-            else:
-                parser.add_argument(f"-{o['arg']}", f"--{o['key']}", dest=o["key"], help=o["help"])
-        args_parsed = parser.parse_args()
-        load_dotenv(self.base_dir / config_folder / ".env" if config_folder else self.base_dir / ".env")
-
-        for o in self.options:
-            value = parse_choice(o["env"], getattr(args_parsed, o["key"]), arg_int=o["type"] == "int", arg_bool=o["type"] == "bool")
-            self.original_choices[o["key"]] = value
-            self.choices[o["key"]] = value
-
-    def __getitem__(self, key):
-        if key in self.choices:
-            return self.choices[key]
-        raise KeyError(key)
-
-    def __setitem__(self, key, value):
-        self.choices[key] = value
-
-    def __contains__(self, key):
-        return key in self.choices
-
-    def _github_request(self, path, repo=None, params=None):
-        response = requests.get(f"https://api.github.com/repos/{repo or self.repo}/{path}", params=params)
-        if response.status_code >= 400:
-            raise Failed(f"({response.status_code} [{response.reason}]) {response.json()}")
-        return response.json()
-
-    def git_release_notes(self, repo=None):
-        return self._github_request("releases/latest", repo=repo)["body"]
-
-    def git_commits(self, repo=None):
-        master_sha = self._github_request("commits/master", repo=repo)["sha"]
-        commits = []
-        for commit in self._github_request("commits", repo=repo, params={"sha": "nightly" if self.is_nightly else "develop"}):
-            if commit["sha"] == master_sha:
-                break
-            message = commit["commit"]["message"]
-            match = re.match("^\\[(\\d)\\]", message)
-            if match and int(match.group(1)) <= self.local_version.patch:
-                break
-            commits.append(message)
-        return "\n".join(commits)
-
-    def git_tags(self, repo=None):
-        return [r["ref"][11:] for r in self._github_request("git/refs/tags", repo=repo)]
-
-    @cached_property
-    def update_notes(self):
-        if self.update_version and self.local_version:
-            if not self.update_version.same_master(self.local_version):
-                return self.git_release_notes()
-            elif self.local_version.patch and self.local_version < self.update_version:
-                return self.git_commits()
-        return None
-
-    @cached_property
-    def uuid(self):
-        uuid_file = self.base_dir / "config" / "UUID"
-        if uuid_file.exists():
-            with uuid_file.open() as handle:
-                for line in handle.readlines():
-                    line = line.strip()
-                    if len(line) > 0:
-                        return str(line)
-        _uuid = str(uuid.uuid4())
-        with uuid_file.open(mode="w") as handle:
-            handle.write(_uuid)
-        return _uuid
-
-    @cached_property
-    def system_version(self):
-        if self.is_docker:
-            return "(Docker)"
-        elif self.is_linuxserver:
-            return "(Linuxserver)"
-        else:
-            return f"(Python {platform.python_version()}){f' (Git: {self.local_branch})' if self.local_branch else ''}"
-
-    @cached_property
-    def is_docker(self):
-        return parse_choice("KOMETA_DOCKER", False, arg_bool=True)
-
-    @cached_property
-    def is_linuxserver(self):
-        return parse_choice("KOMETA_LINUXSERVER", False, arg_bool=True)
-
-    @cached_property
-    def local_version(self):
-        ver = Version()
-        with (self.base_dir / "VERSION").open() as handle:
-            for line in handle.readlines():
-                line = line.strip()
-                if len(line) > 0:
-                    ver = Version(line)
-        return ver
-
-    @cached_property
-    def nightly_version(self):
-        return self.online_version("nightly")
-
-    @cached_property
-    def develop_version(self):
-        return self.online_version("develop")
-
-    @cached_property
-    def master_version(self):
-        return self.online_version("master")
-
-    def online_version(self, level):
-        try:
-            response = requests.get(f"https://raw.githubusercontent.com/{self.repo}/{level}/VERSION")
-            if response.status_code < 400:
-                return Version(response.content.decode().strip(), text=level)
-        except requests.exceptions.ConnectionError:
-            pass
-        return Version()
-
-    @cached_property
-    def version(self):
-        match self.branch:
-            case "nightly":
-                return self.nightly_version
-            case "develop":
-                return self.develop_version
-            case _:
-                return self.master_version
-
-    @cached_property
-    def update_version(self):
-        return self.version if self.version and self.local_version < self.version else None
-
-    @cached_property
-    def local_branch(self):
-        try:
-            from git import Repo
-            return Repo(path=".").head.ref.name # noqa
-        except Exception:
-            return None
-
-    @cached_property
-    def env_branch(self):
-        return parse_choice("BRANCH_NAME", "master")
-
-    @cached_property
-    def branch(self):
-        if self.running_nightly:
-            return "nightly"
-        elif self.local_branch:
-            return self.local_branch
-        elif self.env_branch in ["nightly", "develop"]:
-            return self.env_branch
-        elif self.local_version.has_patch():
-            return "develop" if not self.use_nightly or self.local_version <= self.develop_version else "nightly"
-        else:
-            return "master"
-
-    @cached_property
-    def is_nightly(self):
-        return self.branch == "nightly"
-
-    @cached_property
-    def is_develop(self):
-        return self.branch == "develop"
-
-    @cached_property
-    def is_master(self):
-        return self.branch == "master"
-
+import argparse, os, platform, re, requests, uuid
+from dotenv import load_dotenv
+from functools import cached_property
+from pathlib import Path
+from .exceptions import Failed
+
+def parse_choice(env_str, default, arg_bool=False, arg_int=False):
+    env_value = os.environ.get(env_str)
+    if env_value is None:
+        return default
+    elif arg_bool:
+        return parse_bool(env_value, default)
+    elif arg_int:
+        try:
+            return int(env_value)
+        except ValueError:
+            return default
+    else:
+        return str(env_value)
+
+def parse_bool(value, default=None):
+    if value is True or value is False:
+        return value
+    elif value.lower() in ["t", "true", "1", "y", "yes"]:
+        return True
+    elif value.lower() in ["f", "false", "0", "n", "no"]:
+        return False
+    else:
+        return default
+
+class Version:
+    def __init__(self, original="Unknown", text="develop"):
+        self.original = original
+        self.text = text
+        self.version = self.original.replace("develop", self.text)
+        split_version = self.version.split(f"-{self.text}")
+        self.master = split_version[0]
+        self.patch = int(split_version[1]) if len(split_version) > 1 else 0
+        sp = self.master.split(".")
+        sep = (0, 0, 0) if self.original == "Unknown" or len(sp) < 3 else sp
+        self.compare = (sep[0], sep[1], sep[2], self.patch)
+        self._has_patch = None
+
+    def same_master(self, other):
+        return self.master == other.master
+
+    def has_patch(self):
+        return self.patch > 0
+
+    def __str__(self):
+        return self.version
+
+    def __bool__(self):
+        return self.original != "Unknown"
+
+    def __eq__(self, other):
+        return self.compare == other.compare
+
+    def __ne__(self, other):
+        return self.compare != other.compare
+
+    def __lt__(self, other):
+        return self.compare < other.compare
+
+    def __le__(self, other):
+        return self.compare <= other.compare
+
+    def __gt__(self, other):
+        return self.compare > other.compare
+
+    def __ge__(self, other):
+        return self.compare >= other.compare
+
+class KometaArgs:
+    def __init__(self, repo_name, base_dir, options, config_folder="config", use_nightly=True, running_nightly=False):
+        self.repo = repo_name
+        self.base_dir = Path(base_dir)
+        self.options = options
+        self.use_nightly = use_nightly
+        self.running_nightly = running_nightly
+        self.original_choices = {}
+        self.choices = {}
+        parser = argparse.ArgumentParser()
+        if not isinstance(options, list):
+            raise ValueError("options must be a list")
+        for o in self.options:
+            for atr in ["type", "arg", "env", "key", "help", "default"]:
+                if atr not in o:
+                    raise AttributeError(f"{o} attribute must be in every option")
+            if o["type"] == "int":
+                parser.add_argument(f"-{o['arg']}", f"--{o['key']}", dest=o["key"], help=o["help"], type=int, default=o["default"])
+            elif o["type"] == "bool":
+                parser.add_argument(f"-{o['arg']}", f"--{o['key']}", dest=o["key"], help=o["help"], action="store_true", default=o["default"])
+            else:
+                parser.add_argument(f"-{o['arg']}", f"--{o['key']}", dest=o["key"], help=o["help"])
+        args_parsed = parser.parse_args()
+        load_dotenv(self.base_dir / config_folder / ".env" if config_folder else self.base_dir / ".env")
+
+        for o in self.options:
+            value = parse_choice(o["env"], getattr(args_parsed, o["key"]), arg_int=o["type"] == "int", arg_bool=o["type"] == "bool")
+            self.original_choices[o["key"]] = value
+            self.choices[o["key"]] = value
+
+    def __getitem__(self, key):
+        if key in self.choices:
+            return self.choices[key]
+        raise KeyError(key)
+
+    def __setitem__(self, key, value):
+        self.choices[key] = value
+
+    def __contains__(self, key):
+        return key in self.choices
+
+    def _github_request(self, path, repo=None, params=None):
+        response = requests.get(f"https://api.github.com/repos/{repo or self.repo}/{path}", params=params)
+        if response.status_code >= 400:
+            raise Failed(f"({response.status_code} [{response.reason}]) {response.json()}")
+        return response.json()
+
+    def git_release_notes(self, repo=None):
+        return self._github_request("releases/latest", repo=repo)["body"]
+
+    def git_commits(self, repo=None):
+        master_sha = self._github_request("commits/master", repo=repo)["sha"]
+        commits = []
+        for commit in self._github_request("commits", repo=repo, params={"sha": "nightly" if self.is_nightly else "develop"}):
+            if commit["sha"] == master_sha:
+                break
+            message = commit["commit"]["message"]
+            match = re.match("^\\[(\\d)\\]", message)
+            if match and int(match.group(1)) <= self.local_version.patch:
+                break
+            commits.append(message)
+        return "\n".join(commits)
+
+    def git_tags(self, repo=None):
+        return [r["ref"][11:] for r in self._github_request("git/refs/tags", repo=repo)]
+
+    @cached_property
+    def update_notes(self):
+        if self.update_version and self.local_version:
+            if not self.update_version.same_master(self.local_version):
+                return self.git_release_notes()
+            elif self.local_version.patch and self.local_version < self.update_version:
+                return self.git_commits()
+        return None
+
+    @cached_property
+    def uuid(self):
+        uuid_file = self.base_dir / "config" / "UUID"
+        if uuid_file.exists():
+            with uuid_file.open() as handle:
+                for line in handle.readlines():
+                    line = line.strip()
+                    if len(line) > 0:
+                        return str(line)
+        _uuid = str(uuid.uuid4())
+        with uuid_file.open(mode="w") as handle:
+            handle.write(_uuid)
+        return _uuid
+
+    @cached_property
+    def system_version(self):
+        if self.is_docker:
+            return "(Docker)"
+        elif self.is_linuxserver:
+            return "(Linuxserver)"
+        else:
+            return f"(Python {platform.python_version()}){f' (Git: {self.local_branch})' if self.local_branch else ''}"
+
+    @cached_property
+    def is_docker(self):
+        return parse_choice("KOMETA_DOCKER", False, arg_bool=True)
+
+    @cached_property
+    def is_linuxserver(self):
+        return parse_choice("KOMETA_LINUXSERVER", False, arg_bool=True)
+
+    @cached_property
+    def local_version(self):
+        ver = Version()
+        with (self.base_dir / "VERSION").open() as handle:
+            for line in handle.readlines():
+                line = line.strip()
+                if len(line) > 0:
+                    ver = Version(line)
+        return ver
+
+    @cached_property
+    def nightly_version(self):
+        return self.online_version("nightly")
+
+    @cached_property
+    def develop_version(self):
+        return self.online_version("develop")
+
+    @cached_property
+    def master_version(self):
+        return self.online_version("master")
+
+    def online_version(self, level):
+        try:
+            response = requests.get(f"https://raw.githubusercontent.com/{self.repo}/{level}/VERSION")
+            if response.status_code < 400:
+                return Version(response.content.decode().strip(), text=level)
+        except requests.exceptions.ConnectionError:
+            pass
+        return Version()
+
+    @cached_property
+    def version(self):
+        match self.branch:
+            case "nightly":
+                return self.nightly_version
+            case "develop":
+                return self.develop_version
+            case _:
+                return self.master_version
+
+    @cached_property
+    def update_version(self):
+        return self.version if self.version and self.local_version < self.version else None
+
+    @cached_property
+    def local_branch(self):
+        try:
+            from git import Repo
+            return Repo(path=".").head.ref.name # noqa
+        except Exception:
+            return None
+
+    @cached_property
+    def env_branch(self):
+        return parse_choice("BRANCH_NAME", "master")
+
+    @cached_property
+    def branch(self):
+        if self.running_nightly:
+            return "nightly"
+        elif self.local_branch:
+            return self.local_branch
+        elif self.env_branch in ["nightly", "develop"]:
+            return self.env_branch
+        elif self.local_version.has_patch():
+            return "develop" if not self.use_nightly or self.local_version <= self.develop_version else "nightly"
+        else:
+            return "master"
+
+    @cached_property
+    def is_nightly(self):
+        return self.branch == "nightly"
+
+    @cached_property
+    def is_develop(self):
+        return self.branch == "develop"
+
+    @cached_property
+    def is_master(self):
+        return self.branch == "master"
+
```

### Comparing `kometautils-0.1.0/kometautils/logging.py` & `kometautils-0.2.0/kometautils/logging.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,500 +1,500 @@
-import logging, platform, psutil, requests, sys, traceback
-from datetime import datetime
-from functools import cached_property
-from json import JSONDecodeError
-from logging.handlers import RotatingFileHandler
-from pathlib import Path
-from .exceptions import Failed
-
-logger = None
-
-class RedactingFormatter(logging.Formatter):
-    _secrets = []
-
-    def __init__(self, orig_format, secrets=None):
-        self.orig_formatter = logging.Formatter(orig_format)
-        if secrets:
-            self._secrets.extend(secrets)
-        super().__init__()
-
-    def format(self, record):
-        for secret in self._secrets:
-            if secret:
-                record.msg = record.msg.replace(secret, "(redacted)")
-        return self.orig_formatter.format(record)
-
-    def __getattr__(self, attr):
-        return getattr(self.orig_formatter, attr)
-
-def log_namer(default_name):
-    base, ext, num = default_name.split(".")
-    return f"{base}-{num}.{ext}"
-
-class Stat:
-    def __init__(self, name=None):
-        self.name = name
-        self.start = datetime.now()
-        self.stats = {}
-
-    def __getitem__(self, key):
-        if key in self.stats:
-            return self.stats[key]
-        raise KeyError(key)
-
-    def __setitem__(self, key, value):
-        self.stats[key] = value
-
-    @cached_property
-    def end(self):
-        return datetime.now()
-
-    @cached_property
-    def runtime(self):
-        return str(self.end - self.start).split(".")[0]
-
-    def __str__(self):
-        return self.runtime
-
-def my_except_hook(exctype, value, tb):
-    if issubclass(exctype, KeyboardInterrupt):
-        sys.__excepthook__(exctype, value, tb)
-    elif logger:
-        logger.critical(f"Traceback (most recent call last):\n{''.join(traceback.format_tb(tb))}{exctype.__name__}: {value}", discord=True)
-
-def fmt_filter(record):
-    record.levelname = f"[{record.levelname}]"
-    record.filename = f"[{record.filename}:{record.lineno}]"
-    return True
-
-class KometaLogger:
-    def __init__(self, name, log_name, log_dir, log_file=None, discord_url=None, ignore_ghost=False, is_debug=True, is_trace=False, log_requests=False):
-        global logger
-        logger = self
-        sys.excepthook = my_except_hook
-        self.name = name
-        self.log_name = log_name
-        self.log_dir = Path(log_dir)
-        self.log_file = log_file
-        self.discord_url = discord_url
-        self.is_debug = is_debug
-        self.is_trace = is_trace
-        self.log_requests = log_requests
-        self.ignore_ghost = ignore_ghost
-        self.current = None
-        self.stats = {self.current: Stat()}
-        self.warnings = {}
-        self.errors = {}
-        self.criticals = {}
-        self.spacing = 0
-        self.screen_width = 100
-        self.separating_character = "="
-        self.filename_spacing = 27
-        self.thumbnail_url = "https://github.com/meisnate12/Plex-Meta-Manager/raw/master/docs/_static/favicon.png"
-        self.bot_name = "Metabot"
-        self.bot_image_url = "https://github.com/meisnate12/Plex-Meta-Manager/raw/master/.github/pmm.png"
-        if not self.log_file:
-            self.log_file = f"{self.log_name}.log"
-        self.log_path = self.log_dir / self.log_file
-        self.log_path.parent.mkdir(exist_ok=True)
-        self._logger = logging.getLogger(None if self.log_requests else self.log_name)
-        self._logger.setLevel(logging.DEBUG)
-        self.cmd_handler = logging.StreamHandler()
-        self.cmd_handler.setLevel(logging.DEBUG if self.is_debug else logging.INFO)
-        self._formatter(handler=self.cmd_handler)
-        self._logger.addHandler(self.cmd_handler)
-        self.main_handler = None
-        self.old__log = self._logger._log
-        self._logger._log = self.new__log
-
-    def new__log(self, level, msg, args, exc_info=None, extra=None, stack_info=False, center=False, stacklevel=2):
-        trace = level == logging.NOTSET
-        log_only = False
-        msg = str(msg)
-        if center:
-            msg = self._centered(msg)
-        if trace:
-            level = logging.DEBUG
-        if trace or msg.startswith("|"):
-            self._formatter(trace=trace, border=not msg.startswith("|"))
-        if self.spacing > 0:
-            self.exorcise()
-        if "\n" in msg:
-            for i, line in enumerate(msg.split("\n")):
-                self.old__log(level, line, args, exc_info=exc_info, extra=extra, stack_info=stack_info, stacklevel=stacklevel)
-                if i == 0:
-                    self._formatter(log_only=True, space=True)
-            log_only = True
-        else:
-            self.old__log(level, msg, args, exc_info=exc_info, extra=extra, stack_info=stack_info, stacklevel=stacklevel)
-
-        if trace or log_only or msg.startswith("|"):
-            self._formatter()
-
-    def add_main_handler(self, count=9):
-        self.main_handler = self._add_handler(self.log_path, count=count)
-        self.main_handler.addFilter(fmt_filter)
-        self._logger.addHandler(self.main_handler)
-
-    def remove_main_handler(self):
-        self._logger.removeHandler(self.main_handler)
-
-    def _add_handler(self, log_file, count=3):
-        _handler = RotatingFileHandler(log_file, delay=True, mode="w", backupCount=count, encoding="utf-8")
-        _handler.namer = log_namer
-        self._formatter(handler=_handler)
-        if Path(log_file).is_file():
-            self._logger.removeHandler(_handler)
-            _handler.doRollover()
-            self._logger.addHandler(_handler)
-        return _handler
-
-    def _formatter(self, handler=None, border=True, trace=False, log_only=False, space=False):
-        console = f"%(message)-{self.screen_width - 2}s"
-        console = f"| {console} |" if border else console
-        file = f"{' ' * 65}" if space else f"[%(asctime)s] %(filename)-{self.filename_spacing}s {'[TRACE]   ' if trace else '%(levelname)-10s'} "
-        handlers = [handler] if handler else self._logger.handlers
-        for h in handlers:
-            if not log_only or isinstance(h, RotatingFileHandler):
-                h.setFormatter(RedactingFormatter(f"{file if isinstance(h, RotatingFileHandler) else ''}{console}"))
-
-    def _center(self, text, total, sep=None, left=False, right=False):
-        if sep is None:
-            sep = " "
-        text = str(text)
-        space = total - len(text)
-        if space % 2 == 1:
-            text = f"{sep}{text}" if right else f"{text}{sep}"
-            space -= 1
-        side = int(space / 2)
-        if left:
-            return f"{text}{sep * side}{sep * side}"
-        elif right:
-            return f"{sep * side}{sep * side}{text}"
-        else:
-            return f"{sep * side}{text}{sep * side}"
-
-    def _centered(self, text, sep=None, side_space=True, left=False, right=False):
-        text = str(text)
-        if len(text) > self.screen_width - 2:
-            return text
-        side = " " if side_space else sep if sep else ""
-        final = self._center(f"{side}{text}{side}", self.screen_width - 2, sep=sep, left=left, right=right)
-        return final
-
-    def _separator(self, text=None, space=True, border=True, enclose=False, sep=None, debug=False, trace=False, side_space=True, start=None, left=False, right=False, stacklevel=7):
-        self.separator(text=text, space=space, border=border, enclose=enclose, sep=sep, debug=debug, trace=trace, side_space=side_space, start=start, left=left, right=right, stacklevel=stacklevel)
-
-    def separator(self, text=None, space=True, border=True, enclose=False, sep=None, debug=False, trace=False, side_space=True, start=None, left=False, right=False, stacklevel=5):
-        if start is not None:
-            self.start(start)
-        if trace and not self.is_trace:
-            return None
-        character = sep or self.separating_character
-        sep = " " if space else character
-        border_text = f"|{character * self.screen_width}|"
-        text_list = text.split("\n") if text else []
-        if text and enclose:
-            text_width = len(max(text_list, key=len)) + (2 if side_space else 0)
-            box_width = text_width + 2
-            if box_width < self.screen_width - 2:
-                border_text = self._center(f"{box_width * character}", self.screen_width - 2, left=left, right=right)
-            text_list = [f"|{self._center(t, text_width)}|" for t in text_list]
-        if border:
-            self.print(border_text, debug=debug, trace=trace, stacklevel=stacklevel)
-        if text:
-            for t in text_list:
-                msg = f"|{sep}{self._centered(t, sep=None if enclose else sep, side_space=side_space and not enclose, left=left, right=right)}{sep}|"
-                self.print(msg, debug=debug, trace=trace, stacklevel=stacklevel)
-            if border:
-                self.print(border_text, debug=debug, trace=trace, stacklevel=stacklevel)
-
-    def _print(self, msg="", critical=False, error=False, warning=False, debug=False, trace=False, stacklevel=6):
-        self.print(msg=msg, critical=critical, error=error, warning=warning, debug=debug, trace=trace, stacklevel=stacklevel)
-
-    def print(self, msg="", critical=False, error=False, warning=False, debug=False, trace=False, stacklevel=4):
-        if critical:
-            self.critical(msg, stacklevel=stacklevel)
-        elif error:
-            self.error(msg, stacklevel=stacklevel)
-        elif warning:
-            self.warning(msg, stacklevel=stacklevel)
-        elif debug:
-            self.debug(msg, stacklevel=stacklevel)
-        elif trace:
-            self.trace(msg, stacklevel=stacklevel)
-        else:
-            self.info(msg, stacklevel=stacklevel)
-
-    def _trace(self, msg="", center=False, log=True, discord=False, rows=None, stacklevel=5):
-        return self.trace(msg=msg, center=center, log=log, discord=discord, rows=rows, stacklevel=stacklevel)
-
-    def trace(self, msg="", center=False, log=True, discord=False, start=None, rows=None, stacklevel=3):
-        if self.is_trace:
-            if start is not None:
-                self.start(start)
-            if log:
-                self.new__log(logging.NOTSET, msg, [], center=center, stacklevel=stacklevel)
-            if discord:
-                self.discord_request(" Trace", msg, rows=rows)
-        return str(msg)
-
-    def _debug(self, msg="", center=False, log=True, discord=False, rows=None, stacklevel=5):
-        return self.debug(msg=msg, center=center, log=log, discord=discord, rows=rows, stacklevel=stacklevel)
-
-    def debug(self, msg="", center=False, log=True, discord=False, start=None, rows=None, stacklevel=3):
-        if self._logger.isEnabledFor(logging.DEBUG):
-            if start is not None:
-                self.start(start)
-            if log:
-                self.new__log(logging.DEBUG, msg, [], center=center, stacklevel=stacklevel)
-            if discord:
-                self.discord_request(" Debug", msg, rows=rows)
-        return str(msg)
-
-    def _info(self, msg="", center=False, log=True, discord=False, rows=None, stacklevel=5):
-        return self.info(msg=msg, center=center, log=log, discord=discord, rows=rows, stacklevel=stacklevel)
-
-    def info(self, msg="", center=False, log=True, discord=False, start=None, rows=None, stacklevel=3):
-        if self._logger.isEnabledFor(logging.INFO):
-            if start is not None:
-                self.start(start)
-            if log:
-                self.new__log(logging.INFO, msg, [], center=center, stacklevel=stacklevel)
-            if discord:
-                self.discord_request("", msg, rows=rows)
-        return str(msg)
-
-    def _warning(self, msg="", center=False, group=None, ignore=False, log=True, discord=False, rows=None, stacklevel=5):
-        return self.warning(msg=msg, center=center, group=group, ignore=ignore, log=log, discord=discord, rows=rows, stacklevel=stacklevel)
-
-    def warning(self, msg="", center=False, group=None, ignore=False, log=True, discord=False, start=None, rows=None, stacklevel=3):
-        if self._logger.isEnabledFor(logging.WARNING):
-            if not ignore:
-                if group not in self.warnings:
-                    self.warnings[group] = []
-                self.warnings[group].append(msg)
-            if start is not None:
-                self.start(start)
-            if log:
-                self.new__log(logging.WARNING, msg, [], center=center, stacklevel=stacklevel)
-            if discord:
-                self.discord_request(" Warning", msg, rows=rows, color=0xbc0030)
-        return str(msg)
-
-    def _error(self, msg="", center=False, group=None, ignore=False, log=True, discord=False, rows=None, stacklevel=5):
-        return self.error(msg=msg, center=center, group=group, ignore=ignore, log=log, discord=discord, rows=rows, stacklevel=stacklevel)
-
-    def error(self, msg="", center=False, group=None, ignore=False, log=True, discord=False, start=None, rows=None, stacklevel=3):
-        if self._logger.isEnabledFor(logging.ERROR):
-            if not ignore:
-                if group not in self.errors:
-                    self.errors[group] = []
-                self.errors[group].append(msg)
-            if start is not None:
-                self.start(start)
-            if log:
-                self.new__log(logging.ERROR, msg, [], center=center, stacklevel=stacklevel)
-            if discord:
-                self.discord_request(" Error", msg, rows=rows, color=0xbc0030)
-        return str(msg)
-
-    def _critical(self, msg="", center=False, group=None, ignore=False, log=True, discord=False, rows=None, stacklevel=5):
-        return self.critical(msg=msg, center=center, group=group, ignore=ignore, log=log, discord=discord, rows=rows, stacklevel=stacklevel)
-
-    def critical(self, msg="", center=False, group=None, ignore=False, log=True, discord=False, start=None, rows=None, exc_info=None, stacklevel=3):
-        if self._logger.isEnabledFor(logging.CRITICAL):
-            if not ignore:
-                if group not in self.criticals:
-                    self.criticals[group] = []
-                self.criticals[group].append(msg)
-            if start is not None:
-                self.start(start)
-            if log:
-                self.new__log(logging.CRITICAL, msg, [], center=center, exc_info=exc_info, stacklevel=stacklevel)
-            if discord:
-                self.discord_request(" Critical Failure", msg, rows=rows, color=0xbc0030)
-        return str(msg)
-
-    def stacktrace(self, trace=False):
-        self._print(traceback.format_exc(), debug=not trace, trace=trace)
-
-    def _space(self, display_title):
-        display_title = str(display_title)
-        space_length = self.spacing - len(display_title)
-        if space_length > 0:
-            display_title += " " * space_length
-        return display_title
-
-    def ghost(self, text):
-        if not self.ignore_ghost:
-            try:
-                final_text = f"| {text}"
-            except UnicodeEncodeError:
-                text = text.encode("utf-8")
-                final_text = f"| {text}"
-            print(self._space(final_text), end="\r")
-            self.spacing = len(text) + 2
-
-    def exorcise(self):
-        if not self.ignore_ghost:
-            print(self._space(" "), end="\r")
-            self.spacing = 0
-
-    def secret(self, text):
-        text = text if isinstance(text, list) else [text]
-        for t in text:
-            if t and str(t) not in RedactingFormatter._secrets:
-                RedactingFormatter._secrets.append(str(t))
-
-    def discord_request(self, title, description=None, rows=None, color=0x00bc8c):
-        if self.discord_url:
-            embed = {
-                "title": f"{self.name}{title}",
-                "color": color,
-                "timestamp": str(datetime.utcnow())
-            }
-            if description:
-                embed["description"] = description
-            if self.thumbnail_url:
-                embed["thumbnail"] = {"url": self.thumbnail_url, "height": 0, "width": 0}
-            if rows:
-                fields = []
-                for row in rows:
-                    for col in row:
-                        col_name = col[0] if isinstance(col, tuple) else ""
-                        col_value = col[1] if isinstance(col, tuple) else col
-                        if not col_value:
-                            col_value = f"**{col_name}**"
-                            col_name = ""
-                        field = {"name": str(col_name)}
-                        if col_value:
-                            field["value"] = str(col_value)
-                        if len(row) > 1:
-                            field["inline"] = True
-                        fields.append(field)
-                embed["fields"] = fields
-            try:
-                json = {"embeds": [embed], "username": self.bot_name, "avatar_url": self.bot_image_url}
-                response = requests.post(self.discord_url, json=json)
-                try:
-                    response_json = response.json()
-                    if response.status_code >= 400:
-                        self.discord_url = None
-                        raise Failed(f"({response.status_code} [{response.reason}]) {response_json}")
-                except JSONDecodeError:
-                    if response.status_code >= 400:
-                        self.discord_url = None
-                        raise Failed(f"({response.status_code} [{response.reason}])")
-            except requests.exceptions.RequestException:
-                self.discord_url = None
-                raise Failed(f"Discord URL Connection Failure")
-
-    def start(self, name=None):
-        self.current = name
-        self[name] = Stat()
-
-    def switch(self, name=None):
-        self.current = name
-
-    def end(self, name=None):
-        if name is None:
-            name = self.current
-        return self[name].end
-
-    def runtime(self, name=None):
-        if name is None:
-            name = self.current
-        return self[name].runtime
-
-    def stats(self, name=None):
-        if name is None:
-            name = self.current
-        return self[name].stats
-
-    def stat(self, key, value, name=None):
-        if name is None:
-            name = self.current
-        self[name][key] = value
-
-    def __getitem__(self, name):
-        if name in self.stats:
-            return self.stats[name]
-        raise KeyError(name)
-
-    def __setitem__(self, key, value):
-        self.stats[key] = value
-
-    def header(self, kometa_args, sub=False, discord_update=False, override=None, count=9):
-        self.add_main_handler(count=count)
-        self._separator()
-        self._info(" __  ___   ______   .___  ___.  _______ .___________.    ___      ", center=True)
-        self._info("|  |/  /  /  __  \\  |   \\/   | |   ____||           |   /   \\     ", center=True)
-        self._info("|  '  /  |  |  |  | |  \\  /  | |  |__   `---|  |----`  /  ^  \\    ", center=True)
-        self._info("|    <   |  |  |  | |  |\\/|  | |   __|      |  |      /  /_\\  \\   ", center=True)
-        self._info("|  .  \\  |  `--'  | |  |  |  | |  |____     |  |     /  _____  \\  ", center=True)
-        self._info("|__|\\__\\  \\______/  |__|  |__| |_______|    |__|    /__/     \\__\\ ", center=True)
-        if sub:
-            self._info(self.name, center=True)
-            self._info()
-
-        self._info(f"    Version: {kometa_args.local_version} {kometa_args.system_version}")
-        if kometa_args.update_version:
-            if discord_update and self.discord_url:
-                self._warning("New Version Available!", log=False, discord=True, rows=[
-                    [("Current", str(kometa_args.local_version)), ("Latest", kometa_args.update_version)],
-                    [("Updates", kometa_args.update_notes)]
-                ])
-            self._info(f"    Newest Version: {kometa_args.update_version}")
-        self._info(f"    Platform: {platform.platform()}")
-        self._info(f"    Memory: {round(psutil.virtual_memory().total / (1024.0 ** 3))} GB")
-        self._separator(debug=True)
-
-        run_arg = " ".join([f'"{s}"' if " " in s else s for s in sys.argv[:]])
-        self._debug(f"Run Command: {run_arg}")
-        for o in kometa_args.options:
-            value = override[o["key"]] if override and o["key"] in override else kometa_args.choices[o['key']]
-            self._debug(f"--{o['key']} ({o['env']}): {value}")
-
-    def report(self, title, rows, description=None, width=None, discord=False):
-        self._separator(title)
-        if description:
-            self._info(description)
-        for row in rows:
-            if len(row) > 1:
-                length = 0 if width is None else width
-                if width is None:
-                    for k, v in row:
-                        if (new_length := len(str(k))) > length:
-                            length = new_length
-                for k, v in row:
-                    self._info(f"{k:<{length}} | {v}")
-            elif isinstance(row[0], tuple):
-                if not row[0][1]:
-                    self._separator(row[0][0], space=False, border=False)
-                elif not row[0][0]:
-                    self._info(f"{row[0][1]}")
-                elif width is None:
-                    self._info(f"{row[0][0]} | {row[0][1]}")
-                else:
-                    self._info(f"{row[0][0]:<{width}} | {row[0][1]}")
-            else:
-                self._info(row[0])
-        self._separator()
-        if discord:
-            self.discord_request(title, description=description, rows=rows)
-
-    def error_report(self, warning=False, error=True, critical=True, group_only=False):
-        for check, title, e_dict in [
-            (warning, "Warning", self.warnings),
-            (error, "Error", self.errors),
-            (critical, "Critical", self.criticals)
-        ]:
-            if check and e_dict:
-                self._separator(f"{title} Report")
-                for k, v in e_dict.items():
-                    if group_only and k is None:
-                        continue
-                    self._info()
-                    self._info(f"{'Generic' if k is None else k} {title}s: ")
-                    for e in v:
-                        self._error(f"  {e}", ignore=True)
+import logging, platform, psutil, requests, sys, traceback
+from datetime import datetime
+from functools import cached_property
+from json import JSONDecodeError
+from logging.handlers import RotatingFileHandler
+from pathlib import Path
+from .exceptions import Failed
+
+logger = None
+
+class RedactingFormatter(logging.Formatter):
+    _secrets = []
+
+    def __init__(self, orig_format, secrets=None):
+        self.orig_formatter = logging.Formatter(orig_format)
+        if secrets:
+            self._secrets.extend(secrets)
+        super().__init__()
+
+    def format(self, record):
+        for secret in self._secrets:
+            if secret:
+                record.msg = record.msg.replace(secret, "(redacted)")
+        return self.orig_formatter.format(record)
+
+    def __getattr__(self, attr):
+        return getattr(self.orig_formatter, attr)
+
+def log_namer(default_name):
+    base, ext, num = default_name.split(".")
+    return f"{base}-{num}.{ext}"
+
+class Stat:
+    def __init__(self, name=None):
+        self.name = name
+        self.start = datetime.now()
+        self.stats = {}
+
+    def __getitem__(self, key):
+        if key in self.stats:
+            return self.stats[key]
+        raise KeyError(key)
+
+    def __setitem__(self, key, value):
+        self.stats[key] = value
+
+    @cached_property
+    def end(self):
+        return datetime.now()
+
+    @cached_property
+    def runtime(self):
+        return str(self.end - self.start).split(".")[0]
+
+    def __str__(self):
+        return self.runtime
+
+def my_except_hook(exctype, value, tb):
+    if issubclass(exctype, KeyboardInterrupt):
+        sys.__excepthook__(exctype, value, tb)
+    elif logger:
+        logger.critical(f"Traceback (most recent call last):\n{''.join(traceback.format_tb(tb))}{exctype.__name__}: {value}", discord=True)
+
+def fmt_filter(record):
+    record.levelname = f"[{record.levelname}]"
+    record.filename = f"[{record.filename}:{record.lineno}]"
+    return True
+
+class KometaLogger:
+    def __init__(self, name, log_name, log_dir, log_file=None, discord_url=None, ignore_ghost=False, is_debug=True, is_trace=False, log_requests=False):
+        global logger
+        logger = self
+        sys.excepthook = my_except_hook
+        self.name = name
+        self.log_name = log_name
+        self.log_dir = Path(log_dir)
+        self.log_file = log_file
+        self.discord_url = discord_url
+        self.is_debug = is_debug
+        self.is_trace = is_trace
+        self.log_requests = log_requests
+        self.ignore_ghost = ignore_ghost
+        self.current = None
+        self.stats = {self.current: Stat()}
+        self.warnings = {}
+        self.errors = {}
+        self.criticals = {}
+        self.spacing = 0
+        self.screen_width = 100
+        self.separating_character = "="
+        self.filename_spacing = 27
+        self.thumbnail_url = "https://github.com/meisnate12/Plex-Meta-Manager/raw/master/docs/_static/favicon.png"
+        self.bot_name = "Metabot"
+        self.bot_image_url = "https://github.com/meisnate12/Plex-Meta-Manager/raw/master/.github/pmm.png"
+        if not self.log_file:
+            self.log_file = f"{self.log_name}.log"
+        self.log_path = self.log_dir / self.log_file
+        self.log_path.parent.mkdir(exist_ok=True)
+        self._logger = logging.getLogger(None if self.log_requests else self.log_name)
+        self._logger.setLevel(logging.DEBUG)
+        self.cmd_handler = logging.StreamHandler()
+        self.cmd_handler.setLevel(logging.DEBUG if self.is_debug else logging.INFO)
+        self._formatter(handler=self.cmd_handler)
+        self._logger.addHandler(self.cmd_handler)
+        self.main_handler = None
+        self.old__log = self._logger._log
+        self._logger._log = self.new__log
+
+    def new__log(self, level, msg, args, exc_info=None, extra=None, stack_info=False, center=False, stacklevel=2):
+        trace = level == logging.NOTSET
+        log_only = False
+        msg = str(msg)
+        if center:
+            msg = self._centered(msg)
+        if trace:
+            level = logging.DEBUG
+        if trace or msg.startswith("|"):
+            self._formatter(trace=trace, border=not msg.startswith("|"))
+        if self.spacing > 0:
+            self.exorcise()
+        if "\n" in msg:
+            for i, line in enumerate(msg.split("\n")):
+                self.old__log(level, line, args, exc_info=exc_info, extra=extra, stack_info=stack_info, stacklevel=stacklevel)
+                if i == 0:
+                    self._formatter(log_only=True, space=True)
+            log_only = True
+        else:
+            self.old__log(level, msg, args, exc_info=exc_info, extra=extra, stack_info=stack_info, stacklevel=stacklevel)
+
+        if trace or log_only or msg.startswith("|"):
+            self._formatter()
+
+    def add_main_handler(self, count=9):
+        self.main_handler = self._add_handler(self.log_path, count=count)
+        self.main_handler.addFilter(fmt_filter)
+        self._logger.addHandler(self.main_handler)
+
+    def remove_main_handler(self):
+        self._logger.removeHandler(self.main_handler)
+
+    def _add_handler(self, log_file, count=3):
+        _handler = RotatingFileHandler(log_file, delay=True, mode="w", backupCount=count, encoding="utf-8")
+        _handler.namer = log_namer
+        self._formatter(handler=_handler)
+        if Path(log_file).is_file():
+            self._logger.removeHandler(_handler)
+            _handler.doRollover()
+            self._logger.addHandler(_handler)
+        return _handler
+
+    def _formatter(self, handler=None, border=True, trace=False, log_only=False, space=False):
+        console = f"%(message)-{self.screen_width - 2}s"
+        console = f"| {console} |" if border else console
+        file = f"{' ' * 65}" if space else f"[%(asctime)s] %(filename)-{self.filename_spacing}s {'[TRACE]   ' if trace else '%(levelname)-10s'} "
+        handlers = [handler] if handler else self._logger.handlers
+        for h in handlers:
+            if not log_only or isinstance(h, RotatingFileHandler):
+                h.setFormatter(RedactingFormatter(f"{file if isinstance(h, RotatingFileHandler) else ''}{console}"))
+
+    def _center(self, text, total, sep=None, left=False, right=False):
+        if sep is None:
+            sep = " "
+        text = str(text)
+        space = total - len(text)
+        if space % 2 == 1:
+            text = f"{sep}{text}" if right else f"{text}{sep}"
+            space -= 1
+        side = int(space / 2)
+        if left:
+            return f"{text}{sep * side}{sep * side}"
+        elif right:
+            return f"{sep * side}{sep * side}{text}"
+        else:
+            return f"{sep * side}{text}{sep * side}"
+
+    def _centered(self, text, sep=None, side_space=True, left=False, right=False):
+        text = str(text)
+        if len(text) > self.screen_width - 2:
+            return text
+        side = " " if side_space else sep if sep else ""
+        final = self._center(f"{side}{text}{side}", self.screen_width - 2, sep=sep, left=left, right=right)
+        return final
+
+    def _separator(self, text=None, space=True, border=True, enclose=False, sep=None, debug=False, trace=False, side_space=True, start=None, left=False, right=False, stacklevel=7):
+        self.separator(text=text, space=space, border=border, enclose=enclose, sep=sep, debug=debug, trace=trace, side_space=side_space, start=start, left=left, right=right, stacklevel=stacklevel)
+
+    def separator(self, text=None, space=True, border=True, enclose=False, sep=None, debug=False, trace=False, side_space=True, start=None, left=False, right=False, stacklevel=5):
+        if start is not None:
+            self.start(start)
+        if trace and not self.is_trace:
+            return None
+        character = sep or self.separating_character
+        sep = " " if space else character
+        border_text = f"|{character * self.screen_width}|"
+        text_list = text.split("\n") if text else []
+        if text and enclose:
+            text_width = len(max(text_list, key=len)) + (2 if side_space else 0)
+            box_width = text_width + 2
+            if box_width < self.screen_width - 2:
+                border_text = self._center(f"{box_width * character}", self.screen_width - 2, left=left, right=right)
+            text_list = [f"|{self._center(t, text_width)}|" for t in text_list]
+        if border:
+            self.print(border_text, debug=debug, trace=trace, stacklevel=stacklevel)
+        if text:
+            for t in text_list:
+                msg = f"|{sep}{self._centered(t, sep=None if enclose else sep, side_space=side_space and not enclose, left=left, right=right)}{sep}|"
+                self.print(msg, debug=debug, trace=trace, stacklevel=stacklevel)
+            if border:
+                self.print(border_text, debug=debug, trace=trace, stacklevel=stacklevel)
+
+    def _print(self, msg="", critical=False, error=False, warning=False, debug=False, trace=False, stacklevel=6):
+        self.print(msg=msg, critical=critical, error=error, warning=warning, debug=debug, trace=trace, stacklevel=stacklevel)
+
+    def print(self, msg="", critical=False, error=False, warning=False, debug=False, trace=False, stacklevel=4):
+        if critical:
+            self.critical(msg, stacklevel=stacklevel)
+        elif error:
+            self.error(msg, stacklevel=stacklevel)
+        elif warning:
+            self.warning(msg, stacklevel=stacklevel)
+        elif debug:
+            self.debug(msg, stacklevel=stacklevel)
+        elif trace:
+            self.trace(msg, stacklevel=stacklevel)
+        else:
+            self.info(msg, stacklevel=stacklevel)
+
+    def _trace(self, msg="", center=False, log=True, discord=False, rows=None, stacklevel=5):
+        return self.trace(msg=msg, center=center, log=log, discord=discord, rows=rows, stacklevel=stacklevel)
+
+    def trace(self, msg="", center=False, log=True, discord=False, start=None, rows=None, stacklevel=3):
+        if self.is_trace:
+            if start is not None:
+                self.start(start)
+            if log:
+                self.new__log(logging.NOTSET, msg, [], center=center, stacklevel=stacklevel)
+            if discord:
+                self.discord_request(" Trace", msg, rows=rows)
+        return str(msg)
+
+    def _debug(self, msg="", center=False, log=True, discord=False, rows=None, stacklevel=5):
+        return self.debug(msg=msg, center=center, log=log, discord=discord, rows=rows, stacklevel=stacklevel)
+
+    def debug(self, msg="", center=False, log=True, discord=False, start=None, rows=None, stacklevel=3):
+        if self._logger.isEnabledFor(logging.DEBUG):
+            if start is not None:
+                self.start(start)
+            if log:
+                self.new__log(logging.DEBUG, msg, [], center=center, stacklevel=stacklevel)
+            if discord:
+                self.discord_request(" Debug", msg, rows=rows)
+        return str(msg)
+
+    def _info(self, msg="", center=False, log=True, discord=False, rows=None, stacklevel=5):
+        return self.info(msg=msg, center=center, log=log, discord=discord, rows=rows, stacklevel=stacklevel)
+
+    def info(self, msg="", center=False, log=True, discord=False, start=None, rows=None, stacklevel=3):
+        if self._logger.isEnabledFor(logging.INFO):
+            if start is not None:
+                self.start(start)
+            if log:
+                self.new__log(logging.INFO, msg, [], center=center, stacklevel=stacklevel)
+            if discord:
+                self.discord_request("", msg, rows=rows)
+        return str(msg)
+
+    def _warning(self, msg="", center=False, group=None, ignore=False, log=True, discord=False, rows=None, stacklevel=5):
+        return self.warning(msg=msg, center=center, group=group, ignore=ignore, log=log, discord=discord, rows=rows, stacklevel=stacklevel)
+
+    def warning(self, msg="", center=False, group=None, ignore=False, log=True, discord=False, start=None, rows=None, stacklevel=3):
+        if self._logger.isEnabledFor(logging.WARNING):
+            if not ignore:
+                if group not in self.warnings:
+                    self.warnings[group] = []
+                self.warnings[group].append(msg)
+            if start is not None:
+                self.start(start)
+            if log:
+                self.new__log(logging.WARNING, msg, [], center=center, stacklevel=stacklevel)
+            if discord:
+                self.discord_request(" Warning", msg, rows=rows, color=0xbc0030)
+        return str(msg)
+
+    def _error(self, msg="", center=False, group=None, ignore=False, log=True, discord=False, rows=None, stacklevel=5):
+        return self.error(msg=msg, center=center, group=group, ignore=ignore, log=log, discord=discord, rows=rows, stacklevel=stacklevel)
+
+    def error(self, msg="", center=False, group=None, ignore=False, log=True, discord=False, start=None, rows=None, stacklevel=3):
+        if self._logger.isEnabledFor(logging.ERROR):
+            if not ignore:
+                if group not in self.errors:
+                    self.errors[group] = []
+                self.errors[group].append(msg)
+            if start is not None:
+                self.start(start)
+            if log:
+                self.new__log(logging.ERROR, msg, [], center=center, stacklevel=stacklevel)
+            if discord:
+                self.discord_request(" Error", msg, rows=rows, color=0xbc0030)
+        return str(msg)
+
+    def _critical(self, msg="", center=False, group=None, ignore=False, log=True, discord=False, rows=None, stacklevel=5):
+        return self.critical(msg=msg, center=center, group=group, ignore=ignore, log=log, discord=discord, rows=rows, stacklevel=stacklevel)
+
+    def critical(self, msg="", center=False, group=None, ignore=False, log=True, discord=False, start=None, rows=None, exc_info=None, stacklevel=3):
+        if self._logger.isEnabledFor(logging.CRITICAL):
+            if not ignore:
+                if group not in self.criticals:
+                    self.criticals[group] = []
+                self.criticals[group].append(msg)
+            if start is not None:
+                self.start(start)
+            if log:
+                self.new__log(logging.CRITICAL, msg, [], center=center, exc_info=exc_info, stacklevel=stacklevel)
+            if discord:
+                self.discord_request(" Critical Failure", msg, rows=rows, color=0xbc0030)
+        return str(msg)
+
+    def stacktrace(self, trace=False):
+        self._print(traceback.format_exc(), debug=not trace, trace=trace)
+
+    def _space(self, display_title):
+        display_title = str(display_title)
+        space_length = self.spacing - len(display_title)
+        if space_length > 0:
+            display_title += " " * space_length
+        return display_title
+
+    def ghost(self, text):
+        if not self.ignore_ghost:
+            try:
+                final_text = f"| {text}"
+            except UnicodeEncodeError:
+                text = text.encode("utf-8")
+                final_text = f"| {text}"
+            print(self._space(final_text), end="\r")
+            self.spacing = len(text) + 2
+
+    def exorcise(self):
+        if not self.ignore_ghost:
+            print(self._space(" "), end="\r")
+            self.spacing = 0
+
+    def secret(self, text):
+        text = text if isinstance(text, list) else [text]
+        for t in text:
+            if t and str(t) not in RedactingFormatter._secrets:
+                RedactingFormatter._secrets.append(str(t))
+
+    def discord_request(self, title, description=None, rows=None, color=0x00bc8c):
+        if self.discord_url:
+            embed = {
+                "title": f"{self.name}{title}",
+                "color": color,
+                "timestamp": str(datetime.utcnow())
+            }
+            if description:
+                embed["description"] = description
+            if self.thumbnail_url:
+                embed["thumbnail"] = {"url": self.thumbnail_url, "height": 0, "width": 0}
+            if rows:
+                fields = []
+                for row in rows:
+                    for col in row:
+                        col_name = col[0] if isinstance(col, tuple) else ""
+                        col_value = col[1] if isinstance(col, tuple) else col
+                        if not col_value:
+                            col_value = f"**{col_name}**"
+                            col_name = ""
+                        field = {"name": str(col_name)}
+                        if col_value:
+                            field["value"] = str(col_value)
+                        if len(row) > 1:
+                            field["inline"] = True
+                        fields.append(field)
+                embed["fields"] = fields
+            try:
+                json = {"embeds": [embed], "username": self.bot_name, "avatar_url": self.bot_image_url}
+                response = requests.post(self.discord_url, json=json)
+                try:
+                    response_json = response.json()
+                    if response.status_code >= 400:
+                        self.discord_url = None
+                        raise Failed(f"({response.status_code} [{response.reason}]) {response_json}")
+                except JSONDecodeError:
+                    if response.status_code >= 400:
+                        self.discord_url = None
+                        raise Failed(f"({response.status_code} [{response.reason}])")
+            except requests.exceptions.RequestException:
+                self.discord_url = None
+                raise Failed(f"Discord URL Connection Failure")
+
+    def start(self, name=None):
+        self.current = name
+        self[name] = Stat()
+
+    def switch(self, name=None):
+        self.current = name
+
+    def end(self, name=None):
+        if name is None:
+            name = self.current
+        return self[name].end
+
+    def runtime(self, name=None):
+        if name is None:
+            name = self.current
+        return self[name].runtime
+
+    def stats(self, name=None):
+        if name is None:
+            name = self.current
+        return self[name].stats
+
+    def stat(self, key, value, name=None):
+        if name is None:
+            name = self.current
+        self[name][key] = value
+
+    def __getitem__(self, name):
+        if name in self.stats:
+            return self.stats[name]
+        raise KeyError(name)
+
+    def __setitem__(self, key, value):
+        self.stats[key] = value
+
+    def header(self, kometa_args, sub=False, discord_update=False, override=None, count=9):
+        self.add_main_handler(count=count)
+        self._separator()
+        self._info(" __  ___   ______   .___  ___.  _______ .___________.    ___      ", center=True)
+        self._info("|  |/  /  /  __  \\  |   \\/   | |   ____||           |   /   \\     ", center=True)
+        self._info("|  '  /  |  |  |  | |  \\  /  | |  |__   `---|  |----`  /  ^  \\    ", center=True)
+        self._info("|    <   |  |  |  | |  |\\/|  | |   __|      |  |      /  /_\\  \\   ", center=True)
+        self._info("|  .  \\  |  `--'  | |  |  |  | |  |____     |  |     /  _____  \\  ", center=True)
+        self._info("|__|\\__\\  \\______/  |__|  |__| |_______|    |__|    /__/     \\__\\ ", center=True)
+        if sub:
+            self._info(self.name, center=True)
+            self._info()
+
+        self._info(f"    Version: {kometa_args.local_version} {kometa_args.system_version}")
+        if kometa_args.update_version:
+            if discord_update and self.discord_url:
+                self._warning("New Version Available!", log=False, discord=True, rows=[
+                    [("Current", str(kometa_args.local_version)), ("Latest", kometa_args.update_version)],
+                    [("Updates", kometa_args.update_notes)]
+                ])
+            self._info(f"    Newest Version: {kometa_args.update_version}")
+        self._info(f"    Platform: {platform.platform()}")
+        self._info(f"    Memory: {round(psutil.virtual_memory().total / (1024.0 ** 3))} GB")
+        self._separator(debug=True)
+
+        run_arg = " ".join([f'"{s}"' if " " in s else s for s in sys.argv[:]])
+        self._debug(f"Run Command: {run_arg}")
+        for o in kometa_args.options:
+            value = override[o["key"]] if override and o["key"] in override else kometa_args.choices[o['key']]
+            self._debug(f"--{o['key']} ({o['env']}): {value}")
+
+    def report(self, title, rows, description=None, width=None, discord=False):
+        self._separator(title)
+        if description:
+            self._info(description)
+        for row in rows:
+            if len(row) > 1:
+                length = 0 if width is None else width
+                if width is None:
+                    for k, v in row:
+                        if (new_length := len(str(k))) > length:
+                            length = new_length
+                for k, v in row:
+                    self._info(f"{k:<{length}} | {v}")
+            elif isinstance(row[0], tuple):
+                if not row[0][1]:
+                    self._separator(row[0][0], space=False, border=False)
+                elif not row[0][0]:
+                    self._info(f"{row[0][1]}")
+                elif width is None:
+                    self._info(f"{row[0][0]} | {row[0][1]}")
+                else:
+                    self._info(f"{row[0][0]:<{width}} | {row[0][1]}")
+            else:
+                self._info(row[0])
+        self._separator()
+        if discord:
+            self.discord_request(title, description=description, rows=rows)
+
+    def error_report(self, warning=False, error=True, critical=True, group_only=False):
+        for check, title, e_dict in [
+            (warning, "Warning", self.warnings),
+            (error, "Error", self.errors),
+            (critical, "Critical", self.criticals)
+        ]:
+            if check and e_dict:
+                self._separator(f"{title} Report")
+                for k, v in e_dict.items():
+                    if group_only and k is None:
+                        continue
+                    self._info()
+                    self._info(f"{'Generic' if k is None else k} {title}s: ")
+                    for e in v:
+                        self._error(f"  {e}", ignore=True)
```

### Comparing `kometautils-0.1.0/kometautils/schedule.py` & `kometautils-0.2.0/kometautils/schedule.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,906 +1,906 @@
-"""
-Python job scheduling for humans.
-
-github.com/dbader/schedule
-
-An in-process scheduler for periodic jobs that uses the builder pattern
-for configuration. Schedule lets you run Python functions (or any other
-callable) periodically at pre-determined intervals using a simple,
-human-friendly syntax.
-
-Inspired by Addam Wiggins' article "Rethinking Cron" [1] and the
-"clockwork" Ruby module [2][3].
-
-Features:
-    - A simple to use API for scheduling jobs.
-    - Very lightweight and no external dependencies.
-    - Excellent test coverage.
-    - Tested on Python 3.6, 3.7, 3.8, 3.9
-
-Usage:
-    import schedule
-    import time
-
-    def job(message='stuff'):
-        print("I'm working on:", message)
-
-    schedule.every(10).minutes.do(job)
-    schedule.every(5).to(10).days.do(job)
-    schedule.every().hour.do(job, message='things')
-    schedule.every().day.at("10:30").do(job)
-
-    while True:
-        schedule.run_pending()
-        time.sleep(1)
-
-[1] https://adam.herokuapp.com/past/2010/4/13/rethinking_cron/
-[2] https://github.com/Rykian/clockwork
-[3] https://adam.herokuapp.com/past/2010/6/30/replace_cron_with_clockwork/
-"""
-from collections.abc import Hashable
-import datetime
-import functools
-import logging
-import random
-import re
-import time
-from typing import Set, List, Optional, Callable, Union
-
-logger = logging.getLogger("schedule")
-
-
-class ScheduleError(Exception):
-    """Base schedule exception"""
-
-    pass
-
-
-class ScheduleValueError(ScheduleError):
-    """Base schedule value error"""
-
-    pass
-
-
-class IntervalError(ScheduleValueError):
-    """An improper interval was used"""
-
-    pass
-
-
-class CancelJob(object):
-    """
-    Can be returned from a job to unschedule itself.
-    """
-
-    pass
-
-
-class Scheduler(object):
-    """
-    Objects instantiated by the :class:`Scheduler <Scheduler>` are
-    factories to create jobs, keep record of scheduled jobs and
-    handle their execution.
-    """
-
-    def __init__(self) -> None:
-        self.jobs: List[Job] = []
-
-    def run_pending(self) -> None:
-        """
-        Run all jobs that are scheduled to run.
-
-        Please note that it is *intended behavior that run_pending()
-        does not run missed jobs*. For example, if you've registered a job
-        that should run every minute and you only call run_pending()
-        in one hour increments then your job won't be run 60 times in
-        between but only once.
-        """
-        runnable_jobs = (job for job in self.jobs if job.should_run)
-        for job in sorted(runnable_jobs):
-            self._run_job(job)
-
-    def run_all(self, delay_seconds: int = 0) -> None:
-        """
-        Run all jobs regardless if they are scheduled to run or not.
-
-        A delay of `delay` seconds is added between each job. This helps
-        distribute system load generated by the jobs more evenly
-        over time.
-
-        :param delay_seconds: A delay added between every executed job
-        """
-        logger.debug(
-            "Running *all* %i jobs with %is delay in between",
-            len(self.jobs),
-            delay_seconds,
-        )
-        for job in self.jobs[:]:
-            self._run_job(job)
-            time.sleep(delay_seconds)
-
-    def get_jobs(self, tag: Optional[Hashable] = None) -> List["Job"]:
-        """
-        Gets scheduled jobs marked with the given tag, or all jobs
-        if tag is omitted.
-
-        :param tag: An identifier used to identify a subset of
-                    jobs to retrieve
-        """
-        if tag is None:
-            return self.jobs[:]
-        else:
-            return [job for job in self.jobs if tag in job.tags]
-
-    def clear(self, tag: Optional[Hashable] = None) -> None:
-        """
-        Deletes scheduled jobs marked with the given tag, or all jobs
-        if tag is omitted.
-
-        :param tag: An identifier used to identify a subset of
-                    jobs to delete
-        """
-        if tag is None:
-            logger.debug("Deleting *all* jobs")
-            del self.jobs[:]
-        else:
-            logger.debug('Deleting all jobs tagged "%s"', tag)
-            self.jobs[:] = (job for job in self.jobs if tag not in job.tags)
-
-    def cancel_job(self, job: "Job") -> None:
-        """
-        Delete a scheduled job.
-
-        :param job: The job to be unscheduled
-        """
-        try:
-            logger.debug('Cancelling job "%s"', str(job))
-            self.jobs.remove(job)
-        except ValueError:
-            logger.debug('Cancelling not-scheduled job "%s"', str(job))
-
-    def every(self, interval: int = 1) -> "Job":
-        """
-        Schedule a new periodic job.
-
-        :param interval: A quantity of a certain time unit
-        :return: An unconfigured :class:`Job <Job>`
-        """
-        job = Job(interval, self)
-        return job
-
-    def _run_job(self, job: "Job") -> None:
-        ret = job.run()
-        if isinstance(ret, CancelJob) or ret is CancelJob:
-            self.cancel_job(job)
-
-    def get_next_run(self, tag: Optional[Hashable] = None) -> Optional[datetime.datetime]:
-        """
-        Datetime when the next job should run.
-
-        :param tag: Filter the next run for the given tag parameter
-
-        :return: A :class:`~datetime.datetime` object
-                 or None if no jobs scheduled
-        """
-        if not self.jobs:
-            return None
-        jobs_filtered = self.get_jobs(tag)
-        if not jobs_filtered:
-            return None
-        return min(jobs_filtered).next_run
-
-    next_run = property(get_next_run)
-
-    @property
-    def idle_seconds(self) -> Optional[float]:
-        """
-        :return: Number of seconds until
-                 :meth:`next_run <Scheduler.next_run>`
-                 or None if no jobs are scheduled
-        """
-        if not self.next_run:
-            return None
-        return (self.next_run - datetime.datetime.now()).total_seconds()
-
-
-class Job(object):
-    """
-    A periodic job as used by :class:`Scheduler`.
-
-    :param interval: A quantity of a certain time unit
-    :param scheduler: The :class:`Scheduler <Scheduler>` instance that
-                      this job will register itself with once it has
-                      been fully configured in :meth:`Job.do()`.
-
-    Every job runs at a given fixed time interval that is defined by:
-
-    * a :meth:`time unit <Job.second>`
-    * a quantity of `time units` defined by `interval`
-
-    A job is usually created and returned by :meth:`Scheduler.every`
-    method, which also defines its `interval`.
-    """
-
-    def __init__(self, interval: int, scheduler: Scheduler = None):
-        self.interval: int = interval  # pause interval * unit between runs
-        self.latest: Optional[int] = None  # upper limit to the interval
-        self.job_func: Optional[functools.partial] = None  # the job job_func to run
-
-        # time units, e.g. 'minutes', 'hours', ...
-        self.unit: Optional[str] = None
-
-        # optional time at which this job runs
-        self.at_time: Optional[datetime.time] = None
-
-        # optional time zone of the self.at_time field. Only relevant when at_time is not None
-        self.at_time_zone = None
-
-        # datetime of the last run
-        self.last_run: Optional[datetime.datetime] = None
-
-        # datetime of the next run
-        self.next_run: Optional[datetime.datetime] = None
-
-        # timedelta between runs, only valid for
-        self.period: Optional[datetime.timedelta] = None
-
-        # Specific day of the week to start on
-        self.start_day: Optional[str] = None
-
-        # optional time of final run
-        self.cancel_after: Optional[datetime.datetime] = None
-
-        self.tags: Set[Hashable] = set()  # unique set of tags for the job
-        self.scheduler: Optional[Scheduler] = scheduler  # scheduler to register with
-
-    def __lt__(self, other) -> bool:
-        """
-        PeriodicJobs are sortable based on the scheduled time they
-        run next.
-        """
-        return self.next_run < other.next_run
-
-    def __str__(self) -> str:
-        if hasattr(self.job_func, "__name__"):
-            job_func_name = self.job_func.__name__  # type: ignore
-        else:
-            job_func_name = repr(self.job_func)
-
-        return ("Job(interval={}, unit={}, do={}, args={}, kwargs={})").format(
-            self.interval,
-            self.unit,
-            job_func_name,
-            "()" if self.job_func is None else self.job_func.args,
-            "{}" if self.job_func is None else self.job_func.keywords,
-        )
-
-    def __repr__(self):
-        def format_time(t):
-            return t.strftime("%Y-%m-%d %H:%M:%S") if t else "[never]"
-
-        def is_repr(j):
-            return not isinstance(j, Job)
-
-        timestats = "(last run: %s, next run: %s)" % (
-            format_time(self.last_run),
-            format_time(self.next_run),
-        )
-
-        if hasattr(self.job_func, "__name__"):
-            job_func_name = self.job_func.__name__
-        else:
-            job_func_name = repr(self.job_func)
-        args = [repr(x) if is_repr(x) else str(x) for x in self.job_func.args]
-        kwargs = ["%s=%s" % (k, repr(v)) for k, v in self.job_func.keywords.items()]
-        call_repr = job_func_name + "(" + ", ".join(args + kwargs) + ")"
-
-        if self.at_time is not None:
-            return "Every %s %s %s at %s do %s %s" % (
-                self.interval,
-                self.unit[:-1] if self.interval == 1 else self.unit,
-                self.month_day if self.unit == "month_on" else "",
-                self.at_time,
-                call_repr,
-                timestats,
-            )
-        else:
-            fmt = (
-                    "Every %(interval)s "
-                    + ("to %(latest)s " if self.latest is not None else "")
-                    + "%(unit)s do %(call_repr)s %(timestats)s"
-            )
-
-            return fmt % dict(
-                interval=self.interval,
-                latest=self.latest,
-                unit=(self.unit[:-1] if self.interval == 1 else self.unit),
-                call_repr=call_repr,
-                timestats=timestats,
-            )
-
-    @property
-    def second(self):
-        if self.interval != 1:
-            raise IntervalError("Use seconds instead of second")
-        return self.seconds
-
-    @property
-    def seconds(self):
-        self.unit = "seconds"
-        return self
-
-    @property
-    def minute(self):
-        if self.interval != 1:
-            raise IntervalError("Use minutes instead of minute")
-        return self.minutes
-
-    @property
-    def minutes(self):
-        self.unit = "minutes"
-        return self
-
-    @property
-    def hour(self):
-        if self.interval != 1:
-            raise IntervalError("Use hours instead of hour")
-        return self.hours
-
-    @property
-    def hours(self):
-        self.unit = "hours"
-        return self
-
-    @property
-    def day(self):
-        if self.interval != 1:
-            raise IntervalError("Use days instead of day")
-        return self.days
-
-    @property
-    def days(self):
-        self.unit = "days"
-        return self
-
-    @property
-    def week(self):
-        if self.interval != 1:
-            raise IntervalError("Use weeks instead of week")
-        return self.weeks
-
-    @property
-    def weeks(self):
-        self.unit = "weeks"
-        return self
-
-    @property
-    def monday(self):
-        if self.interval != 1:
-            raise IntervalError(
-                "Scheduling .monday() jobs is only allowed for weekly jobs. "
-                "Using .monday() on a job scheduled to run every 2 or more weeks "
-                "is not supported."
-            )
-        self.start_day = "monday"
-        return self.weeks
-
-    @property
-    def tuesday(self):
-        if self.interval != 1:
-            raise IntervalError(
-                "Scheduling .tuesday() jobs is only allowed for weekly jobs. "
-                "Using .tuesday() on a job scheduled to run every 2 or more weeks "
-                "is not supported."
-            )
-        self.start_day = "tuesday"
-        return self.weeks
-
-    @property
-    def wednesday(self):
-        if self.interval != 1:
-            raise IntervalError(
-                "Scheduling .wednesday() jobs is only allowed for weekly jobs. "
-                "Using .wednesday() on a job scheduled to run every 2 or more weeks "
-                "is not supported."
-            )
-        self.start_day = "wednesday"
-        return self.weeks
-
-    @property
-    def thursday(self):
-        if self.interval != 1:
-            raise IntervalError(
-                "Scheduling .thursday() jobs is only allowed for weekly jobs. "
-                "Using .thursday() on a job scheduled to run every 2 or more weeks "
-                "is not supported."
-            )
-        self.start_day = "thursday"
-        return self.weeks
-
-    @property
-    def friday(self):
-        if self.interval != 1:
-            raise IntervalError(
-                "Scheduling .friday() jobs is only allowed for weekly jobs. "
-                "Using .friday() on a job scheduled to run every 2 or more weeks "
-                "is not supported."
-            )
-        self.start_day = "friday"
-        return self.weeks
-
-    @property
-    def saturday(self):
-        if self.interval != 1:
-            raise IntervalError(
-                "Scheduling .saturday() jobs is only allowed for weekly jobs. "
-                "Using .saturday() on a job scheduled to run every 2 or more weeks "
-                "is not supported."
-            )
-        self.start_day = "saturday"
-        return self.weeks
-
-    @property
-    def sunday(self):
-        if self.interval != 1:
-            raise IntervalError(
-                "Scheduling .sunday() jobs is only allowed for weekly jobs. "
-                "Using .sunday() on a job scheduled to run every 2 or more weeks "
-                "is not supported."
-            )
-        self.start_day = "sunday"
-        return self.weeks
-
-    def month_on(self, month_day):
-        if self.interval != 1:
-            raise IntervalError(
-                "Scheduling .month_on(d) jobs is only allowed for monthly jobs. "
-                "Using .month_on(d) on a job scheduled to run every 2 or more months "
-                "is not supported."
-            )
-        self.unit = "month_on"
-        self.month_day = month_day
-        return self
-
-    def tag(self, *tags: Hashable):
-        """
-        Tags the job with one or more unique identifiers.
-
-        Tags must be hashable. Duplicate tags are discarded.
-
-        :param tags: A unique list of ``Hashable`` tags.
-        :return: The invoked job instance
-        """
-        if not all(isinstance(tag, Hashable) for tag in tags):
-            raise TypeError("Tags must be hashable")
-        self.tags.update(tags)
-        return self
-
-    def at(self, time_str: str, tz: str = None):
-
-        """
-        Specify a particular time that the job should be run at.
-
-        :param time_str: A string in one of the following formats:
-
-            - For daily jobs -> `HH:MM:SS` or `HH:MM`
-            - For hourly jobs -> `MM:SS` or `:MM`
-            - For minute jobs -> `:SS`
-
-            The format must make sense given how often the job is
-            repeating; for example, a job that repeats every minute
-            should not be given a string in the form `HH:MM:SS`. The
-            difference between `:MM` and `:SS` is inferred from the
-            selected time-unit (e.g. `every().hour.at(':30')` vs.
-            `every().minute.at(':30')`).
-
-        :param tz: The timezone that this timestamp refers to. Can be
-            a string that can be parsed by pytz.timezone(), or a pytz.BaseTzInfo object
-
-        :return: The invoked job instance
-        """
-        if self.unit not in ("days", "hours", "minutes", "month_on") and not self.start_day:
-            raise ScheduleValueError(
-                "Invalid unit (valid units are `days`, `hours`, and `minutes` and 'month_on')"
-            )
-
-        if tz is not None:
-            import pytz
-
-            if isinstance(tz, str):
-                self.at_time_zone = pytz.timezone(tz)  # type: ignore
-            elif isinstance(tz, pytz.BaseTzInfo):
-                self.at_time_zone = tz
-            else:
-                raise ScheduleValueError(
-                    "Timezone must be string or pytz.timezone object"
-                )
-
-        if not isinstance(time_str, str):
-            raise TypeError("at() should be passed a string")
-        if self.unit == "days" or self.start_day or self.unit == "month_on":
-            if not re.match(r"^[0-2]\d:[0-5]\d(:[0-5]\d)?$", time_str):
-                raise ScheduleValueError(
-                    "Invalid time format for a daily job (valid format is HH:MM(:SS)?)"
-                )
-        if self.unit == "hours":
-            if not re.match(r"^([0-5]\d)?:[0-5]\d$", time_str):
-                raise ScheduleValueError(
-                    "Invalid time format for an hourly job (valid format is (MM)?:SS)"
-                )
-
-        if self.unit == "minutes":
-            if not re.match(r"^:[0-5]\d$", time_str):
-                raise ScheduleValueError(
-                    "Invalid time format for a minutely job (valid format is :SS)"
-                )
-        time_values = time_str.split(":")
-        hour: Union[str, int]
-        minute: Union[str, int]
-        second: Union[str, int]
-        if len(time_values) == 3:
-            hour, minute, second = time_values
-        elif len(time_values) == 2 and self.unit == "minutes":
-            hour = 0
-            minute = 0
-            _, second = time_values
-        elif len(time_values) == 2 and self.unit == "hours" and len(time_values[0]):
-            hour = 0
-            minute, second = time_values
-        else:
-            hour, minute = time_values
-            second = 0
-        if self.unit == "days" or self.start_day or self.unit == "month_on":
-            hour = int(hour)
-            if not (0 <= hour <= 23):
-                raise ScheduleValueError(
-                    "Invalid number of hours ({} is not between 0 and 23)"
-                )
-        elif self.unit == "hours":
-            hour = 0
-        elif self.unit == "minutes":
-            hour = 0
-            minute = 0
-        hour = int(hour)
-        minute = int(minute)
-        second = int(second)
-        self.at_time = datetime.time(hour, minute, second)
-        return self
-
-    def to(self, latest: int):
-        """
-        Schedule the job to run at an irregular (randomized) interval.
-
-        The job's interval will randomly vary from the value given
-        to  `every` to `latest`. The range defined is inclusive on
-        both ends. For example, `every(A).to(B).seconds` executes
-        the job function every N seconds such that A <= N <= B.
-
-        :param latest: Maximum interval between randomized job runs
-        :return: The invoked job instance
-        """
-        self.latest = latest
-        return self
-
-    def until(
-            self,
-            until_time: Union[datetime.datetime, datetime.timedelta, datetime.time, str],
-    ):
-        """
-        Schedule job to run until the specified moment.
-
-        The job is canceled whenever the next run is calculated and it turns out the
-        next run is after the until_time. The job is also canceled right before it runs,
-        if the current time is after until_time. This latter case can happen when the
-        the job was scheduled to run before until_time, but runs after until_time.
-
-        If until_time is a moment in the past, ScheduleValueError is thrown.
-
-        :param until_time: A moment in the future representing the latest time a job can
-           be run. If only a time is supplied, the date is set to today.
-           The following formats are accepted:
-
-           - datetime.datetime
-           - datetime.timedelta
-           - datetime.time
-           - String in one of the following formats: "%Y-%m-%d %H:%M:%S",
-             "%Y-%m-%d %H:%M", "%Y-%m-%d", "%H:%M:%S", "%H:%M"
-             as defined by strptime() behaviour. If an invalid string format is passed,
-             ScheduleValueError is thrown.
-
-        :return: The invoked job instance
-        """
-
-        if isinstance(until_time, datetime.datetime):
-            self.cancel_after = until_time
-        elif isinstance(until_time, datetime.timedelta):
-            self.cancel_after = datetime.datetime.now() + until_time
-        elif isinstance(until_time, datetime.time):
-            self.cancel_after = datetime.datetime.combine(
-                datetime.datetime.now(), until_time
-            )
-        elif isinstance(until_time, str):
-            cancel_after = self._decode_datetimestr(
-                until_time,
-                [
-                    "%Y-%m-%d %H:%M:%S",
-                    "%Y-%m-%d %H:%M",
-                    "%Y-%m-%d",
-                    "%H:%M:%S",
-                    "%H:%M",
-                ],
-            )
-            if cancel_after is None:
-                raise ScheduleValueError("Invalid string format for until()")
-            if "-" not in until_time:
-                # the until_time is a time-only format. Set the date to today
-                now = datetime.datetime.now()
-                cancel_after = cancel_after.replace(
-                    year=now.year, month=now.month, day=now.day
-                )
-            self.cancel_after = cancel_after
-        else:
-            raise TypeError(
-                "until() takes a string, datetime.datetime, datetime.timedelta, "
-                "datetime.time parameter"
-            )
-        if self.cancel_after < datetime.datetime.now():
-            raise ScheduleValueError(
-                "Cannot schedule a job to run until a time in the past"
-            )
-        return self
-
-    def do(self, job_func: Callable, *args, **kwargs):
-        """
-        Specifies the job_func that should be called every time the
-        job runs.
-
-        Any additional arguments are passed on to job_func when
-        the job runs.
-
-        :param job_func: The function to be scheduled
-        :return: The invoked job instance
-        """
-        self.job_func = functools.partial(job_func, *args, **kwargs)
-        functools.update_wrapper(self.job_func, job_func)
-        self._schedule_next_run()
-        if self.scheduler is None:
-            raise ScheduleError(
-                "Unable to a add job to schedule. "
-                "Job is not associated with an scheduler"
-            )
-        self.scheduler.jobs.append(self)
-        return self
-
-    @property
-    def should_run(self) -> bool:
-        """
-        :return: ``True`` if the job should be run now.
-        """
-        assert self.next_run is not None, "must run _schedule_next_run before"
-        return datetime.datetime.now() >= self.next_run
-
-    def run(self):
-        """
-        Run the job and immediately reschedule it.
-        If the job's deadline is reached (configured using .until()), the job is not
-        run and CancelJob is returned immediately. If the next scheduled run exceeds
-        the job's deadline, CancelJob is returned after the execution. In this latter
-        case CancelJob takes priority over any other returned value.
-
-        :return: The return value returned by the `job_func`, or CancelJob if the job's
-                 deadline is reached.
-
-        """
-        if self._is_overdue(datetime.datetime.now()):
-            logger.debug("Cancelling job %s", self)
-            return CancelJob
-
-        logger.debug("Running job %s", self)
-        ret = self.job_func()
-        self.last_run = datetime.datetime.now()
-        self._schedule_next_run()
-
-        if self._is_overdue(self.next_run):
-            logger.debug("Cancelling job %s", self)
-            return CancelJob
-        return ret
-
-    def _schedule_next_run(self) -> None:
-        """
-        Compute the instant when this job should run next.
-        """
-        if self.unit not in ("seconds", "minutes", "hours", "days", "weeks", "month_on"):
-            raise ScheduleValueError(
-                "Invalid unit (valid units are `seconds`, `minutes`, `hours`, "
-                "`days`, and `weeks` and 'month_on')"
-            )
-
-        if self.latest is not None:
-            if not (self.latest >= self.interval):
-                raise ScheduleError("`latest` is greater than `interval`")
-            interval = random.randint(self.interval, self.latest)
-        else:
-            interval = self.interval
-
-        # Special case for .month_on(d)
-        if self.unit == "month_on":
-            # We search for le period of the next run. <start> to know if already run or not.
-            start = 0 if not self.last_run else 1
-            day_delta = 0
-            highest_day = 0
-            next_date = datetime.datetime.now()
-            for day in range(start, 32):
-                next_date += datetime.timedelta(days=1)
-                if next_date.day == self.month_day:
-                    day_delta = day
-                    break
-                if next_date.day > highest_day:
-                    highest_day = next_date.day
-                    day_delta = day
-            self.period = datetime.timedelta(days=day_delta)
-        else:
-            self.period = datetime.timedelta(**{self.unit: interval})
-
-        self.next_run = datetime.datetime.now() + self.period
-        if self.start_day is not None:
-            if self.unit != "weeks":
-                raise ScheduleValueError("`unit` should be 'weeks'")
-            weekdays = (
-                "monday",
-                "tuesday",
-                "wednesday",
-                "thursday",
-                "friday",
-                "saturday",
-                "sunday",
-            )
-            if self.start_day not in weekdays:
-                raise ScheduleValueError(
-                    "Invalid start day (valid start days are {})".format(weekdays)
-                )
-            weekday = weekdays.index(self.start_day)
-            days_ahead = weekday - self.next_run.weekday()
-            if days_ahead <= 0:  # Target day already happened this week
-                days_ahead += 7
-            self.next_run += datetime.timedelta(days_ahead) - self.period
-        if self.at_time is not None:
-            if self.unit not in ("days", "hours", "minutes", "month_on") and self.start_day is None:
-                raise ScheduleValueError("Invalid unit without specifying start day")
-            kwargs = {"second": self.at_time.second, "microsecond": 0}
-            if self.unit == "days" or self.start_day is not None or self.unit == "month_on":
-                kwargs["hour"] = self.at_time.hour
-            if self.unit in ["days", "hours", "month_on"] or self.start_day is not None:
-                kwargs["minute"] = self.at_time.minute
-            self.next_run = self.next_run.replace(**kwargs)  # type: ignore
-
-            if self.at_time_zone is not None:
-                # Convert next_run from the expected timezone into the local time
-                # self.next_run is a naive datetime so after conversion remove tzinfo
-                self.next_run = (
-                    self.at_time_zone.localize(self.next_run)
-                        .astimezone()
-                        .replace(tzinfo=None)
-                )
-
-            # Make sure we run at the specified time *today* (or *this hour*)
-            # as well. This accounts for when a job takes so long it finished
-            # in the next period.
-            # With month_on we consider a job can’t run so long.
-            if not self.last_run or (self.next_run - self.last_run) > self.period:
-                now = datetime.datetime.now()
-                if (
-                        self.unit == "days"
-                        and self.at_time > now.time()
-                        and self.interval == 1
-                ):
-                    self.next_run = self.next_run - datetime.timedelta(days=1)
-                elif self.unit == "hours" and (
-                        self.at_time.minute > now.minute
-                        or (
-                                self.at_time.minute == now.minute
-                                and self.at_time.second > now.second
-                        )
-                ):
-                    self.next_run = self.next_run - datetime.timedelta(hours=1)
-                elif self.unit == "minutes" and self.at_time.second > now.second:
-                    self.next_run = self.next_run - datetime.timedelta(minutes=1)
-        if self.start_day is not None and self.at_time is not None:
-            # Let's see if we will still make that time we specified today
-            if (self.next_run - datetime.datetime.now()).days >= 7:
-                self.next_run -= self.period
-
-    def _is_overdue(self, when: datetime.datetime):
-        return self.cancel_after is not None and when > self.cancel_after
-
-    def _decode_datetimestr(
-            self, datetime_str: str, formats: List[str]
-    ) -> Optional[datetime.datetime]:
-        for f in formats:
-            try:
-                return datetime.datetime.strptime(datetime_str, f)
-            except ValueError:
-                pass
-        return None
-
-
-# The following methods are shortcuts for not having to
-# create a Scheduler instance:
-
-#: Default :class:`Scheduler <Scheduler>` object
-default_scheduler = Scheduler()
-
-#: Default :class:`Jobs <Job>` list
-jobs = default_scheduler.jobs  # todo: should this be a copy, e.g. jobs()?
-
-
-def every(interval: int = 1) -> Job:
-    """Calls :meth:`every <Scheduler.every>` on the
-    :data:`default scheduler instance <default_scheduler>`.
-    """
-    return default_scheduler.every(interval)
-
-
-def run_pending() -> None:
-    """Calls :meth:`run_pending <Scheduler.run_pending>` on the
-    :data:`default scheduler instance <default_scheduler>`.
-    """
-    default_scheduler.run_pending()
-
-
-def run_all(delay_seconds: int = 0) -> None:
-    """Calls :meth:`run_all <Scheduler.run_all>` on the
-    :data:`default scheduler instance <default_scheduler>`.
-    """
-    default_scheduler.run_all(delay_seconds=delay_seconds)
-
-
-def get_jobs(tag: Optional[Hashable] = None) -> List[Job]:
-    """Calls :meth:`get_jobs <Scheduler.get_jobs>` on the
-    :data:`default scheduler instance <default_scheduler>`.
-    """
-    return default_scheduler.get_jobs(tag)
-
-
-def clear(tag: Optional[Hashable] = None) -> None:
-    """Calls :meth:`clear <Scheduler.clear>` on the
-    :data:`default scheduler instance <default_scheduler>`.
-    """
-    default_scheduler.clear(tag)
-
-
-def cancel_job(job: Job) -> None:
-    """Calls :meth:`cancel_job <Scheduler.cancel_job>` on the
-    :data:`default scheduler instance <default_scheduler>`.
-    """
-    default_scheduler.cancel_job(job)
-
-
-def next_run(tag: Optional[Hashable] = None) -> Optional[datetime.datetime]:
-    """Calls :meth:`next_run <Scheduler.next_run>` on the
-    :data:`default scheduler instance <default_scheduler>`.
-    """
-    return default_scheduler.get_next_run(tag)
-
-
-def idle_seconds() -> Optional[float]:
-    """Calls :meth:`idle_seconds <Scheduler.idle_seconds>` on the
-    :data:`default scheduler instance <default_scheduler>`.
-    """
-    return default_scheduler.idle_seconds
-
-
-def repeat(job, *args, **kwargs):
-    """
-    Decorator to schedule a new periodic job.
-
-    Any additional arguments are passed on to the decorated function
-    when the job runs.
-
-    :param job: a :class:`Jobs <Job>`
-    """
-
-    def _schedule_decorator(decorated_function):
-        job.do(decorated_function, *args, **kwargs)
-        return decorated_function
-
-    return _schedule_decorator
+"""
+Python job scheduling for humans.
+
+github.com/dbader/schedule
+
+An in-process scheduler for periodic jobs that uses the builder pattern
+for configuration. Schedule lets you run Python functions (or any other
+callable) periodically at pre-determined intervals using a simple,
+human-friendly syntax.
+
+Inspired by Addam Wiggins' article "Rethinking Cron" [1] and the
+"clockwork" Ruby module [2][3].
+
+Features:
+    - A simple to use API for scheduling jobs.
+    - Very lightweight and no external dependencies.
+    - Excellent test coverage.
+    - Tested on Python 3.6, 3.7, 3.8, 3.9
+
+Usage:
+    import schedule
+    import time
+
+    def job(message='stuff'):
+        print("I'm working on:", message)
+
+    schedule.every(10).minutes.do(job)
+    schedule.every(5).to(10).days.do(job)
+    schedule.every().hour.do(job, message='things')
+    schedule.every().day.at("10:30").do(job)
+
+    while True:
+        schedule.run_pending()
+        time.sleep(1)
+
+[1] https://adam.herokuapp.com/past/2010/4/13/rethinking_cron/
+[2] https://github.com/Rykian/clockwork
+[3] https://adam.herokuapp.com/past/2010/6/30/replace_cron_with_clockwork/
+"""
+from collections.abc import Hashable
+import datetime
+import functools
+import logging
+import random
+import re
+import time
+from typing import Set, List, Optional, Callable, Union
+
+logger = logging.getLogger("schedule")
+
+
+class ScheduleError(Exception):
+    """Base schedule exception"""
+
+    pass
+
+
+class ScheduleValueError(ScheduleError):
+    """Base schedule value error"""
+
+    pass
+
+
+class IntervalError(ScheduleValueError):
+    """An improper interval was used"""
+
+    pass
+
+
+class CancelJob(object):
+    """
+    Can be returned from a job to unschedule itself.
+    """
+
+    pass
+
+
+class Scheduler(object):
+    """
+    Objects instantiated by the :class:`Scheduler <Scheduler>` are
+    factories to create jobs, keep record of scheduled jobs and
+    handle their execution.
+    """
+
+    def __init__(self) -> None:
+        self.jobs: List[Job] = []
+
+    def run_pending(self) -> None:
+        """
+        Run all jobs that are scheduled to run.
+
+        Please note that it is *intended behavior that run_pending()
+        does not run missed jobs*. For example, if you've registered a job
+        that should run every minute and you only call run_pending()
+        in one hour increments then your job won't be run 60 times in
+        between but only once.
+        """
+        runnable_jobs = (job for job in self.jobs if job.should_run)
+        for job in sorted(runnable_jobs):
+            self._run_job(job)
+
+    def run_all(self, delay_seconds: int = 0) -> None:
+        """
+        Run all jobs regardless if they are scheduled to run or not.
+
+        A delay of `delay` seconds is added between each job. This helps
+        distribute system load generated by the jobs more evenly
+        over time.
+
+        :param delay_seconds: A delay added between every executed job
+        """
+        logger.debug(
+            "Running *all* %i jobs with %is delay in between",
+            len(self.jobs),
+            delay_seconds,
+        )
+        for job in self.jobs[:]:
+            self._run_job(job)
+            time.sleep(delay_seconds)
+
+    def get_jobs(self, tag: Optional[Hashable] = None) -> List["Job"]:
+        """
+        Gets scheduled jobs marked with the given tag, or all jobs
+        if tag is omitted.
+
+        :param tag: An identifier used to identify a subset of
+                    jobs to retrieve
+        """
+        if tag is None:
+            return self.jobs[:]
+        else:
+            return [job for job in self.jobs if tag in job.tags]
+
+    def clear(self, tag: Optional[Hashable] = None) -> None:
+        """
+        Deletes scheduled jobs marked with the given tag, or all jobs
+        if tag is omitted.
+
+        :param tag: An identifier used to identify a subset of
+                    jobs to delete
+        """
+        if tag is None:
+            logger.debug("Deleting *all* jobs")
+            del self.jobs[:]
+        else:
+            logger.debug('Deleting all jobs tagged "%s"', tag)
+            self.jobs[:] = (job for job in self.jobs if tag not in job.tags)
+
+    def cancel_job(self, job: "Job") -> None:
+        """
+        Delete a scheduled job.
+
+        :param job: The job to be unscheduled
+        """
+        try:
+            logger.debug('Cancelling job "%s"', str(job))
+            self.jobs.remove(job)
+        except ValueError:
+            logger.debug('Cancelling not-scheduled job "%s"', str(job))
+
+    def every(self, interval: int = 1) -> "Job":
+        """
+        Schedule a new periodic job.
+
+        :param interval: A quantity of a certain time unit
+        :return: An unconfigured :class:`Job <Job>`
+        """
+        job = Job(interval, self)
+        return job
+
+    def _run_job(self, job: "Job") -> None:
+        ret = job.run()
+        if isinstance(ret, CancelJob) or ret is CancelJob:
+            self.cancel_job(job)
+
+    def get_next_run(self, tag: Optional[Hashable] = None) -> Optional[datetime.datetime]:
+        """
+        Datetime when the next job should run.
+
+        :param tag: Filter the next run for the given tag parameter
+
+        :return: A :class:`~datetime.datetime` object
+                 or None if no jobs scheduled
+        """
+        if not self.jobs:
+            return None
+        jobs_filtered = self.get_jobs(tag)
+        if not jobs_filtered:
+            return None
+        return min(jobs_filtered).next_run
+
+    next_run = property(get_next_run)
+
+    @property
+    def idle_seconds(self) -> Optional[float]:
+        """
+        :return: Number of seconds until
+                 :meth:`next_run <Scheduler.next_run>`
+                 or None if no jobs are scheduled
+        """
+        if not self.next_run:
+            return None
+        return (self.next_run - datetime.datetime.now()).total_seconds()
+
+
+class Job(object):
+    """
+    A periodic job as used by :class:`Scheduler`.
+
+    :param interval: A quantity of a certain time unit
+    :param scheduler: The :class:`Scheduler <Scheduler>` instance that
+                      this job will register itself with once it has
+                      been fully configured in :meth:`Job.do()`.
+
+    Every job runs at a given fixed time interval that is defined by:
+
+    * a :meth:`time unit <Job.second>`
+    * a quantity of `time units` defined by `interval`
+
+    A job is usually created and returned by :meth:`Scheduler.every`
+    method, which also defines its `interval`.
+    """
+
+    def __init__(self, interval: int, scheduler: Scheduler = None):
+        self.interval: int = interval  # pause interval * unit between runs
+        self.latest: Optional[int] = None  # upper limit to the interval
+        self.job_func: Optional[functools.partial] = None  # the job job_func to run
+
+        # time units, e.g. 'minutes', 'hours', ...
+        self.unit: Optional[str] = None
+
+        # optional time at which this job runs
+        self.at_time: Optional[datetime.time] = None
+
+        # optional time zone of the self.at_time field. Only relevant when at_time is not None
+        self.at_time_zone = None
+
+        # datetime of the last run
+        self.last_run: Optional[datetime.datetime] = None
+
+        # datetime of the next run
+        self.next_run: Optional[datetime.datetime] = None
+
+        # timedelta between runs, only valid for
+        self.period: Optional[datetime.timedelta] = None
+
+        # Specific day of the week to start on
+        self.start_day: Optional[str] = None
+
+        # optional time of final run
+        self.cancel_after: Optional[datetime.datetime] = None
+
+        self.tags: Set[Hashable] = set()  # unique set of tags for the job
+        self.scheduler: Optional[Scheduler] = scheduler  # scheduler to register with
+
+    def __lt__(self, other) -> bool:
+        """
+        PeriodicJobs are sortable based on the scheduled time they
+        run next.
+        """
+        return self.next_run < other.next_run
+
+    def __str__(self) -> str:
+        if hasattr(self.job_func, "__name__"):
+            job_func_name = self.job_func.__name__  # type: ignore
+        else:
+            job_func_name = repr(self.job_func)
+
+        return ("Job(interval={}, unit={}, do={}, args={}, kwargs={})").format(
+            self.interval,
+            self.unit,
+            job_func_name,
+            "()" if self.job_func is None else self.job_func.args,
+            "{}" if self.job_func is None else self.job_func.keywords,
+        )
+
+    def __repr__(self):
+        def format_time(t):
+            return t.strftime("%Y-%m-%d %H:%M:%S") if t else "[never]"
+
+        def is_repr(j):
+            return not isinstance(j, Job)
+
+        timestats = "(last run: %s, next run: %s)" % (
+            format_time(self.last_run),
+            format_time(self.next_run),
+        )
+
+        if hasattr(self.job_func, "__name__"):
+            job_func_name = self.job_func.__name__
+        else:
+            job_func_name = repr(self.job_func)
+        args = [repr(x) if is_repr(x) else str(x) for x in self.job_func.args]
+        kwargs = ["%s=%s" % (k, repr(v)) for k, v in self.job_func.keywords.items()]
+        call_repr = job_func_name + "(" + ", ".join(args + kwargs) + ")"
+
+        if self.at_time is not None:
+            return "Every %s %s %s at %s do %s %s" % (
+                self.interval,
+                self.unit[:-1] if self.interval == 1 else self.unit,
+                self.month_day if self.unit == "month_on" else "",
+                self.at_time,
+                call_repr,
+                timestats,
+            )
+        else:
+            fmt = (
+                    "Every %(interval)s "
+                    + ("to %(latest)s " if self.latest is not None else "")
+                    + "%(unit)s do %(call_repr)s %(timestats)s"
+            )
+
+            return fmt % dict(
+                interval=self.interval,
+                latest=self.latest,
+                unit=(self.unit[:-1] if self.interval == 1 else self.unit),
+                call_repr=call_repr,
+                timestats=timestats,
+            )
+
+    @property
+    def second(self):
+        if self.interval != 1:
+            raise IntervalError("Use seconds instead of second")
+        return self.seconds
+
+    @property
+    def seconds(self):
+        self.unit = "seconds"
+        return self
+
+    @property
+    def minute(self):
+        if self.interval != 1:
+            raise IntervalError("Use minutes instead of minute")
+        return self.minutes
+
+    @property
+    def minutes(self):
+        self.unit = "minutes"
+        return self
+
+    @property
+    def hour(self):
+        if self.interval != 1:
+            raise IntervalError("Use hours instead of hour")
+        return self.hours
+
+    @property
+    def hours(self):
+        self.unit = "hours"
+        return self
+
+    @property
+    def day(self):
+        if self.interval != 1:
+            raise IntervalError("Use days instead of day")
+        return self.days
+
+    @property
+    def days(self):
+        self.unit = "days"
+        return self
+
+    @property
+    def week(self):
+        if self.interval != 1:
+            raise IntervalError("Use weeks instead of week")
+        return self.weeks
+
+    @property
+    def weeks(self):
+        self.unit = "weeks"
+        return self
+
+    @property
+    def monday(self):
+        if self.interval != 1:
+            raise IntervalError(
+                "Scheduling .monday() jobs is only allowed for weekly jobs. "
+                "Using .monday() on a job scheduled to run every 2 or more weeks "
+                "is not supported."
+            )
+        self.start_day = "monday"
+        return self.weeks
+
+    @property
+    def tuesday(self):
+        if self.interval != 1:
+            raise IntervalError(
+                "Scheduling .tuesday() jobs is only allowed for weekly jobs. "
+                "Using .tuesday() on a job scheduled to run every 2 or more weeks "
+                "is not supported."
+            )
+        self.start_day = "tuesday"
+        return self.weeks
+
+    @property
+    def wednesday(self):
+        if self.interval != 1:
+            raise IntervalError(
+                "Scheduling .wednesday() jobs is only allowed for weekly jobs. "
+                "Using .wednesday() on a job scheduled to run every 2 or more weeks "
+                "is not supported."
+            )
+        self.start_day = "wednesday"
+        return self.weeks
+
+    @property
+    def thursday(self):
+        if self.interval != 1:
+            raise IntervalError(
+                "Scheduling .thursday() jobs is only allowed for weekly jobs. "
+                "Using .thursday() on a job scheduled to run every 2 or more weeks "
+                "is not supported."
+            )
+        self.start_day = "thursday"
+        return self.weeks
+
+    @property
+    def friday(self):
+        if self.interval != 1:
+            raise IntervalError(
+                "Scheduling .friday() jobs is only allowed for weekly jobs. "
+                "Using .friday() on a job scheduled to run every 2 or more weeks "
+                "is not supported."
+            )
+        self.start_day = "friday"
+        return self.weeks
+
+    @property
+    def saturday(self):
+        if self.interval != 1:
+            raise IntervalError(
+                "Scheduling .saturday() jobs is only allowed for weekly jobs. "
+                "Using .saturday() on a job scheduled to run every 2 or more weeks "
+                "is not supported."
+            )
+        self.start_day = "saturday"
+        return self.weeks
+
+    @property
+    def sunday(self):
+        if self.interval != 1:
+            raise IntervalError(
+                "Scheduling .sunday() jobs is only allowed for weekly jobs. "
+                "Using .sunday() on a job scheduled to run every 2 or more weeks "
+                "is not supported."
+            )
+        self.start_day = "sunday"
+        return self.weeks
+
+    def month_on(self, month_day):
+        if self.interval != 1:
+            raise IntervalError(
+                "Scheduling .month_on(d) jobs is only allowed for monthly jobs. "
+                "Using .month_on(d) on a job scheduled to run every 2 or more months "
+                "is not supported."
+            )
+        self.unit = "month_on"
+        self.month_day = month_day
+        return self
+
+    def tag(self, *tags: Hashable):
+        """
+        Tags the job with one or more unique identifiers.
+
+        Tags must be hashable. Duplicate tags are discarded.
+
+        :param tags: A unique list of ``Hashable`` tags.
+        :return: The invoked job instance
+        """
+        if not all(isinstance(tag, Hashable) for tag in tags):
+            raise TypeError("Tags must be hashable")
+        self.tags.update(tags)
+        return self
+
+    def at(self, time_str: str, tz: str = None):
+
+        """
+        Specify a particular time that the job should be run at.
+
+        :param time_str: A string in one of the following formats:
+
+            - For daily jobs -> `HH:MM:SS` or `HH:MM`
+            - For hourly jobs -> `MM:SS` or `:MM`
+            - For minute jobs -> `:SS`
+
+            The format must make sense given how often the job is
+            repeating; for example, a job that repeats every minute
+            should not be given a string in the form `HH:MM:SS`. The
+            difference between `:MM` and `:SS` is inferred from the
+            selected time-unit (e.g. `every().hour.at(':30')` vs.
+            `every().minute.at(':30')`).
+
+        :param tz: The timezone that this timestamp refers to. Can be
+            a string that can be parsed by pytz.timezone(), or a pytz.BaseTzInfo object
+
+        :return: The invoked job instance
+        """
+        if self.unit not in ("days", "hours", "minutes", "month_on") and not self.start_day:
+            raise ScheduleValueError(
+                "Invalid unit (valid units are `days`, `hours`, and `minutes` and 'month_on')"
+            )
+
+        if tz is not None:
+            import pytz
+
+            if isinstance(tz, str):
+                self.at_time_zone = pytz.timezone(tz)  # type: ignore
+            elif isinstance(tz, pytz.BaseTzInfo):
+                self.at_time_zone = tz
+            else:
+                raise ScheduleValueError(
+                    "Timezone must be string or pytz.timezone object"
+                )
+
+        if not isinstance(time_str, str):
+            raise TypeError("at() should be passed a string")
+        if self.unit == "days" or self.start_day or self.unit == "month_on":
+            if not re.match(r"^[0-2]\d:[0-5]\d(:[0-5]\d)?$", time_str):
+                raise ScheduleValueError(
+                    "Invalid time format for a daily job (valid format is HH:MM(:SS)?)"
+                )
+        if self.unit == "hours":
+            if not re.match(r"^([0-5]\d)?:[0-5]\d$", time_str):
+                raise ScheduleValueError(
+                    "Invalid time format for an hourly job (valid format is (MM)?:SS)"
+                )
+
+        if self.unit == "minutes":
+            if not re.match(r"^:[0-5]\d$", time_str):
+                raise ScheduleValueError(
+                    "Invalid time format for a minutely job (valid format is :SS)"
+                )
+        time_values = time_str.split(":")
+        hour: Union[str, int]
+        minute: Union[str, int]
+        second: Union[str, int]
+        if len(time_values) == 3:
+            hour, minute, second = time_values
+        elif len(time_values) == 2 and self.unit == "minutes":
+            hour = 0
+            minute = 0
+            _, second = time_values
+        elif len(time_values) == 2 and self.unit == "hours" and len(time_values[0]):
+            hour = 0
+            minute, second = time_values
+        else:
+            hour, minute = time_values
+            second = 0
+        if self.unit == "days" or self.start_day or self.unit == "month_on":
+            hour = int(hour)
+            if not (0 <= hour <= 23):
+                raise ScheduleValueError(
+                    "Invalid number of hours ({} is not between 0 and 23)"
+                )
+        elif self.unit == "hours":
+            hour = 0
+        elif self.unit == "minutes":
+            hour = 0
+            minute = 0
+        hour = int(hour)
+        minute = int(minute)
+        second = int(second)
+        self.at_time = datetime.time(hour, minute, second)
+        return self
+
+    def to(self, latest: int):
+        """
+        Schedule the job to run at an irregular (randomized) interval.
+
+        The job's interval will randomly vary from the value given
+        to  `every` to `latest`. The range defined is inclusive on
+        both ends. For example, `every(A).to(B).seconds` executes
+        the job function every N seconds such that A <= N <= B.
+
+        :param latest: Maximum interval between randomized job runs
+        :return: The invoked job instance
+        """
+        self.latest = latest
+        return self
+
+    def until(
+            self,
+            until_time: Union[datetime.datetime, datetime.timedelta, datetime.time, str],
+    ):
+        """
+        Schedule job to run until the specified moment.
+
+        The job is canceled whenever the next run is calculated and it turns out the
+        next run is after the until_time. The job is also canceled right before it runs,
+        if the current time is after until_time. This latter case can happen when the
+        the job was scheduled to run before until_time, but runs after until_time.
+
+        If until_time is a moment in the past, ScheduleValueError is thrown.
+
+        :param until_time: A moment in the future representing the latest time a job can
+           be run. If only a time is supplied, the date is set to today.
+           The following formats are accepted:
+
+           - datetime.datetime
+           - datetime.timedelta
+           - datetime.time
+           - String in one of the following formats: "%Y-%m-%d %H:%M:%S",
+             "%Y-%m-%d %H:%M", "%Y-%m-%d", "%H:%M:%S", "%H:%M"
+             as defined by strptime() behaviour. If an invalid string format is passed,
+             ScheduleValueError is thrown.
+
+        :return: The invoked job instance
+        """
+
+        if isinstance(until_time, datetime.datetime):
+            self.cancel_after = until_time
+        elif isinstance(until_time, datetime.timedelta):
+            self.cancel_after = datetime.datetime.now() + until_time
+        elif isinstance(until_time, datetime.time):
+            self.cancel_after = datetime.datetime.combine(
+                datetime.datetime.now(), until_time
+            )
+        elif isinstance(until_time, str):
+            cancel_after = self._decode_datetimestr(
+                until_time,
+                [
+                    "%Y-%m-%d %H:%M:%S",
+                    "%Y-%m-%d %H:%M",
+                    "%Y-%m-%d",
+                    "%H:%M:%S",
+                    "%H:%M",
+                ],
+            )
+            if cancel_after is None:
+                raise ScheduleValueError("Invalid string format for until()")
+            if "-" not in until_time:
+                # the until_time is a time-only format. Set the date to today
+                now = datetime.datetime.now()
+                cancel_after = cancel_after.replace(
+                    year=now.year, month=now.month, day=now.day
+                )
+            self.cancel_after = cancel_after
+        else:
+            raise TypeError(
+                "until() takes a string, datetime.datetime, datetime.timedelta, "
+                "datetime.time parameter"
+            )
+        if self.cancel_after < datetime.datetime.now():
+            raise ScheduleValueError(
+                "Cannot schedule a job to run until a time in the past"
+            )
+        return self
+
+    def do(self, job_func: Callable, *args, **kwargs):
+        """
+        Specifies the job_func that should be called every time the
+        job runs.
+
+        Any additional arguments are passed on to job_func when
+        the job runs.
+
+        :param job_func: The function to be scheduled
+        :return: The invoked job instance
+        """
+        self.job_func = functools.partial(job_func, *args, **kwargs)
+        functools.update_wrapper(self.job_func, job_func)
+        self._schedule_next_run()
+        if self.scheduler is None:
+            raise ScheduleError(
+                "Unable to a add job to schedule. "
+                "Job is not associated with an scheduler"
+            )
+        self.scheduler.jobs.append(self)
+        return self
+
+    @property
+    def should_run(self) -> bool:
+        """
+        :return: ``True`` if the job should be run now.
+        """
+        assert self.next_run is not None, "must run _schedule_next_run before"
+        return datetime.datetime.now() >= self.next_run
+
+    def run(self):
+        """
+        Run the job and immediately reschedule it.
+        If the job's deadline is reached (configured using .until()), the job is not
+        run and CancelJob is returned immediately. If the next scheduled run exceeds
+        the job's deadline, CancelJob is returned after the execution. In this latter
+        case CancelJob takes priority over any other returned value.
+
+        :return: The return value returned by the `job_func`, or CancelJob if the job's
+                 deadline is reached.
+
+        """
+        if self._is_overdue(datetime.datetime.now()):
+            logger.debug("Cancelling job %s", self)
+            return CancelJob
+
+        logger.debug("Running job %s", self)
+        ret = self.job_func()
+        self.last_run = datetime.datetime.now()
+        self._schedule_next_run()
+
+        if self._is_overdue(self.next_run):
+            logger.debug("Cancelling job %s", self)
+            return CancelJob
+        return ret
+
+    def _schedule_next_run(self) -> None:
+        """
+        Compute the instant when this job should run next.
+        """
+        if self.unit not in ("seconds", "minutes", "hours", "days", "weeks", "month_on"):
+            raise ScheduleValueError(
+                "Invalid unit (valid units are `seconds`, `minutes`, `hours`, "
+                "`days`, and `weeks` and 'month_on')"
+            )
+
+        if self.latest is not None:
+            if not (self.latest >= self.interval):
+                raise ScheduleError("`latest` is greater than `interval`")
+            interval = random.randint(self.interval, self.latest)
+        else:
+            interval = self.interval
+
+        # Special case for .month_on(d)
+        if self.unit == "month_on":
+            # We search for le period of the next run. <start> to know if already run or not.
+            start = 0 if not self.last_run else 1
+            day_delta = 0
+            highest_day = 0
+            next_date = datetime.datetime.now()
+            for day in range(start, 32):
+                next_date += datetime.timedelta(days=1)
+                if next_date.day == self.month_day:
+                    day_delta = day
+                    break
+                if next_date.day > highest_day:
+                    highest_day = next_date.day
+                    day_delta = day
+            self.period = datetime.timedelta(days=day_delta)
+        else:
+            self.period = datetime.timedelta(**{self.unit: interval})
+
+        self.next_run = datetime.datetime.now() + self.period
+        if self.start_day is not None:
+            if self.unit != "weeks":
+                raise ScheduleValueError("`unit` should be 'weeks'")
+            weekdays = (
+                "monday",
+                "tuesday",
+                "wednesday",
+                "thursday",
+                "friday",
+                "saturday",
+                "sunday",
+            )
+            if self.start_day not in weekdays:
+                raise ScheduleValueError(
+                    "Invalid start day (valid start days are {})".format(weekdays)
+                )
+            weekday = weekdays.index(self.start_day)
+            days_ahead = weekday - self.next_run.weekday()
+            if days_ahead <= 0:  # Target day already happened this week
+                days_ahead += 7
+            self.next_run += datetime.timedelta(days_ahead) - self.period
+        if self.at_time is not None:
+            if self.unit not in ("days", "hours", "minutes", "month_on") and self.start_day is None:
+                raise ScheduleValueError("Invalid unit without specifying start day")
+            kwargs = {"second": self.at_time.second, "microsecond": 0}
+            if self.unit == "days" or self.start_day is not None or self.unit == "month_on":
+                kwargs["hour"] = self.at_time.hour
+            if self.unit in ["days", "hours", "month_on"] or self.start_day is not None:
+                kwargs["minute"] = self.at_time.minute
+            self.next_run = self.next_run.replace(**kwargs)  # type: ignore
+
+            if self.at_time_zone is not None:
+                # Convert next_run from the expected timezone into the local time
+                # self.next_run is a naive datetime so after conversion remove tzinfo
+                self.next_run = (
+                    self.at_time_zone.localize(self.next_run)
+                        .astimezone()
+                        .replace(tzinfo=None)
+                )
+
+            # Make sure we run at the specified time *today* (or *this hour*)
+            # as well. This accounts for when a job takes so long it finished
+            # in the next period.
+            # With month_on we consider a job can’t run so long.
+            if not self.last_run or (self.next_run - self.last_run) > self.period:
+                now = datetime.datetime.now()
+                if (
+                        self.unit == "days"
+                        and self.at_time > now.time()
+                        and self.interval == 1
+                ):
+                    self.next_run = self.next_run - datetime.timedelta(days=1)
+                elif self.unit == "hours" and (
+                        self.at_time.minute > now.minute
+                        or (
+                                self.at_time.minute == now.minute
+                                and self.at_time.second > now.second
+                        )
+                ):
+                    self.next_run = self.next_run - datetime.timedelta(hours=1)
+                elif self.unit == "minutes" and self.at_time.second > now.second:
+                    self.next_run = self.next_run - datetime.timedelta(minutes=1)
+        if self.start_day is not None and self.at_time is not None:
+            # Let's see if we will still make that time we specified today
+            if (self.next_run - datetime.datetime.now()).days >= 7:
+                self.next_run -= self.period
+
+    def _is_overdue(self, when: datetime.datetime):
+        return self.cancel_after is not None and when > self.cancel_after
+
+    def _decode_datetimestr(
+            self, datetime_str: str, formats: List[str]
+    ) -> Optional[datetime.datetime]:
+        for f in formats:
+            try:
+                return datetime.datetime.strptime(datetime_str, f)
+            except ValueError:
+                pass
+        return None
+
+
+# The following methods are shortcuts for not having to
+# create a Scheduler instance:
+
+#: Default :class:`Scheduler <Scheduler>` object
+default_scheduler = Scheduler()
+
+#: Default :class:`Jobs <Job>` list
+jobs = default_scheduler.jobs  # todo: should this be a copy, e.g. jobs()?
+
+
+def every(interval: int = 1) -> Job:
+    """Calls :meth:`every <Scheduler.every>` on the
+    :data:`default scheduler instance <default_scheduler>`.
+    """
+    return default_scheduler.every(interval)
+
+
+def run_pending() -> None:
+    """Calls :meth:`run_pending <Scheduler.run_pending>` on the
+    :data:`default scheduler instance <default_scheduler>`.
+    """
+    default_scheduler.run_pending()
+
+
+def run_all(delay_seconds: int = 0) -> None:
+    """Calls :meth:`run_all <Scheduler.run_all>` on the
+    :data:`default scheduler instance <default_scheduler>`.
+    """
+    default_scheduler.run_all(delay_seconds=delay_seconds)
+
+
+def get_jobs(tag: Optional[Hashable] = None) -> List[Job]:
+    """Calls :meth:`get_jobs <Scheduler.get_jobs>` on the
+    :data:`default scheduler instance <default_scheduler>`.
+    """
+    return default_scheduler.get_jobs(tag)
+
+
+def clear(tag: Optional[Hashable] = None) -> None:
+    """Calls :meth:`clear <Scheduler.clear>` on the
+    :data:`default scheduler instance <default_scheduler>`.
+    """
+    default_scheduler.clear(tag)
+
+
+def cancel_job(job: Job) -> None:
+    """Calls :meth:`cancel_job <Scheduler.cancel_job>` on the
+    :data:`default scheduler instance <default_scheduler>`.
+    """
+    default_scheduler.cancel_job(job)
+
+
+def next_run(tag: Optional[Hashable] = None) -> Optional[datetime.datetime]:
+    """Calls :meth:`next_run <Scheduler.next_run>` on the
+    :data:`default scheduler instance <default_scheduler>`.
+    """
+    return default_scheduler.get_next_run(tag)
+
+
+def idle_seconds() -> Optional[float]:
+    """Calls :meth:`idle_seconds <Scheduler.idle_seconds>` on the
+    :data:`default scheduler instance <default_scheduler>`.
+    """
+    return default_scheduler.idle_seconds
+
+
+def repeat(job, *args, **kwargs):
+    """
+    Decorator to schedule a new periodic job.
+
+    Any additional arguments are passed on to the decorated function
+    when the job runs.
+
+    :param job: a :class:`Jobs <Job>`
+    """
+
+    def _schedule_decorator(decorated_function):
+        job.do(decorated_function, *args, **kwargs)
+        return decorated_function
+
+    return _schedule_decorator
```

### Comparing `kometautils-0.1.0/kometautils/util.py` & `kometautils-0.2.0/kometautils/util.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,93 +1,93 @@
-import glob, time, os, requests
-from datetime import datetime, timedelta
-from pathlib import Path
-from pathvalidate import is_valid_filename, sanitize_filename
-from tqdm import tqdm
-from .exceptions import Failed
-
-def update_send(old_send, timeout):
-    def new_send(*send_args, **kwargs):
-        if kwargs.get("timeout", None) is None:
-            kwargs["timeout"] = timeout
-        return old_send(*send_args, **kwargs)
-    return new_send
-
-def glob_filter(filter_in):
-    filter_in = filter_in.translate({ord("["): "[[]", ord("]"): "[]]"}) if "[" in filter_in else filter_in
-    return glob.glob(filter_in)
-
-def is_locked(filepath):
-    locked = None
-    file_object = None
-    if Path(filepath).exists():
-        try:
-            file_object = open(filepath, "a", 8)
-            if file_object:
-                locked = False
-        except IOError:
-            locked = True
-        finally:
-            if file_object:
-                file_object.close()
-    return locked
-
-def validate_filename(filename):
-    if not is_valid_filename(str(filename)):
-        filename = sanitize_filename(str(filename))
-    return filename
-
-def download_image(download_image_url, path, name="temp"):
-    image_response = requests.get(download_image_url)
-    if image_response.status_code >= 400:
-        raise Failed("Image Error: Image Download Failed")
-    if image_response.headers["Content-Type"] not in ["image/png", "image/jpeg", "image/webp"]:
-        raise Failed("Image Error: Image Not PNG, JPG, or WEBP")
-    if image_response.headers["Content-Type"] == "image/jpeg":
-        temp_image_name = f"{name}.jpg"
-    elif image_response.headers["Content-Type"] == "image/webp":
-        temp_image_name = f"{name}.webp"
-    else:
-        temp_image_name = f"{name}.png"
-    temp_image_name = Path(path) / temp_image_name
-    with temp_image_name.open(mode="wb") as handler:
-        handler.write(image_response.content)
-    while is_locked(temp_image_name):
-        time.sleep(1)
-    return temp_image_name
-
-def move_path(file_path, old_base, new_base, suffix=None, append=True):
-    final_path = Path(new_base) / file_path.removeprefix(old_base)[1:]
-    final_path.mkdir(parents=True, exist_ok=True)
-    final_file = Path(f"{final_path}{suffix}" if suffix and append else str(final_path).removesuffix(suffix) if suffix else final_path)
-    Path(file_path).rename(final_file)
-    return final_file
-
-byte_levels = [
-    (1024 ** 5, "PB"), (1024 ** 4, "TB"), (1024 ** 3, "GB"),
-    (1024 ** 2, "MB"), (1024 ** 1, "KB"), (1024 ** 0, "B"),
-]
-def format_bytes(byte_count):
-    byte_count = int(byte_count)
-    if byte_count <= 0:
-        return "0 Bytes"
-    for factor, suffix in byte_levels:
-        if byte_count >= factor:
-            return f"1 {suffix}" if byte_count == factor else f"{byte_count / factor:.2f} {suffix}s"
-
-def copy_with_progress(src, dst, description=None):
-    size = os.path.getsize(src)
-    with open(src, "rb") as fsrc:
-        with open(dst, "wb") as fdst:
-            with tqdm(total=size, unit="B", unit_scale=True, desc=description) as pbar:
-                while True:
-                    chunk = fsrc.read(4096)
-                    if not chunk:
-                        break
-                    fdst.write(chunk)
-                    pbar.update(len(chunk))
-
-def in_the_last(file, days=0, seconds=0, microseconds=0, milliseconds=0, minutes=0, hours=0, weeks=0):
-    file_time = datetime.fromtimestamp(os.path.getctime(file))
-    now = datetime.now()
-    current = now - timedelta(days=days, seconds=seconds, microseconds=microseconds, milliseconds=milliseconds, minutes=minutes, hours=hours, weeks=weeks)
-    return current <= file_time <= now, str(now - file_time).split(".")[0]
+import glob, time, os, requests
+from datetime import datetime, timedelta
+from pathlib import Path
+from pathvalidate import is_valid_filename, sanitize_filename
+from tqdm import tqdm
+from .exceptions import Failed
+
+def update_send(old_send, timeout):
+    def new_send(*send_args, **kwargs):
+        if kwargs.get("timeout", None) is None:
+            kwargs["timeout"] = timeout
+        return old_send(*send_args, **kwargs)
+    return new_send
+
+def glob_filter(filter_in):
+    filter_in = filter_in.translate({ord("["): "[[]", ord("]"): "[]]"}) if "[" in filter_in else filter_in
+    return glob.glob(filter_in)
+
+def is_locked(filepath):
+    locked = None
+    file_object = None
+    if Path(filepath).exists():
+        try:
+            file_object = open(filepath, "a", 8)
+            if file_object:
+                locked = False
+        except IOError:
+            locked = True
+        finally:
+            if file_object:
+                file_object.close()
+    return locked
+
+def validate_filename(filename):
+    if not is_valid_filename(str(filename)):
+        filename = sanitize_filename(str(filename))
+    return filename
+
+def download_image(download_image_url, path, name="temp"):
+    image_response = requests.get(download_image_url)
+    if image_response.status_code >= 400:
+        raise Failed("Image Error: Image Download Failed")
+    if image_response.headers["Content-Type"] not in ["image/png", "image/jpeg", "image/webp"]:
+        raise Failed("Image Error: Image Not PNG, JPG, or WEBP")
+    if image_response.headers["Content-Type"] == "image/jpeg":
+        temp_image_name = f"{name}.jpg"
+    elif image_response.headers["Content-Type"] == "image/webp":
+        temp_image_name = f"{name}.webp"
+    else:
+        temp_image_name = f"{name}.png"
+    temp_image_name = Path(path) / temp_image_name
+    with temp_image_name.open(mode="wb") as handler:
+        handler.write(image_response.content)
+    while is_locked(temp_image_name):
+        time.sleep(1)
+    return temp_image_name
+
+def move_path(file_path, old_base, new_base, suffix=None, append=True):
+    final_path = Path(new_base) / file_path.removeprefix(old_base)[1:]
+    final_path.mkdir(parents=True, exist_ok=True)
+    final_file = Path(f"{final_path}{suffix}" if suffix and append else str(final_path).removesuffix(suffix) if suffix else final_path)
+    Path(file_path).rename(final_file)
+    return final_file
+
+byte_levels = [
+    (1024 ** 5, "PB"), (1024 ** 4, "TB"), (1024 ** 3, "GB"),
+    (1024 ** 2, "MB"), (1024 ** 1, "KB"), (1024 ** 0, "B"),
+]
+def format_bytes(byte_count):
+    byte_count = int(byte_count)
+    if byte_count <= 0:
+        return "0 Bytes"
+    for factor, suffix in byte_levels:
+        if byte_count >= factor:
+            return f"1 {suffix}" if byte_count == factor else f"{byte_count / factor:.2f} {suffix}s"
+
+def copy_with_progress(src, dst, description=None):
+    size = os.path.getsize(src)
+    with open(src, "rb") as fsrc:
+        with open(dst, "wb") as fdst:
+            with tqdm(total=size, unit="B", unit_scale=True, desc=description) as pbar:
+                while True:
+                    chunk = fsrc.read(4096)
+                    if not chunk:
+                        break
+                    fdst.write(chunk)
+                    pbar.update(len(chunk))
+
+def in_the_last(file, days=0, seconds=0, microseconds=0, milliseconds=0, minutes=0, hours=0, weeks=0):
+    file_time = datetime.fromtimestamp(os.path.getctime(file))
+    now = datetime.now()
+    current = now - timedelta(days=days, seconds=seconds, microseconds=microseconds, milliseconds=milliseconds, minutes=minutes, hours=hours, weeks=weeks)
+    return current <= file_time <= now, str(now - file_time).split(".")[0]
```

### Comparing `kometautils-0.1.0/kometautils/yaml.py` & `kometautils-0.2.0/kometautils/yaml.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,100 +1,100 @@
-import ruamel.yaml
-from pathlib import Path
-from .exceptions import Failed
-
-class YAML:
-    def __init__(self, path=None, input_data=None, check_empty=False, create=False, start_empty=False, preserve_quotes=False):
-        self.path = Path(path) if path else path
-        self.input_data = input_data
-        self.yaml = ruamel.yaml.YAML()
-        if preserve_quotes:
-            self.yaml.preserve_quotes = True
-        self.yaml.indent(mapping=2, sequence=2)
-        try:
-            if input_data:
-                self.data = self.yaml.load(input_data)
-            else:
-                if start_empty or (create and not self.path.exists()):
-                    self.path.unlink(missing_ok=True)
-                    self.path.touch()
-                    self.data = {}
-                else:
-                    with self.path.open(encoding="utf-8") as fp:
-                        self.data = self.yaml.load(fp)
-        except ruamel.yaml.error.YAMLError as e:
-            e = str(e).replace("\n", "\n      ")
-            raise Failed(f"YAML Error: {e}")
-        except Exception as e:
-            raise Failed(f"YAML Error: {e}")
-        if not self.data or not isinstance(self.data, dict):
-            if check_empty:
-                raise Failed("YAML Error: File is empty")
-            self.data = {}
-
-    def __getitem__(self, key):
-        if key in self.data:
-            return self.data[key]
-        raise KeyError(key)
-
-    def __setitem__(self, key, value):
-        self.data[key] = value
-
-    def __contains__(self, key):
-        return key in self.data
-
-    def __repr__(self):
-        return repr(self.data)
-
-    def __len__(self):
-        return len(self.data)
-
-    def __delitem__(self, key):
-        del self.data[key]
-
-    def clear(self):
-        return self.data.clear()
-
-    def copy(self):
-        return self.data.copy()
-
-    def has_key(self, k):
-        return k in self.data
-
-    def update(self, *args, **kwargs):
-        return self.data.update(*args, **kwargs)
-
-    def keys(self):
-        return self.data.keys()
-
-    def values(self):
-        return self.data.values()
-
-    def items(self):
-        return self.data.items()
-
-    def pop(self, *args):
-        return self.data.pop(*args)
-
-    def __iter__(self):
-        return iter(self.data)
-
-    def save(self):
-        if self.path:
-            with self.path.open(mode="w", encoding="utf-8") as fp:
-                self.yaml.dump(self.data, fp)
-
-    @staticmethod
-    def inline(data):
-        if isinstance(data, list):
-            output = ruamel.yaml.comments.CommentedSeq(data)
-        elif isinstance(data, dict):
-
-            output = ruamel.yaml.comments.CommentedMap(data)
-        else:
-            return data
-        output.fa.set_flow_style()
-        return output
-
-    @staticmethod
-    def quote(data):
-        return ruamel.yaml.scalarstring.DoubleQuotedScalarString(data)
+import ruamel.yaml
+from pathlib import Path
+from .exceptions import Failed
+
+class YAML:
+    def __init__(self, path=None, input_data=None, check_empty=False, create=False, start_empty=False, preserve_quotes=False):
+        self.path = Path(path) if path else path
+        self.input_data = input_data
+        self.yaml = ruamel.yaml.YAML()
+        if preserve_quotes:
+            self.yaml.preserve_quotes = True
+        self.yaml.indent(mapping=2, sequence=2)
+        try:
+            if input_data:
+                self.data = self.yaml.load(input_data)
+            else:
+                if start_empty or (create and not self.path.exists()):
+                    self.path.unlink(missing_ok=True)
+                    self.path.touch()
+                    self.data = {}
+                else:
+                    with self.path.open(encoding="utf-8") as fp:
+                        self.data = self.yaml.load(fp)
+        except ruamel.yaml.error.YAMLError as e:
+            e = str(e).replace("\n", "\n      ")
+            raise Failed(f"YAML Error: {e}")
+        except Exception as e:
+            raise Failed(f"YAML Error: {e}")
+        if not self.data or not isinstance(self.data, dict):
+            if check_empty:
+                raise Failed("YAML Error: File is empty")
+            self.data = {}
+
+    def __getitem__(self, key):
+        if key in self.data:
+            return self.data[key]
+        raise KeyError(key)
+
+    def __setitem__(self, key, value):
+        self.data[key] = value
+
+    def __contains__(self, key):
+        return key in self.data
+
+    def __repr__(self):
+        return repr(self.data)
+
+    def __len__(self):
+        return len(self.data)
+
+    def __delitem__(self, key):
+        del self.data[key]
+
+    def clear(self):
+        return self.data.clear()
+
+    def copy(self):
+        return self.data.copy()
+
+    def has_key(self, k):
+        return k in self.data
+
+    def update(self, *args, **kwargs):
+        return self.data.update(*args, **kwargs)
+
+    def keys(self):
+        return self.data.keys()
+
+    def values(self):
+        return self.data.values()
+
+    def items(self):
+        return self.data.items()
+
+    def pop(self, *args):
+        return self.data.pop(*args)
+
+    def __iter__(self):
+        return iter(self.data)
+
+    def save(self):
+        if self.path:
+            with self.path.open(mode="w", encoding="utf-8") as fp:
+                self.yaml.dump(self.data, fp)
+
+    @staticmethod
+    def inline(data):
+        if isinstance(data, list):
+            output = ruamel.yaml.comments.CommentedSeq(data)
+        elif isinstance(data, dict):
+
+            output = ruamel.yaml.comments.CommentedMap(data)
+        else:
+            return data
+        output.fa.set_flow_style()
+        return output
+
+    @staticmethod
+    def quote(data):
+        return ruamel.yaml.scalarstring.DoubleQuotedScalarString(data)
```

### Comparing `kometautils-0.1.0/setup.py` & `kometautils-0.2.0/setup.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,47 +1,47 @@
-import kometautils, os
-
-from setuptools import setup, find_packages
-
-with open("README.rst", "r") as f:
-    long_descr = f.read()
-
-__version__ = None
-if os.path.exists("VERSION"):
-    with open("VERSION") as handle:
-        for line in handle.readlines():
-            line = line.strip()
-            if len(line) > 0:
-                __version__ = line
-                break
-
-with open("requirements.txt", "r") as handle:
-    requirements = [i.strip() for i in handle.readlines()]
-
-setup(
-    name=kometautils.__package_name__,
-    version=__version__,
-    description=kometautils.__description__,
-    long_description=long_descr,
-    url=kometautils.__url__,
-    author=kometautils.__author__,
-    author_email=kometautils.__email__,
-    license=kometautils.__license__,
-    packages=find_packages(),
-    python_requires=">=3.11",
-    keywords=["kometautils"],
-    install_requires=requirements,
-    project_urls={
-        "Documentation": "https://github.com/Kometa-Team/Kometa-Utils",
-        "Funding": "https://github.com/sponsors/meisnate12",
-        "Source": "https://github.com/Kometa-Team/Kometa-Utils",
-        "Issues": "https://github.com/Kometa-Team/Kometa-Utils/issues",
-    },
-    classifiers=[
-        "Development Status :: 5 - Production/Stable",
-        "Intended Audience :: Developers",
-        "Topic :: Software Development :: Libraries",
-        "Programming Language :: Python",
-        "Programming Language :: Python :: 3.11",
-        "Programming Language :: Python :: 3.12",
-    ]
-)
+import kometautils, os
+
+from setuptools import setup, find_packages
+
+with open("README.rst", "r") as f:
+    long_descr = f.read()
+
+__version__ = None
+if os.path.exists("VERSION"):
+    with open("VERSION") as handle:
+        for line in handle.readlines():
+            line = line.strip()
+            if len(line) > 0:
+                __version__ = line
+                break
+
+with open("requirements.txt", "r") as handle:
+    requirements = [i.strip() for i in handle.readlines()]
+
+setup(
+    name=kometautils.__package_name__,
+    version=__version__,
+    description=kometautils.__description__,
+    long_description=long_descr,
+    url=kometautils.__url__,
+    author=kometautils.__author__,
+    author_email=kometautils.__email__,
+    license=kometautils.__license__,
+    packages=find_packages(),
+    python_requires=">=3.11",
+    keywords=["kometautils"],
+    install_requires=requirements,
+    project_urls={
+        "Documentation": "https://github.com/Kometa-Team/Kometa-Utils",
+        "Funding": "https://github.com/sponsors/meisnate12",
+        "Source": "https://github.com/Kometa-Team/Kometa-Utils",
+        "Issues": "https://github.com/Kometa-Team/Kometa-Utils/issues",
+    },
+    classifiers=[
+        "Development Status :: 5 - Production/Stable",
+        "Intended Audience :: Developers",
+        "Topic :: Software Development :: Libraries",
+        "Programming Language :: Python",
+        "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
+    ]
+)
```

