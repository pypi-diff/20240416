# Comparing `tmp/openjd_cli-0.4.2.tar.gz` & `tmp/openjd_cli-0.4.3.tar.gz`

## Comparing `openjd_cli-0.4.2.tar` & `openjd_cli-0.4.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 openjd_cli-0.4.2/openjd/cli/__init__.py
--rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 openjd_cli-0.4.2/openjd/cli/_create_argparser.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 openjd_cli-0.4.2/openjd/cli/_version.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 openjd_cli-0.4.2/openjd/cli/py.typed
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 openjd_cli-0.4.2/openjd/cli/_check/__init__.py
--rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 openjd_cli-0.4.2/openjd/cli/_check/_check_command.py
--rw-r--r--   0        0        0     5390 2020-02-02 00:00:00.000000 openjd_cli-0.4.2/openjd/cli/_common/__init__.py
--rw-r--r--   0        0        0     4723 2020-02-02 00:00:00.000000 openjd_cli-0.4.2/openjd/cli/_common/_job_from_template.py
--rw-r--r--   0        0        0     2841 2020-02-02 00:00:00.000000 openjd_cli-0.4.2/openjd/cli/_common/_validation_utils.py
--rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 openjd_cli-0.4.2/openjd/cli/_run/__init__.py
--rw-r--r--   0        0        0    17159 2020-02-02 00:00:00.000000 openjd_cli-0.4.2/openjd/cli/_run/_run_command.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 openjd_cli-0.4.2/openjd/cli/_run/_local_session/__init__.py
--rw-r--r--   0        0        0     1982 2020-02-02 00:00:00.000000 openjd_cli-0.4.2/openjd/cli/_run/_local_session/_actions.py
--rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 openjd_cli-0.4.2/openjd/cli/_run/_local_session/_logs.py
--rw-r--r--   0        0        0    13635 2020-02-02 00:00:00.000000 openjd_cli-0.4.2/openjd/cli/_run/_local_session/_session_manager.py
--rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 openjd_cli-0.4.2/openjd/cli/_schema/__init__.py
--rw-r--r--   0        0        0     2559 2020-02-02 00:00:00.000000 openjd_cli-0.4.2/openjd/cli/_schema/_schema_command.py
--rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 openjd_cli-0.4.2/openjd/cli/_summary/__init__.py
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 openjd_cli-0.4.2/openjd/cli/_summary/_summary_command.py
--rw-r--r--   0        0        0     9604 2020-02-02 00:00:00.000000 openjd_cli-0.4.2/openjd/cli/_summary/_summary_output.py
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 openjd_cli-0.4.2/openjd/__main__.py
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 openjd_cli-0.4.2/.gitignore
--rw-r--r--   0        0        0    10142 2020-02-02 00:00:00.000000 openjd_cli-0.4.2/LICENSE
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 openjd_cli-0.4.2/NOTICE
--rw-r--r--   0        0        0    16591 2020-02-02 00:00:00.000000 openjd_cli-0.4.2/README.md
--rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 openjd_cli-0.4.2/hatch.toml
--rw-r--r--   0        0        0     4215 2020-02-02 00:00:00.000000 openjd_cli-0.4.2/pyproject.toml
--rw-r--r--   0        0        0    17744 2020-02-02 00:00:00.000000 openjd_cli-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 openjd_cli-0.4.3/openjd/cli/__init__.py
+-rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 openjd_cli-0.4.3/openjd/cli/_create_argparser.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 openjd_cli-0.4.3/openjd/cli/_version.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 openjd_cli-0.4.3/openjd/cli/py.typed
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 openjd_cli-0.4.3/openjd/cli/_check/__init__.py
+-rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 openjd_cli-0.4.3/openjd/cli/_check/_check_command.py
+-rw-r--r--   0        0        0     5390 2020-02-02 00:00:00.000000 openjd_cli-0.4.3/openjd/cli/_common/__init__.py
+-rw-r--r--   0        0        0     4723 2020-02-02 00:00:00.000000 openjd_cli-0.4.3/openjd/cli/_common/_job_from_template.py
+-rw-r--r--   0        0        0     2841 2020-02-02 00:00:00.000000 openjd_cli-0.4.3/openjd/cli/_common/_validation_utils.py
+-rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 openjd_cli-0.4.3/openjd/cli/_run/__init__.py
+-rw-r--r--   0        0        0    17159 2020-02-02 00:00:00.000000 openjd_cli-0.4.3/openjd/cli/_run/_run_command.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 openjd_cli-0.4.3/openjd/cli/_run/_local_session/__init__.py
+-rw-r--r--   0        0        0     1982 2020-02-02 00:00:00.000000 openjd_cli-0.4.3/openjd/cli/_run/_local_session/_actions.py
+-rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 openjd_cli-0.4.3/openjd/cli/_run/_local_session/_logs.py
+-rw-r--r--   0        0        0    13635 2020-02-02 00:00:00.000000 openjd_cli-0.4.3/openjd/cli/_run/_local_session/_session_manager.py
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 openjd_cli-0.4.3/openjd/cli/_schema/__init__.py
+-rw-r--r--   0        0        0     2559 2020-02-02 00:00:00.000000 openjd_cli-0.4.3/openjd/cli/_schema/_schema_command.py
+-rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 openjd_cli-0.4.3/openjd/cli/_summary/__init__.py
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 openjd_cli-0.4.3/openjd/cli/_summary/_summary_command.py
+-rw-r--r--   0        0        0     9604 2020-02-02 00:00:00.000000 openjd_cli-0.4.3/openjd/cli/_summary/_summary_output.py
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 openjd_cli-0.4.3/openjd/__main__.py
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 openjd_cli-0.4.3/.gitignore
+-rw-r--r--   0        0        0    10142 2020-02-02 00:00:00.000000 openjd_cli-0.4.3/LICENSE
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 openjd_cli-0.4.3/NOTICE
+-rw-r--r--   0        0        0    16397 2020-02-02 00:00:00.000000 openjd_cli-0.4.3/README.md
+-rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 openjd_cli-0.4.3/hatch.toml
+-rw-r--r--   0        0        0     4263 2020-02-02 00:00:00.000000 openjd_cli-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0    17578 2020-02-02 00:00:00.000000 openjd_cli-0.4.3/PKG-INFO
```

### Comparing `openjd_cli-0.4.2/openjd/cli/_create_argparser.py` & `openjd_cli-0.4.3/openjd/cli/_create_argparser.py`

 * *Files identical despite different names*

### Comparing `openjd_cli-0.4.2/openjd/cli/_check/__init__.py` & `openjd_cli-0.4.3/openjd/cli/_check/__init__.py`

 * *Files identical despite different names*

### Comparing `openjd_cli-0.4.2/openjd/cli/_check/_check_command.py` & `openjd_cli-0.4.3/openjd/cli/_check/_check_command.py`

 * *Files identical despite different names*

### Comparing `openjd_cli-0.4.2/openjd/cli/_common/__init__.py` & `openjd_cli-0.4.3/openjd/cli/_common/__init__.py`

 * *Files identical despite different names*

### Comparing `openjd_cli-0.4.2/openjd/cli/_common/_job_from_template.py` & `openjd_cli-0.4.3/openjd/cli/_common/_job_from_template.py`

 * *Files identical despite different names*

### Comparing `openjd_cli-0.4.2/openjd/cli/_common/_validation_utils.py` & `openjd_cli-0.4.3/openjd/cli/_common/_validation_utils.py`

 * *Files identical despite different names*

### Comparing `openjd_cli-0.4.2/openjd/cli/_run/__init__.py` & `openjd_cli-0.4.3/openjd/cli/_run/__init__.py`

 * *Files identical despite different names*

### Comparing `openjd_cli-0.4.2/openjd/cli/_run/_run_command.py` & `openjd_cli-0.4.3/openjd/cli/_run/_run_command.py`

 * *Files identical despite different names*

### Comparing `openjd_cli-0.4.2/openjd/cli/_run/_local_session/_actions.py` & `openjd_cli-0.4.3/openjd/cli/_run/_local_session/_actions.py`

 * *Files identical despite different names*

### Comparing `openjd_cli-0.4.2/openjd/cli/_run/_local_session/_logs.py` & `openjd_cli-0.4.3/openjd/cli/_run/_local_session/_logs.py`

 * *Files identical despite different names*

### Comparing `openjd_cli-0.4.2/openjd/cli/_run/_local_session/_session_manager.py` & `openjd_cli-0.4.3/openjd/cli/_run/_local_session/_session_manager.py`

 * *Files identical despite different names*

### Comparing `openjd_cli-0.4.2/openjd/cli/_schema/__init__.py` & `openjd_cli-0.4.3/openjd/cli/_schema/__init__.py`

 * *Files identical despite different names*

### Comparing `openjd_cli-0.4.2/openjd/cli/_schema/_schema_command.py` & `openjd_cli-0.4.3/openjd/cli/_schema/_schema_command.py`

 * *Files identical despite different names*

### Comparing `openjd_cli-0.4.2/openjd/cli/_summary/__init__.py` & `openjd_cli-0.4.3/openjd/cli/_summary/__init__.py`

 * *Files identical despite different names*

### Comparing `openjd_cli-0.4.2/openjd/cli/_summary/_summary_command.py` & `openjd_cli-0.4.3/openjd/cli/_summary/_summary_command.py`

 * *Files identical despite different names*

### Comparing `openjd_cli-0.4.2/openjd/cli/_summary/_summary_output.py` & `openjd_cli-0.4.3/openjd/cli/_summary/_summary_output.py`

 * *Files identical despite different names*

### Comparing `openjd_cli-0.4.2/openjd/__main__.py` & `openjd_cli-0.4.3/openjd/__main__.py`

 * *Files identical despite different names*

### Comparing `openjd_cli-0.4.2/LICENSE` & `openjd_cli-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `openjd_cli-0.4.2/README.md` & `openjd_cli-0.4.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 ## Open Job Description - CLI
 
 [![pypi](https://img.shields.io/pypi/v/openjd-cli.svg)](https://pypi.python.org/pypi/openjd-cli)
+[![python](https://img.shields.io/pypi/pyversions/openjd-cli.svg?style=flat)](https://pypi.python.org/pypi/openjd-cli)
+[![license](https://img.shields.io/pypi/l/openjd-cli.svg?style=flat)](https://github.com/OpenJobDescription/openjd-cli/blob/mainline/LICENSE)
 
 Open Job Description (OpenJD) is a flexible open specification for defining render jobs which are portable
 between studios and render solutions. This package provides a command-line interface that can be used
 to validate OpenJD templates, run OpenJD jobs locally, and more.
 
 For more information about Open Job Description and our goals with it, please see the
 Open Job Description [Wiki on GitHub](https://github.com/OpenJobDescription/openjd-specifications/wiki).
@@ -13,21 +15,14 @@
 
 This library requires:
 
 1. Python 3.9 or higher;
 2. Linux, MacOS, or Windows operating system;
 3. On Linux/MacOS:
     * `sudo`
-4. On Windows:
-    * PowerShell 5.x
-
-**EXPERIMENTAL** Note that compatibility with the Windows operating system is currently in active development
-and should be considered to be experimental. We recommend that this application not be used in Windows-based
-production environments at this time. We will remove this notice when Windows compatibility is considered
-sufficiently stable and secure for use in Windows-based production environments.
 
 ## Versioning
 
 This package's version follows [Semantic Versioning 2.0](https://semver.org/), but is still considered to be in its 
 initial development, thus backwards incompatible versions are denoted by minor version bumps. To help illustrate how
 versions will increment during this initial development stage, they are described below:
 
@@ -79,15 +74,15 @@
 |`path`|path|yes| A path leading to a Job template file.                                                                                                                                                                                                    |`/path/to/job.template.json`|
 |`--job-param`, `-p`|string, path|no| The values for the job template's parameters. Can be provided as key-value pairs, inline JSON string, or path(s) to a JSON or YAML document. If provided more than once then the given values are combined in the order that they appear. |`--job-param MyParam=5`, `-p file://parameter_file.json`, `-p '{"MyParam": "5"}'`|
 |`--step`|string|no| The name of the Step to summarize.                                                                                                                                                                                                        |`--step Step1`|
 |`--output`|string|no| How to display the results of the command. Allowed values are `human-readable` (default), `json`, and `yaml`.                                                                                                                             |`--output json`, `--output yaml`|
 
 #### Example
 ```sh
-$ openjd-cli summary /path/to/job.template.json \
+$ openjd summary /path/to/job.template.json \
     --job-param JobName=SampleJob \
     --job-param '{"FileToRender": "sample.blend"}' \
     --job-param file://some_more_parameters.json
 
 --- Summary for 'SampleJob' ---
 
 Parameters:
@@ -133,15 +128,15 @@
 |`--path-mapping-rules`|string, path|no| The path mapping rules to apply to the template. Should be a JSON-formatted list of Open Job Description path mapping rules, provided as a string or a path to a JSON/YAML document prefixed with 'file://'.                                                                          |`--path-mapping-rules [{"source_os": "Windows", "source_path": "C:\test", "destination_path": "/mnt/test"}]`, `--path-mapping-rules file://rules_file.json`|
 |`--preserve`|flag|no| If present, the Session's working directory will not be deleted when the run is completed.           |`--preserve`|
 |`--verbose`|flag|no| If present, then verbose logging will be enabled in the Session's log. |`--verbose`|
 |`--output`|string|no| How to display the results of the command. Allowed values are `human-readable` (default), `json`, and `yaml`.                                                                                                                                                                         |`--output json`, `--output yaml`|
 
 #### Example
 ```sh
-$ openjd-cli run /path/to/job.template.json --step Step1 \
+$ openjd run /path/to/job.template.json --step Step1 \
     --job-param PingServer=amazon.com \
     --task-param PingCount=20 \
     --task-param PingDelay=30
 
 # ... Task logs accompanied by timestamps ...
 
 --- Results of local session ---
@@ -162,15 +157,15 @@
 |Name|Type|Required|Description|Example|
 |---|---|---|---|---|
 |`--version`|string|yes|The specification version to get the JSON schema for.|`--version jobtemplate-2023-09`|
 |`--output`|string|no|How to display the results of the command. Allowed values are `human-readable` (default), `json`, and `yaml`.|`--output json`, `--output yaml`|
 
 #### Example
 ```sh
-$ openjd-cli schema --version jobtemplate-2023-09
+$ openjd schema --version jobtemplate-2023-09
 
 {
     "title": "JobTemplate",
     # ... JSON body corresponding to the Open Job Description model schema ...
 }
 ```
```

### Comparing `openjd_cli-0.4.2/hatch.toml` & `openjd_cli-0.4.3/hatch.toml`

 * *Files identical despite different names*

### Comparing `openjd_cli-0.4.2/pyproject.toml` & `openjd_cli-0.4.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 [build-system]
 requires = ["hatchling", "hatch-vcs"]
 build-backend = "hatchling.build"
 
 [project]
 name = "openjd-cli"
+authors = [
+  {name = "Amazon Web Services"},
+]
 dynamic = ["version"]
 readme = "README.md"
 license = "Apache-2.0"
 requires-python = ">=3.9"
 description = "Provides a command-line interface for working with Open Job Description templates."
 # https://pypi.org/classifiers/
 classifiers = [
```

### Comparing `openjd_cli-0.4.2/PKG-INFO` & `openjd_cli-0.4.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: openjd-cli
-Version: 0.4.2
+Version: 0.4.3
 Summary: Provides a command-line interface for working with Open Job Description templates.
 Project-URL: Homepage, https://github.com/OpenJobDescription/openjd-cli
 Project-URL: Source, https://github.com/OpenJobDescription/openjd-cli
+Author: Amazon Web Services
 License-Expression: Apache-2.0
 License-File: LICENSE
 License-File: NOTICE
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: Apache Software License
@@ -24,14 +25,16 @@
 Requires-Dist: openjd-model==0.4.*
 Requires-Dist: openjd-sessions==0.7.*
 Description-Content-Type: text/markdown
 
 ## Open Job Description - CLI
 
 [![pypi](https://img.shields.io/pypi/v/openjd-cli.svg)](https://pypi.python.org/pypi/openjd-cli)
+[![python](https://img.shields.io/pypi/pyversions/openjd-cli.svg?style=flat)](https://pypi.python.org/pypi/openjd-cli)
+[![license](https://img.shields.io/pypi/l/openjd-cli.svg?style=flat)](https://github.com/OpenJobDescription/openjd-cli/blob/mainline/LICENSE)
 
 Open Job Description (OpenJD) is a flexible open specification for defining render jobs which are portable
 between studios and render solutions. This package provides a command-line interface that can be used
 to validate OpenJD templates, run OpenJD jobs locally, and more.
 
 For more information about Open Job Description and our goals with it, please see the
 Open Job Description [Wiki on GitHub](https://github.com/OpenJobDescription/openjd-specifications/wiki).
@@ -40,21 +43,14 @@
 
 This library requires:
 
 1. Python 3.9 or higher;
 2. Linux, MacOS, or Windows operating system;
 3. On Linux/MacOS:
     * `sudo`
-4. On Windows:
-    * PowerShell 5.x
-
-**EXPERIMENTAL** Note that compatibility with the Windows operating system is currently in active development
-and should be considered to be experimental. We recommend that this application not be used in Windows-based
-production environments at this time. We will remove this notice when Windows compatibility is considered
-sufficiently stable and secure for use in Windows-based production environments.
 
 ## Versioning
 
 This package's version follows [Semantic Versioning 2.0](https://semver.org/), but is still considered to be in its 
 initial development, thus backwards incompatible versions are denoted by minor version bumps. To help illustrate how
 versions will increment during this initial development stage, they are described below:
 
@@ -106,15 +102,15 @@
 |`path`|path|yes| A path leading to a Job template file.                                                                                                                                                                                                    |`/path/to/job.template.json`|
 |`--job-param`, `-p`|string, path|no| The values for the job template's parameters. Can be provided as key-value pairs, inline JSON string, or path(s) to a JSON or YAML document. If provided more than once then the given values are combined in the order that they appear. |`--job-param MyParam=5`, `-p file://parameter_file.json`, `-p '{"MyParam": "5"}'`|
 |`--step`|string|no| The name of the Step to summarize.                                                                                                                                                                                                        |`--step Step1`|
 |`--output`|string|no| How to display the results of the command. Allowed values are `human-readable` (default), `json`, and `yaml`.                                                                                                                             |`--output json`, `--output yaml`|
 
 #### Example
 ```sh
-$ openjd-cli summary /path/to/job.template.json \
+$ openjd summary /path/to/job.template.json \
     --job-param JobName=SampleJob \
     --job-param '{"FileToRender": "sample.blend"}' \
     --job-param file://some_more_parameters.json
 
 --- Summary for 'SampleJob' ---
 
 Parameters:
@@ -160,15 +156,15 @@
 |`--path-mapping-rules`|string, path|no| The path mapping rules to apply to the template. Should be a JSON-formatted list of Open Job Description path mapping rules, provided as a string or a path to a JSON/YAML document prefixed with 'file://'.                                                                          |`--path-mapping-rules [{"source_os": "Windows", "source_path": "C:\test", "destination_path": "/mnt/test"}]`, `--path-mapping-rules file://rules_file.json`|
 |`--preserve`|flag|no| If present, the Session's working directory will not be deleted when the run is completed.           |`--preserve`|
 |`--verbose`|flag|no| If present, then verbose logging will be enabled in the Session's log. |`--verbose`|
 |`--output`|string|no| How to display the results of the command. Allowed values are `human-readable` (default), `json`, and `yaml`.                                                                                                                                                                         |`--output json`, `--output yaml`|
 
 #### Example
 ```sh
-$ openjd-cli run /path/to/job.template.json --step Step1 \
+$ openjd run /path/to/job.template.json --step Step1 \
     --job-param PingServer=amazon.com \
     --task-param PingCount=20 \
     --task-param PingDelay=30
 
 # ... Task logs accompanied by timestamps ...
 
 --- Results of local session ---
@@ -189,15 +185,15 @@
 |Name|Type|Required|Description|Example|
 |---|---|---|---|---|
 |`--version`|string|yes|The specification version to get the JSON schema for.|`--version jobtemplate-2023-09`|
 |`--output`|string|no|How to display the results of the command. Allowed values are `human-readable` (default), `json`, and `yaml`.|`--output json`, `--output yaml`|
 
 #### Example
 ```sh
-$ openjd-cli schema --version jobtemplate-2023-09
+$ openjd schema --version jobtemplate-2023-09
 
 {
     "title": "JobTemplate",
     # ... JSON body corresponding to the Open Job Description model schema ...
 }
 ```
```

