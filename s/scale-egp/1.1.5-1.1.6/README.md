# Comparing `tmp/scale_egp-1.1.5.tar.gz` & `tmp/scale_egp-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scale_egp-1.1.5.tar", max compression
+gzip compressed data, was "scale_egp-1.1.6.tar", max compression
```

## Comparing `scale_egp-1.1.5.tar` & `scale_egp-1.1.6.tar`

### file list

```diff
@@ -1,63 +1,63 @@
--rw-r--r--   0        0        0    17859 2024-04-09 22:10:29.167863 scale_egp-1.1.5/README.md
--rw-r--r--   0        0        0     1100 2024-04-09 22:10:29.167863 scale_egp-1.1.5/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-09 22:10:29.163863 scale_egp-1.1.5/scale_egp/__init__.py
--rw-r--r--   0        0        0       74 2024-04-09 22:10:29.163863 scale_egp-1.1.5/scale_egp/cli/__init__.py
--rw-r--r--   0        0        0     4533 2024-04-09 22:10:29.163863 scale_egp-1.1.5/scale_egp/cli/cli_main.py
--rw-r--r--   0        0        0    17966 2024-04-09 22:10:29.163863 scale_egp-1.1.5/scale_egp/cli/collections.py
--rw-r--r--   0        0        0     7857 2024-04-09 22:10:29.163863 scale_egp-1.1.5/scale_egp/cli/formatter.py
--rw-r--r--   0        0        0     1469 2024-04-09 22:10:29.163863 scale_egp-1.1.5/scale_egp/cli/model_instance_description.py
--rw-r--r--   0        0        0     1828 2024-04-09 22:10:29.163863 scale_egp-1.1.5/scale_egp/cli/parser.py
--rw-r--r--   0        0        0     1733 2024-04-09 22:10:29.163863 scale_egp-1.1.5/scale_egp/exceptions.py
--rw-r--r--   0        0        0        0 2024-04-09 22:10:29.163863 scale_egp-1.1.5/scale_egp/sdk/__init__.py
--rw-r--r--   0        0        0    13096 2024-04-09 22:10:29.163863 scale_egp-1.1.5/scale_egp/sdk/client.py
--rw-r--r--   0        0        0        0 2024-04-09 22:10:29.167863 scale_egp-1.1.5/scale_egp/sdk/collections/__init__.py
--rw-r--r--   0        0        0     2914 2024-04-09 22:10:29.167863 scale_egp-1.1.5/scale_egp/sdk/collections/application_specs.py
--rw-r--r--   0        0        0     3170 2024-04-09 22:10:29.167863 scale_egp-1.1.5/scale_egp/sdk/collections/chunks.py
--rw-r--r--   0        0        0     5272 2024-04-09 22:10:29.167863 scale_egp-1.1.5/scale_egp/sdk/collections/completions.py
--rw-r--r--   0        0        0     2500 2024-04-09 22:10:29.167863 scale_egp-1.1.5/scale_egp/sdk/collections/evaluation_configs.py
--rw-r--r--   0        0        0    25007 2024-04-09 22:10:29.167863 scale_egp-1.1.5/scale_egp/sdk/collections/evaluation_datasets.py
--rw-r--r--   0        0        0     8055 2024-04-09 22:10:29.167863 scale_egp-1.1.5/scale_egp/sdk/collections/evaluations.py
--rw-r--r--   0        0        0     4918 2024-04-09 22:10:29.167863 scale_egp-1.1.5/scale_egp/sdk/collections/fine_tuning.py
--rw-r--r--   0        0        0    25810 2024-04-09 22:10:29.167863 scale_egp-1.1.5/scale_egp/sdk/collections/knowledge_bases.py
--rw-r--r--   0        0        0     2685 2024-04-09 22:10:29.167863 scale_egp-1.1.5/scale_egp/sdk/collections/model_groups.py
--rw-r--r--   0        0        0     4798 2024-04-09 22:10:29.167863 scale_egp-1.1.5/scale_egp/sdk/collections/model_templates.py
--rw-r--r--   0        0        0     7572 2024-04-09 22:10:29.167863 scale_egp-1.1.5/scale_egp/sdk/collections/models.py
--rw-r--r--   0        0        0     1862 2024-04-09 22:10:29.167863 scale_egp-1.1.5/scale_egp/sdk/collections/question_sets.py
--rw-r--r--   0        0        0     2588 2024-04-09 22:10:29.167863 scale_egp-1.1.5/scale_egp/sdk/collections/questions.py
--rw-r--r--   0        0        0     1510 2024-04-09 22:10:29.167863 scale_egp-1.1.5/scale_egp/sdk/collections/users.py
--rw-r--r--   0        0        0        0 2024-04-09 22:10:29.163863 scale_egp-1.1.5/scale_egp/sdk/constants/__init__.py
--rw-r--r--   0        0        0      762 2024-04-09 22:10:29.163863 scale_egp-1.1.5/scale_egp/sdk/constants/model_schemas.py
--rw-r--r--   0        0        0     9225 2024-04-09 22:10:29.163863 scale_egp-1.1.5/scale_egp/sdk/enums.py
--rw-r--r--   0        0        0        0 2024-04-09 22:10:29.163863 scale_egp-1.1.5/scale_egp/sdk/models/__init__.py
--rw-r--r--   0        0        0     2387 2024-04-09 22:10:29.163863 scale_egp-1.1.5/scale_egp/sdk/models/fine_tuning_jobs.py
--rw-r--r--   0        0        0     2069 2024-04-09 22:10:29.163863 scale_egp-1.1.5/scale_egp/sdk/models/model_enums.py
--rw-r--r--   0        0        0     8403 2024-04-09 22:10:29.163863 scale_egp-1.1.5/scale_egp/sdk/models/model_vendor_configuration.py
--rw-r--r--   0        0        0      647 2024-04-09 22:10:29.163863 scale_egp-1.1.5/scale_egp/sdk/types/__init__.py
--rw-r--r--   0        0        0     4651 2024-04-09 22:10:29.163863 scale_egp-1.1.5/scale_egp/sdk/types/agents.py
--rw-r--r--   0        0        0      741 2024-04-09 22:10:29.163863 scale_egp-1.1.5/scale_egp/sdk/types/application_specs.py
--rw-r--r--   0        0        0     6125 2024-04-09 22:10:29.163863 scale_egp-1.1.5/scale_egp/sdk/types/chunks.py
--rw-r--r--   0        0        0     6553 2024-04-09 22:10:29.163863 scale_egp-1.1.5/scale_egp/sdk/types/completions.py
--rw-r--r--   0        0        0     1016 2024-04-09 22:10:29.163863 scale_egp-1.1.5/scale_egp/sdk/types/embeddings.py
--rw-r--r--   0        0        0     1019 2024-04-09 22:10:29.167863 scale_egp-1.1.5/scale_egp/sdk/types/evaluation_configs.py
--rw-r--r--   0        0        0     3474 2024-04-09 22:10:29.167863 scale_egp-1.1.5/scale_egp/sdk/types/evaluation_dataset_test_cases.py
--rw-r--r--   0        0        0     1686 2024-04-09 22:10:29.167863 scale_egp-1.1.5/scale_egp/sdk/types/evaluation_datasets.py
--rw-r--r--   0        0        0     4747 2024-04-09 22:10:29.167863 scale_egp-1.1.5/scale_egp/sdk/types/evaluation_test_case_results.py
--rw-r--r--   0        0        0     1398 2024-04-09 22:10:29.167863 scale_egp-1.1.5/scale_egp/sdk/types/evaluations.py
--rw-r--r--   0        0        0     3401 2024-04-09 22:10:29.167863 scale_egp-1.1.5/scale_egp/sdk/types/fine_tuning.py
--rw-r--r--   0        0        0     1860 2024-04-09 22:10:29.167863 scale_egp-1.1.5/scale_egp/sdk/types/knowledge_base_artifacts.py
--rw-r--r--   0        0        0     1559 2024-04-09 22:10:29.167863 scale_egp-1.1.5/scale_egp/sdk/types/knowledge_base_chunks.py
--rw-r--r--   0        0        0    15686 2024-04-09 22:10:29.167863 scale_egp-1.1.5/scale_egp/sdk/types/knowledge_base_uploads.py
--rw-r--r--   0        0        0     1863 2024-04-09 22:10:29.167863 scale_egp-1.1.5/scale_egp/sdk/types/knowledge_bases.py
--rw-r--r--   0        0        0     1112 2024-04-09 22:10:29.167863 scale_egp-1.1.5/scale_egp/sdk/types/memory_strategy.py
--rw-r--r--   0        0        0     2478 2024-04-09 22:10:29.167863 scale_egp-1.1.5/scale_egp/sdk/types/message.py
--rw-r--r--   0        0        0     3557 2024-04-09 22:10:29.167863 scale_egp-1.1.5/scale_egp/sdk/types/model_templates.py
--rw-r--r--   0        0        0    14065 2024-04-09 22:10:29.167863 scale_egp-1.1.5/scale_egp/sdk/types/models.py
--rw-r--r--   0        0        0     1086 2024-04-09 22:10:29.167863 scale_egp-1.1.5/scale_egp/sdk/types/models_group.py
--rw-r--r--   0        0        0      891 2024-04-09 22:10:29.167863 scale_egp-1.1.5/scale_egp/sdk/types/question_sets.py
--rw-r--r--   0        0        0     5234 2024-04-09 22:10:29.167863 scale_egp-1.1.5/scale_egp/sdk/types/questions.py
--rw-r--r--   0        0        0      410 2024-04-09 22:10:29.167863 scale_egp-1.1.5/scale_egp/sdk/types/user_info.py
--rw-r--r--   0        0        0        0 2024-04-09 22:10:29.167863 scale_egp-1.1.5/scale_egp/utils/__init__.py
--rw-r--r--   0        0        0    11461 2024-04-09 22:10:29.167863 scale_egp-1.1.5/scale_egp/utils/api_utils.py
--rw-r--r--   0        0        0     3541 2024-04-09 22:10:29.167863 scale_egp-1.1.5/scale_egp/utils/model_utils.py
--rw-r--r--   0        0        0      107 2024-04-09 22:10:29.167863 scale_egp-1.1.5/scale_egp/utils/strenum_compat.py
--rw-r--r--   0        0        0    18855 1970-01-01 00:00:00.000000 scale_egp-1.1.5/PKG-INFO
+-rw-r--r--   0        0        0    17873 2024-04-16 18:44:22.539571 scale_egp-1.1.6/README.md
+-rw-r--r--   0        0        0     1101 2024-04-16 18:44:22.539571 scale_egp-1.1.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-16 18:44:22.543572 scale_egp-1.1.6/scale_egp/__init__.py
+-rw-r--r--   0        0        0       74 2024-04-16 18:44:22.539571 scale_egp-1.1.6/scale_egp/cli/__init__.py
+-rw-r--r--   0        0        0     4533 2024-04-16 18:44:22.539571 scale_egp-1.1.6/scale_egp/cli/cli_main.py
+-rw-r--r--   0        0        0    17966 2024-04-16 18:44:22.539571 scale_egp-1.1.6/scale_egp/cli/collections.py
+-rw-r--r--   0        0        0     7857 2024-04-16 18:44:22.539571 scale_egp-1.1.6/scale_egp/cli/formatter.py
+-rw-r--r--   0        0        0     1469 2024-04-16 18:44:22.539571 scale_egp-1.1.6/scale_egp/cli/model_instance_description.py
+-rw-r--r--   0        0        0     1828 2024-04-16 18:44:22.539571 scale_egp-1.1.6/scale_egp/cli/parser.py
+-rw-r--r--   0        0        0     1733 2024-04-16 18:44:22.543572 scale_egp-1.1.6/scale_egp/exceptions.py
+-rw-r--r--   0        0        0        0 2024-04-16 18:44:22.539571 scale_egp-1.1.6/scale_egp/sdk/__init__.py
+-rw-r--r--   0        0        0    13096 2024-04-16 18:44:22.539571 scale_egp-1.1.6/scale_egp/sdk/client.py
+-rw-r--r--   0        0        0        0 2024-04-16 18:44:22.543572 scale_egp-1.1.6/scale_egp/sdk/collections/__init__.py
+-rw-r--r--   0        0        0     2914 2024-04-16 18:44:22.543572 scale_egp-1.1.6/scale_egp/sdk/collections/application_specs.py
+-rw-r--r--   0        0        0     3170 2024-04-16 18:44:22.543572 scale_egp-1.1.6/scale_egp/sdk/collections/chunks.py
+-rw-r--r--   0        0        0     5272 2024-04-16 18:44:22.543572 scale_egp-1.1.6/scale_egp/sdk/collections/completions.py
+-rw-r--r--   0        0        0     2500 2024-04-16 18:44:22.543572 scale_egp-1.1.6/scale_egp/sdk/collections/evaluation_configs.py
+-rw-r--r--   0        0        0    25007 2024-04-16 18:44:22.543572 scale_egp-1.1.6/scale_egp/sdk/collections/evaluation_datasets.py
+-rw-r--r--   0        0        0     8055 2024-04-16 18:44:22.543572 scale_egp-1.1.6/scale_egp/sdk/collections/evaluations.py
+-rw-r--r--   0        0        0     4918 2024-04-16 18:44:22.543572 scale_egp-1.1.6/scale_egp/sdk/collections/fine_tuning.py
+-rw-r--r--   0        0        0    25810 2024-04-16 18:44:22.543572 scale_egp-1.1.6/scale_egp/sdk/collections/knowledge_bases.py
+-rw-r--r--   0        0        0     2685 2024-04-16 18:44:22.543572 scale_egp-1.1.6/scale_egp/sdk/collections/model_groups.py
+-rw-r--r--   0        0        0     4798 2024-04-16 18:44:22.543572 scale_egp-1.1.6/scale_egp/sdk/collections/model_templates.py
+-rw-r--r--   0        0        0     7572 2024-04-16 18:44:22.543572 scale_egp-1.1.6/scale_egp/sdk/collections/models.py
+-rw-r--r--   0        0        0     1862 2024-04-16 18:44:22.543572 scale_egp-1.1.6/scale_egp/sdk/collections/question_sets.py
+-rw-r--r--   0        0        0     2588 2024-04-16 18:44:22.543572 scale_egp-1.1.6/scale_egp/sdk/collections/questions.py
+-rw-r--r--   0        0        0     1510 2024-04-16 18:44:22.543572 scale_egp-1.1.6/scale_egp/sdk/collections/users.py
+-rw-r--r--   0        0        0        0 2024-04-16 18:44:22.543572 scale_egp-1.1.6/scale_egp/sdk/constants/__init__.py
+-rw-r--r--   0        0        0      762 2024-04-16 18:44:22.543572 scale_egp-1.1.6/scale_egp/sdk/constants/model_schemas.py
+-rw-r--r--   0        0        0     9257 2024-04-16 18:44:22.539571 scale_egp-1.1.6/scale_egp/sdk/enums.py
+-rw-r--r--   0        0        0        0 2024-04-16 18:44:22.539571 scale_egp-1.1.6/scale_egp/sdk/models/__init__.py
+-rw-r--r--   0        0        0     2712 2024-04-16 18:44:22.539571 scale_egp-1.1.6/scale_egp/sdk/models/fine_tuning_jobs.py
+-rw-r--r--   0        0        0     2069 2024-04-16 18:44:22.539571 scale_egp-1.1.6/scale_egp/sdk/models/model_enums.py
+-rw-r--r--   0        0        0     8403 2024-04-16 18:44:22.539571 scale_egp-1.1.6/scale_egp/sdk/models/model_vendor_configuration.py
+-rw-r--r--   0        0        0      647 2024-04-16 18:44:22.539571 scale_egp-1.1.6/scale_egp/sdk/types/__init__.py
+-rw-r--r--   0        0        0     4651 2024-04-16 18:44:22.539571 scale_egp-1.1.6/scale_egp/sdk/types/agents.py
+-rw-r--r--   0        0        0      741 2024-04-16 18:44:22.543572 scale_egp-1.1.6/scale_egp/sdk/types/application_specs.py
+-rw-r--r--   0        0        0     6125 2024-04-16 18:44:22.543572 scale_egp-1.1.6/scale_egp/sdk/types/chunks.py
+-rw-r--r--   0        0        0     6553 2024-04-16 18:44:22.543572 scale_egp-1.1.6/scale_egp/sdk/types/completions.py
+-rw-r--r--   0        0        0     1016 2024-04-16 18:44:22.543572 scale_egp-1.1.6/scale_egp/sdk/types/embeddings.py
+-rw-r--r--   0        0        0     1019 2024-04-16 18:44:22.543572 scale_egp-1.1.6/scale_egp/sdk/types/evaluation_configs.py
+-rw-r--r--   0        0        0     3170 2024-04-16 18:44:22.543572 scale_egp-1.1.6/scale_egp/sdk/types/evaluation_dataset_test_cases.py
+-rw-r--r--   0        0        0     1686 2024-04-16 18:44:22.543572 scale_egp-1.1.6/scale_egp/sdk/types/evaluation_datasets.py
+-rw-r--r--   0        0        0     4837 2024-04-16 18:44:22.543572 scale_egp-1.1.6/scale_egp/sdk/types/evaluation_test_case_results.py
+-rw-r--r--   0        0        0     1398 2024-04-16 18:44:22.543572 scale_egp-1.1.6/scale_egp/sdk/types/evaluations.py
+-rw-r--r--   0        0        0     3401 2024-04-16 18:44:22.543572 scale_egp-1.1.6/scale_egp/sdk/types/fine_tuning.py
+-rw-r--r--   0        0        0     1860 2024-04-16 18:44:22.543572 scale_egp-1.1.6/scale_egp/sdk/types/knowledge_base_artifacts.py
+-rw-r--r--   0        0        0     1559 2024-04-16 18:44:22.543572 scale_egp-1.1.6/scale_egp/sdk/types/knowledge_base_chunks.py
+-rw-r--r--   0        0        0    15686 2024-04-16 18:44:22.543572 scale_egp-1.1.6/scale_egp/sdk/types/knowledge_base_uploads.py
+-rw-r--r--   0        0        0     1863 2024-04-16 18:44:22.543572 scale_egp-1.1.6/scale_egp/sdk/types/knowledge_bases.py
+-rw-r--r--   0        0        0     1112 2024-04-16 18:44:22.543572 scale_egp-1.1.6/scale_egp/sdk/types/memory_strategy.py
+-rw-r--r--   0        0        0     2478 2024-04-16 18:44:22.543572 scale_egp-1.1.6/scale_egp/sdk/types/message.py
+-rw-r--r--   0        0        0     3557 2024-04-16 18:44:22.543572 scale_egp-1.1.6/scale_egp/sdk/types/model_templates.py
+-rw-r--r--   0        0        0    14065 2024-04-16 18:44:22.543572 scale_egp-1.1.6/scale_egp/sdk/types/models.py
+-rw-r--r--   0        0        0     1086 2024-04-16 18:44:22.543572 scale_egp-1.1.6/scale_egp/sdk/types/models_group.py
+-rw-r--r--   0        0        0      891 2024-04-16 18:44:22.543572 scale_egp-1.1.6/scale_egp/sdk/types/question_sets.py
+-rw-r--r--   0        0        0     5234 2024-04-16 18:44:22.543572 scale_egp-1.1.6/scale_egp/sdk/types/questions.py
+-rw-r--r--   0        0        0      410 2024-04-16 18:44:22.543572 scale_egp-1.1.6/scale_egp/sdk/types/user_info.py
+-rw-r--r--   0        0        0        0 2024-04-16 18:44:22.543572 scale_egp-1.1.6/scale_egp/utils/__init__.py
+-rw-r--r--   0        0        0    11461 2024-04-16 18:44:22.543572 scale_egp-1.1.6/scale_egp/utils/api_utils.py
+-rw-r--r--   0        0        0     3639 2024-04-16 18:44:22.543572 scale_egp-1.1.6/scale_egp/utils/model_utils.py
+-rw-r--r--   0        0        0      107 2024-04-16 18:44:22.543572 scale_egp-1.1.6/scale_egp/utils/strenum_compat.py
+-rw-r--r--   0        0        0    18869 1970-01-01 00:00:00.000000 scale_egp-1.1.6/PKG-INFO
```

### Comparing `scale_egp-1.1.5/README.md` & `scale_egp-1.1.6/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 import questionary as q
 
 from scale_egp.sdk.client import EGPClient
 from scale_egp.sdk.enums import (
     CrossEncoderModelName,
     EmbeddingModelName,
-    ExtraInfoSchema,
+    ExtraInfoSchemaType,
     TestCaseSchemaType,
     EvaluationType,
 )
 from scale_egp.sdk.types.chunks import CrossEncoderRankParams, CrossEncoderRankStrategy,
 
 RougeRankStrategy
 RougeRankParams
@@ -79,17 +79,17 @@
             chunk_string += re_ranked_top_3_chunk.text + "\n"
             chunk_string += "\n"
 
         rag_prompt = f"{input_prompt}\n\nAdditional information:\n{chunk_string}"
         completion = client.completions().create(model=self.llm_model, prompt=rag_prompt)
         output = completion.completion.text
 
-        extra_info = ExtraInfo(
+        extra_info = StringExtraInfo(
             info=chunk_string,
-            schema_type=ExtraInfoSchema.STRING,
+            schema_type=ExtraInfoSchemaType.STRING,
         )
         return output, extra_info
 
     def generate_chunks(
         self, query: str, initial_recall: int = 10, rouge_recall: int = 5, top_k: int = 3
     ):
         chunks = client.knowledge_bases().query(
```

### Comparing `scale_egp-1.1.5/pyproject.toml` & `scale_egp-1.1.6/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "scale-egp"
-version = "1.1.5"
+version = "1.1.6"
 description = "SDK for Scale SGP API"
 license = "Apache 2.0 modified with Commons Clause"
 authors = ["Scale SGP team"]
 readme = "README.md"
 homepage = "https://scaleapi.github.io/sgp-py/"
 repository = "https://github.com/scaleapi/egp-py"
 packages = [{include = "scale_egp"}]
@@ -25,15 +25,15 @@
 mock = "^4.0.3"
 
 [tool.poetry.scripts]
 scale-egp = "scale_egp.cli.cli_main:exec_cli"
 
 [tool.poetry.dev-dependencies]
 pytest = ">=7.4"
-pylint = ">=2.5"
+pylint = "2.17.7"
 black = ">=21.12b0"
 mypy = ">=1.6.1"
 mypy-extensions = ">=1.0.0"
 types-requests = ">=2.31.0"
 python-dotenv = "1.0.0"
 questionary = ">=1.0.0,<3.0"
 twine = "4.0.2"
```

### Comparing `scale_egp-1.1.5/scale_egp/cli/cli_main.py` & `scale_egp-1.1.6/scale_egp/cli/cli_main.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.5/scale_egp/cli/collections.py` & `scale_egp-1.1.6/scale_egp/cli/collections.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.5/scale_egp/cli/formatter.py` & `scale_egp-1.1.6/scale_egp/cli/formatter.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.5/scale_egp/cli/model_instance_description.py` & `scale_egp-1.1.6/scale_egp/cli/model_instance_description.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.5/scale_egp/cli/parser.py` & `scale_egp-1.1.6/scale_egp/cli/parser.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.5/scale_egp/exceptions.py` & `scale_egp-1.1.6/scale_egp/exceptions.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.5/scale_egp/sdk/client.py` & `scale_egp-1.1.6/scale_egp/sdk/client.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.5/scale_egp/sdk/collections/application_specs.py` & `scale_egp-1.1.6/scale_egp/sdk/collections/application_specs.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.5/scale_egp/sdk/collections/chunks.py` & `scale_egp-1.1.6/scale_egp/sdk/collections/chunks.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.5/scale_egp/sdk/collections/completions.py` & `scale_egp-1.1.6/scale_egp/sdk/collections/completions.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.5/scale_egp/sdk/collections/evaluation_configs.py` & `scale_egp-1.1.6/scale_egp/sdk/collections/evaluation_configs.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.5/scale_egp/sdk/collections/evaluation_datasets.py` & `scale_egp-1.1.6/scale_egp/sdk/collections/evaluation_datasets.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.5/scale_egp/sdk/collections/evaluations.py` & `scale_egp-1.1.6/scale_egp/sdk/collections/evaluations.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.5/scale_egp/sdk/collections/fine_tuning.py` & `scale_egp-1.1.6/scale_egp/sdk/collections/fine_tuning.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.5/scale_egp/sdk/collections/knowledge_bases.py` & `scale_egp-1.1.6/scale_egp/sdk/collections/knowledge_bases.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.5/scale_egp/sdk/collections/model_groups.py` & `scale_egp-1.1.6/scale_egp/sdk/collections/model_groups.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.5/scale_egp/sdk/collections/model_templates.py` & `scale_egp-1.1.6/scale_egp/sdk/collections/model_templates.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.5/scale_egp/sdk/collections/models.py` & `scale_egp-1.1.6/scale_egp/sdk/collections/models.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.5/scale_egp/sdk/collections/question_sets.py` & `scale_egp-1.1.6/scale_egp/sdk/collections/question_sets.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.5/scale_egp/sdk/collections/questions.py` & `scale_egp-1.1.6/scale_egp/sdk/collections/questions.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.5/scale_egp/sdk/collections/users.py` & `scale_egp-1.1.6/scale_egp/sdk/collections/users.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.5/scale_egp/sdk/constants/model_schemas.py` & `scale_egp-1.1.6/scale_egp/sdk/constants/model_schemas.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.5/scale_egp/sdk/enums.py` & `scale_egp-1.1.6/scale_egp/sdk/enums.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,25 +78,26 @@
         FREE_TEXT: Denotes that a question is a free text question.
     """
 
     CATEGORICAL: str = "categorical"
     FREE_TEXT: str = "free_text"
 
 
-class ExtraInfoSchema(str, Enum):
+class ExtraInfoSchemaType(str, Enum):
     """
     An enum representing the different types of extra info schemas.
 
     Denotes the type of the "info" field in the ExtraInfo model.
 
     Attributes:
         STRING: Denotes that the "info" field is a string.
     """
 
     STRING: str = "STRING"
+    CHUNKS: str = "CHUNKS"
 
 
 class EmbeddingModelName(str, Enum):
     """
     An enum representing the different types of embedding models supported.
 
     Attributes:
@@ -131,14 +132,15 @@
     OPENAI_TEXT_EMBEDDING_3_SMALL = "openai/text-embedding-3-small"
     OPENAI_TEXT_EMBEDDING_3_LARGE = "openai/text-embedding-3-large"
     SENTENCE_TRANSFORMERS_MULTI_QA_FINETUNE = "finetuned/multi-qa-mpnet-base-dot-v1"
     COHERE_TEXT_EMBEDDING_ENGLISH_3 = "embed-english-v3.0"
     COHERE_TEXT_EMBEDDING_ENGLISH_LIGHT_3 = "embed-english-light-v3.0"
     COHERE_TEXT_EMBEDDING_MULTILINGUAL_3 = "embed-multilingual-v3.0"
 
+
 class DataSource(str, Enum):
     """
     An enum representing the different types of data sources supported.
 
     Attributes:
         S3: Denotes that the data source is S3.
     """
```

### Comparing `scale_egp-1.1.5/scale_egp/sdk/models/fine_tuning_jobs.py` & `scale_egp-1.1.6/scale_egp/sdk/models/fine_tuning_jobs.py`

 * *Files 9% similar despite different names*

```diff
@@ -29,24 +29,34 @@
     vendor: Literal[ModelVendor.LAUNCH] = Field(ModelVendor.LAUNCH)
     hyperparameters: Optional[Dict[str, Any]]
     wandb_config: Optional[Dict[str, Any]]
     suffix: Optional[str]
     output: Optional[str]
 
 
+class LLMEngineFineTuningJobConfiguration(BaseModel):
+    vendor: Literal[ModelVendor.LLMENGINE] = Field(ModelVendor.LLMENGINE)
+    hyperparameters: Optional[Dict[str, Any]]
+    wandb_config: Optional[Dict[str, Any]]
+    suffix: Optional[str]
+    output: Optional[str]
+
+
 class OpenAIFineTuningJobConfiguration(BaseModel):
     vendor: Literal[ModelVendor.OPENAI] = Field(ModelVendor.OPENAI)
     hyperparameters: Optional[Dict[str, Any]]
     suffix: Optional[str]
 
 
 class FineTuningJobVendorConfiguration(RootModel):
-    __root__: Union[LaunchFineTuningJobConfiguration, OpenAIFineTuningJobConfiguration] = Field(
-        ..., discriminator="vendor"
-    )
+    __root__: Union[
+        LaunchFineTuningJobConfiguration,
+        LLMEngineFineTuningJobConfiguration,
+        OpenAIFineTuningJobConfiguration,
+    ] = Field(..., discriminator="vendor")
 
 
 class FineTuningJobEvent(BaseModel):
     timestamp: Optional[float]
     message: str
     level: str
```

### Comparing `scale_egp-1.1.5/scale_egp/sdk/models/model_enums.py` & `scale_egp-1.1.6/scale_egp/sdk/models/model_enums.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.5/scale_egp/sdk/models/model_vendor_configuration.py` & `scale_egp-1.1.6/scale_egp/sdk/models/model_vendor_configuration.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.5/scale_egp/sdk/types/__init__.py` & `scale_egp-1.1.6/scale_egp/sdk/types/__init__.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.5/scale_egp/sdk/types/agents.py` & `scale_egp-1.1.6/scale_egp/sdk/types/agents.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.5/scale_egp/sdk/types/application_specs.py` & `scale_egp-1.1.6/scale_egp/sdk/types/application_specs.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.5/scale_egp/sdk/types/chunks.py` & `scale_egp-1.1.6/scale_egp/sdk/types/chunks.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.5/scale_egp/sdk/types/completions.py` & `scale_egp-1.1.6/scale_egp/sdk/types/completions.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.5/scale_egp/sdk/types/embeddings.py` & `scale_egp-1.1.6/scale_egp/sdk/types/embeddings.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.5/scale_egp/sdk/types/evaluation_configs.py` & `scale_egp-1.1.6/scale_egp/sdk/types/evaluation_configs.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.5/scale_egp/sdk/types/evaluation_dataset_test_cases.py` & `scale_egp-1.1.6/scale_egp/sdk/types/evaluation_dataset_test_cases.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,56 +1,45 @@
 from __future__ import annotations
 
-from typing import Optional, Dict, Any, Union
+from typing import Optional, Dict, Any, Union, List, Literal
 
 from pydantic import Field, validator, ValidationError
 
-from scale_egp.sdk.enums import TestCaseSchemaType, ExtraInfoSchema
-from scale_egp.utils.model_utils import Entity, BaseModel
+from scale_egp.sdk.enums import TestCaseSchemaType, ExtraInfoSchemaType
+from scale_egp.utils.model_utils import Entity, BaseModel, RootModel
 
 
-class ExtraInfo(BaseModel):
-    """
-    A data model representing the extra info of a generation model.
-
-    Attributes:
-        schema_type: The schema type of the extra info
-        info: The content of the extra info. This must match the schema type.
-    """
+class ChunkData(BaseModel):
+    text: str
+    metadata: Dict[str, Any]
 
-    schema_type: ExtraInfoSchema
+class StringExtraInfo(BaseModel):
+    schema_type: Literal[ExtraInfoSchemaType.STRING] = ExtraInfoSchemaType.STRING
     info: str
 
-    @validator("info")
-    def info_matches_schema_type(cls, info, values):
-        schema_type = values.get("schema_type")
-        if schema_type == ExtraInfoSchema.STRING:
-            if not isinstance(info, str):
-                raise ValueError("schema_type STRING requires info to be a string")
-        else:
-            raise ValueError(f"Unknown schema_type: {schema_type}")
-        return info
+class ChunksExtraInfo(BaseModel):
+    schema_type: Literal[ExtraInfoSchemaType.CHUNKS] = ExtraInfoSchemaType.CHUNKS
+    chunks: List[ChunkData]
 
+class ExtraInfo(RootModel):
+    __root__: Union[StringExtraInfo, ChunksExtraInfo] = Field(..., discriminator="schema_type")
 
 class GenerationTestCaseData(BaseModel):
     """
     A data model representing the data of a Testcase with a GENERATION schema type.
 
     Attributes:
         input: The input to the generation model
         expected_output: The expected output of the generation model
         expected_extra_info: The expected extra info of the generation model
     """
 
     input: str
     expected_output: Optional[str] = ""
-    expected_extra_info: Optional[ExtraInfo] = ExtraInfo(
-        schema_type=ExtraInfoSchema.STRING,
-        info="",
-    )
+    expected_extra_info: Optional[ExtraInfo]
 
 
 class TestCase(Entity):
     """
     A data model representing a test case.
 
     Attributes:
@@ -68,15 +57,15 @@
 
 
 class TestCaseRequest(BaseModel):
     schema_type: TestCaseSchemaType
     test_case_data: Union[GenerationTestCaseData]
     account_id: Optional[str] = Field(
         description="Account to create knowledge base in. If you have access to more than one "
-                    "account, you must specify an account_id"
+        "account, you must specify an account_id"
     )
 
     @validator("test_case_data")
     @classmethod
     def test_case_data_matches_schema_type(cls, test_case_data, values):
         schema_type = values.get("schema_type")
         TestCaseSchemaValidator.validate(schema_type, test_case_data)
```

### Comparing `scale_egp-1.1.5/scale_egp/sdk/types/evaluation_datasets.py` & `scale_egp-1.1.6/scale_egp/sdk/types/evaluation_datasets.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.5/scale_egp/sdk/types/evaluation_test_case_results.py` & `scale_egp-1.1.6/scale_egp/sdk/types/evaluation_test_case_results.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,29 +3,29 @@
 from datetime import datetime
 from typing import Optional, Dict, Any
 from warnings import warn
 
 from pydantic import ValidationError, Field, validator
 
 from scale_egp.sdk.enums import EvaluationStatus, TestCaseSchemaType
-from scale_egp.sdk.types.evaluation_dataset_test_cases import ExtraInfo
+from scale_egp.sdk.types.evaluation_dataset_test_cases import (ExtraInfo, StringExtraInfo, ExtraInfoSchemaType)
 from scale_egp.utils.model_utils import Entity, BaseModel
 
 
 class GenerationTestCaseResultData(BaseModel):
     """
     A data model representing the data of a TestcaseResult with a GENERATION schema type.
 
     Attributes:
         generation_output: The output of the generation model
         generation_extra_info: The extra info of the generation model
     """
 
     generation_output: str
-    generation_extra_info: Optional[ExtraInfo] = None
+    generation_extra_info: ExtraInfo = StringExtraInfo(schema_type=ExtraInfoSchemaType.STRING, info="")
 
 
 class TestCaseResult(Entity):
     """
     A data model representing a test case result.
 
     Attributes:
```

### Comparing `scale_egp-1.1.5/scale_egp/sdk/types/evaluations.py` & `scale_egp-1.1.6/scale_egp/sdk/types/evaluations.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.5/scale_egp/sdk/types/fine_tuning.py` & `scale_egp-1.1.6/scale_egp/sdk/types/fine_tuning.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # !!!!! DO NOT EVER CHANGE THIS FILE MANUALLY -- AUTOGENERATED by orm2pydantic.py !!!!!
-# Generated on 2024-04-08 from module egp_api_backend.server.internal.orm.orm_fine_tuning_jobs in the egp-api-backend package for use in the EGP python SDK
+# Generated on 2024-04-09 from module egp_api_backend.server.internal.orm.orm_fine_tuning_jobs in the egp-api-backend package for use in the EGP python SDK
 # To regenerate this file, run:
 # scaleapi/packages/egp-api-backend/scripts/orm2pydantic.sh
 
 from scale_egp.utils.model_utils import BaseModel, Entity
 from pydantic import Field
 
 from datetime import (datetime)
```

### Comparing `scale_egp-1.1.5/scale_egp/sdk/types/knowledge_base_artifacts.py` & `scale_egp-1.1.6/scale_egp/sdk/types/knowledge_base_artifacts.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.5/scale_egp/sdk/types/knowledge_base_chunks.py` & `scale_egp-1.1.6/scale_egp/sdk/types/knowledge_base_chunks.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.5/scale_egp/sdk/types/knowledge_base_uploads.py` & `scale_egp-1.1.6/scale_egp/sdk/types/knowledge_base_uploads.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.5/scale_egp/sdk/types/knowledge_bases.py` & `scale_egp-1.1.6/scale_egp/sdk/types/knowledge_bases.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.5/scale_egp/sdk/types/memory_strategy.py` & `scale_egp-1.1.6/scale_egp/sdk/types/memory_strategy.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.5/scale_egp/sdk/types/message.py` & `scale_egp-1.1.6/scale_egp/sdk/types/message.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.5/scale_egp/sdk/types/model_templates.py` & `scale_egp-1.1.6/scale_egp/sdk/types/model_templates.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.5/scale_egp/sdk/types/models.py` & `scale_egp-1.1.6/scale_egp/sdk/types/models.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.5/scale_egp/sdk/types/models_group.py` & `scale_egp-1.1.6/scale_egp/sdk/types/models_group.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.5/scale_egp/sdk/types/question_sets.py` & `scale_egp-1.1.6/scale_egp/sdk/types/question_sets.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.5/scale_egp/sdk/types/questions.py` & `scale_egp-1.1.6/scale_egp/sdk/types/questions.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.5/scale_egp/utils/api_utils.py` & `scale_egp-1.1.6/scale_egp/utils/api_utils.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.5/scale_egp/utils/model_utils.py` & `scale_egp-1.1.6/scale_egp/utils/model_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 Create partial model definitions, sort of like Partial<> in TypeScript
 
 Sources:
 https://github.com/pydantic/pydantic/issues/3120#issuecomment-1528030416
 https://stackoverflow.com/a/76560886
 """
+
 from copy import deepcopy
 from typing import Any, Dict, Optional, TypeVar, Type
 
 from pydantic import Extra, create_model, BaseModel as PydanticBaseModel, Field
 from pydantic.fields import ModelField
 
 # pylint: disable=missing-function-docstring
@@ -62,14 +63,17 @@
         arbitrary_types_allowed = True
 
 
 class RootModel(BaseModel):
     def __getattr__(self, name):
         return self.__root__.__getattribute__(name)
 
+    def __setattr__(self, name, value):
+        return self.__root__.__setattr__(name, value)
+
 
 def make_field_optional(field: ModelField, default: Any = None) -> ModelField:
     new = deepcopy(field)
     new.default = default
     new.required = False
     new.annotation = Optional[field.annotation]  # type: ignore
     return new
@@ -114,14 +118,16 @@
 
 
 class Entity(BaseModel):
     """
     Base class for all entities
     """
 
+
 class RootEntity(RootModel):
     """
     Root class for union type entities
     """
 
+
 class hiddenstr(str):
     pass
```

### Comparing `scale_egp-1.1.5/PKG-INFO` & `scale_egp-1.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scale-egp
-Version: 1.1.5
+Version: 1.1.6
 Summary: SDK for Scale SGP API
 Home-page: https://scaleapi.github.io/sgp-py/
 License: Apache 2.0 modified with Commons Clause
 Author: Scale SGP team
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -52,15 +52,15 @@
 
 import questionary as q
 
 from scale_egp.sdk.client import EGPClient
 from scale_egp.sdk.enums import (
     CrossEncoderModelName,
     EmbeddingModelName,
-    ExtraInfoSchema,
+    ExtraInfoSchemaType,
     TestCaseSchemaType,
     EvaluationType,
 )
 from scale_egp.sdk.types.chunks import CrossEncoderRankParams, CrossEncoderRankStrategy,
 
 RougeRankStrategy
 RougeRankParams
@@ -105,17 +105,17 @@
             chunk_string += re_ranked_top_3_chunk.text + "\n"
             chunk_string += "\n"
 
         rag_prompt = f"{input_prompt}\n\nAdditional information:\n{chunk_string}"
         completion = client.completions().create(model=self.llm_model, prompt=rag_prompt)
         output = completion.completion.text
 
-        extra_info = ExtraInfo(
+        extra_info = StringExtraInfo(
             info=chunk_string,
-            schema_type=ExtraInfoSchema.STRING,
+            schema_type=ExtraInfoSchemaType.STRING,
         )
         return output, extra_info
 
     def generate_chunks(
         self, query: str, initial_recall: int = 10, rouge_recall: int = 5, top_k: int = 3
     ):
         chunks = client.knowledge_bases().query(
```

