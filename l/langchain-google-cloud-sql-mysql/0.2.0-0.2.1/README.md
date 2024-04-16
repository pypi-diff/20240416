# Comparing `tmp/langchain_google_cloud_sql_mysql-0.2.0-py3-none-any.whl.zip` & `tmp/langchain_google_cloud_sql_mysql-0.2.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 29964 bytes, number of entries: 13
--rw-r--r--  2.0 unx     1151 b- defN 24-Apr-08 23:12 langchain_google_cloud_sql_mysql/__init__.py
--rw-r--r--  2.0 unx     4636 b- defN 24-Apr-08 23:12 langchain_google_cloud_sql_mysql/chat_message_history.py
--rw-r--r--  2.0 unx    14907 b- defN 24-Apr-08 23:12 langchain_google_cloud_sql_mysql/engine.py
--rw-r--r--  2.0 unx     3430 b- defN 24-Apr-08 23:12 langchain_google_cloud_sql_mysql/indexes.py
--rw-r--r--  2.0 unx    11912 b- defN 24-Apr-08 23:12 langchain_google_cloud_sql_mysql/loader.py
--rw-rw-r--  2.0 unx        0 b- defN 24-Apr-08 23:12 langchain_google_cloud_sql_mysql/py.typed
--rw-r--r--  2.0 unx    29952 b- defN 24-Apr-08 23:12 langchain_google_cloud_sql_mysql/vectorstore.py
--rw-r--r--  2.0 unx      597 b- defN 24-Apr-08 23:12 langchain_google_cloud_sql_mysql/version.py
--rw-rw-r--  2.0 unx    11358 b- defN 24-Apr-08 23:14 langchain_google_cloud_sql_mysql-0.2.0.dist-info/LICENSE
--rw-r--r--  2.0 unx    18482 b- defN 24-Apr-08 23:14 langchain_google_cloud_sql_mysql-0.2.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-08 23:14 langchain_google_cloud_sql_mysql-0.2.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       33 b- defN 24-Apr-08 23:14 langchain_google_cloud_sql_mysql-0.2.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1326 b- defN 24-Apr-08 23:14 langchain_google_cloud_sql_mysql-0.2.0.dist-info/RECORD
-13 files, 97876 bytes uncompressed, 27670 bytes compressed:  71.7%
+Zip file size: 29961 bytes, number of entries: 13
+-rw-r--r--  2.0 unx     1151 b- defN 24-Apr-16 15:57 langchain_google_cloud_sql_mysql/__init__.py
+-rw-r--r--  2.0 unx     4636 b- defN 24-Apr-16 15:57 langchain_google_cloud_sql_mysql/chat_message_history.py
+-rw-r--r--  2.0 unx    14907 b- defN 24-Apr-16 15:57 langchain_google_cloud_sql_mysql/engine.py
+-rw-r--r--  2.0 unx     3430 b- defN 24-Apr-16 15:57 langchain_google_cloud_sql_mysql/indexes.py
+-rw-r--r--  2.0 unx    11912 b- defN 24-Apr-16 15:57 langchain_google_cloud_sql_mysql/loader.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Apr-16 15:57 langchain_google_cloud_sql_mysql/py.typed
+-rw-r--r--  2.0 unx    29956 b- defN 24-Apr-16 15:57 langchain_google_cloud_sql_mysql/vectorstore.py
+-rw-r--r--  2.0 unx      597 b- defN 24-Apr-16 15:57 langchain_google_cloud_sql_mysql/version.py
+-rw-rw-r--  2.0 unx    11358 b- defN 24-Apr-16 15:59 langchain_google_cloud_sql_mysql-0.2.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx    18482 b- defN 24-Apr-16 15:59 langchain_google_cloud_sql_mysql-0.2.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-16 15:59 langchain_google_cloud_sql_mysql-0.2.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       33 b- defN 24-Apr-16 15:59 langchain_google_cloud_sql_mysql-0.2.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1326 b- defN 24-Apr-16 15:59 langchain_google_cloud_sql_mysql-0.2.1.dist-info/RECORD
+13 files, 97880 bytes uncompressed, 27667 bytes compressed:  71.7%
```

## zipnote {}

```diff
@@ -18,23 +18,23 @@
 
 Filename: langchain_google_cloud_sql_mysql/vectorstore.py
 Comment: 
 
 Filename: langchain_google_cloud_sql_mysql/version.py
 Comment: 
 
-Filename: langchain_google_cloud_sql_mysql-0.2.0.dist-info/LICENSE
+Filename: langchain_google_cloud_sql_mysql-0.2.1.dist-info/LICENSE
 Comment: 
 
-Filename: langchain_google_cloud_sql_mysql-0.2.0.dist-info/METADATA
+Filename: langchain_google_cloud_sql_mysql-0.2.1.dist-info/METADATA
 Comment: 
 
-Filename: langchain_google_cloud_sql_mysql-0.2.0.dist-info/WHEEL
+Filename: langchain_google_cloud_sql_mysql-0.2.1.dist-info/WHEEL
 Comment: 
 
-Filename: langchain_google_cloud_sql_mysql-0.2.0.dist-info/top_level.txt
+Filename: langchain_google_cloud_sql_mysql-0.2.1.dist-info/top_level.txt
 Comment: 
 
-Filename: langchain_google_cloud_sql_mysql-0.2.0.dist-info/RECORD
+Filename: langchain_google_cloud_sql_mysql-0.2.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## langchain_google_cloud_sql_mysql/vectorstore.py

```diff
@@ -671,23 +671,23 @@
         distance_function = (
             f"{query_options.distance_measure.value}_distance"
             if query_options.distance_measure != DistanceMeasure.DOT_PRODUCT
             else query_options.distance_measure.value
         )
         if query_options.search_type == SearchType.KNN:
             filter = f"WHERE {filter}" if filter else ""
-            stmt = f"SELECT {column_query}, {distance_function}({self.embedding_column}, string_to_vector('{embedding}')) AS distance FROM {self.table_name} {filter} ORDER BY distance LIMIT {k};"
+            stmt = f"SELECT {column_query}, {distance_function}({self.embedding_column}, string_to_vector('{embedding}')) AS distance FROM `{self.table_name}` {filter} ORDER BY distance LIMIT {k};"
         else:
             filter = f"AND {filter}" if filter else ""
             num_partitions = (
                 f",num_partitions={query_options.num_partitions}"
                 if query_options.num_partitions
                 else ""
             )
-            stmt = f"SELECT {column_query}, {distance_function}({self.embedding_column}, string_to_vector('{embedding}')) AS distance FROM {self.table_name} WHERE NEAREST({self.embedding_column}) TO (string_to_vector('{embedding}'), 'num_neighbors={k}{num_partitions}') {filter} ORDER BY distance;"
+            stmt = f"SELECT {column_query}, {distance_function}({self.embedding_column}, string_to_vector('{embedding}')) AS distance FROM `{self.table_name}` WHERE NEAREST({self.embedding_column}) TO (string_to_vector('{embedding}'), 'num_neighbors={k}{num_partitions}') {filter} ORDER BY distance;"
 
         # return self.engine._fetch(stmt)
         if map_results:
             return self.engine._fetch(stmt)
         else:
             return self.engine._fetch_rows(stmt)
```

## langchain_google_cloud_sql_mysql/version.py

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.2.0"
+__version__ = "0.2.1"
```

## Comparing `langchain_google_cloud_sql_mysql-0.2.0.dist-info/LICENSE` & `langchain_google_cloud_sql_mysql-0.2.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `langchain_google_cloud_sql_mysql-0.2.0.dist-info/METADATA` & `langchain_google_cloud_sql_mysql-0.2.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-google-cloud-sql-mysql
-Version: 0.2.0
+Version: 0.2.1
 Summary: LangChain integrations for Google Cloud SQL for MySQL
 Author-email: Google LLC <googleapis-packages@google.com>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

## Comparing `langchain_google_cloud_sql_mysql-0.2.0.dist-info/RECORD` & `langchain_google_cloud_sql_mysql-0.2.1.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 langchain_google_cloud_sql_mysql/__init__.py,sha256=fH1Y3GlQnwHNFt16hPowLHtEULVMTv1MX-_91qot_rc,1151
 langchain_google_cloud_sql_mysql/chat_message_history.py,sha256=gx2o-QegU04V6fX8P-JfHpm_yVn2Et846pDrPGOevWk,4636
 langchain_google_cloud_sql_mysql/engine.py,sha256=zbr6TIr5jdOP6W21cDsIBwfvoXxAKPPwEpgDjWo6Twg,14907
 langchain_google_cloud_sql_mysql/indexes.py,sha256=sv6co_H0v1j1OwEL3SGTOV9mNt6x-aM-qwNXE1UL9ag,3430
 langchain_google_cloud_sql_mysql/loader.py,sha256=LPYEyoTc-_98zvTN_rtXG-gZdIBd8o5qWxbRvek7Kgk,11912
 langchain_google_cloud_sql_mysql/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-langchain_google_cloud_sql_mysql/vectorstore.py,sha256=cqP_aolGm-_H9xKWiHDFSCxlx7HlzngHslpNGydVb7U,29952
-langchain_google_cloud_sql_mysql/version.py,sha256=c32tFkU7bcWMAeqBrDdHTYBzbZPaJPvhWqbKnyY_LxM,597
-langchain_google_cloud_sql_mysql-0.2.0.dist-info/LICENSE,sha256=z8d0m5b2O9McPEK1xHG_dWgUBT6EfBDz6wA0F7xSPTA,11358
-langchain_google_cloud_sql_mysql-0.2.0.dist-info/METADATA,sha256=LKGEmVIej9dMKgO7fVsuFGZv6LIZ2EIphFQ-sqQ_hY4,18482
-langchain_google_cloud_sql_mysql-0.2.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-langchain_google_cloud_sql_mysql-0.2.0.dist-info/top_level.txt,sha256=66mG3PXjFtwydGTUP8umus8EqCXttsD9B01ulc-Q67g,33
-langchain_google_cloud_sql_mysql-0.2.0.dist-info/RECORD,,
+langchain_google_cloud_sql_mysql/vectorstore.py,sha256=Bkw4CpTxlpRWbDOp4-oQ5_En01ghwuNEhNjYzZrbPNk,29956
+langchain_google_cloud_sql_mysql/version.py,sha256=lal6j0-2qdxqYCLjy1FcTVeiboHQADADWfCBuVKcU3k,597
+langchain_google_cloud_sql_mysql-0.2.1.dist-info/LICENSE,sha256=z8d0m5b2O9McPEK1xHG_dWgUBT6EfBDz6wA0F7xSPTA,11358
+langchain_google_cloud_sql_mysql-0.2.1.dist-info/METADATA,sha256=u5FbLzIt79a1uzE04syXCOINl1SnZ2YXtcDSvbbh_4c,18482
+langchain_google_cloud_sql_mysql-0.2.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+langchain_google_cloud_sql_mysql-0.2.1.dist-info/top_level.txt,sha256=66mG3PXjFtwydGTUP8umus8EqCXttsD9B01ulc-Q67g,33
+langchain_google_cloud_sql_mysql-0.2.1.dist-info/RECORD,,
```

