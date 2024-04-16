# Comparing `tmp/openapi_service_client-0.0.6.tar.gz` & `tmp/openapi_service_client-0.0.7.tar.gz`

## Comparing `openapi_service_client-0.0.6.tar` & `openapi_service_client-0.0.7.tar`

### file list

```diff
@@ -1,50 +1,50 @@
--rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 openapi_service_client-0.0.6/.github/workflows/pypi_release.yml
--rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 openapi_service_client-0.0.6/.github/workflows/tests.yml
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 openapi_service_client-0.0.6/src/openapi_service_client/__init__.py
--rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 openapi_service_client-0.0.6/src/openapi_service_client/client.py
--rw-r--r--   0        0        0     7030 2020-02-02 00:00:00.000000 openapi_service_client-0.0.6/src/openapi_service_client/client_configuration.py
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 openapi_service_client-0.0.6/src/openapi_service_client/config/__init__.py
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 openapi_service_client-0.0.6/src/openapi_service_client/config/auth_strategy.py
--rw-r--r--   0        0        0     3378 2020-02-02 00:00:00.000000 openapi_service_client-0.0.6/src/openapi_service_client/config/configuration.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 openapi_service_client-0.0.6/src/openapi_service_client/http_client/__init__.py
--rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 openapi_service_client-0.0.6/src/openapi_service_client/http_client/client.py
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 openapi_service_client-0.0.6/src/openapi_service_client/providers/__init__.py
--rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 openapi_service_client-0.0.6/src/openapi_service_client/providers/anthropic.py
--rw-r--r--   0        0        0     4924 2020-02-02 00:00:00.000000 openapi_service_client-0.0.6/src/openapi_service_client/providers/cohere.py
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 openapi_service_client-0.0.6/src/openapi_service_client/providers/converter.py
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 openapi_service_client-0.0.6/src/openapi_service_client/providers/llm_provider.py
--rw-r--r--   0        0        0     7295 2020-02-02 00:00:00.000000 openapi_service_client-0.0.6/src/openapi_service_client/providers/openai.py
--rw-r--r--   0        0        0     2592 2020-02-02 00:00:00.000000 openapi_service_client-0.0.6/src/openapi_service_client/providers/payload_extractor.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 openapi_service_client-0.0.6/src/openapi_service_client/request_builder/__init__.py
--rw-r--r--   0        0        0     3908 2020-02-02 00:00:00.000000 openapi_service_client-0.0.6/src/openapi_service_client/request_builder/builder.py
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 openapi_service_client-0.0.6/src/openapi_service_client/spec/__init__.py
--rw-r--r--   0        0        0     4440 2020-02-02 00:00:00.000000 openapi_service_client-0.0.6/src/openapi_service_client/spec/open_api_spec.py
--rw-r--r--   0        0        0     1869 2020-02-02 00:00:00.000000 openapi_service_client-0.0.6/src/openapi_service_client/spec/operation.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openapi_service_client-0.0.6/tests/__init__.py
--rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 openapi_service_client-0.0.6/tests/conftest.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openapi_service_client-0.0.6/tests/client/__init__.py
--rw-r--r--   0        0        0     4208 2020-02-02 00:00:00.000000 openapi_service_client-0.0.6/tests/client/test_client.py
--rw-r--r--   0        0        0     9768 2020-02-02 00:00:00.000000 openapi_service_client-0.0.6/tests/client/test_client_auth.py
--rw-r--r--   0        0        0     2254 2020-02-02 00:00:00.000000 openapi_service_client-0.0.6/tests/client/test_client_complex_request_body.py
--rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 openapi_service_client-0.0.6/tests/client/test_client_complex_request_body_mixed.py
--rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 openapi_service_client-0.0.6/tests/client/test_client_edge_cases.py
--rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 openapi_service_client-0.0.6/tests/client/test_client_error_handling.py
--rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 openapi_service_client-0.0.6/tests/client/test_client_live.py
--rw-r--r--   0        0        0     2532 2020-02-02 00:00:00.000000 openapi_service_client-0.0.6/tests/client/test_client_live_anthropic.py
--rw-r--r--   0        0        0     2807 2020-02-02 00:00:00.000000 openapi_service_client-0.0.6/tests/client/test_client_live_cohere.py
--rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 openapi_service_client-0.0.6/tests/client/test_client_live_openai.py
--rw-r--r--   0        0        0     3855 2020-02-02 00:00:00.000000 openapi_service_client-0.0.6/tests/client/test_cohere_conversion.py
--rw-r--r--   0        0        0     5251 2020-02-02 00:00:00.000000 openapi_service_client-0.0.6/tests/client/test_openai_conversion.py
--rw-r--r--   0        0        0     2782 2020-02-02 00:00:00.000000 openapi_service_client-0.0.6/tests/test_files/complex_types_openapi_service.json
--rw-r--r--   0        0        0    12430 2020-02-02 00:00:00.000000 openapi_service_client-0.0.6/tests/test_files/github_compare.yml
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 openapi_service_client-0.0.6/tests/test_files/openapi_edge_cases.yml
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 openapi_service_client-0.0.6/tests/test_files/openapi_error_handling.yml
--rw-r--r--   0        0        0     6411 2020-02-02 00:00:00.000000 openapi_service_client-0.0.6/tests/test_files/openapi_greeting_service.yml
--rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 openapi_service_client-0.0.6/tests/test_files/openapi_order_service.json
--rw-r--r--   0        0        0     1464 2020-02-02 00:00:00.000000 openapi_service_client-0.0.6/tests/test_files/openapi_order_service.yml
--rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 openapi_service_client-0.0.6/tests/test_files/serper.yaml
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 openapi_service_client-0.0.6/.gitignore
--rw-r--r--   0        0        0    11356 2020-02-02 00:00:00.000000 openapi_service_client-0.0.6/LICENSE
--rw-r--r--   0        0        0     7889 2020-02-02 00:00:00.000000 openapi_service_client-0.0.6/README.md
--rw-r--r--   0        0        0     3931 2020-02-02 00:00:00.000000 openapi_service_client-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     8836 2020-02-02 00:00:00.000000 openapi_service_client-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 openapi_service_client-0.0.7/.github/workflows/pypi_release.yml
+-rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 openapi_service_client-0.0.7/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 openapi_service_client-0.0.7/src/openapi_service_client/__init__.py
+-rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 openapi_service_client-0.0.7/src/openapi_service_client/client.py
+-rw-r--r--   0        0        0     7078 2020-02-02 00:00:00.000000 openapi_service_client-0.0.7/src/openapi_service_client/client_configuration.py
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 openapi_service_client-0.0.7/src/openapi_service_client/config/__init__.py
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 openapi_service_client-0.0.7/src/openapi_service_client/config/auth_strategy.py
+-rw-r--r--   0        0        0     3378 2020-02-02 00:00:00.000000 openapi_service_client-0.0.7/src/openapi_service_client/config/configuration.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 openapi_service_client-0.0.7/src/openapi_service_client/http_client/__init__.py
+-rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 openapi_service_client-0.0.7/src/openapi_service_client/http_client/client.py
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 openapi_service_client-0.0.7/src/openapi_service_client/providers/__init__.py
+-rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 openapi_service_client-0.0.7/src/openapi_service_client/providers/anthropic.py
+-rw-r--r--   0        0        0     4924 2020-02-02 00:00:00.000000 openapi_service_client-0.0.7/src/openapi_service_client/providers/cohere.py
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 openapi_service_client-0.0.7/src/openapi_service_client/providers/converter.py
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 openapi_service_client-0.0.7/src/openapi_service_client/providers/llm_provider.py
+-rw-r--r--   0        0        0     7295 2020-02-02 00:00:00.000000 openapi_service_client-0.0.7/src/openapi_service_client/providers/openai.py
+-rw-r--r--   0        0        0     2592 2020-02-02 00:00:00.000000 openapi_service_client-0.0.7/src/openapi_service_client/providers/payload_extractor.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 openapi_service_client-0.0.7/src/openapi_service_client/request_builder/__init__.py
+-rw-r--r--   0        0        0     3908 2020-02-02 00:00:00.000000 openapi_service_client-0.0.7/src/openapi_service_client/request_builder/builder.py
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 openapi_service_client-0.0.7/src/openapi_service_client/spec/__init__.py
+-rw-r--r--   0        0        0     4440 2020-02-02 00:00:00.000000 openapi_service_client-0.0.7/src/openapi_service_client/spec/open_api_spec.py
+-rw-r--r--   0        0        0     1869 2020-02-02 00:00:00.000000 openapi_service_client-0.0.7/src/openapi_service_client/spec/operation.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openapi_service_client-0.0.7/tests/__init__.py
+-rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 openapi_service_client-0.0.7/tests/conftest.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openapi_service_client-0.0.7/tests/client/__init__.py
+-rw-r--r--   0        0        0     4208 2020-02-02 00:00:00.000000 openapi_service_client-0.0.7/tests/client/test_client.py
+-rw-r--r--   0        0        0     9768 2020-02-02 00:00:00.000000 openapi_service_client-0.0.7/tests/client/test_client_auth.py
+-rw-r--r--   0        0        0     2254 2020-02-02 00:00:00.000000 openapi_service_client-0.0.7/tests/client/test_client_complex_request_body.py
+-rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 openapi_service_client-0.0.7/tests/client/test_client_complex_request_body_mixed.py
+-rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 openapi_service_client-0.0.7/tests/client/test_client_edge_cases.py
+-rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 openapi_service_client-0.0.7/tests/client/test_client_error_handling.py
+-rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 openapi_service_client-0.0.7/tests/client/test_client_live.py
+-rw-r--r--   0        0        0     2532 2020-02-02 00:00:00.000000 openapi_service_client-0.0.7/tests/client/test_client_live_anthropic.py
+-rw-r--r--   0        0        0     2807 2020-02-02 00:00:00.000000 openapi_service_client-0.0.7/tests/client/test_client_live_cohere.py
+-rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 openapi_service_client-0.0.7/tests/client/test_client_live_openai.py
+-rw-r--r--   0        0        0     3855 2020-02-02 00:00:00.000000 openapi_service_client-0.0.7/tests/client/test_cohere_conversion.py
+-rw-r--r--   0        0        0     5251 2020-02-02 00:00:00.000000 openapi_service_client-0.0.7/tests/client/test_openai_conversion.py
+-rw-r--r--   0        0        0     2782 2020-02-02 00:00:00.000000 openapi_service_client-0.0.7/tests/test_files/complex_types_openapi_service.json
+-rw-r--r--   0        0        0    12430 2020-02-02 00:00:00.000000 openapi_service_client-0.0.7/tests/test_files/github_compare.yml
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 openapi_service_client-0.0.7/tests/test_files/openapi_edge_cases.yml
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 openapi_service_client-0.0.7/tests/test_files/openapi_error_handling.yml
+-rw-r--r--   0        0        0     6411 2020-02-02 00:00:00.000000 openapi_service_client-0.0.7/tests/test_files/openapi_greeting_service.yml
+-rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 openapi_service_client-0.0.7/tests/test_files/openapi_order_service.json
+-rw-r--r--   0        0        0     1464 2020-02-02 00:00:00.000000 openapi_service_client-0.0.7/tests/test_files/openapi_order_service.yml
+-rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 openapi_service_client-0.0.7/tests/test_files/serper.yaml
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 openapi_service_client-0.0.7/.gitignore
+-rw-r--r--   0        0        0    11356 2020-02-02 00:00:00.000000 openapi_service_client-0.0.7/LICENSE
+-rw-r--r--   0        0        0     7829 2020-02-02 00:00:00.000000 openapi_service_client-0.0.7/README.md
+-rw-r--r--   0        0        0     3931 2020-02-02 00:00:00.000000 openapi_service_client-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     8776 2020-02-02 00:00:00.000000 openapi_service_client-0.0.7/PKG-INFO
```

### Comparing `openapi_service_client-0.0.6/.github/workflows/tests.yml` & `openapi_service_client-0.0.7/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.6/src/openapi_service_client/client.py` & `openapi_service_client-0.0.7/src/openapi_service_client/client.py`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.6/src/openapi_service_client/client_configuration.py` & `openapi_service_client-0.0.7/src/openapi_service_client/client_configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         pass
 
 
 class _DefaultOpenAPIServiceClientConfiguration(ClientConfiguration):
 
     def __init__(
         self,
-        openapi_spec: Union[str, Path],
+        openapi_spec: Union[str, Path, Dict[str, Any]],
         credentials: Optional[Union[str, Dict[str, Any], AuthenticationStrategy]] = None,
         http_client: Optional[AbstractHttpClient] = None,
         http_client_config: Optional[HttpClientConfig] = None,
         provider: Optional[LLMProvider] = None,
     ):
         if isinstance(openapi_spec, (str, Path)) and os.path.isfile(openapi_spec):
             self.openapi_spec = OpenAPISpecification.from_file(openapi_spec)
@@ -125,21 +125,21 @@
         """Check if a URL is a valid HTTP/HTTPS URL."""
         r = urlparse(url)
         return all([r.scheme in ["http", "https"], r.netloc])
 
 
 class ClientConfigurationBuilder:
     def __init__(self):
-        self._openapi_spec: Union[str, Path, None] = None
+        self._openapi_spec: Union[str, Path, Dict[str, Any], None] = None
         self._credentials: Optional[Union[str, Dict[str, Any], AuthenticationStrategy]] = None
         self._http_client: Optional[AbstractHttpClient] = None
         self._http_client_config: Optional[HttpClientConfig] = None
         self._provider: Optional[LLMProvider] = None
 
-    def with_openapi_spec(self, openapi_spec: Union[str, Path]) -> "ClientConfigurationBuilder":
+    def with_openapi_spec(self, openapi_spec: Union[str, Path, Dict[str, Any]]) -> "ClientConfigurationBuilder":
         self._openapi_spec = openapi_spec
         return self
 
     def with_credentials(
         self, credentials: Union[str, Dict[str, Any], AuthenticationStrategy]
     ) -> "ClientConfigurationBuilder":
         self._credentials = credentials
```

### Comparing `openapi_service_client-0.0.6/src/openapi_service_client/config/configuration.py` & `openapi_service_client-0.0.7/src/openapi_service_client/config/configuration.py`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.6/src/openapi_service_client/http_client/client.py` & `openapi_service_client-0.0.7/src/openapi_service_client/http_client/client.py`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.6/src/openapi_service_client/providers/__init__.py` & `openapi_service_client-0.0.7/src/openapi_service_client/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.6/src/openapi_service_client/providers/anthropic.py` & `openapi_service_client-0.0.7/src/openapi_service_client/providers/anthropic.py`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.6/src/openapi_service_client/providers/cohere.py` & `openapi_service_client-0.0.7/src/openapi_service_client/providers/cohere.py`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.6/src/openapi_service_client/providers/openai.py` & `openapi_service_client-0.0.7/src/openapi_service_client/providers/openai.py`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.6/src/openapi_service_client/providers/payload_extractor.py` & `openapi_service_client-0.0.7/src/openapi_service_client/providers/payload_extractor.py`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.6/src/openapi_service_client/request_builder/builder.py` & `openapi_service_client-0.0.7/src/openapi_service_client/request_builder/builder.py`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.6/src/openapi_service_client/spec/open_api_spec.py` & `openapi_service_client-0.0.7/src/openapi_service_client/spec/open_api_spec.py`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.6/src/openapi_service_client/spec/operation.py` & `openapi_service_client-0.0.7/src/openapi_service_client/spec/operation.py`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.6/tests/conftest.py` & `openapi_service_client-0.0.7/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.6/tests/client/test_client.py` & `openapi_service_client-0.0.7/tests/client/test_client.py`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.6/tests/client/test_client_auth.py` & `openapi_service_client-0.0.7/tests/client/test_client_auth.py`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.6/tests/client/test_client_complex_request_body.py` & `openapi_service_client-0.0.7/tests/client/test_client_complex_request_body.py`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.6/tests/client/test_client_complex_request_body_mixed.py` & `openapi_service_client-0.0.7/tests/client/test_client_complex_request_body_mixed.py`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.6/tests/client/test_client_edge_cases.py` & `openapi_service_client-0.0.7/tests/client/test_client_edge_cases.py`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.6/tests/client/test_client_error_handling.py` & `openapi_service_client-0.0.7/tests/client/test_client_error_handling.py`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.6/tests/client/test_client_live.py` & `openapi_service_client-0.0.7/tests/client/test_client_live.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import json
 import os
 
 import pytest
+import yaml
 
 from openapi_service_client.client import OpenAPIServiceClient
 from openapi_service_client.client_configuration import ClientConfigurationBuilder
 
 
 class TestClientLive:
 
@@ -17,21 +18,40 @@
             .with_credentials(os.getenv("SERPERDEV_API_KEY"))
             .build()
         )
         serper_api = OpenAPIServiceClient(config)
         payload = {
             "id": "call_NJr1NBz2Th7iUWJpRIJZoJIA",
             "function": {
-                "arguments": '{"q": "Who was Zoran Djindjic?"}',
+                "arguments": '{"q": "Who was Nikola Tesla?"}',
                 "name": "serperdev_search",
             },
             "type": "function",
         }
         response = serper_api.invoke(payload)
-        assert "politician" in str(response)
+        assert "invention" in str(response)
+
+    def test_serperdev_load_spec_first(self, test_files_path):
+        with open(test_files_path / "serper.yaml") as file:
+            loaded_spec = yaml.safe_load(file)
+
+        # use builder with dict spec
+        builder = ClientConfigurationBuilder()
+        config = builder.with_openapi_spec(loaded_spec).with_credentials(os.getenv("SERPERDEV_API_KEY")).build()
+        serper_api = OpenAPIServiceClient(config)
+        payload = {
+            "id": "call_NJr1NBz2Th7iUWJpRIJZoJIA",
+            "function": {
+                "arguments": '{"q": "Who was Nikola Tesla?"}',
+                "name": "serperdev_search",
+            },
+            "type": "function",
+        }
+        response = serper_api.invoke(payload)
+        assert "invention" in str(response)
 
     def test_github(self, test_files_path):
         builder = ClientConfigurationBuilder()
         config = builder.with_openapi_spec(test_files_path / "github_compare.yml").build()
         api = OpenAPIServiceClient(config)
 
         params = {"owner": "deepset-ai", "repo": "haystack", "basehead": "main...add_default_adapter_filters"}
```

### Comparing `openapi_service_client-0.0.6/tests/client/test_client_live_anthropic.py` & `openapi_service_client-0.0.7/tests/client/test_client_live_anthropic.py`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.6/tests/client/test_client_live_cohere.py` & `openapi_service_client-0.0.7/tests/client/test_client_live_cohere.py`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.6/tests/client/test_client_live_openai.py` & `openapi_service_client-0.0.7/tests/client/test_client_live_openai.py`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.6/tests/client/test_cohere_conversion.py` & `openapi_service_client-0.0.7/tests/client/test_cohere_conversion.py`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.6/tests/client/test_openai_conversion.py` & `openapi_service_client-0.0.7/tests/client/test_openai_conversion.py`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.6/tests/test_files/complex_types_openapi_service.json` & `openapi_service_client-0.0.7/tests/test_files/complex_types_openapi_service.json`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.6/tests/test_files/github_compare.yml` & `openapi_service_client-0.0.7/tests/test_files/github_compare.yml`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.6/tests/test_files/openapi_error_handling.yml` & `openapi_service_client-0.0.7/tests/test_files/openapi_error_handling.yml`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.6/tests/test_files/openapi_greeting_service.yml` & `openapi_service_client-0.0.7/tests/test_files/openapi_greeting_service.yml`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.6/tests/test_files/openapi_order_service.json` & `openapi_service_client-0.0.7/tests/test_files/openapi_order_service.json`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.6/tests/test_files/openapi_order_service.yml` & `openapi_service_client-0.0.7/tests/test_files/openapi_order_service.yml`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.6/tests/test_files/serper.yaml` & `openapi_service_client-0.0.7/tests/test_files/serper.yaml`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.6/.gitignore` & `openapi_service_client-0.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.6/LICENSE` & `openapi_service_client-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.6/README.md` & `openapi_service_client-0.0.7/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -3,26 +3,26 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/openapi-service-client.svg)](https://pypi.org/project/openapi-service-client)
 
 
 OpenAPI Service Client is a Python library that enables effortless integration between Large Language Models (LLMs) and services defined by OpenAPI specifications. It provides a simple and intuitive way to invoke REST services using the function-calling JSON format, making it easy to integrate with LLM-generated function calls.
 
 ## Motivation
 
-The OpenAPI Service Client library aims to simplify the process of invoking OpenAPI-defined services using function calling payloads from various LLM providers. By abstracting away the complexities of making HTTP requests, handling authentication, preparing invocation payloads and processing responses, it allows users to easily invoke underlying services regardless of the LLM provider.
+The OpenAPI Service Client library aims to simplify the process of invoking OpenAPI-defined services using function calling payloads from various LLM providers. By abstracting away the complexities of making HTTP requests, handling authentication, preparing invocation payloads and processing responses, it allows users to easily invoke underlying services with LLM generated function calls.
 
-The library supports multiple LLM providers, including OpenAI, Anthropic, and Cohere, making it a versatile tool for integrating LLMs with OpenAPI services. It also provides a flexible and extensible architecture that allows users to add support for additional LLM providers and function-calling payload formats.
+The library supports multiple LLM providers, including OpenAI, Anthropic, and Cohere, streamlining the process of integrating LLMs with OpenAPI services. It also provides a flexible and extensible architecture that allows users to add support for additional LLM providers and function-calling formats.
 
 ## Features
 
-- Easy integration with LLM-generated function calls using various function-calling JSON formats
+- Easy integration with LLM-generated function calls
 - Support for various LLM providers, including OpenAI, Anthropic, and Cohere
 - Automatic handling of REST invocations based on OpenAPI specifications
 - Support for various authentication strategies, including API key, HTTP authentication, and OAuth2
 - Flexible configuration options for adapting the client behavior
-- Extensible architecture for adding support for additional LLM providers and function-calling payload formats
+- Extensible architecture for adding support for additional LLM providers and function-calling formats
 
 
 ## Installation
 
 You can install OpenAPI Service Client using pip:
 
 ```shell
```

### Comparing `openapi_service_client-0.0.6/pyproject.toml` & `openapi_service_client-0.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.6/PKG-INFO` & `openapi_service_client-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: openapi-service-client
-Version: 0.0.6
+Version: 0.0.7
 Summary: A client library for invoking APIs based on provided OpenAPI specifications
 Project-URL: Documentation, https://github.com/vblagoje/openapi-service-client/blob/main/README.md
 Project-URL: Issues, https://github.com/vblagoje/openapi-service-client/issues
 Project-URL: Source, https://github.com/vblagoje/openapi-service-client
 Author-email: Vladimir Blagojevic <dovlex@gmail.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
@@ -25,26 +25,26 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/openapi-service-client.svg)](https://pypi.org/project/openapi-service-client)
 
 
 OpenAPI Service Client is a Python library that enables effortless integration between Large Language Models (LLMs) and services defined by OpenAPI specifications. It provides a simple and intuitive way to invoke REST services using the function-calling JSON format, making it easy to integrate with LLM-generated function calls.
 
 ## Motivation
 
-The OpenAPI Service Client library aims to simplify the process of invoking OpenAPI-defined services using function calling payloads from various LLM providers. By abstracting away the complexities of making HTTP requests, handling authentication, preparing invocation payloads and processing responses, it allows users to easily invoke underlying services regardless of the LLM provider.
+The OpenAPI Service Client library aims to simplify the process of invoking OpenAPI-defined services using function calling payloads from various LLM providers. By abstracting away the complexities of making HTTP requests, handling authentication, preparing invocation payloads and processing responses, it allows users to easily invoke underlying services with LLM generated function calls.
 
-The library supports multiple LLM providers, including OpenAI, Anthropic, and Cohere, making it a versatile tool for integrating LLMs with OpenAPI services. It also provides a flexible and extensible architecture that allows users to add support for additional LLM providers and function-calling payload formats.
+The library supports multiple LLM providers, including OpenAI, Anthropic, and Cohere, streamlining the process of integrating LLMs with OpenAPI services. It also provides a flexible and extensible architecture that allows users to add support for additional LLM providers and function-calling formats.
 
 ## Features
 
-- Easy integration with LLM-generated function calls using various function-calling JSON formats
+- Easy integration with LLM-generated function calls
 - Support for various LLM providers, including OpenAI, Anthropic, and Cohere
 - Automatic handling of REST invocations based on OpenAPI specifications
 - Support for various authentication strategies, including API key, HTTP authentication, and OAuth2
 - Flexible configuration options for adapting the client behavior
-- Extensible architecture for adding support for additional LLM providers and function-calling payload formats
+- Extensible architecture for adding support for additional LLM providers and function-calling formats
 
 
 ## Installation
 
 You can install OpenAPI Service Client using pip:
 
 ```shell
```

