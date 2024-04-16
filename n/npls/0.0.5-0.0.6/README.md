# Comparing `tmp/npls-0.0.5.tar.gz` & `tmp/npls-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "npls-0.0.5.tar", last modified: Sun Mar 17 01:00:07 2024, max compression
+gzip compressed data, was "npls-0.0.6.tar", last modified: Tue Apr 16 19:57:56 2024, max compression
```

## Comparing `npls-0.0.5.tar` & `npls-0.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 ferubkomsu  (1000) ferubkomsu  (1000)        0 2024-03-17 01:00:07.678685 npls-0.0.5/
--rw-rw-r--   0 ferubkomsu  (1000) ferubkomsu  (1000)    35149 2023-09-25 21:00:46.000000 npls-0.0.5/LICENSE
--rw-rw-r--   0 ferubkomsu  (1000) ferubkomsu  (1000)     3779 2024-03-17 01:00:07.678685 npls-0.0.5/PKG-INFO
--rw-rw-r--   0 ferubkomsu  (1000) ferubkomsu  (1000)     2622 2024-03-17 00:58:00.000000 npls-0.0.5/README.md
-drwxrwxr-x   0 ferubkomsu  (1000) ferubkomsu  (1000)        0 2024-03-17 01:00:07.670685 npls-0.0.5/npls/
--rw-rw-r--   0 ferubkomsu  (1000) ferubkomsu  (1000)      133 2024-03-17 00:46:32.000000 npls-0.0.5/npls/__init__.py
--rw-rw-r--   0 ferubkomsu  (1000) ferubkomsu  (1000)     6481 2024-03-17 00:46:21.000000 npls-0.0.5/npls/npls.py
-drwxrwxr-x   0 ferubkomsu  (1000) ferubkomsu  (1000)        0 2024-03-17 01:00:07.678685 npls-0.0.5/npls.egg-info/
--rw-rw-r--   0 ferubkomsu  (1000) ferubkomsu  (1000)     3779 2024-03-17 01:00:07.000000 npls-0.0.5/npls.egg-info/PKG-INFO
--rw-rw-r--   0 ferubkomsu  (1000) ferubkomsu  (1000)      205 2024-03-17 01:00:07.000000 npls-0.0.5/npls.egg-info/SOURCES.txt
--rw-rw-r--   0 ferubkomsu  (1000) ferubkomsu  (1000)        1 2024-03-17 01:00:07.000000 npls-0.0.5/npls.egg-info/dependency_links.txt
--rw-rw-r--   0 ferubkomsu  (1000) ferubkomsu  (1000)       32 2024-03-17 01:00:07.000000 npls-0.0.5/npls.egg-info/requires.txt
--rw-rw-r--   0 ferubkomsu  (1000) ferubkomsu  (1000)        5 2024-03-17 01:00:07.000000 npls-0.0.5/npls.egg-info/top_level.txt
--rw-rw-r--   0 ferubkomsu  (1000) ferubkomsu  (1000)       38 2024-03-17 01:00:07.678685 npls-0.0.5/setup.cfg
--rw-rw-r--   0 ferubkomsu  (1000) ferubkomsu  (1000)     1621 2024-03-17 00:59:06.000000 npls-0.0.5/setup.py
+drwxrwxr-x   0 ferubkomsu  (1000) ferubkomsu  (1000)        0 2024-04-16 19:57:56.659542 npls-0.0.6/
+-rw-rw-r--   0 ferubkomsu  (1000) ferubkomsu  (1000)    35149 2023-09-25 21:00:46.000000 npls-0.0.6/LICENSE
+-rw-rw-r--   0 ferubkomsu  (1000) ferubkomsu  (1000)     4366 2024-04-16 19:57:56.659542 npls-0.0.6/PKG-INFO
+-rw-rw-r--   0 ferubkomsu  (1000) ferubkomsu  (1000)     3209 2024-04-16 19:55:31.000000 npls-0.0.6/README.md
+drwxrwxr-x   0 ferubkomsu  (1000) ferubkomsu  (1000)        0 2024-04-16 19:57:56.659542 npls-0.0.6/npls/
+-rw-rw-r--   0 ferubkomsu  (1000) ferubkomsu  (1000)      133 2024-04-16 19:55:48.000000 npls-0.0.6/npls/__init__.py
+-rw-rw-r--   0 ferubkomsu  (1000) ferubkomsu  (1000)     6687 2024-04-16 19:55:36.000000 npls-0.0.6/npls/npls.py
+drwxrwxr-x   0 ferubkomsu  (1000) ferubkomsu  (1000)        0 2024-04-16 19:57:56.659542 npls-0.0.6/npls.egg-info/
+-rw-rw-r--   0 ferubkomsu  (1000) ferubkomsu  (1000)     4366 2024-04-16 19:57:56.000000 npls-0.0.6/npls.egg-info/PKG-INFO
+-rw-rw-r--   0 ferubkomsu  (1000) ferubkomsu  (1000)      205 2024-04-16 19:57:56.000000 npls-0.0.6/npls.egg-info/SOURCES.txt
+-rw-rw-r--   0 ferubkomsu  (1000) ferubkomsu  (1000)        1 2024-04-16 19:57:56.000000 npls-0.0.6/npls.egg-info/dependency_links.txt
+-rw-rw-r--   0 ferubkomsu  (1000) ferubkomsu  (1000)       32 2024-04-16 19:57:56.000000 npls-0.0.6/npls.egg-info/requires.txt
+-rw-rw-r--   0 ferubkomsu  (1000) ferubkomsu  (1000)        5 2024-04-16 19:57:56.000000 npls-0.0.6/npls.egg-info/top_level.txt
+-rw-rw-r--   0 ferubkomsu  (1000) ferubkomsu  (1000)       38 2024-04-16 19:57:56.663542 npls-0.0.6/setup.cfg
+-rw-rw-r--   0 ferubkomsu  (1000) ferubkomsu  (1000)     1621 2024-04-16 19:56:39.000000 npls-0.0.6/setup.py
```

### Comparing `npls-0.0.5/LICENSE` & `npls-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `npls-0.0.5/PKG-INFO` & `npls-0.0.6/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: npls
-Version: 0.0.5
+Version: 0.0.6
 Summary: It is a Python library for the N-PLS1 regression with L1 and L2-regularization.
 Home-page: https://github.com/89605502155/npls
 Author: ['Andrey Ferubko', 'Ivan Krylov']
 Author-email: ferubko1999@yandex.ru
 License: GNU General Public License v3.0
 Download-URL: https://github.com/89605502155/npls/archive/main.zip
 Platform: UNKNOWN
@@ -48,23 +48,41 @@
 
 You can fit your own regression model. n_components - is a number of components of SVD decomposition and l2 is a parameter of L2-regularization (Ridge) and l1 is a parameter of L1-regularization (LASSO), excitation_wavelenth - is an 
 excitation wavelenth of fluor. (if you have not excitation wavelenth you can write list with len equal first shape of X_train),emission_wavelenth is an emission wavelenth. X_train - is a 3d-array. y_train -is a vector.
 
 ```python
 from npls import npls 
 
-model=npls(n_components=4, l2=0.09,excitation_wavelenth=[501,552],emission_wavelenth=[553,604])
+model=npls(n_components=4, l2=0.09)
 model.fit(X_train,y_train)
 #components of svd-decomposition
 w_i=model.w_i
 w_k=model.w_k
 #predict
 y_predicted=model.predict(X_test)
 ```
 
+If you want to use snr, you need input excitation_wavelenth and emission_wavelenth,
+        crash_norm_name and crash_norm_value and norm_func and derivative_rang.
+        Example:
+```python
+from npls import npls 
+model=npls(crash_norm_name='evklid',derivative_rang=[1],
+    emission_wavelenth=np.array([1,2,3]),
+    excitation_wavelenth=np.array([1,2,3]),
+    crash_norm_value=9)
+```
+and with use L2 and N components:
+```python
+from npls import npls 
+model=npls(crash_norm_name='evklid',derivative_rang=[1],
+    emission_wavelenth=np.array([1,2,3]),
+    excitation_wavelenth=np.array([1,2,3]),
+    crash_norm_value=9,n_components=4, l2=0.09)
+```
 ## Example
 
 You can use this library with Scikit-learn library. For example, we can use GridSearchCV.
 
 *If you installed a module from PyPi, you should to import it like this: ``` from npls import npls  ```*
 
 *If from GitHub or source: ``` from npls import npls ```*
```

### Comparing `npls-0.0.5/README.md` & `npls-0.0.6/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -22,23 +22,41 @@
 
 You can fit your own regression model. n_components - is a number of components of SVD decomposition and l2 is a parameter of L2-regularization (Ridge) and l1 is a parameter of L1-regularization (LASSO), excitation_wavelenth - is an 
 excitation wavelenth of fluor. (if you have not excitation wavelenth you can write list with len equal first shape of X_train),emission_wavelenth is an emission wavelenth. X_train - is a 3d-array. y_train -is a vector.
 
 ```python
 from npls import npls 
 
-model=npls(n_components=4, l2=0.09,excitation_wavelenth=[501,552],emission_wavelenth=[553,604])
+model=npls(n_components=4, l2=0.09)
 model.fit(X_train,y_train)
 #components of svd-decomposition
 w_i=model.w_i
 w_k=model.w_k
 #predict
 y_predicted=model.predict(X_test)
 ```
 
+If you want to use snr, you need input excitation_wavelenth and emission_wavelenth,
+        crash_norm_name and crash_norm_value and norm_func and derivative_rang.
+        Example:
+```python
+from npls import npls 
+model=npls(crash_norm_name='evklid',derivative_rang=[1],
+    emission_wavelenth=np.array([1,2,3]),
+    excitation_wavelenth=np.array([1,2,3]),
+    crash_norm_value=9)
+```
+and with use L2 and N components:
+```python
+from npls import npls 
+model=npls(crash_norm_name='evklid',derivative_rang=[1],
+    emission_wavelenth=np.array([1,2,3]),
+    excitation_wavelenth=np.array([1,2,3]),
+    crash_norm_value=9,n_components=4, l2=0.09)
+```
 ## Example
 
 You can use this library with Scikit-learn library. For example, we can use GridSearchCV.
 
 *If you installed a module from PyPi, you should to import it like this: ``` from npls import npls  ```*
 
 *If from GitHub or source: ``` from npls import npls ```*
```

### Comparing `npls-0.0.5/npls/npls.py` & `npls-0.0.6/npls/npls.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,35 +1,46 @@
 import numpy as np
 from sklearn.base import BaseEstimator
 from sklearn.base import RegressorMixin
 from signal_noise import signal_noise
 
 class npls(RegressorMixin,BaseEstimator):
-    def  __init__(self, excitation_wavelenth:np.ndarray,
-                  emission_wavelenth:np.ndarray,l1:float=None, n_components:int=2,l2:float=3,
+    def  __init__(self, excitation_wavelenth:np.ndarray=np.array([0]),
+                  emission_wavelenth:np.ndarray=np.array([0]), n_components:int=2,a:float=3,
                   derivative_rang:list=[],norm_func:list=[],
                   crash_norm_name:str=None,crash_norm_value:float=None):
+        """
+        If you want to use snr, you need input excitation_wavelenth and emission_wavelenth,
+        crash_norm_name and crash_norm_value and norm_func and derivative_rang.
+        Example:
+
+        m=npls(crash_norm_name='evklid',derivative_rang=[1],
+         emission_wavelenth=np.array([1,2,3]),
+         excitation_wavelenth=np.array([1,2,3]),
+         crash_norm_value=9)
+        """
         self.n_components = n_components
-        self.l2=l2
-        self.l1=l1
+        self.a=a
         self.derivative_rang=derivative_rang
         self.norm_func=norm_func
         self.crash_norm_name=crash_norm_name
         self.crash_norm_value=crash_norm_value
         self.excitation_wavelenth=excitation_wavelenth
         self.emission_wavelenth=emission_wavelenth
 
-    def check_smooth_loadings(self,w_i,excitation_wavelenth,
+    def __check_smooth_loadings(self,w_i,excitation_wavelenth,
                               w_k,emission_wavelenth, n_component:int) -> dict[str,dict]:
         # print(w_i.shape,excitation_wavelenth.shape,
         #                       w_k.shape,emission_wavelenth.shape, n_component)
-        resp_emission=self.chek_smooth_one_model(w_k,emission_wavelenth)
-        resp_excitation=self.chek_smooth_one_model(w_i,excitation_wavelenth)
+        resp_emission=self.__chek_smooth_one_model(w_k,emission_wavelenth)
+        resp_excitation=self.__chek_smooth_one_model(w_i,excitation_wavelenth)
         if self.crash_norm_name is not None:
+            #print(resp_emission,self.crash_norm_name,resp_emission[self.crash_norm_name],resp_excitation[self.crash_norm_name])
             for j in range(len(resp_emission[self.crash_norm_name])):
+                #print(resp_emission[self.crash_norm_name][j])
                 if resp_emission[self.crash_norm_name][j]<=self.crash_norm_value:
                     error_message_1=f'Emission {n_component} component is a very noisy.'
                     error_message_2=' May be you can choose another norm.'
                     error_message_3=f' Now you choose {self.crash_norm_name} norm'
                     error_message=error_message_1+error_message_2+error_message_3
                     raise ValueError(error_message)
                 if resp_excitation[self.crash_norm_name][j]<=self.crash_norm_value:
@@ -40,26 +51,20 @@
                     raise ValueError(error_message)
         return {
             "Emission":resp_emission,
             "Excitation":resp_excitation
             }
 
 
-    def chek_smooth_one_model(self,signal,x) -> dict[str, list]:
-        model=signal_noise(derivative_rang=self.derivative_rang,
-                                    norm_func=self.norm_func)
+    def __chek_smooth_one_model(self,signal,x) -> dict[str, list]:
+        model=signal_noise()
         response=model.main(signal=signal,x=x)
+        #print(response,signal,x)
         return response
 
-    def l1_regularization(self,vector:np.ndarray)->np.ndarray:
-      for i in range(vector.shape[0]):
-        if abs(vector[i])<=self.l1:
-          vector[i]=0
-      return vector
-    
     def fit(self, xtrain, ytrain):
         """Fits the model to the data (X, y)
         Parameters
         ----------
         X : ndarray
         y : 1D-array of shape (n_samples, )
             labels associated with each sample
@@ -87,31 +92,28 @@
             x_product=np.zeros([x.shape[0],x.shape[1],x.shape[2]])
             for i in range(0,x.shape[0]):
                 x_product[i,:,:]=y[i]*x[i,:,:]
             z=x_product.sum(axis=0)
             Wk, S, WI = np.linalg.svd(z)
             w_k=np.array(Wk[:,0]).reshape(x.shape[1],1)
             w_i=np.array(WI[0,:]).reshape(x.shape[2],1)
-            if self.l1 is not None:
-              w_k=self.l1_regularization(w_k)
-              w_i=self.l1_regularization(w_i)
-              
+
             if len(self.derivative_rang)>0:
-                response=self.check_smooth_loadings(w_i=w_i[:,0],excitation_wavelenth=self.excitation_wavelenth,
+                response=self.__check_smooth_loadings(w_i=w_i[:,0],excitation_wavelenth=self.excitation_wavelenth,
                                            w_k=w_k[:,0],emission_wavelenth=self.emission_wavelenth,
                                            n_component=f)
                 self.snr_emission.append(response['Emission'])
                 self.snr_excitation.append(response['Excitation'])
 
             w_k_mass[f,:,:]=w_k
             w_i_mass[f,:,:]=w_i
             for h in range(0,x.shape[0]):
                 Tt[h,f]=np.dot(np.dot(w_i.transpose(),x[h,:,:].transpose()),w_k)
             T=np.array(Tt[:,0:f+1]).reshape(x.shape[0],f+1)
-            bf=np.dot((np.dot(np.linalg.inv(np.dot(T,T.transpose())-(((self.l2))*np.eye(x.shape[0]))),T)).transpose(),
+            bf=np.dot((np.dot(np.linalg.inv(np.dot(T,T.transpose())-(((self.a))*np.eye(x.shape[0]))),T)).transpose(),
                         y.reshape([x.shape[0],1]))
             bf_array+=[bf]
             WW=np.kron(w_k,w_i).reshape(x.shape[1],x.shape[2])
             for g in range(0,x.shape[0]):
                 mmas[g,:,:]=Tt[g,f]*WW
             x=np.array(x-(mmas))
             y=(y-(np.dot(T,bf)).reshape(x.shape[0]))
@@ -138,7 +140,8 @@
             WW=np.kron(w_k,w_i).reshape(x.shape[1],x.shape[2])
             for g in range(0,x.shape[0]):
                 mmas[g,:,:]=Tt[g,f]*WW
             x=np.array(x-(mmas))
             y=(y+(np.dot(T,self.bf_array[f])).reshape(x.shape[0]))
         return y
 
+
```

### Comparing `npls-0.0.5/npls.egg-info/PKG-INFO` & `npls-0.0.6/npls.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: npls
-Version: 0.0.5
+Version: 0.0.6
 Summary: It is a Python library for the N-PLS1 regression with L1 and L2-regularization.
 Home-page: https://github.com/89605502155/npls
 Author: ['Andrey Ferubko', 'Ivan Krylov']
 Author-email: ferubko1999@yandex.ru
 License: GNU General Public License v3.0
 Download-URL: https://github.com/89605502155/npls/archive/main.zip
 Platform: UNKNOWN
@@ -48,23 +48,41 @@
 
 You can fit your own regression model. n_components - is a number of components of SVD decomposition and l2 is a parameter of L2-regularization (Ridge) and l1 is a parameter of L1-regularization (LASSO), excitation_wavelenth - is an 
 excitation wavelenth of fluor. (if you have not excitation wavelenth you can write list with len equal first shape of X_train),emission_wavelenth is an emission wavelenth. X_train - is a 3d-array. y_train -is a vector.
 
 ```python
 from npls import npls 
 
-model=npls(n_components=4, l2=0.09,excitation_wavelenth=[501,552],emission_wavelenth=[553,604])
+model=npls(n_components=4, l2=0.09)
 model.fit(X_train,y_train)
 #components of svd-decomposition
 w_i=model.w_i
 w_k=model.w_k
 #predict
 y_predicted=model.predict(X_test)
 ```
 
+If you want to use snr, you need input excitation_wavelenth and emission_wavelenth,
+        crash_norm_name and crash_norm_value and norm_func and derivative_rang.
+        Example:
+```python
+from npls import npls 
+model=npls(crash_norm_name='evklid',derivative_rang=[1],
+    emission_wavelenth=np.array([1,2,3]),
+    excitation_wavelenth=np.array([1,2,3]),
+    crash_norm_value=9)
+```
+and with use L2 and N components:
+```python
+from npls import npls 
+model=npls(crash_norm_name='evklid',derivative_rang=[1],
+    emission_wavelenth=np.array([1,2,3]),
+    excitation_wavelenth=np.array([1,2,3]),
+    crash_norm_value=9,n_components=4, l2=0.09)
+```
 ## Example
 
 You can use this library with Scikit-learn library. For example, we can use GridSearchCV.
 
 *If you installed a module from PyPi, you should to import it like this: ``` from npls import npls  ```*
 
 *If from GitHub or source: ``` from npls import npls ```*
```

### Comparing `npls-0.0.5/setup.py` & `npls-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from io import open
 from setuptools import setup
 
 
-version = '0.0.5'
+version = '0.0.6'
 
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='npls',
     version=version,
```

