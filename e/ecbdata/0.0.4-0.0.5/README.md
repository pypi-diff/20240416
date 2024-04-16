# Comparing `tmp/ecbdata-0.0.4.tar.gz` & `tmp/ecbdata-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecbdata-0.0.4.tar", last modified: Tue Apr 16 09:50:02 2024, max compression
+gzip compressed data, was "ecbdata-0.0.5.tar", last modified: Tue Apr 16 10:49:51 2024, max compression
```

## Comparing `ecbdata-0.0.4.tar` & `ecbdata-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,19 @@
-drwxr-xr-x   0 metellis   (501) staff       (20)        0 2024-04-16 09:50:02.484448 ecbdata-0.0.4/
--rw-r--r--   0 metellis   (501) staff       (20)     1075 2024-04-16 09:46:02.000000 ecbdata-0.0.4/LICENSE.md
--rw-r--r--   0 metellis   (501) staff       (20)     2194 2024-04-16 09:50:02.484194 ecbdata-0.0.4/PKG-INFO
--rw-r--r--   0 metellis   (501) staff       (20)     1773 2024-04-16 09:49:54.000000 ecbdata-0.0.4/README.md
-drwxr-xr-x   0 metellis   (501) staff       (20)        0 2024-04-16 09:50:02.483102 ecbdata-0.0.4/ecbdata/
--rw-r--r--   0 metellis   (501) staff       (20)      188 2024-04-16 09:49:54.000000 ecbdata-0.0.4/ecbdata/__about__.py
--rw-r--r--   0 metellis   (501) staff       (20)      153 2024-04-16 09:46:02.000000 ecbdata-0.0.4/ecbdata/__init__.py
--rw-r--r--   0 metellis   (501) staff       (20)     9852 2024-04-16 09:46:02.000000 ecbdata-0.0.4/ecbdata/api.py
-drwxr-xr-x   0 metellis   (501) staff       (20)        0 2024-04-16 09:50:02.483898 ecbdata-0.0.4/ecbdata.egg-info/
--rw-r--r--   0 metellis   (501) staff       (20)     2194 2024-04-16 09:50:02.000000 ecbdata-0.0.4/ecbdata.egg-info/PKG-INFO
--rw-r--r--   0 metellis   (501) staff       (20)      209 2024-04-16 09:50:02.000000 ecbdata-0.0.4/ecbdata.egg-info/SOURCES.txt
--rw-r--r--   0 metellis   (501) staff       (20)        1 2024-04-16 09:50:02.000000 ecbdata-0.0.4/ecbdata.egg-info/dependency_links.txt
--rw-r--r--   0 metellis   (501) staff       (20)        8 2024-04-16 09:50:02.000000 ecbdata-0.0.4/ecbdata.egg-info/top_level.txt
--rw-r--r--   0 metellis   (501) staff       (20)       38 2024-04-16 09:50:02.484509 ecbdata-0.0.4/setup.cfg
--rw-r--r--   0 metellis   (501) staff       (20)      978 2024-04-16 09:49:54.000000 ecbdata-0.0.4/setup.py
+drwxr-xr-x   0 metellis   (501) staff       (20)        0 2024-04-16 10:49:51.852042 ecbdata-0.0.5/
+-rw-r--r--   0 metellis   (501) staff       (20)     1075 2024-04-16 09:46:02.000000 ecbdata-0.0.5/LICENSE.md
+-rw-r--r--   0 metellis   (501) staff       (20)     2627 2024-04-16 10:49:51.851803 ecbdata-0.0.5/PKG-INFO
+-rw-r--r--   0 metellis   (501) staff       (20)     2160 2024-04-16 10:49:36.000000 ecbdata-0.0.5/README.md
+drwxr-xr-x   0 metellis   (501) staff       (20)        0 2024-04-16 10:49:51.849893 ecbdata-0.0.5/ecbdata/
+-rw-r--r--   0 metellis   (501) staff       (20)      188 2024-04-16 10:49:36.000000 ecbdata-0.0.5/ecbdata/__about__.py
+-rw-r--r--   0 metellis   (501) staff       (20)      137 2024-04-16 10:49:36.000000 ecbdata-0.0.5/ecbdata/__init__.py
+-rw-r--r--   0 metellis   (501) staff       (20)     9648 2024-04-16 10:49:36.000000 ecbdata-0.0.5/ecbdata/api.py
+drwxr-xr-x   0 metellis   (501) staff       (20)        0 2024-04-16 10:49:51.851374 ecbdata-0.0.5/ecbdata/tests/
+-rw-r--r--   0 metellis   (501) staff       (20)      102 2024-04-16 10:49:36.000000 ecbdata-0.0.5/ecbdata/tests/__init__.py
+-rw-r--r--   0 metellis   (501) staff       (20)     1167 2024-04-16 10:49:36.000000 ecbdata-0.0.5/ecbdata/tests/test.py
+drwxr-xr-x   0 metellis   (501) staff       (20)        0 2024-04-16 10:49:51.850933 ecbdata-0.0.5/ecbdata.egg-info/
+-rw-r--r--   0 metellis   (501) staff       (20)     2627 2024-04-16 10:49:51.000000 ecbdata-0.0.5/ecbdata.egg-info/PKG-INFO
+-rw-r--r--   0 metellis   (501) staff       (20)      287 2024-04-16 10:49:51.000000 ecbdata-0.0.5/ecbdata.egg-info/SOURCES.txt
+-rw-r--r--   0 metellis   (501) staff       (20)        1 2024-04-16 10:49:51.000000 ecbdata-0.0.5/ecbdata.egg-info/dependency_links.txt
+-rw-r--r--   0 metellis   (501) staff       (20)       16 2024-04-16 10:49:51.000000 ecbdata-0.0.5/ecbdata.egg-info/requires.txt
+-rw-r--r--   0 metellis   (501) staff       (20)        8 2024-04-16 10:49:51.000000 ecbdata-0.0.5/ecbdata.egg-info/top_level.txt
+-rw-r--r--   0 metellis   (501) staff       (20)       38 2024-04-16 10:49:51.852115 ecbdata-0.0.5/setup.cfg
+-rw-r--r--   0 metellis   (501) staff       (20)      978 2024-04-16 09:49:54.000000 ecbdata-0.0.5/setup.py
```

### Comparing `ecbdata-0.0.4/LICENSE.md` & `ecbdata-0.0.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ecbdata-0.0.4/PKG-INFO` & `ecbdata-0.0.5/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,55 +1,50 @@
-Metadata-Version: 2.1
-Name: ecbdata
-Version: 0.0.4
-Home-page: https://github.com/LucaMingarelli/ecbdata
-Author: Luca Mingarelli
-Author-email: luca.mingarelli@ecb.europa.eu
-License: MIT
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-
 # ecbdata <img src="https://raw.githubusercontent.com/LucaMingarelli/ecbdata/master/ecbdata/res/Logo_European_Central_Bank.svg"  width="80">
 
 [![CircleCI](https://circleci.com/gh/LucaMingarelli/ecbdata.svg?style=svg&circle-token=cd9c300380d25c24c66cd6637693cc50a7e00248)](https://app.circleci.com/pipelines/github/LucaMingarelli/ecbdata)
-[![version](https://img.shields.io/badge/version-0.0.4-success.svg)](#)
+[![version](https://img.shields.io/badge/version-0.0.5-success.svg)](#)
 [![PyPI Latest Release](https://img.shields.io/pypi/v/ecbdata.svg)](https://pypi.org/project/ecbdata/)
 [![License](https://img.shields.io/pypi/l/ecbdata.svg)](https://github.com/LucaMingarelli/ecbdata/blob/master/LICENSE.txt)
 [![Downloads](https://static.pepy.tech/badge/ecbdata)](https://pepy.tech/project/ecbdata)
 <a href="https://www.buymeacoffee.com/lucamingarelli" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/v2/arial-yellow.png" alt="Buy Me A Coffee" style="height: 30px !important;width: 109px !important;" ></a>
 
 ## About
 
-ecbdata xxx .
-
-
-... from the [ECB Data Portal](https://data.ecb.europa.eu/help/data/overview).
+The **ecbdata** API allows for easy querying of data 
+from the [ECB Data Portal](https://data.ecb.europa.eu/help/data/overview).
 
 ## Installation
 You can install with pip as:
 
 `pip install ecbdata`
 
 ### Example
 
-xxx:
+```python
+from ecbdata import ecbdata
+
+df = ecbdata.get_series('ICP.M.U2.Y.XEF000.3.INX', start='2024-01', end='2024-03')
+
+```
+
+When behind a proxy server, one can establish a connection as
 
 ```python
 from ecbdata import ecbdata
+ecbdata.connect(proxies={'https': '<https-proxy>', 
+                         'http': '<http-proxy>'})
+
+df = ecbdata.get_series('ICP.M.U2.Y.XEF000.3.INX', start='2024-01', end='2024-03')
 
-from ecbdata import ECB_DataPortal
-ecbdata = ECB_DataPortal(proxies={'https': '<https-proxy>', 
-                                  'http': '<http-proxy>'})
 ```
 
+For details on available series and filters, 
+please consult the [ECB Data Portal](https://data.ecb.europa.eu/help/data/overview) page.
+
 
 ## Author
 
 Luca Mingarelli, 2024
 
 **You find this work useful?** <a href="https://www.buymeacoffee.com/lucamingarelli" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/v2/arial-yellow.png" alt="Buy Me A Coffee" style="height: 30px !important;width: 109px !important;" ></a>
 
-[![Python](https://img.shields.io/static/v1?label=made%20with&message=Python&color=blue&style=for-the-badge&logo=Python&logoColor=white)](#)
+[![Python](https://img.shields.io/static/v1?label=made%20with&message=Python&color=blue&style=for-the-badge&logo=Python&logoColor=white)](#)
```

#### html2text {}

```diff
@@ -1,24 +1,24 @@
-Metadata-Version: 2.1 Name: ecbdata Version: 0.0.4 Home-page: https://
-github.com/LucaMingarelli/ecbdata Author: Luca Mingarelli Author-email:
-luca.mingarelli@ecb.europa.eu License: MIT Classifier: Programming Language ::
-Python :: 3 Classifier: License :: OSI Approved :: MIT License Classifier:
-Operating System :: OS Independent Requires-Python: >=3.6 Description-Content-
-Type: text/markdown License-File: LICENSE.md # ecbdata [https://
-raw.githubusercontent.com/LucaMingarelli/ecbdata/master/ecbdata/res/
-Logo_European_Central_Bank.svg][![CircleCI](https://circleci.com/gh/
-LucaMingarelli/ecbdata.svg?style=svg&circle-
+# ecbdata [https://raw.githubusercontent.com/LucaMingarelli/ecbdata/master/
+ecbdata/res/Logo_European_Central_Bank.svg][![CircleCI](https://circleci.com/
+gh/LucaMingarelli/ecbdata.svg?style=svg&circle-
 token=cd9c300380d25c24c66cd6637693cc50a7e00248)](https://app.circleci.com/
 pipelines/github/LucaMingarelli/ecbdata) [![version](https://img.shields.io/
-badge/version-0.0.4-success.svg)](#) [![PyPI Latest Release](https://
+badge/version-0.0.5-success.svg)](#) [![PyPI Latest Release](https://
 img.shields.io/pypi/v/ecbdata.svg)](https://pypi.org/project/ecbdata/) [!
 [License](https://img.shields.io/pypi/l/ecbdata.svg)](https://github.com/
 LucaMingarelli/ecbdata/blob/master/LICENSE.txt) [![Downloads](https://
 static.pepy.tech/badge/ecbdata)](https://pepy.tech/project/ecbdata) _[_B_u_y_ _M_e_ _A
-_C_o_f_f_e_e_]## About ecbdata xxx . ... from the [ECB Data Portal](https://
-data.ecb.europa.eu/help/data/overview). ## Installation You can install with
-pip as: `pip install ecbdata` ### Example xxx: ```python from ecbdata import
-ecbdata from ecbdata import ECB_DataPortal ecbdata = ECB_DataPortal(proxies=
-{'https': '', 'http': ''}) ``` ## Author Luca Mingarelli, 2024 **You find this
-work useful?** _[_B_u_y_ _M_e_ _A_ _C_o_f_f_e_e_][![Python](https://img.shields.io/static/
+_C_o_f_f_e_e_]## About The **ecbdata** API allows for easy querying of data from the
+[ECB Data Portal](https://data.ecb.europa.eu/help/data/overview). ##
+Installation You can install with pip as: `pip install ecbdata` ### Example
+```python from ecbdata import ecbdata df = ecbdata.get_series
+('ICP.M.U2.Y.XEF000.3.INX', start='2024-01', end='2024-03') ``` When behind a
+proxy server, one can establish a connection as ```python from ecbdata import
+ecbdata ecbdata.connect(proxies={'https': '', 'http': ''}) df =
+ecbdata.get_series('ICP.M.U2.Y.XEF000.3.INX', start='2024-01', end='2024-03')
+``` For details on available series and filters, please consult the [ECB Data
+Portal](https://data.ecb.europa.eu/help/data/overview) page. ## Author Luca
+Mingarelli, 2024 **You find this work useful?** _[_B_u_y_ _M_e_ _A_ _C_o_f_f_e_e_][![Python]
+(https://img.shields.io/static/
 v1?label=made%20with&message=Python&color=blue&style=for-the-
 badge&logo=Python&logoColor=white)](#)
```

### Comparing `ecbdata-0.0.4/ecbdata/api.py` & `ecbdata-0.0.5/ecbdata/api.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,26 +22,25 @@
             proxy: Proxies specifications: a dictionary mapping protocol names (e.g. 'http', 'https') to proxy URLs. If not provided, environment variables 'HTTP_PROXY', 'HTTPS_PROXY' are used.
             verify: Whether to verify SSL certificates. Either of: `True`: Verifies certificates using the default trust store; `False`: Bypasses certificate verification (use with caution!); Path to a PEM-encoded certificate file: Uses the specified certificate to verify the server's certificate chain.
 
         Examples:
             >>> from ecbdata import ecbdata
             >>> df = ecbdata.get_series('ICP.M.U2.Y.XEF000.3.INX')
             >>> # Or to specify Proxies
-            >>> from ecbdata import ECB_DataPortal
-            >>> ecbdata = ECB_DataPortal(proxies={'https': '<https-proxies>',
-            >>>                                   'http': '<http-proxies>'},
-            >>>                          verify=False)
+            >>> ecbdata.connect(proxies={'https': '<https-proxies>',
+            >>>                          'http': '<http-proxies>'},
+            >>>                 verify=False)
             >>> df = ecbdata.get_series('ICP.M.U2.Y.XEF000.3.INX')
         """
         self.proxies = proxies
         self.verify = verify
-        self._session = self.Session(proxies=self.proxies, verify=self.verify)
+        self.connect(proxies=self.proxies, verify=self.verify)
 
 
-    def Session(self, proxies: dict=None, verify: bool or str=None):
+    def connect(self, proxies: dict=None, verify: bool or str=None):
         """
         Wrapper around :class:`requests:requests.Session`.
 
         The Session object allows you to persist certain parameters across requests. It also persists cookies across
         all requests made from the Session instance, and will use urllib3’s connection pooling. So if you’re making
         several requests to the same host, the underlying TCP connection will be reused, which can result in a
         significant performance increase (see HTTP persistent connection).
@@ -49,21 +48,19 @@
         For more details see the documentation of the wrapped :class:`requests:requests.Session` class.
 
         Args:
             proxy: Proxies specifications: a dictionary mapping protocol names (e.g. 'http', 'https') to proxy URLs. If not provided, environment variables 'HTTP_PROXY', 'HTTPS_PROXY' are used.
             verify: Whether to verify SSL certificates. Either of: `True`: Verifies certificates using the default trust store; `False`: Bypasses certificate verification (use with caution!); Path to a PEM-encoded certificate file: Uses the specified certificate to verify the server's certificate chain.
 
         """
-        if not hasattr(self, '_session') or not self._session:
-            session = requests.Session()
-            session.proxies = proxies or {}
-            if verify:
-                session.verify = verify
-            self._session = session
-            return session
+        session = requests.Session()
+        session.proxies = proxies or {}
+        if verify:
+            session.verify = verify
+        self._session = session
 
 
     def _search_string(self, ticker, start=None, end=None,
                        detail=None, updatedafter=None,
                        firstnobservations=None, lastnobservations=None,
                        includehistory=False
                        ):
```

### Comparing `ecbdata-0.0.4/ecbdata.egg-info/PKG-INFO` & `ecbdata-0.0.5/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,54 +1,65 @@
 Metadata-Version: 2.1
 Name: ecbdata
-Version: 0.0.4
+Version: 0.0.5
 Home-page: https://github.com/LucaMingarelli/ecbdata
 Author: Luca Mingarelli
 Author-email: luca.mingarelli@ecb.europa.eu
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
+Requires-Dist: requests
+Requires-Dist: pandas
 
 # ecbdata <img src="https://raw.githubusercontent.com/LucaMingarelli/ecbdata/master/ecbdata/res/Logo_European_Central_Bank.svg"  width="80">
 
 [![CircleCI](https://circleci.com/gh/LucaMingarelli/ecbdata.svg?style=svg&circle-token=cd9c300380d25c24c66cd6637693cc50a7e00248)](https://app.circleci.com/pipelines/github/LucaMingarelli/ecbdata)
-[![version](https://img.shields.io/badge/version-0.0.4-success.svg)](#)
+[![version](https://img.shields.io/badge/version-0.0.5-success.svg)](#)
 [![PyPI Latest Release](https://img.shields.io/pypi/v/ecbdata.svg)](https://pypi.org/project/ecbdata/)
 [![License](https://img.shields.io/pypi/l/ecbdata.svg)](https://github.com/LucaMingarelli/ecbdata/blob/master/LICENSE.txt)
 [![Downloads](https://static.pepy.tech/badge/ecbdata)](https://pepy.tech/project/ecbdata)
 <a href="https://www.buymeacoffee.com/lucamingarelli" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/v2/arial-yellow.png" alt="Buy Me A Coffee" style="height: 30px !important;width: 109px !important;" ></a>
 
 ## About
 
-ecbdata xxx .
-
-
-... from the [ECB Data Portal](https://data.ecb.europa.eu/help/data/overview).
+The **ecbdata** API allows for easy querying of data 
+from the [ECB Data Portal](https://data.ecb.europa.eu/help/data/overview).
 
 ## Installation
 You can install with pip as:
 
 `pip install ecbdata`
 
 ### Example
 
-xxx:
+```python
+from ecbdata import ecbdata
+
+df = ecbdata.get_series('ICP.M.U2.Y.XEF000.3.INX', start='2024-01', end='2024-03')
+
+```
+
+When behind a proxy server, one can establish a connection as
 
 ```python
 from ecbdata import ecbdata
+ecbdata.connect(proxies={'https': '<https-proxy>', 
+                         'http': '<http-proxy>'})
+
+df = ecbdata.get_series('ICP.M.U2.Y.XEF000.3.INX', start='2024-01', end='2024-03')
 
-from ecbdata import ECB_DataPortal
-ecbdata = ECB_DataPortal(proxies={'https': '<https-proxy>', 
-                                  'http': '<http-proxy>'})
 ```
 
+For details on available series and filters, 
+please consult the [ECB Data Portal](https://data.ecb.europa.eu/help/data/overview) page.
+
 
 ## Author
 
 Luca Mingarelli, 2024
 
 **You find this work useful?** <a href="https://www.buymeacoffee.com/lucamingarelli" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/v2/arial-yellow.png" alt="Buy Me A Coffee" style="height: 30px !important;width: 109px !important;" ></a>
```

#### html2text {}

```diff
@@ -1,24 +1,30 @@
-Metadata-Version: 2.1 Name: ecbdata Version: 0.0.4 Home-page: https://
+Metadata-Version: 2.1 Name: ecbdata Version: 0.0.5 Home-page: https://
 github.com/LucaMingarelli/ecbdata Author: Luca Mingarelli Author-email:
 luca.mingarelli@ecb.europa.eu License: MIT Classifier: Programming Language ::
 Python :: 3 Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: OS Independent Requires-Python: >=3.6 Description-Content-
-Type: text/markdown License-File: LICENSE.md # ecbdata [https://
-raw.githubusercontent.com/LucaMingarelli/ecbdata/master/ecbdata/res/
-Logo_European_Central_Bank.svg][![CircleCI](https://circleci.com/gh/
-LucaMingarelli/ecbdata.svg?style=svg&circle-
+Type: text/markdown License-File: LICENSE.md Requires-Dist: requests Requires-
+Dist: pandas # ecbdata [https://raw.githubusercontent.com/LucaMingarelli/
+ecbdata/master/ecbdata/res/Logo_European_Central_Bank.svg][![CircleCI](https://
+circleci.com/gh/LucaMingarelli/ecbdata.svg?style=svg&circle-
 token=cd9c300380d25c24c66cd6637693cc50a7e00248)](https://app.circleci.com/
 pipelines/github/LucaMingarelli/ecbdata) [![version](https://img.shields.io/
-badge/version-0.0.4-success.svg)](#) [![PyPI Latest Release](https://
+badge/version-0.0.5-success.svg)](#) [![PyPI Latest Release](https://
 img.shields.io/pypi/v/ecbdata.svg)](https://pypi.org/project/ecbdata/) [!
 [License](https://img.shields.io/pypi/l/ecbdata.svg)](https://github.com/
 LucaMingarelli/ecbdata/blob/master/LICENSE.txt) [![Downloads](https://
 static.pepy.tech/badge/ecbdata)](https://pepy.tech/project/ecbdata) _[_B_u_y_ _M_e_ _A
-_C_o_f_f_e_e_]## About ecbdata xxx . ... from the [ECB Data Portal](https://
-data.ecb.europa.eu/help/data/overview). ## Installation You can install with
-pip as: `pip install ecbdata` ### Example xxx: ```python from ecbdata import
-ecbdata from ecbdata import ECB_DataPortal ecbdata = ECB_DataPortal(proxies=
-{'https': '', 'http': ''}) ``` ## Author Luca Mingarelli, 2024 **You find this
-work useful?** _[_B_u_y_ _M_e_ _A_ _C_o_f_f_e_e_][![Python](https://img.shields.io/static/
+_C_o_f_f_e_e_]## About The **ecbdata** API allows for easy querying of data from the
+[ECB Data Portal](https://data.ecb.europa.eu/help/data/overview). ##
+Installation You can install with pip as: `pip install ecbdata` ### Example
+```python from ecbdata import ecbdata df = ecbdata.get_series
+('ICP.M.U2.Y.XEF000.3.INX', start='2024-01', end='2024-03') ``` When behind a
+proxy server, one can establish a connection as ```python from ecbdata import
+ecbdata ecbdata.connect(proxies={'https': '', 'http': ''}) df =
+ecbdata.get_series('ICP.M.U2.Y.XEF000.3.INX', start='2024-01', end='2024-03')
+``` For details on available series and filters, please consult the [ECB Data
+Portal](https://data.ecb.europa.eu/help/data/overview) page. ## Author Luca
+Mingarelli, 2024 **You find this work useful?** _[_B_u_y_ _M_e_ _A_ _C_o_f_f_e_e_][![Python]
+(https://img.shields.io/static/
 v1?label=made%20with&message=Python&color=blue&style=for-the-
 badge&logo=Python&logoColor=white)](#)
```

### Comparing `ecbdata-0.0.4/setup.py` & `ecbdata-0.0.5/setup.py`

 * *Files identical despite different names*

