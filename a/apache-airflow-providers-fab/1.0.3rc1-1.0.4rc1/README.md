# Comparing `tmp/apache_airflow_providers_fab-1.0.3rc1.tar.gz` & `tmp/apache_airflow_providers_fab-1.0.4rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache_airflow_providers_fab-1.0.3rc1.tar", last modified: Tue Apr  9 12:29:26 2024, max compression
+gzip compressed data, was "apache_airflow_providers_fab-1.0.4rc1.tar", last modified: Tue Apr 16 07:37:46 2024, max compression
```

## Comparing `apache_airflow_providers_fab-1.0.3rc1.tar` & `apache_airflow_providers_fab-1.0.4rc1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     3177 2024-04-09 12:29:26.000000 apache_airflow_providers_fab-1.0.3rc1/README.rst
--rw-r--r--   0        0        0    13569 2024-04-09 12:29:26.000000 apache_airflow_providers_fab-1.0.3rc1/airflow/providers/fab/LICENSE
--rw-r--r--   0        0        0     1578 2024-04-09 12:29:26.000000 apache_airflow_providers_fab-1.0.3rc1/airflow/providers/fab/__init__.py
--rw-r--r--   0        0        0      787 2024-04-09 12:29:26.000000 apache_airflow_providers_fab-1.0.3rc1/airflow/providers/fab/auth_manager/__init__.py
--rw-r--r--   0        0        0      787 2024-04-09 12:29:26.000000 apache_airflow_providers_fab-1.0.3rc1/airflow/providers/fab/auth_manager/api/__init__.py
--rw-r--r--   0        0        0      787 2024-04-09 12:29:26.000000 apache_airflow_providers_fab-1.0.3rc1/airflow/providers/fab/auth_manager/api/auth/__init__.py
--rw-r--r--   0        0        0      787 2024-04-09 12:29:26.000000 apache_airflow_providers_fab-1.0.3rc1/airflow/providers/fab/auth_manager/api/auth/backend/__init__.py
--rw-r--r--   0        0        0     2502 2024-04-09 12:29:26.000000 apache_airflow_providers_fab-1.0.3rc1/airflow/providers/fab/auth_manager/api/auth/backend/basic_auth.py
--rw-r--r--   0        0        0     1712 2024-04-09 12:29:26.000000 apache_airflow_providers_fab-1.0.3rc1/airflow/providers/fab/auth_manager/api/auth/backend/kerberos_auth.py
--rw-r--r--   0        0        0      785 2024-04-09 12:29:26.000000 apache_airflow_providers_fab-1.0.3rc1/airflow/providers/fab/auth_manager/api_endpoints/__init__.py
--rw-r--r--   0        0        0     7552 2024-04-09 12:29:26.000000 apache_airflow_providers_fab-1.0.3rc1/airflow/providers/fab/auth_manager/api_endpoints/role_and_permission_endpoint.py
--rw-r--r--   0        0        0     8484 2024-04-09 12:29:26.000000 apache_airflow_providers_fab-1.0.3rc1/airflow/providers/fab/auth_manager/api_endpoints/user_endpoint.py
--rw-r--r--   0        0        0      787 2024-04-09 12:29:26.000000 apache_airflow_providers_fab-1.0.3rc1/airflow/providers/fab/auth_manager/cli_commands/__init__.py
--rw-r--r--   0        0        0     9075 2024-04-09 12:29:26.000000 apache_airflow_providers_fab-1.0.3rc1/airflow/providers/fab/auth_manager/cli_commands/definition.py
--rw-r--r--   0        0        0     9098 2024-04-09 12:29:26.000000 apache_airflow_providers_fab-1.0.3rc1/airflow/providers/fab/auth_manager/cli_commands/role_command.py
--rw-r--r--   0        0        0     1663 2024-04-09 12:29:26.000000 apache_airflow_providers_fab-1.0.3rc1/airflow/providers/fab/auth_manager/cli_commands/sync_perm_command.py
--rw-r--r--   0        0        0    10207 2024-04-09 12:29:26.000000 apache_airflow_providers_fab-1.0.3rc1/airflow/providers/fab/auth_manager/cli_commands/user_command.py
--rw-r--r--   0        0        0     1768 2024-04-09 12:29:26.000000 apache_airflow_providers_fab-1.0.3rc1/airflow/providers/fab/auth_manager/cli_commands/utils.py
--rw-r--r--   0        0        0      787 2024-04-09 12:29:26.000000 apache_airflow_providers_fab-1.0.3rc1/airflow/providers/fab/auth_manager/decorators/__init__.py
--rw-r--r--   0        0        0     4948 2024-04-09 12:29:26.000000 apache_airflow_providers_fab-1.0.3rc1/airflow/providers/fab/auth_manager/decorators/auth.py
--rw-r--r--   0        0        0    19582 2024-04-09 12:29:26.000000 apache_airflow_providers_fab-1.0.3rc1/airflow/providers/fab/auth_manager/fab_auth_manager.py
--rw-r--r--   0        0        0     8827 2024-04-09 12:29:26.000000 apache_airflow_providers_fab-1.0.3rc1/airflow/providers/fab/auth_manager/models/__init__.py
--rw-r--r--   0        0        0     1775 2024-04-09 12:29:26.000000 apache_airflow_providers_fab-1.0.3rc1/airflow/providers/fab/auth_manager/models/anonymous_user.py
--rw-r--r--   0        0        0      785 2024-04-09 12:29:26.000000 apache_airflow_providers_fab-1.0.3rc1/airflow/providers/fab/auth_manager/openapi/__init__.py
--rw-r--r--   0        0        0    19380 2024-04-09 12:29:26.000000 apache_airflow_providers_fab-1.0.3rc1/airflow/providers/fab/auth_manager/openapi/v1.yaml
--rw-r--r--   0        0        0      787 2024-04-09 12:29:26.000000 apache_airflow_providers_fab-1.0.3rc1/airflow/providers/fab/auth_manager/security_manager/__init__.py
--rw-r--r--   0        0        0      907 2024-04-09 12:29:26.000000 apache_airflow_providers_fab-1.0.3rc1/airflow/providers/fab/auth_manager/security_manager/constants.py
--rw-r--r--   0        0        0   111437 2024-04-09 12:29:26.000000 apache_airflow_providers_fab-1.0.3rc1/airflow/providers/fab/auth_manager/security_manager/override.py
--rw-r--r--   0        0        0      785 2024-04-09 12:29:26.000000 apache_airflow_providers_fab-1.0.3rc1/airflow/providers/fab/auth_manager/views/__init__.py
--rw-r--r--   0        0        0     2886 2024-04-09 12:29:26.000000 apache_airflow_providers_fab-1.0.3rc1/airflow/providers/fab/auth_manager/views/permissions.py
--rw-r--r--   0        0        0     1494 2024-04-09 12:29:26.000000 apache_airflow_providers_fab-1.0.3rc1/airflow/providers/fab/auth_manager/views/roles_list.py
--rw-r--r--   0        0        0     5917 2024-04-09 12:29:26.000000 apache_airflow_providers_fab-1.0.3rc1/airflow/providers/fab/auth_manager/views/user.py
--rw-r--r--   0        0        0     2140 2024-04-09 12:29:26.000000 apache_airflow_providers_fab-1.0.3rc1/airflow/providers/fab/auth_manager/views/user_edit.py
--rw-r--r--   0        0        0     1300 2024-04-09 12:29:26.000000 apache_airflow_providers_fab-1.0.3rc1/airflow/providers/fab/auth_manager/views/user_stats.py
--rw-r--r--   0        0        0     2953 2024-04-09 12:29:26.000000 apache_airflow_providers_fab-1.0.3rc1/airflow/providers/fab/get_provider_info.py
--rw-r--r--   0        0        0     3023 2024-04-09 12:29:26.000000 apache_airflow_providers_fab-1.0.3rc1/pyproject.toml
--rw-r--r--   0        0        0     4957 1970-01-01 00:00:00.000000 apache_airflow_providers_fab-1.0.3rc1/PKG-INFO
+-rw-r--r--   0        0        0     3177 2024-04-16 07:37:46.000000 apache_airflow_providers_fab-1.0.4rc1/README.rst
+-rw-r--r--   0        0        0    13569 2024-04-16 07:37:46.000000 apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/LICENSE
+-rw-r--r--   0        0        0     1578 2024-04-16 07:37:46.000000 apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/__init__.py
+-rw-r--r--   0        0        0      787 2024-04-16 07:37:46.000000 apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/auth_manager/__init__.py
+-rw-r--r--   0        0        0      787 2024-04-16 07:37:46.000000 apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/auth_manager/api/__init__.py
+-rw-r--r--   0        0        0      787 2024-04-16 07:37:46.000000 apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/auth_manager/api/auth/__init__.py
+-rw-r--r--   0        0        0      787 2024-04-16 07:37:46.000000 apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/auth_manager/api/auth/backend/__init__.py
+-rw-r--r--   0        0        0     2502 2024-04-16 07:37:46.000000 apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/auth_manager/api/auth/backend/basic_auth.py
+-rw-r--r--   0        0        0     1712 2024-04-16 07:37:46.000000 apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/auth_manager/api/auth/backend/kerberos_auth.py
+-rw-r--r--   0        0        0      785 2024-04-16 07:37:46.000000 apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/auth_manager/api_endpoints/__init__.py
+-rw-r--r--   0        0        0     7552 2024-04-16 07:37:46.000000 apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/auth_manager/api_endpoints/role_and_permission_endpoint.py
+-rw-r--r--   0        0        0     8484 2024-04-16 07:37:46.000000 apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/auth_manager/api_endpoints/user_endpoint.py
+-rw-r--r--   0        0        0      787 2024-04-16 07:37:46.000000 apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/auth_manager/cli_commands/__init__.py
+-rw-r--r--   0        0        0     9075 2024-04-16 07:37:46.000000 apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/auth_manager/cli_commands/definition.py
+-rw-r--r--   0        0        0     9098 2024-04-16 07:37:46.000000 apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/auth_manager/cli_commands/role_command.py
+-rw-r--r--   0        0        0     1663 2024-04-16 07:37:46.000000 apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/auth_manager/cli_commands/sync_perm_command.py
+-rw-r--r--   0        0        0    10207 2024-04-16 07:37:46.000000 apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/auth_manager/cli_commands/user_command.py
+-rw-r--r--   0        0        0     1768 2024-04-16 07:37:46.000000 apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/auth_manager/cli_commands/utils.py
+-rw-r--r--   0        0        0      787 2024-04-16 07:37:46.000000 apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/auth_manager/decorators/__init__.py
+-rw-r--r--   0        0        0     4948 2024-04-16 07:37:46.000000 apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/auth_manager/decorators/auth.py
+-rw-r--r--   0        0        0    19563 2024-04-16 07:37:46.000000 apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/auth_manager/fab_auth_manager.py
+-rw-r--r--   0        0        0     8827 2024-04-16 07:37:46.000000 apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/auth_manager/models/__init__.py
+-rw-r--r--   0        0        0     1775 2024-04-16 07:37:46.000000 apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/auth_manager/models/anonymous_user.py
+-rw-r--r--   0        0        0      785 2024-04-16 07:37:46.000000 apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/auth_manager/openapi/__init__.py
+-rw-r--r--   0        0        0    19380 2024-04-16 07:37:46.000000 apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/auth_manager/openapi/v1.yaml
+-rw-r--r--   0        0        0      787 2024-04-16 07:37:46.000000 apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/auth_manager/security_manager/__init__.py
+-rw-r--r--   0        0        0      907 2024-04-16 07:37:46.000000 apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/auth_manager/security_manager/constants.py
+-rw-r--r--   0        0        0   111437 2024-04-16 07:37:46.000000 apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/auth_manager/security_manager/override.py
+-rw-r--r--   0        0        0      785 2024-04-16 07:37:46.000000 apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/auth_manager/views/__init__.py
+-rw-r--r--   0        0        0     2886 2024-04-16 07:37:46.000000 apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/auth_manager/views/permissions.py
+-rw-r--r--   0        0        0     1494 2024-04-16 07:37:46.000000 apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/auth_manager/views/roles_list.py
+-rw-r--r--   0        0        0     5995 2024-04-16 07:37:46.000000 apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/auth_manager/views/user.py
+-rw-r--r--   0        0        0     2140 2024-04-16 07:37:46.000000 apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/auth_manager/views/user_edit.py
+-rw-r--r--   0        0        0     1300 2024-04-16 07:37:46.000000 apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/auth_manager/views/user_stats.py
+-rw-r--r--   0        0        0     2962 2024-04-16 07:37:46.000000 apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/get_provider_info.py
+-rw-r--r--   0        0        0     3023 2024-04-16 07:37:46.000000 apache_airflow_providers_fab-1.0.4rc1/pyproject.toml
+-rw-r--r--   0        0        0     4957 1970-01-01 00:00:00.000000 apache_airflow_providers_fab-1.0.4rc1/PKG-INFO
```

### Comparing `apache_airflow_providers_fab-1.0.3rc1/README.rst` & `apache_airflow_providers_fab-1.0.4rc1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -38,28 +38,28 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-fab``
 
-Release: ``1.0.3.rc1``
+Release: ``1.0.4.rc1``
 
 
 `Flask App Builder <https://flask-appbuilder.readthedocs.io/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``fab`` provider. All classes for this provider package
 are in ``airflow.providers.fab`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-fab/1.0.3/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-fab/1.0.4/>`_.
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-fab``
@@ -76,8 +76,8 @@
 ``flask``             ``>=2.2,<2.3``
 ``flask-appbuilder``  ``==4.4.1``
 ``flask-login``       ``>=0.6.2``
 ``google-re2``        ``>=1.0``
 ====================  ==================
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-fab/1.0.3/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-fab/1.0.4/changelog.html>`_.
```

### Comparing `apache_airflow_providers_fab-1.0.3rc1/airflow/providers/fab/LICENSE` & `apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/LICENSE`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_fab-1.0.3rc1/airflow/providers/fab/__init__.py` & `apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 #
 from __future__ import annotations
 
 import packaging.version
 
 __all__ = ["__version__"]
 
-__version__ = "1.0.3"
+__version__ = "1.0.4"
 
 try:
     from airflow import __version__ as airflow_version
 except ImportError:
     from airflow.version import version as airflow_version
 
 if packaging.version.parse(packaging.version.parse(airflow_version).base_version) < packaging.version.parse(
```

### Comparing `apache_airflow_providers_fab-1.0.3rc1/airflow/providers/fab/auth_manager/__init__.py` & `apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/auth_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_fab-1.0.3rc1/airflow/providers/fab/auth_manager/api/__init__.py` & `apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/auth_manager/api/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_fab-1.0.3rc1/airflow/providers/fab/auth_manager/api/auth/__init__.py` & `apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/auth_manager/api/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_fab-1.0.3rc1/airflow/providers/fab/auth_manager/api/auth/backend/__init__.py` & `apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/auth_manager/api/auth/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_fab-1.0.3rc1/airflow/providers/fab/auth_manager/api/auth/backend/basic_auth.py` & `apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/auth_manager/api/auth/backend/basic_auth.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_fab-1.0.3rc1/airflow/providers/fab/auth_manager/api/auth/backend/kerberos_auth.py` & `apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/auth_manager/api/auth/backend/kerberos_auth.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_fab-1.0.3rc1/airflow/providers/fab/auth_manager/api_endpoints/__init__.py` & `apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/auth_manager/api_endpoints/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_fab-1.0.3rc1/airflow/providers/fab/auth_manager/api_endpoints/role_and_permission_endpoint.py` & `apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/auth_manager/api_endpoints/role_and_permission_endpoint.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_fab-1.0.3rc1/airflow/providers/fab/auth_manager/api_endpoints/user_endpoint.py` & `apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/auth_manager/api_endpoints/user_endpoint.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_fab-1.0.3rc1/airflow/providers/fab/auth_manager/cli_commands/__init__.py` & `apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/auth_manager/cli_commands/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_fab-1.0.3rc1/airflow/providers/fab/auth_manager/cli_commands/definition.py` & `apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/auth_manager/cli_commands/definition.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_fab-1.0.3rc1/airflow/providers/fab/auth_manager/cli_commands/role_command.py` & `apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/auth_manager/cli_commands/role_command.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_fab-1.0.3rc1/airflow/providers/fab/auth_manager/cli_commands/sync_perm_command.py` & `apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/auth_manager/cli_commands/sync_perm_command.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_fab-1.0.3rc1/airflow/providers/fab/auth_manager/cli_commands/user_command.py` & `apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/auth_manager/cli_commands/user_command.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_fab-1.0.3rc1/airflow/providers/fab/auth_manager/cli_commands/utils.py` & `apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/auth_manager/cli_commands/utils.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_fab-1.0.3rc1/airflow/providers/fab/auth_manager/decorators/__init__.py` & `apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/auth_manager/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_fab-1.0.3rc1/airflow/providers/fab/auth_manager/decorators/auth.py` & `apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/auth_manager/decorators/auth.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_fab-1.0.3rc1/airflow/providers/fab/auth_manager/fab_auth_manager.py` & `apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/auth_manager/fab_auth_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -346,16 +346,16 @@
 
         return FabAirflowSecurityManagerOverride(self.appbuilder)
 
     def get_url_login(self, **kwargs) -> str:
         """Return the login page url."""
         if not self.security_manager.auth_view:
             raise AirflowException("`auth_view` not defined in the security manager.")
-        if "next_url" in kwargs and kwargs["next_url"]:
-            return url_for(f"{self.security_manager.auth_view.endpoint}.login", next=kwargs["next_url"])
+        if next_url := kwargs.get("next_url"):
+            return url_for(f"{self.security_manager.auth_view.endpoint}.login", next=next_url)
         else:
             return url_for(f"{self.security_manager.auth_view.endpoint}.login")
 
     def get_url_logout(self):
         """Return the logout page url."""
         if not self.security_manager.auth_view:
             raise AirflowException("`auth_view` not defined in the security manager.")
```

### Comparing `apache_airflow_providers_fab-1.0.3rc1/airflow/providers/fab/auth_manager/models/__init__.py` & `apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/auth_manager/models/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_fab-1.0.3rc1/airflow/providers/fab/auth_manager/models/anonymous_user.py` & `apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/auth_manager/models/anonymous_user.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_fab-1.0.3rc1/airflow/providers/fab/auth_manager/openapi/__init__.py` & `apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/auth_manager/openapi/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_fab-1.0.3rc1/airflow/providers/fab/auth_manager/openapi/v1.yaml` & `apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/auth_manager/openapi/v1.yaml`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_fab-1.0.3rc1/airflow/providers/fab/auth_manager/security_manager/__init__.py` & `apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/auth_manager/security_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_fab-1.0.3rc1/airflow/providers/fab/auth_manager/security_manager/constants.py` & `apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/auth_manager/security_manager/constants.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_fab-1.0.3rc1/airflow/providers/fab/auth_manager/security_manager/override.py` & `apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/auth_manager/security_manager/override.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_fab-1.0.3rc1/airflow/providers/fab/auth_manager/views/__init__.py` & `apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/auth_manager/views/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_fab-1.0.3rc1/airflow/providers/fab/auth_manager/views/permissions.py` & `apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/auth_manager/views/permissions.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_fab-1.0.3rc1/airflow/providers/fab/auth_manager/views/roles_list.py` & `apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/auth_manager/views/roles_list.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_fab-1.0.3rc1/airflow/providers/fab/auth_manager/views/user.py` & `apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/auth_manager/views/user.py`

 * *Files 4% similar despite different names*

```diff
@@ -75,14 +75,15 @@
 
     @expose("/show/<pk>", methods=["GET"])
     @has_access
     def show(self, pk):
         pk = self._deserialize_pk_if_composite(pk)
         widgets = self._show(pk)
         widgets["show"].template_args["actions"].pop("userinfoedit", None)
+        widgets["show"].template_args["actions"].pop("resetmypassword", None)
         return self.render_template(
             self.show_template,
             pk=pk,
             title=self.show_title,
             widgets=widgets,
             related_views=self._related_views,
         )
```

### Comparing `apache_airflow_providers_fab-1.0.3rc1/airflow/providers/fab/auth_manager/views/user_edit.py` & `apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/auth_manager/views/user_edit.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_fab-1.0.3rc1/airflow/providers/fab/auth_manager/views/user_stats.py` & `apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/auth_manager/views/user_stats.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_fab-1.0.3rc1/airflow/providers/fab/get_provider_info.py` & `apache_airflow_providers_fab-1.0.4rc1/airflow/providers/fab/get_provider_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,16 +24,16 @@
 
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-fab",
         "name": "Fab",
         "description": "`Flask App Builder <https://flask-appbuilder.readthedocs.io/>`__\n",
         "state": "ready",
-        "source-date-epoch": 1712665766,
-        "versions": ["1.0.3", "1.0.2", "1.0.1", "1.0.0"],
+        "source-date-epoch": 1713253066,
+        "versions": ["1.0.4", "1.0.3", "1.0.2", "1.0.1", "1.0.0"],
         "dependencies": [
             "apache-airflow>=2.9.0",
             "flask>=2.2,<2.3",
             "flask-appbuilder==4.4.1",
             "flask-login>=0.6.2",
             "google-re2>=1.0",
         ],
```

### Comparing `apache_airflow_providers_fab-1.0.3rc1/pyproject.toml` & `apache_airflow_providers_fab-1.0.4rc1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "apache-airflow-providers-fab"
-version = "1.0.3.rc1"
+version = "1.0.4.rc1"
 description = "Provider package apache-airflow-providers-fab for Apache Airflow"
 readme = "README.rst"
 authors = [
     {name="Apache Software Foundation", email="dev@airflow.apache.org"},
 ]
 maintainers = [
     {name="Apache Software Foundation", email="dev@airflow.apache.org"},
@@ -60,16 +60,16 @@
     "flask-appbuilder==4.4.1",
     "flask-login>=0.6.2",
     "flask>=2.2,<2.3",
     "google-re2>=1.0",
 ]
 
 [project.urls]
-"Documentation" = "https://airflow.apache.org/docs/apache-airflow-providers-fab/1.0.3"
-"Changelog" = "https://airflow.apache.org/docs/apache-airflow-providers-fab/1.0.3/changelog.html"
+"Documentation" = "https://airflow.apache.org/docs/apache-airflow-providers-fab/1.0.4"
+"Changelog" = "https://airflow.apache.org/docs/apache-airflow-providers-fab/1.0.4/changelog.html"
 "Bug Tracker" = "https://github.com/apache/airflow/issues"
 "Source Code" = "https://github.com/apache/airflow"
 "Slack Chat" = "https://s.apache.org/airflow-slack"
 "Twitter" = "https://twitter.com/ApacheAirflow"
 "YouTube" = "https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/"
 
 [project.entry-points."apache_airflow_provider"]
```

### Comparing `apache_airflow_providers_fab-1.0.3rc1/PKG-INFO` & `apache_airflow_providers_fab-1.0.4rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-fab
-Version: 1.0.3rc1
+Version: 1.0.4rc1
 Summary: Provider package apache-airflow-providers-fab for Apache Airflow
 Keywords: airflow-provider,fab,airflow,integration
 Author-email: Apache Software Foundation <dev@airflow.apache.org>
 Maintainer-email: Apache Software Foundation <dev@airflow.apache.org>
 Requires-Python: ~=3.8
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
@@ -23,16 +23,16 @@
 Classifier: Topic :: System :: Monitoring
 Requires-Dist: apache-airflow>=2.9.0rc0
 Requires-Dist: flask-appbuilder==4.4.1
 Requires-Dist: flask-login>=0.6.2
 Requires-Dist: flask>=2.2,<2.3
 Requires-Dist: google-re2>=1.0
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
-Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-fab/1.0.3/changelog.html
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-fab/1.0.3
+Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-fab/1.0.4/changelog.html
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-fab/1.0.4
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 
 
 .. Licensed to the Apache Software Foundation (ASF) under one
@@ -74,28 +74,28 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-fab``
 
-Release: ``1.0.3.rc1``
+Release: ``1.0.4.rc1``
 
 
 `Flask App Builder <https://flask-appbuilder.readthedocs.io/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``fab`` provider. All classes for this provider package
 are in ``airflow.providers.fab`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-fab/1.0.3/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-fab/1.0.4/>`_.
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-fab``
@@ -112,8 +112,8 @@
 ``flask``             ``>=2.2,<2.3``
 ``flask-appbuilder``  ``==4.4.1``
 ``flask-login``       ``>=0.6.2``
 ``google-re2``        ``>=1.0``
 ====================  ==================
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-fab/1.0.3/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-fab/1.0.4/changelog.html>`_.
```

