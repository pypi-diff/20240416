# Comparing `tmp/offspot_config-1.9.0.tar.gz` & `tmp/offspot_config-2.0.0.tar.gz`

## Comparing `offspot_config-1.9.0.tar` & `offspot_config-2.0.0.tar`

### file list

```diff
@@ -1,36 +1,52 @@
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 offspot_config-1.9.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     6970 2020-02-02 00:00:00.000000 offspot_config-1.9.0/CHANGELOG.md
--rw-r--r--   0        0        0     3091 2020-02-02 00:00:00.000000 offspot_config-1.9.0/tasks.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 offspot_config-1.9.0/src/offspot_config/__init__.py
--rw-r--r--   0        0        0    27601 2020-02-02 00:00:00.000000 offspot_config-1.9.0/src/offspot_config/builder.py
--rw-r--r--   0        0        0    12361 2020-02-02 00:00:00.000000 offspot_config-1.9.0/src/offspot_config/catalog.json
--rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 offspot_config-1.9.0/src/offspot_config/catalog.py
--rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 offspot_config-1.9.0/src/offspot_config/constants.py
--rw-r--r--   0        0        0     4155 2020-02-02 00:00:00.000000 offspot_config-1.9.0/src/offspot_config/file.py
--rw-r--r--   0        0        0     6369 2020-02-02 00:00:00.000000 offspot_config-1.9.0/src/offspot_config/inputs.py
--rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 offspot_config-1.9.0/src/offspot_config/oci_images.py
--rw-r--r--   0        0        0     5397 2020-02-02 00:00:00.000000 offspot_config-1.9.0/src/offspot_config/packages.py
--rw-r--r--   0        0        0     1870 2020-02-02 00:00:00.000000 offspot_config-1.9.0/src/offspot_config/zim.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 offspot_config-1.9.0/src/offspot_config/utils/__init__.py
--rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 offspot_config-1.9.0/src/offspot_config/utils/download.py
--rw-r--r--   0        0        0    12617 2020-02-02 00:00:00.000000 offspot_config-1.9.0/src/offspot_config/utils/misc.py
--rw-r--r--   0        0        0     1935 2020-02-02 00:00:00.000000 offspot_config-1.9.0/src/offspot_config/utils/sizes.py
--rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 offspot_config-1.9.0/src/offspot_config/utils/yaml.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 offspot_config-1.9.0/src/offspot_runtime/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 offspot_config-1.9.0/src/offspot_runtime/__init__.py
--rwxr-xr-x   0        0        0    18295 2020-02-02 00:00:00.000000 offspot_config-1.9.0/src/offspot_runtime/ap.py
--rw-r--r--   0        0        0    20537 2020-02-02 00:00:00.000000 offspot_config-1.9.0/src/offspot_runtime/checks.py
--rw-r--r--   0        0        0     4886 2020-02-02 00:00:00.000000 offspot_config-1.9.0/src/offspot_runtime/configlib.py
--rwxr-xr-x   0        0        0     2564 2020-02-02 00:00:00.000000 offspot_config-1.9.0/src/offspot_runtime/containers.py
--rw-r--r--   0        0        0     3341 2020-02-02 00:00:00.000000 offspot_config-1.9.0/src/offspot_runtime/dnsmasqspoof.py
--rwxr-xr-x   0        0        0     5142 2020-02-02 00:00:00.000000 offspot_config-1.9.0/src/offspot_runtime/ethernet.py
--rwxr-xr-x   0        0        0     7627 2020-02-02 00:00:00.000000 offspot_config-1.9.0/src/offspot_runtime/fromfile.py
--rwxr-xr-x   0        0        0     2122 2020-02-02 00:00:00.000000 offspot_config-1.9.0/src/offspot_runtime/hostname.py
--rwxr-xr-x   0        0        0     1678 2020-02-02 00:00:00.000000 offspot_config-1.9.0/src/offspot_runtime/timezone.py
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 offspot_config-1.9.0/tests/test_catalog.py
--rw-r--r--   0        0        0    20270 2020-02-02 00:00:00.000000 offspot_config-1.9.0/tests/test_checks.py
--rw-r--r--   0        0        0     4062 2020-02-02 00:00:00.000000 offspot_config-1.9.0/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 offspot_config-1.9.0/LICENSE
--rw-r--r--   0        0        0     9526 2020-02-02 00:00:00.000000 offspot_config-1.9.0/README.md
--rw-r--r--   0        0        0     6610 2020-02-02 00:00:00.000000 offspot_config-1.9.0/pyproject.toml
--rw-r--r--   0        0        0    11300 2020-02-02 00:00:00.000000 offspot_config-1.9.0/PKG-INFO
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 offspot_config-2.0.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     9690 2020-02-02 00:00:00.000000 offspot_config-2.0.0/CHANGELOG.md
+-rw-r--r--   0        0        0     3091 2020-02-02 00:00:00.000000 offspot_config-2.0.0/tasks.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 offspot_config-2.0.0/src/offspot_config/__init__.py
+-rw-r--r--   0        0        0    30298 2020-02-02 00:00:00.000000 offspot_config-2.0.0/src/offspot_config/builder.py
+-rw-r--r--   0        0        0    14110 2020-02-02 00:00:00.000000 offspot_config-2.0.0/src/offspot_config/catalog.json
+-rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 offspot_config-2.0.0/src/offspot_config/catalog.py
+-rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 offspot_config-2.0.0/src/offspot_config/constants.py
+-rw-r--r--   0        0        0     4569 2020-02-02 00:00:00.000000 offspot_config-2.0.0/src/offspot_config/file.py
+-rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 offspot_config-2.0.0/src/offspot_config/oci_images.py
+-rw-r--r--   0        0        0     6652 2020-02-02 00:00:00.000000 offspot_config-2.0.0/src/offspot_config/packages.py
+-rw-r--r--   0        0        0     3676 2020-02-02 00:00:00.000000 offspot_config-2.0.0/src/offspot_config/zim.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 offspot_config-2.0.0/src/offspot_config/inputs/__init__.py
+-rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 offspot_config-2.0.0/src/offspot_config/inputs/base.py
+-rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 offspot_config-2.0.0/src/offspot_config/inputs/checksum.py
+-rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 offspot_config-2.0.0/src/offspot_config/inputs/file.py
+-rw-r--r--   0        0        0     3680 2020-02-02 00:00:00.000000 offspot_config-2.0.0/src/offspot_config/inputs/mainconfig.py
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 offspot_config-2.0.0/src/offspot_config/inputs/oci.py
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 offspot_config-2.0.0/src/offspot_config/inputs/output.py
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 offspot_config-2.0.0/src/offspot_config/inputs/str.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 offspot_config-2.0.0/src/offspot_config/inputs/ways.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 offspot_config-2.0.0/src/offspot_config/utils/__init__.py
+-rw-r--r--   0        0        0     2013 2020-02-02 00:00:00.000000 offspot_config-2.0.0/src/offspot_config/utils/dashboard.py
+-rw-r--r--   0        0        0     4458 2020-02-02 00:00:00.000000 offspot_config-2.0.0/src/offspot_config/utils/download.py
+-rw-r--r--   0        0        0    12617 2020-02-02 00:00:00.000000 offspot_config-2.0.0/src/offspot_config/utils/misc.py
+-rw-r--r--   0        0        0     1946 2020-02-02 00:00:00.000000 offspot_config-2.0.0/src/offspot_config/utils/sizes.py
+-rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 offspot_config-2.0.0/src/offspot_config/utils/yaml.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 offspot_config-2.0.0/src/offspot_runtime/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 offspot_config-2.0.0/src/offspot_runtime/__init__.py
+-rwxr-xr-x   0        0        0    18295 2020-02-02 00:00:00.000000 offspot_config-2.0.0/src/offspot_runtime/ap.py
+-rw-r--r--   0        0        0    21248 2020-02-02 00:00:00.000000 offspot_config-2.0.0/src/offspot_runtime/checks.py
+-rw-r--r--   0        0        0     4936 2020-02-02 00:00:00.000000 offspot_config-2.0.0/src/offspot_runtime/configlib.py
+-rwxr-xr-x   0        0        0     2564 2020-02-02 00:00:00.000000 offspot_config-2.0.0/src/offspot_runtime/containers.py
+-rwxr-xr-x   0        0        0     3341 2020-02-02 00:00:00.000000 offspot_config-2.0.0/src/offspot_runtime/dnsmasqspoof.py
+-rwxr-xr-x   0        0        0     5142 2020-02-02 00:00:00.000000 offspot_config-2.0.0/src/offspot_runtime/ethernet.py
+-rwxr-xr-x   0        0        0     5210 2020-02-02 00:00:00.000000 offspot_config-2.0.0/src/offspot_runtime/firmware.py
+-rwxr-xr-x   0        0        0     8362 2020-02-02 00:00:00.000000 offspot_config-2.0.0/src/offspot_runtime/fromfile.py
+-rwxr-xr-x   0        0        0     2122 2020-02-02 00:00:00.000000 offspot_config-2.0.0/src/offspot_runtime/hostname.py
+-rwxr-xr-x   0        0        0     1678 2020-02-02 00:00:00.000000 offspot_config-2.0.0/src/offspot_runtime/timezone.py
+-rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 offspot_config-2.0.0/tests/conftest.py
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 offspot_config-2.0.0/tests/test_catalog.py
+-rw-r--r--   0        0        0    21249 2020-02-02 00:00:00.000000 offspot_config-2.0.0/tests/test_checks.py
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 offspot_config-2.0.0/tests/test_humanid.py
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 offspot_config-2.0.0/tests/test_inputs.py
+-rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 offspot_config-2.0.0/tests/test_link.py
+-rw-r--r--   0        0        0     5778 2020-02-02 00:00:00.000000 offspot_config-2.0.0/tests/test_reader.py
+-rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 offspot_config-2.0.0/tests/test_zim.py
+-rw-r--r--   0        0        0     4062 2020-02-02 00:00:00.000000 offspot_config-2.0.0/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 offspot_config-2.0.0/LICENSE
+-rw-r--r--   0        0        0    11831 2020-02-02 00:00:00.000000 offspot_config-2.0.0/README.md
+-rw-r--r--   0        0        0     6733 2020-02-02 00:00:00.000000 offspot_config-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0    13707 2020-02-02 00:00:00.000000 offspot_config-2.0.0/PKG-INFO
```

### Comparing `offspot_config-1.9.0/.pre-commit-config.yaml` & `offspot_config-2.0.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `offspot_config-1.9.0/CHANGELOG.md` & `offspot_config-2.0.0/CHANGELOG.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,111 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [2.0.0] - 2024-04-16
+
+### Added
+
+- [inputs.file] File now includes a `checksum` property (optional)
+- [inputs.checksum] Checksum now includes an `as_aria` property (`algo=digest` formatted string)
+
+### Changed ⚠️ BREAKING
+
+- [inputs] API refactored into an empty `inputs` module with many sub-modules (breaking change)
+
+## [1.14.0] - 2024-04-11
+
+### Added
+
+- [utils.download] `get_payload_from` to retrieve small bit of data from a URL
+- [utils.download] `read_checksum_from` to retrieve digest-looking string from a URL
+- [inputs] `Checksum` type that describe a checksum with its algo (several supported) and includes mechanism for later-resolution via URL URL retrieval
+- [inputs] Packages (Files, App, Zim) gets an optional `download_checksum` param that is passed to FileConfig
+- [builder] Readers get an automatically fetched checksum if URL is on download.kiwix.org
+- [builder] `add_file()` takes an optional `checksum` param
+
+### Changed
+
+- [catalog] All Catalog entries now have download_checksum if applicable
+- [zim] `get_zim_package` now includes a live-fetched MD5 checksum
+
+
+## [1.13.0] - 2024-04-01
+
+### Added
+
+- [utils.dashboard] Reader struct to ease passing `readers` to dashboard YAML
+- [utils.dashboard] Link struct to ease passing `links` to dashboard YAML
+- [builder] `add_dashboard()` param: `readers` to automatically add and offer Kiwix readers in dashboard (1.4+)
+- [builder] `add_dashboard()` param: `links` to add arbitrary links to dashboard (1.4+)
+
+## Changed
+
+- [builder] `resolved_variable()` can now be used without a Package
+
+## [1.12.2] - 2024-03-14
+
+### Fixed
+
+- [catalog] magoe update wasn't included
+
+## [1.12.1] - 2024-03-05
+
+### Changed
+
+- [catalog] Updated magoe package
+
+## [1.12.0] - 2024-02-21
+
+### Added
+
+- [zim] `get_libkiwix_humanid()` to get kiwix-serve BookName from a filename
+
+### Changed
+
+- [packages] `ZimPackage.get_url()` now uses libkiwix's human ID
+
+## [1.11.0] - 2024-02-17
+
+### Added
+
+- [zim] `to_ident()` and `from_ident()` functions to consistently work on idents
+- [zim] `ZimIdentTuple` type, returned by `from_ident()`
+
+### Changed
+
+- [packages] `ZimPackage.filename` now returns an ident-based one preventing conflicts on files with different flavours
+
+## [1.10.1] - 2024-02-12
+
+### Changed
+
+- [builder] Using dashboard:1.3.1
+
+## [1.10.0] - 2024-02-11
+
+### Added
+
+- [firmware] New `firmware` top level config for runtime to change WiFi firmware
+
+### Fixed
+
+- [builder] Welcome FQDN properly set (goto.kiwix)
+- [catalog] file-manager URL (no trailing slash)
+
+### Changed
+
+- [builder] Using captive-portal:1.4 with offline fix
+- [builder] Using reverse-proxy:1.7 with welcome_fqdn
+- [catalog] Using file-manager:1.3 with metrics headers
+
 ## [1.9.0] - 2024-02-09
 
 ### Added
 
 - [builder] AP welcome_domain now settable (defaulting to `goto.kiwix`)
 - [ap] `captured-address` allows setting the DNS fallback target for when offline
 
@@ -243,7 +340,8 @@
 ## Added
 
 - `auto` option for `spoof` param in `ap` to adjust based on internet connectivity
 
 ## [1.0.0] - 2022-10-05
 
 - initial version
+CHANGELOG.md
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `offspot_config-1.9.0/tasks.py` & `offspot_config-2.0.0/tasks.py`

 * *Files identical despite different names*

### Comparing `offspot_config-1.9.0/src/offspot_config/builder.py` & `offspot_config-2.0.0/src/offspot_config/builder.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,24 @@
 from __future__ import annotations
 
 import re
 from pathlib import PurePath as Path
 from typing import Any
+from urllib.parse import urlsplit
 
 from offspot_config.catalog import app_catalog, get_app_path
 from offspot_config.constants import CONTENT_TARGET_PATH
-from offspot_config.inputs import BaseConfig, BlockStr, FileConfig
+from offspot_config.inputs.base import BaseConfig
+from offspot_config.inputs.checksum import Checksum
+from offspot_config.inputs.file import FileConfig
+from offspot_config.inputs.str import BlockStr
 from offspot_config.oci_images import OCIImage
 from offspot_config.packages import AppPackage, FilesPackage, ZimPackage
+from offspot_config.utils.dashboard import Link, Reader
+from offspot_config.utils.download import read_checksum_from
 from offspot_config.utils.sizes import (
     get_margin_for,
     get_min_image_size_for,
     get_raw_content_size_for,
 )
 from offspot_config.utils.yaml import yaml_dump
 
@@ -23,29 +29,30 @@
 # service subdomain for ZIM downloads, when enabled
 ZIMDL_PREFIX = "zim-download"
 # on-host path to dashboard config
 DASHBOARD_CONFIG_PATH = CONTENT_TARGET_PATH / "dashboard.yaml"
 # on-host metrics persistent data folder
 METRICS_DATA_PATH = CONTENT_TARGET_PATH / "metrics"
 # on-host metrics transient (tmpfs) log folders (caddy-created)
+KIWIXSERVE_DATA_PATH = CONTENT_TARGET_PATH / "zims"
 METRICS_VAR_LOG_PATH_HOST = Path("/var/log/metrics")
 METRICS_VAR_LOG_PATH_CONT = Path("/var/log/host/metrics")
 KIWIX_ZIM_LOAD_BALANCER_URL = "https://download.kiwix.org/zim/"
 
 # data source for “internal images” (out of catalog)
 INTERNAL_IMAGES = {
     "captive-portal": {
-        "source": "ghcr.io/offspot/captive-portal:1.3",
-        "filesize": 184545280,
-        "fullsize": 184474177,
+        "source": "ghcr.io/offspot/captive-portal:1.4",
+        "filesize": 184627200,
+        "fullsize": 184559684,
     },
     "dashboard": {
-        "source": "ghcr.io/offspot/dashboard:1.3",
-        "filesize": 124334080,
-        "fullsize": 124248725,
+        "source": "ghcr.io/offspot/dashboard:1.3.1",
+        "filesize": 124354560,
+        "fullsize": 124261524,
     },
     "file-browser": {
         "source": "ghcr.io/offspot/file-browser:1.1",
         "filesize": 13629440,
         "fullsize": 13598399,
     },
     "hwclock": {
@@ -60,17 +67,17 @@
     },
     "metrics": {
         "source": "ghcr.io/offspot/metrics:0.3.0",
         "filesize": 167311360,
         "fullsize": 167202612,
     },
     "reverse-proxy": {
-        "source": "ghcr.io/offspot/reverse-proxy:1.6",
+        "source": "ghcr.io/offspot/reverse-proxy:1.7",
         "filesize": 120350720,
-        "fullsize": 120278906,
+        "fullsize": 120279091,
     },
 }
 
 
 def get_internal_image(ident: str) -> OCIImage:
     """OCI Image from special key identifying internal image"""
     if ident == "file-manager":
@@ -122,14 +129,18 @@
             },
         }
 
         # Kiwix mirror URL (/ ending) to replace load-balancer URL with for ZIM download
         self.kiwix_zim_mirror = kiwix_zim_mirror
         # whether dashboard will offer downloads for ZIM files
         self.dashboard_offers_zim_downloads = True
+        # list of reader entries to include in dashboard config
+        self.dashboard_readers: list[Reader] = []
+        # list of arbitrary links to display in dashboard
+        self.dashboard_links: list[Link] = []
         # every card the dashboard will display
         self.dashboard_entries = []
 
         # domain of services that must be reversed to (all but special cases)
         # either domain or domain:target-domain:target-port
         self.reversed_services: set[str] = set()
         # domain: folder map of virtual services serving only files
@@ -172,21 +183,56 @@
                 url_or_content="-",
                 to=f"{path}/.touch",
                 size=1,
                 via="direct",
                 is_url=False,
             )
 
-    def add_dashboard(self, *, allow_zim_downloads: bool | None = False):
-        self.dashboard_offers_zim_downloads = allow_zim_downloads
+    def add_dashboard(
+        self,
+        *,
+        allow_zim_downloads: bool | None = None,
+        readers: list[Reader] | None = None,
+        links: list[Link] | None = None,
+    ):
+        # only override options if set to a value (might have been set before)
+        if allow_zim_downloads is not None:
+            self.dashboard_offers_zim_downloads = allow_zim_downloads
+        if readers is not None:
+            self.dashboard_readers = readers
+        if links is not None:
+            self.dashboard_links = links
+
         if self.with_dashboard:
             return
 
         self.with_dashboard = True
 
+        # Add files for requested readers
+        for reader in self.dashboard_readers:
+            checksum = None
+            # download.kiwix.org is known to provide digests via mirrorbrain
+            if urlsplit(reader.download_url).netloc == "download.kiwix.org":
+                try:
+                    checksum = Checksum(
+                        algo="md5",
+                        value=read_checksum_from(f"{reader.download_url}.md5"),
+                    )
+                # we cant assume this this work forever
+                except Exception:
+                    ...
+            self.add_file(
+                url_or_content=reader.download_url,
+                to=str(KIWIXSERVE_DATA_PATH / reader.filename),
+                via="direct",
+                size=reader.size,
+                checksum=checksum,
+                is_url=True,
+            )
+
         image = get_internal_image("dashboard")
         self.config["oci_images"].add(image)
 
         # add to compose
         self.compose["services"]["home"] = {
             "image": image.source,
             "container_name": "home",
@@ -215,15 +261,15 @@
                     "target": "/data/zims",
                     "read_only": True,
                 },
             ],
         }
 
         # add placeholder file to host fs to ensure bind succeeds
-        self.ensure_host_path(CONTENT_TARGET_PATH / "zims")
+        self.ensure_host_path(KIWIXSERVE_DATA_PATH)
 
     def gen_dashboard_config(self):
         """Generate and add YAML config file for dashboard, based on entries"""
 
         if self.dashboard_offers_zim_downloads:
             download_fqdn = f"{ZIMDL_PREFIX}.{self.fqdn}"
         else:
@@ -233,14 +279,26 @@
             "metadata": {"name": self.name, "fqdn": self.fqdn},
             "packages": [
                 package.to_dashboard_entry(fqdn=self.fqdn, download_fqdn=download_fqdn)
                 for package in self.dashboard_entries
             ],
         }
 
+        if self.dashboard_readers:
+            payload["readers"] = [
+                reader.to_dict()
+                for reader in sorted(self.dashboard_readers, key=Reader.sort)
+            ]
+
+        if self.dashboard_links:
+            payload["links"] = [link.to_dict() for link in self.dashboard_links]
+            # resolve variables in link (for FQDN mostly)
+            for link in payload["links"]:
+                link["url"] = self.resolved_variable(text=link["url"])
+
         yaml_str = yaml_dump(payload)
         self.add_file(
             url_or_content=BlockStr(yaml_str),
             to=str(CONTENT_TARGET_PATH / "dashboard.yaml"),
             size=len(yaml_str.encode("utf-8")),
             via="direct",
             is_url=False,
@@ -257,14 +315,18 @@
 
         # add to compose
         self.compose["services"]["reverse-proxy"] = {
             "image": image.source,
             "container_name": "reverse-proxy",
             "environment": {
                 "FQDN": self.fqdn,
+                "WELCOME_FQDN": (
+                    f'{self.config["offspot"]["ap"]["welcome"]}.'
+                    f'{self.config["offspot"]["ap"]["tld"]}'
+                ),
                 "METRICS_LOGS_DIR": str(METRICS_VAR_LOG_PATH_CONT),
             },
             "pull_policy": "never",
             "restart": "unless-stopped",
             "ports": ["80:80", "443:443"],
             "volumes": [
                 # we are not binding METRICS_VAR_LOG_PATH directly because it resides
@@ -440,17 +502,18 @@
                 f"{zim.download_url[len(KIWIX_ZIM_LOAD_BALANCER_URL):]}"
             )
         if zim not in self.dashboard_entries:
             self.dashboard_entries.append(zim)
 
         self.add_file(
             url_or_content=zim.download_url,
-            to=str(CONTENT_TARGET_PATH / "zims" / zim.filename),
+            to=str(KIWIXSERVE_DATA_PATH / zim.filename),
             via="direct",
             size=zim.download_size,
+            checksum=zim.download_checksum,
             is_url=True,
         )
 
         if self.with_kiwixserve:
             return
 
         self.with_kiwixserve = True
@@ -476,15 +539,15 @@
                 }
             ],
             "command": '/bin/sh -c "kiwix-serve --blockexternal '
             '--port 80 --nodatealiases /data/*.zim"',
         }
 
         # add placeholder file to host fs to ensure bind succeeds
-        self.ensure_host_path(CONTENT_TARGET_PATH / "zims")
+        self.ensure_host_path(KIWIXSERVE_DATA_PATH)
 
         if self.dashboard_offers_zim_downloads:
             self.add_files_service()
             self.files_mapping.update({ZIMDL_PREFIX: "zims"})
 
         self.reversed_services.add("kiwix")
 
@@ -677,14 +740,15 @@
         self,
         *,
         url_or_content: str,
         to: str,
         via: str,
         size: int,
         is_url: bool | None = True,
+        checksum: Checksum | None = None,
     ):
         # @to param can reference a specific package's home
         app_dir_match = RE_SPECIFIC_APP_DIR.match(to)
         if app_dir_match:
             ident = app_dir_match.groupdict()["ident"]
             to = to.replace(
                 "${APP_DIR:" + ident + "}", get_app_path(package=app_catalog[ident])
@@ -693,35 +757,39 @@
         self.config["files"].append(
             FileConfig(
                 **{
                     "url" if is_url else "content": url_or_content,
                     "to": to,
                     "via": via,
                     "size": size,
+                    "checksum": checksum,
                 }
             )
         )
 
-    def resolved_variable(self, text: str, package: AppPackage) -> str:
+    def resolved_variable(self, text: str, package: AppPackage | None = None) -> str:
         """dynamic-variables resolved string"""
-        app_dir = get_app_path(package=package)
 
         # replace $environ{XXX} mappings
         match = RE_ENVIRON_VAR.search(text)
         if match:
             repl = self.environ[match.groupdict()["var"]]
             text = RE_ENVIRON_VAR.sub(repl, text)
-        return (
-            text.replace("${APP_DIR}", app_dir)
-            .replace("${FQDN}", self.fqdn)
-            .replace("${PACKAGE_IDENT}", package.ident)
-            .replace("${PACKAGE_DOMAIN}", package.domain)
-            .replace("${PACKAGE_FQDN}", f"{package.domain}.{self.fqdn}")
-            .replace("${REVERSE_NAME}", "reverse-proxy")
+        resolved = text.replace("${FQDN}", self.fqdn).replace(
+            "${REVERSE_NAME}", "reverse-proxy"
         )
+        if package:
+            app_dir = get_app_path(package=package)
+            resolved = (
+                resolved.replace("${APP_DIR}", app_dir)
+                .replace("${PACKAGE_IDENT}", package.ident)
+                .replace("${PACKAGE_DOMAIN}", package.domain)
+                .replace("${PACKAGE_FQDN}", f"{package.domain}.{self.fqdn}")
+            )
+        return resolved
 
     def get_resolved_host_path(self, package: AppPackage, host_path: str) -> str:
         """dynamic-variables resolved host path for package"""
 
         return self.resolved_variable(text=host_path, package=package)
 
     def get_min_size(self) -> int:
```

### Comparing `offspot_config-1.9.0/src/offspot_config/catalog.json` & `offspot_config-2.0.0/src/offspot_config/catalog.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9239342612044816%*

 * *Differences: {'1': "{'download_checksum': OrderedDict([('algo', 'md5'), ('value', "*

 * *      "'9532683142885b67c305b16ad8b5dccd')])}",*

 * * '10': "{'download_checksum': OrderedDict([('algo', 'md5'), ('value', "*

 * *       "'c8ad28bfd8e5a0005ad128c9d09dd5c6')])}",*

 * * '11': "{'download_checksum': OrderedDict([('algo', 'md5'), ('value', "*

 * *       "'4e5e6761f61d71d0b728c0a967d7ca08')])}",*

 * * '12': "{'download_url': 'https://drive.offspot.it/magoe/magoe_fr_app_2024-03.zip', "*

 * *       "'download_size': 295323137, 'download_checksum': OrderedD […]*

```diff
@@ -15,14 +15,18 @@
             "admin"
         ],
         "title": "Content Filter"
     },
     {
         "description": "Environnement qui vous permet de cr\u00e9er des articles Wikip\u00e9dia hors-ligne (en fran\u00e7ais)",
         "domain": "wikifundi-fr",
+        "download_checksum": {
+            "algo": "md5",
+            "value": "9532683142885b67c305b16ad8b5dccd"
+        },
         "download_size": 4723138560,
         "download_url": "https://drive.offspot.it/wikifundi/fr_2021-12.tar",
         "download_via": "tar",
         "environ": {
             "MATHOID_URL": "http://mathoid.${PACKAGE_FQDN}/",
             "RESTBASE_URL": "http://restbase.${PACKAGE_FQDN}/${PACKAGE_FQDN}/",
             "URL": "http://${PACKAGE_FQDN}"
@@ -55,14 +59,18 @@
         "volumes": [
             "${APP_DIR}:/var/www/data"
         ]
     },
     {
         "description": "Offline editable environment that provides a similar experience to editing Wikipedia online (in English)",
         "domain": "wikifundi-en",
+        "download_checksum": {
+            "algo": "md5",
+            "value": "ddfa210ea602e06500b684cbe19e27ec"
+        },
         "download_size": 5477140480,
         "download_url": "https://drive.offspot.it/wikifundi/en_2021-12.tar",
         "download_via": "tar",
         "environ": {
             "MATHOID_URL": "http://mathoid.${PACKAGE_FQDN}/",
             "RESTBASE_URL": "http://restbase.${PACKAGE_FQDN}/${PACKAGE_FQDN}/",
             "URL": "http://${PACKAGE_FQDN}"
@@ -95,14 +103,18 @@
         "volumes": [
             "${APP_DIR}:/var/www/data"
         ]
     },
     {
         "description": "Entorno editable sin conexi\u00f3n que brinda una experiencia similar a la edici\u00f3n de Wikipedia en l\u00ednea (en espa\u00f1ol)",
         "domain": "wikifundi-es",
+        "download_checksum": {
+            "algo": "md5",
+            "value": "44e0894ef16fb04ec4b0feb3c7ea3db8"
+        },
         "download_size": 5842176000,
         "download_url": "https://drive.offspot.it/wikifundi/es_2021-12.tar",
         "download_via": "tar",
         "environ": {
             "MATHOID_URL": "http://mathoid.${PACKAGE_FQDN}/",
             "RESTBASE_URL": "http://restbase.${PACKAGE_FQDN}/${PACKAGE_FQDN}/",
             "URL": "http://${PACKAGE_FQDN}"
@@ -137,25 +149,25 @@
         ]
     },
     {
         "description": "View and download resources",
         "domain": "resources",
         "environ": {
             "ACCESS_MODE": "mixed",
-            "APP_URL": "http://${PACKAGE_FQDN}/"
+            "APP_URL": "http://${PACKAGE_FQDN}"
         },
         "environ_map": {
             "ADMIN_PASSWORD": "ADMIN_PASSWORD",
             "ADMIN_USERNAME": "ADMIN_USERNAME"
         },
         "icon_url": "https://drive.offspot.it/edupi/edupi.png",
         "ident": "file-manager.offspot.kiwix.org",
-        "image": "ghcr.io/offspot/file-manager:1.1",
-        "image_filesize": 42209280,
-        "image_fullsize": 42158625,
+        "image": "ghcr.io/offspot/file-manager:1.3",
+        "image_filesize": 42229760,
+        "image_fullsize": 42171245,
         "kind": "app",
         "languages": [
             "mul"
         ],
         "tags": [
             "files"
         ],
@@ -163,14 +175,18 @@
         "volumes": [
             "${APP_DIR}:/data"
         ]
     },
     {
         "description": "Application Android",
         "domain": "nomad",
+        "download_checksum": {
+            "algo": "md5",
+            "value": "0a5b3814ef7ab67b5de906495989fa59"
+        },
         "download_size": 151606771,
         "download_url": "https://drive.offspot.it/nomad/nomadeducation_fr_android_2023-11.zip",
         "icon_url": "https://drive.offspot.it/nomad/nomad_logo.png",
         "ident": "nomad.offspot.kiwix.org",
         "kind": "files",
         "languages": [
             "fra"
@@ -180,14 +196,18 @@
         ],
         "title": "Nomad exercices du CP \u00e0 la 3\u00e8",
         "via": "zip"
     },
     {
         "description": "Un jeu pour faire des maths (6-9 ans)",
         "domain": "mathews",
+        "download_checksum": {
+            "algo": "md5",
+            "value": "12e4912c44b28e085f6292083c18dc2e"
+        },
         "download_size": 35710192,
         "download_url": "https://drive.offspot.it/mathews/mathmathews_fr_android_1.6.zip",
         "icon_url": "https://drive.offspot.it/mathews/mathmathews_logo.png",
         "ident": "mathews.offspot.kiwix.org",
         "kind": "files",
         "languages": [
             "fra"
@@ -197,14 +217,18 @@
         ],
         "title": "Chasse au tr\u00e9sor Math Mathews",
         "via": "zip"
     },
     {
         "description": "Applications \u00e9ducatives adapt\u00e9es au contexte culturel africain (version \u00c9coles num\u00e9riques)",
         "domain": "africatik-en",
+        "download_checksum": {
+            "algo": "md5",
+            "value": "0055097bf4768b7e295c167265023b9c"
+        },
         "download_size": 13906969131,
         "download_url": "https://drive.offspot.it/africatik/africatik_fr_ecoles-numeriques_2023-02.zip",
         "icon_url": "https://drive.offspot.it/africatik/africatik_logo.png",
         "ident": "africatik-en.offspot.kiwix.org",
         "kind": "files",
         "languages": [
             "fra"
@@ -215,14 +239,18 @@
         ],
         "title": "Africatik \u00c9coles num\u00e9riques",
         "via": "zip"
     },
     {
         "description": "Applications \u00e9ducatives adapt\u00e9es au contexte culturel africain (version Maisons digitales)",
         "domain": "africatik-md",
+        "download_checksum": {
+            "algo": "md5",
+            "value": "d89d79979209247b7ecf8eb3f11eccde"
+        },
         "download_size": 4394410977,
         "download_url": "https://drive.offspot.it/africatik/africatik_fr_maisons-digitales_2023-02.zip",
         "icon_url": "https://drive.offspot.it/africatik/africatik_logo.png",
         "ident": "africatik-md.offspot.kiwix.org",
         "kind": "files",
         "languages": [
             "fra"
@@ -233,14 +261,18 @@
         ],
         "title": "Africatik Maisons digitales",
         "via": "zip"
     },
     {
         "description": "App Android pour l'apprentissage des sciences et de l'investigation scientifique",
         "domain": "fizziq-junior",
+        "download_checksum": {
+            "algo": "md5",
+            "value": "4e528e12576f6d365425306e5d318f32"
+        },
         "download_size": 128724719,
         "download_url": "https://drive.offspot.it/fizziq/fizziq_fr_junior_2023-03.zip",
         "icon_url": "https://drive.offspot.it/fizziq/fizziq-junior.png",
         "ident": "fizziq-junior.offspot.kiwix.org",
         "kind": "files",
         "languages": [
             "fra"
@@ -250,14 +282,18 @@
         ],
         "title": "Fizziq Junior",
         "via": "zip"
     },
     {
         "description": "Les math\u00e9matiques pour l'\u00e9cole primaire avec plus 600 activit\u00e9s randomis\u00e9es du CP au CM2.",
         "domain": "eleda",
+        "download_checksum": {
+            "algo": "md5",
+            "value": "c8ad28bfd8e5a0005ad128c9d09dd5c6"
+        },
         "download_size": 83684857,
         "download_url": "https://drive.offspot.it/eleda/eleda_fr_fo-offline_2023-10.zip",
         "icon_url": "https://drive.offspot.it/eleda/icon_zim.png",
         "ident": "eleda.offspot.kiwix.org",
         "kind": "files",
         "languages": [
             "fra"
@@ -265,14 +301,18 @@
         "tags": [],
         "title": "Les math\u00e9matiques du primaire",
         "via": "zip"
     },
     {
         "description": "App Android avec 600 activit\u00e9s de math\u00e9matiques",
         "domain": "eleda-android",
+        "download_checksum": {
+            "algo": "md5",
+            "value": "4e5e6761f61d71d0b728c0a967d7ca08"
+        },
         "download_size": 49364213,
         "download_url": "https://drive.offspot.it/eleda/eleda_fr_android_2023-10.zip",
         "icon_url": "https://drive.offspot.it/eleda/icon_zim.png",
         "ident": "eleda-android.offspot.kiwix.org",
         "kind": "files",
         "languages": [
             "fra"
@@ -282,16 +322,20 @@
         ],
         "title": "Les math\u00e9matiques du primaire",
         "via": "zip"
     },
     {
         "description": "Application de r\u00e9vision en ligne et de renforcement de capacit\u00e9",
         "domain": "magoe",
-        "download_size": 301348117,
-        "download_url": "https://drive.offspot.it/magoe/magoe_fr_app_2023-12.zip",
+        "download_checksum": {
+            "algo": "md5",
+            "value": "0ec2d9b9c2f61eb22247ceb935124923"
+        },
+        "download_size": 295323137,
+        "download_url": "https://drive.offspot.it/magoe/magoe_fr_app_2024-03.zip",
         "download_via": "zip",
         "environ": {
             "MAGOE_URL": "http://${PACKAGE_FQDN}"
         },
         "icon_url": "https://drive.offspot.it/magoe/magoe.png",
         "ident": "magoe.offspot.kiwix.org",
         "image": "ghcr.io/offspot/magoe:1.0",
@@ -306,14 +350,18 @@
         "volumes": [
             "${APP_DIR}:/var/www/magoe"
         ]
     },
     {
         "description": "Use your phone's sensors to assist with wilderness treks",
         "domain": "com.kylecorry.trail_sense",
+        "download_checksum": {
+            "algo": "md5",
+            "value": "8e7a3e22750789e8a70615a9d74686ee"
+        },
         "download_size": 7171835,
         "download_url": "https://drive.offspot.it/f-droid/com.kylecorry.trail_sense_111.zip",
         "icon_url": "https://drive.offspot.it/f-droid/com.kylecorry.trail_sense.png",
         "ident": "com.kylecorry.trail_sense.offspot.kiwix.org",
         "kind": "files",
         "languages": [
             "eng"
@@ -323,14 +371,18 @@
         ],
         "title": "Trail Sense",
         "via": "zip"
     },
     {
         "description": "Learn how to survive",
         "domain": "org.ligi.survivalmanual",
+        "download_checksum": {
+            "algo": "md5",
+            "value": "620510a857da1655b931081c2f85e33a"
+        },
         "download_size": 5528415,
         "download_url": "https://drive.offspot.it/f-droid/org.ligi.survivalmanual_428.zip",
         "icon_url": "https://drive.offspot.it/f-droid/org.ligi.survivalmanual.png",
         "ident": "org.ligi.survivalmanual.offspot.kiwix.org",
         "kind": "files",
         "languages": [
             "eng"
@@ -340,14 +392,18 @@
         ],
         "title": "Survival Manual",
         "via": "zip"
     },
     {
         "description": "Bible multi languages, free, offline, no advertising.",
         "domain": "org.hlwd.bible_multi_the_life",
+        "download_checksum": {
+            "algo": "md5",
+            "value": "b1a1e31076651b212b6b08f7cd897e07"
+        },
         "download_size": 59891151,
         "download_url": "https://drive.offspot.it/f-droid/org.hlwd.bible_multi_the_life_20230823.zip",
         "icon_url": "https://drive.offspot.it/f-droid/org.hlwd.bible_multi_the_life.png",
         "ident": "org.hlwd.bible_multi_the_life.offspot.kiwix.org",
         "kind": "files",
         "languages": [
             "eng"
```

### Comparing `offspot_config-1.9.0/src/offspot_config/catalog.py` & `offspot_config-2.0.0/src/offspot_config/catalog.py`

 * *Files identical despite different names*

### Comparing `offspot_config-1.9.0/src/offspot_config/constants.py` & `offspot_config-2.0.0/src/offspot_config/constants.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,14 +2,25 @@
 
 import pathlib
 import shutil
 
 DATA_PART_PATH: pathlib.Path = pathlib.Path("/data")
 CONTENT_TARGET_PATH: pathlib.Path = DATA_PART_PATH / "contents"
 SUPPORTED_UNPACKING_FORMATS: list[str] = [f[0] for f in shutil.get_unpack_formats()]
+# based on aria2c v1.37.0 static binary
+SUPPORTED_CHECKSUM_ALGORITHMS: list[str] = [
+    "sha-1",
+    "sha-224",
+    "sha-256",
+    "sha-384",
+    "sha-512",
+    "md5",
+    "adler32",
+]
+MAX_DIRECT_ONLINE_RESOURCE_PAYLOAD_SIZE: int = 4 * 2**20  # 4MiB
 POST_EXPANSION_UNWANTED_PATTERNS = (
     ### Linux ###
     "*~",
     # temp files which can be created if process still has handle open of a deleted file
     ".fuse_hidden*",
     # KDE directory preferences
     ".directory",
```

### Comparing `offspot_config-1.9.0/src/offspot_config/file.py` & `offspot_config-2.0.0/src/offspot_config/file.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
 import pathlib
 import urllib.parse
 
 from offspot_config.constants import DATA_PART_PATH, SUPPORTED_UNPACKING_FORMATS
+from offspot_config.inputs.checksum import Checksum
 from offspot_config.utils.download import get_online_rsc_size
 from offspot_config.utils.misc import get_filesize
 
 
 class File:
     """In-Config reference to a file to write to the data partition
 
@@ -25,15 +26,15 @@
 
     one of content or url must be supplied. content has priority"""
 
     kind: str = "file"  # Item interface
 
     unpack_formats: list[str]
 
-    def __init__(self, payload: dict[str, str | int]):
+    def __init__(self, payload: dict[str, str | int | dict[str, str]]):
         self.unpack_formats = ["direct", *SUPPORTED_UNPACKING_FORMATS]
         self.url: urllib.parse.ParseResult | None = None
         self.content: str = str(payload.get("content", "") or "").strip()
 
         if not self.content:
             try:
                 self.url = urllib.parse.urlparse(str(payload["url"]))
@@ -44,19 +45,26 @@
         if not self.to.is_relative_to(DATA_PART_PATH):
             raise ValueError(f"{self.to} not a descendent of {DATA_PART_PATH}")
 
         self.via: str = str(payload.get("via", "direct"))
         if self.via not in self.unpack_formats:
             raise NotImplementedError(f"Unsupported handler `{self.via}`")
 
+        # optional checksum
+        self.checksum = None
+        if "checksum" in payload and isinstance(payload["checksum"], dict):
+            self.checksum = Checksum(**payload["checksum"])
+
         # initialized has unknown
-        self._size: int = int(payload.get("size", -1))
-        self._fullsize: int | None = (
-            int(payload["fullsize"]) if "fullsize" in payload else None
-        )
+        self._size = -1
+        if "size" in payload and isinstance(payload["size"], (int, str)):
+            self._size: int = int(payload["size"])
+        self._fullsize: int | None = None
+        if "fullsize" in payload and isinstance(payload["fullsize"], (int, str)):
+            self._fullsize = int(payload["fullsize"])
 
     @property
     def source(self) -> str:  # Item interface
         return self.geturl()
 
     @property
     def size(self) -> int:  # Item interface
```

### Comparing `offspot_config-1.9.0/src/offspot_config/oci_images.py` & `offspot_config-2.0.0/src/offspot_config/oci_images.py`

 * *Files identical despite different names*

### Comparing `offspot_config-1.9.0/src/offspot_config/packages.py` & `offspot_config-2.0.0/src/offspot_config/packages.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from __future__ import annotations
 
 import re
 import uuid
 
 from attrs import define, field
+from pathvalidate import sanitize_filename
 from typeguard import typechecked
 
 from offspot_config.constants import CONTENT_TARGET_PATH
-from offspot_config.inputs import FileConfig
+from offspot_config.inputs.checksum import Checksum
+from offspot_config.inputs.file import FileConfig
 from offspot_config.oci_images import OCIImage
 from offspot_config.utils.download import get_base64_from
 
 # @typechecked
 # @define(kw_only=True)
 # class BaseImage:
 #     source: str
@@ -39,42 +41,47 @@
 
     def get_download_url(self, download_fqdn: str) -> str | None:  # noqa: ARG002
         return None
 
     def get_download_size(self) -> int | None:
         return None
 
+    def get_download_checksum(self) -> Checksum | None:
+        return None
+
     def to_dashboard_entry(self, fqdn: str, download_fqdn: str | None):
         entry = {
             "ident": self.ident,
             "kind": self.kind,
             "title": self.title,
             "description": self.description,
             "languages": self.languages,
             "tags": self.tags,
             "url": self.get_url(fqdn),
             "icon": get_base64_from(self.icon_url) if self.icon_url else "",
         }
         if self.get_download_url(str(download_fqdn)) and self.get_download_size():
-            entry.update(
-                {
-                    "download": {
-                        "url": self.get_download_url(str(download_fqdn)),
-                        "size": self.get_download_size(),
-                    }
+            download = {
+                "download": {
+                    "url": self.get_download_url(str(download_fqdn)),
+                    "size": self.get_download_size(),
                 }
-            )
+            }
+            if self.get_download_checksum():
+                download["download"]["checksum"] = self.get_download_checksum()
+            entry.update(download)
         return entry
 
 
 @typechecked
 @define(kw_only=True)
 class ZimPackage(Package):
     kind: str = "zim"
     domain: str = "kiwix"
+    download_checksum: Checksum | None = None
 
     ident: str
     name: str
     flavour: str
     version: str
 
     download_url: str
@@ -82,41 +89,52 @@
 
     @property
     def url_path(self):
         return self.name
 
     @property
     def filename(self):
-        return f"{self.url_path}.zim"
+        from offspot_config.zim import from_ident
+
+        info = from_ident(self.ident)
+        fname = sanitize_filename(f"{info.publisher}_{info.name}_{info.flavour}")
+        return f"{fname}.zim"
 
     @property
     def size(self) -> int:
         return self.download_size
 
     def get_url(
         self, fqdn: str, kiwix_domain: str | None = "kiwix", **kwargs  # noqa: ARG002
     ) -> str:
-        return f"//{kiwix_domain}.{fqdn}/viewer#{self.url_path}"
+        # this assumes that the ZIM is stored using self.filename
+        from offspot_config.zim import get_libkiwix_humanid
+
+        return f"//{kiwix_domain}.{fqdn}/viewer#{get_libkiwix_humanid(self.filename)}"
 
     def get_download_url(self, download_fqdn: str) -> str:
         return f"//{download_fqdn}/{self.filename}"
 
     def get_download_size(self) -> int:
         return self.download_size
 
+    def get_download_checksum(self) -> Checksum | None:
+        return self.download_checksum
+
 
 @typechecked
 @define(kw_only=True)
 class AppPackage(Package):
     ident: str
     image: str
     image_filesize: int
     image_fullsize: int
     download_url: str | None = None
     download_size: int | None = None
+    download_checksum: Checksum | None = None
     download_to: str | None = None
     download_via: str | None = "direct"
     # map of global:local environ to pass from config to container
     environ_map: dict[str, str] | None = None
     # custom static/dynamic environ for app
     environ: dict[str, str] | None = None
     # list of volumes to mount in host:container[:ro] format
@@ -160,24 +178,32 @@
         if not self.has_file:
             return None
         return FileConfig(
             to=str(CONTENT_TARGET_PATH / self.filename),
             url=self.download_url,
             via=self.download_via,
             size=self.download_size,
+            checksum=self.download_checksum,
         )
 
+    def get_download_size(self) -> int:
+        return self.download_size or 0
+
+    def get_download_checksum(self) -> Checksum | None:
+        return self.download_checksum
+
 
 @typechecked
 @define(kw_only=True)
 class FilesPackage(Package):
     ident: str
     via: str
     download_url: str
     download_size: int | None = None
+    download_checksum: Checksum | None = None
     target: str | None = None
 
     @property
     def filename(self):
         return self.target if self.target else self.ident
 
     @property
@@ -190,8 +216,15 @@
     def as_fileconfig(self) -> FileConfig:
         return FileConfig(
             to=str(CONTENT_TARGET_PATH / "files" / self.filename),
             url=self.download_url,
             content=None,
             via=self.via,
             size=self.download_size,
+            checksum=self.download_checksum,
         )
+
+    def get_download_size(self) -> int:
+        return self.size
+
+    def get_download_checksum(self) -> Checksum | None:
+        return self.download_checksum
```

### Comparing `offspot_config-1.9.0/src/offspot_config/utils/misc.py` & `offspot_config-2.0.0/src/offspot_config/utils/misc.py`

 * *Files identical despite different names*

### Comparing `offspot_config-1.9.0/src/offspot_config/utils/sizes.py` & `offspot_config-2.0.0/src/offspot_config/utils/sizes.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import math
 
 from offspot_config.file import File
-from offspot_config.inputs import MainConfig
+from offspot_config.inputs.mainconfig import MainConfig
 from offspot_config.oci_images import OCIImage
 
 ONE_GB = int(1e9)
 ONE_GiB = 2**30
 
 
 def round_for_cluster(size: int, cluster_size: int = 512) -> int:
```

### Comparing `offspot_config-1.9.0/src/offspot_config/utils/yaml.py` & `offspot_config-2.0.0/src/offspot_config/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `offspot_config-1.9.0/src/offspot_runtime/ap.py` & `offspot_config-2.0.0/src/offspot_runtime/ap.py`

 * *Files identical despite different names*

### Comparing `offspot_config-1.9.0/src/offspot_runtime/checks.py` & `offspot_config-2.0.0/src/offspot_runtime/checks.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,23 @@
 )
 RE_HOTSPOT_TLD = re.compile(r"^[a-zA-Z][a-zA-Z0-9\-]*$")
 RE_TIMEZONE = re.compile(r"^([a-zA-Z0-9\-\_\/]){1,80}$")
 RE_SSID = re.compile(r'^[^!#;+\]/"\t][^+\]/"\t]{0,31}$')
 RE_PASSPHRASE = re.compile(r"^[\u0020-\u007e]{8,63}$")  # Basic Latin
 RE_IFACE_NAME = re.compile(r"^[a-z][a-z0-9]+[0-9]+$")
 RE_COUNTRY_CODE = re.compile(r"[a-zA-Z]{2}")
+FIRMWARES = {  # chipset: firmwares list
+    "brcm43455": [
+        "raspios",
+        "supports-19_2021-11-30",
+        "supports-24_2021-10-05_noap+sta",
+        "supports-32_2015-03-01_unreliable",
+    ],
+    "brcm43430": ["raspios", "supports-30_2018-09-28"],
+}
 
 
 def port_in_range(range_or_port: str, expected: Union[str, int]) -> bool:
     """whether expected port is in the range_or_port compose string"""
     if not isinstance(range_or_port, str) or not isinstance(expected, (str, int)):
         return False
 
@@ -558,7 +567,20 @@
         check = is_valid_interface_name(iface)
         if not check.passed:
             return CheckResponse(
                 False, f"NoDHCPD-interfaces #{index}: {check.help_text}"
             )
 
     return CheckResponse(True)
+
+
+def is_valid_firmware_for(chipset: str, firmware: str) -> CheckResponse:
+    """whether name represents a valid Timezone value"""
+    if chipset not in FIRMWARES.keys():
+        return CheckResponse(False, "Incorrect WiFi chipset “{chipset}”")
+
+    if firmware not in FIRMWARES[chipset]:
+        return CheckResponse(
+            False, "Incorrect firmware “{firmware}” for {chipset} chipset"
+        )
+
+    return CheckResponse(True)
```

### Comparing `offspot_config-1.9.0/src/offspot_runtime/configlib.py` & `offspot_config-2.0.0/src/offspot_runtime/configlib.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,15 +71,17 @@
 
 
 def warn_unless_root():
     if os.getuid() != 0:
         Config.logger.warning(f"you are not root! uid={os.getuid()}")
 
 
-def simple_run(command: list[str], stdin: Optional[str] = None):
+def simple_run(
+    command: list[str], stdin: Optional[str] = None, *, failsafe: bool = False
+):
     """returncode from running passed command, optionnaly passing str as stdin"""
     Config.logger.debug(f"{command=}")
     try:
         ps = subprocess.run(
             command,
             text=True,
             input=stdin,
@@ -87,15 +89,15 @@
         )
     except Exception as exc:
         if Config.debug:
             Config.logger.exception(exc)
         else:
             Config.logger.error(exc)
         return 1
-    if ps.returncode != 0:
+    if ps.returncode != 0 and not failsafe:
         Config.logger.error(f"{ps.args} failed with returncode {ps.returncode}")
         return 1
     return ps.returncode
 
 
 def get_runtime_bin(name: str) -> list[str]:
     """full path of sub-command script"""
```

### Comparing `offspot_config-1.9.0/src/offspot_runtime/containers.py` & `offspot_config-2.0.0/src/offspot_runtime/containers.py`

 * *Files identical despite different names*

### Comparing `offspot_config-1.9.0/src/offspot_runtime/dnsmasqspoof.py` & `offspot_config-2.0.0/src/offspot_runtime/dnsmasqspoof.py`

 * *Files identical despite different names*

### Comparing `offspot_config-1.9.0/src/offspot_runtime/ethernet.py` & `offspot_config-2.0.0/src/offspot_runtime/ethernet.py`

 * *Files identical despite different names*

### Comparing `offspot_config-1.9.0/src/offspot_runtime/fromfile.py` & `offspot_config-2.0.0/src/offspot_runtime/fromfile.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     requested setting is valid, and set (or errored) or ignored.
     JSON config file is rewritten to remove applied setting """
 import argparse
 import pathlib
 import sys
 
 from offspot_runtime.__about__ import __version__
+from offspot_runtime.checks import FIRMWARES
 from offspot_runtime.configlib import (
     IPTABLES_DIR,
     SYSTEMCTL_PATH,
     Config,
     colored,
     from_yaml,
     get_progname,
@@ -179,14 +180,28 @@
         payload = to_yaml(item)
         command = get_runtime_bin("containers")
         if Config.debug:
             command += ["--debug"]
         command += ["-"]
         return simple_run(command, stdin=payload)
 
+    @staticmethod
+    def config_firmware(item: dict) -> int:
+        if not isinstance(item, dict):
+            return 2
+
+        command = get_runtime_bin("firmware")
+        if Config.debug:
+            command += ["--debug"]
+        for key in FIRMWARES.keys():
+            if item.get(key):
+                command += [f"--{key}", item.get(key)]
+
+        return simple_run(command, failsafe=True)
+
 
 def restore_iptables():
     """restore *persistent* iptables rules using iptables-restore
 
     Uses systemd's `iptables-restore` unit if it exists;
     Otherwise calls iptables-restore individualy for each rules file"""
     svc_name = "iptables-restore"
@@ -222,28 +237,34 @@
     except Exception as exc:
         logger.critical(
             colored(f"Unable to read/parse YAML config at {config_path}: {exc}", "red")
         )
         start_ap_stack()
         return 1
 
-    for key in ("timezone", "hostname", "ethernet", "ap", "containers"):
+    for key in ("firmware", "timezone", "hostname", "ethernet", "ap", "containers"):
         if config.get(key):
             logger.debug(f"[{key}] config change requested")
             returncode = getattr(Handlers, f"config_{key}")(config.get(key))
-            if returncode == 0:
+            if returncode in (0, 100):  # 100 is special code requesting reboot
                 logger.info(f"[{key}] configuration applied")
                 config.pop(key)
                 save_config(config_path, config)
             else:
                 if returncode == 2:
                     logger.error(f"[{key}] incorrect configuration. Please fix")
                 else:
                     logger.critical(f"[{key}] error applying configuration.")
                 has_error = True
+            if returncode == 100:
+                logger.info(
+                    colored("Mandatory reboot requested. rebooting now.", "red")
+                )
+                simple_run(["/usr/sbin/shutdown", "-r", "now"])
+
         elif key == "ap":
             if start_ap_stack() != 0:
                 has_error = True
 
     if has_error:
         return 1
     return succeed("runtime-config applied successfuly")
```

### Comparing `offspot_config-1.9.0/src/offspot_runtime/hostname.py` & `offspot_config-2.0.0/src/offspot_runtime/hostname.py`

 * *Files identical despite different names*

### Comparing `offspot_config-1.9.0/src/offspot_runtime/timezone.py` & `offspot_config-2.0.0/src/offspot_runtime/timezone.py`

 * *Files identical despite different names*

### Comparing `offspot_config-1.9.0/tests/test_checks.py` & `offspot_config-2.0.0/tests/test_checks.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from offspot_runtime.checks import (
     CheckResponse,
     is_valid_ap_config,
     is_valid_compose,
     is_valid_dhcp_range,
     is_valid_domain,
     is_valid_ethernet_config,
+    is_valid_firmware_for,
     is_valid_hostname,
     is_valid_interface_name,
     is_valid_ipv4,
     is_valid_network,
     is_valid_ssid,
     is_valid_timezone,
     is_valid_tld,
@@ -72,14 +73,38 @@
     ],
 )
 def test_hostnames(hostname: str, should_pass: bool):
     check = is_valid_hostname(hostname)
     assert check.passed == should_pass
 
 
+@pytest.mark.parametrize(
+    "chipset, firmware, should_pass",
+    [
+        (1, "raspios", False),
+        ("", "raspios", False),
+        ("brcm43455", 1, False),
+        ("brcm43455", "", False),
+        ("brcm43455", "raspios", True),
+        ("brcm43455", "supports-19_2021-11-30", True),
+        ("brcm43455", "supports-24_2021-10-05_noap+sta", True),
+        ("brcm43455", "supports-32_2015-03-01_unreliable", True),
+        ("brcm43430", "raspios", True),
+        ("brcm43430", "supports-30_2018-09-28", True),
+        ("brcm43455", "supports-30_2018-09-28", False),
+        ("brcm43430", "supports-19_2021-11-30", False),
+        ("brcm43430", "supports-24_2021-10-05_noap+sta", False),
+        ("brcm43430", "supports-32_2015-03-01_unreliable", False),
+    ],
+)
+def test_firmwares(chipset: str, firmware: str, should_pass: bool):
+    check = is_valid_firmware_for(chipset=chipset, firmware=firmware)
+    assert check.passed == should_pass
+
+
 def test_ipv4_api():
     assert is_valid_ipv4("192.168.1.1").passed
     assert is_valid_ipv4("192.168.1.1", usable=True).passed
     assert is_valid_ipv4("192.168.1.1", usable=True).passed
     assert is_valid_ipv4("192.168.1.1", usable=False).passed
     assert not is_valid_ipv4("192.168.1.0", usable=True).passed
     assert is_valid_ipv4("192.168.1.0", usable=False).passed
```

### Comparing `offspot_config-1.9.0/.gitignore` & `offspot_config-2.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `offspot_config-1.9.0/LICENSE` & `offspot_config-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `offspot_config-1.9.0/README.md` & `offspot_config-2.0.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -74,22 +74,64 @@
 
 - No member is required.
 - Unknown members are simply ignored.
 - No relation between first-level members.
 
 ### Valid first-level members
 
-| Member       | Kind      | Function   |
-|--------------|-----------|------------|
+| Member       | Kind      | Function                                               |
+|--------------|-----------|--------------------------------------------------------|
+| `firmware`   | `string`  | Set WiFi firmware to use                               |
 | `timezone`   | `string`  | Set Host timezone                                      |
 | `hostname`   | `string`  | Set machine's hostname (not domain, see `ap`).         |
 | `ethernet`   | `object`  | Set network configuration for ethernet interface       |
 | `ap`         | `object`  | Set WiFi AP configuration for wireless interface       |
 | `containers` | `object`  | Builds the docker-compose file                         |
 
+### `firmware`
+
+`firmware` is itself a single `object`.
+
+| Member       | Kind      | Required | Function                                             |
+|--------------|-----------|----------|------------------------------------------------------|
+| `brcm43455`  | `string`  | no       | Firmware to use for `brcm43455` chipset (Pi 3B+/4/5) |
+| `brcm43430`  | `string`  | no       | Firmware to use for `brcm43430 ` chipset (Pi 0W/3    |
+
+Chipsets included in RaspiOS have limitations on the number of WiFi clients that can connect to it.
+Using this, you can change the version of the firmware to use for your chipset.
+
+Each chipset supports a different set of firmwares.
+
+#### `brcm43455` chipset firmwares
+
+| Firmware                            | Comment                                                                        |
+|-------------------------------------|--------------------------------------------------------------------------------|
+| `raspios`                           | Supports 4/5 clients. Came with RaspiOS                                        |
+| `supports-19_2021-11-30`            | Supports 19 clients. Can be used in AP+STA mode (not supported in Hotspot yet) |
+| `supports-24_2021-10-05_noap+sta`   | Supports 24 clients. Can **not** be used in `AP+STA` mode                      |
+| `supports-32_2015-03-01_unreliable` | Supports 32 clients. **Unreliable**. Available for tests only                  |
+
+#### `brcm43430` chipset firmwares
+
+| Firmware                            | Comment                                                                        |
+|-------------------------------------|--------------------------------------------------------------------------------|
+| `raspios`                           | Supports 4/5 clients. Came with RaspiOS                                        |
+| `supports-30_2018-09-28`            | Supports 30 clients.                                                           |
+
+**⚠️ Warning**: WiFi firmware update **requires a reboot** to be effective.
+
+Example:
+
+```yaml
+---
+firmware:
+  brcm43455: raspios
+  brcm43430: supports-30_2018-09-28
+```
+
 ### `timezone`
 
 Must be a valid timezone. Get a complete list with:
 
 ```sh
 timedatectl list-timezones
 ```
```

### Comparing `offspot_config-1.9.0/pyproject.toml` & `offspot_config-2.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -28,27 +28,28 @@
     "humanfriendly>=10.0",
     "requests>=2.31.0,<3",
     "typeguard>=4.1.5",
     "iso3166==2.1.1",
     "xmltodict>=0.13.0,<0.14",
     "attrs>=23.1.0,<23.2",
     "urllib3>=2.0.0,<3.0",
+    "pathvalidate>=3.0.0,<4.0",
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 scripts = [
   "invoke==2.2.0",
 ]
 lint = [
   "black==24.1.1",
   "ruff==0.1.15",
 ]
 check = [
-  "pyright==1.1.349",
+  "pyright==1.1.358",
 ]
 test = [
   "pytest==8.0.0",
   "coverage==7.4.1",
 ]
 dev = [
   "pre-commit==3.6.0",
@@ -67,14 +68,15 @@
 offspot-runtime-config-ap = "offspot_runtime.ap:entrypoint"
 offspot-runtime-config-containers = "offspot_runtime.containers:entrypoint"
 offspot-runtime-config-ethernet = "offspot_runtime.ethernet:entrypoint"
 offspot-runtime-config-hostname = "offspot_runtime.hostname:entrypoint"
 offspot-runtime-config-timezone = "offspot_runtime.timezone:entrypoint"
 offspot-runtime-config-fromfile = "offspot_runtime.fromfile:entrypoint"
 toggle-dnsmasq-spoof = "offspot_runtime.dnsmasqspoof:entrypoint"
+offspot-runtime-config-firmware = "offspot_runtime.firmware:entrypoint"
 
 [tool.hatch.version]
 path = "src/offspot_runtime/__about__.py"
 
 [tool.hatch.build]
 exclude = [
   "/.github",
@@ -230,19 +232,19 @@
 
 [tool.pytest.ini_options]
 minversion = "7.3"
 testpaths = ["tests"]
 pythonpath = [".", "src"]
 
 [tool.coverage.paths]
-great_project = ["src/offspot_config", "src/offspot_runtime"]
+offspot_config = ["src/offspot_config", "src/offspot_runtime"]
 tests = ["tests"]
 
 [tool.coverage.run]
-source_pkgs = ["offspot_runtime"]
+source_pkgs = ["offspot_runtime", "offspot_config"]
 branch = true
 parallel = true
 omit = [
   "src/offspot_runtime/__about__.py",
 ]
 
 [tool.coverage.report]
```

### Comparing `offspot_config-1.9.0/PKG-INFO` & `offspot_config-2.0.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: offspot-config
-Version: 1.9.0
+Version: 2.0.0
 Summary: Offspot Config helpers
 Project-URL: Homepage, https://github.com/offspot/offspot-config
 Project-URL: Donate, https://www.kiwix.org/en/support-us/
 Author-email: Kiwix <dev@kiwix.org>
 License: GPL-3.0-or-later
 License-File: LICENSE
 Keywords: offspot
@@ -16,28 +16,31 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.9
 Requires-Dist: attrs<23.2,>=23.1.0
 Requires-Dist: docker-export[visual]<2.0,>=1.0.0
 Requires-Dist: humanfriendly>=10.0
 Requires-Dist: iso3166==2.1.1
+Requires-Dist: pathvalidate<4.0,>=3.0.0
 Requires-Dist: pyyaml==6.0.1
 Requires-Dist: requests<3,>=2.31.0
 Requires-Dist: typeguard>=4.1.5
 Requires-Dist: urllib3<3.0,>=2.0.0
 Requires-Dist: xmltodict<0.14,>=0.13.0
 Provides-Extra: check
-Requires-Dist: pyright==1.1.349; extra == 'check'
+Requires-Dist: pyright==1.1.358; extra == 'check'
 Provides-Extra: dev
+Requires-Dist: black==24.1.1; extra == 'dev'
+Requires-Dist: coverage==7.4.1; extra == 'dev'
+Requires-Dist: invoke==2.2.0; extra == 'dev'
 Requires-Dist: ipython==8.20.0; extra == 'dev'
-Requires-Dist: offspot-config[check]; extra == 'dev'
-Requires-Dist: offspot-config[lint]; extra == 'dev'
-Requires-Dist: offspot-config[scripts]; extra == 'dev'
-Requires-Dist: offspot-config[test]; extra == 'dev'
 Requires-Dist: pre-commit==3.6.0; extra == 'dev'
+Requires-Dist: pyright==1.1.358; extra == 'dev'
+Requires-Dist: pytest==8.0.0; extra == 'dev'
+Requires-Dist: ruff==0.1.15; extra == 'dev'
 Provides-Extra: lint
 Requires-Dist: black==24.1.1; extra == 'lint'
 Requires-Dist: ruff==0.1.15; extra == 'lint'
 Provides-Extra: scripts
 Requires-Dist: invoke==2.2.0; extra == 'scripts'
 Provides-Extra: test
 Requires-Dist: coverage==7.4.1; extra == 'test'
@@ -120,22 +123,64 @@
 
 - No member is required.
 - Unknown members are simply ignored.
 - No relation between first-level members.
 
 ### Valid first-level members
 
-| Member       | Kind      | Function   |
-|--------------|-----------|------------|
+| Member       | Kind      | Function                                               |
+|--------------|-----------|--------------------------------------------------------|
+| `firmware`   | `string`  | Set WiFi firmware to use                               |
 | `timezone`   | `string`  | Set Host timezone                                      |
 | `hostname`   | `string`  | Set machine's hostname (not domain, see `ap`).         |
 | `ethernet`   | `object`  | Set network configuration for ethernet interface       |
 | `ap`         | `object`  | Set WiFi AP configuration for wireless interface       |
 | `containers` | `object`  | Builds the docker-compose file                         |
 
+### `firmware`
+
+`firmware` is itself a single `object`.
+
+| Member       | Kind      | Required | Function                                             |
+|--------------|-----------|----------|------------------------------------------------------|
+| `brcm43455`  | `string`  | no       | Firmware to use for `brcm43455` chipset (Pi 3B+/4/5) |
+| `brcm43430`  | `string`  | no       | Firmware to use for `brcm43430 ` chipset (Pi 0W/3    |
+
+Chipsets included in RaspiOS have limitations on the number of WiFi clients that can connect to it.
+Using this, you can change the version of the firmware to use for your chipset.
+
+Each chipset supports a different set of firmwares.
+
+#### `brcm43455` chipset firmwares
+
+| Firmware                            | Comment                                                                        |
+|-------------------------------------|--------------------------------------------------------------------------------|
+| `raspios`                           | Supports 4/5 clients. Came with RaspiOS                                        |
+| `supports-19_2021-11-30`            | Supports 19 clients. Can be used in AP+STA mode (not supported in Hotspot yet) |
+| `supports-24_2021-10-05_noap+sta`   | Supports 24 clients. Can **not** be used in `AP+STA` mode                      |
+| `supports-32_2015-03-01_unreliable` | Supports 32 clients. **Unreliable**. Available for tests only                  |
+
+#### `brcm43430` chipset firmwares
+
+| Firmware                            | Comment                                                                        |
+|-------------------------------------|--------------------------------------------------------------------------------|
+| `raspios`                           | Supports 4/5 clients. Came with RaspiOS                                        |
+| `supports-30_2018-09-28`            | Supports 30 clients.                                                           |
+
+**⚠️ Warning**: WiFi firmware update **requires a reboot** to be effective.
+
+Example:
+
+```yaml
+---
+firmware:
+  brcm43455: raspios
+  brcm43430: supports-30_2018-09-28
+```
+
 ### `timezone`
 
 Must be a valid timezone. Get a complete list with:
 
 ```sh
 timedatectl list-timezones
 ```
```

