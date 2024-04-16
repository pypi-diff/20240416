# Comparing `tmp/craft-application-2.4.0.tar.gz` & `tmp/craft_application-2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "craft-application-2.4.0.tar", last modified: Tue Apr  2 14:25:30 2024, max compression
+gzip compressed data, was "craft_application-2.5.tar", last modified: Tue Apr 16 16:53:30 2024, max compression
```

## Comparing `craft-application-2.4.0.tar` & `craft_application-2.5.tar`

### file list

```diff
@@ -1,216 +1,216 @@
-drwxrwxr-x   0 lengau    (1000) lengau    (1000)        0 2024-04-02 14:25:30.070026 craft-application-2.4.0/
--rw-rw-r--   0 lengau    (1000) lengau    (1000)      723 2024-03-26 02:12:45.000000 craft-application-2.4.0/.editorconfig
-drwxrwxr-x   0 lengau    (1000) lengau    (1000)        0 2024-04-02 14:25:30.056026 craft-application-2.4.0/.github/
--rw-rw-r--   0 lengau    (1000) lengau    (1000)      518 2024-03-26 02:12:45.000000 craft-application-2.4.0/.github/.jira_sync_config.yaml
-drwxrwxr-x   0 lengau    (1000) lengau    (1000)        0 2024-04-02 14:25:30.057026 craft-application-2.4.0/.github/ISSUE_TEMPLATE/
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     1386 2024-03-26 02:12:45.000000 craft-application-2.4.0/.github/ISSUE_TEMPLATE/bug.yaml
--rw-rw-r--   0 lengau    (1000) lengau    (1000)      389 2024-03-26 02:12:45.000000 craft-application-2.4.0/.github/ISSUE_TEMPLATE/config.yml
--rw-rw-r--   0 lengau    (1000) lengau    (1000)      788 2024-03-26 02:12:45.000000 craft-application-2.4.0/.github/ISSUE_TEMPLATE/task.yaml
--rw-rw-r--   0 lengau    (1000) lengau    (1000)      179 2024-03-26 02:12:45.000000 craft-application-2.4.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-rw-r--   0 lengau    (1000) lengau    (1000)      506 2024-03-26 02:12:45.000000 craft-application-2.4.0/.github/release-drafter.yaml
--rw-rw-r--   0 lengau    (1000) lengau    (1000)      506 2024-03-26 02:12:45.000000 craft-application-2.4.0/.github/release-drafter.yml
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     4699 2024-03-26 02:12:45.000000 craft-application-2.4.0/.github/renovate.json5
-drwxrwxr-x   0 lengau    (1000) lengau    (1000)        0 2024-04-02 14:25:30.057026 craft-application-2.4.0/.github/workflows/
--rw-rw-r--   0 lengau    (1000) lengau    (1000)      179 2024-03-26 02:12:45.000000 craft-application-2.4.0/.github/workflows/cla-check.yaml
--rw-rw-r--   0 lengau    (1000) lengau    (1000)      919 2024-03-26 02:12:45.000000 craft-application-2.4.0/.github/workflows/docs.yaml
--rw-rw-r--   0 lengau    (1000) lengau    (1000)      346 2024-03-26 02:12:45.000000 craft-application-2.4.0/.github/workflows/release-drafter.yaml
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     4541 2024-03-26 02:12:45.000000 craft-application-2.4.0/.github/workflows/tests.yaml
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     1949 2024-03-26 02:12:45.000000 craft-application-2.4.0/.gitignore
--rw-rw-r--   0 lengau    (1000) lengau    (1000)      921 2024-03-26 02:12:45.000000 craft-application-2.4.0/.pre-commit-config.yaml
--rw-rw-r--   0 lengau    (1000) lengau    (1000)      395 2024-03-26 02:12:45.000000 craft-application-2.4.0/.readthedocs.yaml
--rw-rw-r--   0 lengau    (1000) lengau    (1000)      188 2024-03-26 02:12:45.000000 craft-application-2.4.0/.yamllint.yaml
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     4393 2024-03-26 02:12:45.000000 craft-application-2.4.0/HACKING.rst
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     7652 2024-03-26 02:12:45.000000 craft-application-2.4.0/LICENSE
--rw-r--r--   0 lengau    (1000) lengau    (1000)     3310 2024-04-02 14:25:30.070026 craft-application-2.4.0/PKG-INFO
--rw-rw-r--   0 lengau    (1000) lengau    (1000)      552 2024-03-26 02:12:45.000000 craft-application-2.4.0/README.rst
-drwxrwxr-x   0 lengau    (1000) lengau    (1000)        0 2024-04-02 14:25:30.057026 craft-application-2.4.0/craft_application/
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     1522 2024-03-26 22:30:41.000000 craft-application-2.4.0/craft_application/__init__.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)      411 2024-04-02 14:25:29.000000 craft-application-2.4.0/craft_application/_version.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)    29493 2024-04-01 23:33:46.000000 craft-application-2.4.0/craft_application/application.py
-drwxrwxr-x   0 lengau    (1000) lengau    (1000)        0 2024-04-02 14:25:30.058026 craft-application-2.4.0/craft_application/commands/
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     1163 2024-03-26 02:12:45.000000 craft-application-2.4.0/craft_application/commands/__init__.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     7234 2024-03-26 02:12:45.000000 craft-application-2.4.0/craft_application/commands/base.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)    12723 2024-03-26 02:12:45.000000 craft-application-2.4.0/craft_application/commands/lifecycle.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     1608 2024-03-26 02:12:45.000000 craft-application-2.4.0/craft_application/commands/other.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     7040 2024-03-26 02:12:45.000000 craft-application-2.4.0/craft_application/errors.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     2439 2024-03-26 02:12:45.000000 craft-application-2.4.0/craft_application/grammar.py
-drwxrwxr-x   0 lengau    (1000) lengau    (1000)        0 2024-04-02 14:25:30.058026 craft-application-2.4.0/craft_application/launchpad/
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     1135 2024-03-26 02:12:45.000000 craft-application-2.4.0/craft_application/launchpad/__init__.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     1000 2024-03-26 02:12:45.000000 craft-application-2.4.0/craft_application/launchpad/errors.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     8564 2024-03-26 02:12:45.000000 craft-application-2.4.0/craft_application/launchpad/launchpad.py
-drwxrwxr-x   0 lengau    (1000) lengau    (1000)        0 2024-04-02 14:25:30.059026 craft-application-2.4.0/craft_application/launchpad/models/
--rw-rw-r--   0 lengau    (1000) lengau    (1000)      621 2024-03-26 02:12:45.000000 craft-application-2.4.0/craft_application/launchpad/models/__init__.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     6820 2024-03-26 02:12:45.000000 craft-application-2.4.0/craft_application/launchpad/models/base.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     4927 2024-03-26 02:12:45.000000 craft-application-2.4.0/craft_application/launchpad/models/build.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     5292 2024-03-26 02:12:45.000000 craft-application-2.4.0/craft_application/launchpad/models/code.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     2236 2024-03-26 02:12:45.000000 craft-application-2.4.0/craft_application/launchpad/models/distro.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     3496 2024-04-02 14:22:38.000000 craft-application-2.4.0/craft_application/launchpad/models/project.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)    16303 2024-03-26 02:12:45.000000 craft-application-2.4.0/craft_application/launchpad/models/recipe.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     6039 2024-03-26 02:12:45.000000 craft-application-2.4.0/craft_application/launchpad/util.py
-drwxrwxr-x   0 lengau    (1000) lengau    (1000)        0 2024-04-02 14:25:30.059026 craft-application-2.4.0/craft_application/misc/
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     1637 2024-03-26 02:12:45.000000 craft-application-2.4.0/craft_application/misc/instance_bashrc
-drwxrwxr-x   0 lengau    (1000) lengau    (1000)        0 2024-04-02 14:25:30.059026 craft-application-2.4.0/craft_application/models/
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     1421 2024-03-26 02:12:45.000000 craft-application-2.4.0/craft_application/models/__init__.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     3725 2024-03-26 02:12:45.000000 craft-application-2.4.0/craft_application/models/base.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     2935 2024-03-26 02:12:45.000000 craft-application-2.4.0/craft_application/models/constraints.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     2507 2024-03-26 02:12:45.000000 craft-application-2.4.0/craft_application/models/grammar.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     1175 2024-03-26 02:12:45.000000 craft-application-2.4.0/craft_application/models/metadata.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     4752 2024-03-26 02:12:45.000000 craft-application-2.4.0/craft_application/models/project.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)        0 2024-03-26 02:12:45.000000 craft-application-2.4.0/craft_application/py.typed
-drwxrwxr-x   0 lengau    (1000) lengau    (1000)        0 2024-04-02 14:25:30.060026 craft-application-2.4.0/craft_application/remote/
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     1337 2024-03-26 02:12:45.000000 craft-application-2.4.0/craft_application/remote/__init__.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     2329 2024-03-26 02:12:45.000000 craft-application-2.4.0/craft_application/remote/errors.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)    11714 2024-03-26 02:12:45.000000 craft-application-2.4.0/craft_application/remote/git.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     4206 2024-03-26 02:12:45.000000 craft-application-2.4.0/craft_application/remote/utils.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     2070 2024-03-26 02:12:45.000000 craft-application-2.4.0/craft_application/remote/worktree.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     6731 2024-03-26 02:12:45.000000 craft-application-2.4.0/craft_application/secrets.py
-drwxrwxr-x   0 lengau    (1000) lengau    (1000)        0 2024-04-02 14:25:30.061026 craft-application-2.4.0/craft_application/services/
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     1444 2024-03-26 02:12:45.000000 craft-application-2.4.0/craft_application/services/__init__.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     2106 2024-03-26 02:12:45.000000 craft-application-2.4.0/craft_application/services/base.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)    16185 2024-04-01 23:33:46.000000 craft-application-2.4.0/craft_application/services/lifecycle.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     3128 2024-03-26 02:12:45.000000 craft-application-2.4.0/craft_application/services/package.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)    12545 2024-04-01 23:33:46.000000 craft-application-2.4.0/craft_application/services/provider.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)    13794 2024-04-02 14:22:38.000000 craft-application-2.4.0/craft_application/services/remotebuild.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     4323 2024-03-26 02:12:45.000000 craft-application-2.4.0/craft_application/services/request.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     4273 2024-03-26 02:12:45.000000 craft-application-2.4.0/craft_application/services/service_factory.py
-drwxrwxr-x   0 lengau    (1000) lengau    (1000)        0 2024-04-02 14:25:30.061026 craft-application-2.4.0/craft_application/util/
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     1701 2024-03-26 02:12:45.000000 craft-application-2.4.0/craft_application/util/__init__.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     2465 2024-03-26 02:12:45.000000 craft-application-2.4.0/craft_application/util/callbacks.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     4170 2024-03-26 02:12:45.000000 craft-application-2.4.0/craft_application/util/error_formatting.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)      950 2024-03-26 02:12:45.000000 craft-application-2.4.0/craft_application/util/logging.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     1470 2024-03-26 02:12:45.000000 craft-application-2.4.0/craft_application/util/paths.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     2494 2024-03-26 02:12:45.000000 craft-application-2.4.0/craft_application/util/platforms.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     2065 2024-03-26 02:12:45.000000 craft-application-2.4.0/craft_application/util/repositories.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     4110 2024-03-26 02:12:45.000000 craft-application-2.4.0/craft_application/util/snap_config.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     2241 2024-03-26 02:12:45.000000 craft-application-2.4.0/craft_application/util/string.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     4930 2024-03-26 02:12:45.000000 craft-application-2.4.0/craft_application/util/yaml.py
-drwxrwxr-x   0 lengau    (1000) lengau    (1000)        0 2024-04-02 14:25:30.068026 craft-application-2.4.0/craft_application.egg-info/
--rw-r--r--   0 lengau    (1000) lengau    (1000)     3310 2024-04-02 14:25:30.000000 craft-application-2.4.0/craft_application.egg-info/PKG-INFO
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     6026 2024-04-02 14:25:30.000000 craft-application-2.4.0/craft_application.egg-info/SOURCES.txt
--rw-rw-r--   0 lengau    (1000) lengau    (1000)        1 2024-04-02 14:25:30.000000 craft-application-2.4.0/craft_application.egg-info/dependency_links.txt
--rw-rw-r--   0 lengau    (1000) lengau    (1000)      871 2024-04-02 14:25:30.000000 craft-application-2.4.0/craft_application.egg-info/requires.txt
--rw-rw-r--   0 lengau    (1000) lengau    (1000)       18 2024-04-02 14:25:30.000000 craft-application-2.4.0/craft_application.egg-info/top_level.txt
-drwxrwxr-x   0 lengau    (1000) lengau    (1000)        0 2024-04-02 14:25:30.062026 craft-application-2.4.0/docs/
-drwxrwxr-x   0 lengau    (1000) lengau    (1000)        0 2024-04-02 14:25:30.054026 craft-application-2.4.0/docs/_static/
-drwxrwxr-x   0 lengau    (1000) lengau    (1000)        0 2024-04-02 14:25:30.062026 craft-application-2.4.0/docs/_static/css/
--rw-rw-r--   0 lengau    (1000) lengau    (1000)      481 2024-03-26 02:12:45.000000 craft-application-2.4.0/docs/_static/css/custom.css
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     1684 2024-03-26 02:12:45.000000 craft-application-2.4.0/docs/conf.py
-drwxrwxr-x   0 lengau    (1000) lengau    (1000)        0 2024-04-02 14:25:30.062026 craft-application-2.4.0/docs/explanation/
--rw-rw-r--   0 lengau    (1000) lengau    (1000)       72 2024-03-26 02:12:45.000000 craft-application-2.4.0/docs/explanation/index.rst
-drwxrwxr-x   0 lengau    (1000) lengau    (1000)        0 2024-04-02 14:25:30.062026 craft-application-2.4.0/docs/howto/
--rw-rw-r--   0 lengau    (1000) lengau    (1000)       70 2024-03-26 02:12:45.000000 craft-application-2.4.0/docs/howto/index.rst
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     1201 2024-03-26 02:12:45.000000 craft-application-2.4.0/docs/index.rst
-drwxrwxr-x   0 lengau    (1000) lengau    (1000)        0 2024-04-02 14:25:30.062026 craft-application-2.4.0/docs/reference/
--rw-rw-r--   0 lengau    (1000) lengau    (1000)      142 2024-03-26 02:12:45.000000 craft-application-2.4.0/docs/reference/index.rst
-drwxrwxr-x   0 lengau    (1000) lengau    (1000)        0 2024-04-02 14:25:30.062026 craft-application-2.4.0/docs/tutorials/
--rw-rw-r--   0 lengau    (1000) lengau    (1000)      238 2024-03-26 02:12:45.000000 craft-application-2.4.0/docs/tutorials/index.rst
--rw-rw-r--   0 lengau    (1000) lengau    (1000)    10490 2024-04-01 23:33:46.000000 craft-application-2.4.0/pyproject.toml
--rw-rw-r--   0 lengau    (1000) lengau    (1000)       38 2024-04-02 14:25:30.070026 craft-application-2.4.0/setup.cfg
-drwxrwxr-x   0 lengau    (1000) lengau    (1000)        0 2024-04-02 14:25:30.062026 craft-application-2.4.0/tests/
--rw-rw-r--   0 lengau    (1000) lengau    (1000)        0 2024-03-26 02:12:45.000000 craft-application-2.4.0/tests/__init__.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     9326 2024-04-02 14:22:38.000000 craft-application-2.4.0/tests/conftest.py
-drwxrwxr-x   0 lengau    (1000) lengau    (1000)        0 2024-04-02 14:25:30.062026 craft-application-2.4.0/tests/integration/
--rw-rw-r--   0 lengau    (1000) lengau    (1000)        0 2024-03-26 02:12:45.000000 craft-application-2.4.0/tests/integration/__init__.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     3149 2024-04-02 14:22:38.000000 craft-application-2.4.0/tests/integration/conftest.py
-drwxrwxr-x   0 lengau    (1000) lengau    (1000)        0 2024-04-02 14:25:30.055026 craft-application-2.4.0/tests/integration/data/
-drwxrwxr-x   0 lengau    (1000) lengau    (1000)        0 2024-04-02 14:25:30.062026 craft-application-2.4.0/tests/integration/data/build-secrets/
-drwxrwxr-x   0 lengau    (1000) lengau    (1000)        0 2024-04-02 14:25:30.063026 craft-application-2.4.0/tests/integration/data/build-secrets/secret-source-folder/
--rw-rw-r--   0 lengau    (1000) lengau    (1000)       14 2024-03-26 02:12:45.000000 craft-application-2.4.0/tests/integration/data/build-secrets/secret-source-folder/source-file.txt
--rw-rw-r--   0 lengau    (1000) lengau    (1000)      442 2024-03-26 02:12:45.000000 craft-application-2.4.0/tests/integration/data/build-secrets/testcraft.yaml
-drwxrwxr-x   0 lengau    (1000) lengau    (1000)        0 2024-04-02 14:25:30.054026 craft-application-2.4.0/tests/integration/data/invalid_projects/
-drwxrwxr-x   0 lengau    (1000) lengau    (1000)        0 2024-04-02 14:25:30.063026 craft-application-2.4.0/tests/integration/data/invalid_projects/build-error/
--rw-rw-r--   0 lengau    (1000) lengau    (1000)      177 2024-03-26 02:12:45.000000 craft-application-2.4.0/tests/integration/data/invalid_projects/build-error/testcraft.yaml
-drwxrwxr-x   0 lengau    (1000) lengau    (1000)        0 2024-04-02 14:25:30.055026 craft-application-2.4.0/tests/integration/data/valid_projects/
-drwxrwxr-x   0 lengau    (1000) lengau    (1000)        0 2024-04-02 14:25:30.063026 craft-application-2.4.0/tests/integration/data/valid_projects/adoption/
--rw-rw-r--   0 lengau    (1000) lengau    (1000)       26 2024-03-26 02:12:45.000000 craft-application-2.4.0/tests/integration/data/valid_projects/adoption/stderr
--rw-rw-r--   0 lengau    (1000) lengau    (1000)      209 2024-03-26 02:12:45.000000 craft-application-2.4.0/tests/integration/data/valid_projects/adoption/testcraft.yaml
-drwxrwxr-x   0 lengau    (1000) lengau    (1000)        0 2024-04-02 14:25:30.063026 craft-application-2.4.0/tests/integration/data/valid_projects/basic/
--rw-rw-r--   0 lengau    (1000) lengau    (1000)       26 2024-03-26 02:12:45.000000 craft-application-2.4.0/tests/integration/data/valid_projects/basic/stderr
--rw-rw-r--   0 lengau    (1000) lengau    (1000)      114 2024-03-26 02:12:45.000000 craft-application-2.4.0/tests/integration/data/valid_projects/basic/testcraft.yaml
-drwxrwxr-x   0 lengau    (1000) lengau    (1000)        0 2024-04-02 14:25:30.063026 craft-application-2.4.0/tests/integration/data/valid_projects/environment/
--rw-rw-r--   0 lengau    (1000) lengau    (1000)       26 2024-03-26 02:12:45.000000 craft-application-2.4.0/tests/integration/data/valid_projects/environment/stderr
--rw-rw-r--   0 lengau    (1000) lengau    (1000)      483 2024-03-26 02:12:45.000000 craft-application-2.4.0/tests/integration/data/valid_projects/environment/testcraft.yaml
-drwxrwxr-x   0 lengau    (1000) lengau    (1000)        0 2024-04-02 14:25:30.063026 craft-application-2.4.0/tests/integration/data/valid_projects/grammar/
-drwxrwxr-x   0 lengau    (1000) lengau    (1000)        0 2024-04-02 14:25:30.055026 craft-application-2.4.0/tests/integration/data/valid_projects/grammar/src/
-drwxrwxr-x   0 lengau    (1000) lengau    (1000)        0 2024-04-02 14:25:30.063026 craft-application-2.4.0/tests/integration/data/valid_projects/grammar/src/on-amd64-to-amd64/
--rw-rw-r--   0 lengau    (1000) lengau    (1000)       18 2024-03-26 02:12:45.000000 craft-application-2.4.0/tests/integration/data/valid_projects/grammar/src/on-amd64-to-amd64/hello.txt
-drwxrwxr-x   0 lengau    (1000) lengau    (1000)        0 2024-04-02 14:25:30.064026 craft-application-2.4.0/tests/integration/data/valid_projects/grammar/src/on-amd64-to-arm64/
--rw-rw-r--   0 lengau    (1000) lengau    (1000)       18 2024-03-26 02:12:45.000000 craft-application-2.4.0/tests/integration/data/valid_projects/grammar/src/on-amd64-to-arm64/hello.txt
--rw-rw-r--   0 lengau    (1000) lengau    (1000)       26 2024-03-26 02:12:45.000000 craft-application-2.4.0/tests/integration/data/valid_projects/grammar/stderr
--rw-rw-r--   0 lengau    (1000) lengau    (1000)      229 2024-03-26 02:12:45.000000 craft-application-2.4.0/tests/integration/data/valid_projects/grammar/testcraft.yaml
-drwxrwxr-x   0 lengau    (1000) lengau    (1000)        0 2024-04-02 14:25:30.064026 craft-application-2.4.0/tests/integration/launchpad/
--rw-rw-r--   0 lengau    (1000) lengau    (1000)        0 2024-03-26 02:12:45.000000 craft-application-2.4.0/tests/integration/launchpad/__init__.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     1021 2024-03-26 02:12:45.000000 craft-application-2.4.0/tests/integration/launchpad/conftest.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     1647 2024-03-26 02:12:45.000000 craft-application-2.4.0/tests/integration/launchpad/test_anonymous_access.py
-drwxrwxr-x   0 lengau    (1000) lengau    (1000)        0 2024-04-02 14:25:30.064026 craft-application-2.4.0/tests/integration/services/
--rw-rw-r--   0 lengau    (1000) lengau    (1000)        0 2024-03-26 02:12:45.000000 craft-application-2.4.0/tests/integration/services/__init__.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     5475 2024-03-26 02:12:45.000000 craft-application-2.4.0/tests/integration/services/test_lifecycle.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     4287 2024-03-26 21:46:05.000000 craft-application-2.4.0/tests/integration/services/test_provider.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     1886 2024-04-02 14:22:38.000000 craft-application-2.4.0/tests/integration/services/test_remotebuild.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     3445 2024-03-26 02:12:45.000000 craft-application-2.4.0/tests/integration/services/test_request.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     1909 2024-03-26 02:12:45.000000 craft-application-2.4.0/tests/integration/services/test_service_factory.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)    13467 2024-03-26 02:12:45.000000 craft-application-2.4.0/tests/integration/test_application.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     2201 2024-03-26 02:12:45.000000 craft-application-2.4.0/tests/integration/test_version.py
-drwxrwxr-x   0 lengau    (1000) lengau    (1000)        0 2024-04-02 14:25:30.065026 craft-application-2.4.0/tests/unit/
--rw-rw-r--   0 lengau    (1000) lengau    (1000)        0 2024-03-26 02:12:45.000000 craft-application-2.4.0/tests/unit/__init__.py
-drwxrwxr-x   0 lengau    (1000) lengau    (1000)        0 2024-04-02 14:25:30.065026 craft-application-2.4.0/tests/unit/commands/
--rw-rw-r--   0 lengau    (1000) lengau    (1000)        0 2024-03-26 02:12:45.000000 craft-application-2.4.0/tests/unit/commands/__init__.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     6705 2024-03-26 02:12:45.000000 craft-application-2.4.0/tests/unit/commands/test_base.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)    17375 2024-03-26 02:12:45.000000 craft-application-2.4.0/tests/unit/commands/test_lifecycle.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     1363 2024-03-26 02:12:45.000000 craft-application-2.4.0/tests/unit/commands/test_other.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     1673 2024-03-26 02:12:45.000000 craft-application-2.4.0/tests/unit/conftest.py
-drwxrwxr-x   0 lengau    (1000) lengau    (1000)        0 2024-04-02 14:25:30.065026 craft-application-2.4.0/tests/unit/launchpad/
--rw-rw-r--   0 lengau    (1000) lengau    (1000)        0 2024-03-26 02:12:45.000000 craft-application-2.4.0/tests/unit/launchpad/__init__.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     1194 2024-03-26 02:12:45.000000 craft-application-2.4.0/tests/unit/launchpad/conftest.py
-drwxrwxr-x   0 lengau    (1000) lengau    (1000)        0 2024-04-02 14:25:30.066026 craft-application-2.4.0/tests/unit/launchpad/models/
--rw-rw-r--   0 lengau    (1000) lengau    (1000)        0 2024-03-26 02:12:45.000000 craft-application-2.4.0/tests/unit/launchpad/models/__init__.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     5159 2024-03-26 02:12:45.000000 craft-application-2.4.0/tests/unit/launchpad/models/test_base.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     2562 2024-03-26 02:12:45.000000 craft-application-2.4.0/tests/unit/launchpad/models/test_code.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     9305 2024-03-26 02:12:45.000000 craft-application-2.4.0/tests/unit/launchpad/test_launchpad.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     3500 2024-03-26 02:12:45.000000 craft-application-2.4.0/tests/unit/launchpad/test_util.py
-drwxrwxr-x   0 lengau    (1000) lengau    (1000)        0 2024-04-02 14:25:30.066026 craft-application-2.4.0/tests/unit/models/
--rw-rw-r--   0 lengau    (1000) lengau    (1000)        0 2024-03-26 02:12:45.000000 craft-application-2.4.0/tests/unit/models/__init__.py
-drwxrwxr-x   0 lengau    (1000) lengau    (1000)        0 2024-04-02 14:25:30.066026 craft-application-2.4.0/tests/unit/models/project_models/
--rw-rw-r--   0 lengau    (1000) lengau    (1000)       68 2024-03-26 02:12:45.000000 craft-application-2.4.0/tests/unit/models/project_models/basic_project.yaml
--rw-rw-r--   0 lengau    (1000) lengau    (1000)      436 2024-03-26 02:12:45.000000 craft-application-2.4.0/tests/unit/models/project_models/full_project.yaml
--rw-rw-r--   0 lengau    (1000) lengau    (1000)       24 2024-03-26 02:12:45.000000 craft-application-2.4.0/tests/unit/models/project_models/invalid_project.yaml
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     4489 2024-03-26 02:12:45.000000 craft-application-2.4.0/tests/unit/models/test_constraints.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)    10302 2024-03-26 02:12:45.000000 craft-application-2.4.0/tests/unit/models/test_project.py
-drwxrwxr-x   0 lengau    (1000) lengau    (1000)        0 2024-04-02 14:25:30.066026 craft-application-2.4.0/tests/unit/remote/
--rw-rw-r--   0 lengau    (1000) lengau    (1000)        0 2024-03-26 02:12:45.000000 craft-application-2.4.0/tests/unit/remote/__init__.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)      855 2024-03-26 02:12:45.000000 craft-application-2.4.0/tests/unit/remote/conftest.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     2116 2024-03-26 02:12:45.000000 craft-application-2.4.0/tests/unit/remote/test_errors.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)    18388 2024-03-26 02:12:45.000000 craft-application-2.4.0/tests/unit/remote/test_git.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     5855 2024-03-26 02:12:45.000000 craft-application-2.4.0/tests/unit/remote/test_utils.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     3034 2024-03-26 02:12:45.000000 craft-application-2.4.0/tests/unit/remote/test_worktree.py
-drwxrwxr-x   0 lengau    (1000) lengau    (1000)        0 2024-04-02 14:25:30.067026 craft-application-2.4.0/tests/unit/services/
--rw-rw-r--   0 lengau    (1000) lengau    (1000)        0 2024-03-26 02:12:45.000000 craft-application-2.4.0/tests/unit/services/__init__.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     3566 2024-04-02 14:22:36.000000 craft-application-2.4.0/tests/unit/services/conftest.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)    21558 2024-04-01 23:33:46.000000 craft-application-2.4.0/tests/unit/services/test_lifecycle.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     3413 2024-03-26 02:12:45.000000 craft-application-2.4.0/tests/unit/services/test_package.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)    19346 2024-04-01 23:33:46.000000 craft-application-2.4.0/tests/unit/services/test_provider.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     9113 2024-04-02 14:22:38.000000 craft-application-2.4.0/tests/unit/services/test_remotebuild.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     3629 2024-03-26 02:12:45.000000 craft-application-2.4.0/tests/unit/services/test_repositories.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     4000 2024-03-26 02:12:45.000000 craft-application-2.4.0/tests/unit/services/test_request.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     5005 2024-03-26 02:12:45.000000 craft-application-2.4.0/tests/unit/services/test_service_factory.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)    39437 2024-04-01 23:33:46.000000 craft-application-2.4.0/tests/unit/test_application.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     2968 2024-03-26 02:12:45.000000 craft-application-2.4.0/tests/unit/test_errors.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     7670 2024-03-26 02:12:45.000000 craft-application-2.4.0/tests/unit/test_grammar.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)       57 2024-03-26 02:12:45.000000 craft-application-2.4.0/tests/unit/test_nothing.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     5444 2024-03-26 02:12:45.000000 craft-application-2.4.0/tests/unit/test_secrets.py
-drwxrwxr-x   0 lengau    (1000) lengau    (1000)        0 2024-04-02 14:25:30.068026 craft-application-2.4.0/tests/unit/util/
--rw-rw-r--   0 lengau    (1000) lengau    (1000)        0 2024-03-26 02:12:45.000000 craft-application-2.4.0/tests/unit/util/__init__.py
-drwxrwxr-x   0 lengau    (1000) lengau    (1000)        0 2024-04-02 14:25:30.068026 craft-application-2.4.0/tests/unit/util/invalid_yaml/
--rw-rw-r--   0 lengau    (1000) lengau    (1000)      156 2024-03-26 02:12:45.000000 craft-application-2.4.0/tests/unit/util/invalid_yaml/_README
--rw-rw-r--   0 lengau    (1000) lengau    (1000)       46 2024-03-26 02:12:45.000000 craft-application-2.4.0/tests/unit/util/invalid_yaml/duplicate_second_level.yaml-invalid
--rw-rw-r--   0 lengau    (1000) lengau    (1000)       40 2024-03-26 02:12:45.000000 craft-application-2.4.0/tests/unit/util/invalid_yaml/duplicate_top_level.yaml-invalid
--rw-rw-r--   0 lengau    (1000) lengau    (1000)       30 2024-03-26 02:12:45.000000 craft-application-2.4.0/tests/unit/util/invalid_yaml/unhashable.yaml-invalid
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     3189 2024-03-26 02:12:45.000000 craft-application-2.4.0/tests/unit/util/test_error_formatting.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)      603 2024-03-26 02:12:45.000000 craft-application-2.4.0/tests/unit/util/test_logging.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     1573 2024-03-26 02:12:45.000000 craft-application-2.4.0/tests/unit/util/test_paths.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     5221 2024-03-26 02:12:45.000000 craft-application-2.4.0/tests/unit/util/test_snap_config.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     3383 2024-03-26 02:12:45.000000 craft-application-2.4.0/tests/unit/util/test_string.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     2992 2024-03-26 02:12:45.000000 craft-application-2.4.0/tests/unit/util/test_yaml.py
-drwxrwxr-x   0 lengau    (1000) lengau    (1000)        0 2024-04-02 14:25:30.068026 craft-application-2.4.0/tests/unit/util/valid_yaml/
--rw-rw-r--   0 lengau    (1000) lengau    (1000)        0 2024-03-26 02:12:45.000000 craft-application-2.4.0/tests/unit/util/valid_yaml/empty.yaml
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     4900 2024-03-26 02:12:45.000000 craft-application-2.4.0/tox.ini
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-16 16:53:30.747967 craft_application-2.5/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      723 2023-09-29 14:32:21.000000 craft_application-2.5/.editorconfig
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-16 16:53:30.719966 craft_application-2.5/.github/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      518 2024-02-15 23:03:01.000000 craft_application-2.5/.github/.jira_sync_config.yaml
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-16 16:53:30.719966 craft_application-2.5/.github/ISSUE_TEMPLATE/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     1386 2023-09-29 14:32:21.000000 craft_application-2.5/.github/ISSUE_TEMPLATE/bug.yaml
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      389 2023-09-29 14:32:21.000000 craft_application-2.5/.github/ISSUE_TEMPLATE/config.yml
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      788 2023-09-29 14:32:21.000000 craft_application-2.5/.github/ISSUE_TEMPLATE/task.yaml
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      179 2023-09-29 14:32:21.000000 craft_application-2.5/.github/PULL_REQUEST_TEMPLATE.md
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      506 2023-09-29 14:32:21.000000 craft_application-2.5/.github/release-drafter.yaml
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      506 2023-09-29 14:32:21.000000 craft_application-2.5/.github/release-drafter.yml
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     4699 2024-03-19 19:28:11.000000 craft_application-2.5/.github/renovate.json5
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-16 16:53:30.723966 craft_application-2.5/.github/workflows/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      179 2023-09-29 14:32:21.000000 craft_application-2.5/.github/workflows/cla-check.yaml
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      919 2024-02-15 23:03:01.000000 craft_application-2.5/.github/workflows/docs.yaml
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      346 2024-02-15 23:03:01.000000 craft_application-2.5/.github/workflows/release-drafter.yaml
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     4541 2024-02-22 17:50:51.000000 craft_application-2.5/.github/workflows/tests.yaml
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     1949 2023-09-29 14:32:21.000000 craft_application-2.5/.gitignore
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      921 2023-09-29 14:32:21.000000 craft_application-2.5/.pre-commit-config.yaml
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      395 2023-11-10 10:29:35.000000 craft_application-2.5/.readthedocs.yaml
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      188 2023-09-29 14:32:21.000000 craft_application-2.5/.yamllint.yaml
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     4393 2024-03-12 17:53:13.000000 craft_application-2.5/HACKING.rst
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     7652 2023-09-29 14:32:21.000000 craft_application-2.5/LICENSE
+-rw-r--r--   0 tiago     (1000) tiago     (1000)     3310 2024-04-16 16:53:30.747967 craft_application-2.5/PKG-INFO
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      552 2023-09-29 14:32:21.000000 craft_application-2.5/README.rst
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-16 16:53:30.723966 craft_application-2.5/craft_application/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     1522 2024-03-28 20:33:36.000000 craft_application-2.5/craft_application/__init__.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      411 2024-04-16 16:53:30.000000 craft_application-2.5/craft_application/_version.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)    29493 2024-04-02 11:30:59.000000 craft_application-2.5/craft_application/application.py
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-16 16:53:30.723966 craft_application-2.5/craft_application/commands/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     1163 2023-12-06 11:10:45.000000 craft_application-2.5/craft_application/commands/__init__.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     7234 2024-03-12 17:53:13.000000 craft_application-2.5/craft_application/commands/base.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)    12723 2024-03-12 17:53:13.000000 craft_application-2.5/craft_application/commands/lifecycle.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     1608 2023-09-29 14:32:21.000000 craft_application-2.5/craft_application/commands/other.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     7040 2024-03-20 22:10:47.000000 craft_application-2.5/craft_application/errors.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     3843 2024-04-16 16:52:34.000000 craft_application-2.5/craft_application/grammar.py
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-16 16:53:30.723966 craft_application-2.5/craft_application/launchpad/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     1135 2024-02-15 23:03:01.000000 craft_application-2.5/craft_application/launchpad/__init__.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     1000 2024-02-15 23:03:01.000000 craft_application-2.5/craft_application/launchpad/errors.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     8564 2024-02-26 17:15:25.000000 craft_application-2.5/craft_application/launchpad/launchpad.py
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-16 16:53:30.727966 craft_application-2.5/craft_application/launchpad/models/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      621 2024-02-26 17:15:16.000000 craft_application-2.5/craft_application/launchpad/models/__init__.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     6820 2024-02-26 17:15:16.000000 craft_application-2.5/craft_application/launchpad/models/base.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     4927 2024-02-26 17:15:25.000000 craft_application-2.5/craft_application/launchpad/models/build.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     5292 2024-02-26 17:15:16.000000 craft_application-2.5/craft_application/launchpad/models/code.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     2236 2024-02-26 17:15:16.000000 craft_application-2.5/craft_application/launchpad/models/distro.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     3496 2024-04-03 17:32:43.000000 craft_application-2.5/craft_application/launchpad/models/project.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)    16303 2024-03-21 21:55:13.000000 craft_application-2.5/craft_application/launchpad/models/recipe.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     6039 2024-02-22 17:50:51.000000 craft_application-2.5/craft_application/launchpad/util.py
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-16 16:53:30.727966 craft_application-2.5/craft_application/misc/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     1637 2024-02-15 23:03:01.000000 craft_application-2.5/craft_application/misc/instance_bashrc
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-16 16:53:30.727966 craft_application-2.5/craft_application/models/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     1421 2024-02-15 23:03:01.000000 craft_application-2.5/craft_application/models/__init__.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     3725 2024-02-15 23:03:01.000000 craft_application-2.5/craft_application/models/base.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     2935 2024-03-12 17:53:13.000000 craft_application-2.5/craft_application/models/constraints.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     3462 2024-04-16 16:52:34.000000 craft_application-2.5/craft_application/models/grammar.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     1175 2023-09-29 14:32:21.000000 craft_application-2.5/craft_application/models/metadata.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     4752 2024-04-16 16:52:04.000000 craft_application-2.5/craft_application/models/project.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2023-09-29 14:32:21.000000 craft_application-2.5/craft_application/py.typed
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-16 16:53:30.727966 craft_application-2.5/craft_application/remote/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     1337 2024-03-12 17:53:13.000000 craft_application-2.5/craft_application/remote/__init__.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     2329 2024-02-22 17:50:51.000000 craft_application-2.5/craft_application/remote/errors.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)    11974 2024-04-16 16:52:34.000000 craft_application-2.5/craft_application/remote/git.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     4206 2024-03-12 17:53:13.000000 craft_application-2.5/craft_application/remote/utils.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     2070 2024-02-15 23:03:01.000000 craft_application-2.5/craft_application/remote/worktree.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     6731 2024-02-22 17:50:51.000000 craft_application-2.5/craft_application/secrets.py
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-16 16:53:30.727966 craft_application-2.5/craft_application/services/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     1444 2024-02-15 23:03:01.000000 craft_application-2.5/craft_application/services/__init__.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     2106 2024-02-15 23:03:01.000000 craft_application-2.5/craft_application/services/base.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)    16185 2024-04-02 11:30:59.000000 craft_application-2.5/craft_application/services/lifecycle.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     3128 2024-03-19 19:28:11.000000 craft_application-2.5/craft_application/services/package.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)    12545 2024-04-02 11:30:59.000000 craft_application-2.5/craft_application/services/provider.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)    14846 2024-04-16 16:52:34.000000 craft_application-2.5/craft_application/services/remotebuild.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     4323 2024-02-15 23:03:01.000000 craft_application-2.5/craft_application/services/request.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     4273 2024-02-15 23:03:01.000000 craft_application-2.5/craft_application/services/service_factory.py
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-16 16:53:30.731966 craft_application-2.5/craft_application/util/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     1701 2024-03-12 17:53:13.000000 craft_application-2.5/craft_application/util/__init__.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     2465 2024-02-22 17:50:51.000000 craft_application-2.5/craft_application/util/callbacks.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     4170 2024-02-22 17:50:51.000000 craft_application-2.5/craft_application/util/error_formatting.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      950 2023-12-06 11:10:45.000000 craft_application-2.5/craft_application/util/logging.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     1470 2024-02-15 23:03:01.000000 craft_application-2.5/craft_application/util/paths.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     2494 2024-02-28 16:38:56.000000 craft_application-2.5/craft_application/util/platforms.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     2065 2024-02-15 23:03:01.000000 craft_application-2.5/craft_application/util/repositories.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     4110 2024-02-26 17:15:25.000000 craft_application-2.5/craft_application/util/snap_config.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     2241 2024-03-12 17:53:13.000000 craft_application-2.5/craft_application/util/string.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     4930 2024-03-19 19:28:11.000000 craft_application-2.5/craft_application/util/yaml.py
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-16 16:53:30.743967 craft_application-2.5/craft_application.egg-info/
+-rw-r--r--   0 tiago     (1000) tiago     (1000)     3310 2024-04-16 16:53:30.000000 craft_application-2.5/craft_application.egg-info/PKG-INFO
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     6026 2024-04-16 16:53:30.000000 craft_application-2.5/craft_application.egg-info/SOURCES.txt
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)        1 2024-04-16 16:53:30.000000 craft_application-2.5/craft_application.egg-info/dependency_links.txt
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      871 2024-04-16 16:53:30.000000 craft_application-2.5/craft_application.egg-info/requires.txt
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)       18 2024-04-16 16:53:30.000000 craft_application-2.5/craft_application.egg-info/top_level.txt
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-16 16:53:30.731966 craft_application-2.5/docs/
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-16 16:53:30.715966 craft_application-2.5/docs/_static/
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-16 16:53:30.731966 craft_application-2.5/docs/_static/css/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      481 2023-09-29 14:32:21.000000 craft_application-2.5/docs/_static/css/custom.css
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     1684 2023-09-29 14:32:21.000000 craft_application-2.5/docs/conf.py
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-16 16:53:30.731966 craft_application-2.5/docs/explanation/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)       72 2023-09-29 14:32:21.000000 craft_application-2.5/docs/explanation/index.rst
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-16 16:53:30.731966 craft_application-2.5/docs/howto/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)       70 2023-09-29 14:32:21.000000 craft_application-2.5/docs/howto/index.rst
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     1201 2023-09-29 14:32:21.000000 craft_application-2.5/docs/index.rst
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-16 16:53:30.731966 craft_application-2.5/docs/reference/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      142 2023-09-29 14:32:21.000000 craft_application-2.5/docs/reference/index.rst
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-16 16:53:30.731966 craft_application-2.5/docs/tutorials/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      238 2023-09-29 14:32:21.000000 craft_application-2.5/docs/tutorials/index.rst
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)    10638 2024-04-16 16:52:34.000000 craft_application-2.5/pyproject.toml
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)       38 2024-04-16 16:53:30.747967 craft_application-2.5/setup.cfg
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-16 16:53:30.731966 craft_application-2.5/tests/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2023-09-29 14:32:21.000000 craft_application-2.5/tests/__init__.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     9326 2024-04-03 17:32:43.000000 craft_application-2.5/tests/conftest.py
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-16 16:53:30.731966 craft_application-2.5/tests/integration/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2023-09-29 14:32:21.000000 craft_application-2.5/tests/integration/__init__.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     3149 2024-04-03 17:32:43.000000 craft_application-2.5/tests/integration/conftest.py
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-16 16:53:30.715966 craft_application-2.5/tests/integration/data/
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-16 16:53:30.731966 craft_application-2.5/tests/integration/data/build-secrets/
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-16 16:53:30.735967 craft_application-2.5/tests/integration/data/build-secrets/secret-source-folder/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)       14 2023-10-19 21:00:44.000000 craft_application-2.5/tests/integration/data/build-secrets/secret-source-folder/source-file.txt
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      442 2023-10-19 21:00:44.000000 craft_application-2.5/tests/integration/data/build-secrets/testcraft.yaml
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-16 16:53:30.715966 craft_application-2.5/tests/integration/data/invalid_projects/
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-16 16:53:30.735967 craft_application-2.5/tests/integration/data/invalid_projects/build-error/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      177 2023-10-25 15:47:00.000000 craft_application-2.5/tests/integration/data/invalid_projects/build-error/testcraft.yaml
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-16 16:53:30.715966 craft_application-2.5/tests/integration/data/valid_projects/
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-16 16:53:30.735967 craft_application-2.5/tests/integration/data/valid_projects/adoption/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)       26 2024-02-26 17:15:25.000000 craft_application-2.5/tests/integration/data/valid_projects/adoption/stderr
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      209 2024-02-26 17:15:25.000000 craft_application-2.5/tests/integration/data/valid_projects/adoption/testcraft.yaml
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-16 16:53:30.735967 craft_application-2.5/tests/integration/data/valid_projects/basic/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)       26 2024-02-26 17:15:25.000000 craft_application-2.5/tests/integration/data/valid_projects/basic/stderr
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      114 2024-02-26 17:15:25.000000 craft_application-2.5/tests/integration/data/valid_projects/basic/testcraft.yaml
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-16 16:53:30.735967 craft_application-2.5/tests/integration/data/valid_projects/environment/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)       26 2024-02-26 17:15:25.000000 craft_application-2.5/tests/integration/data/valid_projects/environment/stderr
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      483 2024-02-26 17:15:25.000000 craft_application-2.5/tests/integration/data/valid_projects/environment/testcraft.yaml
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-16 16:53:30.735967 craft_application-2.5/tests/integration/data/valid_projects/grammar/
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-16 16:53:30.715966 craft_application-2.5/tests/integration/data/valid_projects/grammar/src/
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-16 16:53:30.735967 craft_application-2.5/tests/integration/data/valid_projects/grammar/src/on-amd64-to-amd64/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)       18 2024-03-20 22:10:47.000000 craft_application-2.5/tests/integration/data/valid_projects/grammar/src/on-amd64-to-amd64/hello.txt
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-16 16:53:30.735967 craft_application-2.5/tests/integration/data/valid_projects/grammar/src/on-amd64-to-arm64/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)       18 2024-03-20 22:10:47.000000 craft_application-2.5/tests/integration/data/valid_projects/grammar/src/on-amd64-to-arm64/hello.txt
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)       26 2024-03-20 22:10:47.000000 craft_application-2.5/tests/integration/data/valid_projects/grammar/stderr
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      500 2024-04-16 16:52:34.000000 craft_application-2.5/tests/integration/data/valid_projects/grammar/testcraft.yaml
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-16 16:53:30.735967 craft_application-2.5/tests/integration/launchpad/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2024-02-15 23:03:01.000000 craft_application-2.5/tests/integration/launchpad/__init__.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     1021 2024-02-26 17:15:16.000000 craft_application-2.5/tests/integration/launchpad/conftest.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     1700 2024-04-16 16:52:34.000000 craft_application-2.5/tests/integration/launchpad/test_anonymous_access.py
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-16 16:53:30.735967 craft_application-2.5/tests/integration/services/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2023-09-29 14:32:21.000000 craft_application-2.5/tests/integration/services/__init__.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     5475 2024-02-28 16:38:56.000000 craft_application-2.5/tests/integration/services/test_lifecycle.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     4287 2024-03-12 17:53:13.000000 craft_application-2.5/tests/integration/services/test_provider.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     1886 2024-04-03 17:32:43.000000 craft_application-2.5/tests/integration/services/test_remotebuild.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     3445 2024-02-15 23:03:01.000000 craft_application-2.5/tests/integration/services/test_request.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     1909 2024-02-28 16:38:56.000000 craft_application-2.5/tests/integration/services/test_service_factory.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)    13467 2024-03-21 21:55:13.000000 craft_application-2.5/tests/integration/test_application.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     2201 2023-09-29 14:32:21.000000 craft_application-2.5/tests/integration/test_version.py
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-16 16:53:30.735967 craft_application-2.5/tests/unit/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2023-09-29 14:32:21.000000 craft_application-2.5/tests/unit/__init__.py
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-16 16:53:30.739966 craft_application-2.5/tests/unit/commands/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2023-09-29 14:32:21.000000 craft_application-2.5/tests/unit/commands/__init__.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     6705 2023-12-06 11:10:45.000000 craft_application-2.5/tests/unit/commands/test_base.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)    17375 2024-03-12 17:53:13.000000 craft_application-2.5/tests/unit/commands/test_lifecycle.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     1363 2023-09-29 14:32:21.000000 craft_application-2.5/tests/unit/commands/test_other.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     1673 2024-02-15 23:03:01.000000 craft_application-2.5/tests/unit/conftest.py
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-16 16:53:30.739966 craft_application-2.5/tests/unit/launchpad/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2024-02-15 23:03:01.000000 craft_application-2.5/tests/unit/launchpad/__init__.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     1194 2024-02-26 17:15:16.000000 craft_application-2.5/tests/unit/launchpad/conftest.py
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-16 16:53:30.739966 craft_application-2.5/tests/unit/launchpad/models/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2024-02-15 23:03:01.000000 craft_application-2.5/tests/unit/launchpad/models/__init__.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     5159 2024-02-26 17:15:16.000000 craft_application-2.5/tests/unit/launchpad/models/test_base.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     2562 2024-02-26 17:15:16.000000 craft_application-2.5/tests/unit/launchpad/models/test_code.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     9305 2024-03-21 21:55:13.000000 craft_application-2.5/tests/unit/launchpad/test_launchpad.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     3500 2024-02-28 16:38:56.000000 craft_application-2.5/tests/unit/launchpad/test_util.py
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-16 16:53:30.739966 craft_application-2.5/tests/unit/models/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2023-09-29 14:32:21.000000 craft_application-2.5/tests/unit/models/__init__.py
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-16 16:53:30.739966 craft_application-2.5/tests/unit/models/project_models/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)       68 2023-09-29 14:32:21.000000 craft_application-2.5/tests/unit/models/project_models/basic_project.yaml
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      436 2023-09-29 14:32:21.000000 craft_application-2.5/tests/unit/models/project_models/full_project.yaml
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)       24 2023-09-29 14:32:21.000000 craft_application-2.5/tests/unit/models/project_models/invalid_project.yaml
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     4489 2024-02-15 23:03:01.000000 craft_application-2.5/tests/unit/models/test_constraints.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)    10302 2024-04-16 16:52:04.000000 craft_application-2.5/tests/unit/models/test_project.py
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-16 16:53:30.739966 craft_application-2.5/tests/unit/remote/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2024-02-15 23:03:01.000000 craft_application-2.5/tests/unit/remote/__init__.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      855 2024-02-15 23:03:01.000000 craft_application-2.5/tests/unit/remote/conftest.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     2116 2024-02-15 23:03:01.000000 craft_application-2.5/tests/unit/remote/test_errors.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)    18388 2024-03-19 19:28:11.000000 craft_application-2.5/tests/unit/remote/test_git.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     5855 2024-03-12 17:53:13.000000 craft_application-2.5/tests/unit/remote/test_utils.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     3034 2024-02-15 23:03:01.000000 craft_application-2.5/tests/unit/remote/test_worktree.py
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-16 16:53:30.743967 craft_application-2.5/tests/unit/services/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2023-09-29 14:32:21.000000 craft_application-2.5/tests/unit/services/__init__.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     3946 2024-04-16 16:52:34.000000 craft_application-2.5/tests/unit/services/conftest.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)    21558 2024-04-02 11:30:59.000000 craft_application-2.5/tests/unit/services/test_lifecycle.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     3413 2024-03-12 17:53:13.000000 craft_application-2.5/tests/unit/services/test_package.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)    19346 2024-04-02 11:30:59.000000 craft_application-2.5/tests/unit/services/test_provider.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)    11829 2024-04-16 16:52:34.000000 craft_application-2.5/tests/unit/services/test_remotebuild.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     3629 2024-02-15 23:03:01.000000 craft_application-2.5/tests/unit/services/test_repositories.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     4000 2024-02-15 23:03:01.000000 craft_application-2.5/tests/unit/services/test_request.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     5005 2024-02-26 17:15:25.000000 craft_application-2.5/tests/unit/services/test_service_factory.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)    53044 2024-04-16 16:52:34.000000 craft_application-2.5/tests/unit/test_application.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     2968 2024-02-15 23:03:01.000000 craft_application-2.5/tests/unit/test_errors.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     7670 2024-04-16 16:52:04.000000 craft_application-2.5/tests/unit/test_grammar.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)       57 2023-09-29 14:32:21.000000 craft_application-2.5/tests/unit/test_nothing.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     5444 2023-10-19 21:00:44.000000 craft_application-2.5/tests/unit/test_secrets.py
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-16 16:53:30.743967 craft_application-2.5/tests/unit/util/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2023-09-29 14:32:21.000000 craft_application-2.5/tests/unit/util/__init__.py
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-16 16:53:30.743967 craft_application-2.5/tests/unit/util/invalid_yaml/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      156 2023-09-29 14:32:21.000000 craft_application-2.5/tests/unit/util/invalid_yaml/_README
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)       46 2023-09-29 14:32:21.000000 craft_application-2.5/tests/unit/util/invalid_yaml/duplicate_second_level.yaml-invalid
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)       40 2023-09-29 14:32:21.000000 craft_application-2.5/tests/unit/util/invalid_yaml/duplicate_top_level.yaml-invalid
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)       30 2023-09-29 14:32:21.000000 craft_application-2.5/tests/unit/util/invalid_yaml/unhashable.yaml-invalid
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     3189 2023-12-07 17:42:39.000000 craft_application-2.5/tests/unit/util/test_error_formatting.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      603 2023-12-06 11:10:45.000000 craft_application-2.5/tests/unit/util/test_logging.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     1573 2024-02-15 23:03:01.000000 craft_application-2.5/tests/unit/util/test_paths.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     5221 2024-02-26 17:15:25.000000 craft_application-2.5/tests/unit/util/test_snap_config.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     3383 2024-03-12 17:53:13.000000 craft_application-2.5/tests/unit/util/test_string.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     2992 2024-03-19 19:28:11.000000 craft_application-2.5/tests/unit/util/test_yaml.py
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-16 16:53:30.743967 craft_application-2.5/tests/unit/util/valid_yaml/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2023-09-29 14:32:21.000000 craft_application-2.5/tests/unit/util/valid_yaml/empty.yaml
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     4900 2024-04-16 16:52:04.000000 craft_application-2.5/tox.ini
```

### Comparing `craft-application-2.4.0/.editorconfig` & `craft_application-2.5/.editorconfig`

 * *Files identical despite different names*

### Comparing `craft-application-2.4.0/.github/.jira_sync_config.yaml` & `craft_application-2.5/.github/.jira_sync_config.yaml`

 * *Files identical despite different names*

### Comparing `craft-application-2.4.0/.github/ISSUE_TEMPLATE/bug.yaml` & `craft_application-2.5/.github/ISSUE_TEMPLATE/bug.yaml`

 * *Files identical despite different names*

### Comparing `craft-application-2.4.0/.github/ISSUE_TEMPLATE/task.yaml` & `craft_application-2.5/.github/ISSUE_TEMPLATE/task.yaml`

 * *Files identical despite different names*

### Comparing `craft-application-2.4.0/.github/renovate.json5` & `craft_application-2.5/.github/renovate.json5`

 * *Files identical despite different names*

### Comparing `craft-application-2.4.0/.github/workflows/docs.yaml` & `craft_application-2.5/.github/workflows/docs.yaml`

 * *Files identical despite different names*

### Comparing `craft-application-2.4.0/.github/workflows/tests.yaml` & `craft_application-2.5/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `craft-application-2.4.0/.gitignore` & `craft_application-2.5/.gitignore`

 * *Files identical despite different names*

### Comparing `craft-application-2.4.0/.pre-commit-config.yaml` & `craft_application-2.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `craft-application-2.4.0/HACKING.rst` & `craft_application-2.5/HACKING.rst`

 * *Files identical despite different names*

### Comparing `craft-application-2.4.0/LICENSE` & `craft_application-2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `craft-application-2.4.0/PKG-INFO` & `craft_application-2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: craft-application
-Version: 2.4.0
+Version: 2.5.0
 Summary: A framework for *craft applications.
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.10
@@ -13,15 +13,15 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Requires-Python: >=3.10
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: craft-archives>=1.1.3
 Requires-Dist: craft-cli>=2.4.0
-Requires-Dist: craft-grammar>=1.1.1
+Requires-Dist: craft-grammar>=1.2.0
 Requires-Dist: craft-parts>=1.21.1
 Requires-Dist: craft-providers<2.0,>=1.20.0
 Requires-Dist: snap-helpers>=0.4.2
 Requires-Dist: platformdirs>=3.10
 Requires-Dist: pydantic<2.0,>=1.10
 Requires-Dist: pydantic-yaml<1.0
 Requires-Dist: pygit2<1.15.0,>=1.13.0
@@ -33,25 +33,25 @@
 Requires-Dist: coverage[toml]==7.4.4; extra == "dev"
 Requires-Dist: hypothesis>=6.0; extra == "dev"
 Requires-Dist: pyfakefs~=5.3; extra == "dev"
 Requires-Dist: pytest==8.1.1; extra == "dev"
 Requires-Dist: pytest-check==2.3.1; extra == "dev"
 Requires-Dist: pytest-cov==5.0.0; extra == "dev"
 Requires-Dist: pytest-mock==3.14.0; extra == "dev"
-Requires-Dist: pytest-rerunfailures==13.0; extra == "dev"
+Requires-Dist: pytest-rerunfailures==14.0; extra == "dev"
 Requires-Dist: pytest-time>=0.3.1; extra == "dev"
 Requires-Dist: responses~=0.25.0; extra == "dev"
 Requires-Dist: craft-application[remote]; extra == "dev"
 Provides-Extra: lint
 Requires-Dist: black~=24.0; extra == "lint"
 Requires-Dist: codespell[toml]==2.2.6; extra == "lint"
 Requires-Dist: yamllint==1.35.1; extra == "lint"
 Provides-Extra: types
 Requires-Dist: mypy[reports]==1.9.0; extra == "types"
-Requires-Dist: pyright==1.1.356; extra == "types"
+Requires-Dist: pyright==1.1.358; extra == "types"
 Requires-Dist: types-requests; extra == "types"
 Requires-Dist: types-urllib3; extra == "types"
 Provides-Extra: docs
 Requires-Dist: furo==2024.1.29; extra == "docs"
 Requires-Dist: sphinx<7.3,>=7.2.6; extra == "docs"
 Requires-Dist: sphinx-autobuild==2024.2.4; extra == "docs"
 Requires-Dist: sphinx-copybutton==0.5.2; extra == "docs"
```

### Comparing `craft-application-2.4.0/README.rst` & `craft_application-2.5/README.rst`

 * *Files identical despite different names*

### Comparing `craft-application-2.4.0/craft_application/__init__.py` & `craft_application-2.5/craft_application/__init__.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.4.0/craft_application/application.py` & `craft_application-2.5/craft_application/application.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.4.0/craft_application/commands/__init__.py` & `craft_application-2.5/craft_application/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.4.0/craft_application/commands/base.py` & `craft_application-2.5/craft_application/commands/base.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.4.0/craft_application/commands/lifecycle.py` & `craft_application-2.5/craft_application/commands/lifecycle.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.4.0/craft_application/commands/other.py` & `craft_application-2.5/craft_application/commands/other.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.4.0/craft_application/errors.py` & `craft_application-2.5/craft_application/errors.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.4.0/craft_application/grammar.py` & `craft_application-2.5/craft_application/grammar.py`

 * *Files 26% similar despite different names*

```diff
@@ -11,46 +11,79 @@
 # SATISFACTORY QUALITY, or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 # General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License along
 # with this program.  If not, see <http://www.gnu.org/licenses/>.
 """Grammar processor."""
 
-from typing import Any
+from typing import Any, cast
 
+import craft_cli
 from craft_grammar import GrammarProcessor  # type: ignore[import-untyped]
+from craft_grammar.errors import GrammarSyntaxError  # type: ignore[import-untyped]
 
-_KEYS = [
-    "source",
+from craft_application.errors import CraftValidationError
+
+# Values that should return as a single object / list / dict.
+_NON_SCALAR_VALUES = [
+    "source-submodules",
+    "after",
+    "overlay-packages",
+    "build-attributes",
+    "permissions",
     "build-environment",
     "build-packages",
     "stage-packages",
     "build-snaps",
     "stage-snaps",
+    "overlay",
+    "organize",
+    "stage",
+    "prime",
 ]
 
-_SCALAR_VALUES = ["source"]
+# Values that should return a dict, not in a list.
+_DICT_ONLY_VALUES = [
+    "organize",
+]
 
 
 def process_part(
     *, part_yaml_data: dict[str, Any], processor: GrammarProcessor
 ) -> dict[str, Any]:
     """Process grammar for a given part."""
-    existing_keys = (key for key in _KEYS if key in part_yaml_data)
-
-    for key in existing_keys:
+    for key in part_yaml_data:
         unprocessed_grammar = part_yaml_data[key]
+        craft_cli.emit.debug(f"Processing grammar for {key}: {unprocessed_grammar}")
 
-        if key in _SCALAR_VALUES and isinstance(unprocessed_grammar, str):
+        # grammar aware models can only be a string or list of dict, skip any other type.
+        if isinstance(unprocessed_grammar, list):
+            if any(not isinstance(d, dict) for d in unprocessed_grammar):  # type: ignore[reportUnknownVariableType]
+                continue
+            if any(not isinstance(k, str) for d in unprocessed_grammar for k in d):  # type: ignore[reportUnknownVariableType]
+                continue
+            unprocessed_grammar = cast(list[dict[str, Any]], unprocessed_grammar)
+        elif isinstance(unprocessed_grammar, str):
             unprocessed_grammar = [unprocessed_grammar]
+        else:
+            continue
 
-        processed_grammar = processor.process(grammar=unprocessed_grammar)
-
-        if key in _SCALAR_VALUES:
+        try:
+            processed_grammar = processor.process(grammar=unprocessed_grammar)
+        except GrammarSyntaxError as e:
+            raise CraftValidationError(
+                f"Invalid grammar syntax while processing '{key}' in '{part_yaml_data}': {e}"
+            ) from e
+
+        # special cases
+        # scalar values should return as a single object, not in a list.
+        # dict values should return as a dict, not in a list.
+        if key not in _NON_SCALAR_VALUES or key in _DICT_ONLY_VALUES:
             processed_grammar = processed_grammar[0] if processed_grammar else None
+
         part_yaml_data[key] = processed_grammar
 
     return part_yaml_data
 
 
 def process_parts(
     *, parts_yaml_data: dict[str, Any], arch: str, target_arch: str
```

### Comparing `craft-application-2.4.0/craft_application/launchpad/__init__.py` & `craft_application-2.5/craft_application/launchpad/__init__.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.4.0/craft_application/launchpad/errors.py` & `craft_application-2.5/craft_application/launchpad/errors.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.4.0/craft_application/launchpad/launchpad.py` & `craft_application-2.5/craft_application/launchpad/launchpad.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.4.0/craft_application/launchpad/models/__init__.py` & `craft_application-2.5/craft_application/launchpad/models/__init__.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.4.0/craft_application/launchpad/models/base.py` & `craft_application-2.5/craft_application/launchpad/models/base.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.4.0/craft_application/launchpad/models/build.py` & `craft_application-2.5/craft_application/launchpad/models/build.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.4.0/craft_application/launchpad/models/code.py` & `craft_application-2.5/craft_application/launchpad/models/code.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.4.0/craft_application/launchpad/models/distro.py` & `craft_application-2.5/craft_application/launchpad/models/distro.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.4.0/craft_application/launchpad/models/project.py` & `craft_application-2.5/craft_application/launchpad/models/project.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.4.0/craft_application/launchpad/models/recipe.py` & `craft_application-2.5/craft_application/launchpad/models/recipe.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.4.0/craft_application/launchpad/util.py` & `craft_application-2.5/craft_application/launchpad/util.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.4.0/craft_application/misc/instance_bashrc` & `craft_application-2.5/craft_application/misc/instance_bashrc`

 * *Files identical despite different names*

### Comparing `craft-application-2.4.0/craft_application/models/__init__.py` & `craft_application-2.5/craft_application/models/__init__.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.4.0/craft_application/models/base.py` & `craft_application-2.5/craft_application/models/base.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.4.0/craft_application/models/constraints.py` & `craft_application-2.5/craft_application/models/constraints.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.4.0/craft_application/models/metadata.py` & `craft_application-2.5/craft_application/models/metadata.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.4.0/craft_application/models/project.py` & `craft_application-2.5/craft_application/models/project.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.4.0/craft_application/remote/__init__.py` & `craft_application-2.5/craft_application/remote/__init__.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.4.0/craft_application/remote/errors.py` & `craft_application-2.5/craft_application/remote/errors.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.4.0/craft_application/remote/git.py` & `craft_application-2.5/craft_application/remote/git.py`

 * *Files 1% similar despite different names*

```diff
@@ -249,15 +249,18 @@
         logger.debug(
             "Pushing %r to remote %r with refspec %r.", ref, stripped_url, refspec
         )
 
         # temporarily call git directly due to libgit2 bug that unable to push
         # large repos using https. See https://github.com/libgit2/libgit2/issues/6385
         # and https://github.com/snapcore/snapcraft/issues/4478
-        cmd: list[str] = ["git", "push", remote_url, refspec, "--progress"]
+        # Force push in case this repository already exists. The repository is always
+        # going to exist solely for remote builds, so the only potential issue here is a
+        # race condition with multiple remote builds on the same machine.
+        cmd: list[str] = ["git", "push", "--force", remote_url, refspec, "--progress"]
         if push_tags:
             cmd.append("--tags")
 
         git_proc: subprocess.Popen[str] | None = None
         try:
             with subprocess.Popen(
                 cmd,
```

### Comparing `craft-application-2.4.0/craft_application/remote/utils.py` & `craft_application-2.5/craft_application/remote/utils.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.4.0/craft_application/remote/worktree.py` & `craft_application-2.5/craft_application/remote/worktree.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.4.0/craft_application/secrets.py` & `craft_application-2.5/craft_application/secrets.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.4.0/craft_application/services/__init__.py` & `craft_application-2.5/craft_application/services/__init__.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.4.0/craft_application/services/base.py` & `craft_application-2.5/craft_application/services/base.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.4.0/craft_application/services/lifecycle.py` & `craft_application-2.5/craft_application/services/lifecycle.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.4.0/craft_application/services/package.py` & `craft_application-2.5/craft_application/services/package.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.4.0/craft_application/services/provider.py` & `craft_application-2.5/craft_application/services/provider.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.4.0/craft_application/services/remotebuild.py` & `craft_application-2.5/craft_application/services/remotebuild.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,29 +12,36 @@
 #  See the GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """Service class for remote build commands."""
 from __future__ import annotations
 
+import contextlib
 import datetime
 import itertools
 import os
 import pathlib
 import time
 import urllib.parse
 from collections.abc import Collection, Iterable, Mapping
 from typing import TYPE_CHECKING, Any, cast
 from urllib import parse
 
 import craft_cli
+import launchpadlib.errors  # type: ignore[import-untyped]
 import platformdirs
 
 from craft_application import errors, launchpad, models
-from craft_application.remote import GitRepo, WorkTree, utils
+from craft_application.remote import (
+    GitRepo,
+    WorkTree,
+    check_git_repo_for_remote_build,
+    utils,
+)
 from craft_application.services import base
 
 if TYPE_CHECKING:  # pragma: no cover
     from craft_application import AppMetadata, ServiceFactory
 
 DEFAULT_POLL_INTERVAL = 30
 
@@ -111,18 +118,20 @@
         This method requires a project to be loaded.
         """
         if self._builds:
             raise ValueError("Cannot start builds if already running builds")
 
         project = cast(models.Project, self._services.project)
 
+        check_git_repo_for_remote_build(project_dir)
+
         self._name = utils.get_build_id(self._app.name, project.name, project_dir)
         self._lp_project = self._ensure_project()
-        _, self._repository = self._new_repository(project_dir)
-        self._recipe = self._new_recipe(
+        _, self._repository = self._ensure_repository(project_dir)
+        self._recipe = self._ensure_recipe(
             self._name, self._repository, architectures=architectures
         )
         self._check_timeout()
         self._builds = list(self._new_builds(self._recipe))
         self._is_setup = True
         return self._builds
 
@@ -245,23 +254,28 @@
             return self.lp.new_project(
                 name=f"{self.lp.username}-craft-remote-build",
                 title=f"*craft remote builds for {self.lp.username}",
                 display_name=f"{self.lp.username} remote builds",
                 summary=f"Automatically-generated project for housing {self.lp.username}'s remote builds in snapcraft, charmcraft, etc.",
             )
 
-    def _new_repository(
+    def _ensure_repository(
         self, project_dir: pathlib.Path
     ) -> tuple[WorkTree, launchpad.models.GitRepository]:
-        """Create a repository on the local machine and on Launchpad."""
+        """Create a repository on the local machine and ensure it's on Launchpad."""
         work_tree = WorkTree(self._app.name, self._name, project_dir)
         work_tree.init_repo()
-        lp_repository = launchpad.models.GitRepository.new(
-            self.lp, self._name, target=self._lp_project.name
-        )
+        try:
+            lp_repository = self.lp.new_repository(
+                self._name, project=self._lp_project.name
+            )
+        except launchpadlib.errors.HTTPError:
+            lp_repository = self.lp.get_repository(
+                name=self._name, project=self._lp_project.name
+            )
 
         token = lp_repository.get_access_token(
             f"{self._app.name} {self._app.version} remote build",
             expiry=datetime.datetime.now(tz=datetime.timezone.utc)
             + datetime.timedelta(seconds=300),
         )
         repo_url = parse.urlparse(str(lp_repository.git_https_url))
@@ -272,27 +286,45 @@
         local_repository = GitRepo(work_tree.repo_dir)
         local_repository.push_url(push_url.geturl(), "main")
 
         return work_tree, lp_repository
 
     def _get_repository(self) -> launchpad.models.GitRepository:
         """Get an existing repository on Launchpad."""
-        return launchpad.models.GitRepository.get(
-            self.lp, name=self._name, owner=self.lp.username
-        )
+        return self.lp.get_repository(name=self._name, owner=self.lp.username)
+
+    def _ensure_recipe(
+        self,
+        name: str,
+        repository: launchpad.models.GitRepository,
+        **kwargs: Any,  # noqa: ANN401
+    ) -> launchpad.models.Recipe:
+        """Get a recipe or create it if it doesn't exist."""
+        with contextlib.suppress(ValueError):  # Recipe doesn't exist
+            recipe = self._get_recipe()
+            recipe.delete()
+
+        return self._new_recipe(name, repository, **kwargs)
 
     def _new_recipe(
         self,
         name: str,
         repository: launchpad.models.GitRepository,
         **kwargs: Any,  # noqa: ANN401
     ) -> launchpad.models.Recipe:
-        """Create a new recipe."""
+        """Create a new recipe for the given repository."""
+        repository.lp_refresh()  # Prevents a race condition on new repositories.
+        git_ref = parse.urlparse(str(repository.git_https_url)).path + "/+ref/main"
         return self.RecipeClass.new(
-            self.lp, name, self.lp.username, git_ref=repository.git_https_url, **kwargs
+            self.lp,
+            name,
+            self.lp.username,
+            git_ref=git_ref,
+            project=self._lp_project.name,
+            **kwargs,
         )
 
     def _get_recipe(self) -> launchpad.models.Recipe:
         """Get a build for this application by its build ID.
 
         If an application's recipe class needs more than just the name and owner,
         this method and new_recipe should be overridden.
```

### Comparing `craft-application-2.4.0/craft_application/services/request.py` & `craft_application-2.5/craft_application/services/request.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.4.0/craft_application/services/service_factory.py` & `craft_application-2.5/craft_application/services/service_factory.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.4.0/craft_application/util/__init__.py` & `craft_application-2.5/craft_application/util/__init__.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.4.0/craft_application/util/callbacks.py` & `craft_application-2.5/craft_application/util/callbacks.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.4.0/craft_application/util/error_formatting.py` & `craft_application-2.5/craft_application/util/error_formatting.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.4.0/craft_application/util/logging.py` & `craft_application-2.5/craft_application/util/logging.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.4.0/craft_application/util/paths.py` & `craft_application-2.5/craft_application/util/paths.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.4.0/craft_application/util/platforms.py` & `craft_application-2.5/craft_application/util/platforms.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.4.0/craft_application/util/repositories.py` & `craft_application-2.5/craft_application/util/repositories.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.4.0/craft_application/util/snap_config.py` & `craft_application-2.5/craft_application/util/snap_config.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.4.0/craft_application/util/string.py` & `craft_application-2.5/craft_application/util/string.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.4.0/craft_application/util/yaml.py` & `craft_application-2.5/craft_application/util/yaml.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.4.0/craft_application.egg-info/PKG-INFO` & `craft_application-2.5/craft_application.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: craft-application
-Version: 2.4.0
+Version: 2.5.0
 Summary: A framework for *craft applications.
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.10
@@ -13,15 +13,15 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Requires-Python: >=3.10
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: craft-archives>=1.1.3
 Requires-Dist: craft-cli>=2.4.0
-Requires-Dist: craft-grammar>=1.1.1
+Requires-Dist: craft-grammar>=1.2.0
 Requires-Dist: craft-parts>=1.21.1
 Requires-Dist: craft-providers<2.0,>=1.20.0
 Requires-Dist: snap-helpers>=0.4.2
 Requires-Dist: platformdirs>=3.10
 Requires-Dist: pydantic<2.0,>=1.10
 Requires-Dist: pydantic-yaml<1.0
 Requires-Dist: pygit2<1.15.0,>=1.13.0
@@ -33,25 +33,25 @@
 Requires-Dist: coverage[toml]==7.4.4; extra == "dev"
 Requires-Dist: hypothesis>=6.0; extra == "dev"
 Requires-Dist: pyfakefs~=5.3; extra == "dev"
 Requires-Dist: pytest==8.1.1; extra == "dev"
 Requires-Dist: pytest-check==2.3.1; extra == "dev"
 Requires-Dist: pytest-cov==5.0.0; extra == "dev"
 Requires-Dist: pytest-mock==3.14.0; extra == "dev"
-Requires-Dist: pytest-rerunfailures==13.0; extra == "dev"
+Requires-Dist: pytest-rerunfailures==14.0; extra == "dev"
 Requires-Dist: pytest-time>=0.3.1; extra == "dev"
 Requires-Dist: responses~=0.25.0; extra == "dev"
 Requires-Dist: craft-application[remote]; extra == "dev"
 Provides-Extra: lint
 Requires-Dist: black~=24.0; extra == "lint"
 Requires-Dist: codespell[toml]==2.2.6; extra == "lint"
 Requires-Dist: yamllint==1.35.1; extra == "lint"
 Provides-Extra: types
 Requires-Dist: mypy[reports]==1.9.0; extra == "types"
-Requires-Dist: pyright==1.1.356; extra == "types"
+Requires-Dist: pyright==1.1.358; extra == "types"
 Requires-Dist: types-requests; extra == "types"
 Requires-Dist: types-urllib3; extra == "types"
 Provides-Extra: docs
 Requires-Dist: furo==2024.1.29; extra == "docs"
 Requires-Dist: sphinx<7.3,>=7.2.6; extra == "docs"
 Requires-Dist: sphinx-autobuild==2024.2.4; extra == "docs"
 Requires-Dist: sphinx-copybutton==0.5.2; extra == "docs"
```

### Comparing `craft-application-2.4.0/craft_application.egg-info/SOURCES.txt` & `craft_application-2.5/craft_application.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `craft-application-2.4.0/craft_application.egg-info/requires.txt` & `craft_application-2.5/craft_application.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 craft-archives>=1.1.3
 craft-cli>=2.4.0
-craft-grammar>=1.1.1
+craft-grammar>=1.2.0
 craft-parts>=1.21.1
 craft-providers<2.0,>=1.20.0
 snap-helpers>=0.4.2
 platformdirs>=3.10
 pydantic<2.0,>=1.10
 pydantic-yaml<1.0
 pygit2<1.15.0,>=1.13.0
@@ -20,15 +20,15 @@
 coverage[toml]==7.4.4
 hypothesis>=6.0
 pyfakefs~=5.3
 pytest==8.1.1
 pytest-check==2.3.1
 pytest-cov==5.0.0
 pytest-mock==3.14.0
-pytest-rerunfailures==13.0
+pytest-rerunfailures==14.0
 pytest-time>=0.3.1
 responses~=0.25.0
 craft-application[remote]
 
 [docs]
 furo==2024.1.29
 sphinx<7.3,>=7.2.6
@@ -45,10 +45,10 @@
 yamllint==1.35.1
 
 [remote]
 launchpadlib>=1.10.16
 
 [types]
 mypy[reports]==1.9.0
-pyright==1.1.356
+pyright==1.1.358
 types-requests
 types-urllib3
```

### Comparing `craft-application-2.4.0/docs/conf.py` & `craft_application-2.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.4.0/docs/index.rst` & `craft_application-2.5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `craft-application-2.4.0/pyproject.toml` & `craft_application-2.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
 name = "craft-application"
 description = "A framework for *craft applications."
 dynamic = ["version", "readme"]
 dependencies = [
     "craft-archives>=1.1.3",
     "craft-cli>=2.4.0",
-    "craft-grammar>=1.1.1",
+    "craft-grammar>=1.2.0",
     "craft-parts>=1.21.1",
     "craft-providers>=1.20.0,<2.0",
     "snap-helpers>=0.4.2",
     "platformdirs>=3.10",
     "pydantic>=1.10,<2.0",
     "pydantic-yaml<1.0",
     # Pygit2 and libgit2 need to match versions.
@@ -48,27 +48,27 @@
     "coverage[toml]==7.4.4",
     "hypothesis>=6.0",
     "pyfakefs~=5.3",
     "pytest==8.1.1",
     "pytest-check==2.3.1",
     "pytest-cov==5.0.0",
     "pytest-mock==3.14.0",
-    "pytest-rerunfailures==13.0",
+    "pytest-rerunfailures==14.0",
     "pytest-time>=0.3.1",
     "responses~=0.25.0",
     "craft-application[remote]"
 ]
 lint = [
     "black~=24.0",
     "codespell[toml]==2.2.6",
     "yamllint==1.35.1"
 ]
 types = [
     "mypy[reports]==1.9.0",
-    "pyright==1.1.356",
+    "pyright==1.1.358",
     "types-requests",
     "types-urllib3",
 ]
 docs = [
     "furo==2024.1.29",
     "sphinx>=7.2.6,<7.3",
     "sphinx-autobuild==2024.2.4",
@@ -80,15 +80,15 @@
 ]
 apt = [
     "python-apt>=2.4.0;sys_platform=='linux'"
 ]
 
 [build-system]
 requires = [
-    "setuptools==69.1.1",
+    "setuptools==69.4.0",
     "setuptools_scm[toml]>=7.1"
 ]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.dynamic]
 readme = {file = "README.rst"}
 
@@ -282,14 +282,17 @@
     "S103", # Allow `os.chmod` setting a permissive mask `0o555` on file or directory
     "S108", # Allow Probable insecure usage of temporary file or directory
     "PLR0913",  # Allow many arguments for test functions
     "PT004", # Allow fixtures that don't return anything to not start with underscores
 ]
 # isort leaves init files alone by default, this makes ruff ignore them too.
 "__init__.py" = ["I001"]
+# TODO: Revert this
+# https://github.com/canonical/craft-application/issues/306
+"tests/integration/launchpad/test_anonymous_access.py" = ["ERA001"]
 
 [tool.ruff.lint.pep8-naming]
 classmethod-decorators = [
     "pydantic.root_validator",
     "pydantic.validator",
 ]
```

### Comparing `craft-application-2.4.0/tests/conftest.py` & `craft_application-2.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.4.0/tests/integration/conftest.py` & `craft_application-2.5/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.4.0/tests/integration/launchpad/conftest.py` & `craft_application-2.5/tests/integration/launchpad/conftest.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.4.0/tests/integration/launchpad/test_anonymous_access.py` & `craft_application-2.5/tests/integration/launchpad/test_anonymous_access.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 """Tests for anonymous access."""
 
 import pytest
 from craft_application import launchpad
-from craft_application.launchpad import models
 
 
 def test_anonymous_login(tmp_path):
     cache_dir = tmp_path / "cache"
     assert not cache_dir.exists()
 
     launchpad.Launchpad.anonymous(
         "craft-application-integration-tests", root="staging", cache_dir=cache_dir
     )
 
     assert cache_dir.is_dir()
 
 
-def test_get_basic_items(anonymous_lp):
-    snapstore_server = anonymous_lp.get_project("snapstore-server")
-    assert snapstore_server.name == "snapstore-server"
-    assert snapstore_server.title == "Snap Store Server"
-
-    snap_recipes = list(models.SnapRecipe.find(anonymous_lp, owner="lengau"))
-    assert len(snap_recipes) > 0
-    for recipe in snap_recipes:
-        assert recipe.owner_name == "lengau"
+# TODO: Re-enable this
+# https://github.com/canonical/craft-application/issues/306
+# def test_get_basic_items(anonymous_lp):
+#     snapstore_server = anonymous_lp.get_project("snapstore-server")
+#     assert snapstore_server.name == "snapstore-server"
+#     assert snapstore_server.title == "Snap Store Server"
+#
+#     snap_recipes = list(models.SnapRecipe.find(anonymous_lp, owner="lengau"))
+#     assert len(snap_recipes) > 0
+#     for recipe in snap_recipes:
+#         assert recipe.owner_name == "lengau"
 
 
 @pytest.mark.parametrize(
     ("name", "path"),
     [
         ("python-apt", "~deity/python-apt/+git/python-apt"),
         ("charmcraft", "~charmcraft-team/charmcraft/+git/charmcraft"),
```

### Comparing `craft-application-2.4.0/tests/integration/services/test_lifecycle.py` & `craft_application-2.5/tests/integration/services/test_lifecycle.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.4.0/tests/integration/services/test_provider.py` & `craft_application-2.5/tests/integration/services/test_provider.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.4.0/tests/integration/services/test_remotebuild.py` & `craft_application-2.5/tests/integration/services/test_remotebuild.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.4.0/tests/integration/services/test_request.py` & `craft_application-2.5/tests/integration/services/test_request.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.4.0/tests/integration/services/test_service_factory.py` & `craft_application-2.5/tests/integration/services/test_service_factory.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.4.0/tests/integration/test_application.py` & `craft_application-2.5/tests/integration/test_application.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.4.0/tests/integration/test_version.py` & `craft_application-2.5/tests/integration/test_version.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.4.0/tests/unit/commands/test_base.py` & `craft_application-2.5/tests/unit/commands/test_base.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.4.0/tests/unit/commands/test_lifecycle.py` & `craft_application-2.5/tests/unit/commands/test_lifecycle.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.4.0/tests/unit/commands/test_other.py` & `craft_application-2.5/tests/unit/commands/test_other.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.4.0/tests/unit/conftest.py` & `craft_application-2.5/tests/unit/conftest.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.4.0/tests/unit/launchpad/conftest.py` & `craft_application-2.5/tests/unit/launchpad/conftest.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.4.0/tests/unit/launchpad/models/test_base.py` & `craft_application-2.5/tests/unit/launchpad/models/test_base.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.4.0/tests/unit/launchpad/models/test_code.py` & `craft_application-2.5/tests/unit/launchpad/models/test_code.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.4.0/tests/unit/launchpad/test_launchpad.py` & `craft_application-2.5/tests/unit/launchpad/test_launchpad.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.4.0/tests/unit/launchpad/test_util.py` & `craft_application-2.5/tests/unit/launchpad/test_util.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.4.0/tests/unit/models/test_constraints.py` & `craft_application-2.5/tests/unit/models/test_constraints.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.4.0/tests/unit/models/test_project.py` & `craft_application-2.5/tests/unit/models/test_project.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.4.0/tests/unit/remote/conftest.py` & `craft_application-2.5/tests/unit/remote/conftest.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.4.0/tests/unit/remote/test_errors.py` & `craft_application-2.5/tests/unit/remote/test_errors.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.4.0/tests/unit/remote/test_git.py` & `craft_application-2.5/tests/unit/remote/test_git.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.4.0/tests/unit/remote/test_utils.py` & `craft_application-2.5/tests/unit/remote/test_utils.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.4.0/tests/unit/remote/test_worktree.py` & `craft_application-2.5/tests/unit/remote/test_worktree.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.4.0/tests/unit/services/conftest.py` & `craft_application-2.5/tests/unit/services/conftest.py`

 * *Files 10% similar despite different names*

```diff
@@ -90,14 +90,24 @@
                     requestBuilds=get_mock_callable(
                         return_value=get_mock_lazr_collection(
                             [], status="Completed", builds=[]
                         )
                     ),
                 )
             ),
+            getByName=get_mock_callable(
+                return_value=get_mock_lazr_entry(
+                    "snap",
+                    requestBuilds=get_mock_callable(
+                        return_value=get_mock_lazr_collection(
+                            [], status="Completed", builds=[]
+                        )
+                    ),
+                ),
+            ),
         ),
     )
     return launchpad.Launchpad(app_metadata.name, lp)
 
 
 @pytest.fixture()
 def remote_build_service(app_metadata, fake_services, fake_launchpad):
```

### Comparing `craft-application-2.4.0/tests/unit/services/test_lifecycle.py` & `craft_application-2.5/tests/unit/services/test_lifecycle.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.4.0/tests/unit/services/test_package.py` & `craft_application-2.5/tests/unit/services/test_package.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.4.0/tests/unit/services/test_provider.py` & `craft_application-2.5/tests/unit/services/test_provider.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.4.0/tests/unit/services/test_remotebuild.py` & `craft_application-2.5/tests/unit/services/test_remotebuild.py`

 * *Files 13% similar despite different names*

```diff
@@ -14,19 +14,21 @@
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """Tests for the remote build service."""
 import datetime
 import pathlib
 from unittest import mock
 
+import launchpadlib.errors
 import lazr.restfulclient.errors
 import lazr.restfulclient.resource
 import pytest
 from craft_application import errors, launchpad
 from craft_application.remote import git
+from craft_application.remote.errors import RemoteBuildInvalidGitRepoError
 
 from tests.unit.services.conftest import (
     get_mock_callable,
 )
 
 
 @pytest.fixture()
@@ -111,29 +113,29 @@
     with pytest.raises(
         RuntimeError,
         match="Cannot check if the project is private before setting its name.",
     ):
         remote_build_service.is_project_private()
 
 
-def test_new_repository(
+def test_ensure_repository_creation(
     monkeypatch, tmp_path, remote_build_service, mock_lp_project, mock_push_url
 ):
     wrapped_repository = mock.Mock(
         spec=launchpad.models.GitRepository,
         git_https_url="https://git.launchpad.net/~user/+git/my_repo",
         **{"get_access_token.return_value": "super_secret_token"},
     )
     repository_new = mock.Mock(return_value=wrapped_repository)
     monkeypatch.setattr(launchpad.models.GitRepository, "new", repository_new)
     sentinel = tmp_path / "sentinel_file"
     sentinel.write_text("I am a sentinel file.")
     remote_build_service._lp_project = mock_lp_project
 
-    work_tree, lp_repository = remote_build_service._new_repository(tmp_path)
+    work_tree, lp_repository = remote_build_service._ensure_repository(tmp_path)
 
     assert (work_tree.repo_dir / "sentinel_file").read_text() == sentinel.read_text()
     mock_push_url.assert_called_once_with(
         "https://craft_test_user:super_secret_token@git.launchpad.net/~user/+git/my_repo",
         "main",
     )
     expiry = wrapped_repository.get_access_token.call_args.kwargs["expiry"]
@@ -143,14 +145,69 @@
     # the expiry time sent to Launchpad will have already expired and Launchpad
     # does not catch that. So instead we make sure thot even when using the easternmost
     # time zone the expiry time is still in the future.
     tz = datetime.timezone(datetime.timedelta(hours=14))
     assert expiry > datetime.datetime.now(tz=tz)
 
 
+def test_ensure_repository_already_exists(
+    monkeypatch, tmp_path, remote_build_service, mock_lp_project, mock_push_url
+):
+    monkeypatch.setattr(
+        launchpad.models.GitRepository,
+        "new",
+        mock.Mock(side_effect=launchpadlib.errors.Conflict("nope", "broken")),
+    )
+    wrapped_repository = mock.Mock(
+        spec=launchpad.models.GitRepository,
+        git_https_url="https://git.launchpad.net/~user/+git/my_repo",
+        **{"get_access_token.return_value": "super_secret_token"},
+    )
+    repository_get = mock.Mock(return_value=wrapped_repository)
+    monkeypatch.setattr(launchpad.models.GitRepository, "get", repository_get)
+    sentinel = tmp_path / "sentinel_file"
+    sentinel.write_text("I am a sentinel file.")
+    remote_build_service._lp_project = mock_lp_project
+    remote_build_service._name = "some-repo-name"
+
+    work_tree, lp_repository = remote_build_service._ensure_repository(tmp_path)
+
+    assert (work_tree.repo_dir / "sentinel_file").read_text() == sentinel.read_text()
+    mock_push_url.assert_called_once_with(
+        "https://craft_test_user:super_secret_token@git.launchpad.net/~user/+git/my_repo",
+        "main",
+    )
+    expiry = wrapped_repository.get_access_token.call_args.kwargs["expiry"]
+
+    # Ensure that we're getting a timezone-aware object in the method.
+    # This is here as a regression test because if you're in a timezone behind UTC
+    # the expiry time sent to Launchpad will have already expired and Launchpad
+    # does not catch that. So instead we make sure thot even when using the easternmost
+    # time zone the expiry time is still in the future.
+    tz = datetime.timezone(datetime.timedelta(hours=14))
+    assert expiry > datetime.datetime.now(tz=tz)
+
+
+def test_create_new_recipe(remote_build_service, mock_lp_project):
+    """Test that _new_recipe works correctly."""
+    remote_build_service._lp_project = mock_lp_project
+    remote_build_service.RecipeClass = mock.Mock()
+    repo = mock.Mock(git_https_url="https://localhost/~me/some-project/+git/my-repo")
+
+    remote_build_service._new_recipe("test-recipe", repo)
+
+    remote_build_service.RecipeClass.new.assert_called_once_with(
+        remote_build_service.lp,
+        "test-recipe",
+        "craft_test_user",
+        git_ref="/~me/some-project/+git/my-repo/+ref/main",
+        project="craft_test_user-craft-remote-build",
+    )
+
+
 def test_not_setup(remote_build_service):
     with pytest.raises(RuntimeError):
         all(remote_build_service.monitor_builds())
     with pytest.raises(RuntimeError):
         remote_build_service.fetch_logs(pathlib.Path())
     with pytest.raises(RuntimeError):
         remote_build_service.fetch_artifacts(pathlib.Path())
@@ -242,12 +299,21 @@
 @pytest.mark.parametrize("architectures", [["amd64"], None])
 @pytest.mark.usefixtures("mock_push_url")
 def test_new_build(
     tmp_path,
     remote_build_service,
     architectures,
 ):
+    git.GitRepo(tmp_path)
     remote_build_service.start_builds(tmp_path, architectures)
     remote_build_service.monitor_builds()
     remote_build_service.fetch_logs(tmp_path)
     remote_build_service.fetch_artifacts(tmp_path)
     remote_build_service.cleanup()
+
+
+def test_new_build_not_git_repo(
+    tmp_path,
+    remote_build_service,
+):
+    with pytest.raises(RemoteBuildInvalidGitRepoError):
+        remote_build_service.start_builds(tmp_path, None)
```

### Comparing `craft-application-2.4.0/tests/unit/services/test_repositories.py` & `craft_application-2.5/tests/unit/services/test_repositories.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.4.0/tests/unit/services/test_request.py` & `craft_application-2.5/tests/unit/services/test_request.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.4.0/tests/unit/services/test_service_factory.py` & `craft_application-2.5/tests/unit/services/test_service_factory.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.4.0/tests/unit/test_application.py` & `craft_application-2.5/tests/unit/test_application.py`

 * *Files 23% similar despite different names*

```diff
@@ -58,14 +58,243 @@
 name: myproject
 version: 1.0
 parts:
   mypart:
     plugin: nil
 """
 
+FULL_PROJECT_YAML = """
+name: myproject
+version: 1.0
+parts:
+  mypart:
+    plugin: nil
+    source: non-grammar-source
+    source-checksum: on-amd64-to-riscv64-checksum
+    source-branch: riscv64-branch
+    source-commit: riscv64-commit
+    source-depth: 1
+    source-subdir: riscv64-subdir
+    source-submodules:
+      - riscv64-submodules-1
+      - riscv64-submodules-2
+    source-tag: riscv64-tag
+    source-type: riscv64-type
+    disable-parallel: true
+    after:
+      - riscv64-after
+    organize:
+      riscv64-organize-1: riscv64-organize-2
+      riscv64-organize-3: riscv64-organize-4
+    overlay:
+      - riscv64-overlay-1
+      - riscv64-overlay-2
+    overlay-packages:
+      - riscv64-overlay-1
+      - riscv64-overlay-2
+    overlay-script: riscv64-overlay-script
+    stage:
+      - riscv64-stage-1
+      - riscv64-stage-2
+    stage-snaps:
+      - riscv64-snap-1
+      - riscv64-snap-2
+    stage-packages:
+      - riscv64-package-1
+      - riscv64-package-2
+    prime:
+      - riscv64-prime-1
+      - riscv64-prime-2
+    build-snaps:
+      - riscv64-snap-1
+      - riscv64-snap-2
+    build-packages:
+      - riscv64-package-1
+      - riscv64-package-2
+    build-environment:
+      - MY_VAR: riscv64-value
+      - MY_VAR2: riscv64-value2
+    build-attributes:
+      - rifcv64-attr-1
+      - rifcv64-attr-2
+    override-pull: riscv64-override-pull
+    override-build: riscv64-override-build
+    override-stage: riscv64-override-stage
+    override-prime: riscv64-override-prime
+    permissions:
+      - path: riscv64-perm-1
+        owner: 123
+        group: 123
+        mode: "777"
+      - path: riscv64-perm-2
+        owner: 456
+        group: 456
+        mode: "666"
+"""
+
+FULL_GRAMMAR_PROJECT_YAML = """
+name: myproject
+version: 1.0
+parts:
+  mypart:
+    plugin:
+      - on amd64 to riscv64: nil
+      - on amd64 to s390x: dump
+    source:
+      - on amd64 to s390x: on-amd64-to-s390x
+      - on amd64 to riscv64: on-amd64-to-riscv64
+    source-checksum:
+      - on amd64 to riscv64: on-amd64-to-riscv64-checksum
+      - on amd64 to s390x: on-amd64-to-s390x-checksum
+    source-branch:
+      - on amd64 to s390x: s390x-branch
+      - on amd64 to riscv64: riscv64-branch
+    source-commit:
+      - on amd64 to riscv64: riscv64-commit
+      - on amd64 to s390x: s390x-commit
+    source-depth:
+      - on amd64 to s390x: 2
+      - on amd64 to riscv64: 1
+    source-subdir:
+      - on amd64 to riscv64: riscv64-subdir
+      - on amd64 to s390x: s390x-subdir
+    source-submodules:
+      - on amd64 to s390x:
+          - s390x-submodules-1
+          - s390x-submodules-2
+      - on amd64 to riscv64:
+          - riscv64-submodules-1
+          - riscv64-submodules-2
+    source-tag:
+      - on amd64 to riscv64: riscv64-tag
+      - on amd64 to s390x: s390x-tag
+    source-type:
+      - on amd64 to s390x: s390x-type
+      - on amd64 to riscv64: riscv64-type
+    disable-parallel:
+      - on amd64 to riscv64: true
+      - on amd64 to s390x: false
+    after:
+      - on amd64 to s390x:
+        - s390x-after
+      - on amd64 to riscv64:
+        - riscv64-after
+    organize:
+        - on amd64 to riscv64:
+            riscv64-organize-1: riscv64-organize-2
+            riscv64-organize-3: riscv64-organize-4
+        - on amd64 to s390x:
+            s390x-organize-1: s390x-organize-2
+            s390x-organize-3: s390x-organize-4
+    overlay:
+      - on amd64 to s390x:
+        - s390x-overlay-1
+        - s390x-overlay-2
+      - on amd64 to riscv64:
+        - riscv64-overlay-1
+        - riscv64-overlay-2
+    overlay-packages:
+      - on amd64 to riscv64:
+        - riscv64-overlay-1
+        - riscv64-overlay-2
+      - on amd64 to s390x:
+        - s390x-overlay-1
+        - s390x-overlay-2
+    overlay-script:
+        - on amd64 to s390x: s390x-overlay-script
+        - on amd64 to riscv64: riscv64-overlay-script
+    stage:
+      - on amd64 to riscv64:
+        - riscv64-stage-1
+        - riscv64-stage-2
+      - on amd64 to s390x:
+        - s390x-stage-1
+        - s390x-stage-2
+    stage-snaps:
+      - on amd64 to s390x:
+        - s390x-snap-1
+        - s390x-snap-2
+      - on amd64 to riscv64:
+        - riscv64-snap-1
+        - riscv64-snap-2
+    stage-packages:
+      - on amd64 to riscv64:
+        - riscv64-package-1
+        - riscv64-package-2
+      - on amd64 to s390x:
+        - s390x-package-1
+        - s390x-package-2
+    prime:
+      - on amd64 to s390x:
+        - s390x-prime-1
+        - s390x-prime-2
+      - on amd64 to riscv64:
+        - riscv64-prime-1
+        - riscv64-prime-2
+    build-snaps:
+      - on amd64 to riscv64:
+        - riscv64-snap-1
+        - riscv64-snap-2
+      - on amd64 to s390x:
+        - s390x-snap-1
+        - s390x-snap-2
+    build-packages:
+      - on amd64 to s390x:
+        - s390x-package-1
+        - s390x-package-2
+      - on amd64 to riscv64:
+        - riscv64-package-1
+        - riscv64-package-2
+    build-environment:
+      - on amd64 to riscv64:
+          - MY_VAR: riscv64-value
+          - MY_VAR2: riscv64-value2
+      - on amd64 to s390x:
+          - MY_VAR: s390x-value
+          - MY_VAR2: s390x-value2
+    build-attributes:
+      - on amd64 to s390x:
+        - s390x-attr-1
+        - s390x-attr-2
+      - on amd64 to riscv64:
+        - rifcv64-attr-1
+        - rifcv64-attr-2
+    override-pull:
+      - on amd64 to riscv64: riscv64-override-pull
+      - on amd64 to s390x: s390x-override-pull
+    override-build:
+      - on amd64 to s390x: s390x-override-build
+      - on amd64 to riscv64: riscv64-override-build
+    override-stage:
+      - on amd64 to riscv64: riscv64-override-stage
+      - on amd64 to s390x: s390x-override-stage
+    override-prime:
+      - on amd64 to s390x: s390x-override-prime
+      - on amd64 to riscv64: riscv64-override-prime
+    permissions:
+      - on amd64 to riscv64:
+        - path: riscv64-perm-1
+          owner: 123
+          group: 123
+          mode: "777"
+        - path: riscv64-perm-2
+          owner: 456
+          group: 456
+          mode: "666"
+      - on amd64 to s390x:
+        - path: s390x-perm-1
+          owner: 123
+          group: 123
+          mode: "666"
+        - path: s390x-perm-2
+          owner: 456
+          group: 456
+          mode: "777"
+"""
+
 
 @pytest.mark.parametrize("summary", ["A summary", None])
 def test_app_metadata_post_init_correct(summary):
     app = application.AppMetadata("craft-application", summary)
 
     pytest_check.equal(app.version, craft_application.__version__)
     pytest_check.is_not_none(app.summary)
@@ -1099,15 +1328,15 @@
     assert (
         str(exc_info.value)
         == "Required field 'license' is not set and 'adopt-info' not used."
     )
 
 
 @pytest.fixture()
-def grammar_project(tmp_path):
+def grammar_project_mini(tmp_path):
     """A project that builds on amd64 to riscv64 and s390x."""
     contents = dedent(
         """\
     name: myproject
     version: 1.0
     parts:
       mypart:
@@ -1118,68 +1347,126 @@
     """
     )
     project_file = tmp_path / "testcraft.yaml"
     project_file.write_text(contents)
 
 
 @pytest.fixture()
+def non_grammar_project_full(tmp_path):
+    """A project that builds on amd64 to riscv64."""
+    project_file = tmp_path / "testcraft.yaml"
+    project_file.write_text(FULL_PROJECT_YAML)
+
+
+@pytest.fixture()
+def grammar_project_full(tmp_path):
+    """A project that builds on amd64 to riscv64 and s390x."""
+    project_file = tmp_path / "testcraft.yaml"
+    project_file.write_text(FULL_GRAMMAR_PROJECT_YAML)
+
+
+@pytest.fixture()
+def non_grammar_build_plan(mocker):
+    """A build plan to build on amd64 to riscv64."""
+    host_arch = "amd64"
+    base = util.get_host_base()
+    build_plan = [
+        models.BuildInfo(
+            "platform-riscv64",
+            host_arch,
+            "riscv64",
+            base,
+        )
+    ]
+
+    mocker.patch.object(MyBuildPlanner, "get_build_plan", return_value=build_plan)
+
+
+@pytest.fixture()
 def grammar_build_plan(mocker):
     """A build plan to build on amd64 to riscv64 and s390x."""
     host_arch = "amd64"
     base = util.get_host_base()
-    build_plan = []
-    for build_for in ("riscv64", "s390x"):
-        build_plan.append(
-            models.BuildInfo(
-                f"platform-{build_for}",
-                host_arch,
-                build_for,
-                base,
-            )
+    build_plan = [
+        models.BuildInfo(
+            f"platform-{build_for}",
+            host_arch,
+            build_for,
+            base,
         )
+        for build_for in ("riscv64", "s390x")
+    ]
 
     mocker.patch.object(MyBuildPlanner, "get_build_plan", return_value=build_plan)
 
 
 @pytest.fixture()
-def grammar_app(
+def grammar_app_mini(
+    tmp_path,
+    grammar_project_mini,  # noqa: ARG001
+    grammar_build_plan,  # noqa: ARG001
+    app_metadata,
+    fake_services,
+):
+    app = application.Application(app_metadata, fake_services)
+    app.project_dir = tmp_path
+
+    return app
+
+
+@pytest.fixture()
+def non_grammar_app_full(
     tmp_path,
-    grammar_project,  # noqa: ARG001
+    non_grammar_project_full,  # noqa: ARG001
+    non_grammar_build_plan,  # noqa: ARG001
+    app_metadata,
+    fake_services,
+):
+    app = application.Application(app_metadata, fake_services)
+    app.project_dir = tmp_path
+
+    return app
+
+
+@pytest.fixture()
+def grammar_app_full(
+    tmp_path,
+    grammar_project_full,  # noqa: ARG001
     grammar_build_plan,  # noqa: ARG001
     app_metadata,
     fake_services,
 ):
     app = application.Application(app_metadata, fake_services)
     app.project_dir = tmp_path
 
     return app
 
 
-def test_process_grammar_build_for(grammar_app):
+def test_process_grammar_build_for(grammar_app_mini):
     """Test that a provided build-for is used to process the grammar."""
-    project = grammar_app.get_project(build_for="s390x")
+    project = grammar_app_mini.get_project(build_for="s390x")
     assert project.parts["mypart"]["source"] == "on-amd64-to-s390x"
 
 
-def test_process_grammar_platform(grammar_app):
+def test_process_grammar_platform(grammar_app_mini):
     """Test that a provided platform is used to process the grammar."""
-    project = grammar_app.get_project(platform="platform-riscv64")
+    project = grammar_app_mini.get_project(platform="platform-riscv64")
     assert project.parts["mypart"]["source"] == "on-amd64-to-riscv64"
 
 
-def test_process_grammar_default(grammar_app):
+def test_process_grammar_default(grammar_app_mini):
     """Test that if nothing is provided the first BuildInfo is used by the grammar."""
-    project = grammar_app.get_project()
+    project = grammar_app_mini.get_project()
     assert project.parts["mypart"]["source"] == "on-amd64-to-riscv64"
 
 
-def test_process_grammar_no_match(grammar_app, mocker):
+def test_process_grammar_no_match(grammar_app_mini, mocker):
     """Test that if the build plan is empty, the grammar uses the host as target arch."""
     mocker.patch("craft_application.util.get_host_architecture", return_value="i386")
-    project = grammar_app.get_project()
+    project = grammar_app_mini.get_project()
     # "source" is empty because "i386" doesn't match any of the grammar statements.
     assert project.parts["mypart"]["source"] is None
 
 
 class FakePartitionsApplication(FakeApplication):
     """A partition using FakeApplication."""
 
@@ -1235,7 +1522,143 @@
     )
     assert project.parts["mypart"]["override-prime"] == dedent(
         f"""\
         touch {app.project_dir}/prime/default
         touch {app.project_dir}/partitions/mypartition/prime/partition
     """
     )
+
+
+@pytest.mark.usefixtures("enable_overlay")
+def test_process_non_grammar_full(non_grammar_app_full):
+    """Test that the non-grammar project is processed correctly.
+
+    The following fields are not included due to not able to be tested in this context:
+    - parse-info
+    """
+    project = non_grammar_app_full.get_project()
+    assert project.parts["mypart"]["plugin"] == "nil"
+    assert project.parts["mypart"]["source"] == "non-grammar-source"
+    assert project.parts["mypart"]["source-checksum"] == "on-amd64-to-riscv64-checksum"
+    assert project.parts["mypart"]["source-branch"] == "riscv64-branch"
+    assert project.parts["mypart"]["source-commit"] == "riscv64-commit"
+    assert project.parts["mypart"]["source-depth"] == 1
+    assert project.parts["mypart"]["source-subdir"] == "riscv64-subdir"
+    assert project.parts["mypart"]["source-submodules"] == [
+        "riscv64-submodules-1",
+        "riscv64-submodules-2",
+    ]
+    assert project.parts["mypart"]["source-tag"] == "riscv64-tag"
+    assert project.parts["mypart"]["source-type"] == "riscv64-type"
+    assert project.parts["mypart"]["disable-parallel"] is True
+    assert project.parts["mypart"]["after"] == ["riscv64-after"]
+    assert project.parts["mypart"]["organize"] == {
+        "riscv64-organize-1": "riscv64-organize-2",
+        "riscv64-organize-3": "riscv64-organize-4",
+    }
+    assert project.parts["mypart"]["overlay"] == [
+        "riscv64-overlay-1",
+        "riscv64-overlay-2",
+    ]
+    assert project.parts["mypart"]["overlay-script"] == "riscv64-overlay-script"
+    assert project.parts["mypart"]["stage"] == ["riscv64-stage-1", "riscv64-stage-2"]
+    assert project.parts["mypart"]["stage-snaps"] == [
+        "riscv64-snap-1",
+        "riscv64-snap-2",
+    ]
+    assert project.parts["mypart"]["stage-packages"] == [
+        "riscv64-package-1",
+        "riscv64-package-2",
+    ]
+    assert project.parts["mypart"]["prime"] == ["riscv64-prime-1", "riscv64-prime-2"]
+    assert project.parts["mypart"]["build-snaps"] == [
+        "riscv64-snap-1",
+        "riscv64-snap-2",
+    ]
+    assert project.parts["mypart"]["build-packages"] == [
+        "riscv64-package-1",
+        "riscv64-package-2",
+    ]
+    assert project.parts["mypart"]["build-environment"] == [
+        {"MY_VAR": "riscv64-value"},
+        {"MY_VAR2": "riscv64-value2"},
+    ]
+    assert project.parts["mypart"]["build-attributes"] == [
+        "rifcv64-attr-1",
+        "rifcv64-attr-2",
+    ]
+    assert project.parts["mypart"]["override-pull"] == "riscv64-override-pull"
+    assert project.parts["mypart"]["override-build"] == "riscv64-override-build"
+    assert project.parts["mypart"]["override-stage"] == "riscv64-override-stage"
+    assert project.parts["mypart"]["override-prime"] == "riscv64-override-prime"
+    assert project.parts["mypart"]["permissions"] == [
+        {"path": "riscv64-perm-1", "owner": 123, "group": 123, "mode": "777"},
+        {"path": "riscv64-perm-2", "owner": 456, "group": 456, "mode": "666"},
+    ]
+
+
+@pytest.mark.usefixtures("enable_overlay")
+def test_process_grammar_full(grammar_app_full):
+    """Test that the nearly all grammar is processed correctly.
+
+    The following fields are not included due to not able to be tested in this context:
+    - parse-info
+    """
+    project = grammar_app_full.get_project()
+    assert project.parts["mypart"]["plugin"] == "nil"
+    assert project.parts["mypart"]["source"] == "on-amd64-to-riscv64"
+    assert project.parts["mypart"]["source-checksum"] == "on-amd64-to-riscv64-checksum"
+    assert project.parts["mypart"]["source-branch"] == "riscv64-branch"
+    assert project.parts["mypart"]["source-commit"] == "riscv64-commit"
+    assert project.parts["mypart"]["source-depth"] == 1
+    assert project.parts["mypart"]["source-subdir"] == "riscv64-subdir"
+    assert project.parts["mypart"]["source-submodules"] == [
+        "riscv64-submodules-1",
+        "riscv64-submodules-2",
+    ]
+    assert project.parts["mypart"]["source-tag"] == "riscv64-tag"
+    assert project.parts["mypart"]["source-type"] == "riscv64-type"
+    assert project.parts["mypart"]["disable-parallel"] is True
+    assert project.parts["mypart"]["after"] == ["riscv64-after"]
+    assert project.parts["mypart"]["organize"] == {
+        "riscv64-organize-1": "riscv64-organize-2",
+        "riscv64-organize-3": "riscv64-organize-4",
+    }
+    assert project.parts["mypart"]["overlay"] == [
+        "riscv64-overlay-1",
+        "riscv64-overlay-2",
+    ]
+    assert project.parts["mypart"]["overlay-script"] == "riscv64-overlay-script"
+    assert project.parts["mypart"]["stage"] == ["riscv64-stage-1", "riscv64-stage-2"]
+    assert project.parts["mypart"]["stage-snaps"] == [
+        "riscv64-snap-1",
+        "riscv64-snap-2",
+    ]
+    assert project.parts["mypart"]["stage-packages"] == [
+        "riscv64-package-1",
+        "riscv64-package-2",
+    ]
+    assert project.parts["mypart"]["prime"] == ["riscv64-prime-1", "riscv64-prime-2"]
+    assert project.parts["mypart"]["build-snaps"] == [
+        "riscv64-snap-1",
+        "riscv64-snap-2",
+    ]
+    assert project.parts["mypart"]["build-packages"] == [
+        "riscv64-package-1",
+        "riscv64-package-2",
+    ]
+    assert project.parts["mypart"]["build-environment"] == [
+        {"MY_VAR": "riscv64-value"},
+        {"MY_VAR2": "riscv64-value2"},
+    ]
+    assert project.parts["mypart"]["build-attributes"] == [
+        "rifcv64-attr-1",
+        "rifcv64-attr-2",
+    ]
+    assert project.parts["mypart"]["override-pull"] == "riscv64-override-pull"
+    assert project.parts["mypart"]["override-build"] == "riscv64-override-build"
+    assert project.parts["mypart"]["override-stage"] == "riscv64-override-stage"
+    assert project.parts["mypart"]["override-prime"] == "riscv64-override-prime"
+    assert project.parts["mypart"]["permissions"] == [
+        {"path": "riscv64-perm-1", "owner": 123, "group": 123, "mode": "777"},
+        {"path": "riscv64-perm-2", "owner": 456, "group": 456, "mode": "666"},
+    ]
```

### Comparing `craft-application-2.4.0/tests/unit/test_errors.py` & `craft_application-2.5/tests/unit/test_errors.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.4.0/tests/unit/test_grammar.py` & `craft_application-2.5/tests/unit/test_grammar.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.4.0/tests/unit/test_secrets.py` & `craft_application-2.5/tests/unit/test_secrets.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.4.0/tests/unit/util/test_error_formatting.py` & `craft_application-2.5/tests/unit/util/test_error_formatting.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.4.0/tests/unit/util/test_logging.py` & `craft_application-2.5/tests/unit/util/test_logging.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.4.0/tests/unit/util/test_paths.py` & `craft_application-2.5/tests/unit/util/test_paths.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.4.0/tests/unit/util/test_snap_config.py` & `craft_application-2.5/tests/unit/util/test_snap_config.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.4.0/tests/unit/util/test_string.py` & `craft_application-2.5/tests/unit/util/test_string.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.4.0/tests/unit/util/test_yaml.py` & `craft_application-2.5/tests/unit/util/test_yaml.py`

 * *Files identical despite different names*

### Comparing `craft-application-2.4.0/tox.ini` & `craft_application-2.5/tox.ini`

 * *Files identical despite different names*

