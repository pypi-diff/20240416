# Comparing `tmp/ogbujipt-0.7.1.tar.gz` & `tmp/ogbujipt-0.8.0.tar.gz`

## Comparing `ogbujipt-0.7.1.tar` & `ogbujipt-0.8.0.tar`

### file list

```diff
@@ -1,55 +1,56 @@
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 ogbujipt-0.7.1/.coveragerc
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 ogbujipt-0.7.1/.flake8
--rw-r--r--   0        0        0     5322 2020-02-02 00:00:00.000000 ogbujipt-0.7.1/CHANGELOG.md
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 ogbujipt-0.7.1/requirements-pgvector.txt
--rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 ogbujipt-0.7.1/.github/workflows/main.yml
--rw-r--r--   0        0        0    32610 2020-02-02 00:00:00.000000 ogbujipt-0.7.1/demo/PGvector_demo.ipynb
--rw-r--r--   0        0        0     4580 2020-02-02 00:00:00.000000 ogbujipt-0.7.1/demo/README.md
--rw-r--r--   0        0        0    13598 2020-02-02 00:00:00.000000 ogbujipt-0.7.1/demo/chat_pdf_streamlit_ui.py
--rw-r--r--   0        0        0     8212 2020-02-02 00:00:00.000000 ogbujipt-0.7.1/demo/chat_web_selects.py
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 ogbujipt-0.7.1/demo/demo.env
--rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 ogbujipt-0.7.1/demo/function_calling.py
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 ogbujipt-0.7.1/demo/language.toml
--rw-r--r--   0        0        0     4379 2020-02-02 00:00:00.000000 ogbujipt-0.7.1/demo/multiprocess.py
--rw-r--r--   0        0        0     3833 2020-02-02 00:00:00.000000 ogbujipt-0.7.1/demo/qa_discord.py
--rw-r--r--   0        0        0     3294 2020-02-02 00:00:00.000000 ogbujipt-0.7.1/demo/simple_fix_xml.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 ogbujipt-0.7.1/ogbujipt/__about__.py
--rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 ogbujipt-0.7.1/ogbujipt/__init__.py
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 ogbujipt-0.7.1/ogbujipt/async_helper.py
--rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 ogbujipt-0.7.1/ogbujipt/config.py
--rw-r--r--   0        0        0    14073 2020-02-02 00:00:00.000000 ogbujipt-0.7.1/ogbujipt/llm_wrapper.py
--rw-r--r--   0        0        0     5276 2020-02-02 00:00:00.000000 ogbujipt-0.7.1/ogbujipt/text_helper.py
--rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 ogbujipt-0.7.1/ogbujipt/word_loom.py
--rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 ogbujipt-0.7.1/ogbujipt/embedding/__init__.py
--rw-r--r--   0        0        0     7231 2020-02-02 00:00:00.000000 ogbujipt-0.7.1/ogbujipt/embedding/pgvector.py
--rw-r--r--   0        0        0    15497 2020-02-02 00:00:00.000000 ogbujipt-0.7.1/ogbujipt/embedding/pgvector_data_doc.py
--rw-r--r--   0        0        0    10375 2020-02-02 00:00:00.000000 ogbujipt-0.7.1/ogbujipt/embedding/pgvector_message.py
--rw-r--r--   0        0        0     8376 2020-02-02 00:00:00.000000 ogbujipt-0.7.1/ogbujipt/embedding/qdrant.py
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 ogbujipt-0.7.1/ogbujipt/prompting/__init__.py
--rwxr-xr-x   0        0        0     4579 2020-02-02 00:00:00.000000 ogbujipt-0.7.1/ogbujipt/prompting/basic.py
--rwxr-xr-x   0        0        0     5803 2020-02-02 00:00:00.000000 ogbujipt-0.7.1/ogbujipt/prompting/model_style.py
--rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 ogbujipt-0.7.1/ogbujipt/resources/wordloom/sample.toml
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 ogbujipt-0.7.1/test/__init__.py
--rw-r--r--   0        0        0     8324 2020-02-02 00:00:00.000000 ogbujipt-0.7.1/test/conftest.py
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 ogbujipt-0.7.1/test/test_config.py
--rw-r--r--   0        0        0     2546 2020-02-02 00:00:00.000000 ogbujipt-0.7.1/test/test_llm_wrapper.py
--rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 ogbujipt-0.7.1/test/test_model_style.py
--rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 ogbujipt-0.7.1/test/test_ogbujipt.py
--rw-r--r--   0        0        0     4938 2020-02-02 00:00:00.000000 ogbujipt-0.7.1/test/test_text_splitter.py
--rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 ogbujipt-0.7.1/test/test_word_loom.py
--rw-r--r--   0        0        0     8124 2020-02-02 00:00:00.000000 ogbujipt-0.7.1/test/embedding/conftest.py
--rw-r--r--   0        0        0     3459 2020-02-02 00:00:00.000000 ogbujipt-0.7.1/test/embedding/test_pgvector_data.py
--rw-r--r--   0        0        0     6943 2020-02-02 00:00:00.000000 ogbujipt-0.7.1/test/embedding/test_pgvector_doc.py
--rw-r--r--   0        0        0     5048 2020-02-02 00:00:00.000000 ogbujipt-0.7.1/test/embedding/test_pgvector_message.py
--rw-r--r--   0        0        0     2717 2020-02-02 00:00:00.000000 ogbujipt-0.7.1/test/embedding/test_qdrant.py
--rwxr-xr-x   0        0        0     1696 2020-02-02 00:00:00.000000 ogbujipt-0.7.1/test/test_prompts/test_airoboros_obedient_prompting.py
--rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 ogbujipt-0.7.1/test/test_prompts/test_alpaca_prompting.py
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 ogbujipt-0.7.1/test/test_prompts/test_orca_prompting.py
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 ogbujipt-0.7.1/test/test_prompts/test_vicuña_prompting.py
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 ogbujipt-0.7.1/util/constraints-apple-silicon.txt
--rw-r--r--   0        0        0    14139 2020-02-02 00:00:00.000000 ogbujipt-0.7.1/util/download-model.py
--rw-r--r--   0        0        0     3211 2020-02-02 00:00:00.000000 ogbujipt-0.7.1/.gitignore
--rw-r--r--   0        0        0    11339 2020-02-02 00:00:00.000000 ogbujipt-0.7.1/LICENSE
--rw-r--r--   0        0        0     8683 2020-02-02 00:00:00.000000 ogbujipt-0.7.1/README.md
--rw-r--r--   0        0        0     3779 2020-02-02 00:00:00.000000 ogbujipt-0.7.1/pyproject.toml
--rw-r--r--   0        0        0     9792 2020-02-02 00:00:00.000000 ogbujipt-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 ogbujipt-0.8.0/.coveragerc
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 ogbujipt-0.8.0/.flake8
+-rw-r--r--   0        0        0     5672 2020-02-02 00:00:00.000000 ogbujipt-0.8.0/CHANGELOG.md
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 ogbujipt-0.8.0/requirements-pgvector.txt
+-rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 ogbujipt-0.8.0/.github/workflows/main.yml
+-rw-r--r--   0        0        0    32610 2020-02-02 00:00:00.000000 ogbujipt-0.8.0/demo/PGvector_demo.ipynb
+-rw-r--r--   0        0        0     4580 2020-02-02 00:00:00.000000 ogbujipt-0.8.0/demo/README.md
+-rw-r--r--   0        0        0    13594 2020-02-02 00:00:00.000000 ogbujipt-0.8.0/demo/chat_pdf_streamlit_ui.py
+-rw-r--r--   0        0        0     8277 2020-02-02 00:00:00.000000 ogbujipt-0.8.0/demo/chat_web_selects.py
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 ogbujipt-0.8.0/demo/demo.env
+-rw-r--r--   0        0        0     1971 2020-02-02 00:00:00.000000 ogbujipt-0.8.0/demo/function_calling.py
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 ogbujipt-0.8.0/demo/language.toml
+-rw-r--r--   0        0        0     4323 2020-02-02 00:00:00.000000 ogbujipt-0.8.0/demo/multiprocess.py
+-rw-r--r--   0        0        0     3820 2020-02-02 00:00:00.000000 ogbujipt-0.8.0/demo/qa_discord.py
+-rw-r--r--   0        0        0     3259 2020-02-02 00:00:00.000000 ogbujipt-0.8.0/demo/simple_fix_xml.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 ogbujipt-0.8.0/ogbujipt/__about__.py
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 ogbujipt-0.8.0/ogbujipt/__init__.py
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 ogbujipt-0.8.0/ogbujipt/async_helper.py
+-rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 ogbujipt-0.8.0/ogbujipt/config.py
+-rw-r--r--   0        0        0    24218 2020-02-02 00:00:00.000000 ogbujipt-0.8.0/ogbujipt/llm_wrapper.py
+-rw-r--r--   0        0        0     5276 2020-02-02 00:00:00.000000 ogbujipt-0.8.0/ogbujipt/text_helper.py
+-rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 ogbujipt-0.8.0/ogbujipt/word_loom.py
+-rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 ogbujipt-0.8.0/ogbujipt/embedding/__init__.py
+-rw-r--r--   0        0        0     7231 2020-02-02 00:00:00.000000 ogbujipt-0.8.0/ogbujipt/embedding/pgvector.py
+-rw-r--r--   0        0        0    14846 2020-02-02 00:00:00.000000 ogbujipt-0.8.0/ogbujipt/embedding/pgvector_data_doc.py
+-rw-r--r--   0        0        0    14677 2020-02-02 00:00:00.000000 ogbujipt-0.8.0/ogbujipt/embedding/pgvector_message.py
+-rw-r--r--   0        0        0     7900 2020-02-02 00:00:00.000000 ogbujipt-0.8.0/ogbujipt/embedding/qdrant.py
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 ogbujipt-0.8.0/ogbujipt/prompting/__init__.py
+-rwxr-xr-x   0        0        0     4579 2020-02-02 00:00:00.000000 ogbujipt-0.8.0/ogbujipt/prompting/basic.py
+-rwxr-xr-x   0        0        0     5803 2020-02-02 00:00:00.000000 ogbujipt-0.8.0/ogbujipt/prompting/model_style.py
+-rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 ogbujipt-0.8.0/ogbujipt/resources/wordloom/sample.toml
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 ogbujipt-0.8.0/test/__init__.py
+-rw-r--r--   0        0        0     8324 2020-02-02 00:00:00.000000 ogbujipt-0.8.0/test/conftest.py
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 ogbujipt-0.8.0/test/test_config.py
+-rw-r--r--   0        0        0     5680 2020-02-02 00:00:00.000000 ogbujipt-0.8.0/test/test_llm_wrapper.py
+-rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 ogbujipt-0.8.0/test/test_model_style.py
+-rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 ogbujipt-0.8.0/test/test_ogbujipt.py
+-rw-r--r--   0        0        0     4938 2020-02-02 00:00:00.000000 ogbujipt-0.8.0/test/test_text_splitter.py
+-rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 ogbujipt-0.8.0/test/test_word_loom.py
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 ogbujipt-0.8.0/test/embedding/README.md
+-rw-r--r--   0        0        0     9786 2020-02-02 00:00:00.000000 ogbujipt-0.8.0/test/embedding/conftest.py
+-rw-r--r--   0        0        0     3616 2020-02-02 00:00:00.000000 ogbujipt-0.8.0/test/embedding/test_pgvector_data.py
+-rw-r--r--   0        0        0     6454 2020-02-02 00:00:00.000000 ogbujipt-0.8.0/test/embedding/test_pgvector_doc.py
+-rw-r--r--   0        0        0     8066 2020-02-02 00:00:00.000000 ogbujipt-0.8.0/test/embedding/test_pgvector_message.py
+-rw-r--r--   0        0        0     2717 2020-02-02 00:00:00.000000 ogbujipt-0.8.0/test/embedding/test_qdrant.py
+-rwxr-xr-x   0        0        0     1696 2020-02-02 00:00:00.000000 ogbujipt-0.8.0/test/test_prompts/test_airoboros_obedient_prompting.py
+-rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 ogbujipt-0.8.0/test/test_prompts/test_alpaca_prompting.py
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 ogbujipt-0.8.0/test/test_prompts/test_orca_prompting.py
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 ogbujipt-0.8.0/test/test_prompts/test_vicuña_prompting.py
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 ogbujipt-0.8.0/util/constraints-apple-silicon.txt
+-rw-r--r--   0        0        0    14139 2020-02-02 00:00:00.000000 ogbujipt-0.8.0/util/download-model.py
+-rw-r--r--   0        0        0     3211 2020-02-02 00:00:00.000000 ogbujipt-0.8.0/.gitignore
+-rw-r--r--   0        0        0    11339 2020-02-02 00:00:00.000000 ogbujipt-0.8.0/LICENSE
+-rw-r--r--   0        0        0    10630 2020-02-02 00:00:00.000000 ogbujipt-0.8.0/README.md
+-rw-r--r--   0        0        0     3779 2020-02-02 00:00:00.000000 ogbujipt-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0    11739 2020-02-02 00:00:00.000000 ogbujipt-0.8.0/PKG-INFO
```

### Comparing `ogbujipt-0.7.1/CHANGELOG.md` & `ogbujipt-0.8.0/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,52 +1,65 @@
 # Changelog
 
-Notable changes to OgbujiPT. Format based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/). Project follows [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
+Notable changes to  Format based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/). Project follows [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 <!--
 ## [Unreleased]
 -->
 
-## [0.7.1] - 20240222
+## [0.8.0] - 20240325
+
+### Added
+
+- `llm_wrapper.llama_cpp_http_chat` & `llm_wrapper.llama_cpp_http`; llama.cpp low-level HTTP API support
+- `llm_wrapper.llama_response` class with flexible handling across API specs
+- `window` init param for for `embedding.pgvector.MessageDB`, to limit message storage per history key
+
+### Changed
+
+- Deprecated `first_choice_text` & `first_choice_message` methods in favor of `first_choice_text` attributes on response objects
+- Clarify set quite setup docs
+
+## [0.7.1] - 20240229
 
 ### Added
 
 - MessageDB.get_messages() options: `since` (for retrieving messages aftter a timestamp) and `limit` (for limiting the number of messages returned, selecting the most recent)
 
 ### Changed
 
 - PGVector users now manage their own connection pool by default
 - Better modularization of embeddings test cases; using `conftest.py` more
 - `pgvector_message.py` PG table timstamp column no longer a primary key
 
 ### Fixed
 
-- Backward threshold check for ogbujipt.embedding.pgvector_data_doc.DataDB
+- Backward threshold check for embedding.pgvector_data_doc.DataDB
 
 ## [0.7.0] - 20240110
 
 ### Added
 
 - Command line options for `demo/chat_web_selects.py`
 - Helper for folks installing on Apple Silicon: `constraints-apple-silicon.txt`
 - Function calling demo
-- `ogbujipt.embedding.pgvector_message.insert_many()`
+- `embedding.pgvector_message.insert_many()`
 
 ### Changed
 
 - Improved use of PGVector helper SQL query parameters
 - PGVector helper `search(query_tags=[..])` now uses contains operator (filters by existence in tag sets), not the same as where tags are OR
 - PGVector helper `search` can now be set to work conjunctively or disjunctively
 - PGVector helper `query` now has threshold arg based on degree of similarity. `limit` default now unlimited. Use SQL query args for query_embedding.
 - `embedding.pgvector` split into a couple of modules.
 - Separated data-style PGVector DBs from doc-style. tags is no longer the final param for PGVector docs helper methods & some params renamed.
 - PGVector helper method results now as `attr_dict`
 - PGVector helper now uses connection pooling & is more multiprocess safe
-- `ogbujipt.embedding.pgvector_chat` renamed to `ogbujipt.embedding.pgvector_message`
-- DB MIGRATION REQUIRED - `ogbujipt.embedding.pgvector_message` table schema
+- `embedding.pgvector_chat` renamed to `embedding.pgvector_message`
+- DB MIGRATION REQUIRED - `embedding.pgvector_message` table schema
 
 ### Fixed
 
 - `insert_many` PGVector helper method; semantics & performance
 - `demo/chat_web_selects.py` & `demo/chat_pdf_streamlit_ui.py` (formerly non-functional)
 - Tests & CI for PGVector helper
 
@@ -127,44 +140,44 @@
 
 - test suite structure
 
 ## [0.3.0] - 20230723
 
 ### Added
 
-- `ogbujipt.__version__`
+- `__version__`
 - chat_web_selects.py demo
-- `ogbujipt.async_helper.save_openai_api_params()`
+- `async_helper.save_openai_api_params()`
 
 ### Fixed
 
 - chat_pdf_streamlit_ui.py demo
 - OpenAI API reentrancy & async_helper.py
 
 ### Changed
 
 - Renamed demo alpaca_simple_fix_xml.py → simple_fix_xml.py
 - Renamed demo alpaca_multitask_fix_xml.py → multiprocess.py
-- Renamed `ogbujipt.oapi_choice1_text()` → `ogbujipt.oapi_first_choice_text()`
-- Renamed `ogbujipt.async_helper.schedule_llm_call()` → `ogbujipt.async_helper.schedule_callable()`
+- Renamed `oapi_choice1_text()` → `oapi_first_choice_text()`
+- Renamed `async_helper.schedule_llm_call()` → `async_helper.schedule_callable()`
 
 ## [0.1.1] - 20230711
 
 ### Added
 
 - GitHub CI workflow
 - Orca model style
-- Convenience function ogbujipt.oapi_choice1_text()
-- Additional conveniences in ogbujipt.prompting.model_style
+- Convenience function oapi_choice1_text()
+- Additional conveniences in prompting.model_style
 
 ### Fixed
 
 - Linter cleanup
 
 ### Changed
 
 - Qdrant embeddings interface
-- Renamed ogbujipt.prompting.context_build() → ogbujipt.prompting.format()
+- Renamed prompting.context_build() → prompting.format()
 
 ## [0.1.0]
 
 - Initial standalone release candidate
```

### Comparing `ogbujipt-0.7.1/.github/workflows/main.yml` & `ogbujipt-0.8.0/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `ogbujipt-0.7.1/demo/PGvector_demo.ipynb` & `ogbujipt-0.8.0/demo/PGvector_demo.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9985119047619048%*

 * *Differences: {"'metadata'": "{'language_info': {'version': '3.11.6'}}"}*

```diff
@@ -995,14 +995,14 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.11.4"
+            "version": "3.11.6"
         },
         "orig_nbformat": 4
     },
     "nbformat": 4,
     "nbformat_minor": 2
 }
```

### Comparing `ogbujipt-0.7.1/demo/README.md` & `ogbujipt-0.8.0/demo/README.md`

 * *Files identical despite different names*

### Comparing `ogbujipt-0.7.1/demo/chat_pdf_streamlit_ui.py` & `ogbujipt-0.8.0/demo/chat_pdf_streamlit_ui.py`

 * *Files 0% similar despite different names*

```diff
@@ -169,20 +169,20 @@
     print('  MESSAGES FOR LLM:  '.center(CONSOLE_WIDTH, '='), '\n', messages)
 
     # Remember max Token length default is 16)
     oapi = st.session_state['openai_api']
     # Need to remove old system messages for subsequent queries
     st.session_state['messages'].extend(messages)
     # print(st.session_state['messages'], '\n', '-'*10)
-    response = oapi(st.session_state['messages'], temperature=LLM_TEMP, max_tokens=1024)
+    response = oapi.call(st.session_state['messages'], temperature=LLM_TEMP, max_tokens=1024)
 
     print('\nFull response data from LLM:\n', response)
 
     # Response is a json-like object; extract the text
-    response_text = oapi.first_choice_message(response)
+    response_text = response.first_choice_text
     print('\nResponse text from LLM:\n', response_text)
 
     st.session_state['messages'].append({'role': 'assistant', 'content': response})
     response_placeholder.write(response_text)
     # print(st.session_state['messages'], '\n', '-'*10)
```

### Comparing `ogbujipt-0.7.1/demo/chat_web_selects.py` & `ogbujipt-0.8.0/demo/chat_web_selects.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,30 +139,32 @@
                 top_p=1,  # AKA nucleus sampling; can increase generated text diversity
                 frequency_penalty=0,  # Favor more or less frequent tokens
                 presence_penalty=1,  # Prefer new, previously unused tokens
                 temperature=0.1
                 )
 
             indicator_task = asyncio.create_task(indicate_progress())
-            llm_task = oapi.wrap_for_multiproc(messages, **model_params)
+            llm_task = asyncio.Task(oapi(messages, **model_params))
             tasks = [indicator_task, llm_task]
             done, _ = await asyncio.wait(
                 tasks, return_when=asyncio.FIRST_COMPLETED)
 
+            # proper cleanup of indicator task, which will still be pending/running
+            indicator_task.cancel()
+
             # Instance of openai.openai_object.OpenAIObject, with lots of useful info
             retval = next(iter(done)).result()
             if verbose:
                 print(type(retval))
             # Response is a json-like object; extract the text
             if verbose:
                 print('\nFull response data from LLM:\n', retval)
 
             # just get back the text of the response
-            response_text = oapi.first_choice_message(retval)
-            print('\nResponse text from LLM:\n\n', response_text)
+            print('\nResponse text from LLM:\n\n', retval.first_choice_text)
 
 
 # Command line arguments defined in click decorators
 @click.command()
 @click.option('--verbose/--no-verbose', default=False)
 @click.option('--chunk-size', type=int, default=200,
               help='Number of characters to include per chunk')
```

### Comparing `ogbujipt-0.7.1/demo/function_calling.py` & `ogbujipt-0.8.0/demo/function_calling.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,15 @@
           'description': 'Respond to a user query by specifying a series of steps',
           'parameters': FUNC_SPEC
         }
 ]
 
 function_call={'name': 'handle_steps_from_user_query'}
 
-resp = llm_api(messages=messages, functions=functions, function_call=function_call)
+resp = llm_api.call(messages=messages, functions=functions, function_call=function_call)
 fc = resp.choices[0].message.function_call
 
 if fc:
     print('Function to be called: ' + fc.name)
     print('Function call arguments: ' + fc.arguments)
 else:
     print('No function call issued')
```

### Comparing `ogbujipt-0.7.1/demo/language.toml` & `ogbujipt-0.8.0/demo/language.toml`

 * *Files identical despite different names*

### Comparing `ogbujipt-0.7.1/demo/multiprocess.py` & `ogbujipt-0.8.0/demo/multiprocess.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,30 +45,29 @@
     llmtemp - LLM temperature; hard-coded across all (see https://beta.openai.com/docs/api-reference/completions/create)
     '''
     # Pro tip: When creating asyncio tasks be mindful to not lose references to tasks,
     # lest they get garbage collected, which sows chaos. asyncio.TaskGroup (new in Python 3.11)
     # is often a better alternative, but waits for all tasks to complete whereas we're done once
     # the LLM generation tasks are complete
     indicator_task = asyncio.create_task(console_progress_indicator())
-    llm_tasks = [llm.wrap_for_multiproc(prompt_to_chat(msg), temperature=temp, max_tokens=1024)
+    llm_tasks = [asyncio.create_task(llm(prompt_to_chat(msg), temperature=temp, max_tokens=1024))
                  for (llm, msg, temp) in requests_info]
     llm_messages = [msg for (llm, msg, temp) in requests_info]
     # Need to gather to make sure all LLM tasks are completed
     gathered_llm_tasks = asyncio.gather(*llm_tasks)
     done, _ = await asyncio.wait((indicator_task, gathered_llm_tasks), return_when=asyncio.FIRST_COMPLETED)
 
     # Completed task will from gather() of llm_tasks; results in original task arg order
     results = zip(llm_messages, next(iter(done)).result())
     for msg, resp in results:
         print(f'Result re {msg}')
         # resp is an instance of openai.openai_object.OpenAIObject, with lots of useful info
         print('\nFull response data from LLM:\n', resp)
         # Just the response text
-        response_text = openai_chat_api.first_choice_message(resp)
-        print('\nResponse text from LLM:\n\n', response_text)
+        print('\nResponse text from LLM:\n\n', resp.first_choice_text)
         print('-'*80)
 
 
 # Command line arguments defined in click decorators
 @click.command()
 @click.option('--apibase', default='http://127.0.0.1:8000', help='OpenAI API base URL')
 @click.option('--llmtemp', default='0.9', type=float, help='LLM temperature')
@@ -78,15 +77,15 @@
 @click.option('--model', default='', type=str, 
               help='OpenAI model to use (see https://platform.openai.com/docs/models)')
 def main(apibase, llmtemp, openai, model):
     # Use OpenAI API if specified, otherwise emulate with supplied URL info
     if openai:
         oapi = openai_chat_api(model=(model or 'gpt-3.5-turbo'))
     else:
-        oapi = openai_chat_api(model=model, api_base=apibase)
+        oapi = openai_chat_api(model=model, base_url=apibase)
 
     # Separate models or params—e.g. temp—for each LLM request is left as an exercise 😊
     requests_info = [
         (oapi, TEXTS['test_prompt_joke'].format(topic=t), llmtemp)
         for t in ('wild animals', 'vehicles', 'space aliens')]
 
     asyncio.run(async_main(requests_info))
```

### Comparing `ogbujipt-0.7.1/demo/qa_discord.py` & `ogbujipt-0.8.0/demo/qa_discord.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 
 You can then @mention the bot in a Discord channel where it's been added & chat with it
 
 For hints on how to modify this to use OpenAI's actual services, see demo/alpaca_fix_xml.py
 '''
 
 import os
+import asyncio
 
 import discord
 
 from ogbujipt.llm_wrapper import openai_chat_api, prompt_to_chat
 
 # Enable all standard intents, plus message content
 # The bot app you set up on Discord will require this intent (Bot tab)
@@ -52,24 +53,23 @@
 
 async def send_llm_msg(msg):
     '''
     Schedule the LLM request
     '''
     # See demo/alpaca_multitask_fix_xml.py for some important warnings here
     # oapi.parameters
-    response = await oapi.wrap_for_multiproc(prompt_to_chat(msg), max_tokens=512)
+    response = await asyncio.create_task(oapi(prompt_to_chat(msg), max_tokens=512))
     print(response)
 
     print('\nFull response data from LLM:\n', response)
 
     # Response is a json-like object; we just need the message text
-    response_text = oapi.first_choice_message(response)
-    print('\nResponse text from LLM:\n', response_text)
+    print('\nResponse text from LLM:\n', response.first_choice_text)
 
-    return response_text
+    return response.first_choice_text
 
 
 @client.event
 async def on_message(message):
     # Ignore the bot's own messages & respond only to @mentions
     # The client.user.id check creens out @everyone & @here pings
     # FIXME: Better content check—what if the bot's id is a common word?
```

### Comparing `ogbujipt-0.7.1/demo/simple_fix_xml.py` & `ogbujipt-0.8.0/demo/simple_fix_xml.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,15 +34,15 @@
               help='OpenAI model to use (see https://platform.openai.com/docs/models)')
 def main(apibase, llmtemp, openai, model):
     # Use OpenAI API if specified, otherwise emulate with supplied host, etc.
     if openai:
         assert not apibase, 'Don\'t use --apibase with --openai'
         oapi = openai_api(model=(model or 'gpt-3.5-turbo'))
     else:
-        oapi = openai_api(model=model, api_base=apibase)
+        oapi = openai_api(model=model, base_url=apibase)
 
     BAD_XML_CODE = '''\
 <earth>
 <country><b>Russia</country></b>
 <capital>Moscow</capital>
 </Earth>'''
 
@@ -52,15 +52,15 @@
         'Correct the given XML to make it well-formed',
         contexts= BAD_XML_CODE,
         preamble='You are a helpful assistant, '
         'who answers questions briefly, in 1st grade language',
         delimiters=ALPACA_INSTRUCT_INPUT_DELIMITERS)
     print(prompt, '\n')
 
-    response = oapi(
+    response = oapi.call(
         prompt=prompt,  # Prompt (Required)
         temperature=llmtemp,  # Temp (Default 1)
         max_tokens=100,  # Max Token length of generated text (Default 16)
         top_p=1,  # AKA nucleus sampling; can increase diversity of the
                   # generated text (Default 1)
         frequency_penalty=0,    # influences the model to favor more or less
                                 # frequent tokens (Default 0)
@@ -68,14 +68,13 @@
                             # not yet used (Default 0)
         )
 
     # Response is a json-like object; extract the text
     print('\nFull response data from LLM:\n', response)
 
     # Response is a json-like object; just get back the text of the response
-    response_text = oapi.first_choice_text(response)
-    print('\nResponse text from LLM:\n\n', response_text)
+    print('\nResponse text from LLM:\n\n', response.first_choice_text)
 
 
 # CLI entry point
 if __name__ == '__main__':
     main()
```

### Comparing `ogbujipt-0.7.1/ogbujipt/async_helper.py` & `ogbujipt-0.8.0/ogbujipt/async_helper.py`

 * *Files identical despite different names*

### Comparing `ogbujipt-0.7.1/ogbujipt/config.py` & `ogbujipt-0.8.0/ogbujipt/config.py`

 * *Files identical despite different names*

### Comparing `ogbujipt-0.7.1/ogbujipt/text_helper.py` & `ogbujipt-0.8.0/ogbujipt/text_helper.py`

 * *Files identical despite different names*

### Comparing `ogbujipt-0.7.1/ogbujipt/word_loom.py` & `ogbujipt-0.8.0/ogbujipt/word_loom.py`

 * *Files identical despite different names*

### Comparing `ogbujipt-0.7.1/ogbujipt/embedding/__init__.py` & `ogbujipt-0.8.0/ogbujipt/embedding/__init__.py`

 * *Files identical despite different names*

### Comparing `ogbujipt-0.7.1/ogbujipt/embedding/pgvector.py` & `ogbujipt-0.8.0/ogbujipt/embedding/pgvector.py`

 * *Files identical despite different names*

### Comparing `ogbujipt-0.7.1/ogbujipt/embedding/pgvector_data_doc.py` & `ogbujipt-0.8.0/ogbujipt/embedding/pgvector_data_doc.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 '''
 
 import warnings
 from typing import Iterable
 
 from ogbujipt.embedding.pgvector import PGVectorHelper, asyncpg, process_search_response
 
-__all__ = ['DocDB']
+__all__ = ['DataDB', 'DocDB']
 
 # ------ SQL queries ---------------------------------------------------------------------------------------------------
 # PG only supports proper query arguments (e.g. $1, $2, etc.) for values, not for table or column names
 # Table names are checked to be legit sequel table names, and embed_dimension is assured to be an integer
 
 CREATE_TABLE_BASE = '''-- Create a table to hold embedded documents or data
 CREATE TABLE IF NOT EXISTS {{table_name}} (
@@ -172,28 +172,17 @@
 
             conjunctive (bool, optional): whether to use conjunctive (AND) or disjunctive (OR) matching
                 in the case of multiple tags. Defaults to True.
 
         Returns:
             generator which yields the rows os the query results ass attributable dicts
         '''
-        if query_tags is not None:
-            warnings.warn('query_tags is deprecated. Use tags instead.', DeprecationWarning)
-            tags = query_tags
-        # else:
-        #     if not isinstance(query_tags, list):
-        #         raise TypeError('query_tags must be a list of strings')
-        #     if not all(isinstance(tag, str) for tag in query_tags):
-        #         raise TypeError('query_tags must be a list of strings')
         if threshold is not None:
-            if not isinstance(threshold, float):
-                raise TypeError('threshold must be a float')
-            if (threshold < 0) or (threshold > 1):
-                raise ValueError('threshold must be between 0 and 1')
-
+            if not isinstance(threshold, float) or (threshold < 0) or (threshold > 1):
+                raise TypeError('threshold must be a float between 0.0 and 1.0')
         if not isinstance(limit, int):
             raise TypeError('limit must be an integer')  # Guard against injection
 
         # Get the embedding of the query string as a PGvector compatible list
         query_embedding = list(self._embedding_model.encode(text))
 
         tags_where_clause = TAGS_WHERE_CLAUSE_CONJ if conjunctive else TAGS_WHERE_CLAUSE_DISJ
@@ -222,18 +211,16 @@
             limit_clause = f'LIMIT {limit}\n'
         else:
             limit_clause = ''
 
         # Execute the search via SQL
         async with self.pool.acquire() as conn:
             search_results = await conn.fetch(
-                QUERY_DATA_TABLE.format(
-                    table_name=self.table_name,
-                    where_clauses=where_clauses,
-                    limit_clause=limit_clause,
+                QUERY_DATA_TABLE.format(table_name=self.table_name, where_clauses=where_clauses,
+                                        limit_clause=limit_clause,
                 ),
                 *query_args
             )
         return process_search_response(search_results)
 
 
 class DocDB(PGVectorHelper):
@@ -241,18 +228,15 @@
     async def create_table(self) -> None:
         '''
         Create the table to hold embedded documents
         '''
         async with self.pool.acquire() as conn:
             async with conn.transaction():
                 await conn.execute(
-                    CREATE_DOC_TABLE.format(
-                        table_name=self.table_name,
-                        embed_dimension=self._embed_dimension)
-                    )
+                    CREATE_DOC_TABLE.format(table_name=self.table_name, embed_dimension=self._embed_dimension))
     
     async def insert(
             self,
             content: str,
             title: str = 'NULL',
             page_numbers: list[int] = [],
             tags: list[str] = []
@@ -340,18 +324,16 @@
         Returns:
             generator which yields the rows os the query results ass attributable dicts
         '''
         if query_tags is not None:
             warnings.warn('query_tags is deprecated. Use tags instead.', DeprecationWarning)
             tags = query_tags
         if threshold is not None:
-            if not isinstance(threshold, float):
-                raise TypeError('threshold must be a float')
-            if (threshold < 0) or (threshold > 1):
-                raise ValueError('threshold must be between 0 and 1')
+            if not isinstance(threshold, float) or (threshold < 0) or (threshold > 1):
+                raise TypeError('threshold must be a float between 0.0 and 1.0')
 
         if not isinstance(limit, int):
             raise TypeError('limit must be an integer')  # Guard against injection
 
         # Get the embedding of the query string as a PGvector compatible list
         query_embedding = list(self._embedding_model.encode(text))
```

### Comparing `ogbujipt-0.7.1/ogbujipt/embedding/qdrant.py` & `ogbujipt-0.8.0/ogbujipt/embedding/qdrant.py`

 * *Files 5% similar despite different names*

```diff
@@ -187,15 +187,7 @@
         '''
         if not self._db_initialized:
             raise RuntimeError('Qdrant Collection must be initialized before counting its contents.')
         # This ugly declaration just gets the count as an integer
         current_count = int(str(self.db.count(self.name)).partition('=')[-1])
         return current_count
 
-
-# Already disambiguated by the module name. Anyone can use import as if that's not enough
-# Deprecating the old name
-class qdrant_collection(collection):
-    def __init__(self, name, embedding_model, db=None,
-                 distance_function=None, **conn_params):
-        warnings.warn('qdrant_collection is deprecated. Use collection instead.', DeprecationWarning)
-        super().__init__(name, embedding_model, db=db, distance_function=distance_function, **conn_params)
```

### Comparing `ogbujipt-0.7.1/ogbujipt/prompting/basic.py` & `ogbujipt-0.8.0/ogbujipt/prompting/basic.py`

 * *Files identical despite different names*

### Comparing `ogbujipt-0.7.1/ogbujipt/prompting/model_style.py` & `ogbujipt-0.8.0/ogbujipt/prompting/model_style.py`

 * *Files identical despite different names*

### Comparing `ogbujipt-0.7.1/ogbujipt/resources/wordloom/sample.toml` & `ogbujipt-0.8.0/ogbujipt/resources/wordloom/sample.toml`

 * *Files identical despite different names*

### Comparing `ogbujipt-0.7.1/test/conftest.py` & `ogbujipt-0.8.0/test/conftest.py`

 * *Files identical despite different names*

### Comparing `ogbujipt-0.7.1/test/test_model_style.py` & `ogbujipt-0.8.0/test/test_model_style.py`

 * *Files identical despite different names*

### Comparing `ogbujipt-0.7.1/test/test_ogbujipt.py` & `ogbujipt-0.8.0/test/test_ogbujipt.py`

 * *Files identical despite different names*

### Comparing `ogbujipt-0.7.1/test/test_text_splitter.py` & `ogbujipt-0.8.0/test/test_text_splitter.py`

 * *Files identical despite different names*

### Comparing `ogbujipt-0.7.1/test/test_word_loom.py` & `ogbujipt-0.8.0/test/test_word_loom.py`

 * *Files identical despite different names*

### Comparing `ogbujipt-0.7.1/test/embedding/conftest.py` & `ogbujipt-0.8.0/test/embedding/conftest.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,20 @@
 # SPDX-FileCopyrightText: 2023-present Oori Data <info@oori.dev>
 # SPDX-License-Identifier: Apache-2.0
 # test/embedding/conftest.py
 '''
 Fixtures/setup/teardown for embedding tests
+
+General note: After setup as described in the README.md for this directory, run the tests with:
+
+pytest test
+
+or, for just embeddings tests:
+
+pytest test/embedding/
 '''
 
 import sys
 import os
 import pytest
 import pytest_asyncio
 from unittest.mock import MagicMock, DEFAULT  # noqa: F401
@@ -99,14 +107,15 @@
 
 DB_CLASS = {
     'test/embedding/test_pgvector_message.py': MessageDB,
     'test/embedding/test_pgvector_data.py': DataDB,
     'test/embedding/test_pgvector_doc.py': DocDB,
 }
 
+# print(HOST, DB_NAME, USER, PASSWORD, PORT)
 
 @pytest_asyncio.fixture  # Notice the async aware fixture declaration
 async def DB(request):
     testname = request.node.name
     testfile = request.node.location[0]
     table_name = testname.lower()
     print(f'DB setup for test: {testname}. Table name {table_name}', file=sys.stderr)
@@ -119,16 +128,52 @@
             db_name=DB_NAME,
             host=HOST,
             port=int(PORT),
             user=USER,
             password=PASSWORD)
     except ConnectionRefusedError:
         pytest.skip("No Postgres instance made available for test. Skipping.", allow_module_level=True)
-    if vDB is None:
+    # Actually we want to propagate the error condition, in this case
+    # if vDB is None:
+    #     pytest.skip("Unable to create a valid DB instance. Skipping.", allow_module_level=True)
+
+    # Create table
+    await vDB.drop_table()
+    assert not await vDB.table_exists(), Exception("Table exists before creation")
+    await vDB.create_table()
+    assert await vDB.table_exists(), Exception("Table does not exist after creation")
+    # The test will take control upon the yield
+    yield vDB
+    # Teardown: Drop table
+    await vDB.drop_table()
+
+
+# FIXME: Lots of DRY violations
+@pytest_asyncio.fixture  # Notice the async aware fixture declaration
+async def DB_WINDOWED2(request):
+    testname = request.node.name
+    table_name = testname.lower()
+    print(f'DB setup for test: {testname}. Table name {table_name}', file=sys.stderr)
+    dummy_model = SentenceTransformer('mock_transformer')
+    dummy_model.encode.return_value = np.array([1, 2, 3])
+    try:
+        vDB = await MessageDB.from_conn_params(
+            embedding_model=dummy_model,
+            table_name=table_name,
+            db_name=DB_NAME,
+            host=HOST,
+            port=int(PORT),
+            user=USER,
+            password=PASSWORD,
+            window=2)
+    except ConnectionRefusedError:
         pytest.skip("No Postgres instance made available for test. Skipping.", allow_module_level=True)
+    # Actually we want to propagate the error condition, in this case
+    # if vDB is None:
+    #     pytest.skip("Unable to create a valid DB instance. Skipping.", allow_module_level=True)
 
     # Create table
     await vDB.drop_table()
     assert not await vDB.table_exists(), Exception("Table exists before creation")
     await vDB.create_table()
     assert await vDB.table_exists(), Exception("Table does not exist after creation")
     # The test will take control upon the yield
```

### Comparing `ogbujipt-0.7.1/test/embedding/test_pgvector_data.py` & `ogbujipt-0.8.0/test/embedding/test_pgvector_data.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,20 @@
 # SPDX-FileCopyrightText: 2023-present Oori Data <info@oori.dev>
 # SPDX-License-Identifier: Apache-2.0
 # test/embedding/test_pgvector_data.py
 '''
-See test/embedding/test_pgvector.py for important notes on running these tests
+After setup as described in the README.md for this directory, run the tests with:
+
+pytest test
+
+or, for just this test module:
+
+pytest test/embedding/test_pgvector_data.py
+
+Uses fixtures from conftest.py in current & parent directories
 '''
 
 import pytest
 from unittest.mock import MagicMock, DEFAULT  # noqa: F401
 
 import numpy as np
```

### Comparing `ogbujipt-0.7.1/test/embedding/test_pgvector_doc.py` & `ogbujipt-0.8.0/test/embedding/test_pgvector_doc.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,20 @@
 # SPDX-FileCopyrightText: 2023-present Oori Data <info@oori.dev>
 # SPDX-License-Identifier: Apache-2.0
-# test/embedding/test_pgvector.py
+# test/embedding/test_pgvector_doc.py
 '''
-Set up a mock Postgres instance with the following commands 
-(make sure you don't have anything running on port 0.0.0.0:5432))):
-docker pull ankane/pgvector
-docker run --name mock-postgres -p 5432:5432 \
-    -e POSTGRES_USER=mock_user -e POSTGRES_PASSWORD=mock_password -e POSTGRES_DB=mock_db \
-    -d ankane/pgvector
+After setup as described in the README.md for this directory, run the tests with:
 
-Then run the tests with:
 pytest test
 
-or
+or, for just this test module:
 
-pytest test/embedding/test_pgvector.py
-
-Uses fixtures from ../conftest.py
+pytest test/embedding/test_pgvector_doc.py
 
+Uses fixtures from conftest.py in current & parent directories
 '''
 
 import pytest
 # from unittest.mock import MagicMock, patch
 from unittest.mock import MagicMock, DEFAULT  # noqa: F401
 
 # from ogbujipt.embedding.pgvector import DocDB
@@ -42,16 +35,14 @@
 class SentenceTransformer(object):
     def __init__(self, model_name_or_path):
         self.encode = MagicMock()
 
 
 @pytest.mark.asyncio
 async def test_PGv_embed_pacer(DB):
-    dummy_model = SentenceTransformer('mock_transformer')
-    dummy_model.encode.return_value = np.array([1, 2, 3])
     # Insert data
     for index, text in enumerate(pacer_copypasta):   # For each line in the copypasta
         await DB.insert(                            # Insert the line into the table
             content=text,                            # The text to be embedded
             title=f'Pacer Copypasta line {index}',   # Title metadata
             page_numbers=[1, 2, 3],                  # Page number metadata
             tags=['fitness', 'pacer', 'copypasta'],  # Tag metadata
@@ -64,16 +55,14 @@
     sim_search = await DB.search(text=search_string, limit=3)
     assert sim_search is not None, Exception("No results returned from perfect search")
 
     await DB.drop_table()
 
 @pytest.mark.asyncio
 async def test_PGv_embed_many_pacer(DB):
-    dummy_model = SentenceTransformer('mock_transformer')
-    dummy_model.encode.return_value = np.array([1, 2, 3])
     # Insert data using insert_many()
     documents = (
         (
             text,
             ['fitness', 'pacer', 'copypasta'],
             f'Pacer Copypasta line {index}',
             [1, 2, 3]
@@ -129,34 +118,39 @@
     #Test conjunctive semantics
     await DB.insert(content='Text', title='Some text', page_numbers=[1], tags=['tag1'])
     await DB.insert(content='Text', title='Some mo text', page_numbers=[1], tags=['tag2', 'tag3'])
     await DB.insert(content='Text', title='Even mo text', page_numbers=[1], tags=['tag3'])
 
     # Using limit default
     sim_search = await DB.search(text='Text', tags=['tag1', 'tag3'], conjunctive=False)
-    assert sim_search is not None, Exception("No results returned from filtered search")
-    assert len(list(sim_search)) == 3, Exception(f"There should be 3 results, received {sim_search}")
+    assert sim_search is not None, Exception("Null return from filtered search")
+    sim_search = list(sim_search)
+    assert len(sim_search) == 3, Exception(f"There should be 3 results, received {sim_search}")
 
     sim_search = await DB.search(text='Text', tags=['tag1', 'tag3'], conjunctive=False, limit=1000)
-    assert sim_search is not None, Exception("No results returned from filtered search")
-    assert len(list(sim_search)) == 3, Exception(f"There should be 3 results, received {sim_search}")
+    assert sim_search is not None, Exception("Null return from filtered search")
+    sim_search = list(sim_search)
+    assert len(sim_search) == 3
 
     texts = ['Hello world', 'Hello Dolly', 'Good-Bye to All That']
     authors = ['Brian Kernighan', 'Louis Armstrong', 'Robert Graves']
     metas = [[f'author={a}'] for a in authors]
     count = len(texts)
     records = zip(texts, metas, ['']*count, [None]*count)
     await DB.insert_many(records)
 
     sim_search = await DB.search(text='Hi there!', threshold=0.999, limit=0)
-    assert sim_search is not None, Exception("No results returned from filtered search")
-    assert len(list(sim_search)) == 3, Exception(f"There should be 3 results, received {sim_search}")
-
-    sim_search = await DB.search(text='Hi there!', threshold=0.999, limit=2)
-    assert sim_search is not None, Exception("No results returned from filtered search")
-    assert len(list(sim_search)) == 2, Exception(f"There should be 2 results, received {sim_search}")
+    assert sim_search is not None, Exception("Null return from filtered search")
+    sim_search = list(sim_search)
+    # FIXME: Double-check this expected result
+    assert len(sim_search) == 10
+
+    sim_search = await DB.search(text='Hi there!', threshold=0.5, limit=2)
+    assert sim_search is not None, Exception("Null return from filtered search")
+    sim_search = list(sim_search)
+    assert len(list(sim_search)) == 2
 
     await DB.drop_table()
 
 
 if __name__ == '__main__':
     raise SystemExit("Attention! Run with pytest")
```

### Comparing `ogbujipt-0.7.1/test/embedding/test_pgvector_message.py` & `ogbujipt-0.8.0/test/embedding/test_pgvector_message.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,28 @@
 # SPDX-FileCopyrightText: 2023-present Oori Data <info@oori.dev>
 # SPDX-License-Identifier: Apache-2.0
 # test/embedding/test_pgvector_message.py
 '''
-See test/embedding/test_pgvector.py for important notes on running these tests
+After setup as described in the README.md for this directory, run the tests with:
+
+pytest test
+
+or, for just this test module:
+
+pytest test/embedding/test_pgvector_message.py
+
+Uses fixtures from conftest.py in current & parent directories
 '''
 
 from datetime import datetime
 
 import pytest
 from unittest.mock import MagicMock, DEFAULT  # noqa: F401
 
-# import numpy as np
+import numpy as np
 
 # XXX: Move to a fixture?
 # Definitely don't want to even import SentenceTransformer class due to massive side-effects
 class SentenceTransformer(object):
     def __init__(self, model_name_or_path):
         self.encode = MagicMock()
 
@@ -49,15 +57,38 @@
     # search table with perfect match
     result = await DB.search(text=content, history_key=history_key, limit=3)
     # assert result is not None, Exception('No results returned from perfect search')
 
     # Even though the embedding is mocked, the stored text should be faithful
     row = next(result)
     assert row.content == content
-    assert row.metadata == {'1': 'a'}
+    assert row.metadata == metadata
+
+
+@pytest.mark.asyncio
+async def test_insert_message_vector_windowed(DB_WINDOWED2, MESSAGES):
+    assert await DB_WINDOWED2.count_items() == 0, Exception('Starting with incorrect number of messages')
+    # Insert data
+    for index, (row) in enumerate(MESSAGES):
+        await DB_WINDOWED2.insert(*row)
+
+    # There should be 2 left from each history key
+    assert await DB_WINDOWED2.count_items() == 4, Exception('Incorrect number of messages after insertion')
+
+    # In the windowed case, the oldest 4 messages should have been deleted
+    history_key, role, content, timestamp, metadata = MESSAGES[5]
+
+    # search table with perfect match
+    result = await DB_WINDOWED2.search(text=content, history_key=history_key, limit=2)
+    # assert result is not None, Exception('No results returned from perfect search')
+
+    # Even though the embedding is mocked, the stored text should be faithful
+    row = next(result)
+    assert row.content == content
+    assert row.metadata == metadata
 
 
 @pytest.mark.asyncio
 async def test_insertmany_message_vector(DB, MESSAGES):
     # Insert data using insert_many()
     await DB.insert_many(MESSAGES)
 
@@ -68,15 +99,37 @@
     # search table with perfect match
     result = await DB.search(text=content, history_key=history_key, limit=3)
     # assert result is not None, Exception('No results returned from perfect search')
 
     # Even though the embedding is mocked, the stored text should be faithful
     row = next(result)
     assert row.content == content
-    assert row.metadata == {'1': 'a'}
+    assert row.metadata == metadata
+
+
+@pytest.mark.asyncio
+async def test_insertmany_message_vector_windowed(DB_WINDOWED2, MESSAGES):
+    assert await DB_WINDOWED2.count_items() == 0, Exception('Starting with incorrect number of messages')
+    # Insert data using insert_many()
+    await DB_WINDOWED2.insert_many(MESSAGES)
+
+    # There should be 2 left from each history key
+    assert await DB_WINDOWED2.count_items() == 4, Exception('Incorrect number of messages after insertion')
+
+    # In the windowed case, the oldest 4 messages should have been deleted
+    history_key, role, content, timestamp, metadata = MESSAGES[5]
+
+    # search table with perfect match
+    result = await DB_WINDOWED2.search(text=content, history_key=history_key, limit=3)
+    # assert result is not None, Exception('No results returned from perfect search')
+
+    # Even though the embedding is mocked, the stored text should be faithful
+    row = next(result)
+    assert row.content == content
+    assert row.metadata == metadata
 
 
 @pytest.mark.asyncio
 async def test_get_messages_all_limit(DB, MESSAGES):
     # Insert data using insert_many()
     await DB.insert_many(MESSAGES)
 
@@ -107,9 +160,34 @@
     assert len(results) == 2, Exception('Incorrect number of messages returned from chatlog')
 
     since_ts = datetime.fromisoformat('2021-10-01 00:00:04+00:00')
     results = list(await DB.get_messages(history_key=history_key, since=since_ts))
     assert len(results) == 1, Exception('Incorrect number of messages returned from chatlog')
 
 
+@pytest.mark.asyncio
+async def test_search_threshold(DB, MESSAGES):
+    dummy_model = SentenceTransformer('mock_transformer')
+    def encode_tweaker(*args, **kwargs):
+        # Note: cosine similarity of [1, 2, 3] & [100, 300, 500] appears to be ~ 0.9939
+        if args[0].startswith('Hi'):
+            return np.array([100, 300, 500])
+        else:
+            return np.array([1, 2, 3])
+
+    dummy_model.encode.side_effect = encode_tweaker
+    # Need to replace the default encoder set up by the fixture
+    DB._embedding_model = dummy_model
+
+    await DB.insert_many(MESSAGES)
+
+    history_key, role, content, timestamp, metadata = MESSAGES[0]
+
+    results = list(await DB.search(history_key, 'Hi!', threshold=0.999))
+    assert results is not None and len(results) == 0
+
+    results = list(await DB.search(history_key, 'Hi!', threshold=0.5))
+    assert results is not None and len(results) == 1
+
+
 if __name__ == '__main__':
     raise SystemExit("Attention! Run with pytest")
```

### Comparing `ogbujipt-0.7.1/test/embedding/test_qdrant.py` & `ogbujipt-0.8.0/test/embedding/test_qdrant.py`

 * *Files identical despite different names*

### Comparing `ogbujipt-0.7.1/test/test_prompts/test_airoboros_obedient_prompting.py` & `ogbujipt-0.8.0/test/test_prompts/test_airoboros_obedient_prompting.py`

 * *Files identical despite different names*

### Comparing `ogbujipt-0.7.1/test/test_prompts/test_alpaca_prompting.py` & `ogbujipt-0.8.0/test/test_prompts/test_alpaca_prompting.py`

 * *Files identical despite different names*

### Comparing `ogbujipt-0.7.1/test/test_prompts/test_orca_prompting.py` & `ogbujipt-0.8.0/test/test_prompts/test_orca_prompting.py`

 * *Files identical despite different names*

### Comparing `ogbujipt-0.7.1/util/constraints-apple-silicon.txt` & `ogbujipt-0.8.0/util/constraints-apple-silicon.txt`

 * *Files identical despite different names*

### Comparing `ogbujipt-0.7.1/util/download-model.py` & `ogbujipt-0.8.0/util/download-model.py`

 * *Files identical despite different names*

### Comparing `ogbujipt-0.7.1/.gitignore` & `ogbujipt-0.8.0/.gitignore`

 * *Files identical despite different names*

### Comparing `ogbujipt-0.7.1/LICENSE` & `ogbujipt-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ogbujipt-0.7.1/README.md` & `ogbujipt-0.8.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 Toolkit for using self-hosted large language models (LLMs), but also with support for full-service such as OpenAI's GPT models.
 
 Includes demos with RAG ("chat your documents") and AGI/AutoGPT/privateGPT-style capabilities, via streamlit, Discord, command line, etc.
 
 There are some helper functions for common LLM tasks, such as those provided by projects such as langchain, but not meant to be as extensive. The OgbujiPT approach emphasizes simplicity and transparency.
 
-Tested back ends are [llama-cpp-python](https://github.com/abetlen/llama-cpp-python), [text-generation-webui](https://github.com/oobabooga/text-generation-webui) (AKA Oobabooga or Ooba) and in-memory hosted LLaMA-class (and more) models via [ctransformers](https://github.com/marella/ctransformers). In our own practice we apply these with Nvidia and Apple M1/M2 GPU enabled.
+Tested back ends are [llama.cpp](https://github.com/ggerganov/llama.cpp/blob/master/examples/server/README.md) (custom HTTP API), [llama-cpp-python](https://github.com/abetlen/llama-cpp-python)  (OpenAI HTTP API), [text-generation-webui](https://github.com/oobabooga/text-generation-webui) (AKA Oobabooga or Ooba) and in-memory hosted LLaMA-class (and more) models via [ctransformers](https://github.com/marella/ctransformers). In our own practice we apply these with Nvidia and Apple M1/M2 GPU enabled.
 
 We also test with OpenAI's full service GPT (3, 3.5, and 4) APIs, and apply these in our practice.
 
 <table><tr>
   <td><a href="https://oori.dev/"><img src="https://www.oori.dev/assets/branding/oori_Logo_FullColor.png" width="64" /></a></td>
   <td>OgbujiPT is primarily developed by the crew at <a href="https://oori.dev/">Oori Data</a>. We offer software engineering services around LLM applications.</td>
 </tr></table>
@@ -37,40 +37,74 @@
 ```py
 from ogbujipt.llm_wrapper import openai_chat_api, prompt_to_chat
 
 llm_api = openai_chat_api(base_url='http://localhost:8000')  # Update for your LLM API host
 prompt = 'Write a short birthday greeting for my star employee'
 
 # You can set model params as needed
-resp = llm_api(prompt_to_chat(prompt), temperature=0.1, max_tokens=256)
+resp = llm_api.call(prompt_to_chat(prompt), temperature=0.1, max_tokens=256)
 # Extract just the response text, but the entire structure is available
-print(llm_api.first_choice_message(resp))
+print(resp.first_choice_text)
 ```
 
 The [Nous-Hermes 13B](https://huggingface.co/TheBloke/Nous-Hermes-13B-GGML) LLM offered the following response:
 
 > Dear [Employee's Name],
 > I hope this message finds you well on your special day! I wanted to take a moment to wish you a very happy birthday and express how much your contributions have meant to our team. Your dedication, hard work, and exceptional talent have been an inspiration to us all.
 > On this occasion, I want you to know that you are appreciated and valued beyond measure. May your day be filled with joy and laughter.
 
-Here's an example using a model loaded in memory using ctransformers, a LLaMMa-based model (so ultimately via llama.cpp).
+### Asynchronous by design
+
+Above example shows the synchronous API, provided for dumb convenience, but for most use cases you'll want to use the asynchronous API. This example also adds a system message.
+
+```py
+import asyncio
+from ogbujipt.llm_wrapper import openai_chat_api, prompt_to_chat
+
+llm_api = openai_chat_api(base_url='http://localhost:8000')  # Update for your LLM API host
+prompt = 'Write a short birthday greeting for my star employee'
+
+messages = prompt_to_chat(prompt, system='You are a helpful AI agent…')
+resp = await asyncio.run(llm_api(messages, temperature=0.1, max_tokens=256))
+# Extract just the response text, but the entire structure is available
+print(resp.first_choice_text)
+```
+
+### llama.cpp HTTP API for flexible LLM control
+
+Here's an example using a model hosted directly by [llama.cpp's server](https://github.com/ggerganov/llama.cpp/blob/master/examples/server/README.md).
+
+```py
+import asyncio
+from ogbujipt.llm_wrapper import prompt_to_chat, llama_cpp_http_chat
+
+llm_api = llama_cpp_http_chat('http://localhost:8000')
+resp = asyncio.run(llm_api(prompt_to_chat('Knock knock!'), min_p=0.05))
+print(resp.first_choice_text)
+```
+
+### ctransformers for local in-process loaded LLMs
+
+Here's an example using a model loaded in-process using ctransformers.
 
 ```py
 from ctransformers import AutoModelForCausalLM
 
 from ogbujipt.llm_wrapper import ctransformer as ctrans_wrapper
 
 model = AutoModelForCausalLM.from_pretrained('TheBloke_LlongOrca-13B-16K-GGUF',
         model_file='llongorca-13b-16k.Q5_K_M.gguf', model_type="llama", gpu_layers=50)
 llm = ctrans_wrapper(model=model)
 
 print(llm(prompt='Write a short birthday greeting for my star employee', max_new_tokens=100))
 ```
 
-For more examples see the [demo directory](https://github.com/uogbuji/OgbujiPT/tree/main/demo). Demos include:
+### For more examples…
+
+See the [demo directory](https://github.com/uogbuji/OgbujiPT/tree/main/demo). Demos include:
 
 * Basics:
   * Use of basic LLM text completion to correct a data format (XML)
   * Multiple simultaneous LLM queries via multiprocessing
 * Chatbots/agents:
   * Simple Discord bot
 * Advanced LLM API features:
@@ -129,14 +163,20 @@
 # Credits
 
 Some initial ideas & code were borrowed from these projects, but with heavy refactoring:
 
 * [ChobPT/oobaboogas-webui-langchain_agent](https://github.com/ChobPT/oobaboogas-webui-langchain_agent)
 * [wafflecomposite/langchain-ask-pdf-local](https://github.com/wafflecomposite/langchain-ask-pdf-local)
 
+# Related projects
+
+* [mlx-tuning-fork
+](https://github.com/chimezie/mlx-tuning-fork)—"very basic framework for parameterized Large Language Model (Q)LoRa fine-tuning with MLX. It uses mlx, mlx_lm, and OgbujiPT, and is based primarily on the excellent mlx-example libraries but adds very minimal architecture for systematic running of easily parameterized fine tunes, hyperparameter sweeping, declarative prompt construction, an equivalent of HF's train on completions, and other capabilities."
+* [living-bookmarks](https://github.com/uogbuji/living-bookmarks)—"Uses [OgbujiPT] to Help a user manage their bookmarks in context of various chat, etc."
+
 # FAQ
 
 - [What's unique about this toolkit?](#whats-unique-about-this-toolkit)
 - [Does this support GPU for locally-hosted models](#does-this-support-gpu-for-locally-hosted-models)
 - [What's with the crazy name?](#whats-with-the-crazy-name)
 
 ## What's unique about this toolkit?
```

#### html2text {}

```diff
@@ -1,53 +1,70 @@
 ![ogbujipt github header](https://github.com/OoriData/OgbujiPT/assets/43561307/
 1a88b411-1ce2-43df-83f0-c9c39d6679bc) Toolkit for using self-hosted large
 language models (LLMs), but also with support for full-service such as OpenAI's
 GPT models. Includes demos with RAG ("chat your documents") and AGI/AutoGPT/
 privateGPT-style capabilities, via streamlit, Discord, command line, etc. There
 are some helper functions for common LLM tasks, such as those provided by
 projects such as langchain, but not meant to be as extensive. The OgbujiPT
-approach emphasizes simplicity and transparency. Tested back ends are [llama-
-cpp-python](https://github.com/abetlen/llama-cpp-python), [text-generation-
-webui](https://github.com/oobabooga/text-generation-webui) (AKA Oobabooga or
-Ooba) and in-memory hosted LLaMA-class (and more) models via [ctransformers]
-(https://github.com/marella/ctransformers). In our own practice we apply these
-with Nvidia and Apple M1/M2 GPU enabled. We also test with OpenAI's full
-service GPT (3, 3.5, and 4) APIs, and apply these in our practice.
+approach emphasizes simplicity and transparency. Tested back ends are
+[llama.cpp](https://github.com/ggerganov/llama.cpp/blob/master/examples/server/
+README.md) (custom HTTP API), [llama-cpp-python](https://github.com/abetlen/
+llama-cpp-python) (OpenAI HTTP API), [text-generation-webui](https://
+github.com/oobabooga/text-generation-webui) (AKA Oobabooga or Ooba) and in-
+memory hosted LLaMA-class (and more) models via [ctransformers](https://
+github.com/marella/ctransformers). In our own practice we apply these with
+Nvidia and Apple M1/M2 GPU enabled. We also test with OpenAI's full service GPT
+(3, 3.5, and 4) APIs, and apply these in our practice.
                                        OgbujiPT is primarily developed by the
 _[_h_t_t_p_s_:_/_/_w_w_w_._o_o_r_i_._d_e_v_/_a_s_s_e_t_s_/_b_r_a_n_d_i_n_g_/ crew at _O_o_r_i_ _D_a_t_a. We offer software
 _o_o_r_i___L_o_g_o___F_u_l_l_C_o_l_o_r_._p_n_g_]               engineering services around LLM
                                        applications.
 [![PyPI - Version](https://img.shields.io/pypi/v/ogbujipt.svg)](https://
 pypi.org/project/ogbujipt) [![PyPI - Python Version](https://img.shields.io/
 pypi/pyversions/ogbujipt.svg)](https://pypi.org/project/ogbujipt) ## Quick
 links - [Getting started](#getting-started) - [License](#license) ----- ##
 Getting started ```console pip install ogbujipt ``` ### Just show me some code,
 dammit! ```py from ogbujipt.llm_wrapper import openai_chat_api, prompt_to_chat
 llm_api = openai_chat_api(base_url='http://localhost:8000') # Update for your
 LLM API host prompt = 'Write a short birthday greeting for my star employee' #
-You can set model params as needed resp = llm_api(prompt_to_chat(prompt),
+You can set model params as needed resp = llm_api.call(prompt_to_chat(prompt),
 temperature=0.1, max_tokens=256) # Extract just the response text, but the
-entire structure is available print(llm_api.first_choice_message(resp)) ``` The
-[Nous-Hermes 13B](https://huggingface.co/TheBloke/Nous-Hermes-13B-GGML) LLM
-offered the following response: > Dear [Employee's Name], > I hope this message
-finds you well on your special day! I wanted to take a moment to wish you a
-very happy birthday and express how much your contributions have meant to our
-team. Your dedication, hard work, and exceptional talent have been an
-inspiration to us all. > On this occasion, I want you to know that you are
-appreciated and valued beyond measure. May your day be filled with joy and
-laughter. Here's an example using a model loaded in memory using ctransformers,
-a LLaMMa-based model (so ultimately via llama.cpp). ```py from ctransformers
-import AutoModelForCausalLM from ogbujipt.llm_wrapper import ctransformer as
-ctrans_wrapper model = AutoModelForCausalLM.from_pretrained
+entire structure is available print(resp.first_choice_text) ``` The [Nous-
+Hermes 13B](https://huggingface.co/TheBloke/Nous-Hermes-13B-GGML) LLM offered
+the following response: > Dear [Employee's Name], > I hope this message finds
+you well on your special day! I wanted to take a moment to wish you a very
+happy birthday and express how much your contributions have meant to our team.
+Your dedication, hard work, and exceptional talent have been an inspiration to
+us all. > On this occasion, I want you to know that you are appreciated and
+valued beyond measure. May your day be filled with joy and laughter. ###
+Asynchronous by design Above example shows the synchronous API, provided for
+dumb convenience, but for most use cases you'll want to use the asynchronous
+API. This example also adds a system message. ```py import asyncio from
+ogbujipt.llm_wrapper import openai_chat_api, prompt_to_chat llm_api =
+openai_chat_api(base_url='http://localhost:8000') # Update for your LLM API
+host prompt = 'Write a short birthday greeting for my star employee' messages =
+prompt_to_chat(prompt, system='You are a helpful AI agentâ¦') resp = await
+asyncio.run(llm_api(messages, temperature=0.1, max_tokens=256)) # Extract just
+the response text, but the entire structure is available print
+(resp.first_choice_text) ``` ### llama.cpp HTTP API for flexible LLM control
+Here's an example using a model hosted directly by [llama.cpp's server](https:/
+/github.com/ggerganov/llama.cpp/blob/master/examples/server/README.md). ```py
+import asyncio from ogbujipt.llm_wrapper import prompt_to_chat,
+llama_cpp_http_chat llm_api = llama_cpp_http_chat('http://localhost:8000') resp
+= asyncio.run(llm_api(prompt_to_chat('Knock knock!'), min_p=0.05)) print
+(resp.first_choice_text) ``` ### ctransformers for local in-process loaded LLMs
+Here's an example using a model loaded in-process using ctransformers. ```py
+from ctransformers import AutoModelForCausalLM from ogbujipt.llm_wrapper import
+ctransformer as ctrans_wrapper model = AutoModelForCausalLM.from_pretrained
 ('TheBloke_LlongOrca-13B-16K-GGUF', model_file='llongorca-13b-16k.Q5_K_M.gguf',
 model_type="llama", gpu_layers=50) llm = ctrans_wrapper(model=model) print(llm
 (prompt='Write a short birthday greeting for my star employee',
-max_new_tokens=100)) ``` For more examples see the [demo directory](https://
-github.com/uogbuji/OgbujiPT/tree/main/demo). Demos include: * Basics: * Use of
-basic LLM text completion to correct a data format (XML) * Multiple
+max_new_tokens=100)) ``` ### For more examplesâ¦ See the [demo directory]
+(https://github.com/uogbuji/OgbujiPT/tree/main/demo). Demos include: * Basics:
+* Use of basic LLM text completion to correct a data format (XML) * Multiple
 simultaneous LLM queries via multiprocessing * Chatbots/agents: * Simple
 Discord bot * Advanced LLM API features: * OpenAI-style function calling *
 Retrieval Augmented Generation (RAG): * Ask LLM questions based on web site
 contents, on the command line * Ask LLM questions based on uploaded PDF, via
 Streamlit interactive UI * Use PostgreSQL/PGVector for extracting context which
 can be fed to LLMs ## A bit more explanation Many self-hosted AI large language
 models are now astonishingly good, even running on consumer-grade hardware,
@@ -88,26 +105,34 @@
 ```shell pip install ruff pytest pytest-mock pytest-asyncio respx pgvector
 asyncpg pytest-asyncio pytest test ``` If you want to make contributions to the
 project, please [read these notes](https://github.com/OoriData/OgbujiPT/wiki/
 Notes-for-contributors). # License Apache 2. For tha culture! # Credits Some
 initial ideas & code were borrowed from these projects, but with heavy
 refactoring: * [ChobPT/oobaboogas-webui-langchain_agent](https://github.com/
 ChobPT/oobaboogas-webui-langchain_agent) * [wafflecomposite/langchain-ask-pdf-
-local](https://github.com/wafflecomposite/langchain-ask-pdf-local) # FAQ -
-[What's unique about this toolkit?](#whats-unique-about-this-toolkit) - [Does
-this support GPU for locally-hosted models](#does-this-support-gpu-for-locally-
-hosted-models) - [What's with the crazy name?](#whats-with-the-crazy-name) ##
-What's unique about this toolkit? I mentioned the bias to software engineering,
-but what does this mean? * Emphasis on modularity, but seeking as much
-consistency as possible * Support for multitasking * Finding ways to apply
-automated testing ## Does this support GPU for locally-hosted models Yes, but
-you have to make sure you set up your back end LLm server (llama.cpp or text-
-generation-webui) with GPU, and properly configure the model you load into it.
-If you can use the webui to query your model and get GPU usage, that will also
-apply here in OgbujiPT. Many install guides I've found for Mac, Linux and
-Windows touch on enabling GPU, but the ecosystem is still in its early days,
-and helpful resouces can feel scattered. * [Quick setup for llama-cpp-python]
-(https://github.com/uogbuji/OgbujiPT/wiki/Quick-setup-for-llama-cpp-python-
-backend) * [Quick setup for Ooba](https://github.com/uogbuji/OgbujiPT/wiki/
-Quick-setup-for-text-generation-webui-(Ooba)-backend) ## What's with the crazy
-name? Enh?! Yo mama! ð My surname is Ogbuji, so it's a bit of a pun. This is
-the notorious OGPT, ya feel me?
+local](https://github.com/wafflecomposite/langchain-ask-pdf-local) # Related
+projects * [mlx-tuning-fork ](https://github.com/chimezie/mlx-tuning-
+fork)â"very basic framework for parameterized Large Language Model (Q)LoRa
+fine-tuning with MLX. It uses mlx, mlx_lm, and OgbujiPT, and is based primarily
+on the excellent mlx-example libraries but adds very minimal architecture for
+systematic running of easily parameterized fine tunes, hyperparameter sweeping,
+declarative prompt construction, an equivalent of HF's train on completions,
+and other capabilities." * [living-bookmarks](https://github.com/uogbuji/
+living-bookmarks)â"Uses [OgbujiPT] to Help a user manage their bookmarks in
+context of various chat, etc." # FAQ - [What's unique about this toolkit?]
+(#whats-unique-about-this-toolkit) - [Does this support GPU for locally-hosted
+models](#does-this-support-gpu-for-locally-hosted-models) - [What's with the
+crazy name?](#whats-with-the-crazy-name) ## What's unique about this toolkit? I
+mentioned the bias to software engineering, but what does this mean? * Emphasis
+on modularity, but seeking as much consistency as possible * Support for
+multitasking * Finding ways to apply automated testing ## Does this support GPU
+for locally-hosted models Yes, but you have to make sure you set up your back
+end LLm server (llama.cpp or text-generation-webui) with GPU, and properly
+configure the model you load into it. If you can use the webui to query your
+model and get GPU usage, that will also apply here in OgbujiPT. Many install
+guides I've found for Mac, Linux and Windows touch on enabling GPU, but the
+ecosystem is still in its early days, and helpful resouces can feel scattered.
+* [Quick setup for llama-cpp-python](https://github.com/uogbuji/OgbujiPT/wiki/
+Quick-setup-for-llama-cpp-python-backend) * [Quick setup for Ooba](https://
+github.com/uogbuji/OgbujiPT/wiki/Quick-setup-for-text-generation-webui-(Ooba)-
+backend) ## What's with the crazy name? Enh?! Yo mama! ð My surname is
+Ogbuji, so it's a bit of a pun. This is the notorious OGPT, ya feel me?
```

### Comparing `ogbujipt-0.7.1/pyproject.toml` & `ogbujipt-0.8.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ogbujipt-0.7.1/PKG-INFO` & `ogbujipt-0.8.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: OgbujiPT
-Version: 0.7.1
+Version: 0.8.0
 Summary: Client-side tools for using large language models, full service (e.g. ChatGPT & Bard) or locally hosted (e.g. LLaMA derivatives)
 Project-URL: Documentation, https://github.com/OoriData/OgbujiPT#readme
 Project-URL: Issues, https://github.com/OoriData/OgbujiPT/issues
 Project-URL: Source, https://github.com/OoriData/OgbujiPT
 Author-email: Uche Ogbuji <uche@ogbuji.net>, Osi Ogbuji <osita@ogbuji.net>, Aidan Reese <aidanreese.professional@gmail.com>, Kai Schuyler Gonzalez <kai.schuyler@gmail.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
@@ -26,15 +26,15 @@
 
 Toolkit for using self-hosted large language models (LLMs), but also with support for full-service such as OpenAI's GPT models.
 
 Includes demos with RAG ("chat your documents") and AGI/AutoGPT/privateGPT-style capabilities, via streamlit, Discord, command line, etc.
 
 There are some helper functions for common LLM tasks, such as those provided by projects such as langchain, but not meant to be as extensive. The OgbujiPT approach emphasizes simplicity and transparency.
 
-Tested back ends are [llama-cpp-python](https://github.com/abetlen/llama-cpp-python), [text-generation-webui](https://github.com/oobabooga/text-generation-webui) (AKA Oobabooga or Ooba) and in-memory hosted LLaMA-class (and more) models via [ctransformers](https://github.com/marella/ctransformers). In our own practice we apply these with Nvidia and Apple M1/M2 GPU enabled.
+Tested back ends are [llama.cpp](https://github.com/ggerganov/llama.cpp/blob/master/examples/server/README.md) (custom HTTP API), [llama-cpp-python](https://github.com/abetlen/llama-cpp-python)  (OpenAI HTTP API), [text-generation-webui](https://github.com/oobabooga/text-generation-webui) (AKA Oobabooga or Ooba) and in-memory hosted LLaMA-class (and more) models via [ctransformers](https://github.com/marella/ctransformers). In our own practice we apply these with Nvidia and Apple M1/M2 GPU enabled.
 
 We also test with OpenAI's full service GPT (3, 3.5, and 4) APIs, and apply these in our practice.
 
 <table><tr>
   <td><a href="https://oori.dev/"><img src="https://www.oori.dev/assets/branding/oori_Logo_FullColor.png" width="64" /></a></td>
   <td>OgbujiPT is primarily developed by the crew at <a href="https://oori.dev/">Oori Data</a>. We offer software engineering services around LLM applications.</td>
 </tr></table>
@@ -60,40 +60,74 @@
 ```py
 from ogbujipt.llm_wrapper import openai_chat_api, prompt_to_chat
 
 llm_api = openai_chat_api(base_url='http://localhost:8000')  # Update for your LLM API host
 prompt = 'Write a short birthday greeting for my star employee'
 
 # You can set model params as needed
-resp = llm_api(prompt_to_chat(prompt), temperature=0.1, max_tokens=256)
+resp = llm_api.call(prompt_to_chat(prompt), temperature=0.1, max_tokens=256)
 # Extract just the response text, but the entire structure is available
-print(llm_api.first_choice_message(resp))
+print(resp.first_choice_text)
 ```
 
 The [Nous-Hermes 13B](https://huggingface.co/TheBloke/Nous-Hermes-13B-GGML) LLM offered the following response:
 
 > Dear [Employee's Name],
 > I hope this message finds you well on your special day! I wanted to take a moment to wish you a very happy birthday and express how much your contributions have meant to our team. Your dedication, hard work, and exceptional talent have been an inspiration to us all.
 > On this occasion, I want you to know that you are appreciated and valued beyond measure. May your day be filled with joy and laughter.
 
-Here's an example using a model loaded in memory using ctransformers, a LLaMMa-based model (so ultimately via llama.cpp).
+### Asynchronous by design
+
+Above example shows the synchronous API, provided for dumb convenience, but for most use cases you'll want to use the asynchronous API. This example also adds a system message.
+
+```py
+import asyncio
+from ogbujipt.llm_wrapper import openai_chat_api, prompt_to_chat
+
+llm_api = openai_chat_api(base_url='http://localhost:8000')  # Update for your LLM API host
+prompt = 'Write a short birthday greeting for my star employee'
+
+messages = prompt_to_chat(prompt, system='You are a helpful AI agent…')
+resp = await asyncio.run(llm_api(messages, temperature=0.1, max_tokens=256))
+# Extract just the response text, but the entire structure is available
+print(resp.first_choice_text)
+```
+
+### llama.cpp HTTP API for flexible LLM control
+
+Here's an example using a model hosted directly by [llama.cpp's server](https://github.com/ggerganov/llama.cpp/blob/master/examples/server/README.md).
+
+```py
+import asyncio
+from ogbujipt.llm_wrapper import prompt_to_chat, llama_cpp_http_chat
+
+llm_api = llama_cpp_http_chat('http://localhost:8000')
+resp = asyncio.run(llm_api(prompt_to_chat('Knock knock!'), min_p=0.05))
+print(resp.first_choice_text)
+```
+
+### ctransformers for local in-process loaded LLMs
+
+Here's an example using a model loaded in-process using ctransformers.
 
 ```py
 from ctransformers import AutoModelForCausalLM
 
 from ogbujipt.llm_wrapper import ctransformer as ctrans_wrapper
 
 model = AutoModelForCausalLM.from_pretrained('TheBloke_LlongOrca-13B-16K-GGUF',
         model_file='llongorca-13b-16k.Q5_K_M.gguf', model_type="llama", gpu_layers=50)
 llm = ctrans_wrapper(model=model)
 
 print(llm(prompt='Write a short birthday greeting for my star employee', max_new_tokens=100))
 ```
 
-For more examples see the [demo directory](https://github.com/uogbuji/OgbujiPT/tree/main/demo). Demos include:
+### For more examples…
+
+See the [demo directory](https://github.com/uogbuji/OgbujiPT/tree/main/demo). Demos include:
 
 * Basics:
   * Use of basic LLM text completion to correct a data format (XML)
   * Multiple simultaneous LLM queries via multiprocessing
 * Chatbots/agents:
   * Simple Discord bot
 * Advanced LLM API features:
@@ -152,14 +186,20 @@
 # Credits
 
 Some initial ideas & code were borrowed from these projects, but with heavy refactoring:
 
 * [ChobPT/oobaboogas-webui-langchain_agent](https://github.com/ChobPT/oobaboogas-webui-langchain_agent)
 * [wafflecomposite/langchain-ask-pdf-local](https://github.com/wafflecomposite/langchain-ask-pdf-local)
 
+# Related projects
+
+* [mlx-tuning-fork
+](https://github.com/chimezie/mlx-tuning-fork)—"very basic framework for parameterized Large Language Model (Q)LoRa fine-tuning with MLX. It uses mlx, mlx_lm, and OgbujiPT, and is based primarily on the excellent mlx-example libraries but adds very minimal architecture for systematic running of easily parameterized fine tunes, hyperparameter sweeping, declarative prompt construction, an equivalent of HF's train on completions, and other capabilities."
+* [living-bookmarks](https://github.com/uogbuji/living-bookmarks)—"Uses [OgbujiPT] to Help a user manage their bookmarks in context of various chat, etc."
+
 # FAQ
 
 - [What's unique about this toolkit?](#whats-unique-about-this-toolkit)
 - [Does this support GPU for locally-hosted models](#does-this-support-gpu-for-locally-hosted-models)
 - [What's with the crazy name?](#whats-with-the-crazy-name)
 
 ## What's unique about this toolkit?
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: OgbujiPT Version: 0.7.1 Summary: Client-side tools
+Metadata-Version: 2.3 Name: OgbujiPT Version: 0.8.0 Summary: Client-side tools
 for using large language models, full service (e.g. ChatGPT & Bard) or locally
 hosted (e.g. LLaMA derivatives) Project-URL: Documentation, https://github.com/
 OoriData/OgbujiPT#readme Project-URL: Issues, https://github.com/OoriData/
 OgbujiPT/issues Project-URL: Source, https://github.com/OoriData/OgbujiPT
 Author-email: Uche Ogbuji
 ogbuji.net>, Osi Ogbuji
 ogbuji.net>, Aidan Reese
@@ -18,53 +18,70 @@
 github.com/OoriData/OgbujiPT/assets/43561307/1a88b411-1ce2-43df-83f0-
 c9c39d6679bc) Toolkit for using self-hosted large language models (LLMs), but
 also with support for full-service such as OpenAI's GPT models. Includes demos
 with RAG ("chat your documents") and AGI/AutoGPT/privateGPT-style capabilities,
 via streamlit, Discord, command line, etc. There are some helper functions for
 common LLM tasks, such as those provided by projects such as langchain, but not
 meant to be as extensive. The OgbujiPT approach emphasizes simplicity and
-transparency. Tested back ends are [llama-cpp-python](https://github.com/
-abetlen/llama-cpp-python), [text-generation-webui](https://github.com/
-oobabooga/text-generation-webui) (AKA Oobabooga or Ooba) and in-memory hosted
-LLaMA-class (and more) models via [ctransformers](https://github.com/marella/
-ctransformers). In our own practice we apply these with Nvidia and Apple M1/M2
-GPU enabled. We also test with OpenAI's full service GPT (3, 3.5, and 4) APIs,
-and apply these in our practice.
+transparency. Tested back ends are [llama.cpp](https://github.com/ggerganov/
+llama.cpp/blob/master/examples/server/README.md) (custom HTTP API), [llama-cpp-
+python](https://github.com/abetlen/llama-cpp-python) (OpenAI HTTP API), [text-
+generation-webui](https://github.com/oobabooga/text-generation-webui) (AKA
+Oobabooga or Ooba) and in-memory hosted LLaMA-class (and more) models via
+[ctransformers](https://github.com/marella/ctransformers). In our own practice
+we apply these with Nvidia and Apple M1/M2 GPU enabled. We also test with
+OpenAI's full service GPT (3, 3.5, and 4) APIs, and apply these in our
+practice.
                                        OgbujiPT is primarily developed by the
 _[_h_t_t_p_s_:_/_/_w_w_w_._o_o_r_i_._d_e_v_/_a_s_s_e_t_s_/_b_r_a_n_d_i_n_g_/ crew at _O_o_r_i_ _D_a_t_a. We offer software
 _o_o_r_i___L_o_g_o___F_u_l_l_C_o_l_o_r_._p_n_g_]               engineering services around LLM
                                        applications.
 [![PyPI - Version](https://img.shields.io/pypi/v/ogbujipt.svg)](https://
 pypi.org/project/ogbujipt) [![PyPI - Python Version](https://img.shields.io/
 pypi/pyversions/ogbujipt.svg)](https://pypi.org/project/ogbujipt) ## Quick
 links - [Getting started](#getting-started) - [License](#license) ----- ##
 Getting started ```console pip install ogbujipt ``` ### Just show me some code,
 dammit! ```py from ogbujipt.llm_wrapper import openai_chat_api, prompt_to_chat
 llm_api = openai_chat_api(base_url='http://localhost:8000') # Update for your
 LLM API host prompt = 'Write a short birthday greeting for my star employee' #
-You can set model params as needed resp = llm_api(prompt_to_chat(prompt),
+You can set model params as needed resp = llm_api.call(prompt_to_chat(prompt),
 temperature=0.1, max_tokens=256) # Extract just the response text, but the
-entire structure is available print(llm_api.first_choice_message(resp)) ``` The
-[Nous-Hermes 13B](https://huggingface.co/TheBloke/Nous-Hermes-13B-GGML) LLM
-offered the following response: > Dear [Employee's Name], > I hope this message
-finds you well on your special day! I wanted to take a moment to wish you a
-very happy birthday and express how much your contributions have meant to our
-team. Your dedication, hard work, and exceptional talent have been an
-inspiration to us all. > On this occasion, I want you to know that you are
-appreciated and valued beyond measure. May your day be filled with joy and
-laughter. Here's an example using a model loaded in memory using ctransformers,
-a LLaMMa-based model (so ultimately via llama.cpp). ```py from ctransformers
-import AutoModelForCausalLM from ogbujipt.llm_wrapper import ctransformer as
-ctrans_wrapper model = AutoModelForCausalLM.from_pretrained
+entire structure is available print(resp.first_choice_text) ``` The [Nous-
+Hermes 13B](https://huggingface.co/TheBloke/Nous-Hermes-13B-GGML) LLM offered
+the following response: > Dear [Employee's Name], > I hope this message finds
+you well on your special day! I wanted to take a moment to wish you a very
+happy birthday and express how much your contributions have meant to our team.
+Your dedication, hard work, and exceptional talent have been an inspiration to
+us all. > On this occasion, I want you to know that you are appreciated and
+valued beyond measure. May your day be filled with joy and laughter. ###
+Asynchronous by design Above example shows the synchronous API, provided for
+dumb convenience, but for most use cases you'll want to use the asynchronous
+API. This example also adds a system message. ```py import asyncio from
+ogbujipt.llm_wrapper import openai_chat_api, prompt_to_chat llm_api =
+openai_chat_api(base_url='http://localhost:8000') # Update for your LLM API
+host prompt = 'Write a short birthday greeting for my star employee' messages =
+prompt_to_chat(prompt, system='You are a helpful AI agentâ¦') resp = await
+asyncio.run(llm_api(messages, temperature=0.1, max_tokens=256)) # Extract just
+the response text, but the entire structure is available print
+(resp.first_choice_text) ``` ### llama.cpp HTTP API for flexible LLM control
+Here's an example using a model hosted directly by [llama.cpp's server](https:/
+/github.com/ggerganov/llama.cpp/blob/master/examples/server/README.md). ```py
+import asyncio from ogbujipt.llm_wrapper import prompt_to_chat,
+llama_cpp_http_chat llm_api = llama_cpp_http_chat('http://localhost:8000') resp
+= asyncio.run(llm_api(prompt_to_chat('Knock knock!'), min_p=0.05)) print
+(resp.first_choice_text) ``` ### ctransformers for local in-process loaded LLMs
+Here's an example using a model loaded in-process using ctransformers. ```py
+from ctransformers import AutoModelForCausalLM from ogbujipt.llm_wrapper import
+ctransformer as ctrans_wrapper model = AutoModelForCausalLM.from_pretrained
 ('TheBloke_LlongOrca-13B-16K-GGUF', model_file='llongorca-13b-16k.Q5_K_M.gguf',
 model_type="llama", gpu_layers=50) llm = ctrans_wrapper(model=model) print(llm
 (prompt='Write a short birthday greeting for my star employee',
-max_new_tokens=100)) ``` For more examples see the [demo directory](https://
-github.com/uogbuji/OgbujiPT/tree/main/demo). Demos include: * Basics: * Use of
-basic LLM text completion to correct a data format (XML) * Multiple
+max_new_tokens=100)) ``` ### For more examplesâ¦ See the [demo directory]
+(https://github.com/uogbuji/OgbujiPT/tree/main/demo). Demos include: * Basics:
+* Use of basic LLM text completion to correct a data format (XML) * Multiple
 simultaneous LLM queries via multiprocessing * Chatbots/agents: * Simple
 Discord bot * Advanced LLM API features: * OpenAI-style function calling *
 Retrieval Augmented Generation (RAG): * Ask LLM questions based on web site
 contents, on the command line * Ask LLM questions based on uploaded PDF, via
 Streamlit interactive UI * Use PostgreSQL/PGVector for extracting context which
 can be fed to LLMs ## A bit more explanation Many self-hosted AI large language
 models are now astonishingly good, even running on consumer-grade hardware,
@@ -105,26 +122,34 @@
 ```shell pip install ruff pytest pytest-mock pytest-asyncio respx pgvector
 asyncpg pytest-asyncio pytest test ``` If you want to make contributions to the
 project, please [read these notes](https://github.com/OoriData/OgbujiPT/wiki/
 Notes-for-contributors). # License Apache 2. For tha culture! # Credits Some
 initial ideas & code were borrowed from these projects, but with heavy
 refactoring: * [ChobPT/oobaboogas-webui-langchain_agent](https://github.com/
 ChobPT/oobaboogas-webui-langchain_agent) * [wafflecomposite/langchain-ask-pdf-
-local](https://github.com/wafflecomposite/langchain-ask-pdf-local) # FAQ -
-[What's unique about this toolkit?](#whats-unique-about-this-toolkit) - [Does
-this support GPU for locally-hosted models](#does-this-support-gpu-for-locally-
-hosted-models) - [What's with the crazy name?](#whats-with-the-crazy-name) ##
-What's unique about this toolkit? I mentioned the bias to software engineering,
-but what does this mean? * Emphasis on modularity, but seeking as much
-consistency as possible * Support for multitasking * Finding ways to apply
-automated testing ## Does this support GPU for locally-hosted models Yes, but
-you have to make sure you set up your back end LLm server (llama.cpp or text-
-generation-webui) with GPU, and properly configure the model you load into it.
-If you can use the webui to query your model and get GPU usage, that will also
-apply here in OgbujiPT. Many install guides I've found for Mac, Linux and
-Windows touch on enabling GPU, but the ecosystem is still in its early days,
-and helpful resouces can feel scattered. * [Quick setup for llama-cpp-python]
-(https://github.com/uogbuji/OgbujiPT/wiki/Quick-setup-for-llama-cpp-python-
-backend) * [Quick setup for Ooba](https://github.com/uogbuji/OgbujiPT/wiki/
-Quick-setup-for-text-generation-webui-(Ooba)-backend) ## What's with the crazy
-name? Enh?! Yo mama! ð My surname is Ogbuji, so it's a bit of a pun. This is
-the notorious OGPT, ya feel me?
+local](https://github.com/wafflecomposite/langchain-ask-pdf-local) # Related
+projects * [mlx-tuning-fork ](https://github.com/chimezie/mlx-tuning-
+fork)â"very basic framework for parameterized Large Language Model (Q)LoRa
+fine-tuning with MLX. It uses mlx, mlx_lm, and OgbujiPT, and is based primarily
+on the excellent mlx-example libraries but adds very minimal architecture for
+systematic running of easily parameterized fine tunes, hyperparameter sweeping,
+declarative prompt construction, an equivalent of HF's train on completions,
+and other capabilities." * [living-bookmarks](https://github.com/uogbuji/
+living-bookmarks)â"Uses [OgbujiPT] to Help a user manage their bookmarks in
+context of various chat, etc." # FAQ - [What's unique about this toolkit?]
+(#whats-unique-about-this-toolkit) - [Does this support GPU for locally-hosted
+models](#does-this-support-gpu-for-locally-hosted-models) - [What's with the
+crazy name?](#whats-with-the-crazy-name) ## What's unique about this toolkit? I
+mentioned the bias to software engineering, but what does this mean? * Emphasis
+on modularity, but seeking as much consistency as possible * Support for
+multitasking * Finding ways to apply automated testing ## Does this support GPU
+for locally-hosted models Yes, but you have to make sure you set up your back
+end LLm server (llama.cpp or text-generation-webui) with GPU, and properly
+configure the model you load into it. If you can use the webui to query your
+model and get GPU usage, that will also apply here in OgbujiPT. Many install
+guides I've found for Mac, Linux and Windows touch on enabling GPU, but the
+ecosystem is still in its early days, and helpful resouces can feel scattered.
+* [Quick setup for llama-cpp-python](https://github.com/uogbuji/OgbujiPT/wiki/
+Quick-setup-for-llama-cpp-python-backend) * [Quick setup for Ooba](https://
+github.com/uogbuji/OgbujiPT/wiki/Quick-setup-for-text-generation-webui-(Ooba)-
+backend) ## What's with the crazy name? Enh?! Yo mama! ð My surname is
+Ogbuji, so it's a bit of a pun. This is the notorious OGPT, ya feel me?
```

