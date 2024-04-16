# Comparing `tmp/nanolab-0.0.8.tar.gz` & `tmp/nanolab-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nanolab-0.0.8.tar", last modified: Thu Aug 10 07:57:31 2023, max compression
+gzip compressed data, was "nanolab-0.0.9.tar", last modified: Thu Aug 10 18:50:57 2023, max compression
```

## Comparing `nanolab-0.0.8.tar` & `nanolab-0.0.9.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-10 07:57:31.831551 nanolab-0.0.8/
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-07 22:25:09.000000 nanolab-0.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1567 2023-08-10 07:57:31.831551 nanolab-0.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1371 2023-05-09 13:33:33.000000 nanolab-0.0.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-10 07:57:31.831551 nanolab-0.0.8/nanolab/
--rw-r--r--   0 root         (0) root         (0)       22 2023-08-10 07:52:37.000000 nanolab-0.0.8/nanolab/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-10 07:57:31.831551 nanolab-0.0.8/nanolab/command/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-07 08:00:48.000000 nanolab-0.0.8/nanolab/command/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1212 2023-05-10 21:50:30.000000 nanolab-0.0.8/nanolab/command/command.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-10 07:57:31.831551 nanolab-0.0.8/nanolab/command/mixins/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-07 13:06:25.000000 nanolab-0.0.8/nanolab/command/mixins/__init__.py
--rw-r--r--   0 root         (0) root         (0)      906 2023-05-10 21:50:04.000000 nanolab-0.0.8/nanolab/command/mixins/base_mixin.py
--rw-r--r--   0 root         (0) root         (0)      839 2023-05-10 21:47:56.000000 nanolab-0.0.8/nanolab/command/mixins/bash_command_mixin.py
--rw-r--r--   0 root         (0) root         (0)     1589 2023-05-10 21:48:04.000000 nanolab-0.0.8/nanolab/command/mixins/python_command_mixin.py
--rw-r--r--   0 root         (0) root         (0)     3111 2023-05-25 15:12:04.000000 nanolab-0.0.8/nanolab/command/mixins/threaded_command_mixin.py
--rw-r--r--   0 root         (0) root         (0)      776 2023-05-12 12:46:16.000000 nanolab-0.0.8/nanolab/decorators.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-10 07:57:31.831551 nanolab-0.0.8/nanolab/loggers/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-12 12:46:16.000000 nanolab-0.0.8/nanolab/loggers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1810 2023-05-12 12:46:16.000000 nanolab-0.0.8/nanolab/loggers/builders.py
--rw-r--r--   0 root         (0) root         (0)      638 2023-05-12 12:46:16.000000 nanolab-0.0.8/nanolab/loggers/contracts.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-10 07:57:31.831551 nanolab-0.0.8/nanolab/loggers/factories/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-12 12:46:16.000000 nanolab-0.0.8/nanolab/loggers/factories/__init__.py
--rw-r--r--   0 root         (0) root         (0)      627 2023-05-12 12:46:16.000000 nanolab-0.0.8/nanolab/loggers/factories/logger_factory.py
--rw-r--r--   0 root         (0) root         (0)      568 2023-05-12 12:46:16.000000 nanolab-0.0.8/nanolab/loggers/factories/sink_factory.py
--rw-r--r--   0 root         (0) root         (0)     2347 2023-05-16 08:04:03.000000 nanolab-0.0.8/nanolab/loggers/logger_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-10 07:57:31.831551 nanolab-0.0.8/nanolab/loggers/sinks/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-12 12:46:16.000000 nanolab-0.0.8/nanolab/loggers/sinks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1167 2023-05-14 16:18:46.000000 nanolab-0.0.8/nanolab/loggers/sinks/console_sink.py
--rw-r--r--   0 root         (0) root         (0)      997 2023-05-12 12:46:16.000000 nanolab-0.0.8/nanolab/loggers/sinks/csv_sink.py
--rw-r--r--   0 root         (0) root         (0)     3771 2023-05-16 08:04:03.000000 nanolab-0.0.8/nanolab/loggers/sinks/sql_sink.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-10 07:57:31.831551 nanolab-0.0.8/nanolab/loggers/sources/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-12 12:46:16.000000 nanolab-0.0.8/nanolab/loggers/sources/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5540 2023-05-12 21:13:03.000000 nanolab-0.0.8/nanolab/loggers/sources/rpc_logger.py
--rwxr-xr-x   0 root         (0) root         (0)      459 2023-05-09 11:04:51.000000 nanolab-0.0.8/nanolab/main.py
--rw-r--r--   0 root         (0) root         (0)     8610 2023-08-09 21:41:30.000000 nanolab-0.0.8/nanolab/node_interaction.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-10 07:57:31.831551 nanolab-0.0.8/nanolab/publisher/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-16 08:04:03.000000 nanolab-0.0.8/nanolab/publisher/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5558 2023-05-16 08:04:03.000000 nanolab-0.0.8/nanolab/publisher/block_asserts.py
--rw-r--r--   0 root         (0) root         (0)      284 2023-05-16 08:04:03.000000 nanolab-0.0.8/nanolab/publisher/block_event.py
--rw-r--r--   0 root         (0) root         (0)     4580 2023-05-16 08:04:03.000000 nanolab-0.0.8/nanolab/publisher/block_generator.py
--rw-r--r--   0 root         (0) root         (0)     4864 2023-05-16 08:04:03.000000 nanolab-0.0.8/nanolab/publisher/confirmation_stats.py
--rw-r--r--   0 root         (0) root         (0)      442 2023-05-16 08:04:03.000000 nanolab-0.0.8/nanolab/publisher/event_bus.py
--rw-r--r--   0 root         (0) root         (0)     5059 2023-05-16 08:04:03.000000 nanolab-0.0.8/nanolab/publisher/test_case.py
--rw-r--r--   0 root         (0) root         (0)     1205 2023-05-16 08:04:03.000000 nanolab-0.0.8/nanolab/pycmd.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-10 07:57:31.831551 nanolab-0.0.8/nanolab/snippets/
--rw-r--r--   0 root         (0) root         (0)     4228 2023-05-16 08:04:03.000000 nanolab-0.0.8/nanolab/snippets/default_snips.json
--rw-r--r--   0 root         (0) root         (0)     2606 2023-05-12 23:35:30.000000 nanolab-0.0.8/nanolab/snippets/test_snippets.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-10 07:57:31.831551 nanolab-0.0.8/nanolab/src/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-07 06:56:43.000000 nanolab-0.0.8/nanolab/src/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3788 2023-05-16 07:27:13.000000 nanolab-0.0.8/nanolab/src/argparse_commands.py
--rw-r--r--   0 root         (0) root         (0)     4938 2023-08-09 22:01:00.000000 nanolab-0.0.8/nanolab/src/config_handler.py
--rw-r--r--   0 root         (0) root         (0)     6308 2023-05-16 08:04:03.000000 nanolab-0.0.8/nanolab/src/config_loader.py
--rw-r--r--   0 root         (0) root         (0)     1721 2023-08-09 21:41:32.000000 nanolab-0.0.8/nanolab/src/github.py
--rw-r--r--   0 root         (0) root         (0)    12606 2023-05-16 08:04:03.000000 nanolab-0.0.8/nanolab/src/nano_rpc.py
--rw-r--r--   0 root         (0) root         (0)     1701 2023-05-08 19:55:35.000000 nanolab-0.0.8/nanolab/src/resolver.py
--rw-r--r--   0 root         (0) root         (0)      972 2023-05-10 13:22:47.000000 nanolab-0.0.8/nanolab/src/snippet_manager.py
--rw-r--r--   0 root         (0) root         (0)     3138 2023-05-12 21:31:38.000000 nanolab-0.0.8/nanolab/src/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-10 07:57:31.831551 nanolab-0.0.8/nanolab/xnomin/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 21:19:13.000000 nanolab-0.0.8/nanolab/xnomin/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1688 2023-04-24 21:16:18.000000 nanolab-0.0.8/nanolab/xnomin/acctools.py
--rw-r--r--   0 root         (0) root         (0)     7345 2023-08-09 21:41:30.000000 nanolab-0.0.8/nanolab/xnomin/handshake.py
--rw-r--r--   0 root         (0) root         (0)    18867 2023-05-12 22:26:37.000000 nanolab-0.0.8/nanolab/xnomin/peers.py
--rwxr-xr-x   0 root         (0) root         (0)     2424 2023-05-10 19:36:27.000000 nanolab-0.0.8/nanolab/xnomin/telemetry_req.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-10 07:57:31.831551 nanolab-0.0.8/nanolab.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1567 2023-08-10 07:57:31.000000 nanolab-0.0.8/nanolab.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1731 2023-08-10 07:57:31.000000 nanolab-0.0.8/nanolab.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-10 07:57:31.000000 nanolab-0.0.8/nanolab.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       46 2023-08-10 07:57:31.000000 nanolab-0.0.8/nanolab.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       28 2023-08-10 07:57:31.000000 nanolab-0.0.8/nanolab.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-08-10 07:57:31.000000 nanolab-0.0.8/nanolab.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-08-10 07:57:31.831551 nanolab-0.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      641 2023-08-10 07:57:27.000000 nanolab-0.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-10 18:50:57.149245 nanolab-0.0.9/
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-07 22:25:09.000000 nanolab-0.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1567 2023-08-10 18:50:57.149245 nanolab-0.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1371 2023-05-09 13:33:33.000000 nanolab-0.0.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-10 18:50:57.149245 nanolab-0.0.9/nanolab/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-08-10 18:50:38.000000 nanolab-0.0.9/nanolab/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-10 18:50:57.149245 nanolab-0.0.9/nanolab/command/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-07 08:00:48.000000 nanolab-0.0.9/nanolab/command/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1212 2023-05-10 21:50:30.000000 nanolab-0.0.9/nanolab/command/command.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-10 18:50:57.149245 nanolab-0.0.9/nanolab/command/mixins/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-07 13:06:25.000000 nanolab-0.0.9/nanolab/command/mixins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      907 2023-08-10 18:50:33.000000 nanolab-0.0.9/nanolab/command/mixins/base_mixin.py
+-rw-r--r--   0 root         (0) root         (0)      753 2023-08-10 18:50:33.000000 nanolab-0.0.9/nanolab/command/mixins/bash_command_mixin.py
+-rw-r--r--   0 root         (0) root         (0)     1589 2023-05-10 21:48:04.000000 nanolab-0.0.9/nanolab/command/mixins/python_command_mixin.py
+-rw-r--r--   0 root         (0) root         (0)     3111 2023-05-25 15:12:04.000000 nanolab-0.0.9/nanolab/command/mixins/threaded_command_mixin.py
+-rw-r--r--   0 root         (0) root         (0)      776 2023-05-12 12:46:16.000000 nanolab-0.0.9/nanolab/decorators.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-10 18:50:57.149245 nanolab-0.0.9/nanolab/loggers/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-12 12:46:16.000000 nanolab-0.0.9/nanolab/loggers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1810 2023-05-12 12:46:16.000000 nanolab-0.0.9/nanolab/loggers/builders.py
+-rw-r--r--   0 root         (0) root         (0)      638 2023-05-12 12:46:16.000000 nanolab-0.0.9/nanolab/loggers/contracts.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-10 18:50:57.149245 nanolab-0.0.9/nanolab/loggers/factories/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-12 12:46:16.000000 nanolab-0.0.9/nanolab/loggers/factories/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      627 2023-05-12 12:46:16.000000 nanolab-0.0.9/nanolab/loggers/factories/logger_factory.py
+-rw-r--r--   0 root         (0) root         (0)      568 2023-05-12 12:46:16.000000 nanolab-0.0.9/nanolab/loggers/factories/sink_factory.py
+-rw-r--r--   0 root         (0) root         (0)     2347 2023-05-16 08:04:03.000000 nanolab-0.0.9/nanolab/loggers/logger_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-10 18:50:57.149245 nanolab-0.0.9/nanolab/loggers/sinks/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-12 12:46:16.000000 nanolab-0.0.9/nanolab/loggers/sinks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1167 2023-05-14 16:18:46.000000 nanolab-0.0.9/nanolab/loggers/sinks/console_sink.py
+-rw-r--r--   0 root         (0) root         (0)      997 2023-05-12 12:46:16.000000 nanolab-0.0.9/nanolab/loggers/sinks/csv_sink.py
+-rw-r--r--   0 root         (0) root         (0)     3771 2023-05-16 08:04:03.000000 nanolab-0.0.9/nanolab/loggers/sinks/sql_sink.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-10 18:50:57.149245 nanolab-0.0.9/nanolab/loggers/sources/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-12 12:46:16.000000 nanolab-0.0.9/nanolab/loggers/sources/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5540 2023-05-12 21:13:03.000000 nanolab-0.0.9/nanolab/loggers/sources/rpc_logger.py
+-rwxr-xr-x   0 root         (0) root         (0)      459 2023-05-09 11:04:51.000000 nanolab-0.0.9/nanolab/main.py
+-rw-r--r--   0 root         (0) root         (0)     8610 2023-08-09 21:41:30.000000 nanolab-0.0.9/nanolab/node_interaction.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-10 18:50:57.149245 nanolab-0.0.9/nanolab/publisher/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-16 08:04:03.000000 nanolab-0.0.9/nanolab/publisher/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5558 2023-05-16 08:04:03.000000 nanolab-0.0.9/nanolab/publisher/block_asserts.py
+-rw-r--r--   0 root         (0) root         (0)      284 2023-05-16 08:04:03.000000 nanolab-0.0.9/nanolab/publisher/block_event.py
+-rw-r--r--   0 root         (0) root         (0)     4580 2023-05-16 08:04:03.000000 nanolab-0.0.9/nanolab/publisher/block_generator.py
+-rw-r--r--   0 root         (0) root         (0)     4864 2023-05-16 08:04:03.000000 nanolab-0.0.9/nanolab/publisher/confirmation_stats.py
+-rw-r--r--   0 root         (0) root         (0)      442 2023-05-16 08:04:03.000000 nanolab-0.0.9/nanolab/publisher/event_bus.py
+-rw-r--r--   0 root         (0) root         (0)     5059 2023-05-16 08:04:03.000000 nanolab-0.0.9/nanolab/publisher/test_case.py
+-rw-r--r--   0 root         (0) root         (0)     1205 2023-05-16 08:04:03.000000 nanolab-0.0.9/nanolab/pycmd.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-10 18:50:57.149245 nanolab-0.0.9/nanolab/snippets/
+-rw-r--r--   0 root         (0) root         (0)     4228 2023-05-16 08:04:03.000000 nanolab-0.0.9/nanolab/snippets/default_snips.json
+-rw-r--r--   0 root         (0) root         (0)     2606 2023-05-12 23:35:30.000000 nanolab-0.0.9/nanolab/snippets/test_snippets.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-10 18:50:57.149245 nanolab-0.0.9/nanolab/src/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-07 06:56:43.000000 nanolab-0.0.9/nanolab/src/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3803 2023-08-10 18:50:33.000000 nanolab-0.0.9/nanolab/src/argparse_commands.py
+-rw-r--r--   0 root         (0) root         (0)     4938 2023-08-09 22:01:00.000000 nanolab-0.0.9/nanolab/src/config_handler.py
+-rw-r--r--   0 root         (0) root         (0)     6309 2023-08-10 18:50:33.000000 nanolab-0.0.9/nanolab/src/config_loader.py
+-rw-r--r--   0 root         (0) root         (0)     1721 2023-08-09 21:41:32.000000 nanolab-0.0.9/nanolab/src/github.py
+-rw-r--r--   0 root         (0) root         (0)    12606 2023-05-16 08:04:03.000000 nanolab-0.0.9/nanolab/src/nano_rpc.py
+-rw-r--r--   0 root         (0) root         (0)     1701 2023-05-08 19:55:35.000000 nanolab-0.0.9/nanolab/src/resolver.py
+-rw-r--r--   0 root         (0) root         (0)      972 2023-05-10 13:22:47.000000 nanolab-0.0.9/nanolab/src/snippet_manager.py
+-rw-r--r--   0 root         (0) root         (0)     3138 2023-05-12 21:31:38.000000 nanolab-0.0.9/nanolab/src/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-10 18:50:57.149245 nanolab-0.0.9/nanolab/xnomin/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 21:19:13.000000 nanolab-0.0.9/nanolab/xnomin/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1688 2023-04-24 21:16:18.000000 nanolab-0.0.9/nanolab/xnomin/acctools.py
+-rw-r--r--   0 root         (0) root         (0)     7345 2023-08-09 21:41:30.000000 nanolab-0.0.9/nanolab/xnomin/handshake.py
+-rw-r--r--   0 root         (0) root         (0)    18867 2023-05-12 22:26:37.000000 nanolab-0.0.9/nanolab/xnomin/peers.py
+-rwxr-xr-x   0 root         (0) root         (0)     2424 2023-05-10 19:36:27.000000 nanolab-0.0.9/nanolab/xnomin/telemetry_req.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-10 18:50:57.149245 nanolab-0.0.9/nanolab.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1567 2023-08-10 18:50:57.000000 nanolab-0.0.9/nanolab.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1731 2023-08-10 18:50:57.000000 nanolab-0.0.9/nanolab.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-10 18:50:57.000000 nanolab-0.0.9/nanolab.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       46 2023-08-10 18:50:57.000000 nanolab-0.0.9/nanolab.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       36 2023-08-10 18:50:57.000000 nanolab-0.0.9/nanolab.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-08-10 18:50:57.000000 nanolab-0.0.9/nanolab.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-10 18:50:57.153245 nanolab-0.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      652 2023-08-10 18:50:38.000000 nanolab-0.0.9/setup.py
```

### Comparing `nanolab-0.0.8/PKG-INFO` & `nanolab-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanolab
-Version: 0.0.8
+Version: 0.0.9
 Summary: testing tool using nanomock
 Home-page: https://github.com/gr0vity-dev/nanolab
 Author: gr0vity
 Description-Content-Type: text/markdown
 
 ##NanoLab
```

### Comparing `nanolab-0.0.8/README.md` & `nanolab-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `nanolab-0.0.8/nanolab/command/command.py` & `nanolab-0.0.9/nanolab/command/command.py`

 * *Files identical despite different names*

### Comparing `nanolab-0.0.8/nanolab/command/mixins/base_mixin.py` & `nanolab-0.0.9/nanolab/command/mixins/base_mixin.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     def __init__(self, command_instance):
         self.command_instance = command_instance
         self.logger = logging.getLogger(__name__)
 
     def _get_completed_variables(self):
         variables = self.command_instance.command_config.get('variables', {})
 
-        #add global variables
+        # add global variables
         variables["docker_tag"] = environ["docker_tag"]
         return variables
 
     def _get_filtered_variables(self, method):
         variables = self._get_completed_variables()
         method_parameters = self._get_method_parameters(method)
         return {
```

### Comparing `nanolab-0.0.8/nanolab/command/mixins/bash_command_mixin.py` & `nanolab-0.0.9/nanolab/command/mixins/bash_command_mixin.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,18 +8,16 @@
         pass
         # Validation logic for BashCommand
 
     def execute(self):
         variables = self._get_completed_variables()
         command = self.command_instance.command_config['command'].format(
             **variables)
-        process = subprocess.run(command,
-                                 shell=True,
-                                 text=True,
-                                 capture_output=True)
+        process = subprocess.run(
+            command, shell=True, text=True, capture_output=True)
 
         if process.returncode != 0:
             print(
                 f"Error executing command: {command}\nError: {process.stderr.strip()}"
             )
         else:
             response = process.stdout.strip() or process.stderr.strip(
```

### Comparing `nanolab-0.0.8/nanolab/command/mixins/python_command_mixin.py` & `nanolab-0.0.9/nanolab/command/mixins/python_command_mixin.py`

 * *Files identical despite different names*

### Comparing `nanolab-0.0.8/nanolab/command/mixins/threaded_command_mixin.py` & `nanolab-0.0.9/nanolab/command/mixins/threaded_command_mixin.py`

 * *Files identical despite different names*

### Comparing `nanolab-0.0.8/nanolab/decorators.py` & `nanolab-0.0.9/nanolab/decorators.py`

 * *Files identical despite different names*

### Comparing `nanolab-0.0.8/nanolab/loggers/builders.py` & `nanolab-0.0.9/nanolab/loggers/builders.py`

 * *Files identical despite different names*

### Comparing `nanolab-0.0.8/nanolab/loggers/contracts.py` & `nanolab-0.0.9/nanolab/loggers/contracts.py`

 * *Files identical despite different names*

### Comparing `nanolab-0.0.8/nanolab/loggers/factories/logger_factory.py` & `nanolab-0.0.9/nanolab/loggers/factories/logger_factory.py`

 * *Files identical despite different names*

### Comparing `nanolab-0.0.8/nanolab/loggers/factories/sink_factory.py` & `nanolab-0.0.9/nanolab/loggers/factories/sink_factory.py`

 * *Files identical despite different names*

### Comparing `nanolab-0.0.8/nanolab/loggers/logger_manager.py` & `nanolab-0.0.9/nanolab/loggers/logger_manager.py`

 * *Files identical despite different names*

### Comparing `nanolab-0.0.8/nanolab/loggers/sinks/console_sink.py` & `nanolab-0.0.9/nanolab/loggers/sinks/console_sink.py`

 * *Files identical despite different names*

### Comparing `nanolab-0.0.8/nanolab/loggers/sinks/csv_sink.py` & `nanolab-0.0.9/nanolab/loggers/sinks/csv_sink.py`

 * *Files identical despite different names*

### Comparing `nanolab-0.0.8/nanolab/loggers/sinks/sql_sink.py` & `nanolab-0.0.9/nanolab/loggers/sinks/sql_sink.py`

 * *Files identical despite different names*

### Comparing `nanolab-0.0.8/nanolab/loggers/sources/rpc_logger.py` & `nanolab-0.0.9/nanolab/loggers/sources/rpc_logger.py`

 * *Files identical despite different names*

### Comparing `nanolab-0.0.8/nanolab/node_interaction.py` & `nanolab-0.0.9/nanolab/node_interaction.py`

 * *Files identical despite different names*

### Comparing `nanolab-0.0.8/nanolab/publisher/block_asserts.py` & `nanolab-0.0.9/nanolab/publisher/block_asserts.py`

 * *Files identical despite different names*

### Comparing `nanolab-0.0.8/nanolab/publisher/block_generator.py` & `nanolab-0.0.9/nanolab/publisher/block_generator.py`

 * *Files identical despite different names*

### Comparing `nanolab-0.0.8/nanolab/publisher/confirmation_stats.py` & `nanolab-0.0.9/nanolab/publisher/confirmation_stats.py`

 * *Files identical despite different names*

### Comparing `nanolab-0.0.8/nanolab/publisher/test_case.py` & `nanolab-0.0.9/nanolab/publisher/test_case.py`

 * *Files identical despite different names*

### Comparing `nanolab-0.0.8/nanolab/pycmd.py` & `nanolab-0.0.9/nanolab/pycmd.py`

 * *Files identical despite different names*

### Comparing `nanolab-0.0.8/nanolab/snippets/default_snips.json` & `nanolab-0.0.9/nanolab/snippets/default_snips.json`

 * *Files identical despite different names*

### Comparing `nanolab-0.0.8/nanolab/snippets/test_snippets.json` & `nanolab-0.0.9/nanolab/snippets/test_snippets.json`

 * *Files identical despite different names*

### Comparing `nanolab-0.0.8/nanolab/src/argparse_commands.py` & `nanolab-0.0.9/nanolab/src/argparse_commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,23 +66,24 @@
     def run(self):
         path_handler = ConfigPathHandler(self.args.testcase)
         resource_handler = ConfigResourceHandler(self.github_api, path_handler)
 
         #
         extract_packaged_data_to_disk(path_handler.get_snippets_path())
 
-        #copy config to disk
+        # copy config to disk
         config_path = resource_handler.copy_config_file(
             path_handler.config_copy_file_path)
 
-        #resolve and downlaod resources defiend in the config
+        # resolve and downlaod resources defiend in the config
         resolved_config = resource_handler.download_and_replace_resources(
             config_path, path_handler.downloads_path)
-        #replace docker_tags with commandline
-        if self.args.image: resolved_config["docker_tags"] = self.args.image
+        # replace docker_tags with commandline
+        if self.args.image:
+            resolved_config["docker_tags"] = self.args.image
 
         resolved_path = path_handler.get_resolved_config_path()
         snippet_path = path_handler.get_snippets_path()
 
         snippet_manager = SnippetManager(snippet_path)
         config_loader = ConfigLoader(snippet_manager)
         final_config = config_loader.load_config(resolved_config)
```

### Comparing `nanolab-0.0.8/nanolab/src/config_handler.py` & `nanolab-0.0.9/nanolab/src/config_handler.py`

 * *Files identical despite different names*

### Comparing `nanolab-0.0.8/nanolab/src/config_loader.py` & `nanolab-0.0.9/nanolab/src/config_loader.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -155,8 +155,8 @@
             for command_config in config["commands"]:
                 ConfigCommandExecutor.execute_command(command_config)
 
     @staticmethod
     def execute_command(command_config):
         command = Command(command_config)
         command.validate()
-        command.execute()
+        command.execute()
```

### Comparing `nanolab-0.0.8/nanolab/src/github.py` & `nanolab-0.0.9/nanolab/src/github.py`

 * *Files identical despite different names*

### Comparing `nanolab-0.0.8/nanolab/src/nano_rpc.py` & `nanolab-0.0.9/nanolab/src/nano_rpc.py`

 * *Files identical despite different names*

### Comparing `nanolab-0.0.8/nanolab/src/resolver.py` & `nanolab-0.0.9/nanolab/src/resolver.py`

 * *Files identical despite different names*

### Comparing `nanolab-0.0.8/nanolab/src/snippet_manager.py` & `nanolab-0.0.9/nanolab/src/snippet_manager.py`

 * *Files identical despite different names*

### Comparing `nanolab-0.0.8/nanolab/src/utils.py` & `nanolab-0.0.9/nanolab/src/utils.py`

 * *Files identical despite different names*

### Comparing `nanolab-0.0.8/nanolab/xnomin/acctools.py` & `nanolab-0.0.9/nanolab/xnomin/acctools.py`

 * *Files identical despite different names*

### Comparing `nanolab-0.0.8/nanolab/xnomin/handshake.py` & `nanolab-0.0.9/nanolab/xnomin/handshake.py`

 * *Files identical despite different names*

### Comparing `nanolab-0.0.8/nanolab/xnomin/peers.py` & `nanolab-0.0.9/nanolab/xnomin/peers.py`

 * *Files identical despite different names*

### Comparing `nanolab-0.0.8/nanolab/xnomin/telemetry_req.py` & `nanolab-0.0.9/nanolab/xnomin/telemetry_req.py`

 * *Files identical despite different names*

### Comparing `nanolab-0.0.8/nanolab.egg-info/PKG-INFO` & `nanolab-0.0.9/nanolab.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanolab
-Version: 0.0.8
+Version: 0.0.9
 Summary: testing tool using nanomock
 Home-page: https://github.com/gr0vity-dev/nanolab
 Author: gr0vity
 Description-Content-Type: text/markdown
 
 ##NanoLab
```

### Comparing `nanolab-0.0.8/nanolab.egg-info/SOURCES.txt` & `nanolab-0.0.9/nanolab.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nanolab-0.0.8/setup.py` & `nanolab-0.0.9/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(name="nanolab",
-      version="0.0.8",
+      version="0.0.9",
       author="gr0vity",
       description="testing tool using nanomock",
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/gr0vity-dev/nanolab",
       packages=find_packages(exclude=["unit_tests"]),
       include_package_data=True,
-      install_requires=["nanomock>=0.0.12", "sqlalchemy"],
+      install_requires=["nanomock>=0.0.14", "sqlalchemy", "aiohttp"],
       entry_points={
           'console_scripts': [
               'nanolab=nanolab.main:main',
           ],
       })
```

