# Comparing `tmp/dagster-plus-cli-0.0.1.tar.gz` & `tmp/dagster-plus-cli-1.7.2rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-plus-cli-0.0.1.tar", last modified: Tue Apr  2 22:35:54 2024, max compression
+gzip compressed data, was "dagster-plus-cli-1.7.2rc1.tar", last modified: Tue Apr 16 18:02:22 2024, max compression
```

## Comparing `dagster-plus-cli-0.0.1.tar` & `dagster-plus-cli-1.7.2rc1.tar`

### file list

```diff
@@ -1,14 +1,92 @@
-drwxr-xr-x   0 claire     (501) staff       (20)        0 2024-04-02 22:35:54.907737 dagster-plus-cli-0.0.1/
--rw-r--r--   0 claire     (501) staff       (20)       89 2024-04-02 22:05:03.000000 dagster-plus-cli-0.0.1/LICENSE.md
--rw-r--r--   0 claire     (501) staff       (20)      445 2024-04-02 22:35:54.907375 dagster-plus-cli-0.0.1/PKG-INFO
--rw-r--r--   0 claire     (501) staff       (20)       53 2024-04-02 22:05:47.000000 dagster-plus-cli-0.0.1/README.md
-drwxr-xr-x   0 claire     (501) staff       (20)        0 2024-04-02 22:35:54.904663 dagster-plus-cli-0.0.1/dagster_plus_cli/
--rw-r--r--   0 claire     (501) staff       (20)        0 2024-04-02 22:06:04.000000 dagster-plus-cli-0.0.1/dagster_plus_cli/__init__.py
-drwxr-xr-x   0 claire     (501) staff       (20)        0 2024-04-02 22:35:54.906935 dagster-plus-cli-0.0.1/dagster_plus_cli.egg-info/
--rw-r--r--   0 claire     (501) staff       (20)      445 2024-04-02 22:35:54.000000 dagster-plus-cli-0.0.1/dagster_plus_cli.egg-info/PKG-INFO
--rw-r--r--   0 claire     (501) staff       (20)      263 2024-04-02 22:35:54.000000 dagster-plus-cli-0.0.1/dagster_plus_cli.egg-info/SOURCES.txt
--rw-r--r--   0 claire     (501) staff       (20)        1 2024-04-02 22:35:54.000000 dagster-plus-cli-0.0.1/dagster_plus_cli.egg-info/dependency_links.txt
--rw-r--r--   0 claire     (501) staff       (20)       18 2024-04-02 22:35:54.000000 dagster-plus-cli-0.0.1/dagster_plus_cli.egg-info/requires.txt
--rw-r--r--   0 claire     (501) staff       (20)       17 2024-04-02 22:35:54.000000 dagster-plus-cli-0.0.1/dagster_plus_cli.egg-info/top_level.txt
--rw-r--r--   0 claire     (501) staff       (20)      406 2024-04-02 22:06:48.000000 dagster-plus-cli-0.0.1/pyproject.toml
--rw-r--r--   0 claire     (501) staff       (20)       38 2024-04-02 22:35:54.907819 dagster-plus-cli-0.0.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 18:02:22.964562 dagster-plus-cli-1.7.2rc1/
+-rw-r--r--   0 root         (0) root         (0)      130 2024-04-16 17:50:53.000000 dagster-plus-cli-1.7.2rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      316 2024-04-16 18:02:22.964562 dagster-plus-cli-1.7.2rc1/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 18:02:22.952562 dagster-plus-cli-1.7.2rc1/dagster_plus_cli/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-16 17:50:53.000000 dagster-plus-cli-1.7.2rc1/dagster_plus_cli/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 18:02:22.952562 dagster-plus-cli-1.7.2rc1/dagster_plus_cli/commands/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-16 17:50:53.000000 dagster-plus-cli-1.7.2rc1/dagster_plus_cli/commands/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 18:02:22.952562 dagster-plus-cli-1.7.2rc1/dagster_plus_cli/commands/branch_deployment/
+-rw-r--r--   0 root         (0) root         (0)     4947 2024-04-16 17:50:53.000000 dagster-plus-cli-1.7.2rc1/dagster_plus_cli/commands/branch_deployment/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 18:02:22.952562 dagster-plus-cli-1.7.2rc1/dagster_plus_cli/commands/ci/
+-rw-r--r--   0 root         (0) root         (0)    29680 2024-04-16 17:50:53.000000 dagster-plus-cli-1.7.2rc1/dagster_plus_cli/commands/ci/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4122 2024-04-16 17:50:53.000000 dagster-plus-cli-1.7.2rc1/dagster_plus_cli/commands/ci/checks.py
+-rw-r--r--   0 root         (0) root         (0)     1872 2024-04-16 17:50:53.000000 dagster-plus-cli-1.7.2rc1/dagster_plus_cli/commands/ci/report.py
+-rw-r--r--   0 root         (0) root         (0)     4120 2024-04-16 17:50:53.000000 dagster-plus-cli-1.7.2rc1/dagster_plus_cli/commands/ci/state.py
+-rw-r--r--   0 root         (0) root         (0)      507 2024-04-16 17:50:53.000000 dagster-plus-cli-1.7.2rc1/dagster_plus_cli/commands/ci/utils.py
+-rw-r--r--   0 root         (0) root         (0)     8651 2024-04-16 17:50:53.000000 dagster-plus-cli-1.7.2rc1/dagster_plus_cli/commands/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 18:02:22.952562 dagster-plus-cli-1.7.2rc1/dagster_plus_cli/commands/deployment/
+-rw-r--r--   0 root         (0) root         (0)     2952 2024-04-16 17:50:53.000000 dagster-plus-cli-1.7.2rc1/dagster_plus_cli/commands/deployment/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 18:02:22.956562 dagster-plus-cli-1.7.2rc1/dagster_plus_cli/commands/deployment/alert_policies/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-16 17:50:53.000000 dagster-plus-cli-1.7.2rc1/dagster_plus_cli/commands/deployment/alert_policies/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1657 2024-04-16 17:50:53.000000 dagster-plus-cli-1.7.2rc1/dagster_plus_cli/commands/deployment/alert_policies/commands.py
+-rw-r--r--   0 root         (0) root         (0)    17055 2024-04-16 17:50:53.000000 dagster-plus-cli-1.7.2rc1/dagster_plus_cli/commands/deployment/alert_policies/config_schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 18:02:22.956562 dagster-plus-cli-1.7.2rc1/dagster_plus_cli/commands/job/
+-rw-r--r--   0 root         (0) root         (0)     1926 2024-04-16 17:50:53.000000 dagster-plus-cli-1.7.2rc1/dagster_plus_cli/commands/job/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4422 2024-04-16 17:50:53.000000 dagster-plus-cli-1.7.2rc1/dagster_plus_cli/commands/metrics.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 18:02:22.956562 dagster-plus-cli-1.7.2rc1/dagster_plus_cli/commands/organization/
+-rw-r--r--   0 root         (0) root         (0)     4001 2024-04-16 17:50:53.000000 dagster-plus-cli-1.7.2rc1/dagster_plus_cli/commands/organization/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 18:02:22.956562 dagster-plus-cli-1.7.2rc1/dagster_plus_cli/commands/organization/saml/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-16 17:50:53.000000 dagster-plus-cli-1.7.2rc1/dagster_plus_cli/commands/organization/saml/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2691 2024-04-16 17:50:53.000000 dagster-plus-cli-1.7.2rc1/dagster_plus_cli/commands/organization/saml/commands.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 18:02:22.956562 dagster-plus-cli-1.7.2rc1/dagster_plus_cli/commands/run/
+-rw-r--r--   0 root         (0) root         (0)      669 2024-04-16 17:50:53.000000 dagster-plus-cli-1.7.2rc1/dagster_plus_cli/commands/run/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 18:02:22.956562 dagster-plus-cli-1.7.2rc1/dagster_plus_cli/commands/serverless/
+-rw-r--r--   0 root         (0) root         (0)     1525 2024-04-16 17:50:53.000000 dagster-plus-cli-1.7.2rc1/dagster_plus_cli/commands/serverless/Dockerfile
+-rw-r--r--   0 root         (0) root         (0)      628 2024-04-16 17:50:53.000000 dagster-plus-cli-1.7.2rc1/dagster_plus_cli/commands/serverless/Dockerfile.dagster-cloud-cli
+-rw-r--r--   0 root         (0) root         (0)    18354 2024-04-16 17:50:53.000000 dagster-plus-cli-1.7.2rc1/dagster_plus_cli/commands/serverless/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 18:02:22.956562 dagster-plus-cli-1.7.2rc1/dagster_plus_cli/commands/workspace/
+-rw-r--r--   0 root         (0) root         (0)    12429 2024-04-16 17:50:53.000000 dagster-plus-cli-1.7.2rc1/dagster_plus_cli/commands/workspace/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18301 2024-04-16 17:50:53.000000 dagster-plus-cli-1.7.2rc1/dagster_plus_cli/config_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 18:02:22.956562 dagster-plus-cli-1.7.2rc1/dagster_plus_cli/core/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-16 17:50:53.000000 dagster-plus-cli-1.7.2rc1/dagster_plus_cli/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      901 2024-04-16 17:50:53.000000 dagster-plus-cli-1.7.2rc1/dagster_plus_cli/core/alert_types.py
+-rw-r--r--   0 root         (0) root         (0)     4797 2024-04-16 17:50:53.000000 dagster-plus-cli-1.7.2rc1/dagster_plus_cli/core/artifacts.py
+-rw-r--r--   0 root         (0) root         (0)     1743 2024-04-16 17:50:53.000000 dagster-plus-cli-1.7.2rc1/dagster_plus_cli/core/docker_runner.py
+-rw-r--r--   0 root         (0) root         (0)     1131 2024-04-16 17:50:53.000000 dagster-plus-cli-1.7.2rc1/dagster_plus_cli/core/errors.py
+-rw-r--r--   0 root         (0) root         (0)    12940 2024-04-16 17:50:53.000000 dagster-plus-cli-1.7.2rc1/dagster_plus_cli/core/graphql_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 18:02:22.960562 dagster-plus-cli-1.7.2rc1/dagster_plus_cli/core/headers/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-16 17:50:53.000000 dagster-plus-cli-1.7.2rc1/dagster_plus_cli/core/headers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      376 2024-04-16 17:50:53.000000 dagster-plus-cli-1.7.2rc1/dagster_plus_cli/core/headers/auth.py
+-rw-r--r--   0 root         (0) root         (0)      924 2024-04-16 17:50:53.000000 dagster-plus-cli-1.7.2rc1/dagster_plus_cli/core/headers/impl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 18:02:22.960562 dagster-plus-cli-1.7.2rc1/dagster_plus_cli/core/headers/versioning/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-16 17:50:53.000000 dagster-plus-cli-1.7.2rc1/dagster_plus_cli/core/headers/versioning/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       96 2024-04-16 17:50:53.000000 dagster-plus-cli-1.7.2rc1/dagster_plus_cli/core/headers/versioning/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 18:02:22.960562 dagster-plus-cli-1.7.2rc1/dagster_plus_cli/core/pex_builder/
+-rw-r--r--   0 root         (0) root         (0)      172 2024-04-16 17:50:53.000000 dagster-plus-cli-1.7.2rc1/dagster_plus_cli/core/pex_builder/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1679 2024-04-16 17:50:53.000000 dagster-plus-cli-1.7.2rc1/dagster_plus_cli/core/pex_builder/code_location.py
+-rw-r--r--   0 root         (0) root         (0)     9422 2024-04-16 17:50:53.000000 dagster-plus-cli-1.7.2rc1/dagster_plus_cli/core/pex_builder/deploy.py
+-rw-r--r--   0 root         (0) root         (0)    13812 2024-04-16 17:50:53.000000 dagster-plus-cli-1.7.2rc1/dagster_plus_cli/core/pex_builder/deps.py
+-rw-r--r--   0 root         (0) root         (0)      949 2024-04-16 17:50:53.000000 dagster-plus-cli-1.7.2rc1/dagster_plus_cli/core/pex_builder/git_context.py
+-rw-r--r--   0 root         (0) root         (0)     6992 2024-04-16 17:50:53.000000 dagster-plus-cli-1.7.2rc1/dagster_plus_cli/core/pex_builder/github_context.py
+-rw-r--r--   0 root         (0) root         (0)     1063 2024-04-16 17:50:53.000000 dagster-plus-cli-1.7.2rc1/dagster_plus_cli/core/pex_builder/gitlab_context.py
+-rw-r--r--   0 root         (0) root         (0)     1232 2024-04-16 17:50:53.000000 dagster-plus-cli-1.7.2rc1/dagster_plus_cli/core/pex_builder/parse_workspace.py
+-rw-r--r--   0 root         (0) root         (0)     4654 2024-04-16 17:50:53.000000 dagster-plus-cli-1.7.2rc1/dagster_plus_cli/core/pex_builder/pex_registry.py
+-rw-r--r--   0 root         (0) root         (0)      709 2024-04-16 17:50:53.000000 dagster-plus-cli-1.7.2rc1/dagster_plus_cli/core/pex_builder/selftest.py
+-rw-r--r--   0 root         (0) root         (0)     5406 2024-04-16 17:50:53.000000 dagster-plus-cli-1.7.2rc1/dagster_plus_cli/core/pex_builder/source.py
+-rw-r--r--   0 root         (0) root         (0)     6219 2024-04-16 17:50:53.000000 dagster-plus-cli-1.7.2rc1/dagster_plus_cli/core/pex_builder/util.py
+-rw-r--r--   0 root         (0) root         (0)     2123 2024-04-16 17:50:53.000000 dagster-plus-cli-1.7.2rc1/dagster_plus_cli/core/pydantic_yaml.py
+-rw-r--r--   0 root         (0) root         (0)     7105 2024-04-16 17:50:53.000000 dagster-plus-cli-1.7.2rc1/dagster_plus_cli/core/workspace.py
+-rw-r--r--   0 root         (0) root         (0)     2461 2024-04-16 17:50:53.000000 dagster-plus-cli-1.7.2rc1/dagster_plus_cli/docker_utils.py
+-rw-r--r--   0 root         (0) root         (0)     6770 2024-04-16 17:50:53.000000 dagster-plus-cli-1.7.2rc1/dagster_plus_cli/entrypoint.py
+-rw-r--r--   0 root         (0) root         (0)    20455 2024-04-16 17:50:53.000000 dagster-plus-cli-1.7.2rc1/dagster_plus_cli/gql.py
+-rw-r--r--   0 root         (0) root         (0)     5855 2024-04-16 17:50:53.000000 dagster-plus-cli-1.7.2rc1/dagster_plus_cli/pex_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1845 2024-04-16 17:50:53.000000 dagster-plus-cli-1.7.2rc1/dagster_plus_cli/types.py
+-rw-r--r--   0 root         (0) root         (0)     2804 2024-04-16 17:50:53.000000 dagster-plus-cli-1.7.2rc1/dagster_plus_cli/ui.py
+-rw-r--r--   0 root         (0) root         (0)     3487 2024-04-16 17:50:53.000000 dagster-plus-cli-1.7.2rc1/dagster_plus_cli/utils.py
+-rw-r--r--   0 root         (0) root         (0)       25 2024-04-16 17:50:53.000000 dagster-plus-cli-1.7.2rc1/dagster_plus_cli/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 18:02:22.952562 dagster-plus-cli-1.7.2rc1/dagster_plus_cli.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      316 2024-04-16 18:02:22.000000 dagster-plus-cli-1.7.2rc1/dagster_plus_cli.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2922 2024-04-16 18:02:22.000000 dagster-plus-cli-1.7.2rc1/dagster_plus_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-16 18:02:22.000000 dagster-plus-cli-1.7.2rc1/dagster_plus_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      113 2024-04-16 18:02:22.000000 dagster-plus-cli-1.7.2rc1/dagster_plus_cli.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       97 2024-04-16 18:02:22.000000 dagster-plus-cli-1.7.2rc1/dagster_plus_cli.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       40 2024-04-16 18:02:22.000000 dagster-plus-cli-1.7.2rc1/dagster_plus_cli.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 18:02:22.964562 dagster-plus-cli-1.7.2rc1/dagster_plus_cli_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-16 17:50:53.000000 dagster-plus-cli-1.7.2rc1/dagster_plus_cli_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      189 2024-04-16 17:50:53.000000 dagster-plus-cli-1.7.2rc1/dagster_plus_cli_tests/conftest.py
+-rw-r--r--   0 root         (0) root         (0)     4128 2024-04-16 17:50:53.000000 dagster-plus-cli-1.7.2rc1/dagster_plus_cli_tests/test_check.py
+-rw-r--r--   0 root         (0) root         (0)    16161 2024-04-16 17:50:53.000000 dagster-plus-cli-1.7.2rc1/dagster_plus_cli_tests/test_ci_commands.py
+-rw-r--r--   0 root         (0) root         (0)      681 2024-04-16 17:50:53.000000 dagster-plus-cli-1.7.2rc1/dagster_plus_cli_tests/test_gql.py
+-rw-r--r--   0 root         (0) root         (0)     8864 2024-04-16 17:50:53.000000 dagster-plus-cli-1.7.2rc1/dagster_plus_cli_tests/test_metrics.py
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-16 18:02:22.964562 dagster-plus-cli-1.7.2rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1197 2024-04-16 17:50:53.000000 dagster-plus-cli-1.7.2rc1/setup.py
```

