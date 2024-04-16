# Comparing `tmp/msanic-1.0.15-py3-none-any.whl.zip` & `tmp/msanic-1.0.16-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 56640 bytes, number of entries: 42
+Zip file size: 56638 bytes, number of entries: 42
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Mar-19 13:56 msanic/__init__.py
 -rw-rw-rw-  2.0 fat     3462 b- defN 24-Apr-15 07:17 msanic/base_blue.py
 -rw-rw-rw-  2.0 fat     8536 b- defN 24-Mar-28 08:50 msanic/base_conf.py
 -rw-rw-rw-  2.0 fat     3241 b- defN 24-Mar-25 14:10 msanic/base_server.py
 -rw-rw-rw-  2.0 fat     9174 b- defN 24-Apr-15 07:12 msanic/base_ws.py
 -rw-rw-rw-  2.0 fat     2847 b- defN 24-Apr-15 07:12 msanic/exception.py
 -rw-rw-rw-  2.0 fat     7677 b- defN 24-Apr-15 07:12 msanic/handler_http.py
@@ -24,21 +24,21 @@
 -rw-rw-rw-  2.0 fat     1116 b- defN 24-Apr-03 08:13 msanic/libs/rds_locker.py
 -rw-rw-rw-  2.0 fat     6838 b- defN 24-Mar-28 15:28 msanic/libs/tool.py
 -rw-rw-rw-  2.0 fat     5014 b- defN 24-Mar-25 15:32 msanic/libs/tool_dt.py
 -rw-rw-rw-  2.0 fat     3070 b- defN 24-Mar-21 14:40 msanic/libs/tool_jwt.py
 -rw-rw-rw-  2.0 fat     1825 b- defN 24-Mar-21 14:40 msanic/libs/tool_ws.py
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Mar-20 12:48 msanic/orm/__init__.py
 -rw-rw-rw-  2.0 fat      730 b- defN 24-Mar-19 13:56 msanic/orm/db_index.py
--rw-rw-rw-  2.0 fat    18495 b- defN 24-Apr-03 03:08 msanic/orm/db_model.py
+-rw-rw-rw-  2.0 fat    18495 b- defN 24-Apr-16 10:04 msanic/orm/db_model.py
 -rw-rw-rw-  2.0 fat    11698 b- defN 24-Apr-03 07:45 msanic/orm/mssql_generator.py
 -rw-rw-rw-  2.0 fat    11698 b- defN 24-Apr-03 07:45 msanic/orm/mysql_generator.py
 -rw-rw-rw-  2.0 fat    11720 b- defN 24-Apr-03 07:45 msanic/orm/pgsql_generator.py
 -rw-rw-rw-  2.0 fat     5098 b- defN 24-Apr-12 02:19 msanic/orm/rc_model.py
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Mar-19 13:56 test/__init__.py
 -rw-rw-rw-  2.0 fat      715 b- defN 24-Mar-25 15:29 test/test_unit.py
--rw-rw-rw-  2.0 fat     1090 b- defN 24-Apr-15 07:40 msanic-1.0.15.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      878 b- defN 24-Apr-15 07:40 msanic-1.0.15.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-15 07:40 msanic-1.0.15.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       52 b- defN 24-Apr-15 07:40 msanic-1.0.15.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat       12 b- defN 24-Apr-15 07:40 msanic-1.0.15.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     3313 b- defN 24-Apr-15 07:40 msanic-1.0.15.dist-info/RECORD
-42 files, 176760 bytes uncompressed, 51446 bytes compressed:  70.9%
+-rw-rw-rw-  2.0 fat     1090 b- defN 24-Apr-16 10:05 msanic-1.0.16.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      878 b- defN 24-Apr-16 10:05 msanic-1.0.16.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-16 10:05 msanic-1.0.16.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       52 b- defN 24-Apr-16 10:05 msanic-1.0.16.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat       12 b- defN 24-Apr-16 10:05 msanic-1.0.16.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     3313 b- defN 24-Apr-16 10:05 msanic-1.0.16.dist-info/RECORD
+42 files, 176760 bytes uncompressed, 51444 bytes compressed:  70.9%
```

## zipnote {}

```diff
@@ -102,26 +102,26 @@
 
 Filename: test/__init__.py
 Comment: 
 
 Filename: test/test_unit.py
 Comment: 
 
-Filename: msanic-1.0.15.dist-info/LICENSE
+Filename: msanic-1.0.16.dist-info/LICENSE
 Comment: 
 
-Filename: msanic-1.0.15.dist-info/METADATA
+Filename: msanic-1.0.16.dist-info/METADATA
 Comment: 
 
-Filename: msanic-1.0.15.dist-info/WHEEL
+Filename: msanic-1.0.16.dist-info/WHEEL
 Comment: 
 
-Filename: msanic-1.0.15.dist-info/entry_points.txt
+Filename: msanic-1.0.16.dist-info/entry_points.txt
 Comment: 
 
-Filename: msanic-1.0.15.dist-info/top_level.txt
+Filename: msanic-1.0.16.dist-info/top_level.txt
 Comment: 
 
-Filename: msanic-1.0.15.dist-info/RECORD
+Filename: msanic-1.0.16.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## msanic/orm/db_model.py

```diff
@@ -246,15 +246,15 @@
             with_del=False,
             split: Union[str, int, float, datetime, date] = None,
             db_key: str = None):
         query_model, _ = cls.gen_simple_query(param=param, with_del=with_del, split=split, db_key=db_key)
         return await query_model.count()
 
     @classmethod
-    async def add_noe(cls, param: dict, fun_success=None, db_key: str = None):
+    async def add_one(cls, param: dict, fun_success=None, db_key: str = None):
         """
         自动分表模式创建
         公共 新增或更新 值为None采用默认值
 
         :param param: 字典数据模型
         :param fun_success: 执行成功后的补充处理函数 协程函数 参数为生成的Model模型
         :param db_key: 指定数据库配置
```

## Comparing `msanic-1.0.15.dist-info/LICENSE` & `msanic-1.0.16.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `msanic-1.0.15.dist-info/METADATA` & `msanic-1.0.16.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msanic
-Version: 1.0.15
+Version: 1.0.16
 Summary: A web framework who is use sanic + tortoise-orm + redis to quick create http&websocket server
 Author: DHDONG
 Author-email: zscych@qq.com
 License: MIT
 Keywords: WebServer,Sanic,WebSite Develop,Web Framework
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

## Comparing `msanic-1.0.15.dist-info/RECORD` & `msanic-1.0.16.dist-info/RECORD`

 * *Files 7% similar despite different names*

```diff
@@ -23,20 +23,20 @@
 msanic/libs/rds_locker.py,sha256=Q8UkKAyHz4xdoG_oL0j5BfsBpTeKbW8sy7yDXwO62_E,1116
 msanic/libs/tool.py,sha256=qwGyceVtYp45hTneFGpWD7KOq8411B7Q8ZyZE_tcZNo,6838
 msanic/libs/tool_dt.py,sha256=ymTQBwxoUHigSX_L06LHDjzGBNmKjKXTLLAQBv_ssA8,5014
 msanic/libs/tool_jwt.py,sha256=cCdHNB16fp3MZfDT77ocUtHFtOrQjKu1qZL9x2iCI0A,3070
 msanic/libs/tool_ws.py,sha256=haIgAeqZDwIpVwoOrLlRVp-qD2lOLS-h5Ej00n0PIpg,1825
 msanic/orm/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 msanic/orm/db_index.py,sha256=LmqneAZnHPfWsWNS4wH6F8iyZ56xtXtczglRFOZtgHA,730
-msanic/orm/db_model.py,sha256=6JEu5iOZ0YDqYzxAcb4eYjMQVZOUPq78vAPnQW9E-eU,18495
+msanic/orm/db_model.py,sha256=YI5yPpENbxHosfybemp-pndCuh5VmeUGbhbsssNZuHs,18495
 msanic/orm/mssql_generator.py,sha256=c9q71hljWqBxoNriG0OefwD48w3gVTb62HnFKjreom4,11698
 msanic/orm/mysql_generator.py,sha256=ctZbt0w_4zo43UCACVKD7-Ioc6RpWCQ1WFse2ZmGHMA,11698
 msanic/orm/pgsql_generator.py,sha256=BMNDAZ-2X9dPbUOBlhR5UJBfqXWpl23KRgTozleKCCQ,11720
 msanic/orm/rc_model.py,sha256=NcgSVW34eSx_TiMYE9DYrA6Bt_qitTRH5pX3UYqa6ok,5098
 test/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 test/test_unit.py,sha256=mJHn2hOiYpjez2oG3-56nFm66qZ7CMnBoYOtrwL9cug,715
-msanic-1.0.15.dist-info/LICENSE,sha256=GSAKapQH5ZIGWlpQTA7v5YrfECyaxaohUb1vJX-qepw,1090
-msanic-1.0.15.dist-info/METADATA,sha256=RKRdgoZWoF9AC8a34QyNscQ4AeMdDJ8_MpDwonjAwAE,878
-msanic-1.0.15.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-msanic-1.0.15.dist-info/entry_points.txt,sha256=CAoZ_qtmP0HhzVmX9w0oN-KSxoCpdqxjDC4pljoU-l4,52
-msanic-1.0.15.dist-info/top_level.txt,sha256=lT96LXfr87NYrx1PR9GraMGNX9KQ6ImvR88MTHEhBkM,12
-msanic-1.0.15.dist-info/RECORD,,
+msanic-1.0.16.dist-info/LICENSE,sha256=GSAKapQH5ZIGWlpQTA7v5YrfECyaxaohUb1vJX-qepw,1090
+msanic-1.0.16.dist-info/METADATA,sha256=DQIb1zQC7rbYL5GFTDHP8mTi_abv-6vawOKqYRIZN7w,878
+msanic-1.0.16.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+msanic-1.0.16.dist-info/entry_points.txt,sha256=CAoZ_qtmP0HhzVmX9w0oN-KSxoCpdqxjDC4pljoU-l4,52
+msanic-1.0.16.dist-info/top_level.txt,sha256=lT96LXfr87NYrx1PR9GraMGNX9KQ6ImvR88MTHEhBkM,12
+msanic-1.0.16.dist-info/RECORD,,
```

