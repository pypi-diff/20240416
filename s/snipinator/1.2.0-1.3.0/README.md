# Comparing `tmp/snipinator-1.2.0.tar.gz` & `tmp/snipinator-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/c/gdrive/code/snipinator.develop/develop/dist/.tmp-hup45qnf/snipinator-1.2.0.tar", last modified: Thu Apr 11 21:45:17 2024, max compression
+gzip compressed data, was "/mnt/c/gdrive/code/snipinator.develop/develop/dist/.tmp-jh0xe38z/snipinator-1.3.0.tar", last modified: Tue Apr 16 05:54:28 2024, max compression
```

## Comparing `snipinator-1.2.0.tar` & `snipinator-1.3.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0 realz     (1000) realz     (1000)        0 2024-04-11 21:45:16.996852 snipinator-1.2.0/
--rwxrwxrwx   0 realz     (1000) realz     (1000)     1102 2024-03-21 17:40:02.000000 snipinator-1.2.0/LICENSE.md
--rwxrwxrwx   0 realz     (1000) realz     (1000)    28191 2024-04-11 21:45:16.987808 snipinator-1.2.0/PKG-INFO
--rwxrwxrwx   0 realz     (1000) realz     (1000)    21315 2024-04-11 21:44:39.000000 snipinator-1.2.0/README.md
--rwxrwxrwx   0 realz     (1000) realz     (1000)     4199 2024-04-11 21:44:39.000000 snipinator-1.2.0/pyproject.toml
--rwxrwxrwx   0 realz     (1000) realz     (1000)       38 2024-04-11 21:45:16.998410 snipinator-1.2.0/setup.cfg
-drwxrwxrwx   0 realz     (1000) realz     (1000)        0 2024-04-11 21:45:16.850839 snipinator-1.2.0/snipinator/
--rwxrwxrwx   0 realz     (1000) realz     (1000)      514 2024-03-27 14:51:50.000000 snipinator-1.2.0/snipinator/__init__.py
--rwxrwxrwx   0 realz     (1000) realz     (1000)    18213 2024-03-27 14:51:50.000000 snipinator-1.2.0/snipinator/cli.py
--rwxrwxrwx   0 realz     (1000) realz     (1000)    31563 2024-04-11 21:44:39.000000 snipinator-1.2.0/snipinator/snipinate.py
--rwxrwxrwx   0 realz     (1000) realz     (1000)      866 2024-03-21 17:40:02.000000 snipinator-1.2.0/snipinator/snipinate_test.py
-drwxrwxrwx   0 realz     (1000) realz     (1000)        0 2024-04-11 21:45:16.965862 snipinator-1.2.0/snipinator.egg-info/
--rwxrwxrwx   0 realz     (1000) realz     (1000)    28191 2024-04-11 21:45:16.000000 snipinator-1.2.0/snipinator.egg-info/PKG-INFO
--rwxrwxrwx   0 realz     (1000) realz     (1000)      335 2024-04-11 21:45:16.000000 snipinator-1.2.0/snipinator.egg-info/SOURCES.txt
--rwxrwxrwx   0 realz     (1000) realz     (1000)        1 2024-04-11 21:45:16.000000 snipinator-1.2.0/snipinator.egg-info/dependency_links.txt
--rwxrwxrwx   0 realz     (1000) realz     (1000)       51 2024-04-11 21:45:16.000000 snipinator-1.2.0/snipinator.egg-info/entry_points.txt
--rwxrwxrwx   0 realz     (1000) realz     (1000)     1820 2024-04-11 21:45:16.000000 snipinator-1.2.0/snipinator.egg-info/requires.txt
--rwxrwxrwx   0 realz     (1000) realz     (1000)       11 2024-04-11 21:45:16.000000 snipinator-1.2.0/snipinator.egg-info/top_level.txt
+drwxrwxrwx   0 realz     (1000) realz     (1000)        0 2024-04-16 05:54:28.392822 snipinator-1.3.0/
+-rwxrwxrwx   0 realz     (1000) realz     (1000)     1102 2024-03-21 17:40:02.000000 snipinator-1.3.0/LICENSE.md
+-rwxrwxrwx   0 realz     (1000) realz     (1000)    35963 2024-04-16 05:54:28.385780 snipinator-1.3.0/PKG-INFO
+-r-xr-xr-x   0 realz     (1000) realz     (1000)    29087 2024-04-16 05:47:35.000000 snipinator-1.3.0/README.md
+-rwxrwxrwx   0 realz     (1000) realz     (1000)     4199 2024-04-16 05:46:20.000000 snipinator-1.3.0/pyproject.toml
+-rwxrwxrwx   0 realz     (1000) realz     (1000)       38 2024-04-16 05:54:28.393822 snipinator-1.3.0/setup.cfg
+drwxrwxrwx   0 realz     (1000) realz     (1000)        0 2024-04-16 05:54:28.275516 snipinator-1.3.0/snipinator/
+-rwxrwxrwx   0 realz     (1000) realz     (1000)      514 2024-03-27 14:51:50.000000 snipinator-1.3.0/snipinator/__init__.py
+-rwxrwxrwx   0 realz     (1000) realz     (1000)    18915 2024-04-16 05:46:20.000000 snipinator-1.3.0/snipinator/cli.py
+-rwxrwxrwx   0 realz     (1000) realz     (1000)    31563 2024-04-16 05:46:20.000000 snipinator-1.3.0/snipinator/snipinate.py
+-rwxrwxrwx   0 realz     (1000) realz     (1000)      866 2024-03-21 17:40:02.000000 snipinator-1.3.0/snipinator/snipinate_test.py
+drwxrwxrwx   0 realz     (1000) realz     (1000)        0 2024-04-16 05:54:28.367144 snipinator-1.3.0/snipinator.egg-info/
+-rwxrwxrwx   0 realz     (1000) realz     (1000)    35963 2024-04-16 05:54:28.000000 snipinator-1.3.0/snipinator.egg-info/PKG-INFO
+-rwxrwxrwx   0 realz     (1000) realz     (1000)      335 2024-04-16 05:54:28.000000 snipinator-1.3.0/snipinator.egg-info/SOURCES.txt
+-rwxrwxrwx   0 realz     (1000) realz     (1000)        1 2024-04-16 05:54:28.000000 snipinator-1.3.0/snipinator.egg-info/dependency_links.txt
+-rwxrwxrwx   0 realz     (1000) realz     (1000)       51 2024-04-16 05:54:28.000000 snipinator-1.3.0/snipinator.egg-info/entry_points.txt
+-rwxrwxrwx   0 realz     (1000) realz     (1000)     1820 2024-04-16 05:54:28.000000 snipinator-1.3.0/snipinator.egg-info/requires.txt
+-rwxrwxrwx   0 realz     (1000) realz     (1000)       11 2024-04-16 05:54:28.000000 snipinator-1.3.0/snipinator.egg-info/top_level.txt
```

### Comparing `snipinator-1.2.0/LICENSE.md` & `snipinator-1.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `snipinator-1.2.0/PKG-INFO` & `snipinator-1.3.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snipinator
-Version: 1.2.0
+Version: 1.3.0
 Summary: Python code snippets for markdown files, e.g READMEs, from actual (testable) code.
 Author-email: AYF <realazthat@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Azriel Fasten.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
@@ -134,47 +134,87 @@
 WARNING: This file is auto-generated by snipinator. Do not edit directly.
 SOURCE: `README.md.jinja2`.
 
 -->
 <!--
 
 
+
+
 -->
 
-# Snipinator
+# <div align="center">![Snipinator][22]</div>
+
+<div align="center">
+
+<!-- Icons from https://lucide.dev/icons/users -->
+<!-- Icons from https://lucide.dev/icons/laptop-minimal -->
+
+![**Audience:** Developers][19] ![**Platform:** Linux][20]
+
+</div>
+
+<p align="center">
+  <strong>
+    <a href="#-features">🎇Features</a> &nbsp;&bull;&nbsp;
+    <a href="#-installation">🛠️Installation</a> &nbsp;&bull;&nbsp;
+    <a href="#-usage">🔧Usage</a> &nbsp;&bull;&nbsp;
+    <a href="#-command-line-options">💻CLI</a> &nbsp;&bull;&nbsp;
+    <a href="#-examples">💡Examples</a> &nbsp;&bull;&nbsp;
+    <a href="#-api">🤖API</a> &nbsp;&bull;&nbsp;
+    <a href="#-requirements">✅Requirements</a> &nbsp;&bull;&nbsp;
+    <a href="#-gotchas-and-limitations">🚸Gotchas</a>
+  </strong>
+</p>
+
+<div align="center">
 
-![Top language][9] ![GitHub License][3] [![PyPI - Version][4]][5]
+![Top language][9] [![GitHub License][3]][21] [![PyPI - Version][4]][5]
 [![Python Version][8]][5]
 
-|         | Status                     | Stable                    | Unstable                  |                    |
-| ------- | -------------------------- | ------------------------- | ------------------------- | ------------------ |
-| Master  | [![Build and Test][1]][2]  | [![since tagged][6]][10]  |                           | ![last commit][7]  |
-| Develop | [![Build and Test][11]][2] | [![since tagged][12]][13] | [![since tagged][15]][16] | ![last commit][14] |
+**CLI to embed (testable) snippets from your codebase into your README**
 
-CLI to embed snippets from your {python,other} codebases into your `README.md`.
+</div>
 
-## What
+---
 
-What it does: Lets you make a `EXAMPLE.md` template and include snippets from
-your (working and tested) python codebase.
+<div align="center">
 
-Turn this (`snipinator/examples/EXAMPLE.md.jinja2`):
+|                   | Status                     | Stable                    | Unstable                  |                    |
+| ----------------- | -------------------------- | ------------------------- | ------------------------- | ------------------ |
+| **[Master][17]**  | [![Build and Test][1]][2]  | [![since tagged][6]][10]  |                           | ![last commit][7]  |
+| **[Develop][18]** | [![Build and Test][11]][2] | [![since tagged][12]][13] | [![since tagged][15]][16] | ![last commit][14] |
 
-````md
+</div>
+
+## ❔ What
+
+What it does: **Snipinator** lets you take a `EXAMPLE.md` template and include
+snippets from your (working and tested) codebase.
+
+Turn this (`./snipinator/examples/EXAMPLE.md.jinja2`):
+
+<!---->
+```md
 # A README
 
 Here is a code snippet:
 
 `{{ pysnippet(path='snipinator/examples/code.py', symbol='MyClass', backtickify='py') }}`
 
-````
+Note that `code.py` has a test:
+[{{path('./snipinator/examples/code_test.py')}}](./snipinator/examples/code_test.py)
+
+```
+<!---->
 
-Into this (`snipinator/examples/EXAMPLE.generated.md`):
+Into this (`./snipinator/examples/EXAMPLE.generated.md`):
 
-``````md
+<!---->
+`````md
 <!--
 
 WARNING: This file is auto-generated by snipinator. Do not edit directly.
 SOURCE: `snipinator/examples/EXAMPLE.md.jinja2`.
 
 -->
 # A README
@@ -189,71 +229,70 @@
     self.name = name
 
   def MyClassMethod(self):
     """This is a method of MyClass"""
     print(self.name)
 ````
 
-``````
+Note that `code.py` has a test:
+[./snipinator/examples/code_test.py](./snipinator/examples/code_test.py)
 
-## Features
+`````
+<!---->
 
-- Supports anything Jinja2 supports.
-- First class support for python source code.
+## 🎇 Features
+
+- 📦✅🪄 Supports anything **[Jinja2](https://github.com/pallets/jinja)**
+  supports.
+- 🥇🐍📜 First-class support for **python** source code.
   - Can include python function signatures, docstrings, entire function source
     code, classes.
-- Supports any language.
-  - With delimiter markers, or entire inclusion of the entire file.
-- First class support for markdown output (with backtickify, decomentify).
-- Can include shell output.
-  - Supports ANSI colors with SVG output.
-
-## Getting Started
-
-### Install
-
-#### Tested on
-
-- WSL2 Ubuntu 20.04, Python 3.8.0
-- Ubuntu 20.04, Python 3.8.0, 3.9.0, 3.10.0, 3.11.0, 3.12.0, tested in GitHub
-  Actions workflow
-  ([build-and-test.yml](./.github/workflows/build-and-test.yml)).
+- ✂🌐🗂️ Snip from **any source code language**.
+  - Put delimiter markers into the code (e.g `# START_SNIPPET`,
+    `# END_TEMPLATE`), and use [snippet()](#snippet).
+- 🥇🔖📜 First-class support for **Markdown** templates (with backtickify,
+  decomentify).
+- 📦🐚🖨️ Can include **[shell](#shell) output**.
+  - Supports ANSI colors :heart: :green_heart: :blue_heart: with SVG output
+    :camera:.
+- ⚙️🔗🗃️ More robust **references/links** to local files using [path()](#path).
 
-**Requirements:**
-
-- Linux-like environment
-  - Why: Uses pexpect.spawn().
-- Python 3.8+
-  - Why: Some dev dependencies require Python 3.8+.
+## 🛠️ Installation
 
 ```bash
 # Install from pypi (https://pypi.org/project/snipinator/)
 pip install snipinator
 
 # Install from git (https://github.com/realazthat/snipinator)
-pip install git+https://github.com/realazthat/snipinator.git@v1.2.0
+pip install git+https://github.com/realazthat/snipinator.git@v1.3.0
 ```
 
-### Use
+## 🔧 Usage
 
-Example tempalte README:
-[`snipinator/examples/EXAMPLE.md.jinja2`](./snipinator/examples/EXAMPLE.md.jinja2):
+Example template README:
+([./snipinator/examples/EXAMPLE.md.jinja2](./snipinator/examples/EXAMPLE.md.jinja2)):
 
-````md
+<!---->
+```md
 # A README
 
 Here is a code snippet:
 
 `{{ pysnippet(path='snipinator/examples/code.py', symbol='MyClass', backtickify='py') }}`
 
-````
+Note that `code.py` has a test:
+[{{path('./snipinator/examples/code_test.py')}}](./snipinator/examples/code_test.py)
+
+```
+<!---->
 
 Generating the README:
 
-``````bash
+<!---->
+`````bash
 $ python -m snipinator.cli -t snipinator/examples/EXAMPLE.md.jinja2
 <!--
 
 WARNING: This file is auto-generated by snipinator. Do not edit directly.
 SOURCE: `snipinator/examples/EXAMPLE.md.jinja2`.
 
 -->
@@ -269,23 +308,77 @@
     self.name = name
 
   def MyClassMethod(self):
     """This is a method of MyClass"""
     print(self.name)
 ````
 
-``````
+Note that `code.py` has a test:
+[./snipinator/examples/code_test.py](./snipinator/examples/code_test.py)
 
-CLI usage help:
+`````
+<!---->
 
-<!----><img src="README.help.generated.svg" alt="Output of `python -m snipinator.cli --help`" /><!---->
+## 💻 Command Line Options
 
-## Available Functions in Jinja2
+<!---->
+<img src="README.help.generated.svg" alt="Output of `python -m snipinator.cli --help`" />
+<!---->
 
-````py
+## 💡 Examples
+
+- Snipinator's own `README`:
+  - Template: [./README.md.jinja2](./README.md.jinja2).
+  - Generated: [./README.md](./README.md).
+  - Generation script:
+    [./scripts/generate-readme.sh](./scripts/generate-readme.sh).
+- Example:
+  - Template:
+    [./snipinator/examples/EXAMPLE.md.jinja2](./snipinator/examples/EXAMPLE.md.jinja2).
+  - Generated:
+    [./snipinator/examples/EXAMPLE.generated.md](./snipinator/examples/EXAMPLE.generated.md).
+  - Generation script:
+    [./snipinator/examples/example.sh](./snipinator/examples/example.sh).
+- Long example of many features:
+  - Template:
+    [./snipinator/examples/LONG-EXAMPLE.md.jinja2](./snipinator/examples/LONG-EXAMPLE.md.jinja2).
+  - Generated:
+    [./snipinator/examples/LONG-EXAMPLE.generated.md](./snipinator/examples/LONG-EXAMPLE.generated.md).
+  - Generation script:
+    [./snipinator/examples/long-example.sh](./snipinator/examples/long-example.sh).
+- Projects using Snipinator:
+  - [github.com/realazthat/snipinator](https://github.com/realazthat/snipinator),
+    See
+    [snipinator/README.md.jinja2](https://github.com/realazthat/snipinator/blob/61cb88593baa099dc375cf5fd40679e4be673fc5/README.md.jinja2).
+  - [github.com/realazthat/changeguard](https://github.com/realazthat/changeguard),
+    See
+    [changeguard/README.md.jinja2](https://github.com/realazthat/changeguard/blob/87d5104b52e651bb9195a3d46dd7f050acbcb534/README.md.jinja2).
+  - [github.com/realazthat/comfy-catapult](https://github.com/realazthat/comfy-catapult),
+    See
+    [comfy-catapult/README.md.jinja2](https://github.com/realazthat/comfy-catapult/blob/ff353d48b25fa7b9c35fa11b31d5f2b3039c41c8/README.md.jinja2).
+  - [github.com/realazthat/comfylowda](https://github.com/realazthat/comfylowda),
+    See
+    [comfylowda/README.md.jinja2](https://github.com/realazthat/comfylowda/blob/e01a32c38107aa0b89ccea21c4678d193a186a78/README.md.jinja2).
+  - [github.com/realazthat/excalidraw-brute-export-cli](https://github.com/realazthat/excalidraw-brute-export-cli),
+    See
+    [excalidraw-brute-export-cli/README.md.jinja2](https://github.com/realazthat/excalidraw-brute-export-cli/blob/54a3b5b08b644e61c721ab565c576094234c5cc7/README.md.jinja2).
+
+## 🤖 API
+
+(Jinja2) Functions made available:
+
+### pysnippet
+
+Used several times in
+[./snipinator/examples/LONG-EXAMPLE.md.jinja2](./snipinator/examples/LONG-EXAMPLE.md.jinja2).
+
+Documentation:
+
+<!---->
+```py
 def pysnippet(path: str,
               symbol: Optional[str],
               *,
               escape: bool = False,
               indent: Union[str, int, None] = None,
               backtickify: Union[bool, str] = False,
               decomentify: Union[bool, Literal['nl']] = False,
@@ -310,17 +403,25 @@
         newline delimiters. Defaults to False.
       _ctx (_Context): This is used by the system and is not available as an
         argument.
 
   Returns:
       Union[str, markupsafe.Markup]: The snippet.
   """
-````
+```
+<!---->
 
-````py
+### pysignature
+
+Used several times in [./README.md.jinja2](./README.md.jinja2).
+
+Documentation:
+
+<!---->
+```py
 def pysignature(path: str,
                 symbol: str,
                 *,
                 escape: bool = False,
                 indent: Union[str, int, None] = None,
                 backtickify: Union[bool, str] = False,
                 decomentify: Union[bool, Literal['nl']] = False,
@@ -346,17 +447,25 @@
         newline delimiters. Defaults to False.
       _ctx (_Context): This is used by the system and is not available as an
         argument.
 
   Returns:
       str: The signature and docstring.
   """
-````
+```
+<!---->
 
-````py
+### rawsnippet
+
+Used several times in [./README.md.jinja2](./README.md.jinja2).
+
+Documentation:
+
+<!---->
+```py
 def rawsnippet(path: str,
                *,
                escape: bool = False,
                indent: Union[str, int, None] = None,
                backtickify: Union[bool, str] = False,
                decomentify: Union[bool, Literal['nl']] = False,
                _ctx: _Context) -> Union[str, markupsafe.Markup]:
@@ -379,29 +488,38 @@
       _ctx (_Context): This is used by the system and is not available as an
         argument.
 
   Returns:
       Union[str, markupsafe.Markup]: The snippet.
   """
 
-````
+```
+<!---->
 
-````py
+### snippet
+
+Example in
+[./snipinator/examples/LONG-EXAMPLE.md.jinja2](./README.md.jinja2).
+
+Documentation:
+
+<!---->
+```py
 def snippet(path: str,
             start: str,
             end: str,
             *,
             escape: bool = False,
             indent: Union[str, int, None] = None,
             backtickify: Union[bool, str] = False,
             decomentify: Union[bool, Literal['nl']] = False,
             _ctx: _Context) -> Union[str, markupsafe.Markup]:
   """Returns a _delimited_ snippet from a file.
 
-  Does not return the delimeters themselves.
+  Does not return the delimiters themselves.
 
   Args:
       path (str): The path to the file.
       start (str): A string that indicates the start of the snippet.
       end (str): A string that indicates the end of the snippet.
       escape (bool, optional): Should use HTML entities escaping? Defaults to
         False.
@@ -418,17 +536,25 @@
       _ctx (_Context): This is used by the system and is not available as an
         argument.
 
   Returns:
       Union[str, markupsafe.Markup]: The snippet.
   """
 
-````
+```
+<!---->
 
-````py
+### shell
+
+Used several times in [./README.md.jinja2](./README.md.jinja2).
+
+Documentation:
+
+<!---->
+```py
 def shell(args: str,
           *,
           escape: bool = False,
           indent: Union[str, int, None] = None,
           backtickify: Union[bool, str] = False,
           decomentify: Union[bool, Literal['nl']] = False,
           rich: Union[Literal['svg'], Literal['img+b64+svg'], Literal['raw'],
@@ -493,20 +619,80 @@
         the output? Defaults to True.
       _ctx (_Context): This is used by the system and is not available as an
         argument.
 
   Returns:
       Union[str, markupsafe.Markup]: Returns the output of the command.
   """
-````
+```
+<!---->
+
+### path
+
+Used several times in [./README.md.jinja2](./README.md.jinja2).
+
+Documentation:
+
+<!---->
+```py
+def path(path: str,
+         *,
+         escape: bool = False,
+         indent: Union[str, int, None] = None,
+         backtickify: Union[bool, str] = False,
+         decomentify: Union[bool, Literal['nl']] = False,
+         _ctx: _Context) -> Union[str, markupsafe.Markup]:
+  """Verifies that `path` exists, and just returns `path`.
+
+  Unfortunately, I don't know how to use this inside a link, because the
+  formatters will destroy it, and it cannot be put into a code block (as the url
+  section of a link in markdown does not allow code blocks).
+
+  Args:
+      path (str): The path to verify.
+      escape (bool, optional): Should use HTML entities escaping? Defaults to
+        False.
+      indent (Union[str, int, None], optional): Should indent? By how much, or
+        with what prefix? Defaults to None.
+      backtickify (Union[bool, str], optional): Should surround with backticks?
+        With what language? Defaults to False.
+      decomentify (Union[bool, Literal['nl']]): Assuming that you will be using
+        HTML comments around this call, setting this to true will add
+        correspondingcomments to uncomment the output. This allows you to have
+        the Jinja2 call unmolested by markdown formatters, because they will be
+        inside of a comment section. "nl" adds additional newlines after the
+        newline delimiters. Defaults to False.
+      _ctx (_Context): This is used by the system and is not available as an
+        argument.
+
+  Returns:
+      Union[str, markupsafe.Markup]: Just returns the path. If the path doesn't exist,
+        it will raise an error.
+  """
+```
+<!---->
 
 Also see Jinja2 v3
 [Template Designer Documentation](https://jinja.palletsprojects.com/en/3.1.x/templates/).
 
-## Gotchas
+## ✅ Requirements
+
+- Linux-like environment
+  - Why: Uses pexpect.spawn().
+- Python 3.8+
+  - Why: Some dev dependencies require Python 3.8+.
+
+### Tested on
+
+- WSL2 Ubuntu 20.04, Python 3.8.0
+- Ubuntu 20.04, Python 3.8.0, 3.9.0, 3.10.0, 3.11.0, 3.12.0, tested in GitHub
+  Actions workflow
+  ([build-and-test.yml](./.github/workflows/build-and-test.yml)).
+
+## 🚸 Gotchas and Limitations
 
 - **Security:** This tool is NOT designed to be used with untrusted input. It is
   designed to be used with your own codebase. Even when using your own input, be
   careful that your own code won't be doing anything that might inadvertently
   include untrusted input.
 - Be careful to escape `{{` and `}}`,
   or `{%` and `%}` or anything jinja2
@@ -526,15 +712,15 @@
   ` ````language ```My Snippet``` ```` ` and this is a method that Markdown uses
   to allow embedded backticks inside a code block.
 - Formatting: The `{{` `}}` used to
   surround the snippet calls will unfortunately be formatted by a Markdown
   formatter and make the call invalid. Workarounds:
   - **Decommentify**: Put the snippet call inside a HTML comment, then use
     `decommentify` parameter. See
-    [`snipinator/examples/LONG-EXAMPLE.md.jinja2`](./snipinator/examples/LONG-EXAMPLE.md.jinja2)
+    [./snipinator/examples/LONG-EXAMPLE.md.jinja2](./snipinator/examples/LONG-EXAMPLE.md.jinja2)
     for examples.
   - [prettier](https://prettier.io/) formatter is pretty good at leaving the
     Jinja2 calls alone, especially if you don't have any spaces. This especially
     helps for markdown "reference-style links" that have Jinja2 calls in them
     generating part of the URL, mdformat will URL encode the Jinja2 calls,
     and/or split them on spaces, which is not what we want. prettier will leave
     them alone.
@@ -551,82 +737,79 @@
   - Snipinator will optionally chmod the file for you to make it read-only.
 - Newlines: This program assumes LF newlines. I don't know if it will work for
   anything else.
 - Combining `backtickify` and `indent`: Doesn't make much sense, but if you do
   it, it will run backtickify first, then indent everything including the
   backticks.
 
-## Examples
+## 🔑 License
 
-- Snipinator's own `README` at
-  [`./README.md.jinja2`](./README.md.jinja2).
-  - Generated: [`./README.md`](./README.md).
-  - Generation script:
-    [`./scripts/generate-readme.sh`](./scripts/generate-readme.sh).
-- [`snipinator/examples/EXAMPLE.md.jinja2`](./snipinator/examples/EXAMPLE.md.jinja2).
-  - Generated:
-    [`snipinator/examples/EXAMPLE.generated.md`](./snipinator/examples/EXAMPLE.generated.md).
-  - Generation script:
-    [`./snipinator/examples/example.sh`](./snipinator/examples/example.sh).
-- [`snipinator/examples/LONG-EXAMPLE.md.jinja2`](./snipinator/examples/LONG-EXAMPLE.md.jinja2).
-  - Generated:
-    [`snipinator/examples/LONG-EXAMPLE.generated.md`](./snipinator/examples/LONG-EXAMPLE.generated.md).
-  - Generation script:
-    [`./snipinator/examples/long-example.sh`](./snipinator/examples/long-example.sh).
+This project is licensed under the MIT License - see the
+[./LICENSE.md](./LICENSE.md) file for details.
 
-## Thanks
+## 🙏 Thanks
 
 Main libraries used in Snipinator are:
 
 - Templating: [Jinja2](https://github.com/pallets/jinja).
 - Snippet inclusion: Python's AST library.
 - Colorful CLI help: [rich-argparse](https://github.com/hamdanal/rich-argparse).
 - ANSI coloring shell output:
   {[pexpect](https://pexpect.readthedocs.io/en/stable/),
   [rich](https://github.com/Textualize/rich)}.
 
-## Contributions
+## Related Projects {#thanks}
+
+- [ARMmbed/snippet](https://github.com/ARMmbed/snippet) "A Python3 tool to
+  extract code snippets from source files".
+- [SimonCropp/MarkdownSnippets](https://github.com/SimonCropp/MarkdownSnippets)
+  "Extracts snippets from code files and merges them into markdown documents".
+- [shiftkey/scribble](https://github.com/shiftkey/scribble) "Making
+  documentation for .NET projects easy and fun".
+
+## 🫡Contributions
 
 ### Development environment: Linux-like
 
 - For running `pre.sh` (Linux-like environment).
   - Requires `pyenv`, or an exact matching version of python as in
     `.python-version` (which is currently
     `3.8.0
 `).
   - `jq`, ([installation](https://jqlang.github.io/jq/)) required for
     [yq](https://github.com/kislyuk/yq), which is itself required for our
-    `README.md` generation, which uses `tomlq` (from the
+    `./README.md` generation, which uses `tomlq` (from the
     [yq](https://github.com/kislyuk/yq) package) to include version strings from
-    `pyproject.toml`.
+    `./pyproject.toml`.
   - `bash`, `grep`, `awk`, `sed` `xxd`, `git`, `xxhash` (for tests/workflows).
   - Requires nodejs (for act).
   - Requires Go (to run act).
   - docker (for act).
 
 ### Commit Process
 
 1. (Optionally) Fork the `develop` branch.
 2. Stage your files: `git add path/to/file.py`.
 3. `bash scripts/pre.sh`, this will format, lint, and test the code.
-4. `git status` check if anything changed (generated `README.md` for
-   example), if so, `git add` the changes, and go back to the previous step.
+4. `git status` check if anything changed (generated `./README.md`
+   for example), if so, `git add` the changes, and go back to the previous step.
 5. `git commit -m "..."`.
 6. Make a PR to `develop` (or push to develop if you have the rights).
 
-## Release Process
+## ⛙ Release Process
 
 These instructions are for maintainers of the project.
 
-1. In the `develop` branch, run `bash scripts/pre.sh` to ensure
+1. In the `develop` branch, run `bash ./scripts/pre.sh` to ensure
    everything is in order.
-2. In the `develop` branch, bump the version in `pyproject.toml`,
+2. In the `develop` branch, bump the version in `./pyproject.toml`,
    following semantic versioning principles. Also modify the
    `last_unstable_release` and `last_stable_release` in the
-   `[tool.changeguard-project-metadata]` table as appropriate.
+   `[tool.changeguard-project-metadata]` table as appropriate. Run
+   `bash scripts/pre.sh` to ensure everything is in order.
 3. In the `develop` branch, commit these changes with a message like
    `"Prepare release X.Y.Z"`. (See the contributions section
    [above](#commit-process)).
 4. Merge the `develop` branch into the `master` branch:
    `git checkout master && git merge develop --no-ff`.
 5. `master` branch: Tag the release: Create a git tag for the release with
    `git tag -a vX.Y.Z -m "Version X.Y.Z"`.
@@ -636,32 +819,51 @@
    `git push && git push --tags`.
 8. The `--no-ff` option adds a commit to the master branch for the merge, so
    refork the develop branch from the master branch:
    `git checkout develop && git merge master`.
 9. Push the develop branch to GitHub: `git push origin develop`.
 
 [1]:
-  https://github.com/realazthat/snipinator/actions/workflows/build-and-test.yml/badge.svg?branch=master
+  https://img.shields.io/github/actions/workflow/status/realazthat/snipinator/build-and-test.yml?branch=master&style=plastic
 [2]:
   https://github.com/realazthat/snipinator/actions/workflows/build-and-test.yml
-[3]: https://img.shields.io/github/license/realazthat/snipinator
-[4]: https://img.shields.io/pypi/v/snipinator
+[3]:
+  https://img.shields.io/github/license/realazthat/snipinator?style=plastic&color=0A1E1E
+[4]:
+  https://img.shields.io/pypi/v/snipinator?style=plastic&color=0A1E1E
 [5]: https://pypi.org/project/snipinator/
 [6]:
-  https://img.shields.io/github/commits-since/realazthat/snipinator/v1.2.0/master
-[7]: https://img.shields.io/github/last-commit/realazthat/snipinator/master
-[8]: https://img.shields.io/pypi/pyversions/snipinator
+  https://img.shields.io/github/commits-since/realazthat/snipinator/v1.3.0/master?style=plastic
+[7]:
+  https://img.shields.io/github/last-commit/realazthat/snipinator/master?style=plastic
+[8]:
+  https://img.shields.io/pypi/pyversions/snipinator?style=plastic&color=0A1E1E
 [9]:
-  https://img.shields.io/github/languages/top/realazthat/snipinator.svg?&cacheSeconds=28800
+  https://img.shields.io/github/languages/top/realazthat/snipinator.svg?&cacheSeconds=28800&style=plastic&color=0A1E1E
 [10]:
-  https://github.com/realazthat/snipinator/compare/v1.2.0...master
+  https://github.com/realazthat/snipinator/compare/v1.3.0...master
 [11]:
-  https://github.com/realazthat/snipinator/actions/workflows/build-and-test.yml/badge.svg?branch=develop
+  https://img.shields.io/github/actions/workflow/status/realazthat/snipinator/build-and-test.yml?branch=develop&style=plastic
 [12]:
-  https://img.shields.io/github/commits-since/realazthat/snipinator/v1.2.0/develop
+  https://img.shields.io/github/commits-since/realazthat/snipinator/v1.3.0/develop?style=plastic
 [13]:
-  https://github.com/realazthat/snipinator/compare/v1.2.0...develop
-[14]: https://img.shields.io/github/last-commit/realazthat/snipinator/develop
+  https://github.com/realazthat/snipinator/compare/v1.3.0...develop
+[14]:
+  https://img.shields.io/github/last-commit/realazthat/snipinator/develop?style=plastic
 [15]:
-  https://img.shields.io/github/commits-since/realazthat/snipinator/v1.2.0/develop
+  https://img.shields.io/github/commits-since/realazthat/snipinator/v1.3.0/develop?style=plastic
 [16]:
-  https://github.com/realazthat/snipinator/compare/v1.2.0...develop
+  https://github.com/realazthat/snipinator/compare/v1.3.0...develop
+[17]: https://github.com/realazthat/snipinator/tree/master
+[18]: https://github.com/realazthat/snipinator/tree/develop
+
+<!-- Logo from https://lucide.dev/icons/users -->
+
+[19]:
+  https://img.shields.io/badge/Audience-Developers-0A1E1E?style=plastic&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIyNCIgaGVpZ2h0PSIyNCIgdmlld0JveD0iMCAwIDI0IDI0IiBmaWxsPSJub25lIiBzdHJva2U9ImN1cnJlbnRDb2xvciIgc3Ryb2tlLXdpZHRoPSIyIiBzdHJva2UtbGluZWNhcD0icm91bmQiIHN0cm9rZS1saW5lam9pbj0icm91bmQiIGNsYXNzPSJsdWNpZGUgbHVjaWRlLXVzZXJzIj48cGF0aCBkPSJNMTYgMjF2LTJhNCA0IDAgMCAwLTQtNEg2YTQgNCAwIDAgMC00IDR2MiIvPjxjaXJjbGUgY3g9IjkiIGN5PSI3IiByPSI0Ii8+PHBhdGggZD0iTTIyIDIxdi0yYTQgNCAwIDAgMC0zLTMuODciLz48cGF0aCBkPSJNMTYgMy4xM2E0IDQgMCAwIDEgMCA3Ljc1Ii8+PC9zdmc+
+
+<!-- Logo from https://lucide.dev/icons/laptop-minimal -->
+
+[20]:
+  https://img.shields.io/badge/Platform-Linux-0A1E1E?style=plastic&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIyNCIgaGVpZ2h0PSIyNCIgdmlld0JveD0iMCAwIDI0IDI0IiBmaWxsPSJub25lIiBzdHJva2U9ImN1cnJlbnRDb2xvciIgc3Ryb2tlLXdpZHRoPSIyIiBzdHJva2UtbGluZWNhcD0icm91bmQiIHN0cm9rZS1saW5lam9pbj0icm91bmQiIGNsYXNzPSJsdWNpZGUgbHVjaWRlLWxhcHRvcC1taW5pbWFsIj48cmVjdCB3aWR0aD0iMTgiIGhlaWdodD0iMTIiIHg9IjMiIHk9IjQiIHJ4PSIyIiByeT0iMiIvPjxsaW5lIHgxPSIyIiB4Mj0iMjIiIHkxPSIyMCIgeTI9IjIwIi8+PC9zdmc+
+[21]: ./LICENSE.md
+[22]: ./.github/logo-exported.svg
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `snipinator-1.2.0/README.md` & `snipinator-1.3.0/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -3,47 +3,87 @@
 WARNING: This file is auto-generated by snipinator. Do not edit directly.
 SOURCE: `README.md.jinja2`.
 
 -->
 <!--
 
 
+
+
 -->
 
-# Snipinator
+# <div align="center">![Snipinator][22]</div>
+
+<div align="center">
+
+<!-- Icons from https://lucide.dev/icons/users -->
+<!-- Icons from https://lucide.dev/icons/laptop-minimal -->
+
+![**Audience:** Developers][19] ![**Platform:** Linux][20]
+
+</div>
+
+<p align="center">
+  <strong>
+    <a href="#-features">🎇Features</a> &nbsp;&bull;&nbsp;
+    <a href="#-installation">🛠️Installation</a> &nbsp;&bull;&nbsp;
+    <a href="#-usage">🔧Usage</a> &nbsp;&bull;&nbsp;
+    <a href="#-command-line-options">💻CLI</a> &nbsp;&bull;&nbsp;
+    <a href="#-examples">💡Examples</a> &nbsp;&bull;&nbsp;
+    <a href="#-api">🤖API</a> &nbsp;&bull;&nbsp;
+    <a href="#-requirements">✅Requirements</a> &nbsp;&bull;&nbsp;
+    <a href="#-gotchas-and-limitations">🚸Gotchas</a>
+  </strong>
+</p>
+
+<div align="center">
 
-![Top language][9] ![GitHub License][3] [![PyPI - Version][4]][5]
+![Top language][9] [![GitHub License][3]][21] [![PyPI - Version][4]][5]
 [![Python Version][8]][5]
 
-|         | Status                     | Stable                    | Unstable                  |                    |
-| ------- | -------------------------- | ------------------------- | ------------------------- | ------------------ |
-| Master  | [![Build and Test][1]][2]  | [![since tagged][6]][10]  |                           | ![last commit][7]  |
-| Develop | [![Build and Test][11]][2] | [![since tagged][12]][13] | [![since tagged][15]][16] | ![last commit][14] |
+**CLI to embed (testable) snippets from your codebase into your README**
 
-CLI to embed snippets from your {python,other} codebases into your `README.md`.
+</div>
 
-## What
+---
 
-What it does: Lets you make a `EXAMPLE.md` template and include snippets from
-your (working and tested) python codebase.
+<div align="center">
 
-Turn this (`snipinator/examples/EXAMPLE.md.jinja2`):
+|                   | Status                     | Stable                    | Unstable                  |                    |
+| ----------------- | -------------------------- | ------------------------- | ------------------------- | ------------------ |
+| **[Master][17]**  | [![Build and Test][1]][2]  | [![since tagged][6]][10]  |                           | ![last commit][7]  |
+| **[Develop][18]** | [![Build and Test][11]][2] | [![since tagged][12]][13] | [![since tagged][15]][16] | ![last commit][14] |
 
-````md
+</div>
+
+## ❔ What
+
+What it does: **Snipinator** lets you take a `EXAMPLE.md` template and include
+snippets from your (working and tested) codebase.
+
+Turn this (`./snipinator/examples/EXAMPLE.md.jinja2`):
+
+<!---->
+```md
 # A README
 
 Here is a code snippet:
 
 `{{ pysnippet(path='snipinator/examples/code.py', symbol='MyClass', backtickify='py') }}`
 
-````
+Note that `code.py` has a test:
+[{{path('./snipinator/examples/code_test.py')}}](./snipinator/examples/code_test.py)
+
+```
+<!---->
 
-Into this (`snipinator/examples/EXAMPLE.generated.md`):
+Into this (`./snipinator/examples/EXAMPLE.generated.md`):
 
-``````md
+<!---->
+`````md
 <!--
 
 WARNING: This file is auto-generated by snipinator. Do not edit directly.
 SOURCE: `snipinator/examples/EXAMPLE.md.jinja2`.
 
 -->
 # A README
@@ -58,71 +98,70 @@
     self.name = name
 
   def MyClassMethod(self):
     """This is a method of MyClass"""
     print(self.name)
 ````
 
-``````
+Note that `code.py` has a test:
+[./snipinator/examples/code_test.py](./snipinator/examples/code_test.py)
 
-## Features
+`````
+<!---->
 
-- Supports anything Jinja2 supports.
-- First class support for python source code.
+## 🎇 Features
+
+- 📦✅🪄 Supports anything **[Jinja2](https://github.com/pallets/jinja)**
+  supports.
+- 🥇🐍📜 First-class support for **python** source code.
   - Can include python function signatures, docstrings, entire function source
     code, classes.
-- Supports any language.
-  - With delimiter markers, or entire inclusion of the entire file.
-- First class support for markdown output (with backtickify, decomentify).
-- Can include shell output.
-  - Supports ANSI colors with SVG output.
-
-## Getting Started
-
-### Install
-
-#### Tested on
-
-- WSL2 Ubuntu 20.04, Python 3.8.0
-- Ubuntu 20.04, Python 3.8.0, 3.9.0, 3.10.0, 3.11.0, 3.12.0, tested in GitHub
-  Actions workflow
-  ([build-and-test.yml](./.github/workflows/build-and-test.yml)).
+- ✂🌐🗂️ Snip from **any source code language**.
+  - Put delimiter markers into the code (e.g `# START_SNIPPET`,
+    `# END_TEMPLATE`), and use [snippet()](#snippet).
+- 🥇🔖📜 First-class support for **Markdown** templates (with backtickify,
+  decomentify).
+- 📦🐚🖨️ Can include **[shell](#shell) output**.
+  - Supports ANSI colors :heart: :green_heart: :blue_heart: with SVG output
+    :camera:.
+- ⚙️🔗🗃️ More robust **references/links** to local files using [path()](#path).
 
-**Requirements:**
-
-- Linux-like environment
-  - Why: Uses pexpect.spawn().
-- Python 3.8+
-  - Why: Some dev dependencies require Python 3.8+.
+## 🛠️ Installation
 
 ```bash
 # Install from pypi (https://pypi.org/project/snipinator/)
 pip install snipinator
 
 # Install from git (https://github.com/realazthat/snipinator)
-pip install git+https://github.com/realazthat/snipinator.git@v1.2.0
+pip install git+https://github.com/realazthat/snipinator.git@v1.3.0
 ```
 
-### Use
+## 🔧 Usage
 
-Example tempalte README:
-[`snipinator/examples/EXAMPLE.md.jinja2`](./snipinator/examples/EXAMPLE.md.jinja2):
+Example template README:
+([./snipinator/examples/EXAMPLE.md.jinja2](./snipinator/examples/EXAMPLE.md.jinja2)):
 
-````md
+<!---->
+```md
 # A README
 
 Here is a code snippet:
 
 `{{ pysnippet(path='snipinator/examples/code.py', symbol='MyClass', backtickify='py') }}`
 
-````
+Note that `code.py` has a test:
+[{{path('./snipinator/examples/code_test.py')}}](./snipinator/examples/code_test.py)
+
+```
+<!---->
 
 Generating the README:
 
-``````bash
+<!---->
+`````bash
 $ python -m snipinator.cli -t snipinator/examples/EXAMPLE.md.jinja2
 <!--
 
 WARNING: This file is auto-generated by snipinator. Do not edit directly.
 SOURCE: `snipinator/examples/EXAMPLE.md.jinja2`.
 
 -->
@@ -138,23 +177,77 @@
     self.name = name
 
   def MyClassMethod(self):
     """This is a method of MyClass"""
     print(self.name)
 ````
 
-``````
+Note that `code.py` has a test:
+[./snipinator/examples/code_test.py](./snipinator/examples/code_test.py)
 
-CLI usage help:
+`````
+<!---->
 
-<!----><img src="README.help.generated.svg" alt="Output of `python -m snipinator.cli --help`" /><!---->
+## 💻 Command Line Options
 
-## Available Functions in Jinja2
+<!---->
+<img src="README.help.generated.svg" alt="Output of `python -m snipinator.cli --help`" />
+<!---->
 
-````py
+## 💡 Examples
+
+- Snipinator's own `README`:
+  - Template: [./README.md.jinja2](./README.md.jinja2).
+  - Generated: [./README.md](./README.md).
+  - Generation script:
+    [./scripts/generate-readme.sh](./scripts/generate-readme.sh).
+- Example:
+  - Template:
+    [./snipinator/examples/EXAMPLE.md.jinja2](./snipinator/examples/EXAMPLE.md.jinja2).
+  - Generated:
+    [./snipinator/examples/EXAMPLE.generated.md](./snipinator/examples/EXAMPLE.generated.md).
+  - Generation script:
+    [./snipinator/examples/example.sh](./snipinator/examples/example.sh).
+- Long example of many features:
+  - Template:
+    [./snipinator/examples/LONG-EXAMPLE.md.jinja2](./snipinator/examples/LONG-EXAMPLE.md.jinja2).
+  - Generated:
+    [./snipinator/examples/LONG-EXAMPLE.generated.md](./snipinator/examples/LONG-EXAMPLE.generated.md).
+  - Generation script:
+    [./snipinator/examples/long-example.sh](./snipinator/examples/long-example.sh).
+- Projects using Snipinator:
+  - [github.com/realazthat/snipinator](https://github.com/realazthat/snipinator),
+    See
+    [snipinator/README.md.jinja2](https://github.com/realazthat/snipinator/blob/61cb88593baa099dc375cf5fd40679e4be673fc5/README.md.jinja2).
+  - [github.com/realazthat/changeguard](https://github.com/realazthat/changeguard),
+    See
+    [changeguard/README.md.jinja2](https://github.com/realazthat/changeguard/blob/87d5104b52e651bb9195a3d46dd7f050acbcb534/README.md.jinja2).
+  - [github.com/realazthat/comfy-catapult](https://github.com/realazthat/comfy-catapult),
+    See
+    [comfy-catapult/README.md.jinja2](https://github.com/realazthat/comfy-catapult/blob/ff353d48b25fa7b9c35fa11b31d5f2b3039c41c8/README.md.jinja2).
+  - [github.com/realazthat/comfylowda](https://github.com/realazthat/comfylowda),
+    See
+    [comfylowda/README.md.jinja2](https://github.com/realazthat/comfylowda/blob/e01a32c38107aa0b89ccea21c4678d193a186a78/README.md.jinja2).
+  - [github.com/realazthat/excalidraw-brute-export-cli](https://github.com/realazthat/excalidraw-brute-export-cli),
+    See
+    [excalidraw-brute-export-cli/README.md.jinja2](https://github.com/realazthat/excalidraw-brute-export-cli/blob/54a3b5b08b644e61c721ab565c576094234c5cc7/README.md.jinja2).
+
+## 🤖 API
+
+(Jinja2) Functions made available:
+
+### pysnippet
+
+Used several times in
+[./snipinator/examples/LONG-EXAMPLE.md.jinja2](./snipinator/examples/LONG-EXAMPLE.md.jinja2).
+
+Documentation:
+
+<!---->
+```py
 def pysnippet(path: str,
               symbol: Optional[str],
               *,
               escape: bool = False,
               indent: Union[str, int, None] = None,
               backtickify: Union[bool, str] = False,
               decomentify: Union[bool, Literal['nl']] = False,
@@ -179,17 +272,25 @@
         newline delimiters. Defaults to False.
       _ctx (_Context): This is used by the system and is not available as an
         argument.
 
   Returns:
       Union[str, markupsafe.Markup]: The snippet.
   """
-````
+```
+<!---->
 
-````py
+### pysignature
+
+Used several times in [./README.md.jinja2](./README.md.jinja2).
+
+Documentation:
+
+<!---->
+```py
 def pysignature(path: str,
                 symbol: str,
                 *,
                 escape: bool = False,
                 indent: Union[str, int, None] = None,
                 backtickify: Union[bool, str] = False,
                 decomentify: Union[bool, Literal['nl']] = False,
@@ -215,17 +316,25 @@
         newline delimiters. Defaults to False.
       _ctx (_Context): This is used by the system and is not available as an
         argument.
 
   Returns:
       str: The signature and docstring.
   """
-````
+```
+<!---->
 
-````py
+### rawsnippet
+
+Used several times in [./README.md.jinja2](./README.md.jinja2).
+
+Documentation:
+
+<!---->
+```py
 def rawsnippet(path: str,
                *,
                escape: bool = False,
                indent: Union[str, int, None] = None,
                backtickify: Union[bool, str] = False,
                decomentify: Union[bool, Literal['nl']] = False,
                _ctx: _Context) -> Union[str, markupsafe.Markup]:
@@ -248,29 +357,38 @@
       _ctx (_Context): This is used by the system and is not available as an
         argument.
 
   Returns:
       Union[str, markupsafe.Markup]: The snippet.
   """
 
-````
+```
+<!---->
 
-````py
+### snippet
+
+Example in
+[./snipinator/examples/LONG-EXAMPLE.md.jinja2](./README.md.jinja2).
+
+Documentation:
+
+<!---->
+```py
 def snippet(path: str,
             start: str,
             end: str,
             *,
             escape: bool = False,
             indent: Union[str, int, None] = None,
             backtickify: Union[bool, str] = False,
             decomentify: Union[bool, Literal['nl']] = False,
             _ctx: _Context) -> Union[str, markupsafe.Markup]:
   """Returns a _delimited_ snippet from a file.
 
-  Does not return the delimeters themselves.
+  Does not return the delimiters themselves.
 
   Args:
       path (str): The path to the file.
       start (str): A string that indicates the start of the snippet.
       end (str): A string that indicates the end of the snippet.
       escape (bool, optional): Should use HTML entities escaping? Defaults to
         False.
@@ -287,17 +405,25 @@
       _ctx (_Context): This is used by the system and is not available as an
         argument.
 
   Returns:
       Union[str, markupsafe.Markup]: The snippet.
   """
 
-````
+```
+<!---->
 
-````py
+### shell
+
+Used several times in [./README.md.jinja2](./README.md.jinja2).
+
+Documentation:
+
+<!---->
+```py
 def shell(args: str,
           *,
           escape: bool = False,
           indent: Union[str, int, None] = None,
           backtickify: Union[bool, str] = False,
           decomentify: Union[bool, Literal['nl']] = False,
           rich: Union[Literal['svg'], Literal['img+b64+svg'], Literal['raw'],
@@ -362,20 +488,80 @@
         the output? Defaults to True.
       _ctx (_Context): This is used by the system and is not available as an
         argument.
 
   Returns:
       Union[str, markupsafe.Markup]: Returns the output of the command.
   """
-````
+```
+<!---->
+
+### path
+
+Used several times in [./README.md.jinja2](./README.md.jinja2).
+
+Documentation:
+
+<!---->
+```py
+def path(path: str,
+         *,
+         escape: bool = False,
+         indent: Union[str, int, None] = None,
+         backtickify: Union[bool, str] = False,
+         decomentify: Union[bool, Literal['nl']] = False,
+         _ctx: _Context) -> Union[str, markupsafe.Markup]:
+  """Verifies that `path` exists, and just returns `path`.
+
+  Unfortunately, I don't know how to use this inside a link, because the
+  formatters will destroy it, and it cannot be put into a code block (as the url
+  section of a link in markdown does not allow code blocks).
+
+  Args:
+      path (str): The path to verify.
+      escape (bool, optional): Should use HTML entities escaping? Defaults to
+        False.
+      indent (Union[str, int, None], optional): Should indent? By how much, or
+        with what prefix? Defaults to None.
+      backtickify (Union[bool, str], optional): Should surround with backticks?
+        With what language? Defaults to False.
+      decomentify (Union[bool, Literal['nl']]): Assuming that you will be using
+        HTML comments around this call, setting this to true will add
+        correspondingcomments to uncomment the output. This allows you to have
+        the Jinja2 call unmolested by markdown formatters, because they will be
+        inside of a comment section. "nl" adds additional newlines after the
+        newline delimiters. Defaults to False.
+      _ctx (_Context): This is used by the system and is not available as an
+        argument.
+
+  Returns:
+      Union[str, markupsafe.Markup]: Just returns the path. If the path doesn't exist,
+        it will raise an error.
+  """
+```
+<!---->
 
 Also see Jinja2 v3
 [Template Designer Documentation](https://jinja.palletsprojects.com/en/3.1.x/templates/).
 
-## Gotchas
+## ✅ Requirements
+
+- Linux-like environment
+  - Why: Uses pexpect.spawn().
+- Python 3.8+
+  - Why: Some dev dependencies require Python 3.8+.
+
+### Tested on
+
+- WSL2 Ubuntu 20.04, Python 3.8.0
+- Ubuntu 20.04, Python 3.8.0, 3.9.0, 3.10.0, 3.11.0, 3.12.0, tested in GitHub
+  Actions workflow
+  ([build-and-test.yml](./.github/workflows/build-and-test.yml)).
+
+## 🚸 Gotchas and Limitations
 
 - **Security:** This tool is NOT designed to be used with untrusted input. It is
   designed to be used with your own codebase. Even when using your own input, be
   careful that your own code won't be doing anything that might inadvertently
   include untrusted input.
 - Be careful to escape `{{` and `}}`,
   or `{%` and `%}` or anything jinja2
@@ -395,15 +581,15 @@
   ` ````language ```My Snippet``` ```` ` and this is a method that Markdown uses
   to allow embedded backticks inside a code block.
 - Formatting: The `{{` `}}` used to
   surround the snippet calls will unfortunately be formatted by a Markdown
   formatter and make the call invalid. Workarounds:
   - **Decommentify**: Put the snippet call inside a HTML comment, then use
     `decommentify` parameter. See
-    [`snipinator/examples/LONG-EXAMPLE.md.jinja2`](./snipinator/examples/LONG-EXAMPLE.md.jinja2)
+    [./snipinator/examples/LONG-EXAMPLE.md.jinja2](./snipinator/examples/LONG-EXAMPLE.md.jinja2)
     for examples.
   - [prettier](https://prettier.io/) formatter is pretty good at leaving the
     Jinja2 calls alone, especially if you don't have any spaces. This especially
     helps for markdown "reference-style links" that have Jinja2 calls in them
     generating part of the URL, mdformat will URL encode the Jinja2 calls,
     and/or split them on spaces, which is not what we want. prettier will leave
     them alone.
@@ -420,82 +606,79 @@
   - Snipinator will optionally chmod the file for you to make it read-only.
 - Newlines: This program assumes LF newlines. I don't know if it will work for
   anything else.
 - Combining `backtickify` and `indent`: Doesn't make much sense, but if you do
   it, it will run backtickify first, then indent everything including the
   backticks.
 
-## Examples
+## 🔑 License
 
-- Snipinator's own `README` at
-  [`./README.md.jinja2`](./README.md.jinja2).
-  - Generated: [`./README.md`](./README.md).
-  - Generation script:
-    [`./scripts/generate-readme.sh`](./scripts/generate-readme.sh).
-- [`snipinator/examples/EXAMPLE.md.jinja2`](./snipinator/examples/EXAMPLE.md.jinja2).
-  - Generated:
-    [`snipinator/examples/EXAMPLE.generated.md`](./snipinator/examples/EXAMPLE.generated.md).
-  - Generation script:
-    [`./snipinator/examples/example.sh`](./snipinator/examples/example.sh).
-- [`snipinator/examples/LONG-EXAMPLE.md.jinja2`](./snipinator/examples/LONG-EXAMPLE.md.jinja2).
-  - Generated:
-    [`snipinator/examples/LONG-EXAMPLE.generated.md`](./snipinator/examples/LONG-EXAMPLE.generated.md).
-  - Generation script:
-    [`./snipinator/examples/long-example.sh`](./snipinator/examples/long-example.sh).
+This project is licensed under the MIT License - see the
+[./LICENSE.md](./LICENSE.md) file for details.
 
-## Thanks
+## 🙏 Thanks
 
 Main libraries used in Snipinator are:
 
 - Templating: [Jinja2](https://github.com/pallets/jinja).
 - Snippet inclusion: Python's AST library.
 - Colorful CLI help: [rich-argparse](https://github.com/hamdanal/rich-argparse).
 - ANSI coloring shell output:
   {[pexpect](https://pexpect.readthedocs.io/en/stable/),
   [rich](https://github.com/Textualize/rich)}.
 
-## Contributions
+## Related Projects {#thanks}
+
+- [ARMmbed/snippet](https://github.com/ARMmbed/snippet) "A Python3 tool to
+  extract code snippets from source files".
+- [SimonCropp/MarkdownSnippets](https://github.com/SimonCropp/MarkdownSnippets)
+  "Extracts snippets from code files and merges them into markdown documents".
+- [shiftkey/scribble](https://github.com/shiftkey/scribble) "Making
+  documentation for .NET projects easy and fun".
+
+## 🫡Contributions
 
 ### Development environment: Linux-like
 
 - For running `pre.sh` (Linux-like environment).
   - Requires `pyenv`, or an exact matching version of python as in
     `.python-version` (which is currently
     `3.8.0
 `).
   - `jq`, ([installation](https://jqlang.github.io/jq/)) required for
     [yq](https://github.com/kislyuk/yq), which is itself required for our
-    `README.md` generation, which uses `tomlq` (from the
+    `./README.md` generation, which uses `tomlq` (from the
     [yq](https://github.com/kislyuk/yq) package) to include version strings from
-    `pyproject.toml`.
+    `./pyproject.toml`.
   - `bash`, `grep`, `awk`, `sed` `xxd`, `git`, `xxhash` (for tests/workflows).
   - Requires nodejs (for act).
   - Requires Go (to run act).
   - docker (for act).
 
 ### Commit Process
 
 1. (Optionally) Fork the `develop` branch.
 2. Stage your files: `git add path/to/file.py`.
 3. `bash scripts/pre.sh`, this will format, lint, and test the code.
-4. `git status` check if anything changed (generated `README.md` for
-   example), if so, `git add` the changes, and go back to the previous step.
+4. `git status` check if anything changed (generated `./README.md`
+   for example), if so, `git add` the changes, and go back to the previous step.
 5. `git commit -m "..."`.
 6. Make a PR to `develop` (or push to develop if you have the rights).
 
-## Release Process
+## ⛙ Release Process
 
 These instructions are for maintainers of the project.
 
-1. In the `develop` branch, run `bash scripts/pre.sh` to ensure
+1. In the `develop` branch, run `bash ./scripts/pre.sh` to ensure
    everything is in order.
-2. In the `develop` branch, bump the version in `pyproject.toml`,
+2. In the `develop` branch, bump the version in `./pyproject.toml`,
    following semantic versioning principles. Also modify the
    `last_unstable_release` and `last_stable_release` in the
-   `[tool.changeguard-project-metadata]` table as appropriate.
+   `[tool.changeguard-project-metadata]` table as appropriate. Run
+   `bash scripts/pre.sh` to ensure everything is in order.
 3. In the `develop` branch, commit these changes with a message like
    `"Prepare release X.Y.Z"`. (See the contributions section
    [above](#commit-process)).
 4. Merge the `develop` branch into the `master` branch:
    `git checkout master && git merge develop --no-ff`.
 5. `master` branch: Tag the release: Create a git tag for the release with
    `git tag -a vX.Y.Z -m "Version X.Y.Z"`.
@@ -505,32 +688,51 @@
    `git push && git push --tags`.
 8. The `--no-ff` option adds a commit to the master branch for the merge, so
    refork the develop branch from the master branch:
    `git checkout develop && git merge master`.
 9. Push the develop branch to GitHub: `git push origin develop`.
 
 [1]:
-  https://github.com/realazthat/snipinator/actions/workflows/build-and-test.yml/badge.svg?branch=master
+  https://img.shields.io/github/actions/workflow/status/realazthat/snipinator/build-and-test.yml?branch=master&style=plastic
 [2]:
   https://github.com/realazthat/snipinator/actions/workflows/build-and-test.yml
-[3]: https://img.shields.io/github/license/realazthat/snipinator
-[4]: https://img.shields.io/pypi/v/snipinator
+[3]:
+  https://img.shields.io/github/license/realazthat/snipinator?style=plastic&color=0A1E1E
+[4]:
+  https://img.shields.io/pypi/v/snipinator?style=plastic&color=0A1E1E
 [5]: https://pypi.org/project/snipinator/
 [6]:
-  https://img.shields.io/github/commits-since/realazthat/snipinator/v1.2.0/master
-[7]: https://img.shields.io/github/last-commit/realazthat/snipinator/master
-[8]: https://img.shields.io/pypi/pyversions/snipinator
+  https://img.shields.io/github/commits-since/realazthat/snipinator/v1.3.0/master?style=plastic
+[7]:
+  https://img.shields.io/github/last-commit/realazthat/snipinator/master?style=plastic
+[8]:
+  https://img.shields.io/pypi/pyversions/snipinator?style=plastic&color=0A1E1E
 [9]:
-  https://img.shields.io/github/languages/top/realazthat/snipinator.svg?&cacheSeconds=28800
+  https://img.shields.io/github/languages/top/realazthat/snipinator.svg?&cacheSeconds=28800&style=plastic&color=0A1E1E
 [10]:
-  https://github.com/realazthat/snipinator/compare/v1.2.0...master
+  https://github.com/realazthat/snipinator/compare/v1.3.0...master
 [11]:
-  https://github.com/realazthat/snipinator/actions/workflows/build-and-test.yml/badge.svg?branch=develop
+  https://img.shields.io/github/actions/workflow/status/realazthat/snipinator/build-and-test.yml?branch=develop&style=plastic
 [12]:
-  https://img.shields.io/github/commits-since/realazthat/snipinator/v1.2.0/develop
+  https://img.shields.io/github/commits-since/realazthat/snipinator/v1.3.0/develop?style=plastic
 [13]:
-  https://github.com/realazthat/snipinator/compare/v1.2.0...develop
-[14]: https://img.shields.io/github/last-commit/realazthat/snipinator/develop
+  https://github.com/realazthat/snipinator/compare/v1.3.0...develop
+[14]:
+  https://img.shields.io/github/last-commit/realazthat/snipinator/develop?style=plastic
 [15]:
-  https://img.shields.io/github/commits-since/realazthat/snipinator/v1.2.0/develop
+  https://img.shields.io/github/commits-since/realazthat/snipinator/v1.3.0/develop?style=plastic
 [16]:
-  https://github.com/realazthat/snipinator/compare/v1.2.0...develop
+  https://github.com/realazthat/snipinator/compare/v1.3.0...develop
+[17]: https://github.com/realazthat/snipinator/tree/master
+[18]: https://github.com/realazthat/snipinator/tree/develop
+
+<!-- Logo from https://lucide.dev/icons/users -->
+
+[19]:
+  https://img.shields.io/badge/Audience-Developers-0A1E1E?style=plastic&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIyNCIgaGVpZ2h0PSIyNCIgdmlld0JveD0iMCAwIDI0IDI0IiBmaWxsPSJub25lIiBzdHJva2U9ImN1cnJlbnRDb2xvciIgc3Ryb2tlLXdpZHRoPSIyIiBzdHJva2UtbGluZWNhcD0icm91bmQiIHN0cm9rZS1saW5lam9pbj0icm91bmQiIGNsYXNzPSJsdWNpZGUgbHVjaWRlLXVzZXJzIj48cGF0aCBkPSJNMTYgMjF2LTJhNCA0IDAgMCAwLTQtNEg2YTQgNCAwIDAgMC00IDR2MiIvPjxjaXJjbGUgY3g9IjkiIGN5PSI3IiByPSI0Ii8+PHBhdGggZD0iTTIyIDIxdi0yYTQgNCAwIDAgMC0zLTMuODciLz48cGF0aCBkPSJNMTYgMy4xM2E0IDQgMCAwIDEgMCA3Ljc1Ii8+PC9zdmc+
+
+<!-- Logo from https://lucide.dev/icons/laptop-minimal -->
+
+[20]:
+  https://img.shields.io/badge/Platform-Linux-0A1E1E?style=plastic&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIyNCIgaGVpZ2h0PSIyNCIgdmlld0JveD0iMCAwIDI0IDI0IiBmaWxsPSJub25lIiBzdHJva2U9ImN1cnJlbnRDb2xvciIgc3Ryb2tlLXdpZHRoPSIyIiBzdHJva2UtbGluZWNhcD0icm91bmQiIHN0cm9rZS1saW5lam9pbj0icm91bmQiIGNsYXNzPSJsdWNpZGUgbHVjaWRlLWxhcHRvcC1taW5pbWFsIj48cmVjdCB3aWR0aD0iMTgiIGhlaWdodD0iMTIiIHg9IjMiIHk9IjQiIHJ4PSIyIiByeT0iMiIvPjxsaW5lIHgxPSIyIiB4Mj0iMjIiIHkxPSIyMCIgeTI9IjIwIi8+PC9zdmc+
+[21]: ./LICENSE.md
+[22]: ./.github/logo-exported.svg
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `snipinator-1.2.0/pyproject.toml` & `snipinator-1.3.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=64", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "snipinator"
-version = "1.2.0"
+version = "1.3.0"
 description = "Python code snippets for markdown files, e.g READMEs, from actual (testable) code."
 authors = [{name = "AYF", email = "realazthat@gmail.com"}]
 license = {file = "LICENSE.md"}
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
   "Operating System :: OS Independent",
@@ -159,11 +159,11 @@
 Documentation = "https://github.com/realazthat/snipinator"
 Repository = "https://github.com/realazthat/snipinator"
 
 [tool.setuptools]
 packages = ["snipinator"]
 
 [tool.snipinator-project-metadata]
-last_unstable_release = "1.2.0"
-last_stable_release = "1.2.0"
+last_unstable_release = "1.3.0"
+last_stable_release = "1.3.0"
 
 [tool.tomlsort]
```

### Comparing `snipinator-1.2.0/snipinator/__init__.py` & `snipinator-1.3.0/snipinator/__init__.py`

 * *Files identical despite different names*

### Comparing `snipinator-1.2.0/snipinator/cli.py` & `snipinator-1.3.0/snipinator/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -299,14 +299,21 @@
         '--force',
         action='store_true',
         default=False,
         help='Force remove the existing file at the output path, before writing'
         ' the new one; useful if the existing file might be write protected.'
         ' Defaults to False.')
     p.add_argument(
+        '--create',
+        action='store_true',
+        default=False,
+        help='Create an empty file at the destination if it does not exist.'
+        ' Useful if the file references itself via path() etc. and so therefore'
+        ' must exist during rendering. Defaults to False.')
+    p.add_argument(
         '--check',
         action='store_true',
         default=False,
         help='Check if the output file is the same as the rendered text, and'
         ' exit with a non-zero status code if it is not. Does not write the'
         ' file. Ignores options that modify the file (e.g --rm and --chmod-ro).'
         ' Useful for CI pipelines. Defaults to False.')
@@ -361,14 +368,16 @@
 
     if args.rm and args.output == '-':
       raise ValueError('Cannot use --rm with stdout')
     if args.chmod and args.output == '-':
       raise ValueError('Cannot use --chmod with stdout')
     if args.chmod_ro and args.output == '-':
       raise ValueError('Cannot use --chmod-ro with stdout')
+    if args.create and args.output == '-':
+      raise ValueError('Cannot use --create with stdout')
     if args.check and args.output == '-':
       raise ValueError('Cannot use --check with stdout')
     ############################################################################
     template_file_name: str = args.template
     template_string: str
     if template_file_name != '-':
       # If we are not dealing with stdin:
@@ -392,14 +401,21 @@
       else:
         template_buffer: bytes = sys.stdin.buffer.read()
         decode_kwargs: Dict[str, Any] = {}
         with io.StringIO(template_buffer.decode(**decode_kwargs),
                          newline=template_newline) as template_io:
           template_string = template_io.read()
     ############################################################################
+    if args.create:
+      if args.output == '-':
+        raise ValueError('Cannot use --create with stdout')
+      output_path = Path(args.output)
+      if not output_path.exists():
+        output_path.touch()
+    ############################################################################
     rendered = Snipinate(template_file_name=template_file_name,
                          template_string=template_string,
                          cwd=args.cwd,
                          template_args=args.args,
                          templates_searchpath=args.templates_searchpath,
                          warning_message=args.warning_message)
     ############################################################################
```

### Comparing `snipinator-1.2.0/snipinator/snipinate.py` & `snipinator-1.3.0/snipinator/snipinate.py`

 * *Files 1% similar despite different names*

```diff
@@ -259,15 +259,15 @@
             escape: bool = False,
             indent: Union[str, int, None] = None,
             backtickify: Union[bool, str] = False,
             decomentify: Union[bool, Literal['nl']] = False,
             _ctx: _Context) -> Union[str, markupsafe.Markup]:
   """Returns a _delimited_ snippet from a file.
 
-  Does not return the delimeters themselves.
+  Does not return the delimiters themselves.
 
   Args:
       path (str): The path to the file.
       start (str): A string that indicates the start of the snippet.
       end (str): A string that indicates the end of the snippet.
       escape (bool, optional): Should use HTML entities escaping? Defaults to
         False.
```

### Comparing `snipinator-1.2.0/snipinator/snipinate_test.py` & `snipinator-1.3.0/snipinator/snipinate_test.py`

 * *Files identical despite different names*

### Comparing `snipinator-1.2.0/snipinator.egg-info/PKG-INFO` & `snipinator-1.3.0/snipinator.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snipinator
-Version: 1.2.0
+Version: 1.3.0
 Summary: Python code snippets for markdown files, e.g READMEs, from actual (testable) code.
 Author-email: AYF <realazthat@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Azriel Fasten.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
@@ -134,47 +134,87 @@
 WARNING: This file is auto-generated by snipinator. Do not edit directly.
 SOURCE: `README.md.jinja2`.
 
 -->
 <!--
 
 
+
+
 -->
 
-# Snipinator
+# <div align="center">![Snipinator][22]</div>
+
+<div align="center">
+
+<!-- Icons from https://lucide.dev/icons/users -->
+<!-- Icons from https://lucide.dev/icons/laptop-minimal -->
+
+![**Audience:** Developers][19] ![**Platform:** Linux][20]
+
+</div>
+
+<p align="center">
+  <strong>
+    <a href="#-features">🎇Features</a> &nbsp;&bull;&nbsp;
+    <a href="#-installation">🛠️Installation</a> &nbsp;&bull;&nbsp;
+    <a href="#-usage">🔧Usage</a> &nbsp;&bull;&nbsp;
+    <a href="#-command-line-options">💻CLI</a> &nbsp;&bull;&nbsp;
+    <a href="#-examples">💡Examples</a> &nbsp;&bull;&nbsp;
+    <a href="#-api">🤖API</a> &nbsp;&bull;&nbsp;
+    <a href="#-requirements">✅Requirements</a> &nbsp;&bull;&nbsp;
+    <a href="#-gotchas-and-limitations">🚸Gotchas</a>
+  </strong>
+</p>
+
+<div align="center">
 
-![Top language][9] ![GitHub License][3] [![PyPI - Version][4]][5]
+![Top language][9] [![GitHub License][3]][21] [![PyPI - Version][4]][5]
 [![Python Version][8]][5]
 
-|         | Status                     | Stable                    | Unstable                  |                    |
-| ------- | -------------------------- | ------------------------- | ------------------------- | ------------------ |
-| Master  | [![Build and Test][1]][2]  | [![since tagged][6]][10]  |                           | ![last commit][7]  |
-| Develop | [![Build and Test][11]][2] | [![since tagged][12]][13] | [![since tagged][15]][16] | ![last commit][14] |
+**CLI to embed (testable) snippets from your codebase into your README**
 
-CLI to embed snippets from your {python,other} codebases into your `README.md`.
+</div>
 
-## What
+---
 
-What it does: Lets you make a `EXAMPLE.md` template and include snippets from
-your (working and tested) python codebase.
+<div align="center">
 
-Turn this (`snipinator/examples/EXAMPLE.md.jinja2`):
+|                   | Status                     | Stable                    | Unstable                  |                    |
+| ----------------- | -------------------------- | ------------------------- | ------------------------- | ------------------ |
+| **[Master][17]**  | [![Build and Test][1]][2]  | [![since tagged][6]][10]  |                           | ![last commit][7]  |
+| **[Develop][18]** | [![Build and Test][11]][2] | [![since tagged][12]][13] | [![since tagged][15]][16] | ![last commit][14] |
 
-````md
+</div>
+
+## ❔ What
+
+What it does: **Snipinator** lets you take a `EXAMPLE.md` template and include
+snippets from your (working and tested) codebase.
+
+Turn this (`./snipinator/examples/EXAMPLE.md.jinja2`):
+
+<!---->
+```md
 # A README
 
 Here is a code snippet:
 
 `{{ pysnippet(path='snipinator/examples/code.py', symbol='MyClass', backtickify='py') }}`
 
-````
+Note that `code.py` has a test:
+[{{path('./snipinator/examples/code_test.py')}}](./snipinator/examples/code_test.py)
+
+```
+<!---->
 
-Into this (`snipinator/examples/EXAMPLE.generated.md`):
+Into this (`./snipinator/examples/EXAMPLE.generated.md`):
 
-``````md
+<!---->
+`````md
 <!--
 
 WARNING: This file is auto-generated by snipinator. Do not edit directly.
 SOURCE: `snipinator/examples/EXAMPLE.md.jinja2`.
 
 -->
 # A README
@@ -189,71 +229,70 @@
     self.name = name
 
   def MyClassMethod(self):
     """This is a method of MyClass"""
     print(self.name)
 ````
 
-``````
+Note that `code.py` has a test:
+[./snipinator/examples/code_test.py](./snipinator/examples/code_test.py)
 
-## Features
+`````
+<!---->
 
-- Supports anything Jinja2 supports.
-- First class support for python source code.
+## 🎇 Features
+
+- 📦✅🪄 Supports anything **[Jinja2](https://github.com/pallets/jinja)**
+  supports.
+- 🥇🐍📜 First-class support for **python** source code.
   - Can include python function signatures, docstrings, entire function source
     code, classes.
-- Supports any language.
-  - With delimiter markers, or entire inclusion of the entire file.
-- First class support for markdown output (with backtickify, decomentify).
-- Can include shell output.
-  - Supports ANSI colors with SVG output.
-
-## Getting Started
-
-### Install
-
-#### Tested on
-
-- WSL2 Ubuntu 20.04, Python 3.8.0
-- Ubuntu 20.04, Python 3.8.0, 3.9.0, 3.10.0, 3.11.0, 3.12.0, tested in GitHub
-  Actions workflow
-  ([build-and-test.yml](./.github/workflows/build-and-test.yml)).
+- ✂🌐🗂️ Snip from **any source code language**.
+  - Put delimiter markers into the code (e.g `# START_SNIPPET`,
+    `# END_TEMPLATE`), and use [snippet()](#snippet).
+- 🥇🔖📜 First-class support for **Markdown** templates (with backtickify,
+  decomentify).
+- 📦🐚🖨️ Can include **[shell](#shell) output**.
+  - Supports ANSI colors :heart: :green_heart: :blue_heart: with SVG output
+    :camera:.
+- ⚙️🔗🗃️ More robust **references/links** to local files using [path()](#path).
 
-**Requirements:**
-
-- Linux-like environment
-  - Why: Uses pexpect.spawn().
-- Python 3.8+
-  - Why: Some dev dependencies require Python 3.8+.
+## 🛠️ Installation
 
 ```bash
 # Install from pypi (https://pypi.org/project/snipinator/)
 pip install snipinator
 
 # Install from git (https://github.com/realazthat/snipinator)
-pip install git+https://github.com/realazthat/snipinator.git@v1.2.0
+pip install git+https://github.com/realazthat/snipinator.git@v1.3.0
 ```
 
-### Use
+## 🔧 Usage
 
-Example tempalte README:
-[`snipinator/examples/EXAMPLE.md.jinja2`](./snipinator/examples/EXAMPLE.md.jinja2):
+Example template README:
+([./snipinator/examples/EXAMPLE.md.jinja2](./snipinator/examples/EXAMPLE.md.jinja2)):
 
-````md
+<!---->
+```md
 # A README
 
 Here is a code snippet:
 
 `{{ pysnippet(path='snipinator/examples/code.py', symbol='MyClass', backtickify='py') }}`
 
-````
+Note that `code.py` has a test:
+[{{path('./snipinator/examples/code_test.py')}}](./snipinator/examples/code_test.py)
+
+```
+<!---->
 
 Generating the README:
 
-``````bash
+<!---->
+`````bash
 $ python -m snipinator.cli -t snipinator/examples/EXAMPLE.md.jinja2
 <!--
 
 WARNING: This file is auto-generated by snipinator. Do not edit directly.
 SOURCE: `snipinator/examples/EXAMPLE.md.jinja2`.
 
 -->
@@ -269,23 +308,77 @@
     self.name = name
 
   def MyClassMethod(self):
     """This is a method of MyClass"""
     print(self.name)
 ````
 
-``````
+Note that `code.py` has a test:
+[./snipinator/examples/code_test.py](./snipinator/examples/code_test.py)
 
-CLI usage help:
+`````
+<!---->
 
-<!----><img src="README.help.generated.svg" alt="Output of `python -m snipinator.cli --help`" /><!---->
+## 💻 Command Line Options
 
-## Available Functions in Jinja2
+<!---->
+<img src="README.help.generated.svg" alt="Output of `python -m snipinator.cli --help`" />
+<!---->
 
-````py
+## 💡 Examples
+
+- Snipinator's own `README`:
+  - Template: [./README.md.jinja2](./README.md.jinja2).
+  - Generated: [./README.md](./README.md).
+  - Generation script:
+    [./scripts/generate-readme.sh](./scripts/generate-readme.sh).
+- Example:
+  - Template:
+    [./snipinator/examples/EXAMPLE.md.jinja2](./snipinator/examples/EXAMPLE.md.jinja2).
+  - Generated:
+    [./snipinator/examples/EXAMPLE.generated.md](./snipinator/examples/EXAMPLE.generated.md).
+  - Generation script:
+    [./snipinator/examples/example.sh](./snipinator/examples/example.sh).
+- Long example of many features:
+  - Template:
+    [./snipinator/examples/LONG-EXAMPLE.md.jinja2](./snipinator/examples/LONG-EXAMPLE.md.jinja2).
+  - Generated:
+    [./snipinator/examples/LONG-EXAMPLE.generated.md](./snipinator/examples/LONG-EXAMPLE.generated.md).
+  - Generation script:
+    [./snipinator/examples/long-example.sh](./snipinator/examples/long-example.sh).
+- Projects using Snipinator:
+  - [github.com/realazthat/snipinator](https://github.com/realazthat/snipinator),
+    See
+    [snipinator/README.md.jinja2](https://github.com/realazthat/snipinator/blob/61cb88593baa099dc375cf5fd40679e4be673fc5/README.md.jinja2).
+  - [github.com/realazthat/changeguard](https://github.com/realazthat/changeguard),
+    See
+    [changeguard/README.md.jinja2](https://github.com/realazthat/changeguard/blob/87d5104b52e651bb9195a3d46dd7f050acbcb534/README.md.jinja2).
+  - [github.com/realazthat/comfy-catapult](https://github.com/realazthat/comfy-catapult),
+    See
+    [comfy-catapult/README.md.jinja2](https://github.com/realazthat/comfy-catapult/blob/ff353d48b25fa7b9c35fa11b31d5f2b3039c41c8/README.md.jinja2).
+  - [github.com/realazthat/comfylowda](https://github.com/realazthat/comfylowda),
+    See
+    [comfylowda/README.md.jinja2](https://github.com/realazthat/comfylowda/blob/e01a32c38107aa0b89ccea21c4678d193a186a78/README.md.jinja2).
+  - [github.com/realazthat/excalidraw-brute-export-cli](https://github.com/realazthat/excalidraw-brute-export-cli),
+    See
+    [excalidraw-brute-export-cli/README.md.jinja2](https://github.com/realazthat/excalidraw-brute-export-cli/blob/54a3b5b08b644e61c721ab565c576094234c5cc7/README.md.jinja2).
+
+## 🤖 API
+
+(Jinja2) Functions made available:
+
+### pysnippet
+
+Used several times in
+[./snipinator/examples/LONG-EXAMPLE.md.jinja2](./snipinator/examples/LONG-EXAMPLE.md.jinja2).
+
+Documentation:
+
+<!---->
+```py
 def pysnippet(path: str,
               symbol: Optional[str],
               *,
               escape: bool = False,
               indent: Union[str, int, None] = None,
               backtickify: Union[bool, str] = False,
               decomentify: Union[bool, Literal['nl']] = False,
@@ -310,17 +403,25 @@
         newline delimiters. Defaults to False.
       _ctx (_Context): This is used by the system and is not available as an
         argument.
 
   Returns:
       Union[str, markupsafe.Markup]: The snippet.
   """
-````
+```
+<!---->
 
-````py
+### pysignature
+
+Used several times in [./README.md.jinja2](./README.md.jinja2).
+
+Documentation:
+
+<!---->
+```py
 def pysignature(path: str,
                 symbol: str,
                 *,
                 escape: bool = False,
                 indent: Union[str, int, None] = None,
                 backtickify: Union[bool, str] = False,
                 decomentify: Union[bool, Literal['nl']] = False,
@@ -346,17 +447,25 @@
         newline delimiters. Defaults to False.
       _ctx (_Context): This is used by the system and is not available as an
         argument.
 
   Returns:
       str: The signature and docstring.
   """
-````
+```
+<!---->
 
-````py
+### rawsnippet
+
+Used several times in [./README.md.jinja2](./README.md.jinja2).
+
+Documentation:
+
+<!---->
+```py
 def rawsnippet(path: str,
                *,
                escape: bool = False,
                indent: Union[str, int, None] = None,
                backtickify: Union[bool, str] = False,
                decomentify: Union[bool, Literal['nl']] = False,
                _ctx: _Context) -> Union[str, markupsafe.Markup]:
@@ -379,29 +488,38 @@
       _ctx (_Context): This is used by the system and is not available as an
         argument.
 
   Returns:
       Union[str, markupsafe.Markup]: The snippet.
   """
 
-````
+```
+<!---->
 
-````py
+### snippet
+
+Example in
+[./snipinator/examples/LONG-EXAMPLE.md.jinja2](./README.md.jinja2).
+
+Documentation:
+
+<!---->
+```py
 def snippet(path: str,
             start: str,
             end: str,
             *,
             escape: bool = False,
             indent: Union[str, int, None] = None,
             backtickify: Union[bool, str] = False,
             decomentify: Union[bool, Literal['nl']] = False,
             _ctx: _Context) -> Union[str, markupsafe.Markup]:
   """Returns a _delimited_ snippet from a file.
 
-  Does not return the delimeters themselves.
+  Does not return the delimiters themselves.
 
   Args:
       path (str): The path to the file.
       start (str): A string that indicates the start of the snippet.
       end (str): A string that indicates the end of the snippet.
       escape (bool, optional): Should use HTML entities escaping? Defaults to
         False.
@@ -418,17 +536,25 @@
       _ctx (_Context): This is used by the system and is not available as an
         argument.
 
   Returns:
       Union[str, markupsafe.Markup]: The snippet.
   """
 
-````
+```
+<!---->
 
-````py
+### shell
+
+Used several times in [./README.md.jinja2](./README.md.jinja2).
+
+Documentation:
+
+<!---->
+```py
 def shell(args: str,
           *,
           escape: bool = False,
           indent: Union[str, int, None] = None,
           backtickify: Union[bool, str] = False,
           decomentify: Union[bool, Literal['nl']] = False,
           rich: Union[Literal['svg'], Literal['img+b64+svg'], Literal['raw'],
@@ -493,20 +619,80 @@
         the output? Defaults to True.
       _ctx (_Context): This is used by the system and is not available as an
         argument.
 
   Returns:
       Union[str, markupsafe.Markup]: Returns the output of the command.
   """
-````
+```
+<!---->
+
+### path
+
+Used several times in [./README.md.jinja2](./README.md.jinja2).
+
+Documentation:
+
+<!---->
+```py
+def path(path: str,
+         *,
+         escape: bool = False,
+         indent: Union[str, int, None] = None,
+         backtickify: Union[bool, str] = False,
+         decomentify: Union[bool, Literal['nl']] = False,
+         _ctx: _Context) -> Union[str, markupsafe.Markup]:
+  """Verifies that `path` exists, and just returns `path`.
+
+  Unfortunately, I don't know how to use this inside a link, because the
+  formatters will destroy it, and it cannot be put into a code block (as the url
+  section of a link in markdown does not allow code blocks).
+
+  Args:
+      path (str): The path to verify.
+      escape (bool, optional): Should use HTML entities escaping? Defaults to
+        False.
+      indent (Union[str, int, None], optional): Should indent? By how much, or
+        with what prefix? Defaults to None.
+      backtickify (Union[bool, str], optional): Should surround with backticks?
+        With what language? Defaults to False.
+      decomentify (Union[bool, Literal['nl']]): Assuming that you will be using
+        HTML comments around this call, setting this to true will add
+        correspondingcomments to uncomment the output. This allows you to have
+        the Jinja2 call unmolested by markdown formatters, because they will be
+        inside of a comment section. "nl" adds additional newlines after the
+        newline delimiters. Defaults to False.
+      _ctx (_Context): This is used by the system and is not available as an
+        argument.
+
+  Returns:
+      Union[str, markupsafe.Markup]: Just returns the path. If the path doesn't exist,
+        it will raise an error.
+  """
+```
+<!---->
 
 Also see Jinja2 v3
 [Template Designer Documentation](https://jinja.palletsprojects.com/en/3.1.x/templates/).
 
-## Gotchas
+## ✅ Requirements
+
+- Linux-like environment
+  - Why: Uses pexpect.spawn().
+- Python 3.8+
+  - Why: Some dev dependencies require Python 3.8+.
+
+### Tested on
+
+- WSL2 Ubuntu 20.04, Python 3.8.0
+- Ubuntu 20.04, Python 3.8.0, 3.9.0, 3.10.0, 3.11.0, 3.12.0, tested in GitHub
+  Actions workflow
+  ([build-and-test.yml](./.github/workflows/build-and-test.yml)).
+
+## 🚸 Gotchas and Limitations
 
 - **Security:** This tool is NOT designed to be used with untrusted input. It is
   designed to be used with your own codebase. Even when using your own input, be
   careful that your own code won't be doing anything that might inadvertently
   include untrusted input.
 - Be careful to escape `{{` and `}}`,
   or `{%` and `%}` or anything jinja2
@@ -526,15 +712,15 @@
   ` ````language ```My Snippet``` ```` ` and this is a method that Markdown uses
   to allow embedded backticks inside a code block.
 - Formatting: The `{{` `}}` used to
   surround the snippet calls will unfortunately be formatted by a Markdown
   formatter and make the call invalid. Workarounds:
   - **Decommentify**: Put the snippet call inside a HTML comment, then use
     `decommentify` parameter. See
-    [`snipinator/examples/LONG-EXAMPLE.md.jinja2`](./snipinator/examples/LONG-EXAMPLE.md.jinja2)
+    [./snipinator/examples/LONG-EXAMPLE.md.jinja2](./snipinator/examples/LONG-EXAMPLE.md.jinja2)
     for examples.
   - [prettier](https://prettier.io/) formatter is pretty good at leaving the
     Jinja2 calls alone, especially if you don't have any spaces. This especially
     helps for markdown "reference-style links" that have Jinja2 calls in them
     generating part of the URL, mdformat will URL encode the Jinja2 calls,
     and/or split them on spaces, which is not what we want. prettier will leave
     them alone.
@@ -551,82 +737,79 @@
   - Snipinator will optionally chmod the file for you to make it read-only.
 - Newlines: This program assumes LF newlines. I don't know if it will work for
   anything else.
 - Combining `backtickify` and `indent`: Doesn't make much sense, but if you do
   it, it will run backtickify first, then indent everything including the
   backticks.
 
-## Examples
+## 🔑 License
 
-- Snipinator's own `README` at
-  [`./README.md.jinja2`](./README.md.jinja2).
-  - Generated: [`./README.md`](./README.md).
-  - Generation script:
-    [`./scripts/generate-readme.sh`](./scripts/generate-readme.sh).
-- [`snipinator/examples/EXAMPLE.md.jinja2`](./snipinator/examples/EXAMPLE.md.jinja2).
-  - Generated:
-    [`snipinator/examples/EXAMPLE.generated.md`](./snipinator/examples/EXAMPLE.generated.md).
-  - Generation script:
-    [`./snipinator/examples/example.sh`](./snipinator/examples/example.sh).
-- [`snipinator/examples/LONG-EXAMPLE.md.jinja2`](./snipinator/examples/LONG-EXAMPLE.md.jinja2).
-  - Generated:
-    [`snipinator/examples/LONG-EXAMPLE.generated.md`](./snipinator/examples/LONG-EXAMPLE.generated.md).
-  - Generation script:
-    [`./snipinator/examples/long-example.sh`](./snipinator/examples/long-example.sh).
+This project is licensed under the MIT License - see the
+[./LICENSE.md](./LICENSE.md) file for details.
 
-## Thanks
+## 🙏 Thanks
 
 Main libraries used in Snipinator are:
 
 - Templating: [Jinja2](https://github.com/pallets/jinja).
 - Snippet inclusion: Python's AST library.
 - Colorful CLI help: [rich-argparse](https://github.com/hamdanal/rich-argparse).
 - ANSI coloring shell output:
   {[pexpect](https://pexpect.readthedocs.io/en/stable/),
   [rich](https://github.com/Textualize/rich)}.
 
-## Contributions
+## Related Projects {#thanks}
+
+- [ARMmbed/snippet](https://github.com/ARMmbed/snippet) "A Python3 tool to
+  extract code snippets from source files".
+- [SimonCropp/MarkdownSnippets](https://github.com/SimonCropp/MarkdownSnippets)
+  "Extracts snippets from code files and merges them into markdown documents".
+- [shiftkey/scribble](https://github.com/shiftkey/scribble) "Making
+  documentation for .NET projects easy and fun".
+
+## 🫡Contributions
 
 ### Development environment: Linux-like
 
 - For running `pre.sh` (Linux-like environment).
   - Requires `pyenv`, or an exact matching version of python as in
     `.python-version` (which is currently
     `3.8.0
 `).
   - `jq`, ([installation](https://jqlang.github.io/jq/)) required for
     [yq](https://github.com/kislyuk/yq), which is itself required for our
-    `README.md` generation, which uses `tomlq` (from the
+    `./README.md` generation, which uses `tomlq` (from the
     [yq](https://github.com/kislyuk/yq) package) to include version strings from
-    `pyproject.toml`.
+    `./pyproject.toml`.
   - `bash`, `grep`, `awk`, `sed` `xxd`, `git`, `xxhash` (for tests/workflows).
   - Requires nodejs (for act).
   - Requires Go (to run act).
   - docker (for act).
 
 ### Commit Process
 
 1. (Optionally) Fork the `develop` branch.
 2. Stage your files: `git add path/to/file.py`.
 3. `bash scripts/pre.sh`, this will format, lint, and test the code.
-4. `git status` check if anything changed (generated `README.md` for
-   example), if so, `git add` the changes, and go back to the previous step.
+4. `git status` check if anything changed (generated `./README.md`
+   for example), if so, `git add` the changes, and go back to the previous step.
 5. `git commit -m "..."`.
 6. Make a PR to `develop` (or push to develop if you have the rights).
 
-## Release Process
+## ⛙ Release Process
 
 These instructions are for maintainers of the project.
 
-1. In the `develop` branch, run `bash scripts/pre.sh` to ensure
+1. In the `develop` branch, run `bash ./scripts/pre.sh` to ensure
    everything is in order.
-2. In the `develop` branch, bump the version in `pyproject.toml`,
+2. In the `develop` branch, bump the version in `./pyproject.toml`,
    following semantic versioning principles. Also modify the
    `last_unstable_release` and `last_stable_release` in the
-   `[tool.changeguard-project-metadata]` table as appropriate.
+   `[tool.changeguard-project-metadata]` table as appropriate. Run
+   `bash scripts/pre.sh` to ensure everything is in order.
 3. In the `develop` branch, commit these changes with a message like
    `"Prepare release X.Y.Z"`. (See the contributions section
    [above](#commit-process)).
 4. Merge the `develop` branch into the `master` branch:
    `git checkout master && git merge develop --no-ff`.
 5. `master` branch: Tag the release: Create a git tag for the release with
    `git tag -a vX.Y.Z -m "Version X.Y.Z"`.
@@ -636,32 +819,51 @@
    `git push && git push --tags`.
 8. The `--no-ff` option adds a commit to the master branch for the merge, so
    refork the develop branch from the master branch:
    `git checkout develop && git merge master`.
 9. Push the develop branch to GitHub: `git push origin develop`.
 
 [1]:
-  https://github.com/realazthat/snipinator/actions/workflows/build-and-test.yml/badge.svg?branch=master
+  https://img.shields.io/github/actions/workflow/status/realazthat/snipinator/build-and-test.yml?branch=master&style=plastic
 [2]:
   https://github.com/realazthat/snipinator/actions/workflows/build-and-test.yml
-[3]: https://img.shields.io/github/license/realazthat/snipinator
-[4]: https://img.shields.io/pypi/v/snipinator
+[3]:
+  https://img.shields.io/github/license/realazthat/snipinator?style=plastic&color=0A1E1E
+[4]:
+  https://img.shields.io/pypi/v/snipinator?style=plastic&color=0A1E1E
 [5]: https://pypi.org/project/snipinator/
 [6]:
-  https://img.shields.io/github/commits-since/realazthat/snipinator/v1.2.0/master
-[7]: https://img.shields.io/github/last-commit/realazthat/snipinator/master
-[8]: https://img.shields.io/pypi/pyversions/snipinator
+  https://img.shields.io/github/commits-since/realazthat/snipinator/v1.3.0/master?style=plastic
+[7]:
+  https://img.shields.io/github/last-commit/realazthat/snipinator/master?style=plastic
+[8]:
+  https://img.shields.io/pypi/pyversions/snipinator?style=plastic&color=0A1E1E
 [9]:
-  https://img.shields.io/github/languages/top/realazthat/snipinator.svg?&cacheSeconds=28800
+  https://img.shields.io/github/languages/top/realazthat/snipinator.svg?&cacheSeconds=28800&style=plastic&color=0A1E1E
 [10]:
-  https://github.com/realazthat/snipinator/compare/v1.2.0...master
+  https://github.com/realazthat/snipinator/compare/v1.3.0...master
 [11]:
-  https://github.com/realazthat/snipinator/actions/workflows/build-and-test.yml/badge.svg?branch=develop
+  https://img.shields.io/github/actions/workflow/status/realazthat/snipinator/build-and-test.yml?branch=develop&style=plastic
 [12]:
-  https://img.shields.io/github/commits-since/realazthat/snipinator/v1.2.0/develop
+  https://img.shields.io/github/commits-since/realazthat/snipinator/v1.3.0/develop?style=plastic
 [13]:
-  https://github.com/realazthat/snipinator/compare/v1.2.0...develop
-[14]: https://img.shields.io/github/last-commit/realazthat/snipinator/develop
+  https://github.com/realazthat/snipinator/compare/v1.3.0...develop
+[14]:
+  https://img.shields.io/github/last-commit/realazthat/snipinator/develop?style=plastic
 [15]:
-  https://img.shields.io/github/commits-since/realazthat/snipinator/v1.2.0/develop
+  https://img.shields.io/github/commits-since/realazthat/snipinator/v1.3.0/develop?style=plastic
 [16]:
-  https://github.com/realazthat/snipinator/compare/v1.2.0...develop
+  https://github.com/realazthat/snipinator/compare/v1.3.0...develop
+[17]: https://github.com/realazthat/snipinator/tree/master
+[18]: https://github.com/realazthat/snipinator/tree/develop
+
+<!-- Logo from https://lucide.dev/icons/users -->
+
+[19]:
+  https://img.shields.io/badge/Audience-Developers-0A1E1E?style=plastic&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIyNCIgaGVpZ2h0PSIyNCIgdmlld0JveD0iMCAwIDI0IDI0IiBmaWxsPSJub25lIiBzdHJva2U9ImN1cnJlbnRDb2xvciIgc3Ryb2tlLXdpZHRoPSIyIiBzdHJva2UtbGluZWNhcD0icm91bmQiIHN0cm9rZS1saW5lam9pbj0icm91bmQiIGNsYXNzPSJsdWNpZGUgbHVjaWRlLXVzZXJzIj48cGF0aCBkPSJNMTYgMjF2LTJhNCA0IDAgMCAwLTQtNEg2YTQgNCAwIDAgMC00IDR2MiIvPjxjaXJjbGUgY3g9IjkiIGN5PSI3IiByPSI0Ii8+PHBhdGggZD0iTTIyIDIxdi0yYTQgNCAwIDAgMC0zLTMuODciLz48cGF0aCBkPSJNMTYgMy4xM2E0IDQgMCAwIDEgMCA3Ljc1Ii8+PC9zdmc+
+
+<!-- Logo from https://lucide.dev/icons/laptop-minimal -->
+
+[20]:
+  https://img.shields.io/badge/Platform-Linux-0A1E1E?style=plastic&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIyNCIgaGVpZ2h0PSIyNCIgdmlld0JveD0iMCAwIDI0IDI0IiBmaWxsPSJub25lIiBzdHJva2U9ImN1cnJlbnRDb2xvciIgc3Ryb2tlLXdpZHRoPSIyIiBzdHJva2UtbGluZWNhcD0icm91bmQiIHN0cm9rZS1saW5lam9pbj0icm91bmQiIGNsYXNzPSJsdWNpZGUgbHVjaWRlLWxhcHRvcC1taW5pbWFsIj48cmVjdCB3aWR0aD0iMTgiIGhlaWdodD0iMTIiIHg9IjMiIHk9IjQiIHJ4PSIyIiByeT0iMiIvPjxsaW5lIHgxPSIyIiB4Mj0iMjIiIHkxPSIyMCIgeTI9IjIwIi8+PC9zdmc+
+[21]: ./LICENSE.md
+[22]: ./.github/logo-exported.svg
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `snipinator-1.2.0/snipinator.egg-info/requires.txt` & `snipinator-1.3.0/snipinator.egg-info/requires.txt`

 * *Files identical despite different names*

