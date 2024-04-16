# Comparing `tmp/airbyte-source-my-hours-0.1.2.tar.gz` & `tmp/airbyte_source_my_hours-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte-source-my-hours-0.1.2.tar", last modified: Wed Jan 31 13:27:23 2024, max compression
+gzip compressed data, was "airbyte_source_my_hours-0.2.0.tar", max compression
```

## Comparing `airbyte-source-my-hours-0.1.2.tar` & `airbyte_source_my_hours-0.2.0.tar`

### file list

```diff
@@ -1,38 +1,9 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 13:27:23.526797 airbyte-source-my-hours-0.1.2/
--rw-r--r--   0 root         (0) root         (0)     5454 2024-01-31 13:27:23.526797 airbyte-source-my-hours-0.1.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5395 2024-01-31 13:14:34.000000 airbyte-source-my-hours-0.1.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 13:27:23.526797 airbyte-source-my-hours-0.1.2/airbyte_source_my_hours.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5454 2024-01-31 13:27:23.000000 airbyte-source-my-hours-0.1.2/airbyte_source_my_hours.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      986 2024-01-31 13:27:23.000000 airbyte-source-my-hours-0.1.2/airbyte_source_my_hours.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-01-31 13:27:23.000000 airbyte-source-my-hours-0.1.2/airbyte_source_my_hours.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       60 2024-01-31 13:27:23.000000 airbyte-source-my-hours-0.1.2/airbyte_source_my_hours.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       91 2024-01-31 13:27:23.000000 airbyte-source-my-hours-0.1.2/airbyte_source_my_hours.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       45 2024-01-31 13:27:23.000000 airbyte-source-my-hours-0.1.2/airbyte_source_my_hours.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 13:27:23.522797 airbyte-source-my-hours-0.1.2/integration_tests/
--rw-r--r--   0 root         (0) root         (0)       61 2024-01-31 13:14:34.000000 airbyte-source-my-hours-0.1.2/integration_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)      314 2024-01-31 13:14:34.000000 airbyte-source-my-hours-0.1.2/integration_tests/acceptance.py
--rw-r--r--   0 root         (0) root         (0)     8513 2024-01-31 13:14:34.000000 airbyte-source-my-hours-0.1.2/integration_tests/catalog.json
--rw-r--r--   0 root         (0) root         (0)     1368 2024-01-31 13:14:34.000000 airbyte-source-my-hours-0.1.2/integration_tests/configured_catalog.json
--rw-r--r--   0 root         (0) root         (0)      109 2024-01-31 13:14:34.000000 airbyte-source-my-hours-0.1.2/integration_tests/invalid_config.json
--rw-r--r--   0 root         (0) root         (0)      104 2024-01-31 13:14:34.000000 airbyte-source-my-hours-0.1.2/integration_tests/sample_config.json
--rw-r--r--   0 root         (0) root         (0)     5299 2024-01-31 13:27:23.526797 airbyte-source-my-hours-0.1.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      947 2024-01-31 13:27:21.000000 airbyte-source-my-hours-0.1.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 13:27:23.522797 airbyte-source-my-hours-0.1.2/source_my_hours/
--rw-r--r--   0 root         (0) root         (0)      126 2024-01-31 13:14:34.000000 airbyte-source-my-hours-0.1.2/source_my_hours/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2119 2024-01-31 13:14:34.000000 airbyte-source-my-hours-0.1.2/source_my_hours/auth.py
--rw-r--r--   0 root         (0) root         (0)      211 2024-01-31 13:14:34.000000 airbyte-source-my-hours-0.1.2/source_my_hours/constants.py
--rw-r--r--   0 root         (0) root         (0)      234 2024-01-31 13:14:34.000000 airbyte-source-my-hours-0.1.2/source_my_hours/run.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 13:27:23.526797 airbyte-source-my-hours-0.1.2/source_my_hours/schemas/
--rw-r--r--   0 root         (0) root         (0)      501 2024-01-31 13:14:34.000000 airbyte-source-my-hours-0.1.2/source_my_hours/schemas/clients.json
--rw-r--r--   0 root         (0) root         (0)     1631 2024-01-31 13:14:34.000000 airbyte-source-my-hours-0.1.2/source_my_hours/schemas/projects.json
--rw-r--r--   0 root         (0) root         (0)      378 2024-01-31 13:14:34.000000 airbyte-source-my-hours-0.1.2/source_my_hours/schemas/tags.json
--rw-r--r--   0 root         (0) root         (0)     3983 2024-01-31 13:14:34.000000 airbyte-source-my-hours-0.1.2/source_my_hours/schemas/time_logs.json
--rw-r--r--   0 root         (0) root         (0)      851 2024-01-31 13:14:34.000000 airbyte-source-my-hours-0.1.2/source_my_hours/schemas/users.json
--rw-r--r--   0 root         (0) root         (0)     4327 2024-01-31 13:14:34.000000 airbyte-source-my-hours-0.1.2/source_my_hours/source.py
--rw-r--r--   0 root         (0) root         (0)     1204 2024-01-31 13:14:34.000000 airbyte-source-my-hours-0.1.2/source_my_hours/spec.json
--rw-r--r--   0 root         (0) root         (0)      808 2024-01-31 13:14:34.000000 airbyte-source-my-hours-0.1.2/source_my_hours/stream.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 13:27:23.526797 airbyte-source-my-hours-0.1.2/unit_tests/
--rw-r--r--   0 root         (0) root         (0)       61 2024-01-31 13:14:34.000000 airbyte-source-my-hours-0.1.2/unit_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1097 2024-01-31 13:14:34.000000 airbyte-source-my-hours-0.1.2/unit_tests/test_auth.py
--rw-r--r--   0 root         (0) root         (0)     2431 2024-01-31 13:14:34.000000 airbyte-source-my-hours-0.1.2/unit_tests/test_source.py
--rw-r--r--   0 root         (0) root         (0)     1370 2024-01-31 13:14:34.000000 airbyte-source-my-hours-0.1.2/unit_tests/test_stream.py
+-rw-r--r--   0        0        0     4524 2024-04-16 00:39:35.638057 airbyte_source_my_hours-0.2.0/README.md
+-rw-r--r--   0        0        0      136 2024-04-16 00:39:35.638057 airbyte_source_my_hours-0.2.0/main.py
+-rw-r--r--   0        0        0      767 2024-04-16 00:43:04.333707 airbyte_source_my_hours-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      126 2024-04-16 00:39:35.638057 airbyte_source_my_hours-0.2.0/source_my_hours/__init__.py
+-rw-r--r--   0        0        0     3323 2024-04-16 00:39:35.638057 airbyte_source_my_hours-0.2.0/source_my_hours/components.py
+-rw-r--r--   0        0        0    13376 2024-04-16 00:39:35.638057 airbyte_source_my_hours-0.2.0/source_my_hours/manifest.yaml
+-rw-r--r--   0        0        0      227 2024-04-16 00:39:35.638057 airbyte_source_my_hours-0.2.0/source_my_hours/run.py
+-rw-r--r--   0        0        0      476 2024-04-16 00:39:35.638057 airbyte_source_my_hours-0.2.0/source_my_hours/source.py
+-rw-r--r--   0        0        0     5232 1970-01-01 00:00:00.000000 airbyte_source_my_hours-0.2.0/PKG-INFO
```

### Comparing `airbyte-source-my-hours-0.1.2/PKG-INFO` & `airbyte_source_my_hours-0.2.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,100 +1,122 @@
 Metadata-Version: 2.1
 Name: airbyte-source-my-hours
-Version: 0.1.2
-Summary: Source implementation for My Hours.
+Version: 0.2.0
+Summary: Source implementation for my-hours.
+Home-page: https://airbyte.com
+License: MIT
 Author: Airbyte
 Author-email: contact@airbyte.io
+Requires-Python: >=3.9,<3.12
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: airbyte-cdk (>=0,<1)
+Project-URL: Documentation, https://docs.airbyte.com/integrations/sources/my-hours
+Project-URL: Repository, https://github.com/airbytehq/airbyte
 Description-Content-Type: text/markdown
-Requires-Dist: airbyte-cdk
-Provides-Extra: tests
-Requires-Dist: requests-mock~=1.9.3; extra == "tests"
-Requires-Dist: pytest~=6.1; extra == "tests"
-Requires-Dist: pytest-mock~=3.6.1; extra == "tests"
-Requires-Dist: responses~=0.16.0; extra == "tests"
 
 # My Hours Source
 
-This is the repository for the My Hours source connector, written in Python.
-For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.io/integrations/sources/my-hours).
+This is the repository for the My Hours configuration based source connector.
+For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/my-hours).
 
+## Local development
 
-**To iterate on this connector, make sure to complete this prerequisites section.**
+### Prerequisites
 
+* Python (`^3.9`)
+* Poetry (`^1.7`) - installation instructions [here](https://python-poetry.org/docs/#installation)
 
-From this connector directory, create a virtual environment:
-```
-python -m venv .venv
-```
 
-This will generate a virtualenv for this module in `.venv/`. Make sure this venv is active in your
-development environment of choice. To activate it from the terminal, run:
-```
-source .venv/bin/activate
-pip install -r requirements.txt
-pip install '.[tests]'
+
+### Installing the connector
+
+From this connector directory, run:
+```bash
+poetry install --with dev
 ```
-If you are in an IDE, follow your IDE's instructions to activate the virtualenv.
 
-Note that while we are installing dependencies from `requirements.txt`, you should only edit `setup.py` for your dependencies. `requirements.txt` is
-used for editable installs (`pip install -e`) to pull in Python dependencies from the monorepo and will call `setup.py`.
-If this is mumbo jumbo to you, don't worry about it, just put your deps in `setup.py` but install using `pip install -r requirements.txt` and everything
-should work as you expect.
 
-**If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.io/integrations/sources/my-hours)
-to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_my_hours/spec.json` file.
+### Create credentials
+
+**If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/my-hours)
+to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `spec` inside `manifest/yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
-See `integration_tests/sample_config.json` for a sample config file.
+See `sample_files/sample_config.json` for a sample config file.
+
 
-**If you are an Airbyte core member**, copy the credentials in Lastpass under the secret name `source my-hours test creds`
-and place them into `secrets/config.json`.
+### Locally running the connector
 
 ```
-python main.py spec
-python main.py check --config secrets/config.json
-python main.py discover --config secrets/config.json
-python main.py read --config secrets/config.json --catalog integration_tests/configured_catalog.json
+poetry run source-my-hours spec
+poetry run source-my-hours check --config secrets/config.json
+poetry run source-my-hours discover --config secrets/config.json
+poetry run source-my-hours read --config secrets/config.json --catalog sample_files/configured_catalog.json
 ```
 
+### Running tests
 
+To run tests locally, from the connector directory run:
 
-**Via [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md) (recommended):**
-```bash
-airbyte-ci connectors --name=source-my-hours build
+```
+poetry run pytest tests
 ```
 
-An image will be built with the tag `airbyte/source-my-hours:dev`.
+### Building the docker image
 
-**Via `docker build`:**
+1. Install [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md)
+2. Run the following command to build the docker image:
 ```bash
-docker build -t airbyte/source-my-hours:dev .
+airbyte-ci connectors --name=source-my-hours build
 ```
 
+An image will be available on your host with the tag `airbyte/source-my-hours:dev`.
+
+
+### Running as a docker container
+
 Then run any of the connector commands as follows:
 ```
 docker run --rm airbyte/source-my-hours:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-my-hours:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-my-hours:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-my-hours:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
+### Running our CI test suite
+
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
 ```bash
 airbyte-ci connectors --name=source-my-hours test
 ```
 
-Customize `acceptance-test-config.yml` file to configure tests. See [Connector Acceptance Tests](https://docs.airbyte.com/connector-development/testing-connectors/connector-acceptance-tests-reference) for more information.
+### Customizing acceptance Tests
+
+Customize `acceptance-test-config.yml` file to configure acceptance tests. See [Connector Acceptance Tests](https://docs.airbyte.com/connector-development/testing-connectors/connector-acceptance-tests-reference) for more information.
 If your connector requires to create or destroy resources for use during acceptance tests create fixtures for it and place them inside integration_tests/acceptance.py.
 
-All of your dependencies should go in `setup.py`, NOT `requirements.txt`. The requirements file is only used to connect internal Airbyte dependencies in the monorepo for local development.
-We split dependencies between two groups, dependencies that are:
-* required for your connector to work need to go to `MAIN_REQUIREMENTS` list.
-* required for the testing need to go to `TEST_REQUIREMENTS` list
+### Dependency Management
+
+All of your dependencies should be managed via Poetry. 
+To add a new dependency, run:
+```bash
+poetry add <package-name>
+```
+
+Please commit the changes to `pyproject.toml` and `poetry.lock` files.
+
+## Publishing a new version of the connector
 
 You've checked out the repo, implemented a million dollar feature, and you're ready to share your changes with the world. Now what?
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-my-hours test`
-2. Bump the connector version in `metadata.yaml`: increment the `dockerImageTag` value. Please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors).
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
+    - bump the `dockerImageTag` value in in `metadata.yaml`
+    - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
-4. Make the connector documentation and its changelog is up to date (`docs/integrations/sources/my-hours.md`).
+4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/my-hours.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
+8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
```

