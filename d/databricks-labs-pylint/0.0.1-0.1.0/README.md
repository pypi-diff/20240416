# Comparing `tmp/databricks_labs_pylint-0.0.1.tar.gz` & `tmp/databricks_labs_pylint-0.1.0.tar.gz`

## Comparing `databricks_labs_pylint-0.0.1.tar` & `databricks_labs_pylint-0.1.0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.0.1/databricks/__init__.py
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.0.1/databricks/labs/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.0.1/databricks/labs/pylint/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.0.1/databricks/labs/pylint/__init__.py
--rw-r--r--   0        0        0     4533 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.0.1/databricks/labs/pylint/airflow.py
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.0.1/databricks/labs/pylint/all.py
--rw-r--r--   0        0        0     2469 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.0.1/databricks/labs/pylint/cli.py
--rw-r--r--   0        0        0     6254 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.0.1/databricks/labs/pylint/dbutils.py
--rw-r--r--   0        0        0     3743 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.0.1/databricks/labs/pylint/legacy.py
--rw-r--r--   0        0        0     2717 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.0.1/databricks/labs/pylint/notebooks.py
--rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.0.1/databricks/labs/pylint/spark.py
--rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.0.1/.gitignore
--rw-r--r--   0        0        0     3862 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.0.1/LICENSE
--rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.0.1/NOTICE
--rw-r--r--   0        0        0    12996 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.0.1/README.md
--rw-r--r--   0        0        0    26402 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.0.1/pyproject.toml
--rw-r--r--   0        0        0    14008 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.1.0/databricks/__init__.py
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.1.0/databricks/labs/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.1.0/databricks/labs/pylint/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.1.0/databricks/labs/pylint/__init__.py
+-rw-r--r--   0        0        0     4533 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.1.0/databricks/labs/pylint/airflow.py
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.1.0/databricks/labs/pylint/all.py
+-rw-r--r--   0        0        0     2469 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.1.0/databricks/labs/pylint/cli.py
+-rw-r--r--   0        0        0     6254 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.1.0/databricks/labs/pylint/dbutils.py
+-rw-r--r--   0        0        0     3743 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.1.0/databricks/labs/pylint/legacy.py
+-rw-r--r--   0        0        0     4483 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.1.0/databricks/labs/pylint/mocking.py
+-rw-r--r--   0        0        0     2717 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.1.0/databricks/labs/pylint/notebooks.py
+-rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.1.0/databricks/labs/pylint/spark.py
+-rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.1.0/.gitignore
+-rw-r--r--   0        0        0     3862 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.1.0/LICENSE
+-rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.1.0/NOTICE
+-rw-r--r--   0        0        0    15833 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.1.0/README.md
+-rw-r--r--   0        0        0    26402 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0    16845 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.1.0/PKG-INFO
```

### Comparing `databricks_labs_pylint-0.0.1/databricks/labs/pylint/airflow.py` & `databricks_labs_pylint-0.1.0/databricks/labs/pylint/airflow.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_pylint-0.0.1/databricks/labs/pylint/all.py` & `databricks_labs_pylint-0.1.0/databricks/labs/pylint/all.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from databricks.labs.pylint.airflow import AirflowChecker
 from databricks.labs.pylint.dbutils import DbutilsChecker
 from databricks.labs.pylint.legacy import LegacyChecker
+from databricks.labs.pylint.mocking import MockingChecker
 from databricks.labs.pylint.notebooks import NotebookChecker
 from databricks.labs.pylint.spark import SparkChecker
 
 
 def register(linter):
     linter.register_checker(NotebookChecker(linter))
     linter.register_checker(DbutilsChecker(linter))
     linter.register_checker(LegacyChecker(linter))
     linter.register_checker(AirflowChecker(linter))
     linter.register_checker(SparkChecker(linter))
+    linter.register_checker(MockingChecker(linter))
```

### Comparing `databricks_labs_pylint-0.0.1/databricks/labs/pylint/cli.py` & `databricks_labs_pylint-0.1.0/databricks/labs/pylint/cli.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_pylint-0.0.1/databricks/labs/pylint/dbutils.py` & `databricks_labs_pylint-0.1.0/databricks/labs/pylint/dbutils.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_pylint-0.0.1/databricks/labs/pylint/legacy.py` & `databricks_labs_pylint-0.1.0/databricks/labs/pylint/legacy.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_pylint-0.0.1/databricks/labs/pylint/notebooks.py` & `databricks_labs_pylint-0.1.0/databricks/labs/pylint/notebooks.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_pylint-0.0.1/databricks/labs/pylint/spark.py` & `databricks_labs_pylint-0.1.0/databricks/labs/pylint/spark.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_pylint-0.0.1/.gitignore` & `databricks_labs_pylint-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `databricks_labs_pylint-0.0.1/LICENSE` & `databricks_labs_pylint-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `databricks_labs_pylint-0.0.1/NOTICE` & `databricks_labs_pylint-0.1.0/NOTICE`

 * *Files identical despite different names*

### Comparing `databricks_labs_pylint-0.0.1/README.md` & `databricks_labs_pylint-0.1.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -243,19 +243,58 @@
 
 ### `W8916`: `no-spark-argument-in-function`
 
 Function XXX is missing a 'spark' argument. Function refers to a global spark variable, which may not always be available. Pass the spark object as an argument to the function instead, so that the function becomes testable in a CI/CD pipelines.
 
 [[back to top](#pylint-plugin-for-databricks)]
 
+## `mocking` checker
+
+[[back to top](#pylint-plugin-for-databricks)]
+
+### `R8918`: `explicit-dependency-required`
+
+Obscure implicit test dependency with mock.patch(XXX). Rewrite to inject dependencies through constructor.. Using `patch` to mock dependencies in unit tests can introduce implicit 
+dependencies within a class, making it unclear to other developers. Constructor arguments, on the other hand, 
+explicitly declare dependencies, enhancing code readability and maintainability. However, reliance on `patch` 
+for testing may lead to issues during refactoring, as updates to underlying implementations would necessitate 
+changes across multiple unrelated unit tests. Moreover, the use of hard-coded strings in `patch` can obscure 
+which unit tests require modification, as they lack strongly typed references. This coupling of the class 
+under test to concrete classes signifies a code smell, and such code is not easily portable to statically typed 
+languages where monkey patching isn't feasible without significant effort. In essence, extensive patching of 
+external clients suggests a need for refactoring, with experienced engineers recognizing the potential for 
+dependency inversion in such scenarios.
+
+To address this issue, refactor the code to inject dependencies through the constructor. This approach
+explicitly declares dependencies, enhancing code readability and maintainability. Moreover, it allows for
+dependency inversion, enabling the use of interfaces to decouple the class under test from concrete classes.
+This decoupling facilitates unit testing, as it allows for the substitution of mock objects for concrete
+implementations, ensuring that the class under test behaves as expected. By following this approach, you can
+create more robust and maintainable unit tests, improving the overall quality of your codebase.
+
+Use `require-explicit-dependency` option to specify the package names that contain code for your project.
+
+[[back to top](#pylint-plugin-for-databricks)]
+
+### `R8919`: `obscure-mock`
+
+Obscure implicit test dependency with MagicMock(). Rewrite with create_autospec(ConcreteType).. Using `MagicMock` to mock dependencies in unit tests can introduce implicit dependencies 
+within a class, making it unclear to other developers. create_autospec(ConcreteType) is a better alternative, as it
+automatically creates a mock object with the same attributes and methods as the concrete class. This
+approach ensures that the mock object behaves like the concrete class, allowing for more robust and
+maintainable unit tests. Moreover, reliance on `MagicMock` for testing leads to issues during refactoring,
+as updates to underlying implementations would necessitate changes across multiple unrelated unit tests.
+
+[[back to top](#pylint-plugin-for-databricks)]
+
 ## Testing in isolation
 To test this plugin in isolation, you can use the following command:
 
 ```bash
-pylint --load-plugins=databricks.labs.pylint.all --disable=all --enable=missing-data-security-mode,unsupported-runtime,dbutils-fs-cp,dbutils-fs-head,dbutils-fs-ls,dbutils-fs-mount,dbutils-credentials,dbutils-notebook-run,pat-token-leaked,internal-api,legacy-cli,incompatible-with-uc,notebooks-too-many-cells,notebooks-percent-run,spark-outside-function,use-display-instead-of-show,no-spark-argument-in-function .
+pylint --load-plugins=databricks.labs.pylint.all --disable=all --enable=missing-data-security-mode,unsupported-runtime,dbutils-fs-cp,dbutils-fs-head,dbutils-fs-ls,dbutils-fs-mount,dbutils-credentials,dbutils-notebook-run,pat-token-leaked,internal-api,legacy-cli,incompatible-with-uc,notebooks-too-many-cells,notebooks-percent-run,spark-outside-function,use-display-instead-of-show,no-spark-argument-in-function,explicit-dependency-required,obscure-mock .
 ```
 
 [[back to top](#pylint-plugin-for-databricks)]
 
 <!-- END CHECKS -->
 
 # Project Support
```

### Comparing `databricks_labs_pylint-0.0.1/pyproject.toml` & `databricks_labs_pylint-0.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `databricks_labs_pylint-0.0.1/PKG-INFO` & `databricks_labs_pylint-0.1.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: databricks-labs-pylint
-Version: 0.0.1
+Version: 0.1.0
 Summary: Plugin for PyLint to support Databricks specific code patterns and best practices.
 Project-URL: Issues, https://github.com/databrickslabs/pylint/issues
 Project-URL: Source, https://github.com/databrickslabs/pylint
 Author-email: Serge Smertin <serge.smertin@databricks.com>
 License-File: LICENSE
 License-File: NOTICE
 Keywords: Databricks
@@ -268,19 +268,58 @@
 
 ### `W8916`: `no-spark-argument-in-function`
 
 Function XXX is missing a 'spark' argument. Function refers to a global spark variable, which may not always be available. Pass the spark object as an argument to the function instead, so that the function becomes testable in a CI/CD pipelines.
 
 [[back to top](#pylint-plugin-for-databricks)]
 
+## `mocking` checker
+
+[[back to top](#pylint-plugin-for-databricks)]
+
+### `R8918`: `explicit-dependency-required`
+
+Obscure implicit test dependency with mock.patch(XXX). Rewrite to inject dependencies through constructor.. Using `patch` to mock dependencies in unit tests can introduce implicit 
+dependencies within a class, making it unclear to other developers. Constructor arguments, on the other hand, 
+explicitly declare dependencies, enhancing code readability and maintainability. However, reliance on `patch` 
+for testing may lead to issues during refactoring, as updates to underlying implementations would necessitate 
+changes across multiple unrelated unit tests. Moreover, the use of hard-coded strings in `patch` can obscure 
+which unit tests require modification, as they lack strongly typed references. This coupling of the class 
+under test to concrete classes signifies a code smell, and such code is not easily portable to statically typed 
+languages where monkey patching isn't feasible without significant effort. In essence, extensive patching of 
+external clients suggests a need for refactoring, with experienced engineers recognizing the potential for 
+dependency inversion in such scenarios.
+
+To address this issue, refactor the code to inject dependencies through the constructor. This approach
+explicitly declares dependencies, enhancing code readability and maintainability. Moreover, it allows for
+dependency inversion, enabling the use of interfaces to decouple the class under test from concrete classes.
+This decoupling facilitates unit testing, as it allows for the substitution of mock objects for concrete
+implementations, ensuring that the class under test behaves as expected. By following this approach, you can
+create more robust and maintainable unit tests, improving the overall quality of your codebase.
+
+Use `require-explicit-dependency` option to specify the package names that contain code for your project.
+
+[[back to top](#pylint-plugin-for-databricks)]
+
+### `R8919`: `obscure-mock`
+
+Obscure implicit test dependency with MagicMock(). Rewrite with create_autospec(ConcreteType).. Using `MagicMock` to mock dependencies in unit tests can introduce implicit dependencies 
+within a class, making it unclear to other developers. create_autospec(ConcreteType) is a better alternative, as it
+automatically creates a mock object with the same attributes and methods as the concrete class. This
+approach ensures that the mock object behaves like the concrete class, allowing for more robust and
+maintainable unit tests. Moreover, reliance on `MagicMock` for testing leads to issues during refactoring,
+as updates to underlying implementations would necessitate changes across multiple unrelated unit tests.
+
+[[back to top](#pylint-plugin-for-databricks)]
+
 ## Testing in isolation
 To test this plugin in isolation, you can use the following command:
 
 ```bash
-pylint --load-plugins=databricks.labs.pylint.all --disable=all --enable=missing-data-security-mode,unsupported-runtime,dbutils-fs-cp,dbutils-fs-head,dbutils-fs-ls,dbutils-fs-mount,dbutils-credentials,dbutils-notebook-run,pat-token-leaked,internal-api,legacy-cli,incompatible-with-uc,notebooks-too-many-cells,notebooks-percent-run,spark-outside-function,use-display-instead-of-show,no-spark-argument-in-function .
+pylint --load-plugins=databricks.labs.pylint.all --disable=all --enable=missing-data-security-mode,unsupported-runtime,dbutils-fs-cp,dbutils-fs-head,dbutils-fs-ls,dbutils-fs-mount,dbutils-credentials,dbutils-notebook-run,pat-token-leaked,internal-api,legacy-cli,incompatible-with-uc,notebooks-too-many-cells,notebooks-percent-run,spark-outside-function,use-display-instead-of-show,no-spark-argument-in-function,explicit-dependency-required,obscure-mock .
 ```
 
 [[back to top](#pylint-plugin-for-databricks)]
 
 <!-- END CHECKS -->
 
 # Project Support
```

