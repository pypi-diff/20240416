# Comparing `tmp/eth-typing-4.1.0.tar.gz` & `tmp/eth_typing-4.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eth-typing-4.1.0.tar", last modified: Mon Apr  1 19:28:09 2024, max compression
+gzip compressed data, was "eth_typing-4.2.0.tar", last modified: Mon Apr 15 20:35:39 2024, max compression
```

## Comparing `eth-typing-4.1.0.tar` & `eth_typing-4.2.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-04-01 19:28:09.088426 eth-typing-4.1.0/
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1095 2024-03-25 21:51:21.000000 eth-typing-4.1.0/LICENSE
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      168 2024-03-25 21:51:21.000000 eth-typing-4.1.0/MANIFEST.in
--rw-r--r--   0 pacrob    (1000) pacrob    (1000)     5005 2024-04-01 19:28:09.088426 eth-typing-4.1.0/PKG-INFO
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     3285 2024-03-25 21:51:21.000000 eth-typing-4.1.0/README.md
-drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-04-01 19:28:09.084426 eth-typing-4.1.0/eth_typing/
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      952 2024-03-25 21:51:21.000000 eth-typing-4.1.0/eth_typing/__init__.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)       85 2024-03-25 21:51:21.000000 eth-typing-4.1.0/eth_typing/abi.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      191 2024-03-25 21:51:21.000000 eth-typing-4.1.0/eth_typing/bls.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)       71 2024-03-25 21:51:21.000000 eth-typing-4.1.0/eth_typing/discovery.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      117 2024-03-25 21:51:21.000000 eth-typing-4.1.0/eth_typing/encoding.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      458 2024-03-25 21:51:21.000000 eth-typing-4.1.0/eth_typing/enums.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      173 2024-03-25 21:51:21.000000 eth-typing-4.1.0/eth_typing/ethpm.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      546 2024-03-25 21:51:21.000000 eth-typing-4.1.0/eth_typing/evm.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)    20845 2024-03-25 21:51:21.000000 eth-typing-4.1.0/eth_typing/networks.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)        0 2024-03-25 21:51:21.000000 eth-typing-4.1.0/eth_typing/py.typed
-drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-04-01 19:28:09.084426 eth-typing-4.1.0/eth_typing.egg-info/
--rw-r--r--   0 pacrob    (1000) pacrob    (1000)     5005 2024-04-01 19:28:08.000000 eth-typing-4.1.0/eth_typing.egg-info/PKG-INFO
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      500 2024-04-01 19:28:09.000000 eth-typing-4.1.0/eth_typing.egg-info/SOURCES.txt
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)        1 2024-04-01 19:28:08.000000 eth-typing-4.1.0/eth_typing.egg-info/dependency_links.txt
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)        1 2024-03-25 21:51:21.000000 eth-typing-4.1.0/eth_typing.egg-info/not-zip-safe
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      284 2024-04-01 19:28:08.000000 eth-typing-4.1.0/eth_typing.egg-info/requires.txt
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)       11 2024-04-01 19:28:08.000000 eth-typing-4.1.0/eth_typing.egg-info/top_level.txt
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     3459 2024-04-01 18:23:03.000000 eth-typing-4.1.0/pyproject.toml
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)       38 2024-04-01 19:28:09.088426 eth-typing-4.1.0/setup.cfg
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1944 2024-04-01 19:27:50.000000 eth-typing-4.1.0/setup.py
-drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-04-01 19:28:09.084426 eth-typing-4.1.0/tests/
-drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-04-01 19:28:09.084426 eth-typing-4.1.0/tests/core/
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      105 2024-03-25 21:51:21.000000 eth-typing-4.1.0/tests/core/test_import_and_version.py
+drwxr-xr-x   0 reedsa     (501) staff       (20)        0 2024-04-15 20:35:39.526535 eth_typing-4.2.0/
+-rw-r--r--   0 reedsa     (501) staff       (20)     1095 2023-09-28 17:35:29.000000 eth_typing-4.2.0/LICENSE
+-rw-r--r--   0 reedsa     (501) staff       (20)      168 2023-08-18 16:16:13.000000 eth_typing-4.2.0/MANIFEST.in
+-rw-r--r--   0 reedsa     (501) staff       (20)     5005 2024-04-15 20:35:39.524356 eth_typing-4.2.0/PKG-INFO
+-rw-r--r--   0 reedsa     (501) staff       (20)     3285 2024-04-08 18:59:39.000000 eth_typing-4.2.0/README.md
+drwxr-xr-x   0 reedsa     (501) staff       (20)        0 2024-04-15 20:35:39.475228 eth_typing-4.2.0/eth_typing/
+-rw-r--r--   0 reedsa     (501) staff       (20)     1389 2024-04-15 20:26:59.000000 eth_typing-4.2.0/eth_typing/__init__.py
+-rw-r--r--   0 reedsa     (501) staff       (20)     4035 2024-04-15 20:26:59.000000 eth_typing-4.2.0/eth_typing/abi.py
+-rw-r--r--   0 reedsa     (501) staff       (20)      191 2023-09-28 17:31:13.000000 eth_typing-4.2.0/eth_typing/bls.py
+-rw-r--r--   0 reedsa     (501) staff       (20)       71 2024-04-09 21:54:01.000000 eth_typing-4.2.0/eth_typing/discovery.py
+-rw-r--r--   0 reedsa     (501) staff       (20)      117 2023-09-28 17:31:13.000000 eth_typing-4.2.0/eth_typing/encoding.py
+-rw-r--r--   0 reedsa     (501) staff       (20)      458 2023-09-28 17:31:13.000000 eth_typing-4.2.0/eth_typing/enums.py
+-rw-r--r--   0 reedsa     (501) staff       (20)      546 2024-04-09 18:21:17.000000 eth_typing-4.2.0/eth_typing/evm.py
+-rw-r--r--   0 reedsa     (501) staff       (20)      320 2024-04-15 20:26:59.000000 eth_typing-4.2.0/eth_typing/exceptions.py
+-rw-r--r--   0 reedsa     (501) staff       (20)    20948 2024-04-15 20:26:59.000000 eth_typing-4.2.0/eth_typing/networks.py
+-rw-r--r--   0 reedsa     (501) staff       (20)        0 2023-09-28 17:31:13.000000 eth_typing-4.2.0/eth_typing/py.typed
+drwxr-xr-x   0 reedsa     (501) staff       (20)        0 2024-04-15 20:35:39.481551 eth_typing-4.2.0/eth_typing.egg-info/
+-rw-r--r--   0 reedsa     (501) staff       (20)     5005 2024-04-15 20:35:38.000000 eth_typing-4.2.0/eth_typing.egg-info/PKG-INFO
+-rw-r--r--   0 reedsa     (501) staff       (20)      505 2024-04-15 20:35:39.000000 eth_typing-4.2.0/eth_typing.egg-info/SOURCES.txt
+-rw-r--r--   0 reedsa     (501) staff       (20)        1 2024-04-15 20:35:38.000000 eth_typing-4.2.0/eth_typing.egg-info/dependency_links.txt
+-rw-r--r--   0 reedsa     (501) staff       (20)        1 2023-10-19 21:43:55.000000 eth_typing-4.2.0/eth_typing.egg-info/not-zip-safe
+-rw-r--r--   0 reedsa     (501) staff       (20)      284 2024-04-15 20:35:38.000000 eth_typing-4.2.0/eth_typing.egg-info/requires.txt
+-rw-r--r--   0 reedsa     (501) staff       (20)       11 2024-04-15 20:35:38.000000 eth_typing-4.2.0/eth_typing.egg-info/top_level.txt
+-rw-r--r--   0 reedsa     (501) staff       (20)     3459 2024-04-08 18:59:39.000000 eth_typing-4.2.0/pyproject.toml
+-rw-r--r--   0 reedsa     (501) staff       (20)       38 2024-04-15 20:35:39.526720 eth_typing-4.2.0/setup.cfg
+-rw-r--r--   0 reedsa     (501) staff       (20)     1944 2024-04-15 20:35:27.000000 eth_typing-4.2.0/setup.py
+drwxr-xr-x   0 reedsa     (501) staff       (20)        0 2024-04-15 20:35:39.327294 eth_typing-4.2.0/tests/
+drwxr-xr-x   0 reedsa     (501) staff       (20)        0 2024-04-15 20:35:39.480757 eth_typing-4.2.0/tests/core/
+-rw-r--r--   0 reedsa     (501) staff       (20)      105 2024-04-08 18:59:39.000000 eth_typing-4.2.0/tests/core/test_import_and_version.py
```

### Comparing `eth-typing-4.1.0/LICENSE` & `eth_typing-4.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `eth-typing-4.1.0/PKG-INFO` & `eth_typing-4.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eth-typing
-Version: 4.1.0
+Version: 4.2.0
 Summary: eth-typing: Common type annotations for ethereum python packages
 Home-page: https://github.com/ethereum/eth-typing
 Author: The Ethereum Foundation
 Author-email: snakecharmers@ethereum.org
 License: MIT
 Keywords: ethereum
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `eth-typing-4.1.0/README.md` & `eth_typing-4.2.0/README.md`

 * *Files identical despite different names*

### Comparing `eth-typing-4.1.0/eth_typing/evm.py` & `eth_typing-4.2.0/eth_typing/evm.py`

 * *Files identical despite different names*

### Comparing `eth-typing-4.1.0/eth_typing/networks.py` & `eth_typing-4.2.0/eth_typing/networks.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 from enum import (
     IntEnum,
 )
+from typing import (
+    NewType,
+)
+
+URI = NewType("URI", str)
+"""Any string that represents a URI."""
 
 
 class ChainId(IntEnum):
     ETH = 1
     EXP = 2
     ROP = 3
     RIN = 4
```

### Comparing `eth-typing-4.1.0/eth_typing.egg-info/PKG-INFO` & `eth_typing-4.2.0/eth_typing.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eth-typing
-Version: 4.1.0
+Version: 4.2.0
 Summary: eth-typing: Common type annotations for ethereum python packages
 Home-page: https://github.com/ethereum/eth-typing
 Author: The Ethereum Foundation
 Author-email: snakecharmers@ethereum.org
 License: MIT
 Keywords: ethereum
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `eth-typing-4.1.0/pyproject.toml` & `eth_typing-4.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `eth-typing-4.1.0/setup.py` & `eth_typing-4.2.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 with open("./README.md") as readme:
     long_description = readme.read()
 
 
 setup(
     name="eth-typing",
     # *IMPORTANT*: Don't manually change the version here. Use `make bump`, as described in readme
-    version="4.1.0",
+    version="4.2.0",
     description="""eth-typing: Common type annotations for ethereum python packages""",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="The Ethereum Foundation",
     author_email="snakecharmers@ethereum.org",
     url="https://github.com/ethereum/eth-typing",
     include_package_data=True,
```

