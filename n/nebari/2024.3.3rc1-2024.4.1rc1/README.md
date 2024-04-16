# Comparing `tmp/nebari-2024.3.3rc1.tar.gz` & `tmp/nebari-2024.4.1rc1.tar.gz`

## Comparing `nebari-2024.3.3rc1.tar` & `nebari-2024.4.1rc1.tar`

### file list

```diff
@@ -1,428 +1,429 @@
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/.cirun.yml
--rw-r--r--   0        0        0     2286 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1993 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/CONTRIBUTING.md
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/MANIFEST.in
--rw-r--r--   0        0        0    85349 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/RELEASE.md
--rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/SECURITY.md
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/flake.lock
--rw-r--r--   0        0        0     2041 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/flake.nix
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/pytest.ini
--rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/.github/release-notes-sync-config.yaml
--rw-r--r--   0        0        0     3992 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/.github/ISSUE_TEMPLATE/bug-report.yml
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/.github/ISSUE_TEMPLATE/feature-request.yml
--rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/.github/ISSUE_TEMPLATE/general-issue.yml
--rw-r--r--   0        0        0     3950 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/.github/ISSUE_TEMPLATE/release-checklist.md
--rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/.github/ISSUE_TEMPLATE/testing-checklist.md
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/.github/actions/publish-from-template/action.yml
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/.github/actions/publish-from-template/render_template.py
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/.github/failed-workflow-issue-templates/test-provider.md
--rw-r--r--   0        0        0     2081 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/.github/workflows/generate_cli_doc.yml
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/.github/workflows/release-notes-sync.yaml
--rw-r--r--   0        0        0     1927 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/.github/workflows/release.yaml
--rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/.github/workflows/run-precommit.yaml
--rw-r--r--   0        0        0     5806 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/.github/workflows/test-provider.yaml
--rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/.github/workflows/test.yaml
--rw-r--r--   0        0        0     2682 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/.github/workflows/test_aws_integration.yaml
--rw-r--r--   0        0        0     1397 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/.github/workflows/test_conda_build.yaml
--rw-r--r--   0        0        0     2729 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/.github/workflows/test_do_integration.yaml
--rw-r--r--   0        0        0     3197 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/.github/workflows/test_gcp_integration.yaml
--rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/.github/workflows/test_helm_charts.yaml
--rw-r--r--   0        0        0     5673 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/.github/workflows/test_local_integration.yaml
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/.github/workflows/typing.yaml
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/docs-sphinx/Makefile
--rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/docs-sphinx/README.md
--rw-r--r--   0        0        0    46502 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/docs-sphinx/cli.html
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/docs-sphinx/cli.rst
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/docs-sphinx/conf.py
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/docs-sphinx/index.rst
--rw-r--r--   0        0        0    14306 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/scripts/aws-force-destroy.py
--rwxr-xr-x   0        0        0     8475 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/scripts/aws-force-destroy.sh
--rw-r--r--   0        0        0     8439 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/scripts/helm-validate.py
--rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/scripts/keycloak-export.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/__init__.py
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/_version.py
--rw-r--r--   0        0        0     2277 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/cli.py
--rw-r--r--   0        0        0     3541 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/config.py
--rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/constants.py
--rw-r--r--   0        0        0     2998 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/deploy.py
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/deprecate.py
--rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/destroy.py
--rw-r--r--   0        0        0    10678 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/initialize.py
--rw-r--r--   0        0        0     5781 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/keycloak.py
--rw-r--r--   0        0        0     6123 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/render.py
--rw-r--r--   0        0        0    31183 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/upgrade.py
--rw-r--r--   0        0        0     9621 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/utils.py
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/provider/__init__.py
--rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/provider/git.py
--rw-r--r--   0        0        0     8126 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/provider/terraform.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/provider/cicd/__init__.py
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/provider/cicd/common.py
--rw-r--r--   0        0        0    10150 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/provider/cicd/github.py
--rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/provider/cicd/gitlab.py
--rw-r--r--   0        0        0     2986 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/provider/cicd/linter.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/provider/cloud/__init__.py
--rw-r--r--   0        0        0    38296 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/provider/cloud/amazon_web_services.py
--rw-r--r--   0        0        0     5415 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/provider/cloud/azure_cloud.py
--rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/provider/cloud/commons.py
--rw-r--r--   0        0        0     4018 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/provider/cloud/digital_ocean.py
--rw-r--r--   0        0        0     8976 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/provider/cloud/google_cloud.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/provider/dns/__init__.py
--rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/provider/dns/cloudflare.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/provider/oauth/__init__.py
--rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/provider/oauth/auth0.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/__init__.py
--rw-r--r--   0        0        0     3917 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/base.py
--rw-r--r--   0        0        0     5543 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/tf_objects.py
--rw-r--r--   0        0        0     2991 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/bootstrap/__init__.py
--rw-r--r--   0        0        0    32021 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/infrastructure/__init__.py
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/infrastructure/template/aws/locals.tf
--rw-r--r--   0        0        0     2708 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/infrastructure/template/aws/main.tf
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/infrastructure/template/aws/outputs.tf
--rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/infrastructure/template/aws/variables.tf
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/infrastructure/template/aws/versions.tf
--rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/infrastructure/template/aws/modules/accounting/main.tf
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/infrastructure/template/aws/modules/accounting/variables.tf
--rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/infrastructure/template/aws/modules/efs/main.tf
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/infrastructure/template/aws/modules/efs/outputs.tf
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/infrastructure/template/aws/modules/efs/variables.tf
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/infrastructure/template/aws/modules/kafka/main.tf
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/infrastructure/template/aws/modules/kafka/outputs.tf
--rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/infrastructure/template/aws/modules/kafka/variables.tf
--rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/infrastructure/template/aws/modules/kubernetes/autoscaling.tf
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/infrastructure/template/aws/modules/kubernetes/locals.tf
--rw-r--r--   0        0        0     3322 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/infrastructure/template/aws/modules/kubernetes/main.tf
--rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/infrastructure/template/aws/modules/kubernetes/outputs.tf
--rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/infrastructure/template/aws/modules/kubernetes/policy.tf
--rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/infrastructure/template/aws/modules/kubernetes/variables.tf
--rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/infrastructure/template/aws/modules/network/main.tf
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/infrastructure/template/aws/modules/network/outputs.tf
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/infrastructure/template/aws/modules/network/variables.tf
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/infrastructure/template/aws/modules/permissions/main.tf
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/infrastructure/template/aws/modules/permissions/outputs.tf
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/infrastructure/template/aws/modules/permissions/variables.tf
--rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/infrastructure/template/aws/modules/rds/main.tf
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/infrastructure/template/aws/modules/rds/outputs.tf
--rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/infrastructure/template/aws/modules/rds/users.tf
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/infrastructure/template/aws/modules/rds/variables.tf
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/infrastructure/template/aws/modules/registry/main.tf
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/infrastructure/template/aws/modules/registry/outputs.tf
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/infrastructure/template/aws/modules/registry/variables.tf
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/infrastructure/template/aws/modules/s3/main.tf
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/infrastructure/template/aws/modules/s3/outputs.tf
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/infrastructure/template/aws/modules/s3/variables.tf
--rw-r--r--   0        0        0     1362 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/infrastructure/template/azure/main.tf
--rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/infrastructure/template/azure/outputs.tf
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/infrastructure/template/azure/providers.tf
--rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/infrastructure/template/azure/variables.tf
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/infrastructure/template/azure/versions.tf
--rw-r--r--   0        0        0     3781 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/infrastructure/template/azure/modules/kubernetes/main.tf
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/infrastructure/template/azure/modules/kubernetes/outputs.tf
--rw-r--r--   0        0        0     1905 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/infrastructure/template/azure/modules/kubernetes/variables.tf
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/infrastructure/template/azure/modules/registry/main.tf
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/infrastructure/template/azure/modules/registry/variables.tf
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/infrastructure/template/do/main.tf
--rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/infrastructure/template/do/outputs.tf
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/infrastructure/template/do/providers.tf
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/infrastructure/template/do/variables.tf
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/infrastructure/template/do/versions.tf
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/infrastructure/template/do/modules/kubernetes/locals.tf
--rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/infrastructure/template/do/modules/kubernetes/main.tf
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/infrastructure/template/do/modules/kubernetes/outputs.tf
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/infrastructure/template/do/modules/kubernetes/variables.tf
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/infrastructure/template/do/modules/kubernetes/versions.tf
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/infrastructure/template/do/modules/registry/main.tf
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/infrastructure/template/do/modules/registry/variable.tf
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/infrastructure/template/do/modules/registry/versions.tf
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/infrastructure/template/existing/main.tf
--rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/infrastructure/template/gcp/main.tf
--rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/infrastructure/template/gcp/outputs.tf
--rw-r--r--   0        0        0     2485 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/infrastructure/template/gcp/variables.tf
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/infrastructure/template/gcp/versions.tf
--rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/infrastructure/template/gcp/modules/kubernetes/locals.tf
--rw-r--r--   0        0        0     3324 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/infrastructure/template/gcp/modules/kubernetes/main.tf
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/infrastructure/template/gcp/modules/kubernetes/outputs.tf
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/infrastructure/template/gcp/modules/kubernetes/service_account.tf
--rw-r--r--   0        0        0     3896 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/infrastructure/template/gcp/modules/kubernetes/variables.tf
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/infrastructure/template/gcp/modules/kubernetes/templates/kubeconfig.yaml
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/infrastructure/template/gcp/modules/network/main.tf
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/infrastructure/template/gcp/modules/network/variables.tf
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/infrastructure/template/gcp/modules/registry/main.tf
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/infrastructure/template/gcp/modules/registry/variables.tf
--rw-r--r--   0        0        0     2497 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/infrastructure/template/local/main.tf
--rw-r--r--   0        0        0     7993 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/infrastructure/template/local/metallb.yaml
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/infrastructure/template/local/outputs.tf
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/infrastructure/template/local/variables.tf
--rw-r--r--   0        0        0     9630 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_ingress/__init__.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_ingress/template/locals.tf
--rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_ingress/template/main.tf
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_ingress/template/outputs.tf
--rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_ingress/template/variables.tf
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_ingress/template/versions.tf
--rw-r--r--   0        0        0     9777 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_ingress/template/modules/kubernetes/ingress/main.tf
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_ingress/template/modules/kubernetes/ingress/outputs.tf
--rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_ingress/template/modules/kubernetes/ingress/variables.tf
--rw-r--r--   0        0        0     4257 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_initialize/__init__.py
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_initialize/template/external-container-registry.tf
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_initialize/template/locals.tf
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_initialize/template/main.tf
--rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_initialize/template/variables.tf
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_initialize/template/versions.tf
--rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_initialize/template/modules/cluster-autoscaler/main.tf
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_initialize/template/modules/cluster-autoscaler/variables.tf
--rw-r--r--   0        0        0     7691 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_initialize/template/modules/extcr/main.tf
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_initialize/template/modules/extcr/variables.tf
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_initialize/template/modules/initialization/main.tf
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_initialize/template/modules/initialization/variables.tf
--rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_initialize/template/modules/nvidia-installer/aws-nvidia-installer.tf
--rw-r--r--   0        0        0     3739 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_initialize/template/modules/nvidia-installer/gcp-nvidia-installer.tf
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_initialize/template/modules/nvidia-installer/variables.tf
--rw-r--r--   0        0        0    57723 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_initialize/template/modules/traefik_crds/main.tf
--rw-r--r--   0        0        0     9398 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_keycloak/__init__.py
--rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_keycloak/template/main.tf
--rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_keycloak/template/outputs.tf
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_keycloak/template/variables.tf
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_keycloak/template/versions.tf
--rw-r--r--   0        0        0     1489 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_keycloak/template/modules/kubernetes/keycloak-helm/main.tf
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_keycloak/template/modules/kubernetes/keycloak-helm/outputs.tf
--rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_keycloak/template/modules/kubernetes/keycloak-helm/values.yaml
--rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_keycloak/template/modules/kubernetes/keycloak-helm/variables.tf
--rw-r--r--   0        0        0     3977 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_keycloak_configuration/__init__.py
--rw-r--r--   0        0        0     3365 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_keycloak_configuration/template/main.tf
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_keycloak_configuration/template/outputs.tf
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_keycloak_configuration/template/permissions.tf
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_keycloak_configuration/template/providers.tf
--rw-r--r--   0        0        0     2637 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_keycloak_configuration/template/social_auth.tf
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_keycloak_configuration/template/variables.tf
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_keycloak_configuration/template/versions.tf
--rw-r--r--   0        0        0    22258 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/__init__.py
--rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/argo-workflows.tf
--rw-r--r--   0        0        0     2460 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/conda-store.tf
--rw-r--r--   0        0        0     1378 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/dask_gateway.tf
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/forward-auth.tf
--rw-r--r--   0        0        0     4481 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/jupyterhub.tf
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/jupyterhub_ssh.tf
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/locals.tf
--rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/monitoring.tf
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/outputs.tf
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/providers.tf
--rw-r--r--   0        0        0     2018 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/variables.tf
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/versions.tf
--rw-r--r--   0        0        0     4548 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/forwardauth/main.tf
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/forwardauth/variables.tf
--rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/nfs-mount/main.tf
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/nfs-mount/outputs.tf
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/nfs-mount/variables.tf
--rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/nfs-server/main.tf
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/nfs-server/output.tf
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/nfs-server/variables.tf
--rw-r--r--   0        0        0    16354 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/argo-workflows/main.tf
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/argo-workflows/values.yaml
--rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/argo-workflows/variables.tf
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/argo-workflows/versions.tf
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/conda-store/output.tf
--rw-r--r--   0        0        0     5210 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/conda-store/server.tf
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/conda-store/storage.tf
--rw-r--r--   0        0        0     1813 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/conda-store/variables.tf
--rw-r--r--   0        0        0     4560 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/conda-store/worker.tf
--rw-r--r--   0        0        0     6543 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/conda-store/config/conda_store_config.py
--rw-r--r--   0        0        0     3917 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/controler.tf
--rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/crds.tf
--rw-r--r--   0        0        0     6381 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/gateway.tf
--rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/main.tf
--rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/middleware.tf
--rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/outputs.tf
--rw-r--r--   0        0        0     5507 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/variables.tf
--rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/files/controller_config.py
--rw-r--r--   0        0        0    10699 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/files/gateway_config.py
--rw-r--r--   0        0        0     4140 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/configmaps.tf
--rw-r--r--   0        0        0     8414 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/main.tf
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/outputs.tf
--rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/values.yaml
--rw-r--r--   0        0        0     4723 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/variables.tf
--rw-r--r--   0        0        0     3947 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/extras/git_clone_update.sh
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/ipython/ipython_config.py
--rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/jupyter/jupyter_jupyterlab_pioneer_config.py.tpl
--rw-r--r--   0        0        0     2323 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/jupyter/jupyter_server_config.py.tpl
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/jupyterhub/01-theme.py
--rw-r--r--   0        0        0     2728 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/jupyterhub/02-spawner.py
--rw-r--r--   0        0        0    19781 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/jupyterhub/03-profiles.py
--rw-r--r--   0        0        0     4347 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/jupyterlab/overrides.json
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/skel/.bash_logout
--rw-r--r--   0        0        0     4768 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/skel/.bashrc
--rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/skel/.profile
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub-ssh/main.tf
--rw-r--r--   0        0        0     2909 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub-ssh/sftp.tf
--rw-r--r--   0        0        0     3127 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub-ssh/ssh.tf
--rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub-ssh/variables.tf
--rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/keycloak-client/main.tf
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/keycloak-client/outputs.tf
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/keycloak-client/variables.tf
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/keycloak-client/versions.tf
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/minio/ingress.tf
--rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/minio/main.tf
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/minio/outputs.tf
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/minio/values.yaml
--rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/minio/variables.tf
--rw-r--r--   0        0        0     9352 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/main.tf
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/values.yaml
--rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/variables.tf
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/versions.tf
--rw-r--r--   0        0        0    26841 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/dashboards/Main/cluster_information.json
--rw-r--r--   0        0        0    15913 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/dashboards/Main/conda_store.json
--rw-r--r--   0        0        0    34598 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/dashboards/Main/jupyterhub_dashboard.json
--rw-r--r--   0        0        0    52146 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/dashboards/Main/keycloak.json
--rw-r--r--   0        0        0    28438 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/dashboards/Main/traefik.json
--rw-r--r--   0        0        0     7418 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/dashboards/Main/usage_report.json
--rw-r--r--   0        0        0     2651 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/loki/main.tf
--rw-r--r--   0        0        0     2625 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/loki/values_loki.yaml
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/loki/values_minio.yaml
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/loki/values_promtail.yaml
--rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/loki/variables.tf
--rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/postgresql/main.tf
--rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/postgresql/outputs.tf
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/postgresql/values.yaml
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/postgresql/variables.tf
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/redis/main.tf
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/redis/outputs.tf
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/redis/values.yaml
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/redis/variables.tf
--rw-r--r--   0        0        0     2211 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/nebari_tf_extensions/__init__.py
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/nebari_tf_extensions/template/helm-extension.tf
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/nebari_tf_extensions/template/nebari-config.tf
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/nebari_tf_extensions/template/providers.tf
--rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/nebari_tf_extensions/template/tf-extensions.tf
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/nebari_tf_extensions/template/variables.tf
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/nebari_tf_extensions/template/versions.tf
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/nebari_tf_extensions/template/modules/helm-extensions/main.tf
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/nebari_tf_extensions/template/modules/helm-extensions/variables.tf
--rw-r--r--   0        0        0     1380 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/nebari_tf_extensions/template/modules/nebariextension/ingress.tf
--rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/nebari_tf_extensions/template/modules/nebariextension/keycloak-config.tf
--rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/nebari_tf_extensions/template/modules/nebariextension/locals.tf
--rw-r--r--   0        0        0     2044 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/nebari_tf_extensions/template/modules/nebariextension/main.tf
--rw-r--r--   0        0        0     1470 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/nebari_tf_extensions/template/modules/nebariextension/variables.tf
--rw-r--r--   0        0        0     9878 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/terraform_state/__init__.py
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/terraform_state/template/aws/main.tf
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/terraform_state/template/aws/modules/terraform-state/main.tf
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/terraform_state/template/aws/modules/terraform-state/output.tf
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/terraform_state/template/aws/modules/terraform-state/variables.tf
--rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/terraform_state/template/azure/main.tf
--rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/terraform_state/template/azure/modules/terraform-state/main.tf
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/terraform_state/template/azure/modules/terraform-state/variables.tf
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/terraform_state/template/do/main.tf
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/terraform_state/template/do/modules/spaces/main.tf
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/terraform_state/template/do/modules/spaces/variables.tf
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/terraform_state/template/do/modules/spaces/versions.tf
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/terraform_state/template/do/modules/terraform-state/main.tf
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/terraform_state/template/do/modules/terraform-state/variables.tf
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/terraform_state/template/do/modules/terraform-state/versions.tf
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/terraform_state/template/existing/main.tf
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/terraform_state/template/gcp/main.tf
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/terraform_state/template/gcp/modules/gcs/main.tf
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/terraform_state/template/gcp/modules/gcs/variables.tf
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/terraform_state/template/gcp/modules/terraform-state/main.tf
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/terraform_state/template/gcp/modules/terraform-state/variables.tf
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/stages/terraform_state/template/local/main.tf
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/subcommands/__init__.py
--rw-r--r--   0        0        0     3191 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/subcommands/deploy.py
--rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/subcommands/destroy.py
--rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/subcommands/dev.py
--rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/subcommands/info.py
--rw-r--r--   0        0        0    36591 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/subcommands/init.py
--rw-r--r--   0        0        0     2714 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/subcommands/keycloak.py
--rw-r--r--   0        0        0     1316 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/subcommands/render.py
--rw-r--r--   0        0        0     3032 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/subcommands/support.py
--rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/subcommands/upgrade.py
--rw-r--r--   0        0        0     1380 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/_nebari/subcommands/validate.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/nebari/__init__.py
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/nebari/__main__.py
--rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/nebari/hookspecs.py
--rw-r--r--   0        0        0     4350 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/nebari/plugins.py
--rw-r--r--   0        0        0     3226 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/src/nebari/schema.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/tests/__init__.py
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/tests/conftest.py
--rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/tests/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/tests/common/__init__.py
--rw-r--r--   0        0        0     4206 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/tests/common/config_mod_utils.py
--rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/tests/common/kube_api.py
--rw-r--r--   0        0        0    16519 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/tests/common/navigator.py
--rw-r--r--   0        0        0     2410 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/tests/common/playwright_fixtures.py
--rw-r--r--   0        0        0    10512 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/tests/common/run_notebook.py
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/tests/common/notebooks/test_notebook_output.ipynb
--rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/tests/common/tests/test_notebook.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/tests/tests_deployment/__init__.py
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/tests/tests_deployment/constants.py
--rw-r--r--   0        0        0     1497 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/tests/tests_deployment/test_dask_gateway.py
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/tests/tests_deployment/test_grafana_api.py
--rw-r--r--   0        0        0     4101 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/tests/tests_deployment/test_jupyterhub_ssh.py
--rw-r--r--   0        0        0     4329 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/tests/tests_deployment/test_loki_deployment.py
--rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/tests/tests_deployment/utils.py
--rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/tests/tests_deployment/assets/notebook/simple.ipynb
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/tests/tests_e2e/.gitignore
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/tests/tests_e2e/cypress.json
--rw-r--r--   0        0        0   147508 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/tests/tests_e2e/package-lock.json
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/tests/tests_e2e/package.json
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/tests/tests_e2e/cypress/.gitignore
--rw-r--r--   0        0        0     2946 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/tests/tests_e2e/cypress/integration/main.js
--rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/tests/tests_e2e/cypress/notebooks/BasicTest.ipynb
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/tests/tests_e2e/cypress/plugins/index.js
--rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/tests/tests_e2e/cypress/support/index.js
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/tests/tests_e2e/playwright/.env.tpl
--rw-r--r--   0        0        0     7127 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/tests/tests_e2e/playwright/README.md
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/tests/tests_e2e/playwright/test_playwright.py
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/tests/tests_integration/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/tests/tests_integration/__init__.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/tests/tests_integration/conftest.py
--rw-r--r--   0        0        0     7102 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/tests/tests_integration/deployment_fixtures.py
--rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/tests/tests_integration/test_all_clouds.py
--rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/tests/tests_integration/test_gpu.py
--rw-r--r--   0        0        0     1240 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/tests/tests_integration/test_preemptible.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/tests/tests_unit/__init__.py
--rw-r--r--   0        0        0     5968 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/tests/tests_unit/conftest.py
--rw-r--r--   0        0        0     1877 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/tests/tests_unit/test_cli.py
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/tests/tests_unit/test_cli_deploy.py
--rw-r--r--   0        0        0     7261 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/tests/tests_unit/test_cli_dev.py
--rw-r--r--   0        0        0     9330 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/tests/tests_unit/test_cli_init.py
--rw-r--r--   0        0        0     6479 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/tests/tests_unit/test_cli_init_repository.py
--rw-r--r--   0        0        0    14131 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/tests/tests_unit/test_cli_keycloak.py
--rw-r--r--   0        0        0     6529 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/tests/tests_unit/test_cli_support.py
--rw-r--r--   0        0        0    18509 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/tests/tests_unit/test_cli_upgrade.py
--rw-r--r--   0        0        0    10415 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/tests/tests_unit/test_cli_validate.py
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/tests/tests_unit/test_commons.py
--rw-r--r--   0        0        0     5037 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/tests/tests_unit/test_config.py
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/tests/tests_unit/test_dependencies.py
--rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/tests/tests_unit/test_init.py
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/tests/tests_unit/test_links.py
--rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/tests/tests_unit/test_provider.py
--rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/tests/tests_unit/test_render.py
--rw-r--r--   0        0        0     5172 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/tests/tests_unit/test_schema.py
--rw-r--r--   0        0        0     4441 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/tests/tests_unit/test_upgrade.py
--rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/tests/tests_unit/utils.py
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/tests/tests_unit/cli_validate/aws.error.kubernetes-version.yaml
--rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/tests/tests_unit/cli_validate/aws.happy.yaml
--rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/tests/tests_unit/cli_validate/azure.happy.yaml
--rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/tests/tests_unit/cli_validate/do.happy.yaml
--rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/tests/tests_unit/cli_validate/gcp.happy.yaml
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/tests/tests_unit/cli_validate/local.error.authentication-type-called-custom.yaml
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/tests/tests_unit/cli_validate/local.error.extra-fields.yaml
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/tests/tests_unit/cli_validate/local.error.project_name.ends_with_special.yaml
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/tests/tests_unit/cli_validate/local.error.project_name.starts_with_number.yaml
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/tests/tests_unit/cli_validate/local.error.project_name.too_long.yaml
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/tests/tests_unit/cli_validate/local.happy.auth0.yaml
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/tests/tests_unit/cli_validate/local.happy.github.yaml
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/tests/tests_unit/cli_validate/local.happy.project_name.with_numbers.yaml
--rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/tests/tests_unit/cli_validate/local.happy.yaml
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/tests/tests_unit/cli_validate/min.happy.jupyterlab.default_settings.yaml
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/tests/tests_unit/cli_validate/min.happy.monitoring.overrides.yaml
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/tests/tests_unit/cli_validate/min.happy.yaml
--rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/tests/tests_unit/qhub-config-yaml-files-for-upgrade/qhub-config-do-310-customauth.yaml
--rw-r--r--   0        0        0     3496 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/tests/tests_unit/qhub-config-yaml-files-for-upgrade/qhub-config-do-310.yaml
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/tests/tests_unit/qhub-config-yaml-files-for-upgrade/qhub-users-import.json
--rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/.gitignore
--rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/LICENSE
--rw-r--r--   0        0        0     9814 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/README.md
--rw-r--r--   0        0        0     3831 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/pyproject.toml
--rw-r--r--   0        0        0    12409 2020-02-02 00:00:00.000000 nebari-2024.3.3rc1/PKG-INFO
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/.cirun.yml
+-rw-r--r--   0        0        0     2286 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1993 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/CONTRIBUTING.md
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/MANIFEST.in
+-rw-r--r--   0        0        0    87041 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/RELEASE.md
+-rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/SECURITY.md
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/flake.lock
+-rw-r--r--   0        0        0     2041 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/flake.nix
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/pytest.ini
+-rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/.github/release-notes-sync-config.yaml
+-rw-r--r--   0        0        0     3992 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/.github/ISSUE_TEMPLATE/bug-report.yml
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/.github/ISSUE_TEMPLATE/feature-request.yml
+-rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/.github/ISSUE_TEMPLATE/general-issue.yml
+-rw-r--r--   0        0        0     3950 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/.github/ISSUE_TEMPLATE/release-checklist.md
+-rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/.github/ISSUE_TEMPLATE/testing-checklist.md
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/.github/actions/publish-from-template/action.yml
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/.github/actions/publish-from-template/render_template.py
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/.github/failed-workflow-issue-templates/test-provider.md
+-rw-r--r--   0        0        0     2081 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/.github/workflows/generate_cli_doc.yml
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/.github/workflows/release-notes-sync.yaml
+-rw-r--r--   0        0        0     1927 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/.github/workflows/release.yaml
+-rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/.github/workflows/run-precommit.yaml
+-rw-r--r--   0        0        0     5806 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/.github/workflows/test-provider.yaml
+-rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/.github/workflows/test.yaml
+-rw-r--r--   0        0        0     2682 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/.github/workflows/test_aws_integration.yaml
+-rw-r--r--   0        0        0     1397 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/.github/workflows/test_conda_build.yaml
+-rw-r--r--   0        0        0     2729 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/.github/workflows/test_do_integration.yaml
+-rw-r--r--   0        0        0     3197 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/.github/workflows/test_gcp_integration.yaml
+-rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/.github/workflows/test_helm_charts.yaml
+-rw-r--r--   0        0        0     5673 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/.github/workflows/test_local_integration.yaml
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/.github/workflows/typing.yaml
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/docs-sphinx/Makefile
+-rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/docs-sphinx/README.md
+-rw-r--r--   0        0        0    46502 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/docs-sphinx/cli.html
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/docs-sphinx/cli.rst
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/docs-sphinx/conf.py
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/docs-sphinx/index.rst
+-rw-r--r--   0        0        0    14306 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/scripts/aws-force-destroy.py
+-rwxr-xr-x   0        0        0     8475 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/scripts/aws-force-destroy.sh
+-rw-r--r--   0        0        0     8439 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/scripts/helm-validate.py
+-rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/scripts/keycloak-export.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/__init__.py
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/_version.py
+-rw-r--r--   0        0        0     2277 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/cli.py
+-rw-r--r--   0        0        0     3541 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/config.py
+-rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/constants.py
+-rw-r--r--   0        0        0     2998 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/deploy.py
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/deprecate.py
+-rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/destroy.py
+-rw-r--r--   0        0        0    11250 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/initialize.py
+-rw-r--r--   0        0        0     5781 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/keycloak.py
+-rw-r--r--   0        0        0     6123 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/render.py
+-rw-r--r--   0        0        0    31183 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/upgrade.py
+-rw-r--r--   0        0        0     9621 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/utils.py
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/provider/__init__.py
+-rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/provider/git.py
+-rw-r--r--   0        0        0     8126 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/provider/terraform.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/provider/cicd/__init__.py
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/provider/cicd/common.py
+-rw-r--r--   0        0        0    10150 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/provider/cicd/github.py
+-rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/provider/cicd/gitlab.py
+-rw-r--r--   0        0        0     2986 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/provider/cicd/linter.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/provider/cloud/__init__.py
+-rw-r--r--   0        0        0    38296 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/provider/cloud/amazon_web_services.py
+-rw-r--r--   0        0        0     5415 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/provider/cloud/azure_cloud.py
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/provider/cloud/commons.py
+-rw-r--r--   0        0        0     4018 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/provider/cloud/digital_ocean.py
+-rw-r--r--   0        0        0     8976 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/provider/cloud/google_cloud.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/provider/dns/__init__.py
+-rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/provider/dns/cloudflare.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/provider/oauth/__init__.py
+-rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/provider/oauth/auth0.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/__init__.py
+-rw-r--r--   0        0        0     3917 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/base.py
+-rw-r--r--   0        0        0     5543 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/tf_objects.py
+-rw-r--r--   0        0        0     2991 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/bootstrap/__init__.py
+-rw-r--r--   0        0        0    32085 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/__init__.py
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/locals.tf
+-rw-r--r--   0        0        0     2708 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/main.tf
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/outputs.tf
+-rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/variables.tf
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/versions.tf
+-rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/accounting/main.tf
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/accounting/variables.tf
+-rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/efs/main.tf
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/efs/outputs.tf
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/efs/variables.tf
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/kafka/main.tf
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/kafka/outputs.tf
+-rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/kafka/variables.tf
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/kubernetes/autoscaling.tf
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/kubernetes/locals.tf
+-rw-r--r--   0        0        0     3322 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/kubernetes/main.tf
+-rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/kubernetes/outputs.tf
+-rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/kubernetes/policy.tf
+-rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/kubernetes/variables.tf
+-rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/network/main.tf
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/network/outputs.tf
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/network/variables.tf
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/permissions/main.tf
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/permissions/outputs.tf
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/permissions/variables.tf
+-rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/rds/main.tf
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/rds/outputs.tf
+-rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/rds/users.tf
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/rds/variables.tf
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/registry/main.tf
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/registry/outputs.tf
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/registry/variables.tf
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/s3/main.tf
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/s3/outputs.tf
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/s3/variables.tf
+-rw-r--r--   0        0        0     1362 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/azure/main.tf
+-rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/azure/outputs.tf
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/azure/providers.tf
+-rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/azure/variables.tf
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/azure/versions.tf
+-rw-r--r--   0        0        0     3781 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/azure/modules/kubernetes/main.tf
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/azure/modules/kubernetes/outputs.tf
+-rw-r--r--   0        0        0     1905 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/azure/modules/kubernetes/variables.tf
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/azure/modules/registry/main.tf
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/azure/modules/registry/variables.tf
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/do/main.tf
+-rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/do/outputs.tf
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/do/providers.tf
+-rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/do/variables.tf
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/do/versions.tf
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/do/modules/kubernetes/locals.tf
+-rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/do/modules/kubernetes/main.tf
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/do/modules/kubernetes/outputs.tf
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/do/modules/kubernetes/variables.tf
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/do/modules/kubernetes/versions.tf
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/do/modules/registry/main.tf
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/do/modules/registry/variable.tf
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/do/modules/registry/versions.tf
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/existing/main.tf
+-rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/gcp/main.tf
+-rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/gcp/outputs.tf
+-rw-r--r--   0        0        0     2485 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/gcp/variables.tf
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/gcp/versions.tf
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/gcp/modules/kubernetes/locals.tf
+-rw-r--r--   0        0        0     3324 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/gcp/modules/kubernetes/main.tf
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/gcp/modules/kubernetes/outputs.tf
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/gcp/modules/kubernetes/service_account.tf
+-rw-r--r--   0        0        0     3896 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/gcp/modules/kubernetes/variables.tf
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/gcp/modules/kubernetes/templates/kubeconfig.yaml
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/gcp/modules/network/main.tf
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/gcp/modules/network/variables.tf
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/gcp/modules/registry/main.tf
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/gcp/modules/registry/variables.tf
+-rw-r--r--   0        0        0     2497 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/local/main.tf
+-rw-r--r--   0        0        0     7993 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/local/metallb.yaml
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/local/outputs.tf
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/local/variables.tf
+-rw-r--r--   0        0        0     9630 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_ingress/__init__.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_ingress/template/locals.tf
+-rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_ingress/template/main.tf
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_ingress/template/outputs.tf
+-rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_ingress/template/variables.tf
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_ingress/template/versions.tf
+-rw-r--r--   0        0        0     9777 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_ingress/template/modules/kubernetes/ingress/main.tf
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_ingress/template/modules/kubernetes/ingress/outputs.tf
+-rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_ingress/template/modules/kubernetes/ingress/variables.tf
+-rw-r--r--   0        0        0     4257 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_initialize/__init__.py
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_initialize/template/external-container-registry.tf
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_initialize/template/locals.tf
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_initialize/template/main.tf
+-rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_initialize/template/variables.tf
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_initialize/template/versions.tf
+-rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_initialize/template/modules/cluster-autoscaler/main.tf
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_initialize/template/modules/cluster-autoscaler/variables.tf
+-rw-r--r--   0        0        0     7691 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_initialize/template/modules/extcr/main.tf
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_initialize/template/modules/extcr/variables.tf
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_initialize/template/modules/initialization/main.tf
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_initialize/template/modules/initialization/variables.tf
+-rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_initialize/template/modules/nvidia-installer/aws-nvidia-installer.tf
+-rw-r--r--   0        0        0     3739 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_initialize/template/modules/nvidia-installer/gcp-nvidia-installer.tf
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_initialize/template/modules/nvidia-installer/variables.tf
+-rw-r--r--   0        0        0    57723 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_initialize/template/modules/traefik_crds/main.tf
+-rw-r--r--   0        0        0     9398 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_keycloak/__init__.py
+-rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_keycloak/template/main.tf
+-rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_keycloak/template/outputs.tf
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_keycloak/template/variables.tf
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_keycloak/template/versions.tf
+-rw-r--r--   0        0        0     1489 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_keycloak/template/modules/kubernetes/keycloak-helm/main.tf
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_keycloak/template/modules/kubernetes/keycloak-helm/outputs.tf
+-rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_keycloak/template/modules/kubernetes/keycloak-helm/values.yaml
+-rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_keycloak/template/modules/kubernetes/keycloak-helm/variables.tf
+-rw-r--r--   0        0        0     3977 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_keycloak_configuration/__init__.py
+-rw-r--r--   0        0        0     3365 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_keycloak_configuration/template/main.tf
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_keycloak_configuration/template/outputs.tf
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_keycloak_configuration/template/permissions.tf
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_keycloak_configuration/template/providers.tf
+-rw-r--r--   0        0        0     2637 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_keycloak_configuration/template/social_auth.tf
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_keycloak_configuration/template/variables.tf
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_keycloak_configuration/template/versions.tf
+-rw-r--r--   0        0        0    22258 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/__init__.py
+-rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/argo-workflows.tf
+-rw-r--r--   0        0        0     2460 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/conda-store.tf
+-rw-r--r--   0        0        0     1378 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/dask_gateway.tf
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/forward-auth.tf
+-rw-r--r--   0        0        0     4481 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/jupyterhub.tf
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/jupyterhub_ssh.tf
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/locals.tf
+-rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/monitoring.tf
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/outputs.tf
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/providers.tf
+-rw-r--r--   0        0        0     2018 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/variables.tf
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/versions.tf
+-rw-r--r--   0        0        0     4548 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/forwardauth/main.tf
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/forwardauth/variables.tf
+-rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/nfs-mount/main.tf
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/nfs-mount/outputs.tf
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/nfs-mount/variables.tf
+-rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/nfs-server/main.tf
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/nfs-server/output.tf
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/nfs-server/variables.tf
+-rw-r--r--   0        0        0    16354 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/argo-workflows/main.tf
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/argo-workflows/values.yaml
+-rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/argo-workflows/variables.tf
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/argo-workflows/versions.tf
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/conda-store/output.tf
+-rw-r--r--   0        0        0     5210 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/conda-store/server.tf
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/conda-store/storage.tf
+-rw-r--r--   0        0        0     1813 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/conda-store/variables.tf
+-rw-r--r--   0        0        0     4560 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/conda-store/worker.tf
+-rw-r--r--   0        0        0     6543 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/conda-store/config/conda_store_config.py
+-rw-r--r--   0        0        0     3917 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/controler.tf
+-rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/crds.tf
+-rw-r--r--   0        0        0     6381 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/gateway.tf
+-rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/main.tf
+-rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/middleware.tf
+-rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/outputs.tf
+-rw-r--r--   0        0        0     5507 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/variables.tf
+-rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/files/controller_config.py
+-rw-r--r--   0        0        0    10699 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/files/gateway_config.py
+-rw-r--r--   0        0        0     4140 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/configmaps.tf
+-rw-r--r--   0        0        0     9424 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/main.tf
+-rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/middleware.tf
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/outputs.tf
+-rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/values.yaml
+-rw-r--r--   0        0        0     4723 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/variables.tf
+-rw-r--r--   0        0        0     3947 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/extras/git_clone_update.sh
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/ipython/ipython_config.py
+-rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/jupyter/jupyter_jupyterlab_pioneer_config.py.tpl
+-rw-r--r--   0        0        0     2323 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/jupyter/jupyter_server_config.py.tpl
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/jupyterhub/01-theme.py
+-rw-r--r--   0        0        0     2728 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/jupyterhub/02-spawner.py
+-rw-r--r--   0        0        0    19781 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/jupyterhub/03-profiles.py
+-rw-r--r--   0        0        0     4347 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/jupyterlab/overrides.json
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/skel/.bash_logout
+-rw-r--r--   0        0        0     4768 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/skel/.bashrc
+-rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/skel/.profile
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub-ssh/main.tf
+-rw-r--r--   0        0        0     2909 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub-ssh/sftp.tf
+-rw-r--r--   0        0        0     3127 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub-ssh/ssh.tf
+-rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub-ssh/variables.tf
+-rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/keycloak-client/main.tf
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/keycloak-client/outputs.tf
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/keycloak-client/variables.tf
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/keycloak-client/versions.tf
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/minio/ingress.tf
+-rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/minio/main.tf
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/minio/outputs.tf
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/minio/values.yaml
+-rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/minio/variables.tf
+-rw-r--r--   0        0        0     9352 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/main.tf
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/values.yaml
+-rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/variables.tf
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/versions.tf
+-rw-r--r--   0        0        0    26841 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/dashboards/Main/cluster_information.json
+-rw-r--r--   0        0        0    15913 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/dashboards/Main/conda_store.json
+-rw-r--r--   0        0        0    34598 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/dashboards/Main/jupyterhub_dashboard.json
+-rw-r--r--   0        0        0    52146 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/dashboards/Main/keycloak.json
+-rw-r--r--   0        0        0    28438 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/dashboards/Main/traefik.json
+-rw-r--r--   0        0        0     7418 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/dashboards/Main/usage_report.json
+-rw-r--r--   0        0        0     2651 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/loki/main.tf
+-rw-r--r--   0        0        0     2625 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/loki/values_loki.yaml
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/loki/values_minio.yaml
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/loki/values_promtail.yaml
+-rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/loki/variables.tf
+-rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/postgresql/main.tf
+-rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/postgresql/outputs.tf
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/postgresql/values.yaml
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/postgresql/variables.tf
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/redis/main.tf
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/redis/outputs.tf
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/redis/values.yaml
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/redis/variables.tf
+-rw-r--r--   0        0        0     2211 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/nebari_tf_extensions/__init__.py
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/nebari_tf_extensions/template/helm-extension.tf
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/nebari_tf_extensions/template/nebari-config.tf
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/nebari_tf_extensions/template/providers.tf
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/nebari_tf_extensions/template/tf-extensions.tf
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/nebari_tf_extensions/template/variables.tf
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/nebari_tf_extensions/template/versions.tf
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/nebari_tf_extensions/template/modules/helm-extensions/main.tf
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/nebari_tf_extensions/template/modules/helm-extensions/variables.tf
+-rw-r--r--   0        0        0     1380 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/nebari_tf_extensions/template/modules/nebariextension/ingress.tf
+-rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/nebari_tf_extensions/template/modules/nebariextension/keycloak-config.tf
+-rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/nebari_tf_extensions/template/modules/nebariextension/locals.tf
+-rw-r--r--   0        0        0     2044 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/nebari_tf_extensions/template/modules/nebariextension/main.tf
+-rw-r--r--   0        0        0     1470 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/nebari_tf_extensions/template/modules/nebariextension/variables.tf
+-rw-r--r--   0        0        0     9878 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/terraform_state/__init__.py
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/terraform_state/template/aws/main.tf
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/terraform_state/template/aws/modules/terraform-state/main.tf
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/terraform_state/template/aws/modules/terraform-state/output.tf
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/terraform_state/template/aws/modules/terraform-state/variables.tf
+-rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/terraform_state/template/azure/main.tf
+-rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/terraform_state/template/azure/modules/terraform-state/main.tf
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/terraform_state/template/azure/modules/terraform-state/variables.tf
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/terraform_state/template/do/main.tf
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/terraform_state/template/do/modules/spaces/main.tf
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/terraform_state/template/do/modules/spaces/variables.tf
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/terraform_state/template/do/modules/spaces/versions.tf
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/terraform_state/template/do/modules/terraform-state/main.tf
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/terraform_state/template/do/modules/terraform-state/variables.tf
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/terraform_state/template/do/modules/terraform-state/versions.tf
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/terraform_state/template/existing/main.tf
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/terraform_state/template/gcp/main.tf
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/terraform_state/template/gcp/modules/gcs/main.tf
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/terraform_state/template/gcp/modules/gcs/variables.tf
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/terraform_state/template/gcp/modules/terraform-state/main.tf
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/terraform_state/template/gcp/modules/terraform-state/variables.tf
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/stages/terraform_state/template/local/main.tf
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/subcommands/__init__.py
+-rw-r--r--   0        0        0     3191 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/subcommands/deploy.py
+-rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/subcommands/destroy.py
+-rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/subcommands/dev.py
+-rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/subcommands/info.py
+-rw-r--r--   0        0        0    36979 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/subcommands/init.py
+-rw-r--r--   0        0        0     2714 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/subcommands/keycloak.py
+-rw-r--r--   0        0        0     1316 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/subcommands/render.py
+-rw-r--r--   0        0        0     3032 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/subcommands/support.py
+-rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/subcommands/upgrade.py
+-rw-r--r--   0        0        0     1380 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/_nebari/subcommands/validate.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/nebari/__init__.py
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/nebari/__main__.py
+-rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/nebari/hookspecs.py
+-rw-r--r--   0        0        0     4350 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/nebari/plugins.py
+-rw-r--r--   0        0        0     3226 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/src/nebari/schema.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/__init__.py
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/conftest.py
+-rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/common/__init__.py
+-rw-r--r--   0        0        0     4206 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/common/config_mod_utils.py
+-rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/common/kube_api.py
+-rw-r--r--   0        0        0    16519 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/common/navigator.py
+-rw-r--r--   0        0        0     2410 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/common/playwright_fixtures.py
+-rw-r--r--   0        0        0    10512 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/common/run_notebook.py
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/common/notebooks/test_notebook_output.ipynb
+-rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/common/tests/test_notebook.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_deployment/__init__.py
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_deployment/constants.py
+-rw-r--r--   0        0        0     1497 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_deployment/test_dask_gateway.py
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_deployment/test_grafana_api.py
+-rw-r--r--   0        0        0     4101 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_deployment/test_jupyterhub_ssh.py
+-rw-r--r--   0        0        0     4329 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_deployment/test_loki_deployment.py
+-rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_deployment/utils.py
+-rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_deployment/assets/notebook/simple.ipynb
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_e2e/.gitignore
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_e2e/cypress.json
+-rw-r--r--   0        0        0   147508 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_e2e/package-lock.json
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_e2e/package.json
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_e2e/cypress/.gitignore
+-rw-r--r--   0        0        0     2946 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_e2e/cypress/integration/main.js
+-rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_e2e/cypress/notebooks/BasicTest.ipynb
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_e2e/cypress/plugins/index.js
+-rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_e2e/cypress/support/index.js
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_e2e/playwright/.env.tpl
+-rw-r--r--   0        0        0     7127 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_e2e/playwright/README.md
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_e2e/playwright/test_playwright.py
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_integration/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_integration/__init__.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_integration/conftest.py
+-rw-r--r--   0        0        0     7102 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_integration/deployment_fixtures.py
+-rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_integration/test_all_clouds.py
+-rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_integration/test_gpu.py
+-rw-r--r--   0        0        0     1240 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_integration/test_preemptible.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_unit/__init__.py
+-rw-r--r--   0        0        0     5968 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_unit/conftest.py
+-rw-r--r--   0        0        0     1877 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_unit/test_cli.py
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_unit/test_cli_deploy.py
+-rw-r--r--   0        0        0     7261 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_unit/test_cli_dev.py
+-rw-r--r--   0        0        0     9330 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_unit/test_cli_init.py
+-rw-r--r--   0        0        0     6479 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_unit/test_cli_init_repository.py
+-rw-r--r--   0        0        0    14131 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_unit/test_cli_keycloak.py
+-rw-r--r--   0        0        0     6529 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_unit/test_cli_support.py
+-rw-r--r--   0        0        0    18509 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_unit/test_cli_upgrade.py
+-rw-r--r--   0        0        0    10415 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_unit/test_cli_validate.py
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_unit/test_commons.py
+-rw-r--r--   0        0        0     5037 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_unit/test_config.py
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_unit/test_dependencies.py
+-rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_unit/test_init.py
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_unit/test_links.py
+-rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_unit/test_provider.py
+-rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_unit/test_render.py
+-rw-r--r--   0        0        0     5172 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_unit/test_schema.py
+-rw-r--r--   0        0        0     4441 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_unit/test_upgrade.py
+-rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_unit/utils.py
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_unit/cli_validate/aws.error.kubernetes-version.yaml
+-rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_unit/cli_validate/aws.happy.yaml
+-rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_unit/cli_validate/azure.happy.yaml
+-rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_unit/cli_validate/do.happy.yaml
+-rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_unit/cli_validate/gcp.happy.yaml
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_unit/cli_validate/local.error.authentication-type-called-custom.yaml
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_unit/cli_validate/local.error.extra-fields.yaml
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_unit/cli_validate/local.error.project_name.ends_with_special.yaml
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_unit/cli_validate/local.error.project_name.starts_with_number.yaml
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_unit/cli_validate/local.error.project_name.too_long.yaml
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_unit/cli_validate/local.happy.auth0.yaml
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_unit/cli_validate/local.happy.github.yaml
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_unit/cli_validate/local.happy.project_name.with_numbers.yaml
+-rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_unit/cli_validate/local.happy.yaml
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_unit/cli_validate/min.happy.jupyterlab.default_settings.yaml
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_unit/cli_validate/min.happy.monitoring.overrides.yaml
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_unit/cli_validate/min.happy.yaml
+-rw-r--r--   0        0        0     3456 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_unit/qhub-config-yaml-files-for-upgrade/qhub-config-do-310-customauth.yaml
+-rw-r--r--   0        0        0     3344 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_unit/qhub-config-yaml-files-for-upgrade/qhub-config-do-310.yaml
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/tests/tests_unit/qhub-config-yaml-files-for-upgrade/qhub-users-import.json
+-rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/.gitignore
+-rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/LICENSE
+-rw-r--r--   0        0        0     9814 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/README.md
+-rw-r--r--   0        0        0     3831 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/pyproject.toml
+-rw-r--r--   0        0        0    12409 2020-02-02 00:00:00.000000 nebari-2024.4.1rc1/PKG-INFO
```

### Comparing `nebari-2024.3.3rc1/.cirun.yml` & `nebari-2024.4.1rc1/.cirun.yml`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/.pre-commit-config.yaml` & `nebari-2024.4.1rc1/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -47,21 +47,21 @@
             "--ignore-words-list=AKS,aks",
             "--write",
           ]
         language: python
 
   # python
   - repo: https://github.com/psf/black
-    rev: 24.1.1
+    rev: 24.3.0
     hooks:
       - id: black
         args: ["--line-length=88", "--exclude=/src/_nebari/template/"]
 
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: v0.2.0
+    rev: v0.3.5
     hooks:
       - id: ruff
         args: ["--fix"]
 
   - repo: https://github.com/pycqa/isort
     rev: 5.13.2
     hooks:
@@ -69,12 +69,12 @@
         name: isort
         additional_dependencies: [toml]
         files: \.py$
         args: ["--profile", "black"]
 
   # terraform
   - repo: https://github.com/antonbabenko/pre-commit-terraform
-    rev: v1.86.0
+    rev: v1.88.4
     hooks:
       - id: terraform_fmt
         args:
           - --args=-write=true
```

### Comparing `nebari-2024.3.3rc1/CODE_OF_CONDUCT.md` & `nebari-2024.4.1rc1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/CONTRIBUTING.md` & `nebari-2024.4.1rc1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/RELEASE.md` & `nebari-2024.4.1rc1/RELEASE.md`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,35 @@
 <!-- Note:
 The RELEASE.md file at the root of the Nebari codebase is the source of truth for all release notes.
 If you want to update the release notes, open a PR against nebari-dev/nebari.
 This file is copied to nebari-dev/nebari-docs using a GitHub Action. -->
 
 ---
 
+## Release 2024.3.3 - March 27, 2024
+
+### What's Changed
+* get default variable value when following a terraform variable by @Adam-D-Lewis in https://github.com/nebari-dev/nebari/pull/2322
+* Upgrade Actions versions by @isumitjha in https://github.com/nebari-dev/nebari/pull/2291
+* Cleanup spawner logs by @krassowski in https://github.com/nebari-dev/nebari/pull/2328
+* Fix loki gateway url when deployed on non-dev namespace by @aktech in https://github.com/nebari-dev/nebari/pull/2327
+* Dmcandrew update ruamel.yaml by @dcmcand in https://github.com/nebari-dev/nebari/pull/2315
+* upgrade auth0-python version to ultimately resolve CVE-2024-26130 by @tylergraff in https://github.com/nebari-dev/nebari/pull/2314
+* remove deprecated code paths by @Adam-D-Lewis in https://github.com/nebari-dev/nebari/pull/2349
+* Create SECURITY.md by @dcmcand in https://github.com/nebari-dev/nebari/pull/2354
+* Set node affinity for more pods to ensure they run on general node pool by @Adam-D-Lewis in https://github.com/nebari-dev/nebari/pull/2353
+* Deduplicate conda-store in JupyterLab main menu by @krassowski in https://github.com/nebari-dev/nebari/pull/2347
+* Pass current namespace to argo via environment variable by @krassowski in https://github.com/nebari-dev/nebari/pull/2317
+* PVC for Traefik Ingress (prevent LetsEncrypt throttling) by @kenafoster in https://github.com/nebari-dev/nebari/pull/2352
+
+### New Contributors
+* @isumitjha made their first contribution in https://github.com/nebari-dev/nebari/pull/2291
+* @tylergraff made their first contribution in https://github.com/nebari-dev/nebari/pull/2314
+
+**Full Changelog**: https://github.com/nebari-dev/nebari/compare/2024.3.2...2024.3.3
 
 ## Release 2024.3.2 - March 14, 2024
 
 ### What's Changed
 * update max k8s versions and remove depreciated api usage in local deploy by @dcmcand in https://github.com/nebari-dev/nebari/pull/2276
 * update keycloak image repo by @Adam-D-Lewis in https://github.com/nebari-dev/nebari/pull/2312
 * Generate random password for Grafana by @aktech in https://github.com/nebari-dev/nebari/pull/2289
```

### Comparing `nebari-2024.3.3rc1/SECURITY.md` & `nebari-2024.4.1rc1/SECURITY.md`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/flake.lock` & `nebari-2024.4.1rc1/flake.lock`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/flake.nix` & `nebari-2024.4.1rc1/flake.nix`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/.github/PULL_REQUEST_TEMPLATE.md` & `nebari-2024.4.1rc1/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/.github/ISSUE_TEMPLATE/bug-report.yml` & `nebari-2024.4.1rc1/.github/ISSUE_TEMPLATE/bug-report.yml`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/.github/ISSUE_TEMPLATE/config.yml` & `nebari-2024.4.1rc1/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/.github/ISSUE_TEMPLATE/feature-request.yml` & `nebari-2024.4.1rc1/.github/ISSUE_TEMPLATE/feature-request.yml`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/.github/ISSUE_TEMPLATE/general-issue.yml` & `nebari-2024.4.1rc1/.github/ISSUE_TEMPLATE/general-issue.yml`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/.github/ISSUE_TEMPLATE/release-checklist.md` & `nebari-2024.4.1rc1/.github/ISSUE_TEMPLATE/release-checklist.md`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/.github/ISSUE_TEMPLATE/testing-checklist.md` & `nebari-2024.4.1rc1/.github/ISSUE_TEMPLATE/testing-checklist.md`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/.github/actions/publish-from-template/action.yml` & `nebari-2024.4.1rc1/.github/actions/publish-from-template/action.yml`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/.github/workflows/generate_cli_doc.yml` & `nebari-2024.4.1rc1/.github/workflows/generate_cli_doc.yml`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/.github/workflows/release-notes-sync.yaml` & `nebari-2024.4.1rc1/.github/workflows/release-notes-sync.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/.github/workflows/release.yaml` & `nebari-2024.4.1rc1/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/.github/workflows/run-precommit.yaml` & `nebari-2024.4.1rc1/.github/workflows/run-precommit.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/.github/workflows/test-provider.yaml` & `nebari-2024.4.1rc1/.github/workflows/test-provider.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/.github/workflows/test.yaml` & `nebari-2024.4.1rc1/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/.github/workflows/test_aws_integration.yaml` & `nebari-2024.4.1rc1/.github/workflows/test_aws_integration.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/.github/workflows/test_conda_build.yaml` & `nebari-2024.4.1rc1/.github/workflows/test_conda_build.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/.github/workflows/test_do_integration.yaml` & `nebari-2024.4.1rc1/.github/workflows/test_do_integration.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/.github/workflows/test_gcp_integration.yaml` & `nebari-2024.4.1rc1/.github/workflows/test_gcp_integration.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/.github/workflows/test_helm_charts.yaml` & `nebari-2024.4.1rc1/.github/workflows/test_helm_charts.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/.github/workflows/test_local_integration.yaml` & `nebari-2024.4.1rc1/.github/workflows/test_local_integration.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/.github/workflows/typing.yaml` & `nebari-2024.4.1rc1/.github/workflows/typing.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/docs-sphinx/Makefile` & `nebari-2024.4.1rc1/docs-sphinx/Makefile`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/docs-sphinx/README.md` & `nebari-2024.4.1rc1/docs-sphinx/README.md`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/docs-sphinx/cli.html` & `nebari-2024.4.1rc1/docs-sphinx/cli.html`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/scripts/aws-force-destroy.py` & `nebari-2024.4.1rc1/scripts/aws-force-destroy.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/scripts/aws-force-destroy.sh` & `nebari-2024.4.1rc1/scripts/aws-force-destroy.sh`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/scripts/helm-validate.py` & `nebari-2024.4.1rc1/scripts/helm-validate.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/scripts/keycloak-export.py` & `nebari-2024.4.1rc1/scripts/keycloak-export.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/cli.py` & `nebari-2024.4.1rc1/src/_nebari/cli.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/config.py` & `nebari-2024.4.1rc1/src/_nebari/config.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/constants.py` & `nebari-2024.4.1rc1/src/_nebari/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-CURRENT_RELEASE = "2024.3.2"
+CURRENT_RELEASE = "2024.3.3"
 
 # NOTE: Terraform cannot be upgraded further due to Hashicorp licensing changes
 # implemented in August 2023.
 # https://www.hashicorp.com/license-faq
 TERRAFORM_VERSION = "1.5.7"
 
 # 04-kubernetes-ingress
```

### Comparing `nebari-2024.3.3rc1/src/_nebari/deploy.py` & `nebari-2024.4.1rc1/src/_nebari/deploy.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/destroy.py` & `nebari-2024.4.1rc1/src/_nebari/destroy.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/initialize.py` & `nebari-2024.4.1rc1/src/_nebari/initialize.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,647 +22,683 @@
 00000150: 205f 6e65 6261 7269 2e70 726f 7669 6465   _nebari.provide
 00000160: 722e 6f61 7574 682e 6175 7468 3020 696d  r.oauth.auth0 im
 00000170: 706f 7274 2063 7265 6174 655f 636c 6965  port create_clie
 00000180: 6e74 0a66 726f 6d20 5f6e 6562 6172 692e  nt.from _nebari.
 00000190: 7374 6167 6573 2e62 6f6f 7473 7472 6170  stages.bootstrap
 000001a0: 2069 6d70 6f72 7420 4369 456e 756d 0a66   import CiEnum.f
 000001b0: 726f 6d20 5f6e 6562 6172 692e 7374 6167  rom _nebari.stag
-000001c0: 6573 2e6b 7562 6572 6e65 7465 735f 696e  es.kubernetes_in
-000001d0: 6772 6573 7320 696d 706f 7274 2043 6572  gress import Cer
-000001e0: 7469 6669 6361 7465 456e 756d 0a66 726f  tificateEnum.fro
-000001f0: 6d20 5f6e 6562 6172 692e 7374 6167 6573  m _nebari.stages
-00000200: 2e6b 7562 6572 6e65 7465 735f 6b65 7963  .kubernetes_keyc
-00000210: 6c6f 616b 2069 6d70 6f72 7420 4175 7468  loak import Auth
-00000220: 656e 7469 6361 7469 6f6e 456e 756d 0a66  enticationEnum.f
-00000230: 726f 6d20 5f6e 6562 6172 692e 7374 6167  rom _nebari.stag
-00000240: 6573 2e74 6572 7261 666f 726d 5f73 7461  es.terraform_sta
-00000250: 7465 2069 6d70 6f72 7420 5465 7272 6166  te import Terraf
-00000260: 6f72 6d53 7461 7465 456e 756d 0a66 726f  ormStateEnum.fro
-00000270: 6d20 5f6e 6562 6172 692e 7574 696c 7320  m _nebari.utils 
-00000280: 696d 706f 7274 2067 6574 5f6c 6174 6573  import get_lates
-00000290: 745f 6b75 6265 726e 6574 6573 5f76 6572  t_kubernetes_ver
-000002a0: 7369 6f6e 2c20 7261 6e64 6f6d 5f73 6563  sion, random_sec
-000002b0: 7572 655f 7374 7269 6e67 0a66 726f 6d20  ure_string.from 
-000002c0: 5f6e 6562 6172 692e 7665 7273 696f 6e20  _nebari.version 
-000002d0: 696d 706f 7274 205f 5f76 6572 7369 6f6e  import __version
-000002e0: 5f5f 0a66 726f 6d20 6e65 6261 7269 2e73  __.from nebari.s
-000002f0: 6368 656d 6120 696d 706f 7274 2050 726f  chema import Pro
-00000300: 7669 6465 7245 6e75 6d2c 2067 6974 6875  viderEnum, githu
-00000310: 625f 7572 6c5f 7265 6765 780a 0a6c 6f67  b_url_regex..log
-00000320: 6765 7220 3d20 6c6f 6767 696e 672e 6765  ger = logging.ge
-00000330: 744c 6f67 6765 7228 5f5f 6e61 6d65 5f5f  tLogger(__name__
-00000340: 290a 0a57 454c 434f 4d45 5f48 4541 4445  )..WELCOME_HEADE
-00000350: 525f 5445 5854 203d 2022 596f 7572 206f  R_TEXT = "Your o
-00000360: 7065 6e20 736f 7572 6365 2064 6174 6120  pen source data 
-00000370: 7363 6965 6e63 6520 706c 6174 666f 726d  science platform
-00000380: 2c20 686f 7374 6564 220a 0a0a 6465 6620  , hosted"...def 
-00000390: 7265 6e64 6572 5f63 6f6e 6669 6728 0a20  render_config(. 
-000003a0: 2020 2070 726f 6a65 6374 5f6e 616d 653a     project_name:
-000003b0: 2073 7472 2c0a 2020 2020 6e65 6261 7269   str,.    nebari
-000003c0: 5f64 6f6d 6169 6e3a 2073 7472 203d 204e  _domain: str = N
-000003d0: 6f6e 652c 0a20 2020 2063 6c6f 7564 5f70  one,.    cloud_p
-000003e0: 726f 7669 6465 723a 2050 726f 7669 6465  rovider: Provide
-000003f0: 7245 6e75 6d20 3d20 5072 6f76 6964 6572  rEnum = Provider
-00000400: 456e 756d 2e6c 6f63 616c 2c0a 2020 2020  Enum.local,.    
-00000410: 6369 5f70 726f 7669 6465 723a 2043 6945  ci_provider: CiE
-00000420: 6e75 6d20 3d20 4369 456e 756d 2e6e 6f6e  num = CiEnum.non
-00000430: 652c 0a20 2020 2072 6570 6f73 6974 6f72  e,.    repositor
-00000440: 793a 2073 7472 203d 204e 6f6e 652c 0a20  y: str = None,. 
-00000450: 2020 2061 7574 685f 7072 6f76 6964 6572     auth_provider
-00000460: 3a20 4175 7468 656e 7469 6361 7469 6f6e  : Authentication
-00000470: 456e 756d 203d 2041 7574 6865 6e74 6963  Enum = Authentic
-00000480: 6174 696f 6e45 6e75 6d2e 7061 7373 776f  ationEnum.passwo
-00000490: 7264 2c0a 2020 2020 6e61 6d65 7370 6163  rd,.    namespac
-000004a0: 653a 2073 7472 203d 2022 6465 7622 2c0a  e: str = "dev",.
-000004b0: 2020 2020 7265 706f 7369 746f 7279 5f61      repository_a
-000004c0: 7574 6f5f 7072 6f76 6973 696f 6e3a 2062  uto_provision: b
-000004d0: 6f6f 6c20 3d20 4661 6c73 652c 0a20 2020  ool = False,.   
-000004e0: 2061 7574 685f 6175 746f 5f70 726f 7669   auth_auto_provi
-000004f0: 7369 6f6e 3a20 626f 6f6c 203d 2046 616c  sion: bool = Fal
-00000500: 7365 2c0a 2020 2020 7465 7272 6166 6f72  se,.    terrafor
-00000510: 6d5f 7374 6174 653a 2054 6572 7261 666f  m_state: Terrafo
-00000520: 726d 5374 6174 6545 6e75 6d20 3d20 5465  rmStateEnum = Te
-00000530: 7272 6166 6f72 6d53 7461 7465 456e 756d  rraformStateEnum
-00000540: 2e72 656d 6f74 652c 0a20 2020 206b 7562  .remote,.    kub
-00000550: 6572 6e65 7465 735f 7665 7273 696f 6e3a  ernetes_version:
-00000560: 2073 7472 203d 204e 6f6e 652c 0a20 2020   str = None,.   
-00000570: 2072 6567 696f 6e3a 2073 7472 203d 204e   region: str = N
-00000580: 6f6e 652c 0a20 2020 2064 6973 6162 6c65  one,.    disable
-00000590: 5f70 726f 6d70 743a 2062 6f6f 6c20 3d20  _prompt: bool = 
-000005a0: 4661 6c73 652c 0a20 2020 2073 736c 5f63  False,.    ssl_c
-000005b0: 6572 745f 656d 6169 6c3a 2073 7472 203d  ert_email: str =
-000005c0: 204e 6f6e 652c 0a29 3a0a 2020 2020 636f   None,.):.    co
-000005d0: 6e66 6967 203d 207b 0a20 2020 2020 2020  nfig = {.       
-000005e0: 2022 7072 6f76 6964 6572 223a 2063 6c6f   "provider": clo
-000005f0: 7564 5f70 726f 7669 6465 722c 0a20 2020  ud_provider,.   
-00000600: 2020 2020 2022 6e61 6d65 7370 6163 6522       "namespace"
-00000610: 3a20 6e61 6d65 7370 6163 652c 0a20 2020  : namespace,.   
-00000620: 2020 2020 2022 6e65 6261 7269 5f76 6572       "nebari_ver
-00000630: 7369 6f6e 223a 205f 5f76 6572 7369 6f6e  sion": __version
-00000640: 5f5f 2c0a 2020 2020 7d0a 0a20 2020 2069  __,.    }..    i
-00000650: 6620 7072 6f6a 6563 745f 6e61 6d65 2069  f project_name i
-00000660: 7320 4e6f 6e65 2061 6e64 206e 6f74 2064  s None and not d
-00000670: 6973 6162 6c65 5f70 726f 6d70 743a 0a20  isable_prompt:. 
-00000680: 2020 2020 2020 2070 726f 6a65 6374 5f6e         project_n
-00000690: 616d 6520 3d20 696e 7075 7428 2250 726f  ame = input("Pro
-000006a0: 7669 6465 2070 726f 6a65 6374 206e 616d  vide project nam
-000006b0: 653a 2022 290a 2020 2020 636f 6e66 6967  e: ").    config
-000006c0: 5b22 7072 6f6a 6563 745f 6e61 6d65 225d  ["project_name"]
-000006d0: 203d 2070 726f 6a65 6374 5f6e 616d 650a   = project_name.
-000006e0: 0a20 2020 2069 6620 6e65 6261 7269 5f64  .    if nebari_d
-000006f0: 6f6d 6169 6e20 6973 206e 6f74 204e 6f6e  omain is not Non
-00000700: 653a 0a20 2020 2020 2020 2063 6f6e 6669  e:.        confi
-00000710: 675b 2264 6f6d 6169 6e22 5d20 3d20 6e65  g["domain"] = ne
-00000720: 6261 7269 5f64 6f6d 6169 6e0a 0a20 2020  bari_domain..   
-00000730: 2063 6f6e 6669 675b 2263 695f 6364 225d   config["ci_cd"]
-00000740: 203d 207b 2274 7970 6522 3a20 6369 5f70   = {"type": ci_p
-00000750: 726f 7669 6465 727d 0a20 2020 2063 6f6e  rovider}.    con
-00000760: 6669 675b 2274 6572 7261 666f 726d 5f73  fig["terraform_s
-00000770: 7461 7465 225d 203d 207b 2274 7970 6522  tate"] = {"type"
-00000780: 3a20 7465 7272 6166 6f72 6d5f 7374 6174  : terraform_stat
-00000790: 657d 0a0a 2020 2020 2320 5361 7665 2064  e}..    # Save d
-000007a0: 6566 6175 6c74 2070 6173 7377 6f72 6420  efault password 
-000007b0: 746f 2066 696c 650a 2020 2020 6465 6661  to file.    defa
-000007c0: 756c 745f 7061 7373 776f 7264 5f66 696c  ult_password_fil
-000007d0: 656e 616d 6520 3d20 5061 7468 2874 656d  ename = Path(tem
-000007e0: 7066 696c 652e 6765 7474 656d 7064 6972  pfile.gettempdir
-000007f0: 2829 2920 2f20 224e 4542 4152 495f 4445  ()) / "NEBARI_DE
-00000800: 4641 554c 545f 5041 5353 574f 5244 220a  FAULT_PASSWORD".
-00000810: 2020 2020 636f 6e66 6967 5b22 7365 6375      config["secu
-00000820: 7269 7479 225d 203d 207b 0a20 2020 2020  rity"] = {.     
-00000830: 2020 2022 6b65 7963 6c6f 616b 223a 207b     "keycloak": {
-00000840: 2269 6e69 7469 616c 5f72 6f6f 745f 7061  "initial_root_pa
-00000850: 7373 776f 7264 223a 2072 616e 646f 6d5f  ssword": random_
-00000860: 7365 6375 7265 5f73 7472 696e 6728 6c65  secure_string(le
-00000870: 6e67 7468 3d33 3229 7d0a 2020 2020 7d0a  ngth=32)}.    }.
-00000880: 2020 2020 7769 7468 2064 6566 6175 6c74      with default
-00000890: 5f70 6173 7377 6f72 645f 6669 6c65 6e61  _password_filena
-000008a0: 6d65 2e6f 7065 6e28 2277 2229 2061 7320  me.open("w") as 
-000008b0: 663a 0a20 2020 2020 2020 2066 2e77 7269  f:.        f.wri
-000008c0: 7465 2863 6f6e 6669 675b 2273 6563 7572  te(config["secur
-000008d0: 6974 7922 5d5b 226b 6579 636c 6f61 6b22  ity"]["keycloak"
-000008e0: 5d5b 2269 6e69 7469 616c 5f72 6f6f 745f  ]["initial_root_
-000008f0: 7061 7373 776f 7264 225d 290a 2020 2020  password"]).    
-00000900: 6465 6661 756c 745f 7061 7373 776f 7264  default_password
-00000910: 5f66 696c 656e 616d 652e 6368 6d6f 6428  _filename.chmod(
-00000920: 306f 3730 3029 0a0a 2020 2020 636f 6e66  0o700)..    conf
-00000930: 6967 5b22 7468 656d 6522 5d20 3d20 7b22  ig["theme"] = {"
-00000940: 6a75 7079 7465 7268 7562 223a 207b 2268  jupyterhub": {"h
-00000950: 7562 5f74 6974 6c65 223a 2066 224e 6562  ub_title": f"Neb
-00000960: 6172 6920 2d20 7b20 7072 6f6a 6563 745f  ari - { project_
-00000970: 6e61 6d65 207d 227d 7d0a 2020 2020 636f  name }"}}.    co
-00000980: 6e66 6967 5b22 7468 656d 6522 5d5b 226a  nfig["theme"]["j
-00000990: 7570 7974 6572 6875 6222 5d5b 0a20 2020  upyterhub"][.   
-000009a0: 2020 2020 2022 7765 6c63 6f6d 6522 0a20       "welcome". 
-000009b0: 2020 205d 203d 2022 2222 5765 6c63 6f6d     ] = """Welcom
-000009c0: 6521 204c 6561 726e 2061 626f 7574 204e  e! Learn about N
-000009d0: 6562 6172 6927 7320 6665 6174 7572 6573  ebari's features
-000009e0: 2061 6e64 2063 6f6e 6669 6775 7261 7469   and configurati
-000009f0: 6f6e 7320 696e 203c 6120 6872 6566 3d22  ons in <a href="
-00000a00: 6874 7470 733a 2f2f 7777 772e 6e65 6261  https://www.neba
-00000a10: 7269 2e64 6576 2f64 6f63 732f 7765 6c63  ri.dev/docs/welc
-00000a20: 6f6d 6522 3e74 6865 2064 6f63 756d 656e  ome">the documen
-00000a30: 7461 7469 6f6e 3c2f 613e 2e20 4966 2079  tation</a>. If y
-00000a40: 6f75 2068 6176 6520 616e 7920 7175 6573  ou have any ques
-00000a50: 7469 6f6e 7320 6f72 2066 6565 6462 6163  tions or feedbac
-00000a60: 6b2c 2072 6561 6368 2074 6865 2074 6561  k, reach the tea
-00000a70: 6d20 6f6e 203c 6120 6872 6566 3d22 6874  m on <a href="ht
-00000a80: 7470 733a 2f2f 7777 772e 6e65 6261 7269  tps://www.nebari
-00000a90: 2e64 6576 2f64 6f63 732f 636f 6d6d 756e  .dev/docs/commun
-00000aa0: 6974 7923 6765 7474 696e 672d 7375 7070  ity#getting-supp
-00000ab0: 6f72 7422 3e4e 6562 6172 6927 7320 7375  ort">Nebari's su
-00000ac0: 7070 6f72 7420 666f 7275 6d73 3c2f 613e  pport forums</a>
-00000ad0: 2e22 2222 0a0a 2020 2020 636f 6e66 6967  ."""..    config
-00000ae0: 5b22 7365 6375 7269 7479 225d 5b22 6175  ["security"]["au
-00000af0: 7468 656e 7469 6361 7469 6f6e 225d 203d  thentication"] =
-00000b00: 207b 2274 7970 6522 3a20 6175 7468 5f70   {"type": auth_p
-00000b10: 726f 7669 6465 727d 0a0a 2020 2020 6966  rovider}..    if
-00000b20: 2061 7574 685f 7072 6f76 6964 6572 203d   auth_provider =
-00000b30: 3d20 4175 7468 656e 7469 6361 7469 6f6e  = Authentication
-00000b40: 456e 756d 2e67 6974 6875 623a 0a20 2020  Enum.github:.   
-00000b50: 2020 2020 2063 6f6e 6669 675b 2273 6563       config["sec
-00000b60: 7572 6974 7922 5d5b 2261 7574 6865 6e74  urity"]["authent
-00000b70: 6963 6174 696f 6e22 5d5b 2263 6f6e 6669  ication"]["confi
-00000b80: 6722 5d20 3d20 7b0a 2020 2020 2020 2020  g"] = {.        
-00000b90: 2020 2020 2263 6c69 656e 745f 6964 223a      "client_id":
-00000ba0: 206f 732e 656e 7669 726f 6e2e 6765 7428   os.environ.get(
-00000bb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000bc0: 2022 4749 5448 5542 5f43 4c49 454e 545f   "GITHUB_CLIENT_
-00000bd0: 4944 222c 0a20 2020 2020 2020 2020 2020  ID",.           
-00000be0: 2020 2020 2022 3c65 6e74 6572 2063 6c69       "<enter cli
-00000bf0: 656e 7420 6964 206f 7220 7265 6d6f 7665  ent id or remove
-00000c00: 2074 6f20 7573 6520 4749 5448 5542 5f43   to use GITHUB_C
-00000c10: 4c49 454e 545f 4944 2065 6e76 6972 6f6e  LIENT_ID environ
-00000c20: 6d65 6e74 2076 6172 6961 626c 6520 2870  ment variable (p
-00000c30: 7265 6665 7272 6564 293e 222c 0a20 2020  referred)>",.   
-00000c40: 2020 2020 2020 2020 2029 2c0a 2020 2020           ),.    
-00000c50: 2020 2020 2020 2020 2263 6c69 656e 745f          "client_
-00000c60: 7365 6372 6574 223a 206f 732e 656e 7669  secret": os.envi
-00000c70: 726f 6e2e 6765 7428 0a20 2020 2020 2020  ron.get(.       
-00000c80: 2020 2020 2020 2020 2022 4749 5448 5542           "GITHUB
-00000c90: 5f43 4c49 454e 545f 5345 4352 4554 222c  _CLIENT_SECRET",
-00000ca0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000cb0: 2022 3c65 6e74 6572 2063 6c69 656e 7420   "<enter client 
-00000cc0: 7365 6372 6574 206f 7220 7265 6d6f 7665  secret or remove
-00000cd0: 2074 6f20 7573 6520 4749 5448 5542 5f43   to use GITHUB_C
-00000ce0: 4c49 454e 545f 5345 4352 4554 2065 6e76  LIENT_SECRET env
-00000cf0: 6972 6f6e 6d65 6e74 2076 6172 6961 626c  ironment variabl
-00000d00: 6520 2870 7265 6665 7272 6564 293e 222c  e (preferred)>",
-00000d10: 0a20 2020 2020 2020 2020 2020 2029 2c0a  .            ),.
-00000d20: 2020 2020 2020 2020 7d0a 2020 2020 656c          }.    el
-00000d30: 6966 2061 7574 685f 7072 6f76 6964 6572  if auth_provider
-00000d40: 203d 3d20 4175 7468 656e 7469 6361 7469   == Authenticati
-00000d50: 6f6e 456e 756d 2e61 7574 6830 3a0a 2020  onEnum.auth0:.  
-00000d60: 2020 2020 2020 6966 2061 7574 685f 6175        if auth_au
-00000d70: 746f 5f70 726f 7669 7369 6f6e 3a0a 2020  to_provision:.  
-00000d80: 2020 2020 2020 2020 2020 6175 7468 305f            auth0_
-00000d90: 636f 6e66 6967 203d 2063 7265 6174 655f  config = create_
-00000da0: 636c 6965 6e74 2863 6f6e 6669 672e 646f  client(config.do
-00000db0: 6d61 696e 2c20 636f 6e66 6967 2e70 726f  main, config.pro
-00000dc0: 6a65 6374 5f6e 616d 6529 0a20 2020 2020  ject_name).     
-00000dd0: 2020 2020 2020 2063 6f6e 6669 675b 2273         config["s
-00000de0: 6563 7572 6974 7922 5d5b 2261 7574 6865  ecurity"]["authe
-00000df0: 6e74 6963 6174 696f 6e22 5d5b 2263 6f6e  ntication"]["con
-00000e00: 6669 6722 5d20 3d20 6175 7468 305f 636f  fig"] = auth0_co
-00000e10: 6e66 6967 0a20 2020 2020 2020 2065 6c73  nfig.        els
-00000e20: 653a 0a20 2020 2020 2020 2020 2020 2063  e:.            c
-00000e30: 6f6e 6669 675b 2273 6563 7572 6974 7922  onfig["security"
-00000e40: 5d5b 2261 7574 6865 6e74 6963 6174 696f  ]["authenticatio
-00000e50: 6e22 5d5b 2263 6f6e 6669 6722 5d20 3d20  n"]["config"] = 
-00000e60: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
-00000e70: 2020 2263 6c69 656e 745f 6964 223a 206f    "client_id": o
-00000e80: 732e 656e 7669 726f 6e2e 6765 7428 0a20  s.environ.get(. 
-00000e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000ea0: 2020 2022 4155 5448 305f 434c 4945 4e54     "AUTH0_CLIENT
-00000eb0: 5f49 4422 2c0a 2020 2020 2020 2020 2020  _ID",.          
-00000ec0: 2020 2020 2020 2020 2020 223c 656e 7465            "<ente
-00000ed0: 7220 636c 6965 6e74 2069 6420 6f72 2072  r client id or r
-00000ee0: 656d 6f76 6520 746f 2075 7365 2041 5554  emove to use AUT
-00000ef0: 4830 5f43 4c49 454e 545f 4944 2065 6e76  H0_CLIENT_ID env
-00000f00: 6972 6f6e 6d65 6e74 2076 6172 6961 626c  ironment variabl
-00000f10: 6520 2870 7265 6665 7272 6564 293e 222c  e (preferred)>",
-00000f20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000f30: 2029 2c0a 2020 2020 2020 2020 2020 2020   ),.            
-00000f40: 2020 2020 2263 6c69 656e 745f 7365 6372      "client_secr
-00000f50: 6574 223a 206f 732e 656e 7669 726f 6e2e  et": os.environ.
-00000f60: 6765 7428 0a20 2020 2020 2020 2020 2020  get(.           
-00000f70: 2020 2020 2020 2020 2022 4155 5448 305f           "AUTH0_
-00000f80: 434c 4945 4e54 5f53 4543 5245 5422 2c0a  CLIENT_SECRET",.
-00000f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000fa0: 2020 2020 223c 656e 7465 7220 636c 6965      "<enter clie
-00000fb0: 6e74 2073 6563 7265 7420 6f72 2072 656d  nt secret or rem
-00000fc0: 6f76 6520 746f 2075 7365 2041 5554 4830  ove to use AUTH0
-00000fd0: 5f43 4c49 454e 545f 5345 4352 4554 2065  _CLIENT_SECRET e
-00000fe0: 6e76 6972 6f6e 6d65 6e74 2076 6172 6961  nvironment varia
-00000ff0: 626c 6520 2870 7265 6665 7272 6564 293e  ble (preferred)>
-00001000: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-00001010: 2020 2029 2c0a 2020 2020 2020 2020 2020     ),.          
-00001020: 2020 2020 2020 2261 7574 6830 5f73 7562        "auth0_sub
-00001030: 646f 6d61 696e 223a 206f 732e 656e 7669  domain": os.envi
-00001040: 726f 6e2e 6765 7428 0a20 2020 2020 2020  ron.get(.       
-00001050: 2020 2020 2020 2020 2020 2020 2022 4155               "AU
-00001060: 5448 305f 444f 4d41 494e 222c 0a20 2020  TH0_DOMAIN",.   
-00001070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001080: 2022 3c65 6e74 6572 2073 7562 646f 6d61   "<enter subdoma
-00001090: 696e 2028 7769 7468 6f75 7420 2e61 7574  in (without .aut
-000010a0: 6830 2e63 6f6d 2920 6f72 2072 656d 6f76  h0.com) or remov
-000010b0: 6520 746f 2075 7365 2041 5554 4830 5f44  e to use AUTH0_D
-000010c0: 4f4d 4149 4e20 656e 7669 726f 6e6d 656e  OMAIN environmen
-000010d0: 7420 7661 7269 6162 6c65 3e22 2c0a 2020  t variable>",.  
-000010e0: 2020 2020 2020 2020 2020 2020 2020 292c                ),
-000010f0: 0a20 2020 2020 2020 2020 2020 207d 0a0a  .            }..
-00001100: 2020 2020 6966 2063 6c6f 7564 5f70 726f      if cloud_pro
-00001110: 7669 6465 7220 3d3d 2050 726f 7669 6465  vider == Provide
-00001120: 7245 6e75 6d2e 646f 3a0a 2020 2020 2020  rEnum.do:.      
-00001130: 2020 646f 5f72 6567 696f 6e20 3d20 7265    do_region = re
-00001140: 6769 6f6e 206f 7220 636f 6e73 7461 6e74  gion or constant
-00001150: 732e 444f 5f44 4546 4155 4c54 5f52 4547  s.DO_DEFAULT_REG
-00001160: 494f 4e0a 2020 2020 2020 2020 646f 5f6b  ION.        do_k
-00001170: 7562 6572 6e65 7465 735f 7665 7273 696f  ubernetes_versio
-00001180: 6e73 203d 206b 7562 6572 6e65 7465 735f  ns = kubernetes_
-00001190: 7665 7273 696f 6e20 6f72 2067 6574 5f6c  version or get_l
-000011a0: 6174 6573 745f 6b75 6265 726e 6574 6573  atest_kubernetes
-000011b0: 5f76 6572 7369 6f6e 280a 2020 2020 2020  _version(.      
-000011c0: 2020 2020 2020 6469 6769 7461 6c5f 6f63        digital_oc
-000011d0: 6561 6e2e 6b75 6265 726e 6574 6573 5f76  ean.kubernetes_v
-000011e0: 6572 7369 6f6e 7328 646f 5f72 6567 696f  ersions(do_regio
-000011f0: 6e29 0a20 2020 2020 2020 2029 0a20 2020  n).        ).   
-00001200: 2020 2020 2063 6f6e 6669 675b 2264 6967       config["dig
-00001210: 6974 616c 5f6f 6365 616e 225d 203d 207b  ital_ocean"] = {
-00001220: 0a20 2020 2020 2020 2020 2020 2022 6b75  .            "ku
-00001230: 6265 726e 6574 6573 5f76 6572 7369 6f6e  bernetes_version
-00001240: 223a 2064 6f5f 6b75 6265 726e 6574 6573  ": do_kubernetes
-00001250: 5f76 6572 7369 6f6e 732c 0a20 2020 2020  _versions,.     
-00001260: 2020 2020 2020 2022 7265 6769 6f6e 223a         "region":
-00001270: 2064 6f5f 7265 6769 6f6e 2c0a 2020 2020   do_region,.    
-00001280: 2020 2020 7d0a 0a20 2020 2020 2020 2063      }..        c
-00001290: 6f6e 6669 675b 2274 6865 6d65 225d 5b22  onfig["theme"]["
-000012a0: 6a75 7079 7465 7268 7562 225d 5b0a 2020  jupyterhub"][.  
-000012b0: 2020 2020 2020 2020 2020 2268 7562 5f73            "hub_s
-000012c0: 7562 7469 746c 6522 0a20 2020 2020 2020  ubtitle".       
-000012d0: 205d 203d 2066 227b 5745 4c43 4f4d 455f   ] = f"{WELCOME_
-000012e0: 4845 4144 4552 5f54 4558 547d 206f 6e20  HEADER_TEXT} on 
-000012f0: 4469 6769 7461 6c20 4f63 6561 6e22 0a0a  Digital Ocean"..
-00001300: 2020 2020 656c 6966 2063 6c6f 7564 5f70      elif cloud_p
-00001310: 726f 7669 6465 7220 3d3d 2050 726f 7669  rovider == Provi
-00001320: 6465 7245 6e75 6d2e 6763 703a 0a20 2020  derEnum.gcp:.   
-00001330: 2020 2020 2067 6370 5f72 6567 696f 6e20       gcp_region 
-00001340: 3d20 7265 6769 6f6e 206f 7220 636f 6e73  = region or cons
-00001350: 7461 6e74 732e 4743 505f 4445 4641 554c  tants.GCP_DEFAUL
-00001360: 545f 5245 4749 4f4e 0a20 2020 2020 2020  T_REGION.       
-00001370: 2067 6370 5f6b 7562 6572 6e65 7465 735f   gcp_kubernetes_
-00001380: 7665 7273 696f 6e20 3d20 6b75 6265 726e  version = kubern
-00001390: 6574 6573 5f76 6572 7369 6f6e 206f 7220  etes_version or 
-000013a0: 6765 745f 6c61 7465 7374 5f6b 7562 6572  get_latest_kuber
-000013b0: 6e65 7465 735f 7665 7273 696f 6e28 0a20  netes_version(. 
-000013c0: 2020 2020 2020 2020 2020 2067 6f6f 676c             googl
-000013d0: 655f 636c 6f75 642e 6b75 6265 726e 6574  e_cloud.kubernet
-000013e0: 6573 5f76 6572 7369 6f6e 7328 6763 705f  es_versions(gcp_
-000013f0: 7265 6769 6f6e 290a 2020 2020 2020 2020  region).        
-00001400: 290a 2020 2020 2020 2020 636f 6e66 6967  ).        config
-00001410: 5b22 676f 6f67 6c65 5f63 6c6f 7564 5f70  ["google_cloud_p
-00001420: 6c61 7466 6f72 6d22 5d20 3d20 7b0a 2020  latform"] = {.  
-00001430: 2020 2020 2020 2020 2020 226b 7562 6572            "kuber
-00001440: 6e65 7465 735f 7665 7273 696f 6e22 3a20  netes_version": 
-00001450: 6763 705f 6b75 6265 726e 6574 6573 5f76  gcp_kubernetes_v
-00001460: 6572 7369 6f6e 2c0a 2020 2020 2020 2020  ersion,.        
-00001470: 2020 2020 2272 6567 696f 6e22 3a20 6763      "region": gc
-00001480: 705f 7265 6769 6f6e 2c0a 2020 2020 2020  p_region,.      
-00001490: 2020 7d0a 0a20 2020 2020 2020 2063 6f6e    }..        con
-000014a0: 6669 675b 2274 6865 6d65 225d 5b22 6a75  fig["theme"]["ju
-000014b0: 7079 7465 7268 7562 225d 5b0a 2020 2020  pyterhub"][.    
-000014c0: 2020 2020 2020 2020 2268 7562 5f73 7562          "hub_sub
-000014d0: 7469 746c 6522 0a20 2020 2020 2020 205d  title".        ]
-000014e0: 203d 2066 227b 5745 4c43 4f4d 455f 4845   = f"{WELCOME_HE
-000014f0: 4144 4552 5f54 4558 547d 206f 6e20 476f  ADER_TEXT} on Go
-00001500: 6f67 6c65 2043 6c6f 7564 2050 6c61 7466  ogle Cloud Platf
-00001510: 6f72 6d22 0a20 2020 2020 2020 2069 6620  orm".        if 
-00001520: 2250 524f 4a45 4354 5f49 4422 2069 6e20  "PROJECT_ID" in 
-00001530: 6f73 2e65 6e76 6972 6f6e 3a0a 2020 2020  os.environ:.    
-00001540: 2020 2020 2020 2020 636f 6e66 6967 5b22          config["
-00001550: 676f 6f67 6c65 5f63 6c6f 7564 5f70 6c61  google_cloud_pla
-00001560: 7466 6f72 6d22 5d5b 2270 726f 6a65 6374  tform"]["project
-00001570: 225d 203d 206f 732e 656e 7669 726f 6e5b  "] = os.environ[
-00001580: 2250 524f 4a45 4354 5f49 4422 5d0a 2020  "PROJECT_ID"].  
-00001590: 2020 2020 2020 656c 6966 206e 6f74 2064        elif not d
-000015a0: 6973 6162 6c65 5f70 726f 6d70 743a 0a20  isable_prompt:. 
-000015b0: 2020 2020 2020 2020 2020 2063 6f6e 6669             confi
-000015c0: 675b 2267 6f6f 676c 655f 636c 6f75 645f  g["google_cloud_
-000015d0: 706c 6174 666f 726d 225d 5b22 7072 6f6a  platform"]["proj
-000015e0: 6563 7422 5d20 3d20 696e 7075 7428 0a20  ect"] = input(. 
-000015f0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00001600: 456e 7465 7220 476f 6f67 6c65 2043 6c6f  Enter Google Clo
-00001610: 7564 2050 6c61 7466 6f72 6d20 5072 6f6a  ud Platform Proj
-00001620: 6563 7420 4944 3a20 220a 2020 2020 2020  ect ID: ".      
-00001630: 2020 2020 2020 290a 0a20 2020 2065 6c69        )..    eli
-00001640: 6620 636c 6f75 645f 7072 6f76 6964 6572  f cloud_provider
-00001650: 203d 3d20 5072 6f76 6964 6572 456e 756d   == ProviderEnum
-00001660: 2e61 7a75 7265 3a0a 2020 2020 2020 2020  .azure:.        
-00001670: 617a 7572 655f 7265 6769 6f6e 203d 2072  azure_region = r
-00001680: 6567 696f 6e20 6f72 2063 6f6e 7374 616e  egion or constan
-00001690: 7473 2e41 5a55 5245 5f44 4546 4155 4c54  ts.AZURE_DEFAULT
-000016a0: 5f52 4547 494f 4e0a 2020 2020 2020 2020  _REGION.        
-000016b0: 617a 7572 655f 6b75 6265 726e 6574 6573  azure_kubernetes
-000016c0: 5f76 6572 7369 6f6e 203d 206b 7562 6572  _version = kuber
-000016d0: 6e65 7465 735f 7665 7273 696f 6e20 6f72  netes_version or
-000016e0: 2067 6574 5f6c 6174 6573 745f 6b75 6265   get_latest_kube
-000016f0: 726e 6574 6573 5f76 6572 7369 6f6e 280a  rnetes_version(.
-00001700: 2020 2020 2020 2020 2020 2020 617a 7572              azur
-00001710: 655f 636c 6f75 642e 6b75 6265 726e 6574  e_cloud.kubernet
-00001720: 6573 5f76 6572 7369 6f6e 7328 617a 7572  es_versions(azur
-00001730: 655f 7265 6769 6f6e 290a 2020 2020 2020  e_region).      
-00001740: 2020 290a 2020 2020 2020 2020 636f 6e66    ).        conf
-00001750: 6967 5b22 617a 7572 6522 5d20 3d20 7b0a  ig["azure"] = {.
-00001760: 2020 2020 2020 2020 2020 2020 226b 7562              "kub
-00001770: 6572 6e65 7465 735f 7665 7273 696f 6e22  ernetes_version"
-00001780: 3a20 617a 7572 655f 6b75 6265 726e 6574  : azure_kubernet
-00001790: 6573 5f76 6572 7369 6f6e 2c0a 2020 2020  es_version,.    
-000017a0: 2020 2020 2020 2020 2272 6567 696f 6e22          "region"
-000017b0: 3a20 617a 7572 655f 7265 6769 6f6e 2c0a  : azure_region,.
-000017c0: 2020 2020 2020 2020 2020 2020 2273 746f              "sto
-000017d0: 7261 6765 5f61 6363 6f75 6e74 5f70 6f73  rage_account_pos
-000017e0: 7466 6978 223a 2072 616e 646f 6d5f 7365  tfix": random_se
-000017f0: 6375 7265 5f73 7472 696e 6728 6c65 6e67  cure_string(leng
-00001800: 7468 3d34 292c 0a20 2020 2020 2020 207d  th=4),.        }
-00001810: 0a0a 2020 2020 2020 2020 636f 6e66 6967  ..        config
-00001820: 5b22 7468 656d 6522 5d5b 226a 7570 7974  ["theme"]["jupyt
-00001830: 6572 6875 6222 5d5b 0a20 2020 2020 2020  erhub"][.       
-00001840: 2020 2020 2022 6875 625f 7375 6274 6974       "hub_subtit
-00001850: 6c65 220a 2020 2020 2020 2020 5d20 3d20  le".        ] = 
-00001860: 6622 7b57 454c 434f 4d45 5f48 4541 4445  f"{WELCOME_HEADE
-00001870: 525f 5445 5854 7d20 6f6e 2041 7a75 7265  R_TEXT} on Azure
-00001880: 220a 0a20 2020 2065 6c69 6620 636c 6f75  "..    elif clou
-00001890: 645f 7072 6f76 6964 6572 203d 3d20 5072  d_provider == Pr
-000018a0: 6f76 6964 6572 456e 756d 2e61 7773 3a0a  oviderEnum.aws:.
-000018b0: 2020 2020 2020 2020 6177 735f 7265 6769          aws_regi
-000018c0: 6f6e 203d 2028 0a20 2020 2020 2020 2020  on = (.         
-000018d0: 2020 2072 6567 696f 6e0a 2020 2020 2020     region.      
-000018e0: 2020 2020 2020 6f72 206f 732e 656e 7669        or os.envi
-000018f0: 726f 6e2e 6765 7428 2241 5753 5f44 4546  ron.get("AWS_DEF
-00001900: 4155 4c54 5f52 4547 494f 4e22 290a 2020  AULT_REGION").  
-00001910: 2020 2020 2020 2020 2020 6f72 2063 6f6e            or con
-00001920: 7374 616e 7473 2e41 5753 5f44 4546 4155  stants.AWS_DEFAU
-00001930: 4c54 5f52 4547 494f 4e0a 2020 2020 2020  LT_REGION.      
-00001940: 2020 290a 2020 2020 2020 2020 6177 735f    ).        aws_
-00001950: 6b75 6265 726e 6574 6573 5f76 6572 7369  kubernetes_versi
-00001960: 6f6e 203d 206b 7562 6572 6e65 7465 735f  on = kubernetes_
-00001970: 7665 7273 696f 6e20 6f72 2067 6574 5f6c  version or get_l
-00001980: 6174 6573 745f 6b75 6265 726e 6574 6573  atest_kubernetes
-00001990: 5f76 6572 7369 6f6e 280a 2020 2020 2020  _version(.      
-000019a0: 2020 2020 2020 616d 617a 6f6e 5f77 6562        amazon_web
-000019b0: 5f73 6572 7669 6365 732e 6b75 6265 726e  _services.kubern
-000019c0: 6574 6573 5f76 6572 7369 6f6e 7328 6177  etes_versions(aw
-000019d0: 735f 7265 6769 6f6e 290a 2020 2020 2020  s_region).      
-000019e0: 2020 290a 2020 2020 2020 2020 636f 6e66    ).        conf
-000019f0: 6967 5b22 616d 617a 6f6e 5f77 6562 5f73  ig["amazon_web_s
-00001a00: 6572 7669 6365 7322 5d20 3d20 7b0a 2020  ervices"] = {.  
-00001a10: 2020 2020 2020 2020 2020 226b 7562 6572            "kuber
-00001a20: 6e65 7465 735f 7665 7273 696f 6e22 3a20  netes_version": 
-00001a30: 6177 735f 6b75 6265 726e 6574 6573 5f76  aws_kubernetes_v
-00001a40: 6572 7369 6f6e 2c0a 2020 2020 2020 2020  ersion,.        
-00001a50: 2020 2020 2272 6567 696f 6e22 3a20 6177      "region": aw
-00001a60: 735f 7265 6769 6f6e 2c0a 2020 2020 2020  s_region,.      
-00001a70: 2020 7d0a 2020 2020 2020 2020 636f 6e66    }.        conf
-00001a80: 6967 5b22 7468 656d 6522 5d5b 226a 7570  ig["theme"]["jup
-00001a90: 7974 6572 6875 6222 5d5b 0a20 2020 2020  yterhub"][.     
-00001aa0: 2020 2020 2020 2022 6875 625f 7375 6274         "hub_subt
-00001ab0: 6974 6c65 220a 2020 2020 2020 2020 5d20  itle".        ] 
-00001ac0: 3d20 6622 7b57 454c 434f 4d45 5f48 4541  = f"{WELCOME_HEA
-00001ad0: 4445 525f 5445 5854 7d20 6f6e 2041 6d61  DER_TEXT} on Ama
-00001ae0: 7a6f 6e20 5765 6220 5365 7276 6963 6573  zon Web Services
-00001af0: 220a 0a20 2020 2065 6c69 6620 636c 6f75  "..    elif clou
-00001b00: 645f 7072 6f76 6964 6572 203d 3d20 5072  d_provider == Pr
-00001b10: 6f76 6964 6572 456e 756d 2e65 7869 7374  oviderEnum.exist
-00001b20: 696e 673a 0a20 2020 2020 2020 2063 6f6e  ing:.        con
-00001b30: 6669 675b 2274 6865 6d65 225d 5b22 6a75  fig["theme"]["ju
-00001b40: 7079 7465 7268 7562 225d 5b22 6875 625f  pyterhub"]["hub_
-00001b50: 7375 6274 6974 6c65 225d 203d 2057 454c  subtitle"] = WEL
-00001b60: 434f 4d45 5f48 4541 4445 525f 5445 5854  COME_HEADER_TEXT
-00001b70: 0a0a 2020 2020 656c 6966 2063 6c6f 7564  ..    elif cloud
-00001b80: 5f70 726f 7669 6465 7220 3d3d 2050 726f  _provider == Pro
-00001b90: 7669 6465 7245 6e75 6d2e 6c6f 6361 6c3a  viderEnum.local:
-00001ba0: 0a20 2020 2020 2020 2063 6f6e 6669 675b  .        config[
-00001bb0: 2274 6865 6d65 225d 5b22 6a75 7079 7465  "theme"]["jupyte
-00001bc0: 7268 7562 225d 5b22 6875 625f 7375 6274  rhub"]["hub_subt
-00001bd0: 6974 6c65 225d 203d 2057 454c 434f 4d45  itle"] = WELCOME
-00001be0: 5f48 4541 4445 525f 5445 5854 0a0a 2020  _HEADER_TEXT..  
-00001bf0: 2020 6966 2073 736c 5f63 6572 745f 656d    if ssl_cert_em
-00001c00: 6169 6c3a 0a20 2020 2020 2020 2063 6f6e  ail:.        con
-00001c10: 6669 675b 2263 6572 7469 6669 6361 7465  fig["certificate
-00001c20: 225d 203d 207b 2274 7970 6522 3a20 4365  "] = {"type": Ce
-00001c30: 7274 6966 6963 6174 6545 6e75 6d2e 6c65  rtificateEnum.le
-00001c40: 7473 656e 6372 7970 742e 7661 6c75 657d  tsencrypt.value}
-00001c50: 0a20 2020 2020 2020 2063 6f6e 6669 675b  .        config[
-00001c60: 2263 6572 7469 6669 6361 7465 225d 5b22  "certificate"]["
-00001c70: 6163 6d65 5f65 6d61 696c 225d 203d 2073  acme_email"] = s
-00001c80: 736c 5f63 6572 745f 656d 6169 6c0a 0a20  sl_cert_email.. 
-00001c90: 2020 2023 2076 616c 6964 6174 6520 636f     # validate co
-00001ca0: 6e66 6967 7572 6174 696f 6e20 616e 6420  nfiguration and 
-00001cb0: 636f 6e76 6572 7420 746f 206d 6f64 656c  convert to model
-00001cc0: 0a20 2020 2066 726f 6d20 6e65 6261 7269  .    from nebari
-00001cd0: 2e70 6c75 6769 6e73 2069 6d70 6f72 7420  .plugins import 
-00001ce0: 6e65 6261 7269 5f70 6c75 6769 6e5f 6d61  nebari_plugin_ma
-00001cf0: 6e61 6765 720a 0a20 2020 2074 7279 3a0a  nager..    try:.
-00001d00: 2020 2020 2020 2020 636f 6e66 6967 5f6d          config_m
-00001d10: 6f64 656c 203d 206e 6562 6172 695f 706c  odel = nebari_pl
-00001d20: 7567 696e 5f6d 616e 6167 6572 2e63 6f6e  ugin_manager.con
-00001d30: 6669 675f 7363 6865 6d61 2e70 6172 7365  fig_schema.parse
-00001d40: 5f6f 626a 2863 6f6e 6669 6729 0a20 2020  _obj(config).   
-00001d50: 2065 7863 6570 7420 7079 6461 6e74 6963   except pydantic
-00001d60: 2e56 616c 6964 6174 696f 6e45 7272 6f72  .ValidationError
-00001d70: 2061 7320 653a 0a20 2020 2020 2020 2070   as e:.        p
-00001d80: 7269 6e74 2873 7472 2865 2929 0a0a 2020  rint(str(e))..  
-00001d90: 2020 6966 2072 6570 6f73 6974 6f72 795f    if repository_
-00001da0: 6175 746f 5f70 726f 7669 7369 6f6e 3a0a  auto_provision:.
-00001db0: 2020 2020 2020 2020 6d61 7463 6820 3d20          match = 
-00001dc0: 7265 2e73 6561 7263 6828 6769 7468 7562  re.search(github
-00001dd0: 5f75 726c 5f72 6567 6578 2c20 7265 706f  _url_regex, repo
-00001de0: 7369 746f 7279 290a 2020 2020 2020 2020  sitory).        
-00001df0: 6966 206d 6174 6368 3a0a 2020 2020 2020  if match:.      
-00001e00: 2020 2020 2020 6769 745f 7265 706f 7369        git_reposi
-00001e10: 746f 7279 203d 2067 6974 6875 625f 6175  tory = github_au
-00001e20: 746f 5f70 726f 7669 7369 6f6e 280a 2020  to_provision(.  
-00001e30: 2020 2020 2020 2020 2020 2020 2020 636f                co
-00001e40: 6e66 6967 5f6d 6f64 656c 2c20 6d61 7463  nfig_model, matc
-00001e50: 682e 6772 6f75 7028 3229 2c20 6d61 7463  h.group(2), matc
-00001e60: 682e 6772 6f75 7028 3329 0a20 2020 2020  h.group(3).     
-00001e70: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-00001e80: 2020 2020 2067 6974 5f72 6570 6f73 6974       git_reposit
-00001e90: 6f72 795f 696e 6974 6961 6c69 7a65 2867  ory_initialize(g
-00001ea0: 6974 5f72 6570 6f73 6974 6f72 7929 0a20  it_repository). 
-00001eb0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-00001ec0: 2020 2020 2020 2020 2072 6169 7365 2056           raise V
-00001ed0: 616c 7565 4572 726f 7228 0a20 2020 2020  alueError(.     
-00001ee0: 2020 2020 2020 2020 2020 2066 2252 6570             f"Rep
-00001ef0: 6f73 6974 6f72 7920 746f 2062 6520 6175  ository to be au
-00001f00: 746f 2d70 726f 7669 7369 6f6e 6564 2069  to-provisioned i
-00001f10: 7320 6e6f 7420 7468 6520 6675 6c6c 2055  s not the full U
-00001f20: 524c 206f 6620 6120 4769 7448 7562 2072  RL of a GitHub r
-00001f30: 6570 6f3a 207b 7265 706f 7369 746f 7279  epo: {repository
-00001f40: 7d22 0a20 2020 2020 2020 2020 2020 2029  }".            )
-00001f50: 0a0a 2020 2020 7265 7475 726e 2063 6f6e  ..    return con
-00001f60: 6669 670a 0a0a 6465 6620 6769 7468 7562  fig...def github
-00001f70: 5f61 7574 6f5f 7072 6f76 6973 696f 6e28  _auto_provision(
-00001f80: 636f 6e66 6967 3a20 7079 6461 6e74 6963  config: pydantic
-00001f90: 2e42 6173 654d 6f64 656c 2c20 6f77 6e65  .BaseModel, owne
-00001fa0: 723a 2073 7472 2c20 7265 706f 3a20 7374  r: str, repo: st
-00001fb0: 7229 3a0a 2020 2020 616c 7265 6164 795f  r):.    already_
-00001fc0: 6578 6973 7473 203d 2054 7275 650a 2020  exists = True.  
-00001fd0: 2020 7472 793a 0a20 2020 2020 2020 2067    try:.        g
-00001fe0: 6974 6875 622e 6765 745f 7265 706f 7369  ithub.get_reposi
-00001ff0: 746f 7279 286f 776e 6572 2c20 7265 706f  tory(owner, repo
-00002000: 290a 2020 2020 6578 6365 7074 2072 6571  ).    except req
-00002010: 7565 7374 732e 6578 6365 7074 696f 6e73  uests.exceptions
-00002020: 2e48 5454 5045 7272 6f72 3a0a 2020 2020  .HTTPError:.    
-00002030: 2020 2020 2320 7265 706f 206e 6f74 2066      # repo not f
-00002040: 6f75 6e64 0a20 2020 2020 2020 2061 6c72  ound.        alr
-00002050: 6561 6479 5f65 7869 7374 7320 3d20 4661  eady_exists = Fa
-00002060: 6c73 650a 0a20 2020 2069 6620 6e6f 7420  lse..    if not 
-00002070: 616c 7265 6164 795f 6578 6973 7473 3a0a  already_exists:.
-00002080: 2020 2020 2020 2020 7472 793a 0a20 2020          try:.   
-00002090: 2020 2020 2020 2020 2067 6974 6875 622e           github.
-000020a0: 6372 6561 7465 5f72 6570 6f73 6974 6f72  create_repositor
-000020b0: 7928 0a20 2020 2020 2020 2020 2020 2020  y(.             
-000020c0: 2020 206f 776e 6572 2c0a 2020 2020 2020     owner,.      
-000020d0: 2020 2020 2020 2020 2020 7265 706f 2c0a            repo,.
-000020e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000020f0: 6465 7363 7269 7074 696f 6e3d 6622 4e65  description=f"Ne
-00002100: 6261 7269 207b 636f 6e66 6967 2e70 726f  bari {config.pro
-00002110: 6a65 6374 5f6e 616d 657d 2d7b 636f 6e66  ject_name}-{conf
-00002120: 6967 2e70 726f 7669 6465 727d 222c 0a20  ig.provider}",. 
-00002130: 2020 2020 2020 2020 2020 2020 2020 2068                 h
-00002140: 6f6d 6570 6167 653d 6622 6874 7470 733a  omepage=f"https:
-00002150: 2f2f 7b63 6f6e 6669 672e 646f 6d61 696e  //{config.domain
-00002160: 7d22 2c0a 2020 2020 2020 2020 2020 2020  }",.            
-00002170: 290a 2020 2020 2020 2020 6578 6365 7074  ).        except
-00002180: 2072 6571 7565 7374 732e 6578 6365 7074   requests.except
-00002190: 696f 6e73 2e48 5454 5045 7272 6f72 2061  ions.HTTPError a
-000021a0: 7320 6865 3a0a 2020 2020 2020 2020 2020  s he:.          
-000021b0: 2020 7261 6973 6520 5661 6c75 6545 7272    raise ValueErr
-000021c0: 6f72 280a 2020 2020 2020 2020 2020 2020  or(.            
-000021d0: 2020 2020 6622 556e 6162 6c65 2074 6f20      f"Unable to 
-000021e0: 6372 6561 7465 2047 6974 4875 6220 7265  create GitHub re
-000021f0: 706f 2068 7474 7073 3a2f 2f67 6974 6875  po https://githu
-00002200: 622e 636f 6d2f 7b6f 776e 6572 7d2f 7b72  b.com/{owner}/{r
-00002210: 6570 6f7d 202d 2065 7272 6f72 206d 6573  epo} - error mes
-00002220: 7361 6765 2066 726f 6d20 4769 7448 7562  sage from GitHub
-00002230: 2069 733a 207b 6865 7d22 0a20 2020 2020   is: {he}".     
-00002240: 2020 2020 2020 2029 0a20 2020 2065 6c73         ).    els
-00002250: 653a 0a20 2020 2020 2020 206c 6f67 6765  e:.        logge
-00002260: 722e 7761 726e 696e 6728 6622 4769 7448  r.warning(f"GitH
-00002270: 7562 2072 6570 6f20 6874 7470 733a 2f2f  ub repo https://
-00002280: 6769 7468 7562 2e63 6f6d 2f7b 6f77 6e65  github.com/{owne
-00002290: 727d 2f7b 7265 706f 7d20 616c 7265 6164  r}/{repo} alread
-000022a0: 7920 6578 6973 7473 2229 0a0a 2020 2020  y exists")..    
-000022b0: 7472 793a 0a20 2020 2020 2020 2023 2053  try:.        # S
-000022c0: 6563 7265 7473 0a20 2020 2020 2020 2069  ecrets.        i
-000022d0: 6620 636f 6e66 6967 2e70 726f 7669 6465  f config.provide
-000022e0: 7220 3d3d 2050 726f 7669 6465 7245 6e75  r == ProviderEnu
-000022f0: 6d2e 646f 3a0a 2020 2020 2020 2020 2020  m.do:.          
-00002300: 2020 666f 7220 6e61 6d65 2069 6e20 7b0a    for name in {.
-00002310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002320: 2241 5753 5f41 4343 4553 535f 4b45 595f  "AWS_ACCESS_KEY_
-00002330: 4944 222c 0a20 2020 2020 2020 2020 2020  ID",.           
-00002340: 2020 2020 2022 4157 535f 5345 4352 4554       "AWS_SECRET
-00002350: 5f41 4343 4553 535f 4b45 5922 2c0a 2020  _ACCESS_KEY",.  
-00002360: 2020 2020 2020 2020 2020 2020 2020 2253                "S
-00002370: 5041 4345 535f 4143 4345 5353 5f4b 4559  PACES_ACCESS_KEY
-00002380: 5f49 4422 2c0a 2020 2020 2020 2020 2020  _ID",.          
-00002390: 2020 2020 2020 2253 5041 4345 535f 5345        "SPACES_SE
-000023a0: 4352 4554 5f41 4343 4553 535f 4b45 5922  CRET_ACCESS_KEY"
-000023b0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000023c0: 2020 2244 4947 4954 414c 4f43 4541 4e5f    "DIGITALOCEAN_
-000023d0: 544f 4b45 4e22 2c0a 2020 2020 2020 2020  TOKEN",.        
-000023e0: 2020 2020 7d3a 0a20 2020 2020 2020 2020      }:.         
-000023f0: 2020 2020 2020 2067 6974 6875 622e 7570         github.up
-00002400: 6461 7465 5f73 6563 7265 7428 6f77 6e65  date_secret(owne
-00002410: 722c 2072 6570 6f2c 206e 616d 652c 206f  r, repo, name, o
-00002420: 732e 656e 7669 726f 6e5b 6e61 6d65 5d29  s.environ[name])
-00002430: 0a20 2020 2020 2020 2065 6c69 6620 636f  .        elif co
-00002440: 6e66 6967 2e70 726f 7669 6465 7220 3d3d  nfig.provider ==
-00002450: 2050 726f 7669 6465 7245 6e75 6d2e 6177   ProviderEnum.aw
-00002460: 733a 0a20 2020 2020 2020 2020 2020 2066  s:.            f
-00002470: 6f72 206e 616d 6520 696e 207b 0a20 2020  or name in {.   
-00002480: 2020 2020 2020 2020 2020 2020 2022 4157               "AW
-00002490: 535f 4143 4345 5353 5f4b 4559 5f49 4422  S_ACCESS_KEY_ID"
-000024a0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000024b0: 2020 2241 5753 5f53 4543 5245 545f 4143    "AWS_SECRET_AC
-000024c0: 4345 5353 5f4b 4559 222c 0a20 2020 2020  CESS_KEY",.     
-000024d0: 2020 2020 2020 207d 3a0a 2020 2020 2020         }:.      
-000024e0: 2020 2020 2020 2020 2020 6769 7468 7562            github
-000024f0: 2e75 7064 6174 655f 7365 6372 6574 286f  .update_secret(o
-00002500: 776e 6572 2c20 7265 706f 2c20 6e61 6d65  wner, repo, name
-00002510: 2c20 6f73 2e65 6e76 6972 6f6e 5b6e 616d  , os.environ[nam
-00002520: 655d 290a 2020 2020 2020 2020 656c 6966  e]).        elif
-00002530: 2063 6f6e 6669 672e 7072 6f76 6964 6572   config.provider
-00002540: 203d 3d20 5072 6f76 6964 6572 456e 756d   == ProviderEnum
-00002550: 2e67 6370 3a0a 2020 2020 2020 2020 2020  .gcp:.          
-00002560: 2020 6769 7468 7562 2e75 7064 6174 655f    github.update_
-00002570: 7365 6372 6574 286f 776e 6572 2c20 7265  secret(owner, re
-00002580: 706f 2c20 2250 524f 4a45 4354 5f49 4422  po, "PROJECT_ID"
-00002590: 2c20 6f73 2e65 6e76 6972 6f6e 5b22 5052  , os.environ["PR
-000025a0: 4f4a 4543 545f 4944 225d 290a 2020 2020  OJECT_ID"]).    
-000025b0: 2020 2020 2020 2020 7769 7468 206f 7065          with ope
-000025c0: 6e28 6f73 2e65 6e76 6972 6f6e 5b22 474f  n(os.environ["GO
-000025d0: 4f47 4c45 5f43 5245 4445 4e54 4941 4c53  OGLE_CREDENTIALS
-000025e0: 225d 2920 6173 2066 3a0a 2020 2020 2020  "]) as f:.      
-000025f0: 2020 2020 2020 2020 2020 6769 7468 7562            github
-00002600: 2e75 7064 6174 655f 7365 6372 6574 286f  .update_secret(o
-00002610: 776e 6572 2c20 7265 706f 2c20 2247 4f4f  wner, repo, "GOO
-00002620: 474c 455f 4352 4544 454e 5449 414c 5322  GLE_CREDENTIALS"
-00002630: 2c20 662e 7265 6164 2829 290a 2020 2020  , f.read()).    
-00002640: 2020 2020 656c 6966 2063 6f6e 6669 672e      elif config.
-00002650: 7072 6f76 6964 6572 203d 3d20 5072 6f76  provider == Prov
-00002660: 6964 6572 456e 756d 2e61 7a75 7265 3a0a  iderEnum.azure:.
-00002670: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-00002680: 6e61 6d65 2069 6e20 7b0a 2020 2020 2020  name in {.      
-00002690: 2020 2020 2020 2020 2020 2241 524d 5f43            "ARM_C
-000026a0: 4c49 454e 545f 4944 222c 0a20 2020 2020  LIENT_ID",.     
-000026b0: 2020 2020 2020 2020 2020 2022 4152 4d5f             "ARM_
-000026c0: 434c 4945 4e54 5f53 4543 5245 5422 2c0a  CLIENT_SECRET",.
-000026d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000026e0: 2241 524d 5f53 5542 5343 5249 5054 494f  "ARM_SUBSCRIPTIO
-000026f0: 4e5f 4944 222c 0a20 2020 2020 2020 2020  N_ID",.         
-00002700: 2020 2020 2020 2022 4152 4d5f 5445 4e41         "ARM_TENA
-00002710: 4e54 5f49 4422 2c0a 2020 2020 2020 2020  NT_ID",.        
-00002720: 2020 2020 7d3a 0a20 2020 2020 2020 2020      }:.         
-00002730: 2020 2020 2020 2067 6974 6875 622e 7570         github.up
-00002740: 6461 7465 5f73 6563 7265 7428 6f77 6e65  date_secret(owne
-00002750: 722c 2072 6570 6f2c 206e 616d 652c 206f  r, repo, name, o
-00002760: 732e 656e 7669 726f 6e5b 6e61 6d65 5d29  s.environ[name])
-00002770: 0a20 2020 2020 2020 2067 6974 6875 622e  .        github.
-00002780: 7570 6461 7465 5f73 6563 7265 7428 0a20  update_secret(. 
-00002790: 2020 2020 2020 2020 2020 206f 776e 6572             owner
-000027a0: 2c20 7265 706f 2c20 2252 4550 4f53 4954  , repo, "REPOSIT
-000027b0: 4f52 595f 4143 4345 5353 5f54 4f4b 454e  ORY_ACCESS_TOKEN
-000027c0: 222c 206f 732e 656e 7669 726f 6e5b 2247  ", os.environ["G
-000027d0: 4954 4855 425f 544f 4b45 4e22 5d0a 2020  ITHUB_TOKEN"].  
-000027e0: 2020 2020 2020 290a 2020 2020 6578 6365        ).    exce
-000027f0: 7074 2072 6571 7565 7374 732e 6578 6365  pt requests.exce
-00002800: 7074 696f 6e73 2e48 5454 5045 7272 6f72  ptions.HTTPError
-00002810: 2061 7320 6865 3a0a 2020 2020 2020 2020   as he:.        
-00002820: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
-00002830: 280a 2020 2020 2020 2020 2020 2020 6622  (.            f"
-00002840: 556e 6162 6c65 2074 6f20 7365 7420 5365  Unable to set Se
-00002850: 6372 6574 7320 6f6e 2047 6974 4875 6220  crets on GitHub 
-00002860: 7265 706f 2068 7474 7073 3a2f 2f67 6974  repo https://git
-00002870: 6875 622e 636f 6d2f 7b6f 776e 6572 7d2f  hub.com/{owner}/
-00002880: 7b72 6570 6f7d 202d 2065 7272 6f72 206d  {repo} - error m
-00002890: 6573 7361 6765 2066 726f 6d20 4769 7448  essage from GitH
-000028a0: 7562 2069 733a 207b 6865 7d22 0a20 2020  ub is: {he}".   
-000028b0: 2020 2020 2029 0a0a 2020 2020 7265 7475       )..    retu
-000028c0: 726e 2066 2267 6974 4067 6974 6875 622e  rn f"git@github.
-000028d0: 636f 6d3a 7b6f 776e 6572 7d2f 7b72 6570  com:{owner}/{rep
-000028e0: 6f7d 2e67 6974 220a 0a0a 6465 6620 6769  o}.git"...def gi
-000028f0: 745f 7265 706f 7369 746f 7279 5f69 6e69  t_repository_ini
-00002900: 7469 616c 697a 6528 6769 745f 7265 706f  tialize(git_repo
-00002910: 7369 746f 7279 293a 0a20 2020 2069 6620  sitory):.    if 
-00002920: 6e6f 7420 6769 742e 6973 5f67 6974 5f72  not git.is_git_r
-00002930: 6570 6f28 5061 7468 2e63 7764 2829 293a  epo(Path.cwd()):
-00002940: 0a20 2020 2020 2020 2067 6974 2e69 6e69  .        git.ini
-00002950: 7469 616c 697a 655f 6769 7428 5061 7468  tialize_git(Path
-00002960: 2e63 7764 2829 290a 2020 2020 6769 742e  .cwd()).    git.
-00002970: 6164 645f 6769 745f 7265 6d6f 7465 2867  add_git_remote(g
-00002980: 6974 5f72 6570 6f73 6974 6f72 792c 2070  it_repository, p
-00002990: 6174 683d 5061 7468 2e63 7764 2829 2c20  ath=Path.cwd(), 
-000029a0: 7265 6d6f 7465 5f6e 616d 653d 226f 7269  remote_name="ori
-000029b0: 6769 6e22 290a                           gin").
+000001c0: 6573 2e69 6e66 7261 7374 7275 6374 7572  es.infrastructur
+000001d0: 6520 696d 706f 7274 2028 0a20 2020 2044  e import (.    D
+000001e0: 4546 4155 4c54 5f41 5753 5f4e 4f44 455f  EFAULT_AWS_NODE_
+000001f0: 4752 4f55 5053 2c0a 2020 2020 4445 4641  GROUPS,.    DEFA
+00000200: 554c 545f 415a 5552 455f 4e4f 4445 5f47  ULT_AZURE_NODE_G
+00000210: 524f 5550 532c 0a20 2020 2044 4546 4155  ROUPS,.    DEFAU
+00000220: 4c54 5f44 4f5f 4e4f 4445 5f47 524f 5550  LT_DO_NODE_GROUP
+00000230: 532c 0a20 2020 2044 4546 4155 4c54 5f47  S,.    DEFAULT_G
+00000240: 4350 5f4e 4f44 455f 4752 4f55 5053 2c0a  CP_NODE_GROUPS,.
+00000250: 290a 6672 6f6d 205f 6e65 6261 7269 2e73  ).from _nebari.s
+00000260: 7461 6765 732e 6b75 6265 726e 6574 6573  tages.kubernetes
+00000270: 5f69 6e67 7265 7373 2069 6d70 6f72 7420  _ingress import 
+00000280: 4365 7274 6966 6963 6174 6545 6e75 6d0a  CertificateEnum.
+00000290: 6672 6f6d 205f 6e65 6261 7269 2e73 7461  from _nebari.sta
+000002a0: 6765 732e 6b75 6265 726e 6574 6573 5f6b  ges.kubernetes_k
+000002b0: 6579 636c 6f61 6b20 696d 706f 7274 2041  eycloak import A
+000002c0: 7574 6865 6e74 6963 6174 696f 6e45 6e75  uthenticationEnu
+000002d0: 6d0a 6672 6f6d 205f 6e65 6261 7269 2e73  m.from _nebari.s
+000002e0: 7461 6765 732e 7465 7272 6166 6f72 6d5f  tages.terraform_
+000002f0: 7374 6174 6520 696d 706f 7274 2054 6572  state import Ter
+00000300: 7261 666f 726d 5374 6174 6545 6e75 6d0a  raformStateEnum.
+00000310: 6672 6f6d 205f 6e65 6261 7269 2e75 7469  from _nebari.uti
+00000320: 6c73 2069 6d70 6f72 7420 6765 745f 6c61  ls import get_la
+00000330: 7465 7374 5f6b 7562 6572 6e65 7465 735f  test_kubernetes_
+00000340: 7665 7273 696f 6e2c 2072 616e 646f 6d5f  version, random_
+00000350: 7365 6375 7265 5f73 7472 696e 670a 6672  secure_string.fr
+00000360: 6f6d 205f 6e65 6261 7269 2e76 6572 7369  om _nebari.versi
+00000370: 6f6e 2069 6d70 6f72 7420 5f5f 7665 7273  on import __vers
+00000380: 696f 6e5f 5f0a 6672 6f6d 206e 6562 6172  ion__.from nebar
+00000390: 692e 7363 6865 6d61 2069 6d70 6f72 7420  i.schema import 
+000003a0: 5072 6f76 6964 6572 456e 756d 2c20 6769  ProviderEnum, gi
+000003b0: 7468 7562 5f75 726c 5f72 6567 6578 0a0a  thub_url_regex..
+000003c0: 6c6f 6767 6572 203d 206c 6f67 6769 6e67  logger = logging
+000003d0: 2e67 6574 4c6f 6767 6572 285f 5f6e 616d  .getLogger(__nam
+000003e0: 655f 5f29 0a0a 5745 4c43 4f4d 455f 4845  e__)..WELCOME_HE
+000003f0: 4144 4552 5f54 4558 5420 3d20 2259 6f75  ADER_TEXT = "You
+00000400: 7220 6f70 656e 2073 6f75 7263 6520 6461  r open source da
+00000410: 7461 2073 6369 656e 6365 2070 6c61 7466  ta science platf
+00000420: 6f72 6d2c 2068 6f73 7465 6422 0a0a 0a64  orm, hosted"...d
+00000430: 6566 205f 6e6f 6465 5f67 726f 7570 735f  ef _node_groups_
+00000440: 746f 5f64 6963 7428 6e6f 6465 5f67 726f  to_dict(node_gro
+00000450: 7570 7329 3a0a 2020 2020 7265 7475 726e  ups):.    return
+00000460: 207b 6e67 5f6e 616d 653a 206e 672e 6469   {ng_name: ng.di
+00000470: 6374 2829 2066 6f72 206e 675f 6e61 6d65  ct() for ng_name
+00000480: 2c20 6e67 2069 6e20 6e6f 6465 5f67 726f  , ng in node_gro
+00000490: 7570 732e 6974 656d 7328 297d 0a0a 0a64  ups.items()}...d
+000004a0: 6566 2072 656e 6465 725f 636f 6e66 6967  ef render_config
+000004b0: 280a 2020 2020 7072 6f6a 6563 745f 6e61  (.    project_na
+000004c0: 6d65 3a20 7374 722c 0a20 2020 206e 6562  me: str,.    neb
+000004d0: 6172 695f 646f 6d61 696e 3a20 7374 7220  ari_domain: str 
+000004e0: 3d20 4e6f 6e65 2c0a 2020 2020 636c 6f75  = None,.    clou
+000004f0: 645f 7072 6f76 6964 6572 3a20 5072 6f76  d_provider: Prov
+00000500: 6964 6572 456e 756d 203d 2050 726f 7669  iderEnum = Provi
+00000510: 6465 7245 6e75 6d2e 6c6f 6361 6c2c 0a20  derEnum.local,. 
+00000520: 2020 2063 695f 7072 6f76 6964 6572 3a20     ci_provider: 
+00000530: 4369 456e 756d 203d 2043 6945 6e75 6d2e  CiEnum = CiEnum.
+00000540: 6e6f 6e65 2c0a 2020 2020 7265 706f 7369  none,.    reposi
+00000550: 746f 7279 3a20 7374 7220 3d20 4e6f 6e65  tory: str = None
+00000560: 2c0a 2020 2020 6175 7468 5f70 726f 7669  ,.    auth_provi
+00000570: 6465 723a 2041 7574 6865 6e74 6963 6174  der: Authenticat
+00000580: 696f 6e45 6e75 6d20 3d20 4175 7468 656e  ionEnum = Authen
+00000590: 7469 6361 7469 6f6e 456e 756d 2e70 6173  ticationEnum.pas
+000005a0: 7377 6f72 642c 0a20 2020 206e 616d 6573  sword,.    names
+000005b0: 7061 6365 3a20 7374 7220 3d20 2264 6576  pace: str = "dev
+000005c0: 222c 0a20 2020 2072 6570 6f73 6974 6f72  ",.    repositor
+000005d0: 795f 6175 746f 5f70 726f 7669 7369 6f6e  y_auto_provision
+000005e0: 3a20 626f 6f6c 203d 2046 616c 7365 2c0a  : bool = False,.
+000005f0: 2020 2020 6175 7468 5f61 7574 6f5f 7072      auth_auto_pr
+00000600: 6f76 6973 696f 6e3a 2062 6f6f 6c20 3d20  ovision: bool = 
+00000610: 4661 6c73 652c 0a20 2020 2074 6572 7261  False,.    terra
+00000620: 666f 726d 5f73 7461 7465 3a20 5465 7272  form_state: Terr
+00000630: 6166 6f72 6d53 7461 7465 456e 756d 203d  aformStateEnum =
+00000640: 2054 6572 7261 666f 726d 5374 6174 6545   TerraformStateE
+00000650: 6e75 6d2e 7265 6d6f 7465 2c0a 2020 2020  num.remote,.    
+00000660: 6b75 6265 726e 6574 6573 5f76 6572 7369  kubernetes_versi
+00000670: 6f6e 3a20 7374 7220 3d20 4e6f 6e65 2c0a  on: str = None,.
+00000680: 2020 2020 7265 6769 6f6e 3a20 7374 7220      region: str 
+00000690: 3d20 4e6f 6e65 2c0a 2020 2020 6469 7361  = None,.    disa
+000006a0: 626c 655f 7072 6f6d 7074 3a20 626f 6f6c  ble_prompt: bool
+000006b0: 203d 2046 616c 7365 2c0a 2020 2020 7373   = False,.    ss
+000006c0: 6c5f 6365 7274 5f65 6d61 696c 3a20 7374  l_cert_email: st
+000006d0: 7220 3d20 4e6f 6e65 2c0a 293a 0a20 2020  r = None,.):.   
+000006e0: 2063 6f6e 6669 6720 3d20 7b0a 2020 2020   config = {.    
+000006f0: 2020 2020 2270 726f 7669 6465 7222 3a20      "provider": 
+00000700: 636c 6f75 645f 7072 6f76 6964 6572 2c0a  cloud_provider,.
+00000710: 2020 2020 2020 2020 226e 616d 6573 7061          "namespa
+00000720: 6365 223a 206e 616d 6573 7061 6365 2c0a  ce": namespace,.
+00000730: 2020 2020 2020 2020 226e 6562 6172 695f          "nebari_
+00000740: 7665 7273 696f 6e22 3a20 5f5f 7665 7273  version": __vers
+00000750: 696f 6e5f 5f2c 0a20 2020 207d 0a0a 2020  ion__,.    }..  
+00000760: 2020 6966 2070 726f 6a65 6374 5f6e 616d    if project_nam
+00000770: 6520 6973 204e 6f6e 6520 616e 6420 6e6f  e is None and no
+00000780: 7420 6469 7361 626c 655f 7072 6f6d 7074  t disable_prompt
+00000790: 3a0a 2020 2020 2020 2020 7072 6f6a 6563  :.        projec
+000007a0: 745f 6e61 6d65 203d 2069 6e70 7574 2822  t_name = input("
+000007b0: 5072 6f76 6964 6520 7072 6f6a 6563 7420  Provide project 
+000007c0: 6e61 6d65 3a20 2229 0a20 2020 2063 6f6e  name: ").    con
+000007d0: 6669 675b 2270 726f 6a65 6374 5f6e 616d  fig["project_nam
+000007e0: 6522 5d20 3d20 7072 6f6a 6563 745f 6e61  e"] = project_na
+000007f0: 6d65 0a0a 2020 2020 6966 206e 6562 6172  me..    if nebar
+00000800: 695f 646f 6d61 696e 2069 7320 6e6f 7420  i_domain is not 
+00000810: 4e6f 6e65 3a0a 2020 2020 2020 2020 636f  None:.        co
+00000820: 6e66 6967 5b22 646f 6d61 696e 225d 203d  nfig["domain"] =
+00000830: 206e 6562 6172 695f 646f 6d61 696e 0a0a   nebari_domain..
+00000840: 2020 2020 636f 6e66 6967 5b22 6369 5f63      config["ci_c
+00000850: 6422 5d20 3d20 7b22 7479 7065 223a 2063  d"] = {"type": c
+00000860: 695f 7072 6f76 6964 6572 7d0a 2020 2020  i_provider}.    
+00000870: 636f 6e66 6967 5b22 7465 7272 6166 6f72  config["terrafor
+00000880: 6d5f 7374 6174 6522 5d20 3d20 7b22 7479  m_state"] = {"ty
+00000890: 7065 223a 2074 6572 7261 666f 726d 5f73  pe": terraform_s
+000008a0: 7461 7465 7d0a 0a20 2020 2023 2053 6176  tate}..    # Sav
+000008b0: 6520 6465 6661 756c 7420 7061 7373 776f  e default passwo
+000008c0: 7264 2074 6f20 6669 6c65 0a20 2020 2064  rd to file.    d
+000008d0: 6566 6175 6c74 5f70 6173 7377 6f72 645f  efault_password_
+000008e0: 6669 6c65 6e61 6d65 203d 2050 6174 6828  filename = Path(
+000008f0: 7465 6d70 6669 6c65 2e67 6574 7465 6d70  tempfile.gettemp
+00000900: 6469 7228 2929 202f 2022 4e45 4241 5249  dir()) / "NEBARI
+00000910: 5f44 4546 4155 4c54 5f50 4153 5357 4f52  _DEFAULT_PASSWOR
+00000920: 4422 0a20 2020 2063 6f6e 6669 675b 2273  D".    config["s
+00000930: 6563 7572 6974 7922 5d20 3d20 7b0a 2020  ecurity"] = {.  
+00000940: 2020 2020 2020 226b 6579 636c 6f61 6b22        "keycloak"
+00000950: 3a20 7b22 696e 6974 6961 6c5f 726f 6f74  : {"initial_root
+00000960: 5f70 6173 7377 6f72 6422 3a20 7261 6e64  _password": rand
+00000970: 6f6d 5f73 6563 7572 655f 7374 7269 6e67  om_secure_string
+00000980: 286c 656e 6774 683d 3332 297d 0a20 2020  (length=32)}.   
+00000990: 207d 0a20 2020 2077 6974 6820 6465 6661   }.    with defa
+000009a0: 756c 745f 7061 7373 776f 7264 5f66 696c  ult_password_fil
+000009b0: 656e 616d 652e 6f70 656e 2822 7722 2920  ename.open("w") 
+000009c0: 6173 2066 3a0a 2020 2020 2020 2020 662e  as f:.        f.
+000009d0: 7772 6974 6528 636f 6e66 6967 5b22 7365  write(config["se
+000009e0: 6375 7269 7479 225d 5b22 6b65 7963 6c6f  curity"]["keyclo
+000009f0: 616b 225d 5b22 696e 6974 6961 6c5f 726f  ak"]["initial_ro
+00000a00: 6f74 5f70 6173 7377 6f72 6422 5d29 0a20  ot_password"]). 
+00000a10: 2020 2064 6566 6175 6c74 5f70 6173 7377     default_passw
+00000a20: 6f72 645f 6669 6c65 6e61 6d65 2e63 686d  ord_filename.chm
+00000a30: 6f64 2830 6f37 3030 290a 0a20 2020 2063  od(0o700)..    c
+00000a40: 6f6e 6669 675b 2274 6865 6d65 225d 203d  onfig["theme"] =
+00000a50: 207b 226a 7570 7974 6572 6875 6222 3a20   {"jupyterhub": 
+00000a60: 7b22 6875 625f 7469 746c 6522 3a20 6622  {"hub_title": f"
+00000a70: 4e65 6261 7269 202d 207b 2070 726f 6a65  Nebari - { proje
+00000a80: 6374 5f6e 616d 6520 7d22 7d7d 0a20 2020  ct_name }"}}.   
+00000a90: 2063 6f6e 6669 675b 2274 6865 6d65 225d   config["theme"]
+00000aa0: 5b22 6a75 7079 7465 7268 7562 225d 5b0a  ["jupyterhub"][.
+00000ab0: 2020 2020 2020 2020 2277 656c 636f 6d65          "welcome
+00000ac0: 220a 2020 2020 5d20 3d20 2222 2257 656c  ".    ] = """Wel
+00000ad0: 636f 6d65 2120 4c65 6172 6e20 6162 6f75  come! Learn abou
+00000ae0: 7420 4e65 6261 7269 2773 2066 6561 7475  t Nebari's featu
+00000af0: 7265 7320 616e 6420 636f 6e66 6967 7572  res and configur
+00000b00: 6174 696f 6e73 2069 6e20 3c61 2068 7265  ations in <a hre
+00000b10: 663d 2268 7474 7073 3a2f 2f77 7777 2e6e  f="https://www.n
+00000b20: 6562 6172 692e 6465 762f 646f 6373 2f77  ebari.dev/docs/w
+00000b30: 656c 636f 6d65 223e 7468 6520 646f 6375  elcome">the docu
+00000b40: 6d65 6e74 6174 696f 6e3c 2f61 3e2e 2049  mentation</a>. I
+00000b50: 6620 796f 7520 6861 7665 2061 6e79 2071  f you have any q
+00000b60: 7565 7374 696f 6e73 206f 7220 6665 6564  uestions or feed
+00000b70: 6261 636b 2c20 7265 6163 6820 7468 6520  back, reach the 
+00000b80: 7465 616d 206f 6e20 3c61 2068 7265 663d  team on <a href=
+00000b90: 2268 7474 7073 3a2f 2f77 7777 2e6e 6562  "https://www.neb
+00000ba0: 6172 692e 6465 762f 646f 6373 2f63 6f6d  ari.dev/docs/com
+00000bb0: 6d75 6e69 7479 2367 6574 7469 6e67 2d73  munity#getting-s
+00000bc0: 7570 706f 7274 223e 4e65 6261 7269 2773  upport">Nebari's
+00000bd0: 2073 7570 706f 7274 2066 6f72 756d 733c   support forums<
+00000be0: 2f61 3e2e 2222 220a 0a20 2020 2063 6f6e  /a>."""..    con
+00000bf0: 6669 675b 2273 6563 7572 6974 7922 5d5b  fig["security"][
+00000c00: 2261 7574 6865 6e74 6963 6174 696f 6e22  "authentication"
+00000c10: 5d20 3d20 7b22 7479 7065 223a 2061 7574  ] = {"type": aut
+00000c20: 685f 7072 6f76 6964 6572 7d0a 0a20 2020  h_provider}..   
+00000c30: 2069 6620 6175 7468 5f70 726f 7669 6465   if auth_provide
+00000c40: 7220 3d3d 2041 7574 6865 6e74 6963 6174  r == Authenticat
+00000c50: 696f 6e45 6e75 6d2e 6769 7468 7562 3a0a  ionEnum.github:.
+00000c60: 2020 2020 2020 2020 636f 6e66 6967 5b22          config["
+00000c70: 7365 6375 7269 7479 225d 5b22 6175 7468  security"]["auth
+00000c80: 656e 7469 6361 7469 6f6e 225d 5b22 636f  entication"]["co
+00000c90: 6e66 6967 225d 203d 207b 0a20 2020 2020  nfig"] = {.     
+00000ca0: 2020 2020 2020 2022 636c 6965 6e74 5f69         "client_i
+00000cb0: 6422 3a20 6f73 2e65 6e76 6972 6f6e 2e67  d": os.environ.g
+00000cc0: 6574 280a 2020 2020 2020 2020 2020 2020  et(.            
+00000cd0: 2020 2020 2247 4954 4855 425f 434c 4945      "GITHUB_CLIE
+00000ce0: 4e54 5f49 4422 2c0a 2020 2020 2020 2020  NT_ID",.        
+00000cf0: 2020 2020 2020 2020 223c 656e 7465 7220          "<enter 
+00000d00: 636c 6965 6e74 2069 6420 6f72 2072 656d  client id or rem
+00000d10: 6f76 6520 746f 2075 7365 2047 4954 4855  ove to use GITHU
+00000d20: 425f 434c 4945 4e54 5f49 4420 656e 7669  B_CLIENT_ID envi
+00000d30: 726f 6e6d 656e 7420 7661 7269 6162 6c65  ronment variable
+00000d40: 2028 7072 6566 6572 7265 6429 3e22 2c0a   (preferred)>",.
+00000d50: 2020 2020 2020 2020 2020 2020 292c 0a20              ),. 
+00000d60: 2020 2020 2020 2020 2020 2022 636c 6965             "clie
+00000d70: 6e74 5f73 6563 7265 7422 3a20 6f73 2e65  nt_secret": os.e
+00000d80: 6e76 6972 6f6e 2e67 6574 280a 2020 2020  nviron.get(.    
+00000d90: 2020 2020 2020 2020 2020 2020 2247 4954              "GIT
+00000da0: 4855 425f 434c 4945 4e54 5f53 4543 5245  HUB_CLIENT_SECRE
+00000db0: 5422 2c0a 2020 2020 2020 2020 2020 2020  T",.            
+00000dc0: 2020 2020 223c 656e 7465 7220 636c 6965      "<enter clie
+00000dd0: 6e74 2073 6563 7265 7420 6f72 2072 656d  nt secret or rem
+00000de0: 6f76 6520 746f 2075 7365 2047 4954 4855  ove to use GITHU
+00000df0: 425f 434c 4945 4e54 5f53 4543 5245 5420  B_CLIENT_SECRET 
+00000e00: 656e 7669 726f 6e6d 656e 7420 7661 7269  environment vari
+00000e10: 6162 6c65 2028 7072 6566 6572 7265 6429  able (preferred)
+00000e20: 3e22 2c0a 2020 2020 2020 2020 2020 2020  >",.            
+00000e30: 292c 0a20 2020 2020 2020 207d 0a20 2020  ),.        }.   
+00000e40: 2065 6c69 6620 6175 7468 5f70 726f 7669   elif auth_provi
+00000e50: 6465 7220 3d3d 2041 7574 6865 6e74 6963  der == Authentic
+00000e60: 6174 696f 6e45 6e75 6d2e 6175 7468 303a  ationEnum.auth0:
+00000e70: 0a20 2020 2020 2020 2069 6620 6175 7468  .        if auth
+00000e80: 5f61 7574 6f5f 7072 6f76 6973 696f 6e3a  _auto_provision:
+00000e90: 0a20 2020 2020 2020 2020 2020 2061 7574  .            aut
+00000ea0: 6830 5f63 6f6e 6669 6720 3d20 6372 6561  h0_config = crea
+00000eb0: 7465 5f63 6c69 656e 7428 636f 6e66 6967  te_client(config
+00000ec0: 2e64 6f6d 6169 6e2c 2063 6f6e 6669 672e  .domain, config.
+00000ed0: 7072 6f6a 6563 745f 6e61 6d65 290a 2020  project_name).  
+00000ee0: 2020 2020 2020 2020 2020 636f 6e66 6967            config
+00000ef0: 5b22 7365 6375 7269 7479 225d 5b22 6175  ["security"]["au
+00000f00: 7468 656e 7469 6361 7469 6f6e 225d 5b22  thentication"]["
+00000f10: 636f 6e66 6967 225d 203d 2061 7574 6830  config"] = auth0
+00000f20: 5f63 6f6e 6669 670a 2020 2020 2020 2020  _config.        
+00000f30: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+00000f40: 2020 636f 6e66 6967 5b22 7365 6375 7269    config["securi
+00000f50: 7479 225d 5b22 6175 7468 656e 7469 6361  ty"]["authentica
+00000f60: 7469 6f6e 225d 5b22 636f 6e66 6967 225d  tion"]["config"]
+00000f70: 203d 207b 0a20 2020 2020 2020 2020 2020   = {.           
+00000f80: 2020 2020 2022 636c 6965 6e74 5f69 6422       "client_id"
+00000f90: 3a20 6f73 2e65 6e76 6972 6f6e 2e67 6574  : os.environ.get
+00000fa0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00000fb0: 2020 2020 2020 2241 5554 4830 5f43 4c49        "AUTH0_CLI
+00000fc0: 454e 545f 4944 222c 0a20 2020 2020 2020  ENT_ID",.       
+00000fd0: 2020 2020 2020 2020 2020 2020 2022 3c65               "<e
+00000fe0: 6e74 6572 2063 6c69 656e 7420 6964 206f  nter client id o
+00000ff0: 7220 7265 6d6f 7665 2074 6f20 7573 6520  r remove to use 
+00001000: 4155 5448 305f 434c 4945 4e54 5f49 4420  AUTH0_CLIENT_ID 
+00001010: 656e 7669 726f 6e6d 656e 7420 7661 7269  environment vari
+00001020: 6162 6c65 2028 7072 6566 6572 7265 6429  able (preferred)
+00001030: 3e22 2c0a 2020 2020 2020 2020 2020 2020  >",.            
+00001040: 2020 2020 292c 0a20 2020 2020 2020 2020      ),.         
+00001050: 2020 2020 2020 2022 636c 6965 6e74 5f73         "client_s
+00001060: 6563 7265 7422 3a20 6f73 2e65 6e76 6972  ecret": os.envir
+00001070: 6f6e 2e67 6574 280a 2020 2020 2020 2020  on.get(.        
+00001080: 2020 2020 2020 2020 2020 2020 2241 5554              "AUT
+00001090: 4830 5f43 4c49 454e 545f 5345 4352 4554  H0_CLIENT_SECRET
+000010a0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+000010b0: 2020 2020 2020 2022 3c65 6e74 6572 2063         "<enter c
+000010c0: 6c69 656e 7420 7365 6372 6574 206f 7220  lient secret or 
+000010d0: 7265 6d6f 7665 2074 6f20 7573 6520 4155  remove to use AU
+000010e0: 5448 305f 434c 4945 4e54 5f53 4543 5245  TH0_CLIENT_SECRE
+000010f0: 5420 656e 7669 726f 6e6d 656e 7420 7661  T environment va
+00001100: 7269 6162 6c65 2028 7072 6566 6572 7265  riable (preferre
+00001110: 6429 3e22 2c0a 2020 2020 2020 2020 2020  d)>",.          
+00001120: 2020 2020 2020 292c 0a20 2020 2020 2020        ),.       
+00001130: 2020 2020 2020 2020 2022 6175 7468 305f           "auth0_
+00001140: 7375 6264 6f6d 6169 6e22 3a20 6f73 2e65  subdomain": os.e
+00001150: 6e76 6972 6f6e 2e67 6574 280a 2020 2020  nviron.get(.    
+00001160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001170: 2241 5554 4830 5f44 4f4d 4149 4e22 2c0a  "AUTH0_DOMAIN",.
+00001180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001190: 2020 2020 223c 656e 7465 7220 7375 6264      "<enter subd
+000011a0: 6f6d 6169 6e20 2877 6974 686f 7574 202e  omain (without .
+000011b0: 6175 7468 302e 636f 6d29 206f 7220 7265  auth0.com) or re
+000011c0: 6d6f 7665 2074 6f20 7573 6520 4155 5448  move to use AUTH
+000011d0: 305f 444f 4d41 494e 2065 6e76 6972 6f6e  0_DOMAIN environ
+000011e0: 6d65 6e74 2076 6172 6961 626c 653e 222c  ment variable>",
+000011f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001200: 2029 2c0a 2020 2020 2020 2020 2020 2020   ),.            
+00001210: 7d0a 0a20 2020 2069 6620 636c 6f75 645f  }..    if cloud_
+00001220: 7072 6f76 6964 6572 203d 3d20 5072 6f76  provider == Prov
+00001230: 6964 6572 456e 756d 2e64 6f3a 0a20 2020  iderEnum.do:.   
+00001240: 2020 2020 2064 6f5f 7265 6769 6f6e 203d       do_region =
+00001250: 2072 6567 696f 6e20 6f72 2063 6f6e 7374   region or const
+00001260: 616e 7473 2e44 4f5f 4445 4641 554c 545f  ants.DO_DEFAULT_
+00001270: 5245 4749 4f4e 0a20 2020 2020 2020 2064  REGION.        d
+00001280: 6f5f 6b75 6265 726e 6574 6573 5f76 6572  o_kubernetes_ver
+00001290: 7369 6f6e 7320 3d20 6b75 6265 726e 6574  sions = kubernet
+000012a0: 6573 5f76 6572 7369 6f6e 206f 7220 6765  es_version or ge
+000012b0: 745f 6c61 7465 7374 5f6b 7562 6572 6e65  t_latest_kuberne
+000012c0: 7465 735f 7665 7273 696f 6e28 0a20 2020  tes_version(.   
+000012d0: 2020 2020 2020 2020 2064 6967 6974 616c           digital
+000012e0: 5f6f 6365 616e 2e6b 7562 6572 6e65 7465  _ocean.kubernete
+000012f0: 735f 7665 7273 696f 6e73 2864 6f5f 7265  s_versions(do_re
+00001300: 6769 6f6e 290a 2020 2020 2020 2020 290a  gion).        ).
+00001310: 2020 2020 2020 2020 636f 6e66 6967 5b22          config["
+00001320: 6469 6769 7461 6c5f 6f63 6561 6e22 5d20  digital_ocean"] 
+00001330: 3d20 7b0a 2020 2020 2020 2020 2020 2020  = {.            
+00001340: 226b 7562 6572 6e65 7465 735f 7665 7273  "kubernetes_vers
+00001350: 696f 6e22 3a20 646f 5f6b 7562 6572 6e65  ion": do_kuberne
+00001360: 7465 735f 7665 7273 696f 6e73 2c0a 2020  tes_versions,.  
+00001370: 2020 2020 2020 2020 2020 2272 6567 696f            "regio
+00001380: 6e22 3a20 646f 5f72 6567 696f 6e2c 0a20  n": do_region,. 
+00001390: 2020 2020 2020 2020 2020 2022 6e6f 6465             "node
+000013a0: 5f67 726f 7570 7322 3a20 5f6e 6f64 655f  _groups": _node_
+000013b0: 6772 6f75 7073 5f74 6f5f 6469 6374 2844  groups_to_dict(D
+000013c0: 4546 4155 4c54 5f44 4f5f 4e4f 4445 5f47  EFAULT_DO_NODE_G
+000013d0: 524f 5550 5329 2c0a 2020 2020 2020 2020  ROUPS),.        
+000013e0: 7d0a 0a20 2020 2020 2020 2063 6f6e 6669  }..        confi
+000013f0: 675b 2274 6865 6d65 225d 5b22 6a75 7079  g["theme"]["jupy
+00001400: 7465 7268 7562 225d 5b0a 2020 2020 2020  terhub"][.      
+00001410: 2020 2020 2020 2268 7562 5f73 7562 7469        "hub_subti
+00001420: 746c 6522 0a20 2020 2020 2020 205d 203d  tle".        ] =
+00001430: 2066 227b 5745 4c43 4f4d 455f 4845 4144   f"{WELCOME_HEAD
+00001440: 4552 5f54 4558 547d 206f 6e20 4469 6769  ER_TEXT} on Digi
+00001450: 7461 6c20 4f63 6561 6e22 0a0a 2020 2020  tal Ocean"..    
+00001460: 656c 6966 2063 6c6f 7564 5f70 726f 7669  elif cloud_provi
+00001470: 6465 7220 3d3d 2050 726f 7669 6465 7245  der == ProviderE
+00001480: 6e75 6d2e 6763 703a 0a20 2020 2020 2020  num.gcp:.       
+00001490: 2067 6370 5f72 6567 696f 6e20 3d20 7265   gcp_region = re
+000014a0: 6769 6f6e 206f 7220 636f 6e73 7461 6e74  gion or constant
+000014b0: 732e 4743 505f 4445 4641 554c 545f 5245  s.GCP_DEFAULT_RE
+000014c0: 4749 4f4e 0a20 2020 2020 2020 2067 6370  GION.        gcp
+000014d0: 5f6b 7562 6572 6e65 7465 735f 7665 7273  _kubernetes_vers
+000014e0: 696f 6e20 3d20 6b75 6265 726e 6574 6573  ion = kubernetes
+000014f0: 5f76 6572 7369 6f6e 206f 7220 6765 745f  _version or get_
+00001500: 6c61 7465 7374 5f6b 7562 6572 6e65 7465  latest_kubernete
+00001510: 735f 7665 7273 696f 6e28 0a20 2020 2020  s_version(.     
+00001520: 2020 2020 2020 2067 6f6f 676c 655f 636c         google_cl
+00001530: 6f75 642e 6b75 6265 726e 6574 6573 5f76  oud.kubernetes_v
+00001540: 6572 7369 6f6e 7328 6763 705f 7265 6769  ersions(gcp_regi
+00001550: 6f6e 290a 2020 2020 2020 2020 290a 2020  on).        ).  
+00001560: 2020 2020 2020 636f 6e66 6967 5b22 676f        config["go
+00001570: 6f67 6c65 5f63 6c6f 7564 5f70 6c61 7466  ogle_cloud_platf
+00001580: 6f72 6d22 5d20 3d20 7b0a 2020 2020 2020  orm"] = {.      
+00001590: 2020 2020 2020 226b 7562 6572 6e65 7465        "kubernete
+000015a0: 735f 7665 7273 696f 6e22 3a20 6763 705f  s_version": gcp_
+000015b0: 6b75 6265 726e 6574 6573 5f76 6572 7369  kubernetes_versi
+000015c0: 6f6e 2c0a 2020 2020 2020 2020 2020 2020  on,.            
+000015d0: 2272 6567 696f 6e22 3a20 6763 705f 7265  "region": gcp_re
+000015e0: 6769 6f6e 2c0a 2020 2020 2020 2020 2020  gion,.          
+000015f0: 2020 226e 6f64 655f 6772 6f75 7073 223a    "node_groups":
+00001600: 205f 6e6f 6465 5f67 726f 7570 735f 746f   _node_groups_to
+00001610: 5f64 6963 7428 4445 4641 554c 545f 4743  _dict(DEFAULT_GC
+00001620: 505f 4e4f 4445 5f47 524f 5550 5329 2c0a  P_NODE_GROUPS),.
+00001630: 2020 2020 2020 2020 7d0a 0a20 2020 2020          }..     
+00001640: 2020 2063 6f6e 6669 675b 2274 6865 6d65     config["theme
+00001650: 225d 5b22 6a75 7079 7465 7268 7562 225d  "]["jupyterhub"]
+00001660: 5b0a 2020 2020 2020 2020 2020 2020 2268  [.            "h
+00001670: 7562 5f73 7562 7469 746c 6522 0a20 2020  ub_subtitle".   
+00001680: 2020 2020 205d 203d 2066 227b 5745 4c43       ] = f"{WELC
+00001690: 4f4d 455f 4845 4144 4552 5f54 4558 547d  OME_HEADER_TEXT}
+000016a0: 206f 6e20 476f 6f67 6c65 2043 6c6f 7564   on Google Cloud
+000016b0: 2050 6c61 7466 6f72 6d22 0a20 2020 2020   Platform".     
+000016c0: 2020 2069 6620 2250 524f 4a45 4354 5f49     if "PROJECT_I
+000016d0: 4422 2069 6e20 6f73 2e65 6e76 6972 6f6e  D" in os.environ
+000016e0: 3a0a 2020 2020 2020 2020 2020 2020 636f  :.            co
+000016f0: 6e66 6967 5b22 676f 6f67 6c65 5f63 6c6f  nfig["google_clo
+00001700: 7564 5f70 6c61 7466 6f72 6d22 5d5b 2270  ud_platform"]["p
+00001710: 726f 6a65 6374 225d 203d 206f 732e 656e  roject"] = os.en
+00001720: 7669 726f 6e5b 2250 524f 4a45 4354 5f49  viron["PROJECT_I
+00001730: 4422 5d0a 2020 2020 2020 2020 656c 6966  D"].        elif
+00001740: 206e 6f74 2064 6973 6162 6c65 5f70 726f   not disable_pro
+00001750: 6d70 743a 0a20 2020 2020 2020 2020 2020  mpt:.           
+00001760: 2063 6f6e 6669 675b 2267 6f6f 676c 655f   config["google_
+00001770: 636c 6f75 645f 706c 6174 666f 726d 225d  cloud_platform"]
+00001780: 5b22 7072 6f6a 6563 7422 5d20 3d20 696e  ["project"] = in
+00001790: 7075 7428 0a20 2020 2020 2020 2020 2020  put(.           
+000017a0: 2020 2020 2022 456e 7465 7220 476f 6f67       "Enter Goog
+000017b0: 6c65 2043 6c6f 7564 2050 6c61 7466 6f72  le Cloud Platfor
+000017c0: 6d20 5072 6f6a 6563 7420 4944 3a20 220a  m Project ID: ".
+000017d0: 2020 2020 2020 2020 2020 2020 290a 0a20              ).. 
+000017e0: 2020 2065 6c69 6620 636c 6f75 645f 7072     elif cloud_pr
+000017f0: 6f76 6964 6572 203d 3d20 5072 6f76 6964  ovider == Provid
+00001800: 6572 456e 756d 2e61 7a75 7265 3a0a 2020  erEnum.azure:.  
+00001810: 2020 2020 2020 617a 7572 655f 7265 6769        azure_regi
+00001820: 6f6e 203d 2072 6567 696f 6e20 6f72 2063  on = region or c
+00001830: 6f6e 7374 616e 7473 2e41 5a55 5245 5f44  onstants.AZURE_D
+00001840: 4546 4155 4c54 5f52 4547 494f 4e0a 2020  EFAULT_REGION.  
+00001850: 2020 2020 2020 617a 7572 655f 6b75 6265        azure_kube
+00001860: 726e 6574 6573 5f76 6572 7369 6f6e 203d  rnetes_version =
+00001870: 206b 7562 6572 6e65 7465 735f 7665 7273   kubernetes_vers
+00001880: 696f 6e20 6f72 2067 6574 5f6c 6174 6573  ion or get_lates
+00001890: 745f 6b75 6265 726e 6574 6573 5f76 6572  t_kubernetes_ver
+000018a0: 7369 6f6e 280a 2020 2020 2020 2020 2020  sion(.          
+000018b0: 2020 617a 7572 655f 636c 6f75 642e 6b75    azure_cloud.ku
+000018c0: 6265 726e 6574 6573 5f76 6572 7369 6f6e  bernetes_version
+000018d0: 7328 617a 7572 655f 7265 6769 6f6e 290a  s(azure_region).
+000018e0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+000018f0: 2020 636f 6e66 6967 5b22 617a 7572 6522    config["azure"
+00001900: 5d20 3d20 7b0a 2020 2020 2020 2020 2020  ] = {.          
+00001910: 2020 226b 7562 6572 6e65 7465 735f 7665    "kubernetes_ve
+00001920: 7273 696f 6e22 3a20 617a 7572 655f 6b75  rsion": azure_ku
+00001930: 6265 726e 6574 6573 5f76 6572 7369 6f6e  bernetes_version
+00001940: 2c0a 2020 2020 2020 2020 2020 2020 2272  ,.            "r
+00001950: 6567 696f 6e22 3a20 617a 7572 655f 7265  egion": azure_re
+00001960: 6769 6f6e 2c0a 2020 2020 2020 2020 2020  gion,.          
+00001970: 2020 2273 746f 7261 6765 5f61 6363 6f75    "storage_accou
+00001980: 6e74 5f70 6f73 7466 6978 223a 2072 616e  nt_postfix": ran
+00001990: 646f 6d5f 7365 6375 7265 5f73 7472 696e  dom_secure_strin
+000019a0: 6728 6c65 6e67 7468 3d34 292c 0a20 2020  g(length=4),.   
+000019b0: 2020 2020 2020 2020 2022 6e6f 6465 5f67           "node_g
+000019c0: 726f 7570 7322 3a20 5f6e 6f64 655f 6772  roups": _node_gr
+000019d0: 6f75 7073 5f74 6f5f 6469 6374 2844 4546  oups_to_dict(DEF
+000019e0: 4155 4c54 5f41 5a55 5245 5f4e 4f44 455f  AULT_AZURE_NODE_
+000019f0: 4752 4f55 5053 292c 0a20 2020 2020 2020  GROUPS),.       
+00001a00: 207d 0a0a 2020 2020 2020 2020 636f 6e66   }..        conf
+00001a10: 6967 5b22 7468 656d 6522 5d5b 226a 7570  ig["theme"]["jup
+00001a20: 7974 6572 6875 6222 5d5b 0a20 2020 2020  yterhub"][.     
+00001a30: 2020 2020 2020 2022 6875 625f 7375 6274         "hub_subt
+00001a40: 6974 6c65 220a 2020 2020 2020 2020 5d20  itle".        ] 
+00001a50: 3d20 6622 7b57 454c 434f 4d45 5f48 4541  = f"{WELCOME_HEA
+00001a60: 4445 525f 5445 5854 7d20 6f6e 2041 7a75  DER_TEXT} on Azu
+00001a70: 7265 220a 0a20 2020 2065 6c69 6620 636c  re"..    elif cl
+00001a80: 6f75 645f 7072 6f76 6964 6572 203d 3d20  oud_provider == 
+00001a90: 5072 6f76 6964 6572 456e 756d 2e61 7773  ProviderEnum.aws
+00001aa0: 3a0a 2020 2020 2020 2020 6177 735f 7265  :.        aws_re
+00001ab0: 6769 6f6e 203d 2028 0a20 2020 2020 2020  gion = (.       
+00001ac0: 2020 2020 2072 6567 696f 6e0a 2020 2020       region.    
+00001ad0: 2020 2020 2020 2020 6f72 206f 732e 656e          or os.en
+00001ae0: 7669 726f 6e2e 6765 7428 2241 5753 5f44  viron.get("AWS_D
+00001af0: 4546 4155 4c54 5f52 4547 494f 4e22 290a  EFAULT_REGION").
+00001b00: 2020 2020 2020 2020 2020 2020 6f72 2063              or c
+00001b10: 6f6e 7374 616e 7473 2e41 5753 5f44 4546  onstants.AWS_DEF
+00001b20: 4155 4c54 5f52 4547 494f 4e0a 2020 2020  AULT_REGION.    
+00001b30: 2020 2020 290a 2020 2020 2020 2020 6177      ).        aw
+00001b40: 735f 6b75 6265 726e 6574 6573 5f76 6572  s_kubernetes_ver
+00001b50: 7369 6f6e 203d 206b 7562 6572 6e65 7465  sion = kubernete
+00001b60: 735f 7665 7273 696f 6e20 6f72 2067 6574  s_version or get
+00001b70: 5f6c 6174 6573 745f 6b75 6265 726e 6574  _latest_kubernet
+00001b80: 6573 5f76 6572 7369 6f6e 280a 2020 2020  es_version(.    
+00001b90: 2020 2020 2020 2020 616d 617a 6f6e 5f77          amazon_w
+00001ba0: 6562 5f73 6572 7669 6365 732e 6b75 6265  eb_services.kube
+00001bb0: 726e 6574 6573 5f76 6572 7369 6f6e 7328  rnetes_versions(
+00001bc0: 6177 735f 7265 6769 6f6e 290a 2020 2020  aws_region).    
+00001bd0: 2020 2020 290a 2020 2020 2020 2020 636f      ).        co
+00001be0: 6e66 6967 5b22 616d 617a 6f6e 5f77 6562  nfig["amazon_web
+00001bf0: 5f73 6572 7669 6365 7322 5d20 3d20 7b0a  _services"] = {.
+00001c00: 2020 2020 2020 2020 2020 2020 226b 7562              "kub
+00001c10: 6572 6e65 7465 735f 7665 7273 696f 6e22  ernetes_version"
+00001c20: 3a20 6177 735f 6b75 6265 726e 6574 6573  : aws_kubernetes
+00001c30: 5f76 6572 7369 6f6e 2c0a 2020 2020 2020  _version,.      
+00001c40: 2020 2020 2020 2272 6567 696f 6e22 3a20        "region": 
+00001c50: 6177 735f 7265 6769 6f6e 2c0a 2020 2020  aws_region,.    
+00001c60: 2020 2020 2020 2020 226e 6f64 655f 6772          "node_gr
+00001c70: 6f75 7073 223a 205f 6e6f 6465 5f67 726f  oups": _node_gro
+00001c80: 7570 735f 746f 5f64 6963 7428 4445 4641  ups_to_dict(DEFA
+00001c90: 554c 545f 4157 535f 4e4f 4445 5f47 524f  ULT_AWS_NODE_GRO
+00001ca0: 5550 5329 2c0a 2020 2020 2020 2020 7d0a  UPS),.        }.
+00001cb0: 2020 2020 2020 2020 636f 6e66 6967 5b22          config["
+00001cc0: 7468 656d 6522 5d5b 226a 7570 7974 6572  theme"]["jupyter
+00001cd0: 6875 6222 5d5b 0a20 2020 2020 2020 2020  hub"][.         
+00001ce0: 2020 2022 6875 625f 7375 6274 6974 6c65     "hub_subtitle
+00001cf0: 220a 2020 2020 2020 2020 5d20 3d20 6622  ".        ] = f"
+00001d00: 7b57 454c 434f 4d45 5f48 4541 4445 525f  {WELCOME_HEADER_
+00001d10: 5445 5854 7d20 6f6e 2041 6d61 7a6f 6e20  TEXT} on Amazon 
+00001d20: 5765 6220 5365 7276 6963 6573 220a 0a20  Web Services".. 
+00001d30: 2020 2065 6c69 6620 636c 6f75 645f 7072     elif cloud_pr
+00001d40: 6f76 6964 6572 203d 3d20 5072 6f76 6964  ovider == Provid
+00001d50: 6572 456e 756d 2e65 7869 7374 696e 673a  erEnum.existing:
+00001d60: 0a20 2020 2020 2020 2063 6f6e 6669 675b  .        config[
+00001d70: 2274 6865 6d65 225d 5b22 6a75 7079 7465  "theme"]["jupyte
+00001d80: 7268 7562 225d 5b22 6875 625f 7375 6274  rhub"]["hub_subt
+00001d90: 6974 6c65 225d 203d 2057 454c 434f 4d45  itle"] = WELCOME
+00001da0: 5f48 4541 4445 525f 5445 5854 0a0a 2020  _HEADER_TEXT..  
+00001db0: 2020 656c 6966 2063 6c6f 7564 5f70 726f    elif cloud_pro
+00001dc0: 7669 6465 7220 3d3d 2050 726f 7669 6465  vider == Provide
+00001dd0: 7245 6e75 6d2e 6c6f 6361 6c3a 0a20 2020  rEnum.local:.   
+00001de0: 2020 2020 2063 6f6e 6669 675b 2274 6865       config["the
+00001df0: 6d65 225d 5b22 6a75 7079 7465 7268 7562  me"]["jupyterhub
+00001e00: 225d 5b22 6875 625f 7375 6274 6974 6c65  "]["hub_subtitle
+00001e10: 225d 203d 2057 454c 434f 4d45 5f48 4541  "] = WELCOME_HEA
+00001e20: 4445 525f 5445 5854 0a0a 2020 2020 6966  DER_TEXT..    if
+00001e30: 2073 736c 5f63 6572 745f 656d 6169 6c3a   ssl_cert_email:
+00001e40: 0a20 2020 2020 2020 2063 6f6e 6669 675b  .        config[
+00001e50: 2263 6572 7469 6669 6361 7465 225d 203d  "certificate"] =
+00001e60: 207b 2274 7970 6522 3a20 4365 7274 6966   {"type": Certif
+00001e70: 6963 6174 6545 6e75 6d2e 6c65 7473 656e  icateEnum.letsen
+00001e80: 6372 7970 742e 7661 6c75 657d 0a20 2020  crypt.value}.   
+00001e90: 2020 2020 2063 6f6e 6669 675b 2263 6572       config["cer
+00001ea0: 7469 6669 6361 7465 225d 5b22 6163 6d65  tificate"]["acme
+00001eb0: 5f65 6d61 696c 225d 203d 2073 736c 5f63  _email"] = ssl_c
+00001ec0: 6572 745f 656d 6169 6c0a 0a20 2020 2023  ert_email..    #
+00001ed0: 2076 616c 6964 6174 6520 636f 6e66 6967   validate config
+00001ee0: 7572 6174 696f 6e20 616e 6420 636f 6e76  uration and conv
+00001ef0: 6572 7420 746f 206d 6f64 656c 0a20 2020  ert to model.   
+00001f00: 2066 726f 6d20 6e65 6261 7269 2e70 6c75   from nebari.plu
+00001f10: 6769 6e73 2069 6d70 6f72 7420 6e65 6261  gins import neba
+00001f20: 7269 5f70 6c75 6769 6e5f 6d61 6e61 6765  ri_plugin_manage
+00001f30: 720a 0a20 2020 2074 7279 3a0a 2020 2020  r..    try:.    
+00001f40: 2020 2020 636f 6e66 6967 5f6d 6f64 656c      config_model
+00001f50: 203d 206e 6562 6172 695f 706c 7567 696e   = nebari_plugin
+00001f60: 5f6d 616e 6167 6572 2e63 6f6e 6669 675f  _manager.config_
+00001f70: 7363 6865 6d61 2e70 6172 7365 5f6f 626a  schema.parse_obj
+00001f80: 2863 6f6e 6669 6729 0a20 2020 2065 7863  (config).    exc
+00001f90: 6570 7420 7079 6461 6e74 6963 2e56 616c  ept pydantic.Val
+00001fa0: 6964 6174 696f 6e45 7272 6f72 2061 7320  idationError as 
+00001fb0: 653a 0a20 2020 2020 2020 2070 7269 6e74  e:.        print
+00001fc0: 2873 7472 2865 2929 0a0a 2020 2020 6966  (str(e))..    if
+00001fd0: 2072 6570 6f73 6974 6f72 795f 6175 746f   repository_auto
+00001fe0: 5f70 726f 7669 7369 6f6e 3a0a 2020 2020  _provision:.    
+00001ff0: 2020 2020 6d61 7463 6820 3d20 7265 2e73      match = re.s
+00002000: 6561 7263 6828 6769 7468 7562 5f75 726c  earch(github_url
+00002010: 5f72 6567 6578 2c20 7265 706f 7369 746f  _regex, reposito
+00002020: 7279 290a 2020 2020 2020 2020 6966 206d  ry).        if m
+00002030: 6174 6368 3a0a 2020 2020 2020 2020 2020  atch:.          
+00002040: 2020 6769 745f 7265 706f 7369 746f 7279    git_repository
+00002050: 203d 2067 6974 6875 625f 6175 746f 5f70   = github_auto_p
+00002060: 726f 7669 7369 6f6e 280a 2020 2020 2020  rovision(.      
+00002070: 2020 2020 2020 2020 2020 636f 6e66 6967            config
+00002080: 5f6d 6f64 656c 2c20 6d61 7463 682e 6772  _model, match.gr
+00002090: 6f75 7028 3229 2c20 6d61 7463 682e 6772  oup(2), match.gr
+000020a0: 6f75 7028 3329 0a20 2020 2020 2020 2020  oup(3).         
+000020b0: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+000020c0: 2067 6974 5f72 6570 6f73 6974 6f72 795f   git_repository_
+000020d0: 696e 6974 6961 6c69 7a65 2867 6974 5f72  initialize(git_r
+000020e0: 6570 6f73 6974 6f72 7929 0a20 2020 2020  epository).     
+000020f0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00002100: 2020 2020 2072 6169 7365 2056 616c 7565       raise Value
+00002110: 4572 726f 7228 0a20 2020 2020 2020 2020  Error(.         
+00002120: 2020 2020 2020 2066 2252 6570 6f73 6974         f"Reposit
+00002130: 6f72 7920 746f 2062 6520 6175 746f 2d70  ory to be auto-p
+00002140: 726f 7669 7369 6f6e 6564 2069 7320 6e6f  rovisioned is no
+00002150: 7420 7468 6520 6675 6c6c 2055 524c 206f  t the full URL o
+00002160: 6620 6120 4769 7448 7562 2072 6570 6f3a  f a GitHub repo:
+00002170: 207b 7265 706f 7369 746f 7279 7d22 0a20   {repository}". 
+00002180: 2020 2020 2020 2020 2020 2029 0a0a 2020             )..  
+00002190: 2020 7265 7475 726e 2063 6f6e 6669 670a    return config.
+000021a0: 0a0a 6465 6620 6769 7468 7562 5f61 7574  ..def github_aut
+000021b0: 6f5f 7072 6f76 6973 696f 6e28 636f 6e66  o_provision(conf
+000021c0: 6967 3a20 7079 6461 6e74 6963 2e42 6173  ig: pydantic.Bas
+000021d0: 654d 6f64 656c 2c20 6f77 6e65 723a 2073  eModel, owner: s
+000021e0: 7472 2c20 7265 706f 3a20 7374 7229 3a0a  tr, repo: str):.
+000021f0: 2020 2020 616c 7265 6164 795f 6578 6973      already_exis
+00002200: 7473 203d 2054 7275 650a 2020 2020 7472  ts = True.    tr
+00002210: 793a 0a20 2020 2020 2020 2067 6974 6875  y:.        githu
+00002220: 622e 6765 745f 7265 706f 7369 746f 7279  b.get_repository
+00002230: 286f 776e 6572 2c20 7265 706f 290a 2020  (owner, repo).  
+00002240: 2020 6578 6365 7074 2072 6571 7565 7374    except request
+00002250: 732e 6578 6365 7074 696f 6e73 2e48 5454  s.exceptions.HTT
+00002260: 5045 7272 6f72 3a0a 2020 2020 2020 2020  PError:.        
+00002270: 2320 7265 706f 206e 6f74 2066 6f75 6e64  # repo not found
+00002280: 0a20 2020 2020 2020 2061 6c72 6561 6479  .        already
+00002290: 5f65 7869 7374 7320 3d20 4661 6c73 650a  _exists = False.
+000022a0: 0a20 2020 2069 6620 6e6f 7420 616c 7265  .    if not alre
+000022b0: 6164 795f 6578 6973 7473 3a0a 2020 2020  ady_exists:.    
+000022c0: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
+000022d0: 2020 2020 2067 6974 6875 622e 6372 6561       github.crea
+000022e0: 7465 5f72 6570 6f73 6974 6f72 7928 0a20  te_repository(. 
+000022f0: 2020 2020 2020 2020 2020 2020 2020 206f                 o
+00002300: 776e 6572 2c0a 2020 2020 2020 2020 2020  wner,.          
+00002310: 2020 2020 2020 7265 706f 2c0a 2020 2020        repo,.    
+00002320: 2020 2020 2020 2020 2020 2020 6465 7363              desc
+00002330: 7269 7074 696f 6e3d 6622 4e65 6261 7269  ription=f"Nebari
+00002340: 207b 636f 6e66 6967 2e70 726f 6a65 6374   {config.project
+00002350: 5f6e 616d 657d 2d7b 636f 6e66 6967 2e70  _name}-{config.p
+00002360: 726f 7669 6465 727d 222c 0a20 2020 2020  rovider}",.     
+00002370: 2020 2020 2020 2020 2020 2068 6f6d 6570             homep
+00002380: 6167 653d 6622 6874 7470 733a 2f2f 7b63  age=f"https://{c
+00002390: 6f6e 6669 672e 646f 6d61 696e 7d22 2c0a  onfig.domain}",.
+000023a0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+000023b0: 2020 2020 2020 6578 6365 7074 2072 6571        except req
+000023c0: 7565 7374 732e 6578 6365 7074 696f 6e73  uests.exceptions
+000023d0: 2e48 5454 5045 7272 6f72 2061 7320 6865  .HTTPError as he
+000023e0: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
+000023f0: 6973 6520 5661 6c75 6545 7272 6f72 280a  ise ValueError(.
+00002400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002410: 6622 556e 6162 6c65 2074 6f20 6372 6561  f"Unable to crea
+00002420: 7465 2047 6974 4875 6220 7265 706f 2068  te GitHub repo h
+00002430: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00002440: 6d2f 7b6f 776e 6572 7d2f 7b72 6570 6f7d  m/{owner}/{repo}
+00002450: 202d 2065 7272 6f72 206d 6573 7361 6765   - error message
+00002460: 2066 726f 6d20 4769 7448 7562 2069 733a   from GitHub is:
+00002470: 207b 6865 7d22 0a20 2020 2020 2020 2020   {he}".         
+00002480: 2020 2029 0a20 2020 2065 6c73 653a 0a20     ).    else:. 
+00002490: 2020 2020 2020 206c 6f67 6765 722e 7761         logger.wa
+000024a0: 726e 696e 6728 6622 4769 7448 7562 2072  rning(f"GitHub r
+000024b0: 6570 6f20 6874 7470 733a 2f2f 6769 7468  epo https://gith
+000024c0: 7562 2e63 6f6d 2f7b 6f77 6e65 727d 2f7b  ub.com/{owner}/{
+000024d0: 7265 706f 7d20 616c 7265 6164 7920 6578  repo} already ex
+000024e0: 6973 7473 2229 0a0a 2020 2020 7472 793a  ists")..    try:
+000024f0: 0a20 2020 2020 2020 2023 2053 6563 7265  .        # Secre
+00002500: 7473 0a20 2020 2020 2020 2069 6620 636f  ts.        if co
+00002510: 6e66 6967 2e70 726f 7669 6465 7220 3d3d  nfig.provider ==
+00002520: 2050 726f 7669 6465 7245 6e75 6d2e 646f   ProviderEnum.do
+00002530: 3a0a 2020 2020 2020 2020 2020 2020 666f  :.            fo
+00002540: 7220 6e61 6d65 2069 6e20 7b0a 2020 2020  r name in {.    
+00002550: 2020 2020 2020 2020 2020 2020 2241 5753              "AWS
+00002560: 5f41 4343 4553 535f 4b45 595f 4944 222c  _ACCESS_KEY_ID",
+00002570: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002580: 2022 4157 535f 5345 4352 4554 5f41 4343   "AWS_SECRET_ACC
+00002590: 4553 535f 4b45 5922 2c0a 2020 2020 2020  ESS_KEY",.      
+000025a0: 2020 2020 2020 2020 2020 2253 5041 4345            "SPACE
+000025b0: 535f 4143 4345 5353 5f4b 4559 5f49 4422  S_ACCESS_KEY_ID"
+000025c0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000025d0: 2020 2253 5041 4345 535f 5345 4352 4554    "SPACES_SECRET
+000025e0: 5f41 4343 4553 535f 4b45 5922 2c0a 2020  _ACCESS_KEY",.  
+000025f0: 2020 2020 2020 2020 2020 2020 2020 2244                "D
+00002600: 4947 4954 414c 4f43 4541 4e5f 544f 4b45  IGITALOCEAN_TOKE
+00002610: 4e22 2c0a 2020 2020 2020 2020 2020 2020  N",.            
+00002620: 7d3a 0a20 2020 2020 2020 2020 2020 2020  }:.             
+00002630: 2020 2067 6974 6875 622e 7570 6461 7465     github.update
+00002640: 5f73 6563 7265 7428 6f77 6e65 722c 2072  _secret(owner, r
+00002650: 6570 6f2c 206e 616d 652c 206f 732e 656e  epo, name, os.en
+00002660: 7669 726f 6e5b 6e61 6d65 5d29 0a20 2020  viron[name]).   
+00002670: 2020 2020 2065 6c69 6620 636f 6e66 6967       elif config
+00002680: 2e70 726f 7669 6465 7220 3d3d 2050 726f  .provider == Pro
+00002690: 7669 6465 7245 6e75 6d2e 6177 733a 0a20  viderEnum.aws:. 
+000026a0: 2020 2020 2020 2020 2020 2066 6f72 206e             for n
+000026b0: 616d 6520 696e 207b 0a20 2020 2020 2020  ame in {.       
+000026c0: 2020 2020 2020 2020 2022 4157 535f 4143           "AWS_AC
+000026d0: 4345 5353 5f4b 4559 5f49 4422 2c0a 2020  CESS_KEY_ID",.  
+000026e0: 2020 2020 2020 2020 2020 2020 2020 2241                "A
+000026f0: 5753 5f53 4543 5245 545f 4143 4345 5353  WS_SECRET_ACCESS
+00002700: 5f4b 4559 222c 0a20 2020 2020 2020 2020  _KEY",.         
+00002710: 2020 207d 3a0a 2020 2020 2020 2020 2020     }:.          
+00002720: 2020 2020 2020 6769 7468 7562 2e75 7064        github.upd
+00002730: 6174 655f 7365 6372 6574 286f 776e 6572  ate_secret(owner
+00002740: 2c20 7265 706f 2c20 6e61 6d65 2c20 6f73  , repo, name, os
+00002750: 2e65 6e76 6972 6f6e 5b6e 616d 655d 290a  .environ[name]).
+00002760: 2020 2020 2020 2020 656c 6966 2063 6f6e          elif con
+00002770: 6669 672e 7072 6f76 6964 6572 203d 3d20  fig.provider == 
+00002780: 5072 6f76 6964 6572 456e 756d 2e67 6370  ProviderEnum.gcp
+00002790: 3a0a 2020 2020 2020 2020 2020 2020 6769  :.            gi
+000027a0: 7468 7562 2e75 7064 6174 655f 7365 6372  thub.update_secr
+000027b0: 6574 286f 776e 6572 2c20 7265 706f 2c20  et(owner, repo, 
+000027c0: 2250 524f 4a45 4354 5f49 4422 2c20 6f73  "PROJECT_ID", os
+000027d0: 2e65 6e76 6972 6f6e 5b22 5052 4f4a 4543  .environ["PROJEC
+000027e0: 545f 4944 225d 290a 2020 2020 2020 2020  T_ID"]).        
+000027f0: 2020 2020 7769 7468 206f 7065 6e28 6f73      with open(os
+00002800: 2e65 6e76 6972 6f6e 5b22 474f 4f47 4c45  .environ["GOOGLE
+00002810: 5f43 5245 4445 4e54 4941 4c53 225d 2920  _CREDENTIALS"]) 
+00002820: 6173 2066 3a0a 2020 2020 2020 2020 2020  as f:.          
+00002830: 2020 2020 2020 6769 7468 7562 2e75 7064        github.upd
+00002840: 6174 655f 7365 6372 6574 286f 776e 6572  ate_secret(owner
+00002850: 2c20 7265 706f 2c20 2247 4f4f 474c 455f  , repo, "GOOGLE_
+00002860: 4352 4544 454e 5449 414c 5322 2c20 662e  CREDENTIALS", f.
+00002870: 7265 6164 2829 290a 2020 2020 2020 2020  read()).        
+00002880: 656c 6966 2063 6f6e 6669 672e 7072 6f76  elif config.prov
+00002890: 6964 6572 203d 3d20 5072 6f76 6964 6572  ider == Provider
+000028a0: 456e 756d 2e61 7a75 7265 3a0a 2020 2020  Enum.azure:.    
+000028b0: 2020 2020 2020 2020 666f 7220 6e61 6d65          for name
+000028c0: 2069 6e20 7b0a 2020 2020 2020 2020 2020   in {.          
+000028d0: 2020 2020 2020 2241 524d 5f43 4c49 454e        "ARM_CLIEN
+000028e0: 545f 4944 222c 0a20 2020 2020 2020 2020  T_ID",.         
+000028f0: 2020 2020 2020 2022 4152 4d5f 434c 4945         "ARM_CLIE
+00002900: 4e54 5f53 4543 5245 5422 2c0a 2020 2020  NT_SECRET",.    
+00002910: 2020 2020 2020 2020 2020 2020 2241 524d              "ARM
+00002920: 5f53 5542 5343 5249 5054 494f 4e5f 4944  _SUBSCRIPTION_ID
+00002930: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00002940: 2020 2022 4152 4d5f 5445 4e41 4e54 5f49     "ARM_TENANT_I
+00002950: 4422 2c0a 2020 2020 2020 2020 2020 2020  D",.            
+00002960: 7d3a 0a20 2020 2020 2020 2020 2020 2020  }:.             
+00002970: 2020 2067 6974 6875 622e 7570 6461 7465     github.update
+00002980: 5f73 6563 7265 7428 6f77 6e65 722c 2072  _secret(owner, r
+00002990: 6570 6f2c 206e 616d 652c 206f 732e 656e  epo, name, os.en
+000029a0: 7669 726f 6e5b 6e61 6d65 5d29 0a20 2020  viron[name]).   
+000029b0: 2020 2020 2067 6974 6875 622e 7570 6461       github.upda
+000029c0: 7465 5f73 6563 7265 7428 0a20 2020 2020  te_secret(.     
+000029d0: 2020 2020 2020 206f 776e 6572 2c20 7265         owner, re
+000029e0: 706f 2c20 2252 4550 4f53 4954 4f52 595f  po, "REPOSITORY_
+000029f0: 4143 4345 5353 5f54 4f4b 454e 222c 206f  ACCESS_TOKEN", o
+00002a00: 732e 656e 7669 726f 6e5b 2247 4954 4855  s.environ["GITHU
+00002a10: 425f 544f 4b45 4e22 5d0a 2020 2020 2020  B_TOKEN"].      
+00002a20: 2020 290a 2020 2020 6578 6365 7074 2072    ).    except r
+00002a30: 6571 7565 7374 732e 6578 6365 7074 696f  equests.exceptio
+00002a40: 6e73 2e48 5454 5045 7272 6f72 2061 7320  ns.HTTPError as 
+00002a50: 6865 3a0a 2020 2020 2020 2020 7261 6973  he:.        rais
+00002a60: 6520 5661 6c75 6545 7272 6f72 280a 2020  e ValueError(.  
+00002a70: 2020 2020 2020 2020 2020 6622 556e 6162            f"Unab
+00002a80: 6c65 2074 6f20 7365 7420 5365 6372 6574  le to set Secret
+00002a90: 7320 6f6e 2047 6974 4875 6220 7265 706f  s on GitHub repo
+00002aa0: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
+00002ab0: 636f 6d2f 7b6f 776e 6572 7d2f 7b72 6570  com/{owner}/{rep
+00002ac0: 6f7d 202d 2065 7272 6f72 206d 6573 7361  o} - error messa
+00002ad0: 6765 2066 726f 6d20 4769 7448 7562 2069  ge from GitHub i
+00002ae0: 733a 207b 6865 7d22 0a20 2020 2020 2020  s: {he}".       
+00002af0: 2029 0a0a 2020 2020 7265 7475 726e 2066   )..    return f
+00002b00: 2267 6974 4067 6974 6875 622e 636f 6d3a  "git@github.com:
+00002b10: 7b6f 776e 6572 7d2f 7b72 6570 6f7d 2e67  {owner}/{repo}.g
+00002b20: 6974 220a 0a0a 6465 6620 6769 745f 7265  it"...def git_re
+00002b30: 706f 7369 746f 7279 5f69 6e69 7469 616c  pository_initial
+00002b40: 697a 6528 6769 745f 7265 706f 7369 746f  ize(git_reposito
+00002b50: 7279 293a 0a20 2020 2069 6620 6e6f 7420  ry):.    if not 
+00002b60: 6769 742e 6973 5f67 6974 5f72 6570 6f28  git.is_git_repo(
+00002b70: 5061 7468 2e63 7764 2829 293a 0a20 2020  Path.cwd()):.   
+00002b80: 2020 2020 2067 6974 2e69 6e69 7469 616c       git.initial
+00002b90: 697a 655f 6769 7428 5061 7468 2e63 7764  ize_git(Path.cwd
+00002ba0: 2829 290a 2020 2020 6769 742e 6164 645f  ()).    git.add_
+00002bb0: 6769 745f 7265 6d6f 7465 2867 6974 5f72  git_remote(git_r
+00002bc0: 6570 6f73 6974 6f72 792c 2070 6174 683d  epository, path=
+00002bd0: 5061 7468 2e63 7764 2829 2c20 7265 6d6f  Path.cwd(), remo
+00002be0: 7465 5f6e 616d 653d 226f 7269 6769 6e22  te_name="origin"
+00002bf0: 290a                                     ).
```

### Comparing `nebari-2024.3.3rc1/src/_nebari/keycloak.py` & `nebari-2024.4.1rc1/src/_nebari/keycloak.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/render.py` & `nebari-2024.4.1rc1/src/_nebari/render.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/upgrade.py` & `nebari-2024.4.1rc1/src/_nebari/upgrade.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/utils.py` & `nebari-2024.4.1rc1/src/_nebari/utils.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/version.py` & `nebari-2024.4.1rc1/src/_nebari/version.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/provider/git.py` & `nebari-2024.4.1rc1/src/_nebari/provider/git.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/provider/terraform.py` & `nebari-2024.4.1rc1/src/_nebari/provider/terraform.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/provider/cicd/github.py` & `nebari-2024.4.1rc1/src/_nebari/provider/cicd/github.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/provider/cicd/gitlab.py` & `nebari-2024.4.1rc1/src/_nebari/provider/cicd/gitlab.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/provider/cicd/linter.py` & `nebari-2024.4.1rc1/src/_nebari/provider/cicd/linter.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/provider/cloud/amazon_web_services.py` & `nebari-2024.4.1rc1/src/_nebari/provider/cloud/amazon_web_services.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/provider/cloud/azure_cloud.py` & `nebari-2024.4.1rc1/src/_nebari/provider/cloud/azure_cloud.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/provider/cloud/digital_ocean.py` & `nebari-2024.4.1rc1/src/_nebari/provider/cloud/digital_ocean.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/provider/cloud/google_cloud.py` & `nebari-2024.4.1rc1/src/_nebari/provider/cloud/google_cloud.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/provider/dns/cloudflare.py` & `nebari-2024.4.1rc1/src/_nebari/provider/dns/cloudflare.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/provider/oauth/auth0.py` & `nebari-2024.4.1rc1/src/_nebari/provider/oauth/auth0.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/base.py` & `nebari-2024.4.1rc1/src/_nebari/stages/base.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/tf_objects.py` & `nebari-2024.4.1rc1/src/_nebari/stages/tf_objects.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/bootstrap/__init__.py` & `nebari-2024.4.1rc1/src/_nebari/stages/bootstrap/__init__.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/infrastructure/__init__.py` & `nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -219,29 +219,26 @@
     """
 
     instance: str
     min_nodes: pydantic.conint(ge=1) = 1
     max_nodes: pydantic.conint(ge=1) = 1
 
 
+DEFAULT_DO_NODE_GROUPS = {
+    "general": DigitalOceanNodeGroup(instance="g-8vcpu-32gb", min_nodes=1, max_nodes=1),
+    "user": DigitalOceanNodeGroup(instance="g-4vcpu-16gb", min_nodes=1, max_nodes=5),
+    "worker": DigitalOceanNodeGroup(instance="g-4vcpu-16gb", min_nodes=1, max_nodes=5),
+}
+
+
 class DigitalOceanProvider(schema.Base):
     region: str
     kubernetes_version: str
     # Digital Ocean image slugs are listed here https://slugs.do-api.dev/
-    node_groups: Dict[str, DigitalOceanNodeGroup] = {
-        "general": DigitalOceanNodeGroup(
-            instance="g-8vcpu-32gb", min_nodes=1, max_nodes=1
-        ),
-        "user": DigitalOceanNodeGroup(
-            instance="g-4vcpu-16gb", min_nodes=1, max_nodes=5
-        ),
-        "worker": DigitalOceanNodeGroup(
-            instance="g-4vcpu-16gb", min_nodes=1, max_nodes=5
-        ),
-    }
+    node_groups: Dict[str, DigitalOceanNodeGroup] = DEFAULT_DO_NODE_GROUPS
     tags: Optional[List[str]] = []
 
     @pydantic.validator("region")
     def _validate_region(cls, value):
         digital_ocean.check_credentials()
 
         available_regions = set(_["slug"] for _ in digital_ocean.regions())
@@ -325,25 +322,28 @@
     min_nodes: pydantic.conint(ge=0) = 0
     max_nodes: pydantic.conint(ge=1) = 1
     preemptible: bool = False
     labels: Dict[str, str] = {}
     guest_accelerators: List[GCPGuestAccelerator] = []
 
 
+DEFAULT_GCP_NODE_GROUPS = {
+    "general": GCPNodeGroup(instance="n1-standard-8", min_nodes=1, max_nodes=1),
+    "user": GCPNodeGroup(instance="n1-standard-4", min_nodes=0, max_nodes=5),
+    "worker": GCPNodeGroup(instance="n1-standard-4", min_nodes=0, max_nodes=5),
+}
+
+
 class GoogleCloudPlatformProvider(schema.Base):
     region: str
     project: str
     kubernetes_version: str
     availability_zones: Optional[List[str]] = []
     release_channel: str = constants.DEFAULT_GKE_RELEASE_CHANNEL
-    node_groups: Dict[str, GCPNodeGroup] = {
-        "general": GCPNodeGroup(instance="n1-standard-8", min_nodes=1, max_nodes=1),
-        "user": GCPNodeGroup(instance="n1-standard-4", min_nodes=0, max_nodes=5),
-        "worker": GCPNodeGroup(instance="n1-standard-4", min_nodes=0, max_nodes=5),
-    }
+    node_groups: Dict[str, GCPNodeGroup] = DEFAULT_GCP_NODE_GROUPS
     tags: Optional[List[str]] = []
     networking_mode: str = "ROUTE"
     network: str = "default"
     subnetwork: Optional[Union[str, None]] = None
     ip_allocation_policy: Optional[Union[GCPIPAllocationPolicy, None]] = None
     master_authorized_networks_config: Optional[Union[GCPCIDRBlock, None]] = None
     private_cluster_config: Optional[Union[GCPPrivateClusterConfig, None]] = None
@@ -377,24 +377,27 @@
 
 class AzureNodeGroup(schema.Base):
     instance: str
     min_nodes: int
     max_nodes: int
 
 
+DEFAULT_AZURE_NODE_GROUPS = {
+    "general": AzureNodeGroup(instance="Standard_D8_v3", min_nodes=1, max_nodes=1),
+    "user": AzureNodeGroup(instance="Standard_D4_v3", min_nodes=0, max_nodes=5),
+    "worker": AzureNodeGroup(instance="Standard_D4_v3", min_nodes=0, max_nodes=5),
+}
+
+
 class AzureProvider(schema.Base):
     region: str
     kubernetes_version: str
     storage_account_postfix: str
     resource_group_name: str = None
-    node_groups: Dict[str, AzureNodeGroup] = {
-        "general": AzureNodeGroup(instance="Standard_D8_v3", min_nodes=1, max_nodes=1),
-        "user": AzureNodeGroup(instance="Standard_D4_v3", min_nodes=0, max_nodes=5),
-        "worker": AzureNodeGroup(instance="Standard_D4_v3", min_nodes=0, max_nodes=5),
-    }
+    node_groups: Dict[str, AzureNodeGroup] = DEFAULT_AZURE_NODE_GROUPS
     storage_account_postfix: str
     vnet_subnet_id: Optional[Union[str, None]] = None
     private_cluster_enabled: bool = False
     resource_group_name: Optional[str] = None
     tags: Optional[Dict[str, str]] = {}
     network_profile: Optional[Dict[str, str]] = None
     max_pods: Optional[int] = None
@@ -438,27 +441,30 @@
     min_nodes: int = 0
     max_nodes: int
     gpu: bool = False
     single_subnet: bool = False
     permissions_boundary: Optional[str] = None
 
 
+DEFAULT_AWS_NODE_GROUPS = {
+    "general": AWSNodeGroup(instance="m5.2xlarge", min_nodes=1, max_nodes=1),
+    "user": AWSNodeGroup(
+        instance="m5.xlarge", min_nodes=0, max_nodes=5, single_subnet=False
+    ),
+    "worker": AWSNodeGroup(
+        instance="m5.xlarge", min_nodes=0, max_nodes=5, single_subnet=False
+    ),
+}
+
+
 class AmazonWebServicesProvider(schema.Base):
     region: str
     kubernetes_version: str
     availability_zones: Optional[List[str]]
-    node_groups: Dict[str, AWSNodeGroup] = {
-        "general": AWSNodeGroup(instance="m5.2xlarge", min_nodes=1, max_nodes=1),
-        "user": AWSNodeGroup(
-            instance="m5.xlarge", min_nodes=0, max_nodes=5, single_subnet=False
-        ),
-        "worker": AWSNodeGroup(
-            instance="m5.xlarge", min_nodes=0, max_nodes=5, single_subnet=False
-        ),
-    }
+    node_groups: Dict[str, AWSNodeGroup] = DEFAULT_AWS_NODE_GROUPS
     existing_subnet_ids: List[str] = None
     existing_security_group_id: str = None
     vpc_cidr_block: str = "10.10.0.0/16"
     permissions_boundary: Optional[str] = None
     tags: Optional[Dict[str, str]] = {}
 
     @pydantic.root_validator
```

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/infrastructure/template/aws/main.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/infrastructure/template/aws/outputs.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/outputs.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/infrastructure/template/aws/variables.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/infrastructure/template/aws/modules/accounting/main.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/accounting/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/infrastructure/template/aws/modules/efs/variables.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/efs/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/infrastructure/template/aws/modules/kafka/main.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/kafka/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/infrastructure/template/aws/modules/kafka/variables.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/kafka/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/infrastructure/template/aws/modules/kubernetes/autoscaling.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/kubernetes/autoscaling.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/infrastructure/template/aws/modules/kubernetes/locals.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/kubernetes/locals.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/infrastructure/template/aws/modules/kubernetes/main.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/kubernetes/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/infrastructure/template/aws/modules/kubernetes/outputs.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/kubernetes/outputs.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/infrastructure/template/aws/modules/kubernetes/policy.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/kubernetes/policy.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/infrastructure/template/aws/modules/kubernetes/variables.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/kubernetes/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/infrastructure/template/aws/modules/network/main.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/network/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/infrastructure/template/aws/modules/network/variables.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/network/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/infrastructure/template/aws/modules/permissions/main.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/permissions/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/infrastructure/template/aws/modules/permissions/variables.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/permissions/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/infrastructure/template/aws/modules/rds/main.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/rds/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/infrastructure/template/aws/modules/rds/users.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/rds/users.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/infrastructure/template/aws/modules/rds/variables.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/rds/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/infrastructure/template/azure/main.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/azure/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/infrastructure/template/azure/outputs.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/azure/outputs.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/infrastructure/template/azure/variables.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/azure/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/infrastructure/template/azure/modules/kubernetes/main.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/azure/modules/kubernetes/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/infrastructure/template/azure/modules/kubernetes/outputs.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/azure/modules/kubernetes/outputs.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/infrastructure/template/azure/modules/kubernetes/variables.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/azure/modules/kubernetes/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/infrastructure/template/do/main.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/do/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/infrastructure/template/do/outputs.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/do/outputs.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/infrastructure/template/do/variables.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/do/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/infrastructure/template/do/modules/kubernetes/main.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/do/modules/kubernetes/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/infrastructure/template/do/modules/kubernetes/outputs.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/do/modules/kubernetes/outputs.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/infrastructure/template/do/modules/kubernetes/variables.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/do/modules/kubernetes/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/infrastructure/template/gcp/main.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/gcp/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/infrastructure/template/gcp/outputs.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/gcp/outputs.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/infrastructure/template/gcp/variables.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/gcp/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/infrastructure/template/gcp/modules/kubernetes/locals.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/gcp/modules/kubernetes/locals.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/infrastructure/template/gcp/modules/kubernetes/main.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/gcp/modules/kubernetes/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/infrastructure/template/gcp/modules/kubernetes/outputs.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/gcp/modules/kubernetes/outputs.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/infrastructure/template/gcp/modules/kubernetes/variables.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/gcp/modules/kubernetes/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/infrastructure/template/local/main.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/local/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/infrastructure/template/local/metallb.yaml` & `nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/local/metallb.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/infrastructure/template/local/outputs.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/infrastructure/template/local/outputs.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_ingress/__init__.py` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_ingress/__init__.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_ingress/template/main.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_ingress/template/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_ingress/template/variables.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_ingress/template/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_ingress/template/modules/kubernetes/ingress/main.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_ingress/template/modules/kubernetes/ingress/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_ingress/template/modules/kubernetes/ingress/variables.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_ingress/template/modules/kubernetes/ingress/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_initialize/__init__.py` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_initialize/__init__.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_initialize/template/main.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_initialize/template/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_initialize/template/variables.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_initialize/template/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_initialize/template/modules/cluster-autoscaler/main.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_initialize/template/modules/cluster-autoscaler/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_initialize/template/modules/extcr/main.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_initialize/template/modules/extcr/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_initialize/template/modules/extcr/variables.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_initialize/template/modules/extcr/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_initialize/template/modules/nvidia-installer/aws-nvidia-installer.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_initialize/template/modules/nvidia-installer/aws-nvidia-installer.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_initialize/template/modules/nvidia-installer/gcp-nvidia-installer.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_initialize/template/modules/nvidia-installer/gcp-nvidia-installer.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_initialize/template/modules/traefik_crds/main.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_initialize/template/modules/traefik_crds/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_keycloak/__init__.py` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_keycloak/__init__.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_keycloak/template/variables.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_keycloak/template/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_keycloak/template/modules/kubernetes/keycloak-helm/main.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_keycloak/template/modules/kubernetes/keycloak-helm/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_keycloak/template/modules/kubernetes/keycloak-helm/values.yaml` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_keycloak/template/modules/kubernetes/keycloak-helm/values.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_keycloak/template/modules/kubernetes/keycloak-helm/variables.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_keycloak/template/modules/kubernetes/keycloak-helm/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_keycloak_configuration/__init__.py` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_keycloak_configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_keycloak_configuration/template/main.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_keycloak_configuration/template/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_keycloak_configuration/template/permissions.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_keycloak_configuration/template/permissions.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_keycloak_configuration/template/social_auth.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_keycloak_configuration/template/social_auth.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_keycloak_configuration/template/variables.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_keycloak_configuration/template/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/__init__.py` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/__init__.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/argo-workflows.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/argo-workflows.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/conda-store.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/conda-store.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/dask_gateway.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/dask_gateway.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/jupyterhub.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/jupyterhub.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/monitoring.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/monitoring.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/outputs.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/outputs.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/variables.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/forwardauth/main.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/forwardauth/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/forwardauth/variables.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/forwardauth/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/nfs-mount/main.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/nfs-mount/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/nfs-server/main.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/nfs-server/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/argo-workflows/main.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/argo-workflows/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/argo-workflows/variables.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/argo-workflows/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/conda-store/output.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/conda-store/output.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/conda-store/server.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/conda-store/server.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/conda-store/storage.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/conda-store/storage.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/conda-store/variables.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/conda-store/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/conda-store/worker.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/conda-store/worker.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/conda-store/config/conda_store_config.py` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/conda-store/config/conda_store_config.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/controler.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/controler.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/crds.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/crds.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/gateway.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/gateway.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/main.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/middleware.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/middleware.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/variables.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/files/controller_config.py` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/files/controller_config.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/files/gateway_config.py` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/files/gateway_config.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/configmaps.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/configmaps.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/main.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/main.tf`

 * *Files 10% similar despite different names*

```diff
@@ -146,26 +146,33 @@
           JupyterHub = {
             authenticator_class = "generic-oauth"
           }
           Authenticator = {
             enable_auth_state = true
           }
           GenericOAuthenticator = {
-            client_id          = module.jupyterhub-openid-client.config.client_id
-            client_secret      = module.jupyterhub-openid-client.config.client_secret
-            oauth_callback_url = "https://${var.external-url}/hub/oauth_callback"
-            authorize_url      = module.jupyterhub-openid-client.config.authentication_url
-            token_url          = module.jupyterhub-openid-client.config.token_url
-            userdata_url       = module.jupyterhub-openid-client.config.userinfo_url
-            login_service      = "Keycloak"
-            username_key       = "preferred_username"
-            claim_groups_key   = "roles"
-            allowed_groups     = ["jupyterhub_admin", "jupyterhub_developer"]
-            admin_groups       = ["jupyterhub_admin"]
-            tls_verify         = false
+            client_id            = module.jupyterhub-openid-client.config.client_id
+            client_secret        = module.jupyterhub-openid-client.config.client_secret
+            oauth_callback_url   = "https://${var.external-url}/hub/oauth_callback"
+            authorize_url        = module.jupyterhub-openid-client.config.authentication_url
+            token_url            = module.jupyterhub-openid-client.config.token_url
+            userdata_url         = module.jupyterhub-openid-client.config.userinfo_url
+            login_service        = "Keycloak"
+            username_claim       = "preferred_username"
+            claim_groups_key     = "groups"
+            allowed_groups       = ["/analyst", "/developer", "/admin"]
+            admin_groups         = ["/admin"]
+            manage_groups        = true
+            refresh_pre_spawn    = true
+            validate_server_cert = false
+
+            # deprecated, to be removed (replaced by validate_server_cert)
+            tls_verify = false
+            # deprecated, to be removed (replaced by username_claim)
+            username_key = "preferred_username"
           }
         }
       }
 
       proxy = {
         chp = {
           nodeSelector = {
@@ -227,14 +234,36 @@
           match = "Host(`${var.external-url}`) && (Path(`/`) || PathPrefix(`/hub`) || PathPrefix(`/user`) || PathPrefix(`/services`))"
           services = [
             {
               name = "proxy-public"
               port = 80
             }
           ]
+          middlewares = [
+            {
+              name      = kubernetes_manifest.jupyterhub-proxy-add-slash.manifest.metadata.name
+              namespace = var.namespace
+            }
+          ]
+        },
+        {
+          kind  = "Rule"
+          match = "Host(`${var.external-url}`) && (PathPrefix(`/home`) || PathPrefix(`/token`) || PathPrefix(`/admin`))"
+          middlewares = [
+            {
+              name      = kubernetes_manifest.jupyterhub-middleware-addprefix.manifest.metadata.name
+              namespace = var.namespace
+            }
+          ]
+          services = [
+            {
+              name = "proxy-public"
+              port = 80
+            }
+          ]
         }
       ]
     }
   }
 }
```

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/values.yaml` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/values.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/variables.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/extras/git_clone_update.sh` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/extras/git_clone_update.sh`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/jupyter/jupyter_jupyterlab_pioneer_config.py.tpl` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/jupyter/jupyter_jupyterlab_pioneer_config.py.tpl`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/jupyter/jupyter_server_config.py.tpl` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/jupyter/jupyter_server_config.py.tpl`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/jupyterhub/02-spawner.py` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/jupyterhub/02-spawner.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/jupyterhub/03-profiles.py` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/jupyterhub/03-profiles.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/jupyterlab/overrides.json` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/jupyterlab/overrides.json`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/skel/.bashrc` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/skel/.bashrc`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/skel/.profile` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/skel/.profile`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub-ssh/main.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub-ssh/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub-ssh/sftp.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub-ssh/sftp.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub-ssh/ssh.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub-ssh/ssh.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub-ssh/variables.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub-ssh/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/keycloak-client/main.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/keycloak-client/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/keycloak-client/outputs.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/keycloak-client/outputs.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/keycloak-client/variables.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/keycloak-client/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/minio/ingress.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/minio/ingress.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/minio/main.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/minio/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/minio/variables.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/minio/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/main.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/variables.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/dashboards/Main/cluster_information.json` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/dashboards/Main/cluster_information.json`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/dashboards/Main/conda_store.json` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/dashboards/Main/conda_store.json`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/dashboards/Main/jupyterhub_dashboard.json` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/dashboards/Main/jupyterhub_dashboard.json`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/dashboards/Main/keycloak.json` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/dashboards/Main/keycloak.json`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/dashboards/Main/traefik.json` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/dashboards/Main/traefik.json`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/dashboards/Main/usage_report.json` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/dashboards/Main/usage_report.json`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/loki/main.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/loki/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/loki/values_loki.yaml` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/loki/values_loki.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/loki/variables.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/loki/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/postgresql/main.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/postgresql/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/postgresql/variables.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/postgresql/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/redis/main.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/redis/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/redis/variables.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/redis/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/nebari_tf_extensions/__init__.py` & `nebari-2024.4.1rc1/src/_nebari/stages/nebari_tf_extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/nebari_tf_extensions/template/tf-extensions.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/nebari_tf_extensions/template/tf-extensions.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/nebari_tf_extensions/template/variables.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/nebari_tf_extensions/template/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/nebari_tf_extensions/template/modules/helm-extensions/variables.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/nebari_tf_extensions/template/modules/helm-extensions/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/nebari_tf_extensions/template/modules/nebariextension/ingress.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/nebari_tf_extensions/template/modules/nebariextension/ingress.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/nebari_tf_extensions/template/modules/nebariextension/keycloak-config.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/nebari_tf_extensions/template/modules/nebariextension/keycloak-config.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/nebari_tf_extensions/template/modules/nebariextension/locals.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/nebari_tf_extensions/template/modules/nebariextension/locals.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/nebari_tf_extensions/template/modules/nebariextension/main.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/nebari_tf_extensions/template/modules/nebariextension/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/nebari_tf_extensions/template/modules/nebariextension/variables.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/nebari_tf_extensions/template/modules/nebariextension/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/terraform_state/__init__.py` & `nebari-2024.4.1rc1/src/_nebari/stages/terraform_state/__init__.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/terraform_state/template/aws/main.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/terraform_state/template/aws/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/terraform_state/template/aws/modules/terraform-state/main.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/terraform_state/template/aws/modules/terraform-state/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/terraform_state/template/azure/main.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/terraform_state/template/azure/main.tf`

 * *Files 8% similar despite different names*

```diff
@@ -43,12 +43,12 @@
   tags                    = var.tags
 }
 
 terraform {
   required_providers {
     azurerm = {
       source  = "hashicorp/azurerm"
-      version = "=3.22.0"
+      version = "=3.97.1"
     }
   }
   required_version = ">= 1.0"
 }
```

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/terraform_state/template/azure/modules/terraform-state/main.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/terraform_state/template/azure/modules/terraform-state/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/terraform_state/template/azure/modules/terraform-state/variables.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/terraform_state/template/azure/modules/terraform-state/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/terraform_state/template/do/main.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/terraform_state/template/do/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/terraform_state/template/gcp/main.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/terraform_state/template/gcp/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/stages/terraform_state/template/gcp/modules/gcs/variables.tf` & `nebari-2024.4.1rc1/src/_nebari/stages/terraform_state/template/gcp/modules/gcs/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/subcommands/deploy.py` & `nebari-2024.4.1rc1/src/_nebari/subcommands/deploy.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/subcommands/destroy.py` & `nebari-2024.4.1rc1/src/_nebari/subcommands/destroy.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/subcommands/dev.py` & `nebari-2024.4.1rc1/src/_nebari/subcommands/dev.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/subcommands/info.py` & `nebari-2024.4.1rc1/src/_nebari/subcommands/info.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/subcommands/init.py` & `nebari-2024.4.1rc1/src/_nebari/subcommands/init.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,14 +71,23 @@
 
 DEFAULT_KUBERNETES_VERSION_MSG = (
     "Defaulting to highest supported Kubernetes version: `{kubernetes_version}`."
 )
 
 LATEST = "latest"
 
+CLOUD_PROVIDER_FULL_NAME = {
+    "Local": ProviderEnum.local.name,
+    "Existing": ProviderEnum.existing.name,
+    "Digital Ocean": ProviderEnum.do.name,
+    "Amazon Web Services": ProviderEnum.aws.name,
+    "Google Cloud Platform": ProviderEnum.gcp.name,
+    "Microsoft Azure": ProviderEnum.azure.name,
+}
+
 
 class GitRepoEnum(str, enum.Enum):
     github = "github.com"
     gitlab = "gitlab.com"
 
 
 class InitInputs(schema.Base):
@@ -643,20 +652,22 @@
                 f"{LINKS_TO_DOCS_TEMPLATE.format(link_to_docs=CHOOSE_CLOUD_PROVIDER)}"
                 "\n\t❗️ [purple]local[/purple] requires Docker and Kubernetes running on your local machine. "
                 "[italic]Currently only available on Linux OS.[/italic]"
                 "\n\t❗️ [purple]existing[/purple] refers to an existing Kubernetes cluster that Nebari can be deployed on.\n"
             )
         )
         # try:
-        inputs.cloud_provider = questionary.select(
+        cloud_provider: str = questionary.select(
             "Where would you like to deploy your Nebari cluster?",
-            choices=enum_to_list(ProviderEnum),
+            choices=CLOUD_PROVIDER_FULL_NAME.keys(),
             qmark=qmark,
         ).unsafe_ask()
 
+        inputs.cloud_provider = CLOUD_PROVIDER_FULL_NAME.get(cloud_provider)
+
         if not disable_checks:
             check_cloud_provider_creds(
                 cloud_provider=inputs.cloud_provider,
                 disable_prompt=ctx.params.get("disable_prompt"),
             )
 
         # specific context needed when `check_project_name` is called
```

### Comparing `nebari-2024.3.3rc1/src/_nebari/subcommands/keycloak.py` & `nebari-2024.4.1rc1/src/_nebari/subcommands/keycloak.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/subcommands/render.py` & `nebari-2024.4.1rc1/src/_nebari/subcommands/render.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/subcommands/support.py` & `nebari-2024.4.1rc1/src/_nebari/subcommands/support.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/subcommands/upgrade.py` & `nebari-2024.4.1rc1/src/_nebari/subcommands/upgrade.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/_nebari/subcommands/validate.py` & `nebari-2024.4.1rc1/src/_nebari/subcommands/validate.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/nebari/hookspecs.py` & `nebari-2024.4.1rc1/src/nebari/hookspecs.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/nebari/plugins.py` & `nebari-2024.4.1rc1/src/nebari/plugins.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/src/nebari/schema.py` & `nebari-2024.4.1rc1/src/nebari/schema.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/tests/utils.py` & `nebari-2024.4.1rc1/tests/utils.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/tests/common/config_mod_utils.py` & `nebari-2024.4.1rc1/tests/common/config_mod_utils.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/tests/common/kube_api.py` & `nebari-2024.4.1rc1/tests/common/kube_api.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/tests/common/navigator.py` & `nebari-2024.4.1rc1/tests/common/navigator.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/tests/common/playwright_fixtures.py` & `nebari-2024.4.1rc1/tests/common/playwright_fixtures.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/tests/common/run_notebook.py` & `nebari-2024.4.1rc1/tests/common/run_notebook.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/tests/common/notebooks/test_notebook_output.ipynb` & `nebari-2024.4.1rc1/tests/common/notebooks/test_notebook_output.ipynb`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/tests/common/tests/test_notebook.py` & `nebari-2024.4.1rc1/tests/common/tests/test_notebook.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/tests/tests_deployment/test_dask_gateway.py` & `nebari-2024.4.1rc1/tests/tests_deployment/test_dask_gateway.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/tests/tests_deployment/test_grafana_api.py` & `nebari-2024.4.1rc1/tests/tests_deployment/test_grafana_api.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/tests/tests_deployment/test_jupyterhub_ssh.py` & `nebari-2024.4.1rc1/tests/tests_deployment/test_jupyterhub_ssh.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/tests/tests_deployment/test_loki_deployment.py` & `nebari-2024.4.1rc1/tests/tests_deployment/test_loki_deployment.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/tests/tests_deployment/utils.py` & `nebari-2024.4.1rc1/tests/tests_deployment/utils.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/tests/tests_deployment/assets/notebook/simple.ipynb` & `nebari-2024.4.1rc1/tests/tests_deployment/assets/notebook/simple.ipynb`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/tests/tests_e2e/package-lock.json` & `nebari-2024.4.1rc1/tests/tests_e2e/package-lock.json`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/tests/tests_e2e/cypress/integration/main.js` & `nebari-2024.4.1rc1/tests/tests_e2e/cypress/integration/main.js`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/tests/tests_e2e/cypress/notebooks/BasicTest.ipynb` & `nebari-2024.4.1rc1/tests/tests_e2e/cypress/notebooks/BasicTest.ipynb`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/tests/tests_e2e/cypress/plugins/index.js` & `nebari-2024.4.1rc1/tests/tests_e2e/cypress/plugins/index.js`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/tests/tests_e2e/cypress/support/index.js` & `nebari-2024.4.1rc1/tests/tests_e2e/cypress/support/index.js`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/tests/tests_e2e/playwright/README.md` & `nebari-2024.4.1rc1/tests/tests_e2e/playwright/README.md`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/tests/tests_e2e/playwright/test_playwright.py` & `nebari-2024.4.1rc1/tests/tests_e2e/playwright/test_playwright.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/tests/tests_integration/README.md` & `nebari-2024.4.1rc1/tests/tests_integration/README.md`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/tests/tests_integration/deployment_fixtures.py` & `nebari-2024.4.1rc1/tests/tests_integration/deployment_fixtures.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/tests/tests_integration/test_all_clouds.py` & `nebari-2024.4.1rc1/tests/tests_integration/test_all_clouds.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/tests/tests_integration/test_gpu.py` & `nebari-2024.4.1rc1/tests/tests_integration/test_gpu.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/tests/tests_integration/test_preemptible.py` & `nebari-2024.4.1rc1/tests/tests_integration/test_preemptible.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/tests/tests_unit/conftest.py` & `nebari-2024.4.1rc1/tests/tests_unit/conftest.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/tests/tests_unit/test_cli.py` & `nebari-2024.4.1rc1/tests/tests_unit/test_cli.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/tests/tests_unit/test_cli_deploy.py` & `nebari-2024.4.1rc1/tests/tests_unit/test_cli_deploy.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/tests/tests_unit/test_cli_dev.py` & `nebari-2024.4.1rc1/tests/tests_unit/test_cli_dev.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/tests/tests_unit/test_cli_init.py` & `nebari-2024.4.1rc1/tests/tests_unit/test_cli_init.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/tests/tests_unit/test_cli_init_repository.py` & `nebari-2024.4.1rc1/tests/tests_unit/test_cli_init_repository.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/tests/tests_unit/test_cli_keycloak.py` & `nebari-2024.4.1rc1/tests/tests_unit/test_cli_keycloak.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/tests/tests_unit/test_cli_support.py` & `nebari-2024.4.1rc1/tests/tests_unit/test_cli_support.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/tests/tests_unit/test_cli_upgrade.py` & `nebari-2024.4.1rc1/tests/tests_unit/test_cli_upgrade.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/tests/tests_unit/test_cli_validate.py` & `nebari-2024.4.1rc1/tests/tests_unit/test_cli_validate.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/tests/tests_unit/test_commons.py` & `nebari-2024.4.1rc1/tests/tests_unit/test_commons.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/tests/tests_unit/test_config.py` & `nebari-2024.4.1rc1/tests/tests_unit/test_config.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/tests/tests_unit/test_dependencies.py` & `nebari-2024.4.1rc1/tests/tests_unit/test_dependencies.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/tests/tests_unit/test_init.py` & `nebari-2024.4.1rc1/tests/tests_unit/test_init.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/tests/tests_unit/test_provider.py` & `nebari-2024.4.1rc1/tests/tests_unit/test_provider.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/tests/tests_unit/test_render.py` & `nebari-2024.4.1rc1/tests/tests_unit/test_render.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import os
 
 from _nebari.stages.bootstrap import CiEnum
-from nebari import schema
 from nebari.plugins import nebari_plugin_manager
 
 
 def test_render_config(nebari_render):
     output_directory, config_filename = nebari_render
     config = nebari_plugin_manager.read_config(config_filename)
     assert {"nebari-config.yaml", "stages", ".gitignore"} <= set(
@@ -18,24 +17,18 @@
         "05-kubernetes-keycloak",
         "08-nebari-tf-extensions",
         "06-kubernetes-keycloak-configuration",
         "04-kubernetes-ingress",
         "03-kubernetes-initialize",
     }.issubset(os.listdir(output_directory / "stages"))
 
-    if config.provider == schema.ProviderEnum.do:
-        assert (output_directory / "stages" / "01-terraform-state/do").is_dir()
-        assert (output_directory / "stages" / "02-infrastructure/do").is_dir()
-    elif config.provider == schema.ProviderEnum.aws:
-        assert (output_directory / "stages" / "01-terraform-state/aws").is_dir()
-        assert (output_directory / "stages" / "02-infrastructure/aws").is_dir()
-    elif config.provider == schema.ProviderEnum.gcp:
-        assert (output_directory / "stages" / "01-terraform-state/gcp").is_dir()
-        assert (output_directory / "stages" / "02-infrastructure/gcp").is_dir()
-    elif config.provider == schema.ProviderEnum.azure:
-        assert (output_directory / "stages" / "01-terraform-state/azure").is_dir()
-        assert (output_directory / "stages" / "02-infrastructure/azure").is_dir()
+    assert (
+        output_directory / "stages" / f"01-terraform-state/{config.provider.value}"
+    ).is_dir()
+    assert (
+        output_directory / "stages" / f"02-infrastructure/{config.provider.value}"
+    ).is_dir()
 
     if config.ci_cd.type == CiEnum.github_actions:
         assert (output_directory / ".github/workflows/").is_dir()
     elif config.ci_cd.type == CiEnum.gitlab_ci:
         assert (output_directory / ".gitlab-ci.yml").is_file()
```

### Comparing `nebari-2024.3.3rc1/tests/tests_unit/test_schema.py` & `nebari-2024.4.1rc1/tests/tests_unit/test_schema.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/tests/tests_unit/test_upgrade.py` & `nebari-2024.4.1rc1/tests/tests_unit/test_upgrade.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/tests/tests_unit/utils.py` & `nebari-2024.4.1rc1/tests/tests_unit/utils.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/tests/tests_unit/cli_validate/aws.happy.yaml` & `nebari-2024.4.1rc1/tests/tests_unit/cli_validate/aws.happy.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/tests/tests_unit/cli_validate/azure.happy.yaml` & `nebari-2024.4.1rc1/tests/tests_unit/cli_validate/azure.happy.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/tests/tests_unit/cli_validate/do.happy.yaml` & `nebari-2024.4.1rc1/tests/tests_unit/cli_validate/do.happy.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/tests/tests_unit/cli_validate/gcp.happy.yaml` & `nebari-2024.4.1rc1/tests/tests_unit/cli_validate/gcp.happy.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/tests/tests_unit/cli_validate/local.happy.yaml` & `nebari-2024.4.1rc1/tests/tests_unit/cli_validate/local.happy.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/tests/tests_unit/qhub-config-yaml-files-for-upgrade/qhub-config-do-310-customauth.yaml` & `nebari-2024.4.1rc1/tests/tests_unit/qhub-config-yaml-files-for-upgrade/qhub-config-do-310-customauth.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -41,18 +41,14 @@
     logo: /hub/custom/images/jupyter_nebari_logo.svg
     primary_color: '#4f4173'
     secondary_color: '#957da6'
     accent_color: '#32C574'
     text_color: '#111111'
     h1_color: '#652e8e'
     h2_color: '#652e8e'
-# cdsdashboards:
-#   enabled: true
-#   cds_hide_user_named_servers: true
-#   cds_hide_user_dashboard_servers: false
 terraform_state:
   type: remote
 namespace: dev
 digital_ocean:
   region: nyc3
   kubernetes_version: 1.21.5-do.0
   node_groups:
@@ -129,8 +125,7 @@
     - param
     - python-graphviz
     - matplotlib >=3.3.4
     - panel >=0.10.3
     - voila >=0.2.7
     - streamlit >=0.76
     - dash >=1.19
-    - cdsdashboards-singleuser >=0.5.6
```

#### html2text {}

```diff
@@ -10,30 +10,29 @@
 jupyterhub: hub_title: Nebari - do-pytest hub_subtitle: Autoscaling Compute
 Environment on Digital Ocean welcome: Welcome to do.nebari.dev. It is
 maintained by _Q_u_a_n_s_i_g_h_t_ _s_t_a_f_f. The hub's configuration is stored in a github
 repository based on _h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_Q_u_a_n_s_i_g_h_t_/_n_e_b_a_r_i_/. To provide feedback
 and report any technical problems, please use the _g_i_t_h_u_b_ _i_s_s_u_e_ _t_r_a_c_k_e_r. logo: /
 hub/custom/images/jupyter_nebari_logo.svg primary_color: '#4f4173'
 secondary_color: '#957da6' accent_color: '#32C574' text_color: '#111111'
-h1_color: '#652e8e' h2_color: '#652e8e' # cdsdashboards: # enabled: true #
-cds_hide_user_named_servers: true # cds_hide_user_dashboard_servers: false
-terraform_state: type: remote namespace: dev digital_ocean: region: nyc3
-kubernetes_version: 1.21.5-do.0 node_groups: general: instance: s-2vcpu-4gb
-min_nodes: 1 max_nodes: 1 user: instance: g-2vcpu-8gb min_nodes: 1 max_nodes: 5
-worker: instance: g-2vcpu-8gb min_nodes: 1 max_nodes: 5 profiles: jupyterlab: -
-display_name: Small Instance description: Stable environment with 1 cpu / 4 GB
-ram default: true kubespawner_override: cpu_limit: 1 cpu_guarantee: 0.75
-mem_limit: 4G mem_guarantee: 2.5G image: quansight/nebari-jupyterlab:v0.3.10 -
-display_name: Medium Instance description: Stable environment with 2 cpu / 8 GB
-ram kubespawner_override: cpu_limit: 2 cpu_guarantee: 1.5 mem_limit: 8G
+h1_color: '#652e8e' h2_color: '#652e8e' terraform_state: type: remote
+namespace: dev digital_ocean: region: nyc3 kubernetes_version: 1.21.5-do.0
+node_groups: general: instance: s-2vcpu-4gb min_nodes: 1 max_nodes: 1 user:
+instance: g-2vcpu-8gb min_nodes: 1 max_nodes: 5 worker: instance: g-2vcpu-8gb
+min_nodes: 1 max_nodes: 5 profiles: jupyterlab: - display_name: Small Instance
+description: Stable environment with 1 cpu / 4 GB ram default: true
+kubespawner_override: cpu_limit: 1 cpu_guarantee: 0.75 mem_limit: 4G
+mem_guarantee: 2.5G image: quansight/nebari-jupyterlab:v0.3.10 - display_name:
+Medium Instance description: Stable environment with 2 cpu / 8 GB ram
+kubespawner_override: cpu_limit: 2 cpu_guarantee: 1.5 mem_limit: 8G
 mem_guarantee: 5G image: quansight/nebari-jupyterlab:v0.3.10 dask_worker: Small
 Worker: worker_cores_limit: 1 worker_cores: 0.75 worker_memory_limit: 4G
 worker_memory: 2.5G worker_threads: 1 image: quansight/nebari-dask-worker:
 v0.3.10 Medium Worker: worker_cores_limit: 2 worker_cores: 1.5
 worker_memory_limit: 8G worker_memory: 5G worker_threads: 2 image: quansight/
 nebari-dask-worker:v0.3.10 environments: environment-dask.yaml: name: dask
 channels: - conda-forge dependencies: - python - ipykernel - ipywidgets -
 python-graphviz - dask ==2.30.0 - distributed ==2.30.1 - dask-gateway ==0.9.0 -
 numpy - numba - pandas environment-dashboard.yaml: name: dashboard channels: -
 conda-forge dependencies: - python - ipykernel - ipywidgets >=7.6 - param -
 python-graphviz - matplotlib >=3.3.4 - panel >=0.10.3 - voila >=0.2.7 -
-streamlit >=0.76 - dash >=1.19 - cdsdashboards-singleuser >=0.5.6
+streamlit >=0.76 - dash >=1.19
```

### Comparing `nebari-2024.3.3rc1/tests/tests_unit/qhub-config-yaml-files-for-upgrade/qhub-config-do-310.yaml` & `nebari-2024.4.1rc1/tests/tests_unit/qhub-config-yaml-files-for-upgrade/qhub-config-do-310.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -38,18 +38,14 @@
     logo: /hub/custom/images/jupyter_nebari_logo.svg
     primary_color: '#4f4173'
     secondary_color: '#957da6'
     accent_color: '#32C574'
     text_color: '#111111'
     h1_color: '#652e8e'
     h2_color: '#652e8e'
-# cdsdashboards:
-#  enabled: true
-#  cds_hide_user_named_servers: true
-#  cds_hide_user_dashboard_servers: false
 terraform_state:
   type: remote
 namespace: dev
 digital_ocean:
   region: nyc3
   kubernetes_version: 1.21.5-do.0
   node_groups:
@@ -126,8 +122,7 @@
     - param
     - python-graphviz
     - matplotlib >=3.3.4
     - panel >=0.10.3
     - voila >=0.2.7
     - streamlit >=0.76
     - dash >=1.19
-    - cdsdashboards-singleuser >=0.5.6
```

#### html2text {}

```diff
@@ -9,30 +9,29 @@
 jupyterhub: hub_title: Nebari - do-pytest hub_subtitle: Autoscaling Compute
 Environment on Digital Ocean welcome: Welcome to do.nebari.dev. It is
 maintained by _Q_u_a_n_s_i_g_h_t_ _s_t_a_f_f. The hub's configuration is stored in a github
 repository based on _h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_Q_u_a_n_s_i_g_h_t_/_n_e_b_a_r_i_/. To provide feedback
 and report any technical problems, please use the _g_i_t_h_u_b_ _i_s_s_u_e_ _t_r_a_c_k_e_r. logo: /
 hub/custom/images/jupyter_nebari_logo.svg primary_color: '#4f4173'
 secondary_color: '#957da6' accent_color: '#32C574' text_color: '#111111'
-h1_color: '#652e8e' h2_color: '#652e8e' # cdsdashboards: # enabled: true #
-cds_hide_user_named_servers: true # cds_hide_user_dashboard_servers: false
-terraform_state: type: remote namespace: dev digital_ocean: region: nyc3
-kubernetes_version: 1.21.5-do.0 node_groups: general: instance: s-2vcpu-4gb
-min_nodes: 1 max_nodes: 1 user: instance: g-2vcpu-8gb min_nodes: 1 max_nodes: 5
-worker: instance: g-2vcpu-8gb min_nodes: 1 max_nodes: 5 profiles: jupyterlab: -
-display_name: Small Instance description: Stable environment with 1 cpu / 4 GB
-ram default: true kubespawner_override: cpu_limit: 1 cpu_guarantee: 0.75
-mem_limit: 4G mem_guarantee: 2.5G image: quansight/nebari-jupyterlab:v0.3.10 -
-display_name: Medium Instance description: Stable environment with 2 cpu / 8 GB
-ram kubespawner_override: cpu_limit: 2 cpu_guarantee: 1.5 mem_limit: 8G
+h1_color: '#652e8e' h2_color: '#652e8e' terraform_state: type: remote
+namespace: dev digital_ocean: region: nyc3 kubernetes_version: 1.21.5-do.0
+node_groups: general: instance: s-2vcpu-4gb min_nodes: 1 max_nodes: 1 user:
+instance: g-2vcpu-8gb min_nodes: 1 max_nodes: 5 worker: instance: g-2vcpu-8gb
+min_nodes: 1 max_nodes: 5 profiles: jupyterlab: - display_name: Small Instance
+description: Stable environment with 1 cpu / 4 GB ram default: true
+kubespawner_override: cpu_limit: 1 cpu_guarantee: 0.75 mem_limit: 4G
+mem_guarantee: 2.5G image: quansight/nebari-jupyterlab:v0.3.10 - display_name:
+Medium Instance description: Stable environment with 2 cpu / 8 GB ram
+kubespawner_override: cpu_limit: 2 cpu_guarantee: 1.5 mem_limit: 8G
 mem_guarantee: 5G image: quansight/nebari-jupyterlab:v0.3.10 dask_worker: Small
 Worker: worker_cores_limit: 1 worker_cores: 0.75 worker_memory_limit: 4G
 worker_memory: 2.5G worker_threads: 1 image: quansight/nebari-dask-worker:
 v0.3.10 Medium Worker: worker_cores_limit: 2 worker_cores: 1.5
 worker_memory_limit: 8G worker_memory: 5G worker_threads: 2 image: quansight/
 nebari-dask-worker:v0.3.10 environments: environment-dask.yaml: name: dask
 channels: - conda-forge dependencies: - python - ipykernel - ipywidgets -
 python-graphviz - dask ==2.30.0 - distributed ==2.30.1 - dask-gateway ==0.9.0 -
 numpy - numba - pandas environment-dashboard.yaml: name: dashboard channels: -
 conda-forge dependencies: - python - ipykernel - ipywidgets >=7.6 - param -
 python-graphviz - matplotlib >=3.3.4 - panel >=0.10.3 - voila >=0.2.7 -
-streamlit >=0.76 - dash >=1.19 - cdsdashboards-singleuser >=0.5.6
+streamlit >=0.76 - dash >=1.19
```

### Comparing `nebari-2024.3.3rc1/.gitignore` & `nebari-2024.4.1rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/LICENSE` & `nebari-2024.4.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/README.md` & `nebari-2024.4.1rc1/README.md`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/pyproject.toml` & `nebari-2024.4.1rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nebari-2024.3.3rc1/PKG-INFO` & `nebari-2024.4.1rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: nebari
-Version: 2024.3.3rc1
+Version: 2024.4.1rc1
 Summary: A Jupyter and Dask-powered open source data science platform.
 Project-URL: Documentation, https://www.nebari.dev/docs
 Project-URL: Source, https://github.com/nebari-dev/nebari
 Author-email: Nebari development team <internal-it@quansight.com>
 License-Expression: BSD-3-Clause
 License-File: LICENSE
 Keywords: aws,azure,dask,do,gcp,jupyter,nebari
```

