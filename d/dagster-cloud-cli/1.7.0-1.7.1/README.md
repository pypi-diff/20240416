# Comparing `tmp/dagster-cloud-cli-1.7.0.tar.gz` & `tmp/dagster-cloud-cli-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-cloud-cli-1.7.0.tar", last modified: Thu Apr  4 19:55:58 2024, max compression
+gzip compressed data, was "dagster-cloud-cli-1.7.1.tar", last modified: Thu Apr 11 18:18:55 2024, max compression
```

## Comparing `dagster-cloud-cli-1.7.0.tar` & `dagster-cloud-cli-1.7.1.tar`

### file list

```diff
@@ -1,92 +1,92 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:55:58.676234 dagster-cloud-cli-1.7.0/
--rw-r--r--   0 root         (0) root         (0)      132 2024-04-04 19:44:30.000000 dagster-cloud-cli-1.7.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      314 2024-04-04 19:55:58.676234 dagster-cloud-cli-1.7.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:55:58.640234 dagster-cloud-cli-1.7.0/dagster_cloud_cli/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 19:44:30.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:55:58.644234 dagster-cloud-cli-1.7.0/dagster_cloud_cli/commands/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 19:44:30.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli/commands/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:55:58.644234 dagster-cloud-cli-1.7.0/dagster_cloud_cli/commands/branch_deployment/
--rw-r--r--   0 root         (0) root         (0)     4947 2024-04-04 19:44:30.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli/commands/branch_deployment/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:55:58.648234 dagster-cloud-cli-1.7.0/dagster_cloud_cli/commands/ci/
--rw-r--r--   0 root         (0) root         (0)    26640 2024-04-04 19:44:30.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli/commands/ci/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4124 2024-04-04 19:44:30.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli/commands/ci/checks.py
--rw-r--r--   0 root         (0) root         (0)     1872 2024-04-04 19:44:30.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli/commands/ci/report.py
--rw-r--r--   0 root         (0) root         (0)     4090 2024-04-04 19:44:30.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli/commands/ci/state.py
--rw-r--r--   0 root         (0) root         (0)      508 2024-04-04 19:44:30.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli/commands/ci/utils.py
--rw-r--r--   0 root         (0) root         (0)     8651 2024-04-04 19:44:30.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli/commands/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:55:58.648234 dagster-cloud-cli-1.7.0/dagster_cloud_cli/commands/deployment/
--rw-r--r--   0 root         (0) root         (0)     2952 2024-04-04 19:44:30.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli/commands/deployment/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:55:58.648234 dagster-cloud-cli-1.7.0/dagster_cloud_cli/commands/deployment/alert_policies/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 19:44:30.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli/commands/deployment/alert_policies/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1634 2024-04-04 19:44:30.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli/commands/deployment/alert_policies/commands.py
--rw-r--r--   0 root         (0) root         (0)    17056 2024-04-04 19:44:30.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli/commands/deployment/alert_policies/config_schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:55:58.648234 dagster-cloud-cli-1.7.0/dagster_cloud_cli/commands/job/
--rw-r--r--   0 root         (0) root         (0)     1926 2024-04-04 19:44:30.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli/commands/job/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4425 2024-04-04 19:44:30.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli/commands/metrics.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:55:58.648234 dagster-cloud-cli-1.7.0/dagster_cloud_cli/commands/organization/
--rw-r--r--   0 root         (0) root         (0)     4001 2024-04-04 19:44:30.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli/commands/organization/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:55:58.652234 dagster-cloud-cli-1.7.0/dagster_cloud_cli/commands/organization/saml/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 19:44:30.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli/commands/organization/saml/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2691 2024-04-04 19:44:30.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli/commands/organization/saml/commands.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:55:58.652234 dagster-cloud-cli-1.7.0/dagster_cloud_cli/commands/run/
--rw-r--r--   0 root         (0) root         (0)      669 2024-04-04 19:44:30.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli/commands/run/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:55:58.656234 dagster-cloud-cli-1.7.0/dagster_cloud_cli/commands/serverless/
--rw-r--r--   0 root         (0) root         (0)     1499 2024-04-04 19:44:30.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli/commands/serverless/Dockerfile
--rw-r--r--   0 root         (0) root         (0)      628 2024-04-04 19:44:30.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli/commands/serverless/Dockerfile.dagster-cloud-cli
--rw-r--r--   0 root         (0) root         (0)    18361 2024-04-04 19:44:30.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli/commands/serverless/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:55:58.656234 dagster-cloud-cli-1.7.0/dagster_cloud_cli/commands/workspace/
--rw-r--r--   0 root         (0) root         (0)    12434 2024-04-04 19:44:30.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli/commands/workspace/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18301 2024-04-04 19:44:30.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli/config_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:55:58.660234 dagster-cloud-cli-1.7.0/dagster_cloud_cli/core/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 19:44:30.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)      901 2024-04-04 19:44:30.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli/core/alert_types.py
--rw-r--r--   0 root         (0) root         (0)     4801 2024-04-04 19:44:30.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli/core/artifacts.py
--rw-r--r--   0 root         (0) root         (0)     1744 2024-04-04 19:44:30.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli/core/docker_runner.py
--rw-r--r--   0 root         (0) root         (0)     1131 2024-04-04 19:44:30.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli/core/errors.py
--rw-r--r--   0 root         (0) root         (0)    12940 2024-04-04 19:44:30.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli/core/graphql_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:55:58.660234 dagster-cloud-cli-1.7.0/dagster_cloud_cli/core/headers/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 19:44:30.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli/core/headers/__init__.py
--rw-r--r--   0 root         (0) root         (0)      376 2024-04-04 19:44:30.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli/core/headers/auth.py
--rw-r--r--   0 root         (0) root         (0)      924 2024-04-04 19:44:30.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli/core/headers/impl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:55:58.664234 dagster-cloud-cli-1.7.0/dagster_cloud_cli/core/headers/versioning/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 19:44:30.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli/core/headers/versioning/__init__.py
--rw-r--r--   0 root         (0) root         (0)       96 2024-04-04 19:44:30.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli/core/headers/versioning/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:55:58.672234 dagster-cloud-cli-1.7.0/dagster_cloud_cli/core/pex_builder/
--rw-r--r--   0 root         (0) root         (0)      172 2024-04-04 19:44:30.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli/core/pex_builder/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1680 2024-04-04 19:44:30.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli/core/pex_builder/code_location.py
--rw-r--r--   0 root         (0) root         (0)     9423 2024-04-04 19:44:30.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli/core/pex_builder/deploy.py
--rw-r--r--   0 root         (0) root         (0)    13814 2024-04-04 19:44:30.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli/core/pex_builder/deps.py
--rw-r--r--   0 root         (0) root         (0)      949 2024-04-04 19:44:30.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli/core/pex_builder/git_context.py
--rw-r--r--   0 root         (0) root         (0)     6992 2024-04-04 19:44:30.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli/core/pex_builder/github_context.py
--rw-r--r--   0 root         (0) root         (0)     1063 2024-04-04 19:44:30.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli/core/pex_builder/gitlab_context.py
--rw-r--r--   0 root         (0) root         (0)     1232 2024-04-04 19:44:30.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli/core/pex_builder/parse_workspace.py
--rw-r--r--   0 root         (0) root         (0)     4655 2024-04-04 19:44:30.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli/core/pex_builder/pex_registry.py
--rw-r--r--   0 root         (0) root         (0)      709 2024-04-04 19:44:30.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli/core/pex_builder/selftest.py
--rw-r--r--   0 root         (0) root         (0)     5407 2024-04-04 19:44:30.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli/core/pex_builder/source.py
--rw-r--r--   0 root         (0) root         (0)     6220 2024-04-04 19:44:30.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli/core/pex_builder/util.py
--rw-r--r--   0 root         (0) root         (0)     2123 2024-04-04 19:44:30.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli/core/pydantic_yaml.py
--rw-r--r--   0 root         (0) root         (0)     7106 2024-04-04 19:44:30.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli/core/workspace.py
--rw-r--r--   0 root         (0) root         (0)     2463 2024-04-04 19:44:30.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli/docker_utils.py
--rw-r--r--   0 root         (0) root         (0)     6708 2024-04-04 19:44:30.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli/entrypoint.py
--rw-r--r--   0 root         (0) root         (0)    21075 2024-04-04 19:44:30.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli/gql.py
--rw-r--r--   0 root         (0) root         (0)     5859 2024-04-04 19:44:30.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli/pex_utils.py
--rw-r--r--   0 root         (0) root         (0)     1845 2024-04-04 19:44:30.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli/types.py
--rw-r--r--   0 root         (0) root         (0)     2804 2024-04-04 19:44:30.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli/ui.py
--rw-r--r--   0 root         (0) root         (0)     3488 2024-04-04 19:44:30.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli/utils.py
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-04 19:44:30.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:55:58.644234 dagster-cloud-cli-1.7.0/dagster_cloud_cli.egg-info/
--rw-r--r--   0 root         (0) root         (0)      314 2024-04-04 19:55:58.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2991 2024-04-04 19:55:58.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-04 19:55:58.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       67 2024-04-04 19:55:58.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       97 2024-04-04 19:55:58.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       42 2024-04-04 19:55:58.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:55:58.676234 dagster-cloud-cli-1.7.0/dagster_cloud_cli_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 19:44:30.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)      189 2024-04-04 19:44:30.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli_tests/conftest.py
--rw-r--r--   0 root         (0) root         (0)     4130 2024-04-04 19:44:30.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli_tests/test_check.py
--rw-r--r--   0 root         (0) root         (0)    16130 2024-04-04 19:44:30.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli_tests/test_ci_commands.py
--rw-r--r--   0 root         (0) root         (0)      683 2024-04-04 19:44:30.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli_tests/test_gql.py
--rw-r--r--   0 root         (0) root         (0)     8872 2024-04-04 19:44:30.000000 dagster-cloud-cli-1.7.0/dagster_cloud_cli_tests/test_metrics.py
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-04 19:55:58.676234 dagster-cloud-cli-1.7.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1139 2024-04-04 19:44:30.000000 dagster-cloud-cli-1.7.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:18:55.119890 dagster-cloud-cli-1.7.1/
+-rw-r--r--   0 root         (0) root         (0)      132 2024-04-11 18:04:43.000000 dagster-cloud-cli-1.7.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      314 2024-04-11 18:18:55.119890 dagster-cloud-cli-1.7.1/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:18:55.083890 dagster-cloud-cli-1.7.1/dagster_cloud_cli/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 18:04:43.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:18:55.087890 dagster-cloud-cli-1.7.1/dagster_cloud_cli/commands/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 18:04:43.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli/commands/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:18:55.087890 dagster-cloud-cli-1.7.1/dagster_cloud_cli/commands/branch_deployment/
+-rw-r--r--   0 root         (0) root         (0)     4947 2024-04-11 18:04:43.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli/commands/branch_deployment/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:18:55.091890 dagster-cloud-cli-1.7.1/dagster_cloud_cli/commands/ci/
+-rw-r--r--   0 root         (0) root         (0)    29688 2024-04-11 18:04:43.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli/commands/ci/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4124 2024-04-11 18:04:43.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli/commands/ci/checks.py
+-rw-r--r--   0 root         (0) root         (0)     1872 2024-04-11 18:04:43.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli/commands/ci/report.py
+-rw-r--r--   0 root         (0) root         (0)     4121 2024-04-11 18:04:43.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli/commands/ci/state.py
+-rw-r--r--   0 root         (0) root         (0)      508 2024-04-11 18:04:43.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli/commands/ci/utils.py
+-rw-r--r--   0 root         (0) root         (0)     8651 2024-04-11 18:04:43.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli/commands/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:18:55.091890 dagster-cloud-cli-1.7.1/dagster_cloud_cli/commands/deployment/
+-rw-r--r--   0 root         (0) root         (0)     2952 2024-04-11 18:04:43.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli/commands/deployment/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:18:55.091890 dagster-cloud-cli-1.7.1/dagster_cloud_cli/commands/deployment/alert_policies/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 18:04:43.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli/commands/deployment/alert_policies/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1634 2024-04-11 18:04:43.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli/commands/deployment/alert_policies/commands.py
+-rw-r--r--   0 root         (0) root         (0)    17056 2024-04-11 18:04:43.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli/commands/deployment/alert_policies/config_schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:18:55.091890 dagster-cloud-cli-1.7.1/dagster_cloud_cli/commands/job/
+-rw-r--r--   0 root         (0) root         (0)     1926 2024-04-11 18:04:43.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli/commands/job/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4425 2024-04-11 18:04:43.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli/commands/metrics.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:18:55.091890 dagster-cloud-cli-1.7.1/dagster_cloud_cli/commands/organization/
+-rw-r--r--   0 root         (0) root         (0)     4001 2024-04-11 18:04:43.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli/commands/organization/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:18:55.095890 dagster-cloud-cli-1.7.1/dagster_cloud_cli/commands/organization/saml/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 18:04:43.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli/commands/organization/saml/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2691 2024-04-11 18:04:43.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli/commands/organization/saml/commands.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:18:55.095890 dagster-cloud-cli-1.7.1/dagster_cloud_cli/commands/run/
+-rw-r--r--   0 root         (0) root         (0)      669 2024-04-11 18:04:43.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli/commands/run/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:18:55.095890 dagster-cloud-cli-1.7.1/dagster_cloud_cli/commands/serverless/
+-rw-r--r--   0 root         (0) root         (0)     1499 2024-04-11 18:04:43.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli/commands/serverless/Dockerfile
+-rw-r--r--   0 root         (0) root         (0)      628 2024-04-11 18:04:43.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli/commands/serverless/Dockerfile.dagster-cloud-cli
+-rw-r--r--   0 root         (0) root         (0)    18361 2024-04-11 18:04:43.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli/commands/serverless/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:18:55.095890 dagster-cloud-cli-1.7.1/dagster_cloud_cli/commands/workspace/
+-rw-r--r--   0 root         (0) root         (0)    12434 2024-04-11 18:04:43.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli/commands/workspace/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18301 2024-04-11 18:04:43.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli/config_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:18:55.103890 dagster-cloud-cli-1.7.1/dagster_cloud_cli/core/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 18:04:43.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      901 2024-04-11 18:04:43.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli/core/alert_types.py
+-rw-r--r--   0 root         (0) root         (0)     4801 2024-04-11 18:04:43.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli/core/artifacts.py
+-rw-r--r--   0 root         (0) root         (0)     1744 2024-04-11 18:04:43.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli/core/docker_runner.py
+-rw-r--r--   0 root         (0) root         (0)     1131 2024-04-11 18:04:43.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli/core/errors.py
+-rw-r--r--   0 root         (0) root         (0)    12940 2024-04-11 18:04:43.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli/core/graphql_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:18:55.103890 dagster-cloud-cli-1.7.1/dagster_cloud_cli/core/headers/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 18:04:43.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli/core/headers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      376 2024-04-11 18:04:43.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli/core/headers/auth.py
+-rw-r--r--   0 root         (0) root         (0)      924 2024-04-11 18:04:43.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli/core/headers/impl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:18:55.103890 dagster-cloud-cli-1.7.1/dagster_cloud_cli/core/headers/versioning/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 18:04:43.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli/core/headers/versioning/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       96 2024-04-11 18:04:43.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli/core/headers/versioning/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:18:55.115890 dagster-cloud-cli-1.7.1/dagster_cloud_cli/core/pex_builder/
+-rw-r--r--   0 root         (0) root         (0)      172 2024-04-11 18:04:43.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli/core/pex_builder/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1680 2024-04-11 18:04:43.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli/core/pex_builder/code_location.py
+-rw-r--r--   0 root         (0) root         (0)     9423 2024-04-11 18:04:43.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli/core/pex_builder/deploy.py
+-rw-r--r--   0 root         (0) root         (0)    13814 2024-04-11 18:04:43.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli/core/pex_builder/deps.py
+-rw-r--r--   0 root         (0) root         (0)      949 2024-04-11 18:04:43.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli/core/pex_builder/git_context.py
+-rw-r--r--   0 root         (0) root         (0)     6992 2024-04-11 18:04:43.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli/core/pex_builder/github_context.py
+-rw-r--r--   0 root         (0) root         (0)     1063 2024-04-11 18:04:43.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli/core/pex_builder/gitlab_context.py
+-rw-r--r--   0 root         (0) root         (0)     1232 2024-04-11 18:04:43.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli/core/pex_builder/parse_workspace.py
+-rw-r--r--   0 root         (0) root         (0)     4655 2024-04-11 18:04:43.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli/core/pex_builder/pex_registry.py
+-rw-r--r--   0 root         (0) root         (0)      709 2024-04-11 18:04:43.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli/core/pex_builder/selftest.py
+-rw-r--r--   0 root         (0) root         (0)     5407 2024-04-11 18:04:43.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli/core/pex_builder/source.py
+-rw-r--r--   0 root         (0) root         (0)     6220 2024-04-11 18:04:43.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli/core/pex_builder/util.py
+-rw-r--r--   0 root         (0) root         (0)     2123 2024-04-11 18:04:43.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli/core/pydantic_yaml.py
+-rw-r--r--   0 root         (0) root         (0)     7106 2024-04-11 18:04:43.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli/core/workspace.py
+-rw-r--r--   0 root         (0) root         (0)     2463 2024-04-11 18:04:43.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli/docker_utils.py
+-rw-r--r--   0 root         (0) root         (0)     6708 2024-04-11 18:04:43.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli/entrypoint.py
+-rw-r--r--   0 root         (0) root         (0)    21075 2024-04-11 18:04:43.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli/gql.py
+-rw-r--r--   0 root         (0) root         (0)     5859 2024-04-11 18:04:43.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli/pex_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1845 2024-04-11 18:04:43.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli/types.py
+-rw-r--r--   0 root         (0) root         (0)     2804 2024-04-11 18:04:43.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli/ui.py
+-rw-r--r--   0 root         (0) root         (0)     3488 2024-04-11 18:04:43.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli/utils.py
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-11 18:04:43.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:18:55.083890 dagster-cloud-cli-1.7.1/dagster_cloud_cli.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      314 2024-04-11 18:18:54.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2991 2024-04-11 18:18:54.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-11 18:18:54.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       67 2024-04-11 18:18:54.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       97 2024-04-11 18:18:54.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       42 2024-04-11 18:18:54.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:18:55.119890 dagster-cloud-cli-1.7.1/dagster_cloud_cli_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 18:04:43.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      189 2024-04-11 18:04:43.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli_tests/conftest.py
+-rw-r--r--   0 root         (0) root         (0)     4130 2024-04-11 18:04:43.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli_tests/test_check.py
+-rw-r--r--   0 root         (0) root         (0)    16177 2024-04-11 18:04:43.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli_tests/test_ci_commands.py
+-rw-r--r--   0 root         (0) root         (0)      683 2024-04-11 18:04:43.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli_tests/test_gql.py
+-rw-r--r--   0 root         (0) root         (0)     8872 2024-04-11 18:04:43.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli_tests/test_metrics.py
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-11 18:18:55.119890 dagster-cloud-cli-1.7.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1139 2024-04-11 18:04:43.000000 dagster-cloud-cli-1.7.1/setup.py
```

### Comparing `dagster-cloud-cli-1.7.0/dagster_cloud_cli/commands/branch_deployment/__init__.py` & `dagster-cloud-cli-1.7.1/dagster_cloud_cli/commands/branch_deployment/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.0/dagster_cloud_cli/commands/ci/__init__.py` & `dagster-cloud-cli-1.7.1/dagster_cloud_cli/commands/ci/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import logging
 import os
 import pathlib
 import shutil
 import sys
 from collections import Counter
 from enum import Enum
-from typing import Any, Dict, List, Optional
+from typing import Any, Dict, List, Optional, cast
 
 import typer
 from typer import Typer
 
 from dagster_cloud_cli import docker_utils, gql, pex_utils, ui
 from dagster_cloud_cli.commands.ci import utils
 from dagster_cloud_cli.commands.workspace import wait_for_load
@@ -24,28 +24,32 @@
     TOKEN_ENV_VAR_NAME,
     URL_ENV_VAR_NAME,
     dagster_cloud_options,
     get_location_document,
     get_org_url,
 )
 from dagster_cloud_cli.core import pex_builder, pydantic_yaml
-
-from .. import metrics
-from . import checks, report, state
-
-app = Typer(hidden=True, help="CI/CD agnostic commands")
+from dagster_cloud_cli.core.artifacts import (
+    download_organization_artifact,
+    upload_organization_artifact,
+)
 from dagster_cloud_cli.core.pex_builder import (
     code_location,
     deps,
     github_context,
     gitlab_context,
     parse_workspace,
 )
 from dagster_cloud_cli.types import CliEventTags, CliEventType
 
+from .. import metrics
+from . import checks, report, state
+
+app = Typer(hidden=True, help="CI/CD agnostic commands")
+
 
 @app.command(help="Print json information about current CI/CD environment")
 def inspect(project_dir: str):
     project_dir = os.path.abspath(project_dir)
     source = metrics.get_source()
     info = {"source": str(source), "project-dir": project_dir}
     if source == CliEventTags.source.github:
@@ -200,38 +204,45 @@
     clean_statedir: bool = typer.Option(True, help="Delete any existing files in statedir"),
     location_name: List[str] = typer.Option([]),
     git_url: Optional[str] = None,
     commit_hash: Optional[str] = None,
     status_url: Optional[str] = None,
 ):
     yaml_path = pathlib.Path(project_dir) / dagster_cloud_yaml_path
+    if not yaml_path.exists():
+        raise ui.error(
+            f"Dagster Cloud yaml file not found at specified path {yaml_path.resolve()}."
+        )
     locations_def = pydantic_yaml.load_dagster_cloud_yaml(yaml_path.read_text())
     locations = locations_def.locations
     if location_name:
         selected_locations = set(location_name)
         unknown = selected_locations - set(location.location_name for location in locations)
         if unknown:
             raise ui.error(f"Locations not found in {dagster_cloud_yaml_path}: {unknown}")
         locations = [
             location for location in locations if location.location_name in selected_locations
         ]
     url = get_org_url(organization, dagster_env)
     # Deploy to the branch deployment for the current context. If there is no branch deployment
     # available (eg. if not in a PR) then we fallback to the --deployment flag.
+
     try:
         branch_deployment = get_deployment_from_context(url, project_dir)
         if deployment:
             ui.print(
                 f"Deploying to branch deployment {branch_deployment}, ignoring"
                 f" --deployment={deployment}"
             )
         deployment = branch_deployment
+        is_branch_deployment = True
     except ValueError as err:
         if deployment:
             ui.print(f"Deploying to {deployment}. No branch deployment ({err}).")
+            is_branch_deployment = False
         else:
             raise ui.error(
                 f"Cannot determine deployment name in current context ({err}). Please specify"
                 " --deployment."
             )
 
     if clean_statedir and os.path.exists(statedir):
@@ -241,14 +252,15 @@
     ui.print(f"Initializing {statedir}")
     for location in locations:
         location_state = state.LocationState(
             url=url,
             deployment_name=deployment,
             location_file=str(yaml_path.absolute()),
             location_name=location.location_name,
+            is_branch_deployment=is_branch_deployment,
             build=state.BuildMetadata(
                 git_url=git_url, commit_hash=commit_hash, build_config=location.build
             ),
             build_output=None,
             status_url=status_url,
         )
         location_state.add_status_change(state.LocationStatus.pending, "initialized")
@@ -699,7 +711,81 @@
         wait_for_load(
             client,
             [location.location_name for location in built_locations],
             location_load_timeout=location_load_timeout,
             agent_heartbeat_timeout=agent_heartbeat_timeout,
             url=deployment_url,
         )
+
+
+dagster_dbt_app = typer.Typer(
+    hidden=True,
+    help="Dagster Cloud commands for managing the `dagster-dbt` integration.",
+    add_completion=False,
+)
+app.add_typer(dagster_dbt_app, name="dagster-dbt", no_args_is_help=True)
+
+project_app = typer.Typer(
+    name="project",
+    no_args_is_help=True,
+    help="Commands for using a dbt project in Dagster.",
+    add_completion=False,
+)
+dagster_dbt_app.add_typer(project_app, name="project", no_args_is_help=True)
+
+
+@project_app.command(
+    name="manage-state",
+    help="""
+    This CLI command will handle uploading and downloading dbt state, in the form of manifest.json,
+    if `state_path` is specified on `DbtProject`.
+    """,
+)
+def manage_state_command(
+    statedir: str = STATEDIR_OPTION,
+    file: str = typer.Option(),
+    source_deployment: str = typer.Option(
+        default="prod",
+        help="Which deployment should upload its manifest.json.",
+    ),
+    key_prefix: str = typer.Option(
+        default="",
+        help="A key prefix for the key the manifest.json is saved with.",
+    ),
+):
+    try:
+        from dagster_dbt import DbtProject
+    except:
+        ui.print(
+            "Unable to import dagster_dbt. To use `manage-state`, dagster_dbt must be installed."
+        )
+        return
+    from dagster._core.code_pointer import load_python_file
+    from dagster._core.definitions.load_assets_from_modules import find_objects_in_module_of_types
+
+    state_store = state.FileStore(statedir=statedir)
+    locations = state_store.list_locations()
+    if not locations:
+        raise ui.error("Unable to determine deployment state.")
+
+    location = locations[0]
+    deployment_name = location.deployment_name
+    is_branch = location.is_branch_deployment
+
+    contents = load_python_file(file, None)
+    for project in find_objects_in_module_of_types(contents, DbtProject):
+        project = cast(DbtProject, project)
+        if project.state_path:
+            download_path = project.state_path.joinpath("manifest.json")
+            key = f"{key_prefix}{os.fspath(download_path)}"
+            if is_branch:
+                ui.print(f"Downloading {source_deployment} manifest for branch deployment.")
+                os.makedirs(project.state_path, exist_ok=True)
+                download_organization_artifact(key, download_path)
+                ui.print("Download complete.")
+
+            elif deployment_name == source_deployment:
+                ui.print(f"Uploading {source_deployment} manifest.")
+                upload_organization_artifact(key, project.manifest_path)
+                ui.print("Upload complete")
+
+        ui.print("Project ready")
```

### Comparing `dagster-cloud-cli-1.7.0/dagster_cloud_cli/commands/ci/checks.py` & `dagster-cloud-cli-1.7.1/dagster_cloud_cli/commands/ci/checks.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.0/dagster_cloud_cli/commands/ci/report.py` & `dagster-cloud-cli-1.7.1/dagster_cloud_cli/commands/ci/report.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.0/dagster_cloud_cli/commands/ci/state.py` & `dagster-cloud-cli-1.7.1/dagster_cloud_cli/commands/ci/state.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,15 @@
 
 class LocationState(BaseModel, extra=Extra.forbid):
     # we intentionally don't save api_token here for security reasons
     url: str
     deployment_name: str
     location_file: str
     location_name: str
+    is_branch_deployment: bool
     selected: bool = True
     build: BuildMetadata
     build_output: Optional[Union[DockerBuildOutput, PexBuildOutput]] = Field(
         None, discriminator="strategy"
     )
     status_url: Optional[str]  # link to cicd run url when building and dagster cloud url when done
     history: List[StatusChange] = []
```

### Comparing `dagster-cloud-cli-1.7.0/dagster_cloud_cli/commands/config.py` & `dagster-cloud-cli-1.7.1/dagster_cloud_cli/commands/config.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.0/dagster_cloud_cli/commands/deployment/__init__.py` & `dagster-cloud-cli-1.7.1/dagster_cloud_cli/commands/deployment/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.0/dagster_cloud_cli/commands/deployment/alert_policies/commands.py` & `dagster-cloud-cli-1.7.1/dagster_cloud_cli/commands/deployment/alert_policies/commands.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.0/dagster_cloud_cli/commands/deployment/alert_policies/config_schema.py` & `dagster-cloud-cli-1.7.1/dagster_cloud_cli/commands/deployment/alert_policies/config_schema.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.0/dagster_cloud_cli/commands/job/__init__.py` & `dagster-cloud-cli-1.7.1/dagster_cloud_cli/commands/job/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.0/dagster_cloud_cli/commands/metrics.py` & `dagster-cloud-cli-1.7.1/dagster_cloud_cli/commands/metrics.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.0/dagster_cloud_cli/commands/organization/__init__.py` & `dagster-cloud-cli-1.7.1/dagster_cloud_cli/commands/organization/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.0/dagster_cloud_cli/commands/organization/saml/commands.py` & `dagster-cloud-cli-1.7.1/dagster_cloud_cli/commands/organization/saml/commands.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.0/dagster_cloud_cli/commands/run/__init__.py` & `dagster-cloud-cli-1.7.1/dagster_cloud_cli/commands/run/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.0/dagster_cloud_cli/commands/serverless/Dockerfile` & `dagster-cloud-cli-1.7.1/dagster_cloud_cli/commands/serverless/Dockerfile`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.0/dagster_cloud_cli/commands/serverless/Dockerfile.dagster-cloud-cli` & `dagster-cloud-cli-1.7.1/dagster_cloud_cli/commands/serverless/Dockerfile.dagster-cloud-cli`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.0/dagster_cloud_cli/commands/serverless/__init__.py` & `dagster-cloud-cli-1.7.1/dagster_cloud_cli/commands/serverless/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.0/dagster_cloud_cli/commands/workspace/__init__.py` & `dagster-cloud-cli-1.7.1/dagster_cloud_cli/commands/workspace/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.0/dagster_cloud_cli/config_utils.py` & `dagster-cloud-cli-1.7.1/dagster_cloud_cli/config_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.0/dagster_cloud_cli/core/alert_types.py` & `dagster-cloud-cli-1.7.1/dagster_cloud_cli/core/alert_types.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.0/dagster_cloud_cli/core/artifacts.py` & `dagster-cloud-cli-1.7.1/dagster_cloud_cli/core/artifacts.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.0/dagster_cloud_cli/core/docker_runner.py` & `dagster-cloud-cli-1.7.1/dagster_cloud_cli/core/docker_runner.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.0/dagster_cloud_cli/core/errors.py` & `dagster-cloud-cli-1.7.1/dagster_cloud_cli/core/errors.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.0/dagster_cloud_cli/core/graphql_client.py` & `dagster-cloud-cli-1.7.1/dagster_cloud_cli/core/graphql_client.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.0/dagster_cloud_cli/core/headers/impl.py` & `dagster-cloud-cli-1.7.1/dagster_cloud_cli/core/headers/impl.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.0/dagster_cloud_cli/core/pex_builder/code_location.py` & `dagster-cloud-cli-1.7.1/dagster_cloud_cli/core/pex_builder/code_location.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.0/dagster_cloud_cli/core/pex_builder/deploy.py` & `dagster-cloud-cli-1.7.1/dagster_cloud_cli/core/pex_builder/deploy.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.0/dagster_cloud_cli/core/pex_builder/deps.py` & `dagster-cloud-cli-1.7.1/dagster_cloud_cli/core/pex_builder/deps.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.0/dagster_cloud_cli/core/pex_builder/git_context.py` & `dagster-cloud-cli-1.7.1/dagster_cloud_cli/core/pex_builder/git_context.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.0/dagster_cloud_cli/core/pex_builder/github_context.py` & `dagster-cloud-cli-1.7.1/dagster_cloud_cli/core/pex_builder/github_context.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.0/dagster_cloud_cli/core/pex_builder/gitlab_context.py` & `dagster-cloud-cli-1.7.1/dagster_cloud_cli/core/pex_builder/gitlab_context.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.0/dagster_cloud_cli/core/pex_builder/parse_workspace.py` & `dagster-cloud-cli-1.7.1/dagster_cloud_cli/core/pex_builder/parse_workspace.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.0/dagster_cloud_cli/core/pex_builder/pex_registry.py` & `dagster-cloud-cli-1.7.1/dagster_cloud_cli/core/pex_builder/pex_registry.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.0/dagster_cloud_cli/core/pex_builder/selftest.py` & `dagster-cloud-cli-1.7.1/dagster_cloud_cli/core/pex_builder/selftest.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.0/dagster_cloud_cli/core/pex_builder/source.py` & `dagster-cloud-cli-1.7.1/dagster_cloud_cli/core/pex_builder/source.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.0/dagster_cloud_cli/core/pex_builder/util.py` & `dagster-cloud-cli-1.7.1/dagster_cloud_cli/core/pex_builder/util.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.0/dagster_cloud_cli/core/pydantic_yaml.py` & `dagster-cloud-cli-1.7.1/dagster_cloud_cli/core/pydantic_yaml.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.0/dagster_cloud_cli/core/workspace.py` & `dagster-cloud-cli-1.7.1/dagster_cloud_cli/core/workspace.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.0/dagster_cloud_cli/docker_utils.py` & `dagster-cloud-cli-1.7.1/dagster_cloud_cli/docker_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.0/dagster_cloud_cli/entrypoint.py` & `dagster-cloud-cli-1.7.1/dagster_cloud_cli/entrypoint.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.0/dagster_cloud_cli/gql.py` & `dagster-cloud-cli-1.7.1/dagster_cloud_cli/gql.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.0/dagster_cloud_cli/pex_utils.py` & `dagster-cloud-cli-1.7.1/dagster_cloud_cli/pex_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.0/dagster_cloud_cli/types.py` & `dagster-cloud-cli-1.7.1/dagster_cloud_cli/types.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.0/dagster_cloud_cli/ui.py` & `dagster-cloud-cli-1.7.1/dagster_cloud_cli/ui.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.0/dagster_cloud_cli/utils.py` & `dagster-cloud-cli-1.7.1/dagster_cloud_cli/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.0/dagster_cloud_cli.egg-info/SOURCES.txt` & `dagster-cloud-cli-1.7.1/dagster_cloud_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.0/dagster_cloud_cli_tests/test_check.py` & `dagster-cloud-cli-1.7.1/dagster_cloud_cli_tests/test_check.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.0/dagster_cloud_cli_tests/test_ci_commands.py` & `dagster-cloud-cli-1.7.1/dagster_cloud_cli_tests/test_ci_commands.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,14 +83,15 @@
                     "build_config": None,
                     "commit_hash": "hash-1234",
                     "git_url": "http://some-git-url",
                 },
                 "build_output": None,
                 "location_name": "a",
                 "deployment_name": "prod",
+                "is_branch_deployment": False,
                 "location_file": f"{project_dir}/dagster_cloud.yaml",
                 "selected": True,
                 "url": "https://some-org.dagster.cloud",
                 "history": [{"log": "initialized", "status": "pending", "timestamp": "-"}],
                 "status_url": "http://github/run-url",
             }
```

### Comparing `dagster-cloud-cli-1.7.0/dagster_cloud_cli_tests/test_gql.py` & `dagster-cloud-cli-1.7.1/dagster_cloud_cli_tests/test_gql.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.0/dagster_cloud_cli_tests/test_metrics.py` & `dagster-cloud-cli-1.7.1/dagster_cloud_cli_tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.0/setup.py` & `dagster-cloud-cli-1.7.1/setup.py`

 * *Files identical despite different names*

