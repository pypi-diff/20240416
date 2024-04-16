# Comparing `tmp/VASP2KP-1.1.2.tar.gz` & `tmp/VASP2KP-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "VASP2KP-1.1.2.tar", last modified: Mon Apr 15 02:34:27 2024, max compression
+gzip compressed data, was "VASP2KP-1.1.3.tar", last modified: Tue Apr 16 10:48:40 2024, max compression
```

## Comparing `VASP2KP-1.1.2.tar` & `VASP2KP-1.1.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 shengzhang   (501) staff       (20)        0 2024-04-15 02:34:27.544859 VASP2KP-1.1.2/
--rw-r--r--   0 shengzhang   (501) staff       (20)    35145 2023-12-06 04:04:45.000000 VASP2KP-1.1.2/LICENSE.txt
--rw-r--r--   0 shengzhang   (501) staff       (20)     1205 2024-04-15 02:34:27.544617 VASP2KP-1.1.2/PKG-INFO
--rw-r--r--   0 shengzhang   (501) staff       (20)     1153 2023-12-06 08:17:03.000000 VASP2KP-1.1.2/README.md
-drwxr-xr-x   0 shengzhang   (501) staff       (20)        0 2024-04-15 02:34:27.542833 VASP2KP-1.1.2/VASP2KP/
--rw-r--r--   0 shengzhang   (501) staff       (20)      676 2023-12-06 06:46:55.000000 VASP2KP-1.1.2/VASP2KP/__init__.py
--rw-r--r--   0 shengzhang   (501) staff       (20)    31562 2024-04-15 02:26:54.000000 VASP2KP-1.1.2/VASP2KP/_get_kp_Zeeman.py
--rw-r--r--   0 shengzhang   (501) staff       (20)    64667 2024-04-13 14:49:00.000000 VASP2KP-1.1.2/VASP2KP/_numeric_kp.py
--rw-r--r--   0 shengzhang   (501) staff       (20)    52438 2024-04-15 02:27:19.000000 VASP2KP-1.1.2/VASP2KP/_read_data.py
--rw-r--r--   0 shengzhang   (501) staff       (20)    91234 2024-04-13 14:23:44.000000 VASP2KP-1.1.2/VASP2KP/_standard_kp.py
--rw-r--r--   0 shengzhang   (501) staff       (20)    24467 2024-04-13 10:00:38.000000 VASP2KP-1.1.2/VASP2KP/_transform_matrix.py
-drwxr-xr-x   0 shengzhang   (501) staff       (20)        0 2024-04-15 02:34:27.544304 VASP2KP-1.1.2/VASP2KP.egg-info/
--rw-r--r--   0 shengzhang   (501) staff       (20)     1205 2024-04-15 02:34:27.000000 VASP2KP-1.1.2/VASP2KP.egg-info/PKG-INFO
--rw-r--r--   0 shengzhang   (501) staff       (20)      421 2024-04-15 02:34:27.000000 VASP2KP-1.1.2/VASP2KP.egg-info/SOURCES.txt
--rw-r--r--   0 shengzhang   (501) staff       (20)        1 2024-04-15 02:34:27.000000 VASP2KP-1.1.2/VASP2KP.egg-info/dependency_links.txt
--rw-r--r--   0 shengzhang   (501) staff       (20)        1 2024-04-15 02:34:27.000000 VASP2KP-1.1.2/VASP2KP.egg-info/not-zip-safe
--rw-r--r--   0 shengzhang   (501) staff       (20)       34 2024-04-15 02:34:27.000000 VASP2KP-1.1.2/VASP2KP.egg-info/requires.txt
--rw-r--r--   0 shengzhang   (501) staff       (20)        8 2024-04-15 02:34:27.000000 VASP2KP-1.1.2/VASP2KP.egg-info/top_level.txt
--rwxrwxrwx   0 shengzhang   (501) staff       (20)     8381 2024-04-15 02:27:44.000000 VASP2KP-1.1.2/mat2kp
--rw-r--r--   0 shengzhang   (501) staff       (20)       38 2024-04-15 02:34:27.544908 VASP2KP-1.1.2/setup.cfg
--rw-r--r--   0 shengzhang   (501) staff       (20)     1720 2024-04-15 02:34:23.000000 VASP2KP-1.1.2/setup.py
--rw-r--r--   0 shengzhang   (501) staff       (20)   129670 2023-12-06 06:49:23.000000 VASP2KP-1.1.2/vasp2mat.5.3-patch-1.0.1.sh
--rw-r--r--   0 shengzhang   (501) staff       (20)   128779 2023-12-06 06:50:33.000000 VASP2KP-1.1.2/vasp2mat.6.4-patch-1.0.1.sh
+drwxr-xr-x   0 shengzhang   (501) staff       (20)        0 2024-04-16 10:48:40.839028 VASP2KP-1.1.3/
+-rw-r--r--   0 shengzhang   (501) staff       (20)    35145 2023-12-06 04:04:45.000000 VASP2KP-1.1.3/LICENSE.txt
+-rw-r--r--   0 shengzhang   (501) staff       (20)     1205 2024-04-16 10:48:40.838780 VASP2KP-1.1.3/PKG-INFO
+-rw-r--r--   0 shengzhang   (501) staff       (20)     1153 2023-12-06 08:17:03.000000 VASP2KP-1.1.3/README.md
+drwxr-xr-x   0 shengzhang   (501) staff       (20)        0 2024-04-16 10:48:40.837091 VASP2KP-1.1.3/VASP2KP/
+-rw-r--r--   0 shengzhang   (501) staff       (20)      676 2023-12-06 06:46:55.000000 VASP2KP-1.1.3/VASP2KP/__init__.py
+-rw-r--r--   0 shengzhang   (501) staff       (20)    31562 2024-04-15 02:26:54.000000 VASP2KP-1.1.3/VASP2KP/_get_kp_Zeeman.py
+-rw-r--r--   0 shengzhang   (501) staff       (20)    64667 2024-04-13 14:49:00.000000 VASP2KP-1.1.3/VASP2KP/_numeric_kp.py
+-rw-r--r--   0 shengzhang   (501) staff       (20)    52731 2024-04-16 10:22:04.000000 VASP2KP-1.1.3/VASP2KP/_read_data.py
+-rw-r--r--   0 shengzhang   (501) staff       (20)    91234 2024-04-13 14:23:44.000000 VASP2KP-1.1.3/VASP2KP/_standard_kp.py
+-rw-r--r--   0 shengzhang   (501) staff       (20)    24467 2024-04-13 10:00:38.000000 VASP2KP-1.1.3/VASP2KP/_transform_matrix.py
+drwxr-xr-x   0 shengzhang   (501) staff       (20)        0 2024-04-16 10:48:40.838487 VASP2KP-1.1.3/VASP2KP.egg-info/
+-rw-r--r--   0 shengzhang   (501) staff       (20)     1205 2024-04-16 10:48:40.000000 VASP2KP-1.1.3/VASP2KP.egg-info/PKG-INFO
+-rw-r--r--   0 shengzhang   (501) staff       (20)      421 2024-04-16 10:48:40.000000 VASP2KP-1.1.3/VASP2KP.egg-info/SOURCES.txt
+-rw-r--r--   0 shengzhang   (501) staff       (20)        1 2024-04-16 10:48:40.000000 VASP2KP-1.1.3/VASP2KP.egg-info/dependency_links.txt
+-rw-r--r--   0 shengzhang   (501) staff       (20)        1 2024-04-16 10:48:40.000000 VASP2KP-1.1.3/VASP2KP.egg-info/not-zip-safe
+-rw-r--r--   0 shengzhang   (501) staff       (20)       34 2024-04-16 10:48:40.000000 VASP2KP-1.1.3/VASP2KP.egg-info/requires.txt
+-rw-r--r--   0 shengzhang   (501) staff       (20)        8 2024-04-16 10:48:40.000000 VASP2KP-1.1.3/VASP2KP.egg-info/top_level.txt
+-rwxrwxrwx   0 shengzhang   (501) staff       (20)     8664 2024-04-16 10:47:09.000000 VASP2KP-1.1.3/mat2kp
+-rw-r--r--   0 shengzhang   (501) staff       (20)       38 2024-04-16 10:48:40.839083 VASP2KP-1.1.3/setup.cfg
+-rw-r--r--   0 shengzhang   (501) staff       (20)     1720 2024-04-16 10:47:33.000000 VASP2KP-1.1.3/setup.py
+-rw-r--r--   0 shengzhang   (501) staff       (20)   129670 2023-12-06 06:49:23.000000 VASP2KP-1.1.3/vasp2mat.5.3-patch-1.0.1.sh
+-rw-r--r--   0 shengzhang   (501) staff       (20)   128779 2023-12-06 06:50:33.000000 VASP2KP-1.1.3/vasp2mat.6.4-patch-1.0.1.sh
```

### Comparing `VASP2KP-1.1.2/LICENSE.txt` & `VASP2KP-1.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `VASP2KP-1.1.2/PKG-INFO` & `VASP2KP-1.1.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: VASP2KP
-Version: 1.1.2
+Version: 1.1.3
 Home-page: https://github.com/zjwang11/VASP2KP
 Author: Sheng Zhang, Haohao Sheng, Zhi-Da Song, Chenhao Liang, Zhijun Wang
 Author-email: zhangsheng221@mails.ucas.ac.cn, songzd@pku.edu.cn, wzj@iphy.ac.cn
 License: GPLv3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
```

### Comparing `VASP2KP-1.1.2/README.md` & `VASP2KP-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `VASP2KP-1.1.2/VASP2KP/__init__.py` & `VASP2KP-1.1.3/VASP2KP/__init__.py`

 * *Files identical despite different names*

### Comparing `VASP2KP-1.1.2/VASP2KP/_get_kp_Zeeman.py` & `VASP2KP-1.1.3/VASP2KP/_get_kp_Zeeman.py`

 * *Files identical despite different names*

### Comparing `VASP2KP-1.1.2/VASP2KP/_numeric_kp.py` & `VASP2KP-1.1.3/VASP2KP/_numeric_kp.py`

 * *Files identical despite different names*

### Comparing `VASP2KP-1.1.2/VASP2KP/_read_data.py` & `VASP2KP-1.1.3/VASP2KP/_read_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -514,15 +514,19 @@
     if len(eigen_energy) == 0:
         #raise EIGENVALERROR("ERROR: Empty EIGENVAL file! You should not use EIGENVAL file generated by vasp2mat!!!")
         print("ERROR: Empty EIGENVAL file! You should not use EIGENVAL file generated by vasp2mat!!!")
         sys.exit()
         
     
     
-    
+    if 'repr_matrix' not in list(Symmetry.values())[0].keys():
+        for i in Symmetry.keys():
+            Symmetry[i]['repr_matrix'] = bandreplist2rep(Symmetry[i]['band_repr_matrix_list'])
+            del Symmetry[i]['band_repr_matrix_list']
+            
     operator_name_list = Symmetry.keys()
     
     band_interest_set = get_interest_band_range(os.path.join(folder_path,"MAT_"+list(operator_name_list)[0]+'.m'))
     
     operator = get_opertors_or_data(folder_path,operator_name_list)
                 
     
@@ -541,15 +545,15 @@
     
     if set_vasp_zero or flag_reduce_Symmetry:
         
         eigen_energy_interest = eigen_energy_array[band_interest_set-1]
         
         id_list = list(range(len(eigen_energy_interest)))
         id_list_ = id_list.copy()
- 
+        
         while len(id_list)!= 0:
             i = id_list[0]
             del id_list[0]
             energy = eigen_energy_interest[i]
             for j in id_list:
                 if abs(energy - eigen_energy_interest[j])>eig_cut:
                     for k in operator.keys():
@@ -989,22 +993,22 @@
         
     elif os.path.exists(os.path.join(folder_path,"MAT_sig.m")):
         data = get_opertors_or_data(folder_path,data_name_list)
         
     else:
         print("Warning: No MAT_sig.m file! All spin matrices are set to zero!")
         data_name_list=["Pi"]
+        operator_name_list = list(operator_name_list)
         data = get_opertors_or_data(folder_path,data_name_list)
         data['sigx']=np.zeros_like(operator[operator_name_list[0]],dtype=np.complex128)
         data['sigy']=np.zeros_like(operator[operator_name_list[0]],dtype=np.complex128)
         data['sigz']=np.zeros_like(operator[operator_name_list[0]],dtype=np.complex128)
     
     
 
-                    
     #print("Finish loading data!")
     
     return operator,data,eigen_energy,band_interest_set,dim_list
 ###############################################################################
```

### Comparing `VASP2KP-1.1.2/VASP2KP/_standard_kp.py` & `VASP2KP-1.1.3/VASP2KP/_standard_kp.py`

 * *Files identical despite different names*

### Comparing `VASP2KP-1.1.2/VASP2KP/_transform_matrix.py` & `VASP2KP-1.1.3/VASP2KP/_transform_matrix.py`

 * *Files identical despite different names*

### Comparing `VASP2KP-1.1.2/VASP2KP.egg-info/PKG-INFO` & `VASP2KP-1.1.3/VASP2KP.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: VASP2KP
-Version: 1.1.2
+Version: 1.1.3
 Home-page: https://github.com/zjwang11/VASP2KP
 Author: Sheng Zhang, Haohao Sheng, Zhi-Da Song, Chenhao Liang, Zhijun Wang
 Author-email: zhangsheng221@mails.ucas.ac.cn, songzd@pku.edu.cn, wzj@iphy.ac.cn
 License: GPLv3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
```

### Comparing `VASP2KP-1.1.2/mat2kp` & `VASP2KP-1.1.3/mat2kp`

 * *Files 8% similar despite different names*

```diff
@@ -211,34 +211,35 @@
         vaspMAT = eval(locals_key[vaspMAT_id])
         
     else:
         vaspMAT = 'mat'
 
 if print_flag == 0:
 
-    raise PrintFlagPatchError("Parameter print_flag is set to 0, there will be no output file! Please reset this parameter.")
+    #raise PrintFlagPatchError("Parameter print_flag is set to 0, there will be no output file! Please reset this parameter.")
+    print("Parameter print_flag is set to 0, there will be no output file! Please reset this parameter.")
     sys.exit()
 
 
 elif print_flag == 1:
     print(r"Warning!!! Parameter 'print_flag' is set to 1, all the result will be output on console, not into files!")
     
-    
+
 # calculate the result
 try:
     if no_vasp_kp:
         result_kp, result_Zeeman = \
         get_std_kp_Zeeman_no_coe(Symmetry, order=order, gfactor=gfactor, print_flag=print_flag, log=log, repr_split = repr_split)
     
     else:
         result_kp, result_Zeeman = \
         get_std_kp_Zeeman(Symmetry, vaspMAT, kpmodel=kpmodel, order=order, gfactor=gfactor, print_flag=print_flag, log=log, acc=acc, repr_split = repr_split)
 
 except:
-    pass
+    print("The program unexpectedly encountered an error. We kindly ask you to send us a screenshot of the error and the input files. Email: zhangsheng221@mails.ucas.ac.cn/wzj@iphy.ac.cn")
 
 else:
     print("Congratulations! The computation of VASP2KP has finished!!!")
 
 
 if gfactor == 1 and (not no_vasp_kp) and mathematica_flag:
     mathematica_file = open("kp-Zeeman.nb",'w')
```

### Comparing `VASP2KP-1.1.2/setup.py` & `VASP2KP-1.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from setuptools import setup
 
 README = """A tool for computing k.p effective Hamiltonians and Zeeman's coupling under given symmetry constraints from VASP calculations."""
 
 
 setup(name='VASP2KP',
       python_requires=">=3.6",
-      version = "1.1.2",
+      version = "1.1.3",
       long_description=README,
       install_requires=[
         'sympy', 'numpy', 'scipy', 'kdotp_generator'
         ],
       packages=['VASP2KP'],
       author = 'Sheng Zhang, Haohao Sheng, Zhi-Da Song, Chenhao Liang, Zhijun Wang',
       author_email='zhangsheng221@mails.ucas.ac.cn, songzd@pku.edu.cn, wzj@iphy.ac.cn',
```

### Comparing `VASP2KP-1.1.2/vasp2mat.5.3-patch-1.0.1.sh` & `VASP2KP-1.1.3/vasp2mat.5.3-patch-1.0.1.sh`

 * *Files identical despite different names*

### Comparing `VASP2KP-1.1.2/vasp2mat.6.4-patch-1.0.1.sh` & `VASP2KP-1.1.3/vasp2mat.6.4-patch-1.0.1.sh`

 * *Files identical despite different names*

