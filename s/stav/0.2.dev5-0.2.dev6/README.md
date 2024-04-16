# Comparing `tmp/stav-0.2.dev5.tar.gz` & `tmp/stav-0.2.dev6.tar.gz`

## Comparing `stav-0.2.dev5.tar` & `stav-0.2.dev6.tar`

### file list

```diff
@@ -1,58 +1,183 @@
--rw-r--r--   0        0        0     7831 2020-02-02 00:00:00.000000 stav-0.2.dev5/ai-stakeholders.drawio
--rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 stav-0.2.dev5/catalog-v001.xml
--rw-r--r--   0        0        0     8905 2020-02-02 00:00:00.000000 stav-0.2.dev5/stav-eu-aia.ttl
--rw-r--r--   0        0        0     6410 2020-02-02 00:00:00.000000 stav-0.2.dev5/stav-th-aisbd.ttl
--rw-r--r--   0        0        0    11686 2020-02-02 00:00:00.000000 stav-0.2.dev5/stav-us-aaa.ttl
--rw-r--r--   0        0        0    23684 2020-02-02 00:00:00.000000 stav-0.2.dev5/stav.ttl
--rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 stav-0.2.dev5/docs/.htaccess
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 stav-0.2.dev5/docs/406.html
--rw-r--r--   0        0        0    63347 2020-02-02 00:00:00.000000 stav-0.2.dev5/docs/index.html
--rw-r--r--   0        0        0    31071 2020-02-02 00:00:00.000000 stav-0.2.dev5/docs/ontology.jsonld
--rw-r--r--   0        0        0    37077 2020-02-02 00:00:00.000000 stav-0.2.dev5/docs/ontology.nt
--rw-r--r--   0        0        0    28158 2020-02-02 00:00:00.000000 stav-0.2.dev5/docs/ontology.owl
--rw-r--r--   0        0        0    26430 2020-02-02 00:00:00.000000 stav-0.2.dev5/docs/ontology.ttl
--rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 stav-0.2.dev5/docs/readme.md
--rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 stav-0.2.dev5/docs/resources/extra.css
--rw-r--r--   0        0        0    91556 2020-02-02 00:00:00.000000 stav-0.2.dev5/docs/resources/jquery.js
--rw-r--r--   0        0        0    47959 2020-02-02 00:00:00.000000 stav-0.2.dev5/docs/resources/marked.min.js
--rw-r--r--   0        0        0     4389 2020-02-02 00:00:00.000000 stav-0.2.dev5/docs/resources/owl.css
--rw-r--r--   0        0        0     2491 2020-02-02 00:00:00.000000 stav-0.2.dev5/docs/resources/primer.css
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 stav-0.2.dev5/docs/resources/rdf.icon
--rw-r--r--   0        0        0     2459 2020-02-02 00:00:00.000000 stav-0.2.dev5/docs/resources/rec.css
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 stav-0.2.dev5/docs/webvowl/favicon.ico
--rw-r--r--   0        0        0    35533 2020-02-02 00:00:00.000000 stav-0.2.dev5/docs/webvowl/index.html
--rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 stav-0.2.dev5/docs/webvowl/license.txt
--rw-r--r--   0        0        0    42681 2020-02-02 00:00:00.000000 stav-0.2.dev5/docs/webvowl/css/webvowl.app.css
--rw-r--r--   0        0        0     5341 2020-02-02 00:00:00.000000 stav-0.2.dev5/docs/webvowl/css/webvowl.css
--rw-r--r--   0        0        0    74704 2020-02-02 00:00:00.000000 stav-0.2.dev5/docs/webvowl/data/foaf.json
--rw-r--r--   0        0        0    39197 2020-02-02 00:00:00.000000 stav-0.2.dev5/docs/webvowl/data/ontology.json
--rw-r--r--   0        0        0     2705 2020-02-02 00:00:00.000000 stav-0.2.dev5/docs/webvowl/data/template.json
--rw-r--r--   0        0        0   151725 2020-02-02 00:00:00.000000 stav-0.2.dev5/docs/webvowl/js/d3.min.js
--rw-r--r--   0        0        0   350028 2020-02-02 00:00:00.000000 stav-0.2.dev5/docs/webvowl/js/webvowl.app.js
--rw-r--r--   0        0        0   751167 2020-02-02 00:00:00.000000 stav-0.2.dev5/docs/webvowl/js/webvowl.js
--rw-r--r--   0        0        0     1482 2020-02-02 00:00:00.000000 stav-0.2.dev5/notebooks/mlflowstav.ipynb
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 stav-0.2.dev5/notebooks/use_instruction.txt
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 stav-0.2.dev5/notebooks/mlruns/0/meta.yaml
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 stav-0.2.dev5/notebooks/mlruns/0/b76a83442850446399a1a55c93bac464/meta.yaml
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 stav-0.2.dev5/notebooks/mlruns/0/b76a83442850446399a1a55c93bac464/params/AIDeployer
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 stav-0.2.dev5/notebooks/mlruns/0/b76a83442850446399a1a55c93bac464/params/AIProvider
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 stav-0.2.dev5/notebooks/mlruns/0/b76a83442850446399a1a55c93bac464/params/EnergyConsumption
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 stav-0.2.dev5/notebooks/mlruns/0/b76a83442850446399a1a55c93bac464/tags/mlflow.runName
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 stav-0.2.dev5/notebooks/mlruns/0/b76a83442850446399a1a55c93bac464/tags/mlflow.source.name
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 stav-0.2.dev5/notebooks/mlruns/0/b76a83442850446399a1a55c93bac464/tags/mlflow.source.type
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 stav-0.2.dev5/notebooks/mlruns/0/b76a83442850446399a1a55c93bac464/tags/mlflow.user
--rw-r--r--   0        0        0  2246897 2020-02-02 00:00:00.000000 stav-0.2.dev5/presentations/ai-accountability-taxonomy-arthit-oss-na-20240416.pdf
--rw-r--r--   0        0        0  3015403 2020-02-02 00:00:00.000000 stav-0.2.dev5/presentations/ai-accountability-taxonomy-arthit-oss-na-20240416.pptx
--rw-r--r--   0        0        0   828085 2020-02-02 00:00:00.000000 stav-0.2.dev5/presentations/oss_na24_template.pptx
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 stav-0.2.dev5/presentations/~$ai-accountability-taxonomy-arthit-oss-na-20240416.pptx
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 stav-0.2.dev5/src/stav/__about__.py
--rw-r--r--   0        0        0     4810 2020-02-02 00:00:00.000000 stav-0.2.dev5/src/stav/__init__.py
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 stav-0.2.dev5/src/stav/eu/__init__.py
--rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 stav-0.2.dev5/src/stav/eu/aia/__init__.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 stav-0.2.dev5/tests/__init__.py
--rw-r--r--   0        0        0     9042 2020-02-02 00:00:00.000000 stav-0.2.dev5/tools/ttltopy.ipynb
--rw-r--r--   0        0        0     3568 2020-02-02 00:00:00.000000 stav-0.2.dev5/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 stav-0.2.dev5/LICENSE.txt
--rw-r--r--   0        0        0     5157 2020-02-02 00:00:00.000000 stav-0.2.dev5/README.md
--rw-r--r--   0        0        0     3098 2020-02-02 00:00:00.000000 stav-0.2.dev5/pyproject.toml
--rw-r--r--   0        0        0     6105 2020-02-02 00:00:00.000000 stav-0.2.dev5/PKG-INFO
+-rw-r--r--   0        0        0     7831 2020-02-02 00:00:00.000000 stav-0.2.dev6/ai-stakeholders.drawio
+-rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 stav-0.2.dev6/catalog-v001.xml
+-rw-r--r--   0        0        0     8905 2020-02-02 00:00:00.000000 stav-0.2.dev6/stav-eu-aia.ttl
+-rw-r--r--   0        0        0     6410 2020-02-02 00:00:00.000000 stav-0.2.dev6/stav-th-aisbd.ttl
+-rw-r--r--   0        0        0    11686 2020-02-02 00:00:00.000000 stav-0.2.dev6/stav-us-aaa.ttl
+-rw-r--r--   0        0        0    23684 2020-02-02 00:00:00.000000 stav-0.2.dev6/stav.ttl
+-rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 stav-0.2.dev6/docs/.htaccess
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 stav-0.2.dev6/docs/406.html
+-rw-r--r--   0        0        0    63347 2020-02-02 00:00:00.000000 stav-0.2.dev6/docs/index.html
+-rw-r--r--   0        0        0    31071 2020-02-02 00:00:00.000000 stav-0.2.dev6/docs/ontology.jsonld
+-rw-r--r--   0        0        0    37077 2020-02-02 00:00:00.000000 stav-0.2.dev6/docs/ontology.nt
+-rw-r--r--   0        0        0    28158 2020-02-02 00:00:00.000000 stav-0.2.dev6/docs/ontology.owl
+-rw-r--r--   0        0        0    26430 2020-02-02 00:00:00.000000 stav-0.2.dev6/docs/ontology.ttl
+-rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 stav-0.2.dev6/docs/readme.md
+-rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 stav-0.2.dev6/docs/resources/extra.css
+-rw-r--r--   0        0        0    91556 2020-02-02 00:00:00.000000 stav-0.2.dev6/docs/resources/jquery.js
+-rw-r--r--   0        0        0    47959 2020-02-02 00:00:00.000000 stav-0.2.dev6/docs/resources/marked.min.js
+-rw-r--r--   0        0        0     4389 2020-02-02 00:00:00.000000 stav-0.2.dev6/docs/resources/owl.css
+-rw-r--r--   0        0        0     2491 2020-02-02 00:00:00.000000 stav-0.2.dev6/docs/resources/primer.css
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 stav-0.2.dev6/docs/resources/rdf.icon
+-rw-r--r--   0        0        0     2459 2020-02-02 00:00:00.000000 stav-0.2.dev6/docs/resources/rec.css
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 stav-0.2.dev6/docs/webvowl/favicon.ico
+-rw-r--r--   0        0        0    35533 2020-02-02 00:00:00.000000 stav-0.2.dev6/docs/webvowl/index.html
+-rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 stav-0.2.dev6/docs/webvowl/license.txt
+-rw-r--r--   0        0        0    42681 2020-02-02 00:00:00.000000 stav-0.2.dev6/docs/webvowl/css/webvowl.app.css
+-rw-r--r--   0        0        0     5341 2020-02-02 00:00:00.000000 stav-0.2.dev6/docs/webvowl/css/webvowl.css
+-rw-r--r--   0        0        0    74704 2020-02-02 00:00:00.000000 stav-0.2.dev6/docs/webvowl/data/foaf.json
+-rw-r--r--   0        0        0    39197 2020-02-02 00:00:00.000000 stav-0.2.dev6/docs/webvowl/data/ontology.json
+-rw-r--r--   0        0        0     2705 2020-02-02 00:00:00.000000 stav-0.2.dev6/docs/webvowl/data/template.json
+-rw-r--r--   0        0        0   151725 2020-02-02 00:00:00.000000 stav-0.2.dev6/docs/webvowl/js/d3.min.js
+-rw-r--r--   0        0        0   350028 2020-02-02 00:00:00.000000 stav-0.2.dev6/docs/webvowl/js/webvowl.app.js
+-rw-r--r--   0        0        0   751167 2020-02-02 00:00:00.000000 stav-0.2.dev6/docs/webvowl/js/webvowl.js
+-rw-r--r--   0        0        0    14826 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlflowstav.ipynb
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/use_instruction.txt
+-rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlartifacts/0/0f1f09d1ac1a4f05a1bbb4159cd331dd/artifacts/iris_model/MLmodel
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlartifacts/0/0f1f09d1ac1a4f05a1bbb4159cd331dd/artifacts/iris_model/conda.yaml
+-rw-r--r--   0        0        0     2652 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlartifacts/0/0f1f09d1ac1a4f05a1bbb4159cd331dd/artifacts/iris_model/input_example.json
+-rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlartifacts/0/0f1f09d1ac1a4f05a1bbb4159cd331dd/artifacts/iris_model/model.pkl
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlartifacts/0/0f1f09d1ac1a4f05a1bbb4159cd331dd/artifacts/iris_model/python_env.yaml
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlartifacts/0/0f1f09d1ac1a4f05a1bbb4159cd331dd/artifacts/iris_model/requirements.txt
+-rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlartifacts/0/0f1f09d1ac1a4f05a1bbb4159cd331dd/artifacts/iris_model/metadata/MLmodel
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlartifacts/0/0f1f09d1ac1a4f05a1bbb4159cd331dd/artifacts/iris_model/metadata/conda.yaml
+-rw-r--r--   0        0        0     2652 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlartifacts/0/0f1f09d1ac1a4f05a1bbb4159cd331dd/artifacts/iris_model/metadata/input_example.json
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlartifacts/0/0f1f09d1ac1a4f05a1bbb4159cd331dd/artifacts/iris_model/metadata/python_env.yaml
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlartifacts/0/0f1f09d1ac1a4f05a1bbb4159cd331dd/artifacts/iris_model/metadata/requirements.txt
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlruns/0/meta.yaml
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlruns/0/057720ec8a574ba28fdb7f38fa41ea75/meta.yaml
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlruns/0/057720ec8a574ba28fdb7f38fa41ea75/params/AIDeployer
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlruns/0/057720ec8a574ba28fdb7f38fa41ea75/params/AIProvider
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlruns/0/057720ec8a574ba28fdb7f38fa41ea75/params/autonomyType
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlruns/0/057720ec8a574ba28fdb7f38fa41ea75/params/hyperparameter
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlruns/0/057720ec8a574ba28fdb7f38fa41ea75/params/useSensitivePersonalInformation
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlruns/0/057720ec8a574ba28fdb7f38fa41ea75/tags/Training Info
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlruns/0/057720ec8a574ba28fdb7f38fa41ea75/tags/mlflow.runName
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlruns/0/057720ec8a574ba28fdb7f38fa41ea75/tags/mlflow.source.name
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlruns/0/057720ec8a574ba28fdb7f38fa41ea75/tags/mlflow.source.type
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlruns/0/057720ec8a574ba28fdb7f38fa41ea75/tags/mlflow.user
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlruns/0/05a0023896ae40278d5a32e52a12060b/meta.yaml
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlruns/0/05a0023896ae40278d5a32e52a12060b/params/AIDeployer
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlruns/0/05a0023896ae40278d5a32e52a12060b/params/AIProvider
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlruns/0/05a0023896ae40278d5a32e52a12060b/params/hyperparameter
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlruns/0/05a0023896ae40278d5a32e52a12060b/params/metric
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlruns/0/05a0023896ae40278d5a32e52a12060b/params/useSensitivePersonalInformation
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlruns/0/05a0023896ae40278d5a32e52a12060b/tags/mlflow.runName
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlruns/0/05a0023896ae40278d5a32e52a12060b/tags/mlflow.source.name
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlruns/0/05a0023896ae40278d5a32e52a12060b/tags/mlflow.source.type
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlruns/0/05a0023896ae40278d5a32e52a12060b/tags/mlflow.user
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlruns/0/0f1f09d1ac1a4f05a1bbb4159cd331dd/meta.yaml
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlruns/0/0f1f09d1ac1a4f05a1bbb4159cd331dd/metrics/MetricsPrecision
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlruns/0/0f1f09d1ac1a4f05a1bbb4159cd331dd/params/hyperparameter
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlruns/0/0f1f09d1ac1a4f05a1bbb4159cd331dd/params/max_iter
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlruns/0/0f1f09d1ac1a4f05a1bbb4159cd331dd/params/multi_class
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlruns/0/0f1f09d1ac1a4f05a1bbb4159cd331dd/params/random_state
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlruns/0/0f1f09d1ac1a4f05a1bbb4159cd331dd/params/solver
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlruns/0/0f1f09d1ac1a4f05a1bbb4159cd331dd/tags/Training Info
+-rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlruns/0/0f1f09d1ac1a4f05a1bbb4159cd331dd/tags/mlflow.log-model.history
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlruns/0/0f1f09d1ac1a4f05a1bbb4159cd331dd/tags/mlflow.runName
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlruns/0/0f1f09d1ac1a4f05a1bbb4159cd331dd/tags/mlflow.source.name
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlruns/0/0f1f09d1ac1a4f05a1bbb4159cd331dd/tags/mlflow.source.type
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlruns/0/0f1f09d1ac1a4f05a1bbb4159cd331dd/tags/mlflow.user
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlruns/0/23de15e0ef364056ac9705a401580373/meta.yaml
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlruns/0/23de15e0ef364056ac9705a401580373/tags/Training Info
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlruns/0/23de15e0ef364056ac9705a401580373/tags/mlflow.runName
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlruns/0/23de15e0ef364056ac9705a401580373/tags/mlflow.source.name
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlruns/0/23de15e0ef364056ac9705a401580373/tags/mlflow.source.type
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlruns/0/23de15e0ef364056ac9705a401580373/tags/mlflow.user
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlruns/0/32346fc378d04ae18e934e53c9748818/meta.yaml
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlruns/0/32346fc378d04ae18e934e53c9748818/params/AIDeployer
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlruns/0/32346fc378d04ae18e934e53c9748818/params/AIProvider
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlruns/0/32346fc378d04ae18e934e53c9748818/params/energyConsumption
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlruns/0/32346fc378d04ae18e934e53c9748818/params/useSensitivePersonalInformation
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlruns/0/32346fc378d04ae18e934e53c9748818/tags/mlflow.runName
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlruns/0/32346fc378d04ae18e934e53c9748818/tags/mlflow.source.name
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlruns/0/32346fc378d04ae18e934e53c9748818/tags/mlflow.source.type
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlruns/0/32346fc378d04ae18e934e53c9748818/tags/mlflow.user
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlruns/0/3d1c746c329d41f39b3397fea51d98df/meta.yaml
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlruns/0/3d1c746c329d41f39b3397fea51d98df/params/AIDeployer
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlruns/0/3d1c746c329d41f39b3397fea51d98df/params/AIProvider
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlruns/0/3d1c746c329d41f39b3397fea51d98df/params/autonomyType
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlruns/0/3d1c746c329d41f39b3397fea51d98df/params/hyperparameter
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlruns/0/3d1c746c329d41f39b3397fea51d98df/params/metric
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlruns/0/3d1c746c329d41f39b3397fea51d98df/params/useSensitivePersonalInformation
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlruns/0/3d1c746c329d41f39b3397fea51d98df/tags/mlflow.runName
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlruns/0/3d1c746c329d41f39b3397fea51d98df/tags/mlflow.source.name
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlruns/0/3d1c746c329d41f39b3397fea51d98df/tags/mlflow.source.type
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlruns/0/3d1c746c329d41f39b3397fea51d98df/tags/mlflow.user
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlruns/0/9706b4766d324006bd0259f446b75b25/meta.yaml
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlruns/0/9706b4766d324006bd0259f446b75b25/params/hyperparameter
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlruns/0/9706b4766d324006bd0259f446b75b25/params/max_iter
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlruns/0/9706b4766d324006bd0259f446b75b25/params/multi_class
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlruns/0/9706b4766d324006bd0259f446b75b25/params/random_state
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlruns/0/9706b4766d324006bd0259f446b75b25/params/solver
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlruns/0/9706b4766d324006bd0259f446b75b25/tags/Training Info
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlruns/0/9706b4766d324006bd0259f446b75b25/tags/mlflow.runName
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlruns/0/9706b4766d324006bd0259f446b75b25/tags/mlflow.source.name
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlruns/0/9706b4766d324006bd0259f446b75b25/tags/mlflow.source.type
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlruns/0/9706b4766d324006bd0259f446b75b25/tags/mlflow.user
+-rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlruns/0/98fc0c442e6d40378f55757bb5e6e8cb/meta.yaml
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlruns/0/98fc0c442e6d40378f55757bb5e6e8cb/params/hyperparameter
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlruns/0/98fc0c442e6d40378f55757bb5e6e8cb/params/max_iter
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlruns/0/98fc0c442e6d40378f55757bb5e6e8cb/params/multi_class
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlruns/0/98fc0c442e6d40378f55757bb5e6e8cb/params/random_state
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlruns/0/98fc0c442e6d40378f55757bb5e6e8cb/params/solver
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlruns/0/98fc0c442e6d40378f55757bb5e6e8cb/tags/Training Info
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlruns/0/98fc0c442e6d40378f55757bb5e6e8cb/tags/mlflow.runName
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlruns/0/98fc0c442e6d40378f55757bb5e6e8cb/tags/mlflow.source.name
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlruns/0/98fc0c442e6d40378f55757bb5e6e8cb/tags/mlflow.source.type
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlruns/0/98fc0c442e6d40378f55757bb5e6e8cb/tags/mlflow.user
+-rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlruns/0/9a8feecd4e674c0f82024548a121e087/meta.yaml
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlruns/0/9a8feecd4e674c0f82024548a121e087/params/AIDeployer
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlruns/0/9a8feecd4e674c0f82024548a121e087/params/AIProvider
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlruns/0/9a8feecd4e674c0f82024548a121e087/params/hyperparameter
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlruns/0/9a8feecd4e674c0f82024548a121e087/params/metric
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlruns/0/9a8feecd4e674c0f82024548a121e087/params/useSensitivePersonalInformation
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlruns/0/9a8feecd4e674c0f82024548a121e087/tags/mlflow.runName
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlruns/0/9a8feecd4e674c0f82024548a121e087/tags/mlflow.source.name
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlruns/0/9a8feecd4e674c0f82024548a121e087/tags/mlflow.source.type
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlruns/0/9a8feecd4e674c0f82024548a121e087/tags/mlflow.user
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlruns/0/9c28f429940f437799170cc7eee1429b/meta.yaml
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlruns/0/9c28f429940f437799170cc7eee1429b/params/AIDeployer
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlruns/0/9c28f429940f437799170cc7eee1429b/params/AIProvider
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlruns/0/9c28f429940f437799170cc7eee1429b/params/hyperparameter
+-rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlruns/0/9c28f429940f437799170cc7eee1429b/params/metric
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlruns/0/9c28f429940f437799170cc7eee1429b/params/useSensitivePersonalInformation
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlruns/0/9c28f429940f437799170cc7eee1429b/tags/mlflow.runName
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlruns/0/9c28f429940f437799170cc7eee1429b/tags/mlflow.source.name
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlruns/0/9c28f429940f437799170cc7eee1429b/tags/mlflow.source.type
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlruns/0/9c28f429940f437799170cc7eee1429b/tags/mlflow.user
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlruns/0/9fd4690261d34febb0a1e23d7dc63d37/meta.yaml
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlruns/0/9fd4690261d34febb0a1e23d7dc63d37/params/AIDeployer
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlruns/0/9fd4690261d34febb0a1e23d7dc63d37/params/AIProvider
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlruns/0/9fd4690261d34febb0a1e23d7dc63d37/params/hyperparameter
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlruns/0/9fd4690261d34febb0a1e23d7dc63d37/params/metric
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlruns/0/9fd4690261d34febb0a1e23d7dc63d37/params/useSensitivePersonalInformation
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlruns/0/9fd4690261d34febb0a1e23d7dc63d37/tags/mlflow.runName
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlruns/0/9fd4690261d34febb0a1e23d7dc63d37/tags/mlflow.source.name
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlruns/0/9fd4690261d34febb0a1e23d7dc63d37/tags/mlflow.source.type
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlruns/0/9fd4690261d34febb0a1e23d7dc63d37/tags/mlflow.user
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlruns/0/b76a83442850446399a1a55c93bac464/meta.yaml
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlruns/0/b76a83442850446399a1a55c93bac464/params/AIDeployer
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlruns/0/b76a83442850446399a1a55c93bac464/params/AIProvider
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlruns/0/b76a83442850446399a1a55c93bac464/params/EnergyConsumption
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlruns/0/b76a83442850446399a1a55c93bac464/tags/mlflow.runName
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlruns/0/b76a83442850446399a1a55c93bac464/tags/mlflow.source.name
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlruns/0/b76a83442850446399a1a55c93bac464/tags/mlflow.source.type
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlruns/0/b76a83442850446399a1a55c93bac464/tags/mlflow.user
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlruns/models/tracking-quickstart/meta.yaml
+-rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 stav-0.2.dev6/notebooks/mlruns/models/tracking-quickstart/version-1/meta.yaml
+-rw-r--r--   0        0        0  2246897 2020-02-02 00:00:00.000000 stav-0.2.dev6/presentations/ai-accountability-taxonomy-arthit-oss-na-20240416.pdf
+-rw-r--r--   0        0        0  3015403 2020-02-02 00:00:00.000000 stav-0.2.dev6/presentations/ai-accountability-taxonomy-arthit-oss-na-20240416.pptx
+-rw-r--r--   0        0        0   828085 2020-02-02 00:00:00.000000 stav-0.2.dev6/presentations/oss_na24_template.pptx
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 stav-0.2.dev6/presentations/~$ai-accountability-taxonomy-arthit-oss-na-20240416.pptx
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 stav-0.2.dev6/src/stav/__about__.py
+-rw-r--r--   0        0        0     4871 2020-02-02 00:00:00.000000 stav-0.2.dev6/src/stav/__init__.py
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 stav-0.2.dev6/src/stav/eu/__init__.py
+-rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 stav-0.2.dev6/src/stav/eu/aia/__init__.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 stav-0.2.dev6/tests/__init__.py
+-rw-r--r--   0        0        0     9042 2020-02-02 00:00:00.000000 stav-0.2.dev6/tools/ttltopy.ipynb
+-rw-r--r--   0        0        0     3568 2020-02-02 00:00:00.000000 stav-0.2.dev6/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 stav-0.2.dev6/LICENSE.txt
+-rw-r--r--   0        0        0     5157 2020-02-02 00:00:00.000000 stav-0.2.dev6/README.md
+-rw-r--r--   0        0        0     3098 2020-02-02 00:00:00.000000 stav-0.2.dev6/pyproject.toml
+-rw-r--r--   0        0        0     6105 2020-02-02 00:00:00.000000 stav-0.2.dev6/PKG-INFO
```

### Comparing `stav-0.2.dev5/ai-stakeholders.drawio` & `stav-0.2.dev6/ai-stakeholders.drawio`

 * *Files identical despite different names*

### Comparing `stav-0.2.dev5/catalog-v001.xml` & `stav-0.2.dev6/catalog-v001.xml`

 * *Files identical despite different names*

### Comparing `stav-0.2.dev5/stav-eu-aia.ttl` & `stav-0.2.dev6/stav-eu-aia.ttl`

 * *Files identical despite different names*

### Comparing `stav-0.2.dev5/stav-th-aisbd.ttl` & `stav-0.2.dev6/stav-th-aisbd.ttl`

 * *Files identical despite different names*

### Comparing `stav-0.2.dev5/stav-us-aaa.ttl` & `stav-0.2.dev6/stav-us-aaa.ttl`

 * *Files identical despite different names*

### Comparing `stav-0.2.dev5/stav.ttl` & `stav-0.2.dev6/stav.ttl`

 * *Files identical despite different names*

### Comparing `stav-0.2.dev5/docs/.htaccess` & `stav-0.2.dev6/docs/.htaccess`

 * *Files identical despite different names*

### Comparing `stav-0.2.dev5/docs/index.html` & `stav-0.2.dev6/docs/index.html`

 * *Files identical despite different names*

### Comparing `stav-0.2.dev5/docs/ontology.jsonld` & `stav-0.2.dev6/docs/ontology.jsonld`

 * *Files identical despite different names*

### Comparing `stav-0.2.dev5/docs/ontology.nt` & `stav-0.2.dev6/docs/ontology.nt`

 * *Files identical despite different names*

### Comparing `stav-0.2.dev5/docs/ontology.owl` & `stav-0.2.dev6/docs/ontology.owl`

 * *Files identical despite different names*

### Comparing `stav-0.2.dev5/docs/ontology.ttl` & `stav-0.2.dev6/docs/ontology.ttl`

 * *Files identical despite different names*

### Comparing `stav-0.2.dev5/docs/readme.md` & `stav-0.2.dev6/docs/readme.md`

 * *Files identical despite different names*

### Comparing `stav-0.2.dev5/docs/resources/extra.css` & `stav-0.2.dev6/docs/resources/extra.css`

 * *Files identical despite different names*

### Comparing `stav-0.2.dev5/docs/resources/jquery.js` & `stav-0.2.dev6/docs/resources/jquery.js`

 * *Files identical despite different names*

### Comparing `stav-0.2.dev5/docs/resources/marked.min.js` & `stav-0.2.dev6/docs/resources/marked.min.js`

 * *Files identical despite different names*

### Comparing `stav-0.2.dev5/docs/resources/owl.css` & `stav-0.2.dev6/docs/resources/owl.css`

 * *Files identical despite different names*

### Comparing `stav-0.2.dev5/docs/resources/primer.css` & `stav-0.2.dev6/docs/resources/primer.css`

 * *Files identical despite different names*

### Comparing `stav-0.2.dev5/docs/resources/rec.css` & `stav-0.2.dev6/docs/resources/rec.css`

 * *Files identical despite different names*

### Comparing `stav-0.2.dev5/docs/webvowl/favicon.ico` & `stav-0.2.dev6/docs/webvowl/favicon.ico`

 * *Files identical despite different names*

### Comparing `stav-0.2.dev5/docs/webvowl/index.html` & `stav-0.2.dev6/docs/webvowl/index.html`

 * *Files identical despite different names*

### Comparing `stav-0.2.dev5/docs/webvowl/license.txt` & `stav-0.2.dev6/docs/webvowl/license.txt`

 * *Files identical despite different names*

### Comparing `stav-0.2.dev5/docs/webvowl/css/webvowl.app.css` & `stav-0.2.dev6/docs/webvowl/css/webvowl.app.css`

 * *Files identical despite different names*

### Comparing `stav-0.2.dev5/docs/webvowl/css/webvowl.css` & `stav-0.2.dev6/docs/webvowl/css/webvowl.css`

 * *Files identical despite different names*

### Comparing `stav-0.2.dev5/docs/webvowl/data/foaf.json` & `stav-0.2.dev6/docs/webvowl/data/foaf.json`

 * *Files identical despite different names*

### Comparing `stav-0.2.dev5/docs/webvowl/data/ontology.json` & `stav-0.2.dev6/docs/webvowl/data/ontology.json`

 * *Files identical despite different names*

### Comparing `stav-0.2.dev5/docs/webvowl/data/template.json` & `stav-0.2.dev6/docs/webvowl/data/template.json`

 * *Files identical despite different names*

### Comparing `stav-0.2.dev5/docs/webvowl/js/d3.min.js` & `stav-0.2.dev6/docs/webvowl/js/d3.min.js`

 * *Files identical despite different names*

### Comparing `stav-0.2.dev5/docs/webvowl/js/webvowl.app.js` & `stav-0.2.dev6/docs/webvowl/js/webvowl.app.js`

 * *Files identical despite different names*

### Comparing `stav-0.2.dev5/docs/webvowl/js/webvowl.js` & `stav-0.2.dev6/docs/webvowl/js/webvowl.js`

 * *Files identical despite different names*

### Comparing `stav-0.2.dev5/presentations/ai-accountability-taxonomy-arthit-oss-na-20240416.pdf` & `stav-0.2.dev6/presentations/ai-accountability-taxonomy-arthit-oss-na-20240416.pdf`

 * *Files identical despite different names*

### Comparing `stav-0.2.dev5/presentations/ai-accountability-taxonomy-arthit-oss-na-20240416.pptx` & `stav-0.2.dev6/presentations/ai-accountability-taxonomy-arthit-oss-na-20240416.pptx`

 * *Files identical despite different names*

### Comparing `stav-0.2.dev5/presentations/oss_na24_template.pptx` & `stav-0.2.dev6/presentations/oss_na24_template.pptx`

 * *Files identical despite different names*

### Comparing `stav-0.2.dev5/src/stav/__init__.py` & `stav-0.2.dev6/src/stav/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,16 +44,17 @@
 PLACING_ON_THE_MARKET = "PlacingOnTheMarket"
 PUTTING_INTO_SERVICE = "PuttingIntoService"
 
 # Measures
 INFORMATION_SECURITY_MEASURES = "InformationSecurityMeasures"
 
 # Metrics
-METRICS_RECALL = "MetricsRecall"
+METRICS_ACCURACY = "MetricsAccuracy"
 METRICS_PRECISION = "MetricsPrecision"
+METRICS_RECALL = "MetricsRecall"
 METRICS_F1 = "MetricsF1"
 METRICS_R2 = "MetricsR2"
 METRICS_RMSE = "MetricsRMSE"
 METRICS_MAE = "MetricsMAE"
 METRICS_ENERGY = "MetricsEnergy"
 
 LOG = "Log"
@@ -113,14 +114,15 @@
     "METRICS_RECALL",
     "METRICS_PRECISION",
     "METRICS_F1",
     "METRICS_R2",
     "METRICS_RMSE",
     "METRICS_MAE",
     "METRICS_ENERGY",
+    "METRICS_ACCURACY",
     "DATASET_SIZE",
     "AUTONOMY_TYPE",
     "DOMAIN",
     "ENERGY_CONSUMPTION",
     "HYPERPARAMETER",
     "INFO_APP",
     "INFO_TRAINING",
```

### Comparing `stav-0.2.dev5/src/stav/eu/aia/__init__.py` & `stav-0.2.dev6/src/stav/eu/aia/__init__.py`

 * *Files identical despite different names*

### Comparing `stav-0.2.dev5/tools/ttltopy.ipynb` & `stav-0.2.dev6/tools/ttltopy.ipynb`

 * *Files identical despite different names*

### Comparing `stav-0.2.dev5/.gitignore` & `stav-0.2.dev6/.gitignore`

 * *Files identical despite different names*

### Comparing `stav-0.2.dev5/LICENSE.txt` & `stav-0.2.dev6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `stav-0.2.dev5/README.md` & `stav-0.2.dev6/README.md`

 * *Files identical despite different names*

### Comparing `stav-0.2.dev5/pyproject.toml` & `stav-0.2.dev6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `stav-0.2.dev5/PKG-INFO` & `stav-0.2.dev6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: stav
-Version: 0.2.dev5
+Version: 0.2.dev6
 Summary: System Trustworthiness and Accountability Vocabulary
 Project-URL: Documentation, https://github.com/unknown/stav#readme
 Project-URL: Issues, https://github.com/unknown/stav/issues
 Project-URL: Source, https://github.com/unknown/stav
 Author-email: Arthit Suriyawongkul <arthit@gmail.com>
 License-Expression: Apache-2.0
 License-File: LICENSE.txt
```

