# Comparing `tmp/datagouv_python-0.1.1.tar.gz` & `tmp/datagouv_python-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datagouv_python-0.1.1.tar", max compression
+gzip compressed data, was "datagouv_python-0.1.2.tar", max compression
```

## Comparing `datagouv_python-0.1.1.tar` & `datagouv_python-0.1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    35149 2024-04-13 15:20:42.145253 datagouv_python-0.1.1/LICENSE
--rw-r--r--   0        0        0     2112 2024-04-15 19:11:59.179304 datagouv_python-0.1.1/README.md
--rw-r--r--   0        0        0      283 2024-04-15 06:43:06.307169 datagouv_python-0.1.1/datagouv/__init__.py
--rw-r--r--   0        0        0        0 2024-04-15 06:37:03.712875 datagouv_python-0.1.1/datagouv/api_client/__init__.py
--rw-r--r--   0        0        0     1373 2024-04-15 19:12:30.887035 datagouv_python-0.1.1/datagouv/api_client/_data_requestor.py
--rw-r--r--   0        0        0      350 2024-04-15 06:37:24.354131 datagouv_python-0.1.1/datagouv/api_client/_datagouv_client.py
--rw-r--r--   0        0        0     1607 2024-04-15 19:08:41.405368 datagouv_python-0.1.1/datagouv/api_client/_datasets_service.py
--rw-r--r--   0        0        0        0 2024-04-15 06:20:34.551164 datagouv_python-0.1.1/datagouv/downloader/__init__.py
--rw-r--r--   0        0        0      912 2024-04-15 18:45:33.019203 datagouv_python-0.1.1/datagouv/downloader/_resources_downloader.py
--rw-r--r--   0        0        0      767 2024-04-15 07:00:51.087557 datagouv_python-0.1.1/datagouv/downloader/_utils.py
--rw-r--r--   0        0        0      131 2024-04-14 15:05:59.938086 datagouv_python-0.1.1/datagouv/main.py
--rw-r--r--   0        0        0      467 2024-04-15 19:14:44.735850 datagouv_python-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2832 1970-01-01 00:00:00.000000 datagouv_python-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-13 15:20:42.145253 datagouv_python-0.1.2/LICENSE
+-rw-r--r--   0        0        0     2494 2024-04-16 18:34:19.846826 datagouv_python-0.1.2/README.md
+-rw-r--r--   0        0        0      283 2024-04-15 06:43:06.307169 datagouv_python-0.1.2/datagouv/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-15 06:37:03.712875 datagouv_python-0.1.2/datagouv/api_client/__init__.py
+-rw-r--r--   0        0        0     1373 2024-04-15 19:12:30.887035 datagouv_python-0.1.2/datagouv/api_client/_data_requestor.py
+-rw-r--r--   0        0        0      350 2024-04-15 06:37:24.354131 datagouv_python-0.1.2/datagouv/api_client/_datagouv_client.py
+-rw-r--r--   0        0        0     1607 2024-04-15 19:08:41.405368 datagouv_python-0.1.2/datagouv/api_client/_datasets_service.py
+-rw-r--r--   0        0        0        0 2024-04-15 06:20:34.551164 datagouv_python-0.1.2/datagouv/downloader/__init__.py
+-rw-r--r--   0        0        0      912 2024-04-15 18:45:33.019203 datagouv_python-0.1.2/datagouv/downloader/_resources_downloader.py
+-rw-r--r--   0        0        0      767 2024-04-15 07:00:51.087557 datagouv_python-0.1.2/datagouv/downloader/_utils.py
+-rw-r--r--   0        0        0      131 2024-04-14 15:05:59.938086 datagouv_python-0.1.2/datagouv/main.py
+-rw-r--r--   0        0        0      682 2024-04-16 18:40:24.082024 datagouv_python-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3354 1970-01-01 00:00:00.000000 datagouv_python-0.1.2/PKG-INFO
```

### Comparing `datagouv_python-0.1.1/LICENSE` & `datagouv_python-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `datagouv_python-0.1.1/README.md` & `datagouv_python-0.1.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 # datagouv-python
 
+[![PyPI version](https://badge.fury.io/py/datagouv-python.svg)](https://badge.fury.io/py/datagouv-python)
+[![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)](https://github.com/MaximePawlakFr/datagouv-python)
+
 Unofficial python client for `data.gouv.fr`.
 
 Official documentation is here: https://guides.data.gouv.fr/guide-data.gouv.fr/api/reference.
 
 Current API version supported = "1".
 
 # Getting Started
@@ -38,71 +41,79 @@
 # Instanciate ResourcesDownloader
 downloader = ResourcesDownloader(dataset_id)
 
 # Download to current directory
 downloader.download()
 ```
 
-
+---
 
 # Development
 
 ```
 poetry run start
 poetry run black datagouv/
 poetry run flake8
 ```
 
-## Build
+## Build and Publish
 
-### Process
+### Steps
 
 ```bash
 poetry version [patch, minor, major]
 poetry install
 poetry build
 # Update CHANGELOG
 git commit -m "vX.X.X"
 git tag vX.X.X
-poetry deploy
+poetry publish
+git push --tags
+git push
 ```
 
-### Details
-```
+### Commands
+```bash
+poetry add pytest --group dev
+
 poetry version
 poetry version -s
 
 poetry version [patch, minor, major]
 ```
 
-```
+```bash
 poetry build
 ```
 
-https://pypi.org/project/datagouv-python/
 
 <!-- 
 ```
 python -m build
 
 python -m twine upload --config-file .pypirc -r testpypi dist/*
 python -m twine upload --config-file .pypirc -r pypi dist/*
 ``` -->
 
-## Publish
-```
+#### Config 
+```bash
+# test-pypi
 poetry config repositories.test-pypi https://test.pypi.org/legacy/
 poetry config pypi-token.test-pypi MY_TOKEN
-poetry config pypi-token.pypi MY_TOKEN
-```
-```
+
 poetry publish -r test-pypi 
+
+# pypi
+poetry config pypi-token.pypi MY_TOKEN
 poetry publish
 ```
 
+# Resources
+* https://pypi.org/project/datagouv-python/
+
 # Roadmap
 
 * [ ] Handle /datasets routes
 * [ ] Handle other routes
     * /site
     * /reuses
     * /discussions
```

### Comparing `datagouv_python-0.1.1/datagouv/api_client/_data_requestor.py` & `datagouv_python-0.1.2/datagouv/api_client/_data_requestor.py`

 * *Files identical despite different names*

### Comparing `datagouv_python-0.1.1/datagouv/api_client/_datasets_service.py` & `datagouv_python-0.1.2/datagouv/api_client/_datasets_service.py`

 * *Files identical despite different names*

### Comparing `datagouv_python-0.1.1/datagouv/downloader/_resources_downloader.py` & `datagouv_python-0.1.2/datagouv/downloader/_resources_downloader.py`

 * *Files identical despite different names*

### Comparing `datagouv_python-0.1.1/datagouv/downloader/_utils.py` & `datagouv_python-0.1.2/datagouv/downloader/_utils.py`

 * *Files identical despite different names*

### Comparing `datagouv_python-0.1.1/PKG-INFO` & `datagouv_python-0.1.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 Metadata-Version: 2.1
 Name: datagouv-python
-Version: 0.1.1
-Summary: 
+Version: 0.1.2
+Summary: Unofficial python client for `data.gouv.fr`
+Home-page: https://github.com/MaximePawlakFr/datagouv-python
 License: GPL-3.0-or-later
+Keywords: open-data,opendata,government
 Author: Maxime Pawlak
 Author-email: maxime.pawlak@amatek.fr
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: black (>=24.4.0,<25.0.0)
-Requires-Dist: flake8 (>=7.0.0,<8.0.0)
 Requires-Dist: pandas (>=2.0.0,<3.0.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
+Project-URL: Repository, https://github.com/MaximePawlakFr/datagouv-python
 Description-Content-Type: text/markdown
 
 # datagouv-python
 
+[![PyPI version](https://badge.fury.io/py/datagouv-python.svg)](https://badge.fury.io/py/datagouv-python)
+[![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)](https://github.com/MaximePawlakFr/datagouv-python)
+
 Unofficial python client for `data.gouv.fr`.
 
 Official documentation is here: https://guides.data.gouv.fr/guide-data.gouv.fr/api/reference.
 
 Current API version supported = "1".
 
 # Getting Started
@@ -58,71 +62,79 @@
 # Instanciate ResourcesDownloader
 downloader = ResourcesDownloader(dataset_id)
 
 # Download to current directory
 downloader.download()
 ```
 
-
+---
 
 # Development
 
 ```
 poetry run start
 poetry run black datagouv/
 poetry run flake8
 ```
 
-## Build
+## Build and Publish
 
-### Process
+### Steps
 
 ```bash
 poetry version [patch, minor, major]
 poetry install
 poetry build
 # Update CHANGELOG
 git commit -m "vX.X.X"
 git tag vX.X.X
-poetry deploy
+poetry publish
+git push --tags
+git push
 ```
 
-### Details
-```
+### Commands
+```bash
+poetry add pytest --group dev
+
 poetry version
 poetry version -s
 
 poetry version [patch, minor, major]
 ```
 
-```
+```bash
 poetry build
 ```
 
-https://pypi.org/project/datagouv-python/
 
 <!-- 
 ```
 python -m build
 
 python -m twine upload --config-file .pypirc -r testpypi dist/*
 python -m twine upload --config-file .pypirc -r pypi dist/*
 ``` -->
 
-## Publish
-```
+#### Config 
+```bash
+# test-pypi
 poetry config repositories.test-pypi https://test.pypi.org/legacy/
 poetry config pypi-token.test-pypi MY_TOKEN
-poetry config pypi-token.pypi MY_TOKEN
-```
-```
+
 poetry publish -r test-pypi 
+
+# pypi
+poetry config pypi-token.pypi MY_TOKEN
 poetry publish
 ```
 
+# Resources
+* https://pypi.org/project/datagouv-python/
+
 # Roadmap
 
 * [ ] Handle /datasets routes
 * [ ] Handle other routes
     * /site
     * /reuses
     * /discussions
```

