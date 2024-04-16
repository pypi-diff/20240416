# Comparing `tmp/syntrac_opentelemetry_instrumentation_vertexai-0.0.1.tar.gz` & `tmp/syntrac_opentelemetry_instrumentation_vertexai-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syntrac_opentelemetry_instrumentation_vertexai-0.0.1.tar", max compression
+gzip compressed data, was "syntrac_opentelemetry_instrumentation_vertexai-0.0.2.tar", max compression
```

## Comparing `syntrac_opentelemetry_instrumentation_vertexai-0.0.1.tar` & `syntrac_opentelemetry_instrumentation_vertexai-0.0.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1189 2024-03-31 06:45:20.485214 syntrac_opentelemetry_instrumentation_vertexai-0.0.1/README.md
--rw-r--r--   0        0        0     2595 2024-03-31 06:45:20.790436 syntrac_opentelemetry_instrumentation_vertexai-0.0.1/pyproject.toml
--rw-r--r--   0        0        0    11471 2024-03-31 06:45:20.487476 syntrac_opentelemetry_instrumentation_vertexai-0.0.1/syntrac_opentelemetry/instrumentation/vertexai/__init__.py
--rw-r--r--   0        0        0       22 2024-03-31 06:45:20.488820 syntrac_opentelemetry_instrumentation_vertexai-0.0.1/syntrac_opentelemetry/instrumentation/vertexai/version.py
--rw-r--r--   0        0        0     2922 1970-01-01 00:00:00.000000 syntrac_opentelemetry_instrumentation_vertexai-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1189 2024-04-16 14:35:32.227721 syntrac_opentelemetry_instrumentation_vertexai-0.0.2/README.md
+-rw-r--r--   0        0        0     1318 2024-04-16 14:35:32.235246 syntrac_opentelemetry_instrumentation_vertexai-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0    11471 2024-04-16 14:35:32.229842 syntrac_opentelemetry_instrumentation_vertexai-0.0.2/syntrac_opentelemetry/instrumentation/vertexai/__init__.py
+-rw-r--r--   0        0        0       22 2024-04-16 14:35:32.231080 syntrac_opentelemetry_instrumentation_vertexai-0.0.2/syntrac_opentelemetry/instrumentation/vertexai/version.py
+-rw-r--r--   0        0        0     2288 1970-01-01 00:00:00.000000 syntrac_opentelemetry_instrumentation_vertexai-0.0.2/PKG-INFO
```

### Comparing `syntrac_opentelemetry_instrumentation_vertexai-0.0.1/README.md` & `syntrac_opentelemetry_instrumentation_vertexai-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `syntrac_opentelemetry_instrumentation_vertexai-0.0.1/syntrac_opentelemetry/instrumentation/vertexai/__init__.py` & `syntrac_opentelemetry_instrumentation_vertexai-0.0.2/syntrac_opentelemetry/instrumentation/vertexai/__init__.py`

 * *Files identical despite different names*

### Comparing `syntrac_opentelemetry_instrumentation_vertexai-0.0.1/PKG-INFO` & `syntrac_opentelemetry_instrumentation_vertexai-0.0.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,32 +1,27 @@
 Metadata-Version: 2.1
 Name: syntrac-opentelemetry-instrumentation-vertexai
-Version: 0.0.1
+Version: 0.0.2
 Summary: OpenTelemetry Vertex AI instrumentation
 Home-page: https://github.com/syntracAI/syntrac/tree/main/packages/python/opentelemetry-instrumentation-vertexai
 License: Apache-2.0
 Author: Gal Kleinman
 Author-email: gal@syntrac.com
 Requires-Python: >=3.9,<4
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: instruments
-Requires-Dist: deprecated (==1.2.14) ; python_version >= "3.9" and python_version < "4"
-Requires-Dist: importlib-metadata (==6.11.0) ; python_version >= "3.9" and python_version < "4"
-Requires-Dist: opentelemetry-api (==1.23.0) ; python_version >= "3.9" and python_version < "4"
-Requires-Dist: opentelemetry-instrumentation (==0.44b0) ; python_version >= "3.9" and python_version < "4"
-Requires-Dist: opentelemetry-semantic-conventions (==0.44b0) ; python_version >= "3.9" and python_version < "4"
-Requires-Dist: setuptools (==69.2.0) ; python_version >= "3.9" and python_version < "4"
-Requires-Dist: syntrac-opentelemetry-semantic-conventions-ai (==0.0.1) ; python_version >= "3.9" and python_version < "4"
-Requires-Dist: wrapt (==1.16.0) ; python_version >= "3.9" and python_version < "4"
-Requires-Dist: zipp (==3.18.1) ; python_version >= "3.9" and python_version < "4"
+Requires-Dist: opentelemetry-api (>=1.23.0,<2.0.0)
+Requires-Dist: opentelemetry-instrumentation (==0.44b0)
+Requires-Dist: opentelemetry-semantic-conventions (==0.44b0)
+Requires-Dist: syntrac-opentelemetry-semantic-conventions-ai (==0.0.1)
 Project-URL: Repository, https://github.com/syntracAI/syntrac/tree/main/packages/python/opentelemetry-instrumentation-vertexai
 Description-Content-Type: text/markdown
 
 # OpenTelemetry VertexAI Instrumentation
 
 <a href="https://pypi.org/project/syntrac-opentelemetry-instrumentation-vertexai/">
     <img src="https://badge.fury.io/py/syntrac-opentelemetry-instrumentation-vertexai.svg">
```

#### html2text {}

```diff
@@ -1,36 +1,28 @@
 Metadata-Version: 2.1 Name: syntrac-opentelemetry-instrumentation-vertexai
-Version: 0.0.1 Summary: OpenTelemetry Vertex AI instrumentation Home-page:
+Version: 0.0.2 Summary: OpenTelemetry Vertex AI instrumentation Home-page:
 https://github.com/syntracAI/syntrac/tree/main/packages/python/opentelemetry-
 instrumentation-vertexai License: Apache-2.0 Author: Gal Kleinman Author-email:
 gal@syntrac.com Requires-Python: >=3.9,<4 Classifier: License :: OSI Approved
 :: Apache Software License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12 Provides-Extra: instruments
-Requires-Dist: deprecated (==1.2.14) ; python_version >= "3.9" and
-python_version < "4" Requires-Dist: importlib-metadata (==6.11.0) ;
-python_version >= "3.9" and python_version < "4" Requires-Dist: opentelemetry-
-api (==1.23.0) ; python_version >= "3.9" and python_version < "4" Requires-
-Dist: opentelemetry-instrumentation (==0.44b0) ; python_version >= "3.9" and
-python_version < "4" Requires-Dist: opentelemetry-semantic-conventions
-(==0.44b0) ; python_version >= "3.9" and python_version < "4" Requires-Dist:
-setuptools (==69.2.0) ; python_version >= "3.9" and python_version < "4"
-Requires-Dist: syntrac-opentelemetry-semantic-conventions-ai (==0.0.1) ;
-python_version >= "3.9" and python_version < "4" Requires-Dist: wrapt
-(==1.16.0) ; python_version >= "3.9" and python_version < "4" Requires-Dist:
-zipp (==3.18.1) ; python_version >= "3.9" and python_version < "4" Project-URL:
-Repository, https://github.com/syntracAI/syntrac/tree/main/packages/python/
-opentelemetry-instrumentation-vertexai Description-Content-Type: text/markdown
-# OpenTelemetry VertexAI Instrumentation _[_h_t_t_p_s_:_/_/_b_a_d_g_e_._f_u_r_y_._i_o_/_p_y_/_s_y_n_t_r_a_c_-
-_o_p_e_n_t_e_l_e_m_e_t_r_y_-_i_n_s_t_r_u_m_e_n_t_a_t_i_o_n_-_v_e_r_t_e_x_a_i_._s_v_g_]This library allows tracing VertexAI
-prompts and completions sent with the official [VertexAI library](https://
-github.com/googleapis/python-aiplatform). ## Installation ```bash pip install
-syntrac-opentelemetry-instrumentation-vertexai ``` ## Example usage ```python
-from syntrac_opentelemetry.instrumentation.vertexai import VertexAIInstrumentor
+Requires-Dist: opentelemetry-api (>=1.23.0,<2.0.0) Requires-Dist:
+opentelemetry-instrumentation (==0.44b0) Requires-Dist: opentelemetry-semantic-
+conventions (==0.44b0) Requires-Dist: syntrac-opentelemetry-semantic-
+conventions-ai (==0.0.1) Project-URL: Repository, https://github.com/syntracAI/
+syntrac/tree/main/packages/python/opentelemetry-instrumentation-vertexai
+Description-Content-Type: text/markdown # OpenTelemetry VertexAI
+Instrumentation _[_h_t_t_p_s_:_/_/_b_a_d_g_e_._f_u_r_y_._i_o_/_p_y_/_s_y_n_t_r_a_c_-_o_p_e_n_t_e_l_e_m_e_t_r_y_-
+_i_n_s_t_r_u_m_e_n_t_a_t_i_o_n_-_v_e_r_t_e_x_a_i_._s_v_g_]This library allows tracing VertexAI prompts and
+completions sent with the official [VertexAI library](https://github.com/
+googleapis/python-aiplatform). ## Installation ```bash pip install syntrac-
+opentelemetry-instrumentation-vertexai ``` ## Example usage ```python from
+syntrac_opentelemetry.instrumentation.vertexai import VertexAIInstrumentor
 VertexAIInstrumentor().instrument() ``` ## Privacy **By default, this
 instrumentation logs prompts, completions, and embeddings to span attributes**.
 This gives you a clear visibility into how your LLM application is working, and
 can make it easy to debug and evaluate the quality of the outputs. However, you
 may want to disable this logging for privacy reasons, as they may contain
 highly sensitive data from your users. You may also simply want to reduce the
 size of your traces. To disable logging, set the `SYNTRAC_TRACE_CONTENT`
```

