# Comparing `tmp/poetry_build_compact-1.1.0.tar.gz` & `tmp/poetry_build_compact-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poetry_build_compact-1.1.0.tar", max compression
+gzip compressed data, was "poetry_build_compact-1.2.0.tar", max compression
```

## Comparing `poetry_build_compact-1.1.0.tar` & `poetry_build_compact-1.2.0.tar`

### file list

```diff
@@ -1,5 +1,7 @@
--rw-r--r--   0        0        0      894 2024-01-31 09:56:38.242419 poetry_build_compact-1.1.0/README.md
--rw-r--r--   0        0        0        0 2024-01-31 09:56:38.242419 poetry_build_compact-1.1.0/poetry_build_compact/__init__.py
--rw-r--r--   0        0        0    14357 2024-01-31 09:56:38.242419 poetry_build_compact-1.1.0/poetry_build_compact/plugin.py
--rw-r--r--   0        0        0      557 2024-01-31 09:56:38.242419 poetry_build_compact-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     1662 1970-01-01 00:00:00.000000 poetry_build_compact-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-16 07:07:33.370023 poetry_build_compact-1.2.0/COPYING
+-rw-r--r--   0        0        0     7652 2024-04-16 07:07:33.374023 poetry_build_compact-1.2.0/COPYING.LESSER
+-rw-r--r--   0        0        0      894 2024-04-16 07:07:33.374023 poetry_build_compact-1.2.0/README.md
+-rw-r--r--   0        0        0        0 2024-04-16 07:07:33.374023 poetry_build_compact-1.2.0/poetry_build_compact/__init__.py
+-rw-r--r--   0        0        0    14684 2024-04-16 07:07:33.374023 poetry_build_compact-1.2.0/poetry_build_compact/plugin.py
+-rw-r--r--   0        0        0      557 2024-04-16 07:07:33.374023 poetry_build_compact-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1662 1970-01-01 00:00:00.000000 poetry_build_compact-1.2.0/PKG-INFO
```

### Comparing `poetry_build_compact-1.1.0/README.md` & `poetry_build_compact-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `poetry_build_compact-1.1.0/poetry_build_compact/plugin.py` & `poetry_build_compact-1.2.0/poetry_build_compact/plugin.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from hashlib import sha256
 from pathlib import Path
 from shutil import make_archive
 
 from cleo.helpers import option
 from poetry.console.commands.command import Command
 from poetry.console.commands.installer_command import InstallerCommand
+from poetry.console.commands.env_command import EnvCommand
 from poetry.core.packages.dependency import Dependency
 from poetry.core.packages.dependency_group import MAIN_GROUP
 from poetry.factory import Factory
 from poetry.plugins.application_plugin import ApplicationPlugin
 from tomlkit import inline_table
 from tomlkit.toml_document import TOMLDocument
 
@@ -23,15 +24,15 @@
 
 class BuildCompactPlugin(ApplicationPlugin):
     @property
     def commands(self) -> list[type[Command]]:
         return [BuildCompactCommand, ReplaceCommand]
 
 
-class BaseReplaceCommand(Command):
+class BaseReplaceCommand(EnvCommand):
     options = [
         option(
             "replace",
             description="Replace these packages dependencies by compiled ones.",
             flag=False,
             multiple=True,
         ),
@@ -45,14 +46,18 @@
             "suffix",
             description="Suffix of compiled packages.",
             flag=False,
             default="-compact",
         ),
     ]
 
+    def python_version(self) -> tuple[str, str]:
+        version_info = self.env.get_version_info()
+        return version_info[:2]
+
     def soft_replace(self) -> bool:
         self.line(
             f"<info>Ephemeral dependencies replace in {self.poetry.package.name}</>"
         )
 
         replaced = False
         dependencies_group = self.poetry.package.dependency_group(MAIN_GROUP)
@@ -67,15 +72,16 @@
         content: dict[str, t.Any] = self.poetry.file.read()
         poetry_content = content["tool"]["poetry"]
 
         if "dependencies" not in poetry_content:
             return None
         section = poetry_content["dependencies"]
 
-        python_constraint = f"~{sys.version_info.major}.{sys.version_info.minor}"
+        major, minor = self.python_version()
+        python_constraint = f"~{major}.{minor}"
         self.line(f"<info>Fix Python version to {python_constraint}</>")
         self.poetry.package.python_versions = python_constraint
         section["python"] = python_constraint
 
         self.line(f"<info>Replacing dependencies in {self.poetry.package.name}</>")
 
         dependencies_group = self.poetry.package.dependency_group(MAIN_GROUP)
@@ -198,15 +204,19 @@
 
             if self.installer.run() != 0:
                 return 1
 
             self.line("")
             self.poetry.file.write(poetry_content)
 
-            return self.call("install", f"--sync --all-extras --only={MAIN_GROUP}")
+            command = f"--all-extras --only={MAIN_GROUP}"
+            if self.poetry.config.get("virtualenvs.create"):
+                command = f"--sync {command}"
+
+            return self.call("install", command)
         return 0
 
     def install(self, lock: bool = False) -> bool:
         self.installer.set_locker(self.poetry.locker)
         self.installer.set_package(self.poetry.package)
         self.installer.verbose(self.io.is_verbose())
         self.installer.update(False)
@@ -255,15 +265,17 @@
 
         assert self.poetry.package.root_dir
         self.dist_dir = self.poetry.package.root_dir / "dist"
         self.tmp_dir = self.dist_dir / "tmp"
         self.meta_dir = self.tmp_dir / f"{self.compact_dist_name}-{version}.dist-info"
 
         self.records: list[str] = []
-        self.python_tag = f"py{sys.version_info.major}{sys.version_info.minor}"
+
+        major, minor = self.python_version()
+        self.python_tag = f"py{major}{minor}"
 
         self.clear()
 
     def build_wheel(self) -> Path:
         self.line("<info>Building compact wheel</>")
 
         self.meta_dir.mkdir(parents=True)
@@ -313,16 +325,18 @@
 """.encode()
 
         wheel_file = self.meta_dir / "WHEEL"
         wheel_file.write_bytes(content)
         self.records.append(record_line(self.tmp_dir, wheel_file, content))
 
     def metadata_file(self) -> None:
-        this_python = f"{sys.version_info.major}.{sys.version_info.minor}"
-        next_python = f"{sys.version_info.major}.{sys.version_info.minor + 1}"
+        major, minor = self.python_version()
+        this_python = f"{major}.{minor}"
+        next_python = f"{major}.{int(minor) + 1}"
+
         content = f"""\
 Metadata-Version: 2.1
 Name: {self.compact_name}
 Version: {self.poetry.package.version}
 Summary: {self.poetry.package.description}
 License: Proprietary
 Requires-Python: >={this_python},<{next_python}
@@ -340,15 +354,15 @@
             content += f"Maintainer-email: {self.poetry.package.maintainer_email}\n"
 
         dependencies = sorted(
             self.poetry.package.dependency_group(MAIN_GROUP).dependencies,
             key=lambda d: d.name,
         )
         for dependency in dependencies:
-            content += f"Requires-Dist: {dependency.base_pep_508_name}\n"
+            content += f"Requires-Dist: {dependency.to_pep_508()}\n"
 
         content_bytes = content.encode()
 
         metadata_file = self.meta_dir / "METADATA"
         metadata_file.write_bytes(content_bytes)
         self.records.append(record_line(self.tmp_dir, metadata_file, content_bytes))
```

### Comparing `poetry_build_compact-1.1.0/pyproject.toml` & `poetry_build_compact-1.2.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "poetry-build-compact"
-version = "1.1.0"
+version = "1.2.0"
 description = "Poetry plugin providing command to compile package into bytecode one"
 authors = ["ZiphyCare LLC <support@ziphycare.com>"]
 packages = [{include = "poetry_build_compact"}]
 license = "LGPL-3.0-only"
 readme = "README.md"
 
 [tool.poetry.dependencies]
```

### Comparing `poetry_build_compact-1.1.0/PKG-INFO` & `poetry_build_compact-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poetry-build-compact
-Version: 1.1.0
+Version: 1.2.0
 Summary: Poetry plugin providing command to compile package into bytecode one
 License: LGPL-3.0-only
 Author: ZiphyCare LLC
 Author-email: support@ziphycare.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: Python :: 3
```

