# Comparing `tmp/qdls-0.1.4.tar.gz` & `tmp/qdls-0.1.5.tar.gz`

## Comparing `qdls-0.1.4.tar` & `qdls-0.1.5.tar`

### file list

```diff
@@ -1,102 +1,102 @@
--rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 qdls-0.1.4/.github/workflows/publish.yml
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 qdls-0.1.4/src/qdls/__init__.py
--rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 qdls-0.1.4/src/qdls/cli.py
--rw-r--r--   0        0        0    11340 2020-02-02 00:00:00.000000 qdls-0.1.4/src/qdls/data.py
--rw-r--r--   0        0        0     3796 2020-02-02 00:00:00.000000 qdls-0.1.4/src/qdls/losses.py
--rw-r--r--   0        0        0     2815 2020-02-02 00:00:00.000000 qdls-0.1.4/src/qdls/metrics.py
--rw-r--r--   0        0        0     4282 2020-02-02 00:00:00.000000 qdls-0.1.4/src/qdls/tensor_ops.py
--rw-r--r--   0        0        0     2338 2020-02-02 00:00:00.000000 qdls-0.1.4/src/qdls/utils.py
--rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 qdls-0.1.4/src/qdls/code_template/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qdls-0.1.4/src/qdls/code_template/notebooks/statis.ipynb
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 qdls-0.1.4/src/qdls/code_template/preliminary/example.py
--rw-r--r--   0        0        0     4095 2020-02-02 00:00:00.000000 qdls-0.1.4/src/qdls/code_template/src/frame.py
--rw-r--r--   0        0        0     1374 2020-02-02 00:00:00.000000 qdls-0.1.4/src/qdls/code_template/src/main.py
--rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 qdls-0.1.4/src/qdls/code_template/src/pl_callbacks.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qdls-0.1.4/src/qdls/code_template/src/utils.py
--rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 qdls-0.1.4/src/qdls/code_template/src/configs/example.yaml
--rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 qdls-0.1.4/src/qdls/code_template/src/data_utils/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qdls-0.1.4/src/qdls/code_template/src/data_utils/common.py
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 qdls-0.1.4/src/qdls/code_template/src/models/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qdls-0.1.4/src/qdls/deprecate/__init__.py
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 qdls-0.1.4/src/qdls/deprecate/data.py
--rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 qdls-0.1.4/src/qdls/deprecate/loggers.py
--rw-r--r--   0        0        0    13330 2020-02-02 00:00:00.000000 qdls-0.1.4/src/qdls/deprecate/object.py
--rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 qdls-0.1.4/src/qdls/deprecate/optim.py
--rw-r--r--   0        0        0    13611 2020-02-02 00:00:00.000000 qdls-0.1.4/src/qdls/deprecate/pretrains.py
--rw-r--r--   0        0        0     3598 2020-02-02 00:00:00.000000 qdls-0.1.4/src/qdls/deprecate/test.py
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 qdls-0.1.4/src/qdls/deprecate/train.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qdls-0.1.4/src/qdls/draw/__init__.py
--rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 qdls-0.1.4/src/qdls/draw/experiment.py
--rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 qdls-0.1.4/src/qdls/draw/stats.py
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 qdls-0.1.4/src/qdls/gql/__init__.py
--rw-r--r--   0        0        0     7433 2020-02-02 00:00:00.000000 qdls-0.1.4/src/qdls/gql/process_utils.py
--rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 qdls-0.1.4/src/qdls/gql/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qdls-0.1.4/src/qdls/gql/cypher/__init__.py
--rw-r--r--   0        0        0    61918 2020-02-02 00:00:00.000000 qdls-0.1.4/src/qdls/gql/cypher/grammar/Cypher.interp
--rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 qdls-0.1.4/src/qdls/gql/cypher/grammar/Cypher.tokens
--rw-r--r--   0        0        0    61096 2020-02-02 00:00:00.000000 qdls-0.1.4/src/qdls/gql/cypher/grammar/CypherLexer.interp
--rw-r--r--   0        0        0    72699 2020-02-02 00:00:00.000000 qdls-0.1.4/src/qdls/gql/cypher/grammar/CypherLexer.py
--rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 qdls-0.1.4/src/qdls/gql/cypher/grammar/CypherLexer.tokens
--rw-r--r--   0        0        0    33891 2020-02-02 00:00:00.000000 qdls-0.1.4/src/qdls/gql/cypher/grammar/CypherListener.py
--rw-r--r--   0        0        0   413383 2020-02-02 00:00:00.000000 qdls-0.1.4/src/qdls/gql/cypher/grammar/CypherParser.py
--rw-r--r--   0        0        0    19984 2020-02-02 00:00:00.000000 qdls-0.1.4/src/qdls/gql/cypher/grammar/CypherVisitor.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qdls-0.1.4/src/qdls/gql/cypher/grammar/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qdls-0.1.4/src/qdls/gql/cypher/utils/__init__.py
--rw-r--r--   0        0        0     4611 2020-02-02 00:00:00.000000 qdls-0.1.4/src/qdls/gql/cypher/utils/execute.py
--rw-r--r--   0        0        0     8873 2020-02-02 00:00:00.000000 qdls-0.1.4/src/qdls/gql/cypher/utils/kqa_eval.py
--rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 qdls-0.1.4/src/qdls/gql/cypher/utils/parse.py
--rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 qdls-0.1.4/src/qdls/gql/cypher/utils/syntax.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qdls-0.1.4/src/qdls/gql/sparql/__init__.py
--rw-r--r--   0        0        0    57079 2020-02-02 00:00:00.000000 qdls-0.1.4/src/qdls/gql/sparql/grammar/Sparql.interp
--rw-r--r--   0        0        0     2016 2020-02-02 00:00:00.000000 qdls-0.1.4/src/qdls/gql/sparql/grammar/Sparql.tokens
--rw-r--r--   0        0        0    52018 2020-02-02 00:00:00.000000 qdls-0.1.4/src/qdls/gql/sparql/grammar/SparqlLexer.interp
--rw-r--r--   0        0        0    62363 2020-02-02 00:00:00.000000 qdls-0.1.4/src/qdls/gql/sparql/grammar/SparqlLexer.py
--rw-r--r--   0        0        0     2016 2020-02-02 00:00:00.000000 qdls-0.1.4/src/qdls/gql/sparql/grammar/SparqlLexer.tokens
--rw-r--r--   0        0        0    44193 2020-02-02 00:00:00.000000 qdls-0.1.4/src/qdls/gql/sparql/grammar/SparqlListener.py
--rw-r--r--   0        0        0   497844 2020-02-02 00:00:00.000000 qdls-0.1.4/src/qdls/gql/sparql/grammar/SparqlParser.py
--rw-r--r--   0        0        0    26235 2020-02-02 00:00:00.000000 qdls-0.1.4/src/qdls/gql/sparql/grammar/SparqlVisitor.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qdls-0.1.4/src/qdls/gql/sparql/grammar/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qdls-0.1.4/src/qdls/gql/sparql/utils/__init__.py
--rw-r--r--   0        0        0    23591 2020-02-02 00:00:00.000000 qdls-0.1.4/src/qdls/gql/sparql/utils/kqa_eval.py
--rw-r--r--   0        0        0     2114 2020-02-02 00:00:00.000000 qdls-0.1.4/src/qdls/gql/sparql/utils/parse.py
--rw-r--r--   0        0        0     1449 2020-02-02 00:00:00.000000 qdls-0.1.4/src/qdls/gql/sparql/utils/syntax.py
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 qdls-0.1.4/src/qdls/kgqa_eval/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qdls-0.1.4/src/qdls/kgqa_eval/__init__.py
--rw-r--r--   0        0        0     4507 2020-02-02 00:00:00.000000 qdls-0.1.4/src/qdls/kgqa_eval/example.py
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 qdls-0.1.4/src/qdls/kgqa_eval/evaluator/__init__.py
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 qdls-0.1.4/src/qdls/kgqa_eval/evaluator/base.py
--rw-r--r--   0        0        0     6770 2020-02-02 00:00:00.000000 qdls-0.1.4/src/qdls/kgqa_eval/evaluator/kqa.py
--rw-r--r--   0        0        0     6000 2020-02-02 00:00:00.000000 qdls-0.1.4/src/qdls/kgqa_eval/evaluator/metric_fns.py
--rw-r--r--   0        0        0    30314 2020-02-02 00:00:00.000000 qdls-0.1.4/src/qdls/kgqa_eval/evaluator/sparql_utils.py
--rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 qdls-0.1.4/src/qdls/kgqa_eval/evaluator/utils.py
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 qdls-0.1.4/src/qdls/kgqa_eval/exact_set/__init__.py
--rw-r--r--   0        0        0     6256 2020-02-02 00:00:00.000000 qdls-0.1.4/src/qdls/kgqa_eval/exact_set/evaluation_em.py
--rw-r--r--   0        0        0     2092 2020-02-02 00:00:00.000000 qdls-0.1.4/src/qdls/kgqa_eval/exact_set/match_evaluate.py
--rw-r--r--   0        0        0     5320 2020-02-02 00:00:00.000000 qdls-0.1.4/src/qdls/kgqa_eval/exact_set/return_evaluate.py
--rw-r--r--   0        0        0     5408 2020-02-02 00:00:00.000000 qdls-0.1.4/src/qdls/kgqa_eval/exact_set/utils.py
--rw-r--r--   0        0        0     2391 2020-02-02 00:00:00.000000 qdls-0.1.4/src/qdls/kgqa_eval/exact_set/where_evaluate.py
--rw-r--r--   0        0        0     2437 2020-02-02 00:00:00.000000 qdls-0.1.4/src/qdls/kgqa_eval/exact_set/with_evaluate.py
--rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 qdls-0.1.4/src/qdls/llm_infer/configs.py
--rw-r--r--   0        0        0     4901 2020-02-02 00:00:00.000000 qdls-0.1.4/src/qdls/llm_infer/runner.py
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 qdls-0.1.4/src/qdls/llm_infer/retrievers/__init__.py
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 qdls-0.1.4/src/qdls/llm_infer/retrievers/base_retriever.py
--rw-r--r--   0        0        0     4491 2020-02-02 00:00:00.000000 qdls-0.1.4/src/qdls/llm_infer/retrievers/bm25_retriever.py
--rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 qdls-0.1.4/src/qdls/llm_infer/retrievers/vector_retriever.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qdls-0.1.4/src/qdls/reg/__init__.py
--rw-r--r--   0        0        0     4364 2020-02-02 00:00:00.000000 qdls-0.1.4/src/qdls/reg/register.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 qdls-0.1.4/src/qdls/reg/collators/__init__.py
--rw-r--r--   0        0        0     2651 2020-02-02 00:00:00.000000 qdls-0.1.4/src/qdls/reg/collators/common_collators.py
--rw-r--r--   0        0        0     4704 2020-02-02 00:00:00.000000 qdls-0.1.4/src/qdls/reg/datamodules/base_dm.py
--rw-r--r--   0        0        0     3088 2020-02-02 00:00:00.000000 qdls-0.1.4/src/qdls/reg/datamodules/dataset_builder.py
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 qdls-0.1.4/src/qdls/reg/models/__init__.py
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 qdls-0.1.4/src/qdls/reg/models/test_model.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qdls-0.1.4/src/qdls/reg/process_functions/__init__.py
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 qdls-0.1.4/src/qdls/reg/process_functions/common.py
--rw-r--r--   0        0        0     7909 2020-02-02 00:00:00.000000 qdls-0.1.4/src/qdls/reg/process_functions/kqa.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 qdls-0.1.4/src/qdls/tools/__init__.py
--rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 qdls-0.1.4/src/qdls/tools/num_params.py
--rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 qdls-0.1.4/.gitignore
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 qdls-0.1.4/LICENSE
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 qdls-0.1.4/README.md
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 qdls-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 qdls-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 qdls-0.1.5/.github/workflows/publish.yml
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 qdls-0.1.5/src/qdls/__init__.py
+-rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 qdls-0.1.5/src/qdls/cli.py
+-rw-r--r--   0        0        0    11340 2020-02-02 00:00:00.000000 qdls-0.1.5/src/qdls/data.py
+-rw-r--r--   0        0        0     3796 2020-02-02 00:00:00.000000 qdls-0.1.5/src/qdls/losses.py
+-rw-r--r--   0        0        0     2815 2020-02-02 00:00:00.000000 qdls-0.1.5/src/qdls/metrics.py
+-rw-r--r--   0        0        0     4282 2020-02-02 00:00:00.000000 qdls-0.1.5/src/qdls/tensor_ops.py
+-rw-r--r--   0        0        0     2338 2020-02-02 00:00:00.000000 qdls-0.1.5/src/qdls/utils.py
+-rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 qdls-0.1.5/src/qdls/code_template/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qdls-0.1.5/src/qdls/code_template/notebooks/statis.ipynb
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 qdls-0.1.5/src/qdls/code_template/preliminary/example.py
+-rw-r--r--   0        0        0     4095 2020-02-02 00:00:00.000000 qdls-0.1.5/src/qdls/code_template/src/frame.py
+-rw-r--r--   0        0        0     1374 2020-02-02 00:00:00.000000 qdls-0.1.5/src/qdls/code_template/src/main.py
+-rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 qdls-0.1.5/src/qdls/code_template/src/pl_callbacks.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qdls-0.1.5/src/qdls/code_template/src/utils.py
+-rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 qdls-0.1.5/src/qdls/code_template/src/configs/example.yaml
+-rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 qdls-0.1.5/src/qdls/code_template/src/data_utils/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qdls-0.1.5/src/qdls/code_template/src/data_utils/common.py
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 qdls-0.1.5/src/qdls/code_template/src/models/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qdls-0.1.5/src/qdls/deprecate/__init__.py
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 qdls-0.1.5/src/qdls/deprecate/data.py
+-rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 qdls-0.1.5/src/qdls/deprecate/loggers.py
+-rw-r--r--   0        0        0    13330 2020-02-02 00:00:00.000000 qdls-0.1.5/src/qdls/deprecate/object.py
+-rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 qdls-0.1.5/src/qdls/deprecate/optim.py
+-rw-r--r--   0        0        0    13611 2020-02-02 00:00:00.000000 qdls-0.1.5/src/qdls/deprecate/pretrains.py
+-rw-r--r--   0        0        0     3598 2020-02-02 00:00:00.000000 qdls-0.1.5/src/qdls/deprecate/test.py
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 qdls-0.1.5/src/qdls/deprecate/train.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qdls-0.1.5/src/qdls/draw/__init__.py
+-rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 qdls-0.1.5/src/qdls/draw/experiment.py
+-rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 qdls-0.1.5/src/qdls/draw/stats.py
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 qdls-0.1.5/src/qdls/gql/__init__.py
+-rw-r--r--   0        0        0     7433 2020-02-02 00:00:00.000000 qdls-0.1.5/src/qdls/gql/process_utils.py
+-rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 qdls-0.1.5/src/qdls/gql/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qdls-0.1.5/src/qdls/gql/cypher/__init__.py
+-rw-r--r--   0        0        0    61918 2020-02-02 00:00:00.000000 qdls-0.1.5/src/qdls/gql/cypher/grammar/Cypher.interp
+-rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 qdls-0.1.5/src/qdls/gql/cypher/grammar/Cypher.tokens
+-rw-r--r--   0        0        0    61096 2020-02-02 00:00:00.000000 qdls-0.1.5/src/qdls/gql/cypher/grammar/CypherLexer.interp
+-rw-r--r--   0        0        0    72699 2020-02-02 00:00:00.000000 qdls-0.1.5/src/qdls/gql/cypher/grammar/CypherLexer.py
+-rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 qdls-0.1.5/src/qdls/gql/cypher/grammar/CypherLexer.tokens
+-rw-r--r--   0        0        0    33891 2020-02-02 00:00:00.000000 qdls-0.1.5/src/qdls/gql/cypher/grammar/CypherListener.py
+-rw-r--r--   0        0        0   413383 2020-02-02 00:00:00.000000 qdls-0.1.5/src/qdls/gql/cypher/grammar/CypherParser.py
+-rw-r--r--   0        0        0    19984 2020-02-02 00:00:00.000000 qdls-0.1.5/src/qdls/gql/cypher/grammar/CypherVisitor.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qdls-0.1.5/src/qdls/gql/cypher/grammar/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qdls-0.1.5/src/qdls/gql/cypher/utils/__init__.py
+-rw-r--r--   0        0        0     4611 2020-02-02 00:00:00.000000 qdls-0.1.5/src/qdls/gql/cypher/utils/execute.py
+-rw-r--r--   0        0        0     8873 2020-02-02 00:00:00.000000 qdls-0.1.5/src/qdls/gql/cypher/utils/kqa_eval.py
+-rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 qdls-0.1.5/src/qdls/gql/cypher/utils/parse.py
+-rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 qdls-0.1.5/src/qdls/gql/cypher/utils/syntax.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qdls-0.1.5/src/qdls/gql/sparql/__init__.py
+-rw-r--r--   0        0        0    57079 2020-02-02 00:00:00.000000 qdls-0.1.5/src/qdls/gql/sparql/grammar/Sparql.interp
+-rw-r--r--   0        0        0     2016 2020-02-02 00:00:00.000000 qdls-0.1.5/src/qdls/gql/sparql/grammar/Sparql.tokens
+-rw-r--r--   0        0        0    52018 2020-02-02 00:00:00.000000 qdls-0.1.5/src/qdls/gql/sparql/grammar/SparqlLexer.interp
+-rw-r--r--   0        0        0    62363 2020-02-02 00:00:00.000000 qdls-0.1.5/src/qdls/gql/sparql/grammar/SparqlLexer.py
+-rw-r--r--   0        0        0     2016 2020-02-02 00:00:00.000000 qdls-0.1.5/src/qdls/gql/sparql/grammar/SparqlLexer.tokens
+-rw-r--r--   0        0        0    44193 2020-02-02 00:00:00.000000 qdls-0.1.5/src/qdls/gql/sparql/grammar/SparqlListener.py
+-rw-r--r--   0        0        0   497844 2020-02-02 00:00:00.000000 qdls-0.1.5/src/qdls/gql/sparql/grammar/SparqlParser.py
+-rw-r--r--   0        0        0    26235 2020-02-02 00:00:00.000000 qdls-0.1.5/src/qdls/gql/sparql/grammar/SparqlVisitor.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qdls-0.1.5/src/qdls/gql/sparql/grammar/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qdls-0.1.5/src/qdls/gql/sparql/utils/__init__.py
+-rw-r--r--   0        0        0    23591 2020-02-02 00:00:00.000000 qdls-0.1.5/src/qdls/gql/sparql/utils/kqa_eval.py
+-rw-r--r--   0        0        0     2114 2020-02-02 00:00:00.000000 qdls-0.1.5/src/qdls/gql/sparql/utils/parse.py
+-rw-r--r--   0        0        0     1449 2020-02-02 00:00:00.000000 qdls-0.1.5/src/qdls/gql/sparql/utils/syntax.py
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 qdls-0.1.5/src/qdls/kgqa_eval/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qdls-0.1.5/src/qdls/kgqa_eval/__init__.py
+-rw-r--r--   0        0        0     4507 2020-02-02 00:00:00.000000 qdls-0.1.5/src/qdls/kgqa_eval/example.py
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 qdls-0.1.5/src/qdls/kgqa_eval/evaluator/__init__.py
+-rw-r--r--   0        0        0     3916 2020-02-02 00:00:00.000000 qdls-0.1.5/src/qdls/kgqa_eval/evaluator/base.py
+-rw-r--r--   0        0        0     6770 2020-02-02 00:00:00.000000 qdls-0.1.5/src/qdls/kgqa_eval/evaluator/kqa.py
+-rw-r--r--   0        0        0     6048 2020-02-02 00:00:00.000000 qdls-0.1.5/src/qdls/kgqa_eval/evaluator/metric_fns.py
+-rw-r--r--   0        0        0    30314 2020-02-02 00:00:00.000000 qdls-0.1.5/src/qdls/kgqa_eval/evaluator/sparql_utils.py
+-rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 qdls-0.1.5/src/qdls/kgqa_eval/evaluator/utils.py
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 qdls-0.1.5/src/qdls/kgqa_eval/exact_set/__init__.py
+-rw-r--r--   0        0        0     6256 2020-02-02 00:00:00.000000 qdls-0.1.5/src/qdls/kgqa_eval/exact_set/evaluation_em.py
+-rw-r--r--   0        0        0     2092 2020-02-02 00:00:00.000000 qdls-0.1.5/src/qdls/kgqa_eval/exact_set/match_evaluate.py
+-rw-r--r--   0        0        0     5320 2020-02-02 00:00:00.000000 qdls-0.1.5/src/qdls/kgqa_eval/exact_set/return_evaluate.py
+-rw-r--r--   0        0        0     5408 2020-02-02 00:00:00.000000 qdls-0.1.5/src/qdls/kgqa_eval/exact_set/utils.py
+-rw-r--r--   0        0        0     2391 2020-02-02 00:00:00.000000 qdls-0.1.5/src/qdls/kgqa_eval/exact_set/where_evaluate.py
+-rw-r--r--   0        0        0     2437 2020-02-02 00:00:00.000000 qdls-0.1.5/src/qdls/kgqa_eval/exact_set/with_evaluate.py
+-rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 qdls-0.1.5/src/qdls/llm_infer/configs.py
+-rw-r--r--   0        0        0     4901 2020-02-02 00:00:00.000000 qdls-0.1.5/src/qdls/llm_infer/runner.py
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 qdls-0.1.5/src/qdls/llm_infer/retrievers/__init__.py
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 qdls-0.1.5/src/qdls/llm_infer/retrievers/base_retriever.py
+-rw-r--r--   0        0        0     4491 2020-02-02 00:00:00.000000 qdls-0.1.5/src/qdls/llm_infer/retrievers/bm25_retriever.py
+-rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 qdls-0.1.5/src/qdls/llm_infer/retrievers/vector_retriever.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qdls-0.1.5/src/qdls/reg/__init__.py
+-rw-r--r--   0        0        0     4364 2020-02-02 00:00:00.000000 qdls-0.1.5/src/qdls/reg/register.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 qdls-0.1.5/src/qdls/reg/collators/__init__.py
+-rw-r--r--   0        0        0     2651 2020-02-02 00:00:00.000000 qdls-0.1.5/src/qdls/reg/collators/common_collators.py
+-rw-r--r--   0        0        0     4704 2020-02-02 00:00:00.000000 qdls-0.1.5/src/qdls/reg/datamodules/base_dm.py
+-rw-r--r--   0        0        0     3088 2020-02-02 00:00:00.000000 qdls-0.1.5/src/qdls/reg/datamodules/dataset_builder.py
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 qdls-0.1.5/src/qdls/reg/models/__init__.py
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 qdls-0.1.5/src/qdls/reg/models/test_model.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qdls-0.1.5/src/qdls/reg/process_functions/__init__.py
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 qdls-0.1.5/src/qdls/reg/process_functions/common.py
+-rw-r--r--   0        0        0     7909 2020-02-02 00:00:00.000000 qdls-0.1.5/src/qdls/reg/process_functions/kqa.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 qdls-0.1.5/src/qdls/tools/__init__.py
+-rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 qdls-0.1.5/src/qdls/tools/num_params.py
+-rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 qdls-0.1.5/.gitignore
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 qdls-0.1.5/LICENSE
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 qdls-0.1.5/README.md
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 qdls-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 qdls-0.1.5/PKG-INFO
```

### Comparing `qdls-0.1.4/.github/workflows/publish.yml` & `qdls-0.1.5/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `qdls-0.1.4/src/qdls/cli.py` & `qdls-0.1.5/src/qdls/cli.py`

 * *Files identical despite different names*

### Comparing `qdls-0.1.4/src/qdls/data.py` & `qdls-0.1.5/src/qdls/data.py`

 * *Files identical despite different names*

### Comparing `qdls-0.1.4/src/qdls/losses.py` & `qdls-0.1.5/src/qdls/losses.py`

 * *Files identical despite different names*

### Comparing `qdls-0.1.4/src/qdls/metrics.py` & `qdls-0.1.5/src/qdls/metrics.py`

 * *Files identical despite different names*

### Comparing `qdls-0.1.4/src/qdls/tensor_ops.py` & `qdls-0.1.5/src/qdls/tensor_ops.py`

 * *Files identical despite different names*

### Comparing `qdls-0.1.4/src/qdls/utils.py` & `qdls-0.1.5/src/qdls/utils.py`

 * *Files identical despite different names*

### Comparing `qdls-0.1.4/src/qdls/code_template/README.md` & `qdls-0.1.5/src/qdls/code_template/README.md`

 * *Files identical despite different names*

### Comparing `qdls-0.1.4/src/qdls/code_template/src/frame.py` & `qdls-0.1.5/src/qdls/code_template/src/frame.py`

 * *Files identical despite different names*

### Comparing `qdls-0.1.4/src/qdls/code_template/src/main.py` & `qdls-0.1.5/src/qdls/code_template/src/main.py`

 * *Files identical despite different names*

### Comparing `qdls-0.1.4/src/qdls/code_template/src/pl_callbacks.py` & `qdls-0.1.5/src/qdls/code_template/src/pl_callbacks.py`

 * *Files identical despite different names*

### Comparing `qdls-0.1.4/src/qdls/code_template/src/configs/example.yaml` & `qdls-0.1.5/src/qdls/code_template/src/configs/example.yaml`

 * *Files identical despite different names*

### Comparing `qdls-0.1.4/src/qdls/code_template/src/data_utils/__init__.py` & `qdls-0.1.5/src/qdls/code_template/src/data_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `qdls-0.1.4/src/qdls/deprecate/data.py` & `qdls-0.1.5/src/qdls/deprecate/data.py`

 * *Files identical despite different names*

### Comparing `qdls-0.1.4/src/qdls/deprecate/loggers.py` & `qdls-0.1.5/src/qdls/deprecate/loggers.py`

 * *Files identical despite different names*

### Comparing `qdls-0.1.4/src/qdls/deprecate/object.py` & `qdls-0.1.5/src/qdls/deprecate/object.py`

 * *Files identical despite different names*

### Comparing `qdls-0.1.4/src/qdls/deprecate/optim.py` & `qdls-0.1.5/src/qdls/deprecate/optim.py`

 * *Files identical despite different names*

### Comparing `qdls-0.1.4/src/qdls/deprecate/pretrains.py` & `qdls-0.1.5/src/qdls/deprecate/pretrains.py`

 * *Files identical despite different names*

### Comparing `qdls-0.1.4/src/qdls/deprecate/test.py` & `qdls-0.1.5/src/qdls/deprecate/test.py`

 * *Files identical despite different names*

### Comparing `qdls-0.1.4/src/qdls/draw/experiment.py` & `qdls-0.1.5/src/qdls/draw/experiment.py`

 * *Files identical despite different names*

### Comparing `qdls-0.1.4/src/qdls/draw/stats.py` & `qdls-0.1.5/src/qdls/draw/stats.py`

 * *Files identical despite different names*

### Comparing `qdls-0.1.4/src/qdls/gql/process_utils.py` & `qdls-0.1.5/src/qdls/gql/process_utils.py`

 * *Files identical despite different names*

### Comparing `qdls-0.1.4/src/qdls/gql/utils.py` & `qdls-0.1.5/src/qdls/gql/utils.py`

 * *Files identical despite different names*

### Comparing `qdls-0.1.4/src/qdls/gql/cypher/grammar/Cypher.interp` & `qdls-0.1.5/src/qdls/gql/cypher/grammar/Cypher.interp`

 * *Files identical despite different names*

### Comparing `qdls-0.1.4/src/qdls/gql/cypher/grammar/Cypher.tokens` & `qdls-0.1.5/src/qdls/gql/cypher/grammar/Cypher.tokens`

 * *Files identical despite different names*

### Comparing `qdls-0.1.4/src/qdls/gql/cypher/grammar/CypherLexer.interp` & `qdls-0.1.5/src/qdls/gql/cypher/grammar/CypherLexer.interp`

 * *Files identical despite different names*

### Comparing `qdls-0.1.4/src/qdls/gql/cypher/grammar/CypherLexer.py` & `qdls-0.1.5/src/qdls/gql/cypher/grammar/CypherLexer.py`

 * *Files identical despite different names*

### Comparing `qdls-0.1.4/src/qdls/gql/cypher/grammar/CypherLexer.tokens` & `qdls-0.1.5/src/qdls/gql/cypher/grammar/CypherLexer.tokens`

 * *Files identical despite different names*

### Comparing `qdls-0.1.4/src/qdls/gql/cypher/grammar/CypherListener.py` & `qdls-0.1.5/src/qdls/gql/cypher/grammar/CypherListener.py`

 * *Files identical despite different names*

### Comparing `qdls-0.1.4/src/qdls/gql/cypher/grammar/CypherParser.py` & `qdls-0.1.5/src/qdls/gql/cypher/grammar/CypherParser.py`

 * *Files identical despite different names*

### Comparing `qdls-0.1.4/src/qdls/gql/cypher/grammar/CypherVisitor.py` & `qdls-0.1.5/src/qdls/gql/cypher/grammar/CypherVisitor.py`

 * *Files identical despite different names*

### Comparing `qdls-0.1.4/src/qdls/gql/cypher/utils/execute.py` & `qdls-0.1.5/src/qdls/gql/cypher/utils/execute.py`

 * *Files identical despite different names*

### Comparing `qdls-0.1.4/src/qdls/gql/cypher/utils/kqa_eval.py` & `qdls-0.1.5/src/qdls/gql/cypher/utils/kqa_eval.py`

 * *Files identical despite different names*

### Comparing `qdls-0.1.4/src/qdls/gql/cypher/utils/parse.py` & `qdls-0.1.5/src/qdls/gql/cypher/utils/parse.py`

 * *Files identical despite different names*

### Comparing `qdls-0.1.4/src/qdls/gql/cypher/utils/syntax.py` & `qdls-0.1.5/src/qdls/gql/cypher/utils/syntax.py`

 * *Files identical despite different names*

### Comparing `qdls-0.1.4/src/qdls/gql/sparql/grammar/Sparql.interp` & `qdls-0.1.5/src/qdls/gql/sparql/grammar/Sparql.interp`

 * *Files identical despite different names*

### Comparing `qdls-0.1.4/src/qdls/gql/sparql/grammar/Sparql.tokens` & `qdls-0.1.5/src/qdls/gql/sparql/grammar/Sparql.tokens`

 * *Files identical despite different names*

### Comparing `qdls-0.1.4/src/qdls/gql/sparql/grammar/SparqlLexer.interp` & `qdls-0.1.5/src/qdls/gql/sparql/grammar/SparqlLexer.interp`

 * *Files identical despite different names*

### Comparing `qdls-0.1.4/src/qdls/gql/sparql/grammar/SparqlLexer.py` & `qdls-0.1.5/src/qdls/gql/sparql/grammar/SparqlLexer.py`

 * *Files identical despite different names*

### Comparing `qdls-0.1.4/src/qdls/gql/sparql/grammar/SparqlLexer.tokens` & `qdls-0.1.5/src/qdls/gql/sparql/grammar/SparqlLexer.tokens`

 * *Files identical despite different names*

### Comparing `qdls-0.1.4/src/qdls/gql/sparql/grammar/SparqlListener.py` & `qdls-0.1.5/src/qdls/gql/sparql/grammar/SparqlListener.py`

 * *Files identical despite different names*

### Comparing `qdls-0.1.4/src/qdls/gql/sparql/grammar/SparqlParser.py` & `qdls-0.1.5/src/qdls/gql/sparql/grammar/SparqlParser.py`

 * *Files identical despite different names*

### Comparing `qdls-0.1.4/src/qdls/gql/sparql/grammar/SparqlVisitor.py` & `qdls-0.1.5/src/qdls/gql/sparql/grammar/SparqlVisitor.py`

 * *Files identical despite different names*

### Comparing `qdls-0.1.4/src/qdls/gql/sparql/utils/kqa_eval.py` & `qdls-0.1.5/src/qdls/gql/sparql/utils/kqa_eval.py`

 * *Files identical despite different names*

### Comparing `qdls-0.1.4/src/qdls/gql/sparql/utils/parse.py` & `qdls-0.1.5/src/qdls/gql/sparql/utils/parse.py`

 * *Files identical despite different names*

### Comparing `qdls-0.1.4/src/qdls/gql/sparql/utils/syntax.py` & `qdls-0.1.5/src/qdls/gql/sparql/utils/syntax.py`

 * *Files identical despite different names*

### Comparing `qdls-0.1.4/src/qdls/kgqa_eval/example.py` & `qdls-0.1.5/src/qdls/kgqa_eval/example.py`

 * *Files identical despite different names*

### Comparing `qdls-0.1.4/src/qdls/kgqa_eval/evaluator/kqa.py` & `qdls-0.1.5/src/qdls/kgqa_eval/evaluator/kqa.py`

 * *Files identical despite different names*

### Comparing `qdls-0.1.4/src/qdls/kgqa_eval/evaluator/metric_fns.py` & `qdls-0.1.5/src/qdls/kgqa_eval/evaluator/metric_fns.py`

 * *Files 1% similar despite different names*

```diff
@@ -144,17 +144,18 @@
             print(e)
             is_correct, info, results = False, "Timeout", '[]'
         sample['is_correct'] = is_correct
         sample['exec_info'] = info
         sample['exec_results'] = results
 
     # 处理其他 metric
-    for k, fn in metric_fns:
+    for k in metrics:
         if k in sample:
             continue
+        fn = metric_fns.get(k) # 获取注册的函数
         res = fn(sample, neo4j_config=neo4j_config, ref_key=ref_key)
         sample[k] = res 
 
     # import pdb;pdb.set_trace();
     return sample
 
 def nltk_bleu():
```

### Comparing `qdls-0.1.4/src/qdls/kgqa_eval/evaluator/sparql_utils.py` & `qdls-0.1.5/src/qdls/kgqa_eval/evaluator/sparql_utils.py`

 * *Files identical despite different names*

### Comparing `qdls-0.1.4/src/qdls/kgqa_eval/evaluator/utils.py` & `qdls-0.1.5/src/qdls/kgqa_eval/evaluator/utils.py`

 * *Files identical despite different names*

### Comparing `qdls-0.1.4/src/qdls/kgqa_eval/exact_set/evaluation_em.py` & `qdls-0.1.5/src/qdls/kgqa_eval/exact_set/evaluation_em.py`

 * *Files identical despite different names*

### Comparing `qdls-0.1.4/src/qdls/kgqa_eval/exact_set/match_evaluate.py` & `qdls-0.1.5/src/qdls/kgqa_eval/exact_set/match_evaluate.py`

 * *Files identical despite different names*

### Comparing `qdls-0.1.4/src/qdls/kgqa_eval/exact_set/return_evaluate.py` & `qdls-0.1.5/src/qdls/kgqa_eval/exact_set/return_evaluate.py`

 * *Files identical despite different names*

### Comparing `qdls-0.1.4/src/qdls/kgqa_eval/exact_set/utils.py` & `qdls-0.1.5/src/qdls/kgqa_eval/exact_set/utils.py`

 * *Files identical despite different names*

### Comparing `qdls-0.1.4/src/qdls/kgqa_eval/exact_set/where_evaluate.py` & `qdls-0.1.5/src/qdls/kgqa_eval/exact_set/where_evaluate.py`

 * *Files identical despite different names*

### Comparing `qdls-0.1.4/src/qdls/kgqa_eval/exact_set/with_evaluate.py` & `qdls-0.1.5/src/qdls/kgqa_eval/exact_set/with_evaluate.py`

 * *Files identical despite different names*

### Comparing `qdls-0.1.4/src/qdls/llm_infer/configs.py` & `qdls-0.1.5/src/qdls/llm_infer/configs.py`

 * *Files identical despite different names*

### Comparing `qdls-0.1.4/src/qdls/llm_infer/runner.py` & `qdls-0.1.5/src/qdls/llm_infer/runner.py`

 * *Files identical despite different names*

### Comparing `qdls-0.1.4/src/qdls/llm_infer/retrievers/bm25_retriever.py` & `qdls-0.1.5/src/qdls/llm_infer/retrievers/bm25_retriever.py`

 * *Files identical despite different names*

### Comparing `qdls-0.1.4/src/qdls/llm_infer/retrievers/vector_retriever.py` & `qdls-0.1.5/src/qdls/llm_infer/retrievers/vector_retriever.py`

 * *Files identical despite different names*

### Comparing `qdls-0.1.4/src/qdls/reg/register.py` & `qdls-0.1.5/src/qdls/reg/register.py`

 * *Files identical despite different names*

### Comparing `qdls-0.1.4/src/qdls/reg/collators/common_collators.py` & `qdls-0.1.5/src/qdls/reg/collators/common_collators.py`

 * *Files identical despite different names*

### Comparing `qdls-0.1.4/src/qdls/reg/datamodules/base_dm.py` & `qdls-0.1.5/src/qdls/reg/datamodules/base_dm.py`

 * *Files identical despite different names*

### Comparing `qdls-0.1.4/src/qdls/reg/datamodules/dataset_builder.py` & `qdls-0.1.5/src/qdls/reg/datamodules/dataset_builder.py`

 * *Files identical despite different names*

### Comparing `qdls-0.1.4/src/qdls/reg/process_functions/kqa.py` & `qdls-0.1.5/src/qdls/reg/process_functions/kqa.py`

 * *Files identical despite different names*

### Comparing `qdls-0.1.4/src/qdls/tools/num_params.py` & `qdls-0.1.5/src/qdls/tools/num_params.py`

 * *Files identical despite different names*

### Comparing `qdls-0.1.4/.gitignore` & `qdls-0.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `qdls-0.1.4/LICENSE` & `qdls-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `qdls-0.1.4/pyproject.toml` & `qdls-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 
 [project]
 name = "qdls"
-version = "0.1.4"
+version = "0.1.5"
 authors = [
   { name="Qing25", email="aqsz2526@outlook.com" },
 ]
 description = "Q-Deep Learning Snippets, my working code snippets"
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = [
```

### Comparing `qdls-0.1.4/PKG-INFO` & `qdls-0.1.5/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: qdls
-Version: 0.1.4
+Version: 0.1.5
 Summary: Q-Deep Learning Snippets, my working code snippets
 Project-URL: Homepage, https://github.com/Qing25/qdls
 Author-email: Qing25 <aqsz2526@outlook.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

