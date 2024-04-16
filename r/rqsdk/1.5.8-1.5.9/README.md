# Comparing `tmp/rqsdk-1.5.8.tar.gz` & `tmp/rqsdk-1.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rqsdk-1.5.8.tar", last modified: Fri Dec  8 09:01:16 2023, max compression
+gzip compressed data, was "rqsdk-1.5.9.tar", last modified: Fri Feb  2 10:04:43 2024, max compression
```

## Comparing `rqsdk-1.5.8.tar` & `rqsdk-1.5.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-12-08 09:01:16.511098 rqsdk-1.5.8/
--rw-rw-rw-   0        0        0      263 2023-12-06 07:28:52.000000 rqsdk-1.5.8/HISTORY.md
--rw-rw-rw-   0        0        0      181 2023-12-06 07:28:52.000000 rqsdk-1.5.8/MANIFEST.in
--rw-rw-rw-   0        0        0      737 2023-12-08 09:01:16.511098 rqsdk-1.5.8/PKG-INFO
--rw-rw-rw-   0        0        0     1126 2023-12-06 07:28:52.000000 rqsdk-1.5.8/README.md
-drwxrwxrwx   0        0        0        0 2023-12-08 09:01:16.514100 rqsdk-1.5.8/rqsdk/
--rw-rw-rw-   0        0        0      778 2023-12-06 07:28:52.000000 rqsdk-1.5.8/rqsdk/__init__.py
--rw-rw-rw-   0        0        0      699 2023-12-06 07:28:52.000000 rqsdk-1.5.8/rqsdk/__main__.py
--rw-rw-rw-   0        0        0      518 2023-12-08 09:01:16.514100 rqsdk-1.5.8/rqsdk/_version.py
--rw-rw-rw-   0        0        0    13368 2023-12-06 07:28:52.000000 rqsdk-1.5.8/rqsdk/cmds.py
--rw-rw-rw-   0        0        0     1864 2023-12-06 07:28:52.000000 rqsdk-1.5.8/rqsdk/const.py
--rw-rw-rw-   0        0        0     6896 2023-12-06 07:28:52.000000 rqsdk-1.5.8/rqsdk/license_helper.py
--rw-rw-rw-   0        0        0      327 2023-12-06 07:28:52.000000 rqsdk-1.5.8/rqsdk/proxy_helper.py
--rw-rw-rw-   0        0        0     2519 2023-12-06 07:28:52.000000 rqsdk-1.5.8/rqsdk/script_update.py
--rw-rw-rw-   0        0        0      763 2023-12-06 07:28:52.000000 rqsdk-1.5.8/rqsdk/testing.py
-drwxrwxrwx   0        0        0        0 2023-12-08 09:01:16.509097 rqsdk-1.5.8/rqsdk.egg-info/
--rw-rw-rw-   0        0        0      737 2023-12-08 09:01:16.000000 rqsdk-1.5.8/rqsdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      438 2023-12-08 09:01:16.000000 rqsdk-1.5.8/rqsdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-12-08 09:01:16.000000 rqsdk-1.5.8/rqsdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-12-08 09:01:16.000000 rqsdk-1.5.8/rqsdk.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-12-08 08:52:03.000000 rqsdk-1.5.8/rqsdk.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     3855 2023-12-08 09:01:16.000000 rqsdk-1.5.8/rqsdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-12-08 09:01:16.000000 rqsdk-1.5.8/rqsdk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      260 2023-12-08 09:01:16.513097 rqsdk-1.5.8/setup.cfg
--rw-rw-rw-   0        0        0     3437 2023-12-08 08:47:19.000000 rqsdk-1.5.8/setup.py
--rw-rw-rw-   0        0        0    81982 2023-12-06 07:28:52.000000 rqsdk-1.5.8/versioneer.py
+drwxrwxrwx   0        0        0        0 2024-02-02 10:04:43.857455 rqsdk-1.5.9/
+-rw-rw-rw-   0        0        0      263 2023-12-06 07:28:52.000000 rqsdk-1.5.9/HISTORY.md
+-rw-rw-rw-   0        0        0      181 2023-12-06 07:28:52.000000 rqsdk-1.5.9/MANIFEST.in
+-rw-rw-rw-   0        0        0    11888 2024-02-02 10:04:43.856456 rqsdk-1.5.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1126 2023-12-06 07:28:52.000000 rqsdk-1.5.9/README.md
+drwxrwxrwx   0        0        0        0 2024-02-02 10:04:43.860456 rqsdk-1.5.9/rqsdk/
+-rw-rw-rw-   0        0        0      778 2023-12-06 07:28:52.000000 rqsdk-1.5.9/rqsdk/__init__.py
+-rw-rw-rw-   0        0        0      699 2023-12-06 07:28:52.000000 rqsdk-1.5.9/rqsdk/__main__.py
+-rw-rw-rw-   0        0        0      518 2024-02-02 10:04:43.861457 rqsdk-1.5.9/rqsdk/_version.py
+-rw-rw-rw-   0        0        0    13368 2023-12-06 07:28:52.000000 rqsdk-1.5.9/rqsdk/cmds.py
+-rw-rw-rw-   0        0        0     1864 2023-12-06 07:28:52.000000 rqsdk-1.5.9/rqsdk/const.py
+-rw-rw-rw-   0        0        0     6896 2023-12-06 07:28:52.000000 rqsdk-1.5.9/rqsdk/license_helper.py
+-rw-rw-rw-   0        0        0      327 2023-12-06 07:28:52.000000 rqsdk-1.5.9/rqsdk/proxy_helper.py
+-rw-rw-rw-   0        0        0     2519 2023-12-06 07:28:52.000000 rqsdk-1.5.9/rqsdk/script_update.py
+-rw-rw-rw-   0        0        0      763 2023-12-06 07:28:52.000000 rqsdk-1.5.9/rqsdk/testing.py
+drwxrwxrwx   0        0        0        0 2024-02-02 10:04:43.821446 rqsdk-1.5.9/rqsdk.egg-info/
+-rw-rw-rw-   0        0        0    11888 2024-02-02 10:04:43.000000 rqsdk-1.5.9/rqsdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      459 2024-02-02 10:04:43.000000 rqsdk-1.5.9/rqsdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-02-02 10:04:43.000000 rqsdk-1.5.9/rqsdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2024-02-02 10:04:43.000000 rqsdk-1.5.9/rqsdk.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-12-08 08:52:03.000000 rqsdk-1.5.9/rqsdk.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0     5356 2024-02-02 10:04:43.000000 rqsdk-1.5.9/rqsdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-02-02 10:04:43.000000 rqsdk-1.5.9/rqsdk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      260 2024-02-02 10:04:43.860456 rqsdk-1.5.9/setup.cfg
+-rw-rw-rw-   0        0        0     3833 2024-02-02 10:03:40.000000 rqsdk-1.5.9/setup.py
+-rw-rw-rw-   0        0        0    89123 2024-02-02 10:03:40.000000 rqsdk-1.5.9/versioneer.py
```

### Comparing `rqsdk-1.5.8/README.md` & `rqsdk-1.5.9/README.md`

 * *Files identical despite different names*

### Comparing `rqsdk-1.5.8/rqsdk/__init__.py` & `rqsdk-1.5.9/rqsdk/__init__.py`

 * *Files identical despite different names*

### Comparing `rqsdk-1.5.8/rqsdk/__main__.py` & `rqsdk-1.5.9/rqsdk/__main__.py`

 * *Files identical despite different names*

### Comparing `rqsdk-1.5.8/rqsdk/cmds.py` & `rqsdk-1.5.9/rqsdk/cmds.py`

 * *Files identical despite different names*

### Comparing `rqsdk-1.5.8/rqsdk/const.py` & `rqsdk-1.5.9/rqsdk/const.py`

 * *Files identical despite different names*

### Comparing `rqsdk-1.5.8/rqsdk/license_helper.py` & `rqsdk-1.5.9/rqsdk/license_helper.py`

 * *Files identical despite different names*

### Comparing `rqsdk-1.5.8/rqsdk/script_update.py` & `rqsdk-1.5.9/rqsdk/script_update.py`

 * *Files identical despite different names*

### Comparing `rqsdk-1.5.8/rqsdk/testing.py` & `rqsdk-1.5.9/rqsdk/testing.py`

 * *Files identical despite different names*

### Comparing `rqsdk-1.5.8/rqsdk.egg-info/requires.txt` & `rqsdk-1.5.9/rqsdk.egg-info/requires.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,179 +1,228 @@
-rqdatac_fund==1.0.*,>=1.0.18
-pandas>=0.24.2
-requests
-wcwidth
-click>=7.0
-rqdatac>=2.9.44
 pyjwt==1.7.1
+click>=7.0
 patsy>=0.5.1
+wcwidth
+pandas>=0.24.2
 statsmodels>=0.12.1
+requests
+rqdatac_fund==1.0.*,>=1.0.18
+
+[:platform_system == "Linux" and python_version >= "3.12"]
+pandas>=2.2.0
+
+[:python_version <= "3.11"]
+rqdatac>=2.9.44
 
 [:python_version <= "3.6"]
-python-rapidjson<=1.5
 numpy>=1.19.5
 tabulate<=0.8.10
+python-rapidjson<=1.5
 cryptography==2.9.2
 
 [:python_version <= "3.7"]
 scipy<=1.7.3
 
 [:python_version == "3.7"]
 numpy>=1.20.0
 
 [:python_version > "3.7"]
 pyopenssl>22.0.0
 
+[:python_version >= "3.12"]
+scipy>=1.11.2
+rqdatac>=2.11.12
+
 [:python_version >= "3.7"]
 tabulate>=0.9.0
 
 [:python_version >= "3.8"]
-scipy<=1.10.1,>=1.8.0
 numpy>=1.23.0
 
+[:python_version >= "3.8" and python_version <= "3.11"]
+scipy<=1.10.1,>=1.8.0
+
 [rqalpha_plus]
-rqrisk==1.0.7
-rqalpha-mod-rqfactor==1.0.10
-rqdatac_fund==1.0.*,>=1.0.18
+pyjwt==1.7.1
+wcwidth
+rqalpha-mod-incremental==0.0.9
 pandas>=0.24.2
-rqalpha-mod-spot==1.0.9
-rqalpha-mod-ams>=1.3.0
+rqalpha-mod-convertible==1.2.17
+rqalpha-mod-rqfactor==1.0.11
+rqalpha-mod-fund==0.0.15
+rqalpha-mod-option==1.2.1
+statsmodels>=0.12.1
+rqalpha-plus==4.2.7
+rqalpha-mod-ams>=1.3.1
+rqalpha==5.3.5
+click>=7.0
+ta-lib>=0.4.20
+rqalpha-mod-optimizer2==1.0.9
+h5py>=3.0.0
+hdf5plugin
+patsy>=0.5.1
 rqfactor==1.3.*,>=1.3.1
-rqalpha-mod-fund==0.0.14
+rqalpha-mod-spot==1.0.10
+rqalpha-mod-ricequant-data==2.4.3
+rqrisk==1.0.8
 matplotlib>=3.1.0
 requests
-ta-lib>=0.4.20
-rqalpha-mod-option==1.2.0
-hdf5plugin
-rqalpha-mod-convertible==1.2.16
-rqalpha-mod-incremental==0.0.8
-wcwidth
-h5py>=3.0.0
-click>=7.0
+rqdatac_fund==1.0.*,>=1.0.18
+
+[rqalpha_plus:platform_system == "Linux" and python_version >= "3.12"]
+pandas>=2.2.0
+
+[rqalpha_plus:python_version <= "3.11"]
 rqdatac>=2.9.44
-rqalpha==5.3.4
-rqalpha-mod-ricequant-data==2.4.1
-rqalpha-plus==4.2.6
-pyjwt==1.7.1
-patsy>=0.5.1
-statsmodels>=0.12.1
-rqalpha-mod-optimizer2==1.0.8
 
 [rqalpha_plus:python_version <= "3.6"]
+tabulate<=0.8.10
 python-rapidjson<=1.5
 numpy>=1.19.5
-tabulate<=0.8.10
 cryptography==2.9.2
 
 [rqalpha_plus:python_version <= "3.7"]
 scipy<=1.7.3
 
 [rqalpha_plus:python_version == "3.7"]
 numpy>=1.20.0
 
 [rqalpha_plus:python_version > "3.7"]
 pyopenssl>22.0.0
 
+[rqalpha_plus:python_version >= "3.12"]
+scipy>=1.11.2
+rqdatac>=2.11.12
+
 [rqalpha_plus:python_version >= "3.7"]
 tabulate>=0.9.0
 
 [rqalpha_plus:python_version >= "3.8"]
-scipy<=1.10.1,>=1.8.0
 numpy>=1.23.0
 
+[rqalpha_plus:python_version >= "3.8" and python_version <= "3.11"]
+scipy<=1.10.1,>=1.8.0
+
 [rqdatac]
-rqdatac_fund==1.0.*,>=1.0.18
-pandas>=0.24.2
-requests
-wcwidth
-click>=7.0
-rqdatac>=2.9.44
 pyjwt==1.7.1
+click>=7.0
 patsy>=0.5.1
+wcwidth
+pandas>=0.24.2
 statsmodels>=0.12.1
+requests
+rqdatac_fund==1.0.*,>=1.0.18
+
+[rqdatac:platform_system == "Linux" and python_version >= "3.12"]
+pandas>=2.2.0
+
+[rqdatac:python_version <= "3.11"]
+rqdatac>=2.9.44
 
 [rqdatac:python_version <= "3.6"]
-python-rapidjson<=1.5
 numpy>=1.19.5
 tabulate<=0.8.10
+python-rapidjson<=1.5
 cryptography==2.9.2
 
 [rqdatac:python_version <= "3.7"]
 scipy<=1.7.3
 
 [rqdatac:python_version == "3.7"]
 numpy>=1.20.0
 
 [rqdatac:python_version > "3.7"]
 pyopenssl>22.0.0
 
+[rqdatac:python_version >= "3.12"]
+scipy>=1.11.2
+rqdatac>=2.11.12
+
 [rqdatac:python_version >= "3.7"]
 tabulate>=0.9.0
 
 [rqdatac:python_version >= "3.8"]
-scipy<=1.10.1,>=1.8.0
 numpy>=1.23.0
 
+[rqdatac:python_version >= "3.8" and python_version <= "3.11"]
+scipy<=1.10.1,>=1.8.0
+
 [rqfactor]
-rqdatac_fund==1.0.*,>=1.0.18
-pandas>=0.24.2
-rqfactor==1.3.*,>=1.3.1
-requests
-ta-lib>=0.4.20
-wcwidth
-click>=7.0
-rqdatac>=2.9.44
 pyjwt==1.7.1
+click>=7.0
+ta-lib>=0.4.20
 patsy>=0.5.1
+wcwidth
+rqfactor==1.3.*,>=1.3.1
+pandas>=0.24.2
 statsmodels>=0.12.1
+requests
+rqdatac_fund==1.0.*,>=1.0.18
+
+[rqfactor:platform_system == "Linux" and python_version >= "3.12"]
+pandas>=2.2.0
+
+[rqfactor:python_version <= "3.11"]
+rqdatac>=2.9.44
 
 [rqfactor:python_version <= "3.6"]
-python-rapidjson<=1.5
 numpy>=1.19.5
 tabulate<=0.8.10
+python-rapidjson<=1.5
 cryptography==2.9.2
 
 [rqfactor:python_version <= "3.7"]
 scipy<=1.7.3
 
 [rqfactor:python_version == "3.7"]
 numpy>=1.20.0
 
 [rqfactor:python_version > "3.7"]
 pyopenssl>22.0.0
 
+[rqfactor:python_version >= "3.12"]
+scipy>=1.11.2
+rqdatac>=2.11.12
+
 [rqfactor:python_version >= "3.7"]
 tabulate>=0.9.0
 
 [rqfactor:python_version >= "3.8"]
-scipy<=1.10.1,>=1.8.0
 numpy>=1.23.0
 
+[rqfactor:python_version >= "3.8" and python_version <= "3.11"]
+scipy<=1.10.1,>=1.8.0
+
 [rqoptimizer]
-rqdatac_fund==1.0.*,>=1.0.18
-pandas>=0.24.2
-rqoptimizer==1.2.*,>=1.2.17
-rqoptimizer2==1.2.*,>=1.2.17
-requests
-wcwidth
-click>=7.0
-rqdatac>=2.9.44
-ecos==2.0.10
+scs==2.1.4
 pyjwt==1.7.1
+ecos==2.0.10
+click>=7.0
 patsy>=0.5.1
-scs==2.1.4
+wcwidth
+pandas>=0.24.2
+rqoptimizer==1.2.*,>=1.2.17
 statsmodels>=0.12.1
+requests
+rqdatac_fund==1.0.*,>=1.0.18
+rqoptimizer2==1.2.*,>=1.2.17
+
+[rqoptimizer:platform_system == "Linux" and python_version >= "3.12"]
+pandas>=2.2.0
 
 [rqoptimizer:python_version <= "3.10"]
 osqp==0.6.2.post5
 
+[rqoptimizer:python_version <= "3.11"]
+rqdatac>=2.9.44
+
 [rqoptimizer:python_version <= "3.6"]
-python-rapidjson<=1.5
 numpy>=1.19.5
 tabulate<=0.8.10
+python-rapidjson<=1.5
 cryptography==2.9.2
 
 [rqoptimizer:python_version <= "3.7"]
 scipy<=1.7.3
 
 [rqoptimizer:python_version == "3.11"]
 osqp==0.6.2.post8
@@ -183,48 +232,65 @@
 
 [rqoptimizer:python_version == "3.7"]
 numpy>=1.20.0
 
 [rqoptimizer:python_version > "3.7"]
 pyopenssl>22.0.0
 
+[rqoptimizer:python_version >= "3.12"]
+scipy>=1.11.2
+rqdatac>=2.11.12
+
 [rqoptimizer:python_version >= "3.7"]
-cvxpy==1.2.0
 tabulate>=0.9.0
+cvxpy==1.2.0
 
 [rqoptimizer:python_version >= "3.8"]
-scipy<=1.10.1,>=1.8.0
 numpy>=1.23.0
 
+[rqoptimizer:python_version >= "3.8" and python_version <= "3.11"]
+scipy<=1.10.1,>=1.8.0
+
 [rqpattr]
-rqdatac_fund==1.0.*,>=1.0.18
-pandas>=0.24.2
-requests
-wcwidth
-rqpattr>=0.0.2
-click>=7.0
-rqdatac>=2.9.44
 pyjwt==1.7.1
+click>=7.0
 patsy>=0.5.1
+wcwidth
+pandas>=0.24.2
+rqpattr>=0.0.2
 statsmodels>=0.12.1
+requests
+rqdatac_fund==1.0.*,>=1.0.18
+
+[rqpattr:platform_system == "Linux" and python_version >= "3.12"]
+pandas>=2.2.0
+
+[rqpattr:python_version <= "3.11"]
+rqdatac>=2.9.44
 
 [rqpattr:python_version <= "3.6"]
-python-rapidjson<=1.5
 numpy>=1.19.5
 tabulate<=0.8.10
+python-rapidjson<=1.5
 cryptography==2.9.2
 
 [rqpattr:python_version <= "3.7"]
 scipy<=1.7.3
 
 [rqpattr:python_version == "3.7"]
 numpy>=1.20.0
 
 [rqpattr:python_version > "3.7"]
 pyopenssl>22.0.0
 
+[rqpattr:python_version >= "3.12"]
+scipy>=1.11.2
+rqdatac>=2.11.12
+
 [rqpattr:python_version >= "3.7"]
 tabulate>=0.9.0
 
 [rqpattr:python_version >= "3.8"]
-scipy<=1.10.1,>=1.8.0
 numpy>=1.23.0
+
+[rqpattr:python_version >= "3.8" and python_version <= "3.11"]
+scipy<=1.10.1,>=1.8.0
```

### Comparing `rqsdk-1.5.8/setup.py` & `rqsdk-1.5.9/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,21 +12,24 @@
     "pyopenssl>22.0.0; python_version > '3.7'",  #  cryptography 的版本由 pyopenssl 来指定
     "cryptography==2.9.2; python_version <= '3.6'",  # python 3.6.0有点过分,pip更新报错，cryptography版本太高也报错
     "click>=7.0",
     "pyjwt==1.7.1",
     "patsy>=0.5.1",
     "statsmodels>=0.12.1",
     "scipy <= 1.7.3; python_version <= '3.7'",
-    "scipy >= 1.8.0, <= 1.10.1; python_version >= '3.8'",
+    "scipy >= 1.8.0, <= 1.10.1; python_version >= '3.8' and python_version <= '3.11'",
+    "scipy >= 1.11.2; python_version >= '3.12'",  # 低版本在python 3.12 下无法正常安装
     "numpy>=1.19.5; python_version <= '3.6'",
     "numpy>=1.20.0; python_version == '3.7'",
     "numpy>=1.23.0; python_version >= '3.8'",  # numpy 1.23.0 修改了类型大小
     "pandas >= 0.24.2",
+    "pandas>=2.2.0; platform_system=='Linux' and python_version>='3.12'", # Linux 系统的 Python 3.12 环境无法安装较低版本的 pandas
     "python-rapidjson <= 1.5; python_version <= '3.6'",  # rapidjson 1.6 开始不再提供 python 3.6 的 whl 包
-    "rqdatac>=2.9.44",
+    "rqdatac>=2.9.44; python_version <= '3.11'",
+    "rqdatac>=2.11.12; python_version >= '3.12'",  # rqdatac==2.11.12 开始兼容 python3.12
     "rqdatac_fund==1.0.*,>=1.0.18"
 }
 version_map["rqfactor"] = version_map["rqdatac"] | {
     "ta-lib>=0.4.20",
     "rqfactor==1.3.*,>=1.3.1",
 }
 version_map["rqoptimizer"] = version_map["rqdatac"] | {
@@ -36,26 +39,26 @@
     "cvxpy==1.2.0 ; python_version >= '3.7'",
     "osqp==0.6.2.post5 ; python_version <= '3.10'",
     "osqp==0.6.2.post8 ; python_version == '3.11'",
     "rqoptimizer==1.2.*,>=1.2.17",
     "rqoptimizer2==1.2.*,>=1.2.17",
 }
 version_map["rqalpha_plus"] = version_map["rqfactor"] | {
-    "rqalpha==5.3.4",
-    "rqalpha-mod-option==1.2.0",
-    "rqalpha-mod-optimizer2==1.0.8",
-    "rqalpha-mod-convertible==1.2.16",
-    "rqalpha-mod-ricequant-data==2.4.1",
-    "rqalpha-mod-rqfactor==1.0.10",
-    "rqalpha-mod-spot==1.0.9",
-    "rqalpha-mod-fund==0.0.14",
-    "rqalpha-mod-incremental==0.0.8",
-    "rqalpha-mod-ams >= 1.3.0",
-    "rqalpha-plus==4.2.6",
-    "rqrisk==1.0.7",
+    "rqalpha==5.3.5",
+    "rqalpha-mod-option==1.2.1",
+    "rqalpha-mod-optimizer2==1.0.9",
+    "rqalpha-mod-convertible==1.2.17",
+    "rqalpha-mod-ricequant-data==2.4.3",
+    "rqalpha-mod-rqfactor==1.0.11",
+    "rqalpha-mod-spot==1.0.10",
+    "rqalpha-mod-fund==0.0.15",
+    "rqalpha-mod-incremental==0.0.9",
+    "rqalpha-mod-ams >= 1.3.1",
+    "rqalpha-plus==4.2.7",
+    "rqrisk==1.0.8",
     "h5py>=3.0.0",
     "hdf5plugin",
     "matplotlib>=3.1.0",
 }
 version_map["rqpattr"] = version_map["rqdatac"] | {
     "rqpattr>=0.0.2"
 }
```

### Comparing `rqsdk-1.5.8/versioneer.py` & `rqsdk-1.5.9/versioneer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,39 +1,63 @@
-# -*- coding: utf-8 -*-
-# Version: 0.18
+# Version: 0.28
 
 """The Versioneer - like a rocketeer, but for versions.
 
 The Versioneer
 ==============
 
 * like a rocketeer, but for versions!
-* https://github.com/warner/python-versioneer
+* https://github.com/python-versioneer/python-versioneer
 * Brian Warner
-* License: Public Domain
-* Compatible With: python2.6, 2.7, 3.2, 3.3, 3.4, 3.5, 3.6, and pypy
-* [![Latest Version]
-(https://pypip.in/version/versioneer/badge.svg?style=flat)
-](https://pypi.python.org/pypi/versioneer/)
-* [![Build Status]
-(https://travis-ci.org/warner/python-versioneer.png?branch=master)
-](https://travis-ci.org/warner/python-versioneer)
+* License: Public Domain (Unlicense)
+* Compatible with: Python 3.7, 3.8, 3.9, 3.10 and pypy3
+* [![Latest Version][pypi-image]][pypi-url]
+* [![Build Status][travis-image]][travis-url]
 
-This is a tool for managing a recorded version number in distutils-based
+This is a tool for managing a recorded version number in setuptools-based
 python projects. The goal is to remove the tedious and error-prone "update
 the embedded version string" step from your release process. Making a new
 release should be as easy as recording a new tag in your version-control
 system, and maybe making new tarballs.
 
 
 ## Quick Install
 
-* `pip install versioneer` to somewhere to your $PATH
-* add a `[versioneer]` section to your setup.cfg (see below)
-* run `versioneer install` in your source tree, commit the results
+Versioneer provides two installation modes. The "classic" vendored mode installs
+a copy of versioneer into your repository. The experimental build-time dependency mode
+is intended to allow you to skip this step and simplify the process of upgrading.
+
+### Vendored mode
+
+* `pip install versioneer` to somewhere in your $PATH
+   * A [conda-forge recipe](https://github.com/conda-forge/versioneer-feedstock) is
+     available, so you can also use `conda install -c conda-forge versioneer`
+* add a `[tool.versioneer]` section to your `pyproject.toml` or a
+  `[versioneer]` section to your `setup.cfg` (see [Install](INSTALL.md))
+   * Note that you will need to add `tomli; python_version < "3.11"` to your
+     build-time dependencies if you use `pyproject.toml`
+* run `versioneer install --vendor` in your source tree, commit the results
+* verify version information with `python setup.py version`
+
+### Build-time dependency mode
+
+* `pip install versioneer` to somewhere in your $PATH
+   * A [conda-forge recipe](https://github.com/conda-forge/versioneer-feedstock) is
+     available, so you can also use `conda install -c conda-forge versioneer`
+* add a `[tool.versioneer]` section to your `pyproject.toml` or a
+  `[versioneer]` section to your `setup.cfg` (see [Install](INSTALL.md))
+* add `versioneer` (with `[toml]` extra, if configuring in `pyproject.toml`)
+  to the `requires` key of the `build-system` table in `pyproject.toml`:
+  ```toml
+  [build-system]
+  requires = ["setuptools", "versioneer[toml]"]
+  build-backend = "setuptools.build_meta"
+  ```
+* run `versioneer install --no-vendor` in your source tree, commit the results
+* verify version information with `python setup.py version`
 
 ## Version Identifiers
 
 Source trees come from a variety of places:
 
 * a version-control system checkout (mostly used by developers)
 * a nightly tarball, produced by build automation
@@ -57,15 +81,15 @@
 unreleased software (between tags), the version identifier should provide
 enough information to help developers recreate the same tree, while also
 giving them an idea of roughly how old the tree is (after version 1.2, before
 version 1.3). Many VCS systems can report a description that captures this,
 for example `git describe --tags --dirty --always` reports things like
 "0.7-1-g574ab98-dirty" to indicate that the checkout is one revision past the
 0.7 tag, has a unique revision id of "574ab98", and is "dirty" (it has
-uncommitted changes.
+uncommitted changes).
 
 The version identifier is used for multiple purposes:
 
 * to allow the module to self-identify its version: `myproject.__version__`
 * to choose a name and prefix for a 'setup.py sdist' tarball
 
 ## Theory of Operation
@@ -162,45 +186,45 @@
 display the full contents of `get_versions()` (including the `error` string,
 which may help identify what went wrong).
 
 ## Known Limitations
 
 Some situations are known to cause problems for Versioneer. This details the
 most significant ones. More can be found on Github
-[issues page](https://github.com/warner/python-versioneer/issues).
+[issues page](https://github.com/python-versioneer/python-versioneer/issues).
 
 ### Subprojects
 
 Versioneer has limited support for source trees in which `setup.py` is not in
 the root directory (e.g. `setup.py` and `.git/` are *not* siblings). The are
 two common reasons why `setup.py` might not be in the root:
 
 * Source trees which contain multiple subprojects, such as
   [Buildbot](https://github.com/buildbot/buildbot), which contains both
   "master" and "slave" subprojects, each with their own `setup.py`,
   `setup.cfg`, and `tox.ini`. Projects like these produce multiple PyPI
   distributions (and upload multiple independently-installable tarballs).
 * Source trees whose main purpose is to contain a C library, but which also
-  provide bindings to Python (and perhaps other langauges) in subdirectories.
+  provide bindings to Python (and perhaps other languages) in subdirectories.
 
 Versioneer will look for `.git` in parent directories, and most operations
 should get the right version string. However `pip` and `setuptools` have bugs
 and implementation details which frequently cause `pip install .` from a
 subproject directory to fail to find a correct version string (so it usually
 defaults to `0+unknown`).
 
 `pip install --editable .` should work correctly. `setup.py install` might
 work too.
 
 Pip-8.1.1 is known to have this problem, but hopefully it will get fixed in
 some later version.
 
-[Bug #38](https://github.com/warner/python-versioneer/issues/38) is tracking
+[Bug #38](https://github.com/python-versioneer/python-versioneer/issues/38) is tracking
 this issue. The discussion in
-[PR #61](https://github.com/warner/python-versioneer/pull/61) describes the
+[PR #61](https://github.com/python-versioneer/python-versioneer/pull/61) describes the
 issue from the Versioneer side in more detail.
 [pip PR#3176](https://github.com/pypa/pip/pull/3176) and
 [pip PR#3615](https://github.com/pypa/pip/pull/3615) contain work to improve
 pip to let Versioneer work correctly.
 
 Versioneer-0.16 and earlier only looked for a `.git` directory next to the
 `setup.cfg`, so subprojects were completely unsupported with those releases.
@@ -220,39 +244,28 @@
 `pkg_resources.DistributionNotFound` errors when running the entrypoint
 script, which must be resolved by re-installing the package. This happens
 when the install happens with one version, then the egg_info data is
 regenerated while a different version is checked out. Many setup.py commands
 cause egg_info to be rebuilt (including `sdist`, `wheel`, and installing into
 a different virtualenv), so this can be surprising.
 
-[Bug #83](https://github.com/warner/python-versioneer/issues/83) describes
+[Bug #83](https://github.com/python-versioneer/python-versioneer/issues/83) describes
 this one, but upgrading to a newer version of setuptools should probably
 resolve it.
 
-### Unicode version strings
-
-While Versioneer works (and is continually tested) with both Python 2 and
-Python 3, it is not entirely consistent with bytes-vs-unicode distinctions.
-Newer releases probably generate unicode version strings on py2. It's not
-clear that this is wrong, but it may be surprising for applications when then
-write these strings to a network connection or include them in bytes-oriented
-APIs like cryptographic checksums.
-
-[Bug #71](https://github.com/warner/python-versioneer/issues/71) investigates
-this question.
-
 
 ## Updating Versioneer
 
 To upgrade your project to a new release of Versioneer, do the following:
 
 * install the new Versioneer (`pip install -U versioneer` or equivalent)
-* edit `setup.cfg`, if necessary, to include any new configuration settings
-  indicated by the release notes. See [UPGRADING](./UPGRADING.md) for details.
-* re-run `versioneer install` in your source tree, to replace
+* edit `setup.cfg` and `pyproject.toml`, if necessary,
+  to include any new configuration settings indicated by the release notes.
+  See [UPGRADING](./UPGRADING.md) for details.
+* re-run `versioneer install --[no-]vendor` in your source tree, to replace
   `SRC/_version.py`
 * commit any changed files
 
 ## Future Directions
 
 This tool is designed to make it easily extended to other version-control
 systems: all VCS-specific components are in separate directories like
@@ -261,41 +274,64 @@
 will take a VCS name as an argument, and will construct a version of
 `versioneer.py` that is specific to the given VCS. It might also take the
 configuration arguments that are currently provided manually during
 installation by editing setup.py . Alternatively, it might go the other
 direction and include code from all supported VCS systems, reducing the
 number of intermediate scripts.
 
+## Similar projects
+
+* [setuptools_scm](https://github.com/pypa/setuptools_scm/) - a non-vendored build-time
+  dependency
+* [minver](https://github.com/jbweston/miniver) - a lightweight reimplementation of
+  versioneer
+* [versioningit](https://github.com/jwodder/versioningit) - a PEP 518-based setuptools
+  plugin
 
 ## License
 
 To make Versioneer easier to embed, all its code is dedicated to the public
 domain. The `_version.py` that it creates is also in the public domain.
-Specifically, both are released under the Creative Commons "Public Domain
-Dedication" license (CC0-1.0), as described in
-https://creativecommons.org/publicdomain/zero/1.0/ .
+Specifically, both are released under the "Unlicense", as described in
+https://unlicense.org/.
 
-"""
+[pypi-image]: https://img.shields.io/pypi/v/versioneer.svg
+[pypi-url]: https://pypi.python.org/pypi/versioneer/
+[travis-image]:
+https://img.shields.io/travis/com/python-versioneer/python-versioneer.svg
+[travis-url]: https://travis-ci.com/github/python-versioneer/python-versioneer
 
-from __future__ import print_function
+"""
+# pylint:disable=invalid-name,import-outside-toplevel,missing-function-docstring
+# pylint:disable=missing-class-docstring,too-many-branches,too-many-statements
+# pylint:disable=raise-missing-from,too-many-lines,too-many-locals,import-error
+# pylint:disable=too-few-public-methods,redefined-outer-name,consider-using-with
+# pylint:disable=attribute-defined-outside-init,too-many-arguments
 
-try:
-    import configparser
-except ImportError:
-    import ConfigParser as configparser
+import configparser
 import errno
 import json
 import os
 import re
 import subprocess
 import sys
+import functools
 
 
 from pkg_resources import parse_version
 
+have_tomllib = True
+if sys.version_info >= (3, 11):
+    import tomllib
+else:
+    try:
+        import tomli as tomllib
+    except ImportError:
+        have_tomllib = False
+
 
 class VersioneerConfig:
     """Container for Versioneer configuration parameters."""
 
 
 def get_root():
     """Get the project root directory.
@@ -321,131 +357,142 @@
     try:
         # Certain runtime workflows (setup.py install/develop in a setuptools
         # tree) execute all dependencies in a single python process, so
         # "versioneer" may be imported multiple times, and python's shared
         # module-import table will cache the first one. So we can't use
         # os.path.dirname(__file__), as that will find whichever
         # versioneer.py was first imported, even in later projects.
-        me = os.path.realpath(os.path.abspath(__file__))
-        me_dir = os.path.normcase(os.path.splitext(me)[0])
+        my_path = os.path.realpath(os.path.abspath(__file__))
+        me_dir = os.path.normcase(os.path.splitext(my_path)[0])
         vsr_dir = os.path.normcase(os.path.splitext(versioneer_py)[0])
-        if me_dir != vsr_dir:
+        if me_dir != vsr_dir and "VERSIONEER_PEP518" not in globals():
             print("Warning: build in %s is using versioneer.py from %s"
-                  % (os.path.dirname(me), versioneer_py))
+                  % (os.path.dirname(my_path), versioneer_py))
     except NameError:
         pass
     return root
 
 
 def get_config_from_root(root):
     """Read the project setup.cfg file to determine Versioneer config."""
-    # This might raise EnvironmentError (if setup.cfg is missing), or
+    # This might raise OSError (if setup.cfg is missing), or
     # configparser.NoSectionError (if it lacks a [versioneer] section), or
     # configparser.NoOptionError (if it lacks "VCS="). See the docstring at
     # the top of versioneer.py for instructions on writing your setup.cfg .
+    pyproject_toml = os.path.join(root, "pyproject.toml")
     setup_cfg = os.path.join(root, "setup.cfg")
-    parser = configparser.SafeConfigParser()
-    with open(setup_cfg, "r") as f:
-        parser.readfp(f)
-    VCS = parser.get("versioneer", "VCS")  # mandatory
+    section = None
+    if os.path.exists(pyproject_toml) and have_tomllib:
+        try:
+            with open(pyproject_toml, 'rb') as fobj:
+                pp = tomllib.load(fobj)
+            section = pp['tool']['versioneer']
+        except (tomllib.TOMLDecodeError, KeyError):
+            pass
+    if not section:
+        parser = configparser.ConfigParser()
+        with open(setup_cfg) as cfg_file:
+            parser.read_file(cfg_file)
+        parser.get("versioneer", "VCS")  # raise error if missing
 
-    def get(parser, name):
-        if parser.has_option("versioneer", name):
-            return parser.get("versioneer", name)
-        return None
+        section = parser["versioneer"]
 
     cfg = VersioneerConfig()
-    cfg.VCS = VCS
-    cfg.style = get(parser, "style") or ""
-    cfg.versionfile_source = get(parser, "versionfile_source")
-    cfg.versionfile_build = get(parser, "versionfile_build")
-    cfg.tag_prefix = get(parser, "tag_prefix")
-    if cfg.tag_prefix in ("''", '""'):
+    cfg.VCS = section['VCS']
+    cfg.style = section.get("style", "")
+    cfg.versionfile_source = section.get("versionfile_source")
+    cfg.versionfile_build = section.get("versionfile_build")
+    cfg.tag_prefix = section.get("tag_prefix")
+    if cfg.tag_prefix in ("''", '""', None):
         cfg.tag_prefix = ""
-    cfg.parentdir_prefix = get(parser, "parentdir_prefix")
-    cfg.verbose = get(parser, "verbose")
+    cfg.parentdir_prefix = section.get("parentdir_prefix")
+    cfg.verbose = section.get("verbose")
     return cfg
 
 
 class NotThisMethod(Exception):
     """Exception raised if a method is not valid for the current scenario."""
 
 
 # these dictionaries contain VCS-specific tools
 LONG_VERSION_PY = {}
 HANDLERS = {}
 
 
 def register_vcs_handler(vcs, method):  # decorator
-    """Decorator to mark a method as the handler for a particular VCS."""
-
+    """Create decorator to mark a method as the handler of a VCS."""
     def decorate(f):
         """Store f in HANDLERS[vcs][method]."""
-        if vcs not in HANDLERS:
-            HANDLERS[vcs] = {}
-        HANDLERS[vcs][method] = f
+        HANDLERS.setdefault(vcs, {})[method] = f
         return f
-
     return decorate
 
 
 def run_command(commands, args, cwd=None, verbose=False, hide_stderr=False,
                 env=None):
     """Call the given command(s)."""
     assert isinstance(commands, list)
-    p = None
-    for c in commands:
+    process = None
+
+    popen_kwargs = {}
+    if sys.platform == "win32":
+        # This hides the console window if pythonw.exe is used
+        startupinfo = subprocess.STARTUPINFO()
+        startupinfo.dwFlags |= subprocess.STARTF_USESHOWWINDOW
+        popen_kwargs["startupinfo"] = startupinfo
+
+    for command in commands:
         try:
-            dispcmd = str([c] + args)
+            dispcmd = str([command] + args)
             # remember shell=False, so use git.cmd on windows, not just git
-            p = subprocess.Popen([c] + args, cwd=cwd, env=env,
-                                 stdout=subprocess.PIPE,
-                                 stderr=(subprocess.PIPE if hide_stderr
-                                         else None))
+            process = subprocess.Popen([command] + args, cwd=cwd, env=env,
+                                       stdout=subprocess.PIPE,
+                                       stderr=(subprocess.PIPE if hide_stderr
+                                               else None), **popen_kwargs)
             break
-        except EnvironmentError:
+        except OSError:
             e = sys.exc_info()[1]
             if e.errno == errno.ENOENT:
                 continue
             if verbose:
                 print("unable to run %s" % dispcmd)
                 print(e)
             return None, None
     else:
         if verbose:
             print("unable to find command, tried %s" % (commands,))
         return None, None
-    stdout = p.communicate()[0].strip()
-    if sys.version_info[0] >= 3:
-        stdout = stdout.decode()
-    if p.returncode != 0:
+    stdout = process.communicate()[0].strip().decode('utf-8')
+    if process.returncode != 0:
         if verbose:
             print("unable to run %s (error)" % dispcmd)
             print("stdout was %s" % stdout)
-        return None, p.returncode
-    return stdout, p.returncode
+        return None, process.returncode
+    return stdout, process.returncode
 
 
-LONG_VERSION_PY['git'] = '''
+LONG_VERSION_PY['git'] = r'''
 # This file helps to compute a version number in source trees obtained from
 # git-archive tarball (such as those provided by githubs download-from-tag
 # feature). Distribution tarballs (built by setup.py sdist) and build
 # directories (produced by setup.py build) will contain a much shorter file
 # that just contains the computed version number.
 
-# This file is released into the public domain. Generated by
-# versioneer-0.18 (https://github.com/warner/python-versioneer)
+# This file is released into the public domain.
+# Generated by versioneer-0.28
+# https://github.com/python-versioneer/python-versioneer
 
 """Git implementation of _version.py."""
 
 import errno
 import os
 import re
 import subprocess
 import sys
+import functools
 
 
 def get_keywords():
     """Get the keywords needed to look up the version information."""
     # these strings will be replaced by git during git-archive.
     # setup.py/versioneer.py will grep for the variable names, so they must
     # each be defined on a line of their own. _version.py will just call
@@ -480,79 +527,84 @@
 
 
 LONG_VERSION_PY = {}
 HANDLERS = {}
 
 
 def register_vcs_handler(vcs, method):  # decorator
-    """Decorator to mark a method as the handler for a particular VCS."""
+    """Create decorator to mark a method as the handler of a VCS."""
     def decorate(f):
         """Store f in HANDLERS[vcs][method]."""
         if vcs not in HANDLERS:
             HANDLERS[vcs] = {}
         HANDLERS[vcs][method] = f
         return f
     return decorate
 
 
 def run_command(commands, args, cwd=None, verbose=False, hide_stderr=False,
                 env=None):
     """Call the given command(s)."""
     assert isinstance(commands, list)
-    p = None
-    for c in commands:
+    process = None
+
+    popen_kwargs = {}
+    if sys.platform == "win32":
+        # This hides the console window if pythonw.exe is used
+        startupinfo = subprocess.STARTUPINFO()
+        startupinfo.dwFlags |= subprocess.STARTF_USESHOWWINDOW
+        popen_kwargs["startupinfo"] = startupinfo
+
+    for command in commands:
         try:
-            dispcmd = str([c] + args)
+            dispcmd = str([command] + args)
             # remember shell=False, so use git.cmd on windows, not just git
-            p = subprocess.Popen([c] + args, cwd=cwd, env=env,
-                                 stdout=subprocess.PIPE,
-                                 stderr=(subprocess.PIPE if hide_stderr
-                                         else None))
+            process = subprocess.Popen([command] + args, cwd=cwd, env=env,
+                                       stdout=subprocess.PIPE,
+                                       stderr=(subprocess.PIPE if hide_stderr
+                                               else None), **popen_kwargs)
             break
-        except EnvironmentError:
+        except OSError:
             e = sys.exc_info()[1]
             if e.errno == errno.ENOENT:
                 continue
             if verbose:
                 print("unable to run %%s" %% dispcmd)
                 print(e)
             return None, None
     else:
         if verbose:
             print("unable to find command, tried %%s" %% (commands,))
         return None, None
-    stdout = p.communicate()[0].strip()
-    if sys.version_info[0] >= 3:
-        stdout = stdout.decode()
-    if p.returncode != 0:
+    stdout = process.communicate()[0].strip().decode()
+    if process.returncode != 0:
         if verbose:
             print("unable to run %%s (error)" %% dispcmd)
             print("stdout was %%s" %% stdout)
-        return None, p.returncode
-    return stdout, p.returncode
+        return None, process.returncode
+    return stdout, process.returncode
 
 
 def versions_from_parentdir(parentdir_prefix, root, verbose):
     """Try to determine the version from the parent directory name.
 
     Source tarballs conventionally unpack into a directory that includes both
     the project name and a version string. We will also support searching up
     two directory levels for an appropriately named parent directory
     """
     rootdirs = []
 
-    for i in range(3):
+    for _ in range(3):
         dirname = os.path.basename(root)
         if dirname.startswith(parentdir_prefix):
             return {"version": dirname[len(parentdir_prefix):],
                     "full-revisionid": None,
                     "dirty": False, "error": None, "date": None}
-        else:
-            rootdirs.append(root)
-            root = os.path.dirname(root)  # up a level
+        rootdirs.append(root)
+        root = os.path.dirname(root)  # up a level
 
     if verbose:
         print("Tried directories %%s but none started with prefix %%s" %%
               (str(rootdirs), parentdir_prefix))
     raise NotThisMethod("rootdir doesn't start with parentdir_prefix")
 
 
@@ -561,75 +613,83 @@
     """Extract version information from the given file."""
     # the code embedded in _version.py can just fetch the value of these
     # keywords. When used from setup.py, we don't want to import _version.py,
     # so we do it with a regexp instead. This function is not used from
     # _version.py.
     keywords = {}
     try:
-        f = open(versionfile_abs, "r")
-        for line in f.readlines():
-            if line.strip().startswith("git_refnames ="):
-                mo = re.search(r'=\s*"(.*)"', line)
-                if mo:
-                    keywords["refnames"] = mo.group(1)
-            if line.strip().startswith("git_full ="):
-                mo = re.search(r'=\s*"(.*)"', line)
-                if mo:
-                    keywords["full"] = mo.group(1)
-            if line.strip().startswith("git_date ="):
-                mo = re.search(r'=\s*"(.*)"', line)
-                if mo:
-                    keywords["date"] = mo.group(1)
-        f.close()
-    except EnvironmentError:
+        with open(versionfile_abs, "r") as fobj:
+            for line in fobj:
+                if line.strip().startswith("git_refnames ="):
+                    mo = re.search(r'=\s*"(.*)"', line)
+                    if mo:
+                        keywords["refnames"] = mo.group(1)
+                if line.strip().startswith("git_full ="):
+                    mo = re.search(r'=\s*"(.*)"', line)
+                    if mo:
+                        keywords["full"] = mo.group(1)
+                if line.strip().startswith("git_date ="):
+                    mo = re.search(r'=\s*"(.*)"', line)
+                    if mo:
+                        keywords["date"] = mo.group(1)
+    except OSError:
         pass
     return keywords
 
 
 @register_vcs_handler("git", "keywords")
 def git_versions_from_keywords(keywords, tag_prefix, verbose):
     """Get version information from git keywords."""
-    if not keywords:
-        raise NotThisMethod("no keywords at all, weird")
+    if "refnames" not in keywords:
+        raise NotThisMethod("Short version file found")
     date = keywords.get("date")
     if date is not None:
+        # Use only the last line.  Previous lines may contain GPG signature
+        # information.
+        date = date.splitlines()[-1]
+
         # git-2.2.0 added "%%cI", which expands to an ISO-8601 -compliant
         # datestamp. However we prefer "%%ci" (which expands to an "ISO-8601
         # -like" string, which we must then edit to make compliant), because
         # it's been around since git-1.5.3, and it's too difficult to
         # discover which version we're using, or to work around using an
         # older one.
         date = date.strip().replace(" ", "T", 1).replace(" ", "", 1)
     refnames = keywords["refnames"].strip()
     if refnames.startswith("$Format"):
         if verbose:
             print("keywords are unexpanded, not using")
         raise NotThisMethod("unexpanded keywords, not a git-archive tarball")
-    refs = set([r.strip() for r in refnames.strip("()").split(",")])
+    refs = {r.strip() for r in refnames.strip("()").split(",")}
     # starting in git-1.8.3, tags are listed as "tag: foo-1.0" instead of
     # just "foo-1.0". If we see a "tag: " prefix, prefer those.
     TAG = "tag: "
-    tags = set([r[len(TAG):] for r in refs if r.startswith(TAG)])
+    tags = {r[len(TAG):] for r in refs if r.startswith(TAG)}
     if not tags:
         # Either we're using git < 1.8.3, or there really are no tags. We use
         # a heuristic: assume all version tags have a digit. The old git %%d
         # expansion behaves like git log --decorate=short and strips out the
         # refs/heads/ and refs/tags/ prefixes that would let us distinguish
         # between branches and tags. By ignoring refnames without digits, we
         # filter out many common branch names like "release" and
         # "stabilization", as well as "HEAD" and "master".
-        tags = set([r for r in refs if re.search(r'\d', r)])
+        tags = {r for r in refs if re.search(r'\d', r)}
         if verbose:
             print("discarding '%%s', no digits" %% ",".join(refs - tags))
     if verbose:
         print("likely tags: %%s" %% ",".join(sorted(tags)))
     for ref in sorted(tags):
         # sorting will prefer e.g. "2.0" over "2.0rc1"
         if ref.startswith(tag_prefix):
             r = ref[len(tag_prefix):]
+            # Filter out refs that exactly match prefix or that don't start
+            # with a number once the prefix is stripped (mostly a concern
+            # when prefix is '')
+            if not re.match(r'\d', r):
+                continue
             if verbose:
                 print("picking %%s" %% r)
             return {"version": r,
                     "full-revisionid": keywords["full"].strip(),
                     "dirty": False, "error": None,
                     "date": date}
     # no suitable tags, so version is "0+unknown", but full hex is still there
@@ -637,52 +697,92 @@
         print("no suitable tags, using unknown + full revision id")
     return {"version": "0+unknown",
             "full-revisionid": keywords["full"].strip(),
             "dirty": False, "error": "no suitable tags", "date": None}
 
 
 @register_vcs_handler("git", "pieces_from_vcs")
-def git_pieces_from_vcs(tag_prefix, root, verbose, run_command=run_command):
+def git_pieces_from_vcs(tag_prefix, root, verbose, runner=run_command):
     """Get version from 'git describe' in the root of the source tree.
 
     This only gets called if the git-archive 'subst' keywords were *not*
     expanded, and _version.py hasn't already been rewritten with a short
     version string, meaning we're inside a checked out source tree.
     """
     GITS = ["git"]
     if sys.platform == "win32":
         GITS = ["git.cmd", "git.exe"]
 
-    out, rc = run_command(GITS, ["rev-parse", "--git-dir"], cwd=root,
-                          hide_stderr=True)
+    # GIT_DIR can interfere with correct operation of Versioneer.
+    # It may be intended to be passed to the Versioneer-versioned project,
+    # but that should not change where we get our version from.
+    env = os.environ.copy()
+    env.pop("GIT_DIR", None)
+    runner = functools.partial(runner, env=env)
+
+    _, rc = runner(GITS, ["rev-parse", "--git-dir"], cwd=root,
+                   hide_stderr=not verbose)
     if rc != 0:
         if verbose:
             print("Directory %%s not under git control" %% root)
         raise NotThisMethod("'git rev-parse --git-dir' returned error")
 
     # if there is a tag matching tag_prefix, this yields TAG-NUM-gHEX[-dirty]
     # if there isn't one, this yields HEX[-dirty] (no NUM)
-    describe_out, rc = run_command(GITS, ["describe", "--tags", "--dirty",
-                                          "--always", "--long",
-                                          "--match", "%%s*" %% tag_prefix],
-                                   cwd=root)
+    describe_out, rc = runner(GITS, [
+        "describe", "--tags", "--dirty", "--always", "--long",
+        "--match", "{}[[:digit:]]*".format(tag_prefix)
+    ], cwd=root)
     # --long was added in git-1.5.5
     if describe_out is None:
         raise NotThisMethod("'git describe' failed")
     describe_out = describe_out.strip()
-    full_out, rc = run_command(GITS, ["rev-parse", "HEAD"], cwd=root)
+    full_out, rc = runner(GITS, ["rev-parse", "HEAD"], cwd=root)
     if full_out is None:
         raise NotThisMethod("'git rev-parse' failed")
     full_out = full_out.strip()
 
     pieces = {}
     pieces["long"] = full_out
     pieces["short"] = full_out[:7]  # maybe improved later
     pieces["error"] = None
 
+    branch_name, rc = runner(GITS, ["rev-parse", "--abbrev-ref", "HEAD"],
+                             cwd=root)
+    # --abbrev-ref was added in git-1.6.3
+    if rc != 0 or branch_name is None:
+        raise NotThisMethod("'git rev-parse --abbrev-ref' returned error")
+    branch_name = branch_name.strip()
+
+    if branch_name == "HEAD":
+        # If we aren't exactly on a branch, pick a branch which represents
+        # the current commit. If all else fails, we are on a branchless
+        # commit.
+        branches, rc = runner(GITS, ["branch", "--contains"], cwd=root)
+        # --contains was added in git-1.5.4
+        if rc != 0 or branches is None:
+            raise NotThisMethod("'git branch --contains' returned error")
+        branches = branches.split("\n")
+
+        # Remove the first line if we're running detached
+        if "(" in branches[0]:
+            branches.pop(0)
+
+        # Strip off the leading "* " from the list of branches.
+        branches = [branch[2:] for branch in branches]
+        if "master" in branches:
+            branch_name = "master"
+        elif not branches:
+            branch_name = None
+        else:
+            # Pick the first branch that is returned. Good or bad.
+            branch_name = branches[0]
+
+    pieces["branch"] = branch_name
+
     # parse describe_out. It will be like TAG-NUM-gHEX[-dirty] or HEX[-dirty]
     # TAG might have hyphens.
     git_describe = describe_out
 
     # look for -dirty suffix
     dirty = git_describe.endswith("-dirty")
     pieces["dirty"] = dirty
@@ -691,15 +791,15 @@
 
     # now we have TAG-NUM-gHEX or HEX
 
     if "-" in git_describe:
         # TAG-NUM-gHEX
         mo = re.search(r'^(.+)-(\d+)-g([0-9a-f]+)$', git_describe)
         if not mo:
-            # unparseable. Maybe git-describe is misbehaving?
+            # unparsable. Maybe git-describe is misbehaving?
             pieces["error"] = ("unable to parse git-describe output: '%%s'"
                                %% describe_out)
             return pieces
 
         # tag
         full_tag = mo.group(1)
         if not full_tag.startswith(tag_prefix):
@@ -716,21 +816,22 @@
 
         # commit: short hex revision ID
         pieces["short"] = mo.group(3)
 
     else:
         # HEX: no tags
         pieces["closest-tag"] = None
-        count_out, rc = run_command(GITS, ["rev-list", "HEAD", "--count"],
-                                    cwd=root)
-        pieces["distance"] = int(count_out)  # total number of commits
+        out, rc = runner(GITS, ["rev-list", "HEAD", "--left-right"], cwd=root)
+        pieces["distance"] = len(out.split())  # total number of commits
 
     # commit date: see ISO-8601 comment in git_versions_from_keywords()
-    date = run_command(GITS, ["show", "-s", "--format=%%ci", "HEAD"],
-                       cwd=root)[0].strip()
+    date = runner(GITS, ["show", "-s", "--format=%%ci", "HEAD"], cwd=root)[0].strip()
+    # Use only the last line.  Previous lines may contain GPG signature
+    # information.
+    date = date.splitlines()[-1]
     pieces["date"] = date.strip().replace(" ", "T", 1).replace(" ", "", 1)
 
     return pieces
 
 
 def plus_or_dot(pieces):
     """Return a + if we don't already have one, else return a ."""
@@ -760,27 +861,75 @@
         rendered = "0+untagged.%%d.g%%s" %% (pieces["distance"],
                                           pieces["short"])
         if pieces["dirty"]:
             rendered += ".dirty"
     return rendered
 
 
-def render_pep440_pre(pieces):
-    """TAG[.post.devDISTANCE] -- No -dirty.
+def render_pep440_branch(pieces):
+    """TAG[[.dev0]+DISTANCE.gHEX[.dirty]] .
+
+    The ".dev0" means not master branch. Note that .dev0 sorts backwards
+    (a feature branch will appear "older" than the master branch).
 
     Exceptions:
-    1: no tags. 0.post.devDISTANCE
+    1: no tags. 0[.dev0]+untagged.DISTANCE.gHEX[.dirty]
     """
     if pieces["closest-tag"]:
         rendered = pieces["closest-tag"]
+        if pieces["distance"] or pieces["dirty"]:
+            if pieces["branch"] != "master":
+                rendered += ".dev0"
+            rendered += plus_or_dot(pieces)
+            rendered += "%%d.g%%s" %% (pieces["distance"], pieces["short"])
+            if pieces["dirty"]:
+                rendered += ".dirty"
+    else:
+        # exception #1
+        rendered = "0"
+        if pieces["branch"] != "master":
+            rendered += ".dev0"
+        rendered += "+untagged.%%d.g%%s" %% (pieces["distance"],
+                                          pieces["short"])
+        if pieces["dirty"]:
+            rendered += ".dirty"
+    return rendered
+
+
+def pep440_split_post(ver):
+    """Split pep440 version string at the post-release segment.
+
+    Returns the release segments before the post-release and the
+    post-release version number (or -1 if no post-release segment is present).
+    """
+    vc = str.split(ver, ".post")
+    return vc[0], int(vc[1] or 0) if len(vc) == 2 else None
+
+
+def render_pep440_pre(pieces):
+    """TAG[.postN.devDISTANCE] -- No -dirty.
+
+    Exceptions:
+    1: no tags. 0.post0.devDISTANCE
+    """
+    if pieces["closest-tag"]:
         if pieces["distance"]:
-            rendered += ".post.dev%%d" %% pieces["distance"]
+            # update the post release segment
+            tag_version, post_version = pep440_split_post(pieces["closest-tag"])
+            rendered = tag_version
+            if post_version is not None:
+                rendered += ".post%%d.dev%%d" %% (post_version + 1, pieces["distance"])
+            else:
+                rendered += ".post0.dev%%d" %% (pieces["distance"])
+        else:
+            # no commits, use the tag as the version
+            rendered = pieces["closest-tag"]
     else:
         # exception #1
-        rendered = "0.post.dev%%d" %% pieces["distance"]
+        rendered = "0.post0.dev%%d" %% pieces["distance"]
     return rendered
 
 
 def render_pep440_post(pieces):
     """TAG[.postDISTANCE[.dev0]+gHEX] .
 
     The ".dev0" means dirty. Note that .dev0 sorts backwards
@@ -803,68 +952,49 @@
         rendered = "0.post%%d" %% pieces["distance"]
         if pieces["dirty"]:
             rendered += ".dev0"
         rendered += "+g%%s" %% pieces["short"]
     return rendered
 
 
-def render_pep440_ricequant(pieces):
-    tag = pieces["closest-tag"]
-    parsed_tag = parse_version(tag) if tag else None
-
-    working = working_version()
-    parsed_working = parse_version(working)
+def render_pep440_post_branch(pieces):
+    """TAG[.postDISTANCE[.dev0]+gHEX[.dirty]] .
 
-    rendered = working
+    The ".dev0" means not master branch.
 
-    if tag:
-        if parsed_working < parsed_tag:
-            if parsed_working.base_version == parsed_tag.base_version:
-                if not parsed_tag.is_postrelease:
-                    raise Exception("Only post release tag allowed, tag %s" % tag)
-                if parsed_tag._version.post[0] != "post":
-                    raise Exception("Only post release tag allowed, tag %s" % tag)
-                post_num = parsed_tag._version.post[1]
-                rendered += ".post%d" % (post_num + 1)
-                if pieces["distance"] or pieces["dirty"]:
-                    rendered += ".dev%d" % pieces["distance"]
-                if pieces["dirty"]:
-                    rendered += ".dirty"
-            else:
-                raise Exception(f"Developing version can not go back in time: {working_version()} < {tag}")
-        elif parsed_working == parsed_tag:
-            if pieces["distance"] or pieces["dirty"]:
-                rendered += ".post1.dev%d" % pieces["distance"]
-            if pieces["dirty"]:
-                rendered += ".dirty"
-        else:
-            if pieces["distance"] or pieces["dirty"]:
-                rendered += ".dev%d" % pieces["distance"]
-            else:
+    Exceptions:
+    1: no tags. 0.postDISTANCE[.dev0]+gHEX[.dirty]
+    """
+    if pieces["closest-tag"]:
+        rendered = pieces["closest-tag"]
+        if pieces["distance"] or pieces["dirty"]:
+            rendered += ".post%%d" %% pieces["distance"]
+            if pieces["branch"] != "master":
                 rendered += ".dev0"
-
+            rendered += plus_or_dot(pieces)
+            rendered += "g%%s" %% pieces["short"]
             if pieces["dirty"]:
                 rendered += ".dirty"
     else:
-        if pieces["distance"] or pieces["dirty"]:
-            rendered += ".dev%d" % pieces["distance"]
-        else:
+        # exception #1
+        rendered = "0.post%%d" %% pieces["distance"]
+        if pieces["branch"] != "master":
             rendered += ".dev0"
-
+        rendered += "+g%%s" %% pieces["short"]
         if pieces["dirty"]:
             rendered += ".dirty"
     return rendered
 
 
 def render_pep440_old(pieces):
     """TAG[.postDISTANCE[.dev0]] .
 
     The ".dev0" means dirty.
 
-    Eexceptions:
+    Exceptions:
     1: no tags. 0.postDISTANCE[.dev0]
     """
     if pieces["closest-tag"]:
         rendered = pieces["closest-tag"]
         if pieces["distance"] or pieces["dirty"]:
             rendered += ".post%%d" %% pieces["distance"]
             if pieces["dirty"]:
@@ -927,22 +1057,24 @@
                 "date": None}
 
     if not style or style == "default":
         style = "pep440"  # the default
 
     if style == "pep440":
         rendered = render_pep440(pieces)
+    elif style == "pep440-branch":
+        rendered = render_pep440_branch(pieces)
     elif style == "pep440-pre":
         rendered = render_pep440_pre(pieces)
     elif style == "pep440-post":
         rendered = render_pep440_post(pieces)
+    elif style == "pep440-post-branch":
+        rendered = render_pep440_post_branch(pieces)
     elif style == "pep440-old":
         rendered = render_pep440_old(pieces)
-    elif style == 'pep440-ricequant':
-        rendered = render_pep440_ricequant(pieces)
     elif style == "git-describe":
         rendered = render_git_describe(pieces)
     elif style == "git-describe-long":
         rendered = render_git_describe_long(pieces)
     else:
         raise ValueError("unknown style '%%s'" %% style)
 
@@ -968,15 +1100,15 @@
         pass
 
     try:
         root = os.path.realpath(__file__)
         # versionfile_source is the relative path from the top of the source
         # tree (where the .git directory might live) to this file. Invert
         # this to find the root from __file__.
-        for i in cfg.versionfile_source.split('/'):
+        for _ in cfg.versionfile_source.split('/'):
             root = os.path.dirname(root)
     except NameError:
         return {"version": "0+unknown", "full-revisionid": None,
                 "dirty": None,
                 "error": "unable to find root of source tree",
                 "date": None}
 
@@ -1003,75 +1135,83 @@
     """Extract version information from the given file."""
     # the code embedded in _version.py can just fetch the value of these
     # keywords. When used from setup.py, we don't want to import _version.py,
     # so we do it with a regexp instead. This function is not used from
     # _version.py.
     keywords = {}
     try:
-        f = open(versionfile_abs, "r")
-        for line in f.readlines():
-            if line.strip().startswith("git_refnames ="):
-                mo = re.search(r'=\s*"(.*)"', line)
-                if mo:
-                    keywords["refnames"] = mo.group(1)
-            if line.strip().startswith("git_full ="):
-                mo = re.search(r'=\s*"(.*)"', line)
-                if mo:
-                    keywords["full"] = mo.group(1)
-            if line.strip().startswith("git_date ="):
-                mo = re.search(r'=\s*"(.*)"', line)
-                if mo:
-                    keywords["date"] = mo.group(1)
-        f.close()
-    except EnvironmentError:
+        with open(versionfile_abs, "r") as fobj:
+            for line in fobj:
+                if line.strip().startswith("git_refnames ="):
+                    mo = re.search(r'=\s*"(.*)"', line)
+                    if mo:
+                        keywords["refnames"] = mo.group(1)
+                if line.strip().startswith("git_full ="):
+                    mo = re.search(r'=\s*"(.*)"', line)
+                    if mo:
+                        keywords["full"] = mo.group(1)
+                if line.strip().startswith("git_date ="):
+                    mo = re.search(r'=\s*"(.*)"', line)
+                    if mo:
+                        keywords["date"] = mo.group(1)
+    except OSError:
         pass
     return keywords
 
 
 @register_vcs_handler("git", "keywords")
 def git_versions_from_keywords(keywords, tag_prefix, verbose):
     """Get version information from git keywords."""
-    if not keywords:
-        raise NotThisMethod("no keywords at all, weird")
+    if "refnames" not in keywords:
+        raise NotThisMethod("Short version file found")
     date = keywords.get("date")
     if date is not None:
+        # Use only the last line.  Previous lines may contain GPG signature
+        # information.
+        date = date.splitlines()[-1]
+
         # git-2.2.0 added "%cI", which expands to an ISO-8601 -compliant
         # datestamp. However we prefer "%ci" (which expands to an "ISO-8601
         # -like" string, which we must then edit to make compliant), because
         # it's been around since git-1.5.3, and it's too difficult to
         # discover which version we're using, or to work around using an
         # older one.
         date = date.strip().replace(" ", "T", 1).replace(" ", "", 1)
     refnames = keywords["refnames"].strip()
     if refnames.startswith("$Format"):
         if verbose:
             print("keywords are unexpanded, not using")
         raise NotThisMethod("unexpanded keywords, not a git-archive tarball")
-    refs = set([r.strip() for r in refnames.strip("()").split(",")])
+    refs = {r.strip() for r in refnames.strip("()").split(",")}
     # starting in git-1.8.3, tags are listed as "tag: foo-1.0" instead of
     # just "foo-1.0". If we see a "tag: " prefix, prefer those.
     TAG = "tag: "
-    tags = set([r[len(TAG):] for r in refs if r.startswith(TAG)])
+    tags = {r[len(TAG):] for r in refs if r.startswith(TAG)}
     if not tags:
         # Either we're using git < 1.8.3, or there really are no tags. We use
         # a heuristic: assume all version tags have a digit. The old git %d
         # expansion behaves like git log --decorate=short and strips out the
         # refs/heads/ and refs/tags/ prefixes that would let us distinguish
         # between branches and tags. By ignoring refnames without digits, we
         # filter out many common branch names like "release" and
         # "stabilization", as well as "HEAD" and "master".
-        tags = set([r for r in refs if re.search(r'\d', r)])
+        tags = {r for r in refs if re.search(r'\d', r)}
         if verbose:
             print("discarding '%s', no digits" % ",".join(refs - tags))
     if verbose:
         print("likely tags: %s" % ",".join(sorted(tags)))
     for ref in sorted(tags):
         # sorting will prefer e.g. "2.0" over "2.0rc1"
         if ref.startswith(tag_prefix):
             r = ref[len(tag_prefix):]
+            # Filter out refs that exactly match prefix or that don't start
+            # with a number once the prefix is stripped (mostly a concern
+            # when prefix is '')
+            if not re.match(r'\d', r):
+                continue
             if verbose:
                 print("picking %s" % r)
             return {"version": r,
                     "full-revisionid": keywords["full"].strip(),
                     "dirty": False, "error": None,
                     "date": date}
     # no suitable tags, so version is "0+unknown", but full hex is still there
@@ -1087,52 +1227,92 @@
     branch_out, rc = run_command(GITS, ["rev-parse", "--abbrev-ref", "--symbolic-full-name", "@{u}"], hide_stderr=True)
     if rc != 0:
         return "notrack"
     return branch_out
 
 
 @register_vcs_handler("git", "pieces_from_vcs")
-def git_pieces_from_vcs(tag_prefix, root, verbose, run_command=run_command):
+def git_pieces_from_vcs(tag_prefix, root, verbose, runner=run_command):
     """Get version from 'git describe' in the root of the source tree.
 
     This only gets called if the git-archive 'subst' keywords were *not*
     expanded, and _version.py hasn't already been rewritten with a short
     version string, meaning we're inside a checked out source tree.
     """
     GITS = ["git"]
     if sys.platform == "win32":
         GITS = ["git.cmd", "git.exe"]
 
-    out, rc = run_command(GITS, ["rev-parse", "--git-dir"], cwd=root,
-                          hide_stderr=True)
+    # GIT_DIR can interfere with correct operation of Versioneer.
+    # It may be intended to be passed to the Versioneer-versioned project,
+    # but that should not change where we get our version from.
+    env = os.environ.copy()
+    env.pop("GIT_DIR", None)
+    runner = functools.partial(runner, env=env)
+
+    _, rc = runner(GITS, ["rev-parse", "--git-dir"], cwd=root,
+                   hide_stderr=not verbose)
     if rc != 0:
         if verbose:
             print("Directory %s not under git control" % root)
         raise NotThisMethod("'git rev-parse --git-dir' returned error")
 
     # if there is a tag matching tag_prefix, this yields TAG-NUM-gHEX[-dirty]
     # if there isn't one, this yields HEX[-dirty] (no NUM)
-    describe_out, rc = run_command(GITS, ["describe", "--tags", "--dirty",
-                                          "--always", "--long",
-                                          "--match", "%s*" % tag_prefix],
-                                   cwd=root)
+    describe_out, rc = runner(GITS, [
+        "describe", "--tags", "--dirty", "--always", "--long",
+        "--match", "{}[[:digit:]]*".format(tag_prefix)
+    ], cwd=root)
     # --long was added in git-1.5.5
     if describe_out is None:
         raise NotThisMethod("'git describe' failed")
     describe_out = describe_out.strip()
-    full_out, rc = run_command(GITS, ["rev-parse", "HEAD"], cwd=root)
+    full_out, rc = runner(GITS, ["rev-parse", "HEAD"], cwd=root)
     if full_out is None:
         raise NotThisMethod("'git rev-parse' failed")
     full_out = full_out.strip()
 
     pieces = {}
     pieces["long"] = full_out
     pieces["short"] = full_out[:7]  # maybe improved later
     pieces["error"] = None
 
+    branch_name, rc = runner(GITS, ["rev-parse", "--abbrev-ref", "HEAD"],
+                             cwd=root)
+    # --abbrev-ref was added in git-1.6.3
+    if rc != 0 or branch_name is None:
+        raise NotThisMethod("'git rev-parse --abbrev-ref' returned error")
+    branch_name = branch_name.strip()
+
+    if branch_name == "HEAD":
+        # If we aren't exactly on a branch, pick a branch which represents
+        # the current commit. If all else fails, we are on a branchless
+        # commit.
+        branches, rc = runner(GITS, ["branch", "--contains"], cwd=root)
+        # --contains was added in git-1.5.4
+        if rc != 0 or branches is None:
+            raise NotThisMethod("'git branch --contains' returned error")
+        branches = branches.split("\n")
+
+        # Remove the first line if we're running detached
+        if "(" in branches[0]:
+            branches.pop(0)
+
+        # Strip off the leading "* " from the list of branches.
+        branches = [branch[2:] for branch in branches]
+        if "master" in branches:
+            branch_name = "master"
+        elif not branches:
+            branch_name = None
+        else:
+            # Pick the first branch that is returned. Good or bad.
+            branch_name = branches[0]
+
+    pieces["branch"] = branch_name
+
     # parse describe_out. It will be like TAG-NUM-gHEX[-dirty] or HEX[-dirty]
     # TAG might have hyphens.
     git_describe = describe_out
 
     # look for -dirty suffix
     dirty = git_describe.endswith("-dirty")
     pieces["dirty"] = dirty
@@ -1141,15 +1321,15 @@
 
     # now we have TAG-NUM-gHEX or HEX
 
     if "-" in git_describe:
         # TAG-NUM-gHEX
         mo = re.search(r'^(.+)-(\d+)-g([0-9a-f]+)$', git_describe)
         if not mo:
-            # unparseable. Maybe git-describe is misbehaving?
+            # unparsable. Maybe git-describe is misbehaving?
             pieces["error"] = ("unable to parse git-describe output: '%s'"
                                % describe_out)
             return pieces
 
         # tag
         full_tag = mo.group(1)
         if not full_tag.startswith(tag_prefix):
@@ -1166,91 +1346,91 @@
 
         # commit: short hex revision ID
         pieces["short"] = mo.group(3)
 
     else:
         # HEX: no tags
         pieces["closest-tag"] = None
-        count_out, rc = run_command(GITS, ["rev-list", "HEAD", "--count"],
-                                    cwd=root)
-        pieces["distance"] = int(count_out)  # total number of commits
+        out, rc = runner(GITS, ["rev-list", "HEAD", "--left-right"], cwd=root)
+        pieces["distance"] = len(out.split())  # total number of commits
 
     # commit date: see ISO-8601 comment in git_versions_from_keywords()
-    date = run_command(GITS, ["show", "-s", "--format=%ci", "HEAD"],
-                       cwd=root)[0].strip()
+    date = runner(GITS, ["show", "-s", "--format=%ci", "HEAD"], cwd=root)[0].strip()
+    # Use only the last line.  Previous lines may contain GPG signature
+    # information.
+    date = date.splitlines()[-1]
     pieces["date"] = date.strip().replace(" ", "T", 1).replace(" ", "", 1)
 
     return pieces
 
 
-def do_vcs_install(manifest_in, versionfile_source, ipy):
+def do_vcs_install(versionfile_source, ipy):
     """Git-specific installation logic for Versioneer.
 
     For Git, this means creating/changing .gitattributes to mark _version.py
     for export-subst keyword substitution.
     """
     GITS = ["git"]
     if sys.platform == "win32":
         GITS = ["git.cmd", "git.exe"]
-    files = [manifest_in, versionfile_source]
+    files = [versionfile_source]
     if ipy:
         files.append(ipy)
-    try:
-        me = __file__
-        if me.endswith(".pyc") or me.endswith(".pyo"):
-            me = os.path.splitext(me)[0] + ".py"
-        versioneer_file = os.path.relpath(me)
-    except NameError:
-        versioneer_file = "versioneer.py"
-    files.append(versioneer_file)
+    if "VERSIONEER_PEP518" not in globals():
+        try:
+            my_path = __file__
+            if my_path.endswith((".pyc", ".pyo")):
+                my_path = os.path.splitext(my_path)[0] + ".py"
+            versioneer_file = os.path.relpath(my_path)
+        except NameError:
+            versioneer_file = "versioneer.py"
+        files.append(versioneer_file)
     present = False
     try:
-        f = open(".gitattributes", "r")
-        for line in f.readlines():
-            if line.strip().startswith(versionfile_source):
-                if "export-subst" in line.strip().split()[1:]:
-                    present = True
-        f.close()
-    except EnvironmentError:
+        with open(".gitattributes", "r") as fobj:
+            for line in fobj:
+                if line.strip().startswith(versionfile_source):
+                    if "export-subst" in line.strip().split()[1:]:
+                        present = True
+                        break
+    except OSError:
         pass
     if not present:
-        f = open(".gitattributes", "a+")
-        f.write("%s export-subst\n" % versionfile_source)
-        f.close()
+        with open(".gitattributes", "a+") as fobj:
+            fobj.write("{} export-subst\n".format(versionfile_source))
         files.append(".gitattributes")
     run_command(GITS, ["add", "--"] + files)
 
 
 def versions_from_parentdir(parentdir_prefix, root, verbose):
     """Try to determine the version from the parent directory name.
 
     Source tarballs conventionally unpack into a directory that includes both
     the project name and a version string. We will also support searching up
     two directory levels for an appropriately named parent directory
     """
     rootdirs = []
 
-    for i in range(3):
+    for _ in range(3):
         dirname = os.path.basename(root)
         if dirname.startswith(parentdir_prefix):
             return {"version": dirname[len(parentdir_prefix):],
                     "full-revisionid": None,
                     "dirty": False, "error": None, "date": None}
-        else:
-            rootdirs.append(root)
-            root = os.path.dirname(root)  # up a level
+        rootdirs.append(root)
+        root = os.path.dirname(root)  # up a level
 
     if verbose:
         print("Tried directories %s but none started with prefix %s" %
               (str(rootdirs), parentdir_prefix))
     raise NotThisMethod("rootdir doesn't start with parentdir_prefix")
 
 
 SHORT_VERSION_PY = """
-# This file was generated by 'versioneer.py' (0.18) from
+# This file was generated by 'versioneer.py' (0.28) from
 # revision-control system data, or from the parent directory name of an
 # unpacked source archive. Distribution tarballs contain a pre-generated copy
 # of this file.
 
 import json
 
 version_json = '''
@@ -1264,15 +1444,15 @@
 
 
 def versions_from_file(filename):
     """Try to determine the version from _version.py if present."""
     try:
         with open(filename) as f:
             contents = f.read()
-    except EnvironmentError:
+    except OSError:
         raise NotThisMethod("unable to read _version.py")
     mo = re.search(r"version_json = '''\n(.*)'''  # END VERSION_JSON",
                    contents, re.M | re.S)
     if not mo:
         mo = re.search(r"version_json = '''\r\n(.*)'''  # END VERSION_JSON",
                        contents, re.M | re.S)
     if not mo:
@@ -1319,27 +1499,75 @@
         rendered = "0+untagged.%d.g%s" % (pieces["distance"],
                                           pieces["short"])
         if pieces["dirty"]:
             rendered += ".dirty"
     return rendered
 
 
-def render_pep440_pre(pieces):
-    """TAG[.post.devDISTANCE] -- No -dirty.
+def render_pep440_branch(pieces):
+    """TAG[[.dev0]+DISTANCE.gHEX[.dirty]] .
+
+    The ".dev0" means not master branch. Note that .dev0 sorts backwards
+    (a feature branch will appear "older" than the master branch).
 
     Exceptions:
-    1: no tags. 0.post.devDISTANCE
+    1: no tags. 0[.dev0]+untagged.DISTANCE.gHEX[.dirty]
     """
     if pieces["closest-tag"]:
         rendered = pieces["closest-tag"]
+        if pieces["distance"] or pieces["dirty"]:
+            if pieces["branch"] != "master":
+                rendered += ".dev0"
+            rendered += plus_or_dot(pieces)
+            rendered += "%d.g%s" % (pieces["distance"], pieces["short"])
+            if pieces["dirty"]:
+                rendered += ".dirty"
+    else:
+        # exception #1
+        rendered = "0"
+        if pieces["branch"] != "master":
+            rendered += ".dev0"
+        rendered += "+untagged.%d.g%s" % (pieces["distance"],
+                                          pieces["short"])
+        if pieces["dirty"]:
+            rendered += ".dirty"
+    return rendered
+
+
+def pep440_split_post(ver):
+    """Split pep440 version string at the post-release segment.
+
+    Returns the release segments before the post-release and the
+    post-release version number (or -1 if no post-release segment is present).
+    """
+    vc = str.split(ver, ".post")
+    return vc[0], int(vc[1] or 0) if len(vc) == 2 else None
+
+
+def render_pep440_pre(pieces):
+    """TAG[.postN.devDISTANCE] -- No -dirty.
+
+    Exceptions:
+    1: no tags. 0.post0.devDISTANCE
+    """
+    if pieces["closest-tag"]:
         if pieces["distance"]:
-            rendered += ".post.dev%d" % pieces["distance"]
+            # update the post release segment
+            tag_version, post_version = pep440_split_post(pieces["closest-tag"])
+            rendered = tag_version
+            if post_version is not None:
+                rendered += ".post%d.dev%d" % (post_version + 1, pieces["distance"])
+            else:
+                rendered += ".post0.dev%d" % (pieces["distance"])
+        else:
+            # no commits, use the tag as the version
+            rendered = pieces["closest-tag"]
     else:
         # exception #1
-        rendered = "0.post.dev%d" % pieces["distance"]
+        rendered = "0.post0.dev%d" % pieces["distance"]
     return rendered
 
 
 def render_pep440_post(pieces):
     """TAG[.postDISTANCE[.dev0]+gHEX] .
 
     The ".dev0" means dirty. Note that .dev0 sorts backwards
@@ -1362,20 +1590,41 @@
         rendered = "0.post%d" % pieces["distance"]
         if pieces["dirty"]:
             rendered += ".dev0"
         rendered += "+g%s" % pieces["short"]
     return rendered
 
 
-def debug_info():
-    root = get_root()
-    cfg = get_config_from_root(root)
-    pieces = git_pieces_from_vcs(cfg.tag_prefix, root, cfg.verbose)
-    return "Developing: %s, CurrentTag: %s, Distance: %d, Dirty: %s" % (
-        working_version(), pieces["closest-tag"], pieces["distance"], pieces["dirty"])
+def render_pep440_post_branch(pieces):
+    """TAG[.postDISTANCE[.dev0]+gHEX[.dirty]] .
+
+    The ".dev0" means not master branch.
+
+    Exceptions:
+    1: no tags. 0.postDISTANCE[.dev0]+gHEX[.dirty]
+    """
+    if pieces["closest-tag"]:
+        rendered = pieces["closest-tag"]
+        if pieces["distance"] or pieces["dirty"]:
+            rendered += ".post%d" % pieces["distance"]
+            if pieces["branch"] != "master":
+                rendered += ".dev0"
+            rendered += plus_or_dot(pieces)
+            rendered += "g%s" % pieces["short"]
+            if pieces["dirty"]:
+                rendered += ".dirty"
+    else:
+        # exception #1
+        rendered = "0.post%d" % pieces["distance"]
+        if pieces["branch"] != "master":
+            rendered += ".dev0"
+        rendered += "+g%s" % pieces["short"]
+        if pieces["dirty"]:
+            rendered += ".dirty"
+    return rendered
 
 
 def render_pep440_ricequant(pieces):
     tag = pieces["closest-tag"]
     parsed_tag = parse_version(tag) if tag else None
 
     working = working_version()
@@ -1393,54 +1642,49 @@
                 if parsed_tag._version.post[0] != "post":
                     raise Exception("Only post release tag allowed, tag %s" % tag)
                 if pieces["distance"] > 0:
                     rendered += ".post%d" % (parsed_tag._version.post[1] + 1)
                     rendered += ".dev%d" % (pieces["distance"])
                 elif pieces["distance"] == 0:
                     rendered += ".post%d" % parsed_tag._version.post[1]
-                if pieces["dirty"]:
-                    rendered += ".dirty"
             else:
                 raise Exception("Developing version can not go back in time: %s < %s" % (working, tag))
         # 如果最近的tag是正式版tag，那么就是在开发该系列的.post1
         elif parsed_working == parsed_tag:
             if pieces["distance"] > 0:
                 rendered += ".post1.dev%d" % (pieces["distance"])
-            if pieces["dirty"]:
-                rendered += ".dirty"
         # 如果正在开发到是一个新的系列，那么就从该系列的.dev0开始
         else:
             if pieces["distance"] >= 0:
                 rendered += ".dev%d" % (pieces["distance"])
-
-            if pieces["dirty"]:
-                rendered += ".dirty"
     # 没有最近的tag等价于正在开发到是一个新的系列，那么就从该系列的.dev0开始
     else:
         if pieces["distance"] >= 0:
             rendered += ".dev%d" % pieces["distance"]
 
-        if pieces["dirty"]:
-            rendered += ".dirty"
-
     tracking_branch = git_tracking_branch()
     # # 如果是dev和master分支或者hotfix分支来的，或者是一个tag，那就用pep440的版本号，否则带上git commit id
     if tracking_branch in ["origin/develop", "origin/master"] or tracking_branch.startswith("origin/hotfix/") or pieces[
         "distance"] == 0:
+        if pieces["dirty"]:
+            rendered += ".dirty"
         return rendered
-    rendered += "+{}".format(pieces["short"])
+
+    rendered += "+%s" % format(pieces["short"])
+    if pieces["dirty"]:
+        rendered += ".dirty"
     return rendered
 
 
 def render_pep440_old(pieces):
     """TAG[.postDISTANCE[.dev0]] .
 
     The ".dev0" means dirty.
 
-    Eexceptions:
+    Exceptions:
     1: no tags. 0.postDISTANCE[.dev0]
     """
     if pieces["closest-tag"]:
         rendered = pieces["closest-tag"]
         if pieces["distance"] or pieces["dirty"]:
             rendered += ".post%d" % pieces["distance"]
             if pieces["dirty"]:
@@ -1503,22 +1747,26 @@
                 "date": None}
 
     if not style or style == "default":
         style = "pep440"  # the default
 
     if style == "pep440":
         rendered = render_pep440(pieces)
+    elif style == "pep440-ricequant":
+        rendered = render_pep440_ricequant(pieces)
+    elif style == "pep440-branch":
+        rendered = render_pep440_branch(pieces)
     elif style == "pep440-pre":
         rendered = render_pep440_pre(pieces)
     elif style == "pep440-post":
         rendered = render_pep440_post(pieces)
+    elif style == "pep440-post-branch":
+        rendered = render_pep440_post_branch(pieces)
     elif style == "pep440-old":
         rendered = render_pep440_old(pieces)
-    elif style == 'pep440-ricequant':
-        rendered = render_pep440_ricequant(pieces)
     elif style == "git-describe":
         rendered = render_git_describe(pieces)
     elif style == "git-describe-long":
         rendered = render_git_describe_long(pieces)
     else:
         raise ValueError("unknown style '%s'" % style)
 
@@ -1608,35 +1856,39 @@
 
 
 def get_version():
     """Get the short version string for this project."""
     return get_versions()["version"]
 
 
-def get_cmdclass():
-    """Get the custom setuptools/distutils subclasses used by Versioneer."""
+def get_cmdclass(cmdclass=None):
+    """Get the custom setuptools subclasses used by Versioneer.
+
+    If the package uses a different cmdclass (e.g. one from numpy), it
+    should be provide as an argument.
+    """
     if "versioneer" in sys.modules:
         del sys.modules["versioneer"]
         # this fixes the "python setup.py develop" case (also 'install' and
         # 'easy_install .'), in which subdependencies of the main project are
         # built (using setup.py bdist_egg) in the same python process. Assume
         # a main project A and a dependency B, which use different versions
         # of Versioneer. A's setup.py imports A's Versioneer, leaving it in
         # sys.modules by the time B's setup.py is executed, causing B to run
         # with the wrong versioneer. Setuptools wraps the sub-dep builds in a
         # sandbox that restores sys.modules to it's pre-build state, so the
         # parent is protected against the child's "import versioneer". By
         # removing ourselves from sys.modules here, before the child build
         # happens, we protect the child from the parent's versioneer too.
-        # Also see https://github.com/warner/python-versioneer/issues/52
+        # Also see https://github.com/python-versioneer/python-versioneer/issues/52
 
-    cmds = {}
+    cmds = {} if cmdclass is None else cmdclass.copy()
 
-    # we add "version" to both distutils and setuptools
-    from distutils.core import Command
+    # we add "version" to setuptools
+    from setuptools import Command
 
     class cmd_version(Command):
         description = "report generated version string"
         user_options = []
         boolean_options = []
 
         def initialize_options(self):
@@ -1649,54 +1901,91 @@
             vers = get_versions(verbose=True)
             print("Version: %s" % vers["version"])
             print(" full-revisionid: %s" % vers.get("full-revisionid"))
             print(" dirty: %s" % vers.get("dirty"))
             print(" date: %s" % vers.get("date"))
             if vers["error"]:
                 print(" error: %s" % vers["error"])
-
     cmds["version"] = cmd_version
 
-    # we override "build_py" in both distutils and setuptools
+    # we override "build_py" in setuptools
     #
     # most invocation pathways end up running build_py:
     #  distutils/build -> build_py
     #  distutils/install -> distutils/build ->..
     #  setuptools/bdist_wheel -> distutils/install ->..
     #  setuptools/bdist_egg -> distutils/install_lib -> build_py
     #  setuptools/install -> bdist_egg ->..
     #  setuptools/develop -> ?
     #  pip install:
     #   copies source tree to a tempdir before running egg_info/etc
     #   if .git isn't copied too, 'git describe' will fail
     #   then does setup.py bdist_wheel, or sometimes setup.py install
     #  setup.py egg_info -> ?
 
+    # pip install -e . and setuptool/editable_wheel will invoke build_py
+    # but the build_py command is not expected to copy any files.
+
     # we override different "build_py" commands for both environments
-    if "setuptools" in sys.modules:
-        from setuptools.command.build_py import build_py as _build_py
+    if 'build_py' in cmds:
+        _build_py = cmds['build_py']
     else:
-        from distutils.command.build_py import build_py as _build_py
+        from setuptools.command.build_py import build_py as _build_py
 
     class cmd_build_py(_build_py):
         def run(self):
             root = get_root()
             cfg = get_config_from_root(root)
             versions = get_versions()
             _build_py.run(self)
+            if getattr(self, "editable_mode", False):
+                # During editable installs `.py` and data files are
+                # not copied to build_lib
+                return
             # now locate _version.py in the new build/ directory and replace
             # it with an updated value
             if cfg.versionfile_build:
                 target_versionfile = os.path.join(self.build_lib,
                                                   cfg.versionfile_build)
                 print("UPDATING %s" % target_versionfile)
                 write_to_version_file(target_versionfile, versions)
-
     cmds["build_py"] = cmd_build_py
 
+    if 'build_ext' in cmds:
+        _build_ext = cmds['build_ext']
+    else:
+        from setuptools.command.build_ext import build_ext as _build_ext
+
+    class cmd_build_ext(_build_ext):
+        def run(self):
+            root = get_root()
+            cfg = get_config_from_root(root)
+            versions = get_versions()
+            _build_ext.run(self)
+            if self.inplace:
+                # build_ext --inplace will only build extensions in
+                # build/lib<..> dir with no _version.py to write to.
+                # As in place builds will already have a _version.py
+                # in the module dir, we do not need to write one.
+                return
+            # now locate _version.py in the new build/ directory and replace
+            # it with an updated value
+            if not cfg.versionfile_build:
+                return
+            target_versionfile = os.path.join(self.build_lib,
+                                              cfg.versionfile_build)
+            if not os.path.exists(target_versionfile):
+                print("Warning: {} does not exist, skipping "
+                      "version update. This can happen if you are running build_ext "
+                      "without first running build_py.".format(target_versionfile))
+                return
+            print("UPDATING %s" % target_versionfile)
+            write_to_version_file(target_versionfile, versions)
+    cmds["build_ext"] = cmd_build_ext
+
     if "cx_Freeze" in sys.modules:  # cx_freeze enabled?
         from cx_Freeze.dist import build_exe as _build_exe
         # nczeczulin reports that py2exe won't like the pep440-style string
         # as FILEVERSION, but it can be used for PRODUCTVERSION, e.g.
         # setup(console=[{
         #   "version": versioneer.get_version().split("+", 1)[0], # FILEVERSION
         #   "product_version": versioneer.get_version(),
@@ -1718,23 +2007,22 @@
                     f.write(LONG %
                             {"DOLLAR": "$",
                              "STYLE": cfg.style,
                              "TAG_PREFIX": cfg.tag_prefix,
                              "PARENTDIR_PREFIX": cfg.parentdir_prefix,
                              "VERSIONFILE_SOURCE": cfg.versionfile_source,
                              })
-
         cmds["build_exe"] = cmd_build_exe
         del cmds["build_py"]
 
     if 'py2exe' in sys.modules:  # py2exe enabled?
         try:
-            from py2exe.distutils_buildexe import py2exe as _py2exe  # py3
+            from py2exe.setuptools_buildexe import py2exe as _py2exe
         except ImportError:
-            from py2exe.build_exe import py2exe as _py2exe  # py2
+            from py2exe.distutils_buildexe import py2exe as _py2exe
 
         class cmd_py2exe(_py2exe):
             def run(self):
                 root = get_root()
                 cfg = get_config_from_root(root)
                 versions = get_versions()
                 target_versionfile = cfg.versionfile_source
@@ -1748,22 +2036,58 @@
                     f.write(LONG %
                             {"DOLLAR": "$",
                              "STYLE": cfg.style,
                              "TAG_PREFIX": cfg.tag_prefix,
                              "PARENTDIR_PREFIX": cfg.parentdir_prefix,
                              "VERSIONFILE_SOURCE": cfg.versionfile_source,
                              })
-
         cmds["py2exe"] = cmd_py2exe
 
+    # sdist farms its file list building out to egg_info
+    if 'egg_info' in cmds:
+        _egg_info = cmds['egg_info']
+    else:
+        from setuptools.command.egg_info import egg_info as _egg_info
+
+    class cmd_egg_info(_egg_info, object):
+        def find_sources(self):
+            # egg_info.find_sources builds the manifest list and writes it
+            # in one shot
+            super(cmd_egg_info, self).find_sources()
+
+            # Modify the filelist and normalize it
+            root = get_root()
+            cfg = get_config_from_root(root)
+            self.filelist.append('versioneer.py')
+            if cfg.versionfile_source:
+                # There are rare cases where versionfile_source might not be
+                # included by default, so we must be explicit
+                self.filelist.append(cfg.versionfile_source)
+            self.filelist.sort()
+            self.filelist.remove_duplicates()
+
+            # The write method is hidden in the manifest_maker instance that
+            # generated the filelist and was thrown away
+            # We will instead replicate their final normalization (to unicode,
+            # and POSIX-style paths)
+            from setuptools import unicode_utils
+            normalized = [unicode_utils.filesys_decode(f).replace(os.sep, '/')
+                          for f in self.filelist.files]
+
+            manifest_filename = os.path.join(self.egg_info, 'SOURCES.txt')
+            with open(manifest_filename, 'w') as fobj:
+                fobj.write('\n'.join(normalized))
+
+    cmds['egg_info'] = cmd_egg_info
+
     # we override different "sdist" commands for both environments
-    if "setuptools" in sys.modules:
-        from setuptools.command.sdist import sdist as _sdist
+    if 'sdist' in cmds:
+        _sdist = cmds['sdist']
     else:
-        from distutils.command.sdist import sdist as _sdist
+        from setuptools.command.sdist import sdist as _sdist
 
     class cmd_sdist(_sdist):
         def run(self):
             versions = get_versions()
             self._versioneer_generated_versions = versions
             # unless we update this, the command will keep using the old
             # version
@@ -1777,15 +2101,14 @@
             # now locate _version.py in the new base_dir directory
             # (remembering that it may be a hardlink) and replace it with an
             # updated value
             target_versionfile = os.path.join(base_dir, cfg.versionfile_source)
             print("UPDATING %s" % target_versionfile)
             write_to_version_file(target_versionfile,
                                   self._versioneer_generated_versions)
-
     cmds["sdist"] = cmd_sdist
 
     return cmds
 
 
 CONFIG_ERROR = """
 setup.cfg is missing the necessary Versioneer configuration. You need
@@ -1820,34 +2143,38 @@
 #versionfile_source =
 #versionfile_build =
 #tag_prefix =
 #parentdir_prefix =
 
 """
 
-INIT_PY_SNIPPET = """
+OLD_SNIPPET = """
 from ._version import get_versions
 __version__ = get_versions()['version']
 del get_versions
 """
 
+INIT_PY_SNIPPET = """
+from . import {0}
+__version__ = {0}.get_versions()['version']
+"""
+
 
 def do_setup():
-    """Main VCS-independent setup function for installing Versioneer."""
+    """Do main VCS-independent setup function for installing Versioneer."""
     root = get_root()
     try:
         cfg = get_config_from_root(root)
-    except (EnvironmentError, configparser.NoSectionError,
+    except (OSError, configparser.NoSectionError,
             configparser.NoOptionError) as e:
-        if isinstance(e, (EnvironmentError, configparser.NoSectionError)):
-            print("Adding sample versioneer config to setup.cfg",
-                  file=sys.stderr)
+        if isinstance(e, (OSError, configparser.NoSectionError)):
+            print("Adding sample versioneer config to setup.cfg")
             with open(os.path.join(root, "setup.cfg"), "a") as f:
                 f.write(SAMPLE_CONFIG)
-        print(CONFIG_ERROR, file=sys.stderr)
+        print(CONFIG_ERROR)
         return 1
 
     print(" creating %s" % cfg.versionfile_source)
     with open(cfg.versionfile_source, "w") as f:
         LONG = LONG_VERSION_PY[cfg.VCS]
         f.write(LONG % {"DOLLAR": "$",
                         "STYLE": cfg.style,
@@ -1858,62 +2185,36 @@
 
     ipy = os.path.join(os.path.dirname(cfg.versionfile_source),
                        "__init__.py")
     if os.path.exists(ipy):
         try:
             with open(ipy, "r") as f:
                 old = f.read()
-        except EnvironmentError:
+        except OSError:
             old = ""
-        if INIT_PY_SNIPPET not in old:
+        module = os.path.splitext(os.path.basename(cfg.versionfile_source))[0]
+        snippet = INIT_PY_SNIPPET.format(module)
+        if OLD_SNIPPET in old:
+            print(" replacing boilerplate in %s" % ipy)
+            with open(ipy, "w") as f:
+                f.write(old.replace(OLD_SNIPPET, snippet))
+        elif snippet not in old:
             print(" appending to %s" % ipy)
             with open(ipy, "a") as f:
-                f.write(INIT_PY_SNIPPET)
+                f.write(snippet)
         else:
             print(" %s unmodified" % ipy)
     else:
         print(" %s doesn't exist, ok" % ipy)
         ipy = None
 
-    # Make sure both the top-level "versioneer.py" and versionfile_source
-    # (PKG/_version.py, used by runtime code) are in MANIFEST.in, so
-    # they'll be copied into source distributions. Pip won't be able to
-    # install the package without this.
-    manifest_in = os.path.join(root, "MANIFEST.in")
-    simple_includes = set()
-    try:
-        with open(manifest_in, "r") as f:
-            for line in f:
-                if line.startswith("include "):
-                    for include in line.split()[1:]:
-                        simple_includes.add(include)
-    except EnvironmentError:
-        pass
-    # That doesn't cover everything MANIFEST.in can do
-    # (http://docs.python.org/2/distutils/sourcedist.html#commands), so
-    # it might give some false negatives. Appending redundant 'include'
-    # lines is safe, though.
-    if "versioneer.py" not in simple_includes:
-        print(" appending 'versioneer.py' to MANIFEST.in")
-        with open(manifest_in, "a") as f:
-            f.write("include versioneer.py\n")
-    else:
-        print(" 'versioneer.py' already in MANIFEST.in")
-    if cfg.versionfile_source not in simple_includes:
-        print(" appending versionfile_source ('%s') to MANIFEST.in" %
-              cfg.versionfile_source)
-        with open(manifest_in, "a") as f:
-            f.write("include %s\n" % cfg.versionfile_source)
-    else:
-        print(" versionfile_source already in MANIFEST.in")
-
     # Make VCS-specific changes. For git, this means creating/changing
     # .gitattributes to mark _version.py for export-subst keyword
     # substitution.
-    do_vcs_install(manifest_in, cfg.versionfile_source, ipy)
+    do_vcs_install(cfg.versionfile_source, ipy)
     return 0
 
 
 def scan_setup_py():
     """Validate the contents of setup.py against Versioneer's expectations."""
     found = set()
     setters = False
@@ -1946,19 +2247,26 @@
         print("'versioneer.versionfile_source = ' . This configuration")
         print("now lives in setup.cfg, and should be removed from setup.py")
         print("")
         errors += 1
     return errors
 
 
+def setup_command():
+    """Set up Versioneer and exit with appropriate error code."""
+    errors = do_setup()
+    errors += scan_setup_py()
+    sys.exit(1 if errors else 0)
+
+
 def get_metadata():
     setup_cfg = os.path.join(get_root(), "setup.cfg")
-    parser = configparser.SafeConfigParser()
+    parser = configparser.RawConfigParser()
     with open(setup_cfg, "r") as f:
-        parser.readfp(f)
+        parser.read_file(f)
 
     def get(section, parser, name):
         if parser.has_option(section, name):
             return parser.get(section, name)
         return None
 
     return {
@@ -1970,154 +2278,11 @@
 def package_name():
     return get_metadata()["name"]
 
 
 def working_version():
     return get_metadata()["version"]
 
-
-def next_tag_name():
-    root = get_root()
-    cfg = get_config_from_root(root)
-    pieces = git_pieces_from_vcs(cfg.tag_prefix, root, cfg.verbose)
-
-    tag = pieces["closest-tag"]
-    parsed_tag = parse_version(tag) if tag else None
-
-    working = working_version()
-    parsed_working = parse_version(working)
-
-    rendered = working
-
-    curr_version = get_version()
-    parsed_curr_version = parse_version(curr_version)
-
-    if tag:
-        # 如果当前开发系列正式版小于最近的tag，那么当前开发系列和该tag必须属于同一个开发版本系列
-        # 当前开发都没有做完，大于当前开发系列的tag不可能存
-        # 因为大于当前开发系列的正式版, 该tag必然是post release
-        # 如果发现当前commit和最近的tag的commit相同，规定next tag不变. 这也限制只有最近tag后的第一个commit存在，
-        # 才会获取到next tag name
-        if parsed_working < parsed_tag:
-            if parsed_working.base_version == parsed_tag.base_version:
-                if not parsed_tag.is_postrelease:
-                    raise Exception("Only post release tag allowed, tag %s" % tag)
-                if parsed_tag._version.post[0] != "post":
-                    raise Exception("Only post release tag allowed, tag %s" % tag)
-                # 正在开发的版本不可能小于等于最近的tag
-                if parsed_curr_version <= parsed_tag:
-                    raise Exception("Current version %s should > latest tag %s" % (curr_version, tag))
-                if pieces["distance"] == 0:
-                    return tag
-
-                rendered += ".post%d" % parsed_curr_version._version.post[1]
-            else:
-                raise Exception(
-                    "Developing version can not go back in time: %s(working version series) < %s(latest tag)" % working,
-                    tag)
-        # 如果当前开发系列的正式版等于最近的tag，那么下一个tag必定是.post1
-        elif parsed_working == parsed_tag:
-            if parsed_curr_version._version.post[0] != "post":
-                raise Exception("Current version should be a post version %s" % curr_version)
-            rendered += ".post%d" % parsed_curr_version._version.post[1]
-
-    # 如果当前开发版本系列正式版大于最近的tag，那么下一个的tag将是当前开发系列的正式版tag
-    return rendered
-
-
-def is_same_package(package_file):
-    curr_version = get_versions()
-    v = _get_version_py_in_tar(package_file)
-    if not v:
-        v = _get_version_py_in_zip(package_file)
-    if not v:
-        raise Exception("Can not get _version.py from %s" % package_file)
-
-    from types import ModuleType
-    m = ModuleType("get_versions")
-    exec(v, m.__dict__)
-    version_info = m.get_versions()
-    return curr_version["full-revisionid"] == version_info["full-revisionid"]
-
-
-def _get_package_dir():
-    package = None
-    for d in os.listdir():
-        if os.path.isdir(d):
-            if "__init__.py" in os.listdir(d):
-                package = d
-    return package
-
-
-def _get_version_py_in_zip(package_file):
-    import zipfile
-    package_dir = _get_package_dir()
-
-    if zipfile.is_zipfile(package_file):
-        f = zipfile.ZipFile(package_file)
-        il = f.infolist()
-        if len(il) == 0:
-            raise Exception("No member found in %s" % package_file)
-        for i in il:
-            if i.filename == os.path.join(package_dir, "_version.py"):
-                return f.open(i).read()
-    return None
-
-
-def _get_version_py_in_tar(package_file):
-    import tarfile
-    package_dir = _get_package_dir()
-    if tarfile.is_tarfile(package_file):
-        f = tarfile.open(package_file)
-        ms = f.getmembers()
-        if len(ms) == 0:
-            raise Exception("No members found in %s" % package_file)
-        for m in ms:
-            if os.path.join(ms[0].name, package_dir, "_version.py") == m.path:
-                version_file = f.extractfile(m)
-                return version_file.read()
-    return None
-
-
-def get_package_name_in_pypi(version=None):
-    from pip._internal.commands.install import InstallCommand
-    from pip._internal.cli.cmdoptions import make_target_python
-
-    class ListVersionCommand(InstallCommand):
-        def __init__(self, name, summary):
-            super().__init__(name, summary)
-
-        def get_version_list(self):
-            with self.main_context():
-                options, args = self.parse_args([package_name()])
-                session = self.get_default_session(options=options)
-                target_python = make_target_python(options)
-                finder = self._build_package_finder(
-                    options=options,
-                    session=session,
-                    target_python=target_python,
-                    ignore_requires_python=options.ignore_requires_python,
-                )
-                versions = {}
-                for c in finder.find_all_candidates(package_name()):
-                    v = str(c.version)
-                    f = c.link.filename
-                    if (v in versions and f.endswith(".whl")) or v not in versions:
-                        versions[v] = f
-                return versions
-
-    if not version:
-        version = get_version()
-    c = ListVersionCommand("listversion", summary="list versions")
-    versions = c.get_version_list()
-    return versions.get(version, "")
-
-
 if __name__ == "__main__":
     cmd = sys.argv[1]
     if cmd == "setup":
-        errors = do_setup()
-        errors += scan_setup_py()
-        if errors:
-            sys.exit(1)
-    elif cmd == "is_pypi_has":
-        get_package_name_in_pypi(sys.argv[2])
+        setup_command()
```

