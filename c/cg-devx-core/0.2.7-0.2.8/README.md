# Comparing `tmp/cg_devx_core-0.2.7.tar.gz` & `tmp/cg_devx_core-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cg_devx_core-0.2.7.tar", max compression
+gzip compressed data, was "cg_devx_core-0.2.8.tar", max compression
```

## Comparing `cg_devx_core-0.2.7.tar` & `cg_devx_core-0.2.8.tar`

### file list

```diff
@@ -1,76 +1,76 @@
--rw-r--r--   0        0        0     2645 2024-04-16 09:59:04.186564 cg_devx_core-0.2.7/README.md
--rw-r--r--   0        0        0      497 2024-04-16 09:59:04.186564 cg_devx_core-0.2.7/cli/.flake8
--rw-r--r--   0        0        0       83 2024-04-16 09:59:04.186564 cg_devx_core-0.2.7/cli/__init__.py
--rw-r--r--   0        0        0      366 2024-04-16 09:59:04.186564 cg_devx_core-0.2.7/cli/__main__.py
--rw-r--r--   0        0        0     1217 2024-04-16 09:59:04.186564 cg_devx_core-0.2.7/cli/build.py
--rw-r--r--   0        0        0     7224 2024-04-16 09:59:04.186564 cg_devx_core-0.2.7/cli/commands/README.md
--rw-r--r--   0        0        0        0 2024-04-16 09:59:04.186564 cg_devx_core-0.2.7/cli/commands/__init__.py
--rw-r--r--   0        0        0     6138 2024-04-16 09:59:04.186564 cg_devx_core-0.2.7/cli/commands/destroy.py
--rw-r--r--   0        0        0    48324 2024-04-16 09:59:04.186564 cg_devx_core-0.2.7/cli/commands/setup.py
--rw-r--r--   0        0        0     7816 2024-04-16 09:59:04.186564 cg_devx_core-0.2.7/cli/commands/workload/README.md
--rw-r--r--   0        0        0        0 2024-04-16 09:59:04.186564 cg_devx_core-0.2.7/cli/commands/workload/__init__.py
--rw-r--r--   0        0        0    15215 2024-04-16 09:59:04.186564 cg_devx_core-0.2.7/cli/commands/workload/bootstrap.py
--rw-r--r--   0        0        0     4398 2024-04-16 09:59:04.186564 cg_devx_core-0.2.7/cli/commands/workload/create.py
--rw-r--r--   0        0        0     8962 2024-04-16 09:59:04.186564 cg_devx_core-0.2.7/cli/commands/workload/delete.py
--rw-r--r--   0        0        0      235 2024-04-16 09:59:04.186564 cg_devx_core-0.2.7/cli/commands/workload/workload.py
--rw-r--r--   0        0        0        0 2024-04-16 09:59:04.186564 cg_devx_core-0.2.7/cli/common/__init__.py
--rw-r--r--   0        0        0        0 2024-04-16 09:59:04.186564 cg_devx_core-0.2.7/cli/common/const/__init__.py
--rw-r--r--   0        0        0      903 2024-04-16 09:59:04.186564 cg_devx_core-0.2.7/cli/common/const/common_path.py
--rw-r--r--   0        0        0     1007 2024-04-16 09:59:04.186564 cg_devx_core-0.2.7/cli/common/const/const.py
--rw-r--r--   0        0        0      247 2024-04-16 09:59:04.186564 cg_devx_core-0.2.7/cli/common/const/namespaces.py
--rw-r--r--   0        0        0      767 2024-04-16 09:59:04.186564 cg_devx_core-0.2.7/cli/common/const/parameter_names.py
--rw-r--r--   0        0        0     1006 2024-04-16 09:59:04.186564 cg_devx_core-0.2.7/cli/common/custom_excpetions.py
--rw-r--r--   0        0        0        0 2024-04-16 09:59:04.186564 cg_devx_core-0.2.7/cli/common/enums/__init__.py
--rw-r--r--   0        0        0      787 2024-04-16 09:59:04.186564 cg_devx_core-0.2.7/cli/common/enums/cloud_providers.py
--rw-r--r--   0        0        0      799 2024-04-16 09:59:04.186564 cg_devx_core-0.2.7/cli/common/enums/dns_registrars.py
--rw-r--r--   0        0        0      263 2024-04-16 09:59:04.186564 cg_devx_core-0.2.7/cli/common/enums/git_plans.py
--rw-r--r--   0        0        0      788 2024-04-16 09:59:04.186564 cg_devx_core-0.2.7/cli/common/enums/git_providers.py
--rw-r--r--   0        0        0     1779 2024-04-16 09:59:04.186564 cg_devx_core-0.2.7/cli/common/logging_config.py
--rw-r--r--   0        0        0      830 2024-04-16 09:59:04.186564 cg_devx_core-0.2.7/cli/common/retry_decorator.py
--rw-r--r--   0        0        0      307 2024-04-16 09:59:04.186564 cg_devx_core-0.2.7/cli/common/singleton_metaclass.py
--rw-r--r--   0        0        0     3574 2024-04-16 09:59:04.186564 cg_devx_core-0.2.7/cli/common/state_store.py
--rw-r--r--   0        0        0     1258 2024-04-16 09:59:04.186564 cg_devx_core-0.2.7/cli/common/tracing_decorator.py
--rw-r--r--   0        0        0        0 2024-04-16 09:59:04.186564 cg_devx_core-0.2.7/cli/common/utils/__init__.py
--rw-r--r--   0        0        0    12697 2024-04-16 09:59:04.186564 cg_devx_core-0.2.7/cli/common/utils/command_utils.py
--rw-r--r--   0        0        0      314 2024-04-16 09:59:04.186564 cg_devx_core-0.2.7/cli/common/utils/generators.py
--rw-r--r--   0        0        0      187 2024-04-16 09:59:04.186564 cg_devx_core-0.2.7/cli/common/utils/os_utils.py
--rw-r--r--   0        0        0      532 2024-04-16 09:59:04.190564 cg_devx_core-0.2.7/cli/services/README.md
--rw-r--r--   0        0        0        0 2024-04-16 09:59:04.190564 cg_devx_core-0.2.7/cli/services/__init__.py
--rw-r--r--   0        0        0        0 2024-04-16 09:59:04.190564 cg_devx_core-0.2.7/cli/services/cloud/__init__.py
--rw-r--r--   0        0        0        0 2024-04-16 09:59:04.190564 cg_devx_core-0.2.7/cli/services/cloud/aws/__init__.py
--rw-r--r--   0        0        0     6482 2024-04-16 09:59:04.190564 cg_devx_core-0.2.7/cli/services/cloud/aws/aws_manager.py
--rw-r--r--   0        0        0    11353 2024-04-16 09:59:04.190564 cg_devx_core-0.2.7/cli/services/cloud/aws/aws_sdk.py
--rw-r--r--   0        0        0      932 2024-04-16 09:59:04.190564 cg_devx_core-0.2.7/cli/services/cloud/aws/aws_session_manager.py
--rw-r--r--   0        0        0     5126 2024-04-16 09:59:04.190564 cg_devx_core-0.2.7/cli/services/cloud/aws/iam_permissions.py
--rw-r--r--   0        0        0        0 2024-04-16 09:59:04.190564 cg_devx_core-0.2.7/cli/services/cloud/azure/__init__.py
--rw-r--r--   0        0        0    11546 2024-04-16 09:59:04.190564 cg_devx_core-0.2.7/cli/services/cloud/azure/azure_manager.py
--rw-r--r--   0        0        0    25095 2024-04-16 09:59:04.190564 cg_devx_core-0.2.7/cli/services/cloud/azure/azure_sdk.py
--rw-r--r--   0        0        0     5846 2024-04-16 09:59:04.190564 cg_devx_core-0.2.7/cli/services/cloud/azure/iam_permissions.py
--rw-r--r--   0        0        0     4460 2024-04-16 09:59:04.190564 cg_devx_core-0.2.7/cli/services/cloud/cloud_provider_manager.py
--rw-r--r--   0        0        0     6504 2024-04-16 09:59:04.190564 cg_devx_core-0.2.7/cli/services/dependency_manager.py
--rw-r--r--   0        0        0        0 2024-04-16 09:59:04.190564 cg_devx_core-0.2.7/cli/services/dns/__init__.py
--rw-r--r--   0        0        0        0 2024-04-16 09:59:04.190564 cg_devx_core-0.2.7/cli/services/dns/azure_dns/__init__.py
--rw-r--r--   0        0        0     1819 2024-04-16 09:59:04.190564 cg_devx_core-0.2.7/cli/services/dns/azure_dns/azure_dns.py
--rw-r--r--   0        0        0     2049 2024-04-16 09:59:04.190564 cg_devx_core-0.2.7/cli/services/dns/dns_provider_manager.py
--rw-r--r--   0        0        0        0 2024-04-16 09:59:04.190564 cg_devx_core-0.2.7/cli/services/dns/route53/__init__.py
--rw-r--r--   0        0        0     1788 2024-04-16 09:59:04.190564 cg_devx_core-0.2.7/cli/services/dns/route53/route53.py
--rw-r--r--   0        0        0        0 2024-04-16 09:59:04.190564 cg_devx_core-0.2.7/cli/services/k8s/__init__.py
--rw-r--r--   0        0        0     1271 2024-04-16 09:59:04.190564 cg_devx_core-0.2.7/cli/services/k8s/config_builder.py
--rw-r--r--   0        0        0     6622 2024-04-16 09:59:04.190564 cg_devx_core-0.2.7/cli/services/k8s/delivery_service_manager.py
--rw-r--r--   0        0        0    21428 2024-04-16 09:59:04.190564 cg_devx_core-0.2.7/cli/services/k8s/k8s.py
--rw-r--r--   0        0        0     2150 2024-04-16 09:59:04.190564 cg_devx_core-0.2.7/cli/services/k8s/kctl_wrapper.py
--rw-r--r--   0        0        0      461 2024-04-16 09:59:04.190564 cg_devx_core-0.2.7/cli/services/k8s/kubeconfig.yaml
--rw-r--r--   0        0        0        0 2024-04-16 09:59:04.190564 cg_devx_core-0.2.7/cli/services/keys/__init__.py
--rw-r--r--   0        0        0     2156 2024-04-16 09:59:04.190564 cg_devx_core-0.2.7/cli/services/keys/key_manager.py
--rw-r--r--   0        0        0     9269 2024-04-16 09:59:04.190564 cg_devx_core-0.2.7/cli/services/platform_gitops.py
--rw-r--r--   0        0        0     6121 2024-04-16 09:59:04.190564 cg_devx_core-0.2.7/cli/services/platform_template_manager.py
--rw-r--r--   0        0        0    15527 2024-04-16 09:59:04.190564 cg_devx_core-0.2.7/cli/services/tf_wrapper.py
--rw-r--r--   0        0        0        0 2024-04-16 09:59:04.190564 cg_devx_core-0.2.7/cli/services/vcs/__init__.py
--rw-r--r--   0        0        0     2025 2024-04-16 09:59:04.190564 cg_devx_core-0.2.7/cli/services/vcs/git_provider_manager.py
--rw-r--r--   0        0        0        0 2024-04-16 09:59:04.190564 cg_devx_core-0.2.7/cli/services/vcs/github/__init__.py
--rw-r--r--   0        0        0     5614 2024-04-16 09:59:04.190564 cg_devx_core-0.2.7/cli/services/vcs/github/github_manager.py
--rw-r--r--   0        0        0        0 2024-04-16 09:59:04.190564 cg_devx_core-0.2.7/cli/services/vcs/gitlab/__init__.py
--rw-r--r--   0        0        0     7767 2024-04-16 09:59:04.190564 cg_devx_core-0.2.7/cli/services/vcs/gitlab/gitlab_manager.py
--rw-r--r--   0        0        0    12262 2024-04-16 09:59:04.190564 cg_devx_core-0.2.7/cli/services/wl_template_manager.py
--rw-r--r--   0        0        0     1229 2024-04-16 09:59:20.354564 cg_devx_core-0.2.7/pyproject.toml
--rw-r--r--   0        0        0     4023 1970-01-01 00:00:00.000000 cg_devx_core-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0     2669 2024-04-16 12:11:02.594653 cg_devx_core-0.2.8/README.md
+-rw-r--r--   0        0        0      497 2024-04-16 12:11:02.594653 cg_devx_core-0.2.8/cli/.flake8
+-rw-r--r--   0        0        0       83 2024-04-16 12:11:02.594653 cg_devx_core-0.2.8/cli/__init__.py
+-rw-r--r--   0        0        0      366 2024-04-16 12:11:02.594653 cg_devx_core-0.2.8/cli/__main__.py
+-rw-r--r--   0        0        0     1217 2024-04-16 12:11:02.594653 cg_devx_core-0.2.8/cli/build.py
+-rw-r--r--   0        0        0     7224 2024-04-16 12:11:02.594653 cg_devx_core-0.2.8/cli/commands/README.md
+-rw-r--r--   0        0        0        0 2024-04-16 12:11:02.594653 cg_devx_core-0.2.8/cli/commands/__init__.py
+-rw-r--r--   0        0        0     6138 2024-04-16 12:11:02.594653 cg_devx_core-0.2.8/cli/commands/destroy.py
+-rw-r--r--   0        0        0    48324 2024-04-16 12:11:02.594653 cg_devx_core-0.2.8/cli/commands/setup.py
+-rw-r--r--   0        0        0     7816 2024-04-16 12:11:02.594653 cg_devx_core-0.2.8/cli/commands/workload/README.md
+-rw-r--r--   0        0        0        0 2024-04-16 12:11:02.594653 cg_devx_core-0.2.8/cli/commands/workload/__init__.py
+-rw-r--r--   0        0        0    15215 2024-04-16 12:11:02.594653 cg_devx_core-0.2.8/cli/commands/workload/bootstrap.py
+-rw-r--r--   0        0        0     4398 2024-04-16 12:11:02.594653 cg_devx_core-0.2.8/cli/commands/workload/create.py
+-rw-r--r--   0        0        0     8962 2024-04-16 12:11:02.594653 cg_devx_core-0.2.8/cli/commands/workload/delete.py
+-rw-r--r--   0        0        0      235 2024-04-16 12:11:02.594653 cg_devx_core-0.2.8/cli/commands/workload/workload.py
+-rw-r--r--   0        0        0        0 2024-04-16 12:11:02.594653 cg_devx_core-0.2.8/cli/common/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-16 12:11:02.594653 cg_devx_core-0.2.8/cli/common/const/__init__.py
+-rw-r--r--   0        0        0      903 2024-04-16 12:11:02.594653 cg_devx_core-0.2.8/cli/common/const/common_path.py
+-rw-r--r--   0        0        0     1007 2024-04-16 12:11:02.594653 cg_devx_core-0.2.8/cli/common/const/const.py
+-rw-r--r--   0        0        0      247 2024-04-16 12:11:02.594653 cg_devx_core-0.2.8/cli/common/const/namespaces.py
+-rw-r--r--   0        0        0      767 2024-04-16 12:11:02.594653 cg_devx_core-0.2.8/cli/common/const/parameter_names.py
+-rw-r--r--   0        0        0     1006 2024-04-16 12:11:02.594653 cg_devx_core-0.2.8/cli/common/custom_excpetions.py
+-rw-r--r--   0        0        0        0 2024-04-16 12:11:02.594653 cg_devx_core-0.2.8/cli/common/enums/__init__.py
+-rw-r--r--   0        0        0      787 2024-04-16 12:11:02.594653 cg_devx_core-0.2.8/cli/common/enums/cloud_providers.py
+-rw-r--r--   0        0        0      799 2024-04-16 12:11:02.594653 cg_devx_core-0.2.8/cli/common/enums/dns_registrars.py
+-rw-r--r--   0        0        0      263 2024-04-16 12:11:02.594653 cg_devx_core-0.2.8/cli/common/enums/git_plans.py
+-rw-r--r--   0        0        0      788 2024-04-16 12:11:02.594653 cg_devx_core-0.2.8/cli/common/enums/git_providers.py
+-rw-r--r--   0        0        0     1779 2024-04-16 12:11:02.594653 cg_devx_core-0.2.8/cli/common/logging_config.py
+-rw-r--r--   0        0        0      830 2024-04-16 12:11:02.594653 cg_devx_core-0.2.8/cli/common/retry_decorator.py
+-rw-r--r--   0        0        0      307 2024-04-16 12:11:02.594653 cg_devx_core-0.2.8/cli/common/singleton_metaclass.py
+-rw-r--r--   0        0        0     3574 2024-04-16 12:11:02.594653 cg_devx_core-0.2.8/cli/common/state_store.py
+-rw-r--r--   0        0        0     1258 2024-04-16 12:11:02.594653 cg_devx_core-0.2.8/cli/common/tracing_decorator.py
+-rw-r--r--   0        0        0        0 2024-04-16 12:11:02.594653 cg_devx_core-0.2.8/cli/common/utils/__init__.py
+-rw-r--r--   0        0        0    12697 2024-04-16 12:11:02.594653 cg_devx_core-0.2.8/cli/common/utils/command_utils.py
+-rw-r--r--   0        0        0      314 2024-04-16 12:11:02.594653 cg_devx_core-0.2.8/cli/common/utils/generators.py
+-rw-r--r--   0        0        0      187 2024-04-16 12:11:02.594653 cg_devx_core-0.2.8/cli/common/utils/os_utils.py
+-rw-r--r--   0        0        0      532 2024-04-16 12:11:02.594653 cg_devx_core-0.2.8/cli/services/README.md
+-rw-r--r--   0        0        0        0 2024-04-16 12:11:02.594653 cg_devx_core-0.2.8/cli/services/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-16 12:11:02.594653 cg_devx_core-0.2.8/cli/services/cloud/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-16 12:11:02.594653 cg_devx_core-0.2.8/cli/services/cloud/aws/__init__.py
+-rw-r--r--   0        0        0     6482 2024-04-16 12:11:02.594653 cg_devx_core-0.2.8/cli/services/cloud/aws/aws_manager.py
+-rw-r--r--   0        0        0    11353 2024-04-16 12:11:02.594653 cg_devx_core-0.2.8/cli/services/cloud/aws/aws_sdk.py
+-rw-r--r--   0        0        0      932 2024-04-16 12:11:02.594653 cg_devx_core-0.2.8/cli/services/cloud/aws/aws_session_manager.py
+-rw-r--r--   0        0        0     5126 2024-04-16 12:11:02.598653 cg_devx_core-0.2.8/cli/services/cloud/aws/iam_permissions.py
+-rw-r--r--   0        0        0        0 2024-04-16 12:11:02.598653 cg_devx_core-0.2.8/cli/services/cloud/azure/__init__.py
+-rw-r--r--   0        0        0    11546 2024-04-16 12:11:02.598653 cg_devx_core-0.2.8/cli/services/cloud/azure/azure_manager.py
+-rw-r--r--   0        0        0    25095 2024-04-16 12:11:02.598653 cg_devx_core-0.2.8/cli/services/cloud/azure/azure_sdk.py
+-rw-r--r--   0        0        0     5846 2024-04-16 12:11:02.598653 cg_devx_core-0.2.8/cli/services/cloud/azure/iam_permissions.py
+-rw-r--r--   0        0        0     4460 2024-04-16 12:11:02.598653 cg_devx_core-0.2.8/cli/services/cloud/cloud_provider_manager.py
+-rw-r--r--   0        0        0     6504 2024-04-16 12:11:02.598653 cg_devx_core-0.2.8/cli/services/dependency_manager.py
+-rw-r--r--   0        0        0        0 2024-04-16 12:11:02.598653 cg_devx_core-0.2.8/cli/services/dns/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-16 12:11:02.598653 cg_devx_core-0.2.8/cli/services/dns/azure_dns/__init__.py
+-rw-r--r--   0        0        0     1819 2024-04-16 12:11:02.598653 cg_devx_core-0.2.8/cli/services/dns/azure_dns/azure_dns.py
+-rw-r--r--   0        0        0     2049 2024-04-16 12:11:02.598653 cg_devx_core-0.2.8/cli/services/dns/dns_provider_manager.py
+-rw-r--r--   0        0        0        0 2024-04-16 12:11:02.598653 cg_devx_core-0.2.8/cli/services/dns/route53/__init__.py
+-rw-r--r--   0        0        0     1788 2024-04-16 12:11:02.598653 cg_devx_core-0.2.8/cli/services/dns/route53/route53.py
+-rw-r--r--   0        0        0        0 2024-04-16 12:11:02.598653 cg_devx_core-0.2.8/cli/services/k8s/__init__.py
+-rw-r--r--   0        0        0     1271 2024-04-16 12:11:02.598653 cg_devx_core-0.2.8/cli/services/k8s/config_builder.py
+-rw-r--r--   0        0        0     6622 2024-04-16 12:11:02.598653 cg_devx_core-0.2.8/cli/services/k8s/delivery_service_manager.py
+-rw-r--r--   0        0        0    21428 2024-04-16 12:11:02.598653 cg_devx_core-0.2.8/cli/services/k8s/k8s.py
+-rw-r--r--   0        0        0     2150 2024-04-16 12:11:02.598653 cg_devx_core-0.2.8/cli/services/k8s/kctl_wrapper.py
+-rw-r--r--   0        0        0      461 2024-04-16 12:11:02.598653 cg_devx_core-0.2.8/cli/services/k8s/kubeconfig.yaml
+-rw-r--r--   0        0        0        0 2024-04-16 12:11:02.598653 cg_devx_core-0.2.8/cli/services/keys/__init__.py
+-rw-r--r--   0        0        0     2156 2024-04-16 12:11:02.598653 cg_devx_core-0.2.8/cli/services/keys/key_manager.py
+-rw-r--r--   0        0        0     9269 2024-04-16 12:11:02.598653 cg_devx_core-0.2.8/cli/services/platform_gitops.py
+-rw-r--r--   0        0        0     6121 2024-04-16 12:11:02.598653 cg_devx_core-0.2.8/cli/services/platform_template_manager.py
+-rw-r--r--   0        0        0    15527 2024-04-16 12:11:02.598653 cg_devx_core-0.2.8/cli/services/tf_wrapper.py
+-rw-r--r--   0        0        0        0 2024-04-16 12:11:02.598653 cg_devx_core-0.2.8/cli/services/vcs/__init__.py
+-rw-r--r--   0        0        0     2025 2024-04-16 12:11:02.598653 cg_devx_core-0.2.8/cli/services/vcs/git_provider_manager.py
+-rw-r--r--   0        0        0        0 2024-04-16 12:11:02.598653 cg_devx_core-0.2.8/cli/services/vcs/github/__init__.py
+-rw-r--r--   0        0        0     5614 2024-04-16 12:11:02.598653 cg_devx_core-0.2.8/cli/services/vcs/github/github_manager.py
+-rw-r--r--   0        0        0        0 2024-04-16 12:11:02.598653 cg_devx_core-0.2.8/cli/services/vcs/gitlab/__init__.py
+-rw-r--r--   0        0        0     7767 2024-04-16 12:11:02.598653 cg_devx_core-0.2.8/cli/services/vcs/gitlab/gitlab_manager.py
+-rw-r--r--   0        0        0    12262 2024-04-16 12:11:02.598653 cg_devx_core-0.2.8/cli/services/wl_template_manager.py
+-rw-r--r--   0        0        0     1244 2024-04-16 12:11:20.406802 cg_devx_core-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0     4062 1970-01-01 00:00:00.000000 cg_devx_core-0.2.8/PKG-INFO
```

### Comparing `cg_devx_core-0.2.7/README.md` & `cg_devx_core-0.2.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -97,7 +97,9 @@
 
 Arguments:
 Are command specific and could be supplied via command lime, environment variables, or file
 
 For more details,
 please check CG DevX quickstart [commands](cli/commands/README.md)
 and [workload commands](cli/commands/workload/README.md)
+
+# generateReleaseNotes
```

### Comparing `cg_devx_core-0.2.7/cli/build.py` & `cg_devx_core-0.2.8/cli/build.py`

 * *Files identical despite different names*

### Comparing `cg_devx_core-0.2.7/cli/commands/README.md` & `cg_devx_core-0.2.8/cli/commands/README.md`

 * *Files identical despite different names*

### Comparing `cg_devx_core-0.2.7/cli/commands/destroy.py` & `cg_devx_core-0.2.8/cli/commands/destroy.py`

 * *Files identical despite different names*

### Comparing `cg_devx_core-0.2.7/cli/commands/setup.py` & `cg_devx_core-0.2.8/cli/commands/setup.py`

 * *Files identical despite different names*

### Comparing `cg_devx_core-0.2.7/cli/commands/workload/README.md` & `cg_devx_core-0.2.8/cli/commands/workload/README.md`

 * *Files identical despite different names*

### Comparing `cg_devx_core-0.2.7/cli/commands/workload/bootstrap.py` & `cg_devx_core-0.2.8/cli/commands/workload/bootstrap.py`

 * *Files identical despite different names*

### Comparing `cg_devx_core-0.2.7/cli/commands/workload/create.py` & `cg_devx_core-0.2.8/cli/commands/workload/create.py`

 * *Files identical despite different names*

### Comparing `cg_devx_core-0.2.7/cli/commands/workload/delete.py` & `cg_devx_core-0.2.8/cli/commands/workload/delete.py`

 * *Files identical despite different names*

### Comparing `cg_devx_core-0.2.7/cli/common/const/common_path.py` & `cg_devx_core-0.2.8/cli/common/const/common_path.py`

 * *Files identical despite different names*

### Comparing `cg_devx_core-0.2.7/cli/common/const/const.py` & `cg_devx_core-0.2.8/cli/common/const/const.py`

 * *Files identical despite different names*

### Comparing `cg_devx_core-0.2.7/cli/common/const/parameter_names.py` & `cg_devx_core-0.2.8/cli/common/const/parameter_names.py`

 * *Files identical despite different names*

### Comparing `cg_devx_core-0.2.7/cli/common/custom_excpetions.py` & `cg_devx_core-0.2.8/cli/common/custom_excpetions.py`

 * *Files identical despite different names*

### Comparing `cg_devx_core-0.2.7/cli/common/enums/cloud_providers.py` & `cg_devx_core-0.2.8/cli/common/enums/cloud_providers.py`

 * *Files identical despite different names*

### Comparing `cg_devx_core-0.2.7/cli/common/enums/dns_registrars.py` & `cg_devx_core-0.2.8/cli/common/enums/dns_registrars.py`

 * *Files identical despite different names*

### Comparing `cg_devx_core-0.2.7/cli/common/enums/git_providers.py` & `cg_devx_core-0.2.8/cli/common/enums/git_providers.py`

 * *Files identical despite different names*

### Comparing `cg_devx_core-0.2.7/cli/common/logging_config.py` & `cg_devx_core-0.2.8/cli/common/logging_config.py`

 * *Files identical despite different names*

### Comparing `cg_devx_core-0.2.7/cli/common/retry_decorator.py` & `cg_devx_core-0.2.8/cli/common/retry_decorator.py`

 * *Files identical despite different names*

### Comparing `cg_devx_core-0.2.7/cli/common/state_store.py` & `cg_devx_core-0.2.8/cli/common/state_store.py`

 * *Files identical despite different names*

### Comparing `cg_devx_core-0.2.7/cli/common/tracing_decorator.py` & `cg_devx_core-0.2.8/cli/common/tracing_decorator.py`

 * *Files identical despite different names*

### Comparing `cg_devx_core-0.2.7/cli/common/utils/command_utils.py` & `cg_devx_core-0.2.8/cli/common/utils/command_utils.py`

 * *Files identical despite different names*

### Comparing `cg_devx_core-0.2.7/cli/services/README.md` & `cg_devx_core-0.2.8/cli/services/README.md`

 * *Files identical despite different names*

### Comparing `cg_devx_core-0.2.7/cli/services/cloud/aws/aws_manager.py` & `cg_devx_core-0.2.8/cli/services/cloud/aws/aws_manager.py`

 * *Files identical despite different names*

### Comparing `cg_devx_core-0.2.7/cli/services/cloud/aws/aws_sdk.py` & `cg_devx_core-0.2.8/cli/services/cloud/aws/aws_sdk.py`

 * *Files identical despite different names*

### Comparing `cg_devx_core-0.2.7/cli/services/cloud/aws/aws_session_manager.py` & `cg_devx_core-0.2.8/cli/services/cloud/aws/aws_session_manager.py`

 * *Files identical despite different names*

### Comparing `cg_devx_core-0.2.7/cli/services/cloud/aws/iam_permissions.py` & `cg_devx_core-0.2.8/cli/services/cloud/aws/iam_permissions.py`

 * *Files identical despite different names*

### Comparing `cg_devx_core-0.2.7/cli/services/cloud/azure/azure_manager.py` & `cg_devx_core-0.2.8/cli/services/cloud/azure/azure_manager.py`

 * *Files identical despite different names*

### Comparing `cg_devx_core-0.2.7/cli/services/cloud/azure/azure_sdk.py` & `cg_devx_core-0.2.8/cli/services/cloud/azure/azure_sdk.py`

 * *Files identical despite different names*

### Comparing `cg_devx_core-0.2.7/cli/services/cloud/azure/iam_permissions.py` & `cg_devx_core-0.2.8/cli/services/cloud/azure/iam_permissions.py`

 * *Files identical despite different names*

### Comparing `cg_devx_core-0.2.7/cli/services/cloud/cloud_provider_manager.py` & `cg_devx_core-0.2.8/cli/services/cloud/cloud_provider_manager.py`

 * *Files identical despite different names*

### Comparing `cg_devx_core-0.2.7/cli/services/dependency_manager.py` & `cg_devx_core-0.2.8/cli/services/dependency_manager.py`

 * *Files identical despite different names*

### Comparing `cg_devx_core-0.2.7/cli/services/dns/azure_dns/azure_dns.py` & `cg_devx_core-0.2.8/cli/services/dns/azure_dns/azure_dns.py`

 * *Files identical despite different names*

### Comparing `cg_devx_core-0.2.7/cli/services/dns/dns_provider_manager.py` & `cg_devx_core-0.2.8/cli/services/dns/dns_provider_manager.py`

 * *Files identical despite different names*

### Comparing `cg_devx_core-0.2.7/cli/services/dns/route53/route53.py` & `cg_devx_core-0.2.8/cli/services/dns/route53/route53.py`

 * *Files identical despite different names*

### Comparing `cg_devx_core-0.2.7/cli/services/k8s/config_builder.py` & `cg_devx_core-0.2.8/cli/services/k8s/config_builder.py`

 * *Files identical despite different names*

### Comparing `cg_devx_core-0.2.7/cli/services/k8s/delivery_service_manager.py` & `cg_devx_core-0.2.8/cli/services/k8s/delivery_service_manager.py`

 * *Files identical despite different names*

### Comparing `cg_devx_core-0.2.7/cli/services/k8s/k8s.py` & `cg_devx_core-0.2.8/cli/services/k8s/k8s.py`

 * *Files identical despite different names*

### Comparing `cg_devx_core-0.2.7/cli/services/k8s/kctl_wrapper.py` & `cg_devx_core-0.2.8/cli/services/k8s/kctl_wrapper.py`

 * *Files identical despite different names*

### Comparing `cg_devx_core-0.2.7/cli/services/keys/key_manager.py` & `cg_devx_core-0.2.8/cli/services/keys/key_manager.py`

 * *Files identical despite different names*

### Comparing `cg_devx_core-0.2.7/cli/services/platform_gitops.py` & `cg_devx_core-0.2.8/cli/services/platform_gitops.py`

 * *Files identical despite different names*

### Comparing `cg_devx_core-0.2.7/cli/services/platform_template_manager.py` & `cg_devx_core-0.2.8/cli/services/platform_template_manager.py`

 * *Files identical despite different names*

### Comparing `cg_devx_core-0.2.7/cli/services/tf_wrapper.py` & `cg_devx_core-0.2.8/cli/services/tf_wrapper.py`

 * *Files identical despite different names*

### Comparing `cg_devx_core-0.2.7/cli/services/vcs/git_provider_manager.py` & `cg_devx_core-0.2.8/cli/services/vcs/git_provider_manager.py`

 * *Files identical despite different names*

### Comparing `cg_devx_core-0.2.7/cli/services/vcs/github/github_manager.py` & `cg_devx_core-0.2.8/cli/services/vcs/github/github_manager.py`

 * *Files identical despite different names*

### Comparing `cg_devx_core-0.2.7/cli/services/vcs/gitlab/gitlab_manager.py` & `cg_devx_core-0.2.8/cli/services/vcs/gitlab/gitlab_manager.py`

 * *Files identical despite different names*

### Comparing `cg_devx_core-0.2.7/cli/services/wl_template_manager.py` & `cg_devx_core-0.2.8/cli/services/wl_template_manager.py`

 * *Files identical despite different names*

### Comparing `cg_devx_core-0.2.7/pyproject.toml` & `cg_devx_core-0.2.8/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "cg-devx-core"
-version = "0.2.7"
-description = ""
+version = "0.2.8"
+description = "cgdevx platform"
 authors = ["Alexander Ulyanov <alexu@cloudgeometry.io>", "Mikhail Turetskii <mturetsky@cloudgeometry.io>"]
 readme = "README.md"
 packages = [{ include = "cli" }]
 
 [tool.poetry.scripts]
 cgdevxcli = "cli.__main__:entry_point"
 build = "cli.build:install"
```

### Comparing `cg_devx_core-0.2.7/PKG-INFO` & `cg_devx_core-0.2.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: cg-devx-core
-Version: 0.2.7
-Summary: 
+Version: 0.2.8
+Summary: cgdevx platform
 Author: Alexander Ulyanov
 Author-email: alexu@cloudgeometry.io
 Requires-Python: >=3.10,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: PyInstaller (==5.13.2)
 Requires-Dist: alive-progress (>=3.1.5,<4.0.0)
@@ -135,7 +135,9 @@
 Arguments:
 Are command specific and could be supplied via command lime, environment variables, or file
 
 For more details,
 please check CG DevX quickstart [commands](cli/commands/README.md)
 and [workload commands](cli/commands/workload/README.md)
 
+# generateReleaseNotes
+
```

