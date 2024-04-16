# Comparing `tmp/atl_tools-1.0.9.tar.gz` & `tmp/atl_tools-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atl_tools-1.0.9.tar", last modified: Tue Apr 16 10:43:59 2024, max compression
+gzip compressed data, was "atl_tools-1.1.0.tar", last modified: Tue Apr 16 11:35:56 2024, max compression
```

## Comparing `atl_tools-1.0.9.tar` & `atl_tools-1.1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 atl       (1002) atl       (1002)        0 2024-04-16 10:43:59.389915 atl_tools-1.0.9/
-drwxrwxr-x   0 atl       (1002) atl       (1002)        0 2024-04-16 10:43:59.389915 atl_tools-1.0.9/ATL_Tools/
--rwxrwxrwx   0 atl       (1002) atl       (1002)    26827 2024-04-16 10:24:52.000000 atl_tools-1.0.9/ATL_Tools/ATL_gdal.py
--rwxrwxrwx   0 atl       (1002) atl       (1002)     4835 2024-04-16 10:15:29.000000 atl_tools-1.0.9/ATL_Tools/ATL_path.py
--rwxrwxrwx   0 atl       (1002) atl       (1002)     2695 2024-04-16 10:42:24.000000 atl_tools-1.0.9/ATL_Tools/__init__.py
-drwxrwxr-x   0 atl       (1002) atl       (1002)        0 2024-04-16 10:43:59.389915 atl_tools-1.0.9/ATL_Tools.egg-info/
--rw-r--r--   0 atl       (1002) atl       (1002)     4003 2024-04-16 10:43:59.000000 atl_tools-1.0.9/ATL_Tools.egg-info/PKG-INFO
--rw-rw-r--   0 atl       (1002) atl       (1002)      222 2024-04-16 10:43:59.000000 atl_tools-1.0.9/ATL_Tools.egg-info/SOURCES.txt
--rw-rw-r--   0 atl       (1002) atl       (1002)        1 2024-04-16 10:43:59.000000 atl_tools-1.0.9/ATL_Tools.egg-info/dependency_links.txt
--rw-rw-r--   0 atl       (1002) atl       (1002)       10 2024-04-16 10:43:59.000000 atl_tools-1.0.9/ATL_Tools.egg-info/top_level.txt
--rw-r--r--   0 atl       (1002) atl       (1002)     4003 2024-04-16 10:43:59.389915 atl_tools-1.0.9/PKG-INFO
--rwxrwxrwx   0 atl       (1002) atl       (1002)     3704 2024-04-16 10:43:08.000000 atl_tools-1.0.9/README.md
--rwxrwxrwx   0 atl       (1002) atl       (1002)      448 2024-04-16 10:25:29.000000 atl_tools-1.0.9/pyproject.toml
--rw-rw-r--   0 atl       (1002) atl       (1002)       38 2024-04-16 10:43:59.389915 atl_tools-1.0.9/setup.cfg
+drwxrwxr-x   0 atl       (1002) atl       (1002)        0 2024-04-16 11:35:56.626291 atl_tools-1.1.0/
+drwxrwxr-x   0 atl       (1002) atl       (1002)        0 2024-04-16 11:35:56.626291 atl_tools-1.1.0/ATL_Tools/
+-rw-rw-r--   0 atl       (1002) atl       (1002)    26827 2024-04-16 11:17:35.000000 atl_tools-1.1.0/ATL_Tools/ATL_gdal.py
+-rw-rw-r--   0 atl       (1002) atl       (1002)     4295 2024-04-16 11:35:05.000000 atl_tools-1.1.0/ATL_Tools/ATL_path.py
+-rw-rw-r--   0 atl       (1002) atl       (1002)     2695 2024-04-16 11:17:35.000000 atl_tools-1.1.0/ATL_Tools/__init__.py
+drwxrwxr-x   0 atl       (1002) atl       (1002)        0 2024-04-16 11:35:56.626291 atl_tools-1.1.0/ATL_Tools.egg-info/
+-rw-r--r--   0 atl       (1002) atl       (1002)     4262 2024-04-16 11:35:56.000000 atl_tools-1.1.0/ATL_Tools.egg-info/PKG-INFO
+-rw-rw-r--   0 atl       (1002) atl       (1002)      222 2024-04-16 11:35:56.000000 atl_tools-1.1.0/ATL_Tools.egg-info/SOURCES.txt
+-rw-rw-r--   0 atl       (1002) atl       (1002)        1 2024-04-16 11:35:56.000000 atl_tools-1.1.0/ATL_Tools.egg-info/dependency_links.txt
+-rw-rw-r--   0 atl       (1002) atl       (1002)       10 2024-04-16 11:35:56.000000 atl_tools-1.1.0/ATL_Tools.egg-info/top_level.txt
+-rw-r--r--   0 atl       (1002) atl       (1002)     4262 2024-04-16 11:35:56.626291 atl_tools-1.1.0/PKG-INFO
+-rw-rw-r--   0 atl       (1002) atl       (1002)     3963 2024-04-16 11:24:31.000000 atl_tools-1.1.0/README.md
+-rw-rw-r--   0 atl       (1002) atl       (1002)      448 2024-04-16 11:26:27.000000 atl_tools-1.1.0/pyproject.toml
+-rw-rw-r--   0 atl       (1002) atl       (1002)       38 2024-04-16 11:35:56.626291 atl_tools-1.1.0/setup.cfg
```

### Comparing `atl_tools-1.0.9/ATL_Tools/ATL_gdal.py` & `atl_tools-1.1.0/ATL_Tools/ATL_gdal.py`

 * *Files identical despite different names*

### Comparing `atl_tools-1.0.9/ATL_Tools/ATL_path.py` & `atl_tools-1.1.0/ATL_Tools/ATL_path.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,26 +10,17 @@
     >>> from ATL_path import mkdir_or_exist, find_data_list, scandir
     ________________________________________________________________
     >>> # 示例1-创建文件夹：
     >>> mkdir_or_exist(xxxx) # 创建文件夹, 存在则不创建
     ________________________________________________________________
     >>> # 示例2-寻找所有符合后缀文件夹名称(绝对路径):
     >>> # 寻找尾缀为'.jpg'的数据集列表
-    >>> find_data_list(img_root_path: str, suffix: str ='.jpg') 
-    ________________________________________________________________
-    >>> # 示例3-寻找所有符合后缀文件夹名称:
-    >>> for label_path in scandir(dataset_path, suffix='.png', recursive=True):
-    >>>     if 'labels' in label_path and 'labels_mask' not in label_path:
-    >>>         rgb_label_path = osp.join(dataset_path, label_path)
-    >>>         RGB_labels_path.append(rgb_label_path)
-    >>>         if 'v1.2' in label_path:
-    >>>             RGB_labels_v1_2_path.append(rgb_label_path)
-    >>>         elif 'v2.0' in label_path:
-    >>>             RGB_labels_v2_0_path.append(rgb_label_path)
-
+    >>> img_list = find_data_list(img_root_path: str, suffix: str ='.jpg') 
+        for img_path in tqdm(img_list):
+            print(img_path)
 """
 
 import os
 import os.path as osp
 from pathlib import Path
 from typing import List
```

### Comparing `atl_tools-1.0.9/ATL_Tools/__init__.py` & `atl_tools-1.1.0/ATL_Tools/__init__.py`

 * *Files identical despite different names*

### Comparing `atl_tools-1.0.9/ATL_Tools.egg-info/PKG-INFO` & `atl_tools-1.1.0/ATL_Tools.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: ATL_Tools
-Version: 1.0.9
+Version: 1.1.0
 Summary: AI-Tianlong的Tools打包，开箱即用, 包含ATL_path和ATL_gdal,可用于文件夹创建、文件搜索、遥感图像处理
 License: MIT License
 Keywords: ATL_Tools,GDAL,AI-Tianlong,Chinese
 Description-Content-Type: text/markdown
 
 # ATL_Tools 使用指南
-## 1. 简介
-ATL_Tools 是一个由[AI-Tianlong](https://github.com/AI-Tianlong)开发的工具集合，包含一些便利的小工具
-### 1. 文件夹/数据绝对路径搜索工具
+## 0. 简介
+ATL_Tools 是一个由 [AI-Tianlong【GitHub】](https://github.com/AI-Tianlong)开发的工具集合，包含一些便利的小工具。
+如果您有新的模块添加，或者对现有模块有改进意见，欢迎提交 PR 至  [ATL_Tools_pypi 【GitHub Repo】](https://github.com/AI-Tianlong/ATL_Tools_pypi).
+## 1. 文件夹/数据绝对路径搜索工具
 加载方式:
 
 ```python
 from ATL_Tools import mkdir_or_exist, find_data_list
 ```
 
-### 2. 遥感图像处理工具:
+## 2. 遥感图像处理工具:
 加载方式:
 ```python
 from ATL_Tools.ATL_gdal import (
     read_img_to_array_with_info, # ✔读取影像为数组并返回信息
     read_img_to_array,  # ✔读取影像为数组
     save_ds_to_tif,     # ✔将GDAL dataset数据格式写入tif保存
     save_array_to_tif,  # 将数组格式写入tif保存
@@ -33,31 +34,31 @@
     raster_overlap,     # 两个栅格数据集取重叠区或求交集（仅测试方形影像）
     crop_tif_with_json_zero, # ✔将带有坐标的图像按照json矢量进行裁切,无数据区域为0
     crop_tif_with_json_nan,  # ✔将带有坐标的图像按照json矢量进行裁切,无数据区域为nan
     Merge_multi_json,   # ✔将多个小的json合并为一个大的json,
     resample_image      # ✔使用GDAL对图像进行重采样
                         )
 ```
-## 2. 使用方法
+## 3. 使用方法
 
-### 2.1 ATL_path 文件夹工具
+### 3.1 ATL_path 文件夹工具
 
 使用程序示例:  
 1. 创建文件夹
     ```python
     from ATL_Tools import mkdir_or_exist, find_data_list
     #创建文件夹
     mkdir_or_exist('新文件夹名称')
     #获取文件夹内所有后缀为.jpg的文件绝对路径
     ```
 2. 获取文件夹内所有后缀为 `.jpg` 的文件绝对路径
     ```python
     img_lists = find_data_list(img_root_path='数据集文件夹路径', suffix ='.jpg')
     ```
-### 2.2 ATL_gdal 遥感图像处理工具
+### 3.2 ATL_gdal 遥感图像处理工具
 使用程序示例：
 1. 根据矢量批量裁切影像
     ```python
     from ATL_Tools import mkdir_or_exist, find_data_list
     from ATL_Tools.ATL_gdal import crop_tif_with_json_nan
     from tqdm import tqdm
     import os 
@@ -73,14 +74,15 @@
 
         img_output_path = os.path.join(output_path_all, os.path.basename(img_path))
         json_path = os.path.join(json_path_all, os.path.basename(img_path).split('_')[-1].replace('.tif', '.json'))
         print(f'正在裁切: {img_output_path},json: {json_path}')
         crop_tif_with_json_nan(img_path, img_output_path, json_path)
     ```
 
-## 3. 版本更新日志
+## 4. 版本更新日志
 - 2023-12-06 v1.0.2 修复README中显示问题。
 - 2023-12-06 v1.0.3 修改项目名称为ATL_Tools。
 - 2024-04-03 v1.0.6 增加ATL_gdal模块，用于处理遥感影像。
 - 2024-04-09 v1.0.7 修复ATL_gdal模块中对于ATL_path的引用，`__init__.py` 注释掉`from ATL_gdal import *`, 可不安装gdal使用ATL_Tools
 - 2024-04-16 v1.0.8 修复 `ValueError: cannot convert float NaN to integer` in ATL_gdal Line 371
 - 2024-04-16 v1.0.9 修复 修复`Mosaic_all_images()`对于mosaic RGB uint8标签的支持，优化`find_data_list()`函数显示，优化`_init_.py`, 优化`Readme.md`显示
+- 2024-04-16 v1.1.0 pypi页面增加`ATL_Tools`Github贡献地址。
```

### Comparing `atl_tools-1.0.9/PKG-INFO` & `atl_tools-1.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: ATL_Tools
-Version: 1.0.9
+Version: 1.1.0
 Summary: AI-Tianlong的Tools打包，开箱即用, 包含ATL_path和ATL_gdal,可用于文件夹创建、文件搜索、遥感图像处理
 License: MIT License
 Keywords: ATL_Tools,GDAL,AI-Tianlong,Chinese
 Description-Content-Type: text/markdown
 
 # ATL_Tools 使用指南
-## 1. 简介
-ATL_Tools 是一个由[AI-Tianlong](https://github.com/AI-Tianlong)开发的工具集合，包含一些便利的小工具
-### 1. 文件夹/数据绝对路径搜索工具
+## 0. 简介
+ATL_Tools 是一个由 [AI-Tianlong【GitHub】](https://github.com/AI-Tianlong)开发的工具集合，包含一些便利的小工具。
+如果您有新的模块添加，或者对现有模块有改进意见，欢迎提交 PR 至  [ATL_Tools_pypi 【GitHub Repo】](https://github.com/AI-Tianlong/ATL_Tools_pypi).
+## 1. 文件夹/数据绝对路径搜索工具
 加载方式:
 
 ```python
 from ATL_Tools import mkdir_or_exist, find_data_list
 ```
 
-### 2. 遥感图像处理工具:
+## 2. 遥感图像处理工具:
 加载方式:
 ```python
 from ATL_Tools.ATL_gdal import (
     read_img_to_array_with_info, # ✔读取影像为数组并返回信息
     read_img_to_array,  # ✔读取影像为数组
     save_ds_to_tif,     # ✔将GDAL dataset数据格式写入tif保存
     save_array_to_tif,  # 将数组格式写入tif保存
@@ -33,31 +34,31 @@
     raster_overlap,     # 两个栅格数据集取重叠区或求交集（仅测试方形影像）
     crop_tif_with_json_zero, # ✔将带有坐标的图像按照json矢量进行裁切,无数据区域为0
     crop_tif_with_json_nan,  # ✔将带有坐标的图像按照json矢量进行裁切,无数据区域为nan
     Merge_multi_json,   # ✔将多个小的json合并为一个大的json,
     resample_image      # ✔使用GDAL对图像进行重采样
                         )
 ```
-## 2. 使用方法
+## 3. 使用方法
 
-### 2.1 ATL_path 文件夹工具
+### 3.1 ATL_path 文件夹工具
 
 使用程序示例:  
 1. 创建文件夹
     ```python
     from ATL_Tools import mkdir_or_exist, find_data_list
     #创建文件夹
     mkdir_or_exist('新文件夹名称')
     #获取文件夹内所有后缀为.jpg的文件绝对路径
     ```
 2. 获取文件夹内所有后缀为 `.jpg` 的文件绝对路径
     ```python
     img_lists = find_data_list(img_root_path='数据集文件夹路径', suffix ='.jpg')
     ```
-### 2.2 ATL_gdal 遥感图像处理工具
+### 3.2 ATL_gdal 遥感图像处理工具
 使用程序示例：
 1. 根据矢量批量裁切影像
     ```python
     from ATL_Tools import mkdir_or_exist, find_data_list
     from ATL_Tools.ATL_gdal import crop_tif_with_json_nan
     from tqdm import tqdm
     import os 
@@ -73,14 +74,15 @@
 
         img_output_path = os.path.join(output_path_all, os.path.basename(img_path))
         json_path = os.path.join(json_path_all, os.path.basename(img_path).split('_')[-1].replace('.tif', '.json'))
         print(f'正在裁切: {img_output_path},json: {json_path}')
         crop_tif_with_json_nan(img_path, img_output_path, json_path)
     ```
 
-## 3. 版本更新日志
+## 4. 版本更新日志
 - 2023-12-06 v1.0.2 修复README中显示问题。
 - 2023-12-06 v1.0.3 修改项目名称为ATL_Tools。
 - 2024-04-03 v1.0.6 增加ATL_gdal模块，用于处理遥感影像。
 - 2024-04-09 v1.0.7 修复ATL_gdal模块中对于ATL_path的引用，`__init__.py` 注释掉`from ATL_gdal import *`, 可不安装gdal使用ATL_Tools
 - 2024-04-16 v1.0.8 修复 `ValueError: cannot convert float NaN to integer` in ATL_gdal Line 371
 - 2024-04-16 v1.0.9 修复 修复`Mosaic_all_images()`对于mosaic RGB uint8标签的支持，优化`find_data_list()`函数显示，优化`_init_.py`, 优化`Readme.md`显示
+- 2024-04-16 v1.1.0 pypi页面增加`ATL_Tools`Github贡献地址。
```

### Comparing `atl_tools-1.0.9/README.md` & `atl_tools-1.1.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 # ATL_Tools 使用指南
-## 1. 简介
-ATL_Tools 是一个由[AI-Tianlong](https://github.com/AI-Tianlong)开发的工具集合，包含一些便利的小工具
-### 1. 文件夹/数据绝对路径搜索工具
+## 0. 简介
+ATL_Tools 是一个由 [AI-Tianlong【GitHub】](https://github.com/AI-Tianlong)开发的工具集合，包含一些便利的小工具。
+如果您有新的模块添加，或者对现有模块有改进意见，欢迎提交 PR 至  [ATL_Tools_pypi 【GitHub Repo】](https://github.com/AI-Tianlong/ATL_Tools_pypi).
+## 1. 文件夹/数据绝对路径搜索工具
 加载方式:
 
 ```python
 from ATL_Tools import mkdir_or_exist, find_data_list
 ```
 
-### 2. 遥感图像处理工具:
+## 2. 遥感图像处理工具:
 加载方式:
 ```python
 from ATL_Tools.ATL_gdal import (
     read_img_to_array_with_info, # ✔读取影像为数组并返回信息
     read_img_to_array,  # ✔读取影像为数组
     save_ds_to_tif,     # ✔将GDAL dataset数据格式写入tif保存
     save_array_to_tif,  # 将数组格式写入tif保存
@@ -25,31 +26,31 @@
     raster_overlap,     # 两个栅格数据集取重叠区或求交集（仅测试方形影像）
     crop_tif_with_json_zero, # ✔将带有坐标的图像按照json矢量进行裁切,无数据区域为0
     crop_tif_with_json_nan,  # ✔将带有坐标的图像按照json矢量进行裁切,无数据区域为nan
     Merge_multi_json,   # ✔将多个小的json合并为一个大的json,
     resample_image      # ✔使用GDAL对图像进行重采样
                         )
 ```
-## 2. 使用方法
+## 3. 使用方法
 
-### 2.1 ATL_path 文件夹工具
+### 3.1 ATL_path 文件夹工具
 
 使用程序示例:  
 1. 创建文件夹
     ```python
     from ATL_Tools import mkdir_or_exist, find_data_list
     #创建文件夹
     mkdir_or_exist('新文件夹名称')
     #获取文件夹内所有后缀为.jpg的文件绝对路径
     ```
 2. 获取文件夹内所有后缀为 `.jpg` 的文件绝对路径
     ```python
     img_lists = find_data_list(img_root_path='数据集文件夹路径', suffix ='.jpg')
     ```
-### 2.2 ATL_gdal 遥感图像处理工具
+### 3.2 ATL_gdal 遥感图像处理工具
 使用程序示例：
 1. 根据矢量批量裁切影像
     ```python
     from ATL_Tools import mkdir_or_exist, find_data_list
     from ATL_Tools.ATL_gdal import crop_tif_with_json_nan
     from tqdm import tqdm
     import os 
@@ -65,14 +66,15 @@
 
         img_output_path = os.path.join(output_path_all, os.path.basename(img_path))
         json_path = os.path.join(json_path_all, os.path.basename(img_path).split('_')[-1].replace('.tif', '.json'))
         print(f'正在裁切: {img_output_path},json: {json_path}')
         crop_tif_with_json_nan(img_path, img_output_path, json_path)
     ```
 
-## 3. 版本更新日志
+## 4. 版本更新日志
 - 2023-12-06 v1.0.2 修复README中显示问题。
 - 2023-12-06 v1.0.3 修改项目名称为ATL_Tools。
 - 2024-04-03 v1.0.6 增加ATL_gdal模块，用于处理遥感影像。
 - 2024-04-09 v1.0.7 修复ATL_gdal模块中对于ATL_path的引用，`__init__.py` 注释掉`from ATL_gdal import *`, 可不安装gdal使用ATL_Tools
 - 2024-04-16 v1.0.8 修复 `ValueError: cannot convert float NaN to integer` in ATL_gdal Line 371
-- 2024-04-16 v1.0.9 修复 修复`Mosaic_all_images()`对于mosaic RGB uint8标签的支持，优化`find_data_list()`函数显示，优化`_init_.py`, 优化`Readme.md`显示
+- 2024-04-16 v1.0.9 修复 修复`Mosaic_all_images()`对于mosaic RGB uint8标签的支持，优化`find_data_list()`函数显示，优化`_init_.py`, 优化`Readme.md`显示
+- 2024-04-16 v1.1.0 pypi页面增加`ATL_Tools`Github贡献地址。
```

