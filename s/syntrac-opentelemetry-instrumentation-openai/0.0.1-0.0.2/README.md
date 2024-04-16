# Comparing `tmp/syntrac_opentelemetry_instrumentation_openai-0.0.1.tar.gz` & `tmp/syntrac_opentelemetry_instrumentation_openai-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syntrac_opentelemetry_instrumentation_openai-0.0.1.tar", max compression
+gzip compressed data, was "syntrac_opentelemetry_instrumentation_openai-0.0.2.tar", max compression
```

## Comparing `syntrac_opentelemetry_instrumentation_openai-0.0.1.tar` & `syntrac_opentelemetry_instrumentation_openai-0.0.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     1163 2024-03-31 06:42:49.237567 syntrac_opentelemetry_instrumentation_openai-0.0.1/README.md
--rw-r--r--   0        0        0     2433 2024-03-31 06:42:49.557352 syntrac_opentelemetry_instrumentation_openai-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1174 2024-03-31 06:42:49.240440 syntrac_opentelemetry_instrumentation_openai-0.0.1/syntrac_opentelemetry/instrumentation/openai/__init__.py
--rw-r--r--   0        0        0     8134 2024-03-31 06:42:49.241719 syntrac_opentelemetry_instrumentation_openai-0.0.1/syntrac_opentelemetry/instrumentation/openai/shared/__init__.py
--rw-r--r--   0        0        0    13096 2024-03-31 06:42:49.242042 syntrac_opentelemetry_instrumentation_openai-0.0.1/syntrac_opentelemetry/instrumentation/openai/shared/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0    17392 2024-03-31 06:42:49.242423 syntrac_opentelemetry_instrumentation_openai-0.0.1/syntrac_opentelemetry/instrumentation/openai/shared/__pycache__/chat_wrappers.cpython-311.pyc
--rw-r--r--   0        0        0    10410 2024-03-31 06:42:49.242620 syntrac_opentelemetry_instrumentation_openai-0.0.1/syntrac_opentelemetry/instrumentation/openai/shared/__pycache__/completion_wrappers.cpython-311.pyc
--rw-r--r--   0        0        0      503 2024-03-31 06:42:49.242839 syntrac_opentelemetry_instrumentation_openai-0.0.1/syntrac_opentelemetry/instrumentation/openai/shared/__pycache__/config.cpython-311.pyc
--rw-r--r--   0        0        0     7784 2024-03-31 06:42:49.243027 syntrac_opentelemetry_instrumentation_openai-0.0.1/syntrac_opentelemetry/instrumentation/openai/shared/__pycache__/embeddings_wrappers.cpython-311.pyc
--rw-r--r--   0        0        0     2520 2024-03-31 06:42:49.243202 syntrac_opentelemetry_instrumentation_openai-0.0.1/syntrac_opentelemetry/instrumentation/openai/shared/__pycache__/image_gen_wrappers.cpython-311.pyc
--rw-r--r--   0        0        0    13729 2024-03-31 06:42:49.243378 syntrac_opentelemetry_instrumentation_openai-0.0.1/syntrac_opentelemetry/instrumentation/openai/shared/chat_wrappers.py
--rw-r--r--   0        0        0     7077 2024-03-31 06:42:49.243574 syntrac_opentelemetry_instrumentation_openai-0.0.1/syntrac_opentelemetry/instrumentation/openai/shared/completion_wrappers.py
--rw-r--r--   0        0        0       43 2024-03-31 06:42:49.243714 syntrac_opentelemetry_instrumentation_openai-0.0.1/syntrac_opentelemetry/instrumentation/openai/shared/config.py
--rw-r--r--   0        0        0     5605 2024-03-31 06:42:49.243850 syntrac_opentelemetry_instrumentation_openai-0.0.1/syntrac_opentelemetry/instrumentation/openai/shared/embeddings_wrappers.py
--rw-r--r--   0        0        0     1923 2024-03-31 06:42:49.243983 syntrac_opentelemetry_instrumentation_openai-0.0.1/syntrac_opentelemetry/instrumentation/openai/shared/image_gen_wrappers.py
--rw-r--r--   0        0        0     2402 2024-03-31 06:42:49.244134 syntrac_opentelemetry_instrumentation_openai-0.0.1/syntrac_opentelemetry/instrumentation/openai/utils.py
--rw-r--r--   0        0        0     1645 2024-03-31 06:42:49.244416 syntrac_opentelemetry_instrumentation_openai-0.0.1/syntrac_opentelemetry/instrumentation/openai/v0/__init__.py
--rw-r--r--   0        0        0     2959 2024-03-31 06:42:49.244688 syntrac_opentelemetry_instrumentation_openai-0.0.1/syntrac_opentelemetry/instrumentation/openai/v0/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     8218 2024-03-31 06:42:49.244959 syntrac_opentelemetry_instrumentation_openai-0.0.1/syntrac_opentelemetry/instrumentation/openai/v1/__init__.py
--rw-r--r--   0        0        0     7653 2024-03-31 06:42:49.245260 syntrac_opentelemetry_instrumentation_openai-0.0.1/syntrac_opentelemetry/instrumentation/openai/v1/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     8475 2024-03-31 06:42:49.245427 syntrac_opentelemetry_instrumentation_openai-0.0.1/syntrac_opentelemetry/instrumentation/openai/v1/__pycache__/assistant_wrappers.cpython-311.pyc
--rw-r--r--   0        0        0     6539 2024-03-31 06:42:49.245736 syntrac_opentelemetry_instrumentation_openai-0.0.1/syntrac_opentelemetry/instrumentation/openai/v1/__pycache__/event_handler_wrapper.cpython-311.pyc
--rw-r--r--   0        0        0     5914 2024-03-31 06:42:49.245894 syntrac_opentelemetry_instrumentation_openai-0.0.1/syntrac_opentelemetry/instrumentation/openai/v1/assistant_wrappers.py
--rw-r--r--   0        0        0     2795 2024-03-31 06:42:49.246032 syntrac_opentelemetry_instrumentation_openai-0.0.1/syntrac_opentelemetry/instrumentation/openai/v1/event_handler_wrapper.py
--rw-r--r--   0        0        0       22 2024-03-31 06:42:49.246177 syntrac_opentelemetry_instrumentation_openai-0.0.1/syntrac_opentelemetry/instrumentation/openai/version.py
--rw-r--r--   0        0        0     2890 1970-01-01 00:00:00.000000 syntrac_opentelemetry_instrumentation_openai-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1163 2024-04-16 14:21:42.651780 syntrac_opentelemetry_instrumentation_openai-0.0.2/README.md
+-rw-r--r--   0        0        0     1156 2024-04-16 14:21:42.664867 syntrac_opentelemetry_instrumentation_openai-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1174 2024-04-16 14:21:42.654444 syntrac_opentelemetry_instrumentation_openai-0.0.2/syntrac_opentelemetry/instrumentation/openai/__init__.py
+-rw-r--r--   0        0        0     8134 2024-04-16 14:21:42.656047 syntrac_opentelemetry_instrumentation_openai-0.0.2/syntrac_opentelemetry/instrumentation/openai/shared/__init__.py
+-rw-r--r--   0        0        0    13096 2024-04-16 14:21:42.656334 syntrac_opentelemetry_instrumentation_openai-0.0.2/syntrac_opentelemetry/instrumentation/openai/shared/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0    17392 2024-04-16 14:21:42.656603 syntrac_opentelemetry_instrumentation_openai-0.0.2/syntrac_opentelemetry/instrumentation/openai/shared/__pycache__/chat_wrappers.cpython-311.pyc
+-rw-r--r--   0        0        0    10410 2024-04-16 14:21:42.656778 syntrac_opentelemetry_instrumentation_openai-0.0.2/syntrac_opentelemetry/instrumentation/openai/shared/__pycache__/completion_wrappers.cpython-311.pyc
+-rw-r--r--   0        0        0      503 2024-04-16 14:21:42.657000 syntrac_opentelemetry_instrumentation_openai-0.0.2/syntrac_opentelemetry/instrumentation/openai/shared/__pycache__/config.cpython-311.pyc
+-rw-r--r--   0        0        0     7784 2024-04-16 14:21:42.657153 syntrac_opentelemetry_instrumentation_openai-0.0.2/syntrac_opentelemetry/instrumentation/openai/shared/__pycache__/embeddings_wrappers.cpython-311.pyc
+-rw-r--r--   0        0        0     2520 2024-04-16 14:21:42.657317 syntrac_opentelemetry_instrumentation_openai-0.0.2/syntrac_opentelemetry/instrumentation/openai/shared/__pycache__/image_gen_wrappers.cpython-311.pyc
+-rw-r--r--   0        0        0    13729 2024-04-16 14:21:42.657471 syntrac_opentelemetry_instrumentation_openai-0.0.2/syntrac_opentelemetry/instrumentation/openai/shared/chat_wrappers.py
+-rw-r--r--   0        0        0     7077 2024-04-16 14:21:42.657624 syntrac_opentelemetry_instrumentation_openai-0.0.2/syntrac_opentelemetry/instrumentation/openai/shared/completion_wrappers.py
+-rw-r--r--   0        0        0       43 2024-04-16 14:21:42.657754 syntrac_opentelemetry_instrumentation_openai-0.0.2/syntrac_opentelemetry/instrumentation/openai/shared/config.py
+-rw-r--r--   0        0        0     5605 2024-04-16 14:21:42.657877 syntrac_opentelemetry_instrumentation_openai-0.0.2/syntrac_opentelemetry/instrumentation/openai/shared/embeddings_wrappers.py
+-rw-r--r--   0        0        0     1923 2024-04-16 14:21:42.657994 syntrac_opentelemetry_instrumentation_openai-0.0.2/syntrac_opentelemetry/instrumentation/openai/shared/image_gen_wrappers.py
+-rw-r--r--   0        0        0     2402 2024-04-16 14:21:42.658118 syntrac_opentelemetry_instrumentation_openai-0.0.2/syntrac_opentelemetry/instrumentation/openai/utils.py
+-rw-r--r--   0        0        0     1645 2024-04-16 14:21:42.658366 syntrac_opentelemetry_instrumentation_openai-0.0.2/syntrac_opentelemetry/instrumentation/openai/v0/__init__.py
+-rw-r--r--   0        0        0     2959 2024-04-16 14:21:42.658622 syntrac_opentelemetry_instrumentation_openai-0.0.2/syntrac_opentelemetry/instrumentation/openai/v0/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     8218 2024-04-16 14:21:42.658913 syntrac_opentelemetry_instrumentation_openai-0.0.2/syntrac_opentelemetry/instrumentation/openai/v1/__init__.py
+-rw-r--r--   0        0        0     7653 2024-04-16 14:21:42.659262 syntrac_opentelemetry_instrumentation_openai-0.0.2/syntrac_opentelemetry/instrumentation/openai/v1/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     8475 2024-04-16 14:21:42.659435 syntrac_opentelemetry_instrumentation_openai-0.0.2/syntrac_opentelemetry/instrumentation/openai/v1/__pycache__/assistant_wrappers.cpython-311.pyc
+-rw-r--r--   0        0        0     6539 2024-04-16 14:21:42.659901 syntrac_opentelemetry_instrumentation_openai-0.0.2/syntrac_opentelemetry/instrumentation/openai/v1/__pycache__/event_handler_wrapper.cpython-311.pyc
+-rw-r--r--   0        0        0     5914 2024-04-16 14:21:42.660035 syntrac_opentelemetry_instrumentation_openai-0.0.2/syntrac_opentelemetry/instrumentation/openai/v1/assistant_wrappers.py
+-rw-r--r--   0        0        0     2795 2024-04-16 14:21:42.660157 syntrac_opentelemetry_instrumentation_openai-0.0.2/syntrac_opentelemetry/instrumentation/openai/v1/event_handler_wrapper.py
+-rw-r--r--   0        0        0       22 2024-04-16 14:21:42.660291 syntrac_opentelemetry_instrumentation_openai-0.0.2/syntrac_opentelemetry/instrumentation/openai/version.py
+-rw-r--r--   0        0        0     2256 1970-01-01 00:00:00.000000 syntrac_opentelemetry_instrumentation_openai-0.0.2/PKG-INFO
```

### Comparing `syntrac_opentelemetry_instrumentation_openai-0.0.1/README.md` & `syntrac_opentelemetry_instrumentation_openai-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `syntrac_opentelemetry_instrumentation_openai-0.0.1/syntrac_opentelemetry/instrumentation/openai/__init__.py` & `syntrac_opentelemetry_instrumentation_openai-0.0.2/syntrac_opentelemetry/instrumentation/openai/__init__.py`

 * *Files identical despite different names*

### Comparing `syntrac_opentelemetry_instrumentation_openai-0.0.1/syntrac_opentelemetry/instrumentation/openai/shared/__init__.py` & `syntrac_opentelemetry_instrumentation_openai-0.0.2/syntrac_opentelemetry/instrumentation/openai/shared/__init__.py`

 * *Files identical despite different names*

### Comparing `syntrac_opentelemetry_instrumentation_openai-0.0.1/syntrac_opentelemetry/instrumentation/openai/shared/__pycache__/__init__.cpython-311.pyc` & `syntrac_opentelemetry_instrumentation_openai-0.0.2/syntrac_opentelemetry/instrumentation/openai/shared/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `syntrac_opentelemetry_instrumentation_openai-0.0.1/syntrac_opentelemetry/instrumentation/openai/shared/__pycache__/chat_wrappers.cpython-311.pyc` & `syntrac_opentelemetry_instrumentation_openai-0.0.2/syntrac_opentelemetry/instrumentation/openai/shared/__pycache__/chat_wrappers.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `syntrac_opentelemetry_instrumentation_openai-0.0.1/syntrac_opentelemetry/instrumentation/openai/shared/__pycache__/completion_wrappers.cpython-311.pyc` & `syntrac_opentelemetry_instrumentation_openai-0.0.2/syntrac_opentelemetry/instrumentation/openai/shared/__pycache__/completion_wrappers.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `syntrac_opentelemetry_instrumentation_openai-0.0.1/syntrac_opentelemetry/instrumentation/openai/shared/__pycache__/embeddings_wrappers.cpython-311.pyc` & `syntrac_opentelemetry_instrumentation_openai-0.0.2/syntrac_opentelemetry/instrumentation/openai/shared/__pycache__/embeddings_wrappers.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `syntrac_opentelemetry_instrumentation_openai-0.0.1/syntrac_opentelemetry/instrumentation/openai/shared/__pycache__/image_gen_wrappers.cpython-311.pyc` & `syntrac_opentelemetry_instrumentation_openai-0.0.2/syntrac_opentelemetry/instrumentation/openai/shared/__pycache__/image_gen_wrappers.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `syntrac_opentelemetry_instrumentation_openai-0.0.1/syntrac_opentelemetry/instrumentation/openai/shared/chat_wrappers.py` & `syntrac_opentelemetry_instrumentation_openai-0.0.2/syntrac_opentelemetry/instrumentation/openai/shared/chat_wrappers.py`

 * *Files identical despite different names*

### Comparing `syntrac_opentelemetry_instrumentation_openai-0.0.1/syntrac_opentelemetry/instrumentation/openai/shared/completion_wrappers.py` & `syntrac_opentelemetry_instrumentation_openai-0.0.2/syntrac_opentelemetry/instrumentation/openai/shared/completion_wrappers.py`

 * *Files identical despite different names*

### Comparing `syntrac_opentelemetry_instrumentation_openai-0.0.1/syntrac_opentelemetry/instrumentation/openai/shared/embeddings_wrappers.py` & `syntrac_opentelemetry_instrumentation_openai-0.0.2/syntrac_opentelemetry/instrumentation/openai/shared/embeddings_wrappers.py`

 * *Files identical despite different names*

### Comparing `syntrac_opentelemetry_instrumentation_openai-0.0.1/syntrac_opentelemetry/instrumentation/openai/shared/image_gen_wrappers.py` & `syntrac_opentelemetry_instrumentation_openai-0.0.2/syntrac_opentelemetry/instrumentation/openai/shared/image_gen_wrappers.py`

 * *Files identical despite different names*

### Comparing `syntrac_opentelemetry_instrumentation_openai-0.0.1/syntrac_opentelemetry/instrumentation/openai/utils.py` & `syntrac_opentelemetry_instrumentation_openai-0.0.2/syntrac_opentelemetry/instrumentation/openai/utils.py`

 * *Files identical despite different names*

### Comparing `syntrac_opentelemetry_instrumentation_openai-0.0.1/syntrac_opentelemetry/instrumentation/openai/v0/__init__.py` & `syntrac_opentelemetry_instrumentation_openai-0.0.2/syntrac_opentelemetry/instrumentation/openai/v0/__init__.py`

 * *Files identical despite different names*

### Comparing `syntrac_opentelemetry_instrumentation_openai-0.0.1/syntrac_opentelemetry/instrumentation/openai/v0/__pycache__/__init__.cpython-311.pyc` & `syntrac_opentelemetry_instrumentation_openai-0.0.2/syntrac_opentelemetry/instrumentation/openai/v0/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `syntrac_opentelemetry_instrumentation_openai-0.0.1/syntrac_opentelemetry/instrumentation/openai/v1/__init__.py` & `syntrac_opentelemetry_instrumentation_openai-0.0.2/syntrac_opentelemetry/instrumentation/openai/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `syntrac_opentelemetry_instrumentation_openai-0.0.1/syntrac_opentelemetry/instrumentation/openai/v1/__pycache__/__init__.cpython-311.pyc` & `syntrac_opentelemetry_instrumentation_openai-0.0.2/syntrac_opentelemetry/instrumentation/openai/v1/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `syntrac_opentelemetry_instrumentation_openai-0.0.1/syntrac_opentelemetry/instrumentation/openai/v1/__pycache__/assistant_wrappers.cpython-311.pyc` & `syntrac_opentelemetry_instrumentation_openai-0.0.2/syntrac_opentelemetry/instrumentation/openai/v1/__pycache__/assistant_wrappers.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `syntrac_opentelemetry_instrumentation_openai-0.0.1/syntrac_opentelemetry/instrumentation/openai/v1/__pycache__/event_handler_wrapper.cpython-311.pyc` & `syntrac_opentelemetry_instrumentation_openai-0.0.2/syntrac_opentelemetry/instrumentation/openai/v1/__pycache__/event_handler_wrapper.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `syntrac_opentelemetry_instrumentation_openai-0.0.1/syntrac_opentelemetry/instrumentation/openai/v1/assistant_wrappers.py` & `syntrac_opentelemetry_instrumentation_openai-0.0.2/syntrac_opentelemetry/instrumentation/openai/v1/assistant_wrappers.py`

 * *Files identical despite different names*

### Comparing `syntrac_opentelemetry_instrumentation_openai-0.0.1/syntrac_opentelemetry/instrumentation/openai/v1/event_handler_wrapper.py` & `syntrac_opentelemetry_instrumentation_openai-0.0.2/syntrac_opentelemetry/instrumentation/openai/v1/event_handler_wrapper.py`

 * *Files identical despite different names*

