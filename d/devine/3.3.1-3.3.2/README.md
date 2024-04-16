# Comparing `tmp/devine-3.3.1.tar.gz` & `tmp/devine-3.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devine-3.3.1.tar", max compression
+gzip compressed data, was "devine-3.3.2.tar", max compression
```

## Comparing `devine-3.3.1.tar` & `devine-3.3.2.tar`

### file list

```diff
@@ -1,69 +1,69 @@
--rw-r--r--   0        0        0    54605 2024-04-05 11:32:20.168872 devine-3.3.1/CHANGELOG.md
--rw-r--r--   0        0        0    35822 2024-04-05 11:32:20.168872 devine-3.3.1/LICENSE
--rw-r--r--   0        0        0    20080 2024-04-05 11:32:20.168872 devine-3.3.1/README.md
--rw-r--r--   0        0        0       80 2024-04-05 11:32:20.168872 devine-3.3.1/devine/__main__.py
--rw-r--r--   0        0        0        0 2024-04-05 11:32:20.168872 devine-3.3.1/devine/commands/__init__.py
--rw-r--r--   0        0        0     3254 2024-04-05 11:32:20.168872 devine-3.3.1/devine/commands/cfg.py
--rw-r--r--   0        0        0    45886 2024-04-05 11:32:20.168872 devine-3.3.1/devine/commands/dl.py
--rw-r--r--   0        0        0     2247 2024-04-05 11:32:20.168872 devine-3.3.1/devine/commands/env.py
--rw-r--r--   0        0        0     7986 2024-04-05 11:32:20.168872 devine-3.3.1/devine/commands/kv.py
--rw-r--r--   0        0        0     6574 2024-04-05 11:32:20.168872 devine-3.3.1/devine/commands/search.py
--rw-r--r--   0        0        0     1743 2024-04-05 11:32:20.168872 devine-3.3.1/devine/commands/serve.py
--rw-r--r--   0        0        0     9243 2024-04-05 11:32:20.168872 devine-3.3.1/devine/commands/util.py
--rw-r--r--   0        0        0     9920 2024-04-05 11:32:20.172872 devine-3.3.1/devine/commands/wvd.py
--rw-r--r--   0        0        0       22 2024-04-05 11:32:20.172872 devine-3.3.1/devine/core/__init__.py
--rw-r--r--   0        0        0     2857 2024-04-05 11:32:20.172872 devine-3.3.1/devine/core/__main__.py
--rw-r--r--   0        0        0     6195 2024-04-05 11:32:20.172872 devine-3.3.1/devine/core/cacher.py
--rw-r--r--   0        0        0     1215 2024-04-05 11:32:20.172872 devine-3.3.1/devine/core/commands.py
--rw-r--r--   0        0        0     4481 2024-04-05 11:32:20.172872 devine-3.3.1/devine/core/config.py
--rw-r--r--   0        0        0    15343 2024-04-05 11:32:20.172872 devine-3.3.1/devine/core/console.py
--rw-r--r--   0        0        0     1065 2024-04-05 11:32:20.172872 devine-3.3.1/devine/core/constants.py
--rw-r--r--   0        0        0     3380 2024-04-05 11:32:20.172872 devine-3.3.1/devine/core/credential.py
--rw-r--r--   0        0        0      159 2024-04-05 11:32:20.172872 devine-3.3.1/devine/core/downloaders/__init__.py
--rw-r--r--   0        0        0    13339 2024-04-05 11:32:20.172872 devine-3.3.1/devine/core/downloaders/aria2c.py
--rw-r--r--   0        0        0    11697 2024-04-05 11:32:20.172872 devine-3.3.1/devine/core/downloaders/curl_impersonate.py
--rw-r--r--   0        0        0    11930 2024-04-05 11:32:20.172872 devine-3.3.1/devine/core/downloaders/requests.py
--rw-r--r--   0        0        0      199 2024-04-05 11:32:20.172872 devine-3.3.1/devine/core/drm/__init__.py
--rw-r--r--   0        0        0     4020 2024-04-05 11:32:20.172872 devine-3.3.1/devine/core/drm/clearkey.py
--rw-r--r--   0        0        0    11898 2024-04-05 11:32:20.172872 devine-3.3.1/devine/core/drm/widevine.py
--rw-r--r--   0        0        0     2818 2024-04-05 11:32:20.172872 devine-3.3.1/devine/core/events.py
--rw-r--r--   0        0        0       71 2024-04-05 11:32:20.172872 devine-3.3.1/devine/core/manifests/__init__.py
--rw-r--r--   0        0        0    31280 2024-04-05 11:32:20.172872 devine-3.3.1/devine/core/manifests/dash.py
--rw-r--r--   0        0        0    28266 2024-04-05 11:32:20.172872 devine-3.3.1/devine/core/manifests/hls.py
--rw-r--r--   0        0        0      117 2024-04-05 11:32:20.172872 devine-3.3.1/devine/core/proxies/__init__.py
--rw-r--r--   0        0        0     1958 2024-04-05 11:32:20.172872 devine-3.3.1/devine/core/proxies/basic.py
--rw-r--r--   0        0        0     2290 2024-04-05 11:32:20.172872 devine-3.3.1/devine/core/proxies/hola.py
--rw-r--r--   0        0        0     5565 2024-04-05 11:32:20.172872 devine-3.3.1/devine/core/proxies/nordvpn.py
--rw-r--r--   0        0        0     1048 2024-04-05 11:32:20.172872 devine-3.3.1/devine/core/proxies/proxy.py
--rw-r--r--   0        0        0     1714 2024-04-05 11:32:20.172872 devine-3.3.1/devine/core/search_result.py
--rw-r--r--   0        0        0    12729 2024-04-05 11:32:20.172872 devine-3.3.1/devine/core/service.py
--rw-r--r--   0        0        0     3001 2024-04-05 11:32:20.172872 devine-3.3.1/devine/core/services.py
--rw-r--r--   0        0        0      298 2024-04-05 11:32:20.172872 devine-3.3.1/devine/core/titles/__init__.py
--rw-r--r--   0        0        0     8002 2024-04-05 11:32:20.172872 devine-3.3.1/devine/core/titles/episode.py
--rw-r--r--   0        0        0     5538 2024-04-05 11:32:20.172872 devine-3.3.1/devine/core/titles/movie.py
--rw-r--r--   0        0        0     4689 2024-04-05 11:32:20.172872 devine-3.3.1/devine/core/titles/song.py
--rw-r--r--   0        0        0     2595 2024-04-05 11:32:20.172872 devine-3.3.1/devine/core/titles/title.py
--rw-r--r--   0        0        0      277 2024-04-05 11:32:20.172872 devine-3.3.1/devine/core/tracks/__init__.py
--rw-r--r--   0        0        0     2132 2024-04-05 11:32:20.172872 devine-3.3.1/devine/core/tracks/attachment.py
--rw-r--r--   0        0        0     5001 2024-04-05 11:32:20.172872 devine-3.3.1/devine/core/tracks/audio.py
--rw-r--r--   0        0        0     2976 2024-04-05 11:32:20.172872 devine-3.3.1/devine/core/tracks/chapter.py
--rw-r--r--   0        0        0     5352 2024-04-05 11:32:20.172872 devine-3.3.1/devine/core/tracks/chapters.py
--rw-r--r--   0        0        0    23374 2024-04-05 11:32:20.172872 devine-3.3.1/devine/core/tracks/subtitle.py
--rw-r--r--   0        0        0    21612 2024-04-05 11:32:20.176872 devine-3.3.1/devine/core/tracks/track.py
--rw-r--r--   0        0        0    17269 2024-04-05 11:32:20.176872 devine-3.3.1/devine/core/tracks/tracks.py
--rw-r--r--   0        0        0    13118 2024-04-05 11:32:20.176872 devine-3.3.1/devine/core/tracks/video.py
--rw-r--r--   0        0        0    10741 2024-04-05 11:32:20.176872 devine-3.3.1/devine/core/utilities.py
--rw-r--r--   0        0        0        0 2024-04-05 11:32:20.176872 devine-3.3.1/devine/core/utils/__init__.py
--rw-r--r--   0        0        0     6227 2024-04-05 11:32:20.176872 devine-3.3.1/devine/core/utils/click_types.py
--rw-r--r--   0        0        0     1532 2024-04-05 11:32:20.176872 devine-3.3.1/devine/core/utils/collections.py
--rw-r--r--   0        0        0     3699 2024-04-05 11:32:20.176872 devine-3.3.1/devine/core/utils/sslciphers.py
--rw-r--r--   0        0        0      845 2024-04-05 11:32:20.176872 devine-3.3.1/devine/core/utils/subprocess.py
--rw-r--r--   0        0        0      791 2024-04-05 11:32:20.176872 devine-3.3.1/devine/core/utils/xml.py
--rw-r--r--   0        0        0     1711 2024-04-05 11:32:20.176872 devine-3.3.1/devine/core/vault.py
--rw-r--r--   0        0        0     2518 2024-04-05 11:32:20.176872 devine-3.3.1/devine/core/vaults.py
--rw-r--r--   0        0        0     6414 2024-04-05 11:32:20.176872 devine-3.3.1/devine/vaults/API.py
--rw-r--r--   0        0        0     8485 2024-04-05 11:32:20.176872 devine-3.3.1/devine/vaults/MySQL.py
--rw-r--r--   0        0        0     6076 2024-04-05 11:32:20.176872 devine-3.3.1/devine/vaults/SQLite.py
--rw-r--r--   0        0        0        0 2024-04-05 11:32:20.176872 devine-3.3.1/devine/vaults/__init__.py
--rw-r--r--   0        0        0     2650 2024-04-05 11:32:20.176872 devine-3.3.1/pyproject.toml
--rw-r--r--   0        0        0    22566 1970-01-01 00:00:00.000000 devine-3.3.1/PKG-INFO
+-rw-r--r--   0        0        0    55720 2024-04-16 05:07:34.820728 devine-3.3.2/CHANGELOG.md
+-rw-r--r--   0        0        0    35822 2024-04-16 05:07:34.820728 devine-3.3.2/LICENSE
+-rw-r--r--   0        0        0    20271 2024-04-16 05:07:34.820728 devine-3.3.2/README.md
+-rw-r--r--   0        0        0       80 2024-04-16 05:07:34.820728 devine-3.3.2/devine/__main__.py
+-rw-r--r--   0        0        0        0 2024-04-16 05:07:34.820728 devine-3.3.2/devine/commands/__init__.py
+-rw-r--r--   0        0        0     3293 2024-04-16 05:07:34.820728 devine-3.3.2/devine/commands/cfg.py
+-rw-r--r--   0        0        0    45886 2024-04-16 05:07:34.824728 devine-3.3.2/devine/commands/dl.py
+-rw-r--r--   0        0        0     2182 2024-04-16 05:07:34.824728 devine-3.3.2/devine/commands/env.py
+-rw-r--r--   0        0        0     7986 2024-04-16 05:07:34.824728 devine-3.3.2/devine/commands/kv.py
+-rw-r--r--   0        0        0     6574 2024-04-16 05:07:34.824728 devine-3.3.2/devine/commands/search.py
+-rw-r--r--   0        0        0     1743 2024-04-16 05:07:34.824728 devine-3.3.2/devine/commands/serve.py
+-rw-r--r--   0        0        0     9243 2024-04-16 05:07:34.824728 devine-3.3.2/devine/commands/util.py
+-rw-r--r--   0        0        0     9920 2024-04-16 05:07:34.824728 devine-3.3.2/devine/commands/wvd.py
+-rw-r--r--   0        0        0       22 2024-04-16 05:07:34.824728 devine-3.3.2/devine/core/__init__.py
+-rw-r--r--   0        0        0     2857 2024-04-16 05:07:34.824728 devine-3.3.2/devine/core/__main__.py
+-rw-r--r--   0        0        0     6195 2024-04-16 05:07:34.824728 devine-3.3.2/devine/core/cacher.py
+-rw-r--r--   0        0        0     1215 2024-04-16 05:07:34.824728 devine-3.3.2/devine/core/commands.py
+-rw-r--r--   0        0        0     4481 2024-04-16 05:07:34.824728 devine-3.3.2/devine/core/config.py
+-rw-r--r--   0        0        0    15343 2024-04-16 05:07:34.824728 devine-3.3.2/devine/core/console.py
+-rw-r--r--   0        0        0     1065 2024-04-16 05:07:34.824728 devine-3.3.2/devine/core/constants.py
+-rw-r--r--   0        0        0     3380 2024-04-16 05:07:34.824728 devine-3.3.2/devine/core/credential.py
+-rw-r--r--   0        0        0      159 2024-04-16 05:07:34.824728 devine-3.3.2/devine/core/downloaders/__init__.py
+-rw-r--r--   0        0        0    13339 2024-04-16 05:07:34.824728 devine-3.3.2/devine/core/downloaders/aria2c.py
+-rw-r--r--   0        0        0    11697 2024-04-16 05:07:34.824728 devine-3.3.2/devine/core/downloaders/curl_impersonate.py
+-rw-r--r--   0        0        0    11930 2024-04-16 05:07:34.824728 devine-3.3.2/devine/core/downloaders/requests.py
+-rw-r--r--   0        0        0      199 2024-04-16 05:07:34.824728 devine-3.3.2/devine/core/drm/__init__.py
+-rw-r--r--   0        0        0     4020 2024-04-16 05:07:34.824728 devine-3.3.2/devine/core/drm/clearkey.py
+-rw-r--r--   0        0        0    11898 2024-04-16 05:07:34.824728 devine-3.3.2/devine/core/drm/widevine.py
+-rw-r--r--   0        0        0     2818 2024-04-16 05:07:34.824728 devine-3.3.2/devine/core/events.py
+-rw-r--r--   0        0        0       71 2024-04-16 05:07:34.824728 devine-3.3.2/devine/core/manifests/__init__.py
+-rw-r--r--   0        0        0    31280 2024-04-16 05:07:34.824728 devine-3.3.2/devine/core/manifests/dash.py
+-rw-r--r--   0        0        0    28517 2024-04-16 05:07:34.824728 devine-3.3.2/devine/core/manifests/hls.py
+-rw-r--r--   0        0        0      117 2024-04-16 05:07:34.824728 devine-3.3.2/devine/core/proxies/__init__.py
+-rw-r--r--   0        0        0     1893 2024-04-16 05:07:34.824728 devine-3.3.2/devine/core/proxies/basic.py
+-rw-r--r--   0        0        0     2290 2024-04-16 05:07:34.824728 devine-3.3.2/devine/core/proxies/hola.py
+-rw-r--r--   0        0        0     5565 2024-04-16 05:07:34.824728 devine-3.3.2/devine/core/proxies/nordvpn.py
+-rw-r--r--   0        0        0     1048 2024-04-16 05:07:34.824728 devine-3.3.2/devine/core/proxies/proxy.py
+-rw-r--r--   0        0        0     1714 2024-04-16 05:07:34.824728 devine-3.3.2/devine/core/search_result.py
+-rw-r--r--   0        0        0    12729 2024-04-16 05:07:34.824728 devine-3.3.2/devine/core/service.py
+-rw-r--r--   0        0        0     3001 2024-04-16 05:07:34.824728 devine-3.3.2/devine/core/services.py
+-rw-r--r--   0        0        0      298 2024-04-16 05:07:34.824728 devine-3.3.2/devine/core/titles/__init__.py
+-rw-r--r--   0        0        0     8002 2024-04-16 05:07:34.824728 devine-3.3.2/devine/core/titles/episode.py
+-rw-r--r--   0        0        0     5538 2024-04-16 05:07:34.824728 devine-3.3.2/devine/core/titles/movie.py
+-rw-r--r--   0        0        0     4689 2024-04-16 05:07:34.824728 devine-3.3.2/devine/core/titles/song.py
+-rw-r--r--   0        0        0     2595 2024-04-16 05:07:34.824728 devine-3.3.2/devine/core/titles/title.py
+-rw-r--r--   0        0        0      277 2024-04-16 05:07:34.824728 devine-3.3.2/devine/core/tracks/__init__.py
+-rw-r--r--   0        0        0     2132 2024-04-16 05:07:34.828728 devine-3.3.2/devine/core/tracks/attachment.py
+-rw-r--r--   0        0        0     7412 2024-04-16 05:07:34.828728 devine-3.3.2/devine/core/tracks/audio.py
+-rw-r--r--   0        0        0     2976 2024-04-16 05:07:34.828728 devine-3.3.2/devine/core/tracks/chapter.py
+-rw-r--r--   0        0        0     5352 2024-04-16 05:07:34.828728 devine-3.3.2/devine/core/tracks/chapters.py
+-rw-r--r--   0        0        0    24647 2024-04-16 05:07:34.828728 devine-3.3.2/devine/core/tracks/subtitle.py
+-rw-r--r--   0        0        0    21612 2024-04-16 05:07:34.828728 devine-3.3.2/devine/core/tracks/track.py
+-rw-r--r--   0        0        0    17269 2024-04-16 05:07:34.828728 devine-3.3.2/devine/core/tracks/tracks.py
+-rw-r--r--   0        0        0    16638 2024-04-16 05:07:34.828728 devine-3.3.2/devine/core/tracks/video.py
+-rw-r--r--   0        0        0    10741 2024-04-16 05:07:34.828728 devine-3.3.2/devine/core/utilities.py
+-rw-r--r--   0        0        0        0 2024-04-16 05:07:34.828728 devine-3.3.2/devine/core/utils/__init__.py
+-rw-r--r--   0        0        0     6227 2024-04-16 05:07:34.828728 devine-3.3.2/devine/core/utils/click_types.py
+-rw-r--r--   0        0        0     1532 2024-04-16 05:07:34.828728 devine-3.3.2/devine/core/utils/collections.py
+-rw-r--r--   0        0        0     3699 2024-04-16 05:07:34.828728 devine-3.3.2/devine/core/utils/sslciphers.py
+-rw-r--r--   0        0        0      845 2024-04-16 05:07:34.828728 devine-3.3.2/devine/core/utils/subprocess.py
+-rw-r--r--   0        0        0      791 2024-04-16 05:07:34.828728 devine-3.3.2/devine/core/utils/xml.py
+-rw-r--r--   0        0        0     1711 2024-04-16 05:07:34.828728 devine-3.3.2/devine/core/vault.py
+-rw-r--r--   0        0        0     2518 2024-04-16 05:07:34.828728 devine-3.3.2/devine/core/vaults.py
+-rw-r--r--   0        0        0     6414 2024-04-16 05:07:34.828728 devine-3.3.2/devine/vaults/API.py
+-rw-r--r--   0        0        0     8485 2024-04-16 05:07:34.828728 devine-3.3.2/devine/vaults/MySQL.py
+-rw-r--r--   0        0        0     6076 2024-04-16 05:07:34.828728 devine-3.3.2/devine/vaults/SQLite.py
+-rw-r--r--   0        0        0        0 2024-04-16 05:07:34.828728 devine-3.3.2/devine/vaults/__init__.py
+-rw-r--r--   0        0        0     2496 2024-04-16 05:07:34.828728 devine-3.3.2/pyproject.toml
+-rw-r--r--   0        0        0    22752 1970-01-01 00:00:00.000000 devine-3.3.2/PKG-INFO
```

### Comparing `devine-3.3.1/CHANGELOG.md` & `devine-3.3.2/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,41 @@
 All notable changes to this project will be documented in this file.
 
 This project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 Versions [3.0.0] and older use a format based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 but versions thereafter use a custom changelog format using [git-cliff](https://git-cliff.org).
 
+## [3.3.2] - 2024-04-16
+
+### Bug Fixes
+
+- *Video*: Ensure track is supported in change_color_range()
+- *Video*: Optionalise constructor args, add doc-string & checks
+- *Audio*: Optionalise constructor args, add doc-string & checks
+- *Subtitle*: Optionalise constructor args, add doc-string & checks
+- *HLS*: Ensure playlist.stream_info.codecs exists before use
+- *HLS*: Ensure playlist.stream_info.resolution exists before use
+- *env*: List used config path, otherwise the default path
+- *cfg*: Use loaded config path instead of hardcoded default
+- *Basic*: Return None not Exception if no proxy configured
+
+### Changes
+
+- *Video*: Do not print "?"/"Unknown" values in str()
+- *Audio*: Do not print "?"/"Unknown" values in str()
+- *Subtitle*: Do not print "?"/"Unknown" values in str()
+- *Audio*: List lang after codec for consistency with other Tracks
+- *Video*: Return None if no m3u RANGE, not SDR
+- *env*: Use -- to indicate no config found/loaded
+
+### New Contributors
+
+- [retouching](https://github.com/retouching)
+
 ## [3.3.1] - 2024-04-05
 
 ### Features
 
 - *dl*: Add *new* --workers to set download threads/workers
 
 ### Bug Fixes
@@ -764,14 +791,15 @@
 - Fixed crash when adding a Cookie using `auth add` to a Service that has no directory yet.
 - Fixed crash when adding a Credential using `auth add` when it's the first ever credential, or first for the Service.
 
 ## [1.0.0] - 2023-02-06
 
 Initial public release under the name Devine.
 
+[3.3.2]: https://github.com/devine-dl/devine/releases/tag/v3.3.2
 [3.3.1]: https://github.com/devine-dl/devine/releases/tag/v3.3.1
 [3.3.0]: https://github.com/devine-dl/devine/releases/tag/v3.3.0
 [3.2.0]: https://github.com/devine-dl/devine/releases/tag/v3.2.0
 [3.1.0]: https://github.com/devine-dl/devine/releases/tag/v3.1.0
 [3.0.0]: https://github.com/devine-dl/devine/releases/tag/v3.0.0
 [2.2.0]: https://github.com/devine-dl/devine/releases/tag/v2.2.0
 [2.1.0]: https://github.com/devine-dl/devine/releases/tag/v2.1.0
```

### Comparing `devine-3.3.1/LICENSE` & `devine-3.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `devine-3.3.1/README.md` & `devine-3.3.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -338,14 +338,15 @@
 <a href="https://github.com/nyuszika7h"><img src="https://images.weserv.nl/?url=avatars.githubusercontent.com/u/482367?v=4&h=25&w=25&fit=cover&mask=circle&maxage=7d" alt="nyuszika7h"/></a>
 <a href="https://github.com/bccornfo"><img src="https://images.weserv.nl/?url=avatars.githubusercontent.com/u/98013276?v=4&h=25&w=25&fit=cover&mask=circle&maxage=7d" alt="bccornfo"/></a>
 <a href="https://github.com/Arias800"><img src="https://images.weserv.nl/?url=avatars.githubusercontent.com/u/24809312?v=4&h=25&w=25&fit=cover&mask=circle&maxage=7d" alt="Arias800"/></a>
 <a href="https://github.com/varyg1001"><img src="https://images.weserv.nl/?url=avatars.githubusercontent.com/u/88599103?v=4&h=25&w=25&fit=cover&mask=circle&maxage=7d" alt="varyg1001"/></a>
 <a href="https://github.com/Hollander-1908"><img src="https://images.weserv.nl/?url=avatars.githubusercontent.com/u/93162595?v=4&h=25&w=25&fit=cover&mask=circle&maxage=7d" alt="Hollander-1908"/></a>
 <a href="https://github.com/Shivelight"><img src="https://images.weserv.nl/?url=avatars.githubusercontent.com/u/20620780?v=4&h=25&w=25&fit=cover&mask=circle&maxage=7d" alt="Shivelight"/></a>
 <a href="https://github.com/knowhere01"><img src="https://images.weserv.nl/?url=avatars.githubusercontent.com/u/113712042?v=4&h=25&w=25&fit=cover&mask=circle&maxage=7d" alt="knowhere01"/></a>
+<a href="https://github.com/retouching"><img src="https://images.weserv.nl/?url=avatars.githubusercontent.com/u/33735357?v=4&h=25&w=25&fit=cover&mask=circle&maxage=7d" alt="retouching"/></a>
 
 ## Licensing
 
 This software is licensed under the terms of [GNU General Public License, Version 3.0](LICENSE).  
 You can find a copy of the license in the LICENSE file in the root folder.
 
 * * *
```

### Comparing `devine-3.3.1/devine/commands/cfg.py` & `devine-3.3.2/devine/commands/cfg.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import ast
 import logging
 import sys
 
 import click
 from ruamel.yaml import YAML
 
-from devine.core.config import config
+from devine.core.config import config, get_config_path
 from devine.core.constants import context_settings
 
 
 @click.command(
     short_help="Manage configuration values for the program and its services.",
     context_settings=context_settings)
 @click.argument("key", type=str, required=False)
@@ -32,23 +32,23 @@
         try:
             value = ast.literal_eval(value)
         except (ValueError, SyntaxError):
             pass  # probably a str without quotes or similar, assume it's a string value
 
     log = logging.getLogger("cfg")
 
-    config_path = config.directories.user_configs / config.filenames.root_config
-
     yaml, data = YAML(), None
     yaml.default_flow_style = False
-    if config_path.is_file():
+
+    config_path = get_config_path() or config.directories.user_configs / config.filenames.root_config
+    if config_path.exists():
         data = yaml.load(config_path)
 
     if not data:
-        log.warning(f"{config_path} has no configuration data, yet")
+        log.warning("No config file was found or it has no data, yet")
         # yaml.load() returns `None` if the input data is blank instead of a usable object
         # force a usable object by making one and removing the only item within it
         data = yaml.load("""__TEMP__: null""")
         del data["__TEMP__"]
 
     if list_:
         yaml.dump(data, sys.stdout)
```

### Comparing `devine-3.3.1/devine/commands/dl.py` & `devine-3.3.2/devine/commands/dl.py`

 * *Files identical despite different names*

### Comparing `devine-3.3.1/devine/commands/env.py` & `devine-3.3.2/devine/commands/env.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 import logging
 import shutil
 from typing import Optional
 
 import click
 
-from devine.core.config import config
+from devine.core.config import config, config_path
 from devine.core.constants import context_settings
 from devine.core.services import Services
 
 
 @click.group(short_help="Manage and configure the project environment.", context_settings=context_settings)
 def env() -> None:
     """Manage and configure the project environment."""
 
 
 @env.command()
 def info() -> None:
     """Displays information about the current environment."""
     log = logging.getLogger("env")
-    log.info(f"[Root Config]     : {config.directories.user_configs / config.filenames.root_config}")
-    log.info(f"[Cookies]         : {config.directories.cookies}")
-    log.info(f"[WVDs]            : {config.directories.wvds}")
-    log.info(f"[Cache]           : {config.directories.cache}")
-    log.info(f"[Logs]            : {config.directories.logs}")
-    log.info(f"[Temp Files]      : {config.directories.temp}")
-    log.info(f"[Downloads]       : {config.directories.downloads}")
+    log.info(f"[Config]     : {config_path or '--'}")
+    log.info(f"[Cookies]    : {config.directories.cookies}")
+    log.info(f"[WVDs]       : {config.directories.wvds}")
+    log.info(f"[Cache]      : {config.directories.cache}")
+    log.info(f"[Logs]       : {config.directories.logs}")
+    log.info(f"[Temp Files] : {config.directories.temp}")
+    log.info(f"[Downloads]  : {config.directories.downloads}")
 
 
 @env.group(name="clear", short_help="Clear an environment directory.", context_settings=context_settings)
 def clear() -> None:
     """Clear an environment directory."""
```

### Comparing `devine-3.3.1/devine/commands/kv.py` & `devine-3.3.2/devine/commands/kv.py`

 * *Files identical despite different names*

### Comparing `devine-3.3.1/devine/commands/search.py` & `devine-3.3.2/devine/commands/search.py`

 * *Files identical despite different names*

### Comparing `devine-3.3.1/devine/commands/serve.py` & `devine-3.3.2/devine/commands/serve.py`

 * *Files identical despite different names*

### Comparing `devine-3.3.1/devine/commands/util.py` & `devine-3.3.2/devine/commands/util.py`

 * *Files identical despite different names*

### Comparing `devine-3.3.1/devine/commands/wvd.py` & `devine-3.3.2/devine/commands/wvd.py`

 * *Files identical despite different names*

### Comparing `devine-3.3.1/devine/core/__main__.py` & `devine-3.3.2/devine/core/__main__.py`

 * *Files identical despite different names*

### Comparing `devine-3.3.1/devine/core/cacher.py` & `devine-3.3.2/devine/core/cacher.py`

 * *Files identical despite different names*

### Comparing `devine-3.3.1/devine/core/commands.py` & `devine-3.3.2/devine/core/commands.py`

 * *Files identical despite different names*

### Comparing `devine-3.3.1/devine/core/config.py` & `devine-3.3.2/devine/core/config.py`

 * *Files identical despite different names*

### Comparing `devine-3.3.1/devine/core/console.py` & `devine-3.3.2/devine/core/console.py`

 * *Files identical despite different names*

### Comparing `devine-3.3.1/devine/core/constants.py` & `devine-3.3.2/devine/core/constants.py`

 * *Files identical despite different names*

### Comparing `devine-3.3.1/devine/core/credential.py` & `devine-3.3.2/devine/core/credential.py`

 * *Files identical despite different names*

### Comparing `devine-3.3.1/devine/core/downloaders/aria2c.py` & `devine-3.3.2/devine/core/downloaders/aria2c.py`

 * *Files identical despite different names*

### Comparing `devine-3.3.1/devine/core/downloaders/curl_impersonate.py` & `devine-3.3.2/devine/core/downloaders/curl_impersonate.py`

 * *Files identical despite different names*

### Comparing `devine-3.3.1/devine/core/downloaders/requests.py` & `devine-3.3.2/devine/core/downloaders/requests.py`

 * *Files identical despite different names*

### Comparing `devine-3.3.1/devine/core/drm/clearkey.py` & `devine-3.3.2/devine/core/drm/clearkey.py`

 * *Files identical despite different names*

### Comparing `devine-3.3.1/devine/core/drm/widevine.py` & `devine-3.3.2/devine/core/drm/widevine.py`

 * *Files identical despite different names*

### Comparing `devine-3.3.1/devine/core/events.py` & `devine-3.3.2/devine/core/events.py`

 * *Files identical despite different names*

### Comparing `devine-3.3.1/devine/core/manifests/dash.py` & `devine-3.3.2/devine/core/manifests/dash.py`

 * *Files identical despite different names*

### Comparing `devine-3.3.1/devine/core/manifests/hls.py` & `devine-3.3.2/devine/core/manifests/hls.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,42 +97,46 @@
             audio_group = playlist.stream_info.audio
             if audio_group:
                 audio_codec = Audio.Codec.from_codecs(playlist.stream_info.codecs)
                 audio_codecs_by_group_id[audio_group] = audio_codec
 
             try:
                 # TODO: Any better way to figure out the primary track type?
-                Video.Codec.from_codecs(playlist.stream_info.codecs)
+                if playlist.stream_info.codecs:
+                    Video.Codec.from_codecs(playlist.stream_info.codecs)
             except ValueError:
                 primary_track_type = Audio
             else:
                 primary_track_type = Video
 
             tracks.add(primary_track_type(
                 id_=hex(crc32(str(playlist).encode()))[2:],
                 url=urljoin(playlist.base_uri, playlist.uri),
-                codec=primary_track_type.Codec.from_codecs(playlist.stream_info.codecs),
+                codec=(
+                    primary_track_type.Codec.from_codecs(playlist.stream_info.codecs)
+                    if playlist.stream_info.codecs else None
+                ),
                 language=language,  # HLS manifests do not seem to have language info
                 is_original_lang=True,  # TODO: All we can do is assume Yes
                 bitrate=playlist.stream_info.average_bandwidth or playlist.stream_info.bandwidth,
                 descriptor=Video.Descriptor.HLS,
                 drm=session_drm,
                 data={
                     "hls": {
                         "playlist": playlist
                     }
                 },
                 # video track args
                 **(dict(
                     range_=Video.Range.DV if any(
                         codec.split(".")[0] in ("dva1", "dvav", "dvhe", "dvh1")
-                        for codec in playlist.stream_info.codecs.lower().split(",")
+                        for codec in (playlist.stream_info.codecs or "").lower().split(",")
                     ) else Video.Range.from_m3u_range_tag(playlist.stream_info.video_range),
-                    width=playlist.stream_info.resolution[0],
-                    height=playlist.stream_info.resolution[1],
+                    width=playlist.stream_info.resolution[0] if playlist.stream_info.resolution else None,
+                    height=playlist.stream_info.resolution[1] if playlist.stream_info.resolution else None,
                     fps=playlist.stream_info.frame_rate
                 ) if primary_track_type is Video else {})
             ))
 
         for media in self.manifest.media:
             if not media.uri:
                 continue
```

### Comparing `devine-3.3.1/devine/core/proxies/basic.py` & `devine-3.3.2/devine/core/proxies/basic.py`

 * *Files 20% similar despite different names*

```diff
@@ -31,15 +31,15 @@
             raise ValueError(f"The query \"{query}\" was not recognized...")
 
         country_code = match.group(1)
         entry = match.group(2)
 
         servers: Optional[Union[str, list[str]]] = self.countries.get(country_code)
         if not servers:
-            raise ValueError(f"There's no proxies configured for \"{country_code}\"...")
+            return None
 
         if isinstance(servers, str):
             proxy = servers
         elif entry:
             try:
                 proxy = servers[int(entry) - 1]
             except IndexError:
```

### Comparing `devine-3.3.1/devine/core/proxies/hola.py` & `devine-3.3.2/devine/core/proxies/hola.py`

 * *Files identical despite different names*

### Comparing `devine-3.3.1/devine/core/proxies/nordvpn.py` & `devine-3.3.2/devine/core/proxies/nordvpn.py`

 * *Files identical despite different names*

### Comparing `devine-3.3.1/devine/core/proxies/proxy.py` & `devine-3.3.2/devine/core/proxies/proxy.py`

 * *Files identical despite different names*

### Comparing `devine-3.3.1/devine/core/search_result.py` & `devine-3.3.2/devine/core/search_result.py`

 * *Files identical despite different names*

### Comparing `devine-3.3.1/devine/core/service.py` & `devine-3.3.2/devine/core/service.py`

 * *Files identical despite different names*

### Comparing `devine-3.3.1/devine/core/services.py` & `devine-3.3.2/devine/core/services.py`

 * *Files identical despite different names*

### Comparing `devine-3.3.1/devine/core/titles/episode.py` & `devine-3.3.2/devine/core/titles/episode.py`

 * *Files identical despite different names*

### Comparing `devine-3.3.1/devine/core/titles/movie.py` & `devine-3.3.2/devine/core/titles/movie.py`

 * *Files identical despite different names*

### Comparing `devine-3.3.1/devine/core/titles/song.py` & `devine-3.3.2/devine/core/titles/song.py`

 * *Files identical despite different names*

### Comparing `devine-3.3.1/devine/core/titles/title.py` & `devine-3.3.2/devine/core/titles/title.py`

 * *Files identical despite different names*

### Comparing `devine-3.3.1/devine/core/tracks/attachment.py` & `devine-3.3.2/devine/core/tracks/attachment.py`

 * *Files identical despite different names*

### Comparing `devine-3.3.1/devine/core/tracks/chapter.py` & `devine-3.3.2/devine/core/tracks/chapter.py`

 * *Files identical despite different names*

### Comparing `devine-3.3.1/devine/core/tracks/chapters.py` & `devine-3.3.2/devine/core/tracks/chapters.py`

 * *Files identical despite different names*

### Comparing `devine-3.3.1/devine/core/tracks/subtitle.py` & `devine-3.3.2/devine/core/tracks/subtitle.py`

 * *Files 3% similar despite different names*

```diff
@@ -70,30 +70,30 @@
             profile = profile.lower().strip()
             if profile.startswith("webvtt"):
                 return Subtitle.Codec.WebVTT
             if profile.startswith("dfxp"):
                 return Subtitle.Codec.TimedTextMarkupLang
             raise ValueError(f"The Content Profile '{profile}' is not a supported Subtitle Codec")
 
-    def __init__(self, *args: Any, codec: Subtitle.Codec, cc: bool = False, sdh: bool = False, forced: bool = False,
-                 **kwargs: Any):
+    def __init__(
+        self,
+        *args: Any,
+        codec: Optional[Subtitle.Codec] = None,
+        cc: bool = False,
+        sdh: bool = False,
+        forced: bool = False,
+        **kwargs: Any
+    ):
         """
-        Information on Subtitle Types:
-            https://bit.ly/2Oe4fLC (3PlayMedia Blog on SUB vs CC vs SDH).
-            However, I wouldn't pay much attention to the claims about SDH needing to
-            be in the original source language. It's logically not true.
-
-            CC == Closed Captions. Source: Basically every site.
-            SDH = Subtitles for the Deaf or Hard-of-Hearing. Source: Basically every site.
-            HOH = Exact same as SDH. Is a term used in the UK. Source: https://bit.ly/2PGJatz (ICO UK)
-
-            More in-depth information, examples, and stuff to look for can be found in the Parameter
-            explanation list below.
+        Create a new Subtitle track object.
 
         Parameters:
+            codec: A Subtitle.Codec enum representing the subtitle format.
+                If not specified, MediaInfo will be used to retrieve the format
+                once the track has been downloaded.
             cc: Closed Caption.
                 - Intended as if you couldn't hear the audio at all.
                 - Can have Sound as well as Dialogue, but doesn't have to.
                 - Original source would be from an EIA-CC encoded stream. Typically all
                   upper-case characters.
                 Indicators of it being CC without knowing original source:
                   - Extracted with CCExtractor, or
@@ -121,28 +121,65 @@
                     Forced tracks are recommended by the Matroska Spec to be played if
                      the player's current playback audio language matches a subtitle
                      marked as "forced".
                     However, that doesn't mean every player works like this but there is
                      no other way to reliably work with Forced subtitles where multiple
                      forced subtitles may be in the output file. Just know what to expect
                      with "forced" subtitles.
+
+        Note: If codec is not specified some checks may be skipped or assume a value.
+        Specifying as much information as possible is highly recommended.
+
+        Information on Subtitle Types:
+            https://bit.ly/2Oe4fLC (3PlayMedia Blog on SUB vs CC vs SDH).
+            However, I wouldn't pay much attention to the claims about SDH needing to
+            be in the original source language. It's logically not true.
+
+            CC == Closed Captions. Source: Basically every site.
+            SDH = Subtitles for the Deaf or Hard-of-Hearing. Source: Basically every site.
+            HOH = Exact same as SDH. Is a term used in the UK. Source: https://bit.ly/2PGJatz (ICO UK)
+
+            More in-depth information, examples, and stuff to look for can be found in the Parameter
+            explanation list above.
         """
         super().__init__(*args, **kwargs)
+
+        if not isinstance(codec, (Subtitle.Codec, type(None))):
+            raise TypeError(f"Expected codec to be a {Subtitle.Codec}, not {codec!r}")
+        if not isinstance(cc, (bool, int)) or (isinstance(cc, int) and cc not in (0, 1)):
+            raise TypeError(f"Expected cc to be a {bool} or bool-like {int}, not {cc!r}")
+        if not isinstance(sdh, (bool, int)) or (isinstance(sdh, int) and sdh not in (0, 1)):
+            raise TypeError(f"Expected sdh to be a {bool} or bool-like {int}, not {sdh!r}")
+        if not isinstance(forced, (bool, int)) or (isinstance(forced, int) and forced not in (0, 1)):
+            raise TypeError(f"Expected forced to be a {bool} or bool-like {int}, not {forced!r}")
+
         self.codec = codec
+
         self.cc = bool(cc)
         self.sdh = bool(sdh)
+        self.forced = bool(forced)
+
         if self.cc and self.sdh:
             raise ValueError("A text track cannot be both CC and SDH.")
-        self.forced = bool(forced)
-        if (self.cc or self.sdh) and self.forced:
+
+        if self.forced and (self.cc or self.sdh):
             raise ValueError("A text track cannot be CC/SDH as well as Forced.")
 
+        # TODO: Migrate to new event observer system
         # Called after Track has been converted to another format
         self.OnConverted: Optional[Callable[[Subtitle.Codec], None]] = None
 
+    def __str__(self) -> str:
+        return " | ".join(filter(bool, [
+            "SUB",
+            f"[{self.codec.value}]" if self.codec else None,
+            str(self.language),
+            self.get_track_name()
+        ]))
+
     def get_track_name(self) -> Optional[str]:
         """Return the base Track Name."""
         track_name = super().get_track_name() or ""
         flag = self.cc and "CC" or self.sdh and "SDH" or self.forced and "Forced"
         if flag:
             if track_name:
                 flag = f" ({flag})"
@@ -521,17 +558,9 @@
                 "/encoding:utf8",
                 "/overwrite"
             ],
             check=True,
             stdout=subprocess.DEVNULL
         )
 
-    def __str__(self) -> str:
-        return " | ".join(filter(bool, [
-            "SUB",
-            f"[{self.codec.value}]",
-            str(self.language),
-            self.get_track_name()
-        ]))
-
 
 __all__ = ("Subtitle",)
```

### Comparing `devine-3.3.1/devine/core/tracks/track.py` & `devine-3.3.2/devine/core/tracks/track.py`

 * *Files identical despite different names*

### Comparing `devine-3.3.1/devine/core/tracks/tracks.py` & `devine-3.3.2/devine/core/tracks/tracks.py`

 * *Files identical despite different names*

### Comparing `devine-3.3.1/devine/core/tracks/video.py` & `devine-3.3.2/devine/core/tracks/video.py`

 * *Files 19% similar despite different names*

```diff
@@ -137,51 +137,129 @@
                 return Video.Range.HDR10
             elif transfer == Transfer.BT_2100_HLG:
                 return Video.Range.HLG
             else:
                 return Video.Range.SDR
 
         @staticmethod
-        def from_m3u_range_tag(tag: str) -> Video.Range:
+        def from_m3u_range_tag(tag: str) -> Optional[Video.Range]:
             tag = (tag or "").upper().replace('"', '').strip()
-            if not tag or tag == "SDR":
+            if not tag:
+                return None
+            if tag == "SDR":
                 return Video.Range.SDR
             elif tag == "PQ":
                 return Video.Range.HDR10  # technically could be any PQ-transfer range
             elif tag == "HLG":
                 return Video.Range.HLG
             # for some reason there's no Dolby Vision info tag
             raise ValueError(f"The M3U Range Tag '{tag}' is not a supported Video Range")
 
-    def __init__(self, *args: Any, codec: Video.Codec, range_: Video.Range, bitrate: Union[str, int, float],
-                 width: int, height: int, fps: Optional[Union[str, int, float]] = None, **kwargs: Any) -> None:
+    def __init__(
+        self,
+        *args: Any,
+        codec: Optional[Video.Codec] = None,
+        range_: Optional[Video.Range] = None,
+        bitrate: Optional[Union[str, int, float]] = None,
+        width: Optional[int] = None,
+        height: Optional[int] = None,
+        fps: Optional[Union[str, int, float]] = None,
+        **kwargs: Any
+    ) -> None:
+        """
+        Create a new Video track object.
+
+        Parameters:
+            codec: A Video.Codec enum representing the video codec.
+                If not specified, MediaInfo will be used to retrieve the codec
+                once the track has been downloaded.
+            range_: A Video.Range enum representing the video color range.
+                Defaults to SDR if not specified.
+            bitrate: A number or float representing the average bandwidth in bytes/s.
+                Float values are rounded up to the nearest integer.
+            width: The horizontal resolution of the video.
+            height: The vertical resolution of the video.
+            fps: A number, float, or string representing the frames/s of the video.
+                Strings may represent numbers, floats, or a fraction (num/den).
+                All strings will be cast to either a number or float.
+
+        Note: If codec, bitrate, width, height, or fps is not specified some checks
+        may be skipped or assume a value. Specifying as much information as possible
+        is highly recommended.
+        """
         super().__init__(*args, **kwargs)
-        # required
+
+        if not isinstance(codec, (Video.Codec, type(None))):
+            raise TypeError(f"Expected codec to be a {Video.Codec}, not {codec!r}")
+        if not isinstance(range_, (Video.Range, type(None))):
+            raise TypeError(f"Expected range_ to be a {Video.Range}, not {range_!r}")
+        if not isinstance(bitrate, (str, int, float, type(None))):
+            raise TypeError(f"Expected bitrate to be a {str}, {int}, or {float}, not {bitrate!r}")
+        if not isinstance(width, (int, str, type(None))):
+            raise TypeError(f"Expected width to be a {int}, not {width!r}")
+        if not isinstance(height, (int, str, type(None))):
+            raise TypeError(f"Expected height to be a {int}, not {height!r}")
+        if not isinstance(fps, (str, int, float, type(None))):
+            raise TypeError(f"Expected fps to be a {str}, {int}, or {float}, not {fps!r}")
+
         self.codec = codec
         self.range = range_ or Video.Range.SDR
-        self.bitrate = int(math.ceil(float(bitrate))) if bitrate else None
-        self.width = int(width)
-        self.height = int(height)
-        # optional
-        self.fps = FPS.parse(str(fps)) if fps else None
+
+        try:
+            self.bitrate = int(math.ceil(float(bitrate))) if bitrate else None
+        except (ValueError, TypeError) as e:
+            raise ValueError(f"Expected bitrate to be a number or float, {e}")
+
+        try:
+            self.width = int(width or 0) or None
+        except ValueError as e:
+            raise ValueError(f"Expected width to be a number, not {width!r}, {e}")
+
+        try:
+            self.height = int(height or 0) or None
+        except ValueError as e:
+            raise ValueError(f"Expected height to be a number, not {height!r}, {e}")
+
+        try:
+            self.fps = (FPS.parse(str(fps)) or None) if fps else None
+        except Exception as e:
+            raise ValueError(
+                "Expected fps to be a number, float, or a string as numerator/denominator form, " +
+                str(e)
+            )
 
     def __str__(self) -> str:
-        fps = f"{self.fps:.3f}" if self.fps else "Unknown"
         return " | ".join(filter(bool, [
             "VID",
-            f"[{self.codec.value}, {self.range.name}]",
+            "[" + (", ".join(filter(bool, [
+                self.codec.value if self.codec else None,
+                self.range.name
+            ]))) + "]",
             str(self.language),
-            f"{self.width}x{self.height} @ {self.bitrate // 1000 if self.bitrate else '?'} kb/s, {fps} FPS",
+            ", ".join(filter(bool, [
+                " @ ".join(filter(bool, [
+                    f"{self.width}x{self.height}" if self.width and self.height else None,
+                    f"{self.bitrate // 1000} kb/s" if self.bitrate else None
+                ])),
+                f"{self.fps:.3f} FPS" if self.fps else None
+            ])),
             self.edition
         ]))
 
     def change_color_range(self, range_: int) -> None:
         """Change the Video's Color Range to Limited (0) or Full (1)."""
         if not self.path or not self.path.exists():
-            raise ValueError("Cannot repackage a Track that has not been downloaded.")
+            raise ValueError("Cannot change the color range flag on a Video that has not been downloaded.")
+        if not self.codec:
+            raise ValueError("Cannot change the color range flag on a Video that has no codec specified.")
+        if self.codec not in (Video.Codec.AVC, Video.Codec.HEVC):
+            raise NotImplementedError(
+                "Cannot change the color range flag on this Video as "
+                f"it's codec, {self.codec.value}, is not yet supported."
+            )
 
         executable = get_binary_path("ffmpeg")
         if not executable:
             raise EnvironmentError("FFmpeg executable \"ffmpeg\" was not found but is required for this call.")
 
         filter_key = {
             Video.Codec.AVC: "h264_metadata",
```

### Comparing `devine-3.3.1/devine/core/utilities.py` & `devine-3.3.2/devine/core/utilities.py`

 * *Files identical despite different names*

### Comparing `devine-3.3.1/devine/core/utils/click_types.py` & `devine-3.3.2/devine/core/utils/click_types.py`

 * *Files identical despite different names*

### Comparing `devine-3.3.1/devine/core/utils/collections.py` & `devine-3.3.2/devine/core/utils/collections.py`

 * *Files identical despite different names*

### Comparing `devine-3.3.1/devine/core/utils/sslciphers.py` & `devine-3.3.2/devine/core/utils/sslciphers.py`

 * *Files identical despite different names*

### Comparing `devine-3.3.1/devine/core/utils/subprocess.py` & `devine-3.3.2/devine/core/utils/subprocess.py`

 * *Files identical despite different names*

### Comparing `devine-3.3.1/devine/core/utils/xml.py` & `devine-3.3.2/devine/core/utils/xml.py`

 * *Files identical despite different names*

### Comparing `devine-3.3.1/devine/core/vault.py` & `devine-3.3.2/devine/core/vault.py`

 * *Files identical despite different names*

### Comparing `devine-3.3.1/devine/core/vaults.py` & `devine-3.3.2/devine/core/vaults.py`

 * *Files identical despite different names*

### Comparing `devine-3.3.1/devine/vaults/API.py` & `devine-3.3.2/devine/vaults/API.py`

 * *Files identical despite different names*

### Comparing `devine-3.3.1/devine/vaults/MySQL.py` & `devine-3.3.2/devine/vaults/MySQL.py`

 * *Files identical despite different names*

### Comparing `devine-3.3.1/devine/vaults/SQLite.py` & `devine-3.3.2/devine/vaults/SQLite.py`

 * *Files identical despite different names*

### Comparing `devine-3.3.1/pyproject.toml` & `devine-3.3.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "devine"
-version = "3.3.1"
+version = "3.3.2"
 description = "Modular Movie, TV, and Music Archival Software."
 license = "GPL-3.0-only"
 authors = ["rlaphoenix <rlaphoenix@pm.me>"]
 readme = "README.md"
 homepage = "https://github.com/devine-dl/devine"
 repository = "https://github.com/devine-dl/devine"
 keywords = ["python", "downloader", "drm", "widevine"]
@@ -35,20 +35,20 @@
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
 appdirs = "^1.4.4"
 Brotli = "^1.1.0"
 click = "^8.1.7"
 construct = "^2.8.8"
 crccheck = "^1.3.0"
-jsonpickle = "^3.0.3"
+jsonpickle = "^3.0.4"
 langcodes = { extras = ["data"], version = "^3.3.0" }
 lxml = "^5.2.1"
 pproxy = "^2.7.9"
 protobuf = "^4.25.3"
-pycaption = "^2.2.4"
+pycaption = "^2.2.6"
 pycryptodomex = "^3.20.0"
 pyjwt = "^2.8.0"
 pymediainfo = "^6.1.0"
 pymp4 = "^1.4.0"
 pymysql = "^1.1.0"
 pywidevine = { extras = ["serve"], version = "^1.8.0" }
 PyYAML = "^6.0.1"
@@ -58,28 +58,26 @@
 "ruamel.yaml" = "^0.18.6"
 sortedcontainers = "^2.4.0"
 subtitle-filter = "^1.4.9"
 Unidecode = "^1.3.8"
 urllib3 = "^2.2.1"
 chardet = "^5.2.0"
 curl-cffi = "^0.6.2"
-# Temporary explicit versions of these langcodes dependencies as language-data v1.1
-# uses marisa-trie v0.7.8 which doesn't have Python 3.12 wheels.
-language-data = "^1.2.0.dev3"
+language-data = "^1.2.0"
 marisa-trie = "^1.1.0"
 
 [tool.poetry.dev-dependencies]
 pre-commit = "^3.7.0"
 mypy = "^1.9.0"
 mypy-protobuf = "^3.6.0"
-types-protobuf = "^4.24.0.20240311"
+types-protobuf = "^4.24.0.20240408"
 types-PyMySQL = "^1.1.0.1"
-types-requests = "^2.31.0.20240403"
+types-requests = "^2.31.0.20240406"
 isort = "^5.13.2"
-ruff = "~0.3.5"
+ruff = "~0.3.7"
 
 [tool.poetry.scripts]
 devine = "devine.core.__main__:main"
 
 [tool.ruff]
 force-exclude = true
 line-length = 120
```

### Comparing `devine-3.3.1/PKG-INFO` & `devine-3.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devine
-Version: 3.3.1
+Version: 3.3.2
 Summary: Modular Movie, TV, and Music Archival Software.
 Home-page: https://github.com/devine-dl/devine
 License: GPL-3.0-only
 Keywords: python,downloader,drm,widevine
 Author: rlaphoenix
 Author-email: rlaphoenix@pm.me
 Requires-Python: >=3.9,<4.0
@@ -25,22 +25,22 @@
 Requires-Dist: Unidecode (>=1.3.8,<2.0.0)
 Requires-Dist: appdirs (>=1.4.4,<2.0.0)
 Requires-Dist: chardet (>=5.2.0,<6.0.0)
 Requires-Dist: click (>=8.1.7,<9.0.0)
 Requires-Dist: construct (>=2.8.8,<3.0.0)
 Requires-Dist: crccheck (>=1.3.0,<2.0.0)
 Requires-Dist: curl-cffi (>=0.6.2,<0.7.0)
-Requires-Dist: jsonpickle (>=3.0.3,<4.0.0)
+Requires-Dist: jsonpickle (>=3.0.4,<4.0.0)
 Requires-Dist: langcodes[data] (>=3.3.0,<4.0.0)
-Requires-Dist: language-data (>=1.2.0.dev3,<2.0.0)
+Requires-Dist: language-data (>=1.2.0,<2.0.0)
 Requires-Dist: lxml (>=5.2.1,<6.0.0)
 Requires-Dist: marisa-trie (>=1.1.0,<2.0.0)
 Requires-Dist: pproxy (>=2.7.9,<3.0.0)
 Requires-Dist: protobuf (>=4.25.3,<5.0.0)
-Requires-Dist: pycaption (>=2.2.4,<3.0.0)
+Requires-Dist: pycaption (>=2.2.6,<3.0.0)
 Requires-Dist: pycryptodomex (>=3.20.0,<4.0.0)
 Requires-Dist: pyjwt (>=2.8.0,<3.0.0)
 Requires-Dist: pymediainfo (>=6.1.0,<7.0.0)
 Requires-Dist: pymp4 (>=1.4.0,<2.0.0)
 Requires-Dist: pymysql (>=1.1.0,<2.0.0)
 Requires-Dist: pywidevine[serve] (>=1.8.0,<2.0.0)
 Requires-Dist: requests[socks] (>=2.31.0,<3.0.0)
@@ -396,14 +396,15 @@
 <a href="https://github.com/nyuszika7h"><img src="https://images.weserv.nl/?url=avatars.githubusercontent.com/u/482367?v=4&h=25&w=25&fit=cover&mask=circle&maxage=7d" alt="nyuszika7h"/></a>
 <a href="https://github.com/bccornfo"><img src="https://images.weserv.nl/?url=avatars.githubusercontent.com/u/98013276?v=4&h=25&w=25&fit=cover&mask=circle&maxage=7d" alt="bccornfo"/></a>
 <a href="https://github.com/Arias800"><img src="https://images.weserv.nl/?url=avatars.githubusercontent.com/u/24809312?v=4&h=25&w=25&fit=cover&mask=circle&maxage=7d" alt="Arias800"/></a>
 <a href="https://github.com/varyg1001"><img src="https://images.weserv.nl/?url=avatars.githubusercontent.com/u/88599103?v=4&h=25&w=25&fit=cover&mask=circle&maxage=7d" alt="varyg1001"/></a>
 <a href="https://github.com/Hollander-1908"><img src="https://images.weserv.nl/?url=avatars.githubusercontent.com/u/93162595?v=4&h=25&w=25&fit=cover&mask=circle&maxage=7d" alt="Hollander-1908"/></a>
 <a href="https://github.com/Shivelight"><img src="https://images.weserv.nl/?url=avatars.githubusercontent.com/u/20620780?v=4&h=25&w=25&fit=cover&mask=circle&maxage=7d" alt="Shivelight"/></a>
 <a href="https://github.com/knowhere01"><img src="https://images.weserv.nl/?url=avatars.githubusercontent.com/u/113712042?v=4&h=25&w=25&fit=cover&mask=circle&maxage=7d" alt="knowhere01"/></a>
+<a href="https://github.com/retouching"><img src="https://images.weserv.nl/?url=avatars.githubusercontent.com/u/33735357?v=4&h=25&w=25&fit=cover&mask=circle&maxage=7d" alt="retouching"/></a>
 
 ## Licensing
 
 This software is licensed under the terms of [GNU General Public License, Version 3.0](LICENSE).  
 You can find a copy of the license in the LICENSE file in the root folder.
 
 * * *
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: devine Version: 3.3.1 Summary: Modular Movie, TV,
+Metadata-Version: 2.1 Name: devine Version: 3.3.2 Summary: Modular Movie, TV,
 and Music Archival Software. Home-page: https://github.com/devine-dl/devine
 License: GPL-3.0-only Keywords: python,downloader,drm,widevine Author:
 rlaphoenix Author-email: rlaphoenix@pm.me Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop Classifier: License :: OSI
 Approved :: GNU General Public License v3 (GPLv3) Classifier: Natural Language
 :: English Classifier: Operating System :: OS Independent Classifier:
@@ -11,31 +11,31 @@
 Programming Language :: Python :: 3.11 Classifier: Topic :: Multimedia :: Video
 Classifier: Topic :: Security :: Cryptography Requires-Dist: Brotli
 (>=1.1.0,<2.0.0) Requires-Dist: PyYAML (>=6.0.1,<7.0.0) Requires-Dist:
 Unidecode (>=1.3.8,<2.0.0) Requires-Dist: appdirs (>=1.4.4,<2.0.0) Requires-
 Dist: chardet (>=5.2.0,<6.0.0) Requires-Dist: click (>=8.1.7,<9.0.0) Requires-
 Dist: construct (>=2.8.8,<3.0.0) Requires-Dist: crccheck (>=1.3.0,<2.0.0)
 Requires-Dist: curl-cffi (>=0.6.2,<0.7.0) Requires-Dist: jsonpickle
-(>=3.0.3,<4.0.0) Requires-Dist: langcodes[data] (>=3.3.0,<4.0.0) Requires-Dist:
-language-data (>=1.2.0.dev3,<2.0.0) Requires-Dist: lxml (>=5.2.1,<6.0.0)
-Requires-Dist: marisa-trie (>=1.1.0,<2.0.0) Requires-Dist: pproxy
-(>=2.7.9,<3.0.0) Requires-Dist: protobuf (>=4.25.3,<5.0.0) Requires-Dist:
-pycaption (>=2.2.4,<3.0.0) Requires-Dist: pycryptodomex (>=3.20.0,<4.0.0)
-Requires-Dist: pyjwt (>=2.8.0,<3.0.0) Requires-Dist: pymediainfo
-(>=6.1.0,<7.0.0) Requires-Dist: pymp4 (>=1.4.0,<2.0.0) Requires-Dist: pymysql
-(>=1.1.0,<2.0.0) Requires-Dist: pywidevine[serve] (>=1.8.0,<2.0.0) Requires-
-Dist: requests[socks] (>=2.31.0,<3.0.0) Requires-Dist: rich (>=13.7.1,<14.0.0)
-Requires-Dist: rlaphoenix.m3u8 (>=3.4.0,<4.0.0) Requires-Dist: ruamel.yaml
-(>=0.18.6,<0.19.0) Requires-Dist: sortedcontainers (>=2.4.0,<3.0.0) Requires-
-Dist: subtitle-filter (>=1.4.9,<2.0.0) Requires-Dist: urllib3 (>=2.2.1,<3.0.0)
-Project-URL: Changelog, https://github.com/devine-dl/devine/blob/master/
-CHANGELOG.md Project-URL: Discussions, https://github.com/devine-dl/devine/
-discussions Project-URL: Issues, https://github.com/devine-dl/devine/issues
-Project-URL: Repository, https://github.com/devine-dl/devine Description-
-Content-Type: text/markdown
+(>=3.0.4,<4.0.0) Requires-Dist: langcodes[data] (>=3.3.0,<4.0.0) Requires-Dist:
+language-data (>=1.2.0,<2.0.0) Requires-Dist: lxml (>=5.2.1,<6.0.0) Requires-
+Dist: marisa-trie (>=1.1.0,<2.0.0) Requires-Dist: pproxy (>=2.7.9,<3.0.0)
+Requires-Dist: protobuf (>=4.25.3,<5.0.0) Requires-Dist: pycaption
+(>=2.2.6,<3.0.0) Requires-Dist: pycryptodomex (>=3.20.0,<4.0.0) Requires-Dist:
+pyjwt (>=2.8.0,<3.0.0) Requires-Dist: pymediainfo (>=6.1.0,<7.0.0) Requires-
+Dist: pymp4 (>=1.4.0,<2.0.0) Requires-Dist: pymysql (>=1.1.0,<2.0.0) Requires-
+Dist: pywidevine[serve] (>=1.8.0,<2.0.0) Requires-Dist: requests[socks]
+(>=2.31.0,<3.0.0) Requires-Dist: rich (>=13.7.1,<14.0.0) Requires-Dist:
+rlaphoenix.m3u8 (>=3.4.0,<4.0.0) Requires-Dist: ruamel.yaml (>=0.18.6,<0.19.0)
+Requires-Dist: sortedcontainers (>=2.4.0,<3.0.0) Requires-Dist: subtitle-filter
+(>=1.4.9,<2.0.0) Requires-Dist: urllib3 (>=2.2.1,<3.0.0) Project-URL:
+Changelog, https://github.com/devine-dl/devine/blob/master/CHANGELOG.md
+Project-URL: Discussions, https://github.com/devine-dl/devine/discussions
+Project-URL: Issues, https://github.com/devine-dl/devine/issues Project-URL:
+Repository, https://github.com/devine-dl/devine Description-Content-Type: text/
+markdown
  [https://user-images.githubusercontent.com/17136956/216880837-478f3ec7-6af6-
                       4cca-8eef-5c98ff02104c.png]_D_e_v_i_n_e
                 MMoodduullaarr MMoovviiee,, TTVV,, aanndd MMuussiicc AArrcchhiivvaall SSooffttwwaarree
                                    _[_D_i_s_c_o_r_d_]
                   _[_B_u_i_l_d_ _s_t_a_t_u_s_]_[_P_y_t_h_o_n_ _v_e_r_s_i_o_n_]_[_D_e_e_p_S_o_u_r_c_e_]
                  _[_L_i_n_t_e_r_:_ _R_u_f_f_]_[_D_e_p_e_n_d_e_n_c_y_ _m_a_n_a_g_e_m_e_n_t_:_ _P_o_e_t_r_y_]
 ## Features - ð Seamless Installation via [pip](#installation) - ð¥ Movie,
@@ -253,11 +253,11 @@
 this includes Widevine Provision Keys, Content Encryption Keys, or Service API
 Calls or Code. 3. The Core codebase is meant to stay Free and Open-Source while
 the Service code should be kept private. 4. Do not sell any part of this
 project, neither alone nor as part of a bundle. If you paid for this software
 or received it as part of a bundle following payment, you should demand your
 money back immediately. 5. Be kind to one another and do not single anyone out.
 ## Contributors _[_r_l_a_p_h_o_e_n_i_x_]_[_m_n_m_l_l_]_[_s_h_i_r_t_-_d_e_v_]_[_n_y_u_s_z_i_k_a_7_h_]_[_b_c_c_o_r_n_f_o_]_[_A_r_i_a_s_8_0_0_]
-_[_v_a_r_y_g_1_0_0_1_]_[_H_o_l_l_a_n_d_e_r_-_1_9_0_8_]_[_S_h_i_v_e_l_i_g_h_t_]_[_k_n_o_w_h_e_r_e_0_1_]## Licensing This software
-is licensed under the terms of [GNU General Public License, Version 3.0]
-(LICENSE). You can find a copy of the license in the LICENSE file in the root
-folder. * * * Â© rlaphoenix 2019-2024
+_[_v_a_r_y_g_1_0_0_1_]_[_H_o_l_l_a_n_d_e_r_-_1_9_0_8_]_[_S_h_i_v_e_l_i_g_h_t_]_[_k_n_o_w_h_e_r_e_0_1_]_[_r_e_t_o_u_c_h_i_n_g_]## Licensing
+This software is licensed under the terms of [GNU General Public License,
+Version 3.0](LICENSE). You can find a copy of the license in the LICENSE file
+in the root folder. * * * Â© rlaphoenix 2019-2024
```

