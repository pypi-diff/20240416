# Comparing `tmp/anylearn-0.20.1rc1.tar.gz` & `tmp/anylearn-0.20.2rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anylearn-0.20.1rc1.tar", last modified: Mon Mar 18 09:59:36 2024, max compression
+gzip compressed data, was "anylearn-0.20.2rc1.tar", last modified: Mon Apr 15 13:48:26 2024, max compression
```

## Comparing `anylearn-0.20.1rc1.tar` & `anylearn-0.20.2rc1.tar`

### file list

```diff
@@ -1,111 +1,111 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 09:59:35.995708 anylearn-0.20.1rc1/
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-03-18 09:59:31.000000 anylearn-0.20.1rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-03-18 09:59:35.995708 anylearn-0.20.1rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-03-18 09:59:31.000000 anylearn-0.20.1rc1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 09:59:35.975708 anylearn-0.20.1rc1/anylearn/
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-03-18 09:59:31.000000 anylearn-0.20.1rc1/anylearn/__about__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-03-18 09:59:31.000000 anylearn-0.20.1rc1/anylearn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 09:59:35.979708 anylearn-0.20.1rc1/anylearn/analyzers/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-03-18 09:59:31.000000 anylearn-0.20.1rc1/anylearn/analyzers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8798 2024-03-18 09:59:31.000000 anylearn-0.20.1rc1/anylearn/analyzers/artifact_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 09:59:35.979708 anylearn-0.20.1rc1/anylearn/applications/
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-03-18 09:59:31.000000 anylearn-0.20.1rc1/anylearn/applications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8925 2024-03-18 09:59:31.000000 anylearn-0.20.1rc1/anylearn/applications/algorithm_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1862 2024-03-18 09:59:31.000000 anylearn-0.20.1rc1/anylearn/applications/git_progress_printer.py
--rw-r--r--   0 runner    (1001) docker     (127)    22035 2024-03-18 09:59:31.000000 anylearn-0.20.1rc1/anylearn/applications/quickstart.py
--rw-r--r--   0 runner    (1001) docker     (127)     1926 2024-03-18 09:59:31.000000 anylearn-0.20.1rc1/anylearn/applications/tracking.py
--rw-r--r--   0 runner    (1001) docker     (127)     4409 2024-03-18 09:59:31.000000 anylearn-0.20.1rc1/anylearn/applications/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 09:59:35.979708 anylearn-0.20.1rc1/anylearn/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 09:59:31.000000 anylearn-0.20.1rc1/anylearn/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-03-18 09:59:31.000000 anylearn-0.20.1rc1/anylearn/cli/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      981 2024-03-18 09:59:31.000000 anylearn-0.20.1rc1/anylearn/cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     7944 2024-03-18 09:59:31.000000 anylearn-0.20.1rc1/anylearn/cli/jupload.py
--rw-r--r--   0 runner    (1001) docker     (127)     6190 2024-03-18 09:59:31.000000 anylearn-0.20.1rc1/anylearn/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-03-18 09:59:31.000000 anylearn-0.20.1rc1/anylearn/env.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 09:59:35.983708 anylearn-0.20.1rc1/anylearn/interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-03-18 09:59:31.000000 anylearn-0.20.1rc1/anylearn/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5756 2024-03-18 09:59:31.000000 anylearn-0.20.1rc1/anylearn/interfaces/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-03-18 09:59:31.000000 anylearn-0.20.1rc1/anylearn/interfaces/mirror.py
--rw-r--r--   0 runner    (1001) docker     (127)     7832 2024-03-18 09:59:31.000000 anylearn-0.20.1rc1/anylearn/interfaces/project.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 09:59:35.983708 anylearn-0.20.1rc1/anylearn/interfaces/quota/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-03-18 09:59:31.000000 anylearn-0.20.1rc1/anylearn/interfaces/quota/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4662 2024-03-18 09:59:31.000000 anylearn-0.20.1rc1/anylearn/interfaces/quota/group.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 09:59:35.983708 anylearn-0.20.1rc1/anylearn/interfaces/resource/
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-03-18 09:59:31.000000 anylearn-0.20.1rc1/anylearn/interfaces/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13140 2024-03-18 09:59:31.000000 anylearn-0.20.1rc1/anylearn/interfaces/resource/algorithm.py
--rw-r--r--   0 runner    (1001) docker     (127)     6228 2024-03-18 09:59:31.000000 anylearn-0.20.1rc1/anylearn/interfaces/resource/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     5456 2024-03-18 09:59:31.000000 anylearn-0.20.1rc1/anylearn/interfaces/resource/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     5765 2024-03-18 09:59:31.000000 anylearn-0.20.1rc1/anylearn/interfaces/resource/model.py
--rw-r--r--   0 runner    (1001) docker     (127)    10223 2024-03-18 09:59:31.000000 anylearn-0.20.1rc1/anylearn/interfaces/resource/resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     3186 2024-03-18 09:59:31.000000 anylearn-0.20.1rc1/anylearn/interfaces/resource/resource_downloader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-03-18 09:59:31.000000 anylearn-0.20.1rc1/anylearn/interfaces/resource/resource_uploader.py
--rw-r--r--   0 runner    (1001) docker     (127)     3325 2024-03-18 09:59:31.000000 anylearn-0.20.1rc1/anylearn/interfaces/train_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)    25452 2024-03-18 09:59:31.000000 anylearn-0.20.1rc1/anylearn/interfaces/train_task.py
--rw-r--r--   0 runner    (1001) docker     (127)     8365 2024-03-18 09:59:31.000000 anylearn-0.20.1rc1/anylearn/interfaces/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 09:59:35.987708 anylearn-0.20.1rc1/anylearn/sdk/
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-03-18 09:59:31.000000 anylearn-0.20.1rc1/anylearn/sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 09:59:35.987708 anylearn-0.20.1rc1/anylearn/sdk/artifacts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 09:59:31.000000 anylearn-0.20.1rc1/anylearn/sdk/artifacts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-03-18 09:59:31.000000 anylearn-0.20.1rc1/anylearn/sdk/artifacts/algorithm.py
--rw-r--r--   0 runner    (1001) docker     (127)     5516 2024-03-18 09:59:31.000000 anylearn-0.20.1rc1/anylearn/sdk/artifacts/artifact.py
--rw-r--r--   0 runner    (1001) docker     (127)     3742 2024-03-18 09:59:31.000000 anylearn-0.20.1rc1/anylearn/sdk/artifacts/compression.py
--rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-03-18 09:59:31.000000 anylearn-0.20.1rc1/anylearn/sdk/artifacts/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-03-18 09:59:31.000000 anylearn-0.20.1rc1/anylearn/sdk/artifacts/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-03-18 09:59:31.000000 anylearn-0.20.1rc1/anylearn/sdk/artifacts/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     9000 2024-03-18 09:59:31.000000 anylearn-0.20.1rc1/anylearn/sdk/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-03-18 09:59:31.000000 anylearn-0.20.1rc1/anylearn/sdk/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-03-18 09:59:31.000000 anylearn-0.20.1rc1/anylearn/sdk/console.py
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-03-18 09:59:31.000000 anylearn-0.20.1rc1/anylearn/sdk/context.py
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-03-18 09:59:31.000000 anylearn-0.20.1rc1/anylearn/sdk/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 09:59:35.987708 anylearn-0.20.1rc1/anylearn/sdk/jumps/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 09:59:31.000000 anylearn-0.20.1rc1/anylearn/sdk/jumps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7354 2024-03-18 09:59:31.000000 anylearn-0.20.1rc1/anylearn/sdk/jumps/channel.py
--rw-r--r--   0 runner    (1001) docker     (127)     5842 2024-03-18 09:59:31.000000 anylearn-0.20.1rc1/anylearn/sdk/jumps/uploader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-03-18 09:59:31.000000 anylearn-0.20.1rc1/anylearn/sdk/project.py
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-03-18 09:59:31.000000 anylearn-0.20.1rc1/anylearn/sdk/sshkey.py
--rw-r--r--   0 runner    (1001) docker     (127)     3969 2024-03-18 09:59:31.000000 anylearn-0.20.1rc1/anylearn/sdk/task.py
--rw-r--r--   0 runner    (1001) docker     (127)     2877 2024-03-18 09:59:31.000000 anylearn-0.20.1rc1/anylearn/sdk/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 09:59:35.991708 anylearn-0.20.1rc1/anylearn/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-03-18 09:59:31.000000 anylearn-0.20.1rc1/anylearn/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3594 2024-03-18 09:59:31.000000 anylearn-0.20.1rc1/anylearn/utils/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-03-18 09:59:31.000000 anylearn-0.20.1rc1/anylearn/utils/cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-03-18 09:59:31.000000 anylearn-0.20.1rc1/anylearn/utils/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-03-18 09:59:31.000000 anylearn-0.20.1rc1/anylearn/utils/func.py
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-03-18 09:59:31.000000 anylearn-0.20.1rc1/anylearn/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-03-18 09:59:31.000000 anylearn-0.20.1rc1/anylearn/utils/singleton.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 09:59:35.995708 anylearn-0.20.1rc1/anylearn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-03-18 09:59:35.000000 anylearn-0.20.1rc1/anylearn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-03-18 09:59:35.000000 anylearn-0.20.1rc1/anylearn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-18 09:59:35.000000 anylearn-0.20.1rc1/anylearn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-18 09:59:35.000000 anylearn-0.20.1rc1/anylearn.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-03-18 09:59:35.000000 anylearn-0.20.1rc1/anylearn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-18 09:59:35.000000 anylearn-0.20.1rc1/anylearn.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-03-18 09:59:31.000000 anylearn-0.20.1rc1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-18 09:59:35.995708 anylearn-0.20.1rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-03-18 09:59:31.000000 anylearn-0.20.1rc1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 09:59:35.991708 anylearn-0.20.1rc1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 09:59:31.000000 anylearn-0.20.1rc1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 09:59:35.991708 anylearn-0.20.1rc1/tests/analyzers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 09:59:31.000000 anylearn-0.20.1rc1/tests/analyzers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-03-18 09:59:31.000000 anylearn-0.20.1rc1/tests/analyzers/test_artifact_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 09:59:35.991708 anylearn-0.20.1rc1/tests/applications/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 09:59:31.000000 anylearn-0.20.1rc1/tests/applications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14164 2024-03-18 09:59:31.000000 anylearn-0.20.1rc1/tests/applications/test_quick_train.py
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-03-18 09:59:31.000000 anylearn-0.20.1rc1/tests/base_test_case.py
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-03-18 09:59:31.000000 anylearn-0.20.1rc1/tests/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 09:59:35.991708 anylearn-0.20.1rc1/tests/interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 09:59:31.000000 anylearn-0.20.1rc1/tests/interfaces/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 09:59:35.995708 anylearn-0.20.1rc1/tests/interfaces/resource/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 09:59:31.000000 anylearn-0.20.1rc1/tests/interfaces/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15601 2024-03-18 09:59:31.000000 anylearn-0.20.1rc1/tests/interfaces/resource/test_algorithm.py
--rw-r--r--   0 runner    (1001) docker     (127)    11502 2024-03-18 09:59:31.000000 anylearn-0.20.1rc1/tests/interfaces/resource/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    11053 2024-03-18 09:59:31.000000 anylearn-0.20.1rc1/tests/interfaces/resource/test_file.py
--rw-r--r--   0 runner    (1001) docker     (127)    10728 2024-03-18 09:59:31.000000 anylearn-0.20.1rc1/tests/interfaces/resource/test_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4343 2024-03-18 09:59:31.000000 anylearn-0.20.1rc1/tests/interfaces/resource/test_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-03-18 09:59:31.000000 anylearn-0.20.1rc1/tests/interfaces/resource/test_resource_downloader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-03-18 09:59:31.000000 anylearn-0.20.1rc1/tests/interfaces/test_mirror.py
--rw-r--r--   0 runner    (1001) docker     (127)    11529 2024-03-18 09:59:31.000000 anylearn-0.20.1rc1/tests/interfaces/test_project.py
--rw-r--r--   0 runner    (1001) docker     (127)    30702 2024-03-18 09:59:31.000000 anylearn-0.20.1rc1/tests/interfaces/test_train_task.py
--rw-r--r--   0 runner    (1001) docker     (127)    14924 2024-03-18 09:59:31.000000 anylearn-0.20.1rc1/tests/interfaces/test_user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 09:59:35.995708 anylearn-0.20.1rc1/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 09:59:31.000000 anylearn-0.20.1rc1/tests/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:48:26.544346 anylearn-0.20.2rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-15 13:48:18.000000 anylearn-0.20.2rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-04-15 13:48:26.544346 anylearn-0.20.2rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-15 13:48:18.000000 anylearn-0.20.2rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:48:26.524346 anylearn-0.20.2rc1/anylearn/
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-15 13:48:18.000000 anylearn-0.20.2rc1/anylearn/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-04-15 13:48:18.000000 anylearn-0.20.2rc1/anylearn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:48:26.528346 anylearn-0.20.2rc1/anylearn/analyzers/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-15 13:48:18.000000 anylearn-0.20.2rc1/anylearn/analyzers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8798 2024-04-15 13:48:18.000000 anylearn-0.20.2rc1/anylearn/analyzers/artifact_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:48:26.528346 anylearn-0.20.2rc1/anylearn/applications/
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-15 13:48:18.000000 anylearn-0.20.2rc1/anylearn/applications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8925 2024-04-15 13:48:18.000000 anylearn-0.20.2rc1/anylearn/applications/algorithm_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1862 2024-04-15 13:48:18.000000 anylearn-0.20.2rc1/anylearn/applications/git_progress_printer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22035 2024-04-15 13:48:18.000000 anylearn-0.20.2rc1/anylearn/applications/quickstart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1926 2024-04-15 13:48:18.000000 anylearn-0.20.2rc1/anylearn/applications/tracking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4409 2024-04-15 13:48:18.000000 anylearn-0.20.2rc1/anylearn/applications/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:48:26.528346 anylearn-0.20.2rc1/anylearn/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:48:18.000000 anylearn-0.20.2rc1/anylearn/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-15 13:48:18.000000 anylearn-0.20.2rc1/anylearn/cli/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-04-15 13:48:18.000000 anylearn-0.20.2rc1/anylearn/cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7944 2024-04-15 13:48:18.000000 anylearn-0.20.2rc1/anylearn/cli/jupload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6190 2024-04-15 13:48:18.000000 anylearn-0.20.2rc1/anylearn/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-04-15 13:48:18.000000 anylearn-0.20.2rc1/anylearn/env.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:48:26.528346 anylearn-0.20.2rc1/anylearn/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-15 13:48:18.000000 anylearn-0.20.2rc1/anylearn/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5756 2024-04-15 13:48:18.000000 anylearn-0.20.2rc1/anylearn/interfaces/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-04-15 13:48:18.000000 anylearn-0.20.2rc1/anylearn/interfaces/mirror.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7832 2024-04-15 13:48:18.000000 anylearn-0.20.2rc1/anylearn/interfaces/project.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:48:26.532346 anylearn-0.20.2rc1/anylearn/interfaces/quota/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-15 13:48:18.000000 anylearn-0.20.2rc1/anylearn/interfaces/quota/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4662 2024-04-15 13:48:18.000000 anylearn-0.20.2rc1/anylearn/interfaces/quota/group.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:48:26.532346 anylearn-0.20.2rc1/anylearn/interfaces/resource/
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-15 13:48:18.000000 anylearn-0.20.2rc1/anylearn/interfaces/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13140 2024-04-15 13:48:18.000000 anylearn-0.20.2rc1/anylearn/interfaces/resource/algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6228 2024-04-15 13:48:18.000000 anylearn-0.20.2rc1/anylearn/interfaces/resource/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5456 2024-04-15 13:48:18.000000 anylearn-0.20.2rc1/anylearn/interfaces/resource/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5765 2024-04-15 13:48:18.000000 anylearn-0.20.2rc1/anylearn/interfaces/resource/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10223 2024-04-15 13:48:18.000000 anylearn-0.20.2rc1/anylearn/interfaces/resource/resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3186 2024-04-15 13:48:18.000000 anylearn-0.20.2rc1/anylearn/interfaces/resource/resource_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-15 13:48:18.000000 anylearn-0.20.2rc1/anylearn/interfaces/resource/resource_uploader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3325 2024-04-15 13:48:18.000000 anylearn-0.20.2rc1/anylearn/interfaces/train_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25452 2024-04-15 13:48:18.000000 anylearn-0.20.2rc1/anylearn/interfaces/train_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8365 2024-04-15 13:48:18.000000 anylearn-0.20.2rc1/anylearn/interfaces/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:48:26.536346 anylearn-0.20.2rc1/anylearn/sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-15 13:48:18.000000 anylearn-0.20.2rc1/anylearn/sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:48:26.536346 anylearn-0.20.2rc1/anylearn/sdk/artifacts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:48:18.000000 anylearn-0.20.2rc1/anylearn/sdk/artifacts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-15 13:48:18.000000 anylearn-0.20.2rc1/anylearn/sdk/artifacts/algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5516 2024-04-15 13:48:18.000000 anylearn-0.20.2rc1/anylearn/sdk/artifacts/artifact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3742 2024-04-15 13:48:18.000000 anylearn-0.20.2rc1/anylearn/sdk/artifacts/compression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-04-15 13:48:18.000000 anylearn-0.20.2rc1/anylearn/sdk/artifacts/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-15 13:48:18.000000 anylearn-0.20.2rc1/anylearn/sdk/artifacts/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-04-15 13:48:18.000000 anylearn-0.20.2rc1/anylearn/sdk/artifacts/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9000 2024-04-15 13:48:18.000000 anylearn-0.20.2rc1/anylearn/sdk/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-04-15 13:48:18.000000 anylearn-0.20.2rc1/anylearn/sdk/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-15 13:48:18.000000 anylearn-0.20.2rc1/anylearn/sdk/console.py
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-15 13:48:18.000000 anylearn-0.20.2rc1/anylearn/sdk/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-15 13:48:18.000000 anylearn-0.20.2rc1/anylearn/sdk/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:48:26.536346 anylearn-0.20.2rc1/anylearn/sdk/jumps/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:48:18.000000 anylearn-0.20.2rc1/anylearn/sdk/jumps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7354 2024-04-15 13:48:18.000000 anylearn-0.20.2rc1/anylearn/sdk/jumps/channel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5842 2024-04-15 13:48:18.000000 anylearn-0.20.2rc1/anylearn/sdk/jumps/uploader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-04-15 13:48:18.000000 anylearn-0.20.2rc1/anylearn/sdk/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-04-15 13:48:18.000000 anylearn-0.20.2rc1/anylearn/sdk/sshkey.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3969 2024-04-15 13:48:18.000000 anylearn-0.20.2rc1/anylearn/sdk/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2877 2024-04-15 13:48:18.000000 anylearn-0.20.2rc1/anylearn/sdk/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:48:26.536346 anylearn-0.20.2rc1/anylearn/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-15 13:48:18.000000 anylearn-0.20.2rc1/anylearn/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3594 2024-04-15 13:48:18.000000 anylearn-0.20.2rc1/anylearn/utils/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-15 13:48:18.000000 anylearn-0.20.2rc1/anylearn/utils/cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-04-15 13:48:18.000000 anylearn-0.20.2rc1/anylearn/utils/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-15 13:48:18.000000 anylearn-0.20.2rc1/anylearn/utils/func.py
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-15 13:48:18.000000 anylearn-0.20.2rc1/anylearn/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-15 13:48:18.000000 anylearn-0.20.2rc1/anylearn/utils/singleton.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:48:26.544346 anylearn-0.20.2rc1/anylearn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-04-15 13:48:26.000000 anylearn-0.20.2rc1/anylearn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-04-15 13:48:26.000000 anylearn-0.20.2rc1/anylearn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 13:48:26.000000 anylearn-0.20.2rc1/anylearn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-15 13:48:26.000000 anylearn-0.20.2rc1/anylearn.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-15 13:48:26.000000 anylearn-0.20.2rc1/anylearn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-15 13:48:26.000000 anylearn-0.20.2rc1/anylearn.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-15 13:48:18.000000 anylearn-0.20.2rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 13:48:26.544346 anylearn-0.20.2rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-04-15 13:48:18.000000 anylearn-0.20.2rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:48:26.540346 anylearn-0.20.2rc1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:48:18.000000 anylearn-0.20.2rc1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:48:26.540346 anylearn-0.20.2rc1/tests/analyzers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:48:18.000000 anylearn-0.20.2rc1/tests/analyzers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-15 13:48:18.000000 anylearn-0.20.2rc1/tests/analyzers/test_artifact_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:48:26.540346 anylearn-0.20.2rc1/tests/applications/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:48:18.000000 anylearn-0.20.2rc1/tests/applications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14164 2024-04-15 13:48:18.000000 anylearn-0.20.2rc1/tests/applications/test_quick_train.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-15 13:48:18.000000 anylearn-0.20.2rc1/tests/base_test_case.py
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-15 13:48:18.000000 anylearn-0.20.2rc1/tests/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:48:26.540346 anylearn-0.20.2rc1/tests/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:48:18.000000 anylearn-0.20.2rc1/tests/interfaces/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:48:26.540346 anylearn-0.20.2rc1/tests/interfaces/resource/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:48:18.000000 anylearn-0.20.2rc1/tests/interfaces/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15601 2024-04-15 13:48:18.000000 anylearn-0.20.2rc1/tests/interfaces/resource/test_algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11502 2024-04-15 13:48:18.000000 anylearn-0.20.2rc1/tests/interfaces/resource/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11053 2024-04-15 13:48:18.000000 anylearn-0.20.2rc1/tests/interfaces/resource/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10728 2024-04-15 13:48:18.000000 anylearn-0.20.2rc1/tests/interfaces/resource/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4343 2024-04-15 13:48:18.000000 anylearn-0.20.2rc1/tests/interfaces/resource/test_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-04-15 13:48:18.000000 anylearn-0.20.2rc1/tests/interfaces/resource/test_resource_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-04-15 13:48:18.000000 anylearn-0.20.2rc1/tests/interfaces/test_mirror.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11529 2024-04-15 13:48:18.000000 anylearn-0.20.2rc1/tests/interfaces/test_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30702 2024-04-15 13:48:18.000000 anylearn-0.20.2rc1/tests/interfaces/test_train_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14924 2024-04-15 13:48:18.000000 anylearn-0.20.2rc1/tests/interfaces/test_user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:48:26.544346 anylearn-0.20.2rc1/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:48:18.000000 anylearn-0.20.2rc1/tests/utils/__init__.py
```

### Comparing `anylearn-0.20.1rc1/PKG-INFO` & `anylearn-0.20.2rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anylearn
-Version: 0.20.1rc1
+Version: 0.20.2rc1
 Summary: Anylearn Python SDK
 Author: Dmagine
 Author-email: anylearn@nelbds.org.cn
 License: Proprietary
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
```

### Comparing `anylearn-0.20.1rc1/README.md` & `anylearn-0.20.2rc1/README.md`

 * *Files identical despite different names*

### Comparing `anylearn-0.20.1rc1/anylearn/__init__.py` & `anylearn-0.20.2rc1/anylearn/__init__.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.20.1rc1/anylearn/analyzers/artifact_collector.py` & `anylearn-0.20.2rc1/anylearn/analyzers/artifact_collector.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.20.1rc1/anylearn/applications/algorithm_manager.py` & `anylearn-0.20.2rc1/anylearn/applications/algorithm_manager.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.20.1rc1/anylearn/applications/git_progress_printer.py` & `anylearn-0.20.2rc1/anylearn/applications/git_progress_printer.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.20.1rc1/anylearn/applications/quickstart.py` & `anylearn-0.20.2rc1/anylearn/applications/quickstart.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.20.1rc1/anylearn/applications/tracking.py` & `anylearn-0.20.2rc1/anylearn/applications/tracking.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.20.1rc1/anylearn/applications/utils.py` & `anylearn-0.20.2rc1/anylearn/applications/utils.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.20.1rc1/anylearn/cli/cli.py` & `anylearn-0.20.2rc1/anylearn/cli/cli.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.20.1rc1/anylearn/cli/jupload.py` & `anylearn-0.20.2rc1/anylearn/cli/jupload.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.20.1rc1/anylearn/config.py` & `anylearn-0.20.2rc1/anylearn/config.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.20.1rc1/anylearn/env.py` & `anylearn-0.20.2rc1/anylearn/env.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.20.1rc1/anylearn/interfaces/base.py` & `anylearn-0.20.2rc1/anylearn/interfaces/base.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.20.1rc1/anylearn/interfaces/mirror.py` & `anylearn-0.20.2rc1/anylearn/interfaces/mirror.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.20.1rc1/anylearn/interfaces/project.py` & `anylearn-0.20.2rc1/anylearn/interfaces/project.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.20.1rc1/anylearn/interfaces/quota/group.py` & `anylearn-0.20.2rc1/anylearn/interfaces/quota/group.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.20.1rc1/anylearn/interfaces/resource/algorithm.py` & `anylearn-0.20.2rc1/anylearn/interfaces/resource/algorithm.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.20.1rc1/anylearn/interfaces/resource/dataset.py` & `anylearn-0.20.2rc1/anylearn/interfaces/resource/dataset.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.20.1rc1/anylearn/interfaces/resource/file.py` & `anylearn-0.20.2rc1/anylearn/interfaces/resource/file.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.20.1rc1/anylearn/interfaces/resource/model.py` & `anylearn-0.20.2rc1/anylearn/interfaces/resource/model.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.20.1rc1/anylearn/interfaces/resource/resource.py` & `anylearn-0.20.2rc1/anylearn/interfaces/resource/resource.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.20.1rc1/anylearn/interfaces/resource/resource_downloader.py` & `anylearn-0.20.2rc1/anylearn/interfaces/resource/resource_downloader.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.20.1rc1/anylearn/interfaces/resource/resource_uploader.py` & `anylearn-0.20.2rc1/anylearn/interfaces/resource/resource_uploader.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.20.1rc1/anylearn/interfaces/train_tag.py` & `anylearn-0.20.2rc1/anylearn/interfaces/train_tag.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.20.1rc1/anylearn/interfaces/train_task.py` & `anylearn-0.20.2rc1/anylearn/interfaces/train_task.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.20.1rc1/anylearn/interfaces/user.py` & `anylearn-0.20.2rc1/anylearn/interfaces/user.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.20.1rc1/anylearn/sdk/artifacts/algorithm.py` & `anylearn-0.20.2rc1/anylearn/sdk/artifacts/algorithm.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.20.1rc1/anylearn/sdk/artifacts/artifact.py` & `anylearn-0.20.2rc1/anylearn/sdk/artifacts/artifact.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.20.1rc1/anylearn/sdk/artifacts/compression.py` & `anylearn-0.20.2rc1/anylearn/sdk/artifacts/compression.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.20.1rc1/anylearn/sdk/artifacts/dataset.py` & `anylearn-0.20.2rc1/anylearn/sdk/artifacts/dataset.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.20.1rc1/anylearn/sdk/artifacts/file.py` & `anylearn-0.20.2rc1/anylearn/sdk/artifacts/file.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.20.1rc1/anylearn/sdk/artifacts/model.py` & `anylearn-0.20.2rc1/anylearn/sdk/artifacts/model.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.20.1rc1/anylearn/sdk/auth.py` & `anylearn-0.20.2rc1/anylearn/sdk/auth.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.20.1rc1/anylearn/sdk/client.py` & `anylearn-0.20.2rc1/anylearn/sdk/client.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.20.1rc1/anylearn/sdk/errors.py` & `anylearn-0.20.2rc1/anylearn/sdk/errors.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.20.1rc1/anylearn/sdk/jumps/channel.py` & `anylearn-0.20.2rc1/anylearn/sdk/jumps/channel.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.20.1rc1/anylearn/sdk/jumps/uploader.py` & `anylearn-0.20.2rc1/anylearn/sdk/jumps/uploader.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.20.1rc1/anylearn/sdk/project.py` & `anylearn-0.20.2rc1/anylearn/sdk/project.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.20.1rc1/anylearn/sdk/sshkey.py` & `anylearn-0.20.2rc1/anylearn/sdk/sshkey.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.20.1rc1/anylearn/sdk/task.py` & `anylearn-0.20.2rc1/anylearn/sdk/task.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.20.1rc1/anylearn/sdk/utils.py` & `anylearn-0.20.2rc1/anylearn/sdk/utils.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.20.1rc1/anylearn/utils/api.py` & `anylearn-0.20.2rc1/anylearn/utils/api.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.20.1rc1/anylearn/utils/errors.py` & `anylearn-0.20.2rc1/anylearn/utils/errors.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.20.1rc1/anylearn/utils/func.py` & `anylearn-0.20.2rc1/anylearn/utils/func.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.20.1rc1/anylearn.egg-info/PKG-INFO` & `anylearn-0.20.2rc1/anylearn.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anylearn
-Version: 0.20.1rc1
+Version: 0.20.2rc1
 Summary: Anylearn Python SDK
 Author: Dmagine
 Author-email: anylearn@nelbds.org.cn
 License: Proprietary
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
```

### Comparing `anylearn-0.20.1rc1/anylearn.egg-info/SOURCES.txt` & `anylearn-0.20.2rc1/anylearn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `anylearn-0.20.1rc1/setup.py` & `anylearn-0.20.2rc1/setup.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.20.1rc1/tests/analyzers/test_artifact_collector.py` & `anylearn-0.20.2rc1/tests/analyzers/test_artifact_collector.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.20.1rc1/tests/applications/test_quick_train.py` & `anylearn-0.20.2rc1/tests/applications/test_quick_train.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.20.1rc1/tests/base_test_case.py` & `anylearn-0.20.2rc1/tests/base_test_case.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.20.1rc1/tests/interfaces/resource/test_algorithm.py` & `anylearn-0.20.2rc1/tests/interfaces/resource/test_algorithm.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.20.1rc1/tests/interfaces/resource/test_dataset.py` & `anylearn-0.20.2rc1/tests/interfaces/resource/test_dataset.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.20.1rc1/tests/interfaces/resource/test_file.py` & `anylearn-0.20.2rc1/tests/interfaces/resource/test_file.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.20.1rc1/tests/interfaces/resource/test_model.py` & `anylearn-0.20.2rc1/tests/interfaces/resource/test_model.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.20.1rc1/tests/interfaces/resource/test_resource.py` & `anylearn-0.20.2rc1/tests/interfaces/resource/test_resource.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.20.1rc1/tests/interfaces/resource/test_resource_downloader.py` & `anylearn-0.20.2rc1/tests/interfaces/resource/test_resource_downloader.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.20.1rc1/tests/interfaces/test_mirror.py` & `anylearn-0.20.2rc1/tests/interfaces/test_mirror.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.20.1rc1/tests/interfaces/test_project.py` & `anylearn-0.20.2rc1/tests/interfaces/test_project.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.20.1rc1/tests/interfaces/test_train_task.py` & `anylearn-0.20.2rc1/tests/interfaces/test_train_task.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.20.1rc1/tests/interfaces/test_user.py` & `anylearn-0.20.2rc1/tests/interfaces/test_user.py`

 * *Files identical despite different names*

