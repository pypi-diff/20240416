# Comparing `tmp/pydcapi-0.1.4.tar.gz` & `tmp/pydcapi-0.1.5.tar.gz`

## Comparing `pydcapi-0.1.4.tar` & `pydcapi-0.1.5.tar`

### file list

```diff
@@ -1,93 +1,93 @@
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 pydcapi-0.1.4/src/pydcapi/__init__.py
--rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 pydcapi-0.1.4/src/pydcapi/client.py
--rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 pydcapi-0.1.4/src/pydcapi/credentials.py
--rw-r--r--   0        0        0     7123 2020-02-02 00:00:00.000000 pydcapi-0.1.4/src/pydcapi/transports.py
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 pydcapi-0.1.4/src/pydcapi/models/asset_block_upload_extend_parameters_v1/__init__.py
--rw-r--r--   0        0        0     2061 2020-02-02 00:00:00.000000 pydcapi-0.1.4/src/pydcapi/models/asset_block_upload_extend_v1/__init__.py
--rw-r--r--   0        0        0     2782 2020-02-02 00:00:00.000000 pydcapi-0.1.4/src/pydcapi/models/asset_block_upload_finalize_parameters_v1/__init__.py
--rw-r--r--   0        0        0     2138 2020-02-02 00:00:00.000000 pydcapi-0.1.4/src/pydcapi/models/asset_block_upload_finalize_v1/__init__.py
--rw-r--r--   0        0        0     2292 2020-02-02 00:00:00.000000 pydcapi-0.1.4/src/pydcapi/models/asset_block_upload_initialize_parameters_v1/__init__.py
--rw-r--r--   0        0        0     2230 2020-02-02 00:00:00.000000 pydcapi-0.1.4/src/pydcapi/models/asset_block_upload_initialize_v1/__init__.py
--rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 pydcapi-0.1.4/src/pydcapi/models/asset_document_rendition_status_v1/__init__.py
--rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 pydcapi-0.1.4/src/pydcapi/models/asset_export_v1/__init__.py
--rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 pydcapi-0.1.4/src/pydcapi/models/asset_import_v1/__init__.py
--rw-r--r--   0        0        0     2926 2020-02-02 00:00:00.000000 pydcapi-0.1.4/src/pydcapi/models/asset_metadata_basic_v1/__init__.py
--rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 pydcapi-0.1.4/src/pydcapi/models/asset_metadata_field_patch_v1/__init__.py
--rw-r--r--   0        0        0     3028 2020-02-02 00:00:00.000000 pydcapi-0.1.4/src/pydcapi/models/asset_metadata_field_v1/__init__.py
--rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 pydcapi-0.1.4/src/pydcapi/models/asset_tag_sensei_contentanalyzer_v1/__init__.py
--rw-r--r--   0        0        0     2742 2020-02-02 00:00:00.000000 pydcapi-0.1.4/src/pydcapi/models/asset_tag_sensei_v1/__init__.py
--rw-r--r--   0        0        0     2095 2020-02-02 00:00:00.000000 pydcapi-0.1.4/src/pydcapi/models/asset_upload_parameters_v1/__init__.py
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 pydcapi-0.1.4/src/pydcapi/models/asset_uri_download_v1/__init__.py
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 pydcapi-0.1.4/src/pydcapi/models/asset_uri_rendition_v1/__init__.py
--rw-r--r--   0        0        0     1187 2020-02-02 00:00:00.000000 pydcapi-0.1.4/src/pydcapi/models/asset_v1/__init__.py
--rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 pydcapi-0.1.4/src/pydcapi/models/authorize_client_verb_v1/__init__.py
--rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 pydcapi-0.1.4/src/pydcapi/models/compute_content_bboxes_parameters_v1/__init__.py
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 pydcapi-0.1.4/src/pydcapi/models/connector_delete_response_v1/__init__.py
--rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 pydcapi-0.1.4/src/pydcapi/models/connector_info_v1/__init__.py
--rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 pydcapi-0.1.4/src/pydcapi/models/connector_link_parameters_v1/__init__.py
--rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 pydcapi-0.1.4/src/pydcapi/models/connector_listing_v1/__init__.py
--rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 pydcapi-0.1.4/src/pydcapi/models/copy_op_params_v1/__init__.py
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 pydcapi-0.1.4/src/pydcapi/models/copy_to_user_parameters_v1/__init__.py
--rw-r--r--   0        0        0     5627 2020-02-02 00:00:00.000000 pydcapi-0.1.4/src/pydcapi/models/createpdf_from_html_parameters_v1/__init__.py
--rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 pydcapi-0.1.4/src/pydcapi/models/createpdf_options_v1/__init__.py
--rw-r--r--   0        0        0     3843 2020-02-02 00:00:00.000000 pydcapi-0.1.4/src/pydcapi/models/createpdf_parameters_v1/__init__.py
--rw-r--r--   0        0        0     3999 2020-02-02 00:00:00.000000 pydcapi-0.1.4/src/pydcapi/models/discovery_v1/__init__.py
--rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 pydcapi-0.1.4/src/pydcapi/models/exportpdf_options_v1/__init__.py
--rw-r--r--   0        0        0     4187 2020-02-02 00:00:00.000000 pydcapi-0.1.4/src/pydcapi/models/exportpdf_parameters_v1/__init__.py
--rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 pydcapi-0.1.4/src/pydcapi/models/feedback_creation_v1/__init__.py
--rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 pydcapi-0.1.4/src/pydcapi/models/folder_breadcrumbs_v1/__init__.py
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 pydcapi-0.1.4/src/pydcapi/models/folder_creation_v1/__init__.py
--rw-r--r--   0        0        0     5435 2020-02-02 00:00:00.000000 pydcapi-0.1.4/src/pydcapi/models/folder_listing_v1/__init__.py
--rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 pydcapi-0.1.4/src/pydcapi/models/folder_metadata_basic_v1/__init__.py
--rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 pydcapi-0.1.4/src/pydcapi/models/folder_metadata_field_patch_v1/__init__.py
--rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 pydcapi-0.1.4/src/pydcapi/models/folder_metadata_field_v1/__init__.py
--rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 pydcapi-0.1.4/src/pydcapi/models/folder_v1/__init__.py
--rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 pydcapi-0.1.4/src/pydcapi/models/move_op_params_v1/__init__.py
--rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 pydcapi-0.1.4/src/pydcapi/models/move_op_result_v1/__init__.py
--rw-r--r--   0        0        0     2428 2020-02-02 00:00:00.000000 pydcapi-0.1.4/src/pydcapi/models/multiple_move_op_result_v1/__init__.py
--rw-r--r--   0        0        0     8135 2020-02-02 00:00:00.000000 pydcapi-0.1.4/src/pydcapi/models/new_asset_job_v1/__init__.py
--rw-r--r--   0        0        0    11142 2020-02-02 00:00:00.000000 pydcapi-0.1.4/src/pydcapi/models/pdf_actions_parameters_v1/__init__.py
--rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 pydcapi-0.1.4/src/pydcapi/models/recent_search_v1/__init__.py
--rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 pydcapi-0.1.4/src/pydcapi/models/recent_searches_v1/__init__.py
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 pydcapi-0.1.4/src/pydcapi/models/root_v1/__init__.py
--rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 pydcapi-0.1.4/src/pydcapi/models/services_v1/__init__.py
--rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 pydcapi-0.1.4/src/pydcapi/models/source_options_v1/__init__.py
--rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 pydcapi-0.1.4/src/pydcapi/models/splitpdf_parameters_v1/__init__.py
--rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 pydcapi-0.1.4/src/pydcapi/models/system_folders_v1/__init__.py
--rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 pydcapi-0.1.4/src/pydcapi/models/system_log_parameters_v1/__init__.py
--rw-r--r--   0        0        0     2349 2020-02-02 00:00:00.000000 pydcapi-0.1.4/src/pydcapi/models/upload_status_v1/__init__.py
--rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 pydcapi-0.1.4/src/pydcapi/models/user_cohorts_v1/__init__.py
--rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 pydcapi-0.1.4/src/pydcapi/models/user_identity_v1/__init__.py
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 pydcapi-0.1.4/src/pydcapi/models/user_limits_acrobat_v1/__init__.py
--rw-r--r--   0        0        0     5941 2020-02-02 00:00:00.000000 pydcapi-0.1.4/src/pydcapi/models/user_limits_conversions_v1/__init__.py
--rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 pydcapi-0.1.4/src/pydcapi/models/user_limits_esign_v1/__init__.py
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 pydcapi-0.1.4/src/pydcapi/models/user_limits_fillsign_v1/__init__.py
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 pydcapi-0.1.4/src/pydcapi/models/user_limits_pdf_services_v1/__init__.py
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 pydcapi-0.1.4/src/pydcapi/models/user_limits_review_v1/__init__.py
--rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 pydcapi-0.1.4/src/pydcapi/models/user_limits_send_v1/__init__.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 pydcapi-0.1.4/src/pydcapi/models/user_limits_storage_document_cloud_v1/__init__.py
--rw-r--r--   0        0        0    54986 2020-02-02 00:00:00.000000 pydcapi-0.1.4/src/pydcapi/models/user_limits_verbs_v1/__init__.py
--rw-r--r--   0        0        0     3425 2020-02-02 00:00:00.000000 pydcapi-0.1.4/src/pydcapi/models/user_prefs_v1/__init__.py
--rw-r--r--   0        0        0     1287 2020-02-02 00:00:00.000000 pydcapi-0.1.4/src/pydcapi/models/user_put_identity_v1/__init__.py
--rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 pydcapi-0.1.4/src/pydcapi/models/user_storage_document_cloud_v1/__init__.py
--rw-r--r--   0        0        0     1996 2020-02-02 00:00:00.000000 pydcapi-0.1.4/src/pydcapi/models/user_subscriptions_v1/__init__.py
--rw-r--r--   0        0        0     2661 2020-02-02 00:00:00.000000 pydcapi-0.1.4/src/pydcapi/models/user_upsell_v1/__init__.py
--rw-r--r--   0        0        0    74991 2020-02-02 00:00:00.000000 pydcapi-0.1.4/src/pydcapi/models/user_v1/__init__.py
--rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 pydcapi-0.1.4/src/pydcapi/models/zip_download_params_v1/__init__.py
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 pydcapi-0.1.4/src/pydcapi/models/zip_download_uri_v1/__init__.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 pydcapi-0.1.4/src/pydcapi/resources/__init__.py
--rw-r--r--   0        0        0    29085 2020-02-02 00:00:00.000000 pydcapi-0.1.4/src/pydcapi/resources/assets.py
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 pydcapi-0.1.4/src/pydcapi/resources/client.py
--rw-r--r--   0        0        0     3375 2020-02-02 00:00:00.000000 pydcapi-0.1.4/src/pydcapi/resources/connector.py
--rw-r--r--   0        0        0     4064 2020-02-02 00:00:00.000000 pydcapi-0.1.4/src/pydcapi/resources/discovery.py
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 pydcapi-0.1.4/src/pydcapi/resources/feedback.py
--rw-r--r--   0        0        0     9581 2020-02-02 00:00:00.000000 pydcapi-0.1.4/src/pydcapi/resources/folders.py
--rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 pydcapi-0.1.4/src/pydcapi/resources/jobs.py
--rw-r--r--   0        0        0     3095 2020-02-02 00:00:00.000000 pydcapi-0.1.4/src/pydcapi/resources/operations.py
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 pydcapi-0.1.4/src/pydcapi/resources/system.py
--rw-r--r--   0        0        0    19028 2020-02-02 00:00:00.000000 pydcapi-0.1.4/src/pydcapi/resources/users.py
--rw-r--r--   0        0        0     4116 2020-02-02 00:00:00.000000 pydcapi-0.1.4/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 pydcapi-0.1.4/LICENSE
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 pydcapi-0.1.4/README.md
--rw-r--r--   0        0        0     1490 2020-02-02 00:00:00.000000 pydcapi-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 pydcapi-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 pydcapi-0.1.5/src/pydcapi/__init__.py
+-rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 pydcapi-0.1.5/src/pydcapi/client.py
+-rw-r--r--   0        0        0     2205 2020-02-02 00:00:00.000000 pydcapi-0.1.5/src/pydcapi/credentials.py
+-rw-r--r--   0        0        0     7123 2020-02-02 00:00:00.000000 pydcapi-0.1.5/src/pydcapi/transports.py
+-rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 pydcapi-0.1.5/src/pydcapi/models/asset_block_upload_extend_parameters_v1/__init__.py
+-rw-r--r--   0        0        0     2061 2020-02-02 00:00:00.000000 pydcapi-0.1.5/src/pydcapi/models/asset_block_upload_extend_v1/__init__.py
+-rw-r--r--   0        0        0     2782 2020-02-02 00:00:00.000000 pydcapi-0.1.5/src/pydcapi/models/asset_block_upload_finalize_parameters_v1/__init__.py
+-rw-r--r--   0        0        0     2138 2020-02-02 00:00:00.000000 pydcapi-0.1.5/src/pydcapi/models/asset_block_upload_finalize_v1/__init__.py
+-rw-r--r--   0        0        0     2292 2020-02-02 00:00:00.000000 pydcapi-0.1.5/src/pydcapi/models/asset_block_upload_initialize_parameters_v1/__init__.py
+-rw-r--r--   0        0        0     2230 2020-02-02 00:00:00.000000 pydcapi-0.1.5/src/pydcapi/models/asset_block_upload_initialize_v1/__init__.py
+-rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 pydcapi-0.1.5/src/pydcapi/models/asset_document_rendition_status_v1/__init__.py
+-rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 pydcapi-0.1.5/src/pydcapi/models/asset_export_v1/__init__.py
+-rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 pydcapi-0.1.5/src/pydcapi/models/asset_import_v1/__init__.py
+-rw-r--r--   0        0        0     2926 2020-02-02 00:00:00.000000 pydcapi-0.1.5/src/pydcapi/models/asset_metadata_basic_v1/__init__.py
+-rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 pydcapi-0.1.5/src/pydcapi/models/asset_metadata_field_patch_v1/__init__.py
+-rw-r--r--   0        0        0     3028 2020-02-02 00:00:00.000000 pydcapi-0.1.5/src/pydcapi/models/asset_metadata_field_v1/__init__.py
+-rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 pydcapi-0.1.5/src/pydcapi/models/asset_tag_sensei_contentanalyzer_v1/__init__.py
+-rw-r--r--   0        0        0     2742 2020-02-02 00:00:00.000000 pydcapi-0.1.5/src/pydcapi/models/asset_tag_sensei_v1/__init__.py
+-rw-r--r--   0        0        0     2095 2020-02-02 00:00:00.000000 pydcapi-0.1.5/src/pydcapi/models/asset_upload_parameters_v1/__init__.py
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 pydcapi-0.1.5/src/pydcapi/models/asset_uri_download_v1/__init__.py
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 pydcapi-0.1.5/src/pydcapi/models/asset_uri_rendition_v1/__init__.py
+-rw-r--r--   0        0        0     1187 2020-02-02 00:00:00.000000 pydcapi-0.1.5/src/pydcapi/models/asset_v1/__init__.py
+-rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 pydcapi-0.1.5/src/pydcapi/models/authorize_client_verb_v1/__init__.py
+-rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 pydcapi-0.1.5/src/pydcapi/models/compute_content_bboxes_parameters_v1/__init__.py
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 pydcapi-0.1.5/src/pydcapi/models/connector_delete_response_v1/__init__.py
+-rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 pydcapi-0.1.5/src/pydcapi/models/connector_info_v1/__init__.py
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 pydcapi-0.1.5/src/pydcapi/models/connector_link_parameters_v1/__init__.py
+-rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 pydcapi-0.1.5/src/pydcapi/models/connector_listing_v1/__init__.py
+-rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 pydcapi-0.1.5/src/pydcapi/models/copy_op_params_v1/__init__.py
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 pydcapi-0.1.5/src/pydcapi/models/copy_to_user_parameters_v1/__init__.py
+-rw-r--r--   0        0        0     5627 2020-02-02 00:00:00.000000 pydcapi-0.1.5/src/pydcapi/models/createpdf_from_html_parameters_v1/__init__.py
+-rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 pydcapi-0.1.5/src/pydcapi/models/createpdf_options_v1/__init__.py
+-rw-r--r--   0        0        0     3843 2020-02-02 00:00:00.000000 pydcapi-0.1.5/src/pydcapi/models/createpdf_parameters_v1/__init__.py
+-rw-r--r--   0        0        0     3999 2020-02-02 00:00:00.000000 pydcapi-0.1.5/src/pydcapi/models/discovery_v1/__init__.py
+-rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 pydcapi-0.1.5/src/pydcapi/models/exportpdf_options_v1/__init__.py
+-rw-r--r--   0        0        0     4187 2020-02-02 00:00:00.000000 pydcapi-0.1.5/src/pydcapi/models/exportpdf_parameters_v1/__init__.py
+-rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 pydcapi-0.1.5/src/pydcapi/models/feedback_creation_v1/__init__.py
+-rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 pydcapi-0.1.5/src/pydcapi/models/folder_breadcrumbs_v1/__init__.py
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 pydcapi-0.1.5/src/pydcapi/models/folder_creation_v1/__init__.py
+-rw-r--r--   0        0        0     5435 2020-02-02 00:00:00.000000 pydcapi-0.1.5/src/pydcapi/models/folder_listing_v1/__init__.py
+-rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 pydcapi-0.1.5/src/pydcapi/models/folder_metadata_basic_v1/__init__.py
+-rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 pydcapi-0.1.5/src/pydcapi/models/folder_metadata_field_patch_v1/__init__.py
+-rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 pydcapi-0.1.5/src/pydcapi/models/folder_metadata_field_v1/__init__.py
+-rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 pydcapi-0.1.5/src/pydcapi/models/folder_v1/__init__.py
+-rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 pydcapi-0.1.5/src/pydcapi/models/move_op_params_v1/__init__.py
+-rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 pydcapi-0.1.5/src/pydcapi/models/move_op_result_v1/__init__.py
+-rw-r--r--   0        0        0     2428 2020-02-02 00:00:00.000000 pydcapi-0.1.5/src/pydcapi/models/multiple_move_op_result_v1/__init__.py
+-rw-r--r--   0        0        0     8135 2020-02-02 00:00:00.000000 pydcapi-0.1.5/src/pydcapi/models/new_asset_job_v1/__init__.py
+-rw-r--r--   0        0        0    11142 2020-02-02 00:00:00.000000 pydcapi-0.1.5/src/pydcapi/models/pdf_actions_parameters_v1/__init__.py
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 pydcapi-0.1.5/src/pydcapi/models/recent_search_v1/__init__.py
+-rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 pydcapi-0.1.5/src/pydcapi/models/recent_searches_v1/__init__.py
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 pydcapi-0.1.5/src/pydcapi/models/root_v1/__init__.py
+-rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 pydcapi-0.1.5/src/pydcapi/models/services_v1/__init__.py
+-rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 pydcapi-0.1.5/src/pydcapi/models/source_options_v1/__init__.py
+-rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 pydcapi-0.1.5/src/pydcapi/models/splitpdf_parameters_v1/__init__.py
+-rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 pydcapi-0.1.5/src/pydcapi/models/system_folders_v1/__init__.py
+-rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 pydcapi-0.1.5/src/pydcapi/models/system_log_parameters_v1/__init__.py
+-rw-r--r--   0        0        0     2349 2020-02-02 00:00:00.000000 pydcapi-0.1.5/src/pydcapi/models/upload_status_v1/__init__.py
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 pydcapi-0.1.5/src/pydcapi/models/user_cohorts_v1/__init__.py
+-rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 pydcapi-0.1.5/src/pydcapi/models/user_identity_v1/__init__.py
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 pydcapi-0.1.5/src/pydcapi/models/user_limits_acrobat_v1/__init__.py
+-rw-r--r--   0        0        0     5941 2020-02-02 00:00:00.000000 pydcapi-0.1.5/src/pydcapi/models/user_limits_conversions_v1/__init__.py
+-rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 pydcapi-0.1.5/src/pydcapi/models/user_limits_esign_v1/__init__.py
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 pydcapi-0.1.5/src/pydcapi/models/user_limits_fillsign_v1/__init__.py
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 pydcapi-0.1.5/src/pydcapi/models/user_limits_pdf_services_v1/__init__.py
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 pydcapi-0.1.5/src/pydcapi/models/user_limits_review_v1/__init__.py
+-rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 pydcapi-0.1.5/src/pydcapi/models/user_limits_send_v1/__init__.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 pydcapi-0.1.5/src/pydcapi/models/user_limits_storage_document_cloud_v1/__init__.py
+-rw-r--r--   0        0        0    54986 2020-02-02 00:00:00.000000 pydcapi-0.1.5/src/pydcapi/models/user_limits_verbs_v1/__init__.py
+-rw-r--r--   0        0        0     3425 2020-02-02 00:00:00.000000 pydcapi-0.1.5/src/pydcapi/models/user_prefs_v1/__init__.py
+-rw-r--r--   0        0        0     1287 2020-02-02 00:00:00.000000 pydcapi-0.1.5/src/pydcapi/models/user_put_identity_v1/__init__.py
+-rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 pydcapi-0.1.5/src/pydcapi/models/user_storage_document_cloud_v1/__init__.py
+-rw-r--r--   0        0        0     1996 2020-02-02 00:00:00.000000 pydcapi-0.1.5/src/pydcapi/models/user_subscriptions_v1/__init__.py
+-rw-r--r--   0        0        0     2661 2020-02-02 00:00:00.000000 pydcapi-0.1.5/src/pydcapi/models/user_upsell_v1/__init__.py
+-rw-r--r--   0        0        0    74991 2020-02-02 00:00:00.000000 pydcapi-0.1.5/src/pydcapi/models/user_v1/__init__.py
+-rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 pydcapi-0.1.5/src/pydcapi/models/zip_download_params_v1/__init__.py
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 pydcapi-0.1.5/src/pydcapi/models/zip_download_uri_v1/__init__.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 pydcapi-0.1.5/src/pydcapi/resources/__init__.py
+-rw-r--r--   0        0        0    29123 2020-02-02 00:00:00.000000 pydcapi-0.1.5/src/pydcapi/resources/assets.py
+-rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 pydcapi-0.1.5/src/pydcapi/resources/client.py
+-rw-r--r--   0        0        0     3380 2020-02-02 00:00:00.000000 pydcapi-0.1.5/src/pydcapi/resources/connector.py
+-rw-r--r--   0        0        0     4092 2020-02-02 00:00:00.000000 pydcapi-0.1.5/src/pydcapi/resources/discovery.py
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 pydcapi-0.1.5/src/pydcapi/resources/feedback.py
+-rw-r--r--   0        0        0     9586 2020-02-02 00:00:00.000000 pydcapi-0.1.5/src/pydcapi/resources/folders.py
+-rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 pydcapi-0.1.5/src/pydcapi/resources/jobs.py
+-rw-r--r--   0        0        0     3193 2020-02-02 00:00:00.000000 pydcapi-0.1.5/src/pydcapi/resources/operations.py
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 pydcapi-0.1.5/src/pydcapi/resources/system.py
+-rw-r--r--   0        0        0    19021 2020-02-02 00:00:00.000000 pydcapi-0.1.5/src/pydcapi/resources/users.py
+-rw-r--r--   0        0        0     4116 2020-02-02 00:00:00.000000 pydcapi-0.1.5/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 pydcapi-0.1.5/LICENSE
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 pydcapi-0.1.5/README.md
+-rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 pydcapi-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 pydcapi-0.1.5/PKG-INFO
```

### Comparing `pydcapi-0.1.4/src/pydcapi/client.py` & `pydcapi-0.1.5/src/pydcapi/client.py`

 * *Files identical despite different names*

### Comparing `pydcapi-0.1.4/src/pydcapi/credentials.py` & `pydcapi-0.1.5/src/pydcapi/credentials.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,20 +10,18 @@
     aux_sid: Optional[str]
     token: Optional[str]
     expiry: Optional[int]
 
 
 class CredentialsProvider(Protocol):
     @abc.abstractmethod
-    def get(self) -> Credentials:
-        ...
+    def get(self) -> Credentials: ...
 
     @abc.abstractmethod
-    def set(self, credentials: Credentials) -> None:
-        ...
+    def set(self, credentials: Credentials) -> None: ...
 
 
 class StaticCredentialsProvider:
     def __init__(self, credentials: Credentials) -> None:
         self.credentials = credentials
 
     def get(self) -> Credentials:
@@ -31,15 +29,15 @@
 
     def set(self, credentials: Credentials) -> None:
         self.credentials = credentials
 
 
 class EnvCredentialsProvider:
     def __init__(self, prefix: str = "") -> None:
-        self.credentials = {
+        self.credentials: Credentials = {
             "ims_sid": os.environ.get(f"{prefix}IMS_SID"),
             "aux_sid": os.environ.get(f"{prefix}AUX_SID"),
             "token": os.environ.get(f"{prefix}TOKEN"),
             "expiry": int(os.environ.get(f"{prefix}EXPIRY", 0)),
         }
 
     def get(self) -> Credentials:
@@ -52,15 +50,23 @@
 class JSONFileCredentialsProvider:
     def __init__(self, path: str):
         self.__path = path
 
     def get(self) -> Credentials:
         with open(self.__path, "r") as file:
             try:
-                return json.load(file)
+                data = json.load(file)
+                credentials: Credentials = {
+                    "ims_sid": str(data.get("ims_sid", "")) or None,
+                    "aux_sid": str(data.get("aux_sid", "")) or None,
+                    "token": str(data.get("token", "")) or None,
+                    "expiry": int(data.get("expiry", 0)) or None,
+                }
+                return credentials
+
             except json.JSONDecodeError:
                 return {}
 
     def set(self, credentials: Credentials) -> None:
         with open(self.__path, "w") as file:
             data = dict(credentials.copy())
             data["updated_at"] = datetime.datetime.now(tz=datetime.timezone.utc).isoformat()
```

### Comparing `pydcapi-0.1.4/src/pydcapi/transports.py` & `pydcapi-0.1.5/src/pydcapi/transports.py`

 * *Files identical despite different names*

### Comparing `pydcapi-0.1.4/src/pydcapi/models/asset_block_upload_extend_parameters_v1/__init__.py` & `pydcapi-0.1.5/src/pydcapi/models/asset_block_upload_extend_parameters_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `pydcapi-0.1.4/src/pydcapi/models/asset_block_upload_extend_v1/__init__.py` & `pydcapi-0.1.5/src/pydcapi/models/asset_block_upload_extend_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `pydcapi-0.1.4/src/pydcapi/models/asset_block_upload_finalize_parameters_v1/__init__.py` & `pydcapi-0.1.5/src/pydcapi/models/asset_block_upload_finalize_parameters_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `pydcapi-0.1.4/src/pydcapi/models/asset_block_upload_finalize_v1/__init__.py` & `pydcapi-0.1.5/src/pydcapi/models/asset_block_upload_finalize_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `pydcapi-0.1.4/src/pydcapi/models/asset_block_upload_initialize_parameters_v1/__init__.py` & `pydcapi-0.1.5/src/pydcapi/models/asset_block_upload_initialize_parameters_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `pydcapi-0.1.4/src/pydcapi/models/asset_block_upload_initialize_v1/__init__.py` & `pydcapi-0.1.5/src/pydcapi/models/asset_block_upload_initialize_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `pydcapi-0.1.4/src/pydcapi/models/asset_document_rendition_status_v1/__init__.py` & `pydcapi-0.1.5/src/pydcapi/models/asset_document_rendition_status_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `pydcapi-0.1.4/src/pydcapi/models/asset_export_v1/__init__.py` & `pydcapi-0.1.5/src/pydcapi/models/asset_export_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `pydcapi-0.1.4/src/pydcapi/models/asset_import_v1/__init__.py` & `pydcapi-0.1.5/src/pydcapi/models/asset_import_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `pydcapi-0.1.4/src/pydcapi/models/asset_metadata_basic_v1/__init__.py` & `pydcapi-0.1.5/src/pydcapi/models/asset_metadata_basic_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `pydcapi-0.1.4/src/pydcapi/models/asset_metadata_field_patch_v1/__init__.py` & `pydcapi-0.1.5/src/pydcapi/models/asset_metadata_field_patch_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `pydcapi-0.1.4/src/pydcapi/models/asset_metadata_field_v1/__init__.py` & `pydcapi-0.1.5/src/pydcapi/models/asset_metadata_field_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `pydcapi-0.1.4/src/pydcapi/models/asset_tag_sensei_contentanalyzer_v1/__init__.py` & `pydcapi-0.1.5/src/pydcapi/models/asset_tag_sensei_contentanalyzer_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `pydcapi-0.1.4/src/pydcapi/models/asset_tag_sensei_v1/__init__.py` & `pydcapi-0.1.5/src/pydcapi/models/asset_tag_sensei_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `pydcapi-0.1.4/src/pydcapi/models/asset_upload_parameters_v1/__init__.py` & `pydcapi-0.1.5/src/pydcapi/models/asset_upload_parameters_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `pydcapi-0.1.4/src/pydcapi/models/asset_v1/__init__.py` & `pydcapi-0.1.5/src/pydcapi/models/asset_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `pydcapi-0.1.4/src/pydcapi/models/authorize_client_verb_v1/__init__.py` & `pydcapi-0.1.5/src/pydcapi/models/authorize_client_verb_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `pydcapi-0.1.4/src/pydcapi/models/compute_content_bboxes_parameters_v1/__init__.py` & `pydcapi-0.1.5/src/pydcapi/models/compute_content_bboxes_parameters_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `pydcapi-0.1.4/src/pydcapi/models/connector_info_v1/__init__.py` & `pydcapi-0.1.5/src/pydcapi/models/connector_info_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `pydcapi-0.1.4/src/pydcapi/models/connector_link_parameters_v1/__init__.py` & `pydcapi-0.1.5/src/pydcapi/models/connector_link_parameters_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `pydcapi-0.1.4/src/pydcapi/models/connector_listing_v1/__init__.py` & `pydcapi-0.1.5/src/pydcapi/models/connector_listing_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `pydcapi-0.1.4/src/pydcapi/models/copy_op_params_v1/__init__.py` & `pydcapi-0.1.5/src/pydcapi/models/copy_op_params_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `pydcapi-0.1.4/src/pydcapi/models/copy_to_user_parameters_v1/__init__.py` & `pydcapi-0.1.5/src/pydcapi/models/copy_to_user_parameters_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `pydcapi-0.1.4/src/pydcapi/models/createpdf_from_html_parameters_v1/__init__.py` & `pydcapi-0.1.5/src/pydcapi/models/createpdf_from_html_parameters_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `pydcapi-0.1.4/src/pydcapi/models/createpdf_options_v1/__init__.py` & `pydcapi-0.1.5/src/pydcapi/models/createpdf_options_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `pydcapi-0.1.4/src/pydcapi/models/createpdf_parameters_v1/__init__.py` & `pydcapi-0.1.5/src/pydcapi/models/createpdf_parameters_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `pydcapi-0.1.4/src/pydcapi/models/discovery_v1/__init__.py` & `pydcapi-0.1.5/src/pydcapi/models/discovery_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `pydcapi-0.1.4/src/pydcapi/models/exportpdf_options_v1/__init__.py` & `pydcapi-0.1.5/src/pydcapi/models/exportpdf_options_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `pydcapi-0.1.4/src/pydcapi/models/exportpdf_parameters_v1/__init__.py` & `pydcapi-0.1.5/src/pydcapi/models/exportpdf_parameters_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `pydcapi-0.1.4/src/pydcapi/models/feedback_creation_v1/__init__.py` & `pydcapi-0.1.5/src/pydcapi/models/feedback_creation_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `pydcapi-0.1.4/src/pydcapi/models/folder_breadcrumbs_v1/__init__.py` & `pydcapi-0.1.5/src/pydcapi/models/folder_breadcrumbs_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `pydcapi-0.1.4/src/pydcapi/models/folder_creation_v1/__init__.py` & `pydcapi-0.1.5/src/pydcapi/models/folder_creation_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `pydcapi-0.1.4/src/pydcapi/models/folder_listing_v1/__init__.py` & `pydcapi-0.1.5/src/pydcapi/models/folder_listing_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `pydcapi-0.1.4/src/pydcapi/models/folder_metadata_basic_v1/__init__.py` & `pydcapi-0.1.5/src/pydcapi/models/folder_metadata_basic_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `pydcapi-0.1.4/src/pydcapi/models/folder_metadata_field_patch_v1/__init__.py` & `pydcapi-0.1.5/src/pydcapi/models/folder_metadata_field_patch_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `pydcapi-0.1.4/src/pydcapi/models/folder_metadata_field_v1/__init__.py` & `pydcapi-0.1.5/src/pydcapi/models/folder_metadata_field_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `pydcapi-0.1.4/src/pydcapi/models/folder_v1/__init__.py` & `pydcapi-0.1.5/src/pydcapi/models/folder_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `pydcapi-0.1.4/src/pydcapi/models/move_op_params_v1/__init__.py` & `pydcapi-0.1.5/src/pydcapi/models/move_op_params_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `pydcapi-0.1.4/src/pydcapi/models/move_op_result_v1/__init__.py` & `pydcapi-0.1.5/src/pydcapi/models/move_op_result_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `pydcapi-0.1.4/src/pydcapi/models/multiple_move_op_result_v1/__init__.py` & `pydcapi-0.1.5/src/pydcapi/models/multiple_move_op_result_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `pydcapi-0.1.4/src/pydcapi/models/new_asset_job_v1/__init__.py` & `pydcapi-0.1.5/src/pydcapi/models/new_asset_job_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `pydcapi-0.1.4/src/pydcapi/models/pdf_actions_parameters_v1/__init__.py` & `pydcapi-0.1.5/src/pydcapi/models/pdf_actions_parameters_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `pydcapi-0.1.4/src/pydcapi/models/recent_search_v1/__init__.py` & `pydcapi-0.1.5/src/pydcapi/models/recent_search_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `pydcapi-0.1.4/src/pydcapi/models/recent_searches_v1/__init__.py` & `pydcapi-0.1.5/src/pydcapi/models/recent_searches_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `pydcapi-0.1.4/src/pydcapi/models/services_v1/__init__.py` & `pydcapi-0.1.5/src/pydcapi/models/services_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `pydcapi-0.1.4/src/pydcapi/models/source_options_v1/__init__.py` & `pydcapi-0.1.5/src/pydcapi/models/source_options_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `pydcapi-0.1.4/src/pydcapi/models/splitpdf_parameters_v1/__init__.py` & `pydcapi-0.1.5/src/pydcapi/models/splitpdf_parameters_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `pydcapi-0.1.4/src/pydcapi/models/system_folders_v1/__init__.py` & `pydcapi-0.1.5/src/pydcapi/models/system_folders_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `pydcapi-0.1.4/src/pydcapi/models/system_log_parameters_v1/__init__.py` & `pydcapi-0.1.5/src/pydcapi/models/system_log_parameters_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `pydcapi-0.1.4/src/pydcapi/models/upload_status_v1/__init__.py` & `pydcapi-0.1.5/src/pydcapi/models/upload_status_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `pydcapi-0.1.4/src/pydcapi/models/user_identity_v1/__init__.py` & `pydcapi-0.1.5/src/pydcapi/models/user_identity_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `pydcapi-0.1.4/src/pydcapi/models/user_limits_conversions_v1/__init__.py` & `pydcapi-0.1.5/src/pydcapi/models/user_limits_conversions_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `pydcapi-0.1.4/src/pydcapi/models/user_limits_esign_v1/__init__.py` & `pydcapi-0.1.5/src/pydcapi/models/user_limits_esign_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `pydcapi-0.1.4/src/pydcapi/models/user_limits_fillsign_v1/__init__.py` & `pydcapi-0.1.5/src/pydcapi/models/user_limits_fillsign_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `pydcapi-0.1.4/src/pydcapi/models/user_limits_pdf_services_v1/__init__.py` & `pydcapi-0.1.5/src/pydcapi/models/user_limits_pdf_services_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `pydcapi-0.1.4/src/pydcapi/models/user_limits_review_v1/__init__.py` & `pydcapi-0.1.5/src/pydcapi/models/user_limits_review_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `pydcapi-0.1.4/src/pydcapi/models/user_limits_send_v1/__init__.py` & `pydcapi-0.1.5/src/pydcapi/models/user_limits_send_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `pydcapi-0.1.4/src/pydcapi/models/user_limits_storage_document_cloud_v1/__init__.py` & `pydcapi-0.1.5/src/pydcapi/models/user_limits_storage_document_cloud_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `pydcapi-0.1.4/src/pydcapi/models/user_limits_verbs_v1/__init__.py` & `pydcapi-0.1.5/src/pydcapi/models/user_limits_verbs_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `pydcapi-0.1.4/src/pydcapi/models/user_prefs_v1/__init__.py` & `pydcapi-0.1.5/src/pydcapi/models/user_prefs_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `pydcapi-0.1.4/src/pydcapi/models/user_put_identity_v1/__init__.py` & `pydcapi-0.1.5/src/pydcapi/models/user_put_identity_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `pydcapi-0.1.4/src/pydcapi/models/user_storage_document_cloud_v1/__init__.py` & `pydcapi-0.1.5/src/pydcapi/models/user_storage_document_cloud_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `pydcapi-0.1.4/src/pydcapi/models/user_subscriptions_v1/__init__.py` & `pydcapi-0.1.5/src/pydcapi/models/user_subscriptions_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `pydcapi-0.1.4/src/pydcapi/models/user_upsell_v1/__init__.py` & `pydcapi-0.1.5/src/pydcapi/models/user_upsell_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `pydcapi-0.1.4/src/pydcapi/models/user_v1/__init__.py` & `pydcapi-0.1.5/src/pydcapi/models/user_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `pydcapi-0.1.4/src/pydcapi/models/zip_download_params_v1/__init__.py` & `pydcapi-0.1.5/src/pydcapi/models/zip_download_params_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `pydcapi-0.1.4/src/pydcapi/resources/assets.py` & `pydcapi-0.1.5/src/pydcapi/resources/assets.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,64 +1,63 @@
 # generated by scripts/generate.py
 
 import re
-from typing import Any, Dict, IO, Literal, TYPE_CHECKING, Union
+from typing import IO, TYPE_CHECKING, Any, Dict, Literal, Union
 
 from .client import Client
 
 if TYPE_CHECKING:
     from ..models import (
-        asset_metadata_basic_v1,
+        asset_block_upload_extend_parameters_v1,
+        asset_block_upload_extend_v1,
         asset_block_upload_finalize_parameters_v1,
-        upload_status_v1,
-        zip_download_uri_v1,
-        asset_import_v1,
+        asset_block_upload_finalize_v1,
+        asset_block_upload_initialize_parameters_v1,
+        asset_block_upload_initialize_v1,
+        asset_document_rendition_status_v1,
         asset_export_v1,
-        asset_block_upload_extend_parameters_v1,
-        zip_download_params_v1,
+        asset_import_v1,
+        asset_metadata_basic_v1,
+        asset_metadata_field_patch_v1,
         asset_metadata_field_v1,
-        authorize_client_verb_v1,
-        pdf_actions_parameters_v1,
-        asset_block_upload_initialize_v1,
-        asset_uri_download_v1,
-        asset_block_upload_extend_v1,
-        splitpdf_parameters_v1,
         asset_tag_sensei_v1,
-        createpdf_parameters_v1,
-        asset_block_upload_finalize_v1,
+        asset_uri_download_v1,
         asset_uri_rendition_v1,
-        asset_metadata_field_patch_v1,
-        asset_document_rendition_status_v1,
-        new_asset_job_v1,
         asset_v1,
-        exportpdf_parameters_v1,
-        asset_block_upload_initialize_parameters_v1,
+        authorize_client_verb_v1,
         createpdf_from_html_parameters_v1,
+        createpdf_parameters_v1,
+        exportpdf_parameters_v1,
+        new_asset_job_v1,
+        pdf_actions_parameters_v1,
+        splitpdf_parameters_v1,
+        upload_status_v1,
+        zip_download_params_v1,
+        zip_download_uri_v1,
     )
 
-
 import uritemplate
 
 
 class Assets:
 
     def __init__(self, client: Client):
         self._client: Client = client
 
     def authorize_client_verb(self, *, _data: "authorize_client_verb_v1.Model") -> Any:
         url = "https://dc-api-v2.adobe.io/{expiry}/assets/authorize/client/verb"
         headers: Dict[str, str] = {}
         headers["Accept"] = "application/json"
+
         resp = self._client.request(
             "PUT",
             url,
             headers=headers,
-            json=_data.dict(),
+            json=_data.model_dump(),
         )
-
         content_type = resp.headers["Content-Type"]
 
         if re.search(r"application/json", content_type):
             return resp.json()
         else:
             raise ValueError(f"Unexpected content type: {content_type}")
 
@@ -69,21 +68,21 @@
             uri="{+asset_block_upload_extend_uri}",
             var_dict={
                 "asset_block_upload_extend_uri": asset_block_upload_extend_uri,
             },
         ).uri
         headers: Dict[str, str] = {}
         headers["Accept"] = 'application/vnd.adobe.dc+json; profile="https://dc-api.adobe.io/schemas/asset_block_upload_extend_v1.json"'
+
         resp = self._client.request(
             "PUT",
             url,
             headers=headers,
-            json=_data.dict(),
+            json=_data.model_dump(),
         )
-
         content_type = resp.headers["Content-Type"]
 
         if re.search(r"schemas/asset_block_upload_extend_v1\.json", content_type):
             return asset_block_upload_extend_v1.Model.model_validate(resp.json())
         else:
             raise ValueError(f"Unexpected content type: {content_type}")
 
@@ -94,81 +93,81 @@
             uri="{+asset_block_upload_finalize_uri}",
             var_dict={
                 "asset_block_upload_finalize_uri": asset_block_upload_finalize_uri,
             },
         ).uri
         headers: Dict[str, str] = {}
         headers["Accept"] = 'application/vnd.adobe.dc+json; profile="https://dc-api.adobe.io/schemas/asset_block_upload_finalize_v1.json"'
+
         resp = self._client.request(
             "PUT",
             url,
             headers=headers,
-            json=_data.dict(),
+            json=_data.model_dump(),
         )
-
         content_type = resp.headers["Content-Type"]
 
         if re.search(r"schemas/asset_block_upload_finalize_v1\.json", content_type):
             return asset_block_upload_finalize_v1.Model.model_validate(resp.json())
         else:
             raise ValueError(f"Unexpected content type: {content_type}")
 
     def block_upload_initialize(self, *, _data: "asset_block_upload_initialize_parameters_v1.Model") -> "asset_block_upload_initialize_v1.Model":
         from ..models import asset_block_upload_initialize_v1
 
         url = "https://dc-api-v2.adobe.io/{expiry}/assets/block_upload/initialize"
         headers: Dict[str, str] = {}
         headers["Accept"] = 'application/vnd.adobe.dc+json; profile="https://dc-api.adobe.io/schemas/asset_block_upload_initialize_v1.json"'
+
         resp = self._client.request(
             "POST",
             url,
             headers=headers,
-            json=_data.dict(),
+            json=_data.model_dump(),
         )
-
         content_type = resp.headers["Content-Type"]
 
         if re.search(r"schemas/asset_block_upload_initialize_v1\.json", content_type):
             return asset_block_upload_initialize_v1.Model.model_validate(resp.json())
         else:
             raise ValueError(f"Unexpected content type: {content_type}")
 
     def createpdf(self, *, _data: "createpdf_parameters_v1.Model") -> "new_asset_job_v1.Model":
         from ..models import new_asset_job_v1
 
         url = "https://dc-api-v2.adobe.io/{expiry}/assets?operation=createpdf"
         headers: Dict[str, str] = {}
         headers["Accept"] = 'application/vnd.adobe.dc+json; profile="https://dc-api.adobe.io/schemas/new_asset_job_v1.json"'
+
         resp = self._client.request(
             "POST",
             url,
             headers=headers,
-            json=_data.dict(),
+            json=_data.model_dump(),
         )
-
         content_type = resp.headers["Content-Type"]
 
         if re.search(r"schemas/new_asset_job_v1\.json", content_type):
             return new_asset_job_v1.Model.model_validate(resp.json())
         else:
             raise ValueError(f"Unexpected content type: {content_type}")
 
     def createpdf_from_html(self, *, _data: "createpdf_from_html_parameters_v1.Model") -> "new_asset_job_v1.Model":
         from ..models import new_asset_job_v1
 
         url = "https://dc-api-v2.adobe.io/{expiry}/assets?operation=createpdf_from_html"
         headers: Dict[str, str] = {}
         headers["Accept"] = 'application/vnd.adobe.dc+json; profile="https://dc-api.adobe.io/schemas/new_asset_job_v1.json"'
+
         resp = self._client.request(
             "POST",
             url,
             headers=headers,
-            json=_data.dict(),
+            json=_data.model_dump(),
         )
-
         content_type = resp.headers["Content-Type"]
 
         if re.search(r"schemas/new_asset_job_v1\.json", content_type):
             return new_asset_job_v1.Model.model_validate(resp.json())
         else:
             raise ValueError(f"Unexpected content type: {content_type}")
 
@@ -176,30 +175,32 @@
         url = uritemplate.partial(
             uri="{+asset_uri}",
             var_dict={
                 "asset_uri": asset_uri,
             },
         ).uri
         headers: Dict[str, str] = {}
-        resp = self._client.request(
+
+        self._client.request(
             "DELETE",
             url,
             headers=headers,
         )
 
     def delete_metadata_field(self, *, fields: Literal["last_access"], asset_uri: str) -> None:
         url = uritemplate.partial(
             uri="{+asset_uri}/metadata{/fields}",
             var_dict={
                 "fields": fields,
                 "asset_uri": asset_uri,
             },
         ).uri
         headers: Dict[str, str] = {}
-        resp = self._client.request(
+
+        self._client.request(
             "DELETE",
             url,
             headers=headers,
         )
 
     def document_rendition(self, *, format: Literal["ftpdf", "jcos", "owp"], asset_rendition_uri: str, fallback: Literal["original", "none"] = "original") -> Union[Any, bytes, str]:
         url = uritemplate.partial(
@@ -208,20 +209,20 @@
                 "format": format,
                 "asset_rendition_uri": asset_rendition_uri,
                 "fallback": fallback,
             },
         ).uri
         headers: Dict[str, str] = {}
         headers["Accept"] = "application/cbor; application/json; application/octet-stream; application/pdf; text/html; */*"
+
         resp = self._client.request(
             "GET",
             url,
             headers=headers,
         )
-
         content_type = resp.headers["Content-Type"]
 
         if re.search(r"application/cbor", content_type):
             return resp.content
         if re.search(r"application/json", content_type):
             return resp.json()
         if re.search(r"application/octet-stream", content_type):
@@ -242,20 +243,20 @@
             uri="{+asset_uri}/document/rendition/status",
             var_dict={
                 "asset_uri": asset_uri,
             },
         ).uri
         headers: Dict[str, str] = {}
         headers["Accept"] = 'application/vnd.adobe.dc+json; profile="https://dc-api.adobe.io/schemas/asset_document_rendition_status_v1.json"'
+
         resp = self._client.request(
             "GET",
             url,
             headers=headers,
         )
-
         content_type = resp.headers["Content-Type"]
 
         if re.search(r"schemas/asset_document_rendition_status_v1\.json", content_type):
             return asset_document_rendition_status_v1.Model.model_validate(resp.json())
         else:
             raise ValueError(f"Unexpected content type: {content_type}")
 
@@ -264,20 +265,20 @@
             uri="{+asset_download_uri}",
             var_dict={
                 "asset_download_uri": asset_download_uri,
             },
         ).uri
         headers: Dict[str, str] = {}
         headers["Accept"] = "*/*"
+
         resp = self._client.request(
             "GET",
             url,
             headers=headers,
         )
-
         content_type = resp.headers["Content-Type"]
 
         if re.search(r".*", content_type):
             return resp.content
         else:
             raise ValueError(f"Unexpected content type: {content_type}")
 
@@ -290,20 +291,20 @@
                 "make_ticket": make_ticket,
                 "asset_uri": asset_uri,
                 "make_direct_storage_uri": make_direct_storage_uri,
             },
         ).uri
         headers: Dict[str, str] = {}
         headers["Accept"] = 'application/vnd.adobe.dc+json; profile="https://dc-api.adobe.io/schemas/asset_uri_download_v1.json"'
+
         resp = self._client.request(
             "GET",
             url,
             headers=headers,
         )
-
         content_type = resp.headers["Content-Type"]
 
         if re.search(r"schemas/asset_uri_download_v1\.json", content_type):
             return asset_uri_download_v1.Model.model_validate(resp.json())
         else:
             raise ValueError(f"Unexpected content type: {content_type}")
 
@@ -314,41 +315,41 @@
             uri="{+export_uri}",
             var_dict={
                 "export_uri": export_uri,
             },
         ).uri
         headers: Dict[str, str] = {}
         headers["Accept"] = 'application/vnd.adobe.dc+json; profile="https://dc-api.adobe.io/schemas/new_asset_job_v1.json"'
+
         resp = self._client.request(
             "POST",
             url,
             headers=headers,
-            json=_data.dict(),
+            json=_data.model_dump(),
         )
-
         content_type = resp.headers["Content-Type"]
 
         if re.search(r"schemas/new_asset_job_v1\.json", content_type):
             return new_asset_job_v1.Model.model_validate(resp.json())
         else:
             raise ValueError(f"Unexpected content type: {content_type}")
 
     def exportpdf(self, *, _data: "exportpdf_parameters_v1.Model") -> "new_asset_job_v1.Model":
         from ..models import new_asset_job_v1
 
         url = "https://dc-api-v2.adobe.io/{expiry}/assets?operation=exportpdf"
         headers: Dict[str, str] = {}
         headers["Accept"] = 'application/vnd.adobe.dc+json; profile="https://dc-api.adobe.io/schemas/new_asset_job_v1.json"'
+
         resp = self._client.request(
             "POST",
             url,
             headers=headers,
-            json=_data.dict(),
+            json=_data.model_dump(),
         )
-
         content_type = resp.headers["Content-Type"]
 
         if re.search(r"schemas/new_asset_job_v1\.json", content_type):
             return new_asset_job_v1.Model.model_validate(resp.json())
         else:
             raise ValueError(f"Unexpected content type: {content_type}")
 
@@ -359,20 +360,20 @@
             uri="{+asset_uri}/metadata",
             var_dict={
                 "asset_uri": asset_uri,
             },
         ).uri
         headers: Dict[str, str] = {}
         headers["Accept"] = 'application/vnd.adobe.dc+json; profile="https://dc-api.adobe.io/schemas/asset_metadata_basic_v1.json"'
+
         resp = self._client.request(
             "GET",
             url,
             headers=headers,
         )
-
         content_type = resp.headers["Content-Type"]
 
         if re.search(r"schemas/asset_metadata_basic_v1\.json", content_type):
             return asset_metadata_basic_v1.Model.model_validate(resp.json())
         else:
             raise ValueError(f"Unexpected content type: {content_type}")
 
@@ -384,40 +385,40 @@
             var_dict={
                 "fields": fields,
                 "asset_uri": asset_uri,
             },
         ).uri
         headers: Dict[str, str] = {}
         headers["Accept"] = 'application/vnd.adobe.dc+json; profile="https://dc-api.adobe.io/schemas/asset_metadata_field_v1.json"'
+
         resp = self._client.request(
             "GET",
             url,
             headers=headers,
         )
-
         content_type = resp.headers["Content-Type"]
 
         if re.search(r"schemas/asset_metadata_field_v1\.json", content_type):
             return asset_metadata_field_v1.Model.model_validate(resp.json())
         else:
             raise ValueError(f"Unexpected content type: {content_type}")
 
     def import_(self, *, _data: "asset_import_v1.Model") -> "new_asset_job_v1.Model":
         from ..models import new_asset_job_v1
 
         url = "https://dc-api-v2.adobe.io/{expiry}/assets?operation=import"
         headers: Dict[str, str] = {}
         headers["Accept"] = 'application/vnd.adobe.dc+json; profile="https://dc-api.adobe.io/schemas/new_asset_job_v1.json"'
+
         resp = self._client.request(
             "POST",
             url,
             headers=headers,
-            json=_data.dict(),
+            json=_data.model_dump(),
         )
-
         content_type = resp.headers["Content-Type"]
 
         if re.search(r"schemas/new_asset_job_v1\.json", content_type):
             return new_asset_job_v1.Model.model_validate(resp.json())
         else:
             raise ValueError(f"Unexpected content type: {content_type}")
 
@@ -429,41 +430,41 @@
             var_dict={
                 "fields": fields,
                 "asset_uri": asset_uri,
             },
         ).uri
         headers: Dict[str, str] = {}
         headers["Accept"] = 'application/vnd.adobe.dc+json; profile="https://dc-api.adobe.io/schemas/asset_metadata_field_v1.json"'
+
         resp = self._client.request(
             "PATCH",
             url,
             headers=headers,
-            json=_data.dict(),
+            json=_data.model_dump(),
         )
-
         content_type = resp.headers["Content-Type"]
 
         if re.search(r"schemas/asset_metadata_field_v1\.json", content_type):
             return asset_metadata_field_v1.Model.model_validate(resp.json())
         else:
             raise ValueError(f"Unexpected content type: {content_type}")
 
     def pdf_actions(self, *, _data: "pdf_actions_parameters_v1.Model") -> "new_asset_job_v1.Model":
         from ..models import new_asset_job_v1
 
         url = "https://dc-api-v2.adobe.io/{expiry}/assets?operation=pdf_actions"
         headers: Dict[str, str] = {}
         headers["Accept"] = 'application/vnd.adobe.dc+json; profile="https://dc-api.adobe.io/schemas/new_asset_job_v1.json"'
+
         resp = self._client.request(
             "POST",
             url,
             headers=headers,
-            json=_data.dict(),
+            json=_data.model_dump(),
         )
-
         content_type = resp.headers["Content-Type"]
 
         if re.search(r"schemas/new_asset_job_v1\.json", content_type):
             return new_asset_job_v1.Model.model_validate(resp.json())
         else:
             raise ValueError(f"Unexpected content type: {content_type}")
 
@@ -472,22 +473,23 @@
             uri="{+asset_uri}/metadata{/fields}",
             var_dict={
                 "fields": fields,
                 "asset_uri": asset_uri,
             },
         ).uri
         headers: Dict[str, str] = {}
-        resp = self._client.request(
+
+        self._client.request(
             "PUT",
             url,
             headers=headers,
-            json=_data.dict(),
+            json=_data.model_dump(),
         )
 
-    def rendition(self, *, download: bool, format: Literal["png", "jpg"], page: int, rendition_class: str, size: str, asset_rendition_uri: str, markup: bool = True, processing_hint: Literal["speed_over_quality", "quality_over_speed"] = "speed_over_quality", wait: int = 10) -> Union[bytes]:
+    def rendition(self, *, download: bool, format: Literal["png", "jpg"], page: int, rendition_class: str, size: str, asset_rendition_uri: str, markup: bool = True, processing_hint: Literal["speed_over_quality", "quality_over_speed"] = "speed_over_quality", wait: int = 10) -> bytes:
         url = uritemplate.partial(
             uri="{+asset_rendition_uri}{&format,size,wait,page,markup,processing_hint,download,rendition_class}",
             var_dict={
                 "download": download,
                 "format": format,
                 "page": page,
                 "rendition_class": rendition_class,
@@ -496,34 +498,34 @@
                 "markup": markup,
                 "processing_hint": processing_hint,
                 "wait": wait,
             },
         ).uri
         headers: Dict[str, str] = {}
         headers["Accept"] = "image/jpeg; image/png; image/*; */*"
+
         resp = self._client.request(
             "GET",
             url,
             headers=headers,
         )
-
         content_type = resp.headers["Content-Type"]
 
         if re.search(r"image/jpeg", content_type):
             return resp.content
         if re.search(r"image/png", content_type):
             return resp.content
         if re.search(r"image/.+", content_type):
             return resp.content
         if re.search(r".*", content_type):
             return resp.content
         else:
             raise ValueError(f"Unexpected content type: {content_type}")
 
-    def rendition_direct(self, *, asset_id: str, download: bool, format: Literal["png", "jpg"], page: int, rendition_class: str, size: str, markup: bool = True, processing_hint: Literal["speed_over_quality", "quality_over_speed"] = "speed_over_quality", wait: int = 10) -> Union[bytes]:
+    def rendition_direct(self, *, asset_id: str, download: bool, format: Literal["png", "jpg"], page: int, rendition_class: str, size: str, markup: bool = True, processing_hint: Literal["speed_over_quality", "quality_over_speed"] = "speed_over_quality", wait: int = 10) -> bytes:
         url = uritemplate.partial(
             uri="https://dc-api-v2.adobecontent.io/{expiry}/assets/download/{+asset_id}/rendition{?format,size,wait,page,markup,processing_hint,download,rendition_class}",
             var_dict={
                 "asset_id": asset_id,
                 "download": download,
                 "format": format,
                 "page": page,
@@ -532,20 +534,20 @@
                 "markup": markup,
                 "processing_hint": processing_hint,
                 "wait": wait,
             },
         ).uri
         headers: Dict[str, str] = {}
         headers["Accept"] = "image/jpeg; image/png; image/*; */*"
+
         resp = self._client.request(
             "GET",
             url,
             headers=headers,
         )
-
         content_type = resp.headers["Content-Type"]
 
         if re.search(r"image/jpeg", content_type):
             return resp.content
         if re.search(r"image/png", content_type):
             return resp.content
         if re.search(r"image/.+", content_type):
@@ -564,66 +566,66 @@
                 "make_ticket": make_ticket,
                 "asset_uri": asset_uri,
                 "type": type,
             },
         ).uri
         headers: Dict[str, str] = {}
         headers["Accept"] = 'application/vnd.adobe.dc+json; profile="https://dc-api.adobe.io/schemas/asset_uri_rendition_v1.json"'
+
         resp = self._client.request(
             "GET",
             url,
             headers=headers,
         )
-
         content_type = resp.headers["Content-Type"]
 
         if re.search(r"schemas/asset_uri_rendition_v1\.json", content_type):
             return asset_uri_rendition_v1.Model.model_validate(resp.json())
         else:
             raise ValueError(f"Unexpected content type: {content_type}")
 
     def splitpdf(self, *, _data: "splitpdf_parameters_v1.Model") -> "new_asset_job_v1.Model":
         from ..models import new_asset_job_v1
 
         url = "https://dc-api-v2.adobe.io/{expiry}/assets?operation=splitpdf"
         headers: Dict[str, str] = {}
         headers["Accept"] = 'application/vnd.adobe.dc+json; profile="https://dc-api.adobe.io/schemas/new_asset_job_v1.json"'
+
         resp = self._client.request(
             "POST",
             url,
             headers=headers,
-            json=_data.dict(),
+            json=_data.model_dump(),
         )
-
         content_type = resp.headers["Content-Type"]
 
         if re.search(r"schemas/new_asset_job_v1\.json", content_type):
             return new_asset_job_v1.Model.model_validate(resp.json())
         else:
             raise ValueError(f"Unexpected content type: {content_type}")
 
-    def tag(self, *, _pdf: bytes, async_: bool, client_version: str, qualify: bool, format: Literal["instance_data", "fully_tagged_pdf"] = "instance_data") -> Union[bytes]:
+    def tag(self, *, _pdf: bytes, async_: bool, client_version: str, qualify: bool, format: Literal["instance_data", "fully_tagged_pdf"] = "instance_data") -> bytes:
         url = uritemplate.partial(
             uri="https://taggedpdf.adobe.io/{expiry}/assets?operation=tag{&format,async,qualify,client_version}",
             var_dict={
                 "async": async_,
                 "client_version": client_version,
                 "qualify": qualify,
                 "format": format,
             },
         ).uri
         headers: Dict[str, str] = {}
         headers["Accept"] = "application/pdf; application/zip"
+
         resp = self._client.request(
             "POST",
             url,
             headers=headers,
             content=_pdf,
         )
-
         content_type = resp.headers["Content-Type"]
 
         if re.search(r"application/pdf", content_type):
             return resp.content
         if re.search(r"application/zip", content_type):
             return resp.content
         else:
@@ -631,21 +633,21 @@
 
     def tag_sensei(self, *, _file: Union[IO[bytes], bytes, str]) -> "asset_tag_sensei_v1.Model":
         from ..models import asset_tag_sensei_v1
 
         url = "https://sensei.adobe.io/services/v1/predict"
         headers: Dict[str, str] = {}
         headers["Accept"] = 'application/vnd.adobe.dc+json; profile="https://dc-api.adobe.io/schemas/asset_tag_sensei_v1.json"'
+
         resp = self._client.request(
             "POST",
             url,
             headers=headers,
             files={"file": _file},
         )
-
         content_type = resp.headers["Content-Type"]
 
         if re.search(r"schemas/asset_tag_sensei_v1\.json", content_type):
             return asset_tag_sensei_v1.Model.model_validate(resp.json())
         else:
             raise ValueError(f"Unexpected content type: {content_type}")
 
@@ -653,34 +655,35 @@
         url = uritemplate.partial(
             uri="https://dc-api-v2.adobe.io/{expiry}/assets{?asset_uri}",
             var_dict={
                 "asset_uri": asset_uri,
             },
         ).uri
         headers: Dict[str, str] = {}
-        resp = self._client.request(
+
+        self._client.request(
             "PUT",
             url,
             headers=headers,
             files={"file": _file},
         )
 
     def upload(self, *, _file: Union[IO[bytes], bytes, str]) -> "asset_v1.Model":
         from ..models import asset_v1
 
         url = "https://dc-api-v2.adobe.io/{expiry}/assets"
         headers: Dict[str, str] = {}
         headers["Accept"] = 'application/vnd.adobe.dc+json; profile="https://dc-api.adobe.io/schemas/asset_v1.json"'
+
         resp = self._client.request(
             "POST",
             url,
             headers=headers,
             files={"file": _file},
         )
-
         content_type = resp.headers["Content-Type"]
 
         if re.search(r"schemas/asset_v1\.json", content_type):
             return asset_v1.Model.model_validate(resp.json())
         else:
             raise ValueError(f"Unexpected content type: {content_type}")
 
@@ -691,20 +694,20 @@
             uri="{+asset_upload_status_monitor_uri}",
             var_dict={
                 "asset_upload_status_monitor_uri": asset_upload_status_monitor_uri,
             },
         ).uri
         headers: Dict[str, str] = {}
         headers["Accept"] = 'application/vnd.adobe.dc+json; profile="https://dc-api.adobe.io/schemas/upload_status_v1.json"'
+
         resp = self._client.request(
             "GET",
             url,
             headers=headers,
         )
-
         content_type = resp.headers["Content-Type"]
 
         if re.search(r"schemas/upload_status_v1\.json", content_type):
             return upload_status_v1.Model.model_validate(resp.json())
         else:
             raise ValueError(f"Unexpected content type: {content_type}")
 
@@ -713,39 +716,39 @@
             uri="{+zip_download_uri}",
             var_dict={
                 "zip_download_uri": zip_download_uri,
             },
         ).uri
         headers: Dict[str, str] = {}
         headers["Accept"] = "application/zip"
+
         resp = self._client.request(
             "GET",
             url,
             headers=headers,
         )
-
         content_type = resp.headers["Content-Type"]
 
         if re.search(r"application/zip", content_type):
             return resp.content
         else:
             raise ValueError(f"Unexpected content type: {content_type}")
 
     def zip_download_uri(self, *, _data: "zip_download_params_v1.Model") -> "zip_download_uri_v1.Model":
         from ..models import zip_download_uri_v1
 
         url = "https://dc-api-v2.adobe.io/{expiry}/assets/zip/uri/download"
         headers: Dict[str, str] = {}
         headers["Accept"] = 'application/vnd.adobe.dc+json; profile="https://dc-api.adobe.io/schemas/zip_download_uri_v1.json"'
+
         resp = self._client.request(
             "POST",
             url,
             headers=headers,
-            json=_data.dict(),
+            json=_data.model_dump(),
         )
-
         content_type = resp.headers["Content-Type"]
 
         if re.search(r"schemas/zip_download_uri_v1\.json", content_type):
             return zip_download_uri_v1.Model.model_validate(resp.json())
         else:
             raise ValueError(f"Unexpected content type: {content_type}")
```

### Comparing `pydcapi-0.1.4/src/pydcapi/resources/connector.py` & `pydcapi-0.1.5/src/pydcapi/resources/connector.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 # generated by scripts/generate.py
 
 import re
-from typing import Dict, Literal, TYPE_CHECKING
+from typing import TYPE_CHECKING, Dict, Literal
 
 from .client import Client
 
 if TYPE_CHECKING:
-    from ..models import connector_info_v1, connector_delete_response_v1, connector_listing_v1, connector_link_parameters_v1
-
+    from ..models import connector_delete_response_v1, connector_info_v1, connector_link_parameters_v1, connector_listing_v1
 
 import uritemplate
 
 
 class Connector:
 
     def __init__(self, client: Client):
@@ -25,20 +24,20 @@
             var_dict={
                 "cloud_id": cloud_id,
                 "connector_id": connector_id,
             },
         ).uri
         headers: Dict[str, str] = {}
         headers["Accept"] = 'application/vnd.adobe.dc+json; profile="https://dc-api.adobe.io/schemas/connector_delete_response_v1.json"'
+
         resp = self._client.request(
             "DELETE",
             url,
             headers=headers,
         )
-
         content_type = resp.headers["Content-Type"]
 
         if re.search(r"schemas/connector_delete_response_v1\.json", content_type):
             return connector_delete_response_v1.Model.model_validate(resp.json())
         else:
             raise ValueError(f"Unexpected content type: {content_type}")
 
@@ -49,21 +48,21 @@
             uri="https://dc-api-v2.adobe.io/{expiry}/{cloud_id}/connector/link",
             var_dict={
                 "cloud_id": cloud_id,
             },
         ).uri
         headers: Dict[str, str] = {}
         headers["Accept"] = 'application/vnd.adobe.dc+json; profile="https://dc-api.adobe.io/schemas/connector_info_v1.json"'
+
         resp = self._client.request(
             "POST",
             url,
             headers=headers,
-            json=_data.dict(),
+            json=_data.model_dump(),
         )
-
         content_type = resp.headers["Content-Type"]
 
         if re.search(r"schemas/connector_info_v1\.json", content_type):
             return connector_info_v1.Model.model_validate(resp.json())
         else:
             raise ValueError(f"Unexpected content type: {content_type}")
 
@@ -74,19 +73,19 @@
             uri="https://dc-api-v2.adobe.io/{expiry}/{cloud_id}/connector/list",
             var_dict={
                 "cloud_id": cloud_id,
             },
         ).uri
         headers: Dict[str, str] = {}
         headers["Accept"] = 'application/vnd.adobe.dc+json; profile="https://dc-api.adobe.io/schemas/connector_listing_v1.json"'
+
         resp = self._client.request(
             "GET",
             url,
             headers=headers,
         )
-
         content_type = resp.headers["Content-Type"]
 
         if re.search(r"schemas/connector_listing_v1\.json", content_type):
             return connector_listing_v1.Model.model_validate(resp.json())
         else:
             raise ValueError(f"Unexpected content type: {content_type}")
```

### Comparing `pydcapi-0.1.4/src/pydcapi/resources/discovery.py` & `pydcapi-0.1.5/src/pydcapi/resources/discovery.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,110 +1,111 @@
 # generated by scripts/generate.py
 
 import re
-from typing import Dict, TYPE_CHECKING
+from typing import TYPE_CHECKING, Dict
 
 from .client import Client
 
 if TYPE_CHECKING:
-    from ..models import discovery_v1, services_v1, source_options_v1, exportpdf_options_v1, createpdf_options_v1
+    from ..models import (createpdf_options_v1, discovery_v1,
+                          exportpdf_options_v1, services_v1, source_options_v1)
 
 
 class Discovery:
 
     def __init__(self, client: Client):
         self._client: Client = client
 
     def createpdf_options(self) -> "createpdf_options_v1.Model":
         from ..models import createpdf_options_v1
 
         url = "https://dc-api-v2.adobe.io/{expiry}/discovery/resources/assets/createpdf/options"
         headers: Dict[str, str] = {}
         headers["Accept"] = 'application/vnd.adobe.dc+json; profile="https://dc-api.adobe.io/schemas/createpdf_options_v1.json"'
+
         resp = self._client.request(
             "GET",
             url,
             headers=headers,
         )
-
         content_type = resp.headers["Content-Type"]
 
         if re.search(r"schemas/createpdf_options_v1\.json", content_type):
             return createpdf_options_v1.Model.model_validate(resp.json())
         else:
             raise ValueError(f"Unexpected content type: {content_type}")
 
     def discover(self) -> "discovery_v1.Model":
         from ..models import discovery_v1
 
         url = "https://dc-api-v2.adobe.io/discovery"
         headers: Dict[str, str] = {}
         headers["Accept"] = 'application/vnd.adobe.dc+json; profile="https://dc-api.adobe.io/schemas/discovery_v1.json"'
+
         resp = self._client.request(
             "GET",
             url,
             headers=headers,
         )
-
         content_type = resp.headers["Content-Type"]
 
         if re.search(r"schemas/discovery_v1\.json", content_type):
             return discovery_v1.Model.model_validate(resp.json())
         else:
             raise ValueError(f"Unexpected content type: {content_type}")
 
     def exportpdf_options(self) -> "exportpdf_options_v1.Model":
         from ..models import exportpdf_options_v1
 
         url = "https://dc-api-v2.adobe.io/{expiry}/discovery/resources/assets/exportpdf/options"
         headers: Dict[str, str] = {}
         headers["Accept"] = 'application/vnd.adobe.dc+json; profile="https://dc-api.adobe.io/schemas/exportpdf_options_v1.json"'
+
         resp = self._client.request(
             "GET",
             url,
             headers=headers,
         )
-
         content_type = resp.headers["Content-Type"]
 
         if re.search(r"schemas/exportpdf_options_v1\.json", content_type):
             return exportpdf_options_v1.Model.model_validate(resp.json())
         else:
             raise ValueError(f"Unexpected content type: {content_type}")
 
     def get_services(self) -> "services_v1.Model":
         from ..models import services_v1
 
         url = "https://dc-api-v2.adobe.io/{expiry}/discovery/services"
         headers: Dict[str, str] = {}
         headers["Accept"] = 'application/vnd.adobe.dc+json; profile="https://dc-api.adobe.io/schemas/services_v1.json"'
+
         resp = self._client.request(
             "GET",
             url,
             headers=headers,
         )
-
         content_type = resp.headers["Content-Type"]
 
         if re.search(r"schemas/services_v1\.json", content_type):
             return services_v1.Model.model_validate(resp.json())
         else:
             raise ValueError(f"Unexpected content type: {content_type}")
 
     def source_options(self) -> "source_options_v1.Model":
         from ..models import source_options_v1
 
         url = "https://dc-api-v2.adobe.io/{expiry}/discovery/resources/assets/source/options"
         headers: Dict[str, str] = {}
         headers["Accept"] = 'application/vnd.adobe.dc+json; profile="https://dc-api.adobe.io/schemas/source_options_v1.json"'
+
         resp = self._client.request(
             "GET",
             url,
             headers=headers,
         )
-
         content_type = resp.headers["Content-Type"]
 
         if re.search(r"schemas/source_options_v1\.json", content_type):
             return source_options_v1.Model.model_validate(resp.json())
         else:
             raise ValueError(f"Unexpected content type: {content_type}")
```

### Comparing `pydcapi-0.1.4/src/pydcapi/resources/folders.py` & `pydcapi-0.1.5/src/pydcapi/resources/folders.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 # generated by scripts/generate.py
 
 import re
-from typing import Dict, Literal, TYPE_CHECKING
+from typing import TYPE_CHECKING, Dict, Literal
 
 from .client import Client
 
 if TYPE_CHECKING:
-    from ..models import folder_metadata_field_patch_v1, folder_metadata_basic_v1, folder_breadcrumbs_v1, folder_metadata_field_v1, root_v1, folder_v1, system_folders_v1, folder_listing_v1, folder_creation_v1
-
+    from ..models import folder_breadcrumbs_v1, folder_creation_v1, folder_listing_v1, folder_metadata_basic_v1, folder_metadata_field_patch_v1, folder_metadata_field_v1, folder_v1, root_v1, system_folders_v1
 
 import uritemplate
 
 
 class Folders:
 
     def __init__(self, client: Client):
@@ -24,40 +23,40 @@
             uri="{+folder_uri}/breadcrumbs",
             var_dict={
                 "folder_uri": folder_uri,
             },
         ).uri
         headers: Dict[str, str] = {}
         headers["Accept"] = 'application/vnd.adobe.dc+json; profile="https://dc-api.adobe.io/schemas/folder_breadcrumbs_v1.json"'
+
         resp = self._client.request(
             "GET",
             url,
             headers=headers,
         )
-
         content_type = resp.headers["Content-Type"]
 
         if re.search(r"schemas/folder_breadcrumbs_v1\.json", content_type):
             return folder_breadcrumbs_v1.Model.model_validate(resp.json())
         else:
             raise ValueError(f"Unexpected content type: {content_type}")
 
     def create(self, *, _data: "folder_creation_v1.Model") -> "folder_v1.Model":
         from ..models import folder_v1
 
         url = "https://dc-api-v2.adobe.io/{expiry}/folders"
         headers: Dict[str, str] = {}
         headers["Accept"] = 'application/vnd.adobe.dc+json; profile="https://dc-api.adobe.io/schemas/folder_v1.json"'
+
         resp = self._client.request(
             "POST",
             url,
             headers=headers,
-            json=_data.dict(),
+            json=_data.model_dump(),
         )
-
         content_type = resp.headers["Content-Type"]
 
         if re.search(r"schemas/folder_v1\.json", content_type):
             return folder_v1.Model.model_validate(resp.json())
         else:
             raise ValueError(f"Unexpected content type: {content_type}")
 
@@ -65,15 +64,16 @@
         url = uritemplate.partial(
             uri="{+folder_uri}",
             var_dict={
                 "folder_uri": folder_uri,
             },
         ).uri
         headers: Dict[str, str] = {}
-        resp = self._client.request(
+
+        self._client.request(
             "DELETE",
             url,
             headers=headers,
         )
 
     def get_metadata(self, *, folder_uri: str) -> "folder_metadata_basic_v1.Model":
         from ..models import folder_metadata_basic_v1
@@ -82,20 +82,20 @@
             uri="{+folder_uri}/metadata",
             var_dict={
                 "folder_uri": folder_uri,
             },
         ).uri
         headers: Dict[str, str] = {}
         headers["Accept"] = 'application/vnd.adobe.dc+json; profile="https://dc-api.adobe.io/schemas/folder_metadata_basic_v1.json"'
+
         resp = self._client.request(
             "GET",
             url,
             headers=headers,
         )
-
         content_type = resp.headers["Content-Type"]
 
         if re.search(r"schemas/folder_metadata_basic_v1\.json", content_type):
             return folder_metadata_basic_v1.Model.model_validate(resp.json())
         else:
             raise ValueError(f"Unexpected content type: {content_type}")
 
@@ -107,58 +107,58 @@
             var_dict={
                 "fields": fields,
                 "folder_uri": folder_uri,
             },
         ).uri
         headers: Dict[str, str] = {}
         headers["Accept"] = 'application/vnd.adobe.dc+json; profile="https://dc-api.adobe.io/schemas/folder_metadata_field_v1.json"'
+
         resp = self._client.request(
             "GET",
             url,
             headers=headers,
         )
-
         content_type = resp.headers["Content-Type"]
 
         if re.search(r"schemas/folder_metadata_field_v1\.json", content_type):
             return folder_metadata_field_v1.Model.model_validate(resp.json())
         else:
             raise ValueError(f"Unexpected content type: {content_type}")
 
     def get_root(self) -> "root_v1.Model":
         from ..models import root_v1
 
         url = "https://dc-api-v2.adobe.io/{expiry}/folders/root"
         headers: Dict[str, str] = {}
         headers["Accept"] = 'application/vnd.adobe.dc+json; profile="https://dc-api.adobe.io/schemas/root_v1.json"'
+
         resp = self._client.request(
             "GET",
             url,
             headers=headers,
         )
-
         content_type = resp.headers["Content-Type"]
 
         if re.search(r"schemas/root_v1\.json", content_type):
             return root_v1.Model.model_validate(resp.json())
         else:
             raise ValueError(f"Unexpected content type: {content_type}")
 
     def get_system_folders(self) -> "system_folders_v1.Model":
         from ..models import system_folders_v1
 
         url = "https://dc-api-v2.adobe.io/{expiry}/folders/system_folders"
         headers: Dict[str, str] = {}
         headers["Accept"] = 'application/vnd.adobe.dc+json; profile="https://dc-api.adobe.io/schemas/system_folders_v1.json"'
+
         resp = self._client.request(
             "GET",
             url,
             headers=headers,
         )
-
         content_type = resp.headers["Content-Type"]
 
         if re.search(r"schemas/system_folders_v1\.json", content_type):
             return system_folders_v1.Model.model_validate(resp.json())
         else:
             raise ValueError(f"Unexpected content type: {content_type}")
 
@@ -173,20 +173,20 @@
                 "folder_uri": folder_uri,
                 "metadata": metadata,
                 "page_size": page_size,
             },
         ).uri
         headers: Dict[str, str] = {}
         headers["Accept"] = 'application/vnd.adobe.dc+json; profile="https://dc-api.adobe.io/schemas/folder_listing_v1.json"'
+
         resp = self._client.request(
             "GET",
             url,
             headers=headers,
         )
-
         content_type = resp.headers["Content-Type"]
 
         if re.search(r"schemas/folder_listing_v1\.json", content_type):
             return folder_listing_v1.Model.model_validate(resp.json())
         else:
             raise ValueError(f"Unexpected content type: {content_type}")
 
@@ -197,20 +197,20 @@
             uri="{+next_page_uri}",
             var_dict={
                 "next_page_uri": next_page_uri,
             },
         ).uri
         headers: Dict[str, str] = {}
         headers["Accept"] = 'application/vnd.adobe.dc+json; profile="https://dc-api.adobe.io/schemas/folder_listing_v1.json"'
+
         resp = self._client.request(
             "GET",
             url,
             headers=headers,
         )
-
         content_type = resp.headers["Content-Type"]
 
         if re.search(r"schemas/folder_listing_v1\.json", content_type):
             return folder_listing_v1.Model.model_validate(resp.json())
         else:
             raise ValueError(f"Unexpected content type: {content_type}")
 
@@ -222,21 +222,21 @@
             var_dict={
                 "fields": fields,
                 "folder_uri": folder_uri,
             },
         ).uri
         headers: Dict[str, str] = {}
         headers["Accept"] = 'application/vnd.adobe.dc+json; profile="https://dc-api.adobe.io/schemas/folder_metadata_field_v1.json"'
+
         resp = self._client.request(
             "PATCH",
             url,
             headers=headers,
-            json=_data.dict(),
+            json=_data.model_dump(),
         )
-
         content_type = resp.headers["Content-Type"]
 
         if re.search(r"schemas/folder_metadata_field_v1\.json", content_type):
             return folder_metadata_field_v1.Model.model_validate(resp.json())
         else:
             raise ValueError(f"Unexpected content type: {content_type}")
 
@@ -245,13 +245,14 @@
             uri="{+folder_uri}/metadata{/fields}",
             var_dict={
                 "fields": fields,
                 "folder_uri": folder_uri,
             },
         ).uri
         headers: Dict[str, str] = {}
-        resp = self._client.request(
+
+        self._client.request(
             "PUT",
             url,
             headers=headers,
-            json=_data.dict(),
+            json=_data.model_dump(),
         )
```

### Comparing `pydcapi-0.1.4/src/pydcapi/resources/jobs.py` & `pydcapi-0.1.5/src/pydcapi/resources/jobs.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 # generated by scripts/generate.py
 
 import re
-from typing import Dict, TYPE_CHECKING
+from typing import TYPE_CHECKING, Dict
 
 from .client import Client
 
 if TYPE_CHECKING:
     from ..models import new_asset_job_v1
 
-
 import uritemplate
 
 
 class Jobs:
 
     def __init__(self, client: Client):
         self._client: Client = client
@@ -24,19 +23,19 @@
             uri="{+job_uri}/status",
             var_dict={
                 "job_uri": job_uri,
             },
         ).uri
         headers: Dict[str, str] = {}
         headers["Accept"] = 'application/vnd.adobe.dc+json; profile="https://dc-api.adobe.io/schemas/new_asset_job_v1.json"'
+
         resp = self._client.request(
             "GET",
             url,
             headers=headers,
         )
-
         content_type = resp.headers["Content-Type"]
 
         if re.search(r"schemas/new_asset_job_v1\.json", content_type):
             return new_asset_job_v1.Model.model_validate(resp.json())
         else:
             raise ValueError(f"Unexpected content type: {content_type}")
```

### Comparing `pydcapi-0.1.4/src/pydcapi/resources/operations.py` & `pydcapi-0.1.5/src/pydcapi/resources/operations.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,76 +1,79 @@
 # generated by scripts/generate.py
 
 import re
-from typing import Dict, TYPE_CHECKING, Union
+from typing import TYPE_CHECKING, Dict, Union
 
 from .client import Client
 
 if TYPE_CHECKING:
-    from ..models import move_op_params_v1, move_op_result_v1, copy_op_params_v1, multiple_move_op_result_v1, copy_to_user_parameters_v1, new_asset_job_v1, asset_v1
+    from ..models import (asset_v1, copy_op_params_v1,
+                          copy_to_user_parameters_v1, move_op_params_v1,
+                          move_op_result_v1, multiple_move_op_result_v1,
+                          new_asset_job_v1)
 
 
 class Operations:
 
     def __init__(self, client: Client):
         self._client: Client = client
 
     def copy(self, *, _data: "copy_op_params_v1.Model") -> "new_asset_job_v1.Model":
         from ..models import new_asset_job_v1
 
         url = "https://dc-api-v2.adobe.io/{expiry}/operations/copy"
         headers: Dict[str, str] = {}
         headers["Accept"] = 'application/vnd.adobe.dc+json; profile="https://dc-api.adobe.io/schemas/new_asset_job_v1.json"'
+
         resp = self._client.request(
             "POST",
             url,
             headers=headers,
-            json=_data.dict(),
+            json=_data.model_dump(),
         )
-
         content_type = resp.headers["Content-Type"]
 
         if re.search(r"schemas/new_asset_job_v1\.json", content_type):
             return new_asset_job_v1.Model.model_validate(resp.json())
         else:
             raise ValueError(f"Unexpected content type: {content_type}")
 
     def copy_to_user(self, *, _data: "copy_to_user_parameters_v1.Model") -> "asset_v1.Model":
         from ..models import asset_v1
 
         url = "https://pdfnow.adobe.io/{expiry}/operations/copy_to_user"
         headers: Dict[str, str] = {}
         headers["Accept"] = 'application/vnd.adobe.dc+json; profile="https://dc-api.adobe.io/schemas/asset_v1.json"'
+
         resp = self._client.request(
             "POST",
             url,
             headers=headers,
-            json=_data.dict(),
+            json=_data.model_dump(),
         )
-
         content_type = resp.headers["Content-Type"]
 
         if re.search(r"schemas/asset_v1\.json", content_type):
             return asset_v1.Model.model_validate(resp.json())
         else:
             raise ValueError(f"Unexpected content type: {content_type}")
 
     def move(self, *, _data: "move_op_params_v1.Model") -> Union["move_op_result_v1.Model", "multiple_move_op_result_v1.Model"]:
         from ..models import move_op_result_v1, multiple_move_op_result_v1
 
         url = "https://dc-api-v2.adobe.io/{expiry}/operations/move"
         headers: Dict[str, str] = {}
         headers["Accept"] = 'application/vnd.adobe.dc+json; profile="https://dc-api.adobe.io/schemas/move_op_result_v1.json"; application/vnd.adobe.dc+json; profile="https://dc-api.adobe.io/schemas/multiple_move_op_result_v1.json"'
+
         resp = self._client.request(
             "POST",
             url,
             headers=headers,
-            json=_data.dict(),
+            json=_data.model_dump(),
         )
-
         content_type = resp.headers["Content-Type"]
 
         if re.search(r"schemas/move_op_result_v1\.json", content_type):
             return move_op_result_v1.Model.model_validate(resp.json())
         if re.search(r"schemas/multiple_move_op_result_v1\.json", content_type):
             return multiple_move_op_result_v1.Model.model_validate(resp.json())
         else:
```

### Comparing `pydcapi-0.1.4/src/pydcapi/resources/system.py` & `pydcapi-0.1.5/src/pydcapi/resources/system.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # generated by scripts/generate.py
 
 import re
-from typing import Dict, TYPE_CHECKING
+from typing import TYPE_CHECKING, Dict
 
 from .client import Client
 
 if TYPE_CHECKING:
     from ..models import system_log_parameters_v1
 
 
@@ -13,30 +13,31 @@
 
     def __init__(self, client: Client):
         self._client: Client = client
 
     def log(self, *, _data: "system_log_parameters_v1.Model") -> None:
         url = "https://dc-api-v2.adobe.io/system/log"
         headers: Dict[str, str] = {}
-        resp = self._client.request(
+
+        self._client.request(
             "POST",
             url,
             headers=headers,
-            json=_data.dict(),
+            json=_data.model_dump(),
         )
 
     def time(self) -> str:
         url = "https://taggedpdf.adobe.io/{expiry}/system/time"
         headers: Dict[str, str] = {}
         headers["Accept"] = "text/plain"
+
         resp = self._client.request(
             "GET",
             url,
             headers=headers,
         )
-
         content_type = resp.headers["Content-Type"]
 
         if re.search(r"text/plain", content_type):
             return resp.text
         else:
             raise ValueError(f"Unexpected content type: {content_type}")
```

### Comparing `pydcapi-0.1.4/src/pydcapi/resources/users.py` & `pydcapi-0.1.5/src/pydcapi/resources/users.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 # generated by scripts/generate.py
 
 import re
-from typing import Dict, Literal, TYPE_CHECKING
+from typing import TYPE_CHECKING, Dict, Literal
 
 from .client import Client
 
 if TYPE_CHECKING:
-    from ..models import user_limits_review_v1, recent_searches_v1, user_storage_document_cloud_v1, user_limits_acrobat_v1, user_upsell_v1, user_limits_esign_v1, user_v1, user_cohorts_v1, user_limits_pdf_services_v1, user_prefs_v1, user_limits_fillsign_v1, user_limits_send_v1, user_limits_storage_document_cloud_v1, user_subscriptions_v1, user_limits_conversions_v1, user_limits_verbs_v1, user_put_identity_v1, recent_search_v1, user_identity_v1
-
+    from ..models import recent_search_v1, recent_searches_v1, user_cohorts_v1, user_identity_v1, user_limits_acrobat_v1, user_limits_conversions_v1, user_limits_esign_v1, user_limits_fillsign_v1, user_limits_pdf_services_v1, user_limits_review_v1, user_limits_send_v1, user_limits_storage_document_cloud_v1, user_limits_verbs_v1, user_prefs_v1, user_put_identity_v1, user_storage_document_cloud_v1, user_subscriptions_v1, user_upsell_v1, user_v1
 
 import uritemplate
 
 
 class Users:
 
     def __init__(self, client: Client):
@@ -21,15 +20,16 @@
         url = uritemplate.partial(
             uri="{+user_uri}/state/recentsearches",
             var_dict={
                 "user_uri": user_uri,
             },
         ).uri
         headers: Dict[str, str] = {}
-        resp = self._client.request(
+
+        self._client.request(
             "DELETE",
             url,
             headers=headers,
         )
 
     def get_cohorts(self, *, user_uri: str = "https://dc-api-v2.adobe.io/{expiry}/users/self") -> "user_cohorts_v1.Model":
         from ..models import user_cohorts_v1
@@ -38,20 +38,20 @@
             uri="{+user_uri}/cohorts",
             var_dict={
                 "user_uri": user_uri,
             },
         ).uri
         headers: Dict[str, str] = {}
         headers["Accept"] = 'application/vnd.adobe.dc+json; profile="https://dc-api.adobe.io/schemas/user_cohorts_v1.json"'
+
         resp = self._client.request(
             "GET",
             url,
             headers=headers,
         )
-
         content_type = resp.headers["Content-Type"]
 
         if re.search(r"schemas/user_cohorts_v1\.json", content_type):
             return user_cohorts_v1.Model.model_validate(resp.json())
         else:
             raise ValueError(f"Unexpected content type: {content_type}")
 
@@ -62,20 +62,20 @@
             uri="{+user_uri}/identity",
             var_dict={
                 "user_uri": user_uri,
             },
         ).uri
         headers: Dict[str, str] = {}
         headers["Accept"] = 'application/vnd.adobe.dc+json; profile="https://dc-api.adobe.io/schemas/user_identity_v1.json"'
+
         resp = self._client.request(
             "GET",
             url,
             headers=headers,
         )
-
         content_type = resp.headers["Content-Type"]
 
         if re.search(r"schemas/user_identity_v1\.json", content_type):
             return user_identity_v1.Model.model_validate(resp.json())
         else:
             raise ValueError(f"Unexpected content type: {content_type}")
 
@@ -86,20 +86,20 @@
             uri="{+user_uri}/limits/acrobat",
             var_dict={
                 "user_uri": user_uri,
             },
         ).uri
         headers: Dict[str, str] = {}
         headers["Accept"] = 'application/vnd.adobe.dc+json; profile="https://dc-api.adobe.io/schemas/user_limits_acrobat_v1.json"'
+
         resp = self._client.request(
             "GET",
             url,
             headers=headers,
         )
-
         content_type = resp.headers["Content-Type"]
 
         if re.search(r"schemas/user_limits_acrobat_v1\.json", content_type):
             return user_limits_acrobat_v1.Model.model_validate(resp.json())
         else:
             raise ValueError(f"Unexpected content type: {content_type}")
 
@@ -110,20 +110,20 @@
             uri="{+user_uri}/limits/conversions",
             var_dict={
                 "user_uri": user_uri,
             },
         ).uri
         headers: Dict[str, str] = {}
         headers["Accept"] = 'application/vnd.adobe.dc+json; profile="https://dc-api.adobe.io/schemas/user_limits_conversions_v1.json"'
+
         resp = self._client.request(
             "GET",
             url,
             headers=headers,
         )
-
         content_type = resp.headers["Content-Type"]
 
         if re.search(r"schemas/user_limits_conversions_v1\.json", content_type):
             return user_limits_conversions_v1.Model.model_validate(resp.json())
         else:
             raise ValueError(f"Unexpected content type: {content_type}")
 
@@ -134,20 +134,20 @@
             uri="{+user_uri}/limits/esign",
             var_dict={
                 "user_uri": user_uri,
             },
         ).uri
         headers: Dict[str, str] = {}
         headers["Accept"] = 'application/vnd.adobe.dc+json; profile="https://dc-api.adobe.io/schemas/user_limits_esign_v1.json"'
+
         resp = self._client.request(
             "GET",
             url,
             headers=headers,
         )
-
         content_type = resp.headers["Content-Type"]
 
         if re.search(r"schemas/user_limits_esign_v1\.json", content_type):
             return user_limits_esign_v1.Model.model_validate(resp.json())
         else:
             raise ValueError(f"Unexpected content type: {content_type}")
 
@@ -158,20 +158,20 @@
             uri="{+user_uri}/limits/fillsign",
             var_dict={
                 "user_uri": user_uri,
             },
         ).uri
         headers: Dict[str, str] = {}
         headers["Accept"] = 'application/vnd.adobe.dc+json; profile="https://dc-api.adobe.io/schemas/user_limits_fillsign_v1.json"'
+
         resp = self._client.request(
             "GET",
             url,
             headers=headers,
         )
-
         content_type = resp.headers["Content-Type"]
 
         if re.search(r"schemas/user_limits_fillsign_v1\.json", content_type):
             return user_limits_fillsign_v1.Model.model_validate(resp.json())
         else:
             raise ValueError(f"Unexpected content type: {content_type}")
 
@@ -182,20 +182,20 @@
             uri="{+user_uri}/limits/pdf_services",
             var_dict={
                 "user_uri": user_uri,
             },
         ).uri
         headers: Dict[str, str] = {}
         headers["Accept"] = 'application/vnd.adobe.dc+json; profile="https://dc-api.adobe.io/schemas/user_limits_pdf_services_v1.json"'
+
         resp = self._client.request(
             "GET",
             url,
             headers=headers,
         )
-
         content_type = resp.headers["Content-Type"]
 
         if re.search(r"schemas/user_limits_pdf_services_v1\.json", content_type):
             return user_limits_pdf_services_v1.Model.model_validate(resp.json())
         else:
             raise ValueError(f"Unexpected content type: {content_type}")
 
@@ -206,20 +206,20 @@
             uri="{+user_uri}/limits/review",
             var_dict={
                 "user_uri": user_uri,
             },
         ).uri
         headers: Dict[str, str] = {}
         headers["Accept"] = 'application/vnd.adobe.dc+json; profile="https://dc-api.adobe.io/schemas/user_limits_review_v1.json"'
+
         resp = self._client.request(
             "GET",
             url,
             headers=headers,
         )
-
         content_type = resp.headers["Content-Type"]
 
         if re.search(r"schemas/user_limits_review_v1\.json", content_type):
             return user_limits_review_v1.Model.model_validate(resp.json())
         else:
             raise ValueError(f"Unexpected content type: {content_type}")
 
@@ -230,20 +230,20 @@
             uri="{+user_uri}/limits/send",
             var_dict={
                 "user_uri": user_uri,
             },
         ).uri
         headers: Dict[str, str] = {}
         headers["Accept"] = 'application/vnd.adobe.dc+json; profile="https://dc-api.adobe.io/schemas/user_limits_send_v1.json"'
+
         resp = self._client.request(
             "GET",
             url,
             headers=headers,
         )
-
         content_type = resp.headers["Content-Type"]
 
         if re.search(r"schemas/user_limits_send_v1\.json", content_type):
             return user_limits_send_v1.Model.model_validate(resp.json())
         else:
             raise ValueError(f"Unexpected content type: {content_type}")
 
@@ -254,20 +254,20 @@
             uri="{+user_uri}/limits/storage/document_cloud",
             var_dict={
                 "user_uri": user_uri,
             },
         ).uri
         headers: Dict[str, str] = {}
         headers["Accept"] = 'application/vnd.adobe.dc+json; profile="https://dc-api.adobe.io/schemas/user_limits_storage_document_cloud_v1.json"'
+
         resp = self._client.request(
             "GET",
             url,
             headers=headers,
         )
-
         content_type = resp.headers["Content-Type"]
 
         if re.search(r"schemas/user_limits_storage_document_cloud_v1\.json", content_type):
             return user_limits_storage_document_cloud_v1.Model.model_validate(resp.json())
         else:
             raise ValueError(f"Unexpected content type: {content_type}")
 
@@ -278,20 +278,20 @@
             uri="{+user_uri}/limits/verbs",
             var_dict={
                 "user_uri": user_uri,
             },
         ).uri
         headers: Dict[str, str] = {}
         headers["Accept"] = 'application/vnd.adobe.dc+json; profile="https://dc-api.adobe.io/schemas/user_limits_verbs_v1.json"'
+
         resp = self._client.request(
             "GET",
             url,
             headers=headers,
         )
-
         content_type = resp.headers["Content-Type"]
 
         if re.search(r"schemas/user_limits_verbs_v1\.json", content_type):
             return user_limits_verbs_v1.Model.model_validate(resp.json())
         else:
             raise ValueError(f"Unexpected content type: {content_type}")
 
@@ -303,20 +303,20 @@
             var_dict={
                 "category": category,
                 "user_uri": user_uri,
             },
         ).uri
         headers: Dict[str, str] = {}
         headers["Accept"] = 'application/vnd.adobe.dc+json; profile="https://dc-api.adobe.io/schemas/user_prefs_v1.json"'
+
         resp = self._client.request(
             "GET",
             url,
             headers=headers,
         )
-
         content_type = resp.headers["Content-Type"]
 
         if re.search(r"schemas/user_prefs_v1\.json", content_type):
             return user_prefs_v1.Model.model_validate(resp.json())
         else:
             raise ValueError(f"Unexpected content type: {content_type}")
 
@@ -327,20 +327,20 @@
             uri="{+user_uri}/state/recentsearches",
             var_dict={
                 "user_uri": user_uri,
             },
         ).uri
         headers: Dict[str, str] = {}
         headers["Accept"] = 'application/vnd.adobe.dc+json; profile="https://dc-api.adobe.io/schemas/recent_searches_v1.json"'
+
         resp = self._client.request(
             "GET",
             url,
             headers=headers,
         )
-
         content_type = resp.headers["Content-Type"]
 
         if re.search(r"schemas/recent_searches_v1\.json", content_type):
             return recent_searches_v1.Model.model_validate(resp.json())
         else:
             raise ValueError(f"Unexpected content type: {content_type}")
 
@@ -351,20 +351,20 @@
             uri="{+user_uri}/storage/document_cloud",
             var_dict={
                 "user_uri": user_uri,
             },
         ).uri
         headers: Dict[str, str] = {}
         headers["Accept"] = 'application/vnd.adobe.dc+json; profile="https://dc-api.adobe.io/schemas/user_storage_document_cloud_v1.json"'
+
         resp = self._client.request(
             "GET",
             url,
             headers=headers,
         )
-
         content_type = resp.headers["Content-Type"]
 
         if re.search(r"schemas/user_storage_document_cloud_v1\.json", content_type):
             return user_storage_document_cloud_v1.Model.model_validate(resp.json())
         else:
             raise ValueError(f"Unexpected content type: {content_type}")
 
@@ -375,20 +375,20 @@
             uri="{+user_uri}/subscriptions",
             var_dict={
                 "user_uri": user_uri,
             },
         ).uri
         headers: Dict[str, str] = {}
         headers["Accept"] = 'application/vnd.adobe.dc+json; profile="https://dc-api.adobe.io/schemas/user_subscriptions_v1.json"'
+
         resp = self._client.request(
             "GET",
             url,
             headers=headers,
         )
-
         content_type = resp.headers["Content-Type"]
 
         if re.search(r"schemas/user_subscriptions_v1\.json", content_type):
             return user_subscriptions_v1.Model.model_validate(resp.json())
         else:
             raise ValueError(f"Unexpected content type: {content_type}")
 
@@ -400,20 +400,20 @@
             var_dict={
                 "entitlement": entitlement,
                 "user_uri": user_uri,
             },
         ).uri
         headers: Dict[str, str] = {}
         headers["Accept"] = 'application/vnd.adobe.dc+json; profile="https://dc-api.adobe.io/schemas/user_upsell_v1.json"'
+
         resp = self._client.request(
             "GET",
             url,
             headers=headers,
         )
-
         content_type = resp.headers["Content-Type"]
 
         if re.search(r"schemas/user_upsell_v1\.json", content_type):
             return user_upsell_v1.Model.model_validate(resp.json())
         else:
             raise ValueError(f"Unexpected content type: {content_type}")
 
@@ -425,20 +425,20 @@
             var_dict={
                 "fields": fields,
                 "user_uri": user_uri,
             },
         ).uri
         headers: Dict[str, str] = {}
         headers["Accept"] = 'application/vnd.adobe.dc+json; profile="https://dc-api.adobe.io/schemas/user_v1.json"'
+
         resp = self._client.request(
             "GET",
             url,
             headers=headers,
         )
-
         content_type = resp.headers["Content-Type"]
 
         if re.search(r"schemas/user_v1\.json", content_type):
             return user_v1.Model.model_validate(resp.json())
         else:
             raise ValueError(f"Unexpected content type: {content_type}")
 
@@ -446,44 +446,47 @@
         url = uritemplate.partial(
             uri="{+user_uri}/state/recentsearches",
             var_dict={
                 "user_uri": user_uri,
             },
         ).uri
         headers: Dict[str, str] = {}
-        resp = self._client.request(
+
+        self._client.request(
             "POST",
             url,
             headers=headers,
-            json=_data.dict(),
+            json=_data.model_dump(),
         )
 
     def put_identity(self, *, _data: "user_put_identity_v1.Model", user_uri: str = "https://dc-api-v2.adobe.io/{expiry}/users/self") -> None:
         url = uritemplate.partial(
             uri="{+user_uri}/identity",
             var_dict={
                 "user_uri": user_uri,
             },
         ).uri
         headers: Dict[str, str] = {}
-        resp = self._client.request(
+
+        self._client.request(
             "PUT",
             url,
             headers=headers,
-            json=_data.dict(),
+            json=_data.model_dump(),
         )
 
     def put_prefs(self, *, _data: "user_prefs_v1.Model", category: Literal["dcweb", "recent_assets", "recent_assets_timestamp", "common", "acrobat", "fillsign"], user_uri: str = "https://dc-api-v2.adobe.io/{expiry}/users/self") -> None:
         url = uritemplate.partial(
             uri="{+user_uri}/prefs/{category}",
             var_dict={
                 "category": category,
                 "user_uri": user_uri,
             },
         ).uri
         headers: Dict[str, str] = {}
-        resp = self._client.request(
+
+        self._client.request(
             "PUT",
             url,
             headers=headers,
-            json=_data.dict(),
+            json=_data.model_dump(),
         )
```

### Comparing `pydcapi-0.1.4/.gitignore` & `pydcapi-0.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `pydcapi-0.1.4/LICENSE` & `pydcapi-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pydcapi-0.1.4/PKG-INFO` & `pydcapi-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: pydcapi
-Version: 0.1.4
+Version: 0.1.5
 Summary: Unofficial Python library for Adobe Document Cloud
 Project-URL: GitHub, https://github.com/mkuznets/pydcapi
 Author-email: Max Kuznetsov <maks.kuznetsov@gmail.com>
 License-File: LICENSE
 Requires-Python: >=3.8
 Requires-Dist: httpx>=0.20.0
 Requires-Dist: pydantic>=2.0
```

