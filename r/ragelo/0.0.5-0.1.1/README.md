# Comparing `tmp/ragelo-0.0.5.tar.gz` & `tmp/ragelo-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ragelo-0.0.5.tar", last modified: Thu Feb 15 15:46:41 2024, max compression
+gzip compressed data, was "ragelo-0.1.1.tar", last modified: Tue Apr 16 10:38:23 2024, max compression
```

## Comparing `ragelo-0.0.5.tar` & `ragelo-0.1.1.tar`

### file list

```diff
@@ -1,51 +1,66 @@
-drwxr-xr-x   0 acamara    (501) staff       (20)        0 2024-02-15 15:46:41.390982 ragelo-0.0.5/
--rw-r--r--   0 acamara    (501) staff       (20)    11357 2023-10-10 13:02:35.000000 ragelo-0.0.5/LICENSE
--rw-r--r--   0 acamara    (501) staff       (20)     7208 2024-02-15 15:46:41.390756 ragelo-0.0.5/PKG-INFO
--rw-r--r--   0 acamara    (501) staff       (20)     5669 2024-02-15 15:45:22.000000 ragelo-0.0.5/README.md
--rw-r--r--   0 acamara    (501) staff       (20)     1837 2024-02-15 15:45:22.000000 ragelo-0.0.5/pyproject.toml
-drwxr-xr-x   0 acamara    (501) staff       (20)        0 2024-02-15 15:46:41.382548 ragelo-0.0.5/ragelo/
--rw-r--r--   0 acamara    (501) staff       (20)      448 2024-02-15 15:45:22.000000 ragelo-0.0.5/ragelo/__init__.py
--rw-r--r--   0 acamara    (501) staff       (20)      127 2023-10-19 14:30:37.000000 ragelo-0.0.5/ragelo/__main__.py
-drwxr-xr-x   0 acamara    (501) staff       (20)        0 2024-02-15 15:46:41.384170 ragelo-0.0.5/ragelo/answer_rankers/
--rw-r--r--   0 acamara    (501) staff       (20)       47 2023-10-19 14:30:37.000000 ragelo-0.0.5/ragelo/answer_rankers/__init__.py
--rw-r--r--   0 acamara    (501) staff       (20)     3754 2023-10-19 14:30:37.000000 ragelo-0.0.5/ragelo/answer_rankers/base_answer_ranker.py
--rw-r--r--   0 acamara    (501) staff       (20)     2406 2023-10-19 14:30:37.000000 ragelo-0.0.5/ragelo/answer_rankers/elo_ranker.py
--rw-r--r--   0 acamara    (501) staff       (20)    10992 2024-02-15 15:45:22.000000 ragelo-0.0.5/ragelo/cli.py
-drwxr-xr-x   0 acamara    (501) staff       (20)        0 2024-02-15 15:46:41.384595 ragelo-0.0.5/ragelo/evaluators/
--rw-r--r--   0 acamara    (501) staff       (20)      170 2024-02-15 15:45:22.000000 ragelo-0.0.5/ragelo/evaluators/__init__.py
-drwxr-xr-x   0 acamara    (501) staff       (20)        0 2024-02-15 15:46:41.385351 ragelo-0.0.5/ragelo/evaluators/answer_evaluators/
--rw-r--r--   0 acamara    (501) staff       (20)      152 2024-02-15 15:45:22.000000 ragelo-0.0.5/ragelo/evaluators/answer_evaluators/__init__.py
--rw-r--r--   0 acamara    (501) staff       (20)     2520 2024-02-15 15:45:22.000000 ragelo-0.0.5/ragelo/evaluators/answer_evaluators/base_answer_evaluator.py
--rw-r--r--   0 acamara    (501) staff       (20)    12583 2024-02-15 15:45:22.000000 ragelo-0.0.5/ragelo/evaluators/answer_evaluators/pairwise_reasoning_evaluator.py
--rw-r--r--   0 acamara    (501) staff       (20)     2889 2024-02-15 15:45:22.000000 ragelo-0.0.5/ragelo/evaluators/base_evaluator.py
-drwxr-xr-x   0 acamara    (501) staff       (20)        0 2024-02-15 15:46:41.386763 ragelo-0.0.5/ragelo/evaluators/retrieval_evaluators/
--rw-r--r--   0 acamara    (501) staff       (20)      241 2024-02-15 15:45:22.000000 ragelo-0.0.5/ragelo/evaluators/retrieval_evaluators/__init__.py
--rw-r--r--   0 acamara    (501) staff       (20)     7404 2024-02-15 15:45:22.000000 ragelo-0.0.5/ragelo/evaluators/retrieval_evaluators/base_retrieval_evaluator.py
--rw-r--r--   0 acamara    (501) staff       (20)     7218 2024-02-15 15:45:22.000000 ragelo-0.0.5/ragelo/evaluators/retrieval_evaluators/domain_expert_evaluator.py
--rw-r--r--   0 acamara    (501) staff       (20)     6579 2024-02-15 15:45:22.000000 ragelo-0.0.5/ragelo/evaluators/retrieval_evaluators/rdnam_evaluator.py
--rw-r--r--   0 acamara    (501) staff       (20)     1388 2024-02-15 15:45:22.000000 ragelo-0.0.5/ragelo/evaluators/retrieval_evaluators/reasoner_evaluator.py
-drwxr-xr-x   0 acamara    (501) staff       (20)        0 2024-02-15 15:46:41.387651 ragelo-0.0.5/ragelo/llm_providers/
--rw-r--r--   0 acamara    (501) staff       (20)       42 2024-02-15 15:45:22.000000 ragelo-0.0.5/ragelo/llm_providers/__init__.py
--rw-r--r--   0 acamara    (501) staff       (20)     1013 2024-02-15 15:45:22.000000 ragelo-0.0.5/ragelo/llm_providers/base_llm_provider.py
--rw-r--r--   0 acamara    (501) staff       (20)     3513 2024-02-15 15:45:22.000000 ragelo-0.0.5/ragelo/llm_providers/openai_client.py
--rw-r--r--   0 acamara    (501) staff       (20)     1149 2023-10-19 12:33:24.000000 ragelo-0.0.5/ragelo/logger.py
-drwxr-xr-x   0 acamara    (501) staff       (20)        0 2024-02-15 15:46:41.388563 ragelo-0.0.5/ragelo/types/
--rw-r--r--   0 acamara    (501) staff       (20)       51 2024-02-15 15:45:22.000000 ragelo-0.0.5/ragelo/types/__init__.py
--rw-r--r--   0 acamara    (501) staff       (20)     1779 2024-02-15 15:45:22.000000 ragelo-0.0.5/ragelo/types/configurations.py
--rw-r--r--   0 acamara    (501) staff       (20)      157 2024-02-15 15:45:22.000000 ragelo-0.0.5/ragelo/types/types.py
-drwxr-xr-x   0 acamara    (501) staff       (20)        0 2024-02-15 15:46:41.388795 ragelo-0.0.5/ragelo/utils/
--rw-r--r--   0 acamara    (501) staff       (20)        0 2023-10-25 15:00:07.000000 ragelo-0.0.5/ragelo/utils/__init__.py
-drwxr-xr-x   0 acamara    (501) staff       (20)        0 2024-02-15 15:46:41.390008 ragelo-0.0.5/ragelo.egg-info/
--rw-r--r--   0 acamara    (501) staff       (20)     7208 2024-02-15 15:46:41.000000 ragelo-0.0.5/ragelo.egg-info/PKG-INFO
--rw-r--r--   0 acamara    (501) staff       (20)     1287 2024-02-15 15:46:41.000000 ragelo-0.0.5/ragelo.egg-info/SOURCES.txt
--rw-r--r--   0 acamara    (501) staff       (20)        1 2024-02-15 15:46:41.000000 ragelo-0.0.5/ragelo.egg-info/dependency_links.txt
--rw-r--r--   0 acamara    (501) staff       (20)       42 2024-02-15 15:46:41.000000 ragelo-0.0.5/ragelo.egg-info/entry_points.txt
--rw-r--r--   0 acamara    (501) staff       (20)      211 2024-02-15 15:46:41.000000 ragelo-0.0.5/ragelo.egg-info/requires.txt
--rw-r--r--   0 acamara    (501) staff       (20)       39 2024-02-15 15:46:41.000000 ragelo-0.0.5/ragelo.egg-info/top_level.txt
--rw-r--r--   0 acamara    (501) staff       (20)       38 2024-02-15 15:46:41.391023 ragelo-0.0.5/setup.cfg
-drwxr-xr-x   0 acamara    (501) staff       (20)        0 2024-02-15 15:46:41.388902 ragelo-0.0.5/tests/
--rw-r--r--   0 acamara    (501) staff       (20)     4328 2024-02-15 15:45:22.000000 ragelo-0.0.5/tests/conftest.py
-drwxr-xr-x   0 acamara    (501) staff       (20)        0 2024-02-15 15:46:41.389568 ragelo-0.0.5/tests/unit/
--rw-r--r--   0 acamara    (501) staff       (20)     1450 2024-02-15 15:45:22.000000 ragelo-0.0.5/tests/unit/test_answer_evaluators.py
--rw-r--r--   0 acamara    (501) staff       (20)     1415 2024-02-15 15:45:22.000000 ragelo-0.0.5/tests/unit/test_llm_providers.py
--rw-r--r--   0 acamara    (501) staff       (20)     6121 2024-02-15 15:45:22.000000 ragelo-0.0.5/tests/unit/test_retrieval_evaluators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:38:23.040865 ragelo-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-16 10:38:14.000000 ragelo-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10654 2024-04-16 10:38:23.040865 ragelo-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9039 2024-04-16 10:38:14.000000 ragelo-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-04-16 10:38:14.000000 ragelo-0.1.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:38:23.028865 ragelo-0.1.1/ragelo/
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-16 10:38:14.000000 ragelo-0.1.1/ragelo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-16 10:38:14.000000 ragelo-0.1.1/ragelo/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:38:23.028865 ragelo-0.1.1/ragelo/agent_rankers/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-16 10:38:14.000000 ragelo-0.1.1/ragelo/agent_rankers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3644 2024-04-16 10:38:14.000000 ragelo-0.1.1/ragelo/agent_rankers/base_agent_ranker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-04-16 10:38:14.000000 ragelo-0.1.1/ragelo/agent_rankers/elo_ranker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:38:23.032865 ragelo-0.1.1/ragelo/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-16 10:38:14.000000 ragelo-0.1.1/ragelo/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-16 10:38:14.000000 ragelo-0.1.1/ragelo/cli/agent_rankers_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-04-16 10:38:14.000000 ragelo-0.1.1/ragelo/cli/answer_evaluators_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2334 2024-04-16 10:38:14.000000 ragelo-0.1.1/ragelo/cli/args.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3158 2024-04-16 10:38:14.000000 ragelo-0.1.1/ragelo/cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3583 2024-04-16 10:38:14.000000 ragelo-0.1.1/ragelo/cli/retrieval_evaluator_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-16 10:38:14.000000 ragelo-0.1.1/ragelo/cli/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:38:23.032865 ragelo-0.1.1/ragelo/evaluators/
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-16 10:38:14.000000 ragelo-0.1.1/ragelo/evaluators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:38:23.032865 ragelo-0.1.1/ragelo/evaluators/answer_evaluators/
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-16 10:38:14.000000 ragelo-0.1.1/ragelo/evaluators/answer_evaluators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8734 2024-04-16 10:38:14.000000 ragelo-0.1.1/ragelo/evaluators/answer_evaluators/base_answer_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-04-16 10:38:14.000000 ragelo-0.1.1/ragelo/evaluators/answer_evaluators/custom_prompt_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10930 2024-04-16 10:38:14.000000 ragelo-0.1.1/ragelo/evaluators/answer_evaluators/pairwise_reasoning_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12512 2024-04-16 10:38:14.000000 ragelo-0.1.1/ragelo/evaluators/base_evaluator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:38:23.032865 ragelo-0.1.1/ragelo/evaluators/retrieval_evaluators/
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-16 10:38:14.000000 ragelo-0.1.1/ragelo/evaluators/retrieval_evaluators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7901 2024-04-16 10:38:14.000000 ragelo-0.1.1/ragelo/evaluators/retrieval_evaluators/base_retrieval_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-04-16 10:38:14.000000 ragelo-0.1.1/ragelo/evaluators/retrieval_evaluators/custom_prompt_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7618 2024-04-16 10:38:14.000000 ragelo-0.1.1/ragelo/evaluators/retrieval_evaluators/domain_expert_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-04-16 10:38:14.000000 ragelo-0.1.1/ragelo/evaluators/retrieval_evaluators/few_shot_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5112 2024-04-16 10:38:14.000000 ragelo-0.1.1/ragelo/evaluators/retrieval_evaluators/rdnam_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-04-16 10:38:14.000000 ragelo-0.1.1/ragelo/evaluators/retrieval_evaluators/reasoner_evaluator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:38:23.036865 ragelo-0.1.1/ragelo/llm_providers/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-16 10:38:14.000000 ragelo-0.1.1/ragelo/llm_providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3579 2024-04-16 10:38:14.000000 ragelo-0.1.1/ragelo/llm_providers/base_llm_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-04-16 10:38:14.000000 ragelo-0.1.1/ragelo/llm_providers/openai_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-04-16 10:38:14.000000 ragelo-0.1.1/ragelo/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:38:23.036865 ragelo-0.1.1/ragelo/types/
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-16 10:38:14.000000 ragelo-0.1.1/ragelo/types/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:38:23.036865 ragelo-0.1.1/ragelo/types/configurations/
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-16 10:38:14.000000 ragelo-0.1.1/ragelo/types/configurations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-16 10:38:14.000000 ragelo-0.1.1/ragelo/types/configurations/agent_ranker_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-04-16 10:38:14.000000 ragelo-0.1.1/ragelo/types/configurations/answer_evaluator_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3616 2024-04-16 10:38:14.000000 ragelo-0.1.1/ragelo/types/configurations/base_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-16 10:38:14.000000 ragelo-0.1.1/ragelo/types/configurations/llm_provider_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4618 2024-04-16 10:38:14.000000 ragelo-0.1.1/ragelo/types/configurations/retrieval_evaluator_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3944 2024-04-16 10:38:14.000000 ragelo-0.1.1/ragelo/types/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6802 2024-04-16 10:38:14.000000 ragelo-0.1.1/ragelo/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:38:23.036865 ragelo-0.1.1/ragelo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10654 2024-04-16 10:38:23.000000 ragelo-0.1.1/ragelo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-04-16 10:38:23.000000 ragelo-0.1.1/ragelo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 10:38:23.000000 ragelo-0.1.1/ragelo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-16 10:38:23.000000 ragelo-0.1.1/ragelo.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-16 10:38:23.000000 ragelo-0.1.1/ragelo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-16 10:38:23.000000 ragelo-0.1.1/ragelo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 10:38:23.040865 ragelo-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:38:23.036865 ragelo-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7681 2024-04-16 10:38:14.000000 ragelo-0.1.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:38:23.036865 ragelo-0.1.1/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)     3704 2024-04-16 10:38:14.000000 ragelo-0.1.1/tests/unit/test_answer_evaluators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-04-16 10:38:14.000000 ragelo-0.1.1/tests/unit/test_llm_providers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12893 2024-04-16 10:38:14.000000 ragelo-0.1.1/tests/unit/test_retrieval_evaluators.py
```

### Comparing `ragelo-0.0.5/LICENSE` & `ragelo-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ragelo-0.0.5/pyproject.toml` & `ragelo-0.1.1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -20,28 +20,29 @@
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python :: 3.10",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: System :: Benchmark",
 ]
-dependencies = ["openai>=1.10", "tenacity", "typer", "numpy"]
+dependencies = ["openai>=1.10", "tenacity", "typer", "numpy", "pydantic>=1.9"]
 
 [project.optional-dependencies]
 cli = ["typer[all]"]
 dev = [
     "bandit==1.7.5",
     "black==23.10.0",
     "isort==5.12.0",
     "flake8==6.1.0",
     "flake8-black==0.3.6",
     "flake8-isort==6.1.0",
-    "mypy==1.6.1",
+    "mypy==1.9.0",
     "Flake8-pyproject==1.2.3",
     "types-tqdm==4.66.0",
+    "pydantic==2.7.0",
 ]
 
 [project.scripts]
 ragelo = "ragelo.cli:app"
 
 [project.urls]
 Homepage = "https://github.com/zetaalphavector/RAGElo"
@@ -50,19 +51,25 @@
 [tool.setuptools.packages.find]
 exclude = ["data*"]
 
 [tool.isort]
 profile = "black"
 
 [tool.mypy]
+plugins = ["pydantic.mypy"]
 python_version = "3.11"
 show_column_numbers = true
 namespace_packages = true
+follow_imports = "silent"
+warn_redundant_casts = true
+check_untyped_defs = true
+implicit_reexport = true
 exclude = ["build/", "dist/", "venv/"]
 
+
 [tool.flake8]
 ignore = ['E501', "W503"]
 per-file-ignores = ['__init__.py:F401,F403']
 exclude = ["build/", "dist/", "venv/"]
 
 
 [tool.setuptools-git-versioning]
```

### Comparing `ragelo-0.0.5/ragelo/answer_rankers/base_answer_ranker.py` & `ragelo-0.1.1/ragelo/agent_rankers/base_agent_ranker.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,107 +1,108 @@
 """Base models for ranking a set of answers generated by LLMs"""
+
 import csv
-import json
 from abc import abstractmethod
 from collections import defaultdict
-from typing import Dict, List, Tuple, Type
+from typing import Type
 
 from ragelo.logger import logger
+from ragelo.types import AgentRankerConfig
+
 
+class AgentRanker:
+    config: AgentRankerConfig
+    evaluations: list[tuple[str, str, str]]
+    ranking: defaultdict[str, list[str]]
+    output_file: str = "agents_ranking.csv"
+    name: str = "Agent Ranker"
 
-class AnswerRanker:
     def __init__(
         self,
-        name: str,
-        output_file: str,
-        evaluations_file: str | None = None,
-        evaluations: List[Tuple[str, str, str]] | None = None,
-        print: bool = False,
-        force: bool = False,
-        **kwargs,
+        config: AgentRankerConfig,
+        evaluations: list[tuple[str, str, str]],
     ):
-        """Base model for dealing with answer rankers
-        Args:
-            evaluations_file (str): Path to jsonl file containing the answers from
-                AnswerEvaluator
-            evaluations: List of dictionary containing at least qid, agent_a, agent_b
-                and relevant (A, B or C)
-            kwargs: Any additional arguments
-        """
-
-        if evaluations_file is None and evaluations is None:
-            raise ValueError(
-                "Either one of evaluations_file or evaluations should be provided"
-            )
-        if evaluations_file is not None:
-            if evaluations is not None:
-                logger.warning("Passing both evaluations and evaluations_file")
-                logger.warning("Will keep only evaluations_file")
-            self.evaluations = self._load_answers(evaluations_file)
-        elif evaluations is not None:
-            self.evaluations = evaluations
-        else:
-            raise ValueError("No evaluations found")
-
-        self.ranking: defaultdict = defaultdict(list)
-        self.name = name
-        self.print = print
-        self.force = force
-        self.output_file = output_file
+        self.config = config
+        self.evaluations = evaluations
+        self.ranking = defaultdict(list)
+        if config.output_file is not None:
+            self.output_file = config.output_file
 
-    def _load_answers(self, answers_file: str) -> List[Tuple[str, str, str]]:
+    @staticmethod
+    def load_evaluations(answers_file: str) -> list[tuple[str, str, str]]:
         evaluations = []
-        for line in open(answers_file, "r"):
-            data = json.loads(line)
-            agent_a = data["agent_a"]
-            agent_b = data["agent_b"]
-            relevant = data["relevant"]
-            evaluations.append((agent_a, agent_b, relevant))
+        with open(answers_file, "r") as f:
+            reader = csv.DictReader(f)
+            for row in reader:
+                agent_a = row["agent_a"]
+                agent_b = row["agent_b"]
+                relevant = row["answer"]
+                evaluations.append((agent_a, agent_b, relevant))
         return evaluations
 
+    @classmethod
+    def from_config(cls, config: AgentRankerConfig):
+        evaluations = cls.load_evaluations(config.evaluations_file)
+        return cls(config, evaluations)
+
     @abstractmethod
-    def evaluate(self):
+    def run(self):
         """Compute score for each agent"""
         raise NotImplementedError
 
     @abstractmethod
-    def get_agents_ratings(self) -> Dict[str, float]:
+    def get_agents_ratings(self) -> dict[str, float]:
         """Returns the score of all players"""
         raise NotImplementedError
 
-    def print_ranking(self):
-        if self.print:
-            logger.info(
-                f"-------[bold white] Agent Scores by {self.name} [/bold white]-------"
-            )
-
-            for agent, rating in sorted(
-                self.get_agents_ratings().items(), key=lambda x: x[1], reverse=True
-            ):
-                logger.info(f"[bold white]{agent:<15}[/bold white]: {rating:.1f}")
+    def dump_ranking(self):
         with open(self.output_file, "w") as f:
             writer = csv.writer(f)
             writer.writerow(["agent", "score"])
             for agent, rating in sorted(
                 self.get_agents_ratings().items(), key=lambda x: x[1], reverse=True
             ):
                 writer.writerow([agent, rating])
 
+    def print_ranking(self):
+        if not self.config.verbose:
+            return
+        scores = sorted(
+            self.get_agents_ratings().items(), key=lambda x: x[1], reverse=True
+        )
+        if self.config.rich_print:
+            try:
+                import rich
+
+                rich.print(
+                    f"-------[bold white] Agent Scores by {self.name} [/bold white]-------"
+                )
+
+                for agent, rating in scores:
+                    rich.print(f"[bold white]{agent:<15}[/bold white]: {rating:.1f}")
+            except ImportError:
+                logger.warning("Rich not installed. Using plain print")
+                self.config.rich_print = False
+        if not self.config.rich_print:
+            print(f"------- Agent Scores by {self.name} -------")
+            for agent, rating in scores:
+                print(f"{agent:<15}: {rating:.1f}")
+
 
-class AnswerRankerFactory:
-    registry: Dict[str, Type[AnswerRanker]] = {}
+class AgentRankerFactory:
+    registry: dict[str, Type[AgentRanker]] = {}
 
     @classmethod
     def register(cls, name: str):
-        def inner_wrapper(wrapped_class: Type[AnswerRanker]):
+        def inner_wrapper(wrapped_class: Type[AgentRanker]):
             if name in cls.registry:
                 logger.warning(f"Overwriting {name} in Answer Evaluator registry")
             cls.registry[name.lower()] = wrapped_class
             return wrapped_class
 
         return inner_wrapper
 
     @classmethod
-    def create(cls, name: str, **kwargs) -> AnswerRanker:
-        if name.lower() not in cls.registry:
-            raise ValueError(f"{name} not in registry")
-        return cls.registry[name.lower()](name=name, **kwargs)
+    def create(cls, ranker_name: str, config: AgentRankerConfig) -> AgentRanker:
+        if ranker_name.lower() not in cls.registry:
+            raise ValueError(f"Unknown Agent Ranker {ranker_name}")
+        return cls.registry[ranker_name.lower()].from_config(config)
```

### Comparing `ragelo-0.0.5/ragelo/answer_rankers/elo_ranker.py` & `ragelo-0.1.1/ragelo/agent_rankers/elo_ranker.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,63 +1,73 @@
 import random
-from typing import Dict, List, Tuple
 
-from ragelo.answer_rankers.base_answer_ranker import AnswerRanker, AnswerRankerFactory
+from ragelo.agent_rankers.base_agent_ranker import AgentRanker, AgentRankerFactory
 from ragelo.logger import logger
+from ragelo.types import EloAgentRankerConfig
 
 
-@AnswerRankerFactory.register("elo")
-class EloRanker(AnswerRanker):
-    def __init__(self, initial_score: int = 1000, k: int = 32, *args, **kwargs):
-        super().__init__(*args, **kwargs)
+@AgentRankerFactory.register("elo")
+class EloRanker(AgentRanker):
+    name: str = "Elo Agent Ranker"
+    config: EloAgentRankerConfig
+
+    def __init__(
+        self,
+        config: EloAgentRankerConfig,
+        evaluations: list[tuple[str, str, str]],
+    ):
+        super().__init__(config, evaluations)
         self.score_map = {"A": 1, "B": 0, "C": 0.5}
-        self.name = "Elo ranking"
-        self.players: Dict[str, float] = {}
-        self.games: List[Tuple[str, str, float]] = []
+
+        self.agents: dict[str, int] = {}
+        self.games: list[tuple[str, str, float]] = []
         self.computed = False
-        self.initial_score = initial_score
-        self.k = k
+        self.initial_score = self.config.initial_score
+        self.k = self.config.k
 
-    def evaluate(self):
+    def run(self):
         """Compute score for each agent"""
-        self.games, self.players = self.__get_elo_scores()
+        self.games, self.agents = self.__get_elo_scores()
+
         while self.games:
             self.__play_one_game()
+        self.dump_ranking()
+        self.print_ranking()
 
     def get_agents_ratings(self):
         if not self.computed:
             raise ValueError("Ranking not computed yet, Run evaluate() first")
-        return self.players
+        return self.agents
 
-    def __get_elo_scores(self) -> Tuple[List[Tuple[str, str, float]], Dict[str, int]]:
-        games: List[Tuple[str, str, float]] = []
-        players = {}
+    def __get_elo_scores(self) -> tuple[list[tuple[str, str, float]], dict[str, int]]:
+        games: list[tuple[str, str, float]] = []
+        agents = {}
         for agent_a, agent_b, score in self.evaluations:
             score_val = self.score_map[score]
             games.append((agent_a, agent_b, score_val))
             logger.info(f"Game: {agent_a} vs {agent_b} -> {score_val}")
-            if agent_a not in players:
-                players[agent_a] = self.initial_score
-            if agent_b not in players:
-                players[agent_b] = self.initial_score
+            if agent_a not in agents:
+                agents[agent_a] = self.initial_score
+            if agent_b not in agents:
+                agents[agent_b] = self.initial_score
         random.shuffle(games)
         self.computed = True
-        return games, players
+        return games, agents
 
     def __play_one_game(self):
         player1, player2, result = self.games.pop()
-        player1_rating = self.players[player1]
-        player2_rating = self.players[player2]
+        player1_rating = self.agents[player1]
+        player2_rating = self.agents[player2]
         expected_score = self.__expected_score(player1_rating, player2_rating)
 
-        self.players[player1] = self.__update_rating(
+        self.agents[player1] = self.__update_rating(
             player1_rating, expected_score, result
         )
-        self.players[player2] = self.__update_rating(
+        self.agents[player2] = self.__update_rating(
             player2_rating, 1 - expected_score, 1 - result
         )
 
     def __expected_score(self, rating1, rating2):
         return 1 / (1 + 10 ** ((rating2 - rating1) / 400))
 
-    def __update_rating(self, rating, expected_score, actual_score):
-        return rating + self.k * (actual_score - expected_score)
+    def __update_rating(self, rating, expected_score, actual_score) -> int:
+        return int(rating + self.k * (actual_score - expected_score))
```

### Comparing `ragelo-0.0.5/ragelo/evaluators/answer_evaluators/pairwise_reasoning_evaluator.py` & `ragelo-0.1.1/ragelo/evaluators/answer_evaluators/pairwise_reasoning_evaluator.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,295 +1,276 @@
 import csv
-import json
-import logging
 import os
 import random
 import re
-from collections import defaultdict, deque
-from typing import Dict, List, Set, Tuple
+from collections import defaultdict
+from typing import Any, Optional
 
 from tenacity import RetryError
 from tqdm.auto import tqdm
 
 from ragelo.evaluators.answer_evaluators.base_answer_evaluator import (
     AnswerEvaluatorFactory,
     BaseAnswerEvaluator,
 )
 from ragelo.llm_providers.base_llm_provider import BaseLLMProvider
-from ragelo.types import Query
-from ragelo.types.configurations import AnswerEvaluatorConfig
+from ragelo.logger import logger
+from ragelo.types import (
+    AgentAnswer,
+    AnswerEvaluatorResult,
+    AnswerEvaluatorTypes,
+    Document,
+    Query,
+)
+from ragelo.types.configurations import PairwiseEvaluatorConfig
 
 
-@AnswerEvaluatorFactory.register("PairwiseWithReasoning")
+@AnswerEvaluatorFactory.register(AnswerEvaluatorTypes.PAIRWISE_REASONING)
 class PairwiseWithReasoningEvaluator(BaseAnswerEvaluator):
     """A evaluator that evaluates RAG-based answers pairwise, with document reasoning"""
 
-    prompt = """Please act as an impartial judge and evaluate the quality of the responses provided by two AI assistants tasked to answer the question displayed below, based on a set of documents retrieved by a search engine.
-You should choose the assistant that best answers the user question based on a set of reference documents that may or not be relevant.
-Answers cite documents using square brackets.  For each reference document, you will be provided with a reasoning explaining why the document is or is not relevant.
-Your evaluation should consider factors such as the correctness, helpfulness, completeness, accuracy, depth, and level of detail of their responses. Details are only useful if they answer the user question. If an answers contains non-relevant details, it should not be preferred over one that only use relevant information.
-Begin your evaluation by explaining why each answer correctly answers the user question. Then, you should compare the two responses and provide a short explanation on their differences. Avoid any position biases and ensure that the order in which the responses were presented does not influence your decision. Do not allow the length of the responses to influence your evaluation. Be as objective as possible. After providing your explanation, output your final verdict by strictly following this format: "[[A]]" if assistant A is better, "[[B]]" if assistant B is better, and "[[C]]" for a tie.
+    config: PairwiseEvaluatorConfig
+    output_columns: list[str] = ["qid", "agent_a", "agent_b", "raw_answer", "answer"]
+    output_file: str = "pairwise_answers_evaluations.csv"
+    prompt = """
+Please act as an impartial judge and evaluate the quality of the responses provided \
+by two AI assistants tasked to answer the question displayed below, based on a set \
+of documents retrieved by a search engine.
+You should choose the assistant that best answers the user question based on a set \
+of reference documents that may or not be relevant.
+Answers cite documents using square brackets. For each reference document, you will \
+be provided with a reasoning explaining why the document is or is not relevant.
+Your evaluation should consider factors such as the correctness, helpfulness, \
+completeness, accuracy, depth, and level of detail of their responses.\
+Details are only useful if they answer the user question. If an answer \
+contains non-relevant details, it should not be preferred over one that only \
+use relevant information.
+Begin your evaluation by explaining why each answer correctly answers the user \
+question. Then, you should compare the two responses and provide a short explanation \
+on their differences. Avoid any position biases and ensure that the order in which \
+the responses were presented does not influence your decision. Do not allow the \
+length of the responses to influence your evaluation. Be as objective as possible.
+After providing your explanation, output your final verdict by strictly following \
+this format: "[[A]]" if assistant A is better, "[[B]]" if assistant B is better, \
+and "[[C]]" for a tie.
 
 [User Question]
 {query}
 
 [Reference Documents]
 {documents}
 
 [The Start of Assistant A's Answer]
 {answer_a}
 [The End of Assistant A's Answer]
 
 [The Start of Assistant B's Answer]
 {answer_b}
-[The End of Assistant B's Answer]"""  # noqa: E501
+[The End of Assistant B's Answer]
+""".strip()
 
     def __init__(
         self,
-        config: AnswerEvaluatorConfig,
-        queries: Dict[str, Query],
-        answers: Dict[str, Dict[str, str]],
-        agents: Set[str],
+        config: PairwiseEvaluatorConfig,
         llm_provider: BaseLLMProvider,
     ):
-        super().__init__(config, queries, answers, agents, llm_provider)
-        if not self.config.output_file:
-            self.output_file = "pairwise_reasoning_evaluator.log"
-        else:
-            self.output_file = self.config.output_file
-        if not self.config.reasoning_file:
-            raise ValueError("Reasoning file is required for PairwiseWithReasoning")
+        super().__init__(config, llm_provider)
         self.k = self.config.k
         self.bidirectional = self.config.bidirectional
         self.pattern = re.compile(r"\[\[([^]]+)]].*$(?:(?!\[\[).)*", re.DOTALL)
-        self.reasoning = self._load_reasoning(self.config.reasoning_file)
-        self.evaluations: List[Dict[str, str]] = []
 
-    # def evaluate_single_answer(self, qid: str)
+    def batch_evaluate(self, queries: list[Query]) -> list[AnswerEvaluatorResult]:
+        failed_evaluations = 0
+        evaluations = [AnswerEvaluatorResult(**x) for x in self._get_existing_output()]
+        skip_tuples = {(x.qid, x.agent_a, x.agent_b) for x in evaluations}
+        tuples_to_eval = []
+        all_tuples = 0
+        queries = self._add_retrieved_documents_to_queries(
+            queries, documents_path=self.config.documents_path, text_column="answer"
+        )
+        for query in queries:
+            games_to_play = self.__prepare_tuples_for_query(query)
+            for answer_a, answer_b in games_to_play:
+                qid = query.qid
+                agent_a = answer_a.agent
+                agent_b = answer_b.agent
+                all_tuples += 1
+                if (qid, agent_a, agent_b) in skip_tuples:
+                    logger.debug(f"Skipping {qid} {agent_a} {agent_b}")
+                    continue
+                tuples_to_eval.append((query, answer_a, answer_b))
+        if len(tuples_to_eval) == 0:
+            logger.info("All answers have been evaluated")
+            if self.config.verbose:
+                print(
+                    f"All {all_tuples} answers are already evaluated.\n"
+                    "If you want to re-evaluate them, use the force flag"
+                )
+            return evaluations
 
-    def run(self) -> List[Dict[str, str]]:
-        use_progress_bar = self.config.verbose
-        unparsed_answers = 0
-        skip_tuples = set()
-        prompts = self.__create_all_prompts(use_progress_bar)
-        if os.path.exists(self.output_file) and not self.config.force:
-            for line in open(self.output_file):
-                data = json.loads(line)
-                qid = data["query_id"]
-                agent_a = data["agent_a"]
-                agent_b = data["agent_b"]
-                skip_tuples.add((qid, agent_a, agent_b))
-            logging.info(f"Skipping {len(skip_tuples)} games...")
-        if self.config.force and os.path.exists(self.output_file):
-            # remove the file
-            logging.info("Removing previous output file")
-            os.remove(self.output_file)
-        if len(prompts) - len(skip_tuples) > 0:
-            logging.info(f"Running {len(prompts) - len(skip_tuples)} games...")
-        for p in tqdm(
-            prompts,
+        for query, answer_a, answer_b in tqdm(
+            tuples_to_eval,
             desc="Evaluating games",
             disable=not self.config.verbose,
+            leave=False,
+            position=0,
             ncols=100,
         ):
-            qid = p["query_id"]
-            agent_a = p["agent_a"]
-            agent_b = p["agent_b"]
-            prompt_str = p["prompt"]
-            if (qid, agent_a, agent_b) in skip_tuples:
-                continue
-            logging.debug(f"Running query id {qid} agent {agent_a} vs {agent_b}")
+            agent_a = answer_a.agent
+            agent_b = answer_b.agent
             try:
-                llm_answer = self.llm_provider(prompt_str)
-            except RetryError:
-                logging.warning(
-                    f"Failed fetching answer for {qid}, {agent_a}, {agent_b}"
+                raw_answer, parsed_answer = self.evaluate_pairwise(
+                    query=query,
+                    answer_a=answer_a,
+                    answer_b=answer_b,
+                    retrieved_documents=query.retrieved_docs,
                 )
+
+            except (RetryError, ValueError):
+                failed_evaluations += 1
                 continue
-            logging.debug(llm_answer)
-            try:
-                relevant = self.__extract_relevant(llm_answer)
-            except ValueError:
-                unparsed_answers += 1
-                logging.warning(
-                    f"Failed extracting answer for {qid}, {agent_a}, {agent_b}."
-                    "Probably not enough tokens in the answer."
-                    f"Full answer:\n{llm_answer}",
+            evaluations.append(
+                AnswerEvaluatorResult(
+                    qid=query.qid,
+                    agent_a=agent_a,
+                    agent_b=agent_b,
+                    raw_answer=raw_answer,
+                    answer=parsed_answer,
                 )
-                continue
-            self.__print_response(qid, agent_a, agent_b, llm_answer, relevant)
-            self.__dump_response(
-                qid, agent_a, agent_b, prompt_str, llm_answer, relevant
             )
+            self._dump_response(evaluations[-1], self.output_columns, self.output_file)
         if self.config.verbose:
             print("✅ Done!")
-            print(f"Unparsed answers: {unparsed_answers}")
-            print(f"Total evaluations: {len(prompts) - unparsed_answers}")
-        return self.evaluations
+            print(f"Unparsed answers: {failed_evaluations}")
+            print(f"Total evaluations: {len(evaluations)}")
+        return evaluations
 
-    def __dump_response(
+    def evaluate_pairwise(
         self,
-        qid: str,
-        agent_a: str,
-        agent_b: str,
-        prompt_str: str,
-        llm_answer: str,
-        relevant: str,
-    ):
-        with open(self.output_file, "a") as f:
-            d = {
-                "query_id": qid,
-                "agent_a": agent_a,
-                "agent_b": agent_b,
-                "prompt": prompt_str,
-                "answer": llm_answer,
-                "relevant": relevant,
-            }
-            json.dump(d, f)
-            f.write("\n")
-            self.evaluations.append(d)
+        query: Query | str,
+        answer_a: AgentAnswer | str,
+        answer_b: AgentAnswer | str,
+        retrieved_documents: list[str] | list[Document],
+        query_metadata: Optional[dict[str, Any]] = None,
+        answer_a_metadata: Optional[dict[str, Any]] = None,
+        answer_b_metadata: Optional[dict[str, Any]] = None,
+        document_metadata: Optional[list[dict[str, Any]]] = None,
+    ) -> tuple[str, str]:
+        query = self._assemble_query(query, query_metadata)
+        answer_a = self._assemble_answer(answer_a, answer_a_metadata)
+        answer_b = self._assemble_answer(answer_b, answer_b_metadata)
+        if isinstance(retrieved_documents, str):
+            retrieved_documents = [retrieved_documents]
+        if retrieved_documents:
+            retrieved_and_assembled_docs = self._assemble_documents(
+                retrieved_documents, document_metadata
+            )
+            query.retrieved_docs = retrieved_and_assembled_docs
 
-    def __print_response(
-        self, qid: str, agent_a: str, agent_b: str, answer: str, relevant: str
-    ):
-        """Prints the response to the console"""
-        if not self.config.verbose:
-            return
-        if self.config.rich_print:
-            try:
-                import rich
+        prompt = self._build_message_pairwise(query, (answer_a, answer_b))
+        qid = query.qid
+        agent_a_id = answer_a.agent
+        agent_b_id = answer_b.agent
+
+        try:
+            raw_answer = self.llm_provider(prompt)
+        except RetryError as e:
+            logger.warning(
+                f"Failed to FETCH answers for {qid} {agent_a_id}, {agent_b_id}"
+            )
+            raise e
+        try:
+            processed_answer = self._process_answer(raw_answer)
+        except ValueError as e:
+            logger.warning(
+                f"Failed extracting answer for {qid}, {agent_a_id}, {agent_b_id}."
+                "Probably not enough tokens in the answer."
+                f"Full answer:\n{raw_answer}",
+            )
+            raise e
+        return raw_answer, processed_answer
 
-                rich.print(
-                    f"[not bold white][{qid}][/not bold white] "
-                    f"[bold blue] {agent_a:<18} [/bold blue] 🆚  "
-                    f"[bold red] {agent_b}[/bold red]"
-                )
-                rich.print("[bold white] Evaluator answer: [/bold white]")
-                if relevant == "A":
-                    parser_ans = answer.replace("[[A]]", "[bold blue]A[/bold blue]")
-                elif relevant == "B":
-                    parser_ans = answer.replace("[[B]]", "[bold red]B[/bold red]")
-                else:
-                    parser_ans = answer.replace("[[C]]", "[bold purple]C[/bold purple]")
-                    rich.print(parser_ans)
-            except ImportError:
-                logging.warning("Rich not installed. Using plain print")
-                self.config.rich_print = False
-            print(f"{qid}: {agent_a} vs {agent_b}")
-            print(f"Evaluator full answer: {answer}")
-
-    def __generate_random_games(self) -> List[Tuple[str, str]]:
-        """Creates all prompts necessary for running the evaluator"""
-        total_agents = len(self.agents)
-        _agents = list(self.agents)
-        if self.k == -1:
-            logging.info("Creating all possible games...")
-            pairs = []
-            for i in range(total_agents):
-                for j in range(i + 1, total_agents):
-                    pairs.append((_agents[i], _agents[j]))
-            random.shuffle(pairs)
-            return pairs
-        rounds_per_agent = self.k // total_agents
-        leftover_rounds = self.k % total_agents
-
-        extra_samples_1 = random.sample(_agents, k=leftover_rounds)
-        extra_samples_2 = random.sample(_agents, k=leftover_rounds)
-
-        first_agents = _agents * rounds_per_agent + extra_samples_1
-        second_agents = _agents * rounds_per_agent + extra_samples_2
-
-        # Shuffle both lists
-        random.shuffle(first_agents)
-        random.shuffle(second_agents)
-
-        # use deque to pop from the left
-        first_agents_q = deque(first_agents)
-        second_agents_q = deque(second_agents)
-
-        used_pairs = set()  # avoid re-using pairs
-        pairs = []
-        while first_agents_q and len(pairs) < self.k:
-            agent_a = first_agents_q.popleft()
-
-            for _ in range(len(second_agents)):
-                agent_b = second_agents_q.popleft()
-                if agent_b != agent_a and (agent_a, agent_b) not in used_pairs:
-                    used_pairs.add((agent_a, agent_b))
-                    pairs.append((agent_a, agent_b))
-                    logging.debug(f"Created game {agent_a} vs {agent_b}")
-                    if self.bidirectional:
-                        pairs.append((agent_b, agent_a))
-                        used_pairs.add((agent_b, agent_a))
-                        logging.debug(f"Created game {agent_b} vs {agent_a}")
-                    second_agents_q.append(agent_b)
-                    break
-                second_agents_q.append(agent_b)
-        logging.info(f"Created {len(pairs)} games")
-        return pairs
-
-    def __create_all_prompts(
-        self, use_progress_bar: bool = True
-    ) -> List[Dict[str, str]]:
-        prompts = []
-        random_pairs = self.__generate_random_games()
-        for qid in tqdm(
-            self.answers,
-            desc="Creating prompts",
-            disable=not use_progress_bar,
-            ncols=100,
-        ):
-            query = self.queries[qid].query
-            for a, b in random_pairs:
-                if a not in self.answers[qid] or b not in self.answers[qid]:
-                    continue
-                reasoning = "\n".join(
-                    list(
-                        [
-                            " ".join([f"[{a}]", b])
-                            for (a, b) in self.reasoning[qid].items()
-                        ]
-                    )
-                )
-                ans_a = self.answers[qid][a].strip()
-                ans_b = self.answers[qid][b].strip()
-                prompt = self.prompt.format(
-                    query=query, documents=reasoning, answer_a=ans_a, answer_b=ans_b
-                )
-                prompts.append(
-                    {"query_id": qid, "agent_a": a, "agent_b": b, "prompt": prompt}
-                )
-        return prompts
+    def _build_message_pairwise(
+        self, query: Query, answer: AgentAnswer | tuple[AgentAnswer, AgentAnswer]
+    ) -> str:
+        assert isinstance(answer, tuple)
+        reasonings = self._prepare_documents(query)
+        query_metadata = self._get_usable_fields_from_metadata(
+            self.prompt, query.metadata, skip_fields=[self.config.query_placeholder]
+        )
+        answer_a_metadata = self._get_usable_fields_from_metadata(
+            self.prompt,
+            answer[0].metadata,
+            skip_fields=[self.config.answer_placeholder],
+        )
+        answer_b_metadata = self._get_usable_fields_from_metadata(
+            self.prompt,
+            answer[1].metadata,
+            skip_fields=[self.config.answer_placeholder],
+        )
+        formatters = {
+            self.config.query_placeholder: query.query,
+            self.config.documents_placeholder: reasonings,
+            "answer_a": answer[0].text,
+            "answer_b": answer[1].text,
+            **query_metadata,
+            **answer_a_metadata,
+            **answer_b_metadata,
+        }
+        return self.prompt.format(**formatters)
+
+    def __generate_games_per_query(self, query: Query) -> list[tuple[str, str]]:
+        """Generates up to self.k random pairs of agents for the given query"""
+        query_agents = list({x.agent for x in query.answers})
+        # Create all possible pairs
+        pairs = [(a, b) for a in query_agents for b in query_agents if a != b]
+        if self.bidirectional:
+            pairs += [(b, a) for a, b in pairs]
+        random.shuffle(pairs)
+        return pairs[: self.k]
 
-    def _check_validity(self):
-        total_agents = len(self.agents)
-        if total_agents < 2:
-            raise ValueError(f"Need at least 2 agents, found {total_agents}")
-        logging.info(f"Loaded {total_agents} agents")
-        if (total_agents * (total_agents - 1)) < self.k:
-            possible_games = total_agents * (total_agents - 1)
-            logging.warning(
-                f"Requested {self.k} games but only {possible_games} are possible"
-            )
-            logging.warning(f"Will create {possible_games} games per query instead")
-            self.k = possible_games
+    def __prepare_tuples_for_query(
+        self,
+        query: Query,
+    ) -> list[tuple[AgentAnswer, AgentAnswer]]:
+        all_tuples = []
+        answers = {}
+        for agent_answer in query.answers:
+            answers[agent_answer.agent] = agent_answer
+        random_pairs = self.__generate_games_per_query(query)
+        for agent_a, agent_b in random_pairs:
+            all_tuples.append((answers[agent_a], answers[agent_b]))
+        return all_tuples
 
-    def __extract_relevant(self, answer: str) -> str:
+    def _process_answer(self, answer: str) -> str:
         """Extracts the relevant part of an answer."""
         match_ans = self.pattern.search(answer)
         if not match_ans:
             raise ValueError(f"Could not find answer in {answer}")
         answer = match_ans.group(1)
         if answer not in ["A", "B", "C"]:
             raise ValueError(f"Unknown answer: {answer}")
         return answer
 
-    def _load_reasoning(self, reasoning_path: str) -> Dict[str, Dict[str, str]]:
-        reasoning: Dict[str, Dict[str, str]] = defaultdict(lambda: dict())
+    def _build_message(
+        self, query: Query, answer: AgentAnswer
+    ) -> str | list[dict[str, str]]:
+        raise NotImplementedError
+
+    @staticmethod
+    def _load_reasonings(
+        reasoning_path: str,
+        query_id_col: str = "qid",
+        document_id_col: str = "did",
+        answer_col: str = "answer",
+    ) -> dict[str, dict[str, str]]:
+        reasoning: dict[str, dict[str, str]] = defaultdict(lambda: dict())
         reasoning_read = 0
+        if not os.path.exists(reasoning_path):
+            raise FileNotFoundError(f"Reasoning file {reasoning_path} not found")
+
+        logger.info(f"Loading reasonings from {reasoning_path}")
         for line in csv.DictReader(open(reasoning_path)):
-            if line["query_id"] not in self.queries:
-                continue
             reasoning_read += 1
-            reasoning[line["query_id"]][line["did"]] = line["answer"]
-        logging.info(f"Loaded {reasoning_read} reasonings")
+            reasoning[line[query_id_col]][line[document_id_col]] = line[answer_col]
+        logger.info(f"Loaded {reasoning_read} reasonings")
         return dict(reasoning)
```

### Comparing `ragelo-0.0.5/ragelo/evaluators/retrieval_evaluators/base_retrieval_evaluator.py` & `ragelo-0.1.1/ragelo/evaluators/retrieval_evaluators/base_retrieval_evaluator.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,208 +1,214 @@
 """A Retrieval Evaluator is a class that evaluates the results of a retrieval system.
 It receives a set of queries used to retrieve a document and their respective retrieved documents,
 and returns a score or a label for each document."""
 
-import csv
-import logging
-import os
-from abc import abstractmethod
-from collections import defaultdict
-from typing import Any, Callable, Dict, List, Set, Tuple, Type
+# import dataclasses
+from typing import Any, Callable, Optional, Type, get_type_hints
 
 from tenacity import RetryError
 from tqdm.auto import tqdm
 
 from ragelo.evaluators.base_evaluator import BaseEvaluator
-from ragelo.llm_providers.base_llm_provider import BaseLLMProvider
-from ragelo.types import Document, Query
-from ragelo.types.configurations import RetrievalEvaluatorConfig
+from ragelo.llm_providers.base_llm_provider import BaseLLMProvider, get_llm_provider
+from ragelo.logger import logger
+from ragelo.types import (
+    AnswerFormat,
+    Document,
+    Query,
+    RetrievalEvaluatorResult,
+    RetrievalEvaluatorTypes,
+)
+from ragelo.types.configurations import BaseRetrievalEvaluatorConfig
 
 
 class BaseRetrievalEvaluator(BaseEvaluator):
+    config: BaseRetrievalEvaluatorConfig
+    output_columns: list[str] = ["qid", "did", "raw_answer", "answer"]
+    output_file: str = "retrieval_evaluations.csv"
+
     def __init__(
         self,
-        config: RetrievalEvaluatorConfig,
-        queries: Dict[str, Query],
-        documents: Dict[str, Dict[str, Document]],
+        config: BaseRetrievalEvaluatorConfig,
         llm_provider: BaseLLMProvider,
     ):
-        if not queries:
-            raise ValueError(
-                "You are trying to use a Retrieval Evaluator without providing queries"
-            )
-        if not documents:
-            raise ValueError(
-                "You are trying to use a Retrieval Evaluator without providing documents"
-            )
-        self.queries = queries
-        self.documents = documents
-        if not config.output_file:
-            self.output_file = "retrieval_evaluator.log"
-        else:
+        self.config = config
+        self.llm_provider = llm_provider
+        if config.output_file is not None:
             self.output_file = config.output_file
 
-        self.llm_provider = llm_provider
-        self.config = config
+        if config.answer_format == AnswerFormat.MULTI_FIELD_JSON:
+            if isinstance(config.scoring_key, str):
+                scoring_keys = [config.scoring_key]
+            else:
+                scoring_keys = config.scoring_key
+            self.output_columns = ["qid", "agent", "raw_answer"] + scoring_keys
+
+        if config.scoring_key and config.scoring_key not in self.output_columns:
+            print(f"Adding scoring key {config.scoring_key} to output columns")
+            self.output_columns.extend(self.config.scoring_key)
 
-    def run(self) -> Dict[str, Dict[str, str]]:
-        """Evaluate all the documents for each query"""
+    def batch_evaluate(self, queries: list[Query]) -> list[RetrievalEvaluatorResult]:
+        """Evaluate all the documents for a list of queries"""
         use_progress_bar = self.config.verbose
-        skip_docs = self.__get_skip_docs()
-        answers: Dict[str, Dict[str, str]] = defaultdict(lambda: dict())
-        for qid in tqdm(
-            self.queries,
-            desc="Annotating Documents",
+        answers = [RetrievalEvaluatorResult(**x) for x in self._get_existing_output()]
+        skip_docs = {(x.qid, x.did) for x in answers}
+        failed_evaluations = 0
+        tuples_to_eval = []
+        all_tuples = 0
+        for query in queries:
+            for document in query.retrieved_docs:
+                qid = query.qid
+                did = document.did
+                all_tuples += 1
+                if (qid, did) in skip_docs:
+                    logger.debug(f"Skipping {qid} {did}")
+                    continue
+                tuples_to_eval.append((query, document))
+        if len(tuples_to_eval) == 0:
+            logger.info("All documents have been evaluated")
+            if self.config.verbose:
+                print(
+                    f"All {all_tuples} documents are already evaluated.\n"
+                    "If you want to re-evaluate documents, use the --force flag."
+                )
+            return answers
+        for query, document in tqdm(
+            tuples_to_eval,
+            desc="Evaluating retrieved documents",
             disable=not use_progress_bar,
             ncols=100,
+            # leave=False,
+            position=0,
         ):
-            for did in tqdm(
-                self.documents[qid],
-                desc=qid,
-                disable=not use_progress_bar,
-                ncols=100,
-                leave=False,
-            ):
-                if (qid, did) in skip_docs:
-                    logging.debug(f"Skipping {qid} {did}")
-                    continue
+            qid = query.qid
+            did = document.did
+            try:
+                raw_answer, answer = self.evaluate(query, document)
+            except (RetryError, ValueError):
+                failed_evaluations += 1
+                continue
+
+            answers.append(
+                RetrievalEvaluatorResult(
+                    qid=qid,
+                    did=did,
+                    raw_answer=raw_answer,
+                    answer=answer,
+                )
+            )
+            self._dump_response(answers[-1], self.output_columns, self.output_file)
 
-                try:
-                    answer = self.evaluate_single_sample(qid, did)
-                except (RetryError, ValueError):
-                    continue
-                self._print_response(qid, did, answer)
-                self._dump_response(qid, did, answer)
-                answers[qid][did] = answer
+        if self.config.verbose:
+            print("✅ Done!")
+            print(f"Unparsed answers: {failed_evaluations}")
+            print(f"Total evaluations: {len(answers)}")
         return answers
 
-    def evaluate_single_sample(self, qid: str, did: str) -> str:
-        """Evaluates a single query-document pair"""
-        message = self._build_message(qid, did)
+    def evaluate(
+        self,
+        query: Query | str,
+        document: Document | str,
+        query_metadata: Optional[dict[str, Any]] = None,
+        doc_metadata: Optional[dict[str, Any]] = None,
+    ) -> tuple[str, Any]:
+        """Evaluates a single query-document pair. Returns the raw answer and the processed answer."""
+        if isinstance(query, str):
+            query = Query(qid="<no_qid>", query=query)
+        if isinstance(document, str):
+            document = Document(did="<no_did>", text=document)
+        query.add_metadata(query_metadata)
+        document.add_metadata(doc_metadata)
+
+        message = self._build_message(query, document)
         try:
-            answer = self.llm_provider(message)
+            raw_answer = self.llm_provider(message)
         except RetryError as e:
-            logging.warning(f"Failed to FETCH answers for {qid} {did}")
+            logger.warning(
+                f"Failed to FETCH answers for qid: {query.qid} did: {document.did}"
+            )
             raise e
         try:
-            answer = self._process_answer(answer)
+            answer = self._process_answer(raw_answer)
         except ValueError as e:
-            logging.warning(f"Failed to PARSE answer for {qid} {did}")
+            logger.warning(
+                f"Failed to PARSE answer for qid: {query.qid} did: {document.did}"
+            )
             raise e
-        return answer
+        return raw_answer, answer
 
-    @abstractmethod
-    def _build_message(self, qid: str, did: str) -> str:
+    def _build_message(
+        self, query: Query, document: Document
+    ) -> str | list[dict[str, str]]:
         """Builds the prompt to send to the LLM."""
         raise NotImplementedError
 
-    @abstractmethod
-    def _process_answer(self, answer: str) -> Any:
-        """Processes the LLM evaluator output into some serializable format"""
-        raise NotImplementedError
-
-    def __get_skip_docs(self) -> Set[Tuple[str, str]]:
-        """Skips documents that have already been annotated"""
-        skip_docs = set()
-        if os.path.isfile(self.output_file) and not self.config.force:
-            for line in csv.reader(open(self.output_file)):
-                qid, did, _ = line
-                skip_docs.add((qid, did))
-        if self.config.force and os.path.isfile(self.output_file):
-            logging.warning(f"Removing existing {self.output_file}!")
-            os.remove(self.output_file)
-        if len(skip_docs) > 0:
-            logging.warning(
-                f"Skipping {len(skip_docs)} documents already annotated! "
-                "If you want to re-annotate them, please use the --force flag"
-            )
-        return skip_docs
-
-    def _print_response(self, qid: str, did: str, answer: str) -> None:
-        if not self.config.verbose:
-            return
-        if self.config.rich_print:
-            try:
-                import rich
-
-                rich.print(
-                    "[bold cyan]🔎Query       [/bold cyan]: [not bold cyan]"
-                    f"{self.queries[qid].query}[/not bold cyan]"
-                )
-                rich.print(f"[bold cyan]Document ID [/bold cyan]: {did}")
-                rich.print(
-                    f"[bold cyan]Evaluation  [/bold cyan]: [not bold]{answer}[/not bold]"
-                )
-                rich.print("")
-
-            except ImportError:
-                logging.warning("Rich not installed. Using plain print")
-                self.config.rich_print = False
-
-        else:
-            print(
-                f"Query: {self.queries[qid].query}, Document ID: {did}, Evaluation: {answer}"
-            )
-
-    def _dump_response(
-        self,
-        qid: str,
-        did: str,
-        answer: str,
-        file: str | None = None,
-    ) -> None:
-        output_file = file if file else self.output_file
-        if not os.path.isfile(output_file):
-            logging.debug(f"Creating new file {output_file}")
-            with open(output_file, "w") as f:
-                writer = csv.writer(f)
-                writer.writerow(["query_id", "did", "answer"])
-
-        with open(output_file, "a") as f:
-            writer = csv.writer(f)
-            if isinstance(answer, List):
-                answer = "\n".join(answer)
-            writer.writerow([qid, did, answer])
-
-    @staticmethod
-    def _load_from_csv(file_path: str) -> Dict[str, str]:
-        """extra content from a CSV file"""
-        contents = {}
-        for line in csv.reader(open(file_path, "r")):
-            contents[line[0]] = line[1]
-        return contents
-
     @classmethod
     def from_config(
-        cls, config: RetrievalEvaluatorConfig, llm_provider: BaseLLMProvider
+        cls, config: BaseRetrievalEvaluatorConfig, llm_provider: BaseLLMProvider
     ):
-        queries = cls._load_queries(config.query_path)
-        documents = cls.load_documents(config.documents_path, queries)
-        return cls(config, queries, documents, llm_provider)
+        return cls(config, llm_provider)
 
-    def __len__(self) -> int:
-        return len(self.queries)
+    @classmethod
+    def get_config_class(cls) -> Type[BaseRetrievalEvaluatorConfig]:
+        return get_type_hints(cls)["config"]
+
+    @staticmethod
+    def _construct_list_of_answers(
+        answers: list[dict[str, str]]
+    ) -> list[RetrievalEvaluatorResult]:
+        return [RetrievalEvaluatorResult(**x) for x in answers]
 
 
 class RetrievalEvaluatorFactory:
-    registry: Dict[str, Type[BaseRetrievalEvaluator]] = {}
+    registry: dict[RetrievalEvaluatorTypes | str, Type[BaseRetrievalEvaluator]] = {}
 
     @classmethod
-    def register(cls, evaluator_name: str) -> Callable:
+    def register(cls, evaluator_name: RetrievalEvaluatorTypes) -> Callable:
         def inner_wrapper(
             wrapped_class: Type[BaseRetrievalEvaluator],
         ) -> Type[BaseRetrievalEvaluator]:
+            if evaluator_name in cls.registry:
+                logger.debug(f"Overwriting {evaluator_name} in registry")
             cls.registry[evaluator_name] = wrapped_class
             return wrapped_class
 
         return inner_wrapper
 
     @classmethod
     def create(
         cls,
-        evaluator_name: str,
-        config: RetrievalEvaluatorConfig,
-        llm_provider: BaseLLMProvider,
+        evaluator_name: RetrievalEvaluatorTypes | str,
+        llm_provider: BaseLLMProvider | str,
+        config: Optional[BaseRetrievalEvaluatorConfig] = None,
+        **kwargs,
     ) -> BaseRetrievalEvaluator:
+        if isinstance(llm_provider, str):
+            llm_provider_instance = get_llm_provider(llm_provider, **kwargs)
+        else:
+            llm_provider_instance = llm_provider
         if evaluator_name not in cls.registry:
-            raise ValueError(f"Unknown evaluator {evaluator_name}")
-        return cls.registry[evaluator_name].from_config(config, llm_provider)
+            raise ValueError(
+                f"Unknown retrieval evaluator {evaluator_name}\n"
+                f"Valid options are {list(cls.registry.keys())}"
+            )
+        if config is None:
+            class_ = cls.registry[evaluator_name]
+            type_config = class_.get_config_class()
+            valid_keys = [field for field in type_config.get_model_fields()]
+            valid_args = {k: v for k, v in kwargs.items() if k in valid_keys}
+            config = type_config(**valid_args)
+        return cls.registry[evaluator_name].from_config(config, llm_provider_instance)
+
+
+def get_retrieval_evaluator(
+    evaluator_name: RetrievalEvaluatorTypes | str,
+    llm_provider: BaseLLMProvider | str,
+    config: Optional[BaseRetrievalEvaluatorConfig] = None,
+    **kwargs,
+) -> BaseRetrievalEvaluator:
+    return RetrievalEvaluatorFactory.create(
+        evaluator_name,
+        llm_provider=llm_provider,
+        config=config,
+        **kwargs,
+    )
```

### Comparing `ragelo-0.0.5/ragelo/evaluators/retrieval_evaluators/domain_expert_evaluator.py` & `ragelo-0.1.1/ragelo/evaluators/retrieval_evaluators/domain_expert_evaluator.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,68 +1,101 @@
 """Evaluator with a domain expert persona"""
 
 import logging
-from typing import Dict
+from typing import Any, Optional
 
 from tenacity import RetryError
 
 from ragelo.evaluators.retrieval_evaluators import (
     BaseRetrievalEvaluator,
     RetrievalEvaluatorFactory,
 )
 from ragelo.llm_providers.base_llm_provider import BaseLLMProvider
-from ragelo.types import Document, Query
-from ragelo.types.configurations import RetrievalEvaluatorConfig
+from ragelo.types import Document, Query, RetrievalEvaluatorTypes
+from ragelo.types.configurations import DomainExpertEvaluatorConfig
 
 
-@RetrievalEvaluatorFactory.register("domain_expert")
+@RetrievalEvaluatorFactory.register(RetrievalEvaluatorTypes.DOMAIN_EXPERT)
 class DomainExpertEvaluator(BaseRetrievalEvaluator):
-    sys_prompt = """You are a domain expert in {domain_long}.{company_prompt_1} You are tasked with evaluating the performance of a retrieval system for question answering in this domain. The question answering system will be used by internal users{company_prompt_2}{domain_short}. They are interested in a retrieval system that provides relevant passages based on their questions."""
-
-    reason_prompt = """Query: {query}
-Document passage: {doc_content}
-Please think in steps about the relevance of the retrieved document given the original query. Consider the query, the document title, and the document passage. Reason whether the document is not relevant to the query, somewhat relevant to the query, or highly relevant to the query.
+    sys_prompt = """
+You are a domain expert in {domain_long}.{company_prompt_1} You are tasked \
+with evaluating the performance of a retrieval system for question \
+answering in this domain. The question answering system will be used \
+by internal users{company_prompt_2}{domain_short}. They are interested \
+in a retrieval system that provides relevant passages based on their questions.
+""".strip()
+
+    reason_prompt = """
+User query:
+{query}
+
+Document passage:
+{doc_content}
+
+Please think in steps about the relevance of the retrieved document given the \
+original query. Consider the query, the document title, and the document \
+passage. Reason whether the document is not relevant to the query, somewhat relevant \
+to the query, or highly relevant to the query.
 Use the following guidelines to reason about the relevance of the retrieved document:
 - Not Relevant:
-    The document contains information that is unrelated, outdated, or completely irrelevant to the query.
-    The document may contain some keywords or phrases from the query, but the context and overall meaning do not align with the query's intent.
-    The document may be from a different field or time period, rendering it irrelevant to the current query.
+    The document contains information that is unrelated, outdated, or completely \
+irrelevant to the query.
+    The document may contain some keywords or phrases from the query, but the context \
+and overall meaning do not align with the query's intent.
+    The document may be from a different field or time period, rendering it irrelevant \
+to the current query.
 - Somewhat Relevant:
-    The document contains some relevant information but lacks comprehensive details or context.
-    The document may discuss a related topic or concept but not directly address the query.
-    The information in the document is tangentially related to the query, but the primary focus remains different.
+    The document contains some relevant information but lacks comprehensive details \
+or context.
+    The document may discuss a related topic or concept but not directly address the \
+query.
+    The information in the document is tangentially related to the query, but the \
+primary focus remains different.
 - Highly Relevant:
-    The document directly addresses the main points of the query and provides comprehensive and accurate information.
+    The document directly addresses the main points of the query and provides \
+comprehensive and accurate information.
     The document may cite relevant information directly applicable to the query.
-    The document may be recent and from the same field as the query, enhancing its relevance.
+    The document may be recent and from the same field as the query, enhancing its \
+relevance.
 General Guidelines:
-    - Context Matters: Annotators should evaluate the relevance of documents within the specific{domain_short} context provided by the query. Understanding the nuances and domain-specific terminology is essential.
-    - Content Overlap: Consider the extent of content overlap between the document and the query. Assess whether the document covers the core aspects of the query or only peripheral topics.
-    - Neutrality: Base judgments solely on the content's relevance and avoid any personal opinions or biases.
-    - Uncertainty: If uncertain about a relevance judgement, annotators default to a lower relevance.
-    {extra_guidelines}"""
-
-    score_prompt = """Given the previous reasoning, please assign a score of 0, 1, or 2 to the retrieved document given the particular query. The score meaning is as follows:
+    - Context Matters: Annotators should evaluate the relevance of documents within \
+the specific{domain_short} context provided by the query. Understanding the nuances \
+and domain-specific terminology is essential.
+    - Content Overlap: Consider the extent of content overlap between the document\
+and the query. Assess whether the document covers the core aspects of the query \
+or only peripheral topics.
+    - Neutrality: Base judgments solely on the content's relevance and avoid any \
+personal opinions or biases.
+    - Uncertainty: If uncertain about a relevance judgement, annotators default to a \
+lower relevance.
+    {extra_guidelines}
+""".strip()
+
+    score_prompt = """
+Given the previous reasoning, please assign a score of 0, 1, or 2 to the retrieved \
+document given the particular query. The score meaning is as follows:
 - 0: indicates that the retrieved document is not relevant to the query
 - 1: the document is somewhat relevant to the query
 - 2: the document is highly relevant to the query
-Please only answer with a single number."""
+Please only answer with a single number.
+""".strip()
 
     COMPANY_PROMPT_1 = " You work for {company}."
     COMPANY_PROMPT_2 = " of {company}"
     DOMAIN_SHORT = " but it also serves some of your external users like {domain_short}"
+    config: DomainExpertEvaluatorConfig
+    output_columns: list[str] = ["qid", "did", "reasoning", "score"]
+    output_file: str = "domain_expert_evaluations.csv"
 
     def __init__(
         self,
-        config: RetrievalEvaluatorConfig,
-        queries: Dict[str, Query],
-        documents: Dict[str, Dict[str, Document]],
+        config: DomainExpertEvaluatorConfig,
         llm_provider: BaseLLMProvider,
     ):
-        super().__init__(config, queries, documents, llm_provider)
+        super().__init__(config, llm_provider)
         if not self.config.domain_long:
             raise ValueError(
                 "You are tying to use the Domain Expert Retrieval Evaluator. "
                 "For this evaluator, you need to provide at least the name of the domain "
                 "in the domain_long field."
             )
 
@@ -85,58 +118,66 @@
             domain_short=(
                 self.DOMAIN_SHORT.format(domain_short=self.config.domain_short)
                 if self.config.domain_short
                 else ""
             ),
         )
         self.extra_guidelines = (
-            self.config.extra_guidelines if self.config.extra_guidelines else ""
+            self.config.extra_guidelines if self.config.extra_guidelines else []
         )
-        self.reasoning_file = self.output_file.replace(".csv", "_reasoning.csv")
 
-    def __build_reason_message(self, qid: str, did: str) -> str:
-        query = self.queries[qid].query
-        document = self.documents[qid][did].text
+    def __build_reason_message(self, query: Query, document: Document) -> str:
+        guidelines = "\n".join(
+            [f"- {guideline}" for guideline in self.extra_guidelines]
+        )
         reason_prompt = self.reason_prompt.format(
-            query=query,
-            doc_content=document,
+            query=query.query,
+            doc_content=document.text,
             domain_short=self.domain_short if self.domain_short else "",
-            extra_guidelines=self.extra_guidelines if self.extra_guidelines else "",
+            extra_guidelines=guidelines,
         )
         return reason_prompt
 
-    def evaluate_single_sample(self, qid: str, did: str) -> str:
+    def evaluate(
+        self,
+        query: Query | str,
+        document: Document | str,
+        query_metadata: Optional[dict[str, Any]] = None,
+        doc_metadata: Optional[dict[str, Any]] = None,
+    ) -> tuple[str, Any]:
         """Processes a single pair of qid, did in a two-shot manner"""
-        reason_message = self.__build_reason_message(qid, did)
+        if isinstance(query, str):
+            query = Query(qid="<no_qid>", query=query)
+        if isinstance(document, str):
+            document = Document(did="<no_did>", text=document)
+        query.add_metadata(query_metadata)
+        document.add_metadata(doc_metadata)
+
+        qid = query.qid
+        did = document.did
+        reason_message = self.__build_reason_message(query, document)
         messages_reasoning = [
             {"role": "system", "content": self.sys_prompt},
             {"role": "user", "content": reason_message},
         ]
         try:
-            answer = self.llm_provider(messages_reasoning)
+            reasoning_answer = self.llm_provider(messages_reasoning)
+
         except RetryError as e:
             logging.warning(f"Failed to fetch reasoning for document {qid} {did}")
             raise e
         except ValueError as e:
             logging.warning(f"Failed to parse reasoning for document {qid} {did}")
             raise e
-        self._print_response(qid, did, answer=f"Reasoning: {answer}")
-        self._dump_response(qid, did, answer, self.reasoning_file)
 
         messages_score = messages_reasoning.copy()
-        messages_score.append({"role": "assistant", "content": answer})
+        messages_score.append({"role": "assistant", "content": reasoning_answer})
         messages_score.append({"role": "user", "content": self.score_prompt})
         try:
-            answer = self.llm_provider(messages_score)
+            score_answer = self._process_answer(self.llm_provider(messages_score))
         except RetryError as e:
             logging.warning(f"Failed to fetch evaluation for document {qid} {did}")
             raise e
         except ValueError as e:
             logging.warning(f"Failed to parse evaluation for document {qid} {did}")
             raise e
-        return answer
-
-    def _build_message(self, qid: str, did: str) -> str:
-        return self.sys_prompt
-
-    def _process_answer(self, answer: str) -> str:
-        return answer
+        return reasoning_answer, score_answer
```

### Comparing `ragelo-0.0.5/ragelo/evaluators/retrieval_evaluators/rdnam_evaluator.py` & `ragelo-0.1.1/ragelo/evaluators/retrieval_evaluators/rdnam_evaluator.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 """Evaluator based on the paper: Paul Thomas, Seth Spielman, Nick Craswell and
 Bhaskar Mitra. Large language models can accurately predict searcher preferences.
 https://arxiv.org/abs/2309.10621
 """
 
 import json
-import logging
-from typing import Dict
 
 import numpy as np
 
 from ragelo.evaluators.retrieval_evaluators.base_retrieval_evaluator import (
     BaseRetrievalEvaluator,
     RetrievalEvaluatorFactory,
 )
 from ragelo.llm_providers.base_llm_provider import BaseLLMProvider
-from ragelo.types import Document, Query
-from ragelo.types.configurations import RetrievalEvaluatorConfig
+from ragelo.types import Document, Query, RetrievalEvaluatorTypes
+from ragelo.types.configurations import RDNAMEvaluatorConfig
 
 
-@RetrievalEvaluatorFactory.register("RDNAM")
+@RetrievalEvaluatorFactory.register(RetrievalEvaluatorTypes.RDNAM)
 class RDNAMEvaluator(BaseRetrievalEvaluator):
-    prompt = """{role}Given a query and a document, you must provide a score on an integer scale of 0 to 2 with the following meanings:
+    prompt = """
+{role}Given a query and a document, you must provide a score on an integer scale \
+of 0 to 2 with the following meanings:
 2 = highly relevant, very helpful for this query
 1 = relevant, may be partly helpful but might contain other irrelevant content
 0 = not relevant, should never be shown for this query
-Assume that you are writing a report on the subject of the topic. If you would use any of the information contained in the document in such a report, mark it 1. If the document is primarily about the topic, or contains vital information about the topic, mark it 2. Otherwise, mark it 0.
+Assume that you are writing a report on the subject of the topic. If you would \
+use any of the information contained in the document in such a report, mark it 1. \
+If the document is primarily about the topic, or contains vital information about \
+the topic, mark it 2. Otherwise, mark it 0.
 
 # Query
 A person has typed {query} into a search engine.
 {narrative_description}
 
 # Result
 Consider the following document.
@@ -36,109 +39,79 @@
 {doc_content}
 ---END DOCUMENT CONTENT---
 
 # Instructions
 Split this problem into steps:
 Consider the underlying intent of the search.
 {aspects}
-Consider the aspects above and relative importance of each, and decide on a final score (O).
+Consider the aspects above and relative importance of each, and decide on a final \
+score (O).
 {multiple}
 Produce a JSON array of scores without providing any reasoning. Example: {example}
 
 # Results
-"""  # noqa: E501
+""".strip()
 
-    NARRATIVE_DESCRIPTION_PROMPT = "They were looking for: {description} {narrative}"
-    ASPECTS_NARRATIVE = """Measure how well the content matches a likely intent of the query (M).
-    Measure how trustworthy the web page is (T)."""  # noqa: E501
+    NARRATIVE_DESCRIPTION_PROMPT = "They were looking for: {description}\n{narrative}"
+    ASPECTS_NARRATIVE = """Measure how well the content matches a likely intent \
+of the query (M).
+Measure how trustworthy the web page is (T).""".strip()
     ASPECTS_EXAMPLE = """[{{"M": 2, "T": 1, "O": 1}}, {{"M": 1..."""
     DEFAULT_EXAMPLE = """[{{"O": 1}}, {{"O": 2}}, {{"O": 0..."""
-    MULTIPLE_PROMPT = """We asked five search engine raters to evaluate the relevance of the web page for the query.
-Each rater used their own independent judgement."""  # noqa: E501
+    MULTIPLE_PROMPT = """We asked five search engine raters to evaluate \
+the relevance of the web page for the query.
+Each rater used their own independent judgement."""
+    config: RDNAMEvaluatorConfig
+    output_columns = ["qid", "did", "raw_answer", "answer"]
+    scoring_key = "answer"
+    output_file = "rdnam_evaluations.csv"
 
     def __init__(
         self,
-        config: RetrievalEvaluatorConfig,
-        queries: Dict[str, Query],
-        documents: Dict[str, Dict[str, Document]],
+        config: RDNAMEvaluatorConfig,
         llm_provider: BaseLLMProvider,
     ):
-        """Initializes an evaluator based on RDNAM framework.
-        Args:
-            role: A String defining the type of user the LLM should mimic
-                (e.g.: "You are a search quality rater evaluating
-                the relevance of web pages")
-            description: Will a description of the task be provided to the LLM?
-            narrative: Will a narrative of the task be provided to the LLM?
-            aspects: Should the prompt include aspects to get tot he final score?
-                If true, will prompt the LLM to compute scores for M (intent match)
-                and T (trustworthy) for the document before computing the final score.
-            multiple: Should the prompt ask the LLM to mimic multiple annotators?
-        """
-        super().__init__(config, queries, documents, llm_provider)
-        self.__role = self.config.role if self.config.role else ""
-        self.__use_narratives = False
-        self.__use_description = False
-
-        if self.config.narrative_file:
-            self.__narratives: Dict[str, str] = self._load_from_csv(
-                self.config.narrative_file
-            )
-            self.__use_narratives = True
-        if self.config.description_file:
-            self.descriptions: Dict[str, str] = self._load_from_csv(
-                self.config.description_file
-            )
-            self.__use_description = True
-
-        self.__aspects_prompt = self.ASPECTS_NARRATIVE if self.config.aspects else ""
-        self.multiple_prompt = self.MULTIPLE_PROMPT if self.config.multiple else ""
-        if self.config.multiple:
+        """Initializes an evaluator based on RDNAM framework."""
+        super().__init__(config, llm_provider)
+
+        self.__role = self.config.annotator_role if self.config.annotator_role else ""
+
+        self.__aspects_prompt = (
+            self.ASPECTS_NARRATIVE if self.config.use_aspects else ""
+        )
+        self.__multiple_prompt = (
+            self.MULTIPLE_PROMPT if self.config.use_multiple_annotators else ""
+        )
+        if self.config.use_multiple_annotators:
             self.prompt += "\n[{{"
         else:
             self.prompt += "\n{{"
-        self.multiple = self.config.multiple
+        self.multiple = self.config.use_multiple_annotators
 
-    def _build_message(
-        self,
-        qid: str,
-        did: str,
-    ) -> str:
-        if self.__use_narratives and qid not in self.__narratives:
-            logging.warning(f"No narrative found for {qid}. Will not use it")
-        if self.__use_description and qid not in self.descriptions:
-            logging.warning(f"No description found for {qid}. Will not use it")
-
-        narrative = (
-            self.__narratives[qid]
-            if qid in self.__narratives and self.__use_narratives
-            else ""
-        )
-        description = (
-            self.descriptions[qid]
-            if qid in self.descriptions and self.__use_description
-            else ""
-        )
-        narrative_description_str = self.NARRATIVE_DESCRIPTION_PROMPT.format(
-            narrative=narrative, description=description
-        )
-        query = self.queries[qid]
-        document = self.documents[qid][did]
+    def _build_message(self, query: Query, document: Document) -> str:
+        narrative_description_str = ""
+        if query.metadata:
+            description = query.metadata.get("description", "")
+            narrative = query.metadata.get("narrative", "")
+            if narrative or description:
+                narrative_description_str = self.NARRATIVE_DESCRIPTION_PROMPT.format(
+                    narrative=narrative, description=description
+                )
 
         example = (
             self.ASPECTS_EXAMPLE if self.__aspects_prompt else self.DEFAULT_EXAMPLE
         )
 
         formatted_prompt = self.prompt.format(
             role=self.__role,
-            query=query,
+            query=query.query,
             doc_content=document,
             narrative_description=narrative_description_str,
             aspects=self.__aspects_prompt,
-            multiple=self.multiple_prompt,
+            multiple=self.__multiple_prompt,
             example=example,
         )
         return formatted_prompt
 
     def _process_answer(self, answer: str) -> int:
         if self.multiple:
             answer = "[{" + answer
```

### Comparing `ragelo-0.0.5/ragelo/evaluators/retrieval_evaluators/reasoner_evaluator.py` & `ragelo-0.1.1/ragelo/evaluators/retrieval_evaluators/reasoner_evaluator.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,31 +1,41 @@
 from ragelo.evaluators.retrieval_evaluators.base_retrieval_evaluator import (
     BaseRetrievalEvaluator,
     RetrievalEvaluatorFactory,
 )
+from ragelo.types import Document, Query, RetrievalEvaluatorTypes
+from ragelo.types.configurations import ReasonerEvaluatorConfig
 
 
-@RetrievalEvaluatorFactory.register("reasoner")
+@RetrievalEvaluatorFactory.register(RetrievalEvaluatorTypes.REASONER)
 class ReasonerEvaluator(BaseRetrievalEvaluator):
     """
     A document Evaluator that only outputs the reasoning for why a document
     is relevant.
     """
 
-    prompt = """You are an expert document annotator, evaluating if a document contains relevant information to answer a question submitted by a user. Please act as an impartial relevance annotator for a search engine. Your goal is to evaluate the relevancy of the documents given a user question.
-    You should write one sentence explaining why the document is relevant or not for the user question. A document can be:
+    output_columns: list[str] = ["qid", "did", "raw_answer", "answer"]
+    output_file: str = "reasonings.csv"
+    config: ReasonerEvaluatorConfig
+    prompt = """
+You are an expert document annotator, evaluating if a document contains relevant \
+information to answer a question submitted by a user. \
+Please act as an impartial relevance annotator for a search engine. \
+Your goal is to evaluate the relevancy of the documents given a user question.
+
+You should write one sentence explaining why the document is relevant or not for \
+the user question. A document can be:
     - Not relevant: The document is not on topic.
-    - Somewhat relevant: The document is on topic but does not fully answer the user question.
+    - Somewhat relevant: The document is on topic but does not fully answer the \
+user question.
     - Very relevant: The document is on topic and answers the user question.
     [user question]
-    {user_question}
+    {query}
 
     [document content]
-    {doc_content}"""  # noqa: E501
+    {document}"""  # noqa: E501
 
-    def _build_message(self, qid: str, did: str) -> str:
-        query = self.queries[qid]
-        document = self.documents[qid][did]
-        return self.prompt.format(user_question=query.query, doc_content=document.text)
+    def _build_message(self, query: Query, document: Document) -> str:
+        return self.prompt.format(query=query.query, document=document.text)
 
     def _process_answer(self, answer: str) -> str:
         return answer
```

### Comparing `ragelo-0.0.5/ragelo/logger.py` & `ragelo-0.1.1/ragelo/logger.py`

 * *Files identical despite different names*

### Comparing `ragelo-0.0.5/ragelo.egg-info/SOURCES.txt` & `ragelo-0.1.1/ragelo.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,37 +1,51 @@
 LICENSE
 README.md
 pyproject.toml
 ragelo/__init__.py
 ragelo/__main__.py
-ragelo/cli.py
 ragelo/logger.py
+ragelo/utils.py
 ragelo.egg-info/PKG-INFO
 ragelo.egg-info/SOURCES.txt
 ragelo.egg-info/dependency_links.txt
 ragelo.egg-info/entry_points.txt
 ragelo.egg-info/requires.txt
 ragelo.egg-info/top_level.txt
-ragelo/answer_rankers/__init__.py
-ragelo/answer_rankers/base_answer_ranker.py
-ragelo/answer_rankers/elo_ranker.py
+ragelo/agent_rankers/__init__.py
+ragelo/agent_rankers/base_agent_ranker.py
+ragelo/agent_rankers/elo_ranker.py
+ragelo/cli/__init__.py
+ragelo/cli/agent_rankers_cmd.py
+ragelo/cli/answer_evaluators_cmd.py
+ragelo/cli/args.py
+ragelo/cli/cli.py
+ragelo/cli/retrieval_evaluator_cmd.py
+ragelo/cli/utils.py
 ragelo/evaluators/__init__.py
 ragelo/evaluators/base_evaluator.py
 ragelo/evaluators/answer_evaluators/__init__.py
 ragelo/evaluators/answer_evaluators/base_answer_evaluator.py
+ragelo/evaluators/answer_evaluators/custom_prompt_evaluator.py
 ragelo/evaluators/answer_evaluators/pairwise_reasoning_evaluator.py
 ragelo/evaluators/retrieval_evaluators/__init__.py
 ragelo/evaluators/retrieval_evaluators/base_retrieval_evaluator.py
+ragelo/evaluators/retrieval_evaluators/custom_prompt_evaluator.py
 ragelo/evaluators/retrieval_evaluators/domain_expert_evaluator.py
+ragelo/evaluators/retrieval_evaluators/few_shot_evaluator.py
 ragelo/evaluators/retrieval_evaluators/rdnam_evaluator.py
 ragelo/evaluators/retrieval_evaluators/reasoner_evaluator.py
 ragelo/llm_providers/__init__.py
 ragelo/llm_providers/base_llm_provider.py
 ragelo/llm_providers/openai_client.py
 ragelo/types/__init__.py
-ragelo/types/configurations.py
 ragelo/types/types.py
-ragelo/utils/__init__.py
+ragelo/types/configurations/__init__.py
+ragelo/types/configurations/agent_ranker_configs.py
+ragelo/types/configurations/answer_evaluator_configs.py
+ragelo/types/configurations/base_configs.py
+ragelo/types/configurations/llm_provider_configs.py
+ragelo/types/configurations/retrieval_evaluator_configs.py
 tests/conftest.py
 tests/unit/test_answer_evaluators.py
 tests/unit/test_llm_providers.py
 tests/unit/test_retrieval_evaluators.py
```

### Comparing `ragelo-0.0.5/tests/unit/test_llm_providers.py` & `ragelo-0.1.1/tests/unit/test_llm_providers.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,18 +1,22 @@
-from openai.types.chat.chat_completion import (
-    ChatCompletion,
-    ChatCompletionMessage,
-    Choice,
-)
+from openai.types.chat.chat_completion import ChatCompletion, Choice
+from openai.types.chat.chat_completion_message import ChatCompletionMessage
 
+from ragelo import get_llm_provider
 from ragelo.llm_providers.openai_client import OpenAIProvider
 
 
 class TestOpenAIProvider:
-    def test_response(self, chat_completion_mock, openai_client_mock):
+    def test_response(
+        self,
+        chat_completion_mock,
+        openai_client_mock,
+        openai_client_config,
+        monkeypatch,
+    ):
         chat_completion_mock.create.return_value = ChatCompletion(
             id="fake id",
             choices=[
                 Choice(
                     finish_reason="stop",
                     index=0,
                     logprobs=None,
@@ -21,20 +25,28 @@
                     ),
                 )
             ],
             created=0,
             model="fake model",
             object="chat.completion",
         )
-        openai_client = OpenAIProvider(openai_client_mock, "fake model")
+        openai_client = OpenAIProvider(config=openai_client_config)
+        monkeypatch.setattr(
+            openai_client, "_OpenAIProvider__openai_client", openai_client_mock
+        )
+
         prompt = "hello world"
         prompts = [
             {"role": "system", "content": "hello world"},
             {"role": "user", "content": "hello openai"},
         ]
         result_1 = openai_client(prompt)
         openai_client(prompts)
         call_args = chat_completion_mock.create.call_args_list
         assert call_args[0][1]["model"] == "fake model"
         assert call_args[0][1]["messages"] == [{"role": "system", "content": prompt}]
         assert call_args[1][1]["messages"] == prompts
         assert result_1 == "fake response"
+
+    def test_get_by_name(self, openai_client_config, openai_client_mock):
+        provider = get_llm_provider("openai", api_key="fake key")
+        assert isinstance(provider, OpenAIProvider)
```

