# Comparing `tmp/think_sql-0.5.1.tar.gz` & `tmp/think_sql-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "think_sql-0.5.1.tar", max compression
+gzip compressed data, was "think_sql-0.6.0.tar", max compression
```

## Comparing `think_sql-0.5.1.tar` & `think_sql-0.6.0.tar`

### file list

```diff
@@ -1,11 +1,20 @@
--rw-r--r--   0        0        0     1037 2024-01-19 04:40:18.644688 think_sql-0.5.1/pyproject.toml
--rw-r--r--   0        0        0    16210 2024-01-19 03:01:15.553880 think_sql-0.5.1/README.md
--rw-r--r--   0        0        0       23 2021-10-25 02:07:33.991402 think_sql-0.5.1/think_sql/__init__.py
--rw-r--r--   0        0        0     2362 2023-09-22 08:52:05.458752 think_sql-0.5.1/think_sql/cache.py
--rw-r--r--   0        0        0     5487 2023-12-01 03:31:51.154749 think_sql-0.5.1/think_sql/database.py
--rw-r--r--   0        0        0     2837 2024-01-19 04:32:29.868664 think_sql-0.5.1/think_sql/parse.py
--rw-r--r--   0        0        0    27985 2023-12-06 09:28:02.470582 think_sql-0.5.1/think_sql/sql_helper.py
--rw-r--r--   0        0        0    32197 2023-12-06 08:56:25.238362 think_sql-0.5.1/think_sql/table.py
--rw-r--r--   0        0        0     1839 2023-09-26 06:04:27.442026 think_sql-0.5.1/think_sql/util.py
--rw-r--r--   0        0        0    17459 1970-01-01 00:00:00.000000 think_sql-0.5.1/setup.py
--rw-r--r--   0        0        0    16820 1970-01-01 00:00:00.000000 think_sql-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1381 2024-04-16 01:45:58.883741 think_sql-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0    16321 2024-04-16 01:15:23.468069 think_sql-0.6.0/README.md
+-rw-r--r--   0        0        0     1139 2024-04-16 00:41:08.411890 think_sql-0.6.0/think_sql/__init__.py
+-rw-r--r--   0        0        0       70 2024-04-15 09:26:44.219328 think_sql-0.6.0/think_sql/dm/__init__.py
+-rw-r--r--   0        0        0     4693 2024-04-16 00:54:00.548774 think_sql-0.6.0/think_sql/dm/db.py
+-rw-r--r--   0        0        0    28591 2024-04-16 00:54:26.526297 think_sql-0.6.0/think_sql/dm/table.py
+-rw-r--r--   0        0        0     5611 2024-04-15 04:52:03.143703 think_sql-0.6.0/think_sql/dm/util.py
+-rw-r--r--   0        0        0       76 2024-04-15 05:46:17.205661 think_sql-0.6.0/think_sql/mysql/__init__.py
+-rw-r--r--   0        0        0     4031 2024-04-16 00:53:42.323876 think_sql-0.6.0/think_sql/mysql/db.py
+-rw-r--r--   0        0        0     2837 2024-01-19 04:32:29.868664 think_sql-0.6.0/think_sql/mysql/parse.py
+-rw-r--r--   0        0        0    27967 2024-04-15 05:46:51.928111 think_sql-0.6.0/think_sql/mysql/sql_helper.py
+-rw-r--r--   0        0        0    25448 2024-04-16 00:54:40.974556 think_sql-0.6.0/think_sql/mysql/table.py
+-rw-r--r--   0        0        0     3475 2024-04-15 06:24:27.467941 think_sql-0.6.0/think_sql/mysql/util.py
+-rw-r--r--   0        0        0        0 2024-04-11 01:32:11.713368 think_sql-0.6.0/think_sql/tool/__init__.py
+-rw-r--r--   0        0        0     3923 2024-04-16 00:57:11.045987 think_sql-0.6.0/think_sql/tool/base.py
+-rw-r--r--   0        0        0     2360 2024-04-15 05:48:22.966562 think_sql-0.6.0/think_sql/tool/cache.py
+-rw-r--r--   0        0        0     3713 2024-04-16 01:02:24.858779 think_sql-0.6.0/think_sql/tool/interface.py
+-rw-r--r--   0        0        0     3419 2024-04-15 09:16:12.244793 think_sql-0.6.0/think_sql/tool/util.py
+-rw-r--r--   0        0        0    17964 1970-01-01 00:00:00.000000 think_sql-0.6.0/setup.py
+-rw-r--r--   0        0        0    17180 1970-01-01 00:00:00.000000 think_sql-0.6.0/PKG-INFO
```

### Comparing `think_sql-0.5.1/README.md` & `think_sql-0.6.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,41 @@
 # ThinkSQL 类似 ThinkPHP 的数据库引擎
 
+## Drivers
+
+- [x] MySQL
+- [x] 达梦(DM8)
+
 ## Install
 
+- use mysql
+
+```
+pip install think-sql[mysql]
+```
+
+- use 达梦(DM8)
+
 ```
-pip install think-sql
+pip install think-sql[dm]
 ```
 
 ## How to use
 
 ### 1. simple demo
 
 > Database: `test` Table: `user`
 
 - example dict params
 
 ```python
-from think_sql.database import DB
+from think_sql import DB
 
 config = {
+    'driver': 'mysql',
     'host': '127.0.0.1',
     'port': 3306,
     'username': 'root',
     'password': 'root',
     'database': 'test',
 }
 
@@ -30,27 +44,27 @@
     print(data)
 
 ```
 
 - example dsn str
 
 ```python
-from think_sql.database import DB
+from think_sql import DB
 
 with DB("root:'root'@127.0.0.1:3306/test") as db:
     data = db.table('user').where('id',1).find()
     print(data)
 
 ```
 
 - example DBConfig
 
 ```python
-from think_sql.database import DB
-from think_sql.util import DBConfig
+from think_sql import DB
+from think_sql.tool.util import DBConfig
 config = DBConfig(
   host='127.0.0.1',
   port=3306,
   username='root',
   password='root',
   database='test',
 )
@@ -69,15 +83,15 @@
   "age": "36",
   "address": "FUJIAN.XIAMEN"
 }
 ```
 
 ### 2. Introduction
 
-#### think_sql.database.DB
+#### DB
 
 - **init**(config:Union[str,dict,DBConfig],params={})
 
   init database, return DB instance
 
   - config:Union[str,dict,DBConfig]
     - str: `username:'password'@host:port/database`
@@ -96,15 +110,15 @@
 
 - query(sql,params=())
   query sql return cursor.fetchall List[dict]
 
 - execute(sql,params=())
   execute sql write operate(ex:insert,update,delete,...)
 
-#### think_sql.table.Table
+#### Table
 
 - **init**(connector: Connection,cursor: Cursor,table_name: str,debug: bool = True)
 
 - init()
   initialize query condition
 
 - debug(flag=True)
@@ -453,15 +467,15 @@
   update `user` set score = 86 where id = 3;
   update `user` set score = 90 where id = 4;
   ```
 
 #### support transaction
 
 ```python
-from think_sql.database import DB
+from think_sql import DB
 db_dsn = "root:'password'@127.0.0.1:3306/database"
 with DB(db_dsn) as db:
     # result: insert two records into database
     with db.start_trans():
         db.table('user').insert({'name':'think_sql1','score':98})
         db.table('user').insert({'name':'think_sql2','score':99})
     # result: nothing inserted
@@ -470,21 +484,21 @@
         db.table('user').insert({'name':'think_sql2','score':99})
         raise Exception('error')
 
     # The above operation does not affect subsequent operations.
     db.table('user').insert({'name':'think_sql3','score':100})
 ```
 
-#### sql_helper
+#### sql_helper for mysql
 
 > [Ref:hcymysql/sql_helper](https://github.com/hcymysql/sql_helper)
 
 ```python
-from think_sql.database import DB
-from think_sql.sql_helper import help
+from think_sql import DB
+from think_sql.mysql.sql_helper import help
 
 db_dsn = "root:'password'@127.0.0.1:3306/database"
 with DB(db_dsn) as db:
     sql = "slow query sql"
     help(db, sql)
 ```
 
@@ -505,20 +519,20 @@
 +------+---------------+------------+--------------+--------+-----------------+-------+-----------+-------+--------+------------+-------------+
 3) 索引优化建议：
 ----------------------------------------------------------------------------------------------------
 取出表 【hy_cabrecs】 where条件字段 【finished_count】 100000 条记录，重复的数据有：【16093】 条，没有必要为该字段创建索引。
  【hy_cabrecs】 表，无需添加任何索引。
 ```
 
-#### parse
+#### parse for mysql
 
 - parse alter sql
 
   ```python
-  from think_sql import parse
+  from think_sql.mysql import parse
   sql = """
     alter     table
     slow_log_test
     add
     iii int not null default 0  comment   'a';
   """
```

### Comparing `think_sql-0.5.1/think_sql/cache.py` & `think_sql-0.6.0/think_sql/tool/cache.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 #!/usr/bin/python
 # -*- coding: utf-8 -*-
 __author__ = "hbh112233abc@163.com"
 
-from functools import wraps
-import hashlib
-import dill
 import abc  # 利用abc模块实现抽象类
+import dill
+import hashlib
+from functools import wraps
 
 import cacheout
 
 cache_storage = cacheout.Cache()
 
-
 def params_to_key(function_name, *args, **kwargs):
     """按参数生成缓存键名
 
     Args:
         function_name (str): 方法名
 
     Returns:
```

### Comparing `think_sql-0.5.1/think_sql/database.py` & `think_sql-0.6.0/think_sql/dm/db.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,164 +1,148 @@
 #!/usr/bin/python
 # -*- coding: utf-8 -*-
-__author__ = "hbh112233abc@163.com"
-
+__author__ = 'hbh112233abc@163.com'
 
 import re
 import contextlib
 from typing import List, Union
 
-import pymysql
+import dmPython
 from loguru import logger
 
-from .util import DBConfig
-from .table import Table
+from think_sql.dm.table import Table
+from think_sql.tool.util import DBConfig
+from think_sql.tool.base import Database
+from think_sql.tool.interface import DatabaseInterface
 
 
-class DB:
+class DB(DatabaseInterface,Database):
+    """达梦数据库连接类
+    https://peps.python.org/pep-0249/
+    https://eco.dameng.com/document/dm/zh-cn/pm/dmpython-interface
+
+    Args:
+        DatabaseInterface (object): 数据库接口类
+        Database (object): 数据库基类
+    """
     def __init__(
         self,
         config: Union[str, dict, DBConfig],
         params={},
     ):
         """实例化数据库连接
 
         Args:
             config: str|dict|DBConfig 数据库连接配置
             params: dict 数据库连接参数
         """
-        if isinstance(config, str):
-            config = DBConfig.parse_dsn(config)
-        elif isinstance(config, dict):
-            config = DBConfig.model_validate(config)
-        if not isinstance(config, DBConfig):
-            raise ValueError(
-                """
-                Invalid database config
-                Right config ex1:
-                  DB({"host": "127.0.0.1","port": 3306,"username": "root","password": "password","database": "test"})
-                Right config ex2:
-                  DB("root:'password'@127.0.0.1:3306/test")
-                Right config ex3:
-                  from think_sql.util import DBConfig
-                  cfg = DBConfig(host="127.0.0.1", port=3306, username="root", password="password",database="test")
-                  DB(cfg)
-                """
-            )
-        self.config = config
-        self.params = params
-
-        self.log = logger
-        self.connector = None
-        self.cursor = None
-        self.auto_commit = True
-
-        self.connect()
-
+        super().__init__(config,params)
     def __repr__(self):
-        return f"<class 'think_sql.database.DB' database={self.database}>"
+        return f"<class 'think_sql.dm.DB' dsn={self.connector.dsn} database={self.config.database}>"
 
     @contextlib.contextmanager
     def start_trans(self):
         """开始事务"""
+        self.connector.autoCommit = 0
         self.auto_commit = False
         try:
-            self.connector.begin()
             yield
             self.connector.commit()
         except Exception as e:
             logger.error(e)
             self.connector.rollback()
         finally:
+            self.connector.autoCommit = 1
             self.auto_commit = True
 
     def close(self):
         """关闭数据库连接"""
         self.cursor.close()
         self.connector.close()
 
     def connect(self):
         """连接数据库"""
-        self.connector = pymysql.connect(
+        self.connector = dmPython.connect(
             host=self.config.host,
             port=int(self.config.port),
             user=self.config.username,
             password=self.config.password,
-            database=self.config.database,
-            **self.params,
+            local_code=dmPython.PG_UTF8,
+            cursorclass=dmPython.DictCursor,
         )
-        # SSCursor (流式游标) 解决 Python 使用 pymysql 查询大量数据导致内存使用过高的问题
-        self.cursor = self.connector.cursor(pymysql.cursors.SSDictCursor)
+        self.cursor = self.connector.cursor()
+
+    def explain(self,sql:str):
+        return self.connector.explain(sql)
+
+    def exec(self, sql:str, params:tuple=())->int:
+        if not params:
+            sql = sql.replace("%", "%%")
+        else:
+            sql = re.sub(r"(?<!%)%(?![%s])(?![%\(])", "%%", sql)
+        return self.cursor.execute(sql.strip(), params)
 
-    def execute(self, sql, params=()) -> int:
+    def execute(self, sql:str, params:tuple=()) -> int:
         try:
-            if not params:
-                sql = sql.replace("%", "%%")
-            else:
-                sql = re.sub(r"(?<!%)%(?![%s])(?![%\(])", "%%", sql)
-            result = self.cursor.execute(sql.strip(), params)
+            result = self.exec(sql,params)
             if self.auto_commit:
                 self.connector.commit()
             return result
         except Exception as e:
             self.log.warning(sql)
             logger.exception(e)
             return 0
 
-    def query(self, sql, params=()) -> List[dict]:
+    def get_tables(self)->List[str]:
+        """获取数据库中的所有表名
+
+        Returns:
+            List[str]: 表名列表
+        """
+        sql = f"select table_name from all_tables WHERE owner='{self.config.database.upper()}'"
+        self.cursor.execute(sql)
+        res = self.cursor.fetchall()
+        return [r[0] for r in res]
+
+    def last_sql(self)->str:
+        return self.cursor.statement
+
+
+    def query(self, sql:str, params:tuple=()) -> List[dict]:
         result = []
         try:
-            if not params:
-                sql = sql.replace("%", "%%")
-            else:
-                sql = re.sub(r"(?<!%)%(?![%s])(?![%\(])", "%%", sql)
-            self.cursor.execute(sql.strip(), params)
+            self.exec(sql,params)
             if self.cursor.rowcount > 0:
                 result = self.cursor.fetchall()
         except Exception as e:
             self.log.warning(sql)
             self.log.exception(e)
         return result
 
-    def __enter__(self):
-        return self
-
-    def __exit__(self, exc_type, exc_value, trace):
-        """退出操作
-        如果return True可以阻止异常传播
-
-        Args:
-            exc_type (object): 异常类型,默认为None
-            exc_value (object): 异常值,默认为None
-            trace (traceback object): 异常位置,默认为None
-        """
-        if exc_value is not None:
-            if self.cursor._executed:
-                self.log.info(f"[sql]({self.config.database}) {self.cursor._executed}")
-            self.log.exception(exc_value)
+    def error(self,err):
+        if self.cursor.execid:
+            self.log.info(f"[sql]({self.config.database}) {self.last_sql()}")
             self.connector.rollback()
-        else:
-            self.connector.commit()
-        if self.cursor:
-            self.cursor.close()
-        if self.connector:
-            self.connector.close()
+        self.log.exception(err)
+
+    def success(self):
+        self.connector.commit()
 
     def table(self, table_name=""):
         """生成对应数据表
 
         Args:
             table_name (str): 表名
 
         Returns:
             Table: 数据表对象,可以执行链式操作
         """
         if not self.check_connected():
             self.connect()
-        return Table(self.connector, self.cursor, table_name, True)
+        return Table(self, table_name)
 
     def check_connected(self):
         """检查mysql是否可用连接
 
         通过ping检查连接是否可用
 
         Keyword Arguments:
```

### Comparing `think_sql-0.5.1/think_sql/parse.py` & `think_sql-0.6.0/think_sql/mysql/parse.py`

 * *Files identical despite different names*

### Comparing `think_sql-0.5.1/think_sql/sql_helper.py` & `think_sql-0.6.0/think_sql/mysql/sql_helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 #!/usr/bin/python
 # -*- coding: utf-8 -*-
 __author__ = "hbh112233abc@163.com"
 
-from collections import Counter
 import re
 import textwrap
+from collections import Counter
 from typing import Any, Dict, List, Tuple
 
 import sqlparse
 from tabulate import tabulate
-from loguru import logger
 from sql_metadata import Parser
 
-from .database import DB
+from think_sql.mysql.db import DB
 
 logs = []
 
 
 def log(s: str = "", level: str = "log") -> List[str]:
     global logs
     tpl = {
```

### Comparing `think_sql-0.5.1/think_sql/table.py` & `think_sql-0.6.0/think_sql/dm/table.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,160 +1,184 @@
 #!/usr/bin/python
 # -*- coding: utf-8 -*-
 __author__ = "hbh112233abc@163.com"
 
-import re
+from copy import deepcopy
 from hashlib import md5
 import itertools
-import cacheout
 from typing import Any, Union, Tuple, List
 from decimal import Decimal
 
-from pymysql.cursors import Cursor
-from pymysql.connections import Connection
+from dmPython import Cursor
 
-from loguru import logger
+from think_sql.tool.base import Database, TableBase
+from think_sql.tool.interface import TableInterface
 
-from .cache import CacheStorage
+from think_sql.tool.util import to_number
+from think_sql.dm.util import parse_key, parse_value,parse_where
 
 
-class Table:
+class Table(TableBase,TableInterface):
     def __init__(
-        self, connector: Connection, cursor: Cursor, table_name: str, debug: bool = True
+        self, db:Database, table_name: str
     ):
-        self.connector = connector
-        self.db_cursor = cursor
-        self.table_name = table_name
-        self.__debug = debug
-        self.__fetch_sql = False
-        self.log = logger
-        self.cache_storage = cacheout.Cache()
+        super().__init__(
+            db,
+            table_name
+        )
+
+        self.schema = self.db.config.database.upper()
+
+        self.columns = {}
+        self.pk = {}
+
+        self.get_fields()
+
         self.init()
 
     def init(self):
         """初始化查询条件"""
         self.condition_str = "1=1"
         self.condition_val = tuple()
         self.limit_dict = {}
         self.order_by = ""
         self.group_by = ""
         self.distinct_by = ""
         self.select_fields = ("*",)
         self.join_list = []
-        # self.__fetch_sql = False
+        self._fetch_sql = False
         # 缓存相关设置
         self.use_cache = False
         self.cache_key = None
         self.cache_expire = 3600
         return self
 
-    def debug(self, flag: bool = True):
-        """设置调试模式
-
-        Args:
-            flag (bool, optional): 调试标识. Defaults to True.
-
-        Returns:
-            self: 支持链式调用
-        """
-        self.__debug = flag
-        return self
-
-    def set_cache_storage(self, storage: CacheStorage):
-        """设置缓存驱动
-
-        Args:
-            storage (CacheStorage): 缓存驱动
-
-        Returns:
-            self: 支持链式调用
-        """
-        self.cache_storage = storage
-        return self
-
-    def cache(self, key: str = None, expire: int = 3600):
-        """数据缓存
-
-        Args:
-            key (str, optional): 缓存键名. Defaults to None.
-            expire (int, optional): 缓存期限(-1 表示永久期限). Defaults to 3600.
-        """
-        self.use_cache = True
-        self.cache_key = key
-        self.cache_expire = expire
-        return self
 
     def cursor(self) -> Cursor:
         """查询操作,返回cursor对象
 
         Args:
             sql (str): sql语句
             params (list, optional): 绑定参数. Defaults to [].
 
         Returns:
             cursor: 游标
         """
-        sql = "SELECT {select_fields} FROM {table} {join} WHERE {where}{group}{order}{limit}".format(
-            select_fields=",".join(self.select_fields),
-            table=self.table_name,
-            join=" ".join(self.join_list),
-            where=self.__condition_str_fix(),
-            group=self.group_by,
-            order=self.order_by,
-            limit=self.limit_dict.get("sql", ""),
-        )
+        select_fields=self.__select_fields_str()
+        join=" ".join(self.join_list)
+        where=self.__condition_str_fix()
+        group=self.group_by
+        order=self.order_by
+        limit=self.limit_dict.get("sql", "")
+        sql = f"SELECT {select_fields} FROM {self.schema}.{parse_key(self.table_name)} {join} WHERE {where}{group}{order}{limit}"
         params = self.condition_val + self.limit_dict.get("params", ())
 
         self.db_cursor.execute(sql, params)
         return self.db_cursor
 
-    def __get_fields(self) -> tuple:
+    def get_fields(self) -> tuple:
         """获取数据表字段名列表
 
         Returns:
             tuple: 字段名列表
         """
-        sql = f"desc `{self.table_name}`;"
-        data = self.query(sql)
+        if self.columns:
+            return tuple(self.columns.keys())
+        sql = f"""
+        SELECT
+                a.column_name,
+                data_type,
+                DECODE (nullable, 'Y', 0, 1) notnull,
+                data_default,
+                DECODE (a.column_name,b.column_name,1,0) pk,
+                DECODE (a.column_name,d.column_name,1,0) autoinc
+            FROM
+            all_tab_columns a,
+            (
+                SELECT column_name
+                FROM
+                all_constraints c,
+                all_cons_columns col
+                WHERE
+                c.constraint_name = col.constraint_name
+                AND c.constraint_type = 'P'
+                AND c.table_name = '{self.table_name}'
+                AND c.owner = '{self.schema}'
+            ) b,
+            (
+                SELECT COL.NAME as column_name
+                FROM SYSOBJECTS TAB
+                    ,SYSCOLUMNS COL
+                    ,DBA_OBJECTS OBJ
+                where TAB.ID = COL.ID
+                AND TAB.SCHID = OBJ.OBJECT_ID
+                AND TAB.TYPE$ = 'SCHOBJ'
+                AND TAB.SUBTYPE$ = 'UTAB'
+                AND COL.INFO2 & 0x01 = 1
+                AND OBJ.OWNER = '{self.schema}'
+                AND TAB.NAME = '{self.table_name}'
+            ) d
+            WHERE table_name = '{self.table_name}'
+            AND owner = '{self.schema}'
+            AND a.column_name = d.column_name (+)
+            AND a.column_name = b.column_name (+)
+        """
+
+        self.db_cursor.execute(sql)
+        data = self.db_cursor.fetchall()
         fields = []
-        fields = tuple(d["Field"] for d in data)
+        fields = tuple([d['column_name'] for d in data])
+        self.columns = {}
+        for d in data:
+            field = {
+                "name": d['column_name'],
+                "type": d['data_type'],
+                "notnull": d['notnull'],
+                "default": d['data_default'],
+                "primary": d['pk'],
+                "autoinc": d['autoinc'],
+            }
+            self.columns[field['name']] = field
+            if field['primary'] == 1:
+                self.pk = field
         return fields
 
     def get_last_sql(self) -> str:
         """获取最后执行的sql"""
-        return self.db_cursor._last_executed
+        return self.db_cursor.statement
 
     def get_lastid(self) -> str:
         """获取最后作用的id"""
         return self.db_cursor.lastrowid
 
     def get_rowcount(self) -> int:
         """获取sql影响条数"""
         return self.db_cursor.rowcount
 
-    def fetch_sql(self, flag: bool = True):
-        """输出sql语句
+    def fetch_sql(self,flag:bool=True):
+        """设置获取sql语句标识
 
         Args:
-            flag (bool, optional): 是否输出sql. Defaults to True.
+            flag (bool, optional): 是否生成sql. Defaults to True.
         """
-        self.__fetch_sql = flag
+        self._fetch_sql = flag
         return self
 
+
     def build_sql(self, operation: str, params: list = []) -> str:
         """生成sql语句
 
         Args:
             operation (str): sql语句
             params (list, optional): 参数. Defaults to [].
 
         Returns:
             str: 组装后的sql语句
         """
-        return self.db_cursor.mogrify(operation, params)
+        return operation % tuple(params)
 
     def __condition_str_fix(self) -> str:
         """清理查询条件前缀
 
         Returns:
             str: 去除前缀的查询语句
         """
@@ -170,41 +194,39 @@
             sql (str): sql语句
             params (list, optional): 绑定参数. Defaults to [].
 
         Returns:
             tuple: 查询结果
         """
         try:
-            if self.__fetch_sql:
-                return self.build_sql(sql, params)
-
+            finally_sql = ""
+            finally_sql = self.build_sql(sql, params)
+            if self._fetch_sql:
+                return finally_sql
             # 缓存操作
             if self.use_cache:
                 if not self.cache_key:
-                    build_sql = self.build_sql(sql, params)
                     hash = md5()
-                    hash.update(build_sql.encode("utf-8"))
+                    hash.update(finally_sql.encode("utf-8"))
                     sql_md5 = hash.hexdigest()
                     self.cache_key = f"{self.table_name}:{sql_md5}"
-                if self.cache_storage.get(self.cache_key):
-                    return self.cache_storage.get(self.cache_key)
-                else:
-                    self.db_cursor.execute(sql, params)
-                    result = self.db_cursor.fetchall()
-                    self.cache_storage.set(self.cache_key, result, self.cache_expire)
-                    self.__log_sql()
+                result = self.get_cache()
+                if result:
                     return result
 
-            self.db_cursor.execute(sql, params)
+            self.db_cursor.execute(finally_sql)
             result = self.db_cursor.fetchall()
+            self.set_cache(result)
             self.__log_sql()
             return result
         except Exception as e:
-            self.log.error(sql)
-            self.log.error(params)
+            if finally_sql:
+                self.log.error(finally_sql)
+            else:
+                self.log.error(sql, params)
             raise e
         finally:
             self.init()
 
     def execute(self, sql: str, params: list = []) -> int:
         """执行操作(写操作)
 
@@ -212,136 +234,36 @@
             sql (str): sql语句
             params (list, optional): 绑定参数. Defaults to [].
 
         Returns:
             int: 影响行数
         """
         try:
-            if self.__fetch_sql:
-                return self.build_sql(sql, params)
-
-            self.db_cursor.execute(sql, params)
+            finally_sql = ''
+            finally_sql = self.build_sql(sql, params)
+            if self._fetch_sql:
+                return finally_sql
+            self.db_cursor.execute(finally_sql)
             self.connector.commit()
             result = self.db_cursor.rowcount
             self.__log_sql()
             return result
         except Exception as e:
-            self.log.error(self.build_sql(sql, params))
+            if finally_sql:
+                self.log.error(finally_sql)
+            else:
+                self.log.error(sql, params)
             raise e
         finally:
             self.init()
 
     def __log_sql(self):
         """记录sql日志"""
-        if self.__debug:
-            self.log.info(f"[sql]({self.connector.db}) {self.db_cursor._executed}")
-
-    @staticmethod
-    def parse_where(
-        field: str, symbol: str = "", value: Any = None
-    ) -> Tuple[str, tuple]:
-        """解析where条件语句
-
-        Args:
-            field (str): 字段名
-            symbol (str): 条件符号
-            value (mix): 条件值
-
-        Raises:
-            Exception: symbol is error
-            Exception: value could not be none
-
-        Returns:
-            str: 解析后的条件语句
-        """
-        check_value = True
-        condition_str = ""
-        condition_val = tuple()
-
-        symbol = str(symbol).strip().lower()
-        if symbol in ("eq", "="):
-            symbol = "="
-        elif symbol in ("neq", "!=", "<>"):
-            symbol = "<>"
-        elif symbol in ("gt", ">"):
-            symbol = ">"
-        elif symbol in ("egt", ">="):
-            symbol = ">="
-        elif symbol in ("lt", "<"):
-            symbol = "<"
-        elif symbol in ("elt", "<="):
-            symbol = "<="
-        elif symbol in ("in", "not in"):
-            symbol = symbol
-            if isinstance(value, str):
-                if not (value.startswith("(") and value.endswith(")")):
-                    value = value.split(",")
-        elif symbol in ("between", "not between"):
-            symbol = symbol
-            r = re.compile(" and ", re.I)
-            if isinstance(value, str):
-                if not r.findall(value):
-                    value = value.split(",")
-
-            if isinstance(value, (list, tuple)):
-                if len(value) != 2:
-                    raise ValueError("`between` optional `value` must 2 arguments")
-                value = f"{value[0]} AND {value[1]}"
-
-            if not isinstance(value, str) or not r.findall(value):
-                raise ValueError("`between` optional `value` error")
-
-        elif symbol in ("like", "not like"):
-            symbol = symbol
-            if not isinstance(value, str):
-                raise ValueError("`like` optional `value` must be a string")
-            if "%" not in value and "_" not in value:
-                raise ValueError("`like` optional `value` should contain `%` or `_`")
-        elif symbol == "is":
-            symbol = "is"
-        elif symbol in ("null", "is null"):
-            symbol = " is null"
-            check_value = False
-        elif symbol in ("not null", "is not null"):
-            symbol = " is not null"
-            check_value = False
-        elif symbol in ("exists", "not exists"):
-            field = f"{symbol}({field})"
-            symbol = ""
-            check_value = False
-        elif symbol == "exp":
-            if not isinstance(value, str):
-                raise ValueError("`exp` optional `value` should be a string")
-            field = f"{field} {value}"
-            symbol = ""
-            check_value = False
-        elif symbol == "" and value is None:
-            # field 原生sql
-            check_value = False
-        else:
-            if value is None:
-                value = symbol
-                symbol = "="
-            else:
-                raise ValueError("symbol is error")
-        if check_value:
-            if value is None:
-                raise ValueError("value could not be none")
-
-            condition_str += " AND {} {}".format(field, symbol)
-            if isinstance(value, (list, tuple)):
-                condition_str += " (%s)" % ("%s," * len(value))[:-1]
-                condition_val += tuple(value)
-            else:
-                condition_str += " %s"
-                condition_val += (value,)
-        else:
-            condition_str += " AND " + field + symbol
-
-        return condition_str, condition_val
+        if self._debug:
+            self.log.info(f"[sql]({self.schema}) {self.get_last_sql()}")
 
     def where(
         self, field: Union[str, list, tuple], symbol: str = "", value: Any = None
     ):
         """条件设置
 
         Args:
@@ -352,23 +274,23 @@
         Raises:
             ValueError: conditions error
 
         Returns:
             self: 对象本身
         """
         if isinstance(field, str):
-            condition_str, condition_val = Table.parse_where(field, symbol, value)
+            condition_str, condition_val = parse_where(field, symbol, value)
             self.condition_str += condition_str
             self.condition_val += condition_val
         elif isinstance(field, list):
             for condition in field:
                 if isinstance(condition, (list, tuple)) and len(condition) == 3:
                     self.where(*condition)
                 else:
-                    raise ValueError("conditions error => {}".format(condition))
+                    raise ValueError(f"conditions error => {condition}")
         elif isinstance(field, dict):
             for k, v in field.items():
                 self.where(k, v)
         else:
             raise ValueError(
                 f"where error:field={field}, symbol={symbol}, value={value}"
             )
@@ -386,24 +308,24 @@
             Exception: conditions error
 
         Returns:
             self: 对象本身
         """
         condition_str = ""
         if isinstance(field, str):
-            condition_str, condition_val = Table.parse_where(field, symbol, value)
+            condition_str, condition_val = parse_where(field, symbol, value)
         elif isinstance(field, list):
             condition_val = tuple()
             for condition in field:
                 if isinstance(condition, (list, tuple)) and len(condition) == 3:
-                    c_s, c_v = Table.parse_where(*condition)
+                    c_s, c_v = parse_where(*condition)
                     condition_str += c_s
                     condition_val += c_v
                 else:
-                    raise Exception("conditions error => {}".format(condition))
+                    raise Exception(f"conditions error => {condition}")
         self.condition_str += " OR (" + condition_str[5:] + ")"
         self.condition_val += condition_val
         return self
 
     def limit(self, start: int, step: int = None):
         """分页设置
 
@@ -447,91 +369,96 @@
 
         Returns:
             self: 对象本身
         """
         sort = str(sort).strip().upper()
         if sort not in ("ASC", "DESC"):
             raise Exception("sort must be ASC or DESC")
+        field = parse_key(field)
         if not self.order_by:
-            self.order_by = " ORDER BY `{}` {}".format(field, sort)
+            self.order_by = f" ORDER BY {field} {sort}"
         else:
-            self.order_by += ",`{}` {}".format(field, sort)
+            self.order_by += f",{field} {sort}"
         return self
 
     def distinct(self, field: str):
         """去重操作
 
         Args:
             field (str): 去重字段名
 
         Returns:
             self: 对象本身
         """
-        self.distinct_by = "DISTINCT {}".format(field)
+        fields = ",".join([parse_key(x) for x in field.split(",")])
+        self.distinct_by = f"DISTINCT {fields}"
         return self
 
     def group(self, field: str):
         """分组设置
 
         Args:
             field (str): 字段名
 
         Returns:
             self: 对象本身
         """
+        fields = ",".join([parse_key(x) for x in field.split(",")])
         if not self.group_by:
-            self.group_by = " GROUP BY {}".format(
-                ",".join([f"`{x}`" for x in field.split(",")])
-            )
+            self.group_by = f" GROUP BY {fields}"
         else:
-            self.group_by += ",`{}`" + field
+            self.group_by += f",{fields}"
 
         return self
 
     def field(self, fields: Any, exclude: bool = False):
         """字段限制
 
         Args:
             fields (mix): True表示所有字段|以逗号隔开的字符串|列表|元祖
             exclude (bool, optional): 是否过滤. Defaults to False.
 
         Returns:
             self: 对象本身
         """
         if fields is True or fields == "*":
-            fields = self.__get_fields()
+            fields = self.get_fields()
         elif isinstance(fields, str):
             fields = [x.strip() for x in fields.split(",")]
         fields = tuple(fields)
         if exclude:
             if not self.select_fields or self.select_fields == ("*",):
-                self.select_fields = self.__get_fields()
+                self.select_fields = self.get_fields()
             fields = tuple(set(self.select_fields).difference(set(fields)))
         self.select_fields = fields
         return self
 
+    def __select_fields_str(self)->str:
+        """获取select字段字符串
+
+        Returns:
+            str: ","分隔的select字段字符串
+        """
+        return ",".join([parse_key(x) for x in self.select_fields])
+
     def select(self, build_sql: bool = False) -> List[dict]:
         """查询数据
 
         Returns:
             tuple: 查询结果
         """
-        fields = ",".join(self.select_fields)
+        fields = self.__select_fields_str()
         if self.distinct_by:
             fields = self.distinct_by
-
-        sql = "SELECT {select_fields} FROM {table} {join} WHERE {where}{group}{order}{limit}".format(
-            select_fields=fields,
-            table=self.table_name,
-            join=" ".join(self.join_list),
-            where=self.__condition_str_fix(),
-            group=self.group_by,
-            order=self.order_by,
-            limit=self.limit_dict.get("sql", ""),
-        )
+        join=" ".join(self.join_list)
+        where=self.__condition_str_fix()
+        group=self.group_by
+        order=self.order_by
+        limit=self.limit_dict.get("sql", "")
+        sql = f"SELECT {fields} FROM {self.schema}.{parse_key(self.table_name)} {join} WHERE {where}{group}{order}{limit}"
         params = self.condition_val + self.limit_dict.get("params", ())
 
         if build_sql:
             real_sql = self.build_sql(sql, params)
             return f"({real_sql})"
 
         return self.query(sql, params)
@@ -540,15 +467,15 @@
         """查询一条数据
 
         Returns:
             dict: 查询结果
         """
         self.limit(1)
         result = self.select()
-        if self.__fetch_sql:
+        if self._fetch_sql:
             return result
         return result[0] if len(result) > 0 else {}
 
     def value(self, field: str) -> Any:
         """获取某个字段值
 
         Args:
@@ -557,29 +484,29 @@
         Returns:
             str: 对应字段值
         """
         self.select_fields = [field]
         result = self.find()
         return result.get(field, "")
 
-    def column(self, fields: str, key: str = "") -> Union[list, dict]:
+    def column(self, fields: str, key: str = "") -> Union[list,dict]:
         """按列取数据
 
         Args:
             fields (str|list|tuple): 获取字段名(逗号分隔或数组)
             key (str, optional): 作为键名字段. Defaults to ''.
 
         Returns:
-            list|dict: 包含键名的返回字典
+            Union[list,dict]: 包含键名的返回字典
         """
         if isinstance(fields, str):
             fields = fields.split(",")
+        self.select_fields = deepcopy(fields)
         if key and key not in fields:
-            fields.append(key)
-        self.select_fields = fields
+            self.select_fields.append(key)
         result = self.select()
         # 无指定键名
         if not key:
             if len(fields) == 1:
                 return [x[fields[0]] for x in result]
             return result
         # 包含键名
@@ -593,15 +520,15 @@
 
         Args:
             short_name (str, optional): 别名. Defaults to ''.
 
         Returns:
             Table: 链式调用
         """
-        self.table_name = f"{self.table_name} AS {short_name}"
+        self.table_name = f"{self.schema}.{self.table_name} AS {short_name}"
         return self
 
     def join(
         self,
         table_name: str,
         as_name: str = "",
         on: str = "",
@@ -618,35 +545,38 @@
             and_str (str, optional): 附加过滤条件. Defaults to ''.
 
         Returns:
             Table: 支持链式调用
         """
         if not as_name:
             if table_name == self.table_name:
-                raise ValueError("table name should set `as_name`")
+                raise ValueError("table name should set as_name")
 
             as_name = table_name
 
         join = join.upper()
         if join not in ("INNER", "LEFT", "RIGHT", "FULL OUTER"):
             raise ValueError(
-                "`join` type must in ('INNER','LEFT','RIGHT','FULL OUTER')"
+                "join type must in ('INNER','LEFT','RIGHT','FULL OUTER')"
             )
 
-        def make_join_str():
+        def make_join_str(table_name, as_name, on, join, and_str):
             if "join" in table_name:
                 return table_name
-
+            if '.' not in table_name:
+                table_name = f"{self.schema}.{table_name}"
+            table_name = parse_key(table_name)
+            as_name = parse_key(as_name)
             join_str = f"{join} JOIN {table_name} AS {as_name} ON {on}"
             if and_str:
                 join_str += f" AND {and_str}"
 
             return join_str
 
-        join_str = make_join_str()
+        join_str = make_join_str(table_name, as_name, on, join, and_str)
         self.join_list.append(join_str)
         return self
 
     def union(self, sql1: str, sql2: str, union_all: bool = False):
         """UNION操作
 
         Args:
@@ -666,52 +596,57 @@
             replace (bool): 是否使用replace
 
         Returns:
             int: 影响行数
         """
 
         if isinstance(data, dict):
-            keys = ",".join(data.keys())
-            inputs = "(" + ",".join(["%s"] * len(data)) + "),"
-            params = tuple(data.values())
+            keys = ",".join([parse_key(key) for key in data.keys()])
+            inputs = "(" + ",".join(["'%s'"] * len(data)) + "),"
+            params = tuple([parse_value(value) for value in data.values()])
         elif isinstance(data, list):
             inputs = ""
             params = tuple()
             for d in data:
-                keys = ",".join(d.keys())
-                inputs += "(" + ",".join(["%s"] * len(d)) + "),"
-                params += tuple(d.values())
+                keys = ",".join([parse_key(key) for key in d.keys()])
+                inputs += "(" + ",".join(["'%s'"] * len(d)) + "),"
+                params += tuple([parse_value(value) for value in d.values()])
         else:
             raise TypeError("data must be dict or List[dict]")
 
+        if self.pk and self.pk['name'] in data:
+            if self.pk['autoinc']:
+                self.execute(f"SET IDENTITY_INSERT {self.schema}.{parse_key(self.table_name)} ON;")
+            if replace:
+                exist = self.where(self.pk['name'],data[self.pk['name']]).exists()
+                if exist:
+                    return self.where(self.pk['name'],data[self.pk['name']]).update(data)
+
         inputs = inputs[:-1]
-        action = "REPLACE" if replace else "INSERT"
-        sql = "{action} INTO {table} ({keys}) VALUES {inputs};".format(
-            action=action, table=self.table_name, keys=keys, inputs=inputs
-        )
+
+        sql = f"INSERT INTO {self.schema}.{parse_key(self.table_name)} ({keys}) VALUES {inputs};"
         result = self.execute(sql, params)
         return result
 
     def update(self, data: dict, all_record: bool = False) -> int:
         """更新数据
 
         Args:
             data (dict): 更新数据内容
             all_record (bool): 是否更新全部数据,默认False
 
         Returns:
             int: 影响行数
         """
         if not all_record and self.condition_str == "1=1":
-            raise ValueError("please set `where` conditions!")
-        inputs = ",".join(map(lambda k: k + "=%s", data.keys()))
-        params = tuple(data.values()) + self.condition_val
-        sql = "UPDATE {table} SET {inputs} WHERE {where};".format(
-            table=self.table_name, inputs=inputs, where=self.__condition_str_fix()
-        )
+            raise ValueError("please set where conditions!")
+        inputs = ",".join(map(lambda k: f"{parse_key(k)}='%s'", data.keys()))
+        params = tuple([parse_value(v) for v in data.values()]) + self.condition_val
+        where=self.__condition_str_fix()
+        sql = f"UPDATE {self.schema}.{parse_key(self.table_name)} SET {inputs} WHERE {where};"
         result = self.execute(sql, params)
         return result
 
     def delete(self, all_record: bool = False) -> int:
         """删除数据
 
         Args:
@@ -720,280 +655,214 @@
         Raises:
             Exception: please set delete conditions!
 
         Returns:
             int: 影响行数
         """
         if not all_record and self.condition_str == "1=1":
-            raise ValueError("please set `where` conditions!")
-        sql = "DELETE FROM {table} WHERE {where};".format(
-            table=self.table_name, where=self.__condition_str_fix()
-        )
+            raise ValueError("please set where conditions!")
+        where=self.__condition_str_fix()
+        sql = f"DELETE FROM {self.schema}.{parse_key(self.table_name)} WHERE {where};"
         result = self.execute(sql, self.condition_val)
         return result
 
-    @staticmethod
-    def to_number(s: Union[str, int, float], key: str = ""):
-        """转换为数值
-
-        Args:
-            s (Union[str, int, float]): 字符串或数字
-            key (str, optional): 键名. Defaults to ''.
-
-        Raises:
-            ValueError: 错误内容
-
-        Returns:
-            [int,float]: 转换后的数值
-        """
-        if isinstance(s, (int, float)):
-            return s
-
-        if isinstance(s, str):
-            s = s.strip()
-            if re.match(r"^\d+$", s):
-                s = int(s)
-                return s
-            if re.match(r"^\d+\.\d+$", s):
-                s = float(s)
-                return s
-
-        if not isinstance(s, (int, float)) and key:
-            raise ValueError(f"`{key}` must number")
-
-        return s
 
     def inc(self, field: str, step: Union[str, int, float] = 1) -> int:
         """递增
 
         Args:
             field (str): 字段名
             step (int, optional): 步长. Defaults to 1.
 
         Returns:
             bool: 递增结果
         """
-        step = Table.to_number(step, "step")
+        step = to_number(step, "step")
 
         if self.condition_str == "1=1":
-            raise ValueError("please set `where` conditions!")
+            raise ValueError("please set where conditions!")
         symbol = "+" if step > 0 else ""
-
-        sql = "UPDATE {table} SET `{field}` = `{field}`{symbol}{step} WHERE {where}".format(
-            table=self.table_name,
-            field=field,
-            symbol=symbol,
-            step=step,
-            where=self.__condition_str_fix(),
-        )
+        where=self.__condition_str_fix()
+        field = parse_key(field)
+        sql = f"UPDATE {self.schema}.{parse_key(self.table_name)} SET {field} = {field}{symbol}{step} WHERE {where}"
         result = self.execute(sql, self.condition_val)
         return result
 
     def dec(self, field: str, step: int = 1) -> int:
         """递减
 
         Args:
             field (str): 字段名
             step (int, optional): 步长. Defaults to 1.
 
         Returns:
             bool: 递减结果
         """
-        step = Table.to_number(step, "step")
+        step = to_number(step, "step")
         return self.inc(field, step=(0 - step))
 
     def max(self, field: str) -> Union[int, float]:
         """最大值
 
         Args:
             field (str): 字段名
 
         Returns:
             number: 最大值
         """
-        sql = "SELECT MAX({field}) AS max FROM `{table}` WHERE {where} LIMIT 1".format(
-            table=self.table_name,
-            field=field,
-            where=self.__condition_str_fix(),
-        )
+        where=self.__condition_str_fix()
+        field = parse_key(field)
+        sql = f"SELECT MAX({field}) AS _max FROM {self.schema}.{parse_key(self.table_name)} WHERE {where} LIMIT 1"
         result = self.query(sql, self.condition_val)
 
-        if self.__fetch_sql:
+        if self._fetch_sql:
             return result
 
         if not result:
             return 0
 
-        max_value = result[0]["max"]
+        max_value = result[0]["_max"]
         if max_value is None:
             return 0
 
         if isinstance(max_value, (int, float, Decimal)):
             return max_value
 
-        return Table.to_number(max_value)
+        return to_number(max_value)
 
     def sum(self, field: str) -> Union[int, float, Decimal]:
         """合计值
 
         Args:
             field (str): 字段名
 
         Returns:
             number: 合计
         """
-        sql = (
-            "SELECT SUM(`{field}`) AS sum FROM `{table}` WHERE {where} LIMIT 1".format(
-                table=self.table_name,
-                field=field,
-                where=self.__condition_str_fix(),
-            )
-        )
+        where=self.__condition_str_fix()
+        field = parse_key(field)
+        sql = f"SELECT SUM({field}) AS _sum FROM {self.schema}.{parse_key(self.table_name)} WHERE {where} LIMIT 1"
         result = self.query(sql, self.condition_val)
 
-        if self.__fetch_sql:
+        if self._fetch_sql:
             return result
 
         if not result:
             return 0
 
-        sum_value = result[0]["sum"]
+        sum_value = result[0]["_sum"]
         if sum_value is None:
             return 0
 
         if isinstance(sum_value, (int, float, Decimal)):
             return sum_value
 
-        return Table.to_number(sum_value)
+        return to_number(sum_value)
 
     def avg(self, field: str) -> Union[int, float, Decimal]:
         """平均值
 
         Args:
             field (str): 字段名
 
         Returns:
             number: 平均值
         """
-        sql = (
-            "SELECT AVG(`{field}`) AS avg FROM `{table}` WHERE {where} LIMIT 1".format(
-                table=self.table_name,
-                field=field,
-                where=self.__condition_str_fix(),
-            )
-        )
+        where=self.__condition_str_fix()
+        field = parse_key(field)
+        sql = f"SELECT AVG({field}) AS _avg FROM {self.schema}.{parse_key(self.table_name)} WHERE {where} LIMIT 1"
         result = self.query(sql, self.condition_val)
 
-        if self.__fetch_sql:
+        if self._fetch_sql:
             return result
 
         if not result:
             return 0
 
-        avg_value = result[0]["avg"]
+        avg_value = result[0]["_avg"]
         if avg_value is None:
             return 0
 
         if isinstance(avg_value, (int, float, Decimal)):
             return avg_value
 
-        return Table.to_number(avg_value)
+        return to_number(avg_value)
 
-    def count(self, field: str = "1") -> Union[str, int]:
+    def count(self, field: str = "") -> Union[str, int]:
         """获取数据行数
 
         Args:
             field (str, optional): 字段名. Defaults to '*'.
 
         Returns:
             int: 行数量
         """
-        sql = "SELECT COUNT({field}) AS count FROM `{table}` WHERE {where} LIMIT 1".format(
-            field=field,
-            table=self.table_name,
-            where=self.__condition_str_fix(),
-        )
+        where=self.__condition_str_fix()
+        if field == "":
+            field = 1
+        field = parse_key(field)
+        sql = f"SELECT COUNT({field}) AS _count FROM {self.schema}.{parse_key(self.table_name)} WHERE {where} LIMIT 1"
         result = self.query(sql, self.condition_val)
 
-        if self.__fetch_sql:
+        if self._fetch_sql:
             return result
 
         if not result:
             return 0
-        return result[0]["count"] or 0
-
-    def copy_to(self, new_table: str = None, create_blank_table: bool = False) -> int:
-        """复制表 SELECT INTO
-
-        Args:
-            new_table (str, optional): 新表名称. Defaults to None.
-            create_blank_table (bool, optional): 是否只创建表结构. Defaults to False.
+        return result[0]["_count"] or 0
 
-        Returns:
-            int: 执行结果
-        """
-        if new_table is None:
-            new_table = f"{self.table_name}_copy"
-        if isinstance(self.select_fields, (list, tuple)):
-            fields = ", ".join(self.select_fields)
-
-        sql = f"SELECT {fields} INTO {new_table} FROM {self.table_name}"
-        if create_blank_table:
-            sql += " WHERE 1=0"
-        else:
-            sql += f" WHERE {self.__condition_str_fix()}"
-        return self.execute(sql, self.condition_val)
 
     def insert_to(self, new_table: str, fields: Union[str, list, tuple] = None) -> int:
         """复制表 INSERT INTO
 
         Args:
             new_table (str): 新表名称
             fields (str, optional): 字段名. Defaults to None.
 
         Returns:
             int: affect rows count
         """
+        new_table = parse_key(new_table)
         sql = f"INSERT INTO {new_table}"
         if fields is not None:
             if isinstance(fields, str):
                 if fields.startswith("("):
                     sql += f" {fields} "
                 else:
-                    fields = fields.split(",")
+                    fields = [parse_key(x) for x in fields.split(",")]
             if isinstance(fields, (list, tuple)):
-                sql += " ({})".format(",".join(itertools.repeat("%s", len(fields))))
+                ss = ",".join(itertools.repeat("%s", len(fields)))
+                sql += f" ({ss})"
 
-        sql += " SELECT {select_fields} FROM {table} {join} WHERE {where}{group}{order}{limit}".format(
-            select_fields=",".join(self.select_fields),
-            table=self.table_name,
-            join=" ".join(self.join_list),
-            where=self.__condition_str_fix(),
-            group=self.group_by,
-            order=self.order_by,
-            limit=self.limit_dict.get("sql", ""),
-        )
+            if len(self.select_fields) != len(fields):
+                raise ValueError("fields count not match select_fields count")
+
+        select_fields=self.__select_fields_str()
+        join=" ".join(self.join_list)
+        where=self.__condition_str_fix()
+        group=self.group_by
+        order=self.order_by
+        limit=self.limit_dict.get("sql", "")
+        sql += f" SELECT {select_fields} FROM {self.schema}.{parse_key(self.table_name)} {join} WHERE {where}{group}{order}{limit}"
 
         params = self.condition_val + self.limit_dict.get("params", tuple())
         if isinstance(fields, (list, tuple)):
             params = tuple(fields) + params
 
         return self.execute(sql, params)
 
     def exists(self) -> bool:
         """判断是否存在数据
 
         Returns:
             bool: 判断当前查询条件下是否存在数据
         """
-        sql = "SELECT 1 FROM {table} {join} WHERE {where} LIMIT 1".format(
-            table=self.table_name,
-            join=" ".join(self.join_list),
-            where=self.__condition_str_fix(),
-        )
+        join=" ".join(self.join_list)
+        where=self.__condition_str_fix()
+        sql = f"SELECT 1 FROM {self.schema}.{parse_key(self.table_name)} {join} WHERE {where} LIMIT 1"
         result = self.query(sql, self.condition_val)
 
         if not result:
             return False
         return True
 
     def batch_update(self, data: List[dict], key: str) -> int:
```

### Comparing `think_sql-0.5.1/setup.py` & `think_sql-0.6.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,38 +1,48 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
-['think_sql']
+['think_sql', 'think_sql.dm', 'think_sql.mysql', 'think_sql.tool']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['cacheout>=0.15.0,<0.16.0',
  'dill>=0.3.7,<0.4.0',
  'jsonpath>=0.82.2,<0.83.0',
  'loguru>=0.7.2,<0.8.0',
  'pydantic>=2.5.2,<3.0.0',
- 'pymysql>=1.1.0,<2.0.0',
- 'sql-metadata>=2.10.0,<3.0.0',
- 'sqlparse>=0.4.4,<0.5.0',
- 'tabulate>=0.9.0,<0.10.0']
+ 'redis>=5.0.3,<6.0.0']
+
+extras_require = \
+{'all': ['pymysql>=1.1.0,<2.0.0',
+         'sql-metadata>=2.10.0,<3.0.0',
+         'tabulate>=0.9.0,<0.10.0',
+         'sqlparse>=0.4.4,<0.5.0',
+         'dmpython>=2.5.5,<3.0.0'],
+ 'dm': ['dmpython>=2.5.5,<3.0.0'],
+ 'mysql': ['pymysql>=1.1.0,<2.0.0',
+           'sql-metadata>=2.10.0,<3.0.0',
+           'tabulate>=0.9.0,<0.10.0',
+           'sqlparse>=0.4.4,<0.5.0']}
 
 setup_kwargs = {
     'name': 'think-sql',
-    'version': '0.5.1',
+    'version': '0.6.0',
     'description': 'ThinkSQL link think-orm(ThinkPHP)',
-    'long_description': '# ThinkSQL 类似 ThinkPHP 的数据库引擎\n\n## Install\n\n```\npip install think-sql\n```\n\n## How to use\n\n### 1. simple demo\n\n> Database: `test` Table: `user`\n\n- example dict params\n\n```python\nfrom think_sql.database import DB\n\nconfig = {\n    \'host\': \'127.0.0.1\',\n    \'port\': 3306,\n    \'username\': \'root\',\n    \'password\': \'root\',\n    \'database\': \'test\',\n}\n\nwith DB(config) as db:\n    data = db.table(\'user\').where(\'id\',1).find()\n    print(data)\n\n```\n\n- example dsn str\n\n```python\nfrom think_sql.database import DB\n\nwith DB("root:\'root\'@127.0.0.1:3306/test") as db:\n    data = db.table(\'user\').where(\'id\',1).find()\n    print(data)\n\n```\n\n- example DBConfig\n\n```python\nfrom think_sql.database import DB\nfrom think_sql.util import DBConfig\nconfig = DBConfig(\n  host=\'127.0.0.1\',\n  port=3306,\n  username=\'root\',\n  password=\'root\',\n  database=\'test\',\n)\nwith DB(config) as db:\n    data = db.table(\'user\').where(\'id\',1).find()\n    print(data)\n\n```\n\nresult\n\n```json\n{\n  "id": 1,\n  "username": "hbh112233abc",\n  "age": "36",\n  "address": "FUJIAN.XIAMEN"\n}\n```\n\n### 2. Introduction\n\n#### think_sql.database.DB\n\n- **init**(config:Union[str,dict,DBConfig],params={})\n\n  init database, return DB instance\n\n  - config:Union[str,dict,DBConfig]\n    - str: `username:\'password\'@host:port/database`\n    - dict: `{\'host\':\'127.0.0.1\',\'port\':3306,\'username\':\'root\',\'password\':\'root\',\'database\':\'test\'}`\n    - DBConfig: `DBConfig(host=\'127.0.0.1\',port=3306,username=\'root\',password=\'root\',database=\'test\')`\n  - params:dict pymysql connect other params\n\n- connect()\n  connect database use **init** params\n\n- table(table_name):Table\n  return class Table <think_sql.table.Table>\n\n- check_connected():bool\n  check connected, try reconnect database\n\n- query(sql,params=())\n  query sql return cursor.fetchall List[dict]\n\n- execute(sql,params=())\n  execute sql write operate(ex:insert,update,delete,...)\n\n#### think_sql.table.Table\n\n- **init**(connector: Connection,cursor: Cursor,table_name: str,debug: bool = True)\n\n- init()\n  initialize query condition\n\n- debug(flag=True)\n  set debug flag\n\n- set_cache_storage(storage: CacheStorage)\n  set cache storage ex: Redis\n\n- cache(key: str = None, expire: int = 3600)\n  use cache at query\n\n- cursor(sql: str, params: list = []) -> Cursor\n  return cursor object\n\n- get_last_sql() -> str\n  return last sql string\n\n- get_lastid() -> str\n  return last row id\n\n- get_rowcount() -> int\n  return affect rows count\n\n- fetch_sql(flag: bool = True)\n  set fetch sql flag,if flag = True then `query` and `execute` will only return sql\n\n- build_sql(operation: str, params: list = []) -> str\n  return build sql\n\n- query(sql: str, params: list = []) -> list\n  execute read operation sql and return cursor.fetchall()\n  when `fetch_sql`=True then return sql and not execute the sql\n\n- execute(sql: str, params: list = []) -> int\n  execute write operation sql and return affect rows count\n  when `fetch_sql`=True then return sql and not execute the sql\n\n- where(field: Union[str, list, tuple], symbol: str = \'\', value: Any = None)\n  set query conditions, support multipe use\n\n  > where(field,value)\n\n  ```sql\n  where field = value\n  ```\n\n  > where(field,symbol,value)\n\n  ```sql\n  where field symbol value\n  ```\n\n  ```python\n  where(\n      [\n          [field1,symbol1,value1],\n          [field2,symbol2,value2]\n      ]\n  )\n  ```\n\n  ```sql\n  where field1 symbol1 value1 and field2 symbol2 value2\n  ```\n\n  > where(field1,symbol1,value1).where(field2,symbol2,value2)\n\n  ```sql\n  where field1 symbol1 value1 and field2 symbol2 value2\n  ```\n\n  - symbol\n\n  | symbol     | another                  | demo                                                                                    |\n  | ---------- | ------------------------ | --------------------------------------------------------------------------------------- |\n  | `=`        | `eq`,`=`                 | where(\'id\',\'=\',1)                                                                       |\n  | `<>`       | `neq`, `!=`, `<>`        | where(\'id\',\'<>\',1)                                                                      |\n  | `>`        | `gt`,`>`                 | where(\'id\',\'>\',1)                                                                       |\n  | `>=`       | `egt`,`>=`               | where(\'id\',\'>=\',1)                                                                      |\n  | `<`        | `lt`, `<`                | where(\'id\',\'<\',1)                                                                       |\n  | `<=`       | `elt`,`<=`               | where(\'id\',\'<=\',1)                                                                      |\n  | `in`       | `in`,`not in`            | where(\'id\',\'in\',[1,2,3])                                                                |\n  | `between`  | `between`,`not between`  | where(\'id\',\'between\',[1,5]) where(\'id\',\'between\',\'1,5\') where(\'id\',\'between\',\'1 and 5\') |\n  | `like`     | `like`, `not like`       | where(\'name\',\'like\',\'%hbh%\')                                                            |\n  | `null`     | `is null`,`null`         | where(\'remark\',\'is null\')                                                               |\n  | `not null` | `is not null`,`not null` | where(\'remark\',\'is not null\')                                                           |\n  | `exists`   | `exists`, `not exists`   | where(\'remark\',\'exists\')                                                                |\n  | `exp`      | `exp`                    | where(\'id\',\'exp\',\'in (1,2,3)\')                                                          |\n\n- where_or(field: Union[str, list], symbol: str = \'\', value: Any = None)\n\n  > where(\'id\',1).where_or(\'id\',5)\n\n  ```\n  where id = 1 or id = 5\n  ```\n\n- limit(start: int, step: int = None)\n  LIMIT start,step\n\n- page(index: int = 1, size: int = 20)\n  LIMIT index\\*size-1,size\n\n- order(field: str, sort: str = \'asc\')\n  ORDER BY field sort\n\n- group(field:str)\n  GROUP BY field\n\n- distinct(field:str)\n  SELECT DISTINCT field\n\n- field(fields: Any, exclude: bool = False)\n  SELECT fields\n  if `exclude`=True then select the fields of table (exlude:`fields`)\n\n- select(build_sql: bool = False) -> list\n  return select query result\n  if `build_sql`=True then return sql\n\n- find()\n  return select ... limit 1\n\n- value(field: str)\n  return the field of first row\n\n- column(field: str,key: str = \'\')\n\n  > column(\'name\')\n\n  return [\'hbh\',\'mondy\']\n\n  > column(\'name,score\')\n\n  return [{\'hbh\':80},{\'mondy\':88}]\n\n  > column(\'score\',\'name\')\n\n  return {\'hbh\':80, \'mondy\':88}\n\n  > column(\'id,score\',\'name\')\n\n  return {\n  \'hbh\':{\'id\':1,\'score\':80},\n  \'mondy\':{\'id\':2,\'score\':88}\n  }\n\n- alias(short_name: str = \'\')\n  set alias table_name\n\n- join(table_name: str, as_name: str = \'\', on: str = \'\', join: str = \'inner\', and_str: str = \'\')\n  - `table_name` join table_name\n  - `as_name` alias short_table_name for `table_name`\n  - `on` join condition\n  - `join` join type in \'INNER\', \'LEFT\', \'RIGHT\', \'FULL OUTER\'\n  - `and_str` and condition\n    demo\n  ```python\n  db.table(\'table1\').alias(\'a\').join(\n    \'table2\',\'b\',\'a.id=b.a_id\',\'left\'\n  ).join(\n    \'table3\',\'c\',\'c.a_id=a.id\'\n  ).field(\n    \'a.id,a.name,b.id as b_id,b.score,c.id as c_id,c.remark\'\n  ).where(\n    \'a.id\',1\n  ).find()\n  ```\n  sql\n  ```sql\n  SELECT\n      a.id,\n      a.name,\n      b.id AS b_id,\n      b.score,\n      c.id AS c_id,\n      c.remark\n  FROM\n      table1 AS a\n      LEFT JOIN table2 AS b ON a.id = b.a_id\n      INNER JOIN table3 AS c ON c.a_id = a.id\n  WHERE\n      a.id = 1\n      LIMIT 1\n  ```\n- union(sql1: str, sql2: str, union_all: bool = False)\n  union sql1 and sql2\n\n  - union_all if union_all is True then `UNION ALL`\n\n  _demo_\n\n  ```python\n  sql1 = db.table(\'table1\').field(\'name,score\').where(\'status\',1).select(build_sql=True)\n  sql2 = db.table(\'table2\').field(\'name,score\').where(\'status\',1).select(build_sql=True)\n\n  result = db.table().union(sql1,sql2).where(\'score\',\'>\',60).select()\n  ```\n\n  _sql_\n\n  ```sql\n  SELECT\n  *\n  FROM\n      ( SELECT `name`, `score` FROM table1 WHERE `status` = 1 )\n      UNION\n      ( SELECT `name`, `score` FROM table2 WHERE `status` = 1 )\n  WHERE\n      score > 60\n  ```\n\n- insert(data: Union[dict, List[dict]], replace: bool = False) -> int\n  insert data to database\n\n  - `data` dict: insert one record; list: insert multiple records\n  - `replace` bool if `replace` is True then use `REPLACE INTO`\n\n  _demo_\n  insert one record\n\n  ```python\n  db.table(\'table1\').insert({\'name\':\'test\',\'score\':100})\n  ```\n\n  ```sql\n  INSERT INTO table1 (`name`, `score`) VALUES (\'test\', 100)\n  ```\n\n  insert multiple records\n\n  ```python\n  db.table(\'table1\').insert([{\'name\':\'test\',\'score\':100},{\'name\':\'test2\',\'score\':101}])\n  ```\n\n  ```sql\n  INSERT INTO table1 (`name`, `score`) VALUES (\'test\', 100), (\'test2\', 101)\n  ```\n\n  replace mode\n\n  ```python\n  db.table(\'table1\').insert({\'id\':1,\'name\':\'test\',\'score\':100},replace=True)\n  ```\n\n  ```sql\n  REPLACE INTO table1 (`id`, `name`, `score`) VALUES (1,\'test\', 100)\n  ```\n\n- update(data: dict, all_record: bool = False) -> int\n  update data\n\n  - `data` dict you want update data\n  - `all_record` bool if `all_record` is False then you must set update condition; if you want to update all records then you need set `all_record` = True\n\n- delete(all_record: bool = False) -> int\n  delete record\n\n  - `all_record` bool if `all_record` is False then you must set delete condition; if you want to delete all records then you need set `all_record` = True\n\n- inc(field: str, step: Union[str, int, float] = 1) -> int\n\n  increase `field` +`step`\n\n- dec(field: str, step: int = 1) -> int\n\n  decrease `field` -`step`\n\n- max(field: str) -> Union[int, float]\n\n  get the max value of `field`\n\n- sum(field: str) -> Union[int, float, Decimal]\n\n  get the sum value of `field`\n\n- avg(field: str) -> Union[int, float, Decimal]\n\n  get the avg value of `field`\n\n- count(field: str = \'\\*\') -> int\n\n  get the count of records\n\n- copy_to(new_table: str = None, create_blank_table: bool = False) -> int\n\n  copy data to `new_table`\n\n  - `new_table` if `new_table` is None then `new_table` will auto set like `{table_name}_copy`\n  - `create_blank_table` bool if `create_blank_table` is True then only create a blank table like current table.\n\n  _demo_\n\n  ```sql\n  db.table(\'user\').field(\n    \'name,score\'\n  ).where(\n    \'score\',\'>\',60\n  ).copy_to(\'good_boy\')\n  ```\n\n  _sql_\n\n  ```sql\n  SELECT\n    `name`,\n      `score`\n  INTO `good_boy`\n  FROM\n  `user`\n  WHERE\n      score > 60\n  ```\n\n- insert_to(new_table: str, fields: Union[str, list, tuple] = None) -> int\n\n  ```sql\n  INSERT INTO {new_table} SELECT {select_fields} FROM {table} {join} WHERE {where}{group}{order}{limit}\n  ```\n\n- exists(self) -> bool\n\n  check record exists with some query conditions, it use `SELECT 1 FROM {table} {join} WHERE {where} LIMIT 1`\n\n- batch_update(data:List[dict],key:str) -> int\n\n  batch update multiple records\n\n  _demo_\n\n  ```python\n  data = [\n      {\'id\':1,\'score\':66},\n      {\'id\':2,\'score\':59},\n      {\'id\':3,\'score\':86},\n      {\'id\':4,\'score\':90},\n  ]\n  db.table(\'user\').batch(data,key=\'id\')\n  ```\n\n  _sql_\n\n  ```sql\n  update `user` set score = 66 where id = 1;\n  update `user` set score = 59 where id = 2;\n  update `user` set score = 86 where id = 3;\n  update `user` set score = 90 where id = 4;\n  ```\n\n#### support transaction\n\n```python\nfrom think_sql.database import DB\ndb_dsn = "root:\'password\'@127.0.0.1:3306/database"\nwith DB(db_dsn) as db:\n    # result: insert two records into database\n    with db.start_trans():\n        db.table(\'user\').insert({\'name\':\'think_sql1\',\'score\':98})\n        db.table(\'user\').insert({\'name\':\'think_sql2\',\'score\':99})\n    # result: nothing inserted\n    with db.start_trans():\n        db.table(\'user\').insert({\'name\':\'think_sql1\',\'score\':98})\n        db.table(\'user\').insert({\'name\':\'think_sql2\',\'score\':99})\n        raise Exception(\'error\')\n\n    # The above operation does not affect subsequent operations.\n    db.table(\'user\').insert({\'name\':\'think_sql3\',\'score\':100})\n```\n\n#### sql_helper\n\n> [Ref:hcymysql/sql_helper](https://github.com/hcymysql/sql_helper)\n\n```python\nfrom think_sql.database import DB\nfrom think_sql.sql_helper import help\n\ndb_dsn = "root:\'password\'@127.0.0.1:3306/database"\nwith DB(db_dsn) as db:\n    sql = "slow query sql"\n    help(db, sql)\n```\n\n> result\n\n```shell\n1) 输入的SQL语句是：\n----------------------------------------------------------------------------------------------------\nSELECT *\nFROM hy_cabrecs\nWHERE finished_count > 0\n----------------------------------------------------------------------------------------------------\n2) EXPLAIN执行计划:\n+------+---------------+------------+--------------+--------+-----------------+-------+-----------+-------+--------+------------+-------------+\n| id   | select_type   | table      | partitions   | type   | possible_keys   | key   | key_len   | ref   | rows   | filtered   | Extra       |\n+======+===============+============+==============+========+=================+=======+===========+=======+========+============+=============+\n| 1    | SIMPLE        | hy_cabrecs | None         | ALL    | None            | None  | None      | None  | 14422  | 33.33      | Using where |\n+------+---------------+------------+--------------+--------+-----------------+-------+-----------+-------+--------+------------+-------------+\n3) 索引优化建议：\n----------------------------------------------------------------------------------------------------\n取出表 【hy_cabrecs】 where条件字段 【finished_count】 100000 条记录，重复的数据有：【16093】 条，没有必要为该字段创建索引。\n 【hy_cabrecs】 表，无需添加任何索引。\n```\n\n#### parse\n\n- parse alter sql\n\n  ```python\n  from think_sql import parse\n  sql = """\n    alter     table\n    slow_log_test\n    add\n    iii int not null default 0  comment   \'a\';\n  """\n\n  print(parse.alter_sql(sql))\n  ```\n\n  result:\n\n  ```json\n  {\n    "table": "slow_log_test",\n    "field": "iii",\n    "field_type": "int",\n    "is_null": "NOT NULL",\n    "default": "0",\n    "comment": "\'a\'",\n    "after": ""\n  }\n  ```\n\n## Development\n\n### poetry 包管理器\n\n[官网](https://python-poetry.org/)\n\n[Python 包管理之 poetry 的使用](https://blog.csdn.net/zhoubihui0000/article/details/104937285)\n\n[Python 包管理之 poetry 基本使用](https://zhuanlan.zhihu.com/p/110721747)\n\n```\n# 配置虚拟环境在项目目录下\npoetry config virtualenvs.path true\n# 安装依赖\npoetry install\n# 进入虚拟环境\npoetry shell\n```\n\n### poetry command\n\n| 名称    | 功能                                                       |\n| ------- | ---------------------------------------------------------- |\n| new     | 创建一个项目脚手架，包含基本结构、pyproject.toml 文件      |\n| init    | 基于已有的项目代码创建 pyproject.toml 文件，支持交互式填写 |\n| install | 安装依赖库                                                 |\n| update  | 更新依赖库                                                 |\n| add     | 添加依赖库                                                 |\n| remove  | 移除依赖库                                                 |\n| show    | 查看具体依赖库信息，支持显示树形依赖链                     |\n| build   | 构建 tar.gz 或 wheel 包                                    |\n| publish | 发布到 PyPI                                                |\n| run     | 运行脚本和代码                                             |\n\n## unit test\n\n```\npytest --cov --cov-report=html\n```\n\n## publish\n\n```\npoetry build\npoetry config pypi-token.pypi "your pypi.org api token"\npoetry publish -n\n```\n',
+    'long_description': '# ThinkSQL 类似 ThinkPHP 的数据库引擎\n\n## Drivers\n\n- [x] MySQL\n- [x] 达梦(DM8)\n\n## Install\n\n- use mysql\n\n```\npip install think-sql[mysql]\n```\n\n- use 达梦(DM8)\n\n```\npip install think-sql[dm]\n```\n\n## How to use\n\n### 1. simple demo\n\n> Database: `test` Table: `user`\n\n- example dict params\n\n```python\nfrom think_sql import DB\n\nconfig = {\n    \'driver\': \'mysql\',\n    \'host\': \'127.0.0.1\',\n    \'port\': 3306,\n    \'username\': \'root\',\n    \'password\': \'root\',\n    \'database\': \'test\',\n}\n\nwith DB(config) as db:\n    data = db.table(\'user\').where(\'id\',1).find()\n    print(data)\n\n```\n\n- example dsn str\n\n```python\nfrom think_sql import DB\n\nwith DB("root:\'root\'@127.0.0.1:3306/test") as db:\n    data = db.table(\'user\').where(\'id\',1).find()\n    print(data)\n\n```\n\n- example DBConfig\n\n```python\nfrom think_sql import DB\nfrom think_sql.tool.util import DBConfig\nconfig = DBConfig(\n  host=\'127.0.0.1\',\n  port=3306,\n  username=\'root\',\n  password=\'root\',\n  database=\'test\',\n)\nwith DB(config) as db:\n    data = db.table(\'user\').where(\'id\',1).find()\n    print(data)\n\n```\n\nresult\n\n```json\n{\n  "id": 1,\n  "username": "hbh112233abc",\n  "age": "36",\n  "address": "FUJIAN.XIAMEN"\n}\n```\n\n### 2. Introduction\n\n#### DB\n\n- **init**(config:Union[str,dict,DBConfig],params={})\n\n  init database, return DB instance\n\n  - config:Union[str,dict,DBConfig]\n    - str: `username:\'password\'@host:port/database`\n    - dict: `{\'host\':\'127.0.0.1\',\'port\':3306,\'username\':\'root\',\'password\':\'root\',\'database\':\'test\'}`\n    - DBConfig: `DBConfig(host=\'127.0.0.1\',port=3306,username=\'root\',password=\'root\',database=\'test\')`\n  - params:dict pymysql connect other params\n\n- connect()\n  connect database use **init** params\n\n- table(table_name):Table\n  return class Table <think_sql.table.Table>\n\n- check_connected():bool\n  check connected, try reconnect database\n\n- query(sql,params=())\n  query sql return cursor.fetchall List[dict]\n\n- execute(sql,params=())\n  execute sql write operate(ex:insert,update,delete,...)\n\n#### Table\n\n- **init**(connector: Connection,cursor: Cursor,table_name: str,debug: bool = True)\n\n- init()\n  initialize query condition\n\n- debug(flag=True)\n  set debug flag\n\n- set_cache_storage(storage: CacheStorage)\n  set cache storage ex: Redis\n\n- cache(key: str = None, expire: int = 3600)\n  use cache at query\n\n- cursor(sql: str, params: list = []) -> Cursor\n  return cursor object\n\n- get_last_sql() -> str\n  return last sql string\n\n- get_lastid() -> str\n  return last row id\n\n- get_rowcount() -> int\n  return affect rows count\n\n- fetch_sql(flag: bool = True)\n  set fetch sql flag,if flag = True then `query` and `execute` will only return sql\n\n- build_sql(operation: str, params: list = []) -> str\n  return build sql\n\n- query(sql: str, params: list = []) -> list\n  execute read operation sql and return cursor.fetchall()\n  when `fetch_sql`=True then return sql and not execute the sql\n\n- execute(sql: str, params: list = []) -> int\n  execute write operation sql and return affect rows count\n  when `fetch_sql`=True then return sql and not execute the sql\n\n- where(field: Union[str, list, tuple], symbol: str = \'\', value: Any = None)\n  set query conditions, support multipe use\n\n  > where(field,value)\n\n  ```sql\n  where field = value\n  ```\n\n  > where(field,symbol,value)\n\n  ```sql\n  where field symbol value\n  ```\n\n  ```python\n  where(\n      [\n          [field1,symbol1,value1],\n          [field2,symbol2,value2]\n      ]\n  )\n  ```\n\n  ```sql\n  where field1 symbol1 value1 and field2 symbol2 value2\n  ```\n\n  > where(field1,symbol1,value1).where(field2,symbol2,value2)\n\n  ```sql\n  where field1 symbol1 value1 and field2 symbol2 value2\n  ```\n\n  - symbol\n\n  | symbol     | another                  | demo                                                                                    |\n  | ---------- | ------------------------ | --------------------------------------------------------------------------------------- |\n  | `=`        | `eq`,`=`                 | where(\'id\',\'=\',1)                                                                       |\n  | `<>`       | `neq`, `!=`, `<>`        | where(\'id\',\'<>\',1)                                                                      |\n  | `>`        | `gt`,`>`                 | where(\'id\',\'>\',1)                                                                       |\n  | `>=`       | `egt`,`>=`               | where(\'id\',\'>=\',1)                                                                      |\n  | `<`        | `lt`, `<`                | where(\'id\',\'<\',1)                                                                       |\n  | `<=`       | `elt`,`<=`               | where(\'id\',\'<=\',1)                                                                      |\n  | `in`       | `in`,`not in`            | where(\'id\',\'in\',[1,2,3])                                                                |\n  | `between`  | `between`,`not between`  | where(\'id\',\'between\',[1,5]) where(\'id\',\'between\',\'1,5\') where(\'id\',\'between\',\'1 and 5\') |\n  | `like`     | `like`, `not like`       | where(\'name\',\'like\',\'%hbh%\')                                                            |\n  | `null`     | `is null`,`null`         | where(\'remark\',\'is null\')                                                               |\n  | `not null` | `is not null`,`not null` | where(\'remark\',\'is not null\')                                                           |\n  | `exists`   | `exists`, `not exists`   | where(\'remark\',\'exists\')                                                                |\n  | `exp`      | `exp`                    | where(\'id\',\'exp\',\'in (1,2,3)\')                                                          |\n\n- where_or(field: Union[str, list], symbol: str = \'\', value: Any = None)\n\n  > where(\'id\',1).where_or(\'id\',5)\n\n  ```\n  where id = 1 or id = 5\n  ```\n\n- limit(start: int, step: int = None)\n  LIMIT start,step\n\n- page(index: int = 1, size: int = 20)\n  LIMIT index\\*size-1,size\n\n- order(field: str, sort: str = \'asc\')\n  ORDER BY field sort\n\n- group(field:str)\n  GROUP BY field\n\n- distinct(field:str)\n  SELECT DISTINCT field\n\n- field(fields: Any, exclude: bool = False)\n  SELECT fields\n  if `exclude`=True then select the fields of table (exlude:`fields`)\n\n- select(build_sql: bool = False) -> list\n  return select query result\n  if `build_sql`=True then return sql\n\n- find()\n  return select ... limit 1\n\n- value(field: str)\n  return the field of first row\n\n- column(field: str,key: str = \'\')\n\n  > column(\'name\')\n\n  return [\'hbh\',\'mondy\']\n\n  > column(\'name,score\')\n\n  return [{\'hbh\':80},{\'mondy\':88}]\n\n  > column(\'score\',\'name\')\n\n  return {\'hbh\':80, \'mondy\':88}\n\n  > column(\'id,score\',\'name\')\n\n  return {\n  \'hbh\':{\'id\':1,\'score\':80},\n  \'mondy\':{\'id\':2,\'score\':88}\n  }\n\n- alias(short_name: str = \'\')\n  set alias table_name\n\n- join(table_name: str, as_name: str = \'\', on: str = \'\', join: str = \'inner\', and_str: str = \'\')\n  - `table_name` join table_name\n  - `as_name` alias short_table_name for `table_name`\n  - `on` join condition\n  - `join` join type in \'INNER\', \'LEFT\', \'RIGHT\', \'FULL OUTER\'\n  - `and_str` and condition\n    demo\n  ```python\n  db.table(\'table1\').alias(\'a\').join(\n    \'table2\',\'b\',\'a.id=b.a_id\',\'left\'\n  ).join(\n    \'table3\',\'c\',\'c.a_id=a.id\'\n  ).field(\n    \'a.id,a.name,b.id as b_id,b.score,c.id as c_id,c.remark\'\n  ).where(\n    \'a.id\',1\n  ).find()\n  ```\n  sql\n  ```sql\n  SELECT\n      a.id,\n      a.name,\n      b.id AS b_id,\n      b.score,\n      c.id AS c_id,\n      c.remark\n  FROM\n      table1 AS a\n      LEFT JOIN table2 AS b ON a.id = b.a_id\n      INNER JOIN table3 AS c ON c.a_id = a.id\n  WHERE\n      a.id = 1\n      LIMIT 1\n  ```\n- union(sql1: str, sql2: str, union_all: bool = False)\n  union sql1 and sql2\n\n  - union_all if union_all is True then `UNION ALL`\n\n  _demo_\n\n  ```python\n  sql1 = db.table(\'table1\').field(\'name,score\').where(\'status\',1).select(build_sql=True)\n  sql2 = db.table(\'table2\').field(\'name,score\').where(\'status\',1).select(build_sql=True)\n\n  result = db.table().union(sql1,sql2).where(\'score\',\'>\',60).select()\n  ```\n\n  _sql_\n\n  ```sql\n  SELECT\n  *\n  FROM\n      ( SELECT `name`, `score` FROM table1 WHERE `status` = 1 )\n      UNION\n      ( SELECT `name`, `score` FROM table2 WHERE `status` = 1 )\n  WHERE\n      score > 60\n  ```\n\n- insert(data: Union[dict, List[dict]], replace: bool = False) -> int\n  insert data to database\n\n  - `data` dict: insert one record; list: insert multiple records\n  - `replace` bool if `replace` is True then use `REPLACE INTO`\n\n  _demo_\n  insert one record\n\n  ```python\n  db.table(\'table1\').insert({\'name\':\'test\',\'score\':100})\n  ```\n\n  ```sql\n  INSERT INTO table1 (`name`, `score`) VALUES (\'test\', 100)\n  ```\n\n  insert multiple records\n\n  ```python\n  db.table(\'table1\').insert([{\'name\':\'test\',\'score\':100},{\'name\':\'test2\',\'score\':101}])\n  ```\n\n  ```sql\n  INSERT INTO table1 (`name`, `score`) VALUES (\'test\', 100), (\'test2\', 101)\n  ```\n\n  replace mode\n\n  ```python\n  db.table(\'table1\').insert({\'id\':1,\'name\':\'test\',\'score\':100},replace=True)\n  ```\n\n  ```sql\n  REPLACE INTO table1 (`id`, `name`, `score`) VALUES (1,\'test\', 100)\n  ```\n\n- update(data: dict, all_record: bool = False) -> int\n  update data\n\n  - `data` dict you want update data\n  - `all_record` bool if `all_record` is False then you must set update condition; if you want to update all records then you need set `all_record` = True\n\n- delete(all_record: bool = False) -> int\n  delete record\n\n  - `all_record` bool if `all_record` is False then you must set delete condition; if you want to delete all records then you need set `all_record` = True\n\n- inc(field: str, step: Union[str, int, float] = 1) -> int\n\n  increase `field` +`step`\n\n- dec(field: str, step: int = 1) -> int\n\n  decrease `field` -`step`\n\n- max(field: str) -> Union[int, float]\n\n  get the max value of `field`\n\n- sum(field: str) -> Union[int, float, Decimal]\n\n  get the sum value of `field`\n\n- avg(field: str) -> Union[int, float, Decimal]\n\n  get the avg value of `field`\n\n- count(field: str = \'\\*\') -> int\n\n  get the count of records\n\n- copy_to(new_table: str = None, create_blank_table: bool = False) -> int\n\n  copy data to `new_table`\n\n  - `new_table` if `new_table` is None then `new_table` will auto set like `{table_name}_copy`\n  - `create_blank_table` bool if `create_blank_table` is True then only create a blank table like current table.\n\n  _demo_\n\n  ```sql\n  db.table(\'user\').field(\n    \'name,score\'\n  ).where(\n    \'score\',\'>\',60\n  ).copy_to(\'good_boy\')\n  ```\n\n  _sql_\n\n  ```sql\n  SELECT\n    `name`,\n      `score`\n  INTO `good_boy`\n  FROM\n  `user`\n  WHERE\n      score > 60\n  ```\n\n- insert_to(new_table: str, fields: Union[str, list, tuple] = None) -> int\n\n  ```sql\n  INSERT INTO {new_table} SELECT {select_fields} FROM {table} {join} WHERE {where}{group}{order}{limit}\n  ```\n\n- exists(self) -> bool\n\n  check record exists with some query conditions, it use `SELECT 1 FROM {table} {join} WHERE {where} LIMIT 1`\n\n- batch_update(data:List[dict],key:str) -> int\n\n  batch update multiple records\n\n  _demo_\n\n  ```python\n  data = [\n      {\'id\':1,\'score\':66},\n      {\'id\':2,\'score\':59},\n      {\'id\':3,\'score\':86},\n      {\'id\':4,\'score\':90},\n  ]\n  db.table(\'user\').batch(data,key=\'id\')\n  ```\n\n  _sql_\n\n  ```sql\n  update `user` set score = 66 where id = 1;\n  update `user` set score = 59 where id = 2;\n  update `user` set score = 86 where id = 3;\n  update `user` set score = 90 where id = 4;\n  ```\n\n#### support transaction\n\n```python\nfrom think_sql import DB\ndb_dsn = "root:\'password\'@127.0.0.1:3306/database"\nwith DB(db_dsn) as db:\n    # result: insert two records into database\n    with db.start_trans():\n        db.table(\'user\').insert({\'name\':\'think_sql1\',\'score\':98})\n        db.table(\'user\').insert({\'name\':\'think_sql2\',\'score\':99})\n    # result: nothing inserted\n    with db.start_trans():\n        db.table(\'user\').insert({\'name\':\'think_sql1\',\'score\':98})\n        db.table(\'user\').insert({\'name\':\'think_sql2\',\'score\':99})\n        raise Exception(\'error\')\n\n    # The above operation does not affect subsequent operations.\n    db.table(\'user\').insert({\'name\':\'think_sql3\',\'score\':100})\n```\n\n#### sql_helper for mysql\n\n> [Ref:hcymysql/sql_helper](https://github.com/hcymysql/sql_helper)\n\n```python\nfrom think_sql import DB\nfrom think_sql.mysql.sql_helper import help\n\ndb_dsn = "root:\'password\'@127.0.0.1:3306/database"\nwith DB(db_dsn) as db:\n    sql = "slow query sql"\n    help(db, sql)\n```\n\n> result\n\n```shell\n1) 输入的SQL语句是：\n----------------------------------------------------------------------------------------------------\nSELECT *\nFROM hy_cabrecs\nWHERE finished_count > 0\n----------------------------------------------------------------------------------------------------\n2) EXPLAIN执行计划:\n+------+---------------+------------+--------------+--------+-----------------+-------+-----------+-------+--------+------------+-------------+\n| id   | select_type   | table      | partitions   | type   | possible_keys   | key   | key_len   | ref   | rows   | filtered   | Extra       |\n+======+===============+============+==============+========+=================+=======+===========+=======+========+============+=============+\n| 1    | SIMPLE        | hy_cabrecs | None         | ALL    | None            | None  | None      | None  | 14422  | 33.33      | Using where |\n+------+---------------+------------+--------------+--------+-----------------+-------+-----------+-------+--------+------------+-------------+\n3) 索引优化建议：\n----------------------------------------------------------------------------------------------------\n取出表 【hy_cabrecs】 where条件字段 【finished_count】 100000 条记录，重复的数据有：【16093】 条，没有必要为该字段创建索引。\n 【hy_cabrecs】 表，无需添加任何索引。\n```\n\n#### parse for mysql\n\n- parse alter sql\n\n  ```python\n  from think_sql.mysql import parse\n  sql = """\n    alter     table\n    slow_log_test\n    add\n    iii int not null default 0  comment   \'a\';\n  """\n\n  print(parse.alter_sql(sql))\n  ```\n\n  result:\n\n  ```json\n  {\n    "table": "slow_log_test",\n    "field": "iii",\n    "field_type": "int",\n    "is_null": "NOT NULL",\n    "default": "0",\n    "comment": "\'a\'",\n    "after": ""\n  }\n  ```\n\n## Development\n\n### poetry 包管理器\n\n[官网](https://python-poetry.org/)\n\n[Python 包管理之 poetry 的使用](https://blog.csdn.net/zhoubihui0000/article/details/104937285)\n\n[Python 包管理之 poetry 基本使用](https://zhuanlan.zhihu.com/p/110721747)\n\n```\n# 配置虚拟环境在项目目录下\npoetry config virtualenvs.path true\n# 安装依赖\npoetry install\n# 进入虚拟环境\npoetry shell\n```\n\n### poetry command\n\n| 名称    | 功能                                                       |\n| ------- | ---------------------------------------------------------- |\n| new     | 创建一个项目脚手架，包含基本结构、pyproject.toml 文件      |\n| init    | 基于已有的项目代码创建 pyproject.toml 文件，支持交互式填写 |\n| install | 安装依赖库                                                 |\n| update  | 更新依赖库                                                 |\n| add     | 添加依赖库                                                 |\n| remove  | 移除依赖库                                                 |\n| show    | 查看具体依赖库信息，支持显示树形依赖链                     |\n| build   | 构建 tar.gz 或 wheel 包                                    |\n| publish | 发布到 PyPI                                                |\n| run     | 运行脚本和代码                                             |\n\n## unit test\n\n```\npytest --cov --cov-report=html\n```\n\n## publish\n\n```\npoetry build\npoetry config pypi-token.pypi "your pypi.org api token"\npoetry publish -n\n```\n',
     'author': 'hbh112233abc',
     'author_email': 'hbh112233abc@163.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/hbh112233abc/think-sql',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.7,<=3.12',
+    'extras_require': extras_require,
+    'python_requires': '>=3.8,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `think_sql-0.5.1/PKG-INFO` & `think_sql-0.6.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,57 +1,75 @@
 Metadata-Version: 2.1
 Name: think-sql
-Version: 0.5.1
+Version: 0.6.0
 Summary: ThinkSQL link think-orm(ThinkPHP)
 Home-page: https://github.com/hbh112233abc/think-sql
 License: MIT
-Keywords: sql,database,table,think-orm,ThinkPHP
+Keywords: sql,think-sql,DB,Table,mysql,达梦
 Author: hbh112233abc
 Author-email: hbh112233abc@163.com
-Requires-Python: >=3.7,<=3.12
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: all
+Provides-Extra: dm
+Provides-Extra: mysql
 Requires-Dist: cacheout (>=0.15.0,<0.16.0)
 Requires-Dist: dill (>=0.3.7,<0.4.0)
+Requires-Dist: dmpython (>=2.5.5,<3.0.0); extra == "dm" or extra == "all"
 Requires-Dist: jsonpath (>=0.82.2,<0.83.0)
 Requires-Dist: loguru (>=0.7.2,<0.8.0)
 Requires-Dist: pydantic (>=2.5.2,<3.0.0)
-Requires-Dist: pymysql (>=1.1.0,<2.0.0)
-Requires-Dist: sql-metadata (>=2.10.0,<3.0.0)
-Requires-Dist: sqlparse (>=0.4.4,<0.5.0)
-Requires-Dist: tabulate (>=0.9.0,<0.10.0)
+Requires-Dist: pymysql (>=1.1.0,<2.0.0); extra == "mysql" or extra == "all"
+Requires-Dist: redis (>=5.0.3,<6.0.0)
+Requires-Dist: sql-metadata (>=2.10.0,<3.0.0); extra == "mysql" or extra == "all"
+Requires-Dist: sqlparse (>=0.4.4,<0.5.0); extra == "mysql" or extra == "all"
+Requires-Dist: tabulate (>=0.9.0,<0.10.0); extra == "mysql" or extra == "all"
 Project-URL: Documentation, https://github.com/hbh112233abc/think-sql
 Project-URL: Repository, https://github.com/hbh112233abc/think-sql
 Description-Content-Type: text/markdown
 
 # ThinkSQL 类似 ThinkPHP 的数据库引擎
 
+## Drivers
+
+- [x] MySQL
+- [x] 达梦(DM8)
+
 ## Install
 
+- use mysql
+
+```
+pip install think-sql[mysql]
+```
+
+- use 达梦(DM8)
+
 ```
-pip install think-sql
+pip install think-sql[dm]
 ```
 
 ## How to use
 
 ### 1. simple demo
 
 > Database: `test` Table: `user`
 
 - example dict params
 
 ```python
-from think_sql.database import DB
+from think_sql import DB
 
 config = {
+    'driver': 'mysql',
     'host': '127.0.0.1',
     'port': 3306,
     'username': 'root',
     'password': 'root',
     'database': 'test',
 }
 
@@ -60,27 +78,27 @@
     print(data)
 
 ```
 
 - example dsn str
 
 ```python
-from think_sql.database import DB
+from think_sql import DB
 
 with DB("root:'root'@127.0.0.1:3306/test") as db:
     data = db.table('user').where('id',1).find()
     print(data)
 
 ```
 
 - example DBConfig
 
 ```python
-from think_sql.database import DB
-from think_sql.util import DBConfig
+from think_sql import DB
+from think_sql.tool.util import DBConfig
 config = DBConfig(
   host='127.0.0.1',
   port=3306,
   username='root',
   password='root',
   database='test',
 )
@@ -99,15 +117,15 @@
   "age": "36",
   "address": "FUJIAN.XIAMEN"
 }
 ```
 
 ### 2. Introduction
 
-#### think_sql.database.DB
+#### DB
 
 - **init**(config:Union[str,dict,DBConfig],params={})
 
   init database, return DB instance
 
   - config:Union[str,dict,DBConfig]
     - str: `username:'password'@host:port/database`
@@ -126,15 +144,15 @@
 
 - query(sql,params=())
   query sql return cursor.fetchall List[dict]
 
 - execute(sql,params=())
   execute sql write operate(ex:insert,update,delete,...)
 
-#### think_sql.table.Table
+#### Table
 
 - **init**(connector: Connection,cursor: Cursor,table_name: str,debug: bool = True)
 
 - init()
   initialize query condition
 
 - debug(flag=True)
@@ -483,15 +501,15 @@
   update `user` set score = 86 where id = 3;
   update `user` set score = 90 where id = 4;
   ```
 
 #### support transaction
 
 ```python
-from think_sql.database import DB
+from think_sql import DB
 db_dsn = "root:'password'@127.0.0.1:3306/database"
 with DB(db_dsn) as db:
     # result: insert two records into database
     with db.start_trans():
         db.table('user').insert({'name':'think_sql1','score':98})
         db.table('user').insert({'name':'think_sql2','score':99})
     # result: nothing inserted
@@ -500,21 +518,21 @@
         db.table('user').insert({'name':'think_sql2','score':99})
         raise Exception('error')
 
     # The above operation does not affect subsequent operations.
     db.table('user').insert({'name':'think_sql3','score':100})
 ```
 
-#### sql_helper
+#### sql_helper for mysql
 
 > [Ref:hcymysql/sql_helper](https://github.com/hcymysql/sql_helper)
 
 ```python
-from think_sql.database import DB
-from think_sql.sql_helper import help
+from think_sql import DB
+from think_sql.mysql.sql_helper import help
 
 db_dsn = "root:'password'@127.0.0.1:3306/database"
 with DB(db_dsn) as db:
     sql = "slow query sql"
     help(db, sql)
 ```
 
@@ -535,20 +553,20 @@
 +------+---------------+------------+--------------+--------+-----------------+-------+-----------+-------+--------+------------+-------------+
 3) 索引优化建议：
 ----------------------------------------------------------------------------------------------------
 取出表 【hy_cabrecs】 where条件字段 【finished_count】 100000 条记录，重复的数据有：【16093】 条，没有必要为该字段创建索引。
  【hy_cabrecs】 表，无需添加任何索引。
 ```
 
-#### parse
+#### parse for mysql
 
 - parse alter sql
 
   ```python
-  from think_sql import parse
+  from think_sql.mysql import parse
   sql = """
     alter     table
     slow_log_test
     add
     iii int not null default 0  comment   'a';
   """
```

