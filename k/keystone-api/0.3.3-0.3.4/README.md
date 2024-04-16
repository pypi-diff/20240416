# Comparing `tmp/keystone_api-0.3.3.tar.gz` & `tmp/keystone_api-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keystone_api-0.3.3.tar", max compression
+gzip compressed data, was "keystone_api-0.3.4.tar", max compression
```

## Comparing `keystone_api-0.3.3.tar` & `keystone_api-0.3.4.tar`

### file list

```diff
@@ -1,111 +1,111 @@
--rw-r--r--   0        0        0    13578 2024-04-08 17:43:08.833383 keystone_api-0.3.3/README.md
--rw-r--r--   0        0        0      428 2024-04-08 17:43:08.833383 keystone_api-0.3.3/keystone_api/__init__.py
--rw-r--r--   0        0        0        0 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/__init__.py
--rw-r--r--   0        0        0        0 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/admin_utils/__init__.py
--rw-r--r--   0        0        0        0 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/admin_utils/management/__init__.py
--rw-r--r--   0        0        0        0 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/admin_utils/management/commands/__init__.py
--rw-r--r--   0        0        0     2619 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/admin_utils/management/commands/clean.py
--rw-r--r--   0        0        0     2820 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/admin_utils/management/commands/enable_autocomplete.py
--rw-r--r--   0        0        0      471 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/admin_utils/management/commands/keystone_autocomplete
--rw-r--r--   0        0        0     3479 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/admin_utils/management/commands/quickstart.py
--rw-r--r--   0        0        0        0 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/admin_utils/tests/__init__.py
--rw-r--r--   0        0        0      625 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/admin_utils/tests/test_managment.py
--rw-r--r--   0        0        0        0 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/allocations/__init__.py
--rw-r--r--   0        0        0     4543 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/allocations/admin.py
--rw-r--r--   0        0        0     2173 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/allocations/managers.py
--rw-r--r--   0        0        0     3420 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/allocations/migrations/0001_initial.py
--rw-r--r--   0        0        0     1298 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/allocations/migrations/0002_initial.py
--rw-r--r--   0        0        0     1063 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/allocations/migrations/0003_remove_allocationrequest_approved_and_more.py
--rw-r--r--   0        0        0        0 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/allocations/migrations/__init__.py
--rw-r--r--   0        0        0     4837 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/allocations/models.py
--rw-r--r--   0        0        0     3347 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/allocations/permissions.py
--rw-r--r--   0        0        0     1917 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/allocations/serializers.py
--rw-r--r--   0        0        0     4324 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/allocations/tasks.py
--rw-r--r--   0        0        0      516 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/allocations/urls.py
--rw-r--r--   0        0        0     3246 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/allocations/views.py
--rw-r--r--   0        0        0        0 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/authentication/__init__.py
--rw-r--r--   0        0        0      572 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/authentication/tasks.py
--rw-r--r--   0        0        0      444 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/authentication/urls.py
--rw-r--r--   0        0        0        0 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/docs/__init__.py
--rw-r--r--   0        0        0      337 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/docs/urls.py
--rw-r--r--   0        0        0        0 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/health/__init__.py
--rw-r--r--   0        0        0        0 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/health/tests/__init__.py
--rw-r--r--   0        0        0     3199 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/health/tests/test_views.py
--rw-r--r--   0        0        0      244 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/health/urls.py
--rw-r--r--   0        0        0     2066 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/health/views.py
--rw-r--r--   0        0        0        0 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/logging/__init__.py
--rw-r--r--   0        0        0     1344 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/logging/handlers.py
--rw-r--r--   0        0        0     1759 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/logging/middleware.py
--rw-r--r--   0        0        0     1959 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/logging/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/logging/migrations/__init__.py
--rw-r--r--   0        0        0     1469 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/logging/models.py
--rw-r--r--   0        0        0      868 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/logging/serializers.py
--rw-r--r--   0        0        0      709 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/logging/tasks.py
--rw-r--r--   0        0        0      278 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/logging/urls.py
--rw-r--r--   0        0        0      949 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/logging/views.py
--rw-r--r--   0        0        0        0 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/research_products/__init__.py
--rw-r--r--   0        0        0     1518 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/research_products/admin.py
--rw-r--r--   0        0        0     1758 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/research_products/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/research_products/migrations/__init__.py
--rw-r--r--   0        0        0     1661 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/research_products/models.py
--rw-r--r--   0        0        0      868 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/research_products/serializers.py
--rw-r--r--   0        0        0      296 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/research_products/urls.py
--rw-r--r--   0        0        0      804 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/research_products/views.py
--rw-r--r--   0        0        0      141 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/scheduler/__init__.py
--rw-r--r--   0        0        0     1029 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/scheduler/admin.py
--rw-r--r--   0        0        0     1344 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/scheduler/celery.py
--rw-r--r--   0        0        0        0 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/users/__init__.py
--rw-r--r--   0        0        0     1307 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/users/admin.py
--rw-r--r--   0        0        0        0 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/users/management/__init__.py
--rw-r--r--   0        0        0        0 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/users/management/commands/__init__.py
--rw-r--r--   0        0        0     1056 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/users/management/commands/ldap_update.py
--rw-r--r--   0        0        0     3134 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/users/managers.py
--rw-r--r--   0        0        0     3018 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/users/migrations/0001_initial.py
--rw-r--r--   0        0        0      405 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/users/migrations/0002_user_is_ldap_user.py
--rw-r--r--   0        0        0        0 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/users/migrations/__init__.py
--rw-r--r--   0        0        0     2370 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/users/models.py
--rw-r--r--   0        0        0      913 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/users/permissions.py
--rw-r--r--   0        0        0      887 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/users/serializers.py
--rw-r--r--   0        0        0     2095 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/users/tasks.py
--rw-r--r--   0        0        0        0 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/users/tests/__init__.py
--rw-r--r--   0        0        0        0 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/users/tests/test_managers/__init__.py
--rw-r--r--   0        0        0     1374 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/users/tests/test_managers/test_ResearchGroupManager.py
--rw-r--r--   0        0        0     2399 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/users/tests/test_managers/test_UserManager.py
--rw-r--r--   0        0        0        0 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/users/tests/test_models/__init__.py
--rw-r--r--   0        0        0     3210 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/users/tests/test_models/test_ResearchGroup.py
--rw-r--r--   0        0        0      471 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/users/tests/test_models/test_User.py
--rw-r--r--   0        0        0      748 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/users/tests/utils.py
--rw-r--r--   0        0        0      329 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/users/urls.py
--rw-r--r--   0        0        0     1329 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/apps/users/views.py
--rw-r--r--   0        0        0        0 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/main/__init__.py
--rw-r--r--   0        0        0      169 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/main/asgi.py
--rw-r--r--   0        0        0     7865 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/main/settings.py
--rw-r--r--   0        0        0     1002 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/main/urls.py
--rw-r--r--   0        0        0      168 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/main/wsgi.py
--rwxr-xr-x   0        0        0      556 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/manage.py
--rw-r--r--   0        0        0        0 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/plugins/__init__.py
--rw-r--r--   0        0        0     4728 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/plugins/slurm.py
--rw-r--r--   0        0        0        0 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/tests/__init__.py
--rw-r--r--   0        0        0        0 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/tests/allocations/__init__.py
--rw-r--r--   0        0        0     2923 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/tests/allocations/test_allocations.py
--rw-r--r--   0        0        0     4229 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/tests/allocations/test_allocations_pk.py
--rw-r--r--   0        0        0     2929 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/tests/allocations/test_clusters.py
--rw-r--r--   0        0        0     3104 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/tests/allocations/test_clusters_pk.py
--rw-r--r--   0        0        0     5631 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/tests/allocations/test_requests.py
--rw-r--r--   0        0        0     5351 2024-04-08 17:43:08.837383 keystone_api-0.3.3/keystone_api/tests/allocations/test_requests_pk.py
--rw-r--r--   0        0        0     2898 2024-04-08 17:43:08.841384 keystone_api-0.3.3/keystone_api/tests/allocations/test_reviews.py
--rw-r--r--   0        0        0     4202 2024-04-08 17:43:08.841384 keystone_api-0.3.3/keystone_api/tests/allocations/test_reviews_pk.py
--rw-r--r--   0        0        0     3015 2024-04-08 17:43:08.841384 keystone_api-0.3.3/keystone_api/tests/fixtures/multi_research_group.yaml
--rw-r--r--   0        0        0        0 2024-04-08 17:43:08.841384 keystone_api-0.3.3/keystone_api/tests/health/__init__.py
--rw-r--r--   0        0        0     3102 2024-04-08 17:43:08.841384 keystone_api-0.3.3/keystone_api/tests/health/test.py
--rw-r--r--   0        0        0        0 2024-04-08 17:43:08.841384 keystone_api-0.3.3/keystone_api/tests/logging/__init__.py
--rw-r--r--   0        0        0     2871 2024-04-08 17:43:08.841384 keystone_api-0.3.3/keystone_api/tests/logging/test_apps.py
--rw-r--r--   0        0        0     2879 2024-04-08 17:43:08.841384 keystone_api-0.3.3/keystone_api/tests/logging/test_requests.py
--rw-r--r--   0        0        0        0 2024-04-08 17:43:08.841384 keystone_api-0.3.3/keystone_api/tests/users/__init__.py
--rw-r--r--   0        0        0     2981 2024-04-08 17:43:08.841384 keystone_api-0.3.3/keystone_api/tests/users/test_researchgroups.py
--rw-r--r--   0        0        0     4244 2024-04-08 17:43:08.841384 keystone_api-0.3.3/keystone_api/tests/users/test_researchgroups_pk.py
--rw-r--r--   0        0        0     2964 2024-04-08 17:43:08.841384 keystone_api-0.3.3/keystone_api/tests/users/test_users.py
--rw-r--r--   0        0        0     4471 2024-04-08 17:43:08.841384 keystone_api-0.3.3/keystone_api/tests/users/test_users_pk.py
--rw-r--r--   0        0        0     2014 2024-04-08 17:43:08.841384 keystone_api-0.3.3/keystone_api/tests/utils.py
--rw-r--r--   0        0        0      957 2024-04-08 17:43:29.901483 keystone_api-0.3.3/pyproject.toml
--rw-r--r--   0        0        0    14773 1970-01-01 00:00:00.000000 keystone_api-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0    13578 2024-04-16 16:31:17.680683 keystone_api-0.3.4/README.md
+-rw-r--r--   0        0        0      428 2024-04-16 16:31:17.680683 keystone_api-0.3.4/keystone_api/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-16 16:31:17.680683 keystone_api-0.3.4/keystone_api/apps/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-16 16:31:17.680683 keystone_api-0.3.4/keystone_api/apps/admin_utils/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-16 16:31:17.680683 keystone_api-0.3.4/keystone_api/apps/admin_utils/management/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-16 16:31:17.680683 keystone_api-0.3.4/keystone_api/apps/admin_utils/management/commands/__init__.py
+-rw-r--r--   0        0        0     2619 2024-04-16 16:31:17.680683 keystone_api-0.3.4/keystone_api/apps/admin_utils/management/commands/clean.py
+-rw-r--r--   0        0        0     2820 2024-04-16 16:31:17.680683 keystone_api-0.3.4/keystone_api/apps/admin_utils/management/commands/enable_autocomplete.py
+-rw-r--r--   0        0        0      471 2024-04-16 16:31:17.680683 keystone_api-0.3.4/keystone_api/apps/admin_utils/management/commands/keystone_autocomplete
+-rw-r--r--   0        0        0     3618 2024-04-16 16:31:17.680683 keystone_api-0.3.4/keystone_api/apps/admin_utils/management/commands/quickstart.py
+-rw-r--r--   0        0        0        0 2024-04-16 16:31:17.680683 keystone_api-0.3.4/keystone_api/apps/admin_utils/tests/__init__.py
+-rw-r--r--   0        0        0      611 2024-04-16 16:31:17.680683 keystone_api-0.3.4/keystone_api/apps/admin_utils/tests/test_managment.py
+-rw-r--r--   0        0        0        0 2024-04-16 16:31:17.680683 keystone_api-0.3.4/keystone_api/apps/allocations/__init__.py
+-rw-r--r--   0        0        0     4543 2024-04-16 16:31:17.680683 keystone_api-0.3.4/keystone_api/apps/allocations/admin.py
+-rw-r--r--   0        0        0     2173 2024-04-16 16:31:17.680683 keystone_api-0.3.4/keystone_api/apps/allocations/managers.py
+-rw-r--r--   0        0        0     3420 2024-04-16 16:31:17.680683 keystone_api-0.3.4/keystone_api/apps/allocations/migrations/0001_initial.py
+-rw-r--r--   0        0        0     1298 2024-04-16 16:31:17.680683 keystone_api-0.3.4/keystone_api/apps/allocations/migrations/0002_initial.py
+-rw-r--r--   0        0        0     1063 2024-04-16 16:31:17.680683 keystone_api-0.3.4/keystone_api/apps/allocations/migrations/0003_remove_allocationrequest_approved_and_more.py
+-rw-r--r--   0        0        0        0 2024-04-16 16:31:17.680683 keystone_api-0.3.4/keystone_api/apps/allocations/migrations/__init__.py
+-rw-r--r--   0        0        0     4837 2024-04-16 16:31:17.680683 keystone_api-0.3.4/keystone_api/apps/allocations/models.py
+-rw-r--r--   0        0        0     3347 2024-04-16 16:31:17.680683 keystone_api-0.3.4/keystone_api/apps/allocations/permissions.py
+-rw-r--r--   0        0        0     1917 2024-04-16 16:31:17.680683 keystone_api-0.3.4/keystone_api/apps/allocations/serializers.py
+-rw-r--r--   0        0        0     4324 2024-04-16 16:31:17.680683 keystone_api-0.3.4/keystone_api/apps/allocations/tasks.py
+-rw-r--r--   0        0        0      516 2024-04-16 16:31:17.680683 keystone_api-0.3.4/keystone_api/apps/allocations/urls.py
+-rw-r--r--   0        0        0     3246 2024-04-16 16:31:17.680683 keystone_api-0.3.4/keystone_api/apps/allocations/views.py
+-rw-r--r--   0        0        0        0 2024-04-16 16:31:17.680683 keystone_api-0.3.4/keystone_api/apps/authentication/__init__.py
+-rw-r--r--   0        0        0      572 2024-04-16 16:31:17.680683 keystone_api-0.3.4/keystone_api/apps/authentication/tasks.py
+-rw-r--r--   0        0        0      444 2024-04-16 16:31:17.680683 keystone_api-0.3.4/keystone_api/apps/authentication/urls.py
+-rw-r--r--   0        0        0        0 2024-04-16 16:31:17.680683 keystone_api-0.3.4/keystone_api/apps/docs/__init__.py
+-rw-r--r--   0        0        0      337 2024-04-16 16:31:17.680683 keystone_api-0.3.4/keystone_api/apps/docs/urls.py
+-rw-r--r--   0        0        0        0 2024-04-16 16:31:17.680683 keystone_api-0.3.4/keystone_api/apps/health/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-16 16:31:17.680683 keystone_api-0.3.4/keystone_api/apps/health/tests/__init__.py
+-rw-r--r--   0        0        0     3199 2024-04-16 16:31:17.680683 keystone_api-0.3.4/keystone_api/apps/health/tests/test_views.py
+-rw-r--r--   0        0        0      244 2024-04-16 16:31:17.680683 keystone_api-0.3.4/keystone_api/apps/health/urls.py
+-rw-r--r--   0        0        0     2066 2024-04-16 16:31:17.680683 keystone_api-0.3.4/keystone_api/apps/health/views.py
+-rw-r--r--   0        0        0        0 2024-04-16 16:31:17.680683 keystone_api-0.3.4/keystone_api/apps/logging/__init__.py
+-rw-r--r--   0        0        0     1344 2024-04-16 16:31:17.680683 keystone_api-0.3.4/keystone_api/apps/logging/handlers.py
+-rw-r--r--   0        0        0     1759 2024-04-16 16:31:17.680683 keystone_api-0.3.4/keystone_api/apps/logging/middleware.py
+-rw-r--r--   0        0        0     1959 2024-04-16 16:31:17.680683 keystone_api-0.3.4/keystone_api/apps/logging/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2024-04-16 16:31:17.680683 keystone_api-0.3.4/keystone_api/apps/logging/migrations/__init__.py
+-rw-r--r--   0        0        0     1469 2024-04-16 16:31:17.680683 keystone_api-0.3.4/keystone_api/apps/logging/models.py
+-rw-r--r--   0        0        0      868 2024-04-16 16:31:17.680683 keystone_api-0.3.4/keystone_api/apps/logging/serializers.py
+-rw-r--r--   0        0        0      709 2024-04-16 16:31:17.680683 keystone_api-0.3.4/keystone_api/apps/logging/tasks.py
+-rw-r--r--   0        0        0      278 2024-04-16 16:31:17.680683 keystone_api-0.3.4/keystone_api/apps/logging/urls.py
+-rw-r--r--   0        0        0      949 2024-04-16 16:31:17.680683 keystone_api-0.3.4/keystone_api/apps/logging/views.py
+-rw-r--r--   0        0        0        0 2024-04-16 16:31:17.680683 keystone_api-0.3.4/keystone_api/apps/research_products/__init__.py
+-rw-r--r--   0        0        0     1518 2024-04-16 16:31:17.680683 keystone_api-0.3.4/keystone_api/apps/research_products/admin.py
+-rw-r--r--   0        0        0     1758 2024-04-16 16:31:17.680683 keystone_api-0.3.4/keystone_api/apps/research_products/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2024-04-16 16:31:17.680683 keystone_api-0.3.4/keystone_api/apps/research_products/migrations/__init__.py
+-rw-r--r--   0        0        0     1661 2024-04-16 16:31:17.680683 keystone_api-0.3.4/keystone_api/apps/research_products/models.py
+-rw-r--r--   0        0        0      868 2024-04-16 16:31:17.680683 keystone_api-0.3.4/keystone_api/apps/research_products/serializers.py
+-rw-r--r--   0        0        0      296 2024-04-16 16:31:17.680683 keystone_api-0.3.4/keystone_api/apps/research_products/urls.py
+-rw-r--r--   0        0        0      804 2024-04-16 16:31:17.680683 keystone_api-0.3.4/keystone_api/apps/research_products/views.py
+-rw-r--r--   0        0        0      141 2024-04-16 16:31:17.684683 keystone_api-0.3.4/keystone_api/apps/scheduler/__init__.py
+-rw-r--r--   0        0        0     1029 2024-04-16 16:31:17.684683 keystone_api-0.3.4/keystone_api/apps/scheduler/admin.py
+-rw-r--r--   0        0        0     1344 2024-04-16 16:31:17.684683 keystone_api-0.3.4/keystone_api/apps/scheduler/celery.py
+-rw-r--r--   0        0        0        0 2024-04-16 16:31:17.684683 keystone_api-0.3.4/keystone_api/apps/users/__init__.py
+-rw-r--r--   0        0        0     1307 2024-04-16 16:31:17.684683 keystone_api-0.3.4/keystone_api/apps/users/admin.py
+-rw-r--r--   0        0        0        0 2024-04-16 16:31:17.684683 keystone_api-0.3.4/keystone_api/apps/users/management/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-16 16:31:17.684683 keystone_api-0.3.4/keystone_api/apps/users/management/commands/__init__.py
+-rw-r--r--   0        0        0     1056 2024-04-16 16:31:17.684683 keystone_api-0.3.4/keystone_api/apps/users/management/commands/ldap_update.py
+-rw-r--r--   0        0        0     3134 2024-04-16 16:31:17.684683 keystone_api-0.3.4/keystone_api/apps/users/managers.py
+-rw-r--r--   0        0        0     3018 2024-04-16 16:31:17.684683 keystone_api-0.3.4/keystone_api/apps/users/migrations/0001_initial.py
+-rw-r--r--   0        0        0      405 2024-04-16 16:31:17.684683 keystone_api-0.3.4/keystone_api/apps/users/migrations/0002_user_is_ldap_user.py
+-rw-r--r--   0        0        0        0 2024-04-16 16:31:17.684683 keystone_api-0.3.4/keystone_api/apps/users/migrations/__init__.py
+-rw-r--r--   0        0        0     2370 2024-04-16 16:31:17.684683 keystone_api-0.3.4/keystone_api/apps/users/models.py
+-rw-r--r--   0        0        0      913 2024-04-16 16:31:17.684683 keystone_api-0.3.4/keystone_api/apps/users/permissions.py
+-rw-r--r--   0        0        0      887 2024-04-16 16:31:17.684683 keystone_api-0.3.4/keystone_api/apps/users/serializers.py
+-rw-r--r--   0        0        0     2095 2024-04-16 16:31:17.684683 keystone_api-0.3.4/keystone_api/apps/users/tasks.py
+-rw-r--r--   0        0        0        0 2024-04-16 16:31:17.684683 keystone_api-0.3.4/keystone_api/apps/users/tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-16 16:31:17.684683 keystone_api-0.3.4/keystone_api/apps/users/tests/test_managers/__init__.py
+-rw-r--r--   0        0        0     1374 2024-04-16 16:31:17.684683 keystone_api-0.3.4/keystone_api/apps/users/tests/test_managers/test_ResearchGroupManager.py
+-rw-r--r--   0        0        0     2399 2024-04-16 16:31:17.684683 keystone_api-0.3.4/keystone_api/apps/users/tests/test_managers/test_UserManager.py
+-rw-r--r--   0        0        0        0 2024-04-16 16:31:17.684683 keystone_api-0.3.4/keystone_api/apps/users/tests/test_models/__init__.py
+-rw-r--r--   0        0        0     3210 2024-04-16 16:31:17.684683 keystone_api-0.3.4/keystone_api/apps/users/tests/test_models/test_ResearchGroup.py
+-rw-r--r--   0        0        0      471 2024-04-16 16:31:17.684683 keystone_api-0.3.4/keystone_api/apps/users/tests/test_models/test_User.py
+-rw-r--r--   0        0        0      748 2024-04-16 16:31:17.684683 keystone_api-0.3.4/keystone_api/apps/users/tests/utils.py
+-rw-r--r--   0        0        0      329 2024-04-16 16:31:17.684683 keystone_api-0.3.4/keystone_api/apps/users/urls.py
+-rw-r--r--   0        0        0     1329 2024-04-16 16:31:17.684683 keystone_api-0.3.4/keystone_api/apps/users/views.py
+-rw-r--r--   0        0        0        0 2024-04-16 16:31:17.684683 keystone_api-0.3.4/keystone_api/main/__init__.py
+-rw-r--r--   0        0        0      169 2024-04-16 16:31:17.684683 keystone_api-0.3.4/keystone_api/main/asgi.py
+-rw-r--r--   0        0        0     7865 2024-04-16 16:31:17.684683 keystone_api-0.3.4/keystone_api/main/settings.py
+-rw-r--r--   0        0        0     1002 2024-04-16 16:31:17.684683 keystone_api-0.3.4/keystone_api/main/urls.py
+-rw-r--r--   0        0        0      168 2024-04-16 16:31:17.684683 keystone_api-0.3.4/keystone_api/main/wsgi.py
+-rwxr-xr-x   0        0        0      556 2024-04-16 16:31:17.684683 keystone_api-0.3.4/keystone_api/manage.py
+-rw-r--r--   0        0        0        0 2024-04-16 16:31:17.684683 keystone_api-0.3.4/keystone_api/plugins/__init__.py
+-rw-r--r--   0        0        0     4728 2024-04-16 16:31:17.684683 keystone_api-0.3.4/keystone_api/plugins/slurm.py
+-rw-r--r--   0        0        0        0 2024-04-16 16:31:17.684683 keystone_api-0.3.4/keystone_api/tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-16 16:31:17.684683 keystone_api-0.3.4/keystone_api/tests/allocations/__init__.py
+-rw-r--r--   0        0        0     2923 2024-04-16 16:31:17.684683 keystone_api-0.3.4/keystone_api/tests/allocations/test_allocations.py
+-rw-r--r--   0        0        0     4229 2024-04-16 16:31:17.684683 keystone_api-0.3.4/keystone_api/tests/allocations/test_allocations_pk.py
+-rw-r--r--   0        0        0     2929 2024-04-16 16:31:17.684683 keystone_api-0.3.4/keystone_api/tests/allocations/test_clusters.py
+-rw-r--r--   0        0        0     3104 2024-04-16 16:31:17.684683 keystone_api-0.3.4/keystone_api/tests/allocations/test_clusters_pk.py
+-rw-r--r--   0        0        0     5631 2024-04-16 16:31:17.684683 keystone_api-0.3.4/keystone_api/tests/allocations/test_requests.py
+-rw-r--r--   0        0        0     5351 2024-04-16 16:31:17.684683 keystone_api-0.3.4/keystone_api/tests/allocations/test_requests_pk.py
+-rw-r--r--   0        0        0     2898 2024-04-16 16:31:17.684683 keystone_api-0.3.4/keystone_api/tests/allocations/test_reviews.py
+-rw-r--r--   0        0        0     4202 2024-04-16 16:31:17.684683 keystone_api-0.3.4/keystone_api/tests/allocations/test_reviews_pk.py
+-rw-r--r--   0        0        0     3015 2024-04-16 16:31:17.684683 keystone_api-0.3.4/keystone_api/tests/fixtures/multi_research_group.yaml
+-rw-r--r--   0        0        0        0 2024-04-16 16:31:17.684683 keystone_api-0.3.4/keystone_api/tests/health/__init__.py
+-rw-r--r--   0        0        0     3102 2024-04-16 16:31:17.684683 keystone_api-0.3.4/keystone_api/tests/health/test.py
+-rw-r--r--   0        0        0        0 2024-04-16 16:31:17.684683 keystone_api-0.3.4/keystone_api/tests/logging/__init__.py
+-rw-r--r--   0        0        0     2871 2024-04-16 16:31:17.684683 keystone_api-0.3.4/keystone_api/tests/logging/test_apps.py
+-rw-r--r--   0        0        0     2879 2024-04-16 16:31:17.684683 keystone_api-0.3.4/keystone_api/tests/logging/test_requests.py
+-rw-r--r--   0        0        0        0 2024-04-16 16:31:17.684683 keystone_api-0.3.4/keystone_api/tests/users/__init__.py
+-rw-r--r--   0        0        0     2981 2024-04-16 16:31:17.684683 keystone_api-0.3.4/keystone_api/tests/users/test_researchgroups.py
+-rw-r--r--   0        0        0     4244 2024-04-16 16:31:17.684683 keystone_api-0.3.4/keystone_api/tests/users/test_researchgroups_pk.py
+-rw-r--r--   0        0        0     2964 2024-04-16 16:31:17.684683 keystone_api-0.3.4/keystone_api/tests/users/test_users.py
+-rw-r--r--   0        0        0     4471 2024-04-16 16:31:17.684683 keystone_api-0.3.4/keystone_api/tests/users/test_users_pk.py
+-rw-r--r--   0        0        0     2014 2024-04-16 16:31:17.684683 keystone_api-0.3.4/keystone_api/tests/utils.py
+-rw-r--r--   0        0        0      957 2024-04-16 16:31:32.536737 keystone_api-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0    14773 1970-01-01 00:00:00.000000 keystone_api-0.3.4/PKG-INFO
```

### Comparing `keystone_api-0.3.3/README.md` & `keystone_api-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.3/keystone_api/apps/admin_utils/management/commands/clean.py` & `keystone_api-0.3.4/keystone_api/apps/admin_utils/management/commands/clean.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.3/keystone_api/apps/admin_utils/management/commands/enable_autocomplete.py` & `keystone_api-0.3.4/keystone_api/apps/admin_utils/management/commands/enable_autocomplete.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.3/keystone_api/apps/admin_utils/management/commands/quickstart.py` & `keystone_api-0.3.4/keystone_api/apps/admin_utils/management/commands/quickstart.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 | Argument   | Description                                                      |
 |------------|------------------------------------------------------------------|
 | --static   | Collect static files                                             |
 | --migrate  | Run database migrations                                          |
 | --celery   | Launch a Celery worker with a Redis backend                      |
 | --gunicorn | Run a web server using Gunicorn                                  |
-| --no-input | Do not prompt for user input of any kind                         |
+| --all      | Launch all available services                                    |
 """
 
 import subprocess
 from argparse import ArgumentParser
 
 from django.core.management import call_command
 from django.core.management.base import BaseCommand
@@ -35,47 +35,50 @@
         """
 
         group = parser.add_argument_group('quickstart options')
         group.add_argument('--static', action='store_true', help='Collect static files.')
         group.add_argument('--migrate', action='store_true', help='Run database migrations.')
         group.add_argument('--celery', action='store_true', help='Launch a background Celery worker.')
         group.add_argument('--gunicorn', action='store_true', help='Run a web server using Gunicorn.')
-        group.add_argument('--no-input', action='store_false', help='Do not prompt for user input of any kind.')
+        group.add_argument('--all', action='store_true', help='Launch all available services.')
 
     def handle(self, *args, **options) -> None:
         """Handle the command execution
 
         Args:
           *args: Additional positional arguments
           **options: Additional keyword arguments
         """
 
-        if options['migrate']:
+        # Note: `no_input=False` indicates the user should not be prompted for input
+
+        if options['migrate'] or options['all']:
             self.stdout.write(self.style.SUCCESS('Running database migrations...'))
-            call_command('migrate', no_input=options['no_input'])
+            call_command('migrate', no_input=False)
 
-        if options['static']:
+        if options['static'] or options['all']:
             self.stdout.write(self.style.SUCCESS('Collecting static files...'))
-            call_command('collectstatic', no_input=options['no_input'])
+            call_command('collectstatic', no_input=False)
 
-        if options['celery']:
+        if options['celery'] or options['all']:
             self.stdout.write(self.style.SUCCESS('Starting Celery worker...'))
             self.run_celery()
 
-        if options['gunicorn']:
+        if options['gunicorn'] or options['all']:
             self.stdout.write(self.style.SUCCESS('Starting Gunicorn server...'))
             self.run_gunicorn()
 
     @staticmethod
     def run_celery() -> None:
         """Start a Celery worker"""
 
         subprocess.Popen(['redis-server'])
-        subprocess.Popen(['celery', '-A', 'keystone_api.apps.scheduler', 'beat', '--scheduler', 'django_celery_beat.schedulers:DatabaseScheduler'])
         subprocess.Popen(['celery', '-A', 'keystone_api.apps.scheduler', 'worker'])
+        subprocess.Popen(['celery', '-A', 'keystone_api.apps.scheduler', 'beat',
+                          '--scheduler', 'django_celery_beat.schedulers:DatabaseScheduler'])
 
     @staticmethod
     def run_gunicorn(host: str = '0.0.0.0', port: int = 8000) -> None:
         """Start a Gunicorn server
 
         Args:
           host: The host to bind to
```

### Comparing `keystone_api-0.3.3/keystone_api/apps/admin_utils/tests/test_managment.py` & `keystone_api-0.3.4/keystone_api/apps/admin_utils/tests/test_managment.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,10 +9,10 @@
 class Quickstart(TestCase):
     """Tests for the `quickstart` CLI utility"""
 
     def test_gunicorn_command(self) -> None:
         """Test the `--gunicorn` flag executes a gunicorn server command"""
 
         with patch('subprocess.run') as mock_run:
-            call_command('quickstart', '--gunicorn', '--no-input')
+            call_command('quickstart', '--gunicorn')
             mock_run.assert_called_with(
                 ['gunicorn', '--bind', '0.0.0.0:8000', 'keystone_api.main.wsgi:application'], check=True)
```

### Comparing `keystone_api-0.3.3/keystone_api/apps/allocations/admin.py` & `keystone_api-0.3.4/keystone_api/apps/allocations/admin.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.3/keystone_api/apps/allocations/managers.py` & `keystone_api-0.3.4/keystone_api/apps/allocations/managers.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.3/keystone_api/apps/allocations/migrations/0001_initial.py` & `keystone_api-0.3.4/keystone_api/apps/allocations/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.3/keystone_api/apps/allocations/migrations/0002_initial.py` & `keystone_api-0.3.4/keystone_api/apps/allocations/migrations/0002_initial.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.3/keystone_api/apps/allocations/migrations/0003_remove_allocationrequest_approved_and_more.py` & `keystone_api-0.3.4/keystone_api/apps/allocations/migrations/0003_remove_allocationrequest_approved_and_more.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.3/keystone_api/apps/allocations/models.py` & `keystone_api-0.3.4/keystone_api/apps/allocations/models.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.3/keystone_api/apps/allocations/permissions.py` & `keystone_api-0.3.4/keystone_api/apps/allocations/permissions.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.3/keystone_api/apps/allocations/serializers.py` & `keystone_api-0.3.4/keystone_api/apps/allocations/serializers.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.3/keystone_api/apps/allocations/tasks.py` & `keystone_api-0.3.4/keystone_api/apps/allocations/tasks.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.3/keystone_api/apps/allocations/urls.py` & `keystone_api-0.3.4/keystone_api/apps/allocations/urls.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.3/keystone_api/apps/allocations/views.py` & `keystone_api-0.3.4/keystone_api/apps/allocations/views.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.3/keystone_api/apps/authentication/tasks.py` & `keystone_api-0.3.4/keystone_api/apps/authentication/tasks.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.3/keystone_api/apps/health/tests/test_views.py` & `keystone_api-0.3.4/keystone_api/apps/health/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.3/keystone_api/apps/health/views.py` & `keystone_api-0.3.4/keystone_api/apps/health/views.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.3/keystone_api/apps/logging/handlers.py` & `keystone_api-0.3.4/keystone_api/apps/logging/handlers.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.3/keystone_api/apps/logging/middleware.py` & `keystone_api-0.3.4/keystone_api/apps/logging/middleware.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.3/keystone_api/apps/logging/migrations/0001_initial.py` & `keystone_api-0.3.4/keystone_api/apps/logging/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.3/keystone_api/apps/logging/models.py` & `keystone_api-0.3.4/keystone_api/apps/logging/models.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.3/keystone_api/apps/logging/serializers.py` & `keystone_api-0.3.4/keystone_api/apps/logging/serializers.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.3/keystone_api/apps/logging/tasks.py` & `keystone_api-0.3.4/keystone_api/apps/logging/tasks.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.3/keystone_api/apps/logging/views.py` & `keystone_api-0.3.4/keystone_api/apps/logging/views.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.3/keystone_api/apps/research_products/admin.py` & `keystone_api-0.3.4/keystone_api/apps/research_products/admin.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.3/keystone_api/apps/research_products/migrations/0001_initial.py` & `keystone_api-0.3.4/keystone_api/apps/research_products/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.3/keystone_api/apps/research_products/models.py` & `keystone_api-0.3.4/keystone_api/apps/research_products/models.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.3/keystone_api/apps/research_products/serializers.py` & `keystone_api-0.3.4/keystone_api/apps/research_products/serializers.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.3/keystone_api/apps/research_products/views.py` & `keystone_api-0.3.4/keystone_api/apps/research_products/views.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.3/keystone_api/apps/scheduler/admin.py` & `keystone_api-0.3.4/keystone_api/apps/scheduler/admin.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.3/keystone_api/apps/scheduler/celery.py` & `keystone_api-0.3.4/keystone_api/apps/scheduler/celery.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.3/keystone_api/apps/users/admin.py` & `keystone_api-0.3.4/keystone_api/apps/users/admin.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.3/keystone_api/apps/users/management/commands/ldap_update.py` & `keystone_api-0.3.4/keystone_api/apps/users/management/commands/ldap_update.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.3/keystone_api/apps/users/managers.py` & `keystone_api-0.3.4/keystone_api/apps/users/managers.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.3/keystone_api/apps/users/migrations/0001_initial.py` & `keystone_api-0.3.4/keystone_api/apps/users/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.3/keystone_api/apps/users/models.py` & `keystone_api-0.3.4/keystone_api/apps/users/models.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.3/keystone_api/apps/users/permissions.py` & `keystone_api-0.3.4/keystone_api/apps/users/permissions.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.3/keystone_api/apps/users/serializers.py` & `keystone_api-0.3.4/keystone_api/apps/users/serializers.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.3/keystone_api/apps/users/tasks.py` & `keystone_api-0.3.4/keystone_api/apps/users/tasks.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.3/keystone_api/apps/users/tests/test_managers/test_ResearchGroupManager.py` & `keystone_api-0.3.4/keystone_api/apps/users/tests/test_managers/test_ResearchGroupManager.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.3/keystone_api/apps/users/tests/test_managers/test_UserManager.py` & `keystone_api-0.3.4/keystone_api/apps/users/tests/test_managers/test_UserManager.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.3/keystone_api/apps/users/tests/test_models/test_ResearchGroup.py` & `keystone_api-0.3.4/keystone_api/apps/users/tests/test_models/test_ResearchGroup.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.3/keystone_api/apps/users/tests/utils.py` & `keystone_api-0.3.4/keystone_api/apps/users/tests/utils.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.3/keystone_api/apps/users/views.py` & `keystone_api-0.3.4/keystone_api/apps/users/views.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.3/keystone_api/main/settings.py` & `keystone_api-0.3.4/keystone_api/main/settings.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.3/keystone_api/main/urls.py` & `keystone_api-0.3.4/keystone_api/main/urls.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.3/keystone_api/manage.py` & `keystone_api-0.3.4/keystone_api/manage.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.3/keystone_api/plugins/slurm.py` & `keystone_api-0.3.4/keystone_api/plugins/slurm.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.3/keystone_api/tests/allocations/test_allocations.py` & `keystone_api-0.3.4/keystone_api/tests/allocations/test_allocations.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.3/keystone_api/tests/allocations/test_allocations_pk.py` & `keystone_api-0.3.4/keystone_api/tests/allocations/test_allocations_pk.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.3/keystone_api/tests/allocations/test_clusters.py` & `keystone_api-0.3.4/keystone_api/tests/allocations/test_clusters.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.3/keystone_api/tests/allocations/test_clusters_pk.py` & `keystone_api-0.3.4/keystone_api/tests/allocations/test_clusters_pk.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.3/keystone_api/tests/allocations/test_requests.py` & `keystone_api-0.3.4/keystone_api/tests/allocations/test_requests.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.3/keystone_api/tests/allocations/test_requests_pk.py` & `keystone_api-0.3.4/keystone_api/tests/allocations/test_requests_pk.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.3/keystone_api/tests/allocations/test_reviews.py` & `keystone_api-0.3.4/keystone_api/tests/allocations/test_reviews.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.3/keystone_api/tests/allocations/test_reviews_pk.py` & `keystone_api-0.3.4/keystone_api/tests/allocations/test_reviews_pk.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.3/keystone_api/tests/fixtures/multi_research_group.yaml` & `keystone_api-0.3.4/keystone_api/tests/fixtures/multi_research_group.yaml`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.3/keystone_api/tests/health/test.py` & `keystone_api-0.3.4/keystone_api/tests/health/test.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.3/keystone_api/tests/logging/test_apps.py` & `keystone_api-0.3.4/keystone_api/tests/logging/test_apps.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.3/keystone_api/tests/logging/test_requests.py` & `keystone_api-0.3.4/keystone_api/tests/logging/test_requests.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.3/keystone_api/tests/users/test_researchgroups.py` & `keystone_api-0.3.4/keystone_api/tests/users/test_researchgroups.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.3/keystone_api/tests/users/test_researchgroups_pk.py` & `keystone_api-0.3.4/keystone_api/tests/users/test_researchgroups_pk.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.3/keystone_api/tests/users/test_users.py` & `keystone_api-0.3.4/keystone_api/tests/users/test_users.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.3/keystone_api/tests/users/test_users_pk.py` & `keystone_api-0.3.4/keystone_api/tests/users/test_users_pk.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.3/keystone_api/tests/utils.py` & `keystone_api-0.3.4/keystone_api/tests/utils.py`

 * *Files identical despite different names*

### Comparing `keystone_api-0.3.3/pyproject.toml` & `keystone_api-0.3.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "keystone-api"
-version = "0.3.3"
+version = "0.3.4"
 readme = "README.md"
 description = "A REST API for managing user resource allocations on HPC systems."
 authors = ["Pitt Center for Research Computing"]
 keywords = ["Pitt", "CRC", "HPC", "django"]
 
 [tool.poetry.scripts]
 keystone-api = "keystone_api.manage:main"
```

### Comparing `keystone_api-0.3.3/PKG-INFO` & `keystone_api-0.3.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keystone-api
-Version: 0.3.3
+Version: 0.3.4
 Summary: A REST API for managing user resource allocations on HPC systems.
 Keywords: Pitt,CRC,HPC,django
 Author: Pitt Center for Research Computing
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

