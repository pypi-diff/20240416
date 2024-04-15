# Comparing `tmp/parsl-2024.4.15.tar.gz` & `tmp/parsl-2024.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parsl-2024.4.15.tar", last modified: Mon Apr 15 22:42:46 2024, max compression
+gzip compressed data, was "parsl-2024.4.8.tar", last modified: Mon Apr  8 22:42:43 2024, max compression
```

## Comparing `parsl-2024.4.15.tar` & `parsl-2024.4.8.tar`

### file list

```diff
@@ -1,536 +1,533 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:46.476878 parsl-2024.4.15/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-15 22:42:43.000000 parsl-2024.4.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-15 22:42:43.000000 parsl-2024.4.15/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-04-15 22:42:46.476878 parsl-2024.4.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4869 2024-04-15 22:42:43.000000 parsl-2024.4.15/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:46.412876 parsl-2024.4.15/parsl/
--rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4819 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/addresses.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:46.416876 parsl-2024.4.15/parsl/app/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8522 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/app/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     5396 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/app/bash.py
--rw-r--r--   0 runner    (1001) docker     (127)     4039 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/app/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/app/futures.py
--rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/app/python.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:46.416876 parsl-2024.4.15/parsl/benchmark/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/benchmark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/benchmark/perf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:46.416876 parsl-2024.4.15/parsl/channels/
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/channels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4294 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/channels/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3282 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/channels/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:46.416876 parsl-2024.4.15/parsl/channels/local/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/channels/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5087 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/channels/local/local.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:46.416876 parsl-2024.4.15/parsl/channels/oauth_ssh/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/channels/oauth_ssh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/channels/oauth_ssh/oauth_ssh.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:46.416876 parsl-2024.4.15/parsl/channels/ssh/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/channels/ssh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9477 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/channels/ssh/ssh.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:46.416876 parsl-2024.4.15/parsl/channels/ssh_il/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/channels/ssh_il/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/channels/ssh_il/ssh_il.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:46.416876 parsl-2024.4.15/parsl/concurrent/
--rw-r--r--   0 runner    (1001) docker     (127)     3288 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/concurrent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7038 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:46.420876 parsl-2024.4.15/parsl/configs/
--rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/configs/ASPIRE1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/configs/Azure.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/configs/ad_hoc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/configs/bridges.py
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/configs/cc_in2p3.py
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/configs/ec2.py
--rw-r--r--   0 runner    (1001) docker     (127)      957 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/configs/expanse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/configs/frontera.py
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/configs/htex_local.py
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/configs/illinoiscluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/configs/kubernetes.py
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/configs/local_threads.py
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/configs/midway.py
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/configs/osg.py
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/configs/polaris.py
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/configs/stampede2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/configs/summit.py
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/configs/toss3_llnl.py
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/configs/vineex_local.py
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/configs/wqex_local.py
--rw-r--r--   0 runner    (1001) docker     (127)     6939 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/curvezmq.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:46.420876 parsl-2024.4.15/parsl/data_provider/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/data_provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7319 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/data_provider/data_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/data_provider/file_noop.py
--rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/data_provider/files.py
--rw-r--r--   0 runner    (1001) docker     (127)     2759 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/data_provider/ftp.py
--rw-r--r--   0 runner    (1001) docker     (127)    12012 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/data_provider/globus.py
--rw-r--r--   0 runner    (1001) docker     (127)     2986 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/data_provider/http.py
--rw-r--r--   0 runner    (1001) docker     (127)     4254 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/data_provider/rsync.py
--rw-r--r--   0 runner    (1001) docker     (127)     4523 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/data_provider/staging.py
--rw-r--r--   0 runner    (1001) docker     (127)     3348 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/data_provider/zip.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:46.424877 parsl-2024.4.15/parsl/dataflow/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/dataflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    63830 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/dataflow/dflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/dataflow/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     5059 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/dataflow/futures.py
--rw-r--r--   0 runner    (1001) docker     (127)     9583 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/dataflow/memoization.py
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/dataflow/rundirs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/dataflow/states.py
--rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/dataflow/taskrecord.py
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:46.424877 parsl-2024.4.15/parsl/executors/
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/executors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4619 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/executors/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/executors/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:46.424877 parsl-2024.4.15/parsl/executors/flux/
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/executors/flux/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/executors/flux/execute_parsl_task.py
--rw-r--r--   0 runner    (1001) docker     (127)    16978 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/executors/flux/executor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/executors/flux/flux_instance_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:46.424877 parsl-2024.4.15/parsl/executors/high_throughput/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/executors/high_throughput/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/executors/high_throughput/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    37124 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/executors/high_throughput/executor.py
--rw-r--r--   0 runner    (1001) docker     (127)    31491 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/executors/high_throughput/interchange.py
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/executors/high_throughput/manager_record.py
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/executors/high_throughput/monitoring_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     4273 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/executors/high_throughput/mpi_prefix_composer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7975 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/executors/high_throughput/mpi_resource_management.py
--rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/executors/high_throughput/probe.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    41267 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/executors/high_throughput/process_worker_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)     6514 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/executors/high_throughput/zmq_pipes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:46.428877 parsl-2024.4.15/parsl/executors/radical/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/executors/radical/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21024 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/executors/radical/executor.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1368 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/executors/radical/rpex_master.py
--rw-r--r--   0 runner    (1001) docker     (127)     4960 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/executors/radical/rpex_resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     1868 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/executors/radical/rpex_worker.py
--rw-r--r--   0 runner    (1001) docker     (127)    13631 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/executors/status_handling.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:46.428877 parsl-2024.4.15/parsl/executors/taskvine/
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/executors/taskvine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/executors/taskvine/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     7085 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/executors/taskvine/exec_parsl_function.py
--rw-r--r--   0 runner    (1001) docker     (127)    32807 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/executors/taskvine/executor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/executors/taskvine/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     3693 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/executors/taskvine/factory_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    25822 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/executors/taskvine/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     7457 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/executors/taskvine/manager_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4156 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/executors/taskvine/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3353 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/executors/threads.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:46.428877 parsl-2024.4.15/parsl/executors/workqueue/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/executors/workqueue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/executors/workqueue/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     7801 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/executors/workqueue/exec_parsl_function.py
--rw-r--r--   0 runner    (1001) docker     (127)    50317 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/executors/workqueue/executor.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5737 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/executors/workqueue/parsl_coprocess.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      735 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/executors/workqueue/parsl_coprocess_stub.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:46.428877 parsl-2024.4.15/parsl/jobs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/jobs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/jobs/error_handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/jobs/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/jobs/job_status_poller.py
--rw-r--r--   0 runner    (1001) docker     (127)     4855 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/jobs/states.py
--rw-r--r--   0 runner    (1001) docker     (127)    13799 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/jobs/strategy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:46.432877 parsl-2024.4.15/parsl/launchers/
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/launchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/launchers/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/launchers/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    15464 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/launchers/launchers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3274 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/log_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:46.432877 parsl-2024.4.15/parsl/monitoring/
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/monitoring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    37021 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/monitoring/db_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/monitoring/message_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    12862 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/monitoring/monitoring.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:46.432877 parsl-2024.4.15/parsl/monitoring/queries/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/monitoring/queries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/monitoring/queries/pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)     5858 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/monitoring/radios.py
--rw-r--r--   0 runner    (1001) docker     (127)    13923 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/monitoring/remote.py
--rw-r--r--   0 runner    (1001) docker     (127)     9557 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/monitoring/router.py
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/monitoring/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:46.432877 parsl-2024.4.15/parsl/monitoring/visualization/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/monitoring/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/monitoring/visualization/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     5139 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/monitoring/visualization/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:46.432877 parsl-2024.4.15/parsl/monitoring/visualization/plots/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/monitoring/visualization/plots/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:46.432877 parsl-2024.4.15/parsl/monitoring/visualization/plots/default/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/monitoring/visualization/plots/default/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/monitoring/visualization/plots/default/task_plots.py
--rw-r--r--   0 runner    (1001) docker     (127)    11985 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/monitoring/visualization/plots/default/workflow_plots.py
--rw-r--r--   0 runner    (1001) docker     (127)    10269 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/monitoring/visualization/plots/default/workflow_resource_plots.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:46.432877 parsl-2024.4.15/parsl/monitoring/visualization/static/
--rwxr-xr-x   0 runner    (1001) docker     (127)    14199 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/monitoring/visualization/static/parsl-logo-white.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      337 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/monitoring/visualization/static/parsl-monitor.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:46.436877 parsl-2024.4.15/parsl/monitoring/visualization/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/monitoring/visualization/templates/app.html
--rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/monitoring/visualization/templates/dag.html
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/monitoring/visualization/templates/error.html
--rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/monitoring/visualization/templates/layout.html
--rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/monitoring/visualization/templates/resource_usage.html
--rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/monitoring/visualization/templates/task.html
--rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/monitoring/visualization/templates/workflow.html
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/monitoring/visualization/templates/workflows_summary.html
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/monitoring/visualization/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/monitoring/visualization/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     8256 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/monitoring/visualization/views.py
--rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/multiprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/process_loggers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:46.436877 parsl-2024.4.15/parsl/providers/
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/providers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:46.436877 parsl-2024.4.15/parsl/providers/ad_hoc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/providers/ad_hoc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8302 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/providers/ad_hoc/ad_hoc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:46.436877 parsl-2024.4.15/parsl/providers/aws/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/providers/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29009 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/providers/aws/aws.py
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/providers/aws/template.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:46.436877 parsl-2024.4.15/parsl/providers/azure/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/providers/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18396 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/providers/azure/azure.py
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/providers/azure/template.py
--rw-r--r--   0 runner    (1001) docker     (127)     5702 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/providers/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4668 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/providers/cluster_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:46.436877 parsl-2024.4.15/parsl/providers/cobalt/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/providers/cobalt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8478 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/providers/cobalt/cobalt.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      273 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/providers/cobalt/template.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:46.436877 parsl-2024.4.15/parsl/providers/condor/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/providers/condor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13175 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/providers/condor/condor.py
--rw-r--r--   0 runner    (1001) docker     (127)      960 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/providers/condor/template.py
--rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/providers/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:46.436877 parsl-2024.4.15/parsl/providers/googlecloud/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/providers/googlecloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8006 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/providers/googlecloud/googlecloud.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:46.440877 parsl-2024.4.15/parsl/providers/grid_engine/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/providers/grid_engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8565 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/providers/grid_engine/grid_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/providers/grid_engine/template.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:46.440877 parsl-2024.4.15/parsl/providers/kubernetes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/providers/kubernetes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12819 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/providers/kubernetes/kube.py
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/providers/kubernetes/template.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:46.440877 parsl-2024.4.15/parsl/providers/local/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/providers/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11372 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/providers/local/local.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:46.440877 parsl-2024.4.15/parsl/providers/lsf/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/providers/lsf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11502 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/providers/lsf/lsf.py
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/providers/lsf/template.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:46.440877 parsl-2024.4.15/parsl/providers/pbspro/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/providers/pbspro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8822 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/providers/pbspro/pbspro.py
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/providers/pbspro/template.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:46.440877 parsl-2024.4.15/parsl/providers/slurm/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/providers/slurm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13916 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/providers/slurm/slurm.py
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/providers/slurm/template.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:46.440877 parsl-2024.4.15/parsl/providers/torque/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/providers/torque/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/providers/torque/template.py
--rw-r--r--   0 runner    (1001) docker     (127)     9497 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/providers/torque/torque.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:46.440877 parsl-2024.4.15/parsl/serialize/
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/serialize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/serialize/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/serialize/concretes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/serialize/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     6795 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/serialize/facade.py
--rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/serialize/proxystore.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:46.444877 parsl-2024.4.15/parsl/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/callables_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:46.448877 parsl-2024.4.15/parsl/tests/configs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/configs/ad_hoc_cluster_htex.py
--rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/configs/azure_single_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/configs/bluewaters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/configs/bridges.py
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/configs/cc_in2p3.py
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/configs/comet.py
--rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/configs/cooley_htex.py
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/configs/ec2_single_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/configs/ec2_spot.py
--rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/configs/frontera.py
--rw-r--r--   0 runner    (1001) docker     (127)      946 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/configs/htex_ad_hoc_cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/configs/htex_local.py
--rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/configs/htex_local_alternate.py
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/configs/htex_local_intask_staging.py
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/configs/htex_local_rsync_staging.py
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/configs/local_adhoc.py
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/configs/local_radical.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/configs/local_radical_mpi.py
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/configs/local_threads.py
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/configs/local_threads_checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/configs/local_threads_checkpoint_dfk_exit.py
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/configs/local_threads_checkpoint_periodic.py
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/configs/local_threads_checkpoint_task_exit.py
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/configs/local_threads_ftp_in_task.py
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/configs/local_threads_globus.py
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/configs/local_threads_http_in_task.py
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/configs/local_threads_monitoring.py
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/configs/local_threads_no_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/configs/midway.py
--rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/configs/nscc_singapore.py
--rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/configs/osg_htex.py
--rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/configs/petrelkube.py
--rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/configs/summit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/configs/swan_htex.py
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/configs/taskvine_ex.py
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/configs/theta.py
--rw-r--r--   0 runner    (1001) docker     (127)     6265 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/configs/user_opts.py
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/configs/workqueue_ex.py
--rw-r--r--   0 runner    (1001) docker     (127)    14284 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:46.448877 parsl-2024.4.15/parsl/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/integration/latency.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:46.448877 parsl-2024.4.15/parsl/tests/integration/test_apps/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/integration/test_apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:46.452877 parsl-2024.4.15/parsl/tests/integration/test_channels/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/integration/test_channels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/integration/test_channels/test_channels.py
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/integration/test_channels/test_local_channel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/integration/test_channels/test_scp_1.py
--rw-r--r--   0 runner    (1001) docker     (127)      933 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/integration/test_channels/test_ssh_1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/integration/test_channels/test_ssh_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/integration/test_channels/test_ssh_file_transport.py
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/integration/test_channels/test_ssh_interactive.py
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/integration/test_parsl_load_default_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:46.452877 parsl-2024.4.15/parsl/tests/integration/test_stress/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/integration/test_stress/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/integration/test_stress/test_python_simple.py
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/integration/test_stress/test_python_threads.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:46.452877 parsl-2024.4.15/parsl/tests/manual_tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/manual_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      820 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/manual_tests/htex_local.py
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/manual_tests/test_ad_hoc_htex.py
--rw-r--r--   0 runner    (1001) docker     (127)     4022 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/manual_tests/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/manual_tests/test_fan_in_out_htex_remote.py
--rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/manual_tests/test_log_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/manual_tests/test_memory_limits.py
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/manual_tests/test_oauth_ssh.py
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/manual_tests/test_regression_220.py
--rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/manual_tests/test_udp_simple.py
--rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/manual_tests/test_worker_count.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:46.452877 parsl-2024.4.15/parsl/tests/scaling_tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/scaling_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/scaling_tests/htex_local.py
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/scaling_tests/local_threads.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3751 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/scaling_tests/test_scale.py
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/scaling_tests/vineex_condor.py
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/scaling_tests/vineex_local.py
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/scaling_tests/wqex_condor.py
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/scaling_tests/wqex_local.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:46.452877 parsl-2024.4.15/parsl/tests/site_tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/site_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/site_tests/site_config_selector.py
--rw-r--r--   0 runner    (1001) docker     (127)     2694 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/site_tests/test_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/site_tests/test_site.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:46.456877 parsl-2024.4.15/parsl/tests/sites/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/sites/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/sites/test_affinity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/sites/test_concurrent.py
--rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/sites/test_dynamic_executor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/sites/test_ec2.py
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/sites/test_launchers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/sites/test_local_adhoc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:46.456877 parsl-2024.4.15/parsl/tests/sites/test_mpi/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/sites/test_mpi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/sites/test_worker_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     9615 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_aalst_patterns.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:46.456877 parsl-2024.4.15/parsl/tests/test_bash_apps/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_bash_apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_bash_apps/test_apptimeout.py
--rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_bash_apps/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (127)     3964 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_bash_apps/test_error_codes.py
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_bash_apps/test_keyword_overlaps.py
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_bash_apps/test_kwarg_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_bash_apps/test_memoize.py
--rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_bash_apps/test_memoize_ignore_args.py
--rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_bash_apps/test_memoize_ignore_args_regr.py
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_bash_apps/test_multiline.py
--rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_bash_apps/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     2787 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_bash_apps/test_stdout.py
--rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_callables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:46.456877 parsl-2024.4.15/parsl/tests/test_channels/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_channels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_channels/test_large_output.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:46.460877 parsl-2024.4.15/parsl/tests/test_checkpointing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_checkpointing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_checkpointing/test_periodic.py
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_checkpointing/test_python_checkpoint_1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_checkpointing/test_python_checkpoint_2.py
--rw-r--r--   0 runner    (1001) docker     (127)      823 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_checkpointing/test_python_checkpoint_3.py
--rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_checkpointing/test_regression_232.py
--rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_checkpointing/test_regression_233.py
--rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_checkpointing/test_regression_239.py
--rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_checkpointing/test_task_exit.py
--rw-r--r--   0 runner    (1001) docker     (127)    12431 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_curvezmq.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:46.460877 parsl-2024.4.15/parsl/tests/test_docs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_docs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_docs/test_from_slides.py
--rw-r--r--   0 runner    (1001) docker     (127)      925 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_docs/test_kwargs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_docs/test_tutorial_1.py
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_docs/test_workflow1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_docs/test_workflow2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_docs/test_workflow4.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:46.460877 parsl-2024.4.15/parsl/tests/test_error_handling/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_error_handling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_error_handling/test_fail.py
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_error_handling/test_python_walltime.py
--rw-r--r--   0 runner    (1001) docker     (127)     3864 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_error_handling/test_rand_fail.py
--rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_error_handling/test_resource_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2445 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_error_handling/test_retries.py
--rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_error_handling/test_retry_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_error_handling/test_retry_handler_failure.py
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_error_handling/test_serialization_fail.py
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_error_handling/test_wrap_with_logs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:46.460877 parsl-2024.4.15/parsl/tests/test_flowcontrol/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_flowcontrol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5098 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_flux.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:46.464877 parsl-2024.4.15/parsl/tests/test_htex/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_htex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_htex/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_htex/test_connected_blocks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_htex/test_cpu_affinity_explicit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_htex/test_disconnected_blocks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_htex/test_drain.py
--rw-r--r--   0 runner    (1001) docker     (127)     3896 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_htex/test_htex.py
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_htex/test_manager_failure.py
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_htex/test_missing_worker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_htex/test_multiple_disconnected_blocks.py
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_htex/test_worker_failure.py
--rw-r--r--   0 runner    (1001) docker     (127)     2937 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_htex/test_zmq_binding.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:46.464877 parsl-2024.4.15/parsl/tests/test_monitoring/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_monitoring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_monitoring/test_app_names.py
--rw-r--r--   0 runner    (1001) docker     (127)     3768 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_monitoring/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_monitoring/test_db_locks.py
--rw-r--r--   0 runner    (1001) docker     (127)     3429 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_monitoring/test_fuzz_zmq.py
--rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_monitoring/test_htex_init_blocks_vs_monitoring.py
--rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_monitoring/test_incomplete_futures.py
--rw-r--r--   0 runner    (1001) docker     (127)     2660 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_monitoring/test_memoization_representation.py
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_monitoring/test_viz_colouring.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:46.464877 parsl-2024.4.15/parsl/tests/test_mpi_apps/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_mpi_apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_mpi_apps/test_bad_mpi_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_mpi_apps/test_mpi_mode_disabled.py
--rw-r--r--   0 runner    (1001) docker     (127)     5034 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_mpi_apps/test_mpi_mode_enabled.py
--rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_mpi_apps/test_mpi_prefix.py
--rw-r--r--   0 runner    (1001) docker     (127)     6317 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_mpi_apps/test_mpi_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3710 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_mpi_apps/test_resource_spec.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:46.464877 parsl-2024.4.15/parsl/tests/test_providers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_providers/test_cobalt_deprecation_warning.py
--rw-r--r--   0 runner    (1001) docker     (127)     6968 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_providers/test_local_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_providers/test_pbspro_template.py
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_providers/test_slurm_instantiate.py
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_providers/test_slurm_template.py
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_providers/test_submiterror_deprecation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:46.468877 parsl-2024.4.15/parsl/tests/test_python_apps/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_python_apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_python_apps/test_arg_input_types.py
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_python_apps/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_python_apps/test_context_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_python_apps/test_dep_standard_futures.py
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_python_apps/test_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_python_apps/test_depfail_propagation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_python_apps/test_fail.py
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_python_apps/test_fibonacci_iterative.py
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_python_apps/test_fibonacci_recursive.py
--rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_python_apps/test_futures.py
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_python_apps/test_garbage_collect.py
--rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_python_apps/test_import_fail.py
--rw-r--r--   0 runner    (1001) docker     (127)     2679 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_python_apps/test_join.py
--rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_python_apps/test_lifted.py
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_python_apps/test_mapred.py
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_python_apps/test_memoize_1.py
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_python_apps/test_memoize_2.py
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_python_apps/test_memoize_4.py
--rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_python_apps/test_memoize_bad_id_for_memo.py
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_python_apps/test_memoize_ignore_args.py
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_python_apps/test_memoize_joinapp.py
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_python_apps/test_outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_python_apps/test_overview.py
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_python_apps/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_python_apps/test_simple.py
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_python_apps/test_timeout.py
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_python_apps/test_type5.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:46.468877 parsl-2024.4.15/parsl/tests/test_radical/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_radical/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_radical/test_mpi_funcs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:46.472878 parsl-2024.4.15/parsl/tests/test_regression/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_regression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_regression/test_1480.py
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_regression/test_1606_wait_for_current_tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_regression/test_1653.py
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_regression/test_221.py
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_regression/test_226.py
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_regression/test_2652.py
--rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_regression/test_69a.py
--rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_regression/test_854.py
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_regression/test_97_parallelism_0.py
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_regression/test_98.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:46.472878 parsl-2024.4.15/parsl/tests/test_scaling/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_scaling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6050 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_scaling/test_block_error_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_scaling/test_regression_1621.py
--rw-r--r--   0 runner    (1001) docker     (127)     2821 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_scaling/test_scale_down.py
--rw-r--r--   0 runner    (1001) docker     (127)     4597 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_scaling/test_scale_down_htex_auto_scale.py
--rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_scaling/test_scale_down_htex_unregistered.py
--rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_scaling/test_shutdown_scalein.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:46.472878 parsl-2024.4.15/parsl/tests/test_serialization/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_serialization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_serialization/test_2555_caching_deserializer.py
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_serialization/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_serialization/test_htex_code_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_serialization/test_pack_resource_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_serialization/test_proxystore_configured.py
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_serialization/test_proxystore_impl.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:46.472878 parsl-2024.4.15/parsl/tests/test_shutdown/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_shutdown/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_shutdown/test_kill_monitoring.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:46.476878 parsl-2024.4.15/parsl/tests/test_staging/
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_staging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_staging/staging_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     2687 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_staging/test_1316.py
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_staging/test_docs_1.py
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_staging/test_docs_2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_staging/test_elaborate_noop_file.py
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_staging/test_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_staging/test_file_apps.py
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_staging/test_file_staging.py
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_staging/test_output_chain_filenames.py
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_staging/test_staging_ftp.py
--rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_staging/test_staging_ftp_in_task.py
--rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_staging/test_staging_globus.py
--rw-r--r--   0 runner    (1001) docker     (127)     3307 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_staging/test_staging_https.py
--rw-r--r--   0 runner    (1001) docker     (127)     3512 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_staging/test_zip_out.py
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_summary.py
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_thread_parallelism.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:46.476878 parsl-2024.4.15/parsl/tests/test_threads/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_threads/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      909 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_threads/test_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_threads/test_lazy_errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:46.476878 parsl-2024.4.15/parsl/tests/test_utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/test_utils/test_representation_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/tests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:46.476878 parsl-2024.4.15/parsl/usage_tracking/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/usage_tracking/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6684 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/usage_tracking/usage.py
--rw-r--r--   0 runner    (1001) docker     (127)    10979 2024-04-15 22:42:43.000000 parsl-2024.4.15/parsl/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-15 22:42:45.000000 parsl-2024.4.15/parsl/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:46.412876 parsl-2024.4.15/parsl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-04-15 22:42:46.000000 parsl-2024.4.15/parsl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    18086 2024-04-15 22:42:46.000000 parsl-2024.4.15/parsl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 22:42:46.000000 parsl-2024.4.15/parsl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-15 22:42:46.000000 parsl-2024.4.15/parsl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-15 22:42:46.000000 parsl-2024.4.15/parsl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-15 22:42:46.000000 parsl-2024.4.15/parsl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-15 22:42:43.000000 parsl-2024.4.15/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 22:42:46.476878 parsl-2024.4.15/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     2874 2024-04-15 22:42:43.000000 parsl-2024.4.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.329331 parsl-2024.4.8/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-08 22:42:39.000000 parsl-2024.4.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-08 22:42:39.000000 parsl-2024.4.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-04-08 22:42:43.329331 parsl-2024.4.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4869 2024-04-08 22:42:39.000000 parsl-2024.4.8/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.277331 parsl-2024.4.8/parsl/
+-rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4819 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/addresses.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.277331 parsl-2024.4.8/parsl/app/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8522 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/app/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5396 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/app/bash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4039 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/app/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/app/futures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/app/python.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.277331 parsl-2024.4.8/parsl/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/benchmark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/benchmark/perf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.277331 parsl-2024.4.8/parsl/channels/
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/channels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4294 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/channels/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3282 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/channels/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.277331 parsl-2024.4.8/parsl/channels/local/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/channels/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5087 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/channels/local/local.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.277331 parsl-2024.4.8/parsl/channels/oauth_ssh/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/channels/oauth_ssh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/channels/oauth_ssh/oauth_ssh.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.281331 parsl-2024.4.8/parsl/channels/ssh/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/channels/ssh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9477 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/channels/ssh/ssh.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.281331 parsl-2024.4.8/parsl/channels/ssh_il/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/channels/ssh_il/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/channels/ssh_il/ssh_il.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.281331 parsl-2024.4.8/parsl/concurrent/
+-rw-r--r--   0 runner    (1001) docker     (127)     3288 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/concurrent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7038 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.281331 parsl-2024.4.8/parsl/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/configs/ASPIRE1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/configs/Azure.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/configs/ad_hoc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/configs/bridges.py
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/configs/cc_in2p3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/configs/ec2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/configs/expanse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/configs/frontera.py
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/configs/htex_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/configs/illinoiscluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/configs/kubernetes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/configs/local_threads.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/configs/midway.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/configs/osg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/configs/polaris.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/configs/stampede2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/configs/summit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/configs/toss3_llnl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/configs/vineex_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/configs/wqex_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6939 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/curvezmq.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.281331 parsl-2024.4.8/parsl/data_provider/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/data_provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7250 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/data_provider/data_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/data_provider/file_noop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/data_provider/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2759 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/data_provider/ftp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12012 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/data_provider/globus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2986 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/data_provider/http.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4254 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/data_provider/rsync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4523 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/data_provider/staging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.285331 parsl-2024.4.8/parsl/dataflow/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/dataflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63254 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/dataflow/dflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/dataflow/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5256 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/dataflow/futures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9583 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/dataflow/memoization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/dataflow/rundirs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/dataflow/states.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/dataflow/taskrecord.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.285331 parsl-2024.4.8/parsl/executors/
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/executors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4559 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/executors/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/executors/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.285331 parsl-2024.4.8/parsl/executors/flux/
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/executors/flux/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/executors/flux/execute_parsl_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16978 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/executors/flux/executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/executors/flux/flux_instance_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.285331 parsl-2024.4.8/parsl/executors/high_throughput/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/executors/high_throughput/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/executors/high_throughput/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37225 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/executors/high_throughput/executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31491 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/executors/high_throughput/interchange.py
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/executors/high_throughput/manager_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/executors/high_throughput/monitoring_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4273 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/executors/high_throughput/mpi_prefix_composer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7975 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/executors/high_throughput/mpi_resource_management.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/executors/high_throughput/probe.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    41221 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/executors/high_throughput/process_worker_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6514 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/executors/high_throughput/zmq_pipes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.289331 parsl-2024.4.8/parsl/executors/radical/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/executors/radical/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21024 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/executors/radical/executor.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1368 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/executors/radical/rpex_master.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4960 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/executors/radical/rpex_resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1868 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/executors/radical/rpex_worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10322 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/executors/status_handling.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.289331 parsl-2024.4.8/parsl/executors/taskvine/
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/executors/taskvine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/executors/taskvine/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7085 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/executors/taskvine/exec_parsl_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32531 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/executors/taskvine/executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/executors/taskvine/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3693 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/executors/taskvine/factory_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25822 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/executors/taskvine/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7457 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/executors/taskvine/manager_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4156 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/executors/taskvine/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3353 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/executors/threads.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.289331 parsl-2024.4.8/parsl/executors/workqueue/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/executors/workqueue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/executors/workqueue/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7801 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/executors/workqueue/exec_parsl_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50038 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/executors/workqueue/executor.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5737 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/executors/workqueue/parsl_coprocess.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      735 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/executors/workqueue/parsl_coprocess_stub.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.289331 parsl-2024.4.8/parsl/jobs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/jobs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/jobs/error_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/jobs/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6143 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/jobs/job_status_poller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4855 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/jobs/states.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13860 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/jobs/strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.289331 parsl-2024.4.8/parsl/launchers/
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/launchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/launchers/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/launchers/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15464 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/launchers/launchers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3274 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/log_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.293331 parsl-2024.4.8/parsl/monitoring/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/monitoring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37021 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/monitoring/db_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/monitoring/message_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13422 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/monitoring/monitoring.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.293331 parsl-2024.4.8/parsl/monitoring/queries/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/monitoring/queries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/monitoring/queries/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5265 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/monitoring/radios.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13923 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/monitoring/remote.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9592 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/monitoring/router.py
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/monitoring/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.293331 parsl-2024.4.8/parsl/monitoring/visualization/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/monitoring/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/monitoring/visualization/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5139 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/monitoring/visualization/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.293331 parsl-2024.4.8/parsl/monitoring/visualization/plots/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/monitoring/visualization/plots/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.293331 parsl-2024.4.8/parsl/monitoring/visualization/plots/default/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/monitoring/visualization/plots/default/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/monitoring/visualization/plots/default/task_plots.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11985 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/monitoring/visualization/plots/default/workflow_plots.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10269 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/monitoring/visualization/plots/default/workflow_resource_plots.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.293331 parsl-2024.4.8/parsl/monitoring/visualization/static/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    14199 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/monitoring/visualization/static/parsl-logo-white.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      337 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/monitoring/visualization/static/parsl-monitor.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.293331 parsl-2024.4.8/parsl/monitoring/visualization/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/monitoring/visualization/templates/app.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/monitoring/visualization/templates/dag.html
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/monitoring/visualization/templates/error.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/monitoring/visualization/templates/layout.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/monitoring/visualization/templates/resource_usage.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/monitoring/visualization/templates/task.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/monitoring/visualization/templates/workflow.html
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/monitoring/visualization/templates/workflows_summary.html
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/monitoring/visualization/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/monitoring/visualization/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8256 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/monitoring/visualization/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/multiprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/process_loggers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.293331 parsl-2024.4.8/parsl/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/providers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.297331 parsl-2024.4.8/parsl/providers/ad_hoc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/providers/ad_hoc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8302 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/providers/ad_hoc/ad_hoc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.297331 parsl-2024.4.8/parsl/providers/aws/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/providers/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29009 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/providers/aws/aws.py
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/providers/aws/template.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.297331 parsl-2024.4.8/parsl/providers/azure/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/providers/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18396 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/providers/azure/azure.py
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/providers/azure/template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5702 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/providers/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4668 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/providers/cluster_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.297331 parsl-2024.4.8/parsl/providers/cobalt/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/providers/cobalt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8478 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/providers/cobalt/cobalt.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      273 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/providers/cobalt/template.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.297331 parsl-2024.4.8/parsl/providers/condor/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/providers/condor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13175 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/providers/condor/condor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/providers/condor/template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/providers/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.297331 parsl-2024.4.8/parsl/providers/googlecloud/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/providers/googlecloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8006 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/providers/googlecloud/googlecloud.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.297331 parsl-2024.4.8/parsl/providers/grid_engine/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/providers/grid_engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8565 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/providers/grid_engine/grid_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/providers/grid_engine/template.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.297331 parsl-2024.4.8/parsl/providers/kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/providers/kubernetes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12819 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/providers/kubernetes/kube.py
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/providers/kubernetes/template.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.297331 parsl-2024.4.8/parsl/providers/local/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/providers/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11369 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/providers/local/local.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.297331 parsl-2024.4.8/parsl/providers/lsf/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/providers/lsf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11502 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/providers/lsf/lsf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/providers/lsf/template.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.297331 parsl-2024.4.8/parsl/providers/pbspro/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/providers/pbspro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8822 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/providers/pbspro/pbspro.py
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/providers/pbspro/template.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.297331 parsl-2024.4.8/parsl/providers/slurm/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/providers/slurm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13916 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/providers/slurm/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/providers/slurm/template.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.301331 parsl-2024.4.8/parsl/providers/torque/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/providers/torque/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/providers/torque/template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9497 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/providers/torque/torque.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.301331 parsl-2024.4.8/parsl/serialize/
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/serialize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/serialize/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/serialize/concretes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/serialize/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6795 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/serialize/facade.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/serialize/proxystore.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.301331 parsl-2024.4.8/parsl/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/callables_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.305331 parsl-2024.4.8/parsl/tests/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/configs/ad_hoc_cluster_htex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/configs/azure_single_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/configs/bluewaters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/configs/bridges.py
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/configs/cc_in2p3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/configs/comet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/configs/cooley_htex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/configs/ec2_single_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/configs/ec2_spot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/configs/frontera.py
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/configs/htex_ad_hoc_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/configs/htex_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/configs/htex_local_alternate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/configs/htex_local_intask_staging.py
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/configs/htex_local_rsync_staging.py
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/configs/local_adhoc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/configs/local_radical.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/configs/local_radical_mpi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/configs/local_threads.py
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/configs/local_threads_checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/configs/local_threads_checkpoint_dfk_exit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/configs/local_threads_checkpoint_periodic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/configs/local_threads_checkpoint_task_exit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/configs/local_threads_ftp_in_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/configs/local_threads_globus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/configs/local_threads_http_in_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/configs/local_threads_monitoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/configs/local_threads_no_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/configs/midway.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/configs/nscc_singapore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/configs/osg_htex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/configs/petrelkube.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/configs/summit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/configs/swan_htex.py
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/configs/taskvine_ex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/configs/theta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6265 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/configs/user_opts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/configs/workqueue_ex.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14304 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.305331 parsl-2024.4.8/parsl/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/integration/latency.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.305331 parsl-2024.4.8/parsl/tests/integration/test_apps/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/integration/test_apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.309331 parsl-2024.4.8/parsl/tests/integration/test_channels/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/integration/test_channels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/integration/test_channels/test_channels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/integration/test_channels/test_local_channel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/integration/test_channels/test_scp_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/integration/test_channels/test_ssh_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/integration/test_channels/test_ssh_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/integration/test_channels/test_ssh_file_transport.py
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/integration/test_channels/test_ssh_interactive.py
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/integration/test_parsl_load_default_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.309331 parsl-2024.4.8/parsl/tests/integration/test_stress/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/integration/test_stress/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/integration/test_stress/test_python_simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/integration/test_stress/test_python_threads.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.309331 parsl-2024.4.8/parsl/tests/manual_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/manual_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/manual_tests/htex_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/manual_tests/test_ad_hoc_htex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4022 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/manual_tests/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/manual_tests/test_fan_in_out_htex_remote.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/manual_tests/test_log_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/manual_tests/test_memory_limits.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/manual_tests/test_oauth_ssh.py
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/manual_tests/test_regression_220.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/manual_tests/test_udp_simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/manual_tests/test_worker_count.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.309331 parsl-2024.4.8/parsl/tests/scaling_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/scaling_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/scaling_tests/htex_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/scaling_tests/local_threads.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3751 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/scaling_tests/test_scale.py
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/scaling_tests/vineex_condor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/scaling_tests/vineex_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/scaling_tests/wqex_condor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/scaling_tests/wqex_local.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.309331 parsl-2024.4.8/parsl/tests/site_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/site_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/site_tests/site_config_selector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2694 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/site_tests/test_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/site_tests/test_site.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.313331 parsl-2024.4.8/parsl/tests/sites/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/sites/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/sites/test_affinity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/sites/test_concurrent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/sites/test_dynamic_executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/sites/test_ec2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/sites/test_launchers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/sites/test_local_adhoc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.313331 parsl-2024.4.8/parsl/tests/sites/test_mpi/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/sites/test_mpi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/sites/test_worker_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9615 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_aalst_patterns.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.313331 parsl-2024.4.8/parsl/tests/test_bash_apps/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_bash_apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_bash_apps/test_apptimeout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_bash_apps/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4030 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_bash_apps/test_error_codes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_bash_apps/test_keyword_overlaps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_bash_apps/test_kwarg_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_bash_apps/test_memoize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_bash_apps/test_memoize_ignore_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_bash_apps/test_memoize_ignore_args_regr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_bash_apps/test_multiline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_bash_apps/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_bash_apps/test_stdout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_callables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.313331 parsl-2024.4.8/parsl/tests/test_channels/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_channels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_channels/test_large_output.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.313331 parsl-2024.4.8/parsl/tests/test_checkpointing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_checkpointing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_checkpointing/test_periodic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_checkpointing/test_python_checkpoint_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_checkpointing/test_python_checkpoint_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_checkpointing/test_python_checkpoint_3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_checkpointing/test_regression_232.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_checkpointing/test_regression_233.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_checkpointing/test_regression_239.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_checkpointing/test_task_exit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12431 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_curvezmq.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.313331 parsl-2024.4.8/parsl/tests/test_docs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_docs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_docs/test_from_slides.py
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_docs/test_kwargs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_docs/test_tutorial_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_docs/test_workflow1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_docs/test_workflow2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_docs/test_workflow4.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.317331 parsl-2024.4.8/parsl/tests/test_error_handling/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_error_handling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_error_handling/test_fail.py
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_error_handling/test_python_walltime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3864 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_error_handling/test_rand_fail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_error_handling/test_resource_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2445 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_error_handling/test_retries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_error_handling/test_retry_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_error_handling/test_retry_handler_failure.py
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_error_handling/test_serialization_fail.py
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_error_handling/test_wrap_with_logs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.317331 parsl-2024.4.8/parsl/tests/test_flowcontrol/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_flowcontrol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5098 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_flux.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.317331 parsl-2024.4.8/parsl/tests/test_htex/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_htex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_htex/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_htex/test_connected_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_htex/test_cpu_affinity_explicit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_htex/test_disconnected_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_htex/test_drain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3896 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_htex/test_htex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_htex/test_manager_failure.py
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_htex/test_missing_worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_htex/test_multiple_disconnected_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_htex/test_worker_failure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2937 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_htex/test_zmq_binding.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.317331 parsl-2024.4.8/parsl/tests/test_monitoring/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_monitoring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_monitoring/test_app_names.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2776 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_monitoring/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_monitoring/test_db_locks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3121 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_monitoring/test_fuzz_zmq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_monitoring/test_htex_init_blocks_vs_monitoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_monitoring/test_incomplete_futures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2660 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_monitoring/test_memoization_representation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_monitoring/test_viz_colouring.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.321331 parsl-2024.4.8/parsl/tests/test_mpi_apps/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_mpi_apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_mpi_apps/test_bad_mpi_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_mpi_apps/test_mpi_mode_disabled.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5034 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_mpi_apps/test_mpi_mode_enabled.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_mpi_apps/test_mpi_prefix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6317 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_mpi_apps/test_mpi_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3710 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_mpi_apps/test_resource_spec.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.321331 parsl-2024.4.8/parsl/tests/test_providers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_providers/test_cobalt_deprecation_warning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6968 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_providers/test_local_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_providers/test_pbspro_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_providers/test_slurm_instantiate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_providers/test_slurm_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_providers/test_submiterror_deprecation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.325331 parsl-2024.4.8/parsl/tests/test_python_apps/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_python_apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_python_apps/test_arg_input_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_python_apps/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_python_apps/test_context_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_python_apps/test_dep_standard_futures.py
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_python_apps/test_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_python_apps/test_depfail_propagation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_python_apps/test_fail.py
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_python_apps/test_fibonacci_iterative.py
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_python_apps/test_fibonacci_recursive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_python_apps/test_futures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_python_apps/test_garbage_collect.py
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_python_apps/test_import_fail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2679 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_python_apps/test_join.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_python_apps/test_lifted.py
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_python_apps/test_mapred.py
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_python_apps/test_memoize_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_python_apps/test_memoize_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_python_apps/test_memoize_4.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_python_apps/test_memoize_bad_id_for_memo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_python_apps/test_memoize_ignore_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_python_apps/test_memoize_joinapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_python_apps/test_outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_python_apps/test_overview.py
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_python_apps/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_python_apps/test_simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_python_apps/test_timeout.py
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_python_apps/test_type5.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.325331 parsl-2024.4.8/parsl/tests/test_radical/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_radical/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_radical/test_mpi_funcs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.325331 parsl-2024.4.8/parsl/tests/test_regression/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_regression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_regression/test_1480.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_regression/test_1606_wait_for_current_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_regression/test_1653.py
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_regression/test_221.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_regression/test_226.py
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_regression/test_2652.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_regression/test_69a.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_regression/test_854.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_regression/test_97_parallelism_0.py
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_regression/test_98.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.325331 parsl-2024.4.8/parsl/tests/test_scaling/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_scaling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6050 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_scaling/test_block_error_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_scaling/test_regression_1621.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2821 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_scaling/test_scale_down.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4597 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_scaling/test_scale_down_htex_auto_scale.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_scaling/test_shutdown_scalein.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.325331 parsl-2024.4.8/parsl/tests/test_serialization/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_serialization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_serialization/test_2555_caching_deserializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_serialization/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_serialization/test_htex_code_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_serialization/test_pack_resource_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_serialization/test_proxystore_configured.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_serialization/test_proxystore_impl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.325331 parsl-2024.4.8/parsl/tests/test_shutdown/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_shutdown/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_shutdown/test_kill_monitoring.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.329331 parsl-2024.4.8/parsl/tests/test_staging/
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_staging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_staging/staging_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2687 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_staging/test_1316.py
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_staging/test_docs_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_staging/test_docs_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_staging/test_elaborate_noop_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_staging/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_staging/test_file_apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_staging/test_file_staging.py
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_staging/test_output_chain_filenames.py
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_staging/test_staging_ftp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_staging/test_staging_ftp_in_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_staging/test_staging_globus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3307 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_staging/test_staging_https.py
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_thread_parallelism.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.329331 parsl-2024.4.8/parsl/tests/test_threads/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_threads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_threads/test_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_threads/test_lazy_errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.329331 parsl-2024.4.8/parsl/tests/test_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_utils/test_representation_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.329331 parsl-2024.4.8/parsl/usage_tracking/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/usage_tracking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6684 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/usage_tracking/usage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10979 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-08 22:42:41.000000 parsl-2024.4.8/parsl/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.277331 parsl-2024.4.8/parsl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-04-08 22:42:43.000000 parsl-2024.4.8/parsl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    17956 2024-04-08 22:42:43.000000 parsl-2024.4.8/parsl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 22:42:43.000000 parsl-2024.4.8/parsl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-08 22:42:43.000000 parsl-2024.4.8/parsl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-04-08 22:42:43.000000 parsl-2024.4.8/parsl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-08 22:42:43.000000 parsl-2024.4.8/parsl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-08 22:42:39.000000 parsl-2024.4.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 22:42:43.329331 parsl-2024.4.8/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2874 2024-04-08 22:42:39.000000 parsl-2024.4.8/setup.py
```

### Comparing `parsl-2024.4.15/LICENSE` & `parsl-2024.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/PKG-INFO` & `parsl-2024.4.8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: parsl
-Version: 2024.4.15
+Version: 2024.4.8
 Summary: Simple data dependent workflows in Python
 Home-page: https://github.com/Parsl/parsl
-Download-URL: https://github.com/Parsl/parsl/archive/2024.04.15.tar.gz
+Download-URL: https://github.com/Parsl/parsl/archive/2024.04.08.tar.gz
 Author: The Parsl Team
 Author-email: parsl@googlegroups.com
 License: Apache 2.0
 Keywords: Workflows,Scientific computing
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `parsl-2024.4.15/README.rst` & `parsl-2024.4.8/README.rst`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/__init__.py` & `parsl-2024.4.8/parsl/__init__.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/addresses.py` & `parsl-2024.4.8/parsl/addresses.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/app/app.py` & `parsl-2024.4.8/parsl/app/app.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/app/bash.py` & `parsl-2024.4.8/parsl/app/bash.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/app/errors.py` & `parsl-2024.4.8/parsl/app/errors.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/app/futures.py` & `parsl-2024.4.8/parsl/app/futures.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/app/python.py` & `parsl-2024.4.8/parsl/app/python.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/benchmark/perf.py` & `parsl-2024.4.8/parsl/benchmark/perf.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/channels/base.py` & `parsl-2024.4.8/parsl/channels/base.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/channels/errors.py` & `parsl-2024.4.8/parsl/channels/errors.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/channels/local/local.py` & `parsl-2024.4.8/parsl/channels/local/local.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/channels/oauth_ssh/oauth_ssh.py` & `parsl-2024.4.8/parsl/channels/oauth_ssh/oauth_ssh.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/channels/ssh/ssh.py` & `parsl-2024.4.8/parsl/channels/ssh/ssh.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/channels/ssh_il/ssh_il.py` & `parsl-2024.4.8/parsl/channels/ssh_il/ssh_il.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/concurrent/__init__.py` & `parsl-2024.4.8/parsl/concurrent/__init__.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/config.py` & `parsl-2024.4.8/parsl/config.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/configs/ASPIRE1.py` & `parsl-2024.4.8/parsl/configs/ASPIRE1.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/configs/Azure.py` & `parsl-2024.4.8/parsl/configs/Azure.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/configs/ad_hoc.py` & `parsl-2024.4.8/parsl/configs/ad_hoc.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/configs/bridges.py` & `parsl-2024.4.8/parsl/configs/bridges.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/configs/cc_in2p3.py` & `parsl-2024.4.8/parsl/configs/cc_in2p3.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/configs/ec2.py` & `parsl-2024.4.8/parsl/configs/ec2.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/configs/expanse.py` & `parsl-2024.4.8/parsl/configs/expanse.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/configs/frontera.py` & `parsl-2024.4.8/parsl/configs/frontera.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/configs/illinoiscluster.py` & `parsl-2024.4.8/parsl/configs/illinoiscluster.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/configs/kubernetes.py` & `parsl-2024.4.8/parsl/configs/kubernetes.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/configs/midway.py` & `parsl-2024.4.8/parsl/configs/midway.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/configs/osg.py` & `parsl-2024.4.8/parsl/configs/osg.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/configs/polaris.py` & `parsl-2024.4.8/parsl/configs/polaris.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/configs/stampede2.py` & `parsl-2024.4.8/parsl/configs/stampede2.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/configs/summit.py` & `parsl-2024.4.8/parsl/configs/summit.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/configs/toss3_llnl.py` & `parsl-2024.4.8/parsl/configs/toss3_llnl.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/configs/vineex_local.py` & `parsl-2024.4.8/parsl/configs/vineex_local.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/configs/wqex_local.py` & `parsl-2024.4.8/parsl/configs/wqex_local.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/curvezmq.py` & `parsl-2024.4.8/parsl/curvezmq.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/data_provider/data_manager.py` & `parsl-2024.4.8/parsl/data_provider/data_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,26 +3,25 @@
 from typing import Any, Callable, List, Optional, TYPE_CHECKING
 
 from parsl.app.futures import DataFuture
 from parsl.data_provider.files import File
 from parsl.data_provider.file_noop import NoOpFileStaging
 from parsl.data_provider.ftp import FTPSeparateTaskStaging
 from parsl.data_provider.http import HTTPSeparateTaskStaging
-from parsl.data_provider.zip import ZipFileStaging
 from parsl.data_provider.staging import Staging
 
 if TYPE_CHECKING:
     from parsl.dataflow.dflow import DataFlowKernel
 
 logger = logging.getLogger(__name__)
 
 # these will be shared between all executors that do not explicitly
 # override, so should not contain executor-specific state
 default_staging: List[Staging]
-default_staging = [NoOpFileStaging(), FTPSeparateTaskStaging(), HTTPSeparateTaskStaging(), ZipFileStaging()]
+default_staging = [NoOpFileStaging(), FTPSeparateTaskStaging(), HTTPSeparateTaskStaging()]
 
 
 class DataManager:
     """The DataManager is responsible for transferring input and output data.
 
     """
```

### Comparing `parsl-2024.4.15/parsl/data_provider/files.py` & `parsl-2024.4.8/parsl/data_provider/files.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/data_provider/ftp.py` & `parsl-2024.4.8/parsl/data_provider/ftp.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/data_provider/globus.py` & `parsl-2024.4.8/parsl/data_provider/globus.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/data_provider/http.py` & `parsl-2024.4.8/parsl/data_provider/http.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/data_provider/rsync.py` & `parsl-2024.4.8/parsl/data_provider/rsync.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/data_provider/staging.py` & `parsl-2024.4.8/parsl/data_provider/staging.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/dataflow/dflow.py` & `parsl-2024.4.8/parsl/dataflow/dflow.py`

 * *Files 1% similar despite different names*

```diff
@@ -173,19 +173,18 @@
         self.checkpointed_tasks = 0
         self._checkpoint_timer = None
         self.checkpoint_mode = config.checkpoint_mode
         self.checkpointable_tasks: List[TaskRecord] = []
 
         # this must be set before executors are added since add_executors calls
         # job_status_poller.add_executors.
-        radio = self.monitoring.radio if self.monitoring else None
         self.job_status_poller = JobStatusPoller(strategy=self.config.strategy,
                                                  strategy_period=self.config.strategy_period,
                                                  max_idletime=self.config.max_idletime,
-                                                 monitoring=radio)
+                                                 dfk=self)
 
         self.executors: Dict[str, ParslExecutor] = {}
 
         self.data_manager = DataManager(self)
         parsl_internal_executor = ThreadPoolExecutor(max_threads=config.internal_tasks_max_threads, label='_parsl_internal')
         self.add_executors(config.executors)
         self.add_executors([parsl_internal_executor])
@@ -236,37 +235,24 @@
         task_log_info['tasks_memo_completed_count'] = self.task_state_counts[States.memo_done]
         task_log_info['from_memo'] = task_record['from_memo']
         task_log_info['task_inputs'] = str(task_record['kwargs'].get('inputs', None))
         task_log_info['task_outputs'] = str(task_record['kwargs'].get('outputs', None))
         task_log_info['task_stdin'] = task_record['kwargs'].get('stdin', None)
         stdout_spec = task_record['kwargs'].get('stdout', None)
         stderr_spec = task_record['kwargs'].get('stderr', None)
-
-        # stdout and stderr strings are set to the filename if we can
-        # interpret the specification; otherwise, set to the empty string
-        # (on exception, or when not specified)
-
-        if stdout_spec is not None:
-            try:
-                stdout_name, _ = get_std_fname_mode('stdout', stdout_spec)
-            except Exception:
-                logger.exception("Could not parse stdout specification {} for task {}".format(stdout_spec, task_record['id']))
-                stdout_name = ""
-        else:
-            stdout_name = ""
-
-        if stderr_spec is not None:
-            try:
-                stderr_name, _ = get_std_fname_mode('stderr', stderr_spec)
-            except Exception:
-                logger.exception("Could not parse stderr specification {} for task {}".format(stderr_spec, task_record['id']))
-                stderr_name = ""
-        else:
-            stderr_name = ""
-
+        try:
+            stdout_name, _ = get_std_fname_mode('stdout', stdout_spec)
+        except Exception as e:
+            logger.warning("Incorrect stdout format {} for Task {}".format(stdout_spec, task_record['id']))
+            stdout_name = str(e)
+        try:
+            stderr_name, _ = get_std_fname_mode('stderr', stderr_spec)
+        except Exception as e:
+            logger.warning("Incorrect stderr format {} for Task {}".format(stderr_spec, task_record['id']))
+            stderr_name = str(e)
         task_log_info['task_stdout'] = stdout_name
         task_log_info['task_stderr'] = stderr_name
         task_log_info['task_fail_history'] = ",".join(task_record['fail_history'])
         task_log_info['task_depends'] = None
         if task_record['depends'] is not None:
             task_log_info['task_depends'] = ",".join([str(t.tid) for t in task_record['depends']
                                                       if isinstance(t, AppFuture) or isinstance(t, DataFuture)])
@@ -684,14 +670,22 @@
                 logger.error("add_done_callback got an exception which will be ignored", exc_info=True)
 
             task_record['exec_fu'] = exec_fu
 
     def launch_task(self, task_record: TaskRecord) -> Future:
         """Handle the actual submission of the task to the executor layer.
 
+        If the app task has the executors attributes not set (default=='all')
+        the task is launched on a randomly selected executor from the
+        list of executors. This behavior could later be updated to support
+        binding to executors based on user specified criteria.
+
+        If the app task specifies a particular set of executors, it will be
+        targeted at those specific executors.
+
         Args:
             task_record : The task record
 
         Returns:
             Future that tracks the execution of the submitted function
         """
         task_id = task_record['id']
@@ -1134,18 +1128,14 @@
 
     def add_executors(self, executors: Sequence[ParslExecutor]) -> None:
         for executor in executors:
             executor.run_id = self.run_id
             executor.run_dir = self.run_dir
             executor.hub_address = self.hub_address
             executor.hub_port = self.hub_zmq_port
-            if self.monitoring:
-                executor.monitoring_radio = self.monitoring.radio
-            else:
-                executor.monitoring_radio = None
             if hasattr(executor, 'provider'):
                 if hasattr(executor.provider, 'script_dir'):
                     executor.provider.script_dir = os.path.join(self.run_dir, 'submit_scripts')
                     os.makedirs(executor.provider.script_dir, exist_ok=True)
 
                     if hasattr(executor.provider, 'channels'):
                         logger.debug("Creating script_dir across multiple channels")
@@ -1241,15 +1231,16 @@
         if self.monitoring:
             logger.info("Sending final monitoring message")
             self.monitoring.send(MessageType.WORKFLOW_INFO,
                                  {'tasks_failed_count': self.task_state_counts[States.failed],
                                   'tasks_completed_count': self.task_state_counts[States.exec_done],
                                   "time_began": self.time_began,
                                   'time_completed': self.time_completed,
-                                  'run_id': self.run_id, 'rundir': self.run_dir})
+                                  'run_id': self.run_id, 'rundir': self.run_dir,
+                                  'exit_now': True})
 
             logger.info("Terminating monitoring")
             self.monitoring.close()
             logger.info("Terminated monitoring")
 
         logger.info("DFK cleanup complete")
 
@@ -1391,28 +1382,18 @@
         if checkpointDirs:
             return self._load_checkpoints(checkpointDirs)
         else:
             return {}
 
     @staticmethod
     def _log_std_streams(task_record: TaskRecord) -> None:
-        tid = task_record['id']
-
-        def log_std_stream(name: str, target) -> None:
-            if target is None:
-                logger.info(f"{name} for task {tid} will not be redirected.")
-            elif isinstance(target, str):
-                logger.info(f"{name} for task {tid} will be redirected to {target}")
-            elif isinstance(target, tuple) and len(target) == 2:
-                logger.info(f"{name} for task {tid} will be redirected to {target[0]} with mode {target[1]}")
-            else:
-                logger.error(f"{name} for task {tid} has unknown specification: {target!r}")
-
-        log_std_stream("Standard out", task_record['app_fu'].stdout)
-        log_std_stream("Standard error", task_record['app_fu'].stderr)
+        if task_record['app_fu'].stdout is not None:
+            logger.info("Standard output for task {} available at {}".format(task_record['id'], task_record['app_fu'].stdout))
+        if task_record['app_fu'].stderr is not None:
+            logger.info("Standard error for task {} available at {}".format(task_record['id'], task_record['app_fu'].stderr))
 
 
 class DataFlowKernelLoader:
     """Manage which DataFlowKernel is active.
 
     This is a singleton class containing only class methods. You should not
     need to instantiate this class.
```

### Comparing `parsl-2024.4.15/parsl/dataflow/errors.py` & `parsl-2024.4.8/parsl/dataflow/errors.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/dataflow/futures.py` & `parsl-2024.4.8/parsl/dataflow/futures.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+"""This module implements the AppFutures.
+
+We have two basic types of futures:
+    1. DataFutures which represent data objects
+    2. AppFutures which represent the futures on App/Leaf tasks.
+
+"""
 from __future__ import annotations
 
 from concurrent.futures import Future
 import logging
 import threading
 from typing import Any, Optional, Sequence
```

### Comparing `parsl-2024.4.15/parsl/dataflow/memoization.py` & `parsl-2024.4.8/parsl/dataflow/memoization.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/dataflow/rundirs.py` & `parsl-2024.4.8/parsl/dataflow/rundirs.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/dataflow/states.py` & `parsl-2024.4.8/parsl/dataflow/states.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/dataflow/taskrecord.py` & `parsl-2024.4.8/parsl/dataflow/taskrecord.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/errors.py` & `parsl-2024.4.8/parsl/errors.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/executors/base.py` & `parsl-2024.4.8/parsl/executors/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from abc import ABCMeta, abstractmethod
 from concurrent.futures import Future
-from typing import Any, Callable, Dict, Optional
+from typing import Any, Callable, Dict, Optional, List
 from typing_extensions import Literal, Self
 
-from parsl.monitoring.radios import MonitoringRadio
+from parsl.jobs.states import JobStatus
 
 
 class ParslExecutor(metaclass=ABCMeta):
     """Executors are abstractions that represent available compute resources
     to which you could submit arbitrary App tasks.
 
     This is an abstract base class that only enforces concrete implementations
@@ -75,14 +75,21 @@
     def shutdown(self) -> None:
         """Shutdown the executor.
 
         This includes all attached resources such as workers and controllers.
         """
         pass
 
+    def create_monitoring_info(self, status: Dict[str, JobStatus]) -> List[object]:
+        """Create a monitoring message for each block based on the poll status.
+
+        :return: a list of dictionaries mapping to the info of each block
+        """
+        return []
+
     def monitor_resources(self) -> bool:
         """Should resource monitoring happen for tasks on running on this executor?
 
         Parsl resource monitoring conflicts with execution styles which use threads, and
         can deadlock while running.
 
         This function allows resource monitoring to be disabled per executor implementation.
@@ -124,17 +131,7 @@
         """Port to the Hub for monitoring.
         """
         return self._hub_port
 
     @hub_port.setter
     def hub_port(self, value: Optional[int]) -> None:
         self._hub_port = value
-
-    @property
-    def monitoring_radio(self) -> Optional[MonitoringRadio]:
-        """Local radio for sending monitoring messages
-        """
-        return self._monitoring_radio
-
-    @monitoring_radio.setter
-    def monitoring_radio(self, value: Optional[MonitoringRadio]) -> None:
-        self._monitoring_radio = value
```

### Comparing `parsl-2024.4.15/parsl/executors/errors.py` & `parsl-2024.4.8/parsl/executors/errors.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/executors/flux/execute_parsl_task.py` & `parsl-2024.4.8/parsl/executors/flux/execute_parsl_task.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/executors/flux/executor.py` & `parsl-2024.4.8/parsl/executors/flux/executor.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/executors/flux/flux_instance_manager.py` & `parsl-2024.4.8/parsl/executors/flux/flux_instance_manager.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/executors/high_throughput/executor.py` & `parsl-2024.4.8/parsl/executors/high_throughput/executor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 import typing
 from collections import defaultdict
 from concurrent.futures import Future
 import typeguard
 import logging
 import threading
 import queue
+import datetime
 import pickle
 from dataclasses import dataclass
 from multiprocessing import Process, Queue
 from typing import Dict, Sequence
 from typing import List, Optional, Tuple, Union, Callable
 import math
 import warnings
 
 import parsl.launchers
 from parsl.serialize import pack_res_spec_apply_message, deserialize
 from parsl.serialize.errors import SerializationError, DeserializationError
 from parsl.app.errors import RemoteExceptionWrapper
-from parsl.jobs.states import JobStatus, JobState, TERMINAL_STATES
+from parsl.jobs.states import JobStatus, JobState
 from parsl.executors.high_throughput import zmq_pipes
 from parsl.executors.high_throughput import interchange
 from parsl.executors.errors import (
     BadMessage, ScalingFailed,
 )
 from parsl.executors.high_throughput.mpi_prefix_composer import (
     VALID_LAUNCHERS,
@@ -672,14 +673,30 @@
 
         # Post task to the outgoing queue
         self.outgoing_q.put(msg)
 
         # Return the future
         return fut
 
+    def create_monitoring_info(self, status):
+        """ Create a msg for monitoring based on the poll status
+
+        """
+        msg = []
+        for bid, s in status.items():
+            d = {}
+            d['run_id'] = self.run_id
+            d['status'] = s.status_name
+            d['timestamp'] = datetime.datetime.now()
+            d['executor_label'] = self.label
+            d['job_id'] = self.blocks_to_job_id.get(bid, None)
+            d['block_id'] = bid
+            msg.append(d)
+        return msg
+
     @property
     def workers_per_node(self) -> Union[int, float]:
         return self._workers_per_node
 
     def scale_in(self, blocks: int, max_idletime: Optional[float] = None) -> List[str]:
         """Scale in the number of active blocks by specified amount.
 
@@ -709,28 +726,16 @@
         logger.debug(f"Scale in called, blocks={blocks}")
 
         @dataclass
         class BlockInfo:
             tasks: int  # sum of tasks in this block
             idle: float  # shortest idle time of any manager in this block
 
-        # block_info will be populated from two sources:
-        # the Job Status Poller mutable block list, and the list of blocks
-        # which have connected to the interchange.
-
-        def new_block_info():
-            return BlockInfo(tasks=0, idle=float('inf'))
-
-        block_info: Dict[str, BlockInfo] = defaultdict(new_block_info)
-
-        for block_id, job_status in self._status.items():
-            if job_status.state not in TERMINAL_STATES:
-                block_info[block_id] = new_block_info()
-
         managers = self.connected_managers()
+        block_info: Dict[str, BlockInfo] = defaultdict(lambda: BlockInfo(tasks=0, idle=float('inf')))
         for manager in managers:
             if not manager['active']:
                 continue
             b_id = manager['block_id']
             block_info[b_id].tasks += manager['tasks']
             block_info[b_id].idle = min(block_info[b_id].idle, manager['idle_duration'])
```

### Comparing `parsl-2024.4.15/parsl/executors/high_throughput/interchange.py` & `parsl-2024.4.8/parsl/executors/high_throughput/interchange.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/executors/high_throughput/mpi_prefix_composer.py` & `parsl-2024.4.8/parsl/executors/high_throughput/mpi_prefix_composer.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/executors/high_throughput/mpi_resource_management.py` & `parsl-2024.4.8/parsl/executors/high_throughput/mpi_resource_management.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/executors/high_throughput/probe.py` & `parsl-2024.4.8/parsl/executors/high_throughput/probe.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/executors/high_throughput/process_worker_pool.py` & `parsl-2024.4.8/parsl/executors/high_throughput/process_worker_pool.py`

 * *Files 0% similar despite different names*

```diff
@@ -357,17 +357,15 @@
                 if tasks == HEARTBEAT_CODE:
                     logger.debug("Got heartbeat from interchange")
                 elif tasks == DRAINED_CODE:
                     logger.info("Got fulled drained message from interchange - setting kill flag")
                     kill_event.set()
                 else:
                     task_recv_counter += len(tasks)
-                    logger.debug("Got executor tasks: {}, cumulative count of tasks: {}".format(
-                        [t['task_id'] for t in tasks], task_recv_counter
-                    ))
+                    logger.debug("Got executor tasks: {}, cumulative count of tasks: {}".format([t['task_id'] for t in tasks], task_recv_counter))
 
                     for task in tasks:
                         self.task_scheduler.put_task(task)
 
             else:
                 logger.debug("No incoming tasks")
```

### Comparing `parsl-2024.4.15/parsl/executors/high_throughput/zmq_pipes.py` & `parsl-2024.4.8/parsl/executors/high_throughput/zmq_pipes.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/executors/radical/executor.py` & `parsl-2024.4.8/parsl/executors/radical/executor.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/executors/radical/rpex_master.py` & `parsl-2024.4.8/parsl/executors/radical/rpex_master.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/executors/radical/rpex_resources.py` & `parsl-2024.4.8/parsl/executors/radical/rpex_resources.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/executors/radical/rpex_worker.py` & `parsl-2024.4.8/parsl/executors/radical/rpex_worker.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/executors/status_handling.py` & `parsl-2024.4.8/parsl/executors/status_handling.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 from __future__ import annotations
-import datetime
 import logging
 import threading
-import time
 from itertools import compress
 from abc import abstractmethod, abstractproperty
 from concurrent.futures import Future
-from typing import List, Any, Dict, Optional, Sequence, Tuple, Union, Callable
+from typing import List, Any, Dict, Optional, Tuple, Union, Callable
 
 from parsl.executors.base import ParslExecutor
 from parsl.executors.errors import BadStateException, ScalingFailed
 from parsl.jobs.states import JobStatus, JobState
 from parsl.jobs.error_handlers import simple_error_handler, noop_error_handler
-from parsl.monitoring.message_type import MessageType
 from parsl.providers.base import ExecutionProvider
 from parsl.utils import AtomicIDCounter
 
 logger = logging.getLogger(__name__)
 
 
 class BlockProviderExecutor(ParslExecutor):
@@ -70,17 +67,14 @@
 
         self._block_id_counter = AtomicIDCounter()
 
         self._tasks = {}  # type: Dict[object, Future]
         self.blocks_to_job_id = {}  # type: Dict[str, str]
         self.job_ids_to_block = {}  # type: Dict[str, str]
 
-        self._last_poll_time = 0.0
-        self._status = {}  # type: Dict[str, JobStatus]
-
     def _make_status_dict(self, block_ids: List[str], status_list: List[JobStatus]) -> Dict[str, JobStatus]:
         """Given a list of block ids and a list of corresponding status strings,
         returns a dictionary mapping each block id to the corresponding status
 
         :param block_ids: the list of block ids
         :param status_list: the list of job status strings
         :return: the resulting dictionary
@@ -236,81 +230,7 @@
         for bid in block_ids:
             job_ids.append(self.blocks_to_job_id[bid])
         return block_ids, job_ids
 
     @abstractproperty
     def workers_per_node(self) -> Union[int, float]:
         pass
-
-    def send_monitoring_info(self, status: Dict) -> None:
-        # Send monitoring info for HTEX when monitoring enabled
-        if self.monitoring_radio:
-            msg = self.create_monitoring_info(status)
-            logger.debug("Sending message {} to hub from job status poller".format(msg))
-            self.monitoring_radio.send((MessageType.BLOCK_INFO, msg))
-
-    def create_monitoring_info(self, status: Dict[str, JobStatus]) -> Sequence[object]:
-        """Create a monitoring message for each block based on the poll status.
-        """
-        msg = []
-        for bid, s in status.items():
-            d: Dict[str, Any] = {}
-            d['run_id'] = self.run_id
-            d['status'] = s.status_name
-            d['timestamp'] = datetime.datetime.now()
-            d['executor_label'] = self.label
-            d['job_id'] = self.blocks_to_job_id.get(bid, None)
-            d['block_id'] = bid
-            msg.append(d)
-        return msg
-
-    def poll_facade(self) -> None:
-        now = time.time()
-        if now >= self._last_poll_time + self.status_polling_interval:
-            previous_status = self._status
-            self._status = self.status()
-            self._last_poll_time = now
-            delta_status = {}
-            for block_id in self._status:
-                if block_id not in previous_status \
-                   or previous_status[block_id].state != self._status[block_id].state:
-                    delta_status[block_id] = self._status[block_id]
-
-            if delta_status:
-                self.send_monitoring_info(delta_status)
-
-    @property
-    def status_facade(self) -> Dict[str, JobStatus]:
-        """Return the status of all jobs/blocks of the executor of this poller.
-
-        :return: a dictionary mapping block ids (in string) to job status
-        """
-        return self._status
-
-    def scale_in_facade(self, n: int, max_idletime: Optional[float] = None) -> List[str]:
-
-        if max_idletime is None:
-            block_ids = self.scale_in(n)
-        else:
-            # This is a HighThroughputExecutor-specific interface violation.
-            # This code hopes, through pan-codebase reasoning, that this
-            # scale_in method really does come from HighThroughputExecutor,
-            # and so does have an extra max_idletime parameter not present
-            # in the executor interface.
-            block_ids = self.scale_in(n, max_idletime=max_idletime)  # type: ignore[call-arg]
-        if block_ids is not None:
-            new_status = {}
-            for block_id in block_ids:
-                new_status[block_id] = JobStatus(JobState.CANCELLED)
-                del self._status[block_id]
-            self.send_monitoring_info(new_status)
-        return block_ids
-
-    def scale_out_facade(self, n: int) -> List[str]:
-        block_ids = self.scale_out(n)
-        if block_ids is not None:
-            new_status = {}
-            for block_id in block_ids:
-                new_status[block_id] = JobStatus(JobState.PENDING)
-            self.send_monitoring_info(new_status)
-            self._status.update(new_status)
-        return block_ids
```

### Comparing `parsl-2024.4.15/parsl/executors/taskvine/errors.py` & `parsl-2024.4.8/parsl/executors/taskvine/errors.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/executors/taskvine/exec_parsl_function.py` & `parsl-2024.4.8/parsl/executors/taskvine/exec_parsl_function.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/executors/taskvine/executor.py` & `parsl-2024.4.8/parsl/executors/taskvine/executor.py`

 * *Files 1% similar despite different names*

```diff
@@ -592,31 +592,26 @@
         logger.debug(f"Counted {self._outstanding_tasks} outstanding tasks")
         return self._outstanding_tasks
 
     @property
     def workers_per_node(self) -> Union[int, float]:
         return 1
 
-    def scale_in(self, count: int) -> List[str]:
+    def scale_in(self, count):
         """Scale in method. Cancel a given number of blocks
         """
         # Obtain list of blocks to kill
         to_kill = list(self.blocks_to_job_id.keys())[:count]
         kill_ids = [self.blocks_to_job_id[block] for block in to_kill]
 
         # Cancel the blocks provisioned
         if self.provider:
-            logger.info(f"Scaling in jobs: {kill_ids}")
-            r = self.provider.cancel(kill_ids)
-            job_ids = self._filter_scale_in_ids(kill_ids, r)
-            block_ids_killed = [self.job_ids_to_block[jid] for jid in job_ids]
-            return block_ids_killed
+            self.provider.cancel(kill_ids)
         else:
             logger.error("No execution provider available to scale")
-            return []
 
     def shutdown(self, *args, **kwargs):
         """Shutdown the executor. Sets flag to cancel the submit process and
         collector thread, which shuts down the TaskVine system submission.
         """
         if not self._is_started:
             # Don't shutdown if the executor never starts.
```

### Comparing `parsl-2024.4.15/parsl/executors/taskvine/factory.py` & `parsl-2024.4.8/parsl/executors/taskvine/factory.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/executors/taskvine/factory_config.py` & `parsl-2024.4.8/parsl/executors/taskvine/factory_config.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/executors/taskvine/manager.py` & `parsl-2024.4.8/parsl/executors/taskvine/manager.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/executors/taskvine/manager_config.py` & `parsl-2024.4.8/parsl/executors/taskvine/manager_config.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/executors/taskvine/utils.py` & `parsl-2024.4.8/parsl/executors/taskvine/utils.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/executors/threads.py` & `parsl-2024.4.8/parsl/executors/threads.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/executors/workqueue/errors.py` & `parsl-2024.4.8/parsl/executors/workqueue/errors.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/executors/workqueue/exec_parsl_function.py` & `parsl-2024.4.8/parsl/executors/workqueue/exec_parsl_function.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/executors/workqueue/executor.py` & `parsl-2024.4.8/parsl/executors/workqueue/executor.py`

 * *Files 1% similar despite different names*

```diff
@@ -687,31 +687,26 @@
         logger.debug(f"Counted {outstanding} outstanding tasks")
         return outstanding
 
     @property
     def workers_per_node(self) -> Union[int, float]:
         return 1
 
-    def scale_in(self, count: int) -> List[str]:
+    def scale_in(self, count):
         """Scale in method.
         """
         # Obtain list of blocks to kill
         to_kill = list(self.blocks_to_job_id.keys())[:count]
         kill_ids = [self.blocks_to_job_id[block] for block in to_kill]
 
         # Cancel the blocks provisioned
         if self.provider:
-            logger.info(f"Scaling in jobs: {kill_ids}")
-            r = self.provider.cancel(kill_ids)
-            job_ids = self._filter_scale_in_ids(kill_ids, r)
-            block_ids_killed = [self.job_ids_to_block[jid] for jid in job_ids]
-            return block_ids_killed
+            self.provider.cancel(kill_ids)
         else:
-            logger.error("No execution provider available to scale in")
-            return []
+            logger.error("No execution provider available to scale")
 
     def shutdown(self, *args, **kwargs):
         """Shutdown the executor. Sets flag to cancel the submit process and
         collector thread, which shuts down the Work Queue system submission.
         """
         if not self.is_started:
             # Don't shutdown if the executor never starts.
```

### Comparing `parsl-2024.4.15/parsl/executors/workqueue/parsl_coprocess.py` & `parsl-2024.4.8/parsl/executors/workqueue/parsl_coprocess.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/executors/workqueue/parsl_coprocess_stub.py` & `parsl-2024.4.8/parsl/executors/workqueue/parsl_coprocess_stub.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/jobs/error_handlers.py` & `parsl-2024.4.8/parsl/jobs/error_handlers.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/jobs/states.py` & `parsl-2024.4.8/parsl/jobs/states.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/jobs/strategy.py` & `parsl-2024.4.8/parsl/jobs/strategy.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from __future__ import annotations
 import logging
 import time
 import math
 import warnings
 from typing import Dict, List, Optional, Sequence, TypedDict
 
+import parsl.jobs.job_status_poller as jsp
+
 from parsl.executors import HighThroughputExecutor
 from parsl.executors.base import ParslExecutor
 from parsl.executors.status_handling import BlockProviderExecutor
 from parsl.jobs.states import JobState
 from parsl.process_loggers import wrap_with_logs
 
 
@@ -144,62 +146,68 @@
 
         logger.debug("Scaling strategy: {0}".format(strategy))
 
     def add_executors(self, executors: Sequence[ParslExecutor]) -> None:
         for executor in executors:
             self.executors[executor.label] = {'idle_since': None, 'first': True}
 
-    def _strategy_init_only(self, executors: List[BlockProviderExecutor]) -> None:
+    def _strategy_init_only(self, executor_facades: List[jsp.PolledExecutorFacade]) -> None:
         """Scale up to init_blocks at the start, then nothing more.
         """
-        for executor in executors:
+        for ef in executor_facades:
+            executor = ef.executor
             if self.executors[executor.label]['first']:
                 logger.debug(f"strategy_init_only: scaling out {executor.provider.init_blocks} initial blocks for {executor.label}")
-                executor.scale_out_facade(executor.provider.init_blocks)
+                ef.scale_out(executor.provider.init_blocks)
                 self.executors[executor.label]['first'] = False
             else:
                 logger.debug("strategy_init_only: doing nothing")
 
-    def _strategy_simple(self, executors: List[BlockProviderExecutor]) -> None:
-        self._general_strategy(executors, strategy_type='simple')
+    def _strategy_simple(self, executor_facades: List[jsp.PolledExecutorFacade]) -> None:
+        self._general_strategy(executor_facades, strategy_type='simple')
 
-    def _strategy_htex_auto_scale(self, executors: List[BlockProviderExecutor]) -> None:
+    def _strategy_htex_auto_scale(self, executor_facades: List[jsp.PolledExecutorFacade]) -> None:
         """HTEX specific auto scaling strategy
 
         This strategy works only for HTEX. This strategy will scale out by
         requesting additional compute resources via the provider when the
         workload requirements exceed the provisioned capacity. The scale out
         behavior is exactly like the 'simple' strategy.
 
         If there are idle blocks during execution, this strategy will terminate
         those idle blocks specifically. When # of tasks >> # of blocks, HTEX places
         tasks evenly across blocks, which makes it rather difficult to ensure that
         some blocks will reach 0% utilization. Consequently, this strategy can be
         expected to scale in effectively only when # of workers, or tasks executing
         per block is close to 1.
         """
-        self._general_strategy(executors, strategy_type='htex')
+        self._general_strategy(executor_facades, strategy_type='htex')
 
     @wrap_with_logs
-    def _general_strategy(self, executors: List[BlockProviderExecutor], *, strategy_type: str) -> None:
-        logger.debug(f"general strategy starting with strategy_type {strategy_type} for {len(executors)} executors")
+    def _general_strategy(self, executor_facades, *, strategy_type):
+        logger.debug(f"general strategy starting with strategy_type {strategy_type} for {len(executor_facades)} executors")
 
-        for executor in executors:
+        for ef in executor_facades:
+            executor = ef.executor
             label = executor.label
+            if not isinstance(executor, BlockProviderExecutor):
+                logger.debug(f"Not strategizing for executor {label} because scaling not enabled")
+                continue
             logger.debug(f"Strategizing for executor {label}")
 
             if self.executors[label]['first']:
+                executor = ef.executor
                 logger.debug(f"Scaling out {executor.provider.init_blocks} initial blocks for {label}")
-                executor.scale_out_facade(executor.provider.init_blocks)
+                ef.scale_out(executor.provider.init_blocks)
                 self.executors[label]['first'] = False
 
             # Tasks that are either pending completion
             active_tasks = executor.outstanding
 
-            status = executor.status_facade
+            status = ef.status
 
             # FIXME we need to handle case where provider does not define these
             # FIXME probably more of this logic should be moved to the provider
             min_blocks = executor.provider.min_blocks
             max_blocks = executor.provider.max_blocks
             tasks_per_node = executor.workers_per_node
 
@@ -235,34 +243,31 @@
                 if active_blocks <= min_blocks:
                     logger.debug("Strategy case 1a: Executor has no active tasks and minimum blocks. Taking no action.")
                 # Case 1b
                 # More blocks than min_blocks. Scale in
                 else:
                     # We want to make sure that max_idletime is reached
                     # before killing off resources
-                    logger.debug(f"Strategy case 1b: Executor has no active tasks, and more ({active_blocks})"
-                                 f" than minimum blocks ({min_blocks})")
+                    logger.debug(f"Strategy case 1b: Executor has no active tasks, and more ({active_blocks}) than minimum blocks ({min_blocks})")
 
                     if not self.executors[executor.label]['idle_since']:
                         logger.debug(f"Starting idle timer for executor. If idle time exceeds {self.max_idletime}s, blocks will be scaled in")
                         self.executors[executor.label]['idle_since'] = time.time()
-                    idle_since = self.executors[executor.label]['idle_since']
-                    assert idle_since is not None, "The `if` statement above this assert should have forced idle time to be not-None"
 
+                    idle_since = self.executors[executor.label]['idle_since']
                     idle_duration = time.time() - idle_since
                     if idle_duration > self.max_idletime:
                         # We have resources idle for the max duration,
                         # we have to scale_in now.
                         logger.debug(f"Idle time has reached {self.max_idletime}s for executor {label}; scaling in")
-                        executor.scale_in_facade(active_blocks - min_blocks)
+                        ef.scale_in(active_blocks - min_blocks)
 
                     else:
                         logger.debug(
-                                f"Idle time {idle_duration}s is less than max_idletime {self.max_idletime}s"
-                                f" for executor {label}; not scaling in")
+                                f"Idle time {idle_duration}s is less than max_idletime {self.max_idletime}s for executor {label}; not scaling in")
 
             # Case 2
             # More tasks than the available slots.
             elif (float(active_slots) / active_tasks) < parallelism:
                 logger.debug("Strategy case 2: slots are overloaded - (slot_ratio = active_slots/active_tasks) < parallelism")
 
                 # Case 2a
@@ -273,24 +278,24 @@
                 # Case 2b
                 else:
                     logger.debug(f"Strategy case 2b: active_blocks {active_blocks} < max_blocks {max_blocks} so scaling out")
                     excess_slots = math.ceil((active_tasks * parallelism) - active_slots)
                     excess_blocks = math.ceil(float(excess_slots) / (tasks_per_node * nodes_per_block))
                     excess_blocks = min(excess_blocks, max_blocks - active_blocks)
                     logger.debug(f"Requesting {excess_blocks} more blocks")
-                    executor.scale_out_facade(excess_blocks)
+                    ef.scale_out(excess_blocks)
 
             elif active_slots == 0 and active_tasks > 0:
                 logger.debug("Strategy case 4a: No active slots but some active tasks - could scale out by a single block")
 
                 # Case 4a
                 if active_blocks < max_blocks:
                     logger.debug("Requesting single block")
 
-                    executor.scale_out_facade(1)
+                    ef.scale_out(1)
                 else:
                     logger.debug("Not requesting single block, because at maxblocks already")
 
             # Case 4b
             # More slots than tasks
             elif active_slots > 0 and active_slots > active_tasks:
                 logger.debug("Strategy case 4b: more slots than tasks")
@@ -298,15 +303,15 @@
                     # Scale in for htex
                     if isinstance(executor, HighThroughputExecutor):
                         if active_blocks > min_blocks:
                             excess_slots = math.ceil(active_slots - (active_tasks * parallelism))
                             excess_blocks = math.ceil(float(excess_slots) / (tasks_per_node * nodes_per_block))
                             excess_blocks = min(excess_blocks, active_blocks - min_blocks)
                             logger.debug(f"Requesting scaling in by {excess_blocks} blocks with idle time {self.max_idletime}s")
-                            executor.scale_in_facade(excess_blocks, max_idletime=self.max_idletime)
+                            ef.scale_in(excess_blocks, max_idletime=self.max_idletime)
                     else:
                         logger.error("This strategy does not support scaling in except for HighThroughputExecutor - taking no action")
                 else:
                     logger.debug("This strategy does not support scaling in")
 
             # Case 3
             # tasks ~ slots
```

### Comparing `parsl-2024.4.15/parsl/launchers/__init__.py` & `parsl-2024.4.8/parsl/launchers/__init__.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/launchers/base.py` & `parsl-2024.4.8/parsl/launchers/base.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/launchers/launchers.py` & `parsl-2024.4.8/parsl/launchers/launchers.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/log_utils.py` & `parsl-2024.4.8/parsl/log_utils.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/monitoring/db_manager.py` & `parsl-2024.4.8/parsl/monitoring/db_manager.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/monitoring/monitoring.py` & `parsl-2024.4.8/parsl/monitoring/monitoring.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 from __future__ import annotations
 
 import os
 import time
 import logging
-import multiprocessing.synchronize as ms
 import typeguard
+import zmq
 
 import queue
 
 from parsl.multiprocessing import ForkProcess, SizedQueue
 from multiprocessing import Process
-from multiprocessing import Event
 from multiprocessing.queues import Queue
 from parsl.log_utils import set_file_logger
 from parsl.utils import RepresentationMixin
 from parsl.process_loggers import wrap_with_logs
 from parsl.utils import setproctitle
 
 from parsl.serialize import deserialize
 
-from parsl.monitoring.radios import MultiprocessingQueueRadio
 from parsl.monitoring.router import router_starter
 from parsl.monitoring.message_type import MessageType
 from parsl.monitoring.types import AddressedMonitoringMessage
 from typing import cast, Any, Optional, Tuple, Union, TYPE_CHECKING
 
 _db_manager_excepts: Optional[Exception]
 
@@ -88,14 +86,20 @@
         resource_monitoring_interval : float
              The time interval, in seconds, at which the monitoring records the resource usage of each task.
              If set to 0, only start and end information will be logged, and no periodic monitoring will
              be made.
              Default: 30 seconds
         """
 
+        # Any is used to disable typechecking on uses of _dfk_channel,
+        # because it is used in the code as if it points to a channel, but
+        # the static type is that it can also be None. The code relies on
+        # .start() being called and initialising this to a real channel.
+        self._dfk_channel = None  # type: Any
+
         if _db_manager_excepts:
             raise _db_manager_excepts
 
         self.hub_address = hub_address
         self.hub_port = hub_port
         self.hub_port_range = hub_port_range
 
@@ -149,20 +153,16 @@
 
         self.node_msgs: Queue[AddressedMonitoringMessage]
         self.node_msgs = SizedQueue()
 
         self.block_msgs: Queue[AddressedMonitoringMessage]
         self.block_msgs = SizedQueue()
 
-        self.router_exit_event: ms.Event
-        self.router_exit_event = Event()
-
         self.router_proc = ForkProcess(target=router_starter,
-                                       args=(comm_q, self.exception_q, self.priority_msgs, self.node_msgs,
-                                             self.block_msgs, self.resource_msgs, self.router_exit_event),
+                                       args=(comm_q, self.exception_q, self.priority_msgs, self.node_msgs, self.block_msgs, self.resource_msgs),
                                        kwargs={"hub_address": self.hub_address,
                                                "udp_port": self.hub_port,
                                                "zmq_port_range": self.hub_port_range,
                                                "logdir": self.logdir,
                                                "logging_level": logging.DEBUG if self.monitoring_debug else logging.INFO,
                                                "run_id": run_id
                                                },
@@ -187,63 +187,72 @@
                                        args=(self.logdir, self.resource_msgs, dfk_run_dir),
                                        name="Monitoring-Filesystem-Process",
                                        daemon=True
                                        )
         self.filesystem_proc.start()
         logger.info(f"Started filesystem radio receiver process {self.filesystem_proc.pid}")
 
-        self.radio = MultiprocessingQueueRadio(self.block_msgs)
-
         try:
             comm_q_result = comm_q.get(block=True, timeout=120)
         except queue.Empty:
             logger.error("Hub has not completed initialization in 120s. Aborting")
             raise Exception("Hub failed to start")
 
         if isinstance(comm_q_result, str):
             logger.error(f"MonitoringRouter sent an error message: {comm_q_result}")
             raise RuntimeError(f"MonitoringRouter failed to start: {comm_q_result}")
 
         udp_port, zmq_port = comm_q_result
 
         self.monitoring_hub_url = "udp://{}:{}".format(self.hub_address, udp_port)
 
+        context = zmq.Context()
+        self.dfk_channel_timeout = 10000  # in milliseconds
+        self._dfk_channel = context.socket(zmq.DEALER)
+        self._dfk_channel.setsockopt(zmq.LINGER, 0)
+        self._dfk_channel.set_hwm(0)
+        self._dfk_channel.setsockopt(zmq.SNDTIMEO, self.dfk_channel_timeout)
+        self._dfk_channel.connect("tcp://{}:{}".format(self.hub_address, zmq_port))
+
         logger.info("Monitoring Hub initialized")
 
         return zmq_port
 
     # TODO: tighten the Any message format
     def send(self, mtype: MessageType, message: Any) -> None:
         logger.debug("Sending message type {}".format(mtype))
-        self.radio.send((mtype, message))
+        try:
+            self._dfk_channel.send_pyobj((mtype, message))
+        except zmq.Again:
+            logger.exception(
+                "The monitoring message sent from DFK to router timed-out after {}ms".format(self.dfk_channel_timeout))
 
     def close(self) -> None:
         logger.info("Terminating Monitoring Hub")
         exception_msgs = []
         while True:
             try:
                 exception_msgs.append(self.exception_q.get(block=False))
                 logger.error("There was a queued exception (Either router or DBM process got exception much earlier?)")
             except queue.Empty:
                 break
-        if self.monitoring_hub_active:
+        if self._dfk_channel and self.monitoring_hub_active:
             self.monitoring_hub_active = False
+            self._dfk_channel.close()
             if exception_msgs:
                 for exception_msg in exception_msgs:
                     logger.error(
                         "{} process delivered an exception: {}. Terminating all monitoring processes immediately.".format(
                             exception_msg[0],
                             exception_msg[1]
                         )
                     )
                 self.router_proc.terminate()
                 self.dbm_proc.terminate()
                 self.filesystem_proc.terminate()
-            logger.info("Setting router termination event")
-            self.router_exit_event.set()
             logger.info("Waiting for router to terminate")
             self.router_proc.join()
             logger.debug("Finished waiting for router termination")
             if len(exception_msgs) == 0:
                 logger.debug("Sending STOP to DBM")
                 self.priority_msgs.put(("STOP", 0))
             else:
```

### Comparing `parsl-2024.4.15/parsl/monitoring/queries/pandas.py` & `parsl-2024.4.8/parsl/monitoring/queries/pandas.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/monitoring/radios.py` & `parsl-2024.4.8/parsl/monitoring/radios.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import socket
 import pickle
 import uuid
 import logging
 
 from abc import ABCMeta, abstractmethod
 
-from multiprocessing.queues import Queue
 from typing import Optional
 
 from parsl.serialize import serialize
 
 _db_manager_excepts: Optional[Exception]
 
 
@@ -170,21 +169,7 @@
 
         try:
             self.sock.sendto(buffer, (self.ip, self.port))
         except socket.timeout:
             logging.error("Could not send message within timeout limit")
             return
         return
-
-
-class MultiprocessingQueueRadio(MonitoringRadio):
-    """A monitoring radio intended which connects over a multiprocessing Queue.
-    This radio is intended to be used on the submit side, where components
-    in the submit process, or processes launched by multiprocessing, will have
-    access to a Queue shared with the monitoring database code (bypassing the
-    monitoring router).
-    """
-    def __init__(self, queue: Queue) -> None:
-        self.queue = queue
-
-    def send(self, message: object) -> None:
-        self.queue.put((message, 0))
```

### Comparing `parsl-2024.4.15/parsl/monitoring/remote.py` & `parsl-2024.4.8/parsl/monitoring/remote.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/monitoring/router.py` & `parsl-2024.4.8/parsl/monitoring/router.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,16 +11,14 @@
 
 from parsl.log_utils import set_file_logger
 from parsl.process_loggers import wrap_with_logs
 from parsl.utils import setproctitle
 
 from parsl.monitoring.message_type import MessageType
 from parsl.monitoring.types import AddressedMonitoringMessage, TaggedMonitoringMessage
-
-from multiprocessing.synchronize import Event
 from typing import Optional, Tuple, Union
 
 
 logger = logging.getLogger(__name__)
 
 
 class MonitoringRouter:
@@ -96,18 +94,18 @@
                                                                                min_port=zmq_port_range[0],
                                                                                max_port=zmq_port_range[1])
 
     def start(self,
               priority_msgs: "queue.Queue[AddressedMonitoringMessage]",
               node_msgs: "queue.Queue[AddressedMonitoringMessage]",
               block_msgs: "queue.Queue[AddressedMonitoringMessage]",
-              resource_msgs: "queue.Queue[AddressedMonitoringMessage]",
-              exit_event: Event) -> None:
+              resource_msgs: "queue.Queue[AddressedMonitoringMessage]") -> None:
         try:
-            while not exit_event.is_set():
+            router_keep_going = True
+            while router_keep_going:
                 try:
                     data, addr = self.udp_sock.recvfrom(2048)
                     resource_msg = pickle.loads(data)
                     self.logger.debug("Got UDP Message from {}: {}".format(addr, resource_msg))
                     resource_msgs.put((resource_msg, addr))
                 except socket.timeout:
                     pass
@@ -133,14 +131,16 @@
                             resource_msgs.put(msg_0)
                         elif msg[0] == MessageType.BLOCK_INFO:
                             block_msgs.put(msg_0)
                         elif msg[0] == MessageType.TASK_INFO:
                             priority_msgs.put(msg_0)
                         elif msg[0] == MessageType.WORKFLOW_INFO:
                             priority_msgs.put(msg_0)
+                            if 'exit_now' in msg[1] and msg[1]['exit_now']:
+                                router_keep_going = False
                         else:
                             # There is a type: ignore here because if msg[0]
                             # is of the correct type, this code is unreachable,
                             # but there is no verification that the message
                             # received from zmq_receiver_channel.recv_pyobj() is actually
                             # of that type.
                             self.logger.error("Discarding message "  # type: ignore[unreachable]
@@ -174,15 +174,14 @@
 @wrap_with_logs
 def router_starter(comm_q: "queue.Queue[Union[Tuple[int, int], str]]",
                    exception_q: "queue.Queue[Tuple[str, str]]",
                    priority_msgs: "queue.Queue[AddressedMonitoringMessage]",
                    node_msgs: "queue.Queue[AddressedMonitoringMessage]",
                    block_msgs: "queue.Queue[AddressedMonitoringMessage]",
                    resource_msgs: "queue.Queue[AddressedMonitoringMessage]",
-                   exit_event: Event,
 
                    hub_address: str,
                    udp_port: Optional[int],
                    zmq_port_range: Tuple[int, int],
 
                    logdir: str,
                    logging_level: int,
@@ -199,11 +198,11 @@
         logger.error("MonitoringRouter construction failed.", exc_info=True)
         comm_q.put(f"Monitoring router construction failed: {e}")
     else:
         comm_q.put((router.udp_port, router.zmq_receiver_port))
 
         router.logger.info("Starting MonitoringRouter in router_starter")
         try:
-            router.start(priority_msgs, node_msgs, block_msgs, resource_msgs, exit_event)
+            router.start(priority_msgs, node_msgs, block_msgs, resource_msgs)
         except Exception as e:
             router.logger.exception("router.start exception")
             exception_q.put(('Hub', str(e)))
```

### Comparing `parsl-2024.4.15/parsl/monitoring/types.py` & `parsl-2024.4.8/parsl/monitoring/types.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/monitoring/visualization/app.py` & `parsl-2024.4.8/parsl/monitoring/visualization/app.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/monitoring/visualization/models.py` & `parsl-2024.4.8/parsl/monitoring/visualization/models.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/monitoring/visualization/plots/default/task_plots.py` & `parsl-2024.4.8/parsl/monitoring/visualization/plots/default/task_plots.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/monitoring/visualization/plots/default/workflow_plots.py` & `parsl-2024.4.8/parsl/monitoring/visualization/plots/default/workflow_plots.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/monitoring/visualization/plots/default/workflow_resource_plots.py` & `parsl-2024.4.8/parsl/monitoring/visualization/plots/default/workflow_resource_plots.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/monitoring/visualization/static/parsl-logo-white.png` & `parsl-2024.4.8/parsl/monitoring/visualization/static/parsl-logo-white.png`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/monitoring/visualization/templates/app.html` & `parsl-2024.4.8/parsl/monitoring/visualization/templates/app.html`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/monitoring/visualization/templates/dag.html` & `parsl-2024.4.8/parsl/monitoring/visualization/templates/dag.html`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/monitoring/visualization/templates/layout.html` & `parsl-2024.4.8/parsl/monitoring/visualization/templates/layout.html`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/monitoring/visualization/templates/resource_usage.html` & `parsl-2024.4.8/parsl/monitoring/visualization/templates/resource_usage.html`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/monitoring/visualization/templates/task.html` & `parsl-2024.4.8/parsl/monitoring/visualization/templates/task.html`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/monitoring/visualization/templates/workflow.html` & `parsl-2024.4.8/parsl/monitoring/visualization/templates/workflow.html`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/monitoring/visualization/templates/workflows_summary.html` & `parsl-2024.4.8/parsl/monitoring/visualization/templates/workflows_summary.html`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/monitoring/visualization/views.py` & `parsl-2024.4.8/parsl/monitoring/visualization/views.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/multiprocessing.py` & `parsl-2024.4.8/parsl/multiprocessing.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/process_loggers.py` & `parsl-2024.4.8/parsl/process_loggers.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/providers/__init__.py` & `parsl-2024.4.8/parsl/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/providers/ad_hoc/ad_hoc.py` & `parsl-2024.4.8/parsl/providers/ad_hoc/ad_hoc.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/providers/aws/aws.py` & `parsl-2024.4.8/parsl/providers/aws/aws.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/providers/azure/azure.py` & `parsl-2024.4.8/parsl/providers/azure/azure.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/providers/base.py` & `parsl-2024.4.8/parsl/providers/base.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/providers/cluster_provider.py` & `parsl-2024.4.8/parsl/providers/cluster_provider.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/providers/cobalt/cobalt.py` & `parsl-2024.4.8/parsl/providers/cobalt/cobalt.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/providers/condor/condor.py` & `parsl-2024.4.8/parsl/providers/condor/condor.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/providers/condor/template.py` & `parsl-2024.4.8/parsl/providers/condor/template.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/providers/errors.py` & `parsl-2024.4.8/parsl/providers/errors.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/providers/googlecloud/googlecloud.py` & `parsl-2024.4.8/parsl/providers/googlecloud/googlecloud.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/providers/grid_engine/grid_engine.py` & `parsl-2024.4.8/parsl/providers/grid_engine/grid_engine.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/providers/kubernetes/kube.py` & `parsl-2024.4.8/parsl/providers/kubernetes/kube.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/providers/local/local.py` & `parsl-2024.4.8/parsl/providers/local/local.py`

 * *Files 0% similar despite different names*

```diff
@@ -262,15 +262,15 @@
         Returns: [True]  Always returns true for every job_id, regardless of
                          whether an individual cancel failed (unless an
                          exception is raised)
         '''
         for job in job_ids:
             job_dict = self.resources[job]
             job_dict['cancelled'] = True
-            logger.debug("Terminating job/process ID: {0}".format(job))
+            logger.debug("Terminating job/proc_id: {0}".format(job))
             cmd = "kill -- -$(ps -o pgid= {} | grep -o '[0-9]*')".format(job_dict['remote_pid'])
             retcode, stdout, stderr = self.channel.execute_wait(cmd, self.cmd_timeout)
             if retcode != 0:
                 logger.warning("Failed to kill PID: {} and child processes on {}".format(job_dict['remote_pid'],
                                                                                          self.label))
 
         rets = [True for i in job_ids]
```

### Comparing `parsl-2024.4.15/parsl/providers/lsf/lsf.py` & `parsl-2024.4.8/parsl/providers/lsf/lsf.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/providers/pbspro/pbspro.py` & `parsl-2024.4.8/parsl/providers/pbspro/pbspro.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/providers/slurm/slurm.py` & `parsl-2024.4.8/parsl/providers/slurm/slurm.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/providers/torque/torque.py` & `parsl-2024.4.8/parsl/providers/torque/torque.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/serialize/base.py` & `parsl-2024.4.8/parsl/serialize/base.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/serialize/concretes.py` & `parsl-2024.4.8/parsl/serialize/concretes.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/serialize/errors.py` & `parsl-2024.4.8/parsl/serialize/errors.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/serialize/facade.py` & `parsl-2024.4.8/parsl/serialize/facade.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/serialize/proxystore.py` & `parsl-2024.4.8/parsl/serialize/proxystore.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/configs/ad_hoc_cluster_htex.py` & `parsl-2024.4.8/parsl/tests/configs/ad_hoc_cluster_htex.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/configs/azure_single_node.py` & `parsl-2024.4.8/parsl/tests/configs/azure_single_node.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/configs/bluewaters.py` & `parsl-2024.4.8/parsl/tests/configs/bluewaters.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/configs/bridges.py` & `parsl-2024.4.8/parsl/tests/configs/bridges.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/configs/cc_in2p3.py` & `parsl-2024.4.8/parsl/tests/configs/cc_in2p3.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/configs/comet.py` & `parsl-2024.4.8/parsl/tests/configs/comet.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/configs/cooley_htex.py` & `parsl-2024.4.8/parsl/tests/configs/cooley_htex.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/configs/ec2_single_node.py` & `parsl-2024.4.8/parsl/tests/configs/ec2_single_node.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/configs/ec2_spot.py` & `parsl-2024.4.8/parsl/tests/configs/ec2_spot.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/configs/frontera.py` & `parsl-2024.4.8/parsl/tests/configs/frontera.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/configs/htex_ad_hoc_cluster.py` & `parsl-2024.4.8/parsl/tests/configs/htex_ad_hoc_cluster.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/configs/htex_local.py` & `parsl-2024.4.8/parsl/tests/configs/htex_local.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/configs/htex_local_alternate.py` & `parsl-2024.4.8/parsl/tests/configs/htex_local_alternate.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,27 +27,26 @@
 from parsl.config import Config
 from parsl.executors import HighThroughputExecutor
 
 
 from parsl.data_provider.http import HTTPInTaskStaging
 from parsl.data_provider.ftp import FTPInTaskStaging
 from parsl.data_provider.file_noop import NoOpFileStaging
-from parsl.data_provider.zip import ZipFileStaging
 
 working_dir = os.getcwd() + "/" + "test_htex_alternate"
 
 
 def fresh_config():
     return Config(
         executors=[
             HighThroughputExecutor(
                 address="127.0.0.1",
                 label="htex_Local",
                 working_dir=working_dir,
-                storage_access=[ZipFileStaging(), FTPInTaskStaging(), HTTPInTaskStaging(), NoOpFileStaging()],
+                storage_access=[FTPInTaskStaging(), HTTPInTaskStaging(), NoOpFileStaging()],
                 worker_debug=True,
                 cores_per_worker=1,
                 heartbeat_period=2,
                 heartbeat_threshold=5,
                 poll_period=100,
                 encrypted=True,
                 provider=LocalProvider(
```

### Comparing `parsl-2024.4.15/parsl/tests/configs/htex_local_intask_staging.py` & `parsl-2024.4.8/parsl/tests/configs/htex_local_intask_staging.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/configs/htex_local_rsync_staging.py` & `parsl-2024.4.8/parsl/tests/configs/htex_local_rsync_staging.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/configs/local_radical_mpi.py` & `parsl-2024.4.8/parsl/tests/configs/local_radical_mpi.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/configs/local_threads_globus.py` & `parsl-2024.4.8/parsl/tests/configs/local_threads_globus.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/configs/midway.py` & `parsl-2024.4.8/parsl/tests/configs/midway.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/configs/nscc_singapore.py` & `parsl-2024.4.8/parsl/tests/configs/nscc_singapore.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/configs/osg_htex.py` & `parsl-2024.4.8/parsl/tests/configs/osg_htex.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/configs/petrelkube.py` & `parsl-2024.4.8/parsl/tests/configs/petrelkube.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/configs/summit.py` & `parsl-2024.4.8/parsl/tests/configs/summit.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/configs/swan_htex.py` & `parsl-2024.4.8/parsl/tests/configs/swan_htex.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/configs/theta.py` & `parsl-2024.4.8/parsl/tests/configs/theta.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/configs/user_opts.py` & `parsl-2024.4.8/parsl/tests/configs/user_opts.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/conftest.py` & `parsl-2024.4.8/parsl/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,35 +131,36 @@
     )
     config.addinivalue_line(
         'markers',
         'local(reason): mark test to only run locally-defined config; report will include supplied reason.'
     )
     config.addinivalue_line(
         'markers',
-        'cleannet: Enable tests that require a clean network connection (such as for testing FTP)'
+        'noci: mark test to be unsuitable for running during automated tests'
     )
+
     config.addinivalue_line(
         'markers',
-        'staging_required: Marks tests that require a staging provider, when there is no sharedFS)'
+        'cleannet: Enable tests that require a clean network connection (such as for testing FTP)'
     )
     config.addinivalue_line(
         'markers',
-        'sshd_required: Marks tests that require a SSHD'
+        'issue363: Marks tests that require a shared filesystem for stdout/stderr - see issue #363'
     )
     config.addinivalue_line(
         'markers',
-        'multiple_cores_required: Marks tests that require multiple cores, such as htex affinity'
+        'staging_required: Marks tests that require a staging provider, when there is no sharedFS)'
     )
     config.addinivalue_line(
         'markers',
-        'issue3328: Marks tests broken by issue #3328'
+        'sshd_required: Marks tests that require a SSHD'
     )
     config.addinivalue_line(
         'markers',
-        'executor_supports_std_stream_tuples: Marks tests that require tuple support for stdout/stderr'
+        'multiple_cores_required: Marks tests that require multiple cores, such as htex affinity'
     )
 
 
 @pytest.fixture(autouse=True, scope='session')
 def load_dfk_session(request, pytestconfig, tmpd_cwd_session):
     """Load a dfk around entire test suite, except in local mode.
```

### Comparing `parsl-2024.4.15/parsl/tests/integration/latency.py` & `parsl-2024.4.8/parsl/tests/integration/latency.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/integration/test_channels/test_local_channel.py` & `parsl-2024.4.8/parsl/tests/integration/test_channels/test_local_channel.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/integration/test_channels/test_scp_1.py` & `parsl-2024.4.8/parsl/tests/integration/test_channels/test_scp_1.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/integration/test_channels/test_ssh_1.py` & `parsl-2024.4.8/parsl/tests/integration/test_channels/test_ssh_1.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/integration/test_channels/test_ssh_errors.py` & `parsl-2024.4.8/parsl/tests/integration/test_channels/test_ssh_errors.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/integration/test_channels/test_ssh_file_transport.py` & `parsl-2024.4.8/parsl/tests/integration/test_channels/test_ssh_file_transport.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/integration/test_channels/test_ssh_interactive.py` & `parsl-2024.4.8/parsl/tests/integration/test_channels/test_ssh_interactive.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/integration/test_stress/test_python_simple.py` & `parsl-2024.4.8/parsl/tests/integration/test_stress/test_python_simple.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/integration/test_stress/test_python_threads.py` & `parsl-2024.4.8/parsl/tests/integration/test_stress/test_python_threads.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/manual_tests/htex_local.py` & `parsl-2024.4.8/parsl/tests/manual_tests/htex_local.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/manual_tests/test_ad_hoc_htex.py` & `parsl-2024.4.8/parsl/tests/manual_tests/test_ad_hoc_htex.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/manual_tests/test_basic.py` & `parsl-2024.4.8/parsl/tests/manual_tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/manual_tests/test_fan_in_out_htex_remote.py` & `parsl-2024.4.8/parsl/tests/manual_tests/test_fan_in_out_htex_remote.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/manual_tests/test_log_filter.py` & `parsl-2024.4.8/parsl/tests/manual_tests/test_log_filter.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/manual_tests/test_memory_limits.py` & `parsl-2024.4.8/parsl/tests/manual_tests/test_memory_limits.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/manual_tests/test_regression_220.py` & `parsl-2024.4.8/parsl/tests/manual_tests/test_regression_220.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/manual_tests/test_udp_simple.py` & `parsl-2024.4.8/parsl/tests/manual_tests/test_udp_simple.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/manual_tests/test_worker_count.py` & `parsl-2024.4.8/parsl/tests/manual_tests/test_worker_count.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/scaling_tests/htex_local.py` & `parsl-2024.4.8/parsl/tests/scaling_tests/htex_local.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/scaling_tests/test_scale.py` & `parsl-2024.4.8/parsl/tests/scaling_tests/test_scale.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/scaling_tests/wqex_condor.py` & `parsl-2024.4.8/parsl/tests/scaling_tests/wqex_condor.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/scaling_tests/wqex_local.py` & `parsl-2024.4.8/parsl/tests/scaling_tests/wqex_local.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/site_tests/site_config_selector.py` & `parsl-2024.4.8/parsl/tests/site_tests/site_config_selector.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/site_tests/test_provider.py` & `parsl-2024.4.8/parsl/tests/site_tests/test_provider.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/site_tests/test_site.py` & `parsl-2024.4.8/parsl/tests/site_tests/test_site.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/sites/test_affinity.py` & `parsl-2024.4.8/parsl/tests/sites/test_affinity.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/sites/test_concurrent.py` & `parsl-2024.4.8/parsl/tests/sites/test_concurrent.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/sites/test_dynamic_executor.py` & `parsl-2024.4.8/parsl/tests/sites/test_dynamic_executor.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/sites/test_ec2.py` & `parsl-2024.4.8/parsl/tests/sites/test_ec2.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/sites/test_local_adhoc.py` & `parsl-2024.4.8/parsl/tests/sites/test_local_adhoc.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/sites/test_worker_info.py` & `parsl-2024.4.8/parsl/tests/sites/test_worker_info.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/test_aalst_patterns.py` & `parsl-2024.4.8/parsl/tests/test_aalst_patterns.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/test_bash_apps/test_apptimeout.py` & `parsl-2024.4.8/parsl/tests/test_bash_apps/test_apptimeout.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/test_bash_apps/test_basic.py` & `parsl-2024.4.8/parsl/tests/test_bash_apps/test_basic.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import logging
 import os
 import random
 import re
 
 import pytest
 
 import parsl
@@ -20,29 +19,31 @@
 
 
 @bash_app
 def foo(x, y, z=10, stdout=None, label=None):
     return f"echo {x} {y} {z}"
 
 
+@pytest.mark.issue363
 def test_command_format_1(tmpd_cwd):
     """Testing command format for BashApps"""
 
     outdir = tmpd_cwd / "outputs"
     outdir.mkdir()
     stdout = outdir / "foo-std.out"
 
     foo_future = foo(1, 4, stdout=str(stdout))
     assert foo_future.result() == 0, "BashApp had non-zero exit code"
 
     so_content = stdout.read_text().strip()
     assert so_content == "1 4 10"
 
 
-def test_auto_log_filename_format(caplog):
+@pytest.mark.issue363
+def test_auto_log_filename_format():
     """Testing auto log filename format for BashApps
     """
     app_label = "label_test_auto_log_filename_format"
     rand_int = random.randint(1000, 1000000000)
 
     foo_future = foo(1, rand_int, stdout=parsl.AUTO_LOGNAME, label=app_label)
 
@@ -56,18 +57,16 @@
     assert os.path.exists(log_fpath), 'Output file does not exist "{0}"'.format(log_fpath)
     with open(log_fpath, 'r') as stdout_f:
         contents = stdout_f.read()
 
     assert contents == '1 {0} 10\n'.format(rand_int), \
         'Output does not match expected string "1 {0} 10", Got: "{1}"'.format(rand_int, contents)
 
-    for record in caplog.records:
-        assert record.levelno < logging.ERROR
-
 
+@pytest.mark.issue363
 def test_parallel_for(tmpd_cwd, n=3):
     """Testing a simple parallel for loop"""
     outdir = tmpd_cwd / "outputs/test_parallel"
     outdir.mkdir(parents=True)
     futs = [
         echo_to_file(
             inputs=[f"Hello World {i}"],
```

### Comparing `parsl-2024.4.15/parsl/tests/test_bash_apps/test_error_codes.py` & `parsl-2024.4.8/parsl/tests/test_bash_apps/test_error_codes.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,28 +72,30 @@
                                                                                       err_code,
                                                                                       e.exitcode)
     print(os.listdir('.'))
     os.remove('std.err')
     os.remove('std.out')
 
 
+@pytest.mark.issue363
 def test_bash_misuse(test_fn=bash_misuse):
     err_code = test_matrix[test_fn]['exit_code']
     f = test_fn()
     try:
         f.result()
     except pe.BashExitFailure as e:
         print("Caught expected BashExitFailure", e)
         assert e.exitcode == err_code, "{0} expected err_code:{1} but got {2}".format(test_fn.__name__,
                                                                                       err_code,
                                                                                       e.exitcode)
     os.remove('std.err')
     os.remove('std.out')
 
 
+@pytest.mark.issue363
 def test_command_not_found(test_fn=command_not_found):
     err_code = test_matrix[test_fn]['exit_code']
     f = test_fn()
     try:
         f.result()
     except pe.BashExitFailure as e:
         print("Caught exception", e)
@@ -102,14 +104,15 @@
                                                                                       e.exitcode)
 
     os.remove('std.err')
     os.remove('std.out')
     return True
 
 
+@pytest.mark.issue363
 def test_not_executable(test_fn=not_executable):
     err_code = test_matrix[test_fn]['exit_code']
     f = test_fn()
     try:
         f.result()
     except BashExitFailure as e:
         print("Caught exception", e)
```

### Comparing `parsl-2024.4.15/parsl/tests/test_bash_apps/test_kwarg_storage.py` & `parsl-2024.4.8/parsl/tests/test_bash_apps/test_kwarg_storage.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 
 @bash_app
 def foo(z=2, stdout=None):
     return f"echo {z}"
 
 
+@pytest.mark.issue363
 def test_command_format_1(tmpd_cwd):
     """Testing command format for BashApps
     """
 
     stdout = tmpd_cwd / "std.out"
     for exp_value, z in (
         ("3", 3),
```

### Comparing `parsl-2024.4.15/parsl/tests/test_bash_apps/test_memoize.py` & `parsl-2024.4.8/parsl/tests/test_bash_apps/test_memoize.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 def fail_on_presence(outputs=()):
     return 'if [ -f {0} ] ; then exit 1 ; else touch {0}; fi'.format(outputs[0])
 
 
 # This test is an oddity that requires a shared-FS and simply
 # won't work if there's a staging provider.
 # @pytest.mark.sharedFS_required
+@pytest.mark.issue363
 def test_bash_memoization(tmpd_cwd, n=2):
     """Testing bash memoization
     """
     mpath = tmpd_cwd / "test.memoization.tmp"
     temp_file = File(str(mpath))
     fail_on_presence(outputs=[temp_file]).result()
 
@@ -28,14 +29,15 @@
 def fail_on_presence_kw(outputs=(), foo=None):
     return 'if [ -f {0} ] ; then exit 1 ; else touch {0}; fi'.format(outputs[0])
 
 
 # This test is an oddity that requires a shared-FS and simply
 # won't work if there's a staging provider.
 # @pytest.mark.sharedFS_required
+@pytest.mark.issue363
 def test_bash_memoization_keywords(tmpd_cwd, n=2):
     """Testing bash memoization
     """
     mpath = tmpd_cwd / "test.memoization.tmp"
     temp_file = File(str(mpath))
 
     foo = {"a": 1, "b": 2}
```

### Comparing `parsl-2024.4.15/parsl/tests/test_bash_apps/test_memoize_ignore_args.py` & `parsl-2024.4.8/parsl/tests/test_bash_apps/test_memoize_ignore_args.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 
 
 @bash_app(cache=True, ignore_for_cache=['stdout'])
 def no_checkpoint_stdout_app_ignore_args(stdout=None):
     return "echo X"
 
 
+@pytest.mark.issue363
 def test_memo_stdout():
 
     # this should run and create a file named after path_x
     path_x = "test.memo.stdout.x"
     if os.path.exists(path_x):
         os.remove(path_x)
```

### Comparing `parsl-2024.4.15/parsl/tests/test_bash_apps/test_memoize_ignore_args_regr.py` & `parsl-2024.4.8/parsl/tests/test_bash_apps/test_memoize_ignore_args_regr.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 
 
 @bash_app(cache=True, ignore_for_cache=const_list_x_arg)
 def no_checkpoint_stdout_app(stdout=None):
     return "echo X"
 
 
+@pytest.mark.issue363
 def test_memo_stdout():
 
     assert const_list_x == const_list_x_arg
 
     path_x = "test.memo.stdout.x"
     if os.path.exists(path_x):
         os.remove(path_x)
```

### Comparing `parsl-2024.4.15/parsl/tests/test_bash_apps/test_multiline.py` & `parsl-2024.4.8/parsl/tests/test_bash_apps/test_multiline.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     echo {inputs[1]} &> {outputs[1]}
     echo {inputs[2]} &> {outputs[2]}
     echo "Testing STDOUT"
     echo "Testing STDERR" 1>&2
     """.format(inputs=inputs, outputs=outputs)
 
 
+@pytest.mark.issue363
 def test_multiline(tmpd_cwd):
     so, se = tmpd_cwd / "std.out", tmpd_cwd / "std.err"
     f = multiline(
         inputs=["Hello", "This is", "Cat!"],
         outputs=[
             File(str(tmpd_cwd / "hello.txt")),
             File(str(tmpd_cwd / "this.txt")),
```

### Comparing `parsl-2024.4.15/parsl/tests/test_bash_apps/test_pipeline.py` & `parsl-2024.4.8/parsl/tests/test_bash_apps/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/test_bash_apps/test_stdout.py` & `parsl-2024.4.8/parsl/tests/test_bash_apps/test_stdout.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import logging
 import os
 
 import pytest
 import typeguard
 
 import parsl.app.errors as perror
 from parsl.app.app import bash_app
@@ -32,14 +31,15 @@
     'not_a_string',
     '3tuple',
     '1tuple',
     'bad_mode'
 ]
 
 
+@pytest.mark.issue363
 @pytest.mark.parametrize('spec', speclist, ids=testids)
 def test_bad_stdout_specs(spec):
     """Testing bad stdout spec cases"""
 
     fn = echo_to_streams("Hello world", stdout=spec, stderr='t.err')
 
     try:
@@ -50,15 +50,15 @@
         # typeguard 4.x. When typeguard 2.x support is dropped, this test can
         # become an isinstance check.
         assert "TypeCheckError" in str(type(e)) or isinstance(e, TypeError) or isinstance(e, perror.BadStdStreamFile), "Exception is wrong type"
     else:
         assert False, "Did not raise expected exception"
 
 
-@pytest.mark.issue3328
+@pytest.mark.issue363
 def test_bad_stderr_file():
     """Testing bad stderr file"""
 
     err = "/bad/dir/t2.err"
 
     fn = echo_to_streams("Hello world", stderr=err)
 
@@ -68,43 +68,38 @@
         pass
     else:
         assert False, "Did not raise expected exception BadStdStreamFile"
 
     return
 
 
-@pytest.mark.executor_supports_std_stream_tuples
-def test_stdout_truncate(tmpd_cwd, caplog):
+@pytest.mark.issue363
+def test_stdout_truncate(tmpd_cwd):
     """Testing truncation of prior content of stdout"""
 
     out = (str(tmpd_cwd / 't1.out'), 'w')
     err = str(tmpd_cwd / 't1.err')
 
     echo_to_streams('hi', stdout=out, stderr=err).result()
     len1 = len(open(out[0]).readlines())
 
     echo_to_streams('hi', stdout=out, stderr=err).result()
     len2 = len(open(out[0]).readlines())
 
     assert len1 == 1
     assert len1 == len2
 
-    for record in caplog.records:
-        assert record.levelno < logging.ERROR
 
-
-def test_stdout_append(tmpd_cwd, caplog):
+@pytest.mark.issue363
+def test_stdout_append(tmpd_cwd):
     """Testing appending to prior content of stdout (default open() mode)"""
 
     out = str(tmpd_cwd / 't1.out')
     err = str(tmpd_cwd / 't1.err')
 
     echo_to_streams('hi', stdout=out, stderr=err).result()
     len1 = len(open(out).readlines())
 
     echo_to_streams('hi', stdout=out, stderr=err).result()
     len2 = len(open(out).readlines())
 
     assert len1 == 1 and len2 == 2
-
-    for record in caplog.records:
-        assert record.levelno < logging.ERROR
```

### Comparing `parsl-2024.4.15/parsl/tests/test_callables.py` & `parsl-2024.4.8/parsl/tests/test_callables.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/test_channels/test_large_output.py` & `parsl-2024.4.8/parsl/tests/test_channels/test_large_output.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/test_checkpointing/test_periodic.py` & `parsl-2024.4.8/parsl/tests/test_checkpointing/test_periodic.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/test_checkpointing/test_python_checkpoint_1.py` & `parsl-2024.4.8/parsl/tests/test_checkpointing/test_python_checkpoint_1.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/test_checkpointing/test_python_checkpoint_2.py` & `parsl-2024.4.8/parsl/tests/test_checkpointing/test_python_checkpoint_2.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/test_checkpointing/test_python_checkpoint_3.py` & `parsl-2024.4.8/parsl/tests/test_checkpointing/test_python_checkpoint_3.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/test_checkpointing/test_regression_232.py` & `parsl-2024.4.8/parsl/tests/test_checkpointing/test_regression_232.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/test_checkpointing/test_regression_233.py` & `parsl-2024.4.8/parsl/tests/test_checkpointing/test_regression_233.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/test_checkpointing/test_regression_239.py` & `parsl-2024.4.8/parsl/tests/test_checkpointing/test_regression_239.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/test_checkpointing/test_task_exit.py` & `parsl-2024.4.8/parsl/tests/test_checkpointing/test_task_exit.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/test_curvezmq.py` & `parsl-2024.4.8/parsl/tests/test_curvezmq.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/test_docs/test_from_slides.py` & `parsl-2024.4.8/parsl/tests/test_docs/test_from_slides.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/test_docs/test_kwargs.py` & `parsl-2024.4.8/parsl/tests/test_docs/test_kwargs.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/test_docs/test_tutorial_1.py` & `parsl-2024.4.8/parsl/tests/test_docs/test_tutorial_1.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/test_docs/test_workflow1.py` & `parsl-2024.4.8/parsl/tests/test_docs/test_workflow1.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/test_docs/test_workflow2.py` & `parsl-2024.4.8/parsl/tests/test_docs/test_workflow2.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/test_docs/test_workflow4.py` & `parsl-2024.4.8/parsl/tests/test_docs/test_workflow4.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/test_error_handling/test_python_walltime.py` & `parsl-2024.4.8/parsl/tests/test_error_handling/test_python_walltime.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/test_error_handling/test_rand_fail.py` & `parsl-2024.4.8/parsl/tests/test_error_handling/test_rand_fail.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/test_error_handling/test_resource_spec.py` & `parsl-2024.4.8/parsl/tests/test_error_handling/test_resource_spec.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/test_error_handling/test_retries.py` & `parsl-2024.4.8/parsl/tests/test_error_handling/test_retries.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/test_error_handling/test_retry_handler.py` & `parsl-2024.4.8/parsl/tests/test_error_handling/test_retry_handler.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/test_error_handling/test_retry_handler_failure.py` & `parsl-2024.4.8/parsl/tests/test_error_handling/test_retry_handler_failure.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/test_error_handling/test_serialization_fail.py` & `parsl-2024.4.8/parsl/tests/test_error_handling/test_serialization_fail.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/test_error_handling/test_wrap_with_logs.py` & `parsl-2024.4.8/parsl/tests/test_error_handling/test_wrap_with_logs.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/test_flux.py` & `parsl-2024.4.8/parsl/tests/test_flux.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/test_htex/test_connected_blocks.py` & `parsl-2024.4.8/parsl/tests/test_htex/test_connected_blocks.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/test_htex/test_cpu_affinity_explicit.py` & `parsl-2024.4.8/parsl/tests/test_htex/test_cpu_affinity_explicit.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/test_htex/test_disconnected_blocks.py` & `parsl-2024.4.8/parsl/tests/test_htex/test_disconnected_blocks.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/test_htex/test_drain.py` & `parsl-2024.4.8/parsl/tests/test_htex/test_drain.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/test_htex/test_htex.py` & `parsl-2024.4.8/parsl/tests/test_htex/test_htex.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/test_htex/test_manager_failure.py` & `parsl-2024.4.8/parsl/tests/test_htex/test_manager_failure.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/test_htex/test_missing_worker.py` & `parsl-2024.4.8/parsl/tests/test_htex/test_missing_worker.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/test_htex/test_multiple_disconnected_blocks.py` & `parsl-2024.4.8/parsl/tests/test_htex/test_multiple_disconnected_blocks.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/test_htex/test_worker_failure.py` & `parsl-2024.4.8/parsl/tests/test_htex/test_worker_failure.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/test_htex/test_zmq_binding.py` & `parsl-2024.4.8/parsl/tests/test_htex/test_zmq_binding.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/test_monitoring/test_app_names.py` & `parsl-2024.4.8/parsl/tests/test_monitoring/test_app_names.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/test_monitoring/test_db_locks.py` & `parsl-2024.4.8/parsl/tests/test_monitoring/test_db_locks.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/test_monitoring/test_fuzz_zmq.py` & `parsl-2024.4.8/parsl/tests/test_monitoring/test_fuzz_zmq.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import logging
 import os
 import parsl
 import pytest
 import socket
 import time
-import zmq
 
 logger = logging.getLogger(__name__)
 
 
 @parsl.python_app
 def this_app():
     return 5
@@ -45,24 +44,16 @@
     hub_zmq_port = parsl.dfk().hub_zmq_port
 
     # this will send a string to a new socket connection
     with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as s:
         s.connect((hub_address, hub_zmq_port))
         s.sendall(b'fuzzing\r')
 
-    context = zmq.Context()
-    channel_timeout = 10000  # in milliseconds
-    hub_channel = context.socket(zmq.DEALER)
-    hub_channel.setsockopt(zmq.LINGER, 0)
-    hub_channel.set_hwm(0)
-    hub_channel.setsockopt(zmq.SNDTIMEO, channel_timeout)
-    hub_channel.connect("tcp://{}:{}".format(hub_address, hub_zmq_port))
-
     # this will send a non-object down the DFK's existing ZMQ connection
-    hub_channel.send(b'FuzzyByte\rSTREAM')
+    parsl.dfk().monitoring._dfk_channel.send(b'FuzzyByte\rSTREAM')
 
     # This following attack is commented out, because monitoring is not resilient
     # to this.
     # In practice, it works some of the time but in some circumstances,
     # it would still abandon writing multiple unrelated records to the database,
     # causing ongoing monitoring data loss.
```

### Comparing `parsl-2024.4.15/parsl/tests/test_monitoring/test_htex_init_blocks_vs_monitoring.py` & `parsl-2024.4.8/parsl/tests/test_monitoring/test_htex_init_blocks_vs_monitoring.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/test_monitoring/test_incomplete_futures.py` & `parsl-2024.4.8/parsl/tests/test_monitoring/test_incomplete_futures.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/test_monitoring/test_memoization_representation.py` & `parsl-2024.4.8/parsl/tests/test_monitoring/test_memoization_representation.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/test_monitoring/test_viz_colouring.py` & `parsl-2024.4.8/parsl/tests/test_monitoring/test_viz_colouring.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/test_mpi_apps/test_bad_mpi_config.py` & `parsl-2024.4.8/parsl/tests/test_mpi_apps/test_bad_mpi_config.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/test_mpi_apps/test_mpi_mode_disabled.py` & `parsl-2024.4.8/parsl/tests/test_mpi_apps/test_mpi_mode_disabled.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/test_mpi_apps/test_mpi_mode_enabled.py` & `parsl-2024.4.8/parsl/tests/test_mpi_apps/test_mpi_mode_enabled.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/test_mpi_apps/test_mpi_prefix.py` & `parsl-2024.4.8/parsl/tests/test_mpi_apps/test_mpi_prefix.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/test_mpi_apps/test_mpi_scheduler.py` & `parsl-2024.4.8/parsl/tests/test_mpi_apps/test_mpi_scheduler.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/test_mpi_apps/test_resource_spec.py` & `parsl-2024.4.8/parsl/tests/test_mpi_apps/test_resource_spec.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/test_providers/test_local_provider.py` & `parsl-2024.4.8/parsl/tests/test_providers/test_local_provider.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/test_providers/test_pbspro_template.py` & `parsl-2024.4.8/parsl/tests/test_providers/test_pbspro_template.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/test_providers/test_slurm_template.py` & `parsl-2024.4.8/parsl/tests/test_providers/test_slurm_template.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/test_python_apps/test_arg_input_types.py` & `parsl-2024.4.8/parsl/tests/test_python_apps/test_arg_input_types.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/test_python_apps/test_basic.py` & `parsl-2024.4.8/parsl/tests/test_python_apps/test_basic.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/test_python_apps/test_context_manager.py` & `parsl-2024.4.8/parsl/tests/test_python_apps/test_context_manager.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/test_python_apps/test_dep_standard_futures.py` & `parsl-2024.4.8/parsl/tests/test_python_apps/test_dep_standard_futures.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/test_python_apps/test_depfail_propagation.py` & `parsl-2024.4.8/parsl/tests/test_python_apps/test_depfail_propagation.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/test_python_apps/test_fail.py` & `parsl-2024.4.8/parsl/tests/test_python_apps/test_fail.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/test_python_apps/test_fibonacci_iterative.py` & `parsl-2024.4.8/parsl/tests/test_python_apps/test_fibonacci_iterative.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/test_python_apps/test_fibonacci_recursive.py` & `parsl-2024.4.8/parsl/tests/test_python_apps/test_fibonacci_recursive.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/test_python_apps/test_futures.py` & `parsl-2024.4.8/parsl/tests/test_python_apps/test_futures.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/test_python_apps/test_garbage_collect.py` & `parsl-2024.4.8/parsl/tests/test_python_apps/test_garbage_collect.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/test_python_apps/test_import_fail.py` & `parsl-2024.4.8/parsl/tests/test_python_apps/test_import_fail.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/test_python_apps/test_join.py` & `parsl-2024.4.8/parsl/tests/test_python_apps/test_join.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/test_python_apps/test_lifted.py` & `parsl-2024.4.8/parsl/tests/test_python_apps/test_lifted.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/test_python_apps/test_mapred.py` & `parsl-2024.4.8/parsl/tests/test_python_apps/test_mapred.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/test_python_apps/test_memoize_1.py` & `parsl-2024.4.8/parsl/tests/test_python_apps/test_memoize_1.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/test_python_apps/test_memoize_2.py` & `parsl-2024.4.8/parsl/tests/test_python_apps/test_memoize_2.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/test_python_apps/test_memoize_4.py` & `parsl-2024.4.8/parsl/tests/test_python_apps/test_memoize_4.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/test_python_apps/test_memoize_bad_id_for_memo.py` & `parsl-2024.4.8/parsl/tests/test_python_apps/test_memoize_bad_id_for_memo.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/test_python_apps/test_memoize_ignore_args.py` & `parsl-2024.4.8/parsl/tests/test_python_apps/test_memoize_ignore_args.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/test_python_apps/test_outputs.py` & `parsl-2024.4.8/parsl/tests/test_python_apps/test_outputs.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,14 +12,15 @@
         f.write(x * 5)
     return x * 5
 
 
 whitelist = os.path.join(os.path.dirname(os.path.dirname(__file__)), 'configs', '*threads*')
 
 
+@pytest.mark.issue363
 def test_launch_apps(tmpd_cwd, n=2):
     outdir = tmpd_cwd / "outputs"
     outdir.mkdir()
 
     futs = [double(i, outputs=[File(str(outdir / f"{i}.txt"))]) for i in range(n)]
     wait(futs)
```

### Comparing `parsl-2024.4.15/parsl/tests/test_python_apps/test_pipeline.py` & `parsl-2024.4.8/parsl/tests/test_python_apps/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/test_python_apps/test_simple.py` & `parsl-2024.4.8/parsl/tests/test_python_apps/test_simple.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/test_python_apps/test_timeout.py` & `parsl-2024.4.8/parsl/tests/test_python_apps/test_timeout.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/test_python_apps/test_type5.py` & `parsl-2024.4.8/parsl/tests/test_python_apps/test_type5.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/test_radical/test_mpi_funcs.py` & `parsl-2024.4.8/parsl/tests/test_radical/test_mpi_funcs.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/test_regression/test_1480.py` & `parsl-2024.4.8/parsl/tests/test_regression/test_1480.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/test_regression/test_1606_wait_for_current_tasks.py` & `parsl-2024.4.8/parsl/tests/test_regression/test_1606_wait_for_current_tasks.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/test_regression/test_1653.py` & `parsl-2024.4.8/parsl/tests/test_regression/test_1653.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/test_regression/test_221.py` & `parsl-2024.4.8/parsl/tests/test_regression/test_221.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/test_regression/test_226.py` & `parsl-2024.4.8/parsl/tests/test_regression/test_226.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/test_regression/test_2652.py` & `parsl-2024.4.8/parsl/tests/test_regression/test_2652.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/test_regression/test_69a.py` & `parsl-2024.4.8/parsl/tests/test_regression/test_69a.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/test_regression/test_854.py` & `parsl-2024.4.8/parsl/tests/test_regression/test_854.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/test_regression/test_97_parallelism_0.py` & `parsl-2024.4.8/parsl/tests/test_regression/test_97_parallelism_0.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/test_scaling/test_block_error_handler.py` & `parsl-2024.4.8/parsl/tests/test_scaling/test_block_error_handler.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/test_scaling/test_regression_1621.py` & `parsl-2024.4.8/parsl/tests/test_scaling/test_regression_1621.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/test_scaling/test_scale_down.py` & `parsl-2024.4.8/parsl/tests/test_scaling/test_scale_down.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/test_scaling/test_scale_down_htex_auto_scale.py` & `parsl-2024.4.8/parsl/tests/test_scaling/test_scale_down_htex_auto_scale.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/test_scaling/test_scale_down_htex_unregistered.py` & `parsl-2024.4.8/parsl/tests/test_scaling/test_shutdown_scalein.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,74 +1,78 @@
-import logging
-import time
+import threading
 
 import pytest
 
 import parsl
-
-from parsl import File, python_app
-from parsl.jobs.states import JobState, TERMINAL_STATES
-from parsl.providers import LocalProvider
 from parsl.channels import LocalChannel
-from parsl.launchers import SingleNodeLauncher
 from parsl.config import Config
 from parsl.executors import HighThroughputExecutor
+from parsl.launchers import SimpleLauncher
+from parsl.providers import LocalProvider
 
-logger = logging.getLogger(__name__)
+import random
 
-_max_blocks = 1
-_min_blocks = 0
+# we need some blocks, but it doesn't matter too much how many, as long
+# as they can all start up and get registered within the try_assert
+# timeout later on.
+BLOCK_COUNT = 3
+
+
+class AccumulatingLocalProvider(LocalProvider):
+    def __init__(self, *args, **kwargs):
+        # Use a list for submitted job IDs because if there are multiple
+        # submissions returning the same job ID, this test should count
+        # those...
+        self.submit_job_ids = []
+
+        # ... but there's no requirement, I think, that cancel must be called
+        # only once per job id. What matters here is that each job ID is
+        # cancelled at least once.
+        self.cancel_job_ids = set()
+
+        super().__init__(*args, **kwargs)
+
+    def submit(self, *args, **kwargs):
+        job_id = super().submit(*args, **kwargs)
+        self.submit_job_ids.append(job_id)
+        return job_id
+
+    def cancel(self, job_ids):
+        self.cancel_job_ids.update(job_ids)
+        return super().cancel(job_ids)
 
 
-def local_config():
-    return Config(
-        executors=[
-            HighThroughputExecutor(
-                heartbeat_period=1,
-                heartbeat_threshold=2,
-                poll_period=100,
-                label="htex_local",
-                address="127.0.0.1",
-                max_workers=1,
-                encrypted=True,
-                launch_cmd="sleep inf",
-                provider=LocalProvider(
-                    channel=LocalChannel(),
-                    init_blocks=1,
-                    max_blocks=_max_blocks,
-                    min_blocks=_min_blocks,
-                    launcher=SingleNodeLauncher(),
-                ),
-            )
-        ],
-        max_idletime=0.5,
-        strategy='htex_auto_scale',
-        strategy_period=0.1
+@pytest.mark.local
+def test_shutdown_scalein_blocks(tmpd_cwd, try_assert):
+    """
+    This test scales up several blocks, and then checks that they are all
+    scaled in at DFK shutdown.
+    """
+    accumulating_provider = AccumulatingLocalProvider(
+        channel=LocalChannel(),
+        init_blocks=BLOCK_COUNT,
+        min_blocks=0,
+        max_blocks=0,
+        launcher=SimpleLauncher(),
     )
 
-
-# see issue #1885 for details of failures of this test.
-# at the time of issue #1885 this test was failing frequently
-# in CI.
-@pytest.mark.local
-def test_scaledown_with_register(try_assert):
-    dfk = parsl.dfk()
-    htex = dfk.executors['htex_local']
-
-    num_managers = len(htex.connected_managers())
-    assert num_managers == 0, "Expected 0 managers at start"
-
-    try_assert(lambda: len(htex.status()),
-               fail_msg="Expected 1 block at start")
-
-    s = htex.status()
-    assert s['0'].state == JobState.RUNNING, "Expected block to be in RUNNING"
-
-    def check_zero_blocks():
-        s = htex.status()
-        return len(s) == 1 and s['0'].state in TERMINAL_STATES
-
-    try_assert(
-        check_zero_blocks,
-        fail_msg="Expected 0 blocks after idle scaledown",
-        timeout_ms=15000,
+    htex = HighThroughputExecutor(
+               label="htex_local",
+               cores_per_worker=1,
+               provider=accumulating_provider
+           )
+
+    config = Config(
+        executors=[htex],
+        strategy='none',
+        strategy_period=0.1,
+        run_dir=str(tmpd_cwd)
     )
+
+    with parsl.load(config):
+        # this will wait for everything to be scaled out fully
+        try_assert(lambda: len(htex.connected_managers()) == BLOCK_COUNT)
+
+    parsl.clear()
+
+    assert len(accumulating_provider.submit_job_ids) == BLOCK_COUNT, f"Exactly {BLOCK_COUNT} blocks should have been launched"
+    assert len(accumulating_provider.cancel_job_ids) == BLOCK_COUNT, f"Exactly {BLOCK_COUNT} blocks should have been scaled in"
```

### Comparing `parsl-2024.4.15/parsl/tests/test_serialization/test_2555_caching_deserializer.py` & `parsl-2024.4.8/parsl/tests/test_serialization/test_2555_caching_deserializer.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/test_serialization/test_basic.py` & `parsl-2024.4.8/parsl/tests/test_serialization/test_basic.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/test_serialization/test_htex_code_cache.py` & `parsl-2024.4.8/parsl/tests/test_serialization/test_htex_code_cache.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/test_serialization/test_pack_resource_spec.py` & `parsl-2024.4.8/parsl/tests/test_serialization/test_pack_resource_spec.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/test_serialization/test_proxystore_configured.py` & `parsl-2024.4.8/parsl/tests/test_serialization/test_proxystore_configured.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/test_serialization/test_proxystore_impl.py` & `parsl-2024.4.8/parsl/tests/test_serialization/test_proxystore_impl.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/test_shutdown/test_kill_monitoring.py` & `parsl-2024.4.8/parsl/tests/test_shutdown/test_kill_monitoring.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/test_staging/staging_provider.py` & `parsl-2024.4.8/parsl/tests/test_staging/staging_provider.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/test_staging/test_1316.py` & `parsl-2024.4.8/parsl/tests/test_staging/test_1316.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/test_staging/test_docs_1.py` & `parsl-2024.4.8/parsl/tests/test_staging/test_docs_1.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/test_staging/test_elaborate_noop_file.py` & `parsl-2024.4.8/parsl/tests/test_staging/test_elaborate_noop_file.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/test_staging/test_file.py` & `parsl-2024.4.8/parsl/tests/test_staging/test_file.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/test_staging/test_file_apps.py` & `parsl-2024.4.8/parsl/tests/test_staging/test_file_apps.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/test_staging/test_file_staging.py` & `parsl-2024.4.8/parsl/tests/test_staging/test_file_staging.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/test_staging/test_output_chain_filenames.py` & `parsl-2024.4.8/parsl/tests/test_staging/test_output_chain_filenames.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/test_staging/test_staging_ftp.py` & `parsl-2024.4.8/parsl/tests/test_staging/test_staging_ftp.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/test_staging/test_staging_ftp_in_task.py` & `parsl-2024.4.8/parsl/tests/test_staging/test_staging_ftp_in_task.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/test_staging/test_staging_globus.py` & `parsl-2024.4.8/parsl/tests/test_staging/test_staging_globus.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/test_staging/test_staging_https.py` & `parsl-2024.4.8/parsl/tests/test_staging/test_staging_https.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/test_summary.py` & `parsl-2024.4.8/parsl/tests/test_summary.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/test_thread_parallelism.py` & `parsl-2024.4.8/parsl/tests/test_thread_parallelism.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/test_threads/test_configs.py` & `parsl-2024.4.8/parsl/tests/test_threads/test_configs.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/test_threads/test_lazy_errors.py` & `parsl-2024.4.8/parsl/tests/test_threads/test_lazy_errors.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/tests/test_utils/test_representation_mixin.py` & `parsl-2024.4.8/parsl/tests/test_utils/test_representation_mixin.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/usage_tracking/usage.py` & `parsl-2024.4.8/parsl/usage_tracking/usage.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl/utils.py` & `parsl-2024.4.8/parsl/utils.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.15/parsl.egg-info/PKG-INFO` & `parsl-2024.4.8/parsl.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: parsl
-Version: 2024.4.15
+Version: 2024.4.8
 Summary: Simple data dependent workflows in Python
 Home-page: https://github.com/Parsl/parsl
-Download-URL: https://github.com/Parsl/parsl/archive/2024.04.15.tar.gz
+Download-URL: https://github.com/Parsl/parsl/archive/2024.04.08.tar.gz
 Author: The Parsl Team
 Author-email: parsl@googlegroups.com
 License: Apache 2.0
 Keywords: Workflows,Scientific computing
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `parsl-2024.4.15/parsl.egg-info/SOURCES.txt` & `parsl-2024.4.8/parsl.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -66,15 +66,14 @@
 parsl/data_provider/file_noop.py
 parsl/data_provider/files.py
 parsl/data_provider/ftp.py
 parsl/data_provider/globus.py
 parsl/data_provider/http.py
 parsl/data_provider/rsync.py
 parsl/data_provider/staging.py
-parsl/data_provider/zip.py
 parsl/dataflow/__init__.py
 parsl/dataflow/dflow.py
 parsl/dataflow/errors.py
 parsl/dataflow/futures.py
 parsl/dataflow/memoization.py
 parsl/dataflow/rundirs.py
 parsl/dataflow/states.py
@@ -420,15 +419,14 @@
 parsl/tests/test_regression/test_97_parallelism_0.py
 parsl/tests/test_regression/test_98.py
 parsl/tests/test_scaling/__init__.py
 parsl/tests/test_scaling/test_block_error_handler.py
 parsl/tests/test_scaling/test_regression_1621.py
 parsl/tests/test_scaling/test_scale_down.py
 parsl/tests/test_scaling/test_scale_down_htex_auto_scale.py
-parsl/tests/test_scaling/test_scale_down_htex_unregistered.py
 parsl/tests/test_scaling/test_shutdown_scalein.py
 parsl/tests/test_serialization/__init__.py
 parsl/tests/test_serialization/test_2555_caching_deserializer.py
 parsl/tests/test_serialization/test_basic.py
 parsl/tests/test_serialization/test_htex_code_cache.py
 parsl/tests/test_serialization/test_pack_resource_spec.py
 parsl/tests/test_serialization/test_proxystore_configured.py
@@ -445,15 +443,14 @@
 parsl/tests/test_staging/test_file_apps.py
 parsl/tests/test_staging/test_file_staging.py
 parsl/tests/test_staging/test_output_chain_filenames.py
 parsl/tests/test_staging/test_staging_ftp.py
 parsl/tests/test_staging/test_staging_ftp_in_task.py
 parsl/tests/test_staging/test_staging_globus.py
 parsl/tests/test_staging/test_staging_https.py
-parsl/tests/test_staging/test_zip_out.py
 parsl/tests/test_threads/__init__.py
 parsl/tests/test_threads/test_configs.py
 parsl/tests/test_threads/test_lazy_errors.py
 parsl/tests/test_utils/__init__.py
 parsl/tests/test_utils/test_representation_mixin.py
 parsl/usage_tracking/__init__.py
 parsl/usage_tracking/usage.py
```

### Comparing `parsl-2024.4.15/parsl.egg-info/requires.txt` & `parsl-2024.4.8/parsl.egg-info/requires.txt`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 globus-sdk
 dill
 tblib
 requests
 paramiko
 psutil>=5.5.1
 setproctitle
-filelock<4,>=3.13
 
 [all]
 sqlalchemy<2,>=1.4
 pydot
 networkx<2.6,>=2.5
 Flask>=1.0.2
 flask_sqlalchemy
```

### Comparing `parsl-2024.4.15/setup.py` & `parsl-2024.4.8/setup.py`

 * *Files identical despite different names*

