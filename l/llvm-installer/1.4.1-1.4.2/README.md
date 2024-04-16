# Comparing `tmp/llvm-installer-1.4.1.tar.gz` & `tmp/llvm_installer-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llvm-installer-1.4.1.tar", last modified: Tue Feb 20 07:31:41 2024, max compression
+gzip compressed data, was "llvm_installer-1.4.2.tar", last modified: Tue Apr 16 00:32:37 2024, max compression
```

## Comparing `llvm-installer-1.4.1.tar` & `llvm_installer-1.4.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 mikhail    (503) staff       (20)        0 2024-02-20 07:31:41.020419 llvm-installer-1.4.1/
--rw-r--r--   0 mikhail    (503) staff       (20)    11358 2022-05-26 15:06:09.000000 llvm-installer-1.4.1/LICENSE
--rw-r--r--   0 mikhail    (503) staff       (20)      989 2024-02-20 07:31:41.020272 llvm-installer-1.4.1/PKG-INFO
--rw-r--r--   0 mikhail    (503) staff       (20)      643 2022-07-07 03:18:16.000000 llvm-installer-1.4.1/README.md
--rw-r--r--   0 mikhail    (503) staff       (20)       38 2024-02-20 07:31:41.020467 llvm-installer-1.4.1/setup.cfg
--rw-r--r--   0 mikhail    (503) staff       (20)     2235 2024-02-20 06:52:36.000000 llvm-installer-1.4.1/setup.py
-drwxr-xr-x   0 mikhail    (503) staff       (20)        0 2024-02-20 07:31:41.016709 llvm-installer-1.4.1/src/
-drwxr-xr-x   0 mikhail    (503) staff       (20)        0 2024-02-20 07:31:41.018514 llvm-installer-1.4.1/src/llvm_installer/
--rw-r--r--   0 mikhail    (503) staff       (20)    11455 2022-08-17 05:24:37.000000 llvm-installer-1.4.1/src/llvm_installer/__init__.py
--rw-r--r--   0 mikhail    (503) staff       (20)     5477 2023-08-24 20:40:18.000000 llvm-installer-1.4.1/src/llvm_installer/__main__.py
--rw-r--r--   0 mikhail    (503) staff       (20)        0 2022-05-26 15:06:09.000000 llvm-installer-1.4.1/src/llvm_installer/py.typed
--rw-r--r--   0 mikhail    (503) staff       (20)   138865 2024-02-20 06:45:24.000000 llvm-installer-1.4.1/src/llvm_installer/release_tags.json
-drwxr-xr-x   0 mikhail    (503) staff       (20)        0 2024-02-20 07:31:41.020043 llvm-installer-1.4.1/src/llvm_installer.egg-info/
--rw-r--r--   0 mikhail    (503) staff       (20)      989 2024-02-20 07:31:40.000000 llvm-installer-1.4.1/src/llvm_installer.egg-info/PKG-INFO
--rw-r--r--   0 mikhail    (503) staff       (20)      407 2024-02-20 07:31:41.000000 llvm-installer-1.4.1/src/llvm_installer.egg-info/SOURCES.txt
--rw-r--r--   0 mikhail    (503) staff       (20)        1 2024-02-20 07:31:40.000000 llvm-installer-1.4.1/src/llvm_installer.egg-info/dependency_links.txt
--rw-r--r--   0 mikhail    (503) staff       (20)       64 2024-02-20 07:31:40.000000 llvm-installer-1.4.1/src/llvm_installer.egg-info/entry_points.txt
--rw-r--r--   0 mikhail    (503) staff       (20)       86 2024-02-20 07:31:40.000000 llvm-installer-1.4.1/src/llvm_installer.egg-info/requires.txt
--rw-r--r--   0 mikhail    (503) staff       (20)       15 2024-02-20 07:31:40.000000 llvm-installer-1.4.1/src/llvm_installer.egg-info/top_level.txt
+drwxr-xr-x   0 mikhail    (503) staff       (20)        0 2024-04-16 00:32:37.843134 llvm_installer-1.4.2/
+-rw-r--r--   0 mikhail    (503) staff       (20)    11358 2022-05-26 15:06:09.000000 llvm_installer-1.4.2/LICENSE
+-rw-r--r--   0 mikhail    (503) staff       (20)     1268 2024-04-16 00:32:37.842871 llvm_installer-1.4.2/PKG-INFO
+-rw-r--r--   0 mikhail    (503) staff       (20)      643 2022-07-07 03:18:16.000000 llvm_installer-1.4.2/README.md
+-rw-r--r--   0 mikhail    (503) staff       (20)       38 2024-04-16 00:32:37.843196 llvm_installer-1.4.2/setup.cfg
+-rw-r--r--   0 mikhail    (503) staff       (20)     2235 2024-04-16 00:23:06.000000 llvm_installer-1.4.2/setup.py
+drwxr-xr-x   0 mikhail    (503) staff       (20)        0 2024-04-16 00:32:37.839516 llvm_installer-1.4.2/src/
+drwxr-xr-x   0 mikhail    (503) staff       (20)        0 2024-04-16 00:32:37.840700 llvm_installer-1.4.2/src/llvm_installer/
+-rw-r--r--   0 mikhail    (503) staff       (20)    11455 2022-08-17 05:24:37.000000 llvm_installer-1.4.2/src/llvm_installer/__init__.py
+-rw-r--r--   0 mikhail    (503) staff       (20)     5477 2023-08-24 20:40:18.000000 llvm_installer-1.4.2/src/llvm_installer/__main__.py
+-rw-r--r--   0 mikhail    (503) staff       (20)        0 2022-05-26 15:06:09.000000 llvm_installer-1.4.2/src/llvm_installer/py.typed
+-rw-r--r--   0 mikhail    (503) staff       (20)   144169 2024-04-16 00:19:40.000000 llvm_installer-1.4.2/src/llvm_installer/release_tags.json
+drwxr-xr-x   0 mikhail    (503) staff       (20)        0 2024-04-16 00:32:37.842227 llvm_installer-1.4.2/src/llvm_installer.egg-info/
+-rw-r--r--   0 mikhail    (503) staff       (20)     1268 2024-04-16 00:32:37.000000 llvm_installer-1.4.2/src/llvm_installer.egg-info/PKG-INFO
+-rw-r--r--   0 mikhail    (503) staff       (20)      407 2024-04-16 00:32:37.000000 llvm_installer-1.4.2/src/llvm_installer.egg-info/SOURCES.txt
+-rw-r--r--   0 mikhail    (503) staff       (20)        1 2024-04-16 00:32:37.000000 llvm_installer-1.4.2/src/llvm_installer.egg-info/dependency_links.txt
+-rw-r--r--   0 mikhail    (503) staff       (20)       64 2024-04-16 00:32:37.000000 llvm_installer-1.4.2/src/llvm_installer.egg-info/entry_points.txt
+-rw-r--r--   0 mikhail    (503) staff       (20)       86 2024-04-16 00:32:37.000000 llvm_installer-1.4.2/src/llvm_installer.egg-info/requires.txt
+-rw-r--r--   0 mikhail    (503) staff       (20)       15 2024-04-16 00:32:37.000000 llvm_installer-1.4.2/src/llvm_installer.egg-info/top_level.txt
```

### Comparing `llvm-installer-1.4.1/LICENSE` & `llvm_installer-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `llvm-installer-1.4.1/README.md` & `llvm_installer-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `llvm-installer-1.4.1/setup.py` & `llvm_installer-1.4.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     from os import path
     this_directory = path.abspath(path.dirname(__file__))
     with open(path.join(this_directory, 'README.md'), encoding='utf-8') as readme_file:
         long_description = readme_file.read()
 
     setup(
         name='llvm-installer',
-        version='1.4.1',
+        version='1.4.2',
         url='https://github.com/yugabyte/llvm-installer',
         author='Mikhail Bautin',
         author_email='mbautin@users.noreply.github.com',
         description='Allows installing pre-built LLVM packages for various operating systems',
         packages=find_packages(where='src'),
         package_dir={"": "src"},
         package_data={'llvm_installer': ['py.typed', 'release_tags.json']},
```

### Comparing `llvm-installer-1.4.1/src/llvm_installer/__init__.py` & `llvm_installer-1.4.2/src/llvm_installer/__init__.py`

 * *Files identical despite different names*

### Comparing `llvm-installer-1.4.1/src/llvm_installer/__main__.py` & `llvm_installer-1.4.2/src/llvm_installer/__main__.py`

 * *Files identical despite different names*

### Comparing `llvm-installer-1.4.1/src/llvm_installer/release_tags.json` & `llvm_installer-1.4.2/src/llvm_installer/release_tags.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9817073170731707%*

 * *Differences: {"'parsed_tags'": "{insert: [(255, OrderedDict([('architecture', 'x86_64'), "*

 * *                  "('is_old_tag_without_os_and_arch', False), ('major_version', 17), "*

 * *                  "('minor_version', 0), ('patch_version', 6), ('sha1_prefix', '9b881774'), "*

 * *                  "('short_os_name_and_version', 'almalinux8'), ('tag', "*

 * *                  "'v17.0.6-yb-1-1711506617-9b881774-almalinux8-x86_64'), ('timestamp', "*

 * *                  "'1711506617'), ('version', '17.0.6'), ('version_suffix', 'yb-1'), "*

 * *   […]*

```diff
@@ -3567,14 +3567,28 @@
             "tag": "v17.0.6-yb-1-1702605315-9b881774-almalinux8-x86_64",
             "timestamp": "1702605315",
             "version": "17.0.6",
             "version_suffix": "yb-1",
             "yb_suffix_version": 1
         },
         {
+            "architecture": "x86_64",
+            "is_old_tag_without_os_and_arch": false,
+            "major_version": 17,
+            "minor_version": 0,
+            "patch_version": 6,
+            "sha1_prefix": "9b881774",
+            "short_os_name_and_version": "almalinux8",
+            "tag": "v17.0.6-yb-1-1711506617-9b881774-almalinux8-x86_64",
+            "timestamp": "1711506617",
+            "version": "17.0.6",
+            "version_suffix": "yb-1",
+            "yb_suffix_version": 1
+        },
+        {
             "architecture": "aarch64",
             "is_old_tag_without_os_and_arch": false,
             "major_version": 17,
             "minor_version": 0,
             "patch_version": 0,
             "sha1_prefix": "ff047e99",
             "short_os_name_and_version": "almalinux9",
@@ -3763,14 +3777,28 @@
             "tag": "v17.0.6-yb-1-1702608813-9b881774-almalinux9-x86_64",
             "timestamp": "1702608813",
             "version": "17.0.6",
             "version_suffix": "yb-1",
             "yb_suffix_version": 1
         },
         {
+            "architecture": "x86_64",
+            "is_old_tag_without_os_and_arch": false,
+            "major_version": 17,
+            "minor_version": 0,
+            "patch_version": 6,
+            "sha1_prefix": "9b881774",
+            "short_os_name_and_version": "almalinux9",
+            "tag": "v17.0.6-yb-1-1711511073-9b881774-almalinux9-x86_64",
+            "timestamp": "1711511073",
+            "version": "17.0.6",
+            "version_suffix": "yb-1",
+            "yb_suffix_version": 1
+        },
+        {
             "architecture": "aarch64",
             "is_old_tag_without_os_and_arch": false,
             "major_version": 17,
             "minor_version": 0,
             "patch_version": 0,
             "sha1_prefix": "ff047e99",
             "short_os_name_and_version": "centos7",
@@ -4257,14 +4285,28 @@
             "yb_suffix_version": 1
         },
         {
             "architecture": "x86_64",
             "is_old_tag_without_os_and_arch": false,
             "major_version": 17,
             "minor_version": 0,
+            "patch_version": 6,
+            "sha1_prefix": "9b881774",
+            "short_os_name_and_version": "ubuntu22.04",
+            "tag": "v17.0.6-yb-1-1711515605-9b881774-ubuntu22.04-x86_64",
+            "timestamp": "1711515605",
+            "version": "17.0.6",
+            "version_suffix": "yb-1",
+            "yb_suffix_version": 1
+        },
+        {
+            "architecture": "x86_64",
+            "is_old_tag_without_os_and_arch": false,
+            "major_version": 17,
+            "minor_version": 0,
             "patch_version": 0,
             "sha1_prefix": "f4941784",
             "short_os_name_and_version": "ubuntu23.04",
             "tag": "v17.0.0-rc4-yb-1-1695194174-f4941784-ubuntu23.04-x86_64",
             "timestamp": "1695194174",
             "version": "17.0.0",
             "version_suffix": "rc4-yb-1",
@@ -4339,14 +4381,42 @@
             "version": "17.0.6",
             "version_suffix": "yb-1",
             "yb_suffix_version": 1
         },
         {
             "architecture": "x86_64",
             "is_old_tag_without_os_and_arch": false,
+            "major_version": 17,
+            "minor_version": 0,
+            "patch_version": 6,
+            "sha1_prefix": "9b881774",
+            "short_os_name_and_version": "ubuntu23.04",
+            "tag": "v17.0.6-yb-1-1711520045-9b881774-ubuntu23.04-x86_64",
+            "timestamp": "1711520045",
+            "version": "17.0.6",
+            "version_suffix": "yb-1",
+            "yb_suffix_version": 1
+        },
+        {
+            "architecture": "aarch64",
+            "is_old_tag_without_os_and_arch": false,
+            "major_version": 18,
+            "minor_version": 1,
+            "patch_version": 2,
+            "sha1_prefix": "53fdd023",
+            "short_os_name_and_version": "almalinux8",
+            "tag": "v18.1.2-yb-1-1711588306-53fdd023-almalinux8-aarch64",
+            "timestamp": "1711588306",
+            "version": "18.1.2",
+            "version_suffix": "yb-1",
+            "yb_suffix_version": 1
+        },
+        {
+            "architecture": "x86_64",
+            "is_old_tag_without_os_and_arch": false,
             "major_version": 18,
             "minor_version": 1,
             "patch_version": 0,
             "sha1_prefix": "1d6270bf",
             "short_os_name_and_version": "almalinux8",
             "tag": "v18.1.0-rc2-yb-1-1708020986-1d6270bf-almalinux8-x86_64",
             "timestamp": "1708020986",
@@ -4355,28 +4425,84 @@
             "yb_suffix_version": null
         },
         {
             "architecture": "x86_64",
             "is_old_tag_without_os_and_arch": false,
             "major_version": 18,
             "minor_version": 1,
+            "patch_version": 2,
+            "sha1_prefix": "53fdd023",
+            "short_os_name_and_version": "almalinux8",
+            "tag": "v18.1.2-yb-1-1711487585-53fdd023-almalinux8-x86_64",
+            "timestamp": "1711487585",
+            "version": "18.1.2",
+            "version_suffix": "yb-1",
+            "yb_suffix_version": 1
+        },
+        {
+            "architecture": "aarch64",
+            "is_old_tag_without_os_and_arch": false,
+            "major_version": 18,
+            "minor_version": 1,
+            "patch_version": 2,
+            "sha1_prefix": "53fdd023",
+            "short_os_name_and_version": "almalinux9",
+            "tag": "v18.1.2-yb-1-1711597954-53fdd023-almalinux9-aarch64",
+            "timestamp": "1711597954",
+            "version": "18.1.2",
+            "version_suffix": "yb-1",
+            "yb_suffix_version": 1
+        },
+        {
+            "architecture": "x86_64",
+            "is_old_tag_without_os_and_arch": false,
+            "major_version": 18,
+            "minor_version": 1,
             "patch_version": 0,
             "sha1_prefix": "1d6270bf",
             "short_os_name_and_version": "almalinux9",
             "tag": "v18.1.0-rc2-yb-1-1708024704-1d6270bf-almalinux9-x86_64",
             "timestamp": "1708024704",
             "version": "18.1.0",
             "version_suffix": "rc2-yb-1",
             "yb_suffix_version": null
         },
         {
             "architecture": "x86_64",
             "is_old_tag_without_os_and_arch": false,
             "major_version": 18,
             "minor_version": 1,
+            "patch_version": 2,
+            "sha1_prefix": "53fdd023",
+            "short_os_name_and_version": "almalinux9",
+            "tag": "v18.1.2-yb-1-1711492549-53fdd023-almalinux9-x86_64",
+            "timestamp": "1711492549",
+            "version": "18.1.2",
+            "version_suffix": "yb-1",
+            "yb_suffix_version": 1
+        },
+        {
+            "architecture": "aarch64",
+            "is_old_tag_without_os_and_arch": false,
+            "major_version": 18,
+            "minor_version": 1,
+            "patch_version": 2,
+            "sha1_prefix": "53fdd023",
+            "short_os_name_and_version": "centos7",
+            "tag": "v18.1.2-yb-1-1711578240-53fdd023-centos7-aarch64",
+            "timestamp": "1711578240",
+            "version": "18.1.2",
+            "version_suffix": "yb-1",
+            "yb_suffix_version": 1
+        },
+        {
+            "architecture": "x86_64",
+            "is_old_tag_without_os_and_arch": false,
+            "major_version": 18,
+            "minor_version": 1,
             "patch_version": 0,
             "sha1_prefix": "1d6270bf",
             "short_os_name_and_version": "centos7",
             "tag": "v18.1.0-rc2-yb-1-1708017141-1d6270bf-centos7-x86_64",
             "timestamp": "1708017141",
             "version": "18.1.0",
             "version_suffix": "rc2-yb-1",
@@ -4393,14 +4519,28 @@
             "tag": "v18.1.0-rc2-yb-1-1707988845-1d6270bf-macos-arm64",
             "timestamp": "1707988845",
             "version": "18.1.0",
             "version_suffix": "rc2-yb-1",
             "yb_suffix_version": null
         },
         {
+            "architecture": "aarch64",
+            "is_old_tag_without_os_and_arch": false,
+            "major_version": 18,
+            "minor_version": 1,
+            "patch_version": 2,
+            "sha1_prefix": "53fdd023",
+            "short_os_name_and_version": "ubuntu22.04",
+            "tag": "v18.1.2-yb-1-1711607838-53fdd023-ubuntu22.04-aarch64",
+            "timestamp": "1711607838",
+            "version": "18.1.2",
+            "version_suffix": "yb-1",
+            "yb_suffix_version": 1
+        },
+        {
             "architecture": "x86_64",
             "is_old_tag_without_os_and_arch": false,
             "major_version": 18,
             "minor_version": 1,
             "patch_version": 0,
             "sha1_prefix": "1d6270bf",
             "short_os_name_and_version": "ubuntu22.04",
@@ -4411,18 +4551,46 @@
             "yb_suffix_version": null
         },
         {
             "architecture": "x86_64",
             "is_old_tag_without_os_and_arch": false,
             "major_version": 18,
             "minor_version": 1,
+            "patch_version": 2,
+            "sha1_prefix": "53fdd023",
+            "short_os_name_and_version": "ubuntu22.04",
+            "tag": "v18.1.2-yb-1-1711497241-53fdd023-ubuntu22.04-x86_64",
+            "timestamp": "1711497241",
+            "version": "18.1.2",
+            "version_suffix": "yb-1",
+            "yb_suffix_version": 1
+        },
+        {
+            "architecture": "x86_64",
+            "is_old_tag_without_os_and_arch": false,
+            "major_version": 18,
+            "minor_version": 1,
             "patch_version": 0,
             "sha1_prefix": "1d6270bf",
             "short_os_name_and_version": "ubuntu23.04",
             "tag": "v18.1.0-rc2-yb-1-1708032174-1d6270bf-ubuntu23.04-x86_64",
             "timestamp": "1708032174",
             "version": "18.1.0",
             "version_suffix": "rc2-yb-1",
             "yb_suffix_version": null
+        },
+        {
+            "architecture": "x86_64",
+            "is_old_tag_without_os_and_arch": false,
+            "major_version": 18,
+            "minor_version": 1,
+            "patch_version": 2,
+            "sha1_prefix": "53fdd023",
+            "short_os_name_and_version": "ubuntu23.04",
+            "tag": "v18.1.2-yb-1-1711501883-53fdd023-ubuntu23.04-x86_64",
+            "timestamp": "1711501883",
+            "version": "18.1.2",
+            "version_suffix": "yb-1",
+            "yb_suffix_version": 1
         }
     ]
 }
```

