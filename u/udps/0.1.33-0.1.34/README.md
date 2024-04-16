# Comparing `tmp/udps-0.1.33.tar.gz` & `tmp/udps-0.1.34.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "udps-0.1.33.tar", max compression
+gzip compressed data, was "udps-0.1.34.tar", max compression
```

## Comparing `udps-0.1.33.tar` & `udps-0.1.34.tar`

### file list

```diff
@@ -1,259 +1,259 @@
--rw-r--r--   0        0        0    11357 2024-03-19 10:07:44.426944 udps-0.1.33/LICENSE
--rw-r--r--   0        0        0     2471 2024-03-19 10:07:44.426944 udps-0.1.33/README.md
--rw-r--r--   0        0        0     3122 2024-03-19 10:07:44.426944 udps-0.1.33/pyproject.toml
--rw-r--r--   0        0        0       44 2024-03-19 10:07:44.426944 udps-0.1.33/tests/__init__.py
--rw-r--r--   0        0        0        0 2024-03-19 10:07:44.426944 udps-0.1.33/tests/mocks/__init__.py
--rw-r--r--   0        0        0      721 2024-03-19 10:07:44.426944 udps-0.1.33/tests/mocks/mock_writers.py
--rw-r--r--   0        0        0     1028 2024-03-19 10:07:44.426944 udps-0.1.33/tests/test_authz_analyzer.py
--rw-r--r--   0        0        0     6550 2024-03-19 10:07:44.426944 udps-0.1.33/tests/test_cli.py
--rw-r--r--   0        0        0        0 2024-03-19 10:07:44.426944 udps-0.1.33/tests/test_writers/__init__.py
--rw-r--r--   0        0        0     1403 2024-03-19 10:07:44.426944 udps-0.1.33/tests/test_writers/test_csv_writer.py
--rw-r--r--   0        0        0      953 2024-03-19 10:07:44.426944 udps-0.1.33/tests/test_writers/test_multijson_writer.py
--rw-r--r--   0        0        0        0 2024-03-19 10:07:44.426944 udps-0.1.33/tests/tests_datastores/__init__.py
--rw-r--r--   0        0        0        1 2024-03-19 10:07:44.426944 udps-0.1.33/tests/tests_datastores/aws/__init__.py
--rw-r--r--   0        0        0        0 2024-03-19 10:07:44.426944 udps-0.1.33/tests/tests_datastores/aws/aws_ptrp/__init__.py
--rw-r--r--   0        0        0    14110 2024-03-19 10:07:44.426944 udps-0.1.33/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/action/action_resolving_assume_role.json
--rw-r--r--   0        0        0    11644 2024-03-19 10:07:44.426944 udps-0.1.33/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/action/action_resolving_federated_user.json
--rw-r--r--   0        0        0    14917 2024-03-19 10:07:44.426944 udps-0.1.33/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/action/action_resolving_s3.json
--rw-r--r--   0        0        0     9884 2024-03-19 10:07:44.426944 udps-0.1.33/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/action/assume_role_actions_for_principal_type.json
--rw-r--r--   0        0        0    20662 2024-03-19 10:07:44.426944 udps-0.1.33/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/deny_with_condition/deny_with_condition_on_assume_role.json
--rw-r--r--   0        0        0    31812 2024-03-19 10:07:44.426944 udps-0.1.33/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/deny_with_condition/deny_with_condition_on_s3_bucket.json
--rw-r--r--   0        0        0    18235 2024-03-19 10:07:44.426944 udps-0.1.33/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/federated_user/federated_user_cross_account.json
--rw-r--r--   0        0        0    17618 2024-03-19 10:07:44.426944 udps-0.1.33/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/federated_user/iam_user_to_federated_user.json
--rw-r--r--   0        0        0     7529 2024-03-19 10:07:44.426944 udps-0.1.33/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_groups/iam_user_with_2_groups_includng_allow_and_deny.json
--rw-r--r--   0        0        0     7744 2024-03-19 10:07:44.426944 udps-0.1.33/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_groups/iam_user_with_group_and_attached_policy.json
--rw-r--r--   0        0        0     4073 2024-03-19 10:07:44.426944 udps-0.1.33/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_groups/iam_user_with_group_simple_policy.json
--rw-r--r--   0        0        0    24204 2024-03-19 10:07:44.426944 udps-0.1.33/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_identity_center/iam_identity_center_with_users_and_groups.json
--rw-r--r--   0        0        0    20163 2024-03-19 10:07:44.426944 udps-0.1.33/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_roles/assume_role_cross_account.json
--rw-r--r--   0        0        0    13494 2024-03-19 10:07:44.426944 udps-0.1.33/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_roles/assume_role_to_role.json
--rw-r--r--   0        0        0     8446 2024-03-19 10:07:44.426944 udps-0.1.33/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_roles/assume_role_via_resourve_based.json
--rw-r--r--   0        0        0    16466 2024-03-19 10:07:44.426944 udps-0.1.33/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_roles/simple_assume_role.json
--rw-r--r--   0        0        0    16126 2024-03-19 10:07:44.426944 udps-0.1.33/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_roles/valid_assume_action.json
--rw-r--r--   0        0        0    14831 2024-03-19 10:07:44.426944 udps-0.1.33/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_user_to_s3_bucket/iam_user_with_attached_policy_and_deny.json
--rw-r--r--   0        0        0     3066 2024-03-19 10:07:44.426944 udps-0.1.33/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_user_to_s3_bucket/iam_user_with_inline_policy.json
--rw-r--r--   0        0        0     5550 2024-03-19 10:07:44.426944 udps-0.1.33/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_user_to_s3_bucket/iam_user_with_inline_policy_and_deny.json
--rw-r--r--   0        0        0     5906 2024-03-19 10:07:44.426944 udps-0.1.33/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_user_to_s3_bucket/iam_user_with_inline_policy_and_resource_based.json
--rw-r--r--   0        0        0     4446 2024-03-19 10:07:44.426944 udps-0.1.33/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_user_to_s3_bucket/iam_user_with_inline_policy_multi_stmts.json
--rw-r--r--   0        0        0     8937 2024-03-19 10:07:44.426944 udps-0.1.33/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/multi_iam_users_to_multi_s3_buckets/iam_users_to_s3_cross_account_via_resource_based.json
--rw-r--r--   0        0        0    20162 2024-03-19 10:07:44.426944 udps-0.1.33/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/multi_iam_users_to_multi_s3_buckets/multi_iam_users_to_multi_s3_buckets.json
--rw-r--r--   0        0        0    10324 2024-03-19 10:07:44.426944 udps-0.1.33/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/assume_role_with_not_resource.json
--rw-r--r--   0        0        0     6886 2024-03-19 10:07:44.426944 udps-0.1.33/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/federated_users_with_not_resource.json
--rw-r--r--   0        0        0    23422 2024-03-19 10:07:44.426944 udps-0.1.33/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_combinations_in_both_allow_and_deny.json
--rw-r--r--   0        0        0     2358 2024-03-19 10:07:44.426944 udps-0.1.33/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_in_all_allow.json
--rw-r--r--   0        0        0     7124 2024-03-19 10:07:44.426944 udps-0.1.33/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_in_all_deny.json
--rw-r--r--   0        0        0     4549 2024-03-19 10:07:44.426944 udps-0.1.33/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_including_wildcard_object_regex_allow.json
--rw-r--r--   0        0        0     5215 2024-03-19 10:07:44.426944 udps-0.1.33/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_including_wildcard_object_regex_deny.json
--rw-r--r--   0        0        0     5987 2024-03-19 10:07:44.426944 udps-0.1.33/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_multiple_wildcard_regexes.json
--rw-r--r--   0        0        0     5862 2024-03-19 10:07:44.426944 udps-0.1.33/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_on_no_valid_resource_arn_allow.json
--rw-r--r--   0        0        0     3396 2024-03-19 10:07:44.426944 udps-0.1.33/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_on_no_valid_resource_arn_deny.json
--rw-r--r--   0        0        0     2298 2024-03-19 10:07:44.426944 udps-0.1.33/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_action/iam_user_allowed_no_action.json
--rw-r--r--   0        0        0     5264 2024-03-19 10:07:44.426944 udps-0.1.33/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_action/iam_user_allowed_no_action_s3_complement.json
--rw-r--r--   0        0        0     4596 2024-03-19 10:07:44.426944 udps-0.1.33/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_action/iam_user_with_multiple_actions_in_no_action_resource.json
--rw-r--r--   0        0        0     3653 2024-03-19 10:07:44.426944 udps-0.1.33/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_action/iam_user_with_resource_no_action_simple.json
--rw-r--r--   0        0        0     4392 2024-03-19 10:07:44.426944 udps-0.1.33/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_action/iam_user_with_resource_no_action_wildcard_action_set.json
--rw-r--r--   0        0        0    26158 2024-03-19 10:07:44.426944 udps-0.1.33/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_principal/iam_users_roles_and_federated_with_deny_not_principal_single_account.json
--rw-r--r--   0        0        0    10097 2024-03-19 10:07:44.426944 udps-0.1.33/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_principal/iam_users_with_deny_not_principal_cross_accounts.json
--rw-r--r--   0        0        0     8580 2024-03-19 10:07:44.426944 udps-0.1.33/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/principal/irrelevant_principal_types.json
--rw-r--r--   0        0        0    33775 2024-03-19 10:07:44.426944 udps-0.1.33/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/principal/principal_resolving_via_resource_based.json
--rw-r--r--   0        0        0    16439 2024-03-19 10:07:44.430944 udps-0.1.33/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/resource/resouce_resolving_assume_role.json
--rw-r--r--   0        0        0    13955 2024-03-19 10:07:44.430944 udps-0.1.33/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/resource/resouce_resolving_federated_user.json
--rw-r--r--   0        0        0    18162 2024-03-19 10:07:44.430944 udps-0.1.33/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/resource/resouce_resolving_s3.json
--rw-r--r--   0        0        0     3040 2024-03-19 10:07:44.430944 udps-0.1.33/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/s3_resource_regex/deny_and_allow_default.json
--rw-r--r--   0        0        0     5254 2024-03-19 10:07:44.430944 udps-0.1.33/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/s3_resource_regex/deny_and_allow_on_object_multi_stmts.json
--rw-r--r--   0        0        0     3569 2024-03-19 10:07:44.430944 udps-0.1.33/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/s3_resource_regex/deny_and_allow_with_one_resource_in_deny_that_is_a_subgroup_of_all_in_allow.json
--rw-r--r--   0        0        0     4436 2024-03-19 10:07:44.430944 udps-0.1.33/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/s3_resource_regex/deny_on_object_and_allow_bucket.json
--rw-r--r--   0        0        0    14441 2024-03-19 10:07:44.430944 udps-0.1.33/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/s3_resource_regex/valid_actions_objects_and_actions_resources.json
--rw-r--r--   0        0        0     3581 2024-03-19 10:07:44.430944 udps-0.1.33/tests/tests_datastores/aws/aws_ptrp/test_create_session_with_assume_role.py
--rw-r--r--   0        0        0     4890 2024-03-19 10:07:44.430944 udps-0.1.33/tests/tests_datastores/aws/aws_ptrp/test_resolve_permissions.py
--rw-r--r--   0        0        0     4859 2024-03-19 10:07:44.430944 udps-0.1.33/tests/tests_datastores/aws/aws_ptrp/test_satori_dev_account_ptrp.py
--rw-r--r--   0        0        0        0 2024-03-19 10:07:44.430944 udps-0.1.33/tests/tests_datastores/aws/aws_ptrp/utils/__init__.py
--rw-r--r--   0        0        0     2831 2024-03-19 10:07:44.430944 udps-0.1.33/tests/tests_datastores/aws/aws_ptrp/utils/aws_ptrp_load_from_dict.py
--rw-r--r--   0        0        0     1595 2024-03-19 10:07:44.430944 udps-0.1.33/tests/tests_datastores/aws/exporter_test_inputs/ptrp_line_basic_iam_user_and_policy_path.json
--rw-r--r--   0        0        0     3805 2024-03-19 10:07:44.430944 udps-0.1.33/tests/tests_datastores/aws/exporter_test_inputs/ptrp_line_iam_identity_center_user_and_group.json
--rw-r--r--   0        0        0     2597 2024-03-19 10:07:44.430944 udps-0.1.33/tests/tests_datastores/aws/exporter_test_inputs/ptrp_line_multiple_roles_in_path_and_all_principals.json
--rw-r--r--   0        0        0     2321 2024-03-19 10:07:44.430944 udps-0.1.33/tests/tests_datastores/aws/exporter_test_inputs/ptrp_line_with_federated_user.json
--rw-r--r--   0        0        0     4018 2024-03-19 10:07:44.430944 udps-0.1.33/tests/tests_datastores/aws/exporter_test_inputs/ptrp_line_with_iam_group_and_notes.json
--rw-r--r--   0        0        0     5298 2024-03-19 10:07:44.430944 udps-0.1.33/tests/tests_datastores/aws/exporter_test_inputs/ptrp_line_with_notes.json
--rw-r--r--   0        0        0     1579 2024-03-19 10:07:44.430944 udps-0.1.33/tests/tests_datastores/aws/test_exporter.py
--rw-r--r--   0        0        0        0 2024-03-19 10:07:44.430944 udps-0.1.33/tests/tests_datastores/aws/utils/__init__.py
--rw-r--r--   0        0        0     1731 2024-03-19 10:07:44.430944 udps-0.1.33/tests/tests_datastores/aws/utils/test_aws_regex_full_subset.py
--rw-r--r--   0        0        0        0 2024-03-19 10:07:44.430944 udps-0.1.33/tests/tests_datastores/bigquery/__init__.py
--rw-r--r--   0        0        0     5596 2024-03-19 10:07:44.430944 udps-0.1.33/tests/tests_datastores/bigquery/generate_authz_entry.py
--rw-r--r--   0        0        0     7185 2024-03-19 10:07:44.430944 udps-0.1.33/tests/tests_datastores/bigquery/mocks.py
--rw-r--r--   0        0        0    15539 2024-03-19 10:07:44.430944 udps-0.1.33/tests/tests_datastores/bigquery/test_bigquery.py
--rw-r--r--   0        0        0        0 2024-03-19 10:07:44.430944 udps-0.1.33/tests/tests_datastores/databricks/__init__.py
--rw-r--r--   0        0        0    17596 2024-03-19 10:07:44.430944 udps-0.1.33/tests/tests_datastores/databricks/generate_authz_entry.py
--rw-r--r--   0        0        0     9136 2024-03-19 10:07:44.430944 udps-0.1.33/tests/tests_datastores/databricks/mocks.py
--rw-r--r--   0        0        0    13149 2024-03-19 10:07:44.430944 udps-0.1.33/tests/tests_datastores/databricks/test_analyzer.py
--rw-r--r--   0        0        0        0 2024-03-19 10:07:44.430944 udps-0.1.33/tests/tests_datastores/mongodb/__init__.py
--rw-r--r--   0        0        0     1809 2024-03-19 10:07:44.430944 udps-0.1.33/tests/tests_datastores/mongodb/test_atlas_build_custom_role_from_response.py
--rw-r--r--   0        0        0    14532 2024-03-19 10:07:44.430944 udps-0.1.33/tests/tests_datastores/mongodb/test_atlas_organization_users.py
--rw-r--r--   0        0        0     7391 2024-03-19 10:07:44.430944 udps-0.1.33/tests/tests_datastores/mongodb/test_mongodb.py
--rw-r--r--   0        0        0        0 2024-03-19 10:07:44.430944 udps-0.1.33/tests/tests_datastores/postgres/__init__.py
--rw-r--r--   0        0        0        0 2024-03-19 10:07:44.430944 udps-0.1.33/tests/tests_datastores/postgres/mocks/__init__.py
--rw-r--r--   0        0        0     1195 2024-03-19 10:07:44.430944 udps-0.1.33/tests/tests_datastores/postgres/mocks/postgres_mock_connector.py
--rw-r--r--   0        0        0    12910 2024-03-19 10:07:44.430944 udps-0.1.33/tests/tests_datastores/postgres/test_postgress_analyzer.py
--rw-r--r--   0        0        0        0 2024-03-19 10:07:44.430944 udps-0.1.33/tests/tests_datastores/redshift/__init__.py
--rw-r--r--   0        0        0    12365 2024-03-19 10:07:44.430944 udps-0.1.33/tests/tests_datastores/redshift/test_redshift.py
--rw-r--r--   0        0        0        0 2024-03-19 10:07:44.430944 udps-0.1.33/tests/tests_datastores/snowflake/__init__.py
--rw-r--r--   0        0        0    19120 2024-03-19 10:07:44.430944 udps-0.1.33/tests/tests_datastores/snowflake/test_snowflake_analyzer.py
--rw-r--r--   0        0        0     1086 2024-03-19 10:07:44.430944 udps-0.1.33/universal_data_permissions_scanner/__init__.py
--rw-r--r--   0        0        0    11916 2024-03-19 10:07:44.430944 udps-0.1.33/universal_data_permissions_scanner/cli.py
--rw-r--r--   0        0        0        0 2024-03-19 10:07:44.430944 udps-0.1.33/universal_data_permissions_scanner/datastores/__init__.py
--rw-r--r--   0        0        0      626 2024-03-19 10:07:44.430944 udps-0.1.33/universal_data_permissions_scanner/datastores/aws/__init__.py
--rw-r--r--   0        0        0      113 2024-03-19 10:07:44.430944 udps-0.1.33/universal_data_permissions_scanner/datastores/aws/analyzer/__init__.py
--rw-r--r--   0        0        0     2912 2024-03-19 10:07:44.430944 udps-0.1.33/universal_data_permissions_scanner/datastores/aws/analyzer/analyzer.py
--rw-r--r--   0        0        0     7808 2024-03-19 10:07:44.430944 udps-0.1.33/universal_data_permissions_scanner/datastores/aws/analyzer/exporter.py
--rw-r--r--   0        0        0        0 2024-03-19 10:07:44.430944 udps-0.1.33/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/__init__.py
--rw-r--r--   0        0        0    13055 2024-03-19 10:07:44.430944 udps-0.1.33/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/analyzer.py
--rw-r--r--   0        0        0       90 2024-03-19 10:07:44.430944 udps-0.1.33/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/commands/all_databases.sql
--rw-r--r--   0        0        0      141 2024-03-19 10:07:44.430944 udps-0.1.33/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/commands/all_tables.sql
--rw-r--r--   0        0        0      111 2024-03-19 10:07:44.430944 udps-0.1.33/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/commands/datashare_consumers.sql
--rw-r--r--   0        0        0       14 2024-03-19 10:07:44.430944 udps-0.1.33/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/commands/datashare_desc.sql
--rw-r--r--   0        0        0      125 2024-03-19 10:07:44.430944 udps-0.1.33/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/commands/datashares.sql
--rw-r--r--   0        0        0      318 2024-03-19 10:07:44.430944 udps-0.1.33/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/commands/identities_pg_user.sql
--rw-r--r--   0        0        0      262 2024-03-19 10:07:44.430944 udps-0.1.33/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/commands/identities_privileges.sql
--rw-r--r--   0        0        0      307 2024-03-19 10:07:44.430944 udps-0.1.33/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/commands/identities_svv_role_grants.sql
--rw-r--r--   0        0        0      256 2024-03-19 10:07:44.430944 udps-0.1.33/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/commands/identities_svv_user_grants.sql
--rw-r--r--   0        0        0     5539 2024-03-19 10:07:44.430944 udps-0.1.33/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/exporter.py
--rw-r--r--   0        0        0     3524 2024-03-19 10:07:44.430944 udps-0.1.33/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/model.py
--rw-r--r--   0        0        0      660 2024-03-19 10:07:44.430944 udps-0.1.33/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/service.py
--rw-r--r--   0        0        0      120 2024-03-19 10:07:44.430944 udps-0.1.33/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/__init__.py
--rw-r--r--   0        0        0        0 2024-03-19 10:07:44.430944 udps-0.1.33/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/actions/__init__.py
--rw-r--r--   0        0        0     3041 2024-03-19 10:07:44.430944 udps-0.1.33/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/actions/actions_resolver.py
--rw-r--r--   0        0        0     2045 2024-03-19 10:07:44.430944 udps-0.1.33/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/actions/aws_actions.py
--rw-r--r--   0        0        0        0 2024-03-19 10:07:44.430944 udps-0.1.33/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/__init__.py
--rw-r--r--   0        0        0     5682 2024-03-19 10:07:44.430944 udps-0.1.33/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/iam_entities.py
--rw-r--r--   0        0        0     3505 2024-03-19 10:07:44.430944 udps-0.1.33/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/iam_groups.py
--rw-r--r--   0        0        0     2481 2024-03-19 10:07:44.430944 udps-0.1.33/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/iam_policies.py
--rw-r--r--   0        0        0     6201 2024-03-19 10:07:44.430944 udps-0.1.33/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/iam_roles.py
--rw-r--r--   0        0        0     3963 2024-03-19 10:07:44.430944 udps-0.1.33/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/iam_users.py
--rw-r--r--   0        0        0      254 2024-03-19 10:07:44.430944 udps-0.1.33/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/policy/__init__.py
--rw-r--r--   0        0        0       87 2024-03-19 10:07:44.430944 udps-0.1.33/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/policy/effect.py
--rw-r--r--   0        0        0      263 2024-03-19 10:07:44.430944 udps-0.1.33/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/policy/group_policy.py
--rw-r--r--   0        0        0      415 2024-03-19 10:07:44.430944 udps-0.1.33/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/policy/policy.py
--rw-r--r--   0        0        0     6232 2024-03-19 10:07:44.430944 udps-0.1.33/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/policy/policy_document.py
--rw-r--r--   0        0        0    10500 2024-03-19 10:07:44.430944 udps-0.1.33/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/policy/policy_document_resolver.py
--rw-r--r--   0        0        0      373 2024-03-19 10:07:44.430944 udps-0.1.33/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/policy/policy_document_utils.py
--rw-r--r--   0        0        0      261 2024-03-19 10:07:44.430944 udps-0.1.33/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/policy/user_policy.py
--rw-r--r--   0        0        0      263 2024-03-19 10:07:44.430944 udps-0.1.33/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/public_block_access_config.py
--rw-r--r--   0        0        0        0 2024-03-19 10:07:44.430944 udps-0.1.33/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/role/__init__.py
--rw-r--r--   0        0        0      261 2024-03-19 10:07:44.430944 udps-0.1.33/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/role/role_policy.py
--rw-r--r--   0        0        0        0 2024-03-19 10:07:44.430944 udps-0.1.33/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam_identity_center/__init__.py
--rw-r--r--   0        0        0     5655 2024-03-19 10:07:44.430944 udps-0.1.33/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam_identity_center/iam_identity_center_entities.py
--rw-r--r--   0        0        0     1961 2024-03-19 10:07:44.430944 udps-0.1.33/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam_identity_center/iam_identity_center_groups.py
--rw-r--r--   0        0        0     1824 2024-03-19 10:07:44.430944 udps-0.1.33/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam_identity_center/iam_identity_center_users.py
--rw-r--r--   0        0        0     2502 2024-03-19 10:07:44.430944 udps-0.1.33/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam_identity_center/permission_sets.py
--rw-r--r--   0        0        0     1046 2024-03-19 10:07:44.430944 udps-0.1.33/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/logger.py
--rw-r--r--   0        0        0      263 2024-03-19 10:07:44.430944 udps-0.1.33/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/policy_evaluation/__init__.py
--rw-r--r--   0        0        0    18760 2024-03-19 10:07:44.430944 udps-0.1.33/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/policy_evaluation/policy_evaluation.py
--rw-r--r--   0        0        0      172 2024-03-19 10:07:44.430944 udps-0.1.33/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/principals/__init__.py
--rw-r--r--   0        0        0    12129 2024-03-19 10:07:44.430944 udps-0.1.33/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/principals/aws_principals.py
--rw-r--r--   0        0        0     1267 2024-03-19 10:07:44.430944 udps-0.1.33/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/principals/no_entity_principal.py
--rw-r--r--   0        0        0    12938 2024-03-19 10:07:44.430944 udps-0.1.33/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/principals/principal.py
--rw-r--r--   0        0        0     3787 2024-03-19 10:07:44.430944 udps-0.1.33/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/principals/principals_resolver.py
--rw-r--r--   0        0        0    10597 2024-03-19 10:07:44.430944 udps-0.1.33/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp.py
--rw-r--r--   0        0        0        0 2024-03-19 10:07:44.430944 udps-0.1.33/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_allowed_lines/__init__.py
--rw-r--r--   0        0        0    12040 2024-03-19 10:07:44.430944 udps-0.1.33/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_allowed_lines/allowed_line.py
--rw-r--r--   0        0        0     8007 2024-03-19 10:07:44.430944 udps-0.1.33/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_allowed_lines/allowed_line_node_notes.py
--rw-r--r--   0        0        0    15325 2024-03-19 10:07:44.430944 udps-0.1.33/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_allowed_lines/allowed_line_nodes_base.py
--rw-r--r--   0        0        0    26515 2024-03-19 10:07:44.430944 udps-0.1.33/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_allowed_lines/allowed_lines_resolver.py
--rw-r--r--   0        0        0     6471 2024-03-19 10:07:44.430944 udps-0.1.33/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_allowed_lines/allowed_lines_resolver_result.py
--rw-r--r--   0        0        0      513 2024-03-19 10:07:44.430944 udps-0.1.33/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_models/__init__.py
--rw-r--r--   0        0        0     8549 2024-03-19 10:07:44.430944 udps-0.1.33/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_models/ptrp_model.py
--rw-r--r--   0        0        0        0 2024-03-19 10:07:44.430944 udps-0.1.33/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/resources/__init__.py
--rw-r--r--   0        0        0     5233 2024-03-19 10:07:44.430944 udps-0.1.33/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/resources/account_resources.py
--rw-r--r--   0        0        0     4475 2024-03-19 10:07:44.430944 udps-0.1.33/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/resources/resources_resolver.py
--rw-r--r--   0        0        0     1644 2024-03-19 10:07:44.430944 udps-0.1.33/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/__init__.py
--rw-r--r--   0        0        0        0 2024-03-19 10:07:44.430944 udps-0.1.33/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/assume_role/__init__.py
--rw-r--r--   0        0        0     2904 2024-03-19 10:07:44.430944 udps-0.1.33/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/assume_role/assume_role_actions.py
--rw-r--r--   0        0        0     6157 2024-03-19 10:07:44.430944 udps-0.1.33/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/assume_role/assume_role_resources.py
--rw-r--r--   0        0        0     2185 2024-03-19 10:07:44.434944 udps-0.1.33/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/assume_role/assume_role_service.py
--rw-r--r--   0        0        0        0 2024-03-19 10:07:44.434944 udps-0.1.33/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/federated_user/__init__.py
--rw-r--r--   0        0        0     2146 2024-03-19 10:07:44.434944 udps-0.1.33/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/federated_user/federated_user_actions.py
--rw-r--r--   0        0        0     7452 2024-03-19 10:07:44.434944 udps-0.1.33/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/federated_user/federated_user_resources.py
--rw-r--r--   0        0        0     2289 2024-03-19 10:07:44.434944 udps-0.1.33/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/federated_user/federated_user_service.py
--rw-r--r--   0        0        0     2594 2024-03-19 10:07:44.434944 udps-0.1.33/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/resolved_stmt.py
--rw-r--r--   0        0        0        0 2024-03-19 10:07:44.434944 udps-0.1.33/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/s3/__init__.py
--rw-r--r--   0        0        0     3377 2024-03-19 10:07:44.434944 udps-0.1.33/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/s3/bucket.py
--rw-r--r--   0        0        0     1054 2024-03-19 10:07:44.434944 udps-0.1.33/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/s3/bucket_acl.py
--rw-r--r--   0        0        0    17632 2024-03-19 10:07:44.434944 udps-0.1.33/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/s3/s3_actions.py
--rw-r--r--   0        0        0     7561 2024-03-19 10:07:44.434944 udps-0.1.33/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/s3/s3_resources.py
--rw-r--r--   0        0        0     1894 2024-03-19 10:07:44.434944 udps-0.1.33/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/s3/s3_service.py
--rw-r--r--   0        0        0      398 2024-03-19 10:07:44.434944 udps-0.1.33/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/service_action_base.py
--rw-r--r--   0        0        0     1973 2024-03-19 10:07:44.434944 udps-0.1.33/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/service_action_type.py
--rw-r--r--   0        0        0     3041 2024-03-19 10:07:44.434944 udps-0.1.33/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/service_actions_resolver_base.py
--rw-r--r--   0        0        0      397 2024-03-19 10:07:44.434944 udps-0.1.33/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/service_base.py
--rw-r--r--   0        0        0      561 2024-03-19 10:07:44.434944 udps-0.1.33/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/service_resource_base.py
--rw-r--r--   0        0        0     2501 2024-03-19 10:07:44.434944 udps-0.1.33/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/service_resource_type.py
--rw-r--r--   0        0        0     9989 2024-03-19 10:07:44.434944 udps-0.1.33/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/service_resources_resolver_base.py
--rw-r--r--   0        0        0        0 2024-03-19 10:07:44.434944 udps-0.1.33/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/utils/__init__.py
--rw-r--r--   0        0        0      482 2024-03-19 10:07:44.434944 udps-0.1.33/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/utils/assume_role.py
--rw-r--r--   0        0        0      879 2024-03-19 10:07:44.434944 udps-0.1.33/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/utils/create_session.py
--rw-r--r--   0        0        0     1000 2024-03-19 10:07:44.434944 udps-0.1.33/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/utils/pagination.py
--rw-r--r--   0        0        0     2747 2024-03-19 10:07:44.434944 udps-0.1.33/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/utils/regex_subset.py
--rw-r--r--   0        0        0      178 2024-03-19 10:07:44.434944 udps-0.1.33/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/utils/serde.py
--rw-r--r--   0        0        0      131 2024-03-19 10:07:44.434944 udps-0.1.33/universal_data_permissions_scanner/datastores/bigquery/__init__.py
--rw-r--r--   0        0        0    11167 2024-03-19 10:07:44.434944 udps-0.1.33/universal_data_permissions_scanner/datastores/bigquery/analyzer.py
--rw-r--r--   0        0        0    12689 2024-03-19 10:07:44.434944 udps-0.1.33/universal_data_permissions_scanner/datastores/bigquery/policy_tree.py
--rw-r--r--   0        0        0     8010 2024-03-19 10:07:44.434944 udps-0.1.33/universal_data_permissions_scanner/datastores/bigquery/service.py
--rw-r--r--   0        0        0      138 2024-03-19 10:07:44.434944 udps-0.1.33/universal_data_permissions_scanner/datastores/databricks/__init__.py
--rw-r--r--   0        0        0     6461 2024-03-19 10:07:44.434944 udps-0.1.33/universal_data_permissions_scanner/datastores/databricks/analyzer.py
--rw-r--r--   0        0        0       53 2024-03-19 10:07:44.434944 udps-0.1.33/universal_data_permissions_scanner/datastores/databricks/exceptions.py
--rw-r--r--   0        0        0     8588 2024-03-19 10:07:44.434944 udps-0.1.33/universal_data_permissions_scanner/datastores/databricks/identities.py
--rw-r--r--   0        0        0     1331 2024-03-19 10:07:44.434944 udps-0.1.33/universal_data_permissions_scanner/datastores/databricks/model.py
--rw-r--r--   0        0        0    10803 2024-03-19 10:07:44.434944 udps-0.1.33/universal_data_permissions_scanner/datastores/databricks/policy_tree.py
--rw-r--r--   0        0        0      138 2024-03-19 10:07:44.434944 udps-0.1.33/universal_data_permissions_scanner/datastores/databricks/service/__init__.py
--rw-r--r--   0        0        0      138 2024-03-19 10:07:44.434944 udps-0.1.33/universal_data_permissions_scanner/datastores/databricks/service/authentication/__init__.py
--rw-r--r--   0        0        0      879 2024-03-19 10:07:44.434944 udps-0.1.33/universal_data_permissions_scanner/datastores/databricks/service/authentication/authentication.py
--rw-r--r--   0        0        0      110 2024-03-19 10:07:44.434944 udps-0.1.33/universal_data_permissions_scanner/datastores/databricks/service/authentication/basic.py
--rw-r--r--   0        0        0     1930 2024-03-19 10:07:44.434944 udps-0.1.33/universal_data_permissions_scanner/datastores/databricks/service/authentication/oauth.py
--rw-r--r--   0        0        0       48 2024-03-19 10:07:44.434944 udps-0.1.33/universal_data_permissions_scanner/datastores/databricks/service/exceptions.py
--rw-r--r--   0        0        0     2448 2024-03-19 10:07:44.434944 udps-0.1.33/universal_data_permissions_scanner/datastores/databricks/service/model.py
--rw-r--r--   0        0        0     4024 2024-03-19 10:07:44.434944 udps-0.1.33/universal_data_permissions_scanner/datastores/databricks/service/scim.py
--rw-r--r--   0        0        0        0 2024-03-19 10:07:44.434944 udps-0.1.33/universal_data_permissions_scanner/datastores/mongodb/__init__.py
--rw-r--r--   0        0        0    15596 2024-03-19 10:07:44.434944 udps-0.1.33/universal_data_permissions_scanner/datastores/mongodb/analyzer.py
--rw-r--r--   0        0        0        0 2024-03-19 10:07:44.434944 udps-0.1.33/universal_data_permissions_scanner/datastores/mongodb/atlas/__init__.py
--rw-r--r--   0        0        0    17520 2024-03-19 10:07:44.434944 udps-0.1.33/universal_data_permissions_scanner/datastores/mongodb/atlas/analyzer.py
--rw-r--r--   0        0        0      625 2024-03-19 10:07:44.434944 udps-0.1.33/universal_data_permissions_scanner/datastores/mongodb/atlas/exceptions.py
--rw-r--r--   0        0        0     7603 2024-03-19 10:07:44.434944 udps-0.1.33/universal_data_permissions_scanner/datastores/mongodb/atlas/model.py
--rw-r--r--   0        0        0     2527 2024-03-19 10:07:44.434944 udps-0.1.33/universal_data_permissions_scanner/datastores/mongodb/atlas/permission_resolvers.py
--rw-r--r--   0        0        0     6270 2024-03-19 10:07:44.434944 udps-0.1.33/universal_data_permissions_scanner/datastores/mongodb/atlas/service.py
--rw-r--r--   0        0        0     2394 2024-03-19 10:07:44.434944 udps-0.1.33/universal_data_permissions_scanner/datastores/mongodb/atlas/service_model.py
--rw-r--r--   0        0        0     2197 2024-03-19 10:07:44.434944 udps-0.1.33/universal_data_permissions_scanner/datastores/mongodb/model.py
--rw-r--r--   0        0        0     1553 2024-03-19 10:07:44.434944 udps-0.1.33/universal_data_permissions_scanner/datastores/mongodb/resolvers.py
--rw-r--r--   0        0        0     1480 2024-03-19 10:07:44.434944 udps-0.1.33/universal_data_permissions_scanner/datastores/mongodb/service.py
--rw-r--r--   0        0        0     1196 2024-03-19 10:07:44.434944 udps-0.1.33/universal_data_permissions_scanner/datastores/mongodb/service_model.py
--rw-r--r--   0        0        0        0 2024-03-19 10:07:44.434944 udps-0.1.33/universal_data_permissions_scanner/datastores/postgres/__init__.py
--rw-r--r--   0        0        0    10637 2024-03-19 10:07:44.434944 udps-0.1.33/universal_data_permissions_scanner/datastores/postgres/analyzer.py
--rw-r--r--   0        0        0       71 2024-03-19 10:07:44.434944 udps-0.1.33/universal_data_permissions_scanner/datastores/postgres/commands/all_databases.sql
--rw-r--r--   0        0        0      369 2024-03-19 10:07:44.434944 udps-0.1.33/universal_data_permissions_scanner/datastores/postgres/commands/all_tables.sql
--rw-r--r--   0        0        0      272 2024-03-19 10:07:44.434944 udps-0.1.33/universal_data_permissions_scanner/datastores/postgres/commands/roles.sql
--rw-r--r--   0        0        0      313 2024-03-19 10:07:44.434944 udps-0.1.33/universal_data_permissions_scanner/datastores/postgres/commands/roles_grants.sql
--rw-r--r--   0        0        0     2404 2024-03-19 10:07:44.434944 udps-0.1.33/universal_data_permissions_scanner/datastores/postgres/database_query_results.py
--rw-r--r--   0        0        0      822 2024-03-19 10:07:44.434944 udps-0.1.33/universal_data_permissions_scanner/datastores/postgres/deployment.py
--rw-r--r--   0        0        0     2687 2024-03-19 10:07:44.434944 udps-0.1.33/universal_data_permissions_scanner/datastores/postgres/exporter.py
--rw-r--r--   0        0        0     1891 2024-03-19 10:07:44.434944 udps-0.1.33/universal_data_permissions_scanner/datastores/postgres/model.py
--rw-r--r--   0        0        0        0 2024-03-19 10:07:44.434944 udps-0.1.33/universal_data_permissions_scanner/datastores/snowflake/__init__.py
--rw-r--r--   0        0        0    12492 2024-03-19 10:07:44.434944 udps-0.1.33/universal_data_permissions_scanner/datastores/snowflake/analyzer.py
--rw-r--r--   0        0        0      389 2024-03-19 10:07:44.434944 udps-0.1.33/universal_data_permissions_scanner/datastores/snowflake/commands/grants_roles.sql
--rw-r--r--   0        0        0       20 2024-03-19 10:07:44.434944 udps-0.1.33/universal_data_permissions_scanner/datastores/snowflake/commands/grants_to_share.sql
--rw-r--r--   0        0        0       11 2024-03-19 10:07:44.434944 udps-0.1.33/universal_data_permissions_scanner/datastores/snowflake/commands/shares.sql
--rw-r--r--   0        0        0      535 2024-03-19 10:07:44.434944 udps-0.1.33/universal_data_permissions_scanner/datastores/snowflake/commands/user_grants.sql
--rw-r--r--   0        0        0     5827 2024-03-19 10:07:44.434944 udps-0.1.33/universal_data_permissions_scanner/datastores/snowflake/exporter.py
--rw-r--r--   0        0        0     4685 2024-03-19 10:07:44.434944 udps-0.1.33/universal_data_permissions_scanner/datastores/snowflake/model.py
--rw-r--r--   0        0        0     1394 2024-03-19 10:07:44.434944 udps-0.1.33/universal_data_permissions_scanner/datastores/snowflake/service.py
--rw-r--r--   0        0        0        0 2024-03-19 10:07:44.434944 udps-0.1.33/universal_data_permissions_scanner/errors/__init__.py
--rw-r--r--   0        0        0       45 2024-03-19 10:07:44.434944 udps-0.1.33/universal_data_permissions_scanner/errors/failed_connection_errors.py
--rw-r--r--   0        0        0       58 2024-03-19 10:07:44.434944 udps-0.1.33/universal_data_permissions_scanner/errors/snowflake.py
--rw-r--r--   0        0        0     7625 2024-03-19 10:07:44.434944 udps-0.1.33/universal_data_permissions_scanner/main.py
--rw-r--r--   0        0        0      195 2024-03-19 10:07:44.434944 udps-0.1.33/universal_data_permissions_scanner/models/__init__.py
--rw-r--r--   0        0        0     7583 2024-03-19 10:07:44.434944 udps-0.1.33/universal_data_permissions_scanner/models/model.py
--rw-r--r--   0        0        0        0 2024-03-19 10:07:44.434944 udps-0.1.33/universal_data_permissions_scanner/utils/__init__.py
--rw-r--r--   0        0        0      651 2024-03-19 10:07:44.434944 udps-0.1.33/universal_data_permissions_scanner/utils/logger.py
--rw-r--r--   0        0        0      455 2024-03-19 10:07:44.434944 udps-0.1.33/universal_data_permissions_scanner/writers/__init__.py
--rw-r--r--   0        0        0     1448 2024-03-19 10:07:44.434944 udps-0.1.33/universal_data_permissions_scanner/writers/base_writers.py
--rw-r--r--   0        0        0      728 2024-03-19 10:07:44.434944 udps-0.1.33/universal_data_permissions_scanner/writers/csv_writer.py
--rw-r--r--   0        0        0     1375 2024-03-19 10:07:44.434944 udps-0.1.33/universal_data_permissions_scanner/writers/get_writers.py
--rw-r--r--   0        0        0     2106 2024-03-19 10:07:44.434944 udps-0.1.33/universal_data_permissions_scanner/writers/multi_json_exporter.py
--rw-r--r--   0        0        0     5078 1970-01-01 00:00:00.000000 udps-0.1.33/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-16 11:04:11.258329 udps-0.1.34/LICENSE
+-rw-r--r--   0        0        0     2471 2024-04-16 11:04:11.258329 udps-0.1.34/README.md
+-rw-r--r--   0        0        0     3121 2024-04-16 11:04:11.258329 udps-0.1.34/pyproject.toml
+-rw-r--r--   0        0        0       44 2024-04-16 11:04:11.258329 udps-0.1.34/tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-16 11:04:11.258329 udps-0.1.34/tests/mocks/__init__.py
+-rw-r--r--   0        0        0      721 2024-04-16 11:04:11.258329 udps-0.1.34/tests/mocks/mock_writers.py
+-rw-r--r--   0        0        0     1028 2024-04-16 11:04:11.258329 udps-0.1.34/tests/test_authz_analyzer.py
+-rw-r--r--   0        0        0     6550 2024-04-16 11:04:11.258329 udps-0.1.34/tests/test_cli.py
+-rw-r--r--   0        0        0        0 2024-04-16 11:04:11.258329 udps-0.1.34/tests/test_writers/__init__.py
+-rw-r--r--   0        0        0     1403 2024-04-16 11:04:11.258329 udps-0.1.34/tests/test_writers/test_csv_writer.py
+-rw-r--r--   0        0        0      953 2024-04-16 11:04:11.258329 udps-0.1.34/tests/test_writers/test_multijson_writer.py
+-rw-r--r--   0        0        0        0 2024-04-16 11:04:11.258329 udps-0.1.34/tests/tests_datastores/__init__.py
+-rw-r--r--   0        0        0        1 2024-04-16 11:04:11.258329 udps-0.1.34/tests/tests_datastores/aws/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-16 11:04:11.258329 udps-0.1.34/tests/tests_datastores/aws/aws_ptrp/__init__.py
+-rw-r--r--   0        0        0    14110 2024-04-16 11:04:11.258329 udps-0.1.34/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/action/action_resolving_assume_role.json
+-rw-r--r--   0        0        0    11644 2024-04-16 11:04:11.262328 udps-0.1.34/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/action/action_resolving_federated_user.json
+-rw-r--r--   0        0        0    14917 2024-04-16 11:04:11.262328 udps-0.1.34/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/action/action_resolving_s3.json
+-rw-r--r--   0        0        0     9884 2024-04-16 11:04:11.262328 udps-0.1.34/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/action/assume_role_actions_for_principal_type.json
+-rw-r--r--   0        0        0    20662 2024-04-16 11:04:11.262328 udps-0.1.34/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/deny_with_condition/deny_with_condition_on_assume_role.json
+-rw-r--r--   0        0        0    31812 2024-04-16 11:04:11.262328 udps-0.1.34/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/deny_with_condition/deny_with_condition_on_s3_bucket.json
+-rw-r--r--   0        0        0    18235 2024-04-16 11:04:11.262328 udps-0.1.34/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/federated_user/federated_user_cross_account.json
+-rw-r--r--   0        0        0    17618 2024-04-16 11:04:11.262328 udps-0.1.34/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/federated_user/iam_user_to_federated_user.json
+-rw-r--r--   0        0        0     7529 2024-04-16 11:04:11.262328 udps-0.1.34/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_groups/iam_user_with_2_groups_includng_allow_and_deny.json
+-rw-r--r--   0        0        0     7744 2024-04-16 11:04:11.262328 udps-0.1.34/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_groups/iam_user_with_group_and_attached_policy.json
+-rw-r--r--   0        0        0     4073 2024-04-16 11:04:11.262328 udps-0.1.34/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_groups/iam_user_with_group_simple_policy.json
+-rw-r--r--   0        0        0    24204 2024-04-16 11:04:11.262328 udps-0.1.34/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_identity_center/iam_identity_center_with_users_and_groups.json
+-rw-r--r--   0        0        0    20163 2024-04-16 11:04:11.262328 udps-0.1.34/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_roles/assume_role_cross_account.json
+-rw-r--r--   0        0        0    13494 2024-04-16 11:04:11.262328 udps-0.1.34/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_roles/assume_role_to_role.json
+-rw-r--r--   0        0        0     8446 2024-04-16 11:04:11.262328 udps-0.1.34/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_roles/assume_role_via_resourve_based.json
+-rw-r--r--   0        0        0    16466 2024-04-16 11:04:11.262328 udps-0.1.34/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_roles/simple_assume_role.json
+-rw-r--r--   0        0        0    16126 2024-04-16 11:04:11.262328 udps-0.1.34/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_roles/valid_assume_action.json
+-rw-r--r--   0        0        0    14831 2024-04-16 11:04:11.262328 udps-0.1.34/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_user_to_s3_bucket/iam_user_with_attached_policy_and_deny.json
+-rw-r--r--   0        0        0     3066 2024-04-16 11:04:11.262328 udps-0.1.34/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_user_to_s3_bucket/iam_user_with_inline_policy.json
+-rw-r--r--   0        0        0     5550 2024-04-16 11:04:11.262328 udps-0.1.34/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_user_to_s3_bucket/iam_user_with_inline_policy_and_deny.json
+-rw-r--r--   0        0        0     5906 2024-04-16 11:04:11.262328 udps-0.1.34/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_user_to_s3_bucket/iam_user_with_inline_policy_and_resource_based.json
+-rw-r--r--   0        0        0     4446 2024-04-16 11:04:11.262328 udps-0.1.34/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_user_to_s3_bucket/iam_user_with_inline_policy_multi_stmts.json
+-rw-r--r--   0        0        0     8937 2024-04-16 11:04:11.262328 udps-0.1.34/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/multi_iam_users_to_multi_s3_buckets/iam_users_to_s3_cross_account_via_resource_based.json
+-rw-r--r--   0        0        0    20162 2024-04-16 11:04:11.262328 udps-0.1.34/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/multi_iam_users_to_multi_s3_buckets/multi_iam_users_to_multi_s3_buckets.json
+-rw-r--r--   0        0        0    10324 2024-04-16 11:04:11.262328 udps-0.1.34/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/assume_role_with_not_resource.json
+-rw-r--r--   0        0        0     6886 2024-04-16 11:04:11.262328 udps-0.1.34/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/federated_users_with_not_resource.json
+-rw-r--r--   0        0        0    23422 2024-04-16 11:04:11.262328 udps-0.1.34/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_combinations_in_both_allow_and_deny.json
+-rw-r--r--   0        0        0     2358 2024-04-16 11:04:11.262328 udps-0.1.34/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_in_all_allow.json
+-rw-r--r--   0        0        0     7124 2024-04-16 11:04:11.262328 udps-0.1.34/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_in_all_deny.json
+-rw-r--r--   0        0        0     4549 2024-04-16 11:04:11.262328 udps-0.1.34/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_including_wildcard_object_regex_allow.json
+-rw-r--r--   0        0        0     5215 2024-04-16 11:04:11.262328 udps-0.1.34/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_including_wildcard_object_regex_deny.json
+-rw-r--r--   0        0        0     5987 2024-04-16 11:04:11.262328 udps-0.1.34/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_multiple_wildcard_regexes.json
+-rw-r--r--   0        0        0     5862 2024-04-16 11:04:11.262328 udps-0.1.34/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_on_no_valid_resource_arn_allow.json
+-rw-r--r--   0        0        0     3396 2024-04-16 11:04:11.262328 udps-0.1.34/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_on_no_valid_resource_arn_deny.json
+-rw-r--r--   0        0        0     2298 2024-04-16 11:04:11.262328 udps-0.1.34/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_action/iam_user_allowed_no_action.json
+-rw-r--r--   0        0        0     5264 2024-04-16 11:04:11.262328 udps-0.1.34/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_action/iam_user_allowed_no_action_s3_complement.json
+-rw-r--r--   0        0        0     4596 2024-04-16 11:04:11.262328 udps-0.1.34/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_action/iam_user_with_multiple_actions_in_no_action_resource.json
+-rw-r--r--   0        0        0     3653 2024-04-16 11:04:11.262328 udps-0.1.34/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_action/iam_user_with_resource_no_action_simple.json
+-rw-r--r--   0        0        0     4392 2024-04-16 11:04:11.262328 udps-0.1.34/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_action/iam_user_with_resource_no_action_wildcard_action_set.json
+-rw-r--r--   0        0        0    26158 2024-04-16 11:04:11.262328 udps-0.1.34/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_principal/iam_users_roles_and_federated_with_deny_not_principal_single_account.json
+-rw-r--r--   0        0        0    10097 2024-04-16 11:04:11.262328 udps-0.1.34/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_principal/iam_users_with_deny_not_principal_cross_accounts.json
+-rw-r--r--   0        0        0     8580 2024-04-16 11:04:11.262328 udps-0.1.34/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/principal/irrelevant_principal_types.json
+-rw-r--r--   0        0        0    33775 2024-04-16 11:04:11.262328 udps-0.1.34/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/principal/principal_resolving_via_resource_based.json
+-rw-r--r--   0        0        0    16439 2024-04-16 11:04:11.262328 udps-0.1.34/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/resource/resouce_resolving_assume_role.json
+-rw-r--r--   0        0        0    13955 2024-04-16 11:04:11.262328 udps-0.1.34/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/resource/resouce_resolving_federated_user.json
+-rw-r--r--   0        0        0    18162 2024-04-16 11:04:11.262328 udps-0.1.34/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/resource/resouce_resolving_s3.json
+-rw-r--r--   0        0        0     3040 2024-04-16 11:04:11.262328 udps-0.1.34/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/s3_resource_regex/deny_and_allow_default.json
+-rw-r--r--   0        0        0     5254 2024-04-16 11:04:11.262328 udps-0.1.34/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/s3_resource_regex/deny_and_allow_on_object_multi_stmts.json
+-rw-r--r--   0        0        0     3569 2024-04-16 11:04:11.262328 udps-0.1.34/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/s3_resource_regex/deny_and_allow_with_one_resource_in_deny_that_is_a_subgroup_of_all_in_allow.json
+-rw-r--r--   0        0        0     4436 2024-04-16 11:04:11.262328 udps-0.1.34/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/s3_resource_regex/deny_on_object_and_allow_bucket.json
+-rw-r--r--   0        0        0    14441 2024-04-16 11:04:11.262328 udps-0.1.34/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/s3_resource_regex/valid_actions_objects_and_actions_resources.json
+-rw-r--r--   0        0        0     3581 2024-04-16 11:04:11.262328 udps-0.1.34/tests/tests_datastores/aws/aws_ptrp/test_create_session_with_assume_role.py
+-rw-r--r--   0        0        0     4890 2024-04-16 11:04:11.262328 udps-0.1.34/tests/tests_datastores/aws/aws_ptrp/test_resolve_permissions.py
+-rw-r--r--   0        0        0     4859 2024-04-16 11:04:11.262328 udps-0.1.34/tests/tests_datastores/aws/aws_ptrp/test_satori_dev_account_ptrp.py
+-rw-r--r--   0        0        0        0 2024-04-16 11:04:11.262328 udps-0.1.34/tests/tests_datastores/aws/aws_ptrp/utils/__init__.py
+-rw-r--r--   0        0        0     2831 2024-04-16 11:04:11.262328 udps-0.1.34/tests/tests_datastores/aws/aws_ptrp/utils/aws_ptrp_load_from_dict.py
+-rw-r--r--   0        0        0     1595 2024-04-16 11:04:11.262328 udps-0.1.34/tests/tests_datastores/aws/exporter_test_inputs/ptrp_line_basic_iam_user_and_policy_path.json
+-rw-r--r--   0        0        0     3805 2024-04-16 11:04:11.262328 udps-0.1.34/tests/tests_datastores/aws/exporter_test_inputs/ptrp_line_iam_identity_center_user_and_group.json
+-rw-r--r--   0        0        0     2597 2024-04-16 11:04:11.262328 udps-0.1.34/tests/tests_datastores/aws/exporter_test_inputs/ptrp_line_multiple_roles_in_path_and_all_principals.json
+-rw-r--r--   0        0        0     2321 2024-04-16 11:04:11.262328 udps-0.1.34/tests/tests_datastores/aws/exporter_test_inputs/ptrp_line_with_federated_user.json
+-rw-r--r--   0        0        0     4018 2024-04-16 11:04:11.262328 udps-0.1.34/tests/tests_datastores/aws/exporter_test_inputs/ptrp_line_with_iam_group_and_notes.json
+-rw-r--r--   0        0        0     5298 2024-04-16 11:04:11.262328 udps-0.1.34/tests/tests_datastores/aws/exporter_test_inputs/ptrp_line_with_notes.json
+-rw-r--r--   0        0        0     1579 2024-04-16 11:04:11.262328 udps-0.1.34/tests/tests_datastores/aws/test_exporter.py
+-rw-r--r--   0        0        0        0 2024-04-16 11:04:11.262328 udps-0.1.34/tests/tests_datastores/aws/utils/__init__.py
+-rw-r--r--   0        0        0     1731 2024-04-16 11:04:11.262328 udps-0.1.34/tests/tests_datastores/aws/utils/test_aws_regex_full_subset.py
+-rw-r--r--   0        0        0        0 2024-04-16 11:04:11.262328 udps-0.1.34/tests/tests_datastores/bigquery/__init__.py
+-rw-r--r--   0        0        0     5596 2024-04-16 11:04:11.262328 udps-0.1.34/tests/tests_datastores/bigquery/generate_authz_entry.py
+-rw-r--r--   0        0        0     7185 2024-04-16 11:04:11.262328 udps-0.1.34/tests/tests_datastores/bigquery/mocks.py
+-rw-r--r--   0        0        0    15539 2024-04-16 11:04:11.262328 udps-0.1.34/tests/tests_datastores/bigquery/test_bigquery.py
+-rw-r--r--   0        0        0        0 2024-04-16 11:04:11.262328 udps-0.1.34/tests/tests_datastores/databricks/__init__.py
+-rw-r--r--   0        0        0    17596 2024-04-16 11:04:11.262328 udps-0.1.34/tests/tests_datastores/databricks/generate_authz_entry.py
+-rw-r--r--   0        0        0     9136 2024-04-16 11:04:11.262328 udps-0.1.34/tests/tests_datastores/databricks/mocks.py
+-rw-r--r--   0        0        0    13149 2024-04-16 11:04:11.262328 udps-0.1.34/tests/tests_datastores/databricks/test_analyzer.py
+-rw-r--r--   0        0        0        0 2024-04-16 11:04:11.262328 udps-0.1.34/tests/tests_datastores/mongodb/__init__.py
+-rw-r--r--   0        0        0     1809 2024-04-16 11:04:11.262328 udps-0.1.34/tests/tests_datastores/mongodb/test_atlas_build_custom_role_from_response.py
+-rw-r--r--   0        0        0    14532 2024-04-16 11:04:11.262328 udps-0.1.34/tests/tests_datastores/mongodb/test_atlas_organization_users.py
+-rw-r--r--   0        0        0     7391 2024-04-16 11:04:11.262328 udps-0.1.34/tests/tests_datastores/mongodb/test_mongodb.py
+-rw-r--r--   0        0        0        0 2024-04-16 11:04:11.262328 udps-0.1.34/tests/tests_datastores/postgres/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-16 11:04:11.262328 udps-0.1.34/tests/tests_datastores/postgres/mocks/__init__.py
+-rw-r--r--   0        0        0     1195 2024-04-16 11:04:11.262328 udps-0.1.34/tests/tests_datastores/postgres/mocks/postgres_mock_connector.py
+-rw-r--r--   0        0        0    12910 2024-04-16 11:04:11.262328 udps-0.1.34/tests/tests_datastores/postgres/test_postgress_analyzer.py
+-rw-r--r--   0        0        0        0 2024-04-16 11:04:11.262328 udps-0.1.34/tests/tests_datastores/redshift/__init__.py
+-rw-r--r--   0        0        0    12365 2024-04-16 11:04:11.262328 udps-0.1.34/tests/tests_datastores/redshift/test_redshift.py
+-rw-r--r--   0        0        0        0 2024-04-16 11:04:11.262328 udps-0.1.34/tests/tests_datastores/snowflake/__init__.py
+-rw-r--r--   0        0        0    19120 2024-04-16 11:04:11.262328 udps-0.1.34/tests/tests_datastores/snowflake/test_snowflake_analyzer.py
+-rw-r--r--   0        0        0     1086 2024-04-16 11:04:11.262328 udps-0.1.34/universal_data_permissions_scanner/__init__.py
+-rw-r--r--   0        0        0    11916 2024-04-16 11:04:11.262328 udps-0.1.34/universal_data_permissions_scanner/cli.py
+-rw-r--r--   0        0        0        0 2024-04-16 11:04:11.262328 udps-0.1.34/universal_data_permissions_scanner/datastores/__init__.py
+-rw-r--r--   0        0        0      626 2024-04-16 11:04:11.262328 udps-0.1.34/universal_data_permissions_scanner/datastores/aws/__init__.py
+-rw-r--r--   0        0        0      113 2024-04-16 11:04:11.262328 udps-0.1.34/universal_data_permissions_scanner/datastores/aws/analyzer/__init__.py
+-rw-r--r--   0        0        0     2912 2024-04-16 11:04:11.262328 udps-0.1.34/universal_data_permissions_scanner/datastores/aws/analyzer/analyzer.py
+-rw-r--r--   0        0        0     7808 2024-04-16 11:04:11.262328 udps-0.1.34/universal_data_permissions_scanner/datastores/aws/analyzer/exporter.py
+-rw-r--r--   0        0        0        0 2024-04-16 11:04:11.262328 udps-0.1.34/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/__init__.py
+-rw-r--r--   0        0        0    13055 2024-04-16 11:04:11.262328 udps-0.1.34/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/analyzer.py
+-rw-r--r--   0        0        0       90 2024-04-16 11:04:11.262328 udps-0.1.34/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/commands/all_databases.sql
+-rw-r--r--   0        0        0      141 2024-04-16 11:04:11.262328 udps-0.1.34/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/commands/all_tables.sql
+-rw-r--r--   0        0        0      111 2024-04-16 11:04:11.262328 udps-0.1.34/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/commands/datashare_consumers.sql
+-rw-r--r--   0        0        0       14 2024-04-16 11:04:11.262328 udps-0.1.34/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/commands/datashare_desc.sql
+-rw-r--r--   0        0        0      125 2024-04-16 11:04:11.262328 udps-0.1.34/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/commands/datashares.sql
+-rw-r--r--   0        0        0      318 2024-04-16 11:04:11.262328 udps-0.1.34/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/commands/identities_pg_user.sql
+-rw-r--r--   0        0        0      262 2024-04-16 11:04:11.262328 udps-0.1.34/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/commands/identities_privileges.sql
+-rw-r--r--   0        0        0      307 2024-04-16 11:04:11.262328 udps-0.1.34/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/commands/identities_svv_role_grants.sql
+-rw-r--r--   0        0        0      256 2024-04-16 11:04:11.262328 udps-0.1.34/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/commands/identities_svv_user_grants.sql
+-rw-r--r--   0        0        0     5539 2024-04-16 11:04:11.266328 udps-0.1.34/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/exporter.py
+-rw-r--r--   0        0        0     3524 2024-04-16 11:04:11.266328 udps-0.1.34/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/model.py
+-rw-r--r--   0        0        0      660 2024-04-16 11:04:11.266328 udps-0.1.34/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/service.py
+-rw-r--r--   0        0        0      120 2024-04-16 11:04:11.266328 udps-0.1.34/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-16 11:04:11.266328 udps-0.1.34/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/actions/__init__.py
+-rw-r--r--   0        0        0     3041 2024-04-16 11:04:11.266328 udps-0.1.34/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/actions/actions_resolver.py
+-rw-r--r--   0        0        0     2045 2024-04-16 11:04:11.266328 udps-0.1.34/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/actions/aws_actions.py
+-rw-r--r--   0        0        0        0 2024-04-16 11:04:11.266328 udps-0.1.34/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/__init__.py
+-rw-r--r--   0        0        0     5682 2024-04-16 11:04:11.266328 udps-0.1.34/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/iam_entities.py
+-rw-r--r--   0        0        0     3505 2024-04-16 11:04:11.266328 udps-0.1.34/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/iam_groups.py
+-rw-r--r--   0        0        0     2481 2024-04-16 11:04:11.266328 udps-0.1.34/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/iam_policies.py
+-rw-r--r--   0        0        0     6201 2024-04-16 11:04:11.266328 udps-0.1.34/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/iam_roles.py
+-rw-r--r--   0        0        0     3963 2024-04-16 11:04:11.266328 udps-0.1.34/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/iam_users.py
+-rw-r--r--   0        0        0      254 2024-04-16 11:04:11.266328 udps-0.1.34/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/policy/__init__.py
+-rw-r--r--   0        0        0       87 2024-04-16 11:04:11.266328 udps-0.1.34/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/policy/effect.py
+-rw-r--r--   0        0        0      263 2024-04-16 11:04:11.266328 udps-0.1.34/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/policy/group_policy.py
+-rw-r--r--   0        0        0      415 2024-04-16 11:04:11.266328 udps-0.1.34/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/policy/policy.py
+-rw-r--r--   0        0        0     6232 2024-04-16 11:04:11.266328 udps-0.1.34/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/policy/policy_document.py
+-rw-r--r--   0        0        0    10500 2024-04-16 11:04:11.266328 udps-0.1.34/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/policy/policy_document_resolver.py
+-rw-r--r--   0        0        0      373 2024-04-16 11:04:11.266328 udps-0.1.34/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/policy/policy_document_utils.py
+-rw-r--r--   0        0        0      261 2024-04-16 11:04:11.266328 udps-0.1.34/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/policy/user_policy.py
+-rw-r--r--   0        0        0      263 2024-04-16 11:04:11.266328 udps-0.1.34/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/public_block_access_config.py
+-rw-r--r--   0        0        0        0 2024-04-16 11:04:11.266328 udps-0.1.34/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/role/__init__.py
+-rw-r--r--   0        0        0      261 2024-04-16 11:04:11.266328 udps-0.1.34/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/role/role_policy.py
+-rw-r--r--   0        0        0        0 2024-04-16 11:04:11.266328 udps-0.1.34/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam_identity_center/__init__.py
+-rw-r--r--   0        0        0     5655 2024-04-16 11:04:11.266328 udps-0.1.34/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam_identity_center/iam_identity_center_entities.py
+-rw-r--r--   0        0        0     1961 2024-04-16 11:04:11.266328 udps-0.1.34/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam_identity_center/iam_identity_center_groups.py
+-rw-r--r--   0        0        0     1824 2024-04-16 11:04:11.266328 udps-0.1.34/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam_identity_center/iam_identity_center_users.py
+-rw-r--r--   0        0        0     2502 2024-04-16 11:04:11.266328 udps-0.1.34/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam_identity_center/permission_sets.py
+-rw-r--r--   0        0        0     1046 2024-04-16 11:04:11.266328 udps-0.1.34/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/logger.py
+-rw-r--r--   0        0        0      263 2024-04-16 11:04:11.266328 udps-0.1.34/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/policy_evaluation/__init__.py
+-rw-r--r--   0        0        0    18760 2024-04-16 11:04:11.266328 udps-0.1.34/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/policy_evaluation/policy_evaluation.py
+-rw-r--r--   0        0        0      172 2024-04-16 11:04:11.266328 udps-0.1.34/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/principals/__init__.py
+-rw-r--r--   0        0        0    12129 2024-04-16 11:04:11.266328 udps-0.1.34/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/principals/aws_principals.py
+-rw-r--r--   0        0        0     1267 2024-04-16 11:04:11.266328 udps-0.1.34/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/principals/no_entity_principal.py
+-rw-r--r--   0        0        0    12938 2024-04-16 11:04:11.266328 udps-0.1.34/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/principals/principal.py
+-rw-r--r--   0        0        0     3787 2024-04-16 11:04:11.266328 udps-0.1.34/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/principals/principals_resolver.py
+-rw-r--r--   0        0        0    10597 2024-04-16 11:04:11.266328 udps-0.1.34/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp.py
+-rw-r--r--   0        0        0        0 2024-04-16 11:04:11.266328 udps-0.1.34/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_allowed_lines/__init__.py
+-rw-r--r--   0        0        0    12040 2024-04-16 11:04:11.266328 udps-0.1.34/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_allowed_lines/allowed_line.py
+-rw-r--r--   0        0        0     8007 2024-04-16 11:04:11.266328 udps-0.1.34/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_allowed_lines/allowed_line_node_notes.py
+-rw-r--r--   0        0        0    15325 2024-04-16 11:04:11.266328 udps-0.1.34/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_allowed_lines/allowed_line_nodes_base.py
+-rw-r--r--   0        0        0    26515 2024-04-16 11:04:11.266328 udps-0.1.34/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_allowed_lines/allowed_lines_resolver.py
+-rw-r--r--   0        0        0     6471 2024-04-16 11:04:11.266328 udps-0.1.34/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_allowed_lines/allowed_lines_resolver_result.py
+-rw-r--r--   0        0        0      513 2024-04-16 11:04:11.266328 udps-0.1.34/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_models/__init__.py
+-rw-r--r--   0        0        0     8549 2024-04-16 11:04:11.266328 udps-0.1.34/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_models/ptrp_model.py
+-rw-r--r--   0        0        0        0 2024-04-16 11:04:11.266328 udps-0.1.34/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/resources/__init__.py
+-rw-r--r--   0        0        0     5233 2024-04-16 11:04:11.266328 udps-0.1.34/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/resources/account_resources.py
+-rw-r--r--   0        0        0     4475 2024-04-16 11:04:11.266328 udps-0.1.34/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/resources/resources_resolver.py
+-rw-r--r--   0        0        0     1644 2024-04-16 11:04:11.266328 udps-0.1.34/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-16 11:04:11.266328 udps-0.1.34/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/assume_role/__init__.py
+-rw-r--r--   0        0        0     2904 2024-04-16 11:04:11.266328 udps-0.1.34/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/assume_role/assume_role_actions.py
+-rw-r--r--   0        0        0     6157 2024-04-16 11:04:11.266328 udps-0.1.34/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/assume_role/assume_role_resources.py
+-rw-r--r--   0        0        0     2185 2024-04-16 11:04:11.266328 udps-0.1.34/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/assume_role/assume_role_service.py
+-rw-r--r--   0        0        0        0 2024-04-16 11:04:11.266328 udps-0.1.34/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/federated_user/__init__.py
+-rw-r--r--   0        0        0     2146 2024-04-16 11:04:11.266328 udps-0.1.34/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/federated_user/federated_user_actions.py
+-rw-r--r--   0        0        0     7452 2024-04-16 11:04:11.266328 udps-0.1.34/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/federated_user/federated_user_resources.py
+-rw-r--r--   0        0        0     2289 2024-04-16 11:04:11.266328 udps-0.1.34/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/federated_user/federated_user_service.py
+-rw-r--r--   0        0        0     2594 2024-04-16 11:04:11.266328 udps-0.1.34/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/resolved_stmt.py
+-rw-r--r--   0        0        0        0 2024-04-16 11:04:11.266328 udps-0.1.34/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/s3/__init__.py
+-rw-r--r--   0        0        0     3377 2024-04-16 11:04:11.266328 udps-0.1.34/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/s3/bucket.py
+-rw-r--r--   0        0        0     1054 2024-04-16 11:04:11.266328 udps-0.1.34/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/s3/bucket_acl.py
+-rw-r--r--   0        0        0    17632 2024-04-16 11:04:11.266328 udps-0.1.34/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/s3/s3_actions.py
+-rw-r--r--   0        0        0     7561 2024-04-16 11:04:11.266328 udps-0.1.34/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/s3/s3_resources.py
+-rw-r--r--   0        0        0     1894 2024-04-16 11:04:11.266328 udps-0.1.34/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/s3/s3_service.py
+-rw-r--r--   0        0        0      398 2024-04-16 11:04:11.266328 udps-0.1.34/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/service_action_base.py
+-rw-r--r--   0        0        0     1973 2024-04-16 11:04:11.266328 udps-0.1.34/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/service_action_type.py
+-rw-r--r--   0        0        0     3041 2024-04-16 11:04:11.266328 udps-0.1.34/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/service_actions_resolver_base.py
+-rw-r--r--   0        0        0      397 2024-04-16 11:04:11.266328 udps-0.1.34/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/service_base.py
+-rw-r--r--   0        0        0      561 2024-04-16 11:04:11.266328 udps-0.1.34/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/service_resource_base.py
+-rw-r--r--   0        0        0     2501 2024-04-16 11:04:11.266328 udps-0.1.34/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/service_resource_type.py
+-rw-r--r--   0        0        0     9989 2024-04-16 11:04:11.266328 udps-0.1.34/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/service_resources_resolver_base.py
+-rw-r--r--   0        0        0        0 2024-04-16 11:04:11.266328 udps-0.1.34/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/utils/__init__.py
+-rw-r--r--   0        0        0      482 2024-04-16 11:04:11.266328 udps-0.1.34/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/utils/assume_role.py
+-rw-r--r--   0        0        0      879 2024-04-16 11:04:11.266328 udps-0.1.34/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/utils/create_session.py
+-rw-r--r--   0        0        0     1000 2024-04-16 11:04:11.266328 udps-0.1.34/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/utils/pagination.py
+-rw-r--r--   0        0        0     2747 2024-04-16 11:04:11.266328 udps-0.1.34/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/utils/regex_subset.py
+-rw-r--r--   0        0        0      178 2024-04-16 11:04:11.266328 udps-0.1.34/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/utils/serde.py
+-rw-r--r--   0        0        0      131 2024-04-16 11:04:11.266328 udps-0.1.34/universal_data_permissions_scanner/datastores/bigquery/__init__.py
+-rw-r--r--   0        0        0    11167 2024-04-16 11:04:11.266328 udps-0.1.34/universal_data_permissions_scanner/datastores/bigquery/analyzer.py
+-rw-r--r--   0        0        0    12689 2024-04-16 11:04:11.266328 udps-0.1.34/universal_data_permissions_scanner/datastores/bigquery/policy_tree.py
+-rw-r--r--   0        0        0     8010 2024-04-16 11:04:11.266328 udps-0.1.34/universal_data_permissions_scanner/datastores/bigquery/service.py
+-rw-r--r--   0        0        0      138 2024-04-16 11:04:11.266328 udps-0.1.34/universal_data_permissions_scanner/datastores/databricks/__init__.py
+-rw-r--r--   0        0        0     6733 2024-04-16 11:04:11.266328 udps-0.1.34/universal_data_permissions_scanner/datastores/databricks/analyzer.py
+-rw-r--r--   0        0        0       53 2024-04-16 11:04:11.266328 udps-0.1.34/universal_data_permissions_scanner/datastores/databricks/exceptions.py
+-rw-r--r--   0        0        0     8588 2024-04-16 11:04:11.266328 udps-0.1.34/universal_data_permissions_scanner/datastores/databricks/identities.py
+-rw-r--r--   0        0        0     1331 2024-04-16 11:04:11.266328 udps-0.1.34/universal_data_permissions_scanner/datastores/databricks/model.py
+-rw-r--r--   0        0        0    10803 2024-04-16 11:04:11.266328 udps-0.1.34/universal_data_permissions_scanner/datastores/databricks/policy_tree.py
+-rw-r--r--   0        0        0      138 2024-04-16 11:04:11.266328 udps-0.1.34/universal_data_permissions_scanner/datastores/databricks/service/__init__.py
+-rw-r--r--   0        0        0      138 2024-04-16 11:04:11.266328 udps-0.1.34/universal_data_permissions_scanner/datastores/databricks/service/authentication/__init__.py
+-rw-r--r--   0        0        0      879 2024-04-16 11:04:11.266328 udps-0.1.34/universal_data_permissions_scanner/datastores/databricks/service/authentication/authentication.py
+-rw-r--r--   0        0        0      110 2024-04-16 11:04:11.266328 udps-0.1.34/universal_data_permissions_scanner/datastores/databricks/service/authentication/basic.py
+-rw-r--r--   0        0        0     1930 2024-04-16 11:04:11.266328 udps-0.1.34/universal_data_permissions_scanner/datastores/databricks/service/authentication/oauth.py
+-rw-r--r--   0        0        0       48 2024-04-16 11:04:11.266328 udps-0.1.34/universal_data_permissions_scanner/datastores/databricks/service/exceptions.py
+-rw-r--r--   0        0        0     2448 2024-04-16 11:04:11.266328 udps-0.1.34/universal_data_permissions_scanner/datastores/databricks/service/model.py
+-rw-r--r--   0        0        0     4024 2024-04-16 11:04:11.266328 udps-0.1.34/universal_data_permissions_scanner/datastores/databricks/service/scim.py
+-rw-r--r--   0        0        0        0 2024-04-16 11:04:11.266328 udps-0.1.34/universal_data_permissions_scanner/datastores/mongodb/__init__.py
+-rw-r--r--   0        0        0    15596 2024-04-16 11:04:11.266328 udps-0.1.34/universal_data_permissions_scanner/datastores/mongodb/analyzer.py
+-rw-r--r--   0        0        0        0 2024-04-16 11:04:11.266328 udps-0.1.34/universal_data_permissions_scanner/datastores/mongodb/atlas/__init__.py
+-rw-r--r--   0        0        0    17520 2024-04-16 11:04:11.266328 udps-0.1.34/universal_data_permissions_scanner/datastores/mongodb/atlas/analyzer.py
+-rw-r--r--   0        0        0      625 2024-04-16 11:04:11.266328 udps-0.1.34/universal_data_permissions_scanner/datastores/mongodb/atlas/exceptions.py
+-rw-r--r--   0        0        0     7603 2024-04-16 11:04:11.266328 udps-0.1.34/universal_data_permissions_scanner/datastores/mongodb/atlas/model.py
+-rw-r--r--   0        0        0     2527 2024-04-16 11:04:11.266328 udps-0.1.34/universal_data_permissions_scanner/datastores/mongodb/atlas/permission_resolvers.py
+-rw-r--r--   0        0        0     6270 2024-04-16 11:04:11.266328 udps-0.1.34/universal_data_permissions_scanner/datastores/mongodb/atlas/service.py
+-rw-r--r--   0        0        0     2394 2024-04-16 11:04:11.266328 udps-0.1.34/universal_data_permissions_scanner/datastores/mongodb/atlas/service_model.py
+-rw-r--r--   0        0        0     2197 2024-04-16 11:04:11.266328 udps-0.1.34/universal_data_permissions_scanner/datastores/mongodb/model.py
+-rw-r--r--   0        0        0     1553 2024-04-16 11:04:11.266328 udps-0.1.34/universal_data_permissions_scanner/datastores/mongodb/resolvers.py
+-rw-r--r--   0        0        0     1480 2024-04-16 11:04:11.266328 udps-0.1.34/universal_data_permissions_scanner/datastores/mongodb/service.py
+-rw-r--r--   0        0        0     1196 2024-04-16 11:04:11.266328 udps-0.1.34/universal_data_permissions_scanner/datastores/mongodb/service_model.py
+-rw-r--r--   0        0        0        0 2024-04-16 11:04:11.266328 udps-0.1.34/universal_data_permissions_scanner/datastores/postgres/__init__.py
+-rw-r--r--   0        0        0    10637 2024-04-16 11:04:11.266328 udps-0.1.34/universal_data_permissions_scanner/datastores/postgres/analyzer.py
+-rw-r--r--   0        0        0       71 2024-04-16 11:04:11.266328 udps-0.1.34/universal_data_permissions_scanner/datastores/postgres/commands/all_databases.sql
+-rw-r--r--   0        0        0      369 2024-04-16 11:04:11.266328 udps-0.1.34/universal_data_permissions_scanner/datastores/postgres/commands/all_tables.sql
+-rw-r--r--   0        0        0      272 2024-04-16 11:04:11.266328 udps-0.1.34/universal_data_permissions_scanner/datastores/postgres/commands/roles.sql
+-rw-r--r--   0        0        0      313 2024-04-16 11:04:11.266328 udps-0.1.34/universal_data_permissions_scanner/datastores/postgres/commands/roles_grants.sql
+-rw-r--r--   0        0        0     2404 2024-04-16 11:04:11.266328 udps-0.1.34/universal_data_permissions_scanner/datastores/postgres/database_query_results.py
+-rw-r--r--   0        0        0      822 2024-04-16 11:04:11.270328 udps-0.1.34/universal_data_permissions_scanner/datastores/postgres/deployment.py
+-rw-r--r--   0        0        0     2687 2024-04-16 11:04:11.270328 udps-0.1.34/universal_data_permissions_scanner/datastores/postgres/exporter.py
+-rw-r--r--   0        0        0     1891 2024-04-16 11:04:11.270328 udps-0.1.34/universal_data_permissions_scanner/datastores/postgres/model.py
+-rw-r--r--   0        0        0        0 2024-04-16 11:04:11.270328 udps-0.1.34/universal_data_permissions_scanner/datastores/snowflake/__init__.py
+-rw-r--r--   0        0        0    12492 2024-04-16 11:04:11.270328 udps-0.1.34/universal_data_permissions_scanner/datastores/snowflake/analyzer.py
+-rw-r--r--   0        0        0      389 2024-04-16 11:04:11.270328 udps-0.1.34/universal_data_permissions_scanner/datastores/snowflake/commands/grants_roles.sql
+-rw-r--r--   0        0        0       20 2024-04-16 11:04:11.270328 udps-0.1.34/universal_data_permissions_scanner/datastores/snowflake/commands/grants_to_share.sql
+-rw-r--r--   0        0        0       11 2024-04-16 11:04:11.270328 udps-0.1.34/universal_data_permissions_scanner/datastores/snowflake/commands/shares.sql
+-rw-r--r--   0        0        0      535 2024-04-16 11:04:11.270328 udps-0.1.34/universal_data_permissions_scanner/datastores/snowflake/commands/user_grants.sql
+-rw-r--r--   0        0        0     5827 2024-04-16 11:04:11.270328 udps-0.1.34/universal_data_permissions_scanner/datastores/snowflake/exporter.py
+-rw-r--r--   0        0        0     4685 2024-04-16 11:04:11.270328 udps-0.1.34/universal_data_permissions_scanner/datastores/snowflake/model.py
+-rw-r--r--   0        0        0     1394 2024-04-16 11:04:11.270328 udps-0.1.34/universal_data_permissions_scanner/datastores/snowflake/service.py
+-rw-r--r--   0        0        0        0 2024-04-16 11:04:11.270328 udps-0.1.34/universal_data_permissions_scanner/errors/__init__.py
+-rw-r--r--   0        0        0       45 2024-04-16 11:04:11.270328 udps-0.1.34/universal_data_permissions_scanner/errors/failed_connection_errors.py
+-rw-r--r--   0        0        0       58 2024-04-16 11:04:11.270328 udps-0.1.34/universal_data_permissions_scanner/errors/snowflake.py
+-rw-r--r--   0        0        0     7625 2024-04-16 11:04:11.270328 udps-0.1.34/universal_data_permissions_scanner/main.py
+-rw-r--r--   0        0        0      195 2024-04-16 11:04:11.270328 udps-0.1.34/universal_data_permissions_scanner/models/__init__.py
+-rw-r--r--   0        0        0     7583 2024-04-16 11:04:11.270328 udps-0.1.34/universal_data_permissions_scanner/models/model.py
+-rw-r--r--   0        0        0        0 2024-04-16 11:04:11.270328 udps-0.1.34/universal_data_permissions_scanner/utils/__init__.py
+-rw-r--r--   0        0        0      651 2024-04-16 11:04:11.270328 udps-0.1.34/universal_data_permissions_scanner/utils/logger.py
+-rw-r--r--   0        0        0      455 2024-04-16 11:04:11.270328 udps-0.1.34/universal_data_permissions_scanner/writers/__init__.py
+-rw-r--r--   0        0        0     1448 2024-04-16 11:04:11.270328 udps-0.1.34/universal_data_permissions_scanner/writers/base_writers.py
+-rw-r--r--   0        0        0      728 2024-04-16 11:04:11.270328 udps-0.1.34/universal_data_permissions_scanner/writers/csv_writer.py
+-rw-r--r--   0        0        0     1375 2024-04-16 11:04:11.270328 udps-0.1.34/universal_data_permissions_scanner/writers/get_writers.py
+-rw-r--r--   0        0        0     2106 2024-04-16 11:04:11.270328 udps-0.1.34/universal_data_permissions_scanner/writers/multi_json_exporter.py
+-rw-r--r--   0        0        0     5077 1970-01-01 00:00:00.000000 udps-0.1.34/PKG-INFO
```

### Comparing `udps-0.1.33/LICENSE` & `udps-0.1.34/LICENSE`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/README.md` & `udps-0.1.34/README.md`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/pyproject.toml` & `udps-0.1.34/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "udps"
-version = "0.1.33"
+version = "0.1.34"
 homepage = "https://github.com/satoricyber/universal-data-permissions-scanner"
 description = "Analyze authorization."
 authors = ["SatoriCyber"]
 readme = "README.md"
 classifiers=[
     'Development Status :: 4 - Beta',
     'Intended Audience :: Developers',
@@ -36,15 +36,15 @@
 psycopg2-binary = "^2.9.5"
 google-cloud-iam = "^2.10.0"
 redshift-connector = "^2.0.909"
 requests = "^2.28.1"
 pymongo = "^4.3.3"
 pytest  = {version="^7.2.0", optional = true}
 pytest-cov  = {version="^4.0.0", optional = true}
-black = {version="^22.12.0", optional=true}
+black = {version="^24.3.0", optional=true}
 isort = {version="^5.11.3", optional=true}
 twine = {version="^4.0.2", optional=true}
 types-psycopg2 = {version="^2.9.21.2", optional=true}
 google-api-python-client-stubs = {version="^1.13.0", optional=true}
 mypy = {version="^0.991", optional=true}
 virtualenv  = {version="^20.17.1", optional=true}
 pip  =  {version=">=22.3.1,<24.0.0", optional=true}
```

### Comparing `udps-0.1.33/tests/mocks/mock_writers.py` & `udps-0.1.34/tests/mocks/mock_writers.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/tests/test_authz_analyzer.py` & `udps-0.1.34/tests/test_authz_analyzer.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/tests/test_cli.py` & `udps-0.1.34/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/tests/test_writers/test_csv_writer.py` & `udps-0.1.34/tests/test_writers/test_csv_writer.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/tests/test_writers/test_multijson_writer.py` & `udps-0.1.34/tests/test_writers/test_multijson_writer.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/action/action_resolving_assume_role.json` & `udps-0.1.34/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/action/action_resolving_assume_role.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/action/action_resolving_federated_user.json` & `udps-0.1.34/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/action/action_resolving_federated_user.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/action/action_resolving_s3.json` & `udps-0.1.34/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/action/action_resolving_s3.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/action/assume_role_actions_for_principal_type.json` & `udps-0.1.34/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/action/assume_role_actions_for_principal_type.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/deny_with_condition/deny_with_condition_on_assume_role.json` & `udps-0.1.34/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/deny_with_condition/deny_with_condition_on_assume_role.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/deny_with_condition/deny_with_condition_on_s3_bucket.json` & `udps-0.1.34/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/deny_with_condition/deny_with_condition_on_s3_bucket.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/federated_user/federated_user_cross_account.json` & `udps-0.1.34/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/federated_user/federated_user_cross_account.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/federated_user/iam_user_to_federated_user.json` & `udps-0.1.34/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/federated_user/iam_user_to_federated_user.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_groups/iam_user_with_2_groups_includng_allow_and_deny.json` & `udps-0.1.34/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_groups/iam_user_with_2_groups_includng_allow_and_deny.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_groups/iam_user_with_group_and_attached_policy.json` & `udps-0.1.34/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_groups/iam_user_with_group_and_attached_policy.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_groups/iam_user_with_group_simple_policy.json` & `udps-0.1.34/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_groups/iam_user_with_group_simple_policy.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_identity_center/iam_identity_center_with_users_and_groups.json` & `udps-0.1.34/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_identity_center/iam_identity_center_with_users_and_groups.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_roles/assume_role_cross_account.json` & `udps-0.1.34/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_roles/assume_role_cross_account.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_roles/assume_role_to_role.json` & `udps-0.1.34/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_roles/assume_role_to_role.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_roles/assume_role_via_resourve_based.json` & `udps-0.1.34/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_roles/assume_role_via_resourve_based.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_roles/simple_assume_role.json` & `udps-0.1.34/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_roles/simple_assume_role.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_roles/valid_assume_action.json` & `udps-0.1.34/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_roles/valid_assume_action.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_user_to_s3_bucket/iam_user_with_attached_policy_and_deny.json` & `udps-0.1.34/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_user_to_s3_bucket/iam_user_with_attached_policy_and_deny.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_user_to_s3_bucket/iam_user_with_inline_policy.json` & `udps-0.1.34/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_user_to_s3_bucket/iam_user_with_inline_policy.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_user_to_s3_bucket/iam_user_with_inline_policy_and_deny.json` & `udps-0.1.34/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_user_to_s3_bucket/iam_user_with_inline_policy_and_deny.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_user_to_s3_bucket/iam_user_with_inline_policy_and_resource_based.json` & `udps-0.1.34/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_user_to_s3_bucket/iam_user_with_inline_policy_and_resource_based.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_user_to_s3_bucket/iam_user_with_inline_policy_multi_stmts.json` & `udps-0.1.34/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_user_to_s3_bucket/iam_user_with_inline_policy_multi_stmts.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/multi_iam_users_to_multi_s3_buckets/iam_users_to_s3_cross_account_via_resource_based.json` & `udps-0.1.34/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/multi_iam_users_to_multi_s3_buckets/iam_users_to_s3_cross_account_via_resource_based.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/multi_iam_users_to_multi_s3_buckets/multi_iam_users_to_multi_s3_buckets.json` & `udps-0.1.34/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/multi_iam_users_to_multi_s3_buckets/multi_iam_users_to_multi_s3_buckets.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/assume_role_with_not_resource.json` & `udps-0.1.34/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/assume_role_with_not_resource.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/federated_users_with_not_resource.json` & `udps-0.1.34/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/federated_users_with_not_resource.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_combinations_in_both_allow_and_deny.json` & `udps-0.1.34/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_combinations_in_both_allow_and_deny.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_in_all_allow.json` & `udps-0.1.34/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_in_all_allow.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_in_all_deny.json` & `udps-0.1.34/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_in_all_deny.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_including_wildcard_object_regex_allow.json` & `udps-0.1.34/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_including_wildcard_object_regex_allow.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_including_wildcard_object_regex_deny.json` & `udps-0.1.34/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_including_wildcard_object_regex_deny.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_multiple_wildcard_regexes.json` & `udps-0.1.34/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_multiple_wildcard_regexes.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_on_no_valid_resource_arn_allow.json` & `udps-0.1.34/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_on_no_valid_resource_arn_allow.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_on_no_valid_resource_arn_deny.json` & `udps-0.1.34/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_on_no_valid_resource_arn_deny.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_action/iam_user_allowed_no_action.json` & `udps-0.1.34/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_action/iam_user_allowed_no_action.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_action/iam_user_allowed_no_action_s3_complement.json` & `udps-0.1.34/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_action/iam_user_allowed_no_action_s3_complement.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_action/iam_user_with_multiple_actions_in_no_action_resource.json` & `udps-0.1.34/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_action/iam_user_with_multiple_actions_in_no_action_resource.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_action/iam_user_with_resource_no_action_simple.json` & `udps-0.1.34/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_action/iam_user_with_resource_no_action_simple.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_action/iam_user_with_resource_no_action_wildcard_action_set.json` & `udps-0.1.34/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_action/iam_user_with_resource_no_action_wildcard_action_set.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_principal/iam_users_roles_and_federated_with_deny_not_principal_single_account.json` & `udps-0.1.34/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_principal/iam_users_roles_and_federated_with_deny_not_principal_single_account.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_principal/iam_users_with_deny_not_principal_cross_accounts.json` & `udps-0.1.34/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_principal/iam_users_with_deny_not_principal_cross_accounts.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/principal/irrelevant_principal_types.json` & `udps-0.1.34/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/principal/irrelevant_principal_types.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/principal/principal_resolving_via_resource_based.json` & `udps-0.1.34/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/principal/principal_resolving_via_resource_based.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/resource/resouce_resolving_assume_role.json` & `udps-0.1.34/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/resource/resouce_resolving_assume_role.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/resource/resouce_resolving_federated_user.json` & `udps-0.1.34/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/resource/resouce_resolving_federated_user.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/resource/resouce_resolving_s3.json` & `udps-0.1.34/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/resource/resouce_resolving_s3.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/s3_resource_regex/deny_and_allow_default.json` & `udps-0.1.34/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/s3_resource_regex/deny_and_allow_default.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/s3_resource_regex/deny_and_allow_on_object_multi_stmts.json` & `udps-0.1.34/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/s3_resource_regex/deny_and_allow_on_object_multi_stmts.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/s3_resource_regex/deny_and_allow_with_one_resource_in_deny_that_is_a_subgroup_of_all_in_allow.json` & `udps-0.1.34/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/s3_resource_regex/deny_and_allow_with_one_resource_in_deny_that_is_a_subgroup_of_all_in_allow.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/s3_resource_regex/deny_on_object_and_allow_bucket.json` & `udps-0.1.34/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/s3_resource_regex/deny_on_object_and_allow_bucket.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/s3_resource_regex/valid_actions_objects_and_actions_resources.json` & `udps-0.1.34/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/s3_resource_regex/valid_actions_objects_and_actions_resources.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/tests/tests_datastores/aws/aws_ptrp/test_create_session_with_assume_role.py` & `udps-0.1.34/tests/tests_datastores/aws/aws_ptrp/test_create_session_with_assume_role.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/tests/tests_datastores/aws/aws_ptrp/test_resolve_permissions.py` & `udps-0.1.34/tests/tests_datastores/aws/aws_ptrp/test_resolve_permissions.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/tests/tests_datastores/aws/aws_ptrp/test_satori_dev_account_ptrp.py` & `udps-0.1.34/tests/tests_datastores/aws/aws_ptrp/test_satori_dev_account_ptrp.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/tests/tests_datastores/aws/aws_ptrp/utils/aws_ptrp_load_from_dict.py` & `udps-0.1.34/tests/tests_datastores/aws/aws_ptrp/utils/aws_ptrp_load_from_dict.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/tests/tests_datastores/aws/exporter_test_inputs/ptrp_line_basic_iam_user_and_policy_path.json` & `udps-0.1.34/tests/tests_datastores/aws/exporter_test_inputs/ptrp_line_basic_iam_user_and_policy_path.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/tests/tests_datastores/aws/exporter_test_inputs/ptrp_line_iam_identity_center_user_and_group.json` & `udps-0.1.34/tests/tests_datastores/aws/exporter_test_inputs/ptrp_line_iam_identity_center_user_and_group.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/tests/tests_datastores/aws/exporter_test_inputs/ptrp_line_multiple_roles_in_path_and_all_principals.json` & `udps-0.1.34/tests/tests_datastores/aws/exporter_test_inputs/ptrp_line_multiple_roles_in_path_and_all_principals.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/tests/tests_datastores/aws/exporter_test_inputs/ptrp_line_with_federated_user.json` & `udps-0.1.34/tests/tests_datastores/aws/exporter_test_inputs/ptrp_line_with_federated_user.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/tests/tests_datastores/aws/exporter_test_inputs/ptrp_line_with_iam_group_and_notes.json` & `udps-0.1.34/tests/tests_datastores/aws/exporter_test_inputs/ptrp_line_with_iam_group_and_notes.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/tests/tests_datastores/aws/exporter_test_inputs/ptrp_line_with_notes.json` & `udps-0.1.34/tests/tests_datastores/aws/exporter_test_inputs/ptrp_line_with_notes.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/tests/tests_datastores/aws/test_exporter.py` & `udps-0.1.34/tests/tests_datastores/aws/test_exporter.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/tests/tests_datastores/aws/utils/test_aws_regex_full_subset.py` & `udps-0.1.34/tests/tests_datastores/aws/utils/test_aws_regex_full_subset.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/tests/tests_datastores/bigquery/generate_authz_entry.py` & `udps-0.1.34/tests/tests_datastores/bigquery/generate_authz_entry.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/tests/tests_datastores/bigquery/mocks.py` & `udps-0.1.34/tests/tests_datastores/bigquery/mocks.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/tests/tests_datastores/bigquery/test_bigquery.py` & `udps-0.1.34/tests/tests_datastores/bigquery/test_bigquery.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/tests/tests_datastores/databricks/generate_authz_entry.py` & `udps-0.1.34/tests/tests_datastores/databricks/generate_authz_entry.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/tests/tests_datastores/databricks/mocks.py` & `udps-0.1.34/tests/tests_datastores/databricks/mocks.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/tests/tests_datastores/databricks/test_analyzer.py` & `udps-0.1.34/tests/tests_datastores/databricks/test_analyzer.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/tests/tests_datastores/mongodb/test_atlas_build_custom_role_from_response.py` & `udps-0.1.34/tests/tests_datastores/mongodb/test_atlas_build_custom_role_from_response.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/tests/tests_datastores/mongodb/test_atlas_organization_users.py` & `udps-0.1.34/tests/tests_datastores/mongodb/test_atlas_organization_users.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/tests/tests_datastores/mongodb/test_mongodb.py` & `udps-0.1.34/tests/tests_datastores/mongodb/test_mongodb.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/tests/tests_datastores/postgres/mocks/postgres_mock_connector.py` & `udps-0.1.34/tests/tests_datastores/postgres/mocks/postgres_mock_connector.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/tests/tests_datastores/postgres/test_postgress_analyzer.py` & `udps-0.1.34/tests/tests_datastores/postgres/test_postgress_analyzer.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/tests/tests_datastores/redshift/test_redshift.py` & `udps-0.1.34/tests/tests_datastores/redshift/test_redshift.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/tests/tests_datastores/snowflake/test_snowflake_analyzer.py` & `udps-0.1.34/tests/tests_datastores/snowflake/test_snowflake_analyzer.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/universal_data_permissions_scanner/__init__.py` & `udps-0.1.34/universal_data_permissions_scanner/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Top-level package for authz-analyzer."""
 
 __author__ = """SatoriCyber"""
 __email__ = 'contact@satoricyber.com'
-__version__ = '0.1.33'
+__version__ = '0.1.34'
 
 from universal_data_permissions_scanner.datastores.aws.analyzer import AwsAssumeRoleInput, AWSAuthzAnalyzer  # type: ignore
 from universal_data_permissions_scanner.datastores.aws.analyzer.redshift.analyzer import RedshiftAuthzAnalyzer  # type: ignore
 from universal_data_permissions_scanner.datastores.bigquery.analyzer import BigQueryAuthzAnalyzer  # type: ignore
 from universal_data_permissions_scanner.datastores.databricks.analyzer import DatabricksAuthzAnalyzer  # type: ignore
 from universal_data_permissions_scanner.datastores.mongodb.analyzer import MongoDBAuthzAnalyzer  # type: ignore
 from universal_data_permissions_scanner.datastores.mongodb.atlas.analyzer import MongoDBAtlasAuthzAnalyzer  # type: ignore
```

### Comparing `udps-0.1.33/universal_data_permissions_scanner/cli.py` & `udps-0.1.34/universal_data_permissions_scanner/cli.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/universal_data_permissions_scanner/datastores/aws/__init__.py` & `udps-0.1.34/universal_data_permissions_scanner/datastores/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/universal_data_permissions_scanner/datastores/aws/analyzer/analyzer.py` & `udps-0.1.34/universal_data_permissions_scanner/datastores/aws/analyzer/analyzer.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/universal_data_permissions_scanner/datastores/aws/analyzer/exporter.py` & `udps-0.1.34/universal_data_permissions_scanner/datastores/aws/analyzer/exporter.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/analyzer.py` & `udps-0.1.34/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/analyzer.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/exporter.py` & `udps-0.1.34/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/exporter.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/model.py` & `udps-0.1.34/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/model.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/service.py` & `udps-0.1.34/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/service.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/actions/actions_resolver.py` & `udps-0.1.34/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/actions/actions_resolver.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/actions/aws_actions.py` & `udps-0.1.34/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/actions/aws_actions.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/iam_entities.py` & `udps-0.1.34/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/iam_entities.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/iam_groups.py` & `udps-0.1.34/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/iam_groups.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/iam_policies.py` & `udps-0.1.34/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/iam_policies.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/iam_roles.py` & `udps-0.1.34/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/iam_roles.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/iam_users.py` & `udps-0.1.34/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/iam_users.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/policy/policy_document.py` & `udps-0.1.34/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/policy/policy_document.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/policy/policy_document_resolver.py` & `udps-0.1.34/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/policy/policy_document_resolver.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam_identity_center/iam_identity_center_entities.py` & `udps-0.1.34/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam_identity_center/iam_identity_center_entities.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam_identity_center/iam_identity_center_groups.py` & `udps-0.1.34/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam_identity_center/iam_identity_center_groups.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam_identity_center/iam_identity_center_users.py` & `udps-0.1.34/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam_identity_center/iam_identity_center_users.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam_identity_center/permission_sets.py` & `udps-0.1.34/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam_identity_center/permission_sets.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/logger.py` & `udps-0.1.34/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/logger.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/policy_evaluation/policy_evaluation.py` & `udps-0.1.34/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/policy_evaluation/policy_evaluation.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/principals/aws_principals.py` & `udps-0.1.34/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/principals/aws_principals.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/principals/no_entity_principal.py` & `udps-0.1.34/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/principals/no_entity_principal.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/principals/principal.py` & `udps-0.1.34/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/principals/principal.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/principals/principals_resolver.py` & `udps-0.1.34/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/principals/principals_resolver.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp.py` & `udps-0.1.34/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_allowed_lines/allowed_line.py` & `udps-0.1.34/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_allowed_lines/allowed_line.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_allowed_lines/allowed_line_node_notes.py` & `udps-0.1.34/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_allowed_lines/allowed_line_node_notes.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_allowed_lines/allowed_line_nodes_base.py` & `udps-0.1.34/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_allowed_lines/allowed_line_nodes_base.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_allowed_lines/allowed_lines_resolver.py` & `udps-0.1.34/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_allowed_lines/allowed_lines_resolver.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_allowed_lines/allowed_lines_resolver_result.py` & `udps-0.1.34/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_allowed_lines/allowed_lines_resolver_result.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_models/__init__.py` & `udps-0.1.34/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_models/__init__.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_models/ptrp_model.py` & `udps-0.1.34/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_models/ptrp_model.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/resources/account_resources.py` & `udps-0.1.34/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/resources/account_resources.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/resources/resources_resolver.py` & `udps-0.1.34/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/resources/resources_resolver.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/__init__.py` & `udps-0.1.34/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/__init__.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/assume_role/assume_role_actions.py` & `udps-0.1.34/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/assume_role/assume_role_actions.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/assume_role/assume_role_resources.py` & `udps-0.1.34/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/assume_role/assume_role_resources.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/assume_role/assume_role_service.py` & `udps-0.1.34/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/assume_role/assume_role_service.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/federated_user/federated_user_actions.py` & `udps-0.1.34/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/federated_user/federated_user_actions.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/federated_user/federated_user_resources.py` & `udps-0.1.34/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/federated_user/federated_user_resources.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/federated_user/federated_user_service.py` & `udps-0.1.34/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/federated_user/federated_user_service.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/resolved_stmt.py` & `udps-0.1.34/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/resolved_stmt.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/s3/bucket.py` & `udps-0.1.34/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/s3/bucket.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/s3/bucket_acl.py` & `udps-0.1.34/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/s3/bucket_acl.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/s3/s3_actions.py` & `udps-0.1.34/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/s3/s3_actions.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/s3/s3_resources.py` & `udps-0.1.34/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/s3/s3_resources.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/s3/s3_service.py` & `udps-0.1.34/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/s3/s3_service.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/service_action_type.py` & `udps-0.1.34/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/service_action_type.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/service_actions_resolver_base.py` & `udps-0.1.34/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/service_actions_resolver_base.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/service_resource_base.py` & `udps-0.1.34/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/service_resource_base.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/service_resource_type.py` & `udps-0.1.34/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/service_resource_type.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/service_resources_resolver_base.py` & `udps-0.1.34/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/service_resources_resolver_base.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/utils/create_session.py` & `udps-0.1.34/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/utils/create_session.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/utils/pagination.py` & `udps-0.1.34/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/utils/pagination.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/utils/regex_subset.py` & `udps-0.1.34/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/utils/regex_subset.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/universal_data_permissions_scanner/datastores/bigquery/analyzer.py` & `udps-0.1.34/universal_data_permissions_scanner/datastores/bigquery/analyzer.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/universal_data_permissions_scanner/datastores/bigquery/policy_tree.py` & `udps-0.1.34/universal_data_permissions_scanner/datastores/bigquery/policy_tree.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/universal_data_permissions_scanner/datastores/bigquery/service.py` & `udps-0.1.34/universal_data_permissions_scanner/datastores/bigquery/service.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/universal_data_permissions_scanner/datastores/databricks/analyzer.py` & `udps-0.1.34/universal_data_permissions_scanner/datastores/databricks/analyzer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from dataclasses import dataclass
-from http.client import UNAUTHORIZED
+from http.client import FORBIDDEN, UNAUTHORIZED
 from logging import Logger
 from typing import Any, Optional
 
 import requests
 
 from databricks_cli.sdk.api_client import ApiClient  # type: ignore
 from databricks_cli.unity_catalog.uc_service import UnityCatalogService  # type: ignore
@@ -94,32 +94,37 @@
             unity_catalog_service=unity_catalog_service,
             scim_service=scim_service,
             metastore_id=metastore_id,
         )
 
     def run(self):
         """Run the analyzer"""
-        self.logger.debug("Starting to analyzer Databricks, fetching users")
-        users = self.scim_service.list_users()["Resources"]
-        self.logger.debug("fetching groups")
-        groups = self.scim_service.list_groups()["Resources"]
-        self.logger.debug("fetching service principals")
-        service_principal = self.scim_service.list_service_principals()["Resources"]
-
-        identities = Identities.build_from_databricks_response(self.logger, users, groups, service_principal)
-        self.logger.info("Starting to analyze catalogs")
-        catalog: CatalogList
-        for catalog in self.unity_catalog_service.list_catalogs()["catalogs"]:  # type: ignore
-            if self.metastore_id is not None and catalog["metastore_id"] != self.metastore_id:
-                self.logger.error("Catalog %s does not match metastore_id %s", catalog["name"], self.metastore_id)
-                continue
-            self.logger.info("Analyzing catalog: %s", catalog["name"])
-            for entry in self._iter_permissions_catalog(catalog, identities):
-                self.logger.debug("Writing entry: %s", entry)
-                self.writer.write_entry(entry)
+        try:
+            self.logger.debug("Starting to analyzer Databricks, fetching users")
+            users = self.scim_service.list_users()["Resources"]
+            self.logger.debug("fetching groups")
+            groups = self.scim_service.list_groups()["Resources"]
+            self.logger.debug("fetching service principals")
+            service_principal = self.scim_service.list_service_principals()["Resources"]
+
+            identities = Identities.build_from_databricks_response(self.logger, users, groups, service_principal)
+            self.logger.info("Starting to analyze catalogs")
+            catalog: CatalogList
+            for catalog in self.unity_catalog_service.list_catalogs()["catalogs"]:  # type: ignore
+                if self.metastore_id is not None and catalog["metastore_id"] != self.metastore_id:
+                    self.logger.error("Catalog %s does not match metastore_id %s", catalog["name"], self.metastore_id)
+                    continue
+                self.logger.info("Analyzing catalog: %s", catalog["name"])
+                for entry in self._iter_permissions_catalog(catalog, identities):
+                    self.logger.debug("Writing entry: %s", entry)
+                    self.writer.write_entry(entry)
+        except requests.exceptions.HTTPError as err:
+            if err.response.status_code == FORBIDDEN:
+                raise ConnectionFailure() from err
+            raise err
 
     def _iter_permissions_catalog(self, catalog: CatalogList, identities: Identities):
         catalog_node = CatalogNode(self.logger, catalog["name"], catalog["owner"])
         self.logger.debug("Starting to analyze schemas")
         schema: Schema
         for schema in self.unity_catalog_service.list_schemas(catalog["name"])["schemas"]:  # type: ignore
             self.logger.info("Analyzing schema: %s", schema["name"])
```

### Comparing `udps-0.1.33/universal_data_permissions_scanner/datastores/databricks/identities.py` & `udps-0.1.34/universal_data_permissions_scanner/datastores/databricks/identities.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/universal_data_permissions_scanner/datastores/databricks/model.py` & `udps-0.1.34/universal_data_permissions_scanner/datastores/databricks/model.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/universal_data_permissions_scanner/datastores/databricks/policy_tree.py` & `udps-0.1.34/universal_data_permissions_scanner/datastores/databricks/policy_tree.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/universal_data_permissions_scanner/datastores/databricks/service/authentication/authentication.py` & `udps-0.1.34/universal_data_permissions_scanner/datastores/databricks/service/authentication/authentication.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/universal_data_permissions_scanner/datastores/databricks/service/authentication/oauth.py` & `udps-0.1.34/universal_data_permissions_scanner/datastores/databricks/service/authentication/oauth.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/universal_data_permissions_scanner/datastores/databricks/service/model.py` & `udps-0.1.34/universal_data_permissions_scanner/datastores/databricks/service/model.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/universal_data_permissions_scanner/datastores/databricks/service/scim.py` & `udps-0.1.34/universal_data_permissions_scanner/datastores/databricks/service/scim.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/universal_data_permissions_scanner/datastores/mongodb/analyzer.py` & `udps-0.1.34/universal_data_permissions_scanner/datastores/mongodb/analyzer.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/universal_data_permissions_scanner/datastores/mongodb/atlas/analyzer.py` & `udps-0.1.34/universal_data_permissions_scanner/datastores/mongodb/atlas/analyzer.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/universal_data_permissions_scanner/datastores/mongodb/atlas/exceptions.py` & `udps-0.1.34/universal_data_permissions_scanner/datastores/mongodb/atlas/exceptions.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/universal_data_permissions_scanner/datastores/mongodb/atlas/model.py` & `udps-0.1.34/universal_data_permissions_scanner/datastores/mongodb/atlas/model.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/universal_data_permissions_scanner/datastores/mongodb/atlas/permission_resolvers.py` & `udps-0.1.34/universal_data_permissions_scanner/datastores/mongodb/atlas/permission_resolvers.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/universal_data_permissions_scanner/datastores/mongodb/atlas/service.py` & `udps-0.1.34/universal_data_permissions_scanner/datastores/mongodb/atlas/service.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/universal_data_permissions_scanner/datastores/mongodb/atlas/service_model.py` & `udps-0.1.34/universal_data_permissions_scanner/datastores/mongodb/atlas/service_model.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/universal_data_permissions_scanner/datastores/mongodb/model.py` & `udps-0.1.34/universal_data_permissions_scanner/datastores/mongodb/model.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/universal_data_permissions_scanner/datastores/mongodb/resolvers.py` & `udps-0.1.34/universal_data_permissions_scanner/datastores/mongodb/resolvers.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/universal_data_permissions_scanner/datastores/mongodb/service.py` & `udps-0.1.34/universal_data_permissions_scanner/datastores/mongodb/service.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/universal_data_permissions_scanner/datastores/mongodb/service_model.py` & `udps-0.1.34/universal_data_permissions_scanner/datastores/mongodb/service_model.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/universal_data_permissions_scanner/datastores/postgres/analyzer.py` & `udps-0.1.34/universal_data_permissions_scanner/datastores/postgres/analyzer.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/universal_data_permissions_scanner/datastores/postgres/database_query_results.py` & `udps-0.1.34/universal_data_permissions_scanner/datastores/postgres/database_query_results.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/universal_data_permissions_scanner/datastores/postgres/deployment.py` & `udps-0.1.34/universal_data_permissions_scanner/datastores/postgres/deployment.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/universal_data_permissions_scanner/datastores/postgres/exporter.py` & `udps-0.1.34/universal_data_permissions_scanner/datastores/postgres/exporter.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/universal_data_permissions_scanner/datastores/postgres/model.py` & `udps-0.1.34/universal_data_permissions_scanner/datastores/postgres/model.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/universal_data_permissions_scanner/datastores/snowflake/analyzer.py` & `udps-0.1.34/universal_data_permissions_scanner/datastores/snowflake/analyzer.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/universal_data_permissions_scanner/datastores/snowflake/commands/user_grants.sql` & `udps-0.1.34/universal_data_permissions_scanner/datastores/snowflake/commands/user_grants.sql`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/universal_data_permissions_scanner/datastores/snowflake/exporter.py` & `udps-0.1.34/universal_data_permissions_scanner/datastores/snowflake/exporter.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/universal_data_permissions_scanner/datastores/snowflake/model.py` & `udps-0.1.34/universal_data_permissions_scanner/datastores/snowflake/model.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/universal_data_permissions_scanner/datastores/snowflake/service.py` & `udps-0.1.34/universal_data_permissions_scanner/datastores/snowflake/service.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/universal_data_permissions_scanner/main.py` & `udps-0.1.34/universal_data_permissions_scanner/main.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/universal_data_permissions_scanner/models/model.py` & `udps-0.1.34/universal_data_permissions_scanner/models/model.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/universal_data_permissions_scanner/utils/logger.py` & `udps-0.1.34/universal_data_permissions_scanner/utils/logger.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/universal_data_permissions_scanner/writers/base_writers.py` & `udps-0.1.34/universal_data_permissions_scanner/writers/base_writers.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/universal_data_permissions_scanner/writers/csv_writer.py` & `udps-0.1.34/universal_data_permissions_scanner/writers/csv_writer.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/universal_data_permissions_scanner/writers/get_writers.py` & `udps-0.1.34/universal_data_permissions_scanner/writers/get_writers.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/universal_data_permissions_scanner/writers/multi_json_exporter.py` & `udps-0.1.34/universal_data_permissions_scanner/writers/multi_json_exporter.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.33/PKG-INFO` & `udps-0.1.34/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: udps
-Version: 0.1.33
+Version: 0.1.34
 Summary: Analyze authorization.
 Home-page: https://github.com/satoricyber/universal-data-permissions-scanner
 Author: SatoriCyber
 Requires-Python: >=3.8.1,<3.12
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
 Provides-Extra: release
 Provides-Extra: test
-Requires-Dist: black (>=22.12.0,<23.0.0) ; extra == "test"
+Requires-Dist: black (>=24.3.0,<25.0.0) ; extra == "test"
 Requires-Dist: boto3 (>=1.26.27,<2.0.0)
 Requires-Dist: bump2version (>=1.0.1,<2.0.0) ; extra == "test"
 Requires-Dist: click (==8.1.3)
 Requires-Dist: databricks-cli (>=0.17.4,<0.18.0)
 Requires-Dist: google-api-python-client (>=2.66.0,<2.67.0)
 Requires-Dist: google-api-python-client-stubs (>=1.13.0,<2.0.0) ; extra == "test"
 Requires-Dist: google-cloud-bigquery (>=3.4.2)
```

