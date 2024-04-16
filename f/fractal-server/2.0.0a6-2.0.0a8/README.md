# Comparing `tmp/fractal_server-2.0.0a6.tar.gz` & `tmp/fractal_server-2.0.0a8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fractal_server-2.0.0a6.tar", max compression
+gzip compressed data, was "fractal_server-2.0.0a8.tar", max compression
```

## Comparing `fractal_server-2.0.0a6.tar` & `fractal_server-2.0.0a8.tar`

### file list

```diff
@@ -1,164 +1,165 @@
--rw-r--r--   0        0        0     1576 2024-04-12 08:51:36.536906 fractal_server-2.0.0a6/LICENSE
--rw-r--r--   0        0        0     2466 2024-04-12 08:51:36.536906 fractal_server-2.0.0a6/README.md
--rw-r--r--   0        0        0       24 2024-04-12 08:51:36.540906 fractal_server-2.0.0a6/fractal_server/__init__.py
--rw-r--r--   0        0        0     4958 2024-04-12 08:51:36.540906 fractal_server-2.0.0a6/fractal_server/__main__.py
--rw-r--r--   0        0        0     3153 2024-04-12 08:51:36.540906 fractal_server-2.0.0a6/fractal_server/alembic.ini
--rw-r--r--   0        0        0        0 2024-04-12 08:51:36.540906 fractal_server-2.0.0a6/fractal_server/app/__init__.py
--rw-r--r--   0        0        0     4042 2024-04-12 08:51:36.540906 fractal_server-2.0.0a6/fractal_server/app/db/__init__.py
--rw-r--r--   0        0        0      183 2024-04-12 08:51:36.540906 fractal_server-2.0.0a6/fractal_server/app/models/__init__.py
--rw-r--r--   0        0        0      567 2024-04-12 08:51:36.540906 fractal_server-2.0.0a6/fractal_server/app/models/linkuserproject.py
--rw-r--r--   0        0        0     3378 2024-04-12 08:51:36.540906 fractal_server-2.0.0a6/fractal_server/app/models/security.py
--rw-r--r--   0        0        0     1090 2024-04-12 08:51:36.540906 fractal_server-2.0.0a6/fractal_server/app/models/state.py
--rw-r--r--   0        0        0      413 2024-04-12 08:51:36.540906 fractal_server-2.0.0a6/fractal_server/app/models/v1/__init__.py
--rw-r--r--   0        0        0     2017 2024-04-12 08:51:36.540906 fractal_server-2.0.0a6/fractal_server/app/models/v1/dataset.py
--rw-r--r--   0        0        0     3304 2024-04-12 08:51:36.540906 fractal_server-2.0.0a6/fractal_server/app/models/v1/job.py
--rw-r--r--   0        0        0      859 2024-04-12 08:51:36.540906 fractal_server-2.0.0a6/fractal_server/app/models/v1/project.py
--rw-r--r--   0        0        0     2782 2024-04-12 08:51:36.540906 fractal_server-2.0.0a6/fractal_server/app/models/v1/task.py
--rw-r--r--   0        0        0     3950 2024-04-12 08:51:36.540906 fractal_server-2.0.0a6/fractal_server/app/models/v1/workflow.py
--rw-r--r--   0        0        0      400 2024-04-12 08:51:36.540906 fractal_server-2.0.0a6/fractal_server/app/models/v2/__init__.py
--rw-r--r--   0        0        0     1455 2024-04-12 08:51:36.540906 fractal_server-2.0.0a6/fractal_server/app/models/v2/dataset.py
--rw-r--r--   0        0        0     1535 2024-04-12 08:51:36.540906 fractal_server-2.0.0a6/fractal_server/app/models/v2/job.py
--rw-r--r--   0        0        0      817 2024-04-12 08:51:36.540906 fractal_server-2.0.0a6/fractal_server/app/models/v2/project.py
--rw-r--r--   0        0        0     3257 2024-04-12 08:51:36.540906 fractal_server-2.0.0a6/fractal_server/app/models/v2/task.py
--rw-r--r--   0        0        0     1256 2024-04-12 08:51:36.540906 fractal_server-2.0.0a6/fractal_server/app/models/v2/workflow.py
--rw-r--r--   0        0        0     2727 2024-04-12 08:51:36.540906 fractal_server-2.0.0a6/fractal_server/app/models/v2/workflowtask.py
--rw-r--r--   0        0        0        0 2024-04-12 08:51:36.540906 fractal_server-2.0.0a6/fractal_server/app/routes/__init__.py
--rw-r--r--   0        0        0        0 2024-04-12 08:51:36.540906 fractal_server-2.0.0a6/fractal_server/app/routes/admin/__init__.py
--rw-r--r--   0        0        0    13981 2024-04-12 08:51:36.540906 fractal_server-2.0.0a6/fractal_server/app/routes/admin/v1.py
--rw-r--r--   0        0        0     9826 2024-04-12 08:51:36.540906 fractal_server-2.0.0a6/fractal_server/app/routes/admin/v2.py
--rw-r--r--   0        0        0      315 2024-04-12 08:51:36.540906 fractal_server-2.0.0a6/fractal_server/app/routes/api/__init__.py
--rw-r--r--   0        0        0      958 2024-04-12 08:51:36.540906 fractal_server-2.0.0a6/fractal_server/app/routes/api/v1/__init__.py
--rw-r--r--   0        0        0    11955 2024-04-12 08:51:36.540906 fractal_server-2.0.0a6/fractal_server/app/routes/api/v1/_aux_functions.py
--rw-r--r--   0        0        0    16911 2024-04-12 08:51:36.540906 fractal_server-2.0.0a6/fractal_server/app/routes/api/v1/dataset.py
--rw-r--r--   0        0        0     5436 2024-04-12 08:51:36.540906 fractal_server-2.0.0a6/fractal_server/app/routes/api/v1/job.py
--rw-r--r--   0        0        0    15765 2024-04-12 08:51:36.540906 fractal_server-2.0.0a6/fractal_server/app/routes/api/v1/project.py
--rw-r--r--   0        0        0     6123 2024-04-12 08:51:36.540906 fractal_server-2.0.0a6/fractal_server/app/routes/api/v1/task.py
--rw-r--r--   0        0        0     8873 2024-04-12 08:51:36.540906 fractal_server-2.0.0a6/fractal_server/app/routes/api/v1/task_collection.py
--rw-r--r--   0        0        0    10930 2024-04-12 08:51:36.540906 fractal_server-2.0.0a6/fractal_server/app/routes/api/v1/workflow.py
--rw-r--r--   0        0        0     5579 2024-04-12 08:51:36.540906 fractal_server-2.0.0a6/fractal_server/app/routes/api/v1/workflowtask.py
--rw-r--r--   0        0        0     1373 2024-04-12 08:51:36.540906 fractal_server-2.0.0a6/fractal_server/app/routes/api/v2/__init__.py
--rw-r--r--   0        0        0    14301 2024-04-12 08:51:36.540906 fractal_server-2.0.0a6/fractal_server/app/routes/api/v2/_aux_functions.py
--rw-r--r--   0        0        0     9680 2024-04-12 08:51:36.540906 fractal_server-2.0.0a6/fractal_server/app/routes/api/v2/dataset.py
--rw-r--r--   0        0        0     5956 2024-04-12 08:51:36.540906 fractal_server-2.0.0a6/fractal_server/app/routes/api/v2/images.py
--rw-r--r--   0        0        0     5334 2024-04-12 08:51:36.540906 fractal_server-2.0.0a6/fractal_server/app/routes/api/v2/job.py
--rw-r--r--   0        0        0     6024 2024-04-12 08:51:36.540906 fractal_server-2.0.0a6/fractal_server/app/routes/api/v2/project.py
--rw-r--r--   0        0        0     6901 2024-04-12 08:51:36.540906 fractal_server-2.0.0a6/fractal_server/app/routes/api/v2/submit.py
--rw-r--r--   0        0        0     7130 2024-04-12 08:51:36.540906 fractal_server-2.0.0a6/fractal_server/app/routes/api/v2/task.py
--rw-r--r--   0        0        0     8904 2024-04-12 08:51:36.540906 fractal_server-2.0.0a6/fractal_server/app/routes/api/v2/task_collection.py
--rw-r--r--   0        0        0     1628 2024-04-12 08:51:36.540906 fractal_server-2.0.0a6/fractal_server/app/routes/api/v2/task_legacy.py
--rw-r--r--   0        0        0    11845 2024-04-12 08:51:36.540906 fractal_server-2.0.0a6/fractal_server/app/routes/api/v2/workflow.py
--rw-r--r--   0        0        0     8414 2024-04-12 08:51:36.540906 fractal_server-2.0.0a6/fractal_server/app/routes/api/v2/workflowtask.py
--rw-r--r--   0        0        0     4885 2024-04-12 08:51:36.540906 fractal_server-2.0.0a6/fractal_server/app/routes/auth.py
--rw-r--r--   0        0        0        0 2024-04-12 08:51:36.540906 fractal_server-2.0.0a6/fractal_server/app/routes/aux/__init__.py
--rw-r--r--   0        0        0     1248 2024-04-12 08:51:36.540906 fractal_server-2.0.0a6/fractal_server/app/routes/aux/_job.py
--rw-r--r--   0        0        0      675 2024-04-12 08:51:36.540906 fractal_server-2.0.0a6/fractal_server/app/routes/aux/_runner.py
--rw-r--r--   0        0        0       16 2024-04-12 08:51:36.540906 fractal_server-2.0.0a6/fractal_server/app/runner/.gitignore
--rw-r--r--   0        0        0        0 2024-04-12 08:51:36.540906 fractal_server-2.0.0a6/fractal_server/app/runner/__init__.py
--rw-r--r--   0        0        0      829 2024-04-12 08:51:36.540906 fractal_server-2.0.0a6/fractal_server/app/runner/async_wrap.py
--rw-r--r--   0        0        0      119 2024-04-12 08:51:36.540906 fractal_server-2.0.0a6/fractal_server/app/runner/components.py
--rw-r--r--   0        0        0     4159 2024-04-12 08:51:36.540906 fractal_server-2.0.0a6/fractal_server/app/runner/exceptions.py
--rw-r--r--   0        0        0        0 2024-04-12 08:51:36.540906 fractal_server-2.0.0a6/fractal_server/app/runner/executors/__init__.py
--rw-r--r--   0        0        0       65 2024-04-12 08:51:36.540906 fractal_server-2.0.0a6/fractal_server/app/runner/executors/slurm/__init__.py
--rw-r--r--   0        0        0     8841 2024-04-12 08:51:36.540906 fractal_server-2.0.0a6/fractal_server/app/runner/executors/slurm/_batching.py
--rw-r--r--   0        0        0     1908 2024-04-12 08:51:36.540906 fractal_server-2.0.0a6/fractal_server/app/runner/executors/slurm/_check_jobs_status.py
--rw-r--r--   0        0        0     4421 2024-04-12 08:51:36.540906 fractal_server-2.0.0a6/fractal_server/app/runner/executors/slurm/_executor_wait_thread.py
--rw-r--r--   0        0        0    15552 2024-04-12 08:51:36.540906 fractal_server-2.0.0a6/fractal_server/app/runner/executors/slurm/_slurm_config.py
--rw-r--r--   0        0        0     5123 2024-04-12 08:51:36.544906 fractal_server-2.0.0a6/fractal_server/app/runner/executors/slurm/_subprocess_run_as_user.py
--rw-r--r--   0        0        0    44451 2024-04-12 08:51:36.544906 fractal_server-2.0.0a6/fractal_server/app/runner/executors/slurm/executor.py
--rw-r--r--   0        0        0     5852 2024-04-12 08:51:36.544906 fractal_server-2.0.0a6/fractal_server/app/runner/executors/slurm/remote.py
--rw-r--r--   0        0        0      206 2024-04-12 08:51:36.544906 fractal_server-2.0.0a6/fractal_server/app/runner/filenames.py
--rw-r--r--   0        0        0     1254 2024-04-12 08:51:36.544906 fractal_server-2.0.0a6/fractal_server/app/runner/set_start_and_last_task_index.py
--rw-r--r--   0        0        0     3219 2024-04-12 08:51:36.544906 fractal_server-2.0.0a6/fractal_server/app/runner/task_files.py
--rw-r--r--   0        0        0    13608 2024-04-12 08:51:36.544906 fractal_server-2.0.0a6/fractal_server/app/runner/v1/__init__.py
--rw-r--r--   0        0        0    21240 2024-04-12 08:51:36.544906 fractal_server-2.0.0a6/fractal_server/app/runner/v1/_common.py
--rw-r--r--   0        0        0     6926 2024-04-12 08:51:36.544906 fractal_server-2.0.0a6/fractal_server/app/runner/v1/_local/__init__.py
--rw-r--r--   0        0        0     3147 2024-04-12 08:51:36.544906 fractal_server-2.0.0a6/fractal_server/app/runner/v1/_local/_local_config.py
--rw-r--r--   0        0        0     1493 2024-04-12 08:51:36.544906 fractal_server-2.0.0a6/fractal_server/app/runner/v1/_local/_submit_setup.py
--rw-r--r--   0        0        0     3620 2024-04-12 08:51:36.544906 fractal_server-2.0.0a6/fractal_server/app/runner/v1/_local/executor.py
--rw-r--r--   0        0        0    10853 2024-04-12 08:51:36.544906 fractal_server-2.0.0a6/fractal_server/app/runner/v1/_slurm/__init__.py
--rw-r--r--   0        0        0     2738 2024-04-12 08:51:36.544906 fractal_server-2.0.0a6/fractal_server/app/runner/v1/_slurm/_submit_setup.py
--rw-r--r--   0        0        0     5977 2024-04-12 08:51:36.544906 fractal_server-2.0.0a6/fractal_server/app/runner/v1/_slurm/get_slurm_config.py
--rw-r--r--   0        0        0     3294 2024-04-12 08:51:36.544906 fractal_server-2.0.0a6/fractal_server/app/runner/v1/common.py
--rw-r--r--   0        0        0     4684 2024-04-12 08:51:36.544906 fractal_server-2.0.0a6/fractal_server/app/runner/v1/handle_failed_job.py
--rw-r--r--   0        0        0    12482 2024-04-12 08:51:36.544906 fractal_server-2.0.0a6/fractal_server/app/runner/v2/__init__.py
--rw-r--r--   0        0        0     5881 2024-04-12 08:51:36.544906 fractal_server-2.0.0a6/fractal_server/app/runner/v2/_local/__init__.py
--rw-r--r--   0        0        0     3630 2024-04-12 08:51:36.544906 fractal_server-2.0.0a6/fractal_server/app/runner/v2/_local/_local_config.py
--rw-r--r--   0        0        0     1614 2024-04-12 08:51:36.544906 fractal_server-2.0.0a6/fractal_server/app/runner/v2/_local/_submit_setup.py
--rw-r--r--   0        0        0     3620 2024-04-12 08:51:36.544906 fractal_server-2.0.0a6/fractal_server/app/runner/v2/_local/executor.py
--rw-r--r--   0        0        0     4409 2024-04-12 08:51:36.544906 fractal_server-2.0.0a6/fractal_server/app/runner/v2/_slurm/__init__.py
--rw-r--r--   0        0        0     2793 2024-04-12 08:51:36.544906 fractal_server-2.0.0a6/fractal_server/app/runner/v2/_slurm/_submit_setup.py
--rw-r--r--   0        0        0     6621 2024-04-12 08:51:36.544906 fractal_server-2.0.0a6/fractal_server/app/runner/v2/_slurm/get_slurm_config.py
--rw-r--r--   0        0        0      639 2024-04-12 08:51:36.544906 fractal_server-2.0.0a6/fractal_server/app/runner/v2/deduplicate_list.py
--rw-r--r--   0        0        0     5202 2024-04-12 08:51:36.544906 fractal_server-2.0.0a6/fractal_server/app/runner/v2/handle_failed_job.py
--rw-r--r--   0        0        0     1281 2024-04-12 08:51:36.544906 fractal_server-2.0.0a6/fractal_server/app/runner/v2/merge_outputs.py
--rw-r--r--   0        0        0    11784 2024-04-12 08:51:36.544906 fractal_server-2.0.0a6/fractal_server/app/runner/v2/runner.py
--rw-r--r--   0        0        0    10087 2024-04-12 08:51:36.544906 fractal_server-2.0.0a6/fractal_server/app/runner/v2/runner_functions.py
--rw-r--r--   0        0        0     3845 2024-04-12 08:51:36.544906 fractal_server-2.0.0a6/fractal_server/app/runner/v2/runner_functions_low_level.py
--rw-r--r--   0        0        0     1410 2024-04-12 08:51:36.544906 fractal_server-2.0.0a6/fractal_server/app/runner/v2/task_interface.py
--rw-r--r--   0        0        0      511 2024-04-12 08:51:36.544906 fractal_server-2.0.0a6/fractal_server/app/runner/v2/v1_compat.py
--rw-r--r--   0        0        0      157 2024-04-12 08:51:36.544906 fractal_server-2.0.0a6/fractal_server/app/schemas/__init__.py
--rw-r--r--   0        0        0     3264 2024-04-12 08:51:36.544906 fractal_server-2.0.0a6/fractal_server/app/schemas/_validators.py
--rw-r--r--   0        0        0      692 2024-04-12 08:51:36.544906 fractal_server-2.0.0a6/fractal_server/app/schemas/state.py
--rw-r--r--   0        0        0     3113 2024-04-12 08:51:36.544906 fractal_server-2.0.0a6/fractal_server/app/schemas/user.py
--rw-r--r--   0        0        0     2078 2024-04-12 08:51:36.544906 fractal_server-2.0.0a6/fractal_server/app/schemas/v1/__init__.py
--rw-r--r--   0        0        0     4302 2024-04-12 08:51:36.544906 fractal_server-2.0.0a6/fractal_server/app/schemas/v1/applyworkflow.py
--rw-r--r--   0        0        0     3444 2024-04-12 08:51:36.544906 fractal_server-2.0.0a6/fractal_server/app/schemas/v1/dataset.py
--rw-r--r--   0        0        0     1274 2024-04-12 08:51:36.544906 fractal_server-2.0.0a6/fractal_server/app/schemas/v1/dumps.py
--rw-r--r--   0        0        0     3829 2024-04-12 08:51:36.544906 fractal_server-2.0.0a6/fractal_server/app/schemas/v1/manifest.py
--rw-r--r--   0        0        0     1218 2024-04-12 08:51:36.544906 fractal_server-2.0.0a6/fractal_server/app/schemas/v1/project.py
--rw-r--r--   0        0        0     3704 2024-04-12 08:51:36.544906 fractal_server-2.0.0a6/fractal_server/app/schemas/v1/task.py
--rw-r--r--   0        0        0     3057 2024-04-12 08:51:36.544906 fractal_server-2.0.0a6/fractal_server/app/schemas/v1/task_collection.py
--rw-r--r--   0        0        0     4618 2024-04-12 08:51:36.544906 fractal_server-2.0.0a6/fractal_server/app/schemas/v1/workflow.py
--rw-r--r--   0        0        0     1752 2024-04-12 08:51:36.544906 fractal_server-2.0.0a6/fractal_server/app/schemas/v2/__init__.py
--rw-r--r--   0        0        0     1757 2024-04-12 08:51:36.544906 fractal_server-2.0.0a6/fractal_server/app/schemas/v2/dataset.py
--rw-r--r--   0        0        0     1997 2024-04-12 08:51:36.544906 fractal_server-2.0.0a6/fractal_server/app/schemas/v2/dumps.py
--rw-r--r--   0        0        0     3250 2024-04-12 08:51:36.544906 fractal_server-2.0.0a6/fractal_server/app/schemas/v2/job.py
--rw-r--r--   0        0        0     6243 2024-04-12 08:51:36.544906 fractal_server-2.0.0a6/fractal_server/app/schemas/v2/manifest.py
--rw-r--r--   0        0        0      736 2024-04-12 08:51:36.544906 fractal_server-2.0.0a6/fractal_server/app/schemas/v2/project.py
--rw-r--r--   0        0        0     4672 2024-04-12 08:51:36.544906 fractal_server-2.0.0a6/fractal_server/app/schemas/v2/task.py
--rw-r--r--   0        0        0     3171 2024-04-12 08:51:36.544906 fractal_server-2.0.0a6/fractal_server/app/schemas/v2/task_collection.py
--rw-r--r--   0        0        0     1827 2024-04-12 08:51:36.544906 fractal_server-2.0.0a6/fractal_server/app/schemas/v2/workflow.py
--rw-r--r--   0        0        0     5051 2024-04-12 08:51:36.544906 fractal_server-2.0.0a6/fractal_server/app/schemas/v2/workflowtask.py
--rw-r--r--   0        0        0    11203 2024-04-12 08:51:36.544906 fractal_server-2.0.0a6/fractal_server/app/security/__init__.py
--rw-r--r--   0        0        0    15080 2024-04-12 08:51:36.544906 fractal_server-2.0.0a6/fractal_server/config.py
--rw-r--r--   0        0        0      398 2024-04-12 08:51:36.544906 fractal_server-2.0.0a6/fractal_server/data_migrations/README.md
--rw-r--r--   0        0        0      144 2024-04-12 08:51:36.544906 fractal_server-2.0.0a6/fractal_server/images/__init__.py
--rw-r--r--   0        0        0     2904 2024-04-12 08:51:36.544906 fractal_server-2.0.0a6/fractal_server/images/models.py
--rw-r--r--   0        0        0     2234 2024-04-12 08:51:36.544906 fractal_server-2.0.0a6/fractal_server/images/tools.py
--rw-r--r--   0        0        0     3924 2024-04-12 08:51:36.544906 fractal_server-2.0.0a6/fractal_server/logger.py
--rw-r--r--   0        0        0     3001 2024-04-12 08:51:36.544906 fractal_server-2.0.0a6/fractal_server/main.py
--rw-r--r--   0        0        0       59 2024-04-12 08:51:36.548905 fractal_server-2.0.0a6/fractal_server/migrations/README
--rw-r--r--   0        0        0     2630 2024-04-12 08:51:36.548905 fractal_server-2.0.0a6/fractal_server/migrations/env.py
--rw-r--r--   0        0        0      526 2024-04-12 08:51:36.548905 fractal_server-2.0.0a6/fractal_server/migrations/script.py.mako
--rw-r--r--   0        0        0      954 2024-04-12 08:51:36.548905 fractal_server-2.0.0a6/fractal_server/migrations/versions/4c308bcaea2b_add_task_args_schema_and_task_args_.py
--rw-r--r--   0        0        0     1157 2024-04-12 08:51:36.548905 fractal_server-2.0.0a6/fractal_server/migrations/versions/4cedeb448a53_workflowtask_foreign_keys_not_nullables.py
--rw-r--r--   0        0        0     8770 2024-04-12 08:51:36.548905 fractal_server-2.0.0a6/fractal_server/migrations/versions/50a13d6138fd_initial_schema.py
--rw-r--r--   0        0        0     1632 2024-04-12 08:51:36.548905 fractal_server-2.0.0a6/fractal_server/migrations/versions/70e77f1c38b0_add_applyworkflow_first_task_index_and_.py
--rw-r--r--   0        0        0     1353 2024-04-12 08:51:36.548905 fractal_server-2.0.0a6/fractal_server/migrations/versions/71eefd1dd202_add_slurm_accounts.py
--rw-r--r--   0        0        0     8116 2024-04-12 08:51:36.548905 fractal_server-2.0.0a6/fractal_server/migrations/versions/80e12e1bc4fd_v2.py
--rw-r--r--   0        0        0     2684 2024-04-12 08:51:36.548905 fractal_server-2.0.0a6/fractal_server/migrations/versions/84bf0fffde30_add_dumps_to_applyworkflow.py
--rw-r--r--   0        0        0     1115 2024-04-12 08:51:36.548905 fractal_server-2.0.0a6/fractal_server/migrations/versions/8f79bd162e35_add_docs_info_and_docs_link_to_task_.py
--rw-r--r--   0        0        0     1057 2024-04-12 08:51:36.548905 fractal_server-2.0.0a6/fractal_server/migrations/versions/97f444d47249_add_applyworkflow_project_dump.py
--rw-r--r--   0        0        0      883 2024-04-12 08:51:36.548905 fractal_server-2.0.0a6/fractal_server/migrations/versions/99ea79d9e5d2_add_dataset_history.py
--rw-r--r--   0        0        0     1849 2024-04-12 08:51:36.548905 fractal_server-2.0.0a6/fractal_server/migrations/versions/9fd26a2b0de4_add_workflow_timestamp_created.py
--rw-r--r--   0        0        0      867 2024-04-12 08:51:36.548905 fractal_server-2.0.0a6/fractal_server/migrations/versions/a7f4d6137b53_add_workflow_dump_to_applyworkflow.py
--rw-r--r--   0        0        0      949 2024-04-12 08:51:36.548905 fractal_server-2.0.0a6/fractal_server/migrations/versions/d4fe3708d309_make_applyworkflow_workflow_dump_non_.py
--rw-r--r--   0        0        0      963 2024-04-12 08:51:36.548905 fractal_server-2.0.0a6/fractal_server/migrations/versions/e75cac726012_make_applyworkflow_start_timestamp_not_.py
--rw-r--r--   0        0        0     1221 2024-04-12 08:51:36.548905 fractal_server-2.0.0a6/fractal_server/migrations/versions/efa89c30e0a4_add_project_timestamp_created.py
--rw-r--r--   0        0        0      746 2024-04-12 08:51:36.548905 fractal_server-2.0.0a6/fractal_server/migrations/versions/f384e1c0cf5d_drop_task_default_args_columns.py
--rw-r--r--   0        0        0        0 2024-04-12 08:51:36.548905 fractal_server-2.0.0a6/fractal_server/py.typed
--rw-r--r--   0        0        0     2786 2024-04-12 08:51:36.548905 fractal_server-2.0.0a6/fractal_server/syringe.py
--rw-r--r--   0        0        0       23 2024-04-12 08:51:36.548905 fractal_server-2.0.0a6/fractal_server/tasks/__init__.py
--rw-r--r--   0        0        0     5379 2024-04-12 08:51:36.548905 fractal_server-2.0.0a6/fractal_server/tasks/endpoint_operations.py
--rw-r--r--   0        0        0     3278 2024-04-12 08:51:36.548905 fractal_server-2.0.0a6/fractal_server/tasks/utils.py
--rw-r--r--   0        0        0     3775 2024-04-12 08:51:36.548905 fractal_server-2.0.0a6/fractal_server/tasks/v1/_TaskCollectPip.py
--rw-r--r--   0        0        0        0 2024-04-12 08:51:36.548905 fractal_server-2.0.0a6/fractal_server/tasks/v1/__init__.py
--rw-r--r--   0        0        0    11725 2024-04-12 08:51:36.548905 fractal_server-2.0.0a6/fractal_server/tasks/v1/background_operations.py
--rw-r--r--   0        0        0      502 2024-04-12 08:51:36.548905 fractal_server-2.0.0a6/fractal_server/tasks/v1/get_collection_data.py
--rw-r--r--   0        0        0     3775 2024-04-12 08:51:36.548905 fractal_server-2.0.0a6/fractal_server/tasks/v2/_TaskCollectPip.py
--rw-r--r--   0        0        0        0 2024-04-12 08:51:36.548905 fractal_server-2.0.0a6/fractal_server/tasks/v2/__init__.py
--rw-r--r--   0        0        0    12803 2024-04-12 08:51:36.548905 fractal_server-2.0.0a6/fractal_server/tasks/v2/background_operations.py
--rw-r--r--   0        0        0      502 2024-04-12 08:51:36.548905 fractal_server-2.0.0a6/fractal_server/tasks/v2/get_collection_data.py
--rw-r--r--   0        0        0     2115 2024-04-12 08:51:36.548905 fractal_server-2.0.0a6/fractal_server/utils.py
--rw-r--r--   0        0        0     2999 2024-04-12 08:51:36.548905 fractal_server-2.0.0a6/pyproject.toml
--rw-r--r--   0        0        0     4204 1970-01-01 00:00:00.000000 fractal_server-2.0.0a6/PKG-INFO
+-rw-r--r--   0        0        0     1576 2024-04-16 09:44:55.210574 fractal_server-2.0.0a8/LICENSE
+-rw-r--r--   0        0        0     2466 2024-04-16 09:44:55.210574 fractal_server-2.0.0a8/README.md
+-rw-r--r--   0        0        0       24 2024-04-16 09:44:55.214574 fractal_server-2.0.0a8/fractal_server/__init__.py
+-rw-r--r--   0        0        0     4958 2024-04-16 09:44:55.214574 fractal_server-2.0.0a8/fractal_server/__main__.py
+-rw-r--r--   0        0        0     3153 2024-04-16 09:44:55.214574 fractal_server-2.0.0a8/fractal_server/alembic.ini
+-rw-r--r--   0        0        0        0 2024-04-16 09:44:55.214574 fractal_server-2.0.0a8/fractal_server/app/__init__.py
+-rw-r--r--   0        0        0     4042 2024-04-16 09:44:55.214574 fractal_server-2.0.0a8/fractal_server/app/db/__init__.py
+-rw-r--r--   0        0        0      183 2024-04-16 09:44:55.214574 fractal_server-2.0.0a8/fractal_server/app/models/__init__.py
+-rw-r--r--   0        0        0      567 2024-04-16 09:44:55.214574 fractal_server-2.0.0a8/fractal_server/app/models/linkuserproject.py
+-rw-r--r--   0        0        0     3378 2024-04-16 09:44:55.214574 fractal_server-2.0.0a8/fractal_server/app/models/security.py
+-rw-r--r--   0        0        0     1090 2024-04-16 09:44:55.214574 fractal_server-2.0.0a8/fractal_server/app/models/state.py
+-rw-r--r--   0        0        0      413 2024-04-16 09:44:55.214574 fractal_server-2.0.0a8/fractal_server/app/models/v1/__init__.py
+-rw-r--r--   0        0        0     2017 2024-04-16 09:44:55.214574 fractal_server-2.0.0a8/fractal_server/app/models/v1/dataset.py
+-rw-r--r--   0        0        0     3304 2024-04-16 09:44:55.214574 fractal_server-2.0.0a8/fractal_server/app/models/v1/job.py
+-rw-r--r--   0        0        0      859 2024-04-16 09:44:55.214574 fractal_server-2.0.0a8/fractal_server/app/models/v1/project.py
+-rw-r--r--   0        0        0     2782 2024-04-16 09:44:55.214574 fractal_server-2.0.0a8/fractal_server/app/models/v1/task.py
+-rw-r--r--   0        0        0     3950 2024-04-16 09:44:55.214574 fractal_server-2.0.0a8/fractal_server/app/models/v1/workflow.py
+-rw-r--r--   0        0        0      400 2024-04-16 09:44:55.214574 fractal_server-2.0.0a8/fractal_server/app/models/v2/__init__.py
+-rw-r--r--   0        0        0     1455 2024-04-16 09:44:55.214574 fractal_server-2.0.0a8/fractal_server/app/models/v2/dataset.py
+-rw-r--r--   0        0        0     1535 2024-04-16 09:44:55.214574 fractal_server-2.0.0a8/fractal_server/app/models/v2/job.py
+-rw-r--r--   0        0        0      817 2024-04-16 09:44:55.214574 fractal_server-2.0.0a8/fractal_server/app/models/v2/project.py
+-rw-r--r--   0        0        0     3257 2024-04-16 09:44:55.214574 fractal_server-2.0.0a8/fractal_server/app/models/v2/task.py
+-rw-r--r--   0        0        0     1256 2024-04-16 09:44:55.214574 fractal_server-2.0.0a8/fractal_server/app/models/v2/workflow.py
+-rw-r--r--   0        0        0     2727 2024-04-16 09:44:55.214574 fractal_server-2.0.0a8/fractal_server/app/models/v2/workflowtask.py
+-rw-r--r--   0        0        0        0 2024-04-16 09:44:55.214574 fractal_server-2.0.0a8/fractal_server/app/routes/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-16 09:44:55.214574 fractal_server-2.0.0a8/fractal_server/app/routes/admin/__init__.py
+-rw-r--r--   0        0        0    13981 2024-04-16 09:44:55.214574 fractal_server-2.0.0a8/fractal_server/app/routes/admin/v1.py
+-rw-r--r--   0        0        0     9826 2024-04-16 09:44:55.214574 fractal_server-2.0.0a8/fractal_server/app/routes/admin/v2.py
+-rw-r--r--   0        0        0      315 2024-04-16 09:44:55.214574 fractal_server-2.0.0a8/fractal_server/app/routes/api/__init__.py
+-rw-r--r--   0        0        0      958 2024-04-16 09:44:55.214574 fractal_server-2.0.0a8/fractal_server/app/routes/api/v1/__init__.py
+-rw-r--r--   0        0        0    11955 2024-04-16 09:44:55.214574 fractal_server-2.0.0a8/fractal_server/app/routes/api/v1/_aux_functions.py
+-rw-r--r--   0        0        0    16911 2024-04-16 09:44:55.214574 fractal_server-2.0.0a8/fractal_server/app/routes/api/v1/dataset.py
+-rw-r--r--   0        0        0     5436 2024-04-16 09:44:55.214574 fractal_server-2.0.0a8/fractal_server/app/routes/api/v1/job.py
+-rw-r--r--   0        0        0    15765 2024-04-16 09:44:55.214574 fractal_server-2.0.0a8/fractal_server/app/routes/api/v1/project.py
+-rw-r--r--   0        0        0     6123 2024-04-16 09:44:55.214574 fractal_server-2.0.0a8/fractal_server/app/routes/api/v1/task.py
+-rw-r--r--   0        0        0     8873 2024-04-16 09:44:55.214574 fractal_server-2.0.0a8/fractal_server/app/routes/api/v1/task_collection.py
+-rw-r--r--   0        0        0    10930 2024-04-16 09:44:55.214574 fractal_server-2.0.0a8/fractal_server/app/routes/api/v1/workflow.py
+-rw-r--r--   0        0        0     5579 2024-04-16 09:44:55.214574 fractal_server-2.0.0a8/fractal_server/app/routes/api/v1/workflowtask.py
+-rw-r--r--   0        0        0     1373 2024-04-16 09:44:55.214574 fractal_server-2.0.0a8/fractal_server/app/routes/api/v2/__init__.py
+-rw-r--r--   0        0        0    14301 2024-04-16 09:44:55.214574 fractal_server-2.0.0a8/fractal_server/app/routes/api/v2/_aux_functions.py
+-rw-r--r--   0        0        0    10008 2024-04-16 09:44:55.214574 fractal_server-2.0.0a8/fractal_server/app/routes/api/v2/dataset.py
+-rw-r--r--   0        0        0     7589 2024-04-16 09:44:55.214574 fractal_server-2.0.0a8/fractal_server/app/routes/api/v2/images.py
+-rw-r--r--   0        0        0     5334 2024-04-16 09:44:55.214574 fractal_server-2.0.0a8/fractal_server/app/routes/api/v2/job.py
+-rw-r--r--   0        0        0     6024 2024-04-16 09:44:55.214574 fractal_server-2.0.0a8/fractal_server/app/routes/api/v2/project.py
+-rw-r--r--   0        0        0     6901 2024-04-16 09:44:55.214574 fractal_server-2.0.0a8/fractal_server/app/routes/api/v2/submit.py
+-rw-r--r--   0        0        0     7130 2024-04-16 09:44:55.214574 fractal_server-2.0.0a8/fractal_server/app/routes/api/v2/task.py
+-rw-r--r--   0        0        0     8904 2024-04-16 09:44:55.214574 fractal_server-2.0.0a8/fractal_server/app/routes/api/v2/task_collection.py
+-rw-r--r--   0        0        0     1628 2024-04-16 09:44:55.214574 fractal_server-2.0.0a8/fractal_server/app/routes/api/v2/task_legacy.py
+-rw-r--r--   0        0        0    11845 2024-04-16 09:44:55.214574 fractal_server-2.0.0a8/fractal_server/app/routes/api/v2/workflow.py
+-rw-r--r--   0        0        0     8414 2024-04-16 09:44:55.214574 fractal_server-2.0.0a8/fractal_server/app/routes/api/v2/workflowtask.py
+-rw-r--r--   0        0        0     4885 2024-04-16 09:44:55.214574 fractal_server-2.0.0a8/fractal_server/app/routes/auth.py
+-rw-r--r--   0        0        0        0 2024-04-16 09:44:55.214574 fractal_server-2.0.0a8/fractal_server/app/routes/aux/__init__.py
+-rw-r--r--   0        0        0     1248 2024-04-16 09:44:55.214574 fractal_server-2.0.0a8/fractal_server/app/routes/aux/_job.py
+-rw-r--r--   0        0        0      675 2024-04-16 09:44:55.214574 fractal_server-2.0.0a8/fractal_server/app/routes/aux/_runner.py
+-rw-r--r--   0        0        0       16 2024-04-16 09:44:55.218574 fractal_server-2.0.0a8/fractal_server/app/runner/.gitignore
+-rw-r--r--   0        0        0        0 2024-04-16 09:44:55.218574 fractal_server-2.0.0a8/fractal_server/app/runner/__init__.py
+-rw-r--r--   0        0        0      829 2024-04-16 09:44:55.218574 fractal_server-2.0.0a8/fractal_server/app/runner/async_wrap.py
+-rw-r--r--   0        0        0      119 2024-04-16 09:44:55.218574 fractal_server-2.0.0a8/fractal_server/app/runner/components.py
+-rw-r--r--   0        0        0     4159 2024-04-16 09:44:55.218574 fractal_server-2.0.0a8/fractal_server/app/runner/exceptions.py
+-rw-r--r--   0        0        0        0 2024-04-16 09:44:55.218574 fractal_server-2.0.0a8/fractal_server/app/runner/executors/__init__.py
+-rw-r--r--   0        0        0       65 2024-04-16 09:44:55.218574 fractal_server-2.0.0a8/fractal_server/app/runner/executors/slurm/__init__.py
+-rw-r--r--   0        0        0     8841 2024-04-16 09:44:55.218574 fractal_server-2.0.0a8/fractal_server/app/runner/executors/slurm/_batching.py
+-rw-r--r--   0        0        0     1908 2024-04-16 09:44:55.218574 fractal_server-2.0.0a8/fractal_server/app/runner/executors/slurm/_check_jobs_status.py
+-rw-r--r--   0        0        0     4421 2024-04-16 09:44:55.218574 fractal_server-2.0.0a8/fractal_server/app/runner/executors/slurm/_executor_wait_thread.py
+-rw-r--r--   0        0        0    15552 2024-04-16 09:44:55.218574 fractal_server-2.0.0a8/fractal_server/app/runner/executors/slurm/_slurm_config.py
+-rw-r--r--   0        0        0     5123 2024-04-16 09:44:55.218574 fractal_server-2.0.0a8/fractal_server/app/runner/executors/slurm/_subprocess_run_as_user.py
+-rw-r--r--   0        0        0    44451 2024-04-16 09:44:55.218574 fractal_server-2.0.0a8/fractal_server/app/runner/executors/slurm/executor.py
+-rw-r--r--   0        0        0     5852 2024-04-16 09:44:55.218574 fractal_server-2.0.0a8/fractal_server/app/runner/executors/slurm/remote.py
+-rw-r--r--   0        0        0      206 2024-04-16 09:44:55.218574 fractal_server-2.0.0a8/fractal_server/app/runner/filenames.py
+-rw-r--r--   0        0        0     1254 2024-04-16 09:44:55.218574 fractal_server-2.0.0a8/fractal_server/app/runner/set_start_and_last_task_index.py
+-rw-r--r--   0        0        0     3219 2024-04-16 09:44:55.218574 fractal_server-2.0.0a8/fractal_server/app/runner/task_files.py
+-rw-r--r--   0        0        0    13608 2024-04-16 09:44:55.218574 fractal_server-2.0.0a8/fractal_server/app/runner/v1/__init__.py
+-rw-r--r--   0        0        0    21240 2024-04-16 09:44:55.218574 fractal_server-2.0.0a8/fractal_server/app/runner/v1/_common.py
+-rw-r--r--   0        0        0     6926 2024-04-16 09:44:55.218574 fractal_server-2.0.0a8/fractal_server/app/runner/v1/_local/__init__.py
+-rw-r--r--   0        0        0     3147 2024-04-16 09:44:55.218574 fractal_server-2.0.0a8/fractal_server/app/runner/v1/_local/_local_config.py
+-rw-r--r--   0        0        0     1493 2024-04-16 09:44:55.218574 fractal_server-2.0.0a8/fractal_server/app/runner/v1/_local/_submit_setup.py
+-rw-r--r--   0        0        0     3620 2024-04-16 09:44:55.218574 fractal_server-2.0.0a8/fractal_server/app/runner/v1/_local/executor.py
+-rw-r--r--   0        0        0    10853 2024-04-16 09:44:55.218574 fractal_server-2.0.0a8/fractal_server/app/runner/v1/_slurm/__init__.py
+-rw-r--r--   0        0        0     2738 2024-04-16 09:44:55.218574 fractal_server-2.0.0a8/fractal_server/app/runner/v1/_slurm/_submit_setup.py
+-rw-r--r--   0        0        0     5977 2024-04-16 09:44:55.218574 fractal_server-2.0.0a8/fractal_server/app/runner/v1/_slurm/get_slurm_config.py
+-rw-r--r--   0        0        0     3294 2024-04-16 09:44:55.218574 fractal_server-2.0.0a8/fractal_server/app/runner/v1/common.py
+-rw-r--r--   0        0        0     4684 2024-04-16 09:44:55.218574 fractal_server-2.0.0a8/fractal_server/app/runner/v1/handle_failed_job.py
+-rw-r--r--   0        0        0    12482 2024-04-16 09:44:55.218574 fractal_server-2.0.0a8/fractal_server/app/runner/v2/__init__.py
+-rw-r--r--   0        0        0     5881 2024-04-16 09:44:55.218574 fractal_server-2.0.0a8/fractal_server/app/runner/v2/_local/__init__.py
+-rw-r--r--   0        0        0     3630 2024-04-16 09:44:55.218574 fractal_server-2.0.0a8/fractal_server/app/runner/v2/_local/_local_config.py
+-rw-r--r--   0        0        0     1614 2024-04-16 09:44:55.218574 fractal_server-2.0.0a8/fractal_server/app/runner/v2/_local/_submit_setup.py
+-rw-r--r--   0        0        0     3620 2024-04-16 09:44:55.218574 fractal_server-2.0.0a8/fractal_server/app/runner/v2/_local/executor.py
+-rw-r--r--   0        0        0     4409 2024-04-16 09:44:55.218574 fractal_server-2.0.0a8/fractal_server/app/runner/v2/_slurm/__init__.py
+-rw-r--r--   0        0        0     2793 2024-04-16 09:44:55.218574 fractal_server-2.0.0a8/fractal_server/app/runner/v2/_slurm/_submit_setup.py
+-rw-r--r--   0        0        0     6621 2024-04-16 09:44:55.218574 fractal_server-2.0.0a8/fractal_server/app/runner/v2/_slurm/get_slurm_config.py
+-rw-r--r--   0        0        0      639 2024-04-16 09:44:55.218574 fractal_server-2.0.0a8/fractal_server/app/runner/v2/deduplicate_list.py
+-rw-r--r--   0        0        0     5202 2024-04-16 09:44:55.218574 fractal_server-2.0.0a8/fractal_server/app/runner/v2/handle_failed_job.py
+-rw-r--r--   0        0        0     1281 2024-04-16 09:44:55.218574 fractal_server-2.0.0a8/fractal_server/app/runner/v2/merge_outputs.py
+-rw-r--r--   0        0        0    11784 2024-04-16 09:44:55.218574 fractal_server-2.0.0a8/fractal_server/app/runner/v2/runner.py
+-rw-r--r--   0        0        0    10087 2024-04-16 09:44:55.218574 fractal_server-2.0.0a8/fractal_server/app/runner/v2/runner_functions.py
+-rw-r--r--   0        0        0     3845 2024-04-16 09:44:55.218574 fractal_server-2.0.0a8/fractal_server/app/runner/v2/runner_functions_low_level.py
+-rw-r--r--   0        0        0     1746 2024-04-16 09:44:55.218574 fractal_server-2.0.0a8/fractal_server/app/runner/v2/task_interface.py
+-rw-r--r--   0        0        0      511 2024-04-16 09:44:55.218574 fractal_server-2.0.0a8/fractal_server/app/runner/v2/v1_compat.py
+-rw-r--r--   0        0        0      157 2024-04-16 09:44:55.218574 fractal_server-2.0.0a8/fractal_server/app/schemas/__init__.py
+-rw-r--r--   0        0        0     3461 2024-04-16 09:44:55.218574 fractal_server-2.0.0a8/fractal_server/app/schemas/_validators.py
+-rw-r--r--   0        0        0      692 2024-04-16 09:44:55.218574 fractal_server-2.0.0a8/fractal_server/app/schemas/state.py
+-rw-r--r--   0        0        0     3113 2024-04-16 09:44:55.218574 fractal_server-2.0.0a8/fractal_server/app/schemas/user.py
+-rw-r--r--   0        0        0     2078 2024-04-16 09:44:55.218574 fractal_server-2.0.0a8/fractal_server/app/schemas/v1/__init__.py
+-rw-r--r--   0        0        0     4302 2024-04-16 09:44:55.218574 fractal_server-2.0.0a8/fractal_server/app/schemas/v1/applyworkflow.py
+-rw-r--r--   0        0        0     3444 2024-04-16 09:44:55.218574 fractal_server-2.0.0a8/fractal_server/app/schemas/v1/dataset.py
+-rw-r--r--   0        0        0     1274 2024-04-16 09:44:55.218574 fractal_server-2.0.0a8/fractal_server/app/schemas/v1/dumps.py
+-rw-r--r--   0        0        0     3829 2024-04-16 09:44:55.218574 fractal_server-2.0.0a8/fractal_server/app/schemas/v1/manifest.py
+-rw-r--r--   0        0        0     1218 2024-04-16 09:44:55.218574 fractal_server-2.0.0a8/fractal_server/app/schemas/v1/project.py
+-rw-r--r--   0        0        0     3704 2024-04-16 09:44:55.218574 fractal_server-2.0.0a8/fractal_server/app/schemas/v1/task.py
+-rw-r--r--   0        0        0     3057 2024-04-16 09:44:55.218574 fractal_server-2.0.0a8/fractal_server/app/schemas/v1/task_collection.py
+-rw-r--r--   0        0        0     4618 2024-04-16 09:44:55.218574 fractal_server-2.0.0a8/fractal_server/app/schemas/v1/workflow.py
+-rw-r--r--   0        0        0     1752 2024-04-16 09:44:55.218574 fractal_server-2.0.0a8/fractal_server/app/schemas/v2/__init__.py
+-rw-r--r--   0        0        0     2086 2024-04-16 09:44:55.218574 fractal_server-2.0.0a8/fractal_server/app/schemas/v2/dataset.py
+-rw-r--r--   0        0        0     1997 2024-04-16 09:44:55.218574 fractal_server-2.0.0a8/fractal_server/app/schemas/v2/dumps.py
+-rw-r--r--   0        0        0     3250 2024-04-16 09:44:55.218574 fractal_server-2.0.0a8/fractal_server/app/schemas/v2/job.py
+-rw-r--r--   0        0        0     6243 2024-04-16 09:44:55.218574 fractal_server-2.0.0a8/fractal_server/app/schemas/v2/manifest.py
+-rw-r--r--   0        0        0      736 2024-04-16 09:44:55.222575 fractal_server-2.0.0a8/fractal_server/app/schemas/v2/project.py
+-rw-r--r--   0        0        0     4672 2024-04-16 09:44:55.222575 fractal_server-2.0.0a8/fractal_server/app/schemas/v2/task.py
+-rw-r--r--   0        0        0     3171 2024-04-16 09:44:55.222575 fractal_server-2.0.0a8/fractal_server/app/schemas/v2/task_collection.py
+-rw-r--r--   0        0        0     1827 2024-04-16 09:44:55.222575 fractal_server-2.0.0a8/fractal_server/app/schemas/v2/workflow.py
+-rw-r--r--   0        0        0     5051 2024-04-16 09:44:55.222575 fractal_server-2.0.0a8/fractal_server/app/schemas/v2/workflowtask.py
+-rw-r--r--   0        0        0    11203 2024-04-16 09:44:55.222575 fractal_server-2.0.0a8/fractal_server/app/security/__init__.py
+-rw-r--r--   0        0        0    15080 2024-04-16 09:44:55.222575 fractal_server-2.0.0a8/fractal_server/config.py
+-rw-r--r--   0        0        0      398 2024-04-16 09:44:55.222575 fractal_server-2.0.0a8/fractal_server/data_migrations/README.md
+-rw-r--r--   0        0        0      196 2024-04-16 09:44:55.222575 fractal_server-2.0.0a8/fractal_server/images/__init__.py
+-rw-r--r--   0        0        0     4167 2024-04-16 09:44:55.222575 fractal_server-2.0.0a8/fractal_server/images/models.py
+-rw-r--r--   0        0        0     2234 2024-04-16 09:44:55.222575 fractal_server-2.0.0a8/fractal_server/images/tools.py
+-rw-r--r--   0        0        0     3924 2024-04-16 09:44:55.222575 fractal_server-2.0.0a8/fractal_server/logger.py
+-rw-r--r--   0        0        0     3001 2024-04-16 09:44:55.222575 fractal_server-2.0.0a8/fractal_server/main.py
+-rw-r--r--   0        0        0       59 2024-04-16 09:44:55.222575 fractal_server-2.0.0a8/fractal_server/migrations/README
+-rw-r--r--   0        0        0     2630 2024-04-16 09:44:55.222575 fractal_server-2.0.0a8/fractal_server/migrations/env.py
+-rw-r--r--   0        0        0      526 2024-04-16 09:44:55.222575 fractal_server-2.0.0a8/fractal_server/migrations/script.py.mako
+-rw-r--r--   0        0        0      954 2024-04-16 09:44:55.222575 fractal_server-2.0.0a8/fractal_server/migrations/versions/4c308bcaea2b_add_task_args_schema_and_task_args_.py
+-rw-r--r--   0        0        0     1157 2024-04-16 09:44:55.222575 fractal_server-2.0.0a8/fractal_server/migrations/versions/4cedeb448a53_workflowtask_foreign_keys_not_nullables.py
+-rw-r--r--   0        0        0     8770 2024-04-16 09:44:55.222575 fractal_server-2.0.0a8/fractal_server/migrations/versions/50a13d6138fd_initial_schema.py
+-rw-r--r--   0        0        0     1632 2024-04-16 09:44:55.222575 fractal_server-2.0.0a8/fractal_server/migrations/versions/70e77f1c38b0_add_applyworkflow_first_task_index_and_.py
+-rw-r--r--   0        0        0     1353 2024-04-16 09:44:55.222575 fractal_server-2.0.0a8/fractal_server/migrations/versions/71eefd1dd202_add_slurm_accounts.py
+-rw-r--r--   0        0        0     8116 2024-04-16 09:44:55.222575 fractal_server-2.0.0a8/fractal_server/migrations/versions/80e12e1bc4fd_v2.py
+-rw-r--r--   0        0        0     2684 2024-04-16 09:44:55.222575 fractal_server-2.0.0a8/fractal_server/migrations/versions/84bf0fffde30_add_dumps_to_applyworkflow.py
+-rw-r--r--   0        0        0     1115 2024-04-16 09:44:55.222575 fractal_server-2.0.0a8/fractal_server/migrations/versions/8f79bd162e35_add_docs_info_and_docs_link_to_task_.py
+-rw-r--r--   0        0        0     1057 2024-04-16 09:44:55.222575 fractal_server-2.0.0a8/fractal_server/migrations/versions/97f444d47249_add_applyworkflow_project_dump.py
+-rw-r--r--   0        0        0      883 2024-04-16 09:44:55.222575 fractal_server-2.0.0a8/fractal_server/migrations/versions/99ea79d9e5d2_add_dataset_history.py
+-rw-r--r--   0        0        0     1849 2024-04-16 09:44:55.222575 fractal_server-2.0.0a8/fractal_server/migrations/versions/9fd26a2b0de4_add_workflow_timestamp_created.py
+-rw-r--r--   0        0        0      867 2024-04-16 09:44:55.222575 fractal_server-2.0.0a8/fractal_server/migrations/versions/a7f4d6137b53_add_workflow_dump_to_applyworkflow.py
+-rw-r--r--   0        0        0      949 2024-04-16 09:44:55.222575 fractal_server-2.0.0a8/fractal_server/migrations/versions/d4fe3708d309_make_applyworkflow_workflow_dump_non_.py
+-rw-r--r--   0        0        0      963 2024-04-16 09:44:55.222575 fractal_server-2.0.0a8/fractal_server/migrations/versions/e75cac726012_make_applyworkflow_start_timestamp_not_.py
+-rw-r--r--   0        0        0     1221 2024-04-16 09:44:55.222575 fractal_server-2.0.0a8/fractal_server/migrations/versions/efa89c30e0a4_add_project_timestamp_created.py
+-rw-r--r--   0        0        0      746 2024-04-16 09:44:55.222575 fractal_server-2.0.0a8/fractal_server/migrations/versions/f384e1c0cf5d_drop_task_default_args_columns.py
+-rw-r--r--   0        0        0        0 2024-04-16 09:44:55.222575 fractal_server-2.0.0a8/fractal_server/py.typed
+-rw-r--r--   0        0        0     2786 2024-04-16 09:44:55.222575 fractal_server-2.0.0a8/fractal_server/syringe.py
+-rw-r--r--   0        0        0       23 2024-04-16 09:44:55.222575 fractal_server-2.0.0a8/fractal_server/tasks/__init__.py
+-rw-r--r--   0        0        0     5379 2024-04-16 09:44:55.222575 fractal_server-2.0.0a8/fractal_server/tasks/endpoint_operations.py
+-rw-r--r--   0        0        0     3278 2024-04-16 09:44:55.222575 fractal_server-2.0.0a8/fractal_server/tasks/utils.py
+-rw-r--r--   0        0        0     3775 2024-04-16 09:44:55.222575 fractal_server-2.0.0a8/fractal_server/tasks/v1/_TaskCollectPip.py
+-rw-r--r--   0        0        0        0 2024-04-16 09:44:55.222575 fractal_server-2.0.0a8/fractal_server/tasks/v1/__init__.py
+-rw-r--r--   0        0        0    11725 2024-04-16 09:44:55.222575 fractal_server-2.0.0a8/fractal_server/tasks/v1/background_operations.py
+-rw-r--r--   0        0        0      502 2024-04-16 09:44:55.222575 fractal_server-2.0.0a8/fractal_server/tasks/v1/get_collection_data.py
+-rw-r--r--   0        0        0     3775 2024-04-16 09:44:55.222575 fractal_server-2.0.0a8/fractal_server/tasks/v2/_TaskCollectPip.py
+-rw-r--r--   0        0        0        0 2024-04-16 09:44:55.222575 fractal_server-2.0.0a8/fractal_server/tasks/v2/__init__.py
+-rw-r--r--   0        0        0    12803 2024-04-16 09:44:55.222575 fractal_server-2.0.0a8/fractal_server/tasks/v2/background_operations.py
+-rw-r--r--   0        0        0      502 2024-04-16 09:44:55.222575 fractal_server-2.0.0a8/fractal_server/tasks/v2/get_collection_data.py
+-rw-r--r--   0        0        0      448 2024-04-16 09:44:55.222575 fractal_server-2.0.0a8/fractal_server/urls.py
+-rw-r--r--   0        0        0     2115 2024-04-16 09:44:55.222575 fractal_server-2.0.0a8/fractal_server/utils.py
+-rw-r--r--   0        0        0     2999 2024-04-16 09:44:55.226575 fractal_server-2.0.0a8/pyproject.toml
+-rw-r--r--   0        0        0     4204 1970-01-01 00:00:00.000000 fractal_server-2.0.0a8/PKG-INFO
```

### Comparing `fractal_server-2.0.0a6/LICENSE` & `fractal_server-2.0.0a8/LICENSE`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a6/README.md` & `fractal_server-2.0.0a8/README.md`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a6/fractal_server/__main__.py` & `fractal_server-2.0.0a8/fractal_server/__main__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a6/fractal_server/alembic.ini` & `fractal_server-2.0.0a8/fractal_server/alembic.ini`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a6/fractal_server/app/db/__init__.py` & `fractal_server-2.0.0a8/fractal_server/app/db/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a6/fractal_server/app/models/linkuserproject.py` & `fractal_server-2.0.0a8/fractal_server/app/models/linkuserproject.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a6/fractal_server/app/models/security.py` & `fractal_server-2.0.0a8/fractal_server/app/models/security.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a6/fractal_server/app/models/state.py` & `fractal_server-2.0.0a8/fractal_server/app/models/state.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a6/fractal_server/app/models/v1/dataset.py` & `fractal_server-2.0.0a8/fractal_server/app/models/v1/dataset.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a6/fractal_server/app/models/v1/job.py` & `fractal_server-2.0.0a8/fractal_server/app/models/v1/job.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a6/fractal_server/app/models/v1/project.py` & `fractal_server-2.0.0a8/fractal_server/app/models/v1/project.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a6/fractal_server/app/models/v1/task.py` & `fractal_server-2.0.0a8/fractal_server/app/models/v1/task.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a6/fractal_server/app/models/v1/workflow.py` & `fractal_server-2.0.0a8/fractal_server/app/models/v1/workflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a6/fractal_server/app/models/v2/dataset.py` & `fractal_server-2.0.0a8/fractal_server/app/models/v2/dataset.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a6/fractal_server/app/models/v2/job.py` & `fractal_server-2.0.0a8/fractal_server/app/models/v2/job.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a6/fractal_server/app/models/v2/project.py` & `fractal_server-2.0.0a8/fractal_server/app/models/v2/project.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a6/fractal_server/app/models/v2/task.py` & `fractal_server-2.0.0a8/fractal_server/app/models/v2/task.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a6/fractal_server/app/models/v2/workflow.py` & `fractal_server-2.0.0a8/fractal_server/app/models/v2/workflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a6/fractal_server/app/models/v2/workflowtask.py` & `fractal_server-2.0.0a8/fractal_server/app/models/v2/workflowtask.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a6/fractal_server/app/routes/admin/v1.py` & `fractal_server-2.0.0a8/fractal_server/app/routes/admin/v1.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a6/fractal_server/app/routes/admin/v2.py` & `fractal_server-2.0.0a8/fractal_server/app/routes/admin/v2.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a6/fractal_server/app/routes/api/v1/__init__.py` & `fractal_server-2.0.0a8/fractal_server/app/routes/api/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a6/fractal_server/app/routes/api/v1/_aux_functions.py` & `fractal_server-2.0.0a8/fractal_server/app/routes/api/v1/_aux_functions.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a6/fractal_server/app/routes/api/v1/dataset.py` & `fractal_server-2.0.0a8/fractal_server/app/routes/api/v1/dataset.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a6/fractal_server/app/routes/api/v1/job.py` & `fractal_server-2.0.0a8/fractal_server/app/routes/api/v1/job.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a6/fractal_server/app/routes/api/v1/project.py` & `fractal_server-2.0.0a8/fractal_server/app/routes/api/v1/project.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a6/fractal_server/app/routes/api/v1/task.py` & `fractal_server-2.0.0a8/fractal_server/app/routes/api/v1/task.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a6/fractal_server/app/routes/api/v1/task_collection.py` & `fractal_server-2.0.0a8/fractal_server/app/routes/api/v1/task_collection.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a6/fractal_server/app/routes/api/v1/workflow.py` & `fractal_server-2.0.0a8/fractal_server/app/routes/api/v1/workflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a6/fractal_server/app/routes/api/v1/workflowtask.py` & `fractal_server-2.0.0a8/fractal_server/app/routes/api/v1/workflowtask.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a6/fractal_server/app/routes/api/v2/__init__.py` & `fractal_server-2.0.0a8/fractal_server/app/routes/api/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a6/fractal_server/app/routes/api/v2/_aux_functions.py` & `fractal_server-2.0.0a8/fractal_server/app/routes/api/v2/_aux_functions.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a6/fractal_server/app/routes/api/v2/dataset.py` & `fractal_server-2.0.0a8/fractal_server/app/routes/api/v2/dataset.py`

 * *Files 5% similar despite different names*

```diff
@@ -130,14 +130,23 @@
         project_id=project_id,
         dataset_id=dataset_id,
         user_id=user.id,
         db=db,
     )
     db_dataset = output["dataset"]
 
+    if (dataset_update.zarr_dir is not None) and (len(db_dataset.images) != 0):
+        raise HTTPException(
+            status_code=status.HTTP_422_UNPROCESSABLE_ENTITY,
+            detail=(
+                "Cannot modify `zarr_dir` because the dataset has a non-empty "
+                "image list."
+            ),
+        )
+
     for key, value in dataset_update.dict(exclude_unset=True).items():
         setattr(db_dataset, key, value)
 
     await db.commit()
     await db.refresh(db_dataset)
     await db.close()
     return db_dataset
```

### Comparing `fractal_server-2.0.0a6/fractal_server/app/routes/api/v2/images.py` & `fractal_server-2.0.0a8/fractal_server/app/routes/api/v2/images.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 from ._aux_functions import _get_dataset_check_owner
 from fractal_server.app.db import AsyncSession
 from fractal_server.app.db import get_async_db
 from fractal_server.app.security import current_active_user
 from fractal_server.app.security import User
 from fractal_server.images import Filters
 from fractal_server.images import SingleImage
+from fractal_server.images import SingleImageUpdate
+from fractal_server.images.tools import find_image_by_zarr_url
 from fractal_server.images.tools import match_filter
 
 router = APIRouter()
 
 
 class ImagePage(BaseModel):
 
@@ -52,14 +54,23 @@
 ) -> Response:
 
     output = await _get_dataset_check_owner(
         project_id=project_id, dataset_id=dataset_id, user_id=user.id, db=db
     )
     dataset = output["dataset"]
 
+    if not new_image.zarr_url.startswith(dataset.zarr_dir):
+        raise HTTPException(
+            status_code=status.HTTP_422_UNPROCESSABLE_ENTITY,
+            detail=(
+                "Cannot create image with zarr_url which is not relative to "
+                f"{dataset.zarr_dir}."
+            ),
+        )
+
     if new_image.zarr_url in dataset.image_zarr_urls:
         raise HTTPException(
             status_code=status.HTTP_422_UNPROCESSABLE_ENTITY,
             detail=(
                 f"Image with zarr_url '{new_image.zarr_url}' "
                 f"already in DatasetV2 {dataset_id}",
             ),
@@ -209,7 +220,52 @@
 
     dataset.images.remove(image_to_remove)
     flag_modified(dataset, "images")
 
     await db.commit()
 
     return Response(status_code=status.HTTP_204_NO_CONTENT)
+
+
+@router.patch(
+    "/project/{project_id}/dataset/{dataset_id}/images/",
+    response_model=SingleImage,
+    status_code=status.HTTP_200_OK,
+)
+async def patch_dataset_image(
+    project_id: int,
+    dataset_id: int,
+    image_update: SingleImageUpdate,
+    user: User = Depends(current_active_user),
+    db: AsyncSession = Depends(get_async_db),
+):
+    output = await _get_dataset_check_owner(
+        project_id=project_id,
+        dataset_id=dataset_id,
+        user_id=user.id,
+        db=db,
+    )
+    db_dataset = output["dataset"]
+
+    ret = find_image_by_zarr_url(
+        images=db_dataset.images, zarr_url=image_update.zarr_url
+    )
+    if ret is None:
+        raise HTTPException(
+            status_code=status.HTTP_404_NOT_FOUND,
+            detail=(
+                f"No image with zarr_url '{image_update.zarr_url}' in "
+                f"DatasetV2 {dataset_id}."
+            ),
+        )
+    index = ret["index"]
+
+    for key, value in image_update.dict(
+        exclude_none=True, exclude={"zarr_url"}
+    ).items():
+        db_dataset.images[index][key] = value
+
+    flag_modified(db_dataset, "images")
+
+    await db.commit()
+    await db.close()
+    return db_dataset.images[index]
```

### Comparing `fractal_server-2.0.0a6/fractal_server/app/routes/api/v2/job.py` & `fractal_server-2.0.0a8/fractal_server/app/routes/api/v2/job.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a6/fractal_server/app/routes/api/v2/project.py` & `fractal_server-2.0.0a8/fractal_server/app/routes/api/v2/project.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a6/fractal_server/app/routes/api/v2/submit.py` & `fractal_server-2.0.0a8/fractal_server/app/routes/api/v2/submit.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a6/fractal_server/app/routes/api/v2/task.py` & `fractal_server-2.0.0a8/fractal_server/app/routes/api/v2/task.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a6/fractal_server/app/routes/api/v2/task_collection.py` & `fractal_server-2.0.0a8/fractal_server/app/routes/api/v2/task_collection.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a6/fractal_server/app/routes/api/v2/task_legacy.py` & `fractal_server-2.0.0a8/fractal_server/app/routes/api/v2/task_legacy.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a6/fractal_server/app/routes/api/v2/workflow.py` & `fractal_server-2.0.0a8/fractal_server/app/routes/api/v2/workflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a6/fractal_server/app/routes/api/v2/workflowtask.py` & `fractal_server-2.0.0a8/fractal_server/app/routes/api/v2/workflowtask.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a6/fractal_server/app/routes/auth.py` & `fractal_server-2.0.0a8/fractal_server/app/routes/auth.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a6/fractal_server/app/routes/aux/_job.py` & `fractal_server-2.0.0a8/fractal_server/app/routes/aux/_job.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a6/fractal_server/app/routes/aux/_runner.py` & `fractal_server-2.0.0a8/fractal_server/app/routes/aux/_runner.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a6/fractal_server/app/runner/async_wrap.py` & `fractal_server-2.0.0a8/fractal_server/app/runner/async_wrap.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a6/fractal_server/app/runner/exceptions.py` & `fractal_server-2.0.0a8/fractal_server/app/runner/exceptions.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a6/fractal_server/app/runner/executors/slurm/_batching.py` & `fractal_server-2.0.0a8/fractal_server/app/runner/executors/slurm/_batching.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a6/fractal_server/app/runner/executors/slurm/_check_jobs_status.py` & `fractal_server-2.0.0a8/fractal_server/app/runner/executors/slurm/_check_jobs_status.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a6/fractal_server/app/runner/executors/slurm/_executor_wait_thread.py` & `fractal_server-2.0.0a8/fractal_server/app/runner/executors/slurm/_executor_wait_thread.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a6/fractal_server/app/runner/executors/slurm/_slurm_config.py` & `fractal_server-2.0.0a8/fractal_server/app/runner/executors/slurm/_slurm_config.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a6/fractal_server/app/runner/executors/slurm/_subprocess_run_as_user.py` & `fractal_server-2.0.0a8/fractal_server/app/runner/executors/slurm/_subprocess_run_as_user.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a6/fractal_server/app/runner/executors/slurm/executor.py` & `fractal_server-2.0.0a8/fractal_server/app/runner/executors/slurm/executor.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a6/fractal_server/app/runner/executors/slurm/remote.py` & `fractal_server-2.0.0a8/fractal_server/app/runner/executors/slurm/remote.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a6/fractal_server/app/runner/set_start_and_last_task_index.py` & `fractal_server-2.0.0a8/fractal_server/app/runner/set_start_and_last_task_index.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a6/fractal_server/app/runner/task_files.py` & `fractal_server-2.0.0a8/fractal_server/app/runner/task_files.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a6/fractal_server/app/runner/v1/__init__.py` & `fractal_server-2.0.0a8/fractal_server/app/runner/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a6/fractal_server/app/runner/v1/_common.py` & `fractal_server-2.0.0a8/fractal_server/app/runner/v1/_common.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a6/fractal_server/app/runner/v1/_local/__init__.py` & `fractal_server-2.0.0a8/fractal_server/app/runner/v1/_local/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a6/fractal_server/app/runner/v1/_local/_local_config.py` & `fractal_server-2.0.0a8/fractal_server/app/runner/v1/_local/_local_config.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a6/fractal_server/app/runner/v1/_local/_submit_setup.py` & `fractal_server-2.0.0a8/fractal_server/app/runner/v1/_local/_submit_setup.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a6/fractal_server/app/runner/v1/_local/executor.py` & `fractal_server-2.0.0a8/fractal_server/app/runner/v1/_local/executor.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a6/fractal_server/app/runner/v1/_slurm/__init__.py` & `fractal_server-2.0.0a8/fractal_server/app/runner/v1/_slurm/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a6/fractal_server/app/runner/v1/_slurm/_submit_setup.py` & `fractal_server-2.0.0a8/fractal_server/app/runner/v1/_slurm/_submit_setup.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a6/fractal_server/app/runner/v1/_slurm/get_slurm_config.py` & `fractal_server-2.0.0a8/fractal_server/app/runner/v1/_slurm/get_slurm_config.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a6/fractal_server/app/runner/v1/common.py` & `fractal_server-2.0.0a8/fractal_server/app/runner/v1/common.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a6/fractal_server/app/runner/v1/handle_failed_job.py` & `fractal_server-2.0.0a8/fractal_server/app/runner/v1/handle_failed_job.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a6/fractal_server/app/runner/v2/__init__.py` & `fractal_server-2.0.0a8/fractal_server/app/runner/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a6/fractal_server/app/runner/v2/_local/__init__.py` & `fractal_server-2.0.0a8/fractal_server/app/runner/v2/_local/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a6/fractal_server/app/runner/v2/_local/_local_config.py` & `fractal_server-2.0.0a8/fractal_server/app/runner/v2/_local/_local_config.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a6/fractal_server/app/runner/v2/_local/_submit_setup.py` & `fractal_server-2.0.0a8/fractal_server/app/runner/v2/_local/_submit_setup.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a6/fractal_server/app/runner/v2/_local/executor.py` & `fractal_server-2.0.0a8/fractal_server/app/runner/v2/_local/executor.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a6/fractal_server/app/runner/v2/_slurm/__init__.py` & `fractal_server-2.0.0a8/fractal_server/app/runner/v2/_slurm/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a6/fractal_server/app/runner/v2/_slurm/_submit_setup.py` & `fractal_server-2.0.0a8/fractal_server/app/runner/v2/_slurm/_submit_setup.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a6/fractal_server/app/runner/v2/_slurm/get_slurm_config.py` & `fractal_server-2.0.0a8/fractal_server/app/runner/v2/_slurm/get_slurm_config.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a6/fractal_server/app/runner/v2/deduplicate_list.py` & `fractal_server-2.0.0a8/fractal_server/app/runner/v2/deduplicate_list.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a6/fractal_server/app/runner/v2/handle_failed_job.py` & `fractal_server-2.0.0a8/fractal_server/app/runner/v2/handle_failed_job.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a6/fractal_server/app/runner/v2/merge_outputs.py` & `fractal_server-2.0.0a8/fractal_server/app/runner/v2/merge_outputs.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a6/fractal_server/app/runner/v2/runner.py` & `fractal_server-2.0.0a8/fractal_server/app/runner/v2/runner.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a6/fractal_server/app/runner/v2/runner_functions.py` & `fractal_server-2.0.0a8/fractal_server/app/runner/v2/runner_functions.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a6/fractal_server/app/runner/v2/runner_functions_low_level.py` & `fractal_server-2.0.0a8/fractal_server/app/runner/v2/runner_functions_low_level.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a6/fractal_server/app/runner/v2/task_interface.py` & `fractal_server-2.0.0a8/fractal_server/app/runner/v2/task_interface.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from typing import Any
 
 from pydantic import BaseModel
 from pydantic import Field
+from pydantic import validator
 
 from ....images import SingleImageTaskOutput
 from fractal_server.images import Filters
+from fractal_server.urls import normalize_url
 
 
 class TaskOutput(BaseModel):
     class Config:
         extra = "forbid"
 
     image_list_updates: list[SingleImageTaskOutput] = Field(
@@ -30,21 +32,29 @@
                 "TaskOutput image-list updates/removals has "
                 "non-unique zarr_urls:"
             )
             for duplicate in duplicates:
                 msg = f"{msg}\n{duplicate}"
             raise ValueError(msg)
 
+    @validator("image_list_removals")
+    def normalize_paths(cls, v: list[str]) -> list[str]:
+        return [normalize_url(zarr_url) for zarr_url in v]
+
 
 class InitArgsModel(BaseModel):
     class Config:
         extra = "forbid"
 
     zarr_url: str
     init_args: dict[str, Any] = Field(default_factory=dict)
 
+    @validator("zarr_url")
+    def normalize_path(cls, v: str) -> str:
+        return normalize_url(v)
+
 
 class InitTaskOutput(BaseModel):
     class Config:
         extra = "forbid"
 
     parallelization_list: list[InitArgsModel] = Field(default_factory=list)
```

### Comparing `fractal_server-2.0.0a6/fractal_server/app/schemas/_validators.py` & `fractal_server-2.0.0a8/fractal_server/app/schemas/_validators.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import os
 from datetime import datetime
 from datetime import timezone
 from typing import Any
+from typing import Optional
 
 
 def valstr(attribute: str, accept_none: bool = False):
     """
     Check that a string attribute is not an empty string, and remove the
     leading and trailing whitespace characters.
 
     If `accept_none`, the validator also accepts `None`.
     """
 
-    def val(string: str):
+    def val(string: Optional[str]) -> Optional[str]:
         if string is None:
             if accept_none:
                 return string
             else:
                 raise ValueError(
                     f"String attribute '{attribute}' cannot be None"
                 )
@@ -25,15 +26,15 @@
             raise ValueError(f"String attribute '{attribute}' cannot be empty")
         return s
 
     return val
 
 
 def valdictkeys(attribute: str):
-    def val(d: dict[str, Any]):
+    def val(d: Optional[dict[str, Any]]) -> Optional[dict[str, Any]]:
         """
         Apply valstr to every key of the dictionary, and fail if there are
         identical keys.
         """
         if d is not None:
             old_keys = list(d.keys())
             new_keys = [valstr(f"{attribute}[{key}]")(key) for key in old_keys]
@@ -51,15 +52,15 @@
 
 def valint(attribute: str, min_val: int = 1):
     """
     Check that an integer attribute (e.g. if it is meant to be the ID of a
     database entry) is greater or equal to min_val.
     """
 
-    def val(integer: int):
+    def val(integer: Optional[int]) -> Optional[int]:
         if integer is None:
             raise ValueError(f"Integer attribute '{attribute}' cannot be None")
         if integer < min_val:
             raise ValueError(
                 f"Integer attribute '{attribute}' cannot be less than "
                 f"{min_val} (given {integer})"
             )
@@ -69,15 +70,15 @@
 
 
 def val_absolute_path(attribute: str):
     """
     Check that a string attribute is an absolute path
     """
 
-    def val(string: str):
+    def val(string: Optional[str]) -> str:
         if string is None:
             raise ValueError(f"String attribute '{attribute}' cannot be None")
         s = string.strip()
         if not s:
             raise ValueError(f"String attribute '{attribute}' cannot be empty")
         if not os.path.isabs(s):
             raise ValueError(
@@ -86,25 +87,25 @@
             )
         return s
 
     return val
 
 
 def val_unique_list(attribute: str):
-    def val(must_be_unique: list):
+    def val(must_be_unique: Optional[list]) -> Optional[list]:
         if must_be_unique is not None:
             if len(set(must_be_unique)) != len(must_be_unique):
                 raise ValueError(f"`{attribute}` list has repetitions")
         return must_be_unique
 
     return val
 
 
 def valutc(attribute: str):
-    def val(timestamp: datetime):
+    def val(timestamp: Optional[datetime]) -> Optional[datetime]:
         """
         Replacing `tzinfo` with `timezone.utc` is just required by SQLite data.
         If using Postgres, this function leaves the datetime exactly as it is.
         """
         if timestamp is not None:
             return timestamp.replace(tzinfo=timezone.utc)
         return None
```

### Comparing `fractal_server-2.0.0a6/fractal_server/app/schemas/state.py` & `fractal_server-2.0.0a8/fractal_server/app/schemas/state.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a6/fractal_server/app/schemas/user.py` & `fractal_server-2.0.0a8/fractal_server/app/schemas/user.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a6/fractal_server/app/schemas/v1/__init__.py` & `fractal_server-2.0.0a8/fractal_server/app/schemas/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a6/fractal_server/app/schemas/v1/applyworkflow.py` & `fractal_server-2.0.0a8/fractal_server/app/schemas/v1/applyworkflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a6/fractal_server/app/schemas/v1/dataset.py` & `fractal_server-2.0.0a8/fractal_server/app/schemas/v1/dataset.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a6/fractal_server/app/schemas/v1/dumps.py` & `fractal_server-2.0.0a8/fractal_server/app/schemas/v1/dumps.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a6/fractal_server/app/schemas/v1/manifest.py` & `fractal_server-2.0.0a8/fractal_server/app/schemas/v1/manifest.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a6/fractal_server/app/schemas/v1/project.py` & `fractal_server-2.0.0a8/fractal_server/app/schemas/v1/project.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a6/fractal_server/app/schemas/v1/task.py` & `fractal_server-2.0.0a8/fractal_server/app/schemas/v1/task.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a6/fractal_server/app/schemas/v1/task_collection.py` & `fractal_server-2.0.0a8/fractal_server/app/schemas/v1/task_collection.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a6/fractal_server/app/schemas/v1/workflow.py` & `fractal_server-2.0.0a8/fractal_server/app/schemas/v1/workflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a6/fractal_server/app/schemas/v2/__init__.py` & `fractal_server-2.0.0a8/fractal_server/app/schemas/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a6/fractal_server/app/schemas/v2/dataset.py` & `fractal_server-2.0.0a8/fractal_server/app/schemas/v2/dataset.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 from .._validators import valstr
 from .._validators import valutc
 from .dumps import WorkflowTaskDumpV2
 from .project import ProjectReadV2
 from .workflowtask import WorkflowTaskStatusTypeV2
 from fractal_server.images import Filters
+from fractal_server.urls import normalize_url
 
 
 class _DatasetHistoryItemV2(BaseModel):
     """
     Class for an item of `Dataset.history`.
     """
 
@@ -46,14 +47,18 @@
     name: str
 
     zarr_dir: str
 
     filters: Filters = Field(default_factory=Filters)
 
     # Validators
+    @validator("zarr_dir")
+    def normalize_zarr_dir(cls, v: str) -> str:
+        return normalize_url(v)
+
     _name = validator("name", allow_reuse=True)(valstr("name"))
 
 
 class DatasetReadV2(BaseModel):
 
     id: int
     name: str
@@ -79,8 +84,14 @@
         extra = "forbid"
 
     name: Optional[str]
     zarr_dir: Optional[str]
     filters: Optional[Filters]
 
     # Validators
+    @validator("zarr_dir")
+    def normalize_zarr_dir(cls, v: Optional[str]) -> Optional[str]:
+        if v is not None:
+            return normalize_url(v)
+        return v
+
     _name = validator("name", allow_reuse=True)(valstr("name"))
```

### Comparing `fractal_server-2.0.0a6/fractal_server/app/schemas/v2/dumps.py` & `fractal_server-2.0.0a8/fractal_server/app/schemas/v2/dumps.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a6/fractal_server/app/schemas/v2/job.py` & `fractal_server-2.0.0a8/fractal_server/app/schemas/v2/job.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a6/fractal_server/app/schemas/v2/manifest.py` & `fractal_server-2.0.0a8/fractal_server/app/schemas/v2/manifest.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a6/fractal_server/app/schemas/v2/project.py` & `fractal_server-2.0.0a8/fractal_server/app/schemas/v2/project.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a6/fractal_server/app/schemas/v2/task.py` & `fractal_server-2.0.0a8/fractal_server/app/schemas/v2/task.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a6/fractal_server/app/schemas/v2/task_collection.py` & `fractal_server-2.0.0a8/fractal_server/app/schemas/v2/task_collection.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a6/fractal_server/app/schemas/v2/workflow.py` & `fractal_server-2.0.0a8/fractal_server/app/schemas/v2/workflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a6/fractal_server/app/schemas/v2/workflowtask.py` & `fractal_server-2.0.0a8/fractal_server/app/schemas/v2/workflowtask.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a6/fractal_server/app/security/__init__.py` & `fractal_server-2.0.0a8/fractal_server/app/security/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a6/fractal_server/config.py` & `fractal_server-2.0.0a8/fractal_server/config.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a6/fractal_server/images/tools.py` & `fractal_server-2.0.0a8/fractal_server/images/tools.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a6/fractal_server/logger.py` & `fractal_server-2.0.0a8/fractal_server/logger.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a6/fractal_server/main.py` & `fractal_server-2.0.0a8/fractal_server/main.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a6/fractal_server/migrations/env.py` & `fractal_server-2.0.0a8/fractal_server/migrations/env.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a6/fractal_server/migrations/script.py.mako` & `fractal_server-2.0.0a8/fractal_server/migrations/script.py.mako`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a6/fractal_server/migrations/versions/4c308bcaea2b_add_task_args_schema_and_task_args_.py` & `fractal_server-2.0.0a8/fractal_server/migrations/versions/4c308bcaea2b_add_task_args_schema_and_task_args_.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a6/fractal_server/migrations/versions/4cedeb448a53_workflowtask_foreign_keys_not_nullables.py` & `fractal_server-2.0.0a8/fractal_server/migrations/versions/4cedeb448a53_workflowtask_foreign_keys_not_nullables.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a6/fractal_server/migrations/versions/50a13d6138fd_initial_schema.py` & `fractal_server-2.0.0a8/fractal_server/migrations/versions/50a13d6138fd_initial_schema.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a6/fractal_server/migrations/versions/70e77f1c38b0_add_applyworkflow_first_task_index_and_.py` & `fractal_server-2.0.0a8/fractal_server/migrations/versions/70e77f1c38b0_add_applyworkflow_first_task_index_and_.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a6/fractal_server/migrations/versions/71eefd1dd202_add_slurm_accounts.py` & `fractal_server-2.0.0a8/fractal_server/migrations/versions/71eefd1dd202_add_slurm_accounts.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a6/fractal_server/migrations/versions/80e12e1bc4fd_v2.py` & `fractal_server-2.0.0a8/fractal_server/migrations/versions/80e12e1bc4fd_v2.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a6/fractal_server/migrations/versions/84bf0fffde30_add_dumps_to_applyworkflow.py` & `fractal_server-2.0.0a8/fractal_server/migrations/versions/84bf0fffde30_add_dumps_to_applyworkflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a6/fractal_server/migrations/versions/8f79bd162e35_add_docs_info_and_docs_link_to_task_.py` & `fractal_server-2.0.0a8/fractal_server/migrations/versions/8f79bd162e35_add_docs_info_and_docs_link_to_task_.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a6/fractal_server/migrations/versions/97f444d47249_add_applyworkflow_project_dump.py` & `fractal_server-2.0.0a8/fractal_server/migrations/versions/97f444d47249_add_applyworkflow_project_dump.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a6/fractal_server/migrations/versions/99ea79d9e5d2_add_dataset_history.py` & `fractal_server-2.0.0a8/fractal_server/migrations/versions/99ea79d9e5d2_add_dataset_history.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a6/fractal_server/migrations/versions/9fd26a2b0de4_add_workflow_timestamp_created.py` & `fractal_server-2.0.0a8/fractal_server/migrations/versions/9fd26a2b0de4_add_workflow_timestamp_created.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a6/fractal_server/migrations/versions/a7f4d6137b53_add_workflow_dump_to_applyworkflow.py` & `fractal_server-2.0.0a8/fractal_server/migrations/versions/a7f4d6137b53_add_workflow_dump_to_applyworkflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a6/fractal_server/migrations/versions/d4fe3708d309_make_applyworkflow_workflow_dump_non_.py` & `fractal_server-2.0.0a8/fractal_server/migrations/versions/d4fe3708d309_make_applyworkflow_workflow_dump_non_.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a6/fractal_server/migrations/versions/e75cac726012_make_applyworkflow_start_timestamp_not_.py` & `fractal_server-2.0.0a8/fractal_server/migrations/versions/e75cac726012_make_applyworkflow_start_timestamp_not_.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a6/fractal_server/migrations/versions/efa89c30e0a4_add_project_timestamp_created.py` & `fractal_server-2.0.0a8/fractal_server/migrations/versions/efa89c30e0a4_add_project_timestamp_created.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a6/fractal_server/migrations/versions/f384e1c0cf5d_drop_task_default_args_columns.py` & `fractal_server-2.0.0a8/fractal_server/migrations/versions/f384e1c0cf5d_drop_task_default_args_columns.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a6/fractal_server/syringe.py` & `fractal_server-2.0.0a8/fractal_server/syringe.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a6/fractal_server/tasks/endpoint_operations.py` & `fractal_server-2.0.0a8/fractal_server/tasks/endpoint_operations.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a6/fractal_server/tasks/utils.py` & `fractal_server-2.0.0a8/fractal_server/tasks/utils.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a6/fractal_server/tasks/v1/_TaskCollectPip.py` & `fractal_server-2.0.0a8/fractal_server/tasks/v1/_TaskCollectPip.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a6/fractal_server/tasks/v1/background_operations.py` & `fractal_server-2.0.0a8/fractal_server/tasks/v1/background_operations.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a6/fractal_server/tasks/v2/_TaskCollectPip.py` & `fractal_server-2.0.0a8/fractal_server/tasks/v2/_TaskCollectPip.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a6/fractal_server/tasks/v2/background_operations.py` & `fractal_server-2.0.0a8/fractal_server/tasks/v2/background_operations.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a6/fractal_server/utils.py` & `fractal_server-2.0.0a8/fractal_server/utils.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a6/pyproject.toml` & `fractal_server-2.0.0a8/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fractal-server"
-version = "2.0.0a6"
+version = "2.0.0a8"
 description = "Server component of the Fractal analytics platform"
 authors = [
     "Jacopo Nespolo <jacopo.nespolo@exact-lab.it>",
     "Marco Franzon <marco.franzon@exact-lab.it>",
     "Tommaso Comparin <tommaso.comparin@exact-lab.it>",
 ]
 readme = "README.md"
@@ -82,15 +82,15 @@
 asyncio_mode = "auto"
 filterwarnings = [
     "error::RuntimeWarning",
     "error::pytest.PytestUnraisableExceptionWarning",
 ]
 
 [tool.bumpver]
-current_version = "2.0.0a6"
+current_version = "2.0.0a8"
 version_pattern = "MAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `fractal_server-2.0.0a6/PKG-INFO` & `fractal_server-2.0.0a8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fractal-server
-Version: 2.0.0a6
+Version: 2.0.0a8
 Summary: Server component of the Fractal analytics platform
 Home-page: https://github.com/fractal-analytics-platform/fractal-server
 License: BSD-3-Clause
 Author: Jacopo Nespolo
 Author-email: jacopo.nespolo@exact-lab.it
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: BSD License
```

