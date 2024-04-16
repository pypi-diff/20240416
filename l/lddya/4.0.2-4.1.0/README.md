# Comparing `tmp/lddya-4.0.2.tar.gz` & `tmp/lddya-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lddya-4.0.2.tar", last modified: Thu Apr 11 13:03:05 2024, max compression
+gzip compressed data, was "lddya-4.1.0.tar", last modified: Tue Apr 16 12:35:38 2024, max compression
```

## Comparing `lddya-4.0.2.tar` & `lddya-4.1.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-04-11 13:03:05.934377 lddya-4.0.2/
--rw-rw-rw-   0        0        0      310 2024-04-11 13:03:05.934377 lddya-4.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       74 2021-12-03 06:05:24.000000 lddya-4.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-11 13:03:05.930288 lddya-4.0.2/lddya/
--rw-rw-rw-   0        0        0    22096 2023-09-07 03:20:10.000000 lddya-4.0.2/lddya/Algorithm.py
--rw-rw-rw-   0        0        0     7851 2022-11-01 06:31:16.000000 lddya-4.0.2/lddya/Data.py
--rw-rw-rw-   0        0        0     1444 2022-01-21 14:37:00.000000 lddya-4.0.2/lddya/DataFrame.py
--rw-rw-rw-   0        0        0     2372 2024-04-11 02:41:50.000000 lddya-4.0.2/lddya/Draw.py
--rw-rw-rw-   0        0        0     4893 2022-10-21 12:41:30.000000 lddya-4.0.2/lddya/Map.py
--rw-rw-rw-   0        0        0    16714 2021-12-03 06:05:24.000000 lddya-4.0.2/lddya/Optimizer.py
--rw-rw-rw-   0        0        0       54 2023-09-07 03:17:02.000000 lddya-4.0.2/lddya/__init__.py
--rw-rw-rw-   0        0        0      393 2021-12-03 06:05:24.000000 lddya-4.0.2/lddya/tool.py
-drwxrwxrwx   0        0        0        0 2024-04-11 13:03:05.933374 lddya-4.0.2/lddya.egg-info/
--rw-rw-rw-   0        0        0      310 2024-04-11 13:03:05.000000 lddya-4.0.2/lddya.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      302 2024-04-11 13:03:05.000000 lddya-4.0.2/lddya.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-11 13:03:05.000000 lddya-4.0.2/lddya.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2024-04-11 13:03:05.000000 lddya-4.0.2/lddya.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-04-11 13:03:05.000000 lddya-4.0.2/lddya.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-11 13:03:05.934377 lddya-4.0.2/setup.cfg
--rw-rw-rw-   0        0        0      810 2024-04-11 13:02:41.000000 lddya-4.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-16 12:35:38.145633 lddya-4.1.0/
+-rw-rw-rw-   0        0        0      443 2024-04-16 12:35:38.145633 lddya-4.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0       74 2021-12-03 06:05:24.000000 lddya-4.1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-16 12:35:38.141634 lddya-4.1.0/lddya/
+-rw-rw-rw-   0        0        0    28753 2024-04-16 12:26:50.000000 lddya-4.1.0/lddya/Algorithm.py
+-rw-rw-rw-   0        0        0     7851 2022-11-01 06:31:16.000000 lddya-4.1.0/lddya/Data.py
+-rw-rw-rw-   0        0        0     1444 2022-01-21 14:37:00.000000 lddya-4.1.0/lddya/DataFrame.py
+-rw-rw-rw-   0        0        0     2372 2024-04-11 02:41:50.000000 lddya-4.1.0/lddya/Draw.py
+-rw-rw-rw-   0        0        0     5133 2024-04-16 12:33:50.000000 lddya-4.1.0/lddya/Map.py
+-rw-rw-rw-   0        0        0    16714 2021-12-03 06:05:24.000000 lddya-4.1.0/lddya/Optimizer.py
+-rw-rw-rw-   0        0        0       54 2023-09-07 03:17:02.000000 lddya-4.1.0/lddya/__init__.py
+-rw-rw-rw-   0        0        0      393 2021-12-03 06:05:24.000000 lddya-4.1.0/lddya/tool.py
+drwxrwxrwx   0        0        0        0 2024-04-16 12:35:38.145633 lddya-4.1.0/lddya.egg-info/
+-rw-rw-rw-   0        0        0      443 2024-04-16 12:35:38.000000 lddya-4.1.0/lddya.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      302 2024-04-16 12:35:38.000000 lddya-4.1.0/lddya.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-16 12:35:38.000000 lddya-4.1.0/lddya.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2024-04-16 12:35:38.000000 lddya-4.1.0/lddya.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-16 12:35:38.000000 lddya-4.1.0/lddya.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-16 12:35:38.146656 lddya-4.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      943 2024-04-16 12:35:07.000000 lddya-4.1.0/setup.py
```

### Comparing `lddya-4.0.2/lddya/Algorithm.py` & `lddya-4.1.0/lddya/Algorithm.py`

 * *Files 21% similar despite different names*

```diff
@@ -477,7 +477,129 @@
                 if 0 in v1:               #如果第一个向量是水平或者垂直的,则必存在冗余
                     del child_1[i][index]    #删除被选中的节点
                 elif self.map_data[(point_a[0]+point_c[0])//2,(point_a[1]+point_c[1])//2]==0:                     #如果第一个向量是对角的,且point_a与point_b之间的节点为可通行，则可优化
                     child_1[i][index]  = [(point_a[0]+point_c[0])//2,(point_a[1]+point_c[1])//2]  #修改被选中的节点为中间节点
 
         for i in child_1:                     #交叉后的染色体个体加入子代群集中
             self.child_list.append(i)
+
+class Dynamic_Programing():
+    def __init__(self,map_data,start = [0,0],end= [19,19]) -> None:
+        '''
+            Function
+            --------
+            parameter initilization
+
+            Parameter
+            --------
+            map_data : 栅格地图数据，   2d矩阵
+            start    : 起点坐标，      1*2向量 [y,x]
+            end      : 终点坐标，      1*2向量 [y,x]
+
+            Return
+            ------
+            None
+        '''
+        self.map_data = map_data
+        self.map_size = map_data.shape[0]
+        self.start = start
+        self.end = end
+        self.relation_matrix = np.zeros_like(self.map_data,dtype = np.int16)   #关系矩阵，标记方向
+        self.relation_code_zhi = np.array([1,3,5,7])          #回溯方向代码，放入关系矩阵中
+        self.relation_code_xie = np.array([2,4,6,8])
+        self.dynamic_matrix  = np.zeros_like(self.map_data)   #动态矩阵，标记需要处理的母节点
+        self.dynamic_matrix[self.end[0],self.end[0]] = 1   #初始时，母节点仅有终点
+        self.static_matrix   = self.dynamic_matrix.copy()   #静态矩阵，冻结的节点(不进行任何操作)
+
+    
+    def run(self):
+        while True:
+            self.relation_matrix_temp = np.zeros_like(self.relation_matrix)
+            self.dynamic_matrix_temp  = np.zeros_like(self.dynamic_matrix) 
+            # step 1: 由需要处理的母节点进行扩散
+            self.task_matrix = np.zeros_like(self.map_data)
+            #self.task_2_matrix = np.zeros(shape=np.array(self.map_data.shape)+2)    #扩大点，就不用考虑边界了，task
+            y_1,x_1 = np.where(self.dynamic_matrix==1)
+            for k,i in enumerate(y_1):      #直线方向上的更新
+                y = y_1[k]
+                x = x_1[k]
+                neighbours = np.array([
+                    [y-1,x],
+                    [y,x+1],
+                    [y+1,x],
+                    [y,x-1],
+                ])
+                cond_1 = np.logical_and(neighbours[:,0]>=0,neighbours[:,0]<self.map_size)
+                cond_2 = np.logical_and(neighbours[:,1]>=0,neighbours[:,1]<self.map_size)
+                allowed_index = np.logical_and(cond_1,cond_2)          #约束1：坐标范围
+                allowed_rela_code = self.relation_code_zhi[allowed_index]
+                allowed_neigh = neighbours[allowed_index]
+                allowed_rela_code = allowed_rela_code[self.map_data[allowed_neigh[:,0],allowed_neigh[:,1]]==0] #约束2的code，因为allowed_neigh下一步变了，故要提前处理code，约束3的同理
+                allowed_neigh = allowed_neigh[self.map_data[allowed_neigh[:,0],allowed_neigh[:,1]]==0]     #约束2 ： 空白栅格
+                allowed_rela_code = allowed_rela_code[self.static_matrix[allowed_neigh[:,0],allowed_neigh[:,1]]==0]
+                allowed_neigh = allowed_neigh[self.static_matrix[allowed_neigh[:,0],allowed_neigh[:,1]]==0]  #约束3： 不能是static
+                
+                a_1 = self.relation_matrix[allowed_neigh[:,0],allowed_neigh[:,1]] == 0  # 没更新的地方,需要判断吗？
+                self.relation_matrix_temp[allowed_neigh[a_1][:,0],allowed_neigh[a_1][:,1]] = allowed_rela_code[a_1]
+                self.relation_matrix[self.relation_matrix_temp!=0] = self.relation_matrix_temp[self.relation_matrix_temp!=0]
+                self.dynamic_matrix_temp[self.relation_matrix_temp!=0] = 1 
+            
+            self.relation_matrix_temp = np.zeros_like(self.relation_matrix)
+            for k,i in enumerate(y_1):      #斜线方向上的更新
+                y = y_1[k]
+                x = x_1[k]
+                neighbours = np.array([
+                    [y-1,x+1],
+                    [y+1,x+1],
+                    [y+1,x-1],
+                    [y-1,x-1]
+                ])
+                cond_1 = np.logical_and(neighbours[:,0]>=0,neighbours[:,0]<self.map_size)
+                cond_2 = np.logical_and(neighbours[:,1]>=0,neighbours[:,1]<self.map_size)
+                allowed_index = np.logical_and(cond_1,cond_2)
+                allowed_rela_code = self.relation_code_xie[allowed_index]
+                allowed_neigh = neighbours[allowed_index]
+                allowed_rela_code = allowed_rela_code[self.map_data[allowed_neigh[:,0],allowed_neigh[:,1]]==0] #约束2的code，因为allowed_neigh下一步变了，故要提前处理code，约束3的同理
+                allowed_neigh = allowed_neigh[self.map_data[allowed_neigh[:,0],allowed_neigh[:,1]]==0]     #约束2 ： 空白栅格
+                allowed_rela_code = allowed_rela_code[self.static_matrix[allowed_neigh[:,0],allowed_neigh[:,1]]==0]
+                allowed_neigh = allowed_neigh[self.static_matrix[allowed_neigh[:,0],allowed_neigh[:,1]]==0]  #约束3： 不能是static
+                a_1 = self.relation_matrix[allowed_neigh[:,0],allowed_neigh[:,1]] == 0  # 没更新的地方,需要判断吗？
+                self.relation_matrix_temp[allowed_neigh[a_1][:,0],allowed_neigh[a_1][:,1]] = allowed_rela_code[a_1] 
+                self.relation_matrix[self.relation_matrix_temp!=0] = self.relation_matrix_temp[self.relation_matrix_temp!=0]
+                self.dynamic_matrix_temp[self.relation_matrix_temp!=0] = 1 
+            
+            
+            self.dynamic_matrix = self.dynamic_matrix_temp.copy()   #更新下一轮的母节点(动态矩阵)
+            self.static_matrix[self.dynamic_matrix!=0] = 1   #本轮的母节点全部冻结
+            if self.static_matrix[self.start[0],self.start[1]] !=0:
+                print('路径规划完成！')
+                self._translate()
+                break
+
+
+    def _translate(self):
+        self.way_data_best = []
+        self.way_len_best = 0
+        grid = self.start.copy()
+        self.way_data_best.append(grid)
+        while True:
+            change_matrix = np.array([
+                [1,0],
+                [1,-1],
+                [0,-1],
+                [-1,-1],
+                [-1,0],
+                [-1,1],
+                [0,1],
+                [1,1]
+            ])
+
+            grid = grid+change_matrix[self.relation_matrix[grid[0],grid[1]]-1]
+            if 0 in change_matrix[self.relation_matrix[grid[0],grid[1]]-1].tolist():
+                self.way_len_best += 1
+            else:
+                self.way_len_best += 2**0.5
+            self.way_data_best.append(grid)
+            if (grid == self.end).all():
+                self.way_data_best = np.array(self.way_data_best)
+                break
+
```

### Comparing `lddya-4.0.2/lddya/Data.py` & `lddya-4.1.0/lddya/Data.py`

 * *Files identical despite different names*

### Comparing `lddya-4.0.2/lddya/DataFrame.py` & `lddya-4.1.0/lddya/DataFrame.py`

 * *Files identical despite different names*

### Comparing `lddya-4.0.2/lddya/Draw.py` & `lddya-4.1.0/lddya/Draw.py`

 * *Files identical despite different names*

### Comparing `lddya-4.0.2/lddya/Map.py` & `lddya-4.1.0/lddya/Map.py`

 * *Files 18% similar despite different names*

```diff
@@ -119,15 +119,21 @@
                 s+=str(j)
             s+='\n'
             str_data.append(s)
         with open(fp,'w')  as f:
             f.writelines(str_data)
         
             
-
+    def gen_random_map(self,p=0.1,size = 20):
+        p = 1-p
+        self.data = np.random.rand(size,size)
+        self.data[self.data<=p] = 0
+        self.data[self.data>p] = 1
+        self.data[0,0] = 0
+        self.data[-1,-1] = 0
```

### Comparing `lddya-4.0.2/lddya/Optimizer.py` & `lddya-4.1.0/lddya/Optimizer.py`

 * *Files identical despite different names*

### Comparing `lddya-4.0.2/setup.py` & `lddya-4.1.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 ############################################
 
 
 from setuptools import setup, find_packages
 
 setup(
     name = "lddya",
-    version = "4.0.2",
+    version = "4.1.0",
     keywords = {"pip", "license","licensetool", "tool", "gm"},
-    description = "新增了优化器类别",
+    description = "1.Map添加生成随机地图的功能，仅提供生成，暂不提供验证，也就是可能会产生无路径的极端情况。2.添加动态规划法。",
     long_description = "具体功能，请自行挖掘。",
     license = "MIT Licence",
 
     url = "https://github.com/not_define/please_wait",
     author = "lidongdong",
     author_email = "927052521@qq.com",
```

