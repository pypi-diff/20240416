# Comparing `tmp/zohocrmsdk2_0-5.1.0.tar.gz` & `tmp/zohocrmsdk2_0-6.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zohocrmsdk2_0-5.1.0.tar", last modified: Mon Feb  6 12:22:43 2023, max compression
+gzip compressed data, was "zohocrmsdk2_0-6.0.0.tar", last modified: Tue Apr 16 13:25:52 2024, max compression
```

## Comparing `zohocrmsdk2_0-5.1.0.tar` & `zohocrmsdk2_0-6.0.0.tar`

### file list

```diff
@@ -1,463 +1,463 @@
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-02-06 12:22:43.289102 zohocrmsdk2_0-5.1.0/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)    11358 2023-02-01 13:00:28.000000 zohocrmsdk2_0-5.1.0/LICENSE
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)       55 2023-02-01 13:00:28.000000 zohocrmsdk2_0-5.1.0/MANIFEST.in
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)    42288 2023-02-06 12:22:43.289102 zohocrmsdk2_0-5.1.0/PKG-INFO
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)    41282 2023-02-01 13:00:28.000000 zohocrmsdk2_0-5.1.0/README.md
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)       67 2023-02-06 12:22:43.293101 zohocrmsdk2_0-5.1.0/setup.cfg
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1584 2023-02-06 11:57:43.000000 zohocrmsdk2_0-5.1.0/setup.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-02-06 12:22:43.229116 zohocrmsdk2_0-5.1.0/zcrmsdk/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)       17 2023-02-01 13:00:28.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/__init__.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-02-06 12:22:43.233115 zohocrmsdk2_0-5.1.0/zcrmsdk/src/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)       17 2023-02-01 13:00:28.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/__init__.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-02-06 12:22:43.233115 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)       18 2023-02-01 13:00:28.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/__init__.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-02-06 12:22:43.233115 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)       35 2023-02-01 13:00:28.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/__init__.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-02-06 12:22:43.233115 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/api/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)       49 2023-02-01 13:00:28.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/api/__init__.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-02-06 12:22:43.233115 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/api/authenticator/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)       81 2023-02-01 13:00:28.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/api/authenticator/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)    12677 2023-02-01 13:00:28.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/api/authenticator/oauth_token.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-02-06 12:22:43.233115 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/api/authenticator/store/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      100 2023-02-01 13:00:28.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/api/authenticator/store/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)    11429 2023-02-06 10:00:47.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/api/authenticator/store/db_store.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     8998 2023-02-01 13:00:28.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/api/authenticator/store/file_store.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1969 2023-02-01 13:00:28.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/api/authenticator/store/token_store.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      665 2023-02-01 13:00:28.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/api/authenticator/token.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-02-06 12:22:43.233115 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/api/logger/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)       39 2023-02-01 13:00:28.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/api/logger/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2815 2023-02-01 13:00:28.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/api/logger/logger.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-02-06 12:22:43.233115 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)       17 2023-02-01 13:00:28.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/__init__.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-02-06 12:22:43.233115 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      984 2023-02-01 13:00:28.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/__init__.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-02-06 12:22:43.237114 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/attachments/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      518 2023-02-03 05:06:34.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/attachments/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      138 2023-02-03 05:06:34.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/attachments/action_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      140 2023-02-03 05:06:34.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/attachments/action_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2037 2023-02-03 05:06:34.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/attachments/action_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3948 2023-02-03 05:06:34.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/attachments/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)    11441 2023-02-03 05:06:34.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/attachments/attachment.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     8807 2023-02-03 05:06:34.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/attachments/attachments_operations.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2135 2023-02-03 05:06:34.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/attachments/file_body_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-02-03 05:06:34.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/attachments/response_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2648 2023-02-03 05:06:34.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/attachments/response_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3662 2023-02-03 05:06:34.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/attachments/success_response.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-02-06 12:22:43.237114 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/blue_print/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      512 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/blue_print/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      140 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/blue_print/action_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3805 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/blue_print/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     4015 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/blue_print/blue_print.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3177 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/blue_print/blue_print_operations.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1949 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/blue_print/body_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2375 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/blue_print/next_transition.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     7825 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/blue_print/process_info.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/blue_print/response_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2291 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/blue_print/response_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3661 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/blue_print/success_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     8191 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/blue_print/transition.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2531 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/blue_print/validation_error.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-02-06 12:22:43.237114 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/bulk_read/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      599 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/bulk_read/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      138 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/bulk_read/action_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      140 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/bulk_read/action_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2519 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/bulk_read/action_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3942 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/bulk_read/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3544 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/bulk_read/bulk_read_operations.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2421 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/bulk_read/call_back.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     4063 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/bulk_read/criteria.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2133 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/bulk_read/file_body_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     6167 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/bulk_read/job_detail.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     4139 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/bulk_read/query.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3309 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/bulk_read/request_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/bulk_read/response_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2049 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/bulk_read/response_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     4225 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/bulk_read/result.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3660 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/bulk_read/success_response.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-02-06 12:22:43.241113 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/bulk_write/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      590 2023-02-03 05:06:34.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/bulk_write/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      140 2023-02-03 05:06:34.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/bulk_write/action_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     7349 2023-02-03 05:06:34.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/bulk_write/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     5548 2023-02-03 05:06:34.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/bulk_write/bulk_write_operations.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     7120 2023-02-03 05:06:34.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/bulk_write/bulk_write_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2421 2023-02-03 05:06:34.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/bulk_write/call_back.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     4729 2023-02-03 05:06:34.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/bulk_write/field_mapping.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     4933 2023-02-03 05:06:34.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/bulk_write/file.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2134 2023-02-03 05:06:34.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/bulk_write/file_body_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3956 2023-02-03 05:06:34.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/bulk_write/request_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     5934 2023-02-03 05:06:34.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/bulk_write/resource.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-02-03 05:06:34.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/bulk_write/response_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-02-03 05:06:34.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/bulk_write/response_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2021 2023-02-03 05:06:34.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/bulk_write/result.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3661 2023-02-03 05:06:34.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/bulk_write/success_response.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-02-06 12:22:43.245112 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/contact_roles/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      831 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/contact_roles/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      138 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/contact_roles/action_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      140 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/contact_roles/action_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2165 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/contact_roles/action_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     4314 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/contact_roles/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2005 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/contact_roles/body_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3043 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/contact_roles/contact_role.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2045 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/contact_roles/contact_role_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)    14167 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/contact_roles/contact_roles_operations.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      150 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/contact_roles/record_action_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2083 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/contact_roles/record_action_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1891 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/contact_roles/record_body_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      154 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/contact_roles/record_response_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2694 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/contact_roles/record_response_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/contact_roles/response_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2179 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/contact_roles/response_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3664 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/contact_roles/success_response.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-02-06 12:22:43.249111 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/currencies/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      649 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/currencies/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      138 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/currencies/action_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      140 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/currencies/action_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2120 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/currencies/action_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     4149 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/currencies/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      162 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/currencies/base_currency_action_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2471 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/currencies/base_currency_action_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2180 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/currencies/base_currency_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1963 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/currencies/body_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     8572 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/currencies/currencies_operations.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     9248 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/currencies/currency.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3407 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/currencies/format.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/currencies/response_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2134 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/currencies/response_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3661 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/currencies/success_response.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-02-06 12:22:43.249111 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/custom_views/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      426 2023-02-03 05:06:34.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/custom_views/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3662 2023-02-03 05:06:34.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/custom_views/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     4015 2023-02-03 05:06:34.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/custom_views/criteria.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)    10152 2023-02-03 05:06:34.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/custom_views/custom_view.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3288 2023-02-03 05:06:34.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/custom_views/custom_views_operations.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     4914 2023-02-03 05:06:34.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/custom_views/info.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2369 2023-02-03 05:06:34.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/custom_views/range.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-02-03 05:06:34.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/custom_views/response_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2769 2023-02-03 05:06:34.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/custom_views/response_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3511 2023-02-03 05:06:34.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/custom_views/shared_details.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     4067 2023-02-03 05:06:34.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/custom_views/translation.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-02-06 12:22:43.249111 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/dc/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      282 2023-02-01 13:00:28.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/dc/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1410 2023-02-01 13:00:28.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/dc/au_data_center.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1399 2023-02-01 13:00:28.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/dc/cn_data_center.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1124 2023-02-01 13:00:28.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/dc/data_center.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1381 2023-02-01 13:00:28.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/dc/eu_data_center.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1379 2023-02-01 13:00:28.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/dc/in_data_center.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1402 2023-02-01 13:00:28.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/dc/jp_data_center.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1384 2023-02-01 13:00:28.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/dc/us_data_center.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-02-06 12:22:43.249111 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/exception/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)       40 2023-02-01 13:00:28.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/exception/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1157 2023-02-01 13:00:28.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/exception/sdk_exception.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-02-06 12:22:43.253110 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/fields/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      730 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/fields/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3656 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/fields/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2989 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/fields/association_details.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3099 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/fields/auto_number.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     4579 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/fields/crypt.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2651 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/fields/currency.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)    32964 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/fields/field.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3108 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/fields/fields_operations.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2611 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/fields/formula.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2369 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/fields/lookup_field.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     4878 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/fields/module.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     5245 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/fields/multi_select_lookup.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     5721 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/fields/pick_list_value.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3027 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/fields/private.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     4247 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/fields/related_details.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/fields/response_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2074 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/fields/response_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2419 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/fields/tool_tip.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2037 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/fields/unique.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3557 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/fields/view_type.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-02-06 12:22:43.253110 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/file/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      421 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/file/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      138 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/file/action_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      140 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/file/action_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2030 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/file/action_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3927 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/file/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1909 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/file/body_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2128 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/file/file_body_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3288 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/file/file_operations.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/file/response_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3655 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/file/success_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      447 2023-02-01 13:00:28.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/header.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1796 2023-02-01 13:00:28.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/header_map.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)    11164 2023-02-01 13:00:28.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/initializer.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-02-06 12:22:43.257109 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/layouts/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      306 2023-02-03 05:06:34.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/layouts/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3657 2023-02-03 05:06:34.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/layouts/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     8542 2023-02-03 05:06:34.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/layouts/layout.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2614 2023-02-03 05:06:34.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/layouts/layouts_operations.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3312 2023-02-03 05:06:34.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/layouts/properties.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-02-03 05:06:34.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/layouts/response_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2089 2023-02-03 05:06:34.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/layouts/response_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     7679 2023-02-03 05:06:34.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/layouts/section.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-02-06 12:22:43.257109 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/modules/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      562 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/modules/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      138 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/modules/action_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      140 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/modules/action_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2075 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/modules/action_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3936 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/modules/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2421 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/modules/argument.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1921 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/modules/body_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)    30518 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/modules/module.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     5464 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/modules/modules_operations.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3087 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/modules/related_list_properties.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/modules/response_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2089 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/modules/response_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3658 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/modules/success_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2995 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/modules/territory.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-02-06 12:22:43.261108 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/notes/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      514 2023-02-03 05:06:34.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/notes/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      138 2023-02-03 05:06:34.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/notes/action_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      140 2023-02-03 05:06:34.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/notes/action_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2031 2023-02-03 05:06:34.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/notes/action_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3930 2023-02-03 05:06:34.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/notes/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1879 2023-02-03 05:06:34.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/notes/body_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3585 2023-02-03 05:06:34.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/notes/info.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)    11186 2023-02-03 05:06:34.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/notes/note.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     9892 2023-02-03 05:06:34.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/notes/notes_operations.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-02-03 05:06:34.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/notes/response_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2643 2023-02-03 05:06:34.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/notes/response_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3656 2023-02-03 05:06:34.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/notes/success_response.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-02-06 12:22:43.261108 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/notification/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      522 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/notification/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      138 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/notification/action_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      140 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/notification/action_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2052 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/notification/action_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3951 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/notification/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1893 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/notification/body_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3585 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/notification/info.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     8186 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/notification/notification.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     8156 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/notification/notification_operations.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/notification/response_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2671 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/notification/response_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3663 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/notification/success_response.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-02-06 12:22:43.265107 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/org/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      376 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/org/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      140 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/org/action_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3791 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/org/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1971 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/org/file_body_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     5172 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/org/license_details.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)    19917 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/org/org.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2317 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/org/org_operations.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/org/response_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2029 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/org/response_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3654 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/org/success_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      454 2023-02-01 13:00:28.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/param.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1817 2023-02-01 13:00:28.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/parameter_map.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-02-06 12:22:43.265107 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/profiles/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      358 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/profiles/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3658 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/profiles/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3243 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/profiles/category.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     4121 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/profiles/permission_detail.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     9210 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/profiles/profile.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2799 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/profiles/profiles_operations.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/profiles/response_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2104 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/profiles/response_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2463 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/profiles/section.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-02-06 12:22:43.265107 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/query/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      216 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/query/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3655 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/query/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2031 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/query/body_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1589 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/query/query_operations.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/query/response_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2642 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/query/response_wrapper.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-02-06 12:22:43.273106 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/record/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2754 2023-02-06 11:57:43.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/record/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      138 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/record/action_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      140 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/record/action_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2032 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/record/action_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     5482 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/record/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1923 2023-02-06 11:57:43.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/record/apply_feature_execution.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     5561 2023-02-06 11:57:43.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/record/body_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2977 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/record/carry_over_tags.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3854 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/record/comment.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     7057 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/record/consent.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      152 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/record/convert_action_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      154 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/record/convert_action_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2083 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/record/convert_action_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1893 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/record/convert_body_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     4015 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/record/criteria.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     5020 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/record/deleted_record.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      154 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/record/deleted_records_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2689 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/record/deleted_records_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/record/download_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)    36464 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/record/field.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2276 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/record/file_body_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)    10456 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/record/file_details.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      134 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/record/file_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3585 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/record/info.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     7930 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/record/inventory_line_items.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     6709 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/record/lead_converter.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2041 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/record/line_item_product.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3489 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/record/line_tax.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     4693 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/record/mass_update.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      158 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/record/mass_update_action_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      160 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/record/mass_update_action_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2106 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/record/mass_update_action_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     4734 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/record/mass_update_body_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      148 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/record/mass_update_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      162 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/record/mass_update_response_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2120 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/record/mass_update_response_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3731 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/record/mass_update_success_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      306 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/record/options.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3489 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/record/participants.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2067 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/record/pricing_details.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     6385 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/record/record.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)    40904 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/record/record_operations.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1931 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/record/recurring_activity.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1913 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/record/remind_at.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2437 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/record/reminder.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/record/response_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2645 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/record/response_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     4991 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/record/success_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3266 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/record/successful_convert.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2503 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/record/territory.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-02-06 12:22:43.273106 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/related_lists/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      274 2023-02-03 05:06:34.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/related_lists/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3663 2023-02-03 05:06:34.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/related_lists/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     7709 2023-02-03 05:06:34.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/related_lists/related_list.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2702 2023-02-03 05:06:34.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/related_lists/related_lists_operations.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-02-03 05:06:34.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/related_lists/response_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2179 2023-02-03 05:06:34.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/related_lists/response_wrapper.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-02-06 12:22:43.273106 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/related_records/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      975 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/related_records/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      138 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/related_records/action_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      140 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/related_records/action_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2041 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/related_records/action_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3960 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/related_records/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1879 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/related_records/body_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2139 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/related_records/file_body_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)    26530 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/related_records/related_records_operations.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/related_records/response_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2652 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/related_records/response_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3666 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/related_records/success_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1858 2023-02-01 13:00:28.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/request_proxy.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-02-06 12:22:43.277105 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/roles/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      201 2023-02-03 05:06:34.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/roles/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3655 2023-02-03 05:06:34.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/roles/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-02-03 05:06:34.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/roles/response_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2059 2023-02-03 05:06:34.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/roles/response_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     6389 2023-02-03 05:06:34.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/roles/role.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1938 2023-02-03 05:06:34.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/roles/roles_operations.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1753 2023-02-01 13:00:28.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/sdk_config.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-02-06 12:22:43.277105 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/share_records/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      681 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/share_records/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      138 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/share_records/action_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      140 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/share_records/action_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2053 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/share_records/action_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     4309 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/share_records/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1893 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/share_records/body_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      150 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/share_records/delete_action_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      152 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/share_records/delete_action_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2383 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/share_records/delete_action_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/share_records/response_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2691 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/share_records/response_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     5510 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/share_records/share_record.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     6226 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/share_records/share_records_operations.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3128 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/share_records/shared_through.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3844 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/share_records/success_response.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-02-06 12:22:43.281104 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/tags/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      972 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/tags/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      138 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/tags/action_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      140 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/tags/action_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2030 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/tags/action_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     4393 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/tags/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1879 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/tags/body_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2023 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/tags/conflict_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      136 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/tags/count_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2063 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/tags/count_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2537 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/tags/info.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1881 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/tags/merge_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      150 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/tags/record_action_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      152 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/tags/record_action_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3982 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/tags/record_action_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/tags/response_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2641 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/tags/response_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3826 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/tags/success_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     5045 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/tags/tag.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)    17611 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/tags/tags_operations.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-02-06 12:22:43.281104 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/taxes/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      464 2023-02-03 05:06:34.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/taxes/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      138 2023-02-03 05:06:34.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/taxes/action_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      140 2023-02-03 05:06:34.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/taxes/action_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2045 2023-02-03 05:06:34.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/taxes/action_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3930 2023-02-03 05:06:34.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/taxes/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1893 2023-02-03 05:06:34.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/taxes/body_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2797 2023-02-03 05:06:34.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/taxes/preference.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-02-03 05:06:34.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/taxes/response_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2801 2023-02-03 05:06:34.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/taxes/response_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3656 2023-02-03 05:06:34.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/taxes/success_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     4203 2023-02-03 05:06:34.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/taxes/tax.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     6502 2023-02-03 05:06:34.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/taxes/taxes_operations.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-02-06 12:22:43.281104 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/territories/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      223 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/territories/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3661 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/territories/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/territories/response_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2149 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/territories/response_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1996 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/territories/territories_operations.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     7598 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/territories/territory.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1145 2023-02-01 13:00:28.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/user_signature.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-02-06 12:22:43.285103 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/users/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      683 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/users/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      138 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/users/action_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      140 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/users/action_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2045 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/users/action_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3930 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/users/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1893 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/users/body_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     5245 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/users/customize_info.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3585 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/users/info.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1899 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/users/request_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/users/response_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2657 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/users/response_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2357 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/users/shift.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3656 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/users/success_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2597 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/users/tab_theme.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2915 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/users/territory.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     5179 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/users/theme.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)    22393 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/users/user.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     8391 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/users/users_operations.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-02-06 12:22:43.289102 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/util/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      630 2023-02-01 13:00:28.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/util/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     6404 2023-02-01 13:00:28.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/util/api_http_connector.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1348 2023-02-01 13:00:28.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/util/api_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      245 2023-02-01 13:00:28.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/util/choice.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)    15313 2023-02-01 13:00:28.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/util/common_api_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)    14708 2023-02-06 11:57:43.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/util/constants.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)    10545 2023-02-01 13:00:28.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/util/converter.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     4275 2023-02-01 13:00:28.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/util/datatype_converter.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3348 2023-02-01 13:00:28.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/util/downloader.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     6752 2023-02-01 13:00:28.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/util/form_data_converter.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3468 2023-02-01 13:00:28.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/util/header_param_validator.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)    30812 2023-02-01 13:00:28.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/util/json_converter.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     5315 2023-02-01 13:00:28.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/util/module_fields_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1531 2023-02-01 13:00:28.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/util/stream_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)    37802 2023-02-01 13:00:28.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/util/utility.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      972 2023-02-01 13:00:28.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/util/xml_converter.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-02-06 12:22:43.289102 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/variable_groups/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      239 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/variable_groups/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3665 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/variable_groups/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/variable_groups/response_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2209 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/variable_groups/response_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     4217 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/variable_groups/variable_group.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3038 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/variable_groups/variable_groups_operations.py
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-02-06 12:22:43.289102 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/variables/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      520 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/variables/__init__.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      138 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/variables/action_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      140 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/variables/action_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2105 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/variables/action_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3942 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/variables/api_exception.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     1949 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/variables/body_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)      142 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/variables/response_handler.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     2119 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/variables/response_wrapper.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     3660 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/variables/success_response.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)     5261 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/variables/variable.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)    11815 2023-02-03 05:06:35.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/variables/variables_operations.py
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)   145217 2023-02-06 11:57:43.000000 zohocrmsdk2_0-5.1.0/zcrmsdk/src/json_details.json
-drwxr-xr-x   0 tharun-15510 (618246689) domain^users (618136065)        0 2023-02-06 12:22:43.289102 zohocrmsdk2_0-5.1.0/zohocrmsdk2_0.egg-info/
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)    42288 2023-02-06 12:22:43.000000 zohocrmsdk2_0-5.1.0/zohocrmsdk2_0.egg-info/PKG-INFO
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)    22760 2023-02-06 12:22:43.000000 zohocrmsdk2_0-5.1.0/zohocrmsdk2_0.egg-info/SOURCES.txt
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)        1 2023-02-06 12:22:43.000000 zohocrmsdk2_0-5.1.0/zohocrmsdk2_0.egg-info/dependency_links.txt
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)       33 2023-02-06 12:22:43.000000 zohocrmsdk2_0-5.1.0/zohocrmsdk2_0.egg-info/requires.txt
--rw-r--r--   0 tharun-15510 (618246689) domain^users (618136065)        8 2023-02-06 12:22:43.000000 zohocrmsdk2_0-5.1.0/zohocrmsdk2_0.egg-info/top_level.txt
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-16 13:25:52.570916 zohocrmsdk2_0-6.0.0/
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)    11358 2021-12-22 14:20:01.000000 zohocrmsdk2_0-6.0.0/LICENSE
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      103 2024-04-16 13:20:09.000000 zohocrmsdk2_0-6.0.0/MANIFEST.in
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)    42430 2024-04-16 13:25:52.570674 zohocrmsdk2_0-6.0.0/PKG-INFO
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)    41282 2022-03-31 06:05:43.000000 zohocrmsdk2_0-6.0.0/README.md
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)       67 2024-04-16 13:25:52.571340 zohocrmsdk2_0-6.0.0/setup.cfg
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1640 2024-04-16 13:20:27.000000 zohocrmsdk2_0-6.0.0/setup.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-16 13:25:52.309330 zohocrmsdk2_0-6.0.0/zcrmsdk/
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)       17 2021-08-10 06:28:43.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/__init__.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-16 13:25:52.310295 zohocrmsdk2_0-6.0.0/zcrmsdk/src/
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)       17 2021-08-10 06:28:43.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/__init__.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-16 13:25:52.311538 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)       18 2021-08-10 06:28:43.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/__init__.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-16 13:25:52.312031 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)       35 2021-08-10 06:28:43.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/__init__.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-16 13:25:52.312526 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/api/
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)       49 2021-08-10 06:28:43.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/api/__init__.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-16 13:25:52.314135 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/api/authenticator/
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)       81 2021-08-10 06:28:43.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/api/authenticator/__init__.py
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)    12677 2021-09-03 12:40:17.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/api/authenticator/oauth_token.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-16 13:25:52.317675 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/api/authenticator/store/
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      100 2021-08-10 06:28:43.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/api/authenticator/store/__init__.py
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)    11429 2021-09-03 05:34:50.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/api/authenticator/store/db_store.py
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     8998 2021-08-10 06:28:43.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/api/authenticator/store/file_store.py
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1969 2021-08-10 06:28:43.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/api/authenticator/store/token_store.py
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      665 2021-08-10 06:28:43.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/api/authenticator/token.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-16 13:25:52.318692 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/api/logger/
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)       39 2021-08-10 06:28:43.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/api/logger/__init__.py
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2815 2021-08-10 06:28:43.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/api/logger/logger.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-16 13:25:52.318988 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)       17 2021-08-10 06:28:43.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/__init__.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-16 13:25:52.324107 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      984 2021-08-10 06:28:43.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/__init__.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-16 13:25:52.332379 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/attachments/
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      518 2024-04-16 13:24:22.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/attachments/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      138 2024-04-16 13:24:21.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/attachments/action_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      140 2024-04-16 13:24:21.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/attachments/action_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2037 2024-04-16 13:24:21.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/attachments/action_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3948 2024-04-16 13:24:21.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/attachments/api_exception.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)    11441 2024-04-16 13:24:21.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/attachments/attachment.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     8807 2024-04-16 13:24:22.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/attachments/attachments_operations.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2135 2024-04-16 13:24:22.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/attachments/file_body_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-16 13:24:21.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/attachments/response_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2648 2024-04-16 13:24:22.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/attachments/response_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3662 2024-04-16 13:24:21.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/attachments/success_response.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-16 13:25:52.345213 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/blue_print/
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      512 2024-04-16 13:24:22.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/blue_print/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      140 2024-04-16 13:24:22.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/blue_print/action_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3805 2024-04-16 13:24:22.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/blue_print/api_exception.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     4015 2024-04-16 13:24:22.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/blue_print/blue_print.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3177 2024-04-16 13:24:22.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/blue_print/blue_print_operations.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1949 2024-04-16 13:24:22.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/blue_print/body_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2375 2024-04-16 13:24:22.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/blue_print/next_transition.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     7825 2024-04-16 13:24:22.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/blue_print/process_info.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-16 13:24:22.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/blue_print/response_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2291 2024-04-16 13:24:22.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/blue_print/response_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3661 2024-04-16 13:24:22.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/blue_print/success_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     8191 2024-04-16 13:24:22.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/blue_print/transition.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2531 2024-04-16 13:24:22.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/blue_print/validation_error.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-16 13:25:52.354384 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/bulk_read/
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      599 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/bulk_read/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      138 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/bulk_read/action_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      140 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/bulk_read/action_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2519 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/bulk_read/action_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3942 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/bulk_read/api_exception.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3544 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/bulk_read/bulk_read_operations.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2421 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/bulk_read/call_back.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     4063 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/bulk_read/criteria.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2133 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/bulk_read/file_body_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     6167 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/bulk_read/job_detail.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     4139 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/bulk_read/query.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3309 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/bulk_read/request_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/bulk_read/response_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2049 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/bulk_read/response_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     4225 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/bulk_read/result.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3660 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/bulk_read/success_response.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-16 13:25:52.365300 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/bulk_write/
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      590 2024-04-16 13:24:22.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/bulk_write/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      140 2024-04-16 13:24:22.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/bulk_write/action_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     7349 2024-04-16 13:24:22.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/bulk_write/api_exception.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     5548 2024-04-16 13:24:22.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/bulk_write/bulk_write_operations.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     7120 2024-04-16 13:24:22.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/bulk_write/bulk_write_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2421 2024-04-16 13:24:22.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/bulk_write/call_back.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     4729 2024-04-16 13:24:22.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/bulk_write/field_mapping.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     4933 2024-04-16 13:24:22.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/bulk_write/file.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2134 2024-04-16 13:24:22.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/bulk_write/file_body_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     4586 2024-04-16 13:24:22.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/bulk_write/request_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     5934 2024-04-16 13:24:22.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/bulk_write/resource.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-16 13:24:22.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/bulk_write/response_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-16 13:24:22.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/bulk_write/response_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2021 2024-04-16 13:24:22.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/bulk_write/result.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3661 2024-04-16 13:24:22.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/bulk_write/success_response.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-16 13:25:52.373472 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/contact_roles/
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      831 2024-04-16 13:24:24.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/contact_roles/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      138 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/contact_roles/action_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      140 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/contact_roles/action_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2165 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/contact_roles/action_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     4314 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/contact_roles/api_exception.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2005 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/contact_roles/body_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3043 2024-04-16 13:24:24.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/contact_roles/contact_role.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2045 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/contact_roles/contact_role_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)    14167 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/contact_roles/contact_roles_operations.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      150 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/contact_roles/record_action_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2083 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/contact_roles/record_action_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1891 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/contact_roles/record_body_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      154 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/contact_roles/record_response_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2694 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/contact_roles/record_response_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/contact_roles/response_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2179 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/contact_roles/response_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3664 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/contact_roles/success_response.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-16 13:25:52.380322 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/currencies/
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      649 2024-04-16 13:24:24.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/currencies/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      138 2024-04-16 13:24:24.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/currencies/action_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      140 2024-04-16 13:24:24.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/currencies/action_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2120 2024-04-16 13:24:24.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/currencies/action_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     4149 2024-04-16 13:24:24.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/currencies/api_exception.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      162 2024-04-16 13:24:24.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/currencies/base_currency_action_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2471 2024-04-16 13:24:24.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/currencies/base_currency_action_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2180 2024-04-16 13:24:24.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/currencies/base_currency_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1963 2024-04-16 13:24:24.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/currencies/body_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     8572 2024-04-16 13:24:24.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/currencies/currencies_operations.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     9248 2024-04-16 13:24:24.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/currencies/currency.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3407 2024-04-16 13:24:24.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/currencies/format.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-16 13:24:24.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/currencies/response_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2134 2024-04-16 13:24:24.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/currencies/response_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3661 2024-04-16 13:24:24.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/currencies/success_response.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-16 13:25:52.385603 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/custom_views/
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      426 2024-04-16 13:24:22.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/custom_views/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3662 2024-04-16 13:24:22.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/custom_views/api_exception.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     4015 2024-04-16 13:24:22.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/custom_views/criteria.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)    10152 2024-04-16 13:24:22.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/custom_views/custom_view.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3288 2024-04-16 13:24:22.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/custom_views/custom_views_operations.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     4914 2024-04-16 13:24:22.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/custom_views/info.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2369 2024-04-16 13:24:22.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/custom_views/range.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-16 13:24:22.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/custom_views/response_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2769 2024-04-16 13:24:22.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/custom_views/response_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3511 2024-04-16 13:24:22.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/custom_views/shared_details.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     4067 2024-04-16 13:24:22.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/custom_views/translation.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-16 13:25:52.388660 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/dc/
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      282 2022-03-30 14:24:58.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/dc/__init__.py
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1410 2021-08-10 06:28:43.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/dc/au_data_center.py
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1399 2021-08-10 06:28:43.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/dc/cn_data_center.py
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1124 2021-08-10 06:28:43.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/dc/data_center.py
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1381 2021-08-10 06:28:43.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/dc/eu_data_center.py
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1379 2021-08-10 06:28:43.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/dc/in_data_center.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1402 2022-03-30 14:24:28.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/dc/jp_data_center.py
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1384 2021-08-10 06:28:43.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/dc/us_data_center.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-16 13:25:52.389445 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/exception/
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)       40 2021-08-10 06:28:43.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/exception/__init__.py
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1157 2021-08-10 06:28:43.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/exception/sdk_exception.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-16 13:25:52.401251 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/fields/
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      730 2024-04-16 13:24:24.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/fields/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3656 2024-04-16 13:24:24.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/fields/api_exception.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2989 2024-04-16 13:24:24.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/fields/association_details.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3099 2024-04-16 13:24:24.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/fields/auto_number.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     4579 2024-04-16 13:24:24.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/fields/crypt.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2651 2024-04-16 13:24:24.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/fields/currency.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)    32964 2024-04-16 13:24:24.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/fields/field.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3108 2024-04-16 13:24:24.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/fields/fields_operations.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2611 2024-04-16 13:24:24.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/fields/formula.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2369 2024-04-16 13:24:24.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/fields/lookup_field.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     4878 2024-04-16 13:24:24.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/fields/module.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     5245 2024-04-16 13:24:24.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/fields/multi_select_lookup.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     5721 2024-04-16 13:24:24.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/fields/pick_list_value.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3027 2024-04-16 13:24:24.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/fields/private.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     4247 2024-04-16 13:24:24.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/fields/related_details.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-16 13:24:24.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/fields/response_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2074 2024-04-16 13:24:24.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/fields/response_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2419 2024-04-16 13:24:24.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/fields/tool_tip.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2037 2024-04-16 13:24:24.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/fields/unique.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3557 2024-04-16 13:24:24.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/fields/view_type.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-16 13:25:52.409050 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/file/
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      421 2024-04-16 13:24:22.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/file/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      138 2024-04-16 13:24:22.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/file/action_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      140 2024-04-16 13:24:22.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/file/action_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2030 2024-04-16 13:24:22.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/file/action_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3927 2024-04-16 13:24:22.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/file/api_exception.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1909 2024-04-16 13:24:22.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/file/body_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2128 2024-04-16 13:24:22.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/file/file_body_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3288 2024-04-16 13:24:22.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/file/file_operations.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-16 13:24:22.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/file/response_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3655 2024-04-16 13:24:22.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/file/success_response.py
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      447 2021-08-10 06:28:43.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/header.py
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1796 2021-08-10 06:28:43.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/header_map.py
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)    11164 2021-12-22 14:21:16.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/initializer.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-16 13:25:52.412716 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/layouts/
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      306 2024-04-16 13:24:22.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/layouts/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3657 2024-04-16 13:24:22.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/layouts/api_exception.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     8542 2024-04-16 13:24:22.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/layouts/layout.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2614 2024-04-16 13:24:22.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/layouts/layouts_operations.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3312 2024-04-16 13:24:22.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/layouts/properties.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-16 13:24:22.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/layouts/response_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2089 2024-04-16 13:24:22.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/layouts/response_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     7679 2024-04-16 13:24:22.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/layouts/section.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-16 13:25:52.426870 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/modules/
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      562 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/modules/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      138 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/modules/action_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      140 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/modules/action_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2075 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/modules/action_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3936 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/modules/api_exception.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2421 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/modules/argument.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1921 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/modules/body_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)    30518 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/modules/module.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     5464 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/modules/modules_operations.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3087 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/modules/related_list_properties.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/modules/response_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2089 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/modules/response_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3658 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/modules/success_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2995 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/modules/territory.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-16 13:25:52.444058 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/notes/
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      514 2024-04-16 13:24:22.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/notes/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      138 2024-04-16 13:24:22.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/notes/action_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      140 2024-04-16 13:24:22.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/notes/action_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2031 2024-04-16 13:24:22.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/notes/action_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3930 2024-04-16 13:24:22.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/notes/api_exception.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1879 2024-04-16 13:24:22.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/notes/body_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3585 2024-04-16 13:24:22.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/notes/info.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)    11186 2024-04-16 13:24:22.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/notes/note.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     9892 2024-04-16 13:24:22.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/notes/notes_operations.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-16 13:24:22.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/notes/response_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2643 2024-04-16 13:24:22.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/notes/response_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3656 2024-04-16 13:24:22.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/notes/success_response.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-16 13:25:52.453530 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/notification/
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      522 2024-04-16 13:24:22.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/notification/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      138 2024-04-16 13:24:22.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/notification/action_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      140 2024-04-16 13:24:22.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/notification/action_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2052 2024-04-16 13:24:22.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/notification/action_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3951 2024-04-16 13:24:22.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/notification/api_exception.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1893 2024-04-16 13:24:22.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/notification/body_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3585 2024-04-16 13:24:22.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/notification/info.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     8186 2024-04-16 13:24:22.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/notification/notification.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     8156 2024-04-16 13:24:22.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/notification/notification_operations.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-16 13:24:22.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/notification/response_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2671 2024-04-16 13:24:22.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/notification/response_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3663 2024-04-16 13:24:22.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/notification/success_response.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-16 13:25:52.459830 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/org/
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      376 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/org/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      140 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/org/action_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3791 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/org/api_exception.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1971 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/org/file_body_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     5172 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/org/license_details.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)    19917 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/org/org.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2317 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/org/org_operations.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/org/response_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2029 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/org/response_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3654 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/org/success_response.py
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      454 2021-08-10 06:28:43.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/param.py
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1817 2021-08-10 06:28:43.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/parameter_map.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-16 13:25:52.464273 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/profiles/
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      358 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/profiles/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3658 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/profiles/api_exception.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3243 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/profiles/category.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     4121 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/profiles/permission_detail.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     9210 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/profiles/profile.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2799 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/profiles/profiles_operations.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/profiles/response_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2104 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/profiles/response_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2463 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/profiles/section.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-16 13:25:52.467860 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/query/
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      216 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/query/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3655 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/query/api_exception.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2031 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/query/body_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1589 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/query/query_operations.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/query/response_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2642 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/query/response_wrapper.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-16 13:25:52.498678 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/record/
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2754 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/record/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      138 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/record/action_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      140 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/record/action_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2032 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/record/action_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     5482 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/record/api_exception.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1923 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/record/apply_feature_execution.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     5561 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/record/body_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2977 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/record/carry_over_tags.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3854 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/record/comment.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     7057 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/record/consent.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      152 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/record/convert_action_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      154 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/record/convert_action_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2083 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/record/convert_action_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1893 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/record/convert_body_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     4015 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/record/criteria.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     5020 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/record/deleted_record.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      154 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/record/deleted_records_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2689 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/record/deleted_records_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/record/download_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)    36464 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/record/field.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2276 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/record/file_body_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)    10456 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/record/file_details.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      134 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/record/file_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3585 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/record/info.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     7930 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/record/inventory_line_items.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     6709 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/record/lead_converter.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2041 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/record/line_item_product.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3489 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/record/line_tax.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     4693 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/record/mass_update.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      158 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/record/mass_update_action_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      160 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/record/mass_update_action_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2106 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/record/mass_update_action_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     4734 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/record/mass_update_body_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      148 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/record/mass_update_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      162 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/record/mass_update_response_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2120 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/record/mass_update_response_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3731 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/record/mass_update_success_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      306 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/record/options.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3489 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/record/participants.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2067 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/record/pricing_details.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     6385 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/record/record.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)    40904 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/record/record_operations.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1931 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/record/recurring_activity.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1913 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/record/remind_at.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2437 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/record/reminder.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/record/response_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2645 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/record/response_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     4991 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/record/success_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3266 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/record/successful_convert.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2503 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/record/territory.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-16 13:25:52.500833 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/related_lists/
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      274 2024-04-16 13:24:22.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/related_lists/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3663 2024-04-16 13:24:22.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/related_lists/api_exception.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     7709 2024-04-16 13:24:22.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/related_lists/related_list.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2702 2024-04-16 13:24:22.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/related_lists/related_lists_operations.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-16 13:24:22.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/related_lists/response_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2179 2024-04-16 13:24:22.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/related_lists/response_wrapper.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-16 13:25:52.505443 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/related_records/
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      975 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/related_records/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      138 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/related_records/action_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      140 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/related_records/action_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2041 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/related_records/action_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3960 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/related_records/api_exception.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1879 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/related_records/body_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2139 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/related_records/file_body_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)    26530 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/related_records/related_records_operations.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/related_records/response_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2652 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/related_records/response_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3666 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/related_records/success_response.py
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1858 2021-08-10 06:28:43.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/request_proxy.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-16 13:25:52.512051 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/roles/
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      201 2024-04-16 13:24:22.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/roles/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3655 2024-04-16 13:24:22.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/roles/api_exception.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-16 13:24:22.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/roles/response_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2059 2024-04-16 13:24:22.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/roles/response_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     6389 2024-04-16 13:24:22.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/roles/role.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1938 2024-04-16 13:24:22.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/roles/roles_operations.py
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1753 2021-08-10 06:28:43.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/sdk_config.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-16 13:25:52.520388 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/share_records/
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      681 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/share_records/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      138 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/share_records/action_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      140 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/share_records/action_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2053 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/share_records/action_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     4309 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/share_records/api_exception.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1893 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/share_records/body_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      150 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/share_records/delete_action_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      152 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/share_records/delete_action_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2383 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/share_records/delete_action_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/share_records/response_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2691 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/share_records/response_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     5510 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/share_records/share_record.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     6226 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/share_records/share_records_operations.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3128 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/share_records/shared_through.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3844 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/share_records/success_response.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-16 13:25:52.530121 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/tags/
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      972 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/tags/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      138 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/tags/action_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      140 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/tags/action_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2030 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/tags/action_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     4393 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/tags/api_exception.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1879 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/tags/body_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2023 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/tags/conflict_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      136 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/tags/count_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2063 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/tags/count_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2537 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/tags/info.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1881 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/tags/merge_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      150 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/tags/record_action_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      152 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/tags/record_action_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3982 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/tags/record_action_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/tags/response_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2641 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/tags/response_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3826 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/tags/success_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     5045 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/tags/tag.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)    17611 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/tags/tags_operations.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-16 13:25:52.536477 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/taxes/
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      464 2024-04-16 13:24:22.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/taxes/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      138 2024-04-16 13:24:22.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/taxes/action_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      140 2024-04-16 13:24:22.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/taxes/action_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2045 2024-04-16 13:24:22.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/taxes/action_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3930 2024-04-16 13:24:22.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/taxes/api_exception.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1893 2024-04-16 13:24:22.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/taxes/body_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2797 2024-04-16 13:24:22.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/taxes/preference.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-16 13:24:22.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/taxes/response_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2801 2024-04-16 13:24:22.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/taxes/response_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3656 2024-04-16 13:24:22.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/taxes/success_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     4203 2024-04-16 13:24:22.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/taxes/tax.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     6502 2024-04-16 13:24:22.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/taxes/taxes_operations.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-16 13:25:52.539247 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/territories/
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      223 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/territories/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3661 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/territories/api_exception.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/territories/response_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2149 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/territories/response_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1996 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/territories/territories_operations.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     7598 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/territories/territory.py
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1145 2021-08-10 06:28:43.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/user_signature.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-16 13:25:52.548803 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/users/
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      683 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/users/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      138 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/users/action_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      140 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/users/action_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2045 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/users/action_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3930 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/users/api_exception.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1893 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/users/body_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     5245 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/users/customize_info.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3585 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/users/info.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1899 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/users/request_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/users/response_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2657 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/users/response_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2357 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/users/shift.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3656 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/users/success_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2597 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/users/tab_theme.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2915 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/users/territory.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     5179 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/users/theme.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)    22393 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/users/user.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     8391 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/users/users_operations.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-16 13:25:52.556933 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/util/
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      630 2021-08-10 06:28:43.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/util/__init__.py
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     6404 2021-08-10 06:28:43.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/util/api_http_connector.py
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1348 2021-08-10 06:28:43.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/util/api_response.py
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      245 2021-08-10 06:28:43.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/util/choice.py
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)    15313 2021-08-10 06:31:43.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/util/common_api_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)    14708 2024-04-16 13:23:35.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/util/constants.py
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)    10545 2021-08-10 06:28:43.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/util/converter.py
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     4275 2021-08-10 06:28:43.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/util/datatype_converter.py
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3348 2021-08-10 06:28:43.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/util/downloader.py
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     6752 2021-08-10 06:28:43.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/util/form_data_converter.py
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3468 2021-08-10 06:28:43.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/util/header_param_validator.py
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)    30812 2021-08-10 06:28:43.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/util/json_converter.py
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     5315 2021-08-10 06:28:43.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/util/module_fields_handler.py
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1531 2021-08-10 06:28:43.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/util/stream_wrapper.py
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)    37802 2022-03-31 06:01:29.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/util/utility.py
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      972 2021-08-10 06:28:43.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/util/xml_converter.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-16 13:25:52.560509 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/variable_groups/
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      239 2024-04-16 13:24:24.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/variable_groups/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3665 2024-04-16 13:24:24.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/variable_groups/api_exception.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-16 13:24:24.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/variable_groups/response_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2209 2024-04-16 13:24:24.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/variable_groups/response_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     4217 2024-04-16 13:24:24.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/variable_groups/variable_group.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3038 2024-04-16 13:24:24.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/variable_groups/variable_groups_operations.py
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-16 13:25:52.564446 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/variables/
+-rwxrwxrwx   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      520 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/variables/__init__.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      138 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/variables/action_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      140 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/variables/action_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2105 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/variables/action_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3942 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/variables/api_exception.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     1949 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/variables/body_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)      142 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/variables/response_handler.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     2119 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/variables/response_wrapper.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     3660 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/variables/success_response.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)     5261 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/variables/variable.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)    11815 2024-04-16 13:24:23.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/variables/variables_operations.py
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)   145273 2024-04-16 13:24:24.000000 zohocrmsdk2_0-6.0.0/zcrmsdk/src/json_details.json
+drwxr-xr-x   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        0 2024-04-16 13:25:52.569965 zohocrmsdk2_0-6.0.0/zohocrmsdk2_0.egg-info/
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)    42430 2024-04-16 13:25:52.000000 zohocrmsdk2_0-6.0.0/zohocrmsdk2_0.egg-info/PKG-INFO
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)    22760 2024-04-16 13:25:52.000000 zohocrmsdk2_0-6.0.0/zohocrmsdk2_0.egg-info/SOURCES.txt
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        1 2024-04-16 13:25:52.000000 zohocrmsdk2_0-6.0.0/zohocrmsdk2_0.egg-info/dependency_links.txt
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)       67 2024-04-16 13:25:52.000000 zohocrmsdk2_0-6.0.0/zohocrmsdk2_0.egg-info/requires.txt
+-rw-r--r--   0 raja-7453 (732579735) ZOHOCORP\Domain Users (884470207)        8 2024-04-16 13:25:52.000000 zohocrmsdk2_0-6.0.0/zohocrmsdk2_0.egg-info/top_level.txt
```

### Comparing `zohocrmsdk2_0-5.1.0/LICENSE` & `zohocrmsdk2_0-6.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/PKG-INFO` & `zohocrmsdk2_0-6.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zohocrmsdk2_0
-Version: 5.1.0
+Version: 6.0.0
 Summary: Zoho CRM SDK for Python developers
 Home-page: https://github.com/zoho/zohocrm-python-sdk-2.0
 Author: Zoho CRM API Team
 Author-email: support@zohocrm.com
 License: Apache Software License, Version 2.0, http://www.apache.org/licenses/LICENSE-2.0
 Keywords: development,zoho,crm,api,zcrmsdk,sdk,zcrm,zohocrmsdk2_0
 Classifier: Development Status :: 5 - Production/Stable
@@ -16,14 +16,19 @@
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: requests
+Requires-Dist: python-dateutil
+Requires-Dist: urllib3
+Requires-Dist: mysql-connector-python
+Requires-Dist: setuptools
 
 #  ZOHO CRM PYTHON SDK 2.0
 
 ## Table Of Contents
 
 * [Overview](#overview)
 * [Registering a Zoho Client](#registering-a-zoho-client)
```

### Comparing `zohocrmsdk2_0-5.1.0/README.md` & `zohocrmsdk2_0-6.0.0/README.md`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/setup.py` & `zohocrmsdk2_0-6.0.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 # Get the long description from the README file
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='zohocrmsdk2_0',
-    version='5.1.0',
+    version='6.0.0',
     description='Zoho CRM SDK for Python developers',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/zoho/zohocrm-python-sdk-2.0',
     author='Zoho CRM API Team',
     author_email='support@zohocrm.com',
     scripts=[],
@@ -31,14 +31,16 @@
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
     ],
     install_requires=[
         'requests',
         'python-dateutil',
-        'urllib3'
+        'urllib3',
+        'mysql-connector-python',
+        'setuptools'
     ],
     keywords=['development', 'zoho', 'crm', 'api', 'zcrmsdk', 'sdk', 'zcrm','zohocrmsdk2_0'],
     packages=find_packages(),
     include_package_data=True,
     license='Apache Software License, Version 2.0, http://www.apache.org/licenses/LICENSE-2.0',
 )
```

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/api/authenticator/oauth_token.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/api/authenticator/oauth_token.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/api/authenticator/store/db_store.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/api/authenticator/store/db_store.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/api/authenticator/store/file_store.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/api/authenticator/store/file_store.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/api/authenticator/store/token_store.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/api/authenticator/store/token_store.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/api/authenticator/token.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/api/authenticator/token.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/api/logger/logger.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/api/logger/logger.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/__init__.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/__init__.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/attachments/__init__.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/attachments/__init__.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/attachments/action_wrapper.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/attachments/action_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/attachments/api_exception.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/attachments/api_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/attachments/attachment.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/attachments/attachment.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/attachments/attachments_operations.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/attachments/attachments_operations.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/attachments/file_body_wrapper.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/attachments/file_body_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/attachments/response_wrapper.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/attachments/response_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/attachments/success_response.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/attachments/success_response.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/blue_print/__init__.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/blue_print/__init__.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/blue_print/api_exception.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/blue_print/api_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/blue_print/blue_print.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/blue_print/blue_print.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/blue_print/blue_print_operations.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/blue_print/blue_print_operations.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/blue_print/body_wrapper.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/blue_print/body_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/blue_print/next_transition.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/blue_print/next_transition.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/blue_print/process_info.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/blue_print/process_info.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/blue_print/response_wrapper.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/blue_print/response_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/blue_print/success_response.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/blue_print/success_response.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/blue_print/transition.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/blue_print/transition.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/blue_print/validation_error.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/blue_print/validation_error.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/bulk_read/__init__.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/bulk_read/__init__.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/bulk_read/action_wrapper.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/bulk_read/action_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/bulk_read/api_exception.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/bulk_read/api_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/bulk_read/bulk_read_operations.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/bulk_read/bulk_read_operations.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/bulk_read/call_back.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/bulk_read/call_back.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/bulk_read/criteria.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/bulk_read/criteria.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/bulk_read/file_body_wrapper.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/bulk_read/file_body_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/bulk_read/job_detail.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/bulk_read/job_detail.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/bulk_read/query.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/bulk_read/query.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/bulk_read/request_wrapper.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/bulk_read/request_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/bulk_read/response_wrapper.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/bulk_read/response_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/bulk_read/result.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/bulk_read/result.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/bulk_read/success_response.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/bulk_read/success_response.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/bulk_write/__init__.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/bulk_write/__init__.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/bulk_write/api_exception.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/bulk_write/api_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/bulk_write/bulk_write_operations.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/bulk_write/bulk_write_operations.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/bulk_write/bulk_write_response.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/bulk_write/bulk_write_response.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/bulk_write/call_back.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/bulk_write/call_back.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/bulk_write/field_mapping.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/bulk_write/field_mapping.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/bulk_write/file.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/bulk_write/file.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/bulk_write/file_body_wrapper.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/bulk_write/file_body_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/bulk_write/request_wrapper.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/bulk_write/request_wrapper.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 	def __init__(self):
 		"""Creates an instance of RequestWrapper"""
 
 		self.__character_encoding = None
 		self.__operation = None
 		self.__callback = None
 		self.__resource = None
+		self.__ignore_empty = None
 		self.__key_modified = dict()
 
 	def get_character_encoding(self):
 		"""
 		The method to get the character_encoding
 
 		Returns:
@@ -113,14 +114,38 @@
 
 		if resource is not None and not isinstance(resource, list):
 			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: resource EXPECTED TYPE: list', None, None)
 		
 		self.__resource = resource
 		self.__key_modified['resource'] = 1
 
+	def get_ignore_empty(self):
+		"""
+		The method to get the ignore_empty
+
+		Returns:
+			bool: A bool representing the ignore_empty
+		"""
+
+		return self.__ignore_empty
+
+	def set_ignore_empty(self, ignore_empty):
+		"""
+		The method to set the value to ignore_empty
+
+		Parameters:
+			ignore_empty (bool) : A bool representing the ignore_empty
+		"""
+
+		if ignore_empty is not None and not isinstance(ignore_empty, bool):
+			raise SDKException(Constants.DATA_TYPE_ERROR, 'KEY: ignore_empty EXPECTED TYPE: bool', None, None)
+		
+		self.__ignore_empty = ignore_empty
+		self.__key_modified['ignore_empty'] = 1
+
 	def is_key_modified(self, key):
 		"""
 		The method to check if the user has modified the given key
 
 		Parameters:
 			key (string) : A string representing the key
```

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/bulk_write/resource.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/bulk_write/resource.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/bulk_write/result.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/bulk_write/result.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/bulk_write/success_response.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/bulk_write/success_response.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/contact_roles/__init__.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/contact_roles/__init__.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/contact_roles/action_wrapper.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/contact_roles/action_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/contact_roles/api_exception.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/contact_roles/api_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/contact_roles/body_wrapper.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/contact_roles/body_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/contact_roles/contact_role.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/contact_roles/contact_role.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/contact_roles/contact_role_wrapper.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/contact_roles/contact_role_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/contact_roles/contact_roles_operations.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/contact_roles/contact_roles_operations.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/contact_roles/record_action_wrapper.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/contact_roles/record_action_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/contact_roles/record_body_wrapper.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/contact_roles/record_body_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/contact_roles/record_response_wrapper.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/contact_roles/record_response_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/contact_roles/response_wrapper.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/contact_roles/response_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/contact_roles/success_response.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/contact_roles/success_response.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/currencies/__init__.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/currencies/__init__.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/currencies/action_wrapper.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/currencies/action_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/currencies/api_exception.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/currencies/api_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/currencies/base_currency_action_wrapper.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/currencies/base_currency_action_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/currencies/base_currency_wrapper.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/currencies/base_currency_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/currencies/body_wrapper.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/currencies/body_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/currencies/currencies_operations.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/currencies/currencies_operations.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/currencies/currency.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/currencies/currency.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/currencies/format.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/currencies/format.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/currencies/response_wrapper.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/currencies/response_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/currencies/success_response.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/currencies/success_response.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/custom_views/api_exception.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/custom_views/api_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/custom_views/criteria.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/custom_views/criteria.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/custom_views/custom_view.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/custom_views/custom_view.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/custom_views/custom_views_operations.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/custom_views/custom_views_operations.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/custom_views/info.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/custom_views/info.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/custom_views/range.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/custom_views/range.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/custom_views/response_wrapper.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/custom_views/response_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/custom_views/shared_details.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/custom_views/shared_details.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/custom_views/translation.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/custom_views/translation.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/dc/au_data_center.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/dc/au_data_center.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/dc/cn_data_center.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/dc/cn_data_center.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/dc/data_center.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/dc/data_center.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/dc/eu_data_center.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/dc/eu_data_center.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/dc/in_data_center.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/dc/in_data_center.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/dc/jp_data_center.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/dc/jp_data_center.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/dc/us_data_center.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/dc/us_data_center.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/exception/sdk_exception.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/exception/sdk_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/fields/__init__.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/fields/__init__.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/fields/api_exception.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/fields/api_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/fields/association_details.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/fields/association_details.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/fields/auto_number.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/fields/auto_number.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/fields/crypt.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/fields/crypt.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/fields/currency.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/fields/currency.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/fields/field.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/fields/field.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/fields/fields_operations.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/fields/fields_operations.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/fields/formula.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/fields/formula.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/fields/lookup_field.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/fields/lookup_field.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/fields/module.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/fields/module.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/fields/multi_select_lookup.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/fields/multi_select_lookup.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/fields/pick_list_value.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/fields/pick_list_value.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/fields/private.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/fields/private.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/fields/related_details.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/fields/related_details.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/fields/response_wrapper.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/fields/response_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/fields/tool_tip.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/fields/tool_tip.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/fields/unique.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/fields/unique.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/fields/view_type.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/fields/view_type.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/file/action_wrapper.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/file/action_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/file/api_exception.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/file/api_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/file/body_wrapper.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/file/body_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/file/file_body_wrapper.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/file/file_body_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/file/file_operations.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/file/file_operations.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/file/success_response.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/file/success_response.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/header_map.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/header_map.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/initializer.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/initializer.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/layouts/api_exception.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/layouts/api_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/layouts/layout.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/layouts/layout.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/layouts/layouts_operations.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/layouts/layouts_operations.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/layouts/properties.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/layouts/properties.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/layouts/response_wrapper.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/layouts/response_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/layouts/section.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/layouts/section.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/modules/__init__.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/modules/action_wrapper.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/modules/action_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/modules/api_exception.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/modules/api_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/modules/argument.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/modules/argument.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/modules/body_wrapper.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/modules/body_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/modules/module.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/modules/module.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/modules/modules_operations.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/modules/modules_operations.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/modules/related_list_properties.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/modules/related_list_properties.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/modules/response_wrapper.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/modules/response_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/modules/success_response.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/modules/success_response.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/modules/territory.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/modules/territory.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/notes/__init__.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/notes/__init__.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/notes/action_wrapper.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/notes/action_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/notes/api_exception.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/notes/api_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/notes/body_wrapper.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/notes/body_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/notes/info.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/notes/info.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/notes/note.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/notes/note.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/notes/notes_operations.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/notes/notes_operations.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/notes/response_wrapper.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/notes/response_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/notes/success_response.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/notes/success_response.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/notification/__init__.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/notification/__init__.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/notification/action_wrapper.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/notification/action_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/notification/api_exception.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/notification/api_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/notification/body_wrapper.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/notification/body_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/notification/info.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/notification/info.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/notification/notification.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/notification/notification.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/notification/notification_operations.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/notification/notification_operations.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/notification/response_wrapper.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/notification/response_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/notification/success_response.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/notification/success_response.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/org/api_exception.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/org/api_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/org/file_body_wrapper.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/org/file_body_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/org/license_details.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/org/license_details.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/org/org.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/org/org.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/org/org_operations.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/org/org_operations.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/org/response_wrapper.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/org/response_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/org/success_response.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/org/success_response.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/parameter_map.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/parameter_map.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/profiles/api_exception.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/profiles/api_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/profiles/category.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/profiles/category.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/profiles/permission_detail.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/profiles/permission_detail.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/profiles/profile.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/profiles/profile.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/profiles/profiles_operations.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/profiles/profiles_operations.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/profiles/response_wrapper.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/profiles/response_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/profiles/section.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/profiles/section.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/query/api_exception.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/query/api_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/query/body_wrapper.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/query/body_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/query/query_operations.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/query/query_operations.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/query/response_wrapper.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/query/response_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/record/__init__.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/record/__init__.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/record/action_wrapper.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/record/action_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/record/api_exception.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/record/api_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/record/apply_feature_execution.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/record/apply_feature_execution.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/record/body_wrapper.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/record/body_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/record/carry_over_tags.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/record/carry_over_tags.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/record/comment.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/record/comment.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/record/consent.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/record/consent.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/record/convert_action_wrapper.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/record/convert_action_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/record/convert_body_wrapper.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/record/convert_body_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/record/criteria.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/record/criteria.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/record/deleted_record.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/record/deleted_record.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/record/deleted_records_wrapper.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/record/deleted_records_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/record/field.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/record/field.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/record/file_body_wrapper.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/record/file_body_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/record/file_details.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/record/file_details.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/record/info.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/record/info.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/record/inventory_line_items.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/record/inventory_line_items.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/record/lead_converter.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/record/lead_converter.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/record/line_item_product.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/record/line_item_product.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/record/line_tax.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/record/line_tax.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/record/mass_update.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/record/mass_update.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/record/mass_update_action_wrapper.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/record/mass_update_action_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/record/mass_update_body_wrapper.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/record/mass_update_body_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/record/mass_update_response_wrapper.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/record/mass_update_response_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/record/mass_update_success_response.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/record/mass_update_success_response.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/record/participants.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/record/participants.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/record/pricing_details.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/record/pricing_details.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/record/record.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/record/record.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/record/record_operations.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/record/record_operations.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/record/recurring_activity.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/record/recurring_activity.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/record/remind_at.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/record/remind_at.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/record/reminder.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/record/reminder.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/record/response_wrapper.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/record/response_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/record/success_response.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/record/success_response.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/record/successful_convert.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/record/successful_convert.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/record/territory.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/record/territory.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/related_lists/api_exception.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/related_lists/api_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/related_lists/related_list.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/related_lists/related_list.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/related_lists/related_lists_operations.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/related_lists/related_lists_operations.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/related_lists/response_wrapper.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/related_lists/response_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/related_records/__init__.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/related_records/__init__.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/related_records/action_wrapper.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/related_records/action_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/related_records/api_exception.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/related_records/api_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/related_records/body_wrapper.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/related_records/body_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/related_records/file_body_wrapper.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/related_records/file_body_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/related_records/related_records_operations.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/related_records/related_records_operations.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/related_records/response_wrapper.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/related_records/response_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/related_records/success_response.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/related_records/success_response.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/request_proxy.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/request_proxy.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/roles/api_exception.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/roles/api_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/roles/response_wrapper.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/roles/response_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/roles/role.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/roles/role.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/roles/roles_operations.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/roles/roles_operations.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/sdk_config.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/sdk_config.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/share_records/__init__.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/share_records/__init__.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/share_records/action_wrapper.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/share_records/action_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/share_records/api_exception.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/share_records/api_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/share_records/body_wrapper.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/share_records/body_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/share_records/delete_action_wrapper.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/share_records/delete_action_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/share_records/response_wrapper.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/share_records/response_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/share_records/share_record.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/share_records/share_record.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/share_records/share_records_operations.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/share_records/share_records_operations.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/share_records/shared_through.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/share_records/shared_through.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/share_records/success_response.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/share_records/success_response.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/tags/__init__.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/tags/__init__.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/tags/action_wrapper.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/tags/action_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/tags/api_exception.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/tags/api_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/tags/body_wrapper.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/tags/body_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/tags/conflict_wrapper.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/tags/conflict_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/tags/count_wrapper.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/tags/count_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/tags/info.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/tags/info.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/tags/merge_wrapper.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/tags/merge_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/tags/record_action_wrapper.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/tags/record_action_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/tags/response_wrapper.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/tags/response_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/tags/success_response.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/tags/success_response.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/tags/tag.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/tags/tag.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/tags/tags_operations.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/tags/tags_operations.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/taxes/action_wrapper.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/taxes/action_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/taxes/api_exception.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/taxes/api_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/taxes/body_wrapper.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/taxes/body_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/taxes/preference.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/taxes/preference.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/taxes/response_wrapper.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/taxes/response_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/taxes/success_response.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/taxes/success_response.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/taxes/tax.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/taxes/tax.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/taxes/taxes_operations.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/taxes/taxes_operations.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/territories/api_exception.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/territories/api_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/territories/response_wrapper.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/territories/response_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/territories/territories_operations.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/territories/territories_operations.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/territories/territory.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/territories/territory.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/user_signature.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/user_signature.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/users/__init__.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/users/__init__.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/users/action_wrapper.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/users/action_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/users/api_exception.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/users/api_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/users/body_wrapper.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/users/body_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/users/customize_info.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/users/customize_info.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/users/info.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/users/info.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/users/request_wrapper.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/users/request_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/users/response_wrapper.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/users/response_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/users/shift.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/users/shift.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/users/success_response.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/users/success_response.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/users/tab_theme.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/users/tab_theme.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/users/territory.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/users/territory.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/users/theme.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/users/theme.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/users/user.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/users/user.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/users/users_operations.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/users/users_operations.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/util/__init__.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/util/__init__.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/util/api_http_connector.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/util/api_http_connector.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/util/api_response.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/util/api_response.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/util/common_api_handler.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/util/common_api_handler.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/util/constants.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/util/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -170,15 +170,15 @@
 
     PHOTO_SUPPORTED_MODULES = ["leads", "contacts", "accounts", "products", "vendors"]
 
     GIVEN_LENGTH = "given-length"
 
     ZOHO_SDK = "X-ZOHO-SDK"
 
-    SDK_VERSION = "5.1.0"
+    SDK_VERSION = "6.0.0"
 
     ZOHO_API_VERSION = "2.0"
 
     CONTENT_DISPOSITION = "Content-Disposition"
 
     TOKEN_ERROR = "TOKEN ERROR"
```

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/util/converter.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/util/converter.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/util/datatype_converter.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/util/datatype_converter.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/util/downloader.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/util/downloader.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/util/form_data_converter.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/util/form_data_converter.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/util/header_param_validator.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/util/header_param_validator.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/util/json_converter.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/util/json_converter.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/util/module_fields_handler.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/util/module_fields_handler.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/util/stream_wrapper.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/util/stream_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/util/utility.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/util/utility.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/util/xml_converter.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/util/xml_converter.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/variable_groups/api_exception.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/variable_groups/api_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/variable_groups/response_wrapper.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/variable_groups/response_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/variable_groups/variable_group.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/variable_groups/variable_group.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/variable_groups/variable_groups_operations.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/variable_groups/variable_groups_operations.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/variables/__init__.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/variables/__init__.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/variables/action_wrapper.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/variables/action_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/variables/api_exception.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/variables/api_exception.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/variables/body_wrapper.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/variables/body_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/variables/response_wrapper.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/variables/response_wrapper.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/variables/success_response.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/variables/success_response.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/variables/variable.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/variables/variable.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/com/zoho/crm/api/variables/variables_operations.py` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/com/zoho/crm/api/variables/variables_operations.py`

 * *Files identical despite different names*

### Comparing `zohocrmsdk2_0-5.1.0/zcrmsdk/src/json_details.json` & `zohocrmsdk2_0-6.0.0/zcrmsdk/src/json_details.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9997402597402597%*

 * *Differences: {"'zcrmsdk.src.com.zoho.crm.api.bulk_write.RequestWrapper'": "{'ignore_empty': "*

 * *                                                             "OrderedDict([('name', "*

 * *                                                             "'ignore_empty'), ('type', "*

 * *                                                             "'Boolean')])}"}*

```diff
@@ -1172,14 +1172,18 @@
             "structure_name": "zcrmsdk.src.com.zoho.crm.api.bulk_write.CallBack",
             "type": "zcrmsdk.src.com.zoho.crm.api.bulk_write.CallBack"
         },
         "character_encoding": {
             "name": "character_encoding",
             "type": "String"
         },
+        "ignore_empty": {
+            "name": "ignore_empty",
+            "type": "Boolean"
+        },
         "operation": {
             "name": "operation",
             "required": true,
             "type": "zcrmsdk.src.com.zoho.crm.api.util.Choice",
             "values": [
                 "insert",
                 "update",
```

### Comparing `zohocrmsdk2_0-5.1.0/zohocrmsdk2_0.egg-info/PKG-INFO` & `zohocrmsdk2_0-6.0.0/zohocrmsdk2_0.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: zohocrmsdk2-0
-Version: 5.1.0
+Name: zohocrmsdk2_0
+Version: 6.0.0
 Summary: Zoho CRM SDK for Python developers
 Home-page: https://github.com/zoho/zohocrm-python-sdk-2.0
 Author: Zoho CRM API Team
 Author-email: support@zohocrm.com
 License: Apache Software License, Version 2.0, http://www.apache.org/licenses/LICENSE-2.0
 Keywords: development,zoho,crm,api,zcrmsdk,sdk,zcrm,zohocrmsdk2_0
 Classifier: Development Status :: 5 - Production/Stable
@@ -16,14 +16,19 @@
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: requests
+Requires-Dist: python-dateutil
+Requires-Dist: urllib3
+Requires-Dist: mysql-connector-python
+Requires-Dist: setuptools
 
 #  ZOHO CRM PYTHON SDK 2.0
 
 ## Table Of Contents
 
 * [Overview](#overview)
 * [Registering a Zoho Client](#registering-a-zoho-client)
```

### Comparing `zohocrmsdk2_0-5.1.0/zohocrmsdk2_0.egg-info/SOURCES.txt` & `zohocrmsdk2_0-6.0.0/zohocrmsdk2_0.egg-info/SOURCES.txt`

 * *Files identical despite different names*

