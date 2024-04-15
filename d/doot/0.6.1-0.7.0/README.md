# Comparing `tmp/doot-0.6.1.tar.gz` & `tmp/doot-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "doot-0.6.1.tar", last modified: Sat Feb 24 00:39:32 2024, max compression
+gzip compressed data, was "doot-0.7.0.tar", last modified: Mon Apr 15 22:34:36 2024, max compression
```

## Comparing `doot-0.6.1.tar` & `doot-0.7.0.tar`

### file list

```diff
@@ -1,190 +1,186 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 00:39:32.021978 doot-0.6.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-02-24 00:39:24.000000 doot-0.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10172 2024-02-24 00:39:32.021978 doot-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7358 2024-02-24 00:39:24.000000 doot-0.6.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 00:39:31.997978 doot-0.6.1/doot/
--rw-r--r--   0 runner    (1001) docker     (127)     3224 2024-02-24 00:39:24.000000 doot-0.6.1/doot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4344 2024-02-24 00:39:24.000000 doot-0.6.1/doot/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 00:39:32.001978 doot-0.6.1/doot/__templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-02-24 00:39:24.000000 doot-0.6.1/doot/__templates/basic_toml
--rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-02-24 00:39:24.000000 doot-0.6.1/doot/__templates/stub_task_py
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-02-24 00:39:24.000000 doot-0.6.1/doot/__templates/tasks_toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 00:39:32.001978 doot-0.6.1/doot/__tests/
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-02-24 00:39:24.000000 doot-0.6.1/doot/__tests/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-02-24 00:39:24.000000 doot-0.6.1/doot/__tests/test_inits.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 00:39:32.001978 doot-0.6.1/doot/_abstract/
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-02-24 00:39:24.000000 doot-0.6.1/doot/_abstract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2262 2024-02-24 00:39:24.000000 doot-0.6.1/doot/_abstract/cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2762 2024-02-24 00:39:24.000000 doot-0.6.1/doot/_abstract/control.py
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-02-24 00:39:24.000000 doot-0.6.1/doot/_abstract/dbm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2516 2024-02-24 00:39:24.000000 doot-0.6.1/doot/_abstract/loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-02-24 00:39:24.000000 doot-0.6.1/doot/_abstract/overlord.py
--rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-02-24 00:39:24.000000 doot-0.6.1/doot/_abstract/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-02-24 00:39:24.000000 doot-0.6.1/doot/_abstract/policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-02-24 00:39:24.000000 doot-0.6.1/doot/_abstract/reporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     7659 2024-02-24 00:39:24.000000 doot-0.6.1/doot/_abstract/task.py
--rw-r--r--   0 runner    (1001) docker     (127)     7299 2024-02-24 00:39:24.000000 doot-0.6.1/doot/_default_plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 00:39:32.005978 doot-0.6.1/doot/_structs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-24 00:39:24.000000 doot-0.6.1/doot/_structs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 00:39:32.005978 doot-0.6.1/doot/_structs/__tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-02-24 00:39:24.000000 doot-0.6.1/doot/_structs/__tests/test_action_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     4648 2024-02-24 00:39:24.000000 doot-0.6.1/doot/_structs/__tests/test_artifact.py
--rw-r--r--   0 runner    (1001) docker     (127)     2983 2024-02-24 00:39:24.000000 doot-0.6.1/doot/_structs/__tests/test_formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)    30375 2024-02-24 00:39:24.000000 doot-0.6.1/doot/_structs/__tests/test_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     6059 2024-02-24 00:39:24.000000 doot-0.6.1/doot/_structs/__tests/test_param_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     8876 2024-02-24 00:39:24.000000 doot-0.6.1/doot/_structs/__tests/test_sname.py
--rw-r--r--   0 runner    (1001) docker     (127)     4035 2024-02-24 00:39:24.000000 doot-0.6.1/doot/_structs/__tests/test_stub.py
--rw-r--r--   0 runner    (1001) docker     (127)     7759 2024-02-24 00:39:24.000000 doot-0.6.1/doot/_structs/__tests/test_task_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     5255 2024-02-24 00:39:24.000000 doot-0.6.1/doot/_structs/action_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     3402 2024-02-24 00:39:24.000000 doot-0.6.1/doot/_structs/artifact.py
--rw-r--r--   0 runner    (1001) docker     (127)     6424 2024-02-24 00:39:24.000000 doot-0.6.1/doot/_structs/code_ref.py
--rw-r--r--   0 runner    (1001) docker     (127)    30332 2024-02-24 00:39:24.000000 doot-0.6.1/doot/_structs/key.py
--rw-r--r--   0 runner    (1001) docker     (127)    11913 2024-02-24 00:39:24.000000 doot-0.6.1/doot/_structs/param_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2510 2024-02-24 00:39:24.000000 doot-0.6.1/doot/_structs/sname.py
--rw-r--r--   0 runner    (1001) docker     (127)     3665 2024-02-24 00:39:24.000000 doot-0.6.1/doot/_structs/structured_name.py
--rw-r--r--   0 runner    (1001) docker     (127)     7801 2024-02-24 00:39:24.000000 doot-0.6.1/doot/_structs/stub.py
--rw-r--r--   0 runner    (1001) docker     (127)     5341 2024-02-24 00:39:24.000000 doot-0.6.1/doot/_structs/task_name.py
--rw-r--r--   0 runner    (1001) docker     (127)    11725 2024-02-24 00:39:24.000000 doot-0.6.1/doot/_structs/task_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-02-24 00:39:24.000000 doot-0.6.1/doot/_structs/trace.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 00:39:32.009978 doot-0.6.1/doot/actions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-24 00:39:24.000000 doot-0.6.1/doot/actions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 00:39:32.009978 doot-0.6.1/doot/actions/__tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-02-24 00:39:24.000000 doot-0.6.1/doot/actions/__tests/test_base_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-02-24 00:39:24.000000 doot-0.6.1/doot/actions/__tests/test_control_flow.py
--rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-02-24 00:39:24.000000 doot-0.6.1/doot/actions/__tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-02-24 00:39:24.000000 doot-0.6.1/doot/actions/__tests/test_postbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-02-24 00:39:24.000000 doot-0.6.1/doot/actions/__tests/test_shell.py
--rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-02-24 00:39:24.000000 doot-0.6.1/doot/actions/__tests/test_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-02-24 00:39:24.000000 doot-0.6.1/doot/actions/base_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     4071 2024-02-24 00:39:24.000000 doot-0.6.1/doot/actions/compression.py
--rw-r--r--   0 runner    (1001) docker     (127)     3314 2024-02-24 00:39:24.000000 doot-0.6.1/doot/actions/control_flow.py
--rw-r--r--   0 runner    (1001) docker     (127)    12794 2024-02-24 00:39:24.000000 doot-0.6.1/doot/actions/io.py
--rw-r--r--   0 runner    (1001) docker     (127)     2194 2024-02-24 00:39:24.000000 doot-0.6.1/doot/actions/json.py
--rw-r--r--   0 runner    (1001) docker     (127)     5898 2024-02-24 00:39:24.000000 doot-0.6.1/doot/actions/postbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     6991 2024-02-24 00:39:24.000000 doot-0.6.1/doot/actions/shell.py
--rw-r--r--   0 runner    (1001) docker     (127)     3135 2024-02-24 00:39:24.000000 doot-0.6.1/doot/actions/speak.py
--rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-02-24 00:39:24.000000 doot-0.6.1/doot/actions/state.py
--rw-r--r--   0 runner    (1001) docker     (127)      939 2024-02-24 00:39:24.000000 doot-0.6.1/doot/actions/templater.py
--rw-r--r--   0 runner    (1001) docker     (127)     1973 2024-02-24 00:39:24.000000 doot-0.6.1/doot/actions/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 00:39:32.009978 doot-0.6.1/doot/cmds/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-24 00:39:24.000000 doot-0.6.1/doot/cmds/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 00:39:32.009978 doot-0.6.1/doot/cmds/__tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5122 2024-02-24 00:39:24.000000 doot-0.6.1/doot/cmds/__tests/test_list_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     4027 2024-02-24 00:39:24.000000 doot-0.6.1/doot/cmds/clean_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-02-24 00:39:24.000000 doot-0.6.1/doot/cmds/complete_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-02-24 00:39:24.000000 doot-0.6.1/doot/cmds/daemon_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     5131 2024-02-24 00:39:24.000000 doot-0.6.1/doot/cmds/graph_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     5871 2024-02-24 00:39:24.000000 doot-0.6.1/doot/cmds/help_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-02-24 00:39:24.000000 doot-0.6.1/doot/cmds/here_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2889 2024-02-24 00:39:24.000000 doot-0.6.1/doot/cmds/last_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     7664 2024-02-24 00:39:24.000000 doot-0.6.1/doot/cmds/list_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2586 2024-02-24 00:39:24.000000 doot-0.6.1/doot/cmds/locs_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     4211 2024-02-24 00:39:24.000000 doot-0.6.1/doot/cmds/plugins_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     4098 2024-02-24 00:39:24.000000 doot-0.6.1/doot/cmds/run_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-02-24 00:39:24.000000 doot-0.6.1/doot/cmds/server_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     3804 2024-02-24 00:39:24.000000 doot-0.6.1/doot/cmds/step_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     9747 2024-02-24 00:39:24.000000 doot-0.6.1/doot/cmds/stub_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     3050 2024-02-24 00:39:24.000000 doot-0.6.1/doot/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 00:39:32.013978 doot-0.6.1/doot/control/
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-24 00:39:24.000000 doot-0.6.1/doot/control/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 00:39:32.013978 doot-0.6.1/doot/control/__tests/
--rw-r--r--   0 runner    (1001) docker     (127)     8058 2024-02-24 00:39:24.000000 doot-0.6.1/doot/control/__tests/test_locations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2944 2024-02-24 00:39:24.000000 doot-0.6.1/doot/control/__tests/test_overlord.py
--rw-r--r--   0 runner    (1001) docker     (127)     7315 2024-02-24 00:39:24.000000 doot-0.6.1/doot/control/__tests/test_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)    11955 2024-02-24 00:39:24.000000 doot-0.6.1/doot/control/__tests/test_tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)     5338 2024-02-24 00:39:24.000000 doot-0.6.1/doot/control/base_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)    17621 2024-02-24 00:39:24.000000 doot-0.6.1/doot/control/base_tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-02-24 00:39:24.000000 doot-0.6.1/doot/control/date_tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)     8545 2024-02-24 00:39:24.000000 doot-0.6.1/doot/control/locations.py
--rw-r--r--   0 runner    (1001) docker     (127)    10176 2024-02-24 00:39:24.000000 doot-0.6.1/doot/control/overlord.py
--rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-02-24 00:39:24.000000 doot-0.6.1/doot/control/policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     9116 2024-02-24 00:39:24.000000 doot-0.6.1/doot/control/runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     8405 2024-02-24 00:39:24.000000 doot-0.6.1/doot/control/step_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     8512 2024-02-24 00:39:24.000000 doot-0.6.1/doot/control/tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)     3022 2024-02-24 00:39:24.000000 doot-0.6.1/doot/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     3023 2024-02-24 00:39:24.000000 doot-0.6.1/doot/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 00:39:32.013978 doot-0.6.1/doot/loaders/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-24 00:39:24.000000 doot-0.6.1/doot/loaders/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 00:39:32.013978 doot-0.6.1/doot/loaders/__tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-02-24 00:39:24.000000 doot-0.6.1/doot/loaders/__tests/test_cmd_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-02-24 00:39:24.000000 doot-0.6.1/doot/loaders/__tests/test_plugin_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     7235 2024-02-24 00:39:24.000000 doot-0.6.1/doot/loaders/__tests/test_task_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-02-24 00:39:24.000000 doot-0.6.1/doot/loaders/cmd_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     5865 2024-02-24 00:39:24.000000 doot-0.6.1/doot/loaders/plugin_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)    12323 2024-02-24 00:39:24.000000 doot-0.6.1/doot/loaders/task_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 00:39:32.013978 doot-0.6.1/doot/mixins/
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-24 00:39:24.000000 doot-0.6.1/doot/mixins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 00:39:32.013978 doot-0.6.1/doot/mixins/action/
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-24 00:39:24.000000 doot-0.6.1/doot/mixins/action/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3731 2024-02-24 00:39:24.000000 doot-0.6.1/doot/mixins/action/batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-02-24 00:39:24.000000 doot-0.6.1/doot/mixins/action/cleaning.py
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-02-24 00:39:24.000000 doot-0.6.1/doot/mixins/action/human_numbers.py
--rw-r--r--   0 runner    (1001) docker     (127)     8401 2024-02-24 00:39:24.000000 doot-0.6.1/doot/mixins/action/zipper.py
--rw-r--r--   0 runner    (1001) docker     (127)     4288 2024-02-24 00:39:24.000000 doot-0.6.1/doot/mixins/importer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 00:39:32.017978 doot-0.6.1/doot/mixins/job/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 00:39:32.017978 doot-0.6.1/doot/mixins/job/__tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5198 2024-02-24 00:39:24.000000 doot-0.6.1/doot/mixins/job/__tests/test_expander.py
--rw-r--r--   0 runner    (1001) docker     (127)     2797 2024-02-24 00:39:24.000000 doot-0.6.1/doot/mixins/job/__tests/test_limiter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3101 2024-02-24 00:39:24.000000 doot-0.6.1/doot/mixins/job/__tests/test_matcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-02-24 00:39:24.000000 doot-0.6.1/doot/mixins/job/__tests/test_shadower.py
--rw-r--r--   0 runner    (1001) docker     (127)     3123 2024-02-24 00:39:24.000000 doot-0.6.1/doot/mixins/job/__tests/test_subtask.py
--rw-r--r--   0 runner    (1001) docker     (127)     3636 2024-02-24 00:39:24.000000 doot-0.6.1/doot/mixins/job/__tests/test_terse.py
--rw-r--r--   0 runner    (1001) docker     (127)    13070 2024-02-24 00:39:24.000000 doot-0.6.1/doot/mixins/job/expander.py
--rw-r--r--   0 runner    (1001) docker     (127)     4643 2024-02-24 00:39:24.000000 doot-0.6.1/doot/mixins/job/limiter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4175 2024-02-24 00:39:24.000000 doot-0.6.1/doot/mixins/job/matcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-02-24 00:39:24.000000 doot-0.6.1/doot/mixins/job/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     4045 2024-02-24 00:39:24.000000 doot-0.6.1/doot/mixins/job/shadower.py
--rw-r--r--   0 runner    (1001) docker     (127)     3960 2024-02-24 00:39:24.000000 doot-0.6.1/doot/mixins/job/subtask.py
--rw-r--r--   0 runner    (1001) docker     (127)     3526 2024-02-24 00:39:24.000000 doot-0.6.1/doot/mixins/job/terse.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 00:39:32.017978 doot-0.6.1/doot/mixins/runner/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-24 00:39:24.000000 doot-0.6.1/doot/mixins/runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-02-24 00:39:24.000000 doot-0.6.1/doot/mixins/runner/fail_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 00:39:32.017978 doot-0.6.1/doot/mixins/task/
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-24 00:39:24.000000 doot-0.6.1/doot/mixins/task/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 00:39:32.017978 doot-0.6.1/doot/parsers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-24 00:39:24.000000 doot-0.6.1/doot/parsers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 00:39:32.017978 doot-0.6.1/doot/parsers/__tests/
--rw-r--r--   0 runner    (1001) docker     (127)    13764 2024-02-24 00:39:24.000000 doot-0.6.1/doot/parsers/__tests/test_flexible.py
--rw-r--r--   0 runner    (1001) docker     (127)    10873 2024-02-24 00:39:24.000000 doot-0.6.1/doot/parsers/flexible.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 00:39:32.017978 doot-0.6.1/doot/reporters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-24 00:39:24.000000 doot-0.6.1/doot/reporters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 00:39:32.017978 doot-0.6.1/doot/reporters/__tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3976 2024-02-24 00:39:24.000000 doot-0.6.1/doot/reporters/__tests/test_stack_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-02-24 00:39:24.000000 doot-0.6.1/doot/reporters/__tests/test_summary_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-02-24 00:39:24.000000 doot-0.6.1/doot/reporters/basic_reporters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-02-24 00:39:24.000000 doot-0.6.1/doot/reporters/stack_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-02-24 00:39:24.000000 doot-0.6.1/doot/reporters/summary_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-02-24 00:39:24.000000 doot-0.6.1/doot/structs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 00:39:32.021978 doot-0.6.1/doot/task/
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-02-24 00:39:24.000000 doot-0.6.1/doot/task/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 00:39:32.021978 doot-0.6.1/doot/task/__tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-02-24 00:39:24.000000 doot-0.6.1/doot/task/__tests/test_base_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     4129 2024-02-24 00:39:24.000000 doot-0.6.1/doot/task/__tests/test_base_task.py
--rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-02-24 00:39:24.000000 doot-0.6.1/doot/task/__tests/test_check_locs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4147 2024-02-24 00:39:24.000000 doot-0.6.1/doot/task/base_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     3986 2024-02-24 00:39:24.000000 doot-0.6.1/doot/task/base_task.py
--rw-r--r--   0 runner    (1001) docker     (127)     1727 2024-02-24 00:39:24.000000 doot-0.6.1/doot/task/check_locs.py
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-02-24 00:39:24.000000 doot-0.6.1/doot/task/dev_scaffold.py
--rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-02-24 00:39:24.000000 doot-0.6.1/doot/task/specialised_jobs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 00:39:32.021978 doot-0.6.1/doot/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-24 00:39:24.000000 doot-0.6.1/doot/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-02-24 00:39:24.000000 doot-0.6.1/doot/utils/check_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)     4525 2024-02-24 00:39:24.000000 doot-0.6.1/doot/utils/log_colour.py
--rw-r--r--   0 runner    (1001) docker     (127)     5336 2024-02-24 00:39:24.000000 doot-0.6.1/doot/utils/log_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-02-24 00:39:24.000000 doot-0.6.1/doot/utils/log_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     5188 2024-02-24 00:39:24.000000 doot-0.6.1/doot/utils/mock_gen.py
--rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-02-24 00:39:24.000000 doot-0.6.1/doot/utils/plugin_selector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-02-24 00:39:24.000000 doot-0.6.1/doot/utils/retrievers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-02-24 00:39:24.000000 doot-0.6.1/doot/utils/signal_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-02-24 00:39:24.000000 doot-0.6.1/doot/utils/testing_fixtures.py
--rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-02-24 00:39:24.000000 doot-0.6.1/doot/utils/trace_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-02-24 00:39:24.000000 doot-0.6.1/doot/utils/url_expand.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 00:39:32.021978 doot-0.6.1/doot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10172 2024-02-24 00:39:31.000000 doot-0.6.1/doot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4466 2024-02-24 00:39:31.000000 doot-0.6.1/doot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-24 00:39:31.000000 doot-0.6.1/doot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-02-24 00:39:31.000000 doot-0.6.1/doot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-02-24 00:39:31.000000 doot-0.6.1/doot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-24 00:39:31.000000 doot-0.6.1/doot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-02-24 00:39:24.000000 doot-0.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-24 00:39:32.021978 doot-0.6.1/setup.cfg
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-15 22:34:36.949531 doot-0.7.0/
+-rw-rw-r--   0 john      (1000) john      (1000)     1421 2023-12-10 00:45:10.000000 doot-0.7.0/LICENSE
+-rw-r--r--   0 john      (1000) john      (1000)    10267 2024-04-15 22:34:36.949531 doot-0.7.0/PKG-INFO
+-rw-rw-r--   0 john      (1000) john      (1000)     7358 2024-04-15 22:32:56.000000 doot-0.7.0/README.md
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-15 22:34:36.929531 doot-0.7.0/doot/
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-15 22:34:36.929531 doot-0.7.0/doot/__data/
+-rw-rw-r--   0 john      (1000) john      (1000)     5167 2024-04-15 22:30:11.000000 doot-0.7.0/doot/__data/aliases.toml
+-rw-rw-r--   0 john      (1000) john      (1000)     2277 2024-04-15 22:30:11.000000 doot-0.7.0/doot/__data/constants.toml
+-rw-rw-r--   0 john      (1000) john      (1000)     5218 2024-04-15 22:32:56.000000 doot-0.7.0/doot/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)     3414 2024-04-15 22:30:11.000000 doot-0.7.0/doot/__main__.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-15 22:34:36.929531 doot-0.7.0/doot/__templates/
+-rw-rw-r--   0 john      (1000) john      (1000)     1413 2024-04-15 22:30:11.000000 doot-0.7.0/doot/__templates/basic_toml
+-rw-rw-r--   0 john      (1000) john      (1000)     2000 2024-04-15 22:30:11.000000 doot-0.7.0/doot/__templates/stub_task_py
+-rw-rw-r--   0 john      (1000) john      (1000)      357 2023-12-09 23:29:38.000000 doot-0.7.0/doot/__templates/tasks_toml
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-15 22:34:36.929531 doot-0.7.0/doot/__tests/
+-rw-rw-r--   0 john      (1000) john      (1000)      996 2024-04-15 22:30:11.000000 doot-0.7.0/doot/__tests/test_basic.py
+-rw-rw-r--   0 john      (1000) john      (1000)      615 2024-04-15 22:30:11.000000 doot-0.7.0/doot/__tests/test_inits.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-15 22:34:36.933531 doot-0.7.0/doot/_abstract/
+-rw-rw-r--   0 john      (1000) john      (1000)      786 2024-04-15 22:30:11.000000 doot-0.7.0/doot/_abstract/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1158 2024-04-15 22:30:11.000000 doot-0.7.0/doot/_abstract/cmd.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2712 2024-04-15 22:30:11.000000 doot-0.7.0/doot/_abstract/control.py
+-rw-rwxr--   0 john      (1000) john      (1000)     1367 2023-10-17 22:05:44.000000 doot-0.7.0/doot/_abstract/dbm.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2464 2024-04-15 22:30:11.000000 doot-0.7.0/doot/_abstract/loader.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1289 2024-04-15 22:30:11.000000 doot-0.7.0/doot/_abstract/overlord.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1700 2024-04-15 22:30:11.000000 doot-0.7.0/doot/_abstract/parser.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1004 2023-12-10 23:41:06.000000 doot-0.7.0/doot/_abstract/policy.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1695 2024-04-15 22:30:11.000000 doot-0.7.0/doot/_abstract/reporter.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1408 2024-04-15 22:30:11.000000 doot-0.7.0/doot/_abstract/structs.py
+-rw-rw-r--   0 john      (1000) john      (1000)     4736 2024-04-15 22:30:11.000000 doot-0.7.0/doot/_abstract/task.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-15 22:34:36.933531 doot-0.7.0/doot/_structs/
+-rw-rw-r--   0 john      (1000) john      (1000)        0 2023-12-09 23:29:38.000000 doot-0.7.0/doot/_structs/__init__.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-15 22:34:36.937531 doot-0.7.0/doot/_structs/__tests/
+-rw-rw-r--   0 john      (1000) john      (1000)     1325 2024-04-15 22:30:11.000000 doot-0.7.0/doot/_structs/__tests/test_action_spec.py
+-rw-rw-r--   0 john      (1000) john      (1000)     4945 2024-04-15 22:30:11.000000 doot-0.7.0/doot/_structs/__tests/test_artifact.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2034 2024-04-15 22:30:11.000000 doot-0.7.0/doot/_structs/__tests/test_code_ref.py
+-rw-rw-r--   0 john      (1000) john      (1000)     3131 2024-04-15 22:30:11.000000 doot-0.7.0/doot/_structs/__tests/test_formatter.py
+-rw-rw-r--   0 john      (1000) john      (1000)    13645 2024-04-15 22:30:11.000000 doot-0.7.0/doot/_structs/__tests/test_key.py
+-rw-rw-r--   0 john      (1000) john      (1000)     5200 2024-04-15 22:30:11.000000 doot-0.7.0/doot/_structs/__tests/test_key_decorators.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2361 2024-04-15 22:30:11.000000 doot-0.7.0/doot/_structs/__tests/test_key_multi.py
+-rw-rw-r--   0 john      (1000) john      (1000)     7054 2024-04-15 22:30:11.000000 doot-0.7.0/doot/_structs/__tests/test_key_path_expansion.py
+-rw-rw-r--   0 john      (1000) john      (1000)     4431 2024-04-15 22:30:11.000000 doot-0.7.0/doot/_structs/__tests/test_key_string_expansion.py
+-rw-rw-r--   0 john      (1000) john      (1000)     3700 2024-04-15 22:30:11.000000 doot-0.7.0/doot/_structs/__tests/test_key_type_expansion.py
+-rw-rw-r--   0 john      (1000) john      (1000)     6022 2024-04-15 22:30:11.000000 doot-0.7.0/doot/_structs/__tests/test_param_spec.py
+-rw-rw-r--   0 john      (1000) john      (1000)     3765 2024-04-15 22:30:11.000000 doot-0.7.0/doot/_structs/__tests/test_stub.py
+-rw-rw-r--   0 john      (1000) john      (1000)     8076 2024-04-15 22:30:11.000000 doot-0.7.0/doot/_structs/__tests/test_task_name.py
+-rw-rw-r--   0 john      (1000) john      (1000)     7701 2024-04-15 22:30:11.000000 doot-0.7.0/doot/_structs/__tests/test_task_spec.py
+-rw-rw-r--   0 john      (1000) john      (1000)     5489 2024-04-15 22:30:11.000000 doot-0.7.0/doot/_structs/action_spec.py
+-rw-rw-r--   0 john      (1000) john      (1000)     4980 2024-04-15 22:30:11.000000 doot-0.7.0/doot/_structs/artifact.py
+-rw-rw-r--   0 john      (1000) john      (1000)     6769 2024-04-15 22:30:11.000000 doot-0.7.0/doot/_structs/code_ref.py
+-rw-rw-r--   0 john      (1000) john      (1000)    32021 2024-04-15 22:30:11.000000 doot-0.7.0/doot/_structs/key.py
+-rw-rw-r--   0 john      (1000) john      (1000)      172 2023-12-11 21:35:03.000000 doot-0.7.0/doot/_structs/log.doot
+-rw-rw-r--   0 john      (1000) john      (1000)    11997 2024-04-15 22:30:11.000000 doot-0.7.0/doot/_structs/param_spec.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2509 2024-04-15 22:30:11.000000 doot-0.7.0/doot/_structs/sname.py
+-rw-rw-r--   0 john      (1000) john      (1000)     3987 2024-04-15 22:30:11.000000 doot-0.7.0/doot/_structs/structured_name.py
+-rw-rw-r--   0 john      (1000) john      (1000)     8066 2024-04-15 22:30:11.000000 doot-0.7.0/doot/_structs/stub.py
+-rw-rw-r--   0 john      (1000) john      (1000)     7258 2024-04-15 22:30:11.000000 doot-0.7.0/doot/_structs/task_name.py
+-rw-rw-r--   0 john      (1000) john      (1000)    12777 2024-04-15 22:30:11.000000 doot-0.7.0/doot/_structs/task_spec.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2472 2024-04-15 22:30:11.000000 doot-0.7.0/doot/_structs/toml_loc.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1956 2024-04-15 22:30:11.000000 doot-0.7.0/doot/_structs/trace.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-15 22:34:36.937531 doot-0.7.0/doot/actions/
+-rw-rwxr--   0 john      (1000) john      (1000)        0 2023-10-17 22:05:44.000000 doot-0.7.0/doot/actions/__init__.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-15 22:34:36.937531 doot-0.7.0/doot/actions/__tests/
+-rw-rw-r--   0 john      (1000) john      (1000)     1039 2024-04-15 22:30:11.000000 doot-0.7.0/doot/actions/__tests/test_base_action.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1349 2024-04-15 22:30:11.000000 doot-0.7.0/doot/actions/__tests/test_control_flow.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1349 2024-04-15 22:30:11.000000 doot-0.7.0/doot/actions/__tests/test_io.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2925 2024-04-15 22:30:11.000000 doot-0.7.0/doot/actions/__tests/test_job_actions.py
+-rw-rw-r--   0 john      (1000) john      (1000)     3371 2024-04-15 22:30:11.000000 doot-0.7.0/doot/actions/__tests/test_job_expansion.py
+-rw-rw-r--   0 john      (1000) john      (1000)     4417 2024-04-15 22:30:11.000000 doot-0.7.0/doot/actions/__tests/test_job_injection.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2896 2024-04-15 22:30:11.000000 doot-0.7.0/doot/actions/__tests/test_job_queuing.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1349 2024-04-15 22:30:11.000000 doot-0.7.0/doot/actions/__tests/test_postbox.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1349 2024-04-15 22:30:11.000000 doot-0.7.0/doot/actions/__tests/test_shell.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1349 2024-04-15 22:30:11.000000 doot-0.7.0/doot/actions/__tests/test_state.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1565 2024-04-15 22:30:11.000000 doot-0.7.0/doot/actions/base_action.py
+-rw-rw-r--   0 john      (1000) john      (1000)     5462 2024-04-15 22:30:11.000000 doot-0.7.0/doot/actions/compression.py
+-rw-rw-r--   0 john      (1000) john      (1000)     4973 2024-04-15 22:30:11.000000 doot-0.7.0/doot/actions/control_flow.py
+-rw-rw-r--   0 john      (1000) john      (1000)    12958 2024-04-15 22:30:11.000000 doot-0.7.0/doot/actions/io.py
+-rw-rw-r--   0 john      (1000) john      (1000)     3081 2024-04-15 22:30:11.000000 doot-0.7.0/doot/actions/job_actions.py
+-rw-rw-r--   0 john      (1000) john      (1000)     4930 2024-04-15 22:30:11.000000 doot-0.7.0/doot/actions/job_expansion.py
+-rw-rw-r--   0 john      (1000) john      (1000)     7012 2024-04-15 22:30:11.000000 doot-0.7.0/doot/actions/job_injection.py
+-rw-rw-r--   0 john      (1000) john      (1000)     4684 2024-04-15 22:30:11.000000 doot-0.7.0/doot/actions/job_queuing.py
+-rw-rw-r--   0 john      (1000) john      (1000)     3902 2024-04-15 22:30:11.000000 doot-0.7.0/doot/actions/json.py
+-rw-rw-r--   0 john      (1000) john      (1000)     5791 2024-04-15 22:30:11.000000 doot-0.7.0/doot/actions/postbox.py
+-rw-rw-r--   0 john      (1000) john      (1000)     6896 2024-04-15 22:30:11.000000 doot-0.7.0/doot/actions/shell.py
+-rw-rw-r--   0 john      (1000) john      (1000)     3112 2024-04-15 22:30:11.000000 doot-0.7.0/doot/actions/speak.py
+-rw-rw-r--   0 john      (1000) john      (1000)     4057 2024-04-15 22:30:11.000000 doot-0.7.0/doot/actions/state.py
+-rw-rw-r--   0 john      (1000) john      (1000)      939 2024-01-20 20:13:07.000000 doot-0.7.0/doot/actions/templater.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1973 2023-12-09 23:29:38.000000 doot-0.7.0/doot/actions/util.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-15 22:34:36.941531 doot-0.7.0/doot/cmds/
+-rw-rwxr--   0 john      (1000) john      (1000)        0 2023-10-17 22:05:44.000000 doot-0.7.0/doot/cmds/__init__.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-15 22:34:36.941531 doot-0.7.0/doot/cmds/__tests/
+-rw-rw-r--   0 john      (1000) john      (1000)     5119 2024-04-15 22:30:11.000000 doot-0.7.0/doot/cmds/__tests/test_list_cmd.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2473 2024-04-15 22:30:11.000000 doot-0.7.0/doot/cmds/base_cmd.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2146 2024-04-15 22:30:11.000000 doot-0.7.0/doot/cmds/clean_cmd.py
+-rw-rw-r--   0 john      (1000) john      (1000)     5149 2024-04-15 22:30:11.000000 doot-0.7.0/doot/cmds/graph_cmd.py
+-rw-rw-r--   0 john      (1000) john      (1000)     5900 2024-04-15 22:30:11.000000 doot-0.7.0/doot/cmds/help_cmd.py
+-rw-rw-r--   0 john      (1000) john      (1000)     7784 2024-04-15 22:30:11.000000 doot-0.7.0/doot/cmds/list_cmd.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2606 2024-04-15 22:30:11.000000 doot-0.7.0/doot/cmds/locs_cmd.py
+-rw-rw-r--   0 john      (1000) john      (1000)     4222 2024-04-15 22:30:11.000000 doot-0.7.0/doot/cmds/plugins_cmd.py
+-rw-rw-r--   0 john      (1000) john      (1000)     4284 2024-04-15 22:30:11.000000 doot-0.7.0/doot/cmds/run_cmd.py
+-rw-rw-r--   0 john      (1000) john      (1000)     3841 2024-04-15 22:30:11.000000 doot-0.7.0/doot/cmds/step_cmd.py
+-rw-rw-r--   0 john      (1000) john      (1000)     9911 2024-04-15 22:30:11.000000 doot-0.7.0/doot/cmds/stub_cmd.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-15 22:34:36.941531 doot-0.7.0/doot/control/
+-rw-rwxr--   0 john      (1000) john      (1000)       10 2023-10-17 22:05:44.000000 doot-0.7.0/doot/control/__init__.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-15 22:34:36.941531 doot-0.7.0/doot/control/__tests/
+-rw-rw-r--   0 john      (1000) john      (1000)     8111 2024-04-15 22:30:11.000000 doot-0.7.0/doot/control/__tests/test_locations.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2887 2024-04-15 22:30:11.000000 doot-0.7.0/doot/control/__tests/test_overlord.py
+-rw-rw-r--   0 john      (1000) john      (1000)     5794 2024-04-15 22:30:11.000000 doot-0.7.0/doot/control/__tests/test_runner.py
+-rw-rw-r--   0 john      (1000) john      (1000)    13774 2024-04-15 22:30:11.000000 doot-0.7.0/doot/control/__tests/test_tracker.py
+-rw-rw-r--   0 john      (1000) john      (1000)     6410 2024-04-15 22:30:11.000000 doot-0.7.0/doot/control/base_runner.py
+-rw-rw-r--   0 john      (1000) john      (1000)    18149 2024-04-15 22:30:11.000000 doot-0.7.0/doot/control/base_tracker.py
+-rw-rw-r--   0 john      (1000) john      (1000)     8389 2024-04-15 22:30:11.000000 doot-0.7.0/doot/control/locations.py
+-rw-rw-r--   0 john      (1000) john      (1000)      172 2023-11-03 03:34:45.000000 doot-0.7.0/doot/control/log.doot
+-rw-rw-r--   0 john      (1000) john      (1000)    11575 2024-04-15 22:30:11.000000 doot-0.7.0/doot/control/overlord.py
+-rw-rw-r--   0 john      (1000) john      (1000)    11246 2024-04-15 22:30:11.000000 doot-0.7.0/doot/control/runner.py
+-rw-rw-r--   0 john      (1000) john      (1000)     8423 2024-04-15 22:30:11.000000 doot-0.7.0/doot/control/step_runner.py
+-rw-rw-r--   0 john      (1000) john      (1000)     8503 2024-04-15 22:30:11.000000 doot-0.7.0/doot/control/tracker.py
+-rw-rw-r--   0 john      (1000) john      (1000)     3546 2024-04-15 22:30:11.000000 doot-0.7.0/doot/enums.py
+-rw-rw-r--   0 john      (1000) john      (1000)     3023 2024-04-14 21:07:32.000000 doot-0.7.0/doot/errors.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-15 22:34:36.941531 doot-0.7.0/doot/loaders/
+-rw-rwxr--   0 john      (1000) john      (1000)        0 2023-10-17 22:05:44.000000 doot-0.7.0/doot/loaders/__init__.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-15 22:34:36.941531 doot-0.7.0/doot/loaders/__tests/
+-rw-rw-r--   0 john      (1000) john      (1000)     1851 2024-04-15 22:30:11.000000 doot-0.7.0/doot/loaders/__tests/test_cmd_loader.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1001 2024-04-15 22:30:11.000000 doot-0.7.0/doot/loaders/__tests/test_plugin_loader.py
+-rw-rw-r--   0 john      (1000) john      (1000)     7251 2024-04-15 22:30:11.000000 doot-0.7.0/doot/loaders/__tests/test_task_loader.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2484 2023-12-10 23:41:06.000000 doot-0.7.0/doot/loaders/cmd_loader.py
+-rw-rw-r--   0 john      (1000) john      (1000)     6048 2024-04-15 22:30:11.000000 doot-0.7.0/doot/loaders/plugin_loader.py
+-rw-rw-r--   0 john      (1000) john      (1000)    12082 2024-04-15 22:30:11.000000 doot-0.7.0/doot/loaders/task_loader.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-15 22:34:36.945531 doot-0.7.0/doot/mixins/
+-rw-r-xr--   0 john      (1000) john      (1000)       10 2023-10-05 00:53:38.000000 doot-0.7.0/doot/mixins/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1993 2024-04-15 22:30:11.000000 doot-0.7.0/doot/mixins/enums.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1161 2024-04-15 22:30:11.000000 doot-0.7.0/doot/mixins/fail_handler.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1719 2024-04-15 22:30:11.000000 doot-0.7.0/doot/mixins/human_numbers.py
+-rw-rw-r--   0 john      (1000) john      (1000)     4443 2024-04-15 22:30:11.000000 doot-0.7.0/doot/mixins/importer.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1185 2024-04-15 22:30:11.000000 doot-0.7.0/doot/mixins/param_spec.py
+-rw-rw-r--   0 john      (1000) john      (1000)     7321 2024-04-15 22:30:11.000000 doot-0.7.0/doot/mixins/path_manip.py
+-rw-rw-r--   0 john      (1000) john      (1000)     8963 2024-04-15 22:30:11.000000 doot-0.7.0/doot/mixins/zipper.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-15 22:34:36.945531 doot-0.7.0/doot/parsers/
+-rw-rwxr--   0 john      (1000) john      (1000)        0 2023-10-17 22:05:44.000000 doot-0.7.0/doot/parsers/__init__.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-15 22:34:36.945531 doot-0.7.0/doot/parsers/__tests/
+-rw-rw-r--   0 john      (1000) john      (1000)    13792 2024-04-15 22:30:11.000000 doot-0.7.0/doot/parsers/__tests/test_flexible.py
+-rw-rw-r--   0 john      (1000) john      (1000)    10925 2024-04-15 22:30:11.000000 doot-0.7.0/doot/parsers/flexible.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-15 22:34:36.945531 doot-0.7.0/doot/reporters/
+-rw-r-xr--   0 john      (1000) john      (1000)        0 2023-10-05 00:53:38.000000 doot-0.7.0/doot/reporters/__init__.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-15 22:34:36.945531 doot-0.7.0/doot/reporters/__tests/
+-rw-rw-r--   0 john      (1000) john      (1000)     4152 2024-04-15 22:30:11.000000 doot-0.7.0/doot/reporters/__tests/test_stack_manager.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2100 2024-04-15 22:30:11.000000 doot-0.7.0/doot/reporters/__tests/test_summary_manager.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1232 2024-04-15 22:30:11.000000 doot-0.7.0/doot/reporters/basic_reporters.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1533 2024-04-14 20:23:48.000000 doot-0.7.0/doot/reporters/stack_manager.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2933 2024-04-14 20:23:55.000000 doot-0.7.0/doot/reporters/summary_manager.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1258 2024-04-15 22:30:11.000000 doot-0.7.0/doot/structs.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-15 22:34:36.945531 doot-0.7.0/doot/task/
+-rw-rw-r--   0 john      (1000) john      (1000)       89 2024-01-20 20:13:07.000000 doot-0.7.0/doot/task/__init__.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-15 22:34:36.945531 doot-0.7.0/doot/task/__tests/
+-rw-rw-r--   0 john      (1000) john      (1000)     1536 2024-04-15 22:30:11.000000 doot-0.7.0/doot/task/__tests/test_base_job.py
+-rw-rw-r--   0 john      (1000) john      (1000)     4104 2024-04-15 22:30:11.000000 doot-0.7.0/doot/task/__tests/test_base_task.py
+-rw-rw-r--   0 john      (1000) john      (1000)      749 2024-04-15 22:30:11.000000 doot-0.7.0/doot/task/__tests/test_check_locs.py
+-rw-rw-r--   0 john      (1000) john      (1000)     4452 2024-04-15 22:30:11.000000 doot-0.7.0/doot/task/base_job.py
+-rw-rw-r--   0 john      (1000) john      (1000)     7941 2024-04-15 22:30:11.000000 doot-0.7.0/doot/task/base_task.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1813 2024-04-15 22:30:11.000000 doot-0.7.0/doot/task/check_locs.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1771 2024-01-20 20:13:07.000000 doot-0.7.0/doot/task/specialised_jobs.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-15 22:34:36.945531 doot-0.7.0/doot/utils/
+-rw-r-xr--   0 john      (1000) john      (1000)       10 2023-10-05 00:53:38.000000 doot-0.7.0/doot/utils/__init__.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-15 22:34:36.949531 doot-0.7.0/doot/utils/__tests/
+-rw-rw-r--   0 john      (1000) john      (1000)     6581 2024-04-15 22:30:11.000000 doot-0.7.0/doot/utils/__tests/test_decorators.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1596 2024-04-15 22:30:11.000000 doot-0.7.0/doot/utils/chain_get.py
+-rw-rwxr--   0 john      (1000) john      (1000)     1180 2023-10-17 22:05:44.000000 doot-0.7.0/doot/utils/check_protocol.py
+-rw-rw-r--   0 john      (1000) john      (1000)     7141 2024-04-15 22:30:11.000000 doot-0.7.0/doot/utils/decorators.py
+-rw-rwxr--   0 john      (1000) john      (1000)     4525 2023-10-17 22:05:44.000000 doot-0.7.0/doot/utils/log_colour.py
+-rw-rw-r--   0 john      (1000) john      (1000)     5750 2024-04-15 22:30:11.000000 doot-0.7.0/doot/utils/log_config.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1881 2024-02-23 23:43:30.000000 doot-0.7.0/doot/utils/log_context.py
+-rw-rw-r--   0 john      (1000) john      (1000)     5221 2024-04-15 22:30:11.000000 doot-0.7.0/doot/utils/mock_gen.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2538 2024-04-15 22:30:11.000000 doot-0.7.0/doot/utils/plugin_selector.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1841 2024-04-15 22:30:11.000000 doot-0.7.0/doot/utils/retrievers.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1909 2024-02-23 23:43:30.000000 doot-0.7.0/doot/utils/signal_handler.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1350 2024-04-15 22:30:11.000000 doot-0.7.0/doot/utils/testing_fixtures.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1787 2024-04-15 20:38:01.000000 doot-0.7.0/doot/utils/trace_helper.py
+-rw-rwxr--   0 john      (1000) john      (1000)     1363 2023-10-17 22:05:44.000000 doot-0.7.0/doot/utils/url_expand.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-15 22:34:36.949531 doot-0.7.0/doot.egg-info/
+-rw-r--r--   0 john      (1000) john      (1000)    10267 2024-04-15 22:34:36.000000 doot-0.7.0/doot.egg-info/PKG-INFO
+-rw-rw-r--   0 john      (1000) john      (1000)     4521 2024-04-15 22:34:36.000000 doot-0.7.0/doot.egg-info/SOURCES.txt
+-rw-rw-r--   0 john      (1000) john      (1000)        1 2024-04-15 22:34:36.000000 doot-0.7.0/doot.egg-info/dependency_links.txt
+-rw-rw-r--   0 john      (1000) john      (1000)       44 2024-04-15 22:34:36.000000 doot-0.7.0/doot.egg-info/entry_points.txt
+-rw-rw-r--   0 john      (1000) john      (1000)      197 2024-04-15 22:34:36.000000 doot-0.7.0/doot.egg-info/requires.txt
+-rw-rw-r--   0 john      (1000) john      (1000)        5 2024-04-15 22:34:36.000000 doot-0.7.0/doot.egg-info/top_level.txt
+-rw-rw-r--   0 john      (1000) john      (1000)     2505 2024-04-15 22:32:56.000000 doot-0.7.0/pyproject.toml
+-rw-rw-r--   0 john      (1000) john      (1000)       38 2024-04-15 22:34:36.949531 doot-0.7.0/setup.cfg
```

### Comparing `doot-0.6.1/LICENSE` & `doot-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `doot-0.6.1/PKG-INFO` & `doot-0.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doot
-Version: 0.6.1
+Version: 0.7.0
 Summary: An opinionated, TOML based task runner
 Author-email: jgrey <jgrey.n.plus.one@gmail.com>
 License:  ACAB License © 2022-12-09 John Grey
         
         
         To the maximum extent applicable by law, and any licenses of components of this work:
         
@@ -55,24 +55,27 @@
 Requires-Dist: networkx>3.0
 Requires-Dist: sh>=2.0.6
 Requires-Dist: stackprinter>=0.2.10
 Requires-Dist: matplotlib
 Requires-Dist: sty
 Requires-Dist: boltons
 Requires-Dist: more_itertools
+Requires-Dist: decorator-validation>=3.0.0
+Requires-Dist: decorator>=5.0.0
+Requires-Dist: jgdv
 Provides-Extra: test
 Requires-Dist: pytest<5.0.0; extra == "test"
 Requires-Dist: pytest-mock; extra == "test"
 Provides-Extra: dev
 Requires-Dist: pipreqs; extra == "dev"
 Requires-Dist: sphinx; extra == "dev"
 
 ![doot](https://github.com/jgrey4296/doot/assets/5943270/170a5631-6175-4d92-8d66-e26aa2c2e472)
 # doot
-Version : 0.6.1  
+Version : 0.7.0  
 Author  : John Grey  
 Date    : 2022-12-09  
 
 ## Overview
 This started out as an opinionated rewrite of the [doit](https://pydoit.org/contents.html) task runner.
 For other, more mature alternatives, see [Luigi](https://github.com/spotify/luigi), and [SnakeMake](https://github.com/snakemake/snakemake)
 and, of course, [GNU Make](https://www.gnu.org/software/make/).
```

### Comparing `doot-0.6.1/README.md` & `doot-0.7.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ![doot](https://github.com/jgrey4296/doot/assets/5943270/170a5631-6175-4d92-8d66-e26aa2c2e472)
 # doot
-Version : 0.6.1  
+Version : 0.7.0  
 Author  : John Grey  
 Date    : 2022-12-09  
 
 ## Overview
 This started out as an opinionated rewrite of the [doit](https://pydoit.org/contents.html) task runner.
 For other, more mature alternatives, see [Luigi](https://github.com/spotify/luigi), and [SnakeMake](https://github.com/snakemake/snakemake)
 and, of course, [GNU Make](https://www.gnu.org/software/make/).
```

### Comparing `doot-0.6.1/doot/__main__.py` & `doot-0.7.0/doot/__main__.py`

 * *Files 27% similar despite different names*

```diff
@@ -21,101 +21,81 @@
 from uuid import UUID, uuid1
 from weakref import ref
 ##-- end imports
 
 logging         = logmod.root
 printer         = logmod.getLogger("doot._printer")
 
+from importlib.resources import files
 import sh
 import stackprinter
 import tomlguard as TG
 import doot
 from bdb import BdbQuit
 from doot.utils.log_config import DootLogConfig
 
+template_path      = files("doot.__templates")
+
 def main():
     result  = 1
-    errored = False
     overlord = None
     try:
         log_config = DootLogConfig()
         # --- Setup
         if not bool(doot.config):
             doot.setup()
 
         log_config.setup()
 
         logging.info("Called with: %s", sys.argv)
         from doot.loaders.plugin_loader import DootPluginLoader
         from doot.control.overlord import DootOverlord
         overlord  = DootOverlord(loaders={"plugin": DootPluginLoader().setup(sys.argv[:]) },
-                                 config_filenames=[doot.constants.DEFAULT_LOAD_TARGETS],
+                                 config_filenames=[doot.constants.paths.DEFAULT_LOAD_TARGETS],
                                  log_config=log_config,
                                  args=sys.argv[:])
 
         # --- Do whatever thats been triggered
         result    = overlord()
 
     ##-- handle doot errors
     except (doot.errors.DootEarlyExit, BdbQuit):
         printer.warning("Early Exit Triggered")
+        result = 0
     except doot.errors.DootMissingConfigError as err:
+        result = 0
         # Handle missing files
-        if not doot.constants.DEFAULT_LOAD_TARGETS[0].exists():
-            if input("No toml config data found, create stub doot.toml? _/n ") != "n":
-                doot.constants.DEFAULT_LOAD_TARGETS[0].write_text(doot.constants.TOML_TEMPLATE.read_text())
-                logging.info("Stubbed")
-
+        if pl.Path(doot.constants.on_fail(["doesntexist"]).paths.DEFAULT_LOAD_TARGETS()[0]).exists():
+            pass
+        elif input("No toml config data found, create stub doot.toml? _/n ") != "n":
+            template = template_path.joinpath(doot.constants.paths.TOML_TEMPLATE)
+            target = pl.Path(doot.constants.on_fail(["doot.toml"]).paths.DEFAULT_LOAD_TARGETS()[0])
+            target.write_text(template.read_text())
+            logging.info("Stubbed")
     except doot.errors.DootTaskError as err:
-        errored = True
         printer.error("%s : %s", err.general_msg, err.task_name)
         printer.error("---- Source: %s", err.task_source)
         printer.error("---- %s", str(err))
     except doot.errors.DootError as err:
-        errored = True
         printer.error("%s", err.general_msg)
         printer.error("---- %s", str(err))
     ##-- end handle doot errors
     ##-- handle todo errors
     except NotImplementedError as err:
-        errored = True
         logging.error(stackprinter.format())
         printer.error("Not Implemented: %s", err)
     ##-- end handle todo errors
     ##-- handle general errors
     except Exception as err:
-        errored = True
         logging.error(stackprinter.format())
         # logging.error("Python Error: %s", err)
     ##-- end handle general errors
     finally: # --- final shutdown
         if overlord:
             overlord.shutdown()
-        match sys.platform:
-            case "linux":
-                pass
-            case "darwin":
-                announce_exit : bool = doot.constants.ANNOUNCE_EXIT
-                announce_voice : str = doot.constants.ANNOUNCE_VOICE
-                if doot.config is not None:
-                    announce_exit        = doot.config.on_fail(announce_exit, bool|str).settings.general.notify.say_on_exit()
-                    announce_voice       = doot.config.on_fail(announce_voice, str).setttings.general.notify.announce_voice()
-
-                match errored, announce_exit:
-                    case False, str() as say_text:
-                        cmd = sh.say("-v", announce_voice, "-r", "50", say_text)
-                    case False, True:
-                        cmd = sh.say("-v", announce_voice, "-r", "50", "Doot Has Finished")
-                    case True, True|str():
-                        cmd = sh.say("-v", announce_voice, "-r", "50", "Doot Encountered a problem")
-                    case _:
-                        cmd = None
-                if cmd is not None:
-                    cmd.execute()
 
         sys.exit(result)
 
-
 ##-- ifmain
 if __name__ == '__main__':
     main()
 ##-- end ifmain
```

### Comparing `doot-0.6.1/doot/__templates/stub_task_py` & `doot-0.7.0/doot/__templates/stub_task_py`

 * *Files 4% similar despite different names*

```diff
@@ -64,13 +64,7 @@
         yield self._extra_actions[1]
 
     def _head(self, spec, state):
         printer.info("A Big number: %s", self.human_sizes(1_000_000))
 
     def _tail(self, spec, state):
         printer.info("Another Big Number: %s", self.human_sizes(50_234_235))
-
-
-"""
-
-
-"""
```

### Comparing `doot-0.6.1/doot/__tests/test_basic.py` & `doot-0.7.0/doot/__tests/test_basic.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,26 +13,27 @@
                     TypeVar, cast)
 ##-- end imports
 logging = logmod.root
 
 import pytest
 import tomlguard
 import doot
+doot._test_setup()
 
 class TestBasicDoot:
 
     def test_initial(self, mocker):
         mocker.patch.object(doot,  "config", None)
         assert(doot.config is None)
-        doot.setup()
+        doot._test_setup()
         assert(isinstance(doot.config, tomlguard.TomlGuard))
 
 
     def test_initial2(self, mocker):
         mocker.patch.object(doot,  "config", None)
         assert(doot.config is None)
-        doot.setup()
+        doot._test_setup()
         assert(isinstance(doot.config, tomlguard.TomlGuard))
 
     def test_overlord(self, mocker):
         mocker.patch
         from doot.control.overlord import DootOverlord
```

### Comparing `doot-0.6.1/doot/_abstract/__init__.py` & `doot-0.7.0/doot/_abstract/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,13 +14,13 @@
 Interfaces need to be inherited from, and their __init__ method called.
 """
 
 from .control import TaskTracker_i, TaskRunner_i
 from .loader import CommandLoader_p, PluginLoader_p, TaskLoader_p
 from .overlord import Overlord_p
 from .cmd import Command_i
-from .task import Action_p, TaskBase_i, Task_i, Job_i
+from .task import Action_p, Task_i, Job_i
 
 from .dbm import DBManager_p
 from .parser import ArgParser_i
 from .reporter import Reporter_i, ReportLine_i
 from .policy import FailPolicy_p
```

### Comparing `doot-0.6.1/doot/_abstract/control.py` & `doot-0.7.0/doot/_abstract/control.py`

 * *Files 10% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 ##-- end logging
 
 from abc import abstractmethod
 from typing import Generator, NewType
 from collections import deque, defaultdict
 
 from doot.enums import TaskStateEnum
-from doot._structs.artifact import DootTaskArtifact
-from doot._structs.task_spec import DootTaskSpec
+
 from doot._abstract.reporter import ReportLine_i, Reporter_i
 from doot._abstract.policy import FailPolicy_p
-from doot._abstract.task import TaskBase_i
+from doot._abstract.task import Task_i
+from doot._abstract.structs import ArtifactStruct_p, SpecStruct_p
 
 class TaskTracker_i:
     """
     Track tasks that have run, need to run, are running,
     and have failed.
     Does not execute anything itself
     """
@@ -62,27 +62,27 @@
         raise NotImplementedError()
 
     @abstractmethod
     def __contains__(self, target:str) -> bool:
         raise NotImplementedError()
 
     @abstractmethod
-    def add_task(self, task:DootTaskSpec|TaskBase_i):
+    def add_task(self, task:SpecStruct_p|Task_i):
         raise NotImplementedError()
 
     @abstractmethod
     def queue_task(self, task:str) -> None:
         raise NotImplementedError()
 
     @abstractmethod
-    def update_state(self, task:str|DootTaskName|DootTaskSpec|TaskBase_i|DootTaskArtifact, state:TaskStateEnum) -> None:
+    def update_state(self, task:str|DootTaskName|SpecStruct_p|Task_i|ArtifactStruct_p, state:TaskStateEnum) -> None:
         raise notimplementederror()
 
     @abstractmethod
-    def next_for(self, target:str) -> TaskBase_i|DootTaskArtifact|None:
+    def next_for(self, target:str) -> Task_i|ArtifactStruct_p|None:
         raise NotImplementedError()
 
     @abstractmethod
     def declared_set(self) -> set[str]:
         raise NotImplementedError()
 
     @abstractmethod
```

### Comparing `doot-0.6.1/doot/_abstract/dbm.py` & `doot-0.7.0/doot/_abstract/dbm.py`

 * *Files identical despite different names*

### Comparing `doot-0.6.1/doot/_abstract/loader.py` & `doot-0.7.0/doot/_abstract/loader.py`

 * *Files 10% similar despite different names*

```diff
@@ -31,15 +31,14 @@
 ##-- end logging
 
 from typing import Self
 from abc import abstractmethod
 from tomlguard import TomlGuard
 from importlib.metadata import EntryPoint
 
-from doot.structs import DootTaskSpec
 from doot._abstract.cmd import Command_i
 from doot._abstract.task import Job_i
 
 
 @runtime_checkable
 class PluginLoader_p(Protocol):
     """ Base for the first things loaded: plugins."""
@@ -85,12 +84,12 @@
     _task_class      : type
 
     @abstractmethod
     def setup(self, plugins:TomlGuard) -> Self:
         raise NotImplementedError()
 
     @abstractmethod
-    def load(self) -> TomlGuard[DootTaskSpec]:
+    def load(self) -> TomlGuard:
         raise NotImplementedError()
 
 
 Loaders_p : TypeAlias = CommandLoader_p | PluginLoader_p | TaskLoader_p
```

### Comparing `doot-0.6.1/doot/_abstract/overlord.py` & `doot-0.7.0/doot/_abstract/overlord.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,19 +3,18 @@
 """
 from __future__ import annotations
 import pathlib as pl
 from abc import abstractmethod
 from typing import NewType, Any
 
 from tomlguard import TomlGuard
-from doot._abstract.parser import ParamSpecMaker_m
 from doot._abstract.loader import Loaders_p
 
 
-class Overlord_p(ParamSpecMaker_m):
+class Overlord_p:
     """
     Main entrypoint for doot
     """
 
     @staticmethod
     def print_version() -> str:
         raise NotImplementedError()
@@ -24,15 +23,15 @@
     def __init__(self, *, loaders:dict[str, Loaders_p]|None=None,
                configs:tuple[pl.Path|str]=('doot.toml', 'pyproject.toml'),
                extra_config:dict[str,Any]|TomlGuard|None=None,
                args:list[str]|None=None):
         raise NotImplementedError()
 
 
-    def __call__(self, cmd:str|None=None) -> None:
+    def __call__(self, cmd:str|None=None) -> int:
         """entry point for all commands
 
         :param all_args: list of string arguments from command line
 
         return codes:
           0: tasks executed successfully
           1: one or more tasks failed
@@ -41,8 +40,8 @@
              in this case the Reporter is not used.
              So be aware if you expect a different formatting (like JSON)
              from the Reporter.
         """
         raise NotImplementedError()
 
     def shutdown(self) -> None:
-        raise NotImplementedError
+        raise NotImplementedError()
```

### Comparing `doot-0.6.1/doot/_abstract/parser.py` & `doot-0.7.0/doot/_abstract/parser.py`

 * *Files 12% similar despite different names*

```diff
@@ -28,46 +28,39 @@
 
 ##-- logging
 logging = logmod.getLogger(__name__)
 ##-- end logging
 
 from abc import abstractmethod
 from tomlguard import TomlGuard
-from doot.structs import DootParamSpec
 
+from doot._abstract.structs import ParamStruct_p
 
 @dataclass
 class _RegexEqual(str):
     """ https://martinheinz.dev/blog/78 """
     string : str
     match :  re.Match = None
 
     def __eq__(self, pattern):
         self.match = re.search(pattern, self.string)
         return self.match is not None
 
     def __getitem__(self, group):
         return self.match[group]
 
-class ParamSpecMaker_m:
-
-    @staticmethod
-    def make_param(*args:Any, **kwargs:Any) -> DootParamSpec:
-        """ Utility method for easily making paramspecs """
-        return DootParamSpec(*args, **kwargs)
-
 class ArgParser_i:
     """
     A Single standard process point for turning the list of passed in args,
     into a dict, into a tomlguard,
     along the way it determines the cmds and tasks that have been chosne
     """
 
     def __init__(self):
         self.specs = []
 
     def add_param_specs(self, specs:list):
         self.specs += specs
 
     @abstractmethod
-    def parse(self, args:list[str], doot_arg_specs:list[DootParamSpec], cmds:TomlGuard, tasks:TomlGuard) -> TomlGuard:
+    def parse(self, args:list[str], doot_arg_specs:list[ParamStruct_p], cmds:TomlGuard, tasks:TomlGuard) -> TomlGuard:
         raise NotImplementedError()
```

### Comparing `doot-0.6.1/doot/_abstract/policy.py` & `doot-0.7.0/doot/_abstract/policy.py`

 * *Files identical despite different names*

### Comparing `doot-0.6.1/doot/_abstract/reporter.py` & `doot-0.7.0/doot/_abstract/reporter.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 ##-- logging
 logging = logmod.getLogger(__name__)
 ##-- end logging
 
 from tomlguard import TomlGuard
 from doot.enums import ReportEnum
-from doot.structs import DootTraceRecord
+from doot._structs.trace import DootTraceRecord
 
 class Reporter_i:
     """
       Holds ReportLine_i's, and stores DootTraceRecords
     """
 
     def __init__(self, reporters:list[ReportLine_i]=None):
@@ -45,15 +45,15 @@
 
     def _default_formatter(self, trace:DootTraceRecord) -> str:
         return str(trace)
 
     def __str__(self):
         raise NotImplementedError()
 
-    def trace(self, msg, *args, flags=None):
+    def add_trace(self, msg, *args, flags=None):
         self._full_trace.append(DootTraceRecord(msg, flags, args))
 
 
 class ReportLine_i:
     """
     Reporters, like loggers, are stacked, and each takes the flags and data and maybe runs.
     """
```

### Comparing `doot-0.6.1/doot/_abstract/task.py` & `doot-0.7.0/doot/task/base_task.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,107 +1,87 @@
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
-
+#!/usr/bin/env python3
 """
+"""
+##-- imports
 from __future__ import annotations
 
-import logging as logmod
-import abc
 import types
-from typing import Generator, NewType, Protocol, Any, runtime_checkable
-
-from tomlguard import TomlGuard
-import doot.errors
-
-from doot.enums import TaskFlags, TaskStateEnum, ActionResponseEnum
-from doot._abstract.parser import ParamSpecMaker_m
-from doot.structs import DootParamSpec, TaskStub, DootTaskSpec, DootTaskName, DootActionSpec
+import abc
+import datetime
+import enum
+import functools as ftz
+import itertools as itz
+import logging as logmod
+import pathlib as pl
+import re
+import time
+from copy import deepcopy
+from dataclasses import InitVar, dataclass, field
+from typing import (TYPE_CHECKING, Any, Callable, ClassVar, Final, Generic,
+                    Iterable, Iterator, Mapping, Match, MutableMapping,
+                    Protocol, Sequence, Tuple, TypeAlias, TypeGuard, TypeVar,
+                    cast, final, overload, runtime_checkable)
+from uuid import UUID, uuid1
+from weakref import ref
 
+##-- end imports
 
 ##-- logging
 logging = logmod.getLogger(__name__)
 ##-- end logging
 
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
+printer = logmod.getLogger("doot._printer")
 
+import doot
+import doot.errors
+import tomlguard
+from doot._abstract import Task_i, Job_i, Action_p, PluginLoader_p
+from doot.enums import TaskFlags, TaskStateEnum
+from doot.structs import TaskStub, TaskStubPart, DootActionSpec, DootCodeReference, DootTaskName
+from doot.actions.base_action import DootBaseAction
+from doot.errors import DootTaskLoadError, DootTaskError
+
+from doot.mixins.param_spec import ParamSpecMaker_m
+from doot.mixins.importer import Importer_m
+
+TASK_ALISES     = doot.aliases.task
+PRINT_LOCATIONS = doot.constants.printer.PRINT_LOCATIONS
+STATE_TASK_NAME_K : Final[str] = doot.constants.patterns.STATE_TASK_NAME_K
 
-class TaskBase_i(ParamSpecMaker_m):
-    """ Core Interface for Tasks """
-
-    _version         : str       = "0.1"
-    _help            : list[str] = []
+class _TaskProperties_m(ParamSpecMaker_m):
 
     @classmethod
     @property
     def param_specs(cls) -> list[DootParamSpec]:
         """  make class parameter specs  """
         return [
-            cls.make_param(name="help", default=False, invisible=True, prefix="--"),
-            cls.make_param(name="debug", default=False, invisible=True, prefix="--"),
-            cls.make_param(name="verbose", default=0, type=int, invisible=True, prefix="--")
+            cls.build_param(name="help", default=False, invisible=True, prefix="--"),
+            cls.build_param(name="debug", default=False, invisible=True, prefix="--"),
+            cls.build_param(name="verbose", default=0, type=int, invisible=True, prefix="--")
            ]
 
-    def __init__(self, spec:DootTaskSpec):
-        self.spec       : DootTaskSpec        = spec
-        self.status     : TaskStateEnum       = TaskStateEnum.WAIT
-        self.flags      : TaskFlags           = TaskFlags.JOB
-        self._records   : list[Any]           = []
-        self.state                            = dict(spec.extra)
-        self.state['_task_name']              = self.spec.name
-        self.state['_action_step']            = 0
+    @property
+    def readable_name(self) -> str:
+        return str(self.spec.name.readable)
+
+    @property
+    def actions(self):
+        """lazy creation of action instances,
+          `prepare_actions` has already ensured all ctors can be found
+        """
+        yield from iter(self.spec.actions)
 
     @property
     def name(self) -> str:
         return str(self.spec.name)
 
     @property
     def fullname(self) -> DootTaskName:
         return self.spec.name
 
-    def __hash__(self):
-        return hash(self.name)
-
-    def __lt__(self, other:TaskBase_i) -> bool:
-        """ Task A < Task B iff A ∈ B.run_after   """
-        return (other.name in self.spec.after_artifacts
-                or other.name in self.spec.depends_on)
-
-    def __eq__(self, other):
-        match other:
-            case str():
-                return self.name == other
-            case TaskBase_i():
-                return self.name == other.name
-            case _:
-                return False
-
     @property
     def short_doc(self) -> str:
         """ Generate Job Class 1 line help string """
         try:
             split_doc = [x for x in self.__class__.__doc__.split("\n") if bool(x)]
             return ":: " + split_doc[0].strip() if bool(split_doc) else ""
         except AttributeError:
@@ -140,107 +120,114 @@
                 lines += msg[0]()
             case list():
                 lines += msg
 
         for line in lines:
             logging.log(level, prefix + str(line))
 
-    @classmethod
-    @abc.abstractmethod
-    def class_help(cls) -> str:
-        raise NotImplementedError(cls, "help")
-
-    @classmethod
-    @abc.abstractmethod
-    def stub_class(cls, TaskStub):
-        """
-        Specialize a TaskStub to describe this class
-        """
-        raise NotImplementedError(cls, "stub_class")
+    @property
+    def is_stale(self):
+        return False
 
-    @abc.abstractmethod
-    def stub_instance(self, TaskStub):
-        """
-          Specialize a TaskStub with the settings of this specific instance
-        """
-        raise NotImplementedError(self.__class__, "stub_instance")
+    def __hash__(self):
+        return hash(self.name)
 
-    @property
-    @abc.abstractmethod
-    def is_stale(self) -> bool:
-        """ Query whether the task's artifacts have become stale and need to be rebuilt"""
-        raise NotImplementedError()
+    def __lt__(self, other:Task_i) -> bool:
+        """ Task A < Task B iff A ∈ B.run_after   """
+        return (other.name in self.spec.after_artifacts
+                or other.name in self.spec.depends_on)
 
-class Task_i(TaskBase_i):
-    """
-    holds task information and state, produces actions to execute.
+    def __eq__(self, other):
+        match other:
+            case str():
+                return self.name == other
+            case Task_i():
+                return self.name == other.name
+            case _:
+                return False
 
+@doot.check_protocol
+class DootTask(_TaskProperties_m, Importer_m, Task_i):
     """
+      The simplest task, which can import action classes.
+      eg:
+      actions = [ {do = "doot.actions.shell_action:DootShellAction", args = ["echo", "this is a test"] } ]
+    """
+    action_ctor    = DootBaseAction
+    _default_flags = TaskFlags.TASK
+    _help          = ["The Simplest Task"]
 
-    def __init__(self, spec:DootTaskSpec, *, job:Job_i=None, **kwargs):
-        super().__init__(spec)
-        self.job     = job
+    def __init__(self, spec, *, job=None, action_ctor=None, **kwargs):
+        self.spec       : SpecStruct_p        = spec
+        self.status     : TaskStateEnum       = TaskStateEnum.WAIT
+        self.flags      : TaskFlags           = TaskFlags.JOB
+        self._records   : list[Any]           = []
+        self.state                            = dict(spec.extra)
+        self.job                              = job
+        self.state[STATE_TASK_NAME_K]         = self.spec.name
+        self.state['_action_step']            = 0
+        self.action_ctor                      = action_ctor
+        self.prepare_actions()
 
     def __repr__(self):
         return f"<Task: {self.name}>"
 
-    def maybe_more_tasks(self) -> Generator[Task_i]:
-        return iter([])
-
     @classmethod
     def class_help(cls):
         """ Task *class* help. """
         help_lines = [f"Task   : {cls.__qualname__} v{cls._version}", ""]
         mro = " -> ".join(x.__name__ for x in cls.mro())
         help_lines.append(f"Task MRO: {mro}")
         help_lines.append("")
         help_lines += cls._help
 
         return "\n".join(help_lines)
 
-    @property
-    @abc.abstractmethod
-    def actions(self) -> Generator[Action_p]:
-        """lazy creation of action instances"""
-        raise NotImplementedError()
-
-class Job_i(TaskBase_i):
-    """
-    builds task descriptions, produces no actions
-    """
-
-    def __init__(self, spec:DootTaskSpec):
-        super().__init__(spec)
-        self.args       : dict                 = {}
-
     @classmethod
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
+    def stub_class(cls, stub) -> TaskStub:
+        """ Create a basic toml stub for this task"""
+        if bool(list(filter(lambda x: x[0] == "task", TASK_ALISES))):
+            stub.ctor = "task"
+        else:
+            stub.ctor                   = cls
+
+        # Come first
+        stub['active_when'].priority    = -90
+        stub['required_for'].priority   = -90
+        stub['depends_on'].priority     = -100
+
+        stub['print_levels'].type       = f"Dict: {PRINT_LOCATIONS}"
+        stub['print_levels'].default    = {"head":"INFO","build":"INFO","sleep":"INFO","action":"INFO", "execute":"INFO"}
+
+        stub['priority'].default        = 10
+        stub['queue_behaviour'].default = "default"
+        stub['queue_behaviour'].comment = "default | auto | reactive"
+        return stub
+
+    def stub_instance(self, stub) -> TaskStub:
+        """ extend the class toml stub with details from this instance """
+        stub['name'].default      = self.fullname
+        if bool(self.doc):
+            stub['doc'].default   = self.doc[:]
+        stub['flags'].default     = self.spec.flags
+
+        return stub
+
+    def prepare_actions(self):
+        """ if the task/action spec requires particular action ctors, load them.
+          if the action spec doesn't have a ctor, use the task's action_ctor
+        """
+        logging.info("Preparing Actions: %s", self.name)
+        for group in self.spec.action_groups:
+            for action_spec in group:
+                match action_spec:
+                    case DootTaskName():
+                        pass
+                    case DootActionSpec() if action_spec.fun is not None:
+                        pass
+                    case DootActionSpec() if action_spec.do is not None:
+                        action_ref = self.import_callable(action_spec.do)
+                        action_spec.set_function(action_ref)
+                    case DootActionSpec():
+                        action_spec.set_function(self.action_ctor)
+                    case _:
+                        raise doot.errors.DootTaskError("Unknown element in action group: ", action_spec)
```

### Comparing `doot-0.6.1/doot/_structs/__tests/test_action_spec.py` & `doot-0.7.0/doot/actions/__tests/test_control_flow.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,38 +5,49 @@
 from __future__ import annotations
 
 import logging as logmod
 import pathlib as pl
 from typing import (Any, Callable, ClassVar, Generic, Iterable, Iterator,
                     Mapping, Match, MutableMapping, Sequence, Tuple, TypeAlias,
                     TypeVar, cast)
+from dataclasses import fields
 import warnings
+import os
 
-import pytest
 logging = logmod.root
 
-import tomlguard
-from doot import structs
-import doot.constants
+import pytest
+
+import doot
+doot._test_setup()
+
+import doot._abstract
+import doot.structs
+from doot.task.base_task import DootTask
+from doot.actions.base_action import DootBaseAction
 
+##-- pytest reminder
 # caplog
 # mocker.patch | patch.object | patch.multiple | patch.dict | stopall | stop | spy | stub
 # pytest.mark.filterwarnings
 # pytest.parameterize
 # pytest.skip | skipif | xfail
 # with pytest.deprecated_call
 # with pytest.raises
 # with pytest.warns(warntype)
 
-class TestActionSpec:
-
-    def test_initial(self):
-        obj = structs.DootActionSpec()
-        assert(isinstance(obj, structs.DootActionSpec))
+##-- end pytest reminder
 
+class TestBaseAction:
 
-    def test_call(self, mocker):
-        fun_mock = mocker.Mock()
-        obj = structs.DootActionSpec(fun=fun_mock)
+    def test_initial(self):
+        action = DootBaseAction()
+        assert(isinstance(action, DootBaseAction))
 
-        obj({})
-        fun_mock.assert_called_once()
+    def test_call_action(self, caplog, mocker):
+        action = DootBaseAction()
+        state  = { "count" : 0  }
+        spec   = mocker.Mock(spec=doot.structs.DootActionSpec)
+        spec.args = []
+        result = action(spec, state)
+        assert(result['count'] == 1)
+        assert("Base Action Called: 0" in caplog.messages)
```

### Comparing `doot-0.6.1/doot/_structs/__tests/test_formatter.py` & `doot-0.7.0/doot/_structs/__tests/test_formatter.py`

 * *Files 9% similar despite different names*

```diff
@@ -25,69 +25,77 @@
 # with pytest.raises
 # with pytest.warns(warntype)
 
 ##-- end pytest reminder
 
 from tomlguard import TomlGuard
 import doot
+doot._test_setup()
+
 from doot.structs import DootActionSpec
 from doot._structs.key import DootFormatter
 
 class TestDootFormatter:
 
     @pytest.fixture(scope="function")
     def setup_locs(self, mocker):
         new_locs = TomlGuard({"p1": "test1", "p2": "test2/sub"})
         return mocker.patch.object(doot.locs, "_data", new_locs)
 
     def test_initial(self, mocker):
         fmt = DootFormatter()
-        spec = mocker.Mock(kwargs={"a":"blah"}, spec=DootActionSpec)
+        spec = mocker.Mock(params={"a":"blah"}, spec=DootActionSpec)
         result = fmt.format("{a}", _spec=spec, _state={})
         assert(result == "blah")
 
     def test_missing(self, mocker):
         fmt = DootFormatter()
-        spec = mocker.Mock(kwargs={"a":"blah"}, spec=DootActionSpec)
+        spec = mocker.Mock(params={"a":"blah"}, spec=DootActionSpec)
         result = fmt.format("{b}", _spec=spec, _state={})
         assert(result == "{b}")
 
 
     def test_multi(self, mocker):
         fmt = DootFormatter()
-        spec = mocker.Mock(kwargs={"a":"blah"}, spec=DootActionSpec)
+        spec = mocker.Mock(params={"a":"blah"}, spec=DootActionSpec)
         state = {"b": "aweg"}
         result = fmt.format("{a}:{b}", _spec=spec, _state=state)
         assert(result == "blah:aweg")
 
 
     def test_indirect(self, mocker):
         fmt = DootFormatter()
-        spec = mocker.Mock(kwargs={"a":"blah"}, spec=DootActionSpec)
+        spec = mocker.Mock(params={"a":"blah"}, spec=DootActionSpec)
         state = {"b": "aweg"}
         result = fmt.format("{a}", _spec=spec, _state=state)
         assert(result == "blah")
 
 
     def test_recursive(self, mocker):
         fmt = DootFormatter()
-        spec = mocker.Mock(kwargs={"a":"this is a {b}"}, spec=DootActionSpec)
+        spec = mocker.Mock(params={"a":"this is a {b}"}, spec=DootActionSpec)
         state = {"b": "aweg {c}", "c": "blah"}
         result = fmt.format("{a}", _spec=spec, _state=state, _rec=True)
         assert(result == "this is a aweg blah")
 
 
     def test_recursive_missing(self, mocker):
         fmt = DootFormatter()
-        spec = mocker.Mock(kwargs={"a":"this is a {b}"}, spec=DootActionSpec)
+        spec = mocker.Mock(params={"a":"this is a {b}"}, spec=DootActionSpec)
         state = {"b": "aweg {c}", "c": "blah {d}"}
         result = fmt.format("{a}", _spec=spec, _state=state, _rec=True)
         assert(result == "this is a aweg blah {d}")
 
 
     @pytest.mark.xfail
     def test_not_str_fails(self, mocker):
         fmt = DootFormatter()
-        spec = mocker.Mock(kwargs={"a":"this is a {b}"}, spec=DootActionSpec)
+        spec = mocker.Mock(params={"a":"this is a {b}"}, spec=DootActionSpec)
         state = {"b": "aweg {c}", "c": [1,2,3]}
         with pytest.raises(TypeError):
             fmt.format("{a}", _spec=spec, _state=state, _rec=True)
+
+
+    def test_empty_format(self):
+        fmt = DootFormatter()
+        result = fmt.format(".")
+        assert(result == ".")
```

### Comparing `doot-0.6.1/doot/_structs/__tests/test_param_spec.py` & `doot-0.7.0/doot/_structs/__tests/test_param_spec.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,193 +11,195 @@
 from typing import (Any, Callable, ClassVar, Generic, Iterable, Iterator,
                     Mapping, Match, MutableMapping, Sequence, Tuple, TypeAlias,
                     TypeVar, cast)
 ##-- end imports
 logging = logmod.root
 
 import pytest
+import doot
+doot._test_setup()
 import doot.errors
 from doot.structs import DootParamSpec, DootTaskSpec
 
 class TestParamSpec:
 
     def test_paramspec(self):
-        example = DootParamSpec.from_dict({
+        example = DootParamSpec.build({
             "name" : "test"
           })
         assert(isinstance(example, DootParamSpec))
 
     def test_equal(self):
-        example = DootParamSpec.from_dict({
+        example = DootParamSpec.build({
             "name" : "test"
           })
         assert(example == "test")
         assert(example == "test=blah")
         assert(example == "-test")
         assert(example == "-test=blah")
         assert(example == "-t")
         assert(example == "-t=blah")
 
     def test_equal_fail(self):
-        example = DootParamSpec.from_dict({
+        example = DootParamSpec.build({
             "name" : "test"
           })
         assert(example != "atest")
         assert(example != "--test")
         assert(example != "-tw")
 
     def test_consume_bool(self):
-        example = DootParamSpec.from_dict({
+        example = DootParamSpec.build({
             "name" : "test",
             "type" : "bool",
           })
         assert(example == "test")
         data = {}
         example.maybe_consume(["-test"], data)
         assert('test' in data)
         assert(bool(data['test']))
 
     def test_consume_short_bool(self):
-        example = DootParamSpec.from_dict({
+        example = DootParamSpec.build({
             "name" : "test"
           })
         assert(example == "test")
         data = {}
         example.maybe_consume(["-t"], data)
         assert('test' in data)
         assert(bool(data['test']))
 
     def test_fail_on_assign_wrong_prefix(self):
-        example = DootParamSpec.from_dict({
+        example = DootParamSpec.build({
             "name" : "test"
           })
         assert(example == "test")
         with pytest.raises(doot.errors.DootParseError):
             example.maybe_consume(["-t=blah"], {})
 
     def test_consume_inverse_bool(self):
-        example = DootParamSpec.from_dict({
+        example = DootParamSpec.build({
             "name" : "test"
           })
         assert(example == "test")
         data = {}
         example.maybe_consume(["-no-test"], data)
         assert('test' in data)
         assert(not bool(data['test']))
 
     def test_consume_list(self):
-        example = DootParamSpec.from_dict({
+        example = DootParamSpec.build({
             "name" : "test",
             "type" : list,
             "default" : [],
           })
         assert(example == "test")
         data = {'test': []}
         example.maybe_consume(["-test", "bloo"], data)
         assert('test' in data)
         assert(data['test'] == ["bloo"])
 
     def test_consume_list_multi(self):
-        example = DootParamSpec.from_dict({
+        example = DootParamSpec.build({
             "name" : "test",
             "type" : list,
             "default" : [],
             "positional": True
           })
         assert(example == "test")
         data = {'test': []}
         example.maybe_consume(["bloo", "blah"], data)
         assert('test' in data)
         assert(data['test'] == ["bloo", "blah"])
 
     @pytest.mark.xfail
     def test_consume_list_multi_joined(self):
-        example = DootParamSpec.from_dict({
+        example = DootParamSpec.build({
             "name" : "test",
             "type" : list,
             "default" : [],
           })
         assert(example == "test")
         data = {'test': []}
         args = ["-test", "bloo", "-test", "blah"]
         example.maybe_consume(args, data)
         example.maybe_consume(args, data)
         assert('test' in data)
         assert(data['test'] == ["bloo", "blah"])
 
     @pytest.mark.xfail
     def test_consume_set_multi_joined(self):
-        example = DootParamSpec.from_dict({
+        example = DootParamSpec.build({
             "name"    : "test",
             "type"    : set,
             "default" : set(),
           })
         assert(example == "test")
         data = {'test': set()}
         example.maybe_consume(["-test", "bloo"], data)
         example.maybe_consume(["-test", "bloo"], data)
         example.maybe_consume(["-test", "blah"], data)
         assert('test' in data)
         assert(data['test'] == {"bloo", "blah"})
 
     def test_consume_str(self):
-        example = DootParamSpec.from_dict({
+        example = DootParamSpec.build({
             "name" : "test",
             "type" : str,
             "default" : "",
           })
         assert(example == "test")
         data = {}
         example.maybe_consume(["-test", "bloo,blah"], data)
         assert('test' in data)
         assert(data['test'] == "bloo,blah")
 
     def test_consume_str_multi_set_fail(self):
-        example = DootParamSpec.from_dict({
+        example = DootParamSpec.build({
             "name" : "test",
             "type" : str,
             "default" : "",
           })
         assert(example == "test")
         data = {} # <---
         example.maybe_consume(["-test", "bloo", "blah"], data)
         with pytest.raises(Exception):
             example.maybe_consume(data, "-test=aweg")
 
     def test_consume_custom_value(self):
-        example = DootParamSpec.from_dict({
+        example = DootParamSpec.build({
             "name" : "test",
             "type" : lambda x: int(x) + 2,
             "default" : 5,
           })
         assert(example == "test")
         data = {} # <---
         example.maybe_consume(["-test", "2"], data)
         assert(example == "test")
         assert(data['test'] == 4)
 
     def test_positional(self):
-        example = DootParamSpec.from_dict({
+        example = DootParamSpec.build({
             "name" : "test",
             "type" : list,
             "default" : [1,2,3],
             "positional" : True
             })
         assert(example.positional is True)
 
     def test_invisible_str(self):
-        example = DootParamSpec.from_dict({
+        example = DootParamSpec.build({
             "name" : "test",
             "type" : list,
             "default" : [1,2,3],
             "invisible" : True,
             })
         assert(str(example) == "")
 
     def test_not_invisible_str(self):
-        example = DootParamSpec.from_dict({
+        example = DootParamSpec.build({
             "name" : "test",
             "type" : list,
             "default" : [1,2,3],
             "invisible" : False,
             })
         assert(str(example) != "")
```

### Comparing `doot-0.6.1/doot/_structs/__tests/test_sname.py` & `doot-0.7.0/doot/_structs/__tests/test_task_name.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,36 +11,35 @@
                     TypeVar, cast)
 import warnings
 
 import pytest
 logging = logmod.root
 
 import tomlguard
+import doot
+doot._test_setup()
 from doot import structs
-import doot.constants
+from doot.enums import TaskFlags
 from doot.task.base_task import DootTask
 
 class TestDootTaskName:
 
-    @pytest.fixture(scope="function")
-    def setup(self):
-        pass
-
-    @pytest.fixture(scope="function")
-    def cleanup(self):
-        yield
-        pass
-
-    def test_complex_name(self):
+    def test_creation(self):
         simple = structs.DootTaskName("basic", "tail")
         assert(simple.head == [ "basic"])
         assert(simple.tail == ["tail"])
 
+
+    def test_build(self):
+        simple = structs.DootTaskName.build("basic::tail")
+        assert(simple.head == [ "basic"])
+        assert(simple.tail == ["tail"])
+
     def test_name_with_leading_tasks(self):
-        simple = structs.DootTaskName.from_str("tasks.basic::tail")
+        simple = structs.DootTaskName.build("tasks.basic::tail")
         assert(simple.head == [ "basic"])
         assert(simple.tail == ["tail"])
 
     def test_cn_with_subgroups_str(self):
         simple = structs.DootTaskName("basic.blah.bloo", "tail")
         assert(simple.head == [ "basic", "blah", "bloo"])
         assert(simple.tail == ["tail"])
@@ -56,54 +55,14 @@
         assert(simple.tail == ["tail", "blah", "bloo"])
 
     def test_cn_with_mixed_subtasks(self):
         simple = structs.DootTaskName("basic", ["tail", "blah.bloo"])
         assert(simple.head == [ "basic"])
         assert(simple.tail == ["tail", "blah", "bloo"])
 
-    def test_cn_comparison(self):
-        simple = structs.DootTaskName("basic", "tail")
-        simple2 = structs.DootTaskName("basic", "tail")
-        assert(simple is not simple2)
-        assert(simple == simple2)
-
-    def test_cn_comparison_fail(self):
-        simple = structs.DootTaskName("basic", "tail")
-        simple2 = structs.DootTaskName("basic", "bloo")
-        assert(simple is not simple2)
-        assert(simple != simple2)
-
-    def test_cn_comparison_subgroups(self):
-        """ where the names have subgrouping """
-        simple  = structs.DootTaskName(["basic", "blah"], "tail")
-        simple2 = structs.DootTaskName(["basic", "blah"], "tail")
-        assert(simple is not simple2)
-        assert(simple == simple2)
-
-    def test_cn_comparison_subgroup_fail(self):
-        """ where the names only differ in subgrouping """
-        simple = structs.DootTaskName(["basic", "blah"], "tail")
-        simple2 = structs.DootTaskName(["basic", "bloo"], "tail")
-        assert(simple is not simple2)
-        assert(simple != simple2)
-
-    def test_cn_comparison_subtasks(self):
-        """ where the names have subtasks"""
-        simple = structs.DootTaskName(["basic", "blah"], "tail")
-        simple2 = structs.DootTaskName(["basic", "blah"], "tail")
-        assert(simple is not simple2)
-        assert(simple == simple2)
-
-    def test_cn_comparison_subtask_fail(self):
-        """ where the names have different subtasks"""
-        simple = structs.DootTaskName(["basic", "blah"], "tail")
-        simple2 = structs.DootTaskName(["basic", "bloo"], "tail")
-        assert(simple is not simple2)
-        assert(simple != simple2)
-
     def test_complex_name_with_dots(self):
         simple = structs.DootTaskName("basic.blah", "tail.bloo")
         assert(simple.head == ["basic", "blah"])
         assert(simple.tail == ["tail", "bloo"])
 
     def test_cn_to_str(self):
         simple = structs.DootTaskName("basic", "tail")
@@ -139,27 +98,89 @@
     def test_specialize_name(self):
         simple = structs.DootTaskName(["basic"], "tail")
         assert(str(simple) == "basic::tail")
         sub    = simple.specialize()
         assert(sub.group == "basic")
         assert(len(sub.tail) == 3)
         assert(sub.tail[0] == "tail")
-        assert(sub.tail[1] == doot.constants.SPECIALIZED_ADD)
+        assert(sub.tail[1] == doot.constants.patterns.SPECIALIZED_ADD)
 
 
     def test_specialize_name_with_info(self):
         simple = structs.DootTaskName(["basic"], "tail")
         assert(str(simple) == "basic::tail")
         sub    = simple.specialize(info="blah")
         assert(sub.group == "basic")
         assert(len(sub.tail) == 4)
         assert(sub.tail[0] == "tail")
-        assert(sub.tail[1] == doot.constants.SPECIALIZED_ADD)
+        assert(sub.tail[1] == doot.constants.patterns.SPECIALIZED_ADD)
         assert(sub.tail[2] == "blah")
 
+    def test_subtask_0(self):
+        simple = structs.DootTaskName(["basic", "sub", "test"], "tail")
+        sub = simple.subtask(0)
+        assert(sub.tail == ["tail", 0])
+        assert(str(sub) == '"basic.sub.test"::tail.0')
+
+
+    def test_subtask_1(self):
+        simple = structs.DootTaskName(["basic", "sub", "test"], "tail")
+        sub = simple.subtask(1)
+        assert(sub.tail == ["tail", 1])
+        assert(str(sub) == '"basic.sub.test"::tail.1')
+
+
+    def test_internal(self):
+        simple = structs.DootTaskName.build("agroup::_internal.task")
+        assert(TaskFlags.INTERNAL in simple.meta)
+
+
+class TestTaskNameComparison:
+
+    def test_comparison(self):
+        simple = structs.DootTaskName("basic", "tail")
+        simple2 = structs.DootTaskName("basic", "tail")
+        assert(simple is not simple2)
+        assert(simple == simple2)
+
+    def test_comparison_fail(self):
+        simple = structs.DootTaskName("basic", "tail")
+        simple2 = structs.DootTaskName("basic", "bloo")
+        assert(simple is not simple2)
+        assert(simple != simple2)
+
+    def test_comparison_subgroups(self):
+        """ where the names have subgrouping """
+        simple  = structs.DootTaskName(["basic", "blah"], "tail")
+        simple2 = structs.DootTaskName(["basic", "blah"], "tail")
+        assert(simple is not simple2)
+        assert(simple == simple2)
+
+    def test_comparison_subgroup_fail(self):
+        """ where the names only differ in subgrouping """
+        simple = structs.DootTaskName(["basic", "blah"], "tail")
+        simple2 = structs.DootTaskName(["basic", "bloo"], "tail")
+        assert(simple is not simple2)
+        assert(simple != simple2)
+
+    def test_comparison_subtasks(self):
+        """ where the names have subtasks"""
+        simple = structs.DootTaskName(["basic", "blah"], "tail")
+        simple2 = structs.DootTaskName(["basic", "blah"], "tail")
+        assert(simple is not simple2)
+        assert(simple == simple2)
+
+    def test_comparison_subtask_fail(self):
+        """ where the names have different subtasks"""
+        simple = structs.DootTaskName(["basic", "blah"], "tail")
+        simple2 = structs.DootTaskName(["basic", "bloo"], "tail")
+        assert(simple is not simple2)
+        assert(simple != simple2)
+
+
     def test_lt_comparison_equal(self):
         simple = structs.DootTaskName(["basic", "sub", "test"], "tail")
         simple2 = structs.DootTaskName(["basic", "sub", "test"], "tail")
         assert(simple < simple2)
 
     def test_lt_comparison_fail(self):
         simple = structs.DootTaskName(["basic", "sub", "test"], "tail")
@@ -177,62 +198,21 @@
         assert(simple < simple2)
 
     def test_lt_group_fail(self):
         simple = structs.DootTaskName(["basic", "sub", "test"], "tail")
         simple2 = structs.DootTaskName(["basic", "test"], ["tail", "sub"])
         assert(not (simple < simple2))
 
-
     def test_contains_basic_group(self):
         simple = structs.DootTaskName(["basic", "sub", "test"], "tail")
         assert("sub" in simple)
 
 
     def test_contains_basic_sub(self):
         simple = structs.DootTaskName(["basic", "sub", "test"], "tail")
         assert("tail" in simple)
 
 
     def test_contains_other_name(self):
         simple = structs.DootTaskName(["basic", "sub", "test"], "tail")
         sub   = structs.DootTaskName(["basic", "sub", "test"], ["tail", "sub"])
         assert(sub in simple)
-
-
-
-
-class TestDootCodeReference:
-
-    def test_basic(self):
-        ref = structs.DootCodeReference.from_str("doot.task.base_task:DootTask")
-        assert(isinstance(ref, structs.DootCodeReference))
-
-    def test_import(self):
-        ref = structs.DootCodeReference.from_str("doot.task.base_task:DootTask")
-        imported = ref.try_import()
-        assert(isinstance(imported, type))
-        assert(imported == DootTask)
-
-    def test_import_module_fail(self):
-        ref = structs.DootCodeReference.from_str("doot.taskSSSSS.base_task:DootTask")
-        with pytest.raises(ImportError):
-            imported = ref.try_import()
-
-    def test_import_class_fail(self):
-        ref = structs.DootCodeReference.from_str("doot.task.base_task:DootTaskSSSSSS")
-        with pytest.raises(ImportError):
-            imported = ref.try_import()
-
-    def test_add_mixin(self):
-        ref = structs.DootCodeReference.from_str("doot.task.base_task:DootTask")
-        assert(not bool(ref._mixins))
-        ref_plus = ref.add_mixins("doot.mixins.job.terse:TerseBuilder_M")
-        assert(ref is not ref_plus)
-        assert(not bool(ref._mixins))
-        assert(bool(ref_plus._mixins))
-
-    def test_build_mixin(self):
-        ref      = structs.DootCodeReference.from_str("doot.task.base_task:DootTask")
-        ref_plus = ref.add_mixins("doot.mixins.job.terse:TerseBuilder_M")
-        result   = ref_plus.try_import()
-        assert(result != DootTask)
-        assert(DootTask in result.mro())
```

### Comparing `doot-0.6.1/doot/_structs/__tests/test_stub.py` & `doot-0.7.0/doot/_structs/__tests/test_stub.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,33 +11,25 @@
                     TypeVar, cast)
 import warnings
 
 import pytest
 logging = logmod.root
 
 import tomlguard
+import doot
+doot._test_setup()
 from doot import structs
-import doot.constants
-
-# caplog
-# mocker.patch | patch.object | patch.multiple | patch.dict | stopall | stop | spy | stub
-# pytest.mark.filterwarnings
-# pytest.parameterize
-# pytest.skip | skipif | xfail
-# with pytest.deprecated_call
-# with pytest.raises
-# with pytest.warns(warntype)
 
 class TestTaskStub:
 
     def test_initial(self):
         obj = structs.TaskStub(dict)
         assert(isinstance(obj, structs.TaskStub))
         assert(obj.ctor == dict)
-        assert(str(obj['name'].default) == "stub::stub")
+        assert(str(obj['name'].default) == "basic::stub")
 
     def test_default_keys(self):
         """ check a stub has the default components of a TaskSpec  """
         obj = structs.TaskStub(dict)
         default_keys = set(structs.DootTaskSpec.__annotations__.keys())
         default_keys -= set(structs.TaskStub.skip_parts)
         default_keys.add("name")
@@ -59,31 +51,32 @@
 
 
     def test_toml_reparse_to_spec(self):
         """ check a stub has the default components of a TaskSpec  """
         obj    = structs.TaskStub()
         as_str = obj.to_toml()
         loaded = tomlguard.read(as_str)
-        spec   = structs.DootTaskSpec.from_dict(loaded.tasks.stub[0])
-        pass
+        spec   = structs.DootTaskSpec.build(loaded.tasks.basic[0])
+
+
 
 
 class TestTaskStubPart:
 
     def test_stub_initial(self):
         obj = structs.TaskStubPart("test", type="list", default=[1,2,3], comment="a simple stub part")
         assert(isinstance(obj, structs.TaskStubPart))
         assert(obj.key == "test")
         assert(obj.type == "list")
         assert(obj.default == [1,2,3])
         assert(obj.comment == "a simple stub part")
 
 
     def test_name_reduce(self):
-        obj = structs.TaskStubPart("name", default=structs.DootTaskName.from_str("blah::bloo"))
+        obj = structs.TaskStubPart("name", default=structs.DootTaskName.build("blah::bloo"))
         res_s = str(obj).split("\n")
         assert(res_s[0] == "[[tasks.blah]]")
         assert(res_s[1] == f"{'name':<20} = \"bloo\"")
 
 
     def test_num_reduce(self):
         obj = structs.TaskStubPart("amount", default=10, type="int")
```

### Comparing `doot-0.6.1/doot/_structs/__tests/test_task_spec.py` & `doot-0.7.0/doot/_structs/__tests/test_task_spec.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,154 +13,156 @@
 
 import pytest
 logging = logmod.root
 
 import tomlguard
 import doot
 import doot.errors
-import doot.constants
+
+doot._test_setup()
 from doot import structs
 from doot.task.base_job import DootJob
-from doot.mixins.job.terse import TerseBuilder_M
+
+DEFAULT_CTOR = doot.aliases.task[doot.constants.entrypoints.DEFAULT_TASK_CTOR_ALIAS]
 
 class TestDootTaskSpec:
 
     def test_initial(self):
-        obj = structs.DootTaskSpec.from_dict({})
+        obj = structs.DootTaskSpec.build({"name":"default::default"})
         assert(isinstance(obj, structs.DootTaskSpec))
         assert(obj.name.group == "default")
         assert(obj.name.task == "default")
-        assert(str(obj.ctor) == doot.constants.DEFAULT_PLUGINS['task'][0][1])
+        assert(str(obj.ctor) == DEFAULT_CTOR)
         assert(obj.version == "0.1")
 
     def test_version_change(self):
-        obj = structs.DootTaskSpec.from_dict({"version" : "0.5"})
+        obj = structs.DootTaskSpec.build({"version" : "0.5", "name":"default::default"})
         assert(isinstance(obj, structs.DootTaskSpec))
         assert(obj.name.group == "default")
         assert(obj.name.task == "default")
-        assert(str(obj.ctor) == doot.constants.DEFAULT_PLUGINS['task'][0][1])
+        assert(str(obj.ctor) == DEFAULT_CTOR)
         assert(obj.version == "0.5")
 
     def test_basic_name(self):
-        obj = structs.DootTaskSpec.from_dict({"name": "agroup::atask"})
+        obj = structs.DootTaskSpec.build({"name": "agroup::atask"})
         assert(isinstance(obj, structs.DootTaskSpec))
         assert(obj.name.group == "agroup")
         assert(obj.name.task == "atask")
 
     def test_groupless_name(self):
-        obj = structs.DootTaskSpec.from_dict({"name": "atask"})
+        obj = structs.DootTaskSpec.build({"name": "atask"})
         assert(isinstance(obj, structs.DootTaskSpec))
         assert(obj.name.group == "default")
         assert(obj.name.task == "atask")
 
     def test_with_extra_data(self):
-        obj = structs.DootTaskSpec.from_dict({"name": "atask", "blah": "bloo", "something": [1,2,3,4]})
+        obj = structs.DootTaskSpec.build({"name": "atask", "blah": "bloo", "something": [1,2,3,4]})
         assert(isinstance(obj, structs.DootTaskSpec))
         assert(obj.name.group == "default")
         assert(obj.name.task == "atask")
         assert("blah" in obj.extra)
         assert("something" in obj.extra)
 
     def test_separate_group_and_task(self):
-        obj = structs.DootTaskSpec.from_dict({"name": "atask", "group": "agroup"})
+        obj = structs.DootTaskSpec.build({"name": "atask", "group": "agroup"})
         assert(isinstance(obj, structs.DootTaskSpec))
         assert(obj.name.group == "agroup")
         assert(obj.name.task == "atask")
 
+@pytest.mark.skip
 class TestSpecMixinBuild:
 
     def test_basic(self):
-        spec = structs.DootTaskSpec.from_dict({"name": "basic",
-                                       "ctor": "doot.task.base_job:DootJob",
-                                       "mixins": ["doot.mixins.job.terse:TerseBuilder_M"],
-
+        spec = structs.DootTaskSpec.build({"name": "basic",
+                                           "ctor": "doot.task.base_job:DootJob",
+                                           "mixins": ["doot.mixins.job.terse:TerseBuilder_M"],
                                       })
-        task = spec.build()
+        task = spec.make()
         assert(isinstance(task,DootJob))
         assert(TerseBuilder_M in task.__class__.mro())
         assert(isinstance(task, TerseBuilder_M))
 
 
 class TestTaskSpecSpecialization:
 
     def test_specialize_from(self):
-        base_task     = structs.DootTaskSpec.from_dict({"name": "base", "group": "agroup", "extra": {"a": 0}})
-        override_task = structs.DootTaskSpec.from_dict({"name": "atask", "group": "agroup", "extra": {"b": 2},
-                                                        "ctor": structs.DootTaskName.from_str("agroup::base")})
+        base_task     = structs.DootTaskSpec.build({"name": "base", "group": "agroup", "extra": {"a": 0}})
+        override_task = structs.DootTaskSpec.build({"name": "atask", "group": "agroup", "extra": {"b": 2},
+                                                        "ctor": structs.DootTaskName.build("agroup::base")})
 
         specialized = base_task.specialize_from(override_task)
         assert(specialized is not base_task)
         assert(specialized is not override_task)
         assert("a" in specialized.extra)
         assert("b" in specialized.extra)
 
     def test_specialize_actions_from(self):
-        base_task     = structs.DootTaskSpec.from_dict({"name": "base", "group": "agroup", "extra": {"a": 0}, "actions":[{"do":"blah"}]})
-        override_task = structs.DootTaskSpec.from_dict({"name": "atask", "group": "agroup", "extra": {"b": 2},
-                                                        "ctor": structs.DootTaskName.from_str("agroup::base")})
+        base_task     = structs.DootTaskSpec.build({"name": "base", "group": "agroup", "extra": {"a": 0}, "actions":[{"do":"blah"}]})
+        override_task = structs.DootTaskSpec.build({"name": "atask", "group": "agroup", "extra": {"b": 2},
+                                                        "ctor": structs.DootTaskName.build("agroup::base")})
 
         specialized = base_task.specialize_from(override_task)
         assert(specialized is not base_task)
         assert(specialized is not override_task)
         assert(bool(specialized.actions))
 
     def test_specialize_actions_from_inverse(self):
-        base_task     = structs.DootTaskSpec.from_dict({"name": "base", "group": "agroup", "extra": {"a": 0}})
-        override_task = structs.DootTaskSpec.from_dict({"name": "atask", "group": "agroup", "extra": {"b": 2}, "actions":[{"do":"blah"}],
-                                                        "ctor": structs.DootTaskName.from_str("agroup::base")})
+        base_task     = structs.DootTaskSpec.build({"name": "base", "group": "agroup", "extra": {"a": 0}})
+        override_task = structs.DootTaskSpec.build({"name": "atask", "group": "agroup", "extra": {"b": 2}, "actions":[{"do":"blah"}],
+                                                        "ctor": structs.DootTaskName.build("agroup::base")})
 
         specialized = base_task.specialize_from(override_task)
         assert(specialized is not base_task)
         assert(specialized is not override_task)
         assert(bool(specialized.actions))
 
     def test_specialize_print_levels(self):
-        base_task     = structs.DootTaskSpec.from_dict({"name": "base", "group": "agroup", "extra": {"a": 0}, "print_levels": {"head":"DEBUG"}})
-        override_task = structs.DootTaskSpec.from_dict({"name": "atask", "group": "agroup", "extra": {"b": 2}, "print_levels": {"head":"WARNING"},
-                                                        "ctor": structs.DootTaskName.from_str("agroup::base")})
+        base_task     = structs.DootTaskSpec.build({"name": "base", "group": "agroup", "extra": {"a": 0}, "print_levels": {"head":"DEBUG"}})
+        override_task = structs.DootTaskSpec.build({"name": "atask", "group": "agroup", "extra": {"b": 2}, "print_levels": {"head":"WARNING"},
+                                                        "ctor": structs.DootTaskName.build("agroup::base")})
 
         specialized = base_task.specialize_from(override_task)
         assert(specialized is not base_task)
         assert(specialized is not override_task)
         assert(specialized.print_levels.head == "WARNING")
 
 
     def test_specialize_ctor_as_taskname(self):
-        base_task     = structs.DootTaskSpec.from_dict({"name": "base", "group": "agroup", "extra": {"a": 0}})
-        override_task = structs.DootTaskSpec.from_dict({"name": "atask",
+        base_task     = structs.DootTaskSpec.build({"name": "base", "group": "agroup", "extra": {"a": 0}})
+        override_task = structs.DootTaskSpec.build({"name": "atask",
                                                         "group": "agroup",
                                                         "extra": {"b": 2},
-                                                        "ctor" : structs.DootTaskName.from_str("agroup::base")
+                                                        "ctor" : structs.DootTaskName.build("agroup::base")
                                                        })
 
         specialized = base_task.specialize_from(override_task)
         assert(specialized is not base_task)
         assert(specialized is not override_task)
         assert(not isinstance(specialized.ctor, structs.DootTaskName))
         assert(specialized.ctor == base_task.ctor)
 
 
     def test_dependency_merge(self):
-        base_task     = structs.DootTaskSpec.from_dict({"name": "base", "group": "agroup", "extra": {"a": 0}, "depends_on": ["basic::dep"]})
-        override_task = structs.DootTaskSpec.from_dict({"name": "atask",
+        base_task     = structs.DootTaskSpec.build({"name": "base", "group": "agroup", "extra": {"a": 0}, "depends_on": ["basic::dep"]})
+        override_task = structs.DootTaskSpec.build({"name": "atask",
                                                         "group": "agroup",
                                                         "depends_on": ["extra::dep"],
                                                         "extra": {"b": 2},
-                                                        "ctor" : structs.DootTaskName.from_str("agroup::base")
+                                                        "ctor" : structs.DootTaskName.build("agroup::base")
                                                        })
 
         specialized = base_task.specialize_from(override_task)
         assert(specialized is not base_task)
         assert(specialized is not override_task)
         assert(len(specialized.depends_on) == 2)
 
 
     def test_specialize_conflict(self):
-        base_task     = structs.DootTaskSpec.from_dict({"name": "base", "group": "agroup", "extra": {"a": 0}})
-        override_task = structs.DootTaskSpec.from_dict({"name": "atask",
+        base_task     = structs.DootTaskSpec.build({"name": "base", "group": "agroup", "extra": {"a": 0}})
+        override_task = structs.DootTaskSpec.build({"name": "atask",
                                                         "group": "agroup",
                                                         "extra": {"b": 2},
-                                                        "ctor" : structs.DootTaskName.from_str("agroup::not.base")
+                                                        "ctor" : structs.DootTaskName.build("agroup::not.base")
                                                        })
 
         with pytest.raises(doot.errors.DootTaskTrackingError):
             base_task.specialize_from(override_task)
```

### Comparing `doot-0.6.1/doot/_structs/action_spec.py` & `doot-0.7.0/doot/_structs/action_spec.py`

 * *Files 2% similar despite different names*

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
@@ -33,26 +32,25 @@
 import more_itertools as mitz
 ##-- end lib imports
 
 ##-- logging
 logging = logmod.getLogger(__name__)
 ##-- end logging
 
-
 import importlib
 from tomlguard import TomlGuard
 import doot.errors
-import doot.constants
 from doot.enums import TaskFlags, ReportEnum
+from doot._abstract.structs import SpecStruct_p
 
 PAD           : Final[int] = 15
 TaskFlagNames : Final[str] = [x.name for x in TaskFlags]
 
 @dataclass
-class DootActionSpec:
+class DootActionSpec(SpecStruct_p):
     """
       When an action isn't a full blown class, it gets wrapped in this,
       which passes the action spec to the callable.
 
       TODO: recogise arg prefixs and convert to correct type.
       eg: path:a/relative/path  -> Path(./a/relative/path)
       path:/usr/bin/python  -> Path(/usr/bin/python)
@@ -61,14 +59,40 @@
     do         : None|str                   = field(default=None)
     args       : list[Any]                  = field(default_factory=list)
     kwargs     : TomlGuard                  = field(default_factory=TomlGuard)
     inState    : set[str]                   = field(default_factory=set)
     outState   : set[str]                   = field(default_factory=set)
     fun        : None|Callable              = field(default=None)
 
+    @staticmethod
+    def build(data:dict|list|TomlGuard|DootActionSpec, *, fun=None) -> DootActionSpec:
+        match data:
+            case DootActionSpec():
+                return data
+            case list():
+                action_spec = DootActionSpec(
+                    args=data,
+                    fun=fun if callable(fun) else None
+                    )
+                return action_spec
+
+            case dict() | TomlGuard():
+                kwargs = TomlGuard({x:y for x,y in data.items() if x not in DootActionSpec.__dataclass_fields__.keys()})
+                action_spec = DootActionSpec(
+                    do=data['do'],
+                    args=data.get('args',[]),
+                    kwargs=kwargs,
+                    inState=set(data.get('inState', set())),
+                    outState=set(data.get('outState', set())),
+                    fun=fun if callable(fun) else None
+                    )
+                return action_spec
+            case _:
+                raise doot.errors.DootActionError("Unrecognized specification data", data)
+
     def __str__(self):
         result = []
         if isinstance(self.do, str):
             result.append(f"do={self.do}")
         elif self.do and hasattr(self.do, '__qualname__'):
             result.append(f"do={self.do.__qualname__}")
         elif self.do:
@@ -87,14 +111,17 @@
             result.append(f"calling={self.fun.__qualname__}")
         elif self.fun:
             result.append(f"calling={self.fun.__class__.__qualname__}")
 
         return f"<ActionSpec: {' '.join(result)} >"
 
     def __call__(self, task_state:dict):
+        if self.fun is None:
+            raise doot.errors.DootActionError("Action Spec has not been finalised with a function", self)
+
         return self.fun(self, task_state)
 
     def set_function(self, fun:Action_p|Callable):
         """
           Sets the function of the action spec.
           if given a class, the class it built,
           if given a callable, that is used directly.
@@ -124,32 +151,10 @@
             return
 
         raise doot.errors.DootActionStateError("%s Fields Missing: %s", pos, [x for x in fields if x not in state])
 
     def verify_out(self, state:dict):
         self.verify(state, fields=self.outState)
 
-    @staticmethod
-    def from_data(data:dict|list|TomlGuard|DootActionSpec, *, fun=None) -> DootActionSpec:
-        match data:
-            case DootActionSpec():
-                return data
-            case list():
-                action_spec = DootActionSpec(
-                    args=data,
-                    fun=fun if callable(fun) else None
-                    )
-                return action_spec
-
-            case dict() | TomlGuard():
-                kwargs = TomlGuard({x:y for x,y in data.items() if x not in DootActionSpec.__dataclass_fields__.keys()})
-                action_spec = DootActionSpec(
-                    do=data['do'],
-                    args=data.get('args',[]),
-                    kwargs=kwargs,
-                    inState=set(data.get('inState', set())),
-                    outState=set(data.get('outState', set())),
-                    fun=fun if callable(fun) else None
-                    )
-                return action_spec
-            case _:
-                raise doot.errors.DootActionError("Unrecognized specification data", data)
+    @property
+    def params(self):
+        return self.kwargs
```

### Comparing `doot-0.6.1/doot/_structs/code_ref.py` & `doot-0.7.0/doot/_structs/code_ref.py`

 * *Files 8% similar despite different names*

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
@@ -34,32 +33,50 @@
 ##-- end lib imports
 
 ##-- logging
 logging = logmod.getLogger(__name__)
 ##-- end logging
 
 import importlib
+from importlib.metadata import EntryPoint
 from tomlguard import TomlGuard
+import doot
 import doot.errors
-import doot.constants
-from doot._structs.structured_name import DootStructuredName
+from doot._structs.structured_name import StructuredName
 
 @dataclass(eq=False, slots=True)
-class DootCodeReference(DootStructuredName):
+class DootCodeReference(StructuredName):
     """
       A reference to a class or function. can be created from a string (so can be used from toml),
       or from the actual object (from in python)
     """
-    separator : str                              = field(default=doot.constants.IMPORT_SEP, kw_only=True)
+    separator : str                              = field(default=doot.constants.patterns.IMPORT_SEP, kw_only=True)
     _mixins   : list[DootCodeReference]          = field(default_factory=list, kw_only=True)
     _type     : None|type                        = field(default=None, kw_only=True)
 
     @classmethod
-    def from_str(cls, name:str):
-        if doot.constants.TASK_SEP in name:
+    def build(cls, name:str|type|EntryPoint):
+        match name:
+            case str():
+                return cls._from_str(name)
+            case type():
+                groupHead = name.__module__
+                codeHead  = name.__name__
+                ref = cls(groupHead, codeHead, _type=name)
+                return ref
+            case EntryPoint():
+                loaded = ctor.load()
+                groupHead = loaded.__module__
+                codeHead  = loaded.__name__
+                ref = cls(groupHead, codeHead, _type=loaded)
+                return ref
+
+    @classmethod
+    def _from_str(cls, name:str):
+        if doot.constants.patterns.TASK_SEP in name:
             raise doot.errors.DootError("Code References should use a single colon, not double")
 
         if ":" in name:
             try:
                 groupHead_r, taskHead_r = name.split(":")
                 groupHead = groupHead_r.split(".")
                 taskHead = taskHead_r.split(".")
@@ -68,29 +85,22 @@
         else:
             groupHead = None
             taskHead  = name
 
         return DootCodeReference(groupHead, taskHead)
 
     @staticmethod
-    def from_type(_type:type):
-        groupHead = _type.__module__
-        codeHead  = _type.__name__
-        ref = DootCodeReference(groupHead, codeHead, _type=_type)
-        return ref
-
-    @staticmethod
     def from_alias(alias:str, group:str, plugins:TomlGuard) -> DootCodeReference:
         if group not in plugins:
-            return DootCodeReference.from_str(alias)
+            return DootCodeReference._from_str(alias)
         match [x for x in plugins[group] if x.name == alias]:
             case [x, *xs]:
-                return DootCodeReference.from_str(x.value)
+                return DootCodeReference._from_str(x.value)
             case _:
-                return DootCodeReference.from_str(alias)
+                return DootCodeReference._from_str(alias)
 
     def __str__(self) -> str:
         return "{}{}{}".format(self.module, self.separator, self.value)
 
     def __repr__(self) -> str:
         code_path = str(self)
         mixins    = ", ".join(str(x) for x in self._mixins)
@@ -110,22 +120,20 @@
     def value(self):
         return self.subseparator.join(self.tail)
 
     def add_mixins(self, *mixins:str|DootCodeReference|type, plugins:TomlGuard=None) -> DootCodeReference:
         to_add = self._mixins[:]
         for mix in mixins:
             match mix:
-                case str() if plugins is not None:
-                    ref = DootCodeReference.from_alias(mix, "mixins", plugins)
-                case str():
-                    ref = DootCodeReference.from_str(mix)
                 case DootCodeReference():
                     ref = mix
-                case type():
-                    ref = DootCodeReference.from_type(mix)
+                case str() if plugins is not None:
+                    ref = DootCodeReference.from_alias(mix, "mixin", plugins)
+                case str() | type():
+                    ref = DootCodeReference.build(mix)
                 case _:
                     raise TypeError("Unrecognised mixin type", mix)
 
             if ref not in to_add:
                 to_add.append(ref)
 
         new_ref = DootCodeReference(head=self.head[:], tail=self.tail[:], _mixins=to_add, _type=self._type)
@@ -179,8 +187,8 @@
         for mixin in reversed(sorted(map(lambda x: x.try_import(), self), key=lambda x:  len(x.mro()))):
             if mixin in found:
                 continue
 
             found.update(mixin.mro())
             minimal_mixins.append(mixin)
 
-        return [DootCodeReference.from_type(x) for x in minimal_mixins]
+        return [DootCodeReference.build(x) for x in minimal_mixins]
```

### Comparing `doot-0.6.1/doot/_structs/key.py` & `doot-0.7.0/doot/_structs/key.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,51 +30,56 @@
 
 ##-- lib imports
 import more_itertools as mitz
 ##-- end lib imports
 
 ##-- logging
 logging = logmod.getLogger(__name__)
+printer = logmod.getLogger("doot._printer")
 ##-- end logging
 
+import decorator
 import abc
-from collections import UserString
 import string
 from tomlguard import TomlGuard
 import doot
 import doot.errors
-from doot.constants import KEY_PATTERN, MAX_KEY_EXPANSIONS
-from doot._structs.action_spec import DootActionSpec
-from doot._structs.task_spec import DootTaskSpec
-from doot._structs.artifact import DootTaskArtifact
+from doot._structs.code_ref import DootCodeReference
+from doot._abstract.structs import SpecStruct_p
+from doot.utils.chain_get import DootKeyGetter
+from doot.utils.decorators import DootDecorator
+
+KEY_PATTERN                                = doot.constants.patterns.KEY_PATTERN
+MAX_KEY_EXPANSIONS                         = doot.constants.patterns.MAX_KEY_EXPANSIONS
+STATE_TASK_NAME_K                          = doot.constants.patterns.STATE_TASK_NAME_K
 
-PATTERN        : Final[re.Pattern]         = re.compile("{(.+?)}")
+PATTERN        : Final[re.Pattern]         = re.compile(KEY_PATTERN)
 FAIL_PATTERN   : Final[re.Pattern]         = re.compile("[^a-zA-Z_{}/0-9-]")
 KEYS_HANDLED   : Final[str]                = "_doot_keys_handler"
 ORIG_ARGS      : Final[str]                = "_doot_orig_args"
 KEY_ANNOTS     : Final[str]                = "_doot_keys"
 EXPANSION_HINT : Final[str]                = "_doot_expansion_hint"
 HELP_HINT      : Final[str]                = "_doot_help_hint"
 FUNC_WRAPPED   : Final[str]                = "__wrapped__"
 
-class KWrapper:
+class KWrapper(DootDecorator):
     """ Decorators for actions
     Kwrapper is accessible as DootKey.kwrap
 
     It registers arguments on an action and extracts them from the spec and state automatically.
 
     provides: expands/paths/types/requires/returns/args/kwargs/redirects/redirects_many
 
     The kwarg 'hint' takes a dict and passes the contents to the relevant expansion method as kwargs
 
     arguments are added to the tail of the action args, in order of the decorators.
     the name of the expansion is expected to be the name of the action parameter,
     with a "_" prepended if the name would conflict with a keyword., or with "_ex" as a suffix
-    eg: @DootKey.wrap.paths("from") -> def __call__(self, spec, state, _from):...
-    or: @DootKey.wrap.paths("from") -> def __call__(self, spec, state, from_ex):...
+    eg: @DootKey.kwrap.paths("from") -> def __call__(self, spec, state, _from):...
+    or: @DootKey.kwrap.paths("from") -> def __call__(self, spec, state, from_ex):...
     """
 
     @staticmethod
     def _annotate_keys(f, keys:list) -> bool:
         """ cache original args, and cache declared keys """
         if hasattr(f, FUNC_WRAPPED): # Deal with the actual function, not any decorators
             return KWrapper._annotate_keys(f.__wrapped__, keys)
@@ -132,65 +137,81 @@
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
 
+
+    @staticmethod
+    def taskname(f):
+        KWrapper._annotate_keys(f, [DootKey.build(STATE_TASK_NAME_K, exp_hint="type")])
+        return KWrapper._add_key_handler(f)
+
     @staticmethod
     def expands(*args, hint:dict|None=None, **kwargs):
         """ mark an action as using expanded string keys """
         exp_hint = {"expansion": "str", "kwargs" : hint or {} }
-        keys = [DootKey.make(x, exp_hint=exp_hint, **kwargs) for x in args]
+        keys = [DootKey.build(x, exp_hint=exp_hint, **kwargs) for x in args]
 
         def expand_wrapper(f):
             KWrapper._annotate_keys(f, keys)
             return KWrapper._add_key_handler(f)
 
         return expand_wrapper
 
     @staticmethod
     def paths(*args, hint:dict|None=None, **kwargs):
         """ mark an action as using expanded path keys """
         exp_hint = {"expansion": "path", "kwargs" : hint or {} }
-        keys = [DootKey.make(x, exp_hint=exp_hint, **kwargs) for x in args]
+        keys = [DootKey.build(x, exp_hint=exp_hint, **kwargs) for x in args]
 
         def expand_wrapper(f):
             KWrapper._annotate_keys(f, keys)
             return KWrapper._add_key_handler(f)
 
         return expand_wrapper
 
     @staticmethod
     def types(*args, hint:dict|None=None, **kwargs):
         """ mark an action as using raw type keys """
         exp_hint = {"expansion": "type", "kwargs" : hint or {} }
-        keys = [DootKey.make(x, exp_hint=exp_hint, **kwargs) for x in args]
+        keys = [DootKey.build(x, exp_hint=exp_hint, **kwargs) for x in args]
 
         def expand_wrapper(f):
             KWrapper._annotate_keys(f, keys)
             return KWrapper._add_key_handler(f)
 
         return expand_wrapper
 
@@ -206,75 +227,94 @@
         """ mark an action as using spec.args """
         KWrapper._annotate_keys(f, [DootKwargsKey("kwargs")])
         return KWrapper._add_key_handler(f)
 
     @staticmethod
     def redirects(*args):
         """ mark an action as using redirection keys """
-        keys = [DootKey.make(x, exp_hint="redirect") for x in args]
+        keys = [DootKey.build(x, exp_hint="redirect") for x in args]
 
         def expand_wrapper(f):
             KWrapper._annotate_keys(f, keys)
             return KWrapper._add_key_handler(f)
 
         return expand_wrapper
 
     @staticmethod
     def redirects_many(*args, **kwargs):
         """ mark an action as using redirection key lists """
-        keys = [DootKey.make(x, exp_hint="redirect_multi") for x in args]
+        keys = [DootKey.build(x, exp_hint="redirect_multi") for x in args]
 
         def expand_wrapper(f):
             KWrapper._annotate_keys(f, keys)
             return KWrapper._add_key_handler(f)
 
         return expand_wrapper
 
     @staticmethod
     def requires(*args, **kwargs):
         """ mark an action as requiring certain keys to be passed in """
-        keys = [DootKey.make(x, **kwargs) for x in args]
+        keys = [DootKey.build(x, **kwargs) for x in args]
 
         def expand_wrapper(f):
             KWrapper._annotate_non_expansions(f, keys)
             return f
 
         return expand_wrapper
 
     @staticmethod
     def returns(*args, **kwargs):
         """ mark an action as needing to return certain keys """
-        keys = [DootKey.make(x, **kwargs) for x in args]
+        keys = [DootKey.build(x, **kwargs) for x in args]
 
         def expand_wrapper(f):
             KWrapper._annotate_non_expansions(f, keys)
             return f
 
         return expand_wrapper
 
+    @staticmethod
+    def references(*args, **kwargs):
+        """ mark keys to use as to_coderef imports """
+        exp_hint = {"expansion": "coderef", "kwargs" : {} }
+        keys = [DootKey.build(x, exp_hint=exp_hint, **kwargs) for x in args]
+
+        def expand_wrapper(f):
+            KWrapper._annotate_keys(f, keys)
+            return KWrapper._add_key_handler(f)
+
+        return expand_wrapper
+
 class DootFormatter(string.Formatter):
     """
       A Formatter for expanding arguments based on action spec kwargs, and task state, and cli args
     """
-    _fmt = None
+    _fmt                = None
+
+    SPEC   : Final[str] = "_spec"
+    INSIST : Final[str] = "_insist"
+    STATE  : Final[str] = "_state"
+    LOCS   : Final[str] = "_locs"
+    REC    : Final[str] = "_rec"
 
     @staticmethod
     def fmt(fmt:str|DootKey|pl.Path, /, *args, **kwargs) -> str:
         if not DootFormatter._fmt:
             DootFormatter._fmt = DootFormatter()
 
         return DootFormatter._fmt.format(fmt, *args, **kwargs)
 
     def format(self, fmt:str|DootKey|pl.Path, /, *args, **kwargs) -> str:
+        """ expand and coerce keys """
         self._depth = 0
-        match kwargs.get("_spec", None):
+        match kwargs.get(self.SPEC, None):
             case None:
                 kwargs['_spec'] = {}
-            case DootActionSpec():
-                kwargs['_spec'] = kwargs['_spec'].kwargs
+            case SpecStruct_p():
+                kwargs['_spec'] = kwargs[self.SPEC].params
             case x:
                 raise TypeError("Bad Spec Type in Format Call", x)
 
         match fmt:
             case DootKey():
                 fmt = fmt.form
                 result = self.vformat(fmt, args, kwargs)
@@ -284,95 +324,88 @@
             #     result = str(ftz.reduce(pl.Path.joinpath, [self.vformat(x, args, kwargs) for x in fmt.parts], pl.Path()))
             case _:
                 raise TypeError("Unrecognized expansion type", fmt)
 
         return result
 
     def get_value(self, key, args, kwargs):
+        """ lowest level handling of keys being expanded """
         logging.debug("Expanding: %s", key)
         if isinstance(key, int):
             return args[key]
 
-        insist            = kwargs.get("_insist", False)
-        state             = kwargs.get('_state', None) or {}
-        locs              = kwargs.get("_locs", None)
-        cli               = doot.args.on_fail({}).tasks[str(state.get('_task_name', None))]()
-        replacement       = cli.get(key, None)
-        if replacement is None:
-            spec        = kwargs.get('_spec')
-            replacement = spec.get(key, None)
-        if replacement is None:
-            replacement = state.get(key, None)
-        if replacement is None and locs is not None:
-            match locs.get(key, None):
-                case None:
-                    pass
-                case pl.Path() as x:
-                    replacement = locs.normalize(x)
+        insist                = kwargs.get(self.INSIST, False)
+        spec  : dict          = kwargs.get(self.SPEC, None) or {}
+        state : dict          = kwargs.get(self.STATE, None) or {}
+        locs  : DootLocations = kwargs.get(self.LOCS,  None)
+        depth_check           = self._depth < MAX_KEY_EXPANSIONS
+        rec_allowed           = kwargs.get(self.REC, False) and depth_check
 
-        match replacement:
+        match (replacement:=DootKeyGetter.chained_get(key, spec, state, locs)):
             case None if insist:
                 raise KeyError("Key Expansion Not Found")
             case None:
-                return DootKey.make(key).form
-            case DootKey() if self._depth < MAX_KEY_EXPANSIONS:
+                return DootKey.build(key).form
+            case DootKey() if depth_check:
                 self._depth += 1
                 return self.vformat(replacement.form, args, kwargs)
-            case str() if kwargs.get("_rec", False) and self._depth < MAX_KEY_EXPANSIONS:
+            case str() if rec_allowed:
                 self._depth += 1
                 return self.vformat(str(replacement), args, kwargs)
             case str():
                 return replacement
-            case pl.Path() if self._depth < MAX_KEY_EXPANSIONS:
+            case pl.Path() if depth_check:
                 self._depth += 1
                 return ftz.reduce(pl.Path.joinpath, map(lambda x: self.vformat(x, args, kwargs), replacement.parts), pl.Path())
             case _:
                 return str(replacement)
                 # raise TypeError("Replacement Value isn't a string", args, kwargs)
 
 class DootKey(abc.ABC):
     """ A shared, non-functional base class for DootKeys and variants like DootMultiKey.
-      Use DootKey.make for constructing keys
-      make takes an 'exp_hint' kwarg dict, which can specialize the expansion
+      Use DootKey.build for constructing keys
+      build takes an 'exp_hint' kwarg dict, which can specialize the expansion
 
       DootSimpleKeys are strings, wrapped in {} when used in toml.
-      so DootKey.make("blah") -> DootSimpleKey("blah") -> DootSimpleKey('blah').form =="{blah}" -> [toml] aValue = "{blah}"
+      so DootKey.build("blah") -> DootSimpleKey("blah") -> DootSimpleKey('blah').form =="{blah}" -> [toml] aValue = "{blah}"
 
       DootMultiKeys are containers of a string `value`, and a list of SimpleKeys the value contains.
-      So DootKey.make("{blah}/{bloo}") -> DootMultiKey("{blah}/{bloo}", [DootSimpleKey("blah", DootSimpleKey("bloo")]) -> .form == "{blah}/{bloo}"
+      So DootKey.build("{blah}/{bloo}") -> DootMultiKey("{blah}/{bloo}", [DootSimpleKey("blah", DootSimpleKey("bloo")]) -> .form == "{blah}/{bloo}"
     """
+    dec   = KWrapper
     kwrap = KWrapper
 
     @staticmethod
-    def make(s:str|DootKey|DootTaskArtifact|pl.Path|dict, *, strict=False, explicit=False, exp_hint:str|dict=None, help=None) -> DootKey:
+    def build(s:str|DootKey|pl.Path|dict, *, strict=False, explicit=False, exp_hint:str|dict=None, help=None) -> DootKey:
         """ Make an appropriate DootKey based on input value
           Can only create MultiKeys if strict = False,
           if explicit, only keys wrapped in {} are made, everything else is returned untouched
           if strict, then only simple keys can be returned
         """
         # TODO annotate with 'help'
-        # TODO store expansion args on make
+        # TODO store expansion args on build
         match exp_hint:
             case "path":
                 is_path = True
             case {"expansion": "path"}:
                 is_path = True
             case _:
                 is_path = False
         result = s
         match s:
             case { "path": x }:
                 result = DootPathMultiKey(x)
                 exp_hint = "path"
+            case pl.Path():
+                result = DootPathMultiKey(s)
+                exp_hint = "path"
             case DootSimpleKey() if strict:
                 result = s
             case DootKey():
                 result = s
-            case DootTaskArtifact(path=path) | (pl.Path() as path) if not strict:
-                result = DootPathMultiKey(path)
             case str() if not (s_keys := PATTERN.findall(s)) and not explicit and not is_path:
                 result = DootSimpleKey(s)
             case str() if is_path and not bool(s_keys):
                 result = DootPathSimpleKey(s)
             case str() if is_path and len(s_keys) == 1 and s_keys[0] == s[1:-1]:
                 result = DootPathSimpleKey(s[1:-1])
             case str() if is_path and len(s_keys) > 1:
@@ -414,46 +447,53 @@
                 return self.to_path(spec, state, **kwargs)
             case {"expansion" : "type", "kwargs" : kwargs}:
                 return self.to_type(spec, state, **kwargs)
             case {"expansion": "redirect"}:
                 return self.redirect(spec)
             case {"expansion": "redirect_multi"}:
                 return self.redirect_multi(spec)
+            case {"expansion": "coderef"}:
+                return self.to_coderef(spec, state)
             case x:
                 raise doot.errors.DootKeyError("Key Called with Bad Key Expansion Type", self, x)
 
     @property
     def form(self) -> str:
         return str(self)
 
     @property
+    def direct(self):
+        return str(self).removesuffix("_")
+
+    @property
     def is_indirect(self) -> bool:
         return False
 
     def redirect(self, spec=None) -> DootKey:
         return self
 
     def to_path(self, spec=None, state=None, chain:list[DootKey]=None, locs:DootLocations=None, on_fail:None|str|pl.Path|DootKey=Any, symlinks=False) -> pl.Path:
         """
-          Convert a key to an absolute path
+          Convert a key to an absolute path, using registered locations
+
+          The Process is:
+          1) redirect the given key if necessary
+          2) Expand each part of the keypath, using DootFormatter
+          3) normalize it
+
+          If necessary, a fallback chain, and on_fail value can be provided
         """
         locs                 = locs or doot.locs
         key : pl.Path        = pl.Path(self.redirect(spec).form)
 
         try:
-            expanded         : list       = [DootFormatter.fmt(x, _spec=spec, _state=state, _rec=True) for x in key.parts]
-            expanded_as_path : pl.Path    = pl.Path().joinpath(*expanded)
-            depth                         = 0
-            while PATTERN.search(str(expanded_as_path)) and depth < MAX_KEY_EXPANSIONS:
-                to_keys          : list       = [DootKey.make(x, explicit=True) or x for x in expanded_as_path.parts]
-                loc_expansions   : list       = [locs.get(x) for x in to_keys]
-                expanded_as_path : pl.Path    = pl.Path().joinpath(*loc_expansions)
-                depth += 1
+            expanded         : list       = [DootFormatter.fmt(x, _spec=spec, _state=state, _rec=True, _locs=locs) for x in key.parts]
+            expanded_as_path : pl.Path    = pl.Path().joinpath(*expanded) # allows ("a", "b/c") -> "a/b/c"
 
-            if any(bool(matches) for x in expanded_as_path.parts if (matches:=PATTERN.findall(x))):
+            if bool(matches:=PATTERN.findall(str(expanded_as_path))):
                 raise doot.errors.DootLocationExpansionError("Missing keys on path expansion", matches, self)
 
             return locs.normalize(expanded_as_path, symlinks=symlinks)
 
         except doot.errors.DootLocationExpansionError as err:
             if bool(chain):
                 return chain[0].to_path(spec, state, chain=chain[1:], on_fail=on_fail, symlinks=symlinks)
@@ -466,22 +506,45 @@
                     return locs.normalize(pl.Path(on_fail),  symlinks=symlinks)
                 case _:
                     raise err
 
     def within(self, other:str|dict|TomlGuard) -> bool:
         return False
 
+    def basic(self, spec:SpecStruct_p, state, locs=None):
+        """ the most basic expansion of a key """
+        kwargs = spec.params
+        return DootKeyGetter.chained_get(str(self), kwargs, state, locs or doot.locs)
+
     @abc.abstractmethod
     def to_type(self, spec, state, type_=Any, chain:list[DootKey]=None, on_fail=Any, **kwargs) -> Any:
         raise NotImplementedError()
 
     @abc.abstractmethod
     def expand(self, spec=None, state=None, *, rec=False, insist=False, chain:list[DootKey]=None, on_fail=Any, locs:DootLocations=None, **kwargs) -> str:
         pass
 
+    def to_coderef(self, spec:None|SpecStruct_p, state) -> None|DootCodeReference:
+        match spec:
+            case SpecStruct_p():
+                kwargs = spec.params
+            case None:
+                kwargs = {}
+
+        redir = self.redirect(spec)
+
+        if redir not in kwargs and redir not in state:
+            return None
+        try:
+            expanded = self.expand(spec, state)
+            ref = DootCodeReference.build(expanded)
+            return ref
+        except doot.errors.DootError:
+            return None
+
 class DootNonKey(str, DootKey):
     """
       Just a string, not a key. But this lets you call no-ops for key specific methods
     """
 
     def __repr__(self):
         return "<DootNonKey: {}>".format(str(self))
@@ -523,16 +586,16 @@
     def expand(self, spec=None, state=None, *, rec=False, insist=False, chain:list[DootKey]=None, on_fail=Any, locs:DootLocations=None, **kwargs) -> str:
         return str(self)
 
     def redirect(self, spec=None) -> DootKey:
         return self
 
     def to_type(self, spec, state, type_=Any, **kwargs) -> str:
-        if type_ != Any or type_ != str:
-            raise TypeError("NonKey's can only be strings", self)
+        if type_ not in [Any, str]:
+            raise TypeError("NonKey's can only be strings", self, type_)
         return str(self)
 
 class DootSimpleKey(str, DootKey):
     """
       A Single key with no extras.
       ie: {x}. not {x}{y}, or {x}.blah.
     """
@@ -558,15 +621,15 @@
 
     @property
     def is_indirect(self):
         return str(self).endswith("_")
 
     @property
     def form(self):
-        """ Return the key in its use form """
+        """ Return the key in its use form, ie: wrapped in braces """
         return "{{{}}}".format(str(self))
 
     def within(self, other:str|dict|TomlGuard) -> bool:
         match other:
             case str():
                 return self.form in other
             case dict() | TomlGuard():
@@ -582,94 +645,83 @@
             if bool(chain):
                 return chain[0].expand(spec, state, rec=rec, chain=chain[1:], on_fail=on_fail)
             elif on_fail != Any:
                 return on_fail
             else:
                 raise err
 
-    def redirect(self, spec=None) -> DootKey:
+    def redirect(self, spec:None|SpecStruct_p=None) -> DootKey:
         """
           If the indirect form of the key is found in the spec, use that as a key instead
         """
         if not spec:
             return self
 
         match spec:
-            case DootTaskSpec():
-                kwargs = spec.extra
-            case DootActionSpec():
-                kwargs = spec.kwargs
+            case SpecStruct_p():
+                kwargs = spec.params
+            case None:
+                kwargs = {}
 
         match kwargs.get(self.indirect, self):
             case str() as x if x == self.indirect:
                 return self
             case str() as x:
-                return DootKey.make(x)
+                return DootKey.build(x)
             case list() as lst:
                 raise TypeError("Key Redirection resulted in a list, use redirect_multi", self)
 
         return self
 
-    def redirect_multi(self, spec=None) -> list[DootKey]:
+    def redirect_multi(self, spec:None|SpecStruct_p=None) -> list[DootKey]:
         """ redirect an indirect key to a *list* of keys """
         if not spec:
             return [self]
 
         match spec:
-            case DootTaskSpec():
-                kwargs = spec.extra
-            case DootActionSpec():
-                kwargs = spec.kwargs
+            case SpecStruct_p():
+                kwargs = spec.params
+            case None:
+                kwargs = {}
 
         match kwargs.get(self.indirect, self):
             case str() as x if x == self:
                 return [self]
             case str() as x:
-                return [DootKey.make(x)]
+                return [DootKey.build(x)]
             case list() as lst:
-                return [DootKey.make(x) for x in lst]
+                return [DootKey.build(x) for x in lst]
 
         return [self]
 
-    def to_type(self, spec=None, state=None, type_=Any, chain:list[DootKey]=None, on_fail=Any) -> Any:
+    def to_type(self, spec:None|SpecStruct_p=None, state=None, type_=Any, chain:list[DootKey]=None, on_fail=Any) -> Any:
         target            = self.redirect(spec)
 
         match spec:
-            case DootTaskSpec():
-                kwargs = spec.extra
-            case DootActionSpec():
-                kwargs = spec.kwargs
+            case SpecStruct_p():
+                kwargs = spec.params
             case None:
                 kwargs = {}
 
-        task_name         = state.get("_task_name", None) if state else None
-        if task_name:
-            cli           = doot.args.on_fail({}).tasks[str(state.get('_task_name', None))]()
-        else:
-            cli           = {}
-
-        replacement       = cli.get(target, None)
-        if replacement is None and kwargs:
-            replacement = kwargs.get(target, None)
-        if replacement is None and state:
-            replacement = state.get(target, None)
-
-        match replacement:
+        task_name = state.get(STATE_TASK_NAME_K, None) if state else None
+        match (replacement:=DootKeyGetter.chained_get(target, kwargs, state)):
             case None if bool(chain):
                 return chain[0].to_type(spec, state, type_=type_, chain=chain[1:], on_fail=on_fail)
             case None if on_fail != Any and isinstance(on_fail, DootKey):
                 return on_fail.to_type(spec, state, type_=type_)
             case None if on_fail != Any:
                 return on_fail
             case None if type_ is Any or type_ is None:
                 return None
             case _ if type_ is Any:
                 return replacement
             case _ if type_ and isinstance(replacement, type_):
                 return replacement
+            case None if not any(target in x for x in [kwargs, state]):
+                raise KeyError("Key is not available in the state or spec", target)
             case _:
                 raise TypeError("Unexpected Type for replacement", type_, replacement, self)
 
 class DootPathSimpleKey(DootSimpleKey):
     """ A Key that always expands as a path """
 
     def expand(self, spec=None, state=None, *, rec=False, insist=False, chain:list[DootKey]=None, on_fail=Any, locs=None, **kwargs):
@@ -706,32 +758,28 @@
     def expand(self, *args, **kwargs):
         raise doot.errors.DootKeyError("Args Key doesn't expand")
 
     def redirect(self, spec=None):
         raise doot.errors.DootKeyError("Args Key doesn't redirect")
 
     def to_type(self, spec=None, state=None, *args, **kwargs) -> list:
-        match spec:
-            case DootTaskSpec():
-                return []
-            case DootActionSpec():
-                return spec.args
+        return spec.args
 
 class DootKwargsKey(DootArgsKey):
     """ A Key representing all of an action spec's kwargs """
 
     def __repr__(self):
         return "<DootArgsKey>"
 
-    def to_type(self, spec=None, state=None, *args, **kwargs) -> dict:
+    def to_type(self, spec:None|SpecStruct_p=None, state=None, *args, **kwargs) -> dict:
         match spec:
-            case DootTaskSpec():
-                return spec.extra
-            case DootActionSpec():
-                return spec.kwargs
+            case SpecStruct_p():
+                return spec.params
+            case None:
+                return {}
 
 class DootMultiKey(DootKey):
     """ A string or path of multiple keys """
 
     def __init__(self, val:str|pl.Path):
         self.value : str|pl.Path        = val
         self._keys : set[DootSimpleKey] = set(DootSimpleKey(x) for x in PATTERN.findall(str(val)))
@@ -771,15 +819,15 @@
             else:
                 raise err
 
     def within(self, other:str|dict|TomlGuard) -> bool:
         return str(self) in other
 
     def to_type(self, spec, state, type_=Any, chain:list[DootKey]=None, on_fail=Any) -> Any:
-        raise TypeError("Converting a MultiKey to a type doesn't make sense", self)
+        raise TypeError("Converting a MultiKey to a type doesn't build sense", self)
 
 class DootPathMultiKey(DootMultiKey):
     """ A MultiKey that always expands as a path """
 
     def expand(self, spec=None, state=None, *, rec=False, insist=False, chain:list[DootKey]=None, on_fail=Any, locs=None, **kwargs):
         return str(self.to_path(spec, state, chain=chain, on_fail=on_fail, locs=locs))
 
@@ -800,10 +848,10 @@
             case {"expansion": "redirect_multi"}:
                 return self.redirect_multi(spec)
             case x:
                 raise doot.errors.DootKeyError("Key Called with Bad Key Expansion Type", self, x)
 
 class DootImportKey(DootSimpleKey):
     """ a key to specify a key is used for importing
-    ie: str expands -> DootCodeReference.from_str -> .try_import
+    ie: str expands -> DootCodeReference.build -> .try_import
     """
     pass
```

### Comparing `doot-0.6.1/doot/_structs/param_spec.py` & `doot-0.7.0/doot/_structs/param_spec.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,23 +34,24 @@
 
 ##-- logging
 logging = logmod.getLogger(__name__)
 ##-- end logging
 
 import importlib
 from tomlguard import TomlGuard
+import doot
 import doot.errors
-import doot.constants
 from doot.enums import TaskFlags, ReportEnum
+from doot._abstract.structs import ParamStruct_p
 
 PAD           : Final[int] = 15
 TaskFlagNames : Final[str] = [x.name for x in TaskFlags]
 
 @dataclass
-class DootParamSpec:
+class DootParamSpec(ParamStruct_p):
     """ Describes a command line parameter to use in the parser
       When `positional`, will not match against a string starting with `prefix`
       consumed in doot._abstract.parser.ArgParser_i's
       produced using doot._abstract.parser.ParamSpecMaker_m classes,
       like tasks, and jobs
     """
     name              : str                       = field()
@@ -67,15 +68,15 @@
 
     _repeatable_types : ClassVar[list[Any]]       = [list, int]
 
     separator         : str                       = field(default="=")
     _consumed         : int                       = field(default=0)
 
     @classmethod
-    def from_dict(cls, data:TomlGuard|dict) -> DootParamSpec:
+    def build(cls, data:TomlGuard|dict) -> DootParamSpec:
         param =  cls(**data)
         match param:
             case DootParamSpec(type="int"):
                 param.type = int
             case DootParamSpec(type="float"):
                 param.type = float
             case DootParamSpec(type="bool"):
@@ -108,14 +109,34 @@
     def inverse(self):
         return f"no-{self.name}"
 
     @property
     def repeatable(self):
         return self.type in DootParamSpec._repeatable_types and not self.positional
 
+    @property
+    def key_str(self):
+        if self.invisible or self.positional:
+            return ""
+
+        if self.prefix == doot.constants.patterns.PARAM_ASSIGN_PREFIX:
+            return f"{self.prefix}{self.name}{self.separator}"
+
+        return f"{self.prefix}{self.name}"
+
+    @property
+    def short_key_str(self):
+        if self.invisible or self.positional:
+            return ""
+
+        if self.prefix == doot.constants.patterns.PARAM_ASSIGN_PREFIX:
+            return f"{self.prefix}{self.name[0]}{self.separator}"
+
+        return f"{self.prefix}{self.name[0]}"
+
     def _split_name_from_value(self, val):
         match self.positional:
             case False:
                 return val.removeprefix(self.prefix).split(self.separator)
             case True if isinstance(val, list):
                 return (self.name, val)
             case True | int():
@@ -171,81 +192,24 @@
         return " ".join(parts)
 
     def __repr__(self):
         if self.positional:
             return f"<ParamSpec: {self.name}>"
         return f"<ParamSpec: {self.prefix}{self.name}>"
 
-    @property
-    def key_str(self):
-        if self.invisible or self.positional:
-            return ""
-
-        if self.prefix == doot.constants.PARAM_ASSIGN_PREFIX:
-            return f"{self.prefix}{self.name}{self.separator}"
-
-        return f"{self.prefix}{self.name}"
-
-    @property
-    def short_key_str(self):
-        if self.invisible or self.positional:
-            return ""
-
-        if self.prefix == doot.constants.PARAM_ASSIGN_PREFIX:
-            return f"{self.prefix}{self.name[0]}{self.separator}"
-
-        return f"{self.prefix}{self.name[0]}"
-
-    def maybe_consume(self, args:list[str], data:dict) -> int:
-        """
-          Given a list of args, possibly add a value to the data.
-          operates *in place* on both the args list and the data.
-          return True if _consumed a value
-
-          handles:
-          ["--arg=val"],
-          ["-arg", "val"],
-          ["val"],     (if positional=True)
-          ["-arg"],    (if type=bool)
-          ["-no-arg"], (if type=bool)
-        """
-        if not bool(args) or data is None or args[0] != self:
-            return 0
-        if 0 < self._consumed:
-            return self._consumed
-
-        pop_count     = 0
-        focus         = args[0]
-        is_positional = bool(self.positional)
-
-
-        if is_positional:
-            pop_count = self._add_positional_value(data, key=self.name, vals=args)
-        else:
-            key, vals, pop_count = self._calc_positional_consumption(focus, args)
-            self._add_non_positional_value(data, key=key, vals=vals)
-
-        # data has been added, so remove it from the input list
-        logging.debug("Arg: %s consuming count %s", self.name, pop_count)
-        for x in range(pop_count):
-            args.pop(0)
-
-        self._consumed += pop_count
-        return self._consumed
-
     def _calc_positional_consumption(self, focus, args):
         pop_count     = 1
         prefixed      = focus.startswith(self.prefix) # form of -param
         is_assign     = self.separator in focus       # form of --param=arg
         key, vals     = None, []
 
         # Figure out the key and value
         match prefixed, is_assign:
-            case _, True if self.prefix != doot.constants.PARAM_ASSIGN_PREFIX:
-                raise doot.errors.DootParseError("Assignment parameters should be prefixed with the PARAM_ASSIGN_PREFIX", doot.constants.PARAM_ASSIGN_PREFIX)
+            case _, True if self.prefix != doot.constants.patterns.PARAM_ASSIGN_PREFIX:
+                raise doot.errors.DootParseError("Assignment parameters should be prefixed with the PARAM_ASSIGN_PREFIX", doot.constants.patterns.PARAM_ASSIGN_PREFIX)
             case True, False if self.type.__name__ != "bool" and not bool(args):
                 raise doot.errors.DootParseError("key lacks a following value", focus, self.type.__name__)
             case True, True: # --key=val
                 key, val = focus.split(self.separator)
                 key = key.removeprefix(self.prefix)
                 vals.append(val)
             case True, False if self.type.__name__ == "bool": # --key
@@ -253,15 +217,14 @@
             case True, False: # -key val
                 key = focus.removeprefix(self.prefix)
                 vals.append(args[1])
                 pop_count = 2
 
         return key, vals, pop_count
 
-
     def _add_non_positional_value(self, data:dict, *, key:str=None, vals:list[str]=None) -> bool:
         """ if the given value is suitable, add it into the given data
         takes separated key, values,
         and the key has had the prefix stripped
         """
         vals = vals or []
         # TODO if constraints, check against them
@@ -320,7 +283,43 @@
             raise doot.errors.DootParseError("Not Enough positional args provided", self.name, self.positional, vals)
         elif 1 < self.positional < pop_count:
             raise doot.errors.DootParseError("Too Many positional args provided", self.name, self.positional, vals)
         elif 1 < pop_count and self.type != list:
             raise doot.errors.DootParseError("Multi positional args should be of type list", self.name, self.positional, self.type)
 
         return pop_count
+
+    def maybe_consume(self, args:list[str], data:dict) -> int:
+        """
+          Given a list of args, possibly add a value to the data.
+          operates *in place* on both the args list and the data.
+          return True if _consumed a value
+
+          handles:
+          ["--arg=val"],
+          ["-arg", "val"],
+          ["val"],     (if positional=True)
+          ["-arg"],    (if type=bool)
+          ["-no-arg"], (if type=bool)
+        """
+        if not bool(args) or data is None or args[0] != self:
+            return 0
+        if 0 < self._consumed:
+            return self._consumed
+
+        pop_count     = 0
+        focus         = args[0]
+        is_positional = bool(self.positional)
+
+        if is_positional:
+            pop_count = self._add_positional_value(data, key=self.name, vals=args)
+        else:
+            key, vals, pop_count = self._calc_positional_consumption(focus, args)
+            self._add_non_positional_value(data, key=key, vals=vals)
+
+        # data has been added, so remove it from the input list
+        logging.debug("Arg: %s consuming count %s", self.name, pop_count)
+        for x in range(pop_count):
+            args.pop(0)
+
+        self._consumed += pop_count
+        return self._consumed
```

### Comparing `doot-0.6.1/doot/_structs/sname.py` & `doot-0.7.0/doot/_structs/sname.py`

 * *Files 8% similar despite different names*

```diff
@@ -34,44 +34,44 @@
 
 ##-- logging
 logging = logmod.getLogger(__name__)
 ##-- end logging
 
 import importlib
 from tomlguard import TomlGuard
+import doot
 import doot.errors
-import doot.constants
 from doot.enums import TaskFlags, ReportEnum
-from doot._structs.structured_name import DootStructuredName
+from doot._structs.structured_name import StructuredName
 from doot._structs.task_name import DootTaskName
 from doot._structs.code_ref import DootCodeReference
 
 PAD           : Final[int] = 15
 TaskFlagNames : Final[str] = [x.name for x in TaskFlags]
 
 @dataclass(eq=False, slots=True)
-class DootStructuredName(DootStructuredName):
+class DootStructuredName(StructuredName):
     """ A Complex name class for identifying tasks and classes.
 
       Classes are the standard form used in importlib: "module.path:ClassName"
       Tasks use a double colon to separate head from tail name: "group.name::TaskName"
 
     """
     head            : list[str]          = field(default_factory=list)
     tail            : list[str]          = field(default_factory=list)
 
-    separator       : str                = field(default=doot.constants.TASK_SEP, kw_only=True)
+    separator       : str                = field(default=doot.constants.patterns.TASK_SEP, kw_only=True)
     subseparator    : str                = field(default=".", kw_only=True)
 
     @staticmethod
     def build(name:str|DootStructuredName|type) -> DootStructuredName:
         match name:
             case DootStructuredName():
                 return name
             case type():
-                return DootCodeReference.from_type(name)
-            case str() if doot.constants.TASK_SEP in name:
-                return DootTaskName.from_str(name)
-            case str() if doot.constants.IMPORT_SEP in name:
-                return DootTaskName.from_str(name)
+                return DootCodeReference.build(name)
+            case str() if doot.constants.patterns.TASK_SEP in name:
+                return DootTaskName.build(name)
+            case str() if doot.constants.patterns.IMPORT_SEP in name:
+                return DootTaskName.build(name)
             case _:
                 raise doot.errors.DootError("Tried to build a name from a bad value", name)
```

### Comparing `doot-0.6.1/doot/_structs/structured_name.py` & `doot-0.7.0/doot/_structs/structured_name.py`

 * *Files 17% similar despite different names*

```diff
@@ -34,67 +34,82 @@
 
 ##-- logging
 logging = logmod.getLogger(__name__)
 ##-- end logging
 
 import importlib
 from tomlguard import TomlGuard
+import doot
 import doot.errors
-import doot.constants
 from doot.enums import TaskFlags, ReportEnum
 
 PAD           : Final[int] = 15
 TaskFlagNames : Final[str] = [x.name for x in TaskFlags]
 
+def aware_splitter(x, sep="."):
+    match x:
+        case str():
+            return x.split(sep)
+        case _:
+            return [x]
+
 @dataclass(eq=False, slots=True)
-class DootStructuredName:
+class StructuredName:
     """ A Complex name class for identifying tasks and classes.
 
       Classes are the standard form used in importlib: "module.path:ClassName"
       Tasks use a double colon to separate head from tail name: "group.name::TaskName"
 
     """
     head            : list[str]          = field(default_factory=list)
-    tail            : list[str]          = field(default_factory=list)
+    tail            : list[str|UUID]     = field(default_factory=list)
 
-    separator       : str                = field(default=doot.constants.TASK_SEP, kw_only=True)
+    separator       : str                = field(default=doot.constants.patterns.TASK_SEP, kw_only=True)
     subseparator    : str                = field(default=".", kw_only=True)
 
     def __post_init__(self):
+        sub_split = ftz.partial(aware_splitter, sep=self.subseparator)
         match self.head:
             case None | []:
                 self.head = ["default"]
             case ["tasks", x] if x.startswith('"') and x.endswith('"'):
-                self.head = ftz.reduce(lambda x, y: x + y, map(lambda x: x.split(self.subseparator), x[1:-1]))
+                self.head = ftz.reduce(lambda x, y: x + y, map(sub_split, x[1:-1]))
             case ["tasks", *xs]:
-                self.head = ftz.reduce(lambda x, y: x + y, map(lambda x: x.split(self.subseparator), xs))
+                self.head = ftz.reduce(lambda x, y: x + y, map(sub_split, xs))
             case list():
-                self.head = ftz.reduce(lambda x, y: x + y, map(lambda x: x.split(self.subseparator), self.head))
+                self.head = ftz.reduce(lambda x, y: x + y, map(sub_split, self.head))
             case str():
                 self.head = self.head.split(self.subseparator)
+            case _:
+                self.head = [self.head]
 
         match self.tail:
             case None | []:
                 self.tail = ["default"]
             case list():
-                self.tail = ftz.reduce(lambda x, y: x + y, map(lambda x: x.split(self.subseparator), self.tail))
+                self.tail = ftz.reduce(lambda x, y: x + y, map(sub_split, self.tail))
             case str():
                 self.tail = self.tail.split(self.subseparator)
+            case _:
+                self.tail = [self.tail]
 
     def __hash__(self):
         return hash(str(self))
 
+    def __str__(self):
+        return self.head_str + self.separator + self.tail_str
+
     def __lt__(self, other) -> bool:
         """ Compare two names, return true if other is a subname of this name
         eg: a.b.c < a.b.c.d
         """
         match other:
             case str():
-                other = DootStructuredName.from_str(other)
-            case DootStructuredName():
+                other = StructuredName.build(other)
+            case StructuredName():
                 pass
             case _:
                 return False
 
         for x,y in zip(self.head, other.head):
             if x != y:
                 return False
@@ -108,11 +123,11 @@
     def __contains__(self, other:str):
         return str(other) in str(self)
 
     def __eq__(self, other):
         return str(self) == str(other)
 
     def tail_str(self):
-        return self.subseparator.join(self.tail)
+        return self.subseparator.join(str(x) for x in self.tail)
 
     def head_str(self):
-        return self.subseparator.join(self.head)
+        return self.subseparator.join(str(x) for x in self.head)
```

### Comparing `doot-0.6.1/doot/_structs/stub.py` & `doot-0.7.0/doot/_structs/stub.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,26 +34,28 @@
 
 ##-- logging
 logging = logmod.getLogger(__name__)
 ##-- end logging
 
 import importlib
 from tomlguard import TomlGuard
+import doot
 import doot.errors
-import doot.constants
-from doot.enums import TaskFlags, ReportEnum
-from doot._structs.sname import DootTaskName, DootCodeReference
+from doot.enums import TaskFlags, ReportEnum, LocationMeta, TaskQueueMeta
+from doot._structs.task_name import DootTaskName
+from doot._structs.code_ref import DootCodeReference
 from doot._structs.task_spec import DootTaskSpec
+from doot._abstract.structs import StubStruct_p
 
 PAD           : Final[int]               = 15
 TaskFlagNames : Final[str]               = [x.name for x in TaskFlags]
-DEFAULT_CTOR  : Final[DootCodeReference] = DootCodeReference.from_str(doot.constants.DEFAULT_PLUGINS['task'][1][1])
+DEFAULT_CTOR  : Final[DootCodeReference] = DootCodeReference.build(doot.aliases.task[doot.constants.entrypoints.DEFAULT_TASK_CTOR_ALIAS])
 
 @dataclass
-class TaskStub:
+class TaskStub(StubStruct_p):
     """ Stub Task Spec for description in toml
     Automatically Adds default keys from DootTaskSpec
 
     This essentially wraps a dict, adding toml stubs parts as you access keys.
     eg:
     obj = TaskStub()
     ob["blah"].type = "int"
@@ -64,33 +66,57 @@
     ctor       : str|DootCodeReference|type                     = field(default=DEFAULT_CTOR)
     parts      : dict[str, TaskStubPart]                        = field(default_factory=dict, kw_only=True)
 
     # Don't copy these from DootTaskSpec blindly
     skip_parts : ClassVar[set[str]]          = set(["name", "extra", "ctor", "source", "version"])
 
     def __post_init__(self):
-        self['name'].default     = DootTaskName.from_str(doot.constants.DEFAULT_STUB_TASK_NAME)
+        self['name'].default     = DootTaskName.build(doot.constants.names.DEFAULT_STUB_TASK_NAME)
         self['version'].default  = "0.1"
         # Auto populate the stub with what fields are defined in a TaskSpec:
         for dcfield in DootTaskSpec.__dataclass_fields__.values():
             if dcfield.name in TaskStub.skip_parts:
                 continue
             self.parts[dcfield.name] = TaskStubPart(key=dcfield.name, type=dcfield.type)
             if dcfield.default != MISSING:
                 self.parts[dcfield.name].default = dcfield.default
 
+    def __getitem__(self, key):
+        if key not in self.parts:
+            self.parts[key] = TaskStubPart(key)
+        return self.parts[key]
+
+    def __iadd__(self, other):
+        match other:
+            case [head, val] if head in self.parts:
+                self.parts[head].default = val
+            case [head, val]:
+                self.parts[head] = TaskStubPart(head, default=val)
+            case { "name" : name, "type": type, "default": default, "doc": doc, }:
+                pass
+            case { "name" : name, "default": default }:
+                pass
+            case dict():
+                part = TaskStubPart(**other)
+            case TomlGuard():
+                pass
+            case TaskStubPart() if other.key not in self.parts:
+                self.parts[other.key] = other
+            case _:
+                raise TypeError("Unrecognized Toml Stub component")
+
     def to_toml(self) -> str:
         parts = []
         parts.append(self.parts['name'])
         parts.append(self.parts['version'])
         parts.append(self.parts['doc'])
         if 'ctor' in self.parts:
             parts.append(self.parts['ctor'])
         elif isinstance(self.ctor, type):
-            parts.append(TaskStubPart("ctor", type="type", default=f"\"{self.ctor.__module__}{doot.constants.IMPORT_SEP}{self.ctor.__name__}\""))
+            parts.append(TaskStubPart("ctor", type="type", default=f"\"{self.ctor.__module__}{doot.constants.patterns.IMPORT_SEP}{self.ctor.__name__}\""))
         else:
             parts.append(TaskStubPart("ctor", type="type", default=f"\"{self.ctor}\""))
         if "mixins" in self.parts:
             parts.append(self.parts['mixins'])
 
         delayed_actions = []
         for key, part in sorted(self.parts.items(), key=lambda x: x[1]):
@@ -103,38 +129,14 @@
 
         # Actions always go at the end
         for part in delayed_actions:
             parts.append(part)
 
         return "\n".join(map(str, parts))
 
-    def __getitem__(self, key):
-        if key not in self.parts:
-            self.parts[key] = TaskStubPart(key)
-        return self.parts[key]
-
-    def __iadd__(self, other):
-        match other:
-            case [head, val] if head in self.parts:
-                self.parts[head].default = val
-            case [head, val]:
-                self.parts[head] = TaskStubPart(head, default=val)
-            case { "name" : name, "type": type, "default": default, "doc": doc, }:
-                pass
-            case { "name" : name, "default": default }:
-                pass
-            case dict():
-                part = TaskStubPart(**other)
-            case TomlGuard():
-                pass
-            case TaskStubPart() if other.key not in self.parts:
-                self.parts[other.key] = other
-            case _:
-                raise TypeError("Unrecognized Toml Stub component")
-
 @dataclass
 class TaskStubPart:
     """ Describes a single part of a stub task in toml """
     key      : str      = field()
     type     : str      = field(default="str")
     prefix   : str      = field(default="")
 
@@ -157,31 +159,35 @@
 
         key_str     = f"{self.key:<20}"
         type_str    = f"<{self.type}>"
         comment_str = f"{self.comment}"
         val_str     = None
 
         match self.default:
-            case TaskFlags():
+            case TaskFlags() | LocationMeta():
                 parts = [x.name for x in TaskFlags if x in self.default]
                 joined = ", ".join(map(lambda x: f"\"{x}\"", parts))
                 val_str = f"[ {joined} ]"
+            case TaskQueueMeta():
+                val_str = '"{}"'.format(self.default.name)
             case "" if self.type == "TaskFlags":
                 val_str = f"[ \"{TaskFlags.TASK.name}\" ]"
             case bool():
                 val_str = str(self.default).lower()
             case str() if self.type == "type":
                 val_str = self.default
             case list() if "Flags" in self.type:
                 parts = ", ".join([f"\"{x}\"" for x in self.default])
                 val_str = f"[{parts}]"
             case list() if all(isinstance(x, (int, float)) for x in self.default):
+
                 def_str = ", ".join(str(x) for x in self.default)
                 val_str = f"[{def_str}]"
             case list():
+
                 def_str = ", ".join([f'"{x}"' for x in self.default])
                 val_str = f"[{def_str}]"
             case dict():
                 val_str = "{}"
             case _ if "list" in self.type:
 
                 def_str = ", ".join(str(x) for x in self.default)
```

### Comparing `doot-0.6.1/doot/_structs/task_name.py` & `doot-0.7.0/doot/_structs/task_name.py`

 * *Files 24% similar despite different names*

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
@@ -35,68 +34,100 @@
 
 ##-- logging
 logging = logmod.getLogger(__name__)
 ##-- end logging
 
 import importlib
 from tomlguard import TomlGuard
+import doot
 import doot.errors
-import doot.constants
 from doot.enums import TaskFlags, ReportEnum
-from doot._structs.structured_name import DootStructuredName
+from doot._structs.structured_name import StructuredName, aware_splitter
 
 TaskFlagNames : Final[str] = [x.name for x in TaskFlags]
 
 @dataclass(eq=False, slots=True)
-class DootTaskName(DootStructuredName):
+class DootTaskName(StructuredName):
     """
       A Task Name.
+
     """
 
-    internal           : bool                    = field(default=False, kw_only=True)
-    separator          : str                     = field(default=doot.constants.TASK_SEP, kw_only=True)
+    separator          : str                     = field(default=doot.constants.patterns.TASK_SEP, kw_only=True)
     version_constraint : None|str                = field(default=None)
+    meta               : TaskFlags               = field(default=TaskFlags.default)
     args               : dict                    = field(default_factory=dict)
 
     @classmethod
-    def from_str(cls, name:str, *, args=None):
-        if ":" in name:
-            try:
-                groupHead_r, taskHead_r = name.split("::")
-                groupHead = groupHead_r.split(".")
-                taskHead = taskHead_r.split(".")
-            except ValueError:
-                raise doot.errors.DootConfigError("Provided Task Name can't be split correctly, check it is of the form group::name", name)
-        else:
-            groupHead = None
-            taskHead  = name
+    def build(cls, name:str|dict|DootTaskName, *, args=None):
+        """ build a name from the various ways it can be specificed.
+          handles a single string of the group and taskname,
+          or a dict that specifies taskname and maybe the groupname
+
+        """
+        groupHead = []
+        taskHead  = []
+        match name:
+            case DootTaskName():
+                return name
+            case str() if doot.constants.patterns.TASK_SEP in name:
+                try:
+                    groupHead_r, taskHead_r = name.split(doot.constants.patterns.TASK_SEP)
+                    groupHead = groupHead_r.split(".")
+                    taskHead = taskHead_r.split(".")
+                except ValueError:
+                    raise doot.errors.DootConfigError("Provided Task Name can't be split correctly, check it is of the form group::name", name)
+            case str():
+                groupHead.append("default")
+                taskHead.append(name)
+            case {"name": str() as name} if doot.constants.patterns.TASK_SEP in name:
+                try:
+                    groupHead_r, taskHead_r = name.split(doot.constants.patterns.TASK_SEP)
+                    groupHead = groupHead_r.split(".")
+                    taskHead = taskHead_r.split(".")
+                except ValueError:
+                    raise doot.errors.DootConfigError("Provided Task Name can't be split correctly, check it is of the form group::name", name)
+            case { "group": str() as group, "name": str() as name }:
+                groupHead.append(group)
+                taskHead.append(name)
+            case {"name": str() as name}:
+                groupHead.append("default")
+                taskHead.append(name)
+            case {"name": DootTaskName() as name}:
+                return name
+            case _:
+                raise doot.errors.DootError("Unrecognized name format: %s", name)
+
+
         return DootTaskName(groupHead, taskHead, args=args)
 
     def __post_init__(self):
+        sub_split = ftz.partial(aware_splitter, sep=self.subseparator)
         match self.head:
             case ["tasks", x] if x.startswith('"') and x.endswith('"'):
-                self.head = ftz.reduce(lambda x, y: x + y, map(lambda x: x.split(self.subseparator), x[1:-1]))
+                self.head = ftz.reduce(lambda x, y: x + y, map(aware_splitter, x[1:-1]))
             case ["tasks", *xs]:
-                self.head = ftz.reduce(lambda x, y: x + y, map(lambda x: x.split(self.subseparator), xs))
+                self.head = ftz.reduce(lambda x, y: x + y, map(aware_splitter, xs))
             case list():
-                self.head = ftz.reduce(lambda x, y: x + y, map(lambda x: x.split(self.subseparator), self.head))
+                self.head = ftz.reduce(lambda x, y: x + y, map(aware_splitter, self.head))
             case str():
                 self.head = self.head.split(self.subseparator)
             case None | []:
                 self.head = ["default"]
 
         match self.tail:
             case list():
-                self.tail = ftz.reduce(lambda x, y: x + y, map(lambda x: x.split(self.subseparator), self.tail))
+                self.tail = ftz.reduce(lambda x, y: x + y, map(aware_splitter, self.tail))
             case str():
                 self.tail = self.tail.split(self.subseparator)
             case None | []:
                 self.tail = ["default"]
 
-        self.internal = self.tail[0].startswith(doot.constants.INTERNAL_TASK_PREFIX) or self.internal
+        if self.tail[0].startswith(doot.constants.patterns.INTERNAL_TASK_PREFIX):
+            self.meta |= TaskFlags.INTERNAL
 
     def __str__(self) -> str:
         return "{}{}{}".format(self.group, self.separator, self.task)
 
     def __repr__(self) -> str:
         name = str(self)
         return f"<TaskName: {name}>"
@@ -123,35 +154,47 @@
         if len(self.head) > 1:
             # fmt = "tasks.\"{}\""
             fmt = '"{}"'
         return fmt.format(self.head_str())
 
     @property
     def task(self) -> str:
-        return self.tail_str()
+        return self.subseparator.join([str(x) if not isinstance(x, UUID) else "${}$".format(x.hex) for x in self.tail])
+
+    @property
+    def readable(self):
+        group = self.group
+        tail = self.subseparator.join([str(x) if not isinstance(x, UUID) else "<UUID>" for x in self.tail])
+        return "{}{}{}".format(group, self.separator, tail)
 
-    def root(self):
-        return f"{self.head_str()}{self.separator}{self.tail[0]}"
+    def root(self) -> DootTaskName:
+        return DootTaskName.build(f"{self.head_str()}{self.separator}{self.tail[0]}")
+
+    def task_head(self):
+        return self.subtask(doot.constants.patterns.SUBTASKED_HEAD)
 
     def subtask(self, *subtasks, subgroups:list[str]|None=None) -> DootTaskName:
         args = self.args.copy() if self.args else None
         subs = []
-        match subtasks:
+        match [x for x in subtasks if x != None]:
             case [int() as i, DootTaskName() as x]:
                 subs.append(str(i))
                 subs.append(x.task.removeprefix(self.task + "."))
             case [str() as x]:
                 subs.append(x)
             case [*xs]:
-                subs = [str(x) for x in xs]
+                subs = xs
 
         return DootTaskName(self.head + (subgroups or []),
                             self.tail + subs,
-                            internal=self.internal,
+                            meta=self.meta,
                             args=args)
 
     def specialize(self, *, info=None):
         match info:
             case None:
-                return self.subtask(doot.constants.SPECIALIZED_ADD, "${}$".format(uuid1().hex))
+                return self.subtask(doot.constants.patterns.SPECIALIZED_ADD, uuid1())
             case _:
-                return self.subtask(doot.constants.SPECIALIZED_ADD, info, "${}$".format(uuid1().hex))
+                return self.subtask(doot.constants.patterns.SPECIALIZED_ADD, info, uuid1())
+
+    def last(self):
+        return self.tail[-1]
```

### Comparing `doot-0.6.1/doot/_structs/task_spec.py` & `doot-0.7.0/doot/_structs/task_spec.py`

 * *Files 11% similar despite different names*

```diff
@@ -35,171 +35,177 @@
 ##-- logging
 logging = logmod.getLogger(__name__)
 ##-- end logging
 
 import importlib
 from importlib.metadata import EntryPoint
 from tomlguard import TomlGuard
+import doot
 import doot.errors
-import doot.constants as consts
-from doot.enums import TaskFlags, ReportEnum
+from doot.enums import TaskFlags, ReportEnum, TaskQueueMeta
 from doot._structs.sname import DootTaskName, DootCodeReference
 from doot._structs.action_spec import DootActionSpec
 from doot._structs.artifact import DootTaskArtifact
+from doot._structs.toml_loc import TomlLocation
+from doot._abstract.structs import SpecStruct_p
 
 PAD           : Final[int] = 15
-TaskFlagNames : Final[str] = [x.name for x in TaskFlags]
 
-def _build_name(data) -> DootTaskName:
-    match data:
-        case {"group": group, "name": str() as name}:
-            return DootTaskName(data['group'], data['name'])
-        case {"name": str() as name}:
-            return DootTaskName.from_str(name)
-        case {"name": DootTaskName() as name}:
-            return name
-        case _:
-            return DootTaskName(None, None)
+# TODO: taskspec.setup, taskspec.cleanup, taskspec.on_fail
 
 def _separate_into_core_and_extra(data) -> tuple[dict, dict]:
     core_keys   = list(DootTaskSpec.__dataclass_fields__.keys())
     core_data, extra_data = dict(), dict()
     # Integrate extras, normalize keys
     for key, val in data.items():
         if "-" in key:
             key = key.replace("-","_")
         match key:
-            case "extra":
+            case "extra" if val is not None:
                 extra_data.update(dict(val))
+            case "extra":
+                pass
             case "print_levels":
                 core_data["print_levels"] = TomlGuard(val)
             case "active_when":
                 processed = _prepare_deps(val)
                 core_data["active_when"] = processed
             case "required_for":
                 processed = _prepare_deps(val)
                 core_data["required_for"] = processed
             case "depends_on":
                 processed = _prepare_deps(val)
                 core_data["depends_on"] = processed
+            case "setup":
+                processed = _prepare_deps(val)
+                core_data["setup"] = processed
+            case "cleanup":
+                processed = _prepare_deps(val)
+                core_data["cleanup"] = processed
+            case "on_fail":
+                processed = _prepare_deps(val)
+                core_data["on_fail"] = processed
+            case "queue_behaviour":
+                as_enum = TaskQueueMeta.build(val)
+                core_data["queue_behaviour"] = as_enum
             case x if x in core_keys:
                 core_data[x] = val
             case x if x not in ["name", "group"]:
                 extra_data[key] = val
 
     return core_data, extra_data
 
-def _valid_flag(x):
-    match x:
-        case str() if x in TaskFlagNames:
-            return True
-        case TaskFlags():
-            return True
-        case _:
-            return False
-
 def _prepare_deps(deps:None|list[str], source=None) -> list[DootTaskArtifact|DootTaskName]:
     """
       Prepares dependencies, converting from strings to Artifacts (ie:files), or Task Names
       # TODO handle callables?
     """
     if deps is None:
         return []
 
     results = []
     for x in deps:
         match x:
-            case { "task": taskname }:
-                results.append(DootTaskName.from_str(taskname, args=x))
-            case str() if x.startswith(consts.FILE_DEP_PREFIX):
-                results.append(DootTaskArtifact(pl.Path(x.removeprefix(consts.FILE_DEP_PREFIX))))
-            case str() if consts.TASK_SEP in x:
-                results.append(DootTaskName.from_str(x))
+            case { "do": action  }:
+                results.append(DootActionSpec.build(x))
+            case { "loc": filename }:
+                results.append(DootTaskArtifact.build(x))
+            case str() if x.startswith(doot.constants.patterns.FILE_DEP_PREFIX):
+                results.append(DootTaskArtifact.build(x))
+            case str() if doot.constants.patterns.TASK_SEP in x:
+                results.append(DootTaskName.build(x))
             case DootTaskName() | DootTaskArtifact():
                 results.append(x)
             case _:
-                raise doot.errors.DootInvalidConfig(f"Unrecognised task pre/post dependency form. (Remember: files are prefixed with `{consts.FILE_DEP_PREFIX}`, tasks are in the form group::name)", x, source)
+                raise doot.errors.DootInvalidConfig(f"Unrecognised task pre/post dependency form. (Remember: files are prefixed with `{doot.constants.patterns.FILE_DEP_PREFIX}`, tasks are in the form group::name)", x, source)
 
     return results
 
-def _prepare_ctor(ctor, mixins):
+def _prepare_ctor(ctor, mixins) -> DootTaskName|DootCodeReference:
     match ctor:
         case None:
-            return DootCodeReference.from_str(doot.constants.DEFAULT_PLUGINS['task'][0][1]).add_mixins(*mixins)
+
+            default_alias = doot.constants.entrypoints.DEFAULT_TASK_CTOR_ALIAS
+            coderef_str   = doot.aliases.task[default_alias]
+            return DootCodeReference.build(coderef_str).add_mixins(*mixins)
         case EntryPoint():
-            loaded = ctor.load()
-            return DootCodeReference.from_type(loaded).add_mixins(*mixins)
+            return DootCodeReference.build(ctor).add_mixins(*mixins)
         case DootTaskName() if bool(mixins):
             raise TypeError("Task name ctor can't take mixins")
         case DootTaskName():
             return ctor
         case DootCodeReference() if not bool(ctor._mixins):
             return ctor.add_mixins(*mixins)
         case DootCodeReference():
             return ctor
         case type():
-            return DootCodeReference.from_type(ctor).add_mixins(*mixins)
+            return DootCodeReference.build(ctor).add_mixins(*mixins)
         case str():
-            return DootCodeReference.from_str(ctor).add_mixins(*mixins)
+            return DootCodeReference.build(ctor).add_mixins(*mixins)
         case _:
-            return DootCodeReference.from_type(ctor).add_mixins(*mixins)
+            return DootCodeReference.build(ctor).add_mixins(*mixins)
 
 @dataclass
-class DootTaskSpec:
+class DootTaskSpec(SpecStruct_p):
     """ The information needed to describe a generic task.
     Optional things are shoved into 'extra', so things can use .on_fail on the tomlguard
 
     the cli parser can understand cli=[{}] specs
     actions                      : list[ [args] | {do="", args=[], **kwargs} ]
 
     """
-    name                         : DootTaskName                                                 = field()
-    doc                          : list[str]                                                    = field(default_factory=list)
-    source                       : DootTaskName|str|None                                        = field(default=None)
+    name                         : DootTaskName                                                            = field()
+    doc                          : list[str]                                                               = field(default_factory=list)
+    source                       : DootTaskName|str|None                                                   = field(default=None)
     actions                      : list[DootActionSpec]                                                    = field(default_factory=list)
 
-    active_when                  : list[DootTaskArtifact|callable]                              = field(default_factory=list)
-    required_for                 : list[DootTaskName|DootTaskArtifact]                          = field(default_factory=list)
-    depends_on                   : list[DootTaskName|DootTaskArtifact]                          = field(default_factory=list)
-    priority                     : int                                                          = field(default=10)
-    ctor                         : DootTaskName|DootCodeReference                               = field(default=None)
+    required_for                 : list[DootTaskName|DootTaskArtifact]                                     = field(default_factory=list)
+    depends_on                   : list[DootTaskName|DootTaskArtifact|DootActionSpec]                      = field(default_factory=list)
+    setup                        : list[DootTaskName|DootActionSpec]                                       = field(default_factory=list)
+    cleanup                      : list[DootTaskName|DootActionSpec]                                       = field(default_factory=list)
+    on_fail                      : list[DootTaskName|DootAcitonSpec]                                       = field(default_factory=list)
+    priority                     : int                                                                     = field(default=10)
+    ctor                         : DootTaskName|DootCodeReference                                          = field(default=None)
     # Any additional information:
-    version                      : str                                             = field(default="0.1")
-    # TODO version : dict = field(default_factory=dict)
-    print_levels                 : TomlGuard                                       = field(default_factory=TomlGuard)
-    flags                        : TaskFlags                                       = field(default=TaskFlags.TASK)
+    version                      : str                                                                     = field(default="0.1")
+    # TODO version               : dict                                                                    = field(default_factory=dict)
+    print_levels                 : TomlGuard                                                               = field(default_factory=TomlGuard)
+    flags                        : TaskFlags                                                               = field(default=TaskFlags.TASK)
 
-    extra                        : TomlGuard                                       = field(default_factory=TomlGuard)
+    extra                        : TomlGuard                                                               = field(default_factory=TomlGuard)
 
-    inject                       : list[str]                                       = field(default_factory=list) # For jobs
-    queue_behaviour              : str                                             = field(default="default")
+    inject                       : list[str]                                                               = field(default_factory=list) # For jobs
+    queue_behaviour              : TaskQueueMeta                                                 = field(default=TaskQueueMeta.default)
+
+    @staticmethod
+    def build(data:TomlGuard|dict|DootTaskName|str):
+        match data:
+            case TomlGuard() | dict():
+                return DootTaskSpec.from_dict(data)
+            case DootTaskName():
+                return DootTaskSpec.from_name(data)
+            case str():
+                return DootTaskSpec.from_name(DootTaskName.build(data))
 
     @staticmethod
     def from_dict(data:TomlGuard|dict):
         """ builds a task spec from a raw dict
           able to handle a name:str = "group::task" form,
           able to convert TaskFlag str's into an or'd enum value
           """
         core_data, extra_data = _separate_into_core_and_extra(data)
 
-        core_data['name'] = _build_name(data)
-
-        # Check flags are valid
-        if any(flag for x in data.get('flags', []) if (flag:=x) and not _valid_flag(flag)):
-            logging.warning("Unknown Task Flag used (%s), check the spec for %s in %s", flag, core_data['name'], data.get('source', ''))
-
-        filtered = filter(lambda x: x in TaskFlagNames, core_data.get('flags', ["TASK"]))
-        core_data['flags'] = ftz.reduce(lambda x,y: x|y, map(lambda x: TaskFlags[x],  filtered), TaskFlags.TASK)
+        core_data['name']     = DootTaskName.build(data)
+        core_data['flags']    = TaskFlags.build(core_data.get("flags", []))
 
         # Prepare constructor
-        mixins = extra_data.get("mixins", [])
-        core_data['ctor'] = _prepare_ctor(data.get("ctor",None), mixins)
+        core_data['ctor'] = _prepare_ctor(data.get("ctor",None), [])
 
         # prep actions
-        core_data['actions'] = [DootActionSpec.from_data(x) for x in core_data.get('actions', [])]
+        core_data['actions'] = [DootActionSpec.build(x) for x in core_data.get('actions', [])]
 
         task = DootTaskSpec(**core_data, extra=TomlGuard(extra_data))
         return task
 
     @staticmethod
     def from_name(name:DootTaskName):
         match name:
@@ -252,22 +258,31 @@
                         case x, _MISSING_TYPE(), _:
                             value = getattr(self, field)
                         case x, y, z:
                             raise TypeError("Unknown Task Spec Specialization field types", field, x, y, z)
 
                     specialized[field] = value
 
-        logging.debug("Specialized Task: %s on top of: %s", data.name, self.name)
-        return DootTaskSpec.from_dict(specialized)
+        logging.debug("Specialized Task: %s on top of: %s", data.name.readable, self.name)
+        return DootTaskSpec.build(specialized)
 
-    def build(self, ensure=Any):
+    def make(self, ensure=Any) -> Task_i:
+        """ Create actual task instance """
         task_ctor = self.ctor.try_import(ensure=ensure)
         return task_ctor(self)
 
     def check(self, ensure=Any):
         if self.ctor.module == "default":
             return True
         self.ctor.try_import(ensure=ensure)
         return True
 
     def __hash__(self):
         return hash(str(self.name))
+
+    @property
+    def params(self):
+        return self.extra
+
+    @property
+    def action_groups(self):
+        return [self.depends_on, self.setup, self.actions, self.cleanup, self.on_fail]
```

### Comparing `doot-0.6.1/doot/_structs/trace.py` & `doot-0.7.0/doot/_structs/trace.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,15 +35,14 @@
 ##-- logging
 logging = logmod.getLogger(__name__)
 ##-- end logging
 
 import importlib
 from tomlguard import TomlGuard
 import doot.errors
-import doot.constants
 from doot.enums import TaskFlags, ReportEnum
 
 PAD           : Final[int] = 15
 TaskFlagNames : Final[str] = [x.name for x in TaskFlags]
 
 @dataclass
 class DootTraceRecord:
@@ -65,11 +64,7 @@
         return all([x in self.flags for x in other])
 
     def __eq__(self, other:ReportEnum) -> bool:
         return self.flags == other
 
     def some(self, other:reportPositionEnum) -> bool:
         return any([x in self.flags for x in other])
-
-"""
-
-"""
```

### Comparing `doot-0.6.1/doot/actions/__tests/test_base_action.py` & `doot-0.7.0/doot/actions/__tests/test_io.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,17 +14,18 @@
 import os
 
 logging = logmod.root
 
 import pytest
 
 import doot
+doot._test_setup()
+
 import doot._abstract
 import doot.structs
-import doot.constants
 from doot.task.base_task import DootTask
 from doot.actions.base_action import DootBaseAction
 
 ##-- pytest reminder
 # caplog
 # mocker.patch | patch.object | patch.multiple | patch.dict | stopall | stop | spy | stub
 # pytest.mark.filterwarnings
```

### Comparing `doot-0.6.1/doot/actions/__tests/test_control_flow.py` & `doot-0.7.0/doot/actions/__tests/test_postbox.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,17 +14,18 @@
 import os
 
 logging = logmod.root
 
 import pytest
 
 import doot
+doot._test_setup()
+
 import doot._abstract
 import doot.structs
-import doot.constants
 from doot.task.base_task import DootTask
 from doot.actions.base_action import DootBaseAction
 
 ##-- pytest reminder
 # caplog
 # mocker.patch | patch.object | patch.multiple | patch.dict | stopall | stop | spy | stub
 # pytest.mark.filterwarnings
```

### Comparing `doot-0.6.1/doot/actions/__tests/test_io.py` & `doot-0.7.0/doot/actions/__tests/test_shell.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,17 +14,18 @@
 import os
 
 logging = logmod.root
 
 import pytest
 
 import doot
+doot._test_setup()
+
 import doot._abstract
 import doot.structs
-import doot.constants
 from doot.task.base_task import DootTask
 from doot.actions.base_action import DootBaseAction
 
 ##-- pytest reminder
 # caplog
 # mocker.patch | patch.object | patch.multiple | patch.dict | stopall | stop | spy | stub
 # pytest.mark.filterwarnings
```

### Comparing `doot-0.6.1/doot/actions/__tests/test_postbox.py` & `doot-0.7.0/doot/actions/__tests/test_state.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,17 +14,18 @@
 import os
 
 logging = logmod.root
 
 import pytest
 
 import doot
+doot._test_setup()
+
 import doot._abstract
 import doot.structs
-import doot.constants
 from doot.task.base_task import DootTask
 from doot.actions.base_action import DootBaseAction
 
 ##-- pytest reminder
 # caplog
 # mocker.patch | patch.object | patch.multiple | patch.dict | stopall | stop | spy | stub
 # pytest.mark.filterwarnings
```

### Comparing `doot-0.6.1/doot/actions/base_action.py` & `doot-0.7.0/doot/actions/base_action.py`

 * *Files 14% similar despite different names*

```diff
@@ -25,23 +25,25 @@
 
 printer = logmod.getLogger("doot._printer")
 
 import doot
 from doot.errors import DootTaskError, DootTaskFailed
 from doot.structs import DootActionSpec
 from doot._abstract import Action_p
+from doot.enums import ActionResponseEnum
 
-@doot.check_protocol
 class DootBaseAction(Action_p):
     """
     The basic action, which just prints that the action was called
     Subclass this and override __call__ for your own actions.
     The arguments of the action are held in the passed in spec
     __call__ is passed a *copy* of the task's state dictionary
     """
+    ActRE = ActionResponseEnum
+
 
     def __str__(self):
         return f"Base Action"
 
     def __call__(self, spec:DootActionSpec, state:dict) -> dict|bool|None:
         printer.debug("Base Action Called: %s", state.get("count", 0))
         printer.info(" ".join(spec.args))
```

### Comparing `doot-0.6.1/doot/actions/compression.py` & `doot-0.7.0/doot/actions/compression.py`

 * *Files 24% similar despite different names*

```diff
@@ -44,90 +44,128 @@
 import tomlguard as TG
 import doot
 from doot.errors import DootTaskError, DootTaskFailed
 from doot.enums import ActionResponseEnum
 from doot._abstract import Action_p
 from doot.structs import DootKey
 from doot.actions.postbox import _DootPostBox
+from doot.mixins.zipper import Zipper_m
 
 ##-- expansion keys
-TO_KEY             : Final[DootKey] = DootKey.make("to")
-FROM_KEY           : Final[DootKey] = DootKey.make("from")
-UPDATE             : Final[DootKey] = DootKey.make("update_")
-PROMPT             : Final[DootKey] = DootKey.make("prompt")
-PATTERN            : Final[DootKey] = DootKey.make("pattern")
-SEP                : Final[DootKey] = DootKey.make("sep")
-TYPE_KEY           : Final[DootKey] = DootKey.make("type")
-AS_BYTES           : Final[DootKey] = DootKey.make("as_bytes")
-FILE_TARGET        : Final[DootKey] = DootKey.make("file")
-RECURSIVE          : Final[DootKey] = DootKey.make("recursive")
-LAX                : Final[DootKey] = DootKey.make("lax")
+TO_KEY             : Final[DootKey] = DootKey.build("to")
+FROM_KEY           : Final[DootKey] = DootKey.build("from")
+UPDATE             : Final[DootKey] = DootKey.build("update_")
+PROMPT             : Final[DootKey] = DootKey.build("prompt")
+PATTERN            : Final[DootKey] = DootKey.build("pattern")
+SEP                : Final[DootKey] = DootKey.build("sep")
+TYPE_KEY           : Final[DootKey] = DootKey.build("type")
+AS_BYTES           : Final[DootKey] = DootKey.build("as_bytes")
+FILE_TARGET        : Final[DootKey] = DootKey.build("file")
+RECURSIVE          : Final[DootKey] = DootKey.build("recursive")
+LAX                : Final[DootKey] = DootKey.build("lax")
 ##-- end expansion keys
 
 COMP_TAR_CMD  = sh.tar.bake("-cf", "-")
 COMP_GZIP_CMD = sh.gzip.bake("--best")
 DECOMP_CMD    = sh.tar.bake("-xf")
 
-@doot.check_protocol
 class TarCompressAction(Action_p):
     """ Compresses a target into a .tar.gz file """
 
-    @DootKey.kwrap.paths("file")
-    @DootKey.kwrap.paths("to", hint={"on_fail":None})
+    @DootKey.dec.paths("file")
+    @DootKey.dec.paths("to", hint={"on_fail":None})
     def __call__(self, spec, state, file, to):
         target = file
         output = to or target.with_suffix(target.suffix + ".tar.gz")
 
         if output.exists():
             raise doot.errors.DootActionError("Compression target already exists")
         if target.is_dir():
             COMP_GZIP_CMD(_in=COMP_TAR_CMD("-C", target, ".", _piped=True), _out=output)
         else:
             COMP_GZIP_CMD(_in=COMP_TAR_CMD("-C", target.parent, target.name, _piped=True), _out=output)
 
-@doot.check_protocol
 class TarDecompressAction(Action_p):
     """ Decompresses a .tar.gz file """
 
-    @DootKey.kwrap.paths("file", "to")
+    @DootKey.dec.paths("file", "to")
     def __call__(self, spec, state, file, to):
         target = file
         output = to
         if not ".tar.gz" in target.name:
             printer.warning("Decompression target isn't a .tar.gz", target)
             return ActionResponseEnum.FAIL
 
         DECOMP_CMD(target, "-C", output)
 
 
-@doot.check_protocol
 class TarListAction(Action_p):
     """ List the contents of a tar archive """
 
-    @DootKey.kwrap.paths("from")
-    @DootKey.kwrap.redirects("update_")
+    @DootKey.dec.paths("from")
+    @DootKey.dec.redirects("update_")
     def __call__(self, spec, state, _from, _update):
         target = _from
         if "".join(target.suffixes) != ".tar.gz":
             printer.warning("Trying to list the contents of a non-tar archive")
             return ActionResponseEnum.FAIL
 
         result = sh.tar("--list", "-f", str(target))
         lines = result.split("\n")
         return { _update : lines }
 
 
-class ZipNewAction(Action_p):
+class ZipNewAction(Zipper_m, Action_p):
     """ Make a new zip archive """
-    pass
 
-class ZipAddAction(Action_p):
+    @DootKey.dec.paths("target")
+    def __call__(self, spec, state, target):
+         self.zip_create(target)
+
+
+class ZipAddAction(Zipper_m, Action_p):
     """ Add a file/directory to a zip archive """
-    pass
 
-class ZipGetAction(Action_p):
+    @DootKey.dec.paths("target")
+    @DootKey.dec.args
+    def __call__(self, spec, state, target, args):
+        arg_paths = []
+        for str in args:
+            key = DootKey.build(x)
+            match key.to_path(spec, state, on_fail=None):
+                case pl.Path() as x if not x.exists():
+                    printer.warning("Can't add non-existent path to zip: %s", key)
+                case pl.Path() as x:
+                    arg_paths.append(x)
+                case _:
+                    printer.warning("Can't add non-expandable path to zip: %s", key)
+
+        self.zip_add_paths(target, *arg_paths)
+
+
+class ZipGetAction(Zipper_m, Action_p):
     """ unpack a file/files/all files from a zip archive """
-    pass
+
+    @DootKey.dec.paths("zipf", "target")
+    def __call__(self, spec, state, zipf:pl.Path, target:pl.Path):
+        if target.is_file():
+            raise doot.errors.DootActionError("Can't unzip to a file: %s", target)
+
+        self.zip_unzip_to(target, zipf)
+
 
 class ZipListAction(Action_p):
     """ List the contents of a zip archive """
-    pass
+
+    @DootKey.dec.paths("target")
+    @DootKey.dec.redirects("update_")
+    def __call__(self, spec, state, target:pl.Path, _update):
+        contents = self.zip_get_contents(target)
+        printer.info("Contents of Zip File: %s", target)
+        for x in contents:
+            printer.info("- %s", x)
+        printer.info("--")
+
+        if _update == "update_":
+            return
+
+        return { _update : contents }
```

### Comparing `doot-0.6.1/doot/actions/io.py` & `doot-0.7.0/doot/actions/io.py`

 * *Files 9% similar despite different names*

```diff
@@ -29,77 +29,77 @@
 from time import sleep
 import sh
 import shutil
 import tomlguard as TG
 import doot
 from doot.errors import DootTaskError, DootTaskFailed
 from doot.enums import ActionResponseEnum
-from doot._abstract import Action_p
+from doot.mixins.path_manip import PathManip_m
 from doot.structs import DootKey
 from doot.actions.postbox import _DootPostBox
+from doot.utils.decorators import IOWriter
 
 # TODO using doot.config.settings.general.protect to disallow write/delete/backup/copy
 
 ##-- expansion keys
-TO_KEY             : Final[DootKey] = DootKey.make("to")
-FROM_KEY           : Final[DootKey] = DootKey.make("from")
-UPDATE             : Final[DootKey] = DootKey.make("update_")
-PROMPT             : Final[DootKey] = DootKey.make("prompt")
-PATTERN            : Final[DootKey] = DootKey.make("pattern")
-SEP                : Final[DootKey] = DootKey.make("sep")
-TYPE_KEY           : Final[DootKey] = DootKey.make("type")
-AS_BYTES           : Final[DootKey] = DootKey.make("as_bytes")
-FILE_TARGET        : Final[DootKey] = DootKey.make("file")
-RECURSIVE          : Final[DootKey] = DootKey.make("recursive")
-LAX                : Final[DootKey] = DootKey.make("lax")
+TO_KEY             : Final[DootKey] = DootKey.build("to")
+FROM_KEY           : Final[DootKey] = DootKey.build("from")
+UPDATE             : Final[DootKey] = DootKey.build("update_")
+PROMPT             : Final[DootKey] = DootKey.build("prompt")
+PATTERN            : Final[DootKey] = DootKey.build("pattern")
+SEP                : Final[DootKey] = DootKey.build("sep")
+TYPE_KEY           : Final[DootKey] = DootKey.build("type")
+AS_BYTES           : Final[DootKey] = DootKey.build("as_bytes")
+FILE_TARGET        : Final[DootKey] = DootKey.build("file")
+RECURSIVE          : Final[DootKey] = DootKey.build("recursive")
+LAX                : Final[DootKey] = DootKey.build("lax")
 ##-- end expansion keys
 
 
-@doot.check_protocol
-class AppendAction(Action_p):
+class AppendAction(PathManip_m):
     """
       Pre/Ap-pend data from the state to a file
     """
     sep = "\n--------------------\n"
 
-    @DootKey.kwrap.args
-    @DootKey.kwrap.types("sep", hint={"on_fail":None})
-    @DootKey.kwrap.paths("to")
+    @DootKey.dec.args
+    @DootKey.dec.types("sep", hint={"on_fail":None})
+    @DootKey.dec.paths("to")
     def __call__(self, spec, state, args, sep, to):
         sep          = sep or AppendAction.sep
         loc          = to
-        args_keys    = [DootKey.make(x, explicit=True) for x in args]
+        args_keys    = [DootKey.build(x, explicit=True) for x in args]
         exp_args     = [k.expand(spec, state, insist=True, on_fail=None) for k in args_keys]
 
-        if not doot.locs.check_writable(loc):
+        if self._is_write_protected(loc):
             raise doot.errors.DootLocationError("Tried to write a protected location", loc)
 
         with open(loc, 'a') as f:
             for arg in exp_args:
                 if not arg:
                     continue
 
                 printer.info("Appending %s chars to %s", len(arg), loc)
                 f.write(sep)
                 f.write(arg)
 
-@doot.check_protocol
-class WriteAction(Action_p):
+@IOWriter()
+class WriteAction(PathManip_m):
     """
       Writes data from the state to a file, accessed through the
       doot.locs object
     """
 
-    @DootKey.kwrap.types("from")
-    @DootKey.kwrap.paths("to")
+    @DootKey.dec.types("from")
+    @DootKey.dec.paths("to")
     def __call__(self, spec, state, _from, to) -> dict|bool|None:
         data = _from
         loc  = to
 
-        if not doot.locs.check_writable(loc):
+        if self._is_write_protected(loc):
             raise doot.errors.DootLocationError("Tried to write a protected location", loc)
 
         match data:
             case None:
                 printer.info("No Data to Write")
             case _ if not bool(data):
                 printer.info("No Data to Write")
@@ -109,27 +109,30 @@
                 loc.write_text(text)
             case bytes():
                 printer.info("Writing %s bytes to %s", len(data), loc)
                 loc.write_bytes(data)
             case str():
                 printer.info("Writing %s chars to %s", len(data), loc)
                 loc.write_text(data)
+            case _:
+                as_str = str(data)
+                printer.info("Writing %s chars to %s", len(as_str), loc)
+                loc.write_text(as_str)
 
 
 
-@doot.check_protocol
-class ReadAction(Action_p):
+class ReadAction(PathManip_m):
     """
       Reads data from the doot.locs location to  return for the state
       The arguments of the action are held in self.spec
     """
-    @DootKey.kwrap.paths("from")
-    @DootKey.kwrap.redirects("update_")
-    @DootKey.kwrap.types("as_bytes", hint={"on_fail":False})
-    @DootKey.kwrap.types("type", hint={"type_":str, "on_fail":"read"})
+    @DootKey.dec.paths("from")
+    @DootKey.dec.redirects("update_")
+    @DootKey.dec.types("as_bytes", hint={"on_fail":False})
+    @DootKey.dec.types("type", hint={"type_":str, "on_fail":"read"})
     def __call__(self, spec, state, _from, _update, as_bytes, _type) -> dict|bool|None:
         loc = _from
         read_binary = as_bytes
         read_lines  = _type
         printer.info("Reading from %s into %s", loc, _update)
         if read_binary:
             with open(loc, "rb") as f:
@@ -141,176 +144,173 @@
                     return { _update : f.read() }
                 case "lines":
                     return { _update : f.readlines() }
                 case unk:
                     raise TypeError("Unknown read type", unk)
 
 
-@doot.check_protocol
-class CopyAction(Action_p):
+class CopyAction(PathManip_m):
     """
       copy a file somewhere
       The arguments of the action are held in self.spec
     """
 
-    @DootKey.kwrap.types("from", hint={"type_":str|pl.Path|list})
-    @DootKey.kwrap.paths("to")
+    @DootKey.dec.types("from", hint={"type_":str|pl.Path|list})
+    @DootKey.dec.paths("to")
     def __call__(self, spec, state, _from, to) -> dict|bool|None:
         dest_loc   = to
         match _from:
             case str() | pl.Path():
-                expanded = [DootKey.make(_from, strict=False).to_path(spec, state)]
+                expanded = [DootKey.build(_from, strict=False).to_path(spec, state)]
             case list():
-                expanded = list(map(lambda x: DootKey.make(x, strict=False).to_path(spec, state), _from))
+                expanded = list(map(lambda x: DootKey.build(x, strict=False).to_path(spec, state), _from))
             case _:
                 raise doot.errors.DootActionError("Unrecognized type for copy sources", _from)
 
 
-        if not all(doot.locs.check_writable(x) for x in expanded):
-            raise doot.errors.DootLocationError("Tried to write a protected location", expanded)
+        if any(self._is_write_protected(x) for x in expanded):
+            raise doot.errors.DootLocationError("Tried to write a protected location", x)
         if any(not x.exists() for x in expanded):
             raise doot.errors.DootActionError("Tried to copy a file that doesn't exist")
         if any((dest_loc/x.name).exists() for x in expanded):
             raise doot.errors.DootActionError("Tried to copy a file that already exists at the destination")
         if len(expanded) > 1 and not dest_loc.is_dir():
             raise doot.errors.DootActionError("Tried to copy multiple files to a non-directory")
 
         for arg in expanded:
             shutil.copy2(arg, dest_loc)
 
-@doot.check_protocol
-class MoveAction(Action_p):
+class MoveAction(PathManip_m):
     """
       move a file somewhere
       The arguments of the action are held in self.spec
     """
 
-    @DootKey.kwrap.paths("from", "to")
+    @DootKey.dec.paths("from", "to")
     def __call__(self, spec, state, _from, to) -> dict|bool|None:
         source     = _from
         dest_loc   = to
 
-        if not doot.locs.check_writable(dest_loc):
+        if self._is_write_protected(dest_loc):
             raise doot.errors.DootLocationError("Tried to write a protected location", dest_loc)
         if not source.exists():
             raise doot.errors.DootActionError("Tried to move a file that doesn't exist", source)
         if dest_loc.exists():
             raise doot.errors.DootActionError("Tried to move a file that already exists at the destination", dest_loc)
         if source.is_dir():
             raise doot.errors.DootActionError("Tried to move multiple files to a non-directory", source)
 
         source.rename(dest_loc)
 
-@doot.check_protocol
-class DeleteAction(Action_p):
+class DeleteAction(PathManip_m):
     """
       delete a file / directory specified in spec.args
     """
-    @DootKey.kwrap.types("recursive", "lax", hint={"type_":bool, "on_fail":False})
+    @DootKey.dec.types("recursive", "lax", hint={"type_":bool, "on_fail":False})
     def __call__(self, spec, state, recursive, lax):
         rec = recursive
         for arg in spec.args:
-            loc = DootKey.make(arg, explicit=True).to_path(spec, state)
-            if not doot.locs.check_writable(loc):
-                raise doot.errors.DootLocationError("Tried to delete a protected location", loc)
+            loc = DootKey.build(arg, explicit=True).to_path(spec, state)
+            if self._is_write_protected(loc):
+                raise doot.errors.DootLocationError("Tried to write a protected location", loc)
+
+            if not loc.exists():
+                printer.info("Not Deleting Due to non-existence: %s", loc)
+                continue
 
-            printer.info("Deleting %s", loc)
             if loc.is_dir() and rec:
+                printer.info("Deleting Directory: %s", loc)
                 shutil.rmtree(loc)
             else:
+                printer.info("Deleting File: %s", loc)
                 loc.unlink(missing_ok=lax)
 
 
-@doot.check_protocol
-class BackupAction(Action_p):
+class BackupAction(PathManip_m):
     """
       copy a file somewhere, but only if it doesn't exist at the dest, or is newer than the dest
       The arguments of the action are held in self.spec
     """
 
-    @DootKey.kwrap.paths("from", "to")
-    def __call__(self, spec, state, _from, to) -> dict|bool|None:
+    @DootKey.dec.paths("from", "to")
+    @DootKey.dec.taskname
+    def __call__(self, spec, state, _from, to, _name) -> dict|bool|None:
         source_loc = _from
         dest_loc   = to
 
-        if not doot.locs.check_writable(dest_loc):
+        if self._is_write_protected(dest_loc):
             raise doot.errors.DootLocationError("Tried to write a protected location", dest_loc)
 
         if dest_loc.exists() and source_loc.stat().st_mtime_ns <= dest_loc.stat().st_mtime_ns:
             return True
 
         printer.warning("Backing up : %s", source_loc)
         printer.warning("Destination: %s", dest_loc)
-        _DootPostBox.put_from(state, dest_loc)
+        _DootPostBox.put(_name, dest_loc)
         shutil.copy2(source_loc,dest_loc)
 
 
-@doot.check_protocol
-class EnsureDirectory(Action_p):
+class EnsureDirectory(PathManip_m):
     """
       ensure the directories passed as arguments exist
       if they don't, build them
     """
 
-    @DootKey.kwrap.args
+    @DootKey.dec.args
     def __call__(self, spec, state, args):
         for arg in args:
-            loc = DootKey.make(arg, explicit=True).to_path(spec, state)
+            loc = DootKey.build(arg, explicit=True).to_path(spec, state)
             if not loc.exists():
                 printer.info("Building Directory: %s", loc)
             loc.mkdir(parents=True, exist_ok=True)
 
 
-@doot.check_protocol
-class UserInput(Action_p):
+class UserInput(PathManip_m):
 
-    @DootKey.kwrap.types("prompt", hint={"type_":str, "on_fail":"?::- "})
-    @DootKey.kwrap.redirects("update_")
+    @DootKey.dec.types("prompt", hint={"type_":str, "on_fail":"?::- "})
+    @DootKey.dec.redirects("update_")
     def __call__(self, spec, state, prompt, _update):
         result = input(prompt)
         return { _update : result }
 
 
-@doot.check_protocol
-class SimpleFind(Action_p):
+class SimpleFind(PathManip_m):
     """
     A Simple glob on a path
     """
 
-    @DootKey.kwrap.paths("from")
-    @DootKey.kwrap.types("rec", hint={"on_fail":False})
-    @DootKey.kwrap.expands("pattern")
-    @DootKey.kwrap.redirects("update_")
+    @DootKey.dec.paths("from")
+    @DootKey.dec.types("rec", hint={"on_fail":False})
+    @DootKey.dec.expands("pattern")
+    @DootKey.dec.redirects("update_")
     def __call__(self, spec, state, _from, rec, pattern, _update):
         from_loc = _from
         match rec:
             case True:
                 return { _update : list(from_loc.rglob(pattern)) }
             case False:
                 return { _update : list(from_loc.glob(pattern)) }
 
 
-@doot.check_protocol
-class TouchFileAction(Action_p):
+class TouchFileAction(PathManip_m):
 
-    @DootKey.kwrap.args
+    @DootKey.dec.args
     def __call__(self, spec, state, args):
-        for target in [DootKey.make(x, exp_hint="path") for x in args]:
+        for target in [DootKey.build(x, exp_hint="path") for x in args]:
             target(spec, state).touch()
 
 
-@doot.check_protocol
-class LinkAction(Action_p):
+class LinkAction(PathManip_m):
     """
       for x,y in spec.args:
       x.to_path().symlink_to(y.to_path())
     """
-    @DootKey.kwrap.paths("link", "to", hint={"on_fail":None})
-    @DootKey.kwrap.args
-    @DootKey.kwrap.types("force", hint={"type_":bool, "on_fail":False})
+    @DootKey.dec.paths("link", "to", hint={"on_fail":None})
+    @DootKey.dec.args
+    @DootKey.dec.types("force", hint={"type_":bool, "on_fail":False})
     def __call__(self, spec, state, link, to, args, force):
         if link is not None and to is not None:
             self._do_link(spec, state, spec.kwargs.link, spec.kwargs.to, force)
 
         for arg in spec.args:
             match arg:
                 case [x,y]:
@@ -321,16 +321,16 @@
                     self._do_link(spec, state, x,y, force)
                 case {"from":x, "to_rel":y}:
                     raise NotImplementedError()
                 case _:
                     raise TypeError("unrecognized link targets")
 
     def _do_link(self, spec, state, x, y, force):
-        x_key  = DootKey.make(x, explicit=True)
-        y_key  = DootKey.make(y, explicit=True)
+        x_key  = DootKey.build(x, explicit=True)
+        y_key  = DootKey.build(y, explicit=True)
         x_path = x_key.to_path(spec, state, symlinks=True)
         y_path = y_key.to_path(spec, state)
         # TODO when py3.12: use follow_symlinks=False
         if (x_path.exists() or x_path.is_symlink()) and not force:
             printer.warning("SKIP: A Symlink already exists: %s -> %s", x_path, x_path.resolve())
             return
         if not y_path.exists():
@@ -338,20 +338,19 @@
         if force and x_path.is_symlink():
             printer.warning("Forcing New Symlink")
             x_path.unlink()
         printer.info("Linking: %s -> %s", x_path, y_path)
         x_path.symlink_to(y_path)
 
 
-@doot.check_protocol
-class ListFiles(Action_p):
+class ListFiles(PathManip_m):
     """ add a list of all files in a path (recursively) to the state """
 
-    @DootKey.kwrap.paths("from")
-    @DootKey.kwrap.redirects("update_")
+    @DootKey.dec.paths("from")
+    @DootKey.dec.redirects("update_")
     def __call__(self, spec, state, _from, _update):
         target = _from
         base   = target.parent
         target = target.name
         result = sh.fdfind("--color", "never", "-t", "f", "--base-directory",  str(base), ".", target, _return_cmd=True)
         filelist = result.stdout.decode().split("\n")
```

### Comparing `doot-0.6.1/doot/actions/json.py` & `doot-0.7.0/doot/utils/retrievers.py`

 * *Files 20% similar despite different names*

```diff
@@ -31,61 +31,37 @@
 
 ##-- lib imports
 import more_itertools as mitz
 ##-- end lib imports
 
 ##-- logging
 logging = logmod.getLogger(__name__)
-##-- end logging
-
 printer = logmod.getLogger("doot._printer")
+##-- end logging
 
-import json
-from time import sleep
-import sh
-import shutil
-import tomlguard as TG
 import doot
-from doot.errors import DootTaskError, DootTaskFailed
-from doot.enums import ActionResponseEnum
-from doot._abstract import Action_p
 from doot.structs import DootKey
 
-
-##-- expansion keys
-FROM_KEY           : Final[DootKey] = DootKey.make("from")
-UPDATE             : Final[DootKey] = DootKey.make("update_")
-##-- end expansion keys
-
-@doot.check_protocol
-class ReadJson(Action_p):
-    """
-        Read a .json file and add it to the task state
+def id_retriever(spec, state) -> list[dict]:
+    """ A Null retriever, retruns to dicts to create subtasks from """
+    return []
+
+@DootKey.dec.types("files", "exts")
+def cli_retriever(spec, state, files, exts):
+    """ A CLI retriever, eg: for pre-commit.
+      gets the cli arg list "files", and makes a dict that can be used with
+      file processors like what walkers use, filtering by extension
     """
-    _toml_kwargs = [FROM_KEY, UPDATE]
-
-    @DootKey.kwrap.paths("from")
-    @DootKey.kwrap.redirects("update_")
-    def __call__(self, spec, state, _from, _update):
-        fpath    = _from
-        with open(fpath) as fp:
-            data     = json.load(fp)
-        return { _update : TG.TomlGuard(data) }
-
-class ParseJson(Action_p):
-    """ parse a string as json """
-    pass
-
-class ReadJsonLines(Action_p):
-    """ read a .jsonl file, or some of it, and add it to the task state  """
-
-    pass
-
-class WriteJsonLines(Action_p):
-    """ Write a list of dicts as a .jsonl file
-      optionally gzip the file
-      """
-    pass
-
-class WriteJson(Action_p):
-    """ Write a dict as a .json file  """
-    pass
+    root = doot.locs["."]
+    printer.info("CLI Retrieval Testing: %s", files)
+    for x in files:
+        fpath = doot.locs[x]
+        if fpath.suffix not in exts:
+            continue
+
+        lpath = fpath.relative_to(root)
+        yield dict(name=fpath.stem,
+                   fpath=fpath,
+                   fstem=fpath.stem,
+                   fname=fpath.name,
+                   lpath=lpath,
+                   pstem=fpath.parent.stem)
```

### Comparing `doot-0.6.1/doot/actions/postbox.py` & `doot-0.7.0/doot/actions/postbox.py`

 * *Files 12% similar despite different names*

```diff
@@ -29,149 +29,143 @@
 
 from collections import defaultdict
 from time import sleep
 import sh
 import doot
 from doot.errors import DootTaskError, DootTaskFailed
 from doot._abstract import Action_p
-from doot.structs import DootKey
+from doot.structs import DootKey, DootTaskName
 
 printer = logmod.getLogger("doot._printer")
+STATE_TASK_NAME_K : Final[str] = doot.constants.patterns.STATE_TASK_NAME_K
 
 ##-- expansion keys
-FROM_KEY    : Final[DootKey] = DootKey.make("from")
-UPDATE      : Final[DootKey] = DootKey.make("update_")
-TASK_NAME   : Final[DootKey] = DootKey.make("_task_name")
-SUBKEY      : Final[DootKey] = DootKey.make("subkey")
+UPDATE      : Final[DootKey] = DootKey.build("update_")
+TASK_NAME   : Final[DootKey] = DootKey.build(STATE_TASK_NAME_K)
+SUBKEY      : Final[DootKey] = DootKey.build("subkey")
 ##-- end expansion keys
 
 class _DootPostBox:
     """
       Internal Postbox class.
       holds a static variable of `boxes`, which maps task roots -> unique postbox
       Postboxes are lists, values are appended to it
     """
 
     boxes : ClassVar[dict[str,list[Any]]] = defaultdict(lambda: defaultdict(list))
     default_subkey                        = "_default"
 
     @staticmethod
-    def put(key, val, subkey=None):
-        subkey = subkey or _DootPostBox.default_subkey
+    def put(key:DootTaskName, val):
+        subbox = str(key.last())
+        box    = str(key.root())
         match val:
             case None | [] | {} | dict() if not bool(val):
                 pass
             case list() | set():
-                _DootPostBox.boxes[key][subkey] += val
+                _DootPostBox.boxes[box][subbox] += val
             case _:
-                _DootPostBox.boxes[key][subkey].append(val)
+                _DootPostBox.boxes[box][subbox].append(val)
 
     @staticmethod
-    def put_from(state, val, subkey=None):
-        """
-        utility to add to a postbox using the state, instead of calculating the root yourself
-        """
-        key    = TASK_NAME.to_type(None, state).root()
-        subkey = subkey or _DootPostBox.default_subkey
-        _DootPostBox.put(key, val, subkey=subkey)
-
-    @staticmethod
-    def get(key, subkey=Any) -> list:
-        match subkey:
+    def get(key:DootTaskName, subkey=Any) -> list|dict:
+        box    = str(key.root())
+        subbox = str(key.last())
+        match subbox:
             case "" | "-":
-                return _DootPostBox.boxes[key][_DootPostBox.default_subkey][:]
+                return _DootPostBox.boxes[box][_DootPostBox.default_subkey][:]
             case x if x == Any:
-                return _DootPostBox.boxes[key][_DootPostBox.default_subkey][:]
+                return _DootPostBox.boxes[box][_DootPostBox.default_subkey][:]
             case "*" | None:
-                return _DootPostBox.boxes[key].copy()
+                return _DootPostBox.boxes[box].copy()
             case _:
-                return _DootPostBox.boxes[key][subkey]
+                return _DootPostBox.boxes[box][subbox]
 
     @staticmethod
-    def clear_box(key, subkey=Any):
-        match subkey:
+    def clear_box(key):
+        box    = str(key.root())
+        subbox = str(key.last())
+        match subbox:
             case x if x == Any:
-                _DootPostBox.boxes[key][_DootPostBox.default_subkey] = []
-            case None:
-                _DootPostBox.boxes[key] = defaultdict(list)
+                _DootPostBox.boxes[box][_DootPostBox.default_subkey] = []
+            case False:
+                _DootPostBox.boxes[box] = defaultdict(list)
             case _:
-                _DootPostBox.boxes[key][subkey] = []
+                _DootPostBox.boxes[box][subkey] = []
 
-@doot.check_protocol
 class PutPostAction(Action_p):
     """
     push data to the inter-task postbox of this task tree
     The arguments of the action are held in self.spec
     'args' are pushed to the default subbox
-    'kwargs' are pushed to the kwarg subbox
+    'kwargs' are pushed to the kwarg specific subbox
+
+    eg: {do="post.put", args=["{key}", "{key}"], subbox="{key}"}
     """
 
-    @DootKey.kwrap.args
-    @DootKey.kwrap.kwargs
-    def __call__(self, spec, state, args, kwargs) -> dict|bool|None:
-        target = TASK_NAME.to_type(spec, state).root()
+    @DootKey.dec.args
+    @DootKey.dec.kwargs
+    @DootKey.dec.taskname
+    def __call__(self, spec, state, args, kwargs, _basename) -> dict|bool|None:
+        target = _basename.root().subtask(_DootPostBox.default_subkey)
         for statekey in args:
-            data = DootKey.make(statekey).to_type(spec, state)
+            data = DootKey.build(statekey).to_type(spec, state)
             _DootPostBox.put(target, data)
 
-        for subkey,statekey in kwargs.items():
-            data = DootKey.make(statekey).to_type(spec, state)
-            _DootPostBox.put(target, data, subkey=subkey)
+        root = _basename.root()
+        for subbox,statekey in kwargs.items():
+            box  = root.subtask(subbox)
+            match statekey:
+                case str():
+                    data = DootKey.build(statekey).to_type(spec, state)
+                    _DootPostBox.put(box, data)
+                case [*xs]:
+                    for x in statekey:
+                        data = DootKey.build(x).to_type(spec, state)
+                        _DootPostBox.put(box, data)
 
 
-@doot.check_protocol
 class GetPostAction(Action_p):
     """
       Read data from the inter-task postbox of a task tree
       The arguments of the action are held in self.spec
 
-      from=task
-      kwarg=subkey -> get the subbox and update task state as kwarg
-      kwarg=""     -> get the default subbox
-      kwarg="*"    -> get the entire box dict
+      stateKey="group::task.{subbox}"
+      eg: data="bib::format.-"
     """
 
-    @DootKey.kwrap.types("from", hint={"type_":str|None})
-    @DootKey.kwrap.kwargs
-    def __call__(self, spec, state, _from, kwargs) -> dict|bool|None:
-        target_box = _from or TASK_NAME.to_type(spec, state).root()
-
+    @DootKey.dec.kwargs
+    def __call__(self, spec, state, kwargs) -> dict|bool|None:
         updates = {}
         for key,subkey in kwargs.items():
-            if key == FROM_KEY:
-                pass
-            actual_key = DootKey.make(key, explicit=True).expand(spec, state)
-            updates[actual_key] = _DootPostBox.get(target_box, subkey=subkey)
+            state_key          = DootKey.build(key, explicit=True).expand(spec, state)
+            target_box         = DootTaskName.build(subkey)
+            updates[state_key] = _DootPostBox.get(target_box)
 
         return updates
 
-@doot.check_protocol
 class ClearPostAction(Action_p):
     """
       Clear your postbox
     """
-    _toml_kwargs = [FROM_KEY, SUBKEY]
-
-    @DootKey.kwrap.expands("subkey", hint={"on_fail":Any})
-    def __call__(self, spec, state, subkey):
-        from_task = TASK_NAME.to_type(spec, state).root()
-        _DootPostBox.clear_box(from_task, subkey=subkey)
+    @DootKey.dec.expands("key", hint={"on_fail":Any})
+    @DootKey.dec.taskname
+    def __call__(self, spec, state, key, _basename):
+        from_task = _basename.root().subtask(key)
+        _DootPostBox.clear_box(from_task)
         return
 
 
-@doot.check_protocol
 class SummarizePostAction(Action_p):
     """
       print a summary of this task tree's postbox
       The arguments of the action are held in self.spec
     """
-    _toml_kwargs = [FROM_KEY, "full"]
-
-    @DootKey.kwrap.types("from", hint={"type_":str|None})
-    @DootKey.kwrap.types("full", hint={"type_":bool, "on_fail":False})
+    @DootKey.dec.types("from", hint={"type_":str|None})
+    @DootKey.dec.types("full", hint={"type_":bool, "on_fail":False})
     def __call__(self, spec, state, _from, full) -> dict|bool|None:
         from_task = _from or TASK_NAME.to_type(spec, state).root()
         data   = _DootPostBox.get(from_task)
         if full:
             for x in data:
                 printer.info("Postbox %s: Item: %s", from_task, str(x))
```

### Comparing `doot-0.6.1/doot/actions/shell.py` & `doot-0.7.0/doot/actions/shell.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,32 +13,31 @@
 import sh
 import doot
 from doot.errors import DootTaskError
 from doot._abstract import Action_p
 from doot.actions.base_action import DootBaseAction
 from doot.structs import DootKey
 
-BACKGROUND = DootKey.make("background")
-UPDATE     = DootKey.make("update_")
-NOTTY      = DootKey.make("notty")
-ENV        = DootKey.make("shenv_")
+BACKGROUND = DootKey.build("background")
+UPDATE     = DootKey.build("update_")
+NOTTY      = DootKey.build("notty")
+ENV        = DootKey.build("shenv_")
 
-@doot.check_protocol
 class DootShellBake:
 
-    @DootKey.kwrap.args
-    @DootKey.kwrap.types("in_", hint={"on_fail":None, "type_":sh.Command|bool|None})
-    @DootKey.kwrap.types("env", hint={"on_fail":sh, "type_":sh.Command|bool|None})
-    @DootKey.kwrap.redirects("update_")
+    @DootKey.dec.args
+    @DootKey.dec.types("in_", hint={"on_fail":None, "type_":sh.Command|bool|None})
+    @DootKey.dec.types("env", hint={"on_fail":sh, "type_":sh.Command|bool|None})
+    @DootKey.dec.redirects("update_")
     def __call__(self, spec, state, args, _in, env, _update):
         if not env:
             env = sh
         try:
-            cmd                     = getattr(env, DootKey.make(args[0], explicit=True).expand(spec, state))
-            keys                    = [DootKey.make(x, explicit=True) for x in args[1:]]
+            cmd                     = getattr(env, DootKey.build(args[0], explicit=True).expand(spec, state))
+            keys                    = [DootKey.build(x, explicit=True) for x in args[1:]]
             expanded                = [x.expand(spec, state, locs=doot.locs) for x in keys]
             match _in:
                 case False | None:
                     baked = cmd.bake(*expanded, _return_cmd=True, _tty_out=False)
                 case sh.Command():
                     baked = cmd.bake(*expanded, _in=_in(), _return_cmd=True, _tty_out=False)
                 case _:
@@ -55,19 +54,18 @@
             printer.info("")
             if bool(err.stderr):
                 printer.error("%s", err.stderr.decode())
 
         return False
 
 
-@doot.check_protocol
 class DootShellBakedRun:
 
-    @DootKey.kwrap.types("in_", hint={"on_fail":None, "type_":sh.Command|None})
-    @DootKey.kwrap.redirects("update_")
+    @DootKey.dec.types("in_", hint={"on_fail":None, "type_":sh.Command|None})
+    @DootKey.dec.redirects("update_")
     def __call__(self, spec, state, _in, _update):
         try:
             result = _in()
             return { _update : result }
         except sh.CommandNotFound as err:
             printer.error("Shell Commmand '%s' Not Action: %s", err.args[0], args)
         except sh.ErrorReturnCode as err:
@@ -77,34 +75,33 @@
 
             printer.info("")
             if bool(err.stderr):
                 printer.error("%s", err.stderr.decode())
 
         return False
 
-@doot.check_protocol
 class DootShellAction(Action_p):
     """
     For actions in subshells.
     all other arguments are passed directly to the program, using `sh`
 
 
     can use a pre-baked sh passed into what "shenv_" points to
     """
 
-    @DootKey.kwrap.args
-    @DootKey.kwrap.types("background", "notty", hint={"type_":bool, "on_fail":False})
-    @DootKey.kwrap.types("env", hint={"on_fail":sh, "type_":sh.Command|None})
-    @DootKey.kwrap.redirects("update_")
+    @DootKey.dec.args
+    @DootKey.dec.types("background", "notty", hint={"type_":bool, "on_fail":False})
+    @DootKey.dec.types("env", hint={"on_fail":sh, "type_":sh.Command|None})
+    @DootKey.dec.redirects("update_")
     def __call__(self, spec, state, args, background, notty, env, _update) -> dict|bool|None:
         result     = None
         try:
             # Build the command by getting it from env, :
-            cmd                     = getattr(env, DootKey.make(args[0], explicit=True).expand(spec, state))
-            keys                    = [DootKey.make(x, explicit=True) for x in args[1:]]
+            cmd                     = getattr(env, DootKey.build(args[0], explicit=True).expand(spec, state))
+            keys                    = [DootKey.build(x, explicit=True) for x in args[1:]]
             expanded                = [x.expand(spec, state, locs=doot.locs) for x in keys]
             result                  = cmd(*expanded, _return_cmd=True, _bg=background, _tty_out=not notty)
             assert(result.exit_code == 0)
 
             printer.debug("(%s) Shell Cmd: %s, Args: %s, Result:", result.exit_code, args[0], args[1:])
             if not _update:
                 printer.info("%s", result, extra={"colour":"reset"})
@@ -121,15 +118,14 @@
 
             printer.info("")
             if bool(err.stderr):
                 printer.error("%s", err.stderr.decode())
 
         return False
 
-@doot.check_protocol
 class DootInteractiveAction(Action_p):
     """
       An interactive command, which uses the self.interact method as a callback for sh.
     """
     _toml_args = ["background"]
     aggregated = ""
     prompt     = ">>> "
@@ -138,15 +134,15 @@
     def __call__(self, spec, state:dict) -> dict|bool|None:
         try:
             self.prompt = spec.kwargs.on_fail(DootInteractiveAction.prompt, str).prompt()
             self.cont   = spec.kwargs.on_fail(DootInteractiveAction.cont, str).cont()
 
             cmd      = getattr(sh, spec.args[0])
             args     = spec.args[1:]
-            keys     = [DootKey.make(x, explicit=True) for x in args]
+            keys     = [DootKey.build(x, explicit=True) for x in args]
             expanded = [x.expand(spec, state, locs=doot.locs) for x in keys]
             result   = cmd(*expanded, _return_cmd=True, _bg=spec.kwargs.on_fail(False, bool).background(), _out=self.interact, _out_bufsize=0, _tty_in=True, _unify_ttys=True)
             assert(result.exit_code == 0)
             printer.debug("(%s) Shell Cmd: %s, Args: %s, Result:", result.exit_code, spec.args[0], spec.args[1:])
             printer.info("%s", result, extra={"colour":"reset"})
             return True
         except sh.CommandNotFound as err:
```

### Comparing `doot-0.6.1/doot/actions/speak.py` & `doot-0.7.0/doot/actions/speak.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,14 @@
 import sys
 import sh
 import doot
 from doot.structs import DootKey
 from doot.errors import DootTaskError, DootTaskFailed
 from doot._abstract import Action_p
 
-@doot.check_protocol
 class SpeakTimeAction(Action_p):
     """
     A Simple Action that announces the time
     Subclass this and override __call__ for your own actions.
     The arguments of the action are held in self.spec
 
     """
@@ -43,15 +42,15 @@
     linux_announce_args = ["The Time Is "]
     time_format   = "%H:%M"
 
     def _current_time(self) -> str:
         now = datetime.datetime.now()
         return now.strftime(self.time_format)
 
-    @DootKey.kwrap.args
+    @DootKey.dec.args
     def __call__(self, spec, state, args):
         try:
             match sys.platform:
                 case "linux":
                     return self._say_linux(spec, state)
                 case "darwin":
                     return self._say_mac(spec, state)
```

### Comparing `doot-0.6.1/doot/actions/state.py` & `doot-0.7.0/doot/actions/state.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,108 +28,100 @@
 from time import sleep
 import datetime
 import sh
 import shutil
 import doot
 from doot.errors import DootTaskError, DootTaskFailed
 from doot._abstract import Action_p
-from doot.mixins.importer import Importer_M
+from doot.mixins.importer import Importer_m
+from doot.mixins.path_manip import PathManip_m
 from doot.structs import DootCodeReference, DootKey
+from doot.actions.job_injection import JobInjectPathParts, JobInjectShadowAction
 
 ##-- expansion keys
-UPDATE : Final[DootKey] = DootKey.make("update_")
-FORMAT : Final[DootKey] = DootKey.make("format")
-FROM   : Final[DootKey] = DootKey.make("from")
+UPDATE : Final[DootKey] = DootKey.build("update_")
+FORMAT : Final[DootKey] = DootKey.build("format")
+FROM   : Final[DootKey] = DootKey.build("from")
 ##-- end expansion keys
 
-@doot.check_protocol
 class AddStateAction(Action_p):
     """
       add to task state in the task description toml,
       adds kwargs directly, without expansion
     """
 
-    @DootKey.kwrap.kwargs
+    @DootKey.dec.kwargs
     def __call__(self, spec, state:dict, kwargs) -> dict|bool|None:
         result = {}
         for k,v in kwargs.items():
-            key = DootKey.make(v, explicit=True)
+            key = DootKey.build(v, explicit=True)
             val = key.to_type(spec, state)
             result[k] = val
         return result
 
-
-@doot.check_protocol
-class AddStateFn(Action_p, Importer_M):
+class AddStateFn(Action_p, Importer_m):
     """ for each toml kwarg, import its value and set the state[kwarg] = val
       with expansion
     """
 
-    @DootKey.kwrap.kwargs
+    @DootKey.dec.kwargs
     def __call__(self, spec, state:dict, kwargs) -> dict|bool|None:
         result = {}
         for kwarg, val in kwargs:
-            key = DootKey.make(val, explicit=True)
+            key = DootKey.build(val, explicit=True)
             val = key.expand(spec, state)
-            ref = DootCodeReference.from_str(val)
+            ref = DootCodeReference.build(val)
             result[kwarg] = ref.try_import()
 
         return result
 
-
-
-@doot.check_protocol
 class PushState(Action_p):
     """
       state[update_] += [state[x] for x in spec.args]
     """
     _toml_kwargs = [UPDATE]
 
-    @DootKey.kwrap.args
-    @DootKey.kwrap.redirects("update_")
+    @DootKey.dec.args
+    @DootKey.dec.redirects("update_")
     def __call__(self, spec, state, args, _update) -> dict|bool|None:
         data     = data_key.to_type(spec, state, type_=list|set|None, on_fail=[])
 
-        arg_keys = (DootKey.make(arg, explicit=True).to_type(spec, state) for arg in args)
+        arg_keys = (DootKey.build(arg, explicit=True).to_type(spec, state) for arg in args)
         to_add   = map(lambda x: x if isinstance(x, list) else [x],
                        filter(lambda x: x is not None, arg_keys))
 
         match data:
             case set():
                 list(map(lambda x: data.update(x), to_add))
             case list():
                 list(map(lambda x: data.extend(x), to_add))
 
         return { _update : data }
 
-
-@doot.check_protocol
 class AddNow(Action_p):
     """
       Add the current date, as a string, to the state
     """
 
-    @DootKey.kwrap.expands("format")
-    @DootKey.kwrap.redirects("update_")
+    @DootKey.dec.expands("format")
+    @DootKey.dec.redirects("update_")
     def __call__(self, spec, state, format, _update):
         now      = datetime.datetime.now()
         return { _update : now.strftime(format) }
 
-
-@doot.check_protocol
-class PathParts(Action_p):
+class PathParts(PathManip_m):
     """ take a path and add fstem, fpar, fname to state """
 
-    @DootKey.kwrap.paths("from")
-    @DootKey.kwrap.returns("fstem", "fpar", "fname")
-    def __call__(self, spec, state, _from):
-        fpath = _from
-        name  = fpath.name
-        stem  = fpath
-        # This handles "a/b/c.tar.gz"
-        while stem.stem != stem.with_suffix("").stem:
-            stem = stem.with_suffix("")
-
-        return { "fstem": stem.stem,
-                 "fpar" : fpath.parent,
-                 "fname": name,
-                }
+    @DootKey.dec.paths("from")
+    @DootKey.dec.types("roots")
+    @DootKey.dec.returns("fstem", "fpar", "fname", "fext", "pstem")
+    def __call__(self, spec, state, _from, roots):
+        root_paths = self._build_roots(spec, state, roots)
+        return self._calc_path_parts(_from, root_paths)
+
+class ShadowPath(PathManip_m):
+
+    @DootKey.dec.paths("shadow_root")
+    @DootKey.dec.types("base", hint={"type_":pl.Path})
+    def __call__(self, spec, state, shadow_root, base):
+        shadow_dir = self._shadow_path(base, shadow_root)
+        return { "shadow_path" : shadow_dir }
```

### Comparing `doot-0.6.1/doot/actions/templater.py` & `doot-0.7.0/doot/actions/templater.py`

 * *Files identical despite different names*

### Comparing `doot-0.6.1/doot/actions/util.py` & `doot-0.7.0/doot/actions/util.py`

 * *Files identical despite different names*

### Comparing `doot-0.6.1/doot/cmds/__tests/test_list_cmd.py` & `doot-0.7.0/doot/cmds/__tests/test_list_cmd.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 
 import pytest
 import functools as ftz
 import sys
 import io
 import contextlib
 import doot
+doot._test_setup()
 import doot.errors
 from doot._abstract import Command_i
 from doot.structs import DootTaskSpec
 from doot.cmds.list_cmd import ListCmd
 
 class TestListCmd:
 
@@ -77,16 +78,16 @@
         mock_class1.__module__ = "builtins"
         mock_class1.__name__   = "type"
         mock_class2 = mocker.MagicMock(type)
         mock_class2.__module__ = "builtins"
         mock_class2.__name__   = "other.type"
         plugin_mock = {"reporter": [mocker.stub("Reporter Stub")]}
         job_mock = {
-            "simple" : DootTaskSpec.from_dict({"group": "blah", "name": "simple", "ctor": mock_class1}),
-            "other"  : DootTaskSpec.from_dict({"group": "bloo", "name": "other", "ctor": mock_class2})
+            "simple" : DootTaskSpec.build({"group": "blah", "name": "simple", "ctor": mock_class1}),
+            "other"  : DootTaskSpec.build({"group": "bloo", "name": "other", "ctor": mock_class2})
             }
         obj(job_mock, plugin_mock)
         message_set : set[str] = {x.message.lower().strip() for x in caplog.records}
 
         assert("defined task generators by group:" in message_set)
         assert(any(x.startswith("simple :: ") for x in message_set) )
         assert(any(x.startswith("other  :: ") for x in message_set) )
@@ -96,35 +97,35 @@
         del doot.args.cmd.args.keys
         doot.args.cmd.args.__iter__.return_value = iter([("pattern", "simple"), ("all", False)])
         doot.args.cmd.args.pattern = "simple"
         doot.args.cmd.args.all     = False
         obj = ListCmd()
         plugin_mock  = {"reporter": [mocker.stub("Reporter Stub")]}
         job_mock = {
-                       "simple" : DootTaskSpec.from_dict({"group": "blah", "name": "simple"}),
-                       "other"  : DootTaskSpec.from_dict({"group": "bloo", "name": "other"}),
+                       "simple" : DootTaskSpec.build({"group": "blah", "name": "simple"}),
+                       "other"  : DootTaskSpec.build({"group": "bloo", "name": "other"}),
             }
         result = obj(job_mock, plugin_mock)
         message_set : set[str] = {x.message.lower().strip() for x in caplog.records}
 
         assert("tasks for pattern: simple" in message_set)
-        assert( any(x.startswith("blah::simple :: doot.task.base_job:dootjob") for x in message_set) )
+        assert( any(x.startswith("blah::simple :: doot.task.base_task:doottask") for x in message_set) )
 
 
     def test_call_partial_target_not_empty(self, caplog, mocker):
         mocker.patch("doot.args")
         del doot.args.cmd.args.keys
         doot.args.cmd.args.__iter__.return_value = iter([("pattern", "simp"), ("all", False)])
         doot.args.cmd.args.pattern = "simp"
         doot.args.cmd.args.all     = False
         obj = ListCmd()
         plugin_mock = {"reporter": [mocker.stub("Reporter Stub")]}
-        job_mock = { "blah::simple" : DootTaskSpec.from_dict({"group": "blah", "name": "simple"}),
-                        "bloo::other": DootTaskSpec.from_dict({"group": "bloo", "name": "other"}),
-                        "bloo::diffSimple": DootTaskSpec.from_dict({"group": "bloo", "name": "diffSimple"}),
+        job_mock = { "blah::simple" : DootTaskSpec.build({"group": "blah", "name": "simple"}),
+                        "bloo::other": DootTaskSpec.build({"group": "bloo", "name": "other"}),
+                        "bloo::diffSimple": DootTaskSpec.build({"group": "bloo", "name": "diffSimple"}),
                        }
         result = obj(job_mock, plugin_mock)
         message_set : set[str] = {x.message.lower().strip() for x in caplog.records}
 
         assert("tasks for pattern: simp" in message_set)
-        assert( any(x.startswith("blah::simple     :: doot.task.base_job:dootjob") for x in message_set) )
-        assert( any(x.startswith("bloo::diffsimple :: doot.task.base_job:dootjob") for x in message_set) )
+        assert( any(x.startswith("blah::simple     :: doot.task.base_task:doottask") for x in message_set) )
+        assert( any(x.startswith("bloo::diffsimple :: doot.task.base_task:doottask") for x in message_set) )
```

### Comparing `doot-0.6.1/doot/cmds/complete_cmd.py` & `doot-0.7.0/doot/mixins/fail_handler.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,44 +1,52 @@
 #!/usr/bin/env python3
 """
 
+
+See EOF for license/metadata/notes as applicable
 """
-##-- imports
+
+##-- builtin imports
 from __future__ import annotations
 
 # import abc
-# import datetime
-# import enum
+import datetime
+import enum
 import functools as ftz
 import itertools as itz
 import logging as logmod
 import pathlib as pl
 import re
 import time
 import types
+import weakref
 # from copy import deepcopy
 # from dataclasses import InitVar, dataclass, field
 from typing import (TYPE_CHECKING, Any, Callable, ClassVar, Final, Generic,
                     Iterable, Iterator, Mapping, Match, MutableMapping,
                     Protocol, Sequence, Tuple, TypeAlias, TypeGuard, TypeVar,
-                    cast, final, overload, runtime_checkable)
-# from uuid import UUID, uuid1
-# from weakref import ref
+                    cast, final, overload, runtime_checkable, Generator)
+from uuid import UUID, uuid1
+
+##-- end builtin imports
 
-##-- end imports
+##-- lib imports
+import more_itertools as mitz
+##-- end lib imports
 
 ##-- logging
 logging = logmod.getLogger(__name__)
 ##-- end logging
+
 printer = logmod.getLogger("doot._printer")
 
 import doot
-from doot._abstract import Command_i
-
-class CompleteCmd(Command_i):
+import doot.errors
+from doot.structs import DootKey
 
-    @property
-    def param_specs(self) -> list:
-        return super().param_specs + []
+class FailHandler_m:
+    """
+      A Mixin for changing how a task runner handles failure
+    """
 
-    def __call__(self, tasks, plugins):
+    def _handle_failure(self, task, err):
         pass
```

### Comparing `doot-0.6.1/doot/cmds/daemon_cmd.py` & `doot-0.7.0/doot/reporters/basic_reporters.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,45 +1,51 @@
 #!/usr/bin/env python3
 """
 
+See EOF for license/metadata/notes as applicable
 """
-##-- imports
+
+##-- builtin imports
 from __future__ import annotations
 
 # import abc
-# import datetime
-# import enum
+import datetime
+import enum
 import functools as ftz
 import itertools as itz
 import logging as logmod
 import pathlib as pl
 import re
 import time
 import types
+import weakref
 # from copy import deepcopy
 # from dataclasses import InitVar, dataclass, field
 from typing import (TYPE_CHECKING, Any, Callable, ClassVar, Final, Generic,
                     Iterable, Iterator, Mapping, Match, MutableMapping,
                     Protocol, Sequence, Tuple, TypeAlias, TypeGuard, TypeVar,
-                    cast, final, overload, runtime_checkable)
-# from uuid import UUID, uuid1
-# from weakref import ref
+                    cast, final, overload, runtime_checkable, Generator)
+from uuid import UUID, uuid1
+
+##-- end builtin imports
 
-##-- end imports
+##-- lib imports
+import more_itertools as mitz
+##-- end lib imports
 
 ##-- logging
 logging = logmod.getLogger(__name__)
 ##-- end logging
-printer = logmod.getLogger("doot._printer")
 
-import doot
-from doot._abstract import Command_i
+from doot.structs import DootTraceRecord
+from doot._abstract import Reporter_i
 
+class DootAlwaysReport(Reporter_i):
 
-class DaemonCmd(Command_i):
+    def __call__(self, trace):
+        return str(trace)
 
-    @property
-    def param_specs(self) -> list:
-        return super().param_specs + []
+class TimeReporter(Reporter_i):
 
-    def __call__(self, tasks, plugins):
-        pass
+    def __call__(self, trace):
+        time = trace.time.strftime("%H:%M")
+        return "{:10} : {}".format(time, str(trace))
```

### Comparing `doot-0.6.1/doot/cmds/graph_cmd.py` & `doot-0.7.0/doot/cmds/graph_cmd.py`

 * *Files 9% similar despite different names*

```diff
@@ -34,43 +34,43 @@
 
 from collections import defaultdict
 import sh
 
 from tomlguard import TomlGuard
 import doot
 import doot.errors
-from doot._abstract import Command_i
+from doot.cmds.base_cmd import BaseCommand
 from doot.structs import DootParamSpec
 from doot.utils.plugin_selector import plugin_selector
 import networkx as nx
 import matplotlib.pyplot as plt
 
 printer                  = logmod.getLogger("doot._printer")
 
 INDENT : Final[str]      = " "*8
 tracker_target           = doot.config.on_fail("default", str).commands.run.tracker()
 
 @doot.check_protocol
-class GraphCmd(Command_i):
+class GraphCmd(BaseCommand):
     _name      = "graph"
     _help      = ["Create a graph representation of the task network"]
 
     @property
     def param_specs(self) -> list[DootParamSpec]:
         return super().param_specs + [
-            self.make_param(name="all",                                          default=True,                   desc="List all loaded tasks, by group"),
-            self.make_param(name="dependencies",                                 default=False,                  desc="List task dependencies",                 prefix="--"),
-            self.make_param(name="dag",       _short="D",                        default=False,                  desc="Output a DOT compatible graph of tasks", prefix="--"),
-            self.make_param(name="groups",                   type=bool,          default=False,                  desc="List just the groups tasks fall into",   prefix="--"),
-            self.make_param(name="by-source",                                    default=False,                  desc="List all loaded tasks, by source file",  prefix="--"),
-            self.make_param(name="locations", _short="l",    type=bool,          default=False,                  desc="List all Loaded Locations"),
-            self.make_param(name="internal",  _short="i",    type=bool,          default=False,                  desc="Include internal tasks (ie: prefixed with an underscore)"),
-            self.make_param(name="as-dot", type=bool, default=True, desc="use dot for visualisation"),
-            self.make_param(name="dot-file", prefix="--", type=str, default=None, desc="a file name to write the dot to"),
-            self.make_param(name="pattern",                  type=str,           default="", positional=True,    desc="List tasks with a basic string pattern in the name"),
+            self.build_param(name="all",                                          default=True,                   desc="List all loaded tasks, by group"),
+            self.build_param(name="dependencies",                                 default=False,                  desc="List task dependencies",                 prefix="--"),
+            self.build_param(name="dag",       _short="D",                        default=False,                  desc="Output a DOT compatible graph of tasks", prefix="--"),
+            self.build_param(name="groups",                   type=bool,          default=False,                  desc="List just the groups tasks fall into",   prefix="--"),
+            self.build_param(name="by-source",                                    default=False,                  desc="List all loaded tasks, by source file",  prefix="--"),
+            self.build_param(name="locations", _short="l",    type=bool,          default=False,                  desc="List all Loaded Locations"),
+            self.build_param(name="internal",  _short="i",    type=bool,          default=False,                  desc="Include internal tasks (ie: prefixed with an underscore)"),
+            self.build_param(name="as-dot", type=bool, default=True, desc="use dot for visualisation"),
+            self.build_param(name="dot-file", prefix="--", type=str, default=None, desc="a file name to write the dot to"),
+            self.build_param(name="pattern",                  type=str,           default="", positional=True,    desc="List tasks with a basic string pattern in the name"),
             ]
 
     def __call__(self, tasks:TomlGuard, plugins:TomlGuard):
         """List task generators"""
         logging.debug("Starting to List Jobs/Tasks")
         tracker = plugin_selector(plugins.on_fail([], list).tracker(), target=tracker_target)()
```

### Comparing `doot-0.6.1/doot/cmds/help_cmd.py` & `doot-0.7.0/doot/cmds/help_cmd.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,31 +28,31 @@
 
 ##-- logging
 logging = logmod.getLogger(__name__)
 printer = logmod.getLogger("doot._printer")
 ##-- end logging
 
 import doot
+from doot.cmds.base_cmd import BaseCommand
 from doot.structs import DootParamSpec, DootTaskSpec, DootCodeReference
-from doot._abstract import Command_i
-from doot.constants import NON_DEFAULT_KEY
 from collections import defaultdict
 
+NON_DEFAULT_KEY : Final[str] = doot.constants.misc.NON_DEFAULT_KEY
 
-class HelpCmd(Command_i):
+class HelpCmd(BaseCommand):
     _name      = "help"
     _help      = ["Print info about the specified cmd or task",
                   "Can also be triggered by passing --help to any command or task"
                   ]
 
     @property
     def param_specs(self) -> list:
         return super().param_specs + [
-            # self.make_param(name="target", type=str, default=""),
-            self.make_param(name="target", type=str, positional=True, default="", desc="The target to get help about. A command or task.")
+            # self.build_param(name="target", type=str, default=""),
+            self.build_param(name="target", type=str, positional=True, default="", desc="The target to get help about. A command or task.")
             ]
 
     def __call__(self, tasks, plugins):
         """List task generators"""
         task_targets = []
         cmd_targets  = []
         match dict(doot.args.cmd.args):
@@ -65,38 +65,35 @@
                 # Print help of just the specified target(s)
                 task_targets +=  [y for x,y in tasks.items() if target in x ]
                 cmd_targets  +=  [x for x in plugins.command if x.name == doot.args.cmd.args.target]
             case {"help": True}:
                 printer.info(self.help)
                 return
 
-
         logging.debug("Matched %s commands, %s tasks", len(cmd_targets), len(task_targets))
         if len(cmd_targets) == 1:
             cmd_class = cmd_targets[0].load()()
             printer.info(cmd_class.help)
             if bool(doot.args.cmd[NON_DEFAULT_KEY]):
                 self._print_current_param_assignments(cmd_class.param_specs, doot.args.cmd.args)
 
-
         elif bool(task_targets):
             for i, spec in enumerate(task_targets):
                 self.print_task_spec(i, spec)
 
         else:
             # Print general help and list cmds
             printer.info("Doot Help Command: No Target Specified/Matched")
             printer.info("Available Command Targets: ")
             for x in sorted(plugins.command, key=lambda x: x.name):
                 printer.info("-- %s", x.name)
 
         printer.info("\n------------------------------")
         printer.info("Call a command by doing 'doot [cmd] [args]'. Eg: doot list --help")
 
-
     def print_task_spec(self, count, spec:DootTaskSpec):
         task_name = spec.name
         match spec.ctor:
             case None:
                 ctor = None
             case DootCodeReference():
                 ctor = spec.ctor.try_import()
@@ -111,15 +108,14 @@
         lines.append(f"ver    : {spec.version}")
         lines.append(f"Group  : {spec.name.group}")
         lines.append(f"Source : {spec.source}")
 
         if ctor is not None:
             lines.append(ctor.class_help())
 
-
         match spec.doc:
             case None:
                 pass
             case str():
                 lines.append("")
                 lines.append(f"--   {spec.doc}")
             case list() as xs:
@@ -136,15 +132,14 @@
 
         if bool(spec.actions):
             printer.info("")
             printer.info("Task Actions: ")
             for action in spec.actions:
                 printer.info("-- %-20s : Args=%-20s Kwargs=%s", action.do, action.args, dict(action.kwargs) )
 
-
         cli_has_params = str(task_name) in doot.args.tasks
         cli_has_non_default = bool(doot.args.tasks[str(task_name)][NON_DEFAULT_KEY])
 
         if cli_has_params and cli_has_non_default and ctor is not None:
             self._print_current_param_assignments(ctor.param_specs, doot.args.tasks[task_name])
 
     def _print_current_param_assignments(self, specs:list[DootParamSpec], args:TomlGuard):
```

### Comparing `doot-0.6.1/doot/cmds/here_cmd.py` & `doot-0.7.0/doot/mixins/param_spec.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 """
-TODO Here Command. - run the system doot at this cwd, using either a local, nearest parent, or global doot toml and tasks
+
 
 See EOF for license/metadata/notes as applicable
 """
 
 ##-- builtin imports
 from __future__ import annotations
 
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
+from doot._structs.param_spec import DootParamSpec
+
+class ParamSpecMaker_m:
+
+    @staticmethod
+    def build_param(*args:Any, **kwargs:Any) -> DootParamSpec:
+        """ Utility method for easily making paramspecs """
+        return DootParamSpec(*args, **kwargs)
```

### Comparing `doot-0.6.1/doot/cmds/last_cmd.py` & `doot-0.7.0/doot/cmds/locs_cmd.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 #!/usr/bin/env python3
 """
-Print a summary of the last run
-
+A Doot Command to report on defined locations
 """
 ##-- imports
 from __future__ import annotations
 
 import types
 import abc
 import datetime
@@ -33,37 +32,52 @@
 
 printer = logmod.getLogger("doot._printer")
 
 from collections import defaultdict
 from tomlguard import TomlGuard
 import doot
 import doot.errors
-from doot._abstract import Command_i
+from doot.cmds.base_cmd import BaseCommand
 from doot.structs import DootParamSpec
 
 
 INDENT : Final[str] = " "*8
 
 @doot.check_protocol
-class LastCmd(Command_i):
-    _name      = "last"
-    _help      = ["Summarise the last run"]
-    STATUS_MAP = {'ignore': 'I', 'up-to-date': 'U', 'run': 'R', 'error': 'E'}
+class LocsCmd(BaseCommand):
+    _name      = "locs"
+    _help      = ["A simple command to list all config defined locations."]
 
     @property
     def param_specs(self) -> list[DootParamSpec]:
         return super().param_specs + [
-            self.make_param(name="all",                                          default=True,                   desc="List all loaded tasks, by group"),
-            self.make_param(name="dependencies",                                 default=False,                  desc="List task dependencies",                 prefix="--"),
-            self.make_param(name="dag",       _short="D",                        default=False,                  desc="Output a DOT compatible graph of tasks", prefix="--"),
-            self.make_param(name="groups",                   type=bool,          default=False,                  desc="List just the groups tasks fall into",   prefix="--"),
-            self.make_param(name="by-source",                                    default=False,                  desc="List all loaded tasks, by source file",  prefix="--"),
-            self.make_param(name="locations", _short="l",    type=bool,          default=False,                  desc="List all Loaded Locations"),
-            self.make_param(name="internal",  _short="i",    type=bool,          default=False,                  desc="Include internal tasks (ie: prefixed with an underscore)"),
-            self.make_param(name="pattern",                  type=str,           default="", positional=True,    desc="List tasks with a basic string pattern in the name"),
+            self.build_param(name="all",                                          default=True,                   desc="List all loaded tasks, by group"),
+            self.build_param(name="by-source",                                    default=False,                  desc="List all loaded tasks, by source file",  prefix="--"),
+            self.build_param(name="pattern",                  type=str,           default="", positional=True,    desc="List tasks with a basic string pattern in the name"),
             ]
 
     def __call__(self, tasks:TomlGuard, plugins:TomlGuard):
         """List task generators"""
-        logging.debug("Starting to List Jobs/Tasks")
+        logging.debug("Starting to List Locations")
+
+        if not bool(doot.locs):
+            printer.info("No Locations Defined")
+            return
+
+        self._print_all()
+
+    def _print_matches(self, plugins):
+        raise NotImplementedError()
+
+    def _print_by_source(self, plugins):
+        raise NotImplementedError()
+
+    def _print_all(self):
+        printer.info("Defined Locations:", extra={"colour":"cyan"})
+        max_key = len(max(doot.locs, key=len))
+        fmt_str = f"{INDENT}%-{max_key}s :: %-25s"
+        locs = defaultdict(list)
+
+        for name in doot.locs:
+            printer.info(fmt_str, name, doot.locs[f"{{{name}}}"])
 
-        raise NotImplementedError("TODO")
+        printer.info("")
```

### Comparing `doot-0.6.1/doot/cmds/list_cmd.py` & `doot-0.7.0/doot/cmds/list_cmd.py`

 * *Files 7% similar despite different names*

```diff
@@ -33,36 +33,36 @@
 
 printer = logmod.getLogger("doot._printer")
 
 from collections import defaultdict
 from tomlguard import TomlGuard
 import doot
 import doot.errors
-from doot._abstract import Command_i
+from doot.enums import TaskFlags
+from doot.cmds.base_cmd import BaseCommand
 from doot.structs import DootParamSpec
 
-
 INDENT : Final[str] = " "*8
 
 @doot.check_protocol
-class ListCmd(Command_i):
+class ListCmd(BaseCommand):
     _name      = "list"
     _help      = ["A simple command to list all loaded task heads."]
 
     @property
     def param_specs(self) -> list[DootParamSpec]:
         return super().param_specs + [
-            self.make_param(name="all",                                          default=True,                   desc="List all loaded tasks, by group"),
-            self.make_param(name="dependencies",                                 default=False,                  desc="List task dependencies",                 prefix="--"),
-            self.make_param(name="dag",       _short="D",                        default=False,                  desc="Output a DOT compatible graph of tasks", prefix="--"),
-            self.make_param(name="groups",                   type=bool,          default=False,                  desc="List just the groups tasks fall into",   prefix="--"),
-            self.make_param(name="by-source",                                    default=False,                  desc="List all loaded tasks, by source file",  prefix="--"),
-            self.make_param(name="locations", _short="l",    type=bool,          default=False,                  desc="List all Loaded Locations"),
-            self.make_param(name="internal",  _short="i",    type=bool,          default=False,                  desc="Include internal tasks (ie: prefixed with an underscore)"),
-            self.make_param(name="pattern",                  type=str,           default="", positional=True,    desc="List tasks with a basic string pattern in the name"),
+            self.build_param(name="all",                                          default=True,                   desc="List all loaded tasks, by group"),
+            self.build_param(name="dependencies",                                 default=False,                  desc="List task dependencies",                 prefix="--"),
+            self.build_param(name="dag",       _short="D",                        default=False,                  desc="Output a DOT compatible graph of tasks", prefix="--"),
+            self.build_param(name="groups",                   type=bool,          default=False,                  desc="List just the groups tasks fall into",   prefix="--"),
+            self.build_param(name="by-source",                                    default=False,                  desc="List all loaded tasks, by source file",  prefix="--"),
+            self.build_param(name="locations", _short="l",    type=bool,          default=False,                  desc="List all Loaded Locations"),
+            self.build_param(name="internal",  _short="i",    type=bool,          default=False,                  desc="Include internal tasks (ie: prefixed with an underscore)"),
+            self.build_param(name="pattern",                  type=str,           default="", positional=True,    desc="List tasks with a basic string pattern in the name"),
             ]
 
     def __call__(self, tasks:TomlGuard, plugins:TomlGuard):
         """List task generators"""
         logging.debug("Starting to List Jobs/Tasks")
 
         if (doot.args.cmd.args.pattern == ""     # type: ignore
@@ -95,15 +95,15 @@
         max_key = len(max(tasks.keys(), key=len))
         fmt_str = f"%-{max_key}s :: %-25s <%s>"
         pattern = doot.args.cmd.args.pattern.lower()
         matches = {x for x in tasks.keys() if pattern in x.lower()}
         printer.info("Tasks for Pattern: %s", pattern)
         for key in matches:
             spec = tasks[key]
-            if spec.name.internal and not doot.args.cmd.args.internal:
+            if TaskFlags.INTERNAL in spec.name.meta and not doot.args.cmd.args.internal:
                 continue
 
             printer.info(fmt_str,
                          spec.name,
                          spec.ctor,
                          spec.source)
 
@@ -111,15 +111,15 @@
         max_key = len(max(tasks.keys(), key=len))
         fmt_str = f"    %-{max_key}s :: %-25s <%s>"
         pattern  = doot.args.cmd.args.pattern.lower()
         groups  = defaultdict(list)
         for name, spec in tasks.items():
             if pattern not in name:
                 continue
-            if spec.name.internal and not doot.args.cmd.args.internal:
+            if TaskFlags.INTERNAL in spec.name.meta and not doot.args.cmd.args.internal:
                 continue
 
             groups[spec.name.group].append((spec.name.task,
                                                   spec.ctor.__module__,
                                                   spec.ctor.__name__,
                                                   spec.source))
 
@@ -131,16 +131,17 @@
 
     def _print_all_by_group(self, tasks):
         printer.info("Defined Task Generators by Group:", extra={"colour":"cyan"})
         max_key = len(max(tasks.keys(), key=len))
         fmt_str = f"{INDENT}%-{max_key}s :: %-60s :: <Source: %s>"
         groups  = defaultdict(list)
         for spec in tasks.values():
-            if spec.name.internal and not doot.args.cmd.args.internal:
+            if TaskFlags.INTERNAL in spec.name.meta and not doot.args.cmd.args.internal:
                 continue
+
             groups[spec.name.group].append((spec.name.task,
                                                   (spec.doc[0] if bool(spec.doc) else "")[:60],
                                                   spec.source))
 
         for group, tasks in groups.items():
             printer.info("*   %s::", group, extra={"colour":"magenta"})
             for task in tasks:
@@ -151,33 +152,32 @@
 
     def _print_all_by_source(self, tasks):
         printer.info("Defined Task Generators by Source File:", extra={"colour":"cyan"})
         max_key = len(max(tasks.keys(), key=len))
         fmt_str = f"{INDENT}%-{max_key}s :: %s.%-25s"
         sources = defaultdict(list)
         for key, spec in tasks.items():
-            if spec.name.internal and not doot.args.cmd.args.internal:
+            if TaskFlags.INTERNAL in spec.name.meta and not doot.args.cmd.args.internal:
                 continue
+
             sources[spec.source].append((spec.name.task,
                                          spec.ctor.__module__,
                                          spec.ctor.__name__,
                                         ))
 
         for source, tasks in sources.items():
             printer.info(":: %s ::", source, extra={"colour":"red"})
             for task in tasks:
                 printer.info(fmt_str, *task)
 
-
     def _print_just_groups(self, tasks):
         printer.info("Defined Task Groups:", extra={"colour":"cyan"})
 
         group_set = set(spec.name.group for spec in tasks.values())
         for group in group_set:
             printer.info("- %s", group)
 
-
     def _print_locations(self):
         printer.info("Defined Locations: ")
 
         for x in sorted(doot.locs):
             printer.info("-- %-25s : %s", x, doot.locs.get(x))
```

### Comparing `doot-0.6.1/doot/cmds/locs_cmd.py` & `doot-0.7.0/doot/cmds/base_cmd.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,83 +1,84 @@
 #!/usr/bin/env python3
 """
-A Doot Command to report on defined locations
+
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
+# import more_itertools as mitz
+# from boltons import
+##-- end lib imports
 
 ##-- logging
 logging = logmod.getLogger(__name__)
 ##-- end logging
 
-printer = logmod.getLogger("doot._printer")
-
-from collections import defaultdict
-from tomlguard import TomlGuard
-import doot
-import doot.errors
 from doot._abstract import Command_i
-from doot.structs import DootParamSpec
+from doot.mixins.param_spec import ParamSpecMaker_m
 
+class BaseCommand(ParamSpecMaker_m, Command_i):
+    """ Generic implementations of command methods """
 
-INDENT : Final[str] = " "*8
+    def __init__(self, name=None):
+        self._name = name
 
-@doot.check_protocol
-class LocsCmd(Command_i):
-    _name      = "locs"
-    _help      = ["A simple command to list all config defined locations."]
+    @property
+    def name(self):
+        """get command name as used from command line"""
+        return self._name or self.__class__.__name__.lower()
 
     @property
-    def param_specs(self) -> list[DootParamSpec]:
-        return super().param_specs + [
-            self.make_param(name="all",                                          default=True,                   desc="List all loaded tasks, by group"),
-            self.make_param(name="by-source",                                    default=False,                  desc="List all loaded tasks, by source file",  prefix="--"),
-            self.make_param(name="pattern",                  type=str,           default="", positional=True,    desc="List tasks with a basic string pattern in the name"),
-            ]
-
-    def __call__(self, tasks:TomlGuard, plugins:TomlGuard):
-        """List task generators"""
-        logging.debug("Starting to List Locations")
-
-        if not bool(doot.locs):
-            printer.info("No Locations Defined")
-            return
-
-        self._print_all()
-
-    def _print_matches(self, plugins):
-        raise NotImplementedError()
-
-    def _print_by_source(self, plugins):
-        raise NotImplementedError()
-
-    def _print_all(self):
-        printer.info("Defined Locations:", extra={"colour":"cyan"})
-        max_key = len(max(doot.locs, key=len))
-        fmt_str = f"{INDENT}%-{max_key}s :: %-25s"
-        locs = defaultdict(list)
+    def help(self) -> str:
+        help_lines = ["", f"Command: {self.name} v{self._version}", ""]
+        help_lines += self._help
+
+        params = self.param_specs
+        if bool(params):
+            key_func = params[0].key_func
+            help_lines += ["", "Params:"]
+            help_lines += map(str, sorted(filter(lambda x: not x.invisible,
+                                            self.param_specs),
+                                    key=key_func))
 
-        for name in doot.locs:
-            printer.info(fmt_str, name, doot.locs[name])
+        return "\n".join(help_lines)
 
-        printer.info("")
+    @property
+    def helpline(self) -> str:
+        """ get just the first line of the help text """
+        if not bool(self._help):
+            return f" {self.name: <10} v{self._version:>5} :"
+        return f" {self.name: <10} v{self._version:>5} : {self._help[0]}"
+
+    @property
+    def param_specs(self) -> list[ParamStruct_p]:
+        """
+        Provide parameter specs for parsing into doot.args.cmd
+        """
+        return [
+           self.build_param(name="help", default=False, prefix="--", invisible=True),
+           self.build_param(name="debug", default=False, prefix="--", invisible=True)
+           ]
```

### Comparing `doot-0.6.1/doot/cmds/plugins_cmd.py` & `doot-0.7.0/doot/cmds/plugins_cmd.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,31 +32,31 @@
 
 printer = logmod.getLogger("doot._printer")
 
 from collections import defaultdict
 from tomlguard import TomlGuard
 import doot
 import doot.errors
-from doot._abstract import Command_i
+from doot.cmds.base_cmd import BaseCommand
 from doot.structs import DootParamSpec
 
 
 INDENT : Final[str] = " "*8
 
 @doot.check_protocol
-class PluginsCmd(Command_i):
+class PluginsCmd(BaseCommand):
     _name      = "plugins"
     _help      = ["A simple command to list all loaded plugins."]
 
     @property
     def param_specs(self) -> list[DootParamSpec]:
         return super().param_specs + [
-            self.make_param(name="all",                  default=True,                   desc="List all loaded tasks, by group"),
-            self.make_param(name="groups",    type=bool, default=False,                  desc="List just the groups tasks fall into",   prefix="--"),
-            self.make_param(name="pattern",   type=str,  default="", positional=True,    desc="List tasks with a basic string pattern in the name"),
+            self.build_param(name="all",                  default=True,                   desc="List all loaded tasks, by group"),
+            self.build_param(name="groups",    type=bool, default=False,                  desc="List just the groups tasks fall into",   prefix="--"),
+            self.build_param(name="pattern",   type=str,  default="", positional=True,    desc="List tasks with a basic string pattern in the name"),
             ]
 
     def __call__(self, tasks:TomlGuard, plugins:TomlGuard):
         """List task generators"""
         logging.debug("Starting to List System Plugins ")
 
         if not bool(plugins):
```

### Comparing `doot-0.6.1/doot/cmds/run_cmd.py` & `doot-0.7.0/doot/cmds/run_cmd.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,41 +29,43 @@
 ##-- logging
 logging = logmod.getLogger(__name__)
 ##-- end logging
 
 from collections import defaultdict
 from tomlguard import TomlGuard
 import doot
-from doot._abstract import ReportLine_i, TaskRunner_i, Reporter_i, Command_i
+from doot.cmds.base_cmd import BaseCommand
+from doot._abstract import ReportLine_i, TaskRunner_i, Reporter_i
 from doot.utils.plugin_selector import plugin_selector
 from doot.task.check_locs import CheckLocsTask
 from doot.structs import DootCodeReference
 
 printer                  = logmod.getLogger("doot._printer")
 
 tracker_target           = doot.config.on_fail("default", str).commands.run.tracker()
 runner_target            = doot.config.on_fail("default", str).commands.run.runner()
 reporter_target          = doot.config.on_fail("default", str).commands.run.reporter()
 report_line_targets      = doot.config.on_fail([]).commands.run.report_line(wrapper=list)
 interrupt_handler        = doot.config.on_fail("doot.utils.signal_handler:SignalHandler", bool|str).commands.run.interrupt()
 
 @doot.check_protocol
-class RunCmd(Command_i):
+class RunCmd(BaseCommand):
     _name      = "run"
     _help      = ["Will perform the tasks/jobs targeted.",
                   "Can be parameterized in a commands.run block with:",
                   "tracker(str), runner(str), reporter(str), report_lines(str)",
                   ]
 
     @property
     def param_specs(self) -> list:
         return super().param_specs + [
-            self.make_param(name="step", default=False),
-            self.make_param(name="dry-run", default=False),
-            self.make_param(name="target", type=list[str], default=[], positional=True),
+            self.build_param(name="step", default=False),
+            self.build_param(name="interrupt", default=False),
+            self.build_param(name="dry-run", default=False),
+            self.build_param(name="target", type=list[str], default=[], positional=True),
             ]
 
     def __call__(self, tasks:TomlGuard, plugins:TomlGuard):
         # Note the final parens to construct:
         available_reporters    = plugins.on_fail([], list).report_line()
         report_lines           = [plugin_selector(available_reporters, target=x)() for x in report_line_targets]
         reporter               = plugin_selector(plugins.on_fail([], list).reporter(), target=reporter_target)(report_lines)
@@ -87,17 +89,19 @@
                 printer.warn(- "%s specified as run target, but it doesn't exist")
             else:
                 tracker.queue_task(target)
 
         tracker.queue_task(CheckLocsTask.task_name)
 
         match interrupt_handler:
+            case _ if not doot.args.cmd.args.interrupt:
+                interrupt = None
+            case None:
+                interrupt = None
             case bool():
                 interrupt = interrupt_handler
             case str():
-                interrupt = DootCodeReference.from_str(interrupt_handler).try_import()
-            case None:
-                interrupt = None
+                interrupt = DootCodeReference.build(interrupt_handler).try_import()
 
         printer.info("- %s Tasks Queued: %s", len(tracker.active_set), " ".join(tracker.active_set))
         with runner:
             runner(handler=interrupt)
```

### Comparing `doot-0.6.1/doot/cmds/server_cmd.py` & `doot-0.7.0/doot/utils/chain_get.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,66 +1,60 @@
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
+# import more_itertools as mitz
+# from boltons import
+##-- end lib imports
 
 ##-- logging
 logging = logmod.getLogger(__name__)
 ##-- end logging
-printer = logmod.getLogger("doot._printer")
-from flask import Flask, request
-import doot
-from doot._abstract import Command_i
 
-app = Flask("basic")
-
-# From https://stackoverflow.com/questions/63902300
-class BasicServer(Command_i):
+class DootKeyGetter:
     """
-    a test doot command
+      The core logic to turn a key into a value.
+      Doesn't perform repeated expansions.
+
+      tries sources in order.
     """
-    name            = 'BasicServer'
-    doc_purpose     = "A Really Simple Https Flask Server"
-    doc_description = ""
-    doc_usage       = ""
-    cmd_options     = ()
-
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-
-    @property
-    def param_specs(self) -> list:
-        return super().param_specs + []
-
-    def __call__(self, tasks:TomlGuard, plugins:TomlGuard):
-        pass
-        # app.run(port=8000, debug=True, ssl_context="adhoc")
-
-@app.route('/', methods=["GET", "POST"])
-def index():
-    # https://improveandrepeat.com/2022/03/python-friday-112-how-to-use-tweepy-in-flask/
-    # args               = request.args
-    logging.info(request.url)
-    return "nothing"
+
+    @staticmethod
+    def chained_get(key:str, *sources:dict|DootLocations) -> Any:
+        # cli   : dict          = doot.args.on_fail({}).tasks[str(state.get(STATE_TASK_NAME_K, None))]()
+        # replacement           = cli.get(key, None)
+        # *Not* elif's, want it to chain.
+        for source in sources:
+            if source is None:
+                continue
+            replacement = source.get(key, None)
+            if replacement is not None:
+                return replacement
+
+        return None
```

### Comparing `doot-0.6.1/doot/cmds/step_cmd.py` & `doot-0.7.0/doot/cmds/step_cmd.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,38 +33,39 @@
 ##-- logging
 logging = logmod.getLogger(__name__)
 ##-- end logging
 
 from collections import defaultdict
 from tomlguard import TomlGuard
 import doot
-from doot._abstract import ReportLine_i, TaskRunner_i, Reporter_i, Command_i
+from doot.cmds.base_cmd import BaseCommand
+from doot._abstract import ReportLine_i, TaskRunner_i, Reporter_i
 from doot.utils.plugin_selector import plugin_selector
 from doot.task.check_locs import CheckLocsTask
 
 printer                  = logmod.getLogger("doot._printer")
 
 runner_target            = doot.config.on_fail("step", str).commands.step.runner()
 tracker_target           = doot.config.on_fail("default", str).commands.step.tracker()
 reporter_target          = doot.config.on_fail("default", str).commands.step.reporter()
 report_line_targets      = doot.config.on_fail([]).commands.run.report_line(wrapper=list)
 
-class StepCmd(Command_i):
+class StepCmd(BaseCommand):
     """
     Standard doit run command, but step through tasks
     """
     _name            = 'step'
     _help            = ["Behaves like Run, but allows user confirmation before job/task/action performance"]
 
     @property
     def param_specs(self) -> list:
         return super().param_specs + [
-            self.make_param(name="dry-run", default=False),
-            self.make_param(name="type", type=str, default="task"),
-            self.make_param(name="target", type=list[str], default=[], positional=True),
+            self.build_param(name="dry-run", default=False),
+            self.build_param(name="type", type=str, default="task"),
+            self.build_param(name="target", type=list[str], default=[], positional=True),
             ]
 
     def __call__(self, tasks:TomlGuard, plugins:TomlGuard):
         # Note the final parens to construct:
         available_reporters    = plugins.on_fail([], list).report_line()
         report_lines           = [plugin_selector(available_reporters, target=x)() for x in report_line_targets]
         reporter               = plugin_selector(plugins.on_fail([], list).reporter(), target=reporter_target)(report_lines)
```

### Comparing `doot-0.6.1/doot/cmds/stub_cmd.py` & `doot-0.7.0/doot/cmds/stub_cmd.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,56 +29,57 @@
 ##-- logging
 logging = logmod.getLogger(__name__)
 printer = logmod.getLogger("doot._printer")
 ##-- end logging
 
 from collections import defaultdict
 import importlib
+from importlib.resources import files
 import doot
 import doot.enums
 import doot.errors
-import doot.constants
-from doot._abstract import Command_i, PluginLoader_p, TaskBase_i
+from doot.cmds.base_cmd import BaseCommand
+from doot._abstract import PluginLoader_p, Task_i
 from doot.structs import TaskStub, DootTaskName, DootCodeReference
 from doot.task.base_job import DootJob
 from doot.task.base_task import DootTask
 from doot._structs.key import KEY_ANNOTS, HELP_HINT
 
-
 ##-- data
-data_path = doot.constants.TOML_TEMPLATE
+data_path = files(doot.constants.paths.TEMPLATE_PATH).joinpath(doot.constants.paths.TOML_TEMPLATE)
 ##-- end data
+PRINT_LOCATIONS : Final[list[str]] = doot.constants.printer.PRINT_LOCATIONS
 
-class StubCmd(Command_i):
+class StubCmd(BaseCommand):
     """ Called to interactively create a stub task definition
       with a `target`, outputs to that file, else to stdout for piping
     """
     _name      = "stub"
     _help      = ["Create a new stub task either to stdout, or path"]
 
     @property
     def param_specs(self) -> list:
         return super().param_specs + [
-            self.make_param("file-target", type=str,     default=""),
-            self.make_param("Config",                    default=False,           desc="Stub a doot.toml",                  prefix="-"),
-            self.make_param("Actions",                   default=False,           desc="Help Stub Actions",                 prefix="-"),
-            self.make_param("cli",                       default=False,           desc="Generate a stub cli arg dict",      prefix="-"),
-            self.make_param("printer",                   default=False,           desc="Generate a stub cli arg dict",      prefix="-"),
-
-            self.make_param("Flags",                     default=False,           desc="Help Stub Task Flags",              prefix="-"),
-
-            self.make_param("name",        type=str,     default=None,            desc="The Name of the new task",                          positional=True),
-            self.make_param("ctor",        type=str,     default="task",          desc="The short type name of the task generator",         positional=True),
-            self.make_param("mixins",      type=list,    default=[],              desc="Mixins to add to task/job", prefix="--"),
-            self.make_param("suppress-header",           default=True, invisible=True)
+            self.build_param("file-target", type=str,     default=""),
+            self.build_param("Config",                    default=False,           desc="Stub a doot.toml",                  prefix="-"),
+            self.build_param("Actions",                   default=False,           desc="Help Stub Actions",                 prefix="-"),
+            self.build_param("cli",                       default=False,           desc="Generate a stub cli arg dict",      prefix="-"),
+            self.build_param("printer",                   default=False,           desc="Generate a stub cli arg dict",      prefix="-"),
+
+            self.build_param("Flags",                     default=False,           desc="Help Stub Task Flags",              prefix="-"),
+
+            self.build_param("name",        type=str,     default=None,            desc="The Name of the new task",                          positional=True),
+            self.build_param("ctor",        type=str,     default="task",          desc="The short type name of the task generator",         positional=True),
+            self.build_param("mixins",      type=list,    default=[],              desc="Mixins to add to task/job", prefix="--"),
+            self.build_param("suppress-header",           default=True, invisible=True)
             ]
 
     def _import_task_class(self, ctor_name):
         try:
-            code_ref = DootCodeReference.from_str(ctor_name)
+            code_ref = DootCodeReference.build(ctor_name)
             return code_ref.try_import()
         except ImportError as err:
             raise doot.errors.DootTaskLoadError(ctor_name)
 
     def __call__(self, tasks:TomlGuard, plugins:TomlGuard):
         match dict(doot.args.cmd.args):
             case {"Config": True}:
@@ -117,15 +118,15 @@
         task_iden_with_mixins       : DootCodeReference       = task_iden.add_mixins(*doot.args.on_fail([]).cmd.args.mixins(), plugins=plugins)
 
         if (name:=doot.args.on_fail((None,)).cmd.args.name()) is None:
             raise doot.errors.DootCommandError("No Name Provided for Stub")
 
         # Create stub toml, with some basic information
         stub                          = TaskStub(ctor=task_iden_with_mixins)
-        stub['name'].default          = DootTaskName.from_str(name)
+        stub['name'].default          = DootTaskName.build(name)
         stub['mixins'].set(type="list", default=[], comment="mix in additional capabilities")
 
         # add ctor specific fields,
         # such as for dir_walker: roots [], exts [], recursive bool, subtask "", head_task ""
         # works *towards* the task_type, not away, so more specific elements are added over the top of more general elements
         try:
             task_mro = task_iden_with_mixins.try_import().mro()
@@ -133,15 +134,15 @@
             logging.error(err.args[0].replace("\n", ""))
             task_mro = []
             return
 
         for cls in reversed(task_mro):
             try:
                 cls.stub_class(stub)
-                if issubclass(cls, TaskBase_i):
+                if issubclass(cls, Task_i):
                     stub['version'].default         = cls.version
                     stub['doc'].default             = [x for x in cls.class_help().split("\n") if bool(x)]
             except NotImplementedError:
                 pass
             except AttributeError:
                 pass
 
@@ -223,13 +224,13 @@
         stub.append('default="", ')
         stub.append('desc="", ')
         stub.append('positional=false ')
 
         printer.info("{ %s }", "".join(stub))
 
     def _stub_printer_settings(self):
-        printer.info("print_levels = { %s }", ", ".join(f'{x}="INFO"' for x in doot.constants.PRINT_LOCATIONS))
+        printer.info("print_levels = { %s }", ", ".join(f'{x}="INFO"' for x in PRINT_LOCATIONS))
 
     def _list_flags(self):
         printer.info("Task Flags: ")
         for x in sorted(doot.enums.TaskFlags, key=lambda x: x.name):
             printer.info("-- %s", x.name)
```

### Comparing `doot-0.6.1/doot/control/__tests/test_locations.py` & `doot-0.7.0/doot/control/__tests/test_locations.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,16 @@
                     Mapping, Match, MutableMapping, Sequence, Tuple, TypeAlias,
                     TypeVar, cast)
 import warnings
 
 import pytest
 
 import tomlguard
+import doot
+doot._test_setup()
 from doot.errors import DootDirAbsent, DootLocationExpansionError, DootLocationError
 from doot.control.locations import DootLocations
 
 logging = logmod.root
 
 ##-- pytest reminder
 # caplog
@@ -40,14 +42,15 @@
 
     def test_update(self):
         simple = DootLocations(pl.Path.cwd())
         assert(not bool(simple._data))
         simple.update({"blah": "bloo"})
         assert(bool(simple._data))
 
+    @pytest.mark.skip
     def test_update_conflict(self):
         simple = DootLocations(pl.Path.cwd())
         simple.update({"blah": "bloo"})
 
         with pytest.raises(DootLocationError):
             simple.update({"blah": "blah"})
 
@@ -231,9 +234,9 @@
 
     def test_context_manager(self):
         simple = DootLocations(pl.Path.cwd())
         assert(not bool(simple._data))
         simple.update({"a": "blah"})
         assert(bool(simple._data))
 
-        with simple(pl.Path("~/desktop")) as ctx:
-            assert(ctx.a == (pl.Path("~/desktop/") / "blah").expanduser().absolute())
+        with simple(pl.Path("~/Desktop")) as ctx:
+            assert(ctx.a == (pl.Path("~/Desktop/") / "blah").expanduser().absolute())
```

### Comparing `doot-0.6.1/doot/control/__tests/test_overlord.py` & `doot-0.7.0/doot/control/__tests/test_overlord.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,16 @@
 ##-- end imports
 logging = logmod.root
 
 import pytest
 import sys
 import tomlguard
 import doot
-doot.config = tomlguard.TomlGuard({})
+doot._test_setup()
+
 from doot.control.overlord import DootOverlord
 
 BASIC_JOB_NAME = "job"
 
 class TestOverlord:
 
     def test_initial(self, mocker):
@@ -34,22 +35,22 @@
         assert(overlord.args == ["doot"])
 
     def test_plugins_loaded(self, mocker):
         mocker.patch("sys.argv", ["doot"])
         mocker.patch("doot.loaders.task_loader.DootTaskLoader")
         overlord = DootOverlord()
         assert(bool(overlord.plugins))
-        assert(all(x in overlord.plugins for x in doot.constants.DEFAULT_PLUGINS.keys()))
+        assert(all(x in overlord.plugins for x in doot.aliases.keys()))
 
     def test_cmds_loaded(self, mocker):
         mocker.patch("sys.argv", ["doot"])
         mocker.patch("doot.loaders.task_loader.DootTaskLoader")
         overlord = DootOverlord()
         assert(bool(overlord.cmds))
-        assert(len(overlord.cmds) >= len(doot.constants.DEFAULT_PLUGINS['command']))
+        assert(len(overlord.cmds) >= len(doot.aliases.command))
 
     def test_tasks_loaded(self, mocker):
         mocker.patch("sys.argv", ["doot"])
         mocker.patch("doot.loaders.task_loader.task_sources")
         overlord = DootOverlord(
             extra_config={"tasks" : {"basic" : [{"name": "simple", "ctor": BASIC_JOB_NAME}]}}
         )
```

### Comparing `doot-0.6.1/doot/control/__tests/test_runner.py` & `doot-0.7.0/doot/control/__tests/test_runner.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,14 +11,16 @@
                     TypeVar, cast)
 import warnings
 
 import pytest
 
 import tomlguard
 import doot
+doot._test_setup()
+
 from doot.enums import TaskStateEnum
 from doot.control.runner import DootRunner
 from doot.control.tracker import DootTracker
 from doot.structs import DootTaskSpec, DootActionSpec
 from doot._abstract import Job_i, Task_i, TaskTracker_i, TaskRunner_i, ReportLine_i, Action_p, Reporter_i
 from doot.utils import mock_gen
 
@@ -70,24 +72,24 @@
         # Run
         runner(handler=False)
 
         ##-- check result
         tracker_m.update_state.assert_called()
         assert(tracker_m.update_state.call_count == 3)
         for call in tracker_m.update_state.call_args_list:
-            assert(call.args[0].name in ["first", "second", "third"])
+            assert(call.args[0].name in ["default::first", "default::second", "default::third"])
             assert(call.args[1] is tracker_m.state_e.SUCCESS)
 
         expand_job.assert_not_called()
         execute_action.assert_not_called()
 
         execute_task.assert_called()
         assert(execute_task.call_count == 3)
         for call in execute_task.call_args_list:
-            assert(call.args[0].name in ["first", "second", "third"])
+            assert(str(call.args[0].name) in ["default::first", "default::second", "default::third"])
         ##-- end check result
 
     def test_jobs_expand(self, ctor, mocker, setup):
         ##-- setup
         reporter_m                                    = mocker.MagicMock(spec=Reporter_i)
 
         job1_m                                        = mock_gen.mock_job("first")
@@ -112,57 +114,17 @@
         ##-- check
         tracker_m.update_state.assert_called()
         assert(tracker_m.update_state.call_count == 3)
 
         expand_job.assert_called()
         assert(expand_job.call_count == 3)
 
-        execute_action.assert_not_called()
         execute_task.assert_not_called()
         ##-- end check
 
-    def test_jobs_add_tasks(self, ctor, mocker, setup):
-        ##-- setup
-        reporter_m                         = mocker.MagicMock(spec=Reporter_i)
-
-        job1_m                             = mock_gen.mock_job("first")
-        job2_m                             = mock_gen.mock_job("second")
-        job3_m                             = mock_gen.mock_job("third")
-
-        task_m                             = mock_gen.mock_task_spec("firstTask")
-        job1_m.build.return_value          = [task_m]
-
-        tracker_m                        = mock_gen.mock_tracker(tasks=[job1_m, job2_m, job3_m])
-        runner                             = ctor(tracker=tracker_m, reporter=reporter_m)
-        expand_job                         = mocker.spy(runner, "_expand_job")
-        execute_task                       = mocker.spy(runner, "_execute_task")
-        execute_action                     = mocker.spy(runner, "_execute_action")
-        ##-- end setup
-
-        ##-- pre-check
-        tracker_m.update_state.assert_not_called()
-        ##-- end pre-check
-
-        ## Run:
-        runner(handler=False)
-
-        ##-- Check
-        tracker_m.add_task.assert_called()
-        assert(tracker_m.add_task.call_count == 1)
-        assert(tracker_m.add_task.call_args.args[0] is task_m)
-
-        tracker_m.update_state.assert_called()
-        assert(tracker_m.update_state.call_count == 3)
-
-        expand_job.assert_called()
-        assert(expand_job.call_count == 3)
-
-        execute_action.assert_not_called()
-        execute_task.assert_not_called()
-
     # @pytest.mark.xfail
     def test_tasks_execute_actions(self, ctor, mocker, setup):
         ##-- setup
         reporter_m                                 = mocker.MagicMock(spec=Reporter_i)
 
         task1_m = mock_gen.mock_task("firstTask")
         task2_m = mock_gen.mock_task("secondTask")
```

### Comparing `doot-0.6.1/doot/control/__tests/test_tracker.py` & `doot-0.7.0/doot/control/__tests/test_tracker.py`

 * *Files 24% similar despite different names*

```diff
@@ -12,305 +12,357 @@
 from typing import (Any, Callable, ClassVar, Generic, Iterable, Iterator,
                     Mapping, Match, MutableMapping, Sequence, Tuple, TypeAlias,
                     TypeVar, cast)
 ##-- end imports
 logging = logmod.root
 
 import pytest
+import doot
+doot._test_setup()
+
 import doot.errors
 import doot.structs
 from doot.control.tracker import DootTracker
 from doot._abstract import Task_i
 from doot.utils import mock_gen
 
 @pytest.mark.parametrize("ctor", [DootTracker])
-class TestTracker:
+class TestTrackerBasic:
 
     def test_initial(self, ctor):
         tracker = ctor()
         assert(tracker is not None)
 
+    @pytest.mark.skip("TODO")
+    def test_clear(self, ctor):
+        pass
+
+    @pytest.mark.skip("TODO")
+    def test_validate(self, ctor):
+        pass
+
+    @pytest.mark.skip("TODO")
+    def test_task_state(self, ctor):
+        pass
+
+    @pytest.mark.skip("TODO")
+    def test_update_task_state(self, ctor):
+        pass
+
+@pytest.mark.parametrize("ctor", [DootTracker])
+class TestTrackerArtifacts:
+
+    @pytest.mark.xfail
+    def test_task_exact_artifact_dependency(self, ctor, mocker):
+        tracker = ctor()
+        for task in mock_gen.task_network({"task1"     : [[pl.Path("test.file")], []],
+                                           "subtask"   : [[], [pl.Path("blah.other")]],
+                                           "subtask2"  : [[], [pl.Path("test.file")]],
+
+                                          }):
+            tracker.add_task(task)
+
+        next_task = tracker.next_for("default::task1")
+        assert(next_task.name == "default::subtask2")
+
+    @pytest.mark.skip
+    def test_task_inexact_artifact_dependency(self, ctor, mocker):
+        tracker = ctor()
+        for task in mock_gen.task_network({"task1"     : [[pl.Path("*.file")], []],
+                                           "subtask"   : [[], [pl.Path("blah.other")]],
+                                           "subtask2"  : [[], [pl.Path("test.file")]],
+
+                                          }):
+            tracker.add_task(task)
+
+        next_task = tracker.next_for("default::task1")
+        assert(isinstance(next_task, doot.structs.DootTaskArtifact))
+
+    @pytest.mark.xfail
+    def test_task_artifact_exists(self, ctor, mocker):
+        """
+          check that if artifacts exist, tasks that generate them aren't queued
+        """
+        mocker.patch.object(pl.Path, "exists", return_value=True)
+        tracker = ctor()
+        for task in mock_gen.task_network({"task1"     : [[pl.Path("*.file")], []],
+                                           "subtask"   : [[], [pl.Path("blah.other")]],
+                                           "subtask2"  : [[], [pl.Path("test.file")]],
+
+                                          }):
+            tracker.add_task(task)
+
+        next_task = tracker.next_for("default::task1")
+        assert(isinstance(next_task, doot.structs.DootTaskArtifact))
+
+    @pytest.mark.skip
+    def test_task_artifact_doesnt_exists(self, ctor, mocker):
+        mocker.patch.object(pl.Path, "exists", return_value=False)
+        tracker = ctor()
+        for task in mock_gen.task_network({"task1"     : [[pl.Path("*.file")], []],
+                                           "subtask"   : [[], [pl.Path("blah.other")]],
+                                           "subtask2"  : [[], [pl.Path("test.file")]],
+
+                                          }):
+            tracker.add_task(task)
+
+        next_task = tracker.next_for("default::task1")
+        assert(isinstance(next_task, doot.structs.DootTaskArtifact))
+
+    @pytest.mark.xfail
+    def test_task_artifact_partial_exists(self, ctor, mocker):
+
+        def temp_exists(self):
+            return not "*" in self.stem
+
+        mocker.patch.object(pl.Path, "exists", new=temp_exists)
+        tracker = ctor()
+        for task in mock_gen.task_network({"task1"     : [[pl.Path("*.file")], []],
+                                           "subtask"   : [[], [pl.Path("blah.other")]],
+                                           "subtask2"  : [[], [pl.Path("test.file")]],
+
+                                          }):
+            tracker.add_task(task)
+
+        next_task = tracker.next_for("default::task1")
+        assert(isinstance(next_task, doot.structs.DootTaskArtifact))
+
+@pytest.mark.parametrize("ctor", [DootTracker])
+class TestTrackerInsertion:
+
     def test_add_task(self, ctor, mocker):
         mock_task = mock_gen.mock_task("task1")
         tracker = ctor()
         tracker.add_task(mock_task)
 
-        assert("task1" in tracker.tasks)
-        assert(tracker.task_graph.nodes['task1']['state'] == tracker.state_e.DEFINED)
+        assert("default::task1" in tracker.tasks)
+        assert(tracker.task_graph.nodes['default::task1']['state'] == tracker.state_e.DEFINED)
 
     def test_duplicate_add_fail(self, ctor, mocker):
         """ dont add a duplicately named task, or its dependencies """
         task1 = mock_gen.mock_task("task1")
         task2 = mock_gen.mock_task("task1")
 
         tracker = ctor()
         tracker.add_task(task1)
         with pytest.raises(doot.errors.DootTaskTrackingError):
             tracker.add_task(task2)
 
-        assert("task1" in tracker.tasks)
+        assert("default::task1" in tracker.tasks)
 
     def test_duplicate_add(self, ctor, mocker):
         task1 = mock_gen.mock_task("task1")
         task2 = mock_gen.mock_task("task1")
 
         tracker = ctor(shadowing=True)
         tracker.add_task(task1)
         tracker.add_task(task2)
 
-        assert("task1" in tracker.tasks)
-
-    def test_contains_defined(self, ctor, mocker):
-        mock_task = mock_gen.mock_task("test_task")
-        mock_task.depends_on = ["example", "blah"]
-
-        tracker = ctor()
-        tracker.add_task(mock_task)
-        # defined Task is contained
-        assert("test_task" in tracker)
-
+        assert("default::task1" in tracker.tasks)
 
     def test_warn_on_undefined(self, ctor, mocker, caplog):
         """ create a task with undefined dependencies, it should just warn not error """
         tracker = ctor()
         for task in mock_gen.task_network({"task1"     : [["subtask", "subtask2"], []]}):
             tracker.add_task(task)
 
-        assert(tracker.next_for("task1").name is "task1")
+        assert(tracker.next_for("default::task1").name == "default::task1")
         assert(bool([x for x in caplog.records if x.levelname == "WARNING"]))
         assert("Tried to Schedule a Declared but Undefined Task: subtask" in caplog.messages)
         assert("Tried to Schedule a Declared but Undefined Task: subtask2" in caplog.messages)
 
-    def test_not_contains_declared(self, ctor, mocker):
-        mock_task = mock_gen.mock_task("test_task", pre=["example", "blah"])
-
-        tracker = ctor()
-        tracker.add_task(mock_task)
-        assert("example" not in tracker)
-        assert("blah" not in tracker)
-
+    @pytest.mark.skip
     def test_task_prior_registration(self, ctor, mocker):
         mock_task = mock_gen.mock_task("test_task")
-        mock_task.depends_on.append("example")
-        mock_task.depends_on.append("blah")
+        mock_task.spec.depends_on.append("example")
+        mock_task.spec.depends_on.append("blah")
 
         tracker = ctor()
         tracker.add_task(mock_task)
+
         assert(tracker.task_graph.nodes['example']['state'] == tracker.state_e.DECLARED)
         assert(tracker.task_graph.nodes['blah']['state'] == tracker.state_e.DECLARED)
         assert("example" in tracker.task_graph)
         assert("blah" in tracker.task_graph)
 
+    @pytest.mark.skip
     def test_task_post_registration(self, ctor, mocker):
         mock_task = mock_gen.mock_task("test_task")
-        mock_task.required_for.append("example")
-        mock_task.required_for.append("blah")
+        mock_task.required_for.append(doot.structs.DootTaskName.build("example"))
+        mock_task.required_for.append(doot.structs.DootTaskName.build("blah"))
 
         tracker = ctor()
         tracker.add_task(mock_task)
-        assert(tracker.task_graph.nodes['example']['state'] == tracker.state_e.DECLARED)
-        assert(tracker.task_graph.nodes['blah']['state'] == tracker.state_e.DECLARED)
-        assert("example" in tracker.task_graph)
-        assert("blah" in tracker.task_graph)
+        assert(tracker.task_graph.nodes['default::example']['state'] == tracker.state_e.DECLARED)
+        assert(tracker.task_graph.nodes['default::blah']['state'] == tracker.state_e.DECLARED)
+        assert("default::example" in tracker.task_graph)
+        assert("default::blah" in tracker.task_graph)
 
+    @pytest.mark.skip
     def test_declared_set(self, ctor, mocker):
         mock_task = mock_gen.mock_task("test_task")
-        mock_task.depends_on   += ["subtask", "sub2"]
-        mock_task.required_for += ["example", "blah"]
+        mock_task.depends_on   += map(doot.structs.DootTaskName.build, ["subtask", "sub2"])
+        mock_task.required_for += map(doot.structs.DootTaskName.build, ["example", "blah"])
 
         tracker = ctor()
         tracker.add_task(mock_task)
         declared = tracker.declared_set()
-        assert(declared == {"__root", "test_task", "subtask","sub2", "example", "blah"})
+        assert(declared == {"__root", "default::test_task", "default::subtask","default::sub2", "default::example", "default::blah"})
 
     def test_defined_set(self, ctor, mocker):
         mock_task = mock_gen.mock_task("test_task")
 
         tracker = ctor()
         tracker.add_task(mock_task)
 
         defined = tracker.defined_set()
-        assert(defined == {"test_task"})
+        assert(defined == {"default::test_task"})
+
+    def test_contains_defined(self, ctor, mocker):
+        mock_task = mock_gen.mock_task("test_task")
+        mock_task.depends_on = ["example", "blah"]
+
+        tracker = ctor()
+        tracker.add_task(mock_task)
+        # defined Task is contained
+        assert("default::test_task" in tracker)
+
+    def test_not_contains_declared(self, ctor, mocker):
+        mock_task = mock_gen.mock_task("test_task", pre=["example", "blah"])
+
+        tracker = ctor()
+        tracker.add_task(mock_task)
+        assert("example" not in tracker)
+        assert("blah" not in tracker)
+
+    @pytest.mark.skip("TODO")
+    def test_late_count(self, ctor):
+        pass
+
+@pytest.mark.parametrize("ctor", [DootTracker])
+class TestTrackerUpdate:
 
     def test_task_order(self, ctor, mocker):
         tasks = mock_gen.task_network({
-            "task1"   : [["subtask", "subtask2"], []],
-            "subtask" : [["subsub"], []],
-            "subtask2": [["subsub"], []],
+            "task1"   : [["default::subtask", "default::subtask2"], []],
+            "subtask" : [["default::subsub"], []],
+            "subtask2": [["default::subsub"], []],
             "subsub"  : [[], []]
          })
 
         tracker  = ctor()
         for task in tasks:
             tracker.add_task(task)
 
-        next_task = tracker.next_for("task1")
-        assert(next_task.name == "subsub")
+        next_task = tracker.next_for("default::task1")
+        assert(next_task.name == "default::subsub")
         tracker.update_state(next_task, tracker.state_e.SUCCESS)
 
         next_task_2 = tracker.next_for()
-        assert(next_task_2.name in {"subtask", "subtask2"})
+        assert(next_task_2.name in {"default::subtask", "default::subtask2"})
         tracker.update_state(next_task_2, tracker.state_e.SUCCESS)
 
         next_task_3 = tracker.next_for()
-        assert(next_task_3.name in {"subtask", "subtask2"} - {next_task_2.name})
+        assert(next_task_3.name in {"default::subtask", "default::subtask2"} - {next_task_2.name})
         tracker.update_state(next_task_3, tracker.state_e.SUCCESS)
 
         next_task_4 = tracker.next_for()
-        assert(next_task_4.name in "task1")
+        assert(next_task_4.name in "default::task1")
 
     def test_task_iter(self, ctor, mocker):
         tasks = mock_gen.task_network({
-            "task1"   : [["subtask", "subtask2", "subtask3"], []],
-            "subtask" : [["subsub"], []],
-            "subtask2": [["subsub"], []],
-            "subtask3": [["subsub"], []],
+            "task1"   : [["default::subtask", "default::subtask2", "default::subtask3"], []],
+            "subtask" : [["default::subsub"], []],
+            "subtask2": [["default::subsub"], []],
+            "subtask3": [["default::subsub"], []],
             "subsub"  : [[], []]
          })
 
         tasks[0].priority = 0
 
         tracker             = ctor()
         for task in tasks:
             tracker.add_task(task)
 
         result_tasks = []
-        tracker.queue_task("task1")
+        tracker.queue_task("default::task1")
         for x in tracker:
             if x:
                 result_tasks.append(x.name)
                 tracker.update_state(x.name, tracker.state_e.SUCCESS)
 
         assert(len(result_tasks) == 5)
 
     def test_task_iter_state_changed(self, ctor, mocker):
         tracker  = ctor()
-        for task in mock_gen.task_network({"task1"   : [["subtask", "subtask2", "subtask3"], []],
-                                           "subtask" : [["subsub"], []],
-                                           "subtask2": [["subsub"], []],
-                                           "subtask3": [["subsub"], []],
+        for task in mock_gen.task_network({"task1"   : [["default::subtask", "default::subtask2", "default::subtask3"], []],
+                                           "subtask" : [["default::subsub"], []],
+                                           "subtask2": [["default::subsub"], []],
+                                           "subtask3": [["default::subsub"], []],
                                            "subsub"  : [[], []]
                                           }):
             tracker.add_task(task)
 
-        tracker.update_state("subtask2", tracker.state_e.SUCCESS)
+        tracker.update_state("default::subtask2", tracker.state_e.SUCCESS)
         tasks = []
-        tracker.queue_task("task1")
+        tracker.queue_task("default::task1")
         for x in tracker:
             if x:
                 tasks.append(x.name)
                 tracker.update_state(x.name, tracker.state_e.SUCCESS)
 
-        assert("subtask2" not in tasks)
+        assert("default::subtask2" not in tasks)
         assert(len(tasks) == 4)
 
     @pytest.mark.xfail
     def test_task_failure(self, ctor, mocker, caplog):
         tracker = ctor()
-        for task in mock_gen.task_network({"task1"   : [["subtask"], []],
-                                           "subtask" : [["subsub"], []],
+        for task in mock_gen.task_network({"task1"   : [["default::subtask"], []],
+                                           "subtask" : [["default::subsub"], []],
                                           }):
             tracker.add_task(task)
 
-        result = tracker.next_for("task1")
-        assert(result.name == "subtask")
+        result = tracker.next_for("default::task1")
+        assert(result.name == "default::subtask")
         tracker.update_state(result, tracker.state_e.SUCCESS)
-        assert(tracker.next_for().name == "task1")
+        assert(tracker.next_for().name == "default::task1")
         assert("Tried to Schedule a Declared but Undefined Task: subsub" in caplog.messages)
 
-
     def test_post_task_order(self, ctor, mocker):
         tracker = ctor()
-        for task in mock_gen.task_network({"task1"     : [["subtask", "subtask2"], []],
-                                           "subtask"   : [["subsub"], ["sidesuper"]],
+        for task in mock_gen.task_network({"task1"     : [["default::subtask", "default::subtask2"], []],
+                                           "subtask"   : [["default::subsub"], ["default::sidesuper"]],
                                            "subtask2"  : [[], []],
                                            "subsub"    : [[], []],
                                            "sidesuper" : [[], []],
 
                                           }):
             tracker.add_task(task)
 
-        next_task = tracker.next_for("task1")
-        assert(next_task.name == "subtask2")
+        next_task = tracker.next_for("default::task1")
+        assert(next_task.name == "default::subtask2")
         tracker.update_state(next_task, tracker.state_e.SUCCESS)
 
         next_task_2 = tracker.next_for()
-        assert(next_task_2.name == "subsub")
+        assert(next_task_2.name == "default::subsub")
         tracker.update_state(next_task_2, tracker.state_e.SUCCESS)
 
         next_task_3 = tracker.next_for()
-        assert(next_task_3.name == "subtask")
+        assert(next_task_3.name == "default::subtask")
         tracker.update_state(next_task_3, tracker.state_e.SUCCESS)
 
         next_task_4 = tracker.next_for()
-        assert(next_task_4.name == "task1" )
-
-    def test_task_exact_artifact_dependency(self, ctor, mocker):
-        tracker = ctor()
-        for task in mock_gen.task_network({"task1"     : [[pl.Path("test.file")], []],
-                                           "subtask"   : [[], [pl.Path("blah.other")]],
-                                           "subtask2"  : [[], [pl.Path("test.file")]],
-
-                                          }):
-            tracker.add_task(task)
-
-        next_task = tracker.next_for("task1")
-        assert(next_task.name == "subtask2")
-
-    def test_task_inexact_artifact_dependency(self, ctor, mocker):
-        tracker = ctor()
-        for task in mock_gen.task_network({"task1"     : [[pl.Path("*.file")], []],
-                                           "subtask"   : [[], [pl.Path("blah.other")]],
-                                           "subtask2"  : [[], [pl.Path("test.file")]],
-
-                                          }):
-            tracker.add_task(task)
-
-        next_task = tracker.next_for("task1")
-        assert(isinstance(next_task, doot.structs.DootTaskArtifact))
-
-    def test_task_artifact_exists(self, ctor, mocker):
-        """
-          check that if artifacts exist, tasks that generate them aren't queued
-        """
-        mocker.patch.object(pl.Path, "exists", return_value=True)
-        tracker = ctor()
-        for task in mock_gen.task_network({"task1"     : [[pl.Path("*.file")], []],
-                                           "subtask"   : [[], [pl.Path("blah.other")]],
-                                           "subtask2"  : [[], [pl.Path("test.file")]],
-
-                                          }):
-            tracker.add_task(task)
-
-
-        next_task = tracker.next_for("task1")
-        assert(isinstance(next_task, doot.structs.DootTaskArtifact))
-
-    def test_task_artifact_doesnt_exists(self, ctor, mocker):
-        mocker.patch.object(pl.Path, "exists", return_value=False)
-        tracker = ctor()
-        for task in mock_gen.task_network({"task1"     : [[pl.Path("*.file")], []],
-                                           "subtask"   : [[], [pl.Path("blah.other")]],
-                                           "subtask2"  : [[], [pl.Path("test.file")]],
-
-                                          }):
-            tracker.add_task(task)
-
-        next_task = tracker.next_for("task1")
-        assert(isinstance(next_task, doot.structs.DootTaskArtifact))
-
-    def test_task_artifact_partial_exists(self, ctor, mocker):
+        assert(next_task_4.name == "default::task1" )
 
-        def temp_exists(self):
-            return not "*" in self.stem
+class TestTrackerPersistence:
 
-        mocker.patch.object(pl.Path, "exists", new=temp_exists)
-        tracker = ctor()
-        for task in mock_gen.task_network({"task1"     : [[pl.Path("*.file")], []],
-                                           "subtask"   : [[], [pl.Path("blah.other")]],
-                                           "subtask2"  : [[], [pl.Path("test.file")]],
+    @pytest.mark.skip("TODO")
+    def test_all_state(self):
+        pass
 
-                                          }):
-            tracker.add_task(task)
+    @pytest.mark.skip("TODO")
+    def test_write(self):
+        pass
 
-        next_task = tracker.next_for("task1")
-        assert(isinstance(next_task, doot.structs.DootTaskArtifact))
+    @pytest.mark.skip("TODO")
+    def test_read(self):
+        pass
```

### Comparing `doot-0.6.1/doot/control/base_runner.py` & `doot-0.7.0/doot/control/base_runner.py`

 * *Files 21% similar despite different names*

```diff
@@ -30,54 +30,55 @@
 
 ##-- lib imports
 import more_itertools as mitz
 ##-- end lib imports
 
 ##-- logging
 logging = logmod.getLogger(__name__)
-##-- end logging
-
 printer = logmod.getLogger("doot._printer")
+##-- end logging
 
 from collections import defaultdict
 import doot
-import doot.constants
 import doot.errors
 from doot.enums import ReportEnum, ActionResponseEnum as ActRE, TaskStateEnum
 from doot._abstract import Job_i, Task_i, FailPolicy_p
-from doot._abstract import TaskTracker_i, TaskRunner_i, TaskBase_i, ReportLine_i, Action_p, Reporter_i
-from doot.structs import DootTaskArtifact
+from doot._abstract import TaskTracker_i, TaskRunner_i, Task_i, ReportLine_i, Action_p, Reporter_i
+from doot.structs import DootTaskArtifact, DootActionSpec
 from doot.utils.signal_handler import SignalHandler
 from doot.structs import DootTaskSpec, DootActionSpec
 from doot.utils.log_context import DootLogContext
 
 dry_run                                      = doot.args.on_fail(False).cmd.args.dry_run()
-head_level           : Final[str]            = doot.constants.DEFAULT_HEAD_LEVEL
-build_level          : Final[str]            = doot.constants.DEFAULT_BUILD_LEVEL
-action_level         : Final[str]            = doot.constants.DEFAULT_ACTION_LEVEL
-sleep_level          : Final[str]            = doot.constants.DEFAULT_SLEEP_LEVEL
-execute_level        : Final[str]            = doot.constants.DEFAULT_EXECUTE_LEVEL
-max_steps            : Final[str]            = doot.config.on_fail(100_000).settings.general.max_steps()
+head_level           : Final[str]            = doot.constants.printer.DEFAULT_HEAD_LEVEL
+build_level          : Final[str]            = doot.constants.printer.DEFAULT_BUILD_LEVEL
+action_level         : Final[str]            = doot.constants.printer.DEFAULT_ACTION_LEVEL
+sleep_level          : Final[str]            = doot.constants.printer.DEFAULT_SLEEP_LEVEL
+execute_level        : Final[str]            = doot.constants.printer.DEFAULT_EXECUTE_LEVEL
+enter_level          : Final[str]            = doot.constants.printer.DEFAULT_ENTER_LEVEL
+max_steps            : Final[str]            = doot.config.on_fail(100_000).settings.tasks.max_steps()
+fail_prefix          : Final[str]            = doot.constants.printer.FAILURE_PREFIX
 
 default_SLEEP_LENGTH : Fina[int|float]       = doot.config.on_fail(0.2, int|float).settings.tasks.sleep.task()
 logctx               : Final[DootLogContext] = DootLogContext(printer)
 
 class BaseRunner(TaskRunner_i):
     """ An incomplete implementation for runners to extend """
 
     def __init__(self:Self, *, tracker:TaskTracker_i, reporter:Reporter_i, policy=None):
-        self.tracker              = tracker
-        self.reporter             = reporter
-        self.policy               = policy
-        self.step                 = 0
-        self._enter_msg = "---------- Task Loop Starting ----------"
-        self._exit_msg  = "---------- Task Loop Finished ----------"
+        self.tracker                                          = tracker
+        self.reporter                                         = reporter
+        self.policy                                           = policy
+        self.step                                             = 0
+        self._signal_failure : None|doot.errors.DootError     = None
+        self._enter_msg                                       = "---------- Task Loop Starting ----------"
+        self._exit_msg                                        = "---------- Task Loop Finished ----------"
 
     def __enter__(self) -> Any:
-        printer.info("- Validating Task Network, building remaining abstract tasks")
+        printer.info("- Validating Task Network, building remaining abstract tasks: %s", self.tracker.late_count)
         self.tracker.validate()
         printer.info(self._enter_msg, extra={"colour" : "green"})
         return
 
     def __exit__(self, exc_type, exc_value, exc_traceback) -> bool:
         printer.setLevel("INFO")
         printer.info("")
@@ -91,45 +92,57 @@
         """
         logging.info("Task Running Completed")
         if self.step >= max_steps:
             printer.info("Runner Hit the Step Limit: %s", max_steps)
 
         printer.info("Final Summary: ")
         printer.info(str(self.reporter), extra={"colour":"magenta"})
+        match self._signal_failure:
+            case None:
+                return
+            case doot.errors.DootError():
+                raise self._signal_failure
 
     def _handle_task_success(self, task):
         if task:
             self.tracker.update_state(task, self.tracker.state_e.SUCCESS)
         return task
 
-    def _handle_failure(self, task, failure):
+    def _handle_failure(self, task:None|Task_i, failure:Error) -> None:
         match failure:
             case doot.errors.DootTaskInterrupt():
                 breakpoint()
-                return failure
-            case doot.errors.DootTaskTrackingError() as err:
-                return err.task
+                pass
             case doot.errors.DootTaskFailed() as err:
-                printer.warning("Task Failed: %s : %s", err.task.name, err)
-                self.tracker.update_state(err.task, self.tracker.state_e.FAILED)
-                return err.task
+                self._signal_failure = err
+                printer.warning("%s %s", fail_prefix, err)
+                self.tracker.update_state(err.task.name, self.tracker.state_e.FAILED)
             case doot.errors.DootTaskError() as err:
-                name = err.task.name if err.task is not None else "unknown"
-                printer.warning("Task Error : %s : %s", name, err)
-                self.tracker.update_state(err.task, self.tracker.state_e.FAILED)
-                return err.task
+                self._signal_failure = err
+                printer.warning("%s %s", fail_prefix, err)
+                self.tracker.update_state(err.task.name, self.tracker.state_e.FAILED)
             case doot.errors.DootError() as err:
-                printer.warning("Doot Error : %s", err)
-                return failure
+                self._signal_failure = err
+                printer.warning("%s %s", fail_prefix, err)
+                self.tracker.update_state(task, self.tracker.state_e.FAILED)
+            case doot.errors.DootTaskTrackingError() as err:
+                self._signal_failure = err
+                printer.warning("%s %s", fail_prefix, err)
+                self.tracker.clear_queue()
             case _:
-                return failure
+                self._signal_failure = doot.errors.DootError("Unknown Failure")
+                printer.exception("%s Unknown failure occurred: %s", fail_prefix, failure)
+                self.tracker.clear_queue()
 
     def _sleep(self, task):
-        if task is None:
-            return
+        match task:
+            case None:
+                return
+            case DootTaskArtifact():
+                return
 
         with logctx(task.spec.print_levels.on_fail(sleep_level).sleep()) as p:
             sleep_len = task.spec.extra.on_fail(default_SLEEP_LENGTH, int|float).sleep()
             p.info("[Sleeping (%s)...]", sleep_len, extra={"colour":"white"})
             time.sleep(sleep_len)
             self.step += 1
```

### Comparing `doot-0.6.1/doot/control/base_tracker.py` & `doot-0.7.0/doot/control/base_tracker.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,53 +30,52 @@
 
 ##-- lib imports
 import more_itertools as mitz
 ##-- end lib imports
 
 ##-- logging
 logging = logmod.getLogger(__name__)
-##-- end logging
-
 printer = logmod.getLogger("doot._printer")
+##-- end logging
 
 import networkx as nx
 import boltons.queueutils
 from collections import defaultdict
 import tomlguard
 import doot
 import doot.errors
-import doot.constants as const
-from doot.enums import TaskStateEnum
+from doot.enums import TaskStateEnum, TaskQueueMeta
 from doot._abstract import Job_i, Task_i, FailPolicy_p
-from doot.structs import DootTaskArtifact, DootTaskSpec, DootTaskName, DootCodeReference
-from doot._abstract import TaskTracker_i, TaskRunner_i, TaskBase_i
+from doot.structs import DootTaskArtifact, DootTaskSpec, DootTaskName, DootCodeReference, DootActionSpec
+from doot._abstract import TaskTracker_i, TaskRunner_i, Task_i
 from doot.task.base_task import DootTask
 
 ROOT             : Final[str]                  = "__root" # Root node of dependency graph
 STATE            : Final[str]                  = "state"  # Node attribute name
 PRIORITY         : Final[str]                  = "priority"
 COMPLETE_STATES  : Final[set[TaskStateEnum]]   = {TaskStateEnum.SUCCESS, TaskStateEnum.EXISTS}
 DECLARE_PRIORITY : Final[int]                  = 10
 MIN_PRIORITY     : Final[int]                  = -10
 
 class EDGE_E(enum.Enum):
+    """ Enum describing the possible edges of the task tracker's task network """
     TASK               = enum.auto()
     ARTIFACT           = enum.auto()
     TASK_CROSS         = enum.auto() # Task to artifact
     ARTIFACT_CROSS     = enum.auto() # artifact to task
 
 class _InternalTrackerBase(TaskTracker_i):
     """ Standard implementation of private tracker methods and plumbing """
 
     state_e            = TaskStateEnum
     INITIAL_TASK_STATE = TaskStateEnum.DEFINED
 
     def __init__(self, shadowing:bool=False, *, policy=None):
         self.policy                                                              = policy
-        self.tasks                   : dict[str, TaskBase_i]                     = {}
+        self.tasks                   : dict[str, Task_i]                         = {}
         self.artifacts               : dict[str, DootTaskArtifact]               = {}
         self.task_graph              : nx.DiGraph                                = nx.DiGraph()
         self.active_set              : list[str|DootTaskName|DootTaskArtifact]   = set()
         self.execution_path          : list[str]                                 = []
         self.shadowing               : bool                                      = shadowing
         self._root_name              : str                                       = ROOT
         self._build_late             : list[str]                                 = list()
@@ -97,163 +96,170 @@
             logging.info("Tracker Queue: %s", self.active_set)
             yield self.next_for()
 
     def __contains__(self, target:str) -> bool:
         # TODO handle definite artifacts -> indefinite artifacts
         return target in self.tasks
 
-    def _prep_artifact(self, artifact:DootTaskArtifact) -> str:
-        """ convert a path to an artifact, and connect it with matching artifacts """
-        match artifact:
-            case _ if str(artifact) in self.artifacts:
-                pass
-            case DootTaskArtifact() if artifact.is_definite:
-                self.artifacts[str(artifact)] = artifact
-                self.task_graph.add_node(str(artifact), state=self.state_e.ARTIFACT, priority=self._declare_priority)
-                # connect to indefinites
-                for x in filter(lambda x: (not x.is_definite) and artifact in x, self.artifacts.values()):
-                    self.task_graph.add_edge(str(artifact), str(x), type=EDGE_E.ARTIFACT)
-            case DootTaskArtifact():
-                self.artifacts[str(artifact)] = artifact
-                self.task_graph.add_node(str(artifact), state=self.state_e.ARTIFACT, priority=self._declare_priority)
-                # connect to definites
-                for x in filter(lambda x: x.is_definite and x in artifact, self.artifacts.values()):
-                    self.task_graph.add_edge(str(x), str(artifact), type=EDGE_E.ARTIFACT)
-
-        return str(artifact)
-
-    def _prep_task(self, spec:DootTaskSpec|TaskBase_i) -> TaskBase_i:
-        """ Internal utility method to convert task identifier into actual task """
+    def _prep_task(self, spec:DootTaskSpec|Task_i) -> Task_i:
+        """ Internal utility method to convert task identifier into actual task
+        doesn't modify tracker state
+        """
         # Build the Task if necessary
+
         match spec:
-            case DootTaskSpec(ctor=DootTaskName() as ctor) if str(ctor) in self.tasks:
+            case DootTaskSpec(ctor=str()|DootTaskName() as ctor) if str(ctor) in self.tasks:
                 # specialize a loaded task
-                base_spec          = self.tasks.get(str(ctor)).spec
+                base_spec           = self.tasks.get(str(ctor)).spec
                 initial_specialized = base_spec.specialize_from(spec)
-                cli_specialized    = self._insert_cli_args_into_spec(initial_specialized)
-                if cli_specialized.ctor is None:
-                    raise doot.errors.DootTaskTrackingError("Attempt to specialize task failed: %s", spec.name)
-
-                task : TaskBase_i = cli_specialized.build()
-            case DootTaskSpec(ctor=DootCodeReference() as ctor) if spec.check(ensure=TaskBase_i):
+                cli_specialized     = self._insert_cli_args_into_spec(initial_specialized)
+                task : Task_i       = cli_specialized.make()
+            case DootTaskSpec(ctor=DootCodeReference() as ctor) if spec.check(ensure=Task_i):
+                # Specialized a custom task class
                 cli_specialized   = self._insert_cli_args_into_spec(spec)
-                task : TaskBase_i = cli_specialized.build()
+                task : Task_i     = cli_specialized.make()
             case DootTaskSpec():
                 cli_specialized   = self._insert_cli_args_into_spec(spec)
-                task : TaskBase_i = DootTask(cli_specialized)
-            case TaskBase_i():
+                task : Task_i = DootTask(cli_specialized)
+            case Task_i():
                 task = spec
             case _:
                 raise doot.errors.DootTaskTrackingError("Unknown task attempted to be added: %s", spec)
 
         # Check it doesn't shadow another task
-        match task.name in self.tasks, task.name in self.task_graph: # type: ignore
+        match task.name in self.tasks, task.name in self.task_graph:
             case True, False:
                 raise doot.errors.DootTaskTrackingError("Task exists in defined tasks, but not the task graph")
             case True, True if not self.shadowing:
                 raise doot.errors.DootTaskTrackingError("Task with Duplicate Name not added: ", task.name)
             case True, True:
-                logging.warning("Task Shadowed by Duplicate Name: %s", task.name)
+                logging.warning("Task Shadowed by Duplicate Name: %s", task.readable_name)
             case False, True:
-                logging.debug("Defining a declared dependency task: %s", task.name)
+                logging.debug("Defining a declared dependency task: %s", task.readable_name)
 
         return task
 
-    def _insert_cli_args_into_spec(self, spec:DootTaskSpec):
+    def _add_artifact(self, artifact:DootTaskArtifact) -> str:
+        """ convert a path to an artifact, and connect it with matching artifacts """
+        match artifact:
+            case _ if str(artifact) in self.artifacts: # artifact already known
+                pass
+            case DootTaskArtifact() if artifact.is_definite: # x/y/y.ext
+                self.artifacts[str(artifact)] = artifact
+                self.task_graph.add_node(str(artifact), state=self.state_e.ARTIFACT, priority=self._declare_priority)
+                # connect to matching indefinites
+                for x in filter(lambda x: artifact in x, self.artifacts.values()):
+                    self.task_graph.add_edge(str(artifact), str(x), type=EDGE_E.ARTIFACT)
+            case DootTaskArtifact(): # x/*/*.ext
+                self.artifacts[str(artifact)] = artifact
+                self.task_graph.add_node(str(artifact), state=self.state_e.ARTIFACT, priority=self._declare_priority)
+                # connect to definites
+                for x in filter(lambda x: x in artifact, self.artifacts.values()):
+                    self.task_graph.add_edge(str(x), str(artifact), type=EDGE_E.ARTIFACT)
+
+        return str(artifact)
+
+    def _insert_cli_args_into_spec(self, spec:DootTaskSpec) -> DootTaskSpec:
+        """ Takes a task spec, and inserts matching cli args into it if necessary """
         spec_extra : dict = dict(spec.extra.items() or [])
 
         for cli in spec.extra.on_fail([]).cli():
-            spec_extra[cli.name] = cli.default
+            if cli.name not in spec_extra:
+                spec_extra[cli.name] = cli.default
 
         if spec.name not in doot.args.on_fail({}).tasks():
             spec.extra = tomlguard.TomlGuard(spec_extra)
             return spec
 
         for key,val in doot.args.tasks[str(spec.name)].items():
             spec_extra[key] = val
 
         spec.extra = tomlguard.TomlGuard(spec_extra)
+
         return spec
 
     def _insert_dependencies(self, task):
+        """ insert a task's dependencies into the network, connecting them to the task """
         for pre in task.depends_on:
-            logging.debug("Connecting Dependency: %s -> %s", pre, task.name)
+            logging.debug("Connecting Dependency: %s -> %s", pre, task.readable_name)
             match pre:
-                case {"task": taskname}:
-                    raise TypeError("Task Deps should not longer be dicts")
-                case pl.Path():
-                    pre = self._prep_artifact(DootTaskArtifact(pre))
-                    self.task_graph.add_edge(pre, task.name, type=EDGE_E.ARTIFACT_CROSS)
+                case DootActionSpec():
+                    # Action spec dependencies are tested when running, not as part of the DAG
+                    pass
                 case DootTaskArtifact():
-                    pre = self._prep_artifact(pre)
+                    pre = self._add_artifact(pre)
                     self.task_graph.add_edge(pre, task.name, type=EDGE_E.ARTIFACT_CROSS)
                 case DootTaskName() if all([(in_graph:=str(pre) in self.task_graph),(has_args:=bool(pre.args))]):
                     base_spec                 = self.tasks[str(pre)].spec
-                    name_spec                 = DootTaskSpec.from_name(pre)
+                    name_spec                 = DootTaskSpec.build(pre)
                     name_spec.ctor            = base_spec.name
                     name_spec.required_for.append(task.name)
-                    self.add_task(name_spec)
+                    self.add_task(name_spec, no_root_connection=True)
                 case DootTaskName() if in_graph and not has_args:
                     # just connect if the tracker already knows the task
                     self.task_graph.add_edge(str(pre), task.name, type=EDGE_E.TASK)
                 case DootTaskName() if has_args:
                     assert(str(pre) not in self.task_graph.nodes)
-                    name_spec      = DootTaskSpec.from_name(pre.specialize(info="late"))
+                    name_spec      = DootTaskSpec.build(pre.specialize(info="late"))
                     name_spec.ctor = pre
                     name_spec.required_for.append(task.name)
                     self._build_late.append(name_spec)
                 case str() | DootTaskName():
+                    logging.debug("Adding Dummy Dependency Task: %s -> %s", task.readable_name, pre)
                     # Otherwise add a dummy task until its defined
                     self.task_graph.add_node(str(pre), state=self.state_e.DECLARED, priority=self._declare_priority)
                     self.task_graph.add_edge(str(pre), task.name, type=EDGE_E.TASK)
                 case _:
                     raise doot.errors.DootTaskTrackingError("Unknown dependency task attempted to be added: %s", pre)
 
     def _insert_dependents(self, task):
+        """ insert a task's downstream dependents into the network, connecting them to the task """
         for post in task.required_for:
-            logging.debug("Connecting Successor: %s -> %s", task.name, post)
+            logging.debug("Connecting Successor: %s -> %s", task.readable_name, post)
             match post:
-                case {"task": taskname}:
-                    raise TypeError("Task Deps should not longer be dicts")
-                case pl.Path():
-                    post = self._prep_artifact(DootTaskArtifact(post))
-                    self.task_graph.add_edge(task.name, post, type=EDGE_E.TASK_CROSS)
+                case DootActionSpec():
+
+                    pass
                 case DootTaskArtifact():
-                    post = self._prep_artifact(post)
+                    post = self._add_artifact(post)
                     self.task_graph.add_edge(task.name, post, type=EDGE_E.TASK_CROSS)
-
                 case DootTaskName() if all([(in_graph:=str(post) in self.task_graph), (has_args:=bool(post.args))]):
                     base_spec                 = self.tasks[str(post)].spec
-                    name_spec                 = DootTaskSpec.from_name(post)
+                    name_spec                 = DootTaskSpec.build(post)
                     name_spec.ctor            = base_spec.name
                     name_spec.depends_on.append(task.name)
                     self.add_task(name_spec)
                 case DootTaskName() if in_graph and not has_args:
                     # just connect if the tracker already knows the task
                     self.task_graph.add_edge(task.name, str(post), type=EDGE_E.TASK)
                 case DootTaskName() if has_args:
                     assert(str(post) not in self.task_graph.nodes)
-                    name_spec      = DootTaskSpec.from_name(post.specialize(info="late"))
+                    name_spec      = DootTaskSpec.build(post.specialize(info="late"))
                     name_spec.ctor = post
                     name_spec.depends_on.append(task.name)
                     self._build_late.append(name_spec)
                 case str() | DootTaskName():
+                    logging.debug("Adding Dummy Dependent Task: %s -> %s", task.readable_name, post)
                     # Otherwise add a dummy task until its defined
                     self.task_graph.add_node(str(post), state=self.state_e.DECLARED, priority=self._declare_priority)
                     self.task_graph.add_edge(task.name, str(post), type=EDGE_E.TASK)
                 case _:
                     raise doot.errors.DootTaskTrackingError("Unknown successor task attempted to be added: %s", post)
 
-    def _insert_according_to_queue_behaviour(self, task):
+    def _maybe_implicit_queue(self, task):
+        """ tasks can be activated for running by a number of different conditions
+          this handles that
+          """
         match task.spec.queue_behaviour:
-            case "auto":
+            case TaskQueueMeta.auto:
                 self.queue_task(task.name)
-            case "reactive":
+            case TaskQueueMeta.reactive:
                 self.task_graph.nodes[task.name][REACTIVE_ADD] = True
-            case "default":
+            case TaskQueueMeta.default:
+                # Waits for explicit queue
                 pass
             case _:
                 raise doot.errors.DootTaskTrackingError("Unknown queue behaviour specified: %s", task.spec.queue_behaviour)
 
     def _task_dependencies(self, task) -> tuple[list[str], list[str]]:
         # TODO detect 'read' actions as implicit dependencies
         dependencies = list(self.task_graph.pred[task].keys())
@@ -270,24 +276,27 @@
         incomplete   = list(filter(lambda x: not bool(self.artifacts[x]), artifacts))
 
         return incomplete, artifacts
 
     def _task_dependents(self, task) -> tuple[list[str], list[str]]:
         raise NotImplementedError()
 
-
 class BaseTracker(_InternalTrackerBase):
     """ The public part of the standard tracker implementation """
+
+    @property
+    def late_count(self):
+        """ Get the count of tasks which are to be built after all definnitions are loaded """
+        return len(self._build_late)
+
     def queue_task(self, *tasks:str|DootTaskName|DootTaskArtifact|tuple, silent=False) -> None:
         """
           Add tasks to the queue.
           By default it does *not* complain on trying to re-add already queued tasks,
         """
-        # TODO queue the task's setup task if it exists / hasn't been executed already
-        # TODO if only task name is specified, without group, and theres no ambiguity, accept that
         logging.debug("Queue Request: %s", tasks)
         targets = set()
         for task in tasks:
             # Retrieve the actual task
             match task:
                 case str() | DootTaskName() | DootTaskArtifact() if str(task) in self.active_set:
                     if not silent:
@@ -310,34 +319,37 @@
         logging.debug("Queueing: %s", targets)
         for task in targets:
             if str(task) not in self.active_set:
                 self.active_set.add(str(task))
                 self.task_queue.add(str(task), self.task_graph.nodes[str(task)].get(PRIORITY, self._declare_priority))
 
     def deque_task(self) -> None:
+        """ remove the top task from the queue """
         focus = self.task_queue.pop()
         self.task_graph.nodes[focus][PRIORITY] -= 1
         logging.debug("Task Priority Decrement: %s = %s", focus, self.task_graph.nodes[focus][PRIORITY])
         self.active_set.remove(focus)
 
     def clear_queue(self) -> None:
+        """ Remove everything from the task queue """
         # TODO queue the task's failure/cleanup task
         self.active_set =  set()
         self.task_queue = boltons.queueutils.HeapPriorityQueue()
 
     def validate(self) -> bool:
         """ Finalise and ensure consistence of the task network.
         run tests to check the dependency graph is acceptable
         """
         logging.debug("Building %s abstract tasks", len(self._build_late))
         while bool(self._build_late):
             curr = self._build_late.pop()
             assert(isinstance(curr, DootTaskSpec))
             self.add_task(curr)
 
+        logging.debug("Validating Graph")
         return all([nx.is_directed_acyclic_graph(self.task_graph),
                     self.declared_set() == self.defined_set()
                    ])
 
     def declared_set(self) -> set[str]:
         """ Get the set of tasks which have been declared, directly or indirectly """
         return set(self.task_graph.nodes)
@@ -355,13 +367,13 @@
 
     def all_states(self) -> dict:
         """ Get a dict of all tasks, and their current state """
         nodes = self.task_graph.nodes
         return {x: y[STATE] for x,y in nodes.items()}
 
     def write(self, target:pl.Path) -> None:
-        """ Write the dependency graph to a file """
+        """ TODO Write the dependency graph to a file """
         raise NotImplementedError()
 
     def read(self, target:pl.Path) -> None:
-        """ Read the dependency graph from a file """
+        """ TODO Read the dependency graph from a file """
         raise NotImplementedError()
```

### Comparing `doot-0.6.1/doot/control/date_tracker.py` & `doot-0.7.0/doot/cmds/clean_cmd.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,83 +3,70 @@
 
 """
 ##-- imports
 from __future__ import annotations
 
 # import abc
 # import datetime
-import enum
+# import enum
 import functools as ftz
 import itertools as itz
 import logging as logmod
 import pathlib as pl
 import re
 import time
 import types
 # from copy import deepcopy
 # from dataclasses import InitVar, dataclass, field
 from typing import (TYPE_CHECKING, Any, Callable, ClassVar, Final, Generic,
                     Iterable, Iterator, Mapping, Match, MutableMapping,
                     Protocol, Sequence, Tuple, TypeAlias, TypeGuard, TypeVar,
-                    cast, final, overload, runtime_checkable, Generator, Literal)
+                    cast, final, overload, runtime_checkable)
 # from uuid import UUID, uuid1
 # from weakref import ref
 
-# from bs4 import BeautifulSoup
-import boltons.queueutils
-import networkx as nx
 ##-- end imports
 
 ##-- logging
 logging = logmod.getLogger(__name__)
 ##-- end logging
+printer = logmod.getLogger("doot._printer")
 
-from collections import defaultdict
 import doot
-import doot.errors
-import doot.constants as const
-from doot.enums import TaskStateEnum
-from doot._abstract import Job_i, Task_i, FailPolicy_p
-from doot.structs import DootTaskArtifact, DootTaskSpec, DootTaskName
-from doot._abstract import TaskTracker_i, TaskRunner_i, TaskBase_i
-from doot.task.base_task import DootTask
-from doot.control.tracker import _TrackerEdgeType, DootTracker
+import shutil
+from doot.cmds.base_cmd import BaseCommand
+from collections import defaultdict
 
-STORAGE_FILE : Final[pl.Path] = doot.config.on_fail(DootKey.make(".tasks.bk")).settings.general.tracker_file(wrapper=DootKey.make).to_path()
+clean_locs = doot.config.on_fail([], list).commands.clean.locs()
 
-@doot.check_protocol
-class DootDateTracker(DootTracker):
+class CleanCmd(BaseCommand):
     """
-      Track task status, using file product modification times
-      reads and writes modification times to wherever config.settings.general.tracker_file locates
+      Runs either a general clean command, or a specific task clean command
 
     """
-    def __init__(self, shadowing:bool=False, *, policy=None):
-        super().__init__(shadowing=shadowing, policy=policy)
-        self._modification_db = None
-
-    def write(self, target:pl.Path) -> None:
-        """ Write the dependency graph to a file """
-        # STORAGE_FILE.write_text(str(self._modification_db))
-        raise NotImplementedError()
-
-    def read(self, target:pl.Path) -> None:
-        """ Read the dependency graph from a file """
-        # self._modification_db = STORAGE_FILE.read_text()
-        raise NotImplementedError()
-
-    def update_state(self, task:str|TaskBase_i|DootTaskArtifact|DootTaskName, state:self.state_e):
-        now = datetime.datetime.now()
-        match state:
-            case self.state_e.EXISTS:
-                task_date  = self._modification_db.set(str(task), now)
-                self._invalidate_descendents(task)
-                pass
-            case self.state_e.FAILED:
-                self._invalidate_descendents(task)
+    _name      = "clean"
+    _help      = [
+        "Called with a -t[arget]={task}, will delete locations listed in that task's toml spec'd `clean_targets`",
+        "Without a target, will delete locations listed in doot.toml's: `commands.clean.locs`",
+        "Directories will *not* be deleted unless -r[ecursive] is passed",
+        ]
+
+    @property
+    def param_specs(self) -> list:
+        return super().param_specs + [
+            self.build_param(name="target", type=str, default=None),
+            self.build_param(name="recursive", type=bool, default=False)
+            ]
+
+    def __call__(self, tasks:dict, plugins:dict):
+        self._loc_clean()
+
+    def _loc_clean(self):
+        cleanable = [doo.locs[x] for x in doot.locs if doot.locs.metacheck(x, doot.locs.locmeta.cleanable)]
+        for x in cleanable:
+            if not x.exists():
                 pass
-            case self.state_e.SUCCESS:
-                pass
-
-    def _invalidate_descendents(task):
-        incomplete, descendants = self._task_dependents(task)
-        pass
+            logging.info("Cleaning: %s", x)
+            if x.is_dir():
+                shutil.rmtree(x)
+            else:
+                x.unlink(missing_ok=True)
```

### Comparing `doot-0.6.1/doot/control/locations.py` & `doot-0.7.0/doot/control/locations.py`

 * *Files 13% similar despite different names*

```diff
@@ -23,218 +23,206 @@
 ##-- logging
 logging = logmod.getLogger(__name__)
 # If CLI:
 # logging = logmod.root
 # logging.setLevel(logmod.NOTSET)
 ##-- end logging
 
+import os
 import re
 import tomlguard
+import doot
 from doot.errors import DootDirAbsent, DootLocationExpansionError, DootLocationError
-from doot._structs.artifact import DootTaskArtifact
-from doot._structs.key import DootKey, DootSimpleKey, DootMultiKey, DootNonKey
-from doot.constants import KEY_PATTERN, MAX_KEY_EXPANSIONS
+from doot.structs import DootTaskArtifact, DootKey, TomlLocation
+from doot._structs.key import DootSimpleKey, DootMultiKey, DootNonKey
+from doot.mixins.path_manip import PathManip_m
+from doot.enums import LocationMeta
 
-KEY_PAT        = KEY_PATTERN
-MAX_EXPANSIONS = MAX_KEY_EXPANSIONS
+KEY_PAT        = doot.constants.patterns.KEY_PATTERN
+MAX_EXPANSIONS = doot.constants.patterns.MAX_KEY_EXPANSIONS
 
-class DootLocations:
+class DootLocations(PathManip_m):
     """
-      A Single point of truth for locations that tasks use.
+      A Single point of truth for task access to locations.
       key=value pairs in [[locations]] toml blocks are integrated into it.
-      Also handles key={protect=value} to designate a path shouldn't have files written in it
-      by certain io actions
 
       it expands relative paths according to cwd(),
       but can be used as a context manager to expand from a temp different root
 
       location designations are of the form:
-      key = "location/subdirectory/file"
+      key = 'location/subdirectory/file'
+      simple locations can be accessed as attributes: locs.temp
 
-        If a location value has "loc/{key}/somewhere",
-        then for key = "blah", it will be expanded upon access to "loc/blah/somewhere"
-    """
+      more complex locations, with expansions, are accessed as items:
+      locs['{temp}/somewhere']
+      will expand 'temp' (if it is a registered location)
+      """
+    locmeta = LocationMeta
 
     def __init__(self, root:Pl.Path):
-        self._root    : pl.Path()       = root.expanduser().absolute()
-        self._data    : TomlGuard       = tomlguard.TomlGuard()
-        self._protect : set             = set()
+        self._root    : pl.Path()               = root.expanduser().absolute()
+        self._data    : dict[str, TomlLocation] = dict()
+        self._loc_ctx : None|DootLocations      = None
 
     def __repr__(self):
         keys = ", ".join(iter(self))
         return f"<DootLocations : {str(self.root)} : ({keys})>"
 
     def __getattr__(self, key) -> pl.Path:
         """
           get a location by name from loaded toml
+          delegates to __getitem__
           eg: locs.temp
           """
         if key == "__self__":
             return None
-        return self[DootKey.make(key, strict=True)]
+        return self[DootKey.build(key, strict=True)]
 
     def __getitem__(self, val:str|DootKey|pl.Path|DootTaskArtifact) -> pl.Path:
         """
-          eg: doot.locs["{data}/somewhere"]
+          eg: doot.locs['{data}/somewhere']
           A public utility method to easily convert paths.
+          delegates to DootKey's path expansion
 
           Get a location using item access for extending a stored path.
-          eg: locs["{temp}/imgs/blah.jpg"]
+          eg: locs['{temp}/imgs/blah.jpg']
         """
-        match DootKey.make(val, explicit=True):
+        match DootKey.build(val, explicit=True):
             case DootNonKey() as key:
                 return key.to_path(locs=self)
             case DootSimpleKey() as key:
                 return key.to_path(locs=self)
             case DootMultiKey() as key:
                 return key.to_path(locs=self)
             case _:
                 raise DootLocationExpansionError("Unrecognized location expansion argument", val)
 
     def __contains__(self, key:str|DootKey|pl.Path|DootTaskArtifact):
         """ Test whether a key is a registered location """
         return key in self._data
 
-    def __iter__(self):
+    def __iter__(self) -> Generator[str]:
         """ Iterate over the registered location names """
         return iter(self._data.keys())
 
-    def __call__(self, new_root) -> Self:
+    def __call__(self, new_root=None) -> Self:
         """ Create a copied locations object, with a different root """
-        new_obj = DootLocations(new_root)
+        new_obj = DootLocations(new_root or self._root)
         return new_obj.update(self)
 
     def __enter__(self) -> Any:
+        """ replaces the global doot.locs with this locations obj,
+        and changes the system root to wherever this locations obj uses as root
+        """
+        self._loc_ctx = doot.locs
+        doot.locs = self
+        os.chdir(doot.locs._root)
         return self
 
     def __exit__(self, exc_type, exc_value, exc_traceback) -> bool:
+        """ returns the global state to its original, """
+        assert(self._loc_ctx is not None)
+        doot.locs     = self._loc_ctx
+        os.chdir(doot.locs._root)
+        self._loc_ctx = None
         return False
 
-    def _calc_path(self, base:pl.Path, *, fallback:pl.Path|None=None) -> pl.Path:
-        """
-          Expands a string or key according to registered locations into a path.
-          so if locs = {"base": "~/Desktop", "bloo": "bloo/sub/dir"}
-          then:
-          _calc_path("base") -> "~/Desktop"
-          _calc_path("{base}/blah") -> "~/Desktop/blah"
-          _calc_path("{base}/{bloo}") -> "~/Desktop/bloo/sub/dir"
-        """
-        expansion = pl.Path()
-
-        # Expand each part:
-        try:
-            for part in base.parts:
-                expanded_part = expand_path_part(part.strip(), self._data)
-                # build the total expansion from the parts
-                logging.debug("Expanded %s -> %s", part, expanded_part)
-                expansion /= expanded_part
-        except (DootLocationExpansionError, DootLocationError) as err:
-            if fallback is not None:
-                logging.debug("Expansion failed, using fallback: %s -> %s", base, fallback)
-                expansion = pl.Path(fallback)
-            else:
-                raise err
-
-        logging.debug("Expansion Result: %s", expansion)
-        # Force the path to be absolute
-        match expansion.parts:
-            case []:
-                return self.root
-            case ["~", *_]:  # absolute path or home
-                return expansion.expanduser().absolute()
-            case ["/", *_]:
-                return expansion.absolute()
-            case _:
-                return self.root / expansion
-
     def get(self, key:DootSimpleKey|str, on_fail:None|str|pl.Path=Any) -> None|pl.Path:
         """
           convert a *simple* key of one value to a path.
-          This pairs with DootKey.to_path, which does the heavy lifting of expansions
-          does *not* expand returned paths
+          does *not* recursively expand returned paths
+          More complex expansion is handled in DootKey and subclasses
         """
         assert(isinstance(key,(DootSimpleKey,str))), (str(key), type(key))
         match key:
             case DootNonKey():
                 return pl.Path(key.form)
             case str() | DootSimpleKey() if key in self._data:
-                return pl.Path(self._data[key])
+                return self._data[key].base
             case _ if on_fail is None:
                 return None
             case _ if on_fail != Any:
                 return self.get(on_fail)
             case DootSimpleKey():
                 return pl.Path(key.form)
             case _:
                 return pl.Path(key)
 
-    def expand(self, path:pl.Path, symlinks:bool=False) -> pl.Path:
-        return self.normalize(path, symlinks)
-
     def normalize(self, path:pl.Path, symlinks:bool=False) -> pl.Path:
         """
           Expand a path to be absolute, taking into account the set doot root.
           resolves symlinks unless symlinks=True
         """
-        result = path
-        match result.parts:
-            case ["~", *xs]:
-                result = result.expanduser().resolve()
-            case ["/", *xs]:
-                result = result
-            case _:
-                result = (self.root / path).expanduser().resolve()
+        return self._normalize(path, root=self.root)
 
-        return result
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
 
     @property
     def root(self):
         """
           the registered root location
         """
         return self._root
 
     def update(self, extra:dict|TomlGuard|DootLocations, strict=True) -> Self:
         """
           Update the registered locations with a dict, tomlguard, or other dootlocations obj.
-          The update process itself is tomlguard.tomlguard.merge
         """
-        if isinstance(extra, DootLocations):
-            return self.update(extra._data)
+        match extra: # unwrap to just a dict
+            case dict():
+                pass
+            case tomlguard.TomlGuard():
+                return self.update(extra._table())
+            case DootLocations():
+                return self.update(extra._data)
+            case _:
+                raise doot.errors.DootLocationError("Tried to update locations with unknown type: %s", extra)
 
-        assert(isinstance(extra, (tomlguard.TomlGuard,dict)))
         raw          = dict(self._data.items())
         base_keys    = set(raw.keys())
+        new_keys     = set()
         for k,v in extra.items():
-            match v:
-                case _ if k in raw and strict:
-                    raise DootLocationError("Duplicated Key", k)
-                case str():
-                    raw[k] = v
-                case {"protect": x}:
-                    self._protect.add(k)
-                    raw[k] = x
+            match TomlLocation.build(k, v):
+                case _ if k in new_keys and v != raw[k]:
+                    raise DootLocationError("Duplicated, non-matching Key", k)
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
+                    raise DootLocationError("Couldn't build a TomlLocation for: (%s : %s)", k, v)
 
-        new_keys = set(raw.keys()) - base_keys
         logging.debug("Registered New Locations: %s", ", ".join(new_keys))
-        self._data = tomlguard.TomlGuard(raw)
-
+        self._data = raw
         return self
 
     def ensure(self, *values, task="doot"):
         """ Ensure the values passed in are registered locations,
           error with DootDirAbsent if they aren't
         """
         missing = set(x for x in values if x not in self)
 
         if bool(missing):
             raise DootDirAbsent("Ensured Locations are missing for %s : %s", task, missing)
 
-
-    def check_writable(self, path:pl.Path) -> bool:
-        """ test a path to see if it is relative to a protected location """
-        for key in self._protect:
-            base = getattr(self, key)
-            if path.is_relative_to(base):
-                return False
-
-        return True
+    def _clear(self):
+        self._data = tomlguard.TomlGuard()
```

### Comparing `doot-0.6.1/doot/control/overlord.py` & `doot-0.7.0/doot/control/overlord.py`

 * *Files 11% similar despite different names*

```diff
@@ -30,40 +30,46 @@
 ##-- logging
 logging = logmod.getLogger(__name__)
 printer = logmod.getLogger("doot._printer")
 ##-- end logging
 
 from importlib.metadata import EntryPoint
 
+import sh
+import sys
 import doot
 import doot.errors
-import doot.constants
 import tomlguard
 from doot._abstract import (ArgParser_i, Command_i, CommandLoader_p,
                             Overlord_p, Task_i, Job_i, TaskLoader_p)
 
 from doot.utils.plugin_selector import plugin_selector
 from doot.errors import DootInvalidConfig, DootParseError
 from doot.loaders.cmd_loader import DootCommandLoader
 from doot.loaders.plugin_loader import DootPluginLoader
 from doot.loaders.task_loader import DootTaskLoader
 from doot.parsers.flexible import DootFlexibleParser
+from doot.mixins.param_spec import ParamSpecMaker_m
 
-plugin_loader_key  : Final = doot.constants.DEFAULT_PLUGIN_LOADER_KEY
-command_loader_key : Final = doot.constants.DEFAULT_COMMAND_LOADER_KEY
-task_loader_key    : Final = doot.constants.DEFAULT_TASK_LOADER_KEY
-
-preferred_cmd_loader  = doot.config.on_fail("default").settings.general.loaders.command()
-preferred_task_loader = doot.config.on_fail("default").settings.general.loaders.task()
-preferred_parser      = doot.config.on_fail("default").settings.general.loaders.parser()
+plugin_loader_key  : Final = doot.constants.entrypoints.DEFAULT_PLUGIN_LOADER_KEY
+command_loader_key : Final = doot.constants.entrypoints.DEFAULT_COMMAND_LOADER_KEY
+task_loader_key    : Final = doot.constants.entrypoints.DEFAULT_TASK_LOADER_KEY
+announce_exit      : bool  = doot.constants.misc.ANNOUNCE_EXIT
+announce_voice     : str   = doot.constants.misc.ANNOUNCE_VOICE
 
-defaulted_file = doot.config.on_fail(pl.Path(".doot_defaults.toml"), pl.Path).report.defaulted_file(pl.Path)
+DEFAULT_CLI_CMD    : Final = doot.constants.misc.DEFAULT_CLI_CMD
+
+preferred_cmd_loader       = doot.config.on_fail("default").settings.general.loaders.command()
+preferred_task_loader      = doot.config.on_fail("default").settings.general.loaders.task()
+preferred_parser           = doot.config.on_fail("default").settings.general.loaders.parser()
+
+defaulted_file             = doot.config.on_fail(pl.Path(".doot_defaults.toml"), pl.Path).report.defaulted_file(pl.Path)
 
 @doot.check_protocol
-class DootOverlord(Overlord_p):
+class DootOverlord(ParamSpecMaker_m, Overlord_p):
     """
     Main control point for doot.
     prefers passed in loaders, then plugins it finds.
 
     default cmds are provided by the cmd loader
     """
     _help = ["An opinionated rewrite of Doit"]
@@ -94,18 +100,18 @@
         self._load_tasks(extra_config)
         self._parse_args()
         logging.debug("Core Overlord Initialisation complete")
 
     @property
     def param_specs(self) -> list[DootParamSpec]:
         return [
-           self.make_param(name="version" , prefix="--"),
-           self.make_param(name="help"    , prefix="--"),
-           self.make_param(name="verbose" , prefix="--"),
-           self.make_param(name="debug",    prefix="--")
+           self.build_param(name="version" , prefix="--"),
+           self.build_param(name="help"    , prefix="--"),
+           self.build_param(name="verbose" , prefix="--"),
+           self.build_param(name="debug",    prefix="--")
         ]
 
     @property
     def help(self) -> str:
         help_lines = ["", f"Doot v{doot.__version__}", ""]
         help_lines += self._help
 
@@ -194,15 +200,28 @@
         if doot.args.on_fail(False).head.args.help():
             printer.info(self.help)
 
             return True
 
         return False
 
-    def __call__(self, cmd=None):
+    def _get_cmd(self, cmd=None):
+        if self.current_cmd is not None:
+            return self.current_cmd
+
+        target = cmd or doot.args.on_fail(DEFAULT_CLI_CMD).cmd.name()
+
+        self.current_cmd = self.cmds.get(target, None)
+        if self.current_cmd is None:
+            self._errored = DootParseError("Specified Command Couldn't be Found: %s", target)
+            raise self._errored
+
+        return self.current_cmd
+
+    def __call__(self, cmd=None) -> int:
 
         if not doot.args.on_fail((None,)).cmd.args.suppress_header():
             printer.info("----------------------------------------------", extra={"colour" : "green"})
             printer.info("-------------------- Doot --------------------", extra={"colour" : "yellow"})
             printer.info("----------------------------------------------", extra={"colour": "green"})
 
         if doot.args.on_fail(False).head.args.debug():
@@ -216,41 +235,54 @@
         # Do the cmd
         logging.info("Overlord Calling: %s", cmd or doot.args.on_fail("Unknown").cmd.name())
         try:
             cmd = self._get_cmd(cmd)
             cmd(self.tasks, self.plugins)
         except doot.errors.DootError as err:
             self._errored = err
-            raise err from err
-
-    def _get_cmd(self, cmd=None):
-        if self.current_cmd is not None:
-            return self.current_cmd
-
-        target = cmd or doot.args.on_fail(doot.constants.DEFAULT_CLI_CMD).cmd.name()
-
-        self.current_cmd = self.cmds.get(target, None)
-        if self.current_cmd is None:
-            self._errored = DootParseError("Specified Command Couldn't be Found: %s", target)
-            raise self._errored
-
-        return self.current_cmd
-
-
+            raise err
+        else:
+            return 0
 
     def shutdown(self):
         """ Doot has finished normally, so report on what was done """
         if self.current_cmd is not None and hasattr(self.current_cmd, "shutdown"):
             self.current_cmd.shutdown(self._errored, self.tasks, self.plugins)
 
         match self._errored:
             case doot.errors.DootError():
                 pass
             case None:
-                logging.info("Shutting Doot Down Normally, reporting defaulted tomlguard values")
-                defaulted_toml = tomlguard.TomlGuard.report_defaulted()
+                logging.info("Shutting Doot Down Normally")
+                self._record_defaulted_config_values()
+
+        self._announce_exit()
 
-                with open(defaulted_file, 'w') as f:
-                    f.write("# default values used:\n")
-                    f.write("\n".join(defaulted_toml) + "\n\n")
-                    # f.write("[.directories]\n")
-                    # f.write("\n".join(defaulted_locs))
+    def _announce_exit(self):
+        match sys.platform:
+            case "linux":
+                pass
+            case "darwin":
+                if doot.config is not None:
+                    announce_exit        = doot.config.on_fail(announce_exit, bool|str).settings.general.notify.say_on_exit()
+                    announce_voice       = doot.config.on_fail(announce_voice, str).setttings.general.notify.announce_voice()
+
+                match result, announce_exit:
+                    case 0, str() as say_text:
+                        cmd = sh.say("-v", announce_voice, "-r", "50", say_text)
+                    case 0, True:
+                        cmd = sh.say("-v", announce_voice, "-r", "50", "Doot Has Finished")
+                    case _, True|str():
+                        cmd = sh.say("-v", announce_voice, "-r", "50", "Doot Encountered a problem")
+                    case _, _:
+                        cmd = None
+                if cmd is not None:
+                    cmd.execute()
+
+    def _record_defaulted_config_values(self):
+
+        defaulted_toml = tomlguard.TomlGuard.report_defaulted()
+        with open(defaulted_file, 'w') as f:
+            f.write("# default values used:\n")
+            f.write("\n".join(defaulted_toml) + "\n\n")
+            # f.write("[.directories]\n")
+            # f.write("\n".join(defaulted_locs))
```

### Comparing `doot-0.6.1/doot/control/runner.py` & `doot-0.7.0/doot/control/runner.py`

 * *Files 20% similar despite different names*

```diff
@@ -25,48 +25,43 @@
 # from weakref import ref
 
 import networkx as nx
 ##-- end imports
 
 ##-- logging
 logging = logmod.getLogger(__name__)
-##-- end logging
-
 printer = logmod.getLogger("doot._printer")
+##-- end logging
 
 from collections import defaultdict
 from contextlib import nullcontext
 import doot
-import doot.constants
 import doot.errors
 from doot.enums import ReportEnum, ActionResponseEnum as ActRE
 from doot._abstract import Job_i, Task_i, FailPolicy_p
-from doot._abstract import TaskTracker_i, TaskRunner_i, TaskBase_i, ReportLine_i, Action_p, Reporter_i
-from doot.structs import DootTaskArtifact
-from doot.structs import DootTaskSpec, DootActionSpec
+from doot._abstract import TaskTracker_i, TaskRunner_i, Task_i, ReportLine_i, Action_p, Reporter_i
+from doot.structs import DootTaskArtifact, DootTaskSpec, DootActionSpec, DootTaskName
 from doot.control.base_runner import BaseRunner, logctx
 from doot.utils.signal_handler import SignalHandler
 
-dry_run                    = doot.args.on_fail(False).cmd.args.dry_run()
-head_level    : Final[str] = doot.constants.DEFAULT_HEAD_LEVEL
-build_level   : Final[str] = doot.constants.DEFAULT_BUILD_LEVEL
-action_level  : Final[str] = doot.constants.DEFAULT_ACTION_LEVEL
-sleep_level   : Final[str] = doot.constants.DEFAULT_SLEEP_LEVEL
-execute_level : Final[str] = doot.constants.DEFAULT_EXECUTE_LEVEL
-max_steps     : Final[str] = doot.config.on_fail(100_000).settings.general.max_steps()
+head_level    : Final[str] = doot.constants.printer.DEFAULT_HEAD_LEVEL
+build_level   : Final[str] = doot.constants.printer.DEFAULT_BUILD_LEVEL
+action_level  : Final[str] = doot.constants.printer.DEFAULT_ACTION_LEVEL
+sleep_level   : Final[str] = doot.constants.printer.DEFAULT_SLEEP_LEVEL
+execute_level : Final[str] = doot.constants.printer.DEFAULT_EXECUTE_LEVEL
+max_steps     : Final[str] = doot.config.on_fail(100_000).settings.tasks.max_steps()
 
 @doot.check_protocol
 class DootRunner(BaseRunner, TaskRunner_i):
     """ The simplest single threaded task runner """
 
     def __init__(self:Self, *, tracker:TaskTracker_i, reporter:Reporter_i, policy=None):
         super().__init__(tracker=tracker, reporter=reporter, policy=policy)
         self.teardown_list  = []                     # list of tasks to teardown
 
-
     def __call__(self, *tasks:str, handler=None):
         """ tasks are initial targets to run.
           so loop on the tracker, getting the next task,
           running its actions,
           and repeating,
           until done
 
@@ -84,128 +79,189 @@
 
         with handler:
             printer.setLevel("INFO")
             while bool(self.tracker) and self.step < max_steps:
                 self._run_next_task()
 
     def _run_next_task(self):
+        """
+          Get the next task from the tracker, expand/run it,
+          and handle the result/failure
+        """
         with logctx("INFO"):
+            task = None
             try:
                 match (task:= self.tracker.next_for()):
                     case None:
                         pass
                     case DootTaskArtifact():
                         self._notify_artifact(task)
-                    case Job_i():
+                    case Job_i() if self._test_conditions(task):
                         self._expand_job(task)
-                    case Task_i():
+                    case Task_i() if self._test_conditions(task):
                         self._execute_task(task)
-
-                self._handle_task_success(task)
-                self._sleep(task)
-
+                    case Task_i():
+                        # test_conditions failed, so skip
+                        printer.info("Skipping Task: %s", task.spec.name)
+                    case _:
+                        pass
             except doot.errors.DootError as err:
                 self._handle_failure(task, err)
-
+            except Exception as err:
+                printer.exception("Unknown, non-Doot failure occurred: %s", err)
+                self.tracker.clear_queue()
+                raise err
+            else:
+                self._handle_task_success(task)
+                self._sleep(task)
 
     def _expand_job(self, job:Job_i) -> None:
         """ turn a job into all of its tasks, including teardowns """
-        logmod.debug("-- Expanding Job %s: %s", self.step, job.name)
-        with logctx(job.spec.print_levels.on_fail(head_level).head()) as p:
-            p.info("---- Job %s: %s", self.step, job.name, extra={"colour":"magenta"})
-
-            if bool(job.spec.actions): # and job != mini...
-                p.warning("-- Job %s: Actions were found in job spec, but jobs don't run actions", job.name)
-
-        self.reporter.trace(job.spec, flags=ReportEnum.JOB | ReportEnum.INIT)
-
-        count = 0
-        with logctx(job.spec.print_levels.on_fail(build_level).build()) as p:
-            for task in job.build():
-                match task:
-                    case Job_i():
-                        p.warning("Jobs probably shouldn't build jobs: %s : %s", job.name, task.name)
-                        self.tracker.add_task(task, no_root_connection=True)
-                    case Task_i():
-                        self.tracker.add_task(task, no_root_connection=True)
-                    case DootTaskSpec():
-                        self.tracker.add_task(task, no_root_connection=True)
-                    case _:
-                        self.reporter.trace(job.spec, flags=ReportEnum.FAIL | ReportEnum.JOB)
-                        raise doot.errors.DootTaskError("Job %s Built a Bad Value: %s", job.name, task, task=job.spec)
+        build_log_level  = job.spec.print_levels.on_fail(build_level).build()
+        head_log_level   = job.spec.print_levels.on_fail(head_level).head()
 
-                count += 1
-
-        logmod.debug("-- Job %s Expansion produced: %s tasks", job.name, count)
-        self.reporter.trace(job.spec, flags=ReportEnum.JOB | ReportEnum.SUCCEED)
+        try:
+            logmod.debug("-- Expanding Job %s: %s", self.step, job.name)
+            with logctx(head_log_level) as p:     # Announce entry
+                p.info("---> Job %s: %s", self.step, job.name, extra={"colour":"magenta"})
+                # TODO queue $head$
+
+            self.reporter.add_trace(job.spec, flags=ReportEnum.JOB | ReportEnum.INIT)
+
+            with logctx(build_log_level) as p: # Run the actions
+                self._execute_action_group(job.spec.setup, job)
+                self._execute_action_group(job.spec.actions, job, allow_queue=True)
+
+        except doot.errors.DootError as err:
+            self._execute_action_group(task.spec.on_fail, task)
+            raise err
+        finally:
+            self._execute_action_group(job.spec.cleanup, job)
+            job.state.clear()
+
+            with logctx(head_log_level)  as p: # Announce Exit
+                self.reporter.add_trace(job.spec, flags=ReportEnum.JOB | ReportEnum.SUCCEED)
+                p.info("---< Job %s: %s", self.step, job.name, extra={"colour":"magenta"})
 
     def _execute_task(self, task:Task_i) -> None:
         """ execute a single task's actions """
-        with logctx(task.spec.print_levels.on_fail(head_level).head()) as p:
-            p.info("---- Task %s: %s", self.step, task.name, extra={"colour":"magenta"})
-
-        self.reporter.trace(task.spec, flags=ReportEnum.TASK | ReportEnum.INIT)
+        build_log_level  = task.spec.print_levels.on_fail(build_level).build()
+        head_log_level   = task.spec.print_levels.on_fail(head_level).head()
 
-        action_count = 0
-        action_result = ActRE.SUCCESS
-        with logctx(task.spec.print_levels.on_fail(build_level).build()) as p:
-            for action in task.actions:
-                match action:
-                    case DootActionSpec() if action.fun is None:
-                        self.reporter.trace(task.spec, flags=ReportEnum.FAIL | ReportEnum.TASK)
-                        raise doot.errors.DootTaskError("Task %s Failed: Produced an action with no callable: %s", task.name, action, task=task.spec)
-                    case DootActionSpec():
-                        action_result = self._execute_action(action_count, action, task)
-                    case _:
-                        self.reporter.trace(task.spec, flags=ReportEnum.FAIL | ReportEnum.TASK)
-                        raise doot.errors.DootTaskError("Task %s Failed: Produced a bad action: %s", task.name, action, task=task.spec)
-
-                action_count += 1
-                if action_result is ActRE.SKIP:
-                    p.info("------ Remaining Task Actions skipped by Action Instruction")
+        try:
+            with logctx(head_log_level) as p: # Announce entry
+                p.info("----> Task %s :  %s", self.step, task.spec.name.readable, extra={"colour":"magenta"})
+                # TODO queue $head$
+
+            self.reporter.add_trace(task.spec, flags=ReportEnum.TASK | ReportEnum.INIT)
+
+            with logctx(build_log_level) as p: # Build then run actions
+                self._execute_action_group(task.spec.setup, task)
+                self._execute_action_group(task.spec.actions, task)
+                self.reporter.add_trace(task.spec, flags=ReportEnum.TASK | ReportEnum.SUCCEED)
+        except doot.errors.DootError as err:
+            self._execute_action_group(task.spec.on_fail, task)
+            raise err
+        finally:
+            self._execute_action_group(task.spec.cleanup, task)
+            task.state.clear()
+
+            with logctx(head_log_level)  as p: # Cleanup and exit
+                p.debug("----< Task: %s", task.name, extra={"colour":"cyan"})
+
+    def _execute_action_group(self, actions:list, task:Task_i, allow_queue=False) -> tuple[int, ActRE]:
+        """ Execute a group of actions, possibly queue any task specs they produced,
+        and return a count of the actions run + the result
+        """
+        group_result    = ActRE.SUCCESS
+        to_queue        = []
+        executed        = 0
+
+        for action in actions:
+            result = None
+            match action:
+                case DootActionSpec():
+                    result = self._execute_action(executed, action, task)
+                case DootTaskArtifact():
+                    pass
+                case DootTaskName():
+                    pass
+                case _:
+                    self.reporter.add_trace(task.spec, flags=ReportEnum.FAIL | ReportEnum.TASK)
+                    raise doot.errors.DootTaskError("Task %s Failed: Produced a bad action: %s", task.name, action, task=task.spec)
+
+            match result:
+                case None:
+                    continue
+                case list():
+                    to_queue += result
+                case ActRE.SKIP:
+                    p.warning("------ Remaining Task Actions skipped by Action Instruction")
+                    group_result = ActRE.SKIP
                     break
 
-            self.reporter.trace(task.spec, flags=ReportEnum.TASK | ReportEnum.SUCCEED)
-            p.debug("------ Task %s: Actions Complete", task.name, extra={"colour":"cyan"})
-            p.debug("------ Task Executed %s Actions", action_count)
-
-    def _execute_action(self, count, action, task) -> ActRE:
-        """ Run the given action of a specific task  """
-        if dry_run:
-            logging.info("Dry Run: Not executing action: %s : %s", task.name, action, extra={"colour":"cyan"})
-            self.reporter.trace(task.spec, flags=ReportEnum.ACTION | ReportEnum.SKIP)
-            return ActRE.SUCCESS
-
-        result = None
-        with logctx(task.spec.print_levels.on_fail(action_level).action()) as p:
-            self.reporter.trace(action, flags=ReportEnum.ACTION | ReportEnum.INIT)
-            task.state['_action_step'] = count
-            p.info("------ Action %s.%s: %s", self.step, count, action.do, extra={"colour":"cyan"})
-            p.debug("------ Action %s.%s: args=%s kwargs=%s. state keys = %s", self.step, count, action.args, dict(action.kwargs), list(task.state.keys()))
+            executed += 1
+
+        else: # runs only if no 'break'
+            if not allow_queue:
+                    return executed, group_result
+
+            for spec in to_queue:
+                self.tracker.add_task(spec, no_root_connection=True)
+
+        return executed, group_result
+
+    def _execute_action(self, count, action, task) -> ActRE|list:
+        """ Run the given action of a specific task.
+
+        """
+        result                     = None
+        action_log_level           = task.spec.print_levels.on_fail(action_level).action()
+        execute_log_level          = task.spec.print_levels.on_fail(execute_level).execute()
+        task.state['_action_step'] = count
+        self.reporter.add_trace(action, flags=ReportEnum.ACTION | ReportEnum.INIT)
+        logmod.debug("-----> Action Execution: %s for %s", action, task.name)
+
+        with logctx(action_log_level) as p: # Prep the action
+            p.info( "-----> Action %s.%s: %s", self.step, count, action.do, extra={"colour":"cyan"})
+            p.debug("-----> Action %s.%s: args=%s kwargs=%s. state keys = %s", self.step, count, action.args, dict(action.kwargs), list(task.state.keys()))
             action.verify(task.state)
 
-            with logctx(task.spec.print_levels.on_fail(execute_level).execute()) as p2:
-                ## Actually call the action here:
+            with logctx(execute_log_level) as p2: # call the action
                 result = action(task.state)
                 ##
             p.debug("-- Action Result: %s", result)
 
-        match result:
-            case ActRE.SKIP:
-                pass
-            case None | True:
-                result = ActRE.SUCCESS
-            case dict():
-                task.state.update(result)
-                result = ActRE.SUCCESS
-            case False | ActRE.FAIL:
-                self.reporter.trace(action, flags=ReportEnum.FAIL | ReportEnum.ACTION)
-                raise doot.errors.DootTaskFailed("Task %s Action Failed: %s", task.name, action, task=task.spec)
-            case _:
-                self.reporter.trace(action, flags=ReportEnum.FAIL | ReportEnum.ACTION)
-                raise doot.errors.DootTaskError("Task %s Action %s Failed: Returned an unplanned for value: %s", task.name, action, result, task=task.spec)
+        with logctx(action_log_level) as p: # Handle the result
+            match result:
+                case ActRE.SKIP:
+                    # result will be returned, and expand_job/execute_task will handle it
+                    pass
+                case None | True:
+                    result = ActRE.SUCCESS
+                case dict(): # update the task's state
+                    task.state.update({str(k):v for k,v in result.items()})
+                    result = ActRE.SUCCESS
+                case list() if all(isinstance(x, (DootTaskName, DootTaskSpec)) for x in result):
+                    pass
+                case False | ActRE.FAIL:
+                    self.reporter.add_trace(action, flags=ReportEnum.FAIL | ReportEnum.ACTION)
+                    raise doot.errors.DootTaskFailed("Task %s: Action Failed: %s", task.name, action.do, task=task.spec)
+                case _:
+                    self.reporter.add_trace(action, flags=ReportEnum.FAIL | ReportEnum.ACTION)
+                    raise doot.errors.DootTaskError("Task %s: Action %s Failed: Returned an unplanned for value: %s", task.name, action.do, result, task=task.spec)
+
+            action.verify_out(task.state)
 
-        action.verify_out(task.state)
+        with logctx(action_log_level) as p: # Prep the action
+            p.debug("-----< Action Execution Complete: %s for %s", action, task.name)
 
-        logmod.debug("------ Action Execution Complete: %s for %s", action, task.name)
-        self.reporter.trace(action, flags=ReportEnum.ACTION | ReportEnum.SUCCEED)
+        self.reporter.add_trace(action, flags=ReportEnum.ACTION | ReportEnum.SUCCEED)
         return result
+
+    def _test_conditions(self, task:Task_i) -> bool:
+        """ run action specs that test if the task can be started """
+        match self._execute_action_group(task.spec.depends_on, task):
+            case _, ActRE.SKIP:
+                return False
+            case _, _:
+                return True
```

### Comparing `doot-0.6.1/doot/control/step_runner.py` & `doot-0.7.0/doot/control/step_runner.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 from doot.utils.signal_handler import SignalHandler
 
 dry_run      = doot.args.on_fail(False).cmd.args.dry_run()
 SLEEP_LENGTH = doot.config.on_fail(0.2, int|float).settings.tasks.sleep.task()
 
 @doot.check_protocol
 class DootStepRunner(DootRunner):
-    """ A runner with step control """
+    """ extends the default runner with step control """
     _conf_prompt  = "::- Command? (? for help): "
     _cmd_prefix   = "_do_"
     _aliases      = { ""  : "continue",
                      "c"  : "continue",
                      "n"  : "skip",
                      "b"  : "break",
                      "l"  : "list",
```

### Comparing `doot-0.6.1/doot/control/tracker.py` & `doot-0.7.0/doot/control/tracker.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,19 +29,18 @@
 logging = logmod.getLogger(__name__)
 ##-- end logging
 printer = logmod.getLogger("doot._printer")
 
 from collections import defaultdict
 import doot
 import doot.errors
-import doot.constants as const
 from doot.enums import TaskStateEnum
 from doot._abstract import Job_i, Task_i, FailPolicy_p
 from doot.structs import DootTaskArtifact, DootTaskSpec, DootTaskName, DootCodeReference
-from doot._abstract import TaskTracker_i, TaskRunner_i, TaskBase_i
+from doot._abstract import TaskTracker_i, TaskRunner_i, Task_i
 from doot.task.base_task import DootTask
 from doot.control.base_tracker import BaseTracker, ROOT, STATE, PRIORITY, EDGE_E, MIN_PRIORITY
 
 REACTIVE_ADD     : Final[str]                  = "reactive-add"
 
 @doot.check_protocol
 class DootTracker(BaseTracker, TaskTracker_i):
@@ -56,47 +55,47 @@
     """
     state_e            = TaskStateEnum
     INITIAL_TASK_STATE = TaskStateEnum.DEFINED
 
     def __init__(self, shadowing:bool=False, *, policy=None):
         super().__init__(shadowing=shadowing, policy=policy) # self.tasks
 
-    def add_task(self, task:DootTaskSpec|TaskBase_i, *, no_root_connection=False) -> None:
+    def add_task(self, task:DootTaskSpec|Task_i, *, no_root_connection=False) -> None:
         """ add a task description into the tracker, but don't queue it
         connecting it with its dependencies and tasks that depend on it
-
-        # TODO check the spec's "active_when" conditions, return early if it fails
         """
-        task : TaskBase_i = self._prep_task(task)
-        assert(isinstance(task, TaskBase_i))
+        task : Task_i = self._prep_task(task)
+        assert(isinstance(task, Task_i))
 
         # Store it
         self.tasks[task.name] = task
 
         # Insert into dependency graph
         self.task_graph.add_node(task.name, state=self.INITIAL_TASK_STATE, priority=task.spec.priority)
 
         # Then connect it to the rest of the graph
         if not no_root_connection and task.name:
             self.task_graph.add_edge(task.name, ROOT)
 
         self._insert_dependencies(task)
         self._insert_dependents(task)
-        self._insert_according_to_queue_behaviour(task)
+        self._maybe_implicit_queue(task)
 
-    def update_state(self, task:str|TaskBase_i|DootTaskArtifact, state:self.state_e):
+    def update_state(self, task:str|Task_i|DootTaskArtifact, state:self.state_e):
         """ update the state of a task in the dependency graph """
         logging.debug("Updating State: %s -> %s", task, state)
         match task, state:
             case str(), self.state_e() if task in self.task_graph:
                 self.task_graph.nodes[task][STATE] = state
-            case TaskBase_i(), self.state_e() if task.name in self.task_graph:
-                self.task_graph.nodes[task.name][STATE] = state
-            case DootTaskArtifact(), self.state_e() if task in self.task_graph:
+            case DootTaskName(), self.state_e() if task in self.task_graph:
                 self.task_graph.nodes[task][STATE] = state
+            case Task_i(), self.state_e() if task.name in self.task_graph:
+                self.task_graph.nodes[task.name][STATE] = state
+            case DootTaskArtifact(), self.state_e() if str(task) in self.task_graph:
+                self.task_graph.nodes[str(task)][STATE] = state
             case _, _:
                 raise doot.errors.DootTaskTrackingError("Bad task update state args", task, state)
 
     def next_for(self, target:None|str=None) -> None|Job_i|Task_i|DootTaskArtifact:
         """ ask for the next task that can be performed """
         if target and target not in self.active_set:
             self.queue_task(target, silent=True)
```

### Comparing `doot-0.6.1/doot/enums.py` & `doot-0.7.0/doot/enums.py`

 * *Files 18% similar despite different names*

```diff
@@ -17,48 +17,54 @@
 
 ##-- end builtin imports
 
 ##-- logging
 logging = logmod.getLogger(__name__)
 ##-- end logging
 
+from doot.mixins.enums import EnumBuilder_m, FlagsBuilder_m
+
 class TaskStateEnum(enum.Enum):
     """
       Enumeration of the different states a task can be in.
       The state is stored in a TaskTracker_i, not the task itself
     """
     TEARDOWN        = enum.auto()
     SUCCESS         = enum.auto()
     FAILED          = enum.auto()
     HALTED          = enum.auto()
     WAIT            = enum.auto()
     READY           = enum.auto()
     RUNNING         = enum.auto()
     EXISTS          = enum.auto()
     INIT            = enum.auto()
+
     DEFINED         = enum.auto()
     DECLARED        = enum.auto()
     ARTIFACT        = enum.auto()
 
-class TaskFlags(enum.Flag):
+class TaskFlags(FlagsBuilder_m, enum.Flag):
     """
       Flags describing properties of a task,
       stored in the Task_i instance itself.
     """
+
+    default      = enum.auto()
     TASK         = enum.auto()
     JOB          = enum.auto()
     EPHEMERAL    = enum.auto()
     IDEMPOTENT   = enum.auto()
     REQ_TEARDOWN = enum.auto()
     REQ_SETUP    = enum.auto()
     IS_TEARDOWN  = enum.auto()
     IS_SETUP     = enum.auto()
     THREAD_SAFE  = enum.auto()
     STATEFUL     = enum.auto()
     STATELESS    = enum.auto()
+    INTERNAL     = enum.auto()
 
 class ReportEnum(enum.Flag):
     """ Flags to mark what a reporter reports """
     INIT     = enum.auto()
     SUCCEED  = enum.auto()
     FAIL     = enum.auto()
     EXECUTE  = enum.auto()
@@ -72,41 +78,52 @@
     PLUGIN   = enum.auto()
     TASK     = enum.auto()
     JOB      = enum.auto()
     ACTION   = enum.auto()
     CONFIG   = enum.auto()
     ARTIFACT = enum.auto()
 
+class ActionResponseEnum(EnumBuilder_m, enum.Enum):
 
-class TaskPolicyEnum(enum.Flag):
+    SUCCEED  = enum.auto()
+    FAIL     = enum.auto()
+    SKIP     = enum.auto()
+    SUCCESS  = SUCCEED
+
+class LoopControl(enum.Enum):
     """
-      Combinable Policy Types:
-      breaker  : fails fast
-      bulkhead : limits extent of problem and continues
-      retry    : trys to do the action again to see if its resolved
-      timeout  : waits then fails
-      cache    : reuses old results
-      fallback : uses defined alternatives
-      cleanup  : uses defined cleanup actions
-      debug    : triggers pdb
-      pretend  : pretend everything went fine
-      accept   : accept the failure
-
-      breaker will overrule bulkhead
-    """
-    BREAKER  = enum.auto()
-    BULKHEAD = enum.auto()
-    RETRY    = enum.auto()
-    TIMEOUT  = enum.auto()
-    CACHE    = enum.auto()
-    FALLBACK = enum.auto()
-    CLEANUP  = enum.auto()
-    DEBUG    = enum.auto()
-    PRETEND  = enum.auto()
-    ACCEPT   = enum.auto()
+      A Simple enum to descrbe results for testing in a maybe recursive loop
+      (like walking a a tree)
 
+    accept  : is a result, and descend if recursive
+    keep    : is a result, don't descend
+    discard : not a result, descend
+    reject  : not a result, don't descend
+    """
+    yesAnd  = enum.auto()
+    yes     = enum.auto()
+    noBut   = enum.auto()
+    no      = enum.auto()
 
-class ActionResponseEnum(enum.Enum):
-    # TODO make success -> succeed
-    SUCCESS  = enum.auto()
-    FAIL     = enum.auto()
-    SKIP     = enum.auto()
+class LocationMeta(FlagsBuilder_m, enum.Flag):
+    """ Available metadata attachable to a location """
+
+    default      = enum.auto()
+    file         = enum.auto()
+    protected    = enum.auto()
+    indefinite   = enum.auto()
+    cleanable    = enum.auto()
+    normOnLoad   = enum.auto()
+
+class TaskQueueMeta(EnumBuilder_m, enum.Enum):
+    """ available ways a task can be activated for running
+      onRegister/auto     : activates automatically when added to the task network
+      reactive            : activates if an adjacent node completes
+
+      default             : activates only if uses queues the task, or its a dependency
+
+    """
+
+    default    = enum.auto()
+    onRegister = enum.auto()
+    reactive   = enum.auto()
+    auto       = onRegister
```

### Comparing `doot-0.6.1/doot/errors.py` & `doot-0.7.0/doot/errors.py`

 * *Files identical despite different names*

### Comparing `doot-0.6.1/doot/loaders/__tests/test_cmd_loader.py` & `doot-0.7.0/doot/loaders/__tests/test_cmd_loader.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,18 +11,20 @@
 import pathlib as pl
 from typing import (Any, Callable, ClassVar, Generic, Iterable, Iterator,
                     Mapping, Match, MutableMapping, Sequence, Tuple, TypeAlias,
                     TypeVar, cast)
 from unittest import mock
 ##-- end imports
 
+from importlib.metadata import EntryPoint
 import pytest
 import tomlguard
 import doot
-from importlib.metadata import EntryPoint
+doot._test_setup()
+
 doot.config = tomlguard.TomlGuard({})
 from doot.loaders import cmd_loader
 logging = logmod.root
 
 class TestCmdLoader(unittest.TestCase):
 
     def test_initial(self):
```

### Comparing `doot-0.6.1/doot/loaders/__tests/test_plugin_loader.py` & `doot-0.7.0/doot/loaders/__tests/test_plugin_loader.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,14 +14,15 @@
                     TypeVar, cast)
 from unittest import mock
 ##-- end imports
 
 import pytest
 import tomlguard
 import doot
+doot._test_setup()
 doot.config = tomlguard.TomlGuard({})
 from doot.loaders import plugin_loader
 logging = logmod.root
 
 class TestPluginLoader:
 
     def test_initial(self):
@@ -29,9 +30,9 @@
         assert(basic is not None)
 
     def test_loads_defaults(self):
         basic = plugin_loader.DootPluginLoader()
         basic.setup()
         loaded = basic.load()
 
-        for key in (doot.constants.FRONTEND_PLUGIN_TYPES + doot.constants.BACKEND_PLUGIN_TYPES):
+        for key in (doot.constants.entrypoints.FRONTEND_PLUGIN_TYPES + doot.constants.entrypoints.BACKEND_PLUGIN_TYPES):
             assert(key in loaded), f"{key} missing"
```

### Comparing `doot-0.6.1/doot/loaders/__tests/test_task_loader.py` & `doot-0.7.0/doot/loaders/__tests/test_task_loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,16 +14,18 @@
                     TypeVar, cast)
 ##-- end imports
 
 import pytest
 import importlib.metadata
 import tomlguard
 import doot
+doot._test_setup()
+
 from doot.structs import DootTaskSpec
-from doot._abstract.task import TaskBase_i
+from doot._abstract.task import Task_i
 from doot.utils.mock_gen import mock_entry_point, mock_task_ctor
 
 doot.config = tomlguard.TomlGuard({})
 from doot.loaders import task_loader
 logging = logmod.root
 
 class TestTaskLoader:
```

### Comparing `doot-0.6.1/doot/loaders/cmd_loader.py` & `doot-0.7.0/doot/loaders/cmd_loader.py`

 * *Files identical despite different names*

### Comparing `doot-0.6.1/doot/loaders/plugin_loader.py` & `doot-0.7.0/doot/loaders/plugin_loader.py`

 * *Files 9% similar despite different names*

```diff
@@ -32,28 +32,28 @@
 # logging.setLevel(logmod.NOTSET)
 ##-- end logging
 
 from collections import defaultdict
 from importlib.metadata import entry_points, EntryPoint
 import tomlguard
 import doot
-import doot.constants
 from doot._abstract import PluginLoader_p
 
 skip_default_plugins        = doot.config.on_fail(False).skip_default_plugins()
 skip_plugin_search          = doot.config.on_fail(False).skip_plugin_search()
 env_plugins                 = doot.config.on_fail({}).plugins(wrapper=dict)
-plugin_types                = set(doot.constants.FRONTEND_PLUGIN_TYPES + doot.constants.BACKEND_PLUGIN_TYPES)
-cmd_loader_key  : Final     = doot.constants.DEFAULT_COMMAND_LOADER_KEY
-task_loader_key : Final     = doot.constants.DEFAULT_TASK_LOADER_KEY
+plugin_types                = set(doot.constants.entrypoints.FRONTEND_PLUGIN_TYPES + doot.constants.entrypoints.BACKEND_PLUGIN_TYPES)
+cmd_loader_key  : Final     = doot.constants.entrypoints.DEFAULT_COMMAND_LOADER_KEY
+task_loader_key : Final     = doot.constants.entrypoints.DEFAULT_TASK_LOADER_KEY
 
-def make_ep (x, y, z):
+def build_entry_point (x, y, z):
+    """ Make an EntryPoint """
     if z not in plugin_types:
         raise doot.errors.DootPluginError("Plugin Type Not Found: %s : %s", z, (x, y))
-    return EntryPoint(name=x, value=y, group="{}.{}".format(doot.constants.PLUGIN_TOML_PREFIX, z))
+    return EntryPoint(name=x, value=y, group="{}.{}".format(doot.constants.entrypoints.PLUGIN_TOML_PREFIX, z))
 
 
 @doot.check_protocol
 class DootPluginLoader(PluginLoader_p):
     """
     Load doot plugins from the system, to choose from with doot.toml or cli args
     """
@@ -71,15 +71,15 @@
         return self
 
     def load(self) -> TomlGuard[EntryPoint]:
         """
         use entry_points(group="doot")
         add to the config tomlguard
         """
-        logging.debug("---- Loading Plugins: %s", doot.constants.PLUGIN_TOML_PREFIX)
+        logging.debug("---- Loading Plugins: %s", doot.constants.entrypoints.PLUGIN_TOML_PREFIX)
         try:
             self._load_system_plugins()
         except Exception as err:
             raise doot.errors.DootPluginError("Failed to load system wide plugins: %s", err) from err
 
         try:
             self._load_from_toml()
@@ -103,15 +103,15 @@
     def _load_system_plugins(self):
         if skip_plugin_search:
             pass
         else:
             logging.info("Searching environment for plugins, skip with `skip_plugin_search` in config")
             for plugin_type in plugin_types:
                 try:
-                    plugin_group = "{}.{}".format(doot.constants.PLUGIN_TOML_PREFIX, plugin_type)
+                    plugin_group = "{}.{}".format(doot.constants.entrypoints.PLUGIN_TOML_PREFIX, plugin_type)
                     # Load env wide entry points
                     for entry_point in entry_points(group=plugin_group):
                         self.plugins[plugin_type].append(entry_point)
                 except Exception as err:
                     raise doot.errors.DootPluginError("Plugin Failed to Load: %s : %s : %s", plugin_group, entry_point, err) from err
 
     def _load_from_toml(self):
@@ -131,21 +131,22 @@
     def _load_extra_plugins(self):
         extra_eps    = self.extra_config.on_fail({}).plugins(wrapper=dict)
         # load extra-config entry points
         for k,v in extra_eps.items():
             if k not in plugin_types:
                 logging.warning("Unknown plugin type found in extra config: %s", k)
                 continue
-            ep = EntryPoint(name=k, value=v, group=doot.constants.PLUGIN_TOML_PREFIX)
+            ep = EntryPoint(name=k, value=v, group=doot.constants.entrypoints.PLUGIN_TOML_PREFIX)
             logging.debug("Adding Plugin: %s", ep)
             self.plugins[k].append(ep)
 
     def _append_defaults(self):
         if skip_default_plugins:
             logging.info("Skipping Default Plugins")
             return
 
-        self.plugins[cmd_loader_key].append(make_ep(cmd_loader_key, "doot.loaders.cmd_loader:DootCommandLoader", cmd_loader_key))
-        self.plugins[task_loader_key].append(make_ep(task_loader_key, "doot.loaders.task_loader:DootTaskLoader", task_loader_key))
+        self.plugins[cmd_loader_key].append(build_entry_point(cmd_loader_key, "doot.loaders.cmd_loader:DootCommandLoader", cmd_loader_key))
+        self.plugins[task_loader_key].append(build_entry_point(task_loader_key, "doot.loaders.task_loader:DootTaskLoader", task_loader_key))
 
-        for group, vals in doot.constants.DEFAULT_PLUGINS.items():
-            self.plugins[group]  += [make_ep(x, y, group) for x,y in vals]
+        for group, vals in doot.aliases:
+            logging.debug("Loading aliases: %s", group)
+            self.plugins[group]  += [build_entry_point(x, y, group) for x,y in vals.items()]
```

### Comparing `doot-0.6.1/doot/loaders/task_loader.py` & `doot-0.7.0/doot/loaders/task_loader.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,17 +36,18 @@
 
 from collections import ChainMap
 import importlib
 import tomlguard
 import doot
 import doot.errors
 from doot.structs import DootTaskSpec, DootTaskName, DootCodeReference
-from doot.constants import DEFAULT_TASK_GROUP, IMPORT_SEP
-from doot._abstract import TaskLoader_p, Job_i, Task_i, TaskBase_i
+from doot._abstract import TaskLoader_p, Job_i, Task_i
 
+DEFAULT_TASK_GROUP        = doot.constants.names.DEFAULT_TASK_GROUP
+IMPORT_SEP                = doot.constants.patterns.IMPORT_SEP
 TASK_STRING : Final[str]  = "task_"
 prefix_len  : Final[int]  = len(TASK_STRING)
 
 task_sources              = doot.config.on_fail([doot.locs[".tasks"]], list).settings.tasks.sources(wrapper=lambda x: [doot.locs[y] for y in x])
 allow_overloads           = doot.config.on_fail(False, bool).allow_overloads()
 
 def apply_group_and_source(group, source, x):
@@ -128,18 +129,14 @@
             raw_specs += self._load_specs_from_path(path)
 
         logging.debug("Loaded %s Task Specs", len(raw_specs))
         if bool(self.tasks):
             logging.warning("Task Loader is overwriting already loaded tasks")
         self.tasks = self._build_task_specs(raw_specs, self.cmd_names)
 
-        # Reapply config location declarations as overrides:
-        for loc in doot.config.on_fail([]).locations():
-            doot.locs.update(loc, strict=False)
-
         logging.debug("Task List Size: %s", len(self.tasks))
         logging.debug("Task List Names: %s", list(self.tasks.keys()))
         logging.debug("---- Tasks Loaded in %s seconds", f"{time.perf_counter() - start_time:0.4f}")
         return tomlguard.TomlGuard(self.tasks)
 
     def _load_raw_specs(self, data:dict, source:pl.Path|Literal['(extra)']) -> list[dict]:
         """ extract raw task descriptions from a toplevel tasks dict, with not format checking
@@ -169,30 +166,28 @@
                 except OSError as err:
                     logging.error("Failed to Load Task File: %s : %s", task_file, err.filename)
                     continue
                 for group, val in data.on_fail({}).tasks().items():
                     # sets 'group' for each task if it hasn't been set already
                     raw_specs += map(ftz.partial(apply_group_and_source, group, task_file), val)
                 logging.info("Loaded Tasks from: %s", task_file)
-                if 'locations' in data:
-                    self._load_location_updates(data.locations, task_file)
+                self._load_location_updates(data.on_fail([]).locations(), task_file)
 
         elif path.is_file():
             try:
                 data = tomlguard.load(path)
             except OSError as err:
                 logging.error("Failed to Load Task File: %s : %s", path, err.filename)
                 return raw_specs
 
             for group, val in data.on_fail({}).tasks().items():
                 # sets 'group' for each task if it hasn't been set already
                 raw_specs += map(ftz.partial(apply_group_and_source, group, path), val)
             logging.info("Loaded Tasks from: %s", path)
-            if 'locations' in data:
-                self._load_location_updates(data.locations, path)
+            self._load_location_updates(data.on_fail([]).locations(), path)
 
         return raw_specs
 
 
     def _build_task_specs(self, group_specs:list[dict], command_names) -> list[DootTaskSpec]:
         """
         convert raw dicts into DootTaskSpec objects,
@@ -211,34 +206,33 @@
                     case {"name": task_name, "group": group} if dont_allow_overloads(task_name, group): # complain on overload
                         raise doot.errors.DootTaskLoadError("Task Name Overloaded: %s : %s", task_name, group)
                     case {"name": task_name, "ctor": str() as task_alias} if task_alias in self.task_builders: # build named plugin type
                         logging.info("Building Task from short name: %s : %s", task_name, task_alias)
                         task_iden                   : DootCodeReference       = DootCodeReference.from_alias(task_alias, "task", self.plugins)
                         task_iden_with_mixins       : DootCodeReference       = task_iden.add_mixins(*spec.get("mixins", []), plugins=self.plugins)
                         spec['ctor'] = task_iden_with_mixins
-                        task_spec = DootTaskSpec.from_dict(spec)
+                        task_spec = DootTaskSpec.build(spec)
                         if str(task_spec.name) in task_descriptions:
                             logging.warning("Overloading Task: %s : %s", str(task_spec.name), task_alias)
 
-                        task_spec.check(ensure=TaskBase_i)
+                        task_spec.check(ensure=Task_i)
                         task_descriptions[str(task_spec.name)] = task_spec
                     case {"name": task_name}:
                         logging.info("Building Task: %s", task_name)
-                        task_spec = DootTaskSpec.from_dict(spec)
+                        task_spec = DootTaskSpec.build(spec)
                         if str(task_spec.name) in task_descriptions:
                             logging.warning("Overloading Task: %s : %s", str(task_spec.name), str(task_spec.ctor))
 
-                        task_spec.check(ensure=TaskBase_i)
+                        task_spec.check(ensure=Task_i)
                         task_descriptions[str(task_spec.name)] = task_spec
 
                     case _: # Else complain
                         raise doot.errors.DootTaskLoadError("Task Spec missing, at least, a name and ctor: %s: %s", spec['source'], spec)
             except doot.errors.DootLocationError as err:
-                logging.debug(err)
-                raise doot.errors.DootTaskLoadError("Task Spec '%s' Load Failure: Missing Location: '%s'. Source File: %s", task_name, str(err), spec['source']) from err
+                logging.warning("Task Spec '%s' Load Failure: Missing Location: '%s'. Source File: %s", task_name, str(err), spec['source'])
             except ModuleNotFoundError as err:
                 logging.debug(err)
                 raise doot.errors.DootTaskLoadError("Task Spec '%s' Load Failure: Bad Module Name: '%s'. Source File: %s", task_name, task_alias, spec['source']) from err
             except AttributeError as err:
                 logging.debug(err)
                 raise doot.errors.DootTaskLoadError("Task Spec '%s' Load Failure: Bad Class Name: '%s'. Source File: %s", task_name, task_alias, spec['source'], err.args) from err
             except ValueError as err:
```

### Comparing `doot-0.6.1/doot/mixins/action/batch.py` & `doot-0.7.0/doot/actions/json.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,118 +1,137 @@
 #!/usr/bin/env python3
 """
 
+
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
-printer = logmod.getLogger("doot._printer")
 ##-- end logging
+
+printer = logmod.getLogger("doot._printer")
+
+import math
+import json
 from time import sleep
+import sh
+import shutil
+import jsonlines
+import tomlguard as TG
 import doot
+from doot.errors import DootTaskError, DootTaskFailed
+from doot.enums import ActionResponseEnum
+from doot._abstract import Action_p
+from doot.structs import DootKey
 
-batch_size       = doot.config.on_fail(10, int).settings.tasks.batch.size()
-batches_max      = doot.config.on_fail(-1,    int).settings.tasks.batch.max()
-sleep_batch      = doot.config.on_fail(2.0,   int|float).settings.tasks.sleep.batch()
-sleep_notify     = doot.config.on_fail(False, bool).settings.general.notify.sleep()
 
-class Batch_M:
-    """
-    A Mixin to enable running batches of *subtasks* with
-    some sleep time
+##-- expansion keys
+FROM_KEY           : Final[DootKey] = DootKey.build("from")
+UPDATE             : Final[DootKey] = DootKey.build("update_")
+##-- end expansion keys
 
-    'run_batches' controls batching bookkeeping,
-    'batch' is the actual action
+class ReadJson(Action_p):
     """
+        Read a .json file and add it to the task state as a tomlguard
+    """
+    _toml_kwargs = [FROM_KEY, UPDATE]
 
-    batch_count       = 0
-
-    def run_batches(self, *batches, reset=True, fn=None, **kwargs):
-        """
-        handles batch bookkeeping
-
-        defaults to self.batch, but can pass in a function
-        """
-        if reset:
-            self._reset_batch_count()
-        fn = fn or self.batch
+    @DootKey.dec.paths("from")
+    @DootKey.dec.redirects("update_")
+    def __call__(self, spec, state, _from, _update):
+        if _from.suffix != ".json":
+            printer.warning("Read Json expected a .json file, got: %s", _from)
+
+        with open(_from) as fp:
+            data     = json.load(fp)
+        return { _update : TG.TomlGuard(data) }
+
+class ParseJson(Action_p):
+    """ parse a string as json """
+
+    @DootKey.dec.types("from")
+    @DootKey.dec.redirects("update_")
+    def __call__(self, spec, state, _from, _update):
+        return { _update : json.loads(_from) }
+
+class ReadJsonLines(Action_p):
+    """ read a .jsonl file, or some of it, and add it to the task state  """
+
+    @DootKey.dec.paths("from")
+    @DootKey.dec.types("offset", hint={"default":0})
+    @DootKey.dec.types("count", hint={"default":math.inf})
+    @DootKey.dec.redirects("update_")
+    def __call__(self, spec, state, _from, offset, count, _update):
+        if _from.suffix != ".jsonl":
+            printer.warning("Read JsonNL expects a .jsonl file, got: %s", _from)
 
         result = []
-        for data in batches:
-            match data:
-                case [*items]:
-                    batch_data = [x for x in items if x is not None]
-                    if not bool(batch_data):
-                        continue
-                    self.log(f"Batch: {self.batch_count} : ({len(batch_data)})")
-                case _:
-                    batch_data = data
-
-            batch_result =  fn(batch_data, **kwargs)
-            match batch_result:
-                case None:
-                    pass
-                case list():
-                    result += batch_result
-                case set():
-                    result += list(batch_result)
-                case _:
-                    result.append(batch_result)
-
-            self.batch_count += 1
-            if -1 < batches_max < self.batch_count:
-                self.log("Max Batch Hit")
-                return
-            if sleep_notify:
-                self.log("Sleep Batch")
-            sleep(sleep_batch)
-
-        return result
-
-    def batch(self, data, **kwargs):
-        """ Override to implement what a batch does """
-        raise NotImplementedError()
-
-    def chunk(self, iterable, n:int=None, *, incomplete='fill', fillvalue=None):
-        """Collect data into non-overlapping fixed-length chunks or blocks
-        from https://docs.python.org/3/library/itertools.html
-         grouper('ABCDEFG', 3, fillvalue='x') --> ABC DEF Gxx
-         grouper('ABCDEFG', 3, incomplete='strict') --> ABC DEF ValueError
-         grouper('ABCDEFG', 3, incomplete='ignore') --> ABC DEF
-        """
-        # TODO replace with more-itertools
-        n    = n or batch_size
-        args = [iter(iterable)] * n
-        if incomplete == 'fill':
-            return itz.zip_longest(*args, fillvalue=fillvalue)
-        if incomplete == 'strict':
-            return zip(*args, strict=True)
-        if incomplete == 'ignore':
-            return zip(*args)
-        else:
-            raise ValueError('Expected fill, strict, or ignore')
+        target_end = offset + count
+        with jsonlines.open(_from) as reader:
+            for i, obj in enumerate(reader):
+                if i < offset:
+                    continue
+                result.append(obj)
+                if target_end <= i:
+                    break
+
+        return { _update : result }
+
+
+class WriteJsonLines(Action_p):
+    """ Write a list of dicts as a .jsonl file
+      optionally gzip the file
+    """
 
-    def _reset_batch_count(self):
-        self.batch_count = 0
+    @DootKey.dec.types("from")
+    @DootKey.dec.paths("to")
+    def __call__(self, spec, state, _from, _to):
+        if _to.suffix != ".jsonl":
+            printer.warning("Write Json Lines expected a .jsonl file, got: %s", _to)
+
+        with jsonlines.open(_to, mode='a') as writer:
+            writer.write(_from)
+
+
+class WriteJson(Action_p):
+    """ Write a dict as a .json file  """
+
+    @DootKey.dec.types("from")
+    @DootKey.dec.paths("to")
+    def __call__(self, spec, state, _from, _to):
+        if _to.suffix != ".json":
+            printer.warning("Write Json Expected a .json file, got: %s", _to)
+        with open(_to, mode='w') as writer:
+            json.dump(_from,
+                      writer,
+                      ensure_ascii=True,
+                      indent=4,
+                      sort_keys=True)
```

### Comparing `doot-0.6.1/doot/mixins/action/cleaning.py` & `doot-0.7.0/doot/mixins/enums.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,69 +1,77 @@
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
+import datetime
+import enum
+import functools as ftz
+import itertools as itz
 import logging as logmod
 import pathlib as pl
-from copy import deepcopy
-from dataclasses import InitVar, dataclass, field
-from re import Pattern
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
 from uuid import UUID, uuid1
-from weakref import ref
 
-import pathlib as pl
-import shutil
+##-- end builtin imports
 
-##-- end imports
+##-- lib imports
+# import more_itertools as mitz
+# from boltons import
+##-- end lib imports
 
 ##-- logging
 logging = logmod.getLogger(__name__)
 ##-- end logging
 
-py_cache_globs = ["**/*.pyc", "**/*.pyo", "**/.mypy_cache", "**/__pycache__", "**/flycheck_*.py"]
-lisp_globs     = ["**/*.elc"]
-mac_os_globs   = ["**/.DS_Store", "**/*~"]
-java_globs     = ["**/*.class"]
-log_globs      = ["**/log.*", "**/*.log"]
-
-class Cleaner_M:
-
-    @staticmethod
-    def clean_target_dirs(task, dryrun):
-        """ Clean targets, including non-empty directories
-        Add to a tasks 'clean' dict value
-        """
-        if dryrun:
-            logging.info("%s - dryrun removing '%s'" % (task.name, task.targets))
-            return
+class EnumBuilder_m:
 
-        force_tree = task.meta is not None and "force_clean" in task.meta
+    @classmethod
+    def build(cls, val:str) -> Self:
+        try:
+            match val:
+                case str():
+                    return cls[val]
+                case cls():
+                    return val
+        except KeyError:
+            logging.warning("Can't Create a flag of (%s):%s. Available: %s", cls, val, list(cls.__members__.keys()))
+
+class FlagsBuilder_m:
+
+    @classmethod
+    def build(cls, vals:str|list|dict) -> Self:
+        match vals:
+            case str():
+                vals = [vals]
+            case list():
+                pass
+            case dict():
+                vals = [x for x,y in vals.items() if bool(y)]
 
-        for target_s in sorted(task.targets, reverse=True):
+        base = cls.default
+        for x in vals:
             try:
-                target = pl.Path(target_s)
-                if not target.exists():
-                    logging.debug("%s - N/A '%s'" % (task.name, target))
-                    continue
-
-                if target.is_file():
-                    logging.debug("%s - removing '%s'" % (task.name, target))
-                    target.remove()
-                elif target.is_dir() and not bool([x for x in target.iterdir() if x.name != ".DS_Store"]):
-                    logging.debug("%s - removing tree '%s'" % (task.name, target))
-                    shutil.rmtree(str(target))
-                elif target.is_dir() and force_tree:
-                    logging.debug("%s - force removing tree '%s'" % (task.name, target))
-                    shutil.rmtree(str(target))
-                else:
-                    contains = " ".join(map(str, target.iterdir()))
-                    logging.debug("%s - not empty: %s : %s" % (task.name, target, contains))
-            except OSError as err:
-                logging.warning(err)
+                match x:
+                    case str():
+                        base |= cls[x]
+                    case cls():
+                        base |= x
+            except KeyError:
+                logging.warning("Can't create a flag of (%s):%s. Available: %s", cls, x, list(cls.__members__.keys()))
+
+        return base
```

### Comparing `doot-0.6.1/doot/mixins/action/human_numbers.py` & `doot-0.7.0/doot/mixins/human_numbers.py`

 * *Files identical despite different names*

### Comparing `doot-0.6.1/doot/mixins/action/zipper.py` & `doot-0.7.0/doot/mixins/zipper.py`

 * *Files 18% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 zip_default_name = doot.config.on_fail("default", str).zip.name()
 zip_overwrite    = doot.config.on_fail(False, bool).zip.overwrite()
 zip_compression  = getattr(zipfile, doot.config.on_fail("ZIP_DEFLATED", str).zip.compression())
 zip_level        = doot.config.on_fail(4, int).zip.level()
 
 zip_choices = [("none", "No compression"), ("zip", "Default Zip Compression"), ("bzip2", "bzip2 Compression"), ("lzma", "lzma compression")]
 
-class Zipper_M:
+class Zipper_m:
     """
     Add methods for manipulating zip files.
     Can set a self.zip_root path, where added files with be relative to
     """
     zip_name                    = zip_default_name
     zip_overwrite               = zip_overwrite
     zip_root                    = None
@@ -60,35 +60,38 @@
             case { "compression": "bzip2", "level": x }:
                 return zipfile.ZIP_BZIP2, x
             case { "compression" : "lzma", "level": x}:
                 return zipfile.ZIP_LZMA, x
             case _:
                 return self._zip_default_compression, self._zip_default_compress_level
 
-    def zip_set_root(self, fpath):
+    def zip_set_root(self, fpath:pl.Path):
+        """ set the filesystem that acts as the root for paths to be added to the zip file """
         self.zip_root = fpath
 
-    def zip_create(self, fpath):
+    def zip_create(self, fpath:pl.Path):
+        """ Create a new zipfile. will overwrite an existing zip if 'zip_overwrite' is set """
         assert(fpath.suffix== ".zip")
         if self.zip_overwrite and fpath.exists():
             fpath.unlink()
         elif fpath.exists():
             return
 
         logging.info("Creating Zip File: %s", fpath)
         now = datetime.datetime.strftime(datetime.datetime.now(), "%Y:%m:%d::%H:%M:%S")
         record_str = f"Zip File created at {now} for doot task: {self.basename}"
         compress_type, compress_level = self._zip_get_compression_settings()
 
         with zipfile.ZipFile(fpath, mode='w', compression=compress_type, compresslevel=compress_level, allowZip64=True ) as targ:
             targ.writestr(".taskrecord", record_str)
 
-    def zip_add_paths(self, fpath, *args):
+    def zip_add_paths(self, fpath:pl.Path, *args:pl.Path):
         """
-        Add specific files to the zip
+        Add specific files to the zip.
+          Will Create the zip if it doesn't exist
         """
         logging.info("Adding to Zipfile: %s : %s", fpath, args)
         assert(fpath.suffix == ".zip")
         self.zip_create(fpath)
 
         root = self.zip_root or pl.Path()
         paths = [pl.Path(x) for x in args]
@@ -110,15 +113,15 @@
                     targ.write(str(file_to_add), write_as)
 
                 except ValueError:
                     relpath = root / pl.Path(file_to_add).name
                 except FileNotFoundError as err:
                     logging.warning(f"Adding File to Zip {fpath} failed: {err}", file=sys.stderr)
 
-    def zip_globs(self, fpath, *globs:str, ignore_dots=False):
+    def zip_globs(self, fpath:pl.Path, *globs:str, ignore_dots=False):
         """
         Add files chosen by globs to the zip, relative to the cwd
         """
         logging.debug(f"Zip Globbing: %s : %s", fpath, globs)
         assert(fpath.suffix == ".zip")
         self.zip_create(fpath)
 
@@ -137,28 +140,29 @@
                             case True:
                                 logging.warning("Duplication Attempt: %s -> %s", globf, relpath)
                             case False:
                                 targ.write(str(globf), relpath)
                     except FileNotFoundError as err:
                         logging.warning(f"Adding File to Zip {fpath} failed: {err}", file=sys.stderr)
 
-    def zip_add_str(self, fpath, fname, text:str):
+    def zip_add_str(self, fpath:pl.Path, fname:str, text:str):
+        """ add a string of text to a zip file as a new file """
         assert(fpath.suffix == ".zip")
         self.zip_create(fpath)
 
         compress_type, compress_level = self._zip_get_compression_settings()
         with zipfile.ZipFile(fpath, mode='a', compression=compress_type, compresslevel=compress_level, allowZip64=True) as targ:
             match fname in targ.namelist():
                 case True:
                     logging.warning("Duplication Attempt: %s -> %s", fpath, fname)
                 case False:
                     targ.writestr(fname, text)
 
 
-    def zip_get_contents(self, fpath) -> list[str]:
+    def zip_get_contents(self, fpath:pl.Path) -> list[str]:
         with zipfile.Zipfile(fpath):
             return zipfile.namelist()
 
 
     def zip_unzip_to(self, fpath:pl.Path, *zips:pl.Path, fn=None):
         """
         extract everything or everything that returns true from fn, from all zips given
@@ -170,15 +174,17 @@
             logging.debug("Extracting: %s (%s) to %s", zipf, fn, fpath)
             (fpath / zipf.stem).mkdir(parents=True, exist_ok=True)
             with zipfile.ZipFile(zipf) as targ:
                 subset = [x for x in targ.namelist() if fn(x)]
                 targ.extractall(fpath / zipf.stem, members=subset)
 
     def zip_unzip_concat(self, fpath:pl.Path, *zips:pl.Path, member=None, header=b"\n\n#------\n\n", footer=b"\n\n#------\n\n"):
-        """ Unzip and concatenate an fpath within multiple zip files, into a single file """
+        """ Unzip a member file in a multiple zip files,
+          append their text contents into a single file """
+        assert(member is not None)
         with open(fpath, "ab") as out:
             for zipf in zips:
                 try:
                     logging.debug("Concating: %s (%s) to %s", zipf, member, fpath)
                     with zipfile.ZipFile(zipf) as targ:
                         data = targ.read(member)
                         if header:
@@ -187,19 +193,21 @@
                         if footer:
                             out.write(footer)
 
                 except Exception as err:
                     logging.warning("Issue reading: %s : %s", zipf, err)
 
     def zip_test(self, *zips:pl.Path):
+        """ Test the validity of zip files """
         for zipf in zips:
             with zipfile.ZipFile(zipf) as targ:
                 result = targ.testzip()
                 if result is not None:
                     logging.warning("Issue with %s : %s", zipf, targ)
 
 
-    def zip_contains(self, fpath, *args) -> bool:
+    def zip_contains(self, fpath:pl.Path, *zips:pl.Path) -> bool:
+        """ test that multiple zip files contain a specified filename """
         with zipfile.ZipFile(fpath, "r") as zipf:
             contents = zipf.namelist()
 
         return all([x in contents for x in args])
```

### Comparing `doot-0.6.1/doot/mixins/importer.py` & `doot-0.7.0/doot/mixins/importer.py`

 * *Files 20% similar despite different names*

```diff
@@ -27,24 +27,26 @@
 ##-- end imports
 
 ##-- logging
 logging = logmod.getLogger(__name__)
 ##-- end logging
 
 import importlib
+import doot
 import doot.errors
-from doot.constants import IMPORT_SEP
 from doot._abstract.loader import PluginLoader_p
 
+IMPORT_SEP   = doot.constants.patterns.IMPORT_SEP
 ACTION_CTORS = {}
 
 if PluginLoader_p.loaded:
     ACTION_CTORS = {x.name : x for x in PluginLoader_p.loaded.action}
 
-class Importer_M:
+class Importer_m:
+    """ Mixin for importing using doot aliases """
 
     def import_task(self, pathname:None|str):
         """
           given a path in the form `package.sub.sub:Class`, import the package, and return the named class.
         """
         if pathname is None:
             return None
@@ -53,19 +55,19 @@
                 return ACTION_CTORS[pathname].load()
 
             logging.info("Importing: %s", pathname)
             module_name, cls_name = pathname.split(IMPORT_SEP)
             module = importlib.import_module(module_name)
             return getattr(module, cls_name)
         except ImportError as err:
-            raise doot.errors.DootTaskLoadError("Import Failed: %s : %s", pathname, err.msg, task=self.spec) from err
+            raise doot.errors.DootTaskLoadError("Task Import Failed: %s : %s", pathname, err.msg, task=self.spec) from err
         except (AttributeError, KeyError) as err:
-            raise doot.errors.DootTaskLoadError("Import Failed: Module has missing attribute/key: %s", pathname, task=self.spec) from err
+            raise doot.errors.DootTaskLoadError("Task Import Failed: Module has missing attribute/key: %s", pathname, task=self.spec) from err
         except ValueError as err:
-            raise doot.errors.DootTaskLoadError("Import Failed: Can't split %s", pathname, task=self.spec) from err
+            raise doot.errors.DootTaskLoadError("Task Import Failed: Can't split %s : %s", pathname, task=self.spec) from err
 
 
     def import_callable(self, pathname:None|str) -> None|callable[Any]:
         """
           given a path in the form `package.sub.sub:function`, import the package, and return the named function.
         """
         if pathname is None:
@@ -78,19 +80,19 @@
             logging.info("Importing: %s", pathname)
             module_name, fun_name = pathname.split(IMPORT_SEP)
             module                = importlib.import_module(module_name)
             fun                   = getattr(module, fun_name)
             assert(callable(fun))
             return fun
         except ImportError as err:
-            raise doot.errors.DootTaskLoadError("Import Failed: %s : %s", pathname, err.msg, task=self.spec) from err
+            raise doot.errors.DootTaskLoadError("Callable Import Failed: %s : %s", pathname, err.msg, task=self.spec) from err
         except (AttributeError, KeyError) as err:
-            raise doot.errors.DootTaskLoadError("Import Failed: Module has missing attribute/key: %s", pathname, task=self.spec) from err
+            raise doot.errors.DootTaskLoadError("Callable Import Failed: Module has missing attribute/key: %s : %s", pathname, err.args, task=self.spec) from err
         except ValueError as err:
-            raise doot.errors.DootTaskLoadError("Import Failed: Can't split %s", pathname, task=self.spec) from err
+            raise doot.errors.DootTaskLoadError("Callable Import Failed: Can't split %s", pathname, task=self.spec) from err
 
     def import_class(self, pathname:None|str, *, is_task_ctor=False) -> None|type[Any]:
         """
           given a path in the form `package.sub.sub:Class`, import the package, and return the named class.
         """
         if pathname is None:
             return None
@@ -99,12 +101,12 @@
                 return ACTION_CTORS[pathname].load()
 
             logging.info("Importing: %s", pathname)
             module_name, cls_name = pathname.split(IMPORT_SEP)
             module = importlib.import_module(module_name)
             return getattr(module, cls_name)
         except ImportError as err:
-            raise doot.errors.DootInvalidConfig("Import Failed: %s : %s", pathname, err.msg) from err
+            raise doot.errors.DootInvalidConfig("Class Import Failed: %s : %s", pathname, err.msg) from err
         except (AttributeError, KeyError) as err:
-            raise doot.errors.DootInvalidConfig("Import Failed: Module has missing attribute/key: %s", pathname) from err
+            raise doot.errors.DootInvalidConfig("Class Import Failed: Module has missing attribute/key: %s", pathname) from err
         except ValueError as err:
-            raise doot.errors.DootInvalidConfig("Import Failed: Can't split %s", pathname) from err
+            raise doot.errors.DootInvalidConfig("Class Import Failed: Can't split %s", pathname) from err
```

### Comparing `doot-0.6.1/doot/mixins/job/limiter.py` & `doot-0.7.0/doot/task/base_job.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,133 +1,131 @@
 #!/usr/bin/env python3
 """
-
-
-See EOF for license/metadata/notes as applicable
+Utility classes for building tasks with a bit of structure
 """
-
-##-- builtin imports
+##-- imports
 from __future__ import annotations
 
 # import abc
-import datetime
-import enum
+# import datetime
+# import enum
 import functools as ftz
 import itertools as itz
 import logging as logmod
 import pathlib as pl
 import re
 import time
 import types
-import weakref
 # from copy import deepcopy
 # from dataclasses import InitVar, dataclass, field
 from typing import (TYPE_CHECKING, Any, Callable, ClassVar, Final, Generic,
                     Iterable, Iterator, Mapping, Match, MutableMapping,
                     Protocol, Sequence, Tuple, TypeAlias, TypeGuard, TypeVar,
                     cast, final, overload, runtime_checkable, Generator)
-from uuid import UUID, uuid1
-
-##-- end builtin imports
+# from uuid import UUID, uuid1
+# from weakref import ref
 
-##-- lib imports
-import more_itertools as mitz
-##-- end lib imports
+##-- end imports
 
 ##-- logging
 logging = logmod.getLogger(__name__)
 ##-- end logging
-printer = logmod.getLogger("doot._printer")
 
 from tomlguard import TomlGuard
 import doot
 import doot.errors
-from doot._abstract import Job_i
-from doot.structs import DootCodeReference, DootTaskSpec, DootTaskName, DootKey
-from doot.mixins.job.expander import WalkExpander_M
+from doot.enums import TaskFlags
+from doot.structs import DootTaskSpec, TaskStub, TaskStubPart, DootTaskName, DootCodeReference, DootStructuredName
+from doot._abstract import Job_i, Task_i
+from doot.errors import DootDirAbsent
+from doot.task.base_task import DootTask
+
+SUBTASKED_HEAD = doot.constants.patterns.SUBTASKED_HEAD
+
+@doot.check_protocol
+class DootJob(Job_i, DootTask):
+    """ Util Class for building single tasks
+      wraps with setup and teardown tasks,
+      manages cleaning,
+      and holds state
 
-class TaskLimit_M:
     """
-      Limit the number of task the job generates
-    """
-
-    def __init__(self, spec):
-        super().__init__(spec)
-        match self.spec.extra.on_fail("identity", str).early_select_fn():
-            case "identity":
-                self.early_select_fn = self._identity_select
-            case str() as s:
-                ref = DootCodeReference.from_str(s)
-                self.early_select_fn = ref.try_import()
-
-        match self.spec.extra.on_fail("hard", str).select_limit_type().lower():
-            case "hard":
-                self.limit_type = "hard"
-            case "soft":
-                self.limit_type = "soft"
-            case x:
-                raise doot.errors.DootConfigError("Bad select_limit_type value", str(self.spec.name), x)
+    _help = ["A Basic Task Constructor"]
+    _default_flags = TaskFlags.JOB
 
-        self.select_limit = self.spec.extra.on_fail((None,), None|int).select_limit()
-        match self.select_limit:
+    def __init__(self, spec:DootTaskSpec):
+        assert(spec is not None), "Spec is empty"
+        super(DootJob, self).__init__(spec)
+
+    def default_task(self, name:str|DootTaskName|None, extra:None|dict|TomlGuard) -> DootTaskSpec:
+        task_name = None
+        match name:
             case None:
-                pass
-            case x if x < 1:
-                raise doot.errors.DootTaskError("Can't subselect a non-positive amount")
-
-        match self.spec.extra.on_fail("all", str).late_select_fn():
-            case "all" | "All":
-                self.late_select_fn = self._select_all
-            case "random" | "Random":
-                self.late_select_fn = self._random_select
-            case str() as s:
-                ref = DootCodeReference.from_str(s)
-                self.late_select_fn = ref.try_import()
-
-    def _build_subs(self) -> Generator[DootTaskSpec]:
-        logging.debug("%s : Building Subselection Walker SubTasks", self.name)
-
-        selected = []
-        for task in super()._build_subs():
-            match task:
-                case None:
-                    pass
-                case DootTaskSpec() as sub if self.early_select_fn(self, sub):
-                    selected.append(sub)
-
-        filtered = self.late_select_fn(self, selected)
-        self.total_subtasks = len(filtered)
-
-        match self.limit_type, self.select_limit, self.total_subtasks:
-            case _, None, _:
-                pass
-            case "hard", lim, total if lim <= total:
-                raise doot.errors.DootTaskError("Job broke its subtask limit", str(self.spec.name), self.select_limit, self.total_subtasks)
-            case "soft", lim, total if lim <= total:
-                logging.debug("Soft Limiting Job: %s : (limit %s) < (generated %s))", str(self.spec.name), lim, total)
-                filtered = filtered[:lim]
+                task_name = self.fullname.subtask(SUBTASKED_HEAD)
+            case str():
+                task_name = self.fullname.subtask(name)
+            case DootTaskName():
+                task_name = name
             case _:
-                pass
+                raise doot.errors.DootTaskError("Bad value used to make a subtask in %s : %s", self.name, name)
 
-        for task in filtered:
-            yield task
+        assert(task_name is not None)
+        return DootTaskSpec(name=task_name, extra=TomlGuard(extra))
 
+    def is_stale(self, task:Task_i):
+        return False
 
-    @staticmethod
-    def _identity_select(job:Job_i, spec:DootTaskSpec) -> bool:
-        return True
+    def specialize_task(self, task):
+        return task
 
-    @staticmethod
-    def _random_select(job:Job_i, specs:list[DootTaskSpec]) -> list[DootTaskSpec]:
-        return random.sample(specs, match_amnt)
-
-    @staticmethod
-    def _select_all(job:Job_i, specs:list[DootTaskSpec]) -> list[DootTaskSpec]:
-        return specs
+    @classmethod
+    def stub_class(cls, stub) -> TaskStub:
+        # Come first
+        stub['active_when'].priority    = -90
+        stub['required_for'].priority   = -90
+        stub['depends_on'].priority     = -100
+
+        stub['head_task'].set(type="taskname", default="", prefix="# ", priority=100)
+        stub['queue_behaviour'].default = "default"
+        stub['queue_behaviour'].comment = "default | auto | reactive"
+        return stub
+
+    def stub_instance(self, stub) -> TaskStub:
+        stub                      = self.__class__.stub_class(stub)
+        stub['name'].default      = self.fullname
+        if bool(self.doc):
+            stub['doc'].default   = [f"\"{x}\"" for x in self.doc]
+        return stub
 
     @classmethod
-    def stub_class(cls, stub):
-        stub['early_select_fn'].set(type="callable",    default="identity", priority=100, comment=" : [job, spec] -> bool")
-        stub['late_select_fn'].set(type="callable",    default="all", priority=100, comment=" : [job, list[spec]] -> list[spec]. (all, random, or coderef)")
+    def class_help(cls) -> str:
+        """ Job *class* help. """
+        help_lines = [f"Job : {cls.__qualname__} v{cls._version}    ({cls.__module__}:{cls.__qualname__})", ""]
+
+        mro = " -> ".join(x.__name__ for x in cls.mro())
+        help_lines.append(f"Job MRO: {mro}")
+        help_lines.append("")
+        help_lines += cls._help
+
+        params = cls.param_specs
+        if bool([x for x in params if not x.invisible]):
+            help_lines += ["", "Params:"]
+            help_lines += [str(x) for x in cls.param_specs if not x.invisible]
+
+        return "\n".join(help_lines)
+
+    def _build_head(self, **kwargs) -> None|DootTaskSpec:
+        logging.debug("Building Head Task for: %s", self.name)
+        inject_keys = set(self.spec.inject)
+        inject_dict = {k: self.spec.extra[k] for k in inject_keys if k in self.spec.extra}
+        extra       = {}
+        extra.update(kwargs)
+        extra.update(inject_dict)
+        task_spec                 = self.default_task(None, TomlGuard(extra))
+        task_spec.queue_behaviour = "auto"
+        task_spec.print_levels    = self.spec.print_levels
+
+        task_ref                  = self.spec.extra.on_fail((None,), None|str).head_task()
+        if task_ref is not None:
+            task_spec.ctor = DootStructuredName.build(task_ref)
 
-        stub['select_limit_type'].set(type="str", default="hard", priority=100, comment="hard | soft")
-        stub['select_limit'].set(type="int|None", default="5", priority=100, prefix="# ")
+        return task_spec
```

### Comparing `doot-0.6.1/doot/mixins/job/setup.py` & `doot-0.7.0/doot/actions/job_actions.py`

 * *Files 25% similar despite different names*

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
@@ -31,50 +30,68 @@
 
 ##-- lib imports
 import more_itertools as mitz
 ##-- end lib imports
 
 ##-- logging
 logging = logmod.getLogger(__name__)
+printer = logmod.getLogger("doot._printer")
 ##-- end logging
 
 
-from collections import defaultdict
+import random
 from tomlguard import TomlGuard
 import doot
 import doot.errors
-from doot.errors import DootDirAbsent, DootTaskError
-from doot.structs import DootTaskSpec, DootTaskName, DootCodeReference, DootActionSpec
+from doot.structs import DootKey, DootTaskSpec, DootTaskName, DootCodeReference
+from doot.actions.base_action import DootBaseAction
+from doot.actions.job_expansion import JobGenerate, JobExpandAction, JobMatchAction
+from doot.actions.job_injection import JobPrependActions, JobAppendActions, JobInjector, JobInjectPathParts, JobInjectShadowAction, JobSubNamer
+from doot.actions.job_queuing import JobQueueAction, JobQueueHead, JobChainer
+from doot.mixins.path_manip import Walker_m
 
 
-class SetupStage_M:
+class JobWalkAction(Walker_m, DootBaseAction):
+    """
+      Triggers a directory walk to build tasks from
     """
-      A terse mixin to add a single setup task before all subtasks/head of this job
+
+    @DootKey.dec.types("roots", "exts")
+    @DootKey.dec.types("recursive", hint={"type_": bool|None})
+    @DootKey.dec.references("fn")
+    @DootKey.dec.redirects("update_")
+    def __call__(self, spec, state, roots, exts, recursive, fn, _update):
+        exts    = {y for x in (exts or []) for y in [x.lower(), x.upper()]}
+        rec     = recursive or False
+        roots   = [DootKey.build(x).to_path(spec, state) for x in roots]
+        match fn:
+            case DootCodeReference():
+                accept_fn = fn.try_import()
+            case None:
+                accept_fn = lambda x: True
+
+        results = [x for x in self.walk_all(roots, exts, rec=rec, fn=accept_fn)]
+        return { _update : results }
+
+class JobLimitAction(DootBaseAction):
+    """
+      Limits a list to an amount, overwriting the 'from' key,
+      'method' defaults to a random sample,
+      or a coderef of type callable[[spec, state, list[taskspec]], list[taskspec]]
+
     """
 
-    @classmethod
-    def stub_class(cls, stub):
-        stub['setup_actions'].set(type="list[dict]",   default=[])
-
-    def build(self, **kwargs):
-        entry_task = self._build_setup(kwargs)
-        for task in super().build(**kwargs):
-            match task:
-                case None:
-                    pass
-                case DootTaskSpec():
-                    task.depends_on.append(entry_task.name)
-                    yield task
-
-        yield entry_task
-
-
-    def _build_setup(self, kwargs) -> DootTaskSpec:
-        inject_keys = set(self.spec.inject)
-        inject_dict = {k: self.spec.extra[k] for k in inject_keys}
-        kwargs.update(inject_dict)
-        setup = self.default_task("$entry$", kwargs)
-        spec_setup_actions     = [DootActionSpec.from_data(x) for x in self.spec.extra.on_fail([], list).setup_actions()]
-        setup.actions         += spec_setup_actions
-        setup.priority        += self.spec.priority
+    @DootKey.dec.types("from_", "count")
+    @DootKey.dec.references("method")
+    @DootKey.dec.redirects("from_")
+    def __call__(self, spec, state, _from, count, method, _update):
+        if count == -1:
+            return
+
+        match method:
+            case None:
+                limited = random.sample(_from, count)
+            case DootCodeReference():
+                fn      = method.try_import()
+                limited = fn(spec, state, _from)
 
-        return setup
+        return { _update : limited }
```

### Comparing `doot-0.6.1/doot/mixins/runner/fail_handler.py` & `doot-0.7.0/doot/reporters/stack_manager.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 #!/usr/bin/env python3
 """
 
-
-See EOF for license/metadata/notes as applicable
 """
 
 ##-- builtin imports
 from __future__ import annotations
 
 # import abc
 import datetime
@@ -33,20 +31,30 @@
 import more_itertools as mitz
 ##-- end lib imports
 
 ##-- logging
 logging = logmod.getLogger(__name__)
 ##-- end logging
 
-printer = logmod.getLogger("doot._printer")
-
-import doot
-import doot.errors
-from doot.structs import DootKey
+from doot._abstract import Reporter_i, ReportLine_i
+from doot.structs import DootTraceRecord
 
-class RunnerFailHandler:
+class DootReportManagerStack(Reporter_i):
     """
-      A Mixin for changing how a task runner handles failure
+    A Stack of Reporters to try using.
+    The First one that returns a DootTrace is used.
     """
 
-    def _handle_failure(self, task, err):
-        pass
+    def __init__(self, reporters:list[ReportLine_i]=None):
+        super().__init__(reporters)
+
+    def __str__(self):
+        result = []
+        for trace in self._full_trace:
+            for reporter in self._reporters:
+                match reporter(trace):
+                    case None:
+                        continue
+                    case str() as res:
+                        result.append(res)
+
+        return "\n".join(result)
```

### Comparing `doot-0.6.1/doot/parsers/__tests/test_flexible.py` & `doot-0.7.0/doot/parsers/__tests/test_flexible.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,16 +11,19 @@
 from typing import (Any, Callable, ClassVar, Generic, Iterable, Iterator,
                     Mapping, Match, MutableMapping, Sequence, Tuple, TypeAlias,
                     TypeVar, cast)
 ##-- end imports
 logging = logmod.root
 
 import pytest
+import doot
+doot._test_setup()
+
 import doot.errors
-from doot._abstract import ArgParser_i, TaskBase_i
+from doot._abstract import ArgParser_i, Task_i
 from doot.parsers.flexible import DootFlexibleParser
 from doot.structs import DootParamSpec, DootTaskSpec, DootCodeReference
 from doot.utils.mock_gen import mock_parse_cmd, mock_parse_task
 
 
 @pytest.mark.parametrize("ctor", [DootFlexibleParser])
 class TestArgParser:
```

### Comparing `doot-0.6.1/doot/parsers/flexible.py` & `doot-0.7.0/doot/parsers/flexible.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,25 +25,25 @@
 ##-- logging
 logging = logmod.getLogger(__name__)
 ##-- end logging
 
 from tomlguard import TomlGuard
 import doot
 import doot.errors
-from doot.constants import PARAM_ASSIGN_PREFIX, NON_DEFAULT_KEY
 from doot._abstract import ArgParser_i
 from doot.structs import DootParamSpec, DootTaskSpec
 from collections import ChainMap
 
-SEP : Final[str] = "--"
+SEP : Final[str]          = "--"
+PARAM_ASSIGN_PREFIX       = doot.constants.patterns.PARAM_ASSIGN_PREFIX
+NON_DEFAULT_KEY           = doot.constants.misc.NON_DEFAULT_KEY
 
 default_task : Final[str] = doot.config.on_fail((None,)).general.settings.default_task()
 default_cmd  : Final[str] = doot.config.on_fail("run", str).general.settings.default_cmd()
 
-@doot.check_protocol
 class DootFlexibleParser(ArgParser_i):
     """
     convert argv to tomlguard by:
     parsing each arg as toml,
 
     # doot {args} {cmd} {cmd_args}
     # doot {args} [{task} {tasks_args}] - implicit do cmd
@@ -175,28 +175,28 @@
     def process_task(self, args) -> list[str]:
         """ consume arguments for tasks """
         logging.debug("Task Parsing: %s", args)
         if args[0] not in self.registered_tasks:
             task                     = self.registered_tasks[default_task]
             assert(isinstance(task, DootTaskSpec))
             task_name                 = default_task
-            spec_params               = [DootParamSpec.from_dict(x) for x in task.extra.on_fail([], list).cli()]
+            spec_params               = [DootParamSpec.build(x) for x in task.extra.on_fail([], list).cli()]
             ctor_params               = task.ctor.try_import().param_specs
             current_specs             = list(sorted(spec_params + ctor_params, key=DootParamSpec.key_func))
             task_args                 = self._build_defaults_dict(current_specs)
             task_args[NON_DEFAULT_KEY] = []
             self.tasks_args.append((task_name, task_args))
             return args
 
 
         while bool(args) and args[0] in self.registered_tasks:
             task_name                 = args.pop(0)
             task                      = self.registered_tasks[task_name]
             assert(isinstance(task, DootTaskSpec))
-            spec_params               = [DootParamSpec.from_dict(x) for x in task.extra.on_fail([], list).cli()]
+            spec_params               = [DootParamSpec.build(x) for x in task.extra.on_fail([], list).cli()]
             ctor_params               = task.ctor.try_import().param_specs
             current_specs             = list(sorted(spec_params + ctor_params, key=DootParamSpec.key_func))
             task_args                 = self._build_defaults_dict(current_specs)
             default_args              = task_args.copy()
             logging.debug("Parsing Task args for: %s: Available: %s", task_name, task_args.keys())
 
             while bool(args) and args[0] not in self.registered_tasks:
```

### Comparing `doot-0.6.1/doot/reporters/__tests/test_stack_manager.py` & `doot-0.7.0/doot/reporters/__tests/test_stack_manager.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,14 +8,17 @@
 import pathlib as pl
 from typing import (Any, Callable, ClassVar, Generic, Iterable, Iterator,
                     Mapping, Match, MutableMapping, Sequence, Tuple, TypeAlias,
                     TypeVar, cast)
 import warnings
 
 import pytest
+import doot
+doot._test_setup()
+
 from doot._abstract import Reporter_i
 from doot.reporters.stack_manager import DootReportManagerStack
 from doot.structs import DootTraceRecord
 from doot.enums import ReportEnum
 
 logging = logmod.root
 
@@ -37,88 +40,88 @@
         manager = DootReportManagerStack()
         assert(isinstance(manager, Reporter_i))
 
 
     def test_add_basic_trace(self):
         manager = DootReportManagerStack()
         assert(not bool(manager._full_trace))
-        manager.trace("test")
+        manager.add_trace("test")
         assert(bool(manager._full_trace))
         assert(isinstance(manager._full_trace[0], DootTraceRecord))
 
     def test_multi_add(self):
         manager = DootReportManagerStack()
         assert(not bool(manager._full_trace))
-        manager.trace("test")
-        manager.trace("test")
-        manager.trace("test")
+        manager.add_trace("test")
+        manager.add_trace("test")
+        manager.add_trace("test")
         assert(len(manager._full_trace) == 3)
         assert(all(isinstance(x, DootTraceRecord) for x in manager._full_trace))
 
 
     def test_str(self):
         manager = DootReportManagerStack()
-        manager.trace("test")
-        manager.trace("test")
-        manager.trace("test")
+        manager.add_trace("test")
+        manager.add_trace("test")
+        manager.add_trace("test")
         assert(str(manager) == "test\ntest\ntest")
 
 
     def test_custom_formatter(self):
         class SimpleFormatter:
-            def __call__(self, trace):
-                return "- {}".format(trace)
+            def __call__(self, add_trace):
+                return "- {}".format(add_trace)
 
         manager = DootReportManagerStack([SimpleFormatter()])
-        manager.trace("test")
-        manager.trace("test")
-        manager.trace("test")
+        manager.add_trace("test")
+        manager.add_trace("test")
+        manager.add_trace("test")
         assert(str(manager) == "- test\n- test\n- test")
 
 
     def test_custom_filter(self):
         class SimpleFilter:
-            def __call__(self, trace):
-                if ReportEnum.TASK in trace.flags:
-                    return str(trace)
+            def __call__(self, add_trace):
+                if ReportEnum.TASK in add_trace.flags:
+                    return str(add_trace)
 
         manager = DootReportManagerStack([SimpleFilter()])
-        manager.trace("first", flags=ReportEnum.TASK)
-        manager.trace("second", flags=ReportEnum.JOB)
-        manager.trace("third", flags=ReportEnum.TASK)
+        manager.add_trace("first", flags=ReportEnum.TASK)
+        manager.add_trace("second", flags=ReportEnum.JOB)
+        manager.add_trace("third", flags=ReportEnum.TASK)
         assert(str(manager) == "first\nthird")
 
 
     def test_multi_filter(self):
         class SimpleTaskFilter:
-            def __call__(self, trace):
-                if trace.flags in ReportEnum.TASK:
-                    return str(trace)
+            def __call__(self, add_trace):
+                if add_trace.flags in ReportEnum.TASK:
+                    return str(add_trace)
 
         class SimpleActionFilter:
-            def __call__(self, trace):
-                if trace.flags in ReportEnum.ACTION:
-                    return str(trace)
+            def __call__(self, add_trace):
+                if add_trace.flags in ReportEnum.ACTION:
+                    return str(add_trace)
 
         manager = DootReportManagerStack([ SimpleTaskFilter(), SimpleActionFilter() ])
-        manager.trace("first", flags=ReportEnum.TASK)
-        manager.trace("second", flags=ReportEnum.JOB)
-        manager.trace("third", flags=ReportEnum.ACTION)
+        manager.add_trace("first", flags=ReportEnum.TASK)
+        manager.add_trace("second", flags=ReportEnum.JOB)
+        manager.add_trace("third", flags=ReportEnum.ACTION)
         assert(str(manager) == "first\nthird")
 
 
     def test_combined_filter_formatter(self):
         class SimpleTaskFilter:
-            def __call__(self, trace):
-                if trace.flags in ReportEnum.TASK:
-                    return str(trace)
+            def __call__(self, add_trace):
+                if add_trace.flags in ReportEnum.TASK:
+                    return str(add_trace)
 
         class SimpleActionFilter:
-            def __call__(self, trace):
-                if trace.flags in ReportEnum.ACTION:
-                    return "- {}".format(trace)
+            def __call__(self, add_trace):
+                if add_trace.flags in ReportEnum.ACTION:
+                    return "- {}".format(add_trace)
 
         manager = DootReportManagerStack([ SimpleTaskFilter(), SimpleActionFilter() ])
-        manager.trace("first", flags=ReportEnum.TASK)
-        manager.trace("second", flags=ReportEnum.JOB)
-        manager.trace("third", flags=ReportEnum.ACTION)
+        manager.add_trace("first", flags=ReportEnum.TASK)
+        manager.add_trace("second", flags=ReportEnum.JOB)
+        manager.add_trace("third", flags=ReportEnum.ACTION)
         assert(str(manager) == "first\n- third")
```

### Comparing `doot-0.6.1/doot/reporters/__tests/test_summary_manager.py` & `doot-0.7.0/doot/reporters/__tests/test_summary_manager.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,14 +9,17 @@
 from typing import (Any, Callable, ClassVar, Generic, Iterable, Iterator,
                     Mapping, Match, MutableMapping, Sequence, Tuple, TypeAlias,
                     TypeVar, cast)
 import warnings
 
 import pytest
 
+import doot
+doot._test_setup()
+
 from doot.reporters.summary_manager import DootReportManagerSummary
 from doot.enums import ReportEnum
 from doot.structs import DootTraceRecord
 from doot._abstract import Reporter_i, ReportLine_i
 
 logging = logmod.root
 
@@ -37,27 +40,27 @@
     def test_initial(self):
         manager = DootReportManagerSummary()
         assert(isinstance(manager, Reporter_i))
 
     def test_add_basic_trace(self):
         manager = DootReportManagerSummary()
         assert(not bool(manager._full_trace))
-        manager.trace("test")
+        manager.add_trace("test")
         assert(bool(manager._full_trace))
         assert(isinstance(manager._full_trace[0], DootTraceRecord))
 
     def test_multi_add(self):
         manager = DootReportManagerSummary()
         assert(not bool(manager._full_trace))
-        manager.trace("test")
-        manager.trace("test")
-        manager.trace("test")
+        manager.add_trace("test")
+        manager.add_trace("test")
+        manager.add_trace("test")
         assert(len(manager._full_trace) == 3)
         assert(all(isinstance(x, DootTraceRecord) for x in manager._full_trace))
 
     @pytest.mark.skip("TODO")
     def test_str(self):
         manager = DootReportManagerSummary()
-        manager.trace("test", flags=ReportEnum.SUCCEED | ReportEnum.TASK)
-        manager.trace("test", flags=ReportEnum.FAIL    | ReportEnum.JOB)
-        manager.trace("test", flags=ReportEnum.SUCCEED | ReportEnum.ACTION)
+        manager.add_trace("test", flags=ReportEnum.SUCCEED | ReportEnum.TASK)
+        manager.add_trace("test", flags=ReportEnum.FAIL    | ReportEnum.JOB)
+        manager.add_trace("test", flags=ReportEnum.SUCCEED | ReportEnum.ACTION)
         assert(isinstance(manager) == "    - Jobs: 0/1\n    - Tasks  : 1/0\n    - Actions: 1/0")
```

### Comparing `doot-0.6.1/doot/reporters/basic_reporters.py` & `doot-0.7.0/doot/utils/url_expand.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,58 +1,51 @@
 #!/usr/bin/env python3
 """
 
-
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
 
-from doot.structs import DootTraceRecord
-from doot._abstract import Reporter_i
-
-class DootAlwaysReport(Reporter_i):
-    def __call__(self, trace):
-        return str(trace)
-
-class TimeReporter(Reporter_i):
-
-    def __call__(self, trace):
-        time = trace.time.strftime("%H:%M")
-        return "{:10} : {}".format(time, str(trace))
-
+from time import sleep
+import requests
 
 
-"""
-
-
-"""
+def expander(current):
+    # header = {'user-agent': args.agent}
+    try:
+        response = requests.head(current, allow_redirects=True, timeout=2, headers=header)
+        if response.ok:
+            expanded[current] = response.url
+        else:
+            expanded[current] = response.status_code
+
+        return "{} |%| {}".format(current, args.separator, expanded[current])
+    except Exception as err:
+        cmd    = 'say -v Moira -r 50 "Error"'
+        system(cmd)
+        expanded[current] = f"400.1 : {str(err)}"
+        logging.info("Error: %s", str(err))
```

### Comparing `doot-0.6.1/doot/reporters/stack_manager.py` & `doot-0.7.0/doot/_abstract/structs.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 #!/usr/bin/env python3
 """
 
+
+See EOF for license/metadata/notes as applicable
 """
 
 ##-- builtin imports
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
@@ -24,37 +26,36 @@
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
 
-from doot._abstract import Reporter_i, ReportLine_i
-from doot.structs import DootTraceRecord
+import tomlguard
 
-class DootReportManagerStack(Reporter_i):
-    """
-    A Stack of Reporters to try using.
-    The First one that returns a DootTrace is used.
-    """
-
-    def __init__(self, reporters:list[ReportLine_i]=None):
-        super().__init__(reporters)
-
-    def __str__(self):
-        result = []
-        for trace in self._full_trace:
-            for reporter in self._reporters:
-                match reporter(trace):
-                    case None:
-                        continue
-                    case str() as res:
-                        result.append(res)
+class SpecStruct_p(abc.ABC):
+    """ Base class for specs, for type matching """
 
-        return "\n".join(result)
+    @property
+    @abc.abstractmethod
+    def params(self) -> dict|tomlguard.TomlGuard:
+        pass
+
+class ArtifactStruct_p(abc.ABC):
+    """ Base class for artifacts, for type matching """
+    pass
+
+class StubStruct_p(abc.ABC):
+    """ Base class for stubs, for type matching """
+    pass
+
+class ParamStruct_p(abc.ABC):
+    """ Base class for param specs, for type matching """
+    pass
```

### Comparing `doot-0.6.1/doot/reporters/summary_manager.py` & `doot-0.7.0/doot/reporters/summary_manager.py`

 * *Files identical despite different names*

### Comparing `doot-0.6.1/doot/structs.py` & `doot-0.7.0/doot/structs.py`

 * *Files 13% similar despite different names*

```diff
@@ -24,14 +24,17 @@
                     Protocol, Sequence, Tuple, TypeAlias, TypeGuard, TypeVar,
                     cast, final, overload, runtime_checkable)
 from uuid import UUID, uuid1
 
 ##-- end builtin imports
 
 from doot._structs.param_spec import DootParamSpec
-from doot._structs.sname import DootCodeReference, DootTaskName, DootStructuredName
+from doot._structs.sname import DootStructuredName
+from doot._structs.task_name import DootTaskName
+from doot._structs.code_ref import DootCodeReference
 from doot._structs.action_spec import DootActionSpec
 from doot._structs.task_spec import DootTaskSpec
 from doot._structs.artifact import DootTaskArtifact
 from doot._structs.stub import TaskStub, TaskStubPart
 from doot._structs.trace import DootTraceRecord
 from doot._structs.key import DootKey
+from doot._structs.toml_loc import TomlLocation
```

### Comparing `doot-0.6.1/doot/task/__tests/test_base_job.py` & `doot-0.7.0/doot/task/__tests/test_base_job.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,65 +12,40 @@
 import warnings
 
 import pytest
 
 logging = logmod.root
 
 import doot
+doot._test_setup()
 from doot.enums import TaskFlags
 from doot.structs import DootTaskSpec, TaskStub
 from doot.task.base_job import DootJob
 import doot._abstract
 
 class TestBaseJob:
 
     def test_initial(self):
-        job = DootJob(DootTaskSpec.from_dict({"name": "basic::example", "flags": ["JOB"]}))
-        assert(isinstance(job, doot._abstract.TaskBase_i))
+        job = DootJob(DootTaskSpec.build({"name": "basic::example", "flags": ["JOB"]}))
+        assert(isinstance(job, doot._abstract.Task_i))
         assert(TaskFlags.JOB in job.spec.flags)
 
     def test_paramspecs(self):
-        job = DootJob(DootTaskSpec.from_dict({"name": "basic::example"}))
+        job = DootJob(DootTaskSpec.build({"name": "basic::example"}))
         param_specs = job.param_specs
         assert(isinstance(param_specs, list))
         assert(len(param_specs) == 3)
 
     def test_spec(self):
         ##-- setup
-        job1 = DootJob(DootTaskSpec.from_dict({"name" :"basic::example"}))
-        job2 = DootJob(DootTaskSpec.from_dict({"name" :"other.group::blah"}))
+        job1 = DootJob(DootTaskSpec.build({"name" :"basic::example"}))
+        job2 = DootJob(DootTaskSpec.build({"name" :"other.group::blah"}))
         ##-- end setup
         assert(str(job1.name) == "basic::example")
         assert(str(job2.name) == "\"other.group\"::blah")
         assert(job1 != job2)
         assert(job1 == job1)
 
-    def test_build(self):
-        ##-- setup
-        job = DootJob(DootTaskSpec.from_dict({"name": "basic::example"}))
-        ##-- end setup
-
-        # Run:
-        tasks = list(job.build())
-
-        ##-- check
-        assert(len(tasks) == 1)
-        ##-- end check
-        pass
-
-    def test_build_multi(self):
-        ##-- setup
-        job = DootJob(DootTaskSpec.from_dict({"name": "basic::example"}))
-        ##-- end setup
-
-        # Run:
-        tasks = list(job.build())
-
-        ##-- check
-        assert(len(tasks) == 1)
-        ##-- end check
-        pass
-
     def test_class_stub(self):
         stub_obj = TaskStub(ctor=DootJob)
         stub = DootJob.stub_class(stub_obj)
         assert(isinstance(stub, TaskStub))
```

### Comparing `doot-0.6.1/doot/task/__tests/test_base_task.py` & `doot-0.7.0/doot/task/__tests/test_base_task.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 import functools as ftz
 
 import pytest
 logging = logmod.root
 
 import tomlguard
 import doot
-import doot.constants
+doot._test_setup()
 from doot.structs import DootTaskSpec, TaskStub
 from doot.task.base_task import DootTask
 import doot._abstract
 
 ##-- reminder
 # caplog
 # mocker.patch | patch.object | patch.multiple | patch.dict | stopall | stop | spy | stub
@@ -40,61 +40,61 @@
 
     def test_initial(self):
         task = DootTask(DootTaskSpec(name="basic::example"), job=None)
         assert(isinstance(task, doot._abstract.Task_i))
 
 
     def test_lambda_action(self):
-        task         = DootTask(DootTaskSpec.from_dict({"name":"basic::example", "action_ctor":basic_action}), job=None)
+        task         = DootTask(DootTaskSpec.build({"name":"basic::example", "action_ctor":basic_action}), job=None)
         assert(isinstance(task, doot._abstract.Task_i))
 
 
     def test_expand_lambda_action(self):
-        task                = DootTask(DootTaskSpec.from_dict({"name":"basic::example", "action_ctor":basic_action, "actions": [{"do": "doot.actions.base_action:DootBaseAction", "args":["blah"]}]}), job=None)
+        task                = DootTask(DootTaskSpec.build({"name":"basic::example", "action_ctor":basic_action, "actions": [{"do": "doot.actions.base_action:DootBaseAction", "args":["blah"]}]}), job=None)
         actions             = list(task.actions)
         assert(len(actions) == 1)
 
 
     def test_run_lambda_action(self, caplog):
         caplog.set_level("DEBUG", logger="doot._printer")
-        task         = DootTask(DootTaskSpec.from_dict({"name":"basic::example", "action_ctor":basic_action, "actions": [{"do": "doot.actions.base_action:DootBaseAction", "args":["blah"]}]}), job=None)
+        task         = DootTask(DootTaskSpec.build({"name":"basic::example", "action_ctor":basic_action, "actions": [{"do": "doot.actions.base_action:DootBaseAction", "args":["blah"]}]}), job=None)
         actions      = list(task.actions)
         result       = actions[0]({"example": "state"})
         assert(result == {"count": 1})
         assert("Base Action Called: 0" in caplog.messages)
         assert("blah" in caplog.messages)
 
 
     def test_expand_action_str(self, caplog):
         caplog.set_level("DEBUG", logger="doot._printer")
-        task         = DootTask(DootTaskSpec.from_dict({"name":"basic::example", "action_ctor": "test_base_task:basic_action", "actions": [{"do": "doot.actions.base_action:DootBaseAction", "args":["blah"]}]}), job=None)
+        task         = DootTask(DootTaskSpec.build({"name":"basic::example", "action_ctor": "test_base_task:basic_action", "actions": [{"do": "doot.actions.base_action:DootBaseAction", "args":["blah"]}]}), job=None)
         actions      = list(task.actions)
         result       = actions[0]({"example": "state"})
         assert(result == {"count" : 1})
         assert("Base Action Called: 0" in caplog.messages)
 
     def test_toml_class_stub(self):
         """ build the simplest stub from the class itself """
         stub_obj = TaskStub(ctor=DootTask)
         stub     = DootTask.stub_class(stub_obj)
-        assert(str(stub['name'].default) == doot.constants.DEFAULT_STUB_TASK_NAME)
+        assert(str(stub['name'].default) == doot.constants.names.DEFAULT_STUB_TASK_NAME)
 
     def test_toml_instance_stub(self):
         """ build the next simplest stub from an instance of the task """
         stub_obj = TaskStub(ctor=DootTask)
-        task     = DootTask(DootTaskSpec.from_dict({"name" : "basic::example", "flags" : ["TASK", "IDEMPOTENT"]}), job=None)
+        task     = DootTask(DootTaskSpec.build({"name" : "basic::example", "flags" : ["TASK", "IDEMPOTENT"]}), job=None)
         stub     = task.stub_instance(stub_obj)
         assert(str(stub['name'].default) == "basic::example")
         as_str = stub.to_toml()
 
     def test_toml_instance_stub_rebuild(self):
         """ take a stub and turn it into a task spec  """
         stub_obj         = TaskStub(ctor=DootTask)
-        task             = DootTask(DootTaskSpec.from_dict({"name" : "basic::example", "flags" : ["TASK", "IDEMPOTENT"]}), job=None)
+        task             = DootTask(DootTaskSpec.build({"name" : "basic::example", "flags" : ["TASK", "IDEMPOTENT"]}), job=None)
         stub             = task.stub_instance(stub_obj)
         as_str           = stub.to_toml()
         loaded           = tomlguard.read(as_str)
         as_dict          = dict(loaded.tasks.basic[0])
         as_dict['group'] = "basic"
-        new_spec         = DootTaskSpec.from_dict(as_dict)
+        new_spec         = DootTaskSpec.build(as_dict)
         assert(isinstance(new_spec, DootTaskSpec))
         assert(str(new_spec.name) == str(task.spec.name))
```

### Comparing `doot-0.6.1/doot/task/check_locs.py` & `doot-0.7.0/doot/task/check_locs.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,31 +16,34 @@
 from tomlguard import TomlGuard
 import doot
 import doot.errors
 from doot.structs import DootTaskSpec
 from doot._abstract import Job_i
 from doot.task.base_job import DootJob
 from doot.task.base_task import DootTask
+from doot.enums import LocationMeta
 
 ##-- logging
 logging = logmod.getLogger(__name__)
 printer = logmod.getLogger("doot._printer")
 ##-- end logging
 
 make_missing = doot.config.on_fail(False).settings.general.location_check.make_missing()
 print_levels = doot.config.on_fail(TomlGuard(), TomlGuard).settings.general.location_check.print_levels(TomlGuard)
 
 @doot.check_protocol
 class CheckLocsTask(DootTask):
-    """ A Task for checking a single location exists """
+    """ A Task for checking a single location exists
+
+    """
     task_name = "_locations::check"
 
     def __init__(self, spec=None):
-        locations = [[doot.locs[f"{{{x}}}"]] for x in doot.locs]
-        spec      = DootTaskSpec.from_dict({
+        locations = [[doot.locs[f"{{{x}}}"]] for x in doot.locs if not doot.locs.metacheck(x, LocationMeta.file)]
+        spec      = DootTaskSpec.build({
             "name"         : CheckLocsTask.task_name,
             "actions"      : locations,
             "print_levels" : print_levels,
             "priority"     : 100,
                                            })
         super().__init__(spec, action_ctor=self.checklocs)
```

### Comparing `doot-0.6.1/doot/task/specialised_jobs.py` & `doot-0.7.0/doot/task/specialised_jobs.py`

 * *Files identical despite different names*

### Comparing `doot-0.6.1/doot/utils/check_protocol.py` & `doot-0.7.0/doot/utils/check_protocol.py`

 * *Files identical despite different names*

### Comparing `doot-0.6.1/doot/utils/log_colour.py` & `doot-0.7.0/doot/utils/log_colour.py`

 * *Files identical despite different names*

### Comparing `doot-0.6.1/doot/utils/log_config.py` & `doot-0.7.0/doot/utils/log_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,15 +30,14 @@
 ##-- logging
 logging = logmod.getLogger(__name__)
 ##-- end logging
 
 import os
 from sys import stdout, stderr
 import doot
-import doot.constants
 from doot.utils.log_colour import DootColourFormatter, DootColourStripFormatter
 
 env : dict = os.environ
 
 class _DootAnyFilter:
     """
 
@@ -57,56 +56,68 @@
 class DootLogConfig:
     """ Utility class to setup [stdout, stderr, file] logging. """
 
     def __init__(self):
         # Root Logger for everything
         self.root    = logmod.root
         # EXCEPT this, which replaces 'print(x)'
-        self.printer               = logmod.getLogger(doot.constants.PRINTER_NAME)
+        self.printer               = logmod.getLogger(doot.constants.printer.PRINTER_NAME)
 
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
+        # self.file_handler.setFormatter(DootColourStripFormatter(fmt="{levelname} : INIT : {message}"))
 
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
-        file_log_level    = doot.config.on_fail("DEBUG", str|int).logging.file.level(wrapper=lambda x: logmod._nameToLevel.get(x, 0))
-        file_log_format   = doot.config.on_fail("{levelname} : {pathname} : {lineno} : {funcName} : {message}", str).logging.file.format()
-        file_filter_names = doot.config.on_fail([], list).logging.file.allow()
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
+        file_log_level     = doot.config.on_fail("DEBUG", str|int).logging.file.level(wrapper=lambda x: logmod._nameToLevel.get(x, 0))
+        file_log_format    = doot.config.on_fail("{levelname} : {pathname} : {lineno} : {funcName} : {message}", str).logging.file.format()
+        file_filter_names  = doot.config.on_fail([], list).logging.file.allow()
 
         self.file_handler.setLevel(file_log_level)
         self.file_handler.setFormatter(DootColourStripFormatter(fmt=file_log_format))
         if bool(file_filter_names):
             self.file_handler.addFilter(_DootAnyFilter(file_filter_names))
 
+        self.root.addHandler(self.file_handler)
+
     def _setup_stream_logging(self):
         stream_log_level    = doot.config.on_fail("WARNING", str|int).logging.stream.level(wrapper=lambda x: logmod._nameToLevel.get(x, 0))
         stream_log_format   = doot.config.on_fail("{levelname} : {pathname} : {lineno} : {funcName} : {message}", str).logging.stream.format()
         stream_filter_names = doot.config.on_fail([], list).logging.stream.allow()
 
         self.stream_handler.setLevel(stream_log_level)
         use_colour = doot.config.on_fail(False, bool).logging.stream.colour()
```

### Comparing `doot-0.6.1/doot/utils/log_context.py` & `doot-0.7.0/doot/utils/log_context.py`

 * *Files identical despite different names*

### Comparing `doot-0.6.1/doot/utils/mock_gen.py` & `doot-0.7.0/doot/utils/mock_gen.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,15 +37,16 @@
 logging = logmod.getLogger(__name__)
 ##-- end logging
 
 from unittest.mock import PropertyMock, MagicMock, create_autospec
 from importlib.metadata import EntryPoint
 import tomlguard
 from doot import structs
-from doot._abstract import Task_i, Job_i, TaskBase_i, Command_i, TaskTracker_i, TaskRunner_i
+from doot.enums import TaskQueueMeta
+from doot._abstract import Task_i, Job_i, Command_i, TaskTracker_i, TaskRunner_i
 
 def _add_prop(m, name, val):
     setattr(type(m), name, PropertyMock(return_value=val))
 
 def task_network(tasks:dict):
     built = []
     for name, [pre, post] in tasks.items():
@@ -54,48 +55,47 @@
 
     return built
 
 
 
 def mock_task(name, spec=None, actions:int=1, **kwargs):
     task_m = MagicMock(spec=Task_i,
-                       depends_on=[],
-                       required_for=[],
                        name=name,
                        state={},
                        **kwargs)
     task_m.spec = spec or mock_task_spec(name=name, action_count=actions)
-    _add_prop(task_m, "name", name)
+    _add_prop(task_m, "name", structs.DootTaskName.build(name))
     _add_prop(task_m, "actions", task_m.spec.actions)
     return task_m
 
 def mock_job(name, pre=None, post=None, spec=None, **kwargs):
     task_m = MagicMock(spec=Job_i,
-                       depends_on=[],
-                       required_for=[],
                        name=name,
+                       state={},
                        **kwargs)
     _add_prop(task_m, "name", name)
     task_m.spec = spec or mock_task_spec(name=name)
     return task_m
 
 def mock_task_spec(name="mockSpec", pre=None, post=None, action_count=1, extra=None,  **kwargs):
     extra = extra or {}
     if "sleep" not in extra:
         extra['sleep'] = 0.1
     spec_m = MagicMock(structs.DootTaskSpec(name=name),
                        actions=mock_action_specs(num=action_count),
                        extra=tomlguard.TomlGuard(extra),
                        priority=10,
-                       queue_behaviour="default",
+                       queue_behaviour=TaskQueueMeta.default,
                        depends_on=pre or [],
                        required_for=post or [],
+                       setup=[],
+                       cleanup=[],
                        print_levels=tomlguard.TomlGuard({}),
-                        )
-    spec_m.name = name
+                       )
+    spec_m.name = structs.DootTaskName.build(name)
     return spec_m
 
 def mock_action_specs(num=1) -> list:
     results = []
     for x in range(num):
         action_spec_m = MagicMock(spec=structs.DootActionSpec(),
                                   args=[],
@@ -124,15 +124,15 @@
     m = MagicMock(spec=EntryPoint)
     _add_prop(m, "name", name)
     _add_prop(m, "value", name)
     m.load.return_value = value
     return m
 
 def mock_task_ctor(name="APretendClass", module="pretend", params=None):
-    mock_ctor = MagicMock(spec=TaskBase_i)
+    mock_ctor = MagicMock(spec=Task_i)
     _add_prop(mock_ctor, "name", name)
     _add_prop(mock_ctor, "param_specs", params or [])
     mock_ctor.__module__ = module
     mock_ctor.__name__   = name
     return mock_ctor
 
 def mock_code_ref(returns=None):
```

### Comparing `doot-0.6.1/doot/utils/plugin_selector.py` & `doot-0.7.0/doot/utils/plugin_selector.py`

 * *Files 8% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 def plugin_selector(plugins:TomlGuard, *, target="default", fallback=None) -> type:
     """ Selects and loads plugins from a tomlguard, based on a target,
     with an available fallback constructor """
     logging.debug("Selecting plugin for target: %s", target)
 
     if target != "default":
         try:
-            name = DootCodeReference.from_str(target)
+            name = DootCodeReference.build(target)
             return name.try_import()
         except ImportError as err:
             # raise doot.errors.DootInvalidConfig("Import Failed: %s : %s", target, err.msg) from err
             pass
         except (AttributeError, KeyError) as err:
             # raise doot.errors.DootInvalidConfig("Import Failed: Module has missing attritbue/key: %s", target) from err
             pass
```

### Comparing `doot-0.6.1/doot/utils/retrievers.py` & `doot-0.7.0/doot/utils/trace_helper.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,64 +1,68 @@
 #!/usr/bin/env python3
 """
 
-
-See EOF for license/metadata/notes as applicable
 """
-
-##-- builtin imports
+##-- imports
 from __future__ import annotations
 
 # import abc
-import datetime
-import enum
+# import datetime
+# import enum
 import functools as ftz
 import itertools as itz
 import logging as logmod
 import pathlib as pl
 import re
 import time
 import types
-import weakref
 # from copy import deepcopy
 # from dataclasses import InitVar, dataclass, field
 from typing import (TYPE_CHECKING, Any, Callable, ClassVar, Final, Generic,
                     Iterable, Iterator, Mapping, Match, MutableMapping,
                     Protocol, Sequence, Tuple, TypeAlias, TypeGuard, TypeVar,
-                    cast, final, overload, runtime_checkable, Generator)
-from uuid import UUID, uuid1
+                    cast, final, overload, runtime_checkable)
+# from uuid import UUID, uuid1
+# from weakref import ref
 
-##-- end builtin imports
-
-##-- lib imports
-import more_itertools as mitz
-##-- end lib imports
+##-- end imports
 
 ##-- logging
 logging = logmod.getLogger(__name__)
-printer = logmod.getLogger("doot._printer")
 ##-- end logging
 
-def id_retriever(spec, state) -> list[dict]:
-    """ A Null retriever, retruns to dicts to create subtasks from """
-    return []
-
-@DootKey.kwrap.types("files", "exts")
-def cli_retriever(spec, state, files, exts):
-    """ A CLI retriever, eg: for pre-commit.
-      gets the cli arg list "files", and makes a dict that can be used with
-      file processors like what walkers use, filtering by extension
-    """
-    root = doot.locs["."]
-    printer.info("CLI Retrieval Testing: %s", files)
-    for x in files:
-        fpath = doot.locs[x]
-        if fpath.suffix not in exts:
-            continue
-
-        lpath = fpath.relative_to(root)
-        yield dict(name=fpath.stem,
-                   fpath=fpath,
-                   fstem=fpath.stem,
-                   fname=fpath.name,
-                   lpath=lpath,
-                   pstem=fpath.parent.stem)
+class TraceHelper:
+
+    def __init__(self):
+        self.frames = []
+        self.get_frames()
+
+    def __getitem__(self, val=None):
+        match val:
+            case None:
+                return self.to_tb()
+            case slice() | int():
+                return self.to_tb(self.frames[val])
+            case _:
+                raise TypeError("Bad value passed to TraceHelper")
+
+    def get_frames(self):
+        """ from https://stackoverflow.com/questions/27138440 """
+        tb    = None
+        depth = 0
+        while True:
+            try:
+                frame = sys._getframe(depth)
+                depth += 1
+            except ValueError as exc:
+                break
+
+            self.frames.append(frame)
+
+    def to_tb(self, frames=None):
+        top = None
+        frames = frames or self.frames
+        for frame in frames:
+            top = types.TracebackType(top, frame,
+                                     frame.f_lasti,
+                                     frame.f_lineno)
+        return top
```

### Comparing `doot-0.6.1/doot/utils/signal_handler.py` & `doot-0.7.0/doot/utils/signal_handler.py`

 * *Files identical despite different names*

### Comparing `doot-0.6.1/doot/utils/testing_fixtures.py` & `doot-0.7.0/doot/utils/testing_fixtures.py`

 * *Files 19% similar despite different names*

```diff
@@ -40,13 +40,17 @@
     """ create a new temp directory, and change cwd to it,
       returning to original cwd after the test
       """
     logging.debug("Moving to temp dir")
     orig     = pl.Path().cwd()
     new_base = tmp_path / "test_root"
     new_base.mkdir()
-    os.chdir(new_base)
-    doot.locs._root = new_base
-    yield new_base
+    with doot.locs(new_base):
+        yield new_base
     logging.debug("Returning to original dir")
-    os.chdir(orig)
-    doot.locs._root = orig
+
+
+@pytest.fixture
+def wrap_locs():
+    logging.debug("Activating temp locs")
+    with doot.locs() as temp:
+        yield temp
```

### Comparing `doot-0.6.1/doot.egg-info/PKG-INFO` & `doot-0.7.0/doot.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doot
-Version: 0.6.1
+Version: 0.7.0
 Summary: An opinionated, TOML based task runner
 Author-email: jgrey <jgrey.n.plus.one@gmail.com>
 License:  ACAB License © 2022-12-09 John Grey
         
         
         To the maximum extent applicable by law, and any licenses of components of this work:
         
@@ -55,24 +55,27 @@
 Requires-Dist: networkx>3.0
 Requires-Dist: sh>=2.0.6
 Requires-Dist: stackprinter>=0.2.10
 Requires-Dist: matplotlib
 Requires-Dist: sty
 Requires-Dist: boltons
 Requires-Dist: more_itertools
+Requires-Dist: decorator-validation>=3.0.0
+Requires-Dist: decorator>=5.0.0
+Requires-Dist: jgdv
 Provides-Extra: test
 Requires-Dist: pytest<5.0.0; extra == "test"
 Requires-Dist: pytest-mock; extra == "test"
 Provides-Extra: dev
 Requires-Dist: pipreqs; extra == "dev"
 Requires-Dist: sphinx; extra == "dev"
 
 ![doot](https://github.com/jgrey4296/doot/assets/5943270/170a5631-6175-4d92-8d66-e26aa2c2e472)
 # doot
-Version : 0.6.1  
+Version : 0.7.0  
 Author  : John Grey  
 Date    : 2022-12-09  
 
 ## Overview
 This started out as an opinionated rewrite of the [doit](https://pydoit.org/contents.html) task runner.
 For other, more mature alternatives, see [Luigi](https://github.com/spotify/luigi), and [SnakeMake](https://github.com/snakemake/snakemake)
 and, of course, [GNU Make](https://www.gnu.org/software/make/).
```

### Comparing `doot-0.6.1/doot.egg-info/SOURCES.txt` & `doot-0.7.0/doot.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,99 +1,111 @@
 LICENSE
 README.md
 pyproject.toml
 doot/__init__.py
 doot/__main__.py
-doot/_default_plugins.py
-doot/constants.py
 doot/enums.py
 doot/errors.py
 doot/structs.py
 doot.egg-info/PKG-INFO
 doot.egg-info/SOURCES.txt
 doot.egg-info/dependency_links.txt
 doot.egg-info/entry_points.txt
 doot.egg-info/requires.txt
 doot.egg-info/top_level.txt
+doot/__data/aliases.toml
+doot/__data/constants.toml
 doot/__templates/basic_toml
 doot/__templates/stub_task_py
 doot/__templates/tasks_toml
 doot/__tests/test_basic.py
 doot/__tests/test_inits.py
 doot/_abstract/__init__.py
 doot/_abstract/cmd.py
 doot/_abstract/control.py
 doot/_abstract/dbm.py
 doot/_abstract/loader.py
 doot/_abstract/overlord.py
 doot/_abstract/parser.py
 doot/_abstract/policy.py
 doot/_abstract/reporter.py
+doot/_abstract/structs.py
 doot/_abstract/task.py
 doot/_structs/__init__.py
 doot/_structs/action_spec.py
 doot/_structs/artifact.py
 doot/_structs/code_ref.py
 doot/_structs/key.py
+doot/_structs/log.doot
 doot/_structs/param_spec.py
 doot/_structs/sname.py
 doot/_structs/structured_name.py
 doot/_structs/stub.py
 doot/_structs/task_name.py
 doot/_structs/task_spec.py
+doot/_structs/toml_loc.py
 doot/_structs/trace.py
 doot/_structs/__tests/test_action_spec.py
 doot/_structs/__tests/test_artifact.py
+doot/_structs/__tests/test_code_ref.py
 doot/_structs/__tests/test_formatter.py
 doot/_structs/__tests/test_key.py
+doot/_structs/__tests/test_key_decorators.py
+doot/_structs/__tests/test_key_multi.py
+doot/_structs/__tests/test_key_path_expansion.py
+doot/_structs/__tests/test_key_string_expansion.py
+doot/_structs/__tests/test_key_type_expansion.py
 doot/_structs/__tests/test_param_spec.py
-doot/_structs/__tests/test_sname.py
 doot/_structs/__tests/test_stub.py
+doot/_structs/__tests/test_task_name.py
 doot/_structs/__tests/test_task_spec.py
 doot/actions/__init__.py
 doot/actions/base_action.py
 doot/actions/compression.py
 doot/actions/control_flow.py
 doot/actions/io.py
+doot/actions/job_actions.py
+doot/actions/job_expansion.py
+doot/actions/job_injection.py
+doot/actions/job_queuing.py
 doot/actions/json.py
 doot/actions/postbox.py
 doot/actions/shell.py
 doot/actions/speak.py
 doot/actions/state.py
 doot/actions/templater.py
 doot/actions/util.py
 doot/actions/__tests/test_base_action.py
 doot/actions/__tests/test_control_flow.py
 doot/actions/__tests/test_io.py
+doot/actions/__tests/test_job_actions.py
+doot/actions/__tests/test_job_expansion.py
+doot/actions/__tests/test_job_injection.py
+doot/actions/__tests/test_job_queuing.py
 doot/actions/__tests/test_postbox.py
 doot/actions/__tests/test_shell.py
 doot/actions/__tests/test_state.py
 doot/cmds/__init__.py
+doot/cmds/base_cmd.py
 doot/cmds/clean_cmd.py
-doot/cmds/complete_cmd.py
-doot/cmds/daemon_cmd.py
 doot/cmds/graph_cmd.py
 doot/cmds/help_cmd.py
-doot/cmds/here_cmd.py
-doot/cmds/last_cmd.py
 doot/cmds/list_cmd.py
 doot/cmds/locs_cmd.py
 doot/cmds/plugins_cmd.py
 doot/cmds/run_cmd.py
-doot/cmds/server_cmd.py
 doot/cmds/step_cmd.py
 doot/cmds/stub_cmd.py
 doot/cmds/__tests/test_list_cmd.py
 doot/control/__init__.py
 doot/control/base_runner.py
 doot/control/base_tracker.py
-doot/control/date_tracker.py
 doot/control/locations.py
+doot/control/log.doot
 doot/control/overlord.py
-doot/control/policy.py
 doot/control/runner.py
 doot/control/step_runner.py
 doot/control/tracker.py
 doot/control/__tests/test_locations.py
 doot/control/__tests/test_overlord.py
 doot/control/__tests/test_runner.py
 doot/control/__tests/test_tracker.py
@@ -101,59 +113,46 @@
 doot/loaders/cmd_loader.py
 doot/loaders/plugin_loader.py
 doot/loaders/task_loader.py
 doot/loaders/__tests/test_cmd_loader.py
 doot/loaders/__tests/test_plugin_loader.py
 doot/loaders/__tests/test_task_loader.py
 doot/mixins/__init__.py
+doot/mixins/enums.py
+doot/mixins/fail_handler.py
+doot/mixins/human_numbers.py
 doot/mixins/importer.py
-doot/mixins/action/__init__.py
-doot/mixins/action/batch.py
-doot/mixins/action/cleaning.py
-doot/mixins/action/human_numbers.py
-doot/mixins/action/zipper.py
-doot/mixins/job/expander.py
-doot/mixins/job/limiter.py
-doot/mixins/job/matcher.py
-doot/mixins/job/setup.py
-doot/mixins/job/shadower.py
-doot/mixins/job/subtask.py
-doot/mixins/job/terse.py
-doot/mixins/job/__tests/test_expander.py
-doot/mixins/job/__tests/test_limiter.py
-doot/mixins/job/__tests/test_matcher.py
-doot/mixins/job/__tests/test_shadower.py
-doot/mixins/job/__tests/test_subtask.py
-doot/mixins/job/__tests/test_terse.py
-doot/mixins/runner/__init__.py
-doot/mixins/runner/fail_handler.py
-doot/mixins/task/__init__.py
+doot/mixins/param_spec.py
+doot/mixins/path_manip.py
+doot/mixins/zipper.py
 doot/parsers/__init__.py
 doot/parsers/flexible.py
 doot/parsers/__tests/test_flexible.py
 doot/reporters/__init__.py
 doot/reporters/basic_reporters.py
 doot/reporters/stack_manager.py
 doot/reporters/summary_manager.py
 doot/reporters/__tests/test_stack_manager.py
 doot/reporters/__tests/test_summary_manager.py
 doot/task/__init__.py
 doot/task/base_job.py
 doot/task/base_task.py
 doot/task/check_locs.py
-doot/task/dev_scaffold.py
 doot/task/specialised_jobs.py
 doot/task/__tests/test_base_job.py
 doot/task/__tests/test_base_task.py
 doot/task/__tests/test_check_locs.py
 doot/utils/__init__.py
+doot/utils/chain_get.py
 doot/utils/check_protocol.py
+doot/utils/decorators.py
 doot/utils/log_colour.py
 doot/utils/log_config.py
 doot/utils/log_context.py
 doot/utils/mock_gen.py
 doot/utils/plugin_selector.py
 doot/utils/retrievers.py
 doot/utils/signal_handler.py
 doot/utils/testing_fixtures.py
 doot/utils/trace_helper.py
-doot/utils/url_expand.py
+doot/utils/url_expand.py
+doot/utils/__tests/test_decorators.py
```

### Comparing `doot-0.6.1/pyproject.toml` & `doot-0.7.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name            = "doot"
-version         = "0.6.1"
+version         = "0.7.0"
 description     = "An opinionated, TOML based task runner"
 readme          = "README.md"
 requires-python = ">=3.11"
 license         = {file = "LICENSE"}
 keywords        = ["toml","taskrunner"]
 authors         = [
   {email = "jgrey.n.plus.one@gmail.com", name  = "jgrey"}
@@ -20,15 +20,18 @@
     "tomlguard",
     "networkx > 3.0",
     "sh >= 2.0.6",
     "stackprinter >= 0.2.10",
     "matplotlib",
     "sty",
     "boltons",
-    "more_itertools"
+    "more_itertools",
+    "decorator-validation >= 3.0.0",
+    "decorator >= 5.0.0",
+    "jgdv",
 ]
 
 [project.optional-dependencies]
 test = [
   "pytest < 5.0.0",
   "pytest-mock",
 ]
@@ -83,15 +86,15 @@
 log_cli_level = "INFO"
 log_format    = "%(levelname)s %(name)s : %(message)s"
 
 ##-- end pytest
 
 ##-- bumpver
 [tool.bumpver]
-current_version    = "0.6.1"
+current_version    = "0.7.0"
 version_pattern    = "MAJOR.MINOR.PATCH"
 commit_message     = "[bump]: version {old_version} -> {new_version}"
 tag_message        = "{new_version}"
 tag_scope          = "default"
 commit             = true
 tag                = true
 # push             = true
```

