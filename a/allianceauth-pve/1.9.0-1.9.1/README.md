# Comparing `tmp/allianceauth_pve-1.9.0.tar.gz` & `tmp/allianceauth_pve-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "allianceauth_pve-1.9.0.tar", last modified: Mon Feb 27 20:02:34 2023, max compression
+gzip compressed data, was "allianceauth_pve-1.9.1.tar", last modified: Mon Feb 27 20:51:31 2023, max compression
```

## Comparing `allianceauth_pve-1.9.0.tar` & `allianceauth_pve-1.9.1.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 20:02:34.099518 allianceauth_pve-1.9.0/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1539 2023-02-27 20:02:24.000000 allianceauth_pve-1.9.0/LICENSE
--rwxr-xr-x   0 runner    (1001) docker     (123)      214 2023-02-27 20:02:24.000000 allianceauth_pve-1.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9446 2023-02-27 20:02:34.099518 allianceauth_pve-1.9.0/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     8273 2023-02-27 20:02:24.000000 allianceauth_pve-1.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 20:02:34.095518 allianceauth_pve-1.9.0/allianceauth_pve/
--rwxr-xr-x   0 runner    (1001) docker     (123)      135 2023-02-27 20:02:24.000000 allianceauth_pve-1.9.0/allianceauth_pve/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2230 2023-02-27 20:02:24.000000 allianceauth_pve-1.9.0/allianceauth_pve/actions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1700 2023-02-27 20:02:24.000000 allianceauth_pve-1.9.0/allianceauth_pve/admin.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      163 2023-02-27 20:02:24.000000 allianceauth_pve-1.9.0/allianceauth_pve/apps.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      739 2023-02-27 20:02:24.000000 allianceauth_pve-1.9.0/allianceauth_pve/auth_hooks.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3618 2023-02-27 20:02:24.000000 allianceauth_pve-1.9.0/allianceauth_pve/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 20:02:34.099518 allianceauth_pve-1.9.0/allianceauth_pve/migrations/
--rwxr-xr-x   0 runner    (1001) docker     (123)     5107 2023-02-27 20:02:24.000000 allianceauth_pve-1.9.0/allianceauth_pve/migrations/0001_initial.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      662 2023-02-27 20:02:24.000000 allianceauth_pve-1.9.0/allianceauth_pve/migrations/0002_auto_20220409_1358.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2560 2023-02-27 20:02:24.000000 allianceauth_pve-1.9.0/allianceauth_pve/migrations/0003_auto_20220411_1104.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      898 2023-02-27 20:02:24.000000 allianceauth_pve-1.9.0/allianceauth_pve/migrations/0004_auto_20220411_2152.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4501 2023-02-27 20:02:24.000000 allianceauth_pve-1.9.0/allianceauth_pve/migrations/0005_rename_character_entrycharacter_user.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1977 2023-02-27 20:02:24.000000 allianceauth_pve-1.9.0/allianceauth_pve/migrations/0006_auto_20220416_1534.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      433 2023-02-27 20:02:24.000000 allianceauth_pve-1.9.0/allianceauth_pve/migrations/0007_alter_rotation_tax_rate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3445 2023-02-27 20:02:24.000000 allianceauth_pve-1.9.0/allianceauth_pve/migrations/0008_auto_20220424_1435.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1791 2023-02-27 20:02:24.000000 allianceauth_pve-1.9.0/allianceauth_pve/migrations/0009_pvebutton_rotation_entry_buttons.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1701 2023-02-27 20:02:24.000000 allianceauth_pve-1.9.0/allianceauth_pve/migrations/0010_rolesetup_generalrole_rotation_roles_setups.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      649 2023-02-27 20:02:24.000000 allianceauth_pve-1.9.0/allianceauth_pve/migrations/0011_entryrole_unique_role_name_per_entry_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)     4842 2023-02-27 20:02:24.000000 allianceauth_pve-1.9.0/allianceauth_pve/migrations/0012_alter_entry_options_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-02-27 20:02:24.000000 allianceauth_pve-1.9.0/allianceauth_pve/migrations/0013_alter_general_options_alter_rotation_entry_buttons_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-02-27 20:02:24.000000 allianceauth_pve-1.9.0/allianceauth_pve/migrations/0014_alter_rotation_priority.py
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-02-27 20:02:24.000000 allianceauth_pve-1.9.0/allianceauth_pve/migrations/0015_alter_entry_estimated_total_alter_pvebutton_amount_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)     3645 2023-02-27 20:02:24.000000 allianceauth_pve-1.9.0/allianceauth_pve/migrations/0016_remove_entrycharacter_actual_share_total_and_more.py
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 20:02:24.000000 allianceauth_pve-1.9.0/allianceauth_pve/migrations/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9308 2023-02-27 20:02:24.000000 allianceauth_pve-1.9.0/allianceauth_pve/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 20:02:34.091518 allianceauth_pve-1.9.0/allianceauth_pve/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 20:02:34.091518 allianceauth_pve-1.9.0/allianceauth_pve/static/allianceauth_pve/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 20:02:34.099518 allianceauth_pve-1.9.0/allianceauth_pve/static/allianceauth_pve/css/
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-02-27 20:02:24.000000 allianceauth_pve-1.9.0/allianceauth_pve/static/allianceauth_pve/css/copy_text.css
--rwxr-xr-x   0 runner    (1001) docker     (123)      303 2023-02-27 20:02:24.000000 allianceauth_pve-1.9.0/allianceauth_pve/static/allianceauth_pve/css/custom_checkbox.css
--rwxr-xr-x   0 runner    (1001) docker     (123)     1054 2023-02-27 20:02:24.000000 allianceauth_pve-1.9.0/allianceauth_pve/static/allianceauth_pve/css/new_entry_styles.css
--rw-r--r--   0 runner    (1001) docker     (123)     6711 2023-02-27 20:02:24.000000 allianceauth_pve-1.9.0/allianceauth_pve/static/allianceauth_pve/css/spop.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 20:02:34.099518 allianceauth_pve-1.9.0/allianceauth_pve/static/allianceauth_pve/js/
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-02-27 20:02:24.000000 allianceauth_pve-1.9.0/allianceauth_pve/static/allianceauth_pve/js/copy_text.js
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-02-27 20:02:24.000000 allianceauth_pve-1.9.0/allianceauth_pve/static/allianceauth_pve/js/localized_checkbox.js
--rwxr-xr-x   0 runner    (1001) docker     (123)    18636 2023-02-27 20:02:24.000000 allianceauth_pve-1.9.0/allianceauth_pve/static/allianceauth_pve/js/new_entry_js.js
--rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-02-27 20:02:24.000000 allianceauth_pve-1.9.0/allianceauth_pve/static/allianceauth_pve/js/spop.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 20:02:34.095518 allianceauth_pve-1.9.0/allianceauth_pve/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 20:02:34.099518 allianceauth_pve-1.9.0/allianceauth_pve/templates/allianceauth_pve/
--rwxr-xr-x   0 runner    (1001) docker     (123)     6940 2023-02-27 20:02:24.000000 allianceauth_pve-1.9.0/allianceauth_pve/templates/allianceauth_pve/entry_detail.html
--rwxr-xr-x   0 runner    (1001) docker     (123)    14905 2023-02-27 20:02:24.000000 allianceauth_pve-1.9.0/allianceauth_pve/templates/allianceauth_pve/entry_form.html
--rwxr-xr-x   0 runner    (1001) docker     (123)    11763 2023-02-27 20:02:24.000000 allianceauth_pve-1.9.0/allianceauth_pve/templates/allianceauth_pve/ratting-dashboard.html
--rwxr-xr-x   0 runner    (1001) docker     (123)    11805 2023-02-27 20:02:24.000000 allianceauth_pve-1.9.0/allianceauth_pve/templates/allianceauth_pve/rotation.html
--rwxr-xr-x   0 runner    (1001) docker     (123)      760 2023-02-27 20:02:24.000000 allianceauth_pve-1.9.0/allianceauth_pve/templates/allianceauth_pve/rotation_create.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 20:02:34.099518 allianceauth_pve-1.9.0/allianceauth_pve/templatetags/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 20:02:24.000000 allianceauth_pve-1.9.0/allianceauth_pve/templatetags/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      532 2023-02-27 20:02:24.000000 allianceauth_pve-1.9.0/allianceauth_pve/templatetags/allianceauth_pve_versioned_static.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1088 2023-02-27 20:02:24.000000 allianceauth_pve-1.9.0/allianceauth_pve/templatetags/pvefilters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 20:02:34.099518 allianceauth_pve-1.9.0/allianceauth_pve/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-27 20:02:24.000000 allianceauth_pve-1.9.0/allianceauth_pve/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-02-27 20:02:24.000000 allianceauth_pve-1.9.0/allianceauth_pve/tests/test_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-02-27 20:02:24.000000 allianceauth_pve-1.9.0/allianceauth_pve/tests/test_admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-02-27 20:02:24.000000 allianceauth_pve-1.9.0/allianceauth_pve/tests/test_auth_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     7973 2023-02-27 20:02:24.000000 allianceauth_pve-1.9.0/allianceauth_pve/tests/test_forms.py
--rw-r--r--   0 runner    (1001) docker     (123)    10073 2023-02-27 20:02:24.000000 allianceauth_pve-1.9.0/allianceauth_pve/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3766 2023-02-27 20:02:24.000000 allianceauth_pve-1.9.0/allianceauth_pve/tests/test_templatetags.py
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-02-27 20:02:24.000000 allianceauth_pve-1.9.0/allianceauth_pve/tests/test_urls.py
--rw-r--r--   0 runner    (1001) docker     (123)    27954 2023-02-27 20:02:24.000000 allianceauth_pve-1.9.0/allianceauth_pve/tests/test_views.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      864 2023-02-27 20:02:24.000000 allianceauth_pve-1.9.0/allianceauth_pve/urls.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13194 2023-02-27 20:02:24.000000 allianceauth_pve-1.9.0/allianceauth_pve/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 20:02:34.095518 allianceauth_pve-1.9.0/allianceauth_pve.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9446 2023-02-27 20:02:34.000000 allianceauth_pve-1.9.0/allianceauth_pve.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-02-27 20:02:34.000000 allianceauth_pve-1.9.0/allianceauth_pve.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-27 20:02:34.000000 allianceauth_pve-1.9.0/allianceauth_pve.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-27 20:02:33.000000 allianceauth_pve-1.9.0/allianceauth_pve.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-27 20:02:34.000000 allianceauth_pve-1.9.0/allianceauth_pve.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-02-27 20:02:34.000000 allianceauth_pve-1.9.0/allianceauth_pve.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)      104 2023-02-27 20:02:24.000000 allianceauth_pve-1.9.0/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1552 2023-02-27 20:02:34.103518 allianceauth_pve-1.9.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 20:51:31.118242 allianceauth_pve-1.9.1/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1539 2023-02-27 20:51:21.000000 allianceauth_pve-1.9.1/LICENSE
+-rwxr-xr-x   0 runner    (1001) docker     (123)      214 2023-02-27 20:51:21.000000 allianceauth_pve-1.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9446 2023-02-27 20:51:31.118242 allianceauth_pve-1.9.1/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8273 2023-02-27 20:51:21.000000 allianceauth_pve-1.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 20:51:31.110242 allianceauth_pve-1.9.1/allianceauth_pve/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      135 2023-02-27 20:51:21.000000 allianceauth_pve-1.9.1/allianceauth_pve/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2230 2023-02-27 20:51:21.000000 allianceauth_pve-1.9.1/allianceauth_pve/actions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1700 2023-02-27 20:51:21.000000 allianceauth_pve-1.9.1/allianceauth_pve/admin.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      163 2023-02-27 20:51:21.000000 allianceauth_pve-1.9.1/allianceauth_pve/apps.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      739 2023-02-27 20:51:21.000000 allianceauth_pve-1.9.1/allianceauth_pve/auth_hooks.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3618 2023-02-27 20:51:21.000000 allianceauth_pve-1.9.1/allianceauth_pve/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 20:51:31.114242 allianceauth_pve-1.9.1/allianceauth_pve/migrations/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5107 2023-02-27 20:51:21.000000 allianceauth_pve-1.9.1/allianceauth_pve/migrations/0001_initial.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      662 2023-02-27 20:51:21.000000 allianceauth_pve-1.9.1/allianceauth_pve/migrations/0002_auto_20220409_1358.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2560 2023-02-27 20:51:21.000000 allianceauth_pve-1.9.1/allianceauth_pve/migrations/0003_auto_20220411_1104.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      898 2023-02-27 20:51:21.000000 allianceauth_pve-1.9.1/allianceauth_pve/migrations/0004_auto_20220411_2152.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4501 2023-02-27 20:51:21.000000 allianceauth_pve-1.9.1/allianceauth_pve/migrations/0005_rename_character_entrycharacter_user.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1977 2023-02-27 20:51:21.000000 allianceauth_pve-1.9.1/allianceauth_pve/migrations/0006_auto_20220416_1534.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      433 2023-02-27 20:51:21.000000 allianceauth_pve-1.9.1/allianceauth_pve/migrations/0007_alter_rotation_tax_rate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3445 2023-02-27 20:51:21.000000 allianceauth_pve-1.9.1/allianceauth_pve/migrations/0008_auto_20220424_1435.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1791 2023-02-27 20:51:21.000000 allianceauth_pve-1.9.1/allianceauth_pve/migrations/0009_pvebutton_rotation_entry_buttons.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1701 2023-02-27 20:51:21.000000 allianceauth_pve-1.9.1/allianceauth_pve/migrations/0010_rolesetup_generalrole_rotation_roles_setups.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      649 2023-02-27 20:51:21.000000 allianceauth_pve-1.9.1/allianceauth_pve/migrations/0011_entryrole_unique_role_name_per_entry_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4842 2023-02-27 20:51:21.000000 allianceauth_pve-1.9.1/allianceauth_pve/migrations/0012_alter_entry_options_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-02-27 20:51:21.000000 allianceauth_pve-1.9.1/allianceauth_pve/migrations/0013_alter_general_options_alter_rotation_entry_buttons_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-02-27 20:51:21.000000 allianceauth_pve-1.9.1/allianceauth_pve/migrations/0014_alter_rotation_priority.py
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-02-27 20:51:21.000000 allianceauth_pve-1.9.1/allianceauth_pve/migrations/0015_alter_entry_estimated_total_alter_pvebutton_amount_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3645 2023-02-27 20:51:21.000000 allianceauth_pve-1.9.1/allianceauth_pve/migrations/0016_remove_entrycharacter_actual_share_total_and_more.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 20:51:21.000000 allianceauth_pve-1.9.1/allianceauth_pve/migrations/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9308 2023-02-27 20:51:21.000000 allianceauth_pve-1.9.1/allianceauth_pve/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 20:51:31.110242 allianceauth_pve-1.9.1/allianceauth_pve/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 20:51:31.110242 allianceauth_pve-1.9.1/allianceauth_pve/static/allianceauth_pve/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 20:51:31.114242 allianceauth_pve-1.9.1/allianceauth_pve/static/allianceauth_pve/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-02-27 20:51:21.000000 allianceauth_pve-1.9.1/allianceauth_pve/static/allianceauth_pve/css/copy_text.css
+-rwxr-xr-x   0 runner    (1001) docker     (123)      303 2023-02-27 20:51:21.000000 allianceauth_pve-1.9.1/allianceauth_pve/static/allianceauth_pve/css/custom_checkbox.css
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1054 2023-02-27 20:51:21.000000 allianceauth_pve-1.9.1/allianceauth_pve/static/allianceauth_pve/css/new_entry_styles.css
+-rw-r--r--   0 runner    (1001) docker     (123)     6711 2023-02-27 20:51:21.000000 allianceauth_pve-1.9.1/allianceauth_pve/static/allianceauth_pve/css/spop.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 20:51:31.114242 allianceauth_pve-1.9.1/allianceauth_pve/static/allianceauth_pve/js/
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-02-27 20:51:21.000000 allianceauth_pve-1.9.1/allianceauth_pve/static/allianceauth_pve/js/copy_text.js
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-02-27 20:51:21.000000 allianceauth_pve-1.9.1/allianceauth_pve/static/allianceauth_pve/js/localized_checkbox.js
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18636 2023-02-27 20:51:21.000000 allianceauth_pve-1.9.1/allianceauth_pve/static/allianceauth_pve/js/new_entry_js.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-02-27 20:51:21.000000 allianceauth_pve-1.9.1/allianceauth_pve/static/allianceauth_pve/js/spop.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 20:51:31.110242 allianceauth_pve-1.9.1/allianceauth_pve/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 20:51:31.114242 allianceauth_pve-1.9.1/allianceauth_pve/templates/allianceauth_pve/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6940 2023-02-27 20:51:21.000000 allianceauth_pve-1.9.1/allianceauth_pve/templates/allianceauth_pve/entry_detail.html
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14905 2023-02-27 20:51:21.000000 allianceauth_pve-1.9.1/allianceauth_pve/templates/allianceauth_pve/entry_form.html
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11763 2023-02-27 20:51:21.000000 allianceauth_pve-1.9.1/allianceauth_pve/templates/allianceauth_pve/ratting-dashboard.html
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11805 2023-02-27 20:51:21.000000 allianceauth_pve-1.9.1/allianceauth_pve/templates/allianceauth_pve/rotation.html
+-rwxr-xr-x   0 runner    (1001) docker     (123)      760 2023-02-27 20:51:21.000000 allianceauth_pve-1.9.1/allianceauth_pve/templates/allianceauth_pve/rotation_create.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 20:51:31.114242 allianceauth_pve-1.9.1/allianceauth_pve/templatetags/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 20:51:21.000000 allianceauth_pve-1.9.1/allianceauth_pve/templatetags/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      532 2023-02-27 20:51:21.000000 allianceauth_pve-1.9.1/allianceauth_pve/templatetags/allianceauth_pve_versioned_static.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1088 2023-02-27 20:51:21.000000 allianceauth_pve-1.9.1/allianceauth_pve/templatetags/pvefilters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 20:51:31.118242 allianceauth_pve-1.9.1/allianceauth_pve/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-27 20:51:21.000000 allianceauth_pve-1.9.1/allianceauth_pve/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-02-27 20:51:21.000000 allianceauth_pve-1.9.1/allianceauth_pve/tests/test_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-02-27 20:51:21.000000 allianceauth_pve-1.9.1/allianceauth_pve/tests/test_admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-02-27 20:51:21.000000 allianceauth_pve-1.9.1/allianceauth_pve/tests/test_auth_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7973 2023-02-27 20:51:21.000000 allianceauth_pve-1.9.1/allianceauth_pve/tests/test_forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10073 2023-02-27 20:51:21.000000 allianceauth_pve-1.9.1/allianceauth_pve/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3766 2023-02-27 20:51:21.000000 allianceauth_pve-1.9.1/allianceauth_pve/tests/test_templatetags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-02-27 20:51:21.000000 allianceauth_pve-1.9.1/allianceauth_pve/tests/test_urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27954 2023-02-27 20:51:21.000000 allianceauth_pve-1.9.1/allianceauth_pve/tests/test_views.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      864 2023-02-27 20:51:21.000000 allianceauth_pve-1.9.1/allianceauth_pve/urls.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13437 2023-02-27 20:51:21.000000 allianceauth_pve-1.9.1/allianceauth_pve/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 20:51:31.114242 allianceauth_pve-1.9.1/allianceauth_pve.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9446 2023-02-27 20:51:31.000000 allianceauth_pve-1.9.1/allianceauth_pve.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-02-27 20:51:31.000000 allianceauth_pve-1.9.1/allianceauth_pve.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-27 20:51:31.000000 allianceauth_pve-1.9.1/allianceauth_pve.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-27 20:51:30.000000 allianceauth_pve-1.9.1/allianceauth_pve.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-27 20:51:31.000000 allianceauth_pve-1.9.1/allianceauth_pve.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-02-27 20:51:31.000000 allianceauth_pve-1.9.1/allianceauth_pve.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      104 2023-02-27 20:51:21.000000 allianceauth_pve-1.9.1/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1552 2023-02-27 20:51:31.118242 allianceauth_pve-1.9.1/setup.cfg
```

### Comparing `allianceauth_pve-1.9.0/LICENSE` & `allianceauth_pve-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `allianceauth_pve-1.9.0/PKG-INFO` & `allianceauth_pve-1.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: allianceauth_pve
-Version: 1.9.0
+Version: 1.9.1
 Summary: PvE tool for AllianceAuth
 Home-page: https://github.com/Maestro-Zacht/allianceauth-pve
 Author-email: matteo.ghia@yahoo.it
 License: GNU General Public License v3
 Keywords: allianceauth_pve,allianceauth,eveonline
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

### Comparing `allianceauth_pve-1.9.0/README.md` & `allianceauth_pve-1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `allianceauth_pve-1.9.0/allianceauth_pve/actions.py` & `allianceauth_pve-1.9.1/allianceauth_pve/actions.py`

 * *Files identical despite different names*

### Comparing `allianceauth_pve-1.9.0/allianceauth_pve/admin.py` & `allianceauth_pve-1.9.1/allianceauth_pve/admin.py`

 * *Files identical despite different names*

### Comparing `allianceauth_pve-1.9.0/allianceauth_pve/auth_hooks.py` & `allianceauth_pve-1.9.1/allianceauth_pve/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `allianceauth_pve-1.9.0/allianceauth_pve/forms.py` & `allianceauth_pve-1.9.1/allianceauth_pve/forms.py`

 * *Files identical despite different names*

### Comparing `allianceauth_pve-1.9.0/allianceauth_pve/migrations/0001_initial.py` & `allianceauth_pve-1.9.1/allianceauth_pve/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `allianceauth_pve-1.9.0/allianceauth_pve/migrations/0002_auto_20220409_1358.py` & `allianceauth_pve-1.9.1/allianceauth_pve/migrations/0002_auto_20220409_1358.py`

 * *Files identical despite different names*

### Comparing `allianceauth_pve-1.9.0/allianceauth_pve/migrations/0003_auto_20220411_1104.py` & `allianceauth_pve-1.9.1/allianceauth_pve/migrations/0003_auto_20220411_1104.py`

 * *Files identical despite different names*

### Comparing `allianceauth_pve-1.9.0/allianceauth_pve/migrations/0004_auto_20220411_2152.py` & `allianceauth_pve-1.9.1/allianceauth_pve/migrations/0004_auto_20220411_2152.py`

 * *Files identical despite different names*

### Comparing `allianceauth_pve-1.9.0/allianceauth_pve/migrations/0005_rename_character_entrycharacter_user.py` & `allianceauth_pve-1.9.1/allianceauth_pve/migrations/0005_rename_character_entrycharacter_user.py`

 * *Files identical despite different names*

### Comparing `allianceauth_pve-1.9.0/allianceauth_pve/migrations/0006_auto_20220416_1534.py` & `allianceauth_pve-1.9.1/allianceauth_pve/migrations/0006_auto_20220416_1534.py`

 * *Files identical despite different names*

### Comparing `allianceauth_pve-1.9.0/allianceauth_pve/migrations/0008_auto_20220424_1435.py` & `allianceauth_pve-1.9.1/allianceauth_pve/migrations/0008_auto_20220424_1435.py`

 * *Files identical despite different names*

### Comparing `allianceauth_pve-1.9.0/allianceauth_pve/migrations/0009_pvebutton_rotation_entry_buttons.py` & `allianceauth_pve-1.9.1/allianceauth_pve/migrations/0009_pvebutton_rotation_entry_buttons.py`

 * *Files identical despite different names*

### Comparing `allianceauth_pve-1.9.0/allianceauth_pve/migrations/0010_rolesetup_generalrole_rotation_roles_setups.py` & `allianceauth_pve-1.9.1/allianceauth_pve/migrations/0010_rolesetup_generalrole_rotation_roles_setups.py`

 * *Files identical despite different names*

### Comparing `allianceauth_pve-1.9.0/allianceauth_pve/migrations/0011_entryrole_unique_role_name_per_entry_and_more.py` & `allianceauth_pve-1.9.1/allianceauth_pve/migrations/0011_entryrole_unique_role_name_per_entry_and_more.py`

 * *Files identical despite different names*

### Comparing `allianceauth_pve-1.9.0/allianceauth_pve/migrations/0012_alter_entry_options_and_more.py` & `allianceauth_pve-1.9.1/allianceauth_pve/migrations/0012_alter_entry_options_and_more.py`

 * *Files identical despite different names*

### Comparing `allianceauth_pve-1.9.0/allianceauth_pve/migrations/0013_alter_general_options_alter_rotation_entry_buttons_and_more.py` & `allianceauth_pve-1.9.1/allianceauth_pve/migrations/0013_alter_general_options_alter_rotation_entry_buttons_and_more.py`

 * *Files identical despite different names*

### Comparing `allianceauth_pve-1.9.0/allianceauth_pve/migrations/0014_alter_rotation_priority.py` & `allianceauth_pve-1.9.1/allianceauth_pve/migrations/0014_alter_rotation_priority.py`

 * *Files identical despite different names*

### Comparing `allianceauth_pve-1.9.0/allianceauth_pve/migrations/0015_alter_entry_estimated_total_alter_pvebutton_amount_and_more.py` & `allianceauth_pve-1.9.1/allianceauth_pve/migrations/0015_alter_entry_estimated_total_alter_pvebutton_amount_and_more.py`

 * *Files identical despite different names*

### Comparing `allianceauth_pve-1.9.0/allianceauth_pve/migrations/0016_remove_entrycharacter_actual_share_total_and_more.py` & `allianceauth_pve-1.9.1/allianceauth_pve/migrations/0016_remove_entrycharacter_actual_share_total_and_more.py`

 * *Files identical despite different names*

### Comparing `allianceauth_pve-1.9.0/allianceauth_pve/models.py` & `allianceauth_pve-1.9.1/allianceauth_pve/models.py`

 * *Files identical despite different names*

### Comparing `allianceauth_pve-1.9.0/allianceauth_pve/static/allianceauth_pve/css/new_entry_styles.css` & `allianceauth_pve-1.9.1/allianceauth_pve/static/allianceauth_pve/css/new_entry_styles.css`

 * *Files identical despite different names*

### Comparing `allianceauth_pve-1.9.0/allianceauth_pve/static/allianceauth_pve/css/spop.css` & `allianceauth_pve-1.9.1/allianceauth_pve/static/allianceauth_pve/css/spop.css`

 * *Files identical despite different names*

### Comparing `allianceauth_pve-1.9.0/allianceauth_pve/static/allianceauth_pve/js/copy_text.js` & `allianceauth_pve-1.9.1/allianceauth_pve/static/allianceauth_pve/js/copy_text.js`

 * *Files identical despite different names*

### Comparing `allianceauth_pve-1.9.0/allianceauth_pve/static/allianceauth_pve/js/new_entry_js.js` & `allianceauth_pve-1.9.1/allianceauth_pve/static/allianceauth_pve/js/new_entry_js.js`

 * *Files identical despite different names*

### Comparing `allianceauth_pve-1.9.0/allianceauth_pve/static/allianceauth_pve/js/spop.js` & `allianceauth_pve-1.9.1/allianceauth_pve/static/allianceauth_pve/js/spop.js`

 * *Files identical despite different names*

### Comparing `allianceauth_pve-1.9.0/allianceauth_pve/templates/allianceauth_pve/entry_detail.html` & `allianceauth_pve-1.9.1/allianceauth_pve/templates/allianceauth_pve/entry_detail.html`

 * *Files identical despite different names*

### Comparing `allianceauth_pve-1.9.0/allianceauth_pve/templates/allianceauth_pve/entry_form.html` & `allianceauth_pve-1.9.1/allianceauth_pve/templates/allianceauth_pve/entry_form.html`

 * *Files identical despite different names*

### Comparing `allianceauth_pve-1.9.0/allianceauth_pve/templates/allianceauth_pve/ratting-dashboard.html` & `allianceauth_pve-1.9.1/allianceauth_pve/templates/allianceauth_pve/ratting-dashboard.html`

 * *Files 1% similar despite different names*

```diff
@@ -96,15 +96,15 @@
                                     </thead>
 
                                     <tbody>
                                         {% for rotation in open_rots %}
                                             <tr>
                                                 <td style="width: 25%;"><a href="{% url 'allianceauth_pve:rotation_view' rotation.pk %}">{{ rotation.name }}</a></td>
                                                 <td style="width: 25%;">{{ rotation.days_since }}</td>
-                                                <td style="width: 25%;">{{ rotation.summary.count }}</td>
+                                                <td style="width: 25%;">{{ rotation.summary_count }}</td>
                                                 <td style="width: 25%;">{{ rotation.estimated_total|floatformat|intcomma }}</td>
                                             </tr>
                                         {% endfor %}
                                     </tbody>
                                 </table>
                             </div>
                         {% else %}
@@ -158,15 +158,15 @@
                                     </thead>
 
                                     <tbody>
                                         {% for rotation in closed_rots %}
                                             <tr>
                                                 <td style="width: 25%;"><a href="{% url 'allianceauth_pve:rotation_view' rotation.pk %}">{{ rotation.pk }} - {{ rotation.name }}</a></td>
                                                 <td style="width: 25%;">{{ rotation.closed_at }}</td>
-                                                <td style="width: 25%;">{{ rotation.summary.count }}</td>
+                                                <td style="width: 25%;">{{ rotation.summary_count }}</td>
                                                 <td style="width: 25%;">{{ rotation.actual_total|floatformat|intcomma }}</td>
                                             </tr>
                                         {% endfor %}
                                     </tbody>
                                 </table>
                             </div>
                         {% else %}
```

#### html2text {}

```diff
@@ -38,15 +38,15 @@
     * {% endif %} _C_l_o_s_e_d_ _R_o_t_a_t_i_o_n_s
 {% if is_closed_param %}
 {% else %}
 {% endif %} {% if open_count > 0 %}
 NNaammee          AAggee ((ddaayyss))          PPaarrttiicciippaannttss           CCuurrrreenntt TToottaall
 _{             {                   {                      {
 _{             {                   {                      {
-_r_o_t_a_t_i_o_n_._n_a_m_e rotation.days_since rotation.summary.count rotation.estimated_total|floatformat|intcomma
+_r_o_t_a_t_i_o_n_._n_a_m_e rotation.days_since rotation.summary_count rotation.estimated_total|floatformat|intcomma
 _}_}            }}                  }}                     }}
 {% else %}
 No open rotations
 {% endif %} {% if open_rots.paginator.num_pages > 1 %}
     * {% if open_rots.has_previous %}
     * _«
     * _1
@@ -69,15 +69,15 @@
 {% if is_closed_param %}
 {% else %}
 {% endif %} {% if closed_rots.paginator.count > 0 %}
 NNaammee          CClloosseedd OOnn          PPaarrttiicciippaannttss           TToottaall
 _{
 _{_ _r_o_t_a_t_i_o_n_._p_k {                  {                      {
 _}_}_ _-_ _{        {                  {                      {
-_{             rotation.closed_at rotation.summary.count rotation.actual_total|floatformat|intcomma
+_{             rotation.closed_at rotation.summary_count rotation.actual_total|floatformat|intcomma
 _r_o_t_a_t_i_o_n_._n_a_m_e }}                 }}                     }}
 _}_}
 {% else %}
 No open rotations
 {% endif %} {% if closed_rots.paginator.num_pages > 1 %}
     * {% if closed_rots.has_previous %}
     * _«
```

### Comparing `allianceauth_pve-1.9.0/allianceauth_pve/templates/allianceauth_pve/rotation.html` & `allianceauth_pve-1.9.1/allianceauth_pve/templates/allianceauth_pve/rotation.html`

 * *Files identical despite different names*

### Comparing `allianceauth_pve-1.9.0/allianceauth_pve/templates/allianceauth_pve/rotation_create.html` & `allianceauth_pve-1.9.1/allianceauth_pve/templates/allianceauth_pve/rotation_create.html`

 * *Files identical despite different names*

### Comparing `allianceauth_pve-1.9.0/allianceauth_pve/templatetags/allianceauth_pve_versioned_static.py` & `allianceauth_pve-1.9.1/allianceauth_pve/templatetags/allianceauth_pve_versioned_static.py`

 * *Files identical despite different names*

### Comparing `allianceauth_pve-1.9.0/allianceauth_pve/templatetags/pvefilters.py` & `allianceauth_pve-1.9.1/allianceauth_pve/templatetags/pvefilters.py`

 * *Files identical despite different names*

### Comparing `allianceauth_pve-1.9.0/allianceauth_pve/tests/test_actions.py` & `allianceauth_pve-1.9.1/allianceauth_pve/tests/test_actions.py`

 * *Files identical despite different names*

### Comparing `allianceauth_pve-1.9.0/allianceauth_pve/tests/test_admin.py` & `allianceauth_pve-1.9.1/allianceauth_pve/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `allianceauth_pve-1.9.0/allianceauth_pve/tests/test_auth_hooks.py` & `allianceauth_pve-1.9.1/allianceauth_pve/tests/test_auth_hooks.py`

 * *Files identical despite different names*

### Comparing `allianceauth_pve-1.9.0/allianceauth_pve/tests/test_forms.py` & `allianceauth_pve-1.9.1/allianceauth_pve/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `allianceauth_pve-1.9.0/allianceauth_pve/tests/test_models.py` & `allianceauth_pve-1.9.1/allianceauth_pve/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `allianceauth_pve-1.9.0/allianceauth_pve/tests/test_templatetags.py` & `allianceauth_pve-1.9.1/allianceauth_pve/tests/test_templatetags.py`

 * *Files identical despite different names*

### Comparing `allianceauth_pve-1.9.0/allianceauth_pve/tests/test_urls.py` & `allianceauth_pve-1.9.1/allianceauth_pve/tests/test_urls.py`

 * *Files identical despite different names*

### Comparing `allianceauth_pve-1.9.0/allianceauth_pve/tests/test_views.py` & `allianceauth_pve-1.9.1/allianceauth_pve/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `allianceauth_pve-1.9.0/allianceauth_pve/urls.py` & `allianceauth_pve-1.9.1/allianceauth_pve/urls.py`

 * *Files identical despite different names*

### Comparing `allianceauth_pve-1.9.0/allianceauth_pve/views.py` & `allianceauth_pve-1.9.1/allianceauth_pve/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,16 +33,27 @@
 def index(request):
     return redirect('allianceauth_pve:dashboard')
 
 
 @login_required
 @permission_required('allianceauth_pve.access_pve')
 def dashboard(request):
-    open_rots = Rotation.objects.filter(is_closed=False).order_by('-priority')
-    closed_rots = Rotation.objects.filter(is_closed=True).order_by('-closed_at')
+    open_rots = (
+        Rotation.objects
+        .annotate(summary_count=Count('entries__ratting_shares__user', distinct=True))
+        .filter(is_closed=False)
+        .order_by('-priority')
+    )
+
+    closed_rots = (
+        Rotation.objects
+        .annotate(summary_count=Count('entries__ratting_shares__user', distinct=True))
+        .filter(is_closed=True)
+        .order_by('-closed_at')
+    )
 
     paginator_open = Paginator(open_rots, 10)
     paginator_closed = Paginator(closed_rots, 10)
 
     npage_open = request.GET.get('page_open')
     npage_closed = request.GET.get('page_closed')
```

### Comparing `allianceauth_pve-1.9.0/allianceauth_pve.egg-info/PKG-INFO` & `allianceauth_pve-1.9.1/allianceauth_pve.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: allianceauth-pve
-Version: 1.9.0
+Version: 1.9.1
 Summary: PvE tool for AllianceAuth
 Home-page: https://github.com/Maestro-Zacht/allianceauth-pve
 Author-email: matteo.ghia@yahoo.it
 License: GNU General Public License v3
 Keywords: allianceauth_pve,allianceauth,eveonline
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

### Comparing `allianceauth_pve-1.9.0/allianceauth_pve.egg-info/SOURCES.txt` & `allianceauth_pve-1.9.1/allianceauth_pve.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `allianceauth_pve-1.9.0/setup.cfg` & `allianceauth_pve-1.9.1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 1.9.0
+current_version = 1.9.1
 commit = True
 tag = True
 sign_tags = True
 
 [metadata]
 name = allianceauth_pve
 version = attr: allianceauth_pve.__version__
```

