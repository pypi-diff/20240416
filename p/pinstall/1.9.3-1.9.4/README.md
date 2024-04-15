# Comparing `tmp/pinstall-1.9.3.tar.gz` & `tmp/pinstall-1.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pinstall-1.9.3.tar", last modified: Sat Jan 13 03:07:51 2024, max compression
+gzip compressed data, was "pinstall-1.9.4.tar", last modified: Sat Jan 13 03:42:22 2024, max compression
```

## Comparing `pinstall-1.9.3.tar` & `pinstall-1.9.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2024-01-13 03:07:51.737857 pinstall-1.9.3/
--rw-r--r--   0 mark      (1000) mark      (1000)       74 2023-09-17 09:50:08.000000 pinstall-1.9.3/.flake8
--rw-r--r--   0 mark      (1000) mark      (1000)       72 2023-09-17 09:50:08.000000 pinstall-1.9.3/.gitignore
--rw-r--r--   0 mark      (1000) mark      (1000)      419 2024-01-12 06:45:26.000000 pinstall-1.9.3/Makefile
--rw-r--r--   0 mark      (1000) mark      (1000)    10664 2024-01-13 03:07:51.737857 pinstall-1.9.3/PKG-INFO
--rw-r--r--   0 mark      (1000) mark      (1000)    10172 2024-01-13 00:44:33.000000 pinstall-1.9.3/README.md
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2024-01-13 03:07:51.734523 pinstall-1.9.3/pinstall/
--rw-r--r--   0 mark      (1000) mark      (1000)        0 2023-09-17 09:50:08.000000 pinstall-1.9.3/pinstall/__init__.py
--rw-r--r--   0 mark      (1000) mark      (1000)       97 2023-09-17 09:50:08.000000 pinstall-1.9.3/pinstall/__main__.py
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2024-01-13 03:07:51.737857 pinstall-1.9.3/pinstall/commands/
--rw-r--r--   0 mark      (1000) mark      (1000)     4274 2024-01-12 08:33:51.000000 pinstall-1.9.3/pinstall/commands/project.py
--rw-r--r--   0 mark      (1000) mark      (1000)     3955 2024-01-13 02:45:41.000000 pinstall-1.9.3/pinstall/commands/pyenv.py
--rw-r--r--   0 mark      (1000) mark      (1000)     6301 2024-01-12 08:34:43.000000 pinstall-1.9.3/pinstall/commands/service.py
--rw-r--r--   0 mark      (1000) mark      (1000)     1417 2024-01-12 08:34:49.000000 pinstall-1.9.3/pinstall/commands/status.py
--rw-r--r--   0 mark      (1000) mark      (1000)     5697 2024-01-12 08:34:55.000000 pinstall-1.9.3/pinstall/commands/venv.py
--rw-r--r--   0 mark      (1000) mark      (1000)     1452 2024-01-13 00:03:55.000000 pinstall-1.9.3/pinstall/pinstall.py
--rw-r--r--   0 mark      (1000) mark      (1000)      835 2024-01-12 06:23:18.000000 pinstall-1.9.3/pinstall/run.py
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2024-01-13 03:07:51.737857 pinstall-1.9.3/pinstall.egg-info/
--rw-r--r--   0 mark      (1000) mark      (1000)    10664 2024-01-13 03:07:51.000000 pinstall-1.9.3/pinstall.egg-info/PKG-INFO
--rw-r--r--   0 mark      (1000) mark      (1000)      464 2024-01-13 03:07:51.000000 pinstall-1.9.3/pinstall.egg-info/SOURCES.txt
--rw-r--r--   0 mark      (1000) mark      (1000)        1 2024-01-13 03:07:51.000000 pinstall-1.9.3/pinstall.egg-info/dependency_links.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       52 2024-01-13 03:07:51.000000 pinstall-1.9.3/pinstall.egg-info/entry_points.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       51 2024-01-13 03:07:51.000000 pinstall-1.9.3/pinstall.egg-info/requires.txt
--rw-r--r--   0 mark      (1000) mark      (1000)        9 2024-01-13 03:07:51.000000 pinstall-1.9.3/pinstall.egg-info/top_level.txt
--rw-r--r--   0 mark      (1000) mark      (1000)     1032 2024-01-13 00:32:22.000000 pinstall-1.9.3/pyproject.toml
--rw-r--r--   0 mark      (1000) mark      (1000)       38 2024-01-13 03:07:51.737857 pinstall-1.9.3/setup.cfg
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2024-01-13 03:42:22.294103 pinstall-1.9.4/
+-rw-r--r--   0 mark      (1000) mark      (1000)       74 2023-09-17 09:50:08.000000 pinstall-1.9.4/.flake8
+-rw-r--r--   0 mark      (1000) mark      (1000)       72 2023-09-17 09:50:08.000000 pinstall-1.9.4/.gitignore
+-rw-r--r--   0 mark      (1000) mark      (1000)      419 2024-01-12 06:45:26.000000 pinstall-1.9.4/Makefile
+-rw-r--r--   0 mark      (1000) mark      (1000)    10649 2024-01-13 03:42:22.294103 pinstall-1.9.4/PKG-INFO
+-rw-r--r--   0 mark      (1000) mark      (1000)    10157 2024-01-13 03:39:32.000000 pinstall-1.9.4/README.md
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2024-01-13 03:42:22.290770 pinstall-1.9.4/pinstall/
+-rw-r--r--   0 mark      (1000) mark      (1000)        0 2023-09-17 09:50:08.000000 pinstall-1.9.4/pinstall/__init__.py
+-rw-r--r--   0 mark      (1000) mark      (1000)       97 2023-09-17 09:50:08.000000 pinstall-1.9.4/pinstall/__main__.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2024-01-13 03:42:22.294103 pinstall-1.9.4/pinstall/commands/
+-rw-r--r--   0 mark      (1000) mark      (1000)     4274 2024-01-12 08:33:51.000000 pinstall-1.9.4/pinstall/commands/project.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     3969 2024-01-13 03:27:22.000000 pinstall-1.9.4/pinstall/commands/pyenv.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     6301 2024-01-12 08:34:43.000000 pinstall-1.9.4/pinstall/commands/service.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     1417 2024-01-12 08:34:49.000000 pinstall-1.9.4/pinstall/commands/status.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     5838 2024-01-13 03:36:42.000000 pinstall-1.9.4/pinstall/commands/venv.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     1452 2024-01-13 00:03:55.000000 pinstall-1.9.4/pinstall/pinstall.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      835 2024-01-12 06:23:18.000000 pinstall-1.9.4/pinstall/run.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2024-01-13 03:42:22.294103 pinstall-1.9.4/pinstall.egg-info/
+-rw-r--r--   0 mark      (1000) mark      (1000)    10649 2024-01-13 03:42:22.000000 pinstall-1.9.4/pinstall.egg-info/PKG-INFO
+-rw-r--r--   0 mark      (1000) mark      (1000)      464 2024-01-13 03:42:22.000000 pinstall-1.9.4/pinstall.egg-info/SOURCES.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)        1 2024-01-13 03:42:22.000000 pinstall-1.9.4/pinstall.egg-info/dependency_links.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       52 2024-01-13 03:42:22.000000 pinstall-1.9.4/pinstall.egg-info/entry_points.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       51 2024-01-13 03:42:22.000000 pinstall-1.9.4/pinstall.egg-info/requires.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)        9 2024-01-13 03:42:22.000000 pinstall-1.9.4/pinstall.egg-info/top_level.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)     1032 2024-01-13 00:32:22.000000 pinstall-1.9.4/pyproject.toml
+-rw-r--r--   0 mark      (1000) mark      (1000)       38 2024-01-13 03:42:22.294103 pinstall-1.9.4/setup.cfg
```

### Comparing `pinstall-1.9.3/PKG-INFO` & `pinstall-1.9.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pinstall
-Version: 1.9.3
+Version: 1.9.4
 Summary: Installer Tool for Python Programs
 Author-email: Mark Blakeney <mark.blakeney@bullet-systems.net>
 License: GPLv3
 Project-URL: Homepage, https://github.com/bulletmark/pinstall
 Keywords: venv,virtualenv,systemd,service,pip,pipx,pyproject.toml
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
@@ -201,15 +201,14 @@
 older or newer version than your system Python.
 
 E.g. Install Python 3.7 and then create a virtual enviroment (in the
 current directory) using it:
 
 ```sh
 $ pyenv install 3.7
-$ pinstall pyenv
 $ pinstall venv -P 3.7
 $ venv/bin/python --version
 Python 3.7.17
 ```
 
 Note in this example that [pyenv](https://github.com/pyenv/pyenv)
 installed Python 3.7.17 because that was the latest 3.7 version
@@ -227,29 +226,29 @@
 `pinstall pyenv -p` to automatically purge any older/superceded
 versions, i.e. to remove 3.7.3 in this example.
 
 `pinstall pyenv` also does something else each time you run it. It
 creates or updates major version links. E.g. after installing 3.7.4 as
 in the above example, `pinstall pyenv` will also create a link in your
 `pyenv` versions directory `3.7 -> 3.7.4`. This allows you to create a
-virtual environment in two ways:
+virtual environment in either of two ways:
 
 1. `pinstall venv -P 3.7.4` will create a virtual environment using
    3.7.4 permanently, or:
 
 2. `pinstall venv -P 3.7` will create a virtual environment using the
    link 3.7 which initially points to 3.7.4 but will automatically use
    3.7.5 when/if the minor version gets updated (i.e. after you have
-   done a later `pinstall pyenv` to find and install a new 3.7.5).
+   done a later `pinstall pyenv` to find and install a new 3.7.5). Note
+   that python minor version updates are always backwards compatible.
 
-Note if you don't use `pinstall pyenv` to update your `pyenv` versions
-and always only manage them via `pyenv` directly then `pinstall venv -P
-3.7` will still work but in this case `pyenv` simply dereferences 3.7 to
-3.7.4 immediately to create the virtual enviroment, i.e. the same as if
-you typed `pinstall venv -P 3.7.4` explicitly.
+Note that whenever you run `pinstall venv` and specify a `-P/--pyenv`
+version then pinstall will always first silently update the pyenv links
+implicitly to ensure the latest major version links are correct before
+creating your new virtual environment.
 
 ## Installation
 
 Arch Linux users can install [pinstall from the
 AUR](https://aur.archlinux.org/packages/pinstall).
 
 Python 3.6 or later is required and the [`sudo`](https://www.sudo.ws/)
```

### Comparing `pinstall-1.9.3/README.md` & `pinstall-1.9.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -187,15 +187,14 @@
 older or newer version than your system Python.
 
 E.g. Install Python 3.7 and then create a virtual enviroment (in the
 current directory) using it:
 
 ```sh
 $ pyenv install 3.7
-$ pinstall pyenv
 $ pinstall venv -P 3.7
 $ venv/bin/python --version
 Python 3.7.17
 ```
 
 Note in this example that [pyenv](https://github.com/pyenv/pyenv)
 installed Python 3.7.17 because that was the latest 3.7 version
@@ -213,29 +212,29 @@
 `pinstall pyenv -p` to automatically purge any older/superceded
 versions, i.e. to remove 3.7.3 in this example.
 
 `pinstall pyenv` also does something else each time you run it. It
 creates or updates major version links. E.g. after installing 3.7.4 as
 in the above example, `pinstall pyenv` will also create a link in your
 `pyenv` versions directory `3.7 -> 3.7.4`. This allows you to create a
-virtual environment in two ways:
+virtual environment in either of two ways:
 
 1. `pinstall venv -P 3.7.4` will create a virtual environment using
    3.7.4 permanently, or:
 
 2. `pinstall venv -P 3.7` will create a virtual environment using the
    link 3.7 which initially points to 3.7.4 but will automatically use
    3.7.5 when/if the minor version gets updated (i.e. after you have
-   done a later `pinstall pyenv` to find and install a new 3.7.5).
+   done a later `pinstall pyenv` to find and install a new 3.7.5). Note
+   that python minor version updates are always backwards compatible.
 
-Note if you don't use `pinstall pyenv` to update your `pyenv` versions
-and always only manage them via `pyenv` directly then `pinstall venv -P
-3.7` will still work but in this case `pyenv` simply dereferences 3.7 to
-3.7.4 immediately to create the virtual enviroment, i.e. the same as if
-you typed `pinstall venv -P 3.7.4` explicitly.
+Note that whenever you run `pinstall venv` and specify a `-P/--pyenv`
+version then pinstall will always first silently update the pyenv links
+implicitly to ensure the latest major version links are correct before
+creating your new virtual environment.
 
 ## Installation
 
 Arch Linux users can install [pinstall from the
 AUR](https://aur.archlinux.org/packages/pinstall).
 
 Python 3.6 or later is required and the [`sudo`](https://www.sudo.ws/)
```

### Comparing `pinstall-1.9.3/pinstall/commands/project.py` & `pinstall-1.9.4/pinstall/commands/project.py`

 * *Files identical despite different names*

### Comparing `pinstall-1.9.3/pinstall/commands/pyenv.py` & `pinstall-1.9.4/pinstall/commands/pyenv.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 from packaging import version
 
 from ..run import run
 
 valids = set(string.digits + '.')
 
-def update_symlinks(args: Namespace) -> None:
+def update_symlinks(remove_symlinks: bool = False) -> None:
     'Update all symlinks in pyenv versions dir'
     basestr = run('pyenv root', capture=True)
     if not basestr:
         return None
 
     base = Path(basestr.strip()) / 'versions'
     if not base.exists():
@@ -25,22 +25,22 @@
 
     # Record of all the existing symlinks and version dirs
     oldlinks = {}
     vers = []
     for path in base.iterdir():
         if all(c in valids for c in path.name):
             if path.is_symlink():
-                if args.remove_major_symlinks:
+                if remove_symlinks:
                     path.unlink()
                 else:
                     oldlinks[path.name] = os.readlink(str(path))
             else:
                 vers.append(path)
 
-    if args.remove_major_symlinks:
+    if remove_symlinks:
         return None
 
     # Create a map of all the new major version links
     newlinks_all = defaultdict(list)
     for path in vers:
         namevers = path.name
         while '.' in namevers[:-1]:
@@ -108,9 +108,9 @@
                 run(f'pyenv uninstall -f {overs}')
         elif latest:
             for uvers in updates:
                 print(f'### {uvers}: updating ...')
                 run(f'pyenv install -s {latest}')
 
     # Ensure we always update all the major version symlinks
-    update_symlinks(args)
+    update_symlinks(args.remove_major_symlinks)
     return None
```

### Comparing `pinstall-1.9.3/pinstall/commands/service.py` & `pinstall-1.9.4/pinstall/commands/service.py`

 * *Files identical despite different names*

### Comparing `pinstall-1.9.3/pinstall/commands/status.py` & `pinstall-1.9.4/pinstall/commands/status.py`

 * *Files identical despite different names*

### Comparing `pinstall-1.9.3/pinstall/commands/venv.py` & `pinstall-1.9.4/pinstall/commands/venv.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 '''
 import shutil
 import sys
 import tempfile
 from argparse import ArgumentParser, Namespace
 from pathlib import Path
 from typing import Any, Optional
+from . import pyenv
 
 from ..run import run
 
 DEFDIR = 'venv'
 DEFEXE = 'python3'
 DEFREQ = 'requirements.txt'
 PYPROJ = 'pyproject.toml'
@@ -80,14 +81,18 @@
 def main(args: Namespace) -> Optional[str]:
     'Called to action this command'
     if args.pyenv:
         pyenv_root = run('pyenv root', capture=True)
         if not pyenv_root:
             return 'Error: Can not find pyenv. Is it installed?'
 
+        # Since we are about to use pyenv, make sure the links are up to
+        # date
+        pyenv.update_symlinks()
+
         pyenv_version = run(f'pyenv latest {args.pyenv}', capture=True,
                             ignore_error=True)
         if not pyenv_version:
             return f'Error: no pyenv version {args.pyenv} installed.'
 
         pyexe_path = Path(pyenv_root, 'versions', pyenv_version,
                           'bin', 'python')
```

### Comparing `pinstall-1.9.3/pinstall/pinstall.py` & `pinstall-1.9.4/pinstall/pinstall.py`

 * *Files identical despite different names*

### Comparing `pinstall-1.9.3/pinstall/run.py` & `pinstall-1.9.4/pinstall/run.py`

 * *Files identical despite different names*

### Comparing `pinstall-1.9.3/pinstall.egg-info/PKG-INFO` & `pinstall-1.9.4/pinstall.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pinstall
-Version: 1.9.3
+Version: 1.9.4
 Summary: Installer Tool for Python Programs
 Author-email: Mark Blakeney <mark.blakeney@bullet-systems.net>
 License: GPLv3
 Project-URL: Homepage, https://github.com/bulletmark/pinstall
 Keywords: venv,virtualenv,systemd,service,pip,pipx,pyproject.toml
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
@@ -201,15 +201,14 @@
 older or newer version than your system Python.
 
 E.g. Install Python 3.7 and then create a virtual enviroment (in the
 current directory) using it:
 
 ```sh
 $ pyenv install 3.7
-$ pinstall pyenv
 $ pinstall venv -P 3.7
 $ venv/bin/python --version
 Python 3.7.17
 ```
 
 Note in this example that [pyenv](https://github.com/pyenv/pyenv)
 installed Python 3.7.17 because that was the latest 3.7 version
@@ -227,29 +226,29 @@
 `pinstall pyenv -p` to automatically purge any older/superceded
 versions, i.e. to remove 3.7.3 in this example.
 
 `pinstall pyenv` also does something else each time you run it. It
 creates or updates major version links. E.g. after installing 3.7.4 as
 in the above example, `pinstall pyenv` will also create a link in your
 `pyenv` versions directory `3.7 -> 3.7.4`. This allows you to create a
-virtual environment in two ways:
+virtual environment in either of two ways:
 
 1. `pinstall venv -P 3.7.4` will create a virtual environment using
    3.7.4 permanently, or:
 
 2. `pinstall venv -P 3.7` will create a virtual environment using the
    link 3.7 which initially points to 3.7.4 but will automatically use
    3.7.5 when/if the minor version gets updated (i.e. after you have
-   done a later `pinstall pyenv` to find and install a new 3.7.5).
+   done a later `pinstall pyenv` to find and install a new 3.7.5). Note
+   that python minor version updates are always backwards compatible.
 
-Note if you don't use `pinstall pyenv` to update your `pyenv` versions
-and always only manage them via `pyenv` directly then `pinstall venv -P
-3.7` will still work but in this case `pyenv` simply dereferences 3.7 to
-3.7.4 immediately to create the virtual enviroment, i.e. the same as if
-you typed `pinstall venv -P 3.7.4` explicitly.
+Note that whenever you run `pinstall venv` and specify a `-P/--pyenv`
+version then pinstall will always first silently update the pyenv links
+implicitly to ensure the latest major version links are correct before
+creating your new virtual environment.
 
 ## Installation
 
 Arch Linux users can install [pinstall from the
 AUR](https://aur.archlinux.org/packages/pinstall).
 
 Python 3.6 or later is required and the [`sudo`](https://www.sudo.ws/)
```

### Comparing `pinstall-1.9.3/pyproject.toml` & `pinstall-1.9.4/pyproject.toml`

 * *Files identical despite different names*

