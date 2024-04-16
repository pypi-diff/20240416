# Comparing `tmp/jgdv-0.1.0.tar.gz` & `tmp/jgdv-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jgdv-0.1.0.tar", last modified: Mon Apr 15 15:30:44 2024, max compression
+gzip compressed data, was "jgdv-0.1.1.tar", last modified: Tue Apr 16 13:58:45 2024, max compression
```

## Comparing `jgdv-0.1.0.tar` & `jgdv-0.1.1.tar`

### file list

```diff
@@ -1,342 +1,364 @@
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-15 15:30:44.356815 jgdv-0.1.0/
--rw-r-xr--   0 john      (1000) john      (1000)     1425 2024-03-04 06:28:16.000000 jgdv-0.1.0/LICENSE
--rw-r--r--   0 john      (1000) john      (1000)     2757 2024-04-15 15:30:44.352815 jgdv-0.1.0/PKG-INFO
--rw-r-xr--   0 john      (1000) john      (1000)       99 2024-03-05 14:03:48.000000 jgdv-0.1.0/README.md
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-15 15:30:44.320815 jgdv-0.1.0/jgdv/
--rw-rw-r--   0 john      (1000) john      (1000)       76 2024-04-15 14:40:43.000000 jgdv-0.1.0/jgdv/__init__.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-15 15:30:44.320815 jgdv-0.1.0/jgdv/__tests/
--rw-rw-r--   0 john      (1000) john      (1000)       10 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/__tests/__init__.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-15 15:30:44.320815 jgdv-0.1.0/jgdv/_interfaces/
--rw-rw-r--   0 john      (1000) john      (1000)        0 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/_interfaces/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)     1154 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/_interfaces/accessors.py
--rw-rw-r--   0 john      (1000) john      (1000)     2262 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/_interfaces/cmd.py
--rw-rw-r--   0 john      (1000) john      (1000)     2762 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/_interfaces/control.py
--rw-rw-r--   0 john      (1000) john      (1000)     1367 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/_interfaces/dbm.py
--rw-rw-r--   0 john      (1000) john      (1000)     1607 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/_interfaces/decorator.py
--rw-rw-r--   0 john      (1000) john      (1000)     1013 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/_interfaces/factory.py
--rw-rw-r--   0 john      (1000) john      (1000)     2445 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/_interfaces/loader.py
--rw-rw-r--   0 john      (1000) john      (1000)     1357 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/_interfaces/overlord.py
--rw-rw-r--   0 john      (1000) john      (1000)     1004 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/_interfaces/policy.py
--rw-rw-r--   0 john      (1000) john      (1000)     2485 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/_interfaces/singletons.py
--rw-rw-r--   0 john      (1000) john      (1000)     7676 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/_interfaces/task.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-15 15:30:44.320815 jgdv-0.1.0/jgdv/_types/
--rw-rw-r--   0 john      (1000) john      (1000)       82 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/_types/__init__.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-15 15:30:44.316815 jgdv-0.1.0/jgdv/apis/
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-15 15:30:44.324816 jgdv-0.1.0/jgdv/apis/clingo/
--rw-rw-r--   0 john      (1000) john      (1000)        0 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/apis/clingo/__init__.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-15 15:30:44.324816 jgdv-0.1.0/jgdv/apis/clingo/__tests/
--rw-rw-r--   0 john      (1000) john      (1000)       10 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/apis/clingo/__tests/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)     4845 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/apis/clingo/__tests/test_clingo_solver.py
--rw-rw-r--   0 john      (1000) john      (1000)     3317 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/apis/clingo/ast.py
--rw-rw-r--   0 john      (1000) john      (1000)     5654 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/apis/clingo/clingo_solver.py
--rw-rw-r--   0 john      (1000) john      (1000)     1529 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/apis/clingo/compiler.py
--rw-rw-r--   0 john      (1000) john      (1000)     8266 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/apis/clingo/parser.py
--rw-rw-r--   0 john      (1000) john      (1000)     1581 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/apis/clingo/reporter.py
--rw-rw-r--   0 john      (1000) john      (1000)     1979 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/apis/clingo/solver.py
--rw-rw-r--   0 john      (1000) john      (1000)     4799 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/apis/clingo/trace.py
--rw-rw-r--   0 john      (1000) john      (1000)     7515 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/apis/clingo/validate.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-15 15:30:44.324816 jgdv-0.1.0/jgdv/apis/mastodon/
--rw-rw-r--   0 john      (1000) john      (1000)      448 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/apis/mastodon/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)     7386 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/apis/mastodon/actions.py
--rw-rw-r--   0 john      (1000) john      (1000)      896 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/apis/mastodon/error.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-15 15:30:44.324816 jgdv-0.1.0/jgdv/apis/selenium/
--rw-rw-r--   0 john      (1000) john      (1000)        0 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/apis/selenium/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)     2920 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/apis/selenium/selenium.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-15 15:30:44.324816 jgdv-0.1.0/jgdv/apis/sphinx/
--rw-rw-r--   0 john      (1000) john      (1000)     1540 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/apis/sphinx/directive.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-15 15:30:44.324816 jgdv-0.1.0/jgdv/cli/
--rw-rw-r--   0 john      (1000) john      (1000)       10 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/cli/__init__.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-15 15:30:44.324816 jgdv-0.1.0/jgdv/cli/__tests/
--rw-rw-r--   0 john      (1000) john      (1000)    13764 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/cli/__tests/test_flexible.py
--rw-rw-r--   0 john      (1000) john      (1000)    11442 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/cli/arg_parser.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-15 15:30:44.324816 jgdv-0.1.0/jgdv/cli/repl/
--rw-rw-r--   0 john      (1000) john      (1000)      209 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/cli/repl/__init__.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-15 15:30:44.328816 jgdv-0.1.0/jgdv/cli/repl/commands/
--rw-rw-r--   0 john      (1000) john      (1000)       23 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/cli/repl/commands/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)     5590 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/cli/repl/commands/break_cmd.py
--rw-rw-r--   0 john      (1000) john      (1000)     1660 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/cli/repl/commands/commands_info.py
--rw-rw-r--   0 john      (1000) john      (1000)     2894 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/cli/repl/commands/control.py
--rw-rw-r--   0 john      (1000) john      (1000)      937 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/cli/repl/commands/exit_cmd.py
--rw-rw-r--   0 john      (1000) john      (1000)     3323 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/cli/repl/commands/force_parser_cmd.py
--rw-rw-r--   0 john      (1000) john      (1000)     2516 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/cli/repl/commands/init_cmd.py
--rw-rw-r--   0 john      (1000) john      (1000)     4627 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/cli/repl/commands/log_cmd.py
--rw-rw-r--   0 john      (1000) john      (1000)     2994 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/cli/repl/commands/memory_cmds.py
--rw-rw-r--   0 john      (1000) john      (1000)     4600 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/cli/repl/commands/print_cmd.py
--rw-rw-r--   0 john      (1000) john      (1000)     6277 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/cli/repl/commands/report_cmd.py
--rw-rw-r--   0 john      (1000) john      (1000)     1097 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/cli/repl/commands/tutorial_cmd.py
--rw-rw-r--   0 john      (1000) john      (1000)     2835 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/cli/repl/commands/util.py
--rw-rw-r--   0 john      (1000) john      (1000)     1003 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/cli/repl/error.py
--rw-rw-r--   0 john      (1000) john      (1000)     6066 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/cli/repl/repl_commander.py
--rw-rw-r--   0 john      (1000) john      (1000)     4095 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/cli/repl/repl_dsl.py
--rw-rw-r--   0 john      (1000) john      (1000)     1469 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/cli/repl/repl_state.py
--rw-rw-r--   0 john      (1000) john      (1000)     6880 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/cli/shell.py
--rw-rw-r--   0 john      (1000) john      (1000)     3114 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/cli/speak.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-15 15:30:44.328816 jgdv-0.1.0/jgdv/debugging/
--rw-rw-r--   0 john      (1000) john      (1000)       54 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/debugging/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)     4603 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/debugging/dsl.py
--rw-rw-r--   0 john      (1000) john      (1000)     1871 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/debugging/frame_helper.py
--rw-rw-r--   0 john      (1000) john      (1000)     1861 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/debugging/human.py
--rw-rw-r--   0 john      (1000) john      (1000)     5613 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/debugging/malloc.py
--rw-rw-r--   0 john      (1000) john      (1000)     2094 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/debugging/running_debugger.py
--rw-rw-r--   0 john      (1000) john      (1000)     3599 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/debugging/timing.py
--rw-rw-r--   0 john      (1000) john      (1000)     1738 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/debugging/trace_helper.py
--rw-rw-r--   0 john      (1000) john      (1000)     1986 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/debugging/util.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-15 15:30:44.328816 jgdv-0.1.0/jgdv/decorators/
--rw-rw-r--   0 john      (1000) john      (1000)     1844 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/decorators/breakpoint.py
--rw-rw-r--   0 john      (1000) john      (1000)     1180 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/decorators/check_protocol.py
--rw-rw-r--   0 john      (1000) john      (1000)     1771 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/decorators/destruction.py
--rw-rw-r--   0 john      (1000) john      (1000)      698 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/decorators/dsl.py
--rw-rw-r--   0 john      (1000) john      (1000)    10853 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/decorators/key.py
--rw-rw-r--   0 john      (1000) john      (1000)     1176 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/decorators/logging.py
--rw-rw-r--   0 john      (1000) john      (1000)     1105 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/decorators/singletons.py
--rw-rw-r--   0 john      (1000) john      (1000)     3054 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/decorators/util.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-15 15:30:44.328816 jgdv-0.1.0/jgdv/dsl/
--rw-rw-r--   0 john      (1000) john      (1000)       10 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/dsl/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)     2472 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/dsl/consts.py
--rw-rw-r--   0 john      (1000) john      (1000)     1150 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/dsl/ctors.py
--rw-rw-r--   0 john      (1000) john      (1000)     1459 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/dsl/funcs.py
--rw-rw-r--   0 john      (1000) john      (1000)     1519 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/dsl/util.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-15 15:30:44.328816 jgdv-0.1.0/jgdv/error/
--rw-rw-r--   0 john      (1000) john      (1000)       10 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/error/__init__.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-15 15:30:44.328816 jgdv-0.1.0/jgdv/files/
--rw-rw-r--   0 john      (1000) john      (1000)       10 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/files/__init__.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-15 15:30:44.328816 jgdv-0.1.0/jgdv/files/binary/
--rw-rw-r--   0 john      (1000) john      (1000)    13689 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/files/binary/infinity.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-15 15:30:44.332816 jgdv-0.1.0/jgdv/files/bookmarks/
--rw-rw-r--   0 john      (1000) john      (1000)     2772 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/files/bookmarks/bookmark.py
--rw-rw-r--   0 john      (1000) john      (1000)     2829 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/files/bookmarks/collection.py
--rw-rw-r--   0 john      (1000) john      (1000)     3560 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/files/bookmarks/netscape.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-15 15:30:44.332816 jgdv-0.1.0/jgdv/files/epub/
--rw-rw-r--   0 john      (1000) john      (1000)       10 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/files/epub/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)      907 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/files/epub/epub.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-15 15:30:44.332816 jgdv-0.1.0/jgdv/files/gif/
--rw-rw-r--   0 john      (1000) john      (1000)       10 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/files/gif/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)     2249 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/files/gif/gif_mixin.py
--rw-rw-r--   0 john      (1000) john      (1000)     1821 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/files/gif/make_gif.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-15 15:30:44.332816 jgdv-0.1.0/jgdv/files/graph/
--rw-rw-r--   0 john      (1000) john      (1000)     2046 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/files/graph/pickles.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-15 15:30:44.332816 jgdv-0.1.0/jgdv/files/jinja/
--rw-rw-r--   0 john      (1000) john      (1000)       10 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/files/jinja/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)     3920 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/files/json.py
--rw-rw-r--   0 john      (1000) john      (1000)     1656 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/files/mem_map.py
--rw-rw-r--   0 john      (1000) john      (1000)     1723 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/files/metadata.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-15 15:30:44.332816 jgdv-0.1.0/jgdv/files/org/
--rw-rw-r--   0 john      (1000) john      (1000)       10 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/files/org/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)      668 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/files/org/base.py
--rw-rw-r--   0 john      (1000) john      (1000)     2605 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/files/org/drawer.py
--rw-rw-r--   0 john      (1000) john      (1000)     1922 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/files/org/file.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-15 15:30:44.332816 jgdv-0.1.0/jgdv/files/pdf/
--rw-rw-r--   0 john      (1000) john      (1000)       10 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/files/pdf/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)     4343 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/files/pdf/pdf.py
--rw-rw-r--   0 john      (1000) john      (1000)     1056 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/files/sha256.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-15 15:30:44.332816 jgdv-0.1.0/jgdv/files/tags/
--rw-rw-r--   0 john      (1000) john      (1000)     3361 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/files/tags/base.py
--rw-rw-r--   0 john      (1000) john      (1000)     3763 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/files/tags/graph.py
--rw-rw-r--   0 john      (1000) john      (1000)     3235 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/files/tags/index.py
--rw-rw-r--   0 john      (1000) john      (1000)     3053 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/files/tags/substitutions.py
--rw-rw-r--   0 john      (1000) john      (1000)     3718 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/files/tar.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-15 15:30:44.332816 jgdv-0.1.0/jgdv/files/tex/
--rw-rw-r--   0 john      (1000) john      (1000)      112 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/files/tex/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)     2628 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/files/tex/base.py
--rw-rw-r--   0 john      (1000) john      (1000)      986 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/files/tex/bib.py
--rw-rw-r--   0 john      (1000) john      (1000)     1358 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/files/tex/envs.py
--rw-rw-r--   0 john      (1000) john      (1000)     7234 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/files/tex/gantt.py
--rw-rw-r--   0 john      (1000) john      (1000)     7578 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/files/tex/pdf.py
--rw-rw-r--   0 john      (1000) john      (1000)     1077 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/files/tex/statements.py
--rw-rw-r--   0 john      (1000) john      (1000)     1157 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/files/tex/util.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-15 15:30:44.332816 jgdv-0.1.0/jgdv/files/timeline/
--rw-rw-r--   0 john      (1000) john      (1000)       10 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/files/timeline/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)     1479 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/files/timeline/entry.py
--rw-rw-r--   0 john      (1000) john      (1000)      896 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/files/timeline/reader.py
--rw-rw-r--   0 john      (1000) john      (1000)     3991 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/files/timeline/timeline.py
--rw-rw-r--   0 john      (1000) john      (1000)      896 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/files/timeline/writer.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-15 15:30:44.336815 jgdv-0.1.0/jgdv/files/twitter/
--rw-rw-r--   0 john      (1000) john      (1000)        0 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/files/twitter/__init__.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-15 15:30:44.336815 jgdv-0.1.0/jgdv/files/twitter/__test/
--rw-rw-r--   0 john      (1000) john      (1000)     2125 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/files/twitter/__test/component_example.json
--rw-rw-r--   0 john      (1000) john      (1000)      979 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/files/twitter/__test/test_file_processing.py
--rw-rw-r--   0 john      (1000) john      (1000)     4210 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/files/twitter/__test/tweet_example.json
--rw-rw-r--   0 john      (1000) john      (1000)     3341 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/files/twitter/__test/user_example.json
--rw-rw-r--   0 john      (1000) john      (1000)      854 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/files/twitter/base.py
--rw-rw-r--   0 john      (1000) john      (1000)     6877 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/files/twitter/mixin_passes.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-15 15:30:44.336815 jgdv-0.1.0/jgdv/files/twitter/structs/
--rw-rw-r--   0 john      (1000) john      (1000)       10 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/files/twitter/structs/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)     1576 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/files/twitter/structs/thread.py
--rw-rw-r--   0 john      (1000) john      (1000)     1744 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/files/twitter/structs/todo_list.py
--rw-rw-r--   0 john      (1000) john      (1000)     1877 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/files/twitter/structs/tweet.py
--rw-rw-r--   0 john      (1000) john      (1000)     5131 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/files/twitter/tweet_graph.py
--rw-rw-r--   0 john      (1000) john      (1000)     3202 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/files/twitter/util.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-15 15:30:44.336815 jgdv-0.1.0/jgdv/files/twitter/writers/
--rw-rw-r--   0 john      (1000) john      (1000)       10 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/files/twitter/writers/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)     4125 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/files/twitter/writers/json_component.py
--rw-rw-r--   0 john      (1000) john      (1000)     3496 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/files/twitter/writers/lazy_json_component.py
--rw-rw-r--   0 john      (1000) john      (1000)     5605 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/files/twitter/writers/thread.py
--rw-rw-r--   0 john      (1000) john      (1000)     6960 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/files/twitter/writers/tweet.py
--rw-rw-r--   0 john      (1000) john      (1000)     1601 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/files/twitter/writers/users_table.py
--rw-rw-r--   0 john      (1000) john      (1000)     1134 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/files/twitter/writers/util.py
--rw-rw-r--   0 john      (1000) john      (1000)     1487 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/files/zip.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-15 15:30:44.336815 jgdv-0.1.0/jgdv/geom/
--rw-rw-r--   0 john      (1000) john      (1000)       10 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/geom/__init__.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-15 15:30:44.336815 jgdv-0.1.0/jgdv/geom/dcel/
--rw-rw-r--   0 john      (1000) john      (1000)       10 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/geom/dcel/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)     1068 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/geom/dcel/constants.py
--rw-rw-r--   0 john      (1000) john      (1000)      918 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/geom/dcel/dcel.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-15 15:30:44.336815 jgdv-0.1.0/jgdv/geom/dcel/io/
--rw-rw-r--   0 john      (1000) john      (1000)       10 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/geom/dcel/io/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)     3368 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/geom/dcel/io/drawing.py
--rw-rw-r--   0 john      (1000) john      (1000)     6611 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/geom/dcel/io/export.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-15 15:30:44.336815 jgdv-0.1.0/jgdv/geom/dcel/mod/
--rw-rw-r--   0 john      (1000) john      (1000)       10 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/geom/dcel/mod/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)     8161 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/geom/dcel/mod/adding.py
--rw-rw-r--   0 john      (1000) john      (1000)     8846 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/geom/dcel/mod/processing.py
--rw-rw-r--   0 john      (1000) john      (1000)     4322 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/geom/dcel/mod/subtracting.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-15 15:30:44.340815 jgdv-0.1.0/jgdv/geom/dcel/structs/
--rw-rw-r--   0 john      (1000) john      (1000)       10 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/geom/dcel/structs/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)     1363 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/geom/dcel/structs/draw_settings.py
--rw-rw-r--   0 john      (1000) john      (1000)     1072 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/geom/dcel/structs/drawable.py
--rw-rw-r--   0 john      (1000) john      (1000)    26133 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/geom/dcel/structs/face.py
--rw-rw-r--   0 john      (1000) john      (1000)    36447 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/geom/dcel/structs/halfedge.py
--rw-rw-r--   0 john      (1000) john      (1000)     6413 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/geom/dcel/structs/line.py
--rw-rw-r--   0 john      (1000) john      (1000)     5372 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/geom/dcel/structs/state.py
--rw-rw-r--   0 john      (1000) john      (1000)    11203 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/geom/dcel/structs/vertex.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-15 15:30:44.340815 jgdv-0.1.0/jgdv/geom/intersection/
--rw-rw-r--   0 john      (1000) john      (1000)       10 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/geom/intersection/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)     1459 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/geom/intersection/result.py
--rw-rw-r--   0 john      (1000) john      (1000)     1965 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/geom/intersection/state.py
--rw-rw-r--   0 john      (1000) john      (1000)    13125 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/geom/intersection/sweep.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-15 15:30:44.340815 jgdv-0.1.0/jgdv/geom/math/
--rw-rw-r--   0 john      (1000) john      (1000)     4782 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/geom/math/bbox.py
--rw-rw-r--   0 john      (1000) john      (1000)     4083 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/geom/math/circles.py
--rw-rw-r--   0 john      (1000) john      (1000)     4760 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/geom/math/direction.py
--rw-rw-r--   0 john      (1000) john      (1000)     3573 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/geom/math/distance.py
--rw-rw-r--   0 john      (1000) john      (1000)     4664 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/geom/math/heightmap.py
--rw-rw-r--   0 john      (1000) john      (1000)     8233 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/geom/math/lines.py
--rw-rw-r--   0 john      (1000) john      (1000)     4585 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/geom/math/movement.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-15 15:30:44.340815 jgdv-0.1.0/jgdv/geom/voronoi/
--rw-rw-r--   0 john      (1000) john      (1000)     2993 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/geom/voronoi/beachline.py
--rw-rw-r--   0 john      (1000) john      (1000)     1232 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/geom/voronoi/breakpoint.py
--rw-rw-r--   0 john      (1000) john      (1000)     4072 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/geom/voronoi/data.py
--rw-rw-r--   0 john      (1000) john      (1000)     9379 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/geom/voronoi/drawing.py
--rw-rw-r--   0 john      (1000) john      (1000)     3019 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/geom/voronoi/events.py
--rw-rw-r--   0 john      (1000) john      (1000)     2484 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/geom/voronoi/graph.py
--rw-rw-r--   0 john      (1000) john      (1000)    12980 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/geom/voronoi/line_sweep.py
--rw-rw-r--   0 john      (1000) john      (1000)    21596 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/geom/voronoi/process.py
--rw-rw-r--   0 john      (1000) john      (1000)    21596 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/geom/voronoi/voronoi.py
--rw-rw-r--   0 john      (1000) john      (1000)     9379 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/geom/voronoi/voronoi_drawing.py
--rw-rw-r--   0 john      (1000) john      (1000)     1118 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/geom/voronoi/voronoi_io.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-15 15:30:44.340815 jgdv-0.1.0/jgdv/handlers/
--rw-rw-r--   0 john      (1000) john      (1000)       10 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/handlers/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)     2740 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/handlers/handler.py
--rw-rw-r--   0 john      (1000) john      (1000)    17278 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/handlers/handler_system.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-15 15:30:44.344815 jgdv-0.1.0/jgdv/importing/
--rw-rw-r--   0 john      (1000) john      (1000)     1808 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/importing/inspect.py
--rw-rw-r--   0 john      (1000) john      (1000)     5977 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/importing/plugin_loader.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-15 15:30:44.344815 jgdv-0.1.0/jgdv/logging/
--rw-rw-r--   0 john      (1000) john      (1000)       85 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/logging/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)     4525 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/logging/log_colour.py
--rw-rw-r--   0 john      (1000) john      (1000)     1881 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/logging/log_context.py
--rw-rw-r--   0 john      (1000) john      (1000)     3805 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/logging/stdout_capture.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-15 15:30:44.344815 jgdv-0.1.0/jgdv/math/
--rw-rw-r--   0 john      (1000) john      (1000)       23 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/math/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)     2992 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/math/colour.py
--rw-rw-r--   0 john      (1000) john      (1000)     5165 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/math/comparison.py
--rw-rw-r--   0 john      (1000) john      (1000)     5037 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/math/easings.py
--rw-rw-r--   0 john      (1000) john      (1000)     1670 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/math/matrices.py
--rw-rw-r--   0 john      (1000) john      (1000)     8413 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/math/parabola.py
--rw-rw-r--   0 john      (1000) john      (1000)     2947 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/math/quadratic.py
--rw-rw-r--   0 john      (1000) john      (1000)     1310 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/math/quantize.py
--rw-rw-r--   0 john      (1000) john      (1000)     1159 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/math/rand.py
--rw-rw-r--   0 john      (1000) john      (1000)     1412 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/math/sorting.py
--rw-rw-r--   0 john      (1000) john      (1000)    26889 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/math/umath.py
--rw-rw-r--   0 john      (1000) john      (1000)     2900 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/math/utils.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-15 15:30:44.344815 jgdv-0.1.0/jgdv/setup/
--rw-rw-r--   0 john      (1000) john      (1000)     2080 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/setup/asyncio_client.py
--rw-rw-r--   0 john      (1000) john      (1000)     2557 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/setup/asyncio_server.py
--rw-rw-r--   0 john      (1000) john      (1000)      969 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/setup/gtk.py
--rw-rw-r--   0 john      (1000) john      (1000)     3401 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/setup/hooks.py
--rw-rw-r--   0 john      (1000) john      (1000)     1189 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/setup/importing.py
--rw-rw-r--   0 john      (1000) john      (1000)     5322 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/setup/logging.py
--rw-rw-r--   0 john      (1000) john      (1000)     4284 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/setup/main.py
--rw-rw-r--   0 john      (1000) john      (1000)     1087 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/setup/pyparsing.py
--rw-rw-r--   0 john      (1000) john      (1000)     4641 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/setup/setup.py
--rw-rw-r--   0 john      (1000) john      (1000)        0 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/setup/tkinter.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-15 15:30:44.348815 jgdv-0.1.0/jgdv/spiders/
--rw-rw-r--   0 john      (1000) john      (1000)     2238 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/spiders/__init__.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-15 15:30:44.348815 jgdv-0.1.0/jgdv/spiders/__tests/
--rw-rw-r--   0 john      (1000) john      (1000)     7315 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/spiders/__tests/test_runner.py
--rw-rw-r--   0 john      (1000) john      (1000)    11644 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/spiders/__tests/test_tracker.py
--rw-rw-r--   0 john      (1000) john      (1000)     1722 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/spiders/actions.py
--rw-rw-r--   0 john      (1000) john      (1000)     5438 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/spiders/caching.py
--rw-rw-r--   0 john      (1000) john      (1000)     2645 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/spiders/crawler.py
--rw-rw-r--   0 john      (1000) john      (1000)     4602 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/spiders/middleware.py
--rw-rw-r--   0 john      (1000) john      (1000)     2650 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/spiders/mixin.py
--rw-rw-r--   0 john      (1000) john      (1000)     4830 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/spiders/pipeline.py
--rw-rw-r--   0 john      (1000) john      (1000)    11655 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/spiders/runner.py
--rw-rw-r--   0 john      (1000) john      (1000)     1854 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/spiders/spiders.py
--rw-rw-r--   0 john      (1000) john      (1000)     8686 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/spiders/tracker.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-15 15:30:44.348815 jgdv-0.1.0/jgdv/structs/
--rw-rw-r--   0 john      (1000) john      (1000)     3022 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/structs/enums.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-15 15:30:44.348815 jgdv-0.1.0/jgdv/structs/heap/
--rw-rw-r--   0 john      (1000) john      (1000)       10 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/structs/heap/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)     1520 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/structs/heap/element.py
--rw-rw-r--   0 john      (1000) john      (1000)     1645 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/structs/heap/heap.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-15 15:30:44.348815 jgdv-0.1.0/jgdv/structs/proxy/
--rw-rw-r--   0 john      (1000) john      (1000)     6094 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/structs/proxy/base.py
--rw-rw-r--   0 john      (1000) john      (1000)    12760 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/structs/proxy/iter_proxy.py
--rw-rw-r--   0 john      (1000) john      (1000)     6312 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/structs/proxy/proxy.py
--rw-rw-r--   0 john      (1000) john      (1000)     3265 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/structs/proxy/proxy_mixin.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-15 15:30:44.348815 jgdv-0.1.0/jgdv/structs/rbtree/
--rw-rw-r--   0 john      (1000) john      (1000)      378 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/structs/rbtree/__init__.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-15 15:30:44.348815 jgdv-0.1.0/jgdv/structs/rbtree/__tests/
--rw-rw-r--   0 john      (1000) john      (1000)        0 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/structs/rbtree/__tests/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)     3854 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/structs/rbtree/__tests/test_rbtree.py
--rw-rw-r--   0 john      (1000) john      (1000)     7645 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/structs/rbtree/__tests/test_rbtree_node.py
--rw-rw-r--   0 john      (1000) john      (1000)     3262 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/structs/rbtree/comparison_functions.py
--rw-rw-r--   0 john      (1000) john      (1000)     1708 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/structs/rbtree/node.py
--rw-rw-r--   0 john      (1000) john      (1000)     7171 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/structs/rbtree/operations.py
--rw-rw-r--   0 john      (1000) john      (1000)     1735 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/structs/rbtree/rb_data.py
--rw-rw-r--   0 john      (1000) john      (1000)     8673 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/structs/rbtree/rbtree.py
--rw-rw-r--   0 john      (1000) john      (1000)     5268 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/structs/rbtree/utils.py
--rw-rw-r--   0 john      (1000) john      (1000)     1259 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/structs/regex.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-15 15:30:44.348815 jgdv-0.1.0/jgdv/structs/rete/
--rw-rw-r--   0 john      (1000) john      (1000)       10 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/structs/rete/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)      896 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/structs/rete/alpha.py
--rw-rw-r--   0 john      (1000) john      (1000)      896 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/structs/rete/beta.py
--rw-rw-r--   0 john      (1000) john      (1000)      896 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/structs/rete/rete.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-15 15:30:44.352815 jgdv-0.1.0/jgdv/structs/time/
--rw-rw-r--   0 john      (1000) john      (1000)      173 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/structs/time/__init__.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-15 15:30:44.352815 jgdv-0.1.0/jgdv/structs/time/__tests/
--rw-rw-r--   0 john      (1000) john      (1000)    12896 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/structs/time/__tests/test_time.py
--rw-rw-r--   0 john      (1000) john      (1000)     1675 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/structs/time/dsl.py
--rw-rw-r--   0 john      (1000) john      (1000)     5217 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/structs/time/pattern_constructor.py
--rw-rw-r--   0 john      (1000) john      (1000)      889 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/structs/time/pattern_iterator.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-15 15:30:44.352815 jgdv-0.1.0/jgdv/structs/time/structs/
--rw-rw-r--   0 john      (1000) john      (1000)       10 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/structs/time/structs/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)     1566 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/structs/time/structs/arc.py
--rw-rw-r--   0 john      (1000) john      (1000)      896 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/structs/time/structs/base.py
--rw-rw-r--   0 john      (1000) john      (1000)     1719 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/structs/time/structs/event.py
--rw-rw-r--   0 john      (1000) john      (1000)     5558 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/structs/time/structs/pattern.py
--rw-rw-r--   0 john      (1000) john      (1000)      968 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/structs/time/structs/var.py
--rw-rw-r--   0 john      (1000) john      (1000)     2464 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/structs/time/utils.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-15 15:30:44.352815 jgdv-0.1.0/jgdv/structs/tree/
--rw-rw-r--   0 john      (1000) john      (1000)       10 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/structs/tree/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)    11147 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/structs/tree/binary_tree.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-15 15:30:44.352815 jgdv-0.1.0/jgdv/structs/trie/
--rw-rw-r--   0 john      (1000) john      (1000)       10 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/structs/trie/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)     3069 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/structs/trie/leaf.py
--rw-rw-r--   0 john      (1000) john      (1000)     6808 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/structs/trie/semantics.py
--rw-rw-r--   0 john      (1000) john      (1000)     3458 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/structs/trie/trie.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-15 15:30:44.352815 jgdv-0.1.0/jgdv/testing/
--rw-rw-r--   0 john      (1000) john      (1000)       10 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/testing/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)     1760 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/testing/testing_fixtures.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-15 15:30:44.352815 jgdv-0.1.0/jgdv/utils/
--rw-rw-r--   0 john      (1000) john      (1000)       10 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/utils/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)     1107 2024-04-15 14:39:20.000000 jgdv-0.1.0/jgdv/utils/slice.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-15 15:30:44.352815 jgdv-0.1.0/jgdv.egg-info/
--rw-r--r--   0 john      (1000) john      (1000)     2757 2024-04-15 15:30:44.000000 jgdv-0.1.0/jgdv.egg-info/PKG-INFO
--rw-rw-r--   0 john      (1000) john      (1000)     7921 2024-04-15 15:30:44.000000 jgdv-0.1.0/jgdv.egg-info/SOURCES.txt
--rw-rw-r--   0 john      (1000) john      (1000)        1 2024-04-15 15:30:44.000000 jgdv-0.1.0/jgdv.egg-info/dependency_links.txt
--rw-rw-r--   0 john      (1000) john      (1000)      131 2024-04-15 15:30:44.000000 jgdv-0.1.0/jgdv.egg-info/requires.txt
--rw-rw-r--   0 john      (1000) john      (1000)        5 2024-04-15 15:30:44.000000 jgdv-0.1.0/jgdv.egg-info/top_level.txt
--rw-rw-r--   0 john      (1000) john      (1000)     3906 2024-04-15 14:40:43.000000 jgdv-0.1.0/pyproject.toml
--rw-rw-r--   0 john      (1000) john      (1000)       38 2024-04-15 15:30:44.356815 jgdv-0.1.0/setup.cfg
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 13:58:45.257055 jgdv-0.1.1/
+-rw-r-xr--   0 john      (1000) john      (1000)     1425 2024-03-04 06:28:16.000000 jgdv-0.1.1/LICENSE
+-rw-r--r--   0 john      (1000) john      (1000)     2763 2024-04-16 13:58:45.257055 jgdv-0.1.1/PKG-INFO
+-rw-r-xr--   0 john      (1000) john      (1000)       99 2024-03-05 14:03:48.000000 jgdv-0.1.1/README.md
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 13:58:45.221055 jgdv-0.1.1/jgdv/
+-rw-rw-r--   0 john      (1000) john      (1000)      134 2024-04-16 13:58:13.000000 jgdv-0.1.1/jgdv/__init__.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 13:58:45.225055 jgdv-0.1.1/jgdv/__tests/
+-rw-rw-r--   0 john      (1000) john      (1000)       10 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/__tests/__init__.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 13:58:45.225055 jgdv-0.1.1/jgdv/_interfaces/
+-rw-rw-r--   0 john      (1000) john      (1000)        0 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/_interfaces/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1154 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/_interfaces/accessors.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1603 2024-04-16 13:57:51.000000 jgdv-0.1.1/jgdv/_interfaces/decorator.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1013 2024-04-16 13:57:51.000000 jgdv-0.1.1/jgdv/_interfaces/factory.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1611 2024-04-16 13:57:51.000000 jgdv-0.1.1/jgdv/_interfaces/loader.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1004 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/_interfaces/policy.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2485 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/_interfaces/singletons.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 13:58:45.225055 jgdv-0.1.1/jgdv/_types/
+-rw-rw-r--   0 john      (1000) john      (1000)       10 2024-04-16 13:57:51.000000 jgdv-0.1.1/jgdv/_types/__init__.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 13:58:45.217055 jgdv-0.1.1/jgdv/apis/
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 13:58:45.225055 jgdv-0.1.1/jgdv/apis/clingo/
+-rw-rw-r--   0 john      (1000) john      (1000)        0 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/apis/clingo/__init__.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 13:58:45.225055 jgdv-0.1.1/jgdv/apis/clingo/__tests/
+-rw-rw-r--   0 john      (1000) john      (1000)       10 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/apis/clingo/__tests/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)     4845 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/apis/clingo/__tests/test_clingo_solver.py
+-rw-rw-r--   0 john      (1000) john      (1000)     3317 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/apis/clingo/ast.py
+-rw-rw-r--   0 john      (1000) john      (1000)     5648 2024-04-16 13:57:51.000000 jgdv-0.1.1/jgdv/apis/clingo/clingo_solver.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1521 2024-04-16 13:57:51.000000 jgdv-0.1.1/jgdv/apis/clingo/compiler.py
+-rw-rw-r--   0 john      (1000) john      (1000)     8264 2024-04-16 13:57:51.000000 jgdv-0.1.1/jgdv/apis/clingo/parser.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1579 2024-04-16 13:57:51.000000 jgdv-0.1.1/jgdv/apis/clingo/reporter.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1976 2024-04-16 13:57:51.000000 jgdv-0.1.1/jgdv/apis/clingo/solver.py
+-rw-rw-r--   0 john      (1000) john      (1000)     4795 2024-04-16 13:57:51.000000 jgdv-0.1.1/jgdv/apis/clingo/trace.py
+-rw-rw-r--   0 john      (1000) john      (1000)     7513 2024-04-16 13:57:51.000000 jgdv-0.1.1/jgdv/apis/clingo/validate.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 13:58:45.225055 jgdv-0.1.1/jgdv/apis/mastodon/
+-rw-rw-r--   0 john      (1000) john      (1000)      448 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/apis/mastodon/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)     7368 2024-04-16 13:57:51.000000 jgdv-0.1.1/jgdv/apis/mastodon/actions.py
+-rw-rw-r--   0 john      (1000) john      (1000)      896 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/apis/mastodon/error.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 13:58:45.225055 jgdv-0.1.1/jgdv/apis/selenium/
+-rw-rw-r--   0 john      (1000) john      (1000)        0 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/apis/selenium/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2717 2024-04-16 13:57:51.000000 jgdv-0.1.1/jgdv/apis/selenium/selenium.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 13:58:45.225055 jgdv-0.1.1/jgdv/apis/sphinx/
+-rw-rw-r--   0 john      (1000) john      (1000)     1540 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/apis/sphinx/directive.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 13:58:45.225055 jgdv-0.1.1/jgdv/cli/
+-rw-rw-r--   0 john      (1000) john      (1000)       10 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/cli/__init__.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 13:58:45.225055 jgdv-0.1.1/jgdv/cli/__tests/
+-rw-rw-r--   0 john      (1000) john      (1000)    13496 2024-04-16 13:57:51.000000 jgdv-0.1.1/jgdv/cli/__tests/test_flexible.py
+-rw-rw-r--   0 john      (1000) john      (1000)    11350 2024-04-16 13:57:51.000000 jgdv-0.1.1/jgdv/cli/arg_parser.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 13:58:45.229055 jgdv-0.1.1/jgdv/cli/repl/
+-rw-rw-r--   0 john      (1000) john      (1000)      207 2024-04-16 13:57:51.000000 jgdv-0.1.1/jgdv/cli/repl/__init__.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 13:58:45.229055 jgdv-0.1.1/jgdv/cli/repl/commands/
+-rw-rw-r--   0 john      (1000) john      (1000)       23 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/cli/repl/commands/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)     5368 2024-04-16 13:57:51.000000 jgdv-0.1.1/jgdv/cli/repl/commands/break_cmd.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1304 2024-04-16 13:57:51.000000 jgdv-0.1.1/jgdv/cli/repl/commands/commands_info.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2878 2024-04-16 13:57:51.000000 jgdv-0.1.1/jgdv/cli/repl/commands/control.py
+-rw-rw-r--   0 john      (1000) john      (1000)      827 2024-04-16 13:57:51.000000 jgdv-0.1.1/jgdv/cli/repl/commands/exit_cmd.py
+-rw-rw-r--   0 john      (1000) john      (1000)     3029 2024-04-16 13:57:51.000000 jgdv-0.1.1/jgdv/cli/repl/commands/force_parser_cmd.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1984 2024-04-16 13:57:51.000000 jgdv-0.1.1/jgdv/cli/repl/commands/init_cmd.py
+-rw-rw-r--   0 john      (1000) john      (1000)     4393 2024-04-16 13:57:51.000000 jgdv-0.1.1/jgdv/cli/repl/commands/log_cmd.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2570 2024-04-16 13:57:51.000000 jgdv-0.1.1/jgdv/cli/repl/commands/memory_cmds.py
+-rw-rw-r--   0 john      (1000) john      (1000)     4401 2024-04-16 13:57:51.000000 jgdv-0.1.1/jgdv/cli/repl/commands/print_cmd.py
+-rw-rw-r--   0 john      (1000) john      (1000)     6044 2024-04-16 13:57:51.000000 jgdv-0.1.1/jgdv/cli/repl/commands/report_cmd.py
+-rw-rw-r--   0 john      (1000) john      (1000)      986 2024-04-16 13:57:51.000000 jgdv-0.1.1/jgdv/cli/repl/commands/tutorial_cmd.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2774 2024-04-16 13:57:51.000000 jgdv-0.1.1/jgdv/cli/repl/commands/util.py
+-rw-rw-r--   0 john      (1000) john      (1000)     6042 2024-04-16 13:57:51.000000 jgdv-0.1.1/jgdv/cli/repl/repl_commander.py
+-rw-rw-r--   0 john      (1000) john      (1000)     3959 2024-04-16 13:57:51.000000 jgdv-0.1.1/jgdv/cli/repl/repl_dsl.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1469 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/cli/repl/repl_state.py
+-rw-rw-r--   0 john      (1000) john      (1000)     6745 2024-04-16 13:57:51.000000 jgdv-0.1.1/jgdv/cli/shell.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2979 2024-04-16 13:57:51.000000 jgdv-0.1.1/jgdv/cli/speak.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 13:58:45.229055 jgdv-0.1.1/jgdv/debugging/
+-rw-rw-r--   0 john      (1000) john      (1000)       54 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/debugging/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)     4923 2024-04-16 13:57:51.000000 jgdv-0.1.1/jgdv/debugging/dsl.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1871 2024-04-15 21:52:45.000000 jgdv-0.1.1/jgdv/debugging/frame_helper.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1861 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/debugging/human.py
+-rw-rw-r--   0 john      (1000) john      (1000)     5609 2024-04-16 13:57:51.000000 jgdv-0.1.1/jgdv/debugging/malloc.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2092 2024-04-16 13:57:51.000000 jgdv-0.1.1/jgdv/debugging/running_debugger.py
+-rw-rw-r--   0 john      (1000) john      (1000)     3758 2024-04-16 13:57:51.000000 jgdv-0.1.1/jgdv/debugging/timing.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1738 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/debugging/trace_helper.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1954 2024-04-16 13:57:51.000000 jgdv-0.1.1/jgdv/debugging/util.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 13:58:45.229055 jgdv-0.1.1/jgdv/decorators/
+-rw-rw-r--   0 john      (1000) john      (1000)     3752 2024-04-16 13:57:51.000000 jgdv-0.1.1/jgdv/decorators/base.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1838 2024-04-16 13:57:51.000000 jgdv-0.1.1/jgdv/decorators/breakpoint.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1180 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/decorators/check_protocol.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1844 2024-04-16 13:57:51.000000 jgdv-0.1.1/jgdv/decorators/destruction.py
+-rw-rw-r--   0 john      (1000) john      (1000)      694 2024-04-16 13:57:51.000000 jgdv-0.1.1/jgdv/decorators/dsl.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1170 2024-04-16 13:57:51.000000 jgdv-0.1.1/jgdv/decorators/logging.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2926 2024-04-16 13:57:51.000000 jgdv-0.1.1/jgdv/decorators/util.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 13:58:45.233055 jgdv-0.1.1/jgdv/dsl/
+-rw-rw-r--   0 john      (1000) john      (1000)       10 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/dsl/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2472 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/dsl/consts.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1150 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/dsl/ctors.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1459 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/dsl/funcs.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1519 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/dsl/util.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 13:58:45.233055 jgdv-0.1.1/jgdv/enums/
+-rw-rw-r--   0 john      (1000) john      (1000)        0 2024-04-16 13:57:51.000000 jgdv-0.1.1/jgdv/enums/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1272 2024-04-16 13:57:51.000000 jgdv-0.1.1/jgdv/enums/location_meta.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1349 2024-04-16 13:57:51.000000 jgdv-0.1.1/jgdv/enums/loop_control.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1137 2024-04-16 13:57:51.000000 jgdv-0.1.1/jgdv/enums/task_response.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1565 2024-04-16 13:57:51.000000 jgdv-0.1.1/jgdv/enums/task_state.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 13:58:45.233055 jgdv-0.1.1/jgdv/error/
+-rw-rw-r--   0 john      (1000) john      (1000)       10 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/error/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)      997 2024-04-16 13:57:51.000000 jgdv-0.1.1/jgdv/error/repl.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 13:58:45.233055 jgdv-0.1.1/jgdv/files/
+-rw-rw-r--   0 john      (1000) john      (1000)       10 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/files/__init__.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 13:58:45.233055 jgdv-0.1.1/jgdv/files/binary/
+-rw-rw-r--   0 john      (1000) john      (1000)    13689 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/files/binary/infinity.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 13:58:45.233055 jgdv-0.1.1/jgdv/files/bookmarks/
+-rw-rw-r--   0 john      (1000) john      (1000)     2772 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/files/bookmarks/bookmark.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2829 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/files/bookmarks/collection.py
+-rw-rw-r--   0 john      (1000) john      (1000)     3490 2024-04-16 13:57:51.000000 jgdv-0.1.1/jgdv/files/bookmarks/netscape.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 13:58:45.233055 jgdv-0.1.1/jgdv/files/epub/
+-rw-rw-r--   0 john      (1000) john      (1000)       10 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/files/epub/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)      907 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/files/epub/epub.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 13:58:45.233055 jgdv-0.1.1/jgdv/files/gif/
+-rw-rw-r--   0 john      (1000) john      (1000)       10 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/files/gif/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2249 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/files/gif/gif_mixin.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1821 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/files/gif/make_gif.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 13:58:45.233055 jgdv-0.1.1/jgdv/files/graph/
+-rw-rw-r--   0 john      (1000) john      (1000)     2046 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/files/graph/pickles.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 13:58:45.233055 jgdv-0.1.1/jgdv/files/jinja/
+-rw-rw-r--   0 john      (1000) john      (1000)       10 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/files/jinja/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)     3743 2024-04-16 13:57:51.000000 jgdv-0.1.1/jgdv/files/json.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1654 2024-04-16 13:57:51.000000 jgdv-0.1.1/jgdv/files/mem_map.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1723 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/files/metadata.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 13:58:45.233055 jgdv-0.1.1/jgdv/files/org/
+-rw-rw-r--   0 john      (1000) john      (1000)       10 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/files/org/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)      668 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/files/org/base.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2603 2024-04-16 13:57:51.000000 jgdv-0.1.1/jgdv/files/org/drawer.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1918 2024-04-16 13:57:51.000000 jgdv-0.1.1/jgdv/files/org/file.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 13:58:45.233055 jgdv-0.1.1/jgdv/files/pdf/
+-rw-rw-r--   0 john      (1000) john      (1000)       10 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/files/pdf/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)     4343 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/files/pdf/pdf.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1056 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/files/sha256.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 13:58:45.237055 jgdv-0.1.1/jgdv/files/tags/
+-rw-rw-r--   0 john      (1000) john      (1000)     3361 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/files/tags/base.py
+-rw-rw-r--   0 john      (1000) john      (1000)     3657 2024-04-16 13:57:51.000000 jgdv-0.1.1/jgdv/files/tags/graph.py
+-rw-rw-r--   0 john      (1000) john      (1000)     3233 2024-04-16 13:57:51.000000 jgdv-0.1.1/jgdv/files/tags/index.py
+-rw-rw-r--   0 john      (1000) john      (1000)     3051 2024-04-16 13:57:51.000000 jgdv-0.1.1/jgdv/files/tags/substitutions.py
+-rw-rw-r--   0 john      (1000) john      (1000)     3507 2024-04-16 13:57:51.000000 jgdv-0.1.1/jgdv/files/tar.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 13:58:45.237055 jgdv-0.1.1/jgdv/files/tex/
+-rw-rw-r--   0 john      (1000) john      (1000)      112 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/files/tex/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2628 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/files/tex/base.py
+-rw-rw-r--   0 john      (1000) john      (1000)      984 2024-04-16 13:57:51.000000 jgdv-0.1.1/jgdv/files/tex/bib.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1356 2024-04-16 13:57:51.000000 jgdv-0.1.1/jgdv/files/tex/envs.py
+-rw-rw-r--   0 john      (1000) john      (1000)     7114 2024-04-16 13:57:51.000000 jgdv-0.1.1/jgdv/files/tex/gantt.py
+-rw-rw-r--   0 john      (1000) john      (1000)     7439 2024-04-16 13:57:51.000000 jgdv-0.1.1/jgdv/files/tex/pdf.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1075 2024-04-16 13:57:51.000000 jgdv-0.1.1/jgdv/files/tex/statements.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1157 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/files/tex/util.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 13:58:45.237055 jgdv-0.1.1/jgdv/files/timeline/
+-rw-rw-r--   0 john      (1000) john      (1000)       10 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/files/timeline/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1479 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/files/timeline/entry.py
+-rw-rw-r--   0 john      (1000) john      (1000)      896 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/files/timeline/reader.py
+-rw-rw-r--   0 john      (1000) john      (1000)     3991 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/files/timeline/timeline.py
+-rw-rw-r--   0 john      (1000) john      (1000)      896 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/files/timeline/writer.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 13:58:45.237055 jgdv-0.1.1/jgdv/files/twitter/
+-rw-rw-r--   0 john      (1000) john      (1000)        0 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/files/twitter/__init__.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 13:58:45.237055 jgdv-0.1.1/jgdv/files/twitter/__test/
+-rw-rw-r--   0 john      (1000) john      (1000)     2125 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/files/twitter/__test/component_example.json
+-rw-rw-r--   0 john      (1000) john      (1000)      979 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/files/twitter/__test/test_file_processing.py
+-rw-rw-r--   0 john      (1000) john      (1000)     4210 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/files/twitter/__test/tweet_example.json
+-rw-rw-r--   0 john      (1000) john      (1000)     3341 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/files/twitter/__test/user_example.json
+-rw-rw-r--   0 john      (1000) john      (1000)      854 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/files/twitter/base.py
+-rw-rw-r--   0 john      (1000) john      (1000)     6516 2024-04-16 13:57:51.000000 jgdv-0.1.1/jgdv/files/twitter/mixin_passes.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 13:58:45.237055 jgdv-0.1.1/jgdv/files/twitter/structs/
+-rw-rw-r--   0 john      (1000) john      (1000)       10 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/files/twitter/structs/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1576 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/files/twitter/structs/thread.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1744 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/files/twitter/structs/todo_list.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1877 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/files/twitter/structs/tweet.py
+-rw-rw-r--   0 john      (1000) john      (1000)     5131 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/files/twitter/tweet_graph.py
+-rw-rw-r--   0 john      (1000) john      (1000)     3202 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/files/twitter/util.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 13:58:45.237055 jgdv-0.1.1/jgdv/files/twitter/writers/
+-rw-rw-r--   0 john      (1000) john      (1000)       10 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/files/twitter/writers/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)     4125 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/files/twitter/writers/json_component.py
+-rw-rw-r--   0 john      (1000) john      (1000)     3496 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/files/twitter/writers/lazy_json_component.py
+-rw-rw-r--   0 john      (1000) john      (1000)     5601 2024-04-16 13:57:51.000000 jgdv-0.1.1/jgdv/files/twitter/writers/thread.py
+-rw-rw-r--   0 john      (1000) john      (1000)     6958 2024-04-16 13:57:51.000000 jgdv-0.1.1/jgdv/files/twitter/writers/tweet.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1601 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/files/twitter/writers/users_table.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1134 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/files/twitter/writers/util.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1487 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/files/zip.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 13:58:45.237055 jgdv-0.1.1/jgdv/geom/
+-rw-rw-r--   0 john      (1000) john      (1000)       10 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/geom/__init__.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 13:58:45.241055 jgdv-0.1.1/jgdv/geom/dcel/
+-rw-rw-r--   0 john      (1000) john      (1000)       10 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/geom/dcel/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1068 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/geom/dcel/constants.py
+-rw-rw-r--   0 john      (1000) john      (1000)      918 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/geom/dcel/dcel.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 13:58:45.241055 jgdv-0.1.1/jgdv/geom/dcel/io/
+-rw-rw-r--   0 john      (1000) john      (1000)       10 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/geom/dcel/io/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)     3368 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/geom/dcel/io/drawing.py
+-rw-rw-r--   0 john      (1000) john      (1000)     6611 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/geom/dcel/io/export.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 13:58:45.241055 jgdv-0.1.1/jgdv/geom/dcel/mod/
+-rw-rw-r--   0 john      (1000) john      (1000)       10 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/geom/dcel/mod/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)     8161 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/geom/dcel/mod/adding.py
+-rw-rw-r--   0 john      (1000) john      (1000)     8846 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/geom/dcel/mod/processing.py
+-rw-rw-r--   0 john      (1000) john      (1000)     4322 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/geom/dcel/mod/subtracting.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 13:58:45.241055 jgdv-0.1.1/jgdv/geom/dcel/structs/
+-rw-rw-r--   0 john      (1000) john      (1000)       10 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/geom/dcel/structs/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1363 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/geom/dcel/structs/draw_settings.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1072 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/geom/dcel/structs/drawable.py
+-rw-rw-r--   0 john      (1000) john      (1000)    26133 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/geom/dcel/structs/face.py
+-rw-rw-r--   0 john      (1000) john      (1000)    36447 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/geom/dcel/structs/halfedge.py
+-rw-rw-r--   0 john      (1000) john      (1000)     6413 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/geom/dcel/structs/line.py
+-rw-rw-r--   0 john      (1000) john      (1000)     5372 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/geom/dcel/structs/state.py
+-rw-rw-r--   0 john      (1000) john      (1000)    11203 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/geom/dcel/structs/vertex.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 13:58:45.241055 jgdv-0.1.1/jgdv/geom/intersection/
+-rw-rw-r--   0 john      (1000) john      (1000)       10 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/geom/intersection/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1459 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/geom/intersection/result.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1965 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/geom/intersection/state.py
+-rw-rw-r--   0 john      (1000) john      (1000)    13125 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/geom/intersection/sweep.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 13:58:45.241055 jgdv-0.1.1/jgdv/geom/math/
+-rw-rw-r--   0 john      (1000) john      (1000)     4782 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/geom/math/bbox.py
+-rw-rw-r--   0 john      (1000) john      (1000)     4083 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/geom/math/circles.py
+-rw-rw-r--   0 john      (1000) john      (1000)     4760 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/geom/math/direction.py
+-rw-rw-r--   0 john      (1000) john      (1000)     3573 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/geom/math/distance.py
+-rw-rw-r--   0 john      (1000) john      (1000)     4664 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/geom/math/heightmap.py
+-rw-rw-r--   0 john      (1000) john      (1000)     8233 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/geom/math/lines.py
+-rw-rw-r--   0 john      (1000) john      (1000)     4585 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/geom/math/movement.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 13:58:45.245055 jgdv-0.1.1/jgdv/geom/voronoi/
+-rw-rw-r--   0 john      (1000) john      (1000)     2993 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/geom/voronoi/beachline.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1232 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/geom/voronoi/breakpoint.py
+-rw-rw-r--   0 john      (1000) john      (1000)     4072 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/geom/voronoi/data.py
+-rw-rw-r--   0 john      (1000) john      (1000)     9358 2024-04-16 13:57:51.000000 jgdv-0.1.1/jgdv/geom/voronoi/drawing.py
+-rw-rw-r--   0 john      (1000) john      (1000)     3019 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/geom/voronoi/events.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2484 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/geom/voronoi/graph.py
+-rw-rw-r--   0 john      (1000) john      (1000)    12980 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/geom/voronoi/line_sweep.py
+-rw-rw-r--   0 john      (1000) john      (1000)    21188 2024-04-16 13:57:51.000000 jgdv-0.1.1/jgdv/geom/voronoi/process.py
+-rw-rw-r--   0 john      (1000) john      (1000)    21184 2024-04-16 13:57:51.000000 jgdv-0.1.1/jgdv/geom/voronoi/voronoi.py
+-rw-rw-r--   0 john      (1000) john      (1000)     9358 2024-04-16 13:57:51.000000 jgdv-0.1.1/jgdv/geom/voronoi/voronoi_drawing.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1118 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/geom/voronoi/voronoi_io.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 13:58:45.245055 jgdv-0.1.1/jgdv/handlers/
+-rw-rw-r--   0 john      (1000) john      (1000)       10 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/handlers/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2740 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/handlers/handler.py
+-rw-rw-r--   0 john      (1000) john      (1000)    16665 2024-04-16 13:57:51.000000 jgdv-0.1.1/jgdv/handlers/handler_system.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 13:58:45.245055 jgdv-0.1.1/jgdv/importing/
+-rw-rw-r--   0 john      (1000) john      (1000)     1808 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/importing/inspect.py
+-rw-rw-r--   0 john      (1000) john      (1000)     5986 2024-04-16 13:57:51.000000 jgdv-0.1.1/jgdv/importing/plugin_loader.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 13:58:45.245055 jgdv-0.1.1/jgdv/keys/
+-rw-rw-r--   0 john      (1000) john      (1000)        0 2024-04-16 13:57:51.000000 jgdv-0.1.1/jgdv/keys/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)     9347 2024-04-16 13:57:51.000000 jgdv-0.1.1/jgdv/keys/base.py
+-rw-rw-r--   0 john      (1000) john      (1000)     9418 2024-04-16 13:57:51.000000 jgdv-0.1.1/jgdv/keys/decorator.py
+-rw-rw-r--   0 john      (1000) john      (1000)     3958 2024-04-16 13:57:51.000000 jgdv-0.1.1/jgdv/keys/formatter.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2573 2024-04-16 13:57:51.000000 jgdv-0.1.1/jgdv/keys/multikey.py
+-rw-rw-r--   0 john      (1000) john      (1000)     3252 2024-04-16 13:57:51.000000 jgdv-0.1.1/jgdv/keys/path_keys.py
+-rw-rw-r--   0 john      (1000) john      (1000)     8046 2024-04-16 13:57:51.000000 jgdv-0.1.1/jgdv/keys/simple.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 13:58:45.245055 jgdv-0.1.1/jgdv/location/
+-rw-rw-r--   0 john      (1000) john      (1000)        0 2024-04-16 13:57:51.000000 jgdv-0.1.1/jgdv/location/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)     8220 2024-04-16 13:57:51.000000 jgdv-0.1.1/jgdv/location/locations.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2397 2024-04-16 13:57:51.000000 jgdv-0.1.1/jgdv/location/toml_loc.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 13:58:45.245055 jgdv-0.1.1/jgdv/logging/
+-rw-rw-r--   0 john      (1000) john      (1000)       87 2024-04-16 13:57:51.000000 jgdv-0.1.1/jgdv/logging/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)     4525 2024-04-16 13:57:51.000000 jgdv-0.1.1/jgdv/logging/log_colour.py
+-rw-rw-r--   0 john      (1000) john      (1000)     5737 2024-04-16 13:57:51.000000 jgdv-0.1.1/jgdv/logging/log_config.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1881 2024-04-16 13:57:51.000000 jgdv-0.1.1/jgdv/logging/log_context.py
+-rw-rw-r--   0 john      (1000) john      (1000)     3809 2024-04-16 13:57:51.000000 jgdv-0.1.1/jgdv/logging/stdout_capture.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 13:58:45.249055 jgdv-0.1.1/jgdv/math/
+-rw-rw-r--   0 john      (1000) john      (1000)       23 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/math/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2992 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/math/colour.py
+-rw-rw-r--   0 john      (1000) john      (1000)     5165 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/math/comparison.py
+-rw-rw-r--   0 john      (1000) john      (1000)     5037 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/math/easings.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1670 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/math/matrices.py
+-rw-rw-r--   0 john      (1000) john      (1000)     8413 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/math/parabola.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2947 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/math/quadratic.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1310 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/math/quantize.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1159 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/math/rand.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1412 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/math/sorting.py
+-rw-rw-r--   0 john      (1000) john      (1000)    26889 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/math/umath.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2900 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/math/utils.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 13:58:45.249055 jgdv-0.1.1/jgdv/mixins/
+-rw-rw-r--   0 john      (1000) john      (1000)        0 2024-04-16 13:57:51.000000 jgdv-0.1.1/jgdv/mixins/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2117 2024-04-16 13:57:51.000000 jgdv-0.1.1/jgdv/mixins/enums.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1184 2024-04-16 13:57:51.000000 jgdv-0.1.1/jgdv/mixins/param_spec.py
+-rw-rw-r--   0 john      (1000) john      (1000)     7354 2024-04-16 13:57:51.000000 jgdv-0.1.1/jgdv/mixins/path_manip.py
+-rw-rw-r--   0 john      (1000) john      (1000)     8951 2024-04-16 13:57:51.000000 jgdv-0.1.1/jgdv/mixins/zipper.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 13:58:45.249055 jgdv-0.1.1/jgdv/setup/
+-rw-rw-r--   0 john      (1000) john      (1000)     2080 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/setup/asyncio_client.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2557 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/setup/asyncio_server.py
+-rw-rw-r--   0 john      (1000) john      (1000)      969 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/setup/gtk.py
+-rw-rw-r--   0 john      (1000) john      (1000)     3470 2024-04-16 13:57:51.000000 jgdv-0.1.1/jgdv/setup/hooks.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1189 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/setup/importing.py
+-rw-rw-r--   0 john      (1000) john      (1000)     4226 2024-04-16 13:57:51.000000 jgdv-0.1.1/jgdv/setup/main.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1087 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/setup/pyparsing.py
+-rw-rw-r--   0 john      (1000) john      (1000)     4571 2024-04-16 13:57:51.000000 jgdv-0.1.1/jgdv/setup/setup.py
+-rw-rw-r--   0 john      (1000) john      (1000)        0 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/setup/tkinter.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 13:58:45.249055 jgdv-0.1.1/jgdv/spiders/
+-rw-rw-r--   0 john      (1000) john      (1000)     2238 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/spiders/__init__.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 13:58:45.249055 jgdv-0.1.1/jgdv/spiders/__tests/
+-rw-rw-r--   0 john      (1000) john      (1000)     7020 2024-04-16 13:57:51.000000 jgdv-0.1.1/jgdv/spiders/__tests/test_runner.py
+-rw-rw-r--   0 john      (1000) john      (1000)    11494 2024-04-16 13:57:51.000000 jgdv-0.1.1/jgdv/spiders/__tests/test_tracker.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1558 2024-04-16 13:57:51.000000 jgdv-0.1.1/jgdv/spiders/actions.py
+-rw-rw-r--   0 john      (1000) john      (1000)     5438 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/spiders/caching.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2645 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/spiders/crawler.py
+-rw-rw-r--   0 john      (1000) john      (1000)     4602 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/spiders/middleware.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2638 2024-04-16 13:57:51.000000 jgdv-0.1.1/jgdv/spiders/mixin.py
+-rw-rw-r--   0 john      (1000) john      (1000)     4830 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/spiders/pipeline.py
+-rw-rw-r--   0 john      (1000) john      (1000)    11326 2024-04-16 13:57:51.000000 jgdv-0.1.1/jgdv/spiders/runner.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1854 2024-04-16 13:57:51.000000 jgdv-0.1.1/jgdv/spiders/spiders.py
+-rw-rw-r--   0 john      (1000) john      (1000)     8343 2024-04-16 13:57:51.000000 jgdv-0.1.1/jgdv/spiders/tracker.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 13:58:45.253055 jgdv-0.1.1/jgdv/structs/
+-rw-rw-r--   0 john      (1000) john      (1000)     4820 2024-04-16 13:57:51.000000 jgdv-0.1.1/jgdv/structs/artifact.py
+-rw-rw-r--   0 john      (1000) john      (1000)     6726 2024-04-16 13:57:51.000000 jgdv-0.1.1/jgdv/structs/code_ref.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 13:58:45.253055 jgdv-0.1.1/jgdv/structs/heap/
+-rw-rw-r--   0 john      (1000) john      (1000)       10 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/structs/heap/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1520 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/structs/heap/element.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1643 2024-04-16 13:57:51.000000 jgdv-0.1.1/jgdv/structs/heap/heap.py
+-rw-rw-r--   0 john      (1000) john      (1000)     3911 2024-04-16 13:57:51.000000 jgdv-0.1.1/jgdv/structs/name.py
+-rw-rw-r--   0 john      (1000) john      (1000)    11727 2024-04-16 13:57:51.000000 jgdv-0.1.1/jgdv/structs/param_spec.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 13:58:45.253055 jgdv-0.1.1/jgdv/structs/proxy/
+-rw-rw-r--   0 john      (1000) john      (1000)     6094 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/structs/proxy/base.py
+-rw-rw-r--   0 john      (1000) john      (1000)    12758 2024-04-16 13:57:51.000000 jgdv-0.1.1/jgdv/structs/proxy/iter_proxy.py
+-rw-rw-r--   0 john      (1000) john      (1000)     6312 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/structs/proxy/proxy.py
+-rw-rw-r--   0 john      (1000) john      (1000)     3265 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/structs/proxy/proxy_mixin.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 13:58:45.253055 jgdv-0.1.1/jgdv/structs/rbtree/
+-rw-rw-r--   0 john      (1000) john      (1000)      378 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/structs/rbtree/__init__.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 13:58:45.253055 jgdv-0.1.1/jgdv/structs/rbtree/__tests/
+-rw-rw-r--   0 john      (1000) john      (1000)        0 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/structs/rbtree/__tests/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)     3733 2024-04-16 13:57:51.000000 jgdv-0.1.1/jgdv/structs/rbtree/__tests/test_rbtree.py
+-rw-rw-r--   0 john      (1000) john      (1000)     7495 2024-04-16 13:57:51.000000 jgdv-0.1.1/jgdv/structs/rbtree/__tests/test_rbtree_node.py
+-rw-rw-r--   0 john      (1000) john      (1000)     3262 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/structs/rbtree/comparison_functions.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1708 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/structs/rbtree/node.py
+-rw-rw-r--   0 john      (1000) john      (1000)     7171 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/structs/rbtree/operations.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1735 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/structs/rbtree/rb_data.py
+-rw-rw-r--   0 john      (1000) john      (1000)     8673 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/structs/rbtree/rbtree.py
+-rw-rw-r--   0 john      (1000) john      (1000)     5268 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/structs/rbtree/utils.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1259 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/structs/regex.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 13:58:45.253055 jgdv-0.1.1/jgdv/structs/rete/
+-rw-rw-r--   0 john      (1000) john      (1000)       10 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/structs/rete/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)      896 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/structs/rete/alpha.py
+-rw-rw-r--   0 john      (1000) john      (1000)      896 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/structs/rete/beta.py
+-rw-rw-r--   0 john      (1000) john      (1000)      896 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/structs/rete/rete.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 13:58:45.253055 jgdv-0.1.1/jgdv/structs/time/
+-rw-rw-r--   0 john      (1000) john      (1000)      173 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/structs/time/__init__.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 13:58:45.253055 jgdv-0.1.1/jgdv/structs/time/__tests/
+-rw-rw-r--   0 john      (1000) john      (1000)    12753 2024-04-16 13:57:51.000000 jgdv-0.1.1/jgdv/structs/time/__tests/test_time.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1675 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/structs/time/dsl.py
+-rw-rw-r--   0 john      (1000) john      (1000)     5217 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/structs/time/pattern_constructor.py
+-rw-rw-r--   0 john      (1000) john      (1000)      889 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/structs/time/pattern_iterator.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 13:58:45.257055 jgdv-0.1.1/jgdv/structs/time/structs/
+-rw-rw-r--   0 john      (1000) john      (1000)       10 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/structs/time/structs/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1566 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/structs/time/structs/arc.py
+-rw-rw-r--   0 john      (1000) john      (1000)      896 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/structs/time/structs/base.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1719 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/structs/time/structs/event.py
+-rw-rw-r--   0 john      (1000) john      (1000)     5558 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/structs/time/structs/pattern.py
+-rw-rw-r--   0 john      (1000) john      (1000)      968 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/structs/time/structs/var.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2464 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/structs/time/utils.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1835 2024-04-16 13:57:51.000000 jgdv-0.1.1/jgdv/structs/trace.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 13:58:45.257055 jgdv-0.1.1/jgdv/structs/tree/
+-rw-rw-r--   0 john      (1000) john      (1000)       10 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/structs/tree/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)    11147 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/structs/tree/binary_tree.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 13:58:45.257055 jgdv-0.1.1/jgdv/structs/trie/
+-rw-rw-r--   0 john      (1000) john      (1000)       10 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/structs/trie/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)     3069 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/structs/trie/leaf.py
+-rw-rw-r--   0 john      (1000) john      (1000)     6186 2024-04-16 13:57:51.000000 jgdv-0.1.1/jgdv/structs/trie/semantics.py
+-rw-rw-r--   0 john      (1000) john      (1000)     3407 2024-04-16 13:57:51.000000 jgdv-0.1.1/jgdv/structs/trie/trie.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 13:58:45.257055 jgdv-0.1.1/jgdv/testing/
+-rw-rw-r--   0 john      (1000) john      (1000)       10 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/testing/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1748 2024-04-16 13:57:51.000000 jgdv-0.1.1/jgdv/testing/testing_fixtures.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 13:58:45.257055 jgdv-0.1.1/jgdv/utils/
+-rw-rw-r--   0 john      (1000) john      (1000)       10 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/utils/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1107 2024-04-15 14:39:20.000000 jgdv-0.1.1/jgdv/utils/slice.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-16 13:58:45.257055 jgdv-0.1.1/jgdv.egg-info/
+-rw-r--r--   0 john      (1000) john      (1000)     2763 2024-04-16 13:58:45.000000 jgdv-0.1.1/jgdv.egg-info/PKG-INFO
+-rw-rw-r--   0 john      (1000) john      (1000)     8341 2024-04-16 13:58:45.000000 jgdv-0.1.1/jgdv.egg-info/SOURCES.txt
+-rw-rw-r--   0 john      (1000) john      (1000)        1 2024-04-16 13:58:45.000000 jgdv-0.1.1/jgdv.egg-info/dependency_links.txt
+-rw-rw-r--   0 john      (1000) john      (1000)      137 2024-04-16 13:58:45.000000 jgdv-0.1.1/jgdv.egg-info/requires.txt
+-rw-rw-r--   0 john      (1000) john      (1000)        5 2024-04-16 13:58:45.000000 jgdv-0.1.1/jgdv.egg-info/top_level.txt
+-rw-rw-r--   0 john      (1000) john      (1000)     3912 2024-04-16 13:58:13.000000 jgdv-0.1.1/pyproject.toml
+-rw-rw-r--   0 john      (1000) john      (1000)       38 2024-04-16 13:58:45.257055 jgdv-0.1.1/setup.cfg
```

### Comparing `jgdv-0.1.0/LICENSE` & `jgdv-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jgdv-0.1.0/PKG-INFO` & `jgdv-0.1.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jgdv
-Version: 0.1.0
+Version: 0.1.1
 Author-email: John Grey <jgrey.n.plus.one+dejavu@gmail.com>
 License: * ACAB License
         
         © 2024-03-04 John Grey
         
         To the maximum extent applicable by law, and any licenses of components of this work:
         
@@ -44,15 +44,15 @@
 Project-URL: repository, https://github.com/jgrey4296/jgdv
 Project-URL: changelog, https://github.com/jgrey4296/jgdv/blob/master/CHANGELOG.md
 Classifier: Programming Language :: Python
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: tomlguard
-Requires-Dist: mastodonpy
+Requires-Dist: mastodon.py>=1.8
 Requires-Dist: selenium
 Requires-Dist: numpy
 Requires-Dist: scrapy
 Requires-Dist: pyparsing
 Requires-Dist: construct
 Requires-Dist: networkx
 Requires-Dist: gi
```

### Comparing `jgdv-0.1.0/jgdv/_interfaces/accessors.py` & `jgdv-0.1.1/jgdv/_interfaces/accessors.py`

 * *Files identical despite different names*

### Comparing `jgdv-0.1.0/jgdv/_interfaces/dbm.py` & `jgdv-0.1.1/jgdv/files/sha256.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,60 +1,44 @@
 #!/usr/bin/env python3
 """
 
+See EOF for license/metadata/notes as applicable
 """
-##-- imports
+
+##-- builtin imports
 from __future__ import annotations
 
-import types
-import abc
+# import abc
 import datetime
 import enum
 import functools as ftz
 import itertools as itz
 import logging as logmod
 import pathlib as pl
 import re
 import time
-from copy import deepcopy
-from dataclasses import InitVar, dataclass, field
+import types
+import weakref
+# from copy import deepcopy
+# from dataclasses import InitVar, dataclass, field
 from typing import (TYPE_CHECKING, Any, Callable, ClassVar, Final, Generic,
                     Iterable, Iterator, Mapping, Match, MutableMapping,
                     Protocol, Sequence, Tuple, TypeAlias, TypeGuard, TypeVar,
-                    cast, final, overload, runtime_checkable)
+                    cast, final, overload, runtime_checkable, Generator)
 from uuid import UUID, uuid1
-from weakref import ref
 
-##-- end imports
+##-- end builtin imports
+
+##-- lib imports
+import more_itertools as mitz
+##-- end lib imports
 
 ##-- logging
 logging = logmod.getLogger(__name__)
 ##-- end logging
 
-from abc import abstractmethod
-
-@runtime_checkable
-class DBManager_p(Protocol):
+from hashlib import sha256
 
-    @abstractmethod
-    def set(self, task_id, dependency, value):
-        raise NotImplementedError()
-
-    @abstractmethod
-    def get(self, task_id, dependency):
-        raise NotImplementedError()
-
-    @abstractmethod
-    def in_(self, task_id):
-        raise NotImplementedError()
-
-    @abstractmethod
-    def dump(self):
-        raise NotImplementedError()
-
-    @abstractmethod
-    def remove(self, task_id):
-        raise NotImplementedError()
-
-    @abstractmethod
-    def remove_all(self):
-        raise NotImplementedError()
+def file_to_hash(filename):
+    path = pl.Path(filename)
+    assert(path.exists())
+    return sha256(path.read_bytes()).hexdigest()
```

### Comparing `jgdv-0.1.0/jgdv/_interfaces/decorator.py` & `jgdv-0.1.1/jgdv/_interfaces/decorator.py`

 * *Files 7% similar despite different names*

```diff
@@ -33,25 +33,25 @@
 import more_itertools as mitz
 ##-- end lib imports
 
 ##-- logging
 logging = logmod.getLogger(__name__)
 ##-- end logging
 
-class DejaVuDecorator_i:
+class JGDVDecorator_i:
     """ Base Class for decorators that annotate callables """
 
     def __init__(self, funcOrCls:Callable):
         ftz.update_wrapper(self, funcOrCls)
         self._func = func
 
     def __call__(self, *args, **kwargs):
         return self._func(*args, **kwargs)
 
-class DejaVuDelayDecorator_i:
+class JGDVDelayDecorator_i:
     """ Base Class for decorators that take arguments, then later annotate callables
 
     https://stackoverflow.com/questions/9416947
       """
 
     def __init__(self):
         self._func = None
```

### Comparing `jgdv-0.1.0/jgdv/_interfaces/factory.py` & `jgdv-0.1.1/jgdv/_interfaces/factory.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -35,11 +35,11 @@
 
 ##-- logging
 logging = logmod.getLogger(__name__)
 ##-- end logging
 
 class Factory_p(abc.ABC):
 
-    @abc.abstractmethod
     @classmethod
+    @abc.abstractmethod
     def build(cls, *args, **kwargs):
         pass
```

### Comparing `jgdv-0.1.0/jgdv/_interfaces/policy.py` & `jgdv-0.1.1/jgdv/_interfaces/policy.py`

 * *Files identical despite different names*

### Comparing `jgdv-0.1.0/jgdv/_interfaces/singletons.py` & `jgdv-0.1.1/jgdv/_interfaces/singletons.py`

 * *Files identical despite different names*

### Comparing `jgdv-0.1.0/jgdv/_interfaces/task.py` & `jgdv-0.1.1/jgdv/location/locations.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,247 +1,225 @@
-"""TASKS ARE THE MAIN ABSTRACTIONS MANAGED BY DOOT
-
-  - JOBS create tasks
-  - TASKS have actions
-  - ACTIONS are individual atomic steps of a task, given the detailed information necessary to perform the step.
-
-Jobs, as they can control refication order, can add setup and teardown tasks.
-This can allow interleaving, or grouping.
-
-  Communication:
-  Job  -> Task   : by creation
-  Task -> Action : by creation
-  Action -> Task : by return value, updating task state dict
-  Task -> Job    : by reference to the job
-
-  Task -> Task     = Task -> Job -> Task
-  Action -> Action = Action -> Task -> Action
+#!/usr/bin/env python3
+"""
 
 """
+##-- imports
 from __future__ import annotations
 
-import logging as logmod
 import abc
-import types
-from typing import Generator, NewType, Protocol, Any, runtime_checkable
-
-from tomlguard import TomlGuard
+import logging as logmod
+import pathlib as pl
+from copy import deepcopy
+from dataclasses import InitVar, dataclass, field, replace
+from re import Pattern
+from typing import (TYPE_CHECKING, Any, Callable, ClassVar, Final, Generic,
+                    Iterable, Iterator, Mapping, Match, MutableMapping,
+                    Protocol, Sequence, Tuple, TypeAlias, TypeGuard, TypeVar,
+                    cast, final, overload, runtime_checkable)
+from uuid import UUID, uuid1
+from weakref import ref
 
-import doot
-import doot.errors
-from doot.enums import TaskFlags, TaskStateEnum, ActionResponseEnum
-from doot._abstract.parser import ParamSpecMaker_m
-from doot.structs import DootParamSpec, TaskStub, DootTaskSpec, DootTaskName, DootActionSpec
+##-- end imports
 
 ##-- logging
 logging = logmod.getLogger(__name__)
+# If CLI:
+# logging = logmod.root
+# logging.setLevel(logmod.NOTSET)
 ##-- end logging
 
-STATE_TASK_NAME_K : Final[str] = doot.constants.patterns.STATE_TASK_NAME_K
-
-@runtime_checkable
-class Action_p(Protocol):
-    """
-    holds individual action information and state, and executes it
-    """
-    _toml_kwargs : ClassVar[list[str]] = []
-
-    @abc.abstractmethod
-    def __call__(self, spec:DootActionSpec, task_state:dict) -> dict|bool|ActionResponseEnum|None:
-        raise NotImplementedError()
-
-class TaskBase_i(ParamSpecMaker_m):
-    """ Core Interface for Tasks """
-
-    _version         : str       = "0.1"
-    _help            : list[str] = []
-
-    @classmethod
-    @property
-    def param_specs(cls) -> list[DootParamSpec]:
-        """  make class parameter specs  """
-        return [
-            cls.make_param(name="help", default=False, invisible=True, prefix="--"),
-            cls.make_param(name="debug", default=False, invisible=True, prefix="--"),
-            cls.make_param(name="verbose", default=0, type=int, invisible=True, prefix="--")
-           ]
-
-    def __init__(self, spec:DootTaskSpec):
-        self.spec       : DootTaskSpec        = spec
-        self.status     : TaskStateEnum       = TaskStateEnum.WAIT
-        self.flags      : TaskFlags           = TaskFlags.JOB
-        self._records   : list[Any]           = []
-        self.state                            = dict(spec.extra)
-        self.state[STATE_TASK_NAME_K]         = self.spec.name
-        self.state['_action_step']            = 0
-
-    @property
-    def readable_name(self) -> str:
-        return str(self.spec.name.readable)
-
-    @property
-    def name(self) -> str:
-        return str(self.spec.name)
-
-    @property
-    def fullname(self) -> DootTaskName:
-        return self.spec.name
-
-    def __hash__(self):
-        return hash(self.name)
+import os
+import re
+import tomlguard
+from jgdv.errors import DirAbsent, LocationExpansionError, LocationError
+from jgdv.mixins.path_manip import PathManip_m
+from jgdv.enums.location_meta import LocationMeta
+
+KEY_PAT        = doot.constants.patterns.KEY_PATTERN
+MAX_EXPANSIONS = doot.constants.patterns.MAX_KEY_EXPANSIONS
+
+class JGDVLocations(PathManip_m):
+    """
+      A Single point of truth for task access to locations.
+      key=value pairs in [[locations]] toml blocks are integrated into it.
+
+      it expands relative paths according to cwd(),
+      but can be used as a context manager to expand from a temp different root
+
+      location designations are of the form:
+      key = 'location/subdirectory/file'
+      simple locations can be accessed as attributes: locs.temp
+
+      more complex locations, with expansions, are accessed as items:
+      locs['{temp}/somewhere']
+      will expand 'temp' (if it is a registered location)
+      """
+    locmeta = LocationMeta
+
+    def __init__(self, root:Pl.Path):
+        self._root    : pl.Path()               = root.expanduser().absolute()
+        self._data    : dict[str, TomlLocation] = dict()
+        self._loc_ctx : None|DootLocations      = None
 
-    def __lt__(self, other:TaskBase_i) -> bool:
-        """ Task A < Task B iff A ∈ B.run_after   """
-        return (other.name in self.spec.after_artifacts
-                or other.name in self.spec.depends_on)
+    def __repr__(self):
+        keys = ", ".join(iter(self))
+        return f"<DootLocations : {str(self.root)} : ({keys})>"
 
-    def __eq__(self, other):
-        match other:
-            case str():
-                return self.name == other
-            case TaskBase_i():
-                return self.name == other.name
+    def __getattr__(self, key) -> pl.Path:
+        """
+          get a location by name from loaded toml
+          delegates to __getitem__
+          eg: locs.temp
+          """
+        if key == "__self__":
+            return None
+        return self[DootKey.build(key, strict=True)]
+
+    def __getitem__(self, val:str|DootKey|pl.Path|DootTaskArtifact) -> pl.Path:
+        """
+          eg: doot.locs['{data}/somewhere']
+          A public utility method to easily convert paths.
+          delegates to DootKey's path expansion
+
+          Get a location using item access for extending a stored path.
+          eg: locs['{temp}/imgs/blah.jpg']
+        """
+        match DootKey.build(val, explicit=True):
+            case DootNonKey() as key:
+                return key.to_path(locs=self)
+            case DootSimpleKey() as key:
+                return key.to_path(locs=self)
+            case DootMultiKey() as key:
+                return key.to_path(locs=self)
             case _:
-                return False
-
-    @property
-    def short_doc(self) -> str:
-        """ Generate Job Class 1 line help string """
-        try:
-            split_doc = [x for x in self.__class__.__doc__.split("\n") if bool(x)]
-            return ":: " + split_doc[0].strip() if bool(split_doc) else ""
-        except AttributeError:
-            return ":: "
-
-    @property
-    def doc(self) -> list[str]:
-        return self.spec.doc or self._help
-
-    @property
-    def depends_on(self) -> abc.Generator[str|DootTaskName]:
-        for x in self.spec.depends_on:
-            yield x
+                raise LocationExpansionError("Unrecognized location expansion argument", val)
 
-    @property
-    def required_for(self) -> abc.Generator[str|DootTaskName]:
-        for x in self.spec.required_for:
-            yield x
-
-    def add_execution_record(self, arg):
-        """ Record some execution record information for display or debugging """
-        self._records.append(arg)
+    def __contains__(self, key:str|DootKey|pl.Path|DootTaskArtifact):
+        """ Test whether a key is a registered location """
+        return key in self._data
+
+    def __iter__(self) -> Generator[str]:
+        """ Iterate over the registered location names """
+        return iter(self._data.keys())
+
+    def __call__(self, new_root=None) -> Self:
+        """ Create a copied locations object, with a different root """
+        new_obj = DootLocations(new_root or self._root)
+        return new_obj.update(self)
+
+    def __enter__(self) -> Any:
+        """ replaces the global doot.locs with this locations obj,
+        and changes the system root to wherever this locations obj uses as root
+        """
+        self._loc_ctx = doot.locs
+        doot.locs = self
+        os.chdir(doot.locs._root)
+        return self
+
+    def __exit__(self, exc_type, exc_value, exc_traceback) -> bool:
+        """ returns the global state to its original, """
+        assert(self._loc_ctx is not None)
+        doot.locs     = self._loc_ctx
+        os.chdir(doot.locs._root)
+        self._loc_ctx = None
+        return False
+
+    def get(self, key:DootSimpleKey|str, on_fail:None|str|pl.Path=Any) -> None|pl.Path:
+        """
+          convert a *simple* key of one value to a path.
+          does *not* recursively expand returned paths
+          More complex expansion is handled in DootKey and subclasses
+        """
+        assert(isinstance(key,(DootSimpleKey,str))), (str(key), type(key))
+        match key:
+            case DootNonKey():
+                return pl.Path(key.form)
+            case str() | DootSimpleKey() if key in self._data:
+                return self._data[key].base
+            case _ if on_fail is None:
+                return None
+            case _ if on_fail != Any:
+                return self.get(on_fail)
+            case DootSimpleKey():
+                return pl.Path(key.form)
+            case _:
+                return pl.Path(key)
 
-    def log(self, msg, level=logmod.DEBUG, prefix=None) -> None:
+    def normalize(self, path:pl.Path, symlinks:bool=False) -> pl.Path:
         """
-        utility method to log a message, useful as tasks are running
+          Expand a path to be absolute, taking into account the set doot root.
+          resolves symlinks unless symlinks=True
         """
-        prefix : str       = prefix or ""
-        lines  : list[str] = []
-        match msg:
-            case str():
-                lines.append(msg)
-            case types.LambdaType():
-                lines.append(msg())
-            case [types.LambdaType()]:
-                lines += msg[0]()
-            case list():
-                lines += msg
+        return self._normalize(path, root=self.root)
 
-        for line in lines:
-            logging.log(level, prefix + str(line))
-
-    @classmethod
-    @abc.abstractmethod
-    def class_help(cls) -> str:
-        raise NotImplementedError(cls, "help")
+    def metacheck(self, key:str|DootKey, meta:LocationMeta) -> bool:
+        """ check if any key provided has the applicable meta flags """
+        match key:
+            case DootNonKey():
+                return False
+            case DootSimpleKey() if key in self._data:
+                return self._data[key].check(meta)
+            case DootMultiKey():
+                 for k in DootKey.build(key):
+                     if k not in self._data:
+                         continue
+                     if self._data[k].check(meta):
+                         return True
+            case str():
+                return self.metacheck(DootKey.build(key), meta)
+        return False
 
-    @classmethod
-    @abc.abstractmethod
-    def stub_class(cls, TaskStub):
+    @property
+    def root(self):
         """
-        Specialize a TaskStub to describe this class
+          the registered root location
         """
-        raise NotImplementedError(cls, "stub_class")
+        return self._root
 
-    @abc.abstractmethod
-    def stub_instance(self, TaskStub):
+    def update(self, extra:dict|TomlGuard|DootLocations, strict=True) -> Self:
         """
-          Specialize a TaskStub with the settings of this specific instance
+          Update the registered locations with a dict, tomlguard, or other dootlocations obj.
         """
-        raise NotImplementedError(self.__class__, "stub_instance")
-
-    @property
-    @abc.abstractmethod
-    def is_stale(self) -> bool:
-        """ Query whether the task's artifacts have become stale and need to be rebuilt"""
-        raise NotImplementedError()
-
-class Task_i(TaskBase_i):
-    """
-    holds task information and state, produces actions to execute.
-
-    """
-
-    def __init__(self, spec:DootTaskSpec, *, job:Job_i=None, **kwargs):
-        super().__init__(spec)
-        self.job     = job
-
-    def __repr__(self):
-        return f"<Task: {self.name}>"
-
-    def maybe_more_tasks(self) -> Generator[Task_i]:
-        return iter([])
-
-    @classmethod
-    def class_help(cls):
-        """ Task *class* help. """
-        help_lines = [f"Task   : {cls.__qualname__} v{cls._version}", ""]
-        mro = " -> ".join(x.__name__ for x in cls.mro())
-        help_lines.append(f"Task MRO: {mro}")
-        help_lines.append("")
-        help_lines += cls._help
-
-        return "\n".join(help_lines)
+        match extra: # unwrap to just a dict
+            case dict():
+                pass
+            case tomlguard.TomlGuard():
+                return self.update(extra._table())
+            case DootLocations():
+                return self.update(extra._data)
+            case _:
+                raise doot.errors.LocationError("Tried to update locations with unknown type: %s", extra)
 
-    @property
-    @abc.abstractmethod
-    def actions(self) -> Generator[Action_p]:
-        """lazy creation of action instances"""
-        raise NotImplementedError()
+        raw          = dict(self._data.items())
+        base_keys    = set(raw.keys())
+        new_keys     = set()
+        for k,v in extra.items():
+            match TomlLocation.build(k, v):
+                case _ if k in new_keys and v != raw[k]:
+                    raise LocationError("Duplicated, non-matching Key", k)
+                case _ if k in base_keys:
+                    logging.debug("Skipping Location update of: %s", k)
+                    pass
+                case TomlLocation() as l if l.check(LocationMeta.normOnLoad):
+                    raw[l.key] = TomlLocation.build(k, v, base=self.normalize(l.base))
+                    new_keys.add(l.key)
+                case TomlLocation() as l:
+                    raw[l.key] = l
+                    new_keys.add(l.key)
+                case _:
+                    raise LocationError("Couldn't build a TomlLocation for: (%s : %s)", k, v)
+
+        logging.debug("Registered New Locations: %s", ", ".join(new_keys))
+        self._data = raw
+        return self
+
+    def ensure(self, *values, task="doot"):
+        """ Ensure the values passed in are registered locations,
+          error with DirAbsent if they aren't
+        """
+        missing = set(x for x in values if x not in self)
 
-class Job_i(Task_i):
-    """
-    builds tasks
-    """
+        if bool(missing):
+            raise DirAbsent("Ensured Locations are missing for %s : %s", task, missing)
 
-    @classmethod
-    def class_help(cls) -> str:
-        """ Job *class* help. """
-        help_lines = [f"Job : {cls.__qualname__} v{cls._version}    ({cls.__module__}:{cls.__qualname__})", ""]
-
-        mro = " -> ".join(x.__name__ for x in cls.mro())
-        help_lines.append(f"Job MRO: {mro}")
-        help_lines.append("")
-        help_lines += cls._help
-
-        params = cls.param_specs
-        if bool([x for x in params if not x.invisible]):
-            help_lines += ["", "Params:"]
-            help_lines += [str(x) for x in cls.param_specs if not x.invisible]
-
-        return "\n".join(help_lines)
-
-    @abc.abstractmethod
-    def default_task(self, name:str|DootTaskName|None, extra:None|dict|TomlGuard) -> DootTaskSpec:
-        raise NotImplementedError(self.__class__, "default_task")
-
-    @abc.abstractmethod
-    def specialize_task(self, task:DootTaskSpec) -> DootTaskSpec|None:
-        raise NotImplementedError(self.__class__, "specialize_task")
-
-    @abc.abstractmethod
-    def build(self, **kwargs) -> abc.Generator[Task_i]:
-        raise NotImplementedError()
-
-    @abc.abstractmethod
-    def _build_head(self, **kwargs) -> DootTaskSpec:
-        raise NotImplementedError()
+    def _clear(self):
+        self._data = tomlguard.TomlGuard()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `jgdv-0.1.0/jgdv/apis/clingo/__tests/test_clingo_solver.py` & `jgdv-0.1.1/jgdv/apis/clingo/__tests/test_clingo_solver.py`

 * *Files identical despite different names*

### Comparing `jgdv-0.1.0/jgdv/apis/clingo/ast.py` & `jgdv-0.1.1/jgdv/apis/clingo/ast.py`

 * *Files identical despite different names*

### Comparing `jgdv-0.1.0/jgdv/apis/clingo/clingo_solver.py` & `jgdv-0.1.1/jgdv/apis/clingo/clingo_solver.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,17 +18,17 @@
 ##-- logging
 logging       = logmod.getLogger(__name__)
 clingo_logger = logmod.getLogger(__name__ + ".ffi.clingo")
 ##-- end logging
 
 import clingo
 from clingo import Control, Function, Number, Symbol, parse_term
-from dejavu._interfaces.solver import SolverWrapper_i
-from dejavu.apis.clingo.ast import SolverAST
-from dejavu.apis.clingo.solver import SolverModelResult, SolverWrapper_i
+from jgdv._interfaces.solver import SolverWrapper_i
+from jgdv.apis.clingo.ast import SolverAST
+from jgdv.apis.clingo.solver import SolverModelResult, SolverWrapper_i
 
 def clingo_intercept_logger(code, msg):
     """
     Intercepts messages from clingo, and controls
     the logging of them
     """
     msg = msg.replace("\n", "")
```

### Comparing `jgdv-0.1.0/jgdv/apis/clingo/compiler.py` & `jgdv-0.1.1/jgdv/apis/clingo/compiler.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,18 +12,18 @@
 from dataclasses import InitVar, dataclass, field
 from pathlib import Path
 
 ##-- end imports
 
 logging = logmod.getLogger(__name__)
 
-from dejavu.apis.clingo.ast import SolverAST
+from jgdv.apis.clingo.ast import SolverAST
 
 @dataclass
-class InstalCompiler_i(metaclass=abc.ABCMeta):
+class Compiler_i(metaclass=abc.ABCMeta):
     """
     Interface for compiling InstaASTR down to a
     specific solver format
     """
     _compiled_text : list[str] = field(init=False, default_factory=list)
     # TODO add delayed registers
```

### Comparing `jgdv-0.1.0/jgdv/apis/clingo/parser.py` & `jgdv-0.1.1/jgdv/apis/clingo/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
                     cast, final, overload, runtime_checkable)
 from unittest.util import safe_repr
 
 ##-- end imports
 
 logging = logmod.getLogger(__name__)
 
-from dejavu.apis.clingo.ast import SolverAST
+from jgdv.apis.clingo.ast import SolverAST
 import pyparsing as pp
 import pyparsing.testing as ppt
 
 class SolverDSL_i(metaclass=abc.ABCMeta):
     """
     The abstract api of an Instal Parser.
```

### Comparing `jgdv-0.1.0/jgdv/apis/clingo/reporter.py` & `jgdv-0.1.1/jgdv/apis/clingo/reporter.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from typing import (TYPE_CHECKING, Any, Callable, ClassVar, Final, Generic,
                     Iterable, Iterator, Mapping, Match, MutableMapping,
                     Protocol, Sequence, Tuple, TypeAlias, TypeGuard, TypeVar,
                     cast, final, overload, runtime_checkable)
 
 ##-- end imports
 
-from dejavu.apis.clingo.trace import Trace_i
+from jgdv.apis.clingo.trace import Trace_i
 
 @dataclass
 class SolverReporter_i(metaclass=abc.ABCMeta):
     """
         Solver Report Generator interface
     """
```

### Comparing `jgdv-0.1.0/jgdv/apis/clingo/solver.py` & `jgdv-0.1.1/jgdv/apis/clingo/solver.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
                     cast, final, overload, runtime_checkable)
 
 ##-- end imports
 
 logging = logmod.getLogger(__name__)
 
 from clingo import parse_term
-from dejavu.appis.clingo.ast import SolverAST
+from jgdv.apis.clingo.ast import SolverAST
 
 @dataclass
 class SolverModelResult:
     """
     The immediate results data structure returned by a solver.
     Does no translation from the data structures the solver uses.
```

### Comparing `jgdv-0.1.0/jgdv/apis/clingo/trace.py` & `jgdv-0.1.1/jgdv/apis/clingo/trace.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,16 +19,16 @@
 from weakref import ref
 
 ##-- end imports
 
 logging = logmod.getLogger(__name__)
 
 from clingo import Symbol
-from dejavu.apis.clingo.ast import SolverAST
-from dejavu.apis.clingo.solver import SolverModelResult
+from jgdv.apis.clingo.ast import SolverAST
+from jgdv.apis.clingo.solver import SolverModelResult
 
 STATE_HOLDSAT_GROUPS = []
 
 @dataclass
 class State_i:
     """
     Description of a single moment in a model's trace.
```

### Comparing `jgdv-0.1.0/jgdv/apis/clingo/validate.py` & `jgdv-0.1.1/jgdv/apis/clingo/validate.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from uuid import UUID, uuid1
 from weakref import ref
 
 ##-- end imports
 
 logging = logmod.getLogger(__name__)
 
-from dejavu.apis.clingo.ast import SolverAST
+from jgdv.apis.clingo.ast import SolverAST
 
 class SolverASTVisitor_i(metaclass=abc.ABCMeta):
     """
     Interface for the AST Visitor,
     the stub of whic which can be generated
     with instal.cli.generate_vistor
     """
```

### Comparing `jgdv-0.1.0/jgdv/apis/mastodon/actions.py` & `jgdv-0.1.1/jgdv/apis/mastodon/actions.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,17 +37,16 @@
 logging = logmod.getLogger(__name__)
 ##-- end logging
 
 printer = logmod.getLogger("doot._printer")
 
 import mastodon
 import tomlguard
-from dejavu.apis.mastodon import errors as djerror
-import doot
-from doot.structs import DootKey
+from jgdv.apis.mastodon import errors as djerror
+from jgdv.key import JGDVKey
 
 TOOT_SIZE            : Final[int]                   = doot.config.on_fail(250, int).mastodon.toot_size()
 TOOT_IMAGE_SIZE      : Final[str]                   = doot.config.on_fail(8_000_000, int).mastodon.image_size()
 RESOLUTION_BLACKLIST : Final[list]                  = doot.locs.image_blacklist
 RESOLUTION_RE        : Final[re.Pattern]            = re.compile(r".*?([0-9]+x[0-9]+)")
 TOOT_IMAGE_TYPES     : Final[list[str]]             = [".jpg", ".png", ".gif"]
```

### Comparing `jgdv-0.1.0/jgdv/apis/mastodon/error.py` & `jgdv-0.1.1/jgdv/apis/mastodon/error.py`

 * *Files identical despite different names*

### Comparing `jgdv-0.1.0/jgdv/apis/selenium/selenium.py` & `jgdv-0.1.1/jgdv/apis/selenium/selenium.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,20 +34,14 @@
 
 ##-- logging
 logging = logmod.getLogger(__name__)
 printer = logmod.getLogger("doot._printer")
 ##-- end logging
 
 import base64
-import doot
-import doot.errors
-from doot.structs import DootKey
-from doot.enums import ActionResponseEnum
-from dootle.tags.structs import TagFile
-from dootle.bookmarks.structs import BookmarkCollection
 
 from selenium.webdriver import FirefoxOptions, FirefoxService, Firefox
 from selenium.webdriver.common.print_page_options import PrintOptions
 
 FF_DRIVER     = "__$ff_driver"
 READER_PREFIX = "about:reader?url="
 
@@ -81,12 +75,11 @@
     time.sleep(2)
     pdf       = _driver.print_page(print_options=print_ops)
     pdf_bytes = base64.b64decode(pdf)
 
     with open(_to, "wb") as f:
         f.write(pdf_bytes)
 
-
 @DootKey.kwrap.types(FF_DRIVER)
 def close_firefox(spec, state, _driver):
     printer.info("Closing Firefox")
     _driver.quit()
```

### Comparing `jgdv-0.1.0/jgdv/apis/sphinx/directive.py` & `jgdv-0.1.1/jgdv/apis/sphinx/directive.py`

 * *Files identical despite different names*

### Comparing `jgdv-0.1.0/jgdv/cli/__tests/test_flexible.py` & `jgdv-0.1.1/jgdv/cli/__tests/test_flexible.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,20 +11,14 @@
 from typing import (Any, Callable, ClassVar, Generic, Iterable, Iterator,
                     Mapping, Match, MutableMapping, Sequence, Tuple, TypeAlias,
                     TypeVar, cast)
 ##-- end imports
 logging = logmod.root
 
 import pytest
-import doot.errors
-from doot._abstract import ArgParser_i, TaskBase_i
-from doot.parsers.flexible import DootFlexibleParser
-from doot.structs import DootParamSpec, DootTaskSpec, DootCodeReference
-from doot.utils.mock_gen import mock_parse_cmd, mock_parse_task
-
 
 @pytest.mark.parametrize("ctor", [DootFlexibleParser])
 class TestArgParser:
 
     def test_initial(self, ctor):
         parser = ctor()
         assert(isinstance(parser, ArgParser_i))
@@ -211,15 +205,14 @@
         parser   = ctor()
         result   = parser.parse(["doot", "-key"],
             doot_specs=[param], cmds={}, tasks={}
             )
 
         assert(result.head.args.key is True)
 
-
     def test_simple_short_arg(self, ctor, mocker):
         param = DootParamSpec("key", bool)
         parser   = ctor()
         result   = parser.parse(["doot", "-k"],
             doot_specs=[param], cmds={}, tasks={}
             )
 
@@ -259,46 +252,41 @@
         parser   = ctor()
         result   = parser.parse(["doot", "--key=blah"],
             doot_specs=[param], cmds={}, tasks={}
             )
 
         assert(result.head.args.key == "blah")
 
-
     def test_assign_fail_with_wrong_prefix(self, ctor, mocker):
         param    = DootParamSpec("key", str, prefix="-")
         parser   = ctor()
 
         with pytest.raises(doot.errors.DootParseError):
             parser.parse(["doot", "--key=blah"],
                 doot_specs=[param], cmds={}, tasks={}
                 )
 
-
-
     def test_simple_follow_assign(self, ctor, mocker):
         param    = DootParamSpec("key", str)
         parser   = ctor()
         result   = parser.parse(["doot", "-key", "blah"],
             doot_specs=[param], cmds={}, tasks={}
             )
 
         assert(result.head.args.key == "blah")
 
-
     def test_simple_prefix_change(self, ctor, mocker):
         param    = DootParamSpec("key", str, prefix="--")
         parser   = ctor()
         result   = parser.parse(["doot", "--key", "blah"],
             doot_specs=[param], cmds={}, tasks={}
             )
 
         assert(result.head.args.key == "blah")
 
-
     def test_simple_separator_change(self, ctor, mocker):
         param    = DootParamSpec("key", str, separator="%%", prefix="--")
         parser   = ctor()
         result   = parser.parse(["doot", "--key%%blah"],
             doot_specs=[param], cmds={}, tasks={}
             )
 
@@ -335,29 +323,27 @@
         parser   = ctor()
         result   = parser.parse(["doot" , "val"],
             doot_specs=[], cmds={"run": cmd_mock }, tasks={"val": task_mock}
             )
 
         assert(result.cmd.name == "run")
 
-
     def test_simple_task(self, ctor, mocker):
         cmd_mock             = mock_parse_cmd()
         task_mock            = mock_parse_task(params=[{"name":"key"}])
 
         parser               = ctor()
         result               = parser.parse(["doot", "list", '-key'],
             doot_specs=[], cmds={"run": cmd_mock }, tasks={"list" : task_mock}
             )
 
         assert(result.cmd.name == "run")
         assert("list" in result.tasks)
         assert(result.tasks.list.key is True)
 
-
     def test_simple_task_sequence(self, ctor, mocker):
         cmd_mock   = mock_parse_cmd()
         task_mock  = mock_parse_task(params=[{"name":"key", "type":bool}])
         task_mock2 = mock_parse_task(params=[{"name":"other", "type":bool}])
 
         parser     = ctor()
         result     = parser.parse(["doot", "list", "-key", "blah", "-other"],
```

### Comparing `jgdv-0.1.0/jgdv/cli/arg_parser.py` & `jgdv-0.1.1/jgdv/cli/arg_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,17 +23,14 @@
 ##-- end imports
 
 ##-- logging
 logging = logmod.getLogger(__name__)
 ##-- end logging
 
 from tomlguard import TomlGuard
-import doot
-import doot.errors
-from doot.structs import DootParamSpec, DootTaskSpec
 from collections import ChainMap
 import jgdv
 
 SEP : Final[str]          = "--"
 PARAM_ASSIGN_PREFIX       = doot.constants.patterns.PARAM_ASSIGN_PREFIX
 NON_DEFAULT_KEY           = doot.constants.misc.NON_DEFAULT_KEY
 
@@ -53,16 +50,16 @@
     def add_param_specs(self, specs:list):
         self.specs += specs
 
     @abstractmethod
     def parse(self, args:list[str], doot_arg_specs:list[DootParamSpec], cmds:TomlGuard, tasks:TomlGuard) -> TomlGuard:
         raise NotImplementedError()
 
-@jgdv.dbg.check_protocol
-class DejaVuCLIParser(ArgParser_i):
+@jgdv.check_protocol
+class JGDVCLIParser(ArgParser_i):
     """
     convert argv to tomlguard by:
     parsing each arg as toml,
 
     # doot {args} {cmd} {cmd_args}
     # doot {args} [{task} {tasks_args}] - implicit do cmd
     """
@@ -70,15 +67,15 @@
     class _ParseState(enum.Enum):
         HEAD  = enum.auto()
         CMD   = enum.auto()
         TASK  = enum.auto()
         EXTRA = enum.auto()
 
     def __init__(self):
-        self.PS               = DejaVuCLIParser._ParseState
+        self.PS               = JGDVCLIParser._ParseState
         self.head_arg_specs   = None
         self.registered_cmds  = None
         self.registered_tasks = None
         self.default_help     = DootParamSpec(name="help", default=False, prefix="--")
 
         ## -- results
         self.head_call                          = None
```

### Comparing `jgdv-0.1.0/jgdv/cli/repl/commands/break_cmd.py` & `jgdv-0.1.1/jgdv/cli/repl/commands/break_cmd.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,42 +8,33 @@
 import logging as logmod
 from dataclasses import InitVar, dataclass, field
 from typing import (TYPE_CHECKING, Any, Callable, ClassVar, Final, Generic,
                     Iterable, Iterator, Mapping, Match, MutableMapping,
                     Protocol, Sequence, Tuple, TypeAlias, TypeGuard, TypeVar,
                     cast, final, overload, runtime_checkable)
 
-import pyparsing as pp
-import acab
-from acab.modules.repl.repl_commander import register_class
-from acab.modules.repl.ReplParser import rst
-from acab.interfaces.debugger import AcabDebugger_i
-
-if TYPE_CHECKING:
-    # tc only imports
-    pass
-
 ##-- end imports
 
+import pyparsing as pp
 
 logging     = logmod.getLogger(__name__)
 config      = acab.config
 # TODO import
 Debugger    = config.imports.specific.debug
 debug_intro = config.module.REPL.debug.intro
 
 the_debugger = Debugger()
 
-
 # TODO breakpoint a semantic handler by name,
 # TODO breakpoint (in)dependent semantic function
 # TODO breakpoint a node by sentence path
 # TODO breakpoint an operator/action
 # TODO breakpoint a variable
 #
+
 @register_class("break")
 class BreakCmd:
     """
     Control the Acab Debugger.
     Specified in Config [Module.Debug].
 
     Usage:
@@ -73,15 +64,14 @@
 
         parser_bp    = pp.Keyword("parser") + rst("parser")
 
         break_parser = parser_bp | semantic_bp("semantic") | basic_bp("basic") | rst
 
         return break_parser
 
-
     def __call__(self, line):
         if not bool(the_debugger):
             the_debugger.set_running_trace()
 
         try:
             ctxs = self._parser.parse_string(line, parse_all=True)
         except pp.ParseException as err:
@@ -141,15 +131,14 @@
         if turn_off:
             print(f"Turning Breakpoint off for: {ctxs['parser']}")
             parser.set_break(False)
         else:
             print(f"Turning Breakpoint on for: {ctxs['parser']}")
             parser.set_break(True)
 
-
     def handle_semantic(self, ctxs):
         # run query
         self._repl.state.ctxs = self._repl.state.engine(ctxs.semantic)
         # attach semantic breakpoints to each prod_abstraction
         if (len(self._repl.state.ctxs) == 1 and
             isinstance(self._repl.state.ctxs[0]._current.value, Instruction_i)):
             curr = self._repl.state.ctxs[0]._current.value
```

### Comparing `jgdv-0.1.0/jgdv/cli/repl/commands/commands_info.py` & `jgdv-0.1.1/jgdv/cli/repl/commands/commands_info.py`

 * *Files 17% similar despite different names*

```diff
@@ -14,27 +14,19 @@
 from enum import Enum
 from os.path import abspath, exists, expanduser, split, splitext
 from typing import (TYPE_CHECKING, Any, Callable, ClassVar, Final, Generic,
                     Iterable, Iterator, Mapping, Match, MutableMapping,
                     Protocol, Sequence, Tuple, TypeAlias, TypeGuard, TypeVar,
                     cast, final, overload, runtime_checkable)
 
-import acab
-import pyparsing as pp
-from acab import types as AT
-from acab.core.parsing import debug_funcs as DBF
-from acab_config.utils.log_formatter import AcabLogFormatter, AcabMinimalLogRecord
-from acab.core.value.instruction import ProductionOperator, ProductionStructure
-from acab.modules.repl import ReplParser as RP
-from acab.modules.repl.repl_commander import register
-
 ##-- end imports
 
-config = acab.config
+import pyparsing as pp
 
+config = acab.config
 
 logging = logmod.getLogger(__name__)
 
 # TODO shift this into config
 ModuleFragment : TypeAlias = AT.ModuleFragment
 
 SPLIT_RE         = re.compile("[ .!?/]")
@@ -46,12 +38,11 @@
     """
     Print the :{kw} shortcut bindings loaded from config
     """
     print("Repl Shortcut commands: ")
     for kw, cmd in shortcut_pairs:
         print(f"    :{kw:<5} -> {cmd}")
 
-
 @register
 def do_acab(self, line):
     """ All Cops Are Bastards """
     print("All Cops Are Bastards")
```

### Comparing `jgdv-0.1.0/jgdv/cli/repl/commands/control.py` & `jgdv-0.1.1/jgdv/cli/repl/commands/control.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 from enum import Enum
 from os.path import abspath, exists, expanduser, split, splitext
 
 ##-- end imports
 
 logging = logmod.getLogger(__name__)
 
-import acab
 import pyparsing as pp
 
 try:
     import readline
 except ImportError:
     readline = None
 
@@ -50,14 +49,15 @@
         self.state.collect_str = []
         self.state.prompt_bkup = self.state.prompt
         self.state.prompt = self.state.prompt_ml
         self.state.indent = 0
         if bool(readline):
             # indent modification based on:
             # https://stackoverflow.com/questions/8505163
+
             def input_hook():
                 indent_str = self.state.indent * "    "
                 readline.insert_text(indent_str)
                 readline.redisplay()
 
             readline.set_pre_input_hook(input_hook)
     else:
@@ -71,17 +71,14 @@
 
         logging.info(f"Collected: {collected}")
         if bool(line):
             self.onecmd(line + " " + collected)
         else:
             self.onecmd(collected)
 
-
-
-
 @register
 def do_pop(self, line):
     """
     Pop off the last string added in multi-line mode,
     for when an error was made
     """
     self.state.collect_str.pop()
@@ -91,15 +88,14 @@
 def do_collect(self, line):
     """ Add a line to the multi line collection,
     ready to be used as one statement when multi line is closed """
     assert(self.state.in_multi_line)
     if line.strip() == "end":
         self.state.indent = max(self.state.indent - 1, 0)
 
-
     curr_indent = self.state.indent
     curr_indent_str = curr_indent * "    "
 
     self.state.collect_str.append(curr_indent_str + line)
     if line[-1] == ":":
         self.state.indent += 1
 
@@ -108,15 +104,14 @@
 @register
 def do_echo(self, line):
     """
     Toggle echoing of working memory state
     """
     self.state.echo = not self.state.echo
 
-
 @register
 def do_suppress(self, line):
     """
     Repl Command to suppress all repl commands
     (except itself and `exit`.)
     """
     # TODO
```

### Comparing `jgdv-0.1.0/jgdv/cli/repl/commands/exit_cmd.py` & `jgdv-0.1.1/jgdv/cli/repl/commands/exit_cmd.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,24 +6,19 @@
 import logging as logmod
 from dataclasses import InitVar, dataclass, field
 from typing import (TYPE_CHECKING, Any, Callable, ClassVar, Final, Generic,
                     Iterable, Iterator, Mapping, Match, MutableMapping,
                     Protocol, Sequence, Tuple, TypeAlias, TypeGuard, TypeVar,
                     cast, final, overload, runtime_checkable)
 
-logging = logmod.getLogger(__name__)
-
-if TYPE_CHECKING:
-    # tc only imports
-    pass
-
-from acab.modules.repl.repl_commander import register_class
 
 ##-- end imports
 
+logging = logmod.getLogger(__name__)
+
 @register_class("exit")
 class ExitCmd:
     """
     Exit the repl, automatically saving the self state
     """
 
     def __call__(self, line):
```

### Comparing `jgdv-0.1.0/jgdv/cli/repl/commands/force_parser_cmd.py` & `jgdv-0.1.1/jgdv/cli/repl/commands/force_parser_cmd.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,28 +7,17 @@
 import traceback
 from dataclasses import InitVar, dataclass, field
 from typing import (TYPE_CHECKING, Any, Callable, ClassVar, Final, Generic,
                     Iterable, Iterator, Mapping, Match, MutableMapping,
                     Protocol, Sequence, Tuple, TypeAlias, TypeGuard, TypeVar,
                     cast, final, overload, runtime_checkable)
 
-logging = logmod.getLogger(__name__)
-
-if TYPE_CHECKING:
-    # tc only imports
-    pass
-
-import pyparsing as pp
-from acab.modules.repl import ReplParser as RP
-from acab.modules.repl.repl_commander import register_class
-from acab.interfaces.handler_system import HandlerSpec_i
-from acab.core.parsing.debug_funcs import dfs_activate
-
 ##-- end imports
 
+logging = logmod.getLogger(__name__)
 rst = RP.rst
 
 @register_class("forcep")
 class ForceParserCmd:
     """ Force Parser:
     Query the bootstrap parser,
     and if supplied text, parse it and try to run it
```

### Comparing `jgdv-0.1.0/jgdv/cli/repl/commands/init_cmd.py` & `jgdv-0.1.1/jgdv/cli/repl/commands/init_cmd.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,26 +8,14 @@
 import logging as logmod
 import re
 import traceback
 from datetime import datetime
 from enum import Enum
 from os.path import abspath, exists, expanduser, split, splitext
 
-import acab
-from acab.core.value.instruction import ProductionContainer
-from acab_config import AcabConfigException
-from acab.error.importer import AcabImportException
-from acab.error.semantic import AcabSemanticException
-from acab.interfaces.engine import AcabEngine_i
-from acab.interfaces.value import Instruction_i
-from acab.modules.repl import ReplParser as RP
-from acab.modules.repl.repl_commander import register
-from acab.modules.repl.util import init_inspect
-from acab.modules.repl.commands.util import print_module_colour
-
 ##-- end imports
 
 logging = logmod.getLogger(__name__)
 config  = acab.config
 
 @register
 def do_init(self, line):
```

### Comparing `jgdv-0.1.0/jgdv/cli/repl/commands/log_cmd.py` & `jgdv-0.1.1/jgdv/cli/repl/commands/log_cmd.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,36 +9,30 @@
 from dataclasses import InitVar, dataclass, field
 from typing import (TYPE_CHECKING, Any, Callable, ClassVar, Final, Generic,
                     Iterable, Iterator, Mapping, Match, MutableMapping,
                     Protocol, Sequence, Tuple, TypeAlias, TypeGuard, TypeVar,
                     cast, final, overload, runtime_checkable)
 from os.path import splitext
 
-import pyparsing as pp
-import acab
-from acab.modules.repl.repl_commander import register_class
-from acab_config.utils.log_formatter import SimpleLogColour
-import acab.modules.repl.commands.util as ColPr
-from acab.interfaces.fragments import ModuleFragment
-
 ##-- end imports
 
+import pyparsing as pp
+
 logging = logmod.getLogger(__name__)
 SC      = SimpleLogColour
 
 config = acab.config
 import_dict = config.imports.specific
 
 @register_class("log")
 class ReportCmd:
     """
     Control the Repl log level, format,
     and specify filters for the logger
 
-
     """
 
     def __init__(self):
         self._parser = self._gen_parser()
 
     def _gen_parser(self):
         operator_kw  = pp.MatchFirst([pp.Keyword("ops"),
```

### Comparing `jgdv-0.1.0/jgdv/cli/repl/commands/memory_cmds.py` & `jgdv-0.1.1/jgdv/cli/repl/commands/memory_cmds.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,26 +15,18 @@
 from enum import Enum
 from os.path import abspath, exists, expanduser, split, splitext
 from typing import (TYPE_CHECKING, Any, Callable, ClassVar, Final, Generic,
                     Iterable, Iterator, Mapping, Match, MutableMapping,
                     Protocol, Sequence, Tuple, TypeAlias, TypeGuard, TypeVar,
                     cast, final, overload, runtime_checkable)
 
-import acab
-import pyparsing as pp
-from acab import types as AT
-from acab.core.parsing import debug_funcs as DBF
-from acab.core.util.debugging import (human, print_diff, print_stat,
-                                      print_stat_file, sh_filter)
-from acab.core.value.instruction import ProductionOperator, ProductionStructure
-from acab.modules.repl import ReplParser as RP
-from acab.modules.repl.repl_commander import register, register_default
-
 ##-- end imports
 
+import pyparsing as pp
+
 logging = logmod.getLogger(__name__)
 config  = acab.config
 
 snap_a  = None
 
 def display_memory(self):
     """
```

### Comparing `jgdv-0.1.0/jgdv/cli/repl/commands/print_cmd.py` & `jgdv-0.1.1/jgdv/cli/repl/commands/print_cmd.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,28 +6,18 @@
 import logging as logmod
 from dataclasses import InitVar, dataclass, field
 from typing import (TYPE_CHECKING, Any, Callable, ClassVar, Final, Generic,
                     Iterable, Iterator, Mapping, Match, MutableMapping,
                     Protocol, Sequence, Tuple, TypeAlias, TypeGuard, TypeVar,
                     cast, final, overload, runtime_checkable)
 
-import pyparsing as pp
-
-logging = logmod.getLogger(__name__)
-
-if TYPE_CHECKING:
-    # tc only imports
-    pass
-
-from acab.modules.repl.repl_commander import register_class
-from acab.modules.repl.ReplParser import rst, ctx_parser
-from acab import types as AT
-
 ##-- end imports
 
+import pyparsing as pp
+logging = logmod.getLogger(__name__)
 ModuleFragment = AT.ModuleFragment
 
 @register_class("print")
 class PrintCmd:
     """
     Print out details of the current state.
```

### Comparing `jgdv-0.1.0/jgdv/cli/repl/commands/report_cmd.py` & `jgdv-0.1.1/jgdv/cli/repl/commands/report_cmd.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,23 +9,18 @@
 from dataclasses import InitVar, dataclass, field
 from typing import (TYPE_CHECKING, Any, Callable, ClassVar, Final, Generic,
                     Iterable, Iterator, Mapping, Match, MutableMapping,
                     Protocol, Sequence, Tuple, TypeAlias, TypeGuard, TypeVar,
                     cast, final, overload, runtime_checkable)
 from os.path import splitext
 
-import pyparsing as pp
-import acab
-from acab.modules.repl.repl_commander import register_class
-from acab_config.utils.log_formatter import SimpleLogColour
-import acab.modules.repl.commands.util as ColPr
-from acab.interfaces.fragments import ModuleFragment
-
 ##-- end imports
 
+import pyparsing as pp
+
 logging = logmod.getLogger(__name__)
 SC      = SimpleLogColour
 
 config = acab.config
 import_dict = config.imports.specific
 
 @register_class("report")
```

### Comparing `jgdv-0.1.0/jgdv/cli/repl/commands/tutorial_cmd.py` & `jgdv-0.1.1/jgdv/structs/time/structs/var.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,40 +1,43 @@
 #!/usr/bin/env python3
-##-- imports
+"""
+
+
+See EOF for license/metadata/notes as applicable
+"""
+
+##-- builtin imports
 from __future__ import annotations
 
-import abc
+# import abc
+import datetime
+import enum
+import functools as ftz
+import itertools as itz
 import logging as logmod
-from dataclasses import InitVar, dataclass, field
+import pathlib as pl
+import re
+import time
+import types
+import weakref
+# from copy import deepcopy
+# from dataclasses import InitVar, dataclass, field
 from typing import (TYPE_CHECKING, Any, Callable, ClassVar, Final, Generic,
                     Iterable, Iterator, Mapping, Match, MutableMapping,
                     Protocol, Sequence, Tuple, TypeAlias, TypeGuard, TypeVar,
-                    cast, final, overload, runtime_checkable)
+                    cast, final, overload, runtime_checkable, Generator)
+from uuid import UUID, uuid1
+
+##-- end builtin imports
+
+##-- lib imports
+import more_itertools as mitz
+##-- end lib imports
 
+##-- logging
 logging = logmod.getLogger(__name__)
+##-- end logging
 
-from acab.modules.repl.repl_commander import register_class
+class TimeVar:
 
-if TYPE_CHECKING:
-    # tc only imports
-    pass
-
-##-- end imports
-
-@register_class("tutorial")
-class TutorialCmd:
-    """
-    Print out a basic tutorial of Acab and this Repl
-    """
-
-    def __init__(self):
-        self._parser = self._gen_parser()
-
-    def _gen_parser(self):
-        pass
-
-    def __call__(self, line):
-        # Print a section, return to main loop,
-        # if tutorial is called again, continue
-        # if restart is passed in, restart the tutorial
-        # also include option to print tutorial for a module
-        return
+    def __init__(self, name):
+        self.name = name
```

### Comparing `jgdv-0.1.0/jgdv/cli/repl/commands/util.py` & `jgdv-0.1.1/jgdv/cli/repl/commands/util.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,16 +11,14 @@
 from typing import (TYPE_CHECKING, Any, Callable, ClassVar, Final, Generic,
                     Iterable, Iterator, Mapping, Match, MutableMapping,
                     Protocol, Sequence, Tuple, TypeAlias, TypeGuard, TypeVar,
                     cast, final, overload, runtime_checkable)
 from uuid import UUID, uuid1
 from weakref import ref
 
-from acab_config.utils.log_formatter import SimpleLogColour
-
 ##-- end imports
 
 logging = logmod.getLogger(__name__)
 SC      = SimpleLogColour
 
 def print_header(header):
     print("\n--------------------")
```

### Comparing `jgdv-0.1.0/jgdv/cli/repl/error.py` & `jgdv-0.1.1/jgdv/error/repl.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,12 +33,12 @@
 import more_itertools as mitz
 ##-- end lib imports
 
 ##-- logging
 logging = logmod.getLogger(__name__)
 ##-- end logging
 
-class DejaVuREPLException(Error):
+class JGDVREPLException(Error):
     pass
 
-class DejaVuREPLPArseException(DejaVuREPLException):
+class JGDVREPLPArseException(JGDVREPLException):
     pass
```

### Comparing `jgdv-0.1.0/jgdv/cli/repl/repl_commander.py` & `jgdv-0.1.1/jgdv/cli/repl/repl_commander.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,25 +17,23 @@
 ##-- end imports
 
 ##-- logging
 logging      = logmod.getLogger(__name__)
 trace_logger = logmod.getLogger('acab.repl.trace')
 ##-- end logging
 
-import acab
 import pyparsing as pp
 from .repl_state import ReplState
-from .error import DejaVuREPLException
+from .error import JGDVREPLException
 
 repl_intro = ["Welcome to DejaVu's Default Repl Commander.",
               "Type 'help' or '?' to list commands.",
               "Type 'tutorial' for a tutorial.", "Type ':q' to quit."
               ]
 
-
 class REPLCommander(cmd.Cmd):
     """ Implementation of cmd.Cmd to provide an extensible REPL"""
     intro                                                   = "\n".join(repl_intro)
     prompt                                                  = initial_prompt + ": "
     _latebind                                               = []
     _default_startups  : ClassVar[list[Callable[..., Any]]] = []
 
@@ -52,17 +50,17 @@
 
     def default(self, line):
         """ Called when no other command matches """
         # default to assertion / query / run
         try:
             self.state.ctxs = self.state.engine(line,
                                                 ctxset=self.state.ctxs)
-        except DejaVuREPLParseException as err:
+        except JGDVREPLParseException as err:
             print(str(err))
-        except DejaVuREPLException as err:
+        except JGDVREPLException as err:
             logging.warning("\n--------------------\nFailure:\n")
             traceback.print_tb(err.__traceback__)
             logging.warning(f"\n{err.args[-1]}\n")
             print(str(err))
 
     def precmd(self, line):
         """ For massaging the input command """
@@ -77,16 +75,14 @@
             if self.state.in_multi_line and not line[0] in ["multi", "pop", "exit", "echo"]:
                 logging.info("In Multi")
                 line = ["collect"] + line
 
             if bool(self.state.echo):
                 print(f"{line}")
 
-
-
             return " ".join(line)
 
         except pp.ParseException as err:
             traceback.print_tb(err.__traceback__)
             logging.warning(f"Parse Failure: {err.markInputline()}")
 
     def onecmd(self, line):
@@ -135,29 +131,29 @@
 
     def emptyline(self):
         """ Overrides default of 'repeat last command',
         and prints the working memory
         """
         return self.onecmd("print wm")
 
-
     @classmethod
     def register(cls, fn):
         """ Decorator for registering a function into the repl """
         logging.debug(f"{cls.__name__} Registration: {fn.__name__}")
         assert("do_" in fn.__name__)
         assert(fn.__name__ not in dir(cls))
         setattr(cls, fn.__name__, fn)
         return fn
 
     @classmethod
     def register_class(cls, name):
         """ Register an entire class as the command bound to do_{name},
         (specifically the class' __call__ method)
         """
+
         def __register(target_cls):
             assert(hasattr(target_cls, "__call__"))
             assert(hasattr(cls, "_latebind"))
             if (not bool(target_cls.__call__.__doc__)) and bool(target_cls.__doc__):
                 target_cls.__call__.__doc__ = target_cls.__doc__
 
             instance = target_cls()
@@ -166,21 +162,18 @@
             setattr(instance, "_repl", None)
 
             cls._latebind.append(instance)
             return target_cls
 
         return __register
 
-
     @classmethod
     def register_default(cls, fn):
         """
         Register and automatically call the function when REPLCommander is created.
         eg: register_default(do_ctxprompt) means the repl will show active context numbers
         from startup
 
         """
         assert(hasattr(cls, "_default_startups"))
         cls.register(fn)
         cls._default_startups.append(fn)
-
-
```

### Comparing `jgdv-0.1.0/jgdv/cli/repl/repl_dsl.py` & `jgdv-0.1.1/jgdv/cli/repl/repl_dsl.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,21 +3,18 @@
 
 """
 ##-- imports
 from __future__ import annotations
 
 import logging as logmod
 
-import pyparsing as pp
-from acab.core.parsing import consts as PU
-from acab.core.parsing import parsers as AP
-from acab.modules.repl.util import build_slice
-
 ##-- end imports
 
+import pyparsing as pp
+
 logging = logmod.getLogger(__name__)
 config  = acab.config
 
 rst     = pp.delimited_list(pp.rest_of_line, delim=pp.White("\n\r"), combine=True).leave_whitespace()
 
 ##-- multi line
 MULTI_LINE_START = config.module.REPL.MULTI_LINE_START
@@ -27,42 +24,41 @@
 multi_line_end = pp.Regex(MULTI_LINE_END)
 
 multi_line_start.set_parse_action(lambda s,l,t: "multi")
 multi_line_end.set_parse_action(lambda s,l,t: "multi")
 
 ##-- end multi line
 
-
 shortcut_config   = config.module.REPL.shortcuts
 short_cmd_parsers = []
 
 ##-- shortcuts
+
 def gen_action(cmd):
+
     def __action(s, l, t):
         return cmd
 
     return __action
 
 for cmd in shortcut_config._keys:
     kw      = shortcut_config[cmd]
     s_cmd_p = pp.Keyword(kw)
     s_cmd_p.set_parse_action(gen_action(cmd))
     short_cmd_parsers.append(s_cmd_p)
 
 ##-- end shortcuts
 
-
 sugared = pp.Suppress(pp.Literal(":")) + pp.MatchFirst(short_cmd_parsers) + rst
 
 precmd_parser = pp.MatchFirst([multi_line_start,
                                multi_line_end + rst,
                                sugared,
                                rst]).leave_whitespace()
 
-
 ##-- step kws
 back_kw     = pp.Keyword("back")
 rule_kw     = pp.Keyword("rule")
 layer_kw    = pp.Keyword("layer")
 pipe_kw     = pp.Keyword("pipe")
 pipeline_kw = pp.Keyword("pipeline")
 step_parser = pp.MatchFirst([back_kw,
@@ -136,15 +132,14 @@
 ##-- context selection
 
 ctx_index  = number("subset")
 ctx_subset = slice_p("subset")
 clear_kw   = pp.Keyword("clear")("clear")
 minus_kw   = pp.Keyword("-")("clear")
 
-
 ctx_select_parser = pp.MatchFirst([ctx_subset,
                                    ctx_index,
                                    clear_kw,
                                    minus_kw,
                                    rst])
 
 ##-- end context selection
```

### Comparing `jgdv-0.1.0/jgdv/cli/repl/repl_state.py` & `jgdv-0.1.1/jgdv/cli/repl/repl_state.py`

 * *Files identical despite different names*

### Comparing `jgdv-0.1.0/jgdv/cli/shell.py` & `jgdv-0.1.1/jgdv/cli/shell.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,26 +7,22 @@
 logging = logmod.getLogger(__name__)
 ##-- end logging
 
 printer = logmod.getLogger("doot._printer")
 
 import sys
 import sh
-import doot
-from doot.errors import DootTaskError
-from doot._abstract import Action_p
-from doot.structs import DootKey
 import jgdv
 
 BACKGROUND = DootKey.make("background")
 UPDATE     = DootKey.make("update_")
 NOTTY      = DootKey.make("notty")
 ENV        = DootKey.make("shenv_")
 
-class DejaVuDootShellBake:
+class JGDVShellBake:
 
     @DootKey.kwrap.args
     @DootKey.kwrap.types("in_", hint={"on_fail":None, "type_":sh.Command|bool|None})
     @DootKey.kwrap.types("env", hint={"on_fail":sh, "type_":sh.Command|bool|None})
     @DootKey.kwrap.redirects("update_")
     def __call__(self, spec, state, args, _in, env, _update):
         if not env:
@@ -53,15 +49,15 @@
 
             printer.info("")
             if bool(err.stderr):
                 printer.error("%s", err.stderr.decode())
 
         return False
 
-class DejaVuShellBakedRun:
+class JGDVShellBakedRun:
 
     @DootKey.kwrap.types("in_", hint={"on_fail":None, "type_":sh.Command|None})
     @DootKey.kwrap.redirects("update_")
     def __call__(self, spec, state, _in, _update):
         try:
             result = _in()
             return { _update : result }
@@ -74,15 +70,15 @@
 
             printer.info("")
             if bool(err.stderr):
                 printer.error("%s", err.stderr.decode())
 
         return False
 
-class DejaVuShellAction(Action_p):
+class JGDVShellAction(Action_p):
     """
     For actions in subshells.
     all other arguments are passed directly to the program, using `sh`
 
     can use a pre-baked sh passed into what "shenv_" points to
     """
 
@@ -116,27 +112,27 @@
 
             printer.info("")
             if bool(err.stderr):
                 printer.error("%s", err.stderr.decode())
 
         return False
 
-class DejaVuInteractiveAction(Action_p):
+class JGDVInteractiveAction(Action_p):
     """
       An interactive command, which uses the self.interact method as a callback for sh.
     """
     _toml_args = ["background"]
     aggregated = ""
     prompt     = ">>> "
     cont       = "... "
 
     def __call__(self, spec, state:dict) -> dict|bool|None:
         try:
-            self.prompt = spec.kwargs.on_fail(DejaVuInteractiveAction.prompt, str).prompt()
-            self.cont   = spec.kwargs.on_fail(DejaVuInteractiveAction.cont, str).cont()
+            self.prompt = spec.kwargs.on_fail(JGDVInteractiveAction.prompt, str).prompt()
+            self.cont   = spec.kwargs.on_fail(JGDVInteractiveAction.cont, str).cont()
 
             cmd      = getattr(sh, spec.args[0])
             args     = spec.args[1:]
             keys     = [DootKey.make(x, explicit=True) for x in args]
             expanded = [x.expand(spec, state, locs=doot.locs) for x in keys]
             result   = cmd(*expanded, _return_cmd=True, _bg=spec.kwargs.on_fail(False, bool).background(), _out=self.interact, _out_bufsize=0, _tty_in=True, _unify_ttys=True)
             assert(result.exit_code == 0)
```

### Comparing `jgdv-0.1.0/jgdv/cli/speak.py` & `jgdv-0.1.1/jgdv/cli/speak.py`

 * *Files 11% similar despite different names*

```diff
@@ -21,18 +21,14 @@
 ##-- end imports
 
 printer = logmod.getLogger("doot._printer")
 
 from time import sleep
 import sys
 import sh
-import doot
-from doot.structs import DootKey
-from doot.errors import DootTaskError, DootTaskFailed
-from doot._abstract import Action_p
 
 class SpeakTimeAction(Action_p):
     """
     A Simple Action that announces the time
     Subclass this and override __call__ for your own actions.
     The arguments of the action are held in self.spec
```

### Comparing `jgdv-0.1.0/jgdv/debugging/dsl.py` & `jgdv-0.1.1/jgdv/debugging/dsl.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,35 +22,95 @@
 
 ##-- end imports
 
 ##-- logging
 logging = logmod.getLogger(__name__)
 ##-- end logging
 
-MARK     = ">!<"
-MATCHING = "Matching" + (" " * 17)
-MATCHED  = "Matched"  + ("-" * 14)
-FAILED   = "Failed"   + ("_" * 11)
+MARK                      = ">!<"
+MATCHING                  = "Matching" + (" " * 17)
+MATCHED                   = "Matched"  + ("-" * 14)
+FAILED                    = "Failed"   + ("_" * 11)
+
+try_format   : Final[str] = "{3[0]:>10}{3[1]:3}{3[2]:<10} {0} <{1}> at {2}:  "
+match_format : Final[str] = "{4[0]:>10}{4[1]:3}{4[2]:<10}\t {0} <{1}> ({2}) {3}"
+fail_format  : Final[str] = "{5[0]:>10}{5[1]:3}{5[2]:<10}\t\t {0} <{1}>: {2} found '{3}' at {4}"
+
+class PyParsingDebuggerControl:
+
+    @staticmethod
+    def debug_pyparsing(*flags, all_warnings=False):
+        """ Set pyparsing to debug
+        Only applies for parsers created *after* this,
+        so has to be set at boot time.
+        """
+        # pylint: disable=protected-access
+        if flags is None:
+            flags = [pp.Diagnostics.enable_debug_on_named_expressions]
+        if not debug_pyparsing_active_p():
+            logging.info("Enabling Debug on %s Parsers", "Named")
+            pp.__diag__.enable_debug_on_named_expressions = True
+            if bool(flags):
+                for flag in flags:
+                    pp.enable_diag(flag)
+
+            if all_warnings:
+                pp.enable_all_warnings()
+            ppc._default_success_debug_action                 = debug_match_action
+            ppc._default_start_debug_action                   = debug_try_action
+            ppc._default_exception_debug_action               = debug_fail_action
+        else:
+            logging.warning("PyParsing Debug is already active")
+
+
+    @staticmethod
+    def dfs_activate(*parsers, remove=False):
+        """ DFS on a parser, adding debug funcs to named sub parsers """
+        # pylint: disable=protected-access
+        queue = list(parsers)
+        found = set()
+        while bool(queue):
+            current = queue.pop(0)
+            if current is None or id(current) in found:
+                continue
+
+            found.add(id(current))
+
+            if bool(current.name) and current.name != current._defaultName and not remove:
+                current.set_debug_actions(debug_try_action,
+                                        debug_match_action,
+                                        debug_fail_action)
+            elif remove:
+                current.set_debug_actions(None, None, None)
+
+            if hasattr(current, 'expr'):
+                queue.append(current.expr)
+            elif hasattr(current, 'exprs'):
+                queue += current.exprs
+
+    @static
+    def debug_active_p() -> bool:
+        return pp.__diag__.enable_debug_on_named_expressions
+
 
-##-- debug funcs
 def debug_try_action(instring, loc, expr, *args):
     """
     Log Entry into parsers
     """
     # pylint: disable=unused-argument, consider-using-f-string
     context = _calc_mark_string(instring, loc)
-    logging.warning("{3[0]:>10}{3[1]:3}{3[2]:<10} {0} <{1}> at {2}:  ".format(MATCHING, expr.name, loc, context))
+    logging.warning(try_format.format(MATCHING, expr.name, loc, context))
 
 def debug_match_action(instring, startloc, endloc, expr, toks, *args):
     """
     Log Parser Success
     """
     # pylint: disable=unused-argument, consider-using-f-string
     context = _calc_mark_string(instring, endloc)
-    logging.warning("{4[0]:>10}{4[1]:3}{4[2]:<10}\t {0} <{1}> ({2}) {3}".format(MATCHED, expr.name, str(toks), endloc, context))
+    logging.warning(match_format.format(MATCHED, expr.name, str(toks), endloc, context))
 
 def debug_fail_action(instring, loc, expr, exc, *args):
     """
     Log Parser failure
     """
     # pylint: disable=unused-argument, consider-using-f-string
     if isinstance(exc, pp.ParseBaseException):
@@ -60,84 +120,28 @@
         loc       = exc.loc
     else:
         found_str = "AssertionError"
         mark_str  = ("", "", "")
         msg       = ""
         loc       = ""
 
-    logging.error("{5[0]:>10}{5[1]:3}{5[2]:<10}\t\t {0} <{1}>: {2} found '{3}' at {4}".format(
-                  FAILED, expr.name, msg, found_str, loc, mark_str))
-
-
-##-- end debug funcs
-
-##-- activation
-def debug_pyparsing(*flags, all_warnings=False):
-    """ Set pyparsing to debug
-    Only applies for parsers created *after* this,
-    so has to be set at boot time.
-    """
-    # pylint: disable=protected-access
-    if flags is None:
-        flags = [pp.Diagnostics.enable_debug_on_named_expressions]
-    if not debug_pyparsing_active_p():
-        logging.info("Enabling Debug on %s Parsers", "Named")
-        pp.__diag__.enable_debug_on_named_expressions = True
-        if bool(flags):
-            for flag in flags:
-                pp.enable_diag(flag)
-
-        if all_warnings:
-            pp.enable_all_warnings()
-        ppc._default_success_debug_action                 = debug_match_action
-        ppc._default_start_debug_action                   = debug_try_action
-        ppc._default_exception_debug_action               = debug_fail_action
-    else:
-        logging.warning("PyParsing Debug is already active")
+    logging.error(fail_format.format(FAILED, expr.name, msg, found_str, loc, mark_str))
 
 
 
-def dfs_activate(*parsers, remove=False):
-    """ DFS on a parser, adding debug funcs to named sub parsers """
-    # pylint: disable=protected-access
-    queue = list(parsers)
-    found = set()
-    while bool(queue):
-        current = queue.pop(0)
-        if current is None or id(current) in found:
-            continue
 
-        found.add(id(current))
 
-        if bool(current.name) and current.name != current._defaultName and not remove:
-            current.set_debug_actions(debug_try_action,
-                                      debug_match_action,
-                                      debug_fail_action)
-        elif remove:
-            current.set_debug_actions(None, None, None)
 
-        if hasattr(current, 'expr'):
-            queue.append(current.expr)
-        elif hasattr(current, 'exprs'):
-            queue += current.exprs
 
-
-##-- end activation
-
-##-- util
+## util
 def _calc_mark_string(instring, loc, buffer=10):
     str_len  = len(instring)
     pre_str  = instring[max(0, loc-buffer):max(0, loc)]
     post_str = instring[max(0, loc):min(str_len, loc+buffer)]
     return pre_str.replace("\n", "\\n"), MARK, post_str.replace("\n", "\\n")
 
 
-def debug_pyparsing_active_p() -> bool:
-    return pp.__diag__.enable_debug_on_named_expressions
-
-##-- end util
-
 
 # except pp.ParseException as err:
 #     import traceback
 #     traceback.print_tb(err.__traceback__)
 #     logging.warning(f"Parse Failure: {err.markInputline()}")
```

### Comparing `jgdv-0.1.0/jgdv/debugging/frame_helper.py` & `jgdv-0.1.1/jgdv/debugging/frame_helper.py`

 * *Files identical despite different names*

### Comparing `jgdv-0.1.0/jgdv/debugging/human.py` & `jgdv-0.1.1/jgdv/debugging/human.py`

 * *Files identical despite different names*

### Comparing `jgdv-0.1.0/jgdv/debugging/malloc.py` & `jgdv-0.1.1/jgdv/debugging/malloc.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,19 +37,19 @@
 logging = logmod.getLogger(__name__)
 ##-- end logging
 
 import tracemalloc
 import linecache
 import fnmatch
 
-class DejaVuMalloc:
+class JGDVMalloc:
     """ see https://docs.python.org/3/library/tracemalloc.html
 
     example:
-    with DejaVuMalloc(2) as dm:
+    with JGDVMalloc(2) as dm:
         dm.whitelist(__file__)
         dm.blacklist("*tracemalloc.py", all_frames=False)
         val = 2
         dm.snapshot("simple")
         vals = [random.random() for x in range(1000)]
         dm.current()
         dm.snapshot("list")
```

### Comparing `jgdv-0.1.0/jgdv/debugging/running_debugger.py` & `jgdv-0.1.1/jgdv/debugging/running_debugger.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import sys
 from bdb import Breakpoint
 from typing import (Any, Callable, ClassVar, Dict, Generic, Iterable, Iterator,
                     List, Mapping, Match, MutableMapping, Optional, Sequence,
                     Set, Tuple, TypeVar, Union, cast)
 
 logging      = logmod.getLogger(__name__)
-trace_logger = logmod.getLogger('dejavu._debug')
+trace_logger = logmod.getLogger('jgdv._debug')
 
 class RunningDebugger(metaclass=SingletonMeta):
     """
       The usual debugger stops execution when you call it.
       This starts the tracing, without pausing execution.
       so on a future breakpoint, you can pause and have a trace from where you started the debugger
     """
```

### Comparing `jgdv-0.1.0/jgdv/debugging/timing.py` & `jgdv-0.1.1/jgdv/debugging/timing.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 #!/usr/bin/env python3
 """
 
-
 See EOF for license/metadata/notes as applicable
 """
 
 ##-- builtin imports
 from __future__ import annotations
 
 # import abc
@@ -33,77 +32,81 @@
 import more_itertools as mitz
 ##-- end lib imports
 
 ##-- logging
 logging = logmod.getLogger(__name__)
 ##-- end logging
 
-
 from time import sleep
 import timeit
 import time
 from random import random
 
-class GroupTime:
+autorange_fmt : Final[str] = "%-*10s : %-*5d calls took: %-*8.2f seconds"
+result_fmt    : Final[str] = "Attempt %-*5d : %-*8.2f seconds"
+block_fmt     : Final[str] = "%-*10s : %-*8.2f seconds"
+once_fmt      : Final[str] = "%-*10s : %-*8.2f seconds"
+
+class JGDVTimer:
     """ Utility Class to time code execution.
 
       see https://docs.python.org/3/library/timeit.html
     """
 
     def __init__(self, count=10, repeat=5, keep_gc=False, group:None|str=None):
         self.level            = level
         self.count            = count
         self.repeat           = repeat
         self.keep_gc          = keep_gc
         self.group : str      = f"{group}::" if group else ""
-        self.total            = 0.0
+        self.total            = 1.0
         self.once_log         = []
 
     def msg(self, str, *args):
         logging.debug(str, *args)
 
     def _set_name(self, name, stmt):
         match name, stmt:
             case str(), _:
                 self.current_name = self.group + name
             case _:
                 self.current_name = self.group + stmt.__qualname__
 
     def autorange_cb(self, number, took):
-        self.msg("%-*10s : %-*5d calls took: %-*8.2f seconds", self.current_name, number, took)
+        self.msg(autorange_fmt, self.current_name, number, took)
         self.total += took
 
     def auto(self, stmt, name=None):
         self._set_name(name, stmt)
         self.msg("-- Autoranging: %s", self.current_name")
         timer = timeit.Timer(stmt, globals=globals())
         timer.autorange(self.autorange_cb)
 
     def repeats(self, stmt, name=None):
         self._set_name(name, stmt)
         self.msg("-- Repeating %s : Timing %s repeats of %s trials", self.current_name, self.repeat, self.count)
         timer  = timeit.Timer(stmt, globals=globals())
         results = timer.repeat(repeat=self.repeat, number=self.count)
         for i, result in enumerate(results):
-            self.msg("Attempt %-*5d : %-*8.2f seconds", i, result)
+            self.msg(result_fmt, i, result)
 
     def block(self, stmt, name=None):
         self._set_name(name, stmt)
         self.msg("-- Running Block %s : Timing block of %-*5f trials", self.current_name, self.count)
         timer  = timeit.Timer(stmt, globals=globals())
         result = timer.timeit(self.count)
-        self.msg("%-*10s : %-*8.2f seconds", self.current_name, result)
+        self.msg(block_fmt, self.current_name, result)
 
     def once(self, stmt, name=None):
         self._set_name(name, stmt)
         self.msg("-- Running Call Once: %s", self.current_name)
         timer  = timeit.Timer(stmt, globals=globals())
         result = timer.timeit(1)
         self.once_log.append((self.current_name, result))
-        self.msg("%-*10s : %-*8.2f seconds", self.current_name, result)
+        self.msg(once_fmt, self.current_name, result)
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, exc_traceback):
         self.msg("-- Finished %s : %-*8.2f", self.group, self.total)
         if self.once_log:
```

### Comparing `jgdv-0.1.0/jgdv/debugging/trace_helper.py` & `jgdv-0.1.1/jgdv/debugging/trace_helper.py`

 * *Files identical despite different names*

### Comparing `jgdv-0.1.0/jgdv/debugging/util.py` & `jgdv-0.1.1/jgdv/debugging/util.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,22 +32,21 @@
 
 ##-- lib imports
 import more_itertools as mitz
 ##-- end lib imports
 
 ##-- logging
 logging = logmod.getLogger(__name__)
-##-- end logging
 printer = logmod.getLogger("doot._printer")
+##-- end logging
 
 import bdb
-import doot
-import doot.errors
 
 def action_debugger(spec, state):
+
     def pstate():
         printer.info("Printing State:")
         printer.info(state)
 
     def pspec():
         printer.info("Printing Spec:")
         printer.info(spec)
@@ -67,9 +66,7 @@
             if target_type != fullname:
                 raise doot.errors.DootActionStateError("Type Error: state.%s : %s != %s", key, fullname, target_type)
 
             printer.debug("Type Matches: state.%s : %s", key, target_type)
 
         except (AttributeError, KeyError):
             raise doot.errors.DootActionStateError("State key missing: %s", key)
-
-
```

### Comparing `jgdv-0.1.0/jgdv/decorators/breakpoint.py` & `jgdv-0.1.1/jgdv/decorators/breakpoint.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,18 +33,18 @@
 import more_itertools as mitz
 ##-- end lib imports
 
 ##-- logging
 logging = logmod.getLogger(__name__)
 ##-- end logging
 
-from jgdv._interfaces.decorator import DejaVuDecorator_i
+from jgdv._interfaces.decorator import JGDVDecorator_i
 from jgdv.debugginer.running_debugger import RunningDebugger
 
-class DejaVuBreakpoint(DejaVuDecorator_i):
+class JGDVBreakpoint(JGDVDecorator_i):
     """
       Decorator to attach a debugger to a function, without pausing execution
     """
 
     def __call__(self, *args, **kwargs):
         # TODO handle repeats
         if args[0].breakpoint:
```

### Comparing `jgdv-0.1.0/jgdv/decorators/check_protocol.py` & `jgdv-0.1.1/jgdv/decorators/check_protocol.py`

 * *Files identical despite different names*

### Comparing `jgdv-0.1.0/jgdv/decorators/destruction.py` & `jgdv-0.1.1/jgdv/decorators/destruction.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,19 +33,22 @@
 import more_itertools as mitz
 ##-- end lib imports
 
 ##-- logging
 logging = logmod.getLogger(__name__)
 ##-- end logging
 
-from jgdv._interfaces.decorator import DejaVuDecorator_i
+from jgdv._interfaces.decorator import JGDVDecorator_i
 
 DEBUG_DESTRUCT_ON = False
 
-class LogDestruction(DejaVuDecorator_i):
+class LogDestruction(JGDVDecorator_i):
+    """
+    A Decorator to log when instances of a class are deleted
+    """
 
     def _debug_del(self):
         """ standalone del logging """
         logging.warning("Deleting: %s", self)
 
     def _debug_del_dec(fn):
         """ wraps existing del method """
```

### Comparing `jgdv-0.1.0/jgdv/decorators/dsl.py` & `jgdv-0.1.1/jgdv/decorators/dsl.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,19 +4,19 @@
                     Iterator, Mapping, Match, MutableMapping, Protocol,
                     Sequence, Tuple, TypeAlias, TypeGuard, TypeVar, cast)
 
 from functools import wraps
 
 ##-- end imports
 
-from jgdv._interfaces.decorator import DejaVuDecorator_i
+from jgdv._interfaces.decorator import JGDVDecorator_i
 
 T = TypeVar('T')
 
-class EnsureDSLInit(DejaVuDecorator_i):
+class EnsureDSLInit(JGDVDecorator_i):
     """ Utility Decorator for DSLs  raising error if not initialised """
 
     def __call__(self, *args, **kwargs):
         if not self._parsers_initialised:
             raise RuntimeError("DSL Not Initialised")
 
         return self._func(self, *args, **kwargs)
```

### Comparing `jgdv-0.1.0/jgdv/decorators/key.py` & `jgdv-0.1.1/jgdv/keys/decorator.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,73 +25,25 @@
                     Protocol, Sequence, Tuple, TypeAlias, TypeGuard, TypeVar,
                     cast, final, overload, runtime_checkable, Generator)
 from uuid import UUID, uuid1
 
 ##-- end builtin imports
 
 ##-- lib imports
-import more_itertools as mitz
+# import more_itertools as mitz
+# from boltons import
 ##-- end lib imports
 
 ##-- logging
 logging = logmod.getLogger(__name__)
 ##-- end logging
 
-import abc
-from collections import UserString
-import string
-from tomlguard import TomlGuard
-import doot
-import doot.errors
-from doot._structs.action_spec import DootActionSpec
-from doot._structs.task_spec import DootTaskSpec
-from doot._structs.artifact import DootTaskArtifact
-from doot._structs.code_ref import DootCodeReference
-
-KEY_PATTERN                                = doot.constants.patterns.KEY_PATTERN
-MAX_KEY_EXPANSIONS                         = doot.constants.patterns.MAX_KEY_EXPANSIONS
-STATE_TASK_NAME_K                          = doot.constants.patterns.STATE_TASK_NAME_K
-
-PATTERN        : Final[re.Pattern]         = re.compile(KEY_PATTERN)
-FAIL_PATTERN   : Final[re.Pattern]         = re.compile("[^a-zA-Z_{}/0-9-]")
-KEYS_HANDLED   : Final[str]                = "_doot_keys_handler"
-ORIG_ARGS      : Final[str]                = "_doot_orig_args"
-KEY_ANNOTS     : Final[str]                = "_doot_keys"
-EXPANSION_HINT : Final[str]                = "_doot_expansion_hint"
-HELP_HINT      : Final[str]                = "_doot_help_hint"
-FUNC_WRAPPED   : Final[str]                = "__wrapped__"
+from jgdv.decorators.base import JGDVBaseDecorator
 
-class _DootKeyGetter:
-    """
-      The core logic to turn a key into a value.
-      Doesn't perform repeated expansions.
-
-      Order it tries:
-      cli -> spec -> state -> locs
-    """
-
-    @staticmethod
-    def get(key:str, spec:None|dict, state:None|dict, locs:None|DootLocations=None) -> Any:
-        cli   : dict          = doot.args.on_fail({}).tasks[str(state.get(STATE_TASK_NAME_K, None))]()
-        replacement           = cli.get(key, None)
-        # *Not* elif's, want it to chain.
-        if replacement is None:
-            replacement = spec.get(key, None)
-        if replacement is None:
-            replacement = state.get(key, None)
-        if replacement is None and locs is not None:
-            match locs.get(key, None):
-                case None:
-                    pass
-                case pl.Path() as x:
-                    replacement = locs.normalize(x)
-
-        return replacement
-
-class KWrapper:
+class KWrapper(JGDVBaseDecorator):
     """ Decorators for actions
     Kwrapper is accessible as DootKey.kwrap
 
     It registers arguments on an action and extracts them from the spec and state automatically.
 
     provides: expands/paths/types/requires/returns/args/kwargs/redirects/redirects_many
 
@@ -163,34 +115,44 @@
                     result &= ((actual == expected) or (actual == f"{expected}_ex"))
 
         return result
 
     @staticmethod
     def _add_key_handler(f):
         """ idempotent key handler so decorated functions dont add unnecessary stack frames """
-        if getattr(f, KEYS_HANDLED, False):
+        if DootDecorator.has_annotations(f):
             return f
 
+        DootDecorator.truncate_signature(f)
+
         match getattr(f, ORIG_ARGS)[0]:
-            case "self":
+            case "self": # The method form handler
 
                 @ftz.wraps(f)
                 def action_expands(self, spec, state, *call_args, **kwargs):
-                    expansions = [x(spec, state) for x in getattr(f, KEY_ANNOTS)]
+                    try:
+                        expansions = [x(spec, state) for x in getattr(f, KEY_ANNOTS)]
+                    except KeyError as err:
+                        printer.warning("Action State Expansion Failure: %s", err)
+                        return False
                     all_args = (*call_args, *expansions)
                     return f(self, spec, state, *all_args, **kwargs)
-            case _:
+            case _: # The function form handler
 
                 @ftz.wraps(f)
                 def action_expands(spec, state, *call_args, **kwargs):
-                    expansions = [x(spec, state) for x in getattr(f, KEY_ANNOTS)]
+                    try:
+                        expansions = [x(spec, state) for x in getattr(f, KEY_ANNOTS)]
+                    except KeyError as err:
+                        printer.warning("Action State Expansion Failure: %s", err)
+                        return False
                     all_args = (*call_args, *expansions)
                     return f(spec, state, *all_args, **kwargs)
 
-        setattr(action_expands, KEYS_HANDLED, True)
+        DootDecorator.annotate(action_expands, {KEYS_HANDLED})
         return action_expands
 
     @staticmethod
     def taskname(f):
         KWrapper._annotate_keys(f, [DootKey.build(STATE_TASK_NAME_K, exp_hint="type")])
         return KWrapper._add_key_handler(f)
 
@@ -294,8 +256,7 @@
         keys = [DootKey.build(x, exp_hint=exp_hint, **kwargs) for x in args]
 
         def expand_wrapper(f):
             KWrapper._annotate_keys(f, keys)
             return KWrapper._add_key_handler(f)
 
         return expand_wrapper
-
```

### Comparing `jgdv-0.1.0/jgdv/decorators/logging.py` & `jgdv-0.1.1/jgdv/decorators/logging.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,26 +15,26 @@
 from typing import TYPE_CHECKING
 if TYPE_CHECKING:
     # tc only imports
     pass
 
 ##-- end imports
 
-from jgdv._interfaces.decorator import DejaVuDecorator_i
+from jgdv._interfaces.decorator import JGDVDecorator_i
 
-class LogReturn(DejaVuDelayDecorator_i):
+class LogReturn(JGDVDelayDecorator_i):
     """
     Utility Decorator to log a functions return value at a set level
     """
 
     def __init__(self, prefix, level=logmod.DEBUG, msg=None, logger=None):
         super().__init__()
         self._prefix = prefix
         self._level  = level
         self._msg    =  msg or "{prefix} result: {result}"
-        self._logger = logger or logmod.getLogger("dejavu._returns")
+        self._logger = logger or logmod.getLogger("jgdv._returns")
 
     def _wrapper(self, *args, **kwargs):
         result = self._func(*args, **kwargs)
         log_msg = self._msg.format(prefix=self._prefix, result=result)
         self._logger.log(level, log_msg)
         return result
```

### Comparing `jgdv-0.1.0/jgdv/decorators/util.py` & `jgdv-0.1.1/jgdv/decorators/util.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,24 +9,17 @@
 from enum import Enum
 from functools import wraps
 from typing import (TYPE_CHECKING, Any, Callable, ClassVar, Dict, Generic,
                     Iterable, Iterator, List, Mapping, Match, MutableMapping,
                     Optional, ParamSpec, Sequence, Set, Tuple, TypeAlias,
                     TypeVar, Union, cast)
 
-logging = logmod.getLogger(__name__)
-
-from acab_config.utils.decorators import registerOn
-
-if TYPE_CHECKING:
-    # tc only imports
-    from acab import types as AT
-
 ##-- end imports
 
+logging = logmod.getLogger(__name__)
 T = TypeVar('T')
 P = ParamSpec('P')
 
 def ForceListArgDecorator(f:Callable[..., T]) -> Callable[..., T]:
     """ Force the first arg to be a list """
 
     @wraps(f)
```

### Comparing `jgdv-0.1.0/jgdv/dsl/consts.py` & `jgdv-0.1.1/jgdv/dsl/consts.py`

 * *Files identical despite different names*

### Comparing `jgdv-0.1.0/jgdv/dsl/ctors.py` & `jgdv-0.1.1/jgdv/dsl/ctors.py`

 * *Files identical despite different names*

### Comparing `jgdv-0.1.0/jgdv/dsl/funcs.py` & `jgdv-0.1.1/jgdv/dsl/funcs.py`

 * *Files identical despite different names*

### Comparing `jgdv-0.1.0/jgdv/dsl/util.py` & `jgdv-0.1.1/jgdv/dsl/util.py`

 * *Files identical despite different names*

### Comparing `jgdv-0.1.0/jgdv/files/binary/infinity.py` & `jgdv-0.1.1/jgdv/files/binary/infinity.py`

 * *Files identical despite different names*

### Comparing `jgdv-0.1.0/jgdv/files/bookmarks/bookmark.py` & `jgdv-0.1.1/jgdv/files/bookmarks/bookmark.py`

 * *Files identical despite different names*

### Comparing `jgdv-0.1.0/jgdv/files/bookmarks/collection.py` & `jgdv-0.1.1/jgdv/files/bookmarks/collection.py`

 * *Files identical despite different names*

### Comparing `jgdv-0.1.0/jgdv/files/bookmarks/netscape.py` & `jgdv-0.1.1/jgdv/files/bookmarks/netscape.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 from __future__ import annotations
 
 import logging
 
 ##-- end imports
 
 from bs4 import BeautifulSoup
-from doot.utils.formats.bookmarks import Bookmark, BookmarkCollection
 
 class NetscapeLoader:
 
     @staticmethod
     def read_netscape(path:pl.Path):
         logging.info('Starting html opener for: %s', path)
         with open(path, 'rb') as f:
```

### Comparing `jgdv-0.1.0/jgdv/files/epub/epub.py` & `jgdv-0.1.1/jgdv/files/epub/epub.py`

 * *Files identical despite different names*

### Comparing `jgdv-0.1.0/jgdv/files/gif/gif_mixin.py` & `jgdv-0.1.1/jgdv/files/gif/gif_mixin.py`

 * *Files identical despite different names*

### Comparing `jgdv-0.1.0/jgdv/files/gif/make_gif.py` & `jgdv-0.1.1/jgdv/files/gif/make_gif.py`

 * *Files identical despite different names*

### Comparing `jgdv-0.1.0/jgdv/files/graph/pickles.py` & `jgdv-0.1.1/jgdv/files/graph/pickles.py`

 * *Files identical despite different names*

### Comparing `jgdv-0.1.0/jgdv/files/json.py` & `jgdv-0.1.1/jgdv/files/json.py`

 * *Files 7% similar despite different names*

```diff
@@ -41,19 +41,14 @@
 import math
 import json
 from time import sleep
 import sh
 import shutil
 import jsonlines
 import tomlguard as TG
-import doot
-from doot.errors import DootTaskError, DootTaskFailed
-from doot.enums import ActionResponseEnum
-from doot._abstract import Action_p
-from doot.structs import DootKey
 
 ##-- expansion keys
 FROM_KEY           : Final[DootKey] = DootKey.make("from")
 UPDATE             : Final[DootKey] = DootKey.make("update_")
 ##-- end expansion keys
 
 class ReadJson(Action_p):
```

### Comparing `jgdv-0.1.0/jgdv/files/mem_map.py` & `jgdv-0.1.1/jgdv/files/mem_map.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
 ##-- logging
 logging = logmod.getLogger(__name__)
 ##-- end logging
 
 import mmap
 
-class DejaVuMemMap:
+class JGDVMemMap:
     """
       A utility wrapper to easily make memory mapped files from a path,
       and use them as in a context manager
     """
 
     def __init__(self, path:pl.Path):
         self._path = path
```

### Comparing `jgdv-0.1.0/jgdv/files/metadata.py` & `jgdv-0.1.1/jgdv/files/metadata.py`

 * *Files identical despite different names*

### Comparing `jgdv-0.1.0/jgdv/files/org/base.py` & `jgdv-0.1.1/jgdv/files/org/base.py`

 * *Files identical despite different names*

### Comparing `jgdv-0.1.0/jgdv/files/org/drawer.py` & `jgdv-0.1.1/jgdv/files/org/drawer.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 import more_itertools as mitz
 ##-- end lib imports
 
 ##-- logging
 logging = logmod.getLogger(__name__)
 ##-- end logging
 
-from dejavu.files.org.base import OrgBuilderBase
+from jgdv.files.org.base import OrgBuilderBase
 
 @dataclass
 class OrgDrawerBuilder(OrgBuilderBase):
     """
     A lazily build org drawer container,
     which aligns values in the block
     """
```

### Comparing `jgdv-0.1.0/jgdv/files/org/file.py` & `jgdv-0.1.1/jgdv/files/org/file.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,16 +33,16 @@
 import more_itertools as mitz
 ##-- end lib imports
 
 ##-- logging
 logging = logmod.getLogger(__name__)
 ##-- end logging
 
-from dejavu.files.org.base import OrgBuilderBase
-from dejavu.files.org.drawer import OrgDrawerBuilder
+from jgdv.files.org.base import OrgBuilderBase
+from jgdv.files.org.drawer import OrgDrawerBuilder
 
 @dataclass
 class OrgStrBuilder(OrgBuilderBase):
     """
     Utility class for building Org files
     """
     output : List[Union[str, 'OrgBuilderBase']] = field(default_factory=list)
```

### Comparing `jgdv-0.1.0/jgdv/files/pdf/pdf.py` & `jgdv-0.1.1/jgdv/files/pdf/pdf.py`

 * *Files identical despite different names*

### Comparing `jgdv-0.1.0/jgdv/files/sha256.py` & `jgdv-0.1.1/jgdv/files/twitter/base.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,44 +1,38 @@
 #!/usr/bin/env python3
 """
 
-See EOF for license/metadata/notes as applicable
 """
-
-##-- builtin imports
+##-- imports
 from __future__ import annotations
 
-# import abc
+import abc
 import datetime
 import enum
 import functools as ftz
 import itertools as itz
 import logging as logmod
 import pathlib as pl
 import re
 import time
 import types
-import weakref
-# from copy import deepcopy
-# from dataclasses import InitVar, dataclass, field
+from copy import deepcopy
+from dataclasses import InitVar, dataclass, field
 from typing import (TYPE_CHECKING, Any, Callable, ClassVar, Final, Generic,
                     Iterable, Iterator, Mapping, Match, MutableMapping,
                     Protocol, Sequence, Tuple, TypeAlias, TypeGuard, TypeVar,
-                    cast, final, overload, runtime_checkable, Generator)
+                    cast, final, overload, runtime_checkable)
 from uuid import UUID, uuid1
+from weakref import ref
 
-##-- end builtin imports
-
-##-- lib imports
-import more_itertools as mitz
-##-- end lib imports
+##-- end imports
 
 ##-- logging
 logging = logmod.getLogger(__name__)
 ##-- end logging
 
-from hashlib import sha256
 
-def file_to_hash(filename):
-    path = pl.Path(filename)
-    assert(path.exists())
-    return sha256(path.read_bytes()).hexdigest()
+class HtmlThreadWriter:
+
+    @staticmethod
+    def build(thread, tweets, users, tags):
+        pass
```

### Comparing `jgdv-0.1.0/jgdv/files/tags/base.py` & `jgdv-0.1.1/jgdv/files/tags/base.py`

 * *Files identical despite different names*

### Comparing `jgdv-0.1.0/jgdv/files/tags/graph.py` & `jgdv-0.1.1/jgdv/files/tags/graph.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,19 +9,18 @@
 import logging as logmod
 import re
 from dataclasses import dataclass, field
 from typing import (Any, Callable, ClassVar, Dict, Generic, Iterable, Iterator,
                     List, Mapping, Match, MutableMapping, Optional, Sequence,
                     Set, Tuple, TypeVar, Union, cast, Final, TypeAlias)
 import re
-import networkx as nx
-from doot.utils.formats.bookmarks import BookmarkCollection
-from doot.utils.formats.tagfile import TagFile
 ##-- end imports
 
+import networkx as nx
+
 logging = logmod.getLogger(__name__)
 
 IGNORE_REPLACEMENTS = ["TO_CHECK"]
 
 TAG_NORM    : Final[re.Pattern] = regex.compile(" +")
 ORG_PATTERN : Final[str]        = r"^\*\*\s+.+?\s+:(\S+):$"
 ORG_SEP     : Final[str]        = ":"
```

### Comparing `jgdv-0.1.0/jgdv/files/tags/index.py` & `jgdv-0.1.1/jgdv/files/tags/index.py`

 * *Files 7% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 import more_itertools as mitz
 ##-- end lib imports
 
 ##-- logging
 logging = logmod.getLogger(__name__)
 ##-- end logging
 
-from dejavu.files_formats.tags.base import TagFile
+from jgdv.files_formats.tags.base import TagFile
 
 @dataclass
 class IndexFile(TagFile):
     """ Utility class for index file specification and writing """
 
     mapping : Dict[str, Set[pl.Path]] = field(default_factory=lambda: defaultdict(set))
     ext     : str                 = field(default=".index")
```

### Comparing `jgdv-0.1.0/jgdv/files/tags/substitutions.py` & `jgdv-0.1.1/jgdv/files/tags/substitutions.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 import more_itertools as mitz
 ##-- end lib imports
 
 ##-- logging
 logging = logmod.getLogger(__name__)
 ##-- end logging
 
-from dejavu.files_formats.tags.base import TagFile
+from jgdv.files_formats.tags.base import TagFile
 
 @dataclass
 class SubstitutionFile(TagFile):
     """ SubstitutionFiles add a replacement tag for some tags """
 
     ext           : str                  = field(default=".sub")
     substitutions : Dict[str, set[str]] = field(default_factory=lambda: defaultdict(set))
```

### Comparing `jgdv-0.1.0/jgdv/files/tar.py` & `jgdv-0.1.1/jgdv/files/tar.py`

 * *Files 23% similar despite different names*

```diff
@@ -38,20 +38,15 @@
 
 printer = logmod.getLogger("doot._printer")
 
 from time import sleep
 import sh
 import shutil
 import tomlguard as TG
-import doot
-from doot.errors import DootTaskError, DootTaskFailed
-from doot.enums import ActionResponseEnum
-from doot._abstract import Action_p
-from doot.structs import DootKey
-from doot.actions.postbox import _DootPostBox
+import jgdv
 
 ##-- expansion keys
 TO_KEY             : Final[DootKey] = DootKey.make("to")
 FROM_KEY           : Final[DootKey] = DootKey.make("from")
 UPDATE             : Final[DootKey] = DootKey.make("update_")
 PROMPT             : Final[DootKey] = DootKey.make("prompt")
 PATTERN            : Final[DootKey] = DootKey.make("pattern")
@@ -63,15 +58,15 @@
 LAX                : Final[DootKey] = DootKey.make("lax")
 ##-- end expansion keys
 
 COMP_TAR_CMD  = sh.tar.bake("-cf", "-")
 COMP_GZIP_CMD = sh.gzip.bake("--best")
 DECOMP_CMD    = sh.tar.bake("-xf")
 
-@doot.check_protocol
+@jgdv.check_protocol
 class TarCompressAction(Action_p):
     """ Compresses a target into a .tar.gz file """
 
     @DootKey.kwrap.paths("file")
     @DootKey.kwrap.paths("to", hint={"on_fail":None})
     def __call__(self, spec, state, file, to):
         target = file
@@ -80,30 +75,30 @@
         if output.exists():
             raise doot.errors.DootActionError("Compression target already exists")
         if target.is_dir():
             COMP_GZIP_CMD(_in=COMP_TAR_CMD("-C", target, ".", _piped=True), _out=output)
         else:
             COMP_GZIP_CMD(_in=COMP_TAR_CMD("-C", target.parent, target.name, _piped=True), _out=output)
 
-@doot.check_protocol
+@jgdv.check_protocol
 class TarDecompressAction(Action_p):
     """ Decompresses a .tar.gz file """
 
     @DootKey.kwrap.paths("file", "to")
     def __call__(self, spec, state, file, to):
         target = file
         output = to
         if not ".tar.gz" in target.name:
             printer.warning("Decompression target isn't a .tar.gz", target)
             return ActionResponseEnum.FAIL
 
         DECOMP_CMD(target, "-C", output)
 
 
-@doot.check_protocol
+@jgdv.check_protocol
 class TarListAction(Action_p):
     """ List the contents of a tar archive """
 
     @DootKey.kwrap.paths("from")
     @DootKey.kwrap.redirects("update_")
     def __call__(self, spec, state, _from, _update):
         target = _from
```

### Comparing `jgdv-0.1.0/jgdv/files/tex/base.py` & `jgdv-0.1.1/jgdv/files/tex/base.py`

 * *Files identical despite different names*

### Comparing `jgdv-0.1.0/jgdv/files/tex/bib.py` & `jgdv-0.1.1/jgdv/files/timeline/reader.py`

 * *Files 10% similar despite different names*

```diff
@@ -32,12 +32,7 @@
 ##-- lib imports
 import more_itertools as mitz
 ##-- end lib imports
 
 ##-- logging
 logging = logmod.getLogger(__name__)
 ##-- end logging
-
-from dejavu.files.tex.base import TexStatement_i
-
-class TexBib(TexStatement_i):
-    pass
```

### Comparing `jgdv-0.1.0/jgdv/files/tex/envs.py` & `jgdv-0.1.1/jgdv/files/tex/envs.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 import more_itertools as mitz
 ##-- end lib imports
 
 ##-- logging
 logging = logmod.getLogger(__name__)
 ##-- end logging
 
-from dejavu.files.tex.base import TexStatement_i, TexEnvironment_i
+from jgdv.files.tex.base import TexStatement_i, TexEnvironment_i
 
 class TexFigure(TexEnvironment_i):
     pass
 
 class TexEquation(TexEnvironment_i):
     pass
```

### Comparing `jgdv-0.1.0/jgdv/files/tex/gantt.py` & `jgdv-0.1.1/jgdv/files/tex/gantt.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,17 +3,14 @@
 from __future__ import annotations
 
 import logging as logmod
 from collections import defaultdict
 from importlib.resources import files
 from string import Template, ascii_uppercase
 
-from instal.defaults import STATE_HOLDSAT_GROUPS, TEX_loc
-from instal.interfaces.reporter import InstalReporter_i
-
 ##-- end imports
 
 ##-- logging
 logging = logmod.getLogger(__name__)
 ##-- end logging
 
 ##-- data
@@ -24,24 +21,25 @@
 GANTT_MILESTONE = Template((tex_path / "gantt_milestone.tex").read_text())
 GANTT_PRELUDE   = Template((tex_path / "gantt_prelude.tex").read_text())
 
 TERM            = Template((tex_path / "term.tex").read_text())
 TERM_BODY       = Template((tex_path / "term_body.tex").read_text())
 ##-- end data
 
-from dejavu.files.tex.base import TexBuilder_i
+from jgdv.files.tex.base import TexBuilder_i
 
 class GanttTexBuilder(TexBuilder_i):
     """
     InstalGanttTracer
     Implementation of Reporter for gantt output.
 
     Milestones are events
     Bars are fluents
     """
+
     def header(self):
         pass
 
     def footer(self):
         pass
 
     def prepare2(self):
@@ -60,16 +58,14 @@
                 "{{{t}}}\n".format(t=len(observed) + 1), file=tfile)
             i = facts[f][0]
             l = (str(f.arguments[0]) + ": " +
                     str(f.arguments[1])).replace('_', '\_')
             print("\\ganttbar{{{label}}}{{{start}}}{{{finish}}}"
                     .format(label=l, start=i, finish=i), file=tfile)
 
-
-
     def render_term(self, term, inst=None) -> str:
         """
         Render a passed in ASTTerm into a useable latex string.
         Adapts to handle institutional terms and non.
         """
         body = ""
         if bool(term.params):
@@ -92,23 +88,20 @@
         {holding}, {initiated}, and {terminated} sets.
 
         """
         init   = {self.render_term(x.params[0]) for x in state.fluents if prior_state is None or x not in prior_state}
         holds  = {self.render_term(x.params[0]) for x in prior_state.fluents if x in state} if prior_state is not None else {}
         termin = {self.render_term(x.params[0]) for x in prior_state.fluents if x not in state} if prior_state is not None else {}
 
-
         init_render   = {self.expand(FLUENT, mod=BOLD,  term=term).strip() for term in init}
         holds_render  = {self.expand(FLUENT, mod="",    term=term).strip() for term in holds}
         termin_render = {self.expand(FLUENT, mod=SOUT, term=term).strip() for term in termin}
 
-
         return sorted(init_render), sorted(holds_render), sorted(termin_render)
 
-
     def render_milestones(self, trace, title="Observed Events", caption="Tracking the events in the trace") -> str:
         """
         Convert the trace to a gantt chart of milestones,
         where each milestone is an event observed in the trace
         """
         content = []
 
@@ -169,14 +162,15 @@
             f_trace    = trace.filter(allow=[inst], reject=rejections)
             inst_chart = self.render_bars(f_trace,
                                           title=f"{inst} Fluents",
                                           caption=f"Fluent Lives in institution {inst}")
             charts.append(inst_chart)
 
         return charts
+
     def trace_to_file(self, trace, path):
         self.clear()
         all_gantts = []
         # build event gantt
         all_gantts.append(self.render_milestones(trace))
         # build fluent gantt
         all_gantts.append(self.render_bars(trace))
```

### Comparing `jgdv-0.1.0/jgdv/files/tex/pdf.py` & `jgdv-0.1.1/jgdv/files/tex/pdf.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,16 +3,14 @@
 from __future__ import annotations
 
 import logging as logmod
 from collections import defaultdict
 from importlib.resources import files
 from string import Template, ascii_uppercase
 
-from instal.defaults import STATE_HOLDSAT_GROUPS, TEX_loc
-from instal.interfaces.reporter import InstalReporter_i
 ##-- end imports
 
 ##-- logging
 logging = logmod.getLogger(__name__)
 ##-- end logging
 
 ##-- data
@@ -39,16 +37,15 @@
 
 FLUENT          = Template((tex_path / "fluent.tex").read_text())
 INST_TERM       = Template((tex_path / "inst_term.tex").read_text())
 TERM            = Template((tex_path / "term.tex").read_text())
 TERM_BODY       = Template((tex_path / "term_body.tex").read_text())
 ##-- end data
 
-
-class InstalPDFReporter(InstalReporter_i):
+class PDFReporter:
     """
         InstalPDFTracer
         Implementation of ABC InstalTracer for pdf output.
     """
 
     def render_term(self, term, inst=None) -> str:
         """
```

### Comparing `jgdv-0.1.0/jgdv/files/tex/statements.py` & `jgdv-0.1.1/jgdv/files/tex/statements.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 import more_itertools as mitz
 ##-- end lib imports
 
 ##-- logging
 logging = logmod.getLogger(__name__)
 ##-- end logging
 
-from dejavu.files.tex.base import TexStatement_i
+from jgdv.files.tex.base import TexStatement_i
 
 class TexQuote(TexStatement_i):
     pass
 
 class TexFootNote(TexStatement_i):
     pass
```

### Comparing `jgdv-0.1.0/jgdv/files/tex/util.py` & `jgdv-0.1.1/jgdv/files/tex/util.py`

 * *Files identical despite different names*

### Comparing `jgdv-0.1.0/jgdv/files/timeline/entry.py` & `jgdv-0.1.1/jgdv/files/timeline/entry.py`

 * *Files identical despite different names*

### Comparing `jgdv-0.1.0/jgdv/files/timeline/reader.py` & `jgdv-0.1.1/jgdv/files/timeline/writer.py`

 * *Files identical despite different names*

### Comparing `jgdv-0.1.0/jgdv/files/timeline/timeline.py` & `jgdv-0.1.1/jgdv/files/timeline/timeline.py`

 * *Files identical despite different names*

### Comparing `jgdv-0.1.0/jgdv/files/timeline/writer.py` & `jgdv-0.1.1/jgdv/structs/rete/alpha.py`

 * *Files identical despite different names*

### Comparing `jgdv-0.1.0/jgdv/files/twitter/__test/component_example.json` & `jgdv-0.1.1/jgdv/files/twitter/__test/component_example.json`

 * *Files identical despite different names*

### Comparing `jgdv-0.1.0/jgdv/files/twitter/__test/test_file_processing.py` & `jgdv-0.1.1/jgdv/files/twitter/__test/test_file_processing.py`

 * *Files identical despite different names*

### Comparing `jgdv-0.1.0/jgdv/files/twitter/__test/tweet_example.json` & `jgdv-0.1.1/jgdv/files/twitter/__test/tweet_example.json`

 * *Files identical despite different names*

### Comparing `jgdv-0.1.0/jgdv/files/twitter/__test/user_example.json` & `jgdv-0.1.1/jgdv/files/twitter/__test/user_example.json`

 * *Files identical despite different names*

### Comparing `jgdv-0.1.0/jgdv/files/twitter/base.py` & `jgdv-0.1.1/jgdv/geom/dcel/dcel.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,38 +1,41 @@
 #!/usr/bin/env python3
 """
 
+
+See EOF for license/metadata/notes as applicable
 """
-##-- imports
+
+##-- builtin imports
 from __future__ import annotations
 
-import abc
+# import abc
 import datetime
 import enum
 import functools as ftz
 import itertools as itz
 import logging as logmod
 import pathlib as pl
 import re
 import time
 import types
-from copy import deepcopy
-from dataclasses import InitVar, dataclass, field
+import weakref
+# from copy import deepcopy
+# from dataclasses import InitVar, dataclass, field
 from typing import (TYPE_CHECKING, Any, Callable, ClassVar, Final, Generic,
                     Iterable, Iterator, Mapping, Match, MutableMapping,
                     Protocol, Sequence, Tuple, TypeAlias, TypeGuard, TypeVar,
-                    cast, final, overload, runtime_checkable)
+                    cast, final, overload, runtime_checkable, Generator)
 from uuid import UUID, uuid1
-from weakref import ref
 
-##-- end imports
+##-- end builtin imports
+
+##-- lib imports
+import more_itertools as mitz
+##-- end lib imports
 
 ##-- logging
 logging = logmod.getLogger(__name__)
 ##-- end logging
 
-
-class HtmlThreadWriter:
-
-    @staticmethod
-    def build(thread, tweets, users, tags):
-        pass
+class DCEL:
+    pass
```

### Comparing `jgdv-0.1.0/jgdv/files/twitter/mixin_passes.py` & `jgdv-0.1.1/jgdv/files/twitter/mixin_passes.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,24 +9,18 @@
 import uuid
 from collections import defaultdict
 from shutil import copyfile, rmtree
 from typing import (Any, Callable, ClassVar, Dict, Generic, Iterable, Iterator,
                     List, Mapping, Match, MutableMapping, Optional, Sequence,
                     Set, Tuple, TypeVar, Union, cast)
 
-import networkx as nx
-from doot.utils.twitter.html_writer import HtmlThreadWriter
-from doot.utils.twitter.lazy_component_writer import LazyComponentWriter
-from doot.utils.twitter.org_writer import OrgThreadWriter
-from doot.utils.twitter.thread_obj import TwitterThreadObj
-from doot.utils.twitter.todo_list import TweetTodoFile
-from doot.utils.twitter.tweet_graph import TwitterGraph
-
 ##-- end imports
 
+import networkx as nx
+
 logging = root_logger.getLogger(__name__)
 
 REPLY  : Final[str] = 'in_reply_to_status_id_str'
 QUOTE  : Final[str] = 'quoted_status_id_str'
 ID_STR : Final[str] = 'id_str'
 
 # TODO could refactor output into template files, ie: jinja.
```

### Comparing `jgdv-0.1.0/jgdv/files/twitter/structs/thread.py` & `jgdv-0.1.1/jgdv/files/twitter/structs/thread.py`

 * *Files identical despite different names*

### Comparing `jgdv-0.1.0/jgdv/files/twitter/structs/todo_list.py` & `jgdv-0.1.1/jgdv/files/twitter/structs/todo_list.py`

 * *Files identical despite different names*

### Comparing `jgdv-0.1.0/jgdv/files/twitter/structs/tweet.py` & `jgdv-0.1.1/jgdv/files/twitter/structs/tweet.py`

 * *Files identical despite different names*

### Comparing `jgdv-0.1.0/jgdv/files/twitter/tweet_graph.py` & `jgdv-0.1.1/jgdv/files/twitter/tweet_graph.py`

 * *Files identical despite different names*

### Comparing `jgdv-0.1.0/jgdv/files/twitter/util.py` & `jgdv-0.1.1/jgdv/files/twitter/util.py`

 * *Files identical despite different names*

### Comparing `jgdv-0.1.0/jgdv/files/twitter/writers/json_component.py` & `jgdv-0.1.1/jgdv/files/twitter/writers/json_component.py`

 * *Files identical despite different names*

### Comparing `jgdv-0.1.0/jgdv/files/twitter/writers/lazy_json_component.py` & `jgdv-0.1.1/jgdv/files/twitter/writers/lazy_json_component.py`

 * *Files identical despite different names*

### Comparing `jgdv-0.1.0/jgdv/files/twitter/writers/thread.py` & `jgdv-0.1.1/jgdv/files/twitter/writers/thread.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,16 +33,16 @@
 ##-- end lib imports
 
 ##-- logging
 logging = logmod.getLogger(__name__)
 ##-- end logging
 
 import networkx as nx
-from dejavu.files.org.file import OrgStrBuilder
-from dejavu.files.twitter.writers.util import parse_date
+from jgdv.files.org.file import OrgStrBuilder
+from jgdv.files.twitter.writers.util import parse_date
 
 media_dict : Final[Callable] = lambda: defaultdict(list)
 
 @dataclass
 class OrgThreadWriter:
     """ Given a thread object, build a string representation for it
     redirecting absolute media paths to relative
```

### Comparing `jgdv-0.1.0/jgdv/files/twitter/writers/tweet.py` & `jgdv-0.1.1/jgdv/files/twitter/writers/tweet.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 ##-- end lib imports
 
 ##-- logging
 logging = logmod.getLogger(__name__)
 ##-- end logging
 
 from collections import defaultdict
-from dejavu.files.twitter.writers.util import parse_date
+from jgdv.files.twitter.writers.util import parse_date
 
 media_dict : Final[Callable] = lambda: defaultdict(list)
 
 @dataclass
 class TwitterTweet:
     id_s         : str
     base_user    : str
```

### Comparing `jgdv-0.1.0/jgdv/files/twitter/writers/users_table.py` & `jgdv-0.1.1/jgdv/files/twitter/writers/users_table.py`

 * *Files identical despite different names*

### Comparing `jgdv-0.1.0/jgdv/files/twitter/writers/util.py` & `jgdv-0.1.1/jgdv/files/twitter/writers/util.py`

 * *Files identical despite different names*

### Comparing `jgdv-0.1.0/jgdv/files/zip.py` & `jgdv-0.1.1/jgdv/files/zip.py`

 * *Files identical despite different names*

### Comparing `jgdv-0.1.0/jgdv/geom/dcel/constants.py` & `jgdv-0.1.1/jgdv/geom/dcel/constants.py`

 * *Files identical despite different names*

### Comparing `jgdv-0.1.0/jgdv/geom/dcel/dcel.py` & `jgdv-0.1.1/jgdv/structs/rete/beta.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,10 +32,7 @@
 ##-- lib imports
 import more_itertools as mitz
 ##-- end lib imports
 
 ##-- logging
 logging = logmod.getLogger(__name__)
 ##-- end logging
-
-class DCEL:
-    pass
```

### Comparing `jgdv-0.1.0/jgdv/geom/dcel/io/drawing.py` & `jgdv-0.1.1/jgdv/geom/dcel/io/drawing.py`

 * *Files identical despite different names*

### Comparing `jgdv-0.1.0/jgdv/geom/dcel/io/export.py` & `jgdv-0.1.1/jgdv/geom/dcel/io/export.py`

 * *Files identical despite different names*

### Comparing `jgdv-0.1.0/jgdv/geom/dcel/mod/adding.py` & `jgdv-0.1.1/jgdv/geom/dcel/mod/adding.py`

 * *Files identical despite different names*

### Comparing `jgdv-0.1.0/jgdv/geom/dcel/mod/processing.py` & `jgdv-0.1.1/jgdv/geom/dcel/mod/processing.py`

 * *Files identical despite different names*

### Comparing `jgdv-0.1.0/jgdv/geom/dcel/mod/subtracting.py` & `jgdv-0.1.1/jgdv/geom/dcel/mod/subtracting.py`

 * *Files identical despite different names*

### Comparing `jgdv-0.1.0/jgdv/geom/dcel/structs/draw_settings.py` & `jgdv-0.1.1/jgdv/geom/dcel/structs/draw_settings.py`

 * *Files identical despite different names*

### Comparing `jgdv-0.1.0/jgdv/geom/dcel/structs/drawable.py` & `jgdv-0.1.1/jgdv/geom/dcel/structs/drawable.py`

 * *Files identical despite different names*

### Comparing `jgdv-0.1.0/jgdv/geom/dcel/structs/face.py` & `jgdv-0.1.1/jgdv/geom/dcel/structs/face.py`

 * *Files identical despite different names*

### Comparing `jgdv-0.1.0/jgdv/geom/dcel/structs/halfedge.py` & `jgdv-0.1.1/jgdv/geom/dcel/structs/halfedge.py`

 * *Files identical despite different names*

### Comparing `jgdv-0.1.0/jgdv/geom/dcel/structs/line.py` & `jgdv-0.1.1/jgdv/geom/dcel/structs/line.py`

 * *Files identical despite different names*

### Comparing `jgdv-0.1.0/jgdv/geom/dcel/structs/state.py` & `jgdv-0.1.1/jgdv/geom/dcel/structs/state.py`

 * *Files identical despite different names*

### Comparing `jgdv-0.1.0/jgdv/geom/dcel/structs/vertex.py` & `jgdv-0.1.1/jgdv/geom/dcel/structs/vertex.py`

 * *Files identical despite different names*

### Comparing `jgdv-0.1.0/jgdv/geom/intersection/result.py` & `jgdv-0.1.1/jgdv/geom/intersection/result.py`

 * *Files identical despite different names*

### Comparing `jgdv-0.1.0/jgdv/geom/intersection/state.py` & `jgdv-0.1.1/jgdv/geom/intersection/state.py`

 * *Files identical despite different names*

### Comparing `jgdv-0.1.0/jgdv/geom/intersection/sweep.py` & `jgdv-0.1.1/jgdv/geom/intersection/sweep.py`

 * *Files identical despite different names*

### Comparing `jgdv-0.1.0/jgdv/geom/math/bbox.py` & `jgdv-0.1.1/jgdv/geom/math/bbox.py`

 * *Files identical despite different names*

### Comparing `jgdv-0.1.0/jgdv/geom/math/circles.py` & `jgdv-0.1.1/jgdv/geom/math/circles.py`

 * *Files identical despite different names*

### Comparing `jgdv-0.1.0/jgdv/geom/math/direction.py` & `jgdv-0.1.1/jgdv/geom/math/direction.py`

 * *Files identical despite different names*

### Comparing `jgdv-0.1.0/jgdv/geom/math/distance.py` & `jgdv-0.1.1/jgdv/geom/math/distance.py`

 * *Files identical despite different names*

### Comparing `jgdv-0.1.0/jgdv/geom/math/heightmap.py` & `jgdv-0.1.1/jgdv/geom/math/heightmap.py`

 * *Files identical despite different names*

### Comparing `jgdv-0.1.0/jgdv/geom/math/lines.py` & `jgdv-0.1.1/jgdv/geom/math/lines.py`

 * *Files identical despite different names*

### Comparing `jgdv-0.1.0/jgdv/geom/math/movement.py` & `jgdv-0.1.1/jgdv/geom/math/movement.py`

 * *Files identical despite different names*

### Comparing `jgdv-0.1.0/jgdv/geom/voronoi/beachline.py` & `jgdv-0.1.1/jgdv/geom/voronoi/beachline.py`

 * *Files identical despite different names*

### Comparing `jgdv-0.1.0/jgdv/geom/voronoi/breakpoint.py` & `jgdv-0.1.1/jgdv/geom/voronoi/breakpoint.py`

 * *Files identical despite different names*

### Comparing `jgdv-0.1.0/jgdv/geom/voronoi/data.py` & `jgdv-0.1.1/jgdv/geom/voronoi/data.py`

 * *Files identical despite different names*

### Comparing `jgdv-0.1.0/jgdv/geom/voronoi/drawing.py` & `jgdv-0.1.1/jgdv/geom/voronoi/drawing.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 """
 ##-- imports
 from __future__ import annotations
 import logging as root_logger
 from math import nan
 from os.path import isdir, join
 import numpy as np
-import cuty as utils
 
 ##-- end imports
 
 logging = root_logger.getLogger(__name__)
 
 #Constants:
 COLOUR                    = [0.2, 0.1, 0.6, 1.0]
```

### Comparing `jgdv-0.1.0/jgdv/geom/voronoi/events.py` & `jgdv-0.1.1/jgdv/geom/voronoi/events.py`

 * *Files identical despite different names*

### Comparing `jgdv-0.1.0/jgdv/geom/voronoi/graph.py` & `jgdv-0.1.1/jgdv/geom/voronoi/graph.py`

 * *Files identical despite different names*

### Comparing `jgdv-0.1.0/jgdv/geom/voronoi/line_sweep.py` & `jgdv-0.1.1/jgdv/geom/voronoi/line_sweep.py`

 * *Files identical despite different names*

### Comparing `jgdv-0.1.0/jgdv/geom/voronoi/process.py` & `jgdv-0.1.1/jgdv/geom/voronoi/process.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 #!/usr/bin/env python3
 """
 
-<<<<<<<< HEAD:cuty/voronoi/process.py
 """
 ##-- imports
 from __future__ import annotations
 
 import types
 import abc
 import datetime
@@ -20,23 +19,14 @@
 from dataclasses import InitVar, dataclass, field
 from typing import (TYPE_CHECKING, Any, Callable, ClassVar, Final, Generic,
                     Iterable, Iterator, Mapping, Match, MutableMapping,
                     Protocol, Sequence, Tuple, TypeAlias, TypeGuard, TypeVar,
                     cast, final, overload, runtime_checkable)
 from uuid import UUID, uuid1
 from weakref import ref
-========
-import cuty as utils
-from cuty import Parabola
-from cuty import rbtree
-from cuty.rbtree.comparison_functions import arc_comparison, Directions, arc_equality
-
-from cuty.dcel import DCEL, HalfEdge
-from cuty.umath import get_distance_raw, bound_line_in_bbox, isClockwise, bbox_centre
->>>>>>>> b18be58 ([refactor]: cairo_utils -> cuty):cuty/dcel/voronoi/voronoi.py
 
 ##-- end imports
 
 ##-- logging
 logging = logmod.getLogger(__name__)
 ##-- end logging
```

### Comparing `jgdv-0.1.0/jgdv/geom/voronoi/voronoi.py` & `jgdv-0.1.1/jgdv/geom/voronoi/voronoi.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 #!/usr/bin/env python3
 """
 
-<<<<<<<< HEAD:cuty/voronoi/process.py
 """
 ##-- imports
 from __future__ import annotations
 
 import types
 import abc
 import datetime
@@ -20,23 +19,14 @@
 from dataclasses import InitVar, dataclass, field
 from typing import (TYPE_CHECKING, Any, Callable, ClassVar, Final, Generic,
                     Iterable, Iterator, Mapping, Match, MutableMapping,
                     Protocol, Sequence, Tuple, TypeAlias, TypeGuard, TypeVar,
                     cast, final, overload, runtime_checkable)
 from uuid import UUID, uuid1
 from weakref import ref
-========
-import cuty as utils
-from cuty import Parabola
-from cuty import rbtree
-from cuty.rbtree.comparison_functions import arc_comparison, Directions, arc_equality
-
-from cuty.dcel import DCEL, HalfEdge
-from cuty.umath import get_distance_raw, bound_line_in_bbox, isClockwise, bbox_centre
->>>>>>>> b18be58 ([refactor]: cairo_utils -> cuty):cuty/dcel/voronoi/voronoi.py
 
 ##-- end imports
 
 ##-- logging
 logging = logmod.getLogger(__name__)
 ##-- end logging
 
@@ -158,15 +148,14 @@
 
     def _update_arcs(self, d):
         """ Trigger the update of all stored arcs with a new frontier line position """
         self.beachline.update_values(lambda v, q: v.update_d(q), d)
 
     #-------------------- DCEL Completion
 
-
     def _add_circle_event(self, loc, source_node, voronoi_vertex, left=True):
         if loc[1] > self.sweep_position.y():# or np.allclose(loc[1], self.sweep_position.y()):
             logging.debug("Breaking out of add circle event: Wrong side of Beachline")
             return
         event = CircleEvent(loc, source_node, voronoi_vertex, i=self.current_step, left=left)
         logging.debug("Adding: {}".format(event))
         heapq.heappush(self.events, event)
@@ -184,16 +173,14 @@
                 node.data[CIRCLE_EVENTS.RIGHT].deactivate()
 
         if pre is not None and CIRCLE_EVENTS.RIGHT in pre.data:
             pre.data[CIRCLE_EVENTS.RIGHT].deactivate()
         if post is not None and CIRCLE_EVENTS.LEFT in post.data:
             post.data[CIRCLE_EVENTS.LEFT].deactivate()
 
-
-
     def relax(self, amnt=0.5, faces=None):
         """ Having calculated the voronoi diagram, use the centroids of
             the faces instead of the sites, and rerun the calculation.
         Can be passed in a subset of faces
         """
         assert(not bool(self.events))
 
@@ -216,15 +203,14 @@
             total_sites = other_face_sites
         assert(len(self.dcel.faces) == len(total_sites))
         #Setup the datastructures with the new sites
         self.reset()
         self.init_graph(data=new_sites, rerun=True)
         self.calculate_to_completion()
 
-
 class _VoronoiHandlers:
 
     def _handle_site_event(self, event):
         """
         provided with a site event, add it to the beachline in the appropriate place
         then update/remove any circle events that trios of arcs generate
         """
```

### Comparing `jgdv-0.1.0/jgdv/geom/voronoi/voronoi_drawing.py` & `jgdv-0.1.1/jgdv/geom/voronoi/voronoi_drawing.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 """
 ##-- imports
 from __future__ import annotations
 import logging as root_logger
 from math import nan
 from os.path import isdir, join
 import numpy as np
-import cuty as utils
 
 ##-- end imports
 
 logging = root_logger.getLogger(__name__)
 
 #Constants:
 COLOUR                    = [0.2, 0.1, 0.6, 1.0]
```

### Comparing `jgdv-0.1.0/jgdv/geom/voronoi/voronoi_io.py` & `jgdv-0.1.1/jgdv/geom/voronoi/voronoi_io.py`

 * *Files identical despite different names*

### Comparing `jgdv-0.1.0/jgdv/handlers/handler.py` & `jgdv-0.1.1/jgdv/handlers/handler.py`

 * *Files identical despite different names*

### Comparing `jgdv-0.1.0/jgdv/handlers/handler_system.py` & `jgdv-0.1.1/jgdv/handlers/handler_system.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,28 +15,14 @@
                     Iterator, Mapping, Match, MutableMapping, NewType,
                     Protocol, Sequence, Tuple, Type, TypeAlias, TypeVar, cast)
 
 ##-- end imports
 
 logging                = logmod.getLogger(__name__)
 
-import acab
-from acab import types as AT
-from acab.core.util.decorators.util import cache
-from acab.error.handler import (AcabHandlerException,
-                                HandlerDuplicationException)
-from acab.interfaces import handler_system as HS
-from acab.interfaces.config import ConfigSpec_d
-from acab.interfaces.data import Structure_i
-from acab.interfaces.fragments import HandlerFragment_i
-from acab.interfaces.protocols import handler_system as HSubP
-from acab.interfaces.sieve import AcabSieve
-from acab.interfaces.value import Sentence_i, Value_i
-from acab_config import AcabProtocolError as APE
-
 config                 = acab.config
 SPACER                 = config.any_of().print.SPACER_SIZE()
 
 DEFAULT_HANDLER_SIGNAL = config.handler.system.DEFAULT_SIGNAL
 # TODO import wrapper
 Handler                = config.on_fail().imports.specific.handler(wrapper="import"))
```

### Comparing `jgdv-0.1.0/jgdv/importing/inspect.py` & `jgdv-0.1.1/jgdv/importing/inspect.py`

 * *Files identical despite different names*

### Comparing `jgdv-0.1.0/jgdv/importing/plugin_loader.py` & `jgdv-0.1.1/jgdv/importing/plugin_loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,32 +31,32 @@
 # logging = logmod.root
 # logging.setLevel(logmod.NOTSET)
 ##-- end logging
 
 from collections import defaultdict
 from importlib.metadata import entry_points, EntryPoint
 import tomlguard
-import doot
-from doot._abstract import PluginLoader_p
+import jgdv
+from jgdv._interfaces.loader import PluginLoader_p
 
 skip_default_plugins        = doot.config.on_fail(False).skip_default_plugins()
 skip_plugin_search          = doot.config.on_fail(False).skip_plugin_search()
 env_plugins                 = doot.config.on_fail({}).plugins(wrapper=dict)
 plugin_types                = set(doot.constants.entrypoints.FRONTEND_PLUGIN_TYPES + doot.constants.entrypoints.BACKEND_PLUGIN_TYPES)
 cmd_loader_key  : Final     = doot.constants.entrypoints.DEFAULT_COMMAND_LOADER_KEY
 task_loader_key : Final     = doot.constants.entrypoints.DEFAULT_TASK_LOADER_KEY
 
 def make_ep (x, y, z):
     if z not in plugin_types:
         raise doot.errors.DootPluginError("Plugin Type Not Found: %s : %s", z, (x, y))
     return EntryPoint(name=x, value=y, group="{}.{}".format(doot.constants.entrypoints.PLUGIN_TOML_PREFIX, z))
 
 
-@doot.check_protocol
-class DootPluginLoader(PluginLoader_p):
+@jgdv.check_protocol
+class JGDVPluginLoader(PluginLoader_p):
     """
     Load doot plugins from the system, to choose from with doot.toml or cli args
     """
 
     def setup(self, extra_config=None) -> Self:
         self.plugins = defaultdict(list)
         match extra_config:
```

### Comparing `jgdv-0.1.0/jgdv/logging/log_colour.py` & `jgdv-0.1.1/jgdv/logging/log_colour.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,15 @@
     def yellow(s):
         return LEVEL_MAP['yellow'] + str(s) + COLOUR_RESET
 
     @staticmethod
     def red(s):
         return LEVEL_MAP['red'] + str(s) + COLOUR_RESET
 
-class DootColourFormatter(logging.Formatter):
+class JGDVColourFormatter(logging.Formatter):
     """
     Stream Formatter for doot, enables use of colour sent to console
 
     Guarded Formatter for adding colour.
     Uses the sty module.
     If sty is missing, behaves as the default formatter class
 
@@ -105,15 +105,15 @@
     def format(self, record):
         log_colour = self.colours[record.levelno]
         if hasattr(record, "colour"):
             log_colour = self.colours[record.colour]
 
         return log_colour + super().format(record) + COLOUR_RESET
 
-class DootColourStripFormatter(logging.Formatter):
+class JGDVColourStripFormatter(logging.Formatter):
     """
     Force Colour Command codes to be stripped out of a string.
     Useful for when you redirect printed strings with colour
     to a file
     """
 
     _default_fmt         = "{asctime} | {levelname:9} | {shortname:25} | {message}"
```

### Comparing `jgdv-0.1.0/jgdv/logging/log_context.py` & `jgdv-0.1.1/jgdv/logging/log_context.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 import more_itertools as mitz
 ##-- end lib imports
 
 ##-- logging
 logging = logmod.getLogger(__name__)
 ##-- end logging
 
-class DootLogContext:
+class JGDVLogContext:
     """
       a really simple wrapper to set a logger's level, then roll it back
     """
 
     def __init__(self, logger, level=None):
         self._logger          = logger
         self._original_level  = self._logger.level
```

### Comparing `jgdv-0.1.0/jgdv/logging/stdout_capture.py` & `jgdv-0.1.1/jgdv/logging/stdout_capture.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,16 +36,16 @@
 ##-- logging
 logging = logmod.getLogger(__name__)
 ##-- end logging
 
 import contextlib
 import io
 
-with contextlib.redirect_stdout(io.StringIO()) as stdout:
-     $0
+# with contextlib.redirect_stdout(io.StringIO()) as stdout:
+#      $0
 
 
 class ColourStripPrintCapture(logmod.Formatter):
     """
       WARNING: MODIFIES builtins.print
       intercept print commands, so they can be logged at DEBUG level
     Force Colour Command codes to be stripped out of a string.
```

### Comparing `jgdv-0.1.0/jgdv/math/colour.py` & `jgdv-0.1.1/jgdv/math/colour.py`

 * *Files identical despite different names*

### Comparing `jgdv-0.1.0/jgdv/math/comparison.py` & `jgdv-0.1.1/jgdv/math/comparison.py`

 * *Files identical despite different names*

### Comparing `jgdv-0.1.0/jgdv/math/easings.py` & `jgdv-0.1.1/jgdv/math/easings.py`

 * *Files identical despite different names*

### Comparing `jgdv-0.1.0/jgdv/math/matrices.py` & `jgdv-0.1.1/jgdv/math/matrices.py`

 * *Files identical despite different names*

### Comparing `jgdv-0.1.0/jgdv/math/parabola.py` & `jgdv-0.1.1/jgdv/math/parabola.py`

 * *Files identical despite different names*

### Comparing `jgdv-0.1.0/jgdv/math/quadratic.py` & `jgdv-0.1.1/jgdv/math/quadratic.py`

 * *Files identical despite different names*

### Comparing `jgdv-0.1.0/jgdv/math/quantize.py` & `jgdv-0.1.1/jgdv/math/quantize.py`

 * *Files identical despite different names*

### Comparing `jgdv-0.1.0/jgdv/math/rand.py` & `jgdv-0.1.1/jgdv/math/rand.py`

 * *Files identical despite different names*

### Comparing `jgdv-0.1.0/jgdv/math/sorting.py` & `jgdv-0.1.1/jgdv/math/sorting.py`

 * *Files identical despite different names*

### Comparing `jgdv-0.1.0/jgdv/math/umath.py` & `jgdv-0.1.1/jgdv/math/umath.py`

 * *Files identical despite different names*

### Comparing `jgdv-0.1.0/jgdv/math/utils.py` & `jgdv-0.1.1/jgdv/math/utils.py`

 * *Files identical despite different names*

### Comparing `jgdv-0.1.0/jgdv/setup/asyncio_client.py` & `jgdv-0.1.1/jgdv/setup/asyncio_client.py`

 * *Files identical despite different names*

### Comparing `jgdv-0.1.0/jgdv/setup/asyncio_server.py` & `jgdv-0.1.1/jgdv/setup/asyncio_server.py`

 * *Files identical despite different names*

### Comparing `jgdv-0.1.0/jgdv/setup/gtk.py` & `jgdv-0.1.1/jgdv/setup/gtk.py`

 * *Files identical despite different names*

### Comparing `jgdv-0.1.0/jgdv/setup/hooks.py` & `jgdv-0.1.1/jgdv/setup/hooks.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,18 @@
 
 def exception_hook_loop(exc_type, exc_value, tb):
     ""
     local_vars = tb.tb_frame.f_locals
     tb = tb.tb_next
     print(f"Local variables in top frame: {local_vars}")
 
-class DejaVuHookConfig:
+class JGDVHookConfig:
+    """
+    Utiility class for setting up various python hooks
+    """
 
     def __init__(self):
         self._disabled = "PRE_COMMIT" in env
         self._exit_hook       = None
         self._exception_hook  = None
         self._breakpoint_hook = None
         self._display_hook    = None
```

### Comparing `jgdv-0.1.0/jgdv/setup/importing.py` & `jgdv-0.1.1/jgdv/setup/importing.py`

 * *Files identical despite different names*

### Comparing `jgdv-0.1.0/jgdv/setup/logging.py` & `jgdv-0.1.1/jgdv/logging/log_config.py`

 * *Files 11% similar despite different names*

```diff
@@ -29,107 +29,118 @@
 
 ##-- logging
 logging = logmod.getLogger(__name__)
 ##-- end logging
 
 import os
 from sys import stdout, stderr
-import doot
-from doot.utils.log_colour import DootColourFormatter, DootColourStripFormatter
+from jgdv.logging.log_colour import JGDVColourFormatter, JGDVColourStripFormatter
 
 env : dict = os.environ
 
-class _DootAnyFilter:
+class _JGDVAnyFilter:
     """
 
     """
 
     def __init__(self, names=None, reject=None):
         self.names      = names or []
         self.rejections = reject or []
         self.name_re    = re.compile("^({})".format("|".join(self.names)))
 
     def __call__(self, record):
         return (record.name not in self.rejections) and (record.name == "root"
                                                          or not bool(self.names)
                                                     or self.name_re.match(record.name))
 
-class DootLogConfig:
+class JGDVLogConfig:
     """ Utility class to setup [stdout, stderr, file] logging. """
 
     def __init__(self):
         # Root Logger for everything
         self.root    = logmod.root
         # EXCEPT this, which replaces 'print(x)'
         self.printer               = logmod.getLogger(doot.constants.printer.PRINTER_NAME)
 
-        self.file_handler          = logmod.FileHandler(pl.Path() / "log.doot", mode='w')
+        self.file_handler          = None
         self.stream_handler        = logmod.StreamHandler(stdout)
         self.print_stream_handler  = logmod.StreamHandler(stdout)
 
-        self._setup()
+        self._pre_setup()
 
-    def _setup(self):
+    def _pre_setup(self):
         """ a basic, config-less setup """
         self.root.setLevel(logmod.NOTSET)
-        self.file_handler.setFormatter(DootColourStripFormatter(fmt="{levelname} : INIT : {message}"))
+        # self.file_handler.setFormatter(JGDVColourStripFormatter(fmt="{levelname} : INIT : {message}"))
 
         self.stream_handler.setLevel(logmod.WARNING)
         self.stream_handler.setFormatter(logmod.Formatter("{levelname}  : INIT : {message}", style="{"))
 
-        self.root.addHandler(self.file_handler)
         self.root.addHandler(self.stream_handler)
 
         self.printer.propagate = False
         self.print_stream_handler.setFormatter(logmod.Formatter("{message}", style="{"))
         self.printer.setLevel(logmod.NOTSET)
         self.printer.addHandler(self.print_stream_handler)
-        self.printer.addHandler(self.file_handler)
+        # self.printer.addHandler(self.file_handler)
 
     def setup(self):
         """ a setup that uses config values """
         assert(doot.config is not None)
         self._setup_file_logging()
         self._setup_stream_logging()
         self._setup_print_logging()
 
     def _setup_file_logging(self):
+        log_name_format = doot.config.on_fail("doot-%Y-%m-%d::%H:%M.log").logging.file.name()
+        log_file_name   = datetime.datetime.now().strftime(log_name_format)
+
+        log_dir = doot.locs["{logs}"]
+        # TODO delete old logs if number of logs larger than N
+        if not log_dir.exists():
+            log_dir = pl.Path()
+
+        log_file_path = log_dir / log_file_name
+
+        self.file_handler  = logmod.FileHandler(log_file_path, mode='w')
         file_log_level    = doot.config.on_fail("DEBUG", str|int).logging.file.level(wrapper=lambda x: logmod._nameToLevel.get(x, 0))
         file_log_format   = doot.config.on_fail("{levelname} : {pathname} : {lineno} : {funcName} : {message}", str).logging.file.format()
         file_filter_names = doot.config.on_fail([], list).logging.file.allow()
 
         self.file_handler.setLevel(file_log_level)
-        self.file_handler.setFormatter(DootColourStripFormatter(fmt=file_log_format))
+        self.file_handler.setFormatter(JGDVColourStripFormatter(fmt=file_log_format))
         if bool(file_filter_names):
-            self.file_handler.addFilter(_DootAnyFilter(file_filter_names))
+            self.file_handler.addFilter(_JGDVAnyFilter(file_filter_names))
+
+        self.root.addHandler(self.file_handler)
 
     def _setup_stream_logging(self):
         stream_log_level    = doot.config.on_fail("WARNING", str|int).logging.stream.level(wrapper=lambda x: logmod._nameToLevel.get(x, 0))
         stream_log_format   = doot.config.on_fail("{levelname} : {pathname} : {lineno} : {funcName} : {message}", str).logging.stream.format()
         stream_filter_names = doot.config.on_fail([], list).logging.stream.allow()
 
         self.stream_handler.setLevel(stream_log_level)
         use_colour = doot.config.on_fail(False, bool).logging.stream.colour()
         use_colour &= "PRE_COMMIT" not in env
         if use_colour:
-            self.stream_handler.setFormatter(DootColourFormatter(fmt=stream_log_format))
+            self.stream_handler.setFormatter(JGDVColourFormatter(fmt=stream_log_format))
         else:
-            self.stream_handler.setFormatter(DootColourStripFormatter(fmt=stream_log_format))
+            self.stream_handler.setFormatter(JGDVColourStripFormatter(fmt=stream_log_format))
 
         if bool(stream_filter_names):
-            self.stream_handler.addFilter(_DootAnyFilter(stream_filter_names))
+            self.stream_handler.addFilter(_JGDVAnyFilter(stream_filter_names))
 
     def _setup_print_logging(self):
         printer_log_level    = doot.config.on_fail("NOTSET", str|int).logging.printer.level(wrapper=lambda x: logmod._nameToLevel.get(x, 0))
         printer_log_format   = doot.config.on_fail("{message}", str).logging.printer.format()
 
         self.print_stream_handler.setLevel(printer_log_level)
 
         use_colour = doot.config.on_fail(False, bool).logging.printer.colour()
         use_colour &= "PRE_COMMIT" not in env
         if use_colour:
-            self.print_stream_handler.setFormatter(DootColourFormatter(fmt=printer_log_format))
+            self.print_stream_handler.setFormatter(JGDVColourFormatter(fmt=printer_log_format))
         else:
-            self.print_stream_handler.setFormatter(DootColourStripFormatter(fmt=printer_log_format))
+            self.print_stream_handler.setFormatter(JGDVColourStripFormatter(fmt=printer_log_format))
 
     def set_level(self, level):
         self.stream_handler.setLevel(level)
```

### Comparing `jgdv-0.1.0/jgdv/setup/main.py` & `jgdv-0.1.1/jgdv/setup/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,34 +24,32 @@
 
 logging         = logmod.root
 printer         = logmod.getLogger("doot._printer")
 
 import sh
 import stackprinter
 import tomlguard as TG
-import doot
 from bdb import BdbQuit
-from doot.utils.log_config import DootLogConfig
 
 def main():
     result  = 1
     errored = False
     overlord = None
     try:
         log_config = DootLogConfig()
         # --- Setup
         if not bool(doot.config):
             doot.setup()
 
         log_config.setup()
 
         logging.info("Called with: %s", sys.argv)
-        from doot.loaders.plugin_loader import DootPluginLoader
+        from jgdv.importing.plugin_loader import JGDVPluginLoader
         from doot.control.overlord import DootOverlord
-        overlord  = DootOverlord(loaders={"plugin": DootPluginLoader().setup(sys.argv[:]) },
+        overlord  = DootOverlord(loaders={"plugin": JGDVPluginLoader().setup(sys.argv[:]) },
                                  config_filenames=[doot.constants.paths.DEFAULT_LOAD_TARGETS],
                                  log_config=log_config,
                                  args=sys.argv[:])
 
         # --- Do whatever thats been triggered
         result    = overlord()
```

### Comparing `jgdv-0.1.0/jgdv/setup/pyparsing.py` & `jgdv-0.1.1/jgdv/setup/pyparsing.py`

 * *Files identical despite different names*

### Comparing `jgdv-0.1.0/jgdv/setup/setup.py` & `jgdv-0.1.1/jgdv/setup/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,16 +11,14 @@
 from typing import Final, Any, assert_type
 from importlib.resources import files
 import sys
 ##-- end std imports
 
 ##-- imports
 import tomlguard as TG
-import doot.errors
-from doot.utils.check_protocol import check_protocol
 ##-- end imports
 
 ##-- data
 data_path      = files("doot.__data")
 constants_file = data_path.joinpath("constants.toml")
 aliases_file   = data_path.joinpath("aliases.toml")
 ##-- end data
@@ -106,16 +104,16 @@
         flat[key].update(dict(val))
 
     aliases = TG.TomlGuard(flat)
 
 def _load_locations():
     """ Load and update the DootLocations db """
     global locs
-    from doot.control.locations import DootLocations
-    locs   = DootLocations(pl.Path.cwd())
+    from jgdv.locations.locations import JGDVLocations
+    locs   = JGDVLocations(pl.Path.cwd())
     # Load Initial locations
     for loc in config.on_fail([]).locations():
         locs.update(loc)
 
 def _update_import_path():
     """ Add locations to the python path for task local code importing  """
     task_sources = config.on_fail([locs[".tasks"]], list).settings.tasks.sources(wrapper=lambda x: [locs[y] for y in x])
```

### Comparing `jgdv-0.1.0/jgdv/spiders/__init__.py` & `jgdv-0.1.1/jgdv/spiders/__init__.py`

 * *Files identical despite different names*

### Comparing `jgdv-0.1.0/jgdv/spiders/__tests/test_runner.py` & `jgdv-0.1.1/jgdv/spiders/__tests/test_runner.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,20 +10,14 @@
                     Mapping, Match, MutableMapping, Sequence, Tuple, TypeAlias,
                     TypeVar, cast)
 import warnings
 
 import pytest
 
 import tomlguard
-import doot
-from doot.enums import TaskStateEnum
-from doot.structs import DootTaskSpec, DootActionSpec
-from doot._abstract import Job_i, Task_i, TaskTracker_i, TaskRunner_i, ReportLine_i, Action_p, Reporter_i
-from doot.utils import mock_gen
-from dootle.spiders.runner import DootleReactorRunner
 
 logging = logmod.root
 
 @pytest.mark.parametrize("ctor", [DootleReactorRunner])
 class TestRunner:
 
     @pytest.fixture(scope="function")
```

### Comparing `jgdv-0.1.0/jgdv/spiders/__tests/test_tracker.py` & `jgdv-0.1.1/jgdv/spiders/__tests/test_tracker.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,19 +12,14 @@
 from typing import (Any, Callable, ClassVar, Generic, Iterable, Iterator,
                     Mapping, Match, MutableMapping, Sequence, Tuple, TypeAlias,
                     TypeVar, cast)
 ##-- end imports
 logging = logmod.root
 
 import pytest
-import doot.errors
-import doot.structs
-from doot.control.tracker import DootTracker
-from doot._abstract import Task_i
-from doot.utils import mock_gen
 
 @pytest.mark.parametrize("ctor", [DootTracker])
 class TestTracker:
 
     def test_initial(self, ctor):
         tracker = ctor()
         assert(tracker is not None)
```

### Comparing `jgdv-0.1.0/jgdv/spiders/actions.py` & `jgdv-0.1.1/jgdv/spiders/actions.py`

 * *Files 9% similar despite different names*

```diff
@@ -33,20 +33,14 @@
 ##-- end lib imports
 
 ##-- logging
 logging = logmod.getLogger(__name__)
 ##-- end logging
 printer = logmod.getLogger("doot._printer")
 
-import doot
-import doot.errors
-from doot._abstract import Action_p
-from doot.mixins.importer import Importer_M
-from doot.structs import DootKey, DootCodeReference
-
 SPIDER  = DootKey.make("spider")
 CRAWLER = DootKey.make("crawler")
 
 class RunSpider(Action_p, Importer_M):
     """
       add a spider to the scrapy crawler that is in state
     """
```

### Comparing `jgdv-0.1.0/jgdv/spiders/caching.py` & `jgdv-0.1.1/jgdv/spiders/caching.py`

 * *Files identical despite different names*

### Comparing `jgdv-0.1.0/jgdv/spiders/crawler.py` & `jgdv-0.1.1/jgdv/spiders/crawler.py`

 * *Files identical despite different names*

### Comparing `jgdv-0.1.0/jgdv/spiders/middleware.py` & `jgdv-0.1.1/jgdv/spiders/middleware.py`

 * *Files identical despite different names*

### Comparing `jgdv-0.1.0/jgdv/spiders/mixin.py` & `jgdv-0.1.1/jgdv/spiders/mixin.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,16 +31,15 @@
 ##-- end logging
 
 ##-- imports
 from importlib.resources import files
 ##-- end imports
 
 import tomlguard
-import doot
-from doot.spiders.crawler import CrawlerProcessFix
+from jgdv.spiders.crawler import CrawlerProcessFix
 from urllib.parse import urlparse
 
 default_toml           = tomlguard.load(files("doot.__templates") / "spider_toml").flatten_on().spiders().get_table()
 spider_settings        = doot.config.flatten_on().spiders().get_table()
 
 settings_with_defaults = default_toml.copy()
 settings_with_defaults.update(spider_settings)
```

### Comparing `jgdv-0.1.0/jgdv/spiders/pipeline.py` & `jgdv-0.1.1/jgdv/spiders/pipeline.py`

 * *Files identical despite different names*

### Comparing `jgdv-0.1.0/jgdv/spiders/runner.py` & `jgdv-0.1.1/jgdv/spiders/runner.py`

 * *Files 12% similar despite different names*

```diff
@@ -56,22 +56,16 @@
 ##-- logging
 logging = logmod.getLogger(__name__)
 ##-- end logging
 
 printer = logmod.getLogger("doot._printer")
 
 from collections import defaultdict
-import doot
-import doot.errors
-from doot.enums import ReportEnum, ActionResponseEnum as ActRE
-from doot._abstract import Job_i, Task_i, FailPolicy_p
-from doot._abstract import TaskTracker_i, TaskRunner_i, TaskBase_i, ReportLine_i, Action_p
-from doot.utils.signal_handler import SignalHandler
-from doot.structs import DootTaskSpec, DootActionSpec
-from doot.control.base_runner import BaseRunner, logctx
+import jgdv
+from jgdv.enums.task_respones import TaskResponseEnum as ActRE
 
 from zope.interface import implementer
 from twisted.internet import reactor, protocol, defer, threads
 from twisted.internet.interfaces import IStreamServerEndpoint
 
 from scrapy.crawler import CrawlerRunner
 import scrapy
@@ -81,16 +75,16 @@
 build_level   : Final[str] = doot.constants.printer.DEFAULT_BUILD_LEVEL
 action_level  : Final[str] = doot.constants.printer.DEFAULT_ACTION_LEVEL
 sleep_level   : Final[str] = doot.constants.printer.DEFAULT_SLEEP_LEVEL
 execute_level : Final[str] = doot.constants.printer.DEFAULT_EXECUTE_LEVEL
 
 reactor_timeout = doot.config.on_fail(2, int).settings.tasks.reactor_timeout()
 
-@doot.check_protocol
-class DootleReactorRunner(BaseRunner, TaskRunner_i):
+@jgdv.check_protocol
+class JGDVReactorRunner(BaseRunner, TaskRunner_i):
     """ The simplest reactor task runner
       https://stackoverflow.com/questions/8532131
 
      wraps steps of running jobs/tasks/actions into deferreds
     """
 
     def __init__(self:Self, *, tracker:TaskTracker_i, reporter:Reporter_i, policy=None):
```

### Comparing `jgdv-0.1.0/jgdv/spiders/spiders.py` & `jgdv-0.1.1/jgdv/spiders/spiders.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 from scrapy.http import Headers, Response
 from scrapy.http.request import Request
 from scrapy.responsetypes import responsetypes
 from scrapy.spiders import Spider
 from scrapy.utils.httpobj import urlparse_cached
 from w3lib.http import headers_dict_to_raw, headers_raw_to_dict
 
-class DootBasicSpider(scrapy.Spider):
+class JGDVBasicSpider(scrapy.Spider):
     """
     Basic Doot Spider that stores locs and its parent task
     """
 
     def __init__(self, name=None, locs=None, urls=None, domains=None, task=None):
         super().__init__(name)
         self.locs            = locs
```

### Comparing `jgdv-0.1.0/jgdv/spiders/tracker.py` & `jgdv-0.1.1/jgdv/spiders/tracker.py`

 * *Files 6% similar despite different names*

```diff
@@ -55,40 +55,34 @@
 
 ##-- logging
 logging = logmod.getLogger(__name__)
 ##-- end logging
 
 from collections import defaultdict
 from queue import PriorityQueue
-import doot
-import doot.errors
-from doot.enums import TaskStateEnum
-from doot._abstract import Job_i, Task_i, FailPolicy_p
-from doot.structs import DootTaskArtifact, DootTaskSpec, DootCodeReference, DootTaskName
-from doot._abstract import TaskTracker_i, TaskRunner_i, TaskBase_i
-from doot.task.base_task import DootTask
-from doot.control.base_tracker import BaseTracker, ROOT, STATE, PRIORITY, EDGE_E
+import jgdv
+from jgdv.enums.task_state import TaskStateEnum
 
-@doot.check_protocol
-class DootleReactorTracker(BaseTracker, TaskTracker_i):
+@jgdv.check_protocol
+class JGDVReactorTracker(BaseTracker, TaskTracker_i):
     """
     track dependencies in a networkx digraph,
     successors of a node are its dependencies.
       ie: ROOT -> Task -> Dependency -> SubDependency
 
     tracks definite and indefinite artifacts as products and dependencies of tasks as well.
 
     the `task_graph` stores nodes as full names of tasks
     """
     state_e = TaskStateEnum
 
     def __init__(self, shadowing:bool=False, *, policy=None):
         super().__init__(policy=policy) # self.tasks
 
-    def add_task(self, task:DootTaskSpec|TaskBase_i, *, no_root_connection=False) -> None:
+    def add_task(self, task:JGDVTaskSpec|TaskBase_i, *, no_root_connection=False) -> None:
         """ add a task description into the tracker, but don't queue it
         connecting it with its dependencies and tasks that depend on it
         """
 
         task : TaskBase_i = self._prep_task(task)
         assert(isinstance(task, TaskBase_i))
         # Store it
@@ -101,33 +95,33 @@
         if not no_root_connection:
             self.task_graph.add_edge(ROOT, task.name)
 
         self._insert_dependencies(task)
         self._insert_dependents(task)
         self._insert_according_to_queue_behaviour(task)
 
-    def update_state(self, task:str|TaskBase_i|DootTaskArtifact, state:self.state_e):
+    def update_state(self, task:str|TaskBase_i|JGDVTaskArtifact, state:self.state_e):
         """ update the state of a task in the dependency graph """
         logging.debug("Updating Task State: %s -> %s", task, state)
         match task, state:
             case str(), self.state_e() if task in self.task_graph:
                 self.task_graph.nodes[task]['state'] = state
             case TaskBase_i(), self.state_e() if task.name in self.task_graph:
                 self.task_graph.nodes[task.name]['state'] = state
-            case DootTaskArtifact(), self.state_e() if task in self.task_graph:
+            case JGDVTaskArtifact(), self.state_e() if task in self.task_graph:
                 self.task_graph.nodes[task]['state'] = state
             case _, _:
                 raise doot.errors.DootTaskTrackingError("Bad task update state args", task, state)
 
     def next_for(self, target:None|str=None) -> None|Job_i|Task_i:
         """ ask for the next task that can be performed """
         if target and target not in self.active_set:
             self.queue_task(target, silent=True)
 
-        focus : str | DootTaskArtifact | None = None
+        focus : str | JGDVTaskArtifact | None = None
         adj                                   = dict(self.task_graph.adjacency())
         while bool(self.task_queue):
             focus : str = self.task_queue.peek()
             logging.debug("Task: %s  State: %s, Stack: %s", focus, self.task_state(focus), self.active_set)
 
             if focus in self.task_graph and self.task_graph.nodes[focus][PRIORITY] < self._min_priority:
                 logging.warning("Task reached minimum priority while waiting, and has been cancelled: %s", focus)
```

### Comparing `jgdv-0.1.0/jgdv/structs/heap/element.py` & `jgdv-0.1.1/jgdv/structs/heap/element.py`

 * *Files identical despite different names*

### Comparing `jgdv-0.1.0/jgdv/structs/heap/heap.py` & `jgdv-0.1.1/jgdv/structs/heap/heap.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
 ##-- logging
 logging = logmod.getLogger(__name__)
 ##-- end logging
 
 import heapq
 
-class DejaVuHeap:
+class JGDVHeap:
 
     def __init__(self):
         self._heap = None
 
     def pop_while_same(self):
         """ Pop while the head is equal to the first value poppped """
         assert(all([isinstance(x, HeapWrapper) for x in self._heap]))
```

### Comparing `jgdv-0.1.0/jgdv/structs/proxy/base.py` & `jgdv-0.1.1/jgdv/structs/proxy/base.py`

 * *Files identical despite different names*

### Comparing `jgdv-0.1.0/jgdv/structs/proxy/iter_proxy.py` & `jgdv-0.1.1/jgdv/structs/proxy/iter_proxy.py`

 * *Files 0% similar despite different names*

```diff
@@ -112,15 +112,14 @@
                 val = val[attr]
 
         return TomlGuardIterFirstProxy(val,
                                        types=self._types,
                                        index=self._index(attr),
                                        fallback=self._fallback)
 
-
     def _nested_inject(self, attr=None, clear=None) -> TomlGuardIterProxy|None:
         sub_proxies = []
         assert(isinstance(self._data, list))
         index    = self._index()
         subindex = self._subindex(attr)
         for data in self._data:
             match data:
@@ -145,15 +144,14 @@
 
         return TomlGuardIterFirstProxy(sub_proxies,
                                        types=self._types,
                                        fallback=self._fallback,
                                        index=index,
                                        subindex=subindex)
 
-
     def _match_type(self, val:TomlTypes) -> TomlTypes:
         return val
 
 class TomlGuardIterAllProxy(TomlGuardIterProxy):
     """
     A Proxy for lists and dicts, which can flatten, or match particulars
     """
```

### Comparing `jgdv-0.1.0/jgdv/structs/proxy/proxy.py` & `jgdv-0.1.1/jgdv/structs/proxy/proxy.py`

 * *Files identical despite different names*

### Comparing `jgdv-0.1.0/jgdv/structs/proxy/proxy_mixin.py` & `jgdv-0.1.1/jgdv/structs/proxy/proxy_mixin.py`

 * *Files identical despite different names*

### Comparing `jgdv-0.1.0/jgdv/structs/rbtree/__tests/test_rbtree.py` & `jgdv-0.1.1/jgdv/structs/rbtree/__tests/test_rbtree.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,10 @@
 import unittest
 import logging
 import IPython
-from test_context import cuty as utils
-from cuty import rbtree
-from cuty.rbtree import comparison_functions as CompFuncs
 
 
 class RBTree_Tests(unittest.TestCase):
 
     def setUp(self):
         self.t = rbtree.RBTree()
```

### Comparing `jgdv-0.1.0/jgdv/structs/rbtree/__tests/test_rbtree_node.py` & `jgdv-0.1.1/jgdv/structs/rbtree/__tests/test_rbtree_node.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,10 @@
 import unittest
 import logging
 import IPython
-from test_context import cuty as utils
-from cuty import rbtree
-from cuty.rbtree import comparison_functions as CompFuncs
-from cuty.rbtree import Node
-
 
 class RBTree_Tests(unittest.TestCase):
 
     def setUp(self):
         self.n = Node(2)
 
     def tearDown(self):
@@ -143,14 +138,15 @@
         n2 = Node(3)
         n3 = Node(4)
         n1.add_left(n2)
         n2.add_right(n3)
         self.assertEqual(n3.get_successor(), n1)
 
     #test getPred/Succ_while
+
     def test_min(self):
         n1 = Node(2)
         n2 = Node(3)
         n3 = Node(4)
         n1.add_left(n2)
         n2.add_left(n3)
         self.assertEqual(n1.min(), n3)
```

### Comparing `jgdv-0.1.0/jgdv/structs/rbtree/comparison_functions.py` & `jgdv-0.1.1/jgdv/structs/rbtree/comparison_functions.py`

 * *Files identical despite different names*

### Comparing `jgdv-0.1.0/jgdv/structs/rbtree/node.py` & `jgdv-0.1.1/jgdv/structs/rbtree/node.py`

 * *Files identical despite different names*

### Comparing `jgdv-0.1.0/jgdv/structs/rbtree/operations.py` & `jgdv-0.1.1/jgdv/structs/rbtree/operations.py`

 * *Files identical despite different names*

### Comparing `jgdv-0.1.0/jgdv/structs/rbtree/rb_data.py` & `jgdv-0.1.1/jgdv/structs/rbtree/rb_data.py`

 * *Files identical despite different names*

### Comparing `jgdv-0.1.0/jgdv/structs/rbtree/rbtree.py` & `jgdv-0.1.1/jgdv/structs/rbtree/rbtree.py`

 * *Files identical despite different names*

### Comparing `jgdv-0.1.0/jgdv/structs/rbtree/utils.py` & `jgdv-0.1.1/jgdv/structs/rbtree/utils.py`

 * *Files identical despite different names*

### Comparing `jgdv-0.1.0/jgdv/structs/regex.py` & `jgdv-0.1.1/jgdv/structs/regex.py`

 * *Files identical despite different names*

### Comparing `jgdv-0.1.0/jgdv/structs/rete/alpha.py` & `jgdv-0.1.1/jgdv/structs/rete/rete.py`

 * *Files identical despite different names*

### Comparing `jgdv-0.1.0/jgdv/structs/rete/beta.py` & `jgdv-0.1.1/jgdv/structs/time/structs/base.py`

 * *Files identical despite different names*

### Comparing `jgdv-0.1.0/jgdv/structs/rete/rete.py` & `jgdv-0.1.1/jgdv/mixins/param_spec.py`

 * *Files 11% similar despite different names*

```diff
@@ -26,13 +26,23 @@
                     Protocol, Sequence, Tuple, TypeAlias, TypeGuard, TypeVar,
                     cast, final, overload, runtime_checkable, Generator)
 from uuid import UUID, uuid1
 
 ##-- end builtin imports
 
 ##-- lib imports
-import more_itertools as mitz
+# import more_itertools as mitz
+# from boltons import
 ##-- end lib imports
 
 ##-- logging
 logging = logmod.getLogger(__name__)
 ##-- end logging
+
+from jgdv.structs.param_spec import JGDVParamSpec
+
+class ParamSpecMaker_m:
+
+    @staticmethod
+    def build_param(*args:Any, **kwargs:Any) -> JGDVParamSpec:
+        """ Utility method for easily making paramspecs """
+        return JGDVParamSpec(*args, **kwargs)
```

### Comparing `jgdv-0.1.0/jgdv/structs/time/__tests/test_time.py` & `jgdv-0.1.1/jgdv/structs/time/__tests/test_time.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,9 @@
 import unittest
 import logging
-from test_context import cuty as utils
-import cuty.time as time
-from cuty.time.arc import Arc
-from cuty.time.event import Event
-import IPython
 t = time.Time
 
 class TestTime(unittest.TestCase):
 
     def setUp(self):
         return 1
```

### Comparing `jgdv-0.1.0/jgdv/structs/time/dsl.py` & `jgdv-0.1.1/jgdv/structs/time/dsl.py`

 * *Files identical despite different names*

### Comparing `jgdv-0.1.0/jgdv/structs/time/pattern_constructor.py` & `jgdv-0.1.1/jgdv/structs/time/pattern_constructor.py`

 * *Files identical despite different names*

### Comparing `jgdv-0.1.0/jgdv/structs/time/pattern_iterator.py` & `jgdv-0.1.1/jgdv/structs/time/pattern_iterator.py`

 * *Files identical despite different names*

### Comparing `jgdv-0.1.0/jgdv/structs/time/structs/arc.py` & `jgdv-0.1.1/jgdv/structs/time/structs/arc.py`

 * *Files identical despite different names*

### Comparing `jgdv-0.1.0/jgdv/structs/time/structs/base.py` & `jgdv-0.1.1/jgdv/files/tex/bib.py`

 * *Files 12% similar despite different names*

```diff
@@ -32,7 +32,12 @@
 ##-- lib imports
 import more_itertools as mitz
 ##-- end lib imports
 
 ##-- logging
 logging = logmod.getLogger(__name__)
 ##-- end logging
+
+from jgdv.files.tex.base import TexStatement_i
+
+class TexBib(TexStatement_i):
+    pass
```

### Comparing `jgdv-0.1.0/jgdv/structs/time/structs/event.py` & `jgdv-0.1.1/jgdv/structs/time/structs/event.py`

 * *Files identical despite different names*

### Comparing `jgdv-0.1.0/jgdv/structs/time/structs/pattern.py` & `jgdv-0.1.1/jgdv/structs/time/structs/pattern.py`

 * *Files identical despite different names*

### Comparing `jgdv-0.1.0/jgdv/structs/time/structs/var.py` & `jgdv-0.1.1/jgdv/enums/loop_control.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 #!/usr/bin/env python3
 """
 
-
 See EOF for license/metadata/notes as applicable
 """
 
 ##-- builtin imports
 from __future__ import annotations
 
 # import abc
@@ -26,18 +25,29 @@
                     Protocol, Sequence, Tuple, TypeAlias, TypeGuard, TypeVar,
                     cast, final, overload, runtime_checkable, Generator)
 from uuid import UUID, uuid1
 
 ##-- end builtin imports
 
 ##-- lib imports
-import more_itertools as mitz
+# import more_itertools as mitz
+# from boltons import
 ##-- end lib imports
 
 ##-- logging
 logging = logmod.getLogger(__name__)
 ##-- end logging
 
-class TimeVar:
-
-    def __init__(self, name):
-        self.name = name
+class LoopControl(enum.Enum):
+    """
+      A Simple enum to descrbe results for testing in a maybe recursive loop
+      (like walking a a tree)
+
+    accept  : is a result, and descend if recursive
+    keep    : is a result, don't descend
+    discard : not a result, descend
+    reject  : not a result, don't descend
+    """
+    yesAnd  = enum.auto()
+    yes     = enum.auto()
+    noBut   = enum.auto()
+    no      = enum.auto()
```

### Comparing `jgdv-0.1.0/jgdv/structs/time/utils.py` & `jgdv-0.1.1/jgdv/structs/time/utils.py`

 * *Files identical despite different names*

### Comparing `jgdv-0.1.0/jgdv/structs/tree/binary_tree.py` & `jgdv-0.1.1/jgdv/structs/tree/binary_tree.py`

 * *Files identical despite different names*

### Comparing `jgdv-0.1.0/jgdv/structs/trie/leaf.py` & `jgdv-0.1.1/jgdv/structs/trie/leaf.py`

 * *Files identical despite different names*

### Comparing `jgdv-0.1.0/jgdv/structs/trie/semantics.py` & `jgdv-0.1.1/jgdv/structs/trie/semantics.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,41 +1,24 @@
 #!/usr/bin/env python3
 ##-- imports
 from __future__ import annotations
 import logging as logmod
 
-import acab.core.defaults.value_keys as DS
-import acab.error.semantic as ASErr
-import acab.interfaces.data as DI
-import acab.interfaces.semantic as SI
-from acab import types as AT
-import acab
-from acab.core.data.acab_struct import BasicNodeStruct
-from acab.core.semantics import basic
-from acab.core.value.instruction import Instruction
-from acab.core.value.sentence import Sentence
-from acab.interfaces.bind import Bind_i
-from acab.interfaces.value import Sentence_i
-from acab_config import AcabProtocolError as APE
-
-from .flatten_query_manager import FlattenQueryManager
-
 ##-- end imports
 
 logging = logmod.getLogger(__name__)
 
 config = acab.config
 
 Node          = DI.StructView
 Value         = AT.Value
 Structure     = AT.DataStructure
 Engine        = AT.Engine
 Contexts      = AT.CtxSet
 
-@APE.assert_implements(SI.StructureSemantics_i)
 class FlattenBreadthTrieSemantics(basic.StructureSemantics, SI.StructureSemantics_i):
     """
     Trie Semantics which map values -> Nodes
     Searches *Breadth First*
 
     Has sentence-flattening logic for querying.
     """
```

### Comparing `jgdv-0.1.0/jgdv/structs/trie/trie.py` & `jgdv-0.1.1/jgdv/structs/trie/trie.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,19 +5,18 @@
 from __future__ import annotations
 
 import logging as logmod
 from dataclasses import InitVar, dataclass, field
 from typing import (Any, Callable, ClassVar, Dict, Generic, Iterable, Iterator,
                     List, Mapping, Match, MutableMapping, Optional, Sequence,
                     Set, Tuple, TypeVar, Union, cast)
-from urllib.parse import parse_qs, urlencode, urlparse, urlunparse
-
-from doot.utils.formats.bookmarks import Bookmark
 ##-- end imports
 
+from urllib.parse import parse_qs, urlencode, urlparse, urlunparse
+
 logging = logmod.getLogger(__name__)
 
 @dataclass
 class Trie:
     """ Main Trie Access class """
     data : InitVar[List[Any]] = field(default=None)
 
@@ -94,8 +93,7 @@
         for key, url_pair in self.query_keys.items():
             count = self.query_key_counts[key]
             result.append("** ({}) {}\n  [[{}][original]]\n  [[{}][filtered]]".format(count,
                                                                                       key,
                                                                                       url_pair[0],
                                                                                       url_pair[1]))
         return "\n".join(result)
-
```

### Comparing `jgdv-0.1.0/jgdv/testing/testing_fixtures.py` & `jgdv-0.1.1/jgdv/testing/testing_fixtures.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,15 +29,14 @@
 
 ##-- logging
 logging = logmod.getLogger(__name__)
 ##-- end logging
 
 import pytest
 import os
-import doot
 
 ##-- imports
 import tempfile
 ##-- end imports
 
 # with tempfile.TemporaryDirectory() as temp_dir:
 #      assert(isisntance(temp_dir, str))
```

### Comparing `jgdv-0.1.0/jgdv/utils/slice.py` & `jgdv-0.1.1/jgdv/utils/slice.py`

 * *Files identical despite different names*

### Comparing `jgdv-0.1.0/jgdv.egg-info/PKG-INFO` & `jgdv-0.1.1/jgdv.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jgdv
-Version: 0.1.0
+Version: 0.1.1
 Author-email: John Grey <jgrey.n.plus.one+dejavu@gmail.com>
 License: * ACAB License
         
         © 2024-03-04 John Grey
         
         To the maximum extent applicable by law, and any licenses of components of this work:
         
@@ -44,15 +44,15 @@
 Project-URL: repository, https://github.com/jgrey4296/jgdv
 Project-URL: changelog, https://github.com/jgrey4296/jgdv/blob/master/CHANGELOG.md
 Classifier: Programming Language :: Python
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: tomlguard
-Requires-Dist: mastodonpy
+Requires-Dist: mastodon.py>=1.8
 Requires-Dist: selenium
 Requires-Dist: numpy
 Requires-Dist: scrapy
 Requires-Dist: pyparsing
 Requires-Dist: construct
 Requires-Dist: networkx
 Requires-Dist: gi
```

### Comparing `jgdv-0.1.0/jgdv.egg-info/SOURCES.txt` & `jgdv-0.1.1/jgdv.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -6,24 +6,19 @@
 jgdv.egg-info/SOURCES.txt
 jgdv.egg-info/dependency_links.txt
 jgdv.egg-info/requires.txt
 jgdv.egg-info/top_level.txt
 jgdv/__tests/__init__.py
 jgdv/_interfaces/__init__.py
 jgdv/_interfaces/accessors.py
-jgdv/_interfaces/cmd.py
-jgdv/_interfaces/control.py
-jgdv/_interfaces/dbm.py
 jgdv/_interfaces/decorator.py
 jgdv/_interfaces/factory.py
 jgdv/_interfaces/loader.py
-jgdv/_interfaces/overlord.py
 jgdv/_interfaces/policy.py
 jgdv/_interfaces/singletons.py
-jgdv/_interfaces/task.py
 jgdv/_types/__init__.py
 jgdv/apis/clingo/__init__.py
 jgdv/apis/clingo/ast.py
 jgdv/apis/clingo/clingo_solver.py
 jgdv/apis/clingo/compiler.py
 jgdv/apis/clingo/parser.py
 jgdv/apis/clingo/reporter.py
@@ -40,15 +35,14 @@
 jgdv/apis/sphinx/directive.py
 jgdv/cli/__init__.py
 jgdv/cli/arg_parser.py
 jgdv/cli/shell.py
 jgdv/cli/speak.py
 jgdv/cli/__tests/test_flexible.py
 jgdv/cli/repl/__init__.py
-jgdv/cli/repl/error.py
 jgdv/cli/repl/repl_commander.py
 jgdv/cli/repl/repl_dsl.py
 jgdv/cli/repl/repl_state.py
 jgdv/cli/repl/commands/__init__.py
 jgdv/cli/repl/commands/break_cmd.py
 jgdv/cli/repl/commands/commands_info.py
 jgdv/cli/repl/commands/control.py
@@ -66,28 +60,33 @@
 jgdv/debugging/frame_helper.py
 jgdv/debugging/human.py
 jgdv/debugging/malloc.py
 jgdv/debugging/running_debugger.py
 jgdv/debugging/timing.py
 jgdv/debugging/trace_helper.py
 jgdv/debugging/util.py
+jgdv/decorators/base.py
 jgdv/decorators/breakpoint.py
 jgdv/decorators/check_protocol.py
 jgdv/decorators/destruction.py
 jgdv/decorators/dsl.py
-jgdv/decorators/key.py
 jgdv/decorators/logging.py
-jgdv/decorators/singletons.py
 jgdv/decorators/util.py
 jgdv/dsl/__init__.py
 jgdv/dsl/consts.py
 jgdv/dsl/ctors.py
 jgdv/dsl/funcs.py
 jgdv/dsl/util.py
+jgdv/enums/__init__.py
+jgdv/enums/location_meta.py
+jgdv/enums/loop_control.py
+jgdv/enums/task_response.py
+jgdv/enums/task_state.py
 jgdv/error/__init__.py
+jgdv/error/repl.py
 jgdv/files/__init__.py
 jgdv/files/json.py
 jgdv/files/mem_map.py
 jgdv/files/metadata.py
 jgdv/files/sha256.py
 jgdv/files/tar.py
 jgdv/files/zip.py
@@ -187,36 +186,51 @@
 jgdv/geom/voronoi/voronoi_drawing.py
 jgdv/geom/voronoi/voronoi_io.py
 jgdv/handlers/__init__.py
 jgdv/handlers/handler.py
 jgdv/handlers/handler_system.py
 jgdv/importing/inspect.py
 jgdv/importing/plugin_loader.py
+jgdv/keys/__init__.py
+jgdv/keys/base.py
+jgdv/keys/decorator.py
+jgdv/keys/formatter.py
+jgdv/keys/multikey.py
+jgdv/keys/path_keys.py
+jgdv/keys/simple.py
+jgdv/location/__init__.py
+jgdv/location/locations.py
+jgdv/location/toml_loc.py
 jgdv/logging/__init__.py
 jgdv/logging/log_colour.py
+jgdv/logging/log_config.py
 jgdv/logging/log_context.py
 jgdv/logging/stdout_capture.py
 jgdv/math/__init__.py
 jgdv/math/colour.py
 jgdv/math/comparison.py
 jgdv/math/easings.py
 jgdv/math/matrices.py
 jgdv/math/parabola.py
 jgdv/math/quadratic.py
 jgdv/math/quantize.py
 jgdv/math/rand.py
 jgdv/math/sorting.py
 jgdv/math/umath.py
 jgdv/math/utils.py
+jgdv/mixins/__init__.py
+jgdv/mixins/enums.py
+jgdv/mixins/param_spec.py
+jgdv/mixins/path_manip.py
+jgdv/mixins/zipper.py
 jgdv/setup/asyncio_client.py
 jgdv/setup/asyncio_server.py
 jgdv/setup/gtk.py
 jgdv/setup/hooks.py
 jgdv/setup/importing.py
-jgdv/setup/logging.py
 jgdv/setup/main.py
 jgdv/setup/pyparsing.py
 jgdv/setup/setup.py
 jgdv/setup/tkinter.py
 jgdv/spiders/__init__.py
 jgdv/spiders/actions.py
 jgdv/spiders/caching.py
@@ -225,16 +239,20 @@
 jgdv/spiders/mixin.py
 jgdv/spiders/pipeline.py
 jgdv/spiders/runner.py
 jgdv/spiders/spiders.py
 jgdv/spiders/tracker.py
 jgdv/spiders/__tests/test_runner.py
 jgdv/spiders/__tests/test_tracker.py
-jgdv/structs/enums.py
+jgdv/structs/artifact.py
+jgdv/structs/code_ref.py
+jgdv/structs/name.py
+jgdv/structs/param_spec.py
 jgdv/structs/regex.py
+jgdv/structs/trace.py
 jgdv/structs/heap/__init__.py
 jgdv/structs/heap/element.py
 jgdv/structs/heap/heap.py
 jgdv/structs/proxy/base.py
 jgdv/structs/proxy/iter_proxy.py
 jgdv/structs/proxy/proxy.py
 jgdv/structs/proxy/proxy_mixin.py
```

### Comparing `jgdv-0.1.0/pyproject.toml` & `jgdv-0.1.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [project]
 name            = "jgdv"
-version         = "0.1.0"
+version         = "0.1.1"
 description     = ""
 readme          = "README.md"
 requires-python = ">=3.10"
 license         = {file = "LICENSE"}
 keywords        = []
 authors         = [
   {name  = "John Grey", email = "jgrey.n.plus.one+dejavu@gmail.com"},
 ]
 classifiers     = [
   "Programming Language :: Python"
 ]
 
 dependencies   = [
                "tomlguard",
-               "mastodonpy",
+               "mastodon.py>=1.8",
                "selenium",
                "numpy",
                "scrapy",
                "pyparsing",
                "construct",
                "networkx",
                "gi"
@@ -147,15 +147,15 @@
 
 [tool.sphinx.html.options]
 
 ##-- end sphinx
 
 ##-- bumpver
 [tool.bumpver]
-current_version    = "0.1.0"
+current_version    = "0.1.1"
 version_pattern    = "MAJOR.MINOR.PATCH"
 commit_message     = "[bump]: version {old_version} -> {new_version}"
 tag_message        = "{new_version}"
 tag_scope          = "default"
 commit             = true
 tag                = true
 # pre_commit_hook  = ""
```

