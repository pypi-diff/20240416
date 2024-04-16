# Comparing `tmp/permit-2.4.0.tar.gz` & `tmp/permit-2.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "permit-2.4.0.tar", last modified: Thu Apr 11 18:30:39 2024, max compression
+gzip compressed data, was "permit-2.4.1.tar", last modified: Tue Apr 16 15:03:41 2024, max compression
```

## Comparing `permit-2.4.0.tar` & `permit-2.4.1.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:30:39.445193 permit-2.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-11 18:29:07.000000 permit-2.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-11 18:29:07.000000 permit-2.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-11 18:30:39.445193 permit-2.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-11 18:29:07.000000 permit-2.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:30:39.441193 permit-2.4.0/permit/
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-11 18:29:07.000000 permit-2.4.0/permit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:30:39.445193 permit-2.4.0/permit/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 18:29:07.000000 permit-2.4.0/permit/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5622 2024-04-11 18:29:07.000000 permit-2.4.0/permit/api/api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    11982 2024-04-11 18:29:07.000000 permit-2.4.0/permit/api/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4020 2024-04-11 18:29:07.000000 permit-2.4.0/permit/api/condition_set_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)     6218 2024-04-11 18:29:07.000000 permit-2.4.0/permit/api/condition_sets.py
--rw-r--r--   0 runner    (1001) docker     (127)     8347 2024-04-11 18:29:07.000000 permit-2.4.0/permit/api/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     6493 2024-04-11 18:29:07.000000 permit-2.4.0/permit/api/deprecated.py
--rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-04-11 18:29:07.000000 permit-2.4.0/permit/api/elements.py
--rw-r--r--   0 runner    (1001) docker     (127)     9818 2024-04-11 18:29:07.000000 permit-2.4.0/permit/api/environments.py
--rw-r--r--   0 runner    (1001) docker     (127)   160550 2024-04-11 18:29:07.000000 permit-2.4.0/permit/api/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     5864 2024-04-11 18:29:07.000000 permit-2.4.0/permit/api/projects.py
--rw-r--r--   0 runner    (1001) docker     (127)     6510 2024-04-11 18:29:07.000000 permit-2.4.0/permit/api/relationship_tuples.py
--rw-r--r--   0 runner    (1001) docker     (127)     7176 2024-04-11 18:29:07.000000 permit-2.4.0/permit/api/resource_action_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     6842 2024-04-11 18:29:07.000000 permit-2.4.0/permit/api/resource_actions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7148 2024-04-11 18:29:07.000000 permit-2.4.0/permit/api/resource_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     9617 2024-04-11 18:29:07.000000 permit-2.4.0/permit/api/resource_instances.py
--rw-r--r--   0 runner    (1001) docker     (127)     5941 2024-04-11 18:29:07.000000 permit-2.4.0/permit/api/resource_relations.py
--rw-r--r--   0 runner    (1001) docker     (127)    12471 2024-04-11 18:29:07.000000 permit-2.4.0/permit/api/resource_roles.py
--rw-r--r--   0 runner    (1001) docker     (127)     6814 2024-04-11 18:29:07.000000 permit-2.4.0/permit/api/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     6265 2024-04-11 18:29:07.000000 permit-2.4.0/permit/api/role_assignments.py
--rw-r--r--   0 runner    (1001) docker     (127)     7541 2024-04-11 18:29:07.000000 permit-2.4.0/permit/api/roles.py
--rw-r--r--   0 runner    (1001) docker     (127)     7125 2024-04-11 18:29:07.000000 permit-2.4.0/permit/api/sync_api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     9843 2024-04-11 18:29:07.000000 permit-2.4.0/permit/api/tenants.py
--rw-r--r--   0 runner    (1001) docker     (127)    12949 2024-04-11 18:29:07.000000 permit-2.4.0/permit/api/users.py
--rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-04-11 18:29:07.000000 permit-2.4.0/permit/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:30:39.445193 permit-2.4.0/permit/enforcement/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 18:29:07.000000 permit-2.4.0/permit/enforcement/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13219 2024-04-11 18:29:07.000000 permit-2.4.0/permit/enforcement/enforcer.py
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-11 18:29:07.000000 permit-2.4.0/permit/enforcement/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (127)     3933 2024-04-11 18:29:07.000000 permit-2.4.0/permit/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-11 18:29:07.000000 permit-2.4.0/permit/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:30:39.445193 permit-2.4.0/permit/pdp_api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 18:29:07.000000 permit-2.4.0/permit/pdp_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-04-11 18:29:07.000000 permit-2.4.0/permit/pdp_api/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-11 18:29:07.000000 permit-2.4.0/permit/pdp_api/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-11 18:29:07.000000 permit-2.4.0/permit/pdp_api/pdp_api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-04-11 18:29:07.000000 permit-2.4.0/permit/pdp_api/role_assignments.py
--rw-r--r--   0 runner    (1001) docker     (127)     4958 2024-04-11 18:29:07.000000 permit-2.4.0/permit/permit.py
--rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-04-11 18:29:07.000000 permit-2.4.0/permit/sync.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:30:39.445193 permit-2.4.0/permit/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 18:29:07.000000 permit-2.4.0/permit/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-04-11 18:29:07.000000 permit-2.4.0/permit/utils/context.py
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-11 18:29:07.000000 permit-2.4.0/permit/utils/deprecation.py
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-11 18:29:07.000000 permit-2.4.0/permit/utils/dicts.py
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-11 18:29:07.000000 permit-2.4.0/permit/utils/pydantic_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-11 18:29:07.000000 permit-2.4.0/permit/utils/sync.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:30:39.441193 permit-2.4.0/permit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-11 18:30:39.000000 permit-2.4.0/permit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-04-11 18:30:39.000000 permit-2.4.0/permit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 18:30:39.000000 permit-2.4.0/permit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-11 18:30:39.000000 permit-2.4.0/permit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-11 18:30:39.000000 permit-2.4.0/permit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-11 18:29:07.000000 permit-2.4.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 18:30:39.445193 permit-2.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-11 18:30:37.000000 permit-2.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:30:39.445193 permit-2.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 18:29:07.000000 permit-2.4.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-04-11 18:29:07.000000 permit-2.4.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    10459 2024-04-11 18:29:07.000000 permit-2.4.0/tests/test_abac_e2e.py
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-11 18:29:07.000000 permit-2.4.0/tests/test_abac_pdp.py
--rw-r--r--   0 runner    (1001) docker     (127)    10396 2024-04-11 18:29:07.000000 permit-2.4.0/tests/test_rbac_e2e.py
--rw-r--r--   0 runner    (1001) docker     (127)     9688 2024-04-11 18:29:07.000000 permit-2.4.0/tests/test_rbac_e2e_sync.py
--rw-r--r--   0 runner    (1001) docker     (127)    30220 2024-04-11 18:29:07.000000 permit-2.4.0/tests/test_rebac_e2e.py
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-11 18:29:07.000000 permit-2.4.0/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:03:41.370129 permit-2.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-16 15:02:26.000000 permit-2.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-16 15:02:26.000000 permit-2.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-16 15:03:41.370129 permit-2.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-16 15:02:26.000000 permit-2.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:03:41.366129 permit-2.4.1/permit/
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-16 15:02:26.000000 permit-2.4.1/permit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:03:41.370129 permit-2.4.1/permit/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 15:02:26.000000 permit-2.4.1/permit/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5622 2024-04-16 15:02:26.000000 permit-2.4.1/permit/api/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11982 2024-04-16 15:02:26.000000 permit-2.4.1/permit/api/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4020 2024-04-16 15:02:26.000000 permit-2.4.1/permit/api/condition_set_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6218 2024-04-16 15:02:26.000000 permit-2.4.1/permit/api/condition_sets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8347 2024-04-16 15:02:26.000000 permit-2.4.1/permit/api/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6493 2024-04-16 15:02:26.000000 permit-2.4.1/permit/api/deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-04-16 15:02:26.000000 permit-2.4.1/permit/api/elements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9818 2024-04-16 15:02:26.000000 permit-2.4.1/permit/api/environments.py
+-rw-r--r--   0 runner    (1001) docker     (127)   160550 2024-04-16 15:02:26.000000 permit-2.4.1/permit/api/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5864 2024-04-16 15:02:26.000000 permit-2.4.1/permit/api/projects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6510 2024-04-16 15:02:26.000000 permit-2.4.1/permit/api/relationship_tuples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7176 2024-04-16 15:02:26.000000 permit-2.4.1/permit/api/resource_action_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6842 2024-04-16 15:02:26.000000 permit-2.4.1/permit/api/resource_actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7148 2024-04-16 15:02:26.000000 permit-2.4.1/permit/api/resource_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9617 2024-04-16 15:02:26.000000 permit-2.4.1/permit/api/resource_instances.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5941 2024-04-16 15:02:26.000000 permit-2.4.1/permit/api/resource_relations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12471 2024-04-16 15:02:26.000000 permit-2.4.1/permit/api/resource_roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6814 2024-04-16 15:02:26.000000 permit-2.4.1/permit/api/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6265 2024-04-16 15:02:26.000000 permit-2.4.1/permit/api/role_assignments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7541 2024-04-16 15:02:26.000000 permit-2.4.1/permit/api/roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7125 2024-04-16 15:02:26.000000 permit-2.4.1/permit/api/sync_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9843 2024-04-16 15:02:26.000000 permit-2.4.1/permit/api/tenants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12949 2024-04-16 15:02:26.000000 permit-2.4.1/permit/api/users.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-04-16 15:02:26.000000 permit-2.4.1/permit/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:03:41.370129 permit-2.4.1/permit/enforcement/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 15:02:26.000000 permit-2.4.1/permit/enforcement/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13219 2024-04-16 15:02:26.000000 permit-2.4.1/permit/enforcement/enforcer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-16 15:02:26.000000 permit-2.4.1/permit/enforcement/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3933 2024-04-16 15:02:26.000000 permit-2.4.1/permit/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-16 15:02:26.000000 permit-2.4.1/permit/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:03:41.370129 permit-2.4.1/permit/pdp_api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 15:02:26.000000 permit-2.4.1/permit/pdp_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-04-16 15:02:26.000000 permit-2.4.1/permit/pdp_api/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-16 15:02:26.000000 permit-2.4.1/permit/pdp_api/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-16 15:02:26.000000 permit-2.4.1/permit/pdp_api/pdp_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-04-16 15:02:26.000000 permit-2.4.1/permit/pdp_api/role_assignments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4958 2024-04-16 15:02:26.000000 permit-2.4.1/permit/permit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4019 2024-04-16 15:02:26.000000 permit-2.4.1/permit/sync.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:03:41.370129 permit-2.4.1/permit/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 15:02:26.000000 permit-2.4.1/permit/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-04-16 15:02:26.000000 permit-2.4.1/permit/utils/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-16 15:02:26.000000 permit-2.4.1/permit/utils/deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-16 15:02:26.000000 permit-2.4.1/permit/utils/dicts.py
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-16 15:02:26.000000 permit-2.4.1/permit/utils/pydantic_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-16 15:02:26.000000 permit-2.4.1/permit/utils/sync.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:03:41.366129 permit-2.4.1/permit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-16 15:03:41.000000 permit-2.4.1/permit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-04-16 15:03:41.000000 permit-2.4.1/permit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 15:03:41.000000 permit-2.4.1/permit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-16 15:03:41.000000 permit-2.4.1/permit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-16 15:03:41.000000 permit-2.4.1/permit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-16 15:02:26.000000 permit-2.4.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 15:03:41.370129 permit-2.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-16 15:03:40.000000 permit-2.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:03:41.370129 permit-2.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 15:02:26.000000 permit-2.4.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-04-16 15:02:26.000000 permit-2.4.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10459 2024-04-16 15:02:26.000000 permit-2.4.1/tests/test_abac_e2e.py
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-16 15:02:26.000000 permit-2.4.1/tests/test_abac_pdp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10396 2024-04-16 15:02:26.000000 permit-2.4.1/tests/test_rbac_e2e.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9688 2024-04-16 15:02:26.000000 permit-2.4.1/tests/test_rbac_e2e_sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30220 2024-04-16 15:02:26.000000 permit-2.4.1/tests/test_rebac_e2e.py
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-16 15:02:26.000000 permit-2.4.1/tests/utils.py
```

### Comparing `permit-2.4.0/LICENSE` & `permit-2.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `permit-2.4.0/PKG-INFO` & `permit-2.4.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: permit
-Version: 2.4.0
+Version: 2.4.1
 Summary: Permit.io python sdk
 Author: Asaf Cohen
 Author-email: asaf@permit.io
 License: Apache 2.0
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+![Python.png](imgs/Python.png)
 # Permit.io Python SDK
 
 Python SDK for interacting with the Permit.io full-stack permissions platform.
 
 ## Installation
 
 ```py
```

### Comparing `permit-2.4.0/permit/api/api_client.py` & `permit-2.4.1/permit/api/api_client.py`

 * *Files identical despite different names*

### Comparing `permit-2.4.0/permit/api/base.py` & `permit-2.4.1/permit/api/base.py`

 * *Files identical despite different names*

### Comparing `permit-2.4.0/permit/api/condition_set_rules.py` & `permit-2.4.1/permit/api/condition_set_rules.py`

 * *Files identical despite different names*

### Comparing `permit-2.4.0/permit/api/condition_sets.py` & `permit-2.4.1/permit/api/condition_sets.py`

 * *Files identical despite different names*

### Comparing `permit-2.4.0/permit/api/context.py` & `permit-2.4.1/permit/api/context.py`

 * *Files identical despite different names*

### Comparing `permit-2.4.0/permit/api/deprecated.py` & `permit-2.4.1/permit/api/deprecated.py`

 * *Files identical despite different names*

### Comparing `permit-2.4.0/permit/api/elements.py` & `permit-2.4.1/permit/api/elements.py`

 * *Files identical despite different names*

### Comparing `permit-2.4.0/permit/api/environments.py` & `permit-2.4.1/permit/api/environments.py`

 * *Files identical despite different names*

### Comparing `permit-2.4.0/permit/api/models.py` & `permit-2.4.1/permit/api/models.py`

 * *Files identical despite different names*

### Comparing `permit-2.4.0/permit/api/projects.py` & `permit-2.4.1/permit/api/projects.py`

 * *Files identical despite different names*

### Comparing `permit-2.4.0/permit/api/relationship_tuples.py` & `permit-2.4.1/permit/api/relationship_tuples.py`

 * *Files identical despite different names*

### Comparing `permit-2.4.0/permit/api/resource_action_groups.py` & `permit-2.4.1/permit/api/resource_action_groups.py`

 * *Files identical despite different names*

### Comparing `permit-2.4.0/permit/api/resource_actions.py` & `permit-2.4.1/permit/api/resource_actions.py`

 * *Files identical despite different names*

### Comparing `permit-2.4.0/permit/api/resource_attributes.py` & `permit-2.4.1/permit/api/resource_attributes.py`

 * *Files identical despite different names*

### Comparing `permit-2.4.0/permit/api/resource_instances.py` & `permit-2.4.1/permit/api/resource_instances.py`

 * *Files identical despite different names*

### Comparing `permit-2.4.0/permit/api/resource_relations.py` & `permit-2.4.1/permit/api/resource_relations.py`

 * *Files identical despite different names*

### Comparing `permit-2.4.0/permit/api/resource_roles.py` & `permit-2.4.1/permit/api/resource_roles.py`

 * *Files identical despite different names*

### Comparing `permit-2.4.0/permit/api/resources.py` & `permit-2.4.1/permit/api/resources.py`

 * *Files identical despite different names*

### Comparing `permit-2.4.0/permit/api/role_assignments.py` & `permit-2.4.1/permit/api/role_assignments.py`

 * *Files identical despite different names*

### Comparing `permit-2.4.0/permit/api/roles.py` & `permit-2.4.1/permit/api/roles.py`

 * *Files identical despite different names*

### Comparing `permit-2.4.0/permit/api/sync_api_client.py` & `permit-2.4.1/permit/api/sync_api_client.py`

 * *Files identical despite different names*

### Comparing `permit-2.4.0/permit/api/tenants.py` & `permit-2.4.1/permit/api/tenants.py`

 * *Files identical despite different names*

### Comparing `permit-2.4.0/permit/api/users.py` & `permit-2.4.1/permit/api/users.py`

 * *Files identical despite different names*

### Comparing `permit-2.4.0/permit/config.py` & `permit-2.4.1/permit/config.py`

 * *Files identical despite different names*

### Comparing `permit-2.4.0/permit/enforcement/enforcer.py` & `permit-2.4.1/permit/enforcement/enforcer.py`

 * *Files identical despite different names*

### Comparing `permit-2.4.0/permit/enforcement/interfaces.py` & `permit-2.4.1/permit/enforcement/interfaces.py`

 * *Files identical despite different names*

### Comparing `permit-2.4.0/permit/exceptions.py` & `permit-2.4.1/permit/exceptions.py`

 * *Files identical despite different names*

### Comparing `permit-2.4.0/permit/pdp_api/base.py` & `permit-2.4.1/permit/pdp_api/base.py`

 * *Files identical despite different names*

### Comparing `permit-2.4.0/permit/pdp_api/models.py` & `permit-2.4.1/permit/pdp_api/models.py`

 * *Files identical despite different names*

### Comparing `permit-2.4.0/permit/pdp_api/pdp_api_client.py` & `permit-2.4.1/permit/pdp_api/pdp_api_client.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from permit.utils.sync import SyncClass
+
 from ..config import PermitConfig
 from .role_assignments import RoleAssignmentsApi
 
 
 class PermitPdpApiClient:
     def __init__(self, config: PermitConfig):
         """
@@ -18,7 +20,11 @@
         self._base_url = self._config.pdp
 
         self._role_assignments = RoleAssignmentsApi(config)
 
     @property
     def role_assignments(self) -> RoleAssignmentsApi:
         return self._role_assignments
+
+
+class SyncPDPApi(PermitPdpApiClient, metaclass=SyncClass):
+    pass
```

### Comparing `permit-2.4.0/permit/pdp_api/role_assignments.py` & `permit-2.4.1/permit/pdp_api/role_assignments.py`

 * *Files identical despite different names*

### Comparing `permit-2.4.0/permit/permit.py` & `permit-2.4.1/permit/permit.py`

 * *Files identical despite different names*

### Comparing `permit-2.4.0/permit/sync.py` & `permit-2.4.1/permit/sync.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 from typing import Optional
 
 from .api.elements import SyncElementsApi
 from .api.sync_api_client import SyncPermitApiClient
 from .config import PermitConfig
 from .enforcement.enforcer import Action, CheckQuery, Resource, SyncEnforcer, User
+from .pdp_api.pdp_api_client import SyncPDPApi
 from .permit import Permit as AsyncPermit
 from .utils.context import Context
 
 
 class Permit(AsyncPermit):
     def __init__(self, config: Optional[PermitConfig] = None, **options):
         super().__init__(config, **options)
         self._enforcer = SyncEnforcer(self._config)
         self._api = SyncPermitApiClient(self._config)
         self._elements = SyncElementsApi(self._config)
+        self._pdp_api = SyncPDPApi(self._config)
 
     @property
     def api(self) -> SyncPermitApiClient:
         """
         Access the Permit REST API using this property.
 
         Usage example:
```

### Comparing `permit-2.4.0/permit/utils/context.py` & `permit-2.4.1/permit/utils/context.py`

 * *Files identical despite different names*

### Comparing `permit-2.4.0/permit/utils/deprecation.py` & `permit-2.4.1/permit/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `permit-2.4.0/permit/utils/sync.py` & `permit-2.4.1/permit/utils/sync.py`

 * *Files identical despite different names*

### Comparing `permit-2.4.0/permit.egg-info/PKG-INFO` & `permit-2.4.1/permit.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: permit
-Version: 2.4.0
+Version: 2.4.1
 Summary: Permit.io python sdk
 Author: Asaf Cohen
 Author-email: asaf@permit.io
 License: Apache 2.0
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+![Python.png](imgs/Python.png)
 # Permit.io Python SDK
 
 Python SDK for interacting with the Permit.io full-stack permissions platform.
 
 ## Installation
 
 ```py
```

### Comparing `permit-2.4.0/permit.egg-info/SOURCES.txt` & `permit-2.4.1/permit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `permit-2.4.0/setup.py` & `permit-2.4.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     this_directory = Path(__file__).parent
     long_description = (this_directory / "README.md").read_text()
     return long_description
 
 
 setup(
     name="permit",
-    version="2.4.0",
+    version="v2.4.1",
     packages=find_packages(),
     author="Asaf Cohen",
     author_email="asaf@permit.io",
     license="Apache 2.0",
     python_requires=">=3.8",
     description="Permit.io python sdk",
     install_requires=get_requirements(),
```

### Comparing `permit-2.4.0/tests/conftest.py` & `permit-2.4.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `permit-2.4.0/tests/test_abac_e2e.py` & `permit-2.4.1/tests/test_abac_e2e.py`

 * *Files identical despite different names*

### Comparing `permit-2.4.0/tests/test_abac_pdp.py` & `permit-2.4.1/tests/test_abac_pdp.py`

 * *Files identical despite different names*

### Comparing `permit-2.4.0/tests/test_rbac_e2e.py` & `permit-2.4.1/tests/test_rbac_e2e.py`

 * *Files identical despite different names*

### Comparing `permit-2.4.0/tests/test_rbac_e2e_sync.py` & `permit-2.4.1/tests/test_rbac_e2e_sync.py`

 * *Files identical despite different names*

### Comparing `permit-2.4.0/tests/test_rebac_e2e.py` & `permit-2.4.1/tests/test_rebac_e2e.py`

 * *Files identical despite different names*

