# Comparing `tmp/peakrdl_markdown-0.1.7.tar.gz` & `tmp/peakrdl_markdown-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peakrdl_markdown-0.1.7.tar", max compression
+gzip compressed data, was "peakrdl_markdown-1.0.0.tar", max compression
```

## Comparing `peakrdl_markdown-0.1.7.tar` & `peakrdl_markdown-1.0.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    35149 2023-11-10 01:38:22.063259 peakrdl_markdown-0.1.7/LICENSE
--rw-r--r--   0        0        0     1241 2023-11-10 01:38:22.063259 peakrdl_markdown-0.1.7/README.md
--rw-r--r--   0        0        0     1569 2023-11-10 01:38:22.063259 peakrdl_markdown-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      170 2023-11-10 01:38:22.063259 peakrdl_markdown-0.1.7/src/peakrdl_markdown/__init__.py
--rw-r--r--   0        0        0     1484 2023-11-10 01:38:22.067259 peakrdl_markdown-0.1.7/src/peakrdl_markdown/__peakrdl__.py
--rw-r--r--   0        0        0    10500 2023-11-10 01:38:22.067259 peakrdl_markdown-0.1.7/src/peakrdl_markdown/exporter.py
--rw-r--r--   0        0        0     2585 1970-01-01 00:00:00.000000 peakrdl_markdown-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-16 19:19:49.504913 peakrdl_markdown-1.0.0/LICENSE
+-rw-r--r--   0        0        0     1259 2024-04-16 19:19:49.504913 peakrdl_markdown-1.0.0/README.md
+-rw-r--r--   0        0        0     2603 2024-04-16 19:19:49.504913 peakrdl_markdown-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      167 2024-04-16 19:19:49.504913 peakrdl_markdown-1.0.0/src/peakrdl_markdown/__init__.py
+-rw-r--r--   0        0        0     1481 2024-04-16 19:19:49.504913 peakrdl_markdown-1.0.0/src/peakrdl_markdown/__peakrdl__.py
+-rw-r--r--   0        0        0    11426 2024-04-16 19:19:49.504913 peakrdl_markdown-1.0.0/src/peakrdl_markdown/exporter.py
+-rw-r--r--   0        0        0     2939 1970-01-01 00:00:00.000000 peakrdl_markdown-1.0.0/PKG-INFO
```

### Comparing `peakrdl_markdown-0.1.7/LICENSE` & `peakrdl_markdown-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `peakrdl_markdown-0.1.7/README.md` & `peakrdl_markdown-1.0.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,33 @@
+# PeakRDL-Markdown
+
 [![Documentation Status](https://readthedocs.org/projects/peakrdl-markdown/badge/?version=latest)](http://peakrdl-markdown.readthedocs.io)
 [![build](https://github.com/SystemRDL/PeakRDL-Markdown/workflows/build/badge.svg)](https://github.com/SystemRDL/PeakRDL-Markdown/actions?query=workflow%3Abuild+branch%3Amain)
 [![Coverage Status](https://coveralls.io/repos/github/SystemRDL/PeakRDL-Markdown/badge.svg?branch=main)](https://coveralls.io/github/SystemRDL/PeakRDL-Markdown?branch=main)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/peakrdl-markdown.svg)](https://pypi.org/project/peakrdl-markdown)
 
-# PeakRDL-Markdown
-
 This package implements Markdown exporter for the PeakRDL toolchain.
 
 - **Export:** Convert compiled SystemRDL input into Markdown description.
 
 For the command line tool, see the [PeakRDL
 project](https://peakrdl.readthedocs.io).
 
 ## Usage
 
 PeakRDL project provides a standard CLI interface. It can be installed directly
 via pip:
 
-    $ pip install peakrdl-markdown
+```shell
+$ pip install peakrdl-markdown
+```
 
 Then this package can be used with the following command:
 
-    $ peakrdl markdown input_file.rdl -o output_file.md
+```shell
+$ peakrdl markdown input_file.rdl -o output_file.md
+```
 
 ## Documentation
 
 See the [PeakRDL-Markdown
 Documentation](http://peakrdl-markdown.readthedocs.io) for more details.
```

### Comparing `peakrdl_markdown-0.1.7/src/peakrdl_markdown/__peakrdl__.py` & `peakrdl_markdown-1.0.0/src/peakrdl_markdown/__peakrdl__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """PeakRDL Markdown plug-in."""
 
-__authors__ = ["Marek Pikuła <marek.pikula at embevity.com>"]
+__authors__ = ["Marek Pikuła <marek at serenitycode.dev>"]
 
 from typing import TYPE_CHECKING
 
 from peakrdl.plugins.exporter import ExporterSubcommandPlugin  # type: ignore
 
 from .exporter import MarkdownExporter
```

### Comparing `peakrdl_markdown-0.1.7/src/peakrdl_markdown/exporter.py` & `peakrdl_markdown-1.0.0/src/peakrdl_markdown/exporter.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,28 @@
 """PeakRDL Markdown exporter."""
 
-__authors__ = ["Marek Pikuła <marek.pikula at embevity.com>"]
+__authors__ = [
+    "Marek Pikuła <marek at serenitycode.dev>",
+    "Maciej Dudek <mdudek at antmicro.com>",
+]
 
 from collections import OrderedDict
 from dataclasses import dataclass
+from functools import reduce
+from operator import mul
 from pathlib import Path
 from typing import List, Optional, Union
 
 from markdownTable import markdownTable  # type:ignore
 from systemrdl.messages import MessageHandler  # type: ignore
 from systemrdl.node import (  # type: ignore
     AddressableNode,
     AddrmapNode,
     FieldNode,
+    MemNode,
     Node,
     RegfileNode,
     RegNode,
     RootNode,
 )
 
 
@@ -50,17 +56,24 @@
         return "\n" + "#" * depth + f" {title}\n\n"
 
     @staticmethod
     def _addrnode_info(node: AddressableNode):
         """Generate AddressableNode basic information dictionary."""
         ret: "OrderedDict[str, str]" = OrderedDict()
 
+        set_index = False
+        if node.is_array and node.current_idx is None:
+            node.current_idx = [0]
+            set_index = True
         ret["Absolute Address"] = f"0x{node.absolute_address:X}"
         ret["Base Offset"] = f"0x{node.raw_address_offset:X}"
-        ret["Size"] = f"0x{node.size:X}"
+        if node.is_array and node.array_dimensions is not None and set_index:
+            ret["Size"] = f"0x{node.size * reduce(mul, node.array_dimensions, 1):X}"
+        else:
+            ret["Size"] = f"0x{node.size:X}"
 
         if node.is_array:
             ret["Array Dimensions"] = str(node.array_dimensions)
             ret["Array Stride"] = f"0x{node.array_stride:X}"
             ret["Total Size"] = f"0x{node.total_size:X}"
 
         return ret
@@ -80,29 +93,35 @@
         name = node.get_html_name()
         if name is None:
             name = "—"
         else:
             name = name.replace("\n", "")
         return name
 
-    def _addrnode_header(self, node: AddressableNode, heading_level: int) -> str:
+    def _addrnode_header(
+        self, node: AddressableNode, msg: MessageHandler, heading_level: int
+    ) -> str:
         """Get the AddressableNode header.
 
         Arguments:
             node -- node to generate the header for.
+            msg -- message handler from top-level.
             heading_level -- Markdown heading level.
         """
         if isinstance(node, AddrmapNode):
             node_type_name = "address map"
         elif isinstance(node, RegfileNode):
             node_type_name = "register file"
+        elif isinstance(node, MemNode):
+            node_type_name = "memory"
         elif isinstance(node, RegNode):
             node_type_name = "register"
         else:
             node_type_name = "addressable node"
+            msg.warning(f"Unsupported type of node ({node.__class__.__name__}).")
 
         ret = self._heading(heading_level, f"{node.inst_name} {node_type_name}")
         ret += self._addrnode_info_md(node) + "\n\n"
         desc = node.get_html_desc()
         if desc is not None:
             ret += desc + "\n\n"
         return ret
@@ -156,77 +175,80 @@
 
         # Ensure proper format of the output path and that the directory exists.
         if not output_path.endswith(".md"):
             raise ValueError("The output file is not Markdown file.")
         Path(output_path).parent.mkdir(parents=True, exist_ok=True)
 
         # Run generation.
-        gen = self._add_addrmap_regfile(top, node.env.msg, depth - 1).generated
+        gen = self._add_addrmap_regfile_mem(top, node.env.msg, depth - 1).generated
 
         # Write to the file.
         with open(output_path, "w", encoding="UTF-8") as output:
             output.write(
                 "<!---\n"
                 "Markdown description for SystemRDL register map.\n\n"
                 f"Don't override. Generated from: {generated_from}\n"
                 "-->\n"
             )
             output.write(gen)
 
-    def _add_addrmap_regfile(
+    def _add_addrmap_regfile_mem(
         self,
-        node: Union[AddrmapNode, RegfileNode],
+        node: Union[AddrmapNode, RegfileNode, MemNode],
         msg: MessageHandler,
         depth: int,
     ) -> GenStageOutput:
-        """Generate addrmap or regfile.
+        """Generate addrmap, regfile or memory.
 
         Arguments:
-            node -- RegfileNode or AddrmapNode.
+            node -- MemNode, RegfileNode or AddrmapNode.
             msg -- message handler from top-level.
             depth -- depth of generation left.
 
         Keyword Arguments:
             is_top -- if the current not is the top node. If True the
                 specification is embedded as class member.
 
         Returns:
             Generated addrmap output.
         """
         members: List[MarkdownExporter.GenStageOutput] = []
         member_gen: str = ""
-        for child in node.children(unroll=True, skip_not_present=False):
-            if isinstance(child, (AddrmapNode, RegfileNode)):
-                output = self._add_addrmap_regfile(child, msg, depth - 1)
+        # Don't unroll register arrays when they are inside memories.
+        # Memories can contain hundreds of entires.
+        not_memory = not isinstance(node, MemNode)
+        for child in node.children(unroll=not_memory, skip_not_present=False):
+            if isinstance(child, (AddrmapNode, RegfileNode, MemNode)):
+                output = self._add_addrmap_regfile_mem(child, msg, depth - 1)
                 member_gen += output.generated
                 members.append(output)
             elif isinstance(child, RegNode):
                 output = self._add_reg(child, msg)
                 member_gen += output.generated
                 members.append(output)
             else:
                 msg.warning(
                     f"Unsupported type of node ({child.__class__.__name__}) "
                     f"for {'/'.join(child.get_path_segments())}."
                 )
 
-        gen: str = self._addrnode_header(node, 2)
+        gen: str = self._addrnode_header(node, msg, 2)
 
         if len(members) == 0:
             gen += "No supported members.\n"
         else:
             # Find the maximum width of the offset hex int and format the
             # offset for all members.
             base_addr_digits = max(
                 map(lambda m: len(f'{m.table_row["Offset"]:X}'), members)
             )
             for member in members:
-                member.table_row[
-                    "Offset"
-                ] = f'0x{member.table_row["Offset"]:0{base_addr_digits}X}'
+                member.table_row["Offset"] = (
+                    f'0x{member.table_row["Offset"]:0{base_addr_digits}X}'
+                )
 
             gen += (
                 markdownTable([*map(lambda m: m.table_row, members)])
                 .setParams(row_sep="markdown", quote=False)
                 .getMarkdown()
             )
 
@@ -251,15 +273,15 @@
         field_gen: str = ""
         members: List[MarkdownExporter.GenStageOutput] = []
         for field in node.fields(skip_not_present=True):
             output = self._add_field(field, msg)
             field_gen += output.generated
             members.append(output)
 
-        gen: str = self._addrnode_header(node, 3)
+        gen: str = self._addrnode_header(node, msg, 3)
         gen += (
             markdownTable([*map(lambda m: m.table_row, members)])
             .setParams(row_sep="markdown", quote=False)
             .getMarkdown()
         )
         gen += "\n"
```

### Comparing `peakrdl_markdown-0.1.7/PKG-INFO` & `peakrdl_markdown-1.0.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,60 +1,69 @@
 Metadata-Version: 2.1
 Name: peakrdl_markdown
-Version: 0.1.7
+Version: 1.0.0
 Summary: Export Markdown description from the systemrdl-compiler register model
 Home-page: https://github.com/SystemRDL/PeakRDL-Markdown
 License: GPL-3.0-only
 Author: Marek Pikuła
 Author-email: marek@serenitycode.dev
 Maintainer: Marek Pikuła
 Maintainer-email: marek@serenitycode.dev
-Requires-Python: >=3.7.0,<4.0.0
-Classifier: Development Status :: 4 - Beta
+Requires-Python: >=3.6.0,<4.0.0
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Electronic Design Automation (EDA)
+Requires-Dist: gitpython (>=3.1.41,<4.0.0) ; python_version >= "3.7"
+Requires-Dist: jinja2 (>=3.1.3,<4.0.0) ; python_version >= "3.7"
 Requires-Dist: peakrdl (>=1.1.0,<2.0.0)
 Requires-Dist: py-markdown-table (>=0.3.3,<0.4.0)
+Requires-Dist: pygments (>=2.15.0,<3.0.0) ; python_version >= "3.7"
+Requires-Dist: setuptools (>=65.5.1,<66.0.0) ; python_version >= "3.7"
 Requires-Dist: systemrdl-compiler (>=1.25.0,<2.0.0)
 Project-URL: Documentation, https://peakrdl-markdown.readthedocs.io
 Project-URL: Repository, https://github.com/SystemRDL/PeakRDL-Markdown
 Description-Content-Type: text/markdown
 
+# PeakRDL-Markdown
+
 [![Documentation Status](https://readthedocs.org/projects/peakrdl-markdown/badge/?version=latest)](http://peakrdl-markdown.readthedocs.io)
 [![build](https://github.com/SystemRDL/PeakRDL-Markdown/workflows/build/badge.svg)](https://github.com/SystemRDL/PeakRDL-Markdown/actions?query=workflow%3Abuild+branch%3Amain)
 [![Coverage Status](https://coveralls.io/repos/github/SystemRDL/PeakRDL-Markdown/badge.svg?branch=main)](https://coveralls.io/github/SystemRDL/PeakRDL-Markdown?branch=main)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/peakrdl-markdown.svg)](https://pypi.org/project/peakrdl-markdown)
 
-# PeakRDL-Markdown
-
 This package implements Markdown exporter for the PeakRDL toolchain.
 
 - **Export:** Convert compiled SystemRDL input into Markdown description.
 
 For the command line tool, see the [PeakRDL
 project](https://peakrdl.readthedocs.io).
 
 ## Usage
 
 PeakRDL project provides a standard CLI interface. It can be installed directly
 via pip:
 
-    $ pip install peakrdl-markdown
+```shell
+$ pip install peakrdl-markdown
+```
 
 Then this package can be used with the following command:
 
-    $ peakrdl markdown input_file.rdl -o output_file.md
+```shell
+$ peakrdl markdown input_file.rdl -o output_file.md
+```
 
 ## Documentation
 
 See the [PeakRDL-Markdown
 Documentation](http://peakrdl-markdown.readthedocs.io) for more details.
```

