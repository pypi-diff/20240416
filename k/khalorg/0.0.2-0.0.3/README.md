# Comparing `tmp/khalorg-0.0.2.tar.gz` & `tmp/khalorg-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "khalorg-0.0.2.tar", last modified: Mon Apr 15 19:50:24 2024, max compression
+gzip compressed data, was "khalorg-0.0.3.tar", last modified: Tue Apr 16 10:40:36 2024, max compression
```

## Comparing `khalorg-0.0.2.tar` & `khalorg-0.0.3.tar`

### file list

```diff
@@ -1,117 +1,117 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:50:24.790639 khalorg-0.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:50:24.762639 khalorg-0.0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:50:24.762639 khalorg-0.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-15 19:50:14.000000 khalorg-0.0.2/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-15 19:50:14.000000 khalorg-0.0.2/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-15 19:50:14.000000 khalorg-0.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-04-15 19:50:14.000000 khalorg-0.0.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-15 19:50:14.000000 khalorg-0.0.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-15 19:50:14.000000 khalorg-0.0.2/LICENCE
--rw-r--r--   0 runner    (1001) docker     (127)    15923 2024-04-15 19:50:24.790639 khalorg-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15226 2024-04-15 19:50:14.000000 khalorg-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:50:24.774639 khalorg-0.0.2/demo/
--rw-r--r--   0 runner    (1001) docker     (127)   474334 2024-04-15 19:50:14.000000 khalorg-0.0.2/demo/delete.gif
--rw-r--r--   0 runner    (1001) docker     (127)   814156 2024-04-15 19:50:14.000000 khalorg-0.0.2/demo/edit.gif
--rw-r--r--   0 runner    (1001) docker     (127)   805028 2024-04-15 19:50:14.000000 khalorg-0.0.2/demo/list.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)    40467 2024-04-15 19:50:14.000000 khalorg-0.0.2/demo/logo.jpg
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-15 19:50:14.000000 khalorg-0.0.2/demo/meeting.org
--rw-r--r--   0 runner    (1001) docker     (127)  5848880 2024-04-15 19:50:14.000000 khalorg-0.0.2/demo/neovim-plugin.gif
--rw-r--r--   0 runner    (1001) docker     (127)   330668 2024-04-15 19:50:14.000000 khalorg-0.0.2/demo/new.gif
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:50:24.774639 khalorg-0.0.2/extras/
--rwxr-xr-x   0 runner    (1001) docker     (127)     4045 2024-04-15 19:50:14.000000 khalorg-0.0.2/extras/calsync
--rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-04-15 19:50:14.000000 khalorg-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 19:50:24.790639 khalorg-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-15 19:50:14.000000 khalorg-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:50:24.762639 khalorg-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:50:24.774639 khalorg-0.0.2/src/khalorg/
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-15 19:50:14.000000 khalorg-0.0.2/src/khalorg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-15 19:50:14.000000 khalorg-0.0.2/src/khalorg/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3476 2024-04-15 19:50:14.000000 khalorg-0.0.2/src/khalorg/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     6355 2024-04-15 19:50:14.000000 khalorg-0.0.2/src/khalorg/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-15 19:50:14.000000 khalorg-0.0.2/src/khalorg/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:50:24.778639 khalorg-0.0.2/src/khalorg/khal/
--rw-r--r--   0 runner    (1001) docker     (127)     7701 2024-04-15 19:50:14.000000 khalorg-0.0.2/src/khalorg/khal/args.py
--rw-r--r--   0 runner    (1001) docker     (127)    10108 2024-04-15 19:50:14.000000 khalorg-0.0.2/src/khalorg/khal/calendar.py
--rw-r--r--   0 runner    (1001) docker     (127)     4823 2024-04-15 19:50:14.000000 khalorg-0.0.2/src/khalorg/khal/checker.py
--rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-04-15 19:50:14.000000 khalorg-0.0.2/src/khalorg/khal/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:50:24.778639 khalorg-0.0.2/src/khalorg/org/
--rw-r--r--   0 runner    (1001) docker     (127)    19368 2024-04-15 19:50:14.000000 khalorg-0.0.2/src/khalorg/org/agenda_items.py
--rw-r--r--   0 runner    (1001) docker     (127)     2461 2024-04-15 19:50:14.000000 khalorg-0.0.2/src/khalorg/org/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-15 19:50:14.000000 khalorg-0.0.2/src/khalorg/paths.py
--rw-r--r--   0 runner    (1001) docker     (127)     8429 2024-04-15 19:50:14.000000 khalorg-0.0.2/src/khalorg/rrule.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:50:24.778639 khalorg-0.0.2/src/khalorg/static/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 19:50:14.000000 khalorg-0.0.2/src/khalorg/static/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-15 19:50:14.000000 khalorg-0.0.2/src/khalorg/static/description_delete_command.txt
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-15 19:50:14.000000 khalorg-0.0.2/src/khalorg/static/description_edit_command.txt
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-15 19:50:14.000000 khalorg-0.0.2/src/khalorg/static/description_list_command.txt
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-15 19:50:14.000000 khalorg-0.0.2/src/khalorg/static/description_new_command.txt
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-15 19:50:14.000000 khalorg-0.0.2/src/khalorg/static/khal_format.txt
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-15 19:50:14.000000 khalorg-0.0.2/src/khalorg/static/khalorg_format.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:50:24.786639 khalorg-0.0.2/src/khalorg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15923 2024-04-15 19:50:24.000000 khalorg-0.0.2/src/khalorg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-04-15 19:50:24.000000 khalorg-0.0.2/src/khalorg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 19:50:24.000000 khalorg-0.0.2/src/khalorg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-15 19:50:24.000000 khalorg-0.0.2/src/khalorg.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-15 19:50:24.000000 khalorg-0.0.2/src/khalorg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-15 19:50:24.000000 khalorg-0.0.2/src/khalorg.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:50:24.778639 khalorg-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 19:50:14.000000 khalorg-0.0.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5000 2024-04-15 19:50:14.000000 khalorg-0.0.2/tests/agenda_items.py
--rw-r--r--   0 runner    (1001) docker     (127)    12803 2024-04-15 19:50:14.000000 khalorg-0.0.2/tests/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-15 19:50:14.000000 khalorg-0.0.2/tests/khalorg_tester
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:50:24.782639 khalorg-0.0.2/tests/static/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 19:50:14.000000 khalorg-0.0.2/tests/static/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:50:24.786639 khalorg-0.0.2/tests/static/agenda_items/
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-15 19:50:14.000000 khalorg-0.0.2/tests/static/agenda_items/all_day.org
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-15 19:50:14.000000 khalorg-0.0.2/tests/static/agenda_items/all_day_until_with_time.org
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-15 19:50:14.000000 khalorg-0.0.2/tests/static/agenda_items/body_first.org
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-15 19:50:14.000000 khalorg-0.0.2/tests/static/agenda_items/demo.org
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-15 19:50:14.000000 khalorg-0.0.2/tests/static/agenda_items/duplicate.org
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-15 19:50:14.000000 khalorg-0.0.2/tests/static/agenda_items/minimal.org
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-15 19:50:14.000000 khalorg-0.0.2/tests/static/agenda_items/multiple_timestamps.org
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-15 19:50:14.000000 khalorg-0.0.2/tests/static/agenda_items/multiple_timestamps_unsorted.org
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-15 19:50:14.000000 khalorg-0.0.2/tests/static/agenda_items/no_heading.org
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-15 19:50:14.000000 khalorg-0.0.2/tests/static/agenda_items/no_time_stamp.org
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-15 19:50:14.000000 khalorg-0.0.2/tests/static/agenda_items/not_first_child.org
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-15 19:50:14.000000 khalorg-0.0.2/tests/static/agenda_items/not_first_heading.org
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-15 19:50:14.000000 khalorg-0.0.2/tests/static/agenda_items/not_first_level.org
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-15 19:50:14.000000 khalorg-0.0.2/tests/static/agenda_items/past.org
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-15 19:50:14.000000 khalorg-0.0.2/tests/static/agenda_items/recurring.org
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-15 19:50:14.000000 khalorg-0.0.2/tests/static/agenda_items/recurring_allday.org
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-15 19:50:14.000000 khalorg-0.0.2/tests/static/agenda_items/recurring_and_non_recurring.org
--rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-04-15 19:50:14.000000 khalorg-0.0.2/tests/static/agenda_items/recurring_first_item_moved.org
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-15 19:50:14.000000 khalorg-0.0.2/tests/static/agenda_items/recurring_first_item_moved_expected.org
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-15 19:50:14.000000 khalorg-0.0.2/tests/static/agenda_items/recurring_monthly.org
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-15 19:50:14.000000 khalorg-0.0.2/tests/static/agenda_items/recurring_not_supported.org
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-15 19:50:14.000000 khalorg-0.0.2/tests/static/agenda_items/rrule_recurring.org
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-15 19:50:14.000000 khalorg-0.0.2/tests/static/agenda_items/rrule_recurring_1th.org
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-15 19:50:14.000000 khalorg-0.0.2/tests/static/agenda_items/rrule_recurring_allday.org
--rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-04-15 19:50:14.000000 khalorg-0.0.2/tests/static/agenda_items/rrule_recurring_and_non_recurring.org
--rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-04-15 19:50:14.000000 khalorg-0.0.2/tests/static/agenda_items/rrule_recurring_duplicates.org
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-15 19:50:14.000000 khalorg-0.0.2/tests/static/agenda_items/rrule_recurring_monthly.org
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-15 19:50:14.000000 khalorg-0.0.2/tests/static/agenda_items/rrule_recurring_not_supported.org
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-15 19:50:14.000000 khalorg-0.0.2/tests/static/agenda_items/scheduled_and_deadline.org
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-15 19:50:14.000000 khalorg-0.0.2/tests/static/agenda_items/short_timestamp.org
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 19:50:14.000000 khalorg-0.0.2/tests/static/agenda_items/timestamp_scheduled_deadline.org
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-15 19:50:14.000000 khalorg-0.0.2/tests/static/agenda_items/two_items.org
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-15 19:50:14.000000 khalorg-0.0.2/tests/static/agenda_items/two_timestamps.org
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-15 19:50:14.000000 khalorg-0.0.2/tests/static/agenda_items/valid.org
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-15 19:50:14.000000 khalorg-0.0.2/tests/static/agenda_items/valid_no_until.org
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-15 19:50:14.000000 khalorg-0.0.2/tests/static/config_template.txt
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-15 19:50:14.000000 khalorg-0.0.2/tests/static/khalorg_format_full.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-15 19:50:14.000000 khalorg-0.0.2/tests/static/test_config_combined.ini
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-15 19:50:14.000000 khalorg-0.0.2/tests/static/test_config_default.ini
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-04-15 19:50:14.000000 khalorg-0.0.2/tests/static/test_config_khal
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-15 19:50:14.000000 khalorg-0.0.2/tests/static/test_config_user.ini
--rw-r--r--   0 runner    (1001) docker     (127)     4160 2024-04-15 19:50:14.000000 khalorg-0.0.2/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     7828 2024-04-15 19:50:14.000000 khalorg-0.0.2/tests/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-15 19:50:14.000000 khalorg-0.0.2/tests/test_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:50:24.786639 khalorg-0.0.2/tests/test_khal/
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-15 19:50:14.000000 khalorg-0.0.2/tests/test_khal/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5326 2024-04-15 19:50:14.000000 khalorg-0.0.2/tests/test_khal/test_args.py
--rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-04-15 19:50:14.000000 khalorg-0.0.2/tests/test_khal/test_calendar.py
--rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-04-15 19:50:14.000000 khalorg-0.0.2/tests/test_khal/test_checker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:50:24.786639 khalorg-0.0.2/tests/test_org/
--rw-r--r--   0 runner    (1001) docker     (127)     9637 2024-04-15 19:50:14.000000 khalorg-0.0.2/tests/test_org/test_agenda_items.py
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-15 19:50:14.000000 khalorg-0.0.2/tests/test_org/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-04-15 19:50:14.000000 khalorg-0.0.2/tests/test_rrule.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:40:36.693045 khalorg-0.0.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:40:36.661045 khalorg-0.0.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:40:36.665045 khalorg-0.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-16 10:40:25.000000 khalorg-0.0.3/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-16 10:40:25.000000 khalorg-0.0.3/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-16 10:40:25.000000 khalorg-0.0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-04-16 10:40:25.000000 khalorg-0.0.3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-16 10:40:25.000000 khalorg-0.0.3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-16 10:40:25.000000 khalorg-0.0.3/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (127)    15923 2024-04-16 10:40:36.693045 khalorg-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15226 2024-04-16 10:40:25.000000 khalorg-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:40:36.677045 khalorg-0.0.3/demo/
+-rw-r--r--   0 runner    (1001) docker     (127)   474334 2024-04-16 10:40:25.000000 khalorg-0.0.3/demo/delete.gif
+-rw-r--r--   0 runner    (1001) docker     (127)   814156 2024-04-16 10:40:25.000000 khalorg-0.0.3/demo/edit.gif
+-rw-r--r--   0 runner    (1001) docker     (127)   805028 2024-04-16 10:40:25.000000 khalorg-0.0.3/demo/list.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)    40467 2024-04-16 10:40:25.000000 khalorg-0.0.3/demo/logo.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-16 10:40:25.000000 khalorg-0.0.3/demo/meeting.org
+-rw-r--r--   0 runner    (1001) docker     (127)  5848880 2024-04-16 10:40:25.000000 khalorg-0.0.3/demo/neovim-plugin.gif
+-rw-r--r--   0 runner    (1001) docker     (127)   330668 2024-04-16 10:40:25.000000 khalorg-0.0.3/demo/new.gif
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:40:36.677045 khalorg-0.0.3/extras/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4045 2024-04-16 10:40:25.000000 khalorg-0.0.3/extras/calsync
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-04-16 10:40:25.000000 khalorg-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 10:40:36.693045 khalorg-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-16 10:40:25.000000 khalorg-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:40:36.665045 khalorg-0.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:40:36.677045 khalorg-0.0.3/src/khalorg/
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-16 10:40:25.000000 khalorg-0.0.3/src/khalorg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-16 10:40:25.000000 khalorg-0.0.3/src/khalorg/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3476 2024-04-16 10:40:25.000000 khalorg-0.0.3/src/khalorg/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6355 2024-04-16 10:40:25.000000 khalorg-0.0.3/src/khalorg/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-16 10:40:25.000000 khalorg-0.0.3/src/khalorg/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:40:36.681045 khalorg-0.0.3/src/khalorg/khal/
+-rw-r--r--   0 runner    (1001) docker     (127)     7701 2024-04-16 10:40:25.000000 khalorg-0.0.3/src/khalorg/khal/args.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9839 2024-04-16 10:40:25.000000 khalorg-0.0.3/src/khalorg/khal/calendar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4823 2024-04-16 10:40:25.000000 khalorg-0.0.3/src/khalorg/khal/checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3191 2024-04-16 10:40:25.000000 khalorg-0.0.3/src/khalorg/khal/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:40:36.681045 khalorg-0.0.3/src/khalorg/org/
+-rw-r--r--   0 runner    (1001) docker     (127)    19368 2024-04-16 10:40:25.000000 khalorg-0.0.3/src/khalorg/org/agenda_items.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2461 2024-04-16 10:40:25.000000 khalorg-0.0.3/src/khalorg/org/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-16 10:40:25.000000 khalorg-0.0.3/src/khalorg/paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8429 2024-04-16 10:40:25.000000 khalorg-0.0.3/src/khalorg/rrule.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:40:36.681045 khalorg-0.0.3/src/khalorg/static/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 10:40:25.000000 khalorg-0.0.3/src/khalorg/static/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-16 10:40:25.000000 khalorg-0.0.3/src/khalorg/static/description_delete_command.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-16 10:40:25.000000 khalorg-0.0.3/src/khalorg/static/description_edit_command.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-16 10:40:25.000000 khalorg-0.0.3/src/khalorg/static/description_list_command.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-16 10:40:25.000000 khalorg-0.0.3/src/khalorg/static/description_new_command.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-16 10:40:25.000000 khalorg-0.0.3/src/khalorg/static/khal_format.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-16 10:40:25.000000 khalorg-0.0.3/src/khalorg/static/khalorg_format.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:40:36.693045 khalorg-0.0.3/src/khalorg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15923 2024-04-16 10:40:36.000000 khalorg-0.0.3/src/khalorg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-04-16 10:40:36.000000 khalorg-0.0.3/src/khalorg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 10:40:36.000000 khalorg-0.0.3/src/khalorg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-16 10:40:36.000000 khalorg-0.0.3/src/khalorg.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-16 10:40:36.000000 khalorg-0.0.3/src/khalorg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-16 10:40:36.000000 khalorg-0.0.3/src/khalorg.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:40:36.685045 khalorg-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 10:40:25.000000 khalorg-0.0.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5000 2024-04-16 10:40:25.000000 khalorg-0.0.3/tests/agenda_items.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12803 2024-04-16 10:40:25.000000 khalorg-0.0.3/tests/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-16 10:40:25.000000 khalorg-0.0.3/tests/khalorg_tester
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:40:36.685045 khalorg-0.0.3/tests/static/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 10:40:25.000000 khalorg-0.0.3/tests/static/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:40:36.689045 khalorg-0.0.3/tests/static/agenda_items/
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-16 10:40:25.000000 khalorg-0.0.3/tests/static/agenda_items/all_day.org
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-16 10:40:25.000000 khalorg-0.0.3/tests/static/agenda_items/all_day_until_with_time.org
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-16 10:40:25.000000 khalorg-0.0.3/tests/static/agenda_items/body_first.org
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-16 10:40:25.000000 khalorg-0.0.3/tests/static/agenda_items/demo.org
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-16 10:40:25.000000 khalorg-0.0.3/tests/static/agenda_items/duplicate.org
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-16 10:40:25.000000 khalorg-0.0.3/tests/static/agenda_items/minimal.org
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-16 10:40:25.000000 khalorg-0.0.3/tests/static/agenda_items/multiple_timestamps.org
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-16 10:40:25.000000 khalorg-0.0.3/tests/static/agenda_items/multiple_timestamps_unsorted.org
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-16 10:40:25.000000 khalorg-0.0.3/tests/static/agenda_items/no_heading.org
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-16 10:40:25.000000 khalorg-0.0.3/tests/static/agenda_items/no_time_stamp.org
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-16 10:40:25.000000 khalorg-0.0.3/tests/static/agenda_items/not_first_child.org
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-16 10:40:25.000000 khalorg-0.0.3/tests/static/agenda_items/not_first_heading.org
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-16 10:40:25.000000 khalorg-0.0.3/tests/static/agenda_items/not_first_level.org
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-16 10:40:25.000000 khalorg-0.0.3/tests/static/agenda_items/past.org
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-16 10:40:25.000000 khalorg-0.0.3/tests/static/agenda_items/recurring.org
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-16 10:40:25.000000 khalorg-0.0.3/tests/static/agenda_items/recurring_allday.org
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-16 10:40:25.000000 khalorg-0.0.3/tests/static/agenda_items/recurring_and_non_recurring.org
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-04-16 10:40:25.000000 khalorg-0.0.3/tests/static/agenda_items/recurring_first_item_moved.org
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-16 10:40:25.000000 khalorg-0.0.3/tests/static/agenda_items/recurring_first_item_moved_expected.org
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-16 10:40:25.000000 khalorg-0.0.3/tests/static/agenda_items/recurring_monthly.org
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-16 10:40:25.000000 khalorg-0.0.3/tests/static/agenda_items/recurring_not_supported.org
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-16 10:40:25.000000 khalorg-0.0.3/tests/static/agenda_items/rrule_recurring.org
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-16 10:40:25.000000 khalorg-0.0.3/tests/static/agenda_items/rrule_recurring_1th.org
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-16 10:40:25.000000 khalorg-0.0.3/tests/static/agenda_items/rrule_recurring_allday.org
+-rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-04-16 10:40:25.000000 khalorg-0.0.3/tests/static/agenda_items/rrule_recurring_and_non_recurring.org
+-rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-04-16 10:40:25.000000 khalorg-0.0.3/tests/static/agenda_items/rrule_recurring_duplicates.org
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-16 10:40:25.000000 khalorg-0.0.3/tests/static/agenda_items/rrule_recurring_monthly.org
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-16 10:40:25.000000 khalorg-0.0.3/tests/static/agenda_items/rrule_recurring_not_supported.org
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-16 10:40:25.000000 khalorg-0.0.3/tests/static/agenda_items/scheduled_and_deadline.org
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-16 10:40:25.000000 khalorg-0.0.3/tests/static/agenda_items/short_timestamp.org
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 10:40:25.000000 khalorg-0.0.3/tests/static/agenda_items/timestamp_scheduled_deadline.org
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-16 10:40:25.000000 khalorg-0.0.3/tests/static/agenda_items/two_items.org
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-16 10:40:25.000000 khalorg-0.0.3/tests/static/agenda_items/two_timestamps.org
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-16 10:40:25.000000 khalorg-0.0.3/tests/static/agenda_items/valid.org
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-16 10:40:25.000000 khalorg-0.0.3/tests/static/agenda_items/valid_no_until.org
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-16 10:40:25.000000 khalorg-0.0.3/tests/static/config_template.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-16 10:40:25.000000 khalorg-0.0.3/tests/static/khalorg_format_full.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-16 10:40:25.000000 khalorg-0.0.3/tests/static/test_config_combined.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-16 10:40:25.000000 khalorg-0.0.3/tests/static/test_config_default.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-04-16 10:40:25.000000 khalorg-0.0.3/tests/static/test_config_khal
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-16 10:40:25.000000 khalorg-0.0.3/tests/static/test_config_user.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     4160 2024-04-16 10:40:25.000000 khalorg-0.0.3/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7828 2024-04-16 10:40:25.000000 khalorg-0.0.3/tests/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-16 10:40:25.000000 khalorg-0.0.3/tests/test_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:40:36.693045 khalorg-0.0.3/tests/test_khal/
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-16 10:40:25.000000 khalorg-0.0.3/tests/test_khal/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5326 2024-04-16 10:40:25.000000 khalorg-0.0.3/tests/test_khal/test_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-04-16 10:40:25.000000 khalorg-0.0.3/tests/test_khal/test_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-04-16 10:40:25.000000 khalorg-0.0.3/tests/test_khal/test_checker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:40:36.693045 khalorg-0.0.3/tests/test_org/
+-rw-r--r--   0 runner    (1001) docker     (127)     9637 2024-04-16 10:40:25.000000 khalorg-0.0.3/tests/test_org/test_agenda_items.py
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-16 10:40:25.000000 khalorg-0.0.3/tests/test_org/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-04-16 10:40:25.000000 khalorg-0.0.3/tests/test_rrule.py
```

### Comparing `khalorg-0.0.2/.github/workflows/release.yml` & `khalorg-0.0.3/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `khalorg-0.0.2/CHANGELOG.md` & `khalorg-0.0.3/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `khalorg-0.0.2/CONTRIBUTING.md` & `khalorg-0.0.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `khalorg-0.0.2/LICENCE` & `khalorg-0.0.3/LICENCE`

 * *Files identical despite different names*

### Comparing `khalorg-0.0.2/PKG-INFO` & `khalorg-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: khalorg
-Version: 0.0.2
+Version: 0.0.3
 Summary: An interface between Org mode and Khal cli calendar.
 Author: BartSte
 License: MIT License
 Keywords: khal,org mode,vdirsyncer,CalDav,agenda,emacs,neovim,orgmode-nvim
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `khalorg-0.0.2/README.md` & `khalorg-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `khalorg-0.0.2/demo/delete.gif` & `khalorg-0.0.3/demo/delete.gif`

 * *Files identical despite different names*

### Comparing `khalorg-0.0.2/demo/edit.gif` & `khalorg-0.0.3/demo/edit.gif`

 * *Files identical despite different names*

### Comparing `khalorg-0.0.2/demo/list.gif` & `khalorg-0.0.3/demo/list.gif`

 * *Files identical despite different names*

### Comparing `khalorg-0.0.2/demo/logo.jpg` & `khalorg-0.0.3/demo/logo.jpg`

 * *Files identical despite different names*

### Comparing `khalorg-0.0.2/demo/neovim-plugin.gif` & `khalorg-0.0.3/demo/neovim-plugin.gif`

 * *Files identical despite different names*

### Comparing `khalorg-0.0.2/demo/new.gif` & `khalorg-0.0.3/demo/new.gif`

 * *Files identical despite different names*

### Comparing `khalorg-0.0.2/extras/calsync` & `khalorg-0.0.3/extras/calsync`

 * *Files identical despite different names*

### Comparing `khalorg-0.0.2/pyproject.toml` & `khalorg-0.0.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     "Programming Language :: Python :: 3",
 ]
 dependencies = [
     "khal>=0.11",
     "vdirsyncer",
     "orgparse"
 ]
-version = "0.0.2"
+version = "0.0.3"
 
 [project.optional-dependencies]
 debug = ["ipdb", "ipython"]
 test = ["pytest"]
 build = ["build", "twine"]
 
 [project.scripts]
@@ -58,19 +58,16 @@
 
 select = [
     "F",  # pyflakes
     "E",  # pycodestyle errors
     "W",  # pycodestyle warnings
     "I",  # isort
     "N",  # PEP8 naming
-    "D",  # pydocstyle
 ]
 
-ignore = ["D212", "D205", "D210", "D203"]
-
 [tool.autopep8]
 max_line_length = 79
 aggressive = 3
 experimental = true
 
 [tool.pytest.ini_options]
 addopts = "-s -rA --log-level INFO"
```

### Comparing `khalorg-0.0.2/src/khalorg/cli.py` & `khalorg-0.0.3/src/khalorg/cli.py`

 * *Files identical despite different names*

### Comparing `khalorg-0.0.2/src/khalorg/commands.py` & `khalorg-0.0.3/src/khalorg/commands.py`

 * *Files identical despite different names*

### Comparing `khalorg-0.0.2/src/khalorg/helpers.py` & `khalorg-0.0.3/src/khalorg/helpers.py`

 * *Files identical despite different names*

### Comparing `khalorg-0.0.2/src/khalorg/khal/args.py` & `khalorg-0.0.3/src/khalorg/khal/args.py`

 * *Files identical despite different names*

### Comparing `khalorg-0.0.2/src/khalorg/khal/calendar.py` & `khalorg-0.0.3/src/khalorg/khal/calendar.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 import logging
-from os.path import dirname, join
-import sys
 from datetime import date, datetime
 from typing import Callable, Iterable, TypedDict, Union
 
 from khal.cli import build_collection
 from khal.controllers import Event
 from khal.khalendar import CalendarCollection
 from khal.khalendar.vdir import NotFoundError
 from khal.settings.settings import (
     ConfigObj,
     find_configuration_file,
     get_config,
 )
 
 from khalorg.khal.helpers import (
+    find_khal_bin,
     is_future,
     remove_tzinfo,
     subprocess_callback,
 )
 
 Time = date | datetime
 
 
 class CalendarProperties(TypedDict):
-    """ Properties of a khal Event. """
+    """Properties of a khal Event."""
 
     attendees: list[str]
     categories: list[str]
     description: str
     end: datetime | date
     location: str
     rrule: dict | None
@@ -63,34 +62,37 @@
     ----------
         name: calendar name
         config: Khal config
         list: export command (khal list)
         new_item: new command (khal new)
     """
 
-    MESSAGE_EDIT: str = ('When trying to edit an event, the number of events '
-                         'found in the khal calendar was not 1 but: {}. The '
-                         'command was aborted.')
+    MESSAGE_EDIT: str = (
+        "When trying to edit an event, the number of events "
+        "found in the khal calendar was not 1 but: {}. The "
+        "command was aborted."
+    )
 
     MESSAGE_DELETE: str = (
-        'When trying to delete an event, the number of events'
-        ' found in the khal calendar was not 1 but: {}. The '
-        'command was aborted.')
+        "When trying to delete an event, the number of events"
+        " found in the khal calendar was not 1 but: {}. The "
+        "command was aborted."
+    )
 
     def __init__(self, name: str):
         """
         Init.
 
         Args:
         ----
             name: name of the khal calendar
         """
         path_config: Union[str, None] = find_configuration_file()
 
-        khal_bin: str = join(dirname(sys.executable), 'khal')
+        khal_bin: str = find_khal_bin()
         new_item_args: list = [khal_bin, "new"]
         list_args: list = [khal_bin, "list", "-df", ""]
 
         self._collection: CalendarCollection
         self._new_item: Callable = subprocess_callback(new_item_args)
         self._list_command: Callable = subprocess_callback(list_args)
 
@@ -122,59 +124,60 @@
             khal_args: list containing the command line arg that are send to
             `khal list`.
 
         Returns
         -------
             stdout of the `khal list`
         """
-        logging.info(f'khalorg list args are: {khal_args}')
+        logging.info(f"khalorg list args are: {khal_args}")
         return self._list_command(khal_args)
 
     @property
     def date_format(self) -> str:
         """
         longdatetimeformat.
 
         Returns
         -------
 
         """
-        return self.config['locale']['longdateformat']
+        return self.config["locale"]["longdateformat"]
 
     @property
     def datetime_format(self) -> str:
         """
         longdatetimeformat.
 
         Returns
         -------
 
         """
-        return self.config['locale']['longdatetimeformat']
+        return self.config["locale"]["longdatetimeformat"]
 
     @property
     def collection(self) -> CalendarCollection:
         """
         Returns the calendar collection of khal.
 
         It will be created once, and stored at `_collection`.
 
 
         Returns
         -------
             khal calendar collection.
 
         """
-        if not hasattr(self, '_collection'):
+        if not hasattr(self, "_collection"):
             self._collection = get_calendar_collection(self.name)
 
         return self._collection
 
-    def edit(self, props: CalendarProperties,
-             edit_dates: bool = False) -> list[Event]:
+    def edit(
+        self, props: CalendarProperties, edit_dates: bool = False
+    ) -> list[Event]:
         """
         Edit an existing event.
 
         The properties can be supplied through `props`.
 
         If the UID property is empty, the event will be located using its
         summary, start time, and end time. This may occur when an event is just
@@ -193,22 +196,22 @@
         Returns
         -------
             the edited events
 
         """
         events: list[Event]
 
-        if props['uid']:
-            events = self.get_events(props['uid'])
+        if props["uid"]:
+            events = self.get_events(props["uid"])
         else:
-            events = self.get_events_no_uid(props['summary'],
-                                            props['start'],
-                                            props['end'])
+            events = self.get_events_no_uid(
+                props["summary"], props["start"], props["end"]
+            )
 
-        logging.info(f'number of events is {len(events)}')
+        logging.info(f"number of events is {len(events)}")
         events = [x for x in events if is_future(x.end)]
 
         if len(events) == 0:
             logging.error(self.MESSAGE_EDIT.format(len(events)))
 
         else:
             # Khal opdates the master/PROTO event (i.e., the series of events),
@@ -224,45 +227,44 @@
         the khal config.
 
         Returns
         -------
             now in the local timezone
 
         """
-        return self.config['locale']['default_timezone'].localize(
-            datetime.now())
+        return self.config["locale"]["default_timezone"].localize(
+            datetime.now()
+        )
 
     def update_event(
-            self,
-            event: Event,
-            props: CalendarProperties,
-            edit_dates: bool = False) -> Event:
+        self, event: Event, props: CalendarProperties, edit_dates: bool = False
+    ) -> Event:
         """
         Update an event with `props`.
 
         Args:
         ----
             event: the event
             props: a typed dict
 
         Returns
         -------
             the update version of `event`
 
         """
-        event.update_url(props['url'])
-        event.update_summary(props['summary'])
-        event.update_location(props['location'])
-        event.update_attendees(props['attendees'])
-        event.update_categories(props['categories'])
-        event.update_description(props['description'])
+        event.update_url(props["url"])
+        event.update_summary(props["summary"])
+        event.update_location(props["location"])
+        event.update_attendees(props["attendees"])
+        event.update_categories(props["categories"])
+        event.update_description(props["description"])
 
         if edit_dates:
-            event.update_start_end(props['start'], props['end'])
-            event.update_rrule(props['rrule'])
+            event.update_start_end(props["start"], props["end"])
+            event.update_rrule(props["rrule"])
 
         event.increment_sequence()
         self.collection.update(event)
         self.collection.update_db()
 
         return event
 
@@ -281,18 +283,16 @@
         # For unknown reasons, the CalendarCollection.search method cannot find
         # uids that are longer than 39 chars. Therefore, they are clipped and
         # filtered with a list comprehension later on.
         events: Iterable[Event] = self.collection.search(uid[-39:])
         return [x for x in events if x.uid == uid or not uid]
 
     def get_events_no_uid(
-            self,
-            summary_wanted: str,
-            start_wanted: Time,
-            end_wanted: Time) -> list[Event]:
+        self, summary_wanted: str, start_wanted: Time, end_wanted: Time
+    ) -> list[Event]:
         """
         Return events that share the same summary, start time and stop time.
 
         Timezone information is not supported yet, so it is ignored by setting
         the Event.end.tzinfo to None.
 
         Args:
@@ -301,61 +301,59 @@
             start_wanted: start time
             end_wanted: end time
 
         Returns
         -------
             list of events
         """
+
         def exists(summary: str, end: Time) -> bool:
             equal_end: bool = remove_tzinfo(end) == remove_tzinfo(end_wanted)
             equal_summary: bool = summary == summary_wanted
             return equal_end and equal_summary
 
-        logging.info(f'Get events on date: {start_wanted}')
+        logging.info(f"Get events on date: {start_wanted}")
         return [
-            event for event in self.collection.get_events_on(start_wanted)
+            event
+            for event in self.collection.get_events_on(start_wanted)
             if exists(event.summary, event.end)
         ]
 
     def update(self, event: Event) -> None:
         self.collection.update(event)
 
     def exists(
-            self,
-            summary_wanted: str,
-            start_wanted: Time,
-            end_wanted: Time) -> bool:
+        self, summary_wanted: str, start_wanted: Time, end_wanted: Time
+    ) -> bool:
         """
         Returns True if an item exists at this specific time, with the same
         title.
         """
         events: list = self.get_events_no_uid(
-            summary_wanted,
-            start_wanted,
-            end_wanted
+            summary_wanted, start_wanted, end_wanted
         )
         return len(events) > 0
 
     def delete(self, props: CalendarProperties) -> str:
         """Deletes an event from the Calendar.collection. The whole series is
         removed.
 
         Args:
         ----
             props: dictionary representing the event.
         """
-        events: list = self.get_events(props['uid'])
+        events: list = self.get_events(props["uid"])
 
         if len(events) == 0:
             logging.error(self.MESSAGE_DELETE.format(len(events)))
         else:
             # For now, the whole series is repmoved.
             event = events[0]
             assert event.href is not None
             try:
-                self.collection.delete(event.href,
-                                       event.etag,
-                                       calendar=event.calendar)
+                self.collection.delete(
+                    event.href, event.etag, calendar=event.calendar
+                )
             except NotFoundError as error:
                 logging.error(error)
             finally:
-                return ''
+                return ""
```

### Comparing `khalorg-0.0.2/src/khalorg/khal/checker.py` & `khalorg-0.0.3/src/khalorg/khal/checker.py`

 * *Files identical despite different names*

### Comparing `khalorg-0.0.2/src/khalorg/khal/helpers.py` & `khalorg-0.0.3/src/khalorg/khal/helpers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,36 @@
 import logging
+import sys
 from datetime import date, datetime
+from os.path import dirname, exists, join
 from subprocess import STDOUT, CalledProcessError, check_output
 from typing import Callable
 
 from khalorg import paths
 
 Time = date | datetime
 
 
+def find_khal_bin() -> str:
+    """Returns the khal executable.
+
+    When pipx is used, the khal executable is located in the same directory
+    as the python executable. When using a virtual environment, or the
+    global python installation, the khal executable is located in the PATH.
+
+    Returns:
+    --------
+        path to the khal executable
+    """
+    bin: str = join(dirname(sys.executable), "khal")
+    bin = bin if exists(bin) else "khal"
+    logging.debug("khal executable is: %s", bin)
+    return bin
+
+
 def get_khal_format():
     """
     Returns the format that is used for the `khal list --format` command
     that is used within the `khalorg list` command.
 
     Returns
     -------
```

### Comparing `khalorg-0.0.2/src/khalorg/org/agenda_items.py` & `khalorg-0.0.3/src/khalorg/org/agenda_items.py`

 * *Files identical despite different names*

### Comparing `khalorg-0.0.2/src/khalorg/org/helpers.py` & `khalorg-0.0.3/src/khalorg/org/helpers.py`

 * *Files identical despite different names*

### Comparing `khalorg-0.0.2/src/khalorg/rrule.py` & `khalorg-0.0.3/src/khalorg/rrule.py`

 * *Files identical despite different names*

### Comparing `khalorg-0.0.2/src/khalorg/static/description_list_command.txt` & `khalorg-0.0.3/src/khalorg/static/description_list_command.txt`

 * *Files identical despite different names*

### Comparing `khalorg-0.0.2/src/khalorg.egg-info/PKG-INFO` & `khalorg-0.0.3/src/khalorg.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: khalorg
-Version: 0.0.2
+Version: 0.0.3
 Summary: An interface between Org mode and Khal cli calendar.
 Author: BartSte
 License: MIT License
 Keywords: khal,org mode,vdirsyncer,CalDav,agenda,emacs,neovim,orgmode-nvim
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `khalorg-0.0.2/src/khalorg.egg-info/SOURCES.txt` & `khalorg-0.0.3/src/khalorg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `khalorg-0.0.2/tests/agenda_items.py` & `khalorg-0.0.3/tests/agenda_items.py`

 * *Files identical despite different names*

### Comparing `khalorg-0.0.2/tests/helpers.py` & `khalorg-0.0.3/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `khalorg-0.0.2/tests/khalorg_tester` & `khalorg-0.0.3/tests/khalorg_tester`

 * *Files identical despite different names*

### Comparing `khalorg-0.0.2/tests/static/agenda_items/duplicate.org` & `khalorg-0.0.3/tests/static/agenda_items/duplicate.org`

 * *Files identical despite different names*

### Comparing `khalorg-0.0.2/tests/static/agenda_items/multiple_timestamps.org` & `khalorg-0.0.3/tests/static/agenda_items/multiple_timestamps.org`

 * *Files identical despite different names*

### Comparing `khalorg-0.0.2/tests/static/agenda_items/multiple_timestamps_unsorted.org` & `khalorg-0.0.3/tests/static/agenda_items/multiple_timestamps_unsorted.org`

 * *Files identical despite different names*

### Comparing `khalorg-0.0.2/tests/static/agenda_items/recurring_first_item_moved.org` & `khalorg-0.0.3/tests/static/agenda_items/recurring_first_item_moved.org`

 * *Files identical despite different names*

### Comparing `khalorg-0.0.2/tests/static/agenda_items/recurring_first_item_moved_expected.org` & `khalorg-0.0.3/tests/static/agenda_items/recurring_first_item_moved_expected.org`

 * *Files identical despite different names*

### Comparing `khalorg-0.0.2/tests/static/agenda_items/rrule_recurring.org` & `khalorg-0.0.3/tests/static/agenda_items/rrule_recurring.org`

 * *Files identical despite different names*

### Comparing `khalorg-0.0.2/tests/static/agenda_items/rrule_recurring_and_non_recurring.org` & `khalorg-0.0.3/tests/static/agenda_items/rrule_recurring_and_non_recurring.org`

 * *Files identical despite different names*

### Comparing `khalorg-0.0.2/tests/static/agenda_items/rrule_recurring_duplicates.org` & `khalorg-0.0.3/tests/static/agenda_items/rrule_recurring_duplicates.org`

 * *Files identical despite different names*

### Comparing `khalorg-0.0.2/tests/static/agenda_items/two_items.org` & `khalorg-0.0.3/tests/static/agenda_items/two_items.org`

 * *Files identical despite different names*

### Comparing `khalorg-0.0.2/tests/static/test_config_khal` & `khalorg-0.0.3/tests/static/test_config_khal`

 * *Files identical despite different names*

### Comparing `khalorg-0.0.2/tests/test_cli.py` & `khalorg-0.0.3/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `khalorg-0.0.2/tests/test_commands.py` & `khalorg-0.0.3/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `khalorg-0.0.2/tests/test_helpers.py` & `khalorg-0.0.3/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `khalorg-0.0.2/tests/test_khal/helpers.py` & `khalorg-0.0.3/tests/test_khal/helpers.py`

 * *Files identical despite different names*

### Comparing `khalorg-0.0.2/tests/test_khal/test_args.py` & `khalorg-0.0.3/tests/test_khal/test_args.py`

 * *Files identical despite different names*

### Comparing `khalorg-0.0.2/tests/test_khal/test_calendar.py` & `khalorg-0.0.3/tests/test_khal/test_calendar.py`

 * *Files identical despite different names*

### Comparing `khalorg-0.0.2/tests/test_khal/test_checker.py` & `khalorg-0.0.3/tests/test_khal/test_checker.py`

 * *Files identical despite different names*

### Comparing `khalorg-0.0.2/tests/test_org/test_agenda_items.py` & `khalorg-0.0.3/tests/test_org/test_agenda_items.py`

 * *Files identical despite different names*

### Comparing `khalorg-0.0.2/tests/test_org/test_helpers.py` & `khalorg-0.0.3/tests/test_org/test_helpers.py`

 * *Files identical despite different names*

### Comparing `khalorg-0.0.2/tests/test_rrule.py` & `khalorg-0.0.3/tests/test_rrule.py`

 * *Files identical despite different names*

