# Comparing `tmp/modelgauge-0.3.3.tar.gz` & `tmp/modelgauge-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelgauge-0.3.3.tar", max compression
+gzip compressed data, was "modelgauge-0.5.0.tar", max compression
```

## Comparing `modelgauge-0.3.3.tar` & `modelgauge-0.5.0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0    10174 2024-04-10 19:55:36.512596 modelgauge-0.3.3/LICENSE.md
--rw-r--r--   0        0        0     1434 2024-04-11 19:30:18.206705 modelgauge-0.3.3/README.md
--rw-r--r--   0        0        0     2709 2024-04-11 19:30:18.209705 modelgauge-0.3.3/modelgauge/aggregations.py
--rw-r--r--   0        0        0      385 2024-04-12 19:02:51.769903 modelgauge-0.3.3/modelgauge/annotation.py
--rw-r--r--   0        0        0     1151 2024-04-12 19:02:51.769903 modelgauge-0.3.3/modelgauge/annotator.py
--rw-r--r--   0        0        0      429 2024-04-11 19:30:18.210705 modelgauge-0.3.3/modelgauge/annotators/README.md
--rw-r--r--   0        0        0     2529 2024-04-12 17:44:37.230043 modelgauge-0.3.3/modelgauge/base_test.py
--rw-r--r--   0        0        0     4079 2024-04-12 20:44:33.539698 modelgauge-0.3.3/modelgauge/caching.py
--rw-r--r--   0        0        0      986 2024-04-11 19:30:18.210705 modelgauge-0.3.3/modelgauge/command_line.py
--rw-r--r--   0        0        0      842 2024-04-11 19:30:18.210705 modelgauge-0.3.3/modelgauge/concurrency.py
--rw-r--r--   0        0        0     3049 2024-04-11 19:30:18.210705 modelgauge-0.3.3/modelgauge/config.py
--rw-r--r--   0        0        0      389 2024-04-11 19:30:18.210705 modelgauge-0.3.3/modelgauge/config_templates/secrets.toml
--rw-r--r--   0        0        0     1913 2024-04-11 19:30:18.210705 modelgauge-0.3.3/modelgauge/data_packing.py
--rw-r--r--   0        0        0     6856 2024-04-12 17:44:37.230043 modelgauge-0.3.3/modelgauge/dependency_helper.py
--rw-r--r--   0        0        0     3284 2024-04-11 19:30:18.210705 modelgauge-0.3.3/modelgauge/dependency_injection.py
--rw-r--r--   0        0        0     2137 2024-04-11 19:30:18.210705 modelgauge-0.3.3/modelgauge/external_data.py
--rw-r--r--   0        0        0     2378 2024-04-12 17:44:37.230043 modelgauge-0.3.3/modelgauge/general.py
--rw-r--r--   0        0        0     3902 2024-04-12 18:58:03.642894 modelgauge-0.3.3/modelgauge/instance_factory.py
--rw-r--r--   0        0        0     1330 2024-04-12 17:44:37.230043 modelgauge-0.3.3/modelgauge/load_plugins.py
--rw-r--r--   0        0        0     7485 2024-04-12 19:21:15.899936 modelgauge-0.3.3/modelgauge/main.py
--rw-r--r--   0        0        0     5278 2024-04-11 19:30:18.211705 modelgauge-0.3.3/modelgauge/multiple_choice_questions.py
--rw-r--r--   0        0        0      570 2024-04-11 19:30:18.211705 modelgauge-0.3.3/modelgauge/not_implemented.py
--rw-r--r--   0        0        0     1808 2024-04-11 19:30:18.211705 modelgauge-0.3.3/modelgauge/prompt.py
--rw-r--r--   0        0        0      539 2024-04-11 19:30:18.211705 modelgauge-0.3.3/modelgauge/prompt_formatting.py
--rw-r--r--   0        0        0     1083 2024-04-11 19:30:18.211705 modelgauge-0.3.3/modelgauge/record_init.py
--rw-r--r--   0        0        0     1282 2024-04-12 17:44:37.231043 modelgauge-0.3.3/modelgauge/records.py
--rw-r--r--   0        0        0      420 2024-04-11 19:30:18.213705 modelgauge-0.3.3/modelgauge/runners/README.md
--rw-r--r--   0        0        0     4799 2024-04-12 17:44:37.231043 modelgauge-0.3.3/modelgauge/secret_values.py
--rw-r--r--   0        0        0     6587 2024-04-12 19:02:51.769903 modelgauge-0.3.3/modelgauge/simple_test_runner.py
--rw-r--r--   0        0        0     4132 2024-04-12 19:02:51.770903 modelgauge-0.3.3/modelgauge/single_turn_prompt_response.py
--rw-r--r--   0        0        0     3011 2024-04-12 17:44:37.231043 modelgauge-0.3.3/modelgauge/sut.py
--rw-r--r--   0        0        0      803 2024-04-11 19:30:18.213705 modelgauge-0.3.3/modelgauge/sut_capabilities.py
--rw-r--r--   0        0        0     1511 2024-04-11 19:30:18.213705 modelgauge-0.3.3/modelgauge/sut_capabilities_verification.py
--rw-r--r--   0        0        0     3888 2024-04-12 17:44:37.231043 modelgauge-0.3.3/modelgauge/sut_decorator.py
--rw-r--r--   0        0        0      170 2024-04-12 17:44:37.231043 modelgauge-0.3.3/modelgauge/sut_registry.py
--rw-r--r--   0        0        0      411 2024-04-11 19:30:18.214705 modelgauge-0.3.3/modelgauge/suts/README.md
--rw-r--r--   0        0        0     5253 2024-04-12 17:44:37.231043 modelgauge-0.3.3/modelgauge/test_decorator.py
--rw-r--r--   0        0        0      188 2024-04-12 17:44:37.231043 modelgauge-0.3.3/modelgauge/test_registry.py
--rw-r--r--   0        0        0      414 2024-04-11 19:30:18.214705 modelgauge-0.3.3/modelgauge/tests/README.md
--rw-r--r--   0        0        0        4 2024-04-11 19:30:18.214705 modelgauge-0.3.3/modelgauge/tests/specifications/README.md
--rw-r--r--   0        0        0      151 2024-04-11 19:30:18.214705 modelgauge-0.3.3/modelgauge/tracked_object.py
--rw-r--r--   0        0        0     2476 2024-04-12 17:05:04.055970 modelgauge-0.3.3/modelgauge/typed_data.py
--rw-r--r--   0        0        0     3959 2024-04-12 18:56:17.758891 modelgauge-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     3757 1970-01-01 00:00:00.000000 modelgauge-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0    10174 2024-04-10 19:55:36.512596 modelgauge-0.5.0/LICENSE.md
+-rw-r--r--   0        0        0     1443 2024-04-15 22:05:52.195001 modelgauge-0.5.0/README.md
+-rw-r--r--   0        0        0     2709 2024-04-11 19:30:18.209705 modelgauge-0.5.0/modelgauge/aggregations.py
+-rw-r--r--   0        0        0      385 2024-04-12 19:02:51.769903 modelgauge-0.5.0/modelgauge/annotation.py
+-rw-r--r--   0        0        0     1151 2024-04-12 19:02:51.769903 modelgauge-0.5.0/modelgauge/annotator.py
+-rw-r--r--   0        0        0      429 2024-04-11 19:30:18.210705 modelgauge-0.5.0/modelgauge/annotators/README.md
+-rw-r--r--   0        0        0     2529 2024-04-12 17:44:37.230043 modelgauge-0.5.0/modelgauge/base_test.py
+-rw-r--r--   0        0        0     4079 2024-04-15 15:41:46.097692 modelgauge-0.5.0/modelgauge/caching.py
+-rw-r--r--   0        0        0      986 2024-04-11 19:30:18.210705 modelgauge-0.5.0/modelgauge/command_line.py
+-rw-r--r--   0        0        0      842 2024-04-11 19:30:18.210705 modelgauge-0.5.0/modelgauge/concurrency.py
+-rw-r--r--   0        0        0     3049 2024-04-11 19:30:18.210705 modelgauge-0.5.0/modelgauge/config.py
+-rw-r--r--   0        0        0      389 2024-04-11 19:30:18.210705 modelgauge-0.5.0/modelgauge/config_templates/secrets.toml
+-rw-r--r--   0        0        0     1913 2024-04-11 19:30:18.210705 modelgauge-0.5.0/modelgauge/data_packing.py
+-rw-r--r--   0        0        0     6856 2024-04-12 17:44:37.230043 modelgauge-0.5.0/modelgauge/dependency_helper.py
+-rw-r--r--   0        0        0     3284 2024-04-11 19:30:18.210705 modelgauge-0.5.0/modelgauge/dependency_injection.py
+-rw-r--r--   0        0        0     2137 2024-04-11 19:30:18.210705 modelgauge-0.5.0/modelgauge/external_data.py
+-rw-r--r--   0        0        0     2378 2024-04-12 17:44:37.230043 modelgauge-0.5.0/modelgauge/general.py
+-rw-r--r--   0        0        0     3902 2024-04-12 18:58:03.642894 modelgauge-0.5.0/modelgauge/instance_factory.py
+-rw-r--r--   0        0        0     1330 2024-04-12 17:44:37.230043 modelgauge-0.5.0/modelgauge/load_plugins.py
+-rw-r--r--   0        0        0     7485 2024-04-12 19:21:15.899936 modelgauge-0.5.0/modelgauge/main.py
+-rw-r--r--   0        0        0     5278 2024-04-11 19:30:18.211705 modelgauge-0.5.0/modelgauge/multiple_choice_questions.py
+-rw-r--r--   0        0        0      570 2024-04-11 19:30:18.211705 modelgauge-0.5.0/modelgauge/not_implemented.py
+-rw-r--r--   0        0        0     1808 2024-04-11 19:30:18.211705 modelgauge-0.5.0/modelgauge/prompt.py
+-rw-r--r--   0        0        0      539 2024-04-11 19:30:18.211705 modelgauge-0.5.0/modelgauge/prompt_formatting.py
+-rw-r--r--   0        0        0     1083 2024-04-11 19:30:18.211705 modelgauge-0.5.0/modelgauge/record_init.py
+-rw-r--r--   0        0        0     1282 2024-04-12 17:44:37.231043 modelgauge-0.5.0/modelgauge/records.py
+-rw-r--r--   0        0        0      420 2024-04-11 19:30:18.213705 modelgauge-0.5.0/modelgauge/runners/README.md
+-rw-r--r--   0        0        0     4799 2024-04-12 17:44:37.231043 modelgauge-0.5.0/modelgauge/secret_values.py
+-rw-r--r--   0        0        0     6587 2024-04-12 19:02:51.769903 modelgauge-0.5.0/modelgauge/simple_test_runner.py
+-rw-r--r--   0        0        0     4132 2024-04-12 19:02:51.770903 modelgauge-0.5.0/modelgauge/single_turn_prompt_response.py
+-rw-r--r--   0        0        0     3011 2024-04-12 17:44:37.231043 modelgauge-0.5.0/modelgauge/sut.py
+-rw-r--r--   0        0        0      803 2024-04-11 19:30:18.213705 modelgauge-0.5.0/modelgauge/sut_capabilities.py
+-rw-r--r--   0        0        0     1511 2024-04-11 19:30:18.213705 modelgauge-0.5.0/modelgauge/sut_capabilities_verification.py
+-rw-r--r--   0        0        0     3888 2024-04-12 17:44:37.231043 modelgauge-0.5.0/modelgauge/sut_decorator.py
+-rw-r--r--   0        0        0      170 2024-04-12 17:44:37.231043 modelgauge-0.5.0/modelgauge/sut_registry.py
+-rw-r--r--   0        0        0      411 2024-04-11 19:30:18.214705 modelgauge-0.5.0/modelgauge/suts/README.md
+-rw-r--r--   0        0        0     5253 2024-04-12 17:44:37.231043 modelgauge-0.5.0/modelgauge/test_decorator.py
+-rw-r--r--   0        0        0      188 2024-04-12 17:44:37.231043 modelgauge-0.5.0/modelgauge/test_registry.py
+-rw-r--r--   0        0        0      414 2024-04-11 19:30:18.214705 modelgauge-0.5.0/modelgauge/tests/README.md
+-rw-r--r--   0        0        0        4 2024-04-11 19:30:18.214705 modelgauge-0.5.0/modelgauge/tests/specifications/README.md
+-rw-r--r--   0        0        0      151 2024-04-11 19:30:18.214705 modelgauge-0.5.0/modelgauge/tracked_object.py
+-rw-r--r--   0        0        0     2476 2024-04-12 17:05:04.055970 modelgauge-0.5.0/modelgauge/typed_data.py
+-rw-r--r--   0        0        0     3967 2024-04-15 22:05:52.198001 modelgauge-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     3867 1970-01-01 00:00:00.000000 modelgauge-0.5.0/PKG-INFO
```

### Comparing `modelgauge-0.3.3/LICENSE.md` & `modelgauge-0.5.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `modelgauge-0.3.3/README.md` & `modelgauge-0.5.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Model Gauge
+# ModelGauge
 
 Goal: Make it easy to automatically and uniformly measure the behavior of many AI Systems.
 
 > [!WARNING]
 > This repo is still in **beta** with a planned full release in Fall 2024. Until then we reserve the right to make backward incompatible changes as needed.
 
 ModelGauge is an evolution of [crfm-helm](https://github.com/stanford-crfm/helm/), intended to meet their existing use cases as well as those needed by the [MLCommons AI Safety](https://mlcommons.org/working-groups/ai-safety/ai-safety/) project.
@@ -15,11 +15,11 @@
 * Adding new Tests or SUTs can be done without modifications to the core libraries or support from ModelGauge authors.
 
 Currently ModelGauge is targeted at LLMs and [single turn prompt response Tests](docs/prompt_response_tests.md), with Tests scored by automated Annotators (e.g. LlamaGuard). However, we expect to extend the library to cover more Test, SUT, and Annotation types as we move toward full release.
 
 
 ## Docs
 
-* [Quick Start](docs/dev_quick_start.md)
+* [Developer Quick Start](docs/dev_quick_start.md)
 * [Tutorial for how to create a Test](docs/tutorial_tests.md)
 * [Tutorial for how to create a System Under Test (SUT)](docs/tutorial_suts.md)
 * How we use [plugins](docs/plugins.md) to connect it all together.
```

### Comparing `modelgauge-0.3.3/modelgauge/aggregations.py` & `modelgauge-0.5.0/modelgauge/aggregations.py`

 * *Files identical despite different names*

### Comparing `modelgauge-0.3.3/modelgauge/annotator.py` & `modelgauge-0.5.0/modelgauge/annotator.py`

 * *Files identical despite different names*

### Comparing `modelgauge-0.3.3/modelgauge/base_test.py` & `modelgauge-0.5.0/modelgauge/base_test.py`

 * *Files identical despite different names*

### Comparing `modelgauge-0.3.3/modelgauge/caching.py` & `modelgauge-0.5.0/modelgauge/caching.py`

 * *Files identical despite different names*

### Comparing `modelgauge-0.3.3/modelgauge/command_line.py` & `modelgauge-0.5.0/modelgauge/command_line.py`

 * *Files identical despite different names*

### Comparing `modelgauge-0.3.3/modelgauge/concurrency.py` & `modelgauge-0.5.0/modelgauge/concurrency.py`

 * *Files identical despite different names*

### Comparing `modelgauge-0.3.3/modelgauge/config.py` & `modelgauge-0.5.0/modelgauge/config.py`

 * *Files identical despite different names*

### Comparing `modelgauge-0.3.3/modelgauge/data_packing.py` & `modelgauge-0.5.0/modelgauge/data_packing.py`

 * *Files identical despite different names*

### Comparing `modelgauge-0.3.3/modelgauge/dependency_helper.py` & `modelgauge-0.5.0/modelgauge/dependency_helper.py`

 * *Files identical despite different names*

### Comparing `modelgauge-0.3.3/modelgauge/dependency_injection.py` & `modelgauge-0.5.0/modelgauge/dependency_injection.py`

 * *Files identical despite different names*

### Comparing `modelgauge-0.3.3/modelgauge/external_data.py` & `modelgauge-0.5.0/modelgauge/external_data.py`

 * *Files identical despite different names*

### Comparing `modelgauge-0.3.3/modelgauge/general.py` & `modelgauge-0.5.0/modelgauge/general.py`

 * *Files identical despite different names*

### Comparing `modelgauge-0.3.3/modelgauge/instance_factory.py` & `modelgauge-0.5.0/modelgauge/instance_factory.py`

 * *Files identical despite different names*

### Comparing `modelgauge-0.3.3/modelgauge/load_plugins.py` & `modelgauge-0.5.0/modelgauge/load_plugins.py`

 * *Files identical despite different names*

### Comparing `modelgauge-0.3.3/modelgauge/main.py` & `modelgauge-0.5.0/modelgauge/main.py`

 * *Files identical despite different names*

### Comparing `modelgauge-0.3.3/modelgauge/multiple_choice_questions.py` & `modelgauge-0.5.0/modelgauge/multiple_choice_questions.py`

 * *Files identical despite different names*

### Comparing `modelgauge-0.3.3/modelgauge/not_implemented.py` & `modelgauge-0.5.0/modelgauge/not_implemented.py`

 * *Files identical despite different names*

### Comparing `modelgauge-0.3.3/modelgauge/prompt.py` & `modelgauge-0.5.0/modelgauge/prompt.py`

 * *Files identical despite different names*

### Comparing `modelgauge-0.3.3/modelgauge/prompt_formatting.py` & `modelgauge-0.5.0/modelgauge/prompt_formatting.py`

 * *Files identical despite different names*

### Comparing `modelgauge-0.3.3/modelgauge/record_init.py` & `modelgauge-0.5.0/modelgauge/record_init.py`

 * *Files identical despite different names*

### Comparing `modelgauge-0.3.3/modelgauge/records.py` & `modelgauge-0.5.0/modelgauge/records.py`

 * *Files identical despite different names*

### Comparing `modelgauge-0.3.3/modelgauge/secret_values.py` & `modelgauge-0.5.0/modelgauge/secret_values.py`

 * *Files identical despite different names*

### Comparing `modelgauge-0.3.3/modelgauge/simple_test_runner.py` & `modelgauge-0.5.0/modelgauge/simple_test_runner.py`

 * *Files identical despite different names*

### Comparing `modelgauge-0.3.3/modelgauge/single_turn_prompt_response.py` & `modelgauge-0.5.0/modelgauge/single_turn_prompt_response.py`

 * *Files identical despite different names*

### Comparing `modelgauge-0.3.3/modelgauge/sut.py` & `modelgauge-0.5.0/modelgauge/sut.py`

 * *Files identical despite different names*

### Comparing `modelgauge-0.3.3/modelgauge/sut_capabilities.py` & `modelgauge-0.5.0/modelgauge/sut_capabilities.py`

 * *Files identical despite different names*

### Comparing `modelgauge-0.3.3/modelgauge/sut_capabilities_verification.py` & `modelgauge-0.5.0/modelgauge/sut_capabilities_verification.py`

 * *Files identical despite different names*

### Comparing `modelgauge-0.3.3/modelgauge/sut_decorator.py` & `modelgauge-0.5.0/modelgauge/sut_decorator.py`

 * *Files identical despite different names*

### Comparing `modelgauge-0.3.3/modelgauge/test_decorator.py` & `modelgauge-0.5.0/modelgauge/test_decorator.py`

 * *Files identical despite different names*

### Comparing `modelgauge-0.3.3/modelgauge/typed_data.py` & `modelgauge-0.5.0/modelgauge/typed_data.py`

 * *Files identical despite different names*

### Comparing `modelgauge-0.3.3/pyproject.toml` & `modelgauge-0.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "modelgauge"
-version = "0.3.3"
+version = "0.5.0"
 description = "Automatically and uniformly measure the behavior of many AI Systems."
 license = "Apache-2.0"
 authors = ["MLCommons AI Safety <ai-safety-engineering@mlcommons.org>"]
 readme = "README.md"
 repository = "https://github.com/mlcommons/modelgauge"
 keywords = [
     "AI",
@@ -37,15 +37,15 @@
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: System :: Benchmark",
     "Typing :: Typed",
 ]
 
 
 [tool.poetry.dependencies]
-python = ">=3.10, <3.11"
+python = "^3.10"
 zstandard = ">=0.18.0,<0.19.0"
 tqdm = ">=4.66.1"
 types-tqdm = "^4.66.0.0"
 pydantic = "^2.6.0"
 sqlitedict = "^2.1.0"
 gdown = ">=5.1.0"
 modelgauge_demo_plugin = {version = "*", optional = true}
@@ -69,14 +69,15 @@
 pytest = "^7.4.3"
 mypy = "^1.7.1"
 black = "^23.11.0"
 pytest-mock = "^3.12.0"
 pytest-timeout = "^2.3.1"
 flaky = "^3.8.1"
 nbmake = "^1.5.3"
+tox = "^4.14.2"
 
 [tool.pytest.ini_options]
 # Ignore the main source that might have things named "test"
 addopts="--ignore=modelgauge/ --ignore=demo_plugin/modelgauge/ --ignore=plugins/*/modelgauge/"
 
 [tool.mypy]
 # Using namespace packages to do plugins requires us not to have __init__.py files.
```

### Comparing `modelgauge-0.3.3/PKG-INFO` & `modelgauge-0.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 Metadata-Version: 2.1
 Name: modelgauge
-Version: 0.3.3
+Version: 0.5.0
 Summary: Automatically and uniformly measure the behavior of many AI Systems.
 Home-page: https://github.com/mlcommons/modelgauge
 License: Apache-2.0
 Keywords: AI,GenAI,LLM,NLP,evaluate,measure,quality,testing,prompt,safety,compare,artificial,intelligence,Large,Language,Models
 Author: MLCommons AI Safety
 Author-email: ai-safety-engineering@mlcommons.org
-Requires-Python: >=3.10,<3.11
+Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Benchmark
 Classifier: Typing :: Typed
 Provides-Extra: all-plugins
 Provides-Extra: demo
@@ -43,15 +45,15 @@
 Requires-Dist: tqdm (>=4.66.1)
 Requires-Dist: types-tqdm (>=4.66.0.0,<5.0.0.0)
 Requires-Dist: typing-extensions (>=4.10.0,<5.0.0)
 Requires-Dist: zstandard (>=0.18.0,<0.19.0)
 Project-URL: Repository, https://github.com/mlcommons/modelgauge
 Description-Content-Type: text/markdown
 
-# Model Gauge
+# ModelGauge
 
 Goal: Make it easy to automatically and uniformly measure the behavior of many AI Systems.
 
 > [!WARNING]
 > This repo is still in **beta** with a planned full release in Fall 2024. Until then we reserve the right to make backward incompatible changes as needed.
 
 ModelGauge is an evolution of [crfm-helm](https://github.com/stanford-crfm/helm/), intended to meet their existing use cases as well as those needed by the [MLCommons AI Safety](https://mlcommons.org/working-groups/ai-safety/ai-safety/) project.
@@ -64,12 +66,12 @@
 * Adding new Tests or SUTs can be done without modifications to the core libraries or support from ModelGauge authors.
 
 Currently ModelGauge is targeted at LLMs and [single turn prompt response Tests](docs/prompt_response_tests.md), with Tests scored by automated Annotators (e.g. LlamaGuard). However, we expect to extend the library to cover more Test, SUT, and Annotation types as we move toward full release.
 
 
 ## Docs
 
-* [Quick Start](docs/dev_quick_start.md)
+* [Developer Quick Start](docs/dev_quick_start.md)
 * [Tutorial for how to create a Test](docs/tutorial_tests.md)
 * [Tutorial for how to create a System Under Test (SUT)](docs/tutorial_suts.md)
 * How we use [plugins](docs/plugins.md) to connect it all together.
```

