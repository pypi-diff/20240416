# Comparing `tmp/virgo_modules-0.0.78.tar.gz` & `tmp/virgo_modules-0.0.79.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "virgo_modules-0.0.78.tar", last modified: Wed Apr 10 16:57:04 2024, max compression
+gzip compressed data, was "virgo_modules-0.0.79.tar", last modified: Tue Apr 16 08:24:07 2024, max compression
```

## Comparing `virgo_modules-0.0.78.tar` & `virgo_modules-0.0.79.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-04-10 16:57:04.881308 virgo_modules-0.0.78/
--rw-rw-rw-   0        0        0     1097 2024-01-28 08:59:04.000000 virgo_modules-0.0.78/LICENSE
--rw-rw-rw-   0        0        0     1411 2024-04-10 16:57:04.875333 virgo_modules-0.0.78/PKG-INFO
--rw-rw-rw-   0        0        0      354 2024-01-28 09:03:10.000000 virgo_modules-0.0.78/README.md
--rw-rw-rw-   0        0        0       42 2024-04-10 16:57:04.882305 virgo_modules-0.0.78/setup.cfg
--rw-rw-rw-   0        0        0     1230 2024-04-10 16:49:15.000000 virgo_modules-0.0.78/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-10 16:57:04.672096 virgo_modules-0.0.78/virgo_app/
-drwxrwxrwx   0        0        0        0 2024-04-10 16:57:04.682094 virgo_modules-0.0.78/virgo_app/virgo_modules/
--rw-rw-rw-   0        0        0        0 2024-01-25 18:20:42.000000 virgo_modules-0.0.78/virgo_app/virgo_modules/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-10 16:57:04.867304 virgo_modules-0.0.78/virgo_app/virgo_modules/src/
--rw-rw-rw-   0        0        0        0 2024-01-25 17:59:03.000000 virgo_modules-0.0.78/virgo_app/virgo_modules/src/__init__.py
--rw-rw-rw-   0        0        0     2571 2024-04-05 07:01:35.000000 virgo_modules-0.0.78/virgo_app/virgo_modules/src/aws_utils.py
--rw-rw-rw-   0        0        0    13268 2024-04-05 06:56:27.000000 virgo_modules-0.0.78/virgo_app/virgo_modules/src/edge_utils.py
--rw-rw-rw-   0        0        0     1989 2023-12-10 12:51:06.000000 virgo_modules-0.0.78/virgo_app/virgo_modules/src/pull_artifacts.py
--rw-rw-rw-   0        0        0    67272 2024-04-10 16:56:38.000000 virgo_modules-0.0.78/virgo_app/virgo_modules/src/re_utils.py
--rw-rw-rw-   0        0        0   142729 2024-04-08 17:58:53.000000 virgo_modules-0.0.78/virgo_app/virgo_modules/src/ticketer_source.py
-drwxrwxrwx   0        0        0        0 2024-04-10 16:57:04.720096 virgo_modules-0.0.78/virgo_app/virgo_modules.egg-info/
--rw-rw-rw-   0        0        0     1411 2024-04-10 16:57:03.000000 virgo_modules-0.0.78/virgo_app/virgo_modules.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      552 2024-04-10 16:57:04.000000 virgo_modules-0.0.78/virgo_app/virgo_modules.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 16:57:03.000000 virgo_modules-0.0.78/virgo_app/virgo_modules.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      276 2024-04-10 16:57:03.000000 virgo_modules-0.0.78/virgo_app/virgo_modules.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-10 16:57:03.000000 virgo_modules-0.0.78/virgo_app/virgo_modules.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-16 08:24:07.740811 virgo_modules-0.0.79/
+-rw-rw-rw-   0        0        0     1097 2024-01-28 08:59:04.000000 virgo_modules-0.0.79/LICENSE
+-rw-rw-rw-   0        0        0     1411 2024-04-16 08:24:07.737817 virgo_modules-0.0.79/PKG-INFO
+-rw-rw-rw-   0        0        0      354 2024-01-28 09:03:10.000000 virgo_modules-0.0.79/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-16 08:24:07.741813 virgo_modules-0.0.79/setup.cfg
+-rw-rw-rw-   0        0        0     1230 2024-04-16 08:11:25.000000 virgo_modules-0.0.79/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-16 08:24:07.546290 virgo_modules-0.0.79/virgo_app/
+drwxrwxrwx   0        0        0        0 2024-04-16 08:24:07.604067 virgo_modules-0.0.79/virgo_app/virgo_modules/
+-rw-rw-rw-   0        0        0        0 2024-01-25 18:20:42.000000 virgo_modules-0.0.79/virgo_app/virgo_modules/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-16 08:24:07.728811 virgo_modules-0.0.79/virgo_app/virgo_modules/src/
+-rw-rw-rw-   0        0        0        0 2024-01-25 17:59:03.000000 virgo_modules-0.0.79/virgo_app/virgo_modules/src/__init__.py
+-rw-rw-rw-   0        0        0     2571 2024-04-05 07:01:35.000000 virgo_modules-0.0.79/virgo_app/virgo_modules/src/aws_utils.py
+-rw-rw-rw-   0        0        0    13268 2024-04-05 06:56:27.000000 virgo_modules-0.0.79/virgo_app/virgo_modules/src/edge_utils.py
+-rw-rw-rw-   0        0        0     1989 2023-12-10 12:51:06.000000 virgo_modules-0.0.79/virgo_app/virgo_modules/src/pull_artifacts.py
+-rw-rw-rw-   0        0        0    69517 2024-04-16 08:22:56.000000 virgo_modules-0.0.79/virgo_app/virgo_modules/src/re_utils.py
+-rw-rw-rw-   0        0        0   142729 2024-04-08 17:58:53.000000 virgo_modules-0.0.79/virgo_app/virgo_modules/src/ticketer_source.py
+drwxrwxrwx   0        0        0        0 2024-04-16 08:24:07.644800 virgo_modules-0.0.79/virgo_app/virgo_modules.egg-info/
+-rw-rw-rw-   0        0        0     1411 2024-04-16 08:24:04.000000 virgo_modules-0.0.79/virgo_app/virgo_modules.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      552 2024-04-16 08:24:04.000000 virgo_modules-0.0.79/virgo_app/virgo_modules.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-16 08:24:04.000000 virgo_modules-0.0.79/virgo_app/virgo_modules.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      276 2024-04-16 08:24:04.000000 virgo_modules-0.0.79/virgo_app/virgo_modules.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-16 08:24:04.000000 virgo_modules-0.0.79/virgo_app/virgo_modules.egg-info/top_level.txt
```

### Comparing `virgo_modules-0.0.78/LICENSE` & `virgo_modules-0.0.79/LICENSE`

 * *Files identical despite different names*

### Comparing `virgo_modules-0.0.78/PKG-INFO` & `virgo_modules-0.0.79/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: virgo_modules
-Version: 0.0.78
+Version: 0.0.79
 Summary: data processing and statistical modeling using stock market data
 Home-page: https://github.com/miguelmayhem92/virgo_module
 Author: Miguel Mayhuire
 Author-email: miguelmayhem92@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `virgo_modules-0.0.78/setup.py` & `virgo_modules-0.0.79/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("virgo_app/README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="virgo_modules",
-    version="0.0.78",
+    version="0.0.79",
     description="data processing and statistical modeling using stock market data",
     package_dir={"": "virgo_app"},
     packages=find_packages(where="virgo_app"),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/miguelmayhem92/virgo_module",
     author="Miguel Mayhuire",
```

### Comparing `virgo_modules-0.0.78/virgo_app/virgo_modules/src/aws_utils.py` & `virgo_modules-0.0.79/virgo_app/virgo_modules/src/aws_utils.py`

 * *Files identical despite different names*

### Comparing `virgo_modules-0.0.78/virgo_app/virgo_modules/src/edge_utils.py` & `virgo_modules-0.0.79/virgo_app/virgo_modules/src/edge_utils.py`

 * *Files identical despite different names*

### Comparing `virgo_modules-0.0.78/virgo_app/virgo_modules/src/pull_artifacts.py` & `virgo_modules-0.0.79/virgo_app/virgo_modules/src/pull_artifacts.py`

 * *Files identical despite different names*

### Comparing `virgo_modules-0.0.78/virgo_app/virgo_modules/src/re_utils.py` & `virgo_modules-0.0.79/virgo_app/virgo_modules/src/re_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -516,14 +516,61 @@
         fig.write_html(save_path+save_name+'.html')
         fig.write_json(save_path+save_name+'.json')
         
     if save_name and save_path and save_aws:
         # upload_file_to_aws(bucket = 'VIRGO_BUCKET', key = f'multi_dashboards/'+save_name+'.json',input_path = save_path+save_name+'.json')
         upload_file_to_aws(bucket = 'VIRGO_BUCKET', key = save_aws + save_name + '.json', input_path = save_path + save_name + '.json', aws_credentials = aws_credential)
         
+def produce_edges_dashboard(dataframe, ticket_list, save_name, show_plot = False, save_path = False, save_aws = False, aws_credentials = False):
+    '''
+    produce dashboard using signals and list of assets
+
+            Parameters:
+                    dataframe (pd.Dataframe): base data
+                    ticket_list (list): list of assets
+                    save_name (str): dashboad name resulting file
+                    show_plot (boolean): if true, display plot
+                    save_path (str): local path for saving e.g r'C:/path/to/the/file/'
+                    save_aws (str): remote key in s3 bucket path e.g. 'path/to/file/'
+                    aws_credential (dict): aws credentials
+
+            Returns:
+                    None
+    '''
+    n_assets = len(ticket_list)
+    
+    result_json_name = save_name
+    cols_length = 4
+    rows_length = math.ceil(n_assets/2) 
+    
+    subtitles = list()
+    for x in ticket_list:
+        subtitles.append(x)
+        subtitles.append(x + ' signal')
+    
+    fig = make_subplots(rows=rows_length, cols=cols_length,vertical_spacing = 0.01, horizontal_spacing = 0.03, shared_xaxes=True, subplot_titles = subtitles)
+    
+    for i,ticket in enumerate(ticket_list):
+        j = i%2*2 +1
+        i = i+1
+        i_r = math.ceil(i/2)
+    
+        show_legend = True if i == 1 else False
+    
+        df = dataframe[dataframe.asset == ticket]
+        fig.add_trace(go.Scatter(x=df['Date'], y=df['Close'],legendgroup="Close",showlegend = show_legend , mode='lines',name = 'Close', marker_color = 'blue'),col = j, row = i_r)
+        fig.add_trace(go.Scatter(x=df['Date'], y=df['proba_target_up'],legendgroup="proba",showlegend = show_legend , mode='lines',name = 'proba_target_up', marker_color = 'orange'),col = j+1, row = i_r)
+    fig.update_layout(height=rows_length*300, width=1500, title_text = f'dashboard top {n_assets} tickets')
+    
+    if save_path:
+        fig.write_json(save_path+result_json_name)
+    if show_plot:
+        fig.show()
+    if save_path and save_aws:
+        upload_file_to_aws(bucket = 'VIRGO_BUCKET', key = save_aws + result_json_name, input_path = save_path + result_json_name, aws_credentials = aws_credentials)
 
 def rank_by_return(data, lag_days, top_n = 5):
     '''
     produce ranking  by returns
 
             Parameters:
                     data (pd.Dataframe): base data
```

### Comparing `virgo_modules-0.0.78/virgo_app/virgo_modules/src/ticketer_source.py` & `virgo_modules-0.0.79/virgo_app/virgo_modules/src/ticketer_source.py`

 * *Files identical despite different names*

### Comparing `virgo_modules-0.0.78/virgo_app/virgo_modules.egg-info/PKG-INFO` & `virgo_modules-0.0.79/virgo_app/virgo_modules.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: virgo-modules
-Version: 0.0.78
+Version: 0.0.79
 Summary: data processing and statistical modeling using stock market data
 Home-page: https://github.com/miguelmayhem92/virgo_module
 Author: Miguel Mayhuire
 Author-email: miguelmayhem92@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `virgo_modules-0.0.78/virgo_app/virgo_modules.egg-info/SOURCES.txt` & `virgo_modules-0.0.79/virgo_app/virgo_modules.egg-info/SOURCES.txt`

 * *Files identical despite different names*

