# Comparing `tmp/mms_client-1.3.0.tar.gz` & `tmp/mms_client-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mms_client-1.3.0.tar", max compression
+gzip compressed data, was "mms_client-1.3.1.tar", max compression
```

## Comparing `mms_client-1.3.0.tar` & `mms_client-1.3.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     1211 2024-04-15 05:26:06.886885 mms_client-1.3.0/LICENSE
--rw-r--r--   0        0        0    13490 2024-04-15 05:26:06.886885 mms_client-1.3.0/README.md
--rw-r--r--   0        0        0     2913 2024-04-15 05:26:06.886885 mms_client-1.3.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-15 05:26:06.886885 mms_client-1.3.0/src/mms_client/__init__.py
--rw-r--r--   0        0        0      571 2024-04-15 05:26:06.886885 mms_client-1.3.0/src/mms_client/client.py
--rw-r--r--   0        0        0        0 2024-04-15 05:26:06.886885 mms_client-1.3.0/src/mms_client/py.typed
--rw-r--r--   0        0        0    10702 2024-04-15 05:26:06.886885 mms_client-1.3.0/src/mms_client/schemas/wsdl/mi-web-service-jbms.wsdl
--rw-r--r--   0        0        0     9894 2024-04-15 05:26:06.890885 mms_client-1.3.0/src/mms_client/schemas/wsdl/omi-web-service.wsdl
--rw-r--r--   0        0        0   109679 2024-04-15 05:26:06.890885 mms_client-1.3.0/src/mms_client/schemas/xsd/mi-market.xsd
--rw-r--r--   0        0        0    76166 2024-04-15 05:26:06.890885 mms_client-1.3.0/src/mms_client/schemas/xsd/mi-outbnd-reports.xsd
--rw-r--r--   0        0        0    13276 2024-04-15 05:26:06.890885 mms_client-1.3.0/src/mms_client/schemas/xsd/mi-report.xsd
--rw-r--r--   0        0        0    69149 2024-04-15 05:26:06.890885 mms_client-1.3.0/src/mms_client/schemas/xsd/mpr.xsd
--rw-r--r--   0        0        0    31524 2024-04-15 05:26:06.890885 mms_client-1.3.0/src/mms_client/schemas/xsd/omi.xsd
--rw-r--r--   0        0        0        0 2024-04-15 05:26:06.890885 mms_client-1.3.0/src/mms_client/security/__init__.py
--rw-r--r--   0        0        0     1489 2024-04-15 05:26:06.890885 mms_client-1.3.0/src/mms_client/security/certs.py
--rw-r--r--   0        0        0     2149 2024-04-15 05:26:06.890885 mms_client-1.3.0/src/mms_client/security/crypto.py
--rw-r--r--   0        0        0        0 2024-04-15 05:26:06.890885 mms_client-1.3.0/src/mms_client/services/__init__.py
--rw-r--r--   0        0        0    25839 2024-04-15 05:26:06.890885 mms_client-1.3.0/src/mms_client/services/base.py
--rw-r--r--   0        0        0     7574 2024-04-15 05:26:06.890885 mms_client-1.3.0/src/mms_client/services/market.py
--rw-r--r--   0        0        0      521 2024-04-15 05:26:06.890885 mms_client-1.3.0/src/mms_client/services/omi.py
--rw-r--r--   0        0        0     3651 2024-04-15 05:26:06.890885 mms_client-1.3.0/src/mms_client/services/registration.py
--rw-r--r--   0        0        0      537 2024-04-15 05:26:06.890885 mms_client-1.3.0/src/mms_client/services/report.py
--rw-r--r--   0        0        0        0 2024-04-15 05:26:06.890885 mms_client-1.3.0/src/mms_client/types/__init__.py
--rw-r--r--   0        0        0    14139 2024-04-15 05:26:06.890885 mms_client-1.3.0/src/mms_client/types/award.py
--rw-r--r--   0        0        0     9701 2024-04-15 05:26:06.890885 mms_client-1.3.0/src/mms_client/types/base.py
--rw-r--r--   0        0        0     1629 2024-04-15 05:26:06.890885 mms_client-1.3.0/src/mms_client/types/enums.py
--rw-r--r--   0        0        0    14785 2024-04-15 05:26:06.890885 mms_client-1.3.0/src/mms_client/types/fields.py
--rw-r--r--   0        0        0     2706 2024-04-15 05:26:06.890885 mms_client-1.3.0/src/mms_client/types/market.py
--rw-r--r--   0        0        0     6791 2024-04-15 05:26:06.890885 mms_client-1.3.0/src/mms_client/types/offer.py
--rw-r--r--   0        0        0     1381 2024-04-15 05:26:06.890885 mms_client-1.3.0/src/mms_client/types/registration.py
--rw-r--r--   0        0        0    65974 2024-04-15 05:26:06.890885 mms_client-1.3.0/src/mms_client/types/resource.py
--rw-r--r--   0        0        0     4399 2024-04-15 05:26:06.890885 mms_client-1.3.0/src/mms_client/types/transport.py
--rw-r--r--   0        0        0        0 2024-04-15 05:26:06.890885 mms_client-1.3.0/src/mms_client/utils/__init__.py
--rw-r--r--   0        0        0     2306 2024-04-15 05:26:06.890885 mms_client-1.3.0/src/mms_client/utils/errors.py
--rw-r--r--   0        0        0    29534 2024-04-15 05:26:06.890885 mms_client-1.3.0/src/mms_client/utils/serialization.py
--rw-r--r--   0        0        0     9653 2024-04-15 05:26:06.890885 mms_client-1.3.0/src/mms_client/utils/web.py
--rw-r--r--   0        0        0    14774 1970-01-01 00:00:00.000000 mms_client-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1211 2024-04-16 05:21:13.995898 mms_client-1.3.1/LICENSE
+-rw-r--r--   0        0        0    13490 2024-04-16 05:21:13.995898 mms_client-1.3.1/README.md
+-rw-r--r--   0        0        0     2913 2024-04-16 05:21:13.999898 mms_client-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-16 05:21:13.999898 mms_client-1.3.1/src/mms_client/__init__.py
+-rw-r--r--   0        0        0      571 2024-04-16 05:21:13.999898 mms_client-1.3.1/src/mms_client/client.py
+-rw-r--r--   0        0        0        0 2024-04-16 05:21:13.999898 mms_client-1.3.1/src/mms_client/py.typed
+-rw-r--r--   0        0        0    10702 2024-04-16 05:21:13.999898 mms_client-1.3.1/src/mms_client/schemas/wsdl/mi-web-service-jbms.wsdl
+-rw-r--r--   0        0        0     9894 2024-04-16 05:21:13.999898 mms_client-1.3.1/src/mms_client/schemas/wsdl/omi-web-service.wsdl
+-rw-r--r--   0        0        0   109679 2024-04-16 05:21:13.999898 mms_client-1.3.1/src/mms_client/schemas/xsd/mi-market.xsd
+-rw-r--r--   0        0        0    76166 2024-04-16 05:21:13.999898 mms_client-1.3.1/src/mms_client/schemas/xsd/mi-outbnd-reports.xsd
+-rw-r--r--   0        0        0    13276 2024-04-16 05:21:13.999898 mms_client-1.3.1/src/mms_client/schemas/xsd/mi-report.xsd
+-rw-r--r--   0        0        0    69149 2024-04-16 05:21:13.999898 mms_client-1.3.1/src/mms_client/schemas/xsd/mpr.xsd
+-rw-r--r--   0        0        0    31524 2024-04-16 05:21:13.999898 mms_client-1.3.1/src/mms_client/schemas/xsd/omi.xsd
+-rw-r--r--   0        0        0        0 2024-04-16 05:21:13.999898 mms_client-1.3.1/src/mms_client/security/__init__.py
+-rw-r--r--   0        0        0     1489 2024-04-16 05:21:13.999898 mms_client-1.3.1/src/mms_client/security/certs.py
+-rw-r--r--   0        0        0     2149 2024-04-16 05:21:13.999898 mms_client-1.3.1/src/mms_client/security/crypto.py
+-rw-r--r--   0        0        0        0 2024-04-16 05:21:13.999898 mms_client-1.3.1/src/mms_client/services/__init__.py
+-rw-r--r--   0        0        0    25839 2024-04-16 05:21:13.999898 mms_client-1.3.1/src/mms_client/services/base.py
+-rw-r--r--   0        0        0     7574 2024-04-16 05:21:13.999898 mms_client-1.3.1/src/mms_client/services/market.py
+-rw-r--r--   0        0        0      521 2024-04-16 05:21:13.999898 mms_client-1.3.1/src/mms_client/services/omi.py
+-rw-r--r--   0        0        0     3651 2024-04-16 05:21:13.999898 mms_client-1.3.1/src/mms_client/services/registration.py
+-rw-r--r--   0        0        0      537 2024-04-16 05:21:13.999898 mms_client-1.3.1/src/mms_client/services/report.py
+-rw-r--r--   0        0        0        0 2024-04-16 05:21:13.999898 mms_client-1.3.1/src/mms_client/types/__init__.py
+-rw-r--r--   0        0        0    14139 2024-04-16 05:21:13.999898 mms_client-1.3.1/src/mms_client/types/award.py
+-rw-r--r--   0        0        0     9710 2024-04-16 05:21:13.999898 mms_client-1.3.1/src/mms_client/types/base.py
+-rw-r--r--   0        0        0     1629 2024-04-16 05:21:13.999898 mms_client-1.3.1/src/mms_client/types/enums.py
+-rw-r--r--   0        0        0    14785 2024-04-16 05:21:13.999898 mms_client-1.3.1/src/mms_client/types/fields.py
+-rw-r--r--   0        0        0     2706 2024-04-16 05:21:13.999898 mms_client-1.3.1/src/mms_client/types/market.py
+-rw-r--r--   0        0        0     6791 2024-04-16 05:21:13.999898 mms_client-1.3.1/src/mms_client/types/offer.py
+-rw-r--r--   0        0        0     1381 2024-04-16 05:21:13.999898 mms_client-1.3.1/src/mms_client/types/registration.py
+-rw-r--r--   0        0        0    65974 2024-04-16 05:21:13.999898 mms_client-1.3.1/src/mms_client/types/resource.py
+-rw-r--r--   0        0        0     4399 2024-04-16 05:21:13.999898 mms_client-1.3.1/src/mms_client/types/transport.py
+-rw-r--r--   0        0        0        0 2024-04-16 05:21:13.999898 mms_client-1.3.1/src/mms_client/utils/__init__.py
+-rw-r--r--   0        0        0     2306 2024-04-16 05:21:14.003898 mms_client-1.3.1/src/mms_client/utils/errors.py
+-rw-r--r--   0        0        0    29534 2024-04-16 05:21:14.003898 mms_client-1.3.1/src/mms_client/utils/serialization.py
+-rw-r--r--   0        0        0     9653 2024-04-16 05:21:14.003898 mms_client-1.3.1/src/mms_client/utils/web.py
+-rw-r--r--   0        0        0    14774 1970-01-01 00:00:00.000000 mms_client-1.3.1/PKG-INFO
```

### Comparing `mms_client-1.3.0/LICENSE` & `mms_client-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mms_client-1.3.0/README.md` & `mms_client-1.3.1/README.md`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -138,22 +138,22 @@
 
 There's a lot of code here but it's not terribly difficult to understand. All this does is pull in the authentication data, create the client, create the payload, submit it to the server and retrieve the response.
 
 ## Connecting to a Test Server
 If you want to test your MMS connection, you can try using the test server:
 
 ```python
-client = MmsClient(participant="F100", user="FAKEUSER", client_type=ClientType.BSP, cert, is_admin=True)
+client = MmsClient(participant="F100", user="FAKEUSER", client_type=ClientType.BSP, cert, test=True)
 ```
 
 ## Connecting as a Market Admin
 If you're connecting as a market operator (MO), you can connect in admin mode:
 
 ```python
-client = MmsClient(participant="F100", user="FAKEUSER", client_type=ClientType.BSP, cert, test=True)
+client = MmsClient(participant="F100", user="FAKEUSER", client_type=ClientType.BSP, cert, is_admin=True)
 ```
 
 ## Log Settings
 The client also supports injection of a custom logger. The default logger is named "MMS Client".
 
 ```python
 client = MmsClient(participant="F100", user="FAKEUSER", client_type=ClientType.BSP, cert, logger=my_logger)
```

### Comparing `mms_client-1.3.0/pyproject.toml` & `mms_client-1.3.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mms_client"
-version = "v1.3.0"
+version = "v1.3.1"
 description = "API client for accessing the MMS"
 authors = ["Ryan Wood <ryan.wood@electroroute.co.jp>"]
 readme = "README.md"
 packages = [{ include = "mms_client", from = "src" }]
 homepage = "https://github.com/ElectroRoute-Japan/mms-client"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
```

### Comparing `mms_client-1.3.0/src/mms_client/client.py` & `mms_client-1.3.1/src/mms_client/client.py`

 * *Files identical despite different names*

### Comparing `mms_client-1.3.0/src/mms_client/schemas/wsdl/mi-web-service-jbms.wsdl` & `mms_client-1.3.1/src/mms_client/schemas/wsdl/mi-web-service-jbms.wsdl`

 * *Files identical despite different names*

### Comparing `mms_client-1.3.0/src/mms_client/schemas/wsdl/omi-web-service.wsdl` & `mms_client-1.3.1/src/mms_client/schemas/wsdl/omi-web-service.wsdl`

 * *Files identical despite different names*

### Comparing `mms_client-1.3.0/src/mms_client/schemas/xsd/mi-market.xsd` & `mms_client-1.3.1/src/mms_client/schemas/xsd/mi-market.xsd`

 * *Files identical despite different names*

### Comparing `mms_client-1.3.0/src/mms_client/schemas/xsd/mi-outbnd-reports.xsd` & `mms_client-1.3.1/src/mms_client/schemas/xsd/mi-outbnd-reports.xsd`

 * *Files identical despite different names*

### Comparing `mms_client-1.3.0/src/mms_client/schemas/xsd/mi-report.xsd` & `mms_client-1.3.1/src/mms_client/schemas/xsd/mi-report.xsd`

 * *Files identical despite different names*

### Comparing `mms_client-1.3.0/src/mms_client/schemas/xsd/mpr.xsd` & `mms_client-1.3.1/src/mms_client/schemas/xsd/mpr.xsd`

 * *Files identical despite different names*

### Comparing `mms_client-1.3.0/src/mms_client/schemas/xsd/omi.xsd` & `mms_client-1.3.1/src/mms_client/schemas/xsd/omi.xsd`

 * *Files identical despite different names*

### Comparing `mms_client-1.3.0/src/mms_client/security/certs.py` & `mms_client-1.3.1/src/mms_client/security/certs.py`

 * *Files identical despite different names*

### Comparing `mms_client-1.3.0/src/mms_client/security/crypto.py` & `mms_client-1.3.1/src/mms_client/security/crypto.py`

 * *Files identical despite different names*

### Comparing `mms_client-1.3.0/src/mms_client/services/base.py` & `mms_client-1.3.1/src/mms_client/services/base.py`

 * *Files identical despite different names*

### Comparing `mms_client-1.3.0/src/mms_client/services/market.py` & `mms_client-1.3.1/src/mms_client/services/market.py`

 * *Files identical despite different names*

### Comparing `mms_client-1.3.0/src/mms_client/services/omi.py` & `mms_client-1.3.1/src/mms_client/services/omi.py`

 * *Files identical despite different names*

### Comparing `mms_client-1.3.0/src/mms_client/services/registration.py` & `mms_client-1.3.1/src/mms_client/services/registration.py`

 * *Files identical despite different names*

### Comparing `mms_client-1.3.0/src/mms_client/services/report.py` & `mms_client-1.3.1/src/mms_client/services/report.py`

 * *Files identical despite different names*

### Comparing `mms_client-1.3.0/src/mms_client/types/award.py` & `mms_client-1.3.1/src/mms_client/types/award.py`

 * *Files identical despite different names*

### Comparing `mms_client-1.3.0/src/mms_client/types/base.py` & `mms_client-1.3.1/src/mms_client/types/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,15 +111,15 @@
 
     MARKET = "mi-market.xsd"
     REPORT = "mi-report.xsd"
     REGISTRATION = "mpr.xsd"
     OMI = "omi.xsd"
 
 
-class PayloadBase(BaseXmlModel, nsmap={"xsi": "http://www.w3.org/2001/XMLSchema"}):
+class PayloadBase(BaseXmlModel, nsmap={"xsi": "http://www.w3.org/2001/XMLSchema-instance"}):
     """Represents the base fields for an MMS request payload."""
 
     # The XML schema to use for validation
     location: SchemaType = attr(name="noNamespaceSchemaLocation", ns="xsi")
 
 
 class BaseResponse(BaseXmlModel, Generic[E], tag="BaseResponse"):
```

### Comparing `mms_client-1.3.0/src/mms_client/types/enums.py` & `mms_client-1.3.1/src/mms_client/types/enums.py`

 * *Files identical despite different names*

### Comparing `mms_client-1.3.0/src/mms_client/types/fields.py` & `mms_client-1.3.1/src/mms_client/types/fields.py`

 * *Files identical despite different names*

### Comparing `mms_client-1.3.0/src/mms_client/types/market.py` & `mms_client-1.3.1/src/mms_client/types/market.py`

 * *Files identical despite different names*

### Comparing `mms_client-1.3.0/src/mms_client/types/offer.py` & `mms_client-1.3.1/src/mms_client/types/offer.py`

 * *Files identical despite different names*

### Comparing `mms_client-1.3.0/src/mms_client/types/registration.py` & `mms_client-1.3.1/src/mms_client/types/registration.py`

 * *Files identical despite different names*

### Comparing `mms_client-1.3.0/src/mms_client/types/resource.py` & `mms_client-1.3.1/src/mms_client/types/resource.py`

 * *Files identical despite different names*

### Comparing `mms_client-1.3.0/src/mms_client/types/transport.py` & `mms_client-1.3.1/src/mms_client/types/transport.py`

 * *Files identical despite different names*

### Comparing `mms_client-1.3.0/src/mms_client/utils/errors.py` & `mms_client-1.3.1/src/mms_client/utils/errors.py`

 * *Files identical despite different names*

### Comparing `mms_client-1.3.0/src/mms_client/utils/serialization.py` & `mms_client-1.3.1/src/mms_client/utils/serialization.py`

 * *Files identical despite different names*

### Comparing `mms_client-1.3.0/src/mms_client/utils/web.py` & `mms_client-1.3.1/src/mms_client/utils/web.py`

 * *Files identical despite different names*

### Comparing `mms_client-1.3.0/PKG-INFO` & `mms_client-1.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mms-client
-Version: 1.3.0
+Version: 1.3.1
 Summary: API client for accessing the MMS
 Home-page: https://github.com/ElectroRoute-Japan/mms-client
 Author: Ryan Wood
 Author-email: ryan.wood@electroroute.co.jp
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Pydantic :: 2
@@ -170,22 +170,22 @@
 
 There's a lot of code here but it's not terribly difficult to understand. All this does is pull in the authentication data, create the client, create the payload, submit it to the server and retrieve the response.
 
 ## Connecting to a Test Server
 If you want to test your MMS connection, you can try using the test server:
 
 ```python
-client = MmsClient(participant="F100", user="FAKEUSER", client_type=ClientType.BSP, cert, is_admin=True)
+client = MmsClient(participant="F100", user="FAKEUSER", client_type=ClientType.BSP, cert, test=True)
 ```
 
 ## Connecting as a Market Admin
 If you're connecting as a market operator (MO), you can connect in admin mode:
 
 ```python
-client = MmsClient(participant="F100", user="FAKEUSER", client_type=ClientType.BSP, cert, test=True)
+client = MmsClient(participant="F100", user="FAKEUSER", client_type=ClientType.BSP, cert, is_admin=True)
 ```
 
 ## Log Settings
 The client also supports injection of a custom logger. The default logger is named "MMS Client".
 
 ```python
 client = MmsClient(participant="F100", user="FAKEUSER", client_type=ClientType.BSP, cert, logger=my_logger)
```

