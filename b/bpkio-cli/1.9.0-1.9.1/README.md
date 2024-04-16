# Comparing `tmp/bpkio_cli-1.9.0.tar.gz` & `tmp/bpkio_cli-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bpkio_cli-1.9.0.tar", max compression
+gzip compressed data, was "bpkio_cli-1.9.1.tar", max compression
```

## Comparing `bpkio_cli-1.9.0.tar` & `bpkio_cli-1.9.1.tar`

### file list

```diff
@@ -1,83 +1,83 @@
--rw-r--r--   0        0        0        0 2023-06-05 14:52:28.912688 bpkio_cli-1.9.0/README.md
--rw-r--r--   0        0        0       22 2023-10-12 11:01:23.743446 bpkio_cli-1.9.0/bpkio_cli/__init__.py
--rw-r--r--   0        0        0     3969 2023-11-01 21:40:20.112799 bpkio_cli-1.9.0/bpkio_cli/app.py
--rw-r--r--   0        0        0    72608 2023-10-26 12:25:17.103635 bpkio_cli-1.9.0/bpkio_cli/assets/C3-C4.wav
--rw-r--r--   0        0        0    72608 2023-10-26 12:25:17.104756 bpkio_cli-1.9.0/bpkio_cli/assets/C4-C3.wav
--rw-r--r--   0        0        0    72608 2023-10-26 12:25:17.105701 bpkio_cli-1.9.0/bpkio_cli/assets/C4-C5.wav
--rw-r--r--   0        0        0    72586 2023-10-26 12:25:17.106979 bpkio_cli-1.9.0/bpkio_cli/assets/C4-G4.wav
--rw-r--r--   0        0        0    72608 2023-10-26 12:25:17.107871 bpkio_cli-1.9.0/bpkio_cli/assets/C5-C4.wav
--rw-r--r--   0        0        0    52346 2023-10-26 12:25:17.108614 bpkio_cli-1.9.0/bpkio_cli/assets/E4-E4.wav
--rw-r--r--   0        0        0    49670 2023-10-26 12:25:17.109301 bpkio_cli-1.9.0/bpkio_cli/assets/G4-C4.wav
--rw-r--r--   0        0        0       91 2023-06-05 14:52:28.913801 bpkio_cli-1.9.0/bpkio_cli/click_mods/__init__.py
--rw-r--r--   0        0        0      771 2023-06-05 14:52:28.914515 bpkio_cli-1.9.0/bpkio_cli/click_mods/default_last_command.py
--rw-r--r--   0        0        0     5244 2023-10-30 20:02:17.916972 bpkio_cli-1.9.0/bpkio_cli/click_mods/group_rest_resource.py
--rw-r--r--   0        0        0     1747 2023-06-05 14:52:28.915564 bpkio_cli-1.9.0/bpkio_cli/click_mods/option_eat_all.py
--rw-r--r--   0        0        0      625 2023-10-12 11:01:23.744874 bpkio_cli-1.9.0/bpkio_cli/click_options/__init__.py
--rw-r--r--   0        0        0      848 2023-06-05 14:52:28.916749 bpkio_cli-1.9.0/bpkio_cli/click_options/admin.py
--rw-r--r--   0        0        0     1380 2023-10-12 11:01:23.745481 bpkio_cli-1.9.0/bpkio_cli/click_options/list.py
--rw-r--r--   0        0        0     1076 2023-10-12 11:01:23.745844 bpkio_cli-1.9.0/bpkio_cli/click_options/list_format.py
--rw-r--r--   0        0        0     1247 2023-10-26 12:25:17.109845 bpkio_cli-1.9.0/bpkio_cli/click_options/poll.py
--rw-r--r--   0        0        0     1106 2023-10-12 11:01:23.746494 bpkio_cli-1.9.0/bpkio_cli/click_options/read.py
--rw-r--r--   0        0        0     1552 2023-10-12 11:01:23.746731 bpkio_cli-1.9.0/bpkio_cli/click_options/search.py
--rw-r--r--   0        0        0      407 2023-10-12 11:01:23.746934 bpkio_cli-1.9.0/bpkio_cli/click_options/table.py
--rw-r--r--   0        0        0     2465 2023-10-31 20:11:23.935620 bpkio_cli-1.9.0/bpkio_cli/click_options/urls.py
--rw-r--r--   0        0        0      722 2023-11-01 21:34:16.399459 bpkio_cli-1.9.0/bpkio_cli/commands/__init__.py
--rw-r--r--   0        0        0      751 2023-06-07 16:02:26.119276 bpkio_cli-1.9.0/bpkio_cli/commands/addons.py
--rw-r--r--   0        0        0      369 2023-11-01 21:39:06.406729 bpkio_cli-1.9.0/bpkio_cli/commands/categories.py
--rw-r--r--   0        0        0     5692 2023-10-12 11:01:42.549805 bpkio_cli-1.9.0/bpkio_cli/commands/configure.py
--rw-r--r--   0        0        0     1766 2023-06-07 15:41:46.997118 bpkio_cli-1.9.0/bpkio_cli/commands/consumption.py
--rw-r--r--   0        0        0     4327 2023-10-16 14:25:54.473649 bpkio_cli-1.9.0/bpkio_cli/commands/creators/ad_insertion.py
--rw-r--r--   0        0        0     1236 2023-10-16 14:25:54.473905 bpkio_cli-1.9.0/bpkio_cli/commands/creators/services.py
--rw-r--r--   0        0        0     7678 2023-10-16 14:25:54.474235 bpkio_cli-1.9.0/bpkio_cli/commands/creators/sources.py
--rw-r--r--   0        0        0     3951 2023-10-30 19:58:12.740153 bpkio_cli-1.9.0/bpkio_cli/commands/creators/virtual_channel.py
--rw-r--r--   0        0        0    11459 2023-11-02 20:47:34.374573 bpkio_cli-1.9.0/bpkio_cli/commands/creators/virtual_channel_populate.py
--rw-r--r--   0        0        0     2259 2023-10-30 20:31:55.804645 bpkio_cli-1.9.0/bpkio_cli/commands/creators/virtual_channel_slot.py
--rw-r--r--   0        0        0      726 2023-10-12 11:01:23.750121 bpkio_cli-1.9.0/bpkio_cli/commands/hello.py
--rw-r--r--   0        0        0    11572 2023-10-26 12:25:17.110522 bpkio_cli-1.9.0/bpkio_cli/commands/live_monitor.py
--rw-r--r--   0        0        0     1251 2023-06-05 14:52:28.924268 bpkio_cli-1.9.0/bpkio_cli/commands/memory.py
--rw-r--r--   0        0        0     3412 2023-10-12 11:01:23.750325 bpkio_cli-1.9.0/bpkio_cli/commands/package.py
--rw-r--r--   0        0        0    10136 2023-10-12 11:01:23.750612 bpkio_cli-1.9.0/bpkio_cli/commands/profiles.py
--rw-r--r--   0        0        0     2641 2023-10-12 11:01:23.750888 bpkio_cli-1.9.0/bpkio_cli/commands/recorder.py
--rw-r--r--   0        0        0     4216 2023-11-02 18:20:19.318978 bpkio_cli-1.9.0/bpkio_cli/commands/services.py
--rw-r--r--   0        0        0     5794 2023-10-16 14:25:54.509736 bpkio_cli-1.9.0/bpkio_cli/commands/sources.py
--rw-r--r--   0        0        0    23019 2023-10-31 20:36:23.544288 bpkio_cli-1.9.0/bpkio_cli/commands/template_crud.py
--rw-r--r--   0        0        0    14382 2023-11-03 15:18:41.466075 bpkio_cli-1.9.0/bpkio_cli/commands/template_crud_slots.py
--rw-r--r--   0        0        0      937 2023-10-12 11:01:52.286089 bpkio_cli-1.9.0/bpkio_cli/commands/tenants.py
--rw-r--r--   0        0        0     7795 2023-10-26 12:25:17.111375 bpkio_cli-1.9.0/bpkio_cli/commands/url.py
--rw-r--r--   0        0        0      363 2023-10-12 11:01:23.753056 bpkio_cli-1.9.0/bpkio_cli/commands/users.py
--rw-r--r--   0        0        0     1036 2023-06-05 14:52:28.927822 bpkio_cli-1.9.0/bpkio_cli/core/app_context.py
--rw-r--r--   0        0        0     1834 2023-10-31 20:36:23.554989 bpkio_cli-1.9.0/bpkio_cli/core/click_helpers.py
--rw-r--r--   0        0        0     4659 2023-10-12 11:01:23.753713 bpkio_cli-1.9.0/bpkio_cli/core/config_provider.py
--rw-r--r--   0        0        0      277 2023-10-16 14:25:54.476298 bpkio_cli-1.9.0/bpkio_cli/core/exceptions.py
--rw-r--r--   0        0        0     2714 2023-10-12 11:01:23.754467 bpkio_cli-1.9.0/bpkio_cli/core/initialize.py
--rw-r--r--   0        0        0     1718 2023-06-05 14:52:28.929630 bpkio_cli-1.9.0/bpkio_cli/core/logger.py
--rw-r--r--   0        0        0     8332 2023-06-07 15:41:47.001439 bpkio_cli-1.9.0/bpkio_cli/core/packager.py
--rw-r--r--   0        0        0      432 2023-11-02 20:42:45.253311 bpkio_cli-1.9.0/bpkio_cli/core/resource_decorator.py
--rw-r--r--   0        0        0     9526 2023-10-12 11:01:23.754841 bpkio_cli-1.9.0/bpkio_cli/core/resource_recorder.py
--rw-r--r--   0        0        0     2272 2023-10-12 11:01:23.755110 bpkio_cli-1.9.0/bpkio_cli/core/resource_trail.py
--rw-r--r--   0        0        0     5961 2023-10-12 11:01:23.755513 bpkio_cli-1.9.0/bpkio_cli/core/response_handler.py
--rw-r--r--   0        0        0     1234 2023-06-05 14:52:28.931905 bpkio_cli-1.9.0/bpkio_cli/core/session_recorder.py
--rw-r--r--   0        0        0      395 2023-06-05 14:52:28.932292 bpkio_cli-1.9.0/bpkio_cli/utils/__init__.py
--rw-r--r--   0        0        0     2288 2023-06-05 14:52:28.932584 bpkio_cli-1.9.0/bpkio_cli/utils/arrays.py
--rw-r--r--   0        0        0     2318 2023-11-03 09:34:50.338820 bpkio_cli-1.9.0/bpkio_cli/utils/datetimes.py
--rw-r--r--   0        0        0     1836 2023-10-12 11:01:23.755910 bpkio_cli-1.9.0/bpkio_cli/utils/editor.py
--rw-r--r--   0        0        0      136 2023-06-05 14:52:28.933905 bpkio_cli-1.9.0/bpkio_cli/utils/json.py
--rw-r--r--   0        0        0      610 2023-10-12 11:01:23.756233 bpkio_cli-1.9.0/bpkio_cli/utils/profile_maker.py
--rw-r--r--   0        0        0     4781 2023-10-12 11:01:23.756439 bpkio_cli-1.9.0/bpkio_cli/utils/prompt.py
--rw-r--r--   0        0        0      519 2023-10-26 12:25:17.111655 bpkio_cli-1.9.0/bpkio_cli/utils/sounds.py
--rw-r--r--   0        0        0    13307 2023-10-31 20:36:09.005488 bpkio_cli-1.9.0/bpkio_cli/utils/url_builders.py
--rw-r--r--   0        0        0     1124 2023-10-31 20:22:56.832795 bpkio_cli-1.9.0/bpkio_cli/utils/urls.py
--rw-r--r--   0        0        0     1034 2023-06-05 14:52:28.935214 bpkio_cli-1.9.0/bpkio_cli/writers/breadcrumbs.py
--rw-r--r--   0        0        0     4318 2023-11-03 09:24:50.981654 bpkio_cli-1.9.0/bpkio_cli/writers/colorizer.py
--rw-r--r--   0        0        0     5679 2023-10-26 12:25:17.112367 bpkio_cli-1.9.0/bpkio_cli/writers/content_display.py
--rw-r--r--   0        0        0      840 2023-06-05 14:52:28.936348 bpkio_cli-1.9.0/bpkio_cli/writers/diff.py
--rw-r--r--   0        0        0      757 2023-10-26 12:25:17.112704 bpkio_cli-1.9.0/bpkio_cli/writers/formatter.py
--rw-r--r--   0        0        0     8587 2023-10-30 12:42:40.993858 bpkio_cli-1.9.0/bpkio_cli/writers/hls_formatter.py
--rw-r--r--   0        0        0      714 2023-10-26 12:19:49.646176 bpkio_cli-1.9.0/bpkio_cli/writers/json_formatter.py
--rw-r--r--   0        0        0     1567 2023-10-12 11:01:23.757942 bpkio_cli-1.9.0/bpkio_cli/writers/players.py
--rw-r--r--   0        0        0     2089 2023-10-26 12:25:17.113205 bpkio_cli-1.9.0/bpkio_cli/writers/scte35.py
--rw-r--r--   0        0        0     2068 2023-10-12 11:01:23.758385 bpkio_cli-1.9.0/bpkio_cli/writers/tables.py
--rw-r--r--   0        0        0     1324 2023-10-12 11:01:48.095433 bpkio_cli-1.9.0/bpkio_cli/writers/urls.py
--rw-r--r--   0        0        0     5740 2023-10-16 14:25:54.477594 bpkio_cli-1.9.0/bpkio_cli/writers/xml_formatter.py
--rw-r--r--   0        0        0     1324 2023-11-06 18:26:38.665278 bpkio_cli-1.9.0/pyproject.toml
--rw-r--r--   0        0        0     1136 1970-01-01 00:00:00.000000 bpkio_cli-1.9.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-05 14:52:28.912688 bpkio_cli-1.9.1/README.md
+-rw-r--r--   0        0        0       22 2023-10-12 11:01:23.743446 bpkio_cli-1.9.1/bpkio_cli/__init__.py
+-rw-r--r--   0        0        0     3969 2023-11-01 21:40:20.112799 bpkio_cli-1.9.1/bpkio_cli/app.py
+-rw-r--r--   0        0        0    72608 2023-10-26 12:25:17.103635 bpkio_cli-1.9.1/bpkio_cli/assets/C3-C4.wav
+-rw-r--r--   0        0        0    72608 2023-10-26 12:25:17.104756 bpkio_cli-1.9.1/bpkio_cli/assets/C4-C3.wav
+-rw-r--r--   0        0        0    72608 2023-10-26 12:25:17.105701 bpkio_cli-1.9.1/bpkio_cli/assets/C4-C5.wav
+-rw-r--r--   0        0        0    72586 2023-10-26 12:25:17.106979 bpkio_cli-1.9.1/bpkio_cli/assets/C4-G4.wav
+-rw-r--r--   0        0        0    72608 2023-10-26 12:25:17.107871 bpkio_cli-1.9.1/bpkio_cli/assets/C5-C4.wav
+-rw-r--r--   0        0        0    52346 2023-10-26 12:25:17.108614 bpkio_cli-1.9.1/bpkio_cli/assets/E4-E4.wav
+-rw-r--r--   0        0        0    49670 2023-10-26 12:25:17.109301 bpkio_cli-1.9.1/bpkio_cli/assets/G4-C4.wav
+-rw-r--r--   0        0        0       91 2023-06-05 14:52:28.913801 bpkio_cli-1.9.1/bpkio_cli/click_mods/__init__.py
+-rw-r--r--   0        0        0      771 2023-06-05 14:52:28.914515 bpkio_cli-1.9.1/bpkio_cli/click_mods/default_last_command.py
+-rw-r--r--   0        0        0     5244 2023-10-30 20:02:17.916972 bpkio_cli-1.9.1/bpkio_cli/click_mods/group_rest_resource.py
+-rw-r--r--   0        0        0     1747 2023-06-05 14:52:28.915564 bpkio_cli-1.9.1/bpkio_cli/click_mods/option_eat_all.py
+-rw-r--r--   0        0        0      625 2023-10-12 11:01:23.744874 bpkio_cli-1.9.1/bpkio_cli/click_options/__init__.py
+-rw-r--r--   0        0        0      848 2023-06-05 14:52:28.916749 bpkio_cli-1.9.1/bpkio_cli/click_options/admin.py
+-rw-r--r--   0        0        0     1380 2023-10-12 11:01:23.745481 bpkio_cli-1.9.1/bpkio_cli/click_options/list.py
+-rw-r--r--   0        0        0     1076 2023-10-12 11:01:23.745844 bpkio_cli-1.9.1/bpkio_cli/click_options/list_format.py
+-rw-r--r--   0        0        0     1247 2023-10-26 12:25:17.109845 bpkio_cli-1.9.1/bpkio_cli/click_options/poll.py
+-rw-r--r--   0        0        0     1106 2023-10-12 11:01:23.746494 bpkio_cli-1.9.1/bpkio_cli/click_options/read.py
+-rw-r--r--   0        0        0     1552 2023-10-12 11:01:23.746731 bpkio_cli-1.9.1/bpkio_cli/click_options/search.py
+-rw-r--r--   0        0        0      407 2023-10-12 11:01:23.746934 bpkio_cli-1.9.1/bpkio_cli/click_options/table.py
+-rw-r--r--   0        0        0     2465 2023-10-31 20:11:23.935620 bpkio_cli-1.9.1/bpkio_cli/click_options/urls.py
+-rw-r--r--   0        0        0      722 2023-11-01 21:34:16.399459 bpkio_cli-1.9.1/bpkio_cli/commands/__init__.py
+-rw-r--r--   0        0        0      751 2023-06-07 16:02:26.119276 bpkio_cli-1.9.1/bpkio_cli/commands/addons.py
+-rw-r--r--   0        0        0      369 2023-11-01 21:39:06.406729 bpkio_cli-1.9.1/bpkio_cli/commands/categories.py
+-rw-r--r--   0        0        0     5692 2023-10-12 11:01:42.549805 bpkio_cli-1.9.1/bpkio_cli/commands/configure.py
+-rw-r--r--   0        0        0     1766 2023-06-07 15:41:46.997118 bpkio_cli-1.9.1/bpkio_cli/commands/consumption.py
+-rw-r--r--   0        0        0     4327 2023-10-16 14:25:54.473649 bpkio_cli-1.9.1/bpkio_cli/commands/creators/ad_insertion.py
+-rw-r--r--   0        0        0     1236 2023-10-16 14:25:54.473905 bpkio_cli-1.9.1/bpkio_cli/commands/creators/services.py
+-rw-r--r--   0        0        0     7678 2023-10-16 14:25:54.474235 bpkio_cli-1.9.1/bpkio_cli/commands/creators/sources.py
+-rw-r--r--   0        0        0     3951 2023-10-30 19:58:12.740153 bpkio_cli-1.9.1/bpkio_cli/commands/creators/virtual_channel.py
+-rw-r--r--   0        0        0    11459 2023-11-02 20:47:34.374573 bpkio_cli-1.9.1/bpkio_cli/commands/creators/virtual_channel_populate.py
+-rw-r--r--   0        0        0     2259 2023-10-30 20:31:55.804645 bpkio_cli-1.9.1/bpkio_cli/commands/creators/virtual_channel_slot.py
+-rw-r--r--   0        0        0      726 2023-10-12 11:01:23.750121 bpkio_cli-1.9.1/bpkio_cli/commands/hello.py
+-rw-r--r--   0        0        0    11649 2023-11-07 14:17:31.895727 bpkio_cli-1.9.1/bpkio_cli/commands/live_monitor.py
+-rw-r--r--   0        0        0     1251 2023-06-05 14:52:28.924268 bpkio_cli-1.9.1/bpkio_cli/commands/memory.py
+-rw-r--r--   0        0        0     3412 2023-10-12 11:01:23.750325 bpkio_cli-1.9.1/bpkio_cli/commands/package.py
+-rw-r--r--   0        0        0    10136 2023-10-12 11:01:23.750612 bpkio_cli-1.9.1/bpkio_cli/commands/profiles.py
+-rw-r--r--   0        0        0     2641 2023-10-12 11:01:23.750888 bpkio_cli-1.9.1/bpkio_cli/commands/recorder.py
+-rw-r--r--   0        0        0     4216 2023-11-02 18:20:19.318978 bpkio_cli-1.9.1/bpkio_cli/commands/services.py
+-rw-r--r--   0        0        0     5794 2023-10-16 14:25:54.509736 bpkio_cli-1.9.1/bpkio_cli/commands/sources.py
+-rw-r--r--   0        0        0    23019 2023-10-31 20:36:23.544288 bpkio_cli-1.9.1/bpkio_cli/commands/template_crud.py
+-rw-r--r--   0        0        0    14382 2023-11-03 15:18:41.466075 bpkio_cli-1.9.1/bpkio_cli/commands/template_crud_slots.py
+-rw-r--r--   0        0        0      937 2023-10-12 11:01:52.286089 bpkio_cli-1.9.1/bpkio_cli/commands/tenants.py
+-rw-r--r--   0        0        0     7795 2023-10-26 12:25:17.111375 bpkio_cli-1.9.1/bpkio_cli/commands/url.py
+-rw-r--r--   0        0        0      363 2023-10-12 11:01:23.753056 bpkio_cli-1.9.1/bpkio_cli/commands/users.py
+-rw-r--r--   0        0        0     1036 2023-06-05 14:52:28.927822 bpkio_cli-1.9.1/bpkio_cli/core/app_context.py
+-rw-r--r--   0        0        0     1834 2023-10-31 20:36:23.554989 bpkio_cli-1.9.1/bpkio_cli/core/click_helpers.py
+-rw-r--r--   0        0        0     4659 2023-10-12 11:01:23.753713 bpkio_cli-1.9.1/bpkio_cli/core/config_provider.py
+-rw-r--r--   0        0        0      277 2023-10-16 14:25:54.476298 bpkio_cli-1.9.1/bpkio_cli/core/exceptions.py
+-rw-r--r--   0        0        0     2714 2023-10-12 11:01:23.754467 bpkio_cli-1.9.1/bpkio_cli/core/initialize.py
+-rw-r--r--   0        0        0     1718 2023-06-05 14:52:28.929630 bpkio_cli-1.9.1/bpkio_cli/core/logger.py
+-rw-r--r--   0        0        0     8332 2023-06-07 15:41:47.001439 bpkio_cli-1.9.1/bpkio_cli/core/packager.py
+-rw-r--r--   0        0        0      432 2023-11-02 20:42:45.253311 bpkio_cli-1.9.1/bpkio_cli/core/resource_decorator.py
+-rw-r--r--   0        0        0     9526 2023-10-12 11:01:23.754841 bpkio_cli-1.9.1/bpkio_cli/core/resource_recorder.py
+-rw-r--r--   0        0        0     2272 2023-10-12 11:01:23.755110 bpkio_cli-1.9.1/bpkio_cli/core/resource_trail.py
+-rw-r--r--   0        0        0     5961 2023-10-12 11:01:23.755513 bpkio_cli-1.9.1/bpkio_cli/core/response_handler.py
+-rw-r--r--   0        0        0     1234 2023-06-05 14:52:28.931905 bpkio_cli-1.9.1/bpkio_cli/core/session_recorder.py
+-rw-r--r--   0        0        0      395 2023-06-05 14:52:28.932292 bpkio_cli-1.9.1/bpkio_cli/utils/__init__.py
+-rw-r--r--   0        0        0     2288 2023-06-05 14:52:28.932584 bpkio_cli-1.9.1/bpkio_cli/utils/arrays.py
+-rw-r--r--   0        0        0     2318 2023-11-03 09:34:50.338820 bpkio_cli-1.9.1/bpkio_cli/utils/datetimes.py
+-rw-r--r--   0        0        0     1836 2023-10-12 11:01:23.755910 bpkio_cli-1.9.1/bpkio_cli/utils/editor.py
+-rw-r--r--   0        0        0      136 2023-06-05 14:52:28.933905 bpkio_cli-1.9.1/bpkio_cli/utils/json.py
+-rw-r--r--   0        0        0      610 2023-10-12 11:01:23.756233 bpkio_cli-1.9.1/bpkio_cli/utils/profile_maker.py
+-rw-r--r--   0        0        0     4781 2023-10-12 11:01:23.756439 bpkio_cli-1.9.1/bpkio_cli/utils/prompt.py
+-rw-r--r--   0        0        0      519 2023-10-26 12:25:17.111655 bpkio_cli-1.9.1/bpkio_cli/utils/sounds.py
+-rw-r--r--   0        0        0    13307 2023-10-31 20:36:09.005488 bpkio_cli-1.9.1/bpkio_cli/utils/url_builders.py
+-rw-r--r--   0        0        0     1124 2023-10-31 20:22:56.832795 bpkio_cli-1.9.1/bpkio_cli/utils/urls.py
+-rw-r--r--   0        0        0     1034 2023-06-05 14:52:28.935214 bpkio_cli-1.9.1/bpkio_cli/writers/breadcrumbs.py
+-rw-r--r--   0        0        0     4318 2023-11-03 09:24:50.981654 bpkio_cli-1.9.1/bpkio_cli/writers/colorizer.py
+-rw-r--r--   0        0        0     5679 2023-10-26 12:25:17.112367 bpkio_cli-1.9.1/bpkio_cli/writers/content_display.py
+-rw-r--r--   0        0        0      840 2023-06-05 14:52:28.936348 bpkio_cli-1.9.1/bpkio_cli/writers/diff.py
+-rw-r--r--   0        0        0      757 2023-10-26 12:25:17.112704 bpkio_cli-1.9.1/bpkio_cli/writers/formatter.py
+-rw-r--r--   0        0        0     8587 2023-10-30 12:42:40.993858 bpkio_cli-1.9.1/bpkio_cli/writers/hls_formatter.py
+-rw-r--r--   0        0        0      714 2023-10-26 12:19:49.646176 bpkio_cli-1.9.1/bpkio_cli/writers/json_formatter.py
+-rw-r--r--   0        0        0     1567 2023-10-12 11:01:23.757942 bpkio_cli-1.9.1/bpkio_cli/writers/players.py
+-rw-r--r--   0        0        0     2089 2023-10-26 12:25:17.113205 bpkio_cli-1.9.1/bpkio_cli/writers/scte35.py
+-rw-r--r--   0        0        0     2068 2023-10-12 11:01:23.758385 bpkio_cli-1.9.1/bpkio_cli/writers/tables.py
+-rw-r--r--   0        0        0     1324 2023-10-12 11:01:48.095433 bpkio_cli-1.9.1/bpkio_cli/writers/urls.py
+-rw-r--r--   0        0        0     5740 2023-10-16 14:25:54.477594 bpkio_cli-1.9.1/bpkio_cli/writers/xml_formatter.py
+-rw-r--r--   0        0        0     1324 2023-11-07 14:20:35.200534 bpkio_cli-1.9.1/pyproject.toml
+-rw-r--r--   0        0        0     1136 1970-01-01 00:00:00.000000 bpkio_cli-1.9.1/PKG-INFO
```

### Comparing `bpkio_cli-1.9.0/bpkio_cli/app.py` & `bpkio_cli-1.9.1/bpkio_cli/app.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.9.0/bpkio_cli/assets/C3-C4.wav` & `bpkio_cli-1.9.1/bpkio_cli/assets/C3-C4.wav`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.9.0/bpkio_cli/assets/C4-C3.wav` & `bpkio_cli-1.9.1/bpkio_cli/assets/C4-C3.wav`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.9.0/bpkio_cli/assets/C4-C5.wav` & `bpkio_cli-1.9.1/bpkio_cli/assets/C4-C5.wav`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.9.0/bpkio_cli/assets/C4-G4.wav` & `bpkio_cli-1.9.1/bpkio_cli/assets/C4-G4.wav`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.9.0/bpkio_cli/assets/C5-C4.wav` & `bpkio_cli-1.9.1/bpkio_cli/assets/C5-C4.wav`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.9.0/bpkio_cli/assets/E4-E4.wav` & `bpkio_cli-1.9.1/bpkio_cli/assets/E4-E4.wav`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.9.0/bpkio_cli/assets/G4-C4.wav` & `bpkio_cli-1.9.1/bpkio_cli/assets/G4-C4.wav`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.9.0/bpkio_cli/click_mods/default_last_command.py` & `bpkio_cli-1.9.1/bpkio_cli/click_mods/default_last_command.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.9.0/bpkio_cli/click_mods/group_rest_resource.py` & `bpkio_cli-1.9.1/bpkio_cli/click_mods/group_rest_resource.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.9.0/bpkio_cli/click_mods/option_eat_all.py` & `bpkio_cli-1.9.1/bpkio_cli/click_mods/option_eat_all.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.9.0/bpkio_cli/click_options/__init__.py` & `bpkio_cli-1.9.1/bpkio_cli/click_options/__init__.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.9.0/bpkio_cli/click_options/admin.py` & `bpkio_cli-1.9.1/bpkio_cli/click_options/admin.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.9.0/bpkio_cli/click_options/list.py` & `bpkio_cli-1.9.1/bpkio_cli/click_options/list.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.9.0/bpkio_cli/click_options/list_format.py` & `bpkio_cli-1.9.1/bpkio_cli/click_options/list_format.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.9.0/bpkio_cli/click_options/poll.py` & `bpkio_cli-1.9.1/bpkio_cli/click_options/poll.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.9.0/bpkio_cli/click_options/read.py` & `bpkio_cli-1.9.1/bpkio_cli/click_options/read.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.9.0/bpkio_cli/click_options/search.py` & `bpkio_cli-1.9.1/bpkio_cli/click_options/search.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.9.0/bpkio_cli/click_options/urls.py` & `bpkio_cli-1.9.1/bpkio_cli/click_options/urls.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.9.0/bpkio_cli/commands/__init__.py` & `bpkio_cli-1.9.1/bpkio_cli/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.9.0/bpkio_cli/commands/addons.py` & `bpkio_cli-1.9.1/bpkio_cli/commands/addons.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.9.0/bpkio_cli/commands/configure.py` & `bpkio_cli-1.9.1/bpkio_cli/commands/configure.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.9.0/bpkio_cli/commands/consumption.py` & `bpkio_cli-1.9.1/bpkio_cli/commands/consumption.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.9.0/bpkio_cli/commands/creators/ad_insertion.py` & `bpkio_cli-1.9.1/bpkio_cli/commands/creators/ad_insertion.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.9.0/bpkio_cli/commands/creators/services.py` & `bpkio_cli-1.9.1/bpkio_cli/commands/creators/services.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.9.0/bpkio_cli/commands/creators/sources.py` & `bpkio_cli-1.9.1/bpkio_cli/commands/creators/sources.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.9.0/bpkio_cli/commands/creators/virtual_channel.py` & `bpkio_cli-1.9.1/bpkio_cli/commands/creators/virtual_channel.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.9.0/bpkio_cli/commands/creators/virtual_channel_populate.py` & `bpkio_cli-1.9.1/bpkio_cli/commands/creators/virtual_channel_populate.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.9.0/bpkio_cli/commands/creators/virtual_channel_slot.py` & `bpkio_cli-1.9.1/bpkio_cli/commands/creators/virtual_channel_slot.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.9.0/bpkio_cli/commands/hello.py` & `bpkio_cli-1.9.1/bpkio_cli/commands/hello.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.9.0/bpkio_cli/commands/live_monitor.py` & `bpkio_cli-1.9.1/bpkio_cli/commands/live_monitor.py`

 * *Files 1% similar despite different names*

```diff
@@ -286,15 +286,17 @@
             # #EXT-X-DATERANGES
             for daterange in segment.dateranges:
                 mon.record_signal(
                     LiveSignal(
                         type=SignalType.DATERANGE,
                         appeared_at=stamp,
                         content=segment,
-                        signal_time=datetime.fromisoformat(daterange.start_date),
+                        signal_time=datetime.fromisoformat(
+                            daterange.start_date.replace("Z", "+00:00")
+                        ),
                         payload=(
                             daterange.scte35_out
                             or daterange.scte35_in
                             or daterange.scte35_cmd
                         ),
                         event_type=(
                             EventType.CUE_IN
```

### Comparing `bpkio_cli-1.9.0/bpkio_cli/commands/memory.py` & `bpkio_cli-1.9.1/bpkio_cli/commands/memory.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.9.0/bpkio_cli/commands/package.py` & `bpkio_cli-1.9.1/bpkio_cli/commands/package.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.9.0/bpkio_cli/commands/profiles.py` & `bpkio_cli-1.9.1/bpkio_cli/commands/profiles.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.9.0/bpkio_cli/commands/recorder.py` & `bpkio_cli-1.9.1/bpkio_cli/commands/recorder.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.9.0/bpkio_cli/commands/services.py` & `bpkio_cli-1.9.1/bpkio_cli/commands/services.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.9.0/bpkio_cli/commands/sources.py` & `bpkio_cli-1.9.1/bpkio_cli/commands/sources.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.9.0/bpkio_cli/commands/template_crud.py` & `bpkio_cli-1.9.1/bpkio_cli/commands/template_crud.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.9.0/bpkio_cli/commands/template_crud_slots.py` & `bpkio_cli-1.9.1/bpkio_cli/commands/template_crud_slots.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.9.0/bpkio_cli/commands/tenants.py` & `bpkio_cli-1.9.1/bpkio_cli/commands/tenants.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.9.0/bpkio_cli/commands/url.py` & `bpkio_cli-1.9.1/bpkio_cli/commands/url.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.9.0/bpkio_cli/core/app_context.py` & `bpkio_cli-1.9.1/bpkio_cli/core/app_context.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.9.0/bpkio_cli/core/click_helpers.py` & `bpkio_cli-1.9.1/bpkio_cli/core/click_helpers.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.9.0/bpkio_cli/core/config_provider.py` & `bpkio_cli-1.9.1/bpkio_cli/core/config_provider.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.9.0/bpkio_cli/core/initialize.py` & `bpkio_cli-1.9.1/bpkio_cli/core/initialize.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.9.0/bpkio_cli/core/logger.py` & `bpkio_cli-1.9.1/bpkio_cli/core/logger.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.9.0/bpkio_cli/core/packager.py` & `bpkio_cli-1.9.1/bpkio_cli/core/packager.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.9.0/bpkio_cli/core/resource_recorder.py` & `bpkio_cli-1.9.1/bpkio_cli/core/resource_recorder.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.9.0/bpkio_cli/core/resource_trail.py` & `bpkio_cli-1.9.1/bpkio_cli/core/resource_trail.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.9.0/bpkio_cli/core/response_handler.py` & `bpkio_cli-1.9.1/bpkio_cli/core/response_handler.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.9.0/bpkio_cli/core/session_recorder.py` & `bpkio_cli-1.9.1/bpkio_cli/core/session_recorder.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.9.0/bpkio_cli/utils/arrays.py` & `bpkio_cli-1.9.1/bpkio_cli/utils/arrays.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.9.0/bpkio_cli/utils/datetimes.py` & `bpkio_cli-1.9.1/bpkio_cli/utils/datetimes.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.9.0/bpkio_cli/utils/editor.py` & `bpkio_cli-1.9.1/bpkio_cli/utils/editor.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.9.0/bpkio_cli/utils/profile_maker.py` & `bpkio_cli-1.9.1/bpkio_cli/utils/profile_maker.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.9.0/bpkio_cli/utils/prompt.py` & `bpkio_cli-1.9.1/bpkio_cli/utils/prompt.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.9.0/bpkio_cli/utils/sounds.py` & `bpkio_cli-1.9.1/bpkio_cli/utils/sounds.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.9.0/bpkio_cli/utils/url_builders.py` & `bpkio_cli-1.9.1/bpkio_cli/utils/url_builders.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.9.0/bpkio_cli/utils/urls.py` & `bpkio_cli-1.9.1/bpkio_cli/utils/urls.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.9.0/bpkio_cli/writers/breadcrumbs.py` & `bpkio_cli-1.9.1/bpkio_cli/writers/breadcrumbs.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.9.0/bpkio_cli/writers/colorizer.py` & `bpkio_cli-1.9.1/bpkio_cli/writers/colorizer.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.9.0/bpkio_cli/writers/content_display.py` & `bpkio_cli-1.9.1/bpkio_cli/writers/content_display.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.9.0/bpkio_cli/writers/diff.py` & `bpkio_cli-1.9.1/bpkio_cli/writers/diff.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.9.0/bpkio_cli/writers/formatter.py` & `bpkio_cli-1.9.1/bpkio_cli/writers/formatter.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.9.0/bpkio_cli/writers/hls_formatter.py` & `bpkio_cli-1.9.1/bpkio_cli/writers/hls_formatter.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.9.0/bpkio_cli/writers/json_formatter.py` & `bpkio_cli-1.9.1/bpkio_cli/writers/json_formatter.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.9.0/bpkio_cli/writers/players.py` & `bpkio_cli-1.9.1/bpkio_cli/writers/players.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.9.0/bpkio_cli/writers/scte35.py` & `bpkio_cli-1.9.1/bpkio_cli/writers/scte35.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.9.0/bpkio_cli/writers/tables.py` & `bpkio_cli-1.9.1/bpkio_cli/writers/tables.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.9.0/bpkio_cli/writers/urls.py` & `bpkio_cli-1.9.1/bpkio_cli/writers/urls.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.9.0/bpkio_cli/writers/xml_formatter.py` & `bpkio_cli-1.9.1/bpkio_cli/writers/xml_formatter.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.9.0/pyproject.toml` & `bpkio_cli-1.9.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bpkio-cli"
-version = "1.9.0"
+version = "1.9.1"
 description = "A command line interface to the broadpeak.io APIs, with additional helpers"
 authors = ["Fabre Lambeau <fabre.lambeau@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "bpkio_cli" }]
 
 [tool.poetry-dynamic-versioning]
 enable = true
```

### Comparing `bpkio_cli-1.9.0/PKG-INFO` & `bpkio_cli-1.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bpkio-cli
-Version: 1.9.0
+Version: 1.9.1
 Summary: A command line interface to the broadpeak.io APIs, with additional helpers
 Author: Fabre Lambeau
 Author-email: fabre.lambeau@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

