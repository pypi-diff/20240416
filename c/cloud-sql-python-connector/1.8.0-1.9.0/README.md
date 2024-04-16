# Comparing `tmp/cloud-sql-python-connector-1.8.0.tar.gz` & `tmp/cloud-sql-python-connector-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloud-sql-python-connector-1.8.0.tar", last modified: Tue Mar 12 16:31:29 2024, max compression
+gzip compressed data, was "cloud-sql-python-connector-1.9.0.tar", last modified: Tue Apr 16 15:44:45 2024, max compression
```

## Comparing `cloud-sql-python-connector-1.8.0.tar` & `cloud-sql-python-connector-1.9.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-12 16:31:29.602207 cloud-sql-python-connector-1.8.0/
--rw-rw-r--   0 root         (0)     1003    11358 2024-03-12 16:29:09.000000 cloud-sql-python-connector-1.8.0/LICENSE
--rw-r--r--   0 root         (0)     1003    23771 2024-03-12 16:31:29.602207 cloud-sql-python-connector-1.8.0/PKG-INFO
--rw-rw-r--   0 root         (0)     1003    22623 2024-03-12 16:29:09.000000 cloud-sql-python-connector-1.8.0/README.md
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-12 16:31:29.598207 cloud-sql-python-connector-1.8.0/cloud_sql_python_connector.egg-info/
--rw-r--r--   0 root         (0)     1003    23771 2024-03-12 16:31:29.000000 cloud-sql-python-connector-1.8.0/cloud_sql_python_connector.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003      876 2024-03-12 16:31:29.000000 cloud-sql-python-connector-1.8.0/cloud_sql_python_connector.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2024-03-12 16:31:29.000000 cloud-sql-python-connector-1.8.0/cloud_sql_python_connector.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003        1 2024-03-12 16:31:29.000000 cloud-sql-python-connector-1.8.0/cloud_sql_python_connector.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      156 2024-03-12 16:31:29.000000 cloud-sql-python-connector-1.8.0/cloud_sql_python_connector.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2024-03-12 16:31:29.000000 cloud-sql-python-connector-1.8.0/cloud_sql_python_connector.egg-info/top_level.txt
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-12 16:31:29.594207 cloud-sql-python-connector-1.8.0/google/
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-12 16:31:29.598207 cloud-sql-python-connector-1.8.0/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-12 16:31:29.598207 cloud-sql-python-connector-1.8.0/google/cloud/sql/
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-12 16:31:29.602207 cloud-sql-python-connector-1.8.0/google/cloud/sql/connector/
--rw-rw-r--   0 root         (0)     1003      883 2024-03-12 16:29:09.000000 cloud-sql-python-connector-1.8.0/google/cloud/sql/connector/__init__.py
--rw-rw-r--   0 root         (0)     1003     1838 2024-03-12 16:29:09.000000 cloud-sql-python-connector-1.8.0/google/cloud/sql/connector/asyncpg.py
--rw-rw-r--   0 root         (0)     1003     8263 2024-03-12 16:29:09.000000 cloud-sql-python-connector-1.8.0/google/cloud/sql/connector/client.py
--rwxrwxr-x   0 root         (0)     1003    16867 2024-03-12 16:29:09.000000 cloud-sql-python-connector-1.8.0/google/cloud/sql/connector/connector.py
--rw-rw-r--   0 root         (0)     1003     1524 2024-03-12 16:29:09.000000 cloud-sql-python-connector-1.8.0/google/cloud/sql/connector/exceptions.py
--rw-rw-r--   0 root         (0)     1003    14920 2024-03-12 16:29:09.000000 cloud-sql-python-connector-1.8.0/google/cloud/sql/connector/instance.py
--rw-rw-r--   0 root         (0)     1003     1814 2024-03-12 16:29:09.000000 cloud-sql-python-connector-1.8.0/google/cloud/sql/connector/pg8000.py
--rw-rw-r--   0 root         (0)     1003        0 2024-03-12 16:29:09.000000 cloud-sql-python-connector-1.8.0/google/cloud/sql/connector/py.typed
--rw-rw-r--   0 root         (0)     1003     2105 2024-03-12 16:29:09.000000 cloud-sql-python-connector-1.8.0/google/cloud/sql/connector/pymysql.py
--rw-rw-r--   0 root         (0)     1003     2452 2024-03-12 16:29:09.000000 cloud-sql-python-connector-1.8.0/google/cloud/sql/connector/pytds.py
--rw-rw-r--   0 root         (0)     1003     2993 2024-03-12 16:29:09.000000 cloud-sql-python-connector-1.8.0/google/cloud/sql/connector/rate_limiter.py
--rw-rw-r--   0 root         (0)     1003     3680 2024-03-12 16:29:09.000000 cloud-sql-python-connector-1.8.0/google/cloud/sql/connector/refresh_utils.py
--rwxrwxr-x   0 root         (0)     1003     3448 2024-03-12 16:29:09.000000 cloud-sql-python-connector-1.8.0/google/cloud/sql/connector/utils.py
--rw-rw-r--   0 root         (0)     1003      597 2024-03-12 16:29:09.000000 cloud-sql-python-connector-1.8.0/google/cloud/sql/connector/version.py
--rw-rw-r--   0 root         (0)     1003       67 2024-03-12 16:31:29.602207 cloud-sql-python-connector-1.8.0/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2897 2024-03-12 16:29:09.000000 cloud-sql-python-connector-1.8.0/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 15:44:45.683349 cloud-sql-python-connector-1.9.0/
+-rw-rw-r--   0 root         (0)     1003    11358 2024-04-16 15:42:12.000000 cloud-sql-python-connector-1.9.0/LICENSE
+-rw-r--r--   0 root         (0)     1003    23771 2024-04-16 15:44:45.683349 cloud-sql-python-connector-1.9.0/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003    22623 2024-04-16 15:42:12.000000 cloud-sql-python-connector-1.9.0/README.md
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 15:44:45.679346 cloud-sql-python-connector-1.9.0/cloud_sql_python_connector.egg-info/
+-rw-r--r--   0 root         (0)     1003    23771 2024-04-16 15:44:45.000000 cloud-sql-python-connector-1.9.0/cloud_sql_python_connector.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003      876 2024-04-16 15:44:45.000000 cloud-sql-python-connector-1.9.0/cloud_sql_python_connector.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2024-04-16 15:44:45.000000 cloud-sql-python-connector-1.9.0/cloud_sql_python_connector.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003        1 2024-04-16 15:44:45.000000 cloud-sql-python-connector-1.9.0/cloud_sql_python_connector.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      156 2024-04-16 15:44:45.000000 cloud-sql-python-connector-1.9.0/cloud_sql_python_connector.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2024-04-16 15:44:45.000000 cloud-sql-python-connector-1.9.0/cloud_sql_python_connector.egg-info/top_level.txt
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 15:44:45.679346 cloud-sql-python-connector-1.9.0/google/
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 15:44:45.679346 cloud-sql-python-connector-1.9.0/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 15:44:45.679346 cloud-sql-python-connector-1.9.0/google/cloud/sql/
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-16 15:44:45.683349 cloud-sql-python-connector-1.9.0/google/cloud/sql/connector/
+-rw-rw-r--   0 root         (0)     1003      883 2024-04-16 15:42:12.000000 cloud-sql-python-connector-1.9.0/google/cloud/sql/connector/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1838 2024-04-16 15:42:12.000000 cloud-sql-python-connector-1.9.0/google/cloud/sql/connector/asyncpg.py
+-rw-rw-r--   0 root         (0)     1003     8494 2024-04-16 15:42:12.000000 cloud-sql-python-connector-1.9.0/google/cloud/sql/connector/client.py
+-rwxrwxr-x   0 root         (0)     1003    19188 2024-04-16 15:42:12.000000 cloud-sql-python-connector-1.9.0/google/cloud/sql/connector/connector.py
+-rw-rw-r--   0 root         (0)     1003     1524 2024-04-16 15:42:12.000000 cloud-sql-python-connector-1.9.0/google/cloud/sql/connector/exceptions.py
+-rw-rw-r--   0 root         (0)     1003    14920 2024-04-16 15:42:12.000000 cloud-sql-python-connector-1.9.0/google/cloud/sql/connector/instance.py
+-rw-rw-r--   0 root         (0)     1003     1814 2024-04-16 15:42:12.000000 cloud-sql-python-connector-1.9.0/google/cloud/sql/connector/pg8000.py
+-rw-rw-r--   0 root         (0)     1003        0 2024-04-16 15:42:12.000000 cloud-sql-python-connector-1.9.0/google/cloud/sql/connector/py.typed
+-rw-rw-r--   0 root         (0)     1003     2105 2024-04-16 15:42:12.000000 cloud-sql-python-connector-1.9.0/google/cloud/sql/connector/pymysql.py
+-rw-rw-r--   0 root         (0)     1003     2452 2024-04-16 15:42:12.000000 cloud-sql-python-connector-1.9.0/google/cloud/sql/connector/pytds.py
+-rw-rw-r--   0 root         (0)     1003     2993 2024-04-16 15:42:12.000000 cloud-sql-python-connector-1.9.0/google/cloud/sql/connector/rate_limiter.py
+-rw-rw-r--   0 root         (0)     1003     3680 2024-04-16 15:42:12.000000 cloud-sql-python-connector-1.9.0/google/cloud/sql/connector/refresh_utils.py
+-rwxrwxr-x   0 root         (0)     1003     3448 2024-04-16 15:42:12.000000 cloud-sql-python-connector-1.9.0/google/cloud/sql/connector/utils.py
+-rw-rw-r--   0 root         (0)     1003      597 2024-04-16 15:42:12.000000 cloud-sql-python-connector-1.9.0/google/cloud/sql/connector/version.py
+-rw-rw-r--   0 root         (0)     1003       67 2024-04-16 15:44:45.683349 cloud-sql-python-connector-1.9.0/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2897 2024-04-16 15:42:12.000000 cloud-sql-python-connector-1.9.0/setup.py
```

### Comparing `cloud-sql-python-connector-1.8.0/LICENSE` & `cloud-sql-python-connector-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cloud-sql-python-connector-1.8.0/PKG-INFO` & `cloud-sql-python-connector-1.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloud-sql-python-connector
-Version: 1.8.0
+Version: 1.9.0
 Summary: The Cloud SQL Python Connector is a library that can be used alongside a database driver to allow users with sufficient permissions to connect to a Cloud SQL database without having to manually allowlist IPs or manage SSL certificates.
 Home-page: https://github.com/GoogleCloudPlatform/cloud-sql-python-connector
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cloud-sql-python-connector Version: 1.8.0 Summary:
+Metadata-Version: 2.1 Name: cloud-sql-python-connector Version: 1.9.0 Summary:
 The Cloud SQL Python Connector is a library that can be used alongside a
 database driver to allow users with sufficient permissions to connect to a
 Cloud SQL database without having to manually allowlist IPs or manage SSL
 certificates. Home-page: https://github.com/GoogleCloudPlatform/cloud-sql-
 python-connector Author: Google LLC Author-email: googleapis-
 packages@google.com License: Apache 2.0 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
```

### Comparing `cloud-sql-python-connector-1.8.0/README.md` & `cloud-sql-python-connector-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `cloud-sql-python-connector-1.8.0/cloud_sql_python_connector.egg-info/PKG-INFO` & `cloud-sql-python-connector-1.9.0/cloud_sql_python_connector.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloud-sql-python-connector
-Version: 1.8.0
+Version: 1.9.0
 Summary: The Cloud SQL Python Connector is a library that can be used alongside a database driver to allow users with sufficient permissions to connect to a Cloud SQL database without having to manually allowlist IPs or manage SSL certificates.
 Home-page: https://github.com/GoogleCloudPlatform/cloud-sql-python-connector
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cloud-sql-python-connector Version: 1.8.0 Summary:
+Metadata-Version: 2.1 Name: cloud-sql-python-connector Version: 1.9.0 Summary:
 The Cloud SQL Python Connector is a library that can be used alongside a
 database driver to allow users with sufficient permissions to connect to a
 Cloud SQL database without having to manually allowlist IPs or manage SSL
 certificates. Home-page: https://github.com/GoogleCloudPlatform/cloud-sql-
 python-connector Author: Google LLC Author-email: googleapis-
 packages@google.com License: Apache 2.0 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
```

### Comparing `cloud-sql-python-connector-1.8.0/cloud_sql_python_connector.egg-info/SOURCES.txt` & `cloud-sql-python-connector-1.9.0/cloud_sql_python_connector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cloud-sql-python-connector-1.8.0/google/cloud/sql/connector/__init__.py` & `cloud-sql-python-connector-1.9.0/google/cloud/sql/connector/__init__.py`

 * *Files identical despite different names*

### Comparing `cloud-sql-python-connector-1.8.0/google/cloud/sql/connector/asyncpg.py` & `cloud-sql-python-connector-1.9.0/google/cloud/sql/connector/asyncpg.py`

 * *Files identical despite different names*

### Comparing `cloud-sql-python-connector-1.8.0/google/cloud/sql/connector/client.py` & `cloud-sql-python-connector-1.9.0/google/cloud/sql/connector/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,29 +27,30 @@
 from google.cloud.sql.connector.version import __version__ as version
 
 if TYPE_CHECKING:
     from google.auth.credentials import Credentials
 
 USER_AGENT: str = f"cloud-sql-python-connector/{version}"
 API_VERSION: str = "v1beta4"
+DEFAULT_SERVICE_ENDPOINT: str = "https://sqladmin.googleapis.com"
 
 logger = logging.getLogger(name=__name__)
 
 
 def _format_user_agent(driver: Optional[str], custom: Optional[str]) -> str:
     agent = f"{USER_AGENT}+{driver}" if driver else USER_AGENT
-    if custom:
+    if custom and isinstance(custom, str):
         agent = f"{agent} {custom}"
     return agent
 
 
 class CloudSQLClient:
     def __init__(
         self,
-        sqladmin_api_endpoint: str,
+        sqladmin_api_endpoint: Optional[str],
         quota_project: Optional[str],
         credentials: Credentials,
         client: Optional[aiohttp.ClientSession] = None,
         driver: Optional[str] = None,
         user_agent: Optional[str] = None,
     ) -> None:
         """
@@ -77,15 +78,18 @@
             "Content-Type": "application/json",
         }
         if quota_project:
             headers["x-goog-user-project"] = quota_project
 
         self._client = client if client else aiohttp.ClientSession(headers=headers)
         self._credentials = credentials
-        self._sqladmin_api_endpoint = sqladmin_api_endpoint
+        if sqladmin_api_endpoint is None:
+            self._sqladmin_api_endpoint = DEFAULT_SERVICE_ENDPOINT
+        else:
+            self._sqladmin_api_endpoint = sqladmin_api_endpoint
         self._user_agent = user_agent
 
     async def _get_metadata(
         self,
         project: str,
         region: str,
         instance: str,
```

### Comparing `cloud-sql-python-connector-1.8.0/google/cloud/sql/connector/connector.py` & `cloud-sql-python-connector-1.9.0/google/cloud/sql/connector/connector.py`

 * *Files 8% similar despite different names*

```diff
@@ -39,67 +39,70 @@
 import google.cloud.sql.connector.pytds as pytds
 from google.cloud.sql.connector.utils import format_database_user
 from google.cloud.sql.connector.utils import generate_keys
 
 logger = logging.getLogger(name=__name__)
 
 ASYNC_DRIVERS = ["asyncpg"]
+_DEFAULT_SCHEME = "https://"
+_DEFAULT_UNIVERSE_DOMAIN = "googleapis.com"
+_SQLADMIN_HOST_TEMPLATE = "sqladmin.{universe_domain}"
 
 
 class Connector:
-    """A class to configure and create connections to Cloud SQL instances.
-
-    :type ip_type: str | IPTypes
-    :param ip_type
-        The IP type used to connect. IP types can be either IPTypes.PUBLIC
-        ("PUBLIC"), IPTypes.PRIVATE ("PRIVATE"), or IPTypes.PSC ("PSC").
-
-    :type enable_iam_auth: bool
-    :param enable_iam_auth
-        Enables automatic IAM database authentication for Postgres or MySQL
-        instances.
-
-    :type timeout: int
-    :param timeout
-        The time limit for a connection before raising a TimeoutError.
-
-    :type credentials: google.auth.credentials.Credentials
-    :param credentials
-        Credentials object used to authenticate connections to Cloud SQL server.
-        If not specified, Application Default Credentials are used.
-
-    :type quota_project: str
-    :param quota_project
-        The Project ID for an existing Google Cloud project. The project specified
-        is used for quota and billing purposes. If not specified, defaults to
-        project sourced from environment.
-
-    :type loop: asyncio.AbstractEventLoop
-    :param loop
-        Event loop to run asyncio tasks, if not specified, defaults to
-        creating new event loop on background thread.
-
-    :type sqladmin_api_endpoint: str
-    :param sqladmin_api_endpoint:
-        Base URL to use when calling the Cloud SQL Admin API endpoint.
-        Defaults to "https://sqladmin.googleapis.com", this argument should
-        only be used in development.
-    """
+    """Configure and create secure connections to Cloud SQL."""
 
     def __init__(
         self,
         ip_type: str | IPTypes = IPTypes.PUBLIC,
         enable_iam_auth: bool = False,
         timeout: int = 30,
         credentials: Optional[Credentials] = None,
         loop: Optional[asyncio.AbstractEventLoop] = None,
         quota_project: Optional[str] = None,
-        sqladmin_api_endpoint: str = "https://sqladmin.googleapis.com",
+        sqladmin_api_endpoint: Optional[str] = None,
         user_agent: Optional[str] = None,
+        universe_domain: Optional[str] = None,
     ) -> None:
+        """Initializes a Connector instance.
+
+        Args:
+            ip_type (str | IPTypes): The default IP address type used to connect to
+                Cloud SQL instances. Can be one of the following:
+                IPTypes.PUBLIC ("PUBLIC"), IPTypes.PRIVATE ("PRIVATE"), or
+                IPTypes.PSC ("PSC"). Default: IPTypes.PUBLIC
+
+            enable_iam_auth (bool): Enables automatic IAM database authentication
+                (Postgres and MySQL) as the default authentication method for all
+                connections.
+
+            timeout (int): The default time limit in seconds for a connection before
+                raising a TimeoutError.
+
+            credentials (google.auth.credentials.Credentials): A credentials object
+                created from the google-auth Python library to be used.
+                If not specified, Application Default Credentials (ADC) are used.
+
+            quota_project (str): The Project ID for an existing Google Cloud
+                project. The project specified is used for quota and billing
+                purposes. If not specified, defaults to project sourced from
+                environment.
+
+            loop (asyncio.AbstractEventLoop): Event loop to run asyncio tasks, if
+                not specified, defaults to creating new event loop on background
+                thread.
+
+            sqladmin_api_endpoint (str): Base URL to use when calling the Cloud SQL
+                Admin API endpoint. Defaults to "https://sqladmin.googleapis.com",
+                this argument should only be used in development.
+
+            universe_domain (str): The universe domain for Cloud SQL API calls.
+                Default: "googleapis.com".
+
+        """
         # if event loop is given, use for background tasks
         if loop:
             self._loop: asyncio.AbstractEventLoop = loop
             self._thread: Optional[Thread] = None
             self._keys: asyncio.Future = loop.create_task(generate_keys())
         # if no event loop is given, spin up new loop in background thread
         else:
@@ -127,46 +130,73 @@
         # otherwise use application default credentials
         else:
             self._credentials, _ = google.auth.default(scopes=scopes)
         # set default params for connections
         self._timeout = timeout
         self._enable_iam_auth = enable_iam_auth
         self._quota_project = quota_project
-        self._sqladmin_api_endpoint = sqladmin_api_endpoint
         self._user_agent = user_agent
         # if ip_type is str, convert to IPTypes enum
         if isinstance(ip_type, str):
             ip_type = IPTypes._from_str(ip_type)
         self._ip_type = ip_type
+        self._universe_domain = universe_domain
+        # construct service endpoint for Cloud SQL Admin API calls
+        if not sqladmin_api_endpoint:
+            self._sqladmin_api_endpoint = (
+                _DEFAULT_SCHEME
+                + _SQLADMIN_HOST_TEMPLATE.format(universe_domain=self.universe_domain)
+            )
+        # otherwise if endpoint override is passed in use it
+        else:
+            self._sqladmin_api_endpoint = sqladmin_api_endpoint
+
+        # validate that the universe domain of the credentials matches the
+        # universe domain of the service endpoint
+        if self._credentials.universe_domain != self.universe_domain:
+            raise ValueError(
+                f"The configured universe domain ({self.universe_domain}) does "
+                "not match the universe domain found in the credentials "
+                f"({self._credentials.universe_domain}). If you haven't "
+                "configured the universe domain explicitly, `googleapis.com` "
+                "is the default."
+            )
+
+    @property
+    def universe_domain(self) -> str:
+        return self._universe_domain or _DEFAULT_UNIVERSE_DOMAIN
 
     def connect(
         self, instance_connection_string: str, driver: str, **kwargs: Any
     ) -> Any:
-        """Prepares and returns a database connection object and starts a
-        background task to refresh the certificates and metadata.
+        """Connect to a Cloud SQL instance.
+
+        Prepares and returns a database connection object connected to a Cloud
+        SQL instance using SSL/TLS. Starts a background refresh to periodically
+        retrieve up-to-date ephemeral certificate and instance metadata.
 
-        :type instance_connection_string: str
-        :param instance_connection_string:
-            A string containing the GCP project name, region name, and instance
-            name separated by colons.
-
-            Example: example-proj:example-region-us6:example-instance
-
-        :type driver: str
-        :param: driver:
-            A string representing the driver to connect with. Supported drivers are
-            pymysql, pg8000, and pytds.
-
-        :param kwargs:
-            Pass in any driver-specific arguments needed to connect to the Cloud
-            SQL instance.
+        Args:
+            instance_connection_string (str): The instance connection name of the
+                Cloud SQL instance to connect to. Takes the form of
+                "project-id:region:instance-name"
 
-        :rtype: Connection
-        :returns:
+                Example: "my-project:us-central1:my-instance"
+
+            driver (str): A string representing the database driver to connect
+                with. Supported drivers are pymysql, pg8000, and pytds.
+
+            **kwargs: Any driver-specific arguments to pass to the underlying
+                driver .connect call.
+
+        Returns:
             A DB-API connection to the specified Cloud SQL instance.
+
+        Raises:
+            ConnectorLoopError: Event loop for background refresh is running in
+                current thread. Error instead of hanging indefinitely.
         """
         try:
             # check if event loop is running in current thread
             if self._loop == asyncio.get_running_loop():
                 raise ConnectorLoopError(
                     "Connector event loop is running in current thread!"
                     "Event loop must be attached to a different thread to prevent blocking code!"
@@ -180,43 +210,45 @@
             self.connect_async(instance_connection_string, driver, **kwargs), self._loop
         )
         return connect_task.result()
 
     async def connect_async(
         self, instance_connection_string: str, driver: str, **kwargs: Any
     ) -> Any:
-        """Prepares and returns a database connection object and starts a
-        background task to refresh the certificates and metadata.
+        """Connect asynchronously to a Cloud SQL instance.
+
+        Prepares and returns a database connection object connected to a Cloud
+        SQL instance using SSL/TLS. Schedules a refresh to periodically
+        retrieve up-to-date ephemeral certificate and instance metadata. Async
+        version of Connector.connect.
+
+        Args:
+            instance_connection_string (str): The instance connection name of the
+                Cloud SQL instance to connect to. Takes the form of
+                "project-id:region:instance-name"
 
-        :type instance_connection_string: str
-        :param instance_connection_string:
-            A string containing the GCP project name, region name, and instance
-            name separated by colons.
-
-            Example: example-proj:example-region-us6:example-instance
-
-        :type driver: str
-        :param: driver:
-            A string representing the driver to connect with. Supported drivers are
-            pymysql, pg8000, asyncpg, and pytds.
-
-        :param kwargs:
-            Pass in any driver-specific arguments needed to connect to the Cloud
-            SQL instance.
+                Example: "my-project:us-central1:my-instance"
 
-        :rtype: Connection
-        :returns:
+            driver (str): A string representing the database driver to connect
+                with. Supported drivers are pymysql, asyncpg, pg8000, and pytds.
+
+            **kwargs: Any driver-specific arguments to pass to the underlying
+                driver .connect call.
+
+        Returns:
             A DB-API connection to the specified Cloud SQL instance.
+
+        Raises:
+            ValueError: Connection attempt with built-in database authentication
+                and then subsequent attempt with IAM database authentication.
+            KeyError: Unsupported database driver Must be one of pymysql, asyncpg,
+                pg8000, and pytds.
+            DnsNameResolutionError: Could not resolve PSC IP address from DNS
+                host name.
         """
-        # Create an Instance object from the connection string.
-        # The Instance should verify arguments.
-        #
-        # Use the Instance to establish an SSL Connection.
-        #
-        # Return a DBAPI connection
         if self._client is None:
             # lazy init client as it has to be initialized in async context
             self._client = CloudSQLClient(
                 self._sqladmin_api_endpoint,
                 self._quota_project,
                 self._credentials,
                 user_agent=self._user_agent,
@@ -359,62 +391,61 @@
             *[instance.close() for instance in self._instances.values()]
         )
         if self._client:
             await self._client.close()
 
 
 async def create_async_connector(
-    ip_type: IPTypes = IPTypes.PUBLIC,
+    ip_type: str | IPTypes = IPTypes.PUBLIC,
     enable_iam_auth: bool = False,
     timeout: int = 30,
     credentials: Optional[Credentials] = None,
     loop: Optional[asyncio.AbstractEventLoop] = None,
     quota_project: Optional[str] = None,
-    sqladmin_api_endpoint: str = "https://sqladmin.googleapis.com",
+    sqladmin_api_endpoint: Optional[str] = None,
     user_agent: Optional[str] = None,
+    universe_domain: Optional[str] = None,
 ) -> Connector:
-    """
-     Create Connector object for asyncio connections that can auto-detect
-     and use current thread's running event loop.
+    """Helper function to create Connector object for asyncio connections.
+
+    Force use of Connector in an asyncio context. Auto-detect and use current
+    thread's running event loop.
+
+    Args:
+        ip_type (str | IPTypes): The default IP address type used to connect to
+            Cloud SQL instances. Can be one of the following:
+            IPTypes.PUBLIC ("PUBLIC"), IPTypes.PRIVATE ("PRIVATE"), or
+            IPTypes.PSC ("PSC"). Default: IPTypes.PUBLIC
+
+        enable_iam_auth (bool): Enables automatic IAM database authentication
+            (Postgres and MySQL) as the default authentication method for all
+            connections.
+
+        timeout (int): The default time limit in seconds for a connection before
+            raising a TimeoutError.
+
+        credentials (google.auth.credentials.Credentials): A credentials object
+            created from the google-auth Python library to be used.
+            If not specified, Application Default Credentials (ADC) are used.
+
+        quota_project (str): The Project ID for an existing Google Cloud
+            project. The project specified is used for quota and billing
+            purposes. If not specified, defaults to project sourced from
+            environment.
+
+        loop (asyncio.AbstractEventLoop): Event loop to run asyncio tasks, if
+            not specified, defaults to creating new event loop on background
+            thread.
+
+        sqladmin_api_endpoint (str): Base URL to use when calling the Cloud SQL
+            Admin API endpoint. Defaults to "https://sqladmin.googleapis.com",
+            this argument should only be used in development.
 
-    :type ip_type: IPTypes
-     :param ip_type
-         The IP type (public or private)  used to connect. IP types
-         can be either IPTypes.PUBLIC or IPTypes.PRIVATE.
-
-     :type enable_iam_auth: bool
-     :param enable_iam_auth
-         Enables automatic IAM database authentication for Postgres or MySQL
-         instances.
-
-     :type timeout: int
-     :param timeout
-         The time limit for a connection before raising a TimeoutError.
-
-     :type credentials: google.auth.credentials.Credentials
-     :param credentials
-         Credentials object used to authenticate connections to Cloud SQL server.
-         If not specified, Application Default Credentials are used.
-
-     :type quota_project: str
-     :param quota_project
-         The Project ID for an existing Google Cloud project. The project specified
-         is used for quota and billing purposes. If not specified, defaults to
-         project sourced from environment.
-
-     :type loop: asyncio.AbstractEventLoop
-     :param loop
-         Event loop to run asyncio tasks, if not specified, defaults to
-         creating new event loop on background thread.
-
-     :type sqladmin_api_endpoint: str
-     :param sqladmin_api_endpoint:
-         Base URL to use when calling the Cloud SQL Admin API endpoint.
-         Defaults to "https://sqladmin.googleapis.com", this argument should
-         only be used in development.
+    Returns:
+        A Connector instance configured with running event loop.
     """
     # if no loop given, automatically detect running event loop
     if loop is None:
         loop = asyncio.get_running_loop()
     return Connector(
         ip_type=ip_type,
         enable_iam_auth=enable_iam_auth,
```

### Comparing `cloud-sql-python-connector-1.8.0/google/cloud/sql/connector/exceptions.py` & `cloud-sql-python-connector-1.9.0/google/cloud/sql/connector/exceptions.py`

 * *Files identical despite different names*

### Comparing `cloud-sql-python-connector-1.8.0/google/cloud/sql/connector/instance.py` & `cloud-sql-python-connector-1.9.0/google/cloud/sql/connector/instance.py`

 * *Files identical despite different names*

### Comparing `cloud-sql-python-connector-1.8.0/google/cloud/sql/connector/pg8000.py` & `cloud-sql-python-connector-1.9.0/google/cloud/sql/connector/pg8000.py`

 * *Files identical despite different names*

### Comparing `cloud-sql-python-connector-1.8.0/google/cloud/sql/connector/pymysql.py` & `cloud-sql-python-connector-1.9.0/google/cloud/sql/connector/pymysql.py`

 * *Files identical despite different names*

### Comparing `cloud-sql-python-connector-1.8.0/google/cloud/sql/connector/pytds.py` & `cloud-sql-python-connector-1.9.0/google/cloud/sql/connector/pytds.py`

 * *Files identical despite different names*

### Comparing `cloud-sql-python-connector-1.8.0/google/cloud/sql/connector/rate_limiter.py` & `cloud-sql-python-connector-1.9.0/google/cloud/sql/connector/rate_limiter.py`

 * *Files identical despite different names*

### Comparing `cloud-sql-python-connector-1.8.0/google/cloud/sql/connector/refresh_utils.py` & `cloud-sql-python-connector-1.9.0/google/cloud/sql/connector/refresh_utils.py`

 * *Files identical despite different names*

### Comparing `cloud-sql-python-connector-1.8.0/google/cloud/sql/connector/utils.py` & `cloud-sql-python-connector-1.9.0/google/cloud/sql/connector/utils.py`

 * *Files identical despite different names*

### Comparing `cloud-sql-python-connector-1.8.0/google/cloud/sql/connector/version.py` & `cloud-sql-python-connector-1.9.0/google/cloud/sql/connector/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "1.8.0"
+__version__ = "1.9.0"
```

### Comparing `cloud-sql-python-connector-1.8.0/setup.py` & `cloud-sql-python-connector-1.9.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -73,15 +73,15 @@
         "Programming Language :: Python :: 3.12",
     ],
     platforms="Posix; MacOS X; Windows",
     packages=packages,
     install_requires=dependencies,
     extras_require={
         "pymysql": ["PyMySQL>=1.1.0"],
-        "pg8000": ["pg8000>=1.30.5"],
+        "pg8000": ["pg8000>=1.31.1"],
         "pytds": ["python-tds>=1.15.0"],
         "asyncpg": ["asyncpg>=0.29.0"],
     },
     python_requires=">=3.8",
     include_package_data=True,
     zip_safe=False,
     package_data={"google.cloud.sql.connector": ["py.typed"]},
```

