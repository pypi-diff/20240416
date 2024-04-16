# Comparing `tmp/backend.ai-common-24.3.0rc4.tar.gz` & `tmp/backend.ai-common-24.3.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backend.ai-common-24.3.0rc4.tar", last modified: Fri Apr  5 03:40:02 2024, max compression
+gzip compressed data, was "backend.ai-common-24.3.1rc1.tar", last modified: Tue Apr 16 17:08:33 2024, max compression
```

## Comparing `backend.ai-common-24.3.0rc4.tar` & `backend.ai-common-24.3.1rc1.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:40:02.417383 backend.ai-common-24.3.0rc4/
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-05 03:40:02.000000 backend.ai-common-24.3.0rc4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3633 2024-04-05 03:40:02.417383 backend.ai-common-24.3.0rc4/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:40:02.405383 backend.ai-common-24.3.0rc4/ai/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:40:02.405383 backend.ai-common-24.3.0rc4/ai/backend/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:40:02.413383 backend.ai-common-24.3.0rc4/ai/backend/common/
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-05 03:40:02.000000 backend.ai-common-24.3.0rc4/ai/backend/common/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-05 03:40:02.000000 backend.ai-common-24.3.0rc4/ai/backend/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-05 03:40:02.000000 backend.ai-common-24.3.0rc4/ai/backend/common/arch.py
--rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-04-05 03:40:02.000000 backend.ai-common-24.3.0rc4/ai/backend/common/argparse.py
--rw-r--r--   0 runner    (1001) docker     (127)     3055 2024-04-05 03:40:02.000000 backend.ai-common-24.3.0rc4/ai/backend/common/asyncio.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:40:02.413383 backend.ai-common-24.3.0rc4/ai/backend/common/auth/
--rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-04-05 03:40:02.000000 backend.ai-common-24.3.0rc4/ai/backend/common/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11477 2024-04-05 03:40:02.000000 backend.ai-common-24.3.0rc4/ai/backend/common/bgtask.py
--rw-r--r--   0 runner    (1001) docker     (127)     3781 2024-04-05 03:40:02.000000 backend.ai-common-24.3.0rc4/ai/backend/common/cgroup.py
--rw-r--r--   0 runner    (1001) docker     (127)     3021 2024-04-05 03:40:02.000000 backend.ai-common-24.3.0rc4/ai/backend/common/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     8540 2024-04-05 03:40:02.000000 backend.ai-common-24.3.0rc4/ai/backend/common/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-05 03:40:02.000000 backend.ai-common-24.3.0rc4/ai/backend/common/defs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2576 2024-04-05 03:40:02.000000 backend.ai-common-24.3.0rc4/ai/backend/common/distributed.py
--rw-r--r--   0 runner    (1001) docker     (127)    21291 2024-04-05 03:40:02.000000 backend.ai-common-24.3.0rc4/ai/backend/common/docker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-05 03:40:02.000000 backend.ai-common-24.3.0rc4/ai/backend/common/enum_extension.py
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-04-05 03:40:02.000000 backend.ai-common-24.3.0rc4/ai/backend/common/enum_extension.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    19833 2024-04-05 03:40:02.000000 backend.ai-common-24.3.0rc4/ai/backend/common/etcd.py
--rw-r--r--   0 runner    (1001) docker     (127)    33020 2024-04-05 03:40:02.000000 backend.ai-common-24.3.0rc4/ai/backend/common/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     2585 2024-04-05 03:40:02.000000 backend.ai-common-24.3.0rc4/ai/backend/common/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-04-05 03:40:02.000000 backend.ai-common-24.3.0rc4/ai/backend/common/files.py
--rw-r--r--   0 runner    (1001) docker     (127)     9964 2024-04-05 03:40:02.000000 backend.ai-common-24.3.0rc4/ai/backend/common/identity.py
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-05 03:40:02.000000 backend.ai-common-24.3.0rc4/ai/backend/common/json.py
--rw-r--r--   0 runner    (1001) docker     (127)     7968 2024-04-05 03:40:02.000000 backend.ai-common-24.3.0rc4/ai/backend/common/lock.py
--rw-r--r--   0 runner    (1001) docker     (127)    23875 2024-04-05 03:40:02.000000 backend.ai-common-24.3.0rc4/ai/backend/common/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-04-05 03:40:02.000000 backend.ai-common-24.3.0rc4/ai/backend/common/logging_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:40:02.405383 backend.ai-common-24.3.0rc4/ai/backend/common/models/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:40:02.417383 backend.ai-common-24.3.0rc4/ai/backend/common/models/minilang/
--rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-04-05 03:40:02.000000 backend.ai-common-24.3.0rc4/ai/backend/common/models/minilang/mount.py
--rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-04-05 03:40:02.000000 backend.ai-common-24.3.0rc4/ai/backend/common/msgpack.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-05 03:40:02.000000 backend.ai-common-24.3.0rc4/ai/backend/common/netns.py
--rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-04-05 03:40:02.000000 backend.ai-common-24.3.0rc4/ai/backend/common/networking.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:40:02.417383 backend.ai-common-24.3.0rc4/ai/backend/common/plugin/
--rw-r--r--   0 runner    (1001) docker     (127)     6990 2024-04-05 03:40:02.000000 backend.ai-common-24.3.0rc4/ai/backend/common/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5646 2024-04-05 03:40:02.000000 backend.ai-common-24.3.0rc4/ai/backend/common/plugin/hook.py
--rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-04-05 03:40:02.000000 backend.ai-common-24.3.0rc4/ai/backend/common/plugin/monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-05 03:40:02.000000 backend.ai-common-24.3.0rc4/ai/backend/common/plugin/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-05 03:40:02.000000 backend.ai-common-24.3.0rc4/ai/backend/common/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    18454 2024-04-05 03:40:02.000000 backend.ai-common-24.3.0rc4/ai/backend/common/redis_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     3914 2024-04-05 03:40:02.000000 backend.ai-common-24.3.0rc4/ai/backend/common/sd_notify.py
--rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-04-05 03:40:02.000000 backend.ai-common-24.3.0rc4/ai/backend/common/service_ports.py
--rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-04-05 03:40:02.000000 backend.ai-common-24.3.0rc4/ai/backend/common/testutils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5874 2024-04-05 03:40:02.000000 backend.ai-common-24.3.0rc4/ai/backend/common/typed_validators.py
--rw-r--r--   0 runner    (1001) docker     (127)    37619 2024-04-05 03:40:02.000000 backend.ai-common-24.3.0rc4/ai/backend/common/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    12536 2024-04-05 03:40:02.000000 backend.ai-common-24.3.0rc4/ai/backend/common/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    25246 2024-04-05 03:40:02.000000 backend.ai-common-24.3.0rc4/ai/backend/common/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:40:02.409383 backend.ai-common-24.3.0rc4/ai/backend/common/web/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:40:02.417383 backend.ai-common-24.3.0rc4/ai/backend/common/web/session/
--rw-r--r--   0 runner    (1001) docker     (127)    10784 2024-04-05 03:40:02.000000 backend.ai-common-24.3.0rc4/ai/backend/common/web/session/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3831 2024-04-05 03:40:02.000000 backend.ai-common-24.3.0rc4/ai/backend/common/web/session/redis_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 03:40:02.417383 backend.ai-common-24.3.0rc4/backend.ai_common.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3633 2024-04-05 03:40:02.000000 backend.ai-common-24.3.0rc4/backend.ai_common.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-04-05 03:40:02.000000 backend.ai-common-24.3.0rc4/backend.ai_common.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 03:40:02.000000 backend.ai-common-24.3.0rc4/backend.ai_common.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 03:40:02.000000 backend.ai-common-24.3.0rc4/backend.ai_common.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 03:40:02.000000 backend.ai-common-24.3.0rc4/backend.ai_common.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-05 03:40:02.000000 backend.ai-common-24.3.0rc4/backend.ai_common.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        3 2024-04-05 03:40:02.000000 backend.ai-common-24.3.0rc4/backend.ai_common.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-04-05 03:40:02.000000 backend.ai-common-24.3.0rc4/backend_shim.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 03:40:02.417383 backend.ai-common-24.3.0rc4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4272 2024-04-05 03:40:02.000000 backend.ai-common-24.3.0rc4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:08:33.319079 backend.ai-common-24.3.1rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-16 17:08:32.000000 backend.ai-common-24.3.1rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3609 2024-04-16 17:08:33.315079 backend.ai-common-24.3.1rc1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:08:33.303079 backend.ai-common-24.3.1rc1/ai/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:08:33.303079 backend.ai-common-24.3.1rc1/ai/backend/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:08:33.311079 backend.ai-common-24.3.1rc1/ai/backend/common/
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-16 17:08:32.000000 backend.ai-common-24.3.1rc1/ai/backend/common/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-16 17:08:32.000000 backend.ai-common-24.3.1rc1/ai/backend/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-16 17:08:32.000000 backend.ai-common-24.3.1rc1/ai/backend/common/arch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-04-16 17:08:32.000000 backend.ai-common-24.3.1rc1/ai/backend/common/argparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3055 2024-04-16 17:08:32.000000 backend.ai-common-24.3.1rc1/ai/backend/common/asyncio.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:08:33.315079 backend.ai-common-24.3.1rc1/ai/backend/common/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-04-16 17:08:32.000000 backend.ai-common-24.3.1rc1/ai/backend/common/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11477 2024-04-16 17:08:32.000000 backend.ai-common-24.3.1rc1/ai/backend/common/bgtask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3781 2024-04-16 17:08:32.000000 backend.ai-common-24.3.1rc1/ai/backend/common/cgroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3021 2024-04-16 17:08:32.000000 backend.ai-common-24.3.1rc1/ai/backend/common/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8540 2024-04-16 17:08:32.000000 backend.ai-common-24.3.1rc1/ai/backend/common/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-16 17:08:32.000000 backend.ai-common-24.3.1rc1/ai/backend/common/defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2576 2024-04-16 17:08:32.000000 backend.ai-common-24.3.1rc1/ai/backend/common/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21291 2024-04-16 17:08:32.000000 backend.ai-common-24.3.1rc1/ai/backend/common/docker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-16 17:08:32.000000 backend.ai-common-24.3.1rc1/ai/backend/common/enum_extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-04-16 17:08:32.000000 backend.ai-common-24.3.1rc1/ai/backend/common/enum_extension.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    21031 2024-04-16 17:08:32.000000 backend.ai-common-24.3.1rc1/ai/backend/common/etcd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33020 2024-04-16 17:08:32.000000 backend.ai-common-24.3.1rc1/ai/backend/common/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2585 2024-04-16 17:08:32.000000 backend.ai-common-24.3.1rc1/ai/backend/common/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-04-16 17:08:32.000000 backend.ai-common-24.3.1rc1/ai/backend/common/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9964 2024-04-16 17:08:32.000000 backend.ai-common-24.3.1rc1/ai/backend/common/identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-16 17:08:32.000000 backend.ai-common-24.3.1rc1/ai/backend/common/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7984 2024-04-16 17:08:32.000000 backend.ai-common-24.3.1rc1/ai/backend/common/lock.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23163 2024-04-16 17:08:32.000000 backend.ai-common-24.3.1rc1/ai/backend/common/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-16 17:08:32.000000 backend.ai-common-24.3.1rc1/ai/backend/common/logging_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:08:33.303079 backend.ai-common-24.3.1rc1/ai/backend/common/models/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:08:33.315079 backend.ai-common-24.3.1rc1/ai/backend/common/models/minilang/
+-rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-04-16 17:08:32.000000 backend.ai-common-24.3.1rc1/ai/backend/common/models/minilang/mount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-04-16 17:08:32.000000 backend.ai-common-24.3.1rc1/ai/backend/common/msgpack.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-16 17:08:32.000000 backend.ai-common-24.3.1rc1/ai/backend/common/netns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-04-16 17:08:32.000000 backend.ai-common-24.3.1rc1/ai/backend/common/networking.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:08:33.315079 backend.ai-common-24.3.1rc1/ai/backend/common/plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)     6990 2024-04-16 17:08:32.000000 backend.ai-common-24.3.1rc1/ai/backend/common/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5646 2024-04-16 17:08:32.000000 backend.ai-common-24.3.1rc1/ai/backend/common/plugin/hook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-04-16 17:08:32.000000 backend.ai-common-24.3.1rc1/ai/backend/common/plugin/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-16 17:08:32.000000 backend.ai-common-24.3.1rc1/ai/backend/common/plugin/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-16 17:08:32.000000 backend.ai-common-24.3.1rc1/ai/backend/common/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    18454 2024-04-16 17:08:32.000000 backend.ai-common-24.3.1rc1/ai/backend/common/redis_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3914 2024-04-16 17:08:32.000000 backend.ai-common-24.3.1rc1/ai/backend/common/sd_notify.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-04-16 17:08:32.000000 backend.ai-common-24.3.1rc1/ai/backend/common/service_ports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-04-16 17:08:32.000000 backend.ai-common-24.3.1rc1/ai/backend/common/testutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5874 2024-04-16 17:08:32.000000 backend.ai-common-24.3.1rc1/ai/backend/common/typed_validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37619 2024-04-16 17:08:32.000000 backend.ai-common-24.3.1rc1/ai/backend/common/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12540 2024-04-16 17:08:32.000000 backend.ai-common-24.3.1rc1/ai/backend/common/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25051 2024-04-16 17:08:32.000000 backend.ai-common-24.3.1rc1/ai/backend/common/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:08:33.303079 backend.ai-common-24.3.1rc1/ai/backend/common/web/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:08:33.315079 backend.ai-common-24.3.1rc1/ai/backend/common/web/session/
+-rw-r--r--   0 runner    (1001) docker     (127)    10784 2024-04-16 17:08:32.000000 backend.ai-common-24.3.1rc1/ai/backend/common/web/session/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3831 2024-04-16 17:08:32.000000 backend.ai-common-24.3.1rc1/ai/backend/common/web/session/redis_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:08:33.315079 backend.ai-common-24.3.1rc1/backend.ai_common.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3609 2024-04-16 17:08:33.000000 backend.ai-common-24.3.1rc1/backend.ai_common.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-04-16 17:08:33.000000 backend.ai-common-24.3.1rc1/backend.ai_common.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 17:08:33.000000 backend.ai-common-24.3.1rc1/backend.ai_common.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 17:08:33.000000 backend.ai-common-24.3.1rc1/backend.ai_common.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 17:08:33.000000 backend.ai-common-24.3.1rc1/backend.ai_common.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-16 17:08:33.000000 backend.ai-common-24.3.1rc1/backend.ai_common.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2024-04-16 17:08:33.000000 backend.ai-common-24.3.1rc1/backend.ai_common.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-04-16 17:08:32.000000 backend.ai-common-24.3.1rc1/backend_shim.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 17:08:33.319079 backend.ai-common-24.3.1rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4252 2024-04-16 17:08:32.000000 backend.ai-common-24.3.1rc1/setup.py
```

### Comparing `backend.ai-common-24.3.0rc4/PKG-INFO` & `backend.ai-common-24.3.1rc1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backend.ai-common
-Version: 24.3.0rc4
+Version: 24.3.1rc1
 Summary: Backend.AI commons library
 Home-page: https://github.com/lablup/backend.ai
 Author: Lablup Inc. and contributors
 License: LGPLv3
 Project-URL: Documentation, https://docs.backend.ai/
 Project-URL: Source, https://github.com/lablup/backend.ai
 Classifier: Intended Audience :: Developers
@@ -18,51 +18,50 @@
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Requires-Python: >=3.12,<3.13
 Description-Content-Type: text/markdown
 Requires-Dist: PyJWT~=2.0
 Requires-Dist: aiodns>=3.0
-Requires-Dist: aiofiles~=0.8.0
+Requires-Dist: aiofiles~=23.2.1
 Requires-Dist: aiohttp_sse>=2.0
 Requires-Dist: aiohttp~=3.9.1
 Requires-Dist: aiomonitor~=0.7.0
 Requires-Dist: aiotools~=1.7.0
 Requires-Dist: async_timeout~=4.0
 Requires-Dist: asynctest>=0.13.0
 Requires-Dist: asyncudp>=0.4
 Requires-Dist: attrs>=20.3
-Requires-Dist: backend.ai-plugin==24.03.0rc4
+Requires-Dist: backend.ai-plugin==24.03.1rc1
 Requires-Dist: callosum~=1.0.3
 Requires-Dist: click~=8.1.7
 Requires-Dist: coloredlogs~=15.0
-Requires-Dist: etcd-client-py==0.2.4
+Requires-Dist: etcd-client-py==0.3.0
 Requires-Dist: graypy==2.1.0
 Requires-Dist: ifaddr~=0.2
 Requires-Dist: janus~=1.0.0
 Requires-Dist: lark~=1.1.5
 Requires-Dist: msgpack>=1.0.5rc1
 Requires-Dist: multidict>=6.0
 Requires-Dist: packaging>=21.3
 Requires-Dist: psutil~=5.9.1
-Requires-Dist: pydantic~=2.4.2
+Requires-Dist: pydantic~=2.6.4
 Requires-Dist: python-dateutil>=2.8
 Requires-Dist: python-json-logger>=2.0.1
 Requires-Dist: pyzmq~=25.1.2
 Requires-Dist: redis[hiredis]==4.5.5
-Requires-Dist: tblib~=1.7
 Requires-Dist: temporenc~=0.1.0
 Requires-Dist: tenacity>=8.0
 Requires-Dist: tomli~=2.0.1
 Requires-Dist: trafaret~=2.1
 Requires-Dist: typeguard~=2.10
 Requires-Dist: types-aiofiles
 Requires-Dist: types-python-dateutil
 Requires-Dist: types-redis
-Requires-Dist: typing_extensions~=4.3
+Requires-Dist: typing_extensions~=4.11
 Requires-Dist: yarl!=1.9.0,!=1.9.1,!=1.9.2,<2.0,>=1.8.2
 
 Backend.AI Commons
 ==================
 
 [![PyPI release version](https://badge.fury.io/py/backend.ai-common.svg)](https://pypi.org/project/backend.ai-common/)
 ![Supported Python versions](https://img.shields.io/pypi/pyversions/backend.ai-common.svg)
```

### Comparing `backend.ai-common-24.3.0rc4/ai/backend/common/argparse.py` & `backend.ai-common-24.3.1rc1/ai/backend/common/argparse.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-24.3.0rc4/ai/backend/common/asyncio.py` & `backend.ai-common-24.3.1rc1/ai/backend/common/asyncio.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-24.3.0rc4/ai/backend/common/auth/__init__.py` & `backend.ai-common-24.3.1rc1/ai/backend/common/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-24.3.0rc4/ai/backend/common/bgtask.py` & `backend.ai-common-24.3.1rc1/ai/backend/common/bgtask.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-24.3.0rc4/ai/backend/common/cgroup.py` & `backend.ai-common-24.3.1rc1/ai/backend/common/cgroup.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-24.3.0rc4/ai/backend/common/cli.py` & `backend.ai-common-24.3.1rc1/ai/backend/common/cli.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-24.3.0rc4/ai/backend/common/config.py` & `backend.ai-common-24.3.1rc1/ai/backend/common/config.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-24.3.0rc4/ai/backend/common/distributed.py` & `backend.ai-common-24.3.1rc1/ai/backend/common/distributed.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-24.3.0rc4/ai/backend/common/docker.py` & `backend.ai-common-24.3.1rc1/ai/backend/common/docker.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-24.3.0rc4/ai/backend/common/enum_extension.py` & `backend.ai-common-24.3.1rc1/ai/backend/common/enum_extension.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-24.3.0rc4/ai/backend/common/enum_extension.pyi` & `backend.ai-common-24.3.1rc1/ai/backend/common/enum_extension.pyi`

 * *Files identical despite different names*

### Comparing `backend.ai-common-24.3.0rc4/ai/backend/common/etcd.py` & `backend.ai-common-24.3.1rc1/ai/backend/common/etcd.py`

 * *Files 7% similar despite different names*

```diff
@@ -40,16 +40,16 @@
     Communicator as EtcdCommunicator,
 )
 from etcd_client import (
     Compare,
     CompareOp,
     CondVar,
     ConnectOptions,
-    GRpcStatusCode,
-    GRpcStatusError,
+    GRPCStatusCode,
+    GRPCStatusError,
     TxnOp,
     Watch,
 )
 from etcd_client import (
     Txn as EtcdTransactionAction,
 )
 
@@ -196,15 +196,17 @@
         :param scope: The config scope for putting the values.
         :param scope_prefix_map: The scope map used to mangle the prefix for the config scope.
         :return:
         """
         scope_prefix = self._merge_scope_prefix_map(scope_prefix_map)[scope]
         mangled_key = self._mangle_key(f"{_slash(scope_prefix)}{key}")
         async with self.etcd.connect() as communicator:
-            await communicator.put(mangled_key, str(val))
+            await communicator.put(
+                mangled_key.encode(self.encoding), str(val).encode(self.encoding)
+            )
 
     async def put_prefix(
         self,
         key: str,
         dict_obj: NestedStrKeyedMapping,
         *,
         scope: ConfigScopes = ConfigScopes.GLOBAL,
@@ -234,15 +236,20 @@
                 else:
                     flattened_dict[flattened_key] = v
 
         _flatten(key, cast(NestedStrKeyedDict, dict_obj))
 
         actions = []
         for k, v in flattened_dict.items():
-            actions.append(TxnOp.put(self._mangle_key(f"{_slash(scope_prefix)}{k}"), str(v)))
+            actions.append(
+                TxnOp.put(
+                    self._mangle_key(f"{_slash(scope_prefix)}{k}").encode(self.encoding),
+                    str(v).encode(self.encoding),
+                )
+            )
 
         async with self.etcd.connect() as communicator:
             await communicator.txn(EtcdTransactionAction().and_then(actions).or_else([]))
 
     async def put_dict(
         self,
         flattened_dict_obj: Mapping[str, str],
@@ -260,15 +267,20 @@
         :param scope_prefix_map: The scope map used to mangle the prefix for the config scope.
         :return:
         """
         scope_prefix = self._merge_scope_prefix_map(scope_prefix_map)[scope]
 
         actions = []
         for k, v in flattened_dict_obj.items():
-            actions.append(TxnOp.put(self._mangle_key(f"{_slash(scope_prefix)}{k}"), str(v)))
+            actions.append(
+                TxnOp.put(
+                    self._mangle_key(f"{_slash(scope_prefix)}{k}").encode(self.encoding),
+                    str(v).encode(self.encoding),
+                )
+            )
 
         async with self.etcd.connect() as communicator:
             await communicator.txn(EtcdTransactionAction().and_then(actions).or_else([]))
 
     async def get(
         self,
         key: str,
@@ -304,17 +316,19 @@
         elif scope == ConfigScopes.GLOBAL:
             scope_prefixes = [_scope_prefix_map[ConfigScopes.GLOBAL]]
         else:
             raise ValueError("Invalid scope prefix value")
 
         async with self.etcd.connect() as communicator:
             for scope_prefix in scope_prefixes:
-                value = await communicator.get(self._mangle_key(f"{_slash(scope_prefix)}{key}"))
+                value = await communicator.get(
+                    self._mangle_key(f"{_slash(scope_prefix)}{key}").encode(self.encoding)
+                )
                 if value is not None:
-                    return value
+                    return bytes(value).decode(self.encoding)
         return None
 
     async def get_prefix(
         self,
         key_prefix: str,
         *,
         scope: ConfigScopes = ConfigScopes.MERGED,
@@ -373,16 +387,22 @@
             scope_prefixes = [_scope_prefix_map[ConfigScopes.GLOBAL]]
         else:
             raise ValueError("Invalid scope prefix value")
         pair_sets: List[List[Mapping | Tuple]] = []
         async with self.etcd.connect() as communicator:
             for scope_prefix in scope_prefixes:
                 mangled_key_prefix = self._mangle_key(f"{_slash(scope_prefix)}{key_prefix}")
-                values = await communicator.get_prefix(mangled_key_prefix)
-                pair_sets.append([(self._demangle_key(k), v) for k, v in values.items()])
+                values = await communicator.get_prefix(mangled_key_prefix.encode(self.encoding))
+                pair_sets.append([
+                    (
+                        self._demangle_key(bytes(k).decode(self.encoding)),
+                        bytes(v).decode(self.encoding),
+                    )
+                    for k, v in values
+                ])
 
         pair_sets = [sorted(pairs, key=lambda x: x[0]) for pairs in pair_sets]
 
         configs = [
             make_dict_from_pairs(f"{_slash(scope_prefix)}{key_prefix}", pairs, "/")
             for scope_prefix, pairs in zip(scope_prefixes, pair_sets)
         ]
@@ -403,17 +423,23 @@
         scope_prefix = self._merge_scope_prefix_map(scope_prefix_map)[scope]
         mangled_key = self._mangle_key(f"{_slash(scope_prefix)}{key}")
 
         async with self.etcd.connect() as communicator:
             result = await communicator.txn(
                 EtcdTransactionAction()
                 .when([
-                    Compare.value(mangled_key, CompareOp.EQUAL, initial_val),
+                    Compare.value(
+                        mangled_key.encode(self.encoding),
+                        CompareOp.EQUAL,
+                        initial_val.encode(self.encoding),
+                    ),
+                ])
+                .and_then([
+                    TxnOp.put(mangled_key.encode(self.encoding), new_val.encode(self.encoding))
                 ])
-                .and_then([TxnOp.put(mangled_key, new_val)])
                 .or_else([])
             )
 
             return result.succeeded()
 
     async def delete(
         self,
@@ -421,41 +447,45 @@
         *,
         scope: ConfigScopes = ConfigScopes.GLOBAL,
         scope_prefix_map: Mapping[ConfigScopes, str] = None,
     ):
         scope_prefix = self._merge_scope_prefix_map(scope_prefix_map)[scope]
         mangled_key = self._mangle_key(f"{_slash(scope_prefix)}{key}")
         async with self.etcd.connect() as communicator:
-            await communicator.delete(mangled_key)
+            await communicator.delete(mangled_key.encode(self.encoding))
 
     async def delete_multi(
         self,
         keys: Iterable[str],
         *,
         scope: ConfigScopes = ConfigScopes.GLOBAL,
         scope_prefix_map: Mapping[ConfigScopes, str] = None,
     ):
         scope_prefix = self._merge_scope_prefix_map(scope_prefix_map)[scope]
         async with self.etcd.connect() as communicator:
             actions = []
             for k in keys:
-                actions.append(TxnOp.delete(self._mangle_key(f"{_slash(scope_prefix)}{k}")))
+                actions.append(
+                    TxnOp.delete(
+                        self._mangle_key(f"{_slash(scope_prefix)}{k}").encode(self.encoding)
+                    )
+                )
             await communicator.txn(EtcdTransactionAction().and_then(actions).or_else([]))
 
     async def delete_prefix(
         self,
         key_prefix: str,
         *,
         scope: ConfigScopes = ConfigScopes.GLOBAL,
         scope_prefix_map: Mapping[ConfigScopes, str] = None,
     ):
         scope_prefix = self._merge_scope_prefix_map(scope_prefix_map)[scope]
         mangled_key_prefix = self._mangle_key(f"{_slash(scope_prefix)}{key_prefix}")
         async with self.etcd.connect() as communicator:
-            await communicator.delete_prefix(mangled_key_prefix)
+            await communicator.delete_prefix(mangled_key_prefix.encode(self.encoding))
 
     async def _watch_impl(
         self,
         iterator_factory: Callable[[EtcdCommunicator], Watch],
         scope_prefix_len: int,
         once: bool,
         cleanup_event: Optional[CondVar] = None,
@@ -467,15 +497,19 @@
 
                 async for ev in iterator:
                     if wait_timeout is not None:
                         try:
                             ev = await asyncio.wait_for(iterator.__anext__(), wait_timeout)
                         except asyncio.TimeoutError:
                             pass
-                    yield Event(ev.key[scope_prefix_len:], ev.event, ev.value)
+                    yield Event(
+                        bytes(ev.key).decode(self.encoding)[scope_prefix_len:],
+                        ev.event,
+                        bytes(ev.value).decode(self.encoding),
+                    )
                     if once:
                         return
         finally:
             if cleanup_event:
                 await cleanup_event.notify_waiters()
 
     async def watch(
@@ -494,28 +528,28 @@
         mangled_key = self._mangle_key(f"{_slash(scope_prefix)}{key}")
         ended_without_error = False
 
         while not ended_without_error:
             try:
                 async for ev in self._watch_impl(
                     lambda communicator: communicator.watch(
-                        mangled_key,
+                        mangled_key.encode(self.encoding),
                         ready_event=ready_event,
                     ),
                     scope_prefix_len,
                     once,
                     cleanup_event=cleanup_event,
                     wait_timeout=wait_timeout,
                 ):
                     yield ev
                 ended_without_error = True
-            except GRpcStatusError as e:
+            except GRPCStatusError as e:
                 err_detail = e.args[0]
 
-                if err_detail["code"] == GRpcStatusCode.Unavailable:
+                if err_detail["code"] == GRPCStatusCode.Unavailable:
                     log.warning("watch(): error while connecting to Etcd server, retrying...")
                     await asyncio.sleep(self.watch_reconnect_intvl)
                     ended_without_error = False
                 else:
                     raise
 
     async def watch_prefix(
@@ -534,28 +568,28 @@
         mangled_key_prefix = self._mangle_key(f"{_slash(scope_prefix)}{key_prefix}")
         ended_without_error = False
 
         while not ended_without_error:
             try:
                 async for ev in self._watch_impl(
                     lambda communicator: communicator.watch_prefix(
-                        mangled_key_prefix,
+                        mangled_key_prefix.encode(self.encoding),
                         ready_event=ready_event,
                     ),
                     scope_prefix_len,
                     once,
                     cleanup_event=cleanup_event,
                     wait_timeout=wait_timeout,
                 ):
                     yield ev
                 ended_without_error = True
-            except GRpcStatusError as e:
+            except GRPCStatusError as e:
                 err_detail = e.args[0]
 
-                if err_detail["code"] == GRpcStatusCode.Unavailable:
+                if err_detail["code"] == GRPCStatusCode.Unavailable:
                     log.warning(
                         "watch_prefix(): error while connecting to Etcd server, retrying..."
                     )
                     await asyncio.sleep(self.watch_reconnect_intvl)
                     ended_without_error = False
                 else:
                     raise e
```

### Comparing `backend.ai-common-24.3.0rc4/ai/backend/common/events.py` & `backend.ai-common-24.3.1rc1/ai/backend/common/events.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-24.3.0rc4/ai/backend/common/exception.py` & `backend.ai-common-24.3.1rc1/ai/backend/common/exception.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-24.3.0rc4/ai/backend/common/files.py` & `backend.ai-common-24.3.1rc1/ai/backend/common/files.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-24.3.0rc4/ai/backend/common/identity.py` & `backend.ai-common-24.3.1rc1/ai/backend/common/identity.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-24.3.0rc4/ai/backend/common/lock.py` & `backend.ai-common-24.3.1rc1/ai/backend/common/lock.py`

 * *Files 1% similar despite different names*

```diff
@@ -169,15 +169,15 @@
         self._timeout = timeout if timeout is not None else self.default_timeout
         self._debug = debug
         self._etcd_client = None
 
     async def __aenter__(self) -> EtcdCommunicator:
         self._etcd_client = self.etcd.etcd.with_lock(
             EtcdLockOption(
-                lock_name=self.lock_name,
+                lock_name=self.lock_name.encode("utf-8"),
                 timeout=self._timeout,
                 ttl=int(self._lifetime) if self._lifetime is not None else None,
             ),
         )
 
         etcd_communicator = await self._etcd_client.__aenter__()
```

### Comparing `backend.ai-common-24.3.0rc4/ai/backend/common/logging.py` & `backend.ai-common-24.3.1rc1/ai/backend/common/logging.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 import json
 import logging
 import logging.config
 import logging.handlers
 import os
-import pickle
 import pprint
 import socket
 import ssl
 import sys
 import threading
 import time
+import traceback
 from abc import ABCMeta, abstractmethod
 from collections import OrderedDict
 from contextvars import ContextVar
 from datetime import datetime
 from pathlib import Path
 from typing import Any, Mapping, MutableMapping, Optional
 
 import coloredlogs
 import graypy
 import trafaret as t
 import yarl
 import zmq
 from pythonjsonlogger.jsonlogger import JsonFormatter
-from tblib import pickling_support
+
+from ai.backend.common import msgpack
 
 from . import config
 from . import validators as tx
 from .exception import ConfigurationError
 from .logging_utils import BraceStyleAdapter
 
 # public APIs of this module
@@ -167,21 +168,14 @@
             self._zmqctx.term()
 
     def emit(self, record):
         self._setup_transport()
         tags = set()
         extra_data = dict()
 
-        if record.exc_info:
-            tags.add("has_exception")
-            if self.formatter:
-                extra_data["exception"] = self.formatter.formatException(record.exc_info)
-            else:
-                extra_data["exception"] = logging._defaultFormatter.formatException(record.exc_info)
-
         # This log format follows logstash's event format.
         log = OrderedDict([
             ("@timestamp", datetime.now().isoformat()),
             ("@version", 1),
             ("host", self._myhost),
             ("logger", record.name),
             ("path", record.pathname),
@@ -195,25 +189,30 @@
         if self._protocol.startswith("zmq"):
             self._sock.send_json(log)
         else:
             # TODO: reconnect if disconnected
             self._sock.sendall(json.dumps(log).encode("utf-8"))
 
 
+def format_exception(self, ei):
+    s = "".join(ei)
+    if s[-1:] == "\n":
+        s = s[:-1]
+    return s
+
+
+class SerializedExceptionFormatter(logging.Formatter):
+    def formatException(self, ei) -> str:
+        return format_exception(self, ei)
+
+
 class GELFTLSHandler(graypy.GELFTLSHandler):
     ssl_ctx: ssl.SSLContext
 
-    def __init__(
-        self,
-        host,
-        port=12204,
-        validate=False,
-        ca_certs=None,
-        **kwargs
-    ):
+    def __init__(self, host, port=12204, validate=False, ca_certs=None, **kwargs):
         """Initialize the GELFTLSHandler
 
         :param host: GELF TLS input host.
         :type host: str
 
         :param port: GELF TLS input port.
         :type port: int
@@ -237,15 +236,16 @@
         """Create a TLS wrapped socket"""
         plain_socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
 
         if hasattr(plain_socket, "settimeout"):
             plain_socket.settimeout(timeout)
 
         wrapped_socket = self.ssl_ctx.wrap_socket(
-            plain_socket, server_hostname=self.host,
+            plain_socket,
+            server_hostname=self.host,
         )
         wrapped_socket.connect((self.host, self.port))
 
         return wrapped_socket
 
 
 def setup_graylog_handler(config: Mapping[str, Any]) -> Optional[logging.Handler]:
@@ -265,25 +265,31 @@
 
     graylog_handler = GELFTLSHandler(**graylog_params)
     graylog_handler.setLevel(config["level"])
     return graylog_handler
 
 
 class ConsoleFormatter(logging.Formatter):
+    def formatException(self, ei) -> str:
+        return format_exception(self, ei)
+
     def formatTime(self, record: logging.LogRecord, datefmt: str = None) -> str:
         ct = self.converter(record.created)  # type: ignore
         if datefmt:
             datefmt = datefmt.replace("%f", f"{int(record.msecs):03d}")
             return time.strftime(datefmt, ct)
         else:
             t = time.strftime("%Y-%m-%d %H:%M:%S", ct)
             return f"{t}.{int(record.msecs):03d}"
 
 
 class CustomJsonFormatter(JsonFormatter):
+    def formatException(self, ei) -> str:
+        return format_exception(self, ei)
+
     def add_fields(
         self,
         log_record: dict[str, Any],  # the manipulated entry object
         record: logging.LogRecord,  # the source log record
         message_dict: dict[str, Any],
     ) -> None:
         super().add_fields(log_record, record, message_dict)
@@ -293,14 +299,20 @@
             log_record["timestamp"] = now
         if loglevel := log_record.get("level"):
             log_record["level"] = loglevel.upper()
         else:
             log_record["level"] = record.levelname.upper()
 
 
+class ColorizedFormatter(coloredlogs.ColoredFormatter):
+    def __init__(self, *args, **kwargs) -> None:
+        super().__init__(*args, **kwargs)
+        coloredlogs.logging.Formatter.formatException = format_exception
+
+
 class pretty:
     """A simple object wrapper to pretty-format it when formatting the log record."""
 
     def __init__(self, obj: Any) -> None:
         self.obj = obj
 
     def __repr__(self) -> str:
@@ -314,15 +326,15 @@
     }
     drv_config = config["console"]
     console_formatter: logging.Formatter
     colored = drv_config["colored"]
     if colored is None:
         colored = sys.stderr.isatty()
     if colored:
-        console_formatter = coloredlogs.ColoredFormatter(
+        console_formatter = ColorizedFormatter(
             log_formats[drv_config["format"]],
             datefmt="%Y-%m-%d %H:%M:%S.%f",  # coloredlogs has intrinsic support for msec
             field_styles={
                 "levelname": {"color": 248, "bold": True},
                 "name": {"color": 246, "bold": False},
                 "process": {"color": "cyan"},
                 "asctime": {"color": 240},
@@ -372,14 +384,17 @@
     ready_event: threading.Event,
 ) -> None:
     console_handler = None
     file_handler = None
     logstash_handler = None
     graylog_handler = None
 
+    # For future references: when implementing new kind of logging adapters,
+    # make sure to adapt our custom `Formatter.formatException()` approach;
+    # Otherwise it won't print out EXCEPTION level log (along with the traceback).
     if "console" in logging_config["drivers"]:
         console_handler = setup_console_log_handler(logging_config)
 
     if "file" in logging_config["drivers"]:
         file_handler = setup_file_log_handler(logging_config)
 
     if "logstash" in logging_config["drivers"]:
@@ -388,42 +403,36 @@
             endpoint=drv_config["endpoint"],
             protocol=drv_config["protocol"],
             ssl_enabled=drv_config["ssl-enabled"],
             ssl_verify=drv_config["ssl-verify"],
             myhost="hostname",  # TODO: implement
         )
         logstash_handler.setLevel(logging_config["level"])
+        logstash_handler.setFormatter(SerializedExceptionFormatter())
     if "graylog" in logging_config["drivers"]:
         graylog_handler = setup_graylog_handler(logging_config)
+        assert graylog_handler is not None
+        graylog_handler.setFormatter(SerializedExceptionFormatter())
 
     zctx = zmq.Context()
     agg_sock = zctx.socket(zmq.PULL)
     agg_sock.bind(log_endpoint)
     ep_url = yarl.URL(log_endpoint)
     if ep_url.scheme.lower() == "ipc":
         os.chmod(ep_url.path, 0o777)
     try:
         ready_event.set()
         while True:
             data = agg_sock.recv()
             if not data:
                 return
-            try:
-                rec = pickle.loads(data)
-            except (pickle.PickleError, TypeError):
-                # We have an unpickling error.
-                # Change into a self-created log record with exception info.
-                rec = logging.makeLogRecord({
-                    "name": __name__,
-                    "msg": "Cannot unpickle the log record (raw data: %r)",
-                    "levelno": logging.ERROR,
-                    "levelname": "error",
-                    "args": (data,),  # attach the original data for inspection
-                    "exc_info": sys.exc_info(),
-                })
+            unpacked_data = msgpack.unpackb(data)
+            if not unpacked_data:
+                break
+            rec = logging.makeLogRecord(unpacked_data)
             if rec is None:
                 break
             if console_handler:
                 console_handler.emit(rec)
             try:
                 if file_handler:
                     file_handler.emit(rec)
@@ -472,47 +481,30 @@
         print(record.getMessage(), file=sys.stderr)
 
     def emit(self, record: Optional[logging.LogRecord]) -> None:
         if self._sock is None:
             self._fallback(record)
             return
         # record may be None to signal shutdown.
+        if record:
+            log_body = {
+                "name": record.name,
+                "pathname": record.pathname,
+                "lineno": record.lineno,
+                "msg": record.getMessage(),
+                "levelno": record.levelno,
+                "levelname": record.levelname,
+            }
+            if record.exc_info:
+                log_body["exc_info"] = traceback.format_exception(*record.exc_info)
+        else:
+            log_body = None
         try:
-            if record is not None and record.exc_info is not None:
-                pickling_support.install(record.exc_info[1])
-            pickled_rec = pickle.dumps(record)
-        except (
-            pickle.PickleError,
-            TypeError,
-            ImportError,  # when "Python is likely to be shutting down"
-        ):
-            # We have a pickling error.
-            # Change it into a self-created picklable log record with exception info.
-            if record is not None:
-                exc_info: Any
-                if isinstance(record.exc_info, tuple):
-                    exc_info = (
-                        PickledException,
-                        PickledException(repr(record.exc_info[1])),  # store stringified repr
-                        record.exc_info[2],
-                    )
-                else:
-                    exc_info = record.exc_info
-                record = logging.makeLogRecord({
-                    "name": record.name,
-                    "pathname": record.pathname,
-                    "lineno": record.lineno,
-                    "msg": record.getMessage(),
-                    "levelno": record.levelno,
-                    "levelname": record.levelname,
-                    "exc_info": exc_info,
-                })
-            pickled_rec = pickle.dumps(record)
-        try:
-            self._sock.send(pickled_rec)
+            serialized_record = msgpack.packb(log_body)
+            self._sock.send(serialized_record)
         except zmq.ZMQError:
             self._fallback(record)
 
 
 class AbstractLogger(metaclass=ABCMeta):
     def __init__(
         self,
@@ -556,15 +548,15 @@
             console_handler = setup_console_log_handler(self.logging_config)
             log_handlers.append(console_handler)
         if "file" in self.logging_config["drivers"]:
             file_handler = setup_file_log_handler(self.logging_config)
             log_handlers.append(file_handler)
         self.log_config = {
             "version": 1,
-            "disable_existing_loggers": True,
+            "disable_existing_loggers": False,
             "handlers": {
                 "null": {"class": "logging.NullHandler"},
             },
             "loggers": {
                 "": {
                     "handlers": [],
                     "level": cfg["level"],
@@ -642,16 +634,14 @@
                     k: {"handlers": [], "level": v, "propagate": False}
                     for k, v in cfg["pkg-ns"].items()
                 },
             },
         }
 
     def __enter__(self):
-        tx.fix_trafaret_pickle_support()  # monkey-patch for pickling trafaret.DataError
-        pickling_support.install()  # enable pickling of tracebacks
         self.log_config["handlers"]["relay"] = {
             "class": "ai.backend.common.logging.RelayHandler",
             "level": self.logging_config["level"],
             "endpoint": self.log_endpoint,
         }
         for _logger in self.log_config["loggers"].values():
             _logger["handlers"].append("relay")
```

### Comparing `backend.ai-common-24.3.0rc4/ai/backend/common/logging_utils.py` & `backend.ai-common-24.3.1rc1/ai/backend/common/logging_utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 class BraceStyleAdapter(logging.LoggerAdapter):
     def __init__(self, logger, extra=None):
         super().__init__(logger, extra)
 
     def log(self, level, msg, *args, **kwargs):
         if self.isEnabledFor(level):
             msg, kwargs = self.process(msg, kwargs)
+            kwargs["stacklevel"] = kwargs.get("stacklevel", 1) + 1
             self.logger._log(level, BraceMessage(msg, args), (), **kwargs)
 
 
 def enforce_debug_logging(loggers: Iterable[str]) -> None:
     # Backend.AI's daemon logging:
     # - All handlers are added to the root logger only.
     #   -> Need to override the log level of the root logger's handlers.
```

### Comparing `backend.ai-common-24.3.0rc4/ai/backend/common/models/minilang/mount.py` & `backend.ai-common-24.3.1rc1/ai/backend/common/models/minilang/mount.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-24.3.0rc4/ai/backend/common/msgpack.py` & `backend.ai-common-24.3.1rc1/ai/backend/common/msgpack.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-24.3.0rc4/ai/backend/common/netns.py` & `backend.ai-common-24.3.1rc1/ai/backend/common/netns.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-24.3.0rc4/ai/backend/common/networking.py` & `backend.ai-common-24.3.1rc1/ai/backend/common/networking.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-24.3.0rc4/ai/backend/common/plugin/__init__.py` & `backend.ai-common-24.3.1rc1/ai/backend/common/plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-24.3.0rc4/ai/backend/common/plugin/hook.py` & `backend.ai-common-24.3.1rc1/ai/backend/common/plugin/hook.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-24.3.0rc4/ai/backend/common/plugin/monitor.py` & `backend.ai-common-24.3.1rc1/ai/backend/common/plugin/monitor.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-24.3.0rc4/ai/backend/common/redis_helper.py` & `backend.ai-common-24.3.1rc1/ai/backend/common/redis_helper.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-24.3.0rc4/ai/backend/common/sd_notify.py` & `backend.ai-common-24.3.1rc1/ai/backend/common/sd_notify.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-24.3.0rc4/ai/backend/common/service_ports.py` & `backend.ai-common-24.3.1rc1/ai/backend/common/service_ports.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-24.3.0rc4/ai/backend/common/testutils.py` & `backend.ai-common-24.3.1rc1/ai/backend/common/testutils.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-24.3.0rc4/ai/backend/common/typed_validators.py` & `backend.ai-common-24.3.1rc1/ai/backend/common/typed_validators.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-24.3.0rc4/ai/backend/common/types.py` & `backend.ai-common-24.3.1rc1/ai/backend/common/types.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-24.3.0rc4/ai/backend/common/utils.py` & `backend.ai-common-24.3.1rc1/ai/backend/common/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -160,15 +160,15 @@
         o = o[p]
     if o is None and null_as_default:
         return def_val
     return o
 
 
 def readable_size_to_bytes(expr: Any) -> BinarySize | Decimal:
-    if isinstance(expr, numbers.Real):
+    if isinstance(expr, numbers.Integral):
         return BinarySize(expr)
     return BinarySize.from_str(expr)
 
 
 def str_to_timedelta(tstr: str) -> timedelta:
     """
     Convert humanized timedelta string into a Python timedelta object.
```

### Comparing `backend.ai-common-24.3.0rc4/ai/backend/common/validators.py` & `backend.ai-common-24.3.1rc1/ai/backend/common/validators.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,21 +72,14 @@
     "TimeZone",
     "TimeDuration",
     "Slug",
     "URL",
 )
 
 
-def fix_trafaret_pickle_support():
-    def __reduce__(self):
-        return (type(self), (self.error, self.name, self.value, self.trafaret, self.code))
-
-    t.DataError.__reduce__ = __reduce__
-
-
 class StringLengthMeta(TrafaretMeta):
     """
     A metaclass that makes string-like trafarets to have sliced min/max length indicator.
     """
 
     def __getitem__(cls, slice_):
         return cls(min_length=slice_.start, max_length=slice_.stop)
```

### Comparing `backend.ai-common-24.3.0rc4/ai/backend/common/web/session/__init__.py` & `backend.ai-common-24.3.1rc1/ai/backend/common/web/session/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-24.3.0rc4/ai/backend/common/web/session/redis_storage.py` & `backend.ai-common-24.3.1rc1/ai/backend/common/web/session/redis_storage.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-24.3.0rc4/backend.ai_common.egg-info/PKG-INFO` & `backend.ai-common-24.3.1rc1/backend.ai_common.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backend.ai-common
-Version: 24.3.0rc4
+Version: 24.3.1rc1
 Summary: Backend.AI commons library
 Home-page: https://github.com/lablup/backend.ai
 Author: Lablup Inc. and contributors
 License: LGPLv3
 Project-URL: Documentation, https://docs.backend.ai/
 Project-URL: Source, https://github.com/lablup/backend.ai
 Classifier: Intended Audience :: Developers
@@ -18,51 +18,50 @@
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Requires-Python: >=3.12,<3.13
 Description-Content-Type: text/markdown
 Requires-Dist: PyJWT~=2.0
 Requires-Dist: aiodns>=3.0
-Requires-Dist: aiofiles~=0.8.0
+Requires-Dist: aiofiles~=23.2.1
 Requires-Dist: aiohttp_sse>=2.0
 Requires-Dist: aiohttp~=3.9.1
 Requires-Dist: aiomonitor~=0.7.0
 Requires-Dist: aiotools~=1.7.0
 Requires-Dist: async_timeout~=4.0
 Requires-Dist: asynctest>=0.13.0
 Requires-Dist: asyncudp>=0.4
 Requires-Dist: attrs>=20.3
-Requires-Dist: backend.ai-plugin==24.03.0rc4
+Requires-Dist: backend.ai-plugin==24.03.1rc1
 Requires-Dist: callosum~=1.0.3
 Requires-Dist: click~=8.1.7
 Requires-Dist: coloredlogs~=15.0
-Requires-Dist: etcd-client-py==0.2.4
+Requires-Dist: etcd-client-py==0.3.0
 Requires-Dist: graypy==2.1.0
 Requires-Dist: ifaddr~=0.2
 Requires-Dist: janus~=1.0.0
 Requires-Dist: lark~=1.1.5
 Requires-Dist: msgpack>=1.0.5rc1
 Requires-Dist: multidict>=6.0
 Requires-Dist: packaging>=21.3
 Requires-Dist: psutil~=5.9.1
-Requires-Dist: pydantic~=2.4.2
+Requires-Dist: pydantic~=2.6.4
 Requires-Dist: python-dateutil>=2.8
 Requires-Dist: python-json-logger>=2.0.1
 Requires-Dist: pyzmq~=25.1.2
 Requires-Dist: redis[hiredis]==4.5.5
-Requires-Dist: tblib~=1.7
 Requires-Dist: temporenc~=0.1.0
 Requires-Dist: tenacity>=8.0
 Requires-Dist: tomli~=2.0.1
 Requires-Dist: trafaret~=2.1
 Requires-Dist: typeguard~=2.10
 Requires-Dist: types-aiofiles
 Requires-Dist: types-python-dateutil
 Requires-Dist: types-redis
-Requires-Dist: typing_extensions~=4.3
+Requires-Dist: typing_extensions~=4.11
 Requires-Dist: yarl!=1.9.0,!=1.9.1,!=1.9.2,<2.0,>=1.8.2
 
 Backend.AI Commons
 ==================
 
 [![PyPI release version](https://badge.fury.io/py/backend.ai-common.svg)](https://pypi.org/project/backend.ai-common/)
 ![Supported Python versions](https://img.shields.io/pypi/pyversions/backend.ai-common.svg)
```

### Comparing `backend.ai-common-24.3.0rc4/backend.ai_common.egg-info/SOURCES.txt` & `backend.ai-common-24.3.1rc1/backend.ai_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `backend.ai-common-24.3.0rc4/backend.ai_common.egg-info/requires.txt` & `backend.ai-common-24.3.1rc1/backend.ai_common.egg-info/requires.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,40 +1,39 @@
 PyJWT~=2.0
 aiodns>=3.0
-aiofiles~=0.8.0
+aiofiles~=23.2.1
 aiohttp_sse>=2.0
 aiohttp~=3.9.1
 aiomonitor~=0.7.0
 aiotools~=1.7.0
 async_timeout~=4.0
 asynctest>=0.13.0
 asyncudp>=0.4
 attrs>=20.3
-backend.ai-plugin==24.03.0rc4
+backend.ai-plugin==24.03.1rc1
 callosum~=1.0.3
 click~=8.1.7
 coloredlogs~=15.0
-etcd-client-py==0.2.4
+etcd-client-py==0.3.0
 graypy==2.1.0
 ifaddr~=0.2
 janus~=1.0.0
 lark~=1.1.5
 msgpack>=1.0.5rc1
 multidict>=6.0
 packaging>=21.3
 psutil~=5.9.1
-pydantic~=2.4.2
+pydantic~=2.6.4
 python-dateutil>=2.8
 python-json-logger>=2.0.1
 pyzmq~=25.1.2
 redis[hiredis]==4.5.5
-tblib~=1.7
 temporenc~=0.1.0
 tenacity>=8.0
 tomli~=2.0.1
 trafaret~=2.1
 typeguard~=2.10
 types-aiofiles
 types-python-dateutil
 types-redis
-typing_extensions~=4.3
+typing_extensions~=4.11
 yarl!=1.9.0,!=1.9.1,!=1.9.2,<2.0,>=1.8.2
```

### Comparing `backend.ai-common-24.3.0rc4/backend_shim.py` & `backend.ai-common-24.3.1rc1/backend_shim.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-24.3.0rc4/setup.py` & `backend.ai-common-24.3.1rc1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,52 +19,51 @@
         'Programming Language :: Python :: 3.12',
         'License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)',
     ],
     'description': 'Backend.AI commons library',
     'install_requires': (
         'PyJWT~=2.0',
         'aiodns>=3.0',
-        'aiofiles~=0.8.0',
+        'aiofiles~=23.2.1',
         'aiohttp_sse>=2.0',
         'aiohttp~=3.9.1',
         'aiomonitor~=0.7.0',
         'aiotools~=1.7.0',
         'async_timeout~=4.0',
         'asynctest>=0.13.0',
         'asyncudp>=0.4',
         'attrs>=20.3',
-        """backend.ai-plugin==24.03.0rc4
+        """backend.ai-plugin==24.03.1rc1
 """,
         'callosum~=1.0.3',
         'click~=8.1.7',
         'coloredlogs~=15.0',
-        'etcd-client-py==0.2.4',
+        'etcd-client-py==0.3.0',
         'graypy==2.1.0',
         'ifaddr~=0.2',
         'janus~=1.0.0',
         'lark~=1.1.5',
         'msgpack>=1.0.5rc1',
         'multidict>=6.0',
         'packaging>=21.3',
         'psutil~=5.9.1',
-        'pydantic~=2.4.2',
+        'pydantic~=2.6.4',
         'python-dateutil>=2.8',
         'python-json-logger>=2.0.1',
         'pyzmq~=25.1.2',
         'redis[hiredis]==4.5.5',
-        'tblib~=1.7',
         'temporenc~=0.1.0',
         'tenacity>=8.0',
         'tomli~=2.0.1',
         'trafaret~=2.1',
         'typeguard~=2.10',
         'types-aiofiles',
         'types-python-dateutil',
         'types-redis',
-        'typing_extensions~=4.3',
+        'typing_extensions~=4.11',
         'yarl!=1.9.0,!=1.9.1,!=1.9.2,<2.0,>=1.8.2',
     ),
     'license': 'LGPLv3',
     'long_description': """Backend.AI Commons
 ==================
 
 [![PyPI release version](https://badge.fury.io/py/backend.ai-common.svg)](https://pypi.org/project/backend.ai-common/)
@@ -127,11 +126,11 @@
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

