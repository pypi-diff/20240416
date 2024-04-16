# Comparing `tmp/dailytasks-2.1.2.tar.gz` & `tmp/dailytasks-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dailytasks-2.1.2.tar", last modified: Sat Mar 23 23:22:51 2024, max compression
+gzip compressed data, was "dailytasks-2.1.3.tar", last modified: Tue Apr 16 17:53:50 2024, max compression
```

## Comparing `dailytasks-2.1.2.tar` & `dailytasks-2.1.3.tar`

### file list

```diff
@@ -1,27 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 23:22:51.533082 dailytasks-2.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-23 23:22:47.000000 dailytasks-2.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-23 23:22:47.000000 dailytasks-2.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-03-23 23:22:51.533082 dailytasks-2.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-03-23 23:22:47.000000 dailytasks-2.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 23:22:51.529082 dailytasks-2.1.2/daily_tasks/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-03-23 23:22:47.000000 dailytasks-2.1.2/daily_tasks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 23:22:51.533082 dailytasks-2.1.2/daily_tasks/commands/
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-03-23 23:22:47.000000 dailytasks-2.1.2/daily_tasks/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-03-23 23:22:47.000000 dailytasks-2.1.2/daily_tasks/commands/filter_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-03-23 23:22:47.000000 dailytasks-2.1.2/daily_tasks/commands/info_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-03-23 23:22:47.000000 dailytasks-2.1.2/daily_tasks/commands/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     2897 2024-03-23 23:22:47.000000 dailytasks-2.1.2/daily_tasks/commands/main_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     1862 2024-03-23 23:22:47.000000 dailytasks-2.1.2/daily_tasks/commands/modification_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-03-23 23:22:47.000000 dailytasks-2.1.2/daily_tasks/commands/removal_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     4011 2024-03-23 23:22:47.000000 dailytasks-2.1.2/daily_tasks/commands/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 23:22:51.533082 dailytasks-2.1.2/daily_tasks/data_files/
--rw-r--r--   0 runner    (1001) docker     (127)        2 2024-03-23 23:22:47.000000 dailytasks-2.1.2/daily_tasks/data_files/tasks.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 23:22:51.533082 dailytasks-2.1.2/dailytasks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-03-23 23:22:51.000000 dailytasks-2.1.2/dailytasks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-03-23 23:22:51.000000 dailytasks-2.1.2/dailytasks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-23 23:22:51.000000 dailytasks-2.1.2/dailytasks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-03-23 23:22:51.000000 dailytasks-2.1.2/dailytasks.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-03-23 23:22:51.000000 dailytasks-2.1.2/dailytasks.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-23 23:22:51.000000 dailytasks-2.1.2/dailytasks.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-23 23:22:51.533082 dailytasks-2.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-03-23 23:22:47.000000 dailytasks-2.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:53:50.183582 dailytasks-2.1.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:53:50.175582 dailytasks-2.1.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:53:50.179582 dailytasks-2.1.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-16 17:53:46.000000 dailytasks-2.1.3/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-16 17:53:46.000000 dailytasks-2.1.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-16 17:53:46.000000 dailytasks-2.1.3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-16 17:53:46.000000 dailytasks-2.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-16 17:53:46.000000 dailytasks-2.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    15478 2024-04-16 17:53:50.183582 dailytasks-2.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1955 2024-04-16 17:53:46.000000 dailytasks-2.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:53:50.179582 dailytasks-2.1.3/daily_tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-16 17:53:46.000000 dailytasks-2.1.3/daily_tasks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:53:50.179582 dailytasks-2.1.3/daily_tasks/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-16 17:53:46.000000 dailytasks-2.1.3/daily_tasks/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-04-16 17:53:46.000000 dailytasks-2.1.3/daily_tasks/commands/filter_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-16 17:53:46.000000 dailytasks-2.1.3/daily_tasks/commands/info_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-16 17:53:46.000000 dailytasks-2.1.3/daily_tasks/commands/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2897 2024-04-16 17:53:46.000000 dailytasks-2.1.3/daily_tasks/commands/main_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1862 2024-04-16 17:53:46.000000 dailytasks-2.1.3/daily_tasks/commands/modification_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-04-16 17:53:46.000000 dailytasks-2.1.3/daily_tasks/commands/removal_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4011 2024-04-16 17:53:46.000000 dailytasks-2.1.3/daily_tasks/commands/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:53:50.179582 dailytasks-2.1.3/daily_tasks/data_files/
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2024-04-16 17:53:46.000000 dailytasks-2.1.3/daily_tasks/data_files/tasks.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:53:50.179582 dailytasks-2.1.3/daily_tasks/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 17:53:46.000000 dailytasks-2.1.3/daily_tasks/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-16 17:53:46.000000 dailytasks-2.1.3/daily_tasks/tests/test_main_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-04-16 17:53:46.000000 dailytasks-2.1.3/daily_tasks/tests/test_sub_commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:53:50.183582 dailytasks-2.1.3/dailytasks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15478 2024-04-16 17:53:50.000000 dailytasks-2.1.3/dailytasks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-04-16 17:53:50.000000 dailytasks-2.1.3/dailytasks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 17:53:50.000000 dailytasks-2.1.3/dailytasks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-16 17:53:50.000000 dailytasks-2.1.3/dailytasks.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-16 17:53:50.000000 dailytasks-2.1.3/dailytasks.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-16 17:53:50.000000 dailytasks-2.1.3/dailytasks.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-16 17:53:46.000000 dailytasks-2.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-16 17:53:46.000000 dailytasks-2.1.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 17:53:50.183582 dailytasks-2.1.3/setup.cfg
```

### Comparing `dailytasks-2.1.2/LICENSE` & `dailytasks-2.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dailytasks-2.1.2/README.md` & `dailytasks-2.1.3/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -19,14 +19,26 @@
 
     1.2. This command will create a json file named 'exported_tasks' in the path provided path.
 
 2. After update execute `dailytasks import` command to restore all your data.
 
     2.1. Provide the path provided before (with `-p` option) and all your data will be restore.
 
-**This is because when you update the CLI, data folder ([data_files](./daily_tasks/data_files/)) is overwritten and all your data deleted.**
+   **This is because when you update the CLI, data folder ([data_files](./daily_tasks/data_files/)) is overwritten and all your data deleted.**
+   
+## Testing ##
+
+Running tests locally:
+
+1. Clone this repository.
+
+1. cd into your clone.
+
+2. Use `pytest test` to run all tests, use `pytest test/test_file_name` to run individual tests.
+   
+3. If you get errors around missing daily_task module, reinstall package using `pip install dailytasks`.
 
 ## Contributing ##
 Read [Contributing file](https://github.com/LuisanaMT2005/dailytasks/blob/main/CONTRIBUTING.md) and make whatever question in Discussions.
 
 ### Thanks to: ###
 [Krishnag09](https://github.com/Krishnag09) for contributing closing [#2](https://github.com/LuisanaMTDev/dailytasks/issues/2) and [#8](https://github.com/LuisanaMTDev/dailytasks/issues/8) issues.
```

### Comparing `dailytasks-2.1.2/daily_tasks/commands/filter_commands.py` & `dailytasks-2.1.3/daily_tasks/commands/filter_commands.py`

 * *Files identical despite different names*

### Comparing `dailytasks-2.1.2/daily_tasks/commands/info_commands.py` & `dailytasks-2.1.3/daily_tasks/commands/info_commands.py`

 * *Files identical despite different names*

### Comparing `dailytasks-2.1.2/daily_tasks/commands/main.py` & `dailytasks-2.1.3/daily_tasks/commands/main.py`

 * *Files identical despite different names*

### Comparing `dailytasks-2.1.2/daily_tasks/commands/main_commands.py` & `dailytasks-2.1.3/daily_tasks/commands/main_commands.py`

 * *Files identical despite different names*

### Comparing `dailytasks-2.1.2/daily_tasks/commands/modification_commands.py` & `dailytasks-2.1.3/daily_tasks/commands/modification_commands.py`

 * *Files identical despite different names*

### Comparing `dailytasks-2.1.2/daily_tasks/commands/removal_commands.py` & `dailytasks-2.1.3/daily_tasks/commands/removal_commands.py`

 * *Files identical despite different names*

### Comparing `dailytasks-2.1.2/daily_tasks/commands/utilities.py` & `dailytasks-2.1.3/daily_tasks/commands/utilities.py`

 * *Files identical despite different names*

### Comparing `dailytasks-2.1.2/dailytasks.egg-info/SOURCES.txt` & `dailytasks-2.1.3/dailytasks.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,27 @@
+.gitignore
+CONTRIBUTING.md
 LICENSE
 MANIFEST.in
 README.md
-setup.py
+pyproject.toml
+requirements.txt
+.github/workflows/publish.yml
 daily_tasks/__init__.py
 daily_tasks/commands/__init__.py
 daily_tasks/commands/filter_commands.py
 daily_tasks/commands/info_commands.py
 daily_tasks/commands/main.py
 daily_tasks/commands/main_commands.py
 daily_tasks/commands/modification_commands.py
 daily_tasks/commands/removal_commands.py
 daily_tasks/commands/utilities.py
 daily_tasks/data_files/tasks.json
+daily_tasks/tests/__init__.py
+daily_tasks/tests/test_main_commands.py
+daily_tasks/tests/test_sub_commands.py
 dailytasks.egg-info/PKG-INFO
 dailytasks.egg-info/SOURCES.txt
 dailytasks.egg-info/dependency_links.txt
 dailytasks.egg-info/entry_points.txt
 dailytasks.egg-info/requires.txt
 dailytasks.egg-info/top_level.txt
```

