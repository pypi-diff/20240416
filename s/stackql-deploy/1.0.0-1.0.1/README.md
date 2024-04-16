# Comparing `tmp/stackql_deploy-1.0.0.tar.gz` & `tmp/stackql_deploy-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stackql_deploy-1.0.0.tar", last modified: Tue Apr 16 21:10:20 2024, max compression
+gzip compressed data, was "stackql_deploy-1.0.1.tar", last modified: Tue Apr 16 21:31:42 2024, max compression
```

## Comparing `stackql_deploy-1.0.0.tar` & `stackql_deploy-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-16 21:10:20.654129 stackql_deploy-1.0.0/
--rwxrwxrwx   0 javen     (1000) javen     (1000)     1071 2024-03-15 01:52:38.000000 stackql_deploy-1.0.0/LICENSE
--rwxrwxrwx   0 javen     (1000) javen     (1000)     9564 2024-04-16 21:10:20.635050 stackql_deploy-1.0.0/PKG-INFO
--rwxrwxrwx   0 javen     (1000) javen     (1000)     8924 2024-04-16 10:08:07.000000 stackql_deploy-1.0.0/README.rst
--rwxrwxrwx   0 javen     (1000) javen     (1000)       38 2024-04-16 21:10:20.656129 stackql_deploy-1.0.0/setup.cfg
--rwxrwxrwx   0 javen     (1000) javen     (1000)     1300 2024-04-16 21:08:54.000000 stackql_deploy-1.0.0/setup.py
-drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-16 21:10:20.355537 stackql_deploy-1.0.0/stackql_deploy/
--rwxrwxrwx   0 javen     (1000) javen     (1000)       23 2024-04-16 04:53:02.000000 stackql_deploy-1.0.0/stackql_deploy/__init__.py
--rwxrwxrwx   0 javen     (1000) javen     (1000)     3965 2024-04-16 05:13:28.000000 stackql_deploy-1.0.0/stackql_deploy/cli.py
-drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-16 21:10:20.613988 stackql_deploy-1.0.0/stackql_deploy.egg-info/
--rwxrwxrwx   0 javen     (1000) javen     (1000)     9564 2024-04-16 21:10:19.000000 stackql_deploy-1.0.0/stackql_deploy.egg-info/PKG-INFO
--rwxrwxrwx   0 javen     (1000) javen     (1000)      306 2024-04-16 21:10:20.000000 stackql_deploy-1.0.0/stackql_deploy.egg-info/SOURCES.txt
--rwxrwxrwx   0 javen     (1000) javen     (1000)        1 2024-04-16 21:10:19.000000 stackql_deploy-1.0.0/stackql_deploy.egg-info/dependency_links.txt
--rwxrwxrwx   0 javen     (1000) javen     (1000)       58 2024-04-16 21:10:19.000000 stackql_deploy-1.0.0/stackql_deploy.egg-info/entry_points.txt
--rwxrwxrwx   0 javen     (1000) javen     (1000)       37 2024-04-16 21:10:20.000000 stackql_deploy-1.0.0/stackql_deploy.egg-info/requires.txt
--rwxrwxrwx   0 javen     (1000) javen     (1000)       15 2024-04-16 21:10:20.000000 stackql_deploy-1.0.0/stackql_deploy.egg-info/top_level.txt
+drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-16 21:31:42.790046 stackql_deploy-1.0.1/
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     1071 2024-03-15 01:52:38.000000 stackql_deploy-1.0.1/LICENSE
+-rwxrwxrwx   0 javen     (1000) javen     (1000)    10342 2024-04-16 21:31:42.774349 stackql_deploy-1.0.1/PKG-INFO
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     9719 2024-04-16 21:29:08.000000 stackql_deploy-1.0.1/README.rst
+-rwxrwxrwx   0 javen     (1000) javen     (1000)       38 2024-04-16 21:31:42.791045 stackql_deploy-1.0.1/setup.cfg
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     1300 2024-04-16 21:31:36.000000 stackql_deploy-1.0.1/setup.py
+drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-16 21:31:42.600012 stackql_deploy-1.0.1/stackql_deploy/
+-rwxrwxrwx   0 javen     (1000) javen     (1000)       23 2024-04-16 21:31:36.000000 stackql_deploy-1.0.1/stackql_deploy/__init__.py
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     3965 2024-04-16 05:13:28.000000 stackql_deploy-1.0.1/stackql_deploy/cli.py
+drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-16 21:31:42.756295 stackql_deploy-1.0.1/stackql_deploy.egg-info/
+-rwxrwxrwx   0 javen     (1000) javen     (1000)    10342 2024-04-16 21:31:42.000000 stackql_deploy-1.0.1/stackql_deploy.egg-info/PKG-INFO
+-rwxrwxrwx   0 javen     (1000) javen     (1000)      306 2024-04-16 21:31:42.000000 stackql_deploy-1.0.1/stackql_deploy.egg-info/SOURCES.txt
+-rwxrwxrwx   0 javen     (1000) javen     (1000)        1 2024-04-16 21:31:42.000000 stackql_deploy-1.0.1/stackql_deploy.egg-info/dependency_links.txt
+-rwxrwxrwx   0 javen     (1000) javen     (1000)       58 2024-04-16 21:31:42.000000 stackql_deploy-1.0.1/stackql_deploy.egg-info/entry_points.txt
+-rwxrwxrwx   0 javen     (1000) javen     (1000)       37 2024-04-16 21:31:42.000000 stackql_deploy-1.0.1/stackql_deploy.egg-info/requires.txt
+-rwxrwxrwx   0 javen     (1000) javen     (1000)       15 2024-04-16 21:31:42.000000 stackql_deploy-1.0.1/stackql_deploy.egg-info/top_level.txt
```

### Comparing `stackql_deploy-1.0.0/LICENSE` & `stackql_deploy-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `stackql_deploy-1.0.0/PKG-INFO` & `stackql_deploy-1.0.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stackql-deploy
-Version: 1.0.0
+Version: 1.0.1
 Summary: Model driven resource provisioning and deployment framework using StackQL.
 Home-page: https://github.com/stackql/stackql-deploy
 Author: Jeffrey Aven
 Author-email: javen@stackql.io
 License: MIT
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
@@ -18,15 +18,31 @@
 Classifier: License :: OSI Approved :: MIT License
 License-File: LICENSE
 Requires-Dist: click
 Requires-Dist: python-dotenv
 Requires-Dist: jinja2
 Requires-Dist: pystackql
 
-stackql-deploy
+.. image:: https://stackql.io/img/stackql-logo-bold.png
+    :alt: "stackql logo"
+    :target: https://github.com/stackql/stackql
+    :align: center
+
+===========================================================================================
+stackql-deploy - Model driven resource provisioning and deployment framework using StackQL.
+===========================================================================================
+
+.. .. image:: https://readthedocs.org/projects/pystackql/badge/?version=latest
+..    :target: https://pystackql.readthedocs.io/en/latest/
+..    :alt: Documentation Status
+
+.. image:: https://img.shields.io/pypi/v/stackql-deploy
+   :target: https://pypi.org/project/stackql-deploy/
+   :alt: PyPI
+
 ==============
 
 **stackql-deploy** is a multi-cloud Infrastructure as Code (IaC) framework using `stackql`_, inspired by dbt (data build tool), which manages data transformation workflows in analytics engineering by treating SQL scripts as models that can be built, tested, and materialized incrementally. You can create a similar framework for infrastructure provisioning with StackQL. The goal is to treat infrastructure-as-code (IaC) queries as models that can be deployed, managed, and interconnected.
 
 This ELT/model-based framework to IaC allows you to provision, test, update and teardown multi-cloud stacks similar to how dbt manages data transformation projects, with the benefits of version control, peer review, and automation. This approach enables you to deploy complex, dependent infrastructure components in a reliable and repeatable manner.
 
 The use of StackQL simplifies the interaction with cloud resources by using SQL-like syntax, making it easier to define and execute complex cloud management operations. Resources are provisioned with ``INSERT`` statements and tests are structured around ``SELECT`` statements.
@@ -39,16 +55,17 @@
 - SQL-based definitions for resources and tests
 
 How stackql-deploy Works
 ------------------------
 
 **stackql-deploy** orchestrates cloud resource provisioning by parsing SQL-like definitions. It determines the necessity of creating or updating resources based on preflight checks, and ensures the creation and correct desired configuration through post-deployment verifications.
 
-.. image:: images/stackql-deploy.png
-   :alt: Workflow diagram
+.. image:: https://stackql.io/img/blog/stackql-deploy.png
+    :alt: "stackql-deploy"
+    :target: https://github.com/stackql/stackql
 
 Installing from PyPI
 --------------------
 
 To install **stackql-deploy** directly from PyPI, run the following command:
 
 .. code-block:: none
@@ -219,15 +236,15 @@
 
     pip install --upgrade setuptools wheel
 
 Then, navigate to your project root directory and build the distribution files:
 
 .. code-block:: none
 
-    python setup.py sdist bdist_wheel
+    python3 setup.py sdist bdist_wheel
 
 This command generates distribution packages in the ``dist/`` directory.
 
 Uploading the Package to PyPI
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 To upload the package to PyPI, you'll need to use ``twine``, a utility for publishing Python packages. First, install ``twine``:
```

### Comparing `stackql_deploy-1.0.0/README.rst` & `stackql_deploy-1.0.1/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,24 @@
-stackql-deploy
+.. image:: https://stackql.io/img/stackql-logo-bold.png
+    :alt: "stackql logo"
+    :target: https://github.com/stackql/stackql
+    :align: center
+
+===========================================================================================
+stackql-deploy - Model driven resource provisioning and deployment framework using StackQL.
+===========================================================================================
+
+.. .. image:: https://readthedocs.org/projects/pystackql/badge/?version=latest
+..    :target: https://pystackql.readthedocs.io/en/latest/
+..    :alt: Documentation Status
+
+.. image:: https://img.shields.io/pypi/v/stackql-deploy
+   :target: https://pypi.org/project/stackql-deploy/
+   :alt: PyPI
+
 ==============
 
 **stackql-deploy** is a multi-cloud Infrastructure as Code (IaC) framework using `stackql`_, inspired by dbt (data build tool), which manages data transformation workflows in analytics engineering by treating SQL scripts as models that can be built, tested, and materialized incrementally. You can create a similar framework for infrastructure provisioning with StackQL. The goal is to treat infrastructure-as-code (IaC) queries as models that can be deployed, managed, and interconnected.
 
 This ELT/model-based framework to IaC allows you to provision, test, update and teardown multi-cloud stacks similar to how dbt manages data transformation projects, with the benefits of version control, peer review, and automation. This approach enables you to deploy complex, dependent infrastructure components in a reliable and repeatable manner.
 
 The use of StackQL simplifies the interaction with cloud resources by using SQL-like syntax, making it easier to define and execute complex cloud management operations. Resources are provisioned with ``INSERT`` statements and tests are structured around ``SELECT`` statements.
@@ -15,16 +31,17 @@
 - SQL-based definitions for resources and tests
 
 How stackql-deploy Works
 ------------------------
 
 **stackql-deploy** orchestrates cloud resource provisioning by parsing SQL-like definitions. It determines the necessity of creating or updating resources based on preflight checks, and ensures the creation and correct desired configuration through post-deployment verifications.
 
-.. image:: images/stackql-deploy.png
-   :alt: Workflow diagram
+.. image:: https://stackql.io/img/blog/stackql-deploy.png
+    :alt: "stackql-deploy"
+    :target: https://github.com/stackql/stackql
 
 Installing from PyPI
 --------------------
 
 To install **stackql-deploy** directly from PyPI, run the following command:
 
 .. code-block:: none
@@ -195,15 +212,15 @@
 
     pip install --upgrade setuptools wheel
 
 Then, navigate to your project root directory and build the distribution files:
 
 .. code-block:: none
 
-    python setup.py sdist bdist_wheel
+    python3 setup.py sdist bdist_wheel
 
 This command generates distribution packages in the ``dist/`` directory.
 
 Uploading the Package to PyPI
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 To upload the package to PyPI, you'll need to use ``twine``, a utility for publishing Python packages. First, install ``twine``:
```

### Comparing `stackql_deploy-1.0.0/setup.py` & `stackql_deploy-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_packages
 
 with open('README.rst', encoding='utf-8') as f:
     readme = f.read()
 
 setup(
     name='stackql-deploy',
-    version='1.0.0',
+    version='1.0.1',
     description='Model driven resource provisioning and deployment framework using StackQL.',
     long_description=readme,
     author='Jeffrey Aven',
     author_email='javen@stackql.io',
     url='https://github.com/stackql/stackql-deploy',
     license='MIT',
     packages=find_packages(),
```

### Comparing `stackql_deploy-1.0.0/stackql_deploy/cli.py` & `stackql_deploy-1.0.1/stackql_deploy/cli.py`

 * *Files identical despite different names*

### Comparing `stackql_deploy-1.0.0/stackql_deploy.egg-info/PKG-INFO` & `stackql_deploy-1.0.1/stackql_deploy.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stackql-deploy
-Version: 1.0.0
+Version: 1.0.1
 Summary: Model driven resource provisioning and deployment framework using StackQL.
 Home-page: https://github.com/stackql/stackql-deploy
 Author: Jeffrey Aven
 Author-email: javen@stackql.io
 License: MIT
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
@@ -18,15 +18,31 @@
 Classifier: License :: OSI Approved :: MIT License
 License-File: LICENSE
 Requires-Dist: click
 Requires-Dist: python-dotenv
 Requires-Dist: jinja2
 Requires-Dist: pystackql
 
-stackql-deploy
+.. image:: https://stackql.io/img/stackql-logo-bold.png
+    :alt: "stackql logo"
+    :target: https://github.com/stackql/stackql
+    :align: center
+
+===========================================================================================
+stackql-deploy - Model driven resource provisioning and deployment framework using StackQL.
+===========================================================================================
+
+.. .. image:: https://readthedocs.org/projects/pystackql/badge/?version=latest
+..    :target: https://pystackql.readthedocs.io/en/latest/
+..    :alt: Documentation Status
+
+.. image:: https://img.shields.io/pypi/v/stackql-deploy
+   :target: https://pypi.org/project/stackql-deploy/
+   :alt: PyPI
+
 ==============
 
 **stackql-deploy** is a multi-cloud Infrastructure as Code (IaC) framework using `stackql`_, inspired by dbt (data build tool), which manages data transformation workflows in analytics engineering by treating SQL scripts as models that can be built, tested, and materialized incrementally. You can create a similar framework for infrastructure provisioning with StackQL. The goal is to treat infrastructure-as-code (IaC) queries as models that can be deployed, managed, and interconnected.
 
 This ELT/model-based framework to IaC allows you to provision, test, update and teardown multi-cloud stacks similar to how dbt manages data transformation projects, with the benefits of version control, peer review, and automation. This approach enables you to deploy complex, dependent infrastructure components in a reliable and repeatable manner.
 
 The use of StackQL simplifies the interaction with cloud resources by using SQL-like syntax, making it easier to define and execute complex cloud management operations. Resources are provisioned with ``INSERT`` statements and tests are structured around ``SELECT`` statements.
@@ -39,16 +55,17 @@
 - SQL-based definitions for resources and tests
 
 How stackql-deploy Works
 ------------------------
 
 **stackql-deploy** orchestrates cloud resource provisioning by parsing SQL-like definitions. It determines the necessity of creating or updating resources based on preflight checks, and ensures the creation and correct desired configuration through post-deployment verifications.
 
-.. image:: images/stackql-deploy.png
-   :alt: Workflow diagram
+.. image:: https://stackql.io/img/blog/stackql-deploy.png
+    :alt: "stackql-deploy"
+    :target: https://github.com/stackql/stackql
 
 Installing from PyPI
 --------------------
 
 To install **stackql-deploy** directly from PyPI, run the following command:
 
 .. code-block:: none
@@ -219,15 +236,15 @@
 
     pip install --upgrade setuptools wheel
 
 Then, navigate to your project root directory and build the distribution files:
 
 .. code-block:: none
 
-    python setup.py sdist bdist_wheel
+    python3 setup.py sdist bdist_wheel
 
 This command generates distribution packages in the ``dist/`` directory.
 
 Uploading the Package to PyPI
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 To upload the package to PyPI, you'll need to use ``twine``, a utility for publishing Python packages. First, install ``twine``:
```

