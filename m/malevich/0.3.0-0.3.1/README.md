# Comparing `tmp/malevich-0.3.0.tar.gz` & `tmp/malevich-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "malevich-0.3.0.tar", last modified: Fri Apr 12 11:04:29 2024, max compression
+gzip compressed data, was "malevich-0.3.1.tar", last modified: Tue Apr 16 09:31:26 2024, max compression
```

## Comparing `malevich-0.3.0.tar` & `malevich-0.3.1.tar`

### file list

```diff
@@ -1,218 +1,221 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:04:29.120376 malevich-0.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:04:29.080377 malevich-0.3.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:04:29.088377 malevich-0.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-12 11:04:16.000000 malevich-0.3.0/.github/workflows/docs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-12 11:04:16.000000 malevich-0.3.0/.github/workflows/pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-04-12 11:04:16.000000 malevich-0.3.0/.github/workflows/pytest.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-12 11:04:16.000000 malevich-0.3.0/.github/workflows/ruff.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-12 11:04:16.000000 malevich-0.3.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-12 11:04:16.000000 malevich-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-12 11:04:16.000000 malevich-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-12 11:04:29.120376 malevich-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5686 2024-04-12 11:04:16.000000 malevich-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-12 11:04:26.000000 malevich-0.3.0/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:04:29.092377 malevich-0.3.0/malevich/
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:04:29.092377 malevich-0.3.0/malevich/_autoflow/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/_autoflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/_autoflow/flow.py
--rw-r--r--   0 runner    (1001) docker     (127)     2824 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/_autoflow/function.py
--rw-r--r--   0 runner    (1001) docker     (127)     4067 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/_autoflow/tracer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5562 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/_autoflow/tree.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:04:29.096377 malevich-0.3.0/malevich/_cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4803 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/_cli/ci.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:04:29.096377 malevich-0.3.0/malevich/_cli/core/
--rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/_cli/core/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     3500 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/_cli/core/assets.py
--rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/_cli/core/endpoints.py
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/_cli/core/limits.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:04:29.096377 malevich-0.3.0/malevich/_cli/dev/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/_cli/dev/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16729 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/_cli/dev/dev.py
--rw-r--r--   0 runner    (1001) docker     (127)     2655 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/_cli/flow.py
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/_cli/init.py
--rw-r--r--   0 runner    (1001) docker     (127)     4924 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/_cli/install.py
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/_cli/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     3841 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/_cli/manifest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:04:29.096377 malevich-0.3.0/malevich/_cli/misc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/_cli/misc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/_cli/misc/make.py
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/_cli/misc/manifest_to_env.py
--rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/_cli/new.py
--rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/_cli/prefs.py
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/_cli/remove.py
--rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/_cli/restore.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:04:29.096377 malevich-0.3.0/malevich/_cli/space/
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/_cli/space/init.py
--rw-r--r--   0 runner    (1001) docker     (127)     2961 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/_cli/space/login.py
--rw-r--r--   0 runner    (1001) docker     (127)    10399 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/_cli/use.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:04:29.096377 malevich-0.3.0/malevich/_core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7911 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/_core/ops.py
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/_core/scan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:04:29.096377 malevich-0.3.0/malevich/_db/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/_db/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:04:29.096377 malevich-0.3.0/malevich/_db/functions/
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/_db/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/_db/functions/credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/_db/functions/get_db.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/_db/local.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:04:29.100377 malevich-0.3.0/malevich/_db/schema/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/_db/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/_db/schema/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/_db/schema/core_creds.py
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/_db/schema/creds.py
--rw-r--r--   0 runner    (1001) docker     (127)     4149 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/_deploy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:04:29.100377 malevich-0.3.0/malevich/_export/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/_export/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5597 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/_export/space_flow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:04:29.100377 malevich-0.3.0/malevich/_meta/
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/_meta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4186 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/_meta/asset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/_meta/collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/_meta/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/_meta/decor.py
--rw-r--r--   0 runner    (1001) docker     (127)     7359 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/_meta/flow.py
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/_meta/run.py
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/_meta/table.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:04:29.100377 malevich-0.3.0/malevich/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/_templates/Dockerfile.app
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/_templates/README.app.md
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/_templates/flow.py.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/_templates/processor.py.txt
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/_templates/space.yaml.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:04:29.104377 malevich-0.3.0/malevich/_utility/
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/_utility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/_utility/_try.py
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/_utility/args.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:04:29.104377 malevich-0.3.0/malevich/_utility/cache/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/_utility/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6620 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/_utility/cache/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:04:29.104377 malevich-0.3.0/malevich/_utility/ci/
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/_utility/ci/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/_utility/ci/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3273 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/_utility/ci/functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6677 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/_utility/ci/github.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:04:29.104377 malevich-0.3.0/malevich/_utility/ci/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/_utility/ci/templates/malevich-ci-manual.yml
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/_utility/ci/templates/malevich-ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      946 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/_utility/dicts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:04:29.104377 malevich-0.3.0/malevich/_utility/git/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/_utility/git/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/_utility/git/clone.py
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/_utility/host.py
--rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/_utility/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     3535 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/_utility/package.py
--rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/_utility/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     4929 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/_utility/scan.py
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/_utility/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/_utility/singleton.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:04:29.104377 malevich-0.3.0/malevich/_utility/space/
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/_utility/space/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/_utility/space/get_core_creds.py
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/_utility/space/space.py
--rw-r--r--   0 runner    (1001) docker     (127)    13580 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/_utility/stub.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:04:29.108377 malevich-0.3.0/malevich/_utility/summary/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/_utility/summary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/_utility/summary/abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/_utility/summary/time.py
--rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/_utility/tree.py
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/annotations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3971 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/core_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/help.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:04:29.108377 malevich-0.3.0/malevich/install/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/install/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5896 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/install/image.py
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/install/installer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2462 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/install/iso.py
--rw-r--r--   0 runner    (1001) docker     (127)     5287 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/install/space.py
--rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/install/stub.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:04:29.108377 malevich-0.3.0/malevich/interpreter/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/interpreter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9998 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/interpreter/abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)    16801 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/interpreter/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    28658 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/interpreter/space.py
--rw-r--r--   0 runner    (1001) docker     (127)    11113 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/manifest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:04:29.112377 malevich-0.3.0/malevich/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/models/actions.py
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/models/argument.py
--rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/models/collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/models/dependency.py
--rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/models/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/models/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/models/flow_function.py
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/models/in_app_core_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/models/injections.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:04:29.112377 malevich-0.3.0/malevich/models/installers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/models/installers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/models/installers/compat.py
--rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/models/installers/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/models/installers/space.py
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/models/manifest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:04:29.112377 malevich-0.3.0/malevich/models/nodes/
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/models/nodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/models/nodes/asset.py
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/models/nodes/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/models/nodes/collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/models/nodes/operation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2744 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/models/nodes/tree.py
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/models/platform.py
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/models/preferences.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:04:29.112377 malevich-0.3.0/malevich/models/registry/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/models/registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/models/registry/core_entry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:04:29.112377 malevich-0.3.0/malevich/models/results/
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/models/results/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/models/results/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:04:29.112377 malevich-0.3.0/malevich/models/results/core/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/models/results/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16796 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/models/results/core/result.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:04:29.112377 malevich-0.3.0/malevich/models/results/space/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/models/results/space/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/models/results/space/collection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:04:29.116376 malevich-0.3.0/malevich/models/state/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/models/state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/models/state/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     3910 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/models/state/space.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:04:29.116376 malevich-0.3.0/malevich/models/task/
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/models/task/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4994 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/models/task/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:04:29.116376 malevich-0.3.0/malevich/models/task/interpreted/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/models/task/interpreted/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23031 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/models/task/interpreted/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    10907 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/models/task/interpreted/space.py
--rw-r--r--   0 runner    (1001) docker     (127)    12515 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/models/task/promised.py
--rw-r--r--   0 runner    (1001) docker     (127)     8424 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/models/task.py
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/models/type_annotations.py
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/models/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/models/verdict.py
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/path.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:04:29.116376 malevich-0.3.0/malevich/runners/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/runners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/runners/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:04:29.116376 malevich-0.3.0/malevich/square/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/square/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/square/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     9148 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/square/df.py
--rw-r--r--   0 runner    (1001) docker     (127)     3707 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/square/jls.py
--rw-r--r--   0 runner    (1001) docker     (127)    42188 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/square/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:04:29.116376 malevich-0.3.0/malevich/testing/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4719 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/testing/env.py
--rw-r--r--   0 runner    (1001) docker     (127)     5102 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/testing/suite.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 11:04:16.000000 malevich-0.3.0/malevich/testing/testcase.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:04:29.116376 malevich-0.3.0/malevich.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-12 11:04:29.000000 malevich-0.3.0/malevich.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5218 2024-04-12 11:04:29.000000 malevich-0.3.0/malevich.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 11:04:29.000000 malevich-0.3.0/malevich.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-12 11:04:29.000000 malevich-0.3.0/malevich.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-12 11:04:29.000000 malevich-0.3.0/malevich.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-12 11:04:29.000000 malevich-0.3.0/malevich.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 11:04:16.000000 malevich-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-12 11:04:16.000000 malevich-0.3.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 11:04:29.120376 malevich-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-12 11:04:16.000000 malevich-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:31:26.444931 malevich-0.3.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:31:26.408931 malevich-0.3.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:31:26.416931 malevich-0.3.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-16 09:31:16.000000 malevich-0.3.1/.github/workflows/docs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-16 09:31:16.000000 malevich-0.3.1/.github/workflows/pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-04-16 09:31:16.000000 malevich-0.3.1/.github/workflows/pytest.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-16 09:31:16.000000 malevich-0.3.1/.github/workflows/ruff.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-16 09:31:16.000000 malevich-0.3.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-16 09:31:16.000000 malevich-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-16 09:31:16.000000 malevich-0.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-16 09:31:26.444931 malevich-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5686 2024-04-16 09:31:16.000000 malevich-0.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-16 09:31:24.000000 malevich-0.3.1/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:31:26.420931 malevich-0.3.1/malevich/
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:31:26.420931 malevich-0.3.1/malevich/_autoflow/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/_autoflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/_autoflow/flow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2824 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/_autoflow/function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4067 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/_autoflow/tracer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5562 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/_autoflow/tree.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:31:26.424931 malevich-0.3.1/malevich/_cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4803 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/_cli/ci.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:31:26.424931 malevich-0.3.1/malevich/_cli/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/_cli/core/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3500 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/_cli/core/assets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/_cli/core/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/_cli/core/limits.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:31:26.424931 malevich-0.3.1/malevich/_cli/dev/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/_cli/dev/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16729 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/_cli/dev/dev.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2655 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/_cli/flow.py
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/_cli/init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4924 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/_cli/install.py
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/_cli/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3841 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/_cli/manifest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:31:26.424931 malevich-0.3.1/malevich/_cli/misc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/_cli/misc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/_cli/misc/make.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/_cli/misc/manifest_to_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/_cli/new.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/_cli/prefs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/_cli/remove.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/_cli/restore.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:31:26.424931 malevich-0.3.1/malevich/_cli/space/
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/_cli/space/init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2961 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/_cli/space/login.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10399 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/_cli/use.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:31:26.424931 malevich-0.3.1/malevich/_core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7911 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/_core/ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/_core/scan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:31:26.424931 malevich-0.3.1/malevich/_db/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/_db/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:31:26.424931 malevich-0.3.1/malevich/_db/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/_db/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/_db/functions/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/_db/functions/get_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/_db/local.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:31:26.428931 malevich-0.3.1/malevich/_db/schema/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/_db/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/_db/schema/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/_db/schema/core_creds.py
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/_db/schema/creds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4239 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/_deploy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:31:26.428931 malevich-0.3.1/malevich/_export/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/_export/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5597 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/_export/space_flow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:31:26.428931 malevich-0.3.1/malevich/_meta/
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/_meta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4186 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/_meta/asset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/_meta/collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/_meta/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3146 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/_meta/decor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7359 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/_meta/flow.py
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/_meta/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/_meta/table.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:31:26.428931 malevich-0.3.1/malevich/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/_templates/Dockerfile.app
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/_templates/README.app.md
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/_templates/flow.py.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/_templates/processor.py.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/_templates/space.yaml.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:31:26.432932 malevich-0.3.1/malevich/_utility/
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/_utility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/_utility/_try.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/_utility/args.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:31:26.432932 malevich-0.3.1/malevich/_utility/cache/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/_utility/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6620 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/_utility/cache/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:31:26.432932 malevich-0.3.1/malevich/_utility/ci/
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/_utility/ci/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/_utility/ci/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3273 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/_utility/ci/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6677 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/_utility/ci/github.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:31:26.432932 malevich-0.3.1/malevich/_utility/ci/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/_utility/ci/templates/malevich-ci-manual.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/_utility/ci/templates/malevich-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/_utility/dicts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:31:26.432932 malevich-0.3.1/malevich/_utility/git/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/_utility/git/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/_utility/git/clone.py
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/_utility/host.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/_utility/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3535 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/_utility/package.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/_utility/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4929 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/_utility/scan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/_utility/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/_utility/singleton.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:31:26.436931 malevich-0.3.1/malevich/_utility/space/
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/_utility/space/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/_utility/space/get_core_creds.py
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/_utility/space/space.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13580 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/_utility/stub.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:31:26.436931 malevich-0.3.1/malevich/_utility/summary/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/_utility/summary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/_utility/summary/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/_utility/summary/time.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/_utility/tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/annotations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3995 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/core_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/help.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:31:26.436931 malevich-0.3.1/malevich/install/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/install/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5896 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/install/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/install/installer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2462 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/install/iso.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5287 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/install/space.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/install/stub.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:31:26.436931 malevich-0.3.1/malevich/interpreter/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/interpreter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9998 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/interpreter/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16801 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/interpreter/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28658 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/interpreter/space.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11113 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/manifest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:31:26.440931 malevich-0.3.1/malevich/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/models/actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/models/argument.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/models/collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/models/dependency.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/models/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/models/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/models/flow_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/models/in_app_core_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/models/injections.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:31:26.440931 malevich-0.3.1/malevich/models/installers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/models/installers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/models/installers/compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/models/installers/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/models/installers/space.py
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/models/manifest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:31:26.440931 malevich-0.3.1/malevich/models/nodes/
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/models/nodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/models/nodes/asset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/models/nodes/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/models/nodes/collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/models/nodes/operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2744 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/models/nodes/tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/models/platform.py
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/models/preferences.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:31:26.440931 malevich-0.3.1/malevich/models/registry/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/models/registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/models/registry/core_entry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:31:26.440931 malevich-0.3.1/malevich/models/results/
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/models/results/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/models/results/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:31:26.440931 malevich-0.3.1/malevich/models/results/core/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/models/results/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16796 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/models/results/core/result.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:31:26.440931 malevich-0.3.1/malevich/models/results/space/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/models/results/space/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/models/results/space/collection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:31:26.444931 malevich-0.3.1/malevich/models/state/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/models/state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/models/state/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3910 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/models/state/space.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:31:26.444931 malevich-0.3.1/malevich/models/task/
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/models/task/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4994 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/models/task/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:31:26.444931 malevich-0.3.1/malevich/models/task/interpreted/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/models/task/interpreted/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23059 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/models/task/interpreted/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10907 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/models/task/interpreted/space.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12949 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/models/task/promised.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8424 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/models/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/models/type_annotations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/models/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/models/verdict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/path.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:31:26.444931 malevich-0.3.1/malevich/runners/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/runners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/runners/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:31:26.444931 malevich-0.3.1/malevich/square/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/square/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/square/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9148 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/square/df.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3701 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/square/jls.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42188 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/square/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:31:26.444931 malevich-0.3.1/malevich/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/testing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:31:26.444931 malevich-0.3.1/malevich/testing/env/
+-rw-r--r--   0 runner    (1001) docker     (127)     5096 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/testing/env/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4719 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/testing/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/testing/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5102 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/testing/suite.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 09:31:16.000000 malevich-0.3.1/malevich/testing/testcase.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:31:26.444931 malevich-0.3.1/malevich.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-16 09:31:26.000000 malevich-0.3.1/malevich.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5463 2024-04-16 09:31:26.000000 malevich-0.3.1/malevich.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 09:31:26.000000 malevich-0.3.1/malevich.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-16 09:31:26.000000 malevich-0.3.1/malevich.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-16 09:31:26.000000 malevich-0.3.1/malevich.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-16 09:31:26.000000 malevich-0.3.1/malevich.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 09:31:16.000000 malevich-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-16 09:31:16.000000 malevich-0.3.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 09:31:26.444931 malevich-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-16 09:31:16.000000 malevich-0.3.1/setup.py
```

### Comparing `malevich-0.3.0/.github/workflows/docs.yaml` & `malevich-0.3.1/.github/workflows/docs.yaml`

 * *Files 25% similar despite different names*

```diff
@@ -18,14 +18,17 @@
           python-version: '3.11'
       - name: Install dependencies
         run: |
           pip install -r requirements.dev.txt
       - name: Sphinx build
         run: |
           sphinx-build docs build-docs
+      - name: Add CNAME
+        run: |
+          echo "docs.malevich.ai" > build-docs/CNAME
       - name: Deploy to GitHub Pages
         uses: peaceiris/actions-gh-pages@v3
         if: ${{ github.event_name == 'push' && github.ref == 'refs/heads/docs' }}
         with:
           publish_branch: gh-pages
           github_token: ${{ secrets.DOCS_GITHUB_TOKEN }}
           publish_dir: build-docs
```

### Comparing `malevich-0.3.0/.github/workflows/pypi.yaml` & `malevich-0.3.1/.github/workflows/pypi.yaml`

 * *Files identical despite different names*

### Comparing `malevich-0.3.0/.github/workflows/pytest.yaml` & `malevich-0.3.1/.github/workflows/pytest.yaml`

 * *Files identical despite different names*

### Comparing `malevich-0.3.0/LICENSE` & `malevich-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `malevich-0.3.0/PKG-INFO` & `malevich-0.3.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: malevich
-Version: 0.3.0
+Version: 0.3.1
 Summary: ('A user-friendly interface to communicate with Malevich AI (malevich.ai)',)
 License-File: LICENSE
 Requires-Dist: typer[all]>=0.9.0
 Requires-Dist: pydantic>=2.0.0
 Requires-Dist: malevich-coretools>=0.3.11
 Requires-Dist: malevich-space>=0.4.18
 Requires-Dist: pandas
```

### Comparing `malevich-0.3.0/README.md` & `malevich-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `malevich-0.3.0/malevich/__init__.py` & `malevich-0.3.1/malevich/__init__.py`

 * *Files identical despite different names*

### Comparing `malevich-0.3.0/malevich/_autoflow/flow.py` & `malevich-0.3.1/malevich/_autoflow/flow.py`

 * *Files identical despite different names*

### Comparing `malevich-0.3.0/malevich/_autoflow/function.py` & `malevich-0.3.1/malevich/_autoflow/function.py`

 * *Files identical despite different names*

### Comparing `malevich-0.3.0/malevich/_autoflow/tracer.py` & `malevich-0.3.1/malevich/_autoflow/tracer.py`

 * *Files identical despite different names*

### Comparing `malevich-0.3.0/malevich/_autoflow/tree.py` & `malevich-0.3.1/malevich/_autoflow/tree.py`

 * *Files identical despite different names*

### Comparing `malevich-0.3.0/malevich/_cli/ci.py` & `malevich-0.3.1/malevich/_cli/ci.py`

 * *Files identical despite different names*

### Comparing `malevich-0.3.0/malevich/_cli/core/app.py` & `malevich-0.3.1/malevich/_cli/core/app.py`

 * *Files identical despite different names*

### Comparing `malevich-0.3.0/malevich/_cli/core/assets.py` & `malevich-0.3.1/malevich/_cli/core/assets.py`

 * *Files identical despite different names*

### Comparing `malevich-0.3.0/malevich/_cli/core/endpoints.py` & `malevich-0.3.1/malevich/_cli/core/endpoints.py`

 * *Files identical despite different names*

### Comparing `malevich-0.3.0/malevich/_cli/core/limits.py` & `malevich-0.3.1/malevich/_cli/core/limits.py`

 * *Files identical despite different names*

### Comparing `malevich-0.3.0/malevich/_cli/dev/dev.py` & `malevich-0.3.1/malevich/_cli/dev/dev.py`

 * *Files identical despite different names*

### Comparing `malevich-0.3.0/malevich/_cli/flow.py` & `malevich-0.3.1/malevich/_cli/flow.py`

 * *Files identical despite different names*

### Comparing `malevich-0.3.0/malevich/_cli/init.py` & `malevich-0.3.1/malevich/_cli/init.py`

 * *Files identical despite different names*

### Comparing `malevich-0.3.0/malevich/_cli/install.py` & `malevich-0.3.1/malevich/_cli/install.py`

 * *Files identical despite different names*

### Comparing `malevich-0.3.0/malevich/_cli/list.py` & `malevich-0.3.1/malevich/_cli/list.py`

 * *Files identical despite different names*

### Comparing `malevich-0.3.0/malevich/_cli/manifest.py` & `malevich-0.3.1/malevich/_cli/manifest.py`

 * *Files identical despite different names*

### Comparing `malevich-0.3.0/malevich/_cli/misc/make.py` & `malevich-0.3.1/malevich/_cli/misc/make.py`

 * *Files identical despite different names*

### Comparing `malevich-0.3.0/malevich/_cli/misc/manifest_to_env.py` & `malevich-0.3.1/malevich/_cli/misc/manifest_to_env.py`

 * *Files identical despite different names*

### Comparing `malevich-0.3.0/malevich/_cli/new.py` & `malevich-0.3.1/malevich/_cli/new.py`

 * *Files identical despite different names*

### Comparing `malevich-0.3.0/malevich/_cli/prefs.py` & `malevich-0.3.1/malevich/_cli/prefs.py`

 * *Files identical despite different names*

### Comparing `malevich-0.3.0/malevich/_cli/remove.py` & `malevich-0.3.1/malevich/_cli/remove.py`

 * *Files identical despite different names*

### Comparing `malevich-0.3.0/malevich/_cli/restore.py` & `malevich-0.3.1/malevich/_cli/restore.py`

 * *Files identical despite different names*

### Comparing `malevich-0.3.0/malevich/_cli/space/init.py` & `malevich-0.3.1/malevich/_cli/space/init.py`

 * *Files identical despite different names*

### Comparing `malevich-0.3.0/malevich/_cli/space/login.py` & `malevich-0.3.1/malevich/_cli/space/login.py`

 * *Files identical despite different names*

### Comparing `malevich-0.3.0/malevich/_cli/use.py` & `malevich-0.3.1/malevich/_cli/use.py`

 * *Files identical despite different names*

### Comparing `malevich-0.3.0/malevich/_core/ops.py` & `malevich-0.3.1/malevich/_core/ops.py`

 * *Files identical despite different names*

### Comparing `malevich-0.3.0/malevich/_core/scan.py` & `malevich-0.3.1/malevich/_core/scan.py`

 * *Files identical despite different names*

### Comparing `malevich-0.3.0/malevich/_db/functions/credentials.py` & `malevich-0.3.1/malevich/_db/functions/credentials.py`

 * *Files identical despite different names*

### Comparing `malevich-0.3.0/malevich/_db/functions/get_db.py` & `malevich-0.3.1/malevich/_db/functions/get_db.py`

 * *Files identical despite different names*

### Comparing `malevich-0.3.0/malevich/_db/schema/creds.py` & `malevich-0.3.1/malevich/_db/schema/creds.py`

 * *Files identical despite different names*

### Comparing `malevich-0.3.0/malevich/_deploy.py` & `malevich-0.3.1/malevich/_deploy.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,27 +67,28 @@
             core_auth=(user, access_key), core_host=core_host
         )
         task.interpret(intepreter)
         return task.get_interpreted_task()
 
 
 class Space:
-    
+
     def __new__(
         cls,
         task: PromisedTask | FlowFunction[..., Any] | Any = None,  # noqa: ANN401, for IDE hints
         version_mode: VersionMode = VersionMode.MINOR,
+        reverse_id: str | None = None,
         force_attach: bool = False,
         deployment_id: str | None = None,
         attach_to_last: bool | None = None,
         ops: SpaceOps | None = None,
         *task_args,
         **task_kwargs
     ) -> SpaceTask:
-        
+
         setup = None
         if not ops:
             try:
                 setup = SpaceSetup(**manf.query('space', resolve_secrets=True))
             except Exception:
                 if not login():
                     raise Exception(
@@ -105,17 +106,18 @@
             warnings.warn(
                 "Ignoring `attach_to_last` as `force_attach` set to False"
             )
 
         if isinstance(task, FlowFunction):
             task: PromisedTask = task(*task_args, **task_kwargs)
 
-        reverse_id = task._component.reverse_id
+        if isinstance(task, PromisedTask):
+            reverse_id = task._component.reverse_id
 
-        if force_attach:
+        if force_attach or task is None:
             return interpreter.attach(
                 reverse_id=reverse_id,
                 deployment_id=deployment_id,
                 attach_to_last=attach_to_last is not None and attach_to_last
             )
 
         task.interpret(interpreter)
```

### Comparing `malevich-0.3.0/malevich/_export/space_flow.py` & `malevich-0.3.1/malevich/_export/space_flow.py`

 * *Files identical despite different names*

### Comparing `malevich-0.3.0/malevich/_meta/asset.py` & `malevich-0.3.1/malevich/_meta/asset.py`

 * *Files identical despite different names*

### Comparing `malevich-0.3.0/malevich/_meta/collection.py` & `malevich-0.3.1/malevich/_meta/collection.py`

 * *Files identical despite different names*

### Comparing `malevich-0.3.0/malevich/_meta/decor.py` & `malevich-0.3.1/malevich/_meta/decor.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import Callable, Generic, ParamSpec, Type, TypeVar
 
 from pydantic import BaseModel
 
 from .._autoflow.function import autotrace, sinktrace
 from ..constants import reserved_config_fields
+from ..models.type_annotations import ConfigArgument
 
 FnArgs = ParamSpec("FnArgs")
 FnReturn = TypeVar("FnReturn")
 Config = TypeVar("Config", bound=BaseModel)
 ProcConfig = TypeVar("ProcConfig", bound=BaseModel)
 
 ProcFunArgs = ParamSpec("ProcFunArgs")
@@ -28,14 +29,15 @@
         self.__config_model = config_model
         self.__call__ = self._fn_call
         self.__required_fields = [
             key
             for key, value in self.__fn.__annotations__.items()
             if hasattr(value, '__metadata__')
             and (metadata := getattr(value, '__metadata__'))
+            and isinstance(metadata[0], ConfigArgument)
             and metadata[0].required
         ]
 
     def _fn_call(self, *args: FnArgs.args, **kwargs: FnArgs.kwargs) -> FnReturn:
         # FIXME: literal 'config' is overused. Should be replaced with constant.
         if kwargs.get('config', None) is None:
             kwargs['config'] = {}
@@ -51,15 +53,15 @@
             assert isinstance(kwargs, dict)
 
         extra_fields = {**kwargs}
         extra_fields.pop('config')
         for reserved, _ in reserved_config_fields:
             extra_fields.pop(reserved, None)
 
-        kwargs['config'] = {
+        kwargs = {
             **kwargs['config'],
             **extra_fields,
         }
 
         if (diff_ := set.difference(set(self.__required_fields), kwargs.keys())) != set():  # noqa: E501
             fields_ = ', '.join([f"`{x}`" for x in diff_])
             raise Exception(
```

### Comparing `malevich-0.3.0/malevich/_meta/flow.py` & `malevich-0.3.1/malevich/_meta/flow.py`

 * *Files identical despite different names*

### Comparing `malevich-0.3.0/malevich/_meta/run.py` & `malevich-0.3.1/malevich/_meta/run.py`

 * *Files identical despite different names*

### Comparing `malevich-0.3.0/malevich/_templates/Dockerfile.app` & `malevich-0.3.1/malevich/_templates/Dockerfile.app`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Malevich App image. You may edit this file to add
 # additional dependencies to your app or set more
 # specific enironment.
 
 # Keep in mind, that source code containing
 # Malevich-specific code (declaration of processors, inits, etc.)
 # should be placed into ./apps directory
-FROM pogrebnoijak/julius_export_python:0.1
+FROM malevichai/app:python_v0.1
 
 # Copying requirements.txt and installing dependencies
 COPY requirements.txt requirements.txt
 RUN if test -e requirements.txt; then pip install --no-cache-dir -r requirements.txt; fi
 
 # Placing source code into the image
 # DO NOT change this line
```

### Comparing `malevich-0.3.0/malevich/_templates/README.app.md` & `malevich-0.3.1/malevich/_templates/README.app.md`

 * *Files identical despite different names*

### Comparing `malevich-0.3.0/malevich/_templates/flow.py.txt` & `malevich-0.3.1/malevich/_templates/flow.py.txt`

 * *Files identical despite different names*

### Comparing `malevich-0.3.0/malevich/_templates/processor.py.txt` & `malevich-0.3.1/malevich/_templates/processor.py.txt`

 * *Files identical despite different names*

### Comparing `malevich-0.3.0/malevich/_utility/__init__.py` & `malevich-0.3.1/malevich/_utility/__init__.py`

 * *Files identical despite different names*

### Comparing `malevich-0.3.0/malevich/_utility/_try.py` & `malevich-0.3.1/malevich/_utility/_try.py`

 * *Files identical despite different names*

### Comparing `malevich-0.3.0/malevich/_utility/args.py` & `malevich-0.3.1/malevich/_utility/args.py`

 * *Files identical despite different names*

### Comparing `malevich-0.3.0/malevich/_utility/cache/manager.py` & `malevich-0.3.1/malevich/_utility/cache/manager.py`

 * *Files identical despite different names*

### Comparing `malevich-0.3.0/malevich/_utility/ci/functions.py` & `malevich-0.3.1/malevich/_utility/ci/functions.py`

 * *Files identical despite different names*

### Comparing `malevich-0.3.0/malevich/_utility/ci/github.py` & `malevich-0.3.1/malevich/_utility/ci/github.py`

 * *Files identical despite different names*

### Comparing `malevich-0.3.0/malevich/_utility/ci/templates/malevich-ci-manual.yml` & `malevich-0.3.1/malevich/_utility/ci/templates/malevich-ci-manual.yml`

 * *Files identical despite different names*

### Comparing `malevich-0.3.0/malevich/_utility/ci/templates/malevich-ci.yml` & `malevich-0.3.1/malevich/_utility/ci/templates/malevich-ci.yml`

 * *Files identical despite different names*

### Comparing `malevich-0.3.0/malevich/_utility/dicts.py` & `malevich-0.3.1/malevich/_utility/dicts.py`

 * *Files identical despite different names*

### Comparing `malevich-0.3.0/malevich/_utility/git/clone.py` & `malevich-0.3.1/malevich/_utility/git/clone.py`

 * *Files identical despite different names*

### Comparing `malevich-0.3.0/malevich/_utility/logging.py` & `malevich-0.3.1/malevich/_utility/logging.py`

 * *Files identical despite different names*

### Comparing `malevich-0.3.0/malevich/_utility/package.py` & `malevich-0.3.1/malevich/_utility/package.py`

 * *Files identical despite different names*

### Comparing `malevich-0.3.0/malevich/_utility/registry.py` & `malevich-0.3.1/malevich/_utility/registry.py`

 * *Files identical despite different names*

### Comparing `malevich-0.3.0/malevich/_utility/scan.py` & `malevich-0.3.1/malevich/_utility/scan.py`

 * *Files identical despite different names*

### Comparing `malevich-0.3.0/malevich/_utility/space/get_core_creds.py` & `malevich-0.3.1/malevich/_utility/space/get_core_creds.py`

 * *Files identical despite different names*

### Comparing `malevich-0.3.0/malevich/_utility/stub.py` & `malevich-0.3.1/malevich/_utility/stub.py`

 * *Files identical despite different names*

### Comparing `malevich-0.3.0/malevich/_utility/summary/abstract.py` & `malevich-0.3.1/malevich/_utility/summary/abstract.py`

 * *Files identical despite different names*

### Comparing `malevich-0.3.0/malevich/_utility/summary/time.py` & `malevich-0.3.1/malevich/_utility/summary/time.py`

 * *Files identical despite different names*

### Comparing `malevich-0.3.0/malevich/_utility/tree.py` & `malevich-0.3.1/malevich/_utility/tree.py`

 * *Files identical despite different names*

### Comparing `malevich-0.3.0/malevich/annotations.py` & `malevich-0.3.1/malevich/annotations.py`

 * *Files identical despite different names*

### Comparing `malevich-0.3.0/malevich/cli.py` & `malevich-0.3.1/malevich/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,15 +70,15 @@
     )
 )
 
 # malevich new
 app.registered_commands.append(
     typer.models.CommandInfo(
         name="new",
-        help=help.list_["--help"],
+        help=help.new["--help"],
         callback=new,
         cls=typer.core.TyperCommand
     )
 )
 
 # malevich init
 app.registered_commands.append(
@@ -137,15 +137,15 @@
 # malevich prefs
 app.add_typer(prefs, name="prefs")
 
 # malevich dev
 app.add_typer(dev_app, name='dev')
 
 #malevich core
-app.add_typer(core_app, name='core')
+app.add_typer(core_app, name='core', help=help.core['--help'])
 # _________________________________________________
 
 
 class CLIContext:
     global_ = False
 
 @app.callback()
```

### Comparing `malevich-0.3.0/malevich/constants.py` & `malevich-0.3.1/malevich/constants.py`

 * *Files identical despite different names*

### Comparing `malevich-0.3.0/malevich/help.py` & `malevich-0.3.1/malevich/help.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,7 +84,11 @@
 list_ = {
     '--help': """List all installed package stubs."""
 }
 
 new = {
     '--help': """Create a new app from a template""",
 }
+
+core = {
+    '--help': """Manage your Core account"""
+}
```

### Comparing `malevich-0.3.0/malevich/install/image.py` & `malevich-0.3.1/malevich/install/image.py`

 * *Files identical despite different names*

### Comparing `malevich-0.3.0/malevich/install/installer.py` & `malevich-0.3.1/malevich/install/installer.py`

 * *Files identical despite different names*

### Comparing `malevich-0.3.0/malevich/install/iso.py` & `malevich-0.3.1/malevich/install/iso.py`

 * *Files identical despite different names*

### Comparing `malevich-0.3.0/malevich/install/space.py` & `malevich-0.3.1/malevich/install/space.py`

 * *Files identical despite different names*

### Comparing `malevich-0.3.0/malevich/install/stub.py` & `malevich-0.3.1/malevich/install/stub.py`

 * *Files identical despite different names*

### Comparing `malevich-0.3.0/malevich/interpreter/abstract.py` & `malevich-0.3.1/malevich/interpreter/abstract.py`

 * *Files identical despite different names*

### Comparing `malevich-0.3.0/malevich/interpreter/core.py` & `malevich-0.3.1/malevich/interpreter/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -220,15 +220,15 @@
         state: CoreInterpreterState,
         callee: traced[BaseNode],
         caller: traced[BaseNode],
         link: ArgumentLink,
     ) -> CoreInterpreterState:
         state.depends[caller.owner.uuid].append((callee.owner, link))
         _log(
-            f"Dependency: {caller.owner.short_info()} -> {callee.owner.short_info()}, "
+            f"Dependency: {callee.owner.short_info()} -> {caller.owner.short_info()}, "
             f"Link: {link.name}", -1, 0, True
         )
         return state
 
     def before_interpret(self, state: CoreInterpreterState) -> CoreInterpreterState:
         _log("Connection to Core is established.", 0, 0, True)
         _log(f"Core host: {self.__core_host}", 0, 0, True)
```

### Comparing `malevich-0.3.0/malevich/interpreter/space.py` & `malevich-0.3.1/malevich/interpreter/space.py`

 * *Files identical despite different names*

### Comparing `malevich-0.3.0/malevich/manifest.py` & `malevich-0.3.1/malevich/manifest.py`

 * *Files identical despite different names*

### Comparing `malevich-0.3.0/malevich/models/argument.py` & `malevich-0.3.1/malevich/models/argument.py`

 * *Files identical despite different names*

### Comparing `malevich-0.3.0/malevich/models/collection.py` & `malevich-0.3.1/malevich/models/collection.py`

 * *Files identical despite different names*

### Comparing `malevich-0.3.0/malevich/models/dependency.py` & `malevich-0.3.1/malevich/models/dependency.py`

 * *Files identical despite different names*

### Comparing `malevich-0.3.0/malevich/models/endpoint.py` & `malevich-0.3.1/malevich/models/endpoint.py`

 * *Files identical despite different names*

### Comparing `malevich-0.3.0/malevich/models/flow_function.py` & `malevich-0.3.1/malevich/models/flow_function.py`

 * *Files identical despite different names*

### Comparing `malevich-0.3.0/malevich/models/injections.py` & `malevich-0.3.1/malevich/models/injections.py`

 * *Files identical despite different names*

### Comparing `malevich-0.3.0/malevich/models/installers/compat.py` & `malevich-0.3.1/malevich/models/installers/compat.py`

 * *Files identical despite different names*

### Comparing `malevich-0.3.0/malevich/models/installers/image.py` & `malevich-0.3.1/malevich/models/installers/image.py`

 * *Files identical despite different names*

### Comparing `malevich-0.3.0/malevich/models/installers/space.py` & `malevich-0.3.1/malevich/models/installers/space.py`

 * *Files identical despite different names*

### Comparing `malevich-0.3.0/malevich/models/manifest.py` & `malevich-0.3.1/malevich/models/manifest.py`

 * *Files identical despite different names*

### Comparing `malevich-0.3.0/malevich/models/nodes/asset.py` & `malevich-0.3.1/malevich/models/nodes/asset.py`

 * *Files identical despite different names*

### Comparing `malevich-0.3.0/malevich/models/nodes/base.py` & `malevich-0.3.1/malevich/models/nodes/base.py`

 * *Files identical despite different names*

### Comparing `malevich-0.3.0/malevich/models/nodes/collection.py` & `malevich-0.3.1/malevich/models/nodes/collection.py`

 * *Files identical despite different names*

### Comparing `malevich-0.3.0/malevich/models/nodes/operation.py` & `malevich-0.3.1/malevich/models/nodes/operation.py`

 * *Files identical despite different names*

### Comparing `malevich-0.3.0/malevich/models/nodes/tree.py` & `malevich-0.3.1/malevich/models/nodes/tree.py`

 * *Files identical despite different names*

### Comparing `malevich-0.3.0/malevich/models/preferences.py` & `malevich-0.3.1/malevich/models/preferences.py`

 * *Files identical despite different names*

### Comparing `malevich-0.3.0/malevich/models/registry/core_entry.py` & `malevich-0.3.1/malevich/models/registry/core_entry.py`

 * *Files identical despite different names*

### Comparing `malevich-0.3.0/malevich/models/results/base.py` & `malevich-0.3.1/malevich/models/results/base.py`

 * *Files identical despite different names*

### Comparing `malevich-0.3.0/malevich/models/results/core/result.py` & `malevich-0.3.1/malevich/models/results/core/result.py`

 * *Files identical despite different names*

### Comparing `malevich-0.3.0/malevich/models/results/space/collection.py` & `malevich-0.3.1/malevich/models/results/space/collection.py`

 * *Files identical despite different names*

### Comparing `malevich-0.3.0/malevich/models/state/core.py` & `malevich-0.3.1/malevich/models/state/core.py`

 * *Files identical despite different names*

### Comparing `malevich-0.3.0/malevich/models/state/space.py` & `malevich-0.3.1/malevich/models/state/space.py`

 * *Files identical despite different names*

### Comparing `malevich-0.3.0/malevich/models/task/base.py` & `malevich-0.3.1/malevich/models/task/base.py`

 * *Files identical despite different names*

### Comparing `malevich-0.3.0/malevich/models/task/interpreted/core.py` & `malevich-0.3.1/malevich/models/task/interpreted/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -595,15 +595,15 @@
         capture_results: list[str] | Literal['all'] | Literal['last'] = 'last',
         enable_not_auth: bool = True,
         hash: str | None = None,
         *args,
         **kwargs
     ) -> MetaEndpoint:
         from malevich_coretools import create_endpoint, update_endpoint
-        if self.get_stage() != CoreTaskStage.BUILT:
+        if self.get_stage() not in [CoreTaskStage.BUILT, CoreTaskStage.ONLINE]:
             self.prepare(stage=PrepareStages.BUILD)
 
         cfg = deepcopy(self.state.cfg)
         if capture_results == 'last':
             cfg.app_settings = [
                 x for x in cfg.app_settings
                 if x.taskId == self.state.params.task_id
```

### Comparing `malevich-0.3.0/malevich/models/task/interpreted/space.py` & `malevich-0.3.1/malevich/models/task/interpreted/space.py`

 * *Files identical despite different names*

### Comparing `malevich-0.3.0/malevich/models/task/promised.py` & `malevich-0.3.1/malevich/models/task/promised.py`

 * *Files 2% similar despite different names*

```diff
@@ -325,13 +325,23 @@
                 "Unable to get interpreted task. "
                 "Please, use `.interpret` first to attach task to "
                 "a particular platform"
             )
         return self.__task
 
     def publish(self, *args, **kwargs) -> MetaEndpoint:
+        """Creates a HTTP endpoint for the task
+
+        Accepts any arguments and keyword arguments and passes them to the
+        underlying callback created in the interpreter itself. For particular
+        arguments and keyword arguments, see the documentation of the interpreter
+        used before calling this method.
+
+        Returns:
+            :class:`malevich.models.endpoint.MetaEndpoint`: An endpoint object
+        """
         if not self.__task:
             raise Exception(
                 "Cannot publish uninterpreted task. "
                 "Use `.interpret()` first."
             )
         return self.__task.publish(*args, **kwargs)
```

### Comparing `malevich-0.3.0/malevich/models/task.py` & `malevich-0.3.1/malevich/models/task.py`

 * *Files identical despite different names*

### Comparing `malevich-0.3.0/malevich/path.py` & `malevich-0.3.1/malevich/path.py`

 * *Files identical despite different names*

### Comparing `malevich-0.3.0/malevich/runners/base.py` & `malevich-0.3.1/malevich/runners/base.py`

 * *Files identical despite different names*

### Comparing `malevich-0.3.0/malevich/square/df.py` & `malevich-0.3.1/malevich/square/df.py`

 * *Files identical despite different names*

### Comparing `malevich-0.3.0/malevich/square/jls.py` & `malevich-0.3.1/malevich/square/jls.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     return wrapper
 
 
 def processor(id: Optional[str] = None, finish_msg: Optional[str] = None, drop_internal: bool = True, get_scale_part_all: bool = False):    # noqa: ANN201, E501
     """Denotes a processor of the app.
     
     Processors are core logical units of the app. To
-    understand processors more, see `What is Processor? <../Apps/What_is_Processor.html>`_
+    understand processors more, see :doc:`What is Processor? </SDK/Apps/Processors>`
     
     Args:
         id: The id of the processor. If not provided, the name of the function will be used.
         finish_msg: The message to be sent to e-mail (if configured) when the processor finishes.
         drop_internal: Whether to drop the internal collections after the processor finishes.
         get_scale_part_all: Whether to get the scale part of the input collection.
```

### Comparing `malevich-0.3.0/malevich/square/utils.py` & `malevich-0.3.1/malevich/square/utils.py`

 * *Files identical despite different names*

### Comparing `malevich-0.3.0/malevich/testing/env.py` & `malevich-0.3.1/malevich/testing/env.py`

 * *Files identical despite different names*

### Comparing `malevich-0.3.0/malevich/testing/suite.py` & `malevich-0.3.1/malevich/testing/suite.py`

 * *Files identical despite different names*

### Comparing `malevich-0.3.0/malevich.egg-info/PKG-INFO` & `malevich-0.3.1/malevich.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: malevich
-Version: 0.3.0
+Version: 0.3.1
 Summary: ('A user-friendly interface to communicate with Malevich AI (malevich.ai)',)
 License-File: LICENSE
 Requires-Dist: typer[all]>=0.9.0
 Requires-Dist: pydantic>=2.0.0
 Requires-Dist: malevich-coretools>=0.3.11
 Requires-Dist: malevich-space>=0.4.18
 Requires-Dist: pandas
```

### Comparing `malevich-0.3.0/malevich.egg-info/SOURCES.txt` & `malevich-0.3.1/malevich.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,19 @@
 requirements.txt
 setup.py
 ./.pre-commit-config.yaml
 ./.github/workflows/docs.yaml
 ./.github/workflows/pypi.yaml
 ./.github/workflows/pytest.yaml
 ./.github/workflows/ruff.yaml
+./malevich/_templates/Dockerfile.app
+./malevich/_templates/README.app.md
+./malevich/_templates/flow.py.txt
+./malevich/_templates/processor.py.txt
+./malevich/_templates/space.yaml.txt
 ./malevich/_utility/ci/templates/malevich-ci-manual.yml
 ./malevich/_utility/ci/templates/malevich-ci.yml
 malevich/__init__.py
 malevich/_deploy.py
 malevich/annotations.py
 malevich/cli.py
 malevich/constants.py
@@ -170,9 +175,11 @@
 malevich/square/__init__.py
 malevich/square/defaults.py
 malevich/square/df.py
 malevich/square/jls.py
 malevich/square/utils.py
 malevich/testing/__init__.py
 malevich/testing/env.py
+malevich/testing/fixtures.py
 malevich/testing/suite.py
-malevich/testing/testcase.py
+malevich/testing/testcase.py
+malevich/testing/env/__init__.py
```

