# Comparing `tmp/sparrowSql-0.1.1.tar.gz` & `tmp/sparrowSql-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sparrowSql-0.1.1.tar", last modified: Mon Apr 15 07:37:00 2024, max compression
+gzip compressed data, was "sparrowSql-0.1.2.tar", last modified: Tue Apr 16 05:45:46 2024, max compression
```

## Comparing `sparrowSql-0.1.1.tar` & `sparrowSql-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 07:37:00.362148 sparrowSql-0.1.1/
--rw-rw-rw-   0        0        0      199 2024-04-15 07:37:00.361209 sparrowSql-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-15 07:37:00.362547 sparrowSql-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      290 2024-04-15 07:36:57.000000 sparrowSql-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-15 07:37:00.351981 sparrowSql-0.1.1/sparrowSql/
--rw-rw-rw-   0        0        0     2743 2024-04-12 08:24:31.000000 sparrowSql-0.1.1/sparrowSql/SQL.py
--rw-rw-rw-   0        0        0      156 2024-04-15 07:10:45.000000 sparrowSql-0.1.1/sparrowSql/__init__.py
--rw-rw-rw-   0        0        0    19139 2024-04-15 05:53:11.000000 sparrowSql-0.1.1/sparrowSql/mariaDB.py
--rw-rw-rw-   0        0        0    19264 2024-04-15 05:53:11.000000 sparrowSql-0.1.1/sparrowSql/mysql.py
--rw-rw-rw-   0        0        0      745 2024-04-12 06:04:46.000000 sparrowSql-0.1.1/sparrowSql/sparrow.py
--rw-rw-rw-   0        0        0    17687 2024-04-15 07:32:50.000000 sparrowSql-0.1.1/sparrowSql/sqLite.py
-drwxrwxrwx   0        0        0        0 2024-04-15 07:37:00.359995 sparrowSql-0.1.1/sparrowSql.egg-info/
--rw-rw-rw-   0        0        0      199 2024-04-15 07:37:00.000000 sparrowSql-0.1.1/sparrowSql.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      303 2024-04-15 07:37:00.000000 sparrowSql-0.1.1/sparrowSql.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 07:37:00.000000 sparrowSql-0.1.1/sparrowSql.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-04-15 07:37:00.000000 sparrowSql-0.1.1/sparrowSql.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-15 07:37:00.000000 sparrowSql-0.1.1/sparrowSql.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-16 05:45:46.990142 sparrowSql-0.1.2/
+-rw-rw-rw-   0        0        0      199 2024-04-16 05:45:46.989301 sparrowSql-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-04-16 05:45:46.990642 sparrowSql-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      290 2024-04-16 05:45:39.000000 sparrowSql-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-16 05:45:46.977641 sparrowSql-0.1.2/sparrowSql/
+-rw-rw-rw-   0        0        0     3569 2024-04-16 05:39:03.000000 sparrowSql-0.1.2/sparrowSql/SQL.py
+-rw-rw-rw-   0        0        0      156 2024-04-15 07:10:45.000000 sparrowSql-0.1.2/sparrowSql/__init__.py
+-rw-rw-rw-   0        0        0    20817 2024-04-16 05:39:03.000000 sparrowSql-0.1.2/sparrowSql/mariaDB.py
+-rw-rw-rw-   0        0        0    20941 2024-04-16 05:39:03.000000 sparrowSql-0.1.2/sparrowSql/mysql.py
+-rw-rw-rw-   0        0        0      745 2024-04-12 06:04:46.000000 sparrowSql-0.1.2/sparrowSql/sparrow.py
+-rw-rw-rw-   0        0        0    19366 2024-04-16 05:39:03.000000 sparrowSql-0.1.2/sparrowSql/sqLite.py
+drwxrwxrwx   0        0        0        0 2024-04-16 05:45:46.987714 sparrowSql-0.1.2/sparrowSql.egg-info/
+-rw-rw-rw-   0        0        0      199 2024-04-16 05:45:46.000000 sparrowSql-0.1.2/sparrowSql.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      303 2024-04-16 05:45:46.000000 sparrowSql-0.1.2/sparrowSql.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-16 05:45:46.000000 sparrowSql-0.1.2/sparrowSql.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-04-16 05:45:46.000000 sparrowSql-0.1.2/sparrowSql.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-16 05:45:46.000000 sparrowSql-0.1.2/sparrowSql.egg-info/top_level.txt
```

### Comparing `sparrowSql-0.1.1/sparrowSql/SQL.py` & `sparrowSql-0.1.2/sparrowSql/SQL.py`

 * *Files 25% similar despite different names*

```diff
@@ -128,7 +128,48 @@
     def add_column(self):
         """
         向表中新增字段，该方法未被实现
         """
         print("该方法未被实现")
         pass
 
+    def create_index(self):
+        """
+        创建索引
+        """
+        print("该方法未被实现")
+        pass
+
+    def create_unique_index(self):
+        """
+        创建唯一索引
+        """
+        print("该方法未被实现")
+        pass
+
+    def drop_index(self):
+        """
+        删除索引
+        """
+        print("该方法未被实现")
+        pass
+
+    def start_transaction(self):
+        """
+        开始事务
+        """
+        print("该方法未被实现")
+        pass
+
+    def rollback_transaction(self):
+        """
+        回滚事务
+        """
+        print("该方法未被实现")
+        pass
+
+    def commit_transaction(self):
+        """
+        提交事务
+        """
+        print("该方法未被实现")
+        pass
```

### Comparing `sparrowSql-0.1.1/sparrowSql/mariaDB.py` & `sparrowSql-0.1.2/sparrowSql/mariaDB.py`

 * *Files 4% similar despite different names*

```diff
@@ -519,7 +519,67 @@
             constraint += " AUTOINCREMENT"
         sql = f"ALTER TABLE {table_name} ADD {column_name} {column_type}({length})"
         sql += constraint
         if is_first:
             sql += " FIRST"
         self._cursor_.execute(sql)
 
+    def create_index(self, table_name: str, column_name: str, index_name: str):
+        """
+        创建索引
+        :param table_name: 表名
+        :param column_name: 列名
+        :param index_name: 索引名
+        :return:
+        """
+        sql = f"CREATE INDEX {index_name} ON {table_name} ({column_name});"
+        self._cursor_.execute(sql)
+
+    def create_unique_index(self, table_name: str, column_name: str, index_name: str):
+        """
+        创建唯一索引
+        :param table_name: 表名
+        :param column_name: 列名
+        :param index_name: 索引名
+        :return:
+        """
+        sql = f"CREATE UNIQUE INDEX {index_name} ON {table_name} ({column_name});"
+        self._cursor_.execute(sql)
+
+    def drop_index(self, table_name: str, index_name: str):
+        """
+        删除索引
+        :param table_name: 表名
+        :param index_name: 索引名
+        :return:
+        """
+        sql = f"ALTER TABLE {table_name} DROP INDEX {index_name};"
+        self._cursor_.execute(sql)
+
+    def start_transaction(self):
+        """
+        开始事务
+        :return:
+        """
+        sql = "BEGIN TRANSACTION;"
+        self._cursor_.execute(sql)
+        print("事务开启...")
+
+    def rollback_transaction(self):
+        """
+        回滚事务
+        :return:
+        """
+        sql = "ROLLBACK;"
+        self._cursor_.execute(sql)
+        print("事务回滚...")
+
+    def commit_transaction(self):
+        """
+        提交事务
+        :return:
+        """
+        sql = "COMMIT;"
+        self._cursor_.execute(sql)
+        print("事务提交...")
+
+
```

### Comparing `sparrowSql-0.1.1/sparrowSql/mysql.py` & `sparrowSql-0.1.2/sparrowSql/mysql.py`

 * *Files 6% similar despite different names*

```diff
@@ -518,11 +518,71 @@
             constraint += " AUTOINCREMENT"
         sql = f"ALTER TABLE {table_name} ADD {column_name} {column_type}({length})"
         sql += constraint
         if is_first:
             sql += " FIRST"
         self._cursor_.execute(sql)
 
+    def create_index(self, table_name: str, column_name: str, index_name: str):
+        """
+        创建单列索引
+        :param table_name: 表名
+        :param column_name: 列名
+        :param index_name: 索引名
+        :return:
+        """
+        sql = f"CREATE INDEX {index_name} ON {table_name} ({column_name});"
+        self._cursor_.execute(sql)
+
+    def create_unique_index(self, table_name: str, column_name: str, index_name: str):
+        """
+        创建单列唯一索引
+        :param table_name: 表名
+        :param column_name: 列名
+        :param index_name: 索引名
+        :return:
+        """
+        sql = f"CREATE UNIQUE INDEX {index_name} ON {table_name} ({column_name});"
+        self._cursor_.execute(sql)
+
+    def drop_index(self, table_name: str, index_name: str):
+        """
+        删除索引
+        :param table_name: 表名
+        :param index_name: 索引名
+        :return:
+        """
+        sql = f"ALTER TABLE {table_name} DROP INDEX {index_name};"
+        self._cursor_.execute(sql)
+
+    def start_transaction(self):
+        """
+        开始事务
+        :return:
+        """
+        sql = "BEGIN TRANSACTION;"
+        self._cursor_.execute(sql)
+        print("事务开启...")
+
+    def rollback_transaction(self):
+        """
+        回滚事务
+        :return:
+        """
+        sql = "ROLLBACK;"
+        self._cursor_.execute(sql)
+        print("事务回滚...")
+
+    def commit_transaction(self):
+        """
+        提交事务
+        :return:
+        """
+        sql = "COMMIT;"
+        self._cursor_.execute(sql)
+        print("事务提交...")
+
+
 
 if __name__ == '__main__':
     run = MySQL("192.168.233.131", 3306, "root", "123456")
-    run.add_column("table_name", "c", "int", 20, is_first=True)
+    run.create_index("test", "name", "name_index")
```

### Comparing `sparrowSql-0.1.1/sparrowSql/sparrow.py` & `sparrowSql-0.1.2/sparrowSql/sparrow.py`

 * *Files identical despite different names*

### Comparing `sparrowSql-0.1.1/sparrowSql/sqLite.py` & `sparrowSql-0.1.2/sparrowSql/sqLite.py`

 * *Files 4% similar despite different names*

```diff
@@ -470,7 +470,67 @@
         if is_auto_increment:
             constraint += " AUTOINCREMENT"
         sql = f"ALTER TABLE {table_name} ADD {column_name} {column_type}({length})"
         sql += constraint
         if is_first:
             sql += " FIRST"
         self._cursor_.execute(sql)
+
+    def create_index(self, table_name: str, column_name: str, index_name: str):
+        """
+        创建索引
+        :param table_name: 表名
+        :param column_name: 列名
+        :param index_name: 索引名
+        :return:
+        """
+        sql = f"CREATE INDEX {index_name} ON {table_name} ({column_name});"
+        self._cursor_.execute(sql)
+
+    def create_unique_index(self, table_name: str, column_name: str, index_name: str):
+        """
+        创建唯一索引
+        :param table_name: 表名
+        :param column_name: 列名
+        :param index_name: 索引名
+        :return:
+        """
+        sql = f"CREATE UNIQUE INDEX {index_name} ON {table_name} ({column_name});"
+        self._cursor_.execute(sql)
+
+    def drop_index(self, table_name: str, index_name: str):
+        """
+        删除索引
+        :param table_name: 表名
+        :param index_name: 索引名
+        :return:
+        """
+        sql = f"DROP INDEX IF EXISTS {index_name}_on_{table_name};"
+        self._cursor_.execute(sql)
+
+    def start_transaction(self):
+        """
+        开始事务
+        :return:
+        """
+        sql = "BEGIN TRANSACTION;"
+        self._cursor_.execute(sql)
+        print("事务开启...")
+
+    def rollback_transaction(self):
+        """
+        回滚事务
+        :return:
+        """
+        sql = "ROLLBACK;"
+        self._cursor_.execute(sql)
+        print("事务回滚...")
+
+    def commit_transaction(self):
+        """
+        提交事务
+        :return:
+        """
+        sql = "COMMIT;"
+        self._cursor_.execute(sql)
+        print("事务提交...")
+
```

