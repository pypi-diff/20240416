# Comparing `tmp/certego_saas-0.7.8.tar.gz` & `tmp/certego_saas-0.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "certego_saas-0.7.8.tar", last modified: Thu Nov 30 15:14:37 2023, max compression
+gzip compressed data, was "certego_saas-0.7.9.tar", last modified: Tue Apr 16 07:47:14 2024, max compression
```

## Comparing `certego_saas-0.7.8.tar` & `certego_saas-0.7.9.tar`

### file list

```diff
@@ -1,181 +1,181 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 15:14:37.629697 certego_saas-0.7.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-11-30 15:14:27.000000 certego_saas-0.7.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      157 2023-11-30 15:14:27.000000 certego_saas-0.7.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4303 2023-11-30 15:14:37.629697 certego_saas-0.7.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1426 2023-11-30 15:14:27.000000 certego_saas-0.7.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 15:14:37.609697 certego_saas-0.7.8/certego_saas/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-30 15:14:27.000000 certego_saas-0.7.8/certego_saas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 15:14:37.609697 certego_saas-0.7.8/certego_saas/apps/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-30 15:14:27.000000 certego_saas-0.7.8/certego_saas/apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 15:14:37.609697 certego_saas-0.7.8/certego_saas/apps/auth/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-30 15:14:27.000000 certego_saas-0.7.8/certego_saas/apps/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      140 2023-11-30 15:14:27.000000 certego_saas-0.7.8/certego_saas/apps/auth/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2023-11-30 15:14:27.000000 certego_saas-0.7.8/certego_saas/apps/auth/backend.py
--rw-r--r--   0 runner    (1001) docker     (127)      211 2023-11-30 15:14:27.000000 certego_saas-0.7.8/certego_saas/apps/auth/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     2222 2023-11-30 15:14:27.000000 certego_saas-0.7.8/certego_saas/apps/auth/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 15:14:37.609697 certego_saas-0.7.8/certego_saas/apps/feedback/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-30 15:14:27.000000 certego_saas-0.7.8/certego_saas/apps/feedback/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      224 2023-11-30 15:14:27.000000 certego_saas-0.7.8/certego_saas/apps/feedback/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      152 2023-11-30 15:14:27.000000 certego_saas-0.7.8/certego_saas/apps/feedback/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 15:14:37.609697 certego_saas-0.7.8/certego_saas/apps/feedback/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     2093 2023-11-30 15:14:27.000000 certego_saas-0.7.8/certego_saas/apps/feedback/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-30 15:14:27.000000 certego_saas-0.7.8/certego_saas/apps/feedback/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1402 2023-11-30 15:14:27.000000 certego_saas-0.7.8/certego_saas/apps/feedback/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      906 2023-11-30 15:14:27.000000 certego_saas-0.7.8/certego_saas/apps/feedback/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)      314 2023-11-30 15:14:27.000000 certego_saas-0.7.8/certego_saas/apps/feedback/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)      620 2023-11-30 15:14:27.000000 certego_saas-0.7.8/certego_saas/apps/feedback/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 15:14:37.613697 certego_saas-0.7.8/certego_saas/apps/notifications/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-30 15:14:27.000000 certego_saas-0.7.8/certego_saas/apps/notifications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      353 2023-11-30 15:14:27.000000 certego_saas-0.7.8/certego_saas/apps/notifications/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      167 2023-11-30 15:14:27.000000 certego_saas-0.7.8/certego_saas/apps/notifications/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)      800 2023-11-30 15:14:27.000000 certego_saas-0.7.8/certego_saas/apps/notifications/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 15:14:37.613697 certego_saas-0.7.8/certego_saas/apps/notifications/management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-30 15:14:27.000000 certego_saas-0.7.8/certego_saas/apps/notifications/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 15:14:37.613697 certego_saas-0.7.8/certego_saas/apps/notifications/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-30 15:14:27.000000 certego_saas-0.7.8/certego_saas/apps/notifications/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3949 2023-11-30 15:14:27.000000 certego_saas-0.7.8/certego_saas/apps/notifications/management/commands/changelog_notification.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 15:14:37.613697 certego_saas-0.7.8/certego_saas/apps/notifications/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     1786 2023-11-30 15:14:27.000000 certego_saas-0.7.8/certego_saas/apps/notifications/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)      715 2023-11-30 15:14:27.000000 certego_saas-0.7.8/certego_saas/apps/notifications/migrations/0002_alter_notification_appname.py
--rw-r--r--   0 runner    (1001) docker     (127)      684 2023-11-30 15:14:27.000000 certego_saas-0.7.8/certego_saas/apps/notifications/migrations/0003_for_user.py
--rw-r--r--   0 runner    (1001) docker     (127)      696 2023-11-30 15:14:27.000000 certego_saas-0.7.8/certego_saas/apps/notifications/migrations/0004_for_user_blank.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-30 15:14:27.000000 certego_saas-0.7.8/certego_saas/apps/notifications/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2023-11-30 15:14:27.000000 certego_saas-0.7.8/certego_saas/apps/notifications/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      731 2023-11-30 15:14:27.000000 certego_saas-0.7.8/certego_saas/apps/notifications/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)      391 2023-11-30 15:14:27.000000 certego_saas-0.7.8/certego_saas/apps/notifications/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     2640 2023-11-30 15:14:27.000000 certego_saas-0.7.8/certego_saas/apps/notifications/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 15:14:37.613697 certego_saas-0.7.8/certego_saas/apps/organization/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-30 15:14:27.000000 certego_saas-0.7.8/certego_saas/apps/organization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      824 2023-11-30 15:14:27.000000 certego_saas-0.7.8/certego_saas/apps/organization/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      164 2023-11-30 15:14:27.000000 certego_saas-0.7.8/certego_saas/apps/organization/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     4735 2023-11-30 15:14:27.000000 certego_saas-0.7.8/certego_saas/apps/organization/invitation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1760 2023-11-30 15:14:27.000000 certego_saas-0.7.8/certego_saas/apps/organization/membership.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 15:14:37.613697 certego_saas-0.7.8/certego_saas/apps/organization/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     4125 2023-11-30 15:14:27.000000 certego_saas-0.7.8/certego_saas/apps/organization/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)      350 2023-11-30 15:14:27.000000 certego_saas-0.7.8/certego_saas/apps/organization/migrations/0002_membership_is_admin.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-30 15:14:27.000000 certego_saas-0.7.8/certego_saas/apps/organization/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1663 2023-11-30 15:14:27.000000 certego_saas-0.7.8/certego_saas/apps/organization/mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)      195 2023-11-30 15:14:27.000000 certego_saas-0.7.8/certego_saas/apps/organization/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     3424 2023-11-30 15:14:27.000000 certego_saas-0.7.8/certego_saas/apps/organization/organization.py
--rw-r--r--   0 runner    (1001) docker     (127)     2846 2023-11-30 15:14:27.000000 certego_saas-0.7.8/certego_saas/apps/organization/permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4415 2023-11-30 15:14:27.000000 certego_saas-0.7.8/certego_saas/apps/organization/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)      495 2023-11-30 15:14:27.000000 certego_saas-0.7.8/certego_saas/apps/organization/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     9689 2023-11-30 15:14:27.000000 certego_saas-0.7.8/certego_saas/apps/organization/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 15:14:37.617697 certego_saas-0.7.8/certego_saas/apps/payments/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-30 15:14:27.000000 certego_saas-0.7.8/certego_saas/apps/payments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      614 2023-11-30 15:14:27.000000 certego_saas-0.7.8/certego_saas/apps/payments/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      152 2023-11-30 15:14:27.000000 certego_saas-0.7.8/certego_saas/apps/payments/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)      555 2023-11-30 15:14:27.000000 certego_saas-0.7.8/certego_saas/apps/payments/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2023-11-30 15:14:27.000000 certego_saas-0.7.8/certego_saas/apps/payments/consts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2023-11-30 15:14:27.000000 certego_saas-0.7.8/certego_saas/apps/payments/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 15:14:37.617697 certego_saas-0.7.8/certego_saas/apps/payments/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     1989 2023-11-30 15:14:27.000000 certego_saas-0.7.8/certego_saas/apps/payments/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-30 15:14:27.000000 certego_saas-0.7.8/certego_saas/apps/payments/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10336 2023-11-30 15:14:27.000000 certego_saas-0.7.8/certego_saas/apps/payments/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      850 2023-11-30 15:14:27.000000 certego_saas-0.7.8/certego_saas/apps/payments/permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2747 2023-11-30 15:14:27.000000 certego_saas-0.7.8/certego_saas/apps/payments/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2023-11-30 15:14:27.000000 certego_saas-0.7.8/certego_saas/apps/payments/throttling.py
--rw-r--r--   0 runner    (1001) docker     (127)     2353 2023-11-30 15:14:27.000000 certego_saas-0.7.8/certego_saas/apps/payments/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 15:14:37.617697 certego_saas-0.7.8/certego_saas/apps/user/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-30 15:14:27.000000 certego_saas-0.7.8/certego_saas/apps/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2023-11-30 15:14:27.000000 certego_saas-0.7.8/certego_saas/apps/user/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      140 2023-11-30 15:14:27.000000 certego_saas-0.7.8/certego_saas/apps/user/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)      703 2023-11-30 15:14:27.000000 certego_saas-0.7.8/certego_saas/apps/user/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 15:14:37.617697 certego_saas-0.7.8/certego_saas/apps/user/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     5021 2023-11-30 15:14:27.000000 certego_saas-0.7.8/certego_saas/apps/user/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)     1984 2023-11-30 15:14:27.000000 certego_saas-0.7.8/certego_saas/apps/user/migrations/0002_migration.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-30 15:14:27.000000 certego_saas-0.7.8/certego_saas/apps/user/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4817 2023-11-30 15:14:27.000000 certego_saas-0.7.8/certego_saas/apps/user/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1031 2023-11-30 15:14:27.000000 certego_saas-0.7.8/certego_saas/apps/user/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)      183 2023-11-30 15:14:27.000000 certego_saas-0.7.8/certego_saas/apps/user/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2023-11-30 15:14:27.000000 certego_saas-0.7.8/certego_saas/apps/user/views.py
--rw-r--r--   0 runner    (1001) docker     (127)      138 2023-11-30 15:14:27.000000 certego_saas-0.7.8/certego_saas/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 15:14:37.621697 certego_saas-0.7.8/certego_saas/ext/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-30 15:14:27.000000 certego_saas-0.7.8/certego_saas/ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3528 2023-11-30 15:14:27.000000 certego_saas-0.7.8/certego_saas/ext/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2023-11-30 15:14:27.000000 certego_saas-0.7.8/certego_saas/ext/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6623 2023-11-30 15:14:27.000000 certego_saas-0.7.8/certego_saas/ext/log.py
--rw-r--r--   0 runner    (1001) docker     (127)     1445 2023-11-30 15:14:27.000000 certego_saas-0.7.8/certego_saas/ext/managers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2204 2023-11-30 15:14:27.000000 certego_saas-0.7.8/certego_saas/ext/middlewares.py
--rw-r--r--   0 runner    (1001) docker     (127)     2250 2023-11-30 15:14:27.000000 certego_saas-0.7.8/certego_saas/ext/mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)     2474 2023-11-30 15:14:27.000000 certego_saas-0.7.8/certego_saas/ext/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1655 2023-11-30 15:14:27.000000 certego_saas-0.7.8/certego_saas/ext/pagination.py
--rw-r--r--   0 runner    (1001) docker     (127)      705 2023-11-30 15:14:27.000000 certego_saas-0.7.8/certego_saas/ext/serializers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 15:14:37.621697 certego_saas-0.7.8/certego_saas/ext/test_utilities/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-30 15:14:27.000000 certego_saas-0.7.8/certego_saas/ext/test_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1613 2023-11-30 15:14:27.000000 certego_saas-0.7.8/certego_saas/ext/test_utilities/no_logs_test_case.py
--rw-r--r--   0 runner    (1001) docker     (127)      870 2023-11-30 15:14:27.000000 certego_saas-0.7.8/certego_saas/ext/test_utilities/timed_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1919 2023-11-30 15:14:27.000000 certego_saas-0.7.8/certego_saas/ext/throttling.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 15:14:37.621697 certego_saas-0.7.8/certego_saas/ext/upload/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2023-11-30 15:14:27.000000 certego_saas-0.7.8/certego_saas/ext/upload/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3053 2023-11-30 15:14:27.000000 certego_saas-0.7.8/certego_saas/ext/upload/elastic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1482 2023-11-30 15:14:27.000000 certego_saas-0.7.8/certego_saas/ext/upload/slack.py
--rw-r--r--   0 runner    (1001) docker     (127)     2689 2023-11-30 15:14:27.000000 certego_saas-0.7.8/certego_saas/ext/upload/twitter.py
--rw-r--r--   0 runner    (1001) docker     (127)      606 2023-11-30 15:14:27.000000 certego_saas-0.7.8/certego_saas/ext/views.py
--rw-r--r--   0 runner    (1001) docker     (127)     1637 2023-11-30 15:14:27.000000 certego_saas-0.7.8/certego_saas/ext/viewsets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 15:14:37.621697 certego_saas-0.7.8/certego_saas/management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-30 15:14:27.000000 certego_saas-0.7.8/certego_saas/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 15:14:37.621697 certego_saas-0.7.8/certego_saas/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-30 15:14:27.000000 certego_saas-0.7.8/certego_saas/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4005 2023-11-30 15:14:27.000000 certego_saas-0.7.8/certego_saas/management/commands/celery.py
--rw-r--r--   0 runner    (1001) docker     (127)     4810 2023-11-30 15:14:27.000000 certego_saas-0.7.8/certego_saas/management/commands/duplicates.py
--rw-r--r--   0 runner    (1001) docker     (127)     3703 2023-11-30 15:14:27.000000 certego_saas-0.7.8/certego_saas/management/commands/queues.py
--rw-r--r--   0 runner    (1001) docker     (127)      828 2023-11-30 15:14:27.000000 certego_saas-0.7.8/certego_saas/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2156 2023-11-30 15:14:27.000000 certego_saas-0.7.8/certego_saas/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 15:14:37.621697 certego_saas-0.7.8/certego_saas/templates/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-30 15:14:27.000000 certego_saas-0.7.8/certego_saas/templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 15:14:37.605697 certego_saas-0.7.8/certego_saas/templates/certego_saas/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 15:14:37.625697 certego_saas-0.7.8/certego_saas/templates/certego_saas/emails/
--rw-r--r--   0 runner    (1001) docker     (127)      571 2023-11-30 15:14:27.000000 certego_saas-0.7.8/certego_saas/templates/certego_saas/emails/base.html
--rw-r--r--   0 runner    (1001) docker     (127)     6392 2023-11-30 15:14:27.000000 certego_saas-0.7.8/certego_saas/templates/certego_saas/emails/certego-logo-positive.png
--rw-r--r--   0 runner    (1001) docker     (127)      572 2023-11-30 15:14:27.000000 certego_saas-0.7.8/certego_saas/templates/certego_saas/emails/org-invitation.html
--rw-r--r--   0 runner    (1001) docker     (127)      338 2023-11-30 15:14:27.000000 certego_saas-0.7.8/certego_saas/templates/context_processors.py
--rw-r--r--   0 runner    (1001) docker     (127)      266 2023-11-30 15:14:27.000000 certego_saas-0.7.8/certego_saas/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)       18 2023-11-30 15:14:27.000000 certego_saas-0.7.8/certego_saas/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 15:14:37.625697 certego_saas-0.7.8/certego_saas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4303 2023-11-30 15:14:37.000000 certego_saas-0.7.8/certego_saas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5393 2023-11-30 15:14:37.000000 certego_saas-0.7.8/certego_saas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-30 15:14:37.000000 certego_saas-0.7.8/certego_saas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      944 2023-11-30 15:14:37.000000 certego_saas-0.7.8/certego_saas.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2023-11-30 15:14:37.000000 certego_saas-0.7.8/certego_saas.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      361 2023-11-30 15:14:27.000000 certego_saas-0.7.8/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 15:14:37.625697 certego_saas-0.7.8/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      247 2023-11-30 15:14:27.000000 certego_saas-0.7.8/requirements/requirements.dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      423 2023-11-30 15:14:27.000000 certego_saas-0.7.8/requirements/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-30 15:14:37.629697 certego_saas-0.7.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1646 2023-11-30 15:14:27.000000 certego_saas-0.7.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 15:14:37.625697 certego_saas-0.7.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      816 2023-11-30 15:14:27.000000 certego_saas-0.7.8/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 15:14:37.625697 certego_saas-0.7.8/tests/apps/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-30 15:14:27.000000 certego_saas-0.7.8/tests/apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 15:14:37.625697 certego_saas-0.7.8/tests/apps/auth/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-30 15:14:27.000000 certego_saas-0.7.8/tests/apps/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3360 2023-11-30 15:14:27.000000 certego_saas-0.7.8/tests/apps/auth/test_auth.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 15:14:37.625697 certego_saas-0.7.8/tests/apps/feedback/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-30 15:14:27.000000 certego_saas-0.7.8/tests/apps/feedback/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      858 2023-11-30 15:14:27.000000 certego_saas-0.7.8/tests/apps/feedback/test_feedback.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 15:14:37.625697 certego_saas-0.7.8/tests/apps/notifications/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-30 15:14:27.000000 certego_saas-0.7.8/tests/apps/notifications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2853 2023-11-30 15:14:27.000000 certego_saas-0.7.8/tests/apps/notifications/test_notifications.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 15:14:37.625697 certego_saas-0.7.8/tests/apps/organization/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-30 15:14:27.000000 certego_saas-0.7.8/tests/apps/organization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9012 2023-11-30 15:14:27.000000 certego_saas-0.7.8/tests/apps/organization/test_invitation.py
--rw-r--r--   0 runner    (1001) docker     (127)    24136 2023-11-30 15:14:27.000000 certego_saas-0.7.8/tests/apps/organization/test_organization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 15:14:37.625697 certego_saas-0.7.8/tests/apps/payments/
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2023-11-30 15:14:27.000000 certego_saas-0.7.8/tests/apps/payments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      499 2023-11-30 15:14:27.000000 certego_saas-0.7.8/tests/apps/payments/test_payments.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 15:14:37.625697 certego_saas-0.7.8/tests/apps/user/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-30 15:14:27.000000 certego_saas-0.7.8/tests/apps/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      780 2023-11-30 15:14:27.000000 certego_saas-0.7.8/tests/apps/user/test_user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 15:14:37.625697 certego_saas-0.7.8/tests/ext/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-30 15:14:27.000000 certego_saas-0.7.8/tests/ext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 15:14:37.625697 certego_saas-0.7.8/tests/ext/upload/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-30 15:14:27.000000 certego_saas-0.7.8/tests/ext/upload/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      307 2023-11-30 15:14:27.000000 certego_saas-0.7.8/tests/ext/upload/test_slack.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 15:14:37.625697 certego_saas-0.7.8/tests/management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-30 15:14:27.000000 certego_saas-0.7.8/tests/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 15:14:37.625697 certego_saas-0.7.8/tests/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-30 15:14:27.000000 certego_saas-0.7.8/tests/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-30 15:14:27.000000 certego_saas-0.7.8/tests/management/commands/test_celery.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-30 15:14:27.000000 certego_saas-0.7.8/tests/management/commands/test_duplicates.py
--rw-r--r--   0 runner    (1001) docker     (127)       78 2023-11-30 15:14:27.000000 certego_saas-0.7.8/tests/management/commands/test_queues.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:47:14.725296 certego_saas-0.7.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-16 07:47:07.000000 certego_saas-0.7.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-16 07:47:07.000000 certego_saas-0.7.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4303 2024-04-16 07:47:14.725296 certego_saas-0.7.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-04-16 07:47:07.000000 certego_saas-0.7.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:47:14.697296 certego_saas-0.7.9/certego_saas/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 07:47:07.000000 certego_saas-0.7.9/certego_saas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:47:14.697296 certego_saas-0.7.9/certego_saas/apps/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 07:47:07.000000 certego_saas-0.7.9/certego_saas/apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:47:14.701296 certego_saas-0.7.9/certego_saas/apps/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 07:47:07.000000 certego_saas-0.7.9/certego_saas/apps/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-16 07:47:07.000000 certego_saas-0.7.9/certego_saas/apps/auth/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-16 07:47:07.000000 certego_saas-0.7.9/certego_saas/apps/auth/backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-16 07:47:07.000000 certego_saas-0.7.9/certego_saas/apps/auth/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-04-16 07:47:07.000000 certego_saas-0.7.9/certego_saas/apps/auth/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:47:14.701296 certego_saas-0.7.9/certego_saas/apps/feedback/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 07:47:07.000000 certego_saas-0.7.9/certego_saas/apps/feedback/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-16 07:47:07.000000 certego_saas-0.7.9/certego_saas/apps/feedback/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-16 07:47:07.000000 certego_saas-0.7.9/certego_saas/apps/feedback/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:47:14.701296 certego_saas-0.7.9/certego_saas/apps/feedback/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-04-16 07:47:07.000000 certego_saas-0.7.9/certego_saas/apps/feedback/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 07:47:07.000000 certego_saas-0.7.9/certego_saas/apps/feedback/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-04-16 07:47:07.000000 certego_saas-0.7.9/certego_saas/apps/feedback/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      906 2024-04-16 07:47:07.000000 certego_saas-0.7.9/certego_saas/apps/feedback/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-16 07:47:07.000000 certego_saas-0.7.9/certego_saas/apps/feedback/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-16 07:47:07.000000 certego_saas-0.7.9/certego_saas/apps/feedback/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:47:14.701296 certego_saas-0.7.9/certego_saas/apps/notifications/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 07:47:07.000000 certego_saas-0.7.9/certego_saas/apps/notifications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-16 07:47:07.000000 certego_saas-0.7.9/certego_saas/apps/notifications/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-16 07:47:07.000000 certego_saas-0.7.9/certego_saas/apps/notifications/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-16 07:47:07.000000 certego_saas-0.7.9/certego_saas/apps/notifications/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:47:14.701296 certego_saas-0.7.9/certego_saas/apps/notifications/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 07:47:07.000000 certego_saas-0.7.9/certego_saas/apps/notifications/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:47:14.701296 certego_saas-0.7.9/certego_saas/apps/notifications/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 07:47:07.000000 certego_saas-0.7.9/certego_saas/apps/notifications/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3949 2024-04-16 07:47:07.000000 certego_saas-0.7.9/certego_saas/apps/notifications/management/commands/changelog_notification.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:47:14.705296 certego_saas-0.7.9/certego_saas/apps/notifications/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-04-16 07:47:07.000000 certego_saas-0.7.9/certego_saas/apps/notifications/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-16 07:47:07.000000 certego_saas-0.7.9/certego_saas/apps/notifications/migrations/0002_alter_notification_appname.py
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-04-16 07:47:07.000000 certego_saas-0.7.9/certego_saas/apps/notifications/migrations/0003_for_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-16 07:47:07.000000 certego_saas-0.7.9/certego_saas/apps/notifications/migrations/0004_for_user_blank.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 07:47:07.000000 certego_saas-0.7.9/certego_saas/apps/notifications/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-16 07:47:07.000000 certego_saas-0.7.9/certego_saas/apps/notifications/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-16 07:47:07.000000 certego_saas-0.7.9/certego_saas/apps/notifications/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-16 07:47:07.000000 certego_saas-0.7.9/certego_saas/apps/notifications/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2640 2024-04-16 07:47:07.000000 certego_saas-0.7.9/certego_saas/apps/notifications/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:47:14.705296 certego_saas-0.7.9/certego_saas/apps/organization/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 07:47:07.000000 certego_saas-0.7.9/certego_saas/apps/organization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-16 07:47:07.000000 certego_saas-0.7.9/certego_saas/apps/organization/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-16 07:47:07.000000 certego_saas-0.7.9/certego_saas/apps/organization/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4735 2024-04-16 07:47:07.000000 certego_saas-0.7.9/certego_saas/apps/organization/invitation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-04-16 07:47:07.000000 certego_saas-0.7.9/certego_saas/apps/organization/membership.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:47:14.705296 certego_saas-0.7.9/certego_saas/apps/organization/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     4125 2024-04-16 07:47:07.000000 certego_saas-0.7.9/certego_saas/apps/organization/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-16 07:47:07.000000 certego_saas-0.7.9/certego_saas/apps/organization/migrations/0002_membership_is_admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 07:47:07.000000 certego_saas-0.7.9/certego_saas/apps/organization/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-04-16 07:47:07.000000 certego_saas-0.7.9/certego_saas/apps/organization/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-16 07:47:07.000000 certego_saas-0.7.9/certego_saas/apps/organization/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3424 2024-04-16 07:47:07.000000 certego_saas-0.7.9/certego_saas/apps/organization/organization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-04-16 07:47:07.000000 certego_saas-0.7.9/certego_saas/apps/organization/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4415 2024-04-16 07:47:07.000000 certego_saas-0.7.9/certego_saas/apps/organization/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-16 07:47:07.000000 certego_saas-0.7.9/certego_saas/apps/organization/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9689 2024-04-16 07:47:07.000000 certego_saas-0.7.9/certego_saas/apps/organization/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:47:14.709296 certego_saas-0.7.9/certego_saas/apps/payments/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 07:47:07.000000 certego_saas-0.7.9/certego_saas/apps/payments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-16 07:47:07.000000 certego_saas-0.7.9/certego_saas/apps/payments/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-16 07:47:07.000000 certego_saas-0.7.9/certego_saas/apps/payments/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-16 07:47:07.000000 certego_saas-0.7.9/certego_saas/apps/payments/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-16 07:47:07.000000 certego_saas-0.7.9/certego_saas/apps/payments/consts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-04-16 07:47:07.000000 certego_saas-0.7.9/certego_saas/apps/payments/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:47:14.709296 certego_saas-0.7.9/certego_saas/apps/payments/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-04-16 07:47:07.000000 certego_saas-0.7.9/certego_saas/apps/payments/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 07:47:07.000000 certego_saas-0.7.9/certego_saas/apps/payments/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10336 2024-04-16 07:47:07.000000 certego_saas-0.7.9/certego_saas/apps/payments/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-16 07:47:07.000000 certego_saas-0.7.9/certego_saas/apps/payments/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-04-16 07:47:07.000000 certego_saas-0.7.9/certego_saas/apps/payments/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-16 07:47:07.000000 certego_saas-0.7.9/certego_saas/apps/payments/throttling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-04-16 07:47:07.000000 certego_saas-0.7.9/certego_saas/apps/payments/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:47:14.709296 certego_saas-0.7.9/certego_saas/apps/user/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 07:47:07.000000 certego_saas-0.7.9/certego_saas/apps/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-04-16 07:47:07.000000 certego_saas-0.7.9/certego_saas/apps/user/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-16 07:47:07.000000 certego_saas-0.7.9/certego_saas/apps/user/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-16 07:47:07.000000 certego_saas-0.7.9/certego_saas/apps/user/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:47:14.709296 certego_saas-0.7.9/certego_saas/apps/user/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     5021 2024-04-16 07:47:07.000000 certego_saas-0.7.9/certego_saas/apps/user/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-04-16 07:47:07.000000 certego_saas-0.7.9/certego_saas/apps/user/migrations/0002_migration.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 07:47:07.000000 certego_saas-0.7.9/certego_saas/apps/user/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4817 2024-04-16 07:47:07.000000 certego_saas-0.7.9/certego_saas/apps/user/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-04-16 07:47:07.000000 certego_saas-0.7.9/certego_saas/apps/user/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-16 07:47:07.000000 certego_saas-0.7.9/certego_saas/apps/user/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-04-16 07:47:07.000000 certego_saas-0.7.9/certego_saas/apps/user/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-16 07:47:07.000000 certego_saas-0.7.9/certego_saas/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:47:14.713296 certego_saas-0.7.9/certego_saas/ext/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 07:47:07.000000 certego_saas-0.7.9/certego_saas/ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3528 2024-04-16 07:47:07.000000 certego_saas-0.7.9/certego_saas/ext/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-16 07:47:07.000000 certego_saas-0.7.9/certego_saas/ext/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6623 2024-04-16 07:47:07.000000 certego_saas-0.7.9/certego_saas/ext/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-04-16 07:47:07.000000 certego_saas-0.7.9/certego_saas/ext/managers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2204 2024-04-16 07:47:07.000000 certego_saas-0.7.9/certego_saas/ext/middlewares.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-04-16 07:47:07.000000 certego_saas-0.7.9/certego_saas/ext/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-04-16 07:47:07.000000 certego_saas-0.7.9/certego_saas/ext/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-04-16 07:47:07.000000 certego_saas-0.7.9/certego_saas/ext/pagination.py
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-16 07:47:07.000000 certego_saas-0.7.9/certego_saas/ext/serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:47:14.713296 certego_saas-0.7.9/certego_saas/ext/test_utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 07:47:07.000000 certego_saas-0.7.9/certego_saas/ext/test_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-04-16 07:47:07.000000 certego_saas-0.7.9/certego_saas/ext/test_utilities/no_logs_test_case.py
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-16 07:47:07.000000 certego_saas-0.7.9/certego_saas/ext/test_utilities/timed_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-04-16 07:47:07.000000 certego_saas-0.7.9/certego_saas/ext/throttling.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:47:14.713296 certego_saas-0.7.9/certego_saas/ext/upload/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-16 07:47:07.000000 certego_saas-0.7.9/certego_saas/ext/upload/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3024 2024-04-16 07:47:07.000000 certego_saas-0.7.9/certego_saas/ext/upload/elastic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-04-16 07:47:07.000000 certego_saas-0.7.9/certego_saas/ext/upload/slack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2689 2024-04-16 07:47:07.000000 certego_saas-0.7.9/certego_saas/ext/upload/twitter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-16 07:47:07.000000 certego_saas-0.7.9/certego_saas/ext/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-04-16 07:47:07.000000 certego_saas-0.7.9/certego_saas/ext/viewsets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:47:14.713296 certego_saas-0.7.9/certego_saas/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 07:47:07.000000 certego_saas-0.7.9/certego_saas/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:47:14.713296 certego_saas-0.7.9/certego_saas/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 07:47:07.000000 certego_saas-0.7.9/certego_saas/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-04-16 07:47:07.000000 certego_saas-0.7.9/certego_saas/management/commands/celery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4810 2024-04-16 07:47:07.000000 certego_saas-0.7.9/certego_saas/management/commands/duplicates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3703 2024-04-16 07:47:07.000000 certego_saas-0.7.9/certego_saas/management/commands/queues.py
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-16 07:47:07.000000 certego_saas-0.7.9/certego_saas/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-04-16 07:47:07.000000 certego_saas-0.7.9/certego_saas/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:47:14.717296 certego_saas-0.7.9/certego_saas/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 07:47:07.000000 certego_saas-0.7.9/certego_saas/templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:47:14.693296 certego_saas-0.7.9/certego_saas/templates/certego_saas/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:47:14.717296 certego_saas-0.7.9/certego_saas/templates/certego_saas/emails/
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-16 07:47:07.000000 certego_saas-0.7.9/certego_saas/templates/certego_saas/emails/base.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6392 2024-04-16 07:47:07.000000 certego_saas-0.7.9/certego_saas/templates/certego_saas/emails/certego-logo-positive.png
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-16 07:47:07.000000 certego_saas-0.7.9/certego_saas/templates/certego_saas/emails/org-invitation.html
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-16 07:47:07.000000 certego_saas-0.7.9/certego_saas/templates/context_processors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-16 07:47:07.000000 certego_saas-0.7.9/certego_saas/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-16 07:47:07.000000 certego_saas-0.7.9/certego_saas/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:47:14.721296 certego_saas-0.7.9/certego_saas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4303 2024-04-16 07:47:14.000000 certego_saas-0.7.9/certego_saas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5393 2024-04-16 07:47:14.000000 certego_saas-0.7.9/certego_saas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 07:47:14.000000 certego_saas-0.7.9/certego_saas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-04-16 07:47:14.000000 certego_saas-0.7.9/certego_saas.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-16 07:47:14.000000 certego_saas-0.7.9/certego_saas.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-16 07:47:07.000000 certego_saas-0.7.9/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:47:14.717296 certego_saas-0.7.9/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-16 07:47:07.000000 certego_saas-0.7.9/requirements/requirements.dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-16 07:47:07.000000 certego_saas-0.7.9/requirements/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 07:47:14.725296 certego_saas-0.7.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-04-16 07:47:07.000000 certego_saas-0.7.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:47:14.717296 certego_saas-0.7.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-16 07:47:07.000000 certego_saas-0.7.9/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:47:14.717296 certego_saas-0.7.9/tests/apps/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 07:47:07.000000 certego_saas-0.7.9/tests/apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:47:14.717296 certego_saas-0.7.9/tests/apps/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 07:47:07.000000 certego_saas-0.7.9/tests/apps/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3360 2024-04-16 07:47:07.000000 certego_saas-0.7.9/tests/apps/auth/test_auth.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:47:14.717296 certego_saas-0.7.9/tests/apps/feedback/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 07:47:07.000000 certego_saas-0.7.9/tests/apps/feedback/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-04-16 07:47:07.000000 certego_saas-0.7.9/tests/apps/feedback/test_feedback.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:47:14.717296 certego_saas-0.7.9/tests/apps/notifications/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 07:47:07.000000 certego_saas-0.7.9/tests/apps/notifications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-04-16 07:47:07.000000 certego_saas-0.7.9/tests/apps/notifications/test_notifications.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:47:14.717296 certego_saas-0.7.9/tests/apps/organization/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 07:47:07.000000 certego_saas-0.7.9/tests/apps/organization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9012 2024-04-16 07:47:07.000000 certego_saas-0.7.9/tests/apps/organization/test_invitation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24136 2024-04-16 07:47:07.000000 certego_saas-0.7.9/tests/apps/organization/test_organization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:47:14.717296 certego_saas-0.7.9/tests/apps/payments/
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-04-16 07:47:07.000000 certego_saas-0.7.9/tests/apps/payments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-16 07:47:07.000000 certego_saas-0.7.9/tests/apps/payments/test_payments.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:47:14.717296 certego_saas-0.7.9/tests/apps/user/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 07:47:07.000000 certego_saas-0.7.9/tests/apps/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-16 07:47:07.000000 certego_saas-0.7.9/tests/apps/user/test_user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:47:14.717296 certego_saas-0.7.9/tests/ext/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 07:47:07.000000 certego_saas-0.7.9/tests/ext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:47:14.721296 certego_saas-0.7.9/tests/ext/upload/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 07:47:07.000000 certego_saas-0.7.9/tests/ext/upload/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-16 07:47:07.000000 certego_saas-0.7.9/tests/ext/upload/test_slack.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:47:14.721296 certego_saas-0.7.9/tests/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 07:47:07.000000 certego_saas-0.7.9/tests/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:47:14.721296 certego_saas-0.7.9/tests/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 07:47:07.000000 certego_saas-0.7.9/tests/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 07:47:07.000000 certego_saas-0.7.9/tests/management/commands/test_celery.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 07:47:07.000000 certego_saas-0.7.9/tests/management/commands/test_duplicates.py
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-16 07:47:07.000000 certego_saas-0.7.9/tests/management/commands/test_queues.py
```

### Comparing `certego_saas-0.7.8/LICENSE` & `certego_saas-0.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `certego_saas-0.7.8/PKG-INFO` & `certego_saas-0.7.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: certego_saas
-Version: 0.7.8
+Version: 0.7.9
 Summary: Certego SaaS
 Home-page: https://github.com/certego/certego-saas
 Author: Certego S.R.L
 License: MIT
 Project-URL: Documentation, https://github.com/certego/certego-saas
 Project-URL: Source, https://github.com/certego/certego-saas
 Project-URL: Tracker, https://github.com/certego/certego-saas/issues
```

### Comparing `certego_saas-0.7.8/README.md` & `certego_saas-0.7.9/README.md`

 * *Files identical despite different names*

### Comparing `certego_saas-0.7.8/certego_saas/apps/auth/backend.py` & `certego_saas-0.7.9/certego_saas/apps/auth/backend.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.7.8/certego_saas/apps/auth/views.py` & `certego_saas-0.7.9/certego_saas/apps/auth/views.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.7.8/certego_saas/apps/feedback/migrations/0001_initial.py` & `certego_saas-0.7.9/certego_saas/apps/feedback/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.7.8/certego_saas/apps/feedback/models.py` & `certego_saas-0.7.9/certego_saas/apps/feedback/models.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.7.8/certego_saas/apps/feedback/serializers.py` & `certego_saas-0.7.9/certego_saas/apps/feedback/serializers.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.7.8/certego_saas/apps/feedback/views.py` & `certego_saas-0.7.9/certego_saas/apps/feedback/views.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.7.8/certego_saas/apps/notifications/filters.py` & `certego_saas-0.7.9/certego_saas/apps/notifications/filters.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.7.8/certego_saas/apps/notifications/management/commands/changelog_notification.py` & `certego_saas-0.7.9/certego_saas/apps/notifications/management/commands/changelog_notification.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.7.8/certego_saas/apps/notifications/migrations/0001_initial.py` & `certego_saas-0.7.9/certego_saas/apps/notifications/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.7.8/certego_saas/apps/notifications/migrations/0002_alter_notification_appname.py` & `certego_saas-0.7.9/certego_saas/apps/notifications/migrations/0002_alter_notification_appname.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.7.8/certego_saas/apps/notifications/migrations/0003_for_user.py` & `certego_saas-0.7.9/certego_saas/apps/notifications/migrations/0003_for_user.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.7.8/certego_saas/apps/notifications/migrations/0004_for_user_blank.py` & `certego_saas-0.7.9/certego_saas/apps/notifications/migrations/0004_for_user_blank.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.7.8/certego_saas/apps/notifications/models.py` & `certego_saas-0.7.9/certego_saas/apps/notifications/models.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.7.8/certego_saas/apps/notifications/serializers.py` & `certego_saas-0.7.9/certego_saas/apps/notifications/serializers.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.7.8/certego_saas/apps/notifications/views.py` & `certego_saas-0.7.9/certego_saas/apps/notifications/views.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.7.8/certego_saas/apps/organization/admin.py` & `certego_saas-0.7.9/certego_saas/apps/organization/admin.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.7.8/certego_saas/apps/organization/invitation.py` & `certego_saas-0.7.9/certego_saas/apps/organization/invitation.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.7.8/certego_saas/apps/organization/membership.py` & `certego_saas-0.7.9/certego_saas/apps/organization/membership.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.7.8/certego_saas/apps/organization/migrations/0001_initial.py` & `certego_saas-0.7.9/certego_saas/apps/organization/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.7.8/certego_saas/apps/organization/mixins.py` & `certego_saas-0.7.9/certego_saas/apps/organization/mixins.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.7.8/certego_saas/apps/organization/organization.py` & `certego_saas-0.7.9/certego_saas/apps/organization/organization.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.7.8/certego_saas/apps/organization/permissions.py` & `certego_saas-0.7.9/certego_saas/apps/organization/permissions.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.7.8/certego_saas/apps/organization/serializers.py` & `certego_saas-0.7.9/certego_saas/apps/organization/serializers.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.7.8/certego_saas/apps/organization/views.py` & `certego_saas-0.7.9/certego_saas/apps/organization/views.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.7.8/certego_saas/apps/payments/admin.py` & `certego_saas-0.7.9/certego_saas/apps/payments/admin.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.7.8/certego_saas/apps/payments/cache.py` & `certego_saas-0.7.9/certego_saas/apps/payments/cache.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.7.8/certego_saas/apps/payments/consts.py` & `certego_saas-0.7.9/certego_saas/apps/payments/consts.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.7.8/certego_saas/apps/payments/exceptions.py` & `certego_saas-0.7.9/certego_saas/apps/payments/exceptions.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.7.8/certego_saas/apps/payments/migrations/0001_initial.py` & `certego_saas-0.7.9/certego_saas/apps/payments/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.7.8/certego_saas/apps/payments/models.py` & `certego_saas-0.7.9/certego_saas/apps/payments/models.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.7.8/certego_saas/apps/payments/permissions.py` & `certego_saas-0.7.9/certego_saas/apps/payments/permissions.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.7.8/certego_saas/apps/payments/serializers.py` & `certego_saas-0.7.9/certego_saas/apps/payments/serializers.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.7.8/certego_saas/apps/payments/throttling.py` & `certego_saas-0.7.9/certego_saas/apps/payments/throttling.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.7.8/certego_saas/apps/payments/utils.py` & `certego_saas-0.7.9/certego_saas/apps/payments/utils.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.7.8/certego_saas/apps/user/admin.py` & `certego_saas-0.7.9/certego_saas/apps/user/admin.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.7.8/certego_saas/apps/user/forms.py` & `certego_saas-0.7.9/certego_saas/apps/user/forms.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.7.8/certego_saas/apps/user/migrations/0001_initial.py` & `certego_saas-0.7.9/certego_saas/apps/user/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.7.8/certego_saas/apps/user/migrations/0002_migration.py` & `certego_saas-0.7.9/certego_saas/apps/user/migrations/0002_migration.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.7.8/certego_saas/apps/user/models.py` & `certego_saas-0.7.9/certego_saas/apps/user/models.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.7.8/certego_saas/apps/user/serializers.py` & `certego_saas-0.7.9/certego_saas/apps/user/serializers.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.7.8/certego_saas/apps/user/views.py` & `certego_saas-0.7.9/certego_saas/apps/user/views.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.7.8/certego_saas/ext/exceptions.py` & `certego_saas-0.7.9/certego_saas/ext/exceptions.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.7.8/certego_saas/ext/helpers.py` & `certego_saas-0.7.9/certego_saas/ext/helpers.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.7.8/certego_saas/ext/log.py` & `certego_saas-0.7.9/certego_saas/ext/log.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.7.8/certego_saas/ext/managers.py` & `certego_saas-0.7.9/certego_saas/ext/managers.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.7.8/certego_saas/ext/middlewares.py` & `certego_saas-0.7.9/certego_saas/ext/middlewares.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.7.8/certego_saas/ext/mixins.py` & `certego_saas-0.7.9/certego_saas/ext/mixins.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.7.8/certego_saas/ext/models.py` & `certego_saas-0.7.9/certego_saas/ext/models.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.7.8/certego_saas/ext/pagination.py` & `certego_saas-0.7.9/certego_saas/ext/pagination.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.7.8/certego_saas/ext/serializers.py` & `certego_saas-0.7.9/certego_saas/ext/serializers.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.7.8/certego_saas/ext/test_utilities/no_logs_test_case.py` & `certego_saas-0.7.9/certego_saas/ext/test_utilities/no_logs_test_case.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.7.8/certego_saas/ext/test_utilities/timed_runner.py` & `certego_saas-0.7.9/certego_saas/ext/test_utilities/timed_runner.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.7.8/certego_saas/ext/throttling.py` & `certego_saas-0.7.9/certego_saas/ext/throttling.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.7.8/certego_saas/ext/upload/elastic.py` & `certego_saas-0.7.9/certego_saas/ext/upload/elastic.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,15 +26,14 @@
         logger.debug(f"Json document: {res}")
         return res
 
     def to_bulk(self) -> Dict[str, Any]:
         return {
             "_op_type": "index",
             "_index": self.index,
-            "_type": "_doc",
             "_source": self.to_json(),
         }
 
     @classmethod
     def upload(
         cls,
         client: elasticsearch.Elasticsearch,
```

### Comparing `certego_saas-0.7.8/certego_saas/ext/upload/slack.py` & `certego_saas-0.7.9/certego_saas/ext/upload/slack.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.7.8/certego_saas/ext/upload/twitter.py` & `certego_saas-0.7.9/certego_saas/ext/upload/twitter.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.7.8/certego_saas/ext/views.py` & `certego_saas-0.7.9/certego_saas/ext/views.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.7.8/certego_saas/ext/viewsets.py` & `certego_saas-0.7.9/certego_saas/ext/viewsets.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.7.8/certego_saas/management/commands/celery.py` & `certego_saas-0.7.9/certego_saas/management/commands/celery.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.7.8/certego_saas/management/commands/duplicates.py` & `certego_saas-0.7.9/certego_saas/management/commands/duplicates.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.7.8/certego_saas/management/commands/queues.py` & `certego_saas-0.7.9/certego_saas/management/commands/queues.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.7.8/certego_saas/models.py` & `certego_saas-0.7.9/certego_saas/models.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.7.8/certego_saas/settings.py` & `certego_saas-0.7.9/certego_saas/settings.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.7.8/certego_saas/templates/certego_saas/emails/base.html` & `certego_saas-0.7.9/certego_saas/templates/certego_saas/emails/base.html`

 * *Files identical despite different names*

### Comparing `certego_saas-0.7.8/certego_saas/templates/certego_saas/emails/certego-logo-positive.png` & `certego_saas-0.7.9/certego_saas/templates/certego_saas/emails/certego-logo-positive.png`

 * *Files identical despite different names*

### Comparing `certego_saas-0.7.8/certego_saas/templates/certego_saas/emails/org-invitation.html` & `certego_saas-0.7.9/certego_saas/templates/certego_saas/emails/org-invitation.html`

 * *Files identical despite different names*

### Comparing `certego_saas-0.7.8/certego_saas.egg-info/PKG-INFO` & `certego_saas-0.7.9/certego_saas.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: certego-saas
-Version: 0.7.8
+Name: certego_saas
+Version: 0.7.9
 Summary: Certego SaaS
 Home-page: https://github.com/certego/certego-saas
 Author: Certego S.R.L
 License: MIT
 Project-URL: Documentation, https://github.com/certego/certego-saas
 Project-URL: Source, https://github.com/certego/certego-saas
 Project-URL: Tracker, https://github.com/certego/certego-saas/issues
```

### Comparing `certego_saas-0.7.8/certego_saas.egg-info/SOURCES.txt` & `certego_saas-0.7.9/certego_saas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `certego_saas-0.7.8/certego_saas.egg-info/requires.txt` & `certego_saas-0.7.9/certego_saas.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `certego_saas-0.7.8/setup.py` & `certego_saas-0.7.9/setup.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.7.8/tests/__init__.py` & `certego_saas-0.7.9/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.7.8/tests/apps/auth/test_auth.py` & `certego_saas-0.7.9/tests/apps/auth/test_auth.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.7.8/tests/apps/feedback/test_feedback.py` & `certego_saas-0.7.9/tests/apps/feedback/test_feedback.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.7.8/tests/apps/notifications/test_notifications.py` & `certego_saas-0.7.9/tests/apps/notifications/test_notifications.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.7.8/tests/apps/organization/test_invitation.py` & `certego_saas-0.7.9/tests/apps/organization/test_invitation.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.7.8/tests/apps/organization/test_organization.py` & `certego_saas-0.7.9/tests/apps/organization/test_organization.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.7.8/tests/apps/payments/__init__.py` & `certego_saas-0.7.9/tests/apps/payments/__init__.py`

 * *Files identical despite different names*

### Comparing `certego_saas-0.7.8/tests/apps/user/test_user.py` & `certego_saas-0.7.9/tests/apps/user/test_user.py`

 * *Files identical despite different names*

