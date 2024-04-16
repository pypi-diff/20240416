# Comparing `tmp/google-cloud-alloydb-connector-1.0.0.tar.gz` & `tmp/google-cloud-alloydb-connector-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-alloydb-connector-1.0.0.tar", last modified: Tue Mar 12 16:22:20 2024, max compression
+gzip compressed data, was "google-cloud-alloydb-connector-1.1.0.tar", last modified: Tue Apr 16 15:32:14 2024, max compression
```

## Comparing `google-cloud-alloydb-connector-1.0.0.tar` & `google-cloud-alloydb-connector-1.1.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-12 16:22:20.937046 google-cloud-alloydb-connector-1.0.0/
--rw-rw-r--   0 root         (0)     1003    11357 2024-03-12 16:19:42.000000 google-cloud-alloydb-connector-1.0.0/LICENSE
--rw-r--r--   0 root         (0)     1003    16619 2024-03-12 16:22:20.937046 google-cloud-alloydb-connector-1.0.0/PKG-INFO
--rw-rw-r--   0 root         (0)     1003    15663 2024-03-12 16:19:42.000000 google-cloud-alloydb-connector-1.0.0/README.md
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-12 16:22:20.933046 google-cloud-alloydb-connector-1.0.0/google/
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-12 16:22:20.933046 google-cloud-alloydb-connector-1.0.0/google/api/
--rw-rw-r--   0 root         (0)     1003      574 2024-03-12 16:19:42.000000 google-cloud-alloydb-connector-1.0.0/google/api/__init__.py
--rwxrwxr-x   0 root         (0)     1003     2620 2024-03-12 16:19:42.000000 google-cloud-alloydb-connector-1.0.0/google/api/field_behavior_pb2.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-12 16:22:20.933046 google-cloud-alloydb-connector-1.0.0/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-12 16:22:20.933046 google-cloud-alloydb-connector-1.0.0/google/cloud/alloydb/
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-12 16:22:20.937046 google-cloud-alloydb-connector-1.0.0/google/cloud/alloydb/connector/
--rw-rw-r--   0 root         (0)     1003      903 2024-03-12 16:19:42.000000 google-cloud-alloydb-connector-1.0.0/google/cloud/alloydb/connector/__init__.py
--rw-rw-r--   0 root         (0)     1003     7785 2024-03-12 16:19:42.000000 google-cloud-alloydb-connector-1.0.0/google/cloud/alloydb/connector/async_connector.py
--rw-rw-r--   0 root         (0)     1003     1841 2024-03-12 16:19:42.000000 google-cloud-alloydb-connector-1.0.0/google/cloud/alloydb/connector/asyncpg.py
--rw-rw-r--   0 root         (0)     1003     6728 2024-03-12 16:19:42.000000 google-cloud-alloydb-connector-1.0.0/google/cloud/alloydb/connector/client.py
--rw-rw-r--   0 root         (0)     1003    13812 2024-03-12 16:19:42.000000 google-cloud-alloydb-connector-1.0.0/google/cloud/alloydb/connector/connector.py
--rw-rw-r--   0 root         (0)     1003      665 2024-03-12 16:19:42.000000 google-cloud-alloydb-connector-1.0.0/google/cloud/alloydb/connector/exceptions.py
--rw-rw-r--   0 root         (0)     1003     9783 2024-03-12 16:19:42.000000 google-cloud-alloydb-connector-1.0.0/google/cloud/alloydb/connector/instance.py
--rw-rw-r--   0 root         (0)     1003     1437 2024-03-12 16:19:42.000000 google-cloud-alloydb-connector-1.0.0/google/cloud/alloydb/connector/pg8000.py
--rw-rw-r--   0 root         (0)     1003        0 2024-03-12 16:19:42.000000 google-cloud-alloydb-connector-1.0.0/google/cloud/alloydb/connector/py.typed
--rw-rw-r--   0 root         (0)     1003     2764 2024-03-12 16:19:42.000000 google-cloud-alloydb-connector-1.0.0/google/cloud/alloydb/connector/rate_limiter.py
--rw-rw-r--   0 root         (0)     1003     4384 2024-03-12 16:19:42.000000 google-cloud-alloydb-connector-1.0.0/google/cloud/alloydb/connector/refresh.py
--rw-rw-r--   0 root         (0)     1003     2076 2024-03-12 16:19:42.000000 google-cloud-alloydb-connector-1.0.0/google/cloud/alloydb/connector/utils.py
--rw-rw-r--   0 root         (0)     1003      597 2024-03-12 16:19:42.000000 google-cloud-alloydb-connector-1.0.0/google/cloud/alloydb/connector/version.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-12 16:22:20.933046 google-cloud-alloydb-connector-1.0.0/google/cloud/alloydb_connectors_v1/
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-12 16:22:20.937046 google-cloud-alloydb-connector-1.0.0/google/cloud/alloydb_connectors_v1/proto/
--rw-rw-r--   0 root         (0)     1003      574 2024-03-12 16:19:42.000000 google-cloud-alloydb-connector-1.0.0/google/cloud/alloydb_connectors_v1/proto/__init__.py
--rwxrwxr-x   0 root         (0)     1003     3962 2024-03-12 16:19:42.000000 google-cloud-alloydb-connector-1.0.0/google/cloud/alloydb_connectors_v1/proto/resources_pb2.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-12 16:22:20.937046 google-cloud-alloydb-connector-1.0.0/google_cloud_alloydb_connector.egg-info/
--rw-r--r--   0 root         (0)     1003    16619 2024-03-12 16:22:20.000000 google-cloud-alloydb-connector-1.0.0/google_cloud_alloydb_connector.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     1085 2024-03-12 16:22:20.000000 google-cloud-alloydb-connector-1.0.0/google_cloud_alloydb_connector.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2024-03-12 16:22:20.000000 google-cloud-alloydb-connector-1.0.0/google_cloud_alloydb_connector.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003        1 2024-03-12 16:22:20.000000 google-cloud-alloydb-connector-1.0.0/google_cloud_alloydb_connector.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      111 2024-03-12 16:22:20.000000 google-cloud-alloydb-connector-1.0.0/google_cloud_alloydb_connector.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2024-03-12 16:22:20.000000 google-cloud-alloydb-connector-1.0.0/google_cloud_alloydb_connector.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2024-03-12 16:22:20.941045 google-cloud-alloydb-connector-1.0.0/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2673 2024-03-12 16:19:42.000000 google-cloud-alloydb-connector-1.0.0/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 15:32:14.562714 google-cloud-alloydb-connector-1.1.0/
+-rw-rw-r--   0 root         (0)     1003    11357 2024-04-16 15:29:39.000000 google-cloud-alloydb-connector-1.1.0/LICENSE
+-rw-r--r--   0 root         (0)     1003    16779 2024-04-16 15:32:14.562714 google-cloud-alloydb-connector-1.1.0/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003    15823 2024-04-16 15:29:39.000000 google-cloud-alloydb-connector-1.1.0/README.md
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 15:32:14.558714 google-cloud-alloydb-connector-1.1.0/google/
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 15:32:14.558714 google-cloud-alloydb-connector-1.1.0/google/api/
+-rw-rw-r--   0 root         (0)     1003      574 2024-04-16 15:29:39.000000 google-cloud-alloydb-connector-1.1.0/google/api/__init__.py
+-rwxrwxr-x   0 root         (0)     1003     2620 2024-04-16 15:29:39.000000 google-cloud-alloydb-connector-1.1.0/google/api/field_behavior_pb2.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 15:32:14.558714 google-cloud-alloydb-connector-1.1.0/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 15:32:14.558714 google-cloud-alloydb-connector-1.1.0/google/cloud/alloydb/
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 15:32:14.562714 google-cloud-alloydb-connector-1.1.0/google/cloud/alloydb/connector/
+-rw-rw-r--   0 root         (0)     1003      903 2024-04-16 15:29:39.000000 google-cloud-alloydb-connector-1.1.0/google/cloud/alloydb/connector/__init__.py
+-rw-rw-r--   0 root         (0)     1003     7785 2024-04-16 15:29:39.000000 google-cloud-alloydb-connector-1.1.0/google/cloud/alloydb/connector/async_connector.py
+-rw-rw-r--   0 root         (0)     1003     1841 2024-04-16 15:29:39.000000 google-cloud-alloydb-connector-1.1.0/google/cloud/alloydb/connector/asyncpg.py
+-rw-rw-r--   0 root         (0)     1003     6956 2024-04-16 15:29:39.000000 google-cloud-alloydb-connector-1.1.0/google/cloud/alloydb/connector/client.py
+-rw-rw-r--   0 root         (0)     1003    13812 2024-04-16 15:29:39.000000 google-cloud-alloydb-connector-1.1.0/google/cloud/alloydb/connector/connector.py
+-rw-rw-r--   0 root         (0)     1003      665 2024-04-16 15:29:39.000000 google-cloud-alloydb-connector-1.1.0/google/cloud/alloydb/connector/exceptions.py
+-rw-rw-r--   0 root         (0)     1003     9804 2024-04-16 15:29:39.000000 google-cloud-alloydb-connector-1.1.0/google/cloud/alloydb/connector/instance.py
+-rw-rw-r--   0 root         (0)     1003     1437 2024-04-16 15:29:39.000000 google-cloud-alloydb-connector-1.1.0/google/cloud/alloydb/connector/pg8000.py
+-rw-rw-r--   0 root         (0)     1003        0 2024-04-16 15:29:39.000000 google-cloud-alloydb-connector-1.1.0/google/cloud/alloydb/connector/py.typed
+-rw-rw-r--   0 root         (0)     1003     2764 2024-04-16 15:29:39.000000 google-cloud-alloydb-connector-1.1.0/google/cloud/alloydb/connector/rate_limiter.py
+-rw-rw-r--   0 root         (0)     1003     4482 2024-04-16 15:29:39.000000 google-cloud-alloydb-connector-1.1.0/google/cloud/alloydb/connector/refresh.py
+-rw-rw-r--   0 root         (0)     1003     2076 2024-04-16 15:29:39.000000 google-cloud-alloydb-connector-1.1.0/google/cloud/alloydb/connector/utils.py
+-rw-rw-r--   0 root         (0)     1003      597 2024-04-16 15:29:39.000000 google-cloud-alloydb-connector-1.1.0/google/cloud/alloydb/connector/version.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 15:32:14.558714 google-cloud-alloydb-connector-1.1.0/google/cloud/alloydb_connectors_v1/
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 15:32:14.562714 google-cloud-alloydb-connector-1.1.0/google/cloud/alloydb_connectors_v1/proto/
+-rw-rw-r--   0 root         (0)     1003      574 2024-04-16 15:29:39.000000 google-cloud-alloydb-connector-1.1.0/google/cloud/alloydb_connectors_v1/proto/__init__.py
+-rwxrwxr-x   0 root         (0)     1003     3962 2024-04-16 15:29:39.000000 google-cloud-alloydb-connector-1.1.0/google/cloud/alloydb_connectors_v1/proto/resources_pb2.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 15:32:14.562714 google-cloud-alloydb-connector-1.1.0/google_cloud_alloydb_connector.egg-info/
+-rw-r--r--   0 root         (0)     1003    16779 2024-04-16 15:32:14.000000 google-cloud-alloydb-connector-1.1.0/google_cloud_alloydb_connector.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     1085 2024-04-16 15:32:14.000000 google-cloud-alloydb-connector-1.1.0/google_cloud_alloydb_connector.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2024-04-16 15:32:14.000000 google-cloud-alloydb-connector-1.1.0/google_cloud_alloydb_connector.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003        1 2024-04-16 15:32:14.000000 google-cloud-alloydb-connector-1.1.0/google_cloud_alloydb_connector.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      111 2024-04-16 15:32:14.000000 google-cloud-alloydb-connector-1.1.0/google_cloud_alloydb_connector.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2024-04-16 15:32:14.000000 google-cloud-alloydb-connector-1.1.0/google_cloud_alloydb_connector.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2024-04-16 15:32:14.566715 google-cloud-alloydb-connector-1.1.0/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2673 2024-04-16 15:29:39.000000 google-cloud-alloydb-connector-1.1.0/setup.py
```

### Comparing `google-cloud-alloydb-connector-1.0.0/LICENSE` & `google-cloud-alloydb-connector-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-alloydb-connector-1.0.0/PKG-INFO` & `google-cloud-alloydb-connector-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-alloydb-connector
-Version: 1.0.0
+Version: 1.1.0
 Summary: A Python client library for connecting securely to your Google Cloud AlloyDB instances.
 Home-page: https://github.com/GoogleCloudPlatform/alloydb-python-connector
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
@@ -115,23 +115,25 @@
 ## Usage
 
 This package provides several functions for authorizing and encrypting
 connections. These functions are used with your database driver to connect to
 your AlloyDB instance.
 
 AlloyDB supports network connectivity through public IP addresses and private,
-internal IP addresses. By default this package will attempt to connect over a
+internal IP addresses, as well as [Private Service Connect][psc] (PSC). 
+By default this package will attempt to connect over a
 private IP connection. When doing so, this package must be run in an
 environment that is connected to the [VPC Network][vpc] that hosts your
 AlloyDB private IP address.
 
 Please see [Configuring AlloyDB Connectivity][alloydb-connectivity] for more details.
 
 [vpc]: https://cloud.google.com/vpc/docs/vpc
 [alloydb-connectivity]: https://cloud.google.com/alloydb/docs/configure-connectivity
+[psc]: https://cloud.google.com/vpc/docs/private-service-connect
 
 ### Synchronous Driver Usage
 
 To connect to AlloyDB using the connector, inititalize a `Connector`
 object and call it's `connect` method with the proper input parameters.
 
 The `Connector` itself creates database connection objects by calling its `connect` method
@@ -404,18 +406,21 @@
 [configure-iam-authn]: https://cloud.google.com/alloydb/docs/manage-iam-authn#enable
 [add-iam-user]: https://cloud.google.com/alloydb/docs/manage-iam-authn#create-user
 
 ### Specifying IP Address Type
 
 The AlloyDB Python Connector by default will attempt to establish connections
 to your instance's private IP. To change this, such as connecting to AlloyDB
-over a public IP address, set the `ip_type` keyword argument when initializing
-a `Connector()` or when calling `connector.connect()`.
+over a public IP address or Private Service Connect (PSC), set the `ip_type`
+keyword argument when initializing a `Connector()` or when calling 
+`connector.connect()`.
+
+Possible values for `ip_type` are `"PRIVATE"` (default value), `"PUBLIC"`, 
+and `"PSC"`.
 
-Possible values for `ip_type` are `"PRIVATE"` (default value), and `"PUBLIC"`.
 Example:
 
 ```python
 from google.cloud.alloydb.connector import Connector
 
 import sqlalchemy
```

### Comparing `google-cloud-alloydb-connector-1.0.0/README.md` & `google-cloud-alloydb-connector-1.1.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -91,23 +91,25 @@
 ## Usage
 
 This package provides several functions for authorizing and encrypting
 connections. These functions are used with your database driver to connect to
 your AlloyDB instance.
 
 AlloyDB supports network connectivity through public IP addresses and private,
-internal IP addresses. By default this package will attempt to connect over a
+internal IP addresses, as well as [Private Service Connect][psc] (PSC). 
+By default this package will attempt to connect over a
 private IP connection. When doing so, this package must be run in an
 environment that is connected to the [VPC Network][vpc] that hosts your
 AlloyDB private IP address.
 
 Please see [Configuring AlloyDB Connectivity][alloydb-connectivity] for more details.
 
 [vpc]: https://cloud.google.com/vpc/docs/vpc
 [alloydb-connectivity]: https://cloud.google.com/alloydb/docs/configure-connectivity
+[psc]: https://cloud.google.com/vpc/docs/private-service-connect
 
 ### Synchronous Driver Usage
 
 To connect to AlloyDB using the connector, inititalize a `Connector`
 object and call it's `connect` method with the proper input parameters.
 
 The `Connector` itself creates database connection objects by calling its `connect` method
@@ -380,18 +382,21 @@
 [configure-iam-authn]: https://cloud.google.com/alloydb/docs/manage-iam-authn#enable
 [add-iam-user]: https://cloud.google.com/alloydb/docs/manage-iam-authn#create-user
 
 ### Specifying IP Address Type
 
 The AlloyDB Python Connector by default will attempt to establish connections
 to your instance's private IP. To change this, such as connecting to AlloyDB
-over a public IP address, set the `ip_type` keyword argument when initializing
-a `Connector()` or when calling `connector.connect()`.
+over a public IP address or Private Service Connect (PSC), set the `ip_type`
+keyword argument when initializing a `Connector()` or when calling 
+`connector.connect()`.
+
+Possible values for `ip_type` are `"PRIVATE"` (default value), `"PUBLIC"`, 
+and `"PSC"`.
 
-Possible values for `ip_type` are `"PRIVATE"` (default value), and `"PUBLIC"`.
 Example:
 
 ```python
 from google.cloud.alloydb.connector import Connector
 
 import sqlalchemy
```

### Comparing `google-cloud-alloydb-connector-1.0.0/google/api/__init__.py` & `google-cloud-alloydb-connector-1.1.0/google/api/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-alloydb-connector-1.0.0/google/api/field_behavior_pb2.py` & `google-cloud-alloydb-connector-1.1.0/google/api/field_behavior_pb2.py`

 * *Files identical despite different names*

### Comparing `google-cloud-alloydb-connector-1.0.0/google/cloud/alloydb/connector/__init__.py` & `google-cloud-alloydb-connector-1.1.0/google/cloud/alloydb/connector/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-alloydb-connector-1.0.0/google/cloud/alloydb/connector/async_connector.py` & `google-cloud-alloydb-connector-1.1.0/google/cloud/alloydb/connector/async_connector.py`

 * *Files identical despite different names*

### Comparing `google-cloud-alloydb-connector-1.0.0/google/cloud/alloydb/connector/asyncpg.py` & `google-cloud-alloydb-connector-1.1.0/google/cloud/alloydb/connector/asyncpg.py`

 * *Files identical despite different names*

### Comparing `google-cloud-alloydb-connector-1.0.0/google/cloud/alloydb/connector/client.py` & `google-cloud-alloydb-connector-1.1.0/google/cloud/alloydb/connector/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     driver: Optional[str],
     custom_user_agent: Optional[str],
 ) -> str:
     """
     Appends user-defined user agents to the base default agent.
     """
     agent = f"{USER_AGENT}+{driver}" if driver else USER_AGENT
-    if custom_user_agent:
+    if custom_user_agent and isinstance(custom_user_agent, str):
         agent = f"{agent} {custom_user_agent}"
 
     return agent
 
 
 class AlloyDBClient:
     def __init__(
@@ -125,17 +125,23 @@
         }
 
         url = f"{self._alloydb_api_endpoint}/{API_VERSION}/projects/{project}/locations/{region}/clusters/{cluster}/instances/{name}/connectionInfo"
 
         resp = await self._client.get(url, headers=headers, raise_for_status=True)
         resp_dict = await resp.json()
 
+        # Remove trailing period from PSC DNS name.
+        psc_dns = resp_dict.get("pscDnsName")
+        if psc_dns:
+            psc_dns = psc_dns.rstrip(".")
+
         return {
             "PRIVATE": resp_dict.get("ipAddress"),
             "PUBLIC": resp_dict.get("publicIpAddress"),
+            "PSC": psc_dns,
         }
 
     async def _get_client_certificate(
         self,
         project: str,
         region: str,
         cluster: str,
```

### Comparing `google-cloud-alloydb-connector-1.0.0/google/cloud/alloydb/connector/connector.py` & `google-cloud-alloydb-connector-1.1.0/google/cloud/alloydb/connector/connector.py`

 * *Files identical despite different names*

### Comparing `google-cloud-alloydb-connector-1.0.0/google/cloud/alloydb/connector/exceptions.py` & `google-cloud-alloydb-connector-1.1.0/google/cloud/alloydb/connector/exceptions.py`

 * *Files identical despite different names*

### Comparing `google-cloud-alloydb-connector-1.0.0/google/cloud/alloydb/connector/instance.py` & `google-cloud-alloydb-connector-1.1.0/google/cloud/alloydb/connector/instance.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,14 +44,15 @@
 class IPTypes(Enum):
     """
     Enum for specifying IP type to connect to AlloyDB with.
     """
 
     PUBLIC: str = "PUBLIC"
     PRIVATE: str = "PRIVATE"
+    PSC: str = "PSC"
 
     @classmethod
     def _missing_(cls, value: object) -> None:
         raise ValueError(
             f"Incorrect value for ip_type, got '{value}'. Want one of: "
             f"{', '.join([repr(m.value) for m in cls])}."
         )
```

### Comparing `google-cloud-alloydb-connector-1.0.0/google/cloud/alloydb/connector/pg8000.py` & `google-cloud-alloydb-connector-1.1.0/google/cloud/alloydb/connector/pg8000.py`

 * *Files identical despite different names*

### Comparing `google-cloud-alloydb-connector-1.0.0/google/cloud/alloydb/connector/rate_limiter.py` & `google-cloud-alloydb-connector-1.1.0/google/cloud/alloydb/connector/rate_limiter.py`

 * *Files identical despite different names*

### Comparing `google-cloud-alloydb-connector-1.0.0/google/cloud/alloydb/connector/refresh.py` & `google-cloud-alloydb-connector-1.1.0/google/cloud/alloydb/connector/refresh.py`

 * *Files 4% similar despite different names*

```diff
@@ -82,15 +82,16 @@
         ip_addrs: Dict[str, Optional[str]],
         key: rsa.RSAPrivateKey,
         certs: Tuple[str, List[str]],
     ) -> None:
         self.ip_addrs = ip_addrs
         # create TLS context
         self.context = ssl.SSLContext(ssl.PROTOCOL_TLS_CLIENT)
-        # update ssl.PROTOCOL_TLS_CLIENT default
+        # TODO: Set check_hostname to True to verify the identity in the
+        # certificate once PSC DNS is populated in all existing clusters.
         self.context.check_hostname = False
         # force TLSv1.3
         self.context.minimum_version = ssl.TLSVersion.TLSv1_3
         # add request_ssl attribute to ssl.SSLContext, required for pg8000 driver
         self.context.request_ssl = False  # type: ignore
         # unpack certs
         ca_cert, cert_chain = certs
```

### Comparing `google-cloud-alloydb-connector-1.0.0/google/cloud/alloydb/connector/utils.py` & `google-cloud-alloydb-connector-1.1.0/google/cloud/alloydb/connector/utils.py`

 * *Files identical despite different names*

### Comparing `google-cloud-alloydb-connector-1.0.0/google/cloud/alloydb/connector/version.py` & `google-cloud-alloydb-connector-1.1.0/google/cloud/alloydb/connector/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "1.0.0"
+__version__ = "1.1.0"
```

### Comparing `google-cloud-alloydb-connector-1.0.0/google/cloud/alloydb_connectors_v1/proto/__init__.py` & `google-cloud-alloydb-connector-1.1.0/google/cloud/alloydb_connectors_v1/proto/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-alloydb-connector-1.0.0/google/cloud/alloydb_connectors_v1/proto/resources_pb2.py` & `google-cloud-alloydb-connector-1.1.0/google/cloud/alloydb_connectors_v1/proto/resources_pb2.py`

 * *Files identical despite different names*

### Comparing `google-cloud-alloydb-connector-1.0.0/google_cloud_alloydb_connector.egg-info/PKG-INFO` & `google-cloud-alloydb-connector-1.1.0/google_cloud_alloydb_connector.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-alloydb-connector
-Version: 1.0.0
+Version: 1.1.0
 Summary: A Python client library for connecting securely to your Google Cloud AlloyDB instances.
 Home-page: https://github.com/GoogleCloudPlatform/alloydb-python-connector
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
@@ -115,23 +115,25 @@
 ## Usage
 
 This package provides several functions for authorizing and encrypting
 connections. These functions are used with your database driver to connect to
 your AlloyDB instance.
 
 AlloyDB supports network connectivity through public IP addresses and private,
-internal IP addresses. By default this package will attempt to connect over a
+internal IP addresses, as well as [Private Service Connect][psc] (PSC). 
+By default this package will attempt to connect over a
 private IP connection. When doing so, this package must be run in an
 environment that is connected to the [VPC Network][vpc] that hosts your
 AlloyDB private IP address.
 
 Please see [Configuring AlloyDB Connectivity][alloydb-connectivity] for more details.
 
 [vpc]: https://cloud.google.com/vpc/docs/vpc
 [alloydb-connectivity]: https://cloud.google.com/alloydb/docs/configure-connectivity
+[psc]: https://cloud.google.com/vpc/docs/private-service-connect
 
 ### Synchronous Driver Usage
 
 To connect to AlloyDB using the connector, inititalize a `Connector`
 object and call it's `connect` method with the proper input parameters.
 
 The `Connector` itself creates database connection objects by calling its `connect` method
@@ -404,18 +406,21 @@
 [configure-iam-authn]: https://cloud.google.com/alloydb/docs/manage-iam-authn#enable
 [add-iam-user]: https://cloud.google.com/alloydb/docs/manage-iam-authn#create-user
 
 ### Specifying IP Address Type
 
 The AlloyDB Python Connector by default will attempt to establish connections
 to your instance's private IP. To change this, such as connecting to AlloyDB
-over a public IP address, set the `ip_type` keyword argument when initializing
-a `Connector()` or when calling `connector.connect()`.
+over a public IP address or Private Service Connect (PSC), set the `ip_type`
+keyword argument when initializing a `Connector()` or when calling 
+`connector.connect()`.
+
+Possible values for `ip_type` are `"PRIVATE"` (default value), `"PUBLIC"`, 
+and `"PSC"`.
 
-Possible values for `ip_type` are `"PRIVATE"` (default value), and `"PUBLIC"`.
 Example:
 
 ```python
 from google.cloud.alloydb.connector import Connector
 
 import sqlalchemy
```

### Comparing `google-cloud-alloydb-connector-1.0.0/google_cloud_alloydb_connector.egg-info/SOURCES.txt` & `google-cloud-alloydb-connector-1.1.0/google_cloud_alloydb_connector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-alloydb-connector-1.0.0/setup.py` & `google-cloud-alloydb-connector-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
     ],
     platforms="Posix; MacOS X; Windows",
     packages=packages,
     install_requires=dependencies,
     extras_require={
-        "pg8000": ["pg8000>=1.30.5"],
+        "pg8000": ["pg8000>=1.31.1"],
         "asyncpg": ["asyncpg>=0.29.0"],
     },
     python_requires=">=3.8",
     include_package_data=True,
     zip_safe=False,
     package_data={"google.cloud.alloydb.connector": ["py.typed"]},
 )
```

