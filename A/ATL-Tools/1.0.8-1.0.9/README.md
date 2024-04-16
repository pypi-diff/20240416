# Comparing `tmp/atl_tools-1.0.8.tar.gz` & `tmp/atl_tools-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atl_tools-1.0.8.tar", last modified: Mon Apr 15 16:42:22 2024, max compression
+gzip compressed data, was "atl_tools-1.0.9.tar", last modified: Tue Apr 16 10:43:59 2024, max compression
```

## Comparing `atl_tools-1.0.8.tar` & `atl_tools-1.0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 atl       (1002) atl       (1002)        0 2024-04-15 16:42:22.919560 atl_tools-1.0.8/
-drwxrwxr-x   0 atl       (1002) atl       (1002)        0 2024-04-15 16:42:22.915560 atl_tools-1.0.8/ATL_Tools/
--rwxrwxrwx   0 atl       (1002) atl       (1002)    24486 2024-04-15 16:41:55.000000 atl_tools-1.0.8/ATL_Tools/ATL_gdal.py
--rwxrwxrwx   0 atl       (1002) atl       (1002)     4851 2024-04-09 08:36:48.000000 atl_tools-1.0.8/ATL_Tools/ATL_path.py
--rwxrwxrwx   0 atl       (1002) atl       (1002)     2009 2024-04-09 08:36:39.000000 atl_tools-1.0.8/ATL_Tools/__init__.py
-drwxrwxr-x   0 atl       (1002) atl       (1002)        0 2024-04-15 16:42:22.915560 atl_tools-1.0.8/ATL_Tools.egg-info/
--rw-r--r--   0 atl       (1002) atl       (1002)     1616 2024-04-15 16:42:22.000000 atl_tools-1.0.8/ATL_Tools.egg-info/PKG-INFO
--rw-rw-r--   0 atl       (1002) atl       (1002)      222 2024-04-15 16:42:22.000000 atl_tools-1.0.8/ATL_Tools.egg-info/SOURCES.txt
--rw-rw-r--   0 atl       (1002) atl       (1002)        1 2024-04-15 16:42:22.000000 atl_tools-1.0.8/ATL_Tools.egg-info/dependency_links.txt
--rw-rw-r--   0 atl       (1002) atl       (1002)       10 2024-04-15 16:42:22.000000 atl_tools-1.0.8/ATL_Tools.egg-info/top_level.txt
--rw-r--r--   0 atl       (1002) atl       (1002)     1616 2024-04-15 16:42:22.919560 atl_tools-1.0.8/PKG-INFO
--rwxrwxrwx   0 atl       (1002) atl       (1002)     1350 2024-04-15 16:42:04.000000 atl_tools-1.0.8/README.md
--rwxrwxrwx   0 atl       (1002) atl       (1002)      415 2024-04-15 16:42:16.000000 atl_tools-1.0.8/pyproject.toml
--rw-rw-r--   0 atl       (1002) atl       (1002)       38 2024-04-15 16:42:22.919560 atl_tools-1.0.8/setup.cfg
+drwxrwxr-x   0 atl       (1002) atl       (1002)        0 2024-04-16 10:43:59.389915 atl_tools-1.0.9/
+drwxrwxr-x   0 atl       (1002) atl       (1002)        0 2024-04-16 10:43:59.389915 atl_tools-1.0.9/ATL_Tools/
+-rwxrwxrwx   0 atl       (1002) atl       (1002)    26827 2024-04-16 10:24:52.000000 atl_tools-1.0.9/ATL_Tools/ATL_gdal.py
+-rwxrwxrwx   0 atl       (1002) atl       (1002)     4835 2024-04-16 10:15:29.000000 atl_tools-1.0.9/ATL_Tools/ATL_path.py
+-rwxrwxrwx   0 atl       (1002) atl       (1002)     2695 2024-04-16 10:42:24.000000 atl_tools-1.0.9/ATL_Tools/__init__.py
+drwxrwxr-x   0 atl       (1002) atl       (1002)        0 2024-04-16 10:43:59.389915 atl_tools-1.0.9/ATL_Tools.egg-info/
+-rw-r--r--   0 atl       (1002) atl       (1002)     4003 2024-04-16 10:43:59.000000 atl_tools-1.0.9/ATL_Tools.egg-info/PKG-INFO
+-rw-rw-r--   0 atl       (1002) atl       (1002)      222 2024-04-16 10:43:59.000000 atl_tools-1.0.9/ATL_Tools.egg-info/SOURCES.txt
+-rw-rw-r--   0 atl       (1002) atl       (1002)        1 2024-04-16 10:43:59.000000 atl_tools-1.0.9/ATL_Tools.egg-info/dependency_links.txt
+-rw-rw-r--   0 atl       (1002) atl       (1002)       10 2024-04-16 10:43:59.000000 atl_tools-1.0.9/ATL_Tools.egg-info/top_level.txt
+-rw-r--r--   0 atl       (1002) atl       (1002)     4003 2024-04-16 10:43:59.389915 atl_tools-1.0.9/PKG-INFO
+-rwxrwxrwx   0 atl       (1002) atl       (1002)     3704 2024-04-16 10:43:08.000000 atl_tools-1.0.9/README.md
+-rwxrwxrwx   0 atl       (1002) atl       (1002)      448 2024-04-16 10:25:29.000000 atl_tools-1.0.9/pyproject.toml
+-rw-rw-r--   0 atl       (1002) atl       (1002)       38 2024-04-16 10:43:59.389915 atl_tools-1.0.9/setup.cfg
```

### Comparing `atl_tools-1.0.8/ATL_Tools/ATL_gdal.py` & `atl_tools-1.0.9/ATL_Tools/ATL_gdal.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,30 +3,31 @@
 ATL_GDAL
 ---
 包含了使用`GDAL`对遥感图像进行处理的一些工具
 
 用法：
 ----
     >>> # 在开头复制这一句
-    >>> from ATL_Tools.ATL_gdal import (read_img_to_array_with_info, # ✔读取影像为数组并返回信息
-                               read_img_to_array,  # ✔读取影像为数组
-                               save_ds_to_tif,     # ✔将GDAL dataset数据格式写入tif保存
-                               save_array_to_tif,  # 将数组格式写入tif保存
-                               read_img_get_geo,   # ✔计算影像角点的地理坐标或投影坐标
-                               ds_get_img_geo,     # 读取dataset格式，计算影像角点的地理坐标或投影坐标
-                               pix_to_geo,         # 计算影像某一像素点的地理坐标或投影坐标
-                               geo_to_pix,         # 根据GDAL的仿射变换参数模型将给定的投影或地理坐标转为影像图上坐标（行列号）
-                               Mosaic_all_imgs,    # ✔将指定路径文件夹下的tif影像全部镶嵌到一张影像上
-                               Mosaic_2img_to_one, # 将两幅影像镶嵌至同一幅影像
-                               raster_overlap,     # 两个栅格数据集取重叠区或求交集（仅测试方形影像）
-                               crop_tif_with_json_zero, # ✔将带有坐标的图像按照json矢量进行裁切,无数据区域为0
-                               crop_tif_with_json_nan,  # ✔将带有坐标的图像按照json矢量进行裁切,无数据区域为nan
-                               Merge_multi_json,   # ✔将多个小的json合并为一个大的json,
-                               resample_image      # ✔使用GDAL对图像进行重采样
-                            )
+    >>> from ATL_Tools.ATL_gdal import (
+            read_img_to_array_with_info, # ✔读取影像为数组并返回信息
+            read_img_to_array,  # ✔读取影像为数组
+            save_ds_to_tif,     # ✔将GDAL dataset数据格式写入tif保存
+            save_array_to_tif,  # 将数组格式写入tif保存
+            read_img_get_geo,   # ✔计算影像角点的地理坐标或投影坐标
+            ds_get_img_geo,     # 读取dataset格式，计算影像角点的地理坐标或投影坐标
+            pix_to_geo,         # 计算影像某一像素点的地理坐标或投影坐标
+            geo_to_pix,         # 根据GDAL的仿射变换参数模型将给定的投影或地理坐标转为影像图上坐标（行列号）
+            Mosaic_all_imgs,    # ✔将指定路径文件夹下的tif影像全部镶嵌到一张影像上
+            Mosaic_2img_to_one, # 将两幅影像镶嵌至同一幅影像
+            raster_overlap,     # 两个栅格数据集取重叠区或求交集（仅测试方形影像）
+            crop_tif_with_json_zero, # ✔将带有坐标的图像按照json矢量进行裁切,无数据区域为0
+            crop_tif_with_json_nan,  # ✔将带有坐标的图像按照json矢量进行裁切,无数据区域为nan
+            Merge_multi_json,   # ✔将多个小的json合并为一个大的json,
+            resample_image      # ✔使用GDAL对图像进行重采样
+        )
                             
     ________________________________________________________________
     >>> # 示例1-读取影像为数组并返回信息
     >>> img = read_img_to_array_with_info(img_path) # 读取图片，并输出图片信息
     ________________________________________________________________
     >>> # 示例2-读取影像为数组
     >>> img = read_img_to_array(img_path) # 读取图片为数组
@@ -42,32 +43,36 @@
 import glob
 import numpy as np
 import math
 from typing import Dict, List, Optional, Sequence
 from .ATL_path import mkdir_or_exist, find_data_list
 from tqdm import tqdm 
 import json
+import cv2
 
 def read_img_to_array_with_info(filename: str, 
              convert_HWC: Optional[bool] = False) -> np.ndarray:   
     '''✔读取影像为数组并返回信息.
 
     Args:
         filename (str): 输入的影像路径
         convert_HWC (bool): 是否转换为 H*W*C 格式，默认为False 
 
     Returns: 
         影像的numpy数组格式，并显示影像的基本信息
+
     '''
+    DataTypeList = ['GDT_Byte','GDT_UInt16','GDT_Int16','GDT_UInt32',
+                    'GDT_Int32','GDT_Float32','GDT_Float64']
 
     dataset = gdal.Open(filename) #打开文件    
     print('栅格矩阵的行数:', dataset.RasterYSize)
     print('栅格矩阵的列数:', dataset.RasterXSize)
     print('波段数:', dataset.RasterCount)
-    print('数据类型:', dataset.GetRasterBand(1).DataType)
+    print('数据类型:', DataTypeList[dataset.GetRasterBand(1).DataType])
     print('仿射矩阵(左上角像素的大地坐标和像素分辨率)', dataset.GetGeoTransform())
     print('地图投影信息:', dataset.GetProjection())
     im_data = dataset.ReadAsArray()
     if convert_HWC:
         im_data = np.transpose(im_data, (1, 2, 0))
 
     del dataset 
@@ -130,15 +135,15 @@
     # del ds
     
 def save_array_to_tif(
         img_array: np.ndarray,
         out_path: str, 
         Transform = None, 
         Projection = None, 
-        Band: int = 1, 
+        Band: int=3, 
         Datatype: int = 6):
     """×将数组格式写入tif保存.
 
     Args:
         img_array (np.ndarry): 待保存的影像数组
         out_path (str): 输出的文件路径
         Transform：仿射矩阵六参数数组，默认为空,详细格式见GDAL。
@@ -149,26 +154,26 @@
     Returns: 
         输出影像文件
     """
 
     h,w,c= img_array.shape
     print(img_array.shape)
     driver = gdal.GetDriverByName("GTiff")
-    ds = driver.Create(out_path ,w, h, c, Datatype)
+    ds = driver.Create(out_path, w, h, c, Datatype)
     if not Transform==None:
         ds.SetGeoTransform(Transform) 
     if not Projection==None:
         ds.SetProjection(Projection)  
     if not Band == None:
         Band = c
 
     for band_num in range(Band):
         band = ds.GetRasterBand(band_num + 1)
         band.WriteArray(img_array[:, :, band_num]) 
-    # del ds
+    del ds
     
 def read_img_get_geo(img_path: str):
     '''计算影像角点的地理坐标或投影坐标
 
     Args:
         img_path (str): 影像路径
 
@@ -247,31 +252,43 @@
     a = np.array([[trans[1], trans[2]], [trans[4], trans[5]]])
     b = np.array([x - trans[0], y - trans[3]])
     
     return np.linalg.solve(a, b)
     
 def Mosaic_all_imgs(img_file_path: str,
                     output_path: str,
+                    add_alpha_chan: bool=False,
                     nan_or_zero: str='zero') -> None:
+    
     '''✔将指定路径文件夹下的tif影像全部镶嵌到一张影像上
         细节测试:
-        ✔镶嵌根据矢量裁切后的图像，无数据区域为nan
-        ✔镶嵌矩形的图像，无数据区域为nan
+        mosaic图像：
+        ✔ 镶嵌根据矢量裁切后的图像，无数据区域为nan
+        ✔ 镶嵌矩形的图像，无数据区域为nan
+        mosaic标签：
+        x 彩色标签是uint8的，不能用nan，只能用0
+
 
     注：将多个图合并之后，再进行裁切的话，nan就是白的，zero就是黑的
         如果单独裁切一个的话，不管nan还是zero都是白的
         如果将裁切后的进行合并的话，会把nan的部分也合并进去，需要单独处理
 
         需要进行优化
     
     Args:
         img_file_path (str)：tif 影像存放路径
         output_path (str): 输出镶嵌后 tif 的路径
+        add_alpha_chan (bool): 是否添加alpha通道，将无数据区域显示为空白，默认为False
         Nan_or_Zero (str): 'nan'或'zero'镶嵌后的无效数据nan或0,默认为0
                            'nan'更适合显示，'0更适合训练'
+        
+        例子: Mosaic_all_imgs(img_path_all, output_path, add_alpha_chan=True) # 对于RGB标签，添加alpha通道
+              Mosaic_all_imgs(img_path_all, output_path, Nan_or_Zero='zero') # 对于float32 img，mosaic为zero
+              Mosaic_all_imgs(img_path_all, output_path, Nan_or_Zero='zero') # 对于float32 img，mosaic为nan #展示用
+
     Returns: 
         镶嵌合成的整体影像
     '''
 
     # os.chdir(img_file_path) # 切换到指定路径
     #如果存在同名影像则先删除
     if os.path.exists(output_path):
@@ -360,24 +377,62 @@
             # 第三部：把两个图相加，得到最后的结果
             zero_mask_in_tiny_of_big = Tiny_in_BigOut_data!=0.
             in_ds_array[zero_mask_in_tiny_of_big] = 0.
             in_ds_array = Tiny_in_BigOut_data + in_ds_array
 
             # 写入大图
             big_out_band.WriteArray(in_ds_array, x, y)
-                        
-            # 最后把所有为0.的地方都变成nan
-            if nan_or_zero == 'nan':
-                big_out_band_nan = big_out_band.ReadAsArray()
-                big_out_band_nan = big_out_band_nan.astype(float) #合并RGB标签用
-                big_out_band_nan[big_out_band_nan==0] = np.nan
-                big_out_band.WriteArray(big_out_band_nan)
+    del in_ds, out_ds # 必须要有这个
+
+    if nan_or_zero=='zero' and add_alpha_chan==False:
+        print(f"  【ATL-LOG】空缺部分为'zero', 不添加alpha通道, 支持float32-img、uint8-label")
+        pass
+    # 最后把所有为0.的地方都变成nan
+    # 如果是float32图像的话,nan是可以work的,则会让无数据的地方变成nan,显示的时候就是透明的
+    elif nan_or_zero=='nan' and add_alpha_chan==False:
+        print(f"  【ATL-LOG】空缺部分为'nan', 不添加alpha通道,支持-float32img")
+        for band_num in range(bands):
+            out_band = out_ds.GetRasterBand(band_num + 1)
+            big_out_band_nan = out_band.ReadAsArray()
+            big_out_band_nan[big_out_band_nan==0.] = np.nan
+            out_band.WriteArray(big_out_band_nan)
+
+    # 如果创建的图像是uint8的话，nan是不行的，只能用0,添加alpha通道
+    elif add_alpha_chan==True:
+        print(f"  【ATL-LOG】添加alpha通道,支持uint8-rgb-img uint8-RGB-label")
+        output_img_ds = gdal.Open(output_path)
+        Transform = output_img_ds.GetGeoTransform()
+        Projection = output_img_ds.GetProjection()
+
+        output_img = output_img_ds.ReadAsArray()
+        output_img = np.transpose(output_img, (1, 2, 0))
+        h,w,c = output_img.shape
+
+        alpha_posi_array = np.zeros((h, w), dtype=np.uint8)
+        alpha_band_sum = np.zeros((h, w), dtype=np.uint16)
+        alpha_band_sum = output_img.sum(2)
+        
+        alpha_posi_array[alpha_band_sum==0]=0
+        alpha_posi_array[alpha_band_sum!=0]=255
+
+        alpha_image_array = cv2.merge((output_img, alpha_posi_array))
+        # 保存带有Alpha通道的图像
+        save_array_to_tif(img_array = alpha_image_array,
+                          out_path = output_path, # 覆盖图像
+                          Transform = Transform,
+                          Projection = Projection,
+                          Datatype = 1)
+
+    else:
+        print(f'--> 暂不支持此数据组合的合Mosaic')
+        print(f'--> 如数据为 float32, 请使用 nan_or_zero="nan"/"zero", add_alpha_chan=False')
+        print(f'--> 如数据为 uint8 RGB, 请使用 nan_or_zero="nan"/"zero", add_alpha_chan=True/False')
 
-    del in_ds, out_ds   
-    print(f'镶嵌图像已完成，输出至 {output_path}')
+      
+    print(f'-->镶嵌图像已完成，输出至 {output_path}')
      
 
 def Mosaic_2img_to_one(ds1 , ds2, path):
     '''将两幅影像镶嵌至同一幅影像
 
     Args:
         ds1：镶嵌数据集1
```

### Comparing `atl_tools-1.0.8/ATL_Tools/ATL_path.py` & `atl_tools-1.0.9/ATL_Tools/ATL_path.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,26 +102,24 @@
 
 
 def find_data_list(img_root_path: str, suffix: str ='.jpg') -> List:
     
     """根据给定的数据集根目录，找出其下所有符合后缀的数据集图片完整路径
 
     Args:
-
         img_root_path (str): 数据集根目录.
-        
-        suffix (str, optional): 后缀名. Defaults to '.jpg'.
+        suffix (str): 后缀名. Defaults to '.jpg'.
 
     Returns:
         List: 所有符合后缀的数据集图片完整路径(经过sorted()排序).
     """     
     print('--------------------------------------------------------------')
     print(f'-- 正在读取数据集列表... "{img_root_path}" ')
 
     img_list = []
     for img_name in scandir(img_root_path, suffix=suffix, recursive=True):
         if suffix in img_name:
             img_path = os.path.join(img_root_path, img_name)
             img_list.append(img_path)
-    print(f'-- 共在 "{img_root_path}" 下寻找到图片 {len(img_list)} 张')
+    print(f'-- 共在 "{img_root_path}" 下寻找到 *{suffix} {len(img_list)} 项')
     print('-------------------------------------------------------------')
     return sorted(img_list)
```

