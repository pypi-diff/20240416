# Comparing `tmp/sphinx_autobuild-2024.2.4.tar.gz` & `tmp/sphinx_autobuild-2024.4.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx_autobuild-2024.2.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "sphinx_autobuild-2024.4.13.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `sphinx_autobuild-2024.2.4.tar` & `sphinx_autobuild-2024.4.13.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0      652 2024-02-04 06:09:59.988140 sphinx_autobuild-2024.2.4/AUTHORS.rst
--rw-r--r--   0        0        0     1129 2024-02-04 06:09:59.988140 sphinx_autobuild-2024.2.4/LICENSE.rst
--rw-r--r--   0        0        0     2978 2024-02-04 06:09:59.988140 sphinx_autobuild-2024.2.4/NEWS.rst
--rw-r--r--   0        0        0     6784 2024-02-04 06:09:59.988140 sphinx_autobuild-2024.2.4/README.rst
--rw-r--r--   0        0        0      825 2024-02-04 06:09:59.988140 sphinx_autobuild-2024.2.4/noxfile.py
--rw-r--r--   0        0        0     2438 2024-02-04 06:09:59.988140 sphinx_autobuild-2024.2.4/pyproject.toml
--rw-r--r--   0        0        0      108 2024-02-04 06:09:59.988140 sphinx_autobuild-2024.2.4/sphinx_autobuild/__init__.py
--rw-r--r--   0        0        0     5628 2024-02-04 06:09:59.988140 sphinx_autobuild-2024.2.4/sphinx_autobuild/__main__.py
--rw-r--r--   0        0        0     1089 2024-02-04 06:09:59.988140 sphinx_autobuild-2024.2.4/sphinx_autobuild/_hacks.py
--rw-r--r--   0        0        0     2594 2024-02-04 06:09:59.988140 sphinx_autobuild-2024.2.4/sphinx_autobuild/build.py
--rw-r--r--   0        0        0     1009 2024-02-04 06:09:59.988140 sphinx_autobuild-2024.2.4/sphinx_autobuild/ignore.py
--rw-r--r--   0        0        0      366 2024-02-04 06:09:59.988140 sphinx_autobuild-2024.2.4/sphinx_autobuild/utils.py
--rw-r--r--   0        0        0     2089 2024-02-04 06:09:59.988140 sphinx_autobuild-2024.2.4/tests/test_ignore.py
--rw-r--r--   0        0        0     8775 1970-01-01 00:00:00.000000 sphinx_autobuild-2024.2.4/PKG-INFO
+-rw-r--r--   0        0        0      588 2024-04-13 01:31:16.332481 sphinx_autobuild-2024.4.13/AUTHORS.rst
+-rw-r--r--   0        0        0     1129 2024-04-13 01:31:16.332481 sphinx_autobuild-2024.4.13/LICENSE.rst
+-rw-r--r--   0        0        0     3204 2024-04-13 01:31:16.332481 sphinx_autobuild-2024.4.13/NEWS.rst
+-rw-r--r--   0        0        0     5595 2024-04-13 01:31:16.332481 sphinx_autobuild-2024.4.13/README.rst
+-rw-r--r--   0        0        0      825 2024-04-13 01:31:16.336481 sphinx_autobuild-2024.4.13/noxfile.py
+-rw-r--r--   0        0        0     2528 2024-04-13 01:31:16.336481 sphinx_autobuild-2024.4.13/pyproject.toml
+-rw-r--r--   0        0        0      110 2024-04-13 01:31:16.336481 sphinx_autobuild-2024.4.13/sphinx_autobuild/__init__.py
+-rw-r--r--   0        0        0     5966 2024-04-13 01:31:16.336481 sphinx_autobuild-2024.4.13/sphinx_autobuild/__main__.py
+-rw-r--r--   0        0        0     1864 2024-04-13 01:31:16.336481 sphinx_autobuild-2024.4.13/sphinx_autobuild/build.py
+-rw-r--r--   0        0        0     1051 2024-04-13 01:31:16.336481 sphinx_autobuild-2024.4.13/sphinx_autobuild/filter.py
+-rw-r--r--   0        0        0     1614 2024-04-13 01:31:16.336481 sphinx_autobuild-2024.4.13/sphinx_autobuild/middleware.py
+-rw-r--r--   0        0        0     2635 2024-04-13 01:31:16.336481 sphinx_autobuild-2024.4.13/sphinx_autobuild/server.py
+-rw-r--r--   0        0        0     1134 2024-04-13 01:31:16.336481 sphinx_autobuild-2024.4.13/sphinx_autobuild/utils.py
+-rw-r--r--   0        0        0     2131 2024-04-13 01:31:16.336481 sphinx_autobuild-2024.4.13/tests/test_ignore.py
+-rw-r--r--   0        0        0     7675 1970-01-01 00:00:00.000000 sphinx_autobuild-2024.4.13/PKG-INFO
```

### Comparing `sphinx_autobuild-2024.2.4/AUTHORS.rst` & `sphinx_autobuild-2024.4.13/AUTHORS.rst`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Project contributors
 ====================
 
-* Alex Gleason <alex@alexgleason.me>
+* Adam Turner <AA-Turner@users.noreply.github.com>
 * Anatoly Bubenkov <bubenkoff@gmail.com>
 * Andrew Lee <ajylee@gmail.com>
-* chohner <mail@chohner.com>
-* Chris Sewell <chrisj_sewell@hotmail.com>
+* Christoph Hohnerlein <mail@chohner.com>
 * Dave Dittrich <dittrich@u.washington.edu>
-* Ed Morley <edmorley@users.noreply.github.com>
 * Jonathan Stoppani <jonathan@stoppani.name>
 * Keita Kita <maoutwo@gmail.com>
 * Kristian Holsheimer <kristian.holsheimer@gmail.com>
 * Matthias Geier <Matthias.Geier@gmail.com>
 * Pradyun Gedam <pradyunsg@users.noreply.github.com>
 * Ralph Cowling <ralph.cowling@digital.cabinet-office.gov.uk>
 * Rodrigue Cloutier <rodcloutier@gmail.com>
```

### Comparing `sphinx_autobuild-2024.2.4/LICENSE.rst` & `sphinx_autobuild-2024.4.13/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `sphinx_autobuild-2024.2.4/NEWS.rst` & `sphinx_autobuild-2024.4.13/NEWS.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,21 @@
 Changelog
 =========
 
 unreleased
 ----------
 
+2024.04.13 - 2024-04-13
+-----------------------
+
+* Drop ``python-livereload``.
+* Add ``starlette`` and ``uvicorn`` as dependencies.
+* Implement hot reloading via websockets.
+* Run Sphinx rebuilds in an asynchronous executor.
+
 2024.02.04 - 2024-02-04
 -----------------------
 
 * Declare support for Python 3.9, 3.10, 3.11, and 3.12
 * Drop support for Python 3.8 and earlier
 * Allow passing relative paths to ``--ignore``
 * Support all valid ``sphinx-build`` options (except Make-mode)
```

### Comparing `sphinx_autobuild-2024.2.4/README.rst` & `sphinx_autobuild-2024.4.13/README.rst`

 * *Files 16% similar despite different names*

```diff
@@ -6,15 +6,15 @@
    :target: https://pypi.org/project/sphinx-autobuild/
    :alt: Package on PyPI
 
 .. image:: https://img.shields.io/badge/License-MIT-blue.svg
    :target: https://opensource.org/licenses/MIT
    :alt: MIT
 
-Rebuild Sphinx documentation on changes, with live-reload in the browser.
+Rebuild Sphinx documentation on changes, with hot reloading in the browser.
 
 .. image:: ./docs/_static/demo.png
    :align: center
    :alt: preview screenshot
 
 Installation
 ============
@@ -48,40 +48,29 @@
 (these get passed to sphinx-build on each build).
 It also has a few additional options,
 which can seen by running ``sphinx-autobuild --help``:
 
 .. code-block:: console
 
    $ sphinx-autobuild --help
-   usage: sphinx-autobuild [-h] [--port PORT] [--host HOST] [--re-ignore RE_IGNORE] [--ignore IGNORE] [--no-initial] [--open-browser]
-                           [--delay DELAY] [--watch DIR] [--pre-build COMMAND] [--version]
-                           sourcedir outdir [filenames [filenames ...]]
-
-   positional arguments:
-     sourcedir             source directory
-     outdir                output directory for built documentation
-     filenames             specific files to rebuild on each run (default: None)
-
-   optional arguments:
-     -h, --help            show this help message and exit
-     --port PORT           port to serve documentation on. 0 means find and use a free port (default: 8000)
-     --host HOST           hostname to serve documentation on (default: 127.0.0.1)
+   usage: sphinx-autobuild [OPTIONS] SOURCEDIR OUTPUTDIR [FILENAMES...]
+
+   ...
+
+   autobuild options:
+     --port PORT           port to serve documentation on. 0 means find and use a free port
+     --host HOST           hostname to serve documentation on
      --re-ignore RE_IGNORE
-                           regular expression for files to ignore, when watching for changes (default: [])
-     --ignore IGNORE       glob expression for files to ignore, when watching for changes (default: [])
-     --no-initial          skip the initial build (default: False)
-     --open-browser        open the browser after building documentation (default: False)
-     --delay DELAY         how long to wait before opening the browser (default: 5)
-     --watch DIR           additional directories to watch (default: [])
-     --pre-build COMMAND   additional command(s) to run prior to building the documentation (default: [])
-     --version             show program's version number and exit
-
-   sphinx's arguments:
-     The following arguments are forwarded as-is to Sphinx. Please look at `sphinx --help` for more information.
-       -b=builder, -a, -E, -d=path, -j=N, -c=path, -C, -D=setting=value, -t=tag, -A=name=value, -n, -v, -q, -Q, -w=file, -W, -T, -N, -P, --keep-going, --color
+                           regular expression for files to ignore, when watching for changes
+     --ignore IGNORE       glob expression for files to ignore, when watching for changes
+     --no-initial          skip the initial build
+     --open-browser        open the browser after building documentation
+     --delay DELAY         how long to wait before opening the browser
+     --watch DIR           additional directories to watch
+     --pre-build COMMAND   additional command(s) to run prior to building the documentation
 
 Using with Makefile
 -------------------
 
     FYI: Sphinx is planning to `move away from`_ using `Makefile`.
 
 To use sphinx-autobuild with the Makefile generated by Sphinx,
@@ -163,20 +152,16 @@
 or passing relevant ``filenames`` in addition to source and output directory in the CLI.
 
 __ https://github.com/sphinx-doc/sphinx-autobuild/issues/34
 
 Acknowledgements
 ================
 
-This project stands on the shoulders of giants like
-Sphinx_, LiveReload_ and python-livereload_,
+This project stands on the shoulders of giants,
 without whom this project would not be possible.
 
 Many thanks to everyone who has `contributed code`_ as well as
 participated in `discussions on the issue tracker`_.
 This project is better thanks to your contribution.
 
-.. _Sphinx: https://sphinx-doc.org/
-.. _LiveReload: https://livereload.com/
-.. _python-livereload: https://github.com/lepture/python-livereload
 .. _contributed code: https://github.com/sphinx-doc/sphinx-autobuild/graphs/contributors
 .. _discussions on the issue tracker: https://github.com/sphinx-doc/sphinx-autobuild/issues
```

### Comparing `sphinx_autobuild-2024.2.4/noxfile.py` & `sphinx_autobuild-2024.4.13/noxfile.py`

 * *Files identical despite different names*

### Comparing `sphinx_autobuild-2024.2.4/pyproject.toml` & `sphinx_autobuild-2024.4.13/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["flit_core>=3.7"]
 build-backend = "flit_core.buildapi"
 
 # project metadata
 [project]
 name = "sphinx-autobuild"
-description = "Rebuild Sphinx documentation on changes, with live-reload in the browser."
+description = "Rebuild Sphinx documentation on changes, with hot reloading in the browser."
 readme = "README.rst"
 urls.Changelog = "https://github.com/sphinx-doc/sphinx-autobuild/blob/main/NEWS.rst"
 urls.Documentation = "https://github.com/sphinx-doc/sphinx-autobuild#readme"
 urls.Download = "https://pypi.org/project/sphinx-autobuild/"
 urls."Issue tracker" = "https://github.com/sphinx-doc/sphinx-autobuild/issues"
 urls.Source = "https://github.com/sphinx-doc/sphinx-autobuild"
 license.text = "MIT"
@@ -39,27 +39,32 @@
     "Topic :: Software Development",
     "Topic :: Software Development :: Documentation",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Utilities",
 ]
 dependencies = [
   "sphinx",
-  "livereload",
+  "starlette>=0.35",
+  "uvicorn>=0.25",
+  "websockets>=11.0",
   "colorama",
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 docs = []
 test = [
     "pytest>=6.0",
     "pytest-cov",
 ]
 
 [[project.authors]]
+name = "Adam Turner"
+
+[[project.authors]]
 name = "Jonathan Stoppani"
 email = "jonathan@stoppani.name"
 
 [project.scripts]
 sphinx-autobuild = "sphinx_autobuild.__main__:main"
 
 [tool.flit.sdist]
```

### Comparing `sphinx_autobuild-2024.2.4/sphinx_autobuild/__main__.py` & `sphinx_autobuild-2024.4.13/sphinx_autobuild/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,89 +1,108 @@
 """Entrypoint for ``python -m sphinx_autobuild``."""
 
-from sphinx_autobuild import _hacks  # isort:skip  # noqa
-
 import argparse
 import os
 import shlex
 import sys
 
 import colorama
-from livereload import Server
+import uvicorn
 
 # This isn't public API, but there aren't many better options
 from sphinx.cmd.build import get_parser as sphinx_get_parser
+from starlette.applications import Starlette
+from starlette.middleware import Middleware
+from starlette.routing import Mount, WebSocketRoute
+from starlette.staticfiles import StaticFiles
 
 from sphinx_autobuild import __version__
 from sphinx_autobuild.build import Builder
-from sphinx_autobuild.ignore import Ignore
-from sphinx_autobuild.utils import find_free_port
+from sphinx_autobuild.filter import IgnoreFilter
+from sphinx_autobuild.middleware import JavascriptInjectorMiddleware
+from sphinx_autobuild.server import RebuildServer
+from sphinx_autobuild.utils import find_free_port, open_browser, show
 
 
 def main():
     """Actual application logic."""
     colorama.init()
 
     args, build_args = _parse_args(sys.argv[1:])
 
-    srcdir = os.path.realpath(args.sourcedir)
-    outdir = os.path.realpath(args.outdir)
-    if not os.path.exists(outdir):
-        os.makedirs(outdir)
+    src_dir = args.sourcedir
+    out_dir = args.outdir
+    if not os.path.exists(out_dir):
+        os.makedirs(out_dir)
 
+    host_name = args.host
     port_num = args.port or find_free_port()
-    server = Server()
+    url_host = f"{host_name}:{port_num}"
 
     pre_build_commands = list(map(shlex.split, args.pre_build))
+
     builder = Builder(
-        server.watcher,
         build_args,
-        host=args.host,
-        port=port_num,
+        url_host=url_host,
         pre_build_commands=pre_build_commands,
     )
 
-    ignore_handler = _get_ignore_handler(
-        args.ignore, args.re_ignore, outdir, args.warnings_file, args.doctree_dir
+    watch_dirs = [src_dir] + args.additional_watched_dirs
+    ignore_handler = IgnoreFilter(
+        [p for p in args.ignore + [out_dir, args.warnings_file, args.doctree_dir] if p],
+        args.re_ignore,
+    )
+    watcher = RebuildServer(watch_dirs, ignore_handler, change_callback=builder)
+
+    app = Starlette(
+        routes=[
+            WebSocketRoute("/websocket-reload", watcher, name="reload"),
+            Mount("/", app=StaticFiles(directory=out_dir, html=True), name="static"),
+        ],
+        middleware=[Middleware(JavascriptInjectorMiddleware, ws_url=url_host)],
+        lifespan=watcher.lifespan,
     )
-    server.watch(srcdir, builder, ignore=ignore_handler)
-    for dirpath in args.additional_watched_dirs:
-        dirpath = os.path.realpath(dirpath)
-        server.watch(dirpath, builder, ignore=ignore_handler)
-    server.watch(outdir, ignore=ignore_handler)
 
     if not args.no_initial_build:
-        builder()
+        show(context="Starting initial build")
+        builder(rebuild=False)
 
-    if args.openbrowser is True:
-        server.serve(
-            port=port_num, host=args.host, root=outdir, open_url_delay=args.delay
-        )
-    else:
-        server.serve(port=port_num, host=args.host, root=outdir)
+    if args.open_browser:
+        open_browser(url_host, args.delay)
+
+    show(context="Waiting to detect changes...")
+    try:
+        uvicorn.run(app, host=host_name, port=port_num, log_level="warning")
+    except KeyboardInterrupt:
+        show(context="Server ceasing operations. Cheerio!")
 
 
 def _parse_args(argv):
     # Parse once with the Sphinx parser to emit errors
     # and capture the ``-d`` and ``-w`` options.
     # NOTE:
     # The Sphinx parser is not considered to be public API,
     # but as this is a first-party project, we can cheat a little bit.
     sphinx_args = _get_sphinx_build_parser().parse_args(argv.copy())
-    print(f"{sphinx_args.filenames=}")
 
     # Parse a second time with just our parser
     parser = _get_parser()
     args, build_args = parser.parse_known_args(argv.copy())
 
     # Copy needed settings
-    args.sourcedir = sphinx_args.sourcedir
-    args.outdir = sphinx_args.outputdir
-    args.doctree_dir = sphinx_args.doctreedir
-    args.warnings_file = sphinx_args.warnfile
+    args.sourcedir = os.path.realpath(sphinx_args.sourcedir)
+    args.outdir = os.path.realpath(sphinx_args.outputdir)
+    if sphinx_args.doctreedir:
+        args.doctree_dir = os.path.realpath(sphinx_args.doctreedir)
+    else:
+        args.doctree_dir = None
+    if sphinx_args.warnfile:
+        args.warnings_file = os.path.realpath(sphinx_args.warnfile)
+    else:
+        args.warnings_file = None
 
     return args, build_args
 
 
 def _get_sphinx_build_parser():
     # NOTE:
     # sphinx.cmd.build.get_parser is not considered to be public API,
@@ -145,23 +164,22 @@
         dest="no_initial_build",
         action="store_true",
         default=False,
         help="skip the initial build",
     )
     group.add_argument(
         "--open-browser",
-        dest="openbrowser",
         action="store_true",
         default=False,
         help="open the browser after building documentation",
     )
     group.add_argument(
         "--delay",
         dest="delay",
-        type=int,
+        type=float,
         default=5,
         help="how long to wait before opening the browser",
     )
     group.add_argument(
         "--watch",
         action="append",
         metavar="DIR",
@@ -175,20 +193,9 @@
         metavar="COMMAND",
         default=[],
         help="additional command(s) to run prior to building the documentation",
     )
     return group
 
 
-def _get_ignore_handler(ignore, regex_based, out_dir, doctree_dir, warnings_file):
-    regular = list(map(os.path.realpath, ignore))
-    regular.append(os.path.realpath(out_dir))  # output directory
-    if doctree_dir:  # Doctrees
-        regular.append(os.path.realpath(doctree_dir))
-    if warnings_file:  # Logfile
-        regular.append(os.path.realpath(warnings_file))
-
-    return Ignore(regular, regex_based)
-
-
 if __name__ == "__main__":
     main()
```

### Comparing `sphinx_autobuild-2024.2.4/sphinx_autobuild/build.py` & `sphinx_autobuild-2024.4.13/sphinx_autobuild/build.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,44 +1,28 @@
 """Logic for interacting with sphinx-build."""
 
-import shlex
 import subprocess
 
-from colorama import Fore, Style
-
 # This isn't public API, but we want to avoid a subprocess call
 from sphinx.cmd.build import build_main
 
-
-def _log(text, *, colour):
-    print(f"{Fore.GREEN}[sphinx-autobuild] {colour}{text}{Style.RESET_ALL}")
-
-
-def show(*, context=None, command=None):
-    """Show context and command-to-be-executed, with nice formatting and colours."""
-    if context is not None:
-        _log(context, colour=Fore.CYAN)
-    if command is not None:
-        assert isinstance(command, (list, tuple))
-        msg = f"> {shlex.join(command)}"
-        _log(msg, colour=Fore.BLUE)
+from sphinx_autobuild.utils import show
 
 
 class Builder:
-    def __init__(self, watcher, sphinx_args, *, host, port, pre_build_commands):
-        self.watcher = watcher
+    def __init__(self, sphinx_args, *, url_host, pre_build_commands):
         self.sphinx_args = sphinx_args
         self.pre_build_commands = pre_build_commands
-        self.uri = f"http://{host}:{port}"
+        self.uri = f"http://{url_host}"
 
-    def __call__(self):
+    def __call__(self, *, rebuild: bool = True):
         """Generate the documentation using ``sphinx``."""
 
-        if self.watcher.filepath:
-            show(context=f"Detected change: {self.watcher.filepath}")
+        if rebuild:
+            show(context="Detected change. Rebuilding...")
 
         try:
             for command in self.pre_build_commands:
                 show(context="pre-build", command=command)
                 subprocess.run(command, check=True)
         except subprocess.CalledProcessError as e:
             print(f"Pre-build command exited with exit code: {e.returncode}")
@@ -49,21 +33,17 @@
             raise
 
         show(command=["sphinx-build"] + self.sphinx_args)
 
         # NOTE:
         # sphinx.cmd.build.build_main is not considered to be public API,
         # but as this is a first-party project, we can cheat a little bit.
-        return_code = build_main(self.sphinx_args)
-        if return_code:
+        if return_code := build_main(self.sphinx_args):
             print(f"Sphinx exited with exit code: {return_code}")
             print(
                 "The server will continue serving the build folder, but the contents "
                 "being served are no longer in sync with the documentation sources. "
                 "Please fix the cause of the error above or press Ctrl+C to stop the "
                 "server."
             )
-        # We present this information, so that the user does not need to keep track
-        # of the port being used. It is presented by livereload when starting the
-        # server, so don't present it in the initial build.
-        if self.watcher.filepath:
-            show(context=f"Serving on {self.uri}")
+        # Remind the user of the server URL for convenience.
+        show(context=f"Serving on {self.uri}")
```

### Comparing `sphinx_autobuild-2024.2.4/tests/test_ignore.py` & `sphinx_autobuild-2024.4.13/tests/test_ignore.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,72 +1,72 @@
-from sphinx_autobuild.ignore import Ignore
+from sphinx_autobuild.filter import IgnoreFilter
 
 
 def test_empty():
-    ignored = Ignore([], [])
+    ignored = IgnoreFilter([], [])
 
     assert not ignored("amazing-file.txt")
     assert not ignored("module.pyc")
     assert not ignored("one.rst")
     assert not ignored("two.rst")
     assert not ignored("one.md")
     assert not ignored("foo/random.txt")
     assert not ignored("bar/__pycache__/file.pyc")
 
 
 def test_single_regex():
-    ignored = Ignore([], [r"\.pyc$"])
+    ignored = IgnoreFilter([], [r"\.pyc$"])
 
     assert not ignored("amazing-file.txt")
     assert ignored("module.pyc")
     assert not ignored("one.rst")
     assert not ignored("two.rst")
     assert not ignored("one.md")
     assert not ignored("foo/random.txt")
     assert ignored("bar/__pycache__/file.pyc")
 
 
 def test_multiple_regex():
-    ignored = Ignore([], [r"\.md", r"one\.rst"])
+    ignored = IgnoreFilter([], [r"\.md", r"one\.rst"])
 
     assert not ignored("amazing-file.txt")
     assert not ignored("module.pyc")
     assert ignored("one.rst")
     assert not ignored("two.rst")
     assert ignored("one.md")
     assert not ignored("foo/random.txt")
     assert not ignored("bar/__pycache__/file.pyc")
 
 
 def test_single_regular():
-    ignored = Ignore(["*.pyc"], [])
+    ignored = IgnoreFilter(["*.pyc"], [])
 
     assert not ignored("amazing-file.txt")
     assert ignored("module.pyc")
     assert not ignored("one.rst")
     assert not ignored("two.rst")
     assert not ignored("one.md")
     assert not ignored("foo/random.txt")
     assert ignored("bar/__pycache__/file.pyc")
 
 
 def test_multiple_regular():
-    ignored = Ignore(["bar", "foo"], [])
+    ignored = IgnoreFilter(["bar", "foo"], [])
 
     assert not ignored("amazing-file.txt")
     assert not ignored("module.pyc")
     assert not ignored("one.md")
     assert not ignored("one.rst")
     assert not ignored("two.rst")
     assert ignored("foo/random.txt")
     assert ignored("bar/__pycache__/file.pyc")
 
 
 def test_multiple_both():
-    ignored = Ignore(["bar", "foo"], [r"\.txt", r"one\.*"])
+    ignored = IgnoreFilter(["bar", "foo"], [r"\.txt", r"one\.*"])
 
     assert ignored("amazing-file.txt")
     assert not ignored("module.pyc")
     assert ignored("one.md")
     assert ignored("one.rst")
     assert not ignored("two.rst")
     assert ignored("foo/random.txt")
```

### Comparing `sphinx_autobuild-2024.2.4/PKG-INFO` & `sphinx_autobuild-2024.4.13/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: sphinx-autobuild
-Version: 2024.2.4
-Summary: Rebuild Sphinx documentation on changes, with live-reload in the browser.
+Version: 2024.4.13
+Summary: Rebuild Sphinx documentation on changes, with hot reloading in the browser.
+Author: Adam Turner
 Author-email: Jonathan Stoppani <jonathan@stoppani.name>
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Sphinx
@@ -25,15 +26,17 @@
 Classifier: Topic :: Documentation
 Classifier: Topic :: Documentation :: Sphinx
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Documentation
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Requires-Dist: sphinx
-Requires-Dist: livereload
+Requires-Dist: starlette>=0.35
+Requires-Dist: uvicorn>=0.25
+Requires-Dist: websockets>=11.0
 Requires-Dist: colorama
 Requires-Dist: pytest>=6.0 ; extra == "test"
 Requires-Dist: pytest-cov ; extra == "test"
 Project-URL: Changelog, https://github.com/sphinx-doc/sphinx-autobuild/blob/main/NEWS.rst
 Project-URL: Documentation, https://github.com/sphinx-doc/sphinx-autobuild#readme
 Project-URL: Download, https://pypi.org/project/sphinx-autobuild/
 Project-URL: Issue tracker, https://github.com/sphinx-doc/sphinx-autobuild/issues
@@ -49,15 +52,15 @@
    :target: https://pypi.org/project/sphinx-autobuild/
    :alt: Package on PyPI
 
 .. image:: https://img.shields.io/badge/License-MIT-blue.svg
    :target: https://opensource.org/licenses/MIT
    :alt: MIT
 
-Rebuild Sphinx documentation on changes, with live-reload in the browser.
+Rebuild Sphinx documentation on changes, with hot reloading in the browser.
 
 .. image:: ./docs/_static/demo.png
    :align: center
    :alt: preview screenshot
 
 Installation
 ============
@@ -91,40 +94,29 @@
 (these get passed to sphinx-build on each build).
 It also has a few additional options,
 which can seen by running ``sphinx-autobuild --help``:
 
 .. code-block:: console
 
    $ sphinx-autobuild --help
-   usage: sphinx-autobuild [-h] [--port PORT] [--host HOST] [--re-ignore RE_IGNORE] [--ignore IGNORE] [--no-initial] [--open-browser]
-                           [--delay DELAY] [--watch DIR] [--pre-build COMMAND] [--version]
-                           sourcedir outdir [filenames [filenames ...]]
-
-   positional arguments:
-     sourcedir             source directory
-     outdir                output directory for built documentation
-     filenames             specific files to rebuild on each run (default: None)
-
-   optional arguments:
-     -h, --help            show this help message and exit
-     --port PORT           port to serve documentation on. 0 means find and use a free port (default: 8000)
-     --host HOST           hostname to serve documentation on (default: 127.0.0.1)
+   usage: sphinx-autobuild [OPTIONS] SOURCEDIR OUTPUTDIR [FILENAMES...]
+
+   ...
+
+   autobuild options:
+     --port PORT           port to serve documentation on. 0 means find and use a free port
+     --host HOST           hostname to serve documentation on
      --re-ignore RE_IGNORE
-                           regular expression for files to ignore, when watching for changes (default: [])
-     --ignore IGNORE       glob expression for files to ignore, when watching for changes (default: [])
-     --no-initial          skip the initial build (default: False)
-     --open-browser        open the browser after building documentation (default: False)
-     --delay DELAY         how long to wait before opening the browser (default: 5)
-     --watch DIR           additional directories to watch (default: [])
-     --pre-build COMMAND   additional command(s) to run prior to building the documentation (default: [])
-     --version             show program's version number and exit
-
-   sphinx's arguments:
-     The following arguments are forwarded as-is to Sphinx. Please look at `sphinx --help` for more information.
-       -b=builder, -a, -E, -d=path, -j=N, -c=path, -C, -D=setting=value, -t=tag, -A=name=value, -n, -v, -q, -Q, -w=file, -W, -T, -N, -P, --keep-going, --color
+                           regular expression for files to ignore, when watching for changes
+     --ignore IGNORE       glob expression for files to ignore, when watching for changes
+     --no-initial          skip the initial build
+     --open-browser        open the browser after building documentation
+     --delay DELAY         how long to wait before opening the browser
+     --watch DIR           additional directories to watch
+     --pre-build COMMAND   additional command(s) to run prior to building the documentation
 
 Using with Makefile
 -------------------
 
     FYI: Sphinx is planning to `move away from`_ using `Makefile`.
 
 To use sphinx-autobuild with the Makefile generated by Sphinx,
@@ -206,21 +198,17 @@
 or passing relevant ``filenames`` in addition to source and output directory in the CLI.
 
 __ https://github.com/sphinx-doc/sphinx-autobuild/issues/34
 
 Acknowledgements
 ================
 
-This project stands on the shoulders of giants like
-Sphinx_, LiveReload_ and python-livereload_,
+This project stands on the shoulders of giants,
 without whom this project would not be possible.
 
 Many thanks to everyone who has `contributed code`_ as well as
 participated in `discussions on the issue tracker`_.
 This project is better thanks to your contribution.
 
-.. _Sphinx: https://sphinx-doc.org/
-.. _LiveReload: https://livereload.com/
-.. _python-livereload: https://github.com/lepture/python-livereload
 .. _contributed code: https://github.com/sphinx-doc/sphinx-autobuild/graphs/contributors
 .. _discussions on the issue tracker: https://github.com/sphinx-doc/sphinx-autobuild/issues
```

