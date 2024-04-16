# Comparing `tmp/limexhub-0.1.8.tar.gz` & `tmp/limexhub-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "limexhub-0.1.8.tar", last modified: Wed Apr 10 13:07:37 2024, max compression
+gzip compressed data, was "limexhub-0.1.9.tar", last modified: Mon Apr 15 14:52:26 2024, max compression
```

## Comparing `limexhub-0.1.8.tar` & `limexhub-0.1.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 vyacheslav   (501) staff       (20)        0 2024-04-10 13:07:37.869740 limexhub-0.1.8/
--rw-r--r--   0 vyacheslav   (501) staff       (20)    11357 2024-02-29 12:40:33.000000 limexhub-0.1.8/LICENSE
--rw-r--r--   0 vyacheslav   (501) staff       (20)     2883 2024-04-10 13:07:37.869617 limexhub-0.1.8/PKG-INFO
--rw-r--r--   0 vyacheslav   (501) staff       (20)     2431 2024-04-09 08:51:04.000000 limexhub-0.1.8/README.md
-drwxr-xr-x   0 vyacheslav   (501) staff       (20)        0 2024-04-10 13:07:37.868845 limexhub-0.1.8/limexhub/
--rw-r--r--   0 vyacheslav   (501) staff       (20)       28 2024-04-09 08:46:30.000000 limexhub-0.1.8/limexhub/__init__.py
--rw-r--r--   0 vyacheslav   (501) staff       (20)     3400 2024-04-10 13:06:25.000000 limexhub-0.1.8/limexhub/restapi.py
-drwxr-xr-x   0 vyacheslav   (501) staff       (20)        0 2024-04-10 13:07:37.869453 limexhub-0.1.8/limexhub.egg-info/
--rw-r--r--   0 vyacheslav   (501) staff       (20)     2883 2024-04-10 13:07:37.000000 limexhub-0.1.8/limexhub.egg-info/PKG-INFO
--rw-r--r--   0 vyacheslav   (501) staff       (20)      226 2024-04-10 13:07:37.000000 limexhub-0.1.8/limexhub.egg-info/SOURCES.txt
--rw-r--r--   0 vyacheslav   (501) staff       (20)        1 2024-04-10 13:07:37.000000 limexhub-0.1.8/limexhub.egg-info/dependency_links.txt
--rw-r--r--   0 vyacheslav   (501) staff       (20)        9 2024-04-10 13:07:37.000000 limexhub-0.1.8/limexhub.egg-info/requires.txt
--rw-r--r--   0 vyacheslav   (501) staff       (20)        9 2024-04-10 13:07:37.000000 limexhub-0.1.8/limexhub.egg-info/top_level.txt
--rw-r--r--   0 vyacheslav   (501) staff       (20)       38 2024-04-10 13:07:37.869781 limexhub-0.1.8/setup.cfg
--rw-r--r--   0 vyacheslav   (501) staff       (20)      698 2024-04-10 13:06:34.000000 limexhub-0.1.8/setup.py
+drwxr-xr-x   0 vyacheslav   (501) staff       (20)        0 2024-04-15 14:52:26.194786 limexhub-0.1.9/
+-rw-r--r--   0 vyacheslav   (501) staff       (20)    11357 2024-02-29 12:40:33.000000 limexhub-0.1.9/LICENSE
+-rw-r--r--   0 vyacheslav   (501) staff       (20)     2883 2024-04-15 14:52:26.194656 limexhub-0.1.9/PKG-INFO
+-rw-r--r--   0 vyacheslav   (501) staff       (20)     2431 2024-04-09 08:51:04.000000 limexhub-0.1.9/README.md
+drwxr-xr-x   0 vyacheslav   (501) staff       (20)        0 2024-04-15 14:52:26.193841 limexhub-0.1.9/limexhub/
+-rw-r--r--   0 vyacheslav   (501) staff       (20)       28 2024-04-09 08:46:30.000000 limexhub-0.1.9/limexhub/__init__.py
+-rw-r--r--   0 vyacheslav   (501) staff       (20)     3494 2024-04-15 14:51:31.000000 limexhub-0.1.9/limexhub/restapi.py
+drwxr-xr-x   0 vyacheslav   (501) staff       (20)        0 2024-04-15 14:52:26.194477 limexhub-0.1.9/limexhub.egg-info/
+-rw-r--r--   0 vyacheslav   (501) staff       (20)     2883 2024-04-15 14:52:26.000000 limexhub-0.1.9/limexhub.egg-info/PKG-INFO
+-rw-r--r--   0 vyacheslav   (501) staff       (20)      226 2024-04-15 14:52:26.000000 limexhub-0.1.9/limexhub.egg-info/SOURCES.txt
+-rw-r--r--   0 vyacheslav   (501) staff       (20)        1 2024-04-15 14:52:26.000000 limexhub-0.1.9/limexhub.egg-info/dependency_links.txt
+-rw-r--r--   0 vyacheslav   (501) staff       (20)        9 2024-04-15 14:52:26.000000 limexhub-0.1.9/limexhub.egg-info/requires.txt
+-rw-r--r--   0 vyacheslav   (501) staff       (20)        9 2024-04-15 14:52:26.000000 limexhub-0.1.9/limexhub.egg-info/top_level.txt
+-rw-r--r--   0 vyacheslav   (501) staff       (20)       38 2024-04-15 14:52:26.194831 limexhub-0.1.9/setup.cfg
+-rw-r--r--   0 vyacheslav   (501) staff       (20)      698 2024-04-15 14:45:08.000000 limexhub-0.1.9/setup.py
```

### Comparing `limexhub-0.1.8/LICENSE` & `limexhub-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `limexhub-0.1.8/PKG-INFO` & `limexhub-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: limexhub
-Version: 0.1.8
+Version: 0.1.9
 Summary: A simple API wrapper for Limex DataHub
 Home-page: https://github.com/Limex-com/limexhub-python
 Author: V.Arbuzov
 Author-email: varbuzov@limex.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `limexhub-0.1.8/README.md` & `limexhub-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `limexhub-0.1.8/limexhub/restapi.py` & `limexhub-0.1.9/limexhub/restapi.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,15 +24,17 @@
         endpoint = "candles"
         params = {'symbol': symbol, 'from': from_date, 'to': to_date, 'timeframe': timeframe}
         res = pd.DataFrame(self._get(endpoint, params=params))
         if timeframe>=3:
             res['ts'] = pd.to_datetime(res['ts'], utc=True).dt.date
         else:
             res['ts'] = pd.to_datetime(res['ts'], utc=True)
-        return res.sort_values(by=['ts'])
+        res = res.sort_values(by=['ts'])
+        res = res.set_index('ts')
+        return res
    
     def fundamental(self, symbol, from_date='2020-01-01',to_date=datetime.today().strftime('%Y-%m-%d'), fields='ebitda'):
         endpoint = "fundamental"
         params = {'symbol': symbol, 'from': from_date,'to': to_date, 'fields': fields}
         res = pd.DataFrame(self._get(endpoint, params=params))
         res['date'] = pd.to_datetime(res['date'], utc=True).dt.date
         return res
@@ -52,14 +54,15 @@
         return res
    
     def signals(self, vendor, model, symbol, from_date='2020-01-01',to_date=datetime.today().strftime('%Y-%m-%d')):
         endpoint = "signals"
         params = {'vendor': vendor, 'model': model, 'symbol': symbol, 'from': from_date,'to': to_date}
         res = pd.DataFrame(self._get(endpoint, params=params))
         res['trade_date'] = pd.to_datetime(res['trade_date'], utc=True).dt.date
+        res = res.set_index('trade_date')
         return res
  
     def models(self, vendor='boosted'):
         endpoint = "models"
         params = {'vendor': vendor}
         return self._get(endpoint, params=params)
```

### Comparing `limexhub-0.1.8/limexhub.egg-info/PKG-INFO` & `limexhub-0.1.9/limexhub.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: limexhub
-Version: 0.1.8
+Version: 0.1.9
 Summary: A simple API wrapper for Limex DataHub
 Home-page: https://github.com/Limex-com/limexhub-python
 Author: V.Arbuzov
 Author-email: varbuzov@limex.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `limexhub-0.1.8/setup.py` & `limexhub-0.1.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
  
 setup(
     name='limexhub',
-    version='0.1.8',
+    version='0.1.9',
     packages=find_packages(),
     include_package_data=True,
     description='A simple API wrapper for Limex DataHub',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/Limex-com/limexhub-python',
     author='V.Arbuzov',
```

