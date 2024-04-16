# Comparing `tmp/acslib-0.1.4.tar.gz` & `tmp/acslib-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acslib-0.1.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "acslib-0.1.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `acslib-0.1.4.tar` & `acslib-0.1.6.tar`

### file list

```diff
@@ -1,53 +1,54 @@
--rw-r--r--   0        0        0      163 2024-04-10 13:51:14.379070 acslib-0.1.4/.coveragerc
--rw-r--r--   0        0        0      104 2024-04-10 13:51:14.379070 acslib-0.1.4/.dockerignore
--rw-r--r--   0        0        0      292 2024-04-10 13:51:14.379070 acslib-0.1.4/.editorconfig
--rw-r--r--   0        0        0      296 2024-04-10 13:51:14.379070 acslib-0.1.4/.github/pr_template.md
--rw-r--r--   0        0        0     9158 2024-04-10 13:51:14.379070 acslib-0.1.4/.github/workflows/test_publish_release..yml
--rw-r--r--   0        0        0     1388 2024-04-10 13:51:14.379070 acslib-0.1.4/.gitignore
--rw-r--r--   0        0        0       81 2024-04-10 13:51:14.379070 acslib-0.1.4/.isort.cfg
--rw-r--r--   0        0        0      875 2024-04-10 13:51:14.379070 acslib-0.1.4/.pre-commit-config.yaml
--rw-r--r--   0        0        0      118 2024-04-10 13:51:14.379070 acslib-0.1.4/AUTHORS.md
--rw-r--r--   0        0        0      212 2024-04-10 13:51:14.379070 acslib-0.1.4/CONTRIBUTING.md
--rw-r--r--   0        0        0      473 2024-04-10 13:51:14.379070 acslib-0.1.4/Dockerfile
--rw-r--r--   0        0        0       59 2024-04-10 13:51:14.379070 acslib-0.1.4/HISTORY.md
--rw-r--r--   0        0        0     1089 2024-04-10 13:51:14.379070 acslib-0.1.4/LICENSE
--rw-r--r--   0        0        0      589 2024-04-10 13:51:14.379070 acslib-0.1.4/Makefile
--rw-r--r--   0        0        0     4455 2024-04-10 13:51:14.379070 acslib-0.1.4/README.md
--rw-r--r--   0        0        0      188 2024-04-10 13:51:14.379070 acslib-0.1.4/acslib/__init__.py
--rw-r--r--   0        0        0      218 2024-04-10 13:51:14.379070 acslib-0.1.4/acslib/base/__init__.py
--rw-r--r--   0        0        0      259 2024-04-10 13:51:14.379070 acslib-0.1.4/acslib/base/acs.py
--rw-r--r--   0        0        0      172 2024-04-10 13:51:14.379070 acslib-0.1.4/acslib/base/config.py
--rw-r--r--   0        0        0     6294 2024-04-10 13:51:14.379070 acslib-0.1.4/acslib/base/connection.py
--rw-r--r--   0        0        0      272 2024-04-10 13:51:14.379070 acslib-0.1.4/acslib/base/search.py
--rw-r--r--   0        0        0     6113 2024-04-10 13:51:14.379070 acslib-0.1.4/acslib/base/status.py
--rw-r--r--   0        0        0      322 2024-04-10 13:51:14.379070 acslib-0.1.4/acslib/ccure/__init__.py
--rw-r--r--   0        0        0      595 2024-04-10 13:51:14.379070 acslib-0.1.4/acslib/ccure/base.py
--rw-r--r--   0        0        0     2923 2024-04-10 13:51:14.379070 acslib-0.1.4/acslib/ccure/config.py
--rw-r--r--   0        0        0     7444 2024-04-10 13:51:14.379070 acslib-0.1.4/acslib/ccure/connection.py
--rw-r--r--   0        0        0    13405 2024-04-10 13:51:14.379070 acslib-0.1.4/acslib/ccure/crud.py
--rw-r--r--   0        0        0     1015 2024-04-10 13:51:14.379070 acslib-0.1.4/acslib/ccure/endpoints.py
--rw-r--r--   0        0        0     7674 2024-04-10 13:51:14.379070 acslib-0.1.4/acslib/ccure/filters.py
--rw-r--r--   0        0        0       36 2024-04-10 13:51:14.379070 acslib-0.1.4/acslib/ccure/tests/__init__.py
--rw-r--r--   0        0        0     1839 2024-04-10 13:51:14.379070 acslib-0.1.4/acslib/ccure/tests/conftest.py
--rw-r--r--   0        0        0     2037 2024-04-10 13:51:14.379070 acslib-0.1.4/acslib/ccure/tests/test_base.py
--rw-r--r--   0        0        0     2801 2024-04-10 13:51:14.379070 acslib-0.1.4/acslib/ccure/tests/test_config.py
--rw-r--r--   0        0        0     2111 2024-04-10 13:51:14.379070 acslib-0.1.4/acslib/ccure/tests/test_connection.py
--rw-r--r--   0        0        0     2588 2024-04-10 13:51:14.379070 acslib-0.1.4/acslib/ccure/tests/test_search.py
--rw-r--r--   0        0        0     1138 2024-04-10 13:51:14.379070 acslib-0.1.4/acslib/ccure/types.py
--rw-r--r--   0        0        0       11 2024-04-10 13:51:14.379070 acslib-0.1.4/docs/api.md
--rw-r--r--   0        0        0       41 2024-04-10 13:51:14.379070 acslib-0.1.4/docs/authors.md
--rw-r--r--   0        0        0       46 2024-04-10 13:51:14.379070 acslib-0.1.4/docs/contributing.md
--rw-r--r--   0        0        0       41 2024-04-10 13:51:14.379070 acslib-0.1.4/docs/history.md
--rw-r--r--   0        0        0       42 2024-04-10 13:51:14.379070 acslib-0.1.4/docs/index.md
--rw-r--r--   0        0        0     1188 2024-04-10 13:51:14.379070 acslib-0.1.4/docs/installation.md
--rw-r--r--   0        0        0       87 2024-04-10 13:51:14.379070 acslib-0.1.4/docs/usage.md
--rw-r--r--   0        0        0       20 2024-04-10 13:51:14.379070 acslib-0.1.4/envrc_sample
--rw-r--r--   0        0        0     1949 2024-04-10 13:51:14.379070 acslib-0.1.4/mkdocs.yml
--rw-r--r--   0        0        0     1918 2024-04-10 13:51:14.379070 acslib-0.1.4/notebooks/.ipynb_checkpoints/encode_investigation-checkpoint
--rw-r--r--   0        0        0     2314 2024-04-10 13:51:14.379070 acslib-0.1.4/notebooks/.ipynb_checkpoints/encode_investigation-checkpoint.ipynb
--rw-r--r--   0        0        0    12624 2024-04-10 13:51:14.379070 acslib-0.1.4/notebooks/encode_investigation.ipynb
--rw-r--r--   0        0        0     2699 2024-04-10 13:51:14.379070 acslib-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      219 2024-04-10 13:51:14.379070 acslib-0.1.4/pytest.ini
--rw-r--r--   0        0        0      926 2024-04-10 13:51:14.379070 acslib-0.1.4/requirements/base/base.txt
--rw-r--r--   0        0        0     4618 2024-04-10 13:51:14.379070 acslib-0.1.4/requirements/dev/dev.txt
--rw-r--r--   0        0        0     6040 1970-01-01 00:00:00.000000 acslib-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      163 2024-04-16 13:04:12.660568 acslib-0.1.6/.coveragerc
+-rw-r--r--   0        0        0      104 2024-04-16 13:04:12.660568 acslib-0.1.6/.dockerignore
+-rw-r--r--   0        0        0      292 2024-04-16 13:04:12.660568 acslib-0.1.6/.editorconfig
+-rw-r--r--   0        0        0      296 2024-04-16 13:04:12.660568 acslib-0.1.6/.github/pr_template.md
+-rw-r--r--   0        0        0     9382 2024-04-16 13:04:12.660568 acslib-0.1.6/.github/workflows/test_publish_release..yml
+-rw-r--r--   0        0        0     1388 2024-04-16 13:04:12.660568 acslib-0.1.6/.gitignore
+-rw-r--r--   0        0        0       81 2024-04-16 13:04:12.660568 acslib-0.1.6/.isort.cfg
+-rw-r--r--   0        0        0      875 2024-04-16 13:04:12.660568 acslib-0.1.6/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      118 2024-04-16 13:04:12.660568 acslib-0.1.6/AUTHORS.md
+-rw-r--r--   0        0        0      212 2024-04-16 13:04:12.660568 acslib-0.1.6/CONTRIBUTING.md
+-rw-r--r--   0        0        0      473 2024-04-16 13:04:12.660568 acslib-0.1.6/Dockerfile
+-rw-r--r--   0        0        0       59 2024-04-16 13:04:12.660568 acslib-0.1.6/HISTORY.md
+-rw-r--r--   0        0        0     1089 2024-04-16 13:04:12.660568 acslib-0.1.6/LICENSE
+-rw-r--r--   0        0        0      589 2024-04-16 13:04:12.660568 acslib-0.1.6/Makefile
+-rw-r--r--   0        0        0     5171 2024-04-16 13:04:12.660568 acslib-0.1.6/README.md
+-rw-r--r--   0        0        0      188 2024-04-16 13:04:12.660568 acslib-0.1.6/acslib/__init__.py
+-rw-r--r--   0        0        0      218 2024-04-16 13:04:12.660568 acslib-0.1.6/acslib/base/__init__.py
+-rw-r--r--   0        0        0      259 2024-04-16 13:04:12.660568 acslib-0.1.6/acslib/base/acs.py
+-rw-r--r--   0        0        0      172 2024-04-16 13:04:12.660568 acslib-0.1.6/acslib/base/config.py
+-rw-r--r--   0        0        0     6294 2024-04-16 13:04:12.660568 acslib-0.1.6/acslib/base/connection.py
+-rw-r--r--   0        0        0      272 2024-04-16 13:04:12.660568 acslib-0.1.6/acslib/base/search.py
+-rw-r--r--   0        0        0     6113 2024-04-16 13:04:12.660568 acslib-0.1.6/acslib/base/status.py
+-rw-r--r--   0        0        0      322 2024-04-16 13:04:12.660568 acslib-0.1.6/acslib/ccure/__init__.py
+-rw-r--r--   0        0        0      595 2024-04-16 13:04:12.660568 acslib-0.1.6/acslib/ccure/base.py
+-rw-r--r--   0        0        0     2923 2024-04-16 13:04:12.660568 acslib-0.1.6/acslib/ccure/config.py
+-rw-r--r--   0        0        0     7444 2024-04-16 13:04:12.660568 acslib-0.1.6/acslib/ccure/connection.py
+-rw-r--r--   0        0        0    17177 2024-04-16 13:04:12.660568 acslib-0.1.6/acslib/ccure/crud.py
+-rw-r--r--   0        0        0     1070 2024-04-16 13:04:12.660568 acslib-0.1.6/acslib/ccure/data_models.py
+-rw-r--r--   0        0        0     1141 2024-04-16 13:04:12.660568 acslib-0.1.6/acslib/ccure/endpoints.py
+-rw-r--r--   0        0        0     7674 2024-04-16 13:04:12.660568 acslib-0.1.6/acslib/ccure/filters.py
+-rw-r--r--   0        0        0       36 2024-04-16 13:04:12.660568 acslib-0.1.6/acslib/ccure/tests/__init__.py
+-rw-r--r--   0        0        0     1839 2024-04-16 13:04:12.660568 acslib-0.1.6/acslib/ccure/tests/conftest.py
+-rw-r--r--   0        0        0     2037 2024-04-16 13:04:12.660568 acslib-0.1.6/acslib/ccure/tests/test_base.py
+-rw-r--r--   0        0        0     2801 2024-04-16 13:04:12.660568 acslib-0.1.6/acslib/ccure/tests/test_config.py
+-rw-r--r--   0        0        0     2111 2024-04-16 13:04:12.660568 acslib-0.1.6/acslib/ccure/tests/test_connection.py
+-rw-r--r--   0        0        0     2588 2024-04-16 13:04:12.660568 acslib-0.1.6/acslib/ccure/tests/test_search.py
+-rw-r--r--   0        0        0      348 2024-04-16 13:04:12.660568 acslib-0.1.6/acslib/ccure/types.py
+-rw-r--r--   0        0        0       11 2024-04-16 13:04:12.660568 acslib-0.1.6/docs/api.md
+-rw-r--r--   0        0        0       41 2024-04-16 13:04:12.660568 acslib-0.1.6/docs/authors.md
+-rw-r--r--   0        0        0       46 2024-04-16 13:04:12.660568 acslib-0.1.6/docs/contributing.md
+-rw-r--r--   0        0        0       41 2024-04-16 13:04:12.660568 acslib-0.1.6/docs/history.md
+-rw-r--r--   0        0        0       42 2024-04-16 13:04:12.660568 acslib-0.1.6/docs/index.md
+-rw-r--r--   0        0        0     1188 2024-04-16 13:04:12.660568 acslib-0.1.6/docs/installation.md
+-rw-r--r--   0        0        0       87 2024-04-16 13:04:12.664568 acslib-0.1.6/docs/usage.md
+-rw-r--r--   0        0        0       20 2024-04-16 13:04:12.664568 acslib-0.1.6/envrc_sample
+-rw-r--r--   0        0        0     1949 2024-04-16 13:04:12.664568 acslib-0.1.6/mkdocs.yml
+-rw-r--r--   0        0        0     1918 2024-04-16 13:04:12.664568 acslib-0.1.6/notebooks/.ipynb_checkpoints/encode_investigation-checkpoint
+-rw-r--r--   0        0        0     2314 2024-04-16 13:04:12.664568 acslib-0.1.6/notebooks/.ipynb_checkpoints/encode_investigation-checkpoint.ipynb
+-rw-r--r--   0        0        0    12624 2024-04-16 13:04:12.664568 acslib-0.1.6/notebooks/encode_investigation.ipynb
+-rw-r--r--   0        0        0     2699 2024-04-16 13:04:12.664568 acslib-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      219 2024-04-16 13:04:12.664568 acslib-0.1.6/pytest.ini
+-rw-r--r--   0        0        0      926 2024-04-16 13:04:12.664568 acslib-0.1.6/requirements/base/base.txt
+-rw-r--r--   0        0        0     4618 2024-04-16 13:04:12.664568 acslib-0.1.6/requirements/dev/dev.txt
+-rw-r--r--   0        0        0     6756 1970-01-01 00:00:00.000000 acslib-0.1.6/PKG-INFO
```

### Comparing `acslib-0.1.4/.github/workflows/test_publish_release..yml` & `acslib-0.1.6/.github/workflows/test_publish_release..yml`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
   workflow_dispatch:
 
 env:
     REPO_NAME: acslib
     RELEASE_REPO: https://github.com/ncstate-sat/acslib
     SLACK_UPDATES: true
     # sends notifications to the clearance slack channel
-    SLACK_CHANNEL_ID: C062CVCCTGW
+    SLACK_CHANNEL_ID: ${{ secrets.ACSLIB_CHANNEL_ID }}
     FLIT_USERNAME: __token__
     FLIT_PASSWORD: ${{ secrets.PYPI_TOKEN }}
 
 jobs:
   run_tests:
     name: Run Tests
     runs-on: ubuntu-latest
@@ -107,18 +107,20 @@
       - name: Retrieve previous version
         run: |
           PREV_VERSION=$(git describe --tags `git rev-list --tags --max-count=1`)
           echo "PREV_VERSION=${PREV_VERSION}" >> $GITHUB_ENV
           echo "PREV_VERSION_NUM=${PREV_VERSION:1}" >> $GITHUB_ENV
 
       - name: Check if version has been updated
-        # bash function checks if the first variable is less than the second one using version-sort
+        # first bash function checks if the first variable is less than or equal to the second one using version-sort
+        # second function uses the first to check if the first is strictly less than the second
         run: |
-          updated() { [  "$1" = "`echo -e "$1\n$2" | sort -V | head -n1`" ]; }
-          updated $PREV_VERSION_NUM $CURRENT_VERSION_NUM && echo "UPDATED=true" >> $GITHUB_ENV || echo "UPDATED=false" >> $GITHUB_ENV
+          verlte() { [  "$1" = "`echo -e "$1\n$2" | sort -V | head -n1`" ]; }
+          verlt() { [ "$1" = "$2" ] && return 1 || verlte $1 $2; }
+          verlt $PREV_VERSION_NUM $CURRENT_VERSION_NUM && echo "UPDATED=true" >> $GITHUB_ENV || echo "UPDATED=false" >> $GITHUB_ENV
 
       - name: Fail if version has not been updated
         if: ${{ !fromJSON(env.UPDATED) }}
         run: |
           echo "Version in pyproject.toml has not been updated"
           exit 1
 
@@ -185,14 +187,15 @@
       PR_BODY: ${{ github.event.pull_request.body }}
       LATEST_COMMIT_MESSAGE: ${{ github.event.head_commit.message }}
     steps:
       - name: Get Code
         uses: actions/checkout@v3
         with:
           ref: ${{ github.head_ref }}
+          fetch-depth: 0
           fetch-tags: true
 
       - name: Get SAT Actions
         uses: actions/checkout@v3
         with:
           repository: ncstate-sat/actions
           path: actions
```

### Comparing `acslib-0.1.4/.gitignore` & `acslib-0.1.6/.gitignore`

 * *Files identical despite different names*

### Comparing `acslib-0.1.4/.pre-commit-config.yaml` & `acslib-0.1.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `acslib-0.1.4/LICENSE` & `acslib-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `acslib-0.1.4/Makefile` & `acslib-0.1.6/Makefile`

 * *Files identical despite different names*

### Comparing `acslib-0.1.4/README.md` & `acslib-0.1.6/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -47,14 +47,45 @@
 from acslib.ccure.filters import PersonnelFilter, FUZZ
 
 ccure_api = CcureAPI()
 search_filter = PersonnelFilter(lookups={"Text1": FUZZ})
 response = ccure_api.personnel.search(["PER0892347"], search_filter=search_filter)
 ```
 
+#### Update a personnel record
+
+```python
+from acslib import CcureAPI
+
+# change MiddleName and Text14 for the person with CCure ID 5001
+ccure_api = CcureAPI()
+ccure_api.personnel.update(5001, {"Text14": "new text here", "MiddleName": "Shaquille"})
+```
+
+#### Add new personnel record
+
+```python
+from acslib import CcureAPI
+from acslib.ccure.types import PersonnelCreateData as pcd
+
+ccure_api = CcureAPI()
+new_person_data = pcd(FirstName="Kenny", LastName="Smith", Text1="001132808")
+ccure_api.personnel.create(new_person_data)
+```
+
+#### Delete a personnel record
+
+```python
+from acslib import CcureAPI
+
+# delete the personnel record with the CCure ID 6008
+ccure_api = CcureAPI()
+ccure_api.personnel.delete(6008)
+```
+
 ### Clearance
 
 #### Find a Clearance by name
 
 ```python
 from acslib import CcureAPI
```

#### html2text {}

```diff
@@ -9,19 +9,28 @@
 `Personnel`, `Clearances`, `Credentials`, and `ClearanceItem` in Ccure9k *
 Supports search by custom fields. ## Usage ### Personnel #### Find a person by
 name ```python from acslib import CcureAPI ccure_api = CcureAPI() response =
 ccure_api.personnel.search("Roddy Piper".split()) ``` #### Find a person by
 custom field ```python from acslib import CcureAPI from acslib.ccure.filters
 import PersonnelFilter, FUZZ ccure_api = CcureAPI() search_filter =
 PersonnelFilter(lookups={"Text1": FUZZ}) response = ccure_api.personnel.search(
-["PER0892347"], search_filter=search_filter) ``` ### Clearance #### Find a
-Clearance by name ```python from acslib import CcureAPI ccure_api = CcureAPI()
-response = ccure_api.clearance.search(["suite", "door"]) ``` #### Find a
-Clearance by other field ```python from acslib import CcureAPI from
-acslib.ccure.filters import ClearanceFilter, NFUZZ # search by ObjectID
+["PER0892347"], search_filter=search_filter) ``` #### Update a personnel record
+```python from acslib import CcureAPI # change MiddleName and Text14 for the
+person with CCure ID 5001 ccure_api = CcureAPI() ccure_api.personnel.update
+(5001, {"Text14": "new text here", "MiddleName": "Shaquille"}) ``` #### Add new
+personnel record ```python from acslib import CcureAPI from acslib.ccure.types
+import PersonnelCreateData as pcd ccure_api = CcureAPI() new_person_data = pcd
+(FirstName="Kenny", LastName="Smith", Text1="001132808")
+ccure_api.personnel.create(new_person_data) ``` #### Delete a personnel record
+```python from acslib import CcureAPI # delete the personnel record with the
+CCure ID 6008 ccure_api = CcureAPI() ccure_api.personnel.delete(6008) ``` ###
+Clearance #### Find a Clearance by name ```python from acslib import CcureAPI
+ccure_api = CcureAPI() response = ccure_api.clearance.search(["suite", "door"])
+``` #### Find a Clearance by other field ```python from acslib import CcureAPI
+from acslib.ccure.filters import ClearanceFilter, NFUZZ # search by ObjectID
 ccure_api = CcureAPI() search_filter = ClearanceFilter(lookups={"ObjectID":
 NFUZZ}) response = ccure_api.clearance.search([8897],
 search_filter=search_filter) ``` ### Credential #### Find all credentials
 ```python from acslib import CcureAPI ccure_api = CcureAPI() response =
 ccure_api.credential.search() ``` #### Find a credential by name ```python from
 acslib import CcureAPI # fuzzy search by name ccure_api = CcureAPI() response =
 ccure_api.credential.search(["charles", "barkley"]) ``` #### Find a credential
```

### Comparing `acslib-0.1.4/acslib/base/connection.py` & `acslib-0.1.6/acslib/base/connection.py`

 * *Files identical despite different names*

### Comparing `acslib-0.1.4/acslib/base/status.py` & `acslib-0.1.6/acslib/base/status.py`

 * *Files identical despite different names*

### Comparing `acslib-0.1.4/acslib/ccure/base.py` & `acslib-0.1.6/acslib/ccure/base.py`

 * *Files identical despite different names*

### Comparing `acslib-0.1.4/acslib/ccure/config.py` & `acslib-0.1.6/acslib/ccure/config.py`

 * *Files identical despite different names*

### Comparing `acslib-0.1.4/acslib/ccure/connection.py` & `acslib-0.1.6/acslib/ccure/connection.py`

 * *Files identical despite different names*

### Comparing `acslib-0.1.4/acslib/ccure/crud.py` & `acslib-0.1.6/acslib/ccure/crud.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,26 @@
+import json
 from typing import Optional
 
 from acslib.base import ACSRequestData, ACSRequestResponse
 from acslib.base.connection import ACSRequestMethod
 from acslib.ccure.base import CcureACS
 from acslib.ccure.connection import CcureConnection
 from acslib.ccure.filters import (
     ClearanceFilter,
     ClearanceItemFilter,
     CredentialFilter,
     PersonnelFilter,
 )
-from acslib.ccure.types import ClearanceItemCreateData, ClearanceItemType, CredentialCreateData
+from acslib.ccure.data_models import (
+    ClearanceItemCreateData,
+    CredentialCreateData,
+    PersonnelCreateData,
+)
+from acslib.ccure.types import ClearanceItemType
 
 
 class CcureAPI:
     def __init__(self, connection: Optional[CcureConnection] = None):
         self.personnel = CcurePersonnel(connection)
         self.clearance = CcureClearance(connection)
         self.credential = CcureCredential(connection)
@@ -23,14 +29,20 @@
 
 class CcurePersonnel(CcureACS):
     def __init__(self, connection: Optional[CcureConnection] = None):
         super().__init__(connection)
         self.search_filter = PersonnelFilter()
 
     def search(self, terms: list, search_filter: Optional[PersonnelFilter] = None) -> list:
+        """
+        Get a list of Personnel objects matching given search terms
+
+        :param terms: list of search terms
+        :param search filter: specifies how and in what fields to look for the search terms
+        """
         self.logger.info("Searching for personnel")
         search_filter = search_filter or self.search_filter
         request_json = {
             "TypeFullName": "Personnel",
             "pageSize": self.connection.config.page_size,
             "pageNumber": 1,
             "DisplayProperties": search_filter.display_properties,
@@ -43,14 +55,15 @@
                 url=self.config.base_url + self.config.endpoints.FIND_OBJS_W_CRITERIA,
                 request_json=request_json,
                 headers=self.connection.base_headers,
             ),
         ).json
 
     def count(self) -> int:
+        """Get the total number of Personnel objects"""
         request_json = {
             "TypeFullName": "Personnel",
             "pageSize": 0,
             "CountOnly": True,
             "WhereClause": "",
         }
         return self.connection.request(
@@ -58,30 +71,82 @@
             request_data=ACSRequestData(
                 url=self.config.base_url + self.config.endpoints.FIND_OBJS_W_CRITERIA,
                 request_json=request_json,
                 headers=self.connection.base_headers,
             ),
         ).json
 
-    def update(self, record_id: str, update_data: dict) -> ACSRequestResponse:
-        pass
+    def update(self, personnel_id: int, update_data: dict) -> ACSRequestResponse:
+        """
+        Edit properties of a personnel object
 
-    def create(self, create_data: dict) -> ACSRequestResponse:
-        pass
+        :param personnel_id: the Personnel object's CCure ID
+        :param update_data: maps Personnel properties to their new values
+        """
+        return self.connection.request(
+            ACSRequestMethod.PUT,
+            request_data=ACSRequestData(
+                url=self.config.base_url + self.config.endpoints.EDIT_OBJECT,
+                params={
+                    "type": "SoftwareHouse.NextGen.Common.SecurityObjects.Personnel",
+                    "id": personnel_id,
+                },
+                data=self.connection.encode_data(
+                    {
+                        "PropertyNames": list(update_data.keys()),
+                        "PropertyValues": list(update_data.values()),
+                    }
+                ),
+                headers=self.connection.base_headers | self.connection.header_for_form_data,
+            ),
+        )
 
-    def delete(self, record_id: str) -> ACSRequestResponse:
-        pass
+    def create(self, create_data: PersonnelCreateData) -> ACSRequestResponse:
+        """
+        Create a new personnel object
+
+        create_data must contain a 'LastName' property.
+        """
+        create_data_dict = create_data.model_dump()
+        request_data = create_data_dict | {
+            "ClassType": "SoftwareHouse.NextGen.Common.SecurityObjects.Personnel"
+        }
+        return self.connection.request(
+            ACSRequestMethod.POST,
+            request_data=ACSRequestData(
+                url=self.config.base_url + self.config.endpoints.CREATE_PERSONNEL,
+                data=json.dumps(request_data),
+                headers=self.connection.base_headers,
+            ),
+        )
+
+    def delete(self, personnel_id: int) -> ACSRequestResponse:
+        """Delete a personnel object by its CCure ID"""
+        return self.connection.request(
+            ACSRequestMethod.DELETE,
+            request_data=ACSRequestData(
+                url=self.config.base_url
+                + self.config.endpoints.DELETE_PERSONNEL.format(_id=personnel_id),
+                headers=self.connection.base_headers,
+            ),
+        )
 
 
 class CcureClearance(CcureACS):
     def __init__(self, connection: Optional[CcureConnection] = None):
         super().__init__(connection)
         self.search_filter = ClearanceFilter()
 
     def search(self, terms: list, search_filter: Optional[ClearanceFilter] = None) -> list:
+        """
+        Get a list of Clearance objects matching given search terms
+
+        :param terms: list of search terms
+        :param search filter: specifies how and in what fields to look for the search terms
+        """
         self.logger.info("Searching for clearances")
         search_filter = search_filter or self.search_filter
         request_json = {
             "partitionList": [],
             "pageSize": self.connection.config.page_size,
             "pageNumber": 1,
             "sortColumnName": "",
@@ -97,14 +162,15 @@
                 + self.connection.config.endpoints.CLEARANCES_FOR_ASSIGNMENT,
                 request_json=request_json,
                 headers=self.connection.base_headers,
             ),
         ).json[1:]
 
     def count(self) -> int:
+        """Get the total number of Clearance objects"""
         request_options = {
             "pageSize": 0,
             "TypeFullName": "Clearance",
             "pageNumber": 1,
             "CountOnly": True,
             "WhereClause": "",
         }
@@ -113,32 +179,38 @@
             request_data=ACSRequestData(
                 url=self.config.base_url + self.config.endpoints.FIND_OBJS_W_CRITERIA,
                 request_json=request_options,
                 headers=self.connection.base_headers,
             ),
         ).json
 
-    def update(self, record_id: str, update_data: dict) -> ACSRequestResponse:
+    def update(self, record_id: int, update_data: dict) -> ACSRequestResponse:
         pass
 
     def create(self, create_data: dict) -> ACSRequestResponse:
         pass
 
-    def delete(self, record_id: str) -> ACSRequestResponse:
+    def delete(self, record_id: int) -> ACSRequestResponse:
         pass
 
 
 class CcureCredential(CcureACS):
     def __init__(self, connection: Optional[CcureConnection] = None):
         super().__init__(connection)
         self.search_filter = CredentialFilter()
 
     def search(
         self, terms: Optional[list] = None, search_filter: Optional[CredentialFilter] = None
     ) -> list:
+        """
+        Get a list of Credential objects matching given search terms
+
+        :param terms: list of search terms
+        :param search filter: specifies how and in what fields to look for the search terms
+        """
         self.logger.info("Searching for credentials")
         if terms:
             search_filter = search_filter or self.search_filter
             request_json = {
                 "TypeFullName": "SoftwareHouse.NextGen.Common.SecurityObjects.Credential",
                 "pageSize": 100,
                 "pageNumber": 1,
@@ -163,24 +235,31 @@
                     url=self.connection.config.base_url
                     + self.connection.config.endpoints.GET_CREDENTIALS,
                     headers=self.connection.base_headers,
                 ),
             ).json[1:]
 
     def count(self) -> int:
+        """Get the total number of Credential objects"""
         response = self.connection.request(
             ACSRequestMethod.GET,
             request_data=ACSRequestData(
                 url=self.config.base_url + self.config.endpoints.GET_CREDENTIALS,
                 headers=self.connection.base_headers,
             ),
         ).json
         return response[0]["TotalRowsInAllPages"]
 
-    def update(self, record_id: str, update_data: dict) -> ACSRequestResponse:
+    def update(self, record_id: int, update_data: dict) -> ACSRequestResponse:
+        """
+        Edit properties of a Credential object
+
+        :param record_id: the Credential object's CCure ID
+        :param update_data: maps Credential properties to their new values
+        """
         return self.connection.request(
             ACSRequestMethod.PUT,
             request_data=ACSRequestData(
                 url=self.config.base_url + self.config.endpoints.EDIT_OBJECT,
                 params={
                     "type": "SoftwareHouse.NextGen.Common.SecurityObjects.Credential",
                     "id": record_id,
@@ -224,14 +303,15 @@
                 url=self.config.base_url + self.config.endpoints.PERSIST_TO_CONTAINER,
                 data=self.connection.encode_data(request_data),
                 headers=self.connection.base_headers | self.connection.header_for_form_data,
             ),
         )
 
     def delete(self, record_id: int) -> ACSRequestResponse:
+        """Delete a Credential object by its CCure ID"""
         return self.connection.request(
             ACSRequestMethod.DELETE,
             request_data=ACSRequestData(
                 url=self.config.base_url
                 + self.config.endpoints.DELETE_CREDENTIAL.format(_id=record_id),
                 headers=self.connection.base_headers,
             ),
@@ -245,14 +325,20 @@
 
     def search(
         self,
         item_type: ClearanceItemType,
         terms: Optional[list] = None,
         search_filter: Optional[ClearanceItemFilter] = None,
     ) -> list:
+        """
+        Get a list of ClearanceItem objects matching given search terms
+
+        :param terms: list of search terms
+        :param search filter: specifies how and in what fields to look for the search terms
+        """
         self.logger.info("Searching for clearance items")
         search_filter = search_filter or self.search_filter
         request_json = {
             "TypeFullName": item_type.complete,
             "pageSize": 100,
             "pageNumber": 1,
             "DisplayProperties": search_filter.display_properties,
@@ -266,14 +352,15 @@
                 request_json=request_json,
                 headers=self.connection.base_headers,
             ),
         )
         return response.json
 
     def count(self, item_type: ClearanceItemType) -> int:
+        """Get the total number of ClearanceItem objects"""
         request_json = {
             "TypeFullName": item_type.complete,
             "pageSize": 0,
             "CountOnly": True,
             "WhereClause": "",
         }
         response = self.connection.request(
@@ -284,16 +371,23 @@
                 request_json=request_json,
                 headers=self.connection.base_headers,
             ),
         )
         return response.json
 
     def update(
-        self, item_type: ClearanceItemType, item_id: str, update_data: dict
+        self, item_type: ClearanceItemType, item_id: int, update_data: dict
     ) -> ACSRequestResponse:
+        """
+        Edit properties of a ClearanceItem object
+
+        :param item_type: specifies an item type. eg ClearanceItemType.DOOR
+        :param item_id: the ClearanceItem object's CCure ID
+        :param update_data: maps ClearanceItem properties to their new values
+        """
         return self.connection.request(
             ACSRequestMethod.PUT,
             request_data=ACSRequestData(
                 url=self.config.base_url + self.config.endpoints.EDIT_OBJECT,
                 params={"type": item_type.complete, "id": item_id},
                 data=self.connection.encode_data(
                     {
@@ -336,14 +430,15 @@
                 url=self.config.base_url + self.config.endpoints.PERSIST_TO_CONTAINER,
                 data=self.connection.encode_data(request_data),
                 headers=self.connection.base_headers | self.connection.header_for_form_data,
             ),
         )
 
     def delete(self, item_type: ClearanceItemType, item_id: int) -> ACSRequestResponse:
+        """Delete a ClearanceItem object by its CCure ID"""
         return self.connection.request(
             ACSRequestMethod.DELETE,
             request_data=ACSRequestData(
                 url=self.config.base_url + self.config.endpoints.DELETE_OBJECT,
                 params={"type": item_type.complete, "id": item_id},
                 headers=self.connection.base_headers,
             ),
```

### Comparing `acslib-0.1.4/acslib/ccure/endpoints.py` & `acslib-0.1.6/acslib/ccure/endpoints.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 @dataclass
 class V2Endpoints:
     FIND_OBJS_W_CRITERIA = "/victorwebservice/api/Objects/FindObjsWithCriteriaFilter"
     CLEARANCES_FOR_ASSIGNMENT = "/victorwebservice/api/v2/Personnel/ClearancesForAssignment"
     GET_ALL_WITH_CRITERIA = "/victorwebservice/api/Objects/GetAllWithCriteria"
     PERSIST_TO_CONTAINER = "/victorwebservice/api/Objects/PersistToContainer"
     REMOVE_FROM_CONTAINER = "/victorwebservice/api/Objects/RemoveFromContainer"
+    CREATE_PERSONNEL = "/victorwebservice/api/v2/Personnel"
+    DELETE_PERSONNEL = "/victorwebservice/api/v2/Personnel/{_id}"
     DELETE_OBJECT = "/victorwebservice/api/Objects/Delete"
     EDIT_OBJECT = "/victorwebservice/api/Objects/Put"
     LOGIN = "/victorwebservice/api/Authenticate/Login"
     LOGOUT = "/victorwebservice/api/Authenticate/Logout"
     KEEPALIVE = "/victorwebservice/api/v2/session/keepalive"
     VERSIONS = "/victorwebservice/api/Generic/Versions"
     DISABLE = "/victorwebservice/api/v2/objects/SetProperty"
```

### Comparing `acslib-0.1.4/acslib/ccure/filters.py` & `acslib-0.1.6/acslib/ccure/filters.py`

 * *Files identical despite different names*

### Comparing `acslib-0.1.4/acslib/ccure/tests/conftest.py` & `acslib-0.1.6/acslib/ccure/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `acslib-0.1.4/acslib/ccure/tests/test_base.py` & `acslib-0.1.6/acslib/ccure/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `acslib-0.1.4/acslib/ccure/tests/test_config.py` & `acslib-0.1.6/acslib/ccure/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `acslib-0.1.4/acslib/ccure/tests/test_connection.py` & `acslib-0.1.6/acslib/ccure/tests/test_connection.py`

 * *Files identical despite different names*

### Comparing `acslib-0.1.4/acslib/ccure/tests/test_search.py` & `acslib-0.1.6/acslib/ccure/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `acslib-0.1.4/docs/installation.md` & `acslib-0.1.6/docs/installation.md`

 * *Files identical despite different names*

### Comparing `acslib-0.1.4/mkdocs.yml` & `acslib-0.1.6/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `acslib-0.1.4/notebooks/.ipynb_checkpoints/encode_investigation-checkpoint` & `acslib-0.1.6/notebooks/.ipynb_checkpoints/encode_investigation-checkpoint`

 * *Files identical despite different names*

### Comparing `acslib-0.1.4/notebooks/.ipynb_checkpoints/encode_investigation-checkpoint.ipynb` & `acslib-0.1.6/notebooks/.ipynb_checkpoints/encode_investigation-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `acslib-0.1.4/notebooks/encode_investigation.ipynb` & `acslib-0.1.6/notebooks/encode_investigation.ipynb`

 * *Files identical despite different names*

### Comparing `acslib-0.1.4/pyproject.toml` & `acslib-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core>=3.2, <4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "acslib"
-version = "0.1.4"
+version = "0.1.6"
 authors = [
     { name="Jeremy Gibson", email="jmgibso3@ncsu.edu" },
     { name="Luc Sanchez", email="lgsanche@ncsu.edu" },
     { name="Ryan Semmler", email="rsemmle@ncsu.edu" },
 ]
 description = "A library for interacting with Access Control Systems like Genetec or Ccure9k"
 readme = "README.md"
```

### Comparing `acslib-0.1.4/requirements/base/base.txt` & `acslib-0.1.6/requirements/base/base.txt`

 * *Files identical despite different names*

### Comparing `acslib-0.1.4/requirements/dev/dev.txt` & `acslib-0.1.6/requirements/dev/dev.txt`

 * *Files identical despite different names*

### Comparing `acslib-0.1.4/PKG-INFO` & `acslib-0.1.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acslib
-Version: 0.1.4
+Version: 0.1.6
 Summary: A library for interacting with Access Control Systems like Genetec or Ccure9k
 Author-email: Jeremy Gibson <jmgibso3@ncsu.edu>, Luc Sanchez <lgsanche@ncsu.edu>, Ryan Semmler <rsemmle@ncsu.edu>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: pydantic>=2.5.3, <3.0.0
 Requires-Dist: sat-utils>=1.1.12, <2.0.0
 Requires-Dist: pytest>=6.2.5, <7.0.0 ; extra == "dev"
@@ -78,14 +78,45 @@
 from acslib.ccure.filters import PersonnelFilter, FUZZ
 
 ccure_api = CcureAPI()
 search_filter = PersonnelFilter(lookups={"Text1": FUZZ})
 response = ccure_api.personnel.search(["PER0892347"], search_filter=search_filter)
 ```
 
+#### Update a personnel record
+
+```python
+from acslib import CcureAPI
+
+# change MiddleName and Text14 for the person with CCure ID 5001
+ccure_api = CcureAPI()
+ccure_api.personnel.update(5001, {"Text14": "new text here", "MiddleName": "Shaquille"})
+```
+
+#### Add new personnel record
+
+```python
+from acslib import CcureAPI
+from acslib.ccure.types import PersonnelCreateData as pcd
+
+ccure_api = CcureAPI()
+new_person_data = pcd(FirstName="Kenny", LastName="Smith", Text1="001132808")
+ccure_api.personnel.create(new_person_data)
+```
+
+#### Delete a personnel record
+
+```python
+from acslib import CcureAPI
+
+# delete the personnel record with the CCure ID 6008
+ccure_api = CcureAPI()
+ccure_api.personnel.delete(6008)
+```
+
 ### Clearance
 
 #### Find a Clearance by name
 
 ```python
 from acslib import CcureAPI
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: acslib Version: 0.1.4 Summary: A library for
+Metadata-Version: 2.1 Name: acslib Version: 0.1.6 Summary: A library for
 interacting with Access Control Systems like Genetec or Ccure9k Author-email:
 Jeremy Gibson
 ncsu.edu>, Luc Sanchez
 ncsu.edu>, Ryan Semmler
 ncsu.edu> Requires-Python: >=3.10 Description-Content-Type: text/markdown
 Requires-Dist: pydantic>=2.5.3, <3.0.0 Requires-Dist: sat-utils>=1.1.12, <2.0.0
 Requires-Dist: pytest>=6.2.5, <7.0.0 ; extra == "dev" Requires-Dist: pytest-
@@ -31,19 +31,28 @@
 `Personnel`, `Clearances`, `Credentials`, and `ClearanceItem` in Ccure9k *
 Supports search by custom fields. ## Usage ### Personnel #### Find a person by
 name ```python from acslib import CcureAPI ccure_api = CcureAPI() response =
 ccure_api.personnel.search("Roddy Piper".split()) ``` #### Find a person by
 custom field ```python from acslib import CcureAPI from acslib.ccure.filters
 import PersonnelFilter, FUZZ ccure_api = CcureAPI() search_filter =
 PersonnelFilter(lookups={"Text1": FUZZ}) response = ccure_api.personnel.search(
-["PER0892347"], search_filter=search_filter) ``` ### Clearance #### Find a
-Clearance by name ```python from acslib import CcureAPI ccure_api = CcureAPI()
-response = ccure_api.clearance.search(["suite", "door"]) ``` #### Find a
-Clearance by other field ```python from acslib import CcureAPI from
-acslib.ccure.filters import ClearanceFilter, NFUZZ # search by ObjectID
+["PER0892347"], search_filter=search_filter) ``` #### Update a personnel record
+```python from acslib import CcureAPI # change MiddleName and Text14 for the
+person with CCure ID 5001 ccure_api = CcureAPI() ccure_api.personnel.update
+(5001, {"Text14": "new text here", "MiddleName": "Shaquille"}) ``` #### Add new
+personnel record ```python from acslib import CcureAPI from acslib.ccure.types
+import PersonnelCreateData as pcd ccure_api = CcureAPI() new_person_data = pcd
+(FirstName="Kenny", LastName="Smith", Text1="001132808")
+ccure_api.personnel.create(new_person_data) ``` #### Delete a personnel record
+```python from acslib import CcureAPI # delete the personnel record with the
+CCure ID 6008 ccure_api = CcureAPI() ccure_api.personnel.delete(6008) ``` ###
+Clearance #### Find a Clearance by name ```python from acslib import CcureAPI
+ccure_api = CcureAPI() response = ccure_api.clearance.search(["suite", "door"])
+``` #### Find a Clearance by other field ```python from acslib import CcureAPI
+from acslib.ccure.filters import ClearanceFilter, NFUZZ # search by ObjectID
 ccure_api = CcureAPI() search_filter = ClearanceFilter(lookups={"ObjectID":
 NFUZZ}) response = ccure_api.clearance.search([8897],
 search_filter=search_filter) ``` ### Credential #### Find all credentials
 ```python from acslib import CcureAPI ccure_api = CcureAPI() response =
 ccure_api.credential.search() ``` #### Find a credential by name ```python from
 acslib import CcureAPI # fuzzy search by name ccure_api = CcureAPI() response =
 ccure_api.credential.search(["charles", "barkley"]) ``` #### Find a credential
```

