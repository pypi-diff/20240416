# Comparing `tmp/atxm-0.2.1.tar.gz` & `tmp/atxm-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atxm-0.2.1.tar", last modified: Thu Feb 15 23:17:26 2024, max compression
+gzip compressed data, was "atxm-0.3.0.tar", last modified: Tue Apr 16 13:02:38 2024, max compression
```

## Comparing `atxm-0.2.1.tar` & `atxm-0.3.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 23:17:26.017011 atxm-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-02-15 23:17:17.000000 atxm-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-02-15 23:17:17.000000 atxm-0.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    55796 2024-02-15 23:17:26.017011 atxm-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2632 2024-02-15 23:17:17.000000 atxm-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 23:17:25.997011 atxm-0.2.1/atxm/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-02-15 23:17:17.000000 atxm-0.2.1/atxm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-02-15 23:17:17.000000 atxm-0.2.1/atxm/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-02-15 23:17:17.000000 atxm-0.2.1/atxm/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)    14238 2024-02-15 23:17:17.000000 atxm-0.2.1/atxm/machine.py
--rw-r--r--   0 runner    (1001) docker     (127)     2908 2024-02-15 23:17:17.000000 atxm-0.2.1/atxm/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-02-15 23:17:17.000000 atxm-0.2.1/atxm/state.py
--rw-r--r--   0 runner    (1001) docker     (127)     6742 2024-02-15 23:17:17.000000 atxm-0.2.1/atxm/strategies.py
--rw-r--r--   0 runner    (1001) docker     (127)     5312 2024-02-15 23:17:17.000000 atxm-0.2.1/atxm/tx.py
--rw-r--r--   0 runner    (1001) docker     (127)     3581 2024-02-15 23:17:17.000000 atxm-0.2.1/atxm/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 23:17:25.997011 atxm-0.2.1/atxm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    55796 2024-02-15 23:17:25.000000 atxm-0.2.1/atxm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-02-15 23:17:25.000000 atxm-0.2.1/atxm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-15 23:17:25.000000 atxm-0.2.1/atxm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4750 2024-02-15 23:17:25.000000 atxm-0.2.1/atxm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-15 23:17:25.000000 atxm-0.2.1/atxm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5284 2024-02-15 23:17:17.000000 atxm-0.2.1/dev-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-02-15 23:17:17.000000 atxm-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-02-15 23:17:17.000000 atxm-0.2.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-15 23:17:26.017011 atxm-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:02:38.914019 atxm-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-04-16 13:02:29.000000 atxm-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-16 13:02:29.000000 atxm-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    56313 2024-04-16 13:02:38.914019 atxm-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2694 2024-04-16 13:02:29.000000 atxm-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:02:38.894019 atxm-0.3.0/atxm/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-16 13:02:29.000000 atxm-0.3.0/atxm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-16 13:02:29.000000 atxm-0.3.0/atxm/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-16 13:02:29.000000 atxm-0.3.0/atxm/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18174 2024-04-16 13:02:29.000000 atxm-0.3.0/atxm/machine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2154 2024-04-16 13:02:29.000000 atxm-0.3.0/atxm/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10632 2024-04-16 13:02:29.000000 atxm-0.3.0/atxm/strategies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9064 2024-04-16 13:02:29.000000 atxm-0.3.0/atxm/tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7129 2024-04-16 13:02:29.000000 atxm-0.3.0/atxm/tx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5739 2024-04-16 13:02:29.000000 atxm-0.3.0/atxm/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:02:38.894019 atxm-0.3.0/atxm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    56313 2024-04-16 13:02:38.000000 atxm-0.3.0/atxm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-16 13:02:38.000000 atxm-0.3.0/atxm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 13:02:38.000000 atxm-0.3.0/atxm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4642 2024-04-16 13:02:38.000000 atxm-0.3.0/atxm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-16 13:02:38.000000 atxm-0.3.0/atxm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5503 2024-04-16 13:02:29.000000 atxm-0.3.0/dev-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-04-16 13:02:29.000000 atxm-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-04-16 13:02:29.000000 atxm-0.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 13:02:38.914019 atxm-0.3.0/setup.cfg
```

### Comparing `atxm-0.2.1/LICENSE` & `atxm-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `atxm-0.2.1/PKG-INFO` & `atxm-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atxm
-Version: 0.2.1
+Version: 0.3.0
 Summary: Automatic Transaction Machine (ATxM) for Ethereum
 Author-email: NuCypher <devs@nucypher.com>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -679,195 +679,204 @@
 Classifier: Natural Language :: English
 Classifier: Typing :: Typed
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: aiohttp==3.9.3; python_version >= "3.8"
+Requires-Dist: aiohttp==3.9.4rc0; python_version >= "3.8"
 Requires-Dist: aiosignal==1.3.1; python_version >= "3.7"
 Requires-Dist: attrs==23.2.0; python_version >= "3.7"
 Requires-Dist: automat==22.10.0
 Requires-Dist: bitarray==2.9.2
 Requires-Dist: certifi==2024.2.2; python_version >= "3.6"
 Requires-Dist: charset-normalizer==3.3.2; python_full_version >= "3.7.0"
 Requires-Dist: constantly==23.10.4; python_version >= "3.8"
 Requires-Dist: cytoolz==0.12.3; implementation_name == "cpython"
 Requires-Dist: eth-abi==4.2.1; python_version < "4" and python_full_version >= "3.7.2"
-Requires-Dist: eth-account==0.8.0; python_version >= "3.6" and python_version < "4"
-Requires-Dist: eth-hash[pycryptodome]==0.6.0; python_version >= "3.8" and python_version < "4"
-Requires-Dist: eth-keyfile==0.6.1
+Requires-Dist: eth-account==0.10.0; python_version >= "3.7" and python_version < "4"
+Requires-Dist: eth-hash[pycryptodome]==0.7.0; python_version >= "3.8" and python_version < "4"
+Requires-Dist: eth-keyfile==0.8.0; python_version >= "3.8" and python_version < "4"
 Requires-Dist: eth-keys==0.4.0
-Requires-Dist: eth-rlp==0.3.0; python_version >= "3.7" and python_version < "4"
+Requires-Dist: eth-rlp==1.0.1; python_version >= "3.8" and python_version < "4"
 Requires-Dist: eth-typing==3.5.2; python_version < "4" and python_full_version >= "3.7.2"
 Requires-Dist: eth-utils==2.3.1; python_version >= "3.7" and python_version < "4"
 Requires-Dist: frozenlist==1.4.1; python_version >= "3.8"
 Requires-Dist: hexbytes==0.3.1; python_version >= "3.7" and python_version < "4"
 Requires-Dist: hyperlink==21.0.0
-Requires-Dist: idna==3.6; python_version >= "3.5"
+Requires-Dist: idna==3.7; python_version >= "3.5"
 Requires-Dist: incremental==22.10.0
 Requires-Dist: jsonschema==4.21.1; python_version >= "3.8"
 Requires-Dist: jsonschema-specifications==2023.12.1; python_version >= "3.8"
 Requires-Dist: lru-dict==1.2.0
 Requires-Dist: multidict==6.0.5; python_version >= "3.7"
 Requires-Dist: parsimonious==0.9.0
-Requires-Dist: protobuf==5.26.0rc2; python_version >= "3.8"
+Requires-Dist: protobuf==5.26.1; python_version >= "3.8"
 Requires-Dist: pycryptodome==3.20.0
+Requires-Dist: python-statemachine==2.1.2; python_version < "3.13" and python_version >= "3.7"
 Requires-Dist: pyunormalize==15.1.0; python_version >= "3.6"
-Requires-Dist: referencing==0.33.0; python_version >= "3.8"
+Requires-Dist: referencing==0.34.0; python_version >= "3.8"
 Requires-Dist: regex==2023.12.25; python_version >= "3.7"
 Requires-Dist: requests==2.31.0; python_version >= "3.7"
 Requires-Dist: rlp==3.0.0
 Requires-Dist: rpds-py==0.18.0; python_version >= "3.8"
-Requires-Dist: setuptools==69.1.0; python_version >= "3.8"
+Requires-Dist: setuptools==69.2.0; python_version >= "3.8"
 Requires-Dist: six==1.16.0; python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2, 3.3"
 Requires-Dist: toolz==0.12.1; python_version >= "3.7"
-Requires-Dist: twisted==23.10.0; python_full_version >= "3.8.0"
-Requires-Dist: typing-extensions==4.9.0; python_version >= "3.8"
-Requires-Dist: urllib3==1.26.18; python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2, 3.3, 3.4, 3.5"
+Requires-Dist: twisted==24.3.0; python_full_version >= "3.8.0"
+Requires-Dist: typing-extensions==4.11.0; python_version >= "3.8"
+Requires-Dist: urllib3==2.2.0; python_version >= "3.8"
 Requires-Dist: web3==6.15.1; python_full_version >= "3.7.2"
 Requires-Dist: websockets==12.0; python_version >= "3.8"
 Requires-Dist: yarl==1.9.4; python_version >= "3.7"
-Requires-Dist: zope-interface==6.1; python_version >= "3.7"
+Requires-Dist: zope-interface==6.2; python_version >= "3.7"
 Provides-Extra: test
-Requires-Dist: aiohttp==3.9.3; python_version >= "3.8" and extra == "test"
+Requires-Dist: aiohttp==3.9.4rc0; python_version >= "3.8" and extra == "test"
 Requires-Dist: aiosignal==1.3.1; python_version >= "3.7" and extra == "test"
 Requires-Dist: annotated-types==0.6.0; python_version >= "3.8" and extra == "test"
 Requires-Dist: asttokens==2.4.1; extra == "test"
 Requires-Dist: attrs==23.2.0; python_version >= "3.7" and extra == "test"
 Requires-Dist: base58==1.0.3; extra == "test"
 Requires-Dist: bitarray==2.9.2; extra == "test"
-Requires-Dist: black==24.2.0; python_version >= "3.8" and extra == "test"
+Requires-Dist: black==24.3.0; python_version >= "3.8" and extra == "test"
 Requires-Dist: cached-property==1.5.2; extra == "test"
 Requires-Dist: certifi==2024.2.2; python_version >= "3.6" and extra == "test"
 Requires-Dist: cffi==1.16.0; python_version >= "3.8" and extra == "test"
 Requires-Dist: cfgv==3.4.0; python_version >= "3.8" and extra == "test"
 Requires-Dist: charset-normalizer==3.3.2; python_full_version >= "3.7.0" and extra == "test"
 Requires-Dist: click==8.1.7; python_version >= "3.7" and extra == "test"
-Requires-Dist: commonmark==0.9.1; extra == "test"
-Requires-Dist: cryptography==43.0.0.dev1; extra == "test"
+Requires-Dist: cryptography==42.0.5; extra == "test"
 Requires-Dist: cytoolz==0.12.3; implementation_name == "cpython" and extra == "test"
 Requires-Dist: dataclassy==0.11.1; python_version >= "3.6" and extra == "test"
 Requires-Dist: decorator==5.1.1; python_version >= "3.5" and extra == "test"
 Requires-Dist: deprecated==1.2.14; (python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2, 3.3") and extra == "test"
 Requires-Dist: distlib==0.3.8; extra == "test"
-Requires-Dist: eip712==0.2.2; (python_version >= "3.8" and python_version < "4") and extra == "test"
+Requires-Dist: eip712==0.2.5; (python_version >= "3.8" and python_version < "4") and extra == "test"
 Requires-Dist: eth-abi==4.2.1; (python_full_version >= "3.7.2" and python_version < "4") and extra == "test"
-Requires-Dist: eth-account==0.8.0; (python_version >= "3.6" and python_version < "4") and extra == "test"
-Requires-Dist: eth-ape==0.6.27; (python_version >= "3.8" and python_version < "4") and extra == "test"
+Requires-Dist: eth-account==0.10.0; (python_version >= "3.7" and python_version < "4") and extra == "test"
+Requires-Dist: eth-ape==0.7.13; (python_version >= "3.8" and python_version < "4") and extra == "test"
 Requires-Dist: eth-bloom==3.0.0; (python_version >= "3.8" and python_version < "4") and extra == "test"
-Requires-Dist: eth-hash[pycryptodome]==0.6.0; (python_version >= "3.8" and python_version < "4") and extra == "test"
-Requires-Dist: eth-keyfile==0.6.1; extra == "test"
+Requires-Dist: eth-hash[pycryptodome]==0.7.0; (python_version >= "3.8" and python_version < "4") and extra == "test"
+Requires-Dist: eth-keyfile==0.8.0; (python_version >= "3.8" and python_version < "4") and extra == "test"
 Requires-Dist: eth-keys==0.4.0; extra == "test"
-Requires-Dist: eth-pydantic-types==0.1.0a5; (python_version >= "3.8" and python_version < "4") and extra == "test"
-Requires-Dist: eth-rlp==0.3.0; (python_version >= "3.7" and python_version < "4") and extra == "test"
+Requires-Dist: eth-pydantic-types==0.1.0; (python_version >= "3.8" and python_version < "4") and extra == "test"
+Requires-Dist: eth-rlp==1.0.1; (python_version >= "3.8" and python_version < "4") and extra == "test"
 Requires-Dist: eth-tester[py-evm]==0.9.1b2; extra == "test"
 Requires-Dist: eth-typing==3.5.2; (python_full_version >= "3.7.2" and python_version < "4") and extra == "test"
 Requires-Dist: eth-utils==2.3.1; (python_version >= "3.7" and python_version < "4") and extra == "test"
-Requires-Dist: ethpm-types==0.5.11; (python_version >= "3.8" and python_version < "4") and extra == "test"
-Requires-Dist: evm-trace==0.1.2; (python_version >= "3.8" and python_version < "4") and extra == "test"
+Requires-Dist: ethpm-types==0.6.9; (python_version >= "3.8" and python_version < "4") and extra == "test"
+Requires-Dist: evm-trace==0.1.3; (python_version >= "3.8" and python_version < "4") and extra == "test"
+Requires-Dist: evmchains==0.0.5; python_version >= "3.8" and extra == "test"
 Requires-Dist: executing==2.0.1; python_version >= "3.5" and extra == "test"
-Requires-Dist: filelock==3.13.1; python_version >= "3.8" and extra == "test"
+Requires-Dist: filelock==3.13.4; python_version >= "3.8" and extra == "test"
 Requires-Dist: frozenlist==1.4.1; python_version >= "3.8" and extra == "test"
 Requires-Dist: greenlet==3.0.3; python_version >= "3.7" and extra == "test"
 Requires-Dist: hexbytes==0.3.1; (python_version >= "3.7" and python_version < "4") and extra == "test"
-Requires-Dist: identify==2.5.34; python_version >= "3.8" and extra == "test"
-Requires-Dist: idna==3.6; python_version >= "3.5" and extra == "test"
+Requires-Dist: identify==2.5.35; python_version >= "3.8" and extra == "test"
+Requires-Dist: idna==3.7; python_version >= "3.5" and extra == "test"
 Requires-Dist: ijson==3.2.3; extra == "test"
-Requires-Dist: importlib-metadata==7.0.1; python_version >= "3.8" and extra == "test"
+Requires-Dist: importlib-metadata==7.1.0; python_version >= "3.8" and extra == "test"
 Requires-Dist: iniconfig==2.0.0; python_version >= "3.7" and extra == "test"
-Requires-Dist: ipython==8.21.0; python_version >= "3.10" and extra == "test"
+Requires-Dist: ipython==8.23.0; python_version >= "3.10" and extra == "test"
 Requires-Dist: jedi==0.19.1; python_version >= "3.6" and extra == "test"
 Requires-Dist: jsonschema==4.21.1; python_version >= "3.8" and extra == "test"
 Requires-Dist: jsonschema-specifications==2023.12.1; python_version >= "3.8" and extra == "test"
 Requires-Dist: lazyasd==0.1.4; extra == "test"
 Requires-Dist: lru-dict==1.2.0; extra == "test"
+Requires-Dist: markdown-it-py==3.0.0; python_version >= "3.8" and extra == "test"
 Requires-Dist: matplotlib-inline==0.1.6; python_version >= "3.5" and extra == "test"
+Requires-Dist: mdurl==0.1.2; python_version >= "3.7" and extra == "test"
 Requires-Dist: morphys==1.0; extra == "test"
 Requires-Dist: msgspec==0.18.6; python_version >= "3.8" and extra == "test"
 Requires-Dist: multidict==6.0.5; python_version >= "3.7" and extra == "test"
 Requires-Dist: mypy-extensions==1.0.0; python_version >= "3.5" and extra == "test"
 Requires-Dist: nodeenv==1.8.0; (python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2, 3.3, 3.4, 3.5, 3.6") and extra == "test"
 Requires-Dist: numpy==1.26.4; python_version >= "3.10" and extra == "test"
 Requires-Dist: packaging==23.2; python_version >= "3.7" and extra == "test"
 Requires-Dist: pandas==1.5.3; python_version >= "3.8" and extra == "test"
 Requires-Dist: parsimonious==0.9.0; extra == "test"
-Requires-Dist: parso==0.8.3; python_version >= "3.6" and extra == "test"
+Requires-Dist: parso==0.8.4; python_version >= "3.6" and extra == "test"
 Requires-Dist: pathspec==0.12.1; python_version >= "3.8" and extra == "test"
-Requires-Dist: pexpect==4.9.0; sys_platform != "win32" and extra == "test"
+Requires-Dist: pexpect==4.9.0; (sys_platform != "win32" and sys_platform != "emscripten") and extra == "test"
 Requires-Dist: platformdirs==4.2.0; python_version >= "3.8" and extra == "test"
 Requires-Dist: pluggy==1.4.0; python_version >= "3.8" and extra == "test"
-Requires-Dist: pre-commit==3.6.1; python_version >= "3.9" and extra == "test"
+Requires-Dist: pre-commit==3.7.0; python_version >= "3.9" and extra == "test"
 Requires-Dist: prompt-toolkit==3.0.43; python_full_version >= "3.7.0" and extra == "test"
-Requires-Dist: protobuf==5.26.0rc2; python_version >= "3.8" and extra == "test"
+Requires-Dist: protobuf==5.26.1; python_version >= "3.8" and extra == "test"
 Requires-Dist: ptyprocess==0.7.0; extra == "test"
 Requires-Dist: pure-eval==0.2.2; extra == "test"
 Requires-Dist: py-cid==0.3.0; extra == "test"
 Requires-Dist: py-ecc==6.0.0; (python_version >= "3.6" and python_version < "4") and extra == "test"
 Requires-Dist: py-evm==0.7.0a4; extra == "test"
-Requires-Dist: py-geth==3.14.0; (python_version >= "3.7" and python_version < "4") and extra == "test"
+Requires-Dist: py-geth==4.4.0; (python_version >= "3.8" and python_version < "4") and extra == "test"
 Requires-Dist: py-multibase==1.0.3; extra == "test"
 Requires-Dist: py-multicodec==0.2.1; extra == "test"
 Requires-Dist: py-multihash==0.2.3; extra == "test"
-Requires-Dist: pycparser==2.21; extra == "test"
+Requires-Dist: pycparser==2.22; python_version >= "3.8" and extra == "test"
 Requires-Dist: pycryptodome==3.20.0; extra == "test"
-Requires-Dist: pydantic==2.6.1; python_version >= "3.8" and extra == "test"
-Requires-Dist: pydantic-core==2.16.2; python_version >= "3.8" and extra == "test"
+Requires-Dist: pydantic==2.5.3; python_version >= "3.7" and extra == "test"
+Requires-Dist: pydantic-core==2.14.6; python_version >= "3.7" and extra == "test"
+Requires-Dist: pydantic-settings==2.2.1; python_version >= "3.8" and extra == "test"
 Requires-Dist: pyethash==0.1.27; extra == "test"
 Requires-Dist: pygithub==1.59.1; python_version >= "3.7" and extra == "test"
 Requires-Dist: pygments==2.17.2; python_version >= "3.7" and extra == "test"
 Requires-Dist: pyjwt[crypto]==2.8.0; python_version >= "3.7" and extra == "test"
 Requires-Dist: pynacl==1.5.0; python_version >= "3.6" and extra == "test"
 Requires-Dist: pytest==7.4.4; python_version >= "3.7" and extra == "test"
-Requires-Dist: pytest-mock==3.12.0; python_version >= "3.8" and extra == "test"
-Requires-Dist: pytest-twisted==1.14.0; (python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2, 3.3, 3.4") and extra == "test"
+Requires-Dist: pytest-mock==3.14.0; python_version >= "3.8" and extra == "test"
+Requires-Dist: pytest-twisted==1.14.1; (python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2, 3.3, 3.4") and extra == "test"
 Requires-Dist: python-baseconv==1.2.2; extra == "test"
-Requires-Dist: python-dateutil==2.8.2; (python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2") and extra == "test"
+Requires-Dist: python-dateutil==2.9.0.post0; (python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2") and extra == "test"
+Requires-Dist: python-dotenv==1.0.1; python_version >= "3.8" and extra == "test"
 Requires-Dist: pytz==2024.1; extra == "test"
 Requires-Dist: pyunormalize==15.1.0; python_version >= "3.6" and extra == "test"
 Requires-Dist: pyyaml==6.0.1; python_version >= "3.6" and extra == "test"
-Requires-Dist: referencing==0.33.0; python_version >= "3.8" and extra == "test"
+Requires-Dist: referencing==0.34.0; python_version >= "3.8" and extra == "test"
 Requires-Dist: regex==2023.12.25; python_version >= "3.7" and extra == "test"
 Requires-Dist: requests==2.31.0; python_version >= "3.7" and extra == "test"
-Requires-Dist: rich==12.6.0; (python_full_version >= "3.6.3" and python_full_version < "4.0.0") and extra == "test"
+Requires-Dist: rich==13.7.1; python_full_version >= "3.7.0" and extra == "test"
 Requires-Dist: rlp==3.0.0; extra == "test"
 Requires-Dist: rpds-py==0.18.0; python_version >= "3.8" and extra == "test"
-Requires-Dist: ruff==0.2.1; python_version >= "3.7" and extra == "test"
+Requires-Dist: ruff==0.3.6; python_version >= "3.7" and extra == "test"
 Requires-Dist: safe-pysha3==1.0.4; extra == "test"
 Requires-Dist: semantic-version==2.10.0; python_version >= "2.7" and extra == "test"
-Requires-Dist: setuptools==69.1.0; python_version >= "3.8" and extra == "test"
+Requires-Dist: setuptools==69.2.0; python_version >= "3.8" and extra == "test"
 Requires-Dist: six==1.16.0; (python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2") and extra == "test"
 Requires-Dist: sortedcontainers==2.4.0; extra == "test"
-Requires-Dist: sqlalchemy==2.0.27; python_version >= "3.7" and extra == "test"
+Requires-Dist: sqlalchemy==2.0.29; python_version >= "3.7" and extra == "test"
 Requires-Dist: stack-data==0.6.3; extra == "test"
 Requires-Dist: toolz==0.12.1; python_version >= "3.7" and extra == "test"
 Requires-Dist: tqdm==4.66.2; python_version >= "3.7" and extra == "test"
-Requires-Dist: traitlets==5.14.1; python_version >= "3.8" and extra == "test"
+Requires-Dist: traitlets==5.14.2; python_version >= "3.8" and extra == "test"
 Requires-Dist: trie==2.2.0; (python_version >= "3.7" and python_version < "4") and extra == "test"
-Requires-Dist: typing-extensions==4.9.0; python_version >= "3.8" and extra == "test"
-Requires-Dist: urllib3==1.26.18; (python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2, 3.3, 3.4, 3.5") and extra == "test"
+Requires-Dist: typing-extensions==4.11.0; python_version >= "3.8" and extra == "test"
+Requires-Dist: urllib3==2.2.0; python_version >= "3.8" and extra == "test"
 Requires-Dist: varint==1.0.2; extra == "test"
-Requires-Dist: virtualenv==20.25.0; python_version >= "3.7" and extra == "test"
+Requires-Dist: virtualenv==20.25.1; python_version >= "3.7" and extra == "test"
 Requires-Dist: watchdog==3.0.0; python_version >= "3.7" and extra == "test"
 Requires-Dist: wcwidth==0.2.13; extra == "test"
 Requires-Dist: web3==6.15.1; python_full_version >= "3.7.2" and extra == "test"
 Requires-Dist: websockets==12.0; python_version >= "3.8" and extra == "test"
 Requires-Dist: wrapt==1.16.0; python_version >= "3.6" and extra == "test"
 Requires-Dist: yarl==1.9.4; python_version >= "3.7" and extra == "test"
-Requires-Dist: zipp==3.17.0; python_version >= "3.8" and extra == "test"
+Requires-Dist: zipp==3.18.1; python_version >= "3.8" and extra == "test"
 
 Automatic Tx Machine 🏧
 ========================
 
 [![Tests](https://github.com/nucypher/ATxM/actions/workflows/pytest.yml/badge.svg)](https://github.com/nucypher/ATxM/actions/workflows/pytest.yml)
 
 An async EVM transaction retry machine.
 Programmatically queue, broadcast, and retrying (speedup) transactions.
 Transactions are queued and broadcasted in a first-in-first-out (FIFO) order.
 
+The machine is designed to be used in a long-running process, like a server.
+
+[![Diagram](./diagram.png)](./diagram.png)
+
 ### Installation
 
 ```bash
 pip install atxm
 ```
 
 ### Usage
@@ -918,15 +927,14 @@
 
 ##### Lifecycle Hooks 
 
 Hooks are fired in a dedicated thread for lifecycle events.
 
 - `on_broadcast`: When a transaction is broadcasted.
 - `on_finalized`: When a transaction is finalized.
-- `on_pause`: When a transaction is halted by the strategy.
 - `on_fault`: When a transaction reverted or another error occurred.
 
 
 ##### Crash-Tolerance
 
 Internal state is written to a file to help recover from crashes
 and restarts. Internally caches LocalAccount instances in-memory which in
```

### Comparing `atxm-0.2.1/README.md` & `atxm-0.3.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -3,14 +3,18 @@
 
 [![Tests](https://github.com/nucypher/ATxM/actions/workflows/pytest.yml/badge.svg)](https://github.com/nucypher/ATxM/actions/workflows/pytest.yml)
 
 An async EVM transaction retry machine.
 Programmatically queue, broadcast, and retrying (speedup) transactions.
 Transactions are queued and broadcasted in a first-in-first-out (FIFO) order.
 
+The machine is designed to be used in a long-running process, like a server.
+
+[![Diagram](./diagram.png)](./diagram.png)
+
 ### Installation
 
 ```bash
 pip install atxm
 ```
 
 ### Usage
@@ -61,15 +65,14 @@
 
 ##### Lifecycle Hooks 
 
 Hooks are fired in a dedicated thread for lifecycle events.
 
 - `on_broadcast`: When a transaction is broadcasted.
 - `on_finalized`: When a transaction is finalized.
-- `on_pause`: When a transaction is halted by the strategy.
 - `on_fault`: When a transaction reverted or another error occurred.
 
 
 ##### Crash-Tolerance
 
 Internal state is written to a file to help recover from crashes
 and restarts. Internally caches LocalAccount instances in-memory which in
```

### Comparing `atxm-0.2.1/atxm/exceptions.py` & `atxm-0.3.0/atxm/exceptions.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,56 +1,38 @@
 from enum import Enum
 
-from web3.types import RPCError
+from web3.types import PendingTx
 
 
-class Faults(Enum):
+class Fault(Enum):
     """
     Fault codes for transaction processing.
     These are alternate states that a transaction can enter
     other than "finalized".
     """
 
     # Strategy has been running for too long
     TIMEOUT = "timeout"
 
-    # Transaction has been capped and subsequently timed out
-    PAUSE = "pause"
-
-    # Transaction reverted
-    REVERT = "revert"
-
     # Something went wrong
     ERROR = "error"
 
-    # ...
-    INSUFFICIENT_FUNDS = "insufficient_funds"
-
-
-class TransactionFinalized(Exception):
-    """raised when a transaction has been included in a block"""
-
 
-class InsufficientFunds(RPCError):
+class InsufficientFunds(Exception):
     """raised when a transaction exceeds the spending cap"""
 
 
-class Wait(Exception):
-    """
-    Raised when a strategy exceeds a limitation.
-    Used to mark a pending transaction as "wait, don't retry".
-    """
+class RPCException(Exception):
+    def __init__(self, error_code: int, error_message: str):
+        self.error_code = error_code
+        self.error_message = error_message
+        super().__init__(f"RPC Error [{error_code}]: {error_message}")
 
 
-class Fault(Exception):
-    """raised when a transaction has been faulted"""
+class TransactionFaulted(Exception):
+    """Raised when a transaction has been faulted."""
 
-    def __init__(self, tx, fault: Faults, clear: bool, message: str):
+    def __init__(self, tx: PendingTx, fault: Fault, message: str):
         self.tx = tx
         self.fault = fault
         self.message = message
-        self.clear = clear
         super().__init__(message)
-
-
-class TransactionReverted(Exception):
-    """raised when a transaction has been reverted"""
```

### Comparing `atxm-0.2.1/atxm/main.py` & `atxm-0.3.0/atxm/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from web3.types import TxParams
 
 from atxm.machine import _Machine
 from atxm.tx import (
     FinalizedTx,
     FutureTx,
     PendingTx,
-    AsyncTx,
 )
 
 
 class AutomaticTxMachine(_Machine):
     def start(self, now: bool = False) -> None:
         """Start the machine. if now is True, start immediately."""
         super()._start(now=now)
@@ -26,55 +25,35 @@
     def running(self) -> bool:
         """Return True if the machine is running."""
         return bool(self._task.running)
 
     @property
     def paused(self) -> bool:
         """Return True if the machine is paused."""
-        return bool(self.__pause)
+        return bool(self._pause)
 
     @property
     def busy(self) -> bool:
         """Returns True if the machine is busy."""
         return super()._busy
 
     @property
     def queued(self) -> List[FutureTx]:
         """Return a list of queued transactions."""
-        return list(self._state.queue)
+        return list(self._tx_tracker.queue)
 
     @property
     def pending(self) -> PendingTx:
         """Return the active transaction if there is one."""
-        return copy(self._state.pending or None)
+        return copy(self._tx_tracker.pending or None)
 
     @property
     def finalized(self) -> Set[FinalizedTx]:
         """Return a set of finalized transactions."""
-        return set(self._state.finalized)
-
-    @property
-    def faults(self) -> List[AsyncTx]:
-        """Return a set of faulted transactions."""
-        return list(self._state.faulty)
-
-    def queue_transaction(
-        self, params: TxParams, signer: LocalAccount, *args, **kwargs
-    ) -> FutureTx:
-        """
-        Queue a new transaction for broadcast and subsequent tracking.
-        Optionally provide a dictionary of additional string data
-        to log during the transaction's lifecycle for identification.
-        """
-        if signer.address not in self.signers:
-            self.signers[signer.address] = signer
-        tx = self._state._queue(_from=signer.address, params=params, *args, **kwargs)
-        if not self._task.running:
-            self._wake()
-        return tx
+        return set(self._tx_tracker.finalized)
 
     def queue_transactions(
         self, params: List[TxParams], signer: LocalAccount, *args, **kwargs
     ) -> List[FutureTx]:
         """
         Queue a list of transactions for broadcast and subsequent tracking.
```

### Comparing `atxm-0.2.1/atxm/state.py` & `atxm-0.3.0/atxm/tracker.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,45 +1,41 @@
 import json
 import time
 from collections import deque
 from copy import copy
 from json import JSONDecodeError
 from pathlib import Path
-from typing import Callable, Deque, Dict, Optional, Set, Tuple
+from typing import Callable, Deque, Dict, Optional, Set, Tuple, Union
 
-from eth_typing import ChecksumAddress
 from web3.types import TxParams, TxReceipt
 
-from atxm.exceptions import Faults
+from atxm.exceptions import InsufficientFunds, TransactionFaulted
 from atxm.logging import log
 from atxm.tx import (
     FinalizedTx,
     FutureTx,
     PendingTx,
     TxHash,
-    AsyncTx,
-    FaultyTx,
+    FaultedTx,
 )
 from atxm.utils import fire_hook
 
 
-class _State:
+class _TxTracker:
     """State management for transaction tracking."""
 
     _FILEPATH = ".txs.json"
     __COUNTER = 0  # id generator
-    __FAULT_CACHE_SIZE = 10
 
     def __init__(self, disk_cache: bool, filepath: Optional[Path] = None):
         self.__filepath = filepath or self._FILEPATH
 
         self.__queue: Deque[FutureTx] = deque()
         self.__active: Optional[PendingTx] = None
         self.finalized: Set[FinalizedTx] = set()
-        self.faulty: Deque[AsyncTx] = deque(maxlen=self.__FAULT_CACHE_SIZE)
 
         self.disk_cache = disk_cache
         if disk_cache:
             self.restore()
 
     def to_dict(self) -> Dict:
         """Serialize the state to a JSON string."""
@@ -52,15 +48,15 @@
     def commit(self) -> None:
         """Write the state to the cache file."""
         if not self.disk_cache:
             return
         with open(self.__filepath, "w+t") as file:
             data = json.dumps(self.to_dict())
             file.write(data)
-        log.debug(f"[state] wrote transaction cache file {self.__filepath}")
+        log.debug(f"[tracker] wrote transaction cache file {self.__filepath}")
 
     def restore(self) -> bool:
         """
         Restore the state from the cache file.
         Returns True if the cache file exists and was successfully
         restored with data.
         """
@@ -78,148 +74,202 @@
             data = dict()
         active = data.get("active", dict())
         queue = data.get("queue", list())
         final = data.get("finalized", list())
 
         # deserialize & restore
         self.__active = PendingTx.from_dict(active) if active else None
-        self.__queue.extend(FutureTx.from_dict(tx) for tx in queue)
+        self.__queue.extend([FutureTx.from_dict(tx) for tx in queue])
         self.finalized = {FinalizedTx.from_dict(tx) for tx in final}
         log.debug(
-            f"[state] restored {len(queue)} transactions from cache file {self.__filepath}"
+            f"[tracker] restored {len(queue)} transactions from cache file {self.__filepath}"
         )
 
         return bool(data)
 
     def __set_active(self, tx: PendingTx) -> None:
         """Update the active transaction (destructive operation)."""
         old = None
         if self.__active:
             old = self.__active.txhash
         self.__active = tx
         self.commit()
         if old:
             log.debug(
-                f"[state] updated active transaction {old.hex()} -> {tx.txhash.hex()}"
+                f"[tracker] updated active transaction {old.hex()} -> {tx.txhash.hex()}"
             )
             return
-        log.debug(f"[state] tracked active transaction {tx.txhash.hex()}")
+        log.debug(f"[tracker] tracked active transaction {tx.txhash.hex()}")
+
+    def __pop(self) -> FutureTx:
+        """Pop the next transaction from the queue."""
+        return self.__queue.popleft()
+
+    def update_active_after_successful_strategy_update(
+        self, tx: PendingTx
+    ) -> PendingTx:
+        if not self.__active:
+            raise RuntimeError("No active transaction to update")
+        if tx.id != self.__active.id:
+            raise RuntimeError(
+                f"Mismatch between active tx ({self.__active.id}) and provided tx ({tx.id})"
+            )
+
+        self.__active.txhash = tx.txhash
+        self.__active.params = tx.params
+        self.__active.last_updated = int(time.time())
+        self.__active.retries = 0  # reset retries to 0
+
+        return self.pending
+
+    def update_active_after_failed_strategy_update(self, tx: PendingTx):
+        if not self.__active:
+            raise RuntimeError("No active transaction to update")
+        if tx.id != self.__active.id:
+            raise RuntimeError(
+                f"Mismatch between active tx ({self.__active.id}) and provided tx ({tx.id})"
+            )
+        self.__active.retries += 1
+        # safety check
+        if tx is not self.__active:
+            tx.retries = self.__active.retries
 
     def morph(self, tx: FutureTx, txhash: TxHash) -> PendingTx:
         """
         Morphs a future transaction into a pending transaction.
         Uses polymorphism to transform the future transaction into a pending transaction.
         """
+        head_tx = self.head()
+        if tx.id != head_tx.id:
+            raise RuntimeError(
+                f"Mismatch between tx at the front of the queue ({head_tx.id}) and provided tx ({tx.id})"
+            )
         tx.txhash = txhash
-        tx.created = int(time.time())
+        now = int(time.time())
+        tx.created = now
+        tx.last_updated = now
+        tx.retries = 0  # reset retries
         tx.capped = False
         tx.__class__ = PendingTx
         tx: PendingTx
-        self.__set_active(tx=tx)
+
+        self.__pop()  # remove from queue
+        self.__set_active(tx=tx)  # set as active
         return tx
 
     def fault(
         self,
-        fault: Faults,
-        clear_active: bool,
-        error: Optional[str] = None,
+        fault_error: TransactionFaulted,
     ) -> None:
         """Fault the active transaction."""
-        hook = self.__active.on_fault
         if not self.__active:
             raise RuntimeError("No active transaction to fault")
+        if fault_error.tx.id != self.__active.id:
+            raise RuntimeError(
+                f"Mismatch between active tx ({self.__active.id}) and faulted tx ({fault_error.tx.id})"
+            )
+
+        hook = self.__active.on_fault
+
         tx = self.__active
-        tx.fault = fault
-        tx.error = error
-        tx.__class__ = FaultyTx
-        tx: FaultyTx
-        self.faulty.append(tx)
+        txhash = tx.txhash.hex()
+
+        tx.fault = fault_error.fault
+        tx.error = fault_error.message
+        tx.__class__ = FaultedTx
+        tx: FaultedTx
+
         log.warn(
-            f"[state] tracked faulty transaction #atx-{tx.id} "
-            f"{len(self.faulty)}/{self.faulty.maxlen} faults cached"
+            f"[tracker] transaction #atx-{tx.id} faulted with '{tx.fault.value}'; "
+            f"{txhash}{f' ({fault_error.message})' if fault_error.message else ''}"
         )
-        if clear_active:
-            self.clear_active()
-        if hook:
-            fire_hook(hook=hook, tx=tx)
+        self.clear_active()
+        fire_hook(hook=hook, tx=tx)
 
     def finalize_active_tx(self, receipt: TxReceipt) -> None:
         """
         Finalizes a pending transaction.
         Use polymorphism to transform the pending transaction into a finalized transaction.
         """
-        hook = self.__active.on_finalized
         if not self.__active:
             raise RuntimeError("No pending transaction to finalize")
+
         self.__active.receipt = receipt
         self.__active.__class__ = FinalizedTx
         tx = self.__active
+        hook = self.__active.on_finalized
         self.finalized.add(tx)  # noqa
-        log.info(f"[state] #atx-{tx.id} pending -> finalized")
+        log.info(f"[tracker] #atx-{tx.id} pending -> finalized")
         self.clear_active()
-        if hook:
-            fire_hook(hook=hook, tx=tx)
+        fire_hook(hook=hook, tx=tx)
 
     def clear_active(self) -> None:
         """Clear the active transaction (destructive operation)."""
         self.__active = None
         self.commit()
         log.debug(
-            f"[state] cleared 1 pending transaction \n"
-            f"[state] {len(self.queue)} queued "
+            f"[tracker] cleared 1 pending transaction \n"
+            f"[tracker] {len(self.queue)} queued "
             f"transaction{'s' if len(self.queue) != 1 else ''} remaining"
         )
 
     @property
     def pending(self) -> Optional[PendingTx]:
         """Return the active pending transaction if there is one."""
         return copy(self.__active)
 
     @property
     def queue(self) -> Tuple[FutureTx, ...]:
         """Return the queue of transactions."""
         return tuple(self.__queue)
 
-    def _pop(self) -> FutureTx:
-        """Pop the next transaction from the queue."""
-        return self.__queue.popleft()
+    def head(self) -> FutureTx:
+        return self.__queue[0]
 
-    def _requeue(self, tx: FutureTx) -> None:
-        """Re-queue a transaction for broadcast and subsequent tracking."""
-        self.__queue.append(tx)
+    def increment_broadcast_retries(self, tx: FutureTx) -> None:
+        tx.retries += 1
         self.commit()
-        log.info(
-            f"[state] re-queued transaction #atx-{tx.id} "
-            f"priority {len(self.__queue)}"
-        )
 
-    def _queue(
+    def reset_broadcast_retries(self, tx: FutureTx) -> None:
+        tx.retries = 0
+        self.commit()
+
+    def queue_tx(
         self,
         params: TxParams,
-        _from: ChecksumAddress,
+        on_broadcast_failure: Callable[[FutureTx, Exception], None],
+        on_fault: Callable[[FaultedTx], None],
+        on_finalized: Callable[[FinalizedTx], None],
+        on_insufficient_funds: Callable[
+            [Union[FutureTx, PendingTx], InsufficientFunds], None
+        ],
         info: Dict[str, str] = None,
-        on_broadcast: Optional[Callable] = None,
-        on_finalized: Optional[Callable] = None,
-        on_pause: Optional[Callable] = None,
-        on_fault: Optional[Callable] = None,
+        on_broadcast: Optional[Callable[[PendingTx], None]] = None,
     ) -> FutureTx:
         """Queue a new transaction for broadcast and subsequent tracking."""
         tx = FutureTx(
-            _from=_from,
             id=self.__COUNTER,
             params=params,
             info=info,
         )
 
         # configure hooks
-        tx.on_broadcast = on_broadcast
-        tx.on_finalized = on_finalized
-        tx.on_pause = on_pause
+        tx.on_broadcast_failure = on_broadcast_failure
         tx.on_fault = on_fault
+        tx.on_finalized = on_finalized
+        tx.on_broadcast = on_broadcast
+        tx.on_insufficient_funds = on_insufficient_funds
 
         self.__queue.append(tx)
         self.commit()
         self.__COUNTER += 1
         log.info(
-            f"[state] queued transaction #atx-{tx.id} " f"priority {len(self.__queue)}"
+            f"[tracker] queued transaction #atx-{tx.id} priority {len(self.__queue)}"
         )
         return tx
+
+    def remove_queued_tx(self, tx: FutureTx) -> bool:
+        try:
+            self.__queue.remove(tx)
+            return True
+        except ValueError:
+            return False
```

### Comparing `atxm-0.2.1/atxm/tx.py` & `atxm-0.3.0/atxm/tx.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,39 +1,51 @@
+import json
 from abc import ABC, abstractmethod
 from dataclasses import dataclass, field
-from typing import Callable, Dict, Optional
+from typing import Callable, Dict, Optional, Union
 
 from eth_typing import ChecksumAddress
 from eth_utils import encode_hex
 from hexbytes import HexBytes
-from web3.types import TxData, TxParams, TxReceipt
+from web3.types import TxParams, TxReceipt
 
-from atxm.exceptions import Faults
+from atxm.exceptions import Fault, InsufficientFunds
 
 TxHash = HexBytes
 
 
 @dataclass
 class AsyncTx(ABC):
     id: int
     final: bool = field(default=None, init=False)
-    fault: Optional[Faults] = field(default=None, init=False)
-    on_broadcast: Optional[Callable] = field(default=None, init=False)
-    on_finalized: Optional[Callable] = field(default=None, init=False)
-    on_pause: Optional[Callable] = field(default=None, init=False)
-    on_fault: Optional[Callable] = field(default=None, init=False)
+    fault: Optional[Fault] = field(default=None, init=False)
+    on_broadcast_failure: Optional[Callable[["FutureTx", Exception], None]] = field(
+        default=None, init=False
+    )
+    on_broadcast: Optional[Callable[["PendingTx"], None]] = field(
+        default=None, init=False
+    )
+    on_fault: Optional[Callable[["FaultedTx"], None]] = field(default=None, init=False)
+    on_finalized: Optional[Callable[["FinalizedTx"], None]] = field(
+        default=None, init=False
+    )
+    on_insufficient_funds: Optional[
+        Callable[[Union["FutureTx", "PendingTx"], InsufficientFunds], None]
+    ] = field(default=None, init=False)
 
     def __repr__(self):
         return f"<{self.__class__.__name__} id={self.id} final={self.final}>"
 
+    @abstractmethod
     def __hash__(self):
-        return hash(self.id)
+        raise NotImplementedError
 
+    @abstractmethod
     def __eq__(self, other):
-        return self.id == other.id
+        raise NotImplementedError
 
     def __ne__(self, other):
         return not self.__eq__(other)
 
     @abstractmethod
     def to_dict(self):
         raise NotImplementedError
@@ -41,101 +53,146 @@
     @classmethod
     def from_dict(cls, data: Dict):
         raise NotImplementedError
 
 
 @dataclass
 class FutureTx(AsyncTx):
-    final: bool = field(default=False, init=False)
     params: TxParams
-    _from: ChecksumAddress
     info: Optional[Dict] = None
+    retries: int = field(default=0, init=False)
+    final: bool = field(default=False, init=False)
 
     def __hash__(self):
-        return hash(self.id)
+        return hash(json.dumps(self.to_dict()))
+
+    def __eq__(self, other):
+        return (
+            self.id == other.id
+            and _serialize_tx_params(self.params) == _serialize_tx_params(other.params)
+            and self.info == other.info
+        )
+
+    @property
+    def _from(self) -> ChecksumAddress:
+        return self.params["from"]
 
     def to_dict(self) -> Dict:
         return {
             "id": self.id,
-            "from": self._from,
             "params": _serialize_tx_params(self.params),
             "info": self.info,
         }
 
     @classmethod
     def from_dict(cls, data: Dict):
         return cls(
             id=int(data["id"]),
-            _from=data["from"],
             params=TxParams(data["params"]),
-            info=dict(data["info"]),
+            info=dict(data["info"]) if data["info"] else None,
         )
 
 
 @dataclass
 class PendingTx(AsyncTx):
+    retries: int = field(default=0, init=False)
     final: bool = field(default=False, init=False)
+    last_updated: int = field(default=0, init=False)
+    params: TxParams
     txhash: TxHash
     created: int
-    data: Optional[TxData] = None
 
     def __hash__(self) -> int:
-        return hash(self.txhash)
+        # don't use "params" or "txhash" for hash because they can change
+        # over the object's lifetime
+        return hash((self.id, self.created))
+
+    def __eq__(self, other):
+        return (
+            self.id == other.id
+            and _serialize_tx_params(self.params) == _serialize_tx_params(other.params)
+            and self.txhash == other.txhash
+            and self.created == other.created
+        )
 
     def to_dict(self) -> Dict:
         return {
             "id": self.id,
+            "params": _serialize_tx_params(self.params),
             "txhash": self.txhash.hex(),
             "created": self.created,
-            "data": self.data,
         }
 
     @classmethod
     def from_dict(cls, data: Dict):
         return cls(
             id=int(data["id"]),
+            params=TxParams(data["params"]),
             txhash=HexBytes(data["txhash"]),
             created=int(data["created"]),
-            data=dict(data) if data else dict(),
         )
 
 
 @dataclass
 class FinalizedTx(AsyncTx):
     final: bool = field(default=True, init=False)
     receipt: TxReceipt
 
     def __hash__(self) -> int:
-        return hash(self.receipt["transactionHash"])
+        return hash((self.id, self.receipt["transactionHash"]))
+
+    def __eq__(self, other):
+        return self.id == other.id and _serialize_tx_receipt(
+            self.receipt
+        ) == _serialize_tx_receipt(other.receipt)
 
     def to_dict(self) -> Dict:
         return {"id": self.id, "receipt": _serialize_tx_receipt(self.receipt)}
 
     @classmethod
     def from_dict(cls, data: Dict):
         receipt = _deserialize_tx_receipt(data["receipt"])
         return cls(id=int(data["id"]), receipt=receipt)
 
+    @property
+    def txhash(self) -> TxHash:
+        return self.receipt["transactionHash"]
+
+    @property
+    def block_number(self):
+        return self.receipt["blockNumber"]
+
+    @property
+    def successful(self):
+        return self.receipt["status"] == 1
+
 
 @dataclass
-class FaultyTx(AsyncTx):
+class FaultedTx(AsyncTx):
     final: bool = field(default=False, init=False)
-    fault: Faults
+    fault: Fault
     error: Optional[str] = None
 
     def __hash__(self) -> int:
-        return hash(self.id)
+        return hash(json.dumps(self.to_dict()))
+
+    def __eq__(self, other):
+        return (
+            self.id == other.id
+            and self.fault == other.fault
+            and self.error == other.error
+        )
 
     def to_dict(self) -> Dict:
         return {"id": self.id, "error": str(self.error), "fault": self.fault.value}
 
     @classmethod
     def from_dict(cls, data: Dict):
         return cls(
-            id=int(data["id"]), error=str(data["error"]), fault=Faults(data["fault"])
+            id=int(data["id"]), error=str(data["error"]), fault=Fault(data["fault"])
         )
 
 
 def _serialize_tx_params(params: TxParams) -> Dict:
     """Serializes transaction parameters to a dictionary for disk storage."""
     data = params.get("data")
     if isinstance(data, bytes):
```

### Comparing `atxm-0.2.1/atxm.egg-info/PKG-INFO` & `atxm-0.3.0/atxm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atxm
-Version: 0.2.1
+Version: 0.3.0
 Summary: Automatic Transaction Machine (ATxM) for Ethereum
 Author-email: NuCypher <devs@nucypher.com>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -679,195 +679,204 @@
 Classifier: Natural Language :: English
 Classifier: Typing :: Typed
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: aiohttp==3.9.3; python_version >= "3.8"
+Requires-Dist: aiohttp==3.9.4rc0; python_version >= "3.8"
 Requires-Dist: aiosignal==1.3.1; python_version >= "3.7"
 Requires-Dist: attrs==23.2.0; python_version >= "3.7"
 Requires-Dist: automat==22.10.0
 Requires-Dist: bitarray==2.9.2
 Requires-Dist: certifi==2024.2.2; python_version >= "3.6"
 Requires-Dist: charset-normalizer==3.3.2; python_full_version >= "3.7.0"
 Requires-Dist: constantly==23.10.4; python_version >= "3.8"
 Requires-Dist: cytoolz==0.12.3; implementation_name == "cpython"
 Requires-Dist: eth-abi==4.2.1; python_version < "4" and python_full_version >= "3.7.2"
-Requires-Dist: eth-account==0.8.0; python_version >= "3.6" and python_version < "4"
-Requires-Dist: eth-hash[pycryptodome]==0.6.0; python_version >= "3.8" and python_version < "4"
-Requires-Dist: eth-keyfile==0.6.1
+Requires-Dist: eth-account==0.10.0; python_version >= "3.7" and python_version < "4"
+Requires-Dist: eth-hash[pycryptodome]==0.7.0; python_version >= "3.8" and python_version < "4"
+Requires-Dist: eth-keyfile==0.8.0; python_version >= "3.8" and python_version < "4"
 Requires-Dist: eth-keys==0.4.0
-Requires-Dist: eth-rlp==0.3.0; python_version >= "3.7" and python_version < "4"
+Requires-Dist: eth-rlp==1.0.1; python_version >= "3.8" and python_version < "4"
 Requires-Dist: eth-typing==3.5.2; python_version < "4" and python_full_version >= "3.7.2"
 Requires-Dist: eth-utils==2.3.1; python_version >= "3.7" and python_version < "4"
 Requires-Dist: frozenlist==1.4.1; python_version >= "3.8"
 Requires-Dist: hexbytes==0.3.1; python_version >= "3.7" and python_version < "4"
 Requires-Dist: hyperlink==21.0.0
-Requires-Dist: idna==3.6; python_version >= "3.5"
+Requires-Dist: idna==3.7; python_version >= "3.5"
 Requires-Dist: incremental==22.10.0
 Requires-Dist: jsonschema==4.21.1; python_version >= "3.8"
 Requires-Dist: jsonschema-specifications==2023.12.1; python_version >= "3.8"
 Requires-Dist: lru-dict==1.2.0
 Requires-Dist: multidict==6.0.5; python_version >= "3.7"
 Requires-Dist: parsimonious==0.9.0
-Requires-Dist: protobuf==5.26.0rc2; python_version >= "3.8"
+Requires-Dist: protobuf==5.26.1; python_version >= "3.8"
 Requires-Dist: pycryptodome==3.20.0
+Requires-Dist: python-statemachine==2.1.2; python_version < "3.13" and python_version >= "3.7"
 Requires-Dist: pyunormalize==15.1.0; python_version >= "3.6"
-Requires-Dist: referencing==0.33.0; python_version >= "3.8"
+Requires-Dist: referencing==0.34.0; python_version >= "3.8"
 Requires-Dist: regex==2023.12.25; python_version >= "3.7"
 Requires-Dist: requests==2.31.0; python_version >= "3.7"
 Requires-Dist: rlp==3.0.0
 Requires-Dist: rpds-py==0.18.0; python_version >= "3.8"
-Requires-Dist: setuptools==69.1.0; python_version >= "3.8"
+Requires-Dist: setuptools==69.2.0; python_version >= "3.8"
 Requires-Dist: six==1.16.0; python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2, 3.3"
 Requires-Dist: toolz==0.12.1; python_version >= "3.7"
-Requires-Dist: twisted==23.10.0; python_full_version >= "3.8.0"
-Requires-Dist: typing-extensions==4.9.0; python_version >= "3.8"
-Requires-Dist: urllib3==1.26.18; python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2, 3.3, 3.4, 3.5"
+Requires-Dist: twisted==24.3.0; python_full_version >= "3.8.0"
+Requires-Dist: typing-extensions==4.11.0; python_version >= "3.8"
+Requires-Dist: urllib3==2.2.0; python_version >= "3.8"
 Requires-Dist: web3==6.15.1; python_full_version >= "3.7.2"
 Requires-Dist: websockets==12.0; python_version >= "3.8"
 Requires-Dist: yarl==1.9.4; python_version >= "3.7"
-Requires-Dist: zope-interface==6.1; python_version >= "3.7"
+Requires-Dist: zope-interface==6.2; python_version >= "3.7"
 Provides-Extra: test
-Requires-Dist: aiohttp==3.9.3; python_version >= "3.8" and extra == "test"
+Requires-Dist: aiohttp==3.9.4rc0; python_version >= "3.8" and extra == "test"
 Requires-Dist: aiosignal==1.3.1; python_version >= "3.7" and extra == "test"
 Requires-Dist: annotated-types==0.6.0; python_version >= "3.8" and extra == "test"
 Requires-Dist: asttokens==2.4.1; extra == "test"
 Requires-Dist: attrs==23.2.0; python_version >= "3.7" and extra == "test"
 Requires-Dist: base58==1.0.3; extra == "test"
 Requires-Dist: bitarray==2.9.2; extra == "test"
-Requires-Dist: black==24.2.0; python_version >= "3.8" and extra == "test"
+Requires-Dist: black==24.3.0; python_version >= "3.8" and extra == "test"
 Requires-Dist: cached-property==1.5.2; extra == "test"
 Requires-Dist: certifi==2024.2.2; python_version >= "3.6" and extra == "test"
 Requires-Dist: cffi==1.16.0; python_version >= "3.8" and extra == "test"
 Requires-Dist: cfgv==3.4.0; python_version >= "3.8" and extra == "test"
 Requires-Dist: charset-normalizer==3.3.2; python_full_version >= "3.7.0" and extra == "test"
 Requires-Dist: click==8.1.7; python_version >= "3.7" and extra == "test"
-Requires-Dist: commonmark==0.9.1; extra == "test"
-Requires-Dist: cryptography==43.0.0.dev1; extra == "test"
+Requires-Dist: cryptography==42.0.5; extra == "test"
 Requires-Dist: cytoolz==0.12.3; implementation_name == "cpython" and extra == "test"
 Requires-Dist: dataclassy==0.11.1; python_version >= "3.6" and extra == "test"
 Requires-Dist: decorator==5.1.1; python_version >= "3.5" and extra == "test"
 Requires-Dist: deprecated==1.2.14; (python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2, 3.3") and extra == "test"
 Requires-Dist: distlib==0.3.8; extra == "test"
-Requires-Dist: eip712==0.2.2; (python_version >= "3.8" and python_version < "4") and extra == "test"
+Requires-Dist: eip712==0.2.5; (python_version >= "3.8" and python_version < "4") and extra == "test"
 Requires-Dist: eth-abi==4.2.1; (python_full_version >= "3.7.2" and python_version < "4") and extra == "test"
-Requires-Dist: eth-account==0.8.0; (python_version >= "3.6" and python_version < "4") and extra == "test"
-Requires-Dist: eth-ape==0.6.27; (python_version >= "3.8" and python_version < "4") and extra == "test"
+Requires-Dist: eth-account==0.10.0; (python_version >= "3.7" and python_version < "4") and extra == "test"
+Requires-Dist: eth-ape==0.7.13; (python_version >= "3.8" and python_version < "4") and extra == "test"
 Requires-Dist: eth-bloom==3.0.0; (python_version >= "3.8" and python_version < "4") and extra == "test"
-Requires-Dist: eth-hash[pycryptodome]==0.6.0; (python_version >= "3.8" and python_version < "4") and extra == "test"
-Requires-Dist: eth-keyfile==0.6.1; extra == "test"
+Requires-Dist: eth-hash[pycryptodome]==0.7.0; (python_version >= "3.8" and python_version < "4") and extra == "test"
+Requires-Dist: eth-keyfile==0.8.0; (python_version >= "3.8" and python_version < "4") and extra == "test"
 Requires-Dist: eth-keys==0.4.0; extra == "test"
-Requires-Dist: eth-pydantic-types==0.1.0a5; (python_version >= "3.8" and python_version < "4") and extra == "test"
-Requires-Dist: eth-rlp==0.3.0; (python_version >= "3.7" and python_version < "4") and extra == "test"
+Requires-Dist: eth-pydantic-types==0.1.0; (python_version >= "3.8" and python_version < "4") and extra == "test"
+Requires-Dist: eth-rlp==1.0.1; (python_version >= "3.8" and python_version < "4") and extra == "test"
 Requires-Dist: eth-tester[py-evm]==0.9.1b2; extra == "test"
 Requires-Dist: eth-typing==3.5.2; (python_full_version >= "3.7.2" and python_version < "4") and extra == "test"
 Requires-Dist: eth-utils==2.3.1; (python_version >= "3.7" and python_version < "4") and extra == "test"
-Requires-Dist: ethpm-types==0.5.11; (python_version >= "3.8" and python_version < "4") and extra == "test"
-Requires-Dist: evm-trace==0.1.2; (python_version >= "3.8" and python_version < "4") and extra == "test"
+Requires-Dist: ethpm-types==0.6.9; (python_version >= "3.8" and python_version < "4") and extra == "test"
+Requires-Dist: evm-trace==0.1.3; (python_version >= "3.8" and python_version < "4") and extra == "test"
+Requires-Dist: evmchains==0.0.5; python_version >= "3.8" and extra == "test"
 Requires-Dist: executing==2.0.1; python_version >= "3.5" and extra == "test"
-Requires-Dist: filelock==3.13.1; python_version >= "3.8" and extra == "test"
+Requires-Dist: filelock==3.13.4; python_version >= "3.8" and extra == "test"
 Requires-Dist: frozenlist==1.4.1; python_version >= "3.8" and extra == "test"
 Requires-Dist: greenlet==3.0.3; python_version >= "3.7" and extra == "test"
 Requires-Dist: hexbytes==0.3.1; (python_version >= "3.7" and python_version < "4") and extra == "test"
-Requires-Dist: identify==2.5.34; python_version >= "3.8" and extra == "test"
-Requires-Dist: idna==3.6; python_version >= "3.5" and extra == "test"
+Requires-Dist: identify==2.5.35; python_version >= "3.8" and extra == "test"
+Requires-Dist: idna==3.7; python_version >= "3.5" and extra == "test"
 Requires-Dist: ijson==3.2.3; extra == "test"
-Requires-Dist: importlib-metadata==7.0.1; python_version >= "3.8" and extra == "test"
+Requires-Dist: importlib-metadata==7.1.0; python_version >= "3.8" and extra == "test"
 Requires-Dist: iniconfig==2.0.0; python_version >= "3.7" and extra == "test"
-Requires-Dist: ipython==8.21.0; python_version >= "3.10" and extra == "test"
+Requires-Dist: ipython==8.23.0; python_version >= "3.10" and extra == "test"
 Requires-Dist: jedi==0.19.1; python_version >= "3.6" and extra == "test"
 Requires-Dist: jsonschema==4.21.1; python_version >= "3.8" and extra == "test"
 Requires-Dist: jsonschema-specifications==2023.12.1; python_version >= "3.8" and extra == "test"
 Requires-Dist: lazyasd==0.1.4; extra == "test"
 Requires-Dist: lru-dict==1.2.0; extra == "test"
+Requires-Dist: markdown-it-py==3.0.0; python_version >= "3.8" and extra == "test"
 Requires-Dist: matplotlib-inline==0.1.6; python_version >= "3.5" and extra == "test"
+Requires-Dist: mdurl==0.1.2; python_version >= "3.7" and extra == "test"
 Requires-Dist: morphys==1.0; extra == "test"
 Requires-Dist: msgspec==0.18.6; python_version >= "3.8" and extra == "test"
 Requires-Dist: multidict==6.0.5; python_version >= "3.7" and extra == "test"
 Requires-Dist: mypy-extensions==1.0.0; python_version >= "3.5" and extra == "test"
 Requires-Dist: nodeenv==1.8.0; (python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2, 3.3, 3.4, 3.5, 3.6") and extra == "test"
 Requires-Dist: numpy==1.26.4; python_version >= "3.10" and extra == "test"
 Requires-Dist: packaging==23.2; python_version >= "3.7" and extra == "test"
 Requires-Dist: pandas==1.5.3; python_version >= "3.8" and extra == "test"
 Requires-Dist: parsimonious==0.9.0; extra == "test"
-Requires-Dist: parso==0.8.3; python_version >= "3.6" and extra == "test"
+Requires-Dist: parso==0.8.4; python_version >= "3.6" and extra == "test"
 Requires-Dist: pathspec==0.12.1; python_version >= "3.8" and extra == "test"
-Requires-Dist: pexpect==4.9.0; sys_platform != "win32" and extra == "test"
+Requires-Dist: pexpect==4.9.0; (sys_platform != "win32" and sys_platform != "emscripten") and extra == "test"
 Requires-Dist: platformdirs==4.2.0; python_version >= "3.8" and extra == "test"
 Requires-Dist: pluggy==1.4.0; python_version >= "3.8" and extra == "test"
-Requires-Dist: pre-commit==3.6.1; python_version >= "3.9" and extra == "test"
+Requires-Dist: pre-commit==3.7.0; python_version >= "3.9" and extra == "test"
 Requires-Dist: prompt-toolkit==3.0.43; python_full_version >= "3.7.0" and extra == "test"
-Requires-Dist: protobuf==5.26.0rc2; python_version >= "3.8" and extra == "test"
+Requires-Dist: protobuf==5.26.1; python_version >= "3.8" and extra == "test"
 Requires-Dist: ptyprocess==0.7.0; extra == "test"
 Requires-Dist: pure-eval==0.2.2; extra == "test"
 Requires-Dist: py-cid==0.3.0; extra == "test"
 Requires-Dist: py-ecc==6.0.0; (python_version >= "3.6" and python_version < "4") and extra == "test"
 Requires-Dist: py-evm==0.7.0a4; extra == "test"
-Requires-Dist: py-geth==3.14.0; (python_version >= "3.7" and python_version < "4") and extra == "test"
+Requires-Dist: py-geth==4.4.0; (python_version >= "3.8" and python_version < "4") and extra == "test"
 Requires-Dist: py-multibase==1.0.3; extra == "test"
 Requires-Dist: py-multicodec==0.2.1; extra == "test"
 Requires-Dist: py-multihash==0.2.3; extra == "test"
-Requires-Dist: pycparser==2.21; extra == "test"
+Requires-Dist: pycparser==2.22; python_version >= "3.8" and extra == "test"
 Requires-Dist: pycryptodome==3.20.0; extra == "test"
-Requires-Dist: pydantic==2.6.1; python_version >= "3.8" and extra == "test"
-Requires-Dist: pydantic-core==2.16.2; python_version >= "3.8" and extra == "test"
+Requires-Dist: pydantic==2.5.3; python_version >= "3.7" and extra == "test"
+Requires-Dist: pydantic-core==2.14.6; python_version >= "3.7" and extra == "test"
+Requires-Dist: pydantic-settings==2.2.1; python_version >= "3.8" and extra == "test"
 Requires-Dist: pyethash==0.1.27; extra == "test"
 Requires-Dist: pygithub==1.59.1; python_version >= "3.7" and extra == "test"
 Requires-Dist: pygments==2.17.2; python_version >= "3.7" and extra == "test"
 Requires-Dist: pyjwt[crypto]==2.8.0; python_version >= "3.7" and extra == "test"
 Requires-Dist: pynacl==1.5.0; python_version >= "3.6" and extra == "test"
 Requires-Dist: pytest==7.4.4; python_version >= "3.7" and extra == "test"
-Requires-Dist: pytest-mock==3.12.0; python_version >= "3.8" and extra == "test"
-Requires-Dist: pytest-twisted==1.14.0; (python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2, 3.3, 3.4") and extra == "test"
+Requires-Dist: pytest-mock==3.14.0; python_version >= "3.8" and extra == "test"
+Requires-Dist: pytest-twisted==1.14.1; (python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2, 3.3, 3.4") and extra == "test"
 Requires-Dist: python-baseconv==1.2.2; extra == "test"
-Requires-Dist: python-dateutil==2.8.2; (python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2") and extra == "test"
+Requires-Dist: python-dateutil==2.9.0.post0; (python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2") and extra == "test"
+Requires-Dist: python-dotenv==1.0.1; python_version >= "3.8" and extra == "test"
 Requires-Dist: pytz==2024.1; extra == "test"
 Requires-Dist: pyunormalize==15.1.0; python_version >= "3.6" and extra == "test"
 Requires-Dist: pyyaml==6.0.1; python_version >= "3.6" and extra == "test"
-Requires-Dist: referencing==0.33.0; python_version >= "3.8" and extra == "test"
+Requires-Dist: referencing==0.34.0; python_version >= "3.8" and extra == "test"
 Requires-Dist: regex==2023.12.25; python_version >= "3.7" and extra == "test"
 Requires-Dist: requests==2.31.0; python_version >= "3.7" and extra == "test"
-Requires-Dist: rich==12.6.0; (python_full_version >= "3.6.3" and python_full_version < "4.0.0") and extra == "test"
+Requires-Dist: rich==13.7.1; python_full_version >= "3.7.0" and extra == "test"
 Requires-Dist: rlp==3.0.0; extra == "test"
 Requires-Dist: rpds-py==0.18.0; python_version >= "3.8" and extra == "test"
-Requires-Dist: ruff==0.2.1; python_version >= "3.7" and extra == "test"
+Requires-Dist: ruff==0.3.6; python_version >= "3.7" and extra == "test"
 Requires-Dist: safe-pysha3==1.0.4; extra == "test"
 Requires-Dist: semantic-version==2.10.0; python_version >= "2.7" and extra == "test"
-Requires-Dist: setuptools==69.1.0; python_version >= "3.8" and extra == "test"
+Requires-Dist: setuptools==69.2.0; python_version >= "3.8" and extra == "test"
 Requires-Dist: six==1.16.0; (python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2") and extra == "test"
 Requires-Dist: sortedcontainers==2.4.0; extra == "test"
-Requires-Dist: sqlalchemy==2.0.27; python_version >= "3.7" and extra == "test"
+Requires-Dist: sqlalchemy==2.0.29; python_version >= "3.7" and extra == "test"
 Requires-Dist: stack-data==0.6.3; extra == "test"
 Requires-Dist: toolz==0.12.1; python_version >= "3.7" and extra == "test"
 Requires-Dist: tqdm==4.66.2; python_version >= "3.7" and extra == "test"
-Requires-Dist: traitlets==5.14.1; python_version >= "3.8" and extra == "test"
+Requires-Dist: traitlets==5.14.2; python_version >= "3.8" and extra == "test"
 Requires-Dist: trie==2.2.0; (python_version >= "3.7" and python_version < "4") and extra == "test"
-Requires-Dist: typing-extensions==4.9.0; python_version >= "3.8" and extra == "test"
-Requires-Dist: urllib3==1.26.18; (python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2, 3.3, 3.4, 3.5") and extra == "test"
+Requires-Dist: typing-extensions==4.11.0; python_version >= "3.8" and extra == "test"
+Requires-Dist: urllib3==2.2.0; python_version >= "3.8" and extra == "test"
 Requires-Dist: varint==1.0.2; extra == "test"
-Requires-Dist: virtualenv==20.25.0; python_version >= "3.7" and extra == "test"
+Requires-Dist: virtualenv==20.25.1; python_version >= "3.7" and extra == "test"
 Requires-Dist: watchdog==3.0.0; python_version >= "3.7" and extra == "test"
 Requires-Dist: wcwidth==0.2.13; extra == "test"
 Requires-Dist: web3==6.15.1; python_full_version >= "3.7.2" and extra == "test"
 Requires-Dist: websockets==12.0; python_version >= "3.8" and extra == "test"
 Requires-Dist: wrapt==1.16.0; python_version >= "3.6" and extra == "test"
 Requires-Dist: yarl==1.9.4; python_version >= "3.7" and extra == "test"
-Requires-Dist: zipp==3.17.0; python_version >= "3.8" and extra == "test"
+Requires-Dist: zipp==3.18.1; python_version >= "3.8" and extra == "test"
 
 Automatic Tx Machine 🏧
 ========================
 
 [![Tests](https://github.com/nucypher/ATxM/actions/workflows/pytest.yml/badge.svg)](https://github.com/nucypher/ATxM/actions/workflows/pytest.yml)
 
 An async EVM transaction retry machine.
 Programmatically queue, broadcast, and retrying (speedup) transactions.
 Transactions are queued and broadcasted in a first-in-first-out (FIFO) order.
 
+The machine is designed to be used in a long-running process, like a server.
+
+[![Diagram](./diagram.png)](./diagram.png)
+
 ### Installation
 
 ```bash
 pip install atxm
 ```
 
 ### Usage
@@ -918,15 +927,14 @@
 
 ##### Lifecycle Hooks 
 
 Hooks are fired in a dedicated thread for lifecycle events.
 
 - `on_broadcast`: When a transaction is broadcasted.
 - `on_finalized`: When a transaction is finalized.
-- `on_pause`: When a transaction is halted by the strategy.
 - `on_fault`: When a transaction reverted or another error occurred.
 
 
 ##### Crash-Tolerance
 
 Internal state is written to a file to help recover from crashes
 and restarts. Internally caches LocalAccount instances in-memory which in
```

### Comparing `atxm-0.2.1/atxm.egg-info/requires.txt` & `atxm-0.3.0/atxm.egg-info/requires.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 automat==22.10.0
 bitarray==2.9.2
-eth-keyfile==0.6.1
 eth-keys==0.4.0
 hyperlink==21.0.0
 incremental==22.10.0
 lru-dict==1.2.0
 parsimonious==0.9.0
 pycryptodome==3.20.0
 rlp==3.0.0
@@ -15,228 +14,228 @@
 [:python_full_version >= "3.7.0"]
 charset-normalizer==3.3.2
 
 [:python_full_version >= "3.7.2"]
 web3==6.15.1
 
 [:python_full_version >= "3.8.0"]
-twisted==23.10.0
+twisted==24.3.0
+
+[:python_version < "3.13" and python_version >= "3.7"]
+python-statemachine==2.1.2
 
 [:python_version < "4" and python_full_version >= "3.7.2"]
 eth-abi==4.2.1
 eth-typing==3.5.2
 
 [:python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2, 3.3"]
 six==1.16.0
 
-[:python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2, 3.3, 3.4, 3.5"]
-urllib3==1.26.18
-
 [:python_version >= "3.5"]
-idna==3.6
+idna==3.7
 
 [:python_version >= "3.6"]
 certifi==2024.2.2
 pyunormalize==15.1.0
 
-[:python_version >= "3.6" and python_version < "4"]
-eth-account==0.8.0
-
 [:python_version >= "3.7"]
 aiosignal==1.3.1
 attrs==23.2.0
 multidict==6.0.5
 regex==2023.12.25
 requests==2.31.0
 toolz==0.12.1
 yarl==1.9.4
-zope-interface==6.1
+zope-interface==6.2
 
 [:python_version >= "3.7" and python_version < "4"]
-eth-rlp==0.3.0
+eth-account==0.10.0
 eth-utils==2.3.1
 hexbytes==0.3.1
 
 [:python_version >= "3.8"]
-aiohttp==3.9.3
+aiohttp==3.9.4rc0
 constantly==23.10.4
 frozenlist==1.4.1
 jsonschema==4.21.1
 jsonschema-specifications==2023.12.1
-protobuf==5.26.0rc2
-referencing==0.33.0
+protobuf==5.26.1
+referencing==0.34.0
 rpds-py==0.18.0
-setuptools==69.1.0
-typing-extensions==4.9.0
+setuptools==69.2.0
+typing-extensions==4.11.0
+urllib3==2.2.0
 websockets==12.0
 
 [:python_version >= "3.8" and python_version < "4"]
-eth-hash[pycryptodome]==0.6.0
+eth-hash[pycryptodome]==0.7.0
+eth-keyfile==0.8.0
+eth-rlp==1.0.1
 
 [test]
 asttokens==2.4.1
 base58==1.0.3
 bitarray==2.9.2
 cached-property==1.5.2
-commonmark==0.9.1
-cryptography==43.0.0.dev1
+cryptography==42.0.5
 distlib==0.3.8
-eth-keyfile==0.6.1
 eth-keys==0.4.0
 eth-tester[py-evm]==0.9.1b2
 ijson==3.2.3
 lazyasd==0.1.4
 lru-dict==1.2.0
 morphys==1.0
 parsimonious==0.9.0
 ptyprocess==0.7.0
 pure-eval==0.2.2
 py-cid==0.3.0
 py-evm==0.7.0a4
 py-multibase==1.0.3
 py-multicodec==0.2.1
 py-multihash==0.2.3
-pycparser==2.21
 pycryptodome==3.20.0
 pyethash==0.1.27
 python-baseconv==1.2.2
 pytz==2024.1
 rlp==3.0.0
 safe-pysha3==1.0.4
 sortedcontainers==2.4.0
 stack-data==0.6.3
 varint==1.0.2
 wcwidth==0.2.13
 
 [test:implementation_name == "cpython"]
 cytoolz==0.12.3
 
-[test:python_full_version >= "3.6.3" and python_full_version < "4.0.0"]
-rich==12.6.0
-
 [test:python_full_version >= "3.7.0"]
 charset-normalizer==3.3.2
 prompt-toolkit==3.0.43
+rich==13.7.1
 
 [test:python_full_version >= "3.7.2"]
 web3==6.15.1
 
 [test:python_full_version >= "3.7.2" and python_version < "4"]
 eth-abi==4.2.1
 eth-typing==3.5.2
 
 [test:python_version >= "2.7"]
 semantic-version==2.10.0
 
 [test:python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2"]
-python-dateutil==2.8.2
+python-dateutil==2.9.0.post0
 six==1.16.0
 
 [test:python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2, 3.3"]
 deprecated==1.2.14
 
 [test:python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2, 3.3, 3.4"]
-pytest-twisted==1.14.0
-
-[test:python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2, 3.3, 3.4, 3.5"]
-urllib3==1.26.18
+pytest-twisted==1.14.1
 
 [test:python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2, 3.3, 3.4, 3.5, 3.6"]
 nodeenv==1.8.0
 
 [test:python_version >= "3.10"]
-ipython==8.21.0
+ipython==8.23.0
 numpy==1.26.4
 
 [test:python_version >= "3.5"]
 decorator==5.1.1
 executing==2.0.1
-idna==3.6
+idna==3.7
 matplotlib-inline==0.1.6
 mypy-extensions==1.0.0
 
 [test:python_version >= "3.6"]
 certifi==2024.2.2
 dataclassy==0.11.1
 jedi==0.19.1
-parso==0.8.3
+parso==0.8.4
 pynacl==1.5.0
 pyunormalize==15.1.0
 pyyaml==6.0.1
 wrapt==1.16.0
 
 [test:python_version >= "3.6" and python_version < "4"]
-eth-account==0.8.0
 py-ecc==6.0.0
 
 [test:python_version >= "3.7"]
 aiosignal==1.3.1
 attrs==23.2.0
 click==8.1.7
 greenlet==3.0.3
 iniconfig==2.0.0
+mdurl==0.1.2
 multidict==6.0.5
 packaging==23.2
+pydantic==2.5.3
+pydantic-core==2.14.6
 pygithub==1.59.1
 pygments==2.17.2
 pyjwt[crypto]==2.8.0
 pytest==7.4.4
 regex==2023.12.25
 requests==2.31.0
-ruff==0.2.1
-sqlalchemy==2.0.27
+ruff==0.3.6
+sqlalchemy==2.0.29
 toolz==0.12.1
 tqdm==4.66.2
-virtualenv==20.25.0
+virtualenv==20.25.1
 watchdog==3.0.0
 yarl==1.9.4
 
 [test:python_version >= "3.7" and python_version < "4"]
-eth-rlp==0.3.0
+eth-account==0.10.0
 eth-utils==2.3.1
 hexbytes==0.3.1
-py-geth==3.14.0
 trie==2.2.0
 
 [test:python_version >= "3.8"]
-aiohttp==3.9.3
+aiohttp==3.9.4rc0
 annotated-types==0.6.0
-black==24.2.0
+black==24.3.0
 cffi==1.16.0
 cfgv==3.4.0
-filelock==3.13.1
+evmchains==0.0.5
+filelock==3.13.4
 frozenlist==1.4.1
-identify==2.5.34
-importlib-metadata==7.0.1
+identify==2.5.35
+importlib-metadata==7.1.0
 jsonschema==4.21.1
 jsonschema-specifications==2023.12.1
+markdown-it-py==3.0.0
 msgspec==0.18.6
 pandas==1.5.3
 pathspec==0.12.1
 platformdirs==4.2.0
 pluggy==1.4.0
-protobuf==5.26.0rc2
-pydantic==2.6.1
-pydantic-core==2.16.2
-pytest-mock==3.12.0
-referencing==0.33.0
+protobuf==5.26.1
+pycparser==2.22
+pydantic-settings==2.2.1
+pytest-mock==3.14.0
+python-dotenv==1.0.1
+referencing==0.34.0
 rpds-py==0.18.0
-setuptools==69.1.0
-traitlets==5.14.1
-typing-extensions==4.9.0
+setuptools==69.2.0
+traitlets==5.14.2
+typing-extensions==4.11.0
+urllib3==2.2.0
 websockets==12.0
-zipp==3.17.0
+zipp==3.18.1
 
 [test:python_version >= "3.8" and python_version < "4"]
-eip712==0.2.2
-eth-ape==0.6.27
+eip712==0.2.5
+eth-ape==0.7.13
 eth-bloom==3.0.0
-eth-hash[pycryptodome]==0.6.0
-eth-pydantic-types==0.1.0a5
-ethpm-types==0.5.11
-evm-trace==0.1.2
+eth-hash[pycryptodome]==0.7.0
+eth-keyfile==0.8.0
+eth-pydantic-types==0.1.0
+eth-rlp==1.0.1
+ethpm-types==0.6.9
+evm-trace==0.1.3
+py-geth==4.4.0
 
 [test:python_version >= "3.9"]
-pre-commit==3.6.1
+pre-commit==3.7.0
 
-[test:sys_platform != "win32"]
+[test:sys_platform != "win32" and sys_platform != "emscripten"]
 pexpect==4.9.0
```

### Comparing `atxm-0.2.1/dev-requirements.txt` & `atxm-0.3.0/dev-requirements.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,125 +1,129 @@
-aiohttp==3.9.3; python_version >= '3.8'
+aiohttp==3.9.4rc0; python_version >= '3.8'
 aiosignal==1.3.1; python_version >= '3.7'
 annotated-types==0.6.0; python_version >= '3.8'
 asttokens==2.4.1
 attrs==23.2.0; python_version >= '3.7'
 base58==1.0.3
 bitarray==2.9.2
-black==24.2.0; python_version >= '3.8'
+black==24.3.0; python_version >= '3.8'
 cached-property==1.5.2
 certifi==2024.2.2; python_version >= '3.6'
 cffi==1.16.0; python_version >= '3.8'
 cfgv==3.4.0; python_version >= '3.8'
 charset-normalizer==3.3.2; python_full_version >= '3.7.0'
 click==8.1.7; python_version >= '3.7'
-commonmark==0.9.1
-cryptography==43.0.0.dev1
+cryptography==42.0.5
 cytoolz==0.12.3; implementation_name == 'cpython'
 dataclassy==0.11.1; python_version >= '3.6'
 decorator==5.1.1; python_version >= '3.5'
 deprecated==1.2.14; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'
 distlib==0.3.8
-eip712==0.2.2; python_version >= '3.8' and python_version < '4'
+eip712==0.2.5; python_version >= '3.8' and python_version < '4'
 eth-abi==4.2.1; python_full_version >= '3.7.2' and python_version < '4'
-eth-account==0.8.0; python_version >= '3.6' and python_version < '4'
-eth-ape==0.6.27; python_version >= '3.8' and python_version < '4'
+eth-account==0.10.0; python_version >= '3.7' and python_version < '4'
+eth-ape==0.7.13; python_version >= '3.8' and python_version < '4'
 eth-bloom==3.0.0; python_version >= '3.8' and python_version < '4'
-eth-hash[pycryptodome]==0.6.0; python_version >= '3.8' and python_version < '4'
-eth-keyfile==0.6.1
+eth-hash[pycryptodome]==0.7.0; python_version >= '3.8' and python_version < '4'
+eth-keyfile==0.8.0; python_version >= '3.8' and python_version < '4'
 eth-keys==0.4.0
-eth-pydantic-types==0.1.0a5; python_version >= '3.8' and python_version < '4'
-eth-rlp==0.3.0; python_version >= '3.7' and python_version < '4'
+eth-pydantic-types==0.1.0; python_version >= '3.8' and python_version < '4'
+eth-rlp==1.0.1; python_version >= '3.8' and python_version < '4'
 eth-tester[py-evm]==0.9.1b2
 eth-typing==3.5.2; python_full_version >= '3.7.2' and python_version < '4'
 eth-utils==2.3.1; python_version >= '3.7' and python_version < '4'
-ethpm-types==0.5.11; python_version >= '3.8' and python_version < '4'
-evm-trace==0.1.2; python_version >= '3.8' and python_version < '4'
+ethpm-types==0.6.9; python_version >= '3.8' and python_version < '4'
+evm-trace==0.1.3; python_version >= '3.8' and python_version < '4'
+evmchains==0.0.5; python_version >= '3.8'
 executing==2.0.1; python_version >= '3.5'
-filelock==3.13.1; python_version >= '3.8'
+filelock==3.13.4; python_version >= '3.8'
 frozenlist==1.4.1; python_version >= '3.8'
 greenlet==3.0.3; python_version >= '3.7'
 hexbytes==0.3.1; python_version >= '3.7' and python_version < '4'
-identify==2.5.34; python_version >= '3.8'
-idna==3.6; python_version >= '3.5'
+identify==2.5.35; python_version >= '3.8'
+idna==3.7; python_version >= '3.5'
 ijson==3.2.3
-importlib-metadata==7.0.1; python_version >= '3.8'
+importlib-metadata==7.1.0; python_version >= '3.8'
 iniconfig==2.0.0; python_version >= '3.7'
-ipython==8.21.0; python_version >= '3.10'
+ipython==8.23.0; python_version >= '3.10'
 jedi==0.19.1; python_version >= '3.6'
 jsonschema==4.21.1; python_version >= '3.8'
 jsonschema-specifications==2023.12.1; python_version >= '3.8'
 lazyasd==0.1.4
 lru-dict==1.2.0
+markdown-it-py==3.0.0; python_version >= '3.8'
 matplotlib-inline==0.1.6; python_version >= '3.5'
+mdurl==0.1.2; python_version >= '3.7'
 morphys==1.0
 msgspec==0.18.6; python_version >= '3.8'
 multidict==6.0.5; python_version >= '3.7'
 mypy-extensions==1.0.0; python_version >= '3.5'
 nodeenv==1.8.0; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5, 3.6'
 numpy==1.26.4; python_version >= '3.10'
 packaging==23.2; python_version >= '3.7'
 pandas==1.5.3; python_version >= '3.8'
 parsimonious==0.9.0
-parso==0.8.3; python_version >= '3.6'
+parso==0.8.4; python_version >= '3.6'
 pathspec==0.12.1; python_version >= '3.8'
-pexpect==4.9.0; sys_platform != 'win32'
+pexpect==4.9.0; sys_platform != 'win32' and sys_platform != 'emscripten'
 platformdirs==4.2.0; python_version >= '3.8'
 pluggy==1.4.0; python_version >= '3.8'
-pre-commit==3.6.1; python_version >= '3.9'
+pre-commit==3.7.0; python_version >= '3.9'
 prompt-toolkit==3.0.43; python_full_version >= '3.7.0'
-protobuf==5.26.0rc2; python_version >= '3.8'
+protobuf==5.26.1; python_version >= '3.8'
 ptyprocess==0.7.0
 pure-eval==0.2.2
 py-cid==0.3.0
 py-ecc==6.0.0; python_version >= '3.6' and python_version < '4'
 py-evm==0.7.0a4
-py-geth==3.14.0; python_version >= '3.7' and python_version < '4'
+py-geth==4.4.0; python_version >= '3.8' and python_version < '4'
 py-multibase==1.0.3
 py-multicodec==0.2.1
 py-multihash==0.2.3
-pycparser==2.21
+pycparser==2.22; python_version >= '3.8'
 pycryptodome==3.20.0
-pydantic==2.6.1; python_version >= '3.8'
-pydantic-core==2.16.2; python_version >= '3.8'
+pydantic==2.5.3; python_version >= '3.7'
+pydantic-core==2.14.6; python_version >= '3.7'
+pydantic-settings==2.2.1; python_version >= '3.8'
 pyethash==0.1.27
 pygithub==1.59.1; python_version >= '3.7'
 pygments==2.17.2; python_version >= '3.7'
 pyjwt[crypto]==2.8.0; python_version >= '3.7'
 pynacl==1.5.0; python_version >= '3.6'
 pytest==7.4.4; python_version >= '3.7'
-pytest-mock==3.12.0; python_version >= '3.8'
-pytest-twisted==1.14.0; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4'
+pytest-mock==3.14.0; python_version >= '3.8'
+pytest-twisted==1.14.1; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4'
 python-baseconv==1.2.2
-python-dateutil==2.8.2; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2'
+python-dateutil==2.9.0.post0; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2'
+python-dotenv==1.0.1; python_version >= '3.8'
 pytz==2024.1
 pyunormalize==15.1.0; python_version >= '3.6'
 pyyaml==6.0.1; python_version >= '3.6'
-referencing==0.33.0; python_version >= '3.8'
+referencing==0.34.0; python_version >= '3.8'
 regex==2023.12.25; python_version >= '3.7'
 requests==2.31.0; python_version >= '3.7'
-rich==12.6.0; python_full_version >= '3.6.3' and python_full_version < '4.0.0'
+rich==13.7.1; python_full_version >= '3.7.0'
 rlp==3.0.0
 rpds-py==0.18.0; python_version >= '3.8'
-ruff==0.2.1; python_version >= '3.7'
+ruff==0.3.6; python_version >= '3.7'
 safe-pysha3==1.0.4
 semantic-version==2.10.0; python_version >= '2.7'
-setuptools==69.1.0; python_version >= '3.8'
+setuptools==69.2.0; python_version >= '3.8'
 six==1.16.0; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2'
 sortedcontainers==2.4.0
-sqlalchemy==2.0.27; python_version >= '3.7'
+sqlalchemy==2.0.29; python_version >= '3.7'
 stack-data==0.6.3
 toolz==0.12.1; python_version >= '3.7'
 tqdm==4.66.2; python_version >= '3.7'
-traitlets==5.14.1; python_version >= '3.8'
+traitlets==5.14.2; python_version >= '3.8'
 trie==2.2.0; python_version >= '3.7' and python_version < '4'
-typing-extensions==4.9.0; python_version >= '3.8'
-urllib3==1.26.18; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5'
+typing-extensions==4.11.0; python_version >= '3.8'
+urllib3==2.2.0; python_version >= '3.8'
 varint==1.0.2
-virtualenv==20.25.0; python_version >= '3.7'
+virtualenv==20.25.1; python_version >= '3.7'
 watchdog==3.0.0; python_version >= '3.7'
 wcwidth==0.2.13
 web3==6.15.1; python_full_version >= '3.7.2'
 websockets==12.0; python_version >= '3.8'
 wrapt==1.16.0; python_version >= '3.6'
 yarl==1.9.4; python_version >= '3.7'
-zipp==3.17.0; python_version >= '3.8'
+zipp==3.18.1; python_version >= '3.8'
```

### Comparing `atxm-0.2.1/pyproject.toml` & `atxm-0.3.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "atxm"
-version = "0.2.1"
+version = "0.3.0"
 authors = [
   { name="NuCypher", email="devs@nucypher.com" },
 ]
 description = "Automatic Transaction Machine (ATxM) for Ethereum"
 license = {file = "LICENSE"}
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `atxm-0.2.1/requirements.txt` & `atxm-0.3.0/requirements.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,45 +1,46 @@
-aiohttp==3.9.3; python_version >= '3.8'
+aiohttp==3.9.4rc0; python_version >= '3.8'
 aiosignal==1.3.1; python_version >= '3.7'
 attrs==23.2.0; python_version >= '3.7'
 automat==22.10.0
 bitarray==2.9.2
 certifi==2024.2.2; python_version >= '3.6'
 charset-normalizer==3.3.2; python_full_version >= '3.7.0'
 constantly==23.10.4; python_version >= '3.8'
 cytoolz==0.12.3; implementation_name == 'cpython'
 eth-abi==4.2.1; python_version < '4' and python_full_version >= '3.7.2'
-eth-account==0.8.0; python_version >= '3.6' and python_version < '4'
-eth-hash[pycryptodome]==0.6.0; python_version >= '3.8' and python_version < '4'
-eth-keyfile==0.6.1
+eth-account==0.10.0; python_version >= '3.7' and python_version < '4'
+eth-hash[pycryptodome]==0.7.0; python_version >= '3.8' and python_version < '4'
+eth-keyfile==0.8.0; python_version >= '3.8' and python_version < '4'
 eth-keys==0.4.0
-eth-rlp==0.3.0; python_version >= '3.7' and python_version < '4'
+eth-rlp==1.0.1; python_version >= '3.8' and python_version < '4'
 eth-typing==3.5.2; python_version < '4' and python_full_version >= '3.7.2'
 eth-utils==2.3.1; python_version >= '3.7' and python_version < '4'
 frozenlist==1.4.1; python_version >= '3.8'
 hexbytes==0.3.1; python_version >= '3.7' and python_version < '4'
 hyperlink==21.0.0
-idna==3.6; python_version >= '3.5'
+idna==3.7; python_version >= '3.5'
 incremental==22.10.0
 jsonschema==4.21.1; python_version >= '3.8'
 jsonschema-specifications==2023.12.1; python_version >= '3.8'
 lru-dict==1.2.0
 multidict==6.0.5; python_version >= '3.7'
 parsimonious==0.9.0
-protobuf==5.26.0rc2; python_version >= '3.8'
+protobuf==5.26.1; python_version >= '3.8'
 pycryptodome==3.20.0
+python-statemachine==2.1.2; python_version < '3.13' and python_version >= '3.7'
 pyunormalize==15.1.0; python_version >= '3.6'
-referencing==0.33.0; python_version >= '3.8'
+referencing==0.34.0; python_version >= '3.8'
 regex==2023.12.25; python_version >= '3.7'
 requests==2.31.0; python_version >= '3.7'
 rlp==3.0.0
 rpds-py==0.18.0; python_version >= '3.8'
-setuptools==69.1.0; python_version >= '3.8'
+setuptools==69.2.0; python_version >= '3.8'
 six==1.16.0; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'
 toolz==0.12.1; python_version >= '3.7'
-twisted==23.10.0; python_full_version >= '3.8.0'
-typing-extensions==4.9.0; python_version >= '3.8'
-urllib3==1.26.18; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5'
+twisted==24.3.0; python_full_version >= '3.8.0'
+typing-extensions==4.11.0; python_version >= '3.8'
+urllib3==2.2.0; python_version >= '3.8'
 web3==6.15.1; python_full_version >= '3.7.2'
 websockets==12.0; python_version >= '3.8'
 yarl==1.9.4; python_version >= '3.7'
-zope-interface==6.1; python_version >= '3.7'
+zope-interface==6.2; python_version >= '3.7'
```

