# Comparing `tmp/zrok-0.4.26.tar.gz` & `tmp/zrok-0.4.27.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zrok-0.4.26.tar", last modified: Fri Mar  8 21:46:56 2024, max compression
+gzip compressed data, was "zrok-0.4.27.tar", last modified: Tue Apr 16 20:48:07 2024, max compression
```

## Comparing `zrok-0.4.26.tar` & `zrok-0.4.27.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 21:46:56.702013 zrok-0.4.26/
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-03-08 21:46:56.702013 zrok-0.4.26/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-03-08 21:46:56.702013 zrok-0.4.26/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-03-08 21:46:52.000000 zrok-0.4.26/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)    86677 2024-03-08 21:46:52.000000 zrok-0.4.26/versioneer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 21:46:56.702013 zrok-0.4.26/zrok/
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-03-08 21:46:52.000000 zrok-0.4.26/zrok/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-03-08 21:46:56.702013 zrok-0.4.26/zrok/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-03-08 21:46:52.000000 zrok-0.4.26/zrok/access.py
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-03-08 21:46:52.000000 zrok-0.4.26/zrok/decor.py
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-03-08 21:46:52.000000 zrok-0.4.26/zrok/dialer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 21:46:56.690013 zrok-0.4.26/zrok/environment/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-03-08 21:46:52.000000 zrok-0.4.26/zrok/environment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-03-08 21:46:52.000000 zrok-0.4.26/zrok/environment/dirs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3578 2024-03-08 21:46:52.000000 zrok-0.4.26/zrok/environment/root.py
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-03-08 21:46:52.000000 zrok-0.4.26/zrok/listener.py
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-03-08 21:46:52.000000 zrok-0.4.26/zrok/model.py
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-03-08 21:46:52.000000 zrok-0.4.26/zrok/overview.py
--rw-r--r--   0 runner    (1001) docker     (127)     3657 2024-03-08 21:46:52.000000 zrok-0.4.26/zrok/share.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 21:46:56.702013 zrok-0.4.26/zrok.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-03-08 21:46:56.000000 zrok-0.4.26/zrok.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2569 2024-03-08 21:46:56.000000 zrok-0.4.26/zrok.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-08 21:46:56.000000 zrok-0.4.26/zrok.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-03-08 21:46:56.000000 zrok-0.4.26/zrok.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-08 21:46:56.000000 zrok-0.4.26/zrok.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 21:46:56.694012 zrok-0.4.26/zrok_api/
--rw-r--r--   0 runner    (1001) docker     (127)     3583 2024-03-08 21:46:52.000000 zrok-0.4.26/zrok_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 21:46:56.694012 zrok-0.4.26/zrok_api/api/
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-03-08 21:46:52.000000 zrok-0.4.26/zrok_api/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26777 2024-03-08 21:46:52.000000 zrok-0.4.26/zrok_api/api/account_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    19872 2024-03-08 21:46:52.000000 zrok-0.4.26/zrok_api/api/admin_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     6996 2024-03-08 21:46:52.000000 zrok-0.4.26/zrok_api/api/environment_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    33642 2024-03-08 21:46:52.000000 zrok-0.4.26/zrok_api/api/metadata_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    16548 2024-03-08 21:46:52.000000 zrok-0.4.26/zrok_api/api/share_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    24955 2024-03-08 21:46:52.000000 zrok-0.4.26/zrok_api/api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     8120 2024-03-08 21:46:52.000000 zrok-0.4.26/zrok_api/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 21:46:56.702013 zrok-0.4.26/zrok_api/models/
--rw-r--r--   0 runner    (1001) docker     (127)     3201 2024-03-08 21:46:52.000000 zrok-0.4.26/zrok_api/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3673 2024-03-08 21:46:52.000000 zrok-0.4.26/zrok_api/models/access_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3885 2024-03-08 21:46:52.000000 zrok-0.4.26/zrok_api/models/access_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-03-08 21:46:52.000000 zrok-0.4.26/zrok_api/models/auth_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     4562 2024-03-08 21:46:52.000000 zrok-0.4.26/zrok_api/models/change_password_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     7189 2024-03-08 21:46:52.000000 zrok-0.4.26/zrok_api/models/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     4523 2024-03-08 21:46:52.000000 zrok-0.4.26/zrok_api/models/create_frontend_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3026 2024-03-08 21:46:52.000000 zrok-0.4.26/zrok_api/models/create_frontend_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-03-08 21:46:52.000000 zrok-0.4.26/zrok_api/models/delete_frontend_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3022 2024-03-08 21:46:52.000000 zrok-0.4.26/zrok_api/models/disable_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-03-08 21:46:52.000000 zrok-0.4.26/zrok_api/models/enable_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3587 2024-03-08 21:46:52.000000 zrok-0.4.26/zrok_api/models/enable_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     7527 2024-03-08 21:46:52.000000 zrok-0.4.26/zrok_api/models/environment.py
--rw-r--r--   0 runner    (1001) docker     (127)     4587 2024-03-08 21:46:52.000000 zrok-0.4.26/zrok_api/models/environment_and_resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-03-08 21:46:52.000000 zrok-0.4.26/zrok_api/models/environments.py
--rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-03-08 21:46:52.000000 zrok-0.4.26/zrok_api/models/error_message.py
--rw-r--r--   0 runner    (1001) docker     (127)     6015 2024-03-08 21:46:52.000000 zrok-0.4.26/zrok_api/models/frontend.py
--rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-03-08 21:46:52.000000 zrok-0.4.26/zrok_api/models/frontends.py
--rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-03-08 21:46:52.000000 zrok-0.4.26/zrok_api/models/identity_body.py
--rw-r--r--   0 runner    (1001) docker     (127)     2986 2024-03-08 21:46:52.000000 zrok-0.4.26/zrok_api/models/inline_response200.py
--rw-r--r--   0 runner    (1001) docker     (127)     3623 2024-03-08 21:46:52.000000 zrok-0.4.26/zrok_api/models/inline_response201.py
--rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-03-08 21:46:52.000000 zrok-0.4.26/zrok_api/models/invite_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-03-08 21:46:52.000000 zrok-0.4.26/zrok_api/models/invite_token_generate_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3603 2024-03-08 21:46:52.000000 zrok-0.4.26/zrok_api/models/login_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-03-08 21:46:52.000000 zrok-0.4.26/zrok_api/models/login_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     4691 2024-03-08 21:46:52.000000 zrok-0.4.26/zrok_api/models/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     4134 2024-03-08 21:46:52.000000 zrok-0.4.26/zrok_api/models/metrics_sample.py
--rw-r--r--   0 runner    (1001) docker     (127)     3915 2024-03-08 21:46:52.000000 zrok-0.4.26/zrok_api/models/overview.py
--rw-r--r--   0 runner    (1001) docker     (127)     6530 2024-03-08 21:46:52.000000 zrok-0.4.26/zrok_api/models/password_requirements.py
--rw-r--r--   0 runner    (1001) docker     (127)     5288 2024-03-08 21:46:52.000000 zrok-0.4.26/zrok_api/models/principal.py
--rw-r--r--   0 runner    (1001) docker     (127)     6422 2024-03-08 21:46:52.000000 zrok-0.4.26/zrok_api/models/public_frontend.py
--rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-03-08 21:46:52.000000 zrok-0.4.26/zrok_api/models/public_frontend_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     3161 2024-03-08 21:46:52.000000 zrok-0.4.26/zrok_api/models/regenerate_token_body.py
--rw-r--r--   0 runner    (1001) docker     (127)     3639 2024-03-08 21:46:52.000000 zrok-0.4.26/zrok_api/models/register_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-03-08 21:46:52.000000 zrok-0.4.26/zrok_api/models/register_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3699 2024-03-08 21:46:52.000000 zrok-0.4.26/zrok_api/models/reset_password_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3201 2024-03-08 21:46:52.000000 zrok-0.4.26/zrok_api/models/reset_password_request_body.py
--rw-r--r--   0 runner    (1001) docker     (127)    10584 2024-03-08 21:46:52.000000 zrok-0.4.26/zrok_api/models/share.py
--rw-r--r--   0 runner    (1001) docker     (127)    14701 2024-03-08 21:46:52.000000 zrok-0.4.26/zrok_api/models/share_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     4030 2024-03-08 21:46:52.000000 zrok-0.4.26/zrok_api/models/share_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2327 2024-03-08 21:46:52.000000 zrok-0.4.26/zrok_api/models/shares.py
--rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-03-08 21:46:52.000000 zrok-0.4.26/zrok_api/models/spark_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3471 2024-03-08 21:46:52.000000 zrok-0.4.26/zrok_api/models/spark_data_sample.py
--rw-r--r--   0 runner    (1001) docker     (127)     4485 2024-03-08 21:46:52.000000 zrok-0.4.26/zrok_api/models/unaccess_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     4353 2024-03-08 21:46:52.000000 zrok-0.4.26/zrok_api/models/unshare_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     4721 2024-03-08 21:46:52.000000 zrok-0.4.26/zrok_api/models/update_frontend_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     5846 2024-03-08 21:46:52.000000 zrok-0.4.26/zrok_api/models/update_share_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2954 2024-03-08 21:46:52.000000 zrok-0.4.26/zrok_api/models/verify_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2962 2024-03-08 21:46:52.000000 zrok-0.4.26/zrok_api/models/verify_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-03-08 21:46:52.000000 zrok-0.4.26/zrok_api/models/version.py
--rw-r--r--   0 runner    (1001) docker     (127)    12931 2024-03-08 21:46:52.000000 zrok-0.4.26/zrok_api/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:48:07.703796 zrok-0.4.27/
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-16 20:48:07.703796 zrok-0.4.27/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-04-16 20:48:07.703796 zrok-0.4.27/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-16 20:48:05.000000 zrok-0.4.27/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    86677 2024-04-16 20:48:05.000000 zrok-0.4.27/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:48:07.703796 zrok-0.4.27/zrok/
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-16 20:48:05.000000 zrok-0.4.27/zrok/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-16 20:48:07.703796 zrok-0.4.27/zrok/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-04-16 20:48:05.000000 zrok-0.4.27/zrok/access.py
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-04-16 20:48:05.000000 zrok-0.4.27/zrok/decor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-16 20:48:05.000000 zrok-0.4.27/zrok/dialer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:48:07.695796 zrok-0.4.27/zrok/environment/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-16 20:48:05.000000 zrok-0.4.27/zrok/environment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-16 20:48:05.000000 zrok-0.4.27/zrok/environment/dirs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3578 2024-04-16 20:48:05.000000 zrok-0.4.27/zrok/environment/root.py
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-16 20:48:05.000000 zrok-0.4.27/zrok/listener.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1712 2024-04-16 20:48:05.000000 zrok-0.4.27/zrok/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-04-16 20:48:05.000000 zrok-0.4.27/zrok/overview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3903 2024-04-16 20:48:05.000000 zrok-0.4.27/zrok/share.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:48:07.703796 zrok-0.4.27/zrok.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-16 20:48:07.000000 zrok-0.4.27/zrok.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2569 2024-04-16 20:48:07.000000 zrok-0.4.27/zrok.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 20:48:07.000000 zrok-0.4.27/zrok.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-16 20:48:07.000000 zrok-0.4.27/zrok.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-16 20:48:07.000000 zrok-0.4.27/zrok.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:48:07.695796 zrok-0.4.27/zrok_api/
+-rw-r--r--   0 runner    (1001) docker     (127)     3583 2024-04-16 20:48:05.000000 zrok-0.4.27/zrok_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:48:07.695796 zrok-0.4.27/zrok_api/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-16 20:48:05.000000 zrok-0.4.27/zrok_api/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26777 2024-04-16 20:48:05.000000 zrok-0.4.27/zrok_api/api/account_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19872 2024-04-16 20:48:05.000000 zrok-0.4.27/zrok_api/api/admin_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6996 2024-04-16 20:48:05.000000 zrok-0.4.27/zrok_api/api/environment_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33642 2024-04-16 20:48:05.000000 zrok-0.4.27/zrok_api/api/metadata_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16548 2024-04-16 20:48:05.000000 zrok-0.4.27/zrok_api/api/share_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24955 2024-04-16 20:48:05.000000 zrok-0.4.27/zrok_api/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8120 2024-04-16 20:48:05.000000 zrok-0.4.27/zrok_api/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:48:07.703796 zrok-0.4.27/zrok_api/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     3201 2024-04-16 20:48:05.000000 zrok-0.4.27/zrok_api/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3673 2024-04-16 20:48:05.000000 zrok-0.4.27/zrok_api/models/access_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3885 2024-04-16 20:48:05.000000 zrok-0.4.27/zrok_api/models/access_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-04-16 20:48:05.000000 zrok-0.4.27/zrok_api/models/auth_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4562 2024-04-16 20:48:05.000000 zrok-0.4.27/zrok_api/models/change_password_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7189 2024-04-16 20:48:05.000000 zrok-0.4.27/zrok_api/models/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4523 2024-04-16 20:48:05.000000 zrok-0.4.27/zrok_api/models/create_frontend_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3026 2024-04-16 20:48:05.000000 zrok-0.4.27/zrok_api/models/create_frontend_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-04-16 20:48:05.000000 zrok-0.4.27/zrok_api/models/delete_frontend_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3022 2024-04-16 20:48:05.000000 zrok-0.4.27/zrok_api/models/disable_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-04-16 20:48:05.000000 zrok-0.4.27/zrok_api/models/enable_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3587 2024-04-16 20:48:05.000000 zrok-0.4.27/zrok_api/models/enable_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7527 2024-04-16 20:48:05.000000 zrok-0.4.27/zrok_api/models/environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4587 2024-04-16 20:48:05.000000 zrok-0.4.27/zrok_api/models/environment_and_resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-04-16 20:48:05.000000 zrok-0.4.27/zrok_api/models/environments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-04-16 20:48:05.000000 zrok-0.4.27/zrok_api/models/error_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6015 2024-04-16 20:48:05.000000 zrok-0.4.27/zrok_api/models/frontend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-04-16 20:48:05.000000 zrok-0.4.27/zrok_api/models/frontends.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-04-16 20:48:05.000000 zrok-0.4.27/zrok_api/models/identity_body.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2986 2024-04-16 20:48:05.000000 zrok-0.4.27/zrok_api/models/inline_response200.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3623 2024-04-16 20:48:05.000000 zrok-0.4.27/zrok_api/models/inline_response201.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-04-16 20:48:05.000000 zrok-0.4.27/zrok_api/models/invite_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-04-16 20:48:05.000000 zrok-0.4.27/zrok_api/models/invite_token_generate_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3603 2024-04-16 20:48:05.000000 zrok-0.4.27/zrok_api/models/login_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-04-16 20:48:05.000000 zrok-0.4.27/zrok_api/models/login_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4691 2024-04-16 20:48:05.000000 zrok-0.4.27/zrok_api/models/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4134 2024-04-16 20:48:05.000000 zrok-0.4.27/zrok_api/models/metrics_sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3915 2024-04-16 20:48:05.000000 zrok-0.4.27/zrok_api/models/overview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6530 2024-04-16 20:48:05.000000 zrok-0.4.27/zrok_api/models/password_requirements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5288 2024-04-16 20:48:05.000000 zrok-0.4.27/zrok_api/models/principal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6422 2024-04-16 20:48:05.000000 zrok-0.4.27/zrok_api/models/public_frontend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-04-16 20:48:05.000000 zrok-0.4.27/zrok_api/models/public_frontend_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3161 2024-04-16 20:48:05.000000 zrok-0.4.27/zrok_api/models/regenerate_token_body.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3639 2024-04-16 20:48:05.000000 zrok-0.4.27/zrok_api/models/register_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-04-16 20:48:05.000000 zrok-0.4.27/zrok_api/models/register_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3699 2024-04-16 20:48:05.000000 zrok-0.4.27/zrok_api/models/reset_password_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3201 2024-04-16 20:48:05.000000 zrok-0.4.27/zrok_api/models/reset_password_request_body.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10584 2024-04-16 20:48:05.000000 zrok-0.4.27/zrok_api/models/share.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14708 2024-04-16 20:48:05.000000 zrok-0.4.27/zrok_api/models/share_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4030 2024-04-16 20:48:05.000000 zrok-0.4.27/zrok_api/models/share_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2327 2024-04-16 20:48:05.000000 zrok-0.4.27/zrok_api/models/shares.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-04-16 20:48:05.000000 zrok-0.4.27/zrok_api/models/spark_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3471 2024-04-16 20:48:05.000000 zrok-0.4.27/zrok_api/models/spark_data_sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4485 2024-04-16 20:48:05.000000 zrok-0.4.27/zrok_api/models/unaccess_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4353 2024-04-16 20:48:05.000000 zrok-0.4.27/zrok_api/models/unshare_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4721 2024-04-16 20:48:05.000000 zrok-0.4.27/zrok_api/models/update_frontend_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5846 2024-04-16 20:48:05.000000 zrok-0.4.27/zrok_api/models/update_share_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2954 2024-04-16 20:48:05.000000 zrok-0.4.27/zrok_api/models/verify_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2962 2024-04-16 20:48:05.000000 zrok-0.4.27/zrok_api/models/verify_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-04-16 20:48:05.000000 zrok-0.4.27/zrok_api/models/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12931 2024-04-16 20:48:05.000000 zrok-0.4.27/zrok_api/rest.py
```

### Comparing `zrok-0.4.26/PKG-INFO` & `zrok-0.4.27/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zrok
-Version: 0.4.26
+Version: 0.4.27
 Summary: zrok
 Home-page: https://github.com/openziti/zrok
 Author: OpenZiti Developers
 Author-email: developers@openziti.org
 License: Apache 2.0
 Project-URL: Source, https://github.com/openziti/zrok
 Project-URL: Tracker, https://github.com/openziti/zrok/issues
```

### Comparing `zrok-0.4.26/setup.cfg` & `zrok-0.4.27/setup.cfg`

 * *Files identical despite different names*

### Comparing `zrok-0.4.26/setup.py` & `zrok-0.4.27/setup.py`

 * *Files identical despite different names*

### Comparing `zrok-0.4.26/versioneer.py` & `zrok-0.4.27/versioneer.py`

 * *Files identical despite different names*

### Comparing `zrok-0.4.26/zrok/access.py` & `zrok-0.4.27/zrok/access.py`

 * *Files identical despite different names*

### Comparing `zrok-0.4.26/zrok/decor.py` & `zrok-0.4.27/zrok/decor.py`

 * *Files identical despite different names*

### Comparing `zrok-0.4.26/zrok/environment/dirs.py` & `zrok-0.4.27/zrok/environment/dirs.py`

 * *Files identical despite different names*

### Comparing `zrok-0.4.26/zrok/environment/root.py` & `zrok-0.4.27/zrok/environment/root.py`

 * *Files identical despite different names*

### Comparing `zrok-0.4.26/zrok/listener.py` & `zrok-0.4.27/zrok/listener.py`

 * *Files identical despite different names*

### Comparing `zrok-0.4.26/zrok/model.py` & `zrok-0.4.27/zrok/model.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,33 +3,43 @@
 BackendMode = str
 
 PROXY_BACKEND_MODE: BackendMode = "proxy"
 WEB_BACKEND_MODE: BackendMode = "web"
 TCP_TUNNEL_BACKEND_MODE: BackendMode = "tcpTunnel"
 UDP_TUNNEL_BACKEND_MODE: BackendMode = "udpTunnel"
 CADDY_BACKEND_MODE: BackendMode = "caddy"
+DRIVE_BACKEND_MODE: BackendMode = "drive"
+SOCKS_BACKEND_MODE: BackendMode = "socks"
+VPN_BACKEND_MODE: BackendMode = "vpn"
 
 ShareMode = str
 
 PRIVATE_SHARE_MODE: ShareMode = "private"
 PUBLIC_SHARE_MODE: ShareMode = "public"
 
+PermissionMode = str
+
+OPEN_PERMISSION_MODE: PermissionMode = "open"
+CLOSED_PERMISSION_MODE: PermissionMode = "closed"
+
 
 @dataclass
 class ShareRequest:
     BackendMode: BackendMode
     ShareMode: ShareMode
     Target: str
     Frontends: list[str] = field(default_factory=list[str])
     BasicAuth: list[str] = field(default_factory=list[str])
     OauthProvider: str = ""
     OauthEmailAddressPatterns: list[str] = field(default_factory=list[str])
     OauthAuthorizationCheckInterval: str = ""
     Reserved: bool = False
     UniqueName: str = ""
+    PermissionMode: PermissionMode = OPEN_PERMISSION_MODE
+    AccessGrants: list[str] = field(default_factory=list[str])
 
 
 @dataclass
 class Share:
     Token: str
     FrontendEndpoints: list[str]
```

### Comparing `zrok-0.4.26/zrok/overview.py` & `zrok-0.4.27/zrok/overview.py`

 * *Files identical despite different names*

### Comparing `zrok-0.4.26/zrok/share.py` & `zrok-0.4.27/zrok/share.py`

 * *Files 10% similar despite different names*

```diff
@@ -63,27 +63,31 @@
 
 
 def __newPrivateShare(root: Root, request: model.ShareRequest) -> ShareRequest:
     return ShareRequest(env_zid=root.env.ZitiIdentity,
                         share_mode=request.ShareMode,
                         backend_mode=request.BackendMode,
                         backend_proxy_endpoint=request.Target,
-                        auth_scheme=model.AUTH_SCHEME_NONE
+                        auth_scheme=model.AUTH_SCHEME_NONE,
+                        permission_mode=request.PermissionMode,
+                        access_grants=request.AccessGrants
                         )
 
 
 def __newPublicShare(root: Root, request: model.ShareRequest) -> ShareRequest:
     ret = ShareRequest(env_zid=root.env.ZitiIdentity,
                        share_mode=request.ShareMode,
                        frontend_selection=request.Frontends,
                        backend_mode=request.BackendMode,
                        backend_proxy_endpoint=request.Target,
                        auth_scheme=model.AUTH_SCHEME_NONE,
                        oauth_email_domains=request.OauthEmailAddressPatterns,
-                       oauth_authorization_check_interval=request.OauthAuthorizationCheckInterval
+                       oauth_authorization_check_interval=request.OauthAuthorizationCheckInterval,
+                       permission_mode=request.PermissionMode,
+                       access_grants=request.AccessGrants
                        )
     if request.OauthProvider != "":
         ret.oauth_provider = request.OauthProvider
 
     return ret
```

### Comparing `zrok-0.4.26/zrok.egg-info/PKG-INFO` & `zrok-0.4.27/zrok.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zrok
-Version: 0.4.26
+Version: 0.4.27
 Summary: zrok
 Home-page: https://github.com/openziti/zrok
 Author: OpenZiti Developers
 Author-email: developers@openziti.org
 License: Apache 2.0
 Project-URL: Source, https://github.com/openziti/zrok
 Project-URL: Tracker, https://github.com/openziti/zrok/issues
```

### Comparing `zrok-0.4.26/zrok.egg-info/SOURCES.txt` & `zrok-0.4.27/zrok.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `zrok-0.4.26/zrok_api/__init__.py` & `zrok-0.4.27/zrok_api/__init__.py`

 * *Files identical despite different names*

### Comparing `zrok-0.4.26/zrok_api/api/account_api.py` & `zrok-0.4.27/zrok_api/api/account_api.py`

 * *Files identical despite different names*

### Comparing `zrok-0.4.26/zrok_api/api/admin_api.py` & `zrok-0.4.27/zrok_api/api/admin_api.py`

 * *Files identical despite different names*

### Comparing `zrok-0.4.26/zrok_api/api/environment_api.py` & `zrok-0.4.27/zrok_api/api/environment_api.py`

 * *Files identical despite different names*

### Comparing `zrok-0.4.26/zrok_api/api/metadata_api.py` & `zrok-0.4.27/zrok_api/api/metadata_api.py`

 * *Files identical despite different names*

### Comparing `zrok-0.4.26/zrok_api/api/share_api.py` & `zrok-0.4.27/zrok_api/api/share_api.py`

 * *Files identical despite different names*

### Comparing `zrok-0.4.26/zrok_api/api_client.py` & `zrok-0.4.27/zrok_api/api_client.py`

 * *Files identical despite different names*

### Comparing `zrok-0.4.26/zrok_api/configuration.py` & `zrok-0.4.27/zrok_api/configuration.py`

 * *Files identical despite different names*

### Comparing `zrok-0.4.26/zrok_api/models/__init__.py` & `zrok-0.4.27/zrok_api/models/__init__.py`

 * *Files identical despite different names*

### Comparing `zrok-0.4.26/zrok_api/models/access_request.py` & `zrok-0.4.27/zrok_api/models/access_request.py`

 * *Files identical despite different names*

### Comparing `zrok-0.4.26/zrok_api/models/access_response.py` & `zrok-0.4.27/zrok_api/models/access_response.py`

 * *Files identical despite different names*

### Comparing `zrok-0.4.26/zrok_api/models/auth_user.py` & `zrok-0.4.27/zrok_api/models/auth_user.py`

 * *Files identical despite different names*

### Comparing `zrok-0.4.26/zrok_api/models/change_password_request.py` & `zrok-0.4.27/zrok_api/models/change_password_request.py`

 * *Files identical despite different names*

### Comparing `zrok-0.4.26/zrok_api/models/configuration.py` & `zrok-0.4.27/zrok_api/models/configuration.py`

 * *Files identical despite different names*

### Comparing `zrok-0.4.26/zrok_api/models/create_frontend_request.py` & `zrok-0.4.27/zrok_api/models/create_frontend_request.py`

 * *Files identical despite different names*

### Comparing `zrok-0.4.26/zrok_api/models/create_frontend_response.py` & `zrok-0.4.27/zrok_api/models/create_frontend_response.py`

 * *Files identical despite different names*

### Comparing `zrok-0.4.26/zrok_api/models/delete_frontend_request.py` & `zrok-0.4.27/zrok_api/models/delete_frontend_request.py`

 * *Files identical despite different names*

### Comparing `zrok-0.4.26/zrok_api/models/disable_request.py` & `zrok-0.4.27/zrok_api/models/disable_request.py`

 * *Files identical despite different names*

### Comparing `zrok-0.4.26/zrok_api/models/enable_request.py` & `zrok-0.4.27/zrok_api/models/enable_request.py`

 * *Files identical despite different names*

### Comparing `zrok-0.4.26/zrok_api/models/enable_response.py` & `zrok-0.4.27/zrok_api/models/enable_response.py`

 * *Files identical despite different names*

### Comparing `zrok-0.4.26/zrok_api/models/environment.py` & `zrok-0.4.27/zrok_api/models/environment.py`

 * *Files identical despite different names*

### Comparing `zrok-0.4.26/zrok_api/models/environment_and_resources.py` & `zrok-0.4.27/zrok_api/models/environment_and_resources.py`

 * *Files identical despite different names*

### Comparing `zrok-0.4.26/zrok_api/models/environments.py` & `zrok-0.4.27/zrok_api/models/environments.py`

 * *Files identical despite different names*

### Comparing `zrok-0.4.26/zrok_api/models/error_message.py` & `zrok-0.4.27/zrok_api/models/error_message.py`

 * *Files identical despite different names*

### Comparing `zrok-0.4.26/zrok_api/models/frontend.py` & `zrok-0.4.27/zrok_api/models/frontend.py`

 * *Files identical despite different names*

### Comparing `zrok-0.4.26/zrok_api/models/frontends.py` & `zrok-0.4.27/zrok_api/models/frontends.py`

 * *Files identical despite different names*

### Comparing `zrok-0.4.26/zrok_api/models/identity_body.py` & `zrok-0.4.27/zrok_api/models/identity_body.py`

 * *Files identical despite different names*

### Comparing `zrok-0.4.26/zrok_api/models/inline_response200.py` & `zrok-0.4.27/zrok_api/models/inline_response200.py`

 * *Files identical despite different names*

### Comparing `zrok-0.4.26/zrok_api/models/inline_response201.py` & `zrok-0.4.27/zrok_api/models/inline_response201.py`

 * *Files identical despite different names*

### Comparing `zrok-0.4.26/zrok_api/models/invite_request.py` & `zrok-0.4.27/zrok_api/models/invite_request.py`

 * *Files identical despite different names*

### Comparing `zrok-0.4.26/zrok_api/models/invite_token_generate_request.py` & `zrok-0.4.27/zrok_api/models/invite_token_generate_request.py`

 * *Files identical despite different names*

### Comparing `zrok-0.4.26/zrok_api/models/login_request.py` & `zrok-0.4.27/zrok_api/models/login_request.py`

 * *Files identical despite different names*

### Comparing `zrok-0.4.26/zrok_api/models/login_response.py` & `zrok-0.4.27/zrok_api/models/login_response.py`

 * *Files identical despite different names*

### Comparing `zrok-0.4.26/zrok_api/models/metrics.py` & `zrok-0.4.27/zrok_api/models/metrics.py`

 * *Files identical despite different names*

### Comparing `zrok-0.4.26/zrok_api/models/metrics_sample.py` & `zrok-0.4.27/zrok_api/models/metrics_sample.py`

 * *Files identical despite different names*

### Comparing `zrok-0.4.26/zrok_api/models/overview.py` & `zrok-0.4.27/zrok_api/models/overview.py`

 * *Files identical despite different names*

### Comparing `zrok-0.4.26/zrok_api/models/password_requirements.py` & `zrok-0.4.27/zrok_api/models/password_requirements.py`

 * *Files identical despite different names*

### Comparing `zrok-0.4.26/zrok_api/models/principal.py` & `zrok-0.4.27/zrok_api/models/principal.py`

 * *Files identical despite different names*

### Comparing `zrok-0.4.26/zrok_api/models/public_frontend.py` & `zrok-0.4.27/zrok_api/models/public_frontend.py`

 * *Files identical despite different names*

### Comparing `zrok-0.4.26/zrok_api/models/public_frontend_list.py` & `zrok-0.4.27/zrok_api/models/public_frontend_list.py`

 * *Files identical despite different names*

### Comparing `zrok-0.4.26/zrok_api/models/regenerate_token_body.py` & `zrok-0.4.27/zrok_api/models/regenerate_token_body.py`

 * *Files identical despite different names*

### Comparing `zrok-0.4.26/zrok_api/models/register_request.py` & `zrok-0.4.27/zrok_api/models/register_request.py`

 * *Files identical despite different names*

### Comparing `zrok-0.4.26/zrok_api/models/register_response.py` & `zrok-0.4.27/zrok_api/models/register_response.py`

 * *Files identical despite different names*

### Comparing `zrok-0.4.26/zrok_api/models/reset_password_request.py` & `zrok-0.4.27/zrok_api/models/reset_password_request.py`

 * *Files identical despite different names*

### Comparing `zrok-0.4.26/zrok_api/models/reset_password_request_body.py` & `zrok-0.4.27/zrok_api/models/reset_password_request_body.py`

 * *Files identical despite different names*

### Comparing `zrok-0.4.26/zrok_api/models/share.py` & `zrok-0.4.27/zrok_api/models/share.py`

 * *Files identical despite different names*

### Comparing `zrok-0.4.26/zrok_api/models/share_request.py` & `zrok-0.4.27/zrok_api/models/share_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -190,15 +190,15 @@
     def backend_mode(self, backend_mode):
         """Sets the backend_mode of this ShareRequest.
 
 
         :param backend_mode: The backend_mode of this ShareRequest.  # noqa: E501
         :type: str
         """
-        allowed_values = ["proxy", "web", "tcpTunnel", "udpTunnel", "caddy", "drive", "socks"]  # noqa: E501
+        allowed_values = ["proxy", "web", "tcpTunnel", "udpTunnel", "caddy", "drive", "socks", "vpn"]  # noqa: E501
         if backend_mode not in allowed_values:
             raise ValueError(
                 "Invalid value for `backend_mode` ({0}), must be one of {1}"  # noqa: E501
                 .format(backend_mode, allowed_values)
             )
 
         self._backend_mode = backend_mode
```

### Comparing `zrok-0.4.26/zrok_api/models/share_response.py` & `zrok-0.4.27/zrok_api/models/share_response.py`

 * *Files identical despite different names*

### Comparing `zrok-0.4.26/zrok_api/models/shares.py` & `zrok-0.4.27/zrok_api/models/shares.py`

 * *Files identical despite different names*

### Comparing `zrok-0.4.26/zrok_api/models/spark_data.py` & `zrok-0.4.27/zrok_api/models/spark_data.py`

 * *Files identical despite different names*

### Comparing `zrok-0.4.26/zrok_api/models/spark_data_sample.py` & `zrok-0.4.27/zrok_api/models/spark_data_sample.py`

 * *Files identical despite different names*

### Comparing `zrok-0.4.26/zrok_api/models/unaccess_request.py` & `zrok-0.4.27/zrok_api/models/unaccess_request.py`

 * *Files identical despite different names*

### Comparing `zrok-0.4.26/zrok_api/models/unshare_request.py` & `zrok-0.4.27/zrok_api/models/unshare_request.py`

 * *Files identical despite different names*

### Comparing `zrok-0.4.26/zrok_api/models/update_frontend_request.py` & `zrok-0.4.27/zrok_api/models/update_frontend_request.py`

 * *Files identical despite different names*

### Comparing `zrok-0.4.26/zrok_api/models/update_share_request.py` & `zrok-0.4.27/zrok_api/models/update_share_request.py`

 * *Files identical despite different names*

### Comparing `zrok-0.4.26/zrok_api/models/verify_request.py` & `zrok-0.4.27/zrok_api/models/verify_request.py`

 * *Files identical despite different names*

### Comparing `zrok-0.4.26/zrok_api/models/verify_response.py` & `zrok-0.4.27/zrok_api/models/verify_response.py`

 * *Files identical despite different names*

### Comparing `zrok-0.4.26/zrok_api/models/version.py` & `zrok-0.4.27/zrok_api/models/version.py`

 * *Files identical despite different names*

### Comparing `zrok-0.4.26/zrok_api/rest.py` & `zrok-0.4.27/zrok_api/rest.py`

 * *Files identical despite different names*

