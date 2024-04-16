# Comparing `tmp/isaacgym_stubs-1.0rc3.tar.gz` & `tmp/isaacgym-stubs-1.0rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "isaacgym_stubs-1.0rc3.tar", last modified: Tue Apr 16 02:28:17 2024, max compression
+gzip compressed data, was "isaacgym-stubs-1.0rc4.tar", last modified: Sat Feb 25 07:19:29 2023, max compression
```

## Comparing `isaacgym_stubs-1.0rc3.tar` & `isaacgym-stubs-1.0rc4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 yuzhe     (1000) yuzhe     (1000)        0 2024-04-16 02:28:17.578509 isaacgym_stubs-1.0rc3/
--rw-rw-r--   0 yuzhe     (1000) yuzhe     (1000)     1067 2023-02-25 07:12:02.000000 isaacgym_stubs-1.0rc3/LICENSE
--rw-r--r--   0 yuzhe     (1000) yuzhe     (1000)     2805 2024-04-16 02:28:17.578509 isaacgym_stubs-1.0rc3/PKG-INFO
--rw-rw-r--   0 yuzhe     (1000) yuzhe     (1000)     2340 2023-10-15 02:33:00.000000 isaacgym_stubs-1.0rc3/README.md
-drwxrwxr-x   0 yuzhe     (1000) yuzhe     (1000)        0 2024-04-16 02:28:17.578509 isaacgym_stubs-1.0rc3/isaacgym-stubs/
--rw-rw-r--   0 yuzhe     (1000) yuzhe     (1000)       22 2023-02-24 05:20:42.000000 isaacgym_stubs-1.0rc3/isaacgym-stubs/__init__.py
--rw-rw-r--   0 yuzhe     (1000) yuzhe     (1000)    68178 2024-04-16 02:25:14.000000 isaacgym_stubs-1.0rc3/isaacgym-stubs/gymapi.pyi
-drwxrwxr-x   0 yuzhe     (1000) yuzhe     (1000)        0 2024-04-16 02:28:17.578509 isaacgym_stubs-1.0rc3/isaacgym_stubs.egg-info/
--rw-r--r--   0 yuzhe     (1000) yuzhe     (1000)     2805 2024-04-16 02:28:17.000000 isaacgym_stubs-1.0rc3/isaacgym_stubs.egg-info/PKG-INFO
--rw-rw-r--   0 yuzhe     (1000) yuzhe     (1000)      246 2024-04-16 02:28:17.000000 isaacgym_stubs-1.0rc3/isaacgym_stubs.egg-info/SOURCES.txt
--rw-rw-r--   0 yuzhe     (1000) yuzhe     (1000)        1 2024-04-16 02:28:17.000000 isaacgym_stubs-1.0rc3/isaacgym_stubs.egg-info/dependency_links.txt
--rw-rw-r--   0 yuzhe     (1000) yuzhe     (1000)       15 2024-04-16 02:28:17.000000 isaacgym_stubs-1.0rc3/isaacgym_stubs.egg-info/top_level.txt
--rw-rw-r--   0 yuzhe     (1000) yuzhe     (1000)      489 2024-04-16 02:25:23.000000 isaacgym_stubs-1.0rc3/pyproject.toml
--rw-rw-r--   0 yuzhe     (1000) yuzhe     (1000)       38 2024-04-16 02:28:17.578509 isaacgym_stubs-1.0rc3/setup.cfg
--rw-rw-r--   0 yuzhe     (1000) yuzhe     (1000)      307 2024-04-16 02:25:23.000000 isaacgym_stubs-1.0rc3/setup.py
+drwxrwxr-x   0 yuzhe     (1000) yuzhe     (1000)        0 2023-02-25 07:19:29.789794 isaacgym-stubs-1.0rc4/
+-rw-rw-r--   0 yuzhe     (1000) yuzhe     (1000)     1067 2023-02-25 07:12:02.000000 isaacgym-stubs-1.0rc4/LICENSE
+-rw-rw-r--   0 yuzhe     (1000) yuzhe     (1000)     1648 2023-02-25 07:19:29.789794 isaacgym-stubs-1.0rc4/PKG-INFO
+-rw-rw-r--   0 yuzhe     (1000) yuzhe     (1000)     1183 2023-02-25 07:13:13.000000 isaacgym-stubs-1.0rc4/README.md
+drwxrwxr-x   0 yuzhe     (1000) yuzhe     (1000)        0 2023-02-25 07:19:29.789794 isaacgym-stubs-1.0rc4/isaacgym-stubs/
+-rw-rw-r--   0 yuzhe     (1000) yuzhe     (1000)       22 2023-02-24 05:20:42.000000 isaacgym-stubs-1.0rc4/isaacgym-stubs/__init__.py
+-rw-rw-r--   0 yuzhe     (1000) yuzhe     (1000)    68303 2023-02-24 05:02:26.000000 isaacgym-stubs-1.0rc4/isaacgym-stubs/gymapi.pyi
+drwxrwxr-x   0 yuzhe     (1000) yuzhe     (1000)        0 2023-02-25 07:19:29.789794 isaacgym-stubs-1.0rc4/isaacgym_stubs.egg-info/
+-rw-rw-r--   0 yuzhe     (1000) yuzhe     (1000)     1648 2023-02-25 07:19:29.000000 isaacgym-stubs-1.0rc4/isaacgym_stubs.egg-info/PKG-INFO
+-rw-rw-r--   0 yuzhe     (1000) yuzhe     (1000)      246 2023-02-25 07:19:29.000000 isaacgym-stubs-1.0rc4/isaacgym_stubs.egg-info/SOURCES.txt
+-rw-rw-r--   0 yuzhe     (1000) yuzhe     (1000)        1 2023-02-25 07:19:29.000000 isaacgym-stubs-1.0rc4/isaacgym_stubs.egg-info/dependency_links.txt
+-rw-rw-r--   0 yuzhe     (1000) yuzhe     (1000)       15 2023-02-25 07:19:29.000000 isaacgym-stubs-1.0rc4/isaacgym_stubs.egg-info/top_level.txt
+-rw-rw-r--   0 yuzhe     (1000) yuzhe     (1000)      489 2023-02-25 07:19:26.000000 isaacgym-stubs-1.0rc4/pyproject.toml
+-rw-rw-r--   0 yuzhe     (1000) yuzhe     (1000)       38 2023-02-25 07:19:29.789794 isaacgym-stubs-1.0rc4/setup.cfg
+-rw-rw-r--   0 yuzhe     (1000) yuzhe     (1000)      307 2023-02-25 06:26:03.000000 isaacgym-stubs-1.0rc4/setup.py
```

### Comparing `isaacgym_stubs-1.0rc3/LICENSE` & `isaacgym-stubs-1.0rc4/LICENSE`

 * *Files identical despite different names*

### Comparing `isaacgym_stubs-1.0rc3/README.md` & `isaacgym-stubs-1.0rc4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,57 +1,47 @@
-Isaac Gym Python Stubs for Code Completion
+Metadata-Version: 2.1
+Name: isaacgym-stubs
+Version: 1.0rc4
+Summary: Isaac Gym Python Stubs for Code Completion
+Author: Yuzhe Qin
+Author-email: Yuzhe Qin <y1qin@ucsd.edu>
+Project-URL: Homepage, https://github.com/yzqin/isaacgym-stubs
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
 
-[![PyPI version](https://badge.fury.io/py/isaacgym-stubs.svg)](https://badge.fury.io/py/isaacgym-stubs)
+Isaac Gym Python Stubs for Code Completion
 ==========================================
 
-Enable code completion for IsaacGym simply with `pip install isaacgym-stubs`, even without IsaacGym itself!
+Code completion for IsaacGym with one line `pip install`, even without IsaacGym itself.
 
 ```bash
-# Install from PyPi
-pip3 install isaacgym-stubs
-
-# Alternatively, install from Github
-# pip3 install git+https://github.com/yzqin/isaacgym-stubs.git
+pip3 install git+https://github.com/yzqin/isaacgym-stubs.git
 ```
 
-Begin your code with the typical `from isaacgym import gymapi` and enjoy auto-completion.
+Depending on which IDE you are using, sometimes you may need to restart the IDE after `pip install` for re-indexing.
 
-The magic of `stub` is that you even **do not need to pip install IsaacGym itself**.
-
-For example, you may want to run IsaacGym on server but develop the code on a MacBook.
-IsaacGym may not support Mac. But you can still install this repo on MacBook and get smooth code completion during
-development!
+The magic of `stub` is that you even **do not need to pip install IsaacGym itself** to write the code.
+For example, you may need to run IsaacGym on server for training but develop the code on your MacBook.
+IsaacGym does not support Mac. But you can still install this repo and get smooth code completion to write IsaacGym
+code on that MacBook!
 
 ### Demo
 
 **VsCode**
 
 ![VsCode Demo](files/vscode.gif)
 
 **PyCharm**
 
 ![PyCharm Demo](files/pycharm.gif)
 
-### Troubleshooting
-
-1. The Python interpreter specified in your IDE should be the Python where isaacgym-stubs is installed. For
-   example, if you install this repository with conda Python but select the system Python as the interpreter in your
-   IDE, you won't have any code auto-completion. Follow the official instruction
-   [here](https://code.visualstudio.com/docs/python/environments) for VSCode
-   and [here](https://www.jetbrains.com/help/pycharm/configuring-python-interpreter.html) for PyCharm.
-2. Code auto-completion will not function if there's a directory named `issacgym` in your workspace. In this
-   case, the isaacgym symbol in your import will point to the directory instead of this package, disrupting the
-   auto-completion. Ensure that there's no `isaacgym` directory in your IDE workspace.
-3. Depending on which IDE you are using, sometimes you may need to restart the IDE after `pip install` for re-indexing.
-
 ### Overview
 
 This repository contains the `pyi` stub for the IsaacGym library, which can be used for code completion and type
 checking.
 According to the guidelines outlined in [PEP-561](https://peps.python.org/pep-0561/), Python stub files contain only
 type information and no runtime code.
 The `stub` in this repo is generated based on IsaacGym version `1.0rc4`.
-
-### How to Generate This `pyi`
-
-See [here](./STUB.md) for more explanation.
-
```

### Comparing `isaacgym_stubs-1.0rc3/isaacgym-stubs/gymapi.pyi` & `isaacgym-stubs-1.0rc4/isaacgym-stubs/gymapi.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -175,14 +175,15 @@
 MOUSE_RIGHT_BUTTON: MouseInput
 MOUSE_SCROLL_DOWN: MouseInput
 MOUSE_SCROLL_LEFT: MouseInput
 MOUSE_SCROLL_RIGHT: MouseInput
 MOUSE_SCROLL_UP: MouseInput
 RIGID_BODY_DISABLE_GRAVITY: int
 RIGID_BODY_DISABLE_SIMULATION: int
+RIGID_BODY_ENABLE_GYROSCOPIC_FORCES: int
 RIGID_BODY_NONE: int
 SIM_FLEX: SimType
 SIM_PHYSX: SimType
 STATE_ALL: int
 STATE_NONE: int
 STATE_POS: int
 STATE_VEL: int
@@ -230,14 +231,15 @@
     angular_damping: float
     armature: float
     collapse_fixed_joints: bool
     convex_decomposition_from_submeshes: bool
     default_dof_drive_mode: int
     density: float
     disable_gravity: bool
+    enable_gyroscopic_forces: bool
     fix_base_link: bool
     flip_visual_attachments: bool
     linear_damping: float
     max_angular_velocity: float
     max_linear_velocity: float
     mesh_normal_mode: MeshNormalMode
     min_particle_mass: float
@@ -1843,16 +1845,18 @@
 
     @property
     def torsion_friction(self) -> float: ...
 
 
 class RigidShapeProperties:
     compliance: float
+    contact_offset: float
     filter: int
     friction: float
+    rest_offset: float
     restitution: float
     rolling_friction: float
     thickness: float
     torsion_friction: float
 
     def __init__(self) -> None: ...
 
@@ -2362,15 +2366,15 @@
     def __init__(self) -> None: ...
 
 
 class Viewer:
     def __init__(self, *args, **kwargs) -> None: ...
 
 
-def acquire_gym(*args, **kwargs) -> Any: ...
+def acquire_gym(*args, **kwargs) -> Gym: ...
 
 
 def carb_init(config_str: str = ...) -> bool: ...
 
 
 def cross(*args, **kwargs) -> Any: ...
```

