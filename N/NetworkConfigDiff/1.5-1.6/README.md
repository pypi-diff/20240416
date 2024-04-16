# Comparing `tmp/networkconfigdiff-1.5.tar.gz` & `tmp/networkconfigdiff-1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "networkconfigdiff-1.5.tar", last modified: Mon Apr 15 07:40:53 2024, max compression
+gzip compressed data, was "networkconfigdiff-1.6.tar", last modified: Tue Apr 16 09:33:03 2024, max compression
```

## Comparing `networkconfigdiff-1.5.tar` & `networkconfigdiff-1.6.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 07:40:53.315700 networkconfigdiff-1.5/
-drwxrwxrwx   0        0        0        0 2024-04-15 07:40:53.207287 networkconfigdiff-1.5/NetworkConfigDiff/
--rw-rw-rw-   0        0        0       35 2024-04-15 07:00:06.000000 networkconfigdiff-1.5/NetworkConfigDiff/__init__.py
--rw-rw-rw-   0        0        0     7221 2024-04-15 07:37:24.000000 networkconfigdiff-1.5/NetworkConfigDiff/network_config_diff.py
--rw-rw-rw-   0        0        0       74 2024-04-15 07:37:27.000000 networkconfigdiff-1.5/NetworkConfigDiff/test1.py
-drwxrwxrwx   0        0        0        0 2024-04-15 07:40:53.296556 networkconfigdiff-1.5/NetworkConfigDiff.egg-info/
--rw-rw-rw-   0        0        0      126 2024-04-15 07:40:52.000000 networkconfigdiff-1.5/NetworkConfigDiff.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      270 2024-04-15 07:40:52.000000 networkconfigdiff-1.5/NetworkConfigDiff.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 07:40:52.000000 networkconfigdiff-1.5/NetworkConfigDiff.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2024-04-15 07:40:52.000000 networkconfigdiff-1.5/NetworkConfigDiff.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      126 2024-04-15 07:40:53.306105 networkconfigdiff-1.5/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-15 07:40:53.316700 networkconfigdiff-1.5/setup.cfg
--rw-rw-rw-   0        0        0      224 2024-04-15 07:37:34.000000 networkconfigdiff-1.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-16 09:33:03.074049 networkconfigdiff-1.6/
+drwxrwxrwx   0        0        0        0 2024-04-16 09:33:02.935938 networkconfigdiff-1.6/NetworkConfigDiff/
+-rw-rw-rw-   0        0        0       35 2024-04-15 07:00:06.000000 networkconfigdiff-1.6/NetworkConfigDiff/__init__.py
+-rw-rw-rw-   0        0        0     5676 2024-04-16 09:31:58.000000 networkconfigdiff-1.6/NetworkConfigDiff/network_config_diff.py
+-rw-rw-rw-   0        0        0       74 2024-04-15 07:45:32.000000 networkconfigdiff-1.6/NetworkConfigDiff/test1.py
+drwxrwxrwx   0        0        0        0 2024-04-16 09:33:03.052146 networkconfigdiff-1.6/NetworkConfigDiff.egg-info/
+-rw-rw-rw-   0        0        0      126 2024-04-16 09:33:02.000000 networkconfigdiff-1.6/NetworkConfigDiff.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      280 2024-04-16 09:33:02.000000 networkconfigdiff-1.6/NetworkConfigDiff.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-16 09:33:02.000000 networkconfigdiff-1.6/NetworkConfigDiff.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2024-04-16 09:33:02.000000 networkconfigdiff-1.6/NetworkConfigDiff.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      126 2024-04-16 09:33:03.063461 networkconfigdiff-1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     4267 2024-04-16 09:25:41.000000 networkconfigdiff-1.6/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-16 09:33:03.075231 networkconfigdiff-1.6/setup.cfg
+-rw-rw-rw-   0        0        0      251 2024-04-16 09:32:14.000000 networkconfigdiff-1.6/setup.py
```

### Comparing `networkconfigdiff-1.5/NetworkConfigDiff/network_config_diff.py` & `networkconfigdiff-1.6/NetworkConfigDiff/network_config_diff.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import difflib
-import json
 
 class ConfigDiff(object):
 
     def __init__(self, old_config, new_config):
         self.old_config = old_config
         self.new_config = new_config
 
@@ -13,62 +12,43 @@
         return level
 
     def get_true_before(self,text,target_line_number,level,fromdata_data):
         '''
         返回：{'bgp 65139': {}},{'global': {}}
         '''
         config_line = text
-        # print(len(config_line))
         line = config_line[target_line_number-1].rstrip('\n')
-        # print(line,target_line_number)
         conf_for_nowstrip = line.lstrip(' ')
         curr_level = self._get_level(line)
-        # print(conf_for_nowstrip)
-        # print(len(line), len(conf_for_nowstrip))
         
         if curr_level < level:
-            flag = ''
             if len(line) == len(conf_for_nowstrip):
                 result = {}
-                # print(conf_for_nowstrip + '123', type(conf_for_nowstrip))
-                if conf_for_nowstrip == '#':
+                if conf_for_nowstrip == '#' or conf_for_nowstrip == '!':
                     result[fromdata_data] = {}
-                    flag = '#'
-                elif conf_for_nowstrip == '!':
-                    # if not result.get('global'):
-                    #     result['global'] = {}
-                    flag = '!'
                     result[fromdata_data] = {}
                 else:
                     result[conf_for_nowstrip] = {}
                     result[conf_for_nowstrip][fromdata_data] = {}
-                # print('result值{}'.format(result))
-                return result,flag
+                return result
             else:
                 # 三层，二层
-                result,flag = self.get_true_before(text,target_line_number-1,curr_level,fromdata_data) # 
-                # return {conf_for_nowstrip:result}
+                result = self.get_true_before(text,target_line_number-1,curr_level,fromdata_data) # 
                 key = list(result.keys())[0]
                 value = list(result[key].keys())[0]
-                # print('key是{},result是{},{},{}'.format(key,result,conf_for_nowstrip,value))
                 result[key][line] = {}
                 result[key][line][value] = {}
                 del result[key][value]
-                # print(result)
-                return result,flag
-        elif curr_level == level:
+                return result
+        elif curr_level >= level:
             for i in range(1, target_line_number):
                 target_level = self._get_level(config_line[target_line_number-i])
-                # print(config_line[target_line_number-i])
-                # print(target_level)
-                # print(level)
-                if target_level == level:
+                if target_level >= level:
                     continue
                 else:
-                    # print(i)
                     return self.get_true_before(text,target_line_number+1-i,level,fromdata_data) # {'bgp 65139': {}}
 
     def _merge_dicts(self,*dicts):
         """
         合并多个字典，其中每个字典可能包含多个嵌套级别的子字典
         """
         result = {}
@@ -78,58 +58,42 @@
                     if isinstance(value, dict):
                         result[key] = self._merge_dicts(result.get(key, {}), value)
                     else:
                         result[key] = value
         return result
 
     def collect_lines(self,diffs):
-        # 生成数组 {{'global':{'aa':{},'bb':{}}},{'bgp':{'cc':{},'dd':{}}}}
         from_all_info = {}
         to_all_info = {}
         for fromdata,todata,flag in diffs:
             if flag:
-                # print(fromdata,todata,flag)
                 fromdata_num,fromdata_data = fromdata
                 fromdata_data = fromdata_data.replace('\0+', '')
                 fromdata_data = fromdata_data.replace('\0-', '')
                 fromdata_data = fromdata_data.replace('\0^', '')
-                # print(fromdata_data, type(fromdata_data))
-                # fromdata_data = move_flag_to_behind(fromdata_data)
                 fromdata_data = fromdata_data.replace('\1', '')
-                # fromdata_data = fromdata_data.replace('\x00', '')
-                # print('1fromdata_data{}'.format(fromdata_data))
                 level = self._get_level(fromdata_data)
-                # print('level为{}'.format(level))
                 if fromdata_data != '\n' and fromdata_num!='':
-                    # print('1fromdata_data{}'.format(fromdata_data))
                     if level == 0:
-                        # if not from_all_info.get('global'):
-                        #     from_all_info['global'] = {}
                         from_all_info[fromdata_data] = {}
                     else:
-                        output,self.flag = self.get_true_before(text_b,fromdata_num-1,level, fromdata_data)
-                        print(output)
+                        output = self.get_true_before(self.old_config,fromdata_num-1,level, fromdata_data)
                         from_all_info  = self._merge_dicts(from_all_info,output)
                 
                 todata_num,todata_data = todata
                 todata_data = todata_data.replace('\0+', '')
                 todata_data = todata_data.replace('\0-', '')
                 todata_data = todata_data.replace('\0^', '')
-                # todata_data = move_flag_to_behind(todata_data)
                 todata_data = todata_data.replace('\1', '')
-                # print('1{}'.format(todata_data))
                 level = self._get_level(todata_data)
-                # print('level为{}'.format(level))
                 if todata_data != '\n' and todata_num != '':
                     if level == 0:
-                        # if not to_all_info.get('global'):
-                        #     to_all_info['global'] = {}
                         to_all_info[todata_data] = {}
                     else:
-                        output,self.flag = self.get_true_before(text_a,todata_num-1,level, todata_data)
+                        output = self.get_true_before(self.new_config,todata_num-1,level, todata_data)
                         # print(output)
                         to_all_info  = self._merge_dicts(to_all_info,output)
         return from_all_info, to_all_info
 
     def dict_to_conf(self,dictionary):
         keys = []
 
@@ -138,25 +102,30 @@
                 keys.append(key)
                 if isinstance(value, dict):
                     recursive_keys(value)
 
         recursive_keys(dictionary)
         return '\n'.join(keys)
 
-    def main(self):
+    def get_content_dict_and_diff(self):
         diffs = difflib._mdiff(self.old_config, self.new_config)
-        # print(diffs)
         from_all_info, to_all_info = self.collect_lines(diffs)
-        print('from_all_info{}'.format(json.dumps(from_all_info,indent=2)))
         change_old_config = self.dict_to_conf(from_all_info)
-        print('to_all_info{}'.format(json.dumps(to_all_info,indent=2)))
         change_new_config = self.dict_to_conf(to_all_info)
-        print(change_new_config)
-        print(change_old_config)
         change_new_lines = change_new_config.splitlines()
         change_old_lines = change_old_config.splitlines()
         # # 全量文字版对比
         d = difflib.Differ()
-        diff = d.compare(change_new_lines, change_old_lines)
+        diff = d.compare(change_old_lines, change_new_lines)
         differ = '\n'.join(list(diff))
-        print(differ)
-        return differ, from_all_info, to_all_info
+        # print(differ)
+        return differ, change_old_config, change_new_config, from_all_info, to_all_info
+
+if __name__ == '__main__':
+    text_a = open('./diff_text/192.16.102.21.txt', 'r', encoding='utf8').read().splitlines()
+    text_b = open('./diff_text/change_192.16.102.21.txt', 'r', encoding='utf8').read().splitlines()
+    differ, change_old_config, change_new_config, from_all_info, to_all_info = ConfigDiff(text_b, text_a).get_content_dict_and_diff()
+    print(differ)
+    print(change_old_config)
+    print(change_new_config)
+    print(from_all_info)
+    print(to_all_info)
```

