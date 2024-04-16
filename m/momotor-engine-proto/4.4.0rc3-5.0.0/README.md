# Comparing `tmp/momotor-engine-proto-4.4.0rc3.tar.gz` & `tmp/momotor_engine_proto-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "momotor-engine-proto-4.4.0rc3.tar", last modified: Mon Mar  7 15:22:02 2022, max compression
+gzip compressed data, was "momotor_engine_proto-5.0.0.tar", last modified: Tue Apr 16 07:54:59 2024, max compression
```

## Comparing `momotor-engine-proto-4.4.0rc3.tar` & `momotor_engine_proto-5.0.0.tar`

### file list

```diff
@@ -1,77 +1,126 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-07 15:22:02.000000 momotor-engine-proto-4.4.0rc3/
--rw-r--r--   0 root         (0) root         (0)     1887 2022-03-07 15:22:02.000000 momotor-engine-proto-4.4.0rc3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      828 2022-03-07 15:20:12.000000 momotor-engine-proto-4.4.0rc3/README.md
--rw-r--r--   0 root         (0) root         (0)       41 2022-03-07 15:22:02.000000 momotor-engine-proto-4.4.0rc3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2362 2022-03-07 15:20:12.000000 momotor-engine-proto-4.4.0rc3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-07 15:22:02.000000 momotor-engine-proto-4.4.0rc3/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-07 15:22:02.000000 momotor-engine-proto-4.4.0rc3/src/momotor/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-07 15:22:02.000000 momotor-engine-proto-4.4.0rc3/src/momotor/rpc/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-03-07 15:20:12.000000 momotor-engine-proto-4.4.0rc3/src/momotor/rpc/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-07 15:22:02.000000 momotor-engine-proto-4.4.0rc3/src/momotor/rpc/asset/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-03-07 15:20:12.000000 momotor-engine-proto-4.4.0rc3/src/momotor/rpc/asset/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      153 2022-03-07 15:20:12.000000 momotor-engine-proto-4.4.0rc3/src/momotor/rpc/asset/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     8405 2022-03-07 15:20:12.000000 momotor-engine-proto-4.4.0rc3/src/momotor/rpc/asset/remote.py
--rw-rw-rw-   0 root         (0) root         (0)     3513 2022-03-07 15:20:12.000000 momotor-engine-proto-4.4.0rc3/src/momotor/rpc/asset/server.py
--rw-rw-rw-   0 root         (0) root         (0)     3603 2022-03-07 15:20:12.000000 momotor-engine-proto-4.4.0rc3/src/momotor/rpc/asset/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-07 15:22:02.000000 momotor-engine-proto-4.4.0rc3/src/momotor/rpc/auth/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-03-07 15:20:12.000000 momotor-engine-proto-4.4.0rc3/src/momotor/rpc/auth/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7136 2022-03-07 15:20:12.000000 momotor-engine-proto-4.4.0rc3/src/momotor/rpc/auth/client.py
--rw-rw-rw-   0 root         (0) root         (0)     2576 2022-03-07 15:20:12.000000 momotor-engine-proto-4.4.0rc3/src/momotor/rpc/auth/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     1024 2022-03-07 15:20:12.000000 momotor-engine-proto-4.4.0rc3/src/momotor/rpc/const.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-07 15:22:02.000000 momotor-engine-proto-4.4.0rc3/src/momotor/rpc/exception/
--rw-rw-rw-   0 root         (0) root         (0)     3886 2022-03-07 15:20:12.000000 momotor-engine-proto-4.4.0rc3/src/momotor/rpc/exception/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-07 15:22:02.000000 momotor-engine-proto-4.4.0rc3/src/momotor/rpc/hash/
--rw-rw-rw-   0 root         (0) root         (0)     4438 2022-03-07 15:20:12.000000 momotor-engine-proto-4.4.0rc3/src/momotor/rpc/hash/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       46 2022-03-07 15:20:12.000000 momotor-engine-proto-4.4.0rc3/src/momotor/rpc/hash/const.py
--rw-rw-rw-   0 root         (0) root         (0)     1674 2022-03-07 15:20:12.000000 momotor-engine-proto-4.4.0rc3/src/momotor/rpc/hash/funcs.py
--rw-rw-rw-   0 root         (0) root         (0)     1590 2022-03-07 15:20:12.000000 momotor-engine-proto-4.4.0rc3/src/momotor/rpc/hash/identity.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-07 15:22:02.000000 momotor-engine-proto-4.4.0rc3/src/momotor/rpc/proto/
--rw-rw-rw-   0 root         (0) root         (0)        1 2022-03-07 15:20:12.000000 momotor-engine-proto-4.4.0rc3/src/momotor/rpc/proto/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      129 2022-03-07 15:20:12.000000 momotor-engine-proto-4.4.0rc3/src/momotor/rpc/proto/asset_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)    21375 2022-03-07 15:20:12.000000 momotor-engine-proto-4.4.0rc3/src/momotor/rpc/proto/asset_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)     2075 2022-03-07 15:20:12.000000 momotor-engine-proto-4.4.0rc3/src/momotor/rpc/proto/auth_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)    14079 2022-03-07 15:20:12.000000 momotor-engine-proto-4.4.0rc3/src/momotor/rpc/proto/auth_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)     5916 2022-03-07 15:20:12.000000 momotor-engine-proto-4.4.0rc3/src/momotor/rpc/proto/client_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)     5169 2022-03-07 15:20:12.000000 momotor-engine-proto-4.4.0rc3/src/momotor/rpc/proto/client_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)      133 2022-03-07 15:20:12.000000 momotor-engine-proto-4.4.0rc3/src/momotor/rpc/proto/exception_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)     4560 2022-03-07 15:20:12.000000 momotor-engine-proto-4.4.0rc3/src/momotor/rpc/proto/exception_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)      127 2022-03-07 15:20:12.000000 momotor-engine-proto-4.4.0rc3/src/momotor/rpc/proto/job_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)    25786 2022-03-07 15:20:12.000000 momotor-engine-proto-4.4.0rc3/src/momotor/rpc/proto/job_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)      132 2022-03-07 15:20:12.000000 momotor-engine-proto-4.4.0rc3/src/momotor/rpc/proto/priority_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)     2519 2022-03-07 15:20:12.000000 momotor-engine-proto-4.4.0rc3/src/momotor/rpc/proto/priority_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)      132 2022-03-07 15:20:12.000000 momotor-engine-proto-4.4.0rc3/src/momotor/rpc/proto/resource_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)     2437 2022-03-07 15:20:12.000000 momotor-engine-proto-4.4.0rc3/src/momotor/rpc/proto/resource_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)      130 2022-03-07 15:20:12.000000 momotor-engine-proto-4.4.0rc3/src/momotor/rpc/proto/shared_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)     5306 2022-03-07 15:20:12.000000 momotor-engine-proto-4.4.0rc3/src/momotor/rpc/proto/shared_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)      128 2022-03-07 15:20:12.000000 momotor-engine-proto-4.4.0rc3/src/momotor/rpc/proto/task_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)     9890 2022-03-07 15:20:12.000000 momotor-engine-proto-4.4.0rc3/src/momotor/rpc/proto/task_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)      128 2022-03-07 15:20:12.000000 momotor-engine-proto-4.4.0rc3/src/momotor/rpc/proto/tool_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)     1957 2022-03-07 15:20:12.000000 momotor-engine-proto-4.4.0rc3/src/momotor/rpc/proto/tool_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)     4599 2022-03-07 15:20:12.000000 momotor-engine-proto-4.4.0rc3/src/momotor/rpc/proto/worker_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)     8053 2022-03-07 15:20:12.000000 momotor-engine-proto-4.4.0rc3/src/momotor/rpc/proto/worker_pb2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-07 15:22:02.000000 momotor-engine-proto-4.4.0rc3/src/momotor/rpc/resources/
--rw-rw-rw-   0 root         (0) root         (0)     1094 2022-03-07 15:20:12.000000 momotor-engine-proto-4.4.0rc3/src/momotor/rpc/resources/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-07 15:22:02.000000 momotor-engine-proto-4.4.0rc3/src/momotor/rpc/shared/
--rw-rw-rw-   0 root         (0) root         (0)     2017 2022-03-07 15:20:12.000000 momotor-engine-proto-4.4.0rc3/src/momotor/rpc/shared/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-07 15:22:02.000000 momotor-engine-proto-4.4.0rc3/src/momotor/rpc/status/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-03-07 15:20:12.000000 momotor-engine-proto-4.4.0rc3/src/momotor/rpc/status/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1147 2022-03-07 15:20:12.000000 momotor-engine-proto-4.4.0rc3/src/momotor/rpc/status/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-07 15:22:02.000000 momotor-engine-proto-4.4.0rc3/src/momotor/rpc/task/
--rw-rw-rw-   0 root         (0) root         (0)     1307 2022-03-07 15:20:12.000000 momotor-engine-proto-4.4.0rc3/src/momotor/rpc/task/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-07 15:22:02.000000 momotor-engine-proto-4.4.0rc3/src/momotor/rpc/tools/
--rw-rw-rw-   0 root         (0) root         (0)      756 2022-03-07 15:20:12.000000 momotor-engine-proto-4.4.0rc3/src/momotor/rpc/tools/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1388 2022-03-07 15:20:12.000000 momotor-engine-proto-4.4.0rc3/src/momotor/rpc/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-07 15:22:02.000000 momotor-engine-proto-4.4.0rc3/src/momotor/rpc/validate/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-03-07 15:20:12.000000 momotor-engine-proto-4.4.0rc3/src/momotor/rpc/validate/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1817 2022-03-07 15:20:12.000000 momotor-engine-proto-4.4.0rc3/src/momotor/rpc/validate/base.py
--rw-rw-rw-   0 root         (0) root         (0)     1191 2022-03-07 15:20:12.000000 momotor-engine-proto-4.4.0rc3/src/momotor/rpc/validate/query.py
--rw-rw-rw-   0 root         (0) root         (0)     5014 2022-03-07 15:20:12.000000 momotor-engine-proto-4.4.0rc3/src/momotor/rpc/validate/request.py
--rw-rw-rw-   0 root         (0) root         (0)      656 2022-03-07 15:20:12.000000 momotor-engine-proto-4.4.0rc3/src/momotor/rpc/validate/response.py
--rw-rw-rw-   0 root         (0) root         (0)       22 2022-03-07 15:20:06.000000 momotor-engine-proto-4.4.0rc3/src/momotor/rpc/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-07 15:22:02.000000 momotor-engine-proto-4.4.0rc3/src/momotor_engine_proto.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1887 2022-03-07 15:22:02.000000 momotor-engine-proto-4.4.0rc3/src/momotor_engine_proto.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2048 2022-03-07 15:22:02.000000 momotor-engine-proto-4.4.0rc3/src/momotor_engine_proto.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-03-07 15:22:02.000000 momotor-engine-proto-4.4.0rc3/src/momotor_engine_proto.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-03-07 15:22:02.000000 momotor-engine-proto-4.4.0rc3/src/momotor_engine_proto.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      239 2022-03-07 15:22:02.000000 momotor-engine-proto-4.4.0rc3/src/momotor_engine_proto.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2022-03-07 15:22:02.000000 momotor-engine-proto-4.4.0rc3/src/momotor_engine_proto.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 07:54:59.000000 momotor_engine_proto-5.0.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1215 2024-04-16 07:54:15.000000 momotor_engine_proto-5.0.0/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     3220 2024-04-16 07:54:15.000000 momotor_engine_proto-5.0.0/.gitlab-ci.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 07:54:59.000000 momotor_engine_proto-5.0.0/.idea/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 07:54:59.000000 momotor_engine_proto-5.0.0/.idea/inspectionProfiles/
+-rw-rw-rw-   0 root         (0) root         (0)      174 2024-04-16 07:54:15.000000 momotor_engine_proto-5.0.0/.idea/inspectionProfiles/profiles_settings.xml
+-rw-rw-rw-   0 root         (0) root         (0)      292 2024-04-16 07:54:15.000000 momotor_engine_proto-5.0.0/.idea/modules.xml
+-rw-rw-rw-   0 root         (0) root         (0)     1026 2024-04-16 07:54:15.000000 momotor_engine_proto-5.0.0/.idea/momotor.lib.engine-proto.iml
+-rw-rw-rw-   0 root         (0) root         (0)    46329 2024-04-16 07:54:55.000000 momotor_engine_proto-5.0.0/CHANGELOG.md
+-rw-r--r--   0 root         (0) root         (0)     2862 2024-04-16 07:54:59.000000 momotor_engine_proto-5.0.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      828 2024-04-16 07:54:15.000000 momotor_engine_proto-5.0.0/README.md
+-rwxrwxrwx   0 root         (0) root         (0)      124 2024-04-16 07:54:15.000000 momotor_engine_proto-5.0.0/build.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 07:54:59.000000 momotor_engine_proto-5.0.0/docs/
+-rw-rw-rw-   0 root         (0) root         (0)      638 2024-04-16 07:54:15.000000 momotor_engine_proto-5.0.0/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)      764 2024-04-16 07:54:15.000000 momotor_engine_proto-5.0.0/docs/make.bat
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 07:54:59.000000 momotor_engine_proto-5.0.0/docs/source/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 07:54:59.000000 momotor_engine_proto-5.0.0/docs/source/_static/
+-rw-rw-rw-   0 root         (0) root         (0)     6988 2024-04-16 07:54:15.000000 momotor_engine_proto-5.0.0/docs/source/_static/logo-text-negative.png
+-rw-rw-rw-   0 root         (0) root         (0)     6887 2024-04-16 07:54:15.000000 momotor_engine_proto-5.0.0/docs/source/_static/logo-text.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 07:54:59.000000 momotor_engine_proto-5.0.0/docs/source/_templates/
+-rw-rw-rw-   0 root         (0) root         (0)      672 2024-04-16 07:54:15.000000 momotor_engine_proto-5.0.0/docs/source/_templates/projectlinks.html
+-rw-rw-rw-   0 root         (0) root         (0)      548 2024-04-16 07:54:15.000000 momotor_engine_proto-5.0.0/docs/source/asset.rst
+-rw-rw-rw-   0 root         (0) root         (0)      465 2024-04-16 07:54:15.000000 momotor_engine_proto-5.0.0/docs/source/auth.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4697 2024-04-16 07:54:15.000000 momotor_engine_proto-5.0.0/docs/source/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      191 2024-04-16 07:54:15.000000 momotor_engine_proto-5.0.0/docs/source/const.rst
+-rw-rw-rw-   0 root         (0) root         (0)      282 2024-04-16 07:54:15.000000 momotor_engine_proto-5.0.0/docs/source/exception.rst
+-rw-rw-rw-   0 root         (0) root         (0)      672 2024-04-16 07:54:15.000000 momotor_engine_proto-5.0.0/docs/source/hash.rst
+-rw-rw-rw-   0 root         (0) root         (0)      950 2024-04-16 07:54:15.000000 momotor_engine_proto-5.0.0/docs/source/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3600 2024-04-16 07:54:15.000000 momotor_engine_proto-5.0.0/docs/source/proto.rst
+-rw-rw-rw-   0 root         (0) root         (0)      237 2024-04-16 07:54:15.000000 momotor_engine_proto-5.0.0/docs/source/resources.rst
+-rw-rw-rw-   0 root         (0) root         (0)      187 2024-04-16 07:54:15.000000 momotor_engine_proto-5.0.0/docs/source/shared.rst
+-rw-rw-rw-   0 root         (0) root         (0)       77 2024-04-16 07:54:15.000000 momotor_engine_proto-5.0.0/docs/source/status.rst
+-rw-rw-rw-   0 root         (0) root         (0)      199 2024-04-16 07:54:15.000000 momotor_engine_proto-5.0.0/docs/source/task.rst
+-rw-rw-rw-   0 root         (0) root         (0)      384 2024-04-16 07:54:15.000000 momotor_engine_proto-5.0.0/docs/source/validate.rst
+-rw-rw-rw-   0 root         (0) root         (0)      436 2024-04-16 07:54:15.000000 momotor_engine_proto-5.0.0/publish-docs.sh
+-rw-rw-rw-   0 root         (0) root         (0)     2633 2024-04-16 07:54:15.000000 momotor_engine_proto-5.0.0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      413 2024-04-16 07:54:15.000000 momotor_engine_proto-5.0.0/semver.sh
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-16 07:54:59.000000 momotor_engine_proto-5.0.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       38 2024-04-16 07:54:15.000000 momotor_engine_proto-5.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 07:54:59.000000 momotor_engine_proto-5.0.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 07:54:59.000000 momotor_engine_proto-5.0.0/src/momotor/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 07:54:59.000000 momotor_engine_proto-5.0.0/src/momotor/rpc/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-16 07:54:15.000000 momotor_engine_proto-5.0.0/src/momotor/rpc/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 07:54:59.000000 momotor_engine_proto-5.0.0/src/momotor/rpc/asset/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-16 07:54:15.000000 momotor_engine_proto-5.0.0/src/momotor/rpc/asset/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      153 2024-04-16 07:54:15.000000 momotor_engine_proto-5.0.0/src/momotor/rpc/asset/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     8448 2024-04-16 07:54:15.000000 momotor_engine_proto-5.0.0/src/momotor/rpc/asset/remote.py
+-rw-rw-rw-   0 root         (0) root         (0)     3556 2024-04-16 07:54:15.000000 momotor_engine_proto-5.0.0/src/momotor/rpc/asset/server.py
+-rw-rw-rw-   0 root         (0) root         (0)     3568 2024-04-16 07:54:15.000000 momotor_engine_proto-5.0.0/src/momotor/rpc/asset/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 07:54:59.000000 momotor_engine_proto-5.0.0/src/momotor/rpc/auth/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-16 07:54:15.000000 momotor_engine_proto-5.0.0/src/momotor/rpc/auth/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7111 2024-04-16 07:54:15.000000 momotor_engine_proto-5.0.0/src/momotor/rpc/auth/client.py
+-rw-rw-rw-   0 root         (0) root         (0)     2576 2024-04-16 07:54:15.000000 momotor_engine_proto-5.0.0/src/momotor/rpc/auth/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1029 2024-04-16 07:54:15.000000 momotor_engine_proto-5.0.0/src/momotor/rpc/const.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 07:54:59.000000 momotor_engine_proto-5.0.0/src/momotor/rpc/exception/
+-rw-rw-rw-   0 root         (0) root         (0)     3896 2024-04-16 07:54:15.000000 momotor_engine_proto-5.0.0/src/momotor/rpc/exception/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 07:54:59.000000 momotor_engine_proto-5.0.0/src/momotor/rpc/hash/
+-rw-rw-rw-   0 root         (0) root         (0)     4427 2024-04-16 07:54:15.000000 momotor_engine_proto-5.0.0/src/momotor/rpc/hash/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       46 2024-04-16 07:54:15.000000 momotor_engine_proto-5.0.0/src/momotor/rpc/hash/const.py
+-rw-rw-rw-   0 root         (0) root         (0)     1682 2024-04-16 07:54:15.000000 momotor_engine_proto-5.0.0/src/momotor/rpc/hash/funcs.py
+-rw-rw-rw-   0 root         (0) root         (0)     1599 2024-04-16 07:54:15.000000 momotor_engine_proto-5.0.0/src/momotor/rpc/hash/identity.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 07:54:59.000000 momotor_engine_proto-5.0.0/src/momotor/rpc/proto/
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-04-16 07:54:15.000000 momotor_engine_proto-5.0.0/src/momotor/rpc/proto/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2012 2024-04-16 07:54:15.000000 momotor_engine_proto-5.0.0/src/momotor/rpc/proto/asset.proto
+-rw-rw-rw-   0 root         (0) root         (0)      129 2024-04-16 07:54:15.000000 momotor_engine_proto-5.0.0/src/momotor/rpc/proto/asset_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)     3480 2024-04-16 07:54:15.000000 momotor_engine_proto-5.0.0/src/momotor/rpc/proto/asset_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)     1466 2024-04-16 07:54:15.000000 momotor_engine_proto-5.0.0/src/momotor/rpc/proto/auth.proto
+-rw-rw-rw-   0 root         (0) root         (0)     2075 2024-04-16 07:54:15.000000 momotor_engine_proto-5.0.0/src/momotor/rpc/proto/auth_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)     2720 2024-04-16 07:54:15.000000 momotor_engine_proto-5.0.0/src/momotor/rpc/proto/auth_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)     1771 2024-04-16 07:54:15.000000 momotor_engine_proto-5.0.0/src/momotor/rpc/proto/client.proto
+-rw-rw-rw-   0 root         (0) root         (0)     5916 2024-04-16 07:54:15.000000 momotor_engine_proto-5.0.0/src/momotor/rpc/proto/client_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)     2146 2024-04-16 07:54:15.000000 momotor_engine_proto-5.0.0/src/momotor/rpc/proto/client_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)      253 2024-04-16 07:54:15.000000 momotor_engine_proto-5.0.0/src/momotor/rpc/proto/exception.proto
+-rw-rw-rw-   0 root         (0) root         (0)      133 2024-04-16 07:54:15.000000 momotor_engine_proto-5.0.0/src/momotor/rpc/proto/exception_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)     1469 2024-04-16 07:54:15.000000 momotor_engine_proto-5.0.0/src/momotor/rpc/proto/exception_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)      338 2024-04-16 07:54:15.000000 momotor_engine_proto-5.0.0/src/momotor/rpc/proto/grpc_proto.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1937 2024-04-16 07:54:15.000000 momotor_engine_proto-5.0.0/src/momotor/rpc/proto/job.proto
+-rw-rw-rw-   0 root         (0) root         (0)      127 2024-04-16 07:54:15.000000 momotor_engine_proto-5.0.0/src/momotor/rpc/proto/job_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)     4613 2024-04-16 07:54:15.000000 momotor_engine_proto-5.0.0/src/momotor/rpc/proto/job_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)      144 2024-04-16 07:54:15.000000 momotor_engine_proto-5.0.0/src/momotor/rpc/proto/priority.proto
+-rw-rw-rw-   0 root         (0) root         (0)      132 2024-04-16 07:54:15.000000 momotor_engine_proto-5.0.0/src/momotor/rpc/proto/priority_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)     1257 2024-04-16 07:54:15.000000 momotor_engine_proto-5.0.0/src/momotor/rpc/proto/priority_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)      110 2024-04-16 07:54:15.000000 momotor_engine_proto-5.0.0/src/momotor/rpc/proto/resource.proto
+-rw-rw-rw-   0 root         (0) root         (0)      132 2024-04-16 07:54:15.000000 momotor_engine_proto-5.0.0/src/momotor/rpc/proto/resource_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)     1091 2024-04-16 07:54:15.000000 momotor_engine_proto-5.0.0/src/momotor/rpc/proto/resource_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)     1010 2024-04-16 07:54:15.000000 momotor_engine_proto-5.0.0/src/momotor/rpc/proto/shared.proto
+-rw-rw-rw-   0 root         (0) root         (0)      130 2024-04-16 07:54:15.000000 momotor_engine_proto-5.0.0/src/momotor/rpc/proto/shared_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)     1565 2024-04-16 07:54:15.000000 momotor_engine_proto-5.0.0/src/momotor/rpc/proto/shared_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)      845 2024-04-16 07:54:15.000000 momotor_engine_proto-5.0.0/src/momotor/rpc/proto/task.proto
+-rw-rw-rw-   0 root         (0) root         (0)      128 2024-04-16 07:54:15.000000 momotor_engine_proto-5.0.0/src/momotor/rpc/proto/task_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)     2358 2024-04-16 07:54:15.000000 momotor_engine_proto-5.0.0/src/momotor/rpc/proto/task_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)       70 2024-04-16 07:54:15.000000 momotor_engine_proto-5.0.0/src/momotor/rpc/proto/tool.proto
+-rw-rw-rw-   0 root         (0) root         (0)      128 2024-04-16 07:54:15.000000 momotor_engine_proto-5.0.0/src/momotor/rpc/proto/tool_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)     1048 2024-04-16 07:54:15.000000 momotor_engine_proto-5.0.0/src/momotor/rpc/proto/tool_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)     2548 2024-04-16 07:54:15.000000 momotor_engine_proto-5.0.0/src/momotor/rpc/proto/worker.proto
+-rw-rw-rw-   0 root         (0) root         (0)     4599 2024-04-16 07:54:15.000000 momotor_engine_proto-5.0.0/src/momotor/rpc/proto/worker_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)     2618 2024-04-16 07:54:15.000000 momotor_engine_proto-5.0.0/src/momotor/rpc/proto/worker_pb2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 07:54:59.000000 momotor_engine_proto-5.0.0/src/momotor/rpc/resources/
+-rw-rw-rw-   0 root         (0) root         (0)     1081 2024-04-16 07:54:15.000000 momotor_engine_proto-5.0.0/src/momotor/rpc/resources/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 07:54:59.000000 momotor_engine_proto-5.0.0/src/momotor/rpc/shared/
+-rw-rw-rw-   0 root         (0) root         (0)     2017 2024-04-16 07:54:15.000000 momotor_engine_proto-5.0.0/src/momotor/rpc/shared/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 07:54:59.000000 momotor_engine_proto-5.0.0/src/momotor/rpc/status/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-16 07:54:15.000000 momotor_engine_proto-5.0.0/src/momotor/rpc/status/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1164 2024-04-16 07:54:15.000000 momotor_engine_proto-5.0.0/src/momotor/rpc/status/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 07:54:59.000000 momotor_engine_proto-5.0.0/src/momotor/rpc/task/
+-rw-rw-rw-   0 root         (0) root         (0)     1341 2024-04-16 07:54:15.000000 momotor_engine_proto-5.0.0/src/momotor/rpc/task/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 07:54:59.000000 momotor_engine_proto-5.0.0/src/momotor/rpc/tools/
+-rw-rw-rw-   0 root         (0) root         (0)      818 2024-04-16 07:54:15.000000 momotor_engine_proto-5.0.0/src/momotor/rpc/tools/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1388 2024-04-16 07:54:15.000000 momotor_engine_proto-5.0.0/src/momotor/rpc/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 07:54:59.000000 momotor_engine_proto-5.0.0/src/momotor/rpc/validate/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-16 07:54:15.000000 momotor_engine_proto-5.0.0/src/momotor/rpc/validate/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1817 2024-04-16 07:54:15.000000 momotor_engine_proto-5.0.0/src/momotor/rpc/validate/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1191 2024-04-16 07:54:15.000000 momotor_engine_proto-5.0.0/src/momotor/rpc/validate/query.py
+-rw-rw-rw-   0 root         (0) root         (0)     5014 2024-04-16 07:54:15.000000 momotor_engine_proto-5.0.0/src/momotor/rpc/validate/request.py
+-rw-rw-rw-   0 root         (0) root         (0)      656 2024-04-16 07:54:15.000000 momotor_engine_proto-5.0.0/src/momotor/rpc/validate/response.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 07:54:59.000000 momotor_engine_proto-5.0.0/src/momotor_engine_proto.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2862 2024-04-16 07:54:59.000000 momotor_engine_proto-5.0.0/src/momotor_engine_proto.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3115 2024-04-16 07:54:59.000000 momotor_engine_proto-5.0.0/src/momotor_engine_proto.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-16 07:54:59.000000 momotor_engine_proto-5.0.0/src/momotor_engine_proto.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      414 2024-04-16 07:54:59.000000 momotor_engine_proto-5.0.0/src/momotor_engine_proto.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-04-16 07:54:59.000000 momotor_engine_proto-5.0.0/src/momotor_engine_proto.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 07:54:59.000000 momotor_engine_proto-5.0.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      812 2024-04-16 07:54:15.000000 momotor_engine_proto-5.0.0/tests/proto_test_consts.py
+-rw-rw-rw-   0 root         (0) root         (0)     1451 2024-04-16 07:54:15.000000 momotor_engine_proto-5.0.0/tests/test_asset_hash.py
+-rw-rw-rw-   0 root         (0) root         (0)      807 2024-04-16 07:54:15.000000 momotor_engine_proto-5.0.0/tests/test_identity_hash.py
+-rw-rw-rw-   0 root         (0) root         (0)       37 2024-04-16 07:54:55.000000 momotor_engine_proto-5.0.0/version.toml
```

### Comparing `momotor-engine-proto-4.4.0rc3/README.md` & `momotor_engine_proto-5.0.0/README.md`

 * *Files identical despite different names*

### Comparing `momotor-engine-proto-4.4.0rc3/src/momotor/rpc/asset/remote.py` & `momotor_engine_proto-5.0.0/src/momotor/rpc/asset/remote.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,14 @@
+from __future__ import annotations
+
 import asyncio
+import collections.abc
 import pathlib
 import typing
 import zipfile
-
 from asyncio_extras import call_in_executor, open_async
 
 from momotor.rpc.asset.exceptions import AssetHashMismatchError, UnexpectedEndOfStream, AssetSizeMismatchError
 from momotor.rpc.asset.utils import get_file_multihash, get_file_hash, file_writer, file_reader
 from momotor.rpc.const import CHUNK_SIZE
 from momotor.rpc.exception import raise_message_exception
 from momotor.rpc.hash import decode as decode_hash, is_identity_code
@@ -23,15 +25,15 @@
 # Remote (clients and workers) side of asset up/downloading.
 # Counterpart is in server.py
 
 StubType = typing.Union[ClientStub, WorkerStub]
 
 
 @annotate_docstring(logger=logger)
-async def send_asset(stub: StubType, job_id: str, query: AssetQuery, path: typing.Union[str, pathlib.Path],
+async def send_asset(stub: StubType, job_id: str, query: AssetQuery, path: str | pathlib.Path,
                      server_info: ServerInfoResponse, *,
                      process_executor=None, timeout=None) -> None:
     """ Function for use by a client or worker to send an asset to the broker server
 
     Produces log messages on the ``{logger.name}`` logger.
 
     :param stub: The connected stub to the broker.
@@ -109,17 +111,17 @@
             try:
                 await stream.end()
             except Exception as exc:
                 await logger.warning(f"unable to end stream: {exc}")
 
 
 @annotate_docstring(logger=logger)
-async def receive_asset(stub: StubType, job_id: str, query: AssetQuery, path: typing.Union[str, pathlib.Path],
-                        exists: typing.Callable[[AssetData], typing.Awaitable[bool]] = None,
-                        process_executor=None, timeout=None) -> typing.Tuple[AssetData, bool]:
+async def receive_asset(stub: StubType, job_id: str, query: AssetQuery, path: str | pathlib.Path,
+                        exists: collections.abc.Callable[[AssetData], collections.abc.Awaitable[bool]] = None,
+                        process_executor=None, timeout=None) -> tuple[AssetData, bool]:
     """ Function for use by a client or worker to request and receive an asset from the broker.
 
     Produces log messages on the ``{logger.name}`` logger.
 
     :param stub: The connected stub to the broker.
     :param job_id: Id of the job
     :param query: Query for the asset
```

### Comparing `momotor-engine-proto-4.4.0rc3/src/momotor/rpc/asset/server.py` & `momotor_engine_proto-5.0.0/src/momotor/rpc/asset/server.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,25 @@
-import asyncio
-import typing
+from __future__ import annotations
 
+import asyncio
+import collections.abc
 from grpclib.server import Stream
 
 from momotor.rpc.asset.exceptions import UnexpectedEndOfStream
 from momotor.rpc.proto.asset_pb2 import AssetData, DownloadAssetResponse, UploadAssetResponse
 from momotor.rpc.validate.request import validate_upload_asset_request, validate_download_asset_request
 
+
 # logger = getAsyncLogger(__name__)
 
 
 # Server's side of asset up/downloading.
 # Counterpart is in remote.py
 
-async def download_asset_stream(data: AssetData, chunks: typing.Optional[typing.AsyncGenerator[bytes, None]],
+async def download_asset_stream(data: AssetData, chunks: collections.abc.AsyncGenerator[bytes, None] | None,
                                 stream: Stream, *, timeout=None):
     """ Function for use by the broker to handle an asset download stream from a client or worker.
 
     This communicates with a remote's :py:func:`momotor.rpc.asset.remote.receive_asset`
 
     :param data: An :py:class:`momotor.rpc.proto.asset_pb2.AssetData` object identifying the requested asset
     :param chunks: A generator producing chunks of the requested asset
@@ -37,15 +39,15 @@
         async for chunk in chunks:
             await asyncio.wait_for(
                 stream.send_message(DownloadAssetResponse(chunk=chunk)),
                 timeout=timeout
             )
 
 
-async def upload_asset_stream(creator: typing.AsyncGenerator[int, typing.Optional[bytes]], stream: Stream, *,
+async def upload_asset_stream(creator: collections.abc.AsyncGenerator[int, bytes | None], stream: Stream, *,
                               timeout=None):
     """ Function for use by the broker to handle an asset upload stream to a client or worker.
 
     This communicates with a remote's :py:func:`momotor.rpc.asset.remote.send_asset`
 
     :param creator: A generator that processes the chunks and writes them to a file or other storage,
                     and yields the number of bytes remaining.
```

### Comparing `momotor-engine-proto-4.4.0rc3/src/momotor/rpc/asset/utils.py` & `momotor_engine_proto-5.0.0/src/momotor/rpc/asset/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,19 @@
+from __future__ import annotations
+
 import asyncio
 import pathlib
-import typing
-
 from asyncio_extras import open_async
 
 from momotor.rpc.const import CHUNK_SIZE, MAX_IDENTITY_LENGTH
 from momotor.rpc.hash import new as new_hash, encode as encode_hash, encode_content
 from momotor.rpc.proto.auth_pb2 import ServerInfoResponse
 
 
-def get_file_multihash(path: typing.Union[str, pathlib.Path], server_info: ServerInfoResponse = None) \
-        -> typing.Tuple[bytes, bool]:
+def get_file_multihash(path: str | pathlib.Path, server_info: ServerInfoResponse = None) -> tuple[bytes, bool]:
     """ Get multihash value for file in `path`
 
     If the file is small enough to fit, the entire contents will be encoded in the multihash instead of an actual
     hash. A boolean in the result will indicate whether the result is a real hash or encoded content
 
     If a `server_info` object is provided, the resulting hash will be compatible with the server, otherwise
     the hash generated will use the capabilities of the local system.
@@ -49,15 +48,15 @@
                 break
 
             hash_func.update(chunk)
 
     return encode_hash(hash_func), False
 
 
-def get_file_hash(func_code: typing.Union[str, int], path: typing.Union[str, pathlib.Path]) -> bytes:
+def get_file_hash(func_code: str | int, path: str | pathlib.Path) -> bytes:
     """ Calculate a hash of the given file's content
 
     :param func_code: a multihash code (string or integer)
     :param path: path of the file to hash
     :return: unencoded hash digest generated by the hash function
     """
     hash_func = new_hash(func_code=func_code)
```

### Comparing `momotor-engine-proto-4.4.0rc3/src/momotor/rpc/auth/client.py` & `momotor_engine_proto-5.0.0/src/momotor/rpc/auth/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,27 @@
-import typing
+from __future__ import annotations
 
+import typing
 from grpclib.client import Channel, Stream
 from grpclib.config import Configuration
 from grpclib.const import Cardinality
 # noinspection PyProtectedMember
 from grpclib.metadata import Deadline, _MetadataLike, _Metadata
 # noinspection PyProtectedMember
 from grpclib.stream import _SendType, _RecvType
+from multidict import MultiDict
+
 from momotor.rpc.auth.utils import calculate_challenge_response
 from momotor.rpc.exception import raise_message_exception, RPCException
 from momotor.rpc.proto.auth_grpc import AuthStub
 from momotor.rpc.proto.auth_pb2 import AuthenticateRequest, AuthenticateResponse, Challenge
 from momotor.rpc.utils import setup_h2_logging
 from momotor.rpc.validate.response import validate_authenticate_response
 from momotor.shared.doc import annotate_docstring
 from momotor.shared.log import getAsyncLogger
-from multidict import MultiDict
 
 logger = getAsyncLogger(__package__)
 
 DEFAULT_PORT = 50051
 DEFAULT_SSL_PORT = 50052
 
 
@@ -36,20 +38,20 @@
         """ Returns `True` if an auth-token is set """
         return self.auth_token is not None
 
     def request(
             self,
             name: str,
             cardinality: Cardinality,
-            request_type: typing.Type[_SendType],
-            reply_type: typing.Type[_RecvType],
+            request_type: type[_SendType],
+            reply_type: type[_RecvType],
             *,
-            timeout: typing.Optional[float] = None,
-            deadline: typing.Optional[Deadline] = None,
-            metadata: typing.Optional[_MetadataLike] = None
+            timeout: float | None = None,
+            deadline: Deadline | None = None,
+            metadata: _MetadataLike | None = None
     ) -> Stream[_SendType, _RecvType]:
         """ Wrapper for :py:func:`grpclib.client.Channel.request`
         """
         auth_metadata = typing.cast(_Metadata, MultiDict(metadata or ()))
         if self.auth_token:
             auth_metadata['auth-token'] = self.auth_token
         if metadata is not None:
@@ -101,20 +103,20 @@
 
         channel.auth_token = response.authToken
 
     return channel
 
 
 @annotate_docstring(logger=logger)
-async def get_authenticated_channel(host: str, port: typing.Optional[int],
+async def get_authenticated_channel(host: str, port: int | None,
                                     api_key: str, api_secret: str, auth_token: str = None,
                                     *, ssl_context=None, loop=None, log_h2=False,
                                     keepalive_time=900,
                                     **channel_opts) \
-        -> typing.Tuple[AuthenticatingChannel, AuthStub]:
+        -> tuple[AuthenticatingChannel, AuthStub]:
     """ Connect to a broker and authenticate, possibly using an already existing token.
 
     Returns a tuple with
 
     * the authenticated channel
     * the auth stub
```

### Comparing `momotor-engine-proto-4.4.0rc3/src/momotor/rpc/auth/utils.py` & `momotor_engine_proto-5.0.0/src/momotor/rpc/auth/utils.py`

 * *Files identical despite different names*

### Comparing `momotor-engine-proto-4.4.0rc3/src/momotor/rpc/const.py` & `momotor_engine_proto-5.0.0/src/momotor/rpc/const.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #: Maximum length of a base58_ encoded hash supported by this version of the library
 MAX_HASH_LEN = MAX_HASH_LEN
 
 #: Maximum length of data that can be encoded in a hash of :py:data:`MAX_HASH_LEN` using identity encoding.
 #: base58_'s efficiency is 0.732, the overhead is the size of the varint encoded length + 1 for the code byte
 MAX_IDENTITY_LENGTH = MAX_IDENTITY_LENGTH
 
-#: List of supported hashing functions, ordered from most to least preferred
+#: List of supported hashing function codes, ordered from most to least preferred
 SUPPORTED_HASH_FUNCS = SUPPORTED_HASH_FUNCS
 
 #: The default port for non-SSL connections
 DEFAULT_PORT = DEFAULT_PORT
 
 #: The default port for SSL connections
 DEFAULT_SSL_PORT = DEFAULT_SSL_PORT
```

### Comparing `momotor-engine-proto-4.4.0rc3/src/momotor/rpc/exception/__init__.py` & `momotor_engine_proto-5.0.0/src/momotor/rpc/exception/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-import logging
-import typing
+from __future__ import annotations
 
+import logging
 from google.protobuf.message import Message
-
 # noinspection PyUnresolvedReferences
 # keep for backwards compatibility. These used to be exported in __all__
 from grpclib.exceptions import StreamTerminatedError, GRPCError, ProtocolError
 
 from momotor.rpc.asset.exceptions import UnexpectedEndOfStream
 from momotor.rpc.proto.exception_pb2 import Exception as ExceptionMessage, INVALID_EXCEPTION, FORMAT, AUTH, JOB, \
     ASSET, ASSET_NOT_FOUND
@@ -98,15 +97,15 @@
         AssetException,
         AssetNotFoundException,
     )
 }
 
 
 @annotate_docstring(logger=logger)
-def raise_message_exception(message: typing.Optional[Message], *, log_level=logging.DEBUG):
+def raise_message_exception(message: Message | None, *, log_level=logging.DEBUG):
     """ If the `message` has an exception field, convert it into an RPCException and raise it
 
     If `message` is `None`, raises :py:exc:`~momotor.rpc.asset.exceptions.UnexpectedEndOfStream`.
 
     If `message` has an `exception` field set, raises a subclass of :py:exc:`RPCException`
 
     Produces logging information on the ``{logger.name}`` logger
```

### Comparing `momotor-engine-proto-4.4.0rc3/src/momotor/rpc/hash/__init__.py` & `momotor_engine_proto-5.0.0/src/momotor/rpc/hash/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,26 @@
-import typing
+from __future__ import annotations
 
 import base58
+import collections.abc
 from multihash import coerce_code, encode as multihash_encode, Multihash, decode as multihash_decode
 
 from momotor.rpc.exception import AssetException
-
 from .const import MAX_HASH_LEN, MAX_IDENTITY_LENGTH
 from .funcs import get_algorithm_by_code, get_code_by_hash_obj, SUPPORTED_HASH_FUNCS
 from .identity import IdentityHash
 
 __all__ = ['new', 'encode', 'encode_content', 'decode', 'is_identity_code', 'is_identity']
 
 ID_HASH_CODE = coerce_code('id')  # deprecated, use is_identity_code()
 
 
-def new(content: typing.Union[bytes, memoryview] = None,
-        *, supported_funcs: typing.Iterable[int] = None, func_code: typing.Union[int, str] = SUPPORTED_HASH_FUNCS[0]):
+def new(content: bytes | memoryview | None = None,
+        *, supported_funcs: collections.abc.Iterable[int] | None = None,
+        func_code: int | str = SUPPORTED_HASH_FUNCS[0]):
     """ Construct a new hash object for best matching algorithm, like hashlib.new()
 
     :param content: Initial content to add to hash
     :param supported_funcs: List of multihash function codes to select the best hash from
     :param func_code: Multihash function code to use, only used if `supported_funcs` is not provided.
     Defaults to SUPPORTED_HASH_FUNCS[0]
     :return: the selected hash function
@@ -54,15 +55,15 @@
 
     if len(encoded) > MAX_HASH_LEN:
         raise ValueError("Hash value too long")
 
     return encoded
 
 
-def encode_content(content: typing.Union[bytes, memoryview], *, use_identity=None) -> bytes:
+def encode_content(content: bytes | memoryview, *, use_identity=None) -> bytes:
     """ Return encoded multihash of content with the preferred algorithm in the required encoding
 
     :param content: content to be encoded
     :param use_identity: True to force use of identity encoding, False to force use of hashing. None (default) to
     use identity encoding automatically if content length fits
     :return: base58 encoded multihash value for content
     """
@@ -73,24 +74,24 @@
 
     if use_identity:
         return encode(IdentityHash(content))
     else:
         return encode(new(content))
 
 
-def _decode_hash(hash_value: typing.Union[bytes, memoryview]) -> Multihash:
+def _decode_hash(hash_value: bytes | memoryview) -> Multihash:
     try:
         b = base58.b58decode(bytes(hash_value))
     except ValueError:
         raise ValueError("illegal hash value")
 
     return multihash_decode(b)
 
 
-def decode(hash_value: typing.Union[bytes, memoryview]) -> typing.Tuple[bytes, int]:
+def decode(hash_value: bytes | memoryview) -> tuple[bytes, int]:
     """ Decode multihash value in required encoding and return the digest or content, and the hash function code
 
     :param hash_value: base58 encoded multihash value
     :return: tuple containing decoded hash digest and multihash function code
     :raises: AssetException if the hash is not a valid encoded multihash or uses an unsupported hashing function
     """
     try:
@@ -108,15 +109,15 @@
 _ID_HASH_CODE = coerce_code('id')
 
 
 def is_identity_code(hash_code: int):
     return hash_code == _ID_HASH_CODE
 
 
-def is_identity(hash_value: typing.Union[bytes, memoryview]) -> bool:
+def is_identity(hash_value: bytes | memoryview) -> bool:
     """ Return True if hash_value encodes identity encoded content
 
     :param hash_value: base58 encoded multihash value
     :return: True if hash_value contains identity encoded content
     """
     try:
         return is_identity_code(_decode_hash(hash_value).code)
```

### Comparing `momotor-engine-proto-4.4.0rc3/src/momotor/rpc/hash/funcs.py` & `momotor_engine_proto-5.0.0/src/momotor/rpc/hash/funcs.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-import hashlib
-import typing
+from __future__ import annotations
 
+import hashlib
 from multihash import coerce_code
 
 from .identity import IdentityHash
 
 _MH_NAME_TO_ALGO_NAME = {
     'sha1': 'sha1',
     'sha2-256': 'sha256',
@@ -26,15 +26,15 @@
     coerce_code(name): algo for name, algo in _MH_NAME_TO_ALGO.items()
 }
 _HASH_NAME_TO_CODE = {
     func().name: coerce_code(name) for name, func in _MH_NAME_TO_ALGO.items() if func
 }
 
 
-def get_algorithm_by_code(code: typing.Union[str, int]) -> object:
+def get_algorithm_by_code(code: str | int) -> object:
     """ Get a :pep:`452` compatible hashing object by its `multihash code`_ or name
 
     :param code: `multihash code`_ or name
     :return: :pep:`452` compatible hashing object
     """
     return _MH_CODE_TO_ALGO[coerce_code(code)]
```

### Comparing `momotor-engine-proto-4.4.0rc3/src/momotor/rpc/hash/identity.py` & `momotor_engine_proto-5.0.0/src/momotor/rpc/hash/identity.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 
 The identity hash stores the literal content as a hash:
 
 >>> IdentityHash(b'any random data').digest() == b'any random data'
 True
 
 """
-import typing
+from __future__ import annotations
 
 
 class IdentityHash(object):
     #: identifier for the hashing function
     name = 'identity'
 
-    def __init__(self, data: typing.Union[bytes, memoryview] = None):
+    def __init__(self, data: bytes | memoryview | None = None):
         self._digest = b'' if data is None else bytes(data)
 
     def update(self, data: bytes):
         """ Extend the hash with `data`
 
         :param data: data to concatenate to the existing data
         """
@@ -50,15 +50,15 @@
         return len(self._digest)
 
     @property
     def block_size(self):
         return NotImplemented
 
 
-def new(data: typing.Union[bytes, memoryview] = None) -> IdentityHash:
+def new(data: bytes | memoryview | None = None) -> IdentityHash:
     """ Create a identity hash object
 
     :param data: initial data for the hash
     :return: the identity hash object
     """
     return IdentityHash(data)
```

### Comparing `momotor-engine-proto-4.4.0rc3/src/momotor/rpc/proto/auth_grpc.py` & `momotor_engine_proto-5.0.0/src/momotor/rpc/proto/auth_grpc.py`

 * *Files identical despite different names*

### Comparing `momotor-engine-proto-4.4.0rc3/src/momotor/rpc/proto/client_grpc.py` & `momotor_engine_proto-5.0.0/src/momotor/rpc/proto/client_grpc.py`

 * *Files identical despite different names*

### Comparing `momotor-engine-proto-4.4.0rc3/src/momotor/rpc/proto/worker_grpc.py` & `momotor_engine_proto-5.0.0/src/momotor/rpc/proto/worker_grpc.py`

 * *Files identical despite different names*

### Comparing `momotor-engine-proto-4.4.0rc3/src/momotor/rpc/resources/__init__.py` & `momotor_engine_proto-5.0.0/src/momotor/rpc/resources/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-import typing
+from __future__ import annotations
 
 from momotor.rpc.proto.resource_pb2 import Resource as ResourceMessage
 from momotor.shared.resources import Resources
 
 
-def resources_to_message(resources: Resources) -> typing.Optional[typing.List[ResourceMessage]]:
+def resources_to_message(resources: Resources) -> list[ResourceMessage] | None:
     """ Convert a :py:class:`~momotor.shared.resources.Resources` object into
     a list of :py:class:`~momotor.rpc.proto.resource_pb2.Resource` messages
 
     :param resources: The resources
     :return: The message
     """
     return [
         ResourceMessage(name=name, value=value) for name, value in resources.as_str_tuples()
     ] if resources else None
 
 
-def message_to_resources(resources: typing.Optional[typing.List[ResourceMessage]]) -> Resources:
+def message_to_resources(resources: list[ResourceMessage] | None) -> Resources:
     """ Convert a list of :py:class:`~momotor.rpc.proto.resource_pb2.Resource` messages into
     a :py:class:`~momotor.shared.resources.Resources`
 
     :param resources: The resource messages
     :return: Resources object for the messages
     """
     return Resources.union(*(
```

### Comparing `momotor-engine-proto-4.4.0rc3/src/momotor/rpc/shared/__init__.py` & `momotor_engine_proto-5.0.0/src/momotor/rpc/shared/__init__.py`

 * *Files identical despite different names*

### Comparing `momotor-engine-proto-4.4.0rc3/src/momotor/rpc/status/client.py` & `momotor_engine_proto-5.0.0/src/momotor/rpc/status/client.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 import asyncio
-import typing
-
+import collections.abc
 from google.protobuf.empty_pb2 import Empty
 
 from momotor.rpc.exception import raise_message_exception
 from momotor.rpc.proto.client_grpc import ClientStub
 from momotor.rpc.proto.job_pb2 import JobStatusStream
 
 
 async def multi_job_status_stream(stub: ClientStub, *, connect_timeout: float = None, status_timeout: float = None) \
-        -> typing.AsyncIterable[JobStatusStream]:
+        -> collections.abc.AsyncIterable[JobStatusStream]:
     """ Async generator that connects to the :py:func:`~momotor.rpc.proto.client_grpc.ClientBase.multiJobStatusStream`
     client endpoint and yields the :py:class:`~momotor.rpc.proto.job_pb2.JobStatusStream` status messages
 
     :param stub: The connected client stub
     :param connect_timeout: Connection timeout
     :param status_timeout: Status message timeout
     """
```

### Comparing `momotor-engine-proto-4.4.0rc3/src/momotor/rpc/task/__init__.py` & `momotor_engine_proto-5.0.0/src/momotor/rpc/task/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,15 @@
-import typing
+from __future__ import annotations
+
+import collections.abc
 
 from momotor.rpc.proto.task_pb2 import TaskId
 
 
-def get_dotted_task_number(task_num: typing.Optional[typing.Sequence[int]]) -> typing.Optional[str]:
+def get_dotted_task_number(task_num: collections.abc.Sequence[int] | None) -> str | None:
     """ Convert a task-number list into a dotted task-number.
     If task_num is empty or None, returns None
 
     >>> get_dotted_task_number(None)
 
     >>> get_dotted_task_number([])
```

### Comparing `momotor-engine-proto-4.4.0rc3/src/momotor/rpc/tools/__init__.py` & `momotor_engine_proto-5.0.0/src/momotor/rpc/tools/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,25 @@
+from __future__ import annotations
+
+import collections.abc
 import typing
 
 from momotor.rpc.proto.tool_pb2 import ToolSet as ToolSetMessage
 
 TN = typing.TypeVar('TN')
 
 
-def toolsets_to_message(toolsets: typing.Iterable[typing.AbstractSet[str]]) -> typing.Iterable[ToolSetMessage]:
+def toolsets_to_message(toolsets: collections.abc.Iterable[set[str]]) -> collections.abc.Iterable[ToolSetMessage]:
     """ Convert an iterable of ToolName objects into a sequence of Tool messages
     """
     for toolset in toolsets:
         yield ToolSetMessage(
             tool=[str(tool) for tool in toolset]
         )
 
 
-def message_to_toolsets(toolset_message: typing.Optional[typing.Sequence[ToolSetMessage]]) \
-        -> typing.Iterable[typing.FrozenSet[str]]:
-
+def message_to_toolsets(toolset_message: collections.abc.Sequence[ToolSetMessage] | None) \
+        -> collections.abc.Iterable[frozenset[str]]:
     """ Convert a sequence of Tool messages back into an iterable of tool sets """
     if toolset_message:
         for msg in toolset_message:
             yield frozenset(msg.tool)
```

### Comparing `momotor-engine-proto-4.4.0rc3/src/momotor/rpc/utils.py` & `momotor_engine_proto-5.0.0/src/momotor/rpc/utils.py`

 * *Files identical despite different names*

### Comparing `momotor-engine-proto-4.4.0rc3/src/momotor/rpc/validate/base.py` & `momotor_engine_proto-5.0.0/src/momotor/rpc/validate/base.py`

 * *Files identical despite different names*

### Comparing `momotor-engine-proto-4.4.0rc3/src/momotor/rpc/validate/query.py` & `momotor_engine_proto-5.0.0/src/momotor/rpc/validate/query.py`

 * *Files identical despite different names*

### Comparing `momotor-engine-proto-4.4.0rc3/src/momotor/rpc/validate/request.py` & `momotor_engine_proto-5.0.0/src/momotor/rpc/validate/request.py`

 * *Files identical despite different names*

### Comparing `momotor-engine-proto-4.4.0rc3/src/momotor/rpc/validate/response.py` & `momotor_engine_proto-5.0.0/src/momotor/rpc/validate/response.py`

 * *Files identical despite different names*

