# Comparing `tmp/sparrowSql-0.1.tar.gz` & `tmp/sparrowSql-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sparrowSql-0.1.tar", last modified: Mon Apr 15 06:04:56 2024, max compression
+gzip compressed data, was "sparrowSql-0.1.1.tar", last modified: Mon Apr 15 07:37:00 2024, max compression
```

## Comparing `sparrowSql-0.1.tar` & `sparrowSql-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 06:04:56.423661 sparrowSql-0.1/
--rw-rw-rw-   0        0        0      197 2024-04-15 06:04:56.422444 sparrowSql-0.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-15 06:04:56.423661 sparrowSql-0.1/setup.cfg
--rw-rw-rw-   0        0        0      288 2024-04-15 05:27:25.000000 sparrowSql-0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-15 06:04:56.412725 sparrowSql-0.1/sparrowSql/
--rw-rw-rw-   0        0        0     2743 2024-04-12 08:24:31.000000 sparrowSql-0.1/sparrowSql/SQL.py
--rw-rw-rw-   0        0        0      118 2024-04-15 05:25:39.000000 sparrowSql-0.1/sparrowSql/__init__.py
--rw-rw-rw-   0        0        0    19139 2024-04-15 05:53:11.000000 sparrowSql-0.1/sparrowSql/mariaDB.py
--rw-rw-rw-   0        0        0    19264 2024-04-15 05:53:11.000000 sparrowSql-0.1/sparrowSql/mysql.py
--rw-rw-rw-   0        0        0      745 2024-04-12 06:04:46.000000 sparrowSql-0.1/sparrowSql/sparrow.py
--rw-rw-rw-   0        0        0    17711 2024-04-15 05:49:58.000000 sparrowSql-0.1/sparrowSql/sqLite.py
-drwxrwxrwx   0        0        0        0 2024-04-15 06:04:56.420676 sparrowSql-0.1/sparrowSql.egg-info/
--rw-rw-rw-   0        0        0      197 2024-04-15 06:04:56.000000 sparrowSql-0.1/sparrowSql.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      303 2024-04-15 06:04:56.000000 sparrowSql-0.1/sparrowSql.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 06:04:56.000000 sparrowSql-0.1/sparrowSql.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-04-15 06:04:56.000000 sparrowSql-0.1/sparrowSql.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-15 06:04:56.000000 sparrowSql-0.1/sparrowSql.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-15 07:37:00.362148 sparrowSql-0.1.1/
+-rw-rw-rw-   0        0        0      199 2024-04-15 07:37:00.361209 sparrowSql-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-04-15 07:37:00.362547 sparrowSql-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      290 2024-04-15 07:36:57.000000 sparrowSql-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-15 07:37:00.351981 sparrowSql-0.1.1/sparrowSql/
+-rw-rw-rw-   0        0        0     2743 2024-04-12 08:24:31.000000 sparrowSql-0.1.1/sparrowSql/SQL.py
+-rw-rw-rw-   0        0        0      156 2024-04-15 07:10:45.000000 sparrowSql-0.1.1/sparrowSql/__init__.py
+-rw-rw-rw-   0        0        0    19139 2024-04-15 05:53:11.000000 sparrowSql-0.1.1/sparrowSql/mariaDB.py
+-rw-rw-rw-   0        0        0    19264 2024-04-15 05:53:11.000000 sparrowSql-0.1.1/sparrowSql/mysql.py
+-rw-rw-rw-   0        0        0      745 2024-04-12 06:04:46.000000 sparrowSql-0.1.1/sparrowSql/sparrow.py
+-rw-rw-rw-   0        0        0    17687 2024-04-15 07:32:50.000000 sparrowSql-0.1.1/sparrowSql/sqLite.py
+drwxrwxrwx   0        0        0        0 2024-04-15 07:37:00.359995 sparrowSql-0.1.1/sparrowSql.egg-info/
+-rw-rw-rw-   0        0        0      199 2024-04-15 07:37:00.000000 sparrowSql-0.1.1/sparrowSql.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      303 2024-04-15 07:37:00.000000 sparrowSql-0.1.1/sparrowSql.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 07:37:00.000000 sparrowSql-0.1.1/sparrowSql.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-04-15 07:37:00.000000 sparrowSql-0.1.1/sparrowSql.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-15 07:37:00.000000 sparrowSql-0.1.1/sparrowSql.egg-info/top_level.txt
```

### Comparing `sparrowSql-0.1/sparrowSql/SQL.py` & `sparrowSql-0.1.1/sparrowSql/SQL.py`

 * *Files identical despite different names*

### Comparing `sparrowSql-0.1/sparrowSql/mariaDB.py` & `sparrowSql-0.1.1/sparrowSql/mariaDB.py`

 * *Files identical despite different names*

### Comparing `sparrowSql-0.1/sparrowSql/mysql.py` & `sparrowSql-0.1.1/sparrowSql/mysql.py`

 * *Files identical despite different names*

### Comparing `sparrowSql-0.1/sparrowSql/sparrow.py` & `sparrowSql-0.1.1/sparrowSql/sparrow.py`

 * *Files identical despite different names*

### Comparing `sparrowSql-0.1/sparrowSql/sqLite.py` & `sparrowSql-0.1.1/sparrowSql/sqLite.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,16 +11,16 @@
         self._cursor_.close()
         self._connect_.close()
 
     def commit(self):
         self._connect_.commit()
 
     def commit_close(self):
-        self.close()
         self.commit()
+        self.close()
 
     def user_defined_sql(self, sql: str, params: tuple = None):
         """
         运行自定义SQL\n
         在不输入参数: user_defined_sql('select name from user where id = 1')\n
         输入参数: user_defined_sql('select name from user where id = ?', (1))
         :param sql: SQL
@@ -55,15 +55,14 @@
                     for value_s in value:
                         params += (value_s,)
                     value_list.append("(" + ", ".join(["?" for i in value]) + ")")
                 else:
                     raise Exception(f"{columns}->{len(columns)} != {value}->{len(value)}")
             values = ", ".join(value_list)
             sql = f"insert into {table} {column} values {values};"
-            print(sql)
             self._cursor_.execute(sql, params)
             return sql
         else:
             params = ()
             if len(values) == len(columns):
                 for value_s in values:
                     params += (value_s,)
```

