# Comparing `tmp/ts_soup-0.1.8.tar.gz` & `tmp/ts_soup-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\PythonProjects\load_predict\ts-soup\dist\.tmp-y9dxwads\ts_soup-0.1.8.tar", last modified: Sun Apr 14 06:14:10 2024, max compression
+gzip compressed data, was "D:\PythonProjects\GDtrading\ts-soup\dist\.tmp-_y0zjito\ts_soup-0.1.9.tar", last modified: Tue Apr 16 04:44:53 2024, max compression
```

## Comparing `ts_soup-0.1.8.tar` & `ts_soup-0.1.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-14 06:14:10.320880 ts_soup-0.1.8/
--rw-rw-rw-   0        0        0     1028 2024-04-14 06:14:10.320880 ts_soup-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0      686 2024-04-05 12:25:36.000000 ts_soup-0.1.8/README.md
--rw-rw-rw-   0        0        0       42 2024-04-14 06:14:10.320880 ts_soup-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0      607 2024-04-14 06:14:02.000000 ts_soup-0.1.8/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-14 06:14:10.320880 ts_soup-0.1.8/ts_soup/
--rw-rw-rw-   0        0        0      373 2024-04-11 23:30:37.000000 ts_soup-0.1.8/ts_soup/__init__.py
--rw-rw-rw-   0        0        0     1418 2024-04-05 21:49:15.000000 ts_soup-0.1.8/ts_soup/app.py
--rw-rw-rw-   0        0        0    15226 2024-04-14 00:57:30.000000 ts_soup-0.1.8/ts_soup/common.py
-drwxrwxrwx   0        0        0        0 2024-04-14 06:14:10.320880 ts_soup-0.1.8/ts_soup/workers/
--rw-rw-rw-   0        0        0       78 2024-04-05 04:01:53.000000 ts_soup-0.1.8/ts_soup/workers/__init__.py
--rw-rw-rw-   0        0        0     3689 2024-04-05 09:36:43.000000 ts_soup-0.1.8/ts_soup/workers/sources.py
--rw-rw-rw-   0        0        0     5525 2024-04-14 06:13:41.000000 ts_soup-0.1.8/ts_soup/workers/targets.py
-drwxrwxrwx   0        0        0        0 2024-04-14 06:14:10.320880 ts_soup-0.1.8/ts_soup.egg-info/
--rw-rw-rw-   0        0        0     1028 2024-04-14 06:14:10.000000 ts_soup-0.1.8/ts_soup.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      277 2024-04-14 06:14:10.000000 ts_soup-0.1.8/ts_soup.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-14 06:14:10.000000 ts_soup-0.1.8/ts_soup.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-14 06:14:10.000000 ts_soup-0.1.8/ts_soup.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-16 04:44:53.097109 ts_soup-0.1.9/
+-rw-rw-rw-   0        0        0     1028 2024-04-16 04:44:53.096108 ts_soup-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0      686 2024-04-07 01:22:11.000000 ts_soup-0.1.9/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-16 04:44:53.097109 ts_soup-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0      607 2024-04-16 04:44:43.000000 ts_soup-0.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-16 04:44:53.082282 ts_soup-0.1.9/ts_soup/
+-rw-rw-rw-   0        0        0      373 2024-04-09 03:17:12.000000 ts_soup-0.1.9/ts_soup/__init__.py
+-rw-rw-rw-   0        0        0     1418 2024-04-07 01:22:11.000000 ts_soup-0.1.9/ts_soup/app.py
+-rw-rw-rw-   0        0        0    15395 2024-04-16 04:44:23.000000 ts_soup-0.1.9/ts_soup/common.py
+drwxrwxrwx   0        0        0        0 2024-04-16 04:44:53.093267 ts_soup-0.1.9/ts_soup/workers/
+-rw-rw-rw-   0        0        0       78 2024-04-07 01:22:11.000000 ts_soup-0.1.9/ts_soup/workers/__init__.py
+-rw-rw-rw-   0        0        0     3689 2024-04-11 09:09:47.000000 ts_soup-0.1.9/ts_soup/workers/sources.py
+-rw-rw-rw-   0        0        0     5595 2024-04-16 04:43:29.000000 ts_soup-0.1.9/ts_soup/workers/targets.py
+drwxrwxrwx   0        0        0        0 2024-04-16 04:44:53.094268 ts_soup-0.1.9/ts_soup.egg-info/
+-rw-rw-rw-   0        0        0     1028 2024-04-16 04:44:53.000000 ts_soup-0.1.9/ts_soup.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      277 2024-04-16 04:44:53.000000 ts_soup-0.1.9/ts_soup.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-16 04:44:53.000000 ts_soup-0.1.9/ts_soup.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-16 04:44:53.000000 ts_soup-0.1.9/ts_soup.egg-info/top_level.txt
```

### Comparing `ts_soup-0.1.8/PKG-INFO` & `ts_soup-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ts-soup
-Version: 0.1.8
+Version: 0.1.9
 Summary: date series data synchronization
 Author: feihan ye
 Author-email: 445280206@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `ts_soup-0.1.8/README.md` & `ts_soup-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `ts_soup-0.1.8/setup.py` & `ts_soup-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r",encoding='utf8') as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="ts-soup",
-  version="0.1.8",
+  version="0.1.9",
   author="feihan ye",
   author_email="445280206@qq.com",
   description="date series data synchronization",
   long_description=long_description,
   long_description_content_type="text/markdown",
   # url="https://github.com/pypa/sampleproject",
   packages=setuptools.find_packages(),
```

### Comparing `ts_soup-0.1.8/ts_soup/app.py` & `ts_soup-0.1.9/ts_soup/app.py`

 * *Files identical despite different names*

### Comparing `ts_soup-0.1.8/ts_soup/common.py` & `ts_soup-0.1.9/ts_soup/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 import pandas as pd
 from functools import wraps
 import traceback
 
 import pymysql
 from sqlalchemy import create_engine
 
-
 warnings.filterwarnings('ignore')
 
 # 注册形成的数据库连接
 USABLE_DBS = {}
 
 CURRENT_DATE = None
 SYNC_FROM_DATE = None
@@ -87,15 +86,14 @@
                         get_sqlalchemy_engine(db_info, db_type)
                     else:
                         get_pymsql_engine(db_info, db_type)
 
             else:
                 raise ValueError('未配置engine类型')
 
-
     SYNC_FROM_DATE = sync_start
     CURRENT_DATE = sync_end
     to_update_tables = pd.read_sql('select * from to_update_tables', con=USABLE_DBS['targets_default'])['table_name']
     with USABLE_DBS['targets_default'].begin() as conn:
         conn.execute("""
         CREATE TABLE if not exists `updated_state`  (
                       `update_date` date DEFAULT NULL,
@@ -119,30 +117,31 @@
     both_columns = [i for i in to_update_tables if i in pivot_table.columns.values.tolist()]  # 原来记录里有且现在仍需要的表
 
     non_columns = [i for i in to_update_tables if i not in pivot_table.columns.values.tolist()]  # 原来记录没有现在新增的表
     DATA_UPDATED_STATE = pivot_table[both_columns].fillna(0)
     DATA_UPDATED_STATE[non_columns] = 0
     DATA_UPDATED_STATE = DATA_UPDATED_STATE.reset_index()
     DATA_UPDATED_STATE['update_date'] = DATA_UPDATED_STATE['update_date'].apply(lambda x: x.strftime('%Y-%m-%d'))
-    to_update_tables = customized_table if len(customized_table)>0 else to_update_tables
+    to_update_tables = customized_table if len(customized_table) > 0 else to_update_tables
     if len(customized_time) > 0:
         DATA_UPDATED_STATE = DATA_UPDATED_STATE.set_index('update_date')
         for one_date in customized_time:
             DATA_UPDATED_STATE.loc[one_date, to_update_tables] = 0
         DATA_UPDATED_STATE = DATA_UPDATED_STATE.loc[customized_time, to_update_tables]
         DATA_UPDATED_STATE = DATA_UPDATED_STATE.reset_index()
     return to_update_tables
 
 
 class BaseSource(ABC):
     """
     定义需要使用在入口函数中注册的数据库连接的source的基类，即 如果需要使用数据库连接，则需要继承BaseSource
     """
+
     def __init__(self,
-                 db:str=None,
+                 db: str = None,
                  index_field: str = 'date',
                  empty_check: bool = True):
         """
         :param db: 数据库名
         :param index_field: 数据源筛选日期的字段，如果不提供则默认"date",如果需要查询全表，则index_field需要设置为 None。
         :param empty_check: 是否为当前方法主要数据源（除了配置信息的数据源），判空时使用，若不想使当前数据源参与判空，可设为 False
         """
@@ -162,15 +161,16 @@
         pass
 
 
 class BaseTarget(ABC):
     """
     定义需要使用在入口函数中注册的数据库连接的target的基类，即 如果需要使用数据库连接，则需要继承BaseTarget
     """
-    def __init__(self,db: str = None):
+
+    def __init__(self, db: str = None):
         if db:
             self.db = USABLE_DBS.get(db)
             self.db_pym = USABLE_DBS.get(f'{db}_pym')
             self.db_str = db
         else:
             self.db = USABLE_DBS.get('targets_default')
             self.db_pym = USABLE_DBS.get('targets_default_pym')
@@ -181,38 +181,35 @@
         """
         :param to_update_date:
         :return: yyyy-mm-dd 格式日期列表
         """
         pass
 
 
-
-
 class Executor:
     """
     数据处理原则：
         n2one: 数据源配置为is_data=True的对应日期查询结果只要存在一个全为空，则视当天的所有数据都为空，不更新数据表，也不更新操作记录表(updated_state)
         one2n:
                如果数据结果存在一个 None或者 emptyDataframe ，则当次调用 updated_state 表不更新
                如果数据结果全都有值，但是存在个别天数的行中存在空数据，则会删除空数据对应的行，updated_state更新取每个数据结果的交集作为日期
     """
 
-    def __init__(self, sources, targets, executed_table,customized_updated_state=None):
+    def __init__(self, sources, targets, executed_table, customized_updated_state=None):
         """
         数据库的操作器，负责从源表读取数据 _make_source_data，以及写入目标表 _handle_result
         """
         self.any_source_empty = False
         self.value = []
         self.sources = sources
         self.targets = targets
         self.source_data = []
         self.executed_table = executed_table
         self.to_update_date = self.__get_update_date()
 
-
     def __get_update_date(self):
         return DATA_UPDATED_STATE.loc[~(DATA_UPDATED_STATE[self.executed_table] == 1), 'update_date']
 
     def make_source_data(self):
         """
         产生数据源source_data的方法，按照TargetInfo顺序写入 source_data中
         判断传入的主要数据源（除了配置信息）是存在空，如果存在空则视所有数据源都为空，当天数据未更新
@@ -222,15 +219,15 @@
             data = source.build_source(self.to_update_date)
             """
             判断数据源（empty_check设置为True的）是否存在空，如果存在空则视所有数据源都为空，当天数据未更新
             主要目的是为了避免需要频繁在funcs的处理逻辑中增加判空的判断，也可以手动给某数据源设置为False,如果某数据源
             empty_check设置为False，需要在数据处理逻辑中对data_source是否为空进行判断，不然当下文在进行数据处理时
             使用行列索引，如果df是空容易导致keyError错误。
             """
-            if hasattr(source,'empty_check'):
+            if hasattr(source, 'empty_check'):
                 if source.empty_check and data.empty:
                     self.any_source_empty = True
                     for _ in self.targets:
                         self.value.append(None)
                     return
             else:
                 raise ValueError("source.empty_check未设置")
@@ -261,25 +258,26 @@
 
             # 调用统一接口完成成果产出，返回每个target更新的日期，最后取交集作为该func的完成同步的日期
             # 先统一转datetime，再转str
             updated_date = target.build_output(cur_result)
             if updated_date is None:
                 continue
             date_df = pd.to_datetime(updated_date)
-            updated_date = pd.DataFrame(date_df, columns=['update_date']).drop_duplicates().applymap(lambda x:x.strftime('%Y-%m-%d'))
+            updated_date = pd.DataFrame(date_df, columns=['update_date']).drop_duplicates().applymap(
+                lambda x: x.strftime('%Y-%m-%d'))
 
             # 如果未传入自定义更新日期，则取数据日期作为 处理操作表的更新日期，取各数据结果交集
             if update_state_date is not None:
                 update_state_date = update_state_date.merge(
-                    pd.DataFrame(updated_date,columns=['update_date']).drop_duplicates(),
+                    pd.DataFrame(updated_date, columns=['update_date']).drop_duplicates(),
                     on='update_date',
                     how='inner'
                 )[['update_date']]
             else:
-                update_state_date = pd.DataFrame(updated_date,columns=['update_date']).drop_duplicates()
+                update_state_date = pd.DataFrame(updated_date, columns=['update_date']).drop_duplicates()
 
         # 将方法的操作记录写入数据库
         if func_update_flag:
             if update_state_date is not None and not update_state_date.empty:
                 self.__handle_insert_update_state(update_state_date)
 
     def __handle_insert_update_state(self, update_state):
@@ -319,22 +317,24 @@
                                     executed_table=func.__name__)
 
                 # 表示该方法已同步完所有数据，则不再执行后续操作
                 if len(executor.to_update_date) == 0:
                     print(f'{func.__name__} 方法已同步至最新')
                     return
 
+                print('>' * 20 + f' {func.__name__} 开始' + '>' * 20)
                 if len(sources) != 0:
                     executor.make_source_data()
 
                 # empty_check为True且有一天数据源为空则不执行数据处理函数
                 if not executor.any_source_empty:
                     func(executor)
 
                 executor.handle_result()
+                print('<' * 20 + f' {func.__name__} 结束' + '<' * 20)
             except Exception:
                 global EXECUTE_STATE
                 EXECUTE_STATE = False
                 print(executor.executed_table + '同步失败')
                 print(traceback.format_exc())
 
         return inner_wrapper
```

### Comparing `ts_soup-0.1.8/ts_soup/workers/sources.py` & `ts_soup-0.1.9/ts_soup/workers/sources.py`

 * *Files identical despite different names*

### Comparing `ts_soup-0.1.8/ts_soup/workers/targets.py` & `ts_soup-0.1.9/ts_soup/workers/targets.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from ts_soup.common import BaseTarget,query_in_sql
+from ts_soup.common import BaseTarget, query_in_sql
 import pandas as pd
 from dateutil.relativedelta import relativedelta
 import datetime
 
 
 class TargetTable(BaseTarget):
     def __init__(self, tb,
@@ -24,36 +24,32 @@
         :param drop_na_thresh:如果该轴不为nan的值的个数少于 drop_na_thresh设置的值，进行dropna操作
         :param has_unique_idx:是否存在唯一索引或主键，以使用replace_into语句，默认关闭，需要表添加唯一索引或主键后才能开启
                 否则会出现数据重复
         :param is_empty_effect:表示该target  数据为空 是否影响update_state设置为 1 ,True表示数据为空，不能设置为 1
         否则会出现数据重复
         """
         super().__init__(
-                         db,
-                         )
+            db,
+        )
         self.tb = tb
         self.index_field = index_field
         self.drop_axis = drop_axis
         self.drop_na_subset = drop_na_subset
         self.drop_na_thresh = drop_na_thresh
         self.has_unique_idx = has_unique_idx
         self.is_empty_effect = is_empty_effect
 
     def build_output(self, cur_result):
         # 写库
 
         # is_empty_effect 为True，表示如果该target数据为空，需要在以后再同步，因此当天update_state 不能设置为1
         # 返回none则不会进行交集，因此不影响其他target update_state设置完成情况
         if cur_result.empty:
-
-            if self.is_empty_effect:
-                print(f'{self.tb} 无数据同步,影响最终update_state状态日期设置')
-                return []
-            print(f'{self.tb} 无数据同步,不影响最终update_state状态日期设置')
-            return
+            print(f'{self.tb} 无数据同步')
+            return [] if self.is_empty_effect else None
 
         # 统一把index_field字段转为str类型，防止后面在insert_update_state 和各表插入数据时 使用datetime64 或 int等类型
         # datetime.date 在dataframe中有可能是Object类型
         if str(cur_result[self.index_field].dtypes) == 'datetime64' or str(
                 cur_result[self.index_field].dtypes).lower() == 'object':
             cur_result[self.index_field] = pd.to_datetime(cur_result[self.index_field]).apply(
                 lambda x: x.strftime('%Y-%m-%d'))
@@ -72,52 +68,49 @@
         params = {'axis': self.drop_axis}
         if self.drop_na_subset:
             params['subset'] = self.drop_na_subset
         if self.drop_na_thresh:
             params['thresh'] = self.drop_na_thresh
 
         updated_date = []
+        not_updated_date = []
         groups = cur_result.groupby(by=self.index_field, dropna=False)
         for index, group in groups:
             rows = group.shape[0]
             new_df = group.dropna(**params)
             new_rows = new_df.shape[0]
             if rows == new_rows:
                 updated_date.append(index)
             else:
-                print(f'{self.tb} {index}因数据不全(dropna)导致update_state当天日期未更新')
+                not_updated_date.append(index)
+        if len(not_updated_date) != 0:
+            print(f'{self.tb} 因数据不全(多个字段有至少一个字段为Null)导致update_state当天日期未更新：\n{",".join(sorted(not_updated_date, reverse=True))}')
         return updated_date
 
-
-    def __execute_sql(self,cur_result):
+    def __execute_sql(self, cur_result):
         """
         需要写库的操作
         :param cur_result:
         :return:
         """
         # 设置了使用replace_into语句(多重索引的情况下无法使用sqlalchemy)，此时需要表设置唯一索引或者主键
         if self.has_unique_idx:
             # 使用Pymysql的连接
             insert_field = cur_result.columns.values.tolist()
             cursor = self.db_pym.cursor()
             try:
-                cursor.executemany(f'replace into {self.tb} ({",".join(insert_field)}) values ({",".join(["%s" for _ in range(len(insert_field))])})',cur_result.values.tolist())
+                cursor.executemany(
+                    f'replace into {self.tb} ({",".join(insert_field)}) values ({",".join(["%s" for _ in range(len(insert_field))])})',
+                    cur_result.values.tolist())
                 self.db_pym.commit()
             except Exception:
                 import traceback
                 print(traceback.format_exc())
                 self.db_pym.rollback()
                 raise Exception('数据库操作错误!')
         else:
             with self.db.begin() as conn:
-                conn.execute(f'delete from {self.tb} where {self.index_field} in ({query_in_sql(cur_result[self.index_field].values.tolist())})')
+                conn.execute(
+                    f'delete from {self.tb} where {self.index_field} in ({query_in_sql(cur_result[self.index_field].values.tolist())})')
                 cur_result.to_sql(self.tb, con=conn, if_exists='append', index=False)
-        print(f'{self.db_str}：{self.tb} 更新成功，更新日期为：\n{",".join(cur_result[self.index_field].drop_duplicates().values.tolist())}')
-
-
-
-
-
-
-
-
-
+        print(
+            f'{self.tb} 更新成功，更新日期为：\n{",".join(cur_result[self.index_field].drop_duplicates().sort_values(ascending=False).values.tolist())}')
```

### Comparing `ts_soup-0.1.8/ts_soup.egg-info/PKG-INFO` & `ts_soup-0.1.9/ts_soup.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ts-soup
-Version: 0.1.8
+Version: 0.1.9
 Summary: date series data synchronization
 Author: feihan ye
 Author-email: 445280206@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

