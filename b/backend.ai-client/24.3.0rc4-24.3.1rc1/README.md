# Comparing `tmp/backend.ai-client-24.3.0rc4.tar.gz` & `tmp/backend.ai-client-24.3.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backend.ai-client-24.3.0rc4.tar", last modified: Fri Apr  5 03:40:02 2024, max compression
+gzip compressed data, was "backend.ai-client-24.3.1rc1.tar", last modified: Tue Apr 16 17:08:33 2024, max compression
```

## Comparing `backend.ai-client-24.3.0rc4.tar` & `backend.ai-client-24.3.1rc1.tar`

### file list

```diff
@@ -1,114 +1,114 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:40:02.005385 backend.ai-client-24.3.0rc4/
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-05 03:40:00.000000 backend.ai-client-24.3.0rc4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9350 2024-04-05 03:40:02.005385 backend.ai-client-24.3.0rc4/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:40:01.985385 backend.ai-client-24.3.0rc4/ai/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:40:01.985385 backend.ai-client-24.3.0rc4/ai/backend/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:40:01.989385 backend.ai-client-24.3.0rc4/ai/backend/client/
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-05 03:40:00.000000 backend.ai-client-24.3.0rc4/ai/backend/client/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-05 03:40:00.000000 backend.ai-client-24.3.0rc4/ai/backend/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-04-05 03:40:00.000000 backend.ai-client-24.3.0rc4/ai/backend/client/auth.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:40:01.993385 backend.ai-client-24.3.0rc4/ai/backend/client/cli/
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-05 03:40:00.000000 backend.ai-client-24.3.0rc4/ai/backend/client/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:40:01.997385 backend.ai-client-24.3.0rc4/ai/backend/client/cli/admin/
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-05 03:40:00.000000 backend.ai-client-24.3.0rc4/ai/backend/client/cli/admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-05 03:40:00.000000 backend.ai-client-24.3.0rc4/ai/backend/client/cli/admin/acl.py
--rw-r--r--   0 runner    (1001) docker     (127)     5143 2024-04-05 03:40:00.000000 backend.ai-client-24.3.0rc4/ai/backend/client/cli/admin/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     8230 2024-04-05 03:40:00.000000 backend.ai-client-24.3.0rc4/ai/backend/client/cli/admin/domain.py
--rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-04-05 03:40:00.000000 backend.ai-client-24.3.0rc4/ai/backend/client/cli/admin/etcd.py
--rw-r--r--   0 runner    (1001) docker     (127)    11198 2024-04-05 03:40:00.000000 backend.ai-client-24.3.0rc4/ai/backend/client/cli/admin/group.py
--rw-r--r--   0 runner    (1001) docker     (127)     4545 2024-04-05 03:40:00.000000 backend.ai-client-24.3.0rc4/ai/backend/client/cli/admin/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     9909 2024-04-05 03:40:00.000000 backend.ai-client-24.3.0rc4/ai/backend/client/cli/admin/keypair.py
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-04-05 03:40:00.000000 backend.ai-client-24.3.0rc4/ai/backend/client/cli/admin/license.py
--rw-r--r--   0 runner    (1001) docker     (127)     6297 2024-04-05 03:40:00.000000 backend.ai-client-24.3.0rc4/ai/backend/client/cli/admin/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     6930 2024-04-05 03:40:00.000000 backend.ai-client-24.3.0rc4/ai/backend/client/cli/admin/quota_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)     6383 2024-04-05 03:40:00.000000 backend.ai-client-24.3.0rc4/ai/backend/client/cli/admin/resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     9478 2024-04-05 03:40:00.000000 backend.ai-client-24.3.0rc4/ai/backend/client/cli/admin/resource_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    11704 2024-04-05 03:40:00.000000 backend.ai-client-24.3.0rc4/ai/backend/client/cli/admin/scaling_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     9694 2024-04-05 03:40:00.000000 backend.ai-client-24.3.0rc4/ai/backend/client/cli/admin/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-04-05 03:40:00.000000 backend.ai-client-24.3.0rc4/ai/backend/client/cli/admin/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)    15514 2024-04-05 03:40:00.000000 backend.ai-client-24.3.0rc4/ai/backend/client/cli/admin/user.py
--rw-r--r--   0 runner    (1001) docker     (127)    12201 2024-04-05 03:40:00.000000 backend.ai-client-24.3.0rc4/ai/backend/client/cli/admin/vfolder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-04-05 03:40:00.000000 backend.ai-client-24.3.0rc4/ai/backend/client/cli/announcement.py
--rw-r--r--   0 runner    (1001) docker     (127)    12150 2024-04-05 03:40:00.000000 backend.ai-client-24.3.0rc4/ai/backend/client/cli/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     7991 2024-04-05 03:40:00.000000 backend.ai-client-24.3.0rc4/ai/backend/client/cli/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7771 2024-04-05 03:40:00.000000 backend.ai-client-24.3.0rc4/ai/backend/client/cli/dotfile.py
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-05 03:40:00.000000 backend.ai-client-24.3.0rc4/ai/backend/client/cli/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-04-05 03:40:00.000000 backend.ai-client-24.3.0rc4/ai/backend/client/cli/extensions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-04-05 03:40:00.000000 backend.ai-client-24.3.0rc4/ai/backend/client/cli/image.py
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-05 03:40:00.000000 backend.ai-client-24.3.0rc4/ai/backend/client/cli/logs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-04-05 03:40:00.000000 backend.ai-client-24.3.0rc4/ai/backend/client/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (127)    10159 2024-04-05 03:40:00.000000 backend.ai-client-24.3.0rc4/ai/backend/client/cli/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3662 2024-04-05 03:40:00.000000 backend.ai-client-24.3.0rc4/ai/backend/client/cli/pagination.py
--rw-r--r--   0 runner    (1001) docker     (127)     9165 2024-04-05 03:40:00.000000 backend.ai-client-24.3.0rc4/ai/backend/client/cli/pretty.py
--rw-r--r--   0 runner    (1001) docker     (127)     8228 2024-04-05 03:40:00.000000 backend.ai-client-24.3.0rc4/ai/backend/client/cli/proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-04-05 03:40:00.000000 backend.ai-client-24.3.0rc4/ai/backend/client/cli/server_log.py
--rw-r--r--   0 runner    (1001) docker     (127)    20889 2024-04-05 03:40:00.000000 backend.ai-client-24.3.0rc4/ai/backend/client/cli/service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:40:01.997385 backend.ai-client-24.3.0rc4/ai/backend/client/cli/session/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 03:40:00.000000 backend.ai-client-24.3.0rc4/ai/backend/client/cli/session/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4419 2024-04-05 03:40:00.000000 backend.ai-client-24.3.0rc4/ai/backend/client/cli/session/args.py
--rw-r--r--   0 runner    (1001) docker     (127)    30037 2024-04-05 03:40:00.000000 backend.ai-client-24.3.0rc4/ai/backend/client/cli/session/execute.py
--rw-r--r--   0 runner    (1001) docker     (127)    49861 2024-04-05 03:40:00.000000 backend.ai-client-24.3.0rc4/ai/backend/client/cli/session/lifecycle.py
--rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-04-05 03:40:00.000000 backend.ai-client-24.3.0rc4/ai/backend/client/cli/session/ssh.py
--rw-r--r--   0 runner    (1001) docker     (127)     6004 2024-04-05 03:40:00.000000 backend.ai-client-24.3.0rc4/ai/backend/client/cli/session_template.py
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-05 03:40:00.000000 backend.ai-client-24.3.0rc4/ai/backend/client/cli/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    35705 2024-04-05 03:40:00.000000 backend.ai-client-24.3.0rc4/ai/backend/client/cli/vfolder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-04-05 03:40:00.000000 backend.ai-client-24.3.0rc4/ai/backend/client/compat.py
--rw-r--r--   0 runner    (1001) docker     (127)    13291 2024-04-05 03:40:00.000000 backend.ai-client-24.3.0rc4/ai/backend/client/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-04-05 03:40:00.000000 backend.ai-client-24.3.0rc4/ai/backend/client/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:40:02.001385 backend.ai-client-24.3.0rc4/ai/backend/client/func/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 03:40:00.000000 backend.ai-client-24.3.0rc4/ai/backend/client/func/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-04-05 03:40:00.000000 backend.ai-client-24.3.0rc4/ai/backend/client/func/acl.py
--rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-04-05 03:40:00.000000 backend.ai-client-24.3.0rc4/ai/backend/client/func/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4837 2024-04-05 03:40:00.000000 backend.ai-client-24.3.0rc4/ai/backend/client/func/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     3277 2024-04-05 03:40:00.000000 backend.ai-client-24.3.0rc4/ai/backend/client/func/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     2841 2024-04-05 03:40:00.000000 backend.ai-client-24.3.0rc4/ai/backend/client/func/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-05 03:40:00.000000 backend.ai-client-24.3.0rc4/ai/backend/client/func/bgtask.py
--rw-r--r--   0 runner    (1001) docker     (127)     6869 2024-04-05 03:40:00.000000 backend.ai-client-24.3.0rc4/ai/backend/client/func/domain.py
--rw-r--r--   0 runner    (1001) docker     (127)     4567 2024-04-05 03:40:00.000000 backend.ai-client-24.3.0rc4/ai/backend/client/func/dotfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-04-05 03:40:00.000000 backend.ai-client-24.3.0rc4/ai/backend/client/func/etcd.py
--rw-r--r--   0 runner    (1001) docker     (127)     9684 2024-04-05 03:40:00.000000 backend.ai-client-24.3.0rc4/ai/backend/client/func/group.py
--rw-r--r--   0 runner    (1001) docker     (127)     4822 2024-04-05 03:40:00.000000 backend.ai-client-24.3.0rc4/ai/backend/client/func/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     8171 2024-04-05 03:40:00.000000 backend.ai-client-24.3.0rc4/ai/backend/client/func/keypair.py
--rw-r--r--   0 runner    (1001) docker     (127)     6846 2024-04-05 03:40:00.000000 backend.ai-client-24.3.0rc4/ai/backend/client/func/keypair_resource_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-04-05 03:40:00.000000 backend.ai-client-24.3.0rc4/ai/backend/client/func/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     3296 2024-04-05 03:40:00.000000 backend.ai-client-24.3.0rc4/ai/backend/client/func/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5018 2024-04-05 03:40:00.000000 backend.ai-client-24.3.0rc4/ai/backend/client/func/quota_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)     3550 2024-04-05 03:40:00.000000 backend.ai-client-24.3.0rc4/ai/backend/client/func/resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    12878 2024-04-05 03:40:00.000000 backend.ai-client-24.3.0rc4/ai/backend/client/func/scaling_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-05 03:40:00.000000 backend.ai-client-24.3.0rc4/ai/backend/client/func/server_log.py
--rw-r--r--   0 runner    (1001) docker     (127)    12337 2024-04-05 03:40:00.000000 backend.ai-client-24.3.0rc4/ai/backend/client/func/service.py
--rw-r--r--   0 runner    (1001) docker     (127)    52303 2024-04-05 03:40:00.000000 backend.ai-client-24.3.0rc4/ai/backend/client/func/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-04-05 03:40:00.000000 backend.ai-client-24.3.0rc4/ai/backend/client/func/session_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-04-05 03:40:00.000000 backend.ai-client-24.3.0rc4/ai/backend/client/func/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)      908 2024-04-05 03:40:00.000000 backend.ai-client-24.3.0rc4/ai/backend/client/func/system.py
--rw-r--r--   0 runner    (1001) docker     (127)    13752 2024-04-05 03:40:00.000000 backend.ai-client-24.3.0rc4/ai/backend/client/func/user.py
--rw-r--r--   0 runner    (1001) docker     (127)    27656 2024-04-05 03:40:00.000000 backend.ai-client-24.3.0rc4/ai/backend/client/func/vfolder.py
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-05 03:40:00.000000 backend.ai-client-24.3.0rc4/ai/backend/client/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-04-05 03:40:00.000000 backend.ai-client-24.3.0rc4/ai/backend/client/load_balancing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:40:02.001385 backend.ai-client-24.3.0rc4/ai/backend/client/output/
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-05 03:40:00.000000 backend.ai-client-24.3.0rc4/ai/backend/client/output/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7357 2024-04-05 03:40:00.000000 backend.ai-client-24.3.0rc4/ai/backend/client/output/console.py
--rw-r--r--   0 runner    (1001) docker     (127)    10216 2024-04-05 03:40:00.000000 backend.ai-client-24.3.0rc4/ai/backend/client/output/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)    12511 2024-04-05 03:40:00.000000 backend.ai-client-24.3.0rc4/ai/backend/client/output/formatters.py
--rw-r--r--   0 runner    (1001) docker     (127)     6749 2024-04-05 03:40:00.000000 backend.ai-client-24.3.0rc4/ai/backend/client/output/json.py
--rw-r--r--   0 runner    (1001) docker     (127)     6054 2024-04-05 03:40:00.000000 backend.ai-client-24.3.0rc4/ai/backend/client/output/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     2712 2024-04-05 03:40:00.000000 backend.ai-client-24.3.0rc4/ai/backend/client/pagination.py
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-05 03:40:00.000000 backend.ai-client-24.3.0rc4/ai/backend/client/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    29791 2024-04-05 03:40:00.000000 backend.ai-client-24.3.0rc4/ai/backend/client/request.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 03:40:00.000000 backend.ai-client-24.3.0rc4/ai/backend/client/service.py
--rw-r--r--   0 runner    (1001) docker     (127)    16998 2024-04-05 03:40:00.000000 backend.ai-client-24.3.0rc4/ai/backend/client/session.py
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-05 03:40:00.000000 backend.ai-client-24.3.0rc4/ai/backend/client/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-04-05 03:40:00.000000 backend.ai-client-24.3.0rc4/ai/backend/client/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-04-05 03:40:00.000000 backend.ai-client-24.3.0rc4/ai/backend/client/versioning.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:40:02.005385 backend.ai-client-24.3.0rc4/backend.ai_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9350 2024-04-05 03:40:01.000000 backend.ai-client-24.3.0rc4/backend.ai_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-04-05 03:40:01.000000 backend.ai-client-24.3.0rc4/backend.ai_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 03:40:01.000000 backend.ai-client-24.3.0rc4/backend.ai_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-05 03:40:01.000000 backend.ai-client-24.3.0rc4/backend.ai_client.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 03:40:01.000000 backend.ai-client-24.3.0rc4/backend.ai_client.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 03:40:01.000000 backend.ai-client-24.3.0rc4/backend.ai_client.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-05 03:40:01.000000 backend.ai-client-24.3.0rc4/backend.ai_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        3 2024-04-05 03:40:01.000000 backend.ai-client-24.3.0rc4/backend.ai_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-04-05 03:40:00.000000 backend.ai-client-24.3.0rc4/backend_shim.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 03:40:02.005385 backend.ai-client-24.3.0rc4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)    10105 2024-04-05 03:40:00.000000 backend.ai-client-24.3.0rc4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:08:33.863073 backend.ai-client-24.3.1rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-16 17:08:33.000000 backend.ai-client-24.3.1rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9349 2024-04-16 17:08:33.863073 backend.ai-client-24.3.1rc1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:08:33.839073 backend.ai-client-24.3.1rc1/ai/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:08:33.839073 backend.ai-client-24.3.1rc1/ai/backend/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:08:33.843073 backend.ai-client-24.3.1rc1/ai/backend/client/
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-16 17:08:33.000000 backend.ai-client-24.3.1rc1/ai/backend/client/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-16 17:08:33.000000 backend.ai-client-24.3.1rc1/ai/backend/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-04-16 17:08:33.000000 backend.ai-client-24.3.1rc1/ai/backend/client/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:08:33.847073 backend.ai-client-24.3.1rc1/ai/backend/client/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-16 17:08:33.000000 backend.ai-client-24.3.1rc1/ai/backend/client/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:08:33.851073 backend.ai-client-24.3.1rc1/ai/backend/client/cli/admin/
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-16 17:08:33.000000 backend.ai-client-24.3.1rc1/ai/backend/client/cli/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-16 17:08:33.000000 backend.ai-client-24.3.1rc1/ai/backend/client/cli/admin/acl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5143 2024-04-16 17:08:33.000000 backend.ai-client-24.3.1rc1/ai/backend/client/cli/admin/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8230 2024-04-16 17:08:33.000000 backend.ai-client-24.3.1rc1/ai/backend/client/cli/admin/domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-04-16 17:08:33.000000 backend.ai-client-24.3.1rc1/ai/backend/client/cli/admin/etcd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11198 2024-04-16 17:08:33.000000 backend.ai-client-24.3.1rc1/ai/backend/client/cli/admin/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4545 2024-04-16 17:08:33.000000 backend.ai-client-24.3.1rc1/ai/backend/client/cli/admin/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9909 2024-04-16 17:08:33.000000 backend.ai-client-24.3.1rc1/ai/backend/client/cli/admin/keypair.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-04-16 17:08:33.000000 backend.ai-client-24.3.1rc1/ai/backend/client/cli/admin/license.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6297 2024-04-16 17:08:33.000000 backend.ai-client-24.3.1rc1/ai/backend/client/cli/admin/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6930 2024-04-16 17:08:33.000000 backend.ai-client-24.3.1rc1/ai/backend/client/cli/admin/quota_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6383 2024-04-16 17:08:33.000000 backend.ai-client-24.3.1rc1/ai/backend/client/cli/admin/resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9478 2024-04-16 17:08:33.000000 backend.ai-client-24.3.1rc1/ai/backend/client/cli/admin/resource_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11704 2024-04-16 17:08:33.000000 backend.ai-client-24.3.1rc1/ai/backend/client/cli/admin/scaling_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9694 2024-04-16 17:08:33.000000 backend.ai-client-24.3.1rc1/ai/backend/client/cli/admin/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-04-16 17:08:33.000000 backend.ai-client-24.3.1rc1/ai/backend/client/cli/admin/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15514 2024-04-16 17:08:33.000000 backend.ai-client-24.3.1rc1/ai/backend/client/cli/admin/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12201 2024-04-16 17:08:33.000000 backend.ai-client-24.3.1rc1/ai/backend/client/cli/admin/vfolder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-04-16 17:08:33.000000 backend.ai-client-24.3.1rc1/ai/backend/client/cli/announcement.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12150 2024-04-16 17:08:33.000000 backend.ai-client-24.3.1rc1/ai/backend/client/cli/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7991 2024-04-16 17:08:33.000000 backend.ai-client-24.3.1rc1/ai/backend/client/cli/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7771 2024-04-16 17:08:33.000000 backend.ai-client-24.3.1rc1/ai/backend/client/cli/dotfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-16 17:08:33.000000 backend.ai-client-24.3.1rc1/ai/backend/client/cli/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-04-16 17:08:33.000000 backend.ai-client-24.3.1rc1/ai/backend/client/cli/extensions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3349 2024-04-16 17:08:33.000000 backend.ai-client-24.3.1rc1/ai/backend/client/cli/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-16 17:08:33.000000 backend.ai-client-24.3.1rc1/ai/backend/client/cli/logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-04-16 17:08:33.000000 backend.ai-client-24.3.1rc1/ai/backend/client/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10159 2024-04-16 17:08:33.000000 backend.ai-client-24.3.1rc1/ai/backend/client/cli/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3662 2024-04-16 17:08:33.000000 backend.ai-client-24.3.1rc1/ai/backend/client/cli/pagination.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9165 2024-04-16 17:08:33.000000 backend.ai-client-24.3.1rc1/ai/backend/client/cli/pretty.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8228 2024-04-16 17:08:33.000000 backend.ai-client-24.3.1rc1/ai/backend/client/cli/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-04-16 17:08:33.000000 backend.ai-client-24.3.1rc1/ai/backend/client/cli/server_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20889 2024-04-16 17:08:33.000000 backend.ai-client-24.3.1rc1/ai/backend/client/cli/service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:08:33.851073 backend.ai-client-24.3.1rc1/ai/backend/client/cli/session/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 17:08:33.000000 backend.ai-client-24.3.1rc1/ai/backend/client/cli/session/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4419 2024-04-16 17:08:33.000000 backend.ai-client-24.3.1rc1/ai/backend/client/cli/session/args.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30037 2024-04-16 17:08:33.000000 backend.ai-client-24.3.1rc1/ai/backend/client/cli/session/execute.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49861 2024-04-16 17:08:33.000000 backend.ai-client-24.3.1rc1/ai/backend/client/cli/session/lifecycle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-04-16 17:08:33.000000 backend.ai-client-24.3.1rc1/ai/backend/client/cli/session/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6004 2024-04-16 17:08:33.000000 backend.ai-client-24.3.1rc1/ai/backend/client/cli/session_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-16 17:08:33.000000 backend.ai-client-24.3.1rc1/ai/backend/client/cli/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35705 2024-04-16 17:08:33.000000 backend.ai-client-24.3.1rc1/ai/backend/client/cli/vfolder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-04-16 17:08:33.000000 backend.ai-client-24.3.1rc1/ai/backend/client/compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13291 2024-04-16 17:08:33.000000 backend.ai-client-24.3.1rc1/ai/backend/client/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-04-16 17:08:33.000000 backend.ai-client-24.3.1rc1/ai/backend/client/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:08:33.859073 backend.ai-client-24.3.1rc1/ai/backend/client/func/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 17:08:33.000000 backend.ai-client-24.3.1rc1/ai/backend/client/func/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-04-16 17:08:33.000000 backend.ai-client-24.3.1rc1/ai/backend/client/func/acl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-04-16 17:08:33.000000 backend.ai-client-24.3.1rc1/ai/backend/client/func/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4837 2024-04-16 17:08:33.000000 backend.ai-client-24.3.1rc1/ai/backend/client/func/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3277 2024-04-16 17:08:33.000000 backend.ai-client-24.3.1rc1/ai/backend/client/func/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2841 2024-04-16 17:08:33.000000 backend.ai-client-24.3.1rc1/ai/backend/client/func/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-16 17:08:33.000000 backend.ai-client-24.3.1rc1/ai/backend/client/func/bgtask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6869 2024-04-16 17:08:33.000000 backend.ai-client-24.3.1rc1/ai/backend/client/func/domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4567 2024-04-16 17:08:33.000000 backend.ai-client-24.3.1rc1/ai/backend/client/func/dotfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-04-16 17:08:33.000000 backend.ai-client-24.3.1rc1/ai/backend/client/func/etcd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9684 2024-04-16 17:08:33.000000 backend.ai-client-24.3.1rc1/ai/backend/client/func/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6646 2024-04-16 17:08:33.000000 backend.ai-client-24.3.1rc1/ai/backend/client/func/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8171 2024-04-16 17:08:33.000000 backend.ai-client-24.3.1rc1/ai/backend/client/func/keypair.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6846 2024-04-16 17:08:33.000000 backend.ai-client-24.3.1rc1/ai/backend/client/func/keypair_resource_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-04-16 17:08:33.000000 backend.ai-client-24.3.1rc1/ai/backend/client/func/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3296 2024-04-16 17:08:33.000000 backend.ai-client-24.3.1rc1/ai/backend/client/func/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5018 2024-04-16 17:08:33.000000 backend.ai-client-24.3.1rc1/ai/backend/client/func/quota_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3550 2024-04-16 17:08:33.000000 backend.ai-client-24.3.1rc1/ai/backend/client/func/resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12878 2024-04-16 17:08:33.000000 backend.ai-client-24.3.1rc1/ai/backend/client/func/scaling_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-16 17:08:33.000000 backend.ai-client-24.3.1rc1/ai/backend/client/func/server_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12337 2024-04-16 17:08:33.000000 backend.ai-client-24.3.1rc1/ai/backend/client/func/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52303 2024-04-16 17:08:33.000000 backend.ai-client-24.3.1rc1/ai/backend/client/func/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-04-16 17:08:33.000000 backend.ai-client-24.3.1rc1/ai/backend/client/func/session_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-04-16 17:08:33.000000 backend.ai-client-24.3.1rc1/ai/backend/client/func/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-04-16 17:08:33.000000 backend.ai-client-24.3.1rc1/ai/backend/client/func/system.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13752 2024-04-16 17:08:33.000000 backend.ai-client-24.3.1rc1/ai/backend/client/func/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27656 2024-04-16 17:08:33.000000 backend.ai-client-24.3.1rc1/ai/backend/client/func/vfolder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-16 17:08:33.000000 backend.ai-client-24.3.1rc1/ai/backend/client/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-04-16 17:08:33.000000 backend.ai-client-24.3.1rc1/ai/backend/client/load_balancing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:08:33.859073 backend.ai-client-24.3.1rc1/ai/backend/client/output/
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-16 17:08:33.000000 backend.ai-client-24.3.1rc1/ai/backend/client/output/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7357 2024-04-16 17:08:33.000000 backend.ai-client-24.3.1rc1/ai/backend/client/output/console.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10203 2024-04-16 17:08:33.000000 backend.ai-client-24.3.1rc1/ai/backend/client/output/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12740 2024-04-16 17:08:33.000000 backend.ai-client-24.3.1rc1/ai/backend/client/output/formatters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6749 2024-04-16 17:08:33.000000 backend.ai-client-24.3.1rc1/ai/backend/client/output/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6054 2024-04-16 17:08:33.000000 backend.ai-client-24.3.1rc1/ai/backend/client/output/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2712 2024-04-16 17:08:33.000000 backend.ai-client-24.3.1rc1/ai/backend/client/pagination.py
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-16 17:08:33.000000 backend.ai-client-24.3.1rc1/ai/backend/client/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    29791 2024-04-16 17:08:33.000000 backend.ai-client-24.3.1rc1/ai/backend/client/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 17:08:33.000000 backend.ai-client-24.3.1rc1/ai/backend/client/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16998 2024-04-16 17:08:33.000000 backend.ai-client-24.3.1rc1/ai/backend/client/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-16 17:08:33.000000 backend.ai-client-24.3.1rc1/ai/backend/client/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-04-16 17:08:33.000000 backend.ai-client-24.3.1rc1/ai/backend/client/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-04-16 17:08:33.000000 backend.ai-client-24.3.1rc1/ai/backend/client/versioning.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:08:33.859073 backend.ai-client-24.3.1rc1/backend.ai_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9349 2024-04-16 17:08:33.000000 backend.ai-client-24.3.1rc1/backend.ai_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-04-16 17:08:33.000000 backend.ai-client-24.3.1rc1/backend.ai_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 17:08:33.000000 backend.ai-client-24.3.1rc1/backend.ai_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-16 17:08:33.000000 backend.ai-client-24.3.1rc1/backend.ai_client.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 17:08:33.000000 backend.ai-client-24.3.1rc1/backend.ai_client.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 17:08:33.000000 backend.ai-client-24.3.1rc1/backend.ai_client.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-16 17:08:33.000000 backend.ai-client-24.3.1rc1/backend.ai_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2024-04-16 17:08:33.000000 backend.ai-client-24.3.1rc1/backend.ai_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-04-16 17:08:33.000000 backend.ai-client-24.3.1rc1/backend_shim.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 17:08:33.863073 backend.ai-client-24.3.1rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)    10104 2024-04-16 17:08:33.000000 backend.ai-client-24.3.1rc1/setup.py
```

### Comparing `backend.ai-client-24.3.0rc4/PKG-INFO` & `backend.ai-client-24.3.1rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backend.ai-client
-Version: 24.3.0rc4
+Version: 24.3.1rc1
 Summary: Backend.AI Client SDK
 Home-page: https://github.com/lablup/backend.ai
 Author: Lablup Inc. and contributors
 License: MIT
 Project-URL: Documentation, https://docs.backend.ai/
 Project-URL: Source, https://github.com/lablup/backend.ai
 Classifier: Intended Audience :: Developers
@@ -21,30 +21,30 @@
 Requires-Python: >=3.12,<3.13
 Description-Content-Type: text/x-rst
 Requires-Dist: aiohttp~=3.9.1
 Requires-Dist: aiotusclient~=0.1.4
 Requires-Dist: appdirs~=1.4.4
 Requires-Dist: async_timeout~=4.0
 Requires-Dist: attrs>=20.3
-Requires-Dist: backend.ai-cli==24.03.0rc4
-Requires-Dist: backend.ai-common==24.03.0rc4
-Requires-Dist: backend.ai-plugin==24.03.0rc4
+Requires-Dist: backend.ai-cli==24.03.1rc1
+Requires-Dist: backend.ai-common==24.03.1rc1
+Requires-Dist: backend.ai-plugin==24.03.1rc1
 Requires-Dist: click~=8.1.7
-Requires-Dist: faker~=13.12.0
+Requires-Dist: faker~=24.7.1
 Requires-Dist: humanize>=3.1.0
 Requires-Dist: inquirer~=2.9.2
 Requires-Dist: janus~=1.0.0
 Requires-Dist: multidict>=6.0
 Requires-Dist: python-dateutil>=2.8
 Requires-Dist: python-dotenv~=0.20.0
 Requires-Dist: rich~=13.6
 Requires-Dist: tabulate~=0.8.9
 Requires-Dist: tenacity>=8.0
 Requires-Dist: tqdm>=4.61
-Requires-Dist: treelib==1.6.1
+Requires-Dist: treelib~=1.7.0
 Requires-Dist: types-python-dateutil
 Requires-Dist: types-tabulate
 Requires-Dist: yarl!=1.9.0,!=1.9.1,!=1.9.2,<2.0,>=1.8.2
 
 Backend.AI Client
 =================
```

### Comparing `backend.ai-client-24.3.0rc4/ai/backend/client/auth.py` & `backend.ai-client-24.3.1rc1/ai/backend/client/auth.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc4/ai/backend/client/cli/__init__.py` & `backend.ai-client-24.3.1rc1/ai/backend/client/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc4/ai/backend/client/cli/admin/acl.py` & `backend.ai-client-24.3.1rc1/ai/backend/client/cli/admin/acl.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc4/ai/backend/client/cli/admin/agent.py` & `backend.ai-client-24.3.1rc1/ai/backend/client/cli/admin/agent.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc4/ai/backend/client/cli/admin/domain.py` & `backend.ai-client-24.3.1rc1/ai/backend/client/cli/admin/domain.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc4/ai/backend/client/cli/admin/etcd.py` & `backend.ai-client-24.3.1rc1/ai/backend/client/cli/admin/etcd.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc4/ai/backend/client/cli/admin/group.py` & `backend.ai-client-24.3.1rc1/ai/backend/client/cli/admin/group.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc4/ai/backend/client/cli/admin/image.py` & `backend.ai-client-24.3.1rc1/ai/backend/client/cli/admin/image.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc4/ai/backend/client/cli/admin/keypair.py` & `backend.ai-client-24.3.1rc1/ai/backend/client/cli/admin/keypair.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc4/ai/backend/client/cli/admin/license.py` & `backend.ai-client-24.3.1rc1/ai/backend/client/cli/admin/license.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc4/ai/backend/client/cli/admin/manager.py` & `backend.ai-client-24.3.1rc1/ai/backend/client/cli/admin/manager.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc4/ai/backend/client/cli/admin/quota_scope.py` & `backend.ai-client-24.3.1rc1/ai/backend/client/cli/admin/quota_scope.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc4/ai/backend/client/cli/admin/resource.py` & `backend.ai-client-24.3.1rc1/ai/backend/client/cli/admin/resource.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc4/ai/backend/client/cli/admin/resource_policy.py` & `backend.ai-client-24.3.1rc1/ai/backend/client/cli/admin/resource_policy.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc4/ai/backend/client/cli/admin/scaling_group.py` & `backend.ai-client-24.3.1rc1/ai/backend/client/cli/admin/scaling_group.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc4/ai/backend/client/cli/admin/session.py` & `backend.ai-client-24.3.1rc1/ai/backend/client/cli/admin/session.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc4/ai/backend/client/cli/admin/storage.py` & `backend.ai-client-24.3.1rc1/ai/backend/client/cli/admin/storage.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc4/ai/backend/client/cli/admin/user.py` & `backend.ai-client-24.3.1rc1/ai/backend/client/cli/admin/user.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc4/ai/backend/client/cli/admin/vfolder.py` & `backend.ai-client-24.3.1rc1/ai/backend/client/cli/admin/vfolder.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc4/ai/backend/client/cli/announcement.py` & `backend.ai-client-24.3.1rc1/ai/backend/client/cli/announcement.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc4/ai/backend/client/cli/app.py` & `backend.ai-client-24.3.1rc1/ai/backend/client/cli/app.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc4/ai/backend/client/cli/config.py` & `backend.ai-client-24.3.1rc1/ai/backend/client/cli/config.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc4/ai/backend/client/cli/dotfile.py` & `backend.ai-client-24.3.1rc1/ai/backend/client/cli/dotfile.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc4/ai/backend/client/cli/extensions.py` & `backend.ai-client-24.3.1rc1/ai/backend/client/cli/extensions.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc4/ai/backend/client/cli/image.py` & `backend.ai-client-24.3.1rc1/ai/backend/client/cli/image.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,48 +1,63 @@
 import sys
 
 import click
 
 # from ai.backend.client.output.fields import image_fields
 from ai.backend.cli.main import main
 from ai.backend.cli.types import ExitCode
+from ai.backend.client.exceptions import BackendAPIError
 from ai.backend.client.func.image import _default_list_fields_admin
 from ai.backend.client.output.fields import image_fields
 from ai.backend.client.session import Session
 
 from .extensions import pass_ctx_obj
-from .pretty import print_done, print_error, print_fail
+from .pretty import print_done, print_error, print_fail, print_warn
 from .types import CLIContext
 
 
 @main.group()
 def image() -> None:
     """
     Image commands.
     """
 
 
+def get_image_id(
+    session: Session,
+    name_or_id: str,
+    architecture: str | None = None,
+) -> str:
+    try:
+        session.Image.get_by_id(name_or_id, fields=[image_fields["id"]])
+        return name_or_id
+    except Exception:
+        image = session.Image.get(name_or_id, architecture, fields=[image_fields["id"]])
+        return image["id"]
+
+
 @image.command()
 @pass_ctx_obj
 @click.option("--customized", is_flag=True, help="Get images customized by user only")
 def list(ctx: CLIContext, customized: bool) -> None:
     """
     Show the list of registered images in this cluster.
     """
     with Session() as session:
         try:
+            fields: tuple
             if customized:
                 fields = (
-                    image_fields["customized_image_name"],
                     image_fields["id"],
                     image_fields["name"],
                     image_fields["registry"],
                     image_fields["architecture"],
                     image_fields["tag"],
                     image_fields["size_bytes"],
+                    image_fields["customized_image"],
                 )
                 items = session.Image.list_customized(fields=fields)
             else:
                 fields = _default_list_fields_admin
                 items = session.Image.list(fields=fields)
             ctx.output.print_list(items, fields)
         except Exception as e:
@@ -56,23 +71,25 @@
 def forget(reference_or_id, arch):
     """Forget image from server. This command will only work for image customized by user
     unless callee has superadmin privileges.
 
     REFERENCE_OR_ID: Canonical string of image (<registry>/<project>/<name>:<tag>)"""
     with Session() as session:
         try:
-            try:
-                result = session.Image.forget_image_by_id(reference_or_id)
-            except Exception:
-                if not arch:
-                    print_fail(
-                        "`arch` option should be set when removing image via its reference string"
-                    )
-                    sys.exit(ExitCode.FAILURE)
-                result = session.Image.forget_image(reference_or_id, arch)
+            image_id = get_image_id(session, reference_or_id, architecture=arch)
+        except BackendAPIError:
+            print_fail("Could not find image.")
+            if not arch:
+                print_warn(
+                    "`arch` parameter not passed. If you are trying to resolve image via its canonical string you have to specify which architecture are you trying to manipulate with."
+                )
+            sys.exit(ExitCode.FAILURE)
+        try:
+            result = session.Image.untag_image_from_registry(image_id)
+            result = session.Image.forget_image_by_id(image_id)
         except Exception as e:
             print_error(e)
             sys.exit(ExitCode.FAILURE)
         if result["ok"]:
             print_done(f"Image forgotten: {reference_or_id}")
         else:
             print_fail("Image forget has failed: {0}".format(result["msg"]))
```

### Comparing `backend.ai-client-24.3.0rc4/ai/backend/client/cli/logs.py` & `backend.ai-client-24.3.1rc1/ai/backend/client/cli/logs.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc4/ai/backend/client/cli/main.py` & `backend.ai-client-24.3.1rc1/ai/backend/client/cli/main.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc4/ai/backend/client/cli/model.py` & `backend.ai-client-24.3.1rc1/ai/backend/client/cli/model.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc4/ai/backend/client/cli/pagination.py` & `backend.ai-client-24.3.1rc1/ai/backend/client/cli/pagination.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc4/ai/backend/client/cli/pretty.py` & `backend.ai-client-24.3.1rc1/ai/backend/client/cli/pretty.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc4/ai/backend/client/cli/proxy.py` & `backend.ai-client-24.3.1rc1/ai/backend/client/cli/proxy.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc4/ai/backend/client/cli/server_log.py` & `backend.ai-client-24.3.1rc1/ai/backend/client/cli/server_log.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc4/ai/backend/client/cli/service.py` & `backend.ai-client-24.3.1rc1/ai/backend/client/cli/service.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc4/ai/backend/client/cli/session/args.py` & `backend.ai-client-24.3.1rc1/ai/backend/client/cli/session/args.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc4/ai/backend/client/cli/session/execute.py` & `backend.ai-client-24.3.1rc1/ai/backend/client/cli/session/execute.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc4/ai/backend/client/cli/session/lifecycle.py` & `backend.ai-client-24.3.1rc1/ai/backend/client/cli/session/lifecycle.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc4/ai/backend/client/cli/session/ssh.py` & `backend.ai-client-24.3.1rc1/ai/backend/client/cli/session/ssh.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc4/ai/backend/client/cli/session_template.py` & `backend.ai-client-24.3.1rc1/ai/backend/client/cli/session_template.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc4/ai/backend/client/cli/vfolder.py` & `backend.ai-client-24.3.1rc1/ai/backend/client/cli/vfolder.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc4/ai/backend/client/compat.py` & `backend.ai-client-24.3.1rc1/ai/backend/client/compat.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc4/ai/backend/client/config.py` & `backend.ai-client-24.3.1rc1/ai/backend/client/config.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc4/ai/backend/client/exceptions.py` & `backend.ai-client-24.3.1rc1/ai/backend/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc4/ai/backend/client/func/acl.py` & `backend.ai-client-24.3.1rc1/ai/backend/client/func/acl.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc4/ai/backend/client/func/admin.py` & `backend.ai-client-24.3.1rc1/ai/backend/client/func/admin.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc4/ai/backend/client/func/agent.py` & `backend.ai-client-24.3.1rc1/ai/backend/client/func/agent.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc4/ai/backend/client/func/auth.py` & `backend.ai-client-24.3.1rc1/ai/backend/client/func/auth.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc4/ai/backend/client/func/base.py` & `backend.ai-client-24.3.1rc1/ai/backend/client/func/base.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc4/ai/backend/client/func/bgtask.py` & `backend.ai-client-24.3.1rc1/ai/backend/client/func/bgtask.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc4/ai/backend/client/func/domain.py` & `backend.ai-client-24.3.1rc1/ai/backend/client/func/domain.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc4/ai/backend/client/func/dotfile.py` & `backend.ai-client-24.3.1rc1/ai/backend/client/func/dotfile.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc4/ai/backend/client/func/etcd.py` & `backend.ai-client-24.3.1rc1/ai/backend/client/func/etcd.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc4/ai/backend/client/func/group.py` & `backend.ai-client-24.3.1rc1/ai/backend/client/func/group.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc4/ai/backend/client/func/image.py` & `backend.ai-client-24.3.1rc1/ai/backend/client/func/image.py`

 * *Files 18% similar despite different names*

```diff
@@ -49,14 +49,58 @@
             "is_operation": operation,
         }
         data = await api_session.get().Admin._query(q, variables)
         return data["images"]
 
     @api_function
     @classmethod
+    async def get(
+        cls,
+        reference: str,
+        architecture: str,
+        fields: Sequence[FieldSpec] = _default_list_fields_admin,
+    ) -> Sequence[dict]:
+        """
+        Fetches the information about registered image in this cluster.
+        """
+        q = (
+            "query($reference: String!, $architecture: String!) {"
+            "  image(reference: $reference, architecture: $architecture) {"
+            "    $fields"
+            "  }"
+            "}"
+        )
+        q = q.replace("$fields", " ".join(f.field_ref for f in fields))
+        variables = {
+            "reference": reference,
+            "architecture": architecture,
+        }
+        data = await api_session.get().Admin._query(q, variables)
+        return data["image"]
+
+    @api_function
+    @classmethod
+    async def get_by_id(
+        cls,
+        id: str,
+        fields: Sequence[FieldSpec] = _default_list_fields_admin,
+    ) -> Sequence[dict]:
+        """
+        Fetches the information about registered image in this cluster.
+        """
+        q = "query($id: String!) {" "  image(id: $id) {" "    $fields" "  }" "}"
+        q = q.replace("$fields", " ".join(f.field_ref for f in fields))
+        variables = {
+            "id": id,
+        }
+        data = await api_session.get().Admin._query(q, variables)
+        return data["image"]
+
+    @api_function
+    @classmethod
     async def list_customized(
         cls,
         fields: Sequence[FieldSpec] = _default_list_fields_admin,
     ) -> Sequence[dict]:
         """
         Fetches the list of customized images in this cluster.
         """
@@ -95,14 +139,30 @@
             "image_id": image_id,
         }
         data = await api_session.get().Admin._query(q, variables)
         return data["forget_image_by_id"]
 
     @api_function
     @classmethod
+    async def untag_image_from_registry(cls, id: str):
+        q = (
+            "mutation($id: String!) {"
+            "  untag_image_from_registry(id: $id) {"
+            "   ok msg"
+            "  }"
+            "}"
+        )
+        variables = {
+            "id": id,
+        }
+        data = await api_session.get().Admin._query(q, variables)
+        return data["untag_image_from_registry"]
+
+    @api_function
+    @classmethod
     async def forget_image(cls, reference: str, architecture: str):
         q = (
             "mutation($reference: String!, $architecture: String!) {"
             "  forget_image(reference: $reference, architecture: $architecture) {"
             "   ok msg"
             "  }"
             "}"
```

### Comparing `backend.ai-client-24.3.0rc4/ai/backend/client/func/keypair.py` & `backend.ai-client-24.3.1rc1/ai/backend/client/func/keypair.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc4/ai/backend/client/func/keypair_resource_policy.py` & `backend.ai-client-24.3.1rc1/ai/backend/client/func/keypair_resource_policy.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc4/ai/backend/client/func/manager.py` & `backend.ai-client-24.3.1rc1/ai/backend/client/func/manager.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc4/ai/backend/client/func/model.py` & `backend.ai-client-24.3.1rc1/ai/backend/client/func/model.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc4/ai/backend/client/func/quota_scope.py` & `backend.ai-client-24.3.1rc1/ai/backend/client/func/quota_scope.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc4/ai/backend/client/func/resource.py` & `backend.ai-client-24.3.1rc1/ai/backend/client/func/resource.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc4/ai/backend/client/func/scaling_group.py` & `backend.ai-client-24.3.1rc1/ai/backend/client/func/scaling_group.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc4/ai/backend/client/func/server_log.py` & `backend.ai-client-24.3.1rc1/ai/backend/client/func/server_log.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc4/ai/backend/client/func/service.py` & `backend.ai-client-24.3.1rc1/ai/backend/client/func/service.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc4/ai/backend/client/func/session.py` & `backend.ai-client-24.3.1rc1/ai/backend/client/func/session.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc4/ai/backend/client/func/session_template.py` & `backend.ai-client-24.3.1rc1/ai/backend/client/func/session_template.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc4/ai/backend/client/func/storage.py` & `backend.ai-client-24.3.1rc1/ai/backend/client/func/storage.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc4/ai/backend/client/func/system.py` & `backend.ai-client-24.3.1rc1/ai/backend/client/func/system.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc4/ai/backend/client/func/user.py` & `backend.ai-client-24.3.1rc1/ai/backend/client/func/user.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc4/ai/backend/client/func/vfolder.py` & `backend.ai-client-24.3.1rc1/ai/backend/client/func/vfolder.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc4/ai/backend/client/load_balancing.py` & `backend.ai-client-24.3.1rc1/ai/backend/client/load_balancing.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc4/ai/backend/client/output/__init__.py` & `backend.ai-client-24.3.1rc1/ai/backend/client/output/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc4/ai/backend/client/output/console.py` & `backend.ai-client-24.3.1rc1/ai/backend/client/output/console.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc4/ai/backend/client/output/fields.py` & `backend.ai-client-24.3.1rc1/ai/backend/client/output/fields.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 from .formatters import (
     AgentStatFormatter,
     ContainerListFormatter,
-    CustomizedImageNameOutputFormatter,
+    CustomizedImageOutputFormatter,
     DependencyListFormatter,
     GroupListFormatter,
     InlineRoutingFormatter,
     KernelStatFormatter,
     SubFieldOutputFormatter,
     mibytes_output_formatter,
     nested_dict_formatter,
@@ -95,17 +95,17 @@
     FieldSpec("tag"),
     FieldSpec("digest"),
     FieldSpec("size_bytes", formatter=sizebytes_output_formatter),
     FieldSpec("aliases"),
     FieldSpec("labels { key value }", "labels"),
     FieldSpec(
         "labels { key value }",
-        "Customized Image Name",
-        alt_name="customized_image_name",
-        formatter=CustomizedImageNameOutputFormatter(),
+        "Customized Image Info",
+        alt_name="customized_image",
+        formatter=CustomizedImageOutputFormatter(),
     ),
 ])
 
 
 keypair_fields = FieldSet([
     FieldSpec("user_id", "Email"),
     FieldSpec(
```

### Comparing `backend.ai-client-24.3.0rc4/ai/backend/client/output/formatters.py` & `backend.ai-client-24.3.1rc1/ai/backend/client/output/formatters.py`

 * *Files 2% similar despite different names*

```diff
@@ -146,21 +146,27 @@
     def format_console(self, value: Any, field: FieldSpec) -> str:
         return super().format_console(value[self._subfield_name], field)
 
     def format_json(self, value: Any, field: FieldSpec) -> Any:
         return super().format_json(value[self._subfield_name], field)
 
 
-class CustomizedImageNameOutputFormatter(OutputFormatter):
+class CustomizedImageOutputFormatter(OutputFormatter):
     def _get_name(self, labels: Any) -> str:
         customized_name = [
             label["value"] for label in labels if label["key"] == "ai.backend.customized-image.name"
         ]
         assert len(customized_name) == 1
-        return customized_name[0]
+        owner_email = [
+            label["value"]
+            for label in labels
+            if label["key"] == "ai.backend.customized-image.user.email"
+        ]
+        assert len(owner_email) == 1
+        return f"{customized_name[0]} (Owner: {owner_email[0]})"
 
     def format_console(self, value: Any, field: FieldSpec) -> str:
         return super().format_console(self._get_name(value), field)
 
     def format_json(self, value: Any, field: FieldSpec) -> Any:
         return super().format_json(self._get_name(value), field)
```

### Comparing `backend.ai-client-24.3.0rc4/ai/backend/client/output/json.py` & `backend.ai-client-24.3.1rc1/ai/backend/client/output/json.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc4/ai/backend/client/output/types.py` & `backend.ai-client-24.3.1rc1/ai/backend/client/output/types.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc4/ai/backend/client/pagination.py` & `backend.ai-client-24.3.1rc1/ai/backend/client/pagination.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc4/ai/backend/client/request.py` & `backend.ai-client-24.3.1rc1/ai/backend/client/request.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc4/ai/backend/client/session.py` & `backend.ai-client-24.3.1rc1/ai/backend/client/session.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc4/ai/backend/client/types.py` & `backend.ai-client-24.3.1rc1/ai/backend/client/types.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc4/ai/backend/client/utils.py` & `backend.ai-client-24.3.1rc1/ai/backend/client/utils.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc4/ai/backend/client/versioning.py` & `backend.ai-client-24.3.1rc1/ai/backend/client/versioning.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc4/backend.ai_client.egg-info/PKG-INFO` & `backend.ai-client-24.3.1rc1/backend.ai_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backend.ai-client
-Version: 24.3.0rc4
+Version: 24.3.1rc1
 Summary: Backend.AI Client SDK
 Home-page: https://github.com/lablup/backend.ai
 Author: Lablup Inc. and contributors
 License: MIT
 Project-URL: Documentation, https://docs.backend.ai/
 Project-URL: Source, https://github.com/lablup/backend.ai
 Classifier: Intended Audience :: Developers
@@ -21,30 +21,30 @@
 Requires-Python: >=3.12,<3.13
 Description-Content-Type: text/x-rst
 Requires-Dist: aiohttp~=3.9.1
 Requires-Dist: aiotusclient~=0.1.4
 Requires-Dist: appdirs~=1.4.4
 Requires-Dist: async_timeout~=4.0
 Requires-Dist: attrs>=20.3
-Requires-Dist: backend.ai-cli==24.03.0rc4
-Requires-Dist: backend.ai-common==24.03.0rc4
-Requires-Dist: backend.ai-plugin==24.03.0rc4
+Requires-Dist: backend.ai-cli==24.03.1rc1
+Requires-Dist: backend.ai-common==24.03.1rc1
+Requires-Dist: backend.ai-plugin==24.03.1rc1
 Requires-Dist: click~=8.1.7
-Requires-Dist: faker~=13.12.0
+Requires-Dist: faker~=24.7.1
 Requires-Dist: humanize>=3.1.0
 Requires-Dist: inquirer~=2.9.2
 Requires-Dist: janus~=1.0.0
 Requires-Dist: multidict>=6.0
 Requires-Dist: python-dateutil>=2.8
 Requires-Dist: python-dotenv~=0.20.0
 Requires-Dist: rich~=13.6
 Requires-Dist: tabulate~=0.8.9
 Requires-Dist: tenacity>=8.0
 Requires-Dist: tqdm>=4.61
-Requires-Dist: treelib==1.6.1
+Requires-Dist: treelib~=1.7.0
 Requires-Dist: types-python-dateutil
 Requires-Dist: types-tabulate
 Requires-Dist: yarl!=1.9.0,!=1.9.1,!=1.9.2,<2.0,>=1.8.2
 
 Backend.AI Client
 =================
```

### Comparing `backend.ai-client-24.3.0rc4/backend.ai_client.egg-info/SOURCES.txt` & `backend.ai-client-24.3.1rc1/backend.ai_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc4/backend_shim.py` & `backend.ai-client-24.3.1rc1/backend_shim.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-24.3.0rc4/setup.py` & `backend.ai-client-24.3.1rc1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,33 +27,33 @@
     },
     'install_requires': (
         'aiohttp~=3.9.1',
         'aiotusclient~=0.1.4',
         'appdirs~=1.4.4',
         'async_timeout~=4.0',
         'attrs>=20.3',
-        """backend.ai-cli==24.03.0rc4
+        """backend.ai-cli==24.03.1rc1
 """,
-        """backend.ai-common==24.03.0rc4
+        """backend.ai-common==24.03.1rc1
 """,
-        """backend.ai-plugin==24.03.0rc4
+        """backend.ai-plugin==24.03.1rc1
 """,
         'click~=8.1.7',
-        'faker~=13.12.0',
+        'faker~=24.7.1',
         'humanize>=3.1.0',
         'inquirer~=2.9.2',
         'janus~=1.0.0',
         'multidict>=6.0',
         'python-dateutil>=2.8',
         'python-dotenv~=0.20.0',
         'rich~=13.6',
         'tabulate~=0.8.9',
         'tenacity>=8.0',
         'tqdm>=4.61',
-        'treelib==1.6.1',
+        'treelib~=1.7.0',
         'types-python-dateutil',
         'types-tabulate',
         'yarl!=1.9.0,!=1.9.1,!=1.9.2,<2.0,>=1.8.2',
     ),
     'license': 'MIT',
     'long_description': """Backend.AI Client
 =================
@@ -283,11 +283,11 @@
     ),
     'project_urls': {
         'Documentation': 'https://docs.backend.ai/',
         'Source': 'https://github.com/lablup/backend.ai',
     },
     'python_requires': '>=3.12,<3.13',
     'url': 'https://github.com/lablup/backend.ai',
-    'version': """24.03.0rc4
+    'version': """24.03.1rc1
 """,
     'zip_safe': False,
 })
```

