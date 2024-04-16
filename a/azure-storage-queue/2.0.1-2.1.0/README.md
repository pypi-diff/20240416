# Comparing `tmp/azure-storage-queue-2.0.1.tar.gz` & `tmp/azure-storage-queue-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "../dist/azure-storage-queue-2.0.1.tar", last modified: Thu May  9 19:54:08 2019, max compression
+gzip compressed data, was "../dist/azure-storage-queue-2.1.0.tar", last modified: Fri Aug  2 04:12:47 2019, max compression
```

## Comparing `azure-storage-queue-2.0.1.tar` & `azure-storage-queue-2.1.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 zed        (501) staff       (20)        0 2019-05-09 19:54:08.000000 azure-storage-queue-2.0.1/
--rw-r--r--   0 zed        (501) staff       (20)     1075 2019-05-09 02:25:10.000000 azure-storage-queue-2.0.1/LICENSE.txt
--rw-r--r--   0 zed        (501) staff       (20)       94 2019-05-09 02:25:10.000000 azure-storage-queue-2.0.1/MANIFEST.in
--rw-r--r--   0 zed        (501) staff       (20)     9757 2019-05-09 19:54:08.000000 azure-storage-queue-2.0.1/PKG-INFO
--rw-r--r--   0 zed        (501) staff       (20)     7067 2019-05-09 02:25:10.000000 azure-storage-queue-2.0.1/README.rst
-drwxr-xr-x   0 zed        (501) staff       (20)        0 2019-05-09 19:54:08.000000 azure-storage-queue-2.0.1/azure/
--rw-r--r--   0 zed        (501) staff       (20)       64 2019-05-09 02:25:10.000000 azure-storage-queue-2.0.1/azure/__init__.py
-drwxr-xr-x   0 zed        (501) staff       (20)        0 2019-05-09 19:54:08.000000 azure-storage-queue-2.0.1/azure/storage/
--rw-r--r--   0 zed        (501) staff       (20)       64 2019-05-09 02:25:10.000000 azure-storage-queue-2.0.1/azure/storage/__init__.py
-drwxr-xr-x   0 zed        (501) staff       (20)        0 2019-05-09 19:54:08.000000 azure-storage-queue-2.0.1/azure/storage/queue/
--rw-r--r--   0 zed        (501) staff       (20)      449 2019-05-09 02:25:10.000000 azure-storage-queue-2.0.1/azure/storage/queue/__init__.py
--rw-r--r--   0 zed        (501) staff       (20)      454 2019-05-09 19:47:55.000000 azure-storage-queue-2.0.1/azure/storage/queue/_constants.py
--rw-r--r--   0 zed        (501) staff       (20)     4935 2019-05-09 02:25:10.000000 azure-storage-queue-2.0.1/azure/storage/queue/_deserialization.py
--rw-r--r--   0 zed        (501) staff       (20)     6728 2019-05-09 02:25:10.000000 azure-storage-queue-2.0.1/azure/storage/queue/_encryption.py
--rw-r--r--   0 zed        (501) staff       (20)     1027 2019-05-09 02:25:10.000000 azure-storage-queue-2.0.1/azure/storage/queue/_error.py
--rw-r--r--   0 zed        (501) staff       (20)     2173 2019-05-09 02:25:10.000000 azure-storage-queue-2.0.1/azure/storage/queue/_serialization.py
--rw-r--r--   0 zed        (501) staff       (20)     8067 2019-05-09 02:25:10.000000 azure-storage-queue-2.0.1/azure/storage/queue/models.py
--rw-r--r--   0 zed        (501) staff       (20)    48435 2019-05-09 02:25:10.000000 azure-storage-queue-2.0.1/azure/storage/queue/queueservice.py
--rw-r--r--   0 zed        (501) staff       (20)     5595 2019-05-09 02:25:39.000000 azure-storage-queue-2.0.1/azure/storage/queue/sharedaccesssignature.py
-drwxr-xr-x   0 zed        (501) staff       (20)        0 2019-05-09 19:54:08.000000 azure-storage-queue-2.0.1/azure_storage_queue.egg-info/
--rw-r--r--   0 zed        (501) staff       (20)     9757 2019-05-09 19:54:08.000000 azure-storage-queue-2.0.1/azure_storage_queue.egg-info/PKG-INFO
--rw-r--r--   0 zed        (501) staff       (20)      673 2019-05-09 19:54:08.000000 azure-storage-queue-2.0.1/azure_storage_queue.egg-info/SOURCES.txt
--rw-r--r--   0 zed        (501) staff       (20)        1 2019-05-09 19:54:08.000000 azure-storage-queue-2.0.1/azure_storage_queue.egg-info/dependency_links.txt
--rw-r--r--   0 zed        (501) staff       (20)        1 2019-05-09 19:54:08.000000 azure-storage-queue-2.0.1/azure_storage_queue.egg-info/not-zip-safe
--rw-r--r--   0 zed        (501) staff       (20)       46 2019-05-09 19:54:08.000000 azure-storage-queue-2.0.1/azure_storage_queue.egg-info/requires.txt
--rw-r--r--   0 zed        (501) staff       (20)        6 2019-05-09 19:54:08.000000 azure-storage-queue-2.0.1/azure_storage_queue.egg-info/top_level.txt
--rw-r--r--   0 zed        (501) staff       (20)       67 2019-05-09 19:54:08.000000 azure-storage-queue-2.0.1/setup.cfg
--rw-r--r--   0 zed        (501) staff       (20)     2381 2019-05-09 19:50:54.000000 azure-storage-queue-2.0.1/setup.py
+drwxr-xr-x   0 zed        (501) staff       (20)        0 2019-08-02 04:12:47.000000 azure-storage-queue-2.1.0/
+-rw-r--r--   0 zed        (501) staff       (20)     1075 2019-06-07 07:59:17.000000 azure-storage-queue-2.1.0/LICENSE.txt
+-rw-r--r--   0 zed        (501) staff       (20)       94 2019-06-07 07:59:17.000000 azure-storage-queue-2.1.0/MANIFEST.in
+-rw-r--r--   0 zed        (501) staff       (20)     9757 2019-08-02 04:12:47.000000 azure-storage-queue-2.1.0/PKG-INFO
+-rw-r--r--   0 zed        (501) staff       (20)     7067 2019-05-09 02:25:10.000000 azure-storage-queue-2.1.0/README.rst
+drwxr-xr-x   0 zed        (501) staff       (20)        0 2019-08-02 04:12:47.000000 azure-storage-queue-2.1.0/azure/
+-rw-r--r--   0 zed        (501) staff       (20)       64 2019-05-09 02:25:10.000000 azure-storage-queue-2.1.0/azure/__init__.py
+drwxr-xr-x   0 zed        (501) staff       (20)        0 2019-08-02 04:12:47.000000 azure-storage-queue-2.1.0/azure/storage/
+-rw-r--r--   0 zed        (501) staff       (20)       64 2019-05-09 02:25:10.000000 azure-storage-queue-2.1.0/azure/storage/__init__.py
+drwxr-xr-x   0 zed        (501) staff       (20)        0 2019-08-02 04:12:47.000000 azure-storage-queue-2.1.0/azure/storage/queue/
+-rw-r--r--   0 zed        (501) staff       (20)      485 2019-07-29 19:18:27.000000 azure-storage-queue-2.1.0/azure/storage/queue/__init__.py
+-rw-r--r--   0 zed        (501) staff       (20)      454 2019-08-02 04:03:48.000000 azure-storage-queue-2.1.0/azure/storage/queue/_constants.py
+-rw-r--r--   0 zed        (501) staff       (20)     4935 2019-05-09 02:25:10.000000 azure-storage-queue-2.1.0/azure/storage/queue/_deserialization.py
+-rw-r--r--   0 zed        (501) staff       (20)     6728 2019-06-07 07:59:17.000000 azure-storage-queue-2.1.0/azure/storage/queue/_encryption.py
+-rw-r--r--   0 zed        (501) staff       (20)     1027 2019-05-09 02:25:10.000000 azure-storage-queue-2.1.0/azure/storage/queue/_error.py
+-rw-r--r--   0 zed        (501) staff       (20)     2173 2019-05-09 02:25:10.000000 azure-storage-queue-2.1.0/azure/storage/queue/_serialization.py
+-rw-r--r--   0 zed        (501) staff       (20)     8067 2019-05-09 02:25:10.000000 azure-storage-queue-2.1.0/azure/storage/queue/models.py
+-rw-r--r--   0 zed        (501) staff       (20)    48435 2019-05-09 02:25:10.000000 azure-storage-queue-2.1.0/azure/storage/queue/queueservice.py
+-rw-r--r--   0 zed        (501) staff       (20)     5595 2019-06-07 07:59:17.000000 azure-storage-queue-2.1.0/azure/storage/queue/sharedaccesssignature.py
+drwxr-xr-x   0 zed        (501) staff       (20)        0 2019-08-02 04:12:47.000000 azure-storage-queue-2.1.0/azure_storage_queue.egg-info/
+-rw-r--r--   0 zed        (501) staff       (20)     9757 2019-08-02 04:12:47.000000 azure-storage-queue-2.1.0/azure_storage_queue.egg-info/PKG-INFO
+-rw-r--r--   0 zed        (501) staff       (20)      673 2019-08-02 04:12:47.000000 azure-storage-queue-2.1.0/azure_storage_queue.egg-info/SOURCES.txt
+-rw-r--r--   0 zed        (501) staff       (20)        1 2019-08-02 04:12:47.000000 azure-storage-queue-2.1.0/azure_storage_queue.egg-info/dependency_links.txt
+-rw-r--r--   0 zed        (501) staff       (20)        1 2019-08-02 04:12:47.000000 azure-storage-queue-2.1.0/azure_storage_queue.egg-info/not-zip-safe
+-rw-r--r--   0 zed        (501) staff       (20)       46 2019-08-02 04:12:47.000000 azure-storage-queue-2.1.0/azure_storage_queue.egg-info/requires.txt
+-rw-r--r--   0 zed        (501) staff       (20)        6 2019-08-02 04:12:47.000000 azure-storage-queue-2.1.0/azure_storage_queue.egg-info/top_level.txt
+-rw-r--r--   0 zed        (501) staff       (20)       67 2019-08-02 04:12:47.000000 azure-storage-queue-2.1.0/setup.cfg
+-rw-r--r--   0 zed        (501) staff       (20)     2381 2019-08-02 04:04:11.000000 azure-storage-queue-2.1.0/setup.py
```

### Comparing `azure-storage-queue-2.0.1/LICENSE.txt` & `azure-storage-queue-2.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `azure-storage-queue-2.0.1/PKG-INFO` & `azure-storage-queue-2.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: azure-storage-queue
-Version: 2.0.1
+Version: 2.1.0
 Summary: Microsoft Azure Storage Queue Client Library for Python
 Home-page: https://github.com/Azure/azure-storage-python
 Author: Microsoft Corporation
 Author-email: ascl@microsoft.com
 License: MIT License
 Description: Microsoft Azure Storage SDK for Python
         ======================================
```

### Comparing `azure-storage-queue-2.0.1/README.rst` & `azure-storage-queue-2.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `azure-storage-queue-2.0.1/azure/storage/queue/_deserialization.py` & `azure-storage-queue-2.1.0/azure/storage/queue/_deserialization.py`

 * *Files identical despite different names*

### Comparing `azure-storage-queue-2.0.1/azure/storage/queue/_encryption.py` & `azure-storage-queue-2.1.0/azure/storage/queue/_encryption.py`

 * *Files identical despite different names*

### Comparing `azure-storage-queue-2.0.1/azure/storage/queue/_error.py` & `azure-storage-queue-2.1.0/azure/storage/queue/_error.py`

 * *Files identical despite different names*

### Comparing `azure-storage-queue-2.0.1/azure/storage/queue/_serialization.py` & `azure-storage-queue-2.1.0/azure/storage/queue/_serialization.py`

 * *Files identical despite different names*

### Comparing `azure-storage-queue-2.0.1/azure/storage/queue/models.py` & `azure-storage-queue-2.1.0/azure/storage/queue/models.py`

 * *Files identical despite different names*

### Comparing `azure-storage-queue-2.0.1/azure/storage/queue/queueservice.py` & `azure-storage-queue-2.1.0/azure/storage/queue/queueservice.py`

 * *Files identical despite different names*

### Comparing `azure-storage-queue-2.0.1/azure/storage/queue/sharedaccesssignature.py` & `azure-storage-queue-2.1.0/azure/storage/queue/sharedaccesssignature.py`

 * *Files identical despite different names*

### Comparing `azure-storage-queue-2.0.1/azure_storage_queue.egg-info/PKG-INFO` & `azure-storage-queue-2.1.0/azure_storage_queue.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: azure-storage-queue
-Version: 2.0.1
+Version: 2.1.0
 Summary: Microsoft Azure Storage Queue Client Library for Python
 Home-page: https://github.com/Azure/azure-storage-python
 Author: Microsoft Corporation
 Author-email: ascl@microsoft.com
 License: MIT License
 Description: Microsoft Azure Storage SDK for Python
         ======================================
```

### Comparing `azure-storage-queue-2.0.1/azure_storage_queue.egg-info/SOURCES.txt` & `azure-storage-queue-2.1.0/azure_storage_queue.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `azure-storage-queue-2.0.1/setup.py` & `azure-storage-queue-2.1.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     except AttributeError:
         pass
 except ImportError:
     pass
 
 setup(
     name='azure-storage-queue',
-    version='2.0.1',
+    version='2.1.0',
     description='Microsoft Azure Storage Queue Client Library for Python',
     long_description=open('README.rst', 'r').read(),
     license='MIT License',
     author='Microsoft Corporation',
     author_email='ascl@microsoft.com',
     url='https://github.com/Azure/azure-storage-python',
     classifiers=[
@@ -68,10 +68,10 @@
     packages=find_packages(exclude=[
         # Exclude packages that will be covered by PEP420 or nspkg
         'azure',
         'azure.storage',
     ]),
     install_requires=[
         'azure-common>=1.1.5',
-        'azure-storage-common~=2.0'
+        'azure-storage-common~=2.1'
     ],
 )
```

