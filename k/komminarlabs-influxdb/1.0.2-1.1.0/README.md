# Comparing `tmp/komminarlabs_influxdb-1.0.2.tar.gz` & `tmp/komminarlabs_influxdb-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "komminarlabs_influxdb-1.0.2.tar", last modified: Wed Apr  3 16:46:58 2024, max compression
+gzip compressed data, was "komminarlabs_influxdb-1.1.0.tar", last modified: Tue Apr 16 12:41:21 2024, max compression
```

## Comparing `komminarlabs_influxdb-1.0.2.tar` & `komminarlabs_influxdb-1.1.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:46:58.423710 komminarlabs_influxdb-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-04-03 16:46:58.423710 komminarlabs_influxdb-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-03 16:46:58.000000 komminarlabs_influxdb-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:46:58.423710 komminarlabs_influxdb-1.0.2/komminarlabs_influxdb/
--rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-04-03 16:46:58.000000 komminarlabs_influxdb-1.0.2/komminarlabs_influxdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4279 2024-04-03 16:46:58.000000 komminarlabs_influxdb-1.0.2/komminarlabs_influxdb/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9282 2024-04-03 16:46:58.000000 komminarlabs_influxdb-1.0.2/komminarlabs_influxdb/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    20570 2024-04-03 16:46:58.000000 komminarlabs_influxdb-1.0.2/komminarlabs_influxdb/authorization.py
--rw-r--r--   0 runner    (1001) docker     (127)    15166 2024-04-03 16:46:58.000000 komminarlabs_influxdb-1.0.2/komminarlabs_influxdb/bucket.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:46:58.423710 komminarlabs_influxdb-1.0.2/komminarlabs_influxdb/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-03 16:46:58.000000 komminarlabs_influxdb-1.0.2/komminarlabs_influxdb/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-03 16:46:58.000000 komminarlabs_influxdb-1.0.2/komminarlabs_influxdb/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)     7155 2024-04-03 16:46:58.000000 komminarlabs_influxdb-1.0.2/komminarlabs_influxdb/get_authorization.py
--rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-04-03 16:46:58.000000 komminarlabs_influxdb-1.0.2/komminarlabs_influxdb/get_authorizations.py
--rw-r--r--   0 runner    (1001) docker     (127)     5391 2024-04-03 16:46:58.000000 komminarlabs_influxdb-1.0.2/komminarlabs_influxdb/get_bucket.py
--rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-04-03 16:46:58.000000 komminarlabs_influxdb-1.0.2/komminarlabs_influxdb/get_buckets.py
--rw-r--r--   0 runner    (1001) docker     (127)     4143 2024-04-03 16:46:58.000000 komminarlabs_influxdb-1.0.2/komminarlabs_influxdb/get_organization.py
--rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-04-03 16:46:58.000000 komminarlabs_influxdb-1.0.2/komminarlabs_influxdb/get_organizations.py
--rw-r--r--   0 runner    (1001) docker     (127)     9224 2024-04-03 16:46:58.000000 komminarlabs_influxdb-1.0.2/komminarlabs_influxdb/organization.py
--rw-r--r--   0 runner    (1001) docker     (127)    17872 2024-04-03 16:46:58.000000 komminarlabs_influxdb-1.0.2/komminarlabs_influxdb/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5482 2024-04-03 16:46:58.000000 komminarlabs_influxdb-1.0.2/komminarlabs_influxdb/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-03 16:46:58.000000 komminarlabs_influxdb-1.0.2/komminarlabs_influxdb/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:46:58.000000 komminarlabs_influxdb-1.0.2/komminarlabs_influxdb/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:46:58.423710 komminarlabs_influxdb-1.0.2/komminarlabs_influxdb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-04-03 16:46:58.000000 komminarlabs_influxdb-1.0.2/komminarlabs_influxdb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      960 2024-04-03 16:46:58.000000 komminarlabs_influxdb-1.0.2/komminarlabs_influxdb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 16:46:58.000000 komminarlabs_influxdb-1.0.2/komminarlabs_influxdb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 16:46:58.000000 komminarlabs_influxdb-1.0.2/komminarlabs_influxdb.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-03 16:46:58.000000 komminarlabs_influxdb-1.0.2/komminarlabs_influxdb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-03 16:46:58.000000 komminarlabs_influxdb-1.0.2/komminarlabs_influxdb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 16:46:58.423710 komminarlabs_influxdb-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-04-03 16:46:58.000000 komminarlabs_influxdb-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 12:41:21.596757 komminarlabs_influxdb-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-04-16 12:41:21.596757 komminarlabs_influxdb-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-16 12:41:21.000000 komminarlabs_influxdb-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 12:41:21.592757 komminarlabs_influxdb-1.1.0/komminarlabs_influxdb/
+-rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-04-16 12:41:21.000000 komminarlabs_influxdb-1.1.0/komminarlabs_influxdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4419 2024-04-16 12:41:21.000000 komminarlabs_influxdb-1.1.0/komminarlabs_influxdb/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9282 2024-04-16 12:41:21.000000 komminarlabs_influxdb-1.1.0/komminarlabs_influxdb/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20570 2024-04-16 12:41:21.000000 komminarlabs_influxdb-1.1.0/komminarlabs_influxdb/authorization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15166 2024-04-16 12:41:21.000000 komminarlabs_influxdb-1.1.0/komminarlabs_influxdb/bucket.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 12:41:21.596757 komminarlabs_influxdb-1.1.0/komminarlabs_influxdb/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-16 12:41:21.000000 komminarlabs_influxdb-1.1.0/komminarlabs_influxdb/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-16 12:41:21.000000 komminarlabs_influxdb-1.1.0/komminarlabs_influxdb/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7155 2024-04-16 12:41:21.000000 komminarlabs_influxdb-1.1.0/komminarlabs_influxdb/get_authorization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-04-16 12:41:21.000000 komminarlabs_influxdb-1.1.0/komminarlabs_influxdb/get_authorizations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5391 2024-04-16 12:41:21.000000 komminarlabs_influxdb-1.1.0/komminarlabs_influxdb/get_bucket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-04-16 12:41:21.000000 komminarlabs_influxdb-1.1.0/komminarlabs_influxdb/get_buckets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4143 2024-04-16 12:41:21.000000 komminarlabs_influxdb-1.1.0/komminarlabs_influxdb/get_organization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-04-16 12:41:21.000000 komminarlabs_influxdb-1.1.0/komminarlabs_influxdb/get_organizations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9224 2024-04-16 12:41:21.000000 komminarlabs_influxdb-1.1.0/komminarlabs_influxdb/organization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18008 2024-04-16 12:41:21.000000 komminarlabs_influxdb-1.1.0/komminarlabs_influxdb/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5482 2024-04-16 12:41:21.000000 komminarlabs_influxdb-1.1.0/komminarlabs_influxdb/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-16 12:41:21.000000 komminarlabs_influxdb-1.1.0/komminarlabs_influxdb/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 12:41:21.000000 komminarlabs_influxdb-1.1.0/komminarlabs_influxdb/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 12:41:21.592757 komminarlabs_influxdb-1.1.0/komminarlabs_influxdb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-04-16 12:41:21.000000 komminarlabs_influxdb-1.1.0/komminarlabs_influxdb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-04-16 12:41:21.000000 komminarlabs_influxdb-1.1.0/komminarlabs_influxdb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 12:41:21.000000 komminarlabs_influxdb-1.1.0/komminarlabs_influxdb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 12:41:21.000000 komminarlabs_influxdb-1.1.0/komminarlabs_influxdb.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-16 12:41:21.000000 komminarlabs_influxdb-1.1.0/komminarlabs_influxdb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-16 12:41:21.000000 komminarlabs_influxdb-1.1.0/komminarlabs_influxdb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 12:41:21.596757 komminarlabs_influxdb-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-04-16 12:41:21.000000 komminarlabs_influxdb-1.1.0/setup.py
```

### Comparing `komminarlabs_influxdb-1.0.2/PKG-INFO` & `komminarlabs_influxdb-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: komminarlabs_influxdb
-Version: 1.0.2
+Version: 1.1.0
 Summary: A Pulumi package for creating and managing InfluxDB resources.
 Home-page: https://www.influxdata.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/komminarlabs/pulumi-influxdb
 Keywords: pulumi influxdb category/database
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

### Comparing `komminarlabs_influxdb-1.0.2/README.md` & `komminarlabs_influxdb-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `komminarlabs_influxdb-1.0.2/komminarlabs_influxdb/__init__.py` & `komminarlabs_influxdb-1.1.0/komminarlabs_influxdb/__init__.py`

 * *Files identical despite different names*

### Comparing `komminarlabs_influxdb-1.0.2/komminarlabs_influxdb/_inputs.py` & `komminarlabs_influxdb-1.1.0/komminarlabs_influxdb/_inputs.py`

 * *Files 16% similar despite different names*

```diff
@@ -46,57 +46,35 @@
     def resource(self, value: pulumi.Input['AuthorizationPermissionResourceArgs']):
         pulumi.set(self, "resource", value)
 
 
 @pulumi.input_type
 class AuthorizationPermissionResourceArgs:
     def __init__(__self__, *,
-                 id: pulumi.Input[str],
-                 org_id: pulumi.Input[str],
                  type: pulumi.Input[str],
+                 id: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
-                 org: Optional[pulumi.Input[str]] = None):
+                 org: Optional[pulumi.Input[str]] = None,
+                 org_id: Optional[pulumi.Input[str]] = None):
         """
-        :param pulumi.Input[str] id: A resource ID. Identifies a specific resource.
-        :param pulumi.Input[str] org_id: An organization ID. Identifies the organization that owns the resource.
         :param pulumi.Input[str] type: A resource type. Identifies the API resource's type (or kind).
+        :param pulumi.Input[str] id: A resource ID. Identifies a specific resource.
         :param pulumi.Input[str] name: The name of the resource. **Note:** not all resource types have a name property.
         :param pulumi.Input[str] org: An organization name. The organization that owns the resource.
+        :param pulumi.Input[str] org_id: An organization ID. Identifies the organization that owns the resource.
         """
-        pulumi.set(__self__, "id", id)
-        pulumi.set(__self__, "org_id", org_id)
         pulumi.set(__self__, "type", type)
+        if id is not None:
+            pulumi.set(__self__, "id", id)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if org is not None:
             pulumi.set(__self__, "org", org)
-
-    @property
-    @pulumi.getter
-    def id(self) -> pulumi.Input[str]:
-        """
-        A resource ID. Identifies a specific resource.
-        """
-        return pulumi.get(self, "id")
-
-    @id.setter
-    def id(self, value: pulumi.Input[str]):
-        pulumi.set(self, "id", value)
-
-    @property
-    @pulumi.getter(name="orgId")
-    def org_id(self) -> pulumi.Input[str]:
-        """
-        An organization ID. Identifies the organization that owns the resource.
-        """
-        return pulumi.get(self, "org_id")
-
-    @org_id.setter
-    def org_id(self, value: pulumi.Input[str]):
-        pulumi.set(self, "org_id", value)
+        if org_id is not None:
+            pulumi.set(__self__, "org_id", org_id)
 
     @property
     @pulumi.getter
     def type(self) -> pulumi.Input[str]:
         """
         A resource type. Identifies the API resource's type (or kind).
         """
@@ -104,14 +82,26 @@
 
     @type.setter
     def type(self, value: pulumi.Input[str]):
         pulumi.set(self, "type", value)
 
     @property
     @pulumi.getter
+    def id(self) -> Optional[pulumi.Input[str]]:
+        """
+        A resource ID. Identifies a specific resource.
+        """
+        return pulumi.get(self, "id")
+
+    @id.setter
+    def id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "id", value)
+
+    @property
+    @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
         The name of the resource. **Note:** not all resource types have a name property.
         """
         return pulumi.get(self, "name")
 
     @name.setter
@@ -126,8 +116,20 @@
         """
         return pulumi.get(self, "org")
 
     @org.setter
     def org(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "org", value)
 
+    @property
+    @pulumi.getter(name="orgId")
+    def org_id(self) -> Optional[pulumi.Input[str]]:
+        """
+        An organization ID. Identifies the organization that owns the resource.
+        """
+        return pulumi.get(self, "org_id")
+
+    @org_id.setter
+    def org_id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "org_id", value)
+
```

### Comparing `komminarlabs_influxdb-1.0.2/komminarlabs_influxdb/_utilities.py` & `komminarlabs_influxdb-1.1.0/komminarlabs_influxdb/_utilities.py`

 * *Files identical despite different names*

### Comparing `komminarlabs_influxdb-1.0.2/komminarlabs_influxdb/authorization.py` & `komminarlabs_influxdb-1.1.0/komminarlabs_influxdb/authorization.py`

 * *Files identical despite different names*

### Comparing `komminarlabs_influxdb-1.0.2/komminarlabs_influxdb/bucket.py` & `komminarlabs_influxdb-1.1.0/komminarlabs_influxdb/bucket.py`

 * *Files identical despite different names*

### Comparing `komminarlabs_influxdb-1.0.2/komminarlabs_influxdb/config/vars.py` & `komminarlabs_influxdb-1.1.0/komminarlabs_influxdb/config/vars.py`

 * *Files identical despite different names*

### Comparing `komminarlabs_influxdb-1.0.2/komminarlabs_influxdb/get_authorization.py` & `komminarlabs_influxdb-1.1.0/komminarlabs_influxdb/get_authorization.py`

 * *Files identical despite different names*

### Comparing `komminarlabs_influxdb-1.0.2/komminarlabs_influxdb/get_authorizations.py` & `komminarlabs_influxdb-1.1.0/komminarlabs_influxdb/get_authorizations.py`

 * *Files identical despite different names*

### Comparing `komminarlabs_influxdb-1.0.2/komminarlabs_influxdb/get_bucket.py` & `komminarlabs_influxdb-1.1.0/komminarlabs_influxdb/get_bucket.py`

 * *Files identical despite different names*

### Comparing `komminarlabs_influxdb-1.0.2/komminarlabs_influxdb/get_buckets.py` & `komminarlabs_influxdb-1.1.0/komminarlabs_influxdb/get_buckets.py`

 * *Files identical despite different names*

### Comparing `komminarlabs_influxdb-1.0.2/komminarlabs_influxdb/get_organization.py` & `komminarlabs_influxdb-1.1.0/komminarlabs_influxdb/get_organization.py`

 * *Files identical despite different names*

### Comparing `komminarlabs_influxdb-1.0.2/komminarlabs_influxdb/get_organizations.py` & `komminarlabs_influxdb-1.1.0/komminarlabs_influxdb/get_organizations.py`

 * *Files identical despite different names*

### Comparing `komminarlabs_influxdb-1.0.2/komminarlabs_influxdb/organization.py` & `komminarlabs_influxdb-1.1.0/komminarlabs_influxdb/organization.py`

 * *Files identical despite different names*

### Comparing `komminarlabs_influxdb-1.0.2/komminarlabs_influxdb/outputs.py` & `komminarlabs_influxdb-1.1.0/komminarlabs_influxdb/outputs.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,57 +63,51 @@
         return super().__getitem__(key)
 
     def get(self, key: str, default = None) -> Any:
         AuthorizationPermissionResource.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
-                 id: str,
-                 org_id: str,
                  type: str,
+                 id: Optional[str] = None,
                  name: Optional[str] = None,
-                 org: Optional[str] = None):
+                 org: Optional[str] = None,
+                 org_id: Optional[str] = None):
         """
-        :param str id: A resource ID. Identifies a specific resource.
-        :param str org_id: An organization ID. Identifies the organization that owns the resource.
         :param str type: A resource type. Identifies the API resource's type (or kind).
+        :param str id: A resource ID. Identifies a specific resource.
         :param str name: The name of the resource. **Note:** not all resource types have a name property.
         :param str org: An organization name. The organization that owns the resource.
+        :param str org_id: An organization ID. Identifies the organization that owns the resource.
         """
-        pulumi.set(__self__, "id", id)
-        pulumi.set(__self__, "org_id", org_id)
         pulumi.set(__self__, "type", type)
+        if id is not None:
+            pulumi.set(__self__, "id", id)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if org is not None:
             pulumi.set(__self__, "org", org)
+        if org_id is not None:
+            pulumi.set(__self__, "org_id", org_id)
 
     @property
     @pulumi.getter
-    def id(self) -> str:
-        """
-        A resource ID. Identifies a specific resource.
-        """
-        return pulumi.get(self, "id")
-
-    @property
-    @pulumi.getter(name="orgId")
-    def org_id(self) -> str:
+    def type(self) -> str:
         """
-        An organization ID. Identifies the organization that owns the resource.
+        A resource type. Identifies the API resource's type (or kind).
         """
-        return pulumi.get(self, "org_id")
+        return pulumi.get(self, "type")
 
     @property
     @pulumi.getter
-    def type(self) -> str:
+    def id(self) -> Optional[str]:
         """
-        A resource type. Identifies the API resource's type (or kind).
+        A resource ID. Identifies a specific resource.
         """
-        return pulumi.get(self, "type")
+        return pulumi.get(self, "id")
 
     @property
     @pulumi.getter
     def name(self) -> Optional[str]:
         """
         The name of the resource. **Note:** not all resource types have a name property.
         """
@@ -123,14 +117,22 @@
     @pulumi.getter
     def org(self) -> Optional[str]:
         """
         An organization name. The organization that owns the resource.
         """
         return pulumi.get(self, "org")
 
+    @property
+    @pulumi.getter(name="orgId")
+    def org_id(self) -> Optional[str]:
+        """
+        An organization ID. Identifies the organization that owns the resource.
+        """
+        return pulumi.get(self, "org_id")
+
 
 @pulumi.output_type
 class GetAuthorizationPermissionResult(dict):
     def __init__(__self__, *,
                  action: str,
                  resource: 'outputs.GetAuthorizationPermissionResourceResult'):
         """
@@ -159,15 +161,15 @@
                  id: str,
                  name: str,
                  org: str,
                  org_id: str,
                  type: str):
         """
         :param str id: A resource ID. Identifies a specific resource.
-        :param str name: The name of the resource. Note: not all resource types have a name property.
+        :param str name: The name of the resource. **Note:** not all resource types have a name property.
         :param str org: An organization name. The organization that owns the resource.
         :param str org_id: An organization ID. Identifies the organization that owns the resource.
         :param str type: A resource type. Identifies the API resource's type (or kind).
         """
         pulumi.set(__self__, "id", id)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "org", org)
@@ -182,15 +184,15 @@
         """
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter
     def name(self) -> str:
         """
-        The name of the resource. Note: not all resource types have a name property.
+        The name of the resource. **Note:** not all resource types have a name property.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def org(self) -> str:
         """
@@ -374,15 +376,15 @@
                  id: str,
                  name: str,
                  org: str,
                  org_id: str,
                  type: str):
         """
         :param str id: The authorization ID.
-        :param str name: The name of the resource. Note: not all resource types have a name property.
+        :param str name: The name of the resource. **Note:** not all resource types have a name property.
         :param str org: An Organization name. Specifies the organization that owns the authorization.
         :param str org_id: An organization ID. Specifies the organization that owns the authorization.
         :param str type: A resource type. Identifies the API resource's type (or kind).
         """
         pulumi.set(__self__, "id", id)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "org", org)
@@ -397,15 +399,15 @@
         """
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter
     def name(self) -> str:
         """
-        The name of the resource. Note: not all resource types have a name property.
+        The name of the resource. **Note:** not all resource types have a name property.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def org(self) -> str:
         """
```

### Comparing `komminarlabs_influxdb-1.0.2/komminarlabs_influxdb/provider.py` & `komminarlabs_influxdb-1.1.0/komminarlabs_influxdb/provider.py`

 * *Files identical despite different names*

### Comparing `komminarlabs_influxdb-1.0.2/komminarlabs_influxdb.egg-info/PKG-INFO` & `komminarlabs_influxdb-1.1.0/komminarlabs_influxdb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: komminarlabs-influxdb
-Version: 1.0.2
+Version: 1.1.0
 Summary: A Pulumi package for creating and managing InfluxDB resources.
 Home-page: https://www.influxdata.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/komminarlabs/pulumi-influxdb
 Keywords: pulumi influxdb category/database
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

### Comparing `komminarlabs_influxdb-1.0.2/komminarlabs_influxdb.egg-info/SOURCES.txt` & `komminarlabs_influxdb-1.1.0/komminarlabs_influxdb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `komminarlabs_influxdb-1.0.2/setup.py` & `komminarlabs_influxdb-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import errno
 import os
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "1.0.2"
+VERSION = "1.1.0"
 def readme():
     try:
         with open('README.md', encoding='utf-8') as f:
             return f.read()
     except FileNotFoundError:
         return "influxdb Pulumi Package - Development Version"
```

