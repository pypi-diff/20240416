# Comparing `tmp/edgeimpulse_api-1.49.5.tar.gz` & `tmp/edgeimpulse_api-1.49.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edgeimpulse_api-1.49.5.tar", max compression
+gzip compressed data, was "edgeimpulse_api-1.49.6.tar", max compression
```

## Comparing `edgeimpulse_api-1.49.5.tar` & `edgeimpulse_api-1.49.6.tar`

### file list

```diff
@@ -1,915 +1,925 @@
--rw-r--r--   0        0        0      377 2024-04-15 13:10:05.598443 edgeimpulse_api-1.49.5/README.md
--rw-r--r--   0        0        0    87564 2024-04-15 13:10:42.038120 edgeimpulse_api-1.49.5/edgeimpulse_api/__init__.py
--rw-r--r--   0        0        0     2172 2024-04-15 13:10:05.602443 edgeimpulse_api-1.49.5/edgeimpulse_api/api/__init__.py
--rw-r--r--   0        0        0   386649 2024-04-15 13:10:05.602443 edgeimpulse_api-1.49.5/edgeimpulse_api/api/admin_api.py
--rw-r--r--   0        0        0    11231 2024-04-15 13:10:05.606443 edgeimpulse_api-1.49.5/edgeimpulse_api/api/auth_api.py
--rw-r--r--   0        0        0     6235 2024-04-15 13:10:05.606443 edgeimpulse_api-1.49.5/edgeimpulse_api/api/cdn_api.py
--rw-r--r--   0        0        0    59980 2024-04-15 13:10:05.606443 edgeimpulse_api-1.49.5/edgeimpulse_api/api/classify_api.py
--rw-r--r--   0        0        0    72480 2024-04-15 13:10:05.610442 edgeimpulse_api-1.49.5/edgeimpulse_api/api/deployment_api.py
--rw-r--r--   0        0        0    38974 2024-04-15 13:10:05.610442 edgeimpulse_api-1.49.5/edgeimpulse_api/api/devices_api.py
--rw-r--r--   0        0        0   139045 2024-04-15 13:10:05.610442 edgeimpulse_api-1.49.5/edgeimpulse_api/api/dsp_api.py
--rw-r--r--   0        0        0    19442 2024-04-15 13:10:05.610442 edgeimpulse_api-1.49.5/edgeimpulse_api/api/email_verification_api.py
--rw-r--r--   0        0        0     6435 2024-04-15 13:10:05.610442 edgeimpulse_api-1.49.5/edgeimpulse_api/api/export_api.py
--rw-r--r--   0        0        0     5996 2024-04-15 13:10:05.614442 edgeimpulse_api-1.49.5/edgeimpulse_api/api/feature_flags_api.py
--rw-r--r--   0        0        0    11921 2024-04-15 13:10:05.614442 edgeimpulse_api-1.49.5/edgeimpulse_api/api/health_api.py
--rw-r--r--   0        0        0    49621 2024-04-15 13:10:05.614442 edgeimpulse_api-1.49.5/edgeimpulse_api/api/impulse_api.py
--rw-r--r--   0        0        0   238420 2024-04-15 13:10:05.614442 edgeimpulse_api-1.49.5/edgeimpulse_api/api/jobs_api.py
--rw-r--r--   0        0        0   154112 2024-04-15 13:10:05.614442 edgeimpulse_api-1.49.5/edgeimpulse_api/api/learn_api.py
--rw-r--r--   0        0        0     6483 2024-04-15 13:10:05.614442 edgeimpulse_api-1.49.5/edgeimpulse_api/api/login_api.py
--rw-r--r--   0        0        0    17897 2024-04-15 13:10:05.614442 edgeimpulse_api-1.49.5/edgeimpulse_api/api/metrics_api.py
--rw-r--r--   0        0        0    85275 2024-04-15 13:10:05.614442 edgeimpulse_api-1.49.5/edgeimpulse_api/api/optimization_api.py
--rw-r--r--   0        0        0   197840 2024-04-15 13:10:05.614442 edgeimpulse_api-1.49.5/edgeimpulse_api/api/organization_blocks_api.py
--rw-r--r--   0        0        0    92715 2024-04-15 13:10:05.614442 edgeimpulse_api-1.49.5/edgeimpulse_api/api/organization_create_project_api.py
--rw-r--r--   0        0        0   331750 2024-04-15 13:10:05.618442 edgeimpulse_api-1.49.5/edgeimpulse_api/api/organization_data_api.py
--rw-r--r--   0        0        0    80882 2024-04-15 13:10:05.618442 edgeimpulse_api-1.49.5/edgeimpulse_api/api/organization_data_campaigns_api.py
--rw-r--r--   0        0        0    58218 2024-04-15 13:10:05.618442 edgeimpulse_api-1.49.5/edgeimpulse_api/api/organization_jobs_api.py
--rw-r--r--   0        0        0    53291 2024-04-15 13:10:05.618442 edgeimpulse_api-1.49.5/edgeimpulse_api/api/organization_pipelines_api.py
--rw-r--r--   0        0        0    45490 2024-04-15 13:10:05.618442 edgeimpulse_api-1.49.5/edgeimpulse_api/api/organization_portals_api.py
--rw-r--r--   0        0        0   505317 2024-04-15 13:10:05.622442 edgeimpulse_api-1.49.5/edgeimpulse_api/api/organizations_api.py
--rw-r--r--   0        0        0    54671 2024-04-15 13:10:05.622442 edgeimpulse_api-1.49.5/edgeimpulse_api/api/performance_calibration_api.py
--rw-r--r--   0        0        0   270960 2024-04-15 13:10:05.626443 edgeimpulse_api-1.49.5/edgeimpulse_api/api/projects_api.py
--rw-r--r--   0        0        0   414581 2024-04-15 13:10:05.630442 edgeimpulse_api-1.49.5/edgeimpulse_api/api/raw_data_api.py
--rw-r--r--   0        0        0    35671 2024-04-15 13:10:05.630442 edgeimpulse_api-1.49.5/edgeimpulse_api/api/themes_api.py
--rw-r--r--   0        0        0    43486 2024-04-15 13:10:05.630442 edgeimpulse_api-1.49.5/edgeimpulse_api/api/third_party_auth_api.py
--rw-r--r--   0        0        0    45692 2024-04-15 13:10:05.630442 edgeimpulse_api-1.49.5/edgeimpulse_api/api/upload_portal_api.py
--rw-r--r--   0        0        0   247228 2024-04-15 13:10:05.630442 edgeimpulse_api-1.49.5/edgeimpulse_api/api/user_api.py
--rw-r--r--   0        0        0    42135 2024-04-15 13:10:05.630442 edgeimpulse_api-1.49.5/edgeimpulse_api/api/whitelabels_api.py
--rw-r--r--   0        0        0    29331 2024-04-15 13:10:05.630442 edgeimpulse_api-1.49.5/edgeimpulse_api/api_client.py
--rw-r--r--   0        0        0    15659 2024-04-15 13:10:05.630442 edgeimpulse_api-1.49.5/edgeimpulse_api/configuration.py
--rw-r--r--   0        0        0     5113 2024-04-15 13:10:05.630442 edgeimpulse_api-1.49.5/edgeimpulse_api/exceptions.py
--rw-r--r--   0        0        0    84939 2024-04-15 13:10:05.634442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/__init__.py
--rw-r--r--   0        0        0     2897 2024-04-15 13:10:05.634442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/activate_user_by_third_party_activation_code_request.py
--rw-r--r--   0        0        0     1982 2024-04-15 13:10:05.634442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/activate_user_or_verify_email_request.py
--rw-r--r--   0        0        0     2052 2024-04-15 13:10:05.634442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/add_api_key_request.py
--rw-r--r--   0        0        0     1963 2024-04-15 13:10:05.634442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/add_collaborator_request.py
--rw-r--r--   0        0        0     2223 2024-04-15 13:10:05.634442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/add_hmac_key_request.py
--rw-r--r--   0        0        0     2299 2024-04-15 13:10:05.634442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/add_member_request.py
--rw-r--r--   0        0        0     2418 2024-04-15 13:10:05.634442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/add_organization_api_key_request.py
--rw-r--r--   0        0        0     2122 2024-04-15 13:10:05.634442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/add_organization_api_key_request_all_of.py
--rw-r--r--   0        0        0     2806 2024-04-15 13:10:05.634442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/add_organization_bucket_request.py
--rw-r--r--   0        0        0     2794 2024-04-15 13:10:05.634442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/add_organization_data_campaign_dashboard_request.py
--rw-r--r--   0        0        0     2469 2024-04-15 13:10:05.634442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/add_organization_data_campaign_dashboard_response.py
--rw-r--r--   0        0        0     2152 2024-04-15 13:10:05.634442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/add_organization_data_campaign_dashboard_response_all_of.py
--rw-r--r--   0        0        0     4230 2024-04-15 13:10:05.634442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/add_organization_data_campaign_request.py
--rw-r--r--   0        0        0     2359 2024-04-15 13:10:05.634442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/add_organization_data_campaign_response.py
--rw-r--r--   0        0        0     2042 2024-04-15 13:10:05.634442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/add_organization_data_campaign_response_all_of.py
--rw-r--r--   0        0        0     2269 2024-04-15 13:10:05.634442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/add_organization_deploy_block_response.py
--rw-r--r--   0        0        0     2816 2024-04-15 13:10:05.634442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/add_organization_dsp_block_request.py
--rw-r--r--   0        0        0     2248 2024-04-15 13:10:05.634442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/add_organization_dsp_block_response.py
--rw-r--r--   0        0        0     2054 2024-04-15 13:10:05.634442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/add_organization_secret_request.py
--rw-r--r--   0        0        0     2266 2024-04-15 13:10:05.634442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/add_organization_secret_response.py
--rw-r--r--   0        0        0     1949 2024-04-15 13:10:05.634442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/add_organization_secret_response_all_of.py
--rw-r--r--   0        0        0     4885 2024-04-15 13:10:05.634442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/add_organization_transfer_learning_block_request.py
--rw-r--r--   0        0        0     2339 2024-04-15 13:10:05.634442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/add_organization_transfer_learning_block_response.py
--rw-r--r--   0        0        0     6169 2024-04-15 13:10:05.638442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/add_organization_transformation_block_request.py
--rw-r--r--   0        0        0     2325 2024-04-15 13:10:05.638442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/add_organization_transformation_block_response.py
--rw-r--r--   0        0        0     2001 2024-04-15 13:10:05.638442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/add_organization_transformation_block_response_all_of.py
--rw-r--r--   0        0        0     2659 2024-04-15 13:10:05.638442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/add_project_api_key_request.py
--rw-r--r--   0        0        0     2370 2024-04-15 13:10:05.638442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/add_project_api_key_request_all_of.py
--rw-r--r--   0        0        0     1940 2024-04-15 13:10:05.638442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/admin_add_disallowed_email_domain_request.py
--rw-r--r--   0        0        0     1961 2024-04-15 13:10:05.638442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/admin_add_or_update_sso_domain_id_ps_request.py
--rw-r--r--   0        0        0     2661 2024-04-15 13:10:05.638442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/admin_add_organization_api_key_request.py
--rw-r--r--   0        0        0     2542 2024-04-15 13:10:05.638442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/admin_add_organization_user_request.py
--rw-r--r--   0        0        0     2246 2024-04-15 13:10:05.638442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/admin_add_organization_user_request_all_of.py
--rw-r--r--   0        0        0     2344 2024-04-15 13:10:05.638442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/admin_add_project_api_key_request.py
--rw-r--r--   0        0        0     2044 2024-04-15 13:10:05.638442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/admin_add_project_api_key_request_all_of.py
--rw-r--r--   0        0        0     2146 2024-04-15 13:10:05.638442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/admin_add_project_user_request.py
--rw-r--r--   0        0        0     2097 2024-04-15 13:10:05.638442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/admin_add_user_request.py
--rw-r--r--   0        0        0     5903 2024-04-15 13:10:05.638442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/admin_api_organization.py
--rw-r--r--   0        0        0     2396 2024-04-15 13:10:05.638442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/admin_api_organization_all_of.py
--rw-r--r--   0        0        0     3259 2024-04-15 13:10:05.642442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/admin_api_project.py
--rw-r--r--   0        0        0     7087 2024-04-15 13:10:05.642442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/admin_api_user.py
--rw-r--r--   0        0        0     5318 2024-04-15 13:10:05.646442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/admin_api_user_all_of.py
--rw-r--r--   0        0        0     2386 2024-04-15 13:10:05.650442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/admin_create_organization_data_export_request.py
--rw-r--r--   0        0        0     2262 2024-04-15 13:10:05.650442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/admin_create_organization_request.py
--rw-r--r--   0        0        0     2718 2024-04-15 13:10:05.650442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/admin_create_project_request.py
--rw-r--r--   0        0        0     1905 2024-04-15 13:10:05.650442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/admin_enable_feature_request.py
--rw-r--r--   0        0        0     2546 2024-04-15 13:10:05.650442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/admin_get_data_migration_response.py
--rw-r--r--   0        0        0     2222 2024-04-15 13:10:05.650442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/admin_get_data_migration_response_all_of.py
--rw-r--r--   0        0        0     2735 2024-04-15 13:10:05.650442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/admin_get_data_migrations_response.py
--rw-r--r--   0        0        0     2428 2024-04-15 13:10:05.650442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/admin_get_data_migrations_response_all_of.py
--rw-r--r--   0        0        0     2318 2024-04-15 13:10:05.650442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/admin_get_disallowed_email_domains_response.py
--rw-r--r--   0        0        0     2022 2024-04-15 13:10:05.650442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/admin_get_disallowed_email_domains_response_all_of.py
--rw-r--r--   0        0        0     2217 2024-04-15 13:10:05.650442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/admin_get_metrics_response.py
--rw-r--r--   0        0        0     1910 2024-04-15 13:10:05.650442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/admin_get_metrics_response_all_of.py
--rw-r--r--   0        0        0     3148 2024-04-15 13:10:05.650442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/admin_get_organization_compute_time_usage_response.py
--rw-r--r--   0        0        0     2647 2024-04-15 13:10:05.650442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/admin_get_organization_usage_report_response.py
--rw-r--r--   0        0        0     2323 2024-04-15 13:10:05.650442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/admin_get_organization_usage_report_response_all_of.py
--rw-r--r--   0        0        0     3029 2024-04-15 13:10:05.650442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/admin_get_organization_usage_reports_response.py
--rw-r--r--   0        0        0     2729 2024-04-15 13:10:05.650442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/admin_get_organization_usage_reports_response_all_of.py
--rw-r--r--   0        0        0     3046 2024-04-15 13:10:05.650442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/admin_get_organizations_response.py
--rw-r--r--   0        0        0     2746 2024-04-15 13:10:05.650442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/admin_get_organizations_response_all_of.py
--rw-r--r--   0        0        0     3409 2024-04-15 13:10:05.650442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/admin_get_organizations_response_all_of_organizations.py
--rw-r--r--   0        0        0     2243 2024-04-15 13:10:05.650442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/admin_get_sso_domain_id_ps_response.py
--rw-r--r--   0        0        0     1947 2024-04-15 13:10:05.650442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/admin_get_sso_domain_id_ps_response_all_of.py
--rw-r--r--   0        0        0     2914 2024-04-15 13:10:05.650442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/admin_get_sso_settings_response.py
--rw-r--r--   0        0        0     2614 2024-04-15 13:10:05.650442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/admin_get_sso_settings_response_all_of.py
--rw-r--r--   0        0        0     2096 2024-04-15 13:10:05.650442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/admin_get_sso_settings_response_all_of_sso_whitelist.py
--rw-r--r--   0        0        0     2208 2024-04-15 13:10:05.650442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/admin_get_user_ids_response.py
--rw-r--r--   0        0        0     1901 2024-04-15 13:10:05.650442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/admin_get_user_ids_response_all_of.py
--rw-r--r--   0        0        0     2245 2024-04-15 13:10:05.650442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/admin_get_user_metrics_response.py
--rw-r--r--   0        0        0     2452 2024-04-15 13:10:05.650442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/admin_get_user_response.py
--rw-r--r--   0        0        0     2128 2024-04-15 13:10:05.650442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/admin_get_user_response_all_of.py
--rw-r--r--   0        0        0     2507 2024-04-15 13:10:05.650442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/admin_get_user_trial_response.py
--rw-r--r--   0        0        0     2183 2024-04-15 13:10:05.650442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/admin_get_user_trial_response_all_of.py
--rw-r--r--   0        0        0     2807 2024-04-15 13:10:05.650442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/admin_get_users_response.py
--rw-r--r--   0        0        0     2500 2024-04-15 13:10:05.650442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/admin_get_users_response_all_of.py
--rw-r--r--   0        0        0     2878 2024-04-15 13:10:05.654442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/admin_get_users_response_all_of_users.py
--rw-r--r--   0        0        0     2445 2024-04-15 13:10:05.654442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/admin_list_projects.py
--rw-r--r--   0        0        0     2836 2024-04-15 13:10:05.654442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/admin_list_projects_response.py
--rw-r--r--   0        0        0     4245 2024-04-15 13:10:05.654442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/admin_organization_info_response.py
--rw-r--r--   0        0        0     3084 2024-04-15 13:10:05.654442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/admin_organization_info_response_all_of.py
--rw-r--r--   0        0        0     2158 2024-04-15 13:10:05.654442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/admin_toggle_data_migration_request.py
--rw-r--r--   0        0        0     2397 2024-04-15 13:10:05.654442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/admin_update_organization_data_export_request.py
--rw-r--r--   0        0        0     3936 2024-04-15 13:10:05.654442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/admin_update_organization_request.py
--rw-r--r--   0        0        0     2015 2024-04-15 13:10:05.654442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/admin_update_user_permissions_request.py
--rw-r--r--   0        0        0     2830 2024-04-15 13:10:05.654442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/admin_update_user_request.py
--rw-r--r--   0        0        0     2532 2024-04-15 13:10:05.654442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/admin_update_user_trial_request.py
--rw-r--r--   0        0        0     2525 2024-04-15 13:10:05.654442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/akida_edge_learning_config.py
--rw-r--r--   0        0        0      512 2024-04-15 13:10:05.654442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/anomaly_capacity.py
--rw-r--r--   0        0        0     2512 2024-04-15 13:10:05.654442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/anomaly_gmm_metadata.py
--rw-r--r--   0        0        0     2212 2024-04-15 13:10:05.654442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/anomaly_gmm_metadata_all_of.py
--rw-r--r--   0        0        0     5499 2024-04-15 13:10:05.654442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/anomaly_model_metadata.py
--rw-r--r--   0        0        0     5221 2024-04-15 13:10:05.654442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/anomaly_model_metadata_all_of.py
--rw-r--r--   0        0        0     2151 2024-04-15 13:10:05.654442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/anomaly_model_metadata_all_of_clusters.py
--rw-r--r--   0        0        0     4079 2024-04-15 13:10:05.654442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/anomaly_response.py
--rw-r--r--   0        0        0     3812 2024-04-15 13:10:05.654442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/anomaly_response_all_of.py
--rw-r--r--   0        0        0     2044 2024-04-15 13:10:05.654442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/anomaly_response_all_of_axes.py
--rw-r--r--   0        0        0     3188 2024-04-15 13:10:05.658442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/anomaly_result.py
--rw-r--r--   0        0        0     3029 2024-04-15 13:10:05.658442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/anomaly_trained_features_response.py
--rw-r--r--   0        0        0     2729 2024-04-15 13:10:05.658442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/anomaly_trained_features_response_all_of.py
--rw-r--r--   0        0        0     2375 2024-04-15 13:10:05.658442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/anomaly_trained_features_response_all_of_data.py
--rw-r--r--   0        0        0     3358 2024-04-15 13:10:05.658442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/application_budget.py
--rw-r--r--   0        0        0      506 2024-04-15 13:10:05.658442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/augmentation_policy_image_enum.py
--rw-r--r--   0        0        0     3635 2024-04-15 13:10:05.658442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/augmentation_policy_spectrogram.py
--rw-r--r--   0        0        0     1895 2024-04-15 13:10:05.658442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/autotune_dsp_request.py
--rw-r--r--   0        0        0      505 2024-04-15 13:10:05.658442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/block_display_category.py
--rw-r--r--   0        0        0      560 2024-04-15 13:10:05.662442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/block_type.py
--rw-r--r--   0        0        0     2044 2024-04-15 13:10:05.662442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/bounding_box.py
--rw-r--r--   0        0        0     2151 2024-04-15 13:10:05.662442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/bounding_box_with_score.py
--rw-r--r--   0        0        0     2197 2024-04-15 13:10:05.662442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/build_on_device_model_request.py
--rw-r--r--   0        0        0     2433 2024-04-15 13:10:05.662442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/build_organization_on_device_model_request.py
--rw-r--r--   0        0        0     2459 2024-04-15 13:10:05.662442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/calculate_data_quality_metrics_request.py
--rw-r--r--   0        0        0     2041 2024-04-15 13:10:05.662442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/change_password_request.py
--rw-r--r--   0        0        0     3701 2024-04-15 13:10:05.662442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/classify_job_response.py
--rw-r--r--   0        0        0     3394 2024-04-15 13:10:05.662442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/classify_job_response_all_of.py
--rw-r--r--   0        0        0     3769 2024-04-15 13:10:05.662442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/classify_job_response_all_of_accuracy.py
--rw-r--r--   0        0        0     2055 2024-04-15 13:10:05.662442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/classify_job_response_all_of_accuracy_total_summary.py
--rw-r--r--   0        0        0     3255 2024-04-15 13:10:05.662442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/classify_job_response_page.py
--rw-r--r--   0        0        0     2948 2024-04-15 13:10:05.662442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/classify_job_response_page_all_of.py
--rw-r--r--   0        0        0     4026 2024-04-15 13:10:05.662442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/classify_sample_response.py
--rw-r--r--   0        0        0     3759 2024-04-15 13:10:05.662442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/classify_sample_response_all_of.py
--rw-r--r--   0        0        0     6252 2024-04-15 13:10:05.662442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/classify_sample_response_classification.py
--rw-r--r--   0        0        0     2755 2024-04-15 13:10:05.662442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/classify_sample_response_classification_details.py
--rw-r--r--   0        0        0     3816 2024-04-15 13:10:05.662442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/classify_sample_v2200_response.py
--rw-r--r--   0        0        0     3004 2024-04-15 13:10:05.662442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/convert_user_request.py
--rw-r--r--   0        0        0     3495 2024-04-15 13:10:05.662442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/cosine_similarity_data.py
--rw-r--r--   0        0        0     3114 2024-04-15 13:10:05.662442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/cosine_similarity_issue.py
--rw-r--r--   0        0        0     3241 2024-04-15 13:10:05.662442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/cosine_similarity_issue_issues_inner.py
--rw-r--r--   0        0        0     2484 2024-04-15 13:10:05.662442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/cosine_similarity_issue_issues_inner_windows_inner.py
--rw-r--r--   0        0        0     2183 2024-04-15 13:10:05.662442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/count_samples_response.py
--rw-r--r--   0        0        0     1859 2024-04-15 13:10:05.662442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/count_samples_response_all_of.py
--rw-r--r--   0        0        0     2255 2024-04-15 13:10:05.662442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/create_block_version_response.py
--rw-r--r--   0        0        0     1938 2024-04-15 13:10:05.662442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/create_block_version_response_all_of.py
--rw-r--r--   0        0        0     2404 2024-04-15 13:10:05.662442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/create_developer_profile_response.py
--rw-r--r--   0        0        0     2125 2024-04-15 13:10:05.662442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/create_developer_profile_response_all_of.py
--rw-r--r--   0        0        0     2387 2024-04-15 13:10:05.662442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/create_device_request.py
--rw-r--r--   0        0        0     2850 2024-04-15 13:10:05.662442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/create_enterprise_trial_response.py
--rw-r--r--   0        0        0     2319 2024-04-15 13:10:05.662442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/create_enterprise_trial_response_all_of.py
--rw-r--r--   0        0        0     6569 2024-04-15 13:10:05.662442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/create_enterprise_trial_user_request.py
--rw-r--r--   0        0        0     4092 2024-04-15 13:10:05.666442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/create_enterprise_trial_user_request_all_of.py
--rw-r--r--   0        0        0     2491 2024-04-15 13:10:05.666442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/create_evaluation_user_response.py
--rw-r--r--   0        0        0     2185 2024-04-15 13:10:05.666442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/create_evaluation_user_response_all_of.py
--rw-r--r--   0        0        0     2600 2024-04-15 13:10:05.666442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/create_organization_portal_request.py
--rw-r--r--   0        0        0     2830 2024-04-15 13:10:05.666442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/create_organization_portal_response.py
--rw-r--r--   0        0        0     2551 2024-04-15 13:10:05.666442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/create_organization_portal_response_all_of.py
--rw-r--r--   0        0        0     1990 2024-04-15 13:10:05.666442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/create_organization_request.py
--rw-r--r--   0        0        0     2454 2024-04-15 13:10:05.666442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/create_organization_response.py
--rw-r--r--   0        0        0     2148 2024-04-15 13:10:05.666442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/create_organization_response_all_of.py
--rw-r--r--   0        0        0     2155 2024-04-15 13:10:05.666442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/create_organization_usage_report_body.py
--rw-r--r--   0        0        0     2185 2024-04-15 13:10:05.666442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/create_pipeline_response.py
--rw-r--r--   0        0        0     2504 2024-04-15 13:10:05.666442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/create_project_request.py
--rw-r--r--   0        0        0     2378 2024-04-15 13:10:05.666442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/create_project_response.py
--rw-r--r--   0        0        0     2072 2024-04-15 13:10:05.666442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/create_project_response_all_of.py
--rw-r--r--   0        0        0     2276 2024-04-15 13:10:05.666442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/create_signed_upload_link_request.py
--rw-r--r--   0        0        0     2414 2024-04-15 13:10:05.666442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/create_signed_upload_link_response.py
--rw-r--r--   0        0        0     2135 2024-04-15 13:10:05.666442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/create_signed_upload_link_response_all_of.py
--rw-r--r--   0        0        0     2413 2024-04-15 13:10:05.666442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/create_third_party_auth_request.py
--rw-r--r--   0        0        0     2450 2024-04-15 13:10:05.666442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/create_third_party_auth_response.py
--rw-r--r--   0        0        0     2144 2024-04-15 13:10:05.666442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/create_third_party_auth_response_all_of.py
--rw-r--r--   0        0        0     4197 2024-04-15 13:10:05.666442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/create_user_request.py
--rw-r--r--   0        0        0     2393 2024-04-15 13:10:05.666442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/create_user_response.py
--rw-r--r--   0        0        0     2114 2024-04-15 13:10:05.666442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/create_user_response_all_of.py
--rw-r--r--   0        0        0     2919 2024-04-15 13:10:05.666442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/create_user_third_party_request.py
--rw-r--r--   0        0        0     2672 2024-04-15 13:10:05.666442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/create_user_third_party_response.py
--rw-r--r--   0        0        0     2393 2024-04-15 13:10:05.666442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/create_user_third_party_response_all_of.py
--rw-r--r--   0        0        0     4384 2024-04-15 13:10:05.666442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/create_whitelabel_request.py
--rw-r--r--   0        0        0     2438 2024-04-15 13:10:05.666442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/create_whitelabel_response.py
--rw-r--r--   0        0        0     2121 2024-04-15 13:10:05.666442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/create_whitelabel_response_all_of.py
--rw-r--r--   0        0        0     2094 2024-04-15 13:10:05.666442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/created_updated_by_user.py
--rw-r--r--   0        0        0     2051 2024-04-15 13:10:05.666442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/crop_sample_request.py
--rw-r--r--   0        0        0     2248 2024-04-15 13:10:05.666442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/crop_sample_response.py
--rw-r--r--   0        0        0     1943 2024-04-15 13:10:05.666442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/crop_sample_response_all_of.py
--rw-r--r--   0        0        0     2368 2024-04-15 13:10:05.666442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/cross_validation_data.py
--rw-r--r--   0        0        0     3412 2024-04-15 13:10:05.666442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/cross_validation_data_scores_inner.py
--rw-r--r--   0        0        0     4054 2024-04-15 13:10:05.666442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/data_campaign.py
--rw-r--r--   0        0        0     2989 2024-04-15 13:10:05.666442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/data_campaign_dashboard.py
--rw-r--r--   0        0        0     2786 2024-04-15 13:10:05.666442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/data_campaign_graph.py
--rw-r--r--   0        0        0     3352 2024-04-15 13:10:05.666442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/data_campaign_graph_x_data_inner.py
--rw-r--r--   0        0        0     2047 2024-04-15 13:10:05.666442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/data_campaign_graph_x_data_inner_values_inner.py
--rw-r--r--   0        0        0     1934 2024-04-15 13:10:05.666442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/data_campaign_link.py
--rw-r--r--   0        0        0     1957 2024-04-15 13:10:05.666442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/data_campaign_query.py
--rw-r--r--   0        0        0     3292 2024-04-15 13:10:05.666442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/data_explorer_predictions_response.py
--rw-r--r--   0        0        0     3003 2024-04-15 13:10:05.666442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/data_explorer_predictions_response_all_of.py
--rw-r--r--   0        0        0     2838 2024-04-15 13:10:05.666442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/data_explorer_settings.py
--rw-r--r--   0        0        0     2149 2024-04-15 13:10:05.666442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/dataset_ratio_data.py
--rw-r--r--   0        0        0     2111 2024-04-15 13:10:05.666442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/dataset_ratio_data_ratio.py
--rw-r--r--   0        0        0     1898 2024-04-15 13:10:05.666442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/delete_portal_file_request.py
--rw-r--r--   0        0        0     2230 2024-04-15 13:10:05.666442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/dependency_data.py
--rw-r--r--   0        0        0     2280 2024-04-15 13:10:05.666442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/deploy_pretrained_model_input_audio.py
--rw-r--r--   0        0        0     2408 2024-04-15 13:10:05.666442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/deploy_pretrained_model_input_image.py
--rw-r--r--   0        0        0     2155 2024-04-15 13:10:05.666442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/deploy_pretrained_model_input_other.py
--rw-r--r--   0        0        0     2484 2024-04-15 13:10:05.666442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/deploy_pretrained_model_input_time_series.py
--rw-r--r--   0        0        0     2344 2024-04-15 13:10:05.666442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/deploy_pretrained_model_model_classification.py
--rw-r--r--   0        0        0     2780 2024-04-15 13:10:05.666442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/deploy_pretrained_model_model_object_detection.py
--rw-r--r--   0        0        0     2200 2024-04-15 13:10:05.666442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/deploy_pretrained_model_model_regression.py
--rw-r--r--   0        0        0     4397 2024-04-15 13:10:05.666442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/deploy_pretrained_model_request.py
--rw-r--r--   0        0        0     2833 2024-04-15 13:10:05.666442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/deploy_pretrained_model_request_model_info.py
--rw-r--r--   0        0        0     8503 2024-04-15 13:10:05.666442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/deploy_pretrained_model_request_model_info_input.py
--rw-r--r--   0        0        0     8065 2024-04-15 13:10:05.666442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/deploy_pretrained_model_request_model_info_model.py
--rw-r--r--   0        0        0     5950 2024-04-15 13:10:05.666442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/deployment_target.py
--rw-r--r--   0        0        0     1926 2024-04-15 13:10:05.666442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/deployment_target_badge.py
--rw-r--r--   0        0        0      737 2024-04-15 13:10:05.666442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/deployment_target_engine.py
--rw-r--r--   0        0        0     2702 2024-04-15 13:10:05.666442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/deployment_targets_response.py
--rw-r--r--   0        0        0     2395 2024-04-15 13:10:05.666442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/deployment_targets_response_all_of.py
--rw-r--r--   0        0        0     2248 2024-04-15 13:10:05.666442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/development_board_created_response.py
--rw-r--r--   0        0        0     2032 2024-04-15 13:10:05.666442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/development_board_request.py
--rw-r--r--   0        0        0     2134 2024-04-15 13:10:05.666442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/development_board_request_update.py
--rw-r--r--   0        0        0     2113 2024-04-15 13:10:05.666442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/development_board_response.py
--rw-r--r--   0        0        0     2864 2024-04-15 13:10:05.666442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/development_boards_response.py
--rw-r--r--   0        0        0     2564 2024-04-15 13:10:05.666442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/development_boards_response_all_of.py
--rw-r--r--   0        0        0     2030 2024-04-15 13:10:05.666442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/development_keys.py
--rw-r--r--   0        0        0     2400 2024-04-15 13:10:05.666442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/development_keys_response.py
--rw-r--r--   0        0        0     3677 2024-04-15 13:10:05.666442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/device.py
--rw-r--r--   0        0        0     2199 2024-04-15 13:10:05.666442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/device_name_response.py
--rw-r--r--   0        0        0     1920 2024-04-15 13:10:05.666442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/device_name_response_all_of.py
--rw-r--r--   0        0        0     2231 2024-04-15 13:10:05.666442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/device_sensors_inner.py
--rw-r--r--   0        0        0     2094 2024-04-15 13:10:05.666442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/download.py
--rw-r--r--   0        0        0     1912 2024-04-15 13:10:05.666442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/download_portal_file_request.py
--rw-r--r--   0        0        0     2260 2024-04-15 13:10:05.666442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/download_portal_file_response.py
--rw-r--r--   0        0        0     1954 2024-04-15 13:10:05.666442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/download_portal_file_response_all_of.py
--rw-r--r--   0        0        0     2724 2024-04-15 13:10:05.666442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/dsp_autotuner_results.py
--rw-r--r--   0        0        0     2417 2024-04-15 13:10:05.666442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/dsp_autotuner_results_all_of.py
--rw-r--r--   0        0        0     1968 2024-04-15 13:10:05.666442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/dsp_autotuner_results_all_of_results.py
--rw-r--r--   0        0        0     3045 2024-04-15 13:10:05.670442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/dsp_block.py
--rw-r--r--   0        0        0     1834 2024-04-15 13:10:05.670442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/dsp_config_request.py
--rw-r--r--   0        0        0     3092 2024-04-15 13:10:05.670442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/dsp_config_response.py
--rw-r--r--   0        0        0     2813 2024-04-15 13:10:05.670442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/dsp_config_response_all_of.py
--rw-r--r--   0        0        0     3016 2024-04-15 13:10:05.670442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/dsp_feature_importance_response.py
--rw-r--r--   0        0        0     2728 2024-04-15 13:10:05.670442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/dsp_feature_importance_response_all_of.py
--rw-r--r--   0        0        0     2058 2024-04-15 13:10:05.670442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/dsp_feature_importance_response_all_of_features.py
--rw-r--r--   0        0        0     2572 2024-04-15 13:10:05.670442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/dsp_feature_importance_response_all_of_labels.py
--rw-r--r--   0        0        0     2216 2024-04-15 13:10:05.670442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/dsp_feature_labels_response.py
--rw-r--r--   0        0        0     1920 2024-04-15 13:10:05.670442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/dsp_feature_labels_response_all_of.py
--rw-r--r--   0        0        0     2294 2024-04-15 13:10:05.670442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/dsp_group.py
--rw-r--r--   0        0        0     4216 2024-04-15 13:10:05.674442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/dsp_group_item.py
--rw-r--r--   0        0        0     2190 2024-04-15 13:10:05.674442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/dsp_group_item_select_options_inner.py
--rw-r--r--   0        0        0     2195 2024-04-15 13:10:05.674442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/dsp_group_item_show_if.py
--rw-r--r--   0        0        0     4848 2024-04-15 13:10:05.674442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/dsp_info.py
--rw-r--r--   0        0        0     2376 2024-04-15 13:10:05.674442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/dsp_info_features.py
--rw-r--r--   0        0        0     1885 2024-04-15 13:10:05.674442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/dsp_info_performance.py
--rw-r--r--   0        0        0     5462 2024-04-15 13:10:05.674442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/dsp_metadata.py
--rw-r--r--   0        0        0     2025 2024-04-15 13:10:05.678442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/dsp_metadata_included_samples_inner.py
--rw-r--r--   0        0        0     2566 2024-04-15 13:10:05.678442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/dsp_metadata_output_config.py
--rw-r--r--   0        0        0     2531 2024-04-15 13:10:05.678442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/dsp_metadata_output_config_shape.py
--rw-r--r--   0        0        0     5820 2024-04-15 13:10:05.678442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/dsp_metadata_response.py
--rw-r--r--   0        0        0     3019 2024-04-15 13:10:05.678442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/dsp_performance_all_variants_response.py
--rw-r--r--   0        0        0     2729 2024-04-15 13:10:05.678442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/dsp_performance_all_variants_response_all_of.py
--rw-r--r--   0        0        0     2278 2024-04-15 13:10:05.678442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/dsp_performance_all_variants_response_all_of_performance.py
--rw-r--r--   0        0        0     4639 2024-04-15 13:10:05.678442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/dsp_run_graph.py
--rw-r--r--   0        0        0     1899 2024-04-15 13:10:05.678442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/dsp_run_graph_axis_labels.py
--rw-r--r--   0        0        0     2677 2024-04-15 13:10:05.678442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/dsp_run_request_with_features.py
--rw-r--r--   0        0        0     2151 2024-04-15 13:10:05.678442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/dsp_run_request_without_features.py
--rw-r--r--   0        0        0     2030 2024-04-15 13:10:05.678442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/dsp_run_request_without_features_read_only.py
--rw-r--r--   0        0        0     3697 2024-04-15 13:10:05.682442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/dsp_run_response.py
--rw-r--r--   0        0        0     3418 2024-04-15 13:10:05.682442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/dsp_run_response_all_of.py
--rw-r--r--   0        0        0     1969 2024-04-15 13:10:05.682442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/dsp_run_response_all_of_performance.py
--rw-r--r--   0        0        0     4579 2024-04-15 13:10:05.682442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/dsp_run_response_with_sample.py
--rw-r--r--   0        0        0     4312 2024-04-15 13:10:05.682442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/dsp_run_response_with_sample_all_of.py
--rw-r--r--   0        0        0     3342 2024-04-15 13:10:05.682442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/dsp_sample_features_response.py
--rw-r--r--   0        0        0     3042 2024-04-15 13:10:05.682442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/dsp_sample_features_response_all_of.py
--rw-r--r--   0        0        0     2748 2024-04-15 13:10:05.682442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/dsp_sample_features_response_all_of_data.py
--rw-r--r--   0        0        0     2213 2024-04-15 13:10:05.682442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/dsp_sample_features_response_all_of_sample.py
--rw-r--r--   0        0        0     3353 2024-04-15 13:10:05.682442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/dsp_trained_features_response.py
--rw-r--r--   0        0        0     3053 2024-04-15 13:10:05.682442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/dsp_trained_features_response_all_of.py
--rw-r--r--   0        0        0     2773 2024-04-15 13:10:05.682442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/dsp_trained_features_response_all_of_data.py
--rw-r--r--   0        0        0     2205 2024-04-15 13:10:05.682442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/dsp_trained_features_response_all_of_sample.py
--rw-r--r--   0        0        0     1893 2024-04-15 13:10:05.682442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/edit_sample_label_request.py
--rw-r--r--   0        0        0     4246 2024-04-15 13:10:05.682442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/enterprise_trial.py
--rw-r--r--   0        0        0     2960 2024-04-15 13:10:05.682442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/enterprise_upgrade_or_trial_extension_request.py
--rw-r--r--   0        0        0     2885 2024-04-15 13:10:05.682442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/entitlement_limits.py
--rw-r--r--   0        0        0     2367 2024-04-15 13:10:05.682442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/entity_created_response.py
--rw-r--r--   0        0        0     2077 2024-04-15 13:10:05.682442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/entity_created_response_all_of.py
--rw-r--r--   0        0        0     2656 2024-04-15 13:10:05.682442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/evaluate_job_response.py
--rw-r--r--   0        0        0     2349 2024-04-15 13:10:05.682442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/evaluate_job_response_all_of.py
--rw-r--r--   0        0        0     2099 2024-04-15 13:10:05.682442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/evaluate_result_value.py
--rw-r--r--   0        0        0     2366 2024-04-15 13:10:05.682442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/export_block_response.py
--rw-r--r--   0        0        0     2060 2024-04-15 13:10:05.682442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/export_block_response_all_of.py
--rw-r--r--   0        0        0     2511 2024-04-15 13:10:05.682442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/export_get_url_response.py
--rw-r--r--   0        0        0     2244 2024-04-15 13:10:05.682442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/export_get_url_response_all_of.py
--rw-r--r--   0        0        0     2116 2024-04-15 13:10:05.682442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/export_keras_block_data_request.py
--rw-r--r--   0        0        0     2373 2024-04-15 13:10:05.682442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/export_original_data_request.py
--rw-r--r--   0        0        0     2021 2024-04-15 13:10:05.682442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/export_wav_data_request.py
--rw-r--r--   0        0        0      500 2024-04-15 13:10:05.682442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/feature.py
--rw-r--r--   0        0        0     2206 2024-04-15 13:10:05.682442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/find_segment_sample_request.py
--rw-r--r--   0        0        0     2804 2024-04-15 13:10:05.682442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/find_segment_sample_response.py
--rw-r--r--   0        0        0     2497 2024-04-15 13:10:05.682442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/find_segment_sample_response_all_of.py
--rw-r--r--   0        0        0     2090 2024-04-15 13:10:05.682442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/find_segment_sample_response_all_of_segments.py
--rw-r--r--   0        0        0     2665 2024-04-15 13:10:05.682442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/find_user_response.py
--rw-r--r--   0        0        0     2358 2024-04-15 13:10:05.682442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/find_user_response_all_of.py
--rw-r--r--   0        0        0     2322 2024-04-15 13:10:05.682442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/find_user_response_all_of_users.py
--rw-r--r--   0        0        0     2507 2024-04-15 13:10:05.682442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/generate_features_request.py
--rw-r--r--   0        0        0     2083 2024-04-15 13:10:05.682442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/generic_api_response.py
--rw-r--r--   0        0        0     2764 2024-04-15 13:10:05.682442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_all_imported_from_response.py
--rw-r--r--   0        0        0     2457 2024-04-15 13:10:05.682442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_all_imported_from_response_all_of.py
--rw-r--r--   0        0        0     2156 2024-04-15 13:10:05.682442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_all_imported_from_response_all_of_data.py
--rw-r--r--   0        0        0     2698 2024-04-15 13:10:05.682442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_all_third_party_auth_response.py
--rw-r--r--   0        0        0     2391 2024-04-15 13:10:05.682442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_all_third_party_auth_response_all_of.py
--rw-r--r--   0        0        0     2713 2024-04-15 13:10:05.682442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_all_whitelabels_response.py
--rw-r--r--   0        0        0     2406 2024-04-15 13:10:05.682442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_all_whitelabels_response_all_of.py
--rw-r--r--   0        0        0     3527 2024-04-15 13:10:05.682442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_auto_labeler_response.py
--rw-r--r--   0        0        0     3260 2024-04-15 13:10:05.682442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_auto_labeler_response_all_of.py
--rw-r--r--   0        0        0     2588 2024-04-15 13:10:05.682442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_auto_labeler_response_all_of_clusters.py
--rw-r--r--   0        0        0     1954 2024-04-15 13:10:05.682442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_auto_labeler_response_all_of_items.py
--rw-r--r--   0        0        0     2345 2024-04-15 13:10:05.682442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_csv_wizard_uploaded_file_info.py
--rw-r--r--   0        0        0     2078 2024-04-15 13:10:05.682442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_csv_wizard_uploaded_file_info_all_of.py
--rw-r--r--   0        0        0     3400 2024-04-15 13:10:05.682442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_data_explorer_features_response.py
--rw-r--r--   0        0        0     3122 2024-04-15 13:10:05.682442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_data_explorer_features_response_all_of.py
--rw-r--r--   0        0        0     3752 2024-04-15 13:10:05.682442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_data_explorer_settings_response.py
--rw-r--r--   0        0        0     2402 2024-04-15 13:10:05.682442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_data_explorer_settings_response_all_of.py
--rw-r--r--   0        0        0     2349 2024-04-15 13:10:05.682442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_deployment_response.py
--rw-r--r--   0        0        0     2071 2024-04-15 13:10:05.682442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_deployment_response_all_of.py
--rw-r--r--   0        0        0     2434 2024-04-15 13:10:05.682442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_device_response.py
--rw-r--r--   0        0        0     2137 2024-04-15 13:10:05.682442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_device_response_all_of.py
--rw-r--r--   0        0        0     2752 2024-04-15 13:10:05.682442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_diversity_data_response.py
--rw-r--r--   0        0        0     2455 2024-04-15 13:10:05.682442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_diversity_data_response_all_of.py
--rw-r--r--   0        0        0     4251 2024-04-15 13:10:05.682442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_diversity_data_response_all_of_cluster_infos.py
--rw-r--r--   0        0        0     2859 2024-04-15 13:10:05.682442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_diversity_data_response_all_of_data.py
--rw-r--r--   0        0        0     2456 2024-04-15 13:10:05.682442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_email_verification_code_response.py
--rw-r--r--   0        0        0     2177 2024-04-15 13:10:05.682442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_email_verification_code_response_all_of.py
--rw-r--r--   0        0        0     2350 2024-04-15 13:10:05.682442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_email_verification_status_response.py
--rw-r--r--   0        0        0     2045 2024-04-15 13:10:05.682442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_email_verification_status_response_all_of.py
--rw-r--r--   0        0        0     2788 2024-04-15 13:10:05.682442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_feature_flags_response.py
--rw-r--r--   0        0        0     2488 2024-04-15 13:10:05.682442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_feature_flags_response_all_of.py
--rw-r--r--   0        0        0     2118 2024-04-15 13:10:05.682442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_feature_flags_response_all_of_flags.py
--rw-r--r--   0        0        0     3930 2024-04-15 13:10:05.682442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_impulse_blocks_response.py
--rw-r--r--   0        0        0     3630 2024-04-15 13:10:05.682442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_impulse_blocks_response_all_of.py
--rw-r--r--   0        0        0     2454 2024-04-15 13:10:05.682442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_impulse_response.py
--rw-r--r--   0        0        0     2157 2024-04-15 13:10:05.682442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_impulse_response_all_of.py
--rw-r--r--   0        0        0     2374 2024-04-15 13:10:05.682442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_job_response.py
--rw-r--r--   0        0        0     2077 2024-04-15 13:10:05.682442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_job_response_all_of.py
--rw-r--r--   0        0        0     3070 2024-04-15 13:10:05.682442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_jwt_request.py
--rw-r--r--   0        0        0     2431 2024-04-15 13:10:05.682442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_jwt_response.py
--rw-r--r--   0        0        0     2152 2024-04-15 13:10:05.682442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_jwt_response_all_of.py
--rw-r--r--   0        0        0     2580 2024-04-15 13:10:05.682442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_label_noise_data_response.py
--rw-r--r--   0        0        0     2256 2024-04-15 13:10:05.682442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_label_noise_data_response_all_of.py
--rw-r--r--   0        0        0     3358 2024-04-15 13:10:05.686442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_label_noise_data_response_all_of_data.py
--rw-r--r--   0        0        0     3578 2024-04-15 13:10:05.686442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_last_deployment_build_response.py
--rw-r--r--   0        0        0     3300 2024-04-15 13:10:05.686442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_last_deployment_build_response_all_of.py
--rw-r--r--   0        0        0     2869 2024-04-15 13:10:05.686442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_last_deployment_build_response_all_of_last_build.py
--rw-r--r--   0        0        0     2572 2024-04-15 13:10:05.686442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_notes_response.py
--rw-r--r--   0        0        0     2265 2024-04-15 13:10:05.686442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_notes_response_all_of.py
--rw-r--r--   0        0        0     2556 2024-04-15 13:10:05.686442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_organization_bucket_response.py
--rw-r--r--   0        0        0     2232 2024-04-15 13:10:05.686442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_organization_bucket_response_all_of.py
--rw-r--r--   0        0        0     2701 2024-04-15 13:10:05.686442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_organization_data_campaign_dashboard_response.py
--rw-r--r--   0        0        0     2377 2024-04-15 13:10:05.686442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_organization_data_campaign_dashboard_response_all_of.py
--rw-r--r--   0        0        0     2890 2024-04-15 13:10:05.686442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_organization_data_campaign_dashboards_response.py
--rw-r--r--   0        0        0     2583 2024-04-15 13:10:05.686442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_organization_data_campaign_dashboards_response_all_of.py
--rw-r--r--   0        0        0     3158 2024-04-15 13:10:05.686442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_organization_data_campaign_response.py
--rw-r--r--   0        0        0     2939 2024-04-15 13:10:05.686442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_organization_data_campaigns_response.py
--rw-r--r--   0        0        0     2632 2024-04-15 13:10:05.686442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_organization_data_campaigns_response_all_of.py
--rw-r--r--   0        0        0     2921 2024-04-15 13:10:05.686442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_organization_data_campaigns_response_all_of_campaigns.py
--rw-r--r--   0        0        0     2601 2024-04-15 13:10:05.686442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_organization_data_export_response.py
--rw-r--r--   0        0        0     2277 2024-04-15 13:10:05.686442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_organization_data_export_response_all_of.py
--rw-r--r--   0        0        0     2982 2024-04-15 13:10:05.686442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_organization_data_exports_response.py
--rw-r--r--   0        0        0     2682 2024-04-15 13:10:05.686442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_organization_data_exports_response_all_of.py
--rw-r--r--   0        0        0     2561 2024-04-15 13:10:05.686442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_organization_data_item_response.py
--rw-r--r--   0        0        0     2237 2024-04-15 13:10:05.686442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_organization_data_item_response_all_of.py
--rw-r--r--   0        0        0     3411 2024-04-15 13:10:05.686442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_organization_data_item_transform_jobs_response.py
--rw-r--r--   0        0        0     3111 2024-04-15 13:10:05.686442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_organization_data_item_transform_jobs_response_all_of.py
--rw-r--r--   0        0        0     3532 2024-04-15 13:10:05.686442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_organization_data_item_transform_jobs_response_all_of_transformation_jobs.py
--rw-r--r--   0        0        0     2576 2024-04-15 13:10:05.686442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_organization_dataset_response.py
--rw-r--r--   0        0        0     2252 2024-04-15 13:10:05.686442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_organization_dataset_response_all_of.py
--rw-r--r--   0        0        0     2690 2024-04-15 13:10:05.686442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_organization_deploy_block_response.py
--rw-r--r--   0        0        0     2373 2024-04-15 13:10:05.686442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_organization_deploy_block_response_all_of.py
--rw-r--r--   0        0        0     2627 2024-04-15 13:10:05.686442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_organization_dsp_block_response.py
--rw-r--r--   0        0        0     2310 2024-04-15 13:10:05.686442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_organization_dsp_block_response_all_of.py
--rw-r--r--   0        0        0     2603 2024-04-15 13:10:05.686442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_organization_pipelines_response.py
--rw-r--r--   0        0        0     2279 2024-04-15 13:10:05.686442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_organization_pipelines_response_all_of.py
--rw-r--r--   0        0        0     3670 2024-04-15 13:10:05.686442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_organization_portal_response.py
--rw-r--r--   0        0        0     3391 2024-04-15 13:10:05.686442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_organization_portal_response_all_of.py
--rw-r--r--   0        0        0     2323 2024-04-15 13:10:05.686442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_organization_projects_data_count_response.py
--rw-r--r--   0        0        0     2906 2024-04-15 13:10:05.686442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_organization_transfer_learning_block_response.py
--rw-r--r--   0        0        0     2589 2024-04-15 13:10:05.686442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_organization_transfer_learning_block_response_all_of.py
--rw-r--r--   0        0        0     2858 2024-04-15 13:10:05.686442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_organization_transformation_block_response.py
--rw-r--r--   0        0        0     2541 2024-04-15 13:10:05.686442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_organization_transformation_block_response_all_of.py
--rw-r--r--   0        0        0     2612 2024-04-15 13:10:05.686442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_organization_usage_report_response.py
--rw-r--r--   0        0        0     2905 2024-04-15 13:10:05.686442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_performance_calibration_ground_truth_response.py
--rw-r--r--   0        0        0     2598 2024-04-15 13:10:05.686442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_performance_calibration_ground_truth_response_all_of.py
--rw-r--r--   0        0        0     3012 2024-04-15 13:10:05.686442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_performance_calibration_parameter_sets_response.py
--rw-r--r--   0        0        0     2712 2024-04-15 13:10:05.686442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_performance_calibration_parameter_sets_response_all_of.py
--rw-r--r--   0        0        0     2722 2024-04-15 13:10:05.686442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_performance_calibration_parameters_response.py
--rw-r--r--   0        0        0     2425 2024-04-15 13:10:05.686442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_performance_calibration_parameters_response_all_of.py
--rw-r--r--   0        0        0     2922 2024-04-15 13:10:05.686442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_performance_calibration_raw_result_response.py
--rw-r--r--   0        0        0     2615 2024-04-15 13:10:05.686442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_performance_calibration_raw_result_response_all_of.py
--rw-r--r--   0        0        0     3151 2024-04-15 13:10:05.686442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_performance_calibration_status_response.py
--rw-r--r--   0        0        0     2884 2024-04-15 13:10:05.686442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_performance_calibration_status_response_all_of.py
--rw-r--r--   0        0        0     3761 2024-04-15 13:10:05.686442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_pretrained_model_response.py
--rw-r--r--   0        0        0     3483 2024-04-15 13:10:05.686442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_pretrained_model_response_all_of.py
--rw-r--r--   0        0        0     4031 2024-04-15 13:10:05.686442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_pretrained_model_response_all_of_model.py
--rw-r--r--   0        0        0     2978 2024-04-15 13:10:05.686442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_pretrained_model_response_all_of_model_info.py
--rw-r--r--   0        0        0     3058 2024-04-15 13:10:05.686442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_pretrained_model_response_all_of_model_profile_info.py
--rw-r--r--   0        0        0     2397 2024-04-15 13:10:05.686442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_public_metrics_response.py
--rw-r--r--   0        0        0     2073 2024-04-15 13:10:05.686442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_public_metrics_response_all_of.py
--rw-r--r--   0        0        0     2767 2024-04-15 13:10:05.686442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_sample_metadata_response.py
--rw-r--r--   0        0        0     3044 2024-04-15 13:10:05.686442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_sample_response.py
--rw-r--r--   0        0        0     2462 2024-04-15 13:10:05.686442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_syntiant_posterior_response.py
--rw-r--r--   0        0        0     2184 2024-04-15 13:10:05.686442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_syntiant_posterior_response_all_of.py
--rw-r--r--   0        0        0     2694 2024-04-15 13:10:05.686442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_target_constraints_response.py
--rw-r--r--   0        0        0     2404 2024-04-15 13:10:05.686442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_target_constraints_response_all_of.py
--rw-r--r--   0        0        0     2414 2024-04-15 13:10:05.686442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_theme_response.py
--rw-r--r--   0        0        0     2117 2024-04-15 13:10:05.686442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_theme_response_all_of.py
--rw-r--r--   0        0        0     2592 2024-04-15 13:10:05.686442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_themes_response.py
--rw-r--r--   0        0        0     2285 2024-04-15 13:10:05.686442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_themes_response_all_of.py
--rw-r--r--   0        0        0     2495 2024-04-15 13:10:05.686442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_third_party_auth_response.py
--rw-r--r--   0        0        0     2171 2024-04-15 13:10:05.686442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_third_party_auth_response_all_of.py
--rw-r--r--   0        0        0     3543 2024-04-15 13:10:05.686442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_user_need_to_set_password_response.py
--rw-r--r--   0        0        0     3276 2024-04-15 13:10:05.686442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_user_need_to_set_password_response_all_of.py
--rw-r--r--   0        0        0     7721 2024-04-15 13:10:05.690442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_user_response.py
--rw-r--r--   0        0        0     5497 2024-04-15 13:10:05.694442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_user_response_all_of.py
--rw-r--r--   0        0        0     2395 2024-04-15 13:10:05.694442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_user_response_all_of_whitelabels.py
--rw-r--r--   0        0        0     2307 2024-04-15 13:10:05.694442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_whitelabel_domain_response.py
--rw-r--r--   0        0        0     2021 2024-04-15 13:10:05.694442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_whitelabel_domain_response_all_of.py
--rw-r--r--   0        0        0     2514 2024-04-15 13:10:05.694442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_whitelabel_response.py
--rw-r--r--   0        0        0     2217 2024-04-15 13:10:05.694442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_whitelabel_response_all_of.py
--rw-r--r--   0        0        0     2776 2024-04-15 13:10:05.694442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/has_data_explorer_features_response.py
--rw-r--r--   0        0        0     2498 2024-04-15 13:10:05.694442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/has_data_explorer_features_response_all_of.py
--rw-r--r--   0        0        0      580 2024-04-15 13:10:05.694442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/image_input_scaling.py
--rw-r--r--   0        0        0     3738 2024-04-15 13:10:05.694442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/impulse.py
--rw-r--r--   0        0        0     6723 2024-04-15 13:10:05.694442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/impulse_block_version.py
--rw-r--r--   0        0        0     6814 2024-04-15 13:10:05.694442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/impulse_dsp_block.py
--rw-r--r--   0        0        0     1967 2024-04-15 13:10:05.694442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/impulse_dsp_block_organization.py
--rw-r--r--   0        0        0     8958 2024-04-15 13:10:05.694442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/impulse_input_block.py
--rw-r--r--   0        0        0     5612 2024-04-15 13:10:05.694442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/impulse_learn_block.py
--rw-r--r--   0        0        0     2627 2024-04-15 13:10:05.694442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/input_block.py
--rw-r--r--   0        0        0     2323 2024-04-15 13:10:05.698442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/invite_organization_member_request.py
--rw-r--r--   0        0        0     4172 2024-04-15 13:10:05.698442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/job.py
--rw-r--r--   0        0        0     2066 2024-04-15 13:10:05.698442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/job_created_by_user.py
--rw-r--r--   0        0        0     5203 2024-04-15 13:10:05.698442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/job_details.py
--rw-r--r--   0        0        0     2736 2024-04-15 13:10:05.698442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/job_details_all_of.py
--rw-r--r--   0        0        0     2613 2024-04-15 13:10:05.698442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/job_details_response.py
--rw-r--r--   0        0        0     2316 2024-04-15 13:10:05.698442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/job_details_response_all_of.py
--rw-r--r--   0        0        0     2257 2024-04-15 13:10:05.698442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/job_failure_details.py
--rw-r--r--   0        0        0     2657 2024-04-15 13:10:05.698442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/job_logs_response.py
--rw-r--r--   0        0        0     2350 2024-04-15 13:10:05.698442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/job_logs_response_all_of.py
--rw-r--r--   0        0        0     3297 2024-04-15 13:10:05.698442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/job_metrics_response.py
--rw-r--r--   0        0        0     3007 2024-04-15 13:10:05.698442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/job_metrics_response_all_of.py
--rw-r--r--   0        0        0      546 2024-04-15 13:10:05.698442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/job_parent_type_enum.py
--rw-r--r--   0        0        0     2944 2024-04-15 13:10:05.698442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/job_state.py
--rw-r--r--   0        0        0     1966 2024-04-15 13:10:05.698442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/job_state_execution_details.py
--rw-r--r--   0        0        0      598 2024-04-15 13:10:05.698442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/job_status.py
--rw-r--r--   0        0        0     2965 2024-04-15 13:10:05.698442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/job_step.py
--rw-r--r--   0        0        0     2713 2024-04-15 13:10:05.698442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/job_summary_response.py
--rw-r--r--   0        0        0     2406 2024-04-15 13:10:05.698442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/job_summary_response_all_of.py
--rw-r--r--   0        0        0     2089 2024-04-15 13:10:05.698442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/job_summary_response_all_of_summary.py
--rw-r--r--   0        0        0     1993 2024-04-15 13:10:05.698442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/keras_custom_metric.py
--rw-r--r--   0        0        0     2510 2024-04-15 13:10:05.698442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/keras_model_layer.py
--rw-r--r--   0        0        0     2093 2024-04-15 13:10:05.698442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/keras_model_layer_input.py
--rw-r--r--   0        0        0     2101 2024-04-15 13:10:05.698442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/keras_model_layer_output.py
--rw-r--r--   0        0        0     5707 2024-04-15 13:10:05.698442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/keras_model_metadata.py
--rw-r--r--   0        0        0     5440 2024-04-15 13:10:05.698442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/keras_model_metadata_all_of.py
--rw-r--r--   0        0        0     5421 2024-04-15 13:10:05.698442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/keras_model_metadata_metrics.py
--rw-r--r--   0        0        0     4495 2024-04-15 13:10:05.698442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/keras_model_metadata_metrics_on_device_performance_inner.py
--rw-r--r--   0        0        0     2497 2024-04-15 13:10:05.698442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/keras_model_metadata_metrics_on_device_performance_inner_tflite.py
--rw-r--r--   0        0        0      562 2024-04-15 13:10:05.698442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/keras_model_type_enum.py
--rw-r--r--   0        0        0      524 2024-04-15 13:10:05.698442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/keras_model_variant_enum.py
--rw-r--r--   0        0        0    11377 2024-04-15 13:10:05.698442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/keras_response.py
--rw-r--r--   0        0        0    11110 2024-04-15 13:10:05.702442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/keras_response_all_of.py
--rw-r--r--   0        0        0     3392 2024-04-15 13:10:05.702442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/keras_visual_layer.py
--rw-r--r--   0        0        0     2310 2024-04-15 13:10:05.702442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/keras_visual_layer_type.py
--rw-r--r--   0        0        0     2529 2024-04-15 13:10:05.702442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/last_modification_date_response.py
--rw-r--r--   0        0        0     2239 2024-04-15 13:10:05.702442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/last_modification_date_response_all_of.py
--rw-r--r--   0        0        0     2633 2024-04-15 13:10:05.702442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/latency_device.py
--rw-r--r--   0        0        0     3146 2024-04-15 13:10:05.706442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/learn_block.py
--rw-r--r--   0        0        0      933 2024-04-15 13:10:05.706442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/learn_block_type.py
--rw-r--r--   0        0        0     2788 2024-04-15 13:10:05.706442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_api_keys_response.py
--rw-r--r--   0        0        0     2488 2024-04-15 13:10:05.706442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_api_keys_response_all_of.py
--rw-r--r--   0        0        0     2704 2024-04-15 13:10:05.706442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_api_keys_response_all_of_api_keys.py
--rw-r--r--   0        0        0     2630 2024-04-15 13:10:05.706442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_devices_response.py
--rw-r--r--   0        0        0     2333 2024-04-15 13:10:05.706442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_devices_response_all_of.py
--rw-r--r--   0        0        0     2726 2024-04-15 13:10:05.706442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_email_response.py
--rw-r--r--   0        0        0     2426 2024-04-15 13:10:05.706442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_email_response_all_of.py
--rw-r--r--   0        0        0     2918 2024-04-15 13:10:05.706442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_email_response_all_of_emails.py
--rw-r--r--   0        0        0     2767 2024-04-15 13:10:05.706442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_enterprise_trials_response.py
--rw-r--r--   0        0        0     2467 2024-04-15 13:10:05.706442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_enterprise_trials_response_all_of.py
--rw-r--r--   0        0        0     2813 2024-04-15 13:10:05.706442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_hmac_keys_response.py
--rw-r--r--   0        0        0     2513 2024-04-15 13:10:05.706442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_hmac_keys_response_all_of.py
--rw-r--r--   0        0        0     2381 2024-04-15 13:10:05.706442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_hmac_keys_response_all_of_hmac_keys.py
--rw-r--r--   0        0        0     2745 2024-04-15 13:10:05.706442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_jobs_response.py
--rw-r--r--   0        0        0     2445 2024-04-15 13:10:05.706442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_jobs_response_all_of.py
--rw-r--r--   0        0        0     2200 2024-04-15 13:10:05.706442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_models_response.py
--rw-r--r--   0        0        0     1910 2024-04-15 13:10:05.706442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_models_response_all_of.py
--rw-r--r--   0        0        0     2921 2024-04-15 13:10:05.706442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_organization_api_keys_response.py
--rw-r--r--   0        0        0     2621 2024-04-15 13:10:05.706442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_organization_api_keys_response_all_of.py
--rw-r--r--   0        0        0     2760 2024-04-15 13:10:05.706442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_organization_api_keys_response_all_of_api_keys.py
--rw-r--r--   0        0        0     2752 2024-04-15 13:10:05.706442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_organization_buckets_response.py
--rw-r--r--   0        0        0     2445 2024-04-15 13:10:05.706442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_organization_buckets_response_all_of.py
--rw-r--r--   0        0        0     2902 2024-04-15 13:10:05.706442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_organization_buckets_user_response.py
--rw-r--r--   0        0        0     2595 2024-04-15 13:10:05.706442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_organization_buckets_user_response_all_of.py
--rw-r--r--   0        0        0     2760 2024-04-15 13:10:05.706442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_organization_buckets_user_response_all_of_buckets.py
--rw-r--r--   0        0        0     3310 2024-04-15 13:10:05.706442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_organization_data_response.py
--rw-r--r--   0        0        0     3031 2024-04-15 13:10:05.706442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_organization_data_response_all_of.py
--rw-r--r--   0        0        0     3430 2024-04-15 13:10:05.706442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_organization_data_response_all_of_data.py
--rw-r--r--   0        0        0     2887 2024-04-15 13:10:05.706442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_organization_deploy_blocks_response.py
--rw-r--r--   0        0        0     2587 2024-04-15 13:10:05.706442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_organization_deploy_blocks_response_all_of.py
--rw-r--r--   0        0        0     2824 2024-04-15 13:10:05.706442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_organization_dsp_blocks_response.py
--rw-r--r--   0        0        0     2524 2024-04-15 13:10:05.706442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_organization_dsp_blocks_response_all_of.py
--rw-r--r--   0        0        0     3353 2024-04-15 13:10:05.706442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_organization_files_response.py
--rw-r--r--   0        0        0     3074 2024-04-15 13:10:05.706442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_organization_files_response_all_of.py
--rw-r--r--   0        0        0     2792 2024-04-15 13:10:05.706442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_organization_pipelines_response.py
--rw-r--r--   0        0        0     2485 2024-04-15 13:10:05.706442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_organization_pipelines_response_all_of.py
--rw-r--r--   0        0        0     2857 2024-04-15 13:10:05.706442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_organization_portals_response.py
--rw-r--r--   0        0        0     2550 2024-04-15 13:10:05.706442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_organization_portals_response_all_of.py
--rw-r--r--   0        0        0     2858 2024-04-15 13:10:05.706442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_organization_portals_response_all_of_portals.py
--rw-r--r--   0        0        0     3449 2024-04-15 13:10:05.706442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_organization_projects_data_response.py
--rw-r--r--   0        0        0     3142 2024-04-15 13:10:05.706442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_organization_projects_data_response_all_of.py
--rw-r--r--   0        0        0     2271 2024-04-15 13:10:05.706442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_organization_projects_data_response_all_of_projects.py
--rw-r--r--   0        0        0     2857 2024-04-15 13:10:05.706442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_organization_secrets_response.py
--rw-r--r--   0        0        0     2550 2024-04-15 13:10:05.706442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_organization_secrets_response_all_of.py
--rw-r--r--   0        0        0     2819 2024-04-15 13:10:05.706442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_organization_secrets_response_all_of_secrets.py
--rw-r--r--   0        0        0     3103 2024-04-15 13:10:05.706442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_organization_transfer_learning_blocks_response.py
--rw-r--r--   0        0        0     2803 2024-04-15 13:10:05.706442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_organization_transfer_learning_blocks_response_all_of.py
--rw-r--r--   0        0        0     3055 2024-04-15 13:10:05.706442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_organization_transformation_blocks_response.py
--rw-r--r--   0        0        0     2755 2024-04-15 13:10:05.706442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_organization_transformation_blocks_response_all_of.py
--rw-r--r--   0        0        0     2988 2024-04-15 13:10:05.706442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_organization_usage_reports_response.py
--rw-r--r--   0        0        0     2688 2024-04-15 13:10:05.706442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_organization_usage_reports_response_all_of.py
--rw-r--r--   0        0        0     2786 2024-04-15 13:10:05.706442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_organizations_response.py
--rw-r--r--   0        0        0     2486 2024-04-15 13:10:05.706442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_organizations_response_all_of.py
--rw-r--r--   0        0        0     2512 2024-04-15 13:10:05.710442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_portal_files_in_folder_request.py
--rw-r--r--   0        0        0     2872 2024-04-15 13:10:05.710442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_portal_files_in_folder_response.py
--rw-r--r--   0        0        0     2593 2024-04-15 13:10:05.710442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_portal_files_in_folder_response_all_of.py
--rw-r--r--   0        0        0     2290 2024-04-15 13:10:05.710442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_projects.py
--rw-r--r--   0        0        0     2681 2024-04-15 13:10:05.710442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_projects_response.py
--rw-r--r--   0        0        0     3122 2024-04-15 13:10:05.710442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_public_organization_transformation_blocks_response.py
--rw-r--r--   0        0        0     2822 2024-04-15 13:10:05.710442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_public_organization_transformation_blocks_response_all_of.py
--rw-r--r--   0        0        0     2553 2024-04-15 13:10:05.710442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_public_projects.py
--rw-r--r--   0        0        0     2944 2024-04-15 13:10:05.710442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_public_projects_response.py
--rw-r--r--   0        0        0     2815 2024-04-15 13:10:05.710442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_public_versions_response.py
--rw-r--r--   0        0        0     2508 2024-04-15 13:10:05.710442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_public_versions_response_all_of.py
--rw-r--r--   0        0        0     2290 2024-04-15 13:10:05.710442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_public_versions_response_all_of_versions.py
--rw-r--r--   0        0        0     2754 2024-04-15 13:10:05.710442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_samples_response.py
--rw-r--r--   0        0        0     2454 2024-04-15 13:10:05.710442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_samples_response_all_of.py
--rw-r--r--   0        0        0     2615 2024-04-15 13:10:05.710442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_tuner_runs_response.py
--rw-r--r--   0        0        0     2308 2024-04-15 13:10:05.710442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_tuner_runs_response_all_of.py
--rw-r--r--   0        0        0     3933 2024-04-15 13:10:05.710442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_versions_response.py
--rw-r--r--   0        0        0     3633 2024-04-15 13:10:05.710442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_versions_response_all_of.py
--rw-r--r--   0        0        0     2353 2024-04-15 13:10:05.710442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_versions_response_all_of_bucket.py
--rw-r--r--   0        0        0     2053 2024-04-15 13:10:05.710442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_versions_response_all_of_custom_learn_blocks.py
--rw-r--r--   0        0        0     3960 2024-04-15 13:10:05.710442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_versions_response_all_of_versions.py
--rw-r--r--   0        0        0     2367 2024-04-15 13:10:05.710442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/log_analytics_event_request.py
--rw-r--r--   0        0        0     2900 2024-04-15 13:10:05.710442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/log_stdout_response.py
--rw-r--r--   0        0        0     2600 2024-04-15 13:10:05.710442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/log_stdout_response_all_of.py
--rw-r--r--   0        0        0     2441 2024-04-15 13:10:05.710442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/log_stdout_response_all_of_stdout.py
--rw-r--r--   0        0        0     2191 2024-04-15 13:10:05.710442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/log_website_pageview_request.py
--rw-r--r--   0        0        0     2217 2024-04-15 13:10:05.710442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/login_response.py
--rw-r--r--   0        0        0     1911 2024-04-15 13:10:05.710442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/login_response_all_of.py
--rw-r--r--   0        0        0     2528 2024-04-15 13:10:05.710442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/memory_spec.py
--rw-r--r--   0        0        0     2746 2024-04-15 13:10:05.714442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/metrics_all_variants_response.py
--rw-r--r--   0        0        0     2449 2024-04-15 13:10:05.718442 edgeimpulse_api-1.49.5/edgeimpulse_api/models/metrics_all_variants_response_all_of.py
--rw-r--r--   0        0        0     2128 2024-04-15 13:10:05.766441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/metrics_for_model_variant.py
--rw-r--r--   0        0        0     2430 2024-04-15 13:10:05.766441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/migration.py
--rw-r--r--   0        0        0      571 2024-04-15 13:10:05.766441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/model_engine_short_enum.py
--rw-r--r--   0        0        0     3010 2024-04-15 13:10:05.770441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/model_prediction.py
--rw-r--r--   0        0        0     2895 2024-04-15 13:10:05.770441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/model_result.py
--rw-r--r--   0        0        0     5046 2024-04-15 13:10:05.770441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/model_variant_stats.py
--rw-r--r--   0        0        0     2128 2024-04-15 13:10:05.770441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/move_raw_data_request.py
--rw-r--r--   0        0        0     2784 2024-04-15 13:10:05.770441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/neighbors_data.py
--rw-r--r--   0        0        0     3584 2024-04-15 13:10:05.770441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/neighbors_score.py
--rw-r--r--   0        0        0     2736 2024-04-15 13:10:05.770441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/neighbors_score_neighbor_windows_inner.py
--rw-r--r--   0        0        0     2687 2024-04-15 13:10:05.770441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/note.py
--rw-r--r--   0        0        0     2221 2024-04-15 13:10:05.770441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/object_detection_auto_label_request.py
--rw-r--r--   0        0        0     2994 2024-04-15 13:10:05.770441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/object_detection_auto_label_response.py
--rw-r--r--   0        0        0     2705 2024-04-15 13:10:05.770441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/object_detection_auto_label_response_all_of.py
--rw-r--r--   0        0        0     2275 2024-04-15 13:10:05.770441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/object_detection_auto_label_response_all_of_results.py
--rw-r--r--   0        0        0     2368 2024-04-15 13:10:05.770441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/object_detection_label_queue_count_response.py
--rw-r--r--   0        0        0     2051 2024-04-15 13:10:05.770441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/object_detection_label_queue_count_response_all_of.py
--rw-r--r--   0        0        0     2887 2024-04-15 13:10:05.770441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/object_detection_label_queue_response.py
--rw-r--r--   0        0        0     2580 2024-04-15 13:10:05.770441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/object_detection_label_queue_response_all_of.py
--rw-r--r--   0        0        0      775 2024-04-15 13:10:05.770441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/object_detection_last_layer.py
--rw-r--r--   0        0        0     6491 2024-04-15 13:10:05.774441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/optimize_config.py
--rw-r--r--   0        0        0     6949 2024-04-15 13:10:05.774441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/optimize_config_response.py
--rw-r--r--   0        0        0     1920 2024-04-15 13:10:05.774441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/optimize_config_response_all_of.py
--rw-r--r--   0        0        0     2056 2024-04-15 13:10:05.774441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/optimize_config_target_device.py
--rw-r--r--   0        0        0     2271 2024-04-15 13:10:05.774441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/optimize_dsp_parameters_response.py
--rw-r--r--   0        0        0     1964 2024-04-15 13:10:05.774441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/optimize_dsp_parameters_response_all_of.py
--rw-r--r--   0        0        0     2756 2024-04-15 13:10:05.774441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/optimize_space_response.py
--rw-r--r--   0        0        0     2456 2024-04-15 13:10:05.774441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/optimize_space_response_all_of.py
--rw-r--r--   0        0        0     5546 2024-04-15 13:10:05.774441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/optimize_state_response.py
--rw-r--r--   0        0        0     5279 2024-04-15 13:10:05.774441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/optimize_state_response_all_of.py
--rw-r--r--   0        0        0     3284 2024-04-15 13:10:05.774441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/optimize_state_response_all_of_status.py
--rw-r--r--   0        0        0     2273 2024-04-15 13:10:05.774441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/optimize_state_response_all_of_workers.py
--rw-r--r--   0        0        0     2749 2024-04-15 13:10:05.774441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/optimize_transfer_learning_models_response.py
--rw-r--r--   0        0        0     2425 2024-04-15 13:10:05.774441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/optimize_transfer_learning_models_response_all_of.py
--rw-r--r--   0        0        0     4717 2024-04-15 13:10:05.774441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/optimize_transfer_learning_models_response_all_of_models.py
--rw-r--r--   0        0        0     5801 2024-04-15 13:10:05.774441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/organization.py
--rw-r--r--   0        0        0     2700 2024-04-15 13:10:05.778441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/organization_add_data_folder_request.py
--rw-r--r--   0        0        0     2498 2024-04-15 13:10:05.778441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/organization_add_data_folder_response.py
--rw-r--r--   0        0        0     2209 2024-04-15 13:10:05.778441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/organization_add_data_folder_response_all_of.py
--rw-r--r--   0        0        0     2835 2024-04-15 13:10:05.778441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/organization_add_dataset_request.py
--rw-r--r--   0        0        0     2493 2024-04-15 13:10:05.778441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/organization_add_dataset_request_bucket.py
--rw-r--r--   0        0        0     2820 2024-04-15 13:10:05.778441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/organization_bucket.py
--rw-r--r--   0        0        0     2711 2024-04-15 13:10:05.778441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/organization_compute_time_usage.py
--rw-r--r--   0        0        0     9492 2024-04-15 13:10:05.778441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/organization_create_project.py
--rw-r--r--   0        0        0      605 2024-04-15 13:10:05.778441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/organization_create_project_output_dataset_path_rule.py
--rw-r--r--   0        0        0     2262 2024-04-15 13:10:05.778441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/organization_create_project_path_filter.py
--rw-r--r--   0        0        0     7464 2024-04-15 13:10:05.778441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/organization_create_project_request.py
--rw-r--r--   0        0        0     2543 2024-04-15 13:10:05.778441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/organization_create_project_response.py
--rw-r--r--   0        0        0     2237 2024-04-15 13:10:05.778441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/organization_create_project_response_all_of.py
--rw-r--r--   0        0        0     2704 2024-04-15 13:10:05.778441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/organization_create_project_status_response.py
--rw-r--r--   0        0        0     2407 2024-04-15 13:10:05.778441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/organization_create_project_status_response_all_of.py
--rw-r--r--   0        0        0     2754 2024-04-15 13:10:05.778441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/organization_create_project_transformation_summary.py
--rw-r--r--   0        0        0    10387 2024-04-15 13:10:05.778441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/organization_create_project_with_files.py
--rw-r--r--   0        0        0     2744 2024-04-15 13:10:05.778441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/organization_create_project_with_files_all_of.py
--rw-r--r--   0        0        0     3483 2024-04-15 13:10:05.778441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/organization_create_project_with_files_all_of_files.py
--rw-r--r--   0        0        0     2559 2024-04-15 13:10:05.778441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/organization_data_campaign_diff_request.py
--rw-r--r--   0        0        0     2327 2024-04-15 13:10:05.778441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/organization_data_campaign_diff_request_queries_inner.py
--rw-r--r--   0        0        0     3041 2024-04-15 13:10:05.778441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/organization_data_campaign_diff_response.py
--rw-r--r--   0        0        0     2741 2024-04-15 13:10:05.778441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/organization_data_campaign_diff_response_all_of.py
--rw-r--r--   0        0        0     2468 2024-04-15 13:10:05.778441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/organization_data_campaign_diff_response_all_of_queries.py
--rw-r--r--   0        0        0     3483 2024-04-15 13:10:05.778441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/organization_data_export.py
--rw-r--r--   0        0        0     3476 2024-04-15 13:10:05.778441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/organization_data_item.py
--rw-r--r--   0        0        0     2303 2024-04-15 13:10:05.778441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/organization_data_item_files_inner.py
--rw-r--r--   0        0        0     4007 2024-04-15 13:10:05.778441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/organization_dataset.py
--rw-r--r--   0        0        0     2800 2024-04-15 13:10:05.778441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/organization_dataset_bucket.py
--rw-r--r--   0        0        0     6005 2024-04-15 13:10:05.782441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/organization_deploy_block.py
--rw-r--r--   0        0        0     4962 2024-04-15 13:10:05.782441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/organization_dsp_block.py
--rw-r--r--   0        0        0     3037 2024-04-15 13:10:05.782441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/organization_get_create_projects_response.py
--rw-r--r--   0        0        0     2737 2024-04-15 13:10:05.782441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/organization_get_create_projects_response_all_of.py
--rw-r--r--   0        0        0     7063 2024-04-15 13:10:05.782441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/organization_get_create_projects_response_all_of_jobs.py
--rw-r--r--   0        0        0     6864 2024-04-15 13:10:05.782441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/organization_info_response.py
--rw-r--r--   0        0        0     6574 2024-04-15 13:10:05.786441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/organization_info_response_all_of.py
--rw-r--r--   0        0        0     3915 2024-04-15 13:10:05.786441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/organization_info_response_all_of_cli_lists.py
--rw-r--r--   0        0        0     2267 2024-04-15 13:10:05.786441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/organization_info_response_all_of_cli_lists_image_input_scaling_options.py
--rw-r--r--   0        0        0     2338 2024-04-15 13:10:05.786441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/organization_info_response_all_of_cli_lists_object_detection_last_layer_options.py
--rw-r--r--   0        0        0     2458 2024-04-15 13:10:05.786441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/organization_info_response_all_of_default_compute_limits.py
--rw-r--r--   0        0        0     2101 2024-04-15 13:10:05.786441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/organization_info_response_all_of_performance.py
--rw-r--r--   0        0        0      525 2024-04-15 13:10:05.790441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/organization_member_role.py
--rw-r--r--   0        0        0     2639 2024-04-15 13:10:05.790441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/organization_metrics_response.py
--rw-r--r--   0        0        0     2315 2024-04-15 13:10:05.790441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/organization_metrics_response_all_of.py
--rw-r--r--   0        0        0     4480 2024-04-15 13:10:05.790441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/organization_metrics_response_all_of_metrics.py
--rw-r--r--   0        0        0     6143 2024-04-15 13:10:05.790441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/organization_pipeline.py
--rw-r--r--   0        0        0     2595 2024-04-15 13:10:05.790441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/organization_pipeline_feeding_into_dataset.py
--rw-r--r--   0        0        0     2275 2024-04-15 13:10:05.790441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/organization_pipeline_feeding_into_project.py
--rw-r--r--   0        0        0     2314 2024-04-15 13:10:05.790441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/organization_pipeline_item_count.py
--rw-r--r--   0        0        0     4129 2024-04-15 13:10:05.790441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/organization_pipeline_run.py
--rw-r--r--   0        0        0     5330 2024-04-15 13:10:05.790441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/organization_pipeline_run_step.py
--rw-r--r--   0        0        0     6532 2024-04-15 13:10:05.790441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/organization_pipeline_step.py
--rw-r--r--   0        0        0     2351 2024-04-15 13:10:05.790441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/organization_projects_data_batch_disable_response.py
--rw-r--r--   0        0        0     2344 2024-04-15 13:10:05.790441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/organization_projects_data_batch_enable_response.py
--rw-r--r--   0        0        0     2037 2024-04-15 13:10:05.790441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/organization_projects_data_batch_request.py
--rw-r--r--   0        0        0     7242 2024-04-15 13:10:05.790441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/organization_transfer_learning_block.py
--rw-r--r--   0        0        0      611 2024-04-15 13:10:05.790441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/organization_transfer_learning_operates_on.py
--rw-r--r--   0        0        0     8670 2024-04-15 13:10:05.794441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/organization_transformation_block.py
--rw-r--r--   0        0        0     3918 2024-04-15 13:10:05.794441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/organization_update_pipeline_body.py
--rw-r--r--   0        0        0     3351 2024-04-15 13:10:05.794441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/organization_usage_report.py
--rw-r--r--   0        0        0     4440 2024-04-15 13:10:05.794441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/organization_user.py
--rw-r--r--   0        0        0     2294 2024-04-15 13:10:05.794441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/organization_user_all_of.py
--rw-r--r--   0        0        0     2104 2024-04-15 13:10:05.794441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/performance_calibration_detection.py
--rw-r--r--   0        0        0     3434 2024-04-15 13:10:05.794441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/performance_calibration_false_positive.py
--rw-r--r--   0        0        0     3770 2024-04-15 13:10:05.794441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/performance_calibration_ground_truth.py
--rw-r--r--   0        0        0     2477 2024-04-15 13:10:05.794441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/performance_calibration_ground_truth_samples_inner.py
--rw-r--r--   0        0        0     4880 2024-04-15 13:10:05.794441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/performance_calibration_parameter_set.py
--rw-r--r--   0        0        0     2255 2024-04-15 13:10:05.794441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/performance_calibration_parameter_set_aggregate_stats.py
--rw-r--r--   0        0        0     4092 2024-04-15 13:10:05.794441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/performance_calibration_parameter_set_stats_inner.py
--rw-r--r--   0        0        0     3007 2024-04-15 13:10:05.794441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/performance_calibration_parameters.py
--rw-r--r--   0        0        0     2585 2024-04-15 13:10:05.794441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/performance_calibration_parameters_standard.py
--rw-r--r--   0        0        0     2250 2024-04-15 13:10:05.794441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/performance_calibration_raw_detection.py
--rw-r--r--   0        0        0     2366 2024-04-15 13:10:05.794441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/performance_calibration_save_parameter_set_request.py
--rw-r--r--   0        0        0     2412 2024-04-15 13:10:05.794441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/performance_calibration_upload_labeled_audio_response.py
--rw-r--r--   0        0        0     2106 2024-04-15 13:10:05.794441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/performance_calibration_upload_labeled_audio_response_all_of.py
--rw-r--r--   0        0        0     1839 2024-04-15 13:10:05.794441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/permission.py
--rw-r--r--   0        0        0     2491 2024-04-15 13:10:05.794441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/portal_file.py
--rw-r--r--   0        0        0     2537 2024-04-15 13:10:05.794441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/portal_info_response.py
--rw-r--r--   0        0        0     2666 2024-04-15 13:10:05.794441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/pretrained_model_tensor.py
--rw-r--r--   0        0        0     2403 2024-04-15 13:10:05.798441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/preview_default_files_in_folder_request.py
--rw-r--r--   0        0        0     3734 2024-04-15 13:10:05.798441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/preview_default_files_in_folder_response.py
--rw-r--r--   0        0        0     3467 2024-04-15 13:10:05.802441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/preview_default_files_in_folder_response_all_of.py
--rw-r--r--   0        0        0     2955 2024-04-15 13:10:05.802441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/profile_model_info.py
--rw-r--r--   0        0        0     3117 2024-04-15 13:10:05.802441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/profile_model_info_memory.py
--rw-r--r--   0        0        0     1918 2024-04-15 13:10:05.802441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/profile_model_info_memory_eon.py
--rw-r--r--   0        0        0     2065 2024-04-15 13:10:05.802441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/profile_model_info_memory_tflite.py
--rw-r--r--   0        0        0     4335 2024-04-15 13:10:05.802441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/profile_model_table.py
--rw-r--r--   0        0        0     2780 2024-04-15 13:10:05.802441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/profile_model_table_mcu.py
--rw-r--r--   0        0        0     3042 2024-04-15 13:10:05.802441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/profile_model_table_mcu_memory.py
--rw-r--r--   0        0        0     2250 2024-04-15 13:10:05.802441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/profile_model_table_mpu.py
--rw-r--r--   0        0        0     2201 2024-04-15 13:10:05.802441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/profile_tf_lite_request.py
--rw-r--r--   0        0        0     3292 2024-04-15 13:10:05.802441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/profile_tf_lite_response.py
--rw-r--r--   0        0        0     7873 2024-04-15 13:10:05.806441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/project.py
--rw-r--r--   0        0        0     4103 2024-04-15 13:10:05.806441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/project_collaborator.py
--rw-r--r--   0        0        0     1895 2024-04-15 13:10:05.806441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/project_collaborator_all_of.py
--rw-r--r--   0        0        0     2416 2024-04-15 13:10:05.806441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/project_data_axes_summary_response.py
--rw-r--r--   0        0        0     2116 2024-04-15 13:10:05.806441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/project_data_axes_summary_response_all_of.py
--rw-r--r--   0        0        0     2281 2024-04-15 13:10:05.806441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/project_data_interval_response.py
--rw-r--r--   0        0        0     1964 2024-04-15 13:10:05.806441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/project_data_interval_response_all_of.py
--rw-r--r--   0        0        0     2235 2024-04-15 13:10:05.806441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/project_data_summary.py
--rw-r--r--   0        0        0     6854 2024-04-15 13:10:05.806441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/project_deployment_target.py
--rw-r--r--   0        0        0     2706 2024-04-15 13:10:05.806441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/project_deployment_target_all_of.py
--rw-r--r--   0        0        0     2780 2024-04-15 13:10:05.806441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/project_deployment_targets_response.py
--rw-r--r--   0        0        0     2473 2024-04-15 13:10:05.806441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/project_deployment_targets_response_all_of.py
--rw-r--r--   0        0        0     1943 2024-04-15 13:10:05.810441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/project_dismiss_notification_request.py
--rw-r--r--   0        0        0     2680 2024-04-15 13:10:05.810441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/project_downloads_response.py
--rw-r--r--   0        0        0     2373 2024-04-15 13:10:05.810441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/project_downloads_response_all_of.py
--rw-r--r--   0        0        0    14783 2024-04-15 13:10:05.810441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/project_info_response.py
--rw-r--r--   0        0        0    14516 2024-04-15 13:10:05.814441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/project_info_response_all_of.py
--rw-r--r--   0        0        0     4174 2024-04-15 13:10:05.814441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/project_info_response_all_of_acquisition_settings.py
--rw-r--r--   0        0        0     2723 2024-04-15 13:10:05.814441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/project_info_response_all_of_compute_time.py
--rw-r--r--   0        0        0     2997 2024-04-15 13:10:05.814441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/project_info_response_all_of_data_summary_per_category.py
--rw-r--r--   0        0        0     3200 2024-04-15 13:10:05.814441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/project_info_response_all_of_deploy_settings.py
--rw-r--r--   0        0        0     2339 2024-04-15 13:10:05.814441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/project_info_response_all_of_experiments.py
--rw-r--r--   0        0        0     2285 2024-04-15 13:10:05.814441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/project_info_response_all_of_impulse.py
--rw-r--r--   0        0        0     2726 2024-04-15 13:10:05.814441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/project_info_response_all_of_performance.py
--rw-r--r--   0        0        0     1977 2024-04-15 13:10:05.814441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/project_info_response_all_of_readme.py
--rw-r--r--   0        0        0     2225 2024-04-15 13:10:05.814441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/project_info_response_all_of_show_getting_started_wizard.py
--rw-r--r--   0        0        0     2735 2024-04-15 13:10:05.814441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/project_info_response_all_of_urls.py
--rw-r--r--   0        0        0     2478 2024-04-15 13:10:05.814441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/project_info_summary_response.py
--rw-r--r--   0        0        0     2172 2024-04-15 13:10:05.814441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/project_info_summary_response_all_of.py
--rw-r--r--   0        0        0     3554 2024-04-15 13:10:05.814441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/project_private_data.py
--rw-r--r--   0        0        0     4127 2024-04-15 13:10:05.814441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/project_public_data.py
--rw-r--r--   0        0        0     1928 2024-04-15 13:10:05.814441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/project_public_data_readme.py
--rw-r--r--   0        0        0     2404 2024-04-15 13:10:05.814441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/project_sample_metadata.py
--rw-r--r--   0        0        0      576 2024-04-15 13:10:05.818441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/project_tier_enum.py
--rw-r--r--   0        0        0     2804 2024-04-15 13:10:05.818441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/project_training_data_summary_response.py
--rw-r--r--   0        0        0     2487 2024-04-15 13:10:05.818441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/project_training_data_summary_response_all_of.py
--rw-r--r--   0        0        0     2253 2024-04-15 13:10:05.818441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/project_training_data_summary_response_all_of_data_summary.py
--rw-r--r--   0        0        0      606 2024-04-15 13:10:05.818441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/project_type.py
--rw-r--r--   0        0        0     2316 2024-04-15 13:10:05.818441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/project_version_request.py
--rw-r--r--   0        0        0      504 2024-04-15 13:10:05.818441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/project_visibility.py
--rw-r--r--   0        0        0     4991 2024-04-15 13:10:05.822441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/public_organization_transformation_block.py
--rw-r--r--   0        0        0     2664 2024-04-15 13:10:05.822441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/raw_sample_data.py
--rw-r--r--   0        0        0     3440 2024-04-15 13:10:05.822441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/raw_sample_payload.py
--rw-r--r--   0        0        0     2537 2024-04-15 13:10:05.822441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/rebalance_dataset_response.py
--rw-r--r--   0        0        0     1984 2024-04-15 13:10:05.822441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/remove_collaborator_request.py
--rw-r--r--   0        0        0     1805 2024-04-15 13:10:05.822441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/remove_member_request.py
--rw-r--r--   0        0        0     1867 2024-04-15 13:10:05.822441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/rename_device_request.py
--rw-r--r--   0        0        0     2081 2024-04-15 13:10:05.822441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/rename_portal_file_request.py
--rw-r--r--   0        0        0     1867 2024-04-15 13:10:05.822441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/rename_sample_request.py
--rw-r--r--   0        0        0     2028 2024-04-15 13:10:05.822441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/request_email_verification_request.py
--rw-r--r--   0        0        0     1873 2024-04-15 13:10:05.822441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/request_reset_password_request.py
--rw-r--r--   0        0        0     2031 2024-04-15 13:10:05.822441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/reset_password_request.py
--rw-r--r--   0        0        0     1896 2024-04-15 13:10:05.822441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/resource_range.py
--rw-r--r--   0        0        0     1985 2024-04-15 13:10:05.822441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/restore_project_from_public_request.py
--rw-r--r--   0        0        0     2265 2024-04-15 13:10:05.822441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/restore_project_request.py
--rw-r--r--   0        0        0     2421 2024-04-15 13:10:05.822441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/run_auto_labeler_request.py
--rw-r--r--   0        0        0     2669 2024-04-15 13:10:05.822441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/run_organization_pipeline_response.py
--rw-r--r--   0        0        0     2352 2024-04-15 13:10:05.822441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/run_organization_pipeline_response_all_of.py
--rw-r--r--   0        0        0    11134 2024-04-15 13:10:05.822441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/sample.py
--rw-r--r--   0        0        0     2443 2024-04-15 13:10:05.822441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/sample_bounding_boxes_request.py
--rw-r--r--   0        0        0     2000 2024-04-15 13:10:05.822441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/sample_metadata.py
--rw-r--r--   0        0        0     2517 2024-04-15 13:10:05.822441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/save_auto_labeler_clusters_request.py
--rw-r--r--   0        0        0     2071 2024-04-15 13:10:05.822441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/save_auto_labeler_clusters_request_clusters_inner.py
--rw-r--r--   0        0        0     2341 2024-04-15 13:10:05.822441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/save_auto_labeler_clusters_response.py
--rw-r--r--   0        0        0     2024 2024-04-15 13:10:05.822441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/save_auto_labeler_clusters_response_all_of.py
--rw-r--r--   0        0        0     2756 2024-04-15 13:10:05.822441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/save_pretrained_model_request.py
--rw-r--r--   0        0        0     3327 2024-04-15 13:10:05.822441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/score_trial_response.py
--rw-r--r--   0        0        0     3003 2024-04-15 13:10:05.822441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/score_trial_response_all_of.py
--rw-r--r--   0        0        0     2240 2024-04-15 13:10:05.822441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/score_trial_response_all_of_latency.py
--rw-r--r--   0        0        0     1914 2024-04-15 13:10:05.822441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/score_trial_response_all_of_ram.py
--rw-r--r--   0        0        0     2405 2024-04-15 13:10:05.822441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/segment_sample_request.py
--rw-r--r--   0        0        0     2055 2024-04-15 13:10:05.822441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/segment_sample_request_segments_inner.py
--rw-r--r--   0        0        0     3346 2024-04-15 13:10:05.826441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/send_user_feedback_request.py
--rw-r--r--   0        0        0     1981 2024-04-15 13:10:05.826441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/sensor.py
--rw-r--r--   0        0        0     2142 2024-04-15 13:10:05.826441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/set_anomaly_parameter_request.py
--rw-r--r--   0        0        0     9364 2024-04-15 13:10:05.830441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/set_keras_parameter_request.py
--rw-r--r--   0        0        0     1893 2024-04-15 13:10:05.830441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/set_member_datasets_request.py
--rw-r--r--   0        0        0     1905 2024-04-15 13:10:05.830441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/set_member_role_request.py
--rw-r--r--   0        0        0     2219 2024-04-15 13:10:05.830441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/set_optimize_space_request.py
--rw-r--r--   0        0        0     2254 2024-04-15 13:10:05.830441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/set_optimize_space_request_all_of.py
--rw-r--r--   0        0        0     1923 2024-04-15 13:10:05.830441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/set_organization_data_dataset_request.py
--rw-r--r--   0        0        0     1974 2024-04-15 13:10:05.830441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/set_project_compute_time_request.py
--rw-r--r--   0        0        0     2011 2024-04-15 13:10:05.830441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/set_project_dsp_file_size_request.py
--rw-r--r--   0        0        0     1919 2024-04-15 13:10:05.830441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/set_sample_metadata_request.py
--rw-r--r--   0        0        0     2531 2024-04-15 13:10:05.830441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/set_sample_structured_labels_request.py
--rw-r--r--   0        0        0     1915 2024-04-15 13:10:05.830441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/set_syntiant_posterior_request.py
--rw-r--r--   0        0        0     2140 2024-04-15 13:10:05.830441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/set_user_password_request.py
--rw-r--r--   0        0        0     2536 2024-04-15 13:10:05.830441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/socket_token_response.py
--rw-r--r--   0        0        0     2239 2024-04-15 13:10:05.830441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/socket_token_response_all_of.py
--rw-r--r--   0        0        0     2059 2024-04-15 13:10:05.830441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/socket_token_response_all_of_token.py
--rw-r--r--   0        0        0     1971 2024-04-15 13:10:05.830441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/split_sample_in_frames_request.py
--rw-r--r--   0        0        0     2110 2024-04-15 13:10:05.830441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/staff_info.py
--rw-r--r--   0        0        0     5388 2024-04-15 13:10:05.830441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/start_enterprise_trial_request.py
--rw-r--r--   0        0        0     2226 2024-04-15 13:10:05.830441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/start_job_response.py
--rw-r--r--   0        0        0     1909 2024-04-15 13:10:05.830441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/start_job_response_all_of.py
--rw-r--r--   0        0        0     2883 2024-04-15 13:10:05.830441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/start_performance_calibration_request.py
--rw-r--r--   0        0        0     2838 2024-04-15 13:10:05.830441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/start_sampling_request.py
--rw-r--r--   0        0        0     2189 2024-04-15 13:10:05.830441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/start_sampling_response.py
--rw-r--r--   0        0        0     1892 2024-04-15 13:10:05.830441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/start_sampling_response_all_of.py
--rw-r--r--   0        0        0     2795 2024-04-15 13:10:05.830441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/start_training_request_anomaly.py
--rw-r--r--   0        0        0     1967 2024-04-15 13:10:05.830441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/store_segment_length_request.py
--rw-r--r--   0        0        0     3394 2024-04-15 13:10:05.830441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/structured_classify_result.py
--rw-r--r--   0        0        0     2270 2024-04-15 13:10:05.830441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/structured_label.py
--rw-r--r--   0        0        0     4399 2024-04-15 13:10:05.830441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/target_constraints.py
--rw-r--r--   0        0        0     2923 2024-04-15 13:10:05.830441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/target_constraints_device.py
--rw-r--r--   0        0        0     2347 2024-04-15 13:10:05.830441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/target_memory.py
--rw-r--r--   0        0        0     3751 2024-04-15 13:10:05.834441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/target_processor.py
--rw-r--r--   0        0        0     2433 2024-04-15 13:10:05.834441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/test_pretrained_model_request.py
--rw-r--r--   0        0        0     3074 2024-04-15 13:10:05.834441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/test_pretrained_model_response.py
--rw-r--r--   0        0        0     2784 2024-04-15 13:10:05.834441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/test_pretrained_model_response_all_of.py
--rw-r--r--   0        0        0     3251 2024-04-15 13:10:05.834441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/theme.py
--rw-r--r--   0        0        0     2239 2024-04-15 13:10:05.834441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/theme_colors.py
--rw-r--r--   0        0        0     2764 2024-04-15 13:10:05.834441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/theme_favicon.py
--rw-r--r--   0        0        0     2721 2024-04-15 13:10:05.834441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/theme_logos.py
--rw-r--r--   0        0        0     2245 2024-04-15 13:10:05.834441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/third_party_auth.py
--rw-r--r--   0        0        0     1921 2024-04-15 13:10:05.834441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/time_series_data_point.py
--rw-r--r--   0        0        0     2031 2024-04-15 13:10:05.834441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/track_objects_request.py
--rw-r--r--   0        0        0     2736 2024-04-15 13:10:05.834441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/track_objects_response.py
--rw-r--r--   0        0        0     2436 2024-04-15 13:10:05.834441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/track_objects_response_all_of.py
--rw-r--r--   0        0        0     5380 2024-04-15 13:10:05.834441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/transfer_learning_model.py
--rw-r--r--   0        0        0     2012 2024-04-15 13:10:05.834441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/transfer_ownership_organization_request.py
--rw-r--r--   0        0        0     2585 2024-04-15 13:10:05.834441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/transformation_block_additional_mount_point.py
--rw-r--r--   0        0        0      548 2024-04-15 13:10:05.834441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/transformation_job_operates_on_enum.py
--rw-r--r--   0        0        0      588 2024-04-15 13:10:05.834441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/transformation_job_status_enum.py
--rw-r--r--   0        0        0     2578 2024-04-15 13:10:05.834441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/tuner_create_trial_impulse.py
--rw-r--r--   0        0        0     2462 2024-04-15 13:10:05.834441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/tuner_run.py
--rw-r--r--   0        0        0     2570 2024-04-15 13:10:05.834441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/tuner_space_impulse.py
--rw-r--r--   0        0        0     4991 2024-04-15 13:10:05.838441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/tuner_trial.py
--rw-r--r--   0        0        0     2739 2024-04-15 13:10:05.838441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/tuner_trial_blocks_inner.py
--rw-r--r--   0        0        0     1935 2024-04-15 13:10:05.838441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/tuner_trial_dsp_job_id.py
--rw-r--r--   0        0        0     2211 2024-04-15 13:10:05.838441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/tuner_trial_impulse.py
--rw-r--r--   0        0        0     2028 2024-04-15 13:10:05.838441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/update_job_request.py
--rw-r--r--   0        0        0     2281 2024-04-15 13:10:05.838441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/update_organization_add_collaborator_request.py
--rw-r--r--   0        0        0     2882 2024-04-15 13:10:05.838441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/update_organization_bucket_request.py
--rw-r--r--   0        0        0     2828 2024-04-15 13:10:05.838441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/update_organization_create_empty_project_request.py
--rw-r--r--   0        0        0     2428 2024-04-15 13:10:05.838441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/update_organization_create_project_request.py
--rw-r--r--   0        0        0     2913 2024-04-15 13:10:05.838441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/update_organization_data_campaign_dashboard_request.py
--rw-r--r--   0        0        0     4154 2024-04-15 13:10:05.838441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/update_organization_data_campaign_request.py
--rw-r--r--   0        0        0     2158 2024-04-15 13:10:05.838441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/update_organization_data_item_request.py
--rw-r--r--   0        0        0     2977 2024-04-15 13:10:05.838441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/update_organization_dataset_request.py
--rw-r--r--   0        0        0     2518 2024-04-15 13:10:05.838441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/update_organization_dataset_request_bucket.py
--rw-r--r--   0        0        0     2881 2024-04-15 13:10:05.838441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/update_organization_dsp_block_request.py
--rw-r--r--   0        0        0     2724 2024-04-15 13:10:05.838441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/update_organization_portal_response.py
--rw-r--r--   0        0        0     2445 2024-04-15 13:10:05.838441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/update_organization_portal_response_all_of.py
--rw-r--r--   0        0        0     2766 2024-04-15 13:10:05.838441 edgeimpulse_api-1.49.5/edgeimpulse_api/models/update_organization_request.py
--rw-r--r--   0        0        0     5211 2024-04-15 13:10:05.842440 edgeimpulse_api-1.49.5/edgeimpulse_api/models/update_organization_transfer_learning_block_request.py
--rw-r--r--   0        0        0     6072 2024-04-15 13:10:05.846440 edgeimpulse_api-1.49.5/edgeimpulse_api/models/update_organization_transformation_block_request.py
--rw-r--r--   0        0        0    11806 2024-04-15 13:10:05.846440 edgeimpulse_api-1.49.5/edgeimpulse_api/models/update_project_request.py
--rw-r--r--   0        0        0     1877 2024-04-15 13:10:05.850440 edgeimpulse_api-1.49.5/edgeimpulse_api/models/update_project_tags_request.py
--rw-r--r--   0        0        0     2259 2024-04-15 13:10:05.850440 edgeimpulse_api-1.49.5/edgeimpulse_api/models/update_theme_colors_request.py
--rw-r--r--   0        0        0     2895 2024-04-15 13:10:05.850440 edgeimpulse_api-1.49.5/edgeimpulse_api/models/update_theme_logos_request.py
--rw-r--r--   0        0        0     2205 2024-04-15 13:10:05.850440 edgeimpulse_api-1.49.5/edgeimpulse_api/models/update_third_party_auth_request.py
--rw-r--r--   0        0        0     1865 2024-04-15 13:10:05.850440 edgeimpulse_api-1.49.5/edgeimpulse_api/models/update_tuner_run_request.py
--rw-r--r--   0        0        0     2375 2024-04-15 13:10:05.850440 edgeimpulse_api-1.49.5/edgeimpulse_api/models/update_user_request.py
--rw-r--r--   0        0        0     1886 2024-04-15 13:10:05.850440 edgeimpulse_api-1.49.5/edgeimpulse_api/models/update_version_request.py
--rw-r--r--   0        0        0     2393 2024-04-15 13:10:05.850440 edgeimpulse_api-1.49.5/edgeimpulse_api/models/update_whitelabel_default_deployment_target_request.py
--rw-r--r--   0        0        0     2237 2024-04-15 13:10:05.850440 edgeimpulse_api-1.49.5/edgeimpulse_api/models/update_whitelabel_deployment_options_order_request.py
--rw-r--r--   0        0        0     2125 2024-04-15 13:10:05.850440 edgeimpulse_api-1.49.5/edgeimpulse_api/models/update_whitelabel_deployment_targets_request.py
--rw-r--r--   0        0        0     2155 2024-04-15 13:10:05.850440 edgeimpulse_api-1.49.5/edgeimpulse_api/models/update_whitelabel_learning_blocks_request.py
--rw-r--r--   0        0        0     2059 2024-04-15 13:10:05.850440 edgeimpulse_api-1.49.5/edgeimpulse_api/models/update_whitelabel_request.py
--rw-r--r--   0        0        0     2168 2024-04-15 13:10:05.850440 edgeimpulse_api-1.49.5/edgeimpulse_api/models/upload_asset_response.py
--rw-r--r--   0        0        0     1882 2024-04-15 13:10:05.850440 edgeimpulse_api-1.49.5/edgeimpulse_api/models/upload_asset_response_all_of.py
--rw-r--r--   0        0        0     2199 2024-04-15 13:10:05.850440 edgeimpulse_api-1.49.5/edgeimpulse_api/models/upload_readme_image_response.py
--rw-r--r--   0        0        0     2185 2024-04-15 13:10:05.850440 edgeimpulse_api-1.49.5/edgeimpulse_api/models/upload_user_photo_response.py
--rw-r--r--   0        0        0     1872 2024-04-15 13:10:05.850440 edgeimpulse_api-1.49.5/edgeimpulse_api/models/upload_user_photo_response_all_of.py
--rw-r--r--   0        0        0     3888 2024-04-15 13:10:05.850440 edgeimpulse_api-1.49.5/edgeimpulse_api/models/user.py
--rw-r--r--   0        0        0     1991 2024-04-15 13:10:05.850440 edgeimpulse_api-1.49.5/edgeimpulse_api/models/user_by_third_party_activation_request.py
--rw-r--r--   0        0        0     1956 2024-04-15 13:10:05.850440 edgeimpulse_api-1.49.5/edgeimpulse_api/models/user_delete_totp_mfa_key_request.py
--rw-r--r--   0        0        0     1922 2024-04-15 13:10:05.850440 edgeimpulse_api-1.49.5/edgeimpulse_api/models/user_dismiss_notification_request.py
--rw-r--r--   0        0        0     2192 2024-04-15 13:10:05.850440 edgeimpulse_api-1.49.5/edgeimpulse_api/models/user_experiment.py
--rw-r--r--   0        0        0     2425 2024-04-15 13:10:05.850440 edgeimpulse_api-1.49.5/edgeimpulse_api/models/user_generate_new_mfa_key_response.py
--rw-r--r--   0        0        0     2119 2024-04-15 13:10:05.850440 edgeimpulse_api-1.49.5/edgeimpulse_api/models/user_generate_new_mfa_key_response_all_of.py
--rw-r--r--   0        0        0     4606 2024-04-15 13:10:05.850440 edgeimpulse_api-1.49.5/edgeimpulse_api/models/user_organization.py
--rw-r--r--   0        0        0     2144 2024-04-15 13:10:05.850440 edgeimpulse_api-1.49.5/edgeimpulse_api/models/user_set_totp_mfa_key_request.py
--rw-r--r--   0        0        0     2480 2024-04-15 13:10:05.850440 edgeimpulse_api-1.49.5/edgeimpulse_api/models/user_set_totp_mfa_key_response.py
--rw-r--r--   0        0        0     2191 2024-04-15 13:10:05.850440 edgeimpulse_api-1.49.5/edgeimpulse_api/models/user_set_totp_mfa_key_response_all_of.py
--rw-r--r--   0        0        0      543 2024-04-15 13:10:05.850440 edgeimpulse_api-1.49.5/edgeimpulse_api/models/user_tier_enum.py
--rw-r--r--   0        0        0     1844 2024-04-15 13:10:05.854440 edgeimpulse_api-1.49.5/edgeimpulse_api/models/verify_dsp_block_url_request.py
--rw-r--r--   0        0        0     2604 2024-04-15 13:10:05.854440 edgeimpulse_api-1.49.5/edgeimpulse_api/models/verify_dsp_block_url_response.py
--rw-r--r--   0        0        0     2307 2024-04-15 13:10:05.854440 edgeimpulse_api-1.49.5/edgeimpulse_api/models/verify_dsp_block_url_response_all_of.py
--rw-r--r--   0        0        0     2407 2024-04-15 13:10:05.854440 edgeimpulse_api-1.49.5/edgeimpulse_api/models/verify_dsp_block_url_response_all_of_block.py
--rw-r--r--   0        0        0     2633 2024-04-15 13:10:05.854440 edgeimpulse_api-1.49.5/edgeimpulse_api/models/verify_email_response.py
--rw-r--r--   0        0        0     2354 2024-04-15 13:10:05.854440 edgeimpulse_api-1.49.5/edgeimpulse_api/models/verify_email_response_all_of.py
--rw-r--r--   0        0        0     2708 2024-04-15 13:10:05.854440 edgeimpulse_api-1.49.5/edgeimpulse_api/models/verify_organization_bucket_request.py
--rw-r--r--   0        0        0     3432 2024-04-15 13:10:05.854440 edgeimpulse_api-1.49.5/edgeimpulse_api/models/verify_organization_bucket_response.py
--rw-r--r--   0        0        0     3155 2024-04-15 13:10:05.854440 edgeimpulse_api-1.49.5/edgeimpulse_api/models/verify_organization_bucket_response_all_of.py
--rw-r--r--   0        0        0     2187 2024-04-15 13:10:05.854440 edgeimpulse_api-1.49.5/edgeimpulse_api/models/verify_organization_bucket_response_all_of_files.py
--rw-r--r--   0        0        0     1961 2024-04-15 13:10:05.854440 edgeimpulse_api-1.49.5/edgeimpulse_api/models/verify_organization_existing_bucket_request.py
--rw-r--r--   0        0        0     1937 2024-04-15 13:10:05.854440 edgeimpulse_api-1.49.5/edgeimpulse_api/models/verify_reset_password_request.py
--rw-r--r--   0        0        0     8565 2024-04-15 13:10:05.854440 edgeimpulse_api-1.49.5/edgeimpulse_api/models/whitelabel.py
--rw-r--r--   0        0        0     2534 2024-04-15 13:10:05.854440 edgeimpulse_api-1.49.5/edgeimpulse_api/models/whitelabel_admin_create_organization_request.py
--rw-r--r--   0        0        0     2085 2024-04-15 13:10:05.854440 edgeimpulse_api-1.49.5/edgeimpulse_api/models/whitelabel_all_learning_blocks_inner.py
--rw-r--r--   0        0        0     2120 2024-04-15 13:10:05.854440 edgeimpulse_api-1.49.5/edgeimpulse_api/models/whitelabel_custom_deployment_blocks_inner.py
--rw-r--r--   0        0        0     2885 2024-04-15 13:10:05.854440 edgeimpulse_api-1.49.5/edgeimpulse_api/models/window_settings_response.py
--rw-r--r--   0        0        0     2585 2024-04-15 13:10:05.854440 edgeimpulse_api-1.49.5/edgeimpulse_api/models/window_settings_response_all_of.py
--rw-r--r--   0        0        0     2848 2024-04-15 13:10:05.854440 edgeimpulse_api-1.49.5/edgeimpulse_api/models/window_settings_response_all_of_window_settings.py
--rw-r--r--   0        0        0    12674 2024-04-15 13:10:05.854440 edgeimpulse_api-1.49.5/edgeimpulse_api/rest.py
--rw-r--r--   0        0        0     1019 2024-04-15 13:10:42.038120 edgeimpulse_api-1.49.5/pyproject.toml
--rw-r--r--   0        0        0     1391 1970-01-01 00:00:00.000000 edgeimpulse_api-1.49.5/PKG-INFO
+-rw-r--r--   0        0        0      377 2024-04-16 10:25:57.709049 edgeimpulse_api-1.49.6/README.md
+-rw-r--r--   0        0        0    88508 2024-04-16 10:26:30.092761 edgeimpulse_api-1.49.6/edgeimpulse_api/__init__.py
+-rw-r--r--   0        0        0     2172 2024-04-16 10:25:57.713049 edgeimpulse_api-1.49.6/edgeimpulse_api/api/__init__.py
+-rw-r--r--   0        0        0   386649 2024-04-16 10:25:57.713049 edgeimpulse_api-1.49.6/edgeimpulse_api/api/admin_api.py
+-rw-r--r--   0        0        0    11231 2024-04-16 10:25:57.717049 edgeimpulse_api-1.49.6/edgeimpulse_api/api/auth_api.py
+-rw-r--r--   0        0        0     6235 2024-04-16 10:25:57.717049 edgeimpulse_api-1.49.6/edgeimpulse_api/api/cdn_api.py
+-rw-r--r--   0        0        0    59980 2024-04-16 10:25:57.717049 edgeimpulse_api-1.49.6/edgeimpulse_api/api/classify_api.py
+-rw-r--r--   0        0        0    72480 2024-04-16 10:25:57.721049 edgeimpulse_api-1.49.6/edgeimpulse_api/api/deployment_api.py
+-rw-r--r--   0        0        0    80789 2024-04-16 10:25:57.721049 edgeimpulse_api-1.49.6/edgeimpulse_api/api/devices_api.py
+-rw-r--r--   0        0        0   139045 2024-04-16 10:25:57.721049 edgeimpulse_api-1.49.6/edgeimpulse_api/api/dsp_api.py
+-rw-r--r--   0        0        0    19442 2024-04-16 10:25:57.721049 edgeimpulse_api-1.49.6/edgeimpulse_api/api/email_verification_api.py
+-rw-r--r--   0        0        0     6435 2024-04-16 10:25:57.721049 edgeimpulse_api-1.49.6/edgeimpulse_api/api/export_api.py
+-rw-r--r--   0        0        0     5996 2024-04-16 10:25:57.721049 edgeimpulse_api-1.49.6/edgeimpulse_api/api/feature_flags_api.py
+-rw-r--r--   0        0        0    11921 2024-04-16 10:25:57.721049 edgeimpulse_api-1.49.6/edgeimpulse_api/api/health_api.py
+-rw-r--r--   0        0        0    49621 2024-04-16 10:25:57.725049 edgeimpulse_api-1.49.6/edgeimpulse_api/api/impulse_api.py
+-rw-r--r--   0        0        0   238420 2024-04-16 10:25:57.725049 edgeimpulse_api-1.49.6/edgeimpulse_api/api/jobs_api.py
+-rw-r--r--   0        0        0   154112 2024-04-16 10:25:57.725049 edgeimpulse_api-1.49.6/edgeimpulse_api/api/learn_api.py
+-rw-r--r--   0        0        0     6483 2024-04-16 10:25:57.725049 edgeimpulse_api-1.49.6/edgeimpulse_api/api/login_api.py
+-rw-r--r--   0        0        0    17897 2024-04-16 10:25:57.725049 edgeimpulse_api-1.49.6/edgeimpulse_api/api/metrics_api.py
+-rw-r--r--   0        0        0    85275 2024-04-16 10:25:57.725049 edgeimpulse_api-1.49.6/edgeimpulse_api/api/optimization_api.py
+-rw-r--r--   0        0        0   197840 2024-04-16 10:25:57.725049 edgeimpulse_api-1.49.6/edgeimpulse_api/api/organization_blocks_api.py
+-rw-r--r--   0        0        0    92715 2024-04-16 10:25:57.725049 edgeimpulse_api-1.49.6/edgeimpulse_api/api/organization_create_project_api.py
+-rw-r--r--   0        0        0   331750 2024-04-16 10:25:57.733049 edgeimpulse_api-1.49.6/edgeimpulse_api/api/organization_data_api.py
+-rw-r--r--   0        0        0    80882 2024-04-16 10:25:57.737049 edgeimpulse_api-1.49.6/edgeimpulse_api/api/organization_data_campaigns_api.py
+-rw-r--r--   0        0        0    58218 2024-04-16 10:25:57.737049 edgeimpulse_api-1.49.6/edgeimpulse_api/api/organization_jobs_api.py
+-rw-r--r--   0        0        0    53291 2024-04-16 10:25:57.737049 edgeimpulse_api-1.49.6/edgeimpulse_api/api/organization_pipelines_api.py
+-rw-r--r--   0        0        0    45490 2024-04-16 10:25:57.737049 edgeimpulse_api-1.49.6/edgeimpulse_api/api/organization_portals_api.py
+-rw-r--r--   0        0        0   505317 2024-04-16 10:25:57.745049 edgeimpulse_api-1.49.6/edgeimpulse_api/api/organizations_api.py
+-rw-r--r--   0        0        0    54671 2024-04-16 10:25:57.745049 edgeimpulse_api-1.49.6/edgeimpulse_api/api/performance_calibration_api.py
+-rw-r--r--   0        0        0   270960 2024-04-16 10:25:57.753049 edgeimpulse_api-1.49.6/edgeimpulse_api/api/projects_api.py
+-rw-r--r--   0        0        0   414581 2024-04-16 10:25:57.761049 edgeimpulse_api-1.49.6/edgeimpulse_api/api/raw_data_api.py
+-rw-r--r--   0        0        0    35671 2024-04-16 10:25:57.761049 edgeimpulse_api-1.49.6/edgeimpulse_api/api/themes_api.py
+-rw-r--r--   0        0        0    43486 2024-04-16 10:25:57.761049 edgeimpulse_api-1.49.6/edgeimpulse_api/api/third_party_auth_api.py
+-rw-r--r--   0        0        0    45692 2024-04-16 10:25:57.761049 edgeimpulse_api-1.49.6/edgeimpulse_api/api/upload_portal_api.py
+-rw-r--r--   0        0        0   247228 2024-04-16 10:25:57.761049 edgeimpulse_api-1.49.6/edgeimpulse_api/api/user_api.py
+-rw-r--r--   0        0        0    42135 2024-04-16 10:25:57.761049 edgeimpulse_api-1.49.6/edgeimpulse_api/api/whitelabels_api.py
+-rw-r--r--   0        0        0    29331 2024-04-16 10:25:57.761049 edgeimpulse_api-1.49.6/edgeimpulse_api/api_client.py
+-rw-r--r--   0        0        0    15659 2024-04-16 10:25:57.761049 edgeimpulse_api-1.49.6/edgeimpulse_api/configuration.py
+-rw-r--r--   0        0        0     5113 2024-04-16 10:25:57.761049 edgeimpulse_api-1.49.6/edgeimpulse_api/exceptions.py
+-rw-r--r--   0        0        0    85883 2024-04-16 10:25:57.761049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/__init__.py
+-rw-r--r--   0        0        0     2897 2024-04-16 10:25:57.761049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/activate_user_by_third_party_activation_code_request.py
+-rw-r--r--   0        0        0     1982 2024-04-16 10:25:57.761049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/activate_user_or_verify_email_request.py
+-rw-r--r--   0        0        0     2052 2024-04-16 10:25:57.761049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/add_api_key_request.py
+-rw-r--r--   0        0        0     1963 2024-04-16 10:25:57.761049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/add_collaborator_request.py
+-rw-r--r--   0        0        0     2223 2024-04-16 10:25:57.761049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/add_hmac_key_request.py
+-rw-r--r--   0        0        0     2299 2024-04-16 10:25:57.761049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/add_member_request.py
+-rw-r--r--   0        0        0     2418 2024-04-16 10:25:57.761049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/add_organization_api_key_request.py
+-rw-r--r--   0        0        0     2122 2024-04-16 10:25:57.761049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/add_organization_api_key_request_all_of.py
+-rw-r--r--   0        0        0     2806 2024-04-16 10:25:57.761049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/add_organization_bucket_request.py
+-rw-r--r--   0        0        0     2794 2024-04-16 10:25:57.761049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/add_organization_data_campaign_dashboard_request.py
+-rw-r--r--   0        0        0     2469 2024-04-16 10:25:57.761049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/add_organization_data_campaign_dashboard_response.py
+-rw-r--r--   0        0        0     2152 2024-04-16 10:25:57.761049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/add_organization_data_campaign_dashboard_response_all_of.py
+-rw-r--r--   0        0        0     4230 2024-04-16 10:25:57.761049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/add_organization_data_campaign_request.py
+-rw-r--r--   0        0        0     2359 2024-04-16 10:25:57.761049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/add_organization_data_campaign_response.py
+-rw-r--r--   0        0        0     2042 2024-04-16 10:25:57.761049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/add_organization_data_campaign_response_all_of.py
+-rw-r--r--   0        0        0     2269 2024-04-16 10:25:57.761049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/add_organization_deploy_block_response.py
+-rw-r--r--   0        0        0     2816 2024-04-16 10:25:57.765049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/add_organization_dsp_block_request.py
+-rw-r--r--   0        0        0     2248 2024-04-16 10:25:57.765049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/add_organization_dsp_block_response.py
+-rw-r--r--   0        0        0     2054 2024-04-16 10:25:57.765049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/add_organization_secret_request.py
+-rw-r--r--   0        0        0     2266 2024-04-16 10:25:57.765049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/add_organization_secret_response.py
+-rw-r--r--   0        0        0     1949 2024-04-16 10:25:57.765049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/add_organization_secret_response_all_of.py
+-rw-r--r--   0        0        0     4885 2024-04-16 10:25:57.765049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/add_organization_transfer_learning_block_request.py
+-rw-r--r--   0        0        0     2339 2024-04-16 10:25:57.765049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/add_organization_transfer_learning_block_response.py
+-rw-r--r--   0        0        0     6169 2024-04-16 10:25:57.765049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/add_organization_transformation_block_request.py
+-rw-r--r--   0        0        0     2325 2024-04-16 10:25:57.765049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/add_organization_transformation_block_response.py
+-rw-r--r--   0        0        0     2001 2024-04-16 10:25:57.765049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/add_organization_transformation_block_response_all_of.py
+-rw-r--r--   0        0        0     2659 2024-04-16 10:25:57.765049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/add_project_api_key_request.py
+-rw-r--r--   0        0        0     2370 2024-04-16 10:25:57.765049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/add_project_api_key_request_all_of.py
+-rw-r--r--   0        0        0     1940 2024-04-16 10:25:57.765049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/admin_add_disallowed_email_domain_request.py
+-rw-r--r--   0        0        0     1961 2024-04-16 10:25:57.765049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/admin_add_or_update_sso_domain_id_ps_request.py
+-rw-r--r--   0        0        0     2661 2024-04-16 10:25:57.765049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/admin_add_organization_api_key_request.py
+-rw-r--r--   0        0        0     2542 2024-04-16 10:25:57.765049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/admin_add_organization_user_request.py
+-rw-r--r--   0        0        0     2246 2024-04-16 10:25:57.765049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/admin_add_organization_user_request_all_of.py
+-rw-r--r--   0        0        0     2344 2024-04-16 10:25:57.765049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/admin_add_project_api_key_request.py
+-rw-r--r--   0        0        0     2044 2024-04-16 10:25:57.765049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/admin_add_project_api_key_request_all_of.py
+-rw-r--r--   0        0        0     2146 2024-04-16 10:25:57.765049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/admin_add_project_user_request.py
+-rw-r--r--   0        0        0     2097 2024-04-16 10:25:57.765049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/admin_add_user_request.py
+-rw-r--r--   0        0        0     5903 2024-04-16 10:25:57.765049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/admin_api_organization.py
+-rw-r--r--   0        0        0     2396 2024-04-16 10:25:57.765049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/admin_api_organization_all_of.py
+-rw-r--r--   0        0        0     3259 2024-04-16 10:25:57.765049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/admin_api_project.py
+-rw-r--r--   0        0        0     7087 2024-04-16 10:25:57.769049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/admin_api_user.py
+-rw-r--r--   0        0        0     5318 2024-04-16 10:25:57.769049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/admin_api_user_all_of.py
+-rw-r--r--   0        0        0     2386 2024-04-16 10:25:57.773049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/admin_create_organization_data_export_request.py
+-rw-r--r--   0        0        0     2262 2024-04-16 10:25:57.773049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/admin_create_organization_request.py
+-rw-r--r--   0        0        0     2718 2024-04-16 10:25:57.773049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/admin_create_project_request.py
+-rw-r--r--   0        0        0     1905 2024-04-16 10:25:57.773049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/admin_enable_feature_request.py
+-rw-r--r--   0        0        0     2546 2024-04-16 10:25:57.773049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/admin_get_data_migration_response.py
+-rw-r--r--   0        0        0     2222 2024-04-16 10:25:57.773049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/admin_get_data_migration_response_all_of.py
+-rw-r--r--   0        0        0     2735 2024-04-16 10:25:57.773049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/admin_get_data_migrations_response.py
+-rw-r--r--   0        0        0     2428 2024-04-16 10:25:57.773049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/admin_get_data_migrations_response_all_of.py
+-rw-r--r--   0        0        0     2318 2024-04-16 10:25:57.773049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/admin_get_disallowed_email_domains_response.py
+-rw-r--r--   0        0        0     2022 2024-04-16 10:25:57.773049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/admin_get_disallowed_email_domains_response_all_of.py
+-rw-r--r--   0        0        0     2217 2024-04-16 10:25:57.773049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/admin_get_metrics_response.py
+-rw-r--r--   0        0        0     1910 2024-04-16 10:25:57.773049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/admin_get_metrics_response_all_of.py
+-rw-r--r--   0        0        0     3148 2024-04-16 10:25:57.773049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/admin_get_organization_compute_time_usage_response.py
+-rw-r--r--   0        0        0     2647 2024-04-16 10:25:57.773049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/admin_get_organization_usage_report_response.py
+-rw-r--r--   0        0        0     2323 2024-04-16 10:25:57.773049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/admin_get_organization_usage_report_response_all_of.py
+-rw-r--r--   0        0        0     3029 2024-04-16 10:25:57.773049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/admin_get_organization_usage_reports_response.py
+-rw-r--r--   0        0        0     2729 2024-04-16 10:25:57.773049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/admin_get_organization_usage_reports_response_all_of.py
+-rw-r--r--   0        0        0     3046 2024-04-16 10:25:57.773049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/admin_get_organizations_response.py
+-rw-r--r--   0        0        0     2746 2024-04-16 10:25:57.773049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/admin_get_organizations_response_all_of.py
+-rw-r--r--   0        0        0     3409 2024-04-16 10:25:57.773049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/admin_get_organizations_response_all_of_organizations.py
+-rw-r--r--   0        0        0     2243 2024-04-16 10:25:57.773049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/admin_get_sso_domain_id_ps_response.py
+-rw-r--r--   0        0        0     1947 2024-04-16 10:25:57.773049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/admin_get_sso_domain_id_ps_response_all_of.py
+-rw-r--r--   0        0        0     2914 2024-04-16 10:25:57.773049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/admin_get_sso_settings_response.py
+-rw-r--r--   0        0        0     2614 2024-04-16 10:25:57.773049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/admin_get_sso_settings_response_all_of.py
+-rw-r--r--   0        0        0     2096 2024-04-16 10:25:57.773049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/admin_get_sso_settings_response_all_of_sso_whitelist.py
+-rw-r--r--   0        0        0     2208 2024-04-16 10:25:57.773049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/admin_get_user_ids_response.py
+-rw-r--r--   0        0        0     1901 2024-04-16 10:25:57.773049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/admin_get_user_ids_response_all_of.py
+-rw-r--r--   0        0        0     2245 2024-04-16 10:25:57.773049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/admin_get_user_metrics_response.py
+-rw-r--r--   0        0        0     2452 2024-04-16 10:25:57.773049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/admin_get_user_response.py
+-rw-r--r--   0        0        0     2128 2024-04-16 10:25:57.773049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/admin_get_user_response_all_of.py
+-rw-r--r--   0        0        0     2507 2024-04-16 10:25:57.777049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/admin_get_user_trial_response.py
+-rw-r--r--   0        0        0     2183 2024-04-16 10:25:57.777049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/admin_get_user_trial_response_all_of.py
+-rw-r--r--   0        0        0     2807 2024-04-16 10:25:57.777049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/admin_get_users_response.py
+-rw-r--r--   0        0        0     2500 2024-04-16 10:25:57.777049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/admin_get_users_response_all_of.py
+-rw-r--r--   0        0        0     2878 2024-04-16 10:25:57.777049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/admin_get_users_response_all_of_users.py
+-rw-r--r--   0        0        0     2445 2024-04-16 10:25:57.777049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/admin_list_projects.py
+-rw-r--r--   0        0        0     2836 2024-04-16 10:25:57.777049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/admin_list_projects_response.py
+-rw-r--r--   0        0        0     4245 2024-04-16 10:25:57.777049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/admin_organization_info_response.py
+-rw-r--r--   0        0        0     3084 2024-04-16 10:25:57.777049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/admin_organization_info_response_all_of.py
+-rw-r--r--   0        0        0     2158 2024-04-16 10:25:57.777049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/admin_toggle_data_migration_request.py
+-rw-r--r--   0        0        0     2397 2024-04-16 10:25:57.777049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/admin_update_organization_data_export_request.py
+-rw-r--r--   0        0        0     3936 2024-04-16 10:25:57.777049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/admin_update_organization_request.py
+-rw-r--r--   0        0        0     2015 2024-04-16 10:25:57.777049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/admin_update_user_permissions_request.py
+-rw-r--r--   0        0        0     2830 2024-04-16 10:25:57.777049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/admin_update_user_request.py
+-rw-r--r--   0        0        0     2532 2024-04-16 10:25:57.777049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/admin_update_user_trial_request.py
+-rw-r--r--   0        0        0     2525 2024-04-16 10:25:57.777049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/akida_edge_learning_config.py
+-rw-r--r--   0        0        0      512 2024-04-16 10:25:57.777049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/anomaly_capacity.py
+-rw-r--r--   0        0        0     2512 2024-04-16 10:25:57.777049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/anomaly_gmm_metadata.py
+-rw-r--r--   0        0        0     2212 2024-04-16 10:25:57.777049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/anomaly_gmm_metadata_all_of.py
+-rw-r--r--   0        0        0     5499 2024-04-16 10:25:57.777049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/anomaly_model_metadata.py
+-rw-r--r--   0        0        0     5221 2024-04-16 10:25:57.777049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/anomaly_model_metadata_all_of.py
+-rw-r--r--   0        0        0     2151 2024-04-16 10:25:57.777049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/anomaly_model_metadata_all_of_clusters.py
+-rw-r--r--   0        0        0     4079 2024-04-16 10:25:57.777049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/anomaly_response.py
+-rw-r--r--   0        0        0     3812 2024-04-16 10:25:57.777049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/anomaly_response_all_of.py
+-rw-r--r--   0        0        0     2044 2024-04-16 10:25:57.777049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/anomaly_response_all_of_axes.py
+-rw-r--r--   0        0        0     3188 2024-04-16 10:25:57.781049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/anomaly_result.py
+-rw-r--r--   0        0        0     3029 2024-04-16 10:25:57.781049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/anomaly_trained_features_response.py
+-rw-r--r--   0        0        0     2729 2024-04-16 10:25:57.781049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/anomaly_trained_features_response_all_of.py
+-rw-r--r--   0        0        0     2375 2024-04-16 10:25:57.781049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/anomaly_trained_features_response_all_of_data.py
+-rw-r--r--   0        0        0     3358 2024-04-16 10:25:57.781049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/application_budget.py
+-rw-r--r--   0        0        0      506 2024-04-16 10:25:57.781049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/augmentation_policy_image_enum.py
+-rw-r--r--   0        0        0     3635 2024-04-16 10:25:57.781049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/augmentation_policy_spectrogram.py
+-rw-r--r--   0        0        0     1895 2024-04-16 10:25:57.781049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/autotune_dsp_request.py
+-rw-r--r--   0        0        0      505 2024-04-16 10:25:57.785049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/block_display_category.py
+-rw-r--r--   0        0        0      560 2024-04-16 10:25:57.785049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/block_type.py
+-rw-r--r--   0        0        0     2044 2024-04-16 10:25:57.789049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/bounding_box.py
+-rw-r--r--   0        0        0     2151 2024-04-16 10:25:57.789049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/bounding_box_with_score.py
+-rw-r--r--   0        0        0     2197 2024-04-16 10:25:57.789049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/build_on_device_model_request.py
+-rw-r--r--   0        0        0     2433 2024-04-16 10:25:57.789049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/build_organization_on_device_model_request.py
+-rw-r--r--   0        0        0     2459 2024-04-16 10:25:57.789049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/calculate_data_quality_metrics_request.py
+-rw-r--r--   0        0        0     2041 2024-04-16 10:25:57.789049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/change_password_request.py
+-rw-r--r--   0        0        0     3701 2024-04-16 10:25:57.789049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/classify_job_response.py
+-rw-r--r--   0        0        0     3394 2024-04-16 10:25:57.789049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/classify_job_response_all_of.py
+-rw-r--r--   0        0        0     3769 2024-04-16 10:25:57.789049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/classify_job_response_all_of_accuracy.py
+-rw-r--r--   0        0        0     2055 2024-04-16 10:25:57.789049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/classify_job_response_all_of_accuracy_total_summary.py
+-rw-r--r--   0        0        0     3255 2024-04-16 10:25:57.789049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/classify_job_response_page.py
+-rw-r--r--   0        0        0     2948 2024-04-16 10:25:57.789049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/classify_job_response_page_all_of.py
+-rw-r--r--   0        0        0     4026 2024-04-16 10:25:57.789049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/classify_sample_response.py
+-rw-r--r--   0        0        0     3759 2024-04-16 10:25:57.789049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/classify_sample_response_all_of.py
+-rw-r--r--   0        0        0     6252 2024-04-16 10:25:57.789049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/classify_sample_response_classification.py
+-rw-r--r--   0        0        0     2755 2024-04-16 10:25:57.789049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/classify_sample_response_classification_details.py
+-rw-r--r--   0        0        0     3816 2024-04-16 10:25:57.789049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/classify_sample_v2200_response.py
+-rw-r--r--   0        0        0     3004 2024-04-16 10:25:57.789049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/convert_user_request.py
+-rw-r--r--   0        0        0     3495 2024-04-16 10:25:57.789049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/cosine_similarity_data.py
+-rw-r--r--   0        0        0     3114 2024-04-16 10:25:57.789049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/cosine_similarity_issue.py
+-rw-r--r--   0        0        0     3241 2024-04-16 10:25:57.789049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/cosine_similarity_issue_issues_inner.py
+-rw-r--r--   0        0        0     2484 2024-04-16 10:25:57.789049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/cosine_similarity_issue_issues_inner_windows_inner.py
+-rw-r--r--   0        0        0     2183 2024-04-16 10:25:57.789049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/count_samples_response.py
+-rw-r--r--   0        0        0     1859 2024-04-16 10:25:57.789049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/count_samples_response_all_of.py
+-rw-r--r--   0        0        0     2255 2024-04-16 10:25:57.789049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/create_block_version_response.py
+-rw-r--r--   0        0        0     1938 2024-04-16 10:25:57.789049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/create_block_version_response_all_of.py
+-rw-r--r--   0        0        0     2404 2024-04-16 10:25:57.789049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/create_developer_profile_response.py
+-rw-r--r--   0        0        0     2125 2024-04-16 10:25:57.789049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/create_developer_profile_response_all_of.py
+-rw-r--r--   0        0        0     2387 2024-04-16 10:25:57.789049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/create_device_request.py
+-rw-r--r--   0        0        0     2850 2024-04-16 10:25:57.789049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/create_enterprise_trial_response.py
+-rw-r--r--   0        0        0     2319 2024-04-16 10:25:57.789049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/create_enterprise_trial_response_all_of.py
+-rw-r--r--   0        0        0     6569 2024-04-16 10:25:57.789049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/create_enterprise_trial_user_request.py
+-rw-r--r--   0        0        0     4092 2024-04-16 10:25:57.789049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/create_enterprise_trial_user_request_all_of.py
+-rw-r--r--   0        0        0     2491 2024-04-16 10:25:57.789049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/create_evaluation_user_response.py
+-rw-r--r--   0        0        0     2185 2024-04-16 10:25:57.789049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/create_evaluation_user_response_all_of.py
+-rw-r--r--   0        0        0     2600 2024-04-16 10:25:57.789049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/create_organization_portal_request.py
+-rw-r--r--   0        0        0     2830 2024-04-16 10:25:57.789049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/create_organization_portal_response.py
+-rw-r--r--   0        0        0     2551 2024-04-16 10:25:57.789049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/create_organization_portal_response_all_of.py
+-rw-r--r--   0        0        0     1990 2024-04-16 10:25:57.789049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/create_organization_request.py
+-rw-r--r--   0        0        0     2454 2024-04-16 10:25:57.789049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/create_organization_response.py
+-rw-r--r--   0        0        0     2148 2024-04-16 10:25:57.789049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/create_organization_response_all_of.py
+-rw-r--r--   0        0        0     2155 2024-04-16 10:25:57.789049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/create_organization_usage_report_body.py
+-rw-r--r--   0        0        0     2185 2024-04-16 10:25:57.789049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/create_pipeline_response.py
+-rw-r--r--   0        0        0     2504 2024-04-16 10:25:57.789049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/create_project_request.py
+-rw-r--r--   0        0        0     2378 2024-04-16 10:25:57.789049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/create_project_response.py
+-rw-r--r--   0        0        0     2072 2024-04-16 10:25:57.789049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/create_project_response_all_of.py
+-rw-r--r--   0        0        0     2276 2024-04-16 10:25:57.789049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/create_signed_upload_link_request.py
+-rw-r--r--   0        0        0     2414 2024-04-16 10:25:57.789049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/create_signed_upload_link_response.py
+-rw-r--r--   0        0        0     2135 2024-04-16 10:25:57.789049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/create_signed_upload_link_response_all_of.py
+-rw-r--r--   0        0        0     2413 2024-04-16 10:25:57.789049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/create_third_party_auth_request.py
+-rw-r--r--   0        0        0     2450 2024-04-16 10:25:57.789049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/create_third_party_auth_response.py
+-rw-r--r--   0        0        0     2144 2024-04-16 10:25:57.789049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/create_third_party_auth_response_all_of.py
+-rw-r--r--   0        0        0     4197 2024-04-16 10:25:57.789049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/create_user_request.py
+-rw-r--r--   0        0        0     2393 2024-04-16 10:25:57.789049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/create_user_response.py
+-rw-r--r--   0        0        0     2114 2024-04-16 10:25:57.789049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/create_user_response_all_of.py
+-rw-r--r--   0        0        0     2919 2024-04-16 10:25:57.789049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/create_user_third_party_request.py
+-rw-r--r--   0        0        0     2672 2024-04-16 10:25:57.789049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/create_user_third_party_response.py
+-rw-r--r--   0        0        0     2393 2024-04-16 10:25:57.789049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/create_user_third_party_response_all_of.py
+-rw-r--r--   0        0        0     4384 2024-04-16 10:25:57.789049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/create_whitelabel_request.py
+-rw-r--r--   0        0        0     2438 2024-04-16 10:25:57.789049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/create_whitelabel_response.py
+-rw-r--r--   0        0        0     2121 2024-04-16 10:25:57.789049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/create_whitelabel_response_all_of.py
+-rw-r--r--   0        0        0     2094 2024-04-16 10:25:57.789049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/created_updated_by_user.py
+-rw-r--r--   0        0        0     2051 2024-04-16 10:25:57.789049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/crop_sample_request.py
+-rw-r--r--   0        0        0     2248 2024-04-16 10:25:57.789049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/crop_sample_response.py
+-rw-r--r--   0        0        0     1943 2024-04-16 10:25:57.789049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/crop_sample_response_all_of.py
+-rw-r--r--   0        0        0     2368 2024-04-16 10:25:57.789049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/cross_validation_data.py
+-rw-r--r--   0        0        0     3412 2024-04-16 10:25:57.789049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/cross_validation_data_scores_inner.py
+-rw-r--r--   0        0        0     4054 2024-04-16 10:25:57.789049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/data_campaign.py
+-rw-r--r--   0        0        0     2989 2024-04-16 10:25:57.789049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/data_campaign_dashboard.py
+-rw-r--r--   0        0        0     2786 2024-04-16 10:25:57.789049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/data_campaign_graph.py
+-rw-r--r--   0        0        0     3352 2024-04-16 10:25:57.789049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/data_campaign_graph_x_data_inner.py
+-rw-r--r--   0        0        0     2047 2024-04-16 10:25:57.789049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/data_campaign_graph_x_data_inner_values_inner.py
+-rw-r--r--   0        0        0     1934 2024-04-16 10:25:57.789049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/data_campaign_link.py
+-rw-r--r--   0        0        0     1957 2024-04-16 10:25:57.789049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/data_campaign_query.py
+-rw-r--r--   0        0        0     3292 2024-04-16 10:25:57.789049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/data_explorer_predictions_response.py
+-rw-r--r--   0        0        0     3003 2024-04-16 10:25:57.789049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/data_explorer_predictions_response_all_of.py
+-rw-r--r--   0        0        0     2838 2024-04-16 10:25:57.789049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/data_explorer_settings.py
+-rw-r--r--   0        0        0     2149 2024-04-16 10:25:57.789049 edgeimpulse_api-1.49.6/edgeimpulse_api/models/dataset_ratio_data.py
+-rw-r--r--   0        0        0     2111 2024-04-16 10:25:57.793048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/dataset_ratio_data_ratio.py
+-rw-r--r--   0        0        0     1898 2024-04-16 10:25:57.793048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/delete_portal_file_request.py
+-rw-r--r--   0        0        0     2230 2024-04-16 10:25:57.793048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/dependency_data.py
+-rw-r--r--   0        0        0     2280 2024-04-16 10:25:57.793048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/deploy_pretrained_model_input_audio.py
+-rw-r--r--   0        0        0     2408 2024-04-16 10:25:57.793048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/deploy_pretrained_model_input_image.py
+-rw-r--r--   0        0        0     2155 2024-04-16 10:25:57.793048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/deploy_pretrained_model_input_other.py
+-rw-r--r--   0        0        0     2484 2024-04-16 10:25:57.793048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/deploy_pretrained_model_input_time_series.py
+-rw-r--r--   0        0        0     2344 2024-04-16 10:25:57.793048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/deploy_pretrained_model_model_classification.py
+-rw-r--r--   0        0        0     2780 2024-04-16 10:25:57.793048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/deploy_pretrained_model_model_object_detection.py
+-rw-r--r--   0        0        0     2200 2024-04-16 10:25:57.793048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/deploy_pretrained_model_model_regression.py
+-rw-r--r--   0        0        0     4397 2024-04-16 10:25:57.793048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/deploy_pretrained_model_request.py
+-rw-r--r--   0        0        0     2833 2024-04-16 10:25:57.793048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/deploy_pretrained_model_request_model_info.py
+-rw-r--r--   0        0        0     8503 2024-04-16 10:25:57.793048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/deploy_pretrained_model_request_model_info_input.py
+-rw-r--r--   0        0        0     8065 2024-04-16 10:25:57.793048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/deploy_pretrained_model_request_model_info_model.py
+-rw-r--r--   0        0        0     5950 2024-04-16 10:25:57.793048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/deployment_target.py
+-rw-r--r--   0        0        0     1926 2024-04-16 10:25:57.793048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/deployment_target_badge.py
+-rw-r--r--   0        0        0      737 2024-04-16 10:25:57.793048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/deployment_target_engine.py
+-rw-r--r--   0        0        0     2702 2024-04-16 10:25:57.793048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/deployment_targets_response.py
+-rw-r--r--   0        0        0     2395 2024-04-16 10:25:57.793048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/deployment_targets_response_all_of.py
+-rw-r--r--   0        0        0     2248 2024-04-16 10:25:57.793048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/development_board_created_response.py
+-rw-r--r--   0        0        0     2032 2024-04-16 10:25:57.793048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/development_board_request.py
+-rw-r--r--   0        0        0     2134 2024-04-16 10:25:57.793048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/development_board_request_update.py
+-rw-r--r--   0        0        0     2113 2024-04-16 10:25:57.793048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/development_board_response.py
+-rw-r--r--   0        0        0     2864 2024-04-16 10:25:57.793048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/development_boards_response.py
+-rw-r--r--   0        0        0     2564 2024-04-16 10:25:57.793048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/development_boards_response_all_of.py
+-rw-r--r--   0        0        0     2030 2024-04-16 10:25:57.793048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/development_keys.py
+-rw-r--r--   0        0        0     2400 2024-04-16 10:25:57.793048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/development_keys_response.py
+-rw-r--r--   0        0        0     4816 2024-04-16 10:25:57.793048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/device.py
+-rw-r--r--   0        0        0      516 2024-04-16 10:25:57.793048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/device_debug_stream_type.py
+-rw-r--r--   0        0        0     2811 2024-04-16 10:25:57.793048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/device_inference_info.py
+-rw-r--r--   0        0        0     2199 2024-04-16 10:25:57.793048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/device_name_response.py
+-rw-r--r--   0        0        0     1920 2024-04-16 10:25:57.793048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/device_name_response_all_of.py
+-rw-r--r--   0        0        0     2231 2024-04-16 10:25:57.793048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/device_sensors_inner.py
+-rw-r--r--   0        0        0     2094 2024-04-16 10:25:57.793048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/download.py
+-rw-r--r--   0        0        0     1912 2024-04-16 10:25:57.793048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/download_portal_file_request.py
+-rw-r--r--   0        0        0     2260 2024-04-16 10:25:57.793048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/download_portal_file_response.py
+-rw-r--r--   0        0        0     1954 2024-04-16 10:25:57.793048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/download_portal_file_response_all_of.py
+-rw-r--r--   0        0        0     2724 2024-04-16 10:25:57.793048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/dsp_autotuner_results.py
+-rw-r--r--   0        0        0     2417 2024-04-16 10:25:57.793048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/dsp_autotuner_results_all_of.py
+-rw-r--r--   0        0        0     1968 2024-04-16 10:25:57.793048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/dsp_autotuner_results_all_of_results.py
+-rw-r--r--   0        0        0     3660 2024-04-16 10:25:57.793048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/dsp_block.py
+-rw-r--r--   0        0        0     1834 2024-04-16 10:25:57.793048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/dsp_config_request.py
+-rw-r--r--   0        0        0     3092 2024-04-16 10:25:57.793048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/dsp_config_response.py
+-rw-r--r--   0        0        0     2813 2024-04-16 10:25:57.793048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/dsp_config_response_all_of.py
+-rw-r--r--   0        0        0     3016 2024-04-16 10:25:57.793048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/dsp_feature_importance_response.py
+-rw-r--r--   0        0        0     2728 2024-04-16 10:25:57.793048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/dsp_feature_importance_response_all_of.py
+-rw-r--r--   0        0        0     2058 2024-04-16 10:25:57.793048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/dsp_feature_importance_response_all_of_features.py
+-rw-r--r--   0        0        0     2572 2024-04-16 10:25:57.793048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/dsp_feature_importance_response_all_of_labels.py
+-rw-r--r--   0        0        0     2216 2024-04-16 10:25:57.793048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/dsp_feature_labels_response.py
+-rw-r--r--   0        0        0     1920 2024-04-16 10:25:57.793048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/dsp_feature_labels_response_all_of.py
+-rw-r--r--   0        0        0     2294 2024-04-16 10:25:57.793048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/dsp_group.py
+-rw-r--r--   0        0        0     4216 2024-04-16 10:25:57.797048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/dsp_group_item.py
+-rw-r--r--   0        0        0     2190 2024-04-16 10:25:57.797048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/dsp_group_item_select_options_inner.py
+-rw-r--r--   0        0        0     2195 2024-04-16 10:25:57.797048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/dsp_group_item_show_if.py
+-rw-r--r--   0        0        0     4848 2024-04-16 10:25:57.797048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/dsp_info.py
+-rw-r--r--   0        0        0     2376 2024-04-16 10:25:57.797048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/dsp_info_features.py
+-rw-r--r--   0        0        0     1885 2024-04-16 10:25:57.797048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/dsp_info_performance.py
+-rw-r--r--   0        0        0     5462 2024-04-16 10:25:57.797048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/dsp_metadata.py
+-rw-r--r--   0        0        0     2025 2024-04-16 10:25:57.801048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/dsp_metadata_included_samples_inner.py
+-rw-r--r--   0        0        0     2566 2024-04-16 10:25:57.801048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/dsp_metadata_output_config.py
+-rw-r--r--   0        0        0     2531 2024-04-16 10:25:57.801048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/dsp_metadata_output_config_shape.py
+-rw-r--r--   0        0        0     5820 2024-04-16 10:25:57.801048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/dsp_metadata_response.py
+-rw-r--r--   0        0        0     1963 2024-04-16 10:25:57.801048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/dsp_named_axis.py
+-rw-r--r--   0        0        0     3019 2024-04-16 10:25:57.801048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/dsp_performance_all_variants_response.py
+-rw-r--r--   0        0        0     2729 2024-04-16 10:25:57.801048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/dsp_performance_all_variants_response_all_of.py
+-rw-r--r--   0        0        0     2278 2024-04-16 10:25:57.801048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/dsp_performance_all_variants_response_all_of_performance.py
+-rw-r--r--   0        0        0     4639 2024-04-16 10:25:57.801048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/dsp_run_graph.py
+-rw-r--r--   0        0        0     1899 2024-04-16 10:25:57.801048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/dsp_run_graph_axis_labels.py
+-rw-r--r--   0        0        0     2677 2024-04-16 10:25:57.801048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/dsp_run_request_with_features.py
+-rw-r--r--   0        0        0     2151 2024-04-16 10:25:57.801048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/dsp_run_request_without_features.py
+-rw-r--r--   0        0        0     2030 2024-04-16 10:25:57.801048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/dsp_run_request_without_features_read_only.py
+-rw-r--r--   0        0        0     3697 2024-04-16 10:25:57.805048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/dsp_run_response.py
+-rw-r--r--   0        0        0     3418 2024-04-16 10:25:57.805048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/dsp_run_response_all_of.py
+-rw-r--r--   0        0        0     1969 2024-04-16 10:25:57.805048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/dsp_run_response_all_of_performance.py
+-rw-r--r--   0        0        0     4579 2024-04-16 10:25:57.805048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/dsp_run_response_with_sample.py
+-rw-r--r--   0        0        0     4312 2024-04-16 10:25:57.805048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/dsp_run_response_with_sample_all_of.py
+-rw-r--r--   0        0        0     3342 2024-04-16 10:25:57.805048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/dsp_sample_features_response.py
+-rw-r--r--   0        0        0     3042 2024-04-16 10:25:57.805048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/dsp_sample_features_response_all_of.py
+-rw-r--r--   0        0        0     2748 2024-04-16 10:25:57.805048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/dsp_sample_features_response_all_of_data.py
+-rw-r--r--   0        0        0     2213 2024-04-16 10:25:57.805048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/dsp_sample_features_response_all_of_sample.py
+-rw-r--r--   0        0        0     3353 2024-04-16 10:25:57.805048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/dsp_trained_features_response.py
+-rw-r--r--   0        0        0     3053 2024-04-16 10:25:57.805048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/dsp_trained_features_response_all_of.py
+-rw-r--r--   0        0        0     2773 2024-04-16 10:25:57.805048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/dsp_trained_features_response_all_of_data.py
+-rw-r--r--   0        0        0     2205 2024-04-16 10:25:57.805048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/dsp_trained_features_response_all_of_sample.py
+-rw-r--r--   0        0        0     1893 2024-04-16 10:25:57.805048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/edit_sample_label_request.py
+-rw-r--r--   0        0        0     4246 2024-04-16 10:25:57.805048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/enterprise_trial.py
+-rw-r--r--   0        0        0     2960 2024-04-16 10:25:57.805048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/enterprise_upgrade_or_trial_extension_request.py
+-rw-r--r--   0        0        0     2885 2024-04-16 10:25:57.805048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/entitlement_limits.py
+-rw-r--r--   0        0        0     2367 2024-04-16 10:25:57.805048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/entity_created_response.py
+-rw-r--r--   0        0        0     2077 2024-04-16 10:25:57.805048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/entity_created_response_all_of.py
+-rw-r--r--   0        0        0     2656 2024-04-16 10:25:57.805048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/evaluate_job_response.py
+-rw-r--r--   0        0        0     2349 2024-04-16 10:25:57.805048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/evaluate_job_response_all_of.py
+-rw-r--r--   0        0        0     2099 2024-04-16 10:25:57.805048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/evaluate_result_value.py
+-rw-r--r--   0        0        0     2366 2024-04-16 10:25:57.805048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/export_block_response.py
+-rw-r--r--   0        0        0     2060 2024-04-16 10:25:57.805048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/export_block_response_all_of.py
+-rw-r--r--   0        0        0     2511 2024-04-16 10:25:57.805048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/export_get_url_response.py
+-rw-r--r--   0        0        0     2244 2024-04-16 10:25:57.805048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/export_get_url_response_all_of.py
+-rw-r--r--   0        0        0     2116 2024-04-16 10:25:57.805048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/export_keras_block_data_request.py
+-rw-r--r--   0        0        0     2373 2024-04-16 10:25:57.805048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/export_original_data_request.py
+-rw-r--r--   0        0        0     2021 2024-04-16 10:25:57.805048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/export_wav_data_request.py
+-rw-r--r--   0        0        0      500 2024-04-16 10:25:57.805048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/feature.py
+-rw-r--r--   0        0        0     2206 2024-04-16 10:25:57.805048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/find_segment_sample_request.py
+-rw-r--r--   0        0        0     2804 2024-04-16 10:25:57.805048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/find_segment_sample_response.py
+-rw-r--r--   0        0        0     2497 2024-04-16 10:25:57.805048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/find_segment_sample_response_all_of.py
+-rw-r--r--   0        0        0     2090 2024-04-16 10:25:57.805048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/find_segment_sample_response_all_of_segments.py
+-rw-r--r--   0        0        0     2665 2024-04-16 10:25:57.805048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/find_user_response.py
+-rw-r--r--   0        0        0     2358 2024-04-16 10:25:57.805048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/find_user_response_all_of.py
+-rw-r--r--   0        0        0     2322 2024-04-16 10:25:57.805048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/find_user_response_all_of_users.py
+-rw-r--r--   0        0        0     2507 2024-04-16 10:25:57.805048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/generate_features_request.py
+-rw-r--r--   0        0        0     2083 2024-04-16 10:25:57.805048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/generic_api_response.py
+-rw-r--r--   0        0        0     2764 2024-04-16 10:25:57.805048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_all_imported_from_response.py
+-rw-r--r--   0        0        0     2457 2024-04-16 10:25:57.805048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_all_imported_from_response_all_of.py
+-rw-r--r--   0        0        0     2156 2024-04-16 10:25:57.805048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_all_imported_from_response_all_of_data.py
+-rw-r--r--   0        0        0     2698 2024-04-16 10:25:57.805048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_all_third_party_auth_response.py
+-rw-r--r--   0        0        0     2391 2024-04-16 10:25:57.805048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_all_third_party_auth_response_all_of.py
+-rw-r--r--   0        0        0     2713 2024-04-16 10:25:57.805048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_all_whitelabels_response.py
+-rw-r--r--   0        0        0     2406 2024-04-16 10:25:57.805048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_all_whitelabels_response_all_of.py
+-rw-r--r--   0        0        0     3527 2024-04-16 10:25:57.805048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_auto_labeler_response.py
+-rw-r--r--   0        0        0     3260 2024-04-16 10:25:57.805048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_auto_labeler_response_all_of.py
+-rw-r--r--   0        0        0     2588 2024-04-16 10:25:57.805048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_auto_labeler_response_all_of_clusters.py
+-rw-r--r--   0        0        0     1954 2024-04-16 10:25:57.805048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_auto_labeler_response_all_of_items.py
+-rw-r--r--   0        0        0     2345 2024-04-16 10:25:57.805048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_csv_wizard_uploaded_file_info.py
+-rw-r--r--   0        0        0     2078 2024-04-16 10:25:57.805048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_csv_wizard_uploaded_file_info_all_of.py
+-rw-r--r--   0        0        0     3400 2024-04-16 10:25:57.805048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_data_explorer_features_response.py
+-rw-r--r--   0        0        0     3122 2024-04-16 10:25:57.805048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_data_explorer_features_response_all_of.py
+-rw-r--r--   0        0        0     3752 2024-04-16 10:25:57.805048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_data_explorer_settings_response.py
+-rw-r--r--   0        0        0     2402 2024-04-16 10:25:57.805048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_data_explorer_settings_response_all_of.py
+-rw-r--r--   0        0        0     2349 2024-04-16 10:25:57.805048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_deployment_response.py
+-rw-r--r--   0        0        0     2071 2024-04-16 10:25:57.805048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_deployment_response_all_of.py
+-rw-r--r--   0        0        0     2434 2024-04-16 10:25:57.805048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_device_response.py
+-rw-r--r--   0        0        0     2137 2024-04-16 10:25:57.805048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_device_response_all_of.py
+-rw-r--r--   0        0        0     2752 2024-04-16 10:25:57.805048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_diversity_data_response.py
+-rw-r--r--   0        0        0     2455 2024-04-16 10:25:57.805048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_diversity_data_response_all_of.py
+-rw-r--r--   0        0        0     4251 2024-04-16 10:25:57.805048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_diversity_data_response_all_of_cluster_infos.py
+-rw-r--r--   0        0        0     2859 2024-04-16 10:25:57.805048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_diversity_data_response_all_of_data.py
+-rw-r--r--   0        0        0     2456 2024-04-16 10:25:57.805048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_email_verification_code_response.py
+-rw-r--r--   0        0        0     2177 2024-04-16 10:25:57.805048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_email_verification_code_response_all_of.py
+-rw-r--r--   0        0        0     2350 2024-04-16 10:25:57.805048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_email_verification_status_response.py
+-rw-r--r--   0        0        0     2045 2024-04-16 10:25:57.809048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_email_verification_status_response_all_of.py
+-rw-r--r--   0        0        0     2788 2024-04-16 10:25:57.809048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_feature_flags_response.py
+-rw-r--r--   0        0        0     2488 2024-04-16 10:25:57.809048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_feature_flags_response_all_of.py
+-rw-r--r--   0        0        0     2118 2024-04-16 10:25:57.809048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_feature_flags_response_all_of_flags.py
+-rw-r--r--   0        0        0     3930 2024-04-16 10:25:57.809048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_impulse_blocks_response.py
+-rw-r--r--   0        0        0     3630 2024-04-16 10:25:57.809048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_impulse_blocks_response_all_of.py
+-rw-r--r--   0        0        0     2429 2024-04-16 10:25:57.809048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_impulse_records_request.py
+-rw-r--r--   0        0        0     2007 2024-04-16 10:25:57.809048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_impulse_records_request_range.py
+-rw-r--r--   0        0        0     2454 2024-04-16 10:25:57.809048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_impulse_response.py
+-rw-r--r--   0        0        0     2157 2024-04-16 10:25:57.809048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_impulse_response_all_of.py
+-rw-r--r--   0        0        0     2374 2024-04-16 10:25:57.809048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_job_response.py
+-rw-r--r--   0        0        0     2077 2024-04-16 10:25:57.809048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_job_response_all_of.py
+-rw-r--r--   0        0        0     3070 2024-04-16 10:25:57.809048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_jwt_request.py
+-rw-r--r--   0        0        0     2431 2024-04-16 10:25:57.809048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_jwt_response.py
+-rw-r--r--   0        0        0     2152 2024-04-16 10:25:57.809048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_jwt_response_all_of.py
+-rw-r--r--   0        0        0     2580 2024-04-16 10:25:57.809048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_label_noise_data_response.py
+-rw-r--r--   0        0        0     2256 2024-04-16 10:25:57.809048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_label_noise_data_response_all_of.py
+-rw-r--r--   0        0        0     3358 2024-04-16 10:25:57.809048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_label_noise_data_response_all_of_data.py
+-rw-r--r--   0        0        0     3578 2024-04-16 10:25:57.809048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_last_deployment_build_response.py
+-rw-r--r--   0        0        0     3300 2024-04-16 10:25:57.809048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_last_deployment_build_response_all_of.py
+-rw-r--r--   0        0        0     2869 2024-04-16 10:25:57.809048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_last_deployment_build_response_all_of_last_build.py
+-rw-r--r--   0        0        0     2572 2024-04-16 10:25:57.809048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_notes_response.py
+-rw-r--r--   0        0        0     2265 2024-04-16 10:25:57.809048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_notes_response_all_of.py
+-rw-r--r--   0        0        0     2556 2024-04-16 10:25:57.809048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_organization_bucket_response.py
+-rw-r--r--   0        0        0     2232 2024-04-16 10:25:57.809048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_organization_bucket_response_all_of.py
+-rw-r--r--   0        0        0     2701 2024-04-16 10:25:57.809048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_organization_data_campaign_dashboard_response.py
+-rw-r--r--   0        0        0     2377 2024-04-16 10:25:57.809048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_organization_data_campaign_dashboard_response_all_of.py
+-rw-r--r--   0        0        0     2890 2024-04-16 10:25:57.809048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_organization_data_campaign_dashboards_response.py
+-rw-r--r--   0        0        0     2583 2024-04-16 10:25:57.809048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_organization_data_campaign_dashboards_response_all_of.py
+-rw-r--r--   0        0        0     3158 2024-04-16 10:25:57.809048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_organization_data_campaign_response.py
+-rw-r--r--   0        0        0     2939 2024-04-16 10:25:57.809048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_organization_data_campaigns_response.py
+-rw-r--r--   0        0        0     2632 2024-04-16 10:25:57.809048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_organization_data_campaigns_response_all_of.py
+-rw-r--r--   0        0        0     2921 2024-04-16 10:25:57.809048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_organization_data_campaigns_response_all_of_campaigns.py
+-rw-r--r--   0        0        0     2601 2024-04-16 10:25:57.809048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_organization_data_export_response.py
+-rw-r--r--   0        0        0     2277 2024-04-16 10:25:57.809048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_organization_data_export_response_all_of.py
+-rw-r--r--   0        0        0     2982 2024-04-16 10:25:57.809048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_organization_data_exports_response.py
+-rw-r--r--   0        0        0     2682 2024-04-16 10:25:57.809048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_organization_data_exports_response_all_of.py
+-rw-r--r--   0        0        0     2561 2024-04-16 10:25:57.809048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_organization_data_item_response.py
+-rw-r--r--   0        0        0     2237 2024-04-16 10:25:57.809048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_organization_data_item_response_all_of.py
+-rw-r--r--   0        0        0     3411 2024-04-16 10:25:57.809048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_organization_data_item_transform_jobs_response.py
+-rw-r--r--   0        0        0     3111 2024-04-16 10:25:57.809048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_organization_data_item_transform_jobs_response_all_of.py
+-rw-r--r--   0        0        0     3532 2024-04-16 10:25:57.809048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_organization_data_item_transform_jobs_response_all_of_transformation_jobs.py
+-rw-r--r--   0        0        0     2576 2024-04-16 10:25:57.809048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_organization_dataset_response.py
+-rw-r--r--   0        0        0     2252 2024-04-16 10:25:57.809048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_organization_dataset_response_all_of.py
+-rw-r--r--   0        0        0     2690 2024-04-16 10:25:57.809048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_organization_deploy_block_response.py
+-rw-r--r--   0        0        0     2373 2024-04-16 10:25:57.809048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_organization_deploy_block_response_all_of.py
+-rw-r--r--   0        0        0     2627 2024-04-16 10:25:57.809048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_organization_dsp_block_response.py
+-rw-r--r--   0        0        0     2310 2024-04-16 10:25:57.809048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_organization_dsp_block_response_all_of.py
+-rw-r--r--   0        0        0     2603 2024-04-16 10:25:57.809048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_organization_pipelines_response.py
+-rw-r--r--   0        0        0     2279 2024-04-16 10:25:57.809048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_organization_pipelines_response_all_of.py
+-rw-r--r--   0        0        0     3670 2024-04-16 10:25:57.809048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_organization_portal_response.py
+-rw-r--r--   0        0        0     3391 2024-04-16 10:25:57.809048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_organization_portal_response_all_of.py
+-rw-r--r--   0        0        0     2323 2024-04-16 10:25:57.809048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_organization_projects_data_count_response.py
+-rw-r--r--   0        0        0     2906 2024-04-16 10:25:57.809048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_organization_transfer_learning_block_response.py
+-rw-r--r--   0        0        0     2589 2024-04-16 10:25:57.809048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_organization_transfer_learning_block_response_all_of.py
+-rw-r--r--   0        0        0     2858 2024-04-16 10:25:57.809048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_organization_transformation_block_response.py
+-rw-r--r--   0        0        0     2541 2024-04-16 10:25:57.809048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_organization_transformation_block_response_all_of.py
+-rw-r--r--   0        0        0     2612 2024-04-16 10:25:57.809048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_organization_usage_report_response.py
+-rw-r--r--   0        0        0     2905 2024-04-16 10:25:57.809048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_performance_calibration_ground_truth_response.py
+-rw-r--r--   0        0        0     2598 2024-04-16 10:25:57.809048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_performance_calibration_ground_truth_response_all_of.py
+-rw-r--r--   0        0        0     3012 2024-04-16 10:25:57.809048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_performance_calibration_parameter_sets_response.py
+-rw-r--r--   0        0        0     2712 2024-04-16 10:25:57.809048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_performance_calibration_parameter_sets_response_all_of.py
+-rw-r--r--   0        0        0     2722 2024-04-16 10:25:57.809048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_performance_calibration_parameters_response.py
+-rw-r--r--   0        0        0     2425 2024-04-16 10:25:57.809048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_performance_calibration_parameters_response_all_of.py
+-rw-r--r--   0        0        0     2922 2024-04-16 10:25:57.809048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_performance_calibration_raw_result_response.py
+-rw-r--r--   0        0        0     2615 2024-04-16 10:25:57.809048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_performance_calibration_raw_result_response_all_of.py
+-rw-r--r--   0        0        0     3151 2024-04-16 10:25:57.809048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_performance_calibration_status_response.py
+-rw-r--r--   0        0        0     2884 2024-04-16 10:25:57.809048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_performance_calibration_status_response_all_of.py
+-rw-r--r--   0        0        0     3761 2024-04-16 10:25:57.809048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_pretrained_model_response.py
+-rw-r--r--   0        0        0     3483 2024-04-16 10:25:57.809048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_pretrained_model_response_all_of.py
+-rw-r--r--   0        0        0     4031 2024-04-16 10:25:57.809048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_pretrained_model_response_all_of_model.py
+-rw-r--r--   0        0        0     2978 2024-04-16 10:25:57.809048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_pretrained_model_response_all_of_model_info.py
+-rw-r--r--   0        0        0     3058 2024-04-16 10:25:57.809048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_pretrained_model_response_all_of_model_profile_info.py
+-rw-r--r--   0        0        0     2397 2024-04-16 10:25:57.809048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_public_metrics_response.py
+-rw-r--r--   0        0        0     2073 2024-04-16 10:25:57.809048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_public_metrics_response_all_of.py
+-rw-r--r--   0        0        0     2767 2024-04-16 10:25:57.809048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_sample_metadata_response.py
+-rw-r--r--   0        0        0     3044 2024-04-16 10:25:57.809048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_sample_response.py
+-rw-r--r--   0        0        0     2462 2024-04-16 10:25:57.809048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_syntiant_posterior_response.py
+-rw-r--r--   0        0        0     2184 2024-04-16 10:25:57.809048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_syntiant_posterior_response_all_of.py
+-rw-r--r--   0        0        0     2694 2024-04-16 10:25:57.809048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_target_constraints_response.py
+-rw-r--r--   0        0        0     2404 2024-04-16 10:25:57.809048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_target_constraints_response_all_of.py
+-rw-r--r--   0        0        0     2414 2024-04-16 10:25:57.809048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_theme_response.py
+-rw-r--r--   0        0        0     2117 2024-04-16 10:25:57.809048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_theme_response_all_of.py
+-rw-r--r--   0        0        0     2592 2024-04-16 10:25:57.809048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_themes_response.py
+-rw-r--r--   0        0        0     2285 2024-04-16 10:25:57.809048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_themes_response_all_of.py
+-rw-r--r--   0        0        0     2495 2024-04-16 10:25:57.809048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_third_party_auth_response.py
+-rw-r--r--   0        0        0     2171 2024-04-16 10:25:57.809048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_third_party_auth_response_all_of.py
+-rw-r--r--   0        0        0     3543 2024-04-16 10:25:57.809048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_user_need_to_set_password_response.py
+-rw-r--r--   0        0        0     3276 2024-04-16 10:25:57.813048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_user_need_to_set_password_response_all_of.py
+-rw-r--r--   0        0        0     7721 2024-04-16 10:25:57.813048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_user_response.py
+-rw-r--r--   0        0        0     5497 2024-04-16 10:25:57.817048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_user_response_all_of.py
+-rw-r--r--   0        0        0     2395 2024-04-16 10:25:57.817048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_user_response_all_of_whitelabels.py
+-rw-r--r--   0        0        0     2307 2024-04-16 10:25:57.817048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_whitelabel_domain_response.py
+-rw-r--r--   0        0        0     2021 2024-04-16 10:25:57.817048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_whitelabel_domain_response_all_of.py
+-rw-r--r--   0        0        0     2514 2024-04-16 10:25:57.817048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_whitelabel_response.py
+-rw-r--r--   0        0        0     2217 2024-04-16 10:25:57.817048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_whitelabel_response_all_of.py
+-rw-r--r--   0        0        0     2776 2024-04-16 10:25:57.817048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/has_data_explorer_features_response.py
+-rw-r--r--   0        0        0     2498 2024-04-16 10:25:57.817048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/has_data_explorer_features_response_all_of.py
+-rw-r--r--   0        0        0      580 2024-04-16 10:25:57.817048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/image_input_scaling.py
+-rw-r--r--   0        0        0     3738 2024-04-16 10:25:57.817048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/impulse.py
+-rw-r--r--   0        0        0     6723 2024-04-16 10:25:57.817048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/impulse_block_version.py
+-rw-r--r--   0        0        0     6814 2024-04-16 10:25:57.817048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/impulse_dsp_block.py
+-rw-r--r--   0        0        0     1967 2024-04-16 10:25:57.817048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/impulse_dsp_block_organization.py
+-rw-r--r--   0        0        0     8958 2024-04-16 10:25:57.817048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/impulse_input_block.py
+-rw-r--r--   0        0        0     5612 2024-04-16 10:25:57.817048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/impulse_learn_block.py
+-rw-r--r--   0        0        0     2627 2024-04-16 10:25:57.817048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/input_block.py
+-rw-r--r--   0        0        0     2323 2024-04-16 10:25:57.817048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/invite_organization_member_request.py
+-rw-r--r--   0        0        0     4172 2024-04-16 10:25:57.821048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/job.py
+-rw-r--r--   0        0        0     2066 2024-04-16 10:25:57.821048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/job_created_by_user.py
+-rw-r--r--   0        0        0     5203 2024-04-16 10:25:57.821048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/job_details.py
+-rw-r--r--   0        0        0     2736 2024-04-16 10:25:57.821048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/job_details_all_of.py
+-rw-r--r--   0        0        0     2613 2024-04-16 10:25:57.821048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/job_details_response.py
+-rw-r--r--   0        0        0     2316 2024-04-16 10:25:57.821048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/job_details_response_all_of.py
+-rw-r--r--   0        0        0     2257 2024-04-16 10:25:57.821048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/job_failure_details.py
+-rw-r--r--   0        0        0     2657 2024-04-16 10:25:57.821048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/job_logs_response.py
+-rw-r--r--   0        0        0     2350 2024-04-16 10:25:57.821048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/job_logs_response_all_of.py
+-rw-r--r--   0        0        0     3297 2024-04-16 10:25:57.821048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/job_metrics_response.py
+-rw-r--r--   0        0        0     3007 2024-04-16 10:25:57.821048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/job_metrics_response_all_of.py
+-rw-r--r--   0        0        0      546 2024-04-16 10:25:57.821048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/job_parent_type_enum.py
+-rw-r--r--   0        0        0     2944 2024-04-16 10:25:57.821048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/job_state.py
+-rw-r--r--   0        0        0     1966 2024-04-16 10:25:57.821048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/job_state_execution_details.py
+-rw-r--r--   0        0        0      598 2024-04-16 10:25:57.821048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/job_status.py
+-rw-r--r--   0        0        0     2965 2024-04-16 10:25:57.821048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/job_step.py
+-rw-r--r--   0        0        0     2713 2024-04-16 10:25:57.821048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/job_summary_response.py
+-rw-r--r--   0        0        0     2406 2024-04-16 10:25:57.821048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/job_summary_response_all_of.py
+-rw-r--r--   0        0        0     2089 2024-04-16 10:25:57.821048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/job_summary_response_all_of_summary.py
+-rw-r--r--   0        0        0     1961 2024-04-16 10:25:57.821048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/keep_device_debug_stream_alive_request.py
+-rw-r--r--   0        0        0     1993 2024-04-16 10:25:57.821048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/keras_custom_metric.py
+-rw-r--r--   0        0        0     2510 2024-04-16 10:25:57.821048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/keras_model_layer.py
+-rw-r--r--   0        0        0     2093 2024-04-16 10:25:57.821048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/keras_model_layer_input.py
+-rw-r--r--   0        0        0     2101 2024-04-16 10:25:57.821048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/keras_model_layer_output.py
+-rw-r--r--   0        0        0     5707 2024-04-16 10:25:57.821048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/keras_model_metadata.py
+-rw-r--r--   0        0        0     5440 2024-04-16 10:25:57.821048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/keras_model_metadata_all_of.py
+-rw-r--r--   0        0        0     5421 2024-04-16 10:25:57.821048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/keras_model_metadata_metrics.py
+-rw-r--r--   0        0        0     4495 2024-04-16 10:25:57.821048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/keras_model_metadata_metrics_on_device_performance_inner.py
+-rw-r--r--   0        0        0     2497 2024-04-16 10:25:57.821048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/keras_model_metadata_metrics_on_device_performance_inner_tflite.py
+-rw-r--r--   0        0        0      562 2024-04-16 10:25:57.821048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/keras_model_type_enum.py
+-rw-r--r--   0        0        0      524 2024-04-16 10:25:57.821048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/keras_model_variant_enum.py
+-rw-r--r--   0        0        0    11377 2024-04-16 10:25:57.821048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/keras_response.py
+-rw-r--r--   0        0        0    11110 2024-04-16 10:25:57.825048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/keras_response_all_of.py
+-rw-r--r--   0        0        0     3392 2024-04-16 10:25:57.825048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/keras_visual_layer.py
+-rw-r--r--   0        0        0     2310 2024-04-16 10:25:57.825048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/keras_visual_layer_type.py
+-rw-r--r--   0        0        0     2529 2024-04-16 10:25:57.825048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/last_modification_date_response.py
+-rw-r--r--   0        0        0     2239 2024-04-16 10:25:57.825048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/last_modification_date_response_all_of.py
+-rw-r--r--   0        0        0     2633 2024-04-16 10:25:57.825048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/latency_device.py
+-rw-r--r--   0        0        0     3146 2024-04-16 10:25:57.829048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/learn_block.py
+-rw-r--r--   0        0        0      933 2024-04-16 10:25:57.829048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/learn_block_type.py
+-rw-r--r--   0        0        0     2788 2024-04-16 10:25:57.829048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_api_keys_response.py
+-rw-r--r--   0        0        0     2488 2024-04-16 10:25:57.829048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_api_keys_response_all_of.py
+-rw-r--r--   0        0        0     2704 2024-04-16 10:25:57.829048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_api_keys_response_all_of_api_keys.py
+-rw-r--r--   0        0        0     2619 2024-04-16 10:25:57.829048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_devices_response.py
+-rw-r--r--   0        0        0     2312 2024-04-16 10:25:57.829048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_devices_response_all_of.py
+-rw-r--r--   0        0        0     2726 2024-04-16 10:25:57.829048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_email_response.py
+-rw-r--r--   0        0        0     2426 2024-04-16 10:25:57.829048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_email_response_all_of.py
+-rw-r--r--   0        0        0     2918 2024-04-16 10:25:57.829048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_email_response_all_of_emails.py
+-rw-r--r--   0        0        0     2767 2024-04-16 10:25:57.829048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_enterprise_trials_response.py
+-rw-r--r--   0        0        0     2467 2024-04-16 10:25:57.829048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_enterprise_trials_response_all_of.py
+-rw-r--r--   0        0        0     2813 2024-04-16 10:25:57.829048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_hmac_keys_response.py
+-rw-r--r--   0        0        0     2513 2024-04-16 10:25:57.829048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_hmac_keys_response_all_of.py
+-rw-r--r--   0        0        0     2381 2024-04-16 10:25:57.829048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_hmac_keys_response_all_of_hmac_keys.py
+-rw-r--r--   0        0        0     2745 2024-04-16 10:25:57.829048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_jobs_response.py
+-rw-r--r--   0        0        0     2445 2024-04-16 10:25:57.829048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_jobs_response_all_of.py
+-rw-r--r--   0        0        0     2200 2024-04-16 10:25:57.829048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_models_response.py
+-rw-r--r--   0        0        0     1910 2024-04-16 10:25:57.829048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_models_response_all_of.py
+-rw-r--r--   0        0        0     2921 2024-04-16 10:25:57.829048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_organization_api_keys_response.py
+-rw-r--r--   0        0        0     2621 2024-04-16 10:25:57.829048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_organization_api_keys_response_all_of.py
+-rw-r--r--   0        0        0     2760 2024-04-16 10:25:57.829048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_organization_api_keys_response_all_of_api_keys.py
+-rw-r--r--   0        0        0     2752 2024-04-16 10:25:57.829048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_organization_buckets_response.py
+-rw-r--r--   0        0        0     2445 2024-04-16 10:25:57.829048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_organization_buckets_response_all_of.py
+-rw-r--r--   0        0        0     2902 2024-04-16 10:25:57.829048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_organization_buckets_user_response.py
+-rw-r--r--   0        0        0     2595 2024-04-16 10:25:57.829048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_organization_buckets_user_response_all_of.py
+-rw-r--r--   0        0        0     2760 2024-04-16 10:25:57.829048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_organization_buckets_user_response_all_of_buckets.py
+-rw-r--r--   0        0        0     3310 2024-04-16 10:25:57.829048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_organization_data_response.py
+-rw-r--r--   0        0        0     3031 2024-04-16 10:25:57.829048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_organization_data_response_all_of.py
+-rw-r--r--   0        0        0     3430 2024-04-16 10:25:57.829048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_organization_data_response_all_of_data.py
+-rw-r--r--   0        0        0     2887 2024-04-16 10:25:57.829048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_organization_deploy_blocks_response.py
+-rw-r--r--   0        0        0     2587 2024-04-16 10:25:57.829048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_organization_deploy_blocks_response_all_of.py
+-rw-r--r--   0        0        0     2824 2024-04-16 10:25:57.829048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_organization_dsp_blocks_response.py
+-rw-r--r--   0        0        0     2524 2024-04-16 10:25:57.829048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_organization_dsp_blocks_response_all_of.py
+-rw-r--r--   0        0        0     3353 2024-04-16 10:25:57.829048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_organization_files_response.py
+-rw-r--r--   0        0        0     3074 2024-04-16 10:25:57.829048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_organization_files_response_all_of.py
+-rw-r--r--   0        0        0     2792 2024-04-16 10:25:57.829048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_organization_pipelines_response.py
+-rw-r--r--   0        0        0     2485 2024-04-16 10:25:57.829048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_organization_pipelines_response_all_of.py
+-rw-r--r--   0        0        0     2857 2024-04-16 10:25:57.829048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_organization_portals_response.py
+-rw-r--r--   0        0        0     2550 2024-04-16 10:25:57.829048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_organization_portals_response_all_of.py
+-rw-r--r--   0        0        0     2858 2024-04-16 10:25:57.829048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_organization_portals_response_all_of_portals.py
+-rw-r--r--   0        0        0     3449 2024-04-16 10:25:57.829048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_organization_projects_data_response.py
+-rw-r--r--   0        0        0     3142 2024-04-16 10:25:57.829048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_organization_projects_data_response_all_of.py
+-rw-r--r--   0        0        0     2271 2024-04-16 10:25:57.829048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_organization_projects_data_response_all_of_projects.py
+-rw-r--r--   0        0        0     2857 2024-04-16 10:25:57.829048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_organization_secrets_response.py
+-rw-r--r--   0        0        0     2550 2024-04-16 10:25:57.829048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_organization_secrets_response_all_of.py
+-rw-r--r--   0        0        0     2819 2024-04-16 10:25:57.829048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_organization_secrets_response_all_of_secrets.py
+-rw-r--r--   0        0        0     3103 2024-04-16 10:25:57.829048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_organization_transfer_learning_blocks_response.py
+-rw-r--r--   0        0        0     2803 2024-04-16 10:25:57.829048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_organization_transfer_learning_blocks_response_all_of.py
+-rw-r--r--   0        0        0     3055 2024-04-16 10:25:57.829048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_organization_transformation_blocks_response.py
+-rw-r--r--   0        0        0     2755 2024-04-16 10:25:57.829048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_organization_transformation_blocks_response_all_of.py
+-rw-r--r--   0        0        0     2988 2024-04-16 10:25:57.829048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_organization_usage_reports_response.py
+-rw-r--r--   0        0        0     2688 2024-04-16 10:25:57.829048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_organization_usage_reports_response_all_of.py
+-rw-r--r--   0        0        0     2786 2024-04-16 10:25:57.829048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_organizations_response.py
+-rw-r--r--   0        0        0     2486 2024-04-16 10:25:57.829048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_organizations_response_all_of.py
+-rw-r--r--   0        0        0     2512 2024-04-16 10:25:57.833048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_portal_files_in_folder_request.py
+-rw-r--r--   0        0        0     2872 2024-04-16 10:25:57.833048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_portal_files_in_folder_response.py
+-rw-r--r--   0        0        0     2593 2024-04-16 10:25:57.833048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_portal_files_in_folder_response_all_of.py
+-rw-r--r--   0        0        0     2290 2024-04-16 10:25:57.833048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_projects.py
+-rw-r--r--   0        0        0     2681 2024-04-16 10:25:57.833048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_projects_response.py
+-rw-r--r--   0        0        0     3122 2024-04-16 10:25:57.833048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_public_organization_transformation_blocks_response.py
+-rw-r--r--   0        0        0     2822 2024-04-16 10:25:57.833048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_public_organization_transformation_blocks_response_all_of.py
+-rw-r--r--   0        0        0     2553 2024-04-16 10:25:57.833048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_public_projects.py
+-rw-r--r--   0        0        0     2944 2024-04-16 10:25:57.833048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_public_projects_response.py
+-rw-r--r--   0        0        0     2815 2024-04-16 10:25:57.833048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_public_versions_response.py
+-rw-r--r--   0        0        0     2508 2024-04-16 10:25:57.833048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_public_versions_response_all_of.py
+-rw-r--r--   0        0        0     2290 2024-04-16 10:25:57.833048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_public_versions_response_all_of_versions.py
+-rw-r--r--   0        0        0     2754 2024-04-16 10:25:57.833048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_samples_response.py
+-rw-r--r--   0        0        0     2454 2024-04-16 10:25:57.833048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_samples_response_all_of.py
+-rw-r--r--   0        0        0     2615 2024-04-16 10:25:57.833048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_tuner_runs_response.py
+-rw-r--r--   0        0        0     2308 2024-04-16 10:25:57.833048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_tuner_runs_response_all_of.py
+-rw-r--r--   0        0        0     3933 2024-04-16 10:25:57.833048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_versions_response.py
+-rw-r--r--   0        0        0     3633 2024-04-16 10:25:57.833048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_versions_response_all_of.py
+-rw-r--r--   0        0        0     2353 2024-04-16 10:25:57.833048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_versions_response_all_of_bucket.py
+-rw-r--r--   0        0        0     2053 2024-04-16 10:25:57.833048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_versions_response_all_of_custom_learn_blocks.py
+-rw-r--r--   0        0        0     3960 2024-04-16 10:25:57.833048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_versions_response_all_of_versions.py
+-rw-r--r--   0        0        0     2367 2024-04-16 10:25:57.833048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/log_analytics_event_request.py
+-rw-r--r--   0        0        0     2900 2024-04-16 10:25:57.833048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/log_stdout_response.py
+-rw-r--r--   0        0        0     2600 2024-04-16 10:25:57.833048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/log_stdout_response_all_of.py
+-rw-r--r--   0        0        0     2441 2024-04-16 10:25:57.833048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/log_stdout_response_all_of_stdout.py
+-rw-r--r--   0        0        0     2191 2024-04-16 10:25:57.833048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/log_website_pageview_request.py
+-rw-r--r--   0        0        0     2217 2024-04-16 10:25:57.833048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/login_response.py
+-rw-r--r--   0        0        0     1911 2024-04-16 10:25:57.833048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/login_response_all_of.py
+-rw-r--r--   0        0        0     2528 2024-04-16 10:25:57.833048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/memory_spec.py
+-rw-r--r--   0        0        0     2746 2024-04-16 10:25:57.837048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/metrics_all_variants_response.py
+-rw-r--r--   0        0        0     2449 2024-04-16 10:25:57.837048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/metrics_all_variants_response_all_of.py
+-rw-r--r--   0        0        0     2128 2024-04-16 10:25:57.841048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/metrics_for_model_variant.py
+-rw-r--r--   0        0        0     2430 2024-04-16 10:25:57.841048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/migration.py
+-rw-r--r--   0        0        0      571 2024-04-16 10:25:57.841048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/model_engine_short_enum.py
+-rw-r--r--   0        0        0     3010 2024-04-16 10:25:57.845048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/model_prediction.py
+-rw-r--r--   0        0        0     2895 2024-04-16 10:25:57.845048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/model_result.py
+-rw-r--r--   0        0        0     5046 2024-04-16 10:25:57.845048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/model_variant_stats.py
+-rw-r--r--   0        0        0     2128 2024-04-16 10:25:57.845048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/move_raw_data_request.py
+-rw-r--r--   0        0        0     2784 2024-04-16 10:25:57.845048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/neighbors_data.py
+-rw-r--r--   0        0        0     3584 2024-04-16 10:25:57.845048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/neighbors_score.py
+-rw-r--r--   0        0        0     2736 2024-04-16 10:25:57.845048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/neighbors_score_neighbor_windows_inner.py
+-rw-r--r--   0        0        0     2687 2024-04-16 10:25:57.845048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/note.py
+-rw-r--r--   0        0        0     2221 2024-04-16 10:25:57.845048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/object_detection_auto_label_request.py
+-rw-r--r--   0        0        0     2994 2024-04-16 10:25:57.845048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/object_detection_auto_label_response.py
+-rw-r--r--   0        0        0     2705 2024-04-16 10:25:57.845048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/object_detection_auto_label_response_all_of.py
+-rw-r--r--   0        0        0     2275 2024-04-16 10:25:57.845048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/object_detection_auto_label_response_all_of_results.py
+-rw-r--r--   0        0        0     2368 2024-04-16 10:25:57.845048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/object_detection_label_queue_count_response.py
+-rw-r--r--   0        0        0     2051 2024-04-16 10:25:57.845048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/object_detection_label_queue_count_response_all_of.py
+-rw-r--r--   0        0        0     2887 2024-04-16 10:25:57.845048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/object_detection_label_queue_response.py
+-rw-r--r--   0        0        0     2580 2024-04-16 10:25:57.845048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/object_detection_label_queue_response_all_of.py
+-rw-r--r--   0        0        0      775 2024-04-16 10:25:57.845048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/object_detection_last_layer.py
+-rw-r--r--   0        0        0     6491 2024-04-16 10:25:57.845048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/optimize_config.py
+-rw-r--r--   0        0        0     6949 2024-04-16 10:25:57.849048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/optimize_config_response.py
+-rw-r--r--   0        0        0     1920 2024-04-16 10:25:57.849048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/optimize_config_response_all_of.py
+-rw-r--r--   0        0        0     2056 2024-04-16 10:25:57.849048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/optimize_config_target_device.py
+-rw-r--r--   0        0        0     2271 2024-04-16 10:25:57.849048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/optimize_dsp_parameters_response.py
+-rw-r--r--   0        0        0     1964 2024-04-16 10:25:57.849048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/optimize_dsp_parameters_response_all_of.py
+-rw-r--r--   0        0        0     2756 2024-04-16 10:25:57.849048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/optimize_space_response.py
+-rw-r--r--   0        0        0     2456 2024-04-16 10:25:57.849048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/optimize_space_response_all_of.py
+-rw-r--r--   0        0        0     5546 2024-04-16 10:25:57.849048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/optimize_state_response.py
+-rw-r--r--   0        0        0     5279 2024-04-16 10:25:57.849048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/optimize_state_response_all_of.py
+-rw-r--r--   0        0        0     3284 2024-04-16 10:25:57.849048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/optimize_state_response_all_of_status.py
+-rw-r--r--   0        0        0     2273 2024-04-16 10:25:57.849048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/optimize_state_response_all_of_workers.py
+-rw-r--r--   0        0        0     2749 2024-04-16 10:25:57.849048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/optimize_transfer_learning_models_response.py
+-rw-r--r--   0        0        0     2425 2024-04-16 10:25:57.849048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/optimize_transfer_learning_models_response_all_of.py
+-rw-r--r--   0        0        0     4717 2024-04-16 10:25:57.849048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/optimize_transfer_learning_models_response_all_of_models.py
+-rw-r--r--   0        0        0     5801 2024-04-16 10:25:57.849048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/organization.py
+-rw-r--r--   0        0        0     2700 2024-04-16 10:25:57.849048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/organization_add_data_folder_request.py
+-rw-r--r--   0        0        0     2498 2024-04-16 10:25:57.849048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/organization_add_data_folder_response.py
+-rw-r--r--   0        0        0     2209 2024-04-16 10:25:57.849048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/organization_add_data_folder_response_all_of.py
+-rw-r--r--   0        0        0     2835 2024-04-16 10:25:57.849048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/organization_add_dataset_request.py
+-rw-r--r--   0        0        0     2493 2024-04-16 10:25:57.849048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/organization_add_dataset_request_bucket.py
+-rw-r--r--   0        0        0     2820 2024-04-16 10:25:57.849048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/organization_bucket.py
+-rw-r--r--   0        0        0     2711 2024-04-16 10:25:57.849048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/organization_compute_time_usage.py
+-rw-r--r--   0        0        0     9492 2024-04-16 10:25:57.849048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/organization_create_project.py
+-rw-r--r--   0        0        0      605 2024-04-16 10:25:57.849048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/organization_create_project_output_dataset_path_rule.py
+-rw-r--r--   0        0        0     2262 2024-04-16 10:25:57.849048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/organization_create_project_path_filter.py
+-rw-r--r--   0        0        0     7464 2024-04-16 10:25:57.849048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/organization_create_project_request.py
+-rw-r--r--   0        0        0     2543 2024-04-16 10:25:57.849048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/organization_create_project_response.py
+-rw-r--r--   0        0        0     2237 2024-04-16 10:25:57.849048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/organization_create_project_response_all_of.py
+-rw-r--r--   0        0        0     2704 2024-04-16 10:25:57.849048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/organization_create_project_status_response.py
+-rw-r--r--   0        0        0     2407 2024-04-16 10:25:57.849048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/organization_create_project_status_response_all_of.py
+-rw-r--r--   0        0        0     2754 2024-04-16 10:25:57.849048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/organization_create_project_transformation_summary.py
+-rw-r--r--   0        0        0    10387 2024-04-16 10:25:57.849048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/organization_create_project_with_files.py
+-rw-r--r--   0        0        0     2744 2024-04-16 10:25:57.849048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/organization_create_project_with_files_all_of.py
+-rw-r--r--   0        0        0     3483 2024-04-16 10:25:57.849048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/organization_create_project_with_files_all_of_files.py
+-rw-r--r--   0        0        0     2559 2024-04-16 10:25:57.849048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/organization_data_campaign_diff_request.py
+-rw-r--r--   0        0        0     2327 2024-04-16 10:25:57.849048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/organization_data_campaign_diff_request_queries_inner.py
+-rw-r--r--   0        0        0     3041 2024-04-16 10:25:57.849048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/organization_data_campaign_diff_response.py
+-rw-r--r--   0        0        0     2741 2024-04-16 10:25:57.849048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/organization_data_campaign_diff_response_all_of.py
+-rw-r--r--   0        0        0     2468 2024-04-16 10:25:57.849048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/organization_data_campaign_diff_response_all_of_queries.py
+-rw-r--r--   0        0        0     3483 2024-04-16 10:25:57.853048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/organization_data_export.py
+-rw-r--r--   0        0        0     3476 2024-04-16 10:25:57.853048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/organization_data_item.py
+-rw-r--r--   0        0        0     2303 2024-04-16 10:25:57.853048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/organization_data_item_files_inner.py
+-rw-r--r--   0        0        0     4007 2024-04-16 10:25:57.853048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/organization_dataset.py
+-rw-r--r--   0        0        0     2800 2024-04-16 10:25:57.853048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/organization_dataset_bucket.py
+-rw-r--r--   0        0        0     6005 2024-04-16 10:25:57.853048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/organization_deploy_block.py
+-rw-r--r--   0        0        0     4962 2024-04-16 10:25:57.853048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/organization_dsp_block.py
+-rw-r--r--   0        0        0     3037 2024-04-16 10:25:57.853048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/organization_get_create_projects_response.py
+-rw-r--r--   0        0        0     2737 2024-04-16 10:25:57.853048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/organization_get_create_projects_response_all_of.py
+-rw-r--r--   0        0        0     7063 2024-04-16 10:25:57.853048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/organization_get_create_projects_response_all_of_jobs.py
+-rw-r--r--   0        0        0     6864 2024-04-16 10:25:57.857048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/organization_info_response.py
+-rw-r--r--   0        0        0     6574 2024-04-16 10:25:57.857048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/organization_info_response_all_of.py
+-rw-r--r--   0        0        0     3915 2024-04-16 10:25:57.857048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/organization_info_response_all_of_cli_lists.py
+-rw-r--r--   0        0        0     2267 2024-04-16 10:25:57.857048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/organization_info_response_all_of_cli_lists_image_input_scaling_options.py
+-rw-r--r--   0        0        0     2338 2024-04-16 10:25:57.857048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/organization_info_response_all_of_cli_lists_object_detection_last_layer_options.py
+-rw-r--r--   0        0        0     2458 2024-04-16 10:25:57.857048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/organization_info_response_all_of_default_compute_limits.py
+-rw-r--r--   0        0        0     2101 2024-04-16 10:25:57.861048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/organization_info_response_all_of_performance.py
+-rw-r--r--   0        0        0      525 2024-04-16 10:25:57.861048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/organization_member_role.py
+-rw-r--r--   0        0        0     2639 2024-04-16 10:25:57.861048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/organization_metrics_response.py
+-rw-r--r--   0        0        0     2315 2024-04-16 10:25:57.861048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/organization_metrics_response_all_of.py
+-rw-r--r--   0        0        0     4480 2024-04-16 10:25:57.861048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/organization_metrics_response_all_of_metrics.py
+-rw-r--r--   0        0        0     6143 2024-04-16 10:25:57.861048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/organization_pipeline.py
+-rw-r--r--   0        0        0     2595 2024-04-16 10:25:57.861048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/organization_pipeline_feeding_into_dataset.py
+-rw-r--r--   0        0        0     2275 2024-04-16 10:25:57.861048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/organization_pipeline_feeding_into_project.py
+-rw-r--r--   0        0        0     2314 2024-04-16 10:25:57.861048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/organization_pipeline_item_count.py
+-rw-r--r--   0        0        0     4129 2024-04-16 10:25:57.861048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/organization_pipeline_run.py
+-rw-r--r--   0        0        0     5330 2024-04-16 10:25:57.861048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/organization_pipeline_run_step.py
+-rw-r--r--   0        0        0     6532 2024-04-16 10:25:57.861048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/organization_pipeline_step.py
+-rw-r--r--   0        0        0     2351 2024-04-16 10:25:57.861048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/organization_projects_data_batch_disable_response.py
+-rw-r--r--   0        0        0     2344 2024-04-16 10:25:57.861048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/organization_projects_data_batch_enable_response.py
+-rw-r--r--   0        0        0     2037 2024-04-16 10:25:57.861048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/organization_projects_data_batch_request.py
+-rw-r--r--   0        0        0     7242 2024-04-16 10:25:57.865048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/organization_transfer_learning_block.py
+-rw-r--r--   0        0        0      611 2024-04-16 10:25:57.865048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/organization_transfer_learning_operates_on.py
+-rw-r--r--   0        0        0     8670 2024-04-16 10:25:57.869048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/organization_transformation_block.py
+-rw-r--r--   0        0        0     3918 2024-04-16 10:25:57.869048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/organization_update_pipeline_body.py
+-rw-r--r--   0        0        0     3351 2024-04-16 10:25:57.869048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/organization_usage_report.py
+-rw-r--r--   0        0        0     4440 2024-04-16 10:25:57.869048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/organization_user.py
+-rw-r--r--   0        0        0     2294 2024-04-16 10:25:57.869048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/organization_user_all_of.py
+-rw-r--r--   0        0        0     2104 2024-04-16 10:25:57.869048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/performance_calibration_detection.py
+-rw-r--r--   0        0        0     3434 2024-04-16 10:25:57.869048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/performance_calibration_false_positive.py
+-rw-r--r--   0        0        0     3770 2024-04-16 10:25:57.869048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/performance_calibration_ground_truth.py
+-rw-r--r--   0        0        0     2477 2024-04-16 10:25:57.869048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/performance_calibration_ground_truth_samples_inner.py
+-rw-r--r--   0        0        0     4880 2024-04-16 10:25:57.869048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/performance_calibration_parameter_set.py
+-rw-r--r--   0        0        0     2255 2024-04-16 10:25:57.869048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/performance_calibration_parameter_set_aggregate_stats.py
+-rw-r--r--   0        0        0     4092 2024-04-16 10:25:57.869048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/performance_calibration_parameter_set_stats_inner.py
+-rw-r--r--   0        0        0     3007 2024-04-16 10:25:57.869048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/performance_calibration_parameters.py
+-rw-r--r--   0        0        0     2585 2024-04-16 10:25:57.869048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/performance_calibration_parameters_standard.py
+-rw-r--r--   0        0        0     2250 2024-04-16 10:25:57.869048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/performance_calibration_raw_detection.py
+-rw-r--r--   0        0        0     2366 2024-04-16 10:25:57.869048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/performance_calibration_save_parameter_set_request.py
+-rw-r--r--   0        0        0     2412 2024-04-16 10:25:57.869048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/performance_calibration_upload_labeled_audio_response.py
+-rw-r--r--   0        0        0     2106 2024-04-16 10:25:57.869048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/performance_calibration_upload_labeled_audio_response_all_of.py
+-rw-r--r--   0        0        0     1839 2024-04-16 10:25:57.869048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/permission.py
+-rw-r--r--   0        0        0     2491 2024-04-16 10:25:57.869048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/portal_file.py
+-rw-r--r--   0        0        0     2537 2024-04-16 10:25:57.869048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/portal_info_response.py
+-rw-r--r--   0        0        0     2666 2024-04-16 10:25:57.869048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/pretrained_model_tensor.py
+-rw-r--r--   0        0        0     2403 2024-04-16 10:25:57.873048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/preview_default_files_in_folder_request.py
+-rw-r--r--   0        0        0     3734 2024-04-16 10:25:57.873048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/preview_default_files_in_folder_response.py
+-rw-r--r--   0        0        0     3467 2024-04-16 10:25:57.877048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/preview_default_files_in_folder_response_all_of.py
+-rw-r--r--   0        0        0     2955 2024-04-16 10:25:57.877048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/profile_model_info.py
+-rw-r--r--   0        0        0     3117 2024-04-16 10:25:57.877048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/profile_model_info_memory.py
+-rw-r--r--   0        0        0     1918 2024-04-16 10:25:57.877048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/profile_model_info_memory_eon.py
+-rw-r--r--   0        0        0     2065 2024-04-16 10:25:57.877048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/profile_model_info_memory_tflite.py
+-rw-r--r--   0        0        0     4335 2024-04-16 10:25:57.877048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/profile_model_table.py
+-rw-r--r--   0        0        0     2780 2024-04-16 10:25:57.877048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/profile_model_table_mcu.py
+-rw-r--r--   0        0        0     3042 2024-04-16 10:25:57.877048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/profile_model_table_mcu_memory.py
+-rw-r--r--   0        0        0     2250 2024-04-16 10:25:57.877048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/profile_model_table_mpu.py
+-rw-r--r--   0        0        0     2201 2024-04-16 10:25:57.877048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/profile_tf_lite_request.py
+-rw-r--r--   0        0        0     3292 2024-04-16 10:25:57.877048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/profile_tf_lite_response.py
+-rw-r--r--   0        0        0     7873 2024-04-16 10:25:57.877048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/project.py
+-rw-r--r--   0        0        0     4103 2024-04-16 10:25:57.877048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/project_collaborator.py
+-rw-r--r--   0        0        0     1895 2024-04-16 10:25:57.881048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/project_collaborator_all_of.py
+-rw-r--r--   0        0        0     2416 2024-04-16 10:25:57.881048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/project_data_axes_summary_response.py
+-rw-r--r--   0        0        0     2116 2024-04-16 10:25:57.881048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/project_data_axes_summary_response_all_of.py
+-rw-r--r--   0        0        0     2281 2024-04-16 10:25:57.881048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/project_data_interval_response.py
+-rw-r--r--   0        0        0     1964 2024-04-16 10:25:57.881048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/project_data_interval_response_all_of.py
+-rw-r--r--   0        0        0     2235 2024-04-16 10:25:57.881048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/project_data_summary.py
+-rw-r--r--   0        0        0     6854 2024-04-16 10:25:57.881048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/project_deployment_target.py
+-rw-r--r--   0        0        0     2706 2024-04-16 10:25:57.881048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/project_deployment_target_all_of.py
+-rw-r--r--   0        0        0     2780 2024-04-16 10:25:57.881048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/project_deployment_targets_response.py
+-rw-r--r--   0        0        0     2473 2024-04-16 10:25:57.881048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/project_deployment_targets_response_all_of.py
+-rw-r--r--   0        0        0     1943 2024-04-16 10:25:57.881048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/project_dismiss_notification_request.py
+-rw-r--r--   0        0        0     2680 2024-04-16 10:25:57.881048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/project_downloads_response.py
+-rw-r--r--   0        0        0     2373 2024-04-16 10:25:57.881048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/project_downloads_response_all_of.py
+-rw-r--r--   0        0        0    14783 2024-04-16 10:25:57.881048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/project_info_response.py
+-rw-r--r--   0        0        0    14516 2024-04-16 10:25:57.885048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/project_info_response_all_of.py
+-rw-r--r--   0        0        0     4174 2024-04-16 10:25:57.885048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/project_info_response_all_of_acquisition_settings.py
+-rw-r--r--   0        0        0     2723 2024-04-16 10:25:57.885048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/project_info_response_all_of_compute_time.py
+-rw-r--r--   0        0        0     2997 2024-04-16 10:25:57.885048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/project_info_response_all_of_data_summary_per_category.py
+-rw-r--r--   0        0        0     3200 2024-04-16 10:25:57.885048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/project_info_response_all_of_deploy_settings.py
+-rw-r--r--   0        0        0     2339 2024-04-16 10:25:57.885048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/project_info_response_all_of_experiments.py
+-rw-r--r--   0        0        0     2285 2024-04-16 10:25:57.885048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/project_info_response_all_of_impulse.py
+-rw-r--r--   0        0        0     2726 2024-04-16 10:25:57.885048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/project_info_response_all_of_performance.py
+-rw-r--r--   0        0        0     1977 2024-04-16 10:25:57.885048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/project_info_response_all_of_readme.py
+-rw-r--r--   0        0        0     2225 2024-04-16 10:25:57.885048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/project_info_response_all_of_show_getting_started_wizard.py
+-rw-r--r--   0        0        0     2735 2024-04-16 10:25:57.885048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/project_info_response_all_of_urls.py
+-rw-r--r--   0        0        0     2478 2024-04-16 10:25:57.885048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/project_info_summary_response.py
+-rw-r--r--   0        0        0     2172 2024-04-16 10:25:57.885048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/project_info_summary_response_all_of.py
+-rw-r--r--   0        0        0     3554 2024-04-16 10:25:57.885048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/project_private_data.py
+-rw-r--r--   0        0        0     4127 2024-04-16 10:25:57.885048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/project_public_data.py
+-rw-r--r--   0        0        0     1928 2024-04-16 10:25:57.885048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/project_public_data_readme.py
+-rw-r--r--   0        0        0     2404 2024-04-16 10:25:57.885048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/project_sample_metadata.py
+-rw-r--r--   0        0        0      576 2024-04-16 10:25:57.889048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/project_tier_enum.py
+-rw-r--r--   0        0        0     2804 2024-04-16 10:25:57.889048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/project_training_data_summary_response.py
+-rw-r--r--   0        0        0     2487 2024-04-16 10:25:57.889048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/project_training_data_summary_response_all_of.py
+-rw-r--r--   0        0        0     2253 2024-04-16 10:25:57.889048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/project_training_data_summary_response_all_of_data_summary.py
+-rw-r--r--   0        0        0      606 2024-04-16 10:25:57.889048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/project_type.py
+-rw-r--r--   0        0        0     2316 2024-04-16 10:25:57.889048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/project_version_request.py
+-rw-r--r--   0        0        0      504 2024-04-16 10:25:57.889048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/project_visibility.py
+-rw-r--r--   0        0        0     4991 2024-04-16 10:25:57.893048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/public_organization_transformation_block.py
+-rw-r--r--   0        0        0     2664 2024-04-16 10:25:57.893048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/raw_sample_data.py
+-rw-r--r--   0        0        0     3440 2024-04-16 10:25:57.893048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/raw_sample_payload.py
+-rw-r--r--   0        0        0     2537 2024-04-16 10:25:57.893048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/rebalance_dataset_response.py
+-rw-r--r--   0        0        0     1984 2024-04-16 10:25:57.893048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/remove_collaborator_request.py
+-rw-r--r--   0        0        0     1805 2024-04-16 10:25:57.893048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/remove_member_request.py
+-rw-r--r--   0        0        0     1867 2024-04-16 10:25:57.893048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/rename_device_request.py
+-rw-r--r--   0        0        0     2081 2024-04-16 10:25:57.893048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/rename_portal_file_request.py
+-rw-r--r--   0        0        0     1867 2024-04-16 10:25:57.893048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/rename_sample_request.py
+-rw-r--r--   0        0        0     2028 2024-04-16 10:25:57.893048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/request_email_verification_request.py
+-rw-r--r--   0        0        0     1873 2024-04-16 10:25:57.893048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/request_reset_password_request.py
+-rw-r--r--   0        0        0     2031 2024-04-16 10:25:57.893048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/reset_password_request.py
+-rw-r--r--   0        0        0     1896 2024-04-16 10:25:57.893048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/resource_range.py
+-rw-r--r--   0        0        0     1985 2024-04-16 10:25:57.893048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/restore_project_from_public_request.py
+-rw-r--r--   0        0        0     2265 2024-04-16 10:25:57.893048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/restore_project_request.py
+-rw-r--r--   0        0        0     2421 2024-04-16 10:25:57.893048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/run_auto_labeler_request.py
+-rw-r--r--   0        0        0     2669 2024-04-16 10:25:57.893048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/run_organization_pipeline_response.py
+-rw-r--r--   0        0        0     2352 2024-04-16 10:25:57.893048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/run_organization_pipeline_response_all_of.py
+-rw-r--r--   0        0        0    11134 2024-04-16 10:25:57.893048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/sample.py
+-rw-r--r--   0        0        0     2443 2024-04-16 10:25:57.893048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/sample_bounding_boxes_request.py
+-rw-r--r--   0        0        0     2000 2024-04-16 10:25:57.893048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/sample_metadata.py
+-rw-r--r--   0        0        0     2517 2024-04-16 10:25:57.893048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/save_auto_labeler_clusters_request.py
+-rw-r--r--   0        0        0     2071 2024-04-16 10:25:57.893048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/save_auto_labeler_clusters_request_clusters_inner.py
+-rw-r--r--   0        0        0     2341 2024-04-16 10:25:57.893048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/save_auto_labeler_clusters_response.py
+-rw-r--r--   0        0        0     2024 2024-04-16 10:25:57.893048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/save_auto_labeler_clusters_response_all_of.py
+-rw-r--r--   0        0        0     2756 2024-04-16 10:25:57.893048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/save_pretrained_model_request.py
+-rw-r--r--   0        0        0     3327 2024-04-16 10:25:57.893048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/score_trial_response.py
+-rw-r--r--   0        0        0     3003 2024-04-16 10:25:57.893048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/score_trial_response_all_of.py
+-rw-r--r--   0        0        0     2240 2024-04-16 10:25:57.893048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/score_trial_response_all_of_latency.py
+-rw-r--r--   0        0        0     1914 2024-04-16 10:25:57.893048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/score_trial_response_all_of_ram.py
+-rw-r--r--   0        0        0     2405 2024-04-16 10:25:57.893048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/segment_sample_request.py
+-rw-r--r--   0        0        0     2055 2024-04-16 10:25:57.893048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/segment_sample_request_segments_inner.py
+-rw-r--r--   0        0        0     3346 2024-04-16 10:25:57.897048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/send_user_feedback_request.py
+-rw-r--r--   0        0        0     1981 2024-04-16 10:25:57.897048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/sensor.py
+-rw-r--r--   0        0        0     2142 2024-04-16 10:25:57.897048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/set_anomaly_parameter_request.py
+-rw-r--r--   0        0        0     9364 2024-04-16 10:25:57.901048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/set_keras_parameter_request.py
+-rw-r--r--   0        0        0     1893 2024-04-16 10:25:57.901048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/set_member_datasets_request.py
+-rw-r--r--   0        0        0     1905 2024-04-16 10:25:57.901048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/set_member_role_request.py
+-rw-r--r--   0        0        0     2219 2024-04-16 10:25:57.901048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/set_optimize_space_request.py
+-rw-r--r--   0        0        0     2254 2024-04-16 10:25:57.901048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/set_optimize_space_request_all_of.py
+-rw-r--r--   0        0        0     1923 2024-04-16 10:25:57.901048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/set_organization_data_dataset_request.py
+-rw-r--r--   0        0        0     1974 2024-04-16 10:25:57.901048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/set_project_compute_time_request.py
+-rw-r--r--   0        0        0     2011 2024-04-16 10:25:57.901048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/set_project_dsp_file_size_request.py
+-rw-r--r--   0        0        0     1919 2024-04-16 10:25:57.901048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/set_sample_metadata_request.py
+-rw-r--r--   0        0        0     2531 2024-04-16 10:25:57.901048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/set_sample_structured_labels_request.py
+-rw-r--r--   0        0        0     1915 2024-04-16 10:25:57.901048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/set_syntiant_posterior_request.py
+-rw-r--r--   0        0        0     2140 2024-04-16 10:25:57.901048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/set_user_password_request.py
+-rw-r--r--   0        0        0     2536 2024-04-16 10:25:57.901048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/socket_token_response.py
+-rw-r--r--   0        0        0     2239 2024-04-16 10:25:57.901048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/socket_token_response_all_of.py
+-rw-r--r--   0        0        0     2059 2024-04-16 10:25:57.901048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/socket_token_response_all_of_token.py
+-rw-r--r--   0        0        0     1971 2024-04-16 10:25:57.901048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/split_sample_in_frames_request.py
+-rw-r--r--   0        0        0     2110 2024-04-16 10:25:57.901048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/staff_info.py
+-rw-r--r--   0        0        0     2292 2024-04-16 10:25:57.901048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/start_device_debug_stream_response.py
+-rw-r--r--   0        0        0     1975 2024-04-16 10:25:57.901048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/start_device_debug_stream_response_all_of.py
+-rw-r--r--   0        0        0     2178 2024-04-16 10:25:57.901048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/start_device_snapshot_debug_stream_request.py
+-rw-r--r--   0        0        0     5388 2024-04-16 10:25:57.901048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/start_enterprise_trial_request.py
+-rw-r--r--   0        0        0     2226 2024-04-16 10:25:57.901048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/start_job_response.py
+-rw-r--r--   0        0        0     1909 2024-04-16 10:25:57.901048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/start_job_response_all_of.py
+-rw-r--r--   0        0        0     2883 2024-04-16 10:25:57.901048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/start_performance_calibration_request.py
+-rw-r--r--   0        0        0     2838 2024-04-16 10:25:57.901048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/start_sampling_request.py
+-rw-r--r--   0        0        0     2189 2024-04-16 10:25:57.901048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/start_sampling_response.py
+-rw-r--r--   0        0        0     1892 2024-04-16 10:25:57.901048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/start_sampling_response_all_of.py
+-rw-r--r--   0        0        0     2795 2024-04-16 10:25:57.901048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/start_training_request_anomaly.py
+-rw-r--r--   0        0        0     1926 2024-04-16 10:25:57.901048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/stop_device_debug_stream_request.py
+-rw-r--r--   0        0        0     1967 2024-04-16 10:25:57.901048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/store_segment_length_request.py
+-rw-r--r--   0        0        0     3394 2024-04-16 10:25:57.901048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/structured_classify_result.py
+-rw-r--r--   0        0        0     2270 2024-04-16 10:25:57.901048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/structured_label.py
+-rw-r--r--   0        0        0     4399 2024-04-16 10:25:57.901048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/target_constraints.py
+-rw-r--r--   0        0        0     2923 2024-04-16 10:25:57.901048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/target_constraints_device.py
+-rw-r--r--   0        0        0     2347 2024-04-16 10:25:57.901048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/target_memory.py
+-rw-r--r--   0        0        0     3751 2024-04-16 10:25:57.905048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/target_processor.py
+-rw-r--r--   0        0        0     2433 2024-04-16 10:25:57.905048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/test_pretrained_model_request.py
+-rw-r--r--   0        0        0     3074 2024-04-16 10:25:57.905048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/test_pretrained_model_response.py
+-rw-r--r--   0        0        0     2784 2024-04-16 10:25:57.905048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/test_pretrained_model_response_all_of.py
+-rw-r--r--   0        0        0     3251 2024-04-16 10:25:57.905048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/theme.py
+-rw-r--r--   0        0        0     2239 2024-04-16 10:25:57.905048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/theme_colors.py
+-rw-r--r--   0        0        0     2764 2024-04-16 10:25:57.905048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/theme_favicon.py
+-rw-r--r--   0        0        0     2721 2024-04-16 10:25:57.905048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/theme_logos.py
+-rw-r--r--   0        0        0     2245 2024-04-16 10:25:57.905048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/third_party_auth.py
+-rw-r--r--   0        0        0     1921 2024-04-16 10:25:57.905048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/time_series_data_point.py
+-rw-r--r--   0        0        0     2031 2024-04-16 10:25:57.905048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/track_objects_request.py
+-rw-r--r--   0        0        0     2736 2024-04-16 10:25:57.905048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/track_objects_response.py
+-rw-r--r--   0        0        0     2436 2024-04-16 10:25:57.905048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/track_objects_response_all_of.py
+-rw-r--r--   0        0        0     5380 2024-04-16 10:25:57.905048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/transfer_learning_model.py
+-rw-r--r--   0        0        0     2012 2024-04-16 10:25:57.905048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/transfer_ownership_organization_request.py
+-rw-r--r--   0        0        0     2585 2024-04-16 10:25:57.905048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/transformation_block_additional_mount_point.py
+-rw-r--r--   0        0        0      548 2024-04-16 10:25:57.905048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/transformation_job_operates_on_enum.py
+-rw-r--r--   0        0        0      588 2024-04-16 10:25:57.905048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/transformation_job_status_enum.py
+-rw-r--r--   0        0        0     2578 2024-04-16 10:25:57.905048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/tuner_create_trial_impulse.py
+-rw-r--r--   0        0        0     2462 2024-04-16 10:25:57.905048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/tuner_run.py
+-rw-r--r--   0        0        0     2570 2024-04-16 10:25:57.905048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/tuner_space_impulse.py
+-rw-r--r--   0        0        0     4991 2024-04-16 10:25:57.905048 edgeimpulse_api-1.49.6/edgeimpulse_api/models/tuner_trial.py
+-rw-r--r--   0        0        0     2739 2024-04-16 10:25:57.909047 edgeimpulse_api-1.49.6/edgeimpulse_api/models/tuner_trial_blocks_inner.py
+-rw-r--r--   0        0        0     1935 2024-04-16 10:25:57.909047 edgeimpulse_api-1.49.6/edgeimpulse_api/models/tuner_trial_dsp_job_id.py
+-rw-r--r--   0        0        0     2211 2024-04-16 10:25:57.909047 edgeimpulse_api-1.49.6/edgeimpulse_api/models/tuner_trial_impulse.py
+-rw-r--r--   0        0        0     2028 2024-04-16 10:25:57.909047 edgeimpulse_api-1.49.6/edgeimpulse_api/models/update_job_request.py
+-rw-r--r--   0        0        0     2281 2024-04-16 10:25:57.909047 edgeimpulse_api-1.49.6/edgeimpulse_api/models/update_organization_add_collaborator_request.py
+-rw-r--r--   0        0        0     2882 2024-04-16 10:25:57.909047 edgeimpulse_api-1.49.6/edgeimpulse_api/models/update_organization_bucket_request.py
+-rw-r--r--   0        0        0     2828 2024-04-16 10:25:57.909047 edgeimpulse_api-1.49.6/edgeimpulse_api/models/update_organization_create_empty_project_request.py
+-rw-r--r--   0        0        0     2428 2024-04-16 10:25:57.909047 edgeimpulse_api-1.49.6/edgeimpulse_api/models/update_organization_create_project_request.py
+-rw-r--r--   0        0        0     2913 2024-04-16 10:25:57.909047 edgeimpulse_api-1.49.6/edgeimpulse_api/models/update_organization_data_campaign_dashboard_request.py
+-rw-r--r--   0        0        0     4154 2024-04-16 10:25:57.909047 edgeimpulse_api-1.49.6/edgeimpulse_api/models/update_organization_data_campaign_request.py
+-rw-r--r--   0        0        0     2158 2024-04-16 10:25:57.909047 edgeimpulse_api-1.49.6/edgeimpulse_api/models/update_organization_data_item_request.py
+-rw-r--r--   0        0        0     2977 2024-04-16 10:25:57.909047 edgeimpulse_api-1.49.6/edgeimpulse_api/models/update_organization_dataset_request.py
+-rw-r--r--   0        0        0     2518 2024-04-16 10:25:57.909047 edgeimpulse_api-1.49.6/edgeimpulse_api/models/update_organization_dataset_request_bucket.py
+-rw-r--r--   0        0        0     2881 2024-04-16 10:25:57.909047 edgeimpulse_api-1.49.6/edgeimpulse_api/models/update_organization_dsp_block_request.py
+-rw-r--r--   0        0        0     2724 2024-04-16 10:25:57.909047 edgeimpulse_api-1.49.6/edgeimpulse_api/models/update_organization_portal_response.py
+-rw-r--r--   0        0        0     2445 2024-04-16 10:25:57.909047 edgeimpulse_api-1.49.6/edgeimpulse_api/models/update_organization_portal_response_all_of.py
+-rw-r--r--   0        0        0     2766 2024-04-16 10:25:57.909047 edgeimpulse_api-1.49.6/edgeimpulse_api/models/update_organization_request.py
+-rw-r--r--   0        0        0     5211 2024-04-16 10:25:57.909047 edgeimpulse_api-1.49.6/edgeimpulse_api/models/update_organization_transfer_learning_block_request.py
+-rw-r--r--   0        0        0     6072 2024-04-16 10:25:57.913047 edgeimpulse_api-1.49.6/edgeimpulse_api/models/update_organization_transformation_block_request.py
+-rw-r--r--   0        0        0    11806 2024-04-16 10:25:57.917047 edgeimpulse_api-1.49.6/edgeimpulse_api/models/update_project_request.py
+-rw-r--r--   0        0        0     1877 2024-04-16 10:25:57.917047 edgeimpulse_api-1.49.6/edgeimpulse_api/models/update_project_tags_request.py
+-rw-r--r--   0        0        0     2259 2024-04-16 10:25:57.917047 edgeimpulse_api-1.49.6/edgeimpulse_api/models/update_theme_colors_request.py
+-rw-r--r--   0        0        0     2895 2024-04-16 10:25:57.917047 edgeimpulse_api-1.49.6/edgeimpulse_api/models/update_theme_logos_request.py
+-rw-r--r--   0        0        0     2205 2024-04-16 10:25:57.917047 edgeimpulse_api-1.49.6/edgeimpulse_api/models/update_third_party_auth_request.py
+-rw-r--r--   0        0        0     1865 2024-04-16 10:25:57.917047 edgeimpulse_api-1.49.6/edgeimpulse_api/models/update_tuner_run_request.py
+-rw-r--r--   0        0        0     2375 2024-04-16 10:25:57.917047 edgeimpulse_api-1.49.6/edgeimpulse_api/models/update_user_request.py
+-rw-r--r--   0        0        0     1886 2024-04-16 10:25:57.917047 edgeimpulse_api-1.49.6/edgeimpulse_api/models/update_version_request.py
+-rw-r--r--   0        0        0     2393 2024-04-16 10:25:57.917047 edgeimpulse_api-1.49.6/edgeimpulse_api/models/update_whitelabel_default_deployment_target_request.py
+-rw-r--r--   0        0        0     2237 2024-04-16 10:25:57.917047 edgeimpulse_api-1.49.6/edgeimpulse_api/models/update_whitelabel_deployment_options_order_request.py
+-rw-r--r--   0        0        0     2125 2024-04-16 10:25:57.917047 edgeimpulse_api-1.49.6/edgeimpulse_api/models/update_whitelabel_deployment_targets_request.py
+-rw-r--r--   0        0        0     2155 2024-04-16 10:25:57.917047 edgeimpulse_api-1.49.6/edgeimpulse_api/models/update_whitelabel_learning_blocks_request.py
+-rw-r--r--   0        0        0     2059 2024-04-16 10:25:57.917047 edgeimpulse_api-1.49.6/edgeimpulse_api/models/update_whitelabel_request.py
+-rw-r--r--   0        0        0     2168 2024-04-16 10:25:57.917047 edgeimpulse_api-1.49.6/edgeimpulse_api/models/upload_asset_response.py
+-rw-r--r--   0        0        0     1882 2024-04-16 10:25:57.917047 edgeimpulse_api-1.49.6/edgeimpulse_api/models/upload_asset_response_all_of.py
+-rw-r--r--   0        0        0     2199 2024-04-16 10:25:57.917047 edgeimpulse_api-1.49.6/edgeimpulse_api/models/upload_readme_image_response.py
+-rw-r--r--   0        0        0     2185 2024-04-16 10:25:57.917047 edgeimpulse_api-1.49.6/edgeimpulse_api/models/upload_user_photo_response.py
+-rw-r--r--   0        0        0     1872 2024-04-16 10:25:57.917047 edgeimpulse_api-1.49.6/edgeimpulse_api/models/upload_user_photo_response_all_of.py
+-rw-r--r--   0        0        0     3888 2024-04-16 10:25:57.917047 edgeimpulse_api-1.49.6/edgeimpulse_api/models/user.py
+-rw-r--r--   0        0        0     1991 2024-04-16 10:25:57.917047 edgeimpulse_api-1.49.6/edgeimpulse_api/models/user_by_third_party_activation_request.py
+-rw-r--r--   0        0        0     1956 2024-04-16 10:25:57.917047 edgeimpulse_api-1.49.6/edgeimpulse_api/models/user_delete_totp_mfa_key_request.py
+-rw-r--r--   0        0        0     1922 2024-04-16 10:25:57.917047 edgeimpulse_api-1.49.6/edgeimpulse_api/models/user_dismiss_notification_request.py
+-rw-r--r--   0        0        0     2192 2024-04-16 10:25:57.917047 edgeimpulse_api-1.49.6/edgeimpulse_api/models/user_experiment.py
+-rw-r--r--   0        0        0     2425 2024-04-16 10:25:57.917047 edgeimpulse_api-1.49.6/edgeimpulse_api/models/user_generate_new_mfa_key_response.py
+-rw-r--r--   0        0        0     2119 2024-04-16 10:25:57.917047 edgeimpulse_api-1.49.6/edgeimpulse_api/models/user_generate_new_mfa_key_response_all_of.py
+-rw-r--r--   0        0        0     4606 2024-04-16 10:25:57.917047 edgeimpulse_api-1.49.6/edgeimpulse_api/models/user_organization.py
+-rw-r--r--   0        0        0     2144 2024-04-16 10:25:57.917047 edgeimpulse_api-1.49.6/edgeimpulse_api/models/user_set_totp_mfa_key_request.py
+-rw-r--r--   0        0        0     2480 2024-04-16 10:25:57.917047 edgeimpulse_api-1.49.6/edgeimpulse_api/models/user_set_totp_mfa_key_response.py
+-rw-r--r--   0        0        0     2191 2024-04-16 10:25:57.917047 edgeimpulse_api-1.49.6/edgeimpulse_api/models/user_set_totp_mfa_key_response_all_of.py
+-rw-r--r--   0        0        0      543 2024-04-16 10:25:57.921047 edgeimpulse_api-1.49.6/edgeimpulse_api/models/user_tier_enum.py
+-rw-r--r--   0        0        0     1844 2024-04-16 10:25:57.921047 edgeimpulse_api-1.49.6/edgeimpulse_api/models/verify_dsp_block_url_request.py
+-rw-r--r--   0        0        0     2604 2024-04-16 10:25:57.921047 edgeimpulse_api-1.49.6/edgeimpulse_api/models/verify_dsp_block_url_response.py
+-rw-r--r--   0        0        0     2307 2024-04-16 10:25:57.921047 edgeimpulse_api-1.49.6/edgeimpulse_api/models/verify_dsp_block_url_response_all_of.py
+-rw-r--r--   0        0        0     3049 2024-04-16 10:25:57.921047 edgeimpulse_api-1.49.6/edgeimpulse_api/models/verify_dsp_block_url_response_all_of_block.py
+-rw-r--r--   0        0        0     2633 2024-04-16 10:25:57.921047 edgeimpulse_api-1.49.6/edgeimpulse_api/models/verify_email_response.py
+-rw-r--r--   0        0        0     2354 2024-04-16 10:25:57.921047 edgeimpulse_api-1.49.6/edgeimpulse_api/models/verify_email_response_all_of.py
+-rw-r--r--   0        0        0     2708 2024-04-16 10:25:57.921047 edgeimpulse_api-1.49.6/edgeimpulse_api/models/verify_organization_bucket_request.py
+-rw-r--r--   0        0        0     3432 2024-04-16 10:25:57.921047 edgeimpulse_api-1.49.6/edgeimpulse_api/models/verify_organization_bucket_response.py
+-rw-r--r--   0        0        0     3155 2024-04-16 10:25:57.921047 edgeimpulse_api-1.49.6/edgeimpulse_api/models/verify_organization_bucket_response_all_of.py
+-rw-r--r--   0        0        0     2187 2024-04-16 10:25:57.921047 edgeimpulse_api-1.49.6/edgeimpulse_api/models/verify_organization_bucket_response_all_of_files.py
+-rw-r--r--   0        0        0     1961 2024-04-16 10:25:57.921047 edgeimpulse_api-1.49.6/edgeimpulse_api/models/verify_organization_existing_bucket_request.py
+-rw-r--r--   0        0        0     1937 2024-04-16 10:25:57.921047 edgeimpulse_api-1.49.6/edgeimpulse_api/models/verify_reset_password_request.py
+-rw-r--r--   0        0        0     8565 2024-04-16 10:25:57.921047 edgeimpulse_api-1.49.6/edgeimpulse_api/models/whitelabel.py
+-rw-r--r--   0        0        0     2534 2024-04-16 10:25:57.921047 edgeimpulse_api-1.49.6/edgeimpulse_api/models/whitelabel_admin_create_organization_request.py
+-rw-r--r--   0        0        0     2085 2024-04-16 10:25:57.921047 edgeimpulse_api-1.49.6/edgeimpulse_api/models/whitelabel_all_learning_blocks_inner.py
+-rw-r--r--   0        0        0     2120 2024-04-16 10:25:57.921047 edgeimpulse_api-1.49.6/edgeimpulse_api/models/whitelabel_custom_deployment_blocks_inner.py
+-rw-r--r--   0        0        0     2885 2024-04-16 10:25:57.921047 edgeimpulse_api-1.49.6/edgeimpulse_api/models/window_settings_response.py
+-rw-r--r--   0        0        0     2585 2024-04-16 10:25:57.921047 edgeimpulse_api-1.49.6/edgeimpulse_api/models/window_settings_response_all_of.py
+-rw-r--r--   0        0        0     2848 2024-04-16 10:25:57.921047 edgeimpulse_api-1.49.6/edgeimpulse_api/models/window_settings_response_all_of_window_settings.py
+-rw-r--r--   0        0        0    12674 2024-04-16 10:25:57.921047 edgeimpulse_api-1.49.6/edgeimpulse_api/rest.py
+-rw-r--r--   0        0        0     1019 2024-04-16 10:26:30.092761 edgeimpulse_api-1.49.6/pyproject.toml
+-rw-r--r--   0        0        0     1391 1970-01-01 00:00:00.000000 edgeimpulse_api-1.49.6/PKG-INFO
```

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/__init__.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
-__version__ = "1.49.5" #DO_NOT_CHANGE_REPLACED_BY_BUILD_SCRIPT
+__version__ = "1.49.6" #DO_NOT_CHANGE_REPLACED_BY_BUILD_SCRIPT
 
 # import apis into sdk package
 from edgeimpulse_api.api.admin_api import AdminApi
 from edgeimpulse_api.api.auth_api import AuthApi
 from edgeimpulse_api.api.cdn_api import CDNApi
 from edgeimpulse_api.api.classify_api import ClassifyApi
 from edgeimpulse_api.api.dsp_api import DSPApi
@@ -247,14 +247,15 @@
 from edgeimpulse_api.models.dsp_info_features import DSPInfoFeatures
 from edgeimpulse_api.models.dsp_info_performance import DSPInfoPerformance
 from edgeimpulse_api.models.dsp_metadata import DSPMetadata
 from edgeimpulse_api.models.dsp_metadata_included_samples_inner import DSPMetadataIncludedSamplesInner
 from edgeimpulse_api.models.dsp_metadata_output_config import DSPMetadataOutputConfig
 from edgeimpulse_api.models.dsp_metadata_output_config_shape import DSPMetadataOutputConfigShape
 from edgeimpulse_api.models.dsp_metadata_response import DSPMetadataResponse
+from edgeimpulse_api.models.dsp_named_axis import DSPNamedAxis
 from edgeimpulse_api.models.data_campaign import DataCampaign
 from edgeimpulse_api.models.data_campaign_dashboard import DataCampaignDashboard
 from edgeimpulse_api.models.data_campaign_graph import DataCampaignGraph
 from edgeimpulse_api.models.data_campaign_graph_x_data_inner import DataCampaignGraphXDataInner
 from edgeimpulse_api.models.data_campaign_graph_x_data_inner_values_inner import DataCampaignGraphXDataInnerValuesInner
 from edgeimpulse_api.models.data_campaign_link import DataCampaignLink
 from edgeimpulse_api.models.data_campaign_query import DataCampaignQuery
@@ -286,14 +287,16 @@
 from edgeimpulse_api.models.development_board_request_update import DevelopmentBoardRequestUpdate
 from edgeimpulse_api.models.development_board_response import DevelopmentBoardResponse
 from edgeimpulse_api.models.development_boards_response import DevelopmentBoardsResponse
 from edgeimpulse_api.models.development_boards_response_all_of import DevelopmentBoardsResponseAllOf
 from edgeimpulse_api.models.development_keys import DevelopmentKeys
 from edgeimpulse_api.models.development_keys_response import DevelopmentKeysResponse
 from edgeimpulse_api.models.device import Device
+from edgeimpulse_api.models.device_debug_stream_type import DeviceDebugStreamType
+from edgeimpulse_api.models.device_inference_info import DeviceInferenceInfo
 from edgeimpulse_api.models.device_name_response import DeviceNameResponse
 from edgeimpulse_api.models.device_name_response_all_of import DeviceNameResponseAllOf
 from edgeimpulse_api.models.device_sensors_inner import DeviceSensorsInner
 from edgeimpulse_api.models.download import Download
 from edgeimpulse_api.models.download_portal_file_request import DownloadPortalFileRequest
 from edgeimpulse_api.models.download_portal_file_response import DownloadPortalFileResponse
 from edgeimpulse_api.models.download_portal_file_response_all_of import DownloadPortalFileResponseAllOf
@@ -383,14 +386,16 @@
 from edgeimpulse_api.models.get_email_verification_status_response import GetEmailVerificationStatusResponse
 from edgeimpulse_api.models.get_email_verification_status_response_all_of import GetEmailVerificationStatusResponseAllOf
 from edgeimpulse_api.models.get_feature_flags_response import GetFeatureFlagsResponse
 from edgeimpulse_api.models.get_feature_flags_response_all_of import GetFeatureFlagsResponseAllOf
 from edgeimpulse_api.models.get_feature_flags_response_all_of_flags import GetFeatureFlagsResponseAllOfFlags
 from edgeimpulse_api.models.get_impulse_blocks_response import GetImpulseBlocksResponse
 from edgeimpulse_api.models.get_impulse_blocks_response_all_of import GetImpulseBlocksResponseAllOf
+from edgeimpulse_api.models.get_impulse_records_request import GetImpulseRecordsRequest
+from edgeimpulse_api.models.get_impulse_records_request_range import GetImpulseRecordsRequestRange
 from edgeimpulse_api.models.get_impulse_response import GetImpulseResponse
 from edgeimpulse_api.models.get_impulse_response_all_of import GetImpulseResponseAllOf
 from edgeimpulse_api.models.get_jwt_request import GetJWTRequest
 from edgeimpulse_api.models.get_jwt_response import GetJWTResponse
 from edgeimpulse_api.models.get_jwt_response_all_of import GetJWTResponseAllOf
 from edgeimpulse_api.models.get_job_response import GetJobResponse
 from edgeimpulse_api.models.get_job_response_all_of import GetJobResponseAllOf
@@ -501,14 +506,15 @@
 from edgeimpulse_api.models.job_state import JobState
 from edgeimpulse_api.models.job_state_execution_details import JobStateExecutionDetails
 from edgeimpulse_api.models.job_status import JobStatus
 from edgeimpulse_api.models.job_step import JobStep
 from edgeimpulse_api.models.job_summary_response import JobSummaryResponse
 from edgeimpulse_api.models.job_summary_response_all_of import JobSummaryResponseAllOf
 from edgeimpulse_api.models.job_summary_response_all_of_summary import JobSummaryResponseAllOfSummary
+from edgeimpulse_api.models.keep_device_debug_stream_alive_request import KeepDeviceDebugStreamAliveRequest
 from edgeimpulse_api.models.keras_custom_metric import KerasCustomMetric
 from edgeimpulse_api.models.keras_model_layer import KerasModelLayer
 from edgeimpulse_api.models.keras_model_layer_input import KerasModelLayerInput
 from edgeimpulse_api.models.keras_model_layer_output import KerasModelLayerOutput
 from edgeimpulse_api.models.keras_model_metadata import KerasModelMetadata
 from edgeimpulse_api.models.keras_model_metadata_all_of import KerasModelMetadataAllOf
 from edgeimpulse_api.models.keras_model_metadata_metrics import KerasModelMetadataMetrics
@@ -825,22 +831,26 @@
 from edgeimpulse_api.models.set_syntiant_posterior_request import SetSyntiantPosteriorRequest
 from edgeimpulse_api.models.set_user_password_request import SetUserPasswordRequest
 from edgeimpulse_api.models.socket_token_response import SocketTokenResponse
 from edgeimpulse_api.models.socket_token_response_all_of import SocketTokenResponseAllOf
 from edgeimpulse_api.models.socket_token_response_all_of_token import SocketTokenResponseAllOfToken
 from edgeimpulse_api.models.split_sample_in_frames_request import SplitSampleInFramesRequest
 from edgeimpulse_api.models.staff_info import StaffInfo
+from edgeimpulse_api.models.start_device_debug_stream_response import StartDeviceDebugStreamResponse
+from edgeimpulse_api.models.start_device_debug_stream_response_all_of import StartDeviceDebugStreamResponseAllOf
+from edgeimpulse_api.models.start_device_snapshot_debug_stream_request import StartDeviceSnapshotDebugStreamRequest
 from edgeimpulse_api.models.start_enterprise_trial_request import StartEnterpriseTrialRequest
 from edgeimpulse_api.models.start_job_response import StartJobResponse
 from edgeimpulse_api.models.start_job_response_all_of import StartJobResponseAllOf
 from edgeimpulse_api.models.start_performance_calibration_request import StartPerformanceCalibrationRequest
 from edgeimpulse_api.models.start_sampling_request import StartSamplingRequest
 from edgeimpulse_api.models.start_sampling_response import StartSamplingResponse
 from edgeimpulse_api.models.start_sampling_response_all_of import StartSamplingResponseAllOf
 from edgeimpulse_api.models.start_training_request_anomaly import StartTrainingRequestAnomaly
+from edgeimpulse_api.models.stop_device_debug_stream_request import StopDeviceDebugStreamRequest
 from edgeimpulse_api.models.store_segment_length_request import StoreSegmentLengthRequest
 from edgeimpulse_api.models.structured_classify_result import StructuredClassifyResult
 from edgeimpulse_api.models.structured_label import StructuredLabel
 from edgeimpulse_api.models.target_constraints import TargetConstraints
 from edgeimpulse_api.models.target_constraints_device import TargetConstraintsDevice
 from edgeimpulse_api.models.target_memory import TargetMemory
 from edgeimpulse_api.models.target_processor import TargetProcessor
```

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/api/__init__.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/api/__init__.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/api/admin_api.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/api/admin_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/api/auth_api.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/api/auth_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/api/cdn_api.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/api/cdn_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/api/classify_api.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/api/classify_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/api/deployment_api.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/api/deployment_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/api/devices_api.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/api/themes_api.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,45 +15,41 @@
 import re  # noqa: F401
 
 from pydantic import validate_arguments, ValidationError
 from typing_extensions import Annotated
 
 from pydantic import Field, StrictInt, StrictStr
 
-from edgeimpulse_api.models.create_device_request import CreateDeviceRequest
 from edgeimpulse_api.models.generic_api_response import GenericApiResponse
-from edgeimpulse_api.models.get_device_response import GetDeviceResponse
-from edgeimpulse_api.models.list_devices_response import ListDevicesResponse
-from edgeimpulse_api.models.rename_device_request import RenameDeviceRequest
-from edgeimpulse_api.models.start_sampling_request import StartSamplingRequest
-from edgeimpulse_api.models.start_sampling_response import StartSamplingResponse
+from edgeimpulse_api.models.get_theme_response import GetThemeResponse
+from edgeimpulse_api.models.get_themes_response import GetThemesResponse
+from edgeimpulse_api.models.update_theme_colors_request import UpdateThemeColorsRequest
+from edgeimpulse_api.models.update_theme_logos_request import UpdateThemeLogosRequest
 
 from edgeimpulse_api.api_client import ApiClient
 from edgeimpulse_api.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
 )
 
 
-class DevicesApi(object):
+class ThemesApi(object):
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient.get_default()
         self.api_client = api_client
 
     @validate_arguments
-    def create_device(self, project_id : Annotated[StrictInt, Field(..., description="Project ID")], create_device_request : CreateDeviceRequest, **kwargs) -> GenericApiResponse:  # noqa: E501
-        """Create device
+    def delete_theme(self, theme_id : Annotated[StrictInt, Field(..., description="Theme ID")], **kwargs) -> GenericApiResponse:  # noqa: E501
+        """Delete theme by ID
 
-        Create a new device. If you set `ifNotExists` to `false` and the device already exists, the `deviceType` will be overwritten.
+        Delete a theme given its unique identifier.
 
-        :param project_id: Project ID (required)
-        :type project_id: int
-        :param create_device_request: (required)
-        :type create_device_request: CreateDeviceRequest
+        :param theme_id: Theme ID (required)
+        :type theme_id: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
@@ -62,26 +58,24 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: GenericApiResponse
         """
         kwargs['_return_http_data_only'] = True
-        return self._create_device_with_http_info(project_id, create_device_request, **kwargs)  # noqa: E501
+        return self._delete_theme_with_http_info(theme_id, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def _create_device_with_http_info(self, project_id : Annotated[StrictInt, Field(..., description="Project ID")], create_device_request : CreateDeviceRequest, **kwargs):  # noqa: E501
-        """Create device 
+    def _delete_theme_with_http_info(self, theme_id : Annotated[StrictInt, Field(..., description="Theme ID")], **kwargs):  # noqa: E501
+        """Delete theme by ID 
 
-        Create a new device. If you set `ifNotExists` to `false` and the device already exists, the `deviceType` will be overwritten.
+        Delete a theme given its unique identifier.
 
-        :param project_id: Project ID (required)
-        :type project_id: int
-        :param create_device_request: (required)
-        :type create_device_request: CreateDeviceRequest
+        :param theme_id: Theme ID (required)
+        :type theme_id: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -101,16 +95,15 @@
                  returns the request thread.
         :rtype: tuple(GenericApiResponse, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
-            'project_id',
-            'create_device_request'
+            'theme_id'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -121,61 +114,52 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method create_device" % _key
+                    " to method delete_theme" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
-        if _params['project_id']:
-            _path_params['projectId'] = _params['project_id']
+        if _params['theme_id']:
+            _path_params['themeId'] = _params['theme_id']
 
         # process the query parameters
         _query_params = []
 
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
 
         # process the form parameters
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
-        if _params['create_device_request']:
-            _body_params = _params['create_device_request']
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
-        # set the HTTP header `Content-Type`
-        _content_types_list = _params.get('_content_type',
-            self.api_client.select_header_content_type(
-                ['application/json']))
-        if _content_types_list:
-                _header_params['Content-Type'] = _content_types_list
-
         # authentication setting
         _auth_settings = ['ApiKeyAuthentication', 'JWTAuthentication', 'JWTHttpHeaderAuthentication']  # noqa: E501
 
         _response_types_map = {
             '200': "GenericApiResponse",
         }
 
         return self.api_client.call_api(
-            '/api/{projectId}/devices/create', 'POST',
+            '/api/themes/{themeId}', 'DELETE',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -184,51 +168,47 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def delete_device(self, project_id : Annotated[StrictInt, Field(..., description="Project ID")], device_id : Annotated[StrictStr, Field(..., description="Device ID")], **kwargs) -> GenericApiResponse:  # noqa: E501
-        """Delete device
+    def get_theme(self, theme_id : Annotated[StrictInt, Field(..., description="Theme ID")], **kwargs) -> GetThemeResponse:  # noqa: E501
+        """Get theme by ID
 
-        Delete a device. When this device sends a new message to ingestion or connects to remote management the device will be recreated.
+        Get a theme given its unique identifier.
 
-        :param project_id: Project ID (required)
-        :type project_id: int
-        :param device_id: Device ID (required)
-        :type device_id: str
+        :param theme_id: Theme ID (required)
+        :type theme_id: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: GenericApiResponse
+        :rtype: GetThemeResponse
         """
         kwargs['_return_http_data_only'] = True
-        return self._delete_device_with_http_info(project_id, device_id, **kwargs)  # noqa: E501
+        return self._get_theme_with_http_info(theme_id, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def _delete_device_with_http_info(self, project_id : Annotated[StrictInt, Field(..., description="Project ID")], device_id : Annotated[StrictStr, Field(..., description="Device ID")], **kwargs):  # noqa: E501
-        """Delete device 
+    def _get_theme_with_http_info(self, theme_id : Annotated[StrictInt, Field(..., description="Theme ID")], **kwargs):  # noqa: E501
+        """Get theme by ID 
 
-        Delete a device. When this device sends a new message to ingestion or connects to remote management the device will be recreated.
+        Get a theme given its unique identifier.
 
-        :param project_id: Project ID (required)
-        :type project_id: int
-        :param device_id: Device ID (required)
-        :type device_id: str
+        :param theme_id: Theme ID (required)
+        :type theme_id: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -242,22 +222,21 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(GenericApiResponse, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(GetThemeResponse, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
-            'project_id',
-            'device_id'
+            'theme_id'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -268,27 +247,25 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method delete_device" % _key
+                    " to method get_theme" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
-        if _params['project_id']:
-            _path_params['projectId'] = _params['project_id']
-        if _params['device_id']:
-            _path_params['deviceId'] = _params['device_id']
+        if _params['theme_id']:
+            _path_params['themeId'] = _params['theme_id']
 
         # process the query parameters
         _query_params = []
 
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
 
@@ -303,19 +280,19 @@
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['ApiKeyAuthentication', 'JWTAuthentication', 'JWTHttpHeaderAuthentication']  # noqa: E501
 
         _response_types_map = {
-            '200': "GenericApiResponse",
+            '200': "GetThemeResponse",
         }
 
         return self.api_client.call_api(
-            '/api/{projectId}/device/{deviceId}', 'DELETE',
+            '/api/themes/{themeId}', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -324,51 +301,43 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def get_device(self, project_id : Annotated[StrictInt, Field(..., description="Project ID")], device_id : Annotated[StrictStr, Field(..., description="Device ID")], **kwargs) -> GetDeviceResponse:  # noqa: E501
-        """Get device
+    def get_themes(self, **kwargs) -> GetThemesResponse:  # noqa: E501
+        """Get themes
 
-        Retrieves a single device
+        Get all available Studio themes.
 
-        :param project_id: Project ID (required)
-        :type project_id: int
-        :param device_id: Device ID (required)
-        :type device_id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: GetDeviceResponse
+        :rtype: GetThemesResponse
         """
         kwargs['_return_http_data_only'] = True
-        return self._get_device_with_http_info(project_id, device_id, **kwargs)  # noqa: E501
+        return self._get_themes_with_http_info(**kwargs)  # noqa: E501
 
     @validate_arguments
-    def _get_device_with_http_info(self, project_id : Annotated[StrictInt, Field(..., description="Project ID")], device_id : Annotated[StrictStr, Field(..., description="Device ID")], **kwargs):  # noqa: E501
-        """Get device 
+    def _get_themes_with_http_info(self, **kwargs):  # noqa: E501
+        """Get themes 
 
-        Retrieves a single device
+        Get all available Studio themes.
 
-        :param project_id: Project ID (required)
-        :type project_id: int
-        :param device_id: Device ID (required)
-        :type device_id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -382,22 +351,20 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(GetDeviceResponse, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(GetThemesResponse, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
-            'project_id',
-            'device_id'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -408,27 +375,23 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method get_device" % _key
+                    " to method get_themes" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
-        if _params['project_id']:
-            _path_params['projectId'] = _params['project_id']
-        if _params['device_id']:
-            _path_params['deviceId'] = _params['device_id']
 
         # process the query parameters
         _query_params = []
 
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
 
@@ -443,19 +406,19 @@
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['ApiKeyAuthentication', 'JWTAuthentication', 'JWTHttpHeaderAuthentication']  # noqa: E501
 
         _response_types_map = {
-            '200': "GetDeviceResponse",
+            '200': "GetThemesResponse",
         }
 
         return self.api_client.call_api(
-            '/api/{projectId}/device/{deviceId}', 'GET',
+            '/api/themes', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -464,47 +427,51 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def list_devices(self, project_id : Annotated[StrictInt, Field(..., description="Project ID")], **kwargs) -> ListDevicesResponse:  # noqa: E501
-        """Lists devices
+    def update_theme_colors(self, theme_id : Annotated[StrictInt, Field(..., description="Theme ID")], update_theme_colors_request : UpdateThemeColorsRequest, **kwargs) -> GenericApiResponse:  # noqa: E501
+        """Update theme colors
 
-        List all devices for this project. Devices get included here if they connect to the remote management API or if they have sent data to the ingestion API and had the `device_id` field set.
+        Update some or all theme colors.
 
-        :param project_id: Project ID (required)
-        :type project_id: int
+        :param theme_id: Theme ID (required)
+        :type theme_id: int
+        :param update_theme_colors_request: (required)
+        :type update_theme_colors_request: UpdateThemeColorsRequest
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: ListDevicesResponse
+        :rtype: GenericApiResponse
         """
         kwargs['_return_http_data_only'] = True
-        return self._list_devices_with_http_info(project_id, **kwargs)  # noqa: E501
+        return self._update_theme_colors_with_http_info(theme_id, update_theme_colors_request, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def _list_devices_with_http_info(self, project_id : Annotated[StrictInt, Field(..., description="Project ID")], **kwargs):  # noqa: E501
-        """Lists devices 
+    def _update_theme_colors_with_http_info(self, theme_id : Annotated[StrictInt, Field(..., description="Theme ID")], update_theme_colors_request : UpdateThemeColorsRequest, **kwargs):  # noqa: E501
+        """Update theme colors 
 
-        List all devices for this project. Devices get included here if they connect to the remote management API or if they have sent data to the ingestion API and had the `device_id` field set.
+        Update some or all theme colors.
 
-        :param project_id: Project ID (required)
-        :type project_id: int
+        :param theme_id: Theme ID (required)
+        :type theme_id: int
+        :param update_theme_colors_request: (required)
+        :type update_theme_colors_request: UpdateThemeColorsRequest
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -518,21 +485,22 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(ListDevicesResponse, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(GenericApiResponse, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
-            'project_id'
+            'theme_id',
+            'update_theme_colors_request'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -543,52 +511,61 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method list_devices" % _key
+                    " to method update_theme_colors" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
-        if _params['project_id']:
-            _path_params['projectId'] = _params['project_id']
+        if _params['theme_id']:
+            _path_params['themeId'] = _params['theme_id']
 
         # process the query parameters
         _query_params = []
 
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
 
         # process the form parameters
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
+        if _params['update_theme_colors_request']:
+            _body_params = _params['update_theme_colors_request']
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
+        # set the HTTP header `Content-Type`
+        _content_types_list = _params.get('_content_type',
+            self.api_client.select_header_content_type(
+                ['application/json']))
+        if _content_types_list:
+                _header_params['Content-Type'] = _content_types_list
+
         # authentication setting
         _auth_settings = ['ApiKeyAuthentication', 'JWTAuthentication', 'JWTHttpHeaderAuthentication']  # noqa: E501
 
         _response_types_map = {
-            '200': "ListDevicesResponse",
+            '200': "GenericApiResponse",
         }
 
         return self.api_client.call_api(
-            '/api/{projectId}/devices', 'GET',
+            '/api/themes/{themeId}/colors', 'POST',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -597,25 +574,23 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def rename_device(self, project_id : Annotated[StrictInt, Field(..., description="Project ID")], device_id : Annotated[StrictStr, Field(..., description="Device ID")], rename_device_request : RenameDeviceRequest, **kwargs) -> GenericApiResponse:  # noqa: E501
-        """Rename
+    def update_theme_favicon(self, theme_id : Annotated[StrictInt, Field(..., description="Theme ID")], image : StrictStr, **kwargs) -> GenericApiResponse:  # noqa: E501
+        """Update theme favicon
 
-        Set the current name for a device.
+        Update the theme favicon
 
-        :param project_id: Project ID (required)
-        :type project_id: int
-        :param device_id: Device ID (required)
-        :type device_id: str
-        :param rename_device_request: (required)
-        :type rename_device_request: RenameDeviceRequest
+        :param theme_id: Theme ID (required)
+        :type theme_id: int
+        :param image: (required)
+        :type image: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
@@ -624,28 +599,26 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: GenericApiResponse
         """
         kwargs['_return_http_data_only'] = True
-        return self._rename_device_with_http_info(project_id, device_id, rename_device_request, **kwargs)  # noqa: E501
+        return self._update_theme_favicon_with_http_info(theme_id, image, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def _rename_device_with_http_info(self, project_id : Annotated[StrictInt, Field(..., description="Project ID")], device_id : Annotated[StrictStr, Field(..., description="Device ID")], rename_device_request : RenameDeviceRequest, **kwargs):  # noqa: E501
-        """Rename 
+    def _update_theme_favicon_with_http_info(self, theme_id : Annotated[StrictInt, Field(..., description="Theme ID")], image : StrictStr, **kwargs):  # noqa: E501
+        """Update theme favicon 
 
-        Set the current name for a device.
+        Update the theme favicon
 
-        :param project_id: Project ID (required)
-        :type project_id: int
-        :param device_id: Device ID (required)
-        :type device_id: str
-        :param rename_device_request: (required)
-        :type rename_device_request: RenameDeviceRequest
+        :param theme_id: Theme ID (required)
+        :type theme_id: int
+        :param image: (required)
+        :type image: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -665,17 +638,16 @@
                  returns the request thread.
         :rtype: tuple(GenericApiResponse, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
-            'project_id',
-            'device_id',
-            'rename_device_request'
+            'theme_id',
+            'image'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -686,63 +658,61 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method rename_device" % _key
+                    " to method update_theme_favicon" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
-        if _params['project_id']:
-            _path_params['projectId'] = _params['project_id']
-        if _params['device_id']:
-            _path_params['deviceId'] = _params['device_id']
+        if _params['theme_id']:
+            _path_params['themeId'] = _params['theme_id']
 
         # process the query parameters
         _query_params = []
 
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
 
         # process the form parameters
         _form_params = []
         _files = {}
+        if _params['image']:
+            _files['image'] = _params['image']
 
         # process the body parameter
         _body_params = None
-        if _params['rename_device_request']:
-            _body_params = _params['rename_device_request']
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # set the HTTP header `Content-Type`
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
-                ['application/json']))
+                ['multipart/form-data']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
         _auth_settings = ['ApiKeyAuthentication', 'JWTAuthentication', 'JWTHttpHeaderAuthentication']  # noqa: E501
 
         _response_types_map = {
             '200': "GenericApiResponse",
         }
 
         return self.api_client.call_api(
-            '/api/{projectId}/devices/{deviceId}/rename', 'POST',
+            '/api/themes/{themeId}/favicon', 'POST',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -751,55 +721,51 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def start_sampling(self, project_id : Annotated[StrictInt, Field(..., description="Project ID")], device_id : Annotated[StrictStr, Field(..., description="Device ID")], start_sampling_request : StartSamplingRequest, **kwargs) -> StartSamplingResponse:  # noqa: E501
-        """Start sampling
+    def update_theme_logos(self, theme_id : Annotated[StrictInt, Field(..., description="Theme ID")], update_theme_logos_request : UpdateThemeLogosRequest, **kwargs) -> GenericApiResponse:  # noqa: E501
+        """Update theme logos
 
-        Start sampling on a device. This function returns immediately. Updates are streamed through the websocket API.
+        Update some or all theme logos.
 
-        :param project_id: Project ID (required)
-        :type project_id: int
-        :param device_id: Device ID (required)
-        :type device_id: str
-        :param start_sampling_request: (required)
-        :type start_sampling_request: StartSamplingRequest
+        :param theme_id: Theme ID (required)
+        :type theme_id: int
+        :param update_theme_logos_request: (required)
+        :type update_theme_logos_request: UpdateThemeLogosRequest
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: StartSamplingResponse
+        :rtype: GenericApiResponse
         """
         kwargs['_return_http_data_only'] = True
-        return self._start_sampling_with_http_info(project_id, device_id, start_sampling_request, **kwargs)  # noqa: E501
+        return self._update_theme_logos_with_http_info(theme_id, update_theme_logos_request, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def _start_sampling_with_http_info(self, project_id : Annotated[StrictInt, Field(..., description="Project ID")], device_id : Annotated[StrictStr, Field(..., description="Device ID")], start_sampling_request : StartSamplingRequest, **kwargs):  # noqa: E501
-        """Start sampling 
+    def _update_theme_logos_with_http_info(self, theme_id : Annotated[StrictInt, Field(..., description="Theme ID")], update_theme_logos_request : UpdateThemeLogosRequest, **kwargs):  # noqa: E501
+        """Update theme logos 
 
-        Start sampling on a device. This function returns immediately. Updates are streamed through the websocket API.
+        Update some or all theme logos.
 
-        :param project_id: Project ID (required)
-        :type project_id: int
-        :param device_id: Device ID (required)
-        :type device_id: str
-        :param start_sampling_request: (required)
-        :type start_sampling_request: StartSamplingRequest
+        :param theme_id: Theme ID (required)
+        :type theme_id: int
+        :param update_theme_logos_request: (required)
+        :type update_theme_logos_request: UpdateThemeLogosRequest
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -813,23 +779,22 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(StartSamplingResponse, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(GenericApiResponse, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
-            'project_id',
-            'device_id',
-            'start_sampling_request'
+            'theme_id',
+            'update_theme_logos_request'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -840,42 +805,40 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method start_sampling" % _key
+                    " to method update_theme_logos" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
-        if _params['project_id']:
-            _path_params['projectId'] = _params['project_id']
-        if _params['device_id']:
-            _path_params['deviceId'] = _params['device_id']
+        if _params['theme_id']:
+            _path_params['themeId'] = _params['theme_id']
 
         # process the query parameters
         _query_params = []
 
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
 
         # process the form parameters
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
-        if _params['start_sampling_request']:
-            _body_params = _params['start_sampling_request']
+        if _params['update_theme_logos_request']:
+            _body_params = _params['update_theme_logos_request']
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # set the HTTP header `Content-Type`
         _content_types_list = _params.get('_content_type',
@@ -884,19 +847,19 @@
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
         _auth_settings = ['ApiKeyAuthentication', 'JWTAuthentication', 'JWTHttpHeaderAuthentication']  # noqa: E501
 
         _response_types_map = {
-            '200': "StartSamplingResponse",
+            '200': "GenericApiResponse",
         }
 
         return self.api_client.call_api(
-            '/api/{projectId}/device/{deviceId}/start-sampling', 'POST',
+            '/api/themes/{themeId}/logos', 'POST',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
```

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/api/dsp_api.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/api/dsp_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/api/email_verification_api.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/api/email_verification_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/api/export_api.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/api/export_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/api/feature_flags_api.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/api/feature_flags_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/api/health_api.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/api/health_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/api/impulse_api.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/api/impulse_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/api/jobs_api.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/api/jobs_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/api/learn_api.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/api/learn_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/api/login_api.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/api/login_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/api/metrics_api.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/api/metrics_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/api/optimization_api.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/api/optimization_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/api/organization_blocks_api.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/api/organization_blocks_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/api/organization_create_project_api.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/api/organization_create_project_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/api/organization_data_api.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/api/organization_data_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/api/organization_data_campaigns_api.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/api/organization_data_campaigns_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/api/organization_jobs_api.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/api/organization_jobs_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/api/organization_pipelines_api.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/api/organization_pipelines_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/api/organization_portals_api.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/api/organization_portals_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/api/organizations_api.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/api/organizations_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/api/performance_calibration_api.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/api/performance_calibration_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/api/projects_api.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/api/projects_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/api/raw_data_api.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/api/raw_data_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/api/themes_api.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/api/whitelabels_api.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,43 +13,186 @@
 from __future__ import absolute_import
 
 import re  # noqa: F401
 
 from pydantic import validate_arguments, ValidationError
 from typing_extensions import Annotated
 
-from pydantic import Field, StrictInt, StrictStr
+from pydantic import Field, StrictInt
 
+from edgeimpulse_api.models.create_whitelabel_request import CreateWhitelabelRequest
+from edgeimpulse_api.models.create_whitelabel_response import CreateWhitelabelResponse
 from edgeimpulse_api.models.generic_api_response import GenericApiResponse
-from edgeimpulse_api.models.get_theme_response import GetThemeResponse
-from edgeimpulse_api.models.get_themes_response import GetThemesResponse
-from edgeimpulse_api.models.update_theme_colors_request import UpdateThemeColorsRequest
-from edgeimpulse_api.models.update_theme_logos_request import UpdateThemeLogosRequest
+from edgeimpulse_api.models.get_all_whitelabels_response import GetAllWhitelabelsResponse
+from edgeimpulse_api.models.get_impulse_blocks_response import GetImpulseBlocksResponse
+from edgeimpulse_api.models.get_whitelabel_domain_response import GetWhitelabelDomainResponse
+from edgeimpulse_api.models.get_whitelabel_response import GetWhitelabelResponse
+from edgeimpulse_api.models.update_whitelabel_deployment_targets_request import UpdateWhitelabelDeploymentTargetsRequest
 
 from edgeimpulse_api.api_client import ApiClient
 from edgeimpulse_api.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
 )
 
 
-class ThemesApi(object):
+class WhitelabelsApi(object):
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient.get_default()
         self.api_client = api_client
 
     @validate_arguments
-    def delete_theme(self, theme_id : Annotated[StrictInt, Field(..., description="Theme ID")], **kwargs) -> GenericApiResponse:  # noqa: E501
-        """Delete theme by ID
+    def create_whitelabel(self, create_whitelabel_request : CreateWhitelabelRequest, **kwargs) -> CreateWhitelabelResponse:  # noqa: E501
+        """Create a new white label
 
-        Delete a theme given its unique identifier.
+        Create a new white label
 
-        :param theme_id: Theme ID (required)
-        :type theme_id: int
+        :param create_whitelabel_request: (required)
+        :type create_whitelabel_request: CreateWhitelabelRequest
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: CreateWhitelabelResponse
+        """
+        kwargs['_return_http_data_only'] = True
+        return self._create_whitelabel_with_http_info(create_whitelabel_request, **kwargs)  # noqa: E501
+
+    @validate_arguments
+    def _create_whitelabel_with_http_info(self, create_whitelabel_request : CreateWhitelabelRequest, **kwargs):  # noqa: E501
+        """Create a new white label 
+
+        Create a new white label
+
+        :param create_whitelabel_request: (required)
+        :type create_whitelabel_request: CreateWhitelabelRequest
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _return_http_data_only: response data without head status code
+                                       and headers
+        :type _return_http_data_only: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the authentication
+                              in the spec for a single request.
+        :type _request_auth: dict, optional
+        :type _content_type: string, optional: force content-type for the request
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: tuple(CreateWhitelabelResponse, status_code(int), headers(HTTPHeaderDict))
+        """
+
+        _params = locals()
+
+        _all_params = [
+            'create_whitelabel_request'
+        ]
+        _all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout',
+                '_request_auth',
+                '_content_type',
+                '_headers'
+            ]
+        )
+
+        # validate the arguments
+        for _key, _val in _params['kwargs'].items():
+            if _key not in _all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method create_whitelabel" % _key
+                )
+            _params[_key] = _val
+        del _params['kwargs']
+
+        _collection_formats = {}
+
+        # process the path parameters
+        _path_params = {}
+
+        # process the query parameters
+        _query_params = []
+
+        # process the header parameters
+        _header_params = dict(_params.get('_headers', {}))
+
+        # process the form parameters
+        _form_params = []
+        _files = {}
+
+        # process the body parameter
+        _body_params = None
+        if _params['create_whitelabel_request']:
+            _body_params = _params['create_whitelabel_request']
+
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # set the HTTP header `Content-Type`
+        _content_types_list = _params.get('_content_type',
+            self.api_client.select_header_content_type(
+                ['application/json']))
+        if _content_types_list:
+                _header_params['Content-Type'] = _content_types_list
+
+        # authentication setting
+        _auth_settings = ['ApiKeyAuthentication', 'JWTAuthentication', 'JWTHttpHeaderAuthentication']  # noqa: E501
+
+        _response_types_map = {
+            '200': "CreateWhitelabelResponse",
+        }
+
+        return self.api_client.call_api(
+            '/api/whitelabels', 'POST',
+            _path_params,
+            _query_params,
+            _header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            response_types_map=_response_types_map,
+            auth_settings=_auth_settings,
+            async_req=_params.get('async_req'),
+            _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=_params.get('_preload_content', True),
+            _request_timeout=_params.get('_request_timeout'),
+            collection_formats=_collection_formats,
+            _request_auth=_params.get('_request_auth'))
+
+    @validate_arguments
+    def delete_whitelabel(self, whitelabel_identifier : Annotated[StrictInt, Field(..., description="Whitelabel ID")], **kwargs) -> GenericApiResponse:  # noqa: E501
+        """Deletes a white label
+
+        Deletes the white label with the given id.
+
+        :param whitelabel_identifier: Whitelabel ID (required)
+        :type whitelabel_identifier: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
@@ -58,24 +201,24 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: GenericApiResponse
         """
         kwargs['_return_http_data_only'] = True
-        return self._delete_theme_with_http_info(theme_id, **kwargs)  # noqa: E501
+        return self._delete_whitelabel_with_http_info(whitelabel_identifier, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def _delete_theme_with_http_info(self, theme_id : Annotated[StrictInt, Field(..., description="Theme ID")], **kwargs):  # noqa: E501
-        """Delete theme by ID 
+    def _delete_whitelabel_with_http_info(self, whitelabel_identifier : Annotated[StrictInt, Field(..., description="Whitelabel ID")], **kwargs):  # noqa: E501
+        """Deletes a white label 
 
-        Delete a theme given its unique identifier.
+        Deletes the white label with the given id.
 
-        :param theme_id: Theme ID (required)
-        :type theme_id: int
+        :param whitelabel_identifier: Whitelabel ID (required)
+        :type whitelabel_identifier: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -95,15 +238,15 @@
                  returns the request thread.
         :rtype: tuple(GenericApiResponse, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
-            'theme_id'
+            'whitelabel_identifier'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -114,25 +257,25 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method delete_theme" % _key
+                    " to method delete_whitelabel" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
-        if _params['theme_id']:
-            _path_params['themeId'] = _params['theme_id']
+        if _params['whitelabel_identifier']:
+            _path_params['whitelabelIdentifier'] = _params['whitelabel_identifier']
 
         # process the query parameters
         _query_params = []
 
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
 
@@ -151,15 +294,15 @@
         _auth_settings = ['ApiKeyAuthentication', 'JWTAuthentication', 'JWTHttpHeaderAuthentication']  # noqa: E501
 
         _response_types_map = {
             '200': "GenericApiResponse",
         }
 
         return self.api_client.call_api(
-            '/api/themes/{themeId}', 'DELETE',
+            '/api/whitelabel/{whitelabelIdentifier}', 'DELETE',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -168,47 +311,47 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def get_theme(self, theme_id : Annotated[StrictInt, Field(..., description="Theme ID")], **kwargs) -> GetThemeResponse:  # noqa: E501
-        """Get theme by ID
+    def get_all_impulse_blocks(self, whitelabel_identifier : Annotated[StrictInt, Field(..., description="Whitelabel ID")], **kwargs) -> GetImpulseBlocksResponse:  # noqa: E501
+        """Get impulse blocks
 
-        Get a theme given its unique identifier.
+        Lists all possible DSP and ML blocks available for this white label.
 
-        :param theme_id: Theme ID (required)
-        :type theme_id: int
+        :param whitelabel_identifier: Whitelabel ID (required)
+        :type whitelabel_identifier: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: GetThemeResponse
+        :rtype: GetImpulseBlocksResponse
         """
         kwargs['_return_http_data_only'] = True
-        return self._get_theme_with_http_info(theme_id, **kwargs)  # noqa: E501
+        return self._get_all_impulse_blocks_with_http_info(whitelabel_identifier, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def _get_theme_with_http_info(self, theme_id : Annotated[StrictInt, Field(..., description="Theme ID")], **kwargs):  # noqa: E501
-        """Get theme by ID 
+    def _get_all_impulse_blocks_with_http_info(self, whitelabel_identifier : Annotated[StrictInt, Field(..., description="Whitelabel ID")], **kwargs):  # noqa: E501
+        """Get impulse blocks 
 
-        Get a theme given its unique identifier.
+        Lists all possible DSP and ML blocks available for this white label.
 
-        :param theme_id: Theme ID (required)
-        :type theme_id: int
+        :param whitelabel_identifier: Whitelabel ID (required)
+        :type whitelabel_identifier: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -222,21 +365,21 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(GetThemeResponse, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(GetImpulseBlocksResponse, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
-            'theme_id'
+            'whitelabel_identifier'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -247,25 +390,25 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method get_theme" % _key
+                    " to method get_all_impulse_blocks" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
-        if _params['theme_id']:
-            _path_params['themeId'] = _params['theme_id']
+        if _params['whitelabel_identifier']:
+            _path_params['whitelabelIdentifier'] = _params['whitelabel_identifier']
 
         # process the query parameters
         _query_params = []
 
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
 
@@ -280,19 +423,19 @@
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['ApiKeyAuthentication', 'JWTAuthentication', 'JWTHttpHeaderAuthentication']  # noqa: E501
 
         _response_types_map = {
-            '200': "GetThemeResponse",
+            '200': "GetImpulseBlocksResponse",
         }
 
         return self.api_client.call_api(
-            '/api/themes/{themeId}', 'GET',
+            '/api/whitelabel/{whitelabelIdentifier}/impulse/blocks', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -301,42 +444,42 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def get_themes(self, **kwargs) -> GetThemesResponse:  # noqa: E501
-        """Get themes
+    def get_all_whitelabels(self, **kwargs) -> GetAllWhitelabelsResponse:  # noqa: E501
+        """List the registered white labels
 
-        Get all available Studio themes.
+        Retrieve the list of registered white labels.
 
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: GetThemesResponse
+        :rtype: GetAllWhitelabelsResponse
         """
         kwargs['_return_http_data_only'] = True
-        return self._get_themes_with_http_info(**kwargs)  # noqa: E501
+        return self._get_all_whitelabels_with_http_info(**kwargs)  # noqa: E501
 
     @validate_arguments
-    def _get_themes_with_http_info(self, **kwargs):  # noqa: E501
-        """Get themes 
+    def _get_all_whitelabels_with_http_info(self, **kwargs):  # noqa: E501
+        """List the registered white labels 
 
-        Get all available Studio themes.
+        Retrieve the list of registered white labels.
 
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
@@ -351,15 +494,15 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(GetThemesResponse, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(GetAllWhitelabelsResponse, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
         ]
         _all_params.extend(
@@ -375,15 +518,15 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method get_themes" % _key
+                    " to method get_all_whitelabels" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
@@ -406,19 +549,19 @@
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['ApiKeyAuthentication', 'JWTAuthentication', 'JWTHttpHeaderAuthentication']  # noqa: E501
 
         _response_types_map = {
-            '200': "GetThemesResponse",
+            '200': "GetAllWhitelabelsResponse",
         }
 
         return self.api_client.call_api(
-            '/api/themes', 'GET',
+            '/api/whitelabels', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -427,51 +570,47 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def update_theme_colors(self, theme_id : Annotated[StrictInt, Field(..., description="Theme ID")], update_theme_colors_request : UpdateThemeColorsRequest, **kwargs) -> GenericApiResponse:  # noqa: E501
-        """Update theme colors
+    def get_whitelabel(self, whitelabel_identifier : Annotated[StrictInt, Field(..., description="Whitelabel ID")], **kwargs) -> GetWhitelabelResponse:  # noqa: E501
+        """White label information
 
-        Update some or all theme colors.
+        Retrieve all the information about this white label.
 
-        :param theme_id: Theme ID (required)
-        :type theme_id: int
-        :param update_theme_colors_request: (required)
-        :type update_theme_colors_request: UpdateThemeColorsRequest
+        :param whitelabel_identifier: Whitelabel ID (required)
+        :type whitelabel_identifier: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: GenericApiResponse
+        :rtype: GetWhitelabelResponse
         """
         kwargs['_return_http_data_only'] = True
-        return self._update_theme_colors_with_http_info(theme_id, update_theme_colors_request, **kwargs)  # noqa: E501
+        return self._get_whitelabel_with_http_info(whitelabel_identifier, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def _update_theme_colors_with_http_info(self, theme_id : Annotated[StrictInt, Field(..., description="Theme ID")], update_theme_colors_request : UpdateThemeColorsRequest, **kwargs):  # noqa: E501
-        """Update theme colors 
+    def _get_whitelabel_with_http_info(self, whitelabel_identifier : Annotated[StrictInt, Field(..., description="Whitelabel ID")], **kwargs):  # noqa: E501
+        """White label information 
 
-        Update some or all theme colors.
+        Retrieve all the information about this white label.
 
-        :param theme_id: Theme ID (required)
-        :type theme_id: int
-        :param update_theme_colors_request: (required)
-        :type update_theme_colors_request: UpdateThemeColorsRequest
+        :param whitelabel_identifier: Whitelabel ID (required)
+        :type whitelabel_identifier: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -485,22 +624,21 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(GenericApiResponse, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(GetWhitelabelResponse, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
-            'theme_id',
-            'update_theme_colors_request'
+            'whitelabel_identifier'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -511,61 +649,52 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method update_theme_colors" % _key
+                    " to method get_whitelabel" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
-        if _params['theme_id']:
-            _path_params['themeId'] = _params['theme_id']
+        if _params['whitelabel_identifier']:
+            _path_params['whitelabelIdentifier'] = _params['whitelabel_identifier']
 
         # process the query parameters
         _query_params = []
 
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
 
         # process the form parameters
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
-        if _params['update_theme_colors_request']:
-            _body_params = _params['update_theme_colors_request']
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
-        # set the HTTP header `Content-Type`
-        _content_types_list = _params.get('_content_type',
-            self.api_client.select_header_content_type(
-                ['application/json']))
-        if _content_types_list:
-                _header_params['Content-Type'] = _content_types_list
-
         # authentication setting
         _auth_settings = ['ApiKeyAuthentication', 'JWTAuthentication', 'JWTHttpHeaderAuthentication']  # noqa: E501
 
         _response_types_map = {
-            '200': "GenericApiResponse",
+            '200': "GetWhitelabelResponse",
         }
 
         return self.api_client.call_api(
-            '/api/themes/{themeId}/colors', 'POST',
+            '/api/whitelabel/{whitelabelIdentifier}', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -574,51 +703,47 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def update_theme_favicon(self, theme_id : Annotated[StrictInt, Field(..., description="Theme ID")], image : StrictStr, **kwargs) -> GenericApiResponse:  # noqa: E501
-        """Update theme favicon
+    def get_whitelabel_domain(self, whitelabel_identifier : Annotated[StrictInt, Field(..., description="Whitelabel ID")], **kwargs) -> GetWhitelabelDomainResponse:  # noqa: E501
+        """Get white label domain
 
-        Update the theme favicon
+        Get a white label domain given its unique identifier.
 
-        :param theme_id: Theme ID (required)
-        :type theme_id: int
-        :param image: (required)
-        :type image: str
+        :param whitelabel_identifier: Whitelabel ID (required)
+        :type whitelabel_identifier: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: GenericApiResponse
+        :rtype: GetWhitelabelDomainResponse
         """
         kwargs['_return_http_data_only'] = True
-        return self._update_theme_favicon_with_http_info(theme_id, image, **kwargs)  # noqa: E501
+        return self._get_whitelabel_domain_with_http_info(whitelabel_identifier, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def _update_theme_favicon_with_http_info(self, theme_id : Annotated[StrictInt, Field(..., description="Theme ID")], image : StrictStr, **kwargs):  # noqa: E501
-        """Update theme favicon 
+    def _get_whitelabel_domain_with_http_info(self, whitelabel_identifier : Annotated[StrictInt, Field(..., description="Whitelabel ID")], **kwargs):  # noqa: E501
+        """Get white label domain 
 
-        Update the theme favicon
+        Get a white label domain given its unique identifier.
 
-        :param theme_id: Theme ID (required)
-        :type theme_id: int
-        :param image: (required)
-        :type image: str
+        :param whitelabel_identifier: Whitelabel ID (required)
+        :type whitelabel_identifier: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -632,22 +757,21 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(GenericApiResponse, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(GetWhitelabelDomainResponse, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
-            'theme_id',
-            'image'
+            'whitelabel_identifier'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -658,61 +782,52 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method update_theme_favicon" % _key
+                    " to method get_whitelabel_domain" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
-        if _params['theme_id']:
-            _path_params['themeId'] = _params['theme_id']
+        if _params['whitelabel_identifier']:
+            _path_params['whitelabelIdentifier'] = _params['whitelabel_identifier']
 
         # process the query parameters
         _query_params = []
 
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
 
         # process the form parameters
         _form_params = []
         _files = {}
-        if _params['image']:
-            _files['image'] = _params['image']
 
         # process the body parameter
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
-        # set the HTTP header `Content-Type`
-        _content_types_list = _params.get('_content_type',
-            self.api_client.select_header_content_type(
-                ['multipart/form-data']))
-        if _content_types_list:
-                _header_params['Content-Type'] = _content_types_list
-
         # authentication setting
-        _auth_settings = ['ApiKeyAuthentication', 'JWTAuthentication', 'JWTHttpHeaderAuthentication']  # noqa: E501
+        _auth_settings = []  # noqa: E501
 
         _response_types_map = {
-            '200': "GenericApiResponse",
+            '200': "GetWhitelabelDomainResponse",
         }
 
         return self.api_client.call_api(
-            '/api/themes/{themeId}/favicon', 'POST',
+            '/api/whitelabel/{whitelabelIdentifier}/domain', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -721,23 +836,23 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def update_theme_logos(self, theme_id : Annotated[StrictInt, Field(..., description="Theme ID")], update_theme_logos_request : UpdateThemeLogosRequest, **kwargs) -> GenericApiResponse:  # noqa: E501
-        """Update theme logos
+    def update_deployment_targets(self, whitelabel_identifier : Annotated[StrictInt, Field(..., description="Whitelabel ID")], update_whitelabel_deployment_targets_request : UpdateWhitelabelDeploymentTargetsRequest, **kwargs) -> GenericApiResponse:  # noqa: E501
+        """Update deployment targets
 
-        Update some or all theme logos.
+        Update some or all of the deployment targets enabled for this white label.
 
-        :param theme_id: Theme ID (required)
-        :type theme_id: int
-        :param update_theme_logos_request: (required)
-        :type update_theme_logos_request: UpdateThemeLogosRequest
+        :param whitelabel_identifier: Whitelabel ID (required)
+        :type whitelabel_identifier: int
+        :param update_whitelabel_deployment_targets_request: (required)
+        :type update_whitelabel_deployment_targets_request: UpdateWhitelabelDeploymentTargetsRequest
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
@@ -746,26 +861,26 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: GenericApiResponse
         """
         kwargs['_return_http_data_only'] = True
-        return self._update_theme_logos_with_http_info(theme_id, update_theme_logos_request, **kwargs)  # noqa: E501
+        return self._update_deployment_targets_with_http_info(whitelabel_identifier, update_whitelabel_deployment_targets_request, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def _update_theme_logos_with_http_info(self, theme_id : Annotated[StrictInt, Field(..., description="Theme ID")], update_theme_logos_request : UpdateThemeLogosRequest, **kwargs):  # noqa: E501
-        """Update theme logos 
+    def _update_deployment_targets_with_http_info(self, whitelabel_identifier : Annotated[StrictInt, Field(..., description="Whitelabel ID")], update_whitelabel_deployment_targets_request : UpdateWhitelabelDeploymentTargetsRequest, **kwargs):  # noqa: E501
+        """Update deployment targets 
 
-        Update some or all theme logos.
+        Update some or all of the deployment targets enabled for this white label.
 
-        :param theme_id: Theme ID (required)
-        :type theme_id: int
-        :param update_theme_logos_request: (required)
-        :type update_theme_logos_request: UpdateThemeLogosRequest
+        :param whitelabel_identifier: Whitelabel ID (required)
+        :type whitelabel_identifier: int
+        :param update_whitelabel_deployment_targets_request: (required)
+        :type update_whitelabel_deployment_targets_request: UpdateWhitelabelDeploymentTargetsRequest
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -785,16 +900,16 @@
                  returns the request thread.
         :rtype: tuple(GenericApiResponse, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
-            'theme_id',
-            'update_theme_logos_request'
+            'whitelabel_identifier',
+            'update_whitelabel_deployment_targets_request'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -805,40 +920,40 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method update_theme_logos" % _key
+                    " to method update_deployment_targets" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
-        if _params['theme_id']:
-            _path_params['themeId'] = _params['theme_id']
+        if _params['whitelabel_identifier']:
+            _path_params['whitelabelIdentifier'] = _params['whitelabel_identifier']
 
         # process the query parameters
         _query_params = []
 
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
 
         # process the form parameters
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
-        if _params['update_theme_logos_request']:
-            _body_params = _params['update_theme_logos_request']
+        if _params['update_whitelabel_deployment_targets_request']:
+            _body_params = _params['update_whitelabel_deployment_targets_request']
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # set the HTTP header `Content-Type`
         _content_types_list = _params.get('_content_type',
@@ -851,15 +966,15 @@
         _auth_settings = ['ApiKeyAuthentication', 'JWTAuthentication', 'JWTHttpHeaderAuthentication']  # noqa: E501
 
         _response_types_map = {
             '200': "GenericApiResponse",
         }
 
         return self.api_client.call_api(
-            '/api/themes/{themeId}/logos', 'POST',
+            '/api/whitelabel/{whitelabelIdentifier}/deploymentTargets', 'POST',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
```

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/api/third_party_auth_api.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/api/third_party_auth_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/api/upload_portal_api.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/api/upload_portal_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/api/user_api.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/api/user_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/api_client.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/api_client.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/configuration.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/configuration.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/exceptions.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/__init__.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -200,14 +200,15 @@
 from edgeimpulse_api.models.dsp_info_features import DSPInfoFeatures
 from edgeimpulse_api.models.dsp_info_performance import DSPInfoPerformance
 from edgeimpulse_api.models.dsp_metadata import DSPMetadata
 from edgeimpulse_api.models.dsp_metadata_included_samples_inner import DSPMetadataIncludedSamplesInner
 from edgeimpulse_api.models.dsp_metadata_output_config import DSPMetadataOutputConfig
 from edgeimpulse_api.models.dsp_metadata_output_config_shape import DSPMetadataOutputConfigShape
 from edgeimpulse_api.models.dsp_metadata_response import DSPMetadataResponse
+from edgeimpulse_api.models.dsp_named_axis import DSPNamedAxis
 from edgeimpulse_api.models.data_campaign import DataCampaign
 from edgeimpulse_api.models.data_campaign_dashboard import DataCampaignDashboard
 from edgeimpulse_api.models.data_campaign_graph import DataCampaignGraph
 from edgeimpulse_api.models.data_campaign_graph_x_data_inner import DataCampaignGraphXDataInner
 from edgeimpulse_api.models.data_campaign_graph_x_data_inner_values_inner import DataCampaignGraphXDataInnerValuesInner
 from edgeimpulse_api.models.data_campaign_link import DataCampaignLink
 from edgeimpulse_api.models.data_campaign_query import DataCampaignQuery
@@ -239,14 +240,16 @@
 from edgeimpulse_api.models.development_board_request_update import DevelopmentBoardRequestUpdate
 from edgeimpulse_api.models.development_board_response import DevelopmentBoardResponse
 from edgeimpulse_api.models.development_boards_response import DevelopmentBoardsResponse
 from edgeimpulse_api.models.development_boards_response_all_of import DevelopmentBoardsResponseAllOf
 from edgeimpulse_api.models.development_keys import DevelopmentKeys
 from edgeimpulse_api.models.development_keys_response import DevelopmentKeysResponse
 from edgeimpulse_api.models.device import Device
+from edgeimpulse_api.models.device_debug_stream_type import DeviceDebugStreamType
+from edgeimpulse_api.models.device_inference_info import DeviceInferenceInfo
 from edgeimpulse_api.models.device_name_response import DeviceNameResponse
 from edgeimpulse_api.models.device_name_response_all_of import DeviceNameResponseAllOf
 from edgeimpulse_api.models.device_sensors_inner import DeviceSensorsInner
 from edgeimpulse_api.models.download import Download
 from edgeimpulse_api.models.download_portal_file_request import DownloadPortalFileRequest
 from edgeimpulse_api.models.download_portal_file_response import DownloadPortalFileResponse
 from edgeimpulse_api.models.download_portal_file_response_all_of import DownloadPortalFileResponseAllOf
@@ -336,14 +339,16 @@
 from edgeimpulse_api.models.get_email_verification_status_response import GetEmailVerificationStatusResponse
 from edgeimpulse_api.models.get_email_verification_status_response_all_of import GetEmailVerificationStatusResponseAllOf
 from edgeimpulse_api.models.get_feature_flags_response import GetFeatureFlagsResponse
 from edgeimpulse_api.models.get_feature_flags_response_all_of import GetFeatureFlagsResponseAllOf
 from edgeimpulse_api.models.get_feature_flags_response_all_of_flags import GetFeatureFlagsResponseAllOfFlags
 from edgeimpulse_api.models.get_impulse_blocks_response import GetImpulseBlocksResponse
 from edgeimpulse_api.models.get_impulse_blocks_response_all_of import GetImpulseBlocksResponseAllOf
+from edgeimpulse_api.models.get_impulse_records_request import GetImpulseRecordsRequest
+from edgeimpulse_api.models.get_impulse_records_request_range import GetImpulseRecordsRequestRange
 from edgeimpulse_api.models.get_impulse_response import GetImpulseResponse
 from edgeimpulse_api.models.get_impulse_response_all_of import GetImpulseResponseAllOf
 from edgeimpulse_api.models.get_jwt_request import GetJWTRequest
 from edgeimpulse_api.models.get_jwt_response import GetJWTResponse
 from edgeimpulse_api.models.get_jwt_response_all_of import GetJWTResponseAllOf
 from edgeimpulse_api.models.get_job_response import GetJobResponse
 from edgeimpulse_api.models.get_job_response_all_of import GetJobResponseAllOf
@@ -454,14 +459,15 @@
 from edgeimpulse_api.models.job_state import JobState
 from edgeimpulse_api.models.job_state_execution_details import JobStateExecutionDetails
 from edgeimpulse_api.models.job_status import JobStatus
 from edgeimpulse_api.models.job_step import JobStep
 from edgeimpulse_api.models.job_summary_response import JobSummaryResponse
 from edgeimpulse_api.models.job_summary_response_all_of import JobSummaryResponseAllOf
 from edgeimpulse_api.models.job_summary_response_all_of_summary import JobSummaryResponseAllOfSummary
+from edgeimpulse_api.models.keep_device_debug_stream_alive_request import KeepDeviceDebugStreamAliveRequest
 from edgeimpulse_api.models.keras_custom_metric import KerasCustomMetric
 from edgeimpulse_api.models.keras_model_layer import KerasModelLayer
 from edgeimpulse_api.models.keras_model_layer_input import KerasModelLayerInput
 from edgeimpulse_api.models.keras_model_layer_output import KerasModelLayerOutput
 from edgeimpulse_api.models.keras_model_metadata import KerasModelMetadata
 from edgeimpulse_api.models.keras_model_metadata_all_of import KerasModelMetadataAllOf
 from edgeimpulse_api.models.keras_model_metadata_metrics import KerasModelMetadataMetrics
@@ -778,22 +784,26 @@
 from edgeimpulse_api.models.set_syntiant_posterior_request import SetSyntiantPosteriorRequest
 from edgeimpulse_api.models.set_user_password_request import SetUserPasswordRequest
 from edgeimpulse_api.models.socket_token_response import SocketTokenResponse
 from edgeimpulse_api.models.socket_token_response_all_of import SocketTokenResponseAllOf
 from edgeimpulse_api.models.socket_token_response_all_of_token import SocketTokenResponseAllOfToken
 from edgeimpulse_api.models.split_sample_in_frames_request import SplitSampleInFramesRequest
 from edgeimpulse_api.models.staff_info import StaffInfo
+from edgeimpulse_api.models.start_device_debug_stream_response import StartDeviceDebugStreamResponse
+from edgeimpulse_api.models.start_device_debug_stream_response_all_of import StartDeviceDebugStreamResponseAllOf
+from edgeimpulse_api.models.start_device_snapshot_debug_stream_request import StartDeviceSnapshotDebugStreamRequest
 from edgeimpulse_api.models.start_enterprise_trial_request import StartEnterpriseTrialRequest
 from edgeimpulse_api.models.start_job_response import StartJobResponse
 from edgeimpulse_api.models.start_job_response_all_of import StartJobResponseAllOf
 from edgeimpulse_api.models.start_performance_calibration_request import StartPerformanceCalibrationRequest
 from edgeimpulse_api.models.start_sampling_request import StartSamplingRequest
 from edgeimpulse_api.models.start_sampling_response import StartSamplingResponse
 from edgeimpulse_api.models.start_sampling_response_all_of import StartSamplingResponseAllOf
 from edgeimpulse_api.models.start_training_request_anomaly import StartTrainingRequestAnomaly
+from edgeimpulse_api.models.stop_device_debug_stream_request import StopDeviceDebugStreamRequest
 from edgeimpulse_api.models.store_segment_length_request import StoreSegmentLengthRequest
 from edgeimpulse_api.models.structured_classify_result import StructuredClassifyResult
 from edgeimpulse_api.models.structured_label import StructuredLabel
 from edgeimpulse_api.models.target_constraints import TargetConstraints
 from edgeimpulse_api.models.target_constraints_device import TargetConstraintsDevice
 from edgeimpulse_api.models.target_memory import TargetMemory
 from edgeimpulse_api.models.target_processor import TargetProcessor
```

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/activate_user_by_third_party_activation_code_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/activate_user_by_third_party_activation_code_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/activate_user_or_verify_email_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/activate_user_or_verify_email_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/add_api_key_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/add_api_key_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/add_collaborator_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/add_collaborator_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/add_hmac_key_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/add_hmac_key_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/add_member_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/add_member_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/add_organization_api_key_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/add_organization_api_key_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/add_organization_api_key_request_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/add_organization_api_key_request_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/add_organization_bucket_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/add_organization_bucket_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/add_organization_data_campaign_dashboard_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/add_organization_data_campaign_dashboard_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/add_organization_data_campaign_dashboard_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/add_organization_data_campaign_dashboard_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/add_organization_data_campaign_dashboard_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/add_organization_data_campaign_dashboard_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/add_organization_data_campaign_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/add_organization_data_campaign_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/add_organization_data_campaign_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/add_organization_data_campaign_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/add_organization_data_campaign_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/add_organization_data_campaign_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/add_organization_deploy_block_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/add_organization_deploy_block_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/add_organization_dsp_block_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/add_organization_dsp_block_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/add_organization_dsp_block_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/add_organization_dsp_block_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/add_organization_secret_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/add_organization_secret_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/add_organization_secret_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/add_organization_secret_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/add_organization_secret_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/add_organization_secret_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/add_organization_transfer_learning_block_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/add_organization_transfer_learning_block_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/add_organization_transfer_learning_block_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/add_organization_transfer_learning_block_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/add_organization_transformation_block_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/add_organization_transformation_block_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/add_organization_transformation_block_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/add_organization_transformation_block_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/add_organization_transformation_block_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/add_organization_transformation_block_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/add_project_api_key_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/add_project_api_key_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/add_project_api_key_request_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/add_project_api_key_request_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/admin_add_disallowed_email_domain_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/admin_add_disallowed_email_domain_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/admin_add_or_update_sso_domain_id_ps_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/admin_add_or_update_sso_domain_id_ps_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/admin_add_organization_api_key_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/admin_add_organization_api_key_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/admin_add_organization_user_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/admin_add_organization_user_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/admin_add_organization_user_request_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/admin_add_organization_user_request_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/admin_add_project_api_key_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/admin_add_project_api_key_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/admin_add_project_api_key_request_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/admin_add_project_api_key_request_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/admin_add_project_user_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/admin_add_project_user_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/admin_add_user_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/admin_add_user_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/admin_api_organization.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/admin_api_organization.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/admin_api_organization_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/admin_api_organization_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/admin_api_project.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/admin_api_project.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/admin_api_user.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/admin_api_user.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/admin_api_user_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/admin_api_user_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/admin_create_organization_data_export_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/admin_create_organization_data_export_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/admin_create_organization_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/admin_create_organization_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/admin_create_project_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/admin_create_project_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/admin_enable_feature_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/admin_enable_feature_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/admin_get_data_migration_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/admin_get_data_migration_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/admin_get_data_migration_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/admin_get_data_migration_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/admin_get_data_migrations_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/admin_get_data_migrations_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/admin_get_data_migrations_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/admin_get_data_migrations_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/admin_get_disallowed_email_domains_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/admin_get_disallowed_email_domains_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/admin_get_disallowed_email_domains_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/admin_get_disallowed_email_domains_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/admin_get_metrics_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/admin_get_metrics_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/admin_get_metrics_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/admin_get_metrics_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/admin_get_organization_compute_time_usage_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/admin_get_organization_compute_time_usage_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/admin_get_organization_usage_report_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/admin_get_organization_usage_report_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/admin_get_organization_usage_report_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/admin_get_organization_usage_report_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/admin_get_organization_usage_reports_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/admin_get_organization_usage_reports_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/admin_get_organization_usage_reports_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/admin_get_organization_usage_reports_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/admin_get_organizations_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/admin_get_organizations_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/admin_get_organizations_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/admin_get_organizations_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/admin_get_organizations_response_all_of_organizations.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/admin_get_organizations_response_all_of_organizations.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/admin_get_sso_domain_id_ps_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/admin_get_sso_domain_id_ps_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/admin_get_sso_domain_id_ps_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/admin_get_sso_domain_id_ps_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/admin_get_sso_settings_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/admin_get_sso_settings_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/admin_get_sso_settings_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/admin_get_sso_settings_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/admin_get_sso_settings_response_all_of_sso_whitelist.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/admin_get_sso_settings_response_all_of_sso_whitelist.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/admin_get_user_ids_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/admin_get_user_ids_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/admin_get_user_ids_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/admin_get_user_ids_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/admin_get_user_metrics_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/admin_get_user_metrics_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/admin_get_user_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/admin_get_user_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/admin_get_user_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/admin_get_user_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/admin_get_user_trial_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/admin_get_user_trial_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/admin_get_user_trial_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/admin_get_user_trial_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/admin_get_users_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/admin_get_users_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/admin_get_users_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/admin_get_users_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/admin_get_users_response_all_of_users.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/admin_get_users_response_all_of_users.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/admin_list_projects.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/admin_list_projects.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/admin_list_projects_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/admin_list_projects_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/admin_organization_info_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/admin_organization_info_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/admin_organization_info_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/admin_organization_info_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/admin_toggle_data_migration_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/admin_toggle_data_migration_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/admin_update_organization_data_export_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/admin_update_organization_data_export_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/admin_update_organization_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/admin_update_organization_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/admin_update_user_permissions_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/admin_update_user_permissions_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/admin_update_user_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/admin_update_user_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/admin_update_user_trial_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/admin_update_user_trial_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/akida_edge_learning_config.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/akida_edge_learning_config.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/anomaly_capacity.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/anomaly_capacity.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/anomaly_gmm_metadata.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/anomaly_gmm_metadata.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/anomaly_gmm_metadata_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/anomaly_gmm_metadata_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/anomaly_model_metadata.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/anomaly_model_metadata.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/anomaly_model_metadata_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/anomaly_model_metadata_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/anomaly_model_metadata_all_of_clusters.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/anomaly_model_metadata_all_of_clusters.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/anomaly_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/anomaly_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/anomaly_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/anomaly_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/anomaly_response_all_of_axes.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/anomaly_response_all_of_axes.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/anomaly_result.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/anomaly_result.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/anomaly_trained_features_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/anomaly_trained_features_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/anomaly_trained_features_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/anomaly_trained_features_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/anomaly_trained_features_response_all_of_data.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/anomaly_trained_features_response_all_of_data.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/application_budget.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/application_budget.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/augmentation_policy_spectrogram.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/augmentation_policy_spectrogram.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/autotune_dsp_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/autotune_dsp_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/block_type.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/block_type.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/bounding_box.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/bounding_box.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/bounding_box_with_score.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/bounding_box_with_score.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/build_on_device_model_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/build_on_device_model_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/build_organization_on_device_model_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/build_organization_on_device_model_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/calculate_data_quality_metrics_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/calculate_data_quality_metrics_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/change_password_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/change_password_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/classify_job_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/classify_job_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/classify_job_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/classify_job_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/classify_job_response_all_of_accuracy.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/classify_job_response_all_of_accuracy.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/classify_job_response_all_of_accuracy_total_summary.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/classify_job_response_all_of_accuracy_total_summary.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/classify_job_response_page.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/classify_job_response_page.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/classify_job_response_page_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/classify_job_response_page_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/classify_sample_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/classify_sample_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/classify_sample_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/classify_sample_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/classify_sample_response_classification.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/classify_sample_response_classification.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/classify_sample_response_classification_details.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/classify_sample_response_classification_details.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/classify_sample_v2200_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/classify_sample_v2200_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/convert_user_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/convert_user_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/cosine_similarity_data.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/cosine_similarity_data.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/cosine_similarity_issue.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/cosine_similarity_issue.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/cosine_similarity_issue_issues_inner.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/cosine_similarity_issue_issues_inner.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/cosine_similarity_issue_issues_inner_windows_inner.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/cosine_similarity_issue_issues_inner_windows_inner.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/count_samples_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/count_samples_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/count_samples_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/count_samples_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/create_block_version_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/create_block_version_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/create_block_version_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/create_block_version_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/create_developer_profile_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/create_developer_profile_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/create_developer_profile_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/create_developer_profile_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/create_device_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/create_device_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/create_enterprise_trial_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/create_enterprise_trial_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/create_enterprise_trial_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/create_enterprise_trial_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/create_enterprise_trial_user_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/create_enterprise_trial_user_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/create_enterprise_trial_user_request_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/create_enterprise_trial_user_request_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/create_evaluation_user_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/create_evaluation_user_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/create_evaluation_user_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/create_evaluation_user_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/create_organization_portal_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/create_organization_portal_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/create_organization_portal_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/create_organization_portal_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/create_organization_portal_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/create_organization_portal_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/create_organization_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/create_organization_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/create_organization_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/create_organization_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/create_organization_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/create_organization_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/create_organization_usage_report_body.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/create_organization_usage_report_body.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/create_pipeline_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/create_pipeline_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/create_project_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/create_project_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/create_project_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/create_project_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/create_project_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/create_project_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/create_signed_upload_link_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/create_signed_upload_link_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/create_signed_upload_link_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/create_signed_upload_link_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/create_signed_upload_link_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/create_signed_upload_link_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/create_third_party_auth_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/create_third_party_auth_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/create_third_party_auth_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/create_third_party_auth_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/create_third_party_auth_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/create_third_party_auth_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/create_user_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/create_user_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/create_user_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/create_user_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/create_user_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/create_user_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/create_user_third_party_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/create_user_third_party_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/create_user_third_party_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/create_user_third_party_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/create_user_third_party_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/create_user_third_party_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/create_whitelabel_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/create_whitelabel_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/create_whitelabel_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/create_whitelabel_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/create_whitelabel_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/create_whitelabel_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/created_updated_by_user.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/created_updated_by_user.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/crop_sample_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/crop_sample_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/crop_sample_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/crop_sample_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/crop_sample_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/crop_sample_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/cross_validation_data.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/cross_validation_data.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/cross_validation_data_scores_inner.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/cross_validation_data_scores_inner.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/data_campaign.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/data_campaign.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/data_campaign_dashboard.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/data_campaign_dashboard.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/data_campaign_graph.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/data_campaign_graph.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/data_campaign_graph_x_data_inner.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/data_campaign_graph_x_data_inner.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/data_campaign_graph_x_data_inner_values_inner.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/data_campaign_graph_x_data_inner_values_inner.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/data_campaign_link.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/data_campaign_link.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/data_campaign_query.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/data_campaign_query.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/data_explorer_predictions_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/data_explorer_predictions_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/data_explorer_predictions_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/data_explorer_predictions_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/data_explorer_settings.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/data_explorer_settings.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/dataset_ratio_data.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/dataset_ratio_data.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/dataset_ratio_data_ratio.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/dataset_ratio_data_ratio.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/delete_portal_file_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/delete_portal_file_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/dependency_data.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/dependency_data.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/deploy_pretrained_model_input_audio.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/deploy_pretrained_model_input_audio.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/deploy_pretrained_model_input_image.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/deploy_pretrained_model_input_image.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/deploy_pretrained_model_input_other.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/deploy_pretrained_model_input_other.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/deploy_pretrained_model_input_time_series.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/deploy_pretrained_model_input_time_series.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/deploy_pretrained_model_model_classification.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/deploy_pretrained_model_model_classification.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/deploy_pretrained_model_model_object_detection.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/deploy_pretrained_model_model_object_detection.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/deploy_pretrained_model_model_regression.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/deploy_pretrained_model_model_regression.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/deploy_pretrained_model_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/deploy_pretrained_model_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/deploy_pretrained_model_request_model_info.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/deploy_pretrained_model_request_model_info.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/deploy_pretrained_model_request_model_info_input.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/deploy_pretrained_model_request_model_info_input.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/deploy_pretrained_model_request_model_info_model.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/deploy_pretrained_model_request_model_info_model.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/deployment_target.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/deployment_target.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/deployment_target_badge.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/deployment_target_badge.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/deployment_target_engine.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/deployment_target_engine.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/deployment_targets_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/deployment_targets_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/deployment_targets_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/deployment_targets_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/development_board_created_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/development_board_created_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/development_board_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/development_board_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/development_board_request_update.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/development_board_request_update.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/development_board_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/development_board_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/development_boards_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/development_boards_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/development_boards_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/development_boards_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/development_keys.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/development_keys.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/development_keys_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/development_keys_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/device.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_organization_data_response_all_of_data.py`

 * *Files 20% similar despite different names*

```diff
@@ -13,79 +13,75 @@
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
-from typing import List, Optional
-from pydantic import BaseModel, Field, StrictBool, StrictInt, StrictStr
-from edgeimpulse_api.models.device_sensors_inner import DeviceSensorsInner
+from typing import Dict
+from pydantic import BaseModel, Field, StrictInt, StrictStr
 
-class Device(BaseModel):
+class ListOrganizationDataResponseAllOfData(BaseModel):
     id: StrictInt = ...
-    device_id: StrictStr = Field(..., alias="deviceId", description="Unique identifier (such as MAC address) for a device")
-    created: datetime = ...
-    last_seen: datetime = Field(..., alias="lastSeen", description="Last message that was received from the device (ignoring keep-alive)")
     name: StrictStr = ...
-    device_type: StrictStr = Field(..., alias="deviceType")
-    sensors: List[DeviceSensorsInner] = ...
-    remote_mgmt_connected: StrictBool = Field(..., description="Whether the device is connected to the remote management interface")
-    remote_mgmt_host: Optional[StrictStr] = Field(None, description="The remote management host that the device is connected to")
-    supports_snapshot_streaming: StrictBool = Field(..., alias="supportsSnapshotStreaming")
-    __properties = ["id", "deviceId", "created", "lastSeen", "name", "deviceType", "sensors", "remote_mgmt_connected", "remote_mgmt_host", "supportsSnapshotStreaming"]
+    bucket_id: StrictInt = Field(..., alias="bucketId")
+    bucket_name: StrictStr = Field(..., alias="bucketName")
+    bucket_path: StrictStr = Field(..., alias="bucketPath")
+    full_bucket_path: StrictStr = Field(..., alias="fullBucketPath")
+    dataset: StrictStr = ...
+    total_file_count: StrictInt = Field(..., alias="totalFileCount")
+    total_file_size: StrictInt = Field(..., alias="totalFileSize")
+    created: datetime = ...
+    metadata: Dict[str, StrictStr] = ...
+    metadata_string_for_cli: StrictStr = Field(..., alias="metadataStringForCLI", description="String that's passed in to a transformation block in `--metadata` (the metadata + a `dataItemInfo` object)")
+    __properties = ["id", "name", "bucketId", "bucketName", "bucketPath", "fullBucketPath", "dataset", "totalFileCount", "totalFileSize", "created", "metadata", "metadataStringForCLI"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> Device:
-        """Create an instance of Device from a JSON string"""
+    def from_json(cls, json_str: str) -> ListOrganizationDataResponseAllOfData:
+        """Create an instance of ListOrganizationDataResponseAllOfData from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
-        # override the default output from pydantic by calling `to_dict()` of each item in sensors (list)
-        _items = []
-        if self.sensors:
-            for _item in self.sensors:
-                if _item:
-                    _items.append(_item.to_dict())
-            _dict['sensors'] = _items
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Device:
-        """Create an instance of Device from a dict"""
+    def from_dict(cls, obj: dict) -> ListOrganizationDataResponseAllOfData:
+        """Create an instance of ListOrganizationDataResponseAllOfData from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return Device.construct(**obj)
+            return ListOrganizationDataResponseAllOfData.construct(**obj)
 
-        _obj = Device.construct(**{
+        _obj = ListOrganizationDataResponseAllOfData.construct(**{
             "id": obj.get("id"),
-            "device_id": obj.get("deviceId"),
-            "created": obj.get("created"),
-            "last_seen": obj.get("lastSeen"),
             "name": obj.get("name"),
-            "device_type": obj.get("deviceType"),
-            "sensors": [DeviceSensorsInner.from_dict(_item) for _item in obj.get("sensors")] if obj.get("sensors") is not None else None,
-            "remote_mgmt_connected": obj.get("remote_mgmt_connected"),
-            "remote_mgmt_host": obj.get("remote_mgmt_host"),
-            "supports_snapshot_streaming": obj.get("supportsSnapshotStreaming")
+            "bucket_id": obj.get("bucketId"),
+            "bucket_name": obj.get("bucketName"),
+            "bucket_path": obj.get("bucketPath"),
+            "full_bucket_path": obj.get("fullBucketPath"),
+            "dataset": obj.get("dataset"),
+            "total_file_count": obj.get("totalFileCount"),
+            "total_file_size": obj.get("totalFileSize"),
+            "created": obj.get("created"),
+            "metadata": obj.get("metadata"),
+            "metadata_string_for_cli": obj.get("metadataStringForCLI")
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/device_name_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/device_name_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/device_name_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/device_name_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/device_sensors_inner.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/device_sensors_inner.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/download.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/download.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/download_portal_file_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/download_portal_file_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/download_portal_file_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/download_portal_file_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/download_portal_file_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/download_portal_file_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/dsp_autotuner_results.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/dsp_autotuner_results.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/dsp_autotuner_results_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/dsp_autotuner_results_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/dsp_autotuner_results_all_of_results.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/dsp_autotuner_results_all_of_results.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/dsp_block.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/learn_block.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,72 +15,71 @@
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
 from pydantic import BaseModel, Field, StrictBool, StrictInt, StrictStr
+from edgeimpulse_api.models.block_display_category import BlockDisplayCategory
 from edgeimpulse_api.models.block_type import BlockType
 
-class DSPBlock(BaseModel):
+class LearnBlock(BaseModel):
     type: StrictStr = ...
     title: StrictStr = ...
     author: StrictStr = ...
     description: StrictStr = ...
     name: StrictStr = ...
     recommended: Optional[StrictBool] = None
-    experimental: StrictBool = ...
-    latest_implementation_version: StrictInt = Field(..., alias="latestImplementationVersion")
-    organization_id: Optional[StrictInt] = Field(None, alias="organizationId")
-    organization_dsp_id: Optional[StrictInt] = Field(None, alias="organizationDspId")
+    organization_model_id: Optional[StrictInt] = Field(None, alias="organizationModelId")
+    is_public_enterprise_only: Optional[StrictBool] = Field(None, alias="isPublicEnterpriseOnly", description="Whether this block is publicly available to Edge Impulse only to enterprise users")
     block_type: BlockType = Field(..., alias="blockType")
-    __properties = ["type", "title", "author", "description", "name", "recommended", "experimental", "latestImplementationVersion", "organizationId", "organizationDspId", "blockType"]
+    display_category: Optional[BlockDisplayCategory] = Field(None, alias="displayCategory")
+    __properties = ["type", "title", "author", "description", "name", "recommended", "organizationModelId", "isPublicEnterpriseOnly", "blockType", "displayCategory"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> DSPBlock:
-        """Create an instance of DSPBlock from a JSON string"""
+    def from_json(cls, json_str: str) -> LearnBlock:
+        """Create an instance of LearnBlock from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> DSPBlock:
-        """Create an instance of DSPBlock from a dict"""
+    def from_dict(cls, obj: dict) -> LearnBlock:
+        """Create an instance of LearnBlock from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return DSPBlock.construct(**obj)
+            return LearnBlock.construct(**obj)
 
-        _obj = DSPBlock.construct(**{
+        _obj = LearnBlock.construct(**{
             "type": obj.get("type"),
             "title": obj.get("title"),
             "author": obj.get("author"),
             "description": obj.get("description"),
             "name": obj.get("name"),
             "recommended": obj.get("recommended"),
-            "experimental": obj.get("experimental"),
-            "latest_implementation_version": obj.get("latestImplementationVersion"),
-            "organization_id": obj.get("organizationId"),
-            "organization_dsp_id": obj.get("organizationDspId"),
-            "block_type": obj.get("blockType")
+            "organization_model_id": obj.get("organizationModelId"),
+            "is_public_enterprise_only": obj.get("isPublicEnterpriseOnly"),
+            "block_type": obj.get("blockType"),
+            "display_category": obj.get("displayCategory")
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/dsp_config_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/dsp_config_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/dsp_config_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/dsp_config_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/dsp_config_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/dsp_config_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/dsp_feature_importance_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/dsp_feature_importance_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/dsp_feature_importance_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/dsp_feature_importance_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/dsp_feature_importance_response_all_of_features.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/dsp_feature_importance_response_all_of_features.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/dsp_feature_importance_response_all_of_labels.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/dsp_feature_importance_response_all_of_labels.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/dsp_feature_labels_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/dsp_feature_labels_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/dsp_feature_labels_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/dsp_feature_labels_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/dsp_group.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/dsp_group.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/dsp_group_item.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/dsp_group_item.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/dsp_group_item_select_options_inner.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/dsp_group_item_select_options_inner.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/dsp_group_item_show_if.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/dsp_group_item_show_if.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/dsp_info.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/dsp_info.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/dsp_info_features.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/dsp_info_features.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/dsp_info_performance.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/dsp_info_performance.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/dsp_metadata.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/dsp_metadata.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/dsp_metadata_included_samples_inner.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/dsp_metadata_included_samples_inner.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/dsp_metadata_output_config.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/dsp_metadata_output_config.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/dsp_metadata_output_config_shape.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/dsp_metadata_output_config_shape.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/dsp_metadata_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/dsp_metadata_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/dsp_performance_all_variants_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/dsp_performance_all_variants_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/dsp_performance_all_variants_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/dsp_performance_all_variants_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/dsp_performance_all_variants_response_all_of_performance.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/dsp_performance_all_variants_response_all_of_performance.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/dsp_run_graph.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/dsp_run_graph.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/dsp_run_graph_axis_labels.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/dsp_run_graph_axis_labels.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/dsp_run_request_with_features.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/dsp_run_request_with_features.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/dsp_run_request_without_features.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/dsp_run_request_without_features.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/dsp_run_request_without_features_read_only.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/dsp_run_request_without_features_read_only.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/dsp_run_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/dsp_run_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/dsp_run_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/dsp_run_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/dsp_run_response_all_of_performance.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/dsp_run_response_all_of_performance.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/dsp_run_response_with_sample.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/dsp_run_response_with_sample.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/dsp_run_response_with_sample_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/dsp_run_response_with_sample_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/dsp_sample_features_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/dsp_sample_features_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/dsp_sample_features_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/dsp_sample_features_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/dsp_sample_features_response_all_of_data.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/dsp_sample_features_response_all_of_data.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/dsp_sample_features_response_all_of_sample.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/dsp_sample_features_response_all_of_sample.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/dsp_trained_features_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/dsp_trained_features_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/dsp_trained_features_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/dsp_trained_features_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/dsp_trained_features_response_all_of_data.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/dsp_trained_features_response_all_of_data.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/dsp_trained_features_response_all_of_sample.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/dsp_trained_features_response_all_of_sample.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/edit_sample_label_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/edit_sample_label_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/enterprise_trial.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/enterprise_trial.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/enterprise_upgrade_or_trial_extension_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/enterprise_upgrade_or_trial_extension_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/entitlement_limits.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/entitlement_limits.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/entity_created_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/entity_created_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/entity_created_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/entity_created_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/evaluate_job_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/evaluate_job_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/evaluate_job_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/evaluate_job_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/evaluate_result_value.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/evaluate_result_value.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/export_block_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/export_block_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/export_block_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/export_block_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/export_get_url_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/export_get_url_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/export_get_url_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/export_get_url_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/export_keras_block_data_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/export_keras_block_data_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/export_original_data_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/export_original_data_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/export_wav_data_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/export_wav_data_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/find_segment_sample_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/find_segment_sample_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/find_segment_sample_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/find_segment_sample_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/find_segment_sample_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/find_segment_sample_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/find_segment_sample_response_all_of_segments.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/find_segment_sample_response_all_of_segments.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/find_user_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/find_user_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/find_user_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/find_user_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/find_user_response_all_of_users.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/find_user_response_all_of_users.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/generate_features_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/generate_features_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/generic_api_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/generic_api_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_all_imported_from_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_all_imported_from_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_all_imported_from_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_all_imported_from_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_all_imported_from_response_all_of_data.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_all_imported_from_response_all_of_data.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_all_third_party_auth_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_all_third_party_auth_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_all_third_party_auth_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_all_third_party_auth_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_all_whitelabels_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_all_whitelabels_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_all_whitelabels_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_all_whitelabels_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_auto_labeler_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_auto_labeler_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_auto_labeler_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_auto_labeler_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_auto_labeler_response_all_of_clusters.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_auto_labeler_response_all_of_clusters.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_auto_labeler_response_all_of_items.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_auto_labeler_response_all_of_items.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_csv_wizard_uploaded_file_info.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_csv_wizard_uploaded_file_info.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_csv_wizard_uploaded_file_info_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_csv_wizard_uploaded_file_info_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_data_explorer_features_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_data_explorer_features_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_data_explorer_features_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_data_explorer_features_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_data_explorer_settings_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_data_explorer_settings_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_data_explorer_settings_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_data_explorer_settings_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_deployment_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_deployment_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_deployment_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_deployment_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_device_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_device_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_device_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_device_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_diversity_data_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_diversity_data_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_diversity_data_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_diversity_data_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_diversity_data_response_all_of_cluster_infos.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_diversity_data_response_all_of_cluster_infos.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_diversity_data_response_all_of_data.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_diversity_data_response_all_of_data.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_email_verification_code_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_email_verification_code_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_email_verification_code_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_email_verification_code_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_email_verification_status_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_email_verification_status_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_email_verification_status_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_email_verification_status_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_feature_flags_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_feature_flags_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_feature_flags_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_feature_flags_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_feature_flags_response_all_of_flags.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_feature_flags_response_all_of_flags.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_impulse_blocks_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_impulse_blocks_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_impulse_blocks_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_impulse_blocks_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_impulse_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_impulse_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_impulse_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_impulse_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_job_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_job_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_job_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_job_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_jwt_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_jwt_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_jwt_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_jwt_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_jwt_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_jwt_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_label_noise_data_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_label_noise_data_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_label_noise_data_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_label_noise_data_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_label_noise_data_response_all_of_data.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_label_noise_data_response_all_of_data.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_last_deployment_build_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_last_deployment_build_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_last_deployment_build_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_last_deployment_build_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_last_deployment_build_response_all_of_last_build.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_last_deployment_build_response_all_of_last_build.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_notes_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_notes_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_notes_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_notes_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_organization_bucket_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_organization_bucket_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_organization_bucket_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_organization_bucket_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_organization_data_campaign_dashboard_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_organization_data_campaign_dashboard_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_organization_data_campaign_dashboard_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_organization_data_campaign_dashboard_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_organization_data_campaign_dashboards_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_organization_data_campaign_dashboards_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_organization_data_campaign_dashboards_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_organization_data_campaign_dashboards_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_organization_data_campaign_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_organization_data_campaign_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_organization_data_campaigns_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_organization_data_campaigns_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_organization_data_campaigns_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_organization_data_campaigns_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_organization_data_campaigns_response_all_of_campaigns.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_organization_data_campaigns_response_all_of_campaigns.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_organization_data_export_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_organization_data_export_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_organization_data_export_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_organization_data_export_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_organization_data_exports_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_organization_data_exports_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_organization_data_exports_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_organization_data_exports_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_organization_data_item_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_organization_data_item_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_organization_data_item_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_organization_data_item_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_organization_data_item_transform_jobs_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_organization_data_item_transform_jobs_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_organization_data_item_transform_jobs_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_organization_data_item_transform_jobs_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_organization_data_item_transform_jobs_response_all_of_transformation_jobs.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_organization_data_item_transform_jobs_response_all_of_transformation_jobs.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_organization_dataset_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_organization_dataset_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_organization_dataset_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_organization_dataset_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_organization_deploy_block_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_organization_deploy_block_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_organization_deploy_block_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_organization_deploy_block_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_organization_dsp_block_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_organization_dsp_block_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_organization_dsp_block_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_organization_dsp_block_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_organization_pipelines_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_organization_pipelines_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_organization_pipelines_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_organization_pipelines_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_organization_portal_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_organization_portal_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_organization_portal_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_organization_portal_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_organization_projects_data_count_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_organization_projects_data_count_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_organization_transfer_learning_block_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_organization_transfer_learning_block_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_organization_transfer_learning_block_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_organization_transfer_learning_block_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_organization_transformation_block_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_organization_transformation_block_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_organization_transformation_block_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_organization_transformation_block_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_organization_usage_report_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_organization_usage_report_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_performance_calibration_ground_truth_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_performance_calibration_ground_truth_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_performance_calibration_ground_truth_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_performance_calibration_ground_truth_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_performance_calibration_parameter_sets_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_performance_calibration_parameter_sets_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_performance_calibration_parameter_sets_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_performance_calibration_parameter_sets_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_performance_calibration_parameters_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_performance_calibration_parameters_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_performance_calibration_parameters_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_performance_calibration_parameters_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_performance_calibration_raw_result_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_performance_calibration_raw_result_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_performance_calibration_raw_result_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_performance_calibration_raw_result_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_performance_calibration_status_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_performance_calibration_status_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_performance_calibration_status_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_performance_calibration_status_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_pretrained_model_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_pretrained_model_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_pretrained_model_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_pretrained_model_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_pretrained_model_response_all_of_model.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_pretrained_model_response_all_of_model.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_pretrained_model_response_all_of_model_info.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_pretrained_model_response_all_of_model_info.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_pretrained_model_response_all_of_model_profile_info.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_pretrained_model_response_all_of_model_profile_info.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_public_metrics_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_public_metrics_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_public_metrics_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_public_metrics_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_sample_metadata_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_sample_metadata_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_sample_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_sample_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_syntiant_posterior_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_syntiant_posterior_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_syntiant_posterior_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_syntiant_posterior_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_target_constraints_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_target_constraints_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_target_constraints_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_target_constraints_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_theme_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_theme_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_theme_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_theme_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_themes_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_themes_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_themes_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_themes_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_third_party_auth_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_third_party_auth_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_third_party_auth_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_third_party_auth_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_user_need_to_set_password_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_user_need_to_set_password_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_user_need_to_set_password_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_user_need_to_set_password_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_user_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_user_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_user_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_user_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_user_response_all_of_whitelabels.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_user_response_all_of_whitelabels.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_whitelabel_domain_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_whitelabel_domain_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_whitelabel_domain_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_whitelabel_domain_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_whitelabel_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_whitelabel_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/get_whitelabel_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/get_whitelabel_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/has_data_explorer_features_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/has_data_explorer_features_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/has_data_explorer_features_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/has_data_explorer_features_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/image_input_scaling.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/image_input_scaling.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/impulse.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/impulse.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/impulse_block_version.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/impulse_block_version.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/impulse_dsp_block.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/impulse_dsp_block.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/impulse_dsp_block_organization.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/impulse_dsp_block_organization.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/impulse_input_block.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/impulse_input_block.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/impulse_learn_block.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/impulse_learn_block.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/input_block.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/input_block.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/invite_organization_member_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/invite_organization_member_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/job.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/job.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/job_created_by_user.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/job_created_by_user.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/job_details.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/job_details.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/job_details_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/job_details_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/job_details_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/job_details_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/job_details_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/job_details_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/job_failure_details.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/job_failure_details.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/job_logs_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/job_logs_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/job_logs_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/job_logs_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/job_metrics_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/job_metrics_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/job_metrics_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/job_metrics_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/job_parent_type_enum.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/job_parent_type_enum.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/job_state.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/job_state.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/job_state_execution_details.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/job_state_execution_details.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/job_status.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/job_status.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/job_step.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/job_step.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/job_summary_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/job_summary_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/job_summary_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/job_summary_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/job_summary_response_all_of_summary.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/job_summary_response_all_of_summary.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/keras_custom_metric.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/keras_custom_metric.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/keras_model_layer.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/keras_model_layer.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/keras_model_layer_input.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/keras_model_layer_input.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/keras_model_layer_output.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/keras_model_layer_output.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/keras_model_metadata.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/keras_model_metadata.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/keras_model_metadata_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/keras_model_metadata_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/keras_model_metadata_metrics.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/keras_model_metadata_metrics.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/keras_model_metadata_metrics_on_device_performance_inner.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/keras_model_metadata_metrics_on_device_performance_inner.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/keras_model_metadata_metrics_on_device_performance_inner_tflite.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/keras_model_metadata_metrics_on_device_performance_inner_tflite.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/keras_model_type_enum.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/keras_model_type_enum.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/keras_model_variant_enum.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/keras_model_variant_enum.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/keras_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/keras_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/keras_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/keras_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/keras_visual_layer.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/keras_visual_layer.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/keras_visual_layer_type.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/keras_visual_layer_type.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/last_modification_date_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/last_modification_date_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/last_modification_date_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/last_modification_date_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/latency_device.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/latency_device.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/learn_block.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/portal_info_response.py`

 * *Files 21% similar despite different names*

```diff
@@ -14,72 +14,62 @@
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import BaseModel, Field, StrictBool, StrictInt, StrictStr
-from edgeimpulse_api.models.block_display_category import BlockDisplayCategory
-from edgeimpulse_api.models.block_type import BlockType
-
-class LearnBlock(BaseModel):
-    type: StrictStr = ...
-    title: StrictStr = ...
-    author: StrictStr = ...
-    description: StrictStr = ...
+from pydantic import BaseModel, Field, StrictInt, StrictStr
+
+class PortalInfoResponse(BaseModel):
     name: StrictStr = ...
-    recommended: Optional[StrictBool] = None
-    organization_model_id: Optional[StrictInt] = Field(None, alias="organizationModelId")
-    is_public_enterprise_only: Optional[StrictBool] = Field(None, alias="isPublicEnterpriseOnly", description="Whether this block is publicly available to Edge Impulse only to enterprise users")
-    block_type: BlockType = Field(..., alias="blockType")
-    display_category: Optional[BlockDisplayCategory] = Field(None, alias="displayCategory")
-    __properties = ["type", "title", "author", "description", "name", "recommended", "organizationModelId", "isPublicEnterpriseOnly", "blockType", "displayCategory"]
+    description: StrictStr = ...
+    organization_id: StrictInt = Field(..., alias="organizationId")
+    organization_name: StrictStr = Field(..., alias="organizationName")
+    organization_logo: Optional[StrictStr] = Field(None, alias="organizationLogo")
+    bucket_name: StrictStr = Field(..., alias="bucketName")
+    __properties = ["name", "description", "organizationId", "organizationName", "organizationLogo", "bucketName"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> LearnBlock:
-        """Create an instance of LearnBlock from a JSON string"""
+    def from_json(cls, json_str: str) -> PortalInfoResponse:
+        """Create an instance of PortalInfoResponse from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> LearnBlock:
-        """Create an instance of LearnBlock from a dict"""
+    def from_dict(cls, obj: dict) -> PortalInfoResponse:
+        """Create an instance of PortalInfoResponse from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return LearnBlock.construct(**obj)
+            return PortalInfoResponse.construct(**obj)
 
-        _obj = LearnBlock.construct(**{
-            "type": obj.get("type"),
-            "title": obj.get("title"),
-            "author": obj.get("author"),
-            "description": obj.get("description"),
+        _obj = PortalInfoResponse.construct(**{
             "name": obj.get("name"),
-            "recommended": obj.get("recommended"),
-            "organization_model_id": obj.get("organizationModelId"),
-            "is_public_enterprise_only": obj.get("isPublicEnterpriseOnly"),
-            "block_type": obj.get("blockType"),
-            "display_category": obj.get("displayCategory")
+            "description": obj.get("description"),
+            "organization_id": obj.get("organizationId"),
+            "organization_name": obj.get("organizationName"),
+            "organization_logo": obj.get("organizationLogo"),
+            "bucket_name": obj.get("bucketName")
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/learn_block_type.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/learn_block_type.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_api_keys_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_api_keys_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_api_keys_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_api_keys_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_api_keys_response_all_of_api_keys.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_api_keys_response_all_of_api_keys.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_devices_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_devices_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from typing import List, Optional
 from pydantic import BaseModel, Field, StrictBool, StrictStr
 from edgeimpulse_api.models.device import Device
 
 class ListDevicesResponse(BaseModel):
     success: StrictBool = Field(..., description="Whether the operation succeeded")
     error: Optional[StrictStr] = Field(None, description="Optional error description (set if 'success' was false)")
-    devices: Optional[List[Device]] = None
+    devices: List[Device] = ...
     __properties = ["success", "error", "devices"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
```

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_devices_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_devices_response_all_of.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,20 +13,20 @@
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import List, Optional
+from typing import List
 from pydantic import BaseModel
 from edgeimpulse_api.models.device import Device
 
 class ListDevicesResponseAllOf(BaseModel):
-    devices: Optional[List[Device]] = None
+    devices: List[Device] = ...
     __properties = ["devices"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
```

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_email_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_email_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_email_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_email_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_email_response_all_of_emails.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_email_response_all_of_emails.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_enterprise_trials_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_enterprise_trials_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_enterprise_trials_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_enterprise_trials_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_hmac_keys_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_hmac_keys_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_hmac_keys_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_hmac_keys_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_hmac_keys_response_all_of_hmac_keys.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_hmac_keys_response_all_of_hmac_keys.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_jobs_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_jobs_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_jobs_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_jobs_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_models_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_models_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_models_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_models_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_organization_api_keys_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_organization_api_keys_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_organization_api_keys_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_organization_api_keys_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_organization_api_keys_response_all_of_api_keys.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_organization_api_keys_response_all_of_api_keys.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_organization_buckets_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_organization_buckets_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_organization_buckets_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_organization_buckets_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_organization_buckets_user_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_organization_buckets_user_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_organization_buckets_user_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_organization_buckets_user_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_organization_buckets_user_response_all_of_buckets.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_organization_buckets_user_response_all_of_buckets.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_organization_data_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_organization_data_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_organization_data_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_organization_data_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_organization_data_response_all_of_data.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/organization_data_export.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,75 +13,73 @@
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
-from typing import Dict
-from pydantic import BaseModel, Field, StrictInt, StrictStr
+from typing import Optional
+from pydantic import BaseModel, Field, StrictBool, StrictInt, StrictStr
+from edgeimpulse_api.models.job_created_by_user import JobCreatedByUser
 
-class ListOrganizationDataResponseAllOfData(BaseModel):
+class OrganizationDataExport(BaseModel):
     id: StrictInt = ...
-    name: StrictStr = ...
-    bucket_id: StrictInt = Field(..., alias="bucketId")
-    bucket_name: StrictStr = Field(..., alias="bucketName")
-    bucket_path: StrictStr = Field(..., alias="bucketPath")
-    full_bucket_path: StrictStr = Field(..., alias="fullBucketPath")
-    dataset: StrictStr = ...
-    total_file_count: StrictInt = Field(..., alias="totalFileCount")
-    total_file_size: StrictInt = Field(..., alias="totalFileSize")
     created: datetime = ...
-    metadata: Dict[str, StrictStr] = ...
-    metadata_string_for_cli: StrictStr = Field(..., alias="metadataStringForCLI", description="String that's passed in to a transformation block in `--metadata` (the metadata + a `dataItemInfo` object)")
-    __properties = ["id", "name", "bucketId", "bucketName", "bucketPath", "fullBucketPath", "dataset", "totalFileCount", "totalFileSize", "created", "metadata", "metadataStringForCLI"]
+    created_by_user: Optional[JobCreatedByUser] = Field(None, alias="createdByUser")
+    job_id: StrictInt = Field(..., alias="jobId")
+    job_finished: StrictBool = Field(..., alias="jobFinished")
+    job_finished_successful: StrictBool = Field(..., alias="jobFinishedSuccessful")
+    description: Optional[StrictStr] = Field(None, description="Description of the data export")
+    expiration_date: datetime = Field(..., alias="expirationDate", description="Date when the export will expire. Default is 30 days. Maximum expiration date is 60 days from the creation date.")
+    download_url: Optional[StrictStr] = Field(None, alias="downloadUrl")
+    __properties = ["id", "created", "createdByUser", "jobId", "jobFinished", "jobFinishedSuccessful", "description", "expirationDate", "downloadUrl"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> ListOrganizationDataResponseAllOfData:
-        """Create an instance of ListOrganizationDataResponseAllOfData from a JSON string"""
+    def from_json(cls, json_str: str) -> OrganizationDataExport:
+        """Create an instance of OrganizationDataExport from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
+        # override the default output from pydantic by calling `to_dict()` of created_by_user
+        if self.created_by_user:
+            _dict['createdByUser'] = self.created_by_user.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> ListOrganizationDataResponseAllOfData:
-        """Create an instance of ListOrganizationDataResponseAllOfData from a dict"""
+    def from_dict(cls, obj: dict) -> OrganizationDataExport:
+        """Create an instance of OrganizationDataExport from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return ListOrganizationDataResponseAllOfData.construct(**obj)
+            return OrganizationDataExport.construct(**obj)
 
-        _obj = ListOrganizationDataResponseAllOfData.construct(**{
+        _obj = OrganizationDataExport.construct(**{
             "id": obj.get("id"),
-            "name": obj.get("name"),
-            "bucket_id": obj.get("bucketId"),
-            "bucket_name": obj.get("bucketName"),
-            "bucket_path": obj.get("bucketPath"),
-            "full_bucket_path": obj.get("fullBucketPath"),
-            "dataset": obj.get("dataset"),
-            "total_file_count": obj.get("totalFileCount"),
-            "total_file_size": obj.get("totalFileSize"),
             "created": obj.get("created"),
-            "metadata": obj.get("metadata"),
-            "metadata_string_for_cli": obj.get("metadataStringForCLI")
+            "created_by_user": JobCreatedByUser.from_dict(obj.get("createdByUser")) if obj.get("createdByUser") is not None else None,
+            "job_id": obj.get("jobId"),
+            "job_finished": obj.get("jobFinished"),
+            "job_finished_successful": obj.get("jobFinishedSuccessful"),
+            "description": obj.get("description"),
+            "expiration_date": obj.get("expirationDate"),
+            "download_url": obj.get("downloadUrl")
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_organization_deploy_blocks_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_organization_deploy_blocks_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_organization_deploy_blocks_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_organization_deploy_blocks_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_organization_dsp_blocks_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_organization_dsp_blocks_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_organization_dsp_blocks_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_organization_dsp_blocks_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_organization_files_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_organization_files_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_organization_files_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_organization_files_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_organization_pipelines_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_organization_pipelines_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_organization_pipelines_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_organization_pipelines_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_organization_portals_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_organization_portals_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_organization_portals_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_organization_portals_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_organization_portals_response_all_of_portals.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_organization_portals_response_all_of_portals.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_organization_projects_data_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_organization_projects_data_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_organization_projects_data_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_organization_projects_data_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_organization_projects_data_response_all_of_projects.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_organization_projects_data_response_all_of_projects.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_organization_secrets_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_organization_secrets_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_organization_secrets_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_organization_secrets_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_organization_secrets_response_all_of_secrets.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_organization_secrets_response_all_of_secrets.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_organization_transfer_learning_blocks_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_organization_transfer_learning_blocks_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_organization_transfer_learning_blocks_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_organization_transfer_learning_blocks_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_organization_transformation_blocks_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_organization_transformation_blocks_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_organization_transformation_blocks_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_organization_transformation_blocks_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_organization_usage_reports_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_organization_usage_reports_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_organization_usage_reports_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_organization_usage_reports_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_organizations_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_organizations_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_organizations_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_organizations_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_portal_files_in_folder_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_portal_files_in_folder_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_portal_files_in_folder_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_portal_files_in_folder_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_portal_files_in_folder_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_portal_files_in_folder_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_projects.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_projects.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_projects_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_projects_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_public_organization_transformation_blocks_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_public_organization_transformation_blocks_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_public_organization_transformation_blocks_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_public_organization_transformation_blocks_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_public_projects.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_public_projects.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_public_projects_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_public_projects_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_public_versions_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_public_versions_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_public_versions_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_public_versions_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_public_versions_response_all_of_versions.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_public_versions_response_all_of_versions.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_samples_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_samples_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_samples_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_samples_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_tuner_runs_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_tuner_runs_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_tuner_runs_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_tuner_runs_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_versions_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_versions_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_versions_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_versions_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_versions_response_all_of_bucket.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_versions_response_all_of_bucket.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_versions_response_all_of_custom_learn_blocks.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_versions_response_all_of_custom_learn_blocks.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/list_versions_response_all_of_versions.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/list_versions_response_all_of_versions.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/log_analytics_event_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/log_analytics_event_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/log_stdout_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/log_stdout_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/log_stdout_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/log_stdout_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/log_stdout_response_all_of_stdout.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/log_stdout_response_all_of_stdout.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/log_website_pageview_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/log_website_pageview_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/login_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/login_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/login_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/login_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/memory_spec.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/memory_spec.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/metrics_all_variants_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/metrics_all_variants_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/metrics_all_variants_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/metrics_all_variants_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/metrics_for_model_variant.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/metrics_for_model_variant.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/migration.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/migration.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/model_engine_short_enum.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/model_engine_short_enum.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/model_prediction.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/model_prediction.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/model_result.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/model_result.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/model_variant_stats.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/model_variant_stats.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/move_raw_data_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/move_raw_data_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/neighbors_data.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/neighbors_data.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/neighbors_score.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/neighbors_score.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/neighbors_score_neighbor_windows_inner.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/neighbors_score_neighbor_windows_inner.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/note.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/note.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/object_detection_auto_label_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/object_detection_auto_label_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/object_detection_auto_label_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/object_detection_auto_label_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/object_detection_auto_label_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/object_detection_auto_label_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/object_detection_auto_label_response_all_of_results.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/object_detection_auto_label_response_all_of_results.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/object_detection_label_queue_count_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/object_detection_label_queue_count_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/object_detection_label_queue_count_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/object_detection_label_queue_count_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/object_detection_label_queue_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/object_detection_label_queue_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/object_detection_label_queue_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/object_detection_label_queue_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/object_detection_last_layer.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/object_detection_last_layer.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/optimize_config.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/optimize_config.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/optimize_config_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/optimize_config_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/optimize_config_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/optimize_config_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/optimize_config_target_device.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/optimize_config_target_device.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/optimize_dsp_parameters_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/optimize_dsp_parameters_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/optimize_dsp_parameters_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/optimize_dsp_parameters_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/optimize_space_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/optimize_space_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/optimize_space_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/optimize_space_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/optimize_state_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/optimize_state_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/optimize_state_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/optimize_state_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/optimize_state_response_all_of_status.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/optimize_state_response_all_of_status.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/optimize_state_response_all_of_workers.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/optimize_state_response_all_of_workers.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/optimize_transfer_learning_models_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/optimize_transfer_learning_models_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/optimize_transfer_learning_models_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/optimize_transfer_learning_models_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/optimize_transfer_learning_models_response_all_of_models.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/optimize_transfer_learning_models_response_all_of_models.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/organization.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/organization.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/organization_add_data_folder_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/organization_add_data_folder_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/organization_add_data_folder_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/organization_add_data_folder_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/organization_add_data_folder_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/organization_add_data_folder_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/organization_add_dataset_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/organization_add_dataset_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/organization_add_dataset_request_bucket.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/organization_add_dataset_request_bucket.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/organization_bucket.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/organization_bucket.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/organization_compute_time_usage.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/organization_compute_time_usage.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/organization_create_project.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/organization_create_project.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/organization_create_project_output_dataset_path_rule.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/organization_create_project_output_dataset_path_rule.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/organization_create_project_path_filter.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/organization_create_project_path_filter.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/organization_create_project_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/organization_create_project_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/organization_create_project_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/organization_create_project_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/organization_create_project_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/organization_create_project_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/organization_create_project_status_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/organization_create_project_status_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/organization_create_project_status_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/organization_create_project_status_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/organization_create_project_transformation_summary.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/organization_create_project_transformation_summary.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/organization_create_project_with_files.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/organization_create_project_with_files.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/organization_create_project_with_files_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/organization_create_project_with_files_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/organization_create_project_with_files_all_of_files.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/organization_create_project_with_files_all_of_files.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/organization_data_campaign_diff_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/organization_data_campaign_diff_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/organization_data_campaign_diff_request_queries_inner.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/organization_data_campaign_diff_request_queries_inner.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/organization_data_campaign_diff_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/organization_data_campaign_diff_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/organization_data_campaign_diff_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/organization_data_campaign_diff_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/organization_data_campaign_diff_response_all_of_queries.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/organization_data_campaign_diff_response_all_of_queries.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/organization_data_export.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/project_collaborator.py`

 * *Files 20% similar despite different names*

```diff
@@ -13,73 +13,88 @@
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
-from typing import Optional
+from typing import List, Optional
 from pydantic import BaseModel, Field, StrictBool, StrictInt, StrictStr
-from edgeimpulse_api.models.job_created_by_user import JobCreatedByUser
+from edgeimpulse_api.models.permission import Permission
+from edgeimpulse_api.models.staff_info import StaffInfo
 
-class OrganizationDataExport(BaseModel):
+class ProjectCollaborator(BaseModel):
     id: StrictInt = ...
+    username: StrictStr = ...
+    name: StrictStr = ...
+    email: StrictStr = ...
+    photo: Optional[StrictStr] = None
     created: datetime = ...
-    created_by_user: Optional[JobCreatedByUser] = Field(None, alias="createdByUser")
-    job_id: StrictInt = Field(..., alias="jobId")
-    job_finished: StrictBool = Field(..., alias="jobFinished")
-    job_finished_successful: StrictBool = Field(..., alias="jobFinishedSuccessful")
-    description: Optional[StrictStr] = Field(None, description="Description of the data export")
-    expiration_date: datetime = Field(..., alias="expirationDate", description="Date when the export will expire. Default is 30 days. Maximum expiration date is 60 days from the creation date.")
-    download_url: Optional[StrictStr] = Field(None, alias="downloadUrl")
-    __properties = ["id", "created", "createdByUser", "jobId", "jobFinished", "jobFinishedSuccessful", "description", "expirationDate", "downloadUrl"]
+    last_seen: Optional[datetime] = Field(None, alias="lastSeen")
+    staff_info: StaffInfo = Field(..., alias="staffInfo")
+    pending: StrictBool = ...
+    last_tos_acceptance_date: Optional[datetime] = Field(None, alias="lastTosAcceptanceDate")
+    job_title: Optional[StrictStr] = Field(None, alias="jobTitle")
+    permissions: Optional[List[Permission]] = Field(None, description="List of permissions the user has")
+    company_name: Optional[StrictStr] = Field(None, alias="companyName")
+    activated: StrictBool = Field(..., description="Whether the user has activated their account or not.")
+    mfa_configured: StrictBool = Field(..., alias="mfaConfigured", description="Whether the user has configured multi-factor authentication")
+    is_owner: StrictBool = Field(..., alias="isOwner")
+    __properties = ["id", "username", "name", "email", "photo", "created", "lastSeen", "staffInfo", "pending", "lastTosAcceptanceDate", "jobTitle", "permissions", "companyName", "activated", "mfaConfigured", "isOwner"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> OrganizationDataExport:
-        """Create an instance of OrganizationDataExport from a JSON string"""
+    def from_json(cls, json_str: str) -> ProjectCollaborator:
+        """Create an instance of ProjectCollaborator from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
-        # override the default output from pydantic by calling `to_dict()` of created_by_user
-        if self.created_by_user:
-            _dict['createdByUser'] = self.created_by_user.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of staff_info
+        if self.staff_info:
+            _dict['staffInfo'] = self.staff_info.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> OrganizationDataExport:
-        """Create an instance of OrganizationDataExport from a dict"""
+    def from_dict(cls, obj: dict) -> ProjectCollaborator:
+        """Create an instance of ProjectCollaborator from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return OrganizationDataExport.construct(**obj)
+            return ProjectCollaborator.construct(**obj)
 
-        _obj = OrganizationDataExport.construct(**{
+        _obj = ProjectCollaborator.construct(**{
             "id": obj.get("id"),
+            "username": obj.get("username"),
+            "name": obj.get("name"),
+            "email": obj.get("email"),
+            "photo": obj.get("photo"),
             "created": obj.get("created"),
-            "created_by_user": JobCreatedByUser.from_dict(obj.get("createdByUser")) if obj.get("createdByUser") is not None else None,
-            "job_id": obj.get("jobId"),
-            "job_finished": obj.get("jobFinished"),
-            "job_finished_successful": obj.get("jobFinishedSuccessful"),
-            "description": obj.get("description"),
-            "expiration_date": obj.get("expirationDate"),
-            "download_url": obj.get("downloadUrl")
+            "last_seen": obj.get("lastSeen"),
+            "staff_info": StaffInfo.from_dict(obj.get("staffInfo")) if obj.get("staffInfo") is not None else None,
+            "pending": obj.get("pending"),
+            "last_tos_acceptance_date": obj.get("lastTosAcceptanceDate"),
+            "job_title": obj.get("jobTitle"),
+            "permissions": obj.get("permissions"),
+            "company_name": obj.get("companyName"),
+            "activated": obj.get("activated"),
+            "mfa_configured": obj.get("mfaConfigured"),
+            "is_owner": obj.get("isOwner")
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/organization_data_item.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/organization_data_item.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/organization_data_item_files_inner.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/organization_data_item_files_inner.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/organization_dataset.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/organization_dataset.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/organization_dataset_bucket.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/organization_dataset_bucket.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/organization_deploy_block.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/organization_deploy_block.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/organization_dsp_block.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/organization_dsp_block.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/organization_get_create_projects_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/organization_get_create_projects_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/organization_get_create_projects_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/organization_get_create_projects_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/organization_get_create_projects_response_all_of_jobs.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/organization_get_create_projects_response_all_of_jobs.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/organization_info_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/organization_info_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/organization_info_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/organization_info_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/organization_info_response_all_of_cli_lists.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/organization_info_response_all_of_cli_lists.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/organization_info_response_all_of_cli_lists_image_input_scaling_options.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/organization_info_response_all_of_cli_lists_image_input_scaling_options.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/organization_info_response_all_of_cli_lists_object_detection_last_layer_options.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/organization_info_response_all_of_cli_lists_object_detection_last_layer_options.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/organization_info_response_all_of_default_compute_limits.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/organization_info_response_all_of_default_compute_limits.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/organization_info_response_all_of_performance.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/organization_info_response_all_of_performance.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/organization_member_role.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/organization_member_role.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/organization_metrics_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/organization_metrics_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/organization_metrics_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/organization_metrics_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/organization_metrics_response_all_of_metrics.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/organization_metrics_response_all_of_metrics.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/organization_pipeline.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/organization_pipeline.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/organization_pipeline_feeding_into_dataset.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/organization_pipeline_feeding_into_dataset.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/organization_pipeline_feeding_into_project.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/organization_pipeline_feeding_into_project.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/organization_pipeline_item_count.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/organization_pipeline_item_count.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/organization_pipeline_run.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/organization_pipeline_run.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/organization_pipeline_run_step.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/organization_pipeline_run_step.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/organization_pipeline_step.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/organization_pipeline_step.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/organization_projects_data_batch_disable_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/organization_projects_data_batch_disable_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/organization_projects_data_batch_enable_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/organization_projects_data_batch_enable_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/organization_projects_data_batch_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/organization_projects_data_batch_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/organization_transfer_learning_block.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/organization_transfer_learning_block.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/organization_transfer_learning_operates_on.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/organization_transfer_learning_operates_on.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/organization_transformation_block.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/organization_transformation_block.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/organization_update_pipeline_body.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/organization_update_pipeline_body.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/organization_usage_report.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/organization_usage_report.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/organization_user.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/organization_user.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/organization_user_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/organization_user_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/performance_calibration_detection.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/performance_calibration_detection.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/performance_calibration_false_positive.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/performance_calibration_false_positive.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/performance_calibration_ground_truth.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/performance_calibration_ground_truth.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/performance_calibration_ground_truth_samples_inner.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/performance_calibration_ground_truth_samples_inner.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/performance_calibration_parameter_set.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/performance_calibration_parameter_set.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/performance_calibration_parameter_set_aggregate_stats.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/performance_calibration_parameter_set_aggregate_stats.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/performance_calibration_parameter_set_stats_inner.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/performance_calibration_parameter_set_stats_inner.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/performance_calibration_parameters.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/performance_calibration_parameters.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/performance_calibration_parameters_standard.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/performance_calibration_parameters_standard.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/performance_calibration_raw_detection.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/performance_calibration_raw_detection.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/performance_calibration_save_parameter_set_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/performance_calibration_save_parameter_set_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/performance_calibration_upload_labeled_audio_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/performance_calibration_upload_labeled_audio_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/performance_calibration_upload_labeled_audio_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/performance_calibration_upload_labeled_audio_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/permission.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/permission.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/portal_file.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/portal_file.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/portal_info_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/sample_metadata.py`

 * *Files 19% similar despite different names*

```diff
@@ -13,63 +13,55 @@
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import Optional
+from typing import Dict
 from pydantic import BaseModel, Field, StrictInt, StrictStr
 
-class PortalInfoResponse(BaseModel):
-    name: StrictStr = ...
-    description: StrictStr = ...
-    organization_id: StrictInt = Field(..., alias="organizationId")
-    organization_name: StrictStr = Field(..., alias="organizationName")
-    organization_logo: Optional[StrictStr] = Field(None, alias="organizationLogo")
-    bucket_name: StrictStr = Field(..., alias="bucketName")
-    __properties = ["name", "description", "organizationId", "organizationName", "organizationLogo", "bucketName"]
+class SampleMetadata(BaseModel):
+    id: StrictInt = Field(..., description="Sample ID")
+    metadata: Dict[str, StrictStr] = Field(..., description="Sample free form associated metadata")
+    __properties = ["id", "metadata"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> PortalInfoResponse:
-        """Create an instance of PortalInfoResponse from a JSON string"""
+    def from_json(cls, json_str: str) -> SampleMetadata:
+        """Create an instance of SampleMetadata from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> PortalInfoResponse:
-        """Create an instance of PortalInfoResponse from a dict"""
+    def from_dict(cls, obj: dict) -> SampleMetadata:
+        """Create an instance of SampleMetadata from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return PortalInfoResponse.construct(**obj)
+            return SampleMetadata.construct(**obj)
 
-        _obj = PortalInfoResponse.construct(**{
-            "name": obj.get("name"),
-            "description": obj.get("description"),
-            "organization_id": obj.get("organizationId"),
-            "organization_name": obj.get("organizationName"),
-            "organization_logo": obj.get("organizationLogo"),
-            "bucket_name": obj.get("bucketName")
+        _obj = SampleMetadata.construct(**{
+            "id": obj.get("id"),
+            "metadata": obj.get("metadata")
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/pretrained_model_tensor.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/pretrained_model_tensor.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/preview_default_files_in_folder_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/preview_default_files_in_folder_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/preview_default_files_in_folder_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/preview_default_files_in_folder_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/preview_default_files_in_folder_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/preview_default_files_in_folder_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/profile_model_info.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/profile_model_info.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/profile_model_info_memory.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/profile_model_info_memory.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/profile_model_info_memory_eon.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/profile_model_info_memory_eon.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/profile_model_info_memory_tflite.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/profile_model_info_memory_tflite.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/profile_model_table.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/profile_model_table.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/profile_model_table_mcu.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/profile_model_table_mcu.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/profile_model_table_mcu_memory.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/profile_model_table_mcu_memory.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/profile_model_table_mpu.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/profile_model_table_mpu.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/profile_tf_lite_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/profile_tf_lite_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/profile_tf_lite_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/profile_tf_lite_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/project.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/project.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/project_collaborator.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/user.py`

 * *Files 17% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 from datetime import datetime
 from typing import List, Optional
 from pydantic import BaseModel, Field, StrictBool, StrictInt, StrictStr
 from edgeimpulse_api.models.permission import Permission
 from edgeimpulse_api.models.staff_info import StaffInfo
 
-class ProjectCollaborator(BaseModel):
+class User(BaseModel):
     id: StrictInt = ...
     username: StrictStr = ...
     name: StrictStr = ...
     email: StrictStr = ...
     photo: Optional[StrictStr] = None
     created: datetime = ...
     last_seen: Optional[datetime] = Field(None, alias="lastSeen")
@@ -34,67 +34,65 @@
     pending: StrictBool = ...
     last_tos_acceptance_date: Optional[datetime] = Field(None, alias="lastTosAcceptanceDate")
     job_title: Optional[StrictStr] = Field(None, alias="jobTitle")
     permissions: Optional[List[Permission]] = Field(None, description="List of permissions the user has")
     company_name: Optional[StrictStr] = Field(None, alias="companyName")
     activated: StrictBool = Field(..., description="Whether the user has activated their account or not.")
     mfa_configured: StrictBool = Field(..., alias="mfaConfigured", description="Whether the user has configured multi-factor authentication")
-    is_owner: StrictBool = Field(..., alias="isOwner")
-    __properties = ["id", "username", "name", "email", "photo", "created", "lastSeen", "staffInfo", "pending", "lastTosAcceptanceDate", "jobTitle", "permissions", "companyName", "activated", "mfaConfigured", "isOwner"]
+    __properties = ["id", "username", "name", "email", "photo", "created", "lastSeen", "staffInfo", "pending", "lastTosAcceptanceDate", "jobTitle", "permissions", "companyName", "activated", "mfaConfigured"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> ProjectCollaborator:
-        """Create an instance of ProjectCollaborator from a JSON string"""
+    def from_json(cls, json_str: str) -> User:
+        """Create an instance of User from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         # override the default output from pydantic by calling `to_dict()` of staff_info
         if self.staff_info:
             _dict['staffInfo'] = self.staff_info.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> ProjectCollaborator:
-        """Create an instance of ProjectCollaborator from a dict"""
+    def from_dict(cls, obj: dict) -> User:
+        """Create an instance of User from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return ProjectCollaborator.construct(**obj)
+            return User.construct(**obj)
 
-        _obj = ProjectCollaborator.construct(**{
+        _obj = User.construct(**{
             "id": obj.get("id"),
             "username": obj.get("username"),
             "name": obj.get("name"),
             "email": obj.get("email"),
             "photo": obj.get("photo"),
             "created": obj.get("created"),
             "last_seen": obj.get("lastSeen"),
             "staff_info": StaffInfo.from_dict(obj.get("staffInfo")) if obj.get("staffInfo") is not None else None,
             "pending": obj.get("pending"),
             "last_tos_acceptance_date": obj.get("lastTosAcceptanceDate"),
             "job_title": obj.get("jobTitle"),
             "permissions": obj.get("permissions"),
             "company_name": obj.get("companyName"),
             "activated": obj.get("activated"),
-            "mfa_configured": obj.get("mfaConfigured"),
-            "is_owner": obj.get("isOwner")
+            "mfa_configured": obj.get("mfaConfigured")
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/project_collaborator_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/project_collaborator_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/project_data_axes_summary_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/project_data_axes_summary_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/project_data_axes_summary_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/project_data_axes_summary_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/project_data_interval_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/project_data_interval_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/project_data_interval_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/project_data_interval_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/project_data_summary.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/project_data_summary.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/project_deployment_target.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/project_deployment_target.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/project_deployment_target_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/project_deployment_target_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/project_deployment_targets_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/project_deployment_targets_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/project_deployment_targets_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/project_deployment_targets_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/project_dismiss_notification_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/project_dismiss_notification_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/project_downloads_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/project_downloads_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/project_downloads_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/project_downloads_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/project_info_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/project_info_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/project_info_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/project_info_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/project_info_response_all_of_acquisition_settings.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/project_info_response_all_of_acquisition_settings.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/project_info_response_all_of_compute_time.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/project_info_response_all_of_compute_time.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/project_info_response_all_of_data_summary_per_category.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/project_info_response_all_of_data_summary_per_category.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/project_info_response_all_of_deploy_settings.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/project_info_response_all_of_deploy_settings.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/project_info_response_all_of_experiments.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/project_info_response_all_of_experiments.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/project_info_response_all_of_impulse.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/project_info_response_all_of_impulse.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/project_info_response_all_of_performance.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/project_info_response_all_of_performance.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/project_info_response_all_of_readme.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/project_info_response_all_of_readme.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/project_info_response_all_of_show_getting_started_wizard.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/project_info_response_all_of_show_getting_started_wizard.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/project_info_response_all_of_urls.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/project_info_response_all_of_urls.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/project_info_summary_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/project_info_summary_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/project_info_summary_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/project_info_summary_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/project_private_data.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/project_private_data.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/project_public_data.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/project_public_data.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/project_public_data_readme.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/project_public_data_readme.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/project_sample_metadata.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/project_sample_metadata.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/project_tier_enum.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/project_tier_enum.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/project_training_data_summary_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/project_training_data_summary_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/project_training_data_summary_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/project_training_data_summary_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/project_training_data_summary_response_all_of_data_summary.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/project_training_data_summary_response_all_of_data_summary.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/project_type.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/project_type.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/project_version_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/project_version_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/public_organization_transformation_block.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/public_organization_transformation_block.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/raw_sample_data.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/raw_sample_data.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/raw_sample_payload.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/raw_sample_payload.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/rebalance_dataset_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/rebalance_dataset_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/remove_collaborator_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/remove_collaborator_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/remove_member_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/remove_member_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/rename_device_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/rename_device_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/rename_portal_file_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/rename_portal_file_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/rename_sample_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/rename_sample_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/request_email_verification_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/request_email_verification_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/request_reset_password_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/request_reset_password_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/reset_password_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/reset_password_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/resource_range.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/resource_range.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/restore_project_from_public_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/restore_project_from_public_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/restore_project_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/restore_project_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/run_auto_labeler_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/run_auto_labeler_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/run_organization_pipeline_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/run_organization_pipeline_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/run_organization_pipeline_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/run_organization_pipeline_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/sample.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/sample.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/sample_bounding_boxes_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/sample_bounding_boxes_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/sample_metadata.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/sensor.py`

 * *Files 19% similar despite different names*

```diff
@@ -13,55 +13,55 @@
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import Dict
-from pydantic import BaseModel, Field, StrictInt, StrictStr
 
-class SampleMetadata(BaseModel):
-    id: StrictInt = Field(..., description="Sample ID")
-    metadata: Dict[str, StrictStr] = Field(..., description="Sample free form associated metadata")
-    __properties = ["id", "metadata"]
+from pydantic import BaseModel, Field, StrictStr
+
+class Sensor(BaseModel):
+    name: StrictStr = Field(..., description="Name of the axis")
+    units: StrictStr = Field(..., description="Type of data on this axis. Needs to comply to SenML units (see https://www.iana.org/assignments/senml/senml.xhtml).")
+    __properties = ["name", "units"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> SampleMetadata:
-        """Create an instance of SampleMetadata from a JSON string"""
+    def from_json(cls, json_str: str) -> Sensor:
+        """Create an instance of Sensor from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> SampleMetadata:
-        """Create an instance of SampleMetadata from a dict"""
+    def from_dict(cls, obj: dict) -> Sensor:
+        """Create an instance of Sensor from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return SampleMetadata.construct(**obj)
+            return Sensor.construct(**obj)
 
-        _obj = SampleMetadata.construct(**{
-            "id": obj.get("id"),
-            "metadata": obj.get("metadata")
+        _obj = Sensor.construct(**{
+            "name": obj.get("name"),
+            "units": obj.get("units")
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/save_auto_labeler_clusters_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/save_auto_labeler_clusters_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/save_auto_labeler_clusters_request_clusters_inner.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/save_auto_labeler_clusters_request_clusters_inner.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/save_auto_labeler_clusters_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/save_auto_labeler_clusters_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/save_auto_labeler_clusters_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/save_auto_labeler_clusters_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/save_pretrained_model_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/save_pretrained_model_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/score_trial_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/score_trial_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/score_trial_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/score_trial_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/score_trial_response_all_of_latency.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/score_trial_response_all_of_latency.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/score_trial_response_all_of_ram.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/score_trial_response_all_of_ram.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/segment_sample_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/segment_sample_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/segment_sample_request_segments_inner.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/segment_sample_request_segments_inner.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/send_user_feedback_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/send_user_feedback_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/sensor.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/start_device_debug_stream_response.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,55 +13,57 @@
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
+from typing import Optional
+from pydantic import BaseModel, Field, StrictBool, StrictInt, StrictStr
 
-from pydantic import BaseModel, Field, StrictStr
-
-class Sensor(BaseModel):
-    name: StrictStr = Field(..., description="Name of the axis")
-    units: StrictStr = Field(..., description="Type of data on this axis. Needs to comply to SenML units (see https://www.iana.org/assignments/senml/senml.xhtml).")
-    __properties = ["name", "units"]
+class StartDeviceDebugStreamResponse(BaseModel):
+    success: StrictBool = Field(..., description="Whether the operation succeeded")
+    error: Optional[StrictStr] = Field(None, description="Optional error description (set if 'success' was false)")
+    stream_id: StrictInt = Field(..., alias="streamId")
+    __properties = ["success", "error", "streamId"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> Sensor:
-        """Create an instance of Sensor from a JSON string"""
+    def from_json(cls, json_str: str) -> StartDeviceDebugStreamResponse:
+        """Create an instance of StartDeviceDebugStreamResponse from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Sensor:
-        """Create an instance of Sensor from a dict"""
+    def from_dict(cls, obj: dict) -> StartDeviceDebugStreamResponse:
+        """Create an instance of StartDeviceDebugStreamResponse from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return Sensor.construct(**obj)
+            return StartDeviceDebugStreamResponse.construct(**obj)
 
-        _obj = Sensor.construct(**{
-            "name": obj.get("name"),
-            "units": obj.get("units")
+        _obj = StartDeviceDebugStreamResponse.construct(**{
+            "success": obj.get("success"),
+            "error": obj.get("error"),
+            "stream_id": obj.get("streamId")
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/set_anomaly_parameter_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/set_anomaly_parameter_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/set_keras_parameter_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/set_keras_parameter_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/set_member_datasets_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/set_member_datasets_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/set_member_role_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/set_member_role_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/set_optimize_space_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/set_optimize_space_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/set_optimize_space_request_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/set_optimize_space_request_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/set_organization_data_dataset_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/set_organization_data_dataset_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/set_project_compute_time_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/set_project_compute_time_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/set_project_dsp_file_size_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/set_project_dsp_file_size_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/set_sample_metadata_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/set_sample_metadata_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/set_sample_structured_labels_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/set_sample_structured_labels_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/set_syntiant_posterior_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/set_syntiant_posterior_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/set_user_password_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/set_user_password_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/socket_token_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/socket_token_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/socket_token_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/socket_token_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/socket_token_response_all_of_token.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/socket_token_response_all_of_token.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/split_sample_in_frames_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/split_sample_in_frames_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/staff_info.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/staff_info.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/start_enterprise_trial_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/start_enterprise_trial_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/start_job_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/start_job_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/start_job_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/start_job_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/start_performance_calibration_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/start_performance_calibration_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/start_sampling_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/start_sampling_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/start_sampling_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/start_sampling_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/start_sampling_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/start_sampling_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/start_training_request_anomaly.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/start_training_request_anomaly.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/store_segment_length_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/store_segment_length_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/structured_classify_result.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/structured_classify_result.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/structured_label.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/structured_label.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/target_constraints.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/target_constraints.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/target_constraints_device.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/target_constraints_device.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/target_memory.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/target_memory.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/target_processor.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/target_processor.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/test_pretrained_model_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/test_pretrained_model_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/test_pretrained_model_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/test_pretrained_model_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/test_pretrained_model_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/test_pretrained_model_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/theme.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/theme.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/theme_colors.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/theme_colors.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/theme_favicon.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/theme_favicon.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/theme_logos.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/theme_logos.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/third_party_auth.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/third_party_auth.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/time_series_data_point.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/time_series_data_point.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/track_objects_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/track_objects_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/track_objects_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/track_objects_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/track_objects_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/track_objects_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/transfer_learning_model.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/transfer_learning_model.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/transfer_ownership_organization_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/transfer_ownership_organization_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/transformation_block_additional_mount_point.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/transformation_block_additional_mount_point.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/transformation_job_operates_on_enum.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/transformation_job_operates_on_enum.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/transformation_job_status_enum.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/transformation_job_status_enum.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/tuner_create_trial_impulse.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/tuner_create_trial_impulse.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/tuner_run.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/tuner_run.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/tuner_space_impulse.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/tuner_space_impulse.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/tuner_trial.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/tuner_trial.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/tuner_trial_blocks_inner.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/tuner_trial_blocks_inner.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/tuner_trial_dsp_job_id.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/tuner_trial_dsp_job_id.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/tuner_trial_impulse.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/tuner_trial_impulse.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/update_job_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/update_job_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/update_organization_add_collaborator_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/update_organization_add_collaborator_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/update_organization_bucket_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/update_organization_bucket_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/update_organization_create_empty_project_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/update_organization_create_empty_project_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/update_organization_create_project_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/update_organization_create_project_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/update_organization_data_campaign_dashboard_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/update_organization_data_campaign_dashboard_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/update_organization_data_campaign_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/update_organization_data_campaign_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/update_organization_data_item_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/update_organization_data_item_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/update_organization_dataset_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/update_organization_dataset_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/update_organization_dataset_request_bucket.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/update_organization_dataset_request_bucket.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/update_organization_dsp_block_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/update_organization_dsp_block_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/update_organization_portal_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/update_organization_portal_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/update_organization_portal_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/update_organization_portal_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/update_organization_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/update_organization_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/update_organization_transfer_learning_block_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/update_organization_transfer_learning_block_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/update_organization_transformation_block_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/update_organization_transformation_block_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/update_project_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/update_project_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/update_project_tags_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/update_project_tags_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/update_theme_colors_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/update_theme_colors_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/update_theme_logos_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/update_theme_logos_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/update_third_party_auth_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/update_third_party_auth_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/update_tuner_run_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/update_tuner_run_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/update_user_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/update_user_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/update_version_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/update_version_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/update_whitelabel_default_deployment_target_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/update_whitelabel_default_deployment_target_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/update_whitelabel_deployment_options_order_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/update_whitelabel_deployment_options_order_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/update_whitelabel_deployment_targets_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/update_whitelabel_deployment_targets_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/update_whitelabel_learning_blocks_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/update_whitelabel_learning_blocks_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/update_whitelabel_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/update_whitelabel_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/upload_asset_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/upload_asset_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/upload_asset_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/upload_asset_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/upload_readme_image_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/upload_readme_image_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/upload_user_photo_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/upload_user_photo_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/upload_user_photo_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/upload_user_photo_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/user.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/user_organization.py`

 * *Files 24% similar despite different names*

```diff
@@ -13,86 +13,93 @@
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
-from typing import List, Optional
+from typing import Optional
 from pydantic import BaseModel, Field, StrictBool, StrictInt, StrictStr
-from edgeimpulse_api.models.permission import Permission
-from edgeimpulse_api.models.staff_info import StaffInfo
+from edgeimpulse_api.models.entitlement_limits import EntitlementLimits
 
-class User(BaseModel):
+class UserOrganization(BaseModel):
     id: StrictInt = ...
-    username: StrictStr = ...
     name: StrictStr = ...
-    email: StrictStr = ...
-    photo: Optional[StrictStr] = None
-    created: datetime = ...
-    last_seen: Optional[datetime] = Field(None, alias="lastSeen")
-    staff_info: StaffInfo = Field(..., alias="staffInfo")
-    pending: StrictBool = ...
-    last_tos_acceptance_date: Optional[datetime] = Field(None, alias="lastTosAcceptanceDate")
-    job_title: Optional[StrictStr] = Field(None, alias="jobTitle")
-    permissions: Optional[List[Permission]] = Field(None, description="List of permissions the user has")
-    company_name: Optional[StrictStr] = Field(None, alias="companyName")
-    activated: StrictBool = Field(..., description="Whether the user has activated their account or not.")
-    mfa_configured: StrictBool = Field(..., alias="mfaConfigured", description="Whether the user has configured multi-factor authentication")
-    __properties = ["id", "username", "name", "email", "photo", "created", "lastSeen", "staffInfo", "pending", "lastTosAcceptanceDate", "jobTitle", "permissions", "companyName", "activated", "mfaConfigured"]
+    logo: Optional[StrictStr] = None
+    is_developer_profile: StrictBool = Field(..., alias="isDeveloperProfile")
+    whitelabel_id: Optional[StrictInt] = Field(..., alias="whitelabelId", description="Unique identifier of the white label this project belongs to, if any.")
+    is_admin: StrictBool = Field(..., alias="isAdmin", description="Whether the user is admin of this organization or not.")
+    created: datetime = Field(..., description="When the organization was created.")
+    trial_id: Optional[float] = Field(..., alias="trialId", description="Unique identifier of the trial this organization belongs to, if any.")
+    trial_expired_date: Optional[datetime] = Field(..., alias="trialExpiredDate", description="Date when the trial expired, if any. A expired trial has a grace period of 30 days before it's associated organization is deleted.")
+    trial_upgraded_date: Optional[datetime] = Field(..., alias="trialUpgradedDate", description="Date when the trial was upgraded to a full enterprise account, if any.")
+    entitlement_limits: EntitlementLimits = Field(..., alias="entitlementLimits")
+    __properties = ["id", "name", "logo", "isDeveloperProfile", "whitelabelId", "isAdmin", "created", "trialId", "trialExpiredDate", "trialUpgradedDate", "entitlementLimits"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> User:
-        """Create an instance of User from a JSON string"""
+    def from_json(cls, json_str: str) -> UserOrganization:
+        """Create an instance of UserOrganization from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
-        # override the default output from pydantic by calling `to_dict()` of staff_info
-        if self.staff_info:
-            _dict['staffInfo'] = self.staff_info.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of entitlement_limits
+        if self.entitlement_limits:
+            _dict['entitlementLimits'] = self.entitlement_limits.to_dict()
+        # set to None if whitelabel_id (nullable) is None
+        if self.whitelabel_id is None:
+            _dict['whitelabelId'] = None
+
+        # set to None if trial_id (nullable) is None
+        if self.trial_id is None:
+            _dict['trialId'] = None
+
+        # set to None if trial_expired_date (nullable) is None
+        if self.trial_expired_date is None:
+            _dict['trialExpiredDate'] = None
+
+        # set to None if trial_upgraded_date (nullable) is None
+        if self.trial_upgraded_date is None:
+            _dict['trialUpgradedDate'] = None
+
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> User:
-        """Create an instance of User from a dict"""
+    def from_dict(cls, obj: dict) -> UserOrganization:
+        """Create an instance of UserOrganization from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return User.construct(**obj)
+            return UserOrganization.construct(**obj)
 
-        _obj = User.construct(**{
+        _obj = UserOrganization.construct(**{
             "id": obj.get("id"),
-            "username": obj.get("username"),
             "name": obj.get("name"),
-            "email": obj.get("email"),
-            "photo": obj.get("photo"),
+            "logo": obj.get("logo"),
+            "is_developer_profile": obj.get("isDeveloperProfile"),
+            "whitelabel_id": obj.get("whitelabelId"),
+            "is_admin": obj.get("isAdmin"),
             "created": obj.get("created"),
-            "last_seen": obj.get("lastSeen"),
-            "staff_info": StaffInfo.from_dict(obj.get("staffInfo")) if obj.get("staffInfo") is not None else None,
-            "pending": obj.get("pending"),
-            "last_tos_acceptance_date": obj.get("lastTosAcceptanceDate"),
-            "job_title": obj.get("jobTitle"),
-            "permissions": obj.get("permissions"),
-            "company_name": obj.get("companyName"),
-            "activated": obj.get("activated"),
-            "mfa_configured": obj.get("mfaConfigured")
+            "trial_id": obj.get("trialId"),
+            "trial_expired_date": obj.get("trialExpiredDate"),
+            "trial_upgraded_date": obj.get("trialUpgradedDate"),
+            "entitlement_limits": EntitlementLimits.from_dict(obj.get("entitlementLimits")) if obj.get("entitlementLimits") is not None else None
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/user_by_third_party_activation_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/user_by_third_party_activation_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/user_delete_totp_mfa_key_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/user_delete_totp_mfa_key_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/user_dismiss_notification_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/user_dismiss_notification_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/user_experiment.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/user_experiment.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/user_generate_new_mfa_key_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/user_generate_new_mfa_key_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/user_generate_new_mfa_key_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/user_generate_new_mfa_key_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/user_set_totp_mfa_key_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/user_set_totp_mfa_key_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/user_set_totp_mfa_key_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/user_set_totp_mfa_key_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/user_set_totp_mfa_key_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/user_set_totp_mfa_key_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/user_tier_enum.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/user_tier_enum.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/verify_dsp_block_url_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/verify_dsp_block_url_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/verify_dsp_block_url_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/verify_dsp_block_url_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/verify_dsp_block_url_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/verify_dsp_block_url_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/verify_dsp_block_url_response_all_of_block.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/verify_dsp_block_url_response_all_of_block.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,24 +13,26 @@
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
-
+from typing import List, Optional
 from pydantic import BaseModel, Field, StrictInt, StrictStr
+from edgeimpulse_api.models.dsp_named_axis import DSPNamedAxis
 
 class VerifyDspBlockUrlResponseAllOfBlock(BaseModel):
     title: StrictStr = ...
     author: StrictStr = ...
     description: StrictStr = ...
     name: StrictStr = ...
     latest_implementation_version: StrictInt = Field(..., alias="latestImplementationVersion")
-    __properties = ["title", "author", "description", "name", "latestImplementationVersion"]
+    named_axes: Optional[List[DSPNamedAxis]] = Field(None, alias="namedAxes")
+    __properties = ["title", "author", "description", "name", "latestImplementationVersion", "namedAxes"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
@@ -47,14 +49,21 @@
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
+        # override the default output from pydantic by calling `to_dict()` of each item in named_axes (list)
+        _items = []
+        if self.named_axes:
+            for _item in self.named_axes:
+                if _item:
+                    _items.append(_item.to_dict())
+            _dict['namedAxes'] = _items
         return _dict
 
     @classmethod
     def from_dict(cls, obj: dict) -> VerifyDspBlockUrlResponseAllOfBlock:
         """Create an instance of VerifyDspBlockUrlResponseAllOfBlock from a dict"""
         if obj is None:
             return None
@@ -63,11 +72,12 @@
             return VerifyDspBlockUrlResponseAllOfBlock.construct(**obj)
 
         _obj = VerifyDspBlockUrlResponseAllOfBlock.construct(**{
             "title": obj.get("title"),
             "author": obj.get("author"),
             "description": obj.get("description"),
             "name": obj.get("name"),
-            "latest_implementation_version": obj.get("latestImplementationVersion")
+            "latest_implementation_version": obj.get("latestImplementationVersion"),
+            "named_axes": [DSPNamedAxis.from_dict(_item) for _item in obj.get("namedAxes")] if obj.get("namedAxes") is not None else None
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/verify_email_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/verify_email_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/verify_email_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/verify_email_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/verify_organization_bucket_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/verify_organization_bucket_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/verify_organization_bucket_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/verify_organization_bucket_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/verify_organization_bucket_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/verify_organization_bucket_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/verify_organization_bucket_response_all_of_files.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/verify_organization_bucket_response_all_of_files.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/verify_organization_existing_bucket_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/verify_organization_existing_bucket_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/verify_reset_password_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/verify_reset_password_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/whitelabel.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/whitelabel.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/whitelabel_admin_create_organization_request.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/whitelabel_admin_create_organization_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/whitelabel_all_learning_blocks_inner.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/whitelabel_all_learning_blocks_inner.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/whitelabel_custom_deployment_blocks_inner.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/whitelabel_custom_deployment_blocks_inner.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/window_settings_response.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/window_settings_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/window_settings_response_all_of.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/window_settings_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/models/window_settings_response_all_of_window_settings.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/models/window_settings_response_all_of_window_settings.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/edgeimpulse_api/rest.py` & `edgeimpulse_api-1.49.6/edgeimpulse_api/rest.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.5/pyproject.toml` & `edgeimpulse_api-1.49.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "edgeimpulse-api"
-version = "1.49.5" #DO_NOT_CHANGE_REPLACED_BY_BUILD_SCRIPT
+version = "1.49.6" #DO_NOT_CHANGE_REPLACED_BY_BUILD_SCRIPT
 description = "Python bindings for the Edge Impulse API."
 authors = ["EdgeImpulse Inc. <hello@edgeimpulse.com>"]
 license = "Apache-2.0"
 homepage = "https://edgeimpulse.com"
 documentation = "https://docs.edgeimpulse.com/reference/edge-impulse-api/edge-impulse-api"
 classifiers = [
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
```

### Comparing `edgeimpulse_api-1.49.5/PKG-INFO` & `edgeimpulse_api-1.49.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edgeimpulse-api
-Version: 1.49.5
+Version: 1.49.6
 Summary: Python bindings for the Edge Impulse API.
 Home-page: https://edgeimpulse.com
 License: Apache-2.0
 Author: EdgeImpulse Inc.
 Author-email: hello@edgeimpulse.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

