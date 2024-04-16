# Comparing `tmp/dagster-cloud-cli-1.7.1.tar.gz` & `tmp/dagster-cloud-cli-1.7.2rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-cloud-cli-1.7.1.tar", last modified: Thu Apr 11 18:18:55 2024, max compression
+gzip compressed data, was "dagster-cloud-cli-1.7.2rc1.tar", last modified: Tue Apr 16 18:02:17 2024, max compression
```

## Comparing `dagster-cloud-cli-1.7.1.tar` & `dagster-cloud-cli-1.7.2rc1.tar`

### file list

```diff
@@ -1,92 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:18:55.119890 dagster-cloud-cli-1.7.1/
--rw-r--r--   0 root         (0) root         (0)      132 2024-04-11 18:04:43.000000 dagster-cloud-cli-1.7.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      314 2024-04-11 18:18:55.119890 dagster-cloud-cli-1.7.1/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:18:55.083890 dagster-cloud-cli-1.7.1/dagster_cloud_cli/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 18:04:43.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:18:55.087890 dagster-cloud-cli-1.7.1/dagster_cloud_cli/commands/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 18:04:43.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli/commands/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:18:55.087890 dagster-cloud-cli-1.7.1/dagster_cloud_cli/commands/branch_deployment/
--rw-r--r--   0 root         (0) root         (0)     4947 2024-04-11 18:04:43.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli/commands/branch_deployment/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:18:55.091890 dagster-cloud-cli-1.7.1/dagster_cloud_cli/commands/ci/
--rw-r--r--   0 root         (0) root         (0)    29688 2024-04-11 18:04:43.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli/commands/ci/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4124 2024-04-11 18:04:43.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli/commands/ci/checks.py
--rw-r--r--   0 root         (0) root         (0)     1872 2024-04-11 18:04:43.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli/commands/ci/report.py
--rw-r--r--   0 root         (0) root         (0)     4121 2024-04-11 18:04:43.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli/commands/ci/state.py
--rw-r--r--   0 root         (0) root         (0)      508 2024-04-11 18:04:43.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli/commands/ci/utils.py
--rw-r--r--   0 root         (0) root         (0)     8651 2024-04-11 18:04:43.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli/commands/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:18:55.091890 dagster-cloud-cli-1.7.1/dagster_cloud_cli/commands/deployment/
--rw-r--r--   0 root         (0) root         (0)     2952 2024-04-11 18:04:43.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli/commands/deployment/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:18:55.091890 dagster-cloud-cli-1.7.1/dagster_cloud_cli/commands/deployment/alert_policies/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 18:04:43.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli/commands/deployment/alert_policies/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1634 2024-04-11 18:04:43.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli/commands/deployment/alert_policies/commands.py
--rw-r--r--   0 root         (0) root         (0)    17056 2024-04-11 18:04:43.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli/commands/deployment/alert_policies/config_schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:18:55.091890 dagster-cloud-cli-1.7.1/dagster_cloud_cli/commands/job/
--rw-r--r--   0 root         (0) root         (0)     1926 2024-04-11 18:04:43.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli/commands/job/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4425 2024-04-11 18:04:43.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli/commands/metrics.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:18:55.091890 dagster-cloud-cli-1.7.1/dagster_cloud_cli/commands/organization/
--rw-r--r--   0 root         (0) root         (0)     4001 2024-04-11 18:04:43.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli/commands/organization/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:18:55.095890 dagster-cloud-cli-1.7.1/dagster_cloud_cli/commands/organization/saml/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 18:04:43.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli/commands/organization/saml/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2691 2024-04-11 18:04:43.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli/commands/organization/saml/commands.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:18:55.095890 dagster-cloud-cli-1.7.1/dagster_cloud_cli/commands/run/
--rw-r--r--   0 root         (0) root         (0)      669 2024-04-11 18:04:43.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli/commands/run/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:18:55.095890 dagster-cloud-cli-1.7.1/dagster_cloud_cli/commands/serverless/
--rw-r--r--   0 root         (0) root         (0)     1499 2024-04-11 18:04:43.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli/commands/serverless/Dockerfile
--rw-r--r--   0 root         (0) root         (0)      628 2024-04-11 18:04:43.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli/commands/serverless/Dockerfile.dagster-cloud-cli
--rw-r--r--   0 root         (0) root         (0)    18361 2024-04-11 18:04:43.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli/commands/serverless/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:18:55.095890 dagster-cloud-cli-1.7.1/dagster_cloud_cli/commands/workspace/
--rw-r--r--   0 root         (0) root         (0)    12434 2024-04-11 18:04:43.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli/commands/workspace/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18301 2024-04-11 18:04:43.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli/config_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:18:55.103890 dagster-cloud-cli-1.7.1/dagster_cloud_cli/core/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 18:04:43.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)      901 2024-04-11 18:04:43.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli/core/alert_types.py
--rw-r--r--   0 root         (0) root         (0)     4801 2024-04-11 18:04:43.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli/core/artifacts.py
--rw-r--r--   0 root         (0) root         (0)     1744 2024-04-11 18:04:43.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli/core/docker_runner.py
--rw-r--r--   0 root         (0) root         (0)     1131 2024-04-11 18:04:43.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli/core/errors.py
--rw-r--r--   0 root         (0) root         (0)    12940 2024-04-11 18:04:43.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli/core/graphql_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:18:55.103890 dagster-cloud-cli-1.7.1/dagster_cloud_cli/core/headers/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 18:04:43.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli/core/headers/__init__.py
--rw-r--r--   0 root         (0) root         (0)      376 2024-04-11 18:04:43.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli/core/headers/auth.py
--rw-r--r--   0 root         (0) root         (0)      924 2024-04-11 18:04:43.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli/core/headers/impl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:18:55.103890 dagster-cloud-cli-1.7.1/dagster_cloud_cli/core/headers/versioning/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 18:04:43.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli/core/headers/versioning/__init__.py
--rw-r--r--   0 root         (0) root         (0)       96 2024-04-11 18:04:43.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli/core/headers/versioning/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:18:55.115890 dagster-cloud-cli-1.7.1/dagster_cloud_cli/core/pex_builder/
--rw-r--r--   0 root         (0) root         (0)      172 2024-04-11 18:04:43.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli/core/pex_builder/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1680 2024-04-11 18:04:43.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli/core/pex_builder/code_location.py
--rw-r--r--   0 root         (0) root         (0)     9423 2024-04-11 18:04:43.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli/core/pex_builder/deploy.py
--rw-r--r--   0 root         (0) root         (0)    13814 2024-04-11 18:04:43.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli/core/pex_builder/deps.py
--rw-r--r--   0 root         (0) root         (0)      949 2024-04-11 18:04:43.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli/core/pex_builder/git_context.py
--rw-r--r--   0 root         (0) root         (0)     6992 2024-04-11 18:04:43.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli/core/pex_builder/github_context.py
--rw-r--r--   0 root         (0) root         (0)     1063 2024-04-11 18:04:43.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli/core/pex_builder/gitlab_context.py
--rw-r--r--   0 root         (0) root         (0)     1232 2024-04-11 18:04:43.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli/core/pex_builder/parse_workspace.py
--rw-r--r--   0 root         (0) root         (0)     4655 2024-04-11 18:04:43.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli/core/pex_builder/pex_registry.py
--rw-r--r--   0 root         (0) root         (0)      709 2024-04-11 18:04:43.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli/core/pex_builder/selftest.py
--rw-r--r--   0 root         (0) root         (0)     5407 2024-04-11 18:04:43.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli/core/pex_builder/source.py
--rw-r--r--   0 root         (0) root         (0)     6220 2024-04-11 18:04:43.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli/core/pex_builder/util.py
--rw-r--r--   0 root         (0) root         (0)     2123 2024-04-11 18:04:43.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli/core/pydantic_yaml.py
--rw-r--r--   0 root         (0) root         (0)     7106 2024-04-11 18:04:43.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli/core/workspace.py
--rw-r--r--   0 root         (0) root         (0)     2463 2024-04-11 18:04:43.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli/docker_utils.py
--rw-r--r--   0 root         (0) root         (0)     6708 2024-04-11 18:04:43.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli/entrypoint.py
--rw-r--r--   0 root         (0) root         (0)    21075 2024-04-11 18:04:43.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli/gql.py
--rw-r--r--   0 root         (0) root         (0)     5859 2024-04-11 18:04:43.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli/pex_utils.py
--rw-r--r--   0 root         (0) root         (0)     1845 2024-04-11 18:04:43.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli/types.py
--rw-r--r--   0 root         (0) root         (0)     2804 2024-04-11 18:04:43.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli/ui.py
--rw-r--r--   0 root         (0) root         (0)     3488 2024-04-11 18:04:43.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli/utils.py
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-11 18:04:43.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:18:55.083890 dagster-cloud-cli-1.7.1/dagster_cloud_cli.egg-info/
--rw-r--r--   0 root         (0) root         (0)      314 2024-04-11 18:18:54.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2991 2024-04-11 18:18:54.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-11 18:18:54.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       67 2024-04-11 18:18:54.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       97 2024-04-11 18:18:54.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       42 2024-04-11 18:18:54.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:18:55.119890 dagster-cloud-cli-1.7.1/dagster_cloud_cli_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 18:04:43.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)      189 2024-04-11 18:04:43.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli_tests/conftest.py
--rw-r--r--   0 root         (0) root         (0)     4130 2024-04-11 18:04:43.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli_tests/test_check.py
--rw-r--r--   0 root         (0) root         (0)    16177 2024-04-11 18:04:43.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli_tests/test_ci_commands.py
--rw-r--r--   0 root         (0) root         (0)      683 2024-04-11 18:04:43.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli_tests/test_gql.py
--rw-r--r--   0 root         (0) root         (0)     8872 2024-04-11 18:04:43.000000 dagster-cloud-cli-1.7.1/dagster_cloud_cli_tests/test_metrics.py
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-11 18:18:55.119890 dagster-cloud-cli-1.7.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1139 2024-04-11 18:04:43.000000 dagster-cloud-cli-1.7.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 18:02:17.172550 dagster-cloud-cli-1.7.2rc1/
+-rw-r--r--   0 root         (0) root         (0)      317 2024-04-16 18:02:17.172550 dagster-cloud-cli-1.7.2rc1/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 18:02:17.172550 dagster-cloud-cli-1.7.2rc1/dagster_cloud_cli.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      317 2024-04-16 18:02:16.000000 dagster-cloud-cli-1.7.2rc1/dagster_cloud_cli.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      256 2024-04-16 18:02:17.000000 dagster-cloud-cli-1.7.2rc1/dagster_cloud_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-16 18:02:16.000000 dagster-cloud-cli-1.7.2rc1/dagster_cloud_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       66 2024-04-16 18:02:16.000000 dagster-cloud-cli-1.7.2rc1/dagster_cloud_cli.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       70 2024-04-16 18:02:16.000000 dagster-cloud-cli-1.7.2rc1/dagster_cloud_cli.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-16 18:02:16.000000 dagster-cloud-cli-1.7.2rc1/dagster_cloud_cli.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-16 18:02:17.172550 dagster-cloud-cli-1.7.2rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1042 2024-04-16 17:50:53.000000 dagster-cloud-cli-1.7.2rc1/setup.py
```

### Comparing `dagster-cloud-cli-1.7.1/setup.py` & `dagster-cloud-cli-1.7.2rc1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,39 +8,28 @@
     version: Dict[str, str] = {}
     with open(Path(__file__).parent / "dagster_cloud_cli/version.py", encoding="utf8") as fp:
         exec(fp.read(), version)
 
     return version["__version__"]
 
 
+ver = get_version()
+pin = "" if ver == "1!0+dev" else f"=={ver}"
 setup(
     name="dagster-cloud-cli",
     version=get_version(),
     author_email="hello@elementl.com",
     packages=find_packages(exclude=["dagster_cloud.cli_tests*"]),
     include_package_data=True,
-    install_requires=[
-        "packaging>=20.9",
-        "questionary",
-        "requests",
-        "typer[all]>=0.4.1",
-        "PyYAML>=5.1",
-        "github3.py",
-    ],
+    install_requires=["dagster-plus-cli==1.7.2rc1"],
     extras_require={
-        "tests": [
-            "freezegun",
-        ],
+        "tests": [f"dagster-plus-cli[tests]{pin}"],
     },
     author="Elementl",
     license="Apache-2.0",
     classifiers=[
         "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
-    entry_points={
-        "console_scripts": [
-            "dagster-cloud = dagster_cloud_cli.entrypoint:app",
-        ]
-    },
+    entry_points={"console_scripts": ["dagster-cloud = dagster_plus_cli.entrypoint:app"]},
 )
```

