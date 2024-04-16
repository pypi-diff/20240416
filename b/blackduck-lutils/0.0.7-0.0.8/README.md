# Comparing `tmp/blackduck_lutils-0.0.7.tar.gz` & `tmp/blackduck_lutils-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression, original size modulo 2^32 423065600 gzip compressed data, reserved method, has CRC, extra field, has comment, encrypted, from FAT filesystem (MS-DOS, OS/2, NT)
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression, original size modulo 2^32 423086080 gzip compressed data, reserved method, ASCII, extra field, has comment, encrypted, from FAT filesystem (MS-DOS, OS/2, NT)
```

## Comparing `blackduck_lutils-0.0.7.tar` & `blackduck_lutils-0.0.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0 86615273 2020-02-02 00:00:00.000000 blackduck_lutils-0.0.7/LicenseConflictTest_LATEST_2024-03-26_164031.csv
--rw-r--r--   0        0        0 86615273 2020-02-02 00:00:00.000000 blackduck_lutils-0.0.7/LicenseConflictTest_LATEST_2024-03-26_164829.csv
--rw-r--r--   0        0        0 86609833 2020-02-02 00:00:00.000000 blackduck_lutils-0.0.7/LicenseConflictTest_LATEST_2024-04-15_084450.csv
--rw-r--r--   0        0        0 74230649 2020-02-02 00:00:00.000000 blackduck_lutils-0.0.7/LicenseConflictTest_LATEST_2024-04-15_103052.csv
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 blackduck_lutils-0.0.7/environ.sh
--rw-r--r--   0        0        0 15841961 2020-02-02 00:00:00.000000 blackduck_lutils-0.0.7/license_data.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 blackduck_lutils-0.0.7/matched
--rw-r--r--   0        0        0 72658599 2020-02-02 00:00:00.000000 blackduck_lutils-0.0.7/nginx.log
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 blackduck_lutils-0.0.7/process.txt
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 blackduck_lutils-0.0.7/requirements.txt
--rw-r--r--   0        0        0   418653 2020-02-02 00:00:00.000000 blackduck_lutils-0.0.7/sample.json
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 blackduck_lutils-0.0.7/src/blackduck_lutils/__about__.py
--rw-r--r--   0        0        0    20028 2020-02-02 00:00:00.000000 blackduck_lutils-0.0.7/src/blackduck_lutils/license_conflicts.py
--rw-r--r--   0        0        0    12617 2020-02-02 00:00:00.000000 blackduck_lutils-0.0.7/src/blackduck_lutils/license_tagging.py
--rw-r--r--   0        0        0     2348 2020-02-02 00:00:00.000000 blackduck_lutils-0.0.7/tests/test_download_license_data.py
--rw-r--r--   0        0        0     2844 2020-02-02 00:00:00.000000 blackduck_lutils-0.0.7/tests/test_license_conflicts.py
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 blackduck_lutils-0.0.7/tests/test_license_tagging.py
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 blackduck_lutils-0.0.7/LICENSE
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 blackduck_lutils-0.0.7/README.md
--rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 blackduck_lutils-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 blackduck_lutils-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0 86615273 2020-02-02 00:00:00.000000 blackduck_lutils-0.0.8/LicenseConflictTest_LATEST_2024-03-26_164031.csv
+-rw-r--r--   0        0        0 86615273 2020-02-02 00:00:00.000000 blackduck_lutils-0.0.8/LicenseConflictTest_LATEST_2024-03-26_164829.csv
+-rw-r--r--   0        0        0 86609833 2020-02-02 00:00:00.000000 blackduck_lutils-0.0.8/LicenseConflictTest_LATEST_2024-04-15_084450.csv
+-rw-r--r--   0        0        0 74230649 2020-02-02 00:00:00.000000 blackduck_lutils-0.0.8/LicenseConflictTest_LATEST_2024-04-15_103052.csv
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 blackduck_lutils-0.0.8/environ.sh
+-rw-r--r--   0        0        0 15841961 2020-02-02 00:00:00.000000 blackduck_lutils-0.0.8/license_data.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 blackduck_lutils-0.0.8/matched
+-rw-r--r--   0        0        0 72658599 2020-02-02 00:00:00.000000 blackduck_lutils-0.0.8/nginx.log
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 blackduck_lutils-0.0.8/process.txt
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 blackduck_lutils-0.0.8/requirements.txt
+-rw-r--r--   0        0        0   418653 2020-02-02 00:00:00.000000 blackduck_lutils-0.0.8/sample.json
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 blackduck_lutils-0.0.8/src/blackduck_lutils/__about__.py
+-rw-r--r--   0        0        0    20028 2020-02-02 00:00:00.000000 blackduck_lutils-0.0.8/src/blackduck_lutils/license_conflicts.py
+-rw-r--r--   0        0        0    12617 2020-02-02 00:00:00.000000 blackduck_lutils-0.0.8/src/blackduck_lutils/license_tagging.py
+-rw-r--r--   0        0        0     2348 2020-02-02 00:00:00.000000 blackduck_lutils-0.0.8/tests/test_download_license_data.py
+-rw-r--r--   0        0        0     2844 2020-02-02 00:00:00.000000 blackduck_lutils-0.0.8/tests/test_license_conflicts.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 blackduck_lutils-0.0.8/tests/test_license_tagging.py
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 blackduck_lutils-0.0.8/LICENSE
+-rw-r--r--   0        0        0    10135 2020-02-02 00:00:00.000000 blackduck_lutils-0.0.8/README.md
+-rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 blackduck_lutils-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0    11173 2020-02-02 00:00:00.000000 blackduck_lutils-0.0.8/PKG-INFO
```

### Comparing `blackduck_lutils-0.0.7/LicenseConflictTest_LATEST_2024-03-26_164031.csv` & `blackduck_lutils-0.0.8/LicenseConflictTest_LATEST_2024-03-26_164031.csv`

 * *Files identical despite different names*

### Comparing `blackduck_lutils-0.0.7/LicenseConflictTest_LATEST_2024-03-26_164829.csv` & `blackduck_lutils-0.0.8/LicenseConflictTest_LATEST_2024-03-26_164829.csv`

 * *Files identical despite different names*

### Comparing `blackduck_lutils-0.0.7/LicenseConflictTest_LATEST_2024-04-15_084450.csv` & `blackduck_lutils-0.0.8/LicenseConflictTest_LATEST_2024-04-15_084450.csv`

 * *Files identical despite different names*

### Comparing `blackduck_lutils-0.0.7/LicenseConflictTest_LATEST_2024-04-15_103052.csv` & `blackduck_lutils-0.0.8/LicenseConflictTest_LATEST_2024-04-15_103052.csv`

 * *Files identical despite different names*

### Comparing `blackduck_lutils-0.0.7/license_data.json` & `blackduck_lutils-0.0.8/license_data.json`

 * *Files identical despite different names*

### Comparing `blackduck_lutils-0.0.7/nginx.log` & `blackduck_lutils-0.0.8/nginx.log`

 * *Files identical despite different names*

### Comparing `blackduck_lutils-0.0.7/sample.json` & `blackduck_lutils-0.0.8/sample.json`

 * *Files identical despite different names*

### Comparing `blackduck_lutils-0.0.7/src/blackduck_lutils/license_conflicts.py` & `blackduck_lutils-0.0.8/src/blackduck_lutils/license_conflicts.py`

 * *Files identical despite different names*

### Comparing `blackduck_lutils-0.0.7/src/blackduck_lutils/license_tagging.py` & `blackduck_lutils-0.0.8/src/blackduck_lutils/license_tagging.py`

 * *Files identical despite different names*

### Comparing `blackduck_lutils-0.0.7/tests/test_download_license_data.py` & `blackduck_lutils-0.0.8/tests/test_download_license_data.py`

 * *Files identical despite different names*

### Comparing `blackduck_lutils-0.0.7/tests/test_license_conflicts.py` & `blackduck_lutils-0.0.8/tests/test_license_conflicts.py`

 * *Files identical despite different names*

### Comparing `blackduck_lutils-0.0.7/LICENSE` & `blackduck_lutils-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `blackduck_lutils-0.0.7/pyproject.toml` & `blackduck_lutils-0.0.8/pyproject.toml`

 * *Files identical despite different names*

