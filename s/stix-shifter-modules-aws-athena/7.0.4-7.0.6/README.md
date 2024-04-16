# Comparing `tmp/stix_shifter_modules_aws_athena-7.0.4-py2.py3-none-any.whl.zip` & `tmp/stix_shifter_modules_aws_athena-7.0.6-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,40 +1,41 @@
-Zip file size: 80950 bytes, number of entries: 38
--rw-rw-r--  2.0 unx        0 b- defN 24-Mar-14 15:47 stix_shifter_modules/aws_athena/__init__.py
--rw-rw-r--  2.0 unx     1374 b- defN 24-Mar-14 15:47 stix_shifter_modules/aws_athena/entry_point.py
--rw-rw-r--  2.0 unx   240254 b- defN 24-Mar-14 15:49 stix_shifter_modules/aws_athena/configuration/config.json
--rw-rw-r--  2.0 unx      229 b- defN 24-Mar-14 15:49 stix_shifter_modules/aws_athena/configuration/dialects.json
--rw-rw-r--  2.0 unx     5053 b- defN 24-Mar-14 15:49 stix_shifter_modules/aws_athena/configuration/lang_en.json
--rw-rw-r--  2.0 unx        0 b- defN 24-Mar-14 15:47 stix_shifter_modules/aws_athena/stix_translation/__init__.py
--rw-rw-r--  2.0 unx    26842 b- defN 24-Mar-14 15:49 stix_shifter_modules/aws_athena/stix_translation/json_to_stix_translator.py
--rw-rw-r--  2.0 unx    24044 b- defN 24-Mar-14 15:47 stix_shifter_modules/aws_athena/stix_translation/query_constructor.py
--rw-rw-r--  2.0 unx     1024 b- defN 24-Mar-14 15:47 stix_shifter_modules/aws_athena/stix_translation/query_translator.py
--rw-rw-r--  2.0 unx     1075 b- defN 24-Mar-14 15:47 stix_shifter_modules/aws_athena/stix_translation/transformers.py
--rw-rw-r--  2.0 unx     4765 b- defN 24-Mar-14 15:47 stix_shifter_modules/aws_athena/stix_translation/json/guardduty_config.json
--rw-rw-r--  2.0 unx     1894 b- defN 24-Mar-14 15:47 stix_shifter_modules/aws_athena/stix_translation/json/guardduty_from_stix_map.json
--rw-rw-r--  2.0 unx    10146 b- defN 24-Mar-14 15:47 stix_shifter_modules/aws_athena/stix_translation/json/guardduty_to_stix_map.json
--rw-rw-r--  2.0 unx      139 b- defN 24-Mar-14 15:47 stix_shifter_modules/aws_athena/stix_translation/json/hash_algorithm_map.json
--rw-rw-r--  2.0 unx     2439 b- defN 24-Mar-14 15:47 stix_shifter_modules/aws_athena/stix_translation/json/network_protocol_map.json
--rw-rw-r--  2.0 unx    18300 b- defN 24-Mar-14 15:47 stix_shifter_modules/aws_athena/stix_translation/json/ocsf_from_stix_map.json
--rw-rw-r--  2.0 unx    75601 b- defN 24-Mar-14 15:47 stix_shifter_modules/aws_athena/stix_translation/json/ocsf_to_stix_map.json
--rw-rw-r--  2.0 unx      591 b- defN 24-Mar-14 15:47 stix_shifter_modules/aws_athena/stix_translation/json/operators.json
--rw-rw-r--  2.0 unx      814 b- defN 24-Mar-14 15:47 stix_shifter_modules/aws_athena/stix_translation/json/vpcflow_from_stix_map.json
--rw-rw-r--  2.0 unx     2350 b- defN 24-Mar-14 15:47 stix_shifter_modules/aws_athena/stix_translation/json/vpcflow_to_stix_map.json
--rw-rw-r--  2.0 unx     1894 b- defN 24-Mar-14 15:47 stix_shifter_modules/aws_athena/stix_translation/json/stix_2_1/guardduty_from_stix_map.json
--rw-rw-r--  2.0 unx    18297 b- defN 24-Mar-14 15:47 stix_shifter_modules/aws_athena/stix_translation/json/stix_2_1/ocsf_from_stix_map.json
--rw-rw-r--  2.0 unx    93792 b- defN 24-Mar-14 15:47 stix_shifter_modules/aws_athena/stix_translation/json/stix_2_1/to_stix_map.json
--rw-rw-r--  2.0 unx      891 b- defN 24-Mar-14 15:47 stix_shifter_modules/aws_athena/stix_translation/json/stix_2_1/vpcflow_from_stix_map.json
--rw-rw-r--  2.0 unx        0 b- defN 24-Mar-14 15:47 stix_shifter_modules/aws_athena/stix_transmission/__init__.py
--rw-rw-r--  2.0 unx     4021 b- defN 24-Mar-14 15:47 stix_shifter_modules/aws_athena/stix_transmission/boto3_client.py
--rw-rw-r--  2.0 unx     1207 b- defN 24-Mar-14 15:47 stix_shifter_modules/aws_athena/stix_transmission/delete_connector.py
--rw-rw-r--  2.0 unx     1969 b- defN 24-Mar-14 15:47 stix_shifter_modules/aws_athena/stix_transmission/error_mapper.py
--rw-rw-r--  2.0 unx     1370 b- defN 24-Mar-14 15:47 stix_shifter_modules/aws_athena/stix_transmission/ping_connector.py
--rw-rw-r--  2.0 unx     7443 b- defN 24-Mar-14 15:47 stix_shifter_modules/aws_athena/stix_transmission/query_connector.py
--rw-rw-r--  2.0 unx    15539 b- defN 24-Mar-14 15:47 stix_shifter_modules/aws_athena/stix_transmission/results_connector.py
--rw-rw-r--  2.0 unx     3175 b- defN 24-Mar-14 15:47 stix_shifter_modules/aws_athena/stix_transmission/status_connector.py
--rw-rw-r--  2.0 unx    12786 b- defN 24-Mar-14 15:49 stix_shifter_modules_aws_athena-7.0.4.dist-info/LICENSE.md
--rw-rw-r--  2.0 unx     7175 b- defN 24-Mar-14 15:49 stix_shifter_modules_aws_athena-7.0.4.dist-info/METADATA
--rw-rw-r--  2.0 unx     1418 b- defN 24-Mar-14 15:49 stix_shifter_modules_aws_athena-7.0.4.dist-info/NOTICE
--rw-rw-r--  2.0 unx      110 b- defN 24-Mar-14 15:49 stix_shifter_modules_aws_athena-7.0.4.dist-info/WHEEL
--rw-rw-r--  2.0 unx       21 b- defN 24-Mar-14 15:49 stix_shifter_modules_aws_athena-7.0.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     4691 b- defN 24-Mar-14 15:49 stix_shifter_modules_aws_athena-7.0.4.dist-info/RECORD
-38 files, 592733 bytes uncompressed, 72870 bytes compressed:  87.7%
+Zip file size: 84367 bytes, number of entries: 39
+-rw-rw-r--  2.0 unx        0 b- defN 24-Apr-16 17:16 stix_shifter_modules/aws_athena/__init__.py
+-rw-rw-r--  2.0 unx     1374 b- defN 24-Apr-16 17:16 stix_shifter_modules/aws_athena/entry_point.py
+-rw-rw-r--  2.0 unx   240254 b- defN 24-Apr-16 17:18 stix_shifter_modules/aws_athena/configuration/config.json
+-rw-rw-r--  2.0 unx      229 b- defN 24-Apr-16 17:18 stix_shifter_modules/aws_athena/configuration/dialects.json
+-rw-rw-r--  2.0 unx     5053 b- defN 24-Apr-16 17:18 stix_shifter_modules/aws_athena/configuration/lang_en.json
+-rw-rw-r--  2.0 unx        0 b- defN 24-Apr-16 17:16 stix_shifter_modules/aws_athena/stix_translation/__init__.py
+-rw-rw-r--  2.0 unx    26842 b- defN 24-Apr-16 17:18 stix_shifter_modules/aws_athena/stix_translation/json_to_stix_translator.py
+-rw-rw-r--  2.0 unx    24044 b- defN 24-Apr-16 17:16 stix_shifter_modules/aws_athena/stix_translation/query_constructor.py
+-rw-rw-r--  2.0 unx     1024 b- defN 24-Apr-16 17:16 stix_shifter_modules/aws_athena/stix_translation/query_translator.py
+-rw-rw-r--  2.0 unx     1075 b- defN 24-Apr-16 17:16 stix_shifter_modules/aws_athena/stix_translation/transformers.py
+-rw-rw-r--  2.0 unx     4765 b- defN 24-Apr-16 17:16 stix_shifter_modules/aws_athena/stix_translation/json/guardduty_config.json
+-rw-rw-r--  2.0 unx     1894 b- defN 24-Apr-16 17:16 stix_shifter_modules/aws_athena/stix_translation/json/guardduty_from_stix_map.json
+-rw-rw-r--  2.0 unx    10146 b- defN 24-Apr-16 17:16 stix_shifter_modules/aws_athena/stix_translation/json/guardduty_to_stix_map.json
+-rw-rw-r--  2.0 unx      139 b- defN 24-Apr-16 17:16 stix_shifter_modules/aws_athena/stix_translation/json/hash_algorithm_map.json
+-rw-rw-r--  2.0 unx     2439 b- defN 24-Apr-16 17:16 stix_shifter_modules/aws_athena/stix_translation/json/network_protocol_map.json
+-rw-rw-r--  2.0 unx    18300 b- defN 24-Apr-16 17:16 stix_shifter_modules/aws_athena/stix_translation/json/ocsf_from_stix_map.json
+-rw-rw-r--  2.0 unx    75601 b- defN 24-Apr-16 17:16 stix_shifter_modules/aws_athena/stix_translation/json/ocsf_to_stix_map.json
+-rw-rw-r--  2.0 unx      591 b- defN 24-Apr-16 17:16 stix_shifter_modules/aws_athena/stix_translation/json/operators.json
+-rw-rw-r--  2.0 unx      814 b- defN 24-Apr-16 17:16 stix_shifter_modules/aws_athena/stix_translation/json/vpcflow_from_stix_map.json
+-rw-rw-r--  2.0 unx     2350 b- defN 24-Apr-16 17:16 stix_shifter_modules/aws_athena/stix_translation/json/vpcflow_to_stix_map.json
+-rw-rw-r--  2.0 unx     1894 b- defN 24-Apr-16 17:16 stix_shifter_modules/aws_athena/stix_translation/json/stix_2_1/guardduty_from_stix_map.json
+-rw-rw-r--  2.0 unx    18297 b- defN 24-Apr-16 17:16 stix_shifter_modules/aws_athena/stix_translation/json/stix_2_1/ocsf_from_stix_map.json
+-rw-rw-r--  2.0 unx    93792 b- defN 24-Apr-16 17:16 stix_shifter_modules/aws_athena/stix_translation/json/stix_2_1/to_stix_map.json
+-rw-rw-r--  2.0 unx      891 b- defN 24-Apr-16 17:16 stix_shifter_modules/aws_athena/stix_translation/json/stix_2_1/vpcflow_from_stix_map.json
+-rw-rw-r--  2.0 unx        0 b- defN 24-Apr-16 17:16 stix_shifter_modules/aws_athena/stix_transmission/__init__.py
+-rw-rw-r--  2.0 unx     4021 b- defN 24-Apr-16 17:16 stix_shifter_modules/aws_athena/stix_transmission/boto3_client.py
+-rw-rw-r--  2.0 unx     1207 b- defN 24-Apr-16 17:16 stix_shifter_modules/aws_athena/stix_transmission/delete_connector.py
+-rw-rw-r--  2.0 unx     1969 b- defN 24-Apr-16 17:16 stix_shifter_modules/aws_athena/stix_transmission/error_mapper.py
+-rw-rw-r--  2.0 unx     1370 b- defN 24-Apr-16 17:16 stix_shifter_modules/aws_athena/stix_transmission/ping_connector.py
+-rw-rw-r--  2.0 unx     7435 b- defN 24-Apr-16 17:16 stix_shifter_modules/aws_athena/stix_transmission/post_query_connector_error_handling.py
+-rw-rw-r--  2.0 unx    10418 b- defN 24-Apr-16 17:16 stix_shifter_modules/aws_athena/stix_transmission/query_connector.py
+-rw-rw-r--  2.0 unx    15539 b- defN 24-Apr-16 17:16 stix_shifter_modules/aws_athena/stix_transmission/results_connector.py
+-rw-rw-r--  2.0 unx     3473 b- defN 24-Apr-16 17:16 stix_shifter_modules/aws_athena/stix_transmission/status_connector.py
+-rw-rw-r--  2.0 unx    12786 b- defN 24-Apr-16 17:18 stix_shifter_modules_aws_athena-7.0.6.dist-info/LICENSE.md
+-rw-rw-r--  2.0 unx     7175 b- defN 24-Apr-16 17:18 stix_shifter_modules_aws_athena-7.0.6.dist-info/METADATA
+-rw-rw-r--  2.0 unx     1418 b- defN 24-Apr-16 17:18 stix_shifter_modules_aws_athena-7.0.6.dist-info/NOTICE
+-rw-rw-r--  2.0 unx      110 b- defN 24-Apr-16 17:18 stix_shifter_modules_aws_athena-7.0.6.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       21 b- defN 24-Apr-16 17:18 stix_shifter_modules_aws_athena-7.0.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     4837 b- defN 24-Apr-16 17:18 stix_shifter_modules_aws_athena-7.0.6.dist-info/RECORD
+39 files, 603587 bytes uncompressed, 76035 bytes compressed:  87.4%
```

## zipnote {}

```diff
@@ -81,35 +81,38 @@
 
 Filename: stix_shifter_modules/aws_athena/stix_transmission/error_mapper.py
 Comment: 
 
 Filename: stix_shifter_modules/aws_athena/stix_transmission/ping_connector.py
 Comment: 
 
+Filename: stix_shifter_modules/aws_athena/stix_transmission/post_query_connector_error_handling.py
+Comment: 
+
 Filename: stix_shifter_modules/aws_athena/stix_transmission/query_connector.py
 Comment: 
 
 Filename: stix_shifter_modules/aws_athena/stix_transmission/results_connector.py
 Comment: 
 
 Filename: stix_shifter_modules/aws_athena/stix_transmission/status_connector.py
 Comment: 
 
-Filename: stix_shifter_modules_aws_athena-7.0.4.dist-info/LICENSE.md
+Filename: stix_shifter_modules_aws_athena-7.0.6.dist-info/LICENSE.md
 Comment: 
 
-Filename: stix_shifter_modules_aws_athena-7.0.4.dist-info/METADATA
+Filename: stix_shifter_modules_aws_athena-7.0.6.dist-info/METADATA
 Comment: 
 
-Filename: stix_shifter_modules_aws_athena-7.0.4.dist-info/NOTICE
+Filename: stix_shifter_modules_aws_athena-7.0.6.dist-info/NOTICE
 Comment: 
 
-Filename: stix_shifter_modules_aws_athena-7.0.4.dist-info/WHEEL
+Filename: stix_shifter_modules_aws_athena-7.0.6.dist-info/WHEEL
 Comment: 
 
-Filename: stix_shifter_modules_aws_athena-7.0.4.dist-info/top_level.txt
+Filename: stix_shifter_modules_aws_athena-7.0.6.dist-info/top_level.txt
 Comment: 
 
-Filename: stix_shifter_modules_aws_athena-7.0.4.dist-info/RECORD
+Filename: stix_shifter_modules_aws_athena-7.0.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## stix_shifter_modules/aws_athena/stix_transmission/query_connector.py

```diff
@@ -1,7 +1,10 @@
+from venv import logger
+from stix_shifter_modules.aws_athena.stix_transmission import status_connector
+from stix_shifter_modules.aws_athena.stix_transmission.post_query_connector_error_handling import PostQueryConnectorErrorHandler
 from stix_shifter_utils.modules.base.stix_transmission.base_connector import BaseQueryConnector
 from stix_shifter_utils.utils.error_response import ErrorResponder
 import json
 import re
 import time
 import uuid
 
@@ -21,14 +24,15 @@
 
 class QueryConnector(BaseQueryConnector):
 
     def __init__(self, client, connection):
         self.client = client
         self.connection = connection
         self.connector = __name__.split('.')[1]
+        self.total_try_count = 0
 
     async def create_query_connection(self, query):
         """
         Function to create query connection
         :param query: dict, Query
         :return: dict
         """
@@ -43,54 +47,91 @@
                 return_obj = {'success': True, 'search_id': str(uuid.uuid4()) + '-dummy:' + query_service_type}
                 return return_obj
             for config in config_details:
                 if config not in self.connection.keys():
                     raise InvalidParameterException("{} is required for {} query operation".format(config,
                                                                                                    query_service_type))
             table_config = self.connection[config_details[0]] + '."' + self.connection[config_details[1]] + '"'
+            
             other_tables = ''
             findall = re.finditer("##UNNEST.*?##", query[query_service_type])
             if findall:
                 for match in findall:
                     if match.group():
                         match_str = str(match.group())
                         query[query_service_type] = query[query_service_type].replace(match_str, '')
                         other_tables += ' %s%s%s ' % ('LEFT JOIN ', match_str.replace('##', ''), ' ON TRUE ')
 
             if query_service_type == 'ocsf':
-                columns = await self.column_list(self.connection[config_details[1]])
+                columns = await self.column_list(self.connection[config_details[0]], self.connection[config_details[1]])
                 column_cast = []
                 for column in columns:
                     column_cast.append("CAST(%s as JSON) AS %s" % (column, column))
 
                 select_statement = "SELECT %s FROM %s%s WHERE " % (", ".join(column_cast), table_config, other_tables)
             else:
                 select_statement = "SELECT %s.* FROM %s%s WHERE " % (table_config, table_config, other_tables)
+                        
+            #self.get_list_of_columns_and_rows(query[query_service_type])
+            #await self.row_list(self.connection[config_details[0]], self.connection[config_details[1]])
             # for multiple observation operators union and intersect, select statement will be added
             if 'UNION' in query[query_service_type] or 'INTERSECT' in query[query_service_type]:
                 query_string = re.sub(r'\(\(', '(({}'.format(select_statement), query[query_service_type], 1)
-                query = query_string.replace('UNION (', 'UNION ({}'.format(select_statement)).\
+                query_with_select = query_string.replace('UNION (', 'UNION ({}'.format(select_statement)).\
                     replace('INTERSECT (', 'INTERSECT ({}'.format(select_statement))
             else:
-                query = select_statement + query[query_service_type]
+                query_with_select = select_statement + query[query_service_type]
             result_config = self.get_result_config()
-            query_args = {"QueryString": query, "ResultConfiguration": result_config}
-            response_dict = await self.client.makeRequest('athena', 'start_query_execution', **query_args)
-            return_obj['success'] = True
-            return_obj['search_id'] = response_dict['QueryExecutionId'] + ":" + query_service_type
-
+            
+            return await self.query_api(query_with_select, result_config, query_service_type, return_obj)
+            
         except Exception as ex:
             response_dict['__type'] = ex.__class__.__name__
             response_dict['message'] = ex
             ErrorResponder.fill_error(return_obj, response_dict, ['message'], connector=self.connector)
         return return_obj
 
-    async def column_list(self, table):
+    async def query_api(self, query, result_config, query_service_type, return_obj):
+        """Creates a query job and ensures that none of the columns requested are missing from the query.
+
+        Args:
+            query (String): The original query without modification. 
+            result_config (Dict): Query configuration.
+            query_service_type (String): The type of query ("OCSF", "VPCFlow, etc)
+            return_obj (Dict): Contains the metadata about the request.
+
+        Returns:
+            Dict: The metadata about the request such as the query/search ID and the status.
+        """
+        logger.debug(f"The current query is : {query}")
+
+        #Creates the initial query job.
+        query_args = {"QueryString": query, "ResultConfiguration": result_config}
+        response_dict = await self.client.makeRequest('athena', 'start_query_execution', **query_args)
+        return_obj['search_id'] = response_dict['QueryExecutionId'] + ":" + query_service_type
+
+        modified_query = dict()
+        modified_query = await PostQueryConnectorErrorHandler.check_status_for_missing_column(self.client, return_obj['search_id'], query)
+        #If the query is successful (or the exception isn't column related) than it's considered a success and exits.
+        #If 10 columns are not found or it fails to replace a column 10 times, than it exits (to prevent endless loops).
+        #If the query is not successful, than it will retry the query with the modified query.
+        if(modified_query == True or self.total_try_count > 10):
+            logger.debug(f"The number of attempts to remove missing columns was {self.total_try_count}")
+            if(self.total_try_count >= 10):
+                logger.warn("There were 10 failed exceptions related to columns. This could be because there were more invalid columns than 10, \
+                             or alternatively that the replacement failed to remove the offending column.")
+            return_obj['success'] = True
+            return return_obj
+        else:
+            self.total_try_count = self.total_try_count + 1
+            return await self.query_api(modified_query, result_config, query_service_type, return_obj)
+            
+    async def column_list(self, database, table):
         columns = []
-        query = "SELECT column_name FROM information_schema.columns WHERE table_name = '%s'" % table
+        query = f"SELECT column_name,data_type FROM information_schema.columns WHERE table_name = '{table}' AND table_schema = '{database}'" 
         result_config = self.get_result_config()
         query_args = {"QueryString": query, "ResultConfiguration": result_config}
         response_dict = await self.client.makeRequest('athena', 'start_query_execution', **query_args)
         execution_id = response_dict['QueryExecutionId']
 
         state = "RUNNING"
         max_execution = 10
@@ -129,14 +170,21 @@
             raise Exception("Error in deleting s3 metadata after Athena query: " + message)
         
         if not columns:
             raise InvalidParameterException('No Athena table with name ' + table)
 
         return columns
 
+    def get_rows_from_response(self, data, parent, row_list):
+        data = data.casefold()
+        ##Root of the tree.
+        if(data.startswith("row(".casefold()) or data.startwith("array(".casefold())):
+            remainder = data[data.find("("):data.rfind(")")]
+            self.get_rows_from_response(remainder, parent, row_list)            
+        
     def get_result_config(self):
         """
         Output location and encryption configuration are added
         :return: dict, result configuration
         """
         output_location = ''
         path = self.connection.get('s3_bucket_location').strip()
@@ -148,7 +196,8 @@
                 if char.isalnum():
                     output_location = 's3://' + split_path[i:]
                     break
         else:
             output_location = 's3://' + path
         result_config = {'OutputLocation': output_location}
         return result_config
+
```

## stix_shifter_modules/aws_athena/stix_transmission/status_connector.py

```diff
@@ -52,14 +52,16 @@
                 return_obj = {'success': True, 'status': 'COMPLETED', 'progress': 100}
                 return return_obj
             response_dict = await self.client.makeRequest('athena', 'get_query_execution', QueryExecutionId=search_id)
             return_obj['success'] = True
             return_obj['status'] = self._getstatus(response_dict.get('QueryExecution', 'FAILED').
                                                    get('Status', 'FAILED').
                                                    get('State', 'FAILED'))
+            if (response_dict != None and "QueryExecution" in response_dict and "Status" in response_dict["QueryExecution"] and "StateChangeReason" in response_dict["QueryExecution"]["Status"]):
+                return_obj['message'] = response_dict["QueryExecution"]["Status"]["StateChangeReason"]
             if return_obj['status'] == 'COMPLETED':
                 return_obj['progress'] = 100
             elif return_obj['status'] == 'RUNNING':
                 query_submit_time = response_dict.get('QueryExecution').get('Status').get('SubmissionDateTime')
                 if query_submit_time:
                     current_time = datetime.datetime.now(tzlocal())
                     time_delta = current_time - query_submit_time
```

## Comparing `stix_shifter_modules_aws_athena-7.0.4.dist-info/LICENSE.md` & `stix_shifter_modules_aws_athena-7.0.6.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `stix_shifter_modules_aws_athena-7.0.4.dist-info/METADATA` & `stix_shifter_modules_aws_athena-7.0.6.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stix_shifter_modules_aws_athena
-Version: 7.0.4
+Version: 7.0.6
 Summary: Tools and interface to translate STIX formatted results and queries to different data source formats and to set up appropriate connection strings for invoking and triggering actions in openwhisk
 Home-page: https://github.com/opencybersecurityalliance/stix-shifter
 Author: ibm
 Author-email: 
 Project-URL: Source, https://github.com/opencybersecurityalliance/stix-shifter
 Keywords: datasource stix translate transform transmit
 Classifier: License :: OSI Approved :: Apache Software License
```

## Comparing `stix_shifter_modules_aws_athena-7.0.4.dist-info/NOTICE` & `stix_shifter_modules_aws_athena-7.0.6.dist-info/NOTICE`

 * *Files identical despite different names*

## Comparing `stix_shifter_modules_aws_athena-7.0.4.dist-info/RECORD` & `stix_shifter_modules_aws_athena-7.0.6.dist-info/RECORD`

 * *Files 1% similar despite different names*

```diff
@@ -23,16 +23,17 @@
 stix_shifter_modules/aws_athena/stix_translation/json/stix_2_1/to_stix_map.json,sha256=Q3hVrbhWXE9i0jn9iaaswGXhRsR7B5QGSPSv-Vw3rxM,93792
 stix_shifter_modules/aws_athena/stix_translation/json/stix_2_1/vpcflow_from_stix_map.json,sha256=TDiBsk4GtUH98mK6_KBKfFcDoOo1UzF08lyFpHF9XqM,891
 stix_shifter_modules/aws_athena/stix_transmission/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 stix_shifter_modules/aws_athena/stix_transmission/boto3_client.py,sha256=8aOpYGLutmNNk3cr2olg5fj2zOk0f7Sjct7JwbHwCkQ,4021
 stix_shifter_modules/aws_athena/stix_transmission/delete_connector.py,sha256=D2A5li6TWgZvqpnDGLXVveLqYHlWI1evVWKYKeXT60M,1207
 stix_shifter_modules/aws_athena/stix_transmission/error_mapper.py,sha256=hKiytRjhZx2BVSP1o13h30krPYLMTRxuWrPa6dij-l0,1969
 stix_shifter_modules/aws_athena/stix_transmission/ping_connector.py,sha256=HkcSFvDlW71v6tBtMTcvAd_jQqit6Uh3YknjBu7YKmw,1370
-stix_shifter_modules/aws_athena/stix_transmission/query_connector.py,sha256=eOK6mHRwtASq4gZxOyqmSUvDDThxkDhhbdYQ8jOTweY,7443
+stix_shifter_modules/aws_athena/stix_transmission/post_query_connector_error_handling.py,sha256=7py2aaPdr2zFlRlndb42ZFvcZrDHPmO9pU-lt1z3xcc,7435
+stix_shifter_modules/aws_athena/stix_transmission/query_connector.py,sha256=r6em2euPvrgDCod82Lp3TkfVi1nZut-_gokuX1nptug,10418
 stix_shifter_modules/aws_athena/stix_transmission/results_connector.py,sha256=3J_nfleKOrrSbOGyxDYVxs4qWG1dFWY-qnJBR8jwhZY,15539
-stix_shifter_modules/aws_athena/stix_transmission/status_connector.py,sha256=G-JPjia6t91hGEtvAgImHpoGdO2DNI9ERZB4AAzqf7s,3175
-stix_shifter_modules_aws_athena-7.0.4.dist-info/LICENSE.md,sha256=ssGEKMVW69oFTBblVhD1YPolqCOyOCJi4wRDRI7xCnU,12786
-stix_shifter_modules_aws_athena-7.0.4.dist-info/METADATA,sha256=OBC0HWh6s5vKQMCnrvbIaJQl4v4FyWJV7H0rVlTGcLo,7175
-stix_shifter_modules_aws_athena-7.0.4.dist-info/NOTICE,sha256=wx-gWE9vSnLJ7YQkrGlMp9VNXOXG57TTxDDRd9CEdYg,1418
-stix_shifter_modules_aws_athena-7.0.4.dist-info/WHEEL,sha256=DZajD4pwLWue70CAfc7YaxT1wLUciNBvN_TTcvXpltE,110
-stix_shifter_modules_aws_athena-7.0.4.dist-info/top_level.txt,sha256=NX-VgUOr8fI-lMXHt3gtjfsEn1UPaGAVszt6Z_CTp2s,21
-stix_shifter_modules_aws_athena-7.0.4.dist-info/RECORD,,
+stix_shifter_modules/aws_athena/stix_transmission/status_connector.py,sha256=cRsTNP300ggHy5d3wFr3LNP3MWr2vCO3rLr-5ZJ9zUM,3473
+stix_shifter_modules_aws_athena-7.0.6.dist-info/LICENSE.md,sha256=ssGEKMVW69oFTBblVhD1YPolqCOyOCJi4wRDRI7xCnU,12786
+stix_shifter_modules_aws_athena-7.0.6.dist-info/METADATA,sha256=3r-0NLv7nbAkRgYHC8Rs3zzxBI1sZJvdcal2f2zPlxg,7175
+stix_shifter_modules_aws_athena-7.0.6.dist-info/NOTICE,sha256=wx-gWE9vSnLJ7YQkrGlMp9VNXOXG57TTxDDRd9CEdYg,1418
+stix_shifter_modules_aws_athena-7.0.6.dist-info/WHEEL,sha256=DZajD4pwLWue70CAfc7YaxT1wLUciNBvN_TTcvXpltE,110
+stix_shifter_modules_aws_athena-7.0.6.dist-info/top_level.txt,sha256=NX-VgUOr8fI-lMXHt3gtjfsEn1UPaGAVszt6Z_CTp2s,21
+stix_shifter_modules_aws_athena-7.0.6.dist-info/RECORD,,
```

