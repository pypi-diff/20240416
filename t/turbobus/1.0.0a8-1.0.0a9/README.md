# Comparing `tmp/turbobus-1.0.0a8.tar.gz` & `tmp/turbobus-1.0.0a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "turbobus-1.0.0a8.tar", last modified: Sun Apr 14 20:45:22 2024, max compression
+gzip compressed data, was "turbobus-1.0.0a9.tar", last modified: Mon Apr 15 00:40:36 2024, max compression
```

## Comparing `turbobus-1.0.0a8.tar` & `turbobus-1.0.0a9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:45:22.326339 turbobus-1.0.0a8/
--rw-r--r--   0 runner    (1001) docker     (127)     7427 2024-04-14 20:45:22.326339 turbobus-1.0.0a8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6980 2024-04-14 20:45:09.000000 turbobus-1.0.0a8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-04-14 20:45:09.000000 turbobus-1.0.0a8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 20:45:22.326339 turbobus-1.0.0a8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-14 20:45:09.000000 turbobus-1.0.0a8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:45:22.326339 turbobus-1.0.0a8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-04-14 20:45:09.000000 turbobus-1.0.0a8/tests/test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4077 2024-04-14 20:45:09.000000 turbobus-1.0.0a8/tests/test_command.py
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-14 20:45:09.000000 turbobus-1.0.0a8/tests/test_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:45:22.326339 turbobus-1.0.0a8/turbobus/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-14 20:45:09.000000 turbobus-1.0.0a8/turbobus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2173 2024-04-14 20:45:09.000000 turbobus-1.0.0a8/turbobus/command.py
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-14 20:45:09.000000 turbobus-1.0.0a8/turbobus/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-14 20:45:09.000000 turbobus-1.0.0a8/turbobus/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-04-14 20:45:09.000000 turbobus-1.0.0a8/turbobus/injection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:45:22.326339 turbobus-1.0.0a8/turbobus.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7427 2024-04-14 20:45:22.000000 turbobus-1.0.0a8/turbobus.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-14 20:45:22.000000 turbobus-1.0.0a8/turbobus.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 20:45:22.000000 turbobus-1.0.0a8/turbobus.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-14 20:45:22.000000 turbobus-1.0.0a8/turbobus.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 00:40:36.644824 turbobus-1.0.0a9/
+-rw-r--r--   0 runner    (1001) docker     (127)     8504 2024-04-15 00:40:36.644824 turbobus-1.0.0a9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8057 2024-04-15 00:40:20.000000 turbobus-1.0.0a9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-04-15 00:40:20.000000 turbobus-1.0.0a9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 00:40:36.644824 turbobus-1.0.0a9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-15 00:40:20.000000 turbobus-1.0.0a9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 00:40:36.640824 turbobus-1.0.0a9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-04-15 00:40:20.000000 turbobus-1.0.0a9/tests/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4077 2024-04-15 00:40:20.000000 turbobus-1.0.0a9/tests/test_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-15 00:40:20.000000 turbobus-1.0.0a9/tests/test_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 00:40:36.644824 turbobus-1.0.0a9/turbobus/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-15 00:40:20.000000 turbobus-1.0.0a9/turbobus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2173 2024-04-15 00:40:20.000000 turbobus-1.0.0a9/turbobus/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-15 00:40:20.000000 turbobus-1.0.0a9/turbobus/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-15 00:40:20.000000 turbobus-1.0.0a9/turbobus/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-04-15 00:40:20.000000 turbobus-1.0.0a9/turbobus/injection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 00:40:36.644824 turbobus-1.0.0a9/turbobus.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8504 2024-04-15 00:40:36.000000 turbobus-1.0.0a9/turbobus.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-15 00:40:36.000000 turbobus-1.0.0a9/turbobus.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 00:40:36.000000 turbobus-1.0.0a9/turbobus.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-15 00:40:36.000000 turbobus-1.0.0a9/turbobus.egg-info/top_level.txt
```

### Comparing `turbobus-1.0.0a8/PKG-INFO` & `turbobus-1.0.0a9/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: turbobus
-Version: 1.0.0a8
-Summary: TurboBus is an opinionated implementation of Command Responsibility Segregation pattern in python.
-Home-page: https://github.com/cafadev/turbobus
-Download-URL: https://github.com/cafadev/turbobus/releases/tag/v1.0.0-alpha.8
-Author: Christopher A. Flores
-Author-email: cafadev@outlook.com
-License: MIT
-Keywords: command,bus,cqrs,commandbus,ddd
-Description-Content-Type: text/markdown
-
 # TurboBus
 
 TurboBus is a package to create software following the Command Responsibility Segregation pattern in python.
 
 ## Installation
 ```bash
 pip install turbobus
@@ -201,15 +189,14 @@
     bus = CommandBus()
 
     bus.execute(
         CreateUserAccount(name='Christopher Flores', email='cafadev@outlook.com')
     )
 
 ```
-@inject(alias={ 'logger': 'ILogger' }, only=['logger'], exclude=['x'])
 The `@inject` decorator also accepts the next parameters:
 
 ### Alias
 
 The `@inject` decorator use the typing to resolve the required dependency. With the `alias: dict[str, Callable[..., Any]]` parameter you can specify a different implementation for the same interface. For example, let's say we have a UserRepository interface and then two different implementations; UserRepositoryInMemory and UserRepositorySQL.
 
 ```python3
@@ -225,12 +212,40 @@
 By default, the `@inject` will use the `UserRepositoryInMemory` to provide the dependency. Let's specify the `UserRepositorySQL` as the provider. To accomplish that we just need to specify the parameter name that we want to override, and then the Provider Key:
 
 
 ```python3
 Provider.set(UserRepository, UserRepositoryInMemory)
 Provider.set(UserRepositorySQL, UserRepositorySQL)
 
-@inject(alias = { 'user': 'UserRepositorySQL' })
+@inject(alias={ 'user': 'UserRepositorySQL' })
 class CreateUserAccount:
 
     user: UserRepository
 ```
+
+### Only and Exclude
+The `only` and `exclude` parameters in the `@inject` decorator allow you to fine-tune which dependencies should be resolved based on their names.
+
+The `only` parameter specifies a list of dependency names that should exclusively be resolved. All other dependencies will be ignored.
+
+```python3
+@inject(only=['dependency1', 'dependency2'])
+def my_function(dep1: Dependency1, dep2: Dependency2, dep3: Dependency3):
+    # Only dep1 and dep2 will be injected
+    pass
+```
+
+In this example, only dep1 and dep2 will be injected into the function because they are specified in the only list.
+
+The `exclude` parameter specifies a list of dependency names that should be excluded from injection.
+
+```python3
+@inject(exclude=['dependency3'])
+def my_function(dep1: Dependency1, dep2: Dependency2, dep3: Dependency3):
+    # Dep3 will not be injected
+    pass
+
+```
+
+In this example, dep3 will not be injected into the function because it is specified in the exclude list.
+
+These parameters provide flexibility in controlling which dependencies are resolved, allowing you to customize the injection behavior according to your specific needs.
```

### Comparing `turbobus-1.0.0a8/README.md` & `turbobus-1.0.0a9/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+Metadata-Version: 2.1
+Name: turbobus
+Version: 1.0.0a9
+Summary: TurboBus is an opinionated implementation of Command Responsibility Segregation pattern in python.
+Home-page: https://github.com/cafadev/turbobus
+Download-URL: https://github.com/cafadev/turbobus/releases/tag/v1.0.0-alpha.9
+Author: Christopher A. Flores
+Author-email: cafadev@outlook.com
+License: MIT
+Keywords: command,bus,cqrs,commandbus,ddd
+Description-Content-Type: text/markdown
+
 # TurboBus
 
 TurboBus is a package to create software following the Command Responsibility Segregation pattern in python.
 
 ## Installation
 ```bash
 pip install turbobus
@@ -189,15 +201,14 @@
     bus = CommandBus()
 
     bus.execute(
         CreateUserAccount(name='Christopher Flores', email='cafadev@outlook.com')
     )
 
 ```
-@inject(alias={ 'logger': 'ILogger' }, only=['logger'], exclude=['x'])
 The `@inject` decorator also accepts the next parameters:
 
 ### Alias
 
 The `@inject` decorator use the typing to resolve the required dependency. With the `alias: dict[str, Callable[..., Any]]` parameter you can specify a different implementation for the same interface. For example, let's say we have a UserRepository interface and then two different implementations; UserRepositoryInMemory and UserRepositorySQL.
 
 ```python3
@@ -213,12 +224,40 @@
 By default, the `@inject` will use the `UserRepositoryInMemory` to provide the dependency. Let's specify the `UserRepositorySQL` as the provider. To accomplish that we just need to specify the parameter name that we want to override, and then the Provider Key:
 
 
 ```python3
 Provider.set(UserRepository, UserRepositoryInMemory)
 Provider.set(UserRepositorySQL, UserRepositorySQL)
 
-@inject(alias = { 'user': 'UserRepositorySQL' })
+@inject(alias={ 'user': 'UserRepositorySQL' })
 class CreateUserAccount:
 
     user: UserRepository
 ```
+
+### Only and Exclude
+The `only` and `exclude` parameters in the `@inject` decorator allow you to fine-tune which dependencies should be resolved based on their names.
+
+The `only` parameter specifies a list of dependency names that should exclusively be resolved. All other dependencies will be ignored.
+
+```python3
+@inject(only=['dependency1', 'dependency2'])
+def my_function(dep1: Dependency1, dep2: Dependency2, dep3: Dependency3):
+    # Only dep1 and dep2 will be injected
+    pass
+```
+
+In this example, only dep1 and dep2 will be injected into the function because they are specified in the only list.
+
+The `exclude` parameter specifies a list of dependency names that should be excluded from injection.
+
+```python3
+@inject(exclude=['dependency3'])
+def my_function(dep1: Dependency1, dep2: Dependency2, dep3: Dependency3):
+    # Dep3 will not be injected
+    pass
+
+```
+
+In this example, dep3 will not be injected into the function because it is specified in the exclude list.
+
+These parameters provide flexibility in controlling which dependencies are resolved, allowing you to customize the injection behavior according to your specific needs.
```

### Comparing `turbobus-1.0.0a8/pyproject.toml` & `turbobus-1.0.0a9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `turbobus-1.0.0a8/setup.py` & `turbobus-1.0.0a9/setup.py`

 * *Files identical despite different names*

### Comparing `turbobus-1.0.0a8/tests/test.py` & `turbobus-1.0.0a9/tests/test.py`

 * *Files identical despite different names*

### Comparing `turbobus-1.0.0a8/tests/test_command.py` & `turbobus-1.0.0a9/tests/test_command.py`

 * *Files identical despite different names*

### Comparing `turbobus-1.0.0a8/tests/test_constants.py` & `turbobus-1.0.0a9/tests/test_constants.py`

 * *Files identical despite different names*

### Comparing `turbobus-1.0.0a8/turbobus/command.py` & `turbobus-1.0.0a9/turbobus/command.py`

 * *Files identical despite different names*

### Comparing `turbobus-1.0.0a8/turbobus/exception.py` & `turbobus-1.0.0a9/turbobus/exception.py`

 * *Files identical despite different names*

### Comparing `turbobus-1.0.0a8/turbobus/injection.py` & `turbobus-1.0.0a9/turbobus/injection.py`

 * *Files identical despite different names*

### Comparing `turbobus-1.0.0a8/turbobus.egg-info/PKG-INFO` & `turbobus-1.0.0a9/turbobus.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: turbobus
-Version: 1.0.0a8
+Version: 1.0.0a9
 Summary: TurboBus is an opinionated implementation of Command Responsibility Segregation pattern in python.
 Home-page: https://github.com/cafadev/turbobus
-Download-URL: https://github.com/cafadev/turbobus/releases/tag/v1.0.0-alpha.8
+Download-URL: https://github.com/cafadev/turbobus/releases/tag/v1.0.0-alpha.9
 Author: Christopher A. Flores
 Author-email: cafadev@outlook.com
 License: MIT
 Keywords: command,bus,cqrs,commandbus,ddd
 Description-Content-Type: text/markdown
 
 # TurboBus
@@ -201,15 +201,14 @@
     bus = CommandBus()
 
     bus.execute(
         CreateUserAccount(name='Christopher Flores', email='cafadev@outlook.com')
     )
 
 ```
-@inject(alias={ 'logger': 'ILogger' }, only=['logger'], exclude=['x'])
 The `@inject` decorator also accepts the next parameters:
 
 ### Alias
 
 The `@inject` decorator use the typing to resolve the required dependency. With the `alias: dict[str, Callable[..., Any]]` parameter you can specify a different implementation for the same interface. For example, let's say we have a UserRepository interface and then two different implementations; UserRepositoryInMemory and UserRepositorySQL.
 
 ```python3
@@ -225,12 +224,40 @@
 By default, the `@inject` will use the `UserRepositoryInMemory` to provide the dependency. Let's specify the `UserRepositorySQL` as the provider. To accomplish that we just need to specify the parameter name that we want to override, and then the Provider Key:
 
 
 ```python3
 Provider.set(UserRepository, UserRepositoryInMemory)
 Provider.set(UserRepositorySQL, UserRepositorySQL)
 
-@inject(alias = { 'user': 'UserRepositorySQL' })
+@inject(alias={ 'user': 'UserRepositorySQL' })
 class CreateUserAccount:
 
     user: UserRepository
 ```
+
+### Only and Exclude
+The `only` and `exclude` parameters in the `@inject` decorator allow you to fine-tune which dependencies should be resolved based on their names.
+
+The `only` parameter specifies a list of dependency names that should exclusively be resolved. All other dependencies will be ignored.
+
+```python3
+@inject(only=['dependency1', 'dependency2'])
+def my_function(dep1: Dependency1, dep2: Dependency2, dep3: Dependency3):
+    # Only dep1 and dep2 will be injected
+    pass
+```
+
+In this example, only dep1 and dep2 will be injected into the function because they are specified in the only list.
+
+The `exclude` parameter specifies a list of dependency names that should be excluded from injection.
+
+```python3
+@inject(exclude=['dependency3'])
+def my_function(dep1: Dependency1, dep2: Dependency2, dep3: Dependency3):
+    # Dep3 will not be injected
+    pass
+
+```
+
+In this example, dep3 will not be injected into the function because it is specified in the exclude list.
+
+These parameters provide flexibility in controlling which dependencies are resolved, allowing you to customize the injection behavior according to your specific needs.
```

