# Comparing `tmp/vertex_deployer-0.4.4.tar.gz` & `tmp/vertex_deployer-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vertex_deployer-0.4.4.tar", max compression
+gzip compressed data, was "vertex_deployer-0.5.0.tar", max compression
```

## Comparing `vertex_deployer-0.4.4.tar` & `vertex_deployer-0.5.0.tar`

### file list

```diff
@@ -1,16 +1,27 @@
--rw-r--r--   0        0        0    11357 2024-04-12 13:04:14.544625 vertex_deployer-0.4.4/LICENSE
--rw-r--r--   0        0        0    17773 2024-04-12 13:04:14.544625 vertex_deployer-0.4.4/README.md
--rw-r--r--   0        0        0       22 2024-04-12 13:04:15.680636 vertex_deployer-0.4.4/deployer/__init__.py
--rw-r--r--   0        0        0    21817 2024-04-12 13:04:14.544625 vertex_deployer-0.4.4/deployer/cli.py
--rw-r--r--   0        0        0      801 2024-04-12 13:04:14.544625 vertex_deployer-0.4.4/deployer/constants.py
--rw-r--r--   0        0        0     5957 2024-04-12 13:04:14.544625 vertex_deployer-0.4.4/deployer/pipeline_checks.py
--rw-r--r--   0        0        0    14627 2024-04-12 13:04:14.544625 vertex_deployer-0.4.4/deployer/pipeline_deployer.py
--rw-r--r--   0        0        0     5014 2024-04-12 13:04:14.544625 vertex_deployer-0.4.4/deployer/settings.py
--rw-r--r--   0        0        0     7992 2024-04-12 13:04:14.544625 vertex_deployer-0.4.4/deployer/utils/config.py
--rw-r--r--   0        0        0     1469 2024-04-12 13:04:14.544625 vertex_deployer-0.4.4/deployer/utils/console.py
--rw-r--r--   0        0        0      484 2024-04-12 13:04:14.544625 vertex_deployer-0.4.4/deployer/utils/exceptions.py
--rw-r--r--   0        0        0      604 2024-04-12 13:04:14.544625 vertex_deployer-0.4.4/deployer/utils/logging.py
--rw-r--r--   0        0        0     2015 2024-04-12 13:04:14.544625 vertex_deployer-0.4.4/deployer/utils/models.py
--rw-r--r--   0        0        0    14560 2024-04-12 13:04:14.544625 vertex_deployer-0.4.4/deployer/utils/utils.py
--rw-r--r--   0        0        0     3007 2024-04-12 13:04:15.680636 vertex_deployer-0.4.4/pyproject.toml
--rw-r--r--   0        0        0    19141 1970-01-01 00:00:00.000000 vertex_deployer-0.4.4/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-16 12:47:01.258186 vertex_deployer-0.5.0/LICENSE
+-rw-r--r--   0        0        0    17462 2024-04-16 12:47:01.258186 vertex_deployer-0.5.0/README.md
+-rw-r--r--   0        0        0       22 2024-04-16 12:47:02.286194 vertex_deployer-0.5.0/deployer/__init__.py
+-rw-r--r--   0        0        0      340 2024-04-16 12:47:01.258186 vertex_deployer-0.5.0/deployer/_templates/components/dummy_component.py.jinja
+-rw-r--r--   0        0        0       27 2024-04-16 12:47:01.258186 vertex_deployer-0.5.0/deployer/_templates/configs/json_config.json.jinja
+-rw-r--r--   0        0        0      712 2024-04-16 12:47:01.258186 vertex_deployer-0.5.0/deployer/_templates/configs/python_config.py.jinja
+-rw-r--r--   0        0        0       18 2024-04-16 12:47:01.258186 vertex_deployer-0.5.0/deployer/_templates/configs/toml_config.toml.jinja
+-rw-r--r--   0        0        0      303 2024-04-16 12:47:01.258186 vertex_deployer-0.5.0/deployer/_templates/deployer.env.jinja
+-rw-r--r--   0        0        0      624 2024-04-16 12:47:01.258186 vertex_deployer-0.5.0/deployer/_templates/deployment/Dockerfile.jinja
+-rw-r--r--   0        0        0      425 2024-04-16 12:47:01.258186 vertex_deployer-0.5.0/deployer/_templates/deployment/build_base_image.sh.jinja
+-rw-r--r--   0        0        0     1308 2024-04-16 12:47:01.258186 vertex_deployer-0.5.0/deployer/_templates/deployment/cloudbuild_local.yaml.jinja
+-rw-r--r--   0        0        0      226 2024-04-16 12:47:01.258186 vertex_deployer-0.5.0/deployer/_templates/pipelines/pipeline_minimal.py.jinja
+-rw-r--r--   0        0        0      188 2024-04-16 12:47:01.258186 vertex_deployer-0.5.0/deployer/_templates/requirements-vertex.txt.jinja
+-rw-r--r--   0        0        0    21772 2024-04-16 12:47:01.258186 vertex_deployer-0.5.0/deployer/cli.py
+-rw-r--r--   0        0        0     2425 2024-04-16 12:47:01.258186 vertex_deployer-0.5.0/deployer/constants.py
+-rw-r--r--   0        0        0     6841 2024-04-16 12:47:01.258186 vertex_deployer-0.5.0/deployer/init_deployer.py
+-rw-r--r--   0        0        0     5959 2024-04-16 12:47:01.258186 vertex_deployer-0.5.0/deployer/pipeline_checks.py
+-rw-r--r--   0        0        0    14557 2024-04-16 12:47:01.258186 vertex_deployer-0.5.0/deployer/pipeline_deployer.py
+-rw-r--r--   0        0        0     5374 2024-04-16 12:47:01.258186 vertex_deployer-0.5.0/deployer/settings.py
+-rw-r--r--   0        0        0     7983 2024-04-16 12:47:01.258186 vertex_deployer-0.5.0/deployer/utils/config.py
+-rw-r--r--   0        0        0     1639 2024-04-16 12:47:01.258186 vertex_deployer-0.5.0/deployer/utils/console.py
+-rw-r--r--   0        0        0      604 2024-04-16 12:47:01.258186 vertex_deployer-0.5.0/deployer/utils/exceptions.py
+-rw-r--r--   0        0        0      604 2024-04-16 12:47:01.258186 vertex_deployer-0.5.0/deployer/utils/logging.py
+-rw-r--r--   0        0        0     2015 2024-04-16 12:47:01.258186 vertex_deployer-0.5.0/deployer/utils/models.py
+-rw-r--r--   0        0        0    14560 2024-04-16 12:47:01.258186 vertex_deployer-0.5.0/deployer/utils/utils.py
+-rw-r--r--   0        0        0     3068 2024-04-16 12:47:02.286194 vertex_deployer-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0    18869 1970-01-01 00:00:00.000000 vertex_deployer-0.5.0/PKG-INFO
```

### Comparing `vertex_deployer-0.4.4/LICENSE` & `vertex_deployer-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vertex_deployer-0.4.4/README.md` & `vertex_deployer-0.5.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -12,24 +12,26 @@
         </p>
 </div>
 <br />
 
 <!-- PROJECT SHIELDS -->
 <div align="center">
 
-[![Python Version](https://img.shields.io/badge/Python-3.8_3.9_3.10-blue?logo=python)](#supported-python-versions)
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-[![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
-[![Linting: ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
-[![Pre-commit](https://img.shields.io/badge/pre--commit-enabled-informational?logo=pre-commit&logoColor=white)](https://github.com/ornikar/vertex-eduscore/blob/develop/.pre-commit-config.yaml)
-[![License](https://img.shields.io/github/license/artefactory/vertex-pipelines-deployer)](https://github.com/artefactory/vertex-pipelines-deployer/blob/main/LICENSE)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/vertex-deployer?logo=python)
+![PyPI - Status](https://img.shields.io/pypi/v/vertex-deployer)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/vertex-deployer?color=blue)
+![PyPI - License](https://img.shields.io/pypi/l/vertex-deployer)
 
 [![CI](https://github.com/artefactory/vertex-pipelines-deployer/actions/workflows/ci.yaml/badge.svg?branch=main&event=push)](https://github.com/artefactory/vertex-pipelines-deployer/actions/workflows/ci.yaml)
 [![Release](https://github.com/artefactory/vertex-pipelines-deployer/actions/workflows/release.yaml/badge.svg?branch=main&event=push)](https://github.com/artefactory/vertex-pipelines-deployer/actions/workflows/release.yaml)
 
+[![Pre-commit](https://img.shields.io/badge/pre--commit-enabled-informational?logo=pre-commit&logoColor=white)](https://github.com/ornikar/vertex-eduscore/blob/develop/.pre-commit-config.yaml)
+[![Linting: ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
+[![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat)](https://pycqa.github.io/isort/)
+
 </div>
 
 
 <details>
   <summary>📚 Table of Contents</summary>
   <ol>
     <li><a href="#-why-this-tool">Why this tool?</a></li>
@@ -316,15 +318,14 @@
 Let's say you defined a pipeline in `dummy_pipeline.py` and a config file named `config_test.json`. You can deploy your pipeline using the following command:
 ```bash
 vertex-deployer deploy dummy_pipeline \
     --compile \
     --upload \
     --run \
     --env-file example.env \
-    --local-package-path . \
     --tags my-tag \
     --config-filepath vertex/configs/dummy_pipeline/config_test.json \
     --experiment-name my-experiment \
     --enable-caching \
     --skip-validation
 ```
 
@@ -410,29 +411,27 @@
 ## Configuration
 
 You can configure the deployer using the `pyproject.toml` file to better fit your needs.
 This will overwrite default values. It can be useful if you always use the same options, e.g. always the same `--scheduler-timezone`
 
 ```toml
 [tool.vertex-deployer]
-pipelines_root_path = "my/path/to/vertex/pipelines"
-configs_root_path = "my/path/to/vertex/configs"
+vertex_folder_path = "my/path/to/vertex"
 log_level = "INFO"
 
 [tool.vertex-deployer.deploy]
 scheduler_timezone = "Europe/Paris"
 ```
 
 You can display all the configurable parameterss with default values by running:
 ```bash
 $ vertex-deployer config --all
 '*' means the value was set in config file
 
-* pipelines_root_path=my/path/to/vertex/pipelines
-* config_root_path=my/path/to/vertex/configs
+* vertex_folder_path=my/path/to/vertex
 * log_level=INFO
 deploy
   env_file=None
   compile=True
   upload=False
   run=False
   schedule=False
@@ -440,15 +439,14 @@
   delete_last_schedule=False
   * scheduler_timezone=Europe/Paris
   tags=['latest']
   config_filepath=None
   config_name=None
   enable_caching=False
   experiment_name=None
-  local_package_path=vertex/pipelines/compiled_pipelines
 check
   all=False
   config_filepath=None
   raise_error=False
 list
   with_configs=True
 create
```

#### html2text {}

```diff
@@ -2,32 +2,31 @@
                     ************ VVeerrtteexx PPiippeelliinneess DDeeppllooyyeerr ************
                                 _[_A_r_t_e_f_a_c_t_ _L_o_g_o_]
                ******** DDeeppllooyy VVeerrtteexx PPiippeelliinneess wwiitthhiinn mmiinnuutteess ********
  This tool is a wrapper around _k_f_p and _g_o_o_g_l_e_-_c_l_o_u_d_-_a_i_p_l_a_t_f_o_r_m that allows you
 to check, compile, upload, run, and schedule Vertex Pipelines in a standardized
                                     manner.
 
-     [![Python Version](https://img.shields.io/badge/Python-3.8_3.9_3.10-
- blue?logo=python)](#supported-python-versions) [![Code style: black](https://
- img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/
-   black) [![Imports: isort](https://img.shields.io/badge/%20imports-isort-
-  %231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/) [!
-         [Linting: ruff](https://img.shields.io/endpoint?url=https://
-raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json)](https:
-//github.com/astral-sh/ruff) [![Pre-commit](https://img.shields.io/badge/pre--
-    commit-enabled-informational?logo=pre-commit&logoColor=white)](https://
-  github.com/ornikar/vertex-eduscore/blob/develop/.pre-commit-config.yaml) [!
- [License](https://img.shields.io/github/license/artefactory/vertex-pipelines-
-deployer)](https://github.com/artefactory/vertex-pipelines-deployer/blob/main/
-   LICENSE) [![CI](https://github.com/artefactory/vertex-pipelines-deployer/
+    ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/vertex-
+ deployer?logo=python) ![PyPI - Status](https://img.shields.io/pypi/v/vertex-
+     deployer) ![PyPI - Downloads](https://img.shields.io/pypi/dm/vertex-
+ deployer?color=blue) ![PyPI - License](https://img.shields.io/pypi/l/vertex-
+  deployer) [![CI](https://github.com/artefactory/vertex-pipelines-deployer/
      actions/workflows/ci.yaml/badge.svg?branch=main&event=push)](https://
 github.com/artefactory/vertex-pipelines-deployer/actions/workflows/ci.yaml) [!
   [Release](https://github.com/artefactory/vertex-pipelines-deployer/actions/
  workflows/release.yaml/badge.svg?branch=main&event=push)](https://github.com/
-     artefactory/vertex-pipelines-deployer/actions/workflows/release.yaml)
+ artefactory/vertex-pipelines-deployer/actions/workflows/release.yaml) [![Pre-
+           commit](https://img.shields.io/badge/pre--commit-enabled-
+  informational?logo=pre-commit&logoColor=white)](https://github.com/ornikar/
+vertex-eduscore/blob/develop/.pre-commit-config.yaml) [![Linting: ruff](https:/
+ /img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/
+ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff) [![Imports:
+  isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat)]
+                       (https://pycqa.github.io/isort/)
 ð Table of Contents
    1. _W_h_y_ _t_h_i_s_ _t_o_o_l_?
    2. _P_r_e_r_e_q_u_i_s_i_t_e_s
    3. _I_n_s_t_a_l_l_a_t_i_o_n
          1. _F_r_o_m_ _g_i_t_ _r_e_p_o
          2. _F_r_o_m_ _A_r_t_i_f_a_c_t_ _R_e_g_i_s_t_r_y_ _(_n_o_t_ _a_v_a_i_l_a_b_l_e_ _i_n_ _P_y_P_I_ _y_e_t_)
          3. _A_d_d_ _t_o_ _r_e_q_u_i_r_e_m_e_n_t_s
@@ -148,70 +147,68 @@
 provided to ensure that you don't accidentally deploy to the wrong project. An
 [`example.env`](./example/example.env) file is provided in this repo. This also
 allows you to work with multiple environments thanks to env files (`test.env`,
 `dev.env`, `prod.env`, etc) ### ð CLI: Deploying a Pipeline with `deploy`
 Let's say you defined a pipeline in `dummy_pipeline.py` and a config file named
 `config_test.json`. You can deploy your pipeline using the following command:
 ```bash vertex-deployer deploy dummy_pipeline \ --compile \ --upload \ --run \
---env-file example.env \ --local-package-path . \ --tags my-tag \ --config-
-filepath vertex/configs/dummy_pipeline/config_test.json \ --experiment-name my-
-experiment \ --enable-caching \ --skip-validation ``` ### â CLI: Checking
-Pipelines are valid with `check` To check that your pipelines are valid, you
-can use the `check` command. It uses a pydantic model to: - check that your
-pipeline imports and definition are valid - check that your pipeline can be
-compiled - check that all configs related to the pipeline are respecting the
-pipeline definition (using a Pydantic model based on pipeline signature) To
-validate one or multiple pipeline(s): ```bash vertex-deployer check
-dummy_pipeline ``` To validate all pipelines in the `vertex/pipelines` folder:
-```bash vertex-deployer check --all ``` ### ð ï¸ CLI: Other commands ####
-`config` You can check your `vertex-deployer` configuration options using the
-`config` command. Fields set in `pyproject.toml` will overwrite default values
-and will be displayed differently: ```bash vertex-deployer config --all ```
-#### `create` You can create all files needed for a pipeline using the `create`
-command: ```bash vertex-deployer create my_new_pipeline --config-type py ```
-This will create a `my_new_pipeline.py` file in the `vertex/pipelines` folder
-and a `vertex/config/my_new_pipeline/` folder with multiple config files in it.
-#### `init` To initialize the deployer with default settings and folder
-structure, use the `init` command: ```bash vertex-deployer init ``` ```bash $
-vertex-deployer init Welcome to Vertex Deployer! This command will help you
-getting fired up. Do you want to configure the deployer? [y/n]: n Do you want
-to build default folder structure [y/n]: n Do you want to create a pipeline?
-[y/n]: n All done â¨ ``` #### `list` You can list all pipelines in the
-`vertex/pipelines` folder using the `list` command: ```bash vertex-deployer
-list --with-configs ``` ### ð­ CLI: Options ```bash vertex-deployer --help
-``` To see package version: ```bash vertex-deployer --version ``` To adapt log
-level, use the `--log-level` option. Default is `INFO`. ```bash vertex-deployer
---log-level DEBUG deploy ... ``` ## Configuration You can configure the
-deployer using the `pyproject.toml` file to better fit your needs. This will
-overwrite default values. It can be useful if you always use the same options,
-e.g. always the same `--scheduler-timezone` ```toml [tool.vertex-deployer]
-pipelines_root_path = "my/path/to/vertex/pipelines" configs_root_path = "my/
-path/to/vertex/configs" log_level = "INFO" [tool.vertex-deployer.deploy]
-scheduler_timezone = "Europe/Paris" ``` You can display all the configurable
-parameterss with default values by running: ```bash $ vertex-deployer config --
-all '*' means the value was set in config file * pipelines_root_path=my/path/
-to/vertex/pipelines * config_root_path=my/path/to/vertex/configs *
-log_level=INFO deploy env_file=None compile=True upload=False run=False
-schedule=False cron=None delete_last_schedule=False *
-scheduler_timezone=Europe/Paris tags=['latest'] config_filepath=None
-config_name=None enable_caching=False experiment_name=None
-local_package_path=vertex/pipelines/compiled_pipelines check all=False
-config_filepath=None raise_error=False list with_configs=True create
-config_type=json ``` ## Repository Structure ``` ââ .github â ââ
-ISSUE_TEMPLATE/ â ââ workflows â â ââ ci.yaml â â ââ
-pr_agent.yaml â â ââ release.yaml â ââ CODEOWNERS â ââ
-PULL_REQUEST_TEMPLATE.md ââ deployer # Source code â ââ __init__.py
-â ââ cli.py â ââ constants.py â ââ pipeline_checks.py â
-ââ pipeline_deployer.py â ââ settings.py â ââ utils â ââ
-config.py â ââ console.py â ââ exceptions.py â ââ logging.py
-â ââ models.py â ââ utils.py ââ docs/ # Documentation folder
-(mkdocs) ââ templates/ # Semantic Release templates ââ tests/ ââ
-example # Example folder with dummy pipeline and config | ââ example.env
-â ââ vertex â ââ components â â ââ dummy.py â ââ
-configs â â ââ broken_pipeline â â â ââ config_test.json â
-â ââ dummy_pipeline â â ââ config_test.json â â ââ
-config.py â â ââ config.toml â ââ deployment â ââ lib â
-ââ pipelines â ââ broken_pipeline.py â ââ dummy_pipeline.py
-ââ .gitignore ââ .pre-commit-config.yaml ââ catalog-info.yaml #
-Roadie integration configuration ââ CHANGELOG.md ââ CONTRIBUTING.md
-ââ LICENSE ââ Makefile ââ mkdocs.yml # Mkdocs configuration ââ
-pyproject.toml ââ README.md ```
+--env-file example.env \ --tags my-tag \ --config-filepath vertex/configs/
+dummy_pipeline/config_test.json \ --experiment-name my-experiment \ --enable-
+caching \ --skip-validation ``` ### â CLI: Checking Pipelines are valid with
+`check` To check that your pipelines are valid, you can use the `check`
+command. It uses a pydantic model to: - check that your pipeline imports and
+definition are valid - check that your pipeline can be compiled - check that
+all configs related to the pipeline are respecting the pipeline definition
+(using a Pydantic model based on pipeline signature) To validate one or
+multiple pipeline(s): ```bash vertex-deployer check dummy_pipeline ``` To
+validate all pipelines in the `vertex/pipelines` folder: ```bash vertex-
+deployer check --all ``` ### ð ï¸ CLI: Other commands #### `config` You can
+check your `vertex-deployer` configuration options using the `config` command.
+Fields set in `pyproject.toml` will overwrite default values and will be
+displayed differently: ```bash vertex-deployer config --all ``` #### `create`
+You can create all files needed for a pipeline using the `create` command:
+```bash vertex-deployer create my_new_pipeline --config-type py ``` This will
+create a `my_new_pipeline.py` file in the `vertex/pipelines` folder and a
+`vertex/config/my_new_pipeline/` folder with multiple config files in it. ####
+`init` To initialize the deployer with default settings and folder structure,
+use the `init` command: ```bash vertex-deployer init ``` ```bash $ vertex-
+deployer init Welcome to Vertex Deployer! This command will help you getting
+fired up. Do you want to configure the deployer? [y/n]: n Do you want to build
+default folder structure [y/n]: n Do you want to create a pipeline? [y/n]: n
+All done â¨ ``` #### `list` You can list all pipelines in the `vertex/
+pipelines` folder using the `list` command: ```bash vertex-deployer list --
+with-configs ``` ### ð­ CLI: Options ```bash vertex-deployer --help ``` To
+see package version: ```bash vertex-deployer --version ``` To adapt log level,
+use the `--log-level` option. Default is `INFO`. ```bash vertex-deployer --log-
+level DEBUG deploy ... ``` ## Configuration You can configure the deployer
+using the `pyproject.toml` file to better fit your needs. This will overwrite
+default values. It can be useful if you always use the same options, e.g.
+always the same `--scheduler-timezone` ```toml [tool.vertex-deployer]
+vertex_folder_path = "my/path/to/vertex" log_level = "INFO" [tool.vertex-
+deployer.deploy] scheduler_timezone = "Europe/Paris" ``` You can display all
+the configurable parameterss with default values by running: ```bash $ vertex-
+deployer config --all '*' means the value was set in config file *
+vertex_folder_path=my/path/to/vertex * log_level=INFO deploy env_file=None
+compile=True upload=False run=False schedule=False cron=None
+delete_last_schedule=False * scheduler_timezone=Europe/Paris tags=['latest']
+config_filepath=None config_name=None enable_caching=False experiment_name=None
+check all=False config_filepath=None raise_error=False list with_configs=True
+create config_type=json ``` ## Repository Structure ``` ââ .github â
+ââ ISSUE_TEMPLATE/ â ââ workflows â â ââ ci.yaml â â
+ââ pr_agent.yaml â â ââ release.yaml â ââ CODEOWNERS â
+ââ PULL_REQUEST_TEMPLATE.md ââ deployer # Source code â ââ
+__init__.py â ââ cli.py â ââ constants.py â ââ
+pipeline_checks.py â ââ pipeline_deployer.py â ââ settings.py â
+ââ utils â ââ config.py â ââ console.py â ââ
+exceptions.py â ââ logging.py â ââ models.py â ââ utils.py
+ââ docs/ # Documentation folder (mkdocs) ââ templates/ # Semantic
+Release templates ââ tests/ ââ example # Example folder with dummy
+pipeline and config | ââ example.env â ââ vertex â ââ
+components â â ââ dummy.py â ââ configs â â ââ
+broken_pipeline â â â ââ config_test.json â â ââ
+dummy_pipeline â â ââ config_test.json â â ââ config.py â â
+ââ config.toml â ââ deployment â ââ lib â ââ pipelines
+â ââ broken_pipeline.py â ââ dummy_pipeline.py ââ .gitignore
+ââ .pre-commit-config.yaml ââ catalog-info.yaml # Roadie integration
+configuration ââ CHANGELOG.md ââ CONTRIBUTING.md ââ LICENSE ââ
+Makefile ââ mkdocs.yml # Mkdocs configuration ââ pyproject.toml ââ
+README.md ```
```

### Comparing `vertex_deployer-0.4.4/deployer/cli.py` & `vertex_deployer-0.5.0/deployer/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,29 +8,33 @@
 import typer
 from loguru import logger
 from pydantic import ValidationError
 from rich.prompt import Confirm, Prompt
 from typing_extensions import Annotated
 
 from deployer import constants
+from deployer.init_deployer import (
+    _create_file_from_template,
+    build_default_folder_structure,
+    configure_deployer,
+    ensure_pyproject_toml,
+    show_commands,
+)
 from deployer.settings import (
     DeployerSettings,
-    find_pyproject_toml,
     load_deployer_settings,
-    update_pyproject_toml,
 )
 from deployer.utils.config import (
     ConfigType,
-    VertexPipelinesSettings,
     list_config_filepaths,
     load_config,
     load_vertex_settings,
     validate_or_log_settings,
 )
-from deployer.utils.console import ask_user_for_model_fields, console
+from deployer.utils.console import console
 from deployer.utils.logging import LoguruLevel
 from deployer.utils.utils import (
     dict_to_repr,
     import_pipeline_from_dir,
     make_enum_from_python_package_dir,
     print_check_results_table,
     print_pipelines_list,
@@ -219,25 +223,14 @@
         typer.Option(
             "--experiment-name",
             "-en",
             help="The name of the experiment to run the pipeline in."
             "Defaults to '{pipeline_name}-experiment'.",
         ),
     ] = None,
-    local_package_path: Annotated[
-        Path,
-        typer.Option(
-            "--local-package-path",
-            "-lpp",
-            help="Local dir path where pipelines will be compiled.",
-            dir_okay=True,
-            file_okay=False,
-            resolve_path=True,
-        ),
-    ] = constants.DEFAULT_LOCAL_PACKAGE_PATH,
     skip_validation: Annotated[
         bool,
         typer.Option(
             "--skip-validation / --no-skip",
             "-y / -n",
             help="Whether to continue without user validation of the settings.",
         ),
@@ -282,21 +275,21 @@
             region=vertex_settings.GCP_REGION,
             staging_bucket_name=vertex_settings.VERTEX_STAGING_BUCKET_NAME,
             service_account=vertex_settings.VERTEX_SERVICE_ACCOUNT,
             pipeline_name=pipeline_name,
             pipeline_func=pipeline_func,
             gar_location=vertex_settings.GAR_LOCATION,
             gar_repo_id=vertex_settings.GAR_PIPELINES_REPO_ID,
-            local_package_path=local_package_path,
+            local_package_path=deployer_settings.local_package_path,
         )
 
         if run or schedule:
             if config_name is not None:
                 config_filepath = (
-                    Path(deployer_settings.config_root_path) / pipeline_name / config_name
+                    Path(deployer_settings.configs_root_path) / pipeline_name / config_name
                 )
             parameter_values, input_artifacts = load_config(config_filepath)
 
         if compile:
             with console.status("Compiling pipeline..."):
                 deployer.compile()
 
@@ -384,15 +377,15 @@
     Checking that a pipeline is valid includes:
 
     * Checking that the pipeline can be imported. It must be a valid python module with a
     `{pipeline_name}` function decorated with `@kfp.dsl.pipeline`.
 
     * Checking that the pipeline can be compiled using `kfp.compiler.Compiler`.
 
-    * Checking that config files in `{config_root_path}/{pipeline_name}` are corresponding to the
+    * Checking that config files in `{configs_root_path}/{pipeline_name}` are corresponding to the
     pipeline parameters definition, using Pydantic.
 
     ---
 
     **This command can be used to check pipelines in a Continuous Integration workflow.**
     """
     if all and pipeline_names:
@@ -405,29 +398,30 @@
     if all:
         # unpack enum to get list of pipeline names
         pipeline_names = [x.value for x in ctx.obj["pipeline_names"]]
     logger.info(f"Checking pipelines {pipeline_names}")
 
     if config_filepath is None:
         to_check = {
-            p: list_config_filepaths(deployer_settings.config_root_path, p) for p in pipeline_names
+            p: list_config_filepaths(deployer_settings.configs_root_path, p)
+            for p in pipeline_names
         }
     else:
         to_check = {p: [config_filepath] for p in pipeline_names}
 
     try:
         with console.status("Checking pipelines..."):
             pipelines_model = Pipelines.model_validate(
                 {
                     "pipelines": {
                         p: {
                             "pipeline_name": p,
                             "config_paths": config_filepaths,
                             "pipelines_root_path": deployer_settings.pipelines_root_path,
-                            "config_root_path": deployer_settings.config_root_path,
+                            "configs_root_path": deployer_settings.configs_root_path,
                         }
                         for p, config_filepaths in to_check.items()
                     }
                 },
                 context={"raise_for_defaults": raise_for_defaults},
             )
     except ValidationError as e:
@@ -450,15 +444,15 @@
             "--with-configs / --no-configs", "-wc / -nc ", help="Whether to list config files."
         ),
     ] = False,
 ):
     """List all pipelines."""
     if with_configs:
         pipelines_dict = {
-            p.name: list_config_filepaths(ctx.obj["settings"].config_root_path, p.name)
+            p.name: list_config_filepaths(ctx.obj["settings"].configs_root_path, p.name)
             for p in ctx.obj["pipeline_names"].__members__.values()
         }
     else:
         pipelines_dict = {p.name: [] for p in ctx.obj["pipeline_names"].__members__.values()}
 
     print_pipelines_list(pipelines_dict, with_configs)
 
@@ -469,27 +463,27 @@
     pipeline_names: Annotated[
         List[str],
         typer.Argument(..., help="The names of the pipeline to create."),
     ],
     config_type: Annotated[
         ConfigType,
         typer.Option("--config-type", "-ct", help="The type of the config to create."),
-    ] = ConfigType.json,
+    ] = ConfigType.py,
 ):
     """Create files structure for a new pipeline."""
     invalid_pipelines = [p for p in pipeline_names if not re.match(r"^[a-zA-Z0-9_]+$", p)]
     if invalid_pipelines:
         raise typer.BadParameter(
             f"Invalid Pipeline name(s): '{invalid_pipelines}'\n"
             "Pipeline name must only contain alphanumeric characters and underscores"
         )
 
     deployer_settings: DeployerSettings = ctx.obj["settings"]
 
-    for path in [deployer_settings.pipelines_root_path, deployer_settings.config_root_path]:
+    for path in [deployer_settings.pipelines_root_path, deployer_settings.configs_root_path]:
         if not Path(path).is_dir():
             raise FileNotFoundError(
                 f"Path '{path}' does not exist."
                 " Please check that the root path is correct"
                 f" or create it with 'mkdir -p {path}'."
             )
 
@@ -501,102 +495,104 @@
 
     console.print(
         f"Creating pipeline {pipeline_names} with config type: [bold]{config_type}[/bold]"
     )
 
     for pipeline_name in pipeline_names:
         pipeline_filepath = deployer_settings.pipelines_root_path / f"{pipeline_name}.py"
-        pipeline_filepath.touch(exist_ok=False)
-        pipeline_filepath.write_text(
-            constants.PIPELINE_MINIMAL_TEMPLATE.format(pipeline_name=pipeline_name)
+        _create_file_from_template(
+            path=pipeline_filepath,
+            template_path=constants.PIPELINE_MINIMAL_TEMPLATE,
+            pipeline_name=pipeline_name,
+            component_module=str(deployer_settings.vertex_folder_path / "components").replace(
+                "/", "."
+            ),
         )
 
         try:
-            config_dirpath = Path(deployer_settings.config_root_path) / pipeline_name
+            config_dirpath = Path(deployer_settings.configs_root_path) / pipeline_name
             config_dirpath.mkdir(exist_ok=True)
             for config_name in ["test", "dev", "prod"]:
                 config_filepath = config_dirpath / f"{config_name}.{config_type}"
-                config_filepath.touch(exist_ok=False)
-                if config_type == ConfigType.py:
-                    config_filepath.write_text(constants.PYTHON_CONFIG_TEMPLATE)
+                config_template = constants.CONFIG_TEMPLATE_MAPPING[config_type]
+                _create_file_from_template(
+                    path=config_filepath,
+                    template_path=config_template,
+                )
+
         except Exception as e:
             pipeline_filepath.unlink()
             raise e
 
         console.print(
-            f"Pipeline '{pipeline_name}' created at '{pipeline_filepath}'"
-            f" with config files: {[str(p) for p in config_dirpath.glob('*')]}. :sparkles:",
+            f"\n Pipeline '{pipeline_name}' created at '{pipeline_filepath}'"
+            f"\n with config files: {[str(p) for p in config_dirpath.glob('*')]}. :sparkles: \n",
             style="blue",
         )
 
 
 @app.command(name="init")
-def init_deployer(ctx: typer.Context):  # noqa: C901
-    deployer_settings: DeployerSettings = ctx.obj["settings"]
-
-    console.print("Welcome to Vertex Deployer!", style="blue")
-    console.print("This command will help you getting fired up.", style="blue")
-
-    if Confirm.ask("Do you want to configure the deployer?"):
-        pyproject_toml_filepath = find_pyproject_toml(Path.cwd().resolve())
-
-        if pyproject_toml_filepath is None:
-            console.print(
-                "No pyproject.toml file found. Creating one in current directory.",
-                style="yellow",
-            )
-            pyproject_toml_filepath = Path("./pyproject.toml")
-            pyproject_toml_filepath.touch()
-
-        set_fields = ask_user_for_model_fields(DeployerSettings)
-
-        new_deployer_settings = DeployerSettings(**set_fields)
-
-        update_pyproject_toml(pyproject_toml_filepath, new_deployer_settings)
-        console.print("Configuration saved in pyproject.toml :sparkles:", style="blue")
-
-    if Confirm.ask("Do you want to build default folder structure"):
+def init_deployer(
+    ctx: typer.Context,
+    default: bool = typer.Option(
+        False,
+        "--default",
+        "-d",
+        help="Instantly creates the full vertex structure and files without configuration prompts",
+    ),
+):
+    """Initialize the deployer."""
+    deployer_settings = ctx.obj["settings"]
+    console.print("Welcome to Vertex Deployer!", style="bold blue")
+
+    if default or Confirm.ask(
+        "Do you want to instantly create the full vertex structure and templates\n"
+        "without configuration prompts? This will use the default settings."
+    ):
+        console.print("Performing quick initialization...", style="bold blue")
+        ensure_pyproject_toml()
+        deployer_settings = load_deployer_settings()
+        build_default_folder_structure(deployer_settings)
+        create_pipeline(ctx, pipeline_names=["dummy_pipeline"], config_type=ConfigType.py)
+
+        console.print("Default initialization done :sparkles:\n", style="bold blue")
+        console.print("Here are some commands on how to use the deployer:", style="blue")
+        show_commands(deployer_settings)
+    else:
+        console.print("This command will help you getting fired up! :fire:\n", style="blue")
 
-        def create_file_or_dir(path: Path, text: str = ""):
-            """Create a file (if text is provided) or a directory at path. Warn if path exists."""
-            if path.exists():
-                console.print(
-                    f"Path '{path}' already exists. Skipping creation of path.", style="yellow"
-                )
-            else:
-                if text:
-                    path.touch()
-                    path.write_text(text)
+        if Confirm.ask("Do you want to configure the deployer?"):
+            deployer_settings = configure_deployer()
+            ctx.obj["settings"] = deployer_settings
+
+        if Confirm.ask("Do you want to build default folder structure"):
+            build_default_folder_structure(deployer_settings)
+
+        if Confirm.ask("Do you want to create a pipeline?"):
+            wrong_name = True
+            while wrong_name:
+                pipeline_name = Prompt.ask("What is the name of the pipeline?")
+
+                try:
+                    config_type = deployer_settings.create.config_type.name
+                    create_pipeline(ctx, pipeline_names=[pipeline_name], config_type=config_type)
+                except typer.BadParameter as e:
+                    console.print(e, style="red")
+                except FileExistsError:
+                    console.print(
+                        f"Pipeline '{pipeline_name}' already exists. Skipping creation.",
+                        style="yellow",
+                    )
                 else:
-                    path.mkdir(parents=True)
+                    wrong_name = False
 
-        create_file_or_dir(deployer_settings.pipelines_root_path)
-        create_file_or_dir(deployer_settings.config_root_path)
-        create_file_or_dir(
-            Path("./.env"), "=\n".join(VertexPipelinesSettings.model_json_schema()["required"])
-        )
-
-    if Confirm.ask("Do you want to create a pipeline?"):
-        wrong_name = True
-        while wrong_name:
-            pipeline_name = Prompt.ask("What is the name of the pipeline?")
-
-            try:
-                create_pipeline(ctx, pipeline_names=[pipeline_name])
-            except typer.BadParameter as e:
-                console.print(e, style="red")
-            except FileExistsError:
-                console.print(
-                    f"Pipeline '{pipeline_name}' already exists. Skipping creation.",
-                    style="yellow",
-                )
-            else:
-                wrong_name = False
+            console.print("All done :sparkles:\n", style="bold blue")
 
-    console.print("All done :sparkles:", style="blue")
+            if Confirm.ask("Do you want to see some instructions on how to use the deployer"):
+                show_commands(deployer_settings)
 
 
 @app.command(name="config")
 def list_deployer_settings(
     ctx: typer.Context,
     all: Annotated[
         bool, typer.Option("--all", "-a", help="Whether to display all configuration values.")
```

### Comparing `vertex_deployer-0.4.4/deployer/pipeline_checks.py` & `vertex_deployer-0.5.0/deployer/pipeline_checks.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,24 +53,24 @@
 
 class Pipeline(CustomBaseModel):
     """Validation of one pipeline and its configs"""
 
     pipeline_name: str
     config_paths: Annotated[List[Path], Field(validate_default=True)] = None
     pipelines_root_path: Path
-    config_root_path: Path
+    configs_root_path: Path
     configs: Optional[Dict[str, ConfigDynamicModel]] = None  # Optional because populated after
 
     @model_validator(mode="before")
     @classmethod
     def populate_config_names(cls, data: Any) -> Any:
         """Populate config names before validation"""
         if data.get("config_paths") is None:
             data["config_paths"] = list_config_filepaths(
-                str(data["config_root_path"]), data["pipeline_name"]
+                str(data["configs_root_path"]), data["pipeline_name"]
             )
         return data
 
     @computed_field
     @property
     def pipeline(self) -> graph_component.GraphComponent:
         """Import pipeline"""
```

### Comparing `vertex_deployer-0.4.4/deployer/pipeline_deployer.py` & `vertex_deployer-0.5.0/deployer/pipeline_deployer.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 from google.cloud import aiplatform
 from google.cloud.aiplatform import PipelineJobSchedule
 from kfp import compiler
 from kfp.registry import RegistryClient
 from loguru import logger
 from requests import HTTPError
 
-from deployer.constants import DEFAULT_LOCAL_PACKAGE_PATH
 from deployer.utils.exceptions import (
     MissingGoogleArtifactRegistryHostError,
     TagNotFoundError,
 )
 
 
 class VertexPipelineDeployer:
@@ -27,15 +26,15 @@
         pipeline_func: Callable,
         project_id: Optional[str] = None,
         region: Optional[str] = None,
         staging_bucket_name: Optional[str] = None,
         service_account: Optional[str] = None,
         gar_location: Optional[str] = None,
         gar_repo_id: Optional[str] = None,
-        local_package_path: Path = DEFAULT_LOCAL_PACKAGE_PATH,
+        local_package_path: Optional[Path] = None,
     ) -> None:
         """I don't want to write a dostring here but ruff wants me to"""
         self.project_id = project_id
         self.region = region
         self.staging_bucket_name = staging_bucket_name
         self.service_account = service_account
```

### Comparing `vertex_deployer-0.4.4/deployer/settings.py` & `vertex_deployer-0.5.0/deployer/settings.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,15 +26,14 @@
     delete_last_schedule: bool = False
     scheduler_timezone: str = constants.DEFAULT_SCHEDULER_TIMEZONE
     tags: Optional[List[str]] = constants.DEFAULT_TAGS
     config_filepath: Optional[Path] = None
     config_name: Optional[str] = None
     enable_caching: Optional[bool] = None
     experiment_name: Optional[str] = None
-    local_package_path: Path = constants.DEFAULT_LOCAL_PACKAGE_PATH
     skip_validation: bool = True
 
 
 class _DeployerCheckSettings(CustomBaseModel):
     """Settings for Vertex Deployer `check` command."""
 
     all: bool = False
@@ -49,35 +48,49 @@
 
     with_configs: bool = False
 
 
 class _DeployerCreateSettings(CustomBaseModel):
     """Settings for Vertex Deployer `create` command."""
 
-    config_type: ConfigType = ConfigType.json
+    config_type: ConfigType = ConfigType.py
 
 
 class _DeployerConfigSettings(CustomBaseModel):
     """Settings for Vertex Deployer `config` command."""
 
     all: bool = False
 
 
 class DeployerSettings(CustomBaseModel):
     """Settings for Vertex Deployer."""
 
-    pipelines_root_path: Path = constants.DEFAULT_PIPELINE_ROOT_PATH
-    config_root_path: Path = constants.DEFAULT_CONFIG_ROOT_PATH
+    vertex_folder_path: Path = constants.DEFAULT_VERTEX_FOLDER_PATH
     log_level: str = "INFO"
     deploy: _DeployerDeploySettings = _DeployerDeploySettings()
     check: _DeployerCheckSettings = _DeployerCheckSettings()
     list: _DeployerListSettings = _DeployerListSettings()
     create: _DeployerCreateSettings = _DeployerCreateSettings()
     config: _DeployerConfigSettings = _DeployerConfigSettings()
 
+    @property
+    def pipelines_root_path(self) -> Path:
+        """Construct the pipelines root path."""
+        return self.vertex_folder_path / "pipelines"
+
+    @property
+    def configs_root_path(self) -> Path:
+        """Construct the configs root path."""
+        return self.vertex_folder_path / "configs"
+
+    @property
+    def local_package_path(self) -> Path:
+        """Construct the local package path."""
+        return self.vertex_folder_path / "pipelines" / "compiled_pipelines"
+
 
 def find_pyproject_toml(path_project_root: Path) -> Optional[str]:
     """Find the pyproject.toml file."""
     path_pyproject_toml = path_project_root / "pyproject.toml"
     if path_pyproject_toml.is_file():
         if path_pyproject_toml.exists():
             return str(path_pyproject_toml)
```

### Comparing `vertex_deployer-0.4.4/deployer/utils/config.py` & `vertex_deployer-0.5.0/deployer/utils/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,25 +81,25 @@
 
 class ConfigType(str, Enum):  # noqa: D101
     json = "json"
     py = "py"
     toml = "toml"
 
 
-def list_config_filepaths(config_root_path: Union[Path, str], pipeline_name: str) -> List[Path]:
+def list_config_filepaths(configs_root_path: Path, pipeline_name: str) -> List[Path]:
     """List the config filepaths for a pipeline.
 
     Args:
-        config_root_path (Path): A `Path` object representing the root path of the configs.
+        configs_root_path (Path): A `Path` object representing the root path of the configs.
         pipeline_name (str): The name of the pipeline.
 
     Returns:
         List[Path]: A list of `Path` objects representing the config filepaths.
     """
-    configs_dirpath = Path(config_root_path) / pipeline_name
+    configs_dirpath = Path(configs_root_path) / pipeline_name
     config_filepaths = [
         x
         for config_type in ConfigType.__members__.values()
         for x in configs_dirpath.glob(f"*.{config_type}")
     ]
     return config_filepaths
```

### Comparing `vertex_deployer-0.4.4/deployer/utils/console.py` & `vertex_deployer-0.5.0/deployer/utils/console.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     Args:
         model (Type[BaseModel]): The pydantic model to configure.
 
     Returns:
         dict: A dictionary of the set fields.
     """
     set_fields = {}
+
     for field_name, field_info in model.model_fields.items():
         if isclass(field_info.annotation) and issubclass(field_info.annotation, BaseModel):
             answer = Confirm.ask(f"Do you want to configure command {field_name}?", default=False)
             if answer:
                 set_fields[field_name] = ask_user_for_model_fields(field_info.annotation)
 
         else:
@@ -32,13 +33,17 @@
 
             if isclass(annotation) and issubclass(annotation, Enum):
                 choices = list(annotation.__members__)
 
             if isclass(annotation) and annotation == bool:
                 answer = Confirm.ask(field_name, default=default)
             else:
-                answer = Prompt.ask(field_name, default=default, choices=choices)
-
-            if answer != field_info.default:
+                answer = Prompt.ask(
+                    field_name, default=default if default is not None else "None", choices=choices
+                )
+
+            if answer != field_info.default and not (
+                answer in [None, "None"] and field_info.default is None
+            ):
                 set_fields[field_name] = answer
 
     return set_fields
```

### Comparing `vertex_deployer-0.4.4/deployer/utils/logging.py` & `vertex_deployer-0.5.0/deployer/utils/logging.py`

 * *Files identical despite different names*

### Comparing `vertex_deployer-0.4.4/deployer/utils/models.py` & `vertex_deployer-0.5.0/deployer/utils/models.py`

 * *Files identical despite different names*

### Comparing `vertex_deployer-0.4.4/deployer/utils/utils.py` & `vertex_deployer-0.5.0/deployer/utils/utils.py`

 * *Files identical despite different names*

### Comparing `vertex_deployer-0.4.4/pyproject.toml` & `vertex_deployer-0.5.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "vertex-deployer"
-version = "0.4.4"
+version = "0.5.0"
 description = "Check, compile, upload, run, and schedule Kubeflow Pipelines on GCP Vertex AI in a standardized manner."
 authors = [
     "artefactory <jules.bertrand@artefact.com>",
     "julesbertrand  <jules.bertrand@artefact.com>"
 ]
 license = "Apache-2.0"
 homepage = "https://github.com/artefactory/vertex-pipelines-deployer"
@@ -26,14 +26,15 @@
 rich = "^13.5"
 loguru = "^0.7"
 pydantic-settings = "^2.0"
 pydantic = "^2.3"
 pyinstrument = { version = "^4.5", optional = true }
 toml = "^0.10"
 tomlkit = "^0.12"
+jinja2 = "^3.1.3"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.0"
 pre-commit = "^3.3"
 ipykernel = "^6.9"
 nbstripout = "^0.7"
 ruff = "^0.3"
@@ -50,14 +51,17 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.ruff]
 target-version = "py38"
 line-length = 99
+exclude = [
+    "deployer/_templates/*",
+]
 
 [tool.ruff.lint]
 ignore = [
     "D100",
     "D205",
     "D415",
 ]
```

### Comparing `vertex_deployer-0.4.4/PKG-INFO` & `vertex_deployer-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: vertex-deployer
-Version: 0.4.4
+Version: 0.5.0
 Summary: Check, compile, upload, run, and schedule Kubeflow Pipelines on GCP Vertex AI in a standardized manner.
 Home-page: https://github.com/artefactory/vertex-pipelines-deployer
 License: Apache-2.0
 Keywords: kubeflow,vertexai,aiplatform,gcp,mlops,deployer,pipeline
 Author: artefactory
 Author-email: jules.bertrand@artefact.com
 Requires-Python: >=3.8,<3.11.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Provides-Extra: profiling
 Requires-Dist: google-cloud-aiplatform (>=1.26,<2.0)
+Requires-Dist: jinja2 (>=3.1.3,<4.0.0)
 Requires-Dist: kfp (>=2.0.1,<3.0)
 Requires-Dist: loguru (>=0.7,<0.8)
 Requires-Dist: pydantic (>=2.3,<3.0)
 Requires-Dist: pydantic-settings (>=2.0,<3.0)
 Requires-Dist: pyinstrument (>=4.5,<5.0) ; extra == "profiling"
 Requires-Dist: requests (>=2.31,<3.0)
 Requires-Dist: rich (>=13.5,<14.0)
@@ -43,24 +44,26 @@
         </p>
 </div>
 <br />
 
 <!-- PROJECT SHIELDS -->
 <div align="center">
 
-[![Python Version](https://img.shields.io/badge/Python-3.8_3.9_3.10-blue?logo=python)](#supported-python-versions)
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-[![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
-[![Linting: ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
-[![Pre-commit](https://img.shields.io/badge/pre--commit-enabled-informational?logo=pre-commit&logoColor=white)](https://github.com/ornikar/vertex-eduscore/blob/develop/.pre-commit-config.yaml)
-[![License](https://img.shields.io/github/license/artefactory/vertex-pipelines-deployer)](https://github.com/artefactory/vertex-pipelines-deployer/blob/main/LICENSE)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/vertex-deployer?logo=python)
+![PyPI - Status](https://img.shields.io/pypi/v/vertex-deployer)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/vertex-deployer?color=blue)
+![PyPI - License](https://img.shields.io/pypi/l/vertex-deployer)
 
 [![CI](https://github.com/artefactory/vertex-pipelines-deployer/actions/workflows/ci.yaml/badge.svg?branch=main&event=push)](https://github.com/artefactory/vertex-pipelines-deployer/actions/workflows/ci.yaml)
 [![Release](https://github.com/artefactory/vertex-pipelines-deployer/actions/workflows/release.yaml/badge.svg?branch=main&event=push)](https://github.com/artefactory/vertex-pipelines-deployer/actions/workflows/release.yaml)
 
+[![Pre-commit](https://img.shields.io/badge/pre--commit-enabled-informational?logo=pre-commit&logoColor=white)](https://github.com/ornikar/vertex-eduscore/blob/develop/.pre-commit-config.yaml)
+[![Linting: ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
+[![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat)](https://pycqa.github.io/isort/)
+
 </div>
 
 
 <details>
   <summary>📚 Table of Contents</summary>
   <ol>
     <li><a href="#-why-this-tool">Why this tool?</a></li>
@@ -347,15 +350,14 @@
 Let's say you defined a pipeline in `dummy_pipeline.py` and a config file named `config_test.json`. You can deploy your pipeline using the following command:
 ```bash
 vertex-deployer deploy dummy_pipeline \
     --compile \
     --upload \
     --run \
     --env-file example.env \
-    --local-package-path . \
     --tags my-tag \
     --config-filepath vertex/configs/dummy_pipeline/config_test.json \
     --experiment-name my-experiment \
     --enable-caching \
     --skip-validation
 ```
 
@@ -441,29 +443,27 @@
 ## Configuration
 
 You can configure the deployer using the `pyproject.toml` file to better fit your needs.
 This will overwrite default values. It can be useful if you always use the same options, e.g. always the same `--scheduler-timezone`
 
 ```toml
 [tool.vertex-deployer]
-pipelines_root_path = "my/path/to/vertex/pipelines"
-configs_root_path = "my/path/to/vertex/configs"
+vertex_folder_path = "my/path/to/vertex"
 log_level = "INFO"
 
 [tool.vertex-deployer.deploy]
 scheduler_timezone = "Europe/Paris"
 ```
 
 You can display all the configurable parameterss with default values by running:
 ```bash
 $ vertex-deployer config --all
 '*' means the value was set in config file
 
-* pipelines_root_path=my/path/to/vertex/pipelines
-* config_root_path=my/path/to/vertex/configs
+* vertex_folder_path=my/path/to/vertex
 * log_level=INFO
 deploy
   env_file=None
   compile=True
   upload=False
   run=False
   schedule=False
@@ -471,15 +471,14 @@
   delete_last_schedule=False
   * scheduler_timezone=Europe/Paris
   tags=['latest']
   config_filepath=None
   config_name=None
   enable_caching=False
   experiment_name=None
-  local_package_path=vertex/pipelines/compiled_pipelines
 check
   all=False
   config_filepath=None
   raise_error=False
 list
   with_configs=True
 create
```

#### html2text {}

```diff
@@ -1,51 +1,50 @@
-Metadata-Version: 2.1 Name: vertex-deployer Version: 0.4.4 Summary: Check,
+Metadata-Version: 2.1 Name: vertex-deployer Version: 0.5.0 Summary: Check,
 compile, upload, run, and schedule Kubeflow Pipelines on GCP Vertex AI in a
 standardized manner. Home-page: https://github.com/artefactory/vertex-
 pipelines-deployer License: Apache-2.0 Keywords:
 kubeflow,vertexai,aiplatform,gcp,mlops,deployer,pipeline Author: artefactory
 Author-email: jules.bertrand@artefact.com Requires-Python: >=3.8,<3.11.0
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Provides-Extra: profiling Requires-Dist:
-google-cloud-aiplatform (>=1.26,<2.0) Requires-Dist: kfp (>=2.0.1,<3.0)
-Requires-Dist: loguru (>=0.7,<0.8) Requires-Dist: pydantic (>=2.3,<3.0)
-Requires-Dist: pydantic-settings (>=2.0,<3.0) Requires-Dist: pyinstrument
-(>=4.5,<5.0) ; extra == "profiling" Requires-Dist: requests (>=2.31,<3.0)
-Requires-Dist: rich (>=13.5,<14.0) Requires-Dist: toml (>=0.10,<0.11) Requires-
-Dist: tomlkit (>=0.12,<0.13) Requires-Dist: typer (>=0.12,<0.13) Project-URL:
-Documentation, https://artefactory.github.io/vertex-pipelines-deployer/
-Project-URL: Repository, https://github.com/artefactory/vertex-pipelines-
-deployer Description-Content-Type: text/markdown
+google-cloud-aiplatform (>=1.26,<2.0) Requires-Dist: jinja2 (>=3.1.3,<4.0.0)
+Requires-Dist: kfp (>=2.0.1,<3.0) Requires-Dist: loguru (>=0.7,<0.8) Requires-
+Dist: pydantic (>=2.3,<3.0) Requires-Dist: pydantic-settings (>=2.0,<3.0)
+Requires-Dist: pyinstrument (>=4.5,<5.0) ; extra == "profiling" Requires-Dist:
+requests (>=2.31,<3.0) Requires-Dist: rich (>=13.5,<14.0) Requires-Dist: toml
+(>=0.10,<0.11) Requires-Dist: tomlkit (>=0.12,<0.13) Requires-Dist: typer
+(>=0.12,<0.13) Project-URL: Documentation, https://artefactory.github.io/
+vertex-pipelines-deployer/ Project-URL: Repository, https://github.com/
+artefactory/vertex-pipelines-deployer Description-Content-Type: text/markdown
                     ************ VVeerrtteexx PPiippeelliinneess DDeeppllooyyeerr ************
                                 _[_A_r_t_e_f_a_c_t_ _L_o_g_o_]
                ******** DDeeppllooyy VVeerrtteexx PPiippeelliinneess wwiitthhiinn mmiinnuutteess ********
  This tool is a wrapper around _k_f_p and _g_o_o_g_l_e_-_c_l_o_u_d_-_a_i_p_l_a_t_f_o_r_m that allows you
 to check, compile, upload, run, and schedule Vertex Pipelines in a standardized
                                     manner.
 
-     [![Python Version](https://img.shields.io/badge/Python-3.8_3.9_3.10-
- blue?logo=python)](#supported-python-versions) [![Code style: black](https://
- img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/
-   black) [![Imports: isort](https://img.shields.io/badge/%20imports-isort-
-  %231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/) [!
-         [Linting: ruff](https://img.shields.io/endpoint?url=https://
-raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json)](https:
-//github.com/astral-sh/ruff) [![Pre-commit](https://img.shields.io/badge/pre--
-    commit-enabled-informational?logo=pre-commit&logoColor=white)](https://
-  github.com/ornikar/vertex-eduscore/blob/develop/.pre-commit-config.yaml) [!
- [License](https://img.shields.io/github/license/artefactory/vertex-pipelines-
-deployer)](https://github.com/artefactory/vertex-pipelines-deployer/blob/main/
-   LICENSE) [![CI](https://github.com/artefactory/vertex-pipelines-deployer/
+    ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/vertex-
+ deployer?logo=python) ![PyPI - Status](https://img.shields.io/pypi/v/vertex-
+     deployer) ![PyPI - Downloads](https://img.shields.io/pypi/dm/vertex-
+ deployer?color=blue) ![PyPI - License](https://img.shields.io/pypi/l/vertex-
+  deployer) [![CI](https://github.com/artefactory/vertex-pipelines-deployer/
      actions/workflows/ci.yaml/badge.svg?branch=main&event=push)](https://
 github.com/artefactory/vertex-pipelines-deployer/actions/workflows/ci.yaml) [!
   [Release](https://github.com/artefactory/vertex-pipelines-deployer/actions/
  workflows/release.yaml/badge.svg?branch=main&event=push)](https://github.com/
-     artefactory/vertex-pipelines-deployer/actions/workflows/release.yaml)
+ artefactory/vertex-pipelines-deployer/actions/workflows/release.yaml) [![Pre-
+           commit](https://img.shields.io/badge/pre--commit-enabled-
+  informational?logo=pre-commit&logoColor=white)](https://github.com/ornikar/
+vertex-eduscore/blob/develop/.pre-commit-config.yaml) [![Linting: ruff](https:/
+ /img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/
+ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff) [![Imports:
+  isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat)]
+                       (https://pycqa.github.io/isort/)
 ð Table of Contents
    1. _W_h_y_ _t_h_i_s_ _t_o_o_l_?
    2. _P_r_e_r_e_q_u_i_s_i_t_e_s
    3. _I_n_s_t_a_l_l_a_t_i_o_n
          1. _F_r_o_m_ _g_i_t_ _r_e_p_o
          2. _F_r_o_m_ _A_r_t_i_f_a_c_t_ _R_e_g_i_s_t_r_y_ _(_n_o_t_ _a_v_a_i_l_a_b_l_e_ _i_n_ _P_y_P_I_ _y_e_t_)
          3. _A_d_d_ _t_o_ _r_e_q_u_i_r_e_m_e_n_t_s
@@ -166,70 +165,68 @@
 provided to ensure that you don't accidentally deploy to the wrong project. An
 [`example.env`](./example/example.env) file is provided in this repo. This also
 allows you to work with multiple environments thanks to env files (`test.env`,
 `dev.env`, `prod.env`, etc) ### ð CLI: Deploying a Pipeline with `deploy`
 Let's say you defined a pipeline in `dummy_pipeline.py` and a config file named
 `config_test.json`. You can deploy your pipeline using the following command:
 ```bash vertex-deployer deploy dummy_pipeline \ --compile \ --upload \ --run \
---env-file example.env \ --local-package-path . \ --tags my-tag \ --config-
-filepath vertex/configs/dummy_pipeline/config_test.json \ --experiment-name my-
-experiment \ --enable-caching \ --skip-validation ``` ### â CLI: Checking
-Pipelines are valid with `check` To check that your pipelines are valid, you
-can use the `check` command. It uses a pydantic model to: - check that your
-pipeline imports and definition are valid - check that your pipeline can be
-compiled - check that all configs related to the pipeline are respecting the
-pipeline definition (using a Pydantic model based on pipeline signature) To
-validate one or multiple pipeline(s): ```bash vertex-deployer check
-dummy_pipeline ``` To validate all pipelines in the `vertex/pipelines` folder:
-```bash vertex-deployer check --all ``` ### ð ï¸ CLI: Other commands ####
-`config` You can check your `vertex-deployer` configuration options using the
-`config` command. Fields set in `pyproject.toml` will overwrite default values
-and will be displayed differently: ```bash vertex-deployer config --all ```
-#### `create` You can create all files needed for a pipeline using the `create`
-command: ```bash vertex-deployer create my_new_pipeline --config-type py ```
-This will create a `my_new_pipeline.py` file in the `vertex/pipelines` folder
-and a `vertex/config/my_new_pipeline/` folder with multiple config files in it.
-#### `init` To initialize the deployer with default settings and folder
-structure, use the `init` command: ```bash vertex-deployer init ``` ```bash $
-vertex-deployer init Welcome to Vertex Deployer! This command will help you
-getting fired up. Do you want to configure the deployer? [y/n]: n Do you want
-to build default folder structure [y/n]: n Do you want to create a pipeline?
-[y/n]: n All done â¨ ``` #### `list` You can list all pipelines in the
-`vertex/pipelines` folder using the `list` command: ```bash vertex-deployer
-list --with-configs ``` ### ð­ CLI: Options ```bash vertex-deployer --help
-``` To see package version: ```bash vertex-deployer --version ``` To adapt log
-level, use the `--log-level` option. Default is `INFO`. ```bash vertex-deployer
---log-level DEBUG deploy ... ``` ## Configuration You can configure the
-deployer using the `pyproject.toml` file to better fit your needs. This will
-overwrite default values. It can be useful if you always use the same options,
-e.g. always the same `--scheduler-timezone` ```toml [tool.vertex-deployer]
-pipelines_root_path = "my/path/to/vertex/pipelines" configs_root_path = "my/
-path/to/vertex/configs" log_level = "INFO" [tool.vertex-deployer.deploy]
-scheduler_timezone = "Europe/Paris" ``` You can display all the configurable
-parameterss with default values by running: ```bash $ vertex-deployer config --
-all '*' means the value was set in config file * pipelines_root_path=my/path/
-to/vertex/pipelines * config_root_path=my/path/to/vertex/configs *
-log_level=INFO deploy env_file=None compile=True upload=False run=False
-schedule=False cron=None delete_last_schedule=False *
-scheduler_timezone=Europe/Paris tags=['latest'] config_filepath=None
-config_name=None enable_caching=False experiment_name=None
-local_package_path=vertex/pipelines/compiled_pipelines check all=False
-config_filepath=None raise_error=False list with_configs=True create
-config_type=json ``` ## Repository Structure ``` ââ .github â ââ
-ISSUE_TEMPLATE/ â ââ workflows â â ââ ci.yaml â â ââ
-pr_agent.yaml â â ââ release.yaml â ââ CODEOWNERS â ââ
-PULL_REQUEST_TEMPLATE.md ââ deployer # Source code â ââ __init__.py
-â ââ cli.py â ââ constants.py â ââ pipeline_checks.py â
-ââ pipeline_deployer.py â ââ settings.py â ââ utils â ââ
-config.py â ââ console.py â ââ exceptions.py â ââ logging.py
-â ââ models.py â ââ utils.py ââ docs/ # Documentation folder
-(mkdocs) ââ templates/ # Semantic Release templates ââ tests/ ââ
-example # Example folder with dummy pipeline and config | ââ example.env
-â ââ vertex â ââ components â â ââ dummy.py â ââ
-configs â â ââ broken_pipeline â â â ââ config_test.json â
-â ââ dummy_pipeline â â ââ config_test.json â â ââ
-config.py â â ââ config.toml â ââ deployment â ââ lib â
-ââ pipelines â ââ broken_pipeline.py â ââ dummy_pipeline.py
-ââ .gitignore ââ .pre-commit-config.yaml ââ catalog-info.yaml #
-Roadie integration configuration ââ CHANGELOG.md ââ CONTRIBUTING.md
-ââ LICENSE ââ Makefile ââ mkdocs.yml # Mkdocs configuration ââ
-pyproject.toml ââ README.md ```
+--env-file example.env \ --tags my-tag \ --config-filepath vertex/configs/
+dummy_pipeline/config_test.json \ --experiment-name my-experiment \ --enable-
+caching \ --skip-validation ``` ### â CLI: Checking Pipelines are valid with
+`check` To check that your pipelines are valid, you can use the `check`
+command. It uses a pydantic model to: - check that your pipeline imports and
+definition are valid - check that your pipeline can be compiled - check that
+all configs related to the pipeline are respecting the pipeline definition
+(using a Pydantic model based on pipeline signature) To validate one or
+multiple pipeline(s): ```bash vertex-deployer check dummy_pipeline ``` To
+validate all pipelines in the `vertex/pipelines` folder: ```bash vertex-
+deployer check --all ``` ### ð ï¸ CLI: Other commands #### `config` You can
+check your `vertex-deployer` configuration options using the `config` command.
+Fields set in `pyproject.toml` will overwrite default values and will be
+displayed differently: ```bash vertex-deployer config --all ``` #### `create`
+You can create all files needed for a pipeline using the `create` command:
+```bash vertex-deployer create my_new_pipeline --config-type py ``` This will
+create a `my_new_pipeline.py` file in the `vertex/pipelines` folder and a
+`vertex/config/my_new_pipeline/` folder with multiple config files in it. ####
+`init` To initialize the deployer with default settings and folder structure,
+use the `init` command: ```bash vertex-deployer init ``` ```bash $ vertex-
+deployer init Welcome to Vertex Deployer! This command will help you getting
+fired up. Do you want to configure the deployer? [y/n]: n Do you want to build
+default folder structure [y/n]: n Do you want to create a pipeline? [y/n]: n
+All done â¨ ``` #### `list` You can list all pipelines in the `vertex/
+pipelines` folder using the `list` command: ```bash vertex-deployer list --
+with-configs ``` ### ð­ CLI: Options ```bash vertex-deployer --help ``` To
+see package version: ```bash vertex-deployer --version ``` To adapt log level,
+use the `--log-level` option. Default is `INFO`. ```bash vertex-deployer --log-
+level DEBUG deploy ... ``` ## Configuration You can configure the deployer
+using the `pyproject.toml` file to better fit your needs. This will overwrite
+default values. It can be useful if you always use the same options, e.g.
+always the same `--scheduler-timezone` ```toml [tool.vertex-deployer]
+vertex_folder_path = "my/path/to/vertex" log_level = "INFO" [tool.vertex-
+deployer.deploy] scheduler_timezone = "Europe/Paris" ``` You can display all
+the configurable parameterss with default values by running: ```bash $ vertex-
+deployer config --all '*' means the value was set in config file *
+vertex_folder_path=my/path/to/vertex * log_level=INFO deploy env_file=None
+compile=True upload=False run=False schedule=False cron=None
+delete_last_schedule=False * scheduler_timezone=Europe/Paris tags=['latest']
+config_filepath=None config_name=None enable_caching=False experiment_name=None
+check all=False config_filepath=None raise_error=False list with_configs=True
+create config_type=json ``` ## Repository Structure ``` ââ .github â
+ââ ISSUE_TEMPLATE/ â ââ workflows â â ââ ci.yaml â â
+ââ pr_agent.yaml â â ââ release.yaml â ââ CODEOWNERS â
+ââ PULL_REQUEST_TEMPLATE.md ââ deployer # Source code â ââ
+__init__.py â ââ cli.py â ââ constants.py â ââ
+pipeline_checks.py â ââ pipeline_deployer.py â ââ settings.py â
+ââ utils â ââ config.py â ââ console.py â ââ
+exceptions.py â ââ logging.py â ââ models.py â ââ utils.py
+ââ docs/ # Documentation folder (mkdocs) ââ templates/ # Semantic
+Release templates ââ tests/ ââ example # Example folder with dummy
+pipeline and config | ââ example.env â ââ vertex â ââ
+components â â ââ dummy.py â ââ configs â â ââ
+broken_pipeline â â â ââ config_test.json â â ââ
+dummy_pipeline â â ââ config_test.json â â ââ config.py â â
+ââ config.toml â ââ deployment â ââ lib â ââ pipelines
+â ââ broken_pipeline.py â ââ dummy_pipeline.py ââ .gitignore
+ââ .pre-commit-config.yaml ââ catalog-info.yaml # Roadie integration
+configuration ââ CHANGELOG.md ââ CONTRIBUTING.md ââ LICENSE ââ
+Makefile ââ mkdocs.yml # Mkdocs configuration ââ pyproject.toml ââ
+README.md ```
```

