# Comparing `tmp/pulumi_fastly-8.6.0a1712986611.tar.gz` & `tmp/pulumi_fastly-8.6.0a1713257333.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_fastly-8.6.0a1712986611.tar", last modified: Sat Apr 13 05:43:48 2024, max compression
+gzip compressed data, was "pulumi_fastly-8.6.0a1713257333.tar", last modified: Tue Apr 16 08:53:27 2024, max compression
```

## Comparing `pulumi_fastly-8.6.0a1712986611.tar` & `pulumi_fastly-8.6.0a1713257333.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:43:48.681431 pulumi_fastly-8.6.0a1712986611/
--rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-04-13 05:43:48.681431 pulumi_fastly-8.6.0a1712986611/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-04-13 05:43:42.000000 pulumi_fastly-8.6.0a1712986611/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:43:48.677431 pulumi_fastly-8.6.0a1712986611/pulumi_fastly/
--rw-r--r--   0 runner    (1001) docker     (127)     5702 2024-04-13 05:43:42.000000 pulumi_fastly-8.6.0a1712986611/pulumi_fastly/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   521997 2024-04-13 05:43:42.000000 pulumi_fastly-8.6.0a1712986611/pulumi_fastly/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-13 05:43:42.000000 pulumi_fastly-8.6.0a1712986611/pulumi_fastly/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    24235 2024-04-13 05:43:42.000000 pulumi_fastly-8.6.0a1712986611/pulumi_fastly/alert.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:43:48.681431 pulumi_fastly-8.6.0a1712986611/pulumi_fastly/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-13 05:43:42.000000 pulumi_fastly-8.6.0a1712986611/pulumi_fastly/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-04-13 05:43:42.000000 pulumi_fastly-8.6.0a1712986611/pulumi_fastly/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-04-13 05:43:42.000000 pulumi_fastly-8.6.0a1712986611/pulumi_fastly/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    13105 2024-04-13 05:43:42.000000 pulumi_fastly-8.6.0a1712986611/pulumi_fastly/configstore.py
--rw-r--r--   0 runner    (1001) docker     (127)    11396 2024-04-13 05:43:42.000000 pulumi_fastly-8.6.0a1712986611/pulumi_fastly/configstore_entries.py
--rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-04-13 05:43:42.000000 pulumi_fastly-8.6.0a1712986611/pulumi_fastly/get_configstores.py
--rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-04-13 05:43:42.000000 pulumi_fastly-8.6.0a1712986611/pulumi_fastly/get_datacenters.py
--rw-r--r--   0 runner    (1001) docker     (127)     6375 2024-04-13 05:43:42.000000 pulumi_fastly-8.6.0a1712986611/pulumi_fastly/get_dictionaries.py
--rw-r--r--   0 runner    (1001) docker     (127)     4521 2024-04-13 05:43:42.000000 pulumi_fastly-8.6.0a1712986611/pulumi_fastly/get_fastly_ip_ranges.py
--rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-04-13 05:43:42.000000 pulumi_fastly-8.6.0a1712986611/pulumi_fastly/get_kvstores.py
--rw-r--r--   0 runner    (1001) docker     (127)     5921 2024-04-13 05:43:42.000000 pulumi_fastly-8.6.0a1712986611/pulumi_fastly/get_package_hash.py
--rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-04-13 05:43:42.000000 pulumi_fastly-8.6.0a1712986611/pulumi_fastly/get_secretstores.py
--rw-r--r--   0 runner    (1001) docker     (127)     3072 2024-04-13 05:43:42.000000 pulumi_fastly-8.6.0a1712986611/pulumi_fastly/get_services.py
--rw-r--r--   0 runner    (1001) docker     (127)     6799 2024-04-13 05:43:42.000000 pulumi_fastly-8.6.0a1712986611/pulumi_fastly/get_tls_activation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4424 2024-04-13 05:43:42.000000 pulumi_fastly-8.6.0a1712986611/pulumi_fastly/get_tls_activation_ids.py
--rw-r--r--   0 runner    (1001) docker     (127)     9956 2024-04-13 05:43:42.000000 pulumi_fastly-8.6.0a1712986611/pulumi_fastly/get_tls_certificate.py
--rw-r--r--   0 runner    (1001) docker     (127)     3307 2024-04-13 05:43:42.000000 pulumi_fastly-8.6.0a1712986611/pulumi_fastly/get_tls_certificate_ids.py
--rw-r--r--   0 runner    (1001) docker     (127)    10865 2024-04-13 05:43:42.000000 pulumi_fastly-8.6.0a1712986611/pulumi_fastly/get_tls_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     3368 2024-04-13 05:43:42.000000 pulumi_fastly-8.6.0a1712986611/pulumi_fastly/get_tls_configuration_ids.py
--rw-r--r--   0 runner    (1001) docker     (127)     5207 2024-04-13 05:43:42.000000 pulumi_fastly-8.6.0a1712986611/pulumi_fastly/get_tls_domain.py
--rw-r--r--   0 runner    (1001) docker     (127)     8137 2024-04-13 05:43:42.000000 pulumi_fastly-8.6.0a1712986611/pulumi_fastly/get_tls_platform_certificate.py
--rw-r--r--   0 runner    (1001) docker     (127)     3488 2024-04-13 05:43:42.000000 pulumi_fastly-8.6.0a1712986611/pulumi_fastly/get_tls_platform_certificate_ids.py
--rw-r--r--   0 runner    (1001) docker     (127)     8652 2024-04-13 05:43:42.000000 pulumi_fastly-8.6.0a1712986611/pulumi_fastly/get_tls_private_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     3101 2024-04-13 05:43:42.000000 pulumi_fastly-8.6.0a1712986611/pulumi_fastly/get_tls_private_key_ids.py
--rw-r--r--   0 runner    (1001) docker     (127)     7856 2024-04-13 05:43:42.000000 pulumi_fastly-8.6.0a1712986611/pulumi_fastly/get_tls_subscription.py
--rw-r--r--   0 runner    (1001) docker     (127)     3461 2024-04-13 05:43:42.000000 pulumi_fastly-8.6.0a1712986611/pulumi_fastly/get_tls_subscription_ids.py
--rw-r--r--   0 runner    (1001) docker     (127)     6294 2024-04-13 05:43:42.000000 pulumi_fastly-8.6.0a1712986611/pulumi_fastly/get_waf_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)    11877 2024-04-13 05:43:42.000000 pulumi_fastly-8.6.0a1712986611/pulumi_fastly/kvstore.py
--rw-r--r--   0 runner    (1001) docker     (127)   470308 2024-04-13 05:43:42.000000 pulumi_fastly-8.6.0a1712986611/pulumi_fastly/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     8428 2024-04-13 05:43:42.000000 pulumi_fastly-8.6.0a1712986611/pulumi_fastly/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-13 05:43:42.000000 pulumi_fastly-8.6.0a1712986611/pulumi_fastly/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 05:43:42.000000 pulumi_fastly-8.6.0a1712986611/pulumi_fastly/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    10398 2024-04-13 05:43:42.000000 pulumi_fastly-8.6.0a1712986611/pulumi_fastly/secretstore.py
--rw-r--r--   0 runner    (1001) docker     (127)    13994 2024-04-13 05:43:42.000000 pulumi_fastly-8.6.0a1712986611/pulumi_fastly/service_acl_entries.py
--rw-r--r--   0 runner    (1001) docker     (127)    11929 2024-04-13 05:43:42.000000 pulumi_fastly-8.6.0a1712986611/pulumi_fastly/service_authorization.py
--rw-r--r--   0 runner    (1001) docker     (127)    97702 2024-04-13 05:43:42.000000 pulumi_fastly-8.6.0a1712986611/pulumi_fastly/service_compute.py
--rw-r--r--   0 runner    (1001) docker     (127)    14051 2024-04-13 05:43:42.000000 pulumi_fastly-8.6.0a1712986611/pulumi_fastly/service_dictionary_items.py
--rw-r--r--   0 runner    (1001) docker     (127)    14248 2024-04-13 05:43:42.000000 pulumi_fastly-8.6.0a1712986611/pulumi_fastly/service_dynamic_snippet_content.py
--rw-r--r--   0 runner    (1001) docker     (127)   131072 2024-04-13 05:43:42.000000 pulumi_fastly-8.6.0a1712986611/pulumi_fastly/service_vcl.py
--rw-r--r--   0 runner    (1001) docker     (127)    92270 2024-04-13 05:43:42.000000 pulumi_fastly-8.6.0a1712986611/pulumi_fastly/service_waf_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)    18014 2024-04-13 05:43:42.000000 pulumi_fastly-8.6.0a1712986611/pulumi_fastly/tls_activation.py
--rw-r--r--   0 runner    (1001) docker     (127)    23295 2024-04-13 05:43:42.000000 pulumi_fastly-8.6.0a1712986611/pulumi_fastly/tls_certificate.py
--rw-r--r--   0 runner    (1001) docker     (127)    18425 2024-04-13 05:43:42.000000 pulumi_fastly-8.6.0a1712986611/pulumi_fastly/tls_mutual_authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)    26322 2024-04-13 05:43:42.000000 pulumi_fastly-8.6.0a1712986611/pulumi_fastly/tls_platform_certificate.py
--rw-r--r--   0 runner    (1001) docker     (127)    14567 2024-04-13 05:43:42.000000 pulumi_fastly-8.6.0a1712986611/pulumi_fastly/tls_private_key.py
--rw-r--r--   0 runner    (1001) docker     (127)    35184 2024-04-13 05:43:42.000000 pulumi_fastly-8.6.0a1712986611/pulumi_fastly/tls_subscription.py
--rw-r--r--   0 runner    (1001) docker     (127)     7241 2024-04-13 05:43:42.000000 pulumi_fastly-8.6.0a1712986611/pulumi_fastly/tls_subscription_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)    11710 2024-04-13 05:43:42.000000 pulumi_fastly-8.6.0a1712986611/pulumi_fastly/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:43:48.681431 pulumi_fastly-8.6.0a1712986611/pulumi_fastly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-04-13 05:43:48.000000 pulumi_fastly-8.6.0a1712986611/pulumi_fastly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-04-13 05:43:48.000000 pulumi_fastly-8.6.0a1712986611/pulumi_fastly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 05:43:48.000000 pulumi_fastly-8.6.0a1712986611/pulumi_fastly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-13 05:43:48.000000 pulumi_fastly-8.6.0a1712986611/pulumi_fastly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-13 05:43:48.000000 pulumi_fastly-8.6.0a1712986611/pulumi_fastly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      679 2024-04-13 05:43:42.000000 pulumi_fastly-8.6.0a1712986611/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 05:43:48.681431 pulumi_fastly-8.6.0a1712986611/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:53:27.617067 pulumi_fastly-8.6.0a1713257333/
+-rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-04-16 08:53:27.613067 pulumi_fastly-8.6.0a1713257333/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-04-16 08:53:21.000000 pulumi_fastly-8.6.0a1713257333/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:53:27.613067 pulumi_fastly-8.6.0a1713257333/pulumi_fastly/
+-rw-r--r--   0 runner    (1001) docker     (127)     5702 2024-04-16 08:53:21.000000 pulumi_fastly-8.6.0a1713257333/pulumi_fastly/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   521999 2024-04-16 08:53:21.000000 pulumi_fastly-8.6.0a1713257333/pulumi_fastly/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-16 08:53:21.000000 pulumi_fastly-8.6.0a1713257333/pulumi_fastly/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24235 2024-04-16 08:53:21.000000 pulumi_fastly-8.6.0a1713257333/pulumi_fastly/alert.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:53:27.613067 pulumi_fastly-8.6.0a1713257333/pulumi_fastly/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-16 08:53:21.000000 pulumi_fastly-8.6.0a1713257333/pulumi_fastly/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-04-16 08:53:21.000000 pulumi_fastly-8.6.0a1713257333/pulumi_fastly/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-04-16 08:53:21.000000 pulumi_fastly-8.6.0a1713257333/pulumi_fastly/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13105 2024-04-16 08:53:21.000000 pulumi_fastly-8.6.0a1713257333/pulumi_fastly/configstore.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11396 2024-04-16 08:53:21.000000 pulumi_fastly-8.6.0a1713257333/pulumi_fastly/configstore_entries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-04-16 08:53:21.000000 pulumi_fastly-8.6.0a1713257333/pulumi_fastly/get_configstores.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-04-16 08:53:21.000000 pulumi_fastly-8.6.0a1713257333/pulumi_fastly/get_datacenters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6375 2024-04-16 08:53:21.000000 pulumi_fastly-8.6.0a1713257333/pulumi_fastly/get_dictionaries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4521 2024-04-16 08:53:21.000000 pulumi_fastly-8.6.0a1713257333/pulumi_fastly/get_fastly_ip_ranges.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-04-16 08:53:21.000000 pulumi_fastly-8.6.0a1713257333/pulumi_fastly/get_kvstores.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5921 2024-04-16 08:53:21.000000 pulumi_fastly-8.6.0a1713257333/pulumi_fastly/get_package_hash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-04-16 08:53:21.000000 pulumi_fastly-8.6.0a1713257333/pulumi_fastly/get_secretstores.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3072 2024-04-16 08:53:21.000000 pulumi_fastly-8.6.0a1713257333/pulumi_fastly/get_services.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6799 2024-04-16 08:53:21.000000 pulumi_fastly-8.6.0a1713257333/pulumi_fastly/get_tls_activation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4424 2024-04-16 08:53:21.000000 pulumi_fastly-8.6.0a1713257333/pulumi_fastly/get_tls_activation_ids.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9956 2024-04-16 08:53:21.000000 pulumi_fastly-8.6.0a1713257333/pulumi_fastly/get_tls_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3307 2024-04-16 08:53:21.000000 pulumi_fastly-8.6.0a1713257333/pulumi_fastly/get_tls_certificate_ids.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10865 2024-04-16 08:53:21.000000 pulumi_fastly-8.6.0a1713257333/pulumi_fastly/get_tls_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3368 2024-04-16 08:53:21.000000 pulumi_fastly-8.6.0a1713257333/pulumi_fastly/get_tls_configuration_ids.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5207 2024-04-16 08:53:21.000000 pulumi_fastly-8.6.0a1713257333/pulumi_fastly/get_tls_domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8137 2024-04-16 08:53:21.000000 pulumi_fastly-8.6.0a1713257333/pulumi_fastly/get_tls_platform_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3488 2024-04-16 08:53:21.000000 pulumi_fastly-8.6.0a1713257333/pulumi_fastly/get_tls_platform_certificate_ids.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8652 2024-04-16 08:53:21.000000 pulumi_fastly-8.6.0a1713257333/pulumi_fastly/get_tls_private_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3101 2024-04-16 08:53:21.000000 pulumi_fastly-8.6.0a1713257333/pulumi_fastly/get_tls_private_key_ids.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8453 2024-04-16 08:53:21.000000 pulumi_fastly-8.6.0a1713257333/pulumi_fastly/get_tls_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3461 2024-04-16 08:53:21.000000 pulumi_fastly-8.6.0a1713257333/pulumi_fastly/get_tls_subscription_ids.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6294 2024-04-16 08:53:21.000000 pulumi_fastly-8.6.0a1713257333/pulumi_fastly/get_waf_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11877 2024-04-16 08:53:21.000000 pulumi_fastly-8.6.0a1713257333/pulumi_fastly/kvstore.py
+-rw-r--r--   0 runner    (1001) docker     (127)   470310 2024-04-16 08:53:21.000000 pulumi_fastly-8.6.0a1713257333/pulumi_fastly/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8428 2024-04-16 08:53:21.000000 pulumi_fastly-8.6.0a1713257333/pulumi_fastly/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-16 08:53:21.000000 pulumi_fastly-8.6.0a1713257333/pulumi_fastly/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 08:53:21.000000 pulumi_fastly-8.6.0a1713257333/pulumi_fastly/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    10398 2024-04-16 08:53:21.000000 pulumi_fastly-8.6.0a1713257333/pulumi_fastly/secretstore.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13994 2024-04-16 08:53:21.000000 pulumi_fastly-8.6.0a1713257333/pulumi_fastly/service_acl_entries.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11929 2024-04-16 08:53:21.000000 pulumi_fastly-8.6.0a1713257333/pulumi_fastly/service_authorization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    97702 2024-04-16 08:53:21.000000 pulumi_fastly-8.6.0a1713257333/pulumi_fastly/service_compute.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14051 2024-04-16 08:53:21.000000 pulumi_fastly-8.6.0a1713257333/pulumi_fastly/service_dictionary_items.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14248 2024-04-16 08:53:21.000000 pulumi_fastly-8.6.0a1713257333/pulumi_fastly/service_dynamic_snippet_content.py
+-rw-r--r--   0 runner    (1001) docker     (127)   131072 2024-04-16 08:53:21.000000 pulumi_fastly-8.6.0a1713257333/pulumi_fastly/service_vcl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    92270 2024-04-16 08:53:21.000000 pulumi_fastly-8.6.0a1713257333/pulumi_fastly/service_waf_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18014 2024-04-16 08:53:21.000000 pulumi_fastly-8.6.0a1713257333/pulumi_fastly/tls_activation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23295 2024-04-16 08:53:21.000000 pulumi_fastly-8.6.0a1713257333/pulumi_fastly/tls_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22173 2024-04-16 08:53:21.000000 pulumi_fastly-8.6.0a1713257333/pulumi_fastly/tls_mutual_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26322 2024-04-16 08:53:21.000000 pulumi_fastly-8.6.0a1713257333/pulumi_fastly/tls_platform_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14567 2024-04-16 08:53:21.000000 pulumi_fastly-8.6.0a1713257333/pulumi_fastly/tls_private_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35184 2024-04-16 08:53:21.000000 pulumi_fastly-8.6.0a1713257333/pulumi_fastly/tls_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7241 2024-04-16 08:53:21.000000 pulumi_fastly-8.6.0a1713257333/pulumi_fastly/tls_subscription_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11710 2024-04-16 08:53:21.000000 pulumi_fastly-8.6.0a1713257333/pulumi_fastly/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:53:27.613067 pulumi_fastly-8.6.0a1713257333/pulumi_fastly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-04-16 08:53:27.000000 pulumi_fastly-8.6.0a1713257333/pulumi_fastly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-04-16 08:53:27.000000 pulumi_fastly-8.6.0a1713257333/pulumi_fastly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 08:53:27.000000 pulumi_fastly-8.6.0a1713257333/pulumi_fastly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-16 08:53:27.000000 pulumi_fastly-8.6.0a1713257333/pulumi_fastly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-16 08:53:27.000000 pulumi_fastly-8.6.0a1713257333/pulumi_fastly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-04-16 08:53:21.000000 pulumi_fastly-8.6.0a1713257333/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 08:53:27.617067 pulumi_fastly-8.6.0a1713257333/setup.cfg
```

### Comparing `pulumi_fastly-8.6.0a1712986611/PKG-INFO` & `pulumi_fastly-8.6.0a1713257333/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_fastly
-Version: 8.6.0a1712986611
+Version: 8.6.0a1713257333
 Summary: A Pulumi package for creating and managing fastly cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-fastly
 Keywords: pulumi,fastly
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_fastly-8.6.0a1712986611/README.md` & `pulumi_fastly-8.6.0a1713257333/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1712986611/pulumi_fastly/__init__.py` & `pulumi_fastly-8.6.0a1713257333/pulumi_fastly/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1712986611/pulumi_fastly/_inputs.py` & `pulumi_fastly-8.6.0a1713257333/pulumi_fastly/_inputs.py`

 * *Files 0% similar despite different names*

```diff
@@ -5677,15 +5677,15 @@
         :param pulumi.Input[int] check_interval: How often to run the Healthcheck in milliseconds. Default `5000`
         :param pulumi.Input[int] expected_response: The status code expected from the host. Default `200`
         :param pulumi.Input[Sequence[pulumi.Input[str]]] headers: Custom health check HTTP headers (e.g. if your health check requires an API key to be provided).
         :param pulumi.Input[str] http_version: Whether to use version 1.0 or 1.1 HTTP. Default `1.1`
         :param pulumi.Input[int] initial: When loading a config, the initial number of probes to be seen as OK. Default `3`
         :param pulumi.Input[str] method: Which HTTP method to use. Default `HEAD`
         :param pulumi.Input[int] threshold: How many Healthchecks must succeed to be considered healthy. Default `3`
-        :param pulumi.Input[int] timeout: Timeout in milliseconds. Default `500`
+        :param pulumi.Input[int] timeout: Timeout in milliseconds. Default `5000`
         :param pulumi.Input[int] window: The number of most recent Healthcheck queries to keep for this Healthcheck. Default `5`
         """
         pulumi.set(__self__, "host", host)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "path", path)
         if check_interval is not None:
             pulumi.set(__self__, "check_interval", check_interval)
@@ -5826,15 +5826,15 @@
     def threshold(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "threshold", value)
 
     @property
     @pulumi.getter
     def timeout(self) -> Optional[pulumi.Input[int]]:
         """
-        Timeout in milliseconds. Default `500`
+        Timeout in milliseconds. Default `5000`
         """
         return pulumi.get(self, "timeout")
 
     @timeout.setter
     def timeout(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "timeout", value)
```

### Comparing `pulumi_fastly-8.6.0a1712986611/pulumi_fastly/_utilities.py` & `pulumi_fastly-8.6.0a1713257333/pulumi_fastly/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1712986611/pulumi_fastly/alert.py` & `pulumi_fastly-8.6.0a1713257333/pulumi_fastly/alert.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1712986611/pulumi_fastly/config/__init__.pyi` & `pulumi_fastly-8.6.0a1713257333/pulumi_fastly/config/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1712986611/pulumi_fastly/config/vars.py` & `pulumi_fastly-8.6.0a1713257333/pulumi_fastly/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1712986611/pulumi_fastly/configstore.py` & `pulumi_fastly-8.6.0a1713257333/pulumi_fastly/configstore.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1712986611/pulumi_fastly/configstore_entries.py` & `pulumi_fastly-8.6.0a1713257333/pulumi_fastly/configstore_entries.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1712986611/pulumi_fastly/get_configstores.py` & `pulumi_fastly-8.6.0a1713257333/pulumi_fastly/get_configstores.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1712986611/pulumi_fastly/get_datacenters.py` & `pulumi_fastly-8.6.0a1713257333/pulumi_fastly/get_datacenters.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1712986611/pulumi_fastly/get_dictionaries.py` & `pulumi_fastly-8.6.0a1713257333/pulumi_fastly/get_dictionaries.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1712986611/pulumi_fastly/get_fastly_ip_ranges.py` & `pulumi_fastly-8.6.0a1713257333/pulumi_fastly/get_fastly_ip_ranges.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1712986611/pulumi_fastly/get_kvstores.py` & `pulumi_fastly-8.6.0a1713257333/pulumi_fastly/get_kvstores.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1712986611/pulumi_fastly/get_package_hash.py` & `pulumi_fastly-8.6.0a1713257333/pulumi_fastly/get_package_hash.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1712986611/pulumi_fastly/get_secretstores.py` & `pulumi_fastly-8.6.0a1713257333/pulumi_fastly/get_secretstores.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1712986611/pulumi_fastly/get_services.py` & `pulumi_fastly-8.6.0a1713257333/pulumi_fastly/get_services.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1712986611/pulumi_fastly/get_tls_activation.py` & `pulumi_fastly-8.6.0a1713257333/pulumi_fastly/get_tls_activation.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1712986611/pulumi_fastly/get_tls_activation_ids.py` & `pulumi_fastly-8.6.0a1713257333/pulumi_fastly/get_tls_activation_ids.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1712986611/pulumi_fastly/get_tls_certificate.py` & `pulumi_fastly-8.6.0a1713257333/pulumi_fastly/get_tls_certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1712986611/pulumi_fastly/get_tls_certificate_ids.py` & `pulumi_fastly-8.6.0a1713257333/pulumi_fastly/get_tls_certificate_ids.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1712986611/pulumi_fastly/get_tls_configuration.py` & `pulumi_fastly-8.6.0a1713257333/pulumi_fastly/get_tls_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1712986611/pulumi_fastly/get_tls_configuration_ids.py` & `pulumi_fastly-8.6.0a1713257333/pulumi_fastly/get_tls_configuration_ids.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1712986611/pulumi_fastly/get_tls_domain.py` & `pulumi_fastly-8.6.0a1713257333/pulumi_fastly/get_tls_domain.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1712986611/pulumi_fastly/get_tls_platform_certificate.py` & `pulumi_fastly-8.6.0a1713257333/pulumi_fastly/get_tls_platform_certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1712986611/pulumi_fastly/get_tls_platform_certificate_ids.py` & `pulumi_fastly-8.6.0a1713257333/pulumi_fastly/get_tls_platform_certificate_ids.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1712986611/pulumi_fastly/get_tls_private_key.py` & `pulumi_fastly-8.6.0a1713257333/pulumi_fastly/get_tls_private_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1712986611/pulumi_fastly/get_tls_private_key_ids.py` & `pulumi_fastly-8.6.0a1713257333/pulumi_fastly/get_tls_private_key_ids.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1712986611/pulumi_fastly/get_tls_subscription.py` & `pulumi_fastly-8.6.0a1713257333/pulumi_fastly/get_tls_subscription.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,18 +17,21 @@
 ]
 
 @pulumi.output_type
 class GetTlsSubscriptionResult:
     """
     A collection of values returned by getTlsSubscription.
     """
-    def __init__(__self__, certificate_authority=None, common_name=None, configuration_id=None, created_at=None, domains=None, id=None, state=None, updated_at=None):
+    def __init__(__self__, certificate_authority=None, certificate_ids=None, common_name=None, configuration_id=None, created_at=None, domains=None, id=None, state=None, updated_at=None):
         if certificate_authority and not isinstance(certificate_authority, str):
             raise TypeError("Expected argument 'certificate_authority' to be a str")
         pulumi.set(__self__, "certificate_authority", certificate_authority)
+        if certificate_ids and not isinstance(certificate_ids, list):
+            raise TypeError("Expected argument 'certificate_ids' to be a list")
+        pulumi.set(__self__, "certificate_ids", certificate_ids)
         if common_name and not isinstance(common_name, str):
             raise TypeError("Expected argument 'common_name' to be a str")
         pulumi.set(__self__, "common_name", common_name)
         if configuration_id and not isinstance(configuration_id, str):
             raise TypeError("Expected argument 'configuration_id' to be a str")
         pulumi.set(__self__, "configuration_id", configuration_id)
         if created_at and not isinstance(created_at, str):
@@ -52,14 +55,22 @@
     def certificate_authority(self) -> str:
         """
         The entity that issues and certifies the TLS certificates for the subscription.
         """
         return pulumi.get(self, "certificate_authority")
 
     @property
+    @pulumi.getter(name="certificateIds")
+    def certificate_ids(self) -> Sequence[str]:
+        """
+        List of certificate IDs associated with the Subscription.
+        """
+        return pulumi.get(self, "certificate_ids")
+
+    @property
     @pulumi.getter(name="commonName")
     def common_name(self) -> str:
         """
         The common name associated with the subscription generated by Fastly TLS.
         """
         return pulumi.get(self, "common_name")
 
@@ -115,14 +126,15 @@
 class AwaitableGetTlsSubscriptionResult(GetTlsSubscriptionResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
             yield self
         return GetTlsSubscriptionResult(
             certificate_authority=self.certificate_authority,
+            certificate_ids=self.certificate_ids,
             common_name=self.common_name,
             configuration_id=self.configuration_id,
             created_at=self.created_at,
             domains=self.domains,
             id=self.id,
             state=self.state,
             updated_at=self.updated_at)
@@ -159,14 +171,15 @@
     __args__['domains'] = domains
     __args__['id'] = id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('fastly:index/getTlsSubscription:getTlsSubscription', __args__, opts=opts, typ=GetTlsSubscriptionResult).value
 
     return AwaitableGetTlsSubscriptionResult(
         certificate_authority=pulumi.get(__ret__, 'certificate_authority'),
+        certificate_ids=pulumi.get(__ret__, 'certificate_ids'),
         common_name=pulumi.get(__ret__, 'common_name'),
         configuration_id=pulumi.get(__ret__, 'configuration_id'),
         created_at=pulumi.get(__ret__, 'created_at'),
         domains=pulumi.get(__ret__, 'domains'),
         id=pulumi.get(__ret__, 'id'),
         state=pulumi.get(__ret__, 'state'),
         updated_at=pulumi.get(__ret__, 'updated_at'))
```

### Comparing `pulumi_fastly-8.6.0a1712986611/pulumi_fastly/get_tls_subscription_ids.py` & `pulumi_fastly-8.6.0a1713257333/pulumi_fastly/get_tls_subscription_ids.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1712986611/pulumi_fastly/get_waf_rules.py` & `pulumi_fastly-8.6.0a1713257333/pulumi_fastly/get_waf_rules.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1712986611/pulumi_fastly/kvstore.py` & `pulumi_fastly-8.6.0a1713257333/pulumi_fastly/kvstore.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1712986611/pulumi_fastly/outputs.py` & `pulumi_fastly-8.6.0a1713257333/pulumi_fastly/outputs.py`

 * *Files 0% similar despite different names*

```diff
@@ -5157,15 +5157,15 @@
         :param int check_interval: How often to run the Healthcheck in milliseconds. Default `5000`
         :param int expected_response: The status code expected from the host. Default `200`
         :param Sequence[str] headers: Custom health check HTTP headers (e.g. if your health check requires an API key to be provided).
         :param str http_version: Whether to use version 1.0 or 1.1 HTTP. Default `1.1`
         :param int initial: When loading a config, the initial number of probes to be seen as OK. Default `3`
         :param str method: Which HTTP method to use. Default `HEAD`
         :param int threshold: How many Healthchecks must succeed to be considered healthy. Default `3`
-        :param int timeout: Timeout in milliseconds. Default `500`
+        :param int timeout: Timeout in milliseconds. Default `5000`
         :param int window: The number of most recent Healthcheck queries to keep for this Healthcheck. Default `5`
         """
         pulumi.set(__self__, "host", host)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "path", path)
         if check_interval is not None:
             pulumi.set(__self__, "check_interval", check_interval)
@@ -5266,15 +5266,15 @@
         """
         return pulumi.get(self, "threshold")
 
     @property
     @pulumi.getter
     def timeout(self) -> Optional[int]:
         """
-        Timeout in milliseconds. Default `500`
+        Timeout in milliseconds. Default `5000`
         """
         return pulumi.get(self, "timeout")
 
     @property
     @pulumi.getter
     def window(self) -> Optional[int]:
         """
```

### Comparing `pulumi_fastly-8.6.0a1712986611/pulumi_fastly/provider.py` & `pulumi_fastly-8.6.0a1713257333/pulumi_fastly/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1712986611/pulumi_fastly/secretstore.py` & `pulumi_fastly-8.6.0a1713257333/pulumi_fastly/secretstore.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1712986611/pulumi_fastly/service_acl_entries.py` & `pulumi_fastly-8.6.0a1713257333/pulumi_fastly/service_acl_entries.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1712986611/pulumi_fastly/service_authorization.py` & `pulumi_fastly-8.6.0a1713257333/pulumi_fastly/service_authorization.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1712986611/pulumi_fastly/service_compute.py` & `pulumi_fastly-8.6.0a1713257333/pulumi_fastly/service_compute.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1712986611/pulumi_fastly/service_dictionary_items.py` & `pulumi_fastly-8.6.0a1713257333/pulumi_fastly/service_dictionary_items.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1712986611/pulumi_fastly/service_dynamic_snippet_content.py` & `pulumi_fastly-8.6.0a1713257333/pulumi_fastly/service_dynamic_snippet_content.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1712986611/pulumi_fastly/service_vcl.py` & `pulumi_fastly-8.6.0a1713257333/pulumi_fastly/service_vcl.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1712986611/pulumi_fastly/service_waf_configuration.py` & `pulumi_fastly-8.6.0a1713257333/pulumi_fastly/service_waf_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1712986611/pulumi_fastly/tls_activation.py` & `pulumi_fastly-8.6.0a1713257333/pulumi_fastly/tls_activation.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1712986611/pulumi_fastly/tls_certificate.py` & `pulumi_fastly-8.6.0a1713257333/pulumi_fastly/tls_certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1712986611/pulumi_fastly/tls_mutual_authentication.py` & `pulumi_fastly-8.6.0a1713257333/pulumi_fastly/tls_mutual_authentication.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,25 +11,30 @@
 
 __all__ = ['TlsMutualAuthenticationArgs', 'TlsMutualAuthentication']
 
 @pulumi.input_type
 class TlsMutualAuthenticationArgs:
     def __init__(__self__, *,
                  cert_bundle: pulumi.Input[str],
+                 activation_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  enforced: Optional[pulumi.Input[bool]] = None,
                  include: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a TlsMutualAuthentication resource.
         :param pulumi.Input[str] cert_bundle: One or more certificates. Enter each individual certificate blob on a new line. Must be PEM-formatted.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] activation_ids: List of TLS Activation IDs
         :param pulumi.Input[bool] enforced: Determines whether Mutual TLS will fail closed (enforced) or fail open. A true value will require a successful Mutual TLS handshake for the connection to continue and will fail closed if unsuccessful. A false value will fail open and allow the connection to proceed (if this attribute is not set we default to `false`).
-        :param pulumi.Input[str] include: Comma-separated list of related objects to include (e.g. `tls_activations` will provide you with the TLS domain names that are related to your Mutual TLS authentication).
+        :param pulumi.Input[str] include: A comma-separated list used by the Terraform provider during a state refresh to return more data related to your mutual
+               authentication from the Fastly API (permitted values: `tls_activations`).
         :param pulumi.Input[str] name: A custom name for your mutual authentication. If name is not supplied we will auto-generate one.
         """
         pulumi.set(__self__, "cert_bundle", cert_bundle)
+        if activation_ids is not None:
+            pulumi.set(__self__, "activation_ids", activation_ids)
         if enforced is not None:
             pulumi.set(__self__, "enforced", enforced)
         if include is not None:
             pulumi.set(__self__, "include", include)
         if name is not None:
             pulumi.set(__self__, "name", name)
 
@@ -42,14 +47,26 @@
         return pulumi.get(self, "cert_bundle")
 
     @cert_bundle.setter
     def cert_bundle(self, value: pulumi.Input[str]):
         pulumi.set(self, "cert_bundle", value)
 
     @property
+    @pulumi.getter(name="activationIds")
+    def activation_ids(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+        """
+        List of TLS Activation IDs
+        """
+        return pulumi.get(self, "activation_ids")
+
+    @activation_ids.setter
+    def activation_ids(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "activation_ids", value)
+
+    @property
     @pulumi.getter
     def enforced(self) -> Optional[pulumi.Input[bool]]:
         """
         Determines whether Mutual TLS will fail closed (enforced) or fail open. A true value will require a successful Mutual TLS handshake for the connection to continue and will fail closed if unsuccessful. A false value will fail open and allow the connection to proceed (if this attribute is not set we default to `false`).
         """
         return pulumi.get(self, "enforced")
 
@@ -57,15 +74,16 @@
     def enforced(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "enforced", value)
 
     @property
     @pulumi.getter
     def include(self) -> Optional[pulumi.Input[str]]:
         """
-        Comma-separated list of related objects to include (e.g. `tls_activations` will provide you with the TLS domain names that are related to your Mutual TLS authentication).
+        A comma-separated list used by the Terraform provider during a state refresh to return more data related to your mutual
+        authentication from the Fastly API (permitted values: `tls_activations`).
         """
         return pulumi.get(self, "include")
 
     @include.setter
     def include(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "include", value)
 
@@ -81,31 +99,36 @@
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
 
 @pulumi.input_type
 class _TlsMutualAuthenticationState:
     def __init__(__self__, *,
+                 activation_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  cert_bundle: Optional[pulumi.Input[str]] = None,
                  created_at: Optional[pulumi.Input[str]] = None,
                  enforced: Optional[pulumi.Input[bool]] = None,
                  include: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  tls_activations: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  updated_at: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering TlsMutualAuthentication resources.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] activation_ids: List of TLS Activation IDs
         :param pulumi.Input[str] cert_bundle: One or more certificates. Enter each individual certificate blob on a new line. Must be PEM-formatted.
         :param pulumi.Input[str] created_at: Date and time in ISO 8601 format.
         :param pulumi.Input[bool] enforced: Determines whether Mutual TLS will fail closed (enforced) or fail open. A true value will require a successful Mutual TLS handshake for the connection to continue and will fail closed if unsuccessful. A false value will fail open and allow the connection to proceed (if this attribute is not set we default to `false`).
-        :param pulumi.Input[str] include: Comma-separated list of related objects to include (e.g. `tls_activations` will provide you with the TLS domain names that are related to your Mutual TLS authentication).
+        :param pulumi.Input[str] include: A comma-separated list used by the Terraform provider during a state refresh to return more data related to your mutual
+               authentication from the Fastly API (permitted values: `tls_activations`).
         :param pulumi.Input[str] name: A custom name for your mutual authentication. If name is not supplied we will auto-generate one.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] tls_activations: List of alphanumeric strings identifying TLS activations.
         :param pulumi.Input[str] updated_at: Date and time in ISO 8601 format.
         """
+        if activation_ids is not None:
+            pulumi.set(__self__, "activation_ids", activation_ids)
         if cert_bundle is not None:
             pulumi.set(__self__, "cert_bundle", cert_bundle)
         if created_at is not None:
             pulumi.set(__self__, "created_at", created_at)
         if enforced is not None:
             pulumi.set(__self__, "enforced", enforced)
         if include is not None:
@@ -114,14 +137,26 @@
             pulumi.set(__self__, "name", name)
         if tls_activations is not None:
             pulumi.set(__self__, "tls_activations", tls_activations)
         if updated_at is not None:
             pulumi.set(__self__, "updated_at", updated_at)
 
     @property
+    @pulumi.getter(name="activationIds")
+    def activation_ids(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+        """
+        List of TLS Activation IDs
+        """
+        return pulumi.get(self, "activation_ids")
+
+    @activation_ids.setter
+    def activation_ids(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "activation_ids", value)
+
+    @property
     @pulumi.getter(name="certBundle")
     def cert_bundle(self) -> Optional[pulumi.Input[str]]:
         """
         One or more certificates. Enter each individual certificate blob on a new line. Must be PEM-formatted.
         """
         return pulumi.get(self, "cert_bundle")
 
@@ -153,15 +188,16 @@
     def enforced(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "enforced", value)
 
     @property
     @pulumi.getter
     def include(self) -> Optional[pulumi.Input[str]]:
         """
-        Comma-separated list of related objects to include (e.g. `tls_activations` will provide you with the TLS domain names that are related to your Mutual TLS authentication).
+        A comma-separated list used by the Terraform provider during a state refresh to return more data related to your mutual
+        authentication from the Fastly API (permitted values: `tls_activations`).
         """
         return pulumi.get(self, "include")
 
     @include.setter
     def include(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "include", value)
 
@@ -203,36 +239,53 @@
 
 
 class TlsMutualAuthentication(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
+                 activation_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  cert_bundle: Optional[pulumi.Input[str]] = None,
                  enforced: Optional[pulumi.Input[bool]] = None,
                  include: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
-        Create a TlsMutualAuthentication resource with the given unique name, props, and options.
+        The Mutual TLS API allows for client-to-server authentication using client-side X.509 authentication.
+
+        The main Mutual Authentication object represents the certificate bundle and other configurations which support Mutual TLS for your domains.
+
+        Mutual TLS can be added to existing TLS activations to allow for client-to-server authentication. In order to use mutual TLS, you must already have active server-side TLS using either custom certificates or an enabled Fastly-managed subscription.
+
+        The examples below demonstrate how to use Mutual Authentication along with a TLS Subscription. Refer to the `TlsSubscription` resource documentation for a deeper explanation of that code.
+
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] activation_ids: List of TLS Activation IDs
         :param pulumi.Input[str] cert_bundle: One or more certificates. Enter each individual certificate blob on a new line. Must be PEM-formatted.
         :param pulumi.Input[bool] enforced: Determines whether Mutual TLS will fail closed (enforced) or fail open. A true value will require a successful Mutual TLS handshake for the connection to continue and will fail closed if unsuccessful. A false value will fail open and allow the connection to proceed (if this attribute is not set we default to `false`).
-        :param pulumi.Input[str] include: Comma-separated list of related objects to include (e.g. `tls_activations` will provide you with the TLS domain names that are related to your Mutual TLS authentication).
+        :param pulumi.Input[str] include: A comma-separated list used by the Terraform provider during a state refresh to return more data related to your mutual
+               authentication from the Fastly API (permitted values: `tls_activations`).
         :param pulumi.Input[str] name: A custom name for your mutual authentication. If name is not supplied we will auto-generate one.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: TlsMutualAuthenticationArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Create a TlsMutualAuthentication resource with the given unique name, props, and options.
+        The Mutual TLS API allows for client-to-server authentication using client-side X.509 authentication.
+
+        The main Mutual Authentication object represents the certificate bundle and other configurations which support Mutual TLS for your domains.
+
+        Mutual TLS can be added to existing TLS activations to allow for client-to-server authentication. In order to use mutual TLS, you must already have active server-side TLS using either custom certificates or an enabled Fastly-managed subscription.
+
+        The examples below demonstrate how to use Mutual Authentication along with a TLS Subscription. Refer to the `TlsSubscription` resource documentation for a deeper explanation of that code.
+
         :param str resource_name: The name of the resource.
         :param TlsMutualAuthenticationArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
         resource_args, opts = _utilities.get_resource_args_opts(TlsMutualAuthenticationArgs, pulumi.ResourceOptions, *args, **kwargs)
@@ -240,27 +293,29 @@
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
+                 activation_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  cert_bundle: Optional[pulumi.Input[str]] = None,
                  enforced: Optional[pulumi.Input[bool]] = None,
                  include: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = TlsMutualAuthenticationArgs.__new__(TlsMutualAuthenticationArgs)
 
+            __props__.__dict__["activation_ids"] = activation_ids
             if cert_bundle is None and not opts.urn:
                 raise TypeError("Missing required property 'cert_bundle'")
             __props__.__dict__["cert_bundle"] = cert_bundle
             __props__.__dict__["enforced"] = enforced
             __props__.__dict__["include"] = include
             __props__.__dict__["name"] = name
             __props__.__dict__["created_at"] = None
@@ -272,50 +327,62 @@
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
+            activation_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
             cert_bundle: Optional[pulumi.Input[str]] = None,
             created_at: Optional[pulumi.Input[str]] = None,
             enforced: Optional[pulumi.Input[bool]] = None,
             include: Optional[pulumi.Input[str]] = None,
             name: Optional[pulumi.Input[str]] = None,
             tls_activations: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
             updated_at: Optional[pulumi.Input[str]] = None) -> 'TlsMutualAuthentication':
         """
         Get an existing TlsMutualAuthentication resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] activation_ids: List of TLS Activation IDs
         :param pulumi.Input[str] cert_bundle: One or more certificates. Enter each individual certificate blob on a new line. Must be PEM-formatted.
         :param pulumi.Input[str] created_at: Date and time in ISO 8601 format.
         :param pulumi.Input[bool] enforced: Determines whether Mutual TLS will fail closed (enforced) or fail open. A true value will require a successful Mutual TLS handshake for the connection to continue and will fail closed if unsuccessful. A false value will fail open and allow the connection to proceed (if this attribute is not set we default to `false`).
-        :param pulumi.Input[str] include: Comma-separated list of related objects to include (e.g. `tls_activations` will provide you with the TLS domain names that are related to your Mutual TLS authentication).
+        :param pulumi.Input[str] include: A comma-separated list used by the Terraform provider during a state refresh to return more data related to your mutual
+               authentication from the Fastly API (permitted values: `tls_activations`).
         :param pulumi.Input[str] name: A custom name for your mutual authentication. If name is not supplied we will auto-generate one.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] tls_activations: List of alphanumeric strings identifying TLS activations.
         :param pulumi.Input[str] updated_at: Date and time in ISO 8601 format.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _TlsMutualAuthenticationState.__new__(_TlsMutualAuthenticationState)
 
+        __props__.__dict__["activation_ids"] = activation_ids
         __props__.__dict__["cert_bundle"] = cert_bundle
         __props__.__dict__["created_at"] = created_at
         __props__.__dict__["enforced"] = enforced
         __props__.__dict__["include"] = include
         __props__.__dict__["name"] = name
         __props__.__dict__["tls_activations"] = tls_activations
         __props__.__dict__["updated_at"] = updated_at
         return TlsMutualAuthentication(resource_name, opts=opts, __props__=__props__)
 
     @property
+    @pulumi.getter(name="activationIds")
+    def activation_ids(self) -> pulumi.Output[Optional[Sequence[str]]]:
+        """
+        List of TLS Activation IDs
+        """
+        return pulumi.get(self, "activation_ids")
+
+    @property
     @pulumi.getter(name="certBundle")
     def cert_bundle(self) -> pulumi.Output[str]:
         """
         One or more certificates. Enter each individual certificate blob on a new line. Must be PEM-formatted.
         """
         return pulumi.get(self, "cert_bundle")
 
@@ -335,15 +402,16 @@
         """
         return pulumi.get(self, "enforced")
 
     @property
     @pulumi.getter
     def include(self) -> pulumi.Output[Optional[str]]:
         """
-        Comma-separated list of related objects to include (e.g. `tls_activations` will provide you with the TLS domain names that are related to your Mutual TLS authentication).
+        A comma-separated list used by the Terraform provider during a state refresh to return more data related to your mutual
+        authentication from the Fastly API (permitted values: `tls_activations`).
         """
         return pulumi.get(self, "include")
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Output[str]:
         """
```

### Comparing `pulumi_fastly-8.6.0a1712986611/pulumi_fastly/tls_platform_certificate.py` & `pulumi_fastly-8.6.0a1713257333/pulumi_fastly/tls_platform_certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1712986611/pulumi_fastly/tls_private_key.py` & `pulumi_fastly-8.6.0a1713257333/pulumi_fastly/tls_private_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1712986611/pulumi_fastly/tls_subscription.py` & `pulumi_fastly-8.6.0a1713257333/pulumi_fastly/tls_subscription.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1712986611/pulumi_fastly/tls_subscription_validation.py` & `pulumi_fastly-8.6.0a1713257333/pulumi_fastly/tls_subscription_validation.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1712986611/pulumi_fastly/user.py` & `pulumi_fastly-8.6.0a1713257333/pulumi_fastly/user.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1712986611/pulumi_fastly.egg-info/PKG-INFO` & `pulumi_fastly-8.6.0a1713257333/pulumi_fastly.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_fastly
-Version: 8.6.0a1712986611
+Version: 8.6.0a1713257333
 Summary: A Pulumi package for creating and managing fastly cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-fastly
 Keywords: pulumi,fastly
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_fastly-8.6.0a1712986611/pulumi_fastly.egg-info/SOURCES.txt` & `pulumi_fastly-8.6.0a1713257333/pulumi_fastly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.6.0a1712986611/pyproject.toml` & `pulumi_fastly-8.6.0a1713257333/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_fastly"
   description = "A Pulumi package for creating and managing fastly cloud resources."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "fastly"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "8.6.0a1712986611"
+  version = "8.6.0a1713257333"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://pulumi.io"
     Repository = "https://github.com/pulumi/pulumi-fastly"
 
 [build-system]
```

