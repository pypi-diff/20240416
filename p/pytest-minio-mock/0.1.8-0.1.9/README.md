# Comparing `tmp/pytest-minio-mock-0.1.8.tar.gz` & `tmp/pytest-minio-mock-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-minio-mock-0.1.8.tar", last modified: Sun Dec 24 15:05:02 2023, max compression
+gzip compressed data, was "pytest-minio-mock-0.1.9.tar", last modified: Thu Jan  4 11:52:09 2024, max compression
```

## Comparing `pytest-minio-mock-0.1.8.tar` & `pytest-minio-mock-0.1.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 ouss       (501) staff       (20)        0 2023-12-24 15:05:02.410068 pytest-minio-mock-0.1.8/
--rw-r--r--   0 ouss       (501) staff       (20)        0 2023-11-28 14:02:23.000000 pytest-minio-mock-0.1.8/LICENSE
--rw-r--r--   0 ouss       (501) staff       (20)        0 2023-11-28 15:52:51.000000 pytest-minio-mock-0.1.8/MANIFEST.in
--rw-r--r--   0 ouss       (501) staff       (20)     4081 2023-12-24 15:05:02.409846 pytest-minio-mock-0.1.8/PKG-INFO
--rw-r--r--   0 ouss       (501) staff       (20)     2759 2023-12-24 15:00:59.000000 pytest-minio-mock-0.1.8/README.md
-drwxr-xr-x   0 ouss       (501) staff       (20)        0 2023-12-24 15:05:02.407792 pytest-minio-mock-0.1.8/pytest_minio_mock/
--rw-r--r--   0 ouss       (501) staff       (20)       54 2023-12-24 12:44:54.000000 pytest-minio-mock-0.1.8/pytest_minio_mock/__init__.py
--rw-r--r--   0 ouss       (501) staff       (20)    10102 2023-12-24 12:44:16.000000 pytest-minio-mock-0.1.8/pytest_minio_mock/plugin.py
-drwxr-xr-x   0 ouss       (501) staff       (20)        0 2023-12-24 15:05:02.409505 pytest-minio-mock-0.1.8/pytest_minio_mock.egg-info/
--rw-r--r--   0 ouss       (501) staff       (20)     4081 2023-12-24 15:05:02.000000 pytest-minio-mock-0.1.8/pytest_minio_mock.egg-info/PKG-INFO
--rw-r--r--   0 ouss       (501) staff       (20)      405 2023-12-24 15:05:02.000000 pytest-minio-mock-0.1.8/pytest_minio_mock.egg-info/SOURCES.txt
--rw-r--r--   0 ouss       (501) staff       (20)        1 2023-12-24 15:05:02.000000 pytest-minio-mock-0.1.8/pytest_minio_mock.egg-info/dependency_links.txt
--rw-r--r--   0 ouss       (501) staff       (20)       56 2023-12-24 15:05:02.000000 pytest-minio-mock-0.1.8/pytest_minio_mock.egg-info/entry_points.txt
--rw-r--r--   0 ouss       (501) staff       (20)       65 2023-12-24 15:05:02.000000 pytest-minio-mock-0.1.8/pytest_minio_mock.egg-info/requires.txt
--rw-r--r--   0 ouss       (501) staff       (20)       24 2023-12-24 15:05:02.000000 pytest-minio-mock-0.1.8/pytest_minio_mock.egg-info/top_level.txt
--rw-r--r--   0 ouss       (501) staff       (20)       38 2023-12-24 15:05:02.410113 pytest-minio-mock-0.1.8/setup.cfg
--rw-r--r--   0 ouss       (501) staff       (20)     1762 2023-12-24 12:44:46.000000 pytest-minio-mock-0.1.8/setup.py
-drwxr-xr-x   0 ouss       (501) staff       (20)        0 2023-12-24 15:05:02.409242 pytest-minio-mock-0.1.8/tests/
--rw-r--r--   0 ouss       (501) staff       (20)        0 2023-11-28 14:02:59.000000 pytest-minio-mock-0.1.8/tests/__init__.py
--rw-r--r--   0 ouss       (501) staff       (20)      104 2023-12-19 09:41:11.000000 pytest-minio-mock-0.1.8/tests/conftest.py
--rw-r--r--   0 ouss       (501) staff       (20)     4191 2023-12-24 12:44:16.000000 pytest-minio-mock-0.1.8/tests/test_minio_mock.py
+drwxr-xr-x   0 ouss       (501) staff       (20)        0 2024-01-04 11:52:09.827764 pytest-minio-mock-0.1.9/
+-rw-r--r--   0 ouss       (501) staff       (20)        0 2023-11-28 14:02:23.000000 pytest-minio-mock-0.1.9/LICENSE
+-rw-r--r--   0 ouss       (501) staff       (20)        0 2023-11-28 15:52:51.000000 pytest-minio-mock-0.1.9/MANIFEST.in
+-rw-r--r--   0 ouss       (501) staff       (20)     4714 2024-01-04 11:52:09.827554 pytest-minio-mock-0.1.9/PKG-INFO
+-rw-r--r--   0 ouss       (501) staff       (20)     3392 2024-01-04 11:51:43.000000 pytest-minio-mock-0.1.9/README.md
+drwxr-xr-x   0 ouss       (501) staff       (20)        0 2024-01-04 11:52:09.825633 pytest-minio-mock-0.1.9/pytest_minio_mock/
+-rw-r--r--   0 ouss       (501) staff       (20)      721 2024-01-04 11:51:43.000000 pytest-minio-mock-0.1.9/pytest_minio_mock/__init__.py
+-rw-r--r--   0 ouss       (501) staff       (20)    24263 2024-01-04 11:51:43.000000 pytest-minio-mock-0.1.9/pytest_minio_mock/plugin.py
+drwxr-xr-x   0 ouss       (501) staff       (20)        0 2024-01-04 11:52:09.827212 pytest-minio-mock-0.1.9/pytest_minio_mock.egg-info/
+-rw-r--r--   0 ouss       (501) staff       (20)     4714 2024-01-04 11:52:09.000000 pytest-minio-mock-0.1.9/pytest_minio_mock.egg-info/PKG-INFO
+-rw-r--r--   0 ouss       (501) staff       (20)      405 2024-01-04 11:52:09.000000 pytest-minio-mock-0.1.9/pytest_minio_mock.egg-info/SOURCES.txt
+-rw-r--r--   0 ouss       (501) staff       (20)        1 2024-01-04 11:52:09.000000 pytest-minio-mock-0.1.9/pytest_minio_mock.egg-info/dependency_links.txt
+-rw-r--r--   0 ouss       (501) staff       (20)       56 2024-01-04 11:52:09.000000 pytest-minio-mock-0.1.9/pytest_minio_mock.egg-info/entry_points.txt
+-rw-r--r--   0 ouss       (501) staff       (20)       65 2024-01-04 11:52:09.000000 pytest-minio-mock-0.1.9/pytest_minio_mock.egg-info/requires.txt
+-rw-r--r--   0 ouss       (501) staff       (20)       18 2024-01-04 11:52:09.000000 pytest-minio-mock-0.1.9/pytest_minio_mock.egg-info/top_level.txt
+-rw-r--r--   0 ouss       (501) staff       (20)       38 2024-01-04 11:52:09.827813 pytest-minio-mock-0.1.9/setup.cfg
+-rw-r--r--   0 ouss       (501) staff       (20)     1780 2024-01-04 11:51:43.000000 pytest-minio-mock-0.1.9/setup.py
+drwxr-xr-x   0 ouss       (501) staff       (20)        0 2024-01-04 11:52:09.827017 pytest-minio-mock-0.1.9/tests/
+-rw-r--r--   0 ouss       (501) staff       (20)        0 2023-11-28 14:02:59.000000 pytest-minio-mock-0.1.9/tests/__init__.py
+-rw-r--r--   0 ouss       (501) staff       (20)      104 2023-12-19 09:41:11.000000 pytest-minio-mock-0.1.9/tests/conftest.py
+-rw-r--r--   0 ouss       (501) staff       (20)     4191 2024-01-04 10:30:51.000000 pytest-minio-mock-0.1.9/tests/test_minio_mock.py
```

### Comparing `pytest-minio-mock-0.1.8/PKG-INFO` & `pytest-minio-mock-0.1.9/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-minio-mock
-Version: 0.1.8
+Version: 0.1.9
 Summary: A pytest plugin for mocking Minio S3 interactions
 Home-page: https://github.com/oussjarrousse/pytest-minio-mock
 Author: Oussama Jarrousse
 Author-email: oussama@jarrousse.org
 License: MIT
 Project-URL: Source, https://github.com/oussjarrousse/pytest-minio-mock/
 Project-URL: Tracker, https://github.com/oussjarrousse/pytest-minio-mock/issues
@@ -31,14 +31,19 @@
 Requires-Dist: validators
 Provides-Extra: dev
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: tox; extra == "dev"
 
 # pytest-minio-mock
 
+### Pip Stats
+[![PyPI version](https://badge.fury.io/py/pytest-minio-mock.svg)](https://badge.fury.io/py/pytest-minio-mock)
+[![Downloads](https://static.pepy.tech/badge/pytest-minio-mock)](https://pepy.tech/project/pytest-minio-mock)
+[![linting: pylint](https://img.shields.io/badge/linting-pylint-yellowgreen)](https://github.com/pylint-dev/pylint)
+
 ## Overview
 `pytest-minio-mock` is a pytest plugin designed to simplify testing of applications that interact with Minio the code  S3 compatible object storage system. It is not designed to test the correnction to the minio server. It provides a fixture that mocks the `minio.Minio` class, allowing for easy testing of Minio interactions without the need for a real Minio server.
 
 ## Features
 - Mock implementation of the `minio.Minio` client.
 - Easy to use pytest fixture.
 - Supports common Minio operations such as bucket creation, file upload/download, etc.
@@ -59,31 +64,42 @@
     try:
         minio_client = minio.Minio(
             endpoint=S3_URI,
             access_key=S3_ACCESS_KEY,
             secret_key=S3_SECRET_KEY,
             region=S3_REGION
         )
-        minio_client.make_bucket("buckets")
+        return minio_client.make_bucket("buckets")
     except Exception as e:
         logging.error(e)
 
+
 def test_file_upload(minio_mock):
     # Calling function foo that involves using minio.Minio()
     assert foo()
+    minio_client = minio.Minio(
+            endpoint=S3_URI,
+            access_key=S3_ACCESS_KEY,
+            secret_key=S3_SECRET_KEY,
+            region=S3_REGION
+        )
+    buckets = minio.list_buckets()
+    assert len(buckets)==1
 
 ```
 
 The `minio_mock` fixture will patch newly created minio.Minio() thus providing you with a way to test your code around the Minio client easily.
 
 At the moment, instances of minio.Minio() created before loading the minio_mock fixture code will not be patched. This might be an issue if one or more of the fixtures you are using in your tests that preceeds `minio_mock` in the parameters list of the test function, initiates instances of minio.Minio() that you want to test. As a workaround make sure that minio_mock is the first fixture in the list of arguments of function where minio_mock is needed. Example:
 
-```
+```python
 @pytest.fixture()
 def system_under_test(minio_mock: MockMinioClient, storage_provider_stub: StorageProvider):
+    # your code here
+    pass
 ```
 
 ## API
 
 ### MockMinioClient
 
 A brief description of the mocked methods and their behavior, like:
```

### Comparing `pytest-minio-mock-0.1.8/README.md` & `pytest-minio-mock-0.1.9/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 # pytest-minio-mock
 
+### Pip Stats
+[![PyPI version](https://badge.fury.io/py/pytest-minio-mock.svg)](https://badge.fury.io/py/pytest-minio-mock)
+[![Downloads](https://static.pepy.tech/badge/pytest-minio-mock)](https://pepy.tech/project/pytest-minio-mock)
+[![linting: pylint](https://img.shields.io/badge/linting-pylint-yellowgreen)](https://github.com/pylint-dev/pylint)
+
 ## Overview
 `pytest-minio-mock` is a pytest plugin designed to simplify testing of applications that interact with Minio the code  S3 compatible object storage system. It is not designed to test the correnction to the minio server. It provides a fixture that mocks the `minio.Minio` class, allowing for easy testing of Minio interactions without the need for a real Minio server.
 
 ## Features
 - Mock implementation of the `minio.Minio` client.
 - Easy to use pytest fixture.
 - Supports common Minio operations such as bucket creation, file upload/download, etc.
@@ -24,31 +29,42 @@
     try:
         minio_client = minio.Minio(
             endpoint=S3_URI,
             access_key=S3_ACCESS_KEY,
             secret_key=S3_SECRET_KEY,
             region=S3_REGION
         )
-        minio_client.make_bucket("buckets")
+        return minio_client.make_bucket("buckets")
     except Exception as e:
         logging.error(e)
 
+
 def test_file_upload(minio_mock):
     # Calling function foo that involves using minio.Minio()
     assert foo()
+    minio_client = minio.Minio(
+            endpoint=S3_URI,
+            access_key=S3_ACCESS_KEY,
+            secret_key=S3_SECRET_KEY,
+            region=S3_REGION
+        )
+    buckets = minio.list_buckets()
+    assert len(buckets)==1
 
 ```
 
 The `minio_mock` fixture will patch newly created minio.Minio() thus providing you with a way to test your code around the Minio client easily.
 
 At the moment, instances of minio.Minio() created before loading the minio_mock fixture code will not be patched. This might be an issue if one or more of the fixtures you are using in your tests that preceeds `minio_mock` in the parameters list of the test function, initiates instances of minio.Minio() that you want to test. As a workaround make sure that minio_mock is the first fixture in the list of arguments of function where minio_mock is needed. Example:
 
-```
+```python
 @pytest.fixture()
 def system_under_test(minio_mock: MockMinioClient, storage_provider_stub: StorageProvider):
+    # your code here
+    pass
 ```
 
 ## API
 
 ### MockMinioClient
 
 A brief description of the mocked methods and their behavior, like:
```

### Comparing `pytest-minio-mock-0.1.8/pytest_minio_mock.egg-info/PKG-INFO` & `pytest-minio-mock-0.1.9/pytest_minio_mock.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-minio-mock
-Version: 0.1.8
+Version: 0.1.9
 Summary: A pytest plugin for mocking Minio S3 interactions
 Home-page: https://github.com/oussjarrousse/pytest-minio-mock
 Author: Oussama Jarrousse
 Author-email: oussama@jarrousse.org
 License: MIT
 Project-URL: Source, https://github.com/oussjarrousse/pytest-minio-mock/
 Project-URL: Tracker, https://github.com/oussjarrousse/pytest-minio-mock/issues
@@ -31,14 +31,19 @@
 Requires-Dist: validators
 Provides-Extra: dev
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: tox; extra == "dev"
 
 # pytest-minio-mock
 
+### Pip Stats
+[![PyPI version](https://badge.fury.io/py/pytest-minio-mock.svg)](https://badge.fury.io/py/pytest-minio-mock)
+[![Downloads](https://static.pepy.tech/badge/pytest-minio-mock)](https://pepy.tech/project/pytest-minio-mock)
+[![linting: pylint](https://img.shields.io/badge/linting-pylint-yellowgreen)](https://github.com/pylint-dev/pylint)
+
 ## Overview
 `pytest-minio-mock` is a pytest plugin designed to simplify testing of applications that interact with Minio the code  S3 compatible object storage system. It is not designed to test the correnction to the minio server. It provides a fixture that mocks the `minio.Minio` class, allowing for easy testing of Minio interactions without the need for a real Minio server.
 
 ## Features
 - Mock implementation of the `minio.Minio` client.
 - Easy to use pytest fixture.
 - Supports common Minio operations such as bucket creation, file upload/download, etc.
@@ -59,31 +64,42 @@
     try:
         minio_client = minio.Minio(
             endpoint=S3_URI,
             access_key=S3_ACCESS_KEY,
             secret_key=S3_SECRET_KEY,
             region=S3_REGION
         )
-        minio_client.make_bucket("buckets")
+        return minio_client.make_bucket("buckets")
     except Exception as e:
         logging.error(e)
 
+
 def test_file_upload(minio_mock):
     # Calling function foo that involves using minio.Minio()
     assert foo()
+    minio_client = minio.Minio(
+            endpoint=S3_URI,
+            access_key=S3_ACCESS_KEY,
+            secret_key=S3_SECRET_KEY,
+            region=S3_REGION
+        )
+    buckets = minio.list_buckets()
+    assert len(buckets)==1
 
 ```
 
 The `minio_mock` fixture will patch newly created minio.Minio() thus providing you with a way to test your code around the Minio client easily.
 
 At the moment, instances of minio.Minio() created before loading the minio_mock fixture code will not be patched. This might be an issue if one or more of the fixtures you are using in your tests that preceeds `minio_mock` in the parameters list of the test function, initiates instances of minio.Minio() that you want to test. As a workaround make sure that minio_mock is the first fixture in the list of arguments of function where minio_mock is needed. Example:
 
-```
+```python
 @pytest.fixture()
 def system_under_test(minio_mock: MockMinioClient, storage_provider_stub: StorageProvider):
+    # your code here
+    pass
 ```
 
 ## API
 
 ### MockMinioClient
 
 A brief description of the mocked methods and their behavior, like:
```

### Comparing `pytest-minio-mock-0.1.8/setup.py` & `pytest-minio-mock-0.1.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,27 +5,27 @@
 setup(
     name="pytest-minio-mock",
     entry_points={
         "pytest11": [
             "pytest_minio_mock = pytest_minio_mock.plugin",
         ],
     },
-    packages=find_packages(),
+    packages=find_packages(exclude=("tests",)),
     platforms="any",
     python_requires=">=3.6",
     install_requires=["pytest>=5.0.0", "minio", "pytest-mock", "validators"],
     url="https://github.com/oussjarrousse/pytest-minio-mock",
     license="MIT",
     author="Oussama Jarrousse",
     author_email="oussama@jarrousse.org",
     description="A pytest plugin for mocking Minio S3 interactions",
     long_description=open("README.md").read(),
     keywords="pytest minio mock",
     extras_require={"dev": ["pre-commit", "tox"]},
-    version="0.1.8",
+    version="0.1.9",
     long_description_content_type="text/markdown",
     classifiers=[
         "Framework :: Pytest",
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Intended Audience :: Developers",
```

### Comparing `pytest-minio-mock-0.1.8/tests/test_minio_mock.py` & `pytest-minio-mock-0.1.9/tests/test_minio_mock.py`

 * *Files identical despite different names*

