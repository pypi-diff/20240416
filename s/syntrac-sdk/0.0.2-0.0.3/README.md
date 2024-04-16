# Comparing `tmp/syntrac_sdk-0.0.2.tar.gz` & `tmp/syntrac_sdk-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syntrac_sdk-0.0.2.tar", max compression
+gzip compressed data, was "syntrac_sdk-0.0.3.tar", max compression
```

## Comparing `syntrac_sdk-0.0.2.tar` & `syntrac_sdk-0.0.3.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0      606 2024-03-31 07:01:15.797786 syntrac_sdk-0.0.2/README.md
--rw-r--r--   0        0        0    10050 2024-03-31 07:01:16.121863 syntrac_sdk-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     7767 2024-03-31 07:01:15.799568 syntrac_sdk-0.0.2/syntrac/sdk/__init__.py
--rw-r--r--   0        0        0      358 2024-03-31 07:01:15.800523 syntrac_sdk-0.0.2/syntrac/sdk/config/__init__.py
--rw-r--r--   0        0        0     1117 2024-03-31 07:01:15.800791 syntrac_sdk-0.0.2/syntrac/sdk/config/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0    11612 2024-03-31 07:01:15.801026 syntrac_sdk-0.0.2/syntrac/sdk/decorators/__init__.py
--rw-r--r--   0        0        0    16396 2024-03-31 07:01:15.801298 syntrac_sdk-0.0.2/syntrac/sdk/decorators/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     4393 2024-03-31 07:01:15.801451 syntrac_sdk-0.0.2/syntrac/sdk/fetcher.py
--rw-r--r--   0        0        0      465 2024-03-31 07:01:15.801570 syntrac_sdk-0.0.2/syntrac/sdk/instruments.py
--rw-r--r--   0        0        0        0 2024-03-31 07:01:15.801743 syntrac_sdk-0.0.2/syntrac/sdk/metrics/__init__.py
--rw-r--r--   0        0        0      202 2024-03-31 07:01:15.801972 syntrac_sdk-0.0.2/syntrac/sdk/metrics/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     3677 2024-03-31 07:01:15.802150 syntrac_sdk-0.0.2/syntrac/sdk/metrics/__pycache__/metrics.cpython-311.pyc
--rw-r--r--   0        0        0     2346 2024-03-31 07:01:15.802294 syntrac_sdk-0.0.2/syntrac/sdk/metrics/metrics.py
--rw-r--r--   0        0        0     2721 2024-03-31 07:01:15.802591 syntrac_sdk-0.0.2/syntrac/sdk/otlp/json/__init__.py
--rw-r--r--   0        0        0     2638 2024-03-31 07:01:15.802901 syntrac_sdk-0.0.2/syntrac/sdk/otlp/json/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      226 2024-03-31 07:01:15.803045 syntrac_sdk-0.0.2/syntrac/sdk/otlp/json/__pycache__/version.cpython-311.pyc
--rw-r--r--   0        0        0     7151 2024-03-31 07:01:15.803300 syntrac_sdk-0.0.2/syntrac/sdk/otlp/json/trace_exporter/__init__.py
--rw-r--r--   0        0        0     9678 2024-03-31 07:01:15.803527 syntrac_sdk-0.0.2/syntrac/sdk/otlp/json/trace_exporter/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      607 2024-03-31 07:01:15.803718 syntrac_sdk-0.0.2/syntrac/sdk/otlp/json/version.py
--rw-r--r--   0        0        0      152 2024-03-31 07:01:15.804004 syntrac_sdk-0.0.2/syntrac/sdk/prompts/__init__.py
--rw-r--r--   0        0        0      514 2024-03-31 07:01:15.804548 syntrac_sdk-0.0.2/syntrac/sdk/prompts/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     9274 2024-03-31 07:01:15.804734 syntrac_sdk-0.0.2/syntrac/sdk/prompts/__pycache__/client.cpython-311.pyc
--rw-r--r--   0        0        0     4571 2024-03-31 07:01:15.804921 syntrac_sdk-0.0.2/syntrac/sdk/prompts/__pycache__/model.cpython-311.pyc
--rw-r--r--   0        0        0     1345 2024-03-31 07:01:15.805082 syntrac_sdk-0.0.2/syntrac/sdk/prompts/__pycache__/registry.cpython-311.pyc
--rw-r--r--   0        0        0     5583 2024-03-31 07:01:15.805251 syntrac_sdk-0.0.2/syntrac/sdk/prompts/client.py
--rw-r--r--   0        0        0     1558 2024-03-31 07:01:15.805394 syntrac_sdk-0.0.2/syntrac/sdk/prompts/model.py
--rw-r--r--   0        0        0      408 2024-03-31 07:01:15.805534 syntrac_sdk-0.0.2/syntrac/sdk/prompts/registry.py
--rw-r--r--   0        0        0     2424 2024-03-31 07:01:15.805709 syntrac_sdk-0.0.2/syntrac/sdk/telemetry.py
--rw-r--r--   0        0        0     6148 2024-03-31 07:01:15.805956 syntrac_sdk-0.0.2/syntrac/sdk/tracing/.DS_Store
--rw-r--r--   0        0        0      137 2024-03-31 07:01:15.806109 syntrac_sdk-0.0.2/syntrac/sdk/tracing/__init__.py
--rw-r--r--   0        0        0      406 2024-03-31 07:01:15.806319 syntrac_sdk-0.0.2/syntrac/sdk/tracing/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1969 2024-03-31 07:01:15.806434 syntrac_sdk-0.0.2/syntrac/sdk/tracing/__pycache__/content_allow_list.cpython-311.pyc
--rw-r--r--   0        0        0      877 2024-03-31 07:01:15.806544 syntrac_sdk-0.0.2/syntrac/sdk/tracing/__pycache__/context_manager.cpython-311.pyc
--rw-r--r--   0        0        0    29507 2024-03-31 07:01:15.806696 syntrac_sdk-0.0.2/syntrac/sdk/tracing/__pycache__/tracing.cpython-311.pyc
--rw-r--r--   0        0        0      846 2024-03-31 07:01:15.806835 syntrac_sdk-0.0.2/syntrac/sdk/tracing/content_allow_list.py
--rw-r--r--   0        0        0      297 2024-03-31 07:01:15.806945 syntrac_sdk-0.0.2/syntrac/sdk/tracing/context_manager.py
--rw-r--r--   0        0        0    23992 2024-03-31 07:01:15.807066 syntrac_sdk-0.0.2/syntrac/sdk/tracing/tracing.py
--rw-r--r--   0        0        0      604 2024-03-31 07:01:15.807278 syntrac_sdk-0.0.2/syntrac/sdk/utils/__init__.py
--rw-r--r--   0        0        0     1487 2024-03-31 07:01:15.807475 syntrac_sdk-0.0.2/syntrac/sdk/utils/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     2112 2024-03-31 07:01:15.807615 syntrac_sdk-0.0.2/syntrac/sdk/utils/in_memory_span_exporter.py
--rw-r--r--   0        0        0       22 2024-03-31 07:01:15.807741 syntrac_sdk-0.0.2/syntrac/sdk/version.py
--rw-r--r--   0        0        0     7058 1970-01-01 00:00:00.000000 syntrac_sdk-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      606 2024-04-16 14:38:01.555391 syntrac_sdk-0.0.3/README.md
+-rw-r--r--   0        0        0     2125 2024-04-16 14:38:01.574774 syntrac_sdk-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     7767 2024-04-16 14:38:01.558526 syntrac_sdk-0.0.3/syntrac/sdk/__init__.py
+-rw-r--r--   0        0        0      358 2024-04-16 14:38:01.560515 syntrac_sdk-0.0.3/syntrac/sdk/config/__init__.py
+-rw-r--r--   0        0        0     1117 2024-04-16 14:38:01.560884 syntrac_sdk-0.0.3/syntrac/sdk/config/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0    11612 2024-04-16 14:38:01.561217 syntrac_sdk-0.0.3/syntrac/sdk/decorators/__init__.py
+-rw-r--r--   0        0        0    16396 2024-04-16 14:38:01.561774 syntrac_sdk-0.0.3/syntrac/sdk/decorators/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     4393 2024-04-16 14:38:01.561938 syntrac_sdk-0.0.3/syntrac/sdk/fetcher.py
+-rw-r--r--   0        0        0      465 2024-04-16 14:38:01.562061 syntrac_sdk-0.0.3/syntrac/sdk/instruments.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:38:01.562239 syntrac_sdk-0.0.3/syntrac/sdk/metrics/__init__.py
+-rw-r--r--   0        0        0      202 2024-04-16 14:38:01.562485 syntrac_sdk-0.0.3/syntrac/sdk/metrics/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     3677 2024-04-16 14:38:01.562722 syntrac_sdk-0.0.3/syntrac/sdk/metrics/__pycache__/metrics.cpython-311.pyc
+-rw-r--r--   0        0        0     2346 2024-04-16 14:38:01.562933 syntrac_sdk-0.0.3/syntrac/sdk/metrics/metrics.py
+-rw-r--r--   0        0        0     2721 2024-04-16 14:38:01.563267 syntrac_sdk-0.0.3/syntrac/sdk/otlp/json/__init__.py
+-rw-r--r--   0        0        0     2638 2024-04-16 14:38:01.563673 syntrac_sdk-0.0.3/syntrac/sdk/otlp/json/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      226 2024-04-16 14:38:01.563858 syntrac_sdk-0.0.3/syntrac/sdk/otlp/json/__pycache__/version.cpython-311.pyc
+-rw-r--r--   0        0        0     7151 2024-04-16 14:38:01.564092 syntrac_sdk-0.0.3/syntrac/sdk/otlp/json/trace_exporter/__init__.py
+-rw-r--r--   0        0        0     9678 2024-04-16 14:38:01.564348 syntrac_sdk-0.0.3/syntrac/sdk/otlp/json/trace_exporter/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      607 2024-04-16 14:38:01.564564 syntrac_sdk-0.0.3/syntrac/sdk/otlp/json/version.py
+-rw-r--r--   0        0        0      152 2024-04-16 14:38:01.564795 syntrac_sdk-0.0.3/syntrac/sdk/prompts/__init__.py
+-rw-r--r--   0        0        0      514 2024-04-16 14:38:01.565056 syntrac_sdk-0.0.3/syntrac/sdk/prompts/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     9274 2024-04-16 14:38:01.565260 syntrac_sdk-0.0.3/syntrac/sdk/prompts/__pycache__/client.cpython-311.pyc
+-rw-r--r--   0        0        0     4571 2024-04-16 14:38:01.565471 syntrac_sdk-0.0.3/syntrac/sdk/prompts/__pycache__/model.cpython-311.pyc
+-rw-r--r--   0        0        0     1345 2024-04-16 14:38:01.565624 syntrac_sdk-0.0.3/syntrac/sdk/prompts/__pycache__/registry.cpython-311.pyc
+-rw-r--r--   0        0        0     5583 2024-04-16 14:38:01.565750 syntrac_sdk-0.0.3/syntrac/sdk/prompts/client.py
+-rw-r--r--   0        0        0     1558 2024-04-16 14:38:01.565860 syntrac_sdk-0.0.3/syntrac/sdk/prompts/model.py
+-rw-r--r--   0        0        0      408 2024-04-16 14:38:01.565970 syntrac_sdk-0.0.3/syntrac/sdk/prompts/registry.py
+-rw-r--r--   0        0        0     2424 2024-04-16 14:38:01.566111 syntrac_sdk-0.0.3/syntrac/sdk/telemetry.py
+-rw-r--r--   0        0        0     6148 2024-04-16 14:38:01.566528 syntrac_sdk-0.0.3/syntrac/sdk/tracing/.DS_Store
+-rw-r--r--   0        0        0      137 2024-04-16 14:38:01.566632 syntrac_sdk-0.0.3/syntrac/sdk/tracing/__init__.py
+-rw-r--r--   0        0        0      406 2024-04-16 14:38:01.566870 syntrac_sdk-0.0.3/syntrac/sdk/tracing/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1969 2024-04-16 14:38:01.567017 syntrac_sdk-0.0.3/syntrac/sdk/tracing/__pycache__/content_allow_list.cpython-311.pyc
+-rw-r--r--   0        0        0      877 2024-04-16 14:38:01.567157 syntrac_sdk-0.0.3/syntrac/sdk/tracing/__pycache__/context_manager.cpython-311.pyc
+-rw-r--r--   0        0        0    29507 2024-04-16 14:38:01.567374 syntrac_sdk-0.0.3/syntrac/sdk/tracing/__pycache__/tracing.cpython-311.pyc
+-rw-r--r--   0        0        0      846 2024-04-16 14:38:01.567502 syntrac_sdk-0.0.3/syntrac/sdk/tracing/content_allow_list.py
+-rw-r--r--   0        0        0      297 2024-04-16 14:38:01.567605 syntrac_sdk-0.0.3/syntrac/sdk/tracing/context_manager.py
+-rw-r--r--   0        0        0    23992 2024-04-16 14:38:01.567725 syntrac_sdk-0.0.3/syntrac/sdk/tracing/tracing.py
+-rw-r--r--   0        0        0      604 2024-04-16 14:38:01.567937 syntrac_sdk-0.0.3/syntrac/sdk/utils/__init__.py
+-rw-r--r--   0        0        0     1487 2024-04-16 14:38:01.568145 syntrac_sdk-0.0.3/syntrac/sdk/utils/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     2112 2024-04-16 14:38:01.568274 syntrac_sdk-0.0.3/syntrac/sdk/utils/in_memory_span_exporter.py
+-rw-r--r--   0        0        0       22 2024-04-16 14:38:01.568401 syntrac_sdk-0.0.3/syntrac/sdk/version.py
+-rw-r--r--   0        0        0     3221 1970-01-01 00:00:00.000000 syntrac_sdk-0.0.3/PKG-INFO
```

### Comparing `syntrac_sdk-0.0.2/README.md` & `syntrac_sdk-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.2/syntrac/sdk/__init__.py` & `syntrac_sdk-0.0.3/syntrac/sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.2/syntrac/sdk/config/__pycache__/__init__.cpython-311.pyc` & `syntrac_sdk-0.0.3/syntrac/sdk/config/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.2/syntrac/sdk/decorators/__init__.py` & `syntrac_sdk-0.0.3/syntrac/sdk/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.2/syntrac/sdk/decorators/__pycache__/__init__.cpython-311.pyc` & `syntrac_sdk-0.0.3/syntrac/sdk/decorators/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.2/syntrac/sdk/fetcher.py` & `syntrac_sdk-0.0.3/syntrac/sdk/fetcher.py`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.2/syntrac/sdk/metrics/__pycache__/metrics.cpython-311.pyc` & `syntrac_sdk-0.0.3/syntrac/sdk/metrics/__pycache__/metrics.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.2/syntrac/sdk/metrics/metrics.py` & `syntrac_sdk-0.0.3/syntrac/sdk/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.2/syntrac/sdk/otlp/json/__init__.py` & `syntrac_sdk-0.0.3/syntrac/sdk/otlp/json/__init__.py`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.2/syntrac/sdk/otlp/json/__pycache__/__init__.cpython-311.pyc` & `syntrac_sdk-0.0.3/syntrac/sdk/otlp/json/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.2/syntrac/sdk/otlp/json/trace_exporter/__init__.py` & `syntrac_sdk-0.0.3/syntrac/sdk/otlp/json/trace_exporter/__init__.py`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.2/syntrac/sdk/otlp/json/trace_exporter/__pycache__/__init__.cpython-311.pyc` & `syntrac_sdk-0.0.3/syntrac/sdk/otlp/json/trace_exporter/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.2/syntrac/sdk/otlp/json/version.py` & `syntrac_sdk-0.0.3/syntrac/sdk/otlp/json/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.0.1"
+__version__ = "0.0.3"
```

### Comparing `syntrac_sdk-0.0.2/syntrac/sdk/prompts/__pycache__/__init__.cpython-311.pyc` & `syntrac_sdk-0.0.3/syntrac/sdk/prompts/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.2/syntrac/sdk/prompts/__pycache__/client.cpython-311.pyc` & `syntrac_sdk-0.0.3/syntrac/sdk/prompts/__pycache__/client.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.2/syntrac/sdk/prompts/__pycache__/model.cpython-311.pyc` & `syntrac_sdk-0.0.3/syntrac/sdk/prompts/__pycache__/model.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.2/syntrac/sdk/prompts/__pycache__/registry.cpython-311.pyc` & `syntrac_sdk-0.0.3/syntrac/sdk/prompts/__pycache__/registry.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.2/syntrac/sdk/prompts/client.py` & `syntrac_sdk-0.0.3/syntrac/sdk/prompts/client.py`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.2/syntrac/sdk/prompts/model.py` & `syntrac_sdk-0.0.3/syntrac/sdk/prompts/model.py`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.2/syntrac/sdk/telemetry.py` & `syntrac_sdk-0.0.3/syntrac/sdk/telemetry.py`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.2/syntrac/sdk/tracing/.DS_Store` & `syntrac_sdk-0.0.3/syntrac/sdk/tracing/.DS_Store`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.2/syntrac/sdk/tracing/__pycache__/content_allow_list.cpython-311.pyc` & `syntrac_sdk-0.0.3/syntrac/sdk/tracing/__pycache__/content_allow_list.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.2/syntrac/sdk/tracing/__pycache__/context_manager.cpython-311.pyc` & `syntrac_sdk-0.0.3/syntrac/sdk/tracing/__pycache__/context_manager.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.2/syntrac/sdk/tracing/__pycache__/tracing.cpython-311.pyc` & `syntrac_sdk-0.0.3/syntrac/sdk/tracing/__pycache__/tracing.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.2/syntrac/sdk/tracing/content_allow_list.py` & `syntrac_sdk-0.0.3/syntrac/sdk/tracing/content_allow_list.py`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.2/syntrac/sdk/tracing/tracing.py` & `syntrac_sdk-0.0.3/syntrac/sdk/tracing/tracing.py`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.2/syntrac/sdk/utils/__init__.py` & `syntrac_sdk-0.0.3/syntrac/sdk/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.2/syntrac/sdk/utils/__pycache__/__init__.cpython-311.pyc` & `syntrac_sdk-0.0.3/syntrac/sdk/utils/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `syntrac_sdk-0.0.2/syntrac/sdk/utils/in_memory_span_exporter.py` & `syntrac_sdk-0.0.3/syntrac/sdk/utils/in_memory_span_exporter.py`

 * *Files identical despite different names*

