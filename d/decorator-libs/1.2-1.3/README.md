# Comparing `tmp/decorator_libs-1.2.tar.gz` & `tmp/decorator_libs-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\decorator_libs-1.2.tar", last modified: Tue Nov  3 02:06:19 2020, max compression
+gzip compressed data, was "dist\decorator_libs-1.3.tar", last modified: Tue Apr 16 03:33:07 2024, max compression
```

## Comparing `decorator_libs-1.2.tar` & `decorator_libs-1.3.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxrwxrwx   0        0        0        0 2020-11-03 02:06:19.000000 decorator_libs-1.2/
-drwxrwxrwx   0        0        0        0 2020-11-03 02:06:19.000000 decorator_libs-1.2/decorator_libs/
--rw-rw-rw-   0        0        0     6033 2020-05-14 04:25:55.000000 decorator_libs-1.2/decorator_libs/black_technology_decorators.py
--rw-rw-rw-   0        0        0    16178 2020-05-14 02:18:32.000000 decorator_libs-1.2/decorator_libs/common_decorators.py
--rw-rw-rw-   0        0        0     2628 2020-05-14 02:05:27.000000 decorator_libs-1.2/decorator_libs/function_timeout_decorators.py
--rw-rw-rw-   0        0        0      258 2020-08-03 02:31:13.000000 decorator_libs-1.2/decorator_libs/__init__.py
-drwxrwxrwx   0        0        0        0 2020-11-03 02:06:19.000000 decorator_libs-1.2/decorator_libs.egg-info/
--rw-rw-rw-   0        0        0        1 2020-11-03 02:06:18.000000 decorator_libs-1.2/decorator_libs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     1327 2020-11-03 02:06:18.000000 decorator_libs-1.2/decorator_libs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       54 2020-11-03 02:06:18.000000 decorator_libs-1.2/decorator_libs.egg-info/requires.txt
--rw-rw-rw-   0        0        0      362 2020-11-03 02:06:18.000000 decorator_libs-1.2/decorator_libs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       15 2020-11-03 02:06:18.000000 decorator_libs-1.2/decorator_libs.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1327 2020-11-03 02:06:19.000000 decorator_libs-1.2/PKG-INFO
--rw-rw-rw-   0        0        0      445 2020-08-03 02:31:30.000000 decorator_libs-1.2/README.md
--rw-rw-rw-   0        0        0       42 2020-11-03 02:06:19.000000 decorator_libs-1.2/setup.cfg
--rw-rw-rw-   0        0        0     1854 2020-11-03 02:05:51.000000 decorator_libs-1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-16 03:33:07.000000 decorator_libs-1.3/
+-rw-rw-rw-   0        0        0     1171 2024-04-16 03:33:07.000000 decorator_libs-1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      445 2024-04-16 03:19:09.000000 decorator_libs-1.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-16 03:33:07.000000 decorator_libs-1.3/decorator_libs/
+-rw-rw-rw-   0        0        0      258 2024-04-16 03:19:09.000000 decorator_libs-1.3/decorator_libs/__init__.py
+-rw-rw-rw-   0        0        0     6033 2024-04-16 03:19:09.000000 decorator_libs-1.3/decorator_libs/black_technology_decorators.py
+-rw-rw-rw-   0        0        0    18870 2024-04-16 03:32:58.000000 decorator_libs-1.3/decorator_libs/common_decorators.py
+-rw-rw-rw-   0        0        0     2628 2024-04-16 03:19:09.000000 decorator_libs-1.3/decorator_libs/function_timeout_decorators.py
+drwxrwxrwx   0        0        0        0 2024-04-16 03:33:07.000000 decorator_libs-1.3/decorator_libs.egg-info/
+-rw-rw-rw-   0        0        0     1171 2024-04-16 03:33:06.000000 decorator_libs-1.3/decorator_libs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      384 2024-04-16 03:33:07.000000 decorator_libs-1.3/decorator_libs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-16 03:33:06.000000 decorator_libs-1.3/decorator_libs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2024-04-16 03:33:06.000000 decorator_libs-1.3/decorator_libs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-04-16 03:33:06.000000 decorator_libs-1.3/decorator_libs.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-16 03:33:07.000000 decorator_libs-1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1854 2024-04-16 03:32:58.000000 decorator_libs-1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-16 03:33:07.000000 decorator_libs-1.3/tests/
+-rw-rw-rw-   0        0        0      149 2024-04-16 03:19:09.000000 decorator_libs-1.3/tests/test_snooper.py
```

### Comparing `decorator_libs-1.2/decorator_libs/black_technology_decorators.py` & `decorator_libs-1.3/decorator_libs/black_technology_decorators.py`

 * *Files identical despite different names*

### Comparing `decorator_libs-1.2/decorator_libs/common_decorators.py` & `decorator_libs-1.3/decorator_libs/common_decorators.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,27 @@
 # coding=utf-8
 """
 这里面是常规的装饰器，实现简单
 """
 
-import base64
 import copy
-import random
 import warnings
 from multiprocessing import Process
-
-from contextlib import contextmanager
+import uuid
 import functools
-import json
 import os
 import sys
 import threading
 import time
 import traceback
 import unittest
 from functools import wraps
 from flask import request as flask_request
 
-from nb_log import LogManager, nb_print
+from nb_log import LogManager, nb_print, LoggerMixin
 
 os_name = os.name
 handle_exception_log = LogManager('function_error').get_logger_and_add_handlers()
 run_times_log = LogManager('run_many_times').get_logger_and_add_handlers(20)
 
 
 class CustomException(Exception):
@@ -143,15 +139,15 @@
     def lock_func(*args, **kwargs):
         with func.__lock__:
             return func(*args, **kwargs)
 
     return lock_func
 
 
-def singleton(cls):
+def singleton(cls):  # 代码补全不好
     """
     单例模式装饰器,新加入线程锁，更牢固的单例模式，主要解决多线程如100线程同时实例化情况下可能会出现三例四例的情况,实测。
     """
     _instance = {}
     singleton.__lock = threading.Lock()
 
     @wraps(cls)
@@ -160,14 +156,53 @@
             if cls not in _instance:
                 _instance[cls] = cls(*args, **kwargs)
             return _instance[cls]
 
     return _singleton
 
 
+class SingletonMeta(type):
+    _instances = {}
+
+    def __call__(cls, *args, **kwargs):
+        if cls not in cls._instances:
+            cls._instances[cls] = super().__call__(*args, **kwargs)
+        return cls._instances[cls]
+
+class SingletonBaseCall(metaclass=SingletonMeta):
+    """
+    单例基类。任何继承自这个基类的子类都会自动成为单例。
+
+    示例：
+    class MyClass(SingletonBase):
+        pass
+
+    instance1 = MyClass()
+    instance2 = MyClass()
+
+    assert instance1 is instance2  # 实例1和实例2实际上是同一个对象
+    """
+
+    def __init_subclass__(cls, **kwargs):
+        super().__init_subclass__(**kwargs)
+        # 可以在此处添加对子类的额外处理，比如检查其是否符合单例要求等
+
+
+class SingletonBaseNew:
+    _instance = None
+
+    def __new__(cls, *args, **kwargs):
+        if not cls._instance:
+            cls._instance = super().__new__(cls)
+        return cls._instance
+
+    def __init_subclass__(cls, **kwargs):
+        super().__init_subclass__(**kwargs)
+        # 可以在此处添加对子类的额外处理，比如检查其是否符合单例要求等
+
 def flyweight(cls):
     _instance = {}
 
     def _make_arguments_to_key(args, kwds):
         key = args
         if kwds:
             sorted_items = sorted(kwds.items())
@@ -295,20 +330,18 @@
             def __cached_function_result_for_a_time(*args, **kwargs):
                 # print(cls.func_result_dict)
                 # if len(cls.func_result_dict) > 1024:
                 if sys.getsizeof(cls.func_result_dict) > 100 * 1000 * 1000:
                     cls.func_result_dict.clear()
 
                 key = cls._make_arguments_to_key(args, kwargs)
-                if (fun, key) in cls.func_result_dict and time.time() - cls.func_result_dict[(fun, key)][
-                    1] < cache_time:
+                if (fun, key) in cls.func_result_dict and time.time() - cls.func_result_dict[(fun, key)][1] < cache_time:
                     return cls.func_result_dict[(fun, key)][0]
                 else:
-                    if (fun, key) in cls.func_result_dict and time.time() - cls.func_result_dict[(fun, key)][
-                        1] < cache_time:
+                    if (fun, key) in cls.func_result_dict and time.time() - cls.func_result_dict[(fun, key)][1] < cache_time:
                         return cls.func_result_dict[(fun, key)][0]
                     else:
                         cls.logger.debug('函数 [{}] 此次不能使用缓存'.format(fun.__name__))
                         result = fun(*args, **kwargs)
                         cls.func_result_dict[(fun, key)] = (result, time.time())
                         return result
 
@@ -334,14 +367,50 @@
         warnings.warn(fn.__doc__.split('\n')[0],
                       category=DeprecationWarning, stacklevel=2)
         return fn(*args, **kwargs)
 
     return wrapper
 
 
+class RedisDistributedLockContextManager(LoggerMixin):
+    """
+    分布式redis锁上下文管理.
+    """
+
+    def __init__(self, redis_client, redis_lock_key, expire_seconds=30):
+        self.redis_client = redis_client
+        self.redis_lock_key = redis_lock_key
+        self._expire_seconds = expire_seconds
+        self.identifier = str(uuid.uuid4())
+        self.has_aquire_lock = False
+
+    # noinspection PyProtectedMember,PyUnresolvedReferences
+    def __enter__(self):
+        self._line = sys._getframe().f_back.f_lineno  # 调用此方法的代码的函数
+        self._file_name = sys._getframe(1).f_code.co_filename  # 哪个文件调了用此方法
+        self.redis_client.set(self.redis_lock_key, value=self.identifier, ex=self._expire_seconds, nx=True)
+        identifier_in_redis = self.redis_client.get(self.redis_lock_key)
+        if identifier_in_redis and identifier_in_redis.decode() == self.identifier:
+            self.has_aquire_lock = True
+        return self
+
+    def __bool__(self):
+        return self.has_aquire_lock
+
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        if self.has_aquire_lock:
+            self.redis_client.delete(self.redis_lock_key)
+        if self.has_aquire_lock:
+            log_msg = f'\n"{self._file_name}:{self._line}" 这行代码获得了redis锁 {self.redis_lock_key}'
+            self.logger.info(log_msg)
+        else:
+            log_msg = f'\n"{self._file_name}:{self._line}" 这行代码没有获得redis锁 {self.redis_lock_key}'
+            self.logger.warning(log_msg)
+
+
 def run_in_new_thread(f):
     @functools.wraps(f)
     def wrapper(*args, **kwargs):
         threading.Thread(target=f, args=args, kwargs=kwargs).start()
 
     return wrapper
```

### Comparing `decorator_libs-1.2/decorator_libs/function_timeout_decorators.py` & `decorator_libs-1.3/decorator_libs/function_timeout_decorators.py`

 * *Files identical despite different names*

### Comparing `decorator_libs-1.2/decorator_libs.egg-info/PKG-INFO` & `decorator_libs-1.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 Metadata-Version: 2.1
-Name: decorator-libs
-Version: 1.2
+Name: decorator_libs
+Version: 1.3
 Summary: all kinds of decorators
-Home-page: UNKNOWN
+Home-page: 
 Author: bfzs
 Author-email: m13148804508@163.com
 Maintainer: ydf
 Maintainer-email: m13148804508@163.com
 License: BSD License
-Description: ## 1. pip install decorator_libs
-        
-        ```
-        各种最常用的日常通用不针对具体业务的装饰器大全
-        
-        包括普通任意实现的装饰器
-        例如单例模式 享元模式 函数结果缓存装饰器。
-        
-        和非常好玩但难实现的装饰器
-        例如where_is_it_called和pysnooper_click_able 装饰器。
-        
-        上下文管理器：
-        自动捕获错误的
-        自动统计代码片段消耗时间的
-        redis分布式锁上下文
-        ```
-        
-        
 Keywords: pysnooper,decorator
 Platform: all
 Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: Implementation
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Software Development :: Libraries
 Description-Content-Type: text/markdown
+
+## 1. pip install decorator_libs
+
+```
+各种最常用的日常通用不针对具体业务的装饰器大全
+
+包括普通任意实现的装饰器
+例如单例模式 享元模式 函数结果缓存装饰器。
+
+和非常好玩但难实现的装饰器
+例如where_is_it_called和pysnooper_click_able 装饰器。
+
+上下文管理器：
+自动捕获错误的
+自动统计代码片段消耗时间的
+redis分布式锁上下文
+```
+
```

### Comparing `decorator_libs-1.2/PKG-INFO` & `decorator_libs-1.3/decorator_libs.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 Metadata-Version: 2.1
-Name: decorator_libs
-Version: 1.2
+Name: decorator-libs
+Version: 1.3
 Summary: all kinds of decorators
-Home-page: UNKNOWN
+Home-page: 
 Author: bfzs
 Author-email: m13148804508@163.com
 Maintainer: ydf
 Maintainer-email: m13148804508@163.com
 License: BSD License
-Description: ## 1. pip install decorator_libs
-        
-        ```
-        各种最常用的日常通用不针对具体业务的装饰器大全
-        
-        包括普通任意实现的装饰器
-        例如单例模式 享元模式 函数结果缓存装饰器。
-        
-        和非常好玩但难实现的装饰器
-        例如where_is_it_called和pysnooper_click_able 装饰器。
-        
-        上下文管理器：
-        自动捕获错误的
-        自动统计代码片段消耗时间的
-        redis分布式锁上下文
-        ```
-        
-        
 Keywords: pysnooper,decorator
 Platform: all
 Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: Implementation
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Software Development :: Libraries
 Description-Content-Type: text/markdown
+
+## 1. pip install decorator_libs
+
+```
+各种最常用的日常通用不针对具体业务的装饰器大全
+
+包括普通任意实现的装饰器
+例如单例模式 享元模式 函数结果缓存装饰器。
+
+和非常好玩但难实现的装饰器
+例如where_is_it_called和pysnooper_click_able 装饰器。
+
+上下文管理器：
+自动捕获错误的
+自动统计代码片段消耗时间的
+redis分布式锁上下文
+```
+
```

### Comparing `decorator_libs-1.2/setup.py` & `decorator_libs-1.3/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 # filepath = ((Path(__file__).parent / Path('README.md')).absolute()).as_posix()
 filepath = 'README.md'
 print(filepath)
 
 setup(
     name='decorator_libs',  #
-    version="1.2",
+    version="1.3",
     description=(
         'all kinds of decorators'
     ),
     keywords=("pysnooper", 'decorator'),
     # long_description=open('README.md', 'r',encoding='utf8').read(),
     long_description_content_type="text/markdown",
     long_description=open(filepath, 'r', encoding='utf8').read(),
@@ -47,13 +47,13 @@
                       ]
 )
 """
 打包上传
 python setup.py sdist upload -r pypi
 
 
-python setup.py sdist & twine upload dist/decorator_libs-1.2.tar.gz
+python setup.py sdist & twine upload dist/decorator_libs-1.3.tar.gz
 
 
 
 python -m pip install decorator_libs --upgrade -i https://pypi.org/simple   # 及时的方式，不用等待 阿里云 豆瓣 同步
 """
```

