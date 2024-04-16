# Comparing `tmp/db_contrib_tool-0.7.1.tar.gz` & `tmp/db_contrib_tool-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "db_contrib_tool-0.7.1.tar", max compression
+gzip compressed data, was "db_contrib_tool-0.7.2.tar", max compression
```

## Comparing `db_contrib_tool-0.7.1.tar` & `db_contrib_tool-0.7.2.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0     6286 2024-04-08 07:29:31.032000 db_contrib_tool-0.7.1/README.md
--rw-r--r--   0        0        0     2184 2024-04-08 07:29:31.032000 db_contrib_tool-0.7.1/pyproject.toml
--rw-r--r--   0        0        0       13 2024-04-08 07:29:31.032000 db_contrib_tool-0.7.1/src/db_contrib_tool/__init__.py
--rw-r--r--   0        0        0      989 2024-04-08 07:29:31.032000 db_contrib_tool-0.7.1/src/db_contrib_tool/cli.py
--rw-r--r--   0        0        0        0 2024-04-08 07:29:31.032000 db_contrib_tool-0.7.1/src/db_contrib_tool/clients/__init__.py
--rw-r--r--   0        0        0     7143 2024-04-08 07:29:31.032000 db_contrib_tool-0.7.1/src/db_contrib_tool/clients/download_client.py
--rw-r--r--   0        0        0     1701 2024-04-08 07:29:31.032000 db_contrib_tool-0.7.1/src/db_contrib_tool/clients/file_service.py
--rw-r--r--   0        0        0     2636 2024-04-08 07:29:31.032000 db_contrib_tool-0.7.1/src/db_contrib_tool/clients/git_client.py
--rw-r--r--   0        0        0      305 2024-04-08 07:29:31.032000 db_contrib_tool-0.7.1/src/db_contrib_tool/clients/io_client.py
--rw-r--r--   0        0        0      984 2024-04-08 07:29:31.032000 db_contrib_tool-0.7.1/src/db_contrib_tool/clients/platform_details.py
--rw-r--r--   0        0        0     2737 2024-04-08 07:29:31.032000 db_contrib_tool-0.7.1/src/db_contrib_tool/clients/resmoke_proxy.py
--rw-r--r--   0        0        0    10275 2024-04-08 07:29:31.032000 db_contrib_tool-0.7.1/src/db_contrib_tool/config/setup_repro_env_config.yml
--rw-r--r--   0        0        0     5999 2024-04-08 07:29:31.032000 db_contrib_tool-0.7.1/src/db_contrib_tool/config.py
--rw-r--r--   0        0        0      445 2024-04-08 07:29:31.032000 db_contrib_tool-0.7.1/src/db_contrib_tool/evg_aware_bisect/README.md
--rw-r--r--   0        0        0     8844 2024-04-08 07:29:31.036000 db_contrib_tool-0.7.1/src/db_contrib_tool/evg_aware_bisect/__init__.py
--rw-r--r--   0        0        0     4639 2024-04-08 07:29:31.036000 db_contrib_tool-0.7.1/src/db_contrib_tool/evg_aware_bisect/cli.py
--rw-r--r--   0        0        0      110 2024-04-08 07:29:31.036000 db_contrib_tool-0.7.1/src/db_contrib_tool/evg_aware_bisect/run_user_script.sh
--rw-r--r--   0        0        0      418 2024-04-08 07:29:31.036000 db_contrib_tool-0.7.1/src/db_contrib_tool/evg_aware_bisect/setup_test_env.sh
--rw-r--r--   0        0        0       52 2024-04-08 07:29:31.036000 db_contrib_tool-0.7.1/src/db_contrib_tool/evg_aware_bisect/teardown_test_env.sh
--rw-r--r--   0        0        0        0 2024-04-08 07:29:31.036000 db_contrib_tool-0.7.1/src/db_contrib_tool/services/__init__.py
--rw-r--r--   0        0        0     9277 2024-04-08 07:29:31.036000 db_contrib_tool-0.7.1/src/db_contrib_tool/services/evergreen_service.py
--rw-r--r--   0        0        0     2404 2024-04-08 07:29:31.036000 db_contrib_tool-0.7.1/src/db_contrib_tool/services/git_service.py
--rw-r--r--   0        0        0     2029 2024-04-08 07:29:31.036000 db_contrib_tool-0.7.1/src/db_contrib_tool/services/platform_service.py
--rw-r--r--   0        0        0       13 2024-04-08 07:29:31.036000 db_contrib_tool-0.7.1/src/db_contrib_tool/setup_mongot_repro_env/__init__.py
--rw-r--r--   0        0        0     3975 2024-04-08 07:29:31.036000 db_contrib_tool-0.7.1/src/db_contrib_tool/setup_mongot_repro_env/cli.py
--rw-r--r--   0        0        0    13806 2024-04-08 07:29:31.036000 db_contrib_tool-0.7.1/src/db_contrib_tool/setup_repro_env/README.md
--rw-r--r--   0        0        0       13 2024-04-08 07:29:31.036000 db_contrib_tool-0.7.1/src/db_contrib_tool/setup_repro_env/__init__.py
--rw-r--r--   0        0        0    18510 2024-04-08 07:29:31.036000 db_contrib_tool-0.7.1/src/db_contrib_tool/setup_repro_env/artifact_discovery_service.py
--rw-r--r--   0        0        0     9874 2024-04-08 07:29:31.036000 db_contrib_tool-0.7.1/src/db_contrib_tool/setup_repro_env/cli.py
--rw-r--r--   0        0        0    10159 2024-04-08 07:29:31.036000 db_contrib_tool-0.7.1/src/db_contrib_tool/setup_repro_env/download_service.py
--rw-r--r--   0        0        0     4796 2024-04-08 07:29:31.036000 db_contrib_tool-0.7.1/src/db_contrib_tool/setup_repro_env/release_discovery_service.py
--rw-r--r--   0        0        0     5586 2024-04-08 07:29:31.036000 db_contrib_tool-0.7.1/src/db_contrib_tool/setup_repro_env/release_models.py
--rw-r--r--   0        0        0     4167 2024-04-08 07:29:31.036000 db_contrib_tool-0.7.1/src/db_contrib_tool/setup_repro_env/request_models.py
--rw-r--r--   0        0        0    10698 2024-04-08 07:29:31.036000 db_contrib_tool-0.7.1/src/db_contrib_tool/setup_repro_env/setup_repro_env.py
--rw-r--r--   0        0        0      615 2024-04-08 07:29:31.036000 db_contrib_tool-0.7.1/src/db_contrib_tool/symbolizer/README.md
--rw-r--r--   0        0        0        0 2024-04-08 07:29:31.036000 db_contrib_tool-0.7.1/src/db_contrib_tool/symbolizer/__init__.py
--rw-r--r--   0        0        0     4190 2024-04-08 07:29:31.036000 db_contrib_tool-0.7.1/src/db_contrib_tool/symbolizer/cli.py
--rw-r--r--   0        0        0     4798 2024-04-08 07:29:31.036000 db_contrib_tool-0.7.1/src/db_contrib_tool/symbolizer/mongo_log_parser_service.py
--rw-r--r--   0        0        0    24229 2024-04-08 07:29:31.036000 db_contrib_tool-0.7.1/src/db_contrib_tool/symbolizer/mongosymb.py
--rw-r--r--   0        0        0     2269 2024-04-08 07:29:31.036000 db_contrib_tool-0.7.1/src/db_contrib_tool/usage_analytics.py
--rw-r--r--   0        0        0      235 2024-04-08 07:29:31.036000 db_contrib_tool-0.7.1/src/db_contrib_tool/utils/__init__.py
--rw-r--r--   0        0        0     1855 2024-04-08 07:29:31.036000 db_contrib_tool-0.7.1/src/db_contrib_tool/utils/build_system_options.py
--rw-r--r--   0        0        0     2072 2024-04-08 07:29:31.036000 db_contrib_tool-0.7.1/src/db_contrib_tool/utils/evergreen_conn.py
--rw-r--r--   0        0        0     1085 2024-04-08 07:29:31.036000 db_contrib_tool-0.7.1/src/db_contrib_tool/utils/filesystem.py
--rw-r--r--   0        0        0    10608 2024-04-08 07:29:31.036000 db_contrib_tool-0.7.1/src/db_contrib_tool/utils/oauth.py
--rw-r--r--   0        0        0     7972 1970-01-01 00:00:00.000000 db_contrib_tool-0.7.1/setup.py
--rw-r--r--   0        0        0     7542 1970-01-01 00:00:00.000000 db_contrib_tool-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0     6286 2024-04-16 06:36:41.992667 db_contrib_tool-0.7.2/README.md
+-rw-r--r--   0        0        0     2184 2024-04-16 06:36:41.992667 db_contrib_tool-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0       13 2024-04-16 06:36:41.992667 db_contrib_tool-0.7.2/src/db_contrib_tool/__init__.py
+-rw-r--r--   0        0        0      989 2024-04-16 06:36:41.992667 db_contrib_tool-0.7.2/src/db_contrib_tool/cli.py
+-rw-r--r--   0        0        0        0 2024-04-16 06:36:41.992667 db_contrib_tool-0.7.2/src/db_contrib_tool/clients/__init__.py
+-rw-r--r--   0        0        0     7143 2024-04-16 06:36:41.992667 db_contrib_tool-0.7.2/src/db_contrib_tool/clients/download_client.py
+-rw-r--r--   0        0        0     1701 2024-04-16 06:36:41.992667 db_contrib_tool-0.7.2/src/db_contrib_tool/clients/file_service.py
+-rw-r--r--   0        0        0     2636 2024-04-16 06:36:41.992667 db_contrib_tool-0.7.2/src/db_contrib_tool/clients/git_client.py
+-rw-r--r--   0        0        0      305 2024-04-16 06:36:41.992667 db_contrib_tool-0.7.2/src/db_contrib_tool/clients/io_client.py
+-rw-r--r--   0        0        0      984 2024-04-16 06:36:41.992667 db_contrib_tool-0.7.2/src/db_contrib_tool/clients/platform_details.py
+-rw-r--r--   0        0        0     2737 2024-04-16 06:36:41.992667 db_contrib_tool-0.7.2/src/db_contrib_tool/clients/resmoke_proxy.py
+-rw-r--r--   0        0        0    10275 2024-04-16 06:36:41.992667 db_contrib_tool-0.7.2/src/db_contrib_tool/config/setup_repro_env_config.yml
+-rw-r--r--   0        0        0     5999 2024-04-16 06:36:41.992667 db_contrib_tool-0.7.2/src/db_contrib_tool/config.py
+-rw-r--r--   0        0        0      445 2024-04-16 06:36:41.992667 db_contrib_tool-0.7.2/src/db_contrib_tool/evg_aware_bisect/README.md
+-rw-r--r--   0        0        0     8844 2024-04-16 06:36:41.996667 db_contrib_tool-0.7.2/src/db_contrib_tool/evg_aware_bisect/__init__.py
+-rw-r--r--   0        0        0     4639 2024-04-16 06:36:41.996667 db_contrib_tool-0.7.2/src/db_contrib_tool/evg_aware_bisect/cli.py
+-rw-r--r--   0        0        0      110 2024-04-16 06:36:41.996667 db_contrib_tool-0.7.2/src/db_contrib_tool/evg_aware_bisect/run_user_script.sh
+-rw-r--r--   0        0        0      418 2024-04-16 06:36:41.996667 db_contrib_tool-0.7.2/src/db_contrib_tool/evg_aware_bisect/setup_test_env.sh
+-rw-r--r--   0        0        0       52 2024-04-16 06:36:41.996667 db_contrib_tool-0.7.2/src/db_contrib_tool/evg_aware_bisect/teardown_test_env.sh
+-rw-r--r--   0        0        0        0 2024-04-16 06:36:41.996667 db_contrib_tool-0.7.2/src/db_contrib_tool/services/__init__.py
+-rw-r--r--   0        0        0     9277 2024-04-16 06:36:41.996667 db_contrib_tool-0.7.2/src/db_contrib_tool/services/evergreen_service.py
+-rw-r--r--   0        0        0     2404 2024-04-16 06:36:41.996667 db_contrib_tool-0.7.2/src/db_contrib_tool/services/git_service.py
+-rw-r--r--   0        0        0     2029 2024-04-16 06:36:41.996667 db_contrib_tool-0.7.2/src/db_contrib_tool/services/platform_service.py
+-rw-r--r--   0        0        0       13 2024-04-16 06:36:41.996667 db_contrib_tool-0.7.2/src/db_contrib_tool/setup_mongot_repro_env/__init__.py
+-rw-r--r--   0        0        0     3990 2024-04-16 06:36:41.996667 db_contrib_tool-0.7.2/src/db_contrib_tool/setup_mongot_repro_env/cli.py
+-rw-r--r--   0        0        0    13806 2024-04-16 06:36:41.996667 db_contrib_tool-0.7.2/src/db_contrib_tool/setup_repro_env/README.md
+-rw-r--r--   0        0        0       13 2024-04-16 06:36:41.996667 db_contrib_tool-0.7.2/src/db_contrib_tool/setup_repro_env/__init__.py
+-rw-r--r--   0        0        0    18510 2024-04-16 06:36:41.996667 db_contrib_tool-0.7.2/src/db_contrib_tool/setup_repro_env/artifact_discovery_service.py
+-rw-r--r--   0        0        0     9874 2024-04-16 06:36:41.996667 db_contrib_tool-0.7.2/src/db_contrib_tool/setup_repro_env/cli.py
+-rw-r--r--   0        0        0    10159 2024-04-16 06:36:41.996667 db_contrib_tool-0.7.2/src/db_contrib_tool/setup_repro_env/download_service.py
+-rw-r--r--   0        0        0     4796 2024-04-16 06:36:41.996667 db_contrib_tool-0.7.2/src/db_contrib_tool/setup_repro_env/release_discovery_service.py
+-rw-r--r--   0        0        0     5586 2024-04-16 06:36:41.996667 db_contrib_tool-0.7.2/src/db_contrib_tool/setup_repro_env/release_models.py
+-rw-r--r--   0        0        0     4167 2024-04-16 06:36:41.996667 db_contrib_tool-0.7.2/src/db_contrib_tool/setup_repro_env/request_models.py
+-rw-r--r--   0        0        0    10698 2024-04-16 06:36:41.996667 db_contrib_tool-0.7.2/src/db_contrib_tool/setup_repro_env/setup_repro_env.py
+-rw-r--r--   0        0        0      615 2024-04-16 06:36:41.996667 db_contrib_tool-0.7.2/src/db_contrib_tool/symbolizer/README.md
+-rw-r--r--   0        0        0        0 2024-04-16 06:36:41.996667 db_contrib_tool-0.7.2/src/db_contrib_tool/symbolizer/__init__.py
+-rw-r--r--   0        0        0     4190 2024-04-16 06:36:41.996667 db_contrib_tool-0.7.2/src/db_contrib_tool/symbolizer/cli.py
+-rw-r--r--   0        0        0     4798 2024-04-16 06:36:41.996667 db_contrib_tool-0.7.2/src/db_contrib_tool/symbolizer/mongo_log_parser_service.py
+-rw-r--r--   0        0        0    24229 2024-04-16 06:36:41.996667 db_contrib_tool-0.7.2/src/db_contrib_tool/symbolizer/mongosymb.py
+-rw-r--r--   0        0        0     2269 2024-04-16 06:36:41.996667 db_contrib_tool-0.7.2/src/db_contrib_tool/usage_analytics.py
+-rw-r--r--   0        0        0      235 2024-04-16 06:36:41.996667 db_contrib_tool-0.7.2/src/db_contrib_tool/utils/__init__.py
+-rw-r--r--   0        0        0     1855 2024-04-16 06:36:41.996667 db_contrib_tool-0.7.2/src/db_contrib_tool/utils/build_system_options.py
+-rw-r--r--   0        0        0     2072 2024-04-16 06:36:41.996667 db_contrib_tool-0.7.2/src/db_contrib_tool/utils/evergreen_conn.py
+-rw-r--r--   0        0        0     1085 2024-04-16 06:36:41.996667 db_contrib_tool-0.7.2/src/db_contrib_tool/utils/filesystem.py
+-rw-r--r--   0        0        0    10608 2024-04-16 06:36:41.996667 db_contrib_tool-0.7.2/src/db_contrib_tool/utils/oauth.py
+-rw-r--r--   0        0        0     7972 1970-01-01 00:00:00.000000 db_contrib_tool-0.7.2/setup.py
+-rw-r--r--   0        0        0     7542 1970-01-01 00:00:00.000000 db_contrib_tool-0.7.2/PKG-INFO
```

### Comparing `db_contrib_tool-0.7.1/README.md` & `db_contrib_tool-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.7.1/pyproject.toml` & `db_contrib_tool-0.7.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "db-contrib-tool"
-version = "0.7.1"
+version = "0.7.2"
 description = "The `db-contrib-tool` - MongoDB's tool for contributors."
 authors = ["DAG team <dev-prod-dag@mongodb.com>"]
 readme = "README.md"
 repository = "https://github.com/10gen/db-contrib-tool"
 include = [
     "src/db_contrib_tool/bisect/*.sh",
     "src/db_contrib_tool/config/*.yml",
```

### Comparing `db_contrib_tool-0.7.1/src/db_contrib_tool/cli.py` & `db_contrib_tool-0.7.2/src/db_contrib_tool/cli.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.7.1/src/db_contrib_tool/clients/download_client.py` & `db_contrib_tool-0.7.2/src/db_contrib_tool/clients/download_client.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.7.1/src/db_contrib_tool/clients/file_service.py` & `db_contrib_tool-0.7.2/src/db_contrib_tool/clients/file_service.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.7.1/src/db_contrib_tool/clients/git_client.py` & `db_contrib_tool-0.7.2/src/db_contrib_tool/clients/git_client.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.7.1/src/db_contrib_tool/clients/platform_details.py` & `db_contrib_tool-0.7.2/src/db_contrib_tool/clients/platform_details.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.7.1/src/db_contrib_tool/clients/resmoke_proxy.py` & `db_contrib_tool-0.7.2/src/db_contrib_tool/clients/resmoke_proxy.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.7.1/src/db_contrib_tool/config/setup_repro_env_config.yml` & `db_contrib_tool-0.7.2/src/db_contrib_tool/config/setup_repro_env_config.yml`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.7.1/src/db_contrib_tool/config.py` & `db_contrib_tool-0.7.2/src/db_contrib_tool/config.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.7.1/src/db_contrib_tool/evg_aware_bisect/__init__.py` & `db_contrib_tool-0.7.2/src/db_contrib_tool/evg_aware_bisect/__init__.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.7.1/src/db_contrib_tool/evg_aware_bisect/cli.py` & `db_contrib_tool-0.7.2/src/db_contrib_tool/evg_aware_bisect/cli.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.7.1/src/db_contrib_tool/services/evergreen_service.py` & `db_contrib_tool-0.7.2/src/db_contrib_tool/services/evergreen_service.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.7.1/src/db_contrib_tool/services/git_service.py` & `db_contrib_tool-0.7.2/src/db_contrib_tool/services/git_service.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.7.1/src/db_contrib_tool/services/platform_service.py` & `db_contrib_tool-0.7.2/src/db_contrib_tool/services/platform_service.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.7.1/src/db_contrib_tool/setup_mongot_repro_env/cli.py` & `db_contrib_tool-0.7.2/src/db_contrib_tool/setup_mongot_repro_env/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -85,45 +85,43 @@
     version: str,
 ) -> None:
     """
     Set up Mongot repro environment.
 
     Downloads and installs particular Mongot versions into install directory.
 
-    Accepts `latest` currently, eventually will accept `release` as well.
+    Accepts `latest` and `release` versions.
 
-    If no version and no architecture are specified the lastest linux_x86_64 binary will be installed.
+    If no version and no architecture are specified the latest linux_x86_64 binary will be installed.
     """
-    # TODO SERVER-85978 support downloading release versions of mongot.
-    if version == "release":
-        raise ValueError(
-            "setup-mongot-repro-env doesn't currently support downloading releases of mongot"
-        )
     setup_logging(True)
-    primaryUrl = (
-        "https://mciuploads.s3.amazonaws.com/fts/atlas-search-localdev/"
-        + massage_binary_name(version, architecture, _platform)
-    )
 
     inject.configure()
     artifact_download_service = inject.instance(ArtifactDownloadService)
     artifact_download_service.download_with_retries(
-        DownloadUrl(primary=primaryUrl), os.path.abspath(install_dir), True
+        DownloadUrl(primary=massage_url_path(version, architecture, _platform)),
+        os.path.abspath(install_dir),
+        True,
     )
 
 
-def massage_binary_name(version: str, architecture: str, platform: str) -> str:
+def massage_url_path(version: str, architecture: str, platform: str) -> str:
     """
-    Return binary name to be referenced in the url passed to download_with_retries.
+    Return url path to be used for downloading appropriate mongot binary.
+
+    10gen/mongot releases latest and production binaries to constant/hardcoded S3 links.
+    In this way, the latest describes the binaries created by the most recent commit merged to 10gen/mongot.
+    Release refers to the mongot binaries running in atlas prod.
 
-    10gen/mongot releases binaries to constant/hardcoded S3 links. In other words, each commit to 10gen/mongot
-    pushes new binaries to the same set of links. This function processes input parameters to figure out the
-    desired binary type (release or latest of given arch + platform combo).
+    This function processes input parameters to figure out the
+    desired url path (release or latest of given arch + platform combo). Release and latest versions differ only in
+    the url path, as binary names stay the same across both versions (for any given arch + platform combo).
 
-    Until release downloads are supported, possible binary names only include:
+    As macos with aarch64 is not supported, possible binary names would be:
     - mongot_latest_linux_x86_64.tgz
     - mongot_latest_linux_aarch64.tgz
     - mongot_latest_macos_x86_64.tgz
     """
     if platform == "macos" and architecture == "aarch64":
         raise ValueError("Mongot doesn't support macos with aarch64 architecture")
-    return f"mongot_{version}_{platform}_{architecture}.tgz"
+    url_version_path = "release" if version == "release" else "atlas-search-localdev"
+    return f"https://mciuploads.s3.amazonaws.com/fts/{url_version_path}/mongot_latest_{platform}_{architecture}.tgz"
```

### Comparing `db_contrib_tool-0.7.1/src/db_contrib_tool/setup_repro_env/README.md` & `db_contrib_tool-0.7.2/src/db_contrib_tool/setup_repro_env/README.md`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.7.1/src/db_contrib_tool/setup_repro_env/artifact_discovery_service.py` & `db_contrib_tool-0.7.2/src/db_contrib_tool/setup_repro_env/artifact_discovery_service.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.7.1/src/db_contrib_tool/setup_repro_env/cli.py` & `db_contrib_tool-0.7.2/src/db_contrib_tool/setup_repro_env/cli.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.7.1/src/db_contrib_tool/setup_repro_env/download_service.py` & `db_contrib_tool-0.7.2/src/db_contrib_tool/setup_repro_env/download_service.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.7.1/src/db_contrib_tool/setup_repro_env/release_discovery_service.py` & `db_contrib_tool-0.7.2/src/db_contrib_tool/setup_repro_env/release_discovery_service.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.7.1/src/db_contrib_tool/setup_repro_env/release_models.py` & `db_contrib_tool-0.7.2/src/db_contrib_tool/setup_repro_env/release_models.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.7.1/src/db_contrib_tool/setup_repro_env/request_models.py` & `db_contrib_tool-0.7.2/src/db_contrib_tool/setup_repro_env/request_models.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.7.1/src/db_contrib_tool/setup_repro_env/setup_repro_env.py` & `db_contrib_tool-0.7.2/src/db_contrib_tool/setup_repro_env/setup_repro_env.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.7.1/src/db_contrib_tool/symbolizer/README.md` & `db_contrib_tool-0.7.2/src/db_contrib_tool/symbolizer/README.md`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.7.1/src/db_contrib_tool/symbolizer/cli.py` & `db_contrib_tool-0.7.2/src/db_contrib_tool/symbolizer/cli.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.7.1/src/db_contrib_tool/symbolizer/mongo_log_parser_service.py` & `db_contrib_tool-0.7.2/src/db_contrib_tool/symbolizer/mongo_log_parser_service.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.7.1/src/db_contrib_tool/symbolizer/mongosymb.py` & `db_contrib_tool-0.7.2/src/db_contrib_tool/symbolizer/mongosymb.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.7.1/src/db_contrib_tool/usage_analytics.py` & `db_contrib_tool-0.7.2/src/db_contrib_tool/usage_analytics.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.7.1/src/db_contrib_tool/utils/build_system_options.py` & `db_contrib_tool-0.7.2/src/db_contrib_tool/utils/build_system_options.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.7.1/src/db_contrib_tool/utils/evergreen_conn.py` & `db_contrib_tool-0.7.2/src/db_contrib_tool/utils/evergreen_conn.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.7.1/src/db_contrib_tool/utils/filesystem.py` & `db_contrib_tool-0.7.2/src/db_contrib_tool/utils/filesystem.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.7.1/src/db_contrib_tool/utils/oauth.py` & `db_contrib_tool-0.7.2/src/db_contrib_tool/utils/oauth.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.7.1/setup.py` & `db_contrib_tool-0.7.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
  'tenacity>=8.0.1,<9.0.0']
 
 entry_points = \
 {'console_scripts': ['db-contrib-tool = db_contrib_tool.cli:cli']}
 
 setup_kwargs = {
     'name': 'db-contrib-tool',
-    'version': '0.7.1',
+    'version': '0.7.2',
     'description': "The `db-contrib-tool` - MongoDB's tool for contributors.",
     'long_description': '# db-contrib-tool\n\nThe `db-contrib-tool` - MongoDB\'s tools for contributors.\n\n## Table of contents\n\n- [db-contrib-tool](#db-contrib-tool)\n  - [Table of contents](#table-of-contents)\n  - [Description](#description)\n  - [Dependencies](#dependencies)\n  - [Installation](#installation)\n  - [Usage](#usage)\n  - [Contributor\'s Guide (local development)](#contributors-guide-local-development)\n    - [Install project dependencies](#install-project-dependencies)\n    - [Run command line tool (local development)](#run-command-line-tool-local-development)\n    - [Run linters](#run-linters)\n    - [Run tests](#run-tests)\n    - [Pre-commit](#pre-commit)\n    - [Testing changes in mongo](#testing-changes-in-mongo)\n    - [Testing changes locally](#testing-changes-locally)\n    - [Versioning](#versioning)\n    - [Code Review](#code-review)\n    - [Deployment](#deployment)\n\n## Description\n\nThe command line tool with various subcommands:\n- `bisect`\n  - [README.md](src/db_contrib_tool/evg_aware_bisect/README.md)\n  - performs an evergreen-aware git-bisect to find the \'last passing version\' and \'first failing version\' of mongo\n- `setup-repro-env`\n  - [README.md](src/db_contrib_tool/setup_repro_env/README.md)\n  - downloads and installs:\n    - particular MongoDB versions\n    - debug symbols\n    - artifacts (including resmoke, python scripts etc)\n    - python venv for resmoke, python scripts etc\n- `symbolize`\n  - [README.md](src/db_contrib_tool/symbolizer/README.md)\n  - Symbolizes stacktraces from recent `mongod` and `mongos` binaries compiled in Evergreen, including patch builds, mainline builds, and release/production builds.\n  - Requires authenticating to an internal MongoDB symbol mapping service.\n\n## Dependencies\n\n- Python 3.9 or later (python3 from the [MongoDB Toolchain](https://github.com/10gen/toolchain-builder/blob/master/INSTALL.md) is highly recommended)\n\n## Installation\n\nMake sure [dependencies](#dependencies) are installed.\nUse [pipx](https://pypa.github.io/pipx/) to install db-contrib-tool that will be available globally on your machine:\n\n```bash\npython3 -m pip install pipx\npython3 -m pipx ensurepath\n```\n\nInstalling db-contrib-tool:\n\n```bash\npython3 -m pipx install db-contrib-tool\n```\n\nUpgrading db-contrib-tool:\n\n```bash\npython3 -m pipx upgrade db-contrib-tool\n```\n\nIn case of installation errors, some of them may be related to pipx and could be fixed by re-installing pipx.\n\nRemoving pipx completely (WARNING! This will delete everything that is installed and managed by pipx):\n\n```bash\npython3 -m pip uninstall pipx\nrm -rf ~/.local/pipx  # in case you\'re using the default pipx home directory\n```\n\nNow you can try to install again from scratch.\n\n## Usage\n\nPrint out help message:\n\n```bash\ndb-contrib-tool --help\n```\n\nFor more information see [description](#description) section.\n\n## Contributor\'s Guide (local development)\n\n### Install project dependencies\n\nThis project uses [poetry](https://python-poetry.org/) for dependency management.\n\n```bash\npoetry install\n```\n\n### Run command line tool (local development)\n\nSome subcommands like `bisect` and `symbolize` could be tested from the db-contrib-tool repo root:\n\n```bash\npoetry run db-contrib-tool --help\n```\n\nFor `setup-repro-env` some features can also be tested from the db-contrib-tool repo root,\nbut full features are available when running from mongo repo root.\nSee [testing changes locally](#testing-changes-locally) section.\n\n### Run linters\n\n```bash\npoetry run isort src tests\npoetry run black src tests\n```\n\n### Run tests\n\n```bash\npoetry run pytest\n```\n\n### Pre-commit\n\nThis project has [pre-commit](https://pre-commit.com/) configured. Pre-commit will run\nconfigured checks at git commit time.<br>\nTo enable pre-commit on your local repository run:\n```bash\npoetry run pre-commit install\n```\n\nTo run pre-commit manually:\n```bash\npoetry run pre-commit run\n```\n\n### Testing changes in mongo\n\nThis tool is used to help run tests in the mongodb/mongo repository. On occasion, it may be\ndesirable to run a mongodb-mongo-* patch build with in-flight changes to this repository. The\nfollowing steps can be taken to accomplish that.\n\n- Create a branch with the changes you wish to test.\n- Push the branch to the origin repository: `git push -u origin <branch_name>`.\n- In the "mongo" repository, edit the [evergreen/prelude_db_contrib_tool.sh](https://github.com/10gen/mongo/blob/bbdc1347cdf2533f81b6fd05715c4ef1a092f5a6/evergreen/prelude_db_contrib_tool.sh#L12)\n  to install from the git repository instead of from pypi:\n\n  ```bash\n  pipx install "git+ssh://git@github.com/<user_name>/db-contrib-tool.git@<branch_name>" || exit 1\n  ```\n\n- Create a patch build.\n\nThe patch build should now pull down the changes from your branch instead of using the published\ndb-contrib-tool.\n\n**Note**: Since the db-contrib-tool is pulled from your branch, if you need to make additional\nchanges to the tool, you can just push to the branch and then restart the desired tasks. There is\nno need to create an additional patch build unless you also need to make updates to the mongo\nrepository.\n\n### Testing changes locally\n\nPipx installation recommendations can be found in [installation](#installation) section.\n\nThe tool can be installed via pipx from your local repo:\n\n```bash\npython3 -m pipx install /path/to/db-contrib-tool/repo/root/dir\n```\n\nIf the tool is already installed you can force install an updated version using --force flag:\n\n```bash\npython3 -m pipx install --force /path/to/db-contrib-tool/repo/root/dir\n```\n\nAfter these steps you can run in-development version of db-contrib-tool from any directory:\n\n```bash\ndb-contrib-tool --help\n```\n\n### Versioning\n\nThis project uses [semver](https://semver.org/) for versioning.\nPlease include a description what is added for each new version in `CHANGELOG.md`.\n\n### Code Review\n\nPlease open a GitHub Pull Request for code review.\nThis project uses the [Evergreen Commit Queue](https://docs.devprod.prod.corp.mongodb.com/evergreen/Project-Configuration/Commit-Queue).\nAdd a PR comment with `evergreen merge` to trigger a merge.\n\n### Deployment\n\nDeployment to pypi is done by [deploy](https://spruce.mongodb.com/commits/db-contrib-tool?taskNames=deploy)\ntask of `db-contrib-tool` project in Evergreen.\nA new version in Evergreen is created on merges to `main` branch.\n',
     'author': 'DAG team',
     'author_email': 'dev-prod-dag@mongodb.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/10gen/db-contrib-tool',
```

### Comparing `db_contrib_tool-0.7.1/PKG-INFO` & `db_contrib_tool-0.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: db-contrib-tool
-Version: 0.7.1
+Version: 0.7.2
 Summary: The `db-contrib-tool` - MongoDB's tool for contributors.
 Home-page: https://github.com/10gen/db-contrib-tool
 Author: DAG team
 Author-email: dev-prod-dag@mongodb.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

