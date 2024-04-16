# Comparing `tmp/slurpit_nautobot-0.8.74.tar.gz` & `tmp/slurpit_nautobot-0.8.75.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slurpit_nautobot-0.8.74.tar", max compression
+gzip compressed data, was "slurpit_nautobot-0.8.75.tar", max compression
```

## Comparing `slurpit_nautobot-0.8.74.tar` & `slurpit_nautobot-0.8.75.tar`

### file list

```diff
@@ -1,62 +1,62 @@
--rw-r--r--   0        0        0     1064 2024-03-16 14:15:06.547086 slurpit_nautobot-0.8.74/LICENSE
--rw-r--r--   0        0        0     1220 2024-04-16 00:10:02.565306 slurpit_nautobot-0.8.74/README.md
--rw-r--r--   0        0        0      559 2024-04-16 10:19:23.470331 slurpit_nautobot-0.8.74/pyproject.toml
--rw-r--r--   0        0        0     1262 2024-04-16 10:19:23.470331 slurpit_nautobot-0.8.74/src/slurpit_nautobot/__init__.py
--rw-r--r--   0        0        0       46 2024-03-16 14:15:06.547086 slurpit_nautobot-0.8.74/src/slurpit_nautobot/api/__init__.py
--rw-r--r--   0        0        0     1993 2024-04-16 00:10:02.573306 slurpit_nautobot-0.8.74/src/slurpit_nautobot/api/serializers.py
--rw-r--r--   0        0        0      484 2024-03-17 21:19:15.970312 slurpit_nautobot-0.8.74/src/slurpit_nautobot/api/urls.py
--rw-r--r--   0        0        0     9406 2024-04-16 00:10:02.581306 slurpit_nautobot-0.8.74/src/slurpit_nautobot/api/views.py
--rw-r--r--   0        0        0     2547 2024-04-16 00:10:02.581306 slurpit_nautobot-0.8.74/src/slurpit_nautobot/decorators.py
--rw-r--r--   0        0        0     2040 2024-03-16 14:15:06.551086 slurpit_nautobot-0.8.74/src/slurpit_nautobot/filtersets.py
--rw-r--r--   0        0        0     7715 2024-04-16 00:10:02.585307 slurpit_nautobot-0.8.74/src/slurpit_nautobot/forms.py
--rw-r--r--   0        0        0    10767 2024-04-16 00:10:02.585307 slurpit_nautobot-0.8.74/src/slurpit_nautobot/importer.py
--rw-r--r--   0        0        0        0 2024-04-16 10:19:23.538331 slurpit_nautobot-0.8.74/src/slurpit_nautobot/management/__init__.py
--rw-r--r--   0        0        0     1159 2024-04-16 00:10:02.585307 slurpit_nautobot-0.8.74/src/slurpit_nautobot/management/choices.py
--rw-r--r--   0        0        0     9130 2024-03-16 14:15:06.551086 slurpit_nautobot-0.8.74/src/slurpit_nautobot/migrations/0001_initial.py
--rw-r--r--   0        0        0     1053 2024-03-17 14:29:31.470119 slurpit_nautobot-0.8.74/src/slurpit_nautobot/migrations/0002_auto_20240317_1425.py
--rw-r--r--   0        0        0      749 2024-04-16 00:10:02.585307 slurpit_nautobot-0.8.74/src/slurpit_nautobot/migrations/0003_manufacturer.py
--rw-r--r--   0        0        0      763 2024-04-16 00:10:02.589306 slurpit_nautobot-0.8.74/src/slurpit_nautobot/migrations/0004_auto_20240408_1105.py
--rw-r--r--   0        0        0      684 2024-04-16 00:10:02.589306 slurpit_nautobot-0.8.74/src/slurpit_nautobot/migrations/0005_locationtype_contenttype.py
--rw-r--r--   0        0        0        0 2024-04-16 10:19:23.546331 slurpit_nautobot-0.8.74/src/slurpit_nautobot/migrations/__init__.py
--rw-r--r--   0        0        0     5071 2024-04-16 00:10:02.589306 slurpit_nautobot-0.8.74/src/slurpit_nautobot/models/__init__.py
--rw-r--r--   0        0        0     3069 2024-04-16 00:10:02.589306 slurpit_nautobot-0.8.74/src/slurpit_nautobot/models/device.py
--rw-r--r--   0        0        0     1409 2024-03-16 14:15:06.551086 slurpit_nautobot-0.8.74/src/slurpit_nautobot/models/logs.py
--rw-r--r--   0        0        0      411 2024-03-16 14:15:06.551086 slurpit_nautobot-0.8.74/src/slurpit_nautobot/models/mapping.py
--rw-r--r--   0        0        0      844 2024-04-16 00:10:02.593306 slurpit_nautobot-0.8.74/src/slurpit_nautobot/models/planning.py
--rw-r--r--   0        0        0     1146 2024-03-16 14:15:06.551086 slurpit_nautobot-0.8.74/src/slurpit_nautobot/models/setting.py
--rw-r--r--   0        0        0     1975 2024-03-16 14:15:06.551086 slurpit_nautobot-0.8.74/src/slurpit_nautobot/navigation.py
--rw-r--r--   0        0        0      101 2024-04-16 00:10:02.593306 slurpit_nautobot-0.8.74/src/slurpit_nautobot/references/__init__.py
--rw-r--r--   0        0        0     1888 2024-04-16 00:10:02.593306 slurpit_nautobot-0.8.74/src/slurpit_nautobot/references/generic.py
--rw-r--r--   0        0        0      648 2024-04-16 00:10:02.593306 slurpit_nautobot-0.8.74/src/slurpit_nautobot/references/imports.py
--rw-r--r--   0        0        0      286 2024-03-16 14:15:06.551086 slurpit_nautobot-0.8.74/src/slurpit_nautobot/search.py
--rw-r--r--   0        0        0      528 2024-03-16 14:15:06.551086 slurpit_nautobot-0.8.74/src/slurpit_nautobot/slurpitch.py
--rw-r--r--   0        0        0     7586 2024-04-16 00:10:02.597306 slurpit_nautobot-0.8.74/src/slurpit_nautobot/tables.py
--rw-r--r--   0        0        0     1506 2024-04-16 00:10:02.597306 slurpit_nautobot-0.8.74/src/slurpit_nautobot/template_content.py
--rw-r--r--   0        0        0     3832 2024-04-16 00:10:02.597306 slurpit_nautobot-0.8.74/src/slurpit_nautobot/templates/slurpit_nautobot/bulk_edit.html
--rw-r--r--   0        0        0     1623 2024-03-16 14:15:06.551086 slurpit_nautobot-0.8.74/src/slurpit_nautobot/templates/slurpit_nautobot/comingsoon.html
--rw-r--r--   0        0        0     3425 2024-04-16 00:10:02.597306 slurpit_nautobot-0.8.74/src/slurpit_nautobot/templates/slurpit_nautobot/data_mapping.html
--rw-r--r--   0        0        0    22100 2024-04-16 00:10:02.601307 slurpit_nautobot-0.8.74/src/slurpit_nautobot/templates/slurpit_nautobot/logo.html
--rw-r--r--   0        0        0      352 2024-03-16 14:15:06.551086 slurpit_nautobot-0.8.74/src/slurpit_nautobot/templates/slurpit_nautobot/mapping/commingsoon.html
--rw-r--r--   0        0        0    17601 2024-04-16 02:39:11.393277 slurpit_nautobot-0.8.74/src/slurpit_nautobot/templates/slurpit_nautobot/mapping/nautobot_to_slurpit.html
--rw-r--r--   0        0        0     3637 2024-04-16 00:10:02.601307 slurpit_nautobot-0.8.74/src/slurpit_nautobot/templates/slurpit_nautobot/onboard/conflict_device_list.html
--rw-r--r--   0        0        0     3623 2024-04-16 00:10:02.601307 slurpit_nautobot-0.8.74/src/slurpit_nautobot/templates/slurpit_nautobot/onboard/migrate_device_list.html
--rw-r--r--   0        0        0     6638 2024-04-16 00:10:02.605306 slurpit_nautobot-0.8.74/src/slurpit_nautobot/templates/slurpit_nautobot/onboard/new_device_list.html
--rw-r--r--   0        0        0      475 2024-03-16 14:15:06.551086 slurpit_nautobot-0.8.74/src/slurpit_nautobot/templates/slurpit_nautobot/onboard/onboarded_device_list.html
--rw-r--r--   0        0        0     3628 2024-04-16 00:10:02.605306 slurpit_nautobot-0.8.74/src/slurpit_nautobot/templates/slurpit_nautobot/onboard_device.html
--rw-r--r--   0        0        0     4044 2024-04-16 00:10:02.605306 slurpit_nautobot-0.8.74/src/slurpit_nautobot/templates/slurpit_nautobot/planning_table.html
--rw-r--r--   0        0        0     3177 2024-04-16 00:10:02.605306 slurpit_nautobot-0.8.74/src/slurpit_nautobot/templates/slurpit_nautobot/settings/data_tabs.html
--rw-r--r--   0        0        0     9331 2024-04-16 00:10:02.609306 slurpit_nautobot-0.8.74/src/slurpit_nautobot/templates/slurpit_nautobot/settings/general.html
--rw-r--r--   0        0        0     2368 2024-04-16 00:10:02.605306 slurpit_nautobot-0.8.74/src/slurpit_nautobot/templates/slurpit_nautobot/settings.html
--rw-r--r--   0        0        0     2841 2024-04-16 00:10:02.613307 slurpit_nautobot-0.8.74/src/slurpit_nautobot/templates/slurpit_nautobot/slurpitlog_list.html
--rw-r--r--   0        0        0     2915 2024-04-16 00:10:02.621307 slurpit_nautobot-0.8.74/src/slurpit_nautobot/templates/slurpit_nautobot/table.html
--rw-r--r--   0        0        0      350 2024-03-16 14:15:06.555086 slurpit_nautobot-0.8.74/src/slurpit_nautobot/templates/slurpit_nautobot/table1.html
--rw-r--r--   0        0        0     1162 2024-03-16 14:15:06.555086 slurpit_nautobot-0.8.74/src/slurpit_nautobot/urls.py
--rw-r--r--   0        0        0      459 2024-03-16 14:15:06.555086 slurpit_nautobot-0.8.74/src/slurpit_nautobot/utilities.py
--rw-r--r--   0        0        0     1490 2024-04-16 00:10:02.629307 slurpit_nautobot-0.8.74/src/slurpit_nautobot/validator.py
--rw-r--r--   0        0        0      298 2024-03-16 14:15:06.555086 slurpit_nautobot-0.8.74/src/slurpit_nautobot/views/__init__.py
--rw-r--r--   0        0        0    10493 2024-04-16 10:19:23.470331 slurpit_nautobot-0.8.74/src/slurpit_nautobot/views/datamapping.py
--rw-r--r--   0        0        0     1073 2024-03-16 14:15:06.555086 slurpit_nautobot-0.8.74/src/slurpit_nautobot/views/logging.py
--rw-r--r--   0        0        0    14365 2024-04-16 00:10:02.637307 slurpit_nautobot-0.8.74/src/slurpit_nautobot/views/onboarding.py
--rw-r--r--   0        0        0      520 2024-03-16 14:15:06.555086 slurpit_nautobot-0.8.74/src/slurpit_nautobot/views/reconcile.py
--rw-r--r--   0        0        0    18895 2024-04-16 00:10:02.645307 slurpit_nautobot-0.8.74/src/slurpit_nautobot/views/setting.py
--rw-r--r--   0        0        0     1709 1970-01-01 00:00:00.000000 slurpit_nautobot-0.8.74/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-03-16 14:15:06.547086 slurpit_nautobot-0.8.75/LICENSE
+-rw-r--r--   0        0        0     1220 2024-04-16 00:10:02.565306 slurpit_nautobot-0.8.75/README.md
+-rw-r--r--   0        0        0      559 2024-04-16 11:12:17.598304 slurpit_nautobot-0.8.75/pyproject.toml
+-rw-r--r--   0        0        0     1262 2024-04-16 11:12:17.598304 slurpit_nautobot-0.8.75/src/slurpit_nautobot/__init__.py
+-rw-r--r--   0        0        0       46 2024-03-16 14:15:06.547086 slurpit_nautobot-0.8.75/src/slurpit_nautobot/api/__init__.py
+-rw-r--r--   0        0        0     1993 2024-04-16 00:10:02.573306 slurpit_nautobot-0.8.75/src/slurpit_nautobot/api/serializers.py
+-rw-r--r--   0        0        0      484 2024-03-17 21:19:15.970312 slurpit_nautobot-0.8.75/src/slurpit_nautobot/api/urls.py
+-rw-r--r--   0        0        0     9406 2024-04-16 00:10:02.581306 slurpit_nautobot-0.8.75/src/slurpit_nautobot/api/views.py
+-rw-r--r--   0        0        0     2547 2024-04-16 00:10:02.581306 slurpit_nautobot-0.8.75/src/slurpit_nautobot/decorators.py
+-rw-r--r--   0        0        0     2040 2024-03-16 14:15:06.551086 slurpit_nautobot-0.8.75/src/slurpit_nautobot/filtersets.py
+-rw-r--r--   0        0        0     7715 2024-04-16 00:10:02.585307 slurpit_nautobot-0.8.75/src/slurpit_nautobot/forms.py
+-rw-r--r--   0        0        0    10767 2024-04-16 00:10:02.585307 slurpit_nautobot-0.8.75/src/slurpit_nautobot/importer.py
+-rw-r--r--   0        0        0        0 2024-04-16 11:12:17.682305 slurpit_nautobot-0.8.75/src/slurpit_nautobot/management/__init__.py
+-rw-r--r--   0        0        0     1159 2024-04-16 00:10:02.585307 slurpit_nautobot-0.8.75/src/slurpit_nautobot/management/choices.py
+-rw-r--r--   0        0        0     9130 2024-03-16 14:15:06.551086 slurpit_nautobot-0.8.75/src/slurpit_nautobot/migrations/0001_initial.py
+-rw-r--r--   0        0        0     1053 2024-03-17 14:29:31.470119 slurpit_nautobot-0.8.75/src/slurpit_nautobot/migrations/0002_auto_20240317_1425.py
+-rw-r--r--   0        0        0      749 2024-04-16 00:10:02.585307 slurpit_nautobot-0.8.75/src/slurpit_nautobot/migrations/0003_manufacturer.py
+-rw-r--r--   0        0        0      763 2024-04-16 00:10:02.589306 slurpit_nautobot-0.8.75/src/slurpit_nautobot/migrations/0004_auto_20240408_1105.py
+-rw-r--r--   0        0        0      684 2024-04-16 00:10:02.589306 slurpit_nautobot-0.8.75/src/slurpit_nautobot/migrations/0005_locationtype_contenttype.py
+-rw-r--r--   0        0        0        0 2024-04-16 11:12:17.682305 slurpit_nautobot-0.8.75/src/slurpit_nautobot/migrations/__init__.py
+-rw-r--r--   0        0        0     5071 2024-04-16 00:10:02.589306 slurpit_nautobot-0.8.75/src/slurpit_nautobot/models/__init__.py
+-rw-r--r--   0        0        0     3069 2024-04-16 00:10:02.589306 slurpit_nautobot-0.8.75/src/slurpit_nautobot/models/device.py
+-rw-r--r--   0        0        0     1409 2024-03-16 14:15:06.551086 slurpit_nautobot-0.8.75/src/slurpit_nautobot/models/logs.py
+-rw-r--r--   0        0        0      411 2024-03-16 14:15:06.551086 slurpit_nautobot-0.8.75/src/slurpit_nautobot/models/mapping.py
+-rw-r--r--   0        0        0      844 2024-04-16 00:10:02.593306 slurpit_nautobot-0.8.75/src/slurpit_nautobot/models/planning.py
+-rw-r--r--   0        0        0     1146 2024-03-16 14:15:06.551086 slurpit_nautobot-0.8.75/src/slurpit_nautobot/models/setting.py
+-rw-r--r--   0        0        0     1975 2024-03-16 14:15:06.551086 slurpit_nautobot-0.8.75/src/slurpit_nautobot/navigation.py
+-rw-r--r--   0        0        0      101 2024-04-16 00:10:02.593306 slurpit_nautobot-0.8.75/src/slurpit_nautobot/references/__init__.py
+-rw-r--r--   0        0        0     1888 2024-04-16 00:10:02.593306 slurpit_nautobot-0.8.75/src/slurpit_nautobot/references/generic.py
+-rw-r--r--   0        0        0      648 2024-04-16 00:10:02.593306 slurpit_nautobot-0.8.75/src/slurpit_nautobot/references/imports.py
+-rw-r--r--   0        0        0      286 2024-03-16 14:15:06.551086 slurpit_nautobot-0.8.75/src/slurpit_nautobot/search.py
+-rw-r--r--   0        0        0      528 2024-03-16 14:15:06.551086 slurpit_nautobot-0.8.75/src/slurpit_nautobot/slurpitch.py
+-rw-r--r--   0        0        0     7586 2024-04-16 00:10:02.597306 slurpit_nautobot-0.8.75/src/slurpit_nautobot/tables.py
+-rw-r--r--   0        0        0     1506 2024-04-16 00:10:02.597306 slurpit_nautobot-0.8.75/src/slurpit_nautobot/template_content.py
+-rw-r--r--   0        0        0     3832 2024-04-16 00:10:02.597306 slurpit_nautobot-0.8.75/src/slurpit_nautobot/templates/slurpit_nautobot/bulk_edit.html
+-rw-r--r--   0        0        0     1623 2024-03-16 14:15:06.551086 slurpit_nautobot-0.8.75/src/slurpit_nautobot/templates/slurpit_nautobot/comingsoon.html
+-rw-r--r--   0        0        0     3425 2024-04-16 00:10:02.597306 slurpit_nautobot-0.8.75/src/slurpit_nautobot/templates/slurpit_nautobot/data_mapping.html
+-rw-r--r--   0        0        0    22100 2024-04-16 00:10:02.601307 slurpit_nautobot-0.8.75/src/slurpit_nautobot/templates/slurpit_nautobot/logo.html
+-rw-r--r--   0        0        0      352 2024-03-16 14:15:06.551086 slurpit_nautobot-0.8.75/src/slurpit_nautobot/templates/slurpit_nautobot/mapping/commingsoon.html
+-rw-r--r--   0        0        0    17601 2024-04-16 02:39:11.393277 slurpit_nautobot-0.8.75/src/slurpit_nautobot/templates/slurpit_nautobot/mapping/nautobot_to_slurpit.html
+-rw-r--r--   0        0        0     3637 2024-04-16 00:10:02.601307 slurpit_nautobot-0.8.75/src/slurpit_nautobot/templates/slurpit_nautobot/onboard/conflict_device_list.html
+-rw-r--r--   0        0        0     3623 2024-04-16 00:10:02.601307 slurpit_nautobot-0.8.75/src/slurpit_nautobot/templates/slurpit_nautobot/onboard/migrate_device_list.html
+-rw-r--r--   0        0        0     6638 2024-04-16 00:10:02.605306 slurpit_nautobot-0.8.75/src/slurpit_nautobot/templates/slurpit_nautobot/onboard/new_device_list.html
+-rw-r--r--   0        0        0      475 2024-03-16 14:15:06.551086 slurpit_nautobot-0.8.75/src/slurpit_nautobot/templates/slurpit_nautobot/onboard/onboarded_device_list.html
+-rw-r--r--   0        0        0     3628 2024-04-16 00:10:02.605306 slurpit_nautobot-0.8.75/src/slurpit_nautobot/templates/slurpit_nautobot/onboard_device.html
+-rw-r--r--   0        0        0     4553 2024-04-16 11:12:17.598304 slurpit_nautobot-0.8.75/src/slurpit_nautobot/templates/slurpit_nautobot/planning_table.html
+-rw-r--r--   0        0        0     3177 2024-04-16 00:10:02.605306 slurpit_nautobot-0.8.75/src/slurpit_nautobot/templates/slurpit_nautobot/settings/data_tabs.html
+-rw-r--r--   0        0        0     9331 2024-04-16 00:10:02.609306 slurpit_nautobot-0.8.75/src/slurpit_nautobot/templates/slurpit_nautobot/settings/general.html
+-rw-r--r--   0        0        0     2368 2024-04-16 00:10:02.605306 slurpit_nautobot-0.8.75/src/slurpit_nautobot/templates/slurpit_nautobot/settings.html
+-rw-r--r--   0        0        0     2841 2024-04-16 00:10:02.613307 slurpit_nautobot-0.8.75/src/slurpit_nautobot/templates/slurpit_nautobot/slurpitlog_list.html
+-rw-r--r--   0        0        0     2915 2024-04-16 00:10:02.621307 slurpit_nautobot-0.8.75/src/slurpit_nautobot/templates/slurpit_nautobot/table.html
+-rw-r--r--   0        0        0      350 2024-03-16 14:15:06.555086 slurpit_nautobot-0.8.75/src/slurpit_nautobot/templates/slurpit_nautobot/table1.html
+-rw-r--r--   0        0        0     1162 2024-03-16 14:15:06.555086 slurpit_nautobot-0.8.75/src/slurpit_nautobot/urls.py
+-rw-r--r--   0        0        0      459 2024-03-16 14:15:06.555086 slurpit_nautobot-0.8.75/src/slurpit_nautobot/utilities.py
+-rw-r--r--   0        0        0     1490 2024-04-16 00:10:02.629307 slurpit_nautobot-0.8.75/src/slurpit_nautobot/validator.py
+-rw-r--r--   0        0        0      298 2024-03-16 14:15:06.555086 slurpit_nautobot-0.8.75/src/slurpit_nautobot/views/__init__.py
+-rw-r--r--   0        0        0    10493 2024-04-16 10:19:23.470331 slurpit_nautobot-0.8.75/src/slurpit_nautobot/views/datamapping.py
+-rw-r--r--   0        0        0     1073 2024-03-16 14:15:06.555086 slurpit_nautobot-0.8.75/src/slurpit_nautobot/views/logging.py
+-rw-r--r--   0        0        0    14365 2024-04-16 00:10:02.637307 slurpit_nautobot-0.8.75/src/slurpit_nautobot/views/onboarding.py
+-rw-r--r--   0        0        0      520 2024-03-16 14:15:06.555086 slurpit_nautobot-0.8.75/src/slurpit_nautobot/views/reconcile.py
+-rw-r--r--   0        0        0    18895 2024-04-16 00:10:02.645307 slurpit_nautobot-0.8.75/src/slurpit_nautobot/views/setting.py
+-rw-r--r--   0        0        0     1709 1970-01-01 00:00:00.000000 slurpit_nautobot-0.8.75/PKG-INFO
```

### Comparing `slurpit_nautobot-0.8.74/LICENSE` & `slurpit_nautobot-0.8.75/LICENSE`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.74/README.md` & `slurpit_nautobot-0.8.75/README.md`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.74/pyproject.toml` & `slurpit_nautobot-0.8.75/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "slurpit_nautobot"
-version = "0.8.74"
+version = "0.8.75"
 description = ""
 authors = ["Pieter <pieter@slurpit.io>"]
 readme = "README.md"
 packages = [{include = "slurpit_nautobot", from = "src"}]
 
 
 [tool.poetry.dependencies]
```

### Comparing `slurpit_nautobot-0.8.74/src/slurpit_nautobot/__init__.py` & `slurpit_nautobot-0.8.75/src/slurpit_nautobot/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from nautobot.apps import NautobotAppConfig
 from nautobot.apps import config as app_config
 
 class SlurpitConfig(NautobotAppConfig):
     name = "slurpit_nautobot"
     verbose_name = "Slurp'it Plugin"
     description = "Sync Slurp'it into Nautobot"
-    version = '0.8.74'
+    version = '0.8.75'
     base_url = "slurpit"   
     default_settings = {
         'DeviceType': {'model': "Slurp'it"},
         'Role': {'name': "Slurp'it"},
         'Location': {'name': 'Slurp\'it'},
         'LocationType': {'name': 'Slurp\'it'},
         'Region': {'name': 'Slurp\'it'},
```

### Comparing `slurpit_nautobot-0.8.74/src/slurpit_nautobot/api/serializers.py` & `slurpit_nautobot-0.8.75/src/slurpit_nautobot/api/serializers.py`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.74/src/slurpit_nautobot/api/views.py` & `slurpit_nautobot-0.8.75/src/slurpit_nautobot/api/views.py`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.74/src/slurpit_nautobot/decorators.py` & `slurpit_nautobot-0.8.75/src/slurpit_nautobot/decorators.py`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.74/src/slurpit_nautobot/filtersets.py` & `slurpit_nautobot-0.8.75/src/slurpit_nautobot/filtersets.py`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.74/src/slurpit_nautobot/forms.py` & `slurpit_nautobot-0.8.75/src/slurpit_nautobot/forms.py`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.74/src/slurpit_nautobot/importer.py` & `slurpit_nautobot-0.8.75/src/slurpit_nautobot/importer.py`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.74/src/slurpit_nautobot/management/choices.py` & `slurpit_nautobot-0.8.75/src/slurpit_nautobot/management/choices.py`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.74/src/slurpit_nautobot/migrations/0001_initial.py` & `slurpit_nautobot-0.8.75/src/slurpit_nautobot/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.74/src/slurpit_nautobot/migrations/0002_auto_20240317_1425.py` & `slurpit_nautobot-0.8.75/src/slurpit_nautobot/migrations/0002_auto_20240317_1425.py`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.74/src/slurpit_nautobot/migrations/0003_manufacturer.py` & `slurpit_nautobot-0.8.75/src/slurpit_nautobot/migrations/0003_manufacturer.py`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.74/src/slurpit_nautobot/migrations/0004_auto_20240408_1105.py` & `slurpit_nautobot-0.8.75/src/slurpit_nautobot/migrations/0004_auto_20240408_1105.py`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.74/src/slurpit_nautobot/migrations/0005_locationtype_contenttype.py` & `slurpit_nautobot-0.8.75/src/slurpit_nautobot/migrations/0005_locationtype_contenttype.py`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.74/src/slurpit_nautobot/models/__init__.py` & `slurpit_nautobot-0.8.75/src/slurpit_nautobot/models/__init__.py`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.74/src/slurpit_nautobot/models/device.py` & `slurpit_nautobot-0.8.75/src/slurpit_nautobot/models/device.py`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.74/src/slurpit_nautobot/models/logs.py` & `slurpit_nautobot-0.8.75/src/slurpit_nautobot/models/logs.py`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.74/src/slurpit_nautobot/models/planning.py` & `slurpit_nautobot-0.8.75/src/slurpit_nautobot/models/planning.py`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.74/src/slurpit_nautobot/models/setting.py` & `slurpit_nautobot-0.8.75/src/slurpit_nautobot/models/setting.py`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.74/src/slurpit_nautobot/navigation.py` & `slurpit_nautobot-0.8.75/src/slurpit_nautobot/navigation.py`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.74/src/slurpit_nautobot/references/generic.py` & `slurpit_nautobot-0.8.75/src/slurpit_nautobot/references/generic.py`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.74/src/slurpit_nautobot/references/imports.py` & `slurpit_nautobot-0.8.75/src/slurpit_nautobot/references/imports.py`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.74/src/slurpit_nautobot/slurpitch.py` & `slurpit_nautobot-0.8.75/src/slurpit_nautobot/slurpitch.py`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.74/src/slurpit_nautobot/tables.py` & `slurpit_nautobot-0.8.75/src/slurpit_nautobot/tables.py`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.74/src/slurpit_nautobot/template_content.py` & `slurpit_nautobot-0.8.75/src/slurpit_nautobot/template_content.py`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.74/src/slurpit_nautobot/templates/slurpit_nautobot/bulk_edit.html` & `slurpit_nautobot-0.8.75/src/slurpit_nautobot/templates/slurpit_nautobot/bulk_edit.html`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.74/src/slurpit_nautobot/templates/slurpit_nautobot/comingsoon.html` & `slurpit_nautobot-0.8.75/src/slurpit_nautobot/templates/slurpit_nautobot/comingsoon.html`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.74/src/slurpit_nautobot/templates/slurpit_nautobot/data_mapping.html` & `slurpit_nautobot-0.8.75/src/slurpit_nautobot/templates/slurpit_nautobot/data_mapping.html`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.74/src/slurpit_nautobot/templates/slurpit_nautobot/logo.html` & `slurpit_nautobot-0.8.75/src/slurpit_nautobot/templates/slurpit_nautobot/logo.html`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.74/src/slurpit_nautobot/templates/slurpit_nautobot/mapping/nautobot_to_slurpit.html` & `slurpit_nautobot-0.8.75/src/slurpit_nautobot/templates/slurpit_nautobot/mapping/nautobot_to_slurpit.html`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.74/src/slurpit_nautobot/templates/slurpit_nautobot/onboard/conflict_device_list.html` & `slurpit_nautobot-0.8.75/src/slurpit_nautobot/templates/slurpit_nautobot/onboard/conflict_device_list.html`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.74/src/slurpit_nautobot/templates/slurpit_nautobot/onboard/migrate_device_list.html` & `slurpit_nautobot-0.8.75/src/slurpit_nautobot/templates/slurpit_nautobot/onboard/migrate_device_list.html`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.74/src/slurpit_nautobot/templates/slurpit_nautobot/onboard/new_device_list.html` & `slurpit_nautobot-0.8.75/src/slurpit_nautobot/templates/slurpit_nautobot/onboard/new_device_list.html`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.74/src/slurpit_nautobot/templates/slurpit_nautobot/onboard_device.html` & `slurpit_nautobot-0.8.75/src/slurpit_nautobot/templates/slurpit_nautobot/onboard_device.html`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.74/src/slurpit_nautobot/templates/slurpit_nautobot/planning_table.html` & `slurpit_nautobot-0.8.75/src/slurpit_nautobot/templates/slurpit_nautobot/planning_table.html`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 <!-- example_plugin/tab_device_detail_1.html -->
 {% extends 'dcim/device/base.html' %}
 {% load static %}
 {% load form_helpers %}
 {% load i18n %}
+{% load helpers %}
+{% load plugins %}
 
 {% block content %}
 <div class="row px-3">
     <div class="col col-12 py-3 mx-auto px-0 plan-filter">
       <form action="" method="get" id="plan-form" class="form form-horizontal">
         <div>
           <div class="col-md-6 d-flex gap-2">
@@ -146,10 +148,26 @@
 <script>
   var form = document.getElementById('plan-form');
   var refreshInput = document.getElementById('refreshInput');
 
   $("#id_planning_id").on('select2:select', function(e){
     form.submit();
   });
+
+  function switch_tab(tab_href, reload=false) {
+
+    let [tab_url, tab_id] = tab_href.split("#")
+
+    if (location.pathname != "{{ object.get_absolute_url }}")
+        window.location.href = `${tab_url}?tab=${tab_id}`;
+    else if (window.history.state["id"] != tab_id){
+        window.history.pushState({id: tab_id}, document.title, `${tab_url}?tab=${tab_id}`);
+    }
+
+    // If set, reload the page after asserting state.
+    reload && window.location.reload();
+
+  }
+
 </script>
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 {% extends 'dcim/device/base.html' %} {% load static %} {% load form_helpers %}
-{% load i18n %} {% block content %}
+{% load i18n %} {% load helpers %} {% load plugins %} {% block content %}
 {% render_form form %}
 Open
 % if "result_type" not in request.GET or request.GET.result_type == 'planning'
 %}selected="selected"{% else %} {% endif %}>{% trans "Planning Result" %}
 % if request.GET.result_type == 'template' %}selected="selected"{% else %} {%
 endif %}>{% trans "Template Result" %}
 {{{{rreessuulltt__ssttaattuuss}}}} rreessuullttss {{%% iiff rreessuulltt__ssttaattuuss ==== ''CCaacchheedd'' %%}} -- RReeffrreesshh ddaattaa {{%%
```

### Comparing `slurpit_nautobot-0.8.74/src/slurpit_nautobot/templates/slurpit_nautobot/settings/data_tabs.html` & `slurpit_nautobot-0.8.75/src/slurpit_nautobot/templates/slurpit_nautobot/settings/data_tabs.html`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.74/src/slurpit_nautobot/templates/slurpit_nautobot/settings/general.html` & `slurpit_nautobot-0.8.75/src/slurpit_nautobot/templates/slurpit_nautobot/settings/general.html`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.74/src/slurpit_nautobot/templates/slurpit_nautobot/settings.html` & `slurpit_nautobot-0.8.75/src/slurpit_nautobot/templates/slurpit_nautobot/settings.html`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.74/src/slurpit_nautobot/templates/slurpit_nautobot/slurpitlog_list.html` & `slurpit_nautobot-0.8.75/src/slurpit_nautobot/templates/slurpit_nautobot/slurpitlog_list.html`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.74/src/slurpit_nautobot/templates/slurpit_nautobot/table.html` & `slurpit_nautobot-0.8.75/src/slurpit_nautobot/templates/slurpit_nautobot/table.html`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.74/src/slurpit_nautobot/urls.py` & `slurpit_nautobot-0.8.75/src/slurpit_nautobot/urls.py`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.74/src/slurpit_nautobot/validator.py` & `slurpit_nautobot-0.8.75/src/slurpit_nautobot/validator.py`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.74/src/slurpit_nautobot/views/datamapping.py` & `slurpit_nautobot-0.8.75/src/slurpit_nautobot/views/datamapping.py`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.74/src/slurpit_nautobot/views/logging.py` & `slurpit_nautobot-0.8.75/src/slurpit_nautobot/views/logging.py`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.74/src/slurpit_nautobot/views/onboarding.py` & `slurpit_nautobot-0.8.75/src/slurpit_nautobot/views/onboarding.py`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.74/src/slurpit_nautobot/views/reconcile.py` & `slurpit_nautobot-0.8.75/src/slurpit_nautobot/views/reconcile.py`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.74/src/slurpit_nautobot/views/setting.py` & `slurpit_nautobot-0.8.75/src/slurpit_nautobot/views/setting.py`

 * *Files identical despite different names*

### Comparing `slurpit_nautobot-0.8.74/PKG-INFO` & `slurpit_nautobot-0.8.75/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slurpit_nautobot
-Version: 0.8.74
+Version: 0.8.75
 Summary: 
 Author: Pieter
 Author-email: pieter@slurpit.io
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```
