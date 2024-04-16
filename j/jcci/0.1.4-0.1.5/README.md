# Comparing `tmp/jcci-0.1.4.tar.gz` & `tmp/jcci-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jcci-0.1.4.tar", last modified: Tue Apr  9 03:13:06 2024, max compression
+gzip compressed data, was "jcci-0.1.5.tar", last modified: Tue Apr 16 05:43:53 2024, max compression
```

## Comparing `jcci-0.1.4.tar` & `jcci-0.1.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 03:13:06.038018 jcci-0.1.4/
--rw-rw-rw-   0        0        0    11541 2024-04-03 09:49:05.000000 jcci-0.1.4/LICENSE
--rw-rw-rw-   0        0        0    15384 2024-04-09 03:13:06.036019 jcci-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     4554 2024-04-08 11:24:14.000000 jcci-0.1.4/README.md
--rw-rw-rw-   0        0        0     1592 2024-04-08 09:44:49.000000 jcci-0.1.4/README.pypi.md
--rw-rw-rw-   0        0        0      763 2024-04-09 02:56:01.000000 jcci-0.1.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-09 03:13:06.038018 jcci-0.1.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-09 03:13:05.991016 jcci-0.1.4/src/
-drwxrwxrwx   0        0        0        0 2024-04-09 03:13:06.021017 jcci-0.1.4/src/jcci/
--rw-rw-rw-   0        0        0       52 2024-04-09 02:53:42.000000 jcci-0.1.4/src/jcci/__init__.py
--rw-rw-rw-   0        0        0    43411 2024-04-09 03:12:36.000000 jcci-0.1.4/src/jcci/analyze.py
--rw-rw-rw-   0        0        0      249 2024-03-25 10:13:40.000000 jcci-0.1.4/src/jcci/config.py
--rw-rw-rw-   0        0        0      591 2024-03-25 09:09:49.000000 jcci-0.1.4/src/jcci/constant.py
--rw-rw-rw-   0        0        0     5344 2024-04-09 02:49:49.000000 jcci-0.1.4/src/jcci/database.py
--rw-rw-rw-   0        0        0     1985 2024-04-03 09:15:20.000000 jcci-0.1.4/src/jcci/diff_parse.py
--rw-rw-rw-   0        0        0     7933 2024-04-09 02:54:35.000000 jcci-0.1.4/src/jcci/graph.py
--rw-rw-rw-   0        0        0    38499 2024-04-09 02:49:49.000000 jcci-0.1.4/src/jcci/java_parse.py
--rw-rw-rw-   0        0        0     4371 2024-04-08 04:24:10.000000 jcci-0.1.4/src/jcci/mapper_parse.py
--rw-rw-rw-   0        0        0     2027 2024-03-25 09:09:49.000000 jcci-0.1.4/src/jcci/sql.py
-drwxrwxrwx   0        0        0        0 2024-04-09 03:13:06.034016 jcci-0.1.4/src/jcci.egg-info/
--rw-rw-rw-   0        0        0    15384 2024-04-09 03:13:05.000000 jcci-0.1.4/src/jcci.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      431 2024-04-09 03:13:05.000000 jcci-0.1.4/src/jcci.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 03:13:05.000000 jcci-0.1.4/src/jcci.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2024-04-09 03:13:05.000000 jcci-0.1.4/src/jcci.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-04-09 03:13:05.000000 jcci-0.1.4/src/jcci.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-09 03:13:06.032019 jcci-0.1.4/test/
--rw-rw-rw-   0        0        0        0 2024-04-08 06:40:37.000000 jcci-0.1.4/test/test_case.py
+drwxrwxrwx   0        0        0        0 2024-04-16 05:43:53.849041 jcci-0.1.5/
+-rw-rw-rw-   0        0        0    11541 2024-04-03 09:49:05.000000 jcci-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0    15384 2024-04-16 05:43:53.847043 jcci-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     4700 2024-04-10 09:22:17.000000 jcci-0.1.5/README.md
+-rw-rw-rw-   0        0        0     1592 2024-04-08 09:44:49.000000 jcci-0.1.5/README.pypi.md
+-rw-rw-rw-   0        0        0      763 2024-04-12 09:32:17.000000 jcci-0.1.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-16 05:43:53.849041 jcci-0.1.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-16 05:43:53.797042 jcci-0.1.5/src/
+drwxrwxrwx   0        0        0        0 2024-04-16 05:43:53.831040 jcci-0.1.5/src/jcci/
+-rw-rw-rw-   0        0        0        0 2024-04-09 03:17:36.000000 jcci-0.1.5/src/jcci/__init__.py
+-rw-rw-rw-   0        0        0    43941 2024-04-12 09:31:08.000000 jcci-0.1.5/src/jcci/analyze.py
+-rw-rw-rw-   0        0        0      249 2024-03-25 10:13:40.000000 jcci-0.1.5/src/jcci/config.py
+-rw-rw-rw-   0        0        0      702 2024-04-12 03:25:49.000000 jcci-0.1.5/src/jcci/constant.py
+-rw-rw-rw-   0        0        0     5344 2024-04-09 06:57:19.000000 jcci-0.1.5/src/jcci/database.py
+-rw-rw-rw-   0        0        0     1985 2024-04-03 09:15:20.000000 jcci-0.1.5/src/jcci/diff_parse.py
+-rw-rw-rw-   0        0        0     7933 2024-04-12 09:31:08.000000 jcci-0.1.5/src/jcci/graph.py
+-rw-rw-rw-   0        0        0    41979 2024-04-12 09:15:24.000000 jcci-0.1.5/src/jcci/java_parse.py
+-rw-rw-rw-   0        0        0     4516 2024-04-11 11:59:35.000000 jcci-0.1.5/src/jcci/mapper_parse.py
+-rw-rw-rw-   0        0        0     2027 2024-03-25 09:09:49.000000 jcci-0.1.5/src/jcci/sql.py
+drwxrwxrwx   0        0        0        0 2024-04-16 05:43:53.844041 jcci-0.1.5/src/jcci.egg-info/
+-rw-rw-rw-   0        0        0    15384 2024-04-16 05:43:53.000000 jcci-0.1.5/src/jcci.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      431 2024-04-16 05:43:53.000000 jcci-0.1.5/src/jcci.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-16 05:43:53.000000 jcci-0.1.5/src/jcci.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2024-04-16 05:43:53.000000 jcci-0.1.5/src/jcci.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-04-16 05:43:53.000000 jcci-0.1.5/src/jcci.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-16 05:43:53.842046 jcci-0.1.5/test/
+-rw-rw-rw-   0        0        0        0 2024-04-08 06:40:37.000000 jcci-0.1.5/test/test_case.py
```

### Comparing `jcci-0.1.4/LICENSE` & `jcci-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `jcci-0.1.4/PKG-INFO` & `jcci-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jcci
-Version: 0.1.4
+Version: 0.1.5
 Summary: Java code commit impact, java code change impact analysis, java代码改动影响范围分析工具
 Author-email: Oliver Li <441640312@qq.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `jcci-0.1.4/README.md` & `jcci-0.1.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -83,10 +83,14 @@
 ![请作者喝咖啡](./images/donation.png)
 
 #### 沟通交流
 扫码加微信，备注：JCCI微信群交流，或者扫码加入钉钉交流群
 
 ![微信交流群](./images/wechat.jpg) ![钉钉交流群](./images/jcci_dingding.jpg) 
 
+#### 鸣谢
+感谢一下同学请作者喝咖啡、提供意见或反馈Bug, 排名不分先后
+[zouchengli](https://github.com/zouchengli) 
+
 #### Star History
 
 [![Star History Chart](https://api.star-history.com/svg?repos=baikaishuipp/jcci&type=Date)](https://star-history.com/#baikaishuipp/jcci&Date)
```

### Comparing `jcci-0.1.4/README.pypi.md` & `jcci-0.1.5/README.pypi.md`

 * *Files identical despite different names*

### Comparing `jcci-0.1.4/pyproject.toml` & `jcci-0.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "jcci"
-version = "0.1.4"
+version = "0.1.5"
 authors = [
   { name="Oliver Li", email="441640312@qq.com" },
 ]
 description = "Java code commit impact, java code change impact analysis, java代码改动影响范围分析工具"
 readme = "README.pypi.md"
 license = { file="LICENSE" }
 requires-python = ">=3.9"
```

### Comparing `jcci-0.1.4/src/jcci/analyze.py` & `jcci-0.1.5/src/jcci/analyze.py`

 * *Files 2% similar despite different names*

```diff
@@ -188,19 +188,21 @@
     def _xml_diff_analyze(self, patch_filepath, diff_parse_obj: dict):
         xml_file_path_list = [filepath for filepath in self.xml_parse_results_new.keys() if filepath.endswith(patch_filepath)]
         if not xml_file_path_list:
             return
         xml_file_path = xml_file_path_list[0]
         xml_name = xml_file_path.split('/')[-1]
         xml_parse_result_new: mapper_parse.Mapper = self.xml_parse_results_new.get(xml_file_path)
-        methods = xml_parse_result_new.result_maps + xml_parse_result_new.sqls + xml_parse_result_new.statements
-        self._xml_method_diff_analyze(methods, diff_parse_obj['line_num_added'], diff_parse_obj['line_content_added'], xml_parse_result_new, xml_name, xml_file_path, self.commit_or_branch_new)
+        if xml_parse_result_new:
+            methods = xml_parse_result_new.result_maps + xml_parse_result_new.sqls + xml_parse_result_new.statements
+            self._xml_method_diff_analyze(methods, diff_parse_obj['line_num_added'], diff_parse_obj['line_content_added'], xml_parse_result_new, xml_name, xml_file_path, self.commit_or_branch_new)
         xml_parse_result_old = self.xml_parse_results_old.get(xml_file_path)
-        methods = xml_parse_result_old.result_maps + xml_parse_result_old.sqls + xml_parse_result_old.statements
-        self._xml_method_diff_analyze(methods, diff_parse_obj['line_num_removed'], diff_parse_obj['line_content_removed'], xml_parse_result_old, xml_name, xml_file_path, self.commit_or_branch_old)
+        if xml_parse_result_old:
+            methods = xml_parse_result_old.result_maps + xml_parse_result_old.sqls + xml_parse_result_old.statements
+            self._xml_method_diff_analyze(methods, diff_parse_obj['line_num_removed'], diff_parse_obj['line_content_removed'], xml_parse_result_old, xml_name, xml_file_path, self.commit_or_branch_old)
 
     # Step 4.1.1
     def _xml_method_diff_analyze(self, methods: list, line_num_list: list, line_content_list: list, xml_parse_result, xml_name, xml_file_path, commit_or_branch):
         namespace = xml_parse_result.namespace
         mapper_extend_dict = {
             'mapper_file_name': xml_name,
             'mapper_filepath': xml_file_path
@@ -376,15 +378,17 @@
 
     def _is_method_param_in_extends_package_class(self, method_param, extends_package_class, is_abstract, commit_or_branch):
         method_name: str = method_param.split('(')[0]
         extends_package = '.'.join(extends_package_class.split('.')[0: -1])
         extends_class_name = extends_package_class.split('.')[-1]
         extends_class_db = self.sqlite.select_data(f'SELECT * FROM class WHERE package_name = "{extends_package}" and class_name = "{extends_class_name}" and project_id = {self.project_id} and commit_or_branch = "{commit_or_branch}"')
         if not extends_class_db:
-            return None
+            extends_class_db = self.sqlite.select_data(f'SELECT * FROM class WHERE package_name = "{extends_package}" and class_name = "{extends_class_name}" and project_id = {self.project_id}')
+            if not extends_class_db:
+                return None
         extends_class_id = extends_class_db[0]['class_id']
         methods_db = self.sqlite.select_data(f'SELECT * FROM methods WHERE class_id = {extends_class_id} and method_name = "{method_name}" and is_abstract = "{is_abstract}"')
         if methods_db:
             return extends_package_class
         else:
             if extends_class_db[0]['extends_class']:
                 return self._is_method_param_in_extends_package_class(method_param, extends_class_db[0]['extends_class'], is_abstract, commit_or_branch)
@@ -459,14 +463,17 @@
             json_extract_sql_list = json_extract_sql_list[0: 995]
         sql = f'SELECT * FROM methods WHERE project_id = {self.project_id} AND (' + ' OR '.join(json_extract_sql_list) + ')'
         logging.info(f'{package_class} {method_param} invocation sql: {sql}')
         methods = self.sqlite.select_data(sql)
         class_ids = [str(method['class_id']) for method in methods]
         class_sql = f'SELECT * FROM class WHERE class_id in ({", ".join(class_ids)}) and commit_or_branch ="{commit_or_branch}"'
         class_db = self.sqlite.select_data(class_sql)
+        if not class_db:
+            class_sql = f'SELECT * FROM class WHERE class_id in ({", ".join(class_ids)})'
+            class_db = self.sqlite.select_data(class_sql)
         class_db_id = [class_item['class_id'] for class_item in class_db]
         return [method for method in methods if method['class_id'] in class_db_id]
 
     # Step 5.4.1
     def _gen_all_possible_method_param_list(self, method_param):
         method_param_list = []
         method_name = method_param.split('(')[0]
@@ -487,64 +494,60 @@
                 continue
             extends_package_class_list = self._get_extends_package_class(new_lst[i])
             for extends_package_class in extends_package_class_list:
                 result_item = [item for item in new_lst]
                 result_item[i] = extends_package_class
                 results.append(result_item)
 
-    def _is_duplicate_item(self, new_lst, lst):
-        is_duplicate = False
-        for item in lst:
-            if item == new_lst:
-                is_duplicate = True
-                break
-        return is_duplicate
-
     # Step 5.4.1.1
     def _replace_with_null_unknown(self, lst: list):
         need_replace_list = []
         replaced_list = []
-        results = []
+        results = set()
         self._replace_params_with_unknown(lst, results, 0, need_replace_list)
         for item in need_replace_list:
+            if len(results) > 1000:
+                break
             if item not in replaced_list:
                 replaced_list.append(item)
                 self._replace_params_with_unknown(item['list'], results, item['index'], need_replace_list)
-        return list(set(tuple(sub_list) for sub_list in results))
+        return list(results)
 
-    def _replace_params_with_unknown(self, lst: list, results: list, idx: int, need_replace_list: list):
+    def _replace_params_with_unknown(self, lst: list, results: set, idx: int, need_replace_list: list):
         # data = [item.split('<')[0].replace('<', '').replace('>', '') for item in data]
         for i in range(idx, len(lst)):
             new_lst = lst[:]
-            if not self._is_duplicate_item(new_lst, results):
-                results.append(new_lst)
+            results.add(tuple(new_lst))
             if new_lst[i].lower() not in constant.JAVA_BASIC_TYPE:
                 new_lst2 = new_lst[:]
                 if new_lst[i].startswith('List'):
                     new_lst2[i] = 'ArrayList'
                 elif new_lst[i].startswith('Map'):
                     new_lst2[i] = 'HashMap'
                 elif new_lst[i].startswith('Set'):
                     new_lst2[i] = 'HashSet'
-                if not self._is_duplicate_item(new_lst2, results):
-                    results.append(new_lst2)
-                    need_replace_list.append({'list': new_lst2, 'index': idx})
-            else:
-                if new_lst[i][0].isupper() and new_lst[i] != 'String':
-                    new_lst2 = new_lst[:]
-                    new_lst2[i] = new_lst[i][0].lower() + new_lst[i][1:]
-                    if not self._is_duplicate_item(new_lst2, results):
-                        results.append(new_lst2)
+                if tuple(new_lst2) not in results:
+                    results.add(tuple(new_lst2))
+                    if {'list': new_lst2, 'index': idx} not in need_replace_list:
                         need_replace_list.append({'list': new_lst2, 'index': idx})
+            # else:
+            #     if new_lst[i][0].isupper() and new_lst[i] != 'String':
+            #         new_lst2 = new_lst[:]
+            #         new_lst2[i] = new_lst[i][0].lower() + new_lst[i][1:]
+            #         if tuple(new_lst2) not in results:
+            #             results.add(tuple(new_lst2))
+            #             if {'list': new_lst2, 'index': idx} not in need_replace_list:
+            #                 need_replace_list.append({'list': new_lst2, 'index': idx})
             for el in ['null', 'unknown']:
                 new_lst_tmp = new_lst[:]
                 new_lst_tmp[i] = el
-                if not self._is_duplicate_item(new_lst_tmp, results):
-                    results.append(new_lst_tmp)
-                    need_replace_list.append({'list': new_lst_tmp, 'index': min(idx, len(new_lst) - 1)})
+                if tuple(new_lst_tmp) not in results:
+                    results.add(tuple(new_lst_tmp))
+                    if {'list': new_lst_tmp, 'index': min(idx, len(new_lst) - 1)} not in need_replace_list:
+                        need_replace_list.append({'list': new_lst_tmp, 'index': min(idx, len(new_lst) - 1)})
 
     # Step 5.5
     def _get_method_param_string(self, method_db: dict):
         method_name: str = method_db['method_name']
         params: list = json.loads(method_db['parameters'])
         params_type_list = [param['parameter_type'] for param in params]
         return f'{method_name}({",".join(params_type_list)})'
@@ -677,17 +680,17 @@
         package_class = package_class.replace("\\", "/")
         self.branch_name = branch
         self.commit_or_branch_new = commit_id
         self.commit_or_branch_new = self.commit_or_branch_new[0: 7] if len(self.commit_or_branch_new) > 7 else self.commit_or_branch_new
         self.project_name = self.git_url.split('/')[-1].split('.git')[0]
         self.file_path = os.path.join(config.project_path, self.project_name)
 
-        project_id = self.sqlite.add_project(self.project_name, self.git_url, self.branch_name, self.commit_or_branch_new, f'{package_class}.{method_nums}')
+        self.project_id = self.sqlite.add_project(self.project_name, self.git_url, self.branch_name, self.commit_or_branch_new, f'{package_class}.{method_nums}')
         class_name = package_class.split("/")[-1].replace('.java', '')
-        cci_path = f'{branch}_{commit_id}_{class_name}_{method_nums}.cci'
+        cci_path = f'{branch.replace("/", "#")}_{commit_id}_{class_name}_{method_nums}.cci'
         self.cci_filepath = os.path.join(self.file_path, cci_path)
         self._can_analyze(self.file_path, self.cci_filepath)
 
         # 无此项目, 先clone项目
         if not os.path.exists(self.file_path):
             logging.info(f'Cloning project: {self.git_url}')
             os.system(f'git clone -b {self.branch_name} {self.git_url} {self.file_path}')
@@ -698,15 +701,15 @@
         time.sleep(1)
 
         self.xml_parse_results_new, self.xml_parse_results_old = self._parse_project(self.file_path, self.commit_or_branch_new, None)
 
         if not method_nums:
             method_nums_all = []
             # todo
-            class_db = self.sqlite.select_data('SELECT * FROM class WHERE project_id = ' + str(project_id) + ' and filepath LIKE "%' + package_class + '"')
+            class_db = self.sqlite.select_data('SELECT * FROM class WHERE project_id = ' + str(self.project_id) + ' and filepath LIKE "%' + package_class + '"')
             if not class_db:
                 logging.error(f'Can not find {package_class} in db')
             class_id = class_db[0]['class_id']
             field_db = self.sqlite.select_data(f'SELECT * FROM field WHERE class_id = {class_id}')
             method_nums_all += [field['start_line'] for field in field_db]
             method_db = self.sqlite.select_data(f'SELECT * FROM methods WHERE class_id = {class_id}')
             method_nums_all += [method['start_line'] for method in method_db]
```

### Comparing `jcci-0.1.4/src/jcci/constant.py` & `jcci-0.1.5/src/jcci/constant.py`

 * *Files 16% similar despite different names*

```diff
@@ -18,7 +18,8 @@
 NODE_TYPE_MAPPER_RESULT_MAP = 'resultMap'
 NODE_TYPE_MAPPER_STATEMENT = 'statement'
 
 DIFF_TYPE_CHANGED = 'changed'
 DIFF_TYPE_IMPACTED = 'impacted'
 
 JAVA_BASIC_TYPE = ['string', 'int', 'boolean', 'long', 'byte', 'short', 'float', 'double', 'char']
+MAPPING_LIST = ['PostMapping', 'GetMapping', 'DeleteMapping', 'PutMapping', 'PatchMapping', 'RequestMapping']
```

### Comparing `jcci-0.1.4/src/jcci/database.py` & `jcci-0.1.5/src/jcci/database.py`

 * *Files identical despite different names*

### Comparing `jcci-0.1.4/src/jcci/diff_parse.py` & `jcci-0.1.5/src/jcci/diff_parse.py`

 * *Files identical despite different names*

### Comparing `jcci-0.1.4/src/jcci/graph.py` & `jcci-0.1.5/src/jcci/graph.py`

 * *Files identical despite different names*

### Comparing `jcci-0.1.4/src/jcci/java_parse.py` & `jcci-0.1.5/src/jcci/java_parse.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
+import os
 import logging
 import json
 import javalang
 from .database import SqliteHelper
-from .constant import ENTITY, RETURN_TYPE, PARAMETERS, BODY, METHODS, FIELDS, PARAMETER_TYPE_METHOD_INVOCATION_UNKNOWN, JAVA_BASIC_TYPE
+from .constant import ENTITY, RETURN_TYPE, PARAMETERS, BODY, METHODS, FIELDS, PARAMETER_TYPE_METHOD_INVOCATION_UNKNOWN, JAVA_BASIC_TYPE, MAPPING_LIST
 
 logging.basicConfig(format='%(asctime)s %(message)s', level=logging.DEBUG)
 
 class JavaParse(object):
     def __init__(self, db_path, project_id):
         self.project_id = project_id
         self.sqlite = SqliteHelper(db_path)
@@ -54,16 +55,16 @@
             package_path = package_class.replace('.', '/') + '.java'
             base_filepath = filepath.replace(package_path, '')
             for extends_package_class_item in extends_package_class_list:
                 extends_package = '.'.join(extends_package_class_item.split('.')[0: -1])
                 extends_class_name = extends_package_class_item.split('.')[-1]
                 extends_class_filepath = base_filepath + extends_package_class_item.replace('.', '/') + '.java'
                 extends_class_db = self.sqlite.select_data(f'SELECT * FROM class WHERE project_id={self.project_id} and package_name = "{extends_package}" and class_name = "{extends_class_name}" and filepath= "{extends_class_filepath}"')
-                # if not extends_class_db:
-                # self.parse_java_file(extends_class_filepath, commit_or_branch)
+                if not extends_class_db:
+                    self.parse_java_file(extends_class_filepath, commit_or_branch)
         implements = ','.join([implement.name for implement in node.implements]) if 'implements' in node.attrs and node.implements else None
         class_id, new_add = self.sqlite.add_class(filepath.replace('\\', '/'), access_modifier, class_type, class_name, package_name, extends_package_class, self.project_id, implements, annotations_json, documentation, is_controller, controller_base_url, commit_or_branch)
         return class_id, new_add
 
     def _parse_imports(self, imports):
         import_list = []
         for import_decl in imports:
@@ -107,15 +108,15 @@
                 'end_line': end_line
             }
             field_list.append(field_obj)
         self.sqlite.update_data(f'DELETE FROM field where class_id={class_id}')
         self.sqlite.insert_data('field', field_list)
         return field_list
 
-    def _parse_method(self, methods, lines, class_id, import_map, field_map):
+    def _parse_method(self, methods, lines, class_id, import_map, field_map, package_name, filepath):
         # 处理 methods
         all_method = []
         class_db = self.sqlite.select_data(f'SELECT * FROM class WHERE class_id = {class_id}')[0]
         base_url = class_db['controller_base_url'] if class_db['controller_base_url'] else ''
         method_name_entity_map = {method.name: method for method in methods}
         for method_obj in methods:
             method_invocation = {}
@@ -124,85 +125,99 @@
             documentation = method_obj.documentation  # document
             annotations = json.dumps(method_obj.annotations, default=lambda obj: obj.__dict__)  # annotations
             is_api, api_path = self._judge_is_api(method_obj.annotations, base_url, method_name)
             access_modifier = [m for m in list(method_obj.modifiers) if m.startswith('p')][0] if list([m for m in list(method_obj.modifiers) if m.startswith('p')]) else 'public'
             is_static = 'static' in list(method_obj.modifiers)
             is_abstract = 'abstract' in list(method_obj.modifiers)
             # 处理返回对象
-            return_type = self._deal_declarator_type(method_obj.return_type, import_map, method_invocation, RETURN_TYPE)
+            return_type = self._deal_declarator_type(method_obj.return_type, import_map, method_invocation, RETURN_TYPE, package_name, filepath)
             method_start_line = method_obj.position.line
             if method_obj.annotations:
                 method_start_line = method_obj.annotations[0].position.line
             method_end_line = self._get_method_end_line(method_obj)
             method_body = lines[method_start_line - 1: method_end_line + 1]
             # 处理参数
             parameters = []
             for parameter in method_obj.parameters:
                 parameter_obj = {
-                    'parameter_type': self._deal_declarator_type(parameter.type, import_map, method_invocation, PARAMETERS),
+                    'parameter_type': self._deal_declarator_type(parameter.type, import_map, method_invocation, PARAMETERS, package_name, filepath),
                     'parameter_name': parameter.name,
                     'parameter_varargs': parameter.varargs
                 }
                 parameters.append(parameter_obj)
             parameters_map = {parameter['parameter_name']: parameter['parameter_type'] for parameter in parameters}
 
             # 处理方法体
             if method_obj.body:
                 for body in method_obj.body:
                     for path, node in body.filter(javalang.tree.VariableDeclaration):
                         var_declarator = node.declarators[0].name
-                        var_declarator_type = self._deal_declarator_type(node.type, import_map, method_invocation, BODY)
+                        var_declarator_type = self._deal_declarator_type(node.type, import_map, method_invocation, BODY, package_name, filepath)
                         variable_map[var_declarator] = var_declarator_type
+                    for path, node in body.filter(javalang.tree.ClassCreator):
+                        qualifier = node.type.name
+                        qualifier_type = self._get_var_type(qualifier, parameters_map, variable_map, field_map, import_map, method_invocation, BODY, package_name, filepath)
+                        if node.selectors is None:
+                            self._add_entity_used_to_method_invocation(method_invocation, qualifier_type, BODY)
+                        else:
+                            for selector in node.selectors:
+                                if type(selector) != javalang.tree.MethodInvocation:
+                                    continue
+                                selector_member = selector.member
+                                selector_arguments = self._deal_var_type(selector.arguments, parameters_map, variable_map, field_map, import_map, method_invocation, BODY, package_name, filepath)
+                                selector_line = selector.position.line
+                                selector_method = f'{selector_member}({",".join(selector_arguments)})'
+                                self._add_method_used_to_method_invocation(method_invocation, qualifier_type, selector_method, [selector_line])
                     for path, node in body.filter(javalang.tree.MethodInvocation):
                         qualifier = node.qualifier
                         member = node.member
                         # 类静态方法调用
                         if not qualifier and not member[0].islower():
-                            qualifier_type = self._get_var_type(member, parameters_map, variable_map, field_map, import_map, method_invocation, BODY)
+                            qualifier_type = self._get_var_type(member, parameters_map, variable_map, field_map, import_map, method_invocation, BODY, package_name, filepath)
                             # todo a.b.c
                             if node.selectors is None:
                                 continue
                             for selector in node.selectors:
                                 selector_member = selector.member
-                                selector_arguments = self._deal_var_type(selector.arguments, parameters_map, variable_map, field_map, import_map, method_invocation, BODY)
+                                selector_arguments = self._deal_var_type(selector.arguments, parameters_map, variable_map, field_map, import_map, method_invocation, BODY, package_name, filepath)
                                 selector_line = selector.position.line
                                 selector_method = f'{selector_member}({",".join(selector_arguments)})'
                                 self._add_method_used_to_method_invocation(method_invocation, qualifier_type, selector_method, [selector_line])
                         elif qualifier:
-                            qualifier_type = self._get_var_type(qualifier, parameters_map, variable_map, field_map, import_map, method_invocation, BODY)
-                            node_arguments = self._deal_var_type(node.arguments, parameters_map, variable_map, field_map, import_map, method_invocation, BODY)
+                            qualifier_type = self._get_var_type(qualifier, parameters_map, variable_map, field_map, import_map, method_invocation, BODY, package_name, filepath)
+                            node_arguments = self._deal_var_type(node.arguments, parameters_map, variable_map, field_map, import_map, method_invocation, BODY, package_name, filepath)
                             node_line = node.position.line
                             node_method = f'{member}({",".join(node_arguments)})'
                             self._add_method_used_to_method_invocation(method_invocation, qualifier_type, node_method, [node_line])
                         # 在一个类的方法或父类方法
                         elif member:
                             class_db = self.sqlite.select_data(f'SELECT * FROM class where class_id={class_id} limit 1')[0]
                             package_class = class_db['package_name'] + '.' + class_db['class_name']
                             node_line = node.position.line
-                            node_arguments = self._deal_var_type(node.arguments, parameters_map, variable_map, field_map, import_map, method_invocation, BODY)
+                            node_arguments = self._deal_var_type(node.arguments, parameters_map, variable_map, field_map, import_map, method_invocation, BODY, package_name, filepath)
                             # todo 同级方法, 判断参数长度，不精确
                             if method_name_entity_map.get(member):
                                 same_class_method = None
                                 max_score = -float('inf')
                                 for method_item in methods:
                                     if method_item.name != member or len(node.arguments) != len(method_item.parameters):
                                         continue
-                                    method_item_param_types = [self._deal_declarator_type(parameter.type, import_map, method_invocation, PARAMETERS) for parameter in method_item.parameters]
+                                    method_item_param_types = [self._deal_declarator_type(parameter.type, import_map, method_invocation, PARAMETERS, package_name, filepath) for parameter in method_item.parameters]
                                     score = self._calculate_similar_score_method_params(node_arguments, method_item_param_types)
                                     if score > max_score:
                                         max_score = score
                                         same_class_method = method_item
                                 if same_class_method:
-                                    node_arguments = self._deal_var_type(same_class_method.parameters, parameters_map, variable_map, field_map, import_map, method_invocation, BODY)
+                                    node_arguments = self._deal_var_type(same_class_method.parameters, parameters_map, variable_map, field_map, import_map, method_invocation, BODY, package_name, filepath)
                                     node_method = f'{member}({",".join(node_arguments)})'
                                     self._add_method_used_to_method_invocation(method_invocation, package_class, node_method, [node_line])
                             # todo 继承方法
                             elif class_db['extends_class']:
                                 extends_package_class, method_params = self._find_method_in_extends(class_db['extends_class'], member, node_arguments)
-                                if not extends_package_class:
+                                if extends_package_class:
                                     self._add_method_used_to_method_invocation(method_invocation, extends_package_class, method_params, [node_line])
 
                     # for path, node in body.filter(javalang.tree.SuperMethodInvocation):
                     #     print(node)
                     # for path, node in body.filter(javalang.tree.TypeArgument):
                     #     print(node)
                     # for path, node in body.filter(javalang.tree.TypeParameter):
@@ -341,14 +356,16 @@
 
     def _get_api_part_route(self, part):
         part_class = type(part).__name__
         if part_class == 'MemberReference':
             return part.member.replace('"', '')
         elif part_class == 'Literal':
             return part.value.replace('"', '')
+        else:
+            return ''
 
     def _judge_is_controller(self, annotation_list):
         is_controller = any('Controller' in annotation.name for annotation in annotation_list)
         base_request = ''
         if not is_controller:
             return is_controller, base_request
         for annotation in annotation_list:
@@ -378,15 +395,15 @@
 
     def _judge_is_api(self, method_annotations, base_request, method_name):
         api_path_list = []
         req_method_list = []
         method_api_path = []
         is_api = False
         for method_annotation in method_annotations:
-            if 'Mapping' not in method_annotation.name:
+            if method_annotation.name not in MAPPING_LIST:
                 continue
             is_api = True
             if method_annotation.name != 'RequestMapping':
                 req_method_list.append(method_annotation.name.replace('Mapping', ''))
             else:
                 if not method_annotation.element:
                     continue
@@ -463,56 +480,72 @@
         elif FIELDS not in method_invocation[package_class].keys():
             method_invocation[package_class][FIELDS] = {field: lines}
         elif field not in method_invocation[package_class][FIELDS].keys():
             method_invocation[package_class][FIELDS][field] = lines
         else:
             method_invocation[package_class][FIELDS][field] += lines
 
-    def _deal_declarator_type(self, node_type, import_map, method_invocation, section):
+    def _deal_declarator_type(self, node_type, import_map, method_invocation, section, package_name, filepath):
         if node_type is None:
             return node_type
         if type(node_type) == javalang.tree.BasicType:
-            return node_type.name
+            node_name = node_type.name
+            node_name = node_name[0].upper() + node_name[1:]
+            return node_name
         var_declarator_type = node_type.name
         if var_declarator_type in import_map.keys():
             var_declarator_type = import_map.get(var_declarator_type)
             self._add_entity_used_to_method_invocation(method_invocation, var_declarator_type, section)
-        var_declarator_type_arguments = self._deal_arguments_type(node_type.arguments, import_map, method_invocation, section)
+        else:
+            node_path = "/".join(filepath.split("/")[0: -1]) + "/" + var_declarator_type + ".java"
+            if os.path.exists(node_path):
+                var_declarator_type = f'{package_name}.{var_declarator_type}'
+            else:
+                var_declarator_type = var_declarator_type[0].upper() + var_declarator_type[1:]
+        var_declarator_type_arguments = self._deal_arguments_type(node_type.arguments, import_map, method_invocation, section, package_name, filepath)
         if var_declarator_type_arguments:
             var_declarator_type = var_declarator_type + '<' + '#'.join(var_declarator_type_arguments) + '>'
         return var_declarator_type
 
-    def _deal_arguments_type(self, arguments, import_map, method_invocation, section):
+    def _deal_arguments_type(self, arguments, import_map, method_invocation, section, package_name, filepath):
         var_declarator_type_arguments_new = []
         if not arguments:
             return var_declarator_type_arguments_new
         var_declarator_type_arguments = []
         for argument in arguments:
             if type(argument) == javalang.tree.MethodInvocation:
                 var_declarator_type_arguments.append(PARAMETER_TYPE_METHOD_INVOCATION_UNKNOWN)
                 continue
             var_declarator_type_argument = self._deal_type(argument)
             if var_declarator_type_argument in import_map.keys():
                 var_declarator_type_argument = import_map.get(var_declarator_type_argument)
                 self._add_entity_used_to_method_invocation(method_invocation, var_declarator_type_argument, section)
+            else:
+                node_path = "/".join(filepath.split("/")[0: -1]) + "/" + var_declarator_type_argument + ".java"
+                if os.path.exists(node_path):
+                    var_declarator_type_argument = f'{package_name}.{var_declarator_type_argument}'
+                elif var_declarator_type_argument != PARAMETER_TYPE_METHOD_INVOCATION_UNKNOWN:
+                    var_declarator_type_argument = var_declarator_type_argument[0].upper() + var_declarator_type_argument[1:]
             var_declarator_type_arguments.append(var_declarator_type_argument)
         return var_declarator_type_arguments
 
     def _deal_type(self, argument):
         if not argument:
             return None
         argument_type = type(argument)
         if argument_type == javalang.tree.MemberReference:
             var_declarator_type_argument = argument.member
+        elif argument_type == javalang.tree.ClassCreator:
+            var_declarator_type_argument = argument.type.name
         elif argument_type == javalang.tree.Literal:
             var_declarator_type_argument = self._deal_literal_type(argument.value)
         elif argument_type == javalang.tree.This:
-            var_declarator_type_argument = 'This'
+            var_declarator_type_argument = PARAMETER_TYPE_METHOD_INVOCATION_UNKNOWN
         elif argument_type == javalang.tree.LambdaExpression:
-            var_declarator_type_argument = 'LambdaExpression'
+            var_declarator_type_argument = PARAMETER_TYPE_METHOD_INVOCATION_UNKNOWN
         elif argument_type == javalang.tree.BinaryOperation:
             # todo BinaryOperation temp set string
             var_declarator_type_argument = 'String'
         elif argument_type == javalang.tree.MethodReference or argument_type == javalang.tree.TernaryExpression:
             # todo MethodReference temp set unknown
             var_declarator_type_argument = PARAMETER_TYPE_METHOD_INVOCATION_UNKNOWN
         elif argument_type == javalang.tree.SuperMethodInvocation:
@@ -521,52 +554,55 @@
         elif argument_type == javalang.tree.Assignment:
             var_declarator_type_argument = self._deal_type(argument.value)
         elif argument_type == javalang.tree.Cast:
             var_declarator_type_argument = argument.type.name
         # todo
         elif argument_type == javalang.tree.SuperMemberReference:
             var_declarator_type_argument = 'String'
-        elif argument.type is not None:
+        elif 'type' in argument.attrs and argument.type is not None:
             var_declarator_type_argument = argument.type.name
         else:
             logging.info(f'argument type is None：{argument}')
             var_declarator_type_argument = PARAMETER_TYPE_METHOD_INVOCATION_UNKNOWN
         return var_declarator_type_argument
 
     def _deal_literal_type(self, text):
         if 'true' == text or 'false' == text:
-            return 'boolean'
+            return 'Boolean'
         if text.isdigit():
-            return 'int'
+            return 'Int'
         return 'String'
 
-    def _deal_var_type(self, arguments, parameters_map, variable_map, field_map, import_map, method_invocation, section):
+    def _deal_var_type(self, arguments, parameters_map, variable_map, field_map, import_map, method_invocation, section, package_name, filepath):
         var_declarator_type_arguments_new = []
         if not arguments:
             return var_declarator_type_arguments_new
         var_declarator_type_arguments = []
         for argument in arguments:
             argument_type = type(argument)
             if argument_type == javalang.tree.MethodInvocation:
                 var_declarator_type_arguments.append(PARAMETER_TYPE_METHOD_INVOCATION_UNKNOWN)
                 continue
+            elif argument_type == javalang.tree.MemberReference and argument.qualifier:
+                var_declarator_type_arguments.append(PARAMETER_TYPE_METHOD_INVOCATION_UNKNOWN)
+                continue
             var_declarator_type_argument = self._deal_type(argument)
-            var_declarator_type_argument = self._get_var_type(var_declarator_type_argument, parameters_map, variable_map, field_map, import_map, method_invocation, section)
-            type_arguments = self._deal_arguments_type(argument.type.arguments, import_map, method_invocation, section) \
+            var_declarator_type_argument = self._get_var_type(var_declarator_type_argument, parameters_map, variable_map, field_map, import_map, method_invocation, section, package_name, filepath)
+            type_arguments = self._deal_arguments_type(argument.type.arguments, import_map, method_invocation, section, package_name, filepath) \
                 if 'type' in argument.attrs \
                    and not isinstance(argument.type, str) \
                    and 'arguments' in argument.type.attrs \
                    and argument.type.arguments \
                 else []
             if type_arguments:
                 var_declarator_type_argument = var_declarator_type_argument + '<' + '#'.join(type_arguments) + '>'
             var_declarator_type_arguments.append(var_declarator_type_argument)
         return var_declarator_type_arguments
 
-    def _get_var_type(self, var, parameters_map, variable_map, field_map, import_map, method_invocation, section):
+    def _get_var_type(self, var, parameters_map, variable_map, field_map, import_map, method_invocation, section, package_name, filepath):
         if not var:
             return var
         if var in parameters_map.keys():
             return parameters_map.get(var)
         if var in variable_map.keys():
             return variable_map.get(var)
         if var in field_map.keys():
@@ -575,15 +611,22 @@
             start_line = field_map.get(var)['start_line']
             self._add_field_used_to_method_invocation(method_invocation, package_class, var, [start_line])
             return field_type
         if var in import_map.keys():
             var_type = import_map.get(var)
             self._add_entity_used_to_method_invocation(method_invocation, var_type, section)
             return var_type
-        return PARAMETER_TYPE_METHOD_INVOCATION_UNKNOWN
+        else:
+            var_path = "/".join(filepath.split("/")[0: -1]) + "/" + var + ".java"
+            if os.path.exists(var_path):
+                var_type = f'{package_name}.{var}'
+                return var_type
+            elif var != PARAMETER_TYPE_METHOD_INVOCATION_UNKNOWN:
+                var = var[0].upper() + var[1:]
+        return var
 
     def _get_extends_class_fields_map(self, class_id: int):
         class_db = self.sqlite.select_data(f'SELECT * FROM class WHERE class_id = {class_id}')[0]
         extend_package_class = class_db['extends_class']
         if not extend_package_class:
             return {}
         extend_package = '.'.join(extend_package_class.split('.')[0: -1])
@@ -600,15 +643,15 @@
         if not extend_class_entity['extends_class']:
             return extend_class_fields_map
         else:
             extend_new_map = self._get_extends_class_fields_map(extend_class_id)
             extend_new_map.update(extend_class_fields_map)
             return extend_new_map
 
-    def parse_java_file(self, filepath, commit_or_branch):
+    def parse_java_file(self, filepath: str, commit_or_branch: str):
         if not filepath.endswith('.java'):
             return
         try:
             with open(filepath, encoding='UTF-8') as fp:
                 file_content = fp.read()
         except:
             return
@@ -644,15 +687,15 @@
         field_map = {field_obj['field_name']: {'field_type': field_obj['field_type'], 'package_class': package_class, 'start_line': field_obj['start_line']} for field_obj in field_list}
         import_map = dict((k, v) for k, v in import_map.items() if v.startswith('com.') or v.startswith('cn.'))
 
         # 将extend class的field导进来
         extends_class_fields_map = self._get_extends_class_fields_map(class_id)
         extends_class_fields_map.update(field_map)
         # 处理 methods 信息
-        self._parse_method(tree.types[0].methods, lines, class_id, import_map, extends_class_fields_map)
+        self._parse_method(tree.types[0].methods, lines, class_id, import_map, extends_class_fields_map, package_name, filepath)
 
     def parse_java_file_list(self, filepath_list: list, commit_or_branch: str):
         for file_path in filepath_list:
             self.parse_java_file(file_path, commit_or_branch)
 
 
 if __name__ == '__main__':
```

### Comparing `jcci-0.1.4/src/jcci/mapper_parse.py` & `jcci-0.1.5/src/jcci/mapper_parse.py`

 * *Files 22% similar despite different names*

```diff
@@ -33,14 +33,20 @@
     match = re.search(pattern, string)
     if match:
         value = match.group(1)
         return value
     else:
         return None
 
+
+def check_string(tag, id_str, string):
+    pattern = r'^' + tag + '.*?id\s*=\s*"' + id_str + '"'
+    match = re.search(pattern, string)
+    return bool(match)
+
 def parse(filepath):
     # 读取XML文件内容
     try:
         with open(filepath, "r", encoding="utf-8") as file:
             xml_content = file.read()
     except:
         return None
@@ -63,29 +69,29 @@
 
     # 获取resultMap的id以及起始行号和截止行号
     for element in root.findall(".//resultMap"):
         result_map_id = element.attrib["id"]
         start_line = 0
         end_line = 0
         for i, line in enumerate(xml_content.splitlines(), start=1):
-            if line.strip().startswith('<resultMap') and f'id="{result_map_id}"' in line:
+            if check_string('<resultMap', result_map_id, line.strip()):
                 start_line = i
             if f'</resultMap>' in line and start_line != 0:
                 end_line = i
                 break
         content = xml_content.splitlines()[start_line - 1: end_line]
         result_map_info.append(MapperElement(result_map_id, 'resultMap', start_line, end_line, content))
 
     # 获取resultMap的id以及起始行号和截止行号
     for sql_element in root.findall(".//sql"):
         sql_id = sql_element.attrib["id"]
         start_line = 0
         end_line = 0
         for i, line in enumerate(xml_content.splitlines(), start=1):
-            if line.strip().startswith('<sql') and f'id="{sql_id}"' in line:
+            if check_string('<sql', sql_id, line.strip()):
                 start_line = i
             if f'</sql>' in line and start_line != 0:
                 end_line = i
                 break
         content = xml_content.splitlines()[start_line - 1: end_line]
         sql_info.append(MapperElement(sql_id, 'sql', start_line, end_line, content))
 
@@ -94,15 +100,15 @@
     for statement_element in statements:
         statement_id = statement_element.attrib["id"]
         start_line = 0
         end_line = 0
         result_map = None
         include_sql = None
         for i, line in enumerate(xml_content.splitlines(), start=1):
-            if f'<{statement_element.tag} id="{statement_id}"' in line:
+            if check_string('<' + statement_element.tag, statement_id, line.strip()):
                 start_line = i
             if f'resultMap="' in line and start_line != 0:
                 result_map = extract_value(line, 'resultMap')
             if line.strip().startswith('<include') and start_line != 0:
                 include_sql = extract_value(line, 'refid')
             if f'</{statement_element.tag}>' in line and start_line != 0:
                 end_line = i
```

### Comparing `jcci-0.1.4/src/jcci/sql.py` & `jcci-0.1.5/src/jcci/sql.py`

 * *Files identical despite different names*

### Comparing `jcci-0.1.4/src/jcci.egg-info/PKG-INFO` & `jcci-0.1.5/src/jcci.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jcci
-Version: 0.1.4
+Version: 0.1.5
 Summary: Java code commit impact, java code change impact analysis, java代码改动影响范围分析工具
 Author-email: Oliver Li <441640312@qq.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

