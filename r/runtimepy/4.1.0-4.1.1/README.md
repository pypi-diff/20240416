# Comparing `tmp/runtimepy-4.1.0.tar.gz` & `tmp/runtimepy-4.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "runtimepy-4.1.0.tar", last modified: Sun Apr 14 07:07:29 2024, max compression
+gzip compressed data, was "runtimepy-4.1.1.tar", last modified: Tue Apr 16 03:04:51 2024, max compression
```

## Comparing `runtimepy-4.1.0.tar` & `runtimepy-4.1.1.tar`

### file list

```diff
@@ -1,291 +1,292 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 07:07:29.714508 runtimepy-4.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-14 07:05:27.000000 runtimepy-4.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7055 2024-04-14 07:07:29.714508 runtimepy-4.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5390 2024-04-14 07:05:27.000000 runtimepy-4.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-14 07:05:27.000000 runtimepy-4.1.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 07:07:29.678508 runtimepy-4.1.0/runtimepy/
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 07:07:29.678508 runtimepy-4.1.0/runtimepy/channel/
--rw-r--r--   0 runner    (1001) docker     (127)     3243 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/channel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 07:07:29.682508 runtimepy-4.1.0/runtimepy/channel/environment/
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/channel/environment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3413 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/channel/environment/array.py
--rw-r--r--   0 runner    (1001) docker     (127)     9188 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/channel/environment/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 07:07:29.682508 runtimepy-4.1.0/runtimepy/channel/environment/command/
--rw-r--r--   0 runner    (1001) docker     (127)     8145 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/channel/environment/command/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/channel/environment/command/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     5669 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/channel/environment/command/processor.py
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/channel/environment/command/result.py
--rw-r--r--   0 runner    (1001) docker     (127)     5562 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/channel/environment/create.py
--rw-r--r--   0 runner    (1001) docker     (127)     6949 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/channel/environment/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/channel/environment/sample.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 07:07:29.682508 runtimepy-4.1.0/runtimepy/channel/event/
--rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/channel/event/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/channel/event/header.py
--rw-r--r--   0 runner    (1001) docker     (127)     5774 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/channel/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 07:07:29.682508 runtimepy-4.1.0/runtimepy/codec/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/codec/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 07:07:29.682508 runtimepy-4.1.0/runtimepy/codec/protocol/
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/codec/protocol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/codec/protocol/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4107 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/codec/protocol/json.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 07:07:29.682508 runtimepy-4.1.0/runtimepy/codec/system/
--rw-r--r--   0 runner    (1001) docker     (127)     6939 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/codec/system/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 07:07:29.682508 runtimepy-4.1.0/runtimepy/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/commands/all.py
--rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/commands/arbiter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/commands/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     3767 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/commands/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/commands/task.py
--rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/commands/tui.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 07:07:29.686508 runtimepy-4.1.0/runtimepy/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 07:07:29.686508 runtimepy-4.1.0/runtimepy/data/css/
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/data/css/bootstrap_extra.css
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/data/css/main.css
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/data/dummy_load.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/data/factories.yaml
--rw-r--r--   0 runner    (1001) docker     (127)   362870 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/data/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 07:07:29.686508 runtimepy-4.1.0/runtimepy/data/js/
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/data/js/DataConnection.js
--rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/data/js/JsonConnection.js
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/data/js/audio.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 07:07:29.686508 runtimepy-4.1.0/runtimepy/data/js/classes/
--rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/data/js/classes/App.js
--rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/data/js/classes/ChannelTable.js
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/data/js/classes/DataConnection.js
--rw-r--r--   0 runner    (1001) docker     (127)     2858 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/data/js/classes/JsonConnection.js
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/data/js/classes/Plot.js
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/data/js/classes/PlotManager.js
--rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/data/js/classes/TabFilter.js
--rw-r--r--   0 runner    (1001) docker     (127)     7567 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/data/js/classes/TabInterface.js
--rw-r--r--   0 runner    (1001) docker     (127)     3337 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/data/js/classes/WindowHashManager.js
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/data/js/classes/WorkerInterface.js
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/data/js/init.js
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/data/js/main.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 07:07:29.690508 runtimepy-4.1.0/runtimepy/data/js/tab/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/data/js/tab/env.js
--rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/data/js/tab/sound.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 07:07:29.690508 runtimepy-4.1.0/runtimepy/data/js/unused/
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/data/js/unused/pyodide.js
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/data/js/util.js
--rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/data/js/worker.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 07:07:29.690508 runtimepy-4.1.0/runtimepy/data/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/data/schemas/BitFields.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/data/schemas/Channel.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/data/schemas/ChannelCommand.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/data/schemas/ChannelRegistry.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/data/schemas/ClientConnectionConfig.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/data/schemas/ConnectionArbiterConfig.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/data/schemas/EnumRegistry.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/data/schemas/FindFile.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/data/schemas/RuntimeEnum.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/data/schemas/ServerConnectionConfig.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/data/schemas/StructConfig.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/data/schemas/TaskConfig.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/data/schemas/has_factory.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/data/schemas/has_name.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/data/schemas/has_request_flag.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/data/server.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/data/server_base.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/data/server_dev.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/dev_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/entry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 07:07:29.690508 runtimepy-4.1.0/runtimepy/enum/
--rw-r--r--   0 runner    (1001) docker     (127)     5819 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/enum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/enum/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/enum/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     5390 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/mapping.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 07:07:29.690508 runtimepy-4.1.0/runtimepy/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/metrics/channel.py
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/metrics/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/metrics/task.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 07:07:29.694508 runtimepy-4.1.0/runtimepy/mixins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/mixins/async_command.py
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/mixins/enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/mixins/environment.py
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/mixins/finalize.py
--rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/mixins/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/mixins/regex.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 07:07:29.694508 runtimepy-4.1.0/runtimepy/net/
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/net/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 07:07:29.694508 runtimepy-4.1.0/runtimepy/net/apps/
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/net/apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 07:07:29.694508 runtimepy-4.1.0/runtimepy/net/arbiter/
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/net/arbiter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13605 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/net/arbiter/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 07:07:29.694508 runtimepy-4.1.0/runtimepy/net/arbiter/config/
--rw-r--r--   0 runner    (1001) docker     (127)     7632 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/net/arbiter/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2607 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/net/arbiter/config/codec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/net/arbiter/config/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 07:07:29.698508 runtimepy-4.1.0/runtimepy/net/arbiter/factory/
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/net/arbiter/factory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3690 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/net/arbiter/factory/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/net/arbiter/factory/task.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 07:07:29.698508 runtimepy-4.1.0/runtimepy/net/arbiter/housekeeping/
--rw-r--r--   0 runner    (1001) docker     (127)     2318 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/net/arbiter/housekeeping/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 07:07:29.698508 runtimepy-4.1.0/runtimepy/net/arbiter/imports/
--rw-r--r--   0 runner    (1001) docker     (127)     3430 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/net/arbiter/imports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/net/arbiter/imports/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     6382 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/net/arbiter/info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/net/arbiter/result.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 07:07:29.698508 runtimepy-4.1.0/runtimepy/net/arbiter/struct/
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/net/arbiter/struct/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/net/arbiter/task.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 07:07:29.698508 runtimepy-4.1.0/runtimepy/net/arbiter/tcp/
--rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/net/arbiter/tcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      742 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/net/arbiter/tcp/json.py
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/net/arbiter/udp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/net/arbiter/websocket.py
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/net/backoff.py
--rw-r--r--   0 runner    (1001) docker     (127)    11894 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/net/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 07:07:29.698508 runtimepy-4.1.0/runtimepy/net/factories/
--rw-r--r--   0 runner    (1001) docker     (127)     4161 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/net/factories/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 07:07:29.698508 runtimepy-4.1.0/runtimepy/net/http/
--rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/net/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/net/http/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/net/http/header.py
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/net/http/request_target.py
--rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/net/http/response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/net/http/state.py
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/net/http/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     4071 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/net/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/net/mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 07:07:29.698508 runtimepy-4.1.0/runtimepy/net/server/
--rw-r--r--   0 runner    (1001) docker     (127)     5178 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/net/server/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 07:07:29.702508 runtimepy-4.1.0/runtimepy/net/server/app/
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/net/server/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/net/server/app/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 07:07:29.702508 runtimepy-4.1.0/runtimepy/net/server/app/bootstrap/
--rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/net/server/app/bootstrap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/net/server/app/bootstrap/elements.py
--rw-r--r--   0 runner    (1001) docker     (127)     3794 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/net/server/app/bootstrap/tabs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/net/server/app/create.py
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/net/server/app/elements.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 07:07:29.702508 runtimepy-4.1.0/runtimepy/net/server/app/env/
--rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/net/server/app/env/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/net/server/app/env/modal.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 07:07:29.702508 runtimepy-4.1.0/runtimepy/net/server/app/env/tab/
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/net/server/app/env/tab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/net/server/app/env/tab/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7423 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/net/server/app/env/tab/html.py
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/net/server/app/env/tab/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     3676 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/net/server/app/env/tab/message.py
--rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/net/server/app/env/widgets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/net/server/app/files.py
--rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/net/server/app/placeholder.py
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/net/server/app/pyodide.py
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/net/server/app/sound.py
--rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/net/server/app/tab.py
--rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/net/server/html.py
--rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/net/server/json.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 07:07:29.702508 runtimepy-4.1.0/runtimepy/net/server/struct/
--rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/net/server/struct/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 07:07:29.702508 runtimepy-4.1.0/runtimepy/net/server/websocket/
--rw-r--r--   0 runner    (1001) docker     (127)     4347 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/net/server/websocket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/net/server/websocket/state.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 07:07:29.702508 runtimepy-4.1.0/runtimepy/net/stream/
--rw-r--r--   0 runner    (1001) docker     (127)     2374 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/net/stream/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3234 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/net/stream/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 07:07:29.702508 runtimepy-4.1.0/runtimepy/net/stream/json/
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/net/stream/json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11453 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/net/stream/json/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3754 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/net/stream/json/handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/net/stream/json/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/net/stream/string.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 07:07:29.706508 runtimepy-4.1.0/runtimepy/net/tcp/
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/net/tcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7377 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/net/tcp/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/net/tcp/create.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 07:07:29.706508 runtimepy-4.1.0/runtimepy/net/tcp/http/
--rw-r--r--   0 runner    (1001) docker     (127)     5236 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/net/tcp/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/net/tcp/protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 07:07:29.706508 runtimepy-4.1.0/runtimepy/net/tcp/telnet/
--rw-r--r--   0 runner    (1001) docker     (127)     4768 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/net/tcp/telnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3518 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/net/tcp/telnet/codes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 07:07:29.706508 runtimepy-4.1.0/runtimepy/net/udp/
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/net/udp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7485 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/net/udp/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/net/udp/create.py
--rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/net/udp/protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/net/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 07:07:29.706508 runtimepy-4.1.0/runtimepy/net/websocket/
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/net/websocket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8068 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/net/websocket/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 07:07:29.706508 runtimepy-4.1.0/runtimepy/primitives/
--rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/primitives/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 07:07:29.706508 runtimepy-4.1.0/runtimepy/primitives/array/
--rw-r--r--   0 runner    (1001) docker     (127)     8239 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/primitives/array/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7494 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/primitives/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/primitives/bool.py
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/primitives/byte_order.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 07:07:29.710508 runtimepy-4.1.0/runtimepy/primitives/field/
--rw-r--r--   0 runner    (1001) docker     (127)     4421 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/primitives/field/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6846 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/primitives/field/fields.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 07:07:29.710508 runtimepy-4.1.0/runtimepy/primitives/field/manager/
--rw-r--r--   0 runner    (1001) docker     (127)     2586 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/primitives/field/manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6125 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/primitives/field/manager/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/primitives/float.py
--rw-r--r--   0 runner    (1001) docker     (127)     3453 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/primitives/int.py
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/primitives/scaling.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 07:07:29.710508 runtimepy-4.1.0/runtimepy/primitives/serializable/
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/primitives/serializable/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4178 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/primitives/serializable/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/primitives/serializable/fixed.py
--rw-r--r--   0 runner    (1001) docker     (127)     2736 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/primitives/serializable/prefixed.py
--rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/primitives/string.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 07:07:29.710508 runtimepy-4.1.0/runtimepy/primitives/types/
--rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/primitives/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4442 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/primitives/types/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/primitives/types/bool.py
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/primitives/types/bounds.py
--rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/primitives/types/float.py
--rw-r--r--   0 runner    (1001) docker     (127)     3631 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/primitives/types/int.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 07:07:29.710508 runtimepy-4.1.0/runtimepy/registry/
--rw-r--r--   0 runner    (1001) docker     (127)     3352 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/registry/bool.py
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/registry/item.py
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/registry/name.py
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 07:07:29.710508 runtimepy-4.1.0/runtimepy/struct/
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/struct/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 07:07:29.710508 runtimepy-4.1.0/runtimepy/task/
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/task/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5947 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/task/asynchronous.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 07:07:29.714508 runtimepy-4.1.0/runtimepy/task/basic/
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/task/basic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/task/basic/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     6388 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/task/basic/periodic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/task/sample.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 07:07:29.714508 runtimepy-4.1.0/runtimepy/task/trig/
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/task/trig/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 07:07:29.714508 runtimepy-4.1.0/runtimepy/telemetry/
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/telemetry/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 07:07:29.714508 runtimepy-4.1.0/runtimepy/tui/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/tui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 07:07:29.714508 runtimepy-4.1.0/runtimepy/tui/channels/
--rw-r--r--   0 runner    (1001) docker     (127)     4483 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/tui/channels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/tui/cursor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/tui/mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/tui/mock.py
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/tui/task.py
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-14 07:05:27.000000 runtimepy-4.1.0/runtimepy/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 07:07:29.714508 runtimepy-4.1.0/runtimepy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7055 2024-04-14 07:07:29.000000 runtimepy-4.1.0/runtimepy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7616 2024-04-14 07:07:29.000000 runtimepy-4.1.0/runtimepy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 07:07:29.000000 runtimepy-4.1.0/runtimepy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-14 07:07:29.000000 runtimepy-4.1.0/runtimepy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-14 07:07:29.000000 runtimepy-4.1.0/runtimepy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-14 07:07:29.000000 runtimepy-4.1.0/runtimepy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 07:07:29.714508 runtimepy-4.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-14 07:05:27.000000 runtimepy-4.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 07:07:29.714508 runtimepy-4.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-04-14 07:05:27.000000 runtimepy-4.1.0/tests/test_entry.py
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-14 07:05:27.000000 runtimepy-4.1.0/tests/test_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-14 07:05:27.000000 runtimepy-4.1.0/tests/test_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:04:51.773031 runtimepy-4.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-16 03:02:39.000000 runtimepy-4.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7055 2024-04-16 03:04:51.773031 runtimepy-4.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5390 2024-04-16 03:02:39.000000 runtimepy-4.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-16 03:02:39.000000 runtimepy-4.1.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:04:51.733031 runtimepy-4.1.1/runtimepy/
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:04:51.737031 runtimepy-4.1.1/runtimepy/channel/
+-rw-r--r--   0 runner    (1001) docker     (127)     3243 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/channel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:04:51.737031 runtimepy-4.1.1/runtimepy/channel/environment/
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/channel/environment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3413 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/channel/environment/array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9188 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/channel/environment/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:04:51.737031 runtimepy-4.1.1/runtimepy/channel/environment/command/
+-rw-r--r--   0 runner    (1001) docker     (127)     8145 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/channel/environment/command/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/channel/environment/command/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5669 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/channel/environment/command/processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/channel/environment/command/result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5562 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/channel/environment/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6949 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/channel/environment/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/channel/environment/sample.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:04:51.737031 runtimepy-4.1.1/runtimepy/channel/event/
+-rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/channel/event/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/channel/event/header.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5774 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/channel/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:04:51.737031 runtimepy-4.1.1/runtimepy/codec/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/codec/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:04:51.737031 runtimepy-4.1.1/runtimepy/codec/protocol/
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/codec/protocol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/codec/protocol/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4107 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/codec/protocol/json.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:04:51.737031 runtimepy-4.1.1/runtimepy/codec/system/
+-rw-r--r--   0 runner    (1001) docker     (127)     6939 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/codec/system/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:04:51.741031 runtimepy-4.1.1/runtimepy/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/commands/all.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/commands/arbiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/commands/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3767 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/commands/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/commands/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/commands/tui.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:04:51.741031 runtimepy-4.1.1/runtimepy/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:04:51.741031 runtimepy-4.1.1/runtimepy/data/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/data/css/bootstrap_extra.css
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/data/css/main.css
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/data/dummy_load.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/data/factories.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)   362870 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/data/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:04:51.741031 runtimepy-4.1.1/runtimepy/data/js/
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/data/js/DataConnection.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/data/js/JsonConnection.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/data/js/audio.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:04:51.745031 runtimepy-4.1.1/runtimepy/data/js/classes/
+-rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/data/js/classes/App.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/data/js/classes/ChannelTable.js
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/data/js/classes/DataConnection.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2858 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/data/js/classes/JsonConnection.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/data/js/classes/Plot.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/data/js/classes/PlotManager.js
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/data/js/classes/PlotModalManager.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/data/js/classes/TabFilter.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7568 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/data/js/classes/TabInterface.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3467 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/data/js/classes/WindowHashManager.js
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/data/js/classes/WorkerInterface.js
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/data/js/init.js
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/data/js/main.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:04:51.745031 runtimepy-4.1.1/runtimepy/data/js/tab/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/data/js/tab/env.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/data/js/tab/sound.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:04:51.745031 runtimepy-4.1.1/runtimepy/data/js/unused/
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/data/js/unused/pyodide.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/data/js/util.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/data/js/worker.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:04:51.749031 runtimepy-4.1.1/runtimepy/data/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/data/schemas/BitFields.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/data/schemas/Channel.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/data/schemas/ChannelCommand.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/data/schemas/ChannelRegistry.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/data/schemas/ClientConnectionConfig.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/data/schemas/ConnectionArbiterConfig.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/data/schemas/EnumRegistry.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/data/schemas/FindFile.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/data/schemas/RuntimeEnum.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/data/schemas/ServerConnectionConfig.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/data/schemas/StructConfig.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/data/schemas/TaskConfig.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/data/schemas/has_factory.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/data/schemas/has_name.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/data/schemas/has_request_flag.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/data/server.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/data/server_base.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/data/server_dev.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/dev_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/entry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:04:51.749031 runtimepy-4.1.1/runtimepy/enum/
+-rw-r--r--   0 runner    (1001) docker     (127)     5819 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/enum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/enum/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/enum/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5390 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/mapping.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:04:51.749031 runtimepy-4.1.1/runtimepy/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/metrics/channel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/metrics/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/metrics/task.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:04:51.749031 runtimepy-4.1.1/runtimepy/mixins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/mixins/async_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/mixins/enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/mixins/environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/mixins/finalize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/mixins/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/mixins/regex.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:04:51.753031 runtimepy-4.1.1/runtimepy/net/
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:04:51.753031 runtimepy-4.1.1/runtimepy/net/apps/
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:04:51.753031 runtimepy-4.1.1/runtimepy/net/arbiter/
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/arbiter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13605 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/arbiter/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:04:51.753031 runtimepy-4.1.1/runtimepy/net/arbiter/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     7632 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/arbiter/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2607 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/arbiter/config/codec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/arbiter/config/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:04:51.753031 runtimepy-4.1.1/runtimepy/net/arbiter/factory/
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/arbiter/factory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3690 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/arbiter/factory/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/arbiter/factory/task.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:04:51.753031 runtimepy-4.1.1/runtimepy/net/arbiter/housekeeping/
+-rw-r--r--   0 runner    (1001) docker     (127)     2318 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/arbiter/housekeeping/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:04:51.753031 runtimepy-4.1.1/runtimepy/net/arbiter/imports/
+-rw-r--r--   0 runner    (1001) docker     (127)     3430 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/arbiter/imports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/arbiter/imports/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6382 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/arbiter/info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/arbiter/result.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:04:51.753031 runtimepy-4.1.1/runtimepy/net/arbiter/struct/
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/arbiter/struct/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/arbiter/task.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:04:51.753031 runtimepy-4.1.1/runtimepy/net/arbiter/tcp/
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/arbiter/tcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/arbiter/tcp/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/arbiter/udp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/arbiter/websocket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/backoff.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11894 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:04:51.753031 runtimepy-4.1.1/runtimepy/net/factories/
+-rw-r--r--   0 runner    (1001) docker     (127)     4161 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/factories/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:04:51.757031 runtimepy-4.1.1/runtimepy/net/http/
+-rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/http/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/http/header.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/http/request_target.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/http/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/http/state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/http/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4071 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:04:51.757031 runtimepy-4.1.1/runtimepy/net/server/
+-rw-r--r--   0 runner    (1001) docker     (127)     5178 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/server/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:04:51.757031 runtimepy-4.1.1/runtimepy/net/server/app/
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/server/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/server/app/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:04:51.757031 runtimepy-4.1.1/runtimepy/net/server/app/bootstrap/
+-rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/server/app/bootstrap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/server/app/bootstrap/elements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3779 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/server/app/bootstrap/tabs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/server/app/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/server/app/elements.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:04:51.757031 runtimepy-4.1.1/runtimepy/net/server/app/env/
+-rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/server/app/env/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/server/app/env/modal.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:04:51.761031 runtimepy-4.1.1/runtimepy/net/server/app/env/tab/
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/server/app/env/tab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/server/app/env/tab/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7408 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/server/app/env/tab/html.py
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/server/app/env/tab/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3676 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/server/app/env/tab/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3285 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/server/app/env/widgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/server/app/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/server/app/placeholder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/server/app/pyodide.py
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/server/app/sound.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/server/app/tab.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/server/html.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/server/json.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:04:51.761031 runtimepy-4.1.1/runtimepy/net/server/struct/
+-rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/server/struct/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:04:51.761031 runtimepy-4.1.1/runtimepy/net/server/websocket/
+-rw-r--r--   0 runner    (1001) docker     (127)     4347 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/server/websocket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/server/websocket/state.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:04:51.761031 runtimepy-4.1.1/runtimepy/net/stream/
+-rw-r--r--   0 runner    (1001) docker     (127)     2374 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/stream/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3234 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/stream/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:04:51.761031 runtimepy-4.1.1/runtimepy/net/stream/json/
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/stream/json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11453 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/stream/json/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3754 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/stream/json/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/stream/json/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/stream/string.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:04:51.761031 runtimepy-4.1.1/runtimepy/net/tcp/
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/tcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7377 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/tcp/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/tcp/create.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:04:51.761031 runtimepy-4.1.1/runtimepy/net/tcp/http/
+-rw-r--r--   0 runner    (1001) docker     (127)     5236 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/tcp/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/tcp/protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:04:51.761031 runtimepy-4.1.1/runtimepy/net/tcp/telnet/
+-rw-r--r--   0 runner    (1001) docker     (127)     4768 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/tcp/telnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3518 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/tcp/telnet/codes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:04:51.765031 runtimepy-4.1.1/runtimepy/net/udp/
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/udp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7485 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/udp/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/udp/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/udp/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:04:51.765031 runtimepy-4.1.1/runtimepy/net/websocket/
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/websocket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8068 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/net/websocket/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:04:51.765031 runtimepy-4.1.1/runtimepy/primitives/
+-rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/primitives/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:04:51.765031 runtimepy-4.1.1/runtimepy/primitives/array/
+-rw-r--r--   0 runner    (1001) docker     (127)     8239 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/primitives/array/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7494 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/primitives/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/primitives/bool.py
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/primitives/byte_order.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:04:51.765031 runtimepy-4.1.1/runtimepy/primitives/field/
+-rw-r--r--   0 runner    (1001) docker     (127)     4421 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/primitives/field/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6846 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/primitives/field/fields.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:04:51.765031 runtimepy-4.1.1/runtimepy/primitives/field/manager/
+-rw-r--r--   0 runner    (1001) docker     (127)     2586 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/primitives/field/manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6125 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/primitives/field/manager/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/primitives/float.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3453 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/primitives/int.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/primitives/scaling.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:04:51.765031 runtimepy-4.1.1/runtimepy/primitives/serializable/
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/primitives/serializable/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4178 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/primitives/serializable/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/primitives/serializable/fixed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2736 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/primitives/serializable/prefixed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/primitives/string.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:04:51.769031 runtimepy-4.1.1/runtimepy/primitives/types/
+-rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/primitives/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4442 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/primitives/types/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/primitives/types/bool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/primitives/types/bounds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/primitives/types/float.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3631 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/primitives/types/int.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:04:51.769031 runtimepy-4.1.1/runtimepy/registry/
+-rw-r--r--   0 runner    (1001) docker     (127)     3352 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/registry/bool.py
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/registry/item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/registry/name.py
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:04:51.769031 runtimepy-4.1.1/runtimepy/struct/
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/struct/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:04:51.769031 runtimepy-4.1.1/runtimepy/task/
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/task/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5947 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/task/asynchronous.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:04:51.769031 runtimepy-4.1.1/runtimepy/task/basic/
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/task/basic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/task/basic/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6388 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/task/basic/periodic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/task/sample.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:04:51.769031 runtimepy-4.1.1/runtimepy/task/trig/
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/task/trig/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:04:51.769031 runtimepy-4.1.1/runtimepy/telemetry/
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/telemetry/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:04:51.769031 runtimepy-4.1.1/runtimepy/tui/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/tui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:04:51.769031 runtimepy-4.1.1/runtimepy/tui/channels/
+-rw-r--r--   0 runner    (1001) docker     (127)     4483 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/tui/channels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/tui/cursor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/tui/mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/tui/mock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/tui/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-16 03:02:39.000000 runtimepy-4.1.1/runtimepy/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:04:51.769031 runtimepy-4.1.1/runtimepy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7055 2024-04-16 03:04:51.000000 runtimepy-4.1.1/runtimepy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7662 2024-04-16 03:04:51.000000 runtimepy-4.1.1/runtimepy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 03:04:51.000000 runtimepy-4.1.1/runtimepy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-16 03:04:51.000000 runtimepy-4.1.1/runtimepy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-16 03:04:51.000000 runtimepy-4.1.1/runtimepy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-16 03:04:51.000000 runtimepy-4.1.1/runtimepy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 03:04:51.773031 runtimepy-4.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-16 03:02:39.000000 runtimepy-4.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:04:51.769031 runtimepy-4.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-04-16 03:02:39.000000 runtimepy-4.1.1/tests/test_entry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-16 03:02:39.000000 runtimepy-4.1.1/tests/test_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-16 03:02:39.000000 runtimepy-4.1.1/tests/test_resources.py
```

### Comparing `runtimepy-4.1.0/LICENSE` & `runtimepy-4.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/PKG-INFO` & `runtimepy-4.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: runtimepy
-Version: 4.1.0
+Version: 4.1.1
 Summary: A framework for implementing Python services.
 Home-page: https://github.com/vkottler/runtimepy
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
@@ -13,18 +13,18 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Unix
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: svgen>=0.6.5
-Requires-Dist: websockets
-Requires-Dist: psutil
 Requires-Dist: vcorelib>=3.2.3
+Requires-Dist: svgen>=0.6.6
+Requires-Dist: psutil
+Requires-Dist: websockets
 Provides-Extra: test
 Requires-Dist: pylint; extra == "test"
 Requires-Dist: flake8; extra == "test"
 Requires-Dist: black; extra == "test"
 Requires-Dist: ruff; extra == "test"
 Requires-Dist: mypy; extra == "test"
 Requires-Dist: isort; extra == "test"
@@ -40,19 +40,19 @@
 Requires-Dist: types-setuptools; extra == "test"
 Requires-Dist: uvloop; (sys_platform != "win32" and sys_platform != "cygwin") and extra == "test"
 
 <!--
     =====================================
     generator=datazen
     version=3.1.4
-    hash=739a1dad9e7a1670fab3bb537c6ea3e9
+    hash=36872ce673f57f77e5b632b95169543d
     =====================================
 -->
 
-# runtimepy ([4.1.0](https://pypi.org/project/runtimepy/))
+# runtimepy ([4.1.1](https://pypi.org/project/runtimepy/))
 
 [![python](https://img.shields.io/pypi/pyversions/runtimepy.svg)](https://pypi.org/project/runtimepy/)
 ![Build Status](https://github.com/vkottler/runtimepy/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/runtimepy/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/runtimepy)
 ![PyPI - Status](https://img.shields.io/pypi/status/runtimepy)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/runtimepy)
```

### Comparing `runtimepy-4.1.0/README.md` & `runtimepy-4.1.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 <!--
     =====================================
     generator=datazen
     version=3.1.4
-    hash=739a1dad9e7a1670fab3bb537c6ea3e9
+    hash=36872ce673f57f77e5b632b95169543d
     =====================================
 -->
 
-# runtimepy ([4.1.0](https://pypi.org/project/runtimepy/))
+# runtimepy ([4.1.1](https://pypi.org/project/runtimepy/))
 
 [![python](https://img.shields.io/pypi/pyversions/runtimepy.svg)](https://pypi.org/project/runtimepy/)
 ![Build Status](https://github.com/vkottler/runtimepy/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/runtimepy/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/runtimepy)
 ![PyPI - Status](https://img.shields.io/pypi/status/runtimepy)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/runtimepy)
```

### Comparing `runtimepy-4.1.0/pyproject.toml` & `runtimepy-4.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools-wrapper", "trove-classifiers"]
 build-backend = "setuptools.build_meta:__legacy__"
 
 [project]
 name = "runtimepy"
-version = "4.1.0"
+version = "4.1.1"
 description = "A framework for implementing Python services."
 readme = "README.md"
 requires-python = ">=3.11"
 authors = [
   {name = "Vaughn Kottler", email = "vaughnkottler@gmail.com"}
 ]
 maintainers = [
```

### Comparing `runtimepy-4.1.0/runtimepy/app.py` & `runtimepy-4.1.1/runtimepy/app.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/channel/__init__.py` & `runtimepy-4.1.1/runtimepy/channel/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/channel/environment/__init__.py` & `runtimepy-4.1.1/runtimepy/channel/environment/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/channel/environment/array.py` & `runtimepy-4.1.1/runtimepy/channel/environment/array.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/channel/environment/base.py` & `runtimepy-4.1.1/runtimepy/channel/environment/base.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/channel/environment/command/__init__.py` & `runtimepy-4.1.1/runtimepy/channel/environment/command/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/channel/environment/command/parser.py` & `runtimepy-4.1.1/runtimepy/channel/environment/command/parser.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/channel/environment/command/processor.py` & `runtimepy-4.1.1/runtimepy/channel/environment/command/processor.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/channel/environment/command/result.py` & `runtimepy-4.1.1/runtimepy/channel/environment/command/result.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/channel/environment/create.py` & `runtimepy-4.1.1/runtimepy/channel/environment/create.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/channel/environment/file.py` & `runtimepy-4.1.1/runtimepy/channel/environment/file.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/channel/environment/sample.py` & `runtimepy-4.1.1/runtimepy/channel/environment/sample.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/channel/event/__init__.py` & `runtimepy-4.1.1/runtimepy/channel/event/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/channel/event/header.py` & `runtimepy-4.1.1/runtimepy/channel/event/header.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/channel/registry.py` & `runtimepy-4.1.1/runtimepy/channel/registry.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/codec/protocol/__init__.py` & `runtimepy-4.1.1/runtimepy/codec/protocol/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/codec/protocol/base.py` & `runtimepy-4.1.1/runtimepy/codec/protocol/base.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/codec/protocol/json.py` & `runtimepy-4.1.1/runtimepy/codec/protocol/json.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/codec/system/__init__.py` & `runtimepy-4.1.1/runtimepy/codec/system/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/commands/all.py` & `runtimepy-4.1.1/runtimepy/commands/all.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/commands/arbiter.py` & `runtimepy-4.1.1/runtimepy/commands/arbiter.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/commands/common.py` & `runtimepy-4.1.1/runtimepy/commands/common.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/commands/server.py` & `runtimepy-4.1.1/runtimepy/commands/server.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/commands/task.py` & `runtimepy-4.1.1/runtimepy/commands/task.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/commands/tui.py` & `runtimepy-4.1.1/runtimepy/commands/tui.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/data/css/bootstrap_extra.css` & `runtimepy-4.1.1/runtimepy/data/css/bootstrap_extra.css`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/data/dummy_load.yaml` & `runtimepy-4.1.1/runtimepy/data/dummy_load.yaml`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/data/factories.yaml` & `runtimepy-4.1.1/runtimepy/data/factories.yaml`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/data/favicon.ico` & `runtimepy-4.1.1/runtimepy/data/favicon.ico`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/data/js/JsonConnection.js` & `runtimepy-4.1.1/runtimepy/data/js/JsonConnection.js`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/data/js/audio.js` & `runtimepy-4.1.1/runtimepy/data/js/audio.js`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/data/js/classes/App.js` & `runtimepy-4.1.1/runtimepy/data/js/classes/App.js`

 * *Files 7% similar despite different names*

#### js-beautify {}

```diff
@@ -15,14 +15,20 @@
     async main() {
         /*
          * Run application initialization when the worker thread responds with an
          * expected value.
          */
         worker.addEventListener("message", async (event) => {
             if (event.data == 0) {
+                /* Manage settings modal. */
+                let _modal = document.getElementById("runtimepy-plot");
+                if (_modal) {
+                    modalManager = new PlotModalManager(_modal);
+                }
+
                 /* Run tab initialization. */
                 for await (const init of inits) {
                     await init();
                 }
 
                 hash.initButtons();
 
@@ -42,47 +48,51 @@
                     for (const key in event.data) {
                         /* Handle forwarding messages to individual tabs. */
                         if (key in tabs) {
                             tabs[key].onmessage(event.data[key]);
                         }
                     }
                 };
+
+                startMainLoop();
             }
         }, {
             once: true
         });
 
         /* Start worker. */
         this.worker.postMessage(this.config);
 
         bootstrap_init();
+    }
+}
 
-        let splash = document.getElementById("runtimepy-splash");
+function startMainLoop() {
+    let splash = document.getElementById("runtimepy-splash");
 
-        let prevTime = 0;
+    let prevTime = 0;
 
-        /* Main loop. */
-        function render(time) {
-            let deltaT = time - prevTime;
-
-            /* Fade splash screen out if necessary. */
-            if (splash) {
-                let curr = window.getComputedStyle(splash).getPropertyValue("opacity");
-                if (curr > 0) {
-                    splash.style.opacity = curr - (deltaT / 2500);
-                } else {
-                    splash.style.display = "none";
-                    splash = undefined;
-                }
-            }
-
-            /* Poll the currently shown tab. */
-            if (shown_tab in tabs) {
-                tabs[shown_tab].poll(time);
+    /* Main loop. */
+    function render(time) {
+        let deltaT = time - prevTime;
+
+        /* Fade splash screen out if necessary. */
+        if (splash) {
+            let curr = window.getComputedStyle(splash).getPropertyValue("opacity");
+            if (curr > 0) {
+                splash.style.opacity = curr - Math.min(0.05, deltaT / 2000);
+            } else {
+                splash.style.display = "none";
+                splash = undefined;
             }
+        }
 
-            prevTime = time;
-            requestAnimationFrame(render);
+        /* Poll the currently shown tab. */
+        if (shown_tab in tabs) {
+            tabs[shown_tab].poll(time);
         }
+
+        prevTime = time;
         requestAnimationFrame(render);
     }
+    requestAnimationFrame(render);
 }
```

### Comparing `runtimepy-4.1.0/runtimepy/data/js/classes/ChannelTable.js` & `runtimepy-4.1.1/runtimepy/data/js/classes/ChannelTable.js`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/data/js/classes/JsonConnection.js` & `runtimepy-4.1.1/runtimepy/data/js/classes/JsonConnection.js`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/data/js/classes/Plot.js` & `runtimepy-4.1.1/runtimepy/data/js/classes/Plot.js`

 * *Files 11% similar despite different names*

#### js-beautify {}

```diff
@@ -10,14 +10,22 @@
         this.plotMessage(msg, [offscreen]);
 
         /* Use resize observer to handle resize events. */
         this.resizeObserver = new ResizeObserver(
             ((entries, observer) => {
                 this.handle_resize();
             }).bind(this));
+
+        /* Handle click events. */
+        let plotButton = document.getElementById("runtimepy-plot-button");
+        if (plotButton) {
+            this.canvas.onclick = (event) => {
+                plotButton.click();
+            };
+        }
     }
 
     plotMessage(data, param) {
         this.worker.toWorker({
             "plot": data
         }, param);
     }
```

### Comparing `runtimepy-4.1.0/runtimepy/data/js/classes/PlotManager.js` & `runtimepy-4.1.1/runtimepy/data/js/classes/PlotManager.js`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/data/js/classes/TabFilter.js` & `runtimepy-4.1.1/runtimepy/data/js/classes/TabFilter.js`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/data/js/classes/TabInterface.js` & `runtimepy-4.1.1/runtimepy/data/js/classes/TabInterface.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -173,14 +173,15 @@
             for (let elem of this.queryAll("input.form-check-input")) {
                 elem.addEventListener(
                     "change",
                     ((event) => {
                         let chan = elem.id.split("-")[1];
                         let state = elem.checked;
                         hash.handlePlotChannelToggle(this.name, chan, state);
+
                         this.worker.send({
                             kind: "plot",
                             value: {
                                 "channel": chan,
                                 "state": state
                             }
                         });
```

### Comparing `runtimepy-4.1.0/runtimepy/data/js/classes/WindowHashManager.js` & `runtimepy-4.1.1/runtimepy/data/js/classes/WindowHashManager.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -26,14 +26,19 @@
             elem.style.display = dividerDisplay;
         }
 
         this.update();
     }
 
     handlePlotChannelToggle(tabName, channel, state) {
+        /* Service settings modal. */
+        if (modalManager) {
+            modalManager.handleChannelToggle(tabName, channel, state);
+        }
+
         if (!(tabName in this.plotChannels)) {
             this.plotChannels[tabName] = {};
         }
         let channelStates = this.plotChannels[tabName];
         channelStates[channel] = state;
 
         this.update();
```

### Comparing `runtimepy-4.1.0/runtimepy/data/js/tab/sound.js` & `runtimepy-4.1.1/runtimepy/data/js/tab/sound.js`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/data/js/unused/pyodide.js` & `runtimepy-4.1.1/runtimepy/data/js/unused/pyodide.js`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/data/js/util.js` & `runtimepy-4.1.1/runtimepy/data/js/util.js`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/data/js/worker.js` & `runtimepy-4.1.1/runtimepy/data/js/worker.js`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/data/schemas/BitFields.yaml` & `runtimepy-4.1.1/runtimepy/data/schemas/BitFields.yaml`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/data/schemas/ConnectionArbiterConfig.yaml` & `runtimepy-4.1.1/runtimepy/data/schemas/ConnectionArbiterConfig.yaml`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/data/schemas/FindFile.yaml` & `runtimepy-4.1.1/runtimepy/data/schemas/FindFile.yaml`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/data/server_base.yaml` & `runtimepy-4.1.1/runtimepy/data/server_base.yaml`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/entry.py` & `runtimepy-4.1.1/runtimepy/entry.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/enum/__init__.py` & `runtimepy-4.1.1/runtimepy/enum/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/enum/registry.py` & `runtimepy-4.1.1/runtimepy/enum/registry.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/enum/types.py` & `runtimepy-4.1.1/runtimepy/enum/types.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/mapping.py` & `runtimepy-4.1.1/runtimepy/mapping.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/metrics/channel.py` & `runtimepy-4.1.1/runtimepy/metrics/channel.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/metrics/connection.py` & `runtimepy-4.1.1/runtimepy/metrics/connection.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/metrics/task.py` & `runtimepy-4.1.1/runtimepy/metrics/task.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/mixins/async_command.py` & `runtimepy-4.1.1/runtimepy/mixins/async_command.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/mixins/enum.py` & `runtimepy-4.1.1/runtimepy/mixins/enum.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/mixins/environment.py` & `runtimepy-4.1.1/runtimepy/mixins/environment.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/mixins/finalize.py` & `runtimepy-4.1.1/runtimepy/mixins/finalize.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/mixins/logging.py` & `runtimepy-4.1.1/runtimepy/mixins/logging.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/mixins/regex.py` & `runtimepy-4.1.1/runtimepy/mixins/regex.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/net/__init__.py` & `runtimepy-4.1.1/runtimepy/net/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/net/apps/__init__.py` & `runtimepy-4.1.1/runtimepy/net/apps/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/net/arbiter/__init__.py` & `runtimepy-4.1.1/runtimepy/net/arbiter/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/net/arbiter/base.py` & `runtimepy-4.1.1/runtimepy/net/arbiter/base.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/net/arbiter/config/__init__.py` & `runtimepy-4.1.1/runtimepy/net/arbiter/config/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/net/arbiter/config/codec.py` & `runtimepy-4.1.1/runtimepy/net/arbiter/config/codec.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/net/arbiter/config/util.py` & `runtimepy-4.1.1/runtimepy/net/arbiter/config/util.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/net/arbiter/factory/connection.py` & `runtimepy-4.1.1/runtimepy/net/arbiter/factory/connection.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/net/arbiter/factory/task.py` & `runtimepy-4.1.1/runtimepy/net/arbiter/factory/task.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/net/arbiter/housekeeping/__init__.py` & `runtimepy-4.1.1/runtimepy/net/arbiter/housekeeping/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/net/arbiter/imports/__init__.py` & `runtimepy-4.1.1/runtimepy/net/arbiter/imports/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/net/arbiter/imports/util.py` & `runtimepy-4.1.1/runtimepy/net/arbiter/imports/util.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/net/arbiter/info.py` & `runtimepy-4.1.1/runtimepy/net/arbiter/info.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/net/arbiter/result.py` & `runtimepy-4.1.1/runtimepy/net/arbiter/result.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/net/arbiter/struct/__init__.py` & `runtimepy-4.1.1/runtimepy/net/arbiter/struct/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/net/arbiter/task.py` & `runtimepy-4.1.1/runtimepy/net/arbiter/task.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/net/arbiter/tcp/__init__.py` & `runtimepy-4.1.1/runtimepy/net/arbiter/tcp/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/net/arbiter/tcp/json.py` & `runtimepy-4.1.1/runtimepy/net/arbiter/tcp/json.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/net/arbiter/udp.py` & `runtimepy-4.1.1/runtimepy/net/arbiter/udp.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/net/arbiter/websocket.py` & `runtimepy-4.1.1/runtimepy/net/arbiter/websocket.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/net/backoff.py` & `runtimepy-4.1.1/runtimepy/net/backoff.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/net/connection.py` & `runtimepy-4.1.1/runtimepy/net/connection.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/net/factories/__init__.py` & `runtimepy-4.1.1/runtimepy/net/factories/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/net/http/__init__.py` & `runtimepy-4.1.1/runtimepy/net/http/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/net/http/common.py` & `runtimepy-4.1.1/runtimepy/net/http/common.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/net/http/header.py` & `runtimepy-4.1.1/runtimepy/net/http/header.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/net/http/request_target.py` & `runtimepy-4.1.1/runtimepy/net/http/request_target.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/net/http/response.py` & `runtimepy-4.1.1/runtimepy/net/http/response.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/net/http/state.py` & `runtimepy-4.1.1/runtimepy/net/http/state.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/net/http/version.py` & `runtimepy-4.1.1/runtimepy/net/http/version.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/net/manager.py` & `runtimepy-4.1.1/runtimepy/net/manager.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/net/mixin.py` & `runtimepy-4.1.1/runtimepy/net/mixin.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/net/server/__init__.py` & `runtimepy-4.1.1/runtimepy/net/server/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/net/server/app/__init__.py` & `runtimepy-4.1.1/runtimepy/net/server/app/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/net/server/app/base.py` & `runtimepy-4.1.1/runtimepy/net/server/app/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 class WebApplication:
     """A simple web-application interface."""
 
     worker_classes = ["JsonConnection", "DataConnection", "PlotManager"]
     ui_classes = [
         "WindowHashManager",
         "WorkerInterface",
+        "PlotModalManager",
         "Plot",
         "ChannelTable",
         "TabInterface",
         "TabFilter",
         "App",
     ]
```

### Comparing `runtimepy-4.1.0/runtimepy/net/server/app/bootstrap/__init__.py` & `runtimepy-4.1.1/runtimepy/net/server/app/bootstrap/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 """
 A module implementing interfaces to include Bootstrap
 (https://getbootstrap.com/) in an application.
 """
 
 # third-party
 from svgen.element import Element
-
-# internal
-from runtimepy.net.server.app.elements import div
+from svgen.element.html import div
 
 CDN = "cdn.jsdelivr.net"
 BOOTSTRAP_VERSION = "5.3.3"
 ICONS_VERSION = "1.11.3"
 
 
 def icon_str(icon: str) -> str:
```

### Comparing `runtimepy-4.1.0/runtimepy/net/server/app/bootstrap/elements.py` & `runtimepy-4.1.1/runtimepy/net/server/app/bootstrap/elements.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """
 A module for creating various bootstrap-related elements.
 """
 
 # third-party
 from svgen.element import Element
+from svgen.element.html import div
 
 # internal
 from runtimepy.net.server.app.bootstrap import icon_str
-from runtimepy.net.server.app.elements import div
 
 TEXT = "font-monospace"
 BOOTSTRAP_BUTTON = f"rounded-0 {TEXT} button-bodge"
 
 
 def flex(kind: str = "row", **kwargs) -> Element:
     """Get a flexbox row container."""
```

### Comparing `runtimepy-4.1.0/runtimepy/net/server/app/bootstrap/tabs.py` & `runtimepy-4.1.1/runtimepy/net/server/app/bootstrap/tabs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """
 A module implementing interfaces for creating tabbed content with bootstrap.
 """
 
 # third-party
 from svgen.element import Element
+from svgen.element.html import div
 
 # internal
 from runtimepy import PKG_NAME
 from runtimepy.net.server.app.bootstrap.elements import (
     BOOTSTRAP_BUTTON,
     collapse_button,
 )
-from runtimepy.net.server.app.elements import div
 
 
 def create_nav_button(
     parent: Element,
     name: str,
     item: str,
     active_tab: bool,
```

### Comparing `runtimepy-4.1.0/runtimepy/net/server/app/create.py` & `runtimepy-4.1.1/runtimepy/net/server/app/create.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/net/server/app/env/__init__.py` & `runtimepy-4.1.1/runtimepy/net/server/app/env/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 """
 A module implementing a channel-environment tab HTML interface.
 """
 
+# third-party
+from svgen.element.html import div
+
 # internal
 from runtimepy import PKG_NAME
 from runtimepy.net.arbiter.info import AppInfo
 from runtimepy.net.server.app.bootstrap.elements import input_box
 from runtimepy.net.server.app.bootstrap.tabs import TabbedContent
-from runtimepy.net.server.app.elements import div
 from runtimepy.net.server.app.env.modal import Modal
 from runtimepy.net.server.app.env.tab import ChannelEnvironmentTab
 from runtimepy.net.server.app.placeholder import dummy_tabs, under_construction
 from runtimepy.net.server.app.sound import SoundTab
 
 
 def channel_environments(app: AppInfo, tabs: TabbedContent) -> None:
@@ -45,14 +47,18 @@
     tabs.add_button(
         "Toggle channel table",
         ".channel-column",
         icon="table",
         id="channels-button",
     )
 
+    # Plot settings modal.
+    plot_settings = Modal(tabs, name="plot", icon="graph-up")
+    under_construction(plot_settings.footer)
+
     # Experimental features.
     if app.config_param("experimental", False):
         # Sound tab.
         SoundTab("sound", app, tabs, source="sound", icon="boombox").entry()
 
         dummy_tabs(3, app, tabs)
```

### Comparing `runtimepy-4.1.0/runtimepy/net/server/app/env/modal.py` & `runtimepy-4.1.1/runtimepy/net/server/app/env/modal.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 """
 A module implementing a simple modal interface.
 """
 
+# third-party
+from svgen.element.html import div
+
 # internal
 from runtimepy import PKG_NAME
 from runtimepy.net.server.app.bootstrap.elements import TEXT
 from runtimepy.net.server.app.bootstrap.tabs import TabbedContent
-from runtimepy.net.server.app.elements import div
 
 
 class Modal:
     """A class implementing a simple bootstrap-modal interface."""
 
     def __init__(
         self,
@@ -44,16 +46,18 @@
             type="button",
             parent=self.header,
             class_str="btn-close",
         )
         button["data-bs-dismiss"] = "modal"
         button["aria-label"] = "close"
 
-        self.body = div(text="Body.", parent=content, class_str="modal-body")
-        self.footer = div(
-            text="Footer.", parent=content, class_str="modal-footer"
-        )
+        self.body = div(parent=content, class_str="modal-body")
+        self.footer = div(parent=content, class_str="modal-footer")
 
         # Add toggle button.
         tabs.add_button(
-            f"Toggle {name}", "#" + modal_id, icon=icon, toggle="modal"
+            f"Toggle {name}",
+            "#" + modal_id,
+            icon=icon,
+            toggle="modal",
+            id=f"{modal_id}-button",
         )
```

### Comparing `runtimepy-4.1.0/runtimepy/net/server/app/env/tab/__init__.py` & `runtimepy-4.1.1/runtimepy/net/server/app/env/tab/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/net/server/app/env/tab/base.py` & `runtimepy-4.1.1/runtimepy/net/server/app/env/tab/base.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/net/server/app/env/tab/html.py` & `runtimepy-4.1.1/runtimepy/net/server/app/env/tab/html.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,26 +3,26 @@
 """
 
 # built-in
 from typing import Optional, cast
 
 # third-party
 from svgen.element import Element
+from svgen.element.html import div
 
 # internal
 from runtimepy.channel import AnyChannel
 from runtimepy.enum import RuntimeEnum
 from runtimepy.net.server.app.bootstrap.elements import (
     TEXT,
     flex,
     input_box,
     set_tooltip,
     toggle_button,
 )
-from runtimepy.net.server.app.elements import div
 from runtimepy.net.server.app.env.tab.base import ChannelEnvironmentTabBase
 from runtimepy.net.server.app.env.widgets import (
     channel_table_header,
     enum_dropdown,
     plot_checkbox,
     value_input_box,
 )
```

### Comparing `runtimepy-4.1.0/runtimepy/net/server/app/env/tab/message.py` & `runtimepy-4.1.1/runtimepy/net/server/app/env/tab/message.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/net/server/app/env/widgets.py` & `runtimepy-4.1.1/runtimepy/net/server/app/env/widgets.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 """
 
 # built-in
 from typing import cast
 
 # third-party
 from svgen.element import Element
+from svgen.element.html import div
 
 # internal
 from runtimepy.enum import RuntimeEnum
 from runtimepy.net.server.app.bootstrap.elements import (
     flex,
     input_box,
     set_tooltip,
     toggle_button,
 )
-from runtimepy.net.server.app.elements import div
 
 
 def plot_checkbox(parent: Element, name: str) -> None:
     """Add a checkbox for individual channel plot status."""
 
     container = div(tag="td", parent=parent)
```

### Comparing `runtimepy-4.1.0/runtimepy/net/server/app/files.py` & `runtimepy-4.1.1/runtimepy/net/server/app/files.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/net/server/app/placeholder.py` & `runtimepy-4.1.1/runtimepy/net/server/app/placeholder.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """
 A module implementing some placeholder widget utilities.
 """
 
 # third-party
 from svgen.element import Element
+from svgen.element.html import div
 
 # internal
 from runtimepy.net.arbiter.info import AppInfo
 from runtimepy.net.server.app.bootstrap import icon_str
 from runtimepy.net.server.app.bootstrap.tabs import TabbedContent
-from runtimepy.net.server.app.elements import div
 from runtimepy.net.server.app.tab import Tab
 
 
 class DummyTab(Tab):
     """A dummy tab for testing."""
 
     def compose(self, parent: Element) -> None:
```

### Comparing `runtimepy-4.1.0/runtimepy/net/server/app/sound.py` & `runtimepy-4.1.1/runtimepy/net/server/app/sound.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 """
 A module implementing a tab for experimenting with sound generation.
 """
 
 # third-party
 from svgen.element import Element
-
-from runtimepy.net.server.app.bootstrap.elements import bootstrap_button
+from svgen.element.html import div
 
 # built-in
-from runtimepy.net.server.app.elements import div
+from runtimepy.net.server.app.bootstrap.elements import bootstrap_button
 from runtimepy.net.server.app.tab import Tab
 
 
 class SoundTab(Tab):
     """A simple sound-tab interface class."""
 
     def compose(self, parent: Element) -> None:
```

### Comparing `runtimepy-4.1.0/runtimepy/net/server/app/tab.py` & `runtimepy-4.1.1/runtimepy/net/server/app/tab.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 
 # built-in
 from io import StringIO
 from typing import cast
 
 # third-party
 from svgen.element import Element
+from svgen.element.html import div
 from vcorelib.io.file_writer import IndentedFileWriter
 
 # internal
 from runtimepy.net.arbiter.info import AppInfo
 from runtimepy.net.server.app.bootstrap import icon_str
 from runtimepy.net.server.app.bootstrap.tabs import TabbedContent
-from runtimepy.net.server.app.elements import div
 from runtimepy.net.server.app.files import kind_url, write_found_file
 
 
 class Tab:
     """A simple application-tab interface class."""
 
     def __init__(
```

### Comparing `runtimepy-4.1.0/runtimepy/net/server/html.py` & `runtimepy-4.1.1/runtimepy/net/server/html.py`

 * *Files 12% similar despite different names*

```diff
@@ -32,12 +32,12 @@
 
     # Set response headers.
     response["Content-Type"] = f"text/html; charset={DEFAULT_ENCODING}"
 
     # Create the application.
     app = apps.get(request.target.path, default_app)
     if app is not None:
-        document = await app(
-            Html(HttpConnection.identity), request, response, request_data
-        )
-        stream.write("<!DOCTYPE html>\n")
-        document.encode(stream)
+        (
+            await app(
+                Html(HttpConnection.identity), request, response, request_data
+            )
+        ).render(stream)
```

### Comparing `runtimepy-4.1.0/runtimepy/net/server/json.py` & `runtimepy-4.1.1/runtimepy/net/server/json.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/net/server/struct/__init__.py` & `runtimepy-4.1.1/runtimepy/net/server/struct/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/net/server/websocket/__init__.py` & `runtimepy-4.1.1/runtimepy/net/server/websocket/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/net/server/websocket/state.py` & `runtimepy-4.1.1/runtimepy/net/server/websocket/state.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/net/stream/__init__.py` & `runtimepy-4.1.1/runtimepy/net/stream/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/net/stream/base.py` & `runtimepy-4.1.1/runtimepy/net/stream/base.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/net/stream/json/base.py` & `runtimepy-4.1.1/runtimepy/net/stream/json/base.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/net/stream/json/handlers.py` & `runtimepy-4.1.1/runtimepy/net/stream/json/handlers.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/net/stream/json/types.py` & `runtimepy-4.1.1/runtimepy/net/stream/json/types.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/net/stream/string.py` & `runtimepy-4.1.1/runtimepy/net/stream/string.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/net/tcp/connection.py` & `runtimepy-4.1.1/runtimepy/net/tcp/connection.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/net/tcp/create.py` & `runtimepy-4.1.1/runtimepy/net/tcp/create.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/net/tcp/http/__init__.py` & `runtimepy-4.1.1/runtimepy/net/tcp/http/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/net/tcp/protocol.py` & `runtimepy-4.1.1/runtimepy/net/tcp/protocol.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/net/tcp/telnet/__init__.py` & `runtimepy-4.1.1/runtimepy/net/tcp/telnet/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/net/tcp/telnet/codes.py` & `runtimepy-4.1.1/runtimepy/net/tcp/telnet/codes.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/net/udp/connection.py` & `runtimepy-4.1.1/runtimepy/net/udp/connection.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/net/udp/create.py` & `runtimepy-4.1.1/runtimepy/net/udp/create.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/net/udp/protocol.py` & `runtimepy-4.1.1/runtimepy/net/udp/protocol.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/net/util.py` & `runtimepy-4.1.1/runtimepy/net/util.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/net/websocket/connection.py` & `runtimepy-4.1.1/runtimepy/net/websocket/connection.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/primitives/__init__.py` & `runtimepy-4.1.1/runtimepy/primitives/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/primitives/array/__init__.py` & `runtimepy-4.1.1/runtimepy/primitives/array/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/primitives/base.py` & `runtimepy-4.1.1/runtimepy/primitives/base.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/primitives/bool.py` & `runtimepy-4.1.1/runtimepy/primitives/bool.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/primitives/byte_order.py` & `runtimepy-4.1.1/runtimepy/primitives/byte_order.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/primitives/field/__init__.py` & `runtimepy-4.1.1/runtimepy/primitives/field/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/primitives/field/fields.py` & `runtimepy-4.1.1/runtimepy/primitives/field/fields.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/primitives/field/manager/__init__.py` & `runtimepy-4.1.1/runtimepy/primitives/field/manager/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/primitives/field/manager/base.py` & `runtimepy-4.1.1/runtimepy/primitives/field/manager/base.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/primitives/float.py` & `runtimepy-4.1.1/runtimepy/primitives/float.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/primitives/int.py` & `runtimepy-4.1.1/runtimepy/primitives/int.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/primitives/scaling.py` & `runtimepy-4.1.1/runtimepy/primitives/scaling.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/primitives/serializable/base.py` & `runtimepy-4.1.1/runtimepy/primitives/serializable/base.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/primitives/serializable/fixed.py` & `runtimepy-4.1.1/runtimepy/primitives/serializable/fixed.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/primitives/serializable/prefixed.py` & `runtimepy-4.1.1/runtimepy/primitives/serializable/prefixed.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/primitives/string.py` & `runtimepy-4.1.1/runtimepy/primitives/string.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/primitives/types/__init__.py` & `runtimepy-4.1.1/runtimepy/primitives/types/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/primitives/types/base.py` & `runtimepy-4.1.1/runtimepy/primitives/types/base.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/primitives/types/bool.py` & `runtimepy-4.1.1/runtimepy/primitives/types/bool.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/primitives/types/bounds.py` & `runtimepy-4.1.1/runtimepy/primitives/types/bounds.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/primitives/types/float.py` & `runtimepy-4.1.1/runtimepy/primitives/types/float.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/primitives/types/int.py` & `runtimepy-4.1.1/runtimepy/primitives/types/int.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/registry/__init__.py` & `runtimepy-4.1.1/runtimepy/registry/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/registry/bool.py` & `runtimepy-4.1.1/runtimepy/registry/bool.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/registry/item.py` & `runtimepy-4.1.1/runtimepy/registry/item.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/registry/name.py` & `runtimepy-4.1.1/runtimepy/registry/name.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/schemas.py` & `runtimepy-4.1.1/runtimepy/schemas.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/struct/__init__.py` & `runtimepy-4.1.1/runtimepy/struct/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/task/asynchronous.py` & `runtimepy-4.1.1/runtimepy/task/asynchronous.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/task/basic/manager.py` & `runtimepy-4.1.1/runtimepy/task/basic/manager.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/task/basic/periodic.py` & `runtimepy-4.1.1/runtimepy/task/basic/periodic.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/task/sample.py` & `runtimepy-4.1.1/runtimepy/task/sample.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/task/trig/__init__.py` & `runtimepy-4.1.1/runtimepy/task/trig/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/tui/channels/__init__.py` & `runtimepy-4.1.1/runtimepy/tui/channels/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/tui/cursor.py` & `runtimepy-4.1.1/runtimepy/tui/cursor.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/tui/mixin.py` & `runtimepy-4.1.1/runtimepy/tui/mixin.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/tui/mock.py` & `runtimepy-4.1.1/runtimepy/tui/mock.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy/tui/task.py` & `runtimepy-4.1.1/runtimepy/tui/task.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/runtimepy.egg-info/PKG-INFO` & `runtimepy-4.1.1/runtimepy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: runtimepy
-Version: 4.1.0
+Version: 4.1.1
 Summary: A framework for implementing Python services.
 Home-page: https://github.com/vkottler/runtimepy
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
@@ -13,18 +13,18 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Unix
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: svgen>=0.6.5
-Requires-Dist: websockets
-Requires-Dist: psutil
 Requires-Dist: vcorelib>=3.2.3
+Requires-Dist: svgen>=0.6.6
+Requires-Dist: psutil
+Requires-Dist: websockets
 Provides-Extra: test
 Requires-Dist: pylint; extra == "test"
 Requires-Dist: flake8; extra == "test"
 Requires-Dist: black; extra == "test"
 Requires-Dist: ruff; extra == "test"
 Requires-Dist: mypy; extra == "test"
 Requires-Dist: isort; extra == "test"
@@ -40,19 +40,19 @@
 Requires-Dist: types-setuptools; extra == "test"
 Requires-Dist: uvloop; (sys_platform != "win32" and sys_platform != "cygwin") and extra == "test"
 
 <!--
     =====================================
     generator=datazen
     version=3.1.4
-    hash=739a1dad9e7a1670fab3bb537c6ea3e9
+    hash=36872ce673f57f77e5b632b95169543d
     =====================================
 -->
 
-# runtimepy ([4.1.0](https://pypi.org/project/runtimepy/))
+# runtimepy ([4.1.1](https://pypi.org/project/runtimepy/))
 
 [![python](https://img.shields.io/pypi/pyversions/runtimepy.svg)](https://pypi.org/project/runtimepy/)
 ![Build Status](https://github.com/vkottler/runtimepy/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/runtimepy/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/runtimepy)
 ![PyPI - Status](https://img.shields.io/pypi/status/runtimepy)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/runtimepy)
```

### Comparing `runtimepy-4.1.0/runtimepy.egg-info/SOURCES.txt` & `runtimepy-4.1.1/runtimepy.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -61,14 +61,15 @@
 runtimepy/data/js/worker.js
 runtimepy/data/js/classes/App.js
 runtimepy/data/js/classes/ChannelTable.js
 runtimepy/data/js/classes/DataConnection.js
 runtimepy/data/js/classes/JsonConnection.js
 runtimepy/data/js/classes/Plot.js
 runtimepy/data/js/classes/PlotManager.js
+runtimepy/data/js/classes/PlotModalManager.js
 runtimepy/data/js/classes/TabFilter.js
 runtimepy/data/js/classes/TabInterface.js
 runtimepy/data/js/classes/WindowHashManager.js
 runtimepy/data/js/classes/WorkerInterface.js
 runtimepy/data/js/tab/env.js
 runtimepy/data/js/tab/sound.js
 runtimepy/data/js/unused/pyodide.js
```

### Comparing `runtimepy-4.1.0/setup.py` & `runtimepy-4.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/tests/test_entry.py` & `runtimepy-4.1.1/tests/test_entry.py`

 * *Files identical despite different names*

### Comparing `runtimepy-4.1.0/tests/test_mapping.py` & `runtimepy-4.1.1/tests/test_mapping.py`

 * *Files identical despite different names*

