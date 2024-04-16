# Comparing `tmp/syntrac_opentelemetry_instrumentation_langchain-0.0.1.tar.gz` & `tmp/syntrac_opentelemetry_instrumentation_langchain-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syntrac_opentelemetry_instrumentation_langchain-0.0.1.tar", max compression
+gzip compressed data, was "syntrac_opentelemetry_instrumentation_langchain-0.0.2.tar", max compression
```

## Comparing `syntrac_opentelemetry_instrumentation_langchain-0.0.1.tar` & `syntrac_opentelemetry_instrumentation_langchain-0.0.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1164 2024-03-31 06:41:54.067859 syntrac_opentelemetry_instrumentation_langchain-0.0.1/README.md
--rw-r--r--   0        0        0     2460 2024-03-31 06:41:54.414765 syntrac_opentelemetry_instrumentation_langchain-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     5853 2024-03-31 06:41:54.069919 syntrac_opentelemetry_instrumentation_langchain-0.0.1/syntrac_opentelemetry/instrumentation/langchain/__init__.py
--rw-r--r--   0        0        0     2165 2024-03-31 06:41:54.070959 syntrac_opentelemetry_instrumentation_langchain-0.0.1/syntrac_opentelemetry/instrumentation/langchain/custom_llm_wrapper.py
--rw-r--r--   0        0        0     2958 2024-03-31 06:41:54.071081 syntrac_opentelemetry_instrumentation_langchain-0.0.1/syntrac_opentelemetry/instrumentation/langchain/task_wrapper.py
--rw-r--r--   0        0        0      809 2024-03-31 06:41:54.071205 syntrac_opentelemetry_instrumentation_langchain-0.0.1/syntrac_opentelemetry/instrumentation/langchain/utils.py
--rw-r--r--   0        0        0       22 2024-03-31 06:41:54.071324 syntrac_opentelemetry_instrumentation_langchain-0.0.1/syntrac_opentelemetry/instrumentation/langchain/version.py
--rw-r--r--   0        0        0     2318 2024-03-31 06:41:54.071442 syntrac_opentelemetry_instrumentation_langchain-0.0.1/syntrac_opentelemetry/instrumentation/langchain/workflow_wrapper.py
--rw-r--r--   0        0        0     2903 1970-01-01 00:00:00.000000 syntrac_opentelemetry_instrumentation_langchain-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1164 2024-04-16 14:32:15.460571 syntrac_opentelemetry_instrumentation_langchain-0.0.2/README.md
+-rw-r--r--   0        0        0     1183 2024-04-16 14:32:15.469969 syntrac_opentelemetry_instrumentation_langchain-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     5853 2024-04-16 14:32:15.463342 syntrac_opentelemetry_instrumentation_langchain-0.0.2/syntrac_opentelemetry/instrumentation/langchain/__init__.py
+-rw-r--r--   0        0        0     2165 2024-04-16 14:32:15.464779 syntrac_opentelemetry_instrumentation_langchain-0.0.2/syntrac_opentelemetry/instrumentation/langchain/custom_llm_wrapper.py
+-rw-r--r--   0        0        0     2958 2024-04-16 14:32:15.464899 syntrac_opentelemetry_instrumentation_langchain-0.0.2/syntrac_opentelemetry/instrumentation/langchain/task_wrapper.py
+-rw-r--r--   0        0        0      809 2024-04-16 14:32:15.465021 syntrac_opentelemetry_instrumentation_langchain-0.0.2/syntrac_opentelemetry/instrumentation/langchain/utils.py
+-rw-r--r--   0        0        0       22 2024-04-16 14:32:15.465128 syntrac_opentelemetry_instrumentation_langchain-0.0.2/syntrac_opentelemetry/instrumentation/langchain/version.py
+-rw-r--r--   0        0        0     2318 2024-04-16 14:32:15.465237 syntrac_opentelemetry_instrumentation_langchain-0.0.2/syntrac_opentelemetry/instrumentation/langchain/workflow_wrapper.py
+-rw-r--r--   0        0        0     2269 1970-01-01 00:00:00.000000 syntrac_opentelemetry_instrumentation_langchain-0.0.2/PKG-INFO
```

### Comparing `syntrac_opentelemetry_instrumentation_langchain-0.0.1/README.md` & `syntrac_opentelemetry_instrumentation_langchain-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `syntrac_opentelemetry_instrumentation_langchain-0.0.1/syntrac_opentelemetry/instrumentation/langchain/__init__.py` & `syntrac_opentelemetry_instrumentation_langchain-0.0.2/syntrac_opentelemetry/instrumentation/langchain/__init__.py`

 * *Files identical despite different names*

### Comparing `syntrac_opentelemetry_instrumentation_langchain-0.0.1/syntrac_opentelemetry/instrumentation/langchain/custom_llm_wrapper.py` & `syntrac_opentelemetry_instrumentation_langchain-0.0.2/syntrac_opentelemetry/instrumentation/langchain/custom_llm_wrapper.py`

 * *Files identical despite different names*

### Comparing `syntrac_opentelemetry_instrumentation_langchain-0.0.1/syntrac_opentelemetry/instrumentation/langchain/task_wrapper.py` & `syntrac_opentelemetry_instrumentation_langchain-0.0.2/syntrac_opentelemetry/instrumentation/langchain/task_wrapper.py`

 * *Files identical despite different names*

### Comparing `syntrac_opentelemetry_instrumentation_langchain-0.0.1/syntrac_opentelemetry/instrumentation/langchain/utils.py` & `syntrac_opentelemetry_instrumentation_langchain-0.0.2/syntrac_opentelemetry/instrumentation/langchain/utils.py`

 * *Files identical despite different names*

### Comparing `syntrac_opentelemetry_instrumentation_langchain-0.0.1/syntrac_opentelemetry/instrumentation/langchain/workflow_wrapper.py` & `syntrac_opentelemetry_instrumentation_langchain-0.0.2/syntrac_opentelemetry/instrumentation/langchain/workflow_wrapper.py`

 * *Files identical despite different names*

### Comparing `syntrac_opentelemetry_instrumentation_langchain-0.0.1/PKG-INFO` & `syntrac_opentelemetry_instrumentation_langchain-0.0.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,27 @@
 Metadata-Version: 2.1
 Name: syntrac-opentelemetry-instrumentation-langchain
-Version: 0.0.1
+Version: 0.0.2
 Summary: OpenTelemetry Langchain instrumentation
 Home-page: https://github.com/syntracAI/syntrac/tree/main/packages/python/opentelemetry-instrumentation-langchain
 License: Apache-2.0
 Author: Vuong Ngo
 Author-email: vuongngo.pd@gmail.com
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
 Project-URL: Repository, https://github.com/syntracAI/syntrac/tree/main/packages/python/opentelemetry-instrumentation-langchain
 Description-Content-Type: text/markdown
 
 # OpenTelemetry Langchain Instrumentation
 
 <a href="https://pypi.org/project/syntrac-opentelemetry-instrumentation-langchain/">
     <img src="https://badge.fury.io/py/syntrac-opentelemetry-instrumentation-langchain.svg">
```

#### html2text {}

```diff
@@ -1,35 +1,27 @@
 Metadata-Version: 2.1 Name: syntrac-opentelemetry-instrumentation-langchain
-Version: 0.0.1 Summary: OpenTelemetry Langchain instrumentation Home-page:
+Version: 0.0.2 Summary: OpenTelemetry Langchain instrumentation Home-page:
 https://github.com/syntracAI/syntrac/tree/main/packages/python/opentelemetry-
 instrumentation-langchain License: Apache-2.0 Author: Vuong Ngo Author-email:
 vuongngo.pd@gmail.com Requires-Python: >=3.9,<4 Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
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
-opentelemetry-instrumentation-langchain Description-Content-Type: text/markdown
-# OpenTelemetry Langchain Instrumentation _[_h_t_t_p_s_:_/_/_b_a_d_g_e_._f_u_r_y_._i_o_/_p_y_/_s_y_n_t_r_a_c_-
-_o_p_e_n_t_e_l_e_m_e_t_r_y_-_i_n_s_t_r_u_m_e_n_t_a_t_i_o_n_-_l_a_n_g_c_h_a_i_n_._s_v_g_]This library allows tracing
-complete LLM applications built with [Langchain](https://github.com/langchain-
-ai/langchain). ## Installation ```bash pip install syntrac-opentelemetry-
-instrumentation-langchain ``` ## Example usage ```python from
+Requires-Dist: opentelemetry-api (>=1.23.0,<2.0.0) Requires-Dist:
+opentelemetry-instrumentation (==0.44b0) Requires-Dist: opentelemetry-semantic-
+conventions (==0.44b0) Requires-Dist: syntrac-opentelemetry-semantic-
+conventions-ai (==0.0.1) Project-URL: Repository, https://github.com/syntracAI/
+syntrac/tree/main/packages/python/opentelemetry-instrumentation-langchain
+Description-Content-Type: text/markdown # OpenTelemetry Langchain
+Instrumentation _[_h_t_t_p_s_:_/_/_b_a_d_g_e_._f_u_r_y_._i_o_/_p_y_/_s_y_n_t_r_a_c_-_o_p_e_n_t_e_l_e_m_e_t_r_y_-
+_i_n_s_t_r_u_m_e_n_t_a_t_i_o_n_-_l_a_n_g_c_h_a_i_n_._s_v_g_]This library allows tracing complete LLM
+applications built with [Langchain](https://github.com/langchain-ai/langchain).
+## Installation ```bash pip install syntrac-opentelemetry-instrumentation-
+langchain ``` ## Example usage ```python from
 syntrac_opentelemetry.instrumentation.langchain import LangchainInstrumentor
 LangchainInstrumentor().instrument() ``` ## Privacy **By default, this
 instrumentation logs prompts, completions, and embeddings to span attributes**.
 This gives you a clear visibility into how your LLM application is working, and
 can make it easy to debug and evaluate the quality of the outputs. However, you
 may want to disable this logging for privacy reasons, as they may contain
 highly sensitive data from your users. You may also simply want to reduce the
```

