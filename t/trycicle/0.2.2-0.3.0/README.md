# Comparing `tmp/trycicle-0.2.2.tar.gz` & `tmp/trycicle-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trycicle-0.2.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "trycicle-0.3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `trycicle-0.2.2.tar` & `trycicle-0.3.0.tar`

### file list

```diff
@@ -1,35 +1,37 @@
--rw-r--r--   0        0        0       83 2024-03-31 15:35:11.648954 trycicle-0.2.2/.gitignore
--rw-r--r--   0        0        0     3570 2024-03-31 15:35:11.648954 trycicle-0.2.2/.gitlab-ci.yml
--rw-r--r--   0        0        0      960 2024-03-31 15:35:11.648954 trycicle-0.2.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0     3146 2024-03-31 15:35:11.648954 trycicle-0.2.2/CHANGELOG.md
--rw-r--r--   0        0        0     1071 2024-03-31 15:35:11.648954 trycicle-0.2.2/LICENSE
--rw-r--r--   0        0        0      596 2024-03-31 15:35:11.648954 trycicle-0.2.2/Pipfile
--rw-r--r--   0        0        0    55711 2024-03-31 15:35:11.649955 trycicle-0.2.2/Pipfile.lock
--rw-r--r--   0        0        0     8779 2024-03-31 15:35:11.649955 trycicle-0.2.2/README.md
--rw-r--r--   0        0        0       53 2024-03-31 15:35:11.649955 trycicle-0.2.2/ci/pipenv/Dockerfile
--rw-r--r--   0        0        0      175 2024-03-31 15:35:11.649955 trycicle-0.2.2/ci/pre-commit/Dockerfile
--rw-r--r--   0        0        0       76 2024-03-31 15:35:11.649955 trycicle-0.2.2/commitlint.config.js
--rw-r--r--   0        0        0     1932 2024-03-31 15:35:11.649955 trycicle-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      102 2024-03-31 15:35:11.649955 trycicle-0.2.2/setup.py
--rw-r--r--   0        0        0      109 2024-03-31 15:35:11.649955 trycicle-0.2.2/tests/basic.yml
--rw-r--r--   0        0        0     2387 2024-03-31 15:35:11.649955 trycicle-0.2.2/tests/conftest.py
--rw-r--r--   0        0        0     1152 2024-03-31 15:35:11.649955 trycicle-0.2.2/tests/example.yml
--rw-r--r--   0        0        0      170 2024-03-31 15:35:11.649955 trycicle-0.2.2/tests/meta.yml
--rw-r--r--   0        0        0      712 2024-03-31 15:35:11.649955 trycicle-0.2.2/tests/references.yml
--rw-r--r--   0        0        0     6621 2024-03-31 15:35:11.649955 trycicle-0.2.2/tests/test_cli.py
--rw-r--r--   0        0        0     1979 2024-03-31 15:35:11.649955 trycicle-0.2.2/tests/test_git_clone.py
--rw-r--r--   0        0        0     5750 2024-03-31 15:35:11.649955 trycicle-0.2.2/tests/test_integration.py
--rw-r--r--   0        0        0     2401 2024-03-31 15:35:11.649955 trycicle-0.2.2/tests/test_models.py
--rw-r--r--   0        0        0     4408 2024-03-31 15:35:11.650955 trycicle-0.2.2/tests/test_parser.py
--rw-r--r--   0        0        0    14772 2024-03-31 15:35:11.650955 trycicle-0.2.2/tests/test_run.py
--rw-r--r--   0        0        0     2552 2024-03-31 15:35:11.650955 trycicle-0.2.2/tests/test_variables.py
--rw-r--r--   0        0        0        0 2024-03-31 15:35:11.675954 trycicle-0.2.2/trycicle/__init__.py
--rw-r--r--   0        0        0       59 2024-03-31 15:35:11.650955 trycicle-0.2.2/trycicle/__main__.py
--rw-r--r--   0        0        0     4320 2024-03-31 15:35:11.650955 trycicle-0.2.2/trycicle/cli.py
--rw-r--r--   0        0        0     1437 2024-03-31 15:35:11.650955 trycicle-0.2.2/trycicle/git_clone.py
--rw-r--r--   0        0        0     2554 2024-03-31 15:35:11.650955 trycicle-0.2.2/trycicle/models.py
--rw-r--r--   0        0        0     3858 2024-03-31 15:35:11.650955 trycicle-0.2.2/trycicle/parser.py
--rw-r--r--   0        0        0     8987 2024-03-31 15:35:11.650955 trycicle-0.2.2/trycicle/run.py
--rw-r--r--   0        0        0      517 2024-03-31 15:35:11.650955 trycicle-0.2.2/trycicle/subprocess.py
--rw-r--r--   0        0        0     5109 2024-03-31 15:35:11.650955 trycicle-0.2.2/trycicle/variables.py
--rw-r--r--   0        0        0     9259 1970-01-01 00:00:00.000000 trycicle-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0       83 2024-04-16 12:08:46.918705 trycicle-0.3.0/.gitignore
+-rw-r--r--   0        0        0     3570 2024-04-16 12:08:46.918705 trycicle-0.3.0/.gitlab-ci.yml
+-rw-r--r--   0        0        0      960 2024-04-16 12:08:46.918705 trycicle-0.3.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     4714 2024-04-16 12:08:46.918705 trycicle-0.3.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1071 2024-04-16 12:08:46.918705 trycicle-0.3.0/LICENSE
+-rw-r--r--   0        0        0      615 2024-04-16 12:08:46.918705 trycicle-0.3.0/Pipfile
+-rw-r--r--   0        0        0    56080 2024-04-16 12:08:46.918705 trycicle-0.3.0/Pipfile.lock
+-rw-r--r--   0        0        0     9417 2024-04-16 12:08:46.918705 trycicle-0.3.0/README.md
+-rw-r--r--   0        0        0       53 2024-04-16 12:08:46.918705 trycicle-0.3.0/ci/pipenv/Dockerfile
+-rw-r--r--   0        0        0      175 2024-04-16 12:08:46.918705 trycicle-0.3.0/ci/pre-commit/Dockerfile
+-rw-r--r--   0        0        0       76 2024-04-16 12:08:46.918705 trycicle-0.3.0/commitlint.config.js
+-rw-r--r--   0        0        0     1959 2024-04-16 12:08:46.919705 trycicle-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      102 2024-04-16 12:08:46.919705 trycicle-0.3.0/setup.py
+-rw-r--r--   0        0        0      109 2024-04-16 12:08:46.919705 trycicle-0.3.0/tests/basic.yml
+-rw-r--r--   0        0        0     2387 2024-04-16 12:08:46.919705 trycicle-0.3.0/tests/conftest.py
+-rw-r--r--   0        0        0     1152 2024-04-16 12:08:46.919705 trycicle-0.3.0/tests/example.yml
+-rw-r--r--   0        0        0     1053 2024-04-16 12:08:46.919705 trycicle-0.3.0/tests/extends.yml
+-rw-r--r--   0        0        0      170 2024-04-16 12:08:46.919705 trycicle-0.3.0/tests/meta.yml
+-rw-r--r--   0        0        0      712 2024-04-16 12:08:46.919705 trycicle-0.3.0/tests/references.yml
+-rw-r--r--   0        0        0     3794 2024-04-16 12:08:46.919705 trycicle-0.3.0/tests/test_cache.py
+-rw-r--r--   0        0        0     6455 2024-04-16 12:08:46.919705 trycicle-0.3.0/tests/test_cli.py
+-rw-r--r--   0        0        0     1979 2024-04-16 12:08:46.919705 trycicle-0.3.0/tests/test_git_clone.py
+-rw-r--r--   0        0        0     6099 2024-04-16 12:08:46.919705 trycicle-0.3.0/tests/test_integration.py
+-rw-r--r--   0        0        0     8379 2024-04-16 12:08:46.919705 trycicle-0.3.0/tests/test_parser.py
+-rw-r--r--   0        0        0    15172 2024-04-16 12:08:46.919705 trycicle-0.3.0/tests/test_run.py
+-rw-r--r--   0        0        0     2552 2024-04-16 12:08:46.919705 trycicle-0.3.0/tests/test_variables.py
+-rw-r--r--   0        0        0        0 2024-04-16 12:08:46.947704 trycicle-0.3.0/trycicle/__init__.py
+-rw-r--r--   0        0        0       59 2024-04-16 12:08:46.919705 trycicle-0.3.0/trycicle/__main__.py
+-rw-r--r--   0        0        0     2149 2024-04-16 12:08:46.919705 trycicle-0.3.0/trycicle/cache.py
+-rw-r--r--   0        0        0     4417 2024-04-16 12:08:46.920705 trycicle-0.3.0/trycicle/cli.py
+-rw-r--r--   0        0        0     1437 2024-04-16 12:08:46.920705 trycicle-0.3.0/trycicle/git_clone.py
+-rw-r--r--   0        0        0     2004 2024-04-16 12:08:46.920705 trycicle-0.3.0/trycicle/models.py
+-rw-r--r--   0        0        0     6923 2024-04-16 12:08:46.920705 trycicle-0.3.0/trycicle/parser.py
+-rw-r--r--   0        0        0     9652 2024-04-16 12:08:46.920705 trycicle-0.3.0/trycicle/run.py
+-rw-r--r--   0        0        0      517 2024-04-16 12:08:46.920705 trycicle-0.3.0/trycicle/subprocess.py
+-rw-r--r--   0        0        0     5109 2024-04-16 12:08:46.920705 trycicle-0.3.0/trycicle/variables.py
+-rw-r--r--   0        0        0     9932 1970-01-01 00:00:00.000000 trycicle-0.3.0/PKG-INFO
```

### Comparing `trycicle-0.2.2/.gitlab-ci.yml` & `trycicle-0.3.0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `trycicle-0.2.2/.pre-commit-config.yaml` & `trycicle-0.3.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `trycicle-0.2.2/CHANGELOG.md` & `trycicle-0.3.0/CHANGELOG.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,54 @@
 # CHANGELOG
 
 
 
+## v0.3.0 (2024-04-16)
+
+### Documentation
+
+* docs: add cache example to readme ([`dfc5336`](https://gitlab.com/phooijenga/trycicle/-/commit/dfc5336bed36ac37c10d65a1979f8f22af6bbef8))
+
+### Feature
+
+* feat: refactor how extends are applied
+
+Previously the parser would construct a set of partial job objects.
+When a job was requested from the config, it would resolve each field
+independenly, following the extends keyword to parent jobs if necessary.
+
+This meant that to merge fields like `variables`, special handling was
+necessary, which was not available to other fields (like `cache`).
+
+The parser now merges values from `extends`, `default` and globals in
+the same way (and only when the job is requested from the config). ([`b2cb7ea`](https://gitlab.com/phooijenga/trycicle/-/commit/b2cb7ea332b0989e3ea12cc6e283f72994092110))
+
+* feat: implement caches ([`d2dce55`](https://gitlab.com/phooijenga/trycicle/-/commit/d2dce554de404deb17adc0ba719fa2ddee793882))
+
+### Fix
+
+* fix: add source directory name to cache key ([`3a2eb24`](https://gitlab.com/phooijenga/trycicle/-/commit/3a2eb242e6fd8d498b5f2cb7402bf917134ea04e))
+
+* fix: ensure directories exist when copying cache ([`f813d6f`](https://gitlab.com/phooijenga/trycicle/-/commit/f813d6f44b81473abe475a909dccfa69a62c7639))
+
+* fix: use user cache directory ([`5356312`](https://gitlab.com/phooijenga/trycicle/-/commit/535631254c76b2999a6218f08fc0787690a752cd))
+
+* fix: allow cache without key ([`0d83b73`](https://gitlab.com/phooijenga/trycicle/-/commit/0d83b7347197010b6d6317091d3e555c3b2176d2))
+
+### Test
+
+* test: add cache test ([`a4d9c4c`](https://gitlab.com/phooijenga/trycicle/-/commit/a4d9c4ce229a967671c90d640900ca90e432888b))
+
+
 ## v0.2.2 (2024-03-31)
 
+### Chore
+
+* chore(release): version 0.2.2 ([`8e574c6`](https://gitlab.com/phooijenga/trycicle/-/commit/8e574c69e96d0334ef167994e681eba825abfa43))
+
 ### Fix
 
 * fix(ci): skip version job only ([`4d01c5e`](https://gitlab.com/phooijenga/trycicle/-/commit/4d01c5ea12619264ad098c27bd7280190f0c21de))
 
 
 ## v0.2.1 (2024-03-31)
 
@@ -69,11 +110,7 @@
 * Reset log level before running integration tests ([`1f66207`](https://gitlab.com/phooijenga/trycicle/-/commit/1f66207eccffadb6f796ee7a8f540a8aae3a6bca))
 
 * Add instructions to set up tab completion to readme
 
 Closes #7. ([`14ce3a8`](https://gitlab.com/phooijenga/trycicle/-/commit/14ce3a821be9f4fff4e100429be79de04d292150))
 
 * Add shell completion for jobs and variables ([`cdbc707`](https://gitlab.com/phooijenga/trycicle/-/commit/cdbc70793f456fbf211aa23677a0718db48674fc))
-
-* Use Click for command-line parsing ([`9688967`](https://gitlab.com/phooijenga/trycicle/-/commit/9688967a92fea89fe75e46a261ea4b203119cac7))
-
-* Display service logs ([`09b9055`](https://gitlab.com/phooijenga/trycicle/-/commit/09b9055b64510a85a2a2bd5992a83f9a36b3bc6d))
```

### Comparing `trycicle-0.2.2/LICENSE` & `trycicle-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trycicle-0.2.2/Pipfile` & `trycicle-0.3.0/Pipfile`

 * *Files 20% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 ci-coverage = "python -m pytest --junit-xml report.xml --cov trycicle/ --cov-branch --cov-fail-under 100 --cov-report term --cov-report xml"
 type-check = "mypy trycicle tests"
 
 [packages]
 pyyaml = "*"
 docker = "*"
 click = "*"
+platformdirs = "*"
 
 [dev-packages]
 pytest = "*"
 pytest-cov = "*"
 mypy = "*"
 types-pyyaml = "*"
 python-semantic-release = "*"
```

### Comparing `trycicle-0.2.2/Pipfile.lock` & `trycicle-0.3.0/Pipfile.lock`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9729166666666668%*

 * *Differences: {"'_meta'": "{'hash': {'sha256': "*

 * *            "'a87446fbc0cbc9548cc1980f26be8b79d161cc9e8594872ba2b23e93d943b7f4'}}",*

 * * "'default'": "{'platformdirs': OrderedDict([('hashes', "*

 * *              "['sha256:0614df2a2f37e1a662acbd8e2b25b92ccf8632929bc6d43467e17fe89c75e068', "*

 * *              "'sha256:ef0cc731df711022c174543cb70a9b5bd22e5a9337c8624ef2c2ceb8ddad8768']), "*

 * *              '(\'index\', \'pypi\'), (\'markers\', "python_version >= \'3.8\'"), (\'version\', '*

 * *              "'==4.2.0')])}"}*

```diff
@@ -1,11 +1,11 @@
 {
     "_meta": {
         "hash": {
-            "sha256": "4509cbfc76563634e9c1f7f7a9e545f6a4466ea5590a63272771f078e945e691"
+            "sha256": "a87446fbc0cbc9548cc1980f26be8b79d161cc9e8594872ba2b23e93d943b7f4"
         },
         "pipfile-spec": 6,
         "requires": {
             "python_version": "3.11"
         },
         "sources": [
             {
@@ -150,14 +150,23 @@
             "hashes": [
                 "sha256:2ddfb553fdf02fb784c234c7ba6ccc288296ceabec964ad2eae3777778130bc5",
                 "sha256:eb82c5e3e56209074766e6885bb04b8c38a0c015d0a30036ebe7ece34c9989e9"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==24.0"
         },
+        "platformdirs": {
+            "hashes": [
+                "sha256:0614df2a2f37e1a662acbd8e2b25b92ccf8632929bc6d43467e17fe89c75e068",
+                "sha256:ef0cc731df711022c174543cb70a9b5bd22e5a9337c8624ef2c2ceb8ddad8768"
+            ],
+            "index": "pypi",
+            "markers": "python_version >= '3.8'",
+            "version": "==4.2.0"
+        },
         "pyyaml": {
             "hashes": [
                 "sha256:04ac92ad1925b2cff1db0cfebffb6ffc43457495c9b3c39d3fcae417d7125dc5",
                 "sha256:062582fca9fabdd2c8b54a3ef1c978d786e0f6b3a1510e0ac93ef59e0ddae2bc",
                 "sha256:0d3304d8c0adc42be59c5f8a4d9e3d7379e6955ad754aa9d6ab7a398b59dd1df",
                 "sha256:1635fd110e8d85d55237ab316b5b011de701ea0f29d07611174a1b42f1444741",
                 "sha256:184c5108a2aca3c5b3d3bf9395d50893a7ab82a38004c8f61c258d4428e80206",
```

### Comparing `trycicle-0.2.2/README.md` & `trycicle-0.3.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+Metadata-Version: 2.1
+Name: trycicle
+Version: 0.3.0
+Summary: Try CI jobs locally
+Author-email: Paul Hooijenga <paul@founda.com>
+Requires-Python: ~= 3.11
+Description-Content-Type: text/markdown
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: POSIX
+Classifier: License :: OSI Approved :: MIT License
+Requires-Dist: pyyaml ~= 6.0
+Requires-Dist: docker ~= 7.0
+Requires-Dist: click ~= 8.1
+Requires-Dist: platformdirs ~= 4.2
+Project-URL: Homepage, https://gitlab.com/phooijenga/trycicle
+
 # Trycicle
 
 Try CI jobs locally, including services.
 
 ## Installation
 
     pipx install trycicle
@@ -276,14 +292,52 @@
 nothing to commit, working tree clean
 ```
 
 As you can see, only the committed changes are visible to the job.
 Trycicle adds your source directory as a remote to the clean copy, this makes it possible to use `git fetch` in the job.
 Pushing does not work, your working directory is mounted read-only.
 
+### Caching
+
+Trycicle has rudimentary support for caching. If a job defines a `cache` key, Trycicle will keep matching files between runs.
+
+```yaml
+image: busybox:latest
+
+cache:
+  key: example
+  paths:
+    - "*.txt"
+
+one:
+  script:
+    - echo 'Hello, world!' > hello.txt
+
+two:
+  script:
+    - cat hello.txt
+```
+
+Running the first job will create a cache with the `hello.txt` file:
+
+```console
+$ trycicle one
+INFO:trycicle.cache:Using cache 'cache-readme-example'
+...
+```
+
+The second job will be able to read the file from the cache:
+
+```console
+$ trycicle two
+INFO:trycicle.cache:Using cache 'cache-readme-example'
+...
+Hello, world!
+```
+
 ## Debugging
 
 ### Logs
 
 Trycicle does not immediately remove the containers it creates, so you can inspect them after the job has finished.
 The containers are labeled with the job they were part of, so you can use a command like `docker ps -a --filter label=trycicle.job=test` to list them.
 This can also be combined with `docker logs`, for example to get the logs of `postgresql` service in the most recent run:
@@ -304,7 +358,8 @@
 ### Interactive debugging
 
 Trycicle can run a job in interactive mode, which means you can execute commands in the container after the job has finished.
 This is useful to inspect the state of the container, check environment variables, or find out what that missing package is called.
 
 The debug shell will start automatically when the job fails, you can also add a `debugger` command to the script to start it manually.
 To enter the debug shell before the job starts, use the `--debug=immediate` option.
+
```

### Comparing `trycicle-0.2.2/pyproject.toml` & `trycicle-0.3.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 [project]
 name = "trycicle"
-version = "0.2.2"
+version = "0.3.0"
 description = "Try CI jobs locally"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: POSIX",
     "License :: OSI Approved :: MIT License",
 ]
 requires-python = "~= 3.11"
 dependencies = [
     "pyyaml ~= 6.0",
     "docker ~= 7.0",
     "click ~= 8.1",
+    "platformdirs ~= 4.2",
 ]
 
 [[project.authors]]
 name = "Paul Hooijenga"
 email = "paul@founda.com"
 
 [project.urls]
```

### Comparing `trycicle-0.2.2/tests/conftest.py` & `trycicle-0.3.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `trycicle-0.2.2/tests/example.yml` & `trycicle-0.3.0/tests/example.yml`

 * *Files identical despite different names*

### Comparing `trycicle-0.2.2/tests/references.yml` & `trycicle-0.3.0/tests/references.yml`

 * *Files identical despite different names*

### Comparing `trycicle-0.2.2/tests/test_cli.py` & `trycicle-0.3.0/tests/test_cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,29 +3,25 @@
 from unittest import mock
 
 import pytest
 from click.shell_completion import ShellComplete
 from click.testing import CliRunner, Result
 
 from trycicle.cli import main
-from trycicle.models import Config, JobImage, PartialJob
+from trycicle.models import Config
 
 
 @pytest.fixture(name="parse_config")
 def mock_parse_config() -> typing.Iterable[mock.MagicMock]:
-    defaults = PartialJob(
-        extends=[],
-        image=JobImage(name="busybox:latest"),
-        before_script=[],
-        script=[],
+    config = Config(
+        globals={"image": "busybox:latest"},
+        default={},
         variables={},
-        services=[],
+        jobs={"deploy": {}},
     )
-    deploy_job = PartialJob(extends=[])
-    config = Config(defaults, {"deploy": deploy_job})
 
     with mock.patch("trycicle.cli.parse_config") as parse_config:
         parse_config.return_value = config
         yield parse_config
 
 
 @pytest.fixture(name="run_job")
@@ -59,15 +55,15 @@
     assert parse_config.call_args.args[0].name == ".gitlab-ci.yml"
 
     assert "Available jobs:" in result.stderr
     assert "  - deploy" in result.stderr
 
 
 def test_job_list_does_not_include_templates(parse_config: mock.MagicMock) -> None:
-    parse_config.return_value.jobs[".hidden"] = PartialJob(extends=[])
+    parse_config.return_value.jobs[".hidden"] = {}
 
     result = run_main()
     assert result.exit_code == 0
 
     assert ".hidden" not in result.stderr
 
 
@@ -134,15 +130,15 @@
     # Remove existing handlers, otherwise the basicConfig call will do nothing
     root_logger = logging.getLogger()
     for h in root_logger.handlers[:]:
         root_logger.removeHandler(h)
         h.close()
 
     result = CliRunner().invoke(main, ["--verbose"] * verbose)
-    assert result.exit_code == 0
+    assert result.exit_code == 0, result.stdout
 
     assert logging.getLevelName(root_logger.level) == root_level
     assert logging.getLevelName(logging.getLogger("trycicle").level) == package_level
 
 
 @pytest.mark.parametrize(
     "incomplete,file,expected",
```

### Comparing `trycicle-0.2.2/tests/test_git_clone.py` & `trycicle-0.3.0/tests/test_git_clone.py`

 * *Files identical despite different names*

### Comparing `trycicle-0.2.2/tests/test_integration.py` & `trycicle-0.3.0/tests/test_integration.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,16 +9,18 @@
 import sys
 import time
 import typing
 from unittest import mock
 
 import pytest
 
+from trycicle.cache import get_cache_path
 from trycicle.cli import main
-from trycicle.variables import slugify
+from trycicle.models import Cache
+from trycicle.variables import Variables, slugify
 
 
 def test_basic_job(capfd: pytest.CaptureFixture[str]) -> None:
     with pytest.raises(SystemExit, match="0"):
         main(["--verbose", "--file", "tests/basic.yml", "job"])
 
     out, err = capfd.readouterr()
@@ -80,14 +82,18 @@
             [
                 pytest.param(example, id=slugify(example.section))
                 for example in examples
             ],
         )
 
 
+def get_readme_cache_path(cache: Cache, variables: Variables, source_dir: str) -> str:
+    return get_cache_path(cache, variables, "readme")
+
+
 def test_readme_example(
     monkeypatch: pytest.MonkeyPatch,
     readme_example: Example,
     tmp_path: pathlib.Path,
     capfd: pytest.CaptureFixture[str],
     get_commit_variables: mock.MagicMock,
     get_project_variables: mock.MagicMock,
@@ -100,15 +106,18 @@
     # Send logs to stdout to simplify test
     logging.basicConfig(level=logging.INFO, stream=sys.stdout, force=True)
     logging.getLogger("trycicle").setLevel(logging.NOTSET)
 
     for command in readme_example.commands:
         args = shlex.split(command)
         if args[0] == "trycicle":
-            with pytest.raises(SystemExit, match="0"):
+            with (
+                pytest.raises(SystemExit, match="0"),
+                mock.patch("trycicle.run.get_cache_path", new=get_readme_cache_path),
+            ):
                 main(["--file", str(config), *args[1:]])
         else:
             subprocess.run(command, check=True, shell=True, cwd=tmp_path)
 
     output = capfd.readouterr().out.splitlines()
     i, skip = 0, False
     for line in readme_example.expected:
```

### Comparing `trycicle-0.2.2/tests/test_run.py` & `trycicle-0.3.0/tests/test_run.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import pathlib
 import typing
 from unittest import mock
 
 import pytest
 from docker.errors import ImageNotFound
 
-from trycicle.models import Job, JobImage, Service
+from trycicle.models import Cache, Job, JobImage, Service
 from trycicle.run import (
     DockerEvent,
     consume_events,
     create_container,
     job_script_debugger,
     job_script_header,
     job_script_shebang,
@@ -77,34 +77,27 @@
         yield client
 
 
 def test_run(docker_client: mock.MagicMock) -> None:
     job = Job(
         name="test",
         image=JobImage(name="busybox:latest"),
-        before_script=[],
-        script=[],
-        variables={},
-        services=[],
     )
     run_job(job, "", "")
 
     assert docker_client.containers.create.call_count == 1
     run_args = docker_client.containers.create.call_args
     assert run_args.kwargs["image"] == "busybox:latest"
     assert run_args.kwargs["command"] == ["/build/job.sh"]
 
 
 def test_run_service(docker_client: mock.MagicMock) -> None:
     job = Job(
         name="test",
         image=JobImage(name="busybox:latest"),
-        before_script=[],
-        script=[],
-        variables={},
         services=[Service("mysql:latest", "mysql")],
     )
     run_job(job, "", "")
 
     assert docker_client.containers.create.call_count == 2
     service_args = docker_client.containers.create.call_args_list[0]
     assert service_args.kwargs["image"] == "mysql:latest"
@@ -117,17 +110,14 @@
     assert docker_client.containers.create.return_value.stop.call_count == 1
 
 
 def test_run_labels(docker_client: mock.MagicMock) -> None:
     job = Job(
         name="test",
         image=JobImage(name="busybox:latest"),
-        before_script=[],
-        script=[],
-        variables={},
         services=[Service("mysql:latest", "mysql")],
     )
     run_job(job, "", "")
 
     assert docker_client.containers.create.call_count == 2
     service_args = docker_client.containers.create.call_args_list[0]
     service_labels = service_args.kwargs["labels"]
@@ -147,17 +137,14 @@
     }
 
 
 def test_run_service_command(docker_client: mock.MagicMock) -> None:
     job = Job(
         name="test",
         image=JobImage("busybox:latest"),
-        before_script=[],
-        script=[],
-        variables={},
         services=[
             Service(
                 "mysql:latest",
                 "mysql",
                 entrypoint=["exec"],
                 command=["ls"],
             )
@@ -174,16 +161,14 @@
     assert docker_client.containers.create.return_value.stop.call_count == 1
 
 
 def test_run_service_specific_variables(docker_client: mock.MagicMock) -> None:
     job = Job(
         name="test",
         image=JobImage(name="busybox:latest"),
-        before_script=[],
-        script=[],
         variables={"FOO": "bar"},
         services=[
             Service(
                 "postgres:latest",
                 "postgres",
                 variables={"POSTGRES_PASSWORD": "test"},
             )
@@ -208,17 +193,14 @@
     assert "POSTGRES_PASSWORD" not in job_environment
 
 
 def test_run_extra_dind_flags(docker_client: mock.MagicMock) -> None:
     job = Job(
         name="test",
         image=JobImage(name="busybox:latest"),
-        before_script=[],
-        script=[],
-        variables={},
         services=[Service("docker:dind", "docker")],
     )
     run_job(job, "", "")
 
     assert docker_client.containers.create.call_count == 2
     service_args = docker_client.containers.create.call_args_list[0]
     assert service_args.kwargs["image"] == "docker:dind"
@@ -231,36 +213,28 @@
     assert job_volumes["dind-certs"] == service_volumes["dind-certs"]
 
 
 def test_run_entrypoint(docker_client: mock.MagicMock) -> None:
     job = Job(
         name="test",
         image=JobImage(name="busybox:latest", entrypoint=["/bin/sh", "-c"]),
-        before_script=[],
-        script=[],
-        variables={},
-        services=[],
     )
     run_job(job, "", "")
 
     assert docker_client.containers.create.call_count == 1
     run_args = docker_client.containers.create.call_args
     assert run_args.kwargs["image"] == "busybox:latest"
     assert run_args.kwargs["entrypoint"] == ["/bin/sh", "-c"]
     assert run_args.kwargs["command"] == ["/build/job.sh"]
 
 
 def test_run_original_volume(docker_client: mock.MagicMock) -> None:
     job = Job(
         name="test",
         image=JobImage(name="busybox:latest"),
-        before_script=[],
-        script=[],
-        variables={},
-        services=[],
     )
     run_job(job, "source", "original")
 
     assert docker_client.containers.create.call_count == 1
     run_args = docker_client.containers.create.call_args
     volumes = run_args.kwargs["volumes"]
     assert any(
@@ -275,17 +249,14 @@
 
 def test_run_with_logs(
     docker_client: mock.MagicMock, capsys: pytest.CaptureFixture[str]
 ) -> None:
     job = Job(
         name="test",
         image=JobImage(name="busybox:latest"),
-        before_script=[],
-        script=[],
-        variables={},
         services=[
             Service(
                 "postgres:latest",
                 "postgres",
             ),
         ],
     )
@@ -297,27 +268,61 @@
 
 
 def test_run_with_debugger(docker_client: mock.MagicMock) -> None:
     with mock.patch("trycicle.run.run_command") as run_command:
         job = Job(
             name="test",
             image=JobImage(name="busybox:latest"),
-            before_script=[],
-            script=[],
-            variables={},
-            services=[],
         )
         run_job(job, "", "", debugger="true")
 
     assert run_command.call_count == 1
     command = run_command.call_args.args[0]
     assert command[:2] == ["docker", "start"]
     assert command[-1] == "id-1"
 
 
+def test_run_with_cache(docker_client: mock.MagicMock) -> None:
+    job = Job(
+        name="test",
+        image=JobImage(name="busybox:latest"),
+        cache=[Cache(policy="pull-push", paths=["test"])],
+    )
+    with (
+        mock.patch("trycicle.run.pull_cache") as pull_cache,
+        mock.patch("trycicle.run.push_cache") as push_cache,
+    ):
+        run_job(job, "", "")
+
+    pull_cache.assert_called_once()
+    push_cache.assert_called_once()
+
+
+def test_run_with_cache_push_when(docker_client: mock.MagicMock) -> None:
+    always = Cache()
+    on_success = Cache(when="on_success")
+    on_failure = Cache(when="on_failure")
+
+    job = Job(
+        name="test",
+        image=JobImage(name="busybox:latest"),
+        cache=[always, on_success, on_failure],
+    )
+    with (
+        mock.patch("trycicle.run.pull_cache") as pull_cache,
+        mock.patch("trycicle.run.push_cache") as push_cache,
+    ):
+        run_job(job, "", "")
+
+    assert pull_cache.call_count == 3
+    assert push_cache.call_count == 2
+    assert push_cache.call_args_list[0].args[0] is always
+    assert push_cache.call_args_list[1].args[0] is on_success
+
+
 @pytest.mark.parametrize(
     "events,expected",
     [
         pytest.param(
             [
                 {
                     "Type": "container",
```

### Comparing `trycicle-0.2.2/tests/test_variables.py` & `trycicle-0.3.0/tests/test_variables.py`

 * *Files identical despite different names*

### Comparing `trycicle-0.2.2/trycicle/cli.py` & `trycicle-0.3.0/trycicle/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import logging
 import os
 import sys
 import typing
 
 import click
+import platformdirs
 from click.shell_completion import CompletionItem
 
 from .git_clone import create_clean_copy, remove_copy
 from .models import Job
 from .parser import parse_config
 from .run import DebugEnabled, run_job
 
@@ -21,19 +22,15 @@
     variable_names: set[str] = set()
     if ctx.params["file"]:
         try:
             config = parse_config(ctx.params["file"])
         except Exception:
             pass
         else:
-            if config.defaults.variables:
-                variable_names |= config.defaults.variables.keys()
-            for job in config.jobs.values():
-                if job.variables:
-                    variable_names |= job.variables.keys()
+            variable_names = config.all_variable_names()
 
     variables = [
         CompletionItem(k, help="Variable")
         for k in sorted(variable_names)
         if k.startswith(incomplete)
     ]
 
@@ -107,14 +104,21 @@
     "--debug",
     type=click.Choice(("true", "false", "immediate"), case_sensitive=False),
     is_flag=False,
     flag_value="true",
     default="false",
     help="Enable interactive debugging",
 )
+@click.option(
+    "--cache-directory",
+    type=click.Path(file_okay=False, dir_okay=True),
+    metavar="DIR",
+    help="Directory to store cache files",
+    default=platformdirs.user_cache_dir("trycicle"),
+)
 @click.argument(
     "job_name",
     metavar="JOB",
     required=False,
     shell_complete=complete_job,
 )
 def main(
@@ -122,14 +126,15 @@
     service_logs: bool,
     workdir: str | None,
     clean: bool,
     env: list[str],
     file: typing.TextIO,
     job_name: str | None,
     debug: DebugEnabled,
+    cache_directory: str,
 ) -> None:
     configure_logging(verbose)
 
     config = parse_config(file)
     if job_name not in config.jobs:
         if job_name is not None:
             click.echo(f"Job {job_name!r} not found in {file!r}", err=True)
@@ -143,15 +148,17 @@
     set_variables(job, env)
 
     source_dir = workdir or os.path.dirname(file.name)
     original_dir = source_dir
     if clean:
         source_dir = create_clean_copy(original_dir)
 
-    result = run_job(job, source_dir, original_dir, service_logs, debug)
+    result = run_job(
+        job, source_dir, original_dir, service_logs, debug, cache_directory
+    )
 
     if clean:
         remove_copy(source_dir)
 
     sys.exit(result)
```

### Comparing `trycicle-0.2.2/trycicle/git_clone.py` & `trycicle-0.3.0/trycicle/git_clone.py`

 * *Files identical despite different names*

### Comparing `trycicle-0.2.2/trycicle/models.py` & `trycicle-0.3.0/trycicle/models.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import dataclasses
 import typing
-from collections import deque
+
+Dict: typing.TypeAlias = dict[str, typing.Any]
 
 
 @dataclasses.dataclass
 class Reference:
     path: list[str]
 
 
@@ -24,69 +25,48 @@
 @dataclasses.dataclass
 class JobImage:
     name: str
     entrypoint: list[str] | None = None
 
 
 @dataclasses.dataclass
-class PartialJob:
-    extends: list[str]
-    image: JobImage | None = None
-    before_script: list[str] | None = None
-    script: list[str] | None = None
-    variables: dict[str, str] | None = None
-    services: list[Service] | None = None
+class Cache:
+    key: str | None = None
+    key_files: list[str] | None = None
+    key_prefix: str | None = None
+    paths: list[str] | None = None  # Array of globs relative to CI_PROJECT_DIR
+    untracked: bool = False
+    when: typing.Literal["on_success", "on_failure", "always"] = "on_success"
+    policy: typing.Literal["pull", "push", "pull-push"] = "pull-push"
 
 
 @dataclasses.dataclass
 class Job:
     name: str
     image: JobImage
-    before_script: list[str]
-    script: list[str]
-    variables: dict[str, str]
-    services: list[Service]
+    before_script: list[str] = dataclasses.field(default_factory=list)
+    script: list[str] = dataclasses.field(default_factory=list)
+    after_script: list[str] = dataclasses.field(default_factory=list)
+    variables: dict[str, str] = dataclasses.field(default_factory=dict)
+    services: list[Service] = dataclasses.field(default_factory=list)
+    cache: list[Cache] = dataclasses.field(default_factory=list)
 
 
 @dataclasses.dataclass
 class Config:
-    defaults: PartialJob
-    jobs: dict[str, PartialJob]
-
-    def all_parents(self, name: str) -> typing.Iterable[PartialJob]:
-        jobs = deque([name])
-        while jobs:
-            job = self.jobs[jobs.popleft()]
-            yield job
-            jobs.extendleft(job.extends)
-        yield self.defaults
-
-    def resolve_field(self, name: str, field: str) -> typing.Any:
-        for job in self.all_parents(name):
-            if (value := getattr(job, field)) is not None:
-                return value
-        raise KeyError(f"Unable to resolve field {field!r} for job {name!r}")
-
-    def merge_fields(self, name: str, field: str) -> dict[str, str]:
-        merged: dict[str, str] = {}
-        for job in self.all_parents(name):
-            if values := getattr(job, field):
-                for key, value in values.items():
-                    merged.setdefault(key, str(value))
-        return merged
-
-    def append_fields(self, name: str, field: str) -> list[typing.Any]:
-        merged = []
-        for job in self.all_parents(name):
-            if values := getattr(job, field):
-                merged += values
-        return merged
+    globals: Dict
+    default: Dict
+    variables: dict[str, str]
+    jobs: Dict
 
     def get_job(self, name: str) -> Job:
-        return Job(
-            name=name,
-            image=self.resolve_field(name, "image"),
-            before_script=self.resolve_field(name, "before_script"),
-            script=self.resolve_field(name, "script"),
-            variables=self.merge_fields(name, "variables"),
-            services=self.append_fields(name, "services"),
+        from .parser import merge_extends_and_defaults, parse_job
+
+        job = merge_extends_and_defaults(
+            name, self.jobs, self.default, self.globals, self.variables
         )
+        return parse_job(name, job)
+
+    def all_variable_names(self) -> set[str]:
+        return set(self.variables.keys()) | {
+            name for job in self.jobs.values() for name in job.get("variables", {})
+        }
```

### Comparing `trycicle-0.2.2/trycicle/run.py` & `trycicle-0.3.0/trycicle/run.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import typing
 from datetime import datetime
 
 from docker import DockerClient
 from docker.errors import ImageNotFound
 from docker.models.containers import Container
 
+from .cache import get_cache_path, pull_cache, push_cache
 from .models import Job, Service
 from .subprocess import run_command
 from .variables import Variables, get_all_variables
 
 logger = logging.getLogger(__name__)
 
 job_script_shebang = "#!/bin/sh\n"
@@ -72,14 +73,15 @@
 
 def run_job(
     job: Job,
     source_dir: str,
     original_dir: str,
     service_logs: bool = False,
     debugger: DebugEnabled = "false",
+    cache_directory: str = "",
 ) -> int:
     job_start = datetime.utcnow()
     docker = DockerClient.from_env()
 
     source_dir = os.path.abspath(source_dir)
     original_dir = os.path.abspath(original_dir)
     build_dir = tempfile.mkdtemp()
@@ -113,14 +115,21 @@
 
     if original_dir != source_dir:
         volumes[original_dir] = {"bind": "/repo", "mode": "ro"}
 
     if any(service.is_docker_dind for service in job.services):
         volumes.update(dind_volumes)
 
+    cache_paths = [
+        os.path.join(cache_directory, get_cache_path(cache, variables, original_dir))
+        for cache in job.cache
+    ]
+    for cache_path, cache in zip(cache_paths, job.cache):
+        pull_cache(cache, variables, cache_path, source_dir)
+
     job_image = variables.replace(job.image.name)
     logger.info(f"Starting job ({job_image})")
 
     interactive = debugger != "false"
     container = create_container(
         docker,
         image=job_image,
@@ -141,27 +150,34 @@
 
     if interactive:
         interactive_session(container)
     else:
         container.start()
         write_logs(container, b"job | " if service_logs else b"")
 
-    status = container.wait()
-
-    logger.debug(f"Job finished with exit code {status['StatusCode']}")
+    status_code = int(container.wait()["StatusCode"])
+    logger.debug(f"Job finished with exit code {status_code}")
 
     if service_containers:
         logger.debug(f"Stopping {len(service_containers)} service containers")
         stop_event_thread()
         for container in service_containers:
             container.stop()
 
+    for cache_path, cache in zip(cache_paths, job.cache):
+        if (
+            cache.when == "always"
+            or (cache.when == "on_success" and status_code == 0)
+            or (cache.when == "on_failure" and status_code != 0)
+        ):
+            push_cache(cache, variables, cache_path, source_dir)
+
     shutil.rmtree(build_dir)
     # TODO: Remove containers? (on success only?)
-    return int(status["StatusCode"])
+    return status_code
 
 
 def write_logs(container: Container, prefix: bytes = b"") -> None:
     """Write logs from a container to stdout, optionally prefixing every line.
 
     Because this function is called from multiple threads, it internally buffers the
     logs until a newline is found, to avoid mixing output from different containers.
```

### Comparing `trycicle-0.2.2/trycicle/subprocess.py` & `trycicle-0.3.0/trycicle/subprocess.py`

 * *Files identical despite different names*

### Comparing `trycicle-0.2.2/trycicle/variables.py` & `trycicle-0.3.0/trycicle/variables.py`

 * *Files identical despite different names*

### Comparing `trycicle-0.2.2/PKG-INFO` & `trycicle-0.3.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: trycicle
-Version: 0.2.2
-Summary: Try CI jobs locally
-Author-email: Paul Hooijenga <paul@founda.com>
-Requires-Python: ~= 3.11
-Description-Content-Type: text/markdown
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: POSIX
-Classifier: License :: OSI Approved :: MIT License
-Requires-Dist: pyyaml ~= 6.0
-Requires-Dist: docker ~= 7.0
-Requires-Dist: click ~= 8.1
-Project-URL: Homepage, https://gitlab.com/phooijenga/trycicle
-
 # Trycicle
 
 Try CI jobs locally, including services.
 
 ## Installation
 
     pipx install trycicle
@@ -291,14 +276,52 @@
 nothing to commit, working tree clean
 ```
 
 As you can see, only the committed changes are visible to the job.
 Trycicle adds your source directory as a remote to the clean copy, this makes it possible to use `git fetch` in the job.
 Pushing does not work, your working directory is mounted read-only.
 
+### Caching
+
+Trycicle has rudimentary support for caching. If a job defines a `cache` key, Trycicle will keep matching files between runs.
+
+```yaml
+image: busybox:latest
+
+cache:
+  key: example
+  paths:
+    - "*.txt"
+
+one:
+  script:
+    - echo 'Hello, world!' > hello.txt
+
+two:
+  script:
+    - cat hello.txt
+```
+
+Running the first job will create a cache with the `hello.txt` file:
+
+```console
+$ trycicle one
+INFO:trycicle.cache:Using cache 'cache-readme-example'
+...
+```
+
+The second job will be able to read the file from the cache:
+
+```console
+$ trycicle two
+INFO:trycicle.cache:Using cache 'cache-readme-example'
+...
+Hello, world!
+```
+
 ## Debugging
 
 ### Logs
 
 Trycicle does not immediately remove the containers it creates, so you can inspect them after the job has finished.
 The containers are labeled with the job they were part of, so you can use a command like `docker ps -a --filter label=trycicle.job=test` to list them.
 This can also be combined with `docker logs`, for example to get the logs of `postgresql` service in the most recent run:
@@ -319,8 +342,7 @@
 ### Interactive debugging
 
 Trycicle can run a job in interactive mode, which means you can execute commands in the container after the job has finished.
 This is useful to inspect the state of the container, check environment variables, or find out what that missing package is called.
 
 The debug shell will start automatically when the job fails, you can also add a `debugger` command to the script to start it manually.
 To enter the debug shell before the job starts, use the `--debug=immediate` option.
-
```

