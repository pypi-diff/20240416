# Comparing `tmp/brom_drake-0.0.2.post2.tar.gz` & `tmp/brom_drake-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brom_drake-0.0.2.post2.tar", last modified: Thu Apr  4 20:39:57 2024, max compression
+gzip compressed data, was "brom_drake-0.1.0.tar", last modified: Tue Apr 16 17:25:27 2024, max compression
```

## Comparing `brom_drake-0.0.2.post2.tar` & `brom_drake-0.1.0.tar`

### file list

```diff
@@ -1,26 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:39:57.291056 brom_drake-0.0.2.post2/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-04 20:39:50.000000 brom_drake-0.0.2.post2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3864 2024-04-04 20:39:57.291056 brom_drake-0.0.2.post2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-04-04 20:39:50.000000 brom_drake-0.0.2.post2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 20:39:57.291056 brom_drake-0.0.2.post2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      933 2024-04-04 20:39:55.000000 brom_drake-0.0.2.post2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:39:57.287056 brom_drake-0.0.2.post2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:39:57.291056 brom_drake-0.0.2.post2/src/brom_drake/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:39:57.291056 brom_drake-0.0.2.post2/src/brom_drake/DiagramTarget/
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-04 20:39:50.000000 brom_drake-0.0.2.post2/src/brom_drake/DiagramTarget/DiagramTarget.py
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-04 20:39:50.000000 brom_drake-0.0.2.post2/src/brom_drake/DiagramTarget/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:39:57.291056 brom_drake-0.0.2.post2/src/brom_drake/DiagramWatcher/
--rw-r--r--   0 runner    (1001) docker     (127)    11919 2024-04-04 20:39:50.000000 brom_drake-0.0.2.post2/src/brom_drake/DiagramWatcher/DiagramWatcher.py
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-04 20:39:50.000000 brom_drake-0.0.2.post2/src/brom_drake/DiagramWatcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-04 20:39:50.000000 brom_drake-0.0.2.post2/src/brom_drake/DiagramWatcher/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-04 20:39:50.000000 brom_drake-0.0.2.post2/src/brom_drake/DiagramWatcher/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-04 20:39:50.000000 brom_drake-0.0.2.post2/src/brom_drake/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:39:57.291056 brom_drake-0.0.2.post2/src/brom_drake/all/
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-04 20:39:50.000000 brom_drake-0.0.2.post2/src/brom_drake/all/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-04-04 20:39:50.000000 brom_drake-0.0.2.post2/src/brom_drake/all/add_watcher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:39:57.291056 brom_drake-0.0.2.post2/src/brom_drake.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3864 2024-04-04 20:39:57.000000 brom_drake-0.0.2.post2/src/brom_drake.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-04 20:39:57.000000 brom_drake-0.0.2.post2/src/brom_drake.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 20:39:57.000000 brom_drake-0.0.2.post2/src/brom_drake.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-04 20:39:57.000000 brom_drake-0.0.2.post2/src/brom_drake.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-04 20:39:57.000000 brom_drake-0.0.2.post2/src/brom_drake.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:25:27.569141 brom_drake-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-16 17:25:25.000000 brom_drake-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4793 2024-04-16 17:25:27.569141 brom_drake-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4431 2024-04-16 17:25:25.000000 brom_drake-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 17:25:27.569141 brom_drake-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-16 17:25:26.000000 brom_drake-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:25:27.565142 brom_drake-0.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:25:27.565142 brom_drake-0.1.0/src/brom_drake/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:25:27.565142 brom_drake-0.1.0/src/brom_drake/DiagramTarget/
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-16 17:25:25.000000 brom_drake-0.1.0/src/brom_drake/DiagramTarget/DiagramTarget.py
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-16 17:25:25.000000 brom_drake-0.1.0/src/brom_drake/DiagramTarget/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:25:27.569141 brom_drake-0.1.0/src/brom_drake/DiagramWatcher/
+-rw-r--r--   0 runner    (1001) docker     (127)     9041 2024-04-16 17:25:25.000000 brom_drake-0.1.0/src/brom_drake/DiagramWatcher/DiagramWatcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-16 17:25:25.000000 brom_drake-0.1.0/src/brom_drake/DiagramWatcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-16 17:25:25.000000 brom_drake-0.1.0/src/brom_drake/DiagramWatcher/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-16 17:25:25.000000 brom_drake-0.1.0/src/brom_drake/DiagramWatcher/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:25:27.569141 brom_drake-0.1.0/src/brom_drake/PortWatcher/
+-rw-r--r--   0 runner    (1001) docker     (127)     6500 2024-04-16 17:25:25.000000 brom_drake-0.1.0/src/brom_drake/PortWatcher/PortWatcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-16 17:25:25.000000 brom_drake-0.1.0/src/brom_drake/PortWatcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-16 17:25:25.000000 brom_drake-0.1.0/src/brom_drake/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:25:27.569141 brom_drake-0.1.0/src/brom_drake/all/
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-16 17:25:25.000000 brom_drake-0.1.0/src/brom_drake/all/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7569 2024-04-16 17:25:25.000000 brom_drake-0.1.0/src/brom_drake/all/add_watcher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:25:27.565142 brom_drake-0.1.0/src/brom_drake.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4793 2024-04-16 17:25:27.000000 brom_drake-0.1.0/src/brom_drake.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-16 17:25:27.000000 brom_drake-0.1.0/src/brom_drake.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 17:25:27.000000 brom_drake-0.1.0/src/brom_drake.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-16 17:25:27.000000 brom_drake-0.1.0/src/brom_drake.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-16 17:25:27.000000 brom_drake-0.1.0/src/brom_drake.egg-info/top_level.txt
```

### Comparing `brom_drake-0.0.2.post2/LICENSE` & `brom_drake-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `brom_drake-0.0.2.post2/PKG-INFO` & `brom_drake-0.1.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,39 @@
-Metadata-Version: 2.1
-Name: brom_drake
-Version: 0.0.2.post2
-Summary: A set of convenient logging and testing tools for the Drake robotics toolbox.
-Author: Kwesi Rutledge
-Author-email: thesolitaryecrivain@gmail.com
-Keywords: drake,robotics,testing,logging
-Classifier: Programming Language :: Python :: 3
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-
 [![codecov](https://codecov.io/gh/kwesiRutledge/brom_drake-py/graph/badge.svg?token=0TI5PV2HUD)](https://codecov.io/gh/kwesiRutledge/brom_drake-py)
 
 # brom_drake-py
 Brom is a helper library for the [Drake](https://drake.mit.edu/) robotics simulation and verification library.
-Its goal is to simplify logging and robustness characterization
-of Drake simulations. 
+Its goal is to simplify common debugging and testing activities in Drake (for example, logging the outputs
+of systems in your block diagrams). 
+
+Some of Brom's features:
+
+Feature                    |  Code | Results
+:-------------------------:|:-------------------------:|:-------------------------:
+The Diagram Watcher (the `DiagramWatcher` will log + plot all output ports of your `Diagram` automatically) |`add_watcher_and_build()`| ![Creation of Brom Directory](./promo/BromWatcher0.gif)
+
+(More coming soon...)
+
+## Installation
+
+`brom_drake` is available on PyPI and installable with pip:
+
+```shell
+pip install brom-drake
+```
+
+### Developer install
+
+You can also install the package during local development by cloning
+the repository and running the following commands from inside it:
+
+```bash
+pip install -r requirements.txt
+pip install -e .
+```
 
 ## Use Cases
 
 Here are a few of the features available in `brom_drake` and how they work.
 
 ### Easily Log Your Diagram's Signals
 
@@ -36,15 +50,15 @@
 
 # Create a diagram builder
 builder = DiagramBuilder()
 
 # Add and connect your systems...
 
 # Add the watcher and build the diagram
-dw, diagram, diagram_context = add_watcher_and_build(builder)
+watcher, diagram, diagram_context = add_watcher_and_build(builder)
 
 # Set up simulation
 simulator = Simulator(diagram, diagram_context)
 simulator.set_target_realtime_rate(1.0)
 simulator.set_publish_every_time_step(False)
 
 # Run simulation
@@ -57,31 +71,28 @@
 What will happen whenever you use this function is that:
 - The `DiagramWatcher` will be created.
   - It will search through all systems that the `DiagramBuilder` has added.
   - For each system, the watcher will add a `VectorLogger` to each output port that is a `kVectorValued` port.
   - The `DiagramWatcher` will connect all loggers to all targeted ports (in the above case, we will target all available output ports).
 - After the simulation is run and the script completes, the watcher will save all data traces for each port in `.png` files. These plots will be in a new `.brom` directory.
 
-## Installation
-
-`brom_drake` is available on PyPI and installable with pip:
-
-```shell
-pip install brom-drake
-```
-
-### Developer install
-
-You can also install the package during local development by cloning
-the repository and running the following commands from inside it:
+### Watching Specific systems
 
-```bash
-pip install -r requirements.txt
-pip install -e .
+If you only want to watch a specific system, then you can do so by passing in information to the "targets" argument:
+```python
+watcher, _, _ = add_watcher_and_build(
+  builder,
+  targets=[
+    ("system_name", "port_name"),
+    "system_name2",
+  ],
+)
 ```
+The above code tells the watcher to watch the port named `port_name` on the system named `system_name`.
+(If you don't know your system's name in Drake, then you can usually find it by using the `get_name()` method.)
 
 ## FAQs
 
 ### Why the name Brom?
 
 [Brom the storyteller](https://inheritance.fandom.com/wiki/Brom) is a character from the
 [Inheritance](https://en.wikipedia.org/wiki/Eragon) series by Christopher Paolini.
@@ -105,8 +116,8 @@
   tutorial's diagram.
   - [x] Determine if we can use `DiagramTarget` objects to do everything (assuming that they are all valid). i.e., with the name and the port # can we do waht we want?
 - [ ] Add more examples
 - [x] Add Code coverage
 - [ ] Add support for abstract output ports?
 - [ ] Add more readme explanations of what is going on under the hood.
 - [ ] Add support for giving `DiagramTarget` (or simpler objects) to the convenience functions.
-- [x] Add to PyPI
+- [x] Add to PyPI
```

### Comparing `brom_drake-0.0.2.post2/README.md` & `brom_drake-0.1.0/src/brom_drake.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,13 +1,51 @@
+Metadata-Version: 2.1
+Name: brom-drake
+Version: 0.1.0
+Summary: A set of convenient logging and testing tools for the Drake robotics toolbox.
+Author: Kwesi Rutledge
+Author-email: thesolitaryecrivain@gmail.com
+Keywords: drake,robotics,testing,logging
+Classifier: Programming Language :: Python :: 3
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+
 [![codecov](https://codecov.io/gh/kwesiRutledge/brom_drake-py/graph/badge.svg?token=0TI5PV2HUD)](https://codecov.io/gh/kwesiRutledge/brom_drake-py)
 
 # brom_drake-py
 Brom is a helper library for the [Drake](https://drake.mit.edu/) robotics simulation and verification library.
-Its goal is to simplify logging and robustness characterization
-of Drake simulations. 
+Its goal is to simplify common debugging and testing activities in Drake (for example, logging the outputs
+of systems in your block diagrams). 
+
+Some of Brom's features:
+
+Feature                    |  Code | Results
+:-------------------------:|:-------------------------:|:-------------------------:
+The Diagram Watcher (the `DiagramWatcher` will log + plot all output ports of your `Diagram` automatically) |`add_watcher_and_build()`| ![Creation of Brom Directory](./promo/BromWatcher0.gif)
+
+(More coming soon...)
+
+## Installation
+
+`brom_drake` is available on PyPI and installable with pip:
+
+```shell
+pip install brom-drake
+```
+
+### Developer install
+
+You can also install the package during local development by cloning
+the repository and running the following commands from inside it:
+
+```bash
+pip install -r requirements.txt
+pip install -e .
+```
 
 ## Use Cases
 
 Here are a few of the features available in `brom_drake` and how they work.
 
 ### Easily Log Your Diagram's Signals
 
@@ -24,15 +62,15 @@
 
 # Create a diagram builder
 builder = DiagramBuilder()
 
 # Add and connect your systems...
 
 # Add the watcher and build the diagram
-dw, diagram, diagram_context = add_watcher_and_build(builder)
+watcher, diagram, diagram_context = add_watcher_and_build(builder)
 
 # Set up simulation
 simulator = Simulator(diagram, diagram_context)
 simulator.set_target_realtime_rate(1.0)
 simulator.set_publish_every_time_step(False)
 
 # Run simulation
@@ -45,31 +83,28 @@
 What will happen whenever you use this function is that:
 - The `DiagramWatcher` will be created.
   - It will search through all systems that the `DiagramBuilder` has added.
   - For each system, the watcher will add a `VectorLogger` to each output port that is a `kVectorValued` port.
   - The `DiagramWatcher` will connect all loggers to all targeted ports (in the above case, we will target all available output ports).
 - After the simulation is run and the script completes, the watcher will save all data traces for each port in `.png` files. These plots will be in a new `.brom` directory.
 
-## Installation
-
-`brom_drake` is available on PyPI and installable with pip:
-
-```shell
-pip install brom-drake
-```
-
-### Developer install
-
-You can also install the package during local development by cloning
-the repository and running the following commands from inside it:
+### Watching Specific systems
 
-```bash
-pip install -r requirements.txt
-pip install -e .
+If you only want to watch a specific system, then you can do so by passing in information to the "targets" argument:
+```python
+watcher, _, _ = add_watcher_and_build(
+  builder,
+  targets=[
+    ("system_name", "port_name"),
+    "system_name2",
+  ],
+)
 ```
+The above code tells the watcher to watch the port named `port_name` on the system named `system_name`.
+(If you don't know your system's name in Drake, then you can usually find it by using the `get_name()` method.)
 
 ## FAQs
 
 ### Why the name Brom?
 
 [Brom the storyteller](https://inheritance.fandom.com/wiki/Brom) is a character from the
 [Inheritance](https://en.wikipedia.org/wiki/Eragon) series by Christopher Paolini.
@@ -93,8 +128,8 @@
   tutorial's diagram.
   - [x] Determine if we can use `DiagramTarget` objects to do everything (assuming that they are all valid). i.e., with the name and the port # can we do waht we want?
 - [ ] Add more examples
 - [x] Add Code coverage
 - [ ] Add support for abstract output ports?
 - [ ] Add more readme explanations of what is going on under the hood.
 - [ ] Add support for giving `DiagramTarget` (or simpler objects) to the convenience functions.
-- [x] Add to PyPI
+- [x] Add to PyPI
```

### Comparing `brom_drake-0.0.2.post2/setup.py` & `brom_drake-0.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     with codecs.open(
         os.path.join(here, "README.md"), encoding="utf-8"
     ) as f:
         long_description = "\n" + f.read()
 
     setup(
         name="brom_drake",
-        version='0.0.2-2',
+        version='0.1.0',
         author="Kwesi Rutledge",
         author_email="thesolitaryecrivain@gmail.com",
         description="A set of convenient logging and testing tools for the Drake robotics toolbox.",
         long_description_content_type="text/markdown",
         long_description=long_description,
         # packages=find_packages(where='src/brom_drake'),
         install_requires=['drake', 'meshcat', 'manipulation', 'loguru', 'matplotlib'],
```

### Comparing `brom_drake-0.0.2.post2/src/brom_drake/DiagramWatcher/DiagramWatcher.py` & `brom_drake-0.1.0/src/brom_drake/DiagramWatcher/DiagramWatcher.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from pydrake.multibody.plant import MultibodyPlant
 from pydrake.systems.framework import Diagram, DiagramBuilder, LeafSystem, PortDataType
 from pydrake.systems.primitives import (
     VectorLogSink, ConstantVectorSource, AffineSystem, LogVectorOutput,
 )
 
 from brom_drake.all import DiagramTarget
+from ..PortWatcher import PortWatcher
 from .constants import INELIGIBLE_SYSTEM_TYPES
 from .errors import UnrecognizedTargetError
 
 
 class DiagramWatcher:
     def __init__(
         self,
@@ -68,27 +69,34 @@
 
         # For Each Target with None ports, we will try to
         # "smartly" create the targets that we want to monitor
         inferred_targets = self.get_smart_targets(subject, targets)
         self.inferred_targets = inferred_targets
 
         # For each target's port, we will add a logger
-        self.loggers = {target.name: {} for target in inferred_targets}
+        self.port_watchers = {target.name: {} for target in inferred_targets}
+        loguru.logger.info("Adding loggers to the diagram... (via PortWatcher objects)")
         for target in inferred_targets:
             system = subject.GetSubsystemByName(target.name)
             for port_index in target.ports:
                 target_port = system.get_output_port(port_index)
 
                 if target_port.get_data_type() != PortDataType.kVectorValued:
                     print(f"Port {port_index} of system {target.name} is not vector-valued! Skipping...")
+                    loguru.logger.warning(
+                        f"Port {port_index} ({target_port.get_name()}) of system {target.name} is not vector-valued! " +
+                        "Will not add a logger for it.",
+                    )
                     continue
 
-                logger = LogVectorOutput(system.get_output_port(port_index), subject)
-                logger.set_name(f"{target.name}_logger_{port_index}")
-                self.loggers[target.name][port_index] = logger
+                self.port_watchers[target.name][port_index] = PortWatcher(
+                    system, target_port, subject,
+                    logger_name=f"{target.name}_logger_{port_index}",
+                    plot_dir=plot_dir,
+                )
 
     def __del__(self):
         """
         Description:
 
             Destructor for the Diagram Watcher.
             Will plot the data from all of our loggers if we have access to the diagram context.
@@ -99,142 +107,32 @@
         dpi = self.dpi
 
         is_ready_to_plot = self.diagram is not None
 
         # Upon deletion, we will PLOT the data from all of our loggers
         # if we have access to the diagram context
         if is_ready_to_plot:
-            for system_name in self.loggers:
+            for system_name in self.port_watchers:
                 system_ii = self.diagram.GetSubsystemByName(system_name)
-                ports_on_ii = self.loggers[system_name]
+                ports_on_ii = self.port_watchers[system_name]
                 for port_index in ports_on_ii:
-                    system_ii_port = system_ii.get_output_port(port_index)
-
-                    fig_ii_pi, ax_list_ii_pi = self.plot_logger_data(
-                        system_ii, port_index
-                    )
-                    # Save the figure, if plot was successful
-                    if fig_ii_pi is None:
-                        continue
-
-                    fig_ii_pi.savefig(
-                        f"{plot_dir}/{self.safe_system_name(system_name)}_port_{system_ii_port.get_name()}.png",
-                    )
-
-                # data and sampling times from the logger
-
-            # self.logger = LogOutput(diagram.get_context())
+                    temp_port_watcher = ports_on_ii[port_index]
+                    temp_port_watcher.savefigs(self.diagram_context)
 
 
     def configure_brom_activity_summary(self):
         """
         Description:
             Configures the "activity summary" a log of brom's activity.
         :return:
         """
         # Setup
-        loguru.logger.remove(0)  # Remove the default logger
+        loguru.logger.remove()  # Remove the default logger
         loguru.logger.add(self.plot_dir + "/activity_summary.log")
 
-    def safe_system_name(self, name: str) -> str:
-        """
-        Description:
-            Returns a safe name for the system.
-        :param name: System's name.
-        :return:
-        """
-        out = name
-        # First, let's check to see how many "/" exist in the name
-        slash_occurences = [i for i, letter in enumerate(name) if letter == "/"]
-        if len(slash_occurences) > 0:
-            out = out[slash_occurences[-1] + 1:]  # truncrate string based on the last slash
-
-        # Second, replace all spaces with underscores
-        out = out.replace(" ", "_")
-
-        return out
-
-    def plot_logger_data(
-        self,
-        system_ii: LeafSystem,
-        port_index: int,
-    ) -> (plt.Figure, List[plt.Axes]):
-        """
-        Description:
-
-            Plots the data from the logger for the specified system and port.
-        :param system_ii:
-        :param port_jj:
-        :return:
-        """
-        # Setup
-        port_jj = system_ii.get_output_port(port_index)
-        logger = self.loggers[system_ii.get_name()][port_index]
-
-        if self.diagram is None:
-            raise ValueError("Cannot plot data without access to the diagram context!")
-
-        diagram_context = self.diagram_context
-
-        # Get the log from the logger
-        temp_log = logger.FindLog(diagram_context)  # Extract the log from the logger
-
-        log_times = temp_log.sample_times()
-        data = temp_log.data()
-
-        if data.shape[0] == 0:
-            loguru.logger.warning(f"No data found for {system_ii.get_name()} - Port {port_index} ({port_jj.get_name()})! Skipping...")
-            return None, None
-
-        # Plot the data
-        n_rows, n_cols = self.compute_plot_shape(data.shape[0])
-
-        fig = plt.figure()
-        ax_list = []
-
-        for dim_index in range(port_jj.size()):
-            ax_list.append(
-                fig.add_subplot(n_rows, n_cols, 1 + dim_index)
-            )
-            plt.plot(log_times, data[dim_index, :])
-            # TODO: Create a flag for how verbose title will be
-            # plt.title(
-            #     system_ii.get_name() +
-            #     " - Port " + str(port_index) +
-            #     'Dim #' + str(dim_index)
-            # )
-            plt.title(f"Dim #{dim_index}")
-
-        plt.subplots_adjust(
-            left=0.1, bottom=0.1, right=0.95, top=0.95,
-            wspace=0.6, hspace=0.8,
-        )
-
-        return fig, ax_list
-
-    def compute_plot_shape(self, n_dims: int) -> tuple:
-        """
-        Description:
-            Computes the shape of the plot based on the data.
-        :param data: The data to be plotted.
-        :return:
-        """
-        if n_dims == 1:
-            return 1, 1
-        if n_dims == 2:
-            return 1, 2
-
-        if n_dims < 9:
-            return 2, int(np.ceil(n_dims / 2.0))
-
-        # Otherwise
-        return 3, int(np.ceil(n_dims / 3.0))
-
-        raise NotImplementedError(f"n_dims should be greater than 0! (received {n_dims})")
-
     def check_targets(
         self,
         targets: List[DiagramTarget],
         eligible_systems: List[Union[MultibodyPlant, AffineSystem, LeafSystem]],
     ) -> List[Union[MultibodyPlant, AffineSystem, LeafSystem]]:
         """
         Description:
@@ -259,24 +157,21 @@
         for target in targets:
             # Check if the target name is in the eligible systems
             if target.name not in eligible_system_dict.keys():
                 raise UnrecognizedTargetError(target, eligible_system_dict.keys())
 
             # If it is, then also check that the port index is correct
             if target.ports is None:
-                continue # No need to check things if ports is None
+                continue  # No need to check things if ports is None
 
             num_ports_in_target = eligible_system_dict[target.name].num_output_ports()
             for port_index in target.ports:
                 if port_index < 0 or port_index >= num_ports_in_target:
                     raise ValueError(f"Port index {port_index} is out of bounds for system {target.name} (only {num_ports_in_target} ports exist)")
 
-
-
-
         # All checks passed!
         pass
 
     def find_eligible_systems(
         self,
         builder: DiagramBuilder
     ) -> List[Union[MultibodyPlant, AffineSystem, LeafSystem]]:
@@ -287,18 +182,21 @@
             - Scene Graphs
             - Loggers
         """
 
         # Find all the systems that are eligible for logging
         eligible_systems = []
 
+        loguru.logger.info("Finding all eligible systems for logging...")
         for system in builder.GetSystems():
-            for system_type in INELIGIBLE_SYSTEM_TYPES:
-                if isinstance(system, system_type):
-                    break
+            if type(system) in INELIGIBLE_SYSTEM_TYPES:
+                loguru.logger.warning(
+                    f"System {system.get_name()} (of type {type(system)}) is not eligible for logging! Skipping..."
+                )
+                continue
 
             # Otherwise add to list
             eligible_systems.append(system)
 
         return eligible_systems
 
     def get_smart_targets(
```

### Comparing `brom_drake-0.0.2.post2/src/brom_drake/DiagramWatcher/errors.py` & `brom_drake-0.1.0/src/brom_drake/DiagramWatcher/errors.py`

 * *Files identical despite different names*

### Comparing `brom_drake-0.0.2.post2/src/brom_drake.egg-info/SOURCES.txt` & `brom_drake-0.1.0/src/brom_drake.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -9,9 +9,11 @@
 src/brom_drake.egg-info/top_level.txt
 src/brom_drake/DiagramTarget/DiagramTarget.py
 src/brom_drake/DiagramTarget/__init__.py
 src/brom_drake/DiagramWatcher/DiagramWatcher.py
 src/brom_drake/DiagramWatcher/__init__.py
 src/brom_drake/DiagramWatcher/constants.py
 src/brom_drake/DiagramWatcher/errors.py
+src/brom_drake/PortWatcher/PortWatcher.py
+src/brom_drake/PortWatcher/__init__.py
 src/brom_drake/all/__init__.py
 src/brom_drake/all/add_watcher.py
```

