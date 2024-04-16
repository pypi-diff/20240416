# Comparing `tmp/mozregression-6.0.2.tar.gz` & `tmp/mozregression-6.1.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mozregression-6.0.2.tar", last modified: Mon Jan 15 13:36:07 2024, max compression
+gzip compressed data, was "mozregression-6.1.0.dev0.tar", last modified: Tue Apr 16 15:46:16 2024, max compression
```

## Comparing `mozregression-6.0.2.tar` & `mozregression-6.1.0.dev0.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 13:36:07.569354 mozregression-6.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-01-15 13:35:21.000000 mozregression-6.0.2/.coveralls.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 13:36:07.561354 mozregression-6.0.2/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-01-15 13:35:21.000000 mozregression-6.0.2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 13:36:07.561354 mozregression-6.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     5852 2024-01-15 13:35:21.000000 mozregression-6.0.2/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3044 2024-01-15 13:35:21.000000 mozregression-6.0.2/.github/workflows/compile-requirements.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4597 2024-01-15 13:35:21.000000 mozregression-6.0.2/.github/workflows/deploy-gui.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-01-15 13:35:21.000000 mozregression-6.0.2/.github/workflows/deploy.yml
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-01-15 13:35:21.000000 mozregression-6.0.2/.github/workflows/glean-probe-scraper.yml
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-01-15 13:35:21.000000 mozregression-6.0.2/.github/workflows/run-compile-requirements.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3911 2024-01-15 13:35:21.000000 mozregression-6.0.2/.github/workflows/upload-gui-to-workflow.yml
--rw-r--r--   0 runner    (1001) docker     (127)    16726 2024-01-15 13:35:21.000000 mozregression-6.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-01-15 13:35:21.000000 mozregression-6.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-01-15 13:36:07.569354 mozregression-6.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4934 2024-01-15 13:35:21.000000 mozregression-6.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 13:36:07.569354 mozregression-6.0.2/mozregression/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-01-15 13:35:21.000000 mozregression-6.0.2/mozregression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-01-15 13:35:21.000000 mozregression-6.0.2/mozregression/approx_persist.py
--rw-r--r--   0 runner    (1001) docker     (127)    25458 2024-01-15 13:35:21.000000 mozregression-6.0.2/mozregression/bisector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3540 2024-01-15 13:35:21.000000 mozregression-6.0.2/mozregression/branches.py
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-01-15 13:35:21.000000 mozregression-6.0.2/mozregression/bugzilla.py
--rw-r--r--   0 runner    (1001) docker     (127)     6029 2024-01-15 13:35:21.000000 mozregression-6.0.2/mozregression/build_info.py
--rw-r--r--   0 runner    (1001) docker     (127)    11266 2024-01-15 13:35:21.000000 mozregression-6.0.2/mozregression/build_range.py
--rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-01-15 13:35:21.000000 mozregression-6.0.2/mozregression/class_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)    24473 2024-01-15 13:35:21.000000 mozregression-6.0.2/mozregression/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     5002 2024-01-15 13:35:21.000000 mozregression-6.0.2/mozregression/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-01-15 13:35:21.000000 mozregression-6.0.2/mozregression/dates.py
--rw-r--r--   0 runner    (1001) docker     (127)    14034 2024-01-15 13:35:21.000000 mozregression-6.0.2/mozregression/download_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-01-15 13:35:21.000000 mozregression-6.0.2/mozregression/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    11133 2024-01-15 13:35:21.000000 mozregression-6.0.2/mozregression/fetch_build_info.py
--rw-r--r--   0 runner    (1001) docker     (127)    23823 2024-01-15 13:35:21.000000 mozregression-6.0.2/mozregression/fetch_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-01-15 13:35:21.000000 mozregression-6.0.2/mozregression/history.py
--rw-r--r--   0 runner    (1001) docker     (127)     4732 2024-01-15 13:35:21.000000 mozregression-6.0.2/mozregression/json_pushes.py
--rw-r--r--   0 runner    (1001) docker     (127)    20699 2024-01-15 13:35:21.000000 mozregression-6.0.2/mozregression/launchers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3378 2024-01-15 13:35:21.000000 mozregression-6.0.2/mozregression/log.py
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-01-15 13:35:21.000000 mozregression-6.0.2/mozregression/mach_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)    14567 2024-01-15 13:35:21.000000 mozregression-6.0.2/mozregression/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     3801 2024-01-15 13:35:21.000000 mozregression-6.0.2/mozregression/metrics.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2483 2024-01-15 13:35:21.000000 mozregression-6.0.2/mozregression/network.py
--rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-01-15 13:35:21.000000 mozregression-6.0.2/mozregression/persist_limit.py
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-01-15 13:35:21.000000 mozregression-6.0.2/mozregression/pings.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3652 2024-01-15 13:35:21.000000 mozregression-6.0.2/mozregression/pyinstaller.py
--rw-r--r--   0 runner    (1001) docker     (127)     4023 2024-01-15 13:35:21.000000 mozregression-6.0.2/mozregression/releases.py
--rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-01-15 13:35:21.000000 mozregression-6.0.2/mozregression/tc_authenticate.py
--rw-r--r--   0 runner    (1001) docker     (127)     4312 2024-01-15 13:35:21.000000 mozregression-6.0.2/mozregression/telemetry.py
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-01-15 13:35:21.000000 mozregression-6.0.2/mozregression/tempdir.py
--rw-r--r--   0 runner    (1001) docker     (127)     8346 2024-01-15 13:35:21.000000 mozregression-6.0.2/mozregression/test_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-01-15 13:36:07.000000 mozregression-6.0.2/mozregression/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 13:36:07.569354 mozregression-6.0.2/mozregression.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-01-15 13:36:07.000000 mozregression-6.0.2/mozregression.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-01-15 13:36:07.000000 mozregression-6.0.2/mozregression.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-15 13:36:07.000000 mozregression-6.0.2/mozregression.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-01-15 13:36:07.000000 mozregression-6.0.2/mozregression.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-01-15 13:36:07.000000 mozregression-6.0.2/mozregression.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-01-15 13:36:07.000000 mozregression-6.0.2/mozregression.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-01-15 13:35:21.000000 mozregression-6.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-15 13:36:07.569354 mozregression-6.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-01-15 13:35:21.000000 mozregression-6.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:46:15.996225 mozregression-6.1.0.dev0/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-16 15:45:30.000000 mozregression-6.1.0.dev0/.coveralls.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:46:15.988225 mozregression-6.1.0.dev0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-16 15:45:30.000000 mozregression-6.1.0.dev0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:46:15.988225 mozregression-6.1.0.dev0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     5852 2024-04-16 15:45:30.000000 mozregression-6.1.0.dev0/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3143 2024-04-16 15:45:30.000000 mozregression-6.1.0.dev0/.github/workflows/compile-requirements.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4707 2024-04-16 15:45:30.000000 mozregression-6.1.0.dev0/.github/workflows/deploy-gui.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-04-16 15:45:30.000000 mozregression-6.1.0.dev0/.github/workflows/deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-16 15:45:30.000000 mozregression-6.1.0.dev0/.github/workflows/glean-probe-scraper.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-16 15:45:30.000000 mozregression-6.1.0.dev0/.github/workflows/run-compile-requirements.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3911 2024-04-16 15:45:30.000000 mozregression-6.1.0.dev0/.github/workflows/upload-gui-to-workflow.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    16726 2024-04-16 15:45:30.000000 mozregression-6.1.0.dev0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-16 15:45:30.000000 mozregression-6.1.0.dev0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-04-16 15:46:15.996225 mozregression-6.1.0.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4934 2024-04-16 15:45:30.000000 mozregression-6.1.0.dev0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:46:15.996225 mozregression-6.1.0.dev0/mozregression/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-16 15:45:30.000000 mozregression-6.1.0.dev0/mozregression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-04-16 15:45:30.000000 mozregression-6.1.0.dev0/mozregression/approx_persist.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25458 2024-04-16 15:45:30.000000 mozregression-6.1.0.dev0/mozregression/bisector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3540 2024-04-16 15:45:30.000000 mozregression-6.1.0.dev0/mozregression/branches.py
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-16 15:45:30.000000 mozregression-6.1.0.dev0/mozregression/bugzilla.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6030 2024-04-16 15:45:30.000000 mozregression-6.1.0.dev0/mozregression/build_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11266 2024-04-16 15:45:30.000000 mozregression-6.1.0.dev0/mozregression/build_range.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-04-16 15:45:30.000000 mozregression-6.1.0.dev0/mozregression/class_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24473 2024-04-16 15:45:30.000000 mozregression-6.1.0.dev0/mozregression/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5019 2024-04-16 15:45:30.000000 mozregression-6.1.0.dev0/mozregression/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-04-16 15:45:30.000000 mozregression-6.1.0.dev0/mozregression/dates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14034 2024-04-16 15:45:30.000000 mozregression-6.1.0.dev0/mozregression/download_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-04-16 15:45:30.000000 mozregression-6.1.0.dev0/mozregression/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11133 2024-04-16 15:45:30.000000 mozregression-6.1.0.dev0/mozregression/fetch_build_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23824 2024-04-16 15:45:30.000000 mozregression-6.1.0.dev0/mozregression/fetch_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-16 15:45:30.000000 mozregression-6.1.0.dev0/mozregression/history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4732 2024-04-16 15:45:30.000000 mozregression-6.1.0.dev0/mozregression/json_pushes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20699 2024-04-16 15:45:30.000000 mozregression-6.1.0.dev0/mozregression/launchers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3378 2024-04-16 15:45:30.000000 mozregression-6.1.0.dev0/mozregression/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-16 15:45:30.000000 mozregression-6.1.0.dev0/mozregression/mach_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14567 2024-04-16 15:45:30.000000 mozregression-6.1.0.dev0/mozregression/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3801 2024-04-16 15:45:30.000000 mozregression-6.1.0.dev0/mozregression/metrics.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2483 2024-04-16 15:45:30.000000 mozregression-6.1.0.dev0/mozregression/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-04-16 15:45:30.000000 mozregression-6.1.0.dev0/mozregression/persist_limit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-04-16 15:45:30.000000 mozregression-6.1.0.dev0/mozregression/pings.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3652 2024-04-16 15:45:30.000000 mozregression-6.1.0.dev0/mozregression/pyinstaller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4023 2024-04-16 15:45:30.000000 mozregression-6.1.0.dev0/mozregression/releases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-04-16 15:45:30.000000 mozregression-6.1.0.dev0/mozregression/tc_authenticate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4312 2024-04-16 15:45:30.000000 mozregression-6.1.0.dev0/mozregression/telemetry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-16 15:45:30.000000 mozregression-6.1.0.dev0/mozregression/tempdir.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8346 2024-04-16 15:45:30.000000 mozregression-6.1.0.dev0/mozregression/test_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-16 15:46:15.000000 mozregression-6.1.0.dev0/mozregression/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:46:15.996225 mozregression-6.1.0.dev0/mozregression.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-04-16 15:46:15.000000 mozregression-6.1.0.dev0/mozregression.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-04-16 15:46:15.000000 mozregression-6.1.0.dev0/mozregression.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 15:46:15.000000 mozregression-6.1.0.dev0/mozregression.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-16 15:46:15.000000 mozregression-6.1.0.dev0/mozregression.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-16 15:46:15.000000 mozregression-6.1.0.dev0/mozregression.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-16 15:46:15.000000 mozregression-6.1.0.dev0/mozregression.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-16 15:45:30.000000 mozregression-6.1.0.dev0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 15:46:15.996225 mozregression-6.1.0.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-04-16 15:45:30.000000 mozregression-6.1.0.dev0/setup.py
```

### Comparing `mozregression-6.0.2/.github/workflows/build.yml` & `mozregression-6.1.0.dev0/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `mozregression-6.0.2/.github/workflows/compile-requirements.yml` & `mozregression-6.1.0.dev0/.github/workflows/compile-requirements.yml`

 * *Files 4% similar despite different names*

```diff
@@ -19,17 +19,21 @@
         required: false
         type: string
       requirements_files:
         default: '["requirements.in"]'
         description: A string representation of a list of requirement files.
         required: false
         type: string
+      commit_and_push:
+        type: string
+        default: 'false'
 
 jobs:
   compile-requirements:
+    if: ${{ inputs.commit_and_push != 'true' }}
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
         os: ${{ fromJSON(inputs.os) }}
         python-version: ${{ fromJSON(inputs.python) }}
         requirements_file: ${{ fromJSON(inputs.requirements_files) }}
     steps:
@@ -52,15 +56,15 @@
         env:
           GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
       - uses: actions/upload-artifact@v2
         with:
           name: ${{ github.sha }}-${{ github.run_number }}-${{ github.run_attempt }}-requirements
           path: requirements/requirements-${{ matrix.python-version }}-${{ runner.os }}.txt
   commit-and-push:
-    needs: compile-requirements
+    if: ${{ inputs.commit_and_push == 'true' }}
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v3
         with:
           persist-credentials: false
       - uses: actions/download-artifact@v3
         with:
@@ -75,8 +79,8 @@
           GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
         run: |
           git status
           git pull --rebase
           find temp-requirements -name "requirements-*" -type f -exec mv -f -t requirements {} +
           git add -A
           git commit -m "Automatically generated requirements"
-          until git push -f https://x-access-token:${GITHUB_TOKEN}@github.com/${GITHUB_REPOSITORY}.git; do git pull --rebase; done
+          git push -f https://x-access-token:${GITHUB_TOKEN}@github.com/${GITHUB_REPOSITORY}.git
```

### Comparing `mozregression-6.0.2/.github/workflows/deploy-gui.yml` & `mozregression-6.1.0.dev0/.github/workflows/deploy-gui.yml`

 * *Files 2% similar despite different names*

```diff
@@ -122,7 +122,9 @@
           upload_url: ${{ github.event.release.upload_url }}
           asset_path: ./gui/wininst/mozregression-gui.exe
           asset_name: mozregression-gui-unsigned.exe
           asset_content_type: application/octet-stream
       - name: Print signing manifest
         run: |
           python ./bin/adhoc-sign.py --os windows ${{ github.event.release.tag_name }}
+      - name: Test binary for viruses
+        run: ./bin/virustotal-scan.py ${{ secrets.VIRUSTOTAL_API_KEY }}
```

### Comparing `mozregression-6.0.2/.github/workflows/deploy.yml` & `mozregression-6.1.0.dev0/.github/workflows/deploy.yml`

 * *Files identical despite different names*

### Comparing `mozregression-6.0.2/.github/workflows/run-compile-requirements.yml` & `mozregression-6.1.0.dev0/.github/workflows/run-compile-requirements.yml`

 * *Files 6% similar despite different names*

```diff
@@ -24,7 +24,16 @@
 
   call-compile-requirements-macos:
     uses: ./.github/workflows/compile-requirements.yml
     with:
       requirements_files: '["base.in base.universal2.in dev.in gui-dev.in gui.in linters.in"]'
       os: '["macos-latest"]'
       python: '["3.9", "3.10", "3.11"]'
+
+  commit-and-push:
+    uses: ./.github/workflows/compile-requirements.yml
+    with:
+      commit_and_push: 'true'
+    needs:
+      - call-compile-requirements-macos
+      - call-compile-requirements-windows
+      - call-compile-requirements-linux
```

### Comparing `mozregression-6.0.2/.github/workflows/upload-gui-to-workflow.yml` & `mozregression-6.1.0.dev0/.github/workflows/upload-gui-to-workflow.yml`

 * *Files identical despite different names*

### Comparing `mozregression-6.0.2/LICENSE` & `mozregression-6.1.0.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `mozregression-6.0.2/PKG-INFO` & `mozregression-6.1.0.dev0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mozregression
-Version: 6.0.2
+Version: 6.1.0.dev0
 Summary: Regression range finder for Mozilla nightly builds
 Home-page: http://github.com/mozilla/mozregression
 Author: Mozilla Automation and Tools Team
 Author-email: tools@lists.mozilla.org
 License: MPL 2.0
 Platform: Any
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
```

### Comparing `mozregression-6.0.2/README.md` & `mozregression-6.1.0.dev0/README.md`

 * *Files identical despite different names*

### Comparing `mozregression-6.0.2/mozregression/approx_persist.py` & `mozregression-6.1.0.dev0/mozregression/approx_persist.py`

 * *Files identical despite different names*

### Comparing `mozregression-6.0.2/mozregression/bisector.py` & `mozregression-6.1.0.dev0/mozregression/bisector.py`

 * *Files identical despite different names*

### Comparing `mozregression-6.0.2/mozregression/branches.py` & `mozregression-6.1.0.dev0/mozregression/branches.py`

 * *Files identical despite different names*

### Comparing `mozregression-6.0.2/mozregression/bugzilla.py` & `mozregression-6.1.0.dev0/mozregression/bugzilla.py`

 * *Files identical despite different names*

### Comparing `mozregression-6.0.2/mozregression/build_info.py` & `mozregression-6.1.0.dev0/mozregression/build_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 The BuildInfo classes, that are used to store information a build.
 """
+
 from __future__ import absolute_import
 
 import datetime
 import re
 from urllib.parse import urlparse
 
 FIELDS = []
```

### Comparing `mozregression-6.0.2/mozregression/build_range.py` & `mozregression-6.1.0.dev0/mozregression/build_range.py`

 * *Files identical despite different names*

### Comparing `mozregression-6.0.2/mozregression/class_registry.py` & `mozregression-6.1.0.dev0/mozregression/class_registry.py`

 * *Files identical despite different names*

### Comparing `mozregression-6.0.2/mozregression/cli.py` & `mozregression-6.1.0.dev0/mozregression/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -497,16 +497,16 @@
         self.logger = init_logger(debug=options.debug)
         # allow to filter process output based on the user option
         if options.process_output is None:
             # process_output not user defined
             log_process_output = options.build_type != ""
         else:
             log_process_output = options.process_output == "stdout"
-        get_default_logger("process").component_filter = (
-            lambda data: data if log_process_output else None
+        get_default_logger("process").component_filter = lambda data: (
+            data if log_process_output else None
         )
 
         # filter some mozversion log lines
         re_ignore_mozversion_line = re.compile(
             r"^(platform_.+|application_vendor|application_remotingname"
             r"|application_id|application_display_name): .+"
         )
```

### Comparing `mozregression-6.0.2/mozregression/config.py` & `mozregression-6.1.0.dev0/mozregression/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,15 +133,15 @@
 
 
 def write_config(conf_path):
     conf_dir = os.path.dirname(conf_path)
     if not os.path.isdir(conf_dir):
         os.makedirs(conf_dir)
 
-    config = ConfigObj(conf_path)
+    config = ConfigObj(conf_path, encoding="UTF8")
     if not config.initial_comment:
         config.initial_comment = CONF_HELP.splitlines()
 
     def _set_option(optname, getfunc, default):
         print()
         if optname not in config:
             value = getfunc(default)
```

### Comparing `mozregression-6.0.2/mozregression/dates.py` & `mozregression-6.1.0.dev0/mozregression/dates.py`

 * *Files identical despite different names*

### Comparing `mozregression-6.0.2/mozregression/download_manager.py` & `mozregression-6.1.0.dev0/mozregression/download_manager.py`

 * *Files identical despite different names*

### Comparing `mozregression-6.0.2/mozregression/errors.py` & `mozregression-6.1.0.dev0/mozregression/errors.py`

 * *Files identical despite different names*

### Comparing `mozregression-6.0.2/mozregression/fetch_build_info.py` & `mozregression-6.1.0.dev0/mozregression/fetch_build_info.py`

 * *Files identical despite different names*

### Comparing `mozregression-6.0.2/mozregression/fetch_configs.py` & `mozregression-6.1.0.dev0/mozregression/fetch_configs.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 
 You can also use the variable *REGISTRY* defined in this module to get a
 list of application names that can be used to build a configuration. This is
 an instance of :class:`ClassRegistry`. Example: ::
 
   print REGISTRY.names()
 """
+
 from __future__ import absolute_import
 
 import datetime
 import re
 from abc import ABCMeta, abstractmethod
 
 from mozlog import get_proxy_logger
```

### Comparing `mozregression-6.0.2/mozregression/history.py` & `mozregression-6.1.0.dev0/mozregression/history.py`

 * *Files identical despite different names*

### Comparing `mozregression-6.0.2/mozregression/json_pushes.py` & `mozregression-6.1.0.dev0/mozregression/json_pushes.py`

 * *Files identical despite different names*

### Comparing `mozregression-6.0.2/mozregression/launchers.py` & `mozregression-6.1.0.dev0/mozregression/launchers.py`

 * *Files identical despite different names*

### Comparing `mozregression-6.0.2/mozregression/log.py` & `mozregression-6.1.0.dev0/mozregression/log.py`

 * *Files identical despite different names*

### Comparing `mozregression-6.0.2/mozregression/mach_interface.py` & `mozregression-6.1.0.dev0/mozregression/mach_interface.py`

 * *Files identical despite different names*

### Comparing `mozregression-6.0.2/mozregression/main.py` & `mozregression-6.1.0.dev0/mozregression/main.py`

 * *Files identical despite different names*

### Comparing `mozregression-6.0.2/mozregression/metrics.yaml` & `mozregression-6.1.0.dev0/mozregression/metrics.yaml`

 * *Files identical despite different names*

### Comparing `mozregression-6.0.2/mozregression/network.py` & `mozregression-6.1.0.dev0/mozregression/network.py`

 * *Files identical despite different names*

### Comparing `mozregression-6.0.2/mozregression/persist_limit.py` & `mozregression-6.1.0.dev0/mozregression/persist_limit.py`

 * *Files identical despite different names*

### Comparing `mozregression-6.0.2/mozregression/pings.yaml` & `mozregression-6.1.0.dev0/mozregression/pings.yaml`

 * *Files identical despite different names*

### Comparing `mozregression-6.0.2/mozregression/pyinstaller.py` & `mozregression-6.1.0.dev0/mozregression/pyinstaller.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """PyInstaller helper module to enable packaging tcl/tk with app bundles."""
 
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at https://mozilla.org/MPL/2.0/.
 
+import _tkinter
 import shutil
 import subprocess
 from pathlib import Path
 
-import _tkinter
 import PyInstaller.log as logging
 from PyInstaller.building.datastruct import Tree
 from PyInstaller.building.osx import BUNDLE
 from PyInstaller.compat import is_darwin
 from PyInstaller.utils.hooks.tcl_tk import (
     _collect_tcl_modules,
     _find_tcl_tk,
```

### Comparing `mozregression-6.0.2/mozregression/releases.py` & `mozregression-6.1.0.dev0/mozregression/releases.py`

 * *Files identical despite different names*

### Comparing `mozregression-6.0.2/mozregression/tc_authenticate.py` & `mozregression-6.1.0.dev0/mozregression/tc_authenticate.py`

 * *Files identical despite different names*

### Comparing `mozregression-6.0.2/mozregression/telemetry.py` & `mozregression-6.1.0.dev0/mozregression/telemetry.py`

 * *Files identical despite different names*

### Comparing `mozregression-6.0.2/mozregression/tempdir.py` & `mozregression-6.1.0.dev0/mozregression/tempdir.py`

 * *Files identical despite different names*

### Comparing `mozregression-6.0.2/mozregression/test_runner.py` & `mozregression-6.1.0.dev0/mozregression/test_runner.py`

 * *Files identical despite different names*

### Comparing `mozregression-6.0.2/mozregression.egg-info/PKG-INFO` & `mozregression-6.1.0.dev0/mozregression.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mozregression
-Version: 6.0.2
+Version: 6.1.0.dev0
 Summary: Regression range finder for Mozilla nightly builds
 Home-page: http://github.com/mozilla/mozregression
 Author: Mozilla Automation and Tools Team
 Author-email: tools@lists.mozilla.org
 License: MPL 2.0
 Platform: Any
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
```

### Comparing `mozregression-6.0.2/mozregression.egg-info/SOURCES.txt` & `mozregression-6.1.0.dev0/mozregression.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mozregression-6.0.2/pyproject.toml` & `mozregression-6.1.0.dev0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mozregression-6.0.2/setup.py` & `mozregression-6.1.0.dev0/setup.py`

 * *Files identical despite different names*

