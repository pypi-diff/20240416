# Comparing `tmp/astro_provider_databricks-0.2.1.tar.gz` & `tmp/astro_provider_databricks-0.2.2.tar.gz`

## Comparing `astro_provider_databricks-0.2.1.tar` & `astro_provider_databricks-0.2.2.tar`

### file list

```diff
@@ -1,69 +1,69 @@
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/.deepsource.toml
--rw-r--r--   0        0        0     2570 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     4341 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/CHANGELOG.rst
--rw-r--r--   0        0        0     5218 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/Tiltfile
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/codecov.yml
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/mlc-config.json
--rw-r--r--   0        0        0     2395 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/noxfile.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/yamllint-config.yml
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/.github/CODEOWNERS
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/.github/ci-test-connections.yaml
--rwxr-xr-x   0        0        0      696 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/.github/scripts/verify_tag_and_version.py
--rw-r--r--   0        0        0     7342 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/.github/workflows/ci.yml
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/.github/workflows/docs.yml
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/.github/workflows/mlc_config.json
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/dev/.dockerignore
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/dev/.gitignore
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/dev/Dockerfile
--rw-r--r--   0        0        0     4359 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/dev/docker-compose.yaml
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/dev/packages.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/dev/requirements.txt
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/dev/.astro/config.yaml
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/docs/Makefile
--rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/docs/conf.py
--rw-r--r--   0        0        0     2820 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/docs/contributing.rst
--rw-r--r--   0        0        0     5262 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/docs/index.rst
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/docs/make.bat
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/docs/requirements.txt
--rw-r--r--   0        0        0   737260 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/docs/_static/banner.png
--rw-r--r--   0        0        0   146128 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/docs/_static/dbt_dag.png
--rw-r--r--   0        0        0   361967 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/docs/_static/dbt_task_group.png
--rw-r--r--   0        0        0    10419 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/docs/_static/logo-dark.png
--rw-r--r--   0        0        0    11220 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/docs/_static/logo-light.png
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/docs/_static/css/custom.css
--rw-r--r--   0        0        0   212922 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/docs/_static/screenshots/workflow_1_airflow.png
--rw-r--r--   0        0        0   763410 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/docs/_static/screenshots/workflow_1_databricks.png
--rw-r--r--   0        0        0    30924 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/docs/assets/images/dbutils-notebook-success.png
--rw-r--r--   0        0        0    73030 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/docs/assets/images/repair-all-failed.png
--rw-r--r--   0        0        0   140389 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/docs/assets/images/repair-single-failed.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/example_dags/.airflowignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/example_dags/__init__.py
--rw-r--r--   0        0        0     1996 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/example_dags/example_databricks_notebook.py
--rw-r--r--   0        0        0     3811 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/example_dags/example_databricks_workflow.py
--rw-r--r--   0        0        0     3050 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/example_dags/example_task_group.py
--rw-r--r--   0        0        0     1970 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/quickstart/astro-cli.md
--rw-r--r--   0        0        0     2773 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/quickstart/without-astro-cli.md
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/astro_databricks/__init__.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/astro_databricks/settings.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/astro_databricks/operators/__init__.py
--rw-r--r--   0        0        0    13366 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/astro_databricks/operators/common.py
--rw-r--r--   0        0        0    15234 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/astro_databricks/operators/notebook.py
--rw-r--r--   0        0        0    17184 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/astro_databricks/operators/workflow.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/astro_databricks/plugins/__init__.py
--rw-r--r--   0        0        0    18556 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/astro_databricks/plugins/plugin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/tests/__init__.py
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/tests/conftest.py
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/tests/pytest.ini
--rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/tests/test_example_dags.py
--rw-r--r--   0        0        0     6352 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/tests/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/tests/databricks/__init__.py
--rw-r--r--   0        0        0    14764 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/tests/databricks/test_common.py
--rw-r--r--   0        0        0    15473 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/tests/databricks/test_notebook.py
--rw-r--r--   0        0        0    15212 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/tests/databricks/test_plugin.py
--rw-r--r--   0        0        0    16684 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/tests/databricks/test_workflow.py
--rw-r--r--   0        0        0     2058 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/LICENSE
--rw-r--r--   0        0        0     6173 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/README.md
--rw-r--r--   0        0        0     3559 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     8164 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.2/.deepsource.toml
+-rw-r--r--   0        0        0     2570 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     4531 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.2/CHANGELOG.rst
+-rw-r--r--   0        0        0     5218 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.2/Tiltfile
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.2/codecov.yml
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.2/mlc-config.json
+-rw-r--r--   0        0        0     2395 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.2/noxfile.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.2/yamllint-config.yml
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.2/.github/CODEOWNERS
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.2/.github/ci-test-connections.yaml
+-rwxr-xr-x   0        0        0      696 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.2/.github/scripts/verify_tag_and_version.py
+-rw-r--r--   0        0        0     7342 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.2/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.2/.github/workflows/docs.yml
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.2/.github/workflows/mlc_config.json
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.2/dev/.dockerignore
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.2/dev/.gitignore
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.2/dev/Dockerfile
+-rw-r--r--   0        0        0     4359 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.2/dev/docker-compose.yaml
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.2/dev/packages.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.2/dev/requirements.txt
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.2/dev/.astro/config.yaml
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.2/docs/Makefile
+-rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.2/docs/conf.py
+-rw-r--r--   0        0        0     2820 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.2/docs/contributing.rst
+-rw-r--r--   0        0        0     5262 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.2/docs/index.rst
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.2/docs/make.bat
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.2/docs/requirements.txt
+-rw-r--r--   0        0        0   737260 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.2/docs/_static/banner.png
+-rw-r--r--   0        0        0   146128 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.2/docs/_static/dbt_dag.png
+-rw-r--r--   0        0        0   361967 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.2/docs/_static/dbt_task_group.png
+-rw-r--r--   0        0        0    10419 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.2/docs/_static/logo-dark.png
+-rw-r--r--   0        0        0    11220 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.2/docs/_static/logo-light.png
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.2/docs/_static/css/custom.css
+-rw-r--r--   0        0        0   212922 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.2/docs/_static/screenshots/workflow_1_airflow.png
+-rw-r--r--   0        0        0   763410 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.2/docs/_static/screenshots/workflow_1_databricks.png
+-rw-r--r--   0        0        0    30924 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.2/docs/assets/images/dbutils-notebook-success.png
+-rw-r--r--   0        0        0    73030 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.2/docs/assets/images/repair-all-failed.png
+-rw-r--r--   0        0        0   140389 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.2/docs/assets/images/repair-single-failed.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.2/example_dags/.airflowignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.2/example_dags/__init__.py
+-rw-r--r--   0        0        0     1996 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.2/example_dags/example_databricks_notebook.py
+-rw-r--r--   0        0        0     3811 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.2/example_dags/example_databricks_workflow.py
+-rw-r--r--   0        0        0     3050 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.2/example_dags/example_task_group.py
+-rw-r--r--   0        0        0     1970 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.2/quickstart/astro-cli.md
+-rw-r--r--   0        0        0     2773 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.2/quickstart/without-astro-cli.md
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.2/astro_databricks/__init__.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.2/astro_databricks/settings.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.2/astro_databricks/operators/__init__.py
+-rw-r--r--   0        0        0    13366 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.2/astro_databricks/operators/common.py
+-rw-r--r--   0        0        0    15234 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.2/astro_databricks/operators/notebook.py
+-rw-r--r--   0        0        0    17117 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.2/astro_databricks/operators/workflow.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.2/astro_databricks/plugins/__init__.py
+-rw-r--r--   0        0        0    18556 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.2/astro_databricks/plugins/plugin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.2/tests/__init__.py
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.2/tests/conftest.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.2/tests/pytest.ini
+-rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.2/tests/test_example_dags.py
+-rw-r--r--   0        0        0     6352 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.2/tests/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.2/tests/databricks/__init__.py
+-rw-r--r--   0        0        0    14764 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.2/tests/databricks/test_common.py
+-rw-r--r--   0        0        0    15473 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.2/tests/databricks/test_notebook.py
+-rw-r--r--   0        0        0    15212 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.2/tests/databricks/test_plugin.py
+-rw-r--r--   0        0        0    17119 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.2/tests/databricks/test_workflow.py
+-rw-r--r--   0        0        0     2058 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.2/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.2/LICENSE
+-rw-r--r--   0        0        0     6173 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.2/README.md
+-rw-r--r--   0        0        0     3559 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     8164 2020-02-02 00:00:00.000000 astro_provider_databricks-0.2.2/PKG-INFO
```

### Comparing `astro_provider_databricks-0.2.1/.pre-commit-config.yaml` & `astro_provider_databricks-0.2.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.2.1/CHANGELOG.rst` & `astro_provider_databricks-0.2.2/CHANGELOG.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 Changelog
 =========
 
+0.2.2 (16-04-24)
+----------------
+
+Bug fixes
+
+* Prevent creation of duplicate jobs in Databricks (PR `#76 <https://github.com/astronomer/astro-provider-databricks/pull/76>`_ by @Hang1225)
+
+
 0.2.1 (03-04-24)
 ----------------
 
 Bug fixes
 
 * Support ``existing_cluster_id`` for ``DatabricksNotebookOperator`` when used from within ``DatabricksWorkflowTaskGroup`` (PR `#73 <https://github.com/astronomer/astro-provider-databricks/pull/73>`_ by @Hang1225)
```

### Comparing `astro_provider_databricks-0.2.1/CODE_OF_CONDUCT.md` & `astro_provider_databricks-0.2.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.2.1/Tiltfile` & `astro_provider_databricks-0.2.2/Tiltfile`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.2.1/noxfile.py` & `astro_provider_databricks-0.2.2/noxfile.py`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.2.1/.github/scripts/verify_tag_and_version.py` & `astro_provider_databricks-0.2.2/.github/scripts/verify_tag_and_version.py`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.2.1/.github/workflows/ci.yml` & `astro_provider_databricks-0.2.2/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.2.1/.github/workflows/docs.yml` & `astro_provider_databricks-0.2.2/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.2.1/dev/Dockerfile` & `astro_provider_databricks-0.2.2/dev/Dockerfile`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.2.1/dev/docker-compose.yaml` & `astro_provider_databricks-0.2.2/dev/docker-compose.yaml`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.2.1/docs/Makefile` & `astro_provider_databricks-0.2.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.2.1/docs/conf.py` & `astro_provider_databricks-0.2.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.2.1/docs/contributing.rst` & `astro_provider_databricks-0.2.2/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.2.1/docs/index.rst` & `astro_provider_databricks-0.2.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.2.1/docs/make.bat` & `astro_provider_databricks-0.2.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.2.1/docs/_static/banner.png` & `astro_provider_databricks-0.2.2/docs/_static/banner.png`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.2.1/docs/_static/dbt_dag.png` & `astro_provider_databricks-0.2.2/docs/_static/dbt_dag.png`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.2.1/docs/_static/dbt_task_group.png` & `astro_provider_databricks-0.2.2/docs/_static/dbt_task_group.png`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.2.1/docs/_static/logo-dark.png` & `astro_provider_databricks-0.2.2/docs/_static/logo-dark.png`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.2.1/docs/_static/logo-light.png` & `astro_provider_databricks-0.2.2/docs/_static/logo-light.png`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.2.1/docs/_static/screenshots/workflow_1_airflow.png` & `astro_provider_databricks-0.2.2/docs/_static/screenshots/workflow_1_airflow.png`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.2.1/docs/_static/screenshots/workflow_1_databricks.png` & `astro_provider_databricks-0.2.2/docs/_static/screenshots/workflow_1_databricks.png`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.2.1/docs/assets/images/dbutils-notebook-success.png` & `astro_provider_databricks-0.2.2/docs/assets/images/dbutils-notebook-success.png`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.2.1/docs/assets/images/repair-all-failed.png` & `astro_provider_databricks-0.2.2/docs/assets/images/repair-all-failed.png`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.2.1/docs/assets/images/repair-single-failed.png` & `astro_provider_databricks-0.2.2/docs/assets/images/repair-single-failed.png`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.2.1/example_dags/example_databricks_notebook.py` & `astro_provider_databricks-0.2.2/example_dags/example_databricks_notebook.py`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.2.1/example_dags/example_databricks_workflow.py` & `astro_provider_databricks-0.2.2/example_dags/example_databricks_workflow.py`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.2.1/example_dags/example_task_group.py` & `astro_provider_databricks-0.2.2/example_dags/example_task_group.py`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.2.1/quickstart/astro-cli.md` & `astro_provider_databricks-0.2.2/quickstart/astro-cli.md`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.2.1/quickstart/without-astro-cli.md` & `astro_provider_databricks-0.2.2/quickstart/without-astro-cli.md`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.2.1/astro_databricks/operators/common.py` & `astro_provider_databricks-0.2.2/astro_databricks/operators/common.py`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.2.1/astro_databricks/operators/notebook.py` & `astro_provider_databricks-0.2.2/astro_databricks/operators/notebook.py`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.2.1/astro_databricks/operators/workflow.py` & `astro_provider_databricks-0.2.2/astro_databricks/operators/workflow.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,19 +37,16 @@
 class DatabricksMetaData:
     databricks_conn_id: str
     databricks_run_id: str
     databricks_job_id: str
 
 
 def _get_job_by_name(job_name: str, jobs_api: JobsApi) -> dict | None:
-    jobs = jobs_api.list_jobs(version=DATABRICKS_JOBS_API_VERSION).get("jobs", [])
-    for job in jobs:
-        if job.get("settings", {}).get("name") == job_name:
-            return job
-    return None
+    jobs = jobs_api.list_jobs(version=DATABRICKS_JOBS_API_VERSION, name=job_name).get("jobs", [])
+    return jobs[0] if jobs else None 
 
 
 def flatten_node(
     node: TaskGroup | BaseOperator, tasks: list[BaseOperator] = []
 ) -> list[BaseOperator]:
     """
     Flattens a node (either a TaskGroup or Operator) to a list of nodes
```

### Comparing `astro_provider_databricks-0.2.1/astro_databricks/plugins/plugin.py` & `astro_provider_databricks-0.2.2/astro_databricks/plugins/plugin.py`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.2.1/tests/conftest.py` & `astro_provider_databricks-0.2.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.2.1/tests/test_example_dags.py` & `astro_provider_databricks-0.2.2/tests/test_example_dags.py`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.2.1/tests/utils.py` & `astro_provider_databricks-0.2.2/tests/utils.py`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.2.1/tests/databricks/test_common.py` & `astro_provider_databricks-0.2.2/tests/databricks/test_common.py`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.2.1/tests/databricks/test_notebook.py` & `astro_provider_databricks-0.2.2/tests/databricks/test_notebook.py`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.2.1/tests/databricks/test_plugin.py` & `astro_provider_databricks-0.2.2/tests/databricks/test_plugin.py`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.2.1/tests/databricks/test_workflow.py` & `astro_provider_databricks-0.2.2/tests/databricks/test_workflow.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,14 +111,18 @@
     "astro_databricks.operators.workflow.RunsApi.get_run",
     return_value={"state": {"life_cycle_state": "RUNNING"}},
 )
 def test_create_workflow_from_notebooks_with_create(
     mock_run_api, mock_jobs_api, mock_api, mock_hook, dag
 ):
     mock_jobs_api.return_value.create_job.return_value = {"job_id": 1}
+    # In unittest, this function returns a MagicMock object by default, which updates an existing workflow instead of creating a new one. 
+    # This causes the create_job assertion to fail. To prevent this, the function's return value should be overridden to an empty list.
+    mock_jobs_api.return_value.list_jobs.return_value.get.return_value = [] 
+
     with dag:
         task_group = DatabricksWorkflowTaskGroup(
             group_id="test_workflow",
             databricks_conn_id="foo",
             job_clusters=[{"job_cluster_key": "foo"}],
             notebook_params={"notebook_path": "/foo/bar"},
             notebook_packages=[{"tg_index": {"package": "tg_package"}}],
@@ -387,14 +391,16 @@
     "astro_databricks.operators.workflow.RunsApi.get_run",
     return_value={"state": {"life_cycle_state": "RUNNING"}},
 )
 def test_create_workflow_from_notebooks_with_different_clusters(
     mock_run_api, mock_jobs_api, mock_api, mock_hook, dag
 ):
     mock_jobs_api.return_value.create_job.return_value = {"job_id": 1}
+    mock_jobs_api.return_value.list_jobs.return_value.get.return_value = [] 
+    
     with dag:
         task_group = DatabricksWorkflowTaskGroup(
             group_id="test_workflow",
             databricks_conn_id="foo",
             job_clusters=[{"job_cluster_key": "foo"}],
             notebook_params={"notebook_path": "/foo/bar"},
             notebook_packages=[{"tg_index": {"package": "tg_package"}}],
```

### Comparing `astro_provider_databricks-0.2.1/.gitignore` & `astro_provider_databricks-0.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.2.1/LICENSE` & `astro_provider_databricks-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.2.1/README.md` & `astro_provider_databricks-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.2.1/pyproject.toml` & `astro_provider_databricks-0.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `astro_provider_databricks-0.2.1/PKG-INFO` & `astro_provider_databricks-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: astro-provider-databricks
-Version: 0.2.1
+Version: 0.2.2
 Summary: Affordable Databricks Workflows in Apache Airflow
 Project-URL: Homepage, https://github.com/astronomer/astro-provider-databricks/
 Project-URL: Documentation, https://github.com/astronomer/astro-provider-databricks/
 Author-email: Astronomer <humans@astronomer.io>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Keywords: airflow,apache-airflow,astronomer,dags
```

