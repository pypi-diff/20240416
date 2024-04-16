# Comparing `tmp/openllmtelemetry-0.0.1.dev1.tar.gz` & `tmp/openllmtelemetry-0.0.1b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openllmtelemetry-0.0.1.dev1.tar", max compression
+gzip compressed data, was "openllmtelemetry-0.0.1b2.tar", max compression
```

## Comparing `openllmtelemetry-0.0.1.dev1.tar` & `openllmtelemetry-0.0.1b2.tar`

### file list

```diff
@@ -1,11 +1,23 @@
--rw-r--r--   0        0        0    11357 2023-11-22 23:27:14.459880 openllmtelemetry-0.0.1.dev1/LICENSE
--rw-r--r--   0        0        0     1218 2023-11-23 00:29:23.130474 openllmtelemetry-0.0.1.dev1/README.md
--rw-r--r--   0        0        0      451 2023-11-23 00:29:23.130882 openllmtelemetry-0.0.1.dev1/openllmtelemetry/__init__.py
--rw-r--r--   0        0        0      940 2024-01-31 22:57:51.764550 openllmtelemetry-0.0.1.dev1/openllmtelemetry/common/constants.py
--rw-r--r--   0        0        0      393 2024-01-31 22:58:40.707890 openllmtelemetry-0.0.1.dev1/openllmtelemetry/common/flags.py
--rw-r--r--   0        0        0      123 2023-11-23 00:29:23.131173 openllmtelemetry-0.0.1.dev1/openllmtelemetry/instrument.py
--rw-r--r--   0        0        0      390 2023-11-28 18:18:00.218742 openllmtelemetry-0.0.1.dev1/openllmtelemetry/langkit.py
--rw-r--r--   0        0        0        0 2023-11-29 15:24:45.135230 openllmtelemetry-0.0.1.dev1/openllmtelemetry/openai/__init__.py
--rw-r--r--   0        0        0    13719 2024-02-01 21:06:05.164973 openllmtelemetry-0.0.1.dev1/openllmtelemetry/openai/tracer.py
--rw-r--r--   0        0        0      685 2024-02-07 19:23:12.714182 openllmtelemetry-0.0.1.dev1/pyproject.toml
--rw-r--r--   0        0        0     1971 1970-01-01 00:00:00.000000 openllmtelemetry-0.0.1.dev1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-11-22 23:28:04.346648 openllmtelemetry-0.0.1b2/LICENSE
+-rw-r--r--   0        0        0     3140 2024-04-16 19:52:01.483937 openllmtelemetry-0.0.1b2/README.md
+-rw-r--r--   0        0        0       75 2024-03-28 15:52:01.437323 openllmtelemetry-0.0.1b2/openllmtelemetry/__init__.py
+-rw-r--r--   0        0        0     4106 2024-04-16 17:45:28.623938 openllmtelemetry-0.0.1b2/openllmtelemetry/instrument.py
+-rw-r--r--   0        0        0    11339 2024-04-16 14:55:52.423938 openllmtelemetry-0.0.1b2/openllmtelemetry/instrumentation/LICENSE
+-rw-r--r--   0        0        0        0 2024-04-16 14:55:52.423938 openllmtelemetry-0.0.1b2/openllmtelemetry/instrumentation/__init__.py
+-rw-r--r--   0        0        0     8792 2024-04-16 18:37:58.063936 openllmtelemetry-0.0.1b2/openllmtelemetry/instrumentation/bedrock/__init__.py
+-rw-r--r--   0        0        0     1673 2024-04-16 14:55:52.423938 openllmtelemetry-0.0.1b2/openllmtelemetry/instrumentation/bedrock/reusable_streaming_body.py
+-rw-r--r--   0        0        0     1030 2024-04-16 14:55:52.423938 openllmtelemetry-0.0.1b2/openllmtelemetry/instrumentation/openai/__init__.py
+-rw-r--r--   0        0        0     4007 2024-04-16 15:25:23.173936 openllmtelemetry-0.0.1b2/openllmtelemetry/instrumentation/openai/shared/__init__.py
+-rw-r--r--   0        0        0     7647 2024-04-16 18:36:43.843936 openllmtelemetry-0.0.1b2/openllmtelemetry/instrumentation/openai/shared/chat_wrappers.py
+-rw-r--r--   0        0        0     4701 2024-04-16 18:36:20.733936 openllmtelemetry-0.0.1b2/openllmtelemetry/instrumentation/openai/shared/completion_wrappers.py
+-rw-r--r--   0        0        0     2838 2024-04-16 18:36:02.693936 openllmtelemetry-0.0.1b2/openllmtelemetry/instrumentation/openai/shared/embeddings_wrappers.py
+-rw-r--r--   0        0        0      560 2024-04-16 14:55:52.433938 openllmtelemetry-0.0.1b2/openllmtelemetry/instrumentation/openai/utils.py
+-rw-r--r--   0        0        0     1712 2024-04-16 15:25:14.393936 openllmtelemetry-0.0.1b2/openllmtelemetry/instrumentation/openai/v0/__init__.py
+-rw-r--r--   0        0        0     2239 2024-04-16 15:25:33.883935 openllmtelemetry-0.0.1b2/openllmtelemetry/instrumentation/openai/v1/__init__.py
+-rw-r--r--   0        0        0       28 2024-03-22 16:01:52.610949 openllmtelemetry-0.0.1b2/openllmtelemetry/instrumentation/openai/version.py
+-rw-r--r--   0        0        0     1357 2024-04-16 15:51:10.973936 openllmtelemetry-0.0.1b2/openllmtelemetry/intrument_openai.py
+-rw-r--r--   0        0        0     3118 2024-04-16 16:58:47.443939 openllmtelemetry-0.0.1b2/openllmtelemetry/secure.py
+-rw-r--r--   0        0        0     1786 2024-03-28 20:14:24.636459 openllmtelemetry-0.0.1b2/openllmtelemetry/semantic_conventions/gen_ai/__init__.py
+-rw-r--r--   0        0        0      477 2024-04-16 14:55:43.883938 openllmtelemetry-0.0.1b2/openllmtelemetry/version.py
+-rw-r--r--   0        0        0     1595 2024-04-16 19:51:35.603937 openllmtelemetry-0.0.1b2/pyproject.toml
+-rw-r--r--   0        0        0     4058 1970-01-01 00:00:00.000000 openllmtelemetry-0.0.1b2/PKG-INFO
```

### Comparing `openllmtelemetry-0.0.1.dev1/LICENSE` & `openllmtelemetry-0.0.1b2/LICENSE`

 * *Files identical despite different names*

