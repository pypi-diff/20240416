# Comparing `tmp/hashboard-cli-1.0.7.tar.gz` & `tmp/hashboard_cli-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/dse/code/glean-cli/dist/.tmp-gouya2oo/hashboard-cli-1.0.7.tar", last modified: Fri Jan 26 20:41:09 2024, max compression
+gzip compressed data, was "hashboard_cli-1.0.8.tar", last modified: Tue Apr 16 14:51:46 2024, max compression
```

## Comparing `hashboard-cli-1.0.7.tar` & `hashboard_cli-1.0.8.tar`

### file list

```diff
@@ -1,47 +1,46 @@
-drwxr-xr-x   0 dse        (501) staff       (20)        0 2024-01-26 20:41:09.000000 hashboard-cli-1.0.7/
--rw-r--r--   0 dse        (501) staff       (20)    11357 2021-08-09 13:38:38.000000 hashboard-cli-1.0.7/LICENSE
--rw-r--r--   0 dse        (501) staff       (20)      610 2024-01-26 20:41:09.000000 hashboard-cli-1.0.7/PKG-INFO
--rw-r--r--   0 dse        (501) staff       (20)      141 2023-12-27 16:23:17.000000 hashboard-cli-1.0.7/README.md
--rw-r--r--   0 dse        (501) staff       (20)      104 2023-08-24 19:56:44.000000 hashboard-cli-1.0.7/pyproject.toml
--rw-r--r--   0 dse        (501) staff       (20)      837 2024-01-26 20:41:09.000000 hashboard-cli-1.0.7/setup.cfg
--rw-r--r--   0 dse        (501) staff       (20)       38 2021-09-03 21:01:45.000000 hashboard-cli-1.0.7/setup.py
-drwxr-xr-x   0 dse        (501) staff       (20)        0 2024-01-26 20:41:09.000000 hashboard-cli-1.0.7/src/
-drwxr-xr-x   0 dse        (501) staff       (20)        0 2024-01-26 20:41:09.000000 hashboard-cli-1.0.7/src/hashboard/
--rw-r--r--   0 dse        (501) staff       (20)       18 2024-01-26 20:40:40.000000 hashboard-cli-1.0.7/src/hashboard/__init__.py
-drwxr-xr-x   0 dse        (501) staff       (20)        0 2024-01-26 20:41:09.000000 hashboard-cli-1.0.7/src/hashboard/api/
--rw-r--r--   0 dse        (501) staff       (20)    11443 2023-09-22 19:12:00.000000 hashboard-cli-1.0.7/src/hashboard/api/__init__.py
-drwxr-xr-x   0 dse        (501) staff       (20)        0 2024-01-26 20:41:09.000000 hashboard-cli-1.0.7/src/hashboard/api/access_keys/
--rw-r--r--   0 dse        (501) staff       (20)        0 2023-09-07 12:15:00.000000 hashboard-cli-1.0.7/src/hashboard/api/access_keys/__init__.py
--rw-r--r--   0 dse        (501) staff       (20)     4227 2023-09-14 16:54:13.000000 hashboard-cli-1.0.7/src/hashboard/api/access_keys/browser_auth.py
--rw-r--r--   0 dse        (501) staff       (20)     4409 2024-01-26 20:40:40.000000 hashboard-cli-1.0.7/src/hashboard/api/access_keys/existing_user.py
--rw-r--r--   0 dse        (501) staff       (20)     4117 2023-09-14 16:54:13.000000 hashboard-cli-1.0.7/src/hashboard/api/access_keys/new_user.py
--rw-r--r--   0 dse        (501) staff       (20)     2143 2024-01-26 20:40:40.000000 hashboard-cli-1.0.7/src/hashboard/api/access_keys/utils.py
-drwxr-xr-x   0 dse        (501) staff       (20)        0 2024-01-26 20:41:09.000000 hashboard-cli-1.0.7/src/hashboard/api/analytics/
--rw-r--r--   0 dse        (501) staff       (20)      900 2023-12-27 16:23:17.000000 hashboard-cli-1.0.7/src/hashboard/api/analytics/__init__.py
--rw-r--r--   0 dse        (501) staff       (20)     4003 2023-12-27 16:23:17.000000 hashboard-cli-1.0.7/src/hashboard/api/analytics/cli_with_tracking.py
--rw-r--r--   0 dse        (501) staff       (20)      143 2023-09-07 12:15:00.000000 hashboard-cli-1.0.7/src/hashboard/api/analytics/events.py
--rw-r--r--   0 dse        (501) staff       (20)    31549 2024-01-26 20:40:40.000000 hashboard-cli-1.0.7/src/hashboard/cli.py
--rw-r--r--   0 dse        (501) staff       (20)      346 2023-09-14 16:54:13.000000 hashboard-cli-1.0.7/src/hashboard/constants.py
--rw-r--r--   0 dse        (501) staff       (20)     1744 2023-09-14 16:54:13.000000 hashboard-cli-1.0.7/src/hashboard/credentials.py
--rw-r--r--   0 dse        (501) staff       (20)     3920 2023-09-07 12:15:00.000000 hashboard-cli-1.0.7/src/hashboard/filesystem.py
--rw-r--r--   0 dse        (501) staff       (20)      597 2023-12-27 16:23:17.000000 hashboard-cli-1.0.7/src/hashboard/session.py
-drwxr-xr-x   0 dse        (501) staff       (20)        0 2024-01-26 20:41:09.000000 hashboard-cli-1.0.7/src/hashboard/utils/
--rw-r--r--   0 dse        (501) staff       (20)        0 2023-09-07 12:15:00.000000 hashboard-cli-1.0.7/src/hashboard/utils/__init__.py
--rw-r--r--   0 dse        (501) staff       (20)      665 2023-09-07 12:15:00.000000 hashboard-cli-1.0.7/src/hashboard/utils/cli.py
--rw-r--r--   0 dse        (501) staff       (20)      230 2023-09-07 12:15:00.000000 hashboard-cli-1.0.7/src/hashboard/utils/env.py
--rw-r--r--   0 dse        (501) staff       (20)     2922 2023-12-27 16:23:17.000000 hashboard-cli-1.0.7/src/hashboard/utils/grn.py
--rw-r--r--   0 dse        (501) staff       (20)      941 2023-09-07 12:15:00.000000 hashboard-cli-1.0.7/src/hashboard/utils/input_validation.py
--rw-r--r--   0 dse        (501) staff       (20)     1468 2023-09-07 12:15:00.000000 hashboard-cli-1.0.7/src/hashboard/utils/resource.py
--rw-r--r--   0 dse        (501) staff       (20)     1176 2023-09-07 12:15:00.000000 hashboard-cli-1.0.7/src/hashboard/utils/validate_config.py
-drwxr-xr-x   0 dse        (501) staff       (20)        0 2024-01-26 20:41:09.000000 hashboard-cli-1.0.7/src/hashboard_cli.egg-info/
--rw-r--r--   0 dse        (501) staff       (20)      610 2024-01-26 20:41:09.000000 hashboard-cli-1.0.7/src/hashboard_cli.egg-info/PKG-INFO
--rw-r--r--   0 dse        (501) staff       (20)     1149 2024-01-26 20:41:09.000000 hashboard-cli-1.0.7/src/hashboard_cli.egg-info/SOURCES.txt
--rw-r--r--   0 dse        (501) staff       (20)        1 2024-01-26 20:41:09.000000 hashboard-cli-1.0.7/src/hashboard_cli.egg-info/dependency_links.txt
--rw-r--r--   0 dse        (501) staff       (20)       42 2024-01-26 20:41:09.000000 hashboard-cli-1.0.7/src/hashboard_cli.egg-info/entry_points.txt
--rw-r--r--   0 dse        (501) staff       (20)      103 2024-01-26 20:41:09.000000 hashboard-cli-1.0.7/src/hashboard_cli.egg-info/requires.txt
--rw-r--r--   0 dse        (501) staff       (20)       10 2024-01-26 20:41:09.000000 hashboard-cli-1.0.7/src/hashboard_cli.egg-info/top_level.txt
-drwxr-xr-x   0 dse        (501) staff       (20)        0 2024-01-26 20:41:09.000000 hashboard-cli-1.0.7/tests/
--rw-r--r--   0 dse        (501) staff       (20)      310 2023-09-07 12:15:00.000000 hashboard-cli-1.0.7/tests/test_cli.py
--rw-r--r--   0 dse        (501) staff       (20)     1534 2023-09-14 16:54:13.000000 hashboard-cli-1.0.7/tests/test_credentials.py
--rw-r--r--   0 dse        (501) staff       (20)     4619 2023-09-07 12:15:00.000000 hashboard-cli-1.0.7/tests/test_filesystem.py
--rw-r--r--   0 dse        (501) staff       (20)      668 2023-09-07 12:15:00.000000 hashboard-cli-1.0.7/tests/test_hashboard_api.py
+drwxr-xr-x   0 elagulsen   (501) staff       (20)        0 2024-04-16 14:51:46.738848 hashboard_cli-1.0.8/
+-rw-r--r--   0 elagulsen   (501) staff       (20)    11357 2023-08-14 18:27:21.000000 hashboard_cli-1.0.8/LICENSE
+-rw-r--r--   0 elagulsen   (501) staff       (20)      859 2024-04-16 14:51:46.738788 hashboard_cli-1.0.8/PKG-INFO
+-rw-r--r--   0 elagulsen   (501) staff       (20)      141 2024-04-11 15:34:55.000000 hashboard_cli-1.0.8/README.md
+-rw-r--r--   0 elagulsen   (501) staff       (20)      104 2023-08-15 19:32:06.000000 hashboard_cli-1.0.8/pyproject.toml
+-rw-r--r--   0 elagulsen   (501) staff       (20)      837 2024-04-16 14:51:46.739091 hashboard_cli-1.0.8/setup.cfg
+-rw-r--r--   0 elagulsen   (501) staff       (20)       38 2023-08-14 18:27:21.000000 hashboard_cli-1.0.8/setup.py
+drwxr-xr-x   0 elagulsen   (501) staff       (20)        0 2024-04-16 14:51:46.732293 hashboard_cli-1.0.8/src/
+drwxr-xr-x   0 elagulsen   (501) staff       (20)        0 2024-04-16 14:51:46.734675 hashboard_cli-1.0.8/src/hashboard/
+-rw-r--r--   0 elagulsen   (501) staff       (20)       18 2024-04-16 14:49:42.000000 hashboard_cli-1.0.8/src/hashboard/__init__.py
+drwxr-xr-x   0 elagulsen   (501) staff       (20)        0 2024-04-16 14:51:46.734942 hashboard_cli-1.0.8/src/hashboard/api/
+-rw-r--r--   0 elagulsen   (501) staff       (20)    13660 2024-04-16 14:49:42.000000 hashboard_cli-1.0.8/src/hashboard/api/__init__.py
+drwxr-xr-x   0 elagulsen   (501) staff       (20)        0 2024-04-16 14:51:46.735592 hashboard_cli-1.0.8/src/hashboard/api/access_keys/
+-rw-r--r--   0 elagulsen   (501) staff       (20)        0 2023-09-13 19:44:14.000000 hashboard_cli-1.0.8/src/hashboard/api/access_keys/__init__.py
+-rw-r--r--   0 elagulsen   (501) staff       (20)     4227 2023-09-13 19:44:14.000000 hashboard_cli-1.0.8/src/hashboard/api/access_keys/browser_auth.py
+-rw-r--r--   0 elagulsen   (501) staff       (20)     4409 2024-04-11 15:34:55.000000 hashboard_cli-1.0.8/src/hashboard/api/access_keys/existing_user.py
+-rw-r--r--   0 elagulsen   (501) staff       (20)     2143 2024-04-11 15:34:55.000000 hashboard_cli-1.0.8/src/hashboard/api/access_keys/utils.py
+drwxr-xr-x   0 elagulsen   (501) staff       (20)        0 2024-04-16 14:51:46.736025 hashboard_cli-1.0.8/src/hashboard/api/analytics/
+-rw-r--r--   0 elagulsen   (501) staff       (20)      900 2024-04-11 15:34:55.000000 hashboard_cli-1.0.8/src/hashboard/api/analytics/__init__.py
+-rw-r--r--   0 elagulsen   (501) staff       (20)     4003 2024-04-11 15:34:55.000000 hashboard_cli-1.0.8/src/hashboard/api/analytics/cli_with_tracking.py
+-rw-r--r--   0 elagulsen   (501) staff       (20)       20 2024-04-12 14:43:11.000000 hashboard_cli-1.0.8/src/hashboard/api/analytics/events.py
+-rw-r--r--   0 elagulsen   (501) staff       (20)    38904 2024-04-16 14:49:42.000000 hashboard_cli-1.0.8/src/hashboard/cli.py
+-rw-r--r--   0 elagulsen   (501) staff       (20)      346 2023-09-13 19:44:14.000000 hashboard_cli-1.0.8/src/hashboard/constants.py
+-rw-r--r--   0 elagulsen   (501) staff       (20)     1744 2023-09-13 19:44:14.000000 hashboard_cli-1.0.8/src/hashboard/credentials.py
+-rw-r--r--   0 elagulsen   (501) staff       (20)     3843 2024-04-16 14:49:42.000000 hashboard_cli-1.0.8/src/hashboard/filesystem.py
+-rw-r--r--   0 elagulsen   (501) staff       (20)      597 2024-04-11 15:34:55.000000 hashboard_cli-1.0.8/src/hashboard/session.py
+drwxr-xr-x   0 elagulsen   (501) staff       (20)        0 2024-04-16 14:51:46.737039 hashboard_cli-1.0.8/src/hashboard/utils/
+-rw-r--r--   0 elagulsen   (501) staff       (20)        0 2023-09-13 19:44:14.000000 hashboard_cli-1.0.8/src/hashboard/utils/__init__.py
+-rw-r--r--   0 elagulsen   (501) staff       (20)      665 2023-09-13 19:44:14.000000 hashboard_cli-1.0.8/src/hashboard/utils/cli.py
+-rw-r--r--   0 elagulsen   (501) staff       (20)     1977 2024-04-16 14:49:42.000000 hashboard_cli-1.0.8/src/hashboard/utils/config.py
+-rw-r--r--   0 elagulsen   (501) staff       (20)      230 2023-09-13 19:44:14.000000 hashboard_cli-1.0.8/src/hashboard/utils/env.py
+-rw-r--r--   0 elagulsen   (501) staff       (20)     2922 2024-04-11 15:34:55.000000 hashboard_cli-1.0.8/src/hashboard/utils/grn.py
+-rw-r--r--   0 elagulsen   (501) staff       (20)      941 2023-09-13 19:44:14.000000 hashboard_cli-1.0.8/src/hashboard/utils/input_validation.py
+-rw-r--r--   0 elagulsen   (501) staff       (20)     1468 2023-09-13 19:44:14.000000 hashboard_cli-1.0.8/src/hashboard/utils/resource.py
+drwxr-xr-x   0 elagulsen   (501) staff       (20)        0 2024-04-16 14:51:46.738501 hashboard_cli-1.0.8/src/hashboard_cli.egg-info/
+-rw-r--r--   0 elagulsen   (501) staff       (20)      859 2024-04-16 14:51:46.000000 hashboard_cli-1.0.8/src/hashboard_cli.egg-info/PKG-INFO
+-rw-r--r--   0 elagulsen   (501) staff       (20)     1098 2024-04-16 14:51:46.000000 hashboard_cli-1.0.8/src/hashboard_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 elagulsen   (501) staff       (20)        1 2024-04-16 14:51:46.000000 hashboard_cli-1.0.8/src/hashboard_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 elagulsen   (501) staff       (20)       42 2024-04-16 14:51:46.000000 hashboard_cli-1.0.8/src/hashboard_cli.egg-info/entry_points.txt
+-rw-r--r--   0 elagulsen   (501) staff       (20)      103 2024-04-16 14:51:46.000000 hashboard_cli-1.0.8/src/hashboard_cli.egg-info/requires.txt
+-rw-r--r--   0 elagulsen   (501) staff       (20)       10 2024-04-16 14:51:46.000000 hashboard_cli-1.0.8/src/hashboard_cli.egg-info/top_level.txt
+drwxr-xr-x   0 elagulsen   (501) staff       (20)        0 2024-04-16 14:51:46.738310 hashboard_cli-1.0.8/tests/
+-rw-r--r--   0 elagulsen   (501) staff       (20)      310 2023-09-13 19:44:14.000000 hashboard_cli-1.0.8/tests/test_cli.py
+-rw-r--r--   0 elagulsen   (501) staff       (20)     1534 2023-09-13 19:44:14.000000 hashboard_cli-1.0.8/tests/test_credentials.py
+-rw-r--r--   0 elagulsen   (501) staff       (20)     3890 2024-04-16 14:49:42.000000 hashboard_cli-1.0.8/tests/test_filesystem.py
+-rw-r--r--   0 elagulsen   (501) staff       (20)      668 2023-09-13 19:44:14.000000 hashboard_cli-1.0.8/tests/test_hashboard_api.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `hashboard-cli-1.0.7/LICENSE` & `hashboard_cli-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `hashboard-cli-1.0.7/setup.cfg` & `hashboard_cli-1.0.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `hashboard-cli-1.0.7/src/hashboard/api/__init__.py` & `hashboard_cli-1.0.8/src/hashboard/api/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -47,40 +47,46 @@
     session: Session,
     project_id: str,
     git_revision: Optional[str],
     git_path: Optional[str],
     deploy: bool,
     allow_dangerous_empty_build: bool = False,
     dbt_manifest_path: Optional[PurePath] = None,
+    async_build=False,
 ):
     """Creates a build based on a git revision and returns the result."""
     build_spec = {
         "configFilesFromGit": {
             "revision": git_revision,
             "path": git_path,
             "dbtManifestPath": dbt_manifest_path,
         }
     }
-    return _create_build(
+
+    build_func = _create_async_build if async_build else _create_build
+    return build_func(
         session, project_id, build_spec, deploy, allow_dangerous_empty_build
     )
 
 
 def create_build_from_local_files(
     session: Session,
     project_id: str,
     path: str,
     deploy: bool,
     targets: Optional[set],
     allow_dangerous_empty_build: bool = False,
     dbt_manifest_path: Optional[PurePath] = None,
+    async_build=False,
 ):
     """Creates a build using local files and returns the result."""
     build_spec = build_spec_from_local(path, project_id, targets, dbt_manifest_path)
-    return _create_build(
+
+    build_func = _create_async_build if async_build else _create_build
+    return build_func(
         session, project_id, build_spec, deploy, allow_dangerous_empty_build
     )
 
 
 def get_datasources(s: Session, project_id: str) -> dict:
     """Queries and formats datasources"""
     query = _get_data_connections(s, project_id)
@@ -138,26 +144,106 @@
     )["data"]["pullResource"]
     res["configs"] = [
         Resource.from_dict(json.loads(string)) for string in res["configs"]
     ]
     return res
 
 
+def fetch_build_status(s: Session, build_id):
+    return _graphql_query(
+        s,
+        """
+        query fetchBuild($buildId: String!){
+            fetchBuild (buildId: $buildId){
+                id,
+                status, 
+            }
+        }
+        """,
+        {"buildId": build_id},
+    )
+
+
+def fetch_build(s: Session, build_id):
+    return _graphql_query(
+        s,
+        """
+        query fetchBuild($buildId: String!){
+            fetchBuild (buildId: $buildId){
+                id,
+                status, 
+                changeSet {
+                    id
+                    resourceChanges
+                    errors
+                    warnings
+                },
+                warnings,
+                errors
+            }
+        }
+        """,
+        {"buildId": build_id},
+    )
+
+
+def apply_preview_build(s: Session, preview_build_id):
+    return _graphql_query(
+        s,
+        """
+        mutation applyPreviewBuild($previewBuildId: String!){
+            applyPreviewBuild (previewBuildId: $previewBuildId){
+                id,
+                status, 
+                changeSet {
+                    id
+                    resourceChanges
+                    errors
+                    warnings
+                },
+                warnings,
+                errors
+            }
+        }
+        """,
+        {"previewBuildId": preview_build_id},
+    )
+
+
 def _parse_table_data(table_data: dict) -> Dict[str, Dict[str, str]]:
     """Formats table names for output, and returns tables names and schemas"""
     tables = table_data["data"]["getAvailableGleanDbTables"]
     tables_by_name = {}
     for table in tables:
         name = (
             table["schema"] + "." + table["name"] if table["schema"] else table["name"]
         )
         tables_by_name[name] = {"schema": table["schema"], "name": table["name"]}
     return tables_by_name
 
 
+def _create_async_build(
+    session, project_id, build_spec, deploy, allow_dangerous_empty_build=False
+):
+    return _graphql_query(
+        session,
+        """
+        mutation CreateAsyncBuild($projectId: String!, $buildSpec: BuildSpecInput!, $deploy: Boolean!, $allowEmptyBuild: Boolean) {
+            createAsyncBuild( projectId: $projectId, buildSpec: $buildSpec, deploy: $deploy, allowEmptyBuild: $allowEmptyBuild)
+        }
+        """,
+        {
+            "projectId": project_id,
+            "buildSpec": build_spec,
+            "deploy": deploy,
+            "allowEmptyBuild": allow_dangerous_empty_build,
+        },
+    )
+
+
 def _create_build(
     session, project_id, build_spec, deploy, allow_dangerous_empty_build=False
 ):
     return _graphql_query(
         session,
         """
         mutation CreateBuild($projectId: String!, $buildSpec: BuildSpecInput!, $deploy: Boolean!, $allowEmptyBuild: Boolean) {
@@ -174,15 +260,15 @@
             }
         }
         """,
         {
             "projectId": project_id,
             "buildSpec": build_spec,
             "deploy": deploy,
-            "allowEmptyBuild": allow_dangerous_empty_build,
+            "allowEmptyBuild": allow_dangerous_empty_build
         },
     )
 
 
 def _get_data_connections(session: Session, project_id: str) -> dict:
     query = _graphql_query(
         session,
```

### Comparing `hashboard-cli-1.0.7/src/hashboard/api/access_keys/browser_auth.py` & `hashboard_cli-1.0.8/src/hashboard/api/access_keys/browser_auth.py`

 * *Files identical despite different names*

### Comparing `hashboard-cli-1.0.7/src/hashboard/api/access_keys/existing_user.py` & `hashboard_cli-1.0.8/src/hashboard/api/access_keys/existing_user.py`

 * *Files identical despite different names*

### Comparing `hashboard-cli-1.0.7/src/hashboard/api/access_keys/utils.py` & `hashboard_cli-1.0.8/src/hashboard/api/access_keys/utils.py`

 * *Files identical despite different names*

### Comparing `hashboard-cli-1.0.7/src/hashboard/api/analytics/__init__.py` & `hashboard_cli-1.0.8/src/hashboard/api/analytics/__init__.py`

 * *Files identical despite different names*

### Comparing `hashboard-cli-1.0.7/src/hashboard/api/analytics/cli_with_tracking.py` & `hashboard_cli-1.0.8/src/hashboard/api/analytics/cli_with_tracking.py`

 * *Files identical despite different names*

### Comparing `hashboard-cli-1.0.7/src/hashboard/cli.py` & `hashboard_cli-1.0.8/src/hashboard/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from contextlib import suppress
 from itertools import count
 import logging
 import os
 import sys
 from pathlib import Path, PurePath, PurePosixPath
+import time
 from requests import Session
 import string
 import subprocess
 from typing import Optional, List
 from uuid import UUID, uuid3
 
 import click
@@ -16,36 +17,34 @@
 
 from hashboard.api.analytics import track
 from hashboard.api.analytics.cli_with_tracking import (
     CommandWithTracking,
     GroupWithTracking,
     set_raw_command,
 )
-from hashboard.api.analytics.events import (
-    ENTER_FULL_NAME_FOR_SIGNUP,
-    ENTER_PROJECT_NAME_FOR_SIGNUP,
-)
 from hashboard.utils.env import env_with_fallback
 from hashboard.utils.input_validation import prompt_and_validate_value_length
 
 from hashboard import VERSION
 from hashboard.api import (
+    apply_preview_build,
     build_details_uri,
     clear_model_cache,
     create_build_from_git_revision,
     create_build_from_local_files,
+    fetch_build,
+    fetch_build_status,
     upload_files_to_hashboard,
     login,
     get_datasources,
     get_tables,
     pull_resource,
 )
 from hashboard.api.access_keys.existing_user import create_access_key
-from hashboard.api.access_keys.new_user import create_account_and_access_key
-from hashboard.constants import DEFAULT_CREDENTIALS_FILEPATH, HASHBOARD_DEBUG
+from hashboard.constants import DEFAULT_CREDENTIALS_FILEPATH, HASHBOARD_BASE_URI, HASHBOARD_DEBUG
 from hashboard.credentials import get_credentials
 from hashboard.filesystem import local_resources
 from hashboard.utils.cli import cli_error_boundary, getenv_bool
 from hashboard.utils.grn import GRN_TYPE_KEY_MODEL, GRNComponents, parse_grn
 from hashboard.utils.resource import Resource
 
 
@@ -126,15 +125,15 @@
 @click.option(
     "--credentials-filepath",
     type=str,
     help="Path to your Hashboard access key credentials. You can also control this by setting a HASHBOARD_CREDENTIALS_FILEPATH environment variable.",
 )
 @click.pass_context
 def cli(ctx: click.Context, credentials_filepath: str):
-    """A command-line interface for interacting with Glean."""
+    """A command-line interface for interacting with Hashboard."""
     if HASHBOARD_DEBUG or HASHBOARD_VERBOSE_DEBUG_UNSAFE:
         _enable_http_logging()
     ctx.ensure_object(dict)
     if credentials_filepath is None:
         credentials_filepath = env_with_fallback(
             "HASHBOARD_CREDENTIALS_FILEPATH",
             "GLEAN_CREDENTIALS_FILEPATH",
@@ -142,29 +141,17 @@
         )
     ctx.obj["credentials_filepath"] = os.path.expanduser(credentials_filepath)
 
 
 @cli.command(cls=CommandWithTracking)
 @click.pass_context
 def signup(ctx: click.Context):
-    """Sign up for a Hashboard account and create an access key to get started.
-
-    If `--credentials-filepath` is passed, will save the access key in that location.
-    """
-    user_full_name = prompt_and_validate_value_length(
-        "Enter your full name", "Full name"
-    )
-    track(ENTER_FULL_NAME_FOR_SIGNUP, {"user_full_name": user_full_name})
-    project_name = prompt_and_validate_value_length(
-        "Enter a name for your Hashboard project", "Hashboard project name"
-    )
-    track(ENTER_PROJECT_NAME_FOR_SIGNUP, {"project_name": project_name})
-    create_account_and_access_key(
-        ctx.obj["credentials_filepath"], user_full_name, project_name
-    )
+    """Sign up for a new Hashboard account."""
+    click.echo(f"👋 Welcome! Follow this link to get started with Hashboard and create a new project: {HASHBOARD_BASE_URI}/getAccess")
+    click.echo("After creating your project, we recommend you to run `hb token` to create an access key.")
 
 
 @cli.command(cls=CommandWithTracking)
 @click.option(
     "--project-id",
     type=str,
     required=False,
@@ -314,14 +301,153 @@
         allow_dangerous_empty_build=allow_dangerous_empty_build,
     )
     _echo_build_results(build_results, True)
     click.echo("")
     click.echo(click.style("✅ Deploy complete.", fg="bright_green"))
 
 
+@cli.command(
+    "preview-async",
+    cls=CommandWithTracking,
+    context_settings=dict(
+        ignore_unknown_options=True,
+    ),
+    hidden=True,
+)
+@git_revision_option
+@git_path_option
+@dbt_manifest_option
+@local_path_argument
+@run_dbt_parse_option
+@dbt_parse_flags_argument
+@allow_dangerous_empty_build_option
+@click.pass_context
+def preview_async(
+    ctx,
+    git_revision,
+    git_path,
+    dbt_manifest_path,
+    filepath,
+    run_dbt_parse,
+    dbt_flags,
+    allow_dangerous_empty_build,
+):
+    """Validates resource configurations and generates a preview link."""
+    ctx.obj["credentials"] = get_credentials(ctx.obj["credentials_filepath"])
+    dbt_manifest_path = _handle_dbt_args(dbt_manifest_path, run_dbt_parse, dbt_flags)
+
+    click.echo("🏗️  Creating preview build...")
+    build_results = _create_build_using_options(
+        ctx,
+        filepath,
+        git_revision=git_revision,
+        git_path=git_path,
+        deploy=False,
+        dbt_manifest_path=dbt_manifest_path,
+        allow_dangerous_empty_build=allow_dangerous_empty_build,
+        async_build=True,
+    )
+    _echo_async_build_creation(build_results, False)
+
+    build_id = build_results["data"]["createAsyncBuild"]
+    build_results = _poll_for_build_status(build_id)
+
+    _echo_async_build_results(build_results)
+
+
+# TODO: Update to follow a build -> apply pattern
+@cli.command("deploy-async", cls=CommandWithTracking, hidden=True)
+@allow_dangerous_empty_build_option
+@git_revision_option
+@git_path_option
+@dbt_manifest_option
+@run_dbt_parse_option
+@local_path_argument
+@dbt_parse_flags_argument
+@click.option(
+    "--preview / --no-preview",
+    default=True,
+    help="Whether to generate a Preview Build before deploying.",
+)
+@click.pass_context
+def deploy_async(
+    ctx: click.Context,
+    git_revision: Optional[str],
+    git_path: Optional[str],
+    dbt_manifest_path: Optional[PurePath],
+    run_dbt_parse: bool,
+    filepath: str,
+    preview: bool,
+    dbt_flags,
+    allow_dangerous_empty_build: bool,
+):
+    """Validates and deploys resource configurations to your project."""
+    ctx.obj["credentials"] = get_credentials(ctx.obj["credentials_filepath"])
+    dbt_manifest_path = _handle_dbt_args(dbt_manifest_path, run_dbt_parse, dbt_flags)
+
+    if not preview:
+        click.echo("🚀 Creating deploy build...")
+        build_results = _create_build_using_options(
+            ctx,
+            filepath,
+            git_revision=git_revision,
+            git_path=git_path,
+            deploy=True,
+            dbt_manifest_path=dbt_manifest_path,
+            allow_dangerous_empty_build=allow_dangerous_empty_build,
+            async_build=True,
+        )
+        _echo_async_build_creation(build_results, True)
+        build_id = build_results["data"]["createAsyncBuild"]
+        build_results = _poll_for_build_status(build_id)
+        _echo_async_build_results(build_results)
+    else:
+        click.echo("🏗️  Creating preview build...")
+        build_results = _create_build_using_options(
+            ctx,
+            filepath,
+            git_revision=git_revision,
+            git_path=git_path,
+            deploy=False,
+            dbt_manifest_path=dbt_manifest_path,
+            allow_dangerous_empty_build=allow_dangerous_empty_build,
+            async_build=True,
+        )
+        _echo_async_build_creation(build_results, False)
+        build_id = build_results["data"]["createAsyncBuild"]
+        build_results = _poll_for_build_status(build_id)
+        _echo_async_build_results(build_results)
+        if not click.confirm("Continue with deploy?"):
+            ctx.exit(1)
+        deploy_build = _deploy_preview_build(build_id)
+        deploy_build_results = deploy_build["data"]["applyPreviewBuild"]
+        _echo_async_build_results(deploy_build_results, deploy=True)
+
+    click.echo("")
+    click.echo(click.style("✅ Deploy complete.", fg="bright_green"))
+
+
+def _poll_for_build_status(build_id):
+    s = get_current_session()
+    click.echo("Compiling resources ", nl=False)
+    for i in range(300):  # arbitrary upper limit
+        click.echo(".", nl=False)
+        # TODO Add error handling here
+        partial_build = fetch_build_status(s, build_id)
+        if ("errors" in partial_build and partial_build["errors"]) or partial_build[
+            "data"
+        ]["fetchBuild"]["status"] == "completed":
+            click.echo()
+            build = fetch_build(s, build_id)
+            return build
+        time.sleep(10)
+    click.echo("Error fetching build, max attempt.", fg="red")
+    click.get_current_context().exit(1)
+
+
 @cli.command(cls=CommandWithTracking)
 @click.pass_context
 def databases(ctx):
     """See your available database connections.
 
     A database connection can be added in the Settings tab on hashboard.com."""
     ctx.obj["credentials"] = get_credentials(ctx.obj["credentials_filepath"])
@@ -647,39 +773,47 @@
     filepath: str,
     dbt_manifest_path: Optional[PurePath] = None,
     git_revision: Optional[str] = None,
     git_path: Optional[str] = None,
     deploy: bool = False,
     targets: Optional[set] = None,
     allow_dangerous_empty_build: bool = False,
+    async_build=False,
 ):
     s = get_current_session()
     project_id = login(s, ctx.obj["credentials"])
     if git_revision:
         return create_build_from_git_revision(
             s,
             project_id,
             git_revision,
             git_path,
             deploy,
             allow_dangerous_empty_build=allow_dangerous_empty_build,
             dbt_manifest_path=dbt_manifest_path,
+            async_build=async_build,
         )
     else:
         return create_build_from_local_files(
             s,
             project_id,
             filepath,
             deploy,
             targets,
             allow_dangerous_empty_build=allow_dangerous_empty_build,
             dbt_manifest_path=dbt_manifest_path,
+            async_build=async_build,
         )
 
 
+def _deploy_preview_build(preview_build_id: str):
+    s = get_current_session()
+    return apply_preview_build(s, preview_build_id)
+
+
 def _echo_tables(table_names: list, datasource: str) -> None:
     click.secho(f"📂 Available Tables From {datasource}", fg="bright_green")
     _echo_list(table_names)
 
 
 def _echo_table_not_found(table: str, tables: dict, datasource: str) -> None:
     """If table is not found in the available tables, output warning and display available tables."""
@@ -704,14 +838,115 @@
     click.echo("")
     click.echo(
         "You can add another database connection in your Settings tab on hashboard.com."
     )
     click.echo("")
 
 
+def _echo_async_build_creation(
+    build_results: dict, deploy: bool, query_name="createAsyncBuild"
+):
+    """Outputs user-friendly build results."""
+    if "errors" in build_results and build_results["errors"]:
+        _echo_build_errors_and_exit(
+            [
+                e["extensions"]["userMessage"]
+                for e in build_results["errors"]
+                if "extensions" in e and "userMessage" in e["extensions"]
+            ]
+        )
+    created_build_results = build_results["data"][query_name]
+
+    click.echo(
+        click.style("📦 Build ", fg="bright_green")
+        + click.style(created_build_results, bold=True)
+        + click.style(" started running successfully.", fg="bright_green")
+    )
+    click.echo("")
+
+
+def _get_empty_status_groups():
+    return {
+        "modelBundles": [],
+        "metrics": [],
+        "savedViews": [],
+        "dashboards": [],
+        "colorPalettes": [],
+        "homepageLaunchpads": [],
+    }
+
+
+def _convert_to_resource_update_list(resource_changes: dict):
+    result = {
+        "added": _get_empty_status_groups(),
+        "changed": _get_empty_status_groups(),
+        "deleted": _get_empty_status_groups(),
+        "unchanged": _get_empty_status_groups(),
+    }
+    action_to_status = {
+        "create": "added",
+        "update": "changed",
+        "delete": "deleted",
+        "unchanged": "unchanged",
+    }
+    type_to_status_group = {
+        "modelBundle": "modelBundles",
+        "savedView": "savedViews",
+        "dashboard-v2": "dashboards",
+        "projectMetric": "metrics",
+        "colorPalette": "colorPalettes",
+        "homepageLaunchpad": "homepageLaunchpads",
+    }
+    for rc in resource_changes.values():
+        result[action_to_status[rc["action"]]][
+            type_to_status_group[rc["newContent"]["value"]["type"]]
+        ].append(rc["newContent"]["value"])
+
+    return result
+
+
+def _echo_async_build_results(
+    build_results: dict, deploy=False, query_name="fetchBuild"
+):
+    """Outputs user-friendly build results."""
+    if "errors" in build_results and build_results["errors"]:
+        _echo_build_errors_and_exit(
+            [
+                e["extensions"]["userMessage"]
+                for e in build_results["errors"]
+                if "extensions" in e and "userMessage" in e["extensions"]
+            ]
+        )
+
+    click.echo()
+
+    created_build_results = build_results["data"][query_name]
+
+    if created_build_results["errors"]:
+        _echo_build_errors_and_exit(created_build_results["errors"])
+
+    click.echo(
+        click.style("📦 Build ", fg="bright_green")
+        + click.style(created_build_results["id"], bold=True)
+        + click.style(" completed successfully.", fg="bright_green")
+    )
+
+    click.echo()
+
+    _echo_build_resources(
+        _convert_to_resource_update_list(build_results["changeSet"]["resourceChanges"]),
+        deploy,
+    )
+
+    if created_build_results["warnings"]:
+        _echo_build_warnings(created_build_results["warnings"])
+
+    click.echo("")
+
+
 def _echo_build_results(build_results: dict, deploy: bool, query_name="createBuild"):
     """Outputs user-friendly build results."""
     if "errors" in build_results and build_results["errors"]:
         _echo_build_errors_and_exit(
             [
                 e["extensions"]["userMessage"]
                 for e in build_results["errors"]
```

### Comparing `hashboard-cli-1.0.7/src/hashboard/credentials.py` & `hashboard_cli-1.0.8/src/hashboard/credentials.py`

 * *Files identical despite different names*

### Comparing `hashboard-cli-1.0.7/src/hashboard/filesystem.py` & `hashboard_cli-1.0.8/src/hashboard/filesystem.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 from contextlib import suppress
 import json
 import os
 import pathlib
 from pathlib import Path, PurePath
-from string import Template
-from typing import Any, Callable, Optional, Dict, Union
+from typing import Any, Callable, Optional, Dict, Union, Set
 
 import yaml
 from click import ClickException
 
 from hashboard.utils.resource import Resource
-from hashboard.utils.validate_config import is_valid_glean_config_file
+from hashboard.utils.config import extract_variable_names, is_valid_glean_config_file
 
 
 VALID_FILE_EXTENSIONS = set([".json", ".yml", ".yaml"])
 
 
 def build_spec_from_local(
     path: str,
     project_id: str,
     targets: Optional[set] = None,
     dbt_manifest_path: Optional[PurePath] = None,
 ) -> dict:
     # Maps parent_directory -> filename -> file contents
     inline_files = []
+    env_var_names : Set[str] = set()
     dbt_manifest = None
 
     if dbt_manifest_path:
         try:
             with open(Path(dbt_manifest_path), "r") as f:
                 dbt_manifest = f.read()
         except Exception as e:
@@ -43,36 +43,34 @@
             with open(os.path.join(root, filename), "r") as f:
                 raw_contents = f.read()
 
                 # Check that the file is a valid config file. Otherwise, ignore it.
                 if not is_valid_glean_config_file(filename, raw_contents):
                     continue
 
+                env_var_names |= extract_variable_names(raw_contents)
+
                 # Right now, changing the filepath of a config file changes its generated ID.
                 # So, we set parentDirectory here to mimic the format that the server uses
                 # when pulling from a git repo.
                 path_suffix = f"/{path}" if path else ""
                 parent_directory = root.replace(
                     path, f"/tmp/repos/{project_id}{path_suffix}"
                 )
-                try:
-                    file_contents = Template(raw_contents).substitute(**os.environ)
-                except KeyError as e:
-                    raise ClickException(
-                        f"No value found for environment variable substitution in {filename}: {str(e)}"
-                    )
 
                 inline_files.append(
                     {
                         "parentDirectory": parent_directory,
                         "filename": filename,
-                        "fileContents": file_contents,
+                        "fileContents": raw_contents,
                     }
                 )
-    return {"inlineConfigFiles": inline_files, "dbtManifest": dbt_manifest}
+
+    env_vars = [{"name": name, "value": os.environ[name]} for name in env_var_names if name in os.environ]
+    return {"inlineConfigFiles": inline_files, "dbtManifest": dbt_manifest, "clientEnvVars": env_vars}
 
 
 def local_resources(root: Union[str, os.PathLike]) -> Dict[PurePath, Resource]:
     """
     Recursively searches root for files that represent Hashboard resources.
     """
     root = Path(root)
```

### Comparing `hashboard-cli-1.0.7/src/hashboard/session.py` & `hashboard_cli-1.0.8/src/hashboard/session.py`

 * *Files identical despite different names*

### Comparing `hashboard-cli-1.0.7/src/hashboard/utils/cli.py` & `hashboard_cli-1.0.8/src/hashboard/utils/cli.py`

 * *Files identical despite different names*

### Comparing `hashboard-cli-1.0.7/src/hashboard/utils/grn.py` & `hashboard_cli-1.0.8/src/hashboard/utils/grn.py`

 * *Files identical despite different names*

### Comparing `hashboard-cli-1.0.7/src/hashboard/utils/input_validation.py` & `hashboard_cli-1.0.8/src/hashboard/utils/input_validation.py`

 * *Files identical despite different names*

### Comparing `hashboard-cli-1.0.7/src/hashboard/utils/resource.py` & `hashboard_cli-1.0.8/src/hashboard/utils/resource.py`

 * *Files identical despite different names*

### Comparing `hashboard-cli-1.0.7/src/hashboard_cli.egg-info/SOURCES.txt` & `hashboard_cli-1.0.8/src/hashboard_cli.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -9,26 +9,25 @@
 src/hashboard/credentials.py
 src/hashboard/filesystem.py
 src/hashboard/session.py
 src/hashboard/api/__init__.py
 src/hashboard/api/access_keys/__init__.py
 src/hashboard/api/access_keys/browser_auth.py
 src/hashboard/api/access_keys/existing_user.py
-src/hashboard/api/access_keys/new_user.py
 src/hashboard/api/access_keys/utils.py
 src/hashboard/api/analytics/__init__.py
 src/hashboard/api/analytics/cli_with_tracking.py
 src/hashboard/api/analytics/events.py
 src/hashboard/utils/__init__.py
 src/hashboard/utils/cli.py
+src/hashboard/utils/config.py
 src/hashboard/utils/env.py
 src/hashboard/utils/grn.py
 src/hashboard/utils/input_validation.py
 src/hashboard/utils/resource.py
-src/hashboard/utils/validate_config.py
 src/hashboard_cli.egg-info/PKG-INFO
 src/hashboard_cli.egg-info/SOURCES.txt
 src/hashboard_cli.egg-info/dependency_links.txt
 src/hashboard_cli.egg-info/entry_points.txt
 src/hashboard_cli.egg-info/requires.txt
 src/hashboard_cli.egg-info/top_level.txt
 tests/test_cli.py
```

### Comparing `hashboard-cli-1.0.7/tests/test_credentials.py` & `hashboard_cli-1.0.8/tests/test_credentials.py`

 * *Files identical despite different names*

### Comparing `hashboard-cli-1.0.7/tests/test_filesystem.py` & `hashboard_cli-1.0.8/tests/test_filesystem.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,37 +17,21 @@
     monkeypatch.setenv("A_NAME", "substitution")
 
     PATH = "model_config_files/with_env_vars"
 
     build_spec = build_spec_from_local(get_fixture_path(PATH), "")
     assert len(build_spec["inlineConfigFiles"]) == 1
 
-    config_file_details = build_spec["inlineConfigFiles"][0]
+    env_vars = build_spec["clientEnvVars"]
 
     # check that the file contents have the substituted value for name
     assert (
-        config_file_details["fileContents"]
-        == 'glean: "1.0"\nname: substitution\ngrn: "m:RNuzTq-85qzAFKJ8"\n'
+       env_vars
+        == [{'name': 'A_NAME', 'value': 'substitution'}]
     )
-    assert config_file_details["filename"] == "file1.yml"
-    assert config_file_details["parentDirectory"].startswith("/tmp/repos")
-    assert config_file_details["parentDirectory"].endswith(PATH)
-
-
-def test_environment_variable_missing(clear_env, monkeypatch: pytest.MonkeyPatch):
-    monkeypatch.setenv("SOMETHING_ELSE", "substitution")
-
-    try:
-        build_spec_from_local(get_fixture_path("model_config_files/with_env_vars"), "")
-        assert False, "Expected exception to be thrown"
-    except ClickException as e:
-        assert (
-            str(e)
-            == "No value found for environment variable substitution in file1.yml: 'A_NAME'"
-        )
 
 
 def test_file_validation():
     with pytest.raises(ClickException) as exception_info:
         build_spec_from_local(
             get_fixture_path("model_config_files/with_invalid_files"), ""
         )
```

### Comparing `hashboard-cli-1.0.7/tests/test_hashboard_api.py` & `hashboard_cli-1.0.8/tests/test_hashboard_api.py`

 * *Files identical despite different names*

